# Comparing `tmp/basicnanoclient-0.0.7.tar.gz` & `tmp/basicnanoclient-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basicnanoclient-0.0.7.tar", last modified: Fri Jul 28 03:13:05 2023, max compression
+gzip compressed data, was "basicnanoclient-0.1.0.tar", last modified: Sat Jul 29 16:21:41 2023, max compression
```

## Comparing `basicnanoclient-0.0.7.tar` & `basicnanoclient-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-28 03:13:05.811622 basicnanoclient-0.0.7/
--rw-r--r--   0 nate       (501) staff       (20)     1211 2023-07-28 01:29:38.000000 basicnanoclient-0.0.7/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)     2762 2023-07-28 03:13:05.811501 basicnanoclient-0.0.7/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)      844 2023-07-28 01:29:38.000000 basicnanoclient-0.0.7/README.md
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-28 03:13:05.810666 basicnanoclient-0.0.7/basicnanoclient/
--rw-r--r--   0 nate       (501) staff       (20)      104 2023-07-28 03:09:02.000000 basicnanoclient-0.0.7/basicnanoclient/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)    10922 2023-07-28 02:23:13.000000 basicnanoclient-0.0.7/basicnanoclient/nano.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-28 03:13:05.811244 basicnanoclient-0.0.7/basicnanoclient.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)     2762 2023-07-28 03:13:05.000000 basicnanoclient-0.0.7/basicnanoclient.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)      287 2023-07-28 03:13:05.000000 basicnanoclient-0.0.7/basicnanoclient.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-28 03:13:05.000000 basicnanoclient-0.0.7/basicnanoclient.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)       60 2023-07-28 03:13:05.000000 basicnanoclient-0.0.7/basicnanoclient.egg-info/requires.txt
--rw-r--r--   0 nate       (501) staff       (20)       16 2023-07-28 03:13:05.000000 basicnanoclient-0.0.7/basicnanoclient.egg-info/top_level.txt
--rw-r--r--   0 nate       (501) staff       (20)      738 2023-07-28 03:12:47.000000 basicnanoclient-0.0.7/pyproject.toml
--rw-r--r--   0 nate       (501) staff       (20)       38 2023-07-28 03:13:05.811654 basicnanoclient-0.0.7/setup.cfg
--rw-r--r--   0 nate       (501) staff       (20)     1034 2023-07-28 03:08:55.000000 basicnanoclient-0.0.7/setup.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-29 16:21:41.929917 basicnanoclient-0.1.0/
+-rw-r--r--   0 nate       (501) staff       (20)     1211 2023-07-28 01:29:38.000000 basicnanoclient-0.1.0/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)     2762 2023-07-29 16:21:41.929803 basicnanoclient-0.1.0/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)      844 2023-07-28 01:29:38.000000 basicnanoclient-0.1.0/README.md
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-29 16:21:41.928882 basicnanoclient-0.1.0/basicnanoclient/
+-rw-r--r--   0 nate       (501) staff       (20)      104 2023-07-29 16:21:05.000000 basicnanoclient-0.1.0/basicnanoclient/__init__.py
+-rw-r--r--   0 nate       (501) staff       (20)    10659 2023-07-29 15:46:06.000000 basicnanoclient-0.1.0/basicnanoclient/nano.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-29 16:21:41.929630 basicnanoclient-0.1.0/basicnanoclient.egg-info/
+-rw-r--r--   0 nate       (501) staff       (20)     2762 2023-07-29 16:21:41.000000 basicnanoclient-0.1.0/basicnanoclient.egg-info/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)      287 2023-07-29 16:21:41.000000 basicnanoclient-0.1.0/basicnanoclient.egg-info/SOURCES.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-29 16:21:41.000000 basicnanoclient-0.1.0/basicnanoclient.egg-info/dependency_links.txt
+-rw-r--r--   0 nate       (501) staff       (20)       60 2023-07-29 16:21:41.000000 basicnanoclient-0.1.0/basicnanoclient.egg-info/requires.txt
+-rw-r--r--   0 nate       (501) staff       (20)       16 2023-07-29 16:21:41.000000 basicnanoclient-0.1.0/basicnanoclient.egg-info/top_level.txt
+-rw-r--r--   0 nate       (501) staff       (20)      738 2023-07-29 16:20:59.000000 basicnanoclient-0.1.0/pyproject.toml
+-rw-r--r--   0 nate       (501) staff       (20)       38 2023-07-29 16:21:41.929950 basicnanoclient-0.1.0/setup.cfg
+-rw-r--r--   0 nate       (501) staff       (20)     1034 2023-07-28 03:08:55.000000 basicnanoclient-0.1.0/setup.py
```

### Comparing `basicnanoclient-0.0.7/LICENSE` & `basicnanoclient-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `basicnanoclient-0.0.7/PKG-INFO` & `basicnanoclient-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicnanoclient
-Version: 0.0.7
+Version: 0.1.0
 Summary: Nano RPC python client
 Home-page: https://github.com/nanoswap/basicnanoclient
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

### Comparing `basicnanoclient-0.0.7/README.md` & `basicnanoclient-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `basicnanoclient-0.0.7/basicnanoclient/nano.py` & `basicnanoclient-0.1.0/basicnanoclient/nano.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 __package__ = "basicnanoclient"
 
 import subprocess
 import uuid
-import secrets
 from typing import Any, Dict
 
 import requests
 
 rpc_network: str = "http://127.0.0.1:17076"
 session: requests.Session = requests.Session()
 
@@ -21,23 +20,14 @@
     ```
     """
 
     def __init__(self, rpc_network: str) -> None:
         """Constructor."""
         self.rpc_network = rpc_network
 
-    def generate_private_key(self) -> str:
-        """Generate a private key using the /dev/urandom command.
-
-        Returns:
-            The generated key
-        """
-        return secrets.token_hex(32)  # 32 bytes = 64 hexadecimal characters
-
-
     def key_expand(self, key: str) -> Dict[str, Any]:
         """Expands a given Nano private key into a public key
         and account address.
 
         Args:
             key (str): A 64-character hexadecimal string representing the
                 Nano private key.
```

### Comparing `basicnanoclient-0.0.7/basicnanoclient.egg-info/PKG-INFO` & `basicnanoclient-0.1.0/basicnanoclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicnanoclient
-Version: 0.0.7
+Version: 0.1.0
 Summary: Nano RPC python client
 Home-page: https://github.com/nanoswap/basicnanoclient
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

### Comparing `basicnanoclient-0.0.7/pyproject.toml` & `basicnanoclient-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 show_missing = true
 
 [build-system]
 requires = ["setuptools", "wheel", "requests"]
 
 [project]
 name = "basicnanoclient"
-version = "0.0.7"
+version = "0.1.0"
 description = "Nano RPC python client"
 urls = {'Bug Tracker' = 'https://github.com/nanoswap/basicnanoclient/issues'}
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: The Unlicense (Unlicense)'
 ]
 authors = [{'name' = 'Nathaniel Schultz', 'email' = 'nate@nanoswap.finance'}]
```

### Comparing `basicnanoclient-0.0.7/setup.py` & `basicnanoclient-0.1.0/setup.py`

 * *Files identical despite different names*

