# Comparing `tmp/p2p-payme-0.1.1.tar.gz` & `tmp/p2p-payme-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p2p-payme-0.1.1.tar", last modified: Sat Jul 29 16:29:19 2023, max compression
+gzip compressed data, was "p2p-payme-0.1.2.tar", last modified: Sat Jul 29 16:58:37 2023, max compression
```

## Comparing `p2p-payme-0.1.1.tar` & `p2p-payme-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,30 @@
-drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 16:29:19.935130 p2p-payme-0.1.1/
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     5345 2023-07-29 16:29:19.935130 p2p-payme-0.1.1/PKG-INFO
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     5026 2023-07-29 16:07:27.000000 p2p-payme-0.1.1/README.md
-drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 16:29:19.931130 p2p-payme-0.1.1/p2p_payme/
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 14:17:48.000000 p2p-payme-0.1.1/p2p_payme/__init__.py
-drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 16:29:19.931130 p2p-payme-0.1.1/p2p_payme/api/
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-26 18:16:05.000000 p2p-payme-0.1.1/p2p_payme/api/__init__.py
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     2682 2023-07-29 16:05:07.000000 p2p-payme-0.1.1/p2p_payme/api/base.py
-drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 16:29:19.931130 p2p-payme-0.1.1/p2p_payme/auth/
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 14:55:35.000000 p2p-payme-0.1.1/p2p_payme/auth/__init__.py
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     2916 2023-07-29 16:05:13.000000 p2p-payme-0.1.1/p2p_payme/auth/api.py
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      244 2023-07-29 13:25:34.000000 p2p-payme-0.1.1/p2p_payme/auth/scheme.py
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 14:39:48.000000 p2p-payme-0.1.1/p2p_payme/auth.py
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      876 2023-07-29 16:00:45.000000 p2p-payme-0.1.1/p2p_payme/cli.py
-drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 16:29:19.931130 p2p-payme-0.1.1/p2p_payme/client/
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)       35 2023-07-27 08:47:24.000000 p2p-payme-0.1.1/p2p_payme/client/__init__.py
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     2544 2023-07-29 12:35:31.000000 p2p-payme-0.1.1/p2p_payme/client/manager.py
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     3014 2023-07-29 16:04:21.000000 p2p-payme-0.1.1/p2p_payme/client/operations.py
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     1496 2023-07-29 13:24:23.000000 p2p-payme-0.1.1/p2p_payme/client/scheme.py
-drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 16:29:19.931130 p2p-payme-0.1.1/p2p_payme/config/
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-26 18:16:05.000000 p2p-payme-0.1.1/p2p_payme/config/__init__.py
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      114 2023-07-28 10:09:34.000000 p2p-payme-0.1.1/p2p_payme/config/constants.py
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      923 2023-07-26 19:37:31.000000 p2p-payme-0.1.1/p2p_payme/request.py
-drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 16:29:19.931130 p2p-payme-0.1.1/p2p_payme.egg-info/
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     5345 2023-07-29 16:29:19.000000 p2p-payme-0.1.1/p2p_payme.egg-info/PKG-INFO
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      592 2023-07-29 16:29:19.000000 p2p-payme-0.1.1/p2p_payme.egg-info/SOURCES.txt
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        1 2023-07-29 16:29:19.000000 p2p-payme-0.1.1/p2p_payme.egg-info/dependency_links.txt
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)       45 2023-07-29 16:29:19.000000 p2p-payme-0.1.1/p2p_payme.egg-info/entry_points.txt
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      256 2023-07-29 16:29:19.000000 p2p-payme-0.1.1/p2p_payme.egg-info/requires.txt
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)       10 2023-07-29 16:29:19.000000 p2p-payme-0.1.1/p2p_payme.egg-info/top_level.txt
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)       38 2023-07-29 16:29:19.935130 p2p-payme-0.1.1/setup.cfg
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     1122 2023-07-29 16:29:16.000000 p2p-payme-0.1.1/setup.py
+drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 16:58:37.188323 p2p-payme-0.1.2/
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     5345 2023-07-29 16:58:37.188323 p2p-payme-0.1.2/PKG-INFO
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     5026 2023-07-29 16:07:27.000000 p2p-payme-0.1.2/README.md
+drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 16:58:37.184323 p2p-payme-0.1.2/p2p_payme/
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 14:17:48.000000 p2p-payme-0.1.2/p2p_payme/__init__.py
+drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 16:58:37.184323 p2p-payme-0.1.2/p2p_payme/api/
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-26 18:16:05.000000 p2p-payme-0.1.2/p2p_payme/api/__init__.py
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     2682 2023-07-29 16:47:54.000000 p2p-payme-0.1.2/p2p_payme/api/base.py
+drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 16:58:37.188323 p2p-payme-0.1.2/p2p_payme/auth/
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 14:55:35.000000 p2p-payme-0.1.2/p2p_payme/auth/__init__.py
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     2916 2023-07-29 16:46:41.000000 p2p-payme-0.1.2/p2p_payme/auth/api.py
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      244 2023-07-29 13:25:34.000000 p2p-payme-0.1.2/p2p_payme/auth/scheme.py
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      876 2023-07-29 16:00:45.000000 p2p-payme-0.1.2/p2p_payme/cli.py
+drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 16:58:37.188323 p2p-payme-0.1.2/p2p_payme/client/
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)       35 2023-07-27 08:47:24.000000 p2p-payme-0.1.2/p2p_payme/client/__init__.py
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     2544 2023-07-29 12:35:31.000000 p2p-payme-0.1.2/p2p_payme/client/manager.py
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     3033 2023-07-29 16:50:56.000000 p2p-payme-0.1.2/p2p_payme/client/operations.py
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     1496 2023-07-29 13:24:23.000000 p2p-payme-0.1.2/p2p_payme/client/scheme.py
+drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 16:58:37.188323 p2p-payme-0.1.2/p2p_payme/config/
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-26 18:16:05.000000 p2p-payme-0.1.2/p2p_payme/config/__init__.py
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      114 2023-07-28 10:09:34.000000 p2p-payme-0.1.2/p2p_payme/config/constants.py
+drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 16:58:37.184323 p2p-payme-0.1.2/p2p_payme.egg-info/
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     5345 2023-07-29 16:58:37.000000 p2p-payme-0.1.2/p2p_payme.egg-info/PKG-INFO
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      553 2023-07-29 16:58:37.000000 p2p-payme-0.1.2/p2p_payme.egg-info/SOURCES.txt
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        1 2023-07-29 16:58:37.000000 p2p-payme-0.1.2/p2p_payme.egg-info/dependency_links.txt
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)       45 2023-07-29 16:58:37.000000 p2p-payme-0.1.2/p2p_payme.egg-info/entry_points.txt
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      256 2023-07-29 16:58:37.000000 p2p-payme-0.1.2/p2p_payme.egg-info/requires.txt
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)       10 2023-07-29 16:58:37.000000 p2p-payme-0.1.2/p2p_payme.egg-info/top_level.txt
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)       38 2023-07-29 16:58:37.188323 p2p-payme-0.1.2/setup.cfg
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     1122 2023-07-29 16:52:00.000000 p2p-payme-0.1.2/setup.py
```

### Comparing `p2p-payme-0.1.1/PKG-INFO` & `p2p-payme-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p2p-payme
-Version: 0.1.1
+Version: 0.1.2
 Summary: P2P automation
 Home-page: https://github.com/Abdulvoris101/p2p-payme
 Author: Abdulvoris Erkinov
 Author-email: erkinovabdulvoris101@gmail.com
 License: UNKNOWN
 Keywords: python payme p2p automation
 Platform: UNKNOWN
```

### Comparing `p2p-payme-0.1.1/README.md` & `p2p-payme-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `p2p-payme-0.1.1/p2p_payme/api/base.py` & `p2p-payme-0.1.2/p2p_payme/api/base.py`

 * *Files identical despite different names*

### Comparing `p2p-payme-0.1.1/p2p_payme/auth/api.py` & `p2p-payme-0.1.2/p2p_payme/auth/api.py`

 * *Files identical despite different names*

### Comparing `p2p-payme-0.1.1/p2p_payme/cli.py` & `p2p-payme-0.1.2/p2p_payme/cli.py`

 * *Files identical despite different names*

### Comparing `p2p-payme-0.1.1/p2p_payme/client/manager.py` & `p2p-payme-0.1.2/p2p_payme/client/manager.py`

 * *Files identical despite different names*

### Comparing `p2p-payme-0.1.1/p2p_payme/client/operations.py` & `p2p-payme-0.1.2/p2p_payme/client/operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,19 @@
 
 class PaymeClient(Authenticator):
     """
         PaymeClient provides various functions related to Payme, such as get_cards, get_cheques, etc.
         Before using any methods, it will log in every time to obtain a new API key.
     """
 
-    def __init__(self, phone_number, password, device):
+    def __init__(self, phone_number: str, password: str, device: str):
         """
             Initialize PaymeClient with user keys and device information
         """
-
-        self.phone_number = phone_number
+        self.phone_number = str(phone_number)
         self.password = password
         self.device = device
 
 
     def set_auth_headers(self):
         """
             Set authentication headers and log in to obtain the API key.
```

### Comparing `p2p-payme-0.1.1/p2p_payme/client/scheme.py` & `p2p-payme-0.1.2/p2p_payme/client/scheme.py`

 * *Files identical despite different names*

### Comparing `p2p-payme-0.1.1/p2p_payme.egg-info/PKG-INFO` & `p2p-payme-0.1.2/p2p_payme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p2p-payme
-Version: 0.1.1
+Version: 0.1.2
 Summary: P2P automation
 Home-page: https://github.com/Abdulvoris101/p2p-payme
 Author: Abdulvoris Erkinov
 Author-email: erkinovabdulvoris101@gmail.com
 License: UNKNOWN
 Keywords: python payme p2p automation
 Platform: UNKNOWN
```

### Comparing `p2p-payme-0.1.1/p2p_payme.egg-info/SOURCES.txt` & `p2p-payme-0.1.2/p2p_payme.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 README.md
 setup.py
 p2p_payme/__init__.py
-p2p_payme/auth.py
 p2p_payme/cli.py
-p2p_payme/request.py
 p2p_payme.egg-info/PKG-INFO
 p2p_payme.egg-info/SOURCES.txt
 p2p_payme.egg-info/dependency_links.txt
 p2p_payme.egg-info/entry_points.txt
 p2p_payme.egg-info/requires.txt
 p2p_payme.egg-info/top_level.txt
 p2p_payme/api/__init__.py
```

### Comparing `p2p-payme-0.1.1/setup.py` & `p2p-payme-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def get_long_description():
     with open('README.md', mode='r', encoding='utf8') as f:
         return f.read()
 
 setup(
     name='p2p-payme',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
         'annotated-types==0.5.0',
         'certifi==2023.7.22',
         'charset-normalizer==3.2.0',
         'idna==3.4',
         'pydantic==2.1.1',
```

