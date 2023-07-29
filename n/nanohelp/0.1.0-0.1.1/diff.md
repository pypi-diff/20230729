# Comparing `tmp/nanohelp-0.1.0.tar.gz` & `tmp/nanohelp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanohelp-0.1.0.tar", max compression
+gzip compressed data, was "nanohelp-0.1.1.tar", max compression
```

## Comparing `nanohelp-0.1.0.tar` & `nanohelp-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.1.0/LICENSE
--rw-r--r--   0        0        0     1189 2023-07-29 16:16:01.618674 nanohelp-0.1.0/README.md
--rw-r--r--   0        0        0      176 2023-07-29 16:17:17.445101 nanohelp-0.1.0/nanohelp/__init__.py
--rw-r--r--   0        0        0     4938 2023-07-29 16:08:52.782706 nanohelp-0.1.0/nanohelp/secret.py
--rw-r--r--   0        0        0     4330 2023-07-29 16:09:59.613284 nanohelp-0.1.0/nanohelp/wallet.py
--rw-r--r--   0        0        0      447 2023-07-29 16:17:23.116606 nanohelp-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 nanohelp-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1189 2023-07-29 16:16:01.618674 nanohelp-0.1.1/README.md
+-rw-r--r--   0        0        0      218 2023-07-29 17:32:49.555004 nanohelp-0.1.1/nanohelp/__init__.py
+-rw-r--r--   0        0        0     4443 2023-07-29 17:37:52.340789 nanohelp-0.1.1/nanohelp/secret.py
+-rw-r--r--   0        0        0     4322 2023-07-29 17:32:30.791254 nanohelp-0.1.1/nanohelp/wallet.py
+-rw-r--r--   0        0        0      447 2023-07-29 17:32:45.592084 nanohelp-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 nanohelp-0.1.1/PKG-INFO
```

### Comparing `nanohelp-0.1.0/LICENSE` & `nanohelp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.0/README.md` & `nanohelp-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.0/nanohelp/secret.py` & `nanohelp-0.1.1/nanohelp/secret.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,45 +36,37 @@
         self.store_private_key(user, private_key)
         return private_key
 
     def store_private_key(
             self: Self,
             project: str,
             name: str,
-            private_key: str,
-            version: str = 'latest',
-            rotation_time: int = 60 * 60 * 24 * 30):
+            private_key: str,):
         """Storing a private key based on a index in Google Secret Manager.
 
         Params:
             - project: the project to store the secret in
             - name: the name of the secret
             - private_key: the private key to store
-            - version: the version of the secret. Defaults to 'latest'.
-            - rotation_time: the time in seconds until the secret should be rotated.
-                Defaults to 30 days. (Not enforced by Google Secret Manager)
 
         Raises:
             - RuntimeError: If unable to store the secret.
         """
         try:
             # Create a new secret version
-            secret = self.secret_manager_client.secret_version_path(
+            secret = self.secret_manager_client.secret_path(
                 project,
                 name,
-                version
             )
 
             # Add the secret version
-            self.secret_manager_client.add_secret_version_with_rotation(
-                parent=secret, payload={'key': private_key},
-                rotation_schedule=secretmanager.types.RotationSchedule(
-                    next_rotation_time={
-                        'seconds': int(time.time() + rotation_time)
-                    }
+            self.secret_manager_client.add_secret_version(
+                parent=secret,
+                payload=secretmanager.SecretPayload(
+                    data=private_key.encode('UTF-8')
                 )
             )
         except Exception as e:
             LOG.error(f"Failed to store private key for {name}: {e}")
             LOG.exception(e)
             raise RuntimeError("Unable to store secret: {}".format(e)) from e
```

### Comparing `nanohelp-0.1.0/nanohelp/wallet.py` & `nanohelp-0.1.1/nanohelp/wallet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from basicnanoclient.nano import BasicNanoClient
 from typing import List, Tuple, Optional, Self
 import logging
 
-from nanohelp.secret_manager import SecretManager
+from nanohelp.secret import SecretManager
 
 LOG = logging.getLogger(__name__)
 logging.basicConfig(level=logging.INFO)
 
 
 class WalletManager:
     """Business logic to abstract the raw nano node RPC logic.
```

### Comparing `nanohelp-0.1.0/PKG-INFO` & `nanohelp-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanohelp
-Version: 0.1.0
+Version: 0.1.1
 Summary: Business logic to abstract the raw nano node RPC logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
```

