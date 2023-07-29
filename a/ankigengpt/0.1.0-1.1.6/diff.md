# Comparing `tmp/ankigengpt-0.1.0-py3-none-any.whl.zip` & `tmp/ankigengpt-1.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 8855 bytes, number of entries: 18
+Zip file size: 9251 bytes, number of entries: 18
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 ankigengpt/__init__.py
 -rw-r--r--  2.0 unx      133 b- defN 80-Jan-01 00:00 ankigengpt/__main__.py
--rw-r--r--  2.0 unx     1247 b- defN 80-Jan-01 00:00 ankigengpt/anki.py
--rw-r--r--  2.0 unx     2486 b- defN 80-Jan-01 00:00 ankigengpt/cli.py
+-rw-r--r--  2.0 unx     1904 b- defN 80-Jan-01 00:00 ankigengpt/anki.py
+-rw-r--r--  2.0 unx     2605 b- defN 80-Jan-01 00:00 ankigengpt/cli.py
 -rw-r--r--  2.0 unx      837 b- defN 80-Jan-01 00:00 ankigengpt/epub.py
--rw-r--r--  2.0 unx     3751 b- defN 80-Jan-01 00:00 ankigengpt/gpt.py
+-rw-r--r--  2.0 unx     4009 b- defN 80-Jan-01 00:00 ankigengpt/gpt.py
 -rw-r--r--  2.0 unx      753 b- defN 80-Jan-01 00:00 ankigengpt/kindle.py
 -rw-r--r--  2.0 unx      664 b- defN 80-Jan-01 00:00 ankigengpt/logging.py
 -rw-r--r--  2.0 unx      103 b- defN 80-Jan-01 00:00 ankigengpt/misc.py
 -rw-r--r--  2.0 unx      473 b- defN 80-Jan-01 00:00 ankigengpt/templates/__init__.py
 -rw-r--r--  2.0 unx       66 b- defN 80-Jan-01 00:00 ankigengpt/templates/epub.j2
--rw-r--r--  2.0 unx     1156 b- defN 80-Jan-01 00:00 ankigengpt/templates/introduction.j2
+-rw-r--r--  2.0 unx     1174 b- defN 80-Jan-01 00:00 ankigengpt/templates/introduction.j2
 -rw-r--r--  2.0 unx       32 b- defN 80-Jan-01 00:00 ankigengpt/templates/kindle.j2
 -rw-r--r--  2.0 unx       32 b- defN 80-Jan-01 00:00 ankigengpt/templates/plain.j2
--rw-r--r--  2.0 unx     1642 b- defN 80-Jan-01 00:00 ankigengpt-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 ankigengpt-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 80-Jan-01 00:00 ankigengpt-0.1.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1424 b- defN 16-Jan-01 00:00 ankigengpt-0.1.0.dist-info/RECORD
-18 files, 14942 bytes uncompressed, 6523 bytes compressed:  56.3%
+-rw-r--r--  2.0 unx     1684 b- defN 80-Jan-01 00:00 ankigengpt-1.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 ankigengpt-1.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 80-Jan-01 00:00 ankigengpt-1.1.6.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1424 b- defN 16-Jan-01 00:00 ankigengpt-1.1.6.dist-info/RECORD
+18 files, 16036 bytes uncompressed, 6919 bytes compressed:  56.9%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: ankigengpt/templates/kindle.j2
 Comment: 
 
 Filename: ankigengpt/templates/plain.j2
 Comment: 
 
-Filename: ankigengpt-0.1.0.dist-info/METADATA
+Filename: ankigengpt-1.1.6.dist-info/METADATA
 Comment: 
 
-Filename: ankigengpt-0.1.0.dist-info/WHEEL
+Filename: ankigengpt-1.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: ankigengpt-0.1.0.dist-info/entry_points.txt
+Filename: ankigengpt-1.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: ankigengpt-0.1.0.dist-info/RECORD
+Filename: ankigengpt-1.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ankigengpt/anki.py

```diff
@@ -15,27 +15,37 @@
 
 @dataclass
 class DeckInput:
     name: str
     cards: list[AnkiCard]
 
 
-def gpt_answer_to_cards(answer: str, source: str) -> list[AnkiCard]:
+def split_gpt_answer(answer: str) -> list[str]:
+    '''Splits list into dicts'''
+    splitted = []
+    for pair in answer.split('\n-'):
+        splitted.append(
+            '\n'.join([i.replace('-', '').strip() for i in pair.split('\n')])
+        )
+    return splitted
+
+
+def gpt_answer_to_cards(answer: str, source: str) -> AnkiCard:
     data = yaml.safe_load(answer)
-    return [AnkiCard(i['question'], i['answer'], source) for i in data]
+    return AnkiCard(data['question'], data['answer'], source)
 
 
 def generate_deck(input: DeckInput, dest: Path) -> None:
     my_deck = genanki.Deck(
         deck_id=random.randrange(11111111, 99999999, 8), name=input.name
     )
 
     for card in input.cards:
         my_note = genanki.Note(
-            model=anki_model, fields=[card.front, card.back, card.source]
+            model=anki_model, fields=[card.front, card.back, 'Source: ' + card.source]
         )
         my_deck.add_note(my_note)
 
     package = genanki.Package(my_deck)
 
     package.write_to_file(dest.joinpath(input.name + '.apkg'))
 
@@ -47,12 +57,24 @@
         {'name': 'Front'},
         {'name': 'Back'},
         {'name': 'Source'},
     ],
     templates=[
         {
             'name': 'Card 1',
-            'qfmt': '{{Front}}',
-            'afmt': '{{Front}}<br>{{Back}}<br>{{Source}}',
+            'qfmt': '<div class="front-back">{{Front}}</div>',
+            'afmt': '<div class="front-back">{{Front}}</div><br><div class="front-back">{{Back}}</div><br><div class="source">{{Source}}</div>',  # noqa
         },
     ],
+    css='''
+        .source {
+            font-size: 0.5em;
+            margin-top: 20px;
+            text-align: center;
+        }
+        .front-back {
+            font-size: 1.3em;
+            margin-top: 20px;
+            text-align: center;
+        }
+    ''',
 )
```

## ankigengpt/cli.py

```diff
@@ -37,18 +37,21 @@
     openai_token: str = typer.Option(..., envvar='OPENAI_TOKEN'),
     debug: bool = typer.Option(False),
     path: Path = typer.Option(..., help='Path to text file'),
     dest: Path = typer.Option(Path().cwd, help='Destination directory'),
 ):
     init_logger(debug)
     with open(path) as f:
-        content = f.readlines()
-    cards = _generate_cards_until_finish(
-        template_plain, content, openai_token, cards_source=path.name
-    )
+        raw = f.read()
+        # remove markdown double new line
+        raw = raw.replace('\n\n', '\n')
+        content = raw.split('\n')
+        cards = _generate_cards_until_finish(
+            template_plain, content, openai_token, cards_source=path.name
+        )
     ankiInput = DeckInput(path.name, cards)
     generate_deck(ankiInput, dest)
 
 
 @app.command()
 def epub(
     openai_token: str = typer.Option(..., envvar='OPENAI_TOKEN'),
```

## ankigengpt/gpt.py

```diff
@@ -1,16 +1,21 @@
 import openai
 import tiktoken
 from jinja2 import Template
+from ratelimit import limits, sleep_and_retry
 from rich.progress import Progress
 
-from ankigengpt.anki import AnkiCard, gpt_answer_to_cards
+from ankigengpt.anki import AnkiCard, gpt_answer_to_cards, split_gpt_answer
 from ankigengpt.logging import logger
 
+ONE_MINUTE = 60
 
+
+@sleep_and_retry
+@limits(3, period=ONE_MINUTE)
 def prompt_openai(
     token: str,
     prompt: str,
     temperature=1.0,
     frequency_penalty=0.0,
     presence_penalty=1.0,
     # model='gpt-3.5-turbo',
@@ -33,15 +38,15 @@
         # Number between -2.0 and 2.0. Positive values penalize new tokens based on
         # whether they appear in the text so far, increasing the model's
         # likelihood to talk about new topics.
         presence_penalty=presence_penalty,
     )
     content = client.choices[0].message.content
     logger.info(f'GPT answered with with {len(content.split(" "))} words')
-    logger.info(client.usage)
+    logger.debug(client.usage)
     return content
 
 
 def calculate_tokens_of_text(text: str, model='gpt-3.5-turbo') -> int:
     enc = tiktoken.encoding_for_model(model)
     encoded = enc.encode(text)
     return len(encoded)
@@ -66,37 +71,38 @@
 
     used_tokens = tokens_intro
     prompt = intro
 
     number_of_inputs = len(inputs)
     cards = []
     with Progress() as progress:
-        task = progress.add_task('Promting GPT...', total=number_of_inputs)
+        task = progress.add_task('Prompting GPT...', total=number_of_inputs)
         for index, item in enumerate(inputs):
             item = f'{item}\n'
             input_tokens = calculate_tokens_of_text(item)
 
             # Add some space for the gpt answer
-            needed_tokens = int(input_tokens + (input_tokens / 4))
+            needed_tokens = int(input_tokens + (input_tokens / 2))
 
             # Check if adding more tokens will exceed the limit or it is the last item
             if (used_tokens + needed_tokens >= token_limit) or (
                 index + 1 == number_of_inputs
             ):
                 logger.info(f'Token limit of {token_limit} reached for current prompt')
 
                 # Get response from GPT
                 try:
                     gpt_answer = prompt_openai(openai_token, prompt)
-
-                    try:
-                        cards.extend(gpt_answer_to_cards(gpt_answer, cards_source))
-                    except Exception as e:
-                        logger.error(e)
-                        logger.error(gpt_answer)
+                    splitted_answer = split_gpt_answer(str(gpt_answer))
+                    for item in splitted_answer:
+                        try:
+                            cards.append(gpt_answer_to_cards(item, cards_source))
+                        except Exception as e:
+                            logger.error(item)
+                            logger.error(e)
                 except Exception as e:
                     logger.error(e)
 
                 # Reset the prompt and used tokens
                 prompt = intro + item
                 used_tokens = tokens_intro
             else:
```

## ankigengpt/templates/introduction.j2

```diff
@@ -3,13 +3,13 @@
 If you are not able to create cards, just answer with nothing.
 
 Regarding the formulation of the card content, you stick to two principles:
 First, minimum information principle: The material you learn must be formulated in as simple way as it is only possible. Simplicity does not have to imply losing information and skipping the difficult part.
 Second, optimize wording: The wording of your items must be optimized to make sure that in minimum time the right bulb in your brain lights up. This will reduce error rates, increase specificity, reduce response time, and help your concentration.
 
 Your answer must be in the YAML Format with quoted strings like the following.
-Quotes in the answer or question itself must be escaped.
+Single Quotes and double quotes in the answer or question must be escaped.
 
 - question: "Where is the Dead Sea located?"
   answer: "on the border between Israel and Jordan"
 - question: "What is the lowest point on the Earth's surface?"
   answer: "The Dead Sea shoreline"
```

## Comparing `ankigengpt-0.1.0.dist-info/METADATA` & `ankigengpt-1.1.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ankigengpt
-Version: 0.1.0
+Version: 1.1.6
 Summary: 
 Author: rwxd
 Author-email: git@rwxd.de
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,14 +12,15 @@
 Requires-Dist: ebooklib (>=0.18,<0.19)
 Requires-Dist: genanki (>=0.13.0,<0.14.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: pdfplumber (>=0.9.0,<0.10.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: ratelimit (>=2.2.1,<3.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # AnkiGenGPT
```

## Comparing `ankigengpt-0.1.0.dist-info/RECORD` & `ankigengpt-1.1.6.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ankigengpt/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ankigengpt/__main__.py,sha256=sVYN-XX0UDXAEBowd3LILGFfXqQIjjvbFIIo9OPIstQ,133
-ankigengpt/anki.py,sha256=FjyIIPXyWnQdnGgODpXKIa7NMTIAhnfgjXKhVJk8dqg,1247
-ankigengpt/cli.py,sha256=AiNRuvwpslbMg_wcmx4tN-k9Ew_h9EaWUKjtjDF5q-Y,2486
+ankigengpt/anki.py,sha256=0WYIFRRr2Vd1pNCPpCDkh_Ly_I_gFCDY0tYue9X4DC8,1904
+ankigengpt/cli.py,sha256=nXgRFxXgQKoCka8xJOId6I4D_piWCuYaKZpa5D3iedM,2605
 ankigengpt/epub.py,sha256=xv3CzGTwKH-zTEcVSXc4lcpPzigw4ma4XqaQ9NVrHNE,837
-ankigengpt/gpt.py,sha256=Fz9GeUAgtyOEK4YqKnGCJ8St4IKCXq6AxQ1Dqa8g6IE,3751
+ankigengpt/gpt.py,sha256=BL9VJ0E9sI-kCedhA_EO3y3xQIjekNxsUnjVtL54d2E,4009
 ankigengpt/kindle.py,sha256=ENFI5mohXni0GYIPkgvm-uy0myXoxiCN53OCCmIKRW0,753
 ankigengpt/logging.py,sha256=vuzbOTlGJfmw0FeLzekkhdXBVQK2raQejOtEmX3efnU,664
 ankigengpt/misc.py,sha256=iMvHIex41APvh1qm-fvcdmXMemMs7MxVWUWd7YjUkBY,103
 ankigengpt/templates/__init__.py,sha256=vMyumStijq4bWLP158od8i3jGAW2sGQvXQfxzkEhoPk,473
 ankigengpt/templates/epub.j2,sha256=08bQYIQLJBFm9cGut2swMJBn-c_RqGo6DgDC7GVDIXI,66
-ankigengpt/templates/introduction.j2,sha256=aXQO5BHxDQFsJ88ydfWsTGAF88LNBtP9toRohEyvmKY,1156
+ankigengpt/templates/introduction.j2,sha256=bgUDHt1KiwN8MHwDvZk7woCjnUtiTmZkkUAT_8TPVA4,1174
 ankigengpt/templates/kindle.j2,sha256=TyrTQUapEOEE78gSkkxjEma3U8aF_AC4tIkPxbpzrc0,32
 ankigengpt/templates/plain.j2,sha256=TyrTQUapEOEE78gSkkxjEma3U8aF_AC4tIkPxbpzrc0,32
-ankigengpt-0.1.0.dist-info/METADATA,sha256=glm1LklXoVHCphcmfVoZ7uJ8BckVBSKt0XLDwxzg5RY,1642
-ankigengpt-0.1.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-ankigengpt-0.1.0.dist-info/entry_points.txt,sha256=oUfAyWgpkI4rT6NQO7_qU7wDj2whvpunNSs_JzZpT6g,55
-ankigengpt-0.1.0.dist-info/RECORD,,
+ankigengpt-1.1.6.dist-info/METADATA,sha256=Y_r0x82WTbWX7CIc1ki9BqPtRKwIWl_maZS3v5Z9gF8,1684
+ankigengpt-1.1.6.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+ankigengpt-1.1.6.dist-info/entry_points.txt,sha256=oUfAyWgpkI4rT6NQO7_qU7wDj2whvpunNSs_JzZpT6g,55
+ankigengpt-1.1.6.dist-info/RECORD,,
```

