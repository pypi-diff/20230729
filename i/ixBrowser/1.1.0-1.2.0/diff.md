# Comparing `tmp/ixBrowser-1.1.0.tar.gz` & `tmp/ixBrowser-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ixBrowser-1.1.0.tar", last modified: Sat Jul 29 05:13:48 2023, max compression
+gzip compressed data, was "dist\ixBrowser-1.2.0.tar", last modified: Sat Jul 29 05:55:08 2023, max compression
```

## Comparing `ixBrowser-1.1.0.tar` & `ixBrowser-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/
--rw-rw-rw-   0        0        0     1119 2023-07-29 03:38:21.000000 ixBrowser-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      633 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/ixBrowser/
--rw-rw-rw-   0        0        0        0 2023-07-29 03:36:18.000000 ixBrowser-1.1.0/ixBrowser/__init__.py
--rw-rw-rw-   0        0        0     9463 2023-07-29 05:12:46.000000 ixBrowser-1.1.0/ixBrowser/client.py
-drwxrwxrwx   0        0        0        0 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/ixBrowser.egg-info/
--rw-rw-rw-   0        0        0      633 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/ixBrowser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/ixBrowser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/ixBrowser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/ixBrowser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/ixBrowser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1462 2023-07-29 05:12:58.000000 ixBrowser-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 05:13:48.000000 ixBrowser-1.1.0/tests/
--rw-rw-rw-   0        0        0     1622 2023-07-29 03:35:16.000000 ixBrowser-1.1.0/tests/test_ixbrowser.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:55:08.000000 ixBrowser-1.2.0/
+-rw-rw-rw-   0        0        0     1119 2023-07-29 03:38:21.000000 ixBrowser-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      633 2023-07-29 05:55:08.000000 ixBrowser-1.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 05:55:08.000000 ixBrowser-1.2.0/ixBrowser/
+-rw-rw-rw-   0        0        0        0 2023-07-29 03:36:18.000000 ixBrowser-1.2.0/ixBrowser/__init__.py
+-rw-rw-rw-   0        0        0     9545 2023-07-29 05:52:33.000000 ixBrowser-1.2.0/ixBrowser/client.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:55:08.000000 ixBrowser-1.2.0/ixBrowser.egg-info/
+-rw-rw-rw-   0        0        0      633 2023-07-29 05:55:08.000000 ixBrowser-1.2.0/ixBrowser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-07-29 05:55:08.000000 ixBrowser-1.2.0/ixBrowser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 05:55:08.000000 ixBrowser-1.2.0/ixBrowser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-07-29 05:55:08.000000 ixBrowser-1.2.0/ixBrowser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-29 05:55:08.000000 ixBrowser-1.2.0/ixBrowser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 05:55:08.000000 ixBrowser-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1462 2023-07-29 05:55:05.000000 ixBrowser-1.2.0/setup.py
```

### Comparing `ixBrowser-1.1.0/LICENSE` & `ixBrowser-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ixBrowser-1.1.0/PKG-INFO` & `ixBrowser-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixBrowser
-Version: 1.1.0
+Version: 1.2.0
 Summary: A SDK for ixBrowser
 Home-page: https://github.com/ontisme/ixBrowser
 Download-URL: https://pypi.org/project/ixBrowser/
 Author: Alan Ting & Ontisme
 Author-email: alanting0716@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ixBrowser-1.1.0/ixBrowser/client.py` & `ixBrowser-1.2.0/ixBrowser/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,23 +205,23 @@
             # 遞歸處理"data"，如果有更底層的"data"，則覆蓋之前的"data"
             deepest_data = get_deepest_data(response["data"])
             if deepest_data is not None:
                 result["data"] = deepest_data
 
         return result
 
-    def api_browser_list(self):
+    def api_browser_list(self, page: int = 1, limit: int = 1000, group_id: int = 0, name: str = ""):
         """
         取得ixBrowser的瀏覽器列表
         """
         params = {
-            "page": 1,
-            "limit": 1000,
-            "group_id": 0,
-            "name": ""
+            "page": page,
+            "limit": limit,
+            "group_id": group_id,
+            "name": name
         }
         return self.__api_response(self.ses.post(self.ixbrowser_api_host + "browser-list", json=params).json())
 
     def api_browser_open(self, profile_id: int, args: list = None, load_extensions: bool = False,
                          load_default_page: bool = False):
         """
         開啟ixBrowser
```

### Comparing `ixBrowser-1.1.0/ixBrowser.egg-info/PKG-INFO` & `ixBrowser-1.2.0/ixBrowser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixBrowser
-Version: 1.1.0
+Version: 1.2.0
 Summary: A SDK for ixBrowser
 Home-page: https://github.com/ontisme/ixBrowser
 Download-URL: https://pypi.org/project/ixBrowser/
 Author: Alan Ting & Ontisme
 Author-email: alanting0716@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ixBrowser-1.1.0/setup.py` & `ixBrowser-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 PACKAGE_NAME = "ixBrowser"
 AUTHOR = "Alan Ting & Ontisme"
 AUTHOR_EMAIL = "alanting0716@gmail.com"
 URL = "https://github.com/ontisme/ixBrowser"
 DOWNLOAD_URL = "https://pypi.org/project/ixBrowser/"
 
 LICENSE = "MIT"
-VERSION = "1.1.0"
+VERSION = "1.2.0"
 DESCRIPTION = "A SDK for ixBrowser"
 LONG_DESCRIPTION = (HERE / "docs" / "README.md").read_text(encoding="utf8")
 LONG_DESC_TYPE = "text/markdown"
 
 with open((HERE / "requirements.txt"), encoding="utf8", errors='ignore') as f:
     requirements = f.read()
 INSTALL_REQUIRES = [s.strip() for s in requirements.split("\n")]
```

