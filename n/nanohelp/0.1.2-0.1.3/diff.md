# Comparing `tmp/nanohelp-0.1.2.tar.gz` & `tmp/nanohelp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanohelp-0.1.2.tar", max compression
+gzip compressed data, was "nanohelp-0.1.3.tar", max compression
```

## Comparing `nanohelp-0.1.2.tar` & `nanohelp-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.1.2/LICENSE
--rw-r--r--   0        0        0     1189 2023-07-29 16:16:01.618674 nanohelp-0.1.2/README.md
--rw-r--r--   0        0        0      218 2023-07-29 17:55:56.231846 nanohelp-0.1.2/nanohelp/__init__.py
--rw-r--r--   0        0        0     4820 2023-07-29 17:55:31.021995 nanohelp-0.1.2/nanohelp/secret.py
--rw-r--r--   0        0        0     4322 2023-07-29 17:32:30.791254 nanohelp-0.1.2/nanohelp/wallet.py
--rw-r--r--   0        0        0      447 2023-07-29 17:55:53.015079 nanohelp-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 nanohelp-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1189 2023-07-29 16:16:01.618674 nanohelp-0.1.3/README.md
+-rw-r--r--   0        0        0      218 2023-07-29 19:12:18.551156 nanohelp-0.1.3/nanohelp/__init__.py
+-rw-r--r--   0        0        0     4820 2023-07-29 17:55:31.021995 nanohelp-0.1.3/nanohelp/secret.py
+-rw-r--r--   0        0        0     4403 2023-07-29 19:11:09.309954 nanohelp-0.1.3/nanohelp/wallet.py
+-rw-r--r--   0        0        0      447 2023-07-29 19:12:15.350925 nanohelp-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 nanohelp-0.1.3/PKG-INFO
```

### Comparing `nanohelp-0.1.2/LICENSE` & `nanohelp-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.2/README.md` & `nanohelp-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.2/nanohelp/secret.py` & `nanohelp-0.1.3/nanohelp/secret.py`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.2/nanohelp/wallet.py` & `nanohelp-0.1.3/nanohelp/wallet.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,25 +24,26 @@
             - node_address: the address of the node to connect to.
                 Defaults to the local node at port 17076.
 
         """
         self.client = BasicNanoClient(node_address)
         self.secret_manager = secret_manager
 
-    def create_wallet(self: Self, name: str) -> Optional[Tuple[str, str]]:
+    def create_wallet(self: Self, project: str, name: str) -> Optional[Tuple[str, str]]:
         """Generate a new private key and create a new wallet.
 
         Params:
+            - project: the project to store the secret in
             - name: the name of the wallet to create
 
         Returns: a tuple containing wallet_id and account_address
         """
         try:
             wallet_id = self.client.wallet_create(
-                self.secret_manager.generate_and_store_private_key(name)
+                self.secret_manager.generate_and_store_private_key(project, name)
             )['wallet']
             account_address = self.client.accounts_create(wallet_id)['accounts'][0]
         except Exception as e:
             LOG.error(f"Failed to create wallet: {e}")
             LOG.exception(e)
             return None
```

### Comparing `nanohelp-0.1.2/PKG-INFO` & `nanohelp-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanohelp
-Version: 0.1.2
+Version: 0.1.3
 Summary: Business logic to abstract the raw nano node RPC logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
```

