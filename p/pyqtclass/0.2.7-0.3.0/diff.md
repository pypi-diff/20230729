# Comparing `tmp/pyqtclass-0.2.7.tar.gz` & `tmp/pyqtclass-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqtclass-0.2.7.tar", last modified: Sat Jul 29 09:48:46 2023, max compression
+gzip compressed data, was "pyqtclass-0.3.0.tar", last modified: Sat Jul 29 09:52:04 2023, max compression
```

## Comparing `pyqtclass-0.2.7.tar` & `pyqtclass-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 09:48:46.679868 pyqtclass-0.2.7/
--rw-rw-rw-   0        0        0     1086 2023-03-24 01:33:53.000000 pyqtclass-0.2.7/LICENSE
--rw-rw-rw-   0        0        0     1094 2023-07-29 09:48:46.678868 pyqtclass-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      604 2023-07-29 09:47:21.000000 pyqtclass-0.2.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-29 09:48:46.679868 pyqtclass-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      835 2023-07-29 09:44:57.000000 pyqtclass-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:48:46.644861 pyqtclass-0.2.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-29 09:48:46.651861 pyqtclass-0.2.7/src/pyqtclass/
--rw-rw-rw-   0        0        0     6274 2023-07-29 05:03:35.000000 pyqtclass-0.2.7/src/pyqtclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:48:46.675867 pyqtclass-0.2.7/src/pyqtclass.egg-info/
--rw-rw-rw-   0        0        0     1094 2023-07-29 09:48:46.000000 pyqtclass-0.2.7/src/pyqtclass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-07-29 09:48:46.000000 pyqtclass-0.2.7/src/pyqtclass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 09:48:46.000000 pyqtclass-0.2.7/src/pyqtclass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-29 09:48:46.000000 pyqtclass-0.2.7/src/pyqtclass.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-29 09:48:46.000000 pyqtclass-0.2.7/src/pyqtclass.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 09:52:04.811818 pyqtclass-0.3.0/
+-rw-rw-rw-   0        0        0     1086 2023-03-24 01:33:53.000000 pyqtclass-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     1094 2023-07-29 09:52:04.809818 pyqtclass-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      604 2023-07-29 09:47:21.000000 pyqtclass-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-29 09:52:04.811818 pyqtclass-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      835 2023-07-29 09:51:04.000000 pyqtclass-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:52:04.755806 pyqtclass-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-29 09:52:04.767808 pyqtclass-0.3.0/src/pyqtclass/
+-rw-rw-rw-   0        0        0     6274 2023-07-29 05:03:35.000000 pyqtclass-0.3.0/src/pyqtclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:52:04.806817 pyqtclass-0.3.0/src/pyqtclass.egg-info/
+-rw-rw-rw-   0        0        0     1094 2023-07-29 09:52:04.000000 pyqtclass-0.3.0/src/pyqtclass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-07-29 09:52:04.000000 pyqtclass-0.3.0/src/pyqtclass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 09:52:04.000000 pyqtclass-0.3.0/src/pyqtclass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-29 09:52:04.000000 pyqtclass-0.3.0/src/pyqtclass.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-29 09:52:04.000000 pyqtclass-0.3.0/src/pyqtclass.egg-info/top_level.txt
```

### Comparing `pyqtclass-0.2.7/LICENSE` & `pyqtclass-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqtclass-0.2.7/PKG-INFO` & `pyqtclass-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqtclass
-Version: 0.2.7
+Version: 0.3.0
 Summary: PyQt 기반으로 동작하는 객체들의 베이스클래스 모음 패키지
 Home-page: https://github.com/innovata/PyQtClasses
 Author: innovata
 Author-email: iinnovata@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyqtclass-0.2.7/README.md` & `pyqtclass-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyqtclass-0.2.7/setup.py` & `pyqtclass-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyqtclass",
-    version="0.2.7",
+    version="0.3.0",
     author="innovata",
     author_email="iinnovata@gmail.com",
     description='PyQt 기반으로 동작하는 객체들의 베이스클래스 모음 패키지',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f"https://github.com/innovata/PyQtClasses",
     classifiers=[
```

### Comparing `pyqtclass-0.2.7/src/pyqtclass/__init__.py` & `pyqtclass-0.3.0/src/pyqtclass/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtclass-0.2.7/src/pyqtclass.egg-info/PKG-INFO` & `pyqtclass-0.3.0/src/pyqtclass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqtclass
-Version: 0.2.7
+Version: 0.3.0
 Summary: PyQt 기반으로 동작하는 객체들의 베이스클래스 모음 패키지
 Home-page: https://github.com/innovata/PyQtClasses
 Author: innovata
 Author-email: iinnovata@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

