# Comparing `tmp/nanohelp-0.1.3.tar.gz` & `tmp/nanohelp-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanohelp-0.1.3.tar", max compression
+gzip compressed data, was "nanohelp-0.1.4.tar", max compression
```

## Comparing `nanohelp-0.1.3.tar` & `nanohelp-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.1.3/LICENSE
--rw-r--r--   0        0        0     1189 2023-07-29 16:16:01.618674 nanohelp-0.1.3/README.md
--rw-r--r--   0        0        0      218 2023-07-29 19:12:18.551156 nanohelp-0.1.3/nanohelp/__init__.py
--rw-r--r--   0        0        0     4820 2023-07-29 17:55:31.021995 nanohelp-0.1.3/nanohelp/secret.py
--rw-r--r--   0        0        0     4403 2023-07-29 19:11:09.309954 nanohelp-0.1.3/nanohelp/wallet.py
--rw-r--r--   0        0        0      447 2023-07-29 19:12:15.350925 nanohelp-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 nanohelp-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1189 2023-07-29 16:16:01.618674 nanohelp-0.1.4/README.md
+-rw-r--r--   0        0        0      218 2023-07-29 19:36:19.034326 nanohelp-0.1.4/nanohelp/__init__.py
+-rw-r--r--   0        0        0     5170 2023-07-29 19:35:28.734277 nanohelp-0.1.4/nanohelp/secret.py
+-rw-r--r--   0        0        0     4403 2023-07-29 19:11:09.309954 nanohelp-0.1.4/nanohelp/wallet.py
+-rw-r--r--   0        0        0      447 2023-07-29 19:36:13.251222 nanohelp-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 nanohelp-0.1.4/PKG-INFO
```

### Comparing `nanohelp-0.1.3/LICENSE` & `nanohelp-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.3/README.md` & `nanohelp-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.3/nanohelp/secret.py` & `nanohelp-0.1.4/nanohelp/secret.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 from typing import Self
 import time
 import secrets
 from google.cloud import secretmanager
 import logging
+import os
+from pathlib import Path
+from dotenv import load_dotenv
 
 LOG = logging.getLogger(__name__)
 logging.basicConfig(level=logging.INFO)
 
 
 class SecretManager:
     """Class to handle operations related to Google Cloud Secret Manager."""
 
     def __init__(self: Self):
+        """Initialize the secret manager.
+
+        The GOOGLE_APPLICATION_CREDENTIALS environment variable must be set to
+        the path to the service account key file (for google secret manager)
+        """
+        load_dotenv(Path(os.environ['SECRETS_PATH'] + "/.env.nanoswap"))
         self.secret_manager_client = secretmanager.SecretManagerServiceClient()
 
     def generate_private_key(self: Self) -> str:
         """Generate a private key using the /dev/urandom command.
 
         Returns:
             The generated key
```

### Comparing `nanohelp-0.1.3/nanohelp/wallet.py` & `nanohelp-0.1.4/nanohelp/wallet.py`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.3/PKG-INFO` & `nanohelp-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanohelp
-Version: 0.1.3
+Version: 0.1.4
 Summary: Business logic to abstract the raw nano node RPC logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
```

