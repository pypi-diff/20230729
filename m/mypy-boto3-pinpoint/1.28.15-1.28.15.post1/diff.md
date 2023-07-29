# Comparing `tmp/mypy-boto3-pinpoint-1.28.15.tar.gz` & `tmp/mypy-boto3-pinpoint-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pinpoint-1.28.15.tar", last modified: Fri Jul 28 19:47:31 2023, max compression
+gzip compressed data, was "mypy-boto3-pinpoint-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:53 2023, max compression
```

## Comparing `mypy-boto3-pinpoint-1.28.15.tar` & `mypy-boto3-pinpoint-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.676180 mypy-boto3-pinpoint-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-07-28 19:47:31.676180 mypy-boto3-pinpoint-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28667 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.676180 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79752 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    79624 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   170188 2023-07-28 19:47:22.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   169965 2023-07-28 19:47:20.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.676180 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-07-28 19:47:31.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-28 19:47:31.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:47:31.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:47:31.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 19:47:31.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 19:47:31.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:47:31.676180 mypy-boto3-pinpoint-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:53.357338 mypy-boto3-pinpoint-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:53:08.000000 mypy-boto3-pinpoint-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    30164 2023-07-29 10:03:53.357338 mypy-boto3-pinpoint-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28667 2023-07-29 09:53:08.000000 mypy-boto3-pinpoint-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:53.353338 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-29 09:53:08.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-29 09:53:08.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 09:53:08.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79811 2023-07-29 09:53:09.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79683 2023-07-29 09:53:09.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-07-29 09:53:09.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-07-29 09:53:09.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:53:08.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   170188 2023-07-29 09:53:17.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169965 2023-07-29 09:53:15.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:53:08.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:53.357338 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30164 2023-07-29 10:03:53.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-29 10:03:53.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:53.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:53.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:53.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:03:53.000000 mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:53.357338 mypy-boto3-pinpoint-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 09:53:08.000000 mypy-boto3-pinpoint-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-pinpoint-1.28.15/LICENSE` & `mypy-boto3-pinpoint-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.15/PKG-INFO` & `mypy-boto3-pinpoint-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint
-Version: 1.28.15
-Summary: Type annotations for boto3.Pinpoint 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Pinpoint 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-pinpoint-1.28.15/README.md` & `mypy-boto3-pinpoint-1.28.15.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/__main__.py` & `mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Pinpoint 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Pinpoint 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15")
+    print("1.28.15.post1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/client.py` & `mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,14 +136,15 @@
     SendMessagesResponseTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SendOTPMessageResponseTypeDef,
     SendUsersMessageRequestTypeDef,
     SendUsersMessagesResponseTypeDef,
     SMSChannelRequestTypeDef,
     SMSTemplateRequestTypeDef,
+    TagsModelOutputTypeDef,
     TagsModelTypeDef,
     TemplateActiveVersionRequestTypeDef,
     UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelResponseTypeDef,
@@ -1260,15 +1261,15 @@
         Creates and sends a message to a list of users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.send_users_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#send_users_messages)
         """
 
     def tag_resource(
-        self, *, ResourceArn: str, TagsModel: TagsModelTypeDef
+        self, *, ResourceArn: str, TagsModel: Union[TagsModelTypeDef, TagsModelOutputTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds one or more tags (keys and values) to an application, campaign, message
         template, or segment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#tag_resource)
```

### Comparing `mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/client.pyi` & `mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -136,14 +136,15 @@
     SendMessagesResponseTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SendOTPMessageResponseTypeDef,
     SendUsersMessageRequestTypeDef,
     SendUsersMessagesResponseTypeDef,
     SMSChannelRequestTypeDef,
     SMSTemplateRequestTypeDef,
+    TagsModelOutputTypeDef,
     TagsModelTypeDef,
     TemplateActiveVersionRequestTypeDef,
     UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelResponseTypeDef,
@@ -1158,15 +1159,15 @@
         """
         Creates and sends a message to a list of users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.send_users_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#send_users_messages)
         """
     def tag_resource(
-        self, *, ResourceArn: str, TagsModel: TagsModelTypeDef
+        self, *, ResourceArn: str, TagsModel: Union[TagsModelTypeDef, TagsModelOutputTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds one or more tags (keys and values) to an application, campaign, message
         template, or segment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#tag_resource)
```

### Comparing `mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/literals.py` & `mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/literals.pyi` & `mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/type_defs.py` & `mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/type_defs.pyi` & `mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint.egg-info/PKG-INFO` & `mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint
-Version: 1.28.15
-Summary: Type annotations for boto3.Pinpoint 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Pinpoint 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint.egg-info/SOURCES.txt` & `mypy-boto3-pinpoint-1.28.15.post1/mypy_boto3_pinpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.15/setup.py` & `mypy-boto3-pinpoint-1.28.15.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pinpoint",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_pinpoint"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Pinpoint 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.1"
+        " 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```
