# Comparing `tmp/nanohelp-0.1.1.tar.gz` & `tmp/nanohelp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanohelp-0.1.1.tar", max compression
+gzip compressed data, was "nanohelp-0.1.2.tar", max compression
```

## Comparing `nanohelp-0.1.1.tar` & `nanohelp-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.1.1/LICENSE
--rw-r--r--   0        0        0     1189 2023-07-29 16:16:01.618674 nanohelp-0.1.1/README.md
--rw-r--r--   0        0        0      218 2023-07-29 17:32:49.555004 nanohelp-0.1.1/nanohelp/__init__.py
--rw-r--r--   0        0        0     4443 2023-07-29 17:37:52.340789 nanohelp-0.1.1/nanohelp/secret.py
--rw-r--r--   0        0        0     4322 2023-07-29 17:32:30.791254 nanohelp-0.1.1/nanohelp/wallet.py
--rw-r--r--   0        0        0      447 2023-07-29 17:32:45.592084 nanohelp-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 nanohelp-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1189 2023-07-29 16:16:01.618674 nanohelp-0.1.2/README.md
+-rw-r--r--   0        0        0      218 2023-07-29 17:55:56.231846 nanohelp-0.1.2/nanohelp/__init__.py
+-rw-r--r--   0        0        0     4820 2023-07-29 17:55:31.021995 nanohelp-0.1.2/nanohelp/secret.py
+-rw-r--r--   0        0        0     4322 2023-07-29 17:32:30.791254 nanohelp-0.1.2/nanohelp/wallet.py
+-rw-r--r--   0        0        0      447 2023-07-29 17:55:53.015079 nanohelp-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 nanohelp-0.1.2/PKG-INFO
```

### Comparing `nanohelp-0.1.1/LICENSE` & `nanohelp-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.1/README.md` & `nanohelp-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.1/nanohelp/secret.py` & `nanohelp-0.1.2/nanohelp/secret.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,32 +19,36 @@
 
         Returns:
             The generated key
         """
         return secrets.token_hex(32)  # 32 bytes = 64 hexadecimal characters
 
 
-    def generate_and_store_private_key(self: Self, user: str) -> str:
+    def generate_and_store_private_key(
+            self: Self,
+            project: str,
+            name: str) -> str:
         """This method generates a private key and stores it in Google Secret Manager.
 
         Params:
-            - user: the user to store the private key for
+            - project: the project to store the secret in
+            - name: the secret name to store the private key for
 
         Raises:
             - RuntimeError: If unable to store the secret.
         """
         private_key = self.generate_private_key()
-        self.store_private_key(user, private_key)
+        self.store_private_key(project, name, private_key)
         return private_key
 
     def store_private_key(
             self: Self,
             project: str,
             name: str,
-            private_key: str,):
+            private_key: str) -> None:
         """Storing a private key based on a index in Google Secret Manager.
 
         Params:
             - project: the project to store the secret in
             - name: the name of the secret
             - private_key: the private key to store
 
@@ -86,46 +90,56 @@
             - private_key: the private key for the user
 
         Raises:
             - RuntimeError: If unable to retrieve the secret.
         """
         try:
             # Build the resource name of the secret version.
-            name = self.secret_manager_client.secret_version_path(project, name, version)
+            name = self.secret_manager_client.secret_version_path(
+                project,
+                name,
+                version
+            )
 
             # Access the secret version.
             response = self.secret_manager_client.access_secret_version(name)
 
             # Get the payload of the secret.
             payload = response.payload.data.decode('UTF-8')
 
             return payload
         except Exception as e:
             LOG.error(f"Failed to retrieve private key for {name}: {e}")
             LOG.exception(e)
             raise RuntimeError("Unable to retrieve secret: {}".format(e)) from e
 
-    def rotate_private_key(self: Self, name: str):
+    def rotate_private_key(
+            self: Self,
+            project: str,
+            name: str,
+            new_key: str) -> None:
         """Rotate a private key, replacing it with a new version.
 
         **Caution**: the old private key will be lost, and if it is used for
         anything (ex: a crypto wallet), it will no longer work with the new key.
 
         This will generate a new private key and store it in Google Secret Manager,
         effectively replacing the old one.
 
         Params:
-            - name: the name of the secret to rotate the private key for
+            - project: the project to store the secret in
+            - name: the name of the secret
+            - new_key: the new private key to store
 
         Returns:
             - The new private key that was generated.
 
         Raises:
             - RuntimeError: If unable to generate and store the new private key.
         """
         raise NotImplementedError("No use case found for rotating private keys (using this for crypto wallets is a bad idea)")
 
         try:
             # Generate and store a new private key
-            return self.generate_and_store_private_key(name)
+            return self.generate_and_store_private_key(project, name, new_key)
         except Exception as e:
             raise RuntimeError(f"Unable to rotate private key: {e}") from e
```

### Comparing `nanohelp-0.1.1/nanohelp/wallet.py` & `nanohelp-0.1.2/nanohelp/wallet.py`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.1/PKG-INFO` & `nanohelp-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanohelp
-Version: 0.1.1
+Version: 0.1.2
 Summary: Business logic to abstract the raw nano node RPC logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
```

