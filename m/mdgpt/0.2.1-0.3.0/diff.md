# Comparing `tmp/mdgpt-0.2.1.tar.gz` & `tmp/mdgpt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdgpt-0.2.1.tar", max compression
+gzip compressed data, was "mdgpt-0.3.0.tar", max compression
```

## Comparing `mdgpt-0.2.1.tar` & `mdgpt-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-07-18 20:46:07.614765 mdgpt-0.2.1/LICENSE
--rw-r--r--   0        0        0     5552 2023-07-24 21:22:25.841195 mdgpt-0.2.1/README.md
--rw-r--r--   0        0        0     7685 2023-07-26 19:28:45.661699 mdgpt-0.2.1/mdgpt/__init__.py
--rw-r--r--   0        0        0     4229 2023-07-26 12:21:16.040964 mdgpt-0.2.1/mdgpt/build.py
--rw-r--r--   0        0        0      448 2023-07-24 21:53:42.866848 mdgpt-0.2.1/mdgpt/misc.py
--rw-r--r--   0        0        0     2027 2023-07-26 19:33:53.466171 mdgpt-0.2.1/mdgpt/models.py
--rw-r--r--   0        0        0     9952 2023-07-26 19:34:15.975350 mdgpt-0.2.1/mdgpt/translate.py
--rw-r--r--   0        0        0     4964 2023-07-26 19:36:05.278406 mdgpt-0.2.1/mdgpt/utils.py
--rw-r--r--   0        0        0      895 2023-07-26 19:53:57.285323 mdgpt-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6757 2023-07-26 19:55:17.052047 mdgpt-0.2.1/setup.py
--rw-r--r--   0        0        0     6443 2023-07-26 19:55:17.052469 mdgpt-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-18 20:46:07.614765 mdgpt-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5552 2023-07-27 21:10:00.673003 mdgpt-0.3.0/README.md
+-rw-r--r--   0        0        0     7746 2023-07-29 21:09:50.848726 mdgpt-0.3.0/mdgpt/__init__.py
+-rw-r--r--   0        0        0     4322 2023-07-29 21:00:05.927261 mdgpt-0.3.0/mdgpt/build.py
+-rw-r--r--   0        0        0     1301 2023-07-29 20:35:09.844197 mdgpt-0.3.0/mdgpt/image.py
+-rw-r--r--   0        0        0      448 2023-07-24 21:53:42.866848 mdgpt-0.3.0/mdgpt/misc.py
+-rw-r--r--   0        0        0     2715 2023-07-29 20:36:43.111687 mdgpt-0.3.0/mdgpt/models.py
+-rw-r--r--   0        0        0    11060 2023-07-29 20:45:20.754845 mdgpt-0.3.0/mdgpt/translate.py
+-rw-r--r--   0        0        0     5726 2023-07-29 14:25:42.495475 mdgpt-0.3.0/mdgpt/utils.py
+-rw-r--r--   0        0        0      940 2023-07-29 20:58:09.903291 mdgpt-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6817 2023-07-29 21:12:23.429977 mdgpt-0.3.0/setup.py
+-rw-r--r--   0        0        0     6531 2023-07-29 21:12:23.430647 mdgpt-0.3.0/PKG-INFO
```

### Comparing `mdgpt-0.2.1/LICENSE` & `mdgpt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mdgpt-0.2.1/README.md` & `mdgpt-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mdgpt-0.2.1/mdgpt/__init__.py` & `mdgpt-0.3.0/mdgpt/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,56 @@
 import argparse
+import frontmatter
 
 from dotenv import load_dotenv
 from pathlib import Path
 
 from rich import print
 from rich.progress import track
 
 from mdgpt.utils import log_usage
 from mdgpt.models import PromptConfig
-from mdgpt.models import get_prompt_config_from_yaml
+from mdgpt.models import get_prompt_config
 from mdgpt.build import get_build_tasks
 from mdgpt.build import build_step
-from mdgpt.translate import get_translation_tasks
 from mdgpt.utils import get_json_to_translate
-from mdgpt.translate import save_json_translated
 from mdgpt.utils import get_url_map
-from mdgpt.translate import translate_missing_json
 from mdgpt.utils import get_lang_dict
+from mdgpt.utils import get_markdown_files
+from mdgpt.translate import save_json_translated
+from mdgpt.translate import translate_missing_json
+from mdgpt.translate import get_translation_tasks
 from mdgpt.translate import translate_markdown_file
 from mdgpt.translate import get_target_file
 
 
 load_dotenv()
 
 
 def cli():
 
     args = parse_args()
-    cfg = get_prompt_config_from_yaml(args.prompt, **vars(args))
+    cfg = get_prompt_config(args.prompt, **vars(args))
 
     source_lang = get_lang_dict(cfg.LANGUAGE)
     source_lang['dir'] = cfg.SOURCE_DIR if cfg.SOURCE_DIR else cfg.LANGUAGE
 
     if args.action == 'build':
         _build(cfg, source_lang)
 
     elif args.action == 'translate':
         _translate(cfg, source_lang)
 
+    elif args.action == 'image':
+        from mdgpt.image import create_image
+        create_image(cfg)
+
+    elif args.action == 'debug':
+        _debug(cfg)
+
     else:
         print('Unknown action')
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description='Build and translate markdown files from a prompt configuration file')
     parser.add_argument('action', type=str, help='Action to perform')
@@ -66,30 +75,30 @@
         print('[red]No website builder config found.')
         exit(1)
 
     tasks = get_build_tasks(wcfg)
     total_tasks = len(tasks)
     print('Tasks:', len(tasks))
 
-    for i in track(range(len(tasks)), description="Building ..."):
+    for i in track(range(total_tasks), description="Building ..."):
         step = tasks[i]
 
         print_details = f'({i+1}/{total_tasks}) Writing {step.destination} ...'
         print(print_details, end='', flush=True)
 
-        usage, err = build_step(cfg, source_lang, step)
+        usage, err = build_step(cfg, step)
         if err:
-            print(f'[red]({print_details} ERROR:', err)
+            print(f'[red]{print_details} ERROR:', err)
             errors += 1
         else:
             if usage:
-                print(f'[green]({print_details} ok ;)')
+                print(f'[green]{print_details} ok ;)')
                 oks += 1
             else:
-                print(f'[yellow]({print_details} Skipped!')
+                print(f'[yellow]{print_details} Skipped!')
                 skips += 1
 
         if usage:
             prompt_tokens += usage['prompt_tokens']
             completion_tokens += usage['completion_tokens']
             log_usage('write_md', cfg.LANGUAGE, step.destination, usage['prompt_tokens'], usage['completion_tokens'])
 
@@ -115,99 +124,100 @@
         url_map, missing = get_json_to_translate(cfg, url_hashes, target)
 
         url_matrix[target] = url_map
         missing_matrix[target] = missing
         lang_matrix[target] = get_lang_dict(target)
 
     # Execute translation tasks
-    for i in track(range(len(tasks)), description="Translating ..."):
-        task = tasks[i]
-        action, target, file = task.split(':')[:3]
-
-        if action == 'js':
+    try:
+        for i in track(range(total_tasks), description="Translating ..."):
+            task = tasks[i]
+            action, target, file = task.split(':')[:3]
 
-            url_map = url_matrix[target]
-            missing = missing_matrix[target]
-            target_lang = lang_matrix[target]
+            if action == 'js':
 
-            print_details = f'({i+1}/{total_tasks}) Translating file urls -> {target} ...'
-            print(print_details, end='', flush=True)   # end='\r',
-
-            if len(missing) == 0:
-                print(f'[yellow]{print_details} Skip!')
-                skips += 1
+                url_map = url_matrix[target]
+                missing = missing_matrix[target]
+                target_lang = lang_matrix[target]
 
-            if len(missing) > 0:
-                missing_translations = translate_missing_json(cfg, missing, source_lang, target_lang)
+                print_details = f'{i+1}/{total_tasks} Translating file urls {cfg.LANGUAGE} -> {target} ...'
+                print(print_details, end='', flush=True)   # end='\r',
 
-                # Backfill missing translations
-                for key, value in missing_translations.items():
-                    if value is not None and len(value) > 0:
-                        url_map[key] = value
-
-                # Save url_map ...
-                save_json_translated(cfg, url_map, target)
-                print(f'[green]{print_details} ok ;)')
-                oks += 1
-
-        elif action == 'md':
-
-            # Check if file exists
-            root = Path(cfg.ROOT_DIR)
-            target_path = get_target_file(file, root, target, url_matrix[target])
-
-            print_details = f'({i+1}/{total_tasks}) Translating {file} -> {target_path} ...'
-
-            print(print_details, end='', flush=True)   # end='\r',
-            if target_path.exists():
-                skip = True
-                if cfg.FILE:
-                    if cfg.FILE == file:
-                        skip = False
-
-                if skip:
-                    skips += 1
+                if len(missing) == 0:
                     print(f'[yellow]{print_details} Skip!')
-                    # time.sleep(0.1)
-                    continue
-
-            # if usage := translate_markdown_file(file, prompt_cfg.ROOT_DIR, source_lang, target_lang, url_map, prompt_cfg.MARKDOWN_PROMPT, prompt_cfg.FIELD_KEYS, prompt_cfg.MODEL):
-            if usage := translate_markdown_file(cfg, file, source_lang, target_lang, url_matrix[target]):
-                prompt_tokens += usage['prompt_tokens']
-                completion_tokens += usage['completion_tokens']
-                log_usage('translate_md', target, file, usage['prompt_tokens'], usage['completion_tokens'])
-
-                oks += 1
+                    skips += 1
 
-                print(f'[green]{print_details} ok!')
-                # print('ok')
+                if len(missing) > 0:
+                    missing_translations = translate_missing_json(cfg, missing, source_lang, target_lang)
 
-            else:
-                errors += 1
-                print(f'[red]{print_details} error!')
-                # print(f'Error...', end='\n')  # end='\r'
-
-        # time.sleep(0.1)  # Simulate work being done
-
-    # with Progress() as progress:
-    #     task = progress.add_task("twiddling thumbs", total=len(tasks))
-    #     for job in range(len(tasks)):
-    #         progress.console.print(f"Working on job #{job}")
-    #         # run_job(job)
-    #         time.sleep(0.1)
-    #         progress.advance(task)
-
-    # text_column = TextColumn("{task.description}", table_column=Column(ratio=1))
-    # bar_column = BarColumn(bar_width=None, table_column=Column(ratio=2))
-    # progress = Progress(text_column, bar_column, expand=True)
-
-    # with progress:
-    #     for n in progress.track(range(100)):
-    #         progress.print(n)
-    #         time.sleep(0.08)
+                    # Backfill missing translations
+                    for key, value in missing_translations.items():
+                        if value is not None and len(value) > 0:
+                            url_map[key] = value
+
+                    # Save url_map ...
+                    save_json_translated(cfg, url_map, target)
+                    print(f'[green]{print_details} ok ;)')
+                    oks += 1
+
+            elif action == 'md':
+
+                # Check if file exists
+                root = Path(cfg.ROOT_DIR)
+                target_path = get_target_file(file, root, target, url_matrix[target])
+
+                print_details = f'{i+1}/{total_tasks} Translating {target_path} ...'
+
+                print(print_details, end='', flush=True)   # end='\r',
+                if target_path.exists():
+                    skip = True
+                    if cfg.FILE:
+                        if cfg.FILE == file:
+                            skip = False
+
+                    if skip:
+                        skips += 1
+                        print(f'[yellow]{print_details} Skip!')
+                        continue
+
+                if usage := translate_markdown_file(cfg, file, source_lang, target_lang, url_matrix[target]):
+                    prompt_tokens += usage['prompt_tokens']
+                    completion_tokens += usage['completion_tokens']
+                    log_usage('translate_md', target, file, usage['prompt_tokens'], usage['completion_tokens'])
+
+                    oks += 1
+
+                    print(f'[green]{print_details} ok!')
+
+                else:
+                    errors += 1
+                    print(f'[red]{print_details} error!')
+    except KeyboardInterrupt:
+        print('Interrupted!')
+    except Exception as e:
+        print('An error occurred:', e)
 
+    print('---')
     print('prompt_tokens:', prompt_tokens)
     print('completion_tokens:', completion_tokens)
-
+    print('---')
+    print(f'[bold]Tasks: {total_tasks}')
     print(f'[yellow]skips: {skips}')
     print(f'[green]oks: {oks}')
     print(f'[red]errors: {errors}')
+
+
+def _debug(cfg: PromptConfig):
+    print(f'cfg:', cfg)
+
+    unique_matters = []
+    matters = []
+    root_path = Path(cfg.ROOT_DIR, cfg.SOURCE_DIR or cfg.LANGUAGE)
+    files = get_markdown_files(root_path)
+    for file in files:
+        content = Path(root_path, file).read_text()
+        matter = frontmatter.loads(content)
+        for k, v in matter.metadata.items():
+            if k not in unique_matters:
+                unique_matters.append(k)
+
+    print('unique_matters:', sorted(unique_matters))
```

### Comparing `mdgpt-0.2.1/mdgpt/build.py` & `mdgpt-0.3.0/mdgpt/build.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,71 +8,75 @@
 from mdgpt.models import WebsiteBuilder
 
 from mdgpt.utils import (
     load_prompt,
     get_chat_response,
     get_gpt_options,
     get_language_name,
+    DefaultDictFormatter,
 )
 
 
-def build_step(prompt_cfg: PromptConfig, source_lang, step):
-
-    target_path = Path(prompt_cfg.ROOT_DIR, source_lang['dir'], step.destination)
+def build_step(prompt_cfg: PromptConfig, step):
+    target_path = Path(prompt_cfg.ROOT_DIR, prompt_cfg.LANG.directory, step.destination)
     if target_path.exists():
         skip = True
         if prompt_cfg.FILE:
             if prompt_cfg.FILE == step.destination:
                 skip = False
 
         if skip:
             return False, None
 
     wcfg = prompt_cfg.WEBSITE_BUILDER
 
-    title = wcfg.title
-    description = wcfg.description
+    # title = wcfg.title
+    # description = wcfg.description
 
     user_suffix = wcfg.user_suffix.strip()
     system_prompt = wcfg.system_prompt.strip()
 
+    step_prompt = '\n'.join([
+        step.prompt.strip(),
+        user_suffix,
+    ])
+
+    variables = wcfg.variables
+
+    variables['lang_name'] = prompt_cfg.LANG.name
+    variables['lang_code'] = prompt_cfg.LANG.code
+
     messages = [
         {
             'role': 'system',
-            'content': system_prompt.format(lang=source_lang, title=title, description=description)
+            # 'content': system_prompt.format(lang=source_lang, **variables)
+            'content': system_prompt.format_map(DefaultDictFormatter(variables)).strip()
         },
         {
             'role': 'user',
-            'content': '\n'.join([
-                step.prompt.format(lang=source_lang, title=title).strip(),
-                user_suffix
-            ])
+            'content': step_prompt.format_map(DefaultDictFormatter(variables))
         }
     ]
 
     options = get_gpt_options(prompt_cfg.MODEL)
 
     try:
         response, usage = get_chat_response(messages, **options)
 
     except Exception as e:
-        # raise Exception(f'Could not get response: {e}')
-        # print(f'Could not get response: {e}')
         return None, e
 
     try:
         new_matter, new_content = frontmatter.parse(response)
     except Exception as e:
         # raise Exception(f'Could not parse: {e}. response: {response}')
         # print(f'Could not parse: {e}. response: {response}')
         return usage, e
 
-    post = frontmatter.Post('')
-    post.content = new_content
-    post.metadata = new_matter
+    post = frontmatter.Post(new_content, **new_matter)
 
     target_path.parent.mkdir(parents=True, exist_ok=True)
     target_path.write_text(frontmatter.dumps(post))
 
     return usage, None
 
 
@@ -145,7 +149,9 @@
         print('No website builder config found.')
         exit(1)
 
     steps = website_builder_cfg.steps
     return steps
     # for i, step in enumerate(steps):
     #     ...
+
+
```

### Comparing `mdgpt-0.2.1/mdgpt/models.py` & `mdgpt-0.3.0/mdgpt/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,23 @@
+import yaml
+import pycountry
+
 from pydantic_core.core_schema import FieldValidationInfo
 from pydantic import BaseModel, ValidationError, field_validator
 from typing import List, Optional
-import yaml
 
 from pathlib import Path
 
 
+class LangModel(BaseModel):
+    code: str
+    name: str
+    directory: str
+
+
 class ChatGPTModel(BaseModel):
     temperature: float=0.2
     engine: str='gpt-3.5-turbo'
     max_tokens: int=1024*2
 
 
 class ChatGPTPrompt(BaseModel):
@@ -25,37 +33,55 @@
 
 class WebsiteBuilder(BaseModel):
     title: str=''
     description: str=''
     user_suffix: str=''
     system_prompt: str=''
     steps: List[ChatGPTStepPrompt]
+    variables: dict={}
 
 
 class PromptConfig(BaseModel):
     LANGUAGE: str=None
     ROOT_DIR: str=None
     SOURCE_DIR: str=None
     TARGET_LANGUAGES: List[str]=[]
     MODEL: ChatGPTModel=None
     WEBSITE_BUILDER: WebsiteBuilder=None
     URL_PROMPT: List[ChatGPTPrompt]
     MARKDOWN_PROMPT: List[ChatGPTPrompt]
     ONLY_INDEXES: bool=False
     FILE: str=None
     FIELD_KEYS: List[str]=None
+    FIELD_KEYS_DELETE: List[str]=None
+    LANG: LangModel=None
 
     @field_validator('LANGUAGE')
     def language_must_be_iso(cls, v):
         if len(v) != 2:
             raise ValueError('LANGUAGE must be an ISO 639-1 two-letter language code')
         return v
 
 
-def get_prompt_config_from_yaml(prompt_file: str, **kwargs) -> PromptConfig:
+def get_prompt_config(prompt_file: str, **kwargs) -> PromptConfig:
+
+    def get_language_name(lang_code):
+        lang = None
+        try:
+            lang = pycountry.languages.get(alpha_2=lang_code)
+        except Exception as e:
+            print(f'An error occurred: {e}')
+            exit(1)
+
+        if lang is None:
+            print(f'Language {lang_code} not found.', lang)
+            exit(1)
+
+        return lang.name
+
     try:
         with open(f'{prompt_file}.yaml', 'r') as f:
             prompt = yaml.load(f, Loader=yaml.loader.SafeLoader)
 
     except FileNotFoundError:
         print(f'Prompt file {prompt_file} not found.')
         exit(1)
@@ -78,8 +104,13 @@
     try:
         cfg = PromptConfig(**prompt)
 
     except ValidationError as e:
         print(e)
         exit(1)
 
+    cfg.LANG = LangModel(
+        code=cfg.LANGUAGE,
+        name=get_language_name(cfg.LANGUAGE),
+        directory=cfg.SOURCE_DIR or cfg.LANGUAGE
+    )
     return cfg
```

### Comparing `mdgpt-0.2.1/mdgpt/translate.py` & `mdgpt-0.3.0/mdgpt/translate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import argparse
-import glob
 import json
 import frontmatter
 import yaml
 
 from pathlib import Path
 from rich import print
 
@@ -12,42 +10,49 @@
 from mdgpt.utils import get_url_map
 from mdgpt.utils import (
     urlize,
     log_usage,
     load_prompt,
     get_chat_response,
     get_gpt_options,
-    get_language_name
+    get_language_name,
+    get_markdown_files,
 )
 
 
 def get_translation_tasks(prompt_cfg: PromptConfig):
-    source_lang = get_lang_dict(prompt_cfg.LANGUAGE)
-    source_lang['dir'] = prompt_cfg.SOURCE_DIR if prompt_cfg.SOURCE_DIR else prompt_cfg.LANGUAGE
-
     tasks = []
     for target in prompt_cfg.TARGET_LANGUAGES:
-        # target_lang = get_lang_dict(target)
-
         url_hash = get_url_map(prompt_cfg)
-
         tasks.append(f'js:{target}:{prompt_cfg.LANGUAGE}_{target}')
 
         if prompt_cfg.FILE:
             tasks.append(f'md:{target}:{prompt_cfg.FILE}' )
+            continue
         else:
             for k, v in url_hash.items():
                 if not k.endswith('.md'):
                     if len(k) > 0:
                         k = f'{k}/index.md'
                     else:
                         k = f'{k}index.md'
                 tasks.append(f'md:{target}:{k}')
             # tasks.extend([f'md:{target}:{k}' for k, v in url_hash.items()])
 
+        files = get_markdown_files(Path(prompt_cfg.ROOT_DIR, prompt_cfg.SOURCE_DIR or prompt_cfg.LANGUAGE))
+        for f in files:
+            if f.endswith('README.md'):
+                continue
+
+            if f.endswith('index.md'):
+                f = f.rstrip('index.md').rstrip('/')
+
+            if url_hash.get(f) is None:
+                tasks.append(f'md:{target}:{f}')
+
     return tasks
 
 
 def translate(prompt_cfg: PromptConfig):
     source_lang = {
         'code': prompt_cfg.LANGUAGE,
         'name': get_language_name(prompt_cfg.LANGUAGE),
@@ -100,36 +105,47 @@
 
         print('')
         print('counter', counter)
         print('prompt_tokens', prompt_tokens)
         print('completion_tokens', completion_tokens)
 
 
-def generate_frontmatter(post, field_keys):
+def generate_frontmatter(post, field_keys, field_keys_delete=None):
     field_dict = {}
     if field_keys is not None and len(field_keys) > 0:
         for field in field_keys:
             if field in post.keys():
                 if post[field] is not None:
                     field_value = post[field]
                     field_dict[field] = field_value
     else:
         field_dict = post.metadata
+
+    if field_keys_delete is not None and len(field_keys_delete) > 0:
+        for field in field_keys_delete:
+            if field in field_dict.keys():
+                del field_dict[field]
+
     frontmatter = yaml.dump(field_dict)
     return frontmatter
 
 
-def generate_md_promt(prompt_messages, post, lang, target_lang, field_keys):
-    frontmatter = generate_frontmatter(post, field_keys)
+def generate_md_promt(prompt_messages, post, lang, target_lang, field_keys, field_keys_delete=None):
+    frontmatter = generate_frontmatter(post, field_keys, field_keys_delete)
+
     return [
         {
             'role': msg.role,
             'content': msg.prompt.format(
                 lang=lang,
+                lang_name=lang['name'],
+                lang_code=lang['code'],
                 target_lang=target_lang,
+                target_lang_name=target_lang['name'],
+                target_lang_code=target_lang['code'],
                 frontmatter=frontmatter,
                 content=post.content
             )
         } for msg in prompt_messages
     ]
 
 
@@ -177,27 +193,25 @@
         if target_file.exists():
             continue
 
         filtered_files.append(file)
     return filtered_files
 
 
-
-
 def translate_markdown_file(prompt_cfg: PromptConfig, file, src, target, url_map, ignore_existing=True):
     root = Path(prompt_cfg.ROOT_DIR)
 
     src_code, src_name, src_dir = src['code'], src['name'], src['dir']
     trg_code, trg_name, trg_dir = target['code'], target['name'], target['dir']
 
     with open(root / src_dir / file) as f:
         post = frontmatter.load(f)
 
     target_path = get_target_file(file, root, trg_dir, url_map)
-    messages = generate_md_promt(prompt_cfg.MARKDOWN_PROMPT, post, src, target, prompt_cfg.FIELD_KEYS)
+    messages = generate_md_promt(prompt_cfg.MARKDOWN_PROMPT, post, src, target, prompt_cfg.FIELD_KEYS, prompt_cfg.FIELD_KEYS_DELETE)
     options = get_gpt_options(prompt_cfg.MODEL)
 
     try:
         response, usage = get_chat_response(messages, **options)
     except Exception as e:
         # raise Exception(f'Could not get response for {file}: {e}')
         print(f'Could not get response for {file}: {e}')
@@ -209,14 +223,19 @@
     except Exception as e:
         # raise Exception(f'Could not parse {file}: {e}. response: {response}')
         print(f'Could not parse {file}: {e}. response: {response}')
         return
 
     post.content = new_content
 
+    if prompt_cfg.FIELD_KEYS_DELETE is not None and len(prompt_cfg.FIELD_KEYS_DELETE) > 0:
+        for field in prompt_cfg.FIELD_KEYS_DELETE:
+            if post.get(field):
+                del post[field]
+
     if prompt_cfg.FIELD_KEYS is not None and len(prompt_cfg.FIELD_KEYS) > 0:
         for field in prompt_cfg.FIELD_KEYS:
             if new_matter.get(field):
                 post[field] = new_matter[field]
     else:
         post.metadata = new_matter
 
@@ -236,15 +255,22 @@
     src_file.write_text(json.dumps(json_dict, indent=2))
 
 
 def translate_missing_json(prompt_cfg: PromptConfig, json_dict, src, target):
     messages = [
         {
             'role': msg.role,
-            'content': msg.prompt.format(lang=src, target_lang=target, content=json.dumps(json_dict, indent=2))
+            'content': msg.prompt.format(
+                lang=src,
+                lang_name=src['name'],
+                lang_code=src['code'],
+                target_lang=target,
+                target_lang_name=target['name'],
+                target_lang_code=target['code'],
+                content=json.dumps(json_dict, indent=2))
         }
         for msg in prompt_cfg.URL_PROMPT
     ]
     options = get_gpt_options(prompt_cfg.MODEL)
     response, usage = get_chat_response(messages, **options)
     log_usage('translate_json', target['code'], f'{src["code"]}_{target["code"]}', usage['prompt_tokens'], usage['completion_tokens'])
```

### Comparing `mdgpt-0.2.1/mdgpt/utils.py` & `mdgpt-0.3.0/mdgpt/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -55,23 +55,26 @@
         message = completions.choices[0].message.content
         usage = completions.usage.to_dict()
 
         return message, usage
 
     except openai.error.AuthenticationError as e:
         print(f'OpenAI AuthenticationError: {e}')
-        exit(1)
+        # exit(1)
+        raise e
 
     except openai.error.OpenAIError as e:
         print(f'OpenAI Error: {e}')
-        exit(1)
+        # exit(1)
+        raise e
 
     except Exception as e:
         print(f'An error occurred: {e}')
-        exit(1)
+        # exit(1)
+        raise e
 
 
 def get_gpt_options(gpt_model):
     options = {}
 
     if gpt_model is None:
         return options
@@ -171,10 +174,36 @@
     }
 
 
 def get_markdown_files(path: Path):
     files = []
     for filepath in glob.iglob(f'{path}/**/*.md', recursive=True):
         relative_path = filepath[len(f'{path}'):]
+        if relative_path.endswith('README.md'):
+            continue
         files.append(relative_path.lstrip('/'))
     files.sort()
     return files
+
+
+class DefaultDictFormatter(dict):
+    def __missing__(self, key):
+        return MissingAttrHandler('{{{}'.format(key))
+
+
+class MissingAttrHandler(str):
+    def __init__(self, format):
+        self.format = format
+
+    def __getattr__(self, attr):
+        return type(self)('{}.{}'.format(self.format, attr))
+
+    def __repr__(self):
+        return MissingAttrHandler(self.format + '!r}')
+
+    def __str__(self):
+        return MissingAttrHandler(self.format + '!s}')
+
+    def __format__(self, format):
+        if self.format.endswith('}'):
+            self.format = self.format[:-1]
+        return '{}:{}}}'.format(self.format, format)
```

### Comparing `mdgpt-0.2.1/pyproject.toml` & `mdgpt-0.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   | dist
   | venv
 )/
 '''
 
 [tool.poetry]
 name = "mdgpt"
-version = "0.2.1"
+version = "0.3.0"
 description = "Translate markdown files using OpenAI ChatGPT, and generate localized copies of each file."
 authors = ["Jeppe Bårris <jeppe@barris.dk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Djarnis/mdGPT"
 repository = "https://github.com/Djarnis/mdGPT"
 keywords = ["markdown", "translation", "openai", "chatgpt", "gpt"]
@@ -26,14 +26,16 @@
 python-frontmatter = "^1.0.0"
 requests = "^2.31.0"
 pycountry = "^22.3.5"
 openai = "^0.27.8"
 rich = "^13.4.2"
 python-dotenv = "^1.0.0"
 pydantic = "^2.0.3"
+Pillow = "^10.0.0"
+python-slugify = "^8.0.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mdgpt-0.2.1/setup.py` & `mdgpt-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 packages = \
 ['mdgpt']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['openai>=0.27.8,<0.28.0',
+['Pillow>=10.0.0,<11.0.0',
+ 'openai>=0.27.8,<0.28.0',
  'pycountry>=22.3.5,<23.0.0',
  'pydantic>=2.0.3,<3.0.0',
  'python-dotenv>=1.0.0,<2.0.0',
  'python-frontmatter>=1.0.0,<2.0.0',
+ 'python-slugify>=8.0.1,<9.0.0',
  'requests>=2.31.0,<3.0.0',
  'rich>=13.4.2,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['mdgpt = mdgpt:cli']}
 
 setup_kwargs = {
     'name': 'mdgpt',
-    'version': '0.2.1',
+    'version': '0.3.0',
     'description': 'Translate markdown files using OpenAI ChatGPT, and generate localized copies of each file.',
     'long_description': '# mdGPT - Mark Down General Purpose Transformer\n\nTranslate markdown files using OpenAI ChatGPT, and generate localized copies of each file.\n\n## Installation\n\n### Using pip\n\n```bash\npip install mdgpt\n```\n\nSet environment variable `OPENAI_API_KEY` or create it in a `.env` file\n\n```bash\nexport OPENAI_API_KEY=YOUR_API_KEY\n```\n\nDownload example prompts:\n\n```bash\ncurl -o example.yaml https://raw.githubusercontent.com/Djarnis/mdGPT/main/prompts.yaml\n```\n\nUse the example `WEBSITE_BUILDER` option from the prompts to build some example files;\n\n```bash\nmdgpt build example\n```\n\nTranslate these markdown files into Finish (fi) versions:\n\n```bash\nmdgpt translate example --target fi\n```\n\nor Danish (da):\n\n```bash\nmdgpt translate example --target da\n```\n\nor German (de):\n\n```bash\nmdgpt translate example --target de\n```\n\nOr whatever. Just make sure it is an ISO 639-1 two-letter language code, and all should be fine.\n\nAdjust the `example.yaml` prompts to suit your needs.\n\n#### MODEL\n\nYou can change the `MODEL` to any engine supported by OpenAI, change the default temperature, and adjust max tokens.\n\nDefault values are:\n\n```yaml\nMODEL:\n    temperature: 0.2\n    engine: gpt-3.5-turbo\n    max_tokens: 2048\n```\n\n#### WEBSITE_BUILDER\n\nThis option is used for building mark down documents, given the example instructions below:\n\n```yaml\nWEBSITE_BUILDER:\n    title: The AI Markdown Translator\n    description: Translate markdown files for websites\n    system_prompt: |\n        Only reply in valid markdown with frontmatter.\n        No explanations. No notes.\n        Language: {lang[name]}\n        Markdown Document:\n        ---\n        # Frontmatter attributes:\n        title: Title of webpage\n        description: Short meta description\n        ---\n        <!-- markdown content -->\n    user_suffix: |\n        Respond in valid markdown format including all provided frontmatter attributes.\n\n    steps:\n        - prompt: |\n              Write the homepage content for the fictive product "The AI Markdown Translator" in {lang[name]} ({lang[code]}).\n          destination: index.md\n        - prompt: |\n              Write the "About Us" page content for a fictive team behind the fictive product "The AI Markdown Translator" in {lang[name]} ({lang[code]}).\n          destination: about.md\n        - prompt: |\n              Write the history for the fictive product "The AI Markdown Translator" in {lang[name]} ({lang[code]}), starting in 2019 with 5 major milestones.\n          destination: history.md\n```\n\n#### URL_PROMPT\n\nThis prompt is used when translating file paths.\n\n#### MARKDOWN_PROMPT\n\nThis prompt is used when translating markdown files.\n\n#### ONLY_INDEXES\n\nOptional boolean value, if you only want `index.md` files translated.\n\n```yaml\nONLY_INDEXES: True\n```\n\n#### FIELD_KEYS\n\nOptional list of frontmatter keys you want to translate.\n\nPer default, all keys will be translated, but you can define selected ones here.\n\n```yaml\nFIELD_KEYS:\n    - title\n    - description\n    - keywords\n    - heading\n    - teaser\n```\n\n---\n\n### Using repo source and Poetry:\n\n#### Step 1: Install Poetry\n\nPoetry is a tool for dependency management and packaging in Python. It allows you to declare the libraries your project depends on and it will manage (install/update) them for you.\n\nOn Unix-based systems like Linux and MacOS, you can install Poetry by using the following command in your terminal:\n\n```bash\ncurl -sSL https://install.python-poetry.org | python -\n```\n\nOn Windows, you can use PowerShell to install Poetry with the following command:\n\n```powershell\n(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | python -\n```\n\nYou can check if Poetry was installed correctly by running:\n\n```bash\npoetry --version\n```\n\n#### Step 2: Rename .env.tpl to .env\n\nIn your project directory, you have a file named .env.tpl which serves as a template for environment variables. To use this file, you should rename it to .env.\n\nOn Unix-based systems, use the following command:\n\n```bash\nmv .env.tpl .env\n```\n\nOn Windows, use the following command:\n\n```powershell\nrename .env.tpl .env\n```\n\n#### Step 3: Add OPENAI_API_KEY value to .env\n\nOpen your .env file in a text editor. You should see a line that looks something like this:\n\n```bash\nOPENAI_API_KEY=\n```\n\nAfter the equal sign, add your OpenAI API key in quotes. It should look something like this:\n\n```bash\nOPENAI_API_KEY="your-api-key-goes-here"\n```\n\nSave the .env file and close it.\n\n_Please note:_\n\n-   Make sure to replace "your-api-key-goes-here" with your actual OpenAI API key.\n-   Do not share your .env file or post it online, as it contains sensitive information.\n\n#### Step 4: Install mdGPT\n\nFrom the project directory, install mdGPT and its dependencies:\n\n```bash\npoetry install\n```\n\nThis installs mdGPT and all its dependencies, and you can now follow the example below.\n\n## Example\n\n### Build Markdown files\n\nThe example website ([./example/en](example/en)) was created using the `WEBSITE_BUILDER` option included in the [prompts.yaml](prompts.yaml) file.\n\n```bash\npoetry run mdgpt build example\n```\n\nWhich will create these files in the ./example/en directory:\n\n-   index.md\n-   about.md\n-   contact.md\n-   history.md\n\n## Translate website\n\nTo translate the markdown files into Finish (fi) versions, run this command:\n\n```bash\npoetry run mdgot translate example --target fi\n```\n\nAnd you should get a `/fi` subdirectory ./example/fi/ containing these files, translated from their original English (en) source:\n\n-   index.md\n-   tietoja.md\n-   yhteystiedot.md\n-   historia.md\n',
     'author': 'Jeppe Bårris',
     'author_email': 'jeppe@barris.dk',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Djarnis/mdGPT',
```

### Comparing `mdgpt-0.2.1/PKG-INFO` & `mdgpt-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: mdgpt
-Version: 0.2.1
+Version: 0.3.0
 Summary: Translate markdown files using OpenAI ChatGPT, and generate localized copies of each file.
 Home-page: https://github.com/Djarnis/mdGPT
 License: MIT
 Keywords: markdown,translation,openai,chatgpt,gpt
 Author: Jeppe Bårris
 Author-email: jeppe@barris.dk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: Pillow (>=10.0.0,<11.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pycountry (>=22.3.5,<23.0.0)
 Requires-Dist: pydantic (>=2.0.3,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-frontmatter (>=1.0.0,<2.0.0)
+Requires-Dist: python-slugify (>=8.0.1,<9.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Project-URL: Repository, https://github.com/Djarnis/mdGPT
 Description-Content-Type: text/markdown
 
 # mdGPT - Mark Down General Purpose Transformer
```

