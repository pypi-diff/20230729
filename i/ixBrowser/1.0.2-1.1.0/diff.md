# Comparing `tmp/ixBrowser-1.0.2.tar.gz` & `tmp/ixBrowser-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ixBrowser-1.0.2.tar", last modified: Sat Jul 29 05:00:47 2023, max compression
+gzip compressed data, was "dist\ixBrowser-1.1.0.tar", last modified: Sat Jul 29 05:13:48 2023, max compression
```

## Comparing `ixBrowser-1.0.2.tar` & `ixBrowser-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 05:00:47.017131 ixBrowser-1.0.2/
--rw-rw-rw-   0        0        0     1119 2023-07-29 03:38:21.000000 ixBrowser-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      633 2023-07-29 05:00:47.016135 ixBrowser-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 05:00:46.992215 ixBrowser-1.0.2/ixBrowser/
--rw-rw-rw-   0        0        0        0 2023-07-29 03:36:18.000000 ixBrowser-1.0.2/ixBrowser/__init__.py
--rw-rw-rw-   0        0        0     9475 2023-07-29 03:35:16.000000 ixBrowser-1.0.2/ixBrowser/client.py
-drwxrwxrwx   0        0        0        0 2023-07-29 05:00:47.014142 ixBrowser-1.0.2/ixBrowser.egg-info/
--rw-rw-rw-   0        0        0      633 2023-07-29 05:00:46.000000 ixBrowser-1.0.2/ixBrowser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-07-29 05:00:46.000000 ixBrowser-1.0.2/ixBrowser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 05:00:46.000000 ixBrowser-1.0.2/ixBrowser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      339 2023-07-29 05:00:46.000000 ixBrowser-1.0.2/ixBrowser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-29 05:00:46.000000 ixBrowser-1.0.2/ixBrowser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 05:00:47.018128 ixBrowser-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1462 2023-07-29 05:00:45.000000 ixBrowser-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/
+-rw-rw-rw-   0        0        0     1119 2023-07-29 03:38:21.000000 ixBrowser-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      633 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/ixBrowser/
+-rw-rw-rw-   0        0        0        0 2023-07-29 03:36:18.000000 ixBrowser-1.1.0/ixBrowser/__init__.py
+-rw-rw-rw-   0        0        0     9463 2023-07-29 05:12:46.000000 ixBrowser-1.1.0/ixBrowser/client.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/ixBrowser.egg-info/
+-rw-rw-rw-   0        0        0      633 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/ixBrowser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/ixBrowser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/ixBrowser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/ixBrowser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/ixBrowser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1462 2023-07-29 05:12:58.000000 ixBrowser-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/tests/
+-rw-rw-rw-   0        0        0     1622 2023-07-29 03:35:16.000000 ixBrowser-1.1.0/tests/test_ixbrowser.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ixBrowser-1.0.2/LICENSE` & `ixBrowser-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ixBrowser-1.0.2/PKG-INFO` & `ixBrowser-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ixBrowser
-Version: 1.0.2
+Version: 1.1.0
 Summary: A SDK for ixBrowser
 Home-page: https://github.com/ontisme/ixBrowser
 Download-URL: https://pypi.org/project/ixBrowser/
 Author: Alan Ting & Ontisme
 Author-email: alanting0716@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `ixBrowser-1.0.2/ixBrowser/client.py` & `ixBrowser-1.1.0/ixBrowser/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-import re
 import time
 import winreg
 from typing import Union
 
 import requests
 
 from utils.use_logger import WrapperRichLogger
 
 
 class IxBrowser:
-    def __init__(self, api_host: str = "http://127.0.0.1:53200/api/"):
+    def __init__(self, api_port: int = 53200):
         self.ixbrowser_install_dir: str
         self.ixbrowser_exe_path: str
         self.ixbrowser_version: str
-        self.ixbrowser_api_host = api_host
+        self.ixbrowser_api_host = f"http://127.0.0.1:{api_port}/api/"
         self.logger = WrapperRichLogger()
         self.ses = requests.Session()
         self.headers = {
             "Content-Type": "application/json"
         }
         self.ses.headers.update(self.headers)
         self.init()
@@ -262,9 +261,7 @@
         }
         return self.__api_response(self.ses.post(self.ixbrowser_api_host + "browser-close-all", json=params).json())
 
 
 if __name__ == '__main__':
     ixbrowser = IxBrowser()
     ixbrowser.get_ixbrowser_info()
-
-
```

### Comparing `ixBrowser-1.0.2/ixBrowser.egg-info/PKG-INFO` & `ixBrowser-1.1.0/ixBrowser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ixBrowser
-Version: 1.0.2
+Version: 1.1.0
 Summary: A SDK for ixBrowser
 Home-page: https://github.com/ontisme/ixBrowser
 Download-URL: https://pypi.org/project/ixBrowser/
 Author: Alan Ting & Ontisme
 Author-email: alanting0716@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `ixBrowser-1.0.2/setup.py` & `ixBrowser-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 PACKAGE_NAME = "ixBrowser"
 AUTHOR = "Alan Ting & Ontisme"
 AUTHOR_EMAIL = "alanting0716@gmail.com"
 URL = "https://github.com/ontisme/ixBrowser"
 DOWNLOAD_URL = "https://pypi.org/project/ixBrowser/"
 
 LICENSE = "MIT"
-VERSION = "1.0.2"
+VERSION = "1.1.0"
 DESCRIPTION = "A SDK for ixBrowser"
 LONG_DESCRIPTION = (HERE / "docs" / "README.md").read_text(encoding="utf8")
 LONG_DESC_TYPE = "text/markdown"
 
 with open((HERE / "requirements.txt"), encoding="utf8", errors='ignore') as f:
     requirements = f.read()
 INSTALL_REQUIRES = [s.strip() for s in requirements.split("\n")]
 
 with open((HERE / "dev_requirements.txt"), encoding="utf8", errors='ignore') as f:
     dev_requirements = f.read()
 EXTRAS_REQUIRE = {"dev": [s.strip() for s in dev_requirements.split("\n")]}
 
 CLASSIFIERS = [f"Programming Language :: Python :: 3.{str(v)}" for v in range(7, 12)]
-PYTHON_REQUIRES = ">=3.8"
+PYTHON_REQUIRES = ">=3.7"
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type=LONG_DESC_TYPE,
```

