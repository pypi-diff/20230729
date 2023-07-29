# Comparing `tmp/mypy-boto3-payment-cryptography-1.28.15.tar.gz` & `tmp/mypy-boto3-payment-cryptography-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-payment-cryptography-1.28.15.tar", last modified: Fri Jul 28 20:43:27 2023, max compression
+gzip compressed data, was "mypy-boto3-payment-cryptography-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:51 2023, max compression
```

## Comparing `mypy-boto3-payment-cryptography-1.28.15.tar` & `mypy-boto3-payment-cryptography-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:27.233638 mypy-boto3-payment-cryptography-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15707 2023-07-28 20:43:27.229638 mypy-boto3-payment-cryptography-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:27.225638 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-07-28 20:33:12.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17647 2023-07-28 20:33:15.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17623 2023-07-28 20:33:14.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:27.229638 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15707 2023-07-28 20:43:26.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:43:27.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:26.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:26.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:26.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 20:43:26.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:27.233638 mypy-boto3-payment-cryptography-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:51.341330 mypy-boto3-payment-cryptography-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:52:51.000000 mypy-boto3-payment-cryptography-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-07-29 10:03:51.333330 mypy-boto3-payment-cryptography-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-07-29 09:52:51.000000 mypy-boto3-payment-cryptography-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:51.325330 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-29 09:52:51.000000 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-29 09:52:51.000000 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-29 09:52:51.000000 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-07-29 09:52:52.000000 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-07-29 09:52:52.000000 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-07-29 09:52:52.000000 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-07-29 09:52:52.000000 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-29 09:52:52.000000 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-29 09:52:52.000000 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:52:51.000000 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17647 2023-07-29 09:52:52.000000 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17623 2023-07-29 09:52:52.000000 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:52:51.000000 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:51.333330 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-07-29 10:03:51.000000 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 10:03:51.000000 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:51.000000 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:51.000000 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:51.000000 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-29 10:03:51.000000 mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:51.341330 mypy-boto3-payment-cryptography-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-29 09:52:51.000000 mypy-boto3-payment-cryptography-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-payment-cryptography-1.28.15/LICENSE` & `mypy-boto3-payment-cryptography-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.15/PKG-INFO` & `mypy-boto3-payment-cryptography-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-payment-cryptography
-Version: 1.28.15
-Summary: Type annotations for boto3.PaymentCryptographyControlPlane 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.PaymentCryptographyControlPlane 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/
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
 [mypy-boto3-payment-cryptography docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-payment-cryptography-1.28.15/README.md` & `mypy-boto3-payment-cryptography-1.28.15.post1/README.md`

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
 [mypy-boto3-payment-cryptography docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/__init__.py` & `mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/__init__.pyi` & `mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/__main__.py` & `mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for boto3.PaymentCryptographyControlPlane 1.28.15\nVersion:        "
-        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane\nOther"
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

### Comparing `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/client.py` & `mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/client.pyi` & `mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/literals.py` & `mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/literals.pyi` & `mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/paginator.py` & `mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/paginator.pyi` & `mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/type_defs.py` & `mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/type_defs.pyi` & `mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography.egg-info/PKG-INFO` & `mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-payment-cryptography
-Version: 1.28.15
-Summary: Type annotations for boto3.PaymentCryptographyControlPlane 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.PaymentCryptographyControlPlane 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/
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
 [mypy-boto3-payment-cryptography docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography.egg-info/SOURCES.txt` & `mypy-boto3-payment-cryptography-1.28.15.post1/mypy_boto3_payment_cryptography.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.15/setup.py` & `mypy-boto3-payment-cryptography-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-payment-cryptography",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_payment_cryptography"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.PaymentCryptographyControlPlane 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.1"
+        " mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

