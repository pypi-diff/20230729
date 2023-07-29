# Comparing `tmp/nanohelp-0.0.6.tar.gz` & `tmp/nanohelp-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanohelp-0.0.6.tar", max compression
+gzip compressed data, was "nanohelp-0.0.8.tar", max compression
```

## Comparing `nanohelp-0.0.6.tar` & `nanohelp-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.0.6/LICENSE
--rw-r--r--   0        0        0      175 2023-07-28 02:45:10.243651 nanohelp-0.0.6/README.md
--rw-r--r--   0        0        0      176 2023-07-28 03:14:29.634894 nanohelp-0.0.6/nanohelp/__init__.py
--rw-r--r--   0        0        0     3450 2023-07-28 02:55:07.370199 nanohelp-0.0.6/nanohelp/wallet.py
--rw-r--r--   0        0        0      447 2023-07-28 03:14:24.428041 nanohelp-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 nanohelp-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.0.8/LICENSE
+-rw-r--r--   0        0        0      175 2023-07-28 02:45:10.243651 nanohelp-0.0.8/README.md
+-rw-r--r--   0        0        0      176 2023-07-29 15:26:24.281654 nanohelp-0.0.8/nanohelp/__init__.py
+-rw-r--r--   0        0        0     4095 2023-07-29 15:25:28.035588 nanohelp-0.0.8/nanohelp/wallet.py
+-rw-r--r--   0        0        0      447 2023-07-29 15:26:20.692752 nanohelp-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 nanohelp-0.0.8/PKG-INFO
```

### Comparing `nanohelp-0.0.6/LICENSE` & `nanohelp-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nanohelp-0.0.6/nanohelp/wallet.py` & `nanohelp-0.0.8/nanohelp/wallet.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,114 @@
 from basicnanoclient.nano import BasicNanoClient
-import time
+from typing import List, Tuple, Optional, Self
+import logging
+
+LOG = logging.getLogger(__name__)
+logging.basicConfig(level=logging.INFO)
+
 
 class WalletManager:
-    def __init__(self, node_address):
-        self.client = BasicNanoClient(node_address)
-        self.transaction_history = {}
+    """Business logic to abstract the raw nano node RPC logic.
 
-    def create_wallet(self):
+    This class is responsible for creating wallets, adding accounts to wallets,
+    and making transactions.
+    """
+    def __init__(
+            self: Self,
+            node_address: str = "http://127.0.0.1:17076") -> None:
+        """Initialize the wallet manager.
+
+        Params:
+            - node_address: the address of the node to connect to.
+                Defaults to the local node at port 17076.
         """
-        This method abstracts the process of creating a new wallet.
+        self.client = BasicNanoClient(node_address)
+
+    def create_wallet(self: Self) -> Optional[Tuple[str, str, str]]:
+        """Create a new wallet.
 
         Returns: a tuple containing wallet_id, account_address and private_key
         """
         try:
             private_key = self.client.generate_private_key()
             wallet_id = self.client.wallet_create(private_key)['wallet']
             account_address = self.client.accounts_create(wallet_id)['accounts'][0]
         except Exception as e:
-            print(f"Failed to create wallet: {e}")
+            LOG.error(f"Failed to create wallet: {e}")
+            LOG.exception(e)
             return None
 
         return wallet_id, account_address, private_key
 
-    def add_account_to_wallet(self, wallet_id):
-        """
-        Add a new account to an existing wallet.
+    def add_account_to_wallet(self: Self, wallet_id: str) -> Optional[str]:
+        """Add a new account to an existing wallet.
+
+        Params:
+            - wallet_id: the wallet id to add the account to
         """
         try:
             account_address = self.client.accounts_create(wallet_id)['accounts'][0]
         except Exception as e:
-            print(f"Failed to add account to wallet {wallet_id}: {e}")
+            LOG.error(f"Failed to add account to wallet {wallet_id}: {e}")
+            LOG.exception(e)
             return None
 
         return account_address
 
-    def make_transaction(self, source_wallet, source_account, destination_account, amount, private_key, retries=3):
-        """
-        This method abstracts the process of making a transaction.
+    def make_transaction(
+            self: Self,
+            source_wallet: str,
+            source_account: str,
+            destination_account: str,
+            amount: int,
+            private_key: str,
+            retries: int = 3) -> Optional[str]:
+        """Make a transaction.
 
         Params:
             - source_wallet: the wallet id of the source account
             - source_account: the address of the source account
             - destination_account: the address of the destination account
             - amount: the amount of Nano to be sent
             - private_key: the private key of the source account
-            - retries: the number of times to retry the transaction in case of failure
+            - retries: the number of times to retry the transaction in case of failure  # noqa: E501
 
         Returns: the transaction block
         """
         if retries <= 0:
             raise ValueError("Transaction failed after multiple retries")
 
         try:
             account_list = self.client.account_list(source_wallet)['accounts']
             if source_account not in account_list:
-                raise ValueError(f"Account {source_account} doesn't belong to wallet {source_wallet}")
+                raise ValueError(f"Account {source_account} doesn't belong to wallet {source_wallet}")  # noqa: E501
 
             # Check if the account has enough balance
             balance = self.client.account_info(source_account)['balance']
             if int(balance) < amount:
-                raise ValueError(f"Account {source_account} has insufficient balance")
+                raise ValueError(f"Account {source_account} has insufficient balance")  # noqa: E501
 
             # Make the transaction
-            transaction = self.client.send(source_wallet, source_account, destination_account, amount, private_key)
+            transaction = self.client.send(
+                source_wallet,
+                source_account,
+                destination_account,
+                amount,
+                private_key
+            )
+            LOG.info(f"Transaction successful: {transaction}")
             block = transaction.get('block')
-
-            # Update transaction history
-            if source_account not in self.transaction_history:
-                self.transaction_history[source_account] = []
-            self.transaction_history[source_account].append((destination_account, amount, block))
-
+            LOG.info(f"Block: {block}")
             return block
 
         except Exception as e:
-            print(f"Transaction failed: {e}")
+            LOG.error(f"Transaction failed: {e}")
+            LOG.exception(e)
             # TODO: redo retry to use decorator
-            return self.make_transaction(source_wallet, source_account, destination_account, amount, private_key, retries-1)
-
-    def get_transaction_history(self, account):
-        """
-        Returns a list of transactions made by the account
-        """
-        if account not in self.transaction_history:
-            return []
-
-        return self.transaction_history[account]
+            return self.make_transaction(
+                source_wallet,
+                source_account,
+                destination_account,
+                amount,
+                private_key,
+                retries - 1
+            )
```

### Comparing `nanohelp-0.0.6/PKG-INFO` & `nanohelp-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanohelp
-Version: 0.0.6
+Version: 0.0.8
 Summary: Business logic to abstract the raw nano node RPC logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
```

