# Comparing `tmp/nanohelp-0.1.5.tar.gz` & `tmp/nanohelp-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanohelp-0.1.5.tar", max compression
+gzip compressed data, was "nanohelp-0.1.7.tar", max compression
```

## Comparing `nanohelp-0.1.5.tar` & `nanohelp-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.1.5/LICENSE
--rw-r--r--   0        0        0     1189 2023-07-29 16:16:01.618674 nanohelp-0.1.5/README.md
--rw-r--r--   0        0        0      218 2023-07-29 19:44:59.003710 nanohelp-0.1.5/nanohelp/__init__.py
--rw-r--r--   0        0        0     5170 2023-07-29 19:35:28.734277 nanohelp-0.1.5/nanohelp/secret.py
--rw-r--r--   0        0        0     4516 2023-07-29 19:44:44.557934 nanohelp-0.1.5/nanohelp/wallet.py
--rw-r--r--   0        0        0      447 2023-07-29 19:44:54.931158 nanohelp-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 nanohelp-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1189 2023-07-29 16:16:01.618674 nanohelp-0.1.7/README.md
+-rw-r--r--   0        0        0      218 2023-07-29 20:16:30.635294 nanohelp-0.1.7/nanohelp/__init__.py
+-rw-r--r--   0        0        0     6586 2023-07-29 20:11:07.958270 nanohelp-0.1.7/nanohelp/secret.py
+-rw-r--r--   0        0        0     4516 2023-07-29 19:44:44.557934 nanohelp-0.1.7/nanohelp/wallet.py
+-rw-r--r--   0        0        0      447 2023-07-29 20:16:27.717444 nanohelp-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 nanohelp-0.1.7/PKG-INFO
```

### Comparing `nanohelp-0.1.5/LICENSE` & `nanohelp-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.5/README.md` & `nanohelp-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.5/nanohelp/secret.py` & `nanohelp-0.1.7/nanohelp/secret.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,48 +45,14 @@
         Raises:
             - RuntimeError: If unable to store the secret.
         """
         private_key = self.generate_private_key()
         self.store_private_key(project, name, private_key)
         return private_key
 
-    def store_private_key(
-            self: Self,
-            project: str,
-            name: str,
-            private_key: str) -> None:
-        """Storing a private key based on a index in Google Secret Manager.
-
-        Params:
-            - project: the project to store the secret in
-            - name: the name of the secret
-            - private_key: the private key to store
-
-        Raises:
-            - RuntimeError: If unable to store the secret.
-        """
-        try:
-            # Create a new secret version
-            secret = self.secret_manager_client.secret_path(
-                project,
-                name,
-            )
-
-            # Add the secret version
-            self.secret_manager_client.add_secret_version(
-                parent=secret,
-                payload=secretmanager.SecretPayload(
-                    data=private_key.encode('UTF-8')
-                )
-            )
-        except Exception as e:
-            LOG.error(f"Failed to store private key for {name}: {e}")
-            LOG.exception(e)
-            raise RuntimeError("Unable to store secret: {}".format(e)) from e
-
     def get_private_key(
             self: Self,
             project: str,
             name: str,
             version: str = "latest") -> str:
         """Fetch the private key from Google Secret Manager.
 
@@ -117,14 +83,89 @@
 
             return payload
         except Exception as e:
             LOG.error(f"Failed to retrieve private key for {name}: {e}")
             LOG.exception(e)
             raise RuntimeError("Unable to retrieve secret: {}".format(e)) from e
 
+    def create_secret(
+            self: Self,
+            project: str,
+            name: str) -> None:
+        """Create a new secret.
+
+        Params:
+            - project: the project to create the secret in
+            - name: the name of the secret
+
+        Raises:
+            - RuntimeError: If unable to create the secret.
+        """
+        try:
+            # Define the parent project
+            parent = f"projects/{project}"
+
+            # Create a new secret
+            response = self.secret_manager_client.create_secret(
+                parent=parent,
+                secret_id=name,
+                secret=secretmanager.Secret(
+                    replication=secretmanager.Replication(
+                        automatic=secretmanager.Replication.Automatic()
+                    )
+                ),
+            )
+        except Exception as e:
+            LOG.error(f"Failed to create secret {name}: {e}")
+            LOG.exception(e)
+            raise RuntimeError("Unable to create secret: {}".format(e)) from e
+
+    def store_private_key(
+            self: Self,
+            project: str,
+            name: str,
+            private_key: str) -> None:
+        """Storing a private key based on a index in Google Secret Manager.
+
+        Params:
+            - project: the project to store the secret in
+            - name: the name of the secret
+            - private_key: the private key to store
+
+        Raises:
+            - RuntimeError: If unable to store the secret.
+        """
+        try:
+            # Define the parent project
+            parent = f"projects/{project}"
+            
+            # Check if the secret exists
+            secrets = self.secret_manager_client.list_secrets(parent)
+            if name not in [secret.name for secret in secrets]:
+                # If the secret doesn't exist, create it
+                self.create_secret(project, name)
+
+            # Create a new secret version
+            secret = self.secret_manager_client.secret_path(
+                project,
+                name,
+            )
+
+            # Add the secret version
+            self.secret_manager_client.add_secret_version(
+                parent=secret,
+                payload=secretmanager.SecretPayload(
+                    data=private_key.encode('UTF-8')
+                )
+            )
+        except Exception as e:
+            LOG.error(f"Failed to store private key for {name}: {e}")
+            LOG.exception(e)
+            raise RuntimeError("Unable to store secret: {}".format(e)) from e
+
     def rotate_private_key(
             self: Self,
             project: str,
             name: str,
             new_key: str) -> None:
         """Rotate a private key, replacing it with a new version.
```

### Comparing `nanohelp-0.1.5/nanohelp/wallet.py` & `nanohelp-0.1.7/nanohelp/wallet.py`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.5/PKG-INFO` & `nanohelp-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanohelp
-Version: 0.1.5
+Version: 0.1.7
 Summary: Business logic to abstract the raw nano node RPC logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
```

