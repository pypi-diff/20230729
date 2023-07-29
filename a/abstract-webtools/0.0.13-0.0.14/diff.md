# Comparing `tmp/abstract_webtools-0.0.13.tar.gz` & `tmp/abstract_webtools-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_webtools-0.0.13.tar", last modified: Sat Jul 29 19:45:51 2023, max compression
+gzip compressed data, was "abstract_webtools-0.0.14.tar", last modified: Sat Jul 29 19:50:03 2023, max compression
```

## Comparing `abstract_webtools-0.0.13.tar` & `abstract_webtools-0.0.14.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:45:51.244279 abstract_webtools-0.0.13/
--rw-r--r--   0 root         (0) root         (0)     3788 2023-07-29 19:45:51.244279 abstract_webtools-0.0.13/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3111 2023-07-29 19:45:03.000000 abstract_webtools-0.0.13/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_webtools-0.0.13/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-07-29 19:45:51.244279 abstract_webtools-0.0.13/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1217 2023-07-29 19:45:13.000000 abstract_webtools-0.0.13/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:45:51.244279 abstract_webtools-0.0.13/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:45:51.244279 abstract_webtools-0.0.13/src/abstract_webtools/
--rw-rw-r--   0 root         (0) root         (0)       28 2023-07-29 19:28:16.000000 abstract_webtools-0.0.13/src/abstract_webtools/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1329 2023-07-29 19:09:21.000000 abstract_webtools-0.0.13/src/abstract_webtools/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:45:51.244279 abstract_webtools-0.0.13/src/abstract_webtools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3788 2023-07-29 19:45:51.000000 abstract_webtools-0.0.13/src/abstract_webtools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-07-29 19:45:51.000000 abstract_webtools-0.0.13/src/abstract_webtools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 19:45:51.000000 abstract_webtools-0.0.13/src/abstract_webtools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-29 19:45:51.000000 abstract_webtools-0.0.13/src/abstract_webtools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-29 19:45:51.000000 abstract_webtools-0.0.13/src/abstract_webtools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:50:03.590374 abstract_webtools-0.0.14/
+-rw-r--r--   0 root         (0) root         (0)     3788 2023-07-29 19:50:03.590374 abstract_webtools-0.0.14/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3111 2023-07-29 19:45:03.000000 abstract_webtools-0.0.14/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_webtools-0.0.14/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-29 19:50:03.590374 abstract_webtools-0.0.14/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1217 2023-07-29 19:49:31.000000 abstract_webtools-0.0.14/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:50:03.590374 abstract_webtools-0.0.14/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:50:03.590374 abstract_webtools-0.0.14/src/abstract_webtools/
+-rw-rw-r--   0 root         (0) root         (0)       28 2023-07-29 19:28:16.000000 abstract_webtools-0.0.14/src/abstract_webtools/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1329 2023-07-29 19:09:21.000000 abstract_webtools-0.0.14/src/abstract_webtools/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:50:03.590374 abstract_webtools-0.0.14/src/abstract_webtools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3788 2023-07-29 19:50:03.000000 abstract_webtools-0.0.14/src/abstract_webtools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-07-29 19:50:03.000000 abstract_webtools-0.0.14/src/abstract_webtools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 19:50:03.000000 abstract_webtools-0.0.14/src/abstract_webtools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-29 19:50:03.000000 abstract_webtools-0.0.14/src/abstract_webtools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-29 19:50:03.000000 abstract_webtools-0.0.14/src/abstract_webtools.egg-info/top_level.txt
```

### Comparing `abstract_webtools-0.0.13/PKG-INFO` & `abstract_webtools-0.0.14/src/abstract_webtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: abstract_webtools
-Version: 0.0.13
+Name: abstract-webtools
+Version: 0.0.14
 Summary: Abstract Web Tools is a Python package that provides various utility functions for web scraping tasks. It is built on top of popular libraries such as `requests`, `BeautifulSoup`, and `urllib3` to simplify the process of fetching and parsing web content.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_webtools
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_nvfx3fos_/tmp_9o_i88c_TarContainer/0/1", line 125, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_nvfx3fos_/tmp_9o_i88c_TarContainer/0/1", line 125, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: abstract_webtools Version: 0.0.13 Summary: Abstract
+Metadata-Version: 2.1 Name: abstract-webtools Version: 0.0.14 Summary: Abstract
 Web Tools is a Python package that provides various utility functions for web
 scraping tasks. It is built on top of popular libraries such as `requests`,
 `BeautifulSoup`, and `urllib3` to simplify the process of fetching and parsing
 web content. Home-page: https://github.com/AbstractEndeavors/
 abstract_essentials/tree/main/abstract_webtools Author: putkoff Author-email:
 partners@abstractendeavors.com Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
```

### Comparing `abstract_webtools-0.0.13/README.md` & `abstract_webtools-0.0.14/README.md`

 * *Files identical despite different names*

### Comparing `abstract_webtools-0.0.13/setup.py` & `abstract_webtools-0.0.14/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_webtools',
-    version='0.0.13',
+    version='0.0.14',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='Abstract Web Tools is a Python package that provides various utility functions for web scraping tasks. It is built on top of popular libraries such as `requests`, `BeautifulSoup`, and `urllib3` to simplify the process of fetching and parsing web content.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_webtools',
     classifiers=[
```

### Comparing `abstract_webtools-0.0.13/src/abstract_webtools/main.py` & `abstract_webtools-0.0.14/src/abstract_webtools/main.py`

 * *Files identical despite different names*

### Comparing `abstract_webtools-0.0.13/src/abstract_webtools.egg-info/PKG-INFO` & `abstract_webtools-0.0.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: abstract-webtools
-Version: 0.0.13
+Name: abstract_webtools
+Version: 0.0.14
 Summary: Abstract Web Tools is a Python package that provides various utility functions for web scraping tasks. It is built on top of popular libraries such as `requests`, `BeautifulSoup`, and `urllib3` to simplify the process of fetching and parsing web content.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_webtools
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_nvfx3fos_/tmp_9o_i88c_TarContainer/0/11", line 125, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_nvfx3fos_/tmp_9o_i88c_TarContainer/0/11", line 125, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: abstract-webtools Version: 0.0.13 Summary: Abstract
+Metadata-Version: 2.1 Name: abstract_webtools Version: 0.0.14 Summary: Abstract
 Web Tools is a Python package that provides various utility functions for web
 scraping tasks. It is built on top of popular libraries such as `requests`,
 `BeautifulSoup`, and `urllib3` to simplify the process of fetching and parsing
 web content. Home-page: https://github.com/AbstractEndeavors/
 abstract_essentials/tree/main/abstract_webtools Author: putkoff Author-email:
 partners@abstractendeavors.com Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
```

