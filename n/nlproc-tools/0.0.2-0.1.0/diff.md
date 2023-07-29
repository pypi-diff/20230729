# Comparing `tmp/nlproc_tools-0.0.2.tar.gz` & `tmp/nlproc_tools-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\heine\Documents\research\nlproc.tools\data_tools\dist\.tmp-twkdh_6j\nlproc_tools-0.0.2.tar", last modified: Wed Jul 26 07:19:21 2023, max compression
+gzip compressed data, was "C:\Users\heine\Documents\research\nlproc.tools\data_tools\dist\.tmp-j3kwt9w4\nlproc_tools-0.1.0.tar", last modified: Sat Jul 29 06:31:52 2023, max compression
```

## Comparing `nlproc_tools-0.0.2.tar` & `nlproc_tools-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 07:19:21.488420 nlproc_tools-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-07-23 23:56:05.000000 nlproc_tools-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      770 2023-07-26 07:19:21.489419 nlproc_tools-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-07-24 01:33:17.000000 nlproc_tools-0.0.2/README.md
--rw-rw-rw-   0        0        0      110 2023-07-23 23:55:48.000000 nlproc_tools-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      720 2023-07-26 07:19:21.491418 nlproc_tools-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-26 07:19:21.441112 nlproc_tools-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 07:19:21.457418 nlproc_tools-0.0.2/src/nlproc_tools/
--rw-rw-rw-   0        0        0      108 2023-07-26 06:12:28.000000 nlproc_tools-0.0.2/src/nlproc_tools/__init__.py
--rw-rw-rw-   0        0        0     2469 2023-07-26 05:03:26.000000 nlproc_tools-0.0.2/src/nlproc_tools/convert.py
--rw-rw-rw-   0        0        0     2555 2023-07-26 06:34:44.000000 nlproc_tools-0.0.2/src/nlproc_tools/dataloader.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:19:21.487421 nlproc_tools-0.0.2/src/nlproc_tools/datasets/
--rw-rw-rw-   0        0        0        0 2023-07-24 00:28:54.000000 nlproc_tools-0.0.2/src/nlproc_tools/datasets/__init__.py
--rw-rw-rw-   0        0        0     2160 2023-07-23 23:48:28.000000 nlproc_tools-0.0.2/src/nlproc_tools/datasets/da-san-martino-etal-2019.py
--rw-rw-rw-   0        0        0      895 2023-07-23 23:32:07.000000 nlproc_tools-0.0.2/src/nlproc_tools/datasets/frank.py
--rw-rw-rw-   0        0        0     3910 2023-07-23 23:48:42.000000 nlproc_tools-0.0.2/src/nlproc_tools/datasets/mqm.py
--rw-rw-rw-   0        0        0       33 2023-07-23 23:32:28.000000 nlproc_tools-0.0.2/src/nlproc_tools/datasets/salsa.py
--rw-rw-rw-   0        0        0     2048 2023-07-23 23:48:49.000000 nlproc_tools-0.0.2/src/nlproc_tools/datasets/scarecrow.py
--rw-rw-rw-   0        0        0     1277 2023-07-24 00:39:40.000000 nlproc_tools-0.0.2/src/nlproc_tools/datasets/snac.py
--rw-rw-rw-   0        0        0     2336 2023-07-23 23:47:42.000000 nlproc_tools-0.0.2/src/nlproc_tools/datasets/wu-etal-2023.py
--rw-rw-rw-   0        0        0     1783 2023-07-26 06:09:42.000000 nlproc_tools-0.0.2/src/nlproc_tools/names.py
--rw-rw-rw-   0        0        0      768 2023-07-26 06:29:10.000000 nlproc_tools-0.0.2/src/nlproc_tools/util.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:19:21.474429 nlproc_tools-0.0.2/src/nlproc_tools.egg-info/
--rw-rw-rw-   0        0        0      770 2023-07-26 07:19:21.000000 nlproc_tools-0.0.2/src/nlproc_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      651 2023-07-26 07:19:21.000000 nlproc_tools-0.0.2/src/nlproc_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 07:19:21.000000 nlproc_tools-0.0.2/src/nlproc_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-26 07:19:21.000000 nlproc_tools-0.0.2/src/nlproc_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 06:31:52.095587 nlproc_tools-0.1.0/
+-rw-rw-rw-   0        0        0     1091 2023-07-23 23:56:05.000000 nlproc_tools-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      761 2023-07-29 06:31:52.095587 nlproc_tools-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-26 07:21:27.000000 nlproc_tools-0.1.0/README.md
+-rw-rw-rw-   0        0        0      110 2023-07-23 23:55:48.000000 nlproc_tools-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      737 2023-07-29 06:31:52.103589 nlproc_tools-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-29 06:31:52.035590 nlproc_tools-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-29 06:31:52.054598 nlproc_tools-0.1.0/src/nlproc_tools/
+-rw-rw-rw-   0        0        0       76 2023-07-29 01:51:02.000000 nlproc_tools-0.1.0/src/nlproc_tools/__init__.py
+-rw-rw-rw-   0        0        0     2213 2023-07-29 06:18:57.000000 nlproc_tools-0.1.0/src/nlproc_tools/convert.py
+-rw-rw-rw-   0        0        0     1868 2023-07-29 01:50:58.000000 nlproc_tools-0.1.0/src/nlproc_tools/dataloader.py
+drwxrwxrwx   0        0        0        0 2023-07-29 06:31:52.094592 nlproc_tools-0.1.0/src/nlproc_tools/datasets/
+-rw-rw-rw-   0        0        0        0 2023-07-24 00:28:54.000000 nlproc_tools-0.1.0/src/nlproc_tools/datasets/__init__.py
+-rw-rw-rw-   0        0        0     2332 2023-07-29 06:21:41.000000 nlproc_tools-0.1.0/src/nlproc_tools/datasets/da-san-martino-etal-2019.py
+-rw-rw-rw-   0        0        0      980 2023-07-29 06:05:30.000000 nlproc_tools-0.1.0/src/nlproc_tools/datasets/frank.py
+-rw-rw-rw-   0        0        0     4056 2023-07-29 06:28:43.000000 nlproc_tools-0.1.0/src/nlproc_tools/datasets/mqm.py
+-rw-rw-rw-   0        0        0      168 2023-07-29 05:47:24.000000 nlproc_tools-0.1.0/src/nlproc_tools/datasets/salsa.py
+-rw-rw-rw-   0        0        0     2104 2023-07-29 06:29:02.000000 nlproc_tools-0.1.0/src/nlproc_tools/datasets/scarecrow.py
+-rw-rw-rw-   0        0        0     1270 2023-07-29 06:05:07.000000 nlproc_tools-0.1.0/src/nlproc_tools/datasets/snac.py
+-rw-rw-rw-   0        0        0     2575 2023-07-29 06:14:00.000000 nlproc_tools-0.1.0/src/nlproc_tools/datasets/wu-etal-2023.py
+-rw-rw-rw-   0        0        0    12962 2023-07-29 05:13:25.000000 nlproc_tools-0.1.0/src/nlproc_tools/names.py
+-rw-rw-rw-   0        0        0      935 2023-07-29 01:38:47.000000 nlproc_tools-0.1.0/src/nlproc_tools/util.py
+drwxrwxrwx   0        0        0        0 2023-07-29 06:31:52.078599 nlproc_tools-0.1.0/src/nlproc_tools.egg-info/
+-rw-rw-rw-   0        0        0      761 2023-07-29 06:31:52.000000 nlproc_tools-0.1.0/src/nlproc_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-07-29 06:31:52.000000 nlproc_tools-0.1.0/src/nlproc_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 06:31:52.000000 nlproc_tools-0.1.0/src/nlproc_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-29 06:31:52.000000 nlproc_tools-0.1.0/src/nlproc_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-29 06:31:52.000000 nlproc_tools-0.1.0/src/nlproc_tools.egg-info/top_level.txt
```

### Comparing `nlproc_tools-0.0.2/LICENSE` & `nlproc_tools-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nlproc_tools-0.0.2/PKG-INFO` & `nlproc_tools-0.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nlproc_tools
-Version: 0.0.2
-Summary: A helper package for loading / managing data collection with nlproc.tools
+Version: 0.1.0
+Summary: Load and manage data collection with nlproc.tools
 Home-page: https://github.com/davidheineman/nlproc.tools
 Author: David Heineman
 Author-email: dheineman3@gatech.edu
 Project-URL: Bug Tracker, https://github.com/davidheineman/nlproc.tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## nlproc_tools
+## Data Tools for nlproc.tools
 
 This is a helper library for [**nlproc.tools**](https://nlproc.tools/). Please see the [**main repo**](https://github.com/davidheineman/nlproc.tools) for documentation.
```

### Comparing `nlproc_tools-0.0.2/src/nlproc_tools/convert.py` & `nlproc_tools-0.1.0/src/nlproc_tools/convert.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 from .util import verify_exists
-import csv, json, os, copy, logging, argparse
+import csv, json, os, copy, logging, importlib
 
 utils_path = "datasets"
+folder_based_datasets = ["da-san-martino-etal-2019"]
 
-def convert_dataset(dataset_name: str, data_path: str, output_path: str, reverse: bool=False):
+logging.basicConfig(level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s")
+logger = logging.getLogger(__name__)
+
+
+def convert_dataset(dataset_name: str, data_path: str, reverse: bool=False, output_path: str=None, limit: int=None) -> dict:
+    """
+    Converts to the nlproc.tools dataset format from supported dataset formats.
+    """
     logger.info("=" * 60)
     logger.info(f"Dataset name: {dataset_name}")
     logger.info(f"Data path: {data_path}")
-    logger.info(f"Output path: {output_path}")
     logger.info(f"Reverse flag: {reverse}")
+    logger.info(f"Output path (Optional): {output_path}")
     logger.info("=" * 60)
 
-    verify_exists(data_path)
-
+    if dataset_name not in folder_based_datasets:
+        verify_exists(data_path)
+    
     try:
-        dataset_module = __import__(f"{utils_path}.{dataset_name}", fromlist=[utils_path])
+        dataset_module = importlib.import_module(f"nlproc_tools.{utils_path}.{dataset_name}")
         logger.info("Converting dataset...")
         if reverse:
             # converted_data = dataset_module.convert_data_backward(data_path, output_path)
             logger.error("Reverse conversion is not yet supported.")
         else:
-            converted_data = dataset_module.convert_data_forward(data_path)
+            converted_data = dataset_module.convert_data_forward(data_path, limit=limit)
             logger.info("Done!")
             
+            if output_path is None:
+                return converted_data
+
             output_filename = f'{output_path}/{dataset_name}.json'
             logger.info(f"Saving to {output_filename}...")
             if not os.path.exists(output_path):
                 os.makedirs(output_path)
             with open(output_filename, 'w') as f:
                 json.dump(converted_data, f, indent=4)
+            return None
     except ImportError:
-        error_value = f"Dataset '{dataset_name}' is not supported. Supported datasets are {supported_datasets()}"
+        error_value = f"Dataset '{dataset_name}' is not supported. {supported_datasets()}"
         logger.error(error_value)
         raise ValueError(error_value)
 
-def supported_datasets():
-    return [f[:-3] for f in os.listdir(utils_path) if f.endswith(".py") and f != "__init__.py"]
-
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(description="Script to convert datasets.")
-    parser.add_argument("--reverse", action="store_true", help="Use this flag to convert back to the original format.")
-    parser.add_argument("--dataset", required=True, help="Name of the dataset, see /utils for names. E.g., 'salsa'")
-    parser.add_argument("--data_path", required=True, help="Path to the data. E.g., 'data/salsa_raw.json'")
-    parser.add_argument("--output_path", required=True, help="Path to the output. E.g., 'data/salsa'")
-
-    args = parser.parse_args()
-
-    logging.basicConfig(level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s")
-    logger = logging.getLogger(__name__)
 
-    convert_dataset(args.dataset, args.data_path, args.output_path, args.reverse)
-
-    logger.info("Done!")
+def supported_datasets():
+    if not os.path.exists(utils_path):
+        return "Cannot find datasets!"
+    return "Supported datasets are " + [f[:-3] for f in os.listdir(utils_path) if f.endswith(".py") and f != "__init__.py"]
```

### Comparing `nlproc_tools-0.0.2/src/nlproc_tools/datasets/da-san-martino-etal-2019.py` & `nlproc_tools-0.1.0/src/nlproc_tools/datasets/da-san-martino-etal-2019.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from deepdiff import DeepDiff
+import json, csv, os, copy, random, logging
 
 category_map = {
     'Loaded_Language': 'loaded_language',
     'Name_Calling,Labeling': 'name_calling',
     'Repetition': 'repetition',
     'Exaggeration,Minimisation': 'exaggeration',
     'Doubt': 'doubt',
@@ -16,23 +16,24 @@
     'Whataboutism': 'whataboutism',
     'Reductio_ad_hitlerum': 'reductio_ad_hitlerum',
     'Red_Herring': 'red_herring',
     'Bandwagon': 'bandwagon',
     'Obfuscation,Intentional_Vagueness,Confusion': 'obfuscate',
     'Straw_Men': 'straw_man'
 }
+reverse_category_map = {v: k for k, v in category_map.items()}
 
 def load_propaganda(filename):
     data = []
     with open(filename, 'r', newline='', encoding='utf-8') as tsv_file:
         reader = csv.reader(tsv_file, delimiter="\t")
         data = [r for r in reader]
     return data
 
-def load_article(filename):
+def convert_entry_forward(filename):
     label_filename = f'{filename}.labels.tsv'
     text_filename = f'{filename}.txt'
     annotations = load_propaganda(label_filename)
 
     with open(text_filename, "r", encoding='utf-8') as f:
         article = f.read()
 
@@ -47,20 +48,22 @@
 
     return {
         'source': '',
         'target': article,
         'edits': edits
     }
 
-dirpath = 'da-san-martino-etal-2019/test/'
-article_names = set([dirpath+x.replace('.txt', '').replace('.labels.tsv', '') for x in os.listdir(dirpath) if 'article' in x])
+def convert_data_forward(data_path, limit=None):
+    """
+    Note: dir_path should correspond to a folder containing pairs of .txt and .labels.tsv files.
+    """
+    article_names = set([data_path + x.replace('.txt', '').replace('.labels.tsv', '') for x in os.listdir(data_path) if 'article' in x])
+
+    if limit:
+        article_names = list(article_names)[:limit]
+        random.shuffle(article_names)
+
+    ported_data = []
+    for filename in article_names:
+        ported_data += [convert_entry_forward(filename)]
 
-article_names = list(article_names)[:50]
-random.shuffle(article_names)
-
-ported_data = []
-for name in article_names:
-    article = load_article(name)
-    ported_data += [article]
-
-with open('../public/data/da-san-martino-etal-2019.json', 'w') as f:
-    json.dump(ported_data, f, indent=4)
+    return ported_data
```

### Comparing `nlproc_tools-0.0.2/src/nlproc_tools/datasets/frank.py` & `nlproc_tools-0.1.0/src/nlproc_tools/datasets/frank.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-filename = 'frank/human_annotations_sentence.json'
+import json, os, copy, random, logging
 
-with open(filename, "r", encoding='utf-8') as f:
-    data = json.load(f)
+def convert_data_forward(data_path, limit=None):
+    with open(data_path, "r", encoding='utf-8') as f:
+        data = json.load(f)
+
+    if limit:
+        random.shuffle(data)
+        data = data[:limit]
+
+    ported_data = []
+    for sent in data:
+        errors = [error_list for ann, error_list in sent['summary_sentences_annotations'][0].items()]
+        errors = list(set([i for j in errors for i in j if i != 'NoE']))
+
+        # if limit and len(errors) < 2: continue
+
+        edits = []
+        for i, error in enumerate(errors):
+            edits += [{
+                "category": error,
+                "id": i,
+                "annotation": None
+            }]
+
+        new_sent = {
+            'context': sent['article'],
+            'source': sent['reference'],
+            'target': sent['summary'],
+            'edits': edits
+        }
 
-random.shuffle(data)
+        ported_data += [new_sent]
 
-ported_data = []
-for sent in data:
-    errors = [error_list for ann, error_list in sent['summary_sentences_annotations'][0].items()]
-    errors = list(set([i for j in errors for i in j if i != 'NoE']))
-
-    if len(errors) < 2: continue
-
-    edits = []
-    for i, error in enumerate(errors):
-        edits += [{
-            "category": error,
-            "id": i,
-            "annotation": None
-        }]
-
-    new_sent = {
-        'context': sent['article'],
-        'source': sent['reference'],
-        'target': sent['summary'],
-        'edits': edits
-    }
-
-    ported_data += [new_sent]
-
-ported_data = ported_data[:50]
-
-with open('../public/data/frank.json', 'w') as f:
-    json.dump(ported_data, f, indent=4)
+    return ported_data
```

### Comparing `nlproc_tools-0.0.2/src/nlproc_tools/datasets/mqm.py` & `nlproc_tools-0.1.0/src/nlproc_tools/datasets/mqm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,35 @@
+import json, csv, os, copy, random, logging
 from deepdiff import DeepDiff
 
-filename = 'mqm/mqm_newstest2020_ende.tsv'
-
-def load_mqm(filename):
-    data = []
-    with open(filename, 'r', newline='', encoding='utf-8') as tsvfile:
-        reader = csv.DictReader(tsvfile, delimiter='\t')
-        data = [r for r in reader]
-    return data
-
-data = load_mqm(filename)
-
 severity_map = {
     'Major': 'a lot', 
     'Minor': 'somewhat', 
     'Neutral': 'minor',
     'no-error': None
 }
+reverse_severity_map = {v: k for k, v in severity_map.items()}
 
-systems = set([s['system'] for s in data])
-
-seg_ids = set([s['seg_id'] for s in data])
-seg_ids = set(list(seg_ids)[:20])
-
-raters = set([s['rater'] for s in data])
-
-ported_data = []
-
-def process_sentences(matching_sentences):
+def convert_entry_forward(matching_sentences):
     new_sent = {}
     sources, targets = [s['source'] for s in matching_sentences], [s['target'] for s in matching_sentences]
 
     if len(sources) == 0 or len(targets) == 0:
         return None
 
     assert len(set(sources)) == 1, sources
     source = sources[0]
     target = targets[0].replace('<v>', '').replace('</v>', '')
 
     new_sent.update({
         'metadata': {
             'system': matching_sentences[0]['system'],
             'doc': matching_sentences[0]['doc'],
-            'seg_id': seg_id,
-            'rater': rater,
+            'seg_id': matching_sentences[0]['seg_id'],
+            'rater': matching_sentences[0]['rater'],
         },
         'source': source,
         'target': target,
         'edits': []
     })
 
     # Add Edits
@@ -60,15 +42,14 @@
         start_idx = target.find(start_tag)
         end_idx = target.find(end_tag) - len(start_tag)
 
         if start_idx == -1 or end_idx == -1:
             return None
 
         severity = target_data['severity']
-
         category = target_data['category'].replace('Style/Awkward', 'akward').split('/')
 
         type_ = category[0]
         sub_type = None
         if len(category) > 1:
             sub_type = category[1]
 
@@ -106,33 +87,43 @@
                     exists = True
             if not exists:
                 new_sent['edits'] += [edit_annotation]
         
         j_id += 1
     return new_sent
 
-i = 1
-for system in systems:
-    for seg_id in seg_ids:
-        for rater in raters:
-            matching_sentences = [s for s in data if\
-                s['seg_id'] == seg_id and\
-                s['rater'] == rater and\
-                s['system'] == system\
-            ]
-            
-            new_sent = process_sentences(matching_sentences)
-
-            if new_sent == None: continue
-
-            new_sent.update({
-                'id': i
-            })
 
-            if i > 50: break
+def convert_data_forward(data_path, limit=None):
+    data = []
+    with open(data_path, 'r', newline='', encoding='utf-8') as tsvfile:
+        reader = csv.DictReader(tsvfile, delimiter='\t')
+        data = [r for r in reader]
+
+    systems = set([s['system'] for s in data])
+    seg_ids = set([s['seg_id'] for s in data])
+    raters = set([s['rater'] for s in data])
+
+    if limit: seg_ids = set(list(seg_ids)[:limit])
+
+    ported_data = []
+    for system in systems:
+        for seg_id in seg_ids:
+            for rater in raters:
+                matching_sentences = [s for s in data if\
+                    s['seg_id'] == seg_id and\
+                    s['rater'] == rater and\
+                    s['system'] == system\
+                ]
+                
+                new_sent = convert_entry_forward(matching_sentences)
+
+                if new_sent == None: continue
+
+                new_sent.update({
+                    'id': len(ported_data) + 1
+                })
 
-            ported_data += [new_sent]
+                if limit and len(ported_data) > limit: break
 
-            i += 1
+                ported_data += [new_sent]
 
-with open('../public/data/mqm.json', 'w') as f:
-    json.dump(ported_data, f, indent=4)
+    return ported_data
```

### Comparing `nlproc_tools-0.0.2/src/nlproc_tools/datasets/scarecrow.py` & `nlproc_tools-0.1.0/src/nlproc_tools/datasets/scarecrow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,67 @@
-from deepdiff import DeepDiff
+import json, csv, os, copy, random, logging, ast
 
-filename = 'scarecrow/scarecrow.csv'
+severity_map = {
+    1: 'minor',
+    2: 'somewhat',
+    3: 'a lot'
+}
+reverse_severity_map = {v: k for k, v in severity_map.items()}
 
-def load_scarecrow(filename):
+def convert_data_forward(data_path, limit=None):
     data = []
-    with open(filename, 'r', newline='', encoding='utf-8') as csvfile:
+    with open(data_path, 'r', newline='', encoding='utf-8') as csvfile:
         reader = csv.DictReader(csvfile)
         data = [r for r in reader]
-    return data
 
-data = load_scarecrow(filename)
+    if limit: data = data[:limit]
 
-data = data[:50]
+    ported_data = []
+    for sent in data:
+        new_sent = {}
+
+        new_sent.update({
+            'id': len(ported_data) + 1,
+            'metadata': {
+                'gid': sent['gid'],
+                'model': sent['model'],
+                'p': sent['p'],
+                'temperature': sent['temperature'],
+                'frequency_penalty': sent['frequency_penalty'],
+            },
+            'source': sent['prompt'],
+            'target': sent['generation'],
+            'edits': []
+        })
 
-ported_data = []
+        annotations = ast.literal_eval(sent['responses'])
 
-severity_map = {
-    1: 'minor',
-    2: 'somewhat',
-    3: 'a lot'
-}
-
-i = 1
-for sent in data:
-    new_sent = {}
-
-    new_sent.update({
-        'id': i,
-        'metadata': {
-            'gid': sent['gid'],
-            'model': sent['model'],
-            'p': sent['p'],
-            'temperature': sent['temperature'],
-            'frequency_penalty': sent['frequency_penalty'],
-        },
-        'source': sent['prompt'],
-        'target': sent['generation'],
-        'edits': []
-    })
-
-    annotations = ast.literal_eval(sent['responses'])
-    # SCARECROW collected 10 annotations
-
-    # Add Edits
-    j = 0
-    for edit in annotations[4]:
-        new_edit = {}
-        type_, explanation, severity, start_idx, end_idx, antacedents = edit
-
-        ann_type = type_.lower().replace('-', '_').replace(' ', '_')
-        ann_type_label = f'{ann_type}_type'
-
-        output_idx = [[start_idx, end_idx]]
-
-        if len(antacedents) > 0:
-            for i in range(len(antacedents) // 2):
-                start_idx, end_idx = antacedents[2 * i], antacedents[2 * i + 1]
-                output_idx += [[start_idx, end_idx]]
-
-        new_edit.update({
-            'id': j,
-            'category': ann_type,
-            'output_idx': output_idx,
-        })
+        # Add Edits
+        for edit in annotations[4]:
+            new_edit = {}
+            type_, explanation, severity, start_idx, end_idx, antacedents = edit
+
+            ann_type = type_.lower().replace('-', '_').replace(' ', '_')
+            ann_type_label = f'{ann_type}_type'
+
+            output_idx = [[start_idx, end_idx]]
+
+            if len(antacedents) > 0:
+                for i in range(len(antacedents) // 2):
+                    start_idx, end_idx = antacedents[2 * i], antacedents[2 * i + 1]
+                    output_idx += [[start_idx, end_idx]]
+
+            new_edit.update({
+                'id': len(new_edit) - 1,
+                'category': ann_type,
+                'output_idx': output_idx,
+            })
+
+            new_edit['annotation'] = {
+                'explanation': explanation.replace('_SEP_', ',').replace('_QUOTE_', '"'),
+                ann_type_label: severity_map[severity]
+            }
 
-        new_edit['annotation'] = {
-            'explaination': explanation.replace('_SEP_', ',').replace('_QUOTE_', '"'),
-            ann_type_label: severity_map[severity]
-        }
-
-        new_sent['edits'] += [new_edit]
-        j += 1
-    ported_data += [new_sent]
-    i += 1
+            new_sent['edits'] += [new_edit]
+        ported_data += [new_sent]
 
-with open('../public/data/scarecrow.json', 'w') as f:
-    json.dump(ported_data, f, indent=4)
+    return ported_data
```

### Comparing `nlproc_tools-0.0.2/src/nlproc_tools/datasets/wu-etal-2023.py` & `nlproc_tools-0.1.0/src/nlproc_tools/datasets/wu-etal-2023.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,76 +1,75 @@
-filename = 'wu-etal-2023/dev_feedback.json'
-
-with open(filename, "r", encoding='utf-8') as f:
-    data = json.load(f)
-
-data = data[:50]
+import json, os, copy, random, logging
 
 category_map = {
     'Irrelevant': 'irrelevant',
     'Redundant': 'repetitive',
     'Wrong-Grounding': 'inconsistent',
     'Unverifiable': 'unverifiable',
     'Incoherent': 'incoherent',
-
     'Missing-Answer': 'missing_answer',
     'Missing-Major-Auxiliary': 'missing_major_auxiliary',
     'Missing-Minor-Auxiliary': 'missing_minor_auxiliary',
 }
+reverse_category_map = {v: k for k, v in category_map.items()}
 
-ported_data = []
-for sent in data:
-    if 'feedback' not in sent: continue
-
-    passages = sent['passages']
-    if len(passages) == 0: continue
-
-    context = ""
-    for passage in passages:
-        passage_text = f'\n\n### Passage Title: {passage[0]}'
-        for passage_sent in passage[1:]:
-            passage_text += "\n" + passage_sent.replace(passage[0] + "\n\n", "")
-        context += passage_text
-
-    context += f'\n\n### Question: {sent["question"]}' 
-
-    new_sent = {
-        'context': context,
-        'source': sent['gold'],
-        'target': sent['prediction 1'],
-        'edits': []
-    }
-
-    for i, edit in enumerate(sent['feedback']['errors']):
-        new_edit = {
-            'id': i,
-            'category': 'factual',
-            'annotation': {
-                'factual_error': {
-                    'val': category_map[edit['error type']]
-                },
-                'explaination': edit['explanation'] if edit['explanation'] != '' else None
-            },
-            'output_idx': [[edit['start'], edit['end']]],
+def convert_data_forward(data_path, limit=None):
+    with open(data_path, "r", encoding='utf-8') as f:
+        data = json.load(f)
+
+    if limit: data = data[:limit]
+
+    ported_data = []
+    for sent in data:
+        if 'feedback' not in sent: continue
+
+        passages = sent['passages']
+        if len(passages) == 0: continue
+
+        context = ""
+        for passage in passages:
+            passage_text = f'\n\n### Passage Title: {passage[0]}'
+            for passage_sent in passage[1:]:
+                passage_text += "\n" + passage_sent.replace(passage[0] + "\n\n", "")
+            context += passage_text
+
+        context += f'\n\n### Question: {sent["question"]}' 
+
+        new_sent = {
+            'context': context,
+            'source': sent['gold'],
+            'target': sent['prediction 1'],
+            'edits': []
         }
-        new_sent['edits'] += [new_edit]
 
-    for i, edit in enumerate(sent['feedback']['missing-info']):
-        new_edit = {
-            'id': i + len(sent['feedback']['errors']),
-            'category': 'missing_info',
-            'annotation': {
-                'missing_info_error': {
-                    'val': category_map[edit['error type']]
+        for i, edit in enumerate(sent['feedback']['errors']):
+            new_edit = {
+                'id': i,
+                'category': 'factual',
+                'annotation': {
+                    'factual_error': {
+                        'val': category_map[edit['error type']]
+                    },
+                    'explanation': edit['explanation'] if edit['explanation'] != '' else None
                 },
-                "passage_id": str(edit['passage_id']),
-                "sentence_id": str(edit['sentence_id'])
+                'output_idx': [[edit['start'], edit['end']]],
             }
-        }
-        new_sent['edits'] += [new_edit]
+            new_sent['edits'] += [new_edit]
 
-    # TODO: need to add corrected-prediction
+        for i, edit in enumerate(sent['feedback']['missing-info']):
+            new_edit = {
+                'id': i + len(sent['feedback']['errors']),
+                'category': 'missing_info',
+                'annotation': {
+                    'missing_info_error': {
+                        'val': category_map[edit['error type']]
+                    },
+                    "passage_id": str(edit['passage_id']),
+                    "sentence_id": str(edit['sentence_id'])
+                }
+            }
+            new_sent['edits'] += [new_edit]
 
-    ported_data += [new_sent]
+        # TODO: need to add corrected-prediction
 
-with open('../public/data/wu-etal-2023.json', 'w') as f:
-    json.dump(ported_data, f, indent=4)
+        ported_data += [new_sent]
+    return ported_data
```

### Comparing `nlproc_tools-0.0.2/src/nlproc_tools/util.py` & `nlproc_tools-0.1.0/src/nlproc_tools/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,7 +19,14 @@
 
 
 def get_meta_keys(data: dict) -> List[str]:
     """
     Get all unique metadata keys
     """
     return list(set([_ for _ in [list(s['metadata'].keys()) for s in data if 'metadata' in s.keys()] for _ in _]))
+
+
+def format_class_str(class_str: any) -> str:
+    """
+    Indents any class string for pretty printing
+    """
+    return str(class_str).replace('\n', '\n  ')
```

### Comparing `nlproc_tools-0.0.2/src/nlproc_tools.egg-info/PKG-INFO` & `nlproc_tools-0.1.0/src/nlproc_tools.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nlproc-tools
-Version: 0.0.2
-Summary: A helper package for loading / managing data collection with nlproc.tools
+Version: 0.1.0
+Summary: Load and manage data collection with nlproc.tools
 Home-page: https://github.com/davidheineman/nlproc.tools
 Author: David Heineman
 Author-email: dheineman3@gatech.edu
 Project-URL: Bug Tracker, https://github.com/davidheineman/nlproc.tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## nlproc_tools
+## Data Tools for nlproc.tools
 
 This is a helper library for [**nlproc.tools**](https://nlproc.tools/). Please see the [**main repo**](https://github.com/davidheineman/nlproc.tools) for documentation.
```

### Comparing `nlproc_tools-0.0.2/src/nlproc_tools.egg-info/SOURCES.txt` & `nlproc_tools-0.1.0/src/nlproc_tools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/nlproc_tools/convert.py
 src/nlproc_tools/dataloader.py
 src/nlproc_tools/names.py
 src/nlproc_tools/util.py
 src/nlproc_tools.egg-info/PKG-INFO
 src/nlproc_tools.egg-info/SOURCES.txt
 src/nlproc_tools.egg-info/dependency_links.txt
+src/nlproc_tools.egg-info/requires.txt
 src/nlproc_tools.egg-info/top_level.txt
 src/nlproc_tools/datasets/__init__.py
 src/nlproc_tools/datasets/da-san-martino-etal-2019.py
 src/nlproc_tools/datasets/frank.py
 src/nlproc_tools/datasets/mqm.py
 src/nlproc_tools/datasets/salsa.py
 src/nlproc_tools/datasets/scarecrow.py
```

