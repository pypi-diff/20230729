# Comparing `tmp/cerebrium-1.3.0.tar.gz` & `tmp/cerebrium-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-1.3.0.tar", max compression
+gzip compressed data, was "cerebrium-1.3.1.tar", max compression
```

## Comparing `cerebrium-1.3.0.tar` & `cerebrium-1.3.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      372 2023-07-25 14:13:12.773940 cerebrium-1.3.0/EXTERNAL_README.md
--rw-r--r--   0        0        0    34594 2023-07-25 14:13:12.777940 cerebrium-1.3.0/LICENSE
--rw-r--r--   0        0        0      360 2023-07-25 14:16:12.471104 cerebrium-1.3.0/cerebrium/__init__.py
--rwxr-xr-x   0        0        0    36049 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/cli.py
--rw-r--r--   0        0        0    35162 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/conduit.py
--rw-r--r--   0        0        0     5048 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/core.py
--rw-r--r--   0        0        0     2488 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/errors.py
--rw-r--r--   0        0        0    10182 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/flow.py
--rw-r--r--   0        0        0     3070 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3990 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      600 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/models/base.py
--rw-r--r--   0        0        0      550 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/models/hf_pipeline.py
--rw-r--r--   0        0        0      411 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/models/onnx.py
--rw-r--r--   0        0        0      793 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      270 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      273 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/models/torch.py
--rw-r--r--   0        0        0     8545 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/requests.py
--rw-r--r--   0        0        0    10957 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/README_Diffusers.md
--rw-r--r--   0        0        0     5592 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/README_Transformers.md
--rw-r--r--   0        0        0      110 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/__init__.py
--rw-r--r--   0        0        0     2515 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/config/diffuser.yaml
--rw-r--r--   0        0        0     1940 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/config/falcon-40b.yaml
--rw-r--r--   0        0        0     1864 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/config/falcon-7b.yaml
--rw-r--r--   0        0        0     1916 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/config/llama-13b.yaml
--rw-r--r--   0        0        0     1692 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/config/llama-7b.yaml
--rw-r--r--   0        0        0     1991 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/config/llama2-13b.yaml
--rw-r--r--   0        0        0     1751 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/config/llama2-7b.yaml
--rw-r--r--   0        0        0     1747 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/config/transformer.yaml
--rw-r--r--   0        0        0    15030 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/diffuser_tuner.py
--rw-r--r--   0        0        0     8826 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/fine_tuner.py
--rw-r--r--   0        0        0     1716 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/finetune_LLM/finetuning_model.py
--rw-r--r--   0        0        0        0 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/finetune_LLM/userDataset/__init__.py
--rw-r--r--   0        0        0     2647 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py
--rw-r--r--   0        0        0     4115 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py
--rw-r--r--   0        0        0     1048 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/utils.py
--rw-r--r--   0        0        0     2346 2023-07-25 14:16:12.467104 cerebrium-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 cerebrium-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      372 2023-07-29 14:10:33.220170 cerebrium-1.3.1/EXTERNAL_README.md
+-rw-r--r--   0        0        0    34594 2023-07-29 14:10:33.220170 cerebrium-1.3.1/LICENSE
+-rw-r--r--   0        0        0      360 2023-07-29 14:13:03.751144 cerebrium-1.3.1/cerebrium/__init__.py
+-rwxr-xr-x   0        0        0    36049 2023-07-29 14:10:33.220170 cerebrium-1.3.1/cerebrium/cli.py
+-rw-r--r--   0        0        0    35162 2023-07-29 14:10:33.220170 cerebrium-1.3.1/cerebrium/conduit.py
+-rw-r--r--   0        0        0     5048 2023-07-29 14:10:33.220170 cerebrium-1.3.1/cerebrium/core.py
+-rw-r--r--   0        0        0     2488 2023-07-29 14:10:33.220170 cerebrium-1.3.1/cerebrium/errors.py
+-rw-r--r--   0        0        0    10182 2023-07-29 14:10:33.220170 cerebrium-1.3.1/cerebrium/flow.py
+-rw-r--r--   0        0        0     3070 2023-07-29 14:10:33.220170 cerebrium-1.3.1/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-07-29 14:10:33.220170 cerebrium-1.3.1/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3990 2023-07-29 14:10:33.220170 cerebrium-1.3.1/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      600 2023-07-29 14:10:33.220170 cerebrium-1.3.1/cerebrium/models/base.py
+-rw-r--r--   0        0        0      550 2023-07-29 14:10:33.220170 cerebrium-1.3.1/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      431 2023-07-29 14:10:33.220170 cerebrium-1.3.1/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0      793 2023-07-29 14:10:33.220170 cerebrium-1.3.1/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      270 2023-07-29 14:10:33.220170 cerebrium-1.3.1/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      273 2023-07-29 14:10:33.220170 cerebrium-1.3.1/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     8545 2023-07-29 14:10:33.224171 cerebrium-1.3.1/cerebrium/requests.py
+-rw-r--r--   0        0        0    10957 2023-07-29 14:10:33.224171 cerebrium-1.3.1/cerebrium/trainer/README_Diffusers.md
+-rw-r--r--   0        0        0     5592 2023-07-29 14:10:33.224171 cerebrium-1.3.1/cerebrium/trainer/README_Transformers.md
+-rw-r--r--   0        0        0      110 2023-07-29 14:10:33.224171 cerebrium-1.3.1/cerebrium/trainer/__init__.py
+-rw-r--r--   0        0        0     2515 2023-07-29 14:10:33.224171 cerebrium-1.3.1/cerebrium/trainer/config/diffuser.yaml
+-rw-r--r--   0        0        0     1940 2023-07-29 14:10:33.224171 cerebrium-1.3.1/cerebrium/trainer/config/falcon-40b.yaml
+-rw-r--r--   0        0        0     1864 2023-07-29 14:10:33.224171 cerebrium-1.3.1/cerebrium/trainer/config/falcon-7b.yaml
+-rw-r--r--   0        0        0     1916 2023-07-29 14:10:33.224171 cerebrium-1.3.1/cerebrium/trainer/config/llama-13b.yaml
+-rw-r--r--   0        0        0     1692 2023-07-29 14:10:33.224171 cerebrium-1.3.1/cerebrium/trainer/config/llama-7b.yaml
+-rw-r--r--   0        0        0     1991 2023-07-29 14:10:33.224171 cerebrium-1.3.1/cerebrium/trainer/config/llama2-13b.yaml
+-rw-r--r--   0        0        0     1751 2023-07-29 14:10:33.224171 cerebrium-1.3.1/cerebrium/trainer/config/llama2-7b.yaml
+-rw-r--r--   0        0        0     1747 2023-07-29 14:10:33.224171 cerebrium-1.3.1/cerebrium/trainer/config/transformer.yaml
+-rw-r--r--   0        0        0    15030 2023-07-29 14:10:33.224171 cerebrium-1.3.1/cerebrium/trainer/diffuser_tuner.py
+-rw-r--r--   0        0        0     8826 2023-07-29 14:10:33.224171 cerebrium-1.3.1/cerebrium/trainer/fine_tuner.py
+-rw-r--r--   0        0        0     1716 2023-07-29 14:10:33.224171 cerebrium-1.3.1/cerebrium/trainer/finetune_LLM/finetuning_model.py
+-rw-r--r--   0        0        0        0 2023-07-29 14:10:33.224171 cerebrium-1.3.1/cerebrium/trainer/finetune_LLM/userDataset/__init__.py
+-rw-r--r--   0        0        0     2647 2023-07-29 14:10:33.224171 cerebrium-1.3.1/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py
+-rw-r--r--   0        0        0     4115 2023-07-29 14:10:33.224171 cerebrium-1.3.1/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py
+-rw-r--r--   0        0        0     1048 2023-07-29 14:10:33.224171 cerebrium-1.3.1/cerebrium/utils.py
+-rw-r--r--   0        0        0     2346 2023-07-29 14:13:03.751144 cerebrium-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 cerebrium-1.3.1/PKG-INFO
```

### Comparing `cerebrium-1.3.0/LICENSE` & `cerebrium-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/cli.py` & `cerebrium-1.3.1/cerebrium/cli.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/conduit.py` & `cerebrium-1.3.1/cerebrium/conduit.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/core.py` & `cerebrium-1.3.1/cerebrium/core.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/errors.py` & `cerebrium-1.3.1/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/flow.py` & `cerebrium-1.3.1/cerebrium/flow.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/logging/arize.py` & `cerebrium-1.3.1/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/logging/base.py` & `cerebrium-1.3.1/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/logging/censius.py` & `cerebrium-1.3.1/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/models/base.py` & `cerebrium-1.3.1/cerebrium/models/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/models/hf_pipeline.py` & `cerebrium-1.3.1/cerebrium/models/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/models/sklearn.py` & `cerebrium-1.3.1/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/requests.py` & `cerebrium-1.3.1/cerebrium/requests.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/trainer/README_Diffusers.md` & `cerebrium-1.3.1/cerebrium/trainer/README_Diffusers.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/trainer/README_Transformers.md` & `cerebrium-1.3.1/cerebrium/trainer/README_Transformers.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/trainer/config/diffuser.yaml` & `cerebrium-1.3.1/cerebrium/trainer/config/diffuser.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/trainer/config/falcon-40b.yaml` & `cerebrium-1.3.1/cerebrium/trainer/config/falcon-40b.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/trainer/config/falcon-7b.yaml` & `cerebrium-1.3.1/cerebrium/trainer/config/falcon-7b.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/trainer/config/llama-13b.yaml` & `cerebrium-1.3.1/cerebrium/trainer/config/llama-13b.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/trainer/config/llama-7b.yaml` & `cerebrium-1.3.1/cerebrium/trainer/config/llama-7b.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/trainer/config/llama2-13b.yaml` & `cerebrium-1.3.1/cerebrium/trainer/config/llama2-13b.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/trainer/config/llama2-7b.yaml` & `cerebrium-1.3.1/cerebrium/trainer/config/llama2-7b.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/trainer/config/transformer.yaml` & `cerebrium-1.3.1/cerebrium/trainer/config/transformer.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/trainer/diffuser_tuner.py` & `cerebrium-1.3.1/cerebrium/trainer/diffuser_tuner.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/trainer/fine_tuner.py` & `cerebrium-1.3.1/cerebrium/trainer/fine_tuner.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/trainer/finetune_LLM/finetuning_model.py` & `cerebrium-1.3.1/cerebrium/trainer/finetune_LLM/finetuning_model.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py` & `cerebrium-1.3.1/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py` & `cerebrium-1.3.1/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/cerebrium/utils.py` & `cerebrium-1.3.1/cerebrium/utils.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.0/pyproject.toml` & `cerebrium-1.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cerebrium"
-version = "1.3.0"
+version = "1.3.1"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "EXTERNAL_README.md"
 exclude = ["tests/*", "dist/*", "webhook/*", "builder/*", "prebuilt/*", "common/*", "examples/*", "trainer/*", "README.md"]
 
 [tool.poetry.urls]
```

### Comparing `cerebrium-1.3.0/PKG-INFO` & `cerebrium-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.3.0
+Version: 1.3.1
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

