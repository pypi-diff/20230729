# Comparing `tmp/easyencryption-0.1.8.1.tar.gz` & `tmp/easyencryption-0.1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyencryption-0.1.8.1.tar", last modified: Sat Jul 29 16:54:34 2023, max compression
+gzip compressed data, was "easyencryption-0.1.8.2.tar", last modified: Sat Jul 29 17:01:05 2023, max compression
```

## Comparing `easyencryption-0.1.8.1.tar` & `easyencryption-0.1.8.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 16:54:34.349405 easyencryption-0.1.8.1/
--rw-rw-rw-   0        0        0     3674 2023-07-29 16:54:34.350406 easyencryption-0.1.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     2416 2023-07-29 16:53:46.000000 easyencryption-0.1.8.1/README.md
--rw-rw-rw-   0        0        0      723 2023-07-29 16:54:34.351404 easyencryption-0.1.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1994 2023-07-29 16:54:20.000000 easyencryption-0.1.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 16:54:34.322880 easyencryption-0.1.8.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-29 16:54:34.332889 easyencryption-0.1.8.1/src/easyencryption/
--rw-rw-rw-   0        0        0      467 2023-07-29 16:43:27.000000 easyencryption-0.1.8.1/src/easyencryption/__init__.py
--rw-rw-rw-   0        0        0     1492 2023-07-29 16:46:57.000000 easyencryption-0.1.8.1/src/easyencryption/aes.py
--rw-rw-rw-   0        0        0     1672 2023-07-29 16:47:28.000000 easyencryption-0.1.8.1/src/easyencryption/custom.py
--rw-rw-rw-   0        0        0     1457 2023-07-29 16:48:16.000000 easyencryption-0.1.8.1/src/easyencryption/ecc.py
--rw-rw-rw-   0        0        0     1131 2023-07-29 16:48:48.000000 easyencryption-0.1.8.1/src/easyencryption/fernet.py
--rw-rw-rw-   0        0        0     2029 2023-07-29 16:50:15.000000 easyencryption-0.1.8.1/src/easyencryption/rsa.py
--rw-rw-rw-   0        0        0     2043 2023-07-29 16:50:30.000000 easyencryption-0.1.8.1/src/easyencryption/sha.py
--rw-rw-rw-   0        0        0     1878 2023-07-29 16:44:10.000000 easyencryption-0.1.8.1/src/easyencryption/xor.py
-drwxrwxrwx   0        0        0        0 2023-07-29 16:54:34.349405 easyencryption-0.1.8.1/src/easyencryption.egg-info/
--rw-rw-rw-   0        0        0     3674 2023-07-29 16:54:34.000000 easyencryption-0.1.8.1/src/easyencryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-07-29 16:54:34.000000 easyencryption-0.1.8.1/src/easyencryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 16:54:34.000000 easyencryption-0.1.8.1/src/easyencryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-29 16:54:34.000000 easyencryption-0.1.8.1/src/easyencryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-29 16:54:34.000000 easyencryption-0.1.8.1/src/easyencryption.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 17:01:05.527381 easyencryption-0.1.8.2/
+-rw-rw-rw-   0        0        0     3674 2023-07-29 17:01:05.527381 easyencryption-0.1.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2416 2023-07-29 16:53:46.000000 easyencryption-0.1.8.2/README.md
+-rw-rw-rw-   0        0        0      723 2023-07-29 17:01:05.532386 easyencryption-0.1.8.2/setup.cfg
+-rw-rw-rw-   0        0        0     1994 2023-07-29 17:00:54.000000 easyencryption-0.1.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:01:05.495380 easyencryption-0.1.8.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-29 17:01:05.513382 easyencryption-0.1.8.2/src/easyencryption/
+-rw-rw-rw-   0        0        0      467 2023-07-29 16:43:27.000000 easyencryption-0.1.8.2/src/easyencryption/__init__.py
+-rw-rw-rw-   0        0        0     1353 2023-07-29 17:00:49.000000 easyencryption-0.1.8.2/src/easyencryption/aes.py
+-rw-rw-rw-   0        0        0     1672 2023-07-29 16:47:28.000000 easyencryption-0.1.8.2/src/easyencryption/custom.py
+-rw-rw-rw-   0        0        0     1457 2023-07-29 16:48:16.000000 easyencryption-0.1.8.2/src/easyencryption/ecc.py
+-rw-rw-rw-   0        0        0     1131 2023-07-29 16:48:48.000000 easyencryption-0.1.8.2/src/easyencryption/fernet.py
+-rw-rw-rw-   0        0        0     2029 2023-07-29 16:50:15.000000 easyencryption-0.1.8.2/src/easyencryption/rsa.py
+-rw-rw-rw-   0        0        0     2043 2023-07-29 16:50:30.000000 easyencryption-0.1.8.2/src/easyencryption/sha.py
+-rw-rw-rw-   0        0        0     1878 2023-07-29 16:44:10.000000 easyencryption-0.1.8.2/src/easyencryption/xor.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:01:05.526381 easyencryption-0.1.8.2/src/easyencryption.egg-info/
+-rw-rw-rw-   0        0        0     3674 2023-07-29 17:01:05.000000 easyencryption-0.1.8.2/src/easyencryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-07-29 17:01:05.000000 easyencryption-0.1.8.2/src/easyencryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 17:01:05.000000 easyencryption-0.1.8.2/src/easyencryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-29 17:01:05.000000 easyencryption-0.1.8.2/src/easyencryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-29 17:01:05.000000 easyencryption-0.1.8.2/src/easyencryption.egg-info/top_level.txt
```

### Comparing `easyencryption-0.1.8.1/PKG-INFO` & `easyencryption-0.1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.8.1
+Version: 0.1.8.2
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
```

### Comparing `easyencryption-0.1.8.1/README.md` & `easyencryption-0.1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.1/setup.cfg` & `easyencryption-0.1.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.1/setup.py` & `easyencryption-0.1.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_desc = open("README.md", "r")
 long_description = long_desc.read()
 ##with open('src/easyencryption/__init__.py', 'r') as f:
     ##version = [line.split('=')[1].strip(" '\"") for line in f.read().splitlines() if line.startswith('__version__')][0]
-version = "0.1.8.1"
+version = "0.1.8.2"
 
 setup(
     name='easyencryption',
     version=version,
     description='A very easy way to encrypt data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `easyencryption-0.1.8.1/src/easyencryption/aes.py` & `easyencryption-0.1.8.2/src/easyencryption/aes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import base64, hashlib, Cryptodome, Crypto
+import base64, hashlib, Crypto
+from Cryptodome.Cipher import AES
 
 async def genkey():
-    generated_key = Crypto.Random.new().read(Cryptodome.Cipher.AES.block_size)
+    generated_key = Crypto.Random.new().read(AES.block_size)
     key = hashlib.sha256(generated_key).digest()
     with open("aeseasyencryption.key", "wb") as key_file:
         key_file.write(key)
     return key
 
 async def callkey():
   try:
@@ -18,23 +19,23 @@
     await genkey()
     key = open("aeseasyencryption.key", "rb").read()
     return key
 
 
 async def aesencrypt(slogan:str):
     key = await callkey()
-    BS = Cryptodome.Cipher.AES.block_size
+    BS = AES.block_size
     pad = lambda s: s + (BS - len(s) % BS) * chr(BS - len(s) % BS)
 
     slogan = base64.b64encode(pad(slogan).encode('utf8'))
-    iv = Crypto.Random.get_random_bytes(Cryptodome.Cipher.AES.block_size)
-    cipher = Cryptodome.Cipher.AES.new(key=key, mode= Cryptodome.Cipher.AES.MODE_CFB,iv= iv)
+    iv = Crypto.Random.get_random_bytes(AES.block_size)
+    cipher = AES.new(key=key, mode= AES.MODE_CFB,iv= iv)
     return base64.b64encode(iv + cipher.encrypt(slogan))
 
 async def aesdecrypt(coded_slogan:bytes):
     key = await callkey()
     unpad = lambda s: s[:-ord(s[-1:])]
 
     coded_slogan = base64.b64decode(coded_slogan)
-    iv = coded_slogan[:Cryptodome.Cipher.AES.block_size]
-    cipher = Cryptodome.Cipher.AES.new(key, Cryptodome.Cipher.AES.MODE_CFB, iv)
-    return unpad(base64.b64decode(cipher.decrypt(coded_slogan[Cryptodome.Cipher.AES.block_size:])).decode('utf8'))
+    iv = coded_slogan[:AES.block_size]
+    cipher = AES.new(key, AES.MODE_CFB, iv)
+    return unpad(base64.b64decode(cipher.decrypt(coded_slogan[AES.block_size:])).decode('utf8'))
```

### Comparing `easyencryption-0.1.8.1/src/easyencryption/custom.py` & `easyencryption-0.1.8.2/src/easyencryption/custom.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.1/src/easyencryption/ecc.py` & `easyencryption-0.1.8.2/src/easyencryption/ecc.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.1/src/easyencryption/fernet.py` & `easyencryption-0.1.8.2/src/easyencryption/fernet.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.1/src/easyencryption/rsa.py` & `easyencryption-0.1.8.2/src/easyencryption/rsa.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.1/src/easyencryption/sha.py` & `easyencryption-0.1.8.2/src/easyencryption/sha.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.1/src/easyencryption/xor.py` & `easyencryption-0.1.8.2/src/easyencryption/xor.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.1/src/easyencryption.egg-info/PKG-INFO` & `easyencryption-0.1.8.2/src/easyencryption.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.8.1
+Version: 0.1.8.2
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
```

