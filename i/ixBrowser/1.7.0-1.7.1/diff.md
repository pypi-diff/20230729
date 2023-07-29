# Comparing `tmp/ixBrowser-1.7.0.tar.gz` & `tmp/ixBrowser-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ixBrowser-1.7.0.tar", last modified: Sat Jul 29 09:53:45 2023, max compression
+gzip compressed data, was "dist\ixBrowser-1.7.1.tar", last modified: Sat Jul 29 10:05:46 2023, max compression
```

## Comparing `ixBrowser-1.7.0.tar` & `ixBrowser-1.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 09:53:45.000000 ixBrowser-1.7.0/
--rw-rw-rw-   0        0        0     1119 2023-07-29 07:13:14.000000 ixBrowser-1.7.0/LICENSE
--rw-rw-rw-   0        0        0     1163 2023-07-29 09:53:45.000000 ixBrowser-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0      526 2023-07-29 09:53:25.000000 ixBrowser-1.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 09:53:45.000000 ixBrowser-1.7.0/ixBrowser/
--rw-rw-rw-   0        0        0       42 2023-07-29 08:32:05.000000 ixBrowser-1.7.0/ixBrowser/__init__.py
--rw-rw-rw-   0        0        0    21182 2023-07-29 09:47:56.000000 ixBrowser-1.7.0/ixBrowser/client.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:53:45.000000 ixBrowser-1.7.0/ixBrowser/tests/
--rw-rw-rw-   0        0        0        0 2023-07-29 07:13:14.000000 ixBrowser-1.7.0/ixBrowser/tests/__init__.py
--rw-rw-rw-   0        0        0     2659 2023-07-29 09:47:56.000000 ixBrowser-1.7.0/ixBrowser/tests/test_ixbrowser.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:53:45.000000 ixBrowser-1.7.0/ixBrowser/utils/
--rw-rw-rw-   0        0        0       26 2023-07-29 09:47:56.000000 ixBrowser-1.7.0/ixBrowser/utils/__init__.py
--rw-rw-rw-   0        0        0     1714 2023-07-29 07:13:14.000000 ixBrowser-1.7.0/ixBrowser/utils/use_logger.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:53:45.000000 ixBrowser-1.7.0/ixBrowser.egg-info/
--rw-rw-rw-   0        0        0     1163 2023-07-29 09:53:45.000000 ixBrowser-1.7.0/ixBrowser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-07-29 09:53:45.000000 ixBrowser-1.7.0/ixBrowser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 09:53:45.000000 ixBrowser-1.7.0/ixBrowser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2023-07-29 09:53:45.000000 ixBrowser-1.7.0/ixBrowser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-29 09:53:45.000000 ixBrowser-1.7.0/ixBrowser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 09:53:45.000000 ixBrowser-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1453 2023-07-29 09:47:56.000000 ixBrowser-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/
+-rw-rw-rw-   0        0        0     1119 2023-07-29 07:13:14.000000 ixBrowser-1.7.1/LICENSE
+-rw-rw-rw-   0        0        0     1163 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-07-29 09:53:25.000000 ixBrowser-1.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/ixBrowser/
+-rw-rw-rw-   0        0        0       42 2023-07-29 08:32:05.000000 ixBrowser-1.7.1/ixBrowser/__init__.py
+-rw-rw-rw-   0        0        0    21188 2023-07-29 10:05:18.000000 ixBrowser-1.7.1/ixBrowser/client.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/ixBrowser/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-29 07:13:14.000000 ixBrowser-1.7.1/ixBrowser/tests/__init__.py
+-rw-rw-rw-   0        0        0     2659 2023-07-29 09:47:56.000000 ixBrowser-1.7.1/ixBrowser/tests/test_ixbrowser.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/ixBrowser/utils/
+-rw-rw-rw-   0        0        0       26 2023-07-29 09:47:56.000000 ixBrowser-1.7.1/ixBrowser/utils/__init__.py
+-rw-rw-rw-   0        0        0     1714 2023-07-29 07:13:14.000000 ixBrowser-1.7.1/ixBrowser/utils/use_logger.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/ixBrowser.egg-info/
+-rw-rw-rw-   0        0        0     1163 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/ixBrowser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/ixBrowser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/ixBrowser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/ixBrowser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/ixBrowser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1453 2023-07-29 10:05:34.000000 ixBrowser-1.7.1/setup.py
```

### Comparing `ixBrowser-1.7.0/LICENSE` & `ixBrowser-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ixBrowser-1.7.0/PKG-INFO` & `ixBrowser-1.7.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixBrowser
-Version: 1.7.0
+Version: 1.7.1
 Summary: A SDK for ixBrowser
 Home-page: https://github.com/ontisme/ixBrowser
 Download-URL: https://pypi.org/project/ixBrowser/
 Author: Alan Ting & Ontisme
 Author-email: alanting0716@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ixBrowser-1.7.0/README.md` & `ixBrowser-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `ixBrowser-1.7.0/ixBrowser/client.py` & `ixBrowser-1.7.1/ixBrowser/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import random
 import time
 import uuid
 import winreg
-from typing import Union
+from typing import Union, List
 
 import requests
 from ixBrowser.utils.use_logger import WrapperRichLogger
 
 
 class IxBrowser:
     def __init__(self, api_port: int = 53200):
@@ -272,15 +272,15 @@
             "profile_id": profile_id,
             "args": args,
             "load_extensions": load_extensions,
             "load_default_page": load_default_page
         }
         return self.__api_response(self.ses.post(self.ixbrowser_api_host + "browser-open", json=params).json())
 
-    def api_browser_close(self, profile_id: Union[int, list[int]]):
+    def api_browser_close(self, profile_id: Union[int, List[int]]):
         """
         關閉ixBrowser
 
         profile_id 是int也可以是一個list，關閉多個ixBrowser
 
         :param profile_id:  profile_id的ID
         :return:
@@ -288,15 +288,15 @@
         if isinstance(profile_id, int):
             profile_id = [profile_id]
         params = {
             "profile_id": profile_id
         }
         return self.__api_response(self.ses.post(self.ixbrowser_api_host + "browser-close-all", json=params).json())
 
-    def api_browser_cache_clear(self, profile_id: Union[int, list[int]]):
+    def api_browser_cache_clear(self, profile_id: Union[int, List[int]]):
         """
         清除ixBrowser快取
 
         profile_id 是int也可以是一個list，清除多個ixBrowser的快取
 
         :param profile_id:  profile_id的ID
         :return: {'result': Bool } 不必關注結果，因為沒有緩存也會回傳False
@@ -510,15 +510,15 @@
             "allow_scan_ports_content": "",
             "real_ip": "120.36.89.204"
         }
         base_values.update(config)
         base_values.update(kwargs)
         return self.__api_response(self.ses.post(self.ixbrowser_api_host + "browser-update", json=base_values).json())
 
-    def api_browser_delete(self, profile_id: Union[int, list[int]]):
+    def api_browser_delete(self, profile_id: Union[int, List[int]]):
         """
         删除ixBrowser
 
         :param profile_id:  ixBrowser的profile_id
         :return:
         """
         if isinstance(profile_id, int):
```

### Comparing `ixBrowser-1.7.0/ixBrowser/tests/test_ixbrowser.py` & `ixBrowser-1.7.1/ixBrowser/tests/test_ixbrowser.py`

 * *Files identical despite different names*

### Comparing `ixBrowser-1.7.0/ixBrowser/utils/use_logger.py` & `ixBrowser-1.7.1/ixBrowser/utils/use_logger.py`

 * *Files identical despite different names*

### Comparing `ixBrowser-1.7.0/ixBrowser.egg-info/PKG-INFO` & `ixBrowser-1.7.1/ixBrowser.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixBrowser
-Version: 1.7.0
+Version: 1.7.1
 Summary: A SDK for ixBrowser
 Home-page: https://github.com/ontisme/ixBrowser
 Download-URL: https://pypi.org/project/ixBrowser/
 Author: Alan Ting & Ontisme
 Author-email: alanting0716@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ixBrowser-1.7.0/setup.py` & `ixBrowser-1.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 PACKAGE_NAME = "ixBrowser"
 AUTHOR = "Alan Ting & Ontisme"
 AUTHOR_EMAIL = "alanting0716@gmail.com"
 URL = "https://github.com/ontisme/ixBrowser"
 DOWNLOAD_URL = "https://pypi.org/project/ixBrowser/"
 
 LICENSE = "MIT"
-VERSION = "1.7.0"
+VERSION = "1.7.1"
 DESCRIPTION = "A SDK for ixBrowser"
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding="utf8")
 LONG_DESC_TYPE = "text/markdown"
 
 with open((HERE / "requirements.txt"), encoding="utf8", errors='ignore') as f:
     requirements = f.read()
 INSTALL_REQUIRES = [s.strip() for s in requirements.split("\n")]
```

