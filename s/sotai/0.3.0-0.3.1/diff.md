# Comparing `tmp/sotai-0.3.0.tar.gz` & `tmp/sotai-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sotai-0.3.0.tar", last modified: Wed Jul 26 19:16:46 2023, max compression
+gzip compressed data, was "sotai-0.3.1.tar", last modified: Sat Jul 29 00:35:05 2023, max compression
```

## Comparing `sotai-0.3.0.tar` & `sotai-0.3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:16:46.375932 sotai-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-26 19:16:30.000000 sotai-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-26 19:16:46.375932 sotai-0.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:16:46.367932 sotai-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-26 19:16:30.000000 sotai-0.3.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-26 19:16:30.000000 sotai-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 19:16:46.375932 sotai-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:16:46.371932 sotai-0.3.0/sotai/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26335 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:16:46.375932 sotai-0.3.0/sotai/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/layers/categorical_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    17381 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/layers/numerical_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30302 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/trained_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/training.py
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-07-26 19:16:30.000000 sotai-0.3.0/sotai/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:16:46.371932 sotai-0.3.0/sotai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-26 19:16:46.000000 sotai-0.3.0/sotai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-26 19:16:46.000000 sotai-0.3.0/sotai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:16:46.000000 sotai-0.3.0/sotai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-26 19:16:46.000000 sotai-0.3.0/sotai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 19:16:46.000000 sotai-0.3.0/sotai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:16:46.375932 sotai-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    23951 2023-07-26 19:16:30.000000 sotai-0.3.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-26 19:16:30.000000 sotai-0.3.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-26 19:16:30.000000 sotai-0.3.0/tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-07-26 19:16:30.000000 sotai-0.3.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    16865 2023-07-26 19:16:30.000000 sotai-0.3.0/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-26 19:16:30.000000 sotai-0.3.0/tests/test_trained_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:05.398939 sotai-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-29 00:34:51.000000 sotai-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-29 00:35:05.398939 sotai-0.3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:05.394938 sotai-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-29 00:34:51.000000 sotai-0.3.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-29 00:34:51.000000 sotai-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 00:35:05.398939 sotai-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:05.394938 sotai-0.3.1/sotai/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26348 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:05.398939 sotai-0.3.1/sotai/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/layers/categorical_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17381 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/layers/numerical_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30327 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/trained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-07-29 00:34:51.000000 sotai-0.3.1/sotai/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:05.398939 sotai-0.3.1/sotai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-29 00:35:05.000000 sotai-0.3.1/sotai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-29 00:35:05.000000 sotai-0.3.1/sotai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 00:35:05.000000 sotai-0.3.1/sotai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-29 00:35:05.000000 sotai-0.3.1/sotai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 00:35:05.000000 sotai-0.3.1/sotai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:05.398939 sotai-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    23955 2023-07-29 00:34:51.000000 sotai-0.3.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-29 00:34:51.000000 sotai-0.3.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-29 00:34:51.000000 sotai-0.3.1/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-07-29 00:34:51.000000 sotai-0.3.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16954 2023-07-29 00:34:51.000000 sotai-0.3.1/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-29 00:34:51.000000 sotai-0.3.1/tests/test_trained_model.py
```

### Comparing `sotai-0.3.0/LICENSE` & `sotai-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sotai-0.3.0/PKG-INFO` & `sotai-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotai
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python Library For Calibrated Modeling Built With PyTorch
 Author-email: SOTAI <support@sotai.ai>
 Maintainer-email: SOTAI <support@sotai.ai>
 License: MIT
 Project-URL: Source, https://github.com/SOTAI-Labs/sotai
 Project-URL: Documentation, https://github.com/SOTAI-Labs/sotai/tree/main/docs
 Project-URL: Feature Requests, https://github.com/SOTAI-Labs/pytorch-calibrated/issues
```

### Comparing `sotai-0.3.0/docs/README.md` & `sotai-0.3.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `sotai-0.3.0/pyproject.toml` & `sotai-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sotai"
 # This version must always be one version ahead of the current release, so it
 # matches the current state of development, which will always be ahead of the
 # current release. Use Semantic Versioning.
-version = "0.3.0"
+version = "0.3.1"
 description = "A Python Library For Calibrated Modeling Built With PyTorch"
 readme = "docs/README.md"
 license = {text = "MIT"}
 authors = [
   {name = "SOTAI", email = "support@sotai.ai"},
 ]
 maintainers = [
```

### Comparing `sotai-0.3.0/sotai/api.py` & `sotai-0.3.1/sotai/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,18 +173,18 @@
 
     Returns:
         A tuple containing the status of the API call and a dict containing the UUIDs
         of the resources created as well as a link that can be used to view the trained
         model analysis. If unsuccessful, the UUID will be `None`.
 
         Keys:
-            - `trainedModelMetadataUUID`: The UUID of the trained model.
-            - `modelConfigUUID`: The UUID of the model configuration.
-            - `pipelineConfigUUID`: The UUID of the pipeline configuration.
-            - `analysisURL`: The URL of the trained model analysis.
+            - `trained_model_metadata_uuid`: The UUID of the trained model.
+            - `model_config_uuid`: The UUID of the model configuration.
+            - `pipeline_config_uuid`: The UUID of the pipeline configuration.
+            - `analysis_url`: The URL of the trained model analysis.
     """
     training_results = trained_model.training_results
     train_primary_metrics = training_results.train_primary_metric_by_epoch
     val_primary_metrics = training_results.val_primary_metric_by_epoch
     overall_model_results_dict = {
         "epochs": trained_model.training_config.epochs,
         "batch_size": trained_model.training_config.batch_size,
@@ -315,15 +315,15 @@
         )
 
     if response.status_code != 200:
         logging.error("Failed to create inference")
         logging.error(response.json())
         return APIStatus.ERROR, None
 
-    return APIStatus.SUCCESS, response.json()["inferenceConfigUUID"]
+    return APIStatus.SUCCESS, response.json()["inference_config_uuid"]
 
 
 def get_inference_status(
     inference_uuid: str,
 ) -> Tuple[APIStatus, Optional[InferenceConfigStatus]]:
     """Get an inference from the SOTAI API.
 
@@ -473,15 +473,15 @@
     )
 
     if response.status_code != 200:
         logging.error("Failed to run hypertuning")
         logging.error(response.json())
         return APIStatus.ERROR, None
 
-    return APIStatus.SUCCESS, response.json()["trainedModelMetadataUuids"]
+    return APIStatus.SUCCESS, response.json()["trained_model_metadata_uuids"]
 
 
 def _parse_pipeline_config(
     pipeline_config_json: Dict[str, Any], update_dict: Dict[str, Any]
 ) -> PipelineConfig:
     """Parse a pipeline config from the SOTAI API.
```

### Comparing `sotai-0.3.0/sotai/data.py` & `sotai-0.3.1/sotai/data.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.0/sotai/enums.py` & `sotai-0.3.1/sotai/enums.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.0/sotai/features.py` & `sotai-0.3.1/sotai/features.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.0/sotai/layers/categorical_calibrator.py` & `sotai-0.3.1/sotai/layers/categorical_calibrator.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.0/sotai/layers/linear.py` & `sotai-0.3.1/sotai/layers/linear.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.0/sotai/layers/numerical_calibrator.py` & `sotai-0.3.1/sotai/layers/numerical_calibrator.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.0/sotai/models.py` & `sotai-0.3.1/sotai/models.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.0/sotai/pipeline.py` & `sotai-0.3.1/sotai/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,24 +389,24 @@
         analysis_response_status, analysis_results = post_trained_model_analysis(
             pipeline_config_uuid, trained_model
         )
 
         if analysis_response_status == APIStatus.ERROR:
             return None
 
-        trained_model.uuid = analysis_results["trainedModelMetadataUUID"]
+        trained_model.uuid = analysis_results["trained_model_metadata_uuid"]
 
         upload_response = self._upload_model(trained_model)
         if upload_response == APIStatus.ERROR:
             return None
 
         # TODO: update to use response analysisUrl once no longer broken.
         analysis_url = (
             f"{SOTAI_BASE_URL}/pipelines/{self.uuid}"
-            f"/trained-models/{trained_model.uuid}"
+            f"/trained-models/{trained_model.uuid}/overall-model-results"
         )
         trained_model.analysis_url = analysis_url
 
         return analysis_url
 
     def inference(
         self,
```

### Comparing `sotai-0.3.0/sotai/trained_model.py` & `sotai-0.3.1/sotai/trained_model.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.0/sotai/training.py` & `sotai-0.3.1/sotai/training.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.0/sotai/types.py` & `sotai-0.3.1/sotai/types.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.0/sotai.egg-info/PKG-INFO` & `sotai-0.3.1/sotai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotai
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python Library For Calibrated Modeling Built With PyTorch
 Author-email: SOTAI <support@sotai.ai>
 Maintainer-email: SOTAI <support@sotai.ai>
 License: MIT
 Project-URL: Source, https://github.com/SOTAI-Labs/sotai
 Project-URL: Documentation, https://github.com/SOTAI-Labs/sotai/tree/main/docs
 Project-URL: Feature Requests, https://github.com/SOTAI-Labs/pytorch-calibrated/issues
```

### Comparing `sotai-0.3.0/sotai.egg-info/SOURCES.txt` & `sotai-0.3.1/sotai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sotai-0.3.0/tests/test_api.py` & `sotai-0.3.1/tests/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,18 +202,18 @@
 
     assert pipeline_response == "success"
 
 
 @patch("builtins.open")
 @patch(
     "requests.post",
-    return_value=MockResponse({"inferenceConfigUUID": "test_inference_uuid"}),
+    return_value=MockResponse({"inference_config_uuid": "test_inference_uuid"}),
 )
 @patch("sotai.api.get_api_key", return_value="test_api_key")
-def test_post_inferencel(
+def test_post_inference(
     mock_get_api_key,
     mock_post,
     mock_open_data,
 ):
     """Tests that feature configs are posted correctly."""
     mock_open_data.return_value.__enter__.return_value = "data"
     pipeline_response = post_inference("/tmp/model", "test_uuid")
@@ -299,15 +299,15 @@
     assert pipeline_response[1] == "test_dataset_uuid"
     assert pipeline_response[0] == "success"
 
 
 @patch(
     "requests.post",
     return_value=MockResponse(
-        {"trainedModelMetadataUuids": ["test_uuid_1", "test_uuid_2"]}
+        {"trained_model_metadata_uuids": ["test_uuid_1", "test_uuid_2"]}
     ),
 )
 @patch("sotai.api.get_api_key", return_value="test_api_key")
 def test_post_hypertune(mock_get_api_key, mock_post, fixture_pipeline_config):
     """Tests that a trained model is posted correctly."""
 
     hypertune_config = HypertuneConfig(
```

### Comparing `sotai-0.3.0/tests/test_data.py` & `sotai-0.3.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.0/tests/test_features.py` & `sotai-0.3.1/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.0/tests/test_models.py` & `sotai-0.3.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.0/tests/test_pipeline.py` & `sotai-0.3.1/tests/test_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,15 @@
 
 
 @patch("sotai.pipeline.Pipeline._upload_model", return_value=APIStatus.SUCCESS)
 @patch(
     "sotai.pipeline.post_trained_model_analysis",
     return_value=(
         APIStatus.SUCCESS,
-        {"trainedModelMetadataUUID": "test_uuid"},
+        {"trained_model_metadata_uuid": "test_uuid"},
     ),
 )
 @patch("sotai.pipeline.post_pipeline_feature_configs", return_value=APIStatus.SUCCESS)
 @patch(
     "sotai.pipeline.post_pipeline_config",
     return_value=(APIStatus.SUCCESS, "test_pipeline_config_id"),
 )
@@ -297,18 +297,19 @@
     )
     post_pipeline_feature_configs.assert_called_once_with(
         "test_pipeline_config_id", trained_model.pipeline_config.feature_configs
     )
     post_trained_model_analysis.assert_called_once_with(
         "test_pipeline_config_id", trained_model
     )
-    assert (
-        analysis_response
-        == f"{SOTAI_BASE_URL}/pipelines/test_pipeline_id/trained-models/test_uuid"
+    expected_analysis_response = (
+        f"{SOTAI_BASE_URL}/pipelines/test_pipeline_id/"
+        f"trained-models/test_uuid/overall-model-results"
     )
+    assert analysis_response == expected_analysis_response
 
 
 @patch(
     "sotai.pipeline.post_inference",
     return_value=(APIStatus.SUCCESS, "test_inference_uuid"),
 )
 @patch("sotai.pipeline.get_api_key", return_value="test_api_key")
```

### Comparing `sotai-0.3.0/tests/test_trained_model.py` & `sotai-0.3.1/tests/test_trained_model.py`

 * *Files identical despite different names*

