# Comparing `tmp/payload-validator-0.1.7.tar.gz` & `tmp/payload-validator-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\payload-validator-0.1.7.tar", last modified: Tue Jul 25 15:12:26 2023, max compression
+gzip compressed data, was "dist\payload-validator-0.1.8.tar", last modified: Sat Jul 29 13:43:29 2023, max compression
```

## Comparing `payload-validator-0.1.7.tar` & `payload-validator-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 15:12:26.000000 payload-validator-0.1.7/
--rw-rw-rw-   0        0        0     1069 2023-07-23 05:40:32.000000 payload-validator-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       74 2023-07-23 05:40:32.000000 payload-validator-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0    12476 2023-07-25 15:12:26.000000 payload-validator-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0    11599 2023-07-23 09:56:08.000000 payload-validator-0.1.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-25 15:12:26.000000 payload-validator-0.1.7/payload_validator/
--rw-rw-rw-   0        0        0        0 2023-07-23 05:40:32.000000 payload-validator-0.1.7/payload_validator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 15:12:26.000000 payload-validator-0.1.7/payload_validator/__pycache__/
--rw-rw-rw-   0        0        0      160 2023-07-23 16:52:28.000000 payload-validator-0.1.7/payload_validator/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     1622 2023-07-23 16:52:28.000000 payload-validator-0.1.7/payload_validator/__pycache__/exceptions.cpython-37.pyc
--rw-rw-rw-   0        0        0     6463 2023-07-25 14:47:02.000000 payload-validator-0.1.7/payload_validator/__pycache__/validators.cpython-37.pyc
--rw-rw-rw-   0        0        0      958 2023-07-23 06:25:16.000000 payload-validator-0.1.7/payload_validator/exceptions.py
--rw-rw-rw-   0        0        0     6080 2023-07-25 15:10:13.000000 payload-validator-0.1.7/payload_validator/validators.py
-drwxrwxrwx   0        0        0        0 2023-07-25 15:12:26.000000 payload-validator-0.1.7/payload_validator.egg-info/
--rw-rw-rw-   0        0        0    12476 2023-07-25 15:12:26.000000 payload-validator-0.1.7/payload_validator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      541 2023-07-25 15:12:26.000000 payload-validator-0.1.7/payload_validator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 15:12:26.000000 payload-validator-0.1.7/payload_validator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-25 15:12:26.000000 payload-validator-0.1.7/payload_validator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      893 2023-07-25 15:12:26.000000 payload-validator-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0       68 2023-07-23 05:40:32.000000 payload-validator-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 15:12:26.000000 payload-validator-0.1.7/tests/
--rw-rw-rw-   0        0        0        0 2023-07-23 05:40:32.000000 payload-validator-0.1.7/tests/__init__.py
--rw-rw-rw-   0        0        0     2960 2023-07-23 05:40:32.000000 payload-validator-0.1.7/tests/test_exceptions.py
--rw-rw-rw-   0        0        0    38040 2023-07-25 15:10:13.000000 payload-validator-0.1.7/tests/test_validators.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:43:29.000000 payload-validator-0.1.8/
+-rw-rw-rw-   0        0        0     1069 2023-07-23 05:40:32.000000 payload-validator-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0       74 2023-07-23 05:40:32.000000 payload-validator-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    12476 2023-07-29 13:43:29.000000 payload-validator-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    11599 2023-07-23 09:56:08.000000 payload-validator-0.1.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-29 13:43:28.000000 payload-validator-0.1.8/payload_validator/
+-rw-rw-rw-   0        0        0        0 2023-07-23 05:40:32.000000 payload-validator-0.1.8/payload_validator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:43:29.000000 payload-validator-0.1.8/payload_validator/__pycache__/
+-rw-rw-rw-   0        0        0      160 2023-07-23 16:52:28.000000 payload-validator-0.1.8/payload_validator/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2775 2023-07-29 13:37:23.000000 payload-validator-0.1.8/payload_validator/__pycache__/comparisons.cpython-37.pyc
+-rw-rw-rw-   0        0        0      937 2023-07-29 13:37:23.000000 payload-validator-0.1.8/payload_validator/__pycache__/error_contexts.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1622 2023-07-23 16:52:28.000000 payload-validator-0.1.8/payload_validator/__pycache__/exceptions.cpython-37.pyc
+-rw-rw-rw-   0        0        0     5364 2023-07-29 13:37:23.000000 payload-validator-0.1.8/payload_validator/__pycache__/validators.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2101 2023-07-29 13:43:02.000000 payload-validator-0.1.8/payload_validator/comparisons.py
+-rw-rw-rw-   0        0        0      369 2023-07-29 13:43:02.000000 payload-validator-0.1.8/payload_validator/error_contexts.py
+-rw-rw-rw-   0        0        0      958 2023-07-23 06:25:16.000000 payload-validator-0.1.8/payload_validator/exceptions.py
+-rw-rw-rw-   0        0        0     5562 2023-07-29 13:43:02.000000 payload-validator-0.1.8/payload_validator/validators.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:43:28.000000 payload-validator-0.1.8/payload_validator.egg-info/
+-rw-rw-rw-   0        0        0    12476 2023-07-29 13:43:28.000000 payload-validator-0.1.8/payload_validator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      782 2023-07-29 13:43:28.000000 payload-validator-0.1.8/payload_validator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 13:43:28.000000 payload-validator-0.1.8/payload_validator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-29 13:43:28.000000 payload-validator-0.1.8/payload_validator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      893 2023-07-29 13:43:29.000000 payload-validator-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0       68 2023-07-23 05:40:32.000000 payload-validator-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:43:29.000000 payload-validator-0.1.8/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-23 05:40:32.000000 payload-validator-0.1.8/tests/__init__.py
+-rw-rw-rw-   0        0        0     3069 2023-07-29 13:43:02.000000 payload-validator-0.1.8/tests/test_comparisons.py
+-rw-rw-rw-   0        0        0     1451 2023-07-29 13:43:02.000000 payload-validator-0.1.8/tests/test_error_contexts.py
+-rw-rw-rw-   0        0        0     2960 2023-07-23 05:40:32.000000 payload-validator-0.1.8/tests/test_exceptions.py
+-rw-rw-rw-   0        0        0    28911 2023-07-29 13:43:02.000000 payload-validator-0.1.8/tests/test_validators.py
```

### Comparing `payload-validator-0.1.7/LICENSE` & `payload-validator-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `payload-validator-0.1.7/PKG-INFO` & `payload-validator-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payload-validator
-Version: 0.1.7
+Version: 0.1.8
 Summary: Validating payload datas for Python
 Home-page: https://github.com/cwadven/payload-validator
 Author: cwadven
 Author-email: cwadven4@gmail.com
 Maintainer: cwadven
 License: MIT
 Keywords: input,payload,validator,validate,validation,data,datas,python,python3,python3.6,python3.7,python3.8
```

### Comparing `payload-validator-0.1.7/README.rst` & `payload-validator-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `payload-validator-0.1.7/payload_validator/__pycache__/exceptions.cpython-37.pyc` & `payload-validator-0.1.8/payload_validator/__pycache__/exceptions.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `payload-validator-0.1.7/payload_validator/exceptions.py` & `payload-validator-0.1.8/payload_validator/exceptions.py`

 * *Files identical despite different names*

### Comparing `payload-validator-0.1.7/payload_validator/validators.py` & `payload-validator-0.1.8/payload_validator/validators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,73 @@
-import re
-import traceback
-from abc import (
-    ABC,
-    abstractmethod,
-)
-from itertools import chain
 from types import FunctionType
 from typing import (
     Callable,
+    Dict,
     Iterable,
+    List,
     Optional,
     TypeVar,
     Union,
 )
 
+from payload_validator.comparisons import PayloadComparison
+from payload_validator.error_contexts import (
+    NormalValidatorErrorContext,
+    ValidatorErrorContext,
+)
 from payload_validator.exceptions import (
     InvalidValueError,
     MismatchedErrorKeysException,
     ValidationException,
     ValidationNotRunException,
 )
 
 
 T = TypeVar("T")  # Use TypeVar for arbitrary object types
 
 
-class ValidatorErrorContext(ABC, dict):
-    @abstractmethod
-    def add_error(self, field: str, error: str):
-        pass
-
-
-class NormalValidatorErrorContext(ValidatorErrorContext):
-    def add_error(self, field: str, error: str):
-        value = self.setdefault(field, [])
-        value.append(error)
-
-
 class PayloadValidator(object):
     DEFAULT_MANDATORY_ERROR_MESSAGE = "mandatory data missing"
 
     def __init__(self, payload: dict, error_context: ValidatorErrorContext = None) -> None:
-        self.payload = payload
-        self._skip_validate_keys = set()
-        self._validate_called = False
-        self._error_context = (
+        self.payload: dict = payload
+        self._cache_payload_comparisons: dict = {}
+
+        self.skip_validate_keys: set = set()
+
+        self._error_context: ValidatorErrorContext = (
             error_context
             if error_context is not None
             else NormalValidatorErrorContext()
         )
 
-        self.mandatory_keys = getattr(self._get_meta_attribute(), "mandatory_keys", {})
-        self.type_of_keys = getattr(self._get_meta_attribute(), "type_of_keys", {})
+        self.mandatory_keys: Dict[str, str] = getattr(self._get_meta_attribute(), "mandatory_keys", {})
+        self.type_of_keys: Dict[str, List] = getattr(self._get_meta_attribute(), "type_of_keys", {})
+
+        self._validate_called: bool = False
+
+    def get_payload(self, key: str) -> PayloadComparison:
+        if key not in self._cache_payload_comparisons:
+            self._cache_payload_comparisons[key] = PayloadComparison(self, key)
+        return self._cache_payload_comparisons[key]
 
     def add_error_context(self, key: str, errors: Union[str, Iterable]) -> None:
-        if key not in self._skip_validate_keys:
+        if key not in self.skip_validate_keys:
             if isinstance(errors, str):
                 self._error_context.add_error(key, errors)
             else:
                 for error in errors:
                     self._error_context.add_error(key, error)
 
     def add_error_and_skip_validation_key(self, key: str, errors: Union[str, Iterable]) -> None:
         """
         add only main error so other errors cannot add
         """
         self.add_error_context(key, errors)
-        self._skip_validate_keys.add(key)
+        self.skip_validate_keys.add(key)
 
     def _get_meta_attribute(self) -> Optional[T]:
         return getattr(self, "Meta", None)
 
     def _validate_mandatory_payloads(self) -> None:
         """
         mandatory_keys example:
@@ -106,32 +103,21 @@
     def _handle_invalid_value_error_exception(self, e: InvalidValueError) -> None:
         for key, value in e.error_value_by_key.items():
             if key in e.add_skip_validation_keys:
                 self.add_error_and_skip_validation_key(key, value)
             else:
                 self.add_error_context(key, value)
 
-    def _handle_skip_validation_key_payload_exception(self, e: Exception) -> None:
-        tb = traceback.extract_tb(e.__traceback__)
-        pattern = r"self\.payload(?:\.get\('([^']*)'\)|\['([^']*)'\]|(?:\[\"|\'|)([^\"\']*)(?:\"|\'|)\])"
-        for key in [match for match in chain(*re.findall(pattern, tb[-1].line)) if match]:
-            if key in self._skip_validate_keys:
-                pass
-            else:
-                raise e
-
     def _common_validate(self) -> None:
         try:
             self.common_validate()
         except MismatchedErrorKeysException as e:
             raise e
         except InvalidValueError as e:
             self._handle_invalid_value_error_exception(e)
-        except Exception as e:
-            self._handle_skip_validation_key_payload_exception(e)
 
     def common_validate(self) -> None:
         """
         override this method to add custom validation
         """
         pass
 
@@ -140,16 +126,14 @@
             if type(y) == FunctionType and x.startswith("validate"):
                 try:
                     y(self)
                 except MismatchedErrorKeysException as e:
                     raise e
                 except InvalidValueError as e:
                     self._handle_invalid_value_error_exception(e)
-                except Exception as e:
-                    self._handle_skip_validation_key_payload_exception(e)
 
     def validate(self) -> None:
         if not self._validate_called:
             self._validate_mandatory_payloads()
             self._validate_payloads_type()
             self._validate_methods()
             self._common_validate()
```

### Comparing `payload-validator-0.1.7/payload_validator.egg-info/PKG-INFO` & `payload-validator-0.1.8/payload_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payload-validator
-Version: 0.1.7
+Version: 0.1.8
 Summary: Validating payload datas for Python
 Home-page: https://github.com/cwadven/payload-validator
 Author: cwadven
 Author-email: cwadven4@gmail.com
 Maintainer: cwadven
 License: MIT
 Keywords: input,payload,validator,validate,validation,data,datas,python,python3,python3.6,python3.7,python3.8
```

### Comparing `payload-validator-0.1.7/payload_validator.egg-info/SOURCES.txt` & `payload-validator-0.1.8/payload_validator.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 payload_validator/__init__.py
+payload_validator/comparisons.py
+payload_validator/error_contexts.py
 payload_validator/exceptions.py
 payload_validator/validators.py
 payload_validator.egg-info/PKG-INFO
 payload_validator.egg-info/SOURCES.txt
 payload_validator.egg-info/dependency_links.txt
 payload_validator.egg-info/top_level.txt
 payload_validator/__pycache__/__init__.cpython-37.pyc
+payload_validator/__pycache__/comparisons.cpython-37.pyc
+payload_validator/__pycache__/error_contexts.cpython-37.pyc
 payload_validator/__pycache__/exceptions.cpython-37.pyc
 payload_validator/__pycache__/validators.cpython-37.pyc
 tests/__init__.py
+tests/test_comparisons.py
+tests/test_error_contexts.py
 tests/test_exceptions.py
 tests/test_validators.py
```

### Comparing `payload-validator-0.1.7/setup.cfg` & `payload-validator-0.1.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6179 6c6f 6164 2d76 616c 6964   = payload-valid
 00000020: 6174 6f72 0d0a 7665 7273 696f 6e20 3d20  ator..version = 
-00000030: 302e 312e 370d 0a61 7574 686f 7220 3d20  0.1.7..author = 
+00000030: 302e 312e 380d 0a61 7574 686f 7220 3d20  0.1.8..author = 
 00000040: 6377 6164 7665 6e0d 0a61 7574 686f 725f  cwadven..author_
 00000050: 656d 6169 6c20 3d20 6377 6164 7665 6e34  email = cwadven4
 00000060: 4067 6d61 696c 2e63 6f6d 0d0a 6d61 696e  @gmail.com..main
 00000070: 7461 696e 6572 203d 2063 7761 6476 656e  tainer = cwadven
 00000080: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000090: 5661 6c69 6461 7469 6e67 2070 6179 6c6f  Validating paylo
 000000a0: 6164 2064 6174 6173 2066 6f72 2050 7974  ad datas for Pyt
```

### Comparing `payload-validator-0.1.7/tests/test_exceptions.py` & `payload-validator-0.1.8/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `payload-validator-0.1.7/tests/test_validators.py` & `payload-validator-0.1.8/tests/test_validators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import unittest
 from unittest.mock import patch
 
+from payload_validator.comparisons import PayloadComparison
 from payload_validator.exceptions import (
     InvalidValueError,
     MismatchedErrorKeysException,
     ValidationException,
     ValidationNotRunException,
 )
 from payload_validator.validators import (
@@ -202,21 +203,21 @@
         with self.assertRaises(ValidationException):
             validator = MandatoryAndTypeValidPayloadValidator(fail_payload)
             validator.validate()
 
         # Then: 4 keys should be in error context
         self.assertEqual(validator._validate_called, True)
         self.assertEqual(len(validator.error_context), 4)
-        # And: if mandatory key is missing, error message should be only mandatory due to _skip_validate_keys
-        self.assertIn("displayable", validator._skip_validate_keys)
+        # And: if mandatory key is missing, error message should be only mandatory due to skip_validate_keys
+        self.assertIn("displayable", validator.skip_validate_keys)
         self.assertEqual(
             validator.error_context["displayable"],
             [MandatoryAndTypeValidPayloadValidator.Meta.mandatory_keys["displayable"]],
         )
-        self.assertIn("count", validator._skip_validate_keys)
+        self.assertIn("count", validator.skip_validate_keys)
         self.assertEqual(
             validator.error_context["count"],
             [MandatoryAndTypeValidPayloadValidator.DEFAULT_MANDATORY_ERROR_MESSAGE],
         )
         self.assertEqual(
             validator.error_context["amount"],
             [MandatoryAndTypeValidPayloadValidator.Meta.type_of_keys["amount"][1]],
@@ -559,15 +560,15 @@
 
         with self.assertRaises(ValidationException):
             validator = CustomValidator(payload)
             validator.validate()
 
         # Then:
         self.assertEqual(validator._validate_called, True)
-        self.assertIn("start_date", validator._skip_validate_keys)
+        self.assertIn("start_date", validator.skip_validate_keys)
         self.assertEqual(len(validator.error_context), 1)
         # And: Due to add_skip_validation_keys, validate_start_date1 error is not exists
         self.assertEqual(
             validator.error_context["start_date"],
             ["start_date error1"],
         )
 
@@ -601,15 +602,15 @@
 
         with self.assertRaises(ValidationException):
             validator = CustomValidator(payload)
             validator.validate()
 
         # Then:
         self.assertEqual(validator._validate_called, True)
-        self.assertIn("start_date", validator._skip_validate_keys)
+        self.assertIn("start_date", validator.skip_validate_keys)
         self.assertEqual(len(validator.error_context), 1)
         self.assertEqual(
             validator.error_context["start_date"],
             ["start_date error"],
         )
 
     def test_add_error_context_method_should_return_error_context(self):
@@ -644,15 +645,15 @@
 
         with self.assertRaises(ValidationException):
             validator = CustomValidator(payload)
             validator.validate()
 
         # Then:
         self.assertEqual(validator._validate_called, True)
-        self.assertIn("start_date", validator._skip_validate_keys)
+        self.assertIn("start_date", validator.skip_validate_keys)
         self.assertEqual(len(validator.error_context), 1)
         # And: Due to add_skip_validation_keys error is not exists
         self.assertEqual(
             validator.error_context["start_date"],
             ["start_date error1"],
         )
 
@@ -673,239 +674,44 @@
         # When:
         validator._handle_invalid_value_error_exception(InvalidValueError({"displayable": "displayable error"}))
 
         # Then:
         self.assertEqual(len(validator._error_context), 1)
         self.assertEqual(validator._error_context["displayable"], ["displayable error"])
         # And: Due to add_skip_validation_keys error is not exists
-        self.assertNotIn("displayable", validator._skip_validate_keys)
+        self.assertNotIn("displayable", validator.skip_validate_keys)
 
-    def test_handle_invalid_value_error_exception_when_add_skip_validation_keys_exists(self):
+    def test_get_payload(self):
         # Given:
         payload = {"displayable": "example"}
         validator = PayloadValidator(payload)
 
         # When:
-        validator._handle_invalid_value_error_exception(
-            InvalidValueError({"displayable": "displayable error"}, ["displayable"])
-        )
-
-        # Then:
-        self.assertEqual(len(validator._error_context), 1)
-        self.assertEqual(validator._error_context["displayable"], ["displayable error"])
-        # And: Due to add_skip_validation_keys error is exists
-        self.assertIn("displayable", validator._skip_validate_keys)
-
-    @patch("payload_validator.validators.PayloadValidator._handle_skip_validation_key_payload_exception")
-    def test_handle_skip_validation_key_payload_in_payload_key_not_exists_common_validate_exception(self, mock_handle_skip_validation_key_payload_exception):
-        # Given: common_validate method validation
-        class CustomValidator(PayloadValidator):
-            def common_validate(self):
-                if self.payload["start_date"] > 1:
-                    pass
-        # And: Add payload start_date key not exists
-        custom_validator = CustomValidator({})
-        custom_validator.add_error_and_skip_validation_key("start_date", "start_date is required")
-        # And: Set _validate_called to True
-        custom_validator._validate_called = True
-
-        # When:
-        custom_validator._common_validate()
-
-        # Then:
-        mock_handle_skip_validation_key_payload_exception.assert_called_once()
-        self.assertEqual(custom_validator.error_context["start_date"], ["start_date is required"])
-
-    def test_handle_skip_validation_key_payload_in_payload_key_not_exists_common_validate_exception_should_pass(self):
-        # Given: common_validate method validation
-        class CustomValidator(PayloadValidator):
-            def common_validate(self):
-                if self.payload["start_date"] > 1:
-                    pass
-
-        # And: Add payload start_date key not exists
-        custom_validator = CustomValidator({})
-        custom_validator.add_error_and_skip_validation_key("start_date", "start_date is required")
-        # And: Set _validate_called to True
-        custom_validator._validate_called = True
-
-        # When:
-        custom_validator._common_validate()
-
-        # Then:
-        self.assertEqual(custom_validator.error_context["start_date"], ["start_date is required"])
-
-    def test_handle_skip_validation_key_payload_in_payload_key_not_exists_common_validate_exception_should_not_pass(self):
-        # Given: common_validate method validation
-        class CustomValidator(PayloadValidator):
-            def common_validate(self):
-                if self.payload["start_date"] > 1:
-                    pass
-
-        # And: Add payload start_date key not exists
-        custom_validator = CustomValidator({})
-
-        # Expected:
-        with self.assertRaises(KeyError):
-            custom_validator._common_validate()
-
-    @patch("payload_validator.validators.PayloadValidator._handle_skip_validation_key_payload_exception")
-    def test_handle_skip_validation_key_payload_in_payload_key_type_invalid_common_validate_exception(self, mock_handle_skip_validation_key_payload_exception):
-        # Given: common_validate method validation
-        class CustomValidator(PayloadValidator):
-            def common_validate(self):
-                if self.payload["start_date"] > 1:
-                    pass
-
-        # And: Add payload start_date is String
-        custom_validator = CustomValidator({"start_date": "String"})
-        custom_validator.add_error_and_skip_validation_key("start_date", "type should be integer")
-        # And: Set _validate_called to True
-        custom_validator._validate_called = True
-
-        # When:
-        custom_validator._common_validate()
-
-        # Then:
-        mock_handle_skip_validation_key_payload_exception.assert_called_once()
-        self.assertEqual(custom_validator.error_context["start_date"], ["type should be integer"])
-
-    def test_handle_skip_validation_key_payload_in_payload_key_type_invalid_common_validate_exception_should_pass(self):
-        # Given: common_validate method validation
-        class CustomValidator(PayloadValidator):
-            def common_validate(self):
-                if self.payload["start_date"] > 1:
-                    pass
-
-        # And: Add payload start_date is String
-        custom_validator = CustomValidator({"start_date": "String"})
-        custom_validator.add_error_and_skip_validation_key("start_date", "type should be integer")
-        # And: Set _validate_called to True
-        custom_validator._validate_called = True
-
-        # When:
-        custom_validator._common_validate()
-
-        # Then:
-        self.assertEqual(custom_validator.error_context["start_date"], ["type should be integer"])
-
-    def test_handle_skip_validation_key_payload_in_payload_key_type_invalid_common_validate_exception_should_not_pass(self):
-        # Given: common_validate method validation
-        class CustomValidator(PayloadValidator):
-            def common_validate(self):
-                if self.payload["start_date"] > 1:
-                    pass
-
-        # And: Add payload start_date is String
-        custom_validator = CustomValidator({"start_date": "String"})
-
-        # Expected:
-        with self.assertRaises(TypeError):
-            custom_validator._common_validate()
-
-    @patch("payload_validator.validators.PayloadValidator._handle_skip_validation_key_payload_exception")
-    def test_handle_skip_validation_key_payload_in_payload_key_not_exists_validate_method_exception(self, mock_handle_skip_validation_key_payload_exception):
-        # Given: validate method validation
-        class CustomValidator(PayloadValidator):
-            def validate_start_date(self):
-                if self.payload["start_date"] > 1:
-                    pass
-
-        # And: Add payload start_date key not exists
-        custom_validator = CustomValidator({})
-        custom_validator.add_error_and_skip_validation_key("start_date", "start_date is required")
-        # And: Set _validate_called to True
-        custom_validator._validate_called = True
-
-        # When:
-        custom_validator._validate_methods()
+        comparison_displayable = validator.get_payload("displayable")
 
         # Then:
-        mock_handle_skip_validation_key_payload_exception.assert_called_once()
-        self.assertEqual(custom_validator.error_context["start_date"], ["start_date is required"])
-
-    def test_handle_skip_validation_key_payload_in_payload_key_not_exists_validate_method_should_pass(self):
-        # Given: validate method validation
-        class CustomValidator(PayloadValidator):
-            def validate_start_date(self):
-                if self.payload["start_date"] > 1:
-                    pass
-
-        # And: Add payload start_date key not exists
-        custom_validator = CustomValidator({})
-        custom_validator.add_error_and_skip_validation_key("start_date", "start_date is required")
-        # And: Set _validate_called to True
-        custom_validator._validate_called = True
-
-        # When:
-        custom_validator._validate_methods()
-
-        # Then:
-        self.assertEqual(custom_validator.error_context["start_date"], ["start_date is required"])
-
-    def test_handle_skip_validation_key_payload_in_payload_key_not_exists_validate_method_should_not_pass(self):
-        # Given: validate method validation
-        class CustomValidator(PayloadValidator):
-            def validate_start_date(self):
-                if self.payload["start_date"] > 1:
-                    pass
+        self.assertIsInstance(comparison_displayable, PayloadComparison)
 
-        # And: Add payload start_date key not exists
-        custom_validator = CustomValidator({})
-
-        # Expected:
-        with self.assertRaises(KeyError):
-            custom_validator._validate_methods()
-
-    @patch("payload_validator.validators.PayloadValidator._handle_skip_validation_key_payload_exception")
-    def test_handle_skip_validation_key_payload_in_payload_key_type_invalid_validate_method_exception(self, mock_handle_skip_validation_key_payload_exception):
-        # Given: validate method validation
-        class CustomValidator(PayloadValidator):
-            def validate_start_date(self):
-                if self.payload["start_date"] > 1:
-                    pass
-
-        # And: Add payload start_date is String
-        custom_validator = CustomValidator({"start_date": "String"})
-        custom_validator.add_error_and_skip_validation_key("start_date", "type should be integer")
-        # And: Set _validate_called to True
-        custom_validator._validate_called = True
+    def test_get_payload_when_cached(self):
+        # Given:
+        payload = {"displayable": "example"}
+        validator = PayloadValidator(payload)
+        # And: not cached
+        self.assertEqual(validator._cache_payload_comparisons, {})
 
         # When:
-        custom_validator._validate_methods()
-
-        # Then:
-        mock_handle_skip_validation_key_payload_exception.assert_called_once()
-        self.assertEqual(custom_validator.error_context["start_date"], ["type should be integer"])
+        comparison_displayable = validator.get_payload("displayable")
 
-    def test_handle_skip_validation_key_payload_in_payload_key_type_invalid_validate_method_exception_should_pass(self):
-        # Given: validate method validation
-        class CustomValidator(PayloadValidator):
-            def validate_start_date(self):
-                if self.payload["start_date"] > 1:
-                    pass
+        # Then: cached
+        self.assertIsInstance(comparison_displayable, PayloadComparison)
+        self.assertEqual(validator._cache_payload_comparisons["displayable"], comparison_displayable)
 
-        # And: Add payload start_date is String
-        custom_validator = CustomValidator({"start_date": "String"})
-        custom_validator.add_error_and_skip_validation_key("start_date", "type should be integer")
-        # And: Set _validate_called to True
-        custom_validator._validate_called = True
+    @patch("payload_validator.validators.PayloadValidator.common_validate")
+    def test_mismatched_error_keys_exception(self, mock_common_validate):
+        # Given:
+        payload = {"displayable": "example"}
+        validator = PayloadValidator(payload)
+        mock_common_validate.side_effect = MismatchedErrorKeysException()
 
         # When:
-        custom_validator._validate_methods()
-
-        # Then:
-        self.assertEqual(custom_validator.error_context["start_date"], ["type should be integer"])
-
-    def test_handle_skip_validation_key_payload_in_payload_key_type_invalid_validate_method_exception_should_not_pass(self):
-        # Given: validate method validation
-        class CustomValidator(PayloadValidator):
-            def validate_start_date(self):
-                if self.payload["start_date"] > 1:
-                    pass
-
-        # And: Add payload start_date is String
-        custom_validator = CustomValidator({"start_date": "String"})
-
-        # Expected:
-        with self.assertRaises(TypeError):
-            custom_validator._validate_methods()
+        with self.assertRaises(MismatchedErrorKeysException):
+            validator._common_validate()
```

