# Comparing `tmp/liana-rpc-0.0.2.tar.gz` & `tmp/liana-rpc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liana-rpc-0.0.2.tar", last modified: Sat Jul 29 18:09:00 2023, max compression
+gzip compressed data, was "liana-rpc-0.0.3.tar", last modified: Sat Jul 29 20:52:38 2023, max compression
```

## Comparing `liana-rpc-0.0.2.tar` & `liana-rpc-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cc1       (1000) cc1       (1000)        0 2023-07-29 18:09:00.288139 liana-rpc-0.0.2/
--rw-rw-r--   0 cc1       (1000) cc1       (1000)     1528 2023-05-29 18:34:18.000000 liana-rpc-0.0.2/LICENCE
--rw-rw-r--   0 cc1       (1000) cc1       (1000)      498 2023-07-29 18:09:00.288139 liana-rpc-0.0.2/PKG-INFO
--rw-rw-r--   0 cc1       (1000) cc1       (1000)    27130 2023-07-27 03:11:49.000000 liana-rpc-0.0.2/README.md
-drwxrwxr-x   0 cc1       (1000) cc1       (1000)        0 2023-07-29 18:09:00.288139 liana-rpc-0.0.2/liana_rpc/
--rw-rw-r--   0 cc1       (1000) cc1       (1000)        0 2023-07-22 19:06:12.000000 liana-rpc-0.0.2/liana_rpc/__init__.py
--rw-rw-r--   0 cc1       (1000) cc1       (1000)    12314 2023-07-29 18:03:23.000000 liana-rpc-0.0.2/liana_rpc/liana_rpc.py
-drwxrwxr-x   0 cc1       (1000) cc1       (1000)        0 2023-07-29 18:09:00.288139 liana-rpc-0.0.2/liana_rpc/utils/
--rw-rw-r--   0 cc1       (1000) cc1       (1000)        0 2023-07-22 10:07:08.000000 liana-rpc-0.0.2/liana_rpc/utils/__init__.py
--rw-rw-r--   0 cc1       (1000) cc1       (1000)     5728 2023-07-23 18:43:50.000000 liana-rpc-0.0.2/liana_rpc/utils/rpc.py
-drwxrwxr-x   0 cc1       (1000) cc1       (1000)        0 2023-07-29 18:09:00.288139 liana-rpc-0.0.2/liana_rpc.egg-info/
--rw-rw-r--   0 cc1       (1000) cc1       (1000)      498 2023-07-29 18:09:00.000000 liana-rpc-0.0.2/liana_rpc.egg-info/PKG-INFO
--rw-rw-r--   0 cc1       (1000) cc1       (1000)      260 2023-07-29 18:09:00.000000 liana-rpc-0.0.2/liana_rpc.egg-info/SOURCES.txt
--rw-rw-r--   0 cc1       (1000) cc1       (1000)        1 2023-07-29 18:09:00.000000 liana-rpc-0.0.2/liana_rpc.egg-info/dependency_links.txt
--rw-rw-r--   0 cc1       (1000) cc1       (1000)       10 2023-07-29 18:09:00.000000 liana-rpc-0.0.2/liana_rpc.egg-info/top_level.txt
--rw-rw-r--   0 cc1       (1000) cc1       (1000)      688 2023-07-29 18:08:39.000000 liana-rpc-0.0.2/pyproject.toml
--rw-rw-r--   0 cc1       (1000) cc1       (1000)       38 2023-07-29 18:09:00.288139 liana-rpc-0.0.2/setup.cfg
+drwxrwxr-x   0 cc1       (1000) cc1       (1000)        0 2023-07-29 20:52:38.134391 liana-rpc-0.0.3/
+-rw-rw-r--   0 cc1       (1000) cc1       (1000)     1528 2023-05-29 18:34:18.000000 liana-rpc-0.0.3/LICENCE
+-rw-rw-r--   0 cc1       (1000) cc1       (1000)      498 2023-07-29 20:52:38.134391 liana-rpc-0.0.3/PKG-INFO
+-rw-rw-r--   0 cc1       (1000) cc1       (1000)    27130 2023-07-27 03:11:49.000000 liana-rpc-0.0.3/README.md
+drwxrwxr-x   0 cc1       (1000) cc1       (1000)        0 2023-07-29 20:52:38.134391 liana-rpc-0.0.3/liana_rpc/
+-rw-rw-r--   0 cc1       (1000) cc1       (1000)        0 2023-07-22 19:06:12.000000 liana-rpc-0.0.3/liana_rpc/__init__.py
+-rw-rw-r--   0 cc1       (1000) cc1       (1000)    12791 2023-07-29 20:49:45.000000 liana-rpc-0.0.3/liana_rpc/liana_rpc.py
+drwxrwxr-x   0 cc1       (1000) cc1       (1000)        0 2023-07-29 20:52:38.134391 liana-rpc-0.0.3/liana_rpc/utils/
+-rw-rw-r--   0 cc1       (1000) cc1       (1000)        0 2023-07-22 10:07:08.000000 liana-rpc-0.0.3/liana_rpc/utils/__init__.py
+-rw-rw-r--   0 cc1       (1000) cc1       (1000)     5728 2023-07-23 18:43:50.000000 liana-rpc-0.0.3/liana_rpc/utils/rpc.py
+drwxrwxr-x   0 cc1       (1000) cc1       (1000)        0 2023-07-29 20:52:38.134391 liana-rpc-0.0.3/liana_rpc.egg-info/
+-rw-rw-r--   0 cc1       (1000) cc1       (1000)      498 2023-07-29 20:52:38.000000 liana-rpc-0.0.3/liana_rpc.egg-info/PKG-INFO
+-rw-rw-r--   0 cc1       (1000) cc1       (1000)      260 2023-07-29 20:52:38.000000 liana-rpc-0.0.3/liana_rpc.egg-info/SOURCES.txt
+-rw-rw-r--   0 cc1       (1000) cc1       (1000)        1 2023-07-29 20:52:38.000000 liana-rpc-0.0.3/liana_rpc.egg-info/dependency_links.txt
+-rw-rw-r--   0 cc1       (1000) cc1       (1000)       10 2023-07-29 20:52:38.000000 liana-rpc-0.0.3/liana_rpc.egg-info/top_level.txt
+-rw-rw-r--   0 cc1       (1000) cc1       (1000)      688 2023-07-29 20:52:07.000000 liana-rpc-0.0.3/pyproject.toml
+-rw-rw-r--   0 cc1       (1000) cc1       (1000)       38 2023-07-29 20:52:38.134391 liana-rpc-0.0.3/setup.cfg
```

### Comparing `liana-rpc-0.0.2/LICENCE` & `liana-rpc-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `liana-rpc-0.0.2/README.md` & `liana-rpc-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `liana-rpc-0.0.2/liana_rpc/liana_rpc.py` & `liana-rpc-0.0.3/liana_rpc/liana_rpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,59 +24,71 @@
             for i in out:
                 liana_sockets.append("/".join(i.split(' ')[-1].split('/')[:-1]) + '/lianad_rpc')
             return liana_sockets
 
     return []
 
 
-def psbt_to_txid(psbt):
+def psbt_to_txid(psbt, network='main'):
     """
     Extract txid from a Base64 PSBT using bitcoin-core trough a "bitcoin-cli decodepsbt" call
     
     :param psbt: Base64 encoded psbt
     
     return txid in hexadecimal encoded format
     """
-    command = f"bitcoin-cli decodepsbt {psbt}"
+    if network == 'main':
+        network = ''
+    elif network in ['testnet', 'regtest', 'signet']:
+        network = f'-{network}'
+    command = f"bitcoin-cli {network} decodepsbt {psbt}"
     result = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, text=True)
     if result.returncode == 0:
         txid = json.loads(result.stdout)['tx']['txid']
         return txid
     else:
         data = {'error': f'Cannot decode psbt: {psbt}'}
         return data
    
     
-def rawtx_to_txid(rawtx):
+def rawtx_to_txid(rawtx, network='main'):
     """
     Extract txid from a raw transaction (hex format) using bitcoin-core trough a "bitcoin-cli decoderawtransaction" call
 
     :param rawtx: raw tx in hexadecimal format
 
     return txid in hexadecimal encoded format
     """
-    command = f"bitcoin-cli decoderawtransaction {rawtx}"
+    if network == 'main':
+        network = ''
+    elif network in ['testnet', 'regtest', 'signet']:
+        network = f'-{network}'
+    command = f"bitcoin-cli {network} decoderawtransaction {rawtx}"
     result = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, text=True)
     if result.returncode == 0:
         txid = json.loads(result.stdout)['txid']
         return txid
     else:
         data = {'error': f'Cannot decode rawtx: {rawtx}'}
         return data
     
     
-def decode_tx(rawtx):
+def decode_tx(rawtx, network='main'):
     """
     Decode a raw transaction (hex format) using bitcoin-core trough a "bitcoin-cli decoderawtransaction" call
 
     :param rawtx: raw tx in hexadecimal format
 
     return a decoded tx
     """
-    command = f"bitcoin-cli decoderawtransaction {rawtx}"
+    if network == 'main':
+        network = ''
+    elif network in ['testnet', 'regtest', 'signet']:
+        network = f'-{network}'
+    command = f"bitcoin-cli {network} decoderawtransaction {rawtx}"
     result = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, text=True)
     if result.returncode == 0:
         tx = json.loads(result.stdout)
         return tx
     else:
         data = {'error': f'Cannot decode rawtx: {rawtx}'}
         return data
```

### Comparing `liana-rpc-0.0.2/liana_rpc/utils/rpc.py` & `liana-rpc-0.0.3/liana_rpc/utils/rpc.py`

 * *Files identical despite different names*

### Comparing `liana-rpc-0.0.2/pyproject.toml` & `liana-rpc-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel" ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "liana-rpc"
-version = "0.0.2"
+version = "0.0.3"
 description = "RPC client for connect to Liana daemon (lianad)"
 license = {file = "LICENSE"}
 authors = [
   {name = "pythcoiner", email = "pythcoiner@proton.me"},
   {name = "darosior", email = "darosior@protonmail.com"},
 ]
 requires-python = ">=3.9"
```

