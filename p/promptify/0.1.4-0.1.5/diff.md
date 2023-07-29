# Comparing `tmp/promptify-0.1.4.tar.gz` & `tmp/promptify-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptify-0.1.4.tar", last modified: Thu Jan 26 18:40:16 2023, max compression
+gzip compressed data, was "promptify-0.1.5.tar", last modified: Sat Jul 29 12:32:51 2023, max compression
```

## Comparing `promptify-0.1.4.tar` & `promptify-0.1.5.tar`

### file list

```diff
@@ -1,67 +1,135 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 18:40:16.580687 promptify-0.1.4/
--rw-r--r--   0 root         (0) root         (0)     1799 2023-01-26 18:39:55.000000 promptify-0.1.4/.gitignore
--rw-r--r--   0 root         (0) root         (0)    11357 2023-01-26 18:39:55.000000 promptify-0.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      258 2023-01-26 18:39:55.000000 promptify-0.1.4/Makefile
--rw-r--r--   0 root         (0) root         (0)     4444 2023-01-26 18:40:16.579687 promptify-0.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3979 2023-01-26 18:39:55.000000 promptify-0.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 18:40:16.568687 promptify-0.1.4/examples/
--rw-r--r--   0 root         (0) root         (0)    13573 2023-01-26 18:39:55.000000 promptify-0.1.4/examples/classification.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 18:40:16.570687 promptify-0.1.4/examples/data/
--rw-r--r--   0 root         (0) root         (0)     2179 2023-01-26 18:39:55.000000 promptify-0.1.4/examples/data/binary.json
--rw-r--r--   0 root         (0) root         (0)     1885 2023-01-26 18:39:55.000000 promptify-0.1.4/examples/data/multiclass.json
--rw-r--r--   0 root         (0) root         (0)     4391 2023-01-26 18:39:55.000000 promptify-0.1.4/examples/data/optimized_multilabel.json
--rw-r--r--   0 root         (0) root         (0)     7069 2023-01-26 18:39:55.000000 promptify-0.1.4/examples/data/optimized_ner.json
--rw-r--r--   0 root         (0) root         (0)     3474 2023-01-26 18:39:55.000000 promptify-0.1.4/examples/data/paragraph.json
--rw-r--r--   0 root         (0) root         (0)     6026 2023-01-26 18:39:55.000000 promptify-0.1.4/examples/data/qa.json
--rw-r--r--   0 root         (0) root         (0)    15569 2023-01-26 18:39:55.000000 promptify-0.1.4/examples/examples.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 18:40:16.572687 promptify-0.1.4/logo/
--rw-r--r--   0 root         (0) root         (0)   869490 2023-01-26 18:39:55.000000 promptify-0.1.4/logo/logo.png
--rw-r--r--   0 root         (0) root         (0)   231031 2023-01-26 18:39:55.000000 promptify-0.1.4/logo/multilabel.png
--rw-r--r--   0 root         (0) root         (0)   265368 2023-01-26 18:39:55.000000 promptify-0.1.4/logo/ner.png
--rw-r--r--   0 root         (0) root         (0)   262245 2023-01-26 18:39:55.000000 promptify-0.1.4/logo/qa_gen.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 18:40:16.573687 promptify-0.1.4/promptify/
--rw-r--r--   0 root         (0) root         (0)        6 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/VERSION
--rw-r--r--   0 root         (0) root         (0)      109 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 18:40:16.574687 promptify-0.1.4/promptify/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 18:40:16.575687 promptify-0.1.4/promptify/models/nlp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/models/nlp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/models/nlp/model.py
--rw-r--r--   0 root         (0) root         (0)     3760 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/models/nlp/openai_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 18:40:16.576687 promptify-0.1.4/promptify/models/nlp/utils/
--rw-r--r--   0 root         (0) root         (0)       37 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/models/nlp/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3749 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/models/nlp/utils/bpe_encoder.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/models/nlp/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 18:40:16.576687 promptify-0.1.4/promptify/models/tabular/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/models/tabular/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 18:40:16.576687 promptify-0.1.4/promptify/models/vision/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/models/vision/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 18:40:16.576687 promptify-0.1.4/promptify/prompts/
--rw-r--r--   0 root         (0) root         (0)        2 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/prompts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 18:40:16.577687 promptify-0.1.4/promptify/prompts/nlp/
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/prompts/nlp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2321 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/prompts/nlp/prompter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 18:40:16.579687 promptify-0.1.4/promptify/prompts/nlp/templates/
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/prompts/nlp/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      545 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/prompts/nlp/templates/binary_classification.jinja
--rw-r--r--   0 root         (0) root         (0)      603 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/prompts/nlp/templates/explain.jinja
--rw-r--r--   0 root         (0) root         (0)      610 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/prompts/nlp/templates/multiclass_classification.jinja
--rw-r--r--   0 root         (0) root         (0)     1067 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/prompts/nlp/templates/multilabel_classification.jinja
--rw-r--r--   0 root         (0) root         (0)     1825 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/prompts/nlp/templates/ner.jinja
--rw-r--r--   0 root         (0) root         (0)      861 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/prompts/nlp/templates/qa.jinja
--rw-r--r--   0 root         (0) root         (0)     1058 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/prompts/nlp/templates/qa_gen.jinja
--rw-r--r--   0 root         (0) root         (0)      789 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/prompts/nlp/templates/summary.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 18:40:16.579687 promptify-0.1.4/promptify/prompts/tabular/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/prompts/tabular/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 18:40:16.579687 promptify-0.1.4/promptify/prompts/vision/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-26 18:39:55.000000 promptify-0.1.4/promptify/prompts/vision/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 18:40:16.574687 promptify-0.1.4/promptify.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4444 2023-01-26 18:40:16.000000 promptify-0.1.4/promptify.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1529 2023-01-26 18:40:16.000000 promptify-0.1.4/promptify.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-26 18:40:16.000000 promptify-0.1.4/promptify.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      113 2023-01-26 18:40:16.000000 promptify-0.1.4/promptify.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-01-26 18:40:16.000000 promptify-0.1.4/promptify.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-01-26 18:39:55.000000 promptify-0.1.4/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-01-26 18:39:55.000000 promptify-0.1.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-26 18:40:16.580687 promptify-0.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1375 2023-01-26 18:39:55.000000 promptify-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.016544 promptify-0.1.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-29 12:32:45.000000 promptify-0.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-07-29 12:32:51.016544 promptify-0.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6965 2023-07-29 12:32:45.000000 promptify-0.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:50.998544 promptify-0.1.5/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/benchmarks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:50.998544 promptify-0.1.5/examples/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/examples/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-07-29 12:32:45.000000 promptify-0.1.5/examples/medical_ner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:50.998544 promptify-0.1.5/promptify/
+-rw-r--r--   0 root         (0) root         (0)      776 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.000544 promptify-0.1.5/promptify/data/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.000544 promptify-0.1.5/promptify/data/text2text/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/data/text2text/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.000544 promptify-0.1.5/promptify/data/text2text/en/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/data/text2text/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.000544 promptify-0.1.5/promptify/databases/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/databases/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.000544 promptify-0.1.5/promptify/embeddings/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/embeddings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.001544 promptify-0.1.5/promptify/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.001544 promptify-0.1.5/promptify/models/text2image/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/models/text2image/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.001544 promptify-0.1.5/promptify/models/text2text/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/models/text2text/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.003544 promptify-0.1.5/promptify/models/text2text/api/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/models/text2text/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/models/text2text/api/anthropic.py
+-rw-r--r--   0 root         (0) root         (0)     5681 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/models/text2text/api/azure_openai.py
+-rw-r--r--   0 root         (0) root         (0)    12087 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/models/text2text/api/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/models/text2text/api/cohere.py
+-rw-r--r--   0 root         (0) root         (0)     5631 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/models/text2text/api/hub_model.py
+-rw-r--r--   0 root         (0) root         (0)     4433 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/models/text2text/api/mock_model.py
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/models/text2text/api/openai_models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.003544 promptify-0.1.5/promptify/models/text2text/inference/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/models/text2text/inference/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.003544 promptify-0.1.5/promptify/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12197 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/parser/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.003544 promptify-0.1.5/promptify/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3542 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/pipelines/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.004544 promptify-0.1.5/promptify/plugins/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/plugins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.005544 promptify-0.1.5/promptify/prompter/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompter/conversation_logger.py
+-rw-r--r--   0 root         (0) root         (0)     3640 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompter/nlp_prompter.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompter/prompt_cache.py
+-rw-r--r--   0 root         (0) root         (0)     5401 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompter/template_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.005544 promptify-0.1.5/promptify/prompts/
+-rw-r--r--   0 root         (0) root         (0)        2 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.005544 promptify-0.1.5/promptify/prompts/text2image/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2image/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.005544 promptify-0.1.5/promptify/prompts/text2text/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.006544 promptify-0.1.5/promptify/prompts/text2text/binary_classification/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/binary_classification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      545 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/binary_classification/binary_classification.jinja
+-rw-r--r--   0 root         (0) root         (0)     1549 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/binary_classification/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.007544 promptify-0.1.5/promptify/prompts/text2text/explain/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/explain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/explain/explain.jinja
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/explain/metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.007544 promptify-0.1.5/promptify/prompts/text2text/multiclass_classification/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/multiclass_classification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/multiclass_classification/metadata.json
+-rw-r--r--   0 root         (0) root         (0)      610 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/multiclass_classification/multiclass_classification.jinja
+-rw-r--r--   0 root         (0) root         (0)      610 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/multiclass_classification/multiclass_gpt.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.008544 promptify-0.1.5/promptify/prompts/text2text/multilabel_classification/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/multilabel_classification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/multilabel_classification/metadata.json
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/multilabel_classification/multilabel_classification.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.008544 promptify-0.1.5/promptify/prompts/text2text/ner/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/ner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/ner/metadata.json
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/ner/ner_openai.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.009544 promptify-0.1.5/promptify/prompts/text2text/qa/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/qa/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/qa/metadata.json
+-rw-r--r--   0 root         (0) root         (0)      864 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/qa/qa.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.010544 promptify-0.1.5/promptify/prompts/text2text/qa_gen/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/qa_gen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/qa_gen/metadata.json
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/qa_gen/qa_gen.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.010544 promptify-0.1.5/promptify/prompts/text2text/relation_extraction/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/relation_extraction/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/relation_extraction/metadata.json
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/relation_extraction/relation_extraction.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.011544 promptify-0.1.5/promptify/prompts/text2text/sql_writer/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/sql_writer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/sql_writer/metadata.json
+-rw-r--r--   0 root         (0) root         (0)      867 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/sql_writer/sql_writer_gpt.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.011544 promptify-0.1.5/promptify/prompts/text2text/summary/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/summary/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      792 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/summary/summary.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.012544 promptify-0.1.5/promptify/prompts/text2text/tabular_extractor/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/tabular_extractor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/tabular_extractor/metadata.json
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/tabular_extractor/tabular_extractor_gpt.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.012544 promptify-0.1.5/promptify/prompts/text2text/text_normalization/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/text_normalization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      756 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/text_normalization/text_normalization_draft.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.013544 promptify-0.1.5/promptify/prompts/text2text/topic_modelling/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/topic_modelling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1478 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/prompts/text2text/topic_modelling/topic_modeling_draft.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.013544 promptify-0.1.5/promptify/utils/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2424 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/utils/conversation_utils.py
+-rw-r--r--   0 root         (0) root         (0)      532 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/utils/data_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2023-07-29 12:32:45.000000 promptify-0.1.5/promptify/utils/file_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:50.999544 promptify-0.1.5/promptify.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-07-29 12:32:50.000000 promptify-0.1.5/promptify.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4059 2023-07-29 12:32:50.000000 promptify-0.1.5/promptify.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:50.000000 promptify-0.1.5/promptify.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-29 12:32:50.000000 promptify-0.1.5/promptify.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-29 12:32:50.000000 promptify-0.1.5/promptify.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 12:32:51.016544 promptify-0.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1330 2023-07-29 12:32:45.000000 promptify-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.013544 promptify-0.1.5/tests/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.014544 promptify-0.1.5/tests/unit_tests/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/tests/unit_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.014544 promptify-0.1.5/tests/unit_tests/models/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/tests/unit_tests/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-07-29 12:32:45.000000 promptify-0.1.5/tests/unit_tests/models/test_base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-07-29 12:32:45.000000 promptify-0.1.5/tests/unit_tests/models/test_hf_model.py
+-rw-r--r--   0 root         (0) root         (0)     7580 2023-07-29 12:32:45.000000 promptify-0.1.5/tests/unit_tests/models/test_openai_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.015544 promptify-0.1.5/tests/unit_tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/tests/unit_tests/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5427 2023-07-29 12:32:45.000000 promptify-0.1.5/tests/unit_tests/parser/test_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:32:51.015544 promptify-0.1.5/tests/unit_tests/prompter/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:32:45.000000 promptify-0.1.5/tests/unit_tests/prompter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4179 2023-07-29 12:32:45.000000 promptify-0.1.5/tests/unit_tests/prompter/test_prompter.py
```

### Comparing `promptify-0.1.4/LICENSE` & `promptify-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `promptify-0.1.4/examples/data/binary.json` & `promptify-0.1.5/promptify/prompts/text2text/binary_classification/metadata.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

```diff
@@ -1,62 +1,48 @@
 [
     {
-        "complexity": "",
-        "labels": "negative",
-        "score": "",
-        "text": "Eight years the republicans denied obama\u2019s picks. Breitbarters outrage is as phony as their fake president."
-    },
-    {
-        "complexity": "",
-        "labels": "positive",
-        "score": "",
-        "text": "Except he\u2019s the most successful president in our lifetimes. He\u2019s undone most of the damage Obummer did and set America on the right path again."
-    },
-    {
-        "complexity": "",
-        "labels": "negative",
-        "score": "",
-        "text": "So disappointed in wwe summerslam! I want to see john cena wins his 16th title"
-    },
-    {
-        "complexity": "",
-        "labels": "positive",
-        "score": "",
-        "text": "Looking forward to going to Carrow Rd tonight. Last time we were there\\u002c Bale scored 2 and we were 3rd. Do not want extra time though"
-    },
-    {
-        "complexity": "",
-        "labels": "positive",
-        "score": "",
-        "text": "It's a good day at work when you get to shake Jim Lehrer's hand. Thanks, @user Still kicking myself for being to shy to hug"
-    },
-    {
-        "complexity": "",
-        "labels": "negative",
-        "score": "",
-        "text": "Trumpism likewise rests on a bed of racial resentment that was made knowingly and intentionally, long before Trump got into politics."
-    },
-    {
-        "complexity": "",
-        "labels": "positive",
-        "score": "",
-        "text": "i have been with petronas for years i feel that petronas has performed well and made a huge profit"
-    },
-    {
-        "complexity": "",
-        "labels": "negative",
-        "score": "",
-        "text": "i have been with petronas for years i feel that petronas has performed well and made a huge profit"
-    },
-    {
-        "complexity": "",
-        "labels": "positive",
-        "score": "",
-        "text": "I've read many post on here saying Israel gives training to US law enforcement ."
-    },
-    {
-        "complexity": "",
-        "labels": "negative",
-        "review": "And the sad thing is the white students at those schools will act like that too .",
-        "score": ""
+        "authors": "Ankit Pal",
+        "citation": "Pal, A. (2022). Prompt for classifying text into two classes using Large Language Models(LLMs). [Computer software]. Retrieved from https://github.com/promptslab/Promptify/tree/main/promptify/prompts/text2text/binary_classification.jinja",
+        "contributors": [],
+        "created": "Dec 12, 2022, 11:36 PM",
+        "description": "Prompt for classifying text into two classes using Large Language Models(LLMs).",
+        "file_name": "binary_classification.jinja",
+        "github": "monk1337",
+        "language": "en",
+        "license": {
+            "name": "CC BY-SA 4.0",
+            "restrictions": "None",
+            "url": "https://creativecommons.org/licenses/by-sa/4.0/"
+        },
+        "limitations": "",
+        "llm_parameters": {
+            "temperature": 0.7
+        },
+        "models": [
+            "text-davinci-003",
+            "gpt-3.5-turbo"
+        ],
+        "nft": "",
+        "point_of_contact": "aadityaura@gmail.com",
+        "prompt_id": "1115d146-e47e-4187-bccd-b67ced35eeb6",
+        "sample_data": "binary_classification_data.json",
+        "sample_output": {
+            "labels": "negative"
+        },
+        "source": "Original",
+        "tags": [
+            "text_classification",
+            "natural_language_processing",
+            "text_analysis",
+            "binary_classification",
+            "nlp",
+            "text",
+            "classification",
+            "binary",
+            "two",
+            "classes"
+        ],
+        "task": "Binary Text Classification",
+        "updated": "2023-04-21",
+        "version": "1.1"
     }
 ]
```

### Comparing `promptify-0.1.4/promptify/prompts/nlp/templates/binary_classification.jinja` & `promptify-0.1.5/promptify/prompts/text2text/binary_classification/binary_classification.jinja`

 * *Files identical despite different names*

### Comparing `promptify-0.1.4/promptify/prompts/nlp/templates/explain.jinja` & `promptify-0.1.5/promptify/prompts/text2text/explain/explain.jinja`

 * *Files identical despite different names*

### Comparing `promptify-0.1.4/promptify/prompts/nlp/templates/multiclass_classification.jinja` & `promptify-0.1.5/promptify/prompts/text2text/multiclass_classification/multiclass_classification.jinja`

 * *Files identical despite different names*

### Comparing `promptify-0.1.4/promptify/prompts/nlp/templates/multilabel_classification.jinja` & `promptify-0.1.5/promptify/prompts/text2text/multilabel_classification/multilabel_classification.jinja`

 * *Files identical despite different names*

### Comparing `promptify-0.1.4/promptify/prompts/nlp/templates/ner.jinja` & `promptify-0.1.5/promptify/prompts/text2text/ner/ner_openai.jinja`

 * *Files 13% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 {%- if labels is not none -%}
 You are a highly intelligent and accurate Named-entity recognition(NER) system. You take Passage as input and your task is to recognize and extract specific types of named entities in that given passage and classify into a set of following predefined entity types:
 {{ labels }}
 {%- else -%}
 You are a highly intelligent and accurate Named-entity recognition(NER) system. You take Passage as input and your task is to recognize and extract specific types of named entities in that given passage and classify into a set of entity types.
 {%- endif -%}
 {% endif -%}
-Your output format is only {{ output_format|default("[{{'T': type of entity from predefined entity types, 'E': entity in the input text}},...,{{'branch' : Appropriate branch of the passage ,'group': Appropriate Group of the passage}}]") }} form, no other form.
+Your output format is only {{ output_format|default("[{'T': type of entity from predefined entity types, 'E': entity in the input text}},...,{{'branch' : Appropriate branch of the passage ,'group': Appropriate Group of the passage}]") }} form, no other form. Don't include any text in response such as 'here are named entities..' etc, return only valid json
 
 {% if examples is defined and examples|length > 0 -%}
 Examples:
 {% for sentence, label in examples %}
 Input: {{ sentence }}
 Output: [{{ label }}]
 {% endfor %}
 {% endif -%}
 
 Input: {{ text_input }}
-Output:
+Output:
```

### Comparing `promptify-0.1.4/promptify/prompts/nlp/templates/qa.jinja` & `promptify-0.1.5/promptify/prompts/text2text/qa/qa.jinja`

 * *Files 14% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 {% if examples is defined and examples|length > 0 -%}
 Examples:
 {% for example in examples %}
 {{ example }}
 {% endfor %}
 {% endif -%}
 
-Context: {{ context }}
+Context: {{ text_input }}
 Question: {{ question }}
 Output:
```

### Comparing `promptify-0.1.4/promptify/prompts/nlp/templates/qa_gen.jinja` & `promptify-0.1.5/promptify/prompts/text2text/qa_gen/qa_gen.jinja`

 * *Files identical despite different names*

### Comparing `promptify-0.1.4/promptify/prompts/nlp/templates/summary.jinja` & `promptify-0.1.5/promptify/prompts/text2text/summary/summary.jinja`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 {% endif -%}
 
 {%- if domain is not none -%}
 {%- if token_length is not none -%}
 You are a highly intelligent {{ domain }} domain expert Summarization system. You take Passage as input and summarize the passage as a {{ domain }} expert in {{ token_length }} tokens.
 {%- else -%}
 You are a highly intelligent {{ domain }} domain expert Summarization system. You take Passage as input and summarize the passage as a {{ domain }} expert.
-{% endif -%}
-{% else %}
+{%- endif -%}
+{%- else -%}
 You are a highly intelligent Summarization system. You take Passage as input and summarize the passage as an expert.
-{% endif -%}
-Your output format is only {{ output_format|default("[{'S': Summarization paragraph}},]") } form, no other form.
+{%- endif %}
+Your output format is only {{ output_format|default("[{'S': Summarization paragraph},]") }} form, no other form.
 
 Passage: {{ text_input }}
 Output:
```

### Comparing `promptify-0.1.4/setup.py` & `promptify-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     name="promptify",
     version=read("promptify", "VERSION"),
     description="Use GPT or other prompt based models to get structured output",
     url="https://github.com/promptslab/Promptify",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     license="Apache",
-    author='monk1337',
-    maintainer="The promptslab team with the help of all our contributors (https://github.com/promptslab/Promptify/graphs/contributors)",
+    author="monk1337",
+    maintainer="The promptslab team with the help of all our contributors",
     packages=find_packages(),
-    package_data={"promptify.prompts.nlp": ["templates/*.jinja"]},
+    package_data={"promptify.prompts.text2text": ["*/*.jinja", "*/metadata.json"]},
     install_requires=read_requirements("requirements.txt"),
     python_requires=">=3.7.0",
     extras_require={"dev": read_requirements("requirements-dev.txt")},
 )
```

