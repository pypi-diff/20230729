# Comparing `tmp/nanohelp-0.1.4.tar.gz` & `tmp/nanohelp-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanohelp-0.1.4.tar", max compression
+gzip compressed data, was "nanohelp-0.1.5.tar", max compression
```

## Comparing `nanohelp-0.1.4.tar` & `nanohelp-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.1.4/LICENSE
--rw-r--r--   0        0        0     1189 2023-07-29 16:16:01.618674 nanohelp-0.1.4/README.md
--rw-r--r--   0        0        0      218 2023-07-29 19:36:19.034326 nanohelp-0.1.4/nanohelp/__init__.py
--rw-r--r--   0        0        0     5170 2023-07-29 19:35:28.734277 nanohelp-0.1.4/nanohelp/secret.py
--rw-r--r--   0        0        0     4403 2023-07-29 19:11:09.309954 nanohelp-0.1.4/nanohelp/wallet.py
--rw-r--r--   0        0        0      447 2023-07-29 19:36:13.251222 nanohelp-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 nanohelp-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1189 2023-07-29 16:16:01.618674 nanohelp-0.1.5/README.md
+-rw-r--r--   0        0        0      218 2023-07-29 19:44:59.003710 nanohelp-0.1.5/nanohelp/__init__.py
+-rw-r--r--   0        0        0     5170 2023-07-29 19:35:28.734277 nanohelp-0.1.5/nanohelp/secret.py
+-rw-r--r--   0        0        0     4516 2023-07-29 19:44:44.557934 nanohelp-0.1.5/nanohelp/wallet.py
+-rw-r--r--   0        0        0      447 2023-07-29 19:44:54.931158 nanohelp-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 nanohelp-0.1.5/PKG-INFO
```

### Comparing `nanohelp-0.1.4/LICENSE` & `nanohelp-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.4/README.md` & `nanohelp-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.4/nanohelp/secret.py` & `nanohelp-0.1.5/nanohelp/secret.py`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.4/nanohelp/wallet.py` & `nanohelp-0.1.5/nanohelp/wallet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from basicnanoclient.nano import BasicNanoClient
 from typing import List, Tuple, Optional, Self
 import logging
+import os
 
 from nanohelp.secret import SecretManager
 
 LOG = logging.getLogger(__name__)
-logging.basicConfig(level=logging.INFO)
+logging.basicConfig(level=logging.DEBUG)
 
 
 class WalletManager:
     """Business logic to abstract the raw nano node RPC logic.
 
     This class is responsible for creating wallets, adding accounts to wallets,
     and making transactions.
@@ -22,14 +23,15 @@
 
         Params:
             - node_address: the address of the node to connect to.
                 Defaults to the local node at port 17076.
 
         """
         self.client = BasicNanoClient(node_address)
+        LOG.debug("Google Application Credentials: %s", os.environ['GOOGLE_APPLICATION_CREDENTIALS'])
         self.secret_manager = secret_manager
 
     def create_wallet(self: Self, project: str, name: str) -> Optional[Tuple[str, str]]:
         """Generate a new private key and create a new wallet.
 
         Params:
             - project: the project to store the secret in
```

### Comparing `nanohelp-0.1.4/PKG-INFO` & `nanohelp-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanohelp
-Version: 0.1.4
+Version: 0.1.5
 Summary: Business logic to abstract the raw nano node RPC logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
```

