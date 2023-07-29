# Comparing `tmp/easyencryption-0.1.8.3.tar.gz` & `tmp/easyencryption-0.1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyencryption-0.1.8.3.tar", last modified: Sat Jul 29 17:21:43 2023, max compression
+gzip compressed data, was "easyencryption-0.1.8.4.tar", last modified: Sat Jul 29 17:28:52 2023, max compression
```

## Comparing `easyencryption-0.1.8.3.tar` & `easyencryption-0.1.8.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 17:21:43.493365 easyencryption-0.1.8.3/
--rw-rw-rw-   0        0        0     3674 2023-07-29 17:21:43.493365 easyencryption-0.1.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     2416 2023-07-29 16:53:46.000000 easyencryption-0.1.8.3/README.md
--rw-rw-rw-   0        0        0      723 2023-07-29 17:21:43.495368 easyencryption-0.1.8.3/setup.cfg
--rw-rw-rw-   0        0        0     1994 2023-07-29 17:21:31.000000 easyencryption-0.1.8.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 17:21:43.461286 easyencryption-0.1.8.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-29 17:21:43.478833 easyencryption-0.1.8.3/src/easyencryption/
--rw-rw-rw-   0        0        0      467 2023-07-29 16:43:27.000000 easyencryption-0.1.8.3/src/easyencryption/__init__.py
--rw-rw-rw-   0        0        0     1353 2023-07-29 17:00:49.000000 easyencryption-0.1.8.3/src/easyencryption/aes.py
--rw-rw-rw-   0        0        0     1672 2023-07-29 16:47:28.000000 easyencryption-0.1.8.3/src/easyencryption/custom.py
--rw-rw-rw-   0        0        0     1457 2023-07-29 16:48:16.000000 easyencryption-0.1.8.3/src/easyencryption/ecc.py
--rw-rw-rw-   0        0        0     1097 2023-07-29 17:21:25.000000 easyencryption-0.1.8.3/src/easyencryption/fernet.py
--rw-rw-rw-   0        0        0     2029 2023-07-29 16:50:15.000000 easyencryption-0.1.8.3/src/easyencryption/rsa.py
--rw-rw-rw-   0        0        0     2043 2023-07-29 16:50:30.000000 easyencryption-0.1.8.3/src/easyencryption/sha.py
--rw-rw-rw-   0        0        0     1878 2023-07-29 16:44:10.000000 easyencryption-0.1.8.3/src/easyencryption/xor.py
-drwxrwxrwx   0        0        0        0 2023-07-29 17:21:43.492367 easyencryption-0.1.8.3/src/easyencryption.egg-info/
--rw-rw-rw-   0        0        0     3674 2023-07-29 17:21:43.000000 easyencryption-0.1.8.3/src/easyencryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-07-29 17:21:43.000000 easyencryption-0.1.8.3/src/easyencryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 17:21:43.000000 easyencryption-0.1.8.3/src/easyencryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-29 17:21:43.000000 easyencryption-0.1.8.3/src/easyencryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-29 17:21:43.000000 easyencryption-0.1.8.3/src/easyencryption.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 17:28:52.158166 easyencryption-0.1.8.4/
+-rw-rw-rw-   0        0        0     3674 2023-07-29 17:28:52.158166 easyencryption-0.1.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2416 2023-07-29 16:53:46.000000 easyencryption-0.1.8.4/README.md
+-rw-rw-rw-   0        0        0      723 2023-07-29 17:28:52.160175 easyencryption-0.1.8.4/setup.cfg
+-rw-rw-rw-   0        0        0     1994 2023-07-29 17:27:54.000000 easyencryption-0.1.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:28:51.618762 easyencryption-0.1.8.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-29 17:28:52.143131 easyencryption-0.1.8.4/src/easyencryption/
+-rw-rw-rw-   0        0        0      467 2023-07-29 16:43:27.000000 easyencryption-0.1.8.4/src/easyencryption/__init__.py
+-rw-rw-rw-   0        0        0     1353 2023-07-29 17:00:49.000000 easyencryption-0.1.8.4/src/easyencryption/aes.py
+-rw-rw-rw-   0        0        0     1672 2023-07-29 16:47:28.000000 easyencryption-0.1.8.4/src/easyencryption/custom.py
+-rw-rw-rw-   0        0        0     1457 2023-07-29 16:48:16.000000 easyencryption-0.1.8.4/src/easyencryption/ecc.py
+-rw-rw-rw-   0        0        0     1097 2023-07-29 17:21:25.000000 easyencryption-0.1.8.4/src/easyencryption/fernet.py
+-rw-rw-rw-   0        0        0     1980 2023-07-29 17:27:46.000000 easyencryption-0.1.8.4/src/easyencryption/rsa.py
+-rw-rw-rw-   0        0        0     2043 2023-07-29 16:50:30.000000 easyencryption-0.1.8.4/src/easyencryption/sha.py
+-rw-rw-rw-   0        0        0     1878 2023-07-29 16:44:10.000000 easyencryption-0.1.8.4/src/easyencryption/xor.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:28:52.157654 easyencryption-0.1.8.4/src/easyencryption.egg-info/
+-rw-rw-rw-   0        0        0     3674 2023-07-29 17:28:51.000000 easyencryption-0.1.8.4/src/easyencryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-07-29 17:28:51.000000 easyencryption-0.1.8.4/src/easyencryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 17:28:51.000000 easyencryption-0.1.8.4/src/easyencryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-29 17:28:51.000000 easyencryption-0.1.8.4/src/easyencryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-29 17:28:51.000000 easyencryption-0.1.8.4/src/easyencryption.egg-info/top_level.txt
```

### Comparing `easyencryption-0.1.8.3/PKG-INFO` & `easyencryption-0.1.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.8.3
+Version: 0.1.8.4
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
```

### Comparing `easyencryption-0.1.8.3/README.md` & `easyencryption-0.1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.3/setup.cfg` & `easyencryption-0.1.8.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.3/setup.py` & `easyencryption-0.1.8.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_desc = open("README.md", "r")
 long_description = long_desc.read()
 ##with open('src/easyencryption/__init__.py', 'r') as f:
     ##version = [line.split('=')[1].strip(" '\"") for line in f.read().splitlines() if line.startswith('__version__')][0]
-version = "0.1.8.3"
+version = "0.1.8.4"
 
 setup(
     name='easyencryption',
     version=version,
     description='A very easy way to encrypt data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `easyencryption-0.1.8.3/src/easyencryption/aes.py` & `easyencryption-0.1.8.4/src/easyencryption/aes.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.3/src/easyencryption/custom.py` & `easyencryption-0.1.8.4/src/easyencryption/custom.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.3/src/easyencryption/ecc.py` & `easyencryption-0.1.8.4/src/easyencryption/ecc.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.3/src/easyencryption/fernet.py` & `easyencryption-0.1.8.4/src/easyencryption/fernet.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.3/src/easyencryption/rsa.py` & `easyencryption-0.1.8.4/src/easyencryption/rsa.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import os, Crypto
+import os
+from Crypto.PublicKey import RSA
+from Crypto.Cipher import PKCS1_OAEP
 
 async def genkeys():
-    key = Crypto.PublicKey.RSA.generate(2048)
+    key = RSA.generate(2048)
     publickey = key.publickey().export_key()
     privatekey = key.export_key()
     with open("pubeasyencryption.key", "wb") as pub_key_file:
         pub_key_file.write(publickey)
     with open("priveasyencryption.key", "wb") as priv_key_file:
         priv_key_file.write(privatekey)
     keys = [publickey, privatekey]
@@ -20,44 +22,44 @@
 
 async def callpubkey():
   try:
     key = open("pubeasyencryption.key", "rb").read()
     if str(key) == "b''":
       await genkeys()
       key = open("pubeasyencryption.key", "rb").read()
-    key = Crypto.PublicKey.RSA.import_key(key)
+    key = RSA.import_key(key)
     return key
   except:
     await genkeys()
     key = open("pubeasyencryption.key", "rb").read()
-    key = Crypto.PublicKey.RSA.import_key(key)
+    key = RSA.import_key(key)
     return key
 
 async def callprivkey():
   try:
     key = open("priveasyencryption.key", "rb").read()
     if str(key) == "b''":
       await genkeys()
       key = open("priveasyencryption.key", "rb").read()
-    key = Crypto.PublicKey.RSA.import_key(key)
+    key = RSA.import_key(key)
     return key
   except:
     await genkeys()
     key = open("priveasyencryption.key", "rb").read()
-    key = Crypto.PublicKey.RSA.import_key(key)
+    key = RSA.import_key(key)
     return key
 
 async def rsaencrypt(slogan:str):
     key = await callpubkey()
-    encryptor = Crypto.Cipher.PKCS1_OAEP.new(key)
+    encryptor = PKCS1_OAEP.new(key)
     coded_slogan = encryptor.encrypt(slogan.encode("utf-8"))
     return coded_slogan
 
 async def rsadecrypt(coded_slogan:bytes):
     key = await callprivkey()
-    decryptor = Crypto.Cipher.PKCS1_OAEP.new(key)
+    decryptor = PKCS1_OAEP.new(key)
     decoded_slogan = decryptor.decrypt(coded_slogan)
     decoded_slogan = str(decoded_slogan)
     decoded_slogan = decoded_slogan[2:]
     decoded_slogan = decoded_slogan[:-1]
     return decoded_slogan
```

### Comparing `easyencryption-0.1.8.3/src/easyencryption/sha.py` & `easyencryption-0.1.8.4/src/easyencryption/sha.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.3/src/easyencryption/xor.py` & `easyencryption-0.1.8.4/src/easyencryption/xor.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.3/src/easyencryption.egg-info/PKG-INFO` & `easyencryption-0.1.8.4/src/easyencryption.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.8.3
+Version: 0.1.8.4
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
```

