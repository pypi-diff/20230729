# Comparing `tmp/spark_generated_rules_tools-0.1.0.tar.gz` & `tmp/spark_generated_rules_tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_generated_rules_tools-0.1.0.tar", last modified: Tue Jul 18 06:53:33 2023, max compression
+gzip compressed data, was "spark_generated_rules_tools-0.1.1.tar", last modified: Sat Jul 29 05:46:06 2023, max compression
```

## Comparing `spark_generated_rules_tools-0.1.0.tar` & `spark_generated_rules_tools-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 06:53:33.348213 spark_generated_rules_tools-0.1.0/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       52 2023-07-18 06:18:04.000000 spark_generated_rules_tools-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2411 2023-07-18 06:53:33.348213 spark_generated_rules_tools-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1604 2023-07-18 06:35:00.000000 spark_generated_rules_tools-0.1.0/README.md
--rw-rw-rw-   0        0        0      689 2023-07-18 06:18:04.000000 spark_generated_rules_tools-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-18 06:53:33.363839 spark_generated_rules_tools-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1218 2023-07-18 06:18:04.000000 spark_generated_rules_tools-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 06:53:33.332588 spark_generated_rules_tools-0.1.0/spark_generated_rules_tools/
--rw-rw-rw-   0        0        0      874 2023-07-18 06:43:54.000000 spark_generated_rules_tools-0.1.0/spark_generated_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 06:53:33.348213 spark_generated_rules_tools-0.1.0/spark_generated_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.0/spark_generated_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0     8133 2023-07-18 06:52:37.000000 spark_generated_rules_tools-0.1.0/spark_generated_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-07-18 06:53:33.348213 spark_generated_rules_tools-0.1.0/spark_generated_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.0/spark_generated_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_generated_rules_tools-0.1.0/spark_generated_rules_tools/utils/color.py
-drwxrwxrwx   0        0        0        0 2023-07-18 06:53:33.348213 spark_generated_rules_tools-0.1.0/spark_generated_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0    25810 2023-07-14 13:19:59.000000 spark_generated_rules_tools-0.1.0/spark_generated_rules_tools/utils/resource/rules.json
-drwxrwxrwx   0        0        0        0 2023-07-18 06:53:33.348213 spark_generated_rules_tools-0.1.0/spark_generated_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     2411 2023-07-18 06:53:33.000000 spark_generated_rules_tools-0.1.0/spark_generated_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      601 2023-07-18 06:53:33.000000 spark_generated_rules_tools-0.1.0/spark_generated_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 06:53:33.000000 spark_generated_rules_tools-0.1.0/spark_generated_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-07-18 06:53:33.000000 spark_generated_rules_tools-0.1.0/spark_generated_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-07-18 06:53:33.000000 spark_generated_rules_tools-0.1.0/spark_generated_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 05:46:06.993401 spark_generated_rules_tools-0.1.1/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       52 2023-07-18 06:18:04.000000 spark_generated_rules_tools-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2411 2023-07-29 05:46:06.993401 spark_generated_rules_tools-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1604 2023-07-18 06:35:00.000000 spark_generated_rules_tools-0.1.1/README.md
+-rw-rw-rw-   0        0        0      689 2023-07-18 06:18:04.000000 spark_generated_rules_tools-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-29 05:46:06.994401 spark_generated_rules_tools-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1218 2023-07-29 05:45:56.000000 spark_generated_rules_tools-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:46:06.968556 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/
+-rw-rw-rw-   0        0        0     1101 2023-07-29 05:44:29.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:46:06.990408 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    24417 2023-07-29 05:42:33.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:46:06.992400 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/utils/color.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:46:06.992400 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0    26115 2023-07-29 02:06:11.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0      501 2023-07-29 03:39:01.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/utils/utilitty.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:46:06.989396 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     2411 2023-07-29 05:46:06.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      647 2023-07-29 05:46:06.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 05:46:06.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-07-29 05:46:06.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-29 05:46:06.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_generated_rules_tools-0.1.0/LICENSE` & `spark_generated_rules_tools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_generated_rules_tools-0.1.0/PKG-INFO` & `spark_generated_rules_tools-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_generated_rules_tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: spark_generated_rules_tools
 Home-page: https://github.com/jonaqp/spark_generated_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_generated_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_generated_rules_tools-0.1.0/README.md` & `spark_generated_rules_tools-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `spark_generated_rules_tools-0.1.0/pyproject.toml` & `spark_generated_rules_tools-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_generated_rules_tools-0.1.0/setup.py` & `spark_generated_rules_tools-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_generated_rules_tools',
     packages=find_packages(),
-    version='0.1.0',
+    version='0.1.1',
     description='spark_generated_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_generated_rules_tools/',
     download_url='https://github.com/jonaqp/spark_generated_rules_tools/archive/main.zip',
```

### Comparing `spark_generated_rules_tools-0.1.0/spark_generated_rules_tools/__init__.py` & `spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from spark_generated_rules_tools.functions.generator import dq_creating_directory_sandbox
 from spark_generated_rules_tools.functions.generator import dq_generated_rules
 from spark_generated_rules_tools.functions.generator import dq_get_rules_list
 from spark_generated_rules_tools.functions.generator import dq_path_workspace
 from spark_generated_rules_tools.functions.generator import dq_searching_rules
+from spark_generated_rules_tools.functions.generator import dq_generated_dataframe_info
+from spark_generated_rules_tools.functions.generator import dq_generated_mvp
 from spark_generated_rules_tools.utils import BASE_DIR
 from spark_generated_rules_tools.utils.color import get_color
 from spark_generated_rules_tools.utils.color import get_color_b
 
 generator_all = [
     "dq_generated_rules",
     "dq_get_rules_list",
     "dq_path_workspace",
     "dq_searching_rules",
     "dq_creating_directory_sandbox",
+    "dq_generated_dataframe_info",
+    "dq_generated_mvp"
 ]
 
 utils_all = [
     "BASE_DIR",
     "get_color",
     "get_color_b"
 ]
```

### Comparing `spark_generated_rules_tools-0.1.0/spark_generated_rules_tools/utils/resource/rules.json` & `spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/utils/resource/rules.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998640046296297%*

 * *Differences: {"'rules_config'": "{'completeness': {'CompletenessRule': {0: {'rules_columns': {0: "*

 * *                   "{'withRefusals': ['Boolean', 'False', 'False']}}}}, "*

 * *                   "'BasicPerimeterCompletenessRule': {0: {'rules_columns': {0: {'withRefusals': "*

 * *                   "['Boolean', 'False', 'False']}}}}, 'BasicPerimeterVariationCompletenessRule': "*

 * *                   "{0: {'rules_columns': {0: {'withRefusals': ['Boolean', 'False', 'False']}}}}, "*

 * *                   "'ConditionalPerimeterCompleteness […]*

```diff
@@ -626,14 +626,19 @@
                                 "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
                                 "False",
                                 "100"
+                            ],
+                            "withRefusals": [
+                                "Boolean",
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Perimeter Completeness",
                     "rules_version": "2.2-1"
                 }
             ],
@@ -673,14 +678,19 @@
                                 "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
                                 "False",
                                 "100"
+                            ],
+                            "withRefusals": [
+                                "Boolean",
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Perimeter Completeness",
                     "rules_version": "2.2-2"
                 }
             ],
@@ -710,14 +720,19 @@
                                 "False",
                                 "100"
                             ],
                             "targetThreshold": [
                                 "Double",
                                 "False",
                                 "100"
+                            ],
+                            "withRefusals": [
+                                "Boolean",
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Records Completeness",
                     "rules_version": "2.1"
                 }
             ],
@@ -762,14 +777,19 @@
                                 "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
                                 "False",
                                 "100"
+                            ],
+                            "withRefusals": [
+                                "Boolean",
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Perimeter completeness with a filter",
                     "rules_version": "2.3-1"
                 }
             ],
@@ -809,14 +829,19 @@
                                 "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
                                 "False",
                                 "100"
+                            ],
+                            "withRefusals": [
+                                "Boolean",
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Metadata completeness",
                     "rules_version": "2.4"
                 }
             ]
```

### Comparing `spark_generated_rules_tools-0.1.0/spark_generated_rules_tools.egg-info/PKG-INFO` & `spark_generated_rules_tools-0.1.1/spark_generated_rules_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-generated-rules-tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: spark_generated_rules_tools
 Home-page: https://github.com/jonaqp/spark_generated_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_generated_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_generated_rules_tools-0.1.0/spark_generated_rules_tools.egg-info/SOURCES.txt` & `spark_generated_rules_tools-0.1.1/spark_generated_rules_tools.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 spark_generated_rules_tools.egg-info/dependency_links.txt
 spark_generated_rules_tools.egg-info/requires.txt
 spark_generated_rules_tools.egg-info/top_level.txt
 spark_generated_rules_tools/functions/__init__.py
 spark_generated_rules_tools/functions/generator.py
 spark_generated_rules_tools/utils/__init__.py
 spark_generated_rules_tools/utils/color.py
+spark_generated_rules_tools/utils/utilitty.py
 spark_generated_rules_tools/utils/resource/rules.json
```

