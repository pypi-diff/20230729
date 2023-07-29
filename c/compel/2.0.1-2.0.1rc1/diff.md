# Comparing `tmp/compel-2.0.1.tar.gz` & `tmp/compel-2.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compel-2.0.1.tar", last modified: Sat Jul 29 15:56:43 2023, max compression
+gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-f99dy6mm/compel-2.0.1rc1.tar", last modified: Thu Jul 20 18:55:38 2023, max compression
```

## Comparing `compel-2.0.1.tar` & `compel-2.0.1rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-29 15:56:43.367762 compel-2.0.1/
--rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-2.0.1/LICENSE
--rw-r--r--   0 damian     (501) staff       (20)    12383 2023-07-29 15:56:43.363964 compel-2.0.1/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)    11805 2023-07-29 15:54:58.000000 compel-2.0.1/README.md
--rw-r--r--   0 damian     (501) staff       (20)      761 2023-07-29 15:50:29.000000 compel-2.0.1/pyproject.toml
--rw-r--r--   0 damian     (501) staff       (20)       38 2023-07-29 15:56:43.367934 compel-2.0.1/setup.cfg
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-29 15:56:43.343450 compel-2.0.1/src/
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-29 15:56:43.350781 compel-2.0.1/src/compel/
--rw-r--r--   0 damian     (501) staff       (20)      175 2023-06-03 06:15:19.000000 compel-2.0.1/src/compel/__init__.py
--rw-r--r--   0 damian     (501) staff       (20)    20868 2023-07-29 15:44:31.000000 compel-2.0.1/src/compel/compel.py
--rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-2.0.1/src/compel/conditioning_scheduler.py
--rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-2.0.1/src/compel/cross_attention_control.py
--rw-r--r--   0 damian     (501) staff       (20)      653 2023-06-03 06:15:19.000000 compel-2.0.1/src/compel/diffusers_textual_inversion_manager.py
--rw-r--r--   0 damian     (501) staff       (20)    30822 2023-07-20 18:51:59.000000 compel-2.0.1/src/compel/embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    30771 2023-07-04 21:57:36.000000 compel-2.0.1/src/compel/prompt_parser.py
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-29 15:56:43.358412 compel-2.0.1/src/compel.egg-info/
--rw-r--r--   0 damian     (501) staff       (20)    12383 2023-07-29 15:56:43.000000 compel-2.0.1/src/compel.egg-info/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)      512 2023-07-29 15:56:43.000000 compel-2.0.1/src/compel.egg-info/SOURCES.txt
--rw-r--r--   0 damian     (501) staff       (20)        1 2023-07-29 15:56:43.000000 compel-2.0.1/src/compel.egg-info/dependency_links.txt
--rw-r--r--   0 damian     (501) staff       (20)       56 2023-07-29 15:56:43.000000 compel-2.0.1/src/compel.egg-info/requires.txt
--rw-r--r--   0 damian     (501) staff       (20)        7 2023-07-29 15:56:43.000000 compel-2.0.1/src/compel.egg-info/top_level.txt
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-29 15:56:43.362389 compel-2.0.1/test/
--rw-r--r--   0 damian     (501) staff       (20)    16457 2023-07-18 10:18:45.000000 compel-2.0.1/test/test_compel.py
--rw-r--r--   0 damian     (501) staff       (20)    21072 2023-06-03 06:15:11.000000 compel-2.0.1/test/test_embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    47562 2023-06-03 06:55:54.000000 compel-2.0.1/test/test_prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-20 18:55:38.000000 compel-2.0.1rc1/
+-rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-2.0.1rc1/LICENSE
+-rw-r--r--   0 damian     (501) staff       (20)    12250 2023-07-20 18:55:38.000000 compel-2.0.1rc1/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)    11669 2023-07-18 14:01:58.000000 compel-2.0.1rc1/README.md
+-rw-r--r--   0 damian     (501) staff       (20)      766 2023-07-20 18:55:28.000000 compel-2.0.1rc1/pyproject.toml
+-rw-r--r--   0 damian     (501) staff       (20)       38 2023-07-20 18:55:38.000000 compel-2.0.1rc1/setup.cfg
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel/
+-rw-r--r--   0 damian     (501) staff       (20)      175 2023-06-03 06:15:19.000000 compel-2.0.1rc1/src/compel/__init__.py
+-rw-r--r--   0 damian     (501) staff       (20)    20730 2023-07-20 18:51:59.000000 compel-2.0.1rc1/src/compel/compel.py
+-rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-2.0.1rc1/src/compel/conditioning_scheduler.py
+-rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-2.0.1rc1/src/compel/cross_attention_control.py
+-rw-r--r--   0 damian     (501) staff       (20)      653 2023-06-03 06:15:19.000000 compel-2.0.1rc1/src/compel/diffusers_textual_inversion_manager.py
+-rw-r--r--   0 damian     (501) staff       (20)    30822 2023-07-20 18:51:59.000000 compel-2.0.1rc1/src/compel/embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    30771 2023-07-04 21:57:36.000000 compel-2.0.1rc1/src/compel/prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel.egg-info/
+-rw-r--r--   0 damian     (501) staff       (20)    12250 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel.egg-info/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)      512 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel.egg-info/SOURCES.txt
+-rw-r--r--   0 damian     (501) staff       (20)        1 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel.egg-info/dependency_links.txt
+-rw-r--r--   0 damian     (501) staff       (20)       56 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel.egg-info/requires.txt
+-rw-r--r--   0 damian     (501) staff       (20)        7 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel.egg-info/top_level.txt
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-20 18:55:38.000000 compel-2.0.1rc1/test/
+-rw-r--r--   0 damian     (501) staff       (20)    16457 2023-07-18 10:18:45.000000 compel-2.0.1rc1/test/test_compel.py
+-rw-r--r--   0 damian     (501) staff       (20)    21072 2023-06-03 06:15:11.000000 compel-2.0.1rc1/test/test_embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    47562 2023-06-03 06:55:54.000000 compel-2.0.1rc1/test/test_prompt_parser.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `compel-2.0.1/LICENSE` & `compel-2.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `compel-2.0.1/PKG-INFO` & `compel-2.0.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 2.0.1
+Version: 2.0.1rc1
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -95,16 +95,14 @@
 If this doesn't help, you could try this advice offered by @kshieh1: 
 > After image generation, you should explictly de-reference the tensor object (i.e., prompt_embeds = None) and call gc.collect()
 
 See https://github.com/damian0815/compel/issues/24 for more details. Thanks @kshieh1 !
 
 ## Changelog
 
-#### 2.0.1 - fix for [#45](https://github.com/damian0815/compel/issues/45) padding issue with SDXL non-truncated prompts and `.and()` 
-
 ### 2.0.0 - SDXL Support
 
 With big thanks to Patrick von Platen from Hugging Face for [the pull request](https://github.com/damian0815/compel/pull/41), Compel now supports SDXL. Use it like this: 
 
 ```
 from compel import Compel, ReturnedEmbeddingsType
 from diffusers import DiffusionPipeline
```

### Comparing `compel-2.0.1/README.md` & `compel-2.0.1rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,14 @@
 If this doesn't help, you could try this advice offered by @kshieh1: 
 > After image generation, you should explictly de-reference the tensor object (i.e., prompt_embeds = None) and call gc.collect()
 
 See https://github.com/damian0815/compel/issues/24 for more details. Thanks @kshieh1 !
 
 ## Changelog
 
-#### 2.0.1 - fix for [#45](https://github.com/damian0815/compel/issues/45) padding issue with SDXL non-truncated prompts and `.and()` 
-
 ### 2.0.0 - SDXL Support
 
 With big thanks to Patrick von Platen from Hugging Face for [the pull request](https://github.com/damian0815/compel/pull/41), Compel now supports SDXL. Use it like this: 
 
 ```
 from compel import Compel, ReturnedEmbeddingsType
 from diffusers import DiffusionPipeline
```

### Comparing `compel-2.0.1/pyproject.toml` & `compel-2.0.1rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "compel"
-version = "2.0.1"
+version = "2.0.1-pre1"
 authors = [
   { name="Damian Stewart", email="null@damianstewart.com" },
 ]
 description = "A prompting enhancement library for transformers-type text embedding systems."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `compel-2.0.1/src/compel/compel.py` & `compel-2.0.1rc1/src/compel/compel.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,17 +221,15 @@
             conditionings = [c.unsqueeze(0) for c in conditionings]
             c0_shape = conditionings[0].shape
         if len(c0_shape) != 3:
             raise ValueError(f"All conditioning tensors must have the same number of dimensions (2 or 3)")
 
         if not all([c.shape[0] == c0_shape[0] and c.shape[2] == c0_shape[2] for c in conditionings]):
             raise ValueError(f"All conditioning tensors must have the same batch size ({c0_shape[0]}) and number of embeddings per token ({c0_shape[1]}")
-        
-        if len(emptystring_conditioning.shape) == 2:
-            emptystring_conditioning = emptystring_conditioning.unsqueeze(0)
+
         empty_z = torch.cat([emptystring_conditioning] * c0_shape[0])
         max_token_count = max([c.shape[1] for c in conditionings])
         # if necessary, pad shorter tensors out with an emptystring tensor
         for i, c in enumerate(conditionings):
             while c.shape[1] < max_token_count:
                 c = torch.cat([c, empty_z], dim=1)
                 conditionings[i] = c
```

### Comparing `compel-2.0.1/src/compel/conditioning_scheduler.py` & `compel-2.0.1rc1/src/compel/conditioning_scheduler.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.1/src/compel/cross_attention_control.py` & `compel-2.0.1rc1/src/compel/cross_attention_control.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.1/src/compel/diffusers_textual_inversion_manager.py` & `compel-2.0.1rc1/src/compel/diffusers_textual_inversion_manager.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.1/src/compel/embeddings_provider.py` & `compel-2.0.1rc1/src/compel/embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.1/src/compel/prompt_parser.py` & `compel-2.0.1rc1/src/compel/prompt_parser.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.1/src/compel.egg-info/PKG-INFO` & `compel-2.0.1rc1/src/compel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 2.0.1
+Version: 2.0.1rc1
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -95,16 +95,14 @@
 If this doesn't help, you could try this advice offered by @kshieh1: 
 > After image generation, you should explictly de-reference the tensor object (i.e., prompt_embeds = None) and call gc.collect()
 
 See https://github.com/damian0815/compel/issues/24 for more details. Thanks @kshieh1 !
 
 ## Changelog
 
-#### 2.0.1 - fix for [#45](https://github.com/damian0815/compel/issues/45) padding issue with SDXL non-truncated prompts and `.and()` 
-
 ### 2.0.0 - SDXL Support
 
 With big thanks to Patrick von Platen from Hugging Face for [the pull request](https://github.com/damian0815/compel/pull/41), Compel now supports SDXL. Use it like this: 
 
 ```
 from compel import Compel, ReturnedEmbeddingsType
 from diffusers import DiffusionPipeline
```

### Comparing `compel-2.0.1/src/compel.egg-info/SOURCES.txt` & `compel-2.0.1rc1/src/compel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compel-2.0.1/test/test_compel.py` & `compel-2.0.1rc1/test/test_compel.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.1/test/test_embeddings_provider.py` & `compel-2.0.1rc1/test/test_embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.1/test/test_prompt_parser.py` & `compel-2.0.1rc1/test/test_prompt_parser.py`

 * *Files identical despite different names*

