# Comparing `tmp/cf2tf-0.6.0.tar.gz` & `tmp/cf2tf-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf2tf-0.6.0.tar", max compression
+gzip compressed data, was "cf2tf-0.6.1.tar", max compression
```

## Comparing `cf2tf-0.6.0.tar` & `cf2tf-0.6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-07-09 21:10:05.191587 cf2tf-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     7382 2023-07-09 21:10:05.191587 cf2tf-0.6.0/README.md
--rw-r--r--   0        0        0     1087 2023-07-09 21:10:19.743600 cf2tf-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-09 21:10:05.191587 cf2tf-0.6.0/src/cf2tf/__init__.py
--rw-r--r--   0        0        0     1451 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/app.py
--rw-r--r--   0        0        0       46 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/cloudformation/__init__.py
--rw-r--r--   0        0        0     2605 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/cloudformation/_template.py
--rw-r--r--   0        0        0        0 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/conversion/__init__.py
--rw-r--r--   0        0        0    31201 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/conversion/expressions.py
--rw-r--r--   0        0        0     2026 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/conversion/overrides.py
--rw-r--r--   0        0        0    20221 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/convert.py
--rw-r--r--   0        0        0     2629 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/save.py
--rw-r--r--   0        0        0        0 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/__init__.py
--rw-r--r--   0        0        0      368 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/_configuration.py
--rw-r--r--   0        0        0     2200 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/blocks.py
--rw-r--r--   0        0        0     3995 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/code.py
--rw-r--r--   0        0        0     2865 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/doc_file.py
--rw-r--r--   0        0        0      304 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/hcl2/__init__.py
--rw-r--r--   0        0        0     2971 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/hcl2/_block.py
--rw-r--r--   0        0        0     1815 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/hcl2/complex.py
--rw-r--r--   0        0        0      868 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/hcl2/custom.py
--rw-r--r--   0        0        0     2171 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/hcl2/primitive.py
--rw-r--r--   0        0        0     8428 1970-01-01 00:00:00.000000 cf2tf-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-29 13:31:13.203145 cf2tf-0.6.1/LICENSE.txt
+-rw-r--r--   0        0        0     7382 2023-07-29 13:31:13.203145 cf2tf-0.6.1/README.md
+-rw-r--r--   0        0        0     1087 2023-07-29 13:31:25.775005 cf2tf-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-29 13:31:13.203145 cf2tf-0.6.1/src/cf2tf/__init__.py
+-rw-r--r--   0        0        0     1451 2023-07-29 13:31:13.207145 cf2tf-0.6.1/src/cf2tf/app.py
+-rw-r--r--   0        0        0       46 2023-07-29 13:31:13.207145 cf2tf-0.6.1/src/cf2tf/cloudformation/__init__.py
+-rw-r--r--   0        0        0     2605 2023-07-29 13:31:13.207145 cf2tf-0.6.1/src/cf2tf/cloudformation/_template.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:31:13.207145 cf2tf-0.6.1/src/cf2tf/conversion/__init__.py
+-rw-r--r--   0        0        0    31201 2023-07-29 13:31:13.207145 cf2tf-0.6.1/src/cf2tf/conversion/expressions.py
+-rw-r--r--   0        0        0     2026 2023-07-29 13:31:13.207145 cf2tf-0.6.1/src/cf2tf/conversion/overrides.py
+-rw-r--r--   0        0        0    20221 2023-07-29 13:31:13.207145 cf2tf-0.6.1/src/cf2tf/convert.py
+-rw-r--r--   0        0        0     2629 2023-07-29 13:31:13.207145 cf2tf-0.6.1/src/cf2tf/save.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:31:13.207145 cf2tf-0.6.1/src/cf2tf/terraform/__init__.py
+-rw-r--r--   0        0        0      368 2023-07-29 13:31:13.207145 cf2tf-0.6.1/src/cf2tf/terraform/_configuration.py
+-rw-r--r--   0        0        0     2200 2023-07-29 13:31:13.207145 cf2tf-0.6.1/src/cf2tf/terraform/blocks.py
+-rw-r--r--   0        0        0     3995 2023-07-29 13:31:13.207145 cf2tf-0.6.1/src/cf2tf/terraform/code.py
+-rw-r--r--   0        0        0     2864 2023-07-29 13:31:13.207145 cf2tf-0.6.1/src/cf2tf/terraform/doc_file.py
+-rw-r--r--   0        0        0      304 2023-07-29 13:31:13.207145 cf2tf-0.6.1/src/cf2tf/terraform/hcl2/__init__.py
+-rw-r--r--   0        0        0     2971 2023-07-29 13:31:13.207145 cf2tf-0.6.1/src/cf2tf/terraform/hcl2/_block.py
+-rw-r--r--   0        0        0     1815 2023-07-29 13:31:13.207145 cf2tf-0.6.1/src/cf2tf/terraform/hcl2/complex.py
+-rw-r--r--   0        0        0      868 2023-07-29 13:31:13.207145 cf2tf-0.6.1/src/cf2tf/terraform/hcl2/custom.py
+-rw-r--r--   0        0        0     2171 2023-07-29 13:31:13.207145 cf2tf-0.6.1/src/cf2tf/terraform/hcl2/primitive.py
+-rw-r--r--   0        0        0     8428 1970-01-01 00:00:00.000000 cf2tf-0.6.1/PKG-INFO
```

### Comparing `cf2tf-0.6.0/LICENSE.txt` & `cf2tf-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.0/README.md` & `cf2tf-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.0/pyproject.toml` & `cf2tf-0.6.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cf2tf"
-version = "0.6.0"
+version = "0.6.1"
 description = "Convert Cloudformation Templates to Terraform."
 readme = "README.md"
 authors = ["Levi Blaney <shadycuz@gmail.com>"]
 repository = "https://github.com/DontShaveTheYak/cf2tf"
 keywords = ["cloudformation", "terraform", "cf2tf", "convert", "cloud", "conversion"]
 license = "GPL-3.0-only"
```

### Comparing `cf2tf-0.6.0/src/cf2tf/app.py` & `cf2tf-0.6.1/src/cf2tf/app.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.0/src/cf2tf/cloudformation/_template.py` & `cf2tf-0.6.1/src/cf2tf/cloudformation/_template.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.0/src/cf2tf/conversion/expressions.py` & `cf2tf-0.6.1/src/cf2tf/conversion/expressions.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.0/src/cf2tf/conversion/overrides.py` & `cf2tf-0.6.1/src/cf2tf/conversion/overrides.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.0/src/cf2tf/convert.py` & `cf2tf-0.6.1/src/cf2tf/convert.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.0/src/cf2tf/save.py` & `cf2tf-0.6.1/src/cf2tf/save.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.0/src/cf2tf/terraform/blocks.py` & `cf2tf-0.6.1/src/cf2tf/terraform/blocks.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.0/src/cf2tf/terraform/code.py` & `cf2tf-0.6.1/src/cf2tf/terraform/code.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.0/src/cf2tf/terraform/doc_file.py` & `cf2tf-0.6.1/src/cf2tf/terraform/doc_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     with open(docs_path) as file:
         try:
             arguments = parse_section("Argument Reference", file)
         except Exception as e:
             raise Exception(f"Unable to find arguments in {file.name}") from e
 
         try:
-            attributes = parse_section("Attributes Reference", file)
+            attributes = parse_section("Attribute Reference", file)
         except Exception as e:
             raise Exception(f"Unable to find attributes in {file.name}") from e
 
     return (arguments, attributes)
 
 
 def read_section(docs_path: Path, section_name: str):
```

### Comparing `cf2tf-0.6.0/src/cf2tf/terraform/hcl2/_block.py` & `cf2tf-0.6.1/src/cf2tf/terraform/hcl2/_block.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.0/src/cf2tf/terraform/hcl2/complex.py` & `cf2tf-0.6.1/src/cf2tf/terraform/hcl2/complex.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.0/src/cf2tf/terraform/hcl2/custom.py` & `cf2tf-0.6.1/src/cf2tf/terraform/hcl2/custom.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.0/src/cf2tf/terraform/hcl2/primitive.py` & `cf2tf-0.6.1/src/cf2tf/terraform/hcl2/primitive.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.0/PKG-INFO` & `cf2tf-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf2tf
-Version: 0.6.0
+Version: 0.6.1
 Summary: Convert Cloudformation Templates to Terraform.
 Home-page: https://github.com/DontShaveTheYak/cf2tf
 License: GPL-3.0-only
 Keywords: cloudformation,terraform,cf2tf,convert,cloud,conversion
 Author: Levi Blaney
 Author-email: shadycuz@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cf2tf Version: 0.6.0 Summary: Convert
+Metadata-Version: 2.1 Name: cf2tf Version: 0.6.1 Summary: Convert
 Cloudformation Templates to Terraform. Home-page: https://github.com/
 DontShaveTheYak/cf2tf License: GPL-3.0-only Keywords:
 cloudformation,terraform,cf2tf,convert,cloud,conversion Author: Levi Blaney
 Author-email: shadycuz@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

