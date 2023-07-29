# Comparing `tmp/ixBrowser-1.7.1.tar.gz` & `tmp/ixBrowser-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ixBrowser-1.7.1.tar", last modified: Sat Jul 29 10:05:46 2023, max compression
+gzip compressed data, was "dist\ixBrowser-1.7.2.tar", last modified: Sat Jul 29 10:08:45 2023, max compression
```

## Comparing `ixBrowser-1.7.1.tar` & `ixBrowser-1.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/
--rw-rw-rw-   0        0        0     1119 2023-07-29 07:13:14.000000 ixBrowser-1.7.1/LICENSE
--rw-rw-rw-   0        0        0     1163 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/PKG-INFO
--rw-rw-rw-   0        0        0      526 2023-07-29 09:53:25.000000 ixBrowser-1.7.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/ixBrowser/
--rw-rw-rw-   0        0        0       42 2023-07-29 08:32:05.000000 ixBrowser-1.7.1/ixBrowser/__init__.py
--rw-rw-rw-   0        0        0    21188 2023-07-29 10:05:18.000000 ixBrowser-1.7.1/ixBrowser/client.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/ixBrowser/tests/
--rw-rw-rw-   0        0        0        0 2023-07-29 07:13:14.000000 ixBrowser-1.7.1/ixBrowser/tests/__init__.py
--rw-rw-rw-   0        0        0     2659 2023-07-29 09:47:56.000000 ixBrowser-1.7.1/ixBrowser/tests/test_ixbrowser.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/ixBrowser/utils/
--rw-rw-rw-   0        0        0       26 2023-07-29 09:47:56.000000 ixBrowser-1.7.1/ixBrowser/utils/__init__.py
--rw-rw-rw-   0        0        0     1714 2023-07-29 07:13:14.000000 ixBrowser-1.7.1/ixBrowser/utils/use_logger.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/ixBrowser.egg-info/
--rw-rw-rw-   0        0        0     1163 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/ixBrowser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/ixBrowser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/ixBrowser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/ixBrowser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/ixBrowser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 10:05:46.000000 ixBrowser-1.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1453 2023-07-29 10:05:34.000000 ixBrowser-1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:08:45.000000 ixBrowser-1.7.2/
+-rw-rw-rw-   0        0        0     1119 2023-07-29 07:13:14.000000 ixBrowser-1.7.2/LICENSE
+-rw-rw-rw-   0        0        0     1163 2023-07-29 10:08:45.000000 ixBrowser-1.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-07-29 09:53:25.000000 ixBrowser-1.7.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 10:08:45.000000 ixBrowser-1.7.2/ixBrowser/
+-rw-rw-rw-   0        0        0       42 2023-07-29 08:32:05.000000 ixBrowser-1.7.2/ixBrowser/__init__.py
+-rw-rw-rw-   0        0        0    21188 2023-07-29 10:07:53.000000 ixBrowser-1.7.2/ixBrowser/client.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:08:45.000000 ixBrowser-1.7.2/ixBrowser/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-29 07:13:14.000000 ixBrowser-1.7.2/ixBrowser/tests/__init__.py
+-rw-rw-rw-   0        0        0     2659 2023-07-29 09:47:56.000000 ixBrowser-1.7.2/ixBrowser/tests/test_ixbrowser.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:08:45.000000 ixBrowser-1.7.2/ixBrowser/utils/
+-rw-rw-rw-   0        0        0       26 2023-07-29 09:47:56.000000 ixBrowser-1.7.2/ixBrowser/utils/__init__.py
+-rw-rw-rw-   0        0        0     1714 2023-07-29 07:13:14.000000 ixBrowser-1.7.2/ixBrowser/utils/use_logger.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:08:45.000000 ixBrowser-1.7.2/ixBrowser.egg-info/
+-rw-rw-rw-   0        0        0     1163 2023-07-29 10:08:44.000000 ixBrowser-1.7.2/ixBrowser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-07-29 10:08:45.000000 ixBrowser-1.7.2/ixBrowser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 10:08:44.000000 ixBrowser-1.7.2/ixBrowser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-07-29 10:08:44.000000 ixBrowser-1.7.2/ixBrowser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-29 10:08:44.000000 ixBrowser-1.7.2/ixBrowser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 10:08:45.000000 ixBrowser-1.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     1453 2023-07-29 10:08:01.000000 ixBrowser-1.7.2/setup.py
```

### Comparing `ixBrowser-1.7.1/LICENSE` & `ixBrowser-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ixBrowser-1.7.1/PKG-INFO` & `ixBrowser-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixBrowser
-Version: 1.7.1
+Version: 1.7.2
 Summary: A SDK for ixBrowser
 Home-page: https://github.com/ontisme/ixBrowser
 Download-URL: https://pypi.org/project/ixBrowser/
 Author: Alan Ting & Ontisme
 Author-email: alanting0716@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ixBrowser-1.7.1/README.md` & `ixBrowser-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `ixBrowser-1.7.1/ixBrowser/client.py` & `ixBrowser-1.7.2/ixBrowser/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
             deepest_data = get_deepest_data(response["data"])
             if deepest_data is not None:
                 result["data"] = deepest_data
 
         return result
 
     def api_browser_list(self, page: int = 1, limit: int = 1000, group_id: int = 0, name: str = "",
-                         include_fields: list[str] = None, exclude_fields: list[str] = None):
+                         include_fields: List[str] = None, exclude_fields: List[str] = None):
         """
         獲取ixBrowser的瀏覽器列表
         :param page:            頁碼
         :param limit:           每頁顯示的數量
         :param group_id:        組ID
         :param name:            瀏覽器名稱
         :param include_fields:  只回傳想要的瀏覽器配置
```

### Comparing `ixBrowser-1.7.1/ixBrowser/tests/test_ixbrowser.py` & `ixBrowser-1.7.2/ixBrowser/tests/test_ixbrowser.py`

 * *Files identical despite different names*

### Comparing `ixBrowser-1.7.1/ixBrowser/utils/use_logger.py` & `ixBrowser-1.7.2/ixBrowser/utils/use_logger.py`

 * *Files identical despite different names*

### Comparing `ixBrowser-1.7.1/ixBrowser.egg-info/PKG-INFO` & `ixBrowser-1.7.2/ixBrowser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixBrowser
-Version: 1.7.1
+Version: 1.7.2
 Summary: A SDK for ixBrowser
 Home-page: https://github.com/ontisme/ixBrowser
 Download-URL: https://pypi.org/project/ixBrowser/
 Author: Alan Ting & Ontisme
 Author-email: alanting0716@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ixBrowser-1.7.1/setup.py` & `ixBrowser-1.7.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 PACKAGE_NAME = "ixBrowser"
 AUTHOR = "Alan Ting & Ontisme"
 AUTHOR_EMAIL = "alanting0716@gmail.com"
 URL = "https://github.com/ontisme/ixBrowser"
 DOWNLOAD_URL = "https://pypi.org/project/ixBrowser/"
 
 LICENSE = "MIT"
-VERSION = "1.7.1"
+VERSION = "1.7.2"
 DESCRIPTION = "A SDK for ixBrowser"
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding="utf8")
 LONG_DESC_TYPE = "text/markdown"
 
 with open((HERE / "requirements.txt"), encoding="utf8", errors='ignore') as f:
     requirements = f.read()
 INSTALL_REQUIRES = [s.strip() for s in requirements.split("\n")]
```

