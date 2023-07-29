# Comparing `tmp/nanohelp-0.0.8.tar.gz` & `tmp/nanohelp-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanohelp-0.0.8.tar", max compression
+gzip compressed data, was "nanohelp-0.1.0.tar", max compression
```

## Comparing `nanohelp-0.0.8.tar` & `nanohelp-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.0.8/LICENSE
--rw-r--r--   0        0        0      175 2023-07-28 02:45:10.243651 nanohelp-0.0.8/README.md
--rw-r--r--   0        0        0      176 2023-07-29 15:26:24.281654 nanohelp-0.0.8/nanohelp/__init__.py
--rw-r--r--   0        0        0     4095 2023-07-29 15:25:28.035588 nanohelp-0.0.8/nanohelp/wallet.py
--rw-r--r--   0        0        0      447 2023-07-29 15:26:20.692752 nanohelp-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 nanohelp-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1189 2023-07-29 16:16:01.618674 nanohelp-0.1.0/README.md
+-rw-r--r--   0        0        0      176 2023-07-29 16:17:17.445101 nanohelp-0.1.0/nanohelp/__init__.py
+-rw-r--r--   0        0        0     4938 2023-07-29 16:08:52.782706 nanohelp-0.1.0/nanohelp/secret.py
+-rw-r--r--   0        0        0     4330 2023-07-29 16:09:59.613284 nanohelp-0.1.0/nanohelp/wallet.py
+-rw-r--r--   0        0        0      447 2023-07-29 16:17:23.116606 nanohelp-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 nanohelp-0.1.0/PKG-INFO
```

### Comparing `nanohelp-0.0.8/LICENSE` & `nanohelp-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nanohelp-0.0.8/nanohelp/wallet.py` & `nanohelp-0.1.0/nanohelp/wallet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,56 @@
 from basicnanoclient.nano import BasicNanoClient
 from typing import List, Tuple, Optional, Self
 import logging
 
+from nanohelp.secret_manager import SecretManager
+
 LOG = logging.getLogger(__name__)
 logging.basicConfig(level=logging.INFO)
 
 
 class WalletManager:
     """Business logic to abstract the raw nano node RPC logic.
 
     This class is responsible for creating wallets, adding accounts to wallets,
     and making transactions.
     """
     def __init__(
             self: Self,
+            secret_manager: SecretManager,
             node_address: str = "http://127.0.0.1:17076") -> None:
         """Initialize the wallet manager.
 
         Params:
             - node_address: the address of the node to connect to.
                 Defaults to the local node at port 17076.
+
         """
         self.client = BasicNanoClient(node_address)
+        self.secret_manager = secret_manager
 
-    def create_wallet(self: Self) -> Optional[Tuple[str, str, str]]:
-        """Create a new wallet.
+    def create_wallet(self: Self, name: str) -> Optional[Tuple[str, str]]:
+        """Generate a new private key and create a new wallet.
+
+        Params:
+            - name: the name of the wallet to create
 
-        Returns: a tuple containing wallet_id, account_address and private_key
+        Returns: a tuple containing wallet_id and account_address
         """
         try:
-            private_key = self.client.generate_private_key()
-            wallet_id = self.client.wallet_create(private_key)['wallet']
+            wallet_id = self.client.wallet_create(
+                self.secret_manager.generate_and_store_private_key(name)
+            )['wallet']
             account_address = self.client.accounts_create(wallet_id)['accounts'][0]
         except Exception as e:
             LOG.error(f"Failed to create wallet: {e}")
             LOG.exception(e)
             return None
 
-        return wallet_id, account_address, private_key
+        return wallet_id, account_address
 
     def add_account_to_wallet(self: Self, wallet_id: str) -> Optional[str]:
         """Add a new account to an existing wallet.
 
         Params:
             - wallet_id: the wallet id to add the account to
         """
```

