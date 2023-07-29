# Comparing `tmp/sparkdantic-0.1.0.tar.gz` & `tmp/sparkdantic-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkdantic-0.1.0.tar", max compression
+gzip compressed data, was "sparkdantic-0.2.1.tar", max compression
```

## Comparing `sparkdantic-0.1.0.tar` & `sparkdantic-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1471 2023-07-29 05:06:13.853019 sparkdantic-0.1.0/README.md
--rw-r--r--   0        0        0      981 2023-07-29 05:06:13.853019 sparkdantic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      128 2023-07-29 05:06:13.857019 sparkdantic-0.1.0/src/sparkdantic/__init__.py
--rw-r--r--   0        0        0     4220 2023-07-29 05:06:13.857019 sparkdantic-0.1.0/src/sparkdantic/model.py
--rw-r--r--   0        0        0     1982 1970-01-01 00:00:00.000000 sparkdantic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1570 2023-07-29 12:14:24.030539 sparkdantic-0.2.1/README.md
+-rw-r--r--   0        0        0      981 2023-07-29 12:14:24.030539 sparkdantic-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-07-29 12:14:24.030539 sparkdantic-0.2.1/src/sparkdantic/__init__.py
+-rw-r--r--   0        0        0     4577 2023-07-29 12:14:24.030539 sparkdantic-0.2.1/src/sparkdantic/model.py
+-rw-r--r--   0        0        0     2081 1970-01-01 00:00:00.000000 sparkdantic-0.2.1/PKG-INFO
```

### Comparing `sparkdantic-0.1.0/README.md` & `sparkdantic-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 ##  SparkDantic
 
-> 1️⃣ version: 0.1.0
+[![PyPI version](https://badge.fury.io/py/sparkdantic.svg)](https://badge.fury.io/py/sparkdantic)
+
+> 1️⃣ version: 0.2.1
 
 > ✍️ author: Mitchell Lisle
 
 # PySpark Model Conversion Tool
 
 This Python module provides a utility for converting Pydantic models to PySpark schemas. It's implemented as a class 
 named `SparkModel` that extends the Pydantic's `BaseModel`.
```

### Comparing `sparkdantic-0.1.0/pyproject.toml` & `sparkdantic-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sparkdantic"
-version = "0.1.0"
+version = "0.2.1"
 description = "A pydantic -> spark schema library"
 authors = ["Mitchell Lisle <m.lisle90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "sparkdantic", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `sparkdantic-0.1.0/src/sparkdantic/model.py` & `sparkdantic-0.2.1/src/sparkdantic/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 import sys
 from datetime import date, datetime, timedelta
 from decimal import Decimal
 from types import MappingProxyType
 from typing import Tuple, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel, ConfigDict
@@ -21,15 +22,15 @@
     StructType,
     TimestampType,
 )
 
 if sys.version_info > (3, 10):
     from types import UnionType
 else:
-    UnionType = Union
+    UnionType = Union  # pragma: no cover
 
 type_map = MappingProxyType(
     {
         int: IntegerType,
         float: DoubleType,
         str: StringType,
         bool: BooleanType,
@@ -44,33 +45,38 @@
 )
 
 
 class SparkModel(BaseModel):
     """Spark Model representing a Pydantic BaseModel with additional methods to convert it to a PySpark schema.
 
     Methods:
-        spark_schema: Generates a PySpark schema from the model fields.
+        model_spark_schema: Generates a PySpark schema from the model fields.
         _is_nullable: Determines if a type is nullable and returns the type without the Union.
         _get_spark_type: Returns the corresponding PySpark data type for a given Python type, considering nullability.
         _type_to_spark: Converts a given Python type to a corresponding PySpark data type.
     """
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
-    def model_spark_schema(self) -> StructType:
+    @classmethod
+    def model_spark_schema(cls) -> StructType:
         """Generates a PySpark schema from the model fields.
 
         Returns:
             StructType: The generated PySpark schema.
         """
         fields = []
-        for k, v in self.model_fields.items():
-            t, nullable = self._type_to_spark(v.annotation)
-            _struct_field = StructField(k, t, nullable)
-            fields.append(_struct_field)
+        for k, v in cls.model_fields.items():
+            if (inspect.isclass(v.annotation)) and (issubclass(v.annotation, SparkModel)):
+                _struct_field = StructField(k, v.annotation.model_spark_schema(), True)
+                fields.append(StructField(k, v.annotation.model_spark_schema()))
+            else:
+                t, nullable = cls._type_to_spark(v.annotation)
+                _struct_field = StructField(k, t, nullable)
+                fields.append(_struct_field)
         return StructType(fields)
 
     @staticmethod
     def _is_nullable(t: Type) -> Tuple[bool, Type]:
         """Determines if a type is nullable and returns the type without the Union.
 
         Args:
@@ -97,37 +103,38 @@
         Returns:
             DataType: The corresponding PySpark data type.
         """
         spark_type = type_map[t]
         spark_type.nullable = nullable
         return spark_type()
 
-    def _type_to_spark(self, t: Type) -> Tuple[DataType, bool]:
+    @classmethod
+    def _type_to_spark(cls, t: Type) -> Tuple[DataType, bool]:
         """Converts a given Python type to a corresponding PySpark data type.
 
         Args:
             t (Type): The type to convert to a PySpark data type.
 
         Returns:
             DataType: The corresponding PySpark data type.
 
         Raises:
             TypeError: If the type is not recognized in the type map.
         """
-        nullable, t = self._is_nullable(t)
+        nullable, t = cls._is_nullable(t)
 
         args = get_args(t)
         origin = get_origin(t)
 
         if origin is list:
-            array_type = self._get_spark_type(args[0], nullable)
+            array_type = cls._get_spark_type(args[0], nullable)
             return ArrayType(array_type, nullable), nullable
         elif origin is dict:
-            key_type, _ = self._type_to_spark(args[0])
-            value_type, _ = self._type_to_spark(args[1])
+            key_type, _ = cls._type_to_spark(args[0])
+            value_type, _ = cls._type_to_spark(args[1])
             return MapType(key_type, value_type, nullable), nullable
 
         try:
             spark_type = type_map[t]
             spark_type.nullable = nullable
             return spark_type(), nullable
         except KeyError:
```

### Comparing `sparkdantic-0.1.0/PKG-INFO` & `sparkdantic-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: sparkdantic
-Version: 0.1.0
+Version: 0.2.1
 Summary: A pydantic -> spark schema library
 Author: Mitchell Lisle
 Author-email: m.lisle90@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Requires-Dist: pyspark (>=3.4.1,<4.0.0)
 Description-Content-Type: text/markdown
 
 ##  SparkDantic
 
-> 1️⃣ version: 0.1.0
+[![PyPI version](https://badge.fury.io/py/sparkdantic.svg)](https://badge.fury.io/py/sparkdantic)
+
+> 1️⃣ version: 0.2.1
 
 > ✍️ author: Mitchell Lisle
 
 # PySpark Model Conversion Tool
 
 This Python module provides a utility for converting Pydantic models to PySpark schemas. It's implemented as a class 
 named `SparkModel` that extends the Pydantic's `BaseModel`.
```

