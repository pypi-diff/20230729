# Comparing `tmp/ingestor_by_ckl-1.tar.gz` & `tmp/ingestor_by_ckl-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ingestor_by_ckl-1.tar", last modified: Thu Jul 27 15:55:33 2023, max compression
+gzip compressed data, was "ingestor_by_ckl-2.tar", last modified: Sat Jul 29 15:43:15 2023, max compression
```

## Comparing `ingestor_by_ckl-1.tar` & `ingestor_by_ckl-2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-27 15:55:33.750687 ingestor_by_ckl-1/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      275 2023-07-27 15:55:33.746687 ingestor_by_ckl-1/PKG-INFO
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-27 15:55:33.730687 ingestor_by_ckl-1/ingestor/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       24 2023-07-25 22:26:46.000000 ingestor_by_ckl-1/ingestor/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2293 2023-07-21 20:41:49.000000 ingestor_by_ckl-1/ingestor/processors.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-27 15:55:33.746687 ingestor_by_ckl-1/ingestor_by_ckl.egg-info/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      275 2023-07-27 15:55:33.000000 ingestor_by_ckl-1/ingestor_by_ckl.egg-info/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      208 2023-07-27 15:55:33.000000 ingestor_by_ckl-1/ingestor_by_ckl.egg-info/SOURCES.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-07-27 15:55:33.000000 ingestor_by_ckl-1/ingestor_by_ckl.egg-info/dependency_links.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        9 2023-07-27 15:55:33.000000 ingestor_by_ckl-1/ingestor_by_ckl.egg-info/top_level.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-07-27 15:55:33.750687 ingestor_by_ckl-1/setup.cfg
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      638 2023-07-27 15:55:10.000000 ingestor_by_ckl-1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 15:43:15.707599 ingestor_by_ckl-2/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-29 15:43:15.707599 ingestor_by_ckl-2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 15:43:15.707599 ingestor_by_ckl-2/ingestor/
+-rw-rw-r--   0 root         (0) root         (0)       24 2023-07-25 22:26:46.000000 ingestor_by_ckl-2/ingestor/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2392 2023-07-29 15:39:40.000000 ingestor_by_ckl-2/ingestor/processors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 15:43:15.707599 ingestor_by_ckl-2/ingestor_by_ckl.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)      322 2023-07-29 15:43:15.000000 ingestor_by_ckl-2/ingestor_by_ckl.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      208 2023-07-29 15:43:15.000000 ingestor_by_ckl-2/ingestor_by_ckl.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-29 15:43:15.000000 ingestor_by_ckl-2/ingestor_by_ckl.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)        9 2023-07-29 15:43:15.000000 ingestor_by_ckl-2/ingestor_by_ckl.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 15:43:15.707599 ingestor_by_ckl-2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      638 2023-07-29 15:43:03.000000 ingestor_by_ckl-2/setup.py
```

### Comparing `ingestor_by_ckl-1/ingestor/processors.py` & `ingestor_by_ckl-2/ingestor/processors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,31 @@
-from pyspark.ml import Transformer
+from pprint import pprint
+
 import pyspark.sql.functions as F
 from pyspark import keyword_only
+from pyspark.ml import Transformer
 from pyspark.ml.param.shared import HasInputCols, HasOutputCol, HasInputCol
 from pyspark.ml.util import DefaultParamsReadable, DefaultParamsWritable
+import os
+print("VARS:")
+print(os.environ['JAVA_HOME'])
+pprint(os.environ)
 
 class PreProcessor(Transformer, HasOutputCol, HasInputCols, DefaultParamsReadable, DefaultParamsWritable):
     @keyword_only
     def __init__(self, inputCols=None, outputCol=None):
         super(PreProcessor, self).__init__()
         kwargs = self._input_kwargs
         self.setParams(**kwargs)
 
     @keyword_only
     def setParams(self, inputCols=None, outputCol=None):
         kwargs = self._input_kwargs
         return self._set(**kwargs)
-    
+
     def setInputCols(self, value):
         """
         Sets the value of :py:attr:`inputCol`.
         """
         return self._set(inputCols=value)
 
     def setOutputCol(self, value):
@@ -32,26 +38,27 @@
         output_column = self.getOutputCol()
         input_columns = self.getInputCols()
         return (
             dataset
             .withColumn(output_column, F.col(input_columns[0]) * F.col(input_columns[1]))
         )
 
+
 class PostProcessor(Transformer, HasOutputCol, HasInputCol, DefaultParamsReadable, DefaultParamsWritable):
     @keyword_only
     def __init__(self, inputCol=None, outputCol=None):
         super(PostProcessor, self).__init__()
         kwargs = self._input_kwargs
         self.setParams(**kwargs)
 
     @keyword_only
     def setParams(self, inputCol=None, outputCol=None):
         kwargs = self._input_kwargs
         return self._set(**kwargs)
-    
+
     def setInputCol(self, value):
         """
         Sets the value of :py:attr:`inputCol`.
         """
         return self._set(inputCol=value)
 
     def setOutputCol(self, value):
@@ -60,8 +67,10 @@
         """
         return self._set(outputCol=value)
 
     def _transform(self, dataset):
         output_column = self.getOutputCol()
         input_column = self.getInputCol()
         # Clip regression values at a minimum of 0.
-        return dataset.withColumn(output_column, F.when(F.col(input_column) < 0.0,0.0).otherwise(F.col(input_column)))
+        return dataset.withColumn(output_column, F.when(F.col(input_column) < 0.0, 0.0).otherwise(F.col(input_column)))
+
+
```

### Comparing `ingestor_by_ckl-1/setup.py` & `ingestor_by_ckl-2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def is_comment_or_empty(line):
     stripped = line.strip()
     return stripped == "" or stripped.startswith("#")
 
 setup(
     name="ingestor_by_ckl",
-    version='1',
+    version='2',
     packages=find_packages(exclude=["tests", "tests.*"]),
     author="Databricks",
     description="MLflow: A Platform for ML Development and Productionization",
     long_description_content_type="text/x-rst",
     license="Apache License 2.0",
     classifiers=[
         "Intended Audience :: Developers",
```

