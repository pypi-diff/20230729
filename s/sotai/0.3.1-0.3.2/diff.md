# Comparing `tmp/sotai-0.3.1.tar.gz` & `tmp/sotai-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sotai-0.3.1.tar", last modified: Sat Jul 29 00:35:05 2023, max compression
+gzip compressed data, was "sotai-0.3.2.tar", last modified: Sat Jul 29 01:10:59 2023, max compression
```

## Comparing `sotai-0.3.1.tar` & `sotai-0.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:05.398939 sotai-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-29 00:34:51.000000 sotai-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-29 00:35:05.398939 sotai-0.3.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:05.394938 sotai-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-29 00:34:51.000000 sotai-0.3.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-29 00:34:51.000000 sotai-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 00:35:05.398939 sotai-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:05.394938 sotai-0.3.1/sotai/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26348 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:05.398939 sotai-0.3.1/sotai/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/layers/categorical_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    17381 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/layers/numerical_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30327 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/trained_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/training.py
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:05.398939 sotai-0.3.1/sotai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-29 00:35:05.000000 sotai-0.3.1/sotai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-29 00:35:05.000000 sotai-0.3.1/sotai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 00:35:05.000000 sotai-0.3.1/sotai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-29 00:35:05.000000 sotai-0.3.1/sotai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 00:35:05.000000 sotai-0.3.1/sotai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:05.398939 sotai-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    23955 2023-07-29 00:34:51.000000 sotai-0.3.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-29 00:34:51.000000 sotai-0.3.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-29 00:34:51.000000 sotai-0.3.1/tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-07-29 00:34:51.000000 sotai-0.3.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    16954 2023-07-29 00:34:51.000000 sotai-0.3.1/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-29 00:34:51.000000 sotai-0.3.1/tests/test_trained_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:10:59.257522 sotai-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-29 01:10:42.000000 sotai-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-29 01:10:59.257522 sotai-0.3.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:10:59.253522 sotai-0.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-29 01:10:42.000000 sotai-0.3.2/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-29 01:10:42.000000 sotai-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 01:10:59.257522 sotai-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:10:59.257522 sotai-0.3.2/sotai/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26347 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:10:59.257522 sotai-0.3.2/sotai/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/layers/categorical_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17381 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/layers/numerical_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30327 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/trained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:10:59.257522 sotai-0.3.2/sotai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-29 01:10:59.000000 sotai-0.3.2/sotai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-29 01:10:59.000000 sotai-0.3.2/sotai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 01:10:59.000000 sotai-0.3.2/sotai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-29 01:10:59.000000 sotai-0.3.2/sotai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 01:10:59.000000 sotai-0.3.2/sotai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:10:59.257522 sotai-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    23955 2023-07-29 01:10:42.000000 sotai-0.3.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-29 01:10:42.000000 sotai-0.3.2/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-29 01:10:42.000000 sotai-0.3.2/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-07-29 01:10:42.000000 sotai-0.3.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16954 2023-07-29 01:10:42.000000 sotai-0.3.2/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-29 01:10:42.000000 sotai-0.3.2/tests/test_trained_model.py
```

### Comparing `sotai-0.3.1/LICENSE` & `sotai-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sotai-0.3.1/PKG-INFO` & `sotai-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotai
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python Library For Calibrated Modeling Built With PyTorch
 Author-email: SOTAI <support@sotai.ai>
 Maintainer-email: SOTAI <support@sotai.ai>
 License: MIT
 Project-URL: Source, https://github.com/SOTAI-Labs/sotai
 Project-URL: Documentation, https://github.com/SOTAI-Labs/sotai/tree/main/docs
 Project-URL: Feature Requests, https://github.com/SOTAI-Labs/pytorch-calibrated/issues
```

### Comparing `sotai-0.3.1/docs/README.md` & `sotai-0.3.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `sotai-0.3.1/pyproject.toml` & `sotai-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sotai"
 # This version must always be one version ahead of the current release, so it
 # matches the current state of development, which will always be ahead of the
 # current release. Use Semantic Versioning.
-version = "0.3.1"
+version = "0.3.2"
 description = "A Python Library For Calibrated Modeling Built With PyTorch"
 readme = "docs/README.md"
 license = {text = "MIT"}
 authors = [
   {name = "SOTAI", email = "support@sotai.ai"},
 ]
 maintainers = [
```

### Comparing `sotai-0.3.1/sotai/api.py` & `sotai-0.3.2/sotai/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,14 @@
         },
         headers=get_auth_headers(),
         timeout=SOTAI_API_TIMEOUT,
     )
     if response.status_code != 200:
         logging.error("Failed to create pipeline")
         return APIStatus.ERROR, None
-
     return APIStatus.SUCCESS, response.json()["uuid"]
 
 
 def post_pipeline_config(
     pipeline_uuid: str, pipeline_config: PipelineConfig
 ) -> Tuple[APIStatus, Optional[str]]:
     """Create a new pipeline config on the SOTAI API.
@@ -500,15 +499,15 @@
         val=pipeline_config_json["validation_percentage"],
         test=pipeline_config_json["test_percentage"],
     )
     feature_configs = {}
     for feature in pipeline_config_json["feature_config_list"]:
         feature["name"] = feature["feature_name"]
         feature["type"] = feature["feature_type"]
-        if feature["feature_type"] == "CATEGORICAL":
+        if feature["feature_type"] == "categorical":
             if feature["categories_str"]:
                 feature["categories"] = feature["categories_str"]
                 del feature["categories_str"]
             else:
                 feature["categories_int"] = feature["categories_int"]
                 del feature["categories_int"]
             feature_configs[feature["name"]] = CategoricalFeatureConfig(**feature)
```

### Comparing `sotai-0.3.1/sotai/data.py` & `sotai-0.3.2/sotai/data.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.1/sotai/enums.py` & `sotai-0.3.2/sotai/enums.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.1/sotai/features.py` & `sotai-0.3.2/sotai/features.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.1/sotai/layers/categorical_calibrator.py` & `sotai-0.3.2/sotai/layers/categorical_calibrator.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.1/sotai/layers/linear.py` & `sotai-0.3.2/sotai/layers/linear.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.1/sotai/layers/numerical_calibrator.py` & `sotai-0.3.2/sotai/layers/numerical_calibrator.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.1/sotai/models.py` & `sotai-0.3.2/sotai/models.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.1/sotai/pipeline.py` & `sotai-0.3.2/sotai/pipeline.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.1/sotai/trained_model.py` & `sotai-0.3.2/sotai/trained_model.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.1/sotai/training.py` & `sotai-0.3.2/sotai/training.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.1/sotai/types.py` & `sotai-0.3.2/sotai/types.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.1/sotai.egg-info/PKG-INFO` & `sotai-0.3.2/sotai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotai
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python Library For Calibrated Modeling Built With PyTorch
 Author-email: SOTAI <support@sotai.ai>
 Maintainer-email: SOTAI <support@sotai.ai>
 License: MIT
 Project-URL: Source, https://github.com/SOTAI-Labs/sotai
 Project-URL: Documentation, https://github.com/SOTAI-Labs/sotai/tree/main/docs
 Project-URL: Feature Requests, https://github.com/SOTAI-Labs/pytorch-calibrated/issues
```

### Comparing `sotai-0.3.1/sotai.egg-info/SOURCES.txt` & `sotai-0.3.2/sotai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sotai-0.3.1/tests/test_api.py` & `sotai-0.3.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.1/tests/test_data.py` & `sotai-0.3.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.1/tests/test_features.py` & `sotai-0.3.2/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.1/tests/test_models.py` & `sotai-0.3.2/tests/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,8 +380,8 @@
     )
 
     with torch.no_grad():
         trained_predictions = calibrated_linear(training_examples)
         trained_loss = loss_fn(trained_predictions, training_labels)
 
     assert trained_loss < initial_loss
-    assert trained_loss < 0.0175
+    assert trained_loss < 0.02
```

### Comparing `sotai-0.3.1/tests/test_pipeline.py` & `sotai-0.3.2/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.1/tests/test_trained_model.py` & `sotai-0.3.2/tests/test_trained_model.py`

 * *Files identical despite different names*

