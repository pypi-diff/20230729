# Comparing `tmp/easyencryption-0.1.7.1.tar.gz` & `tmp/easyencryption-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyencryption-0.1.7.1.tar", last modified: Tue Jul 25 21:28:19 2023, max compression
+gzip compressed data, was "easyencryption-0.1.8.tar", last modified: Sat Jul 29 16:51:12 2023, max compression
```

## Comparing `easyencryption-0.1.7.1.tar` & `easyencryption-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 21:28:19.337709 easyencryption-0.1.7.1/
--rw-rw-rw-   0        0        0     3516 2023-07-25 21:28:19.338710 easyencryption-0.1.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     2258 2023-07-25 21:22:54.000000 easyencryption-0.1.7.1/README.md
--rw-rw-rw-   0        0        0      723 2023-07-25 21:28:19.339714 easyencryption-0.1.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1994 2023-07-25 21:27:57.000000 easyencryption-0.1.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 21:28:19.301759 easyencryption-0.1.7.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-25 21:28:19.317145 easyencryption-0.1.7.1/src/easyencryption/
--rw-rw-rw-   0        0        0      642 2023-07-25 21:27:50.000000 easyencryption-0.1.7.1/src/easyencryption/__init__.py
--rw-rw-rw-   0        0        0     1355 2023-07-25 00:01:43.000000 easyencryption-0.1.7.1/src/easyencryption/aes.py
--rw-rw-rw-   0        0        0     1679 2023-06-25 21:36:58.000000 easyencryption-0.1.7.1/src/easyencryption/custom.py
--rw-rw-rw-   0        0        0     1490 2023-07-25 00:00:48.000000 easyencryption-0.1.7.1/src/easyencryption/ecc.py
--rw-rw-rw-   0        0        0     1087 2023-06-24 15:16:52.000000 easyencryption-0.1.7.1/src/easyencryption/fernet.py
--rw-rw-rw-   0        0        0     1977 2023-07-25 00:01:03.000000 easyencryption-0.1.7.1/src/easyencryption/rsa.py
--rw-rw-rw-   0        0        0     2057 2023-06-24 15:16:52.000000 easyencryption-0.1.7.1/src/easyencryption/sha.py
-drwxrwxrwx   0        0        0        0 2023-07-25 21:28:19.337709 easyencryption-0.1.7.1/src/easyencryption.egg-info/
--rw-rw-rw-   0        0        0     3516 2023-07-25 21:28:19.000000 easyencryption-0.1.7.1/src/easyencryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-07-25 21:28:19.000000 easyencryption-0.1.7.1/src/easyencryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 21:28:19.000000 easyencryption-0.1.7.1/src/easyencryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-25 21:28:19.000000 easyencryption-0.1.7.1/src/easyencryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-25 21:28:19.000000 easyencryption-0.1.7.1/src/easyencryption.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 16:51:12.891944 easyencryption-0.1.8/
+-rw-rw-rw-   0        0        0     3514 2023-07-29 16:51:12.891944 easyencryption-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2258 2023-07-25 21:22:54.000000 easyencryption-0.1.8/README.md
+-rw-rw-rw-   0        0        0      723 2023-07-29 16:51:12.892947 easyencryption-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1992 2023-07-29 16:50:50.000000 easyencryption-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:51:12.821581 easyencryption-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-29 16:51:12.874100 easyencryption-0.1.8/src/easyencryption/
+-rw-rw-rw-   0        0        0      467 2023-07-29 16:43:27.000000 easyencryption-0.1.8/src/easyencryption/__init__.py
+-rw-rw-rw-   0        0        0     1492 2023-07-29 16:46:57.000000 easyencryption-0.1.8/src/easyencryption/aes.py
+-rw-rw-rw-   0        0        0     1672 2023-07-29 16:47:28.000000 easyencryption-0.1.8/src/easyencryption/custom.py
+-rw-rw-rw-   0        0        0     1457 2023-07-29 16:48:16.000000 easyencryption-0.1.8/src/easyencryption/ecc.py
+-rw-rw-rw-   0        0        0     1131 2023-07-29 16:48:48.000000 easyencryption-0.1.8/src/easyencryption/fernet.py
+-rw-rw-rw-   0        0        0     2029 2023-07-29 16:50:15.000000 easyencryption-0.1.8/src/easyencryption/rsa.py
+-rw-rw-rw-   0        0        0     2043 2023-07-29 16:50:30.000000 easyencryption-0.1.8/src/easyencryption/sha.py
+-rw-rw-rw-   0        0        0     1878 2023-07-29 16:44:10.000000 easyencryption-0.1.8/src/easyencryption/xor.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:51:12.890944 easyencryption-0.1.8/src/easyencryption.egg-info/
+-rw-rw-rw-   0        0        0     3514 2023-07-29 16:51:12.000000 easyencryption-0.1.8/src/easyencryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-07-29 16:51:12.000000 easyencryption-0.1.8/src/easyencryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 16:51:12.000000 easyencryption-0.1.8/src/easyencryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-29 16:51:12.000000 easyencryption-0.1.8/src/easyencryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-29 16:51:12.000000 easyencryption-0.1.8/src/easyencryption.egg-info/top_level.txt
```

### Comparing `easyencryption-0.1.7.1/PKG-INFO` & `easyencryption-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.7.1
+Version: 0.1.8
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
```

### Comparing `easyencryption-0.1.7.1/README.md` & `easyencryption-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.7.1/setup.cfg` & `easyencryption-0.1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.7.1/setup.py` & `easyencryption-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_desc = open("README.md", "r")
 long_description = long_desc.read()
 ##with open('src/easyencryption/__init__.py', 'r') as f:
     ##version = [line.split('=')[1].strip(" '\"") for line in f.read().splitlines() if line.startswith('__version__')][0]
-version = "0.1.7.1"
+version = "0.1.8"
 
 setup(
     name='easyencryption',
     version=version,
     description='A very easy way to encrypt data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `easyencryption-0.1.7.1/src/easyencryption/aes.py` & `easyencryption-0.1.8/src/easyencryption/aes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import base64
-import hashlib
-from Cryptodome.Cipher import AES
-from Crypto import Random
+import base64, hashlib, Cryptodome, Crypto
 
 async def genkey():
-    generated_key = Random.new().read(AES.block_size)
+    generated_key = Crypto.Random.new().read(Cryptodome.Cipher.AES.block_size)
     key = hashlib.sha256(generated_key).digest()
     with open("aeseasyencryption.key", "wb") as key_file:
         key_file.write(key)
     return key
 
 async def callkey():
   try:
@@ -19,25 +16,25 @@
     return key
   except:
     await genkey()
     key = open("aeseasyencryption.key", "rb").read()
     return key
 
 
-async def aesencrypt(slogan):
+async def aesencrypt(slogan:str):
     key = await callkey()
-    BS = AES.block_size
+    BS = Cryptodome.Cipher.AES.block_size
     pad = lambda s: s + (BS - len(s) % BS) * chr(BS - len(s) % BS)
 
     slogan = base64.b64encode(pad(slogan).encode('utf8'))
-    iv = Random.get_random_bytes(AES.block_size)
-    cipher = AES.new(key=key, mode= AES.MODE_CFB,iv= iv)
+    iv = Crypto.Random.get_random_bytes(Cryptodome.Cipher.AES.block_size)
+    cipher = Cryptodome.Cipher.AES.new(key=key, mode= Cryptodome.Cipher.AES.MODE_CFB,iv= iv)
     return base64.b64encode(iv + cipher.encrypt(slogan))
 
-async def aesdecrypt(coded_slogan):
+async def aesdecrypt(coded_slogan:bytes):
     key = await callkey()
     unpad = lambda s: s[:-ord(s[-1:])]
 
     coded_slogan = base64.b64decode(coded_slogan)
-    iv = coded_slogan[:AES.block_size]
-    cipher = AES.new(key, AES.MODE_CFB, iv)
-    return unpad(base64.b64decode(cipher.decrypt(coded_slogan[AES.block_size:])).decode('utf8'))
+    iv = coded_slogan[:Cryptodome.Cipher.AES.block_size]
+    cipher = Cryptodome.Cipher.AES.new(key, Cryptodome.Cipher.AES.MODE_CFB, iv)
+    return unpad(base64.b64decode(cipher.decrypt(coded_slogan[Cryptodome.Cipher.AES.block_size:])).decode('utf8'))
```

### Comparing `easyencryption-0.1.7.1/src/easyencryption/custom.py` & `easyencryption-0.1.8/src/easyencryption/custom.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import random
-import math
+import random, math
 
 async def customencrypt(string:str):
     asciis = []
     biggest = 0
     for char in enumerate(string):
         charascii = ord(char[1])
         rand = math.floor(random.random() * (126-charascii))
```

### Comparing `easyencryption-0.1.7.1/src/easyencryption/ecc.py` & `easyencryption-0.1.8/src/easyencryption/ecc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from ecies.utils import generate_key
-from ecies import encrypt, decrypt
-import codecs
+import codecs, ecies
 
 async def genkeys():
-    secp_k = generate_key()
+    secp_k = ecies.utils.generate_key()
     sk_bytes = secp_k.secret  # bytes
     pk_bytes = secp_k.public_key.format(True)
     with open("eccseasyencryption.key", "wb") as pub_key_file:
         pub_key_file.write(sk_bytes)
     with open("eccpeasyencryption.key", "wb") as priv_key_file:
         priv_key_file.write(pk_bytes)
     keys = [sk_bytes, pk_bytes]
@@ -33,18 +31,18 @@
       key = open("eccpeasyencryption.key", "rb").read()
     return key
   except:
     await genkeys()
     key = open("eccpeasyencryption.key", "rb").read()
     return key
 
-async def eccencrypt(slogan):
+async def eccencrypt(slogan:str):
     data = codecs.encode(slogan)
     pk_bytes = await callpkey()  # bytes
-    encrypted = encrypt(pk_bytes, data)
+    encrypted = ecies.encrypt(pk_bytes, data)
     return encrypted
 
-async def eccdecrypt(coded_slogan):
+async def eccdecrypt(coded_slogan:bytes):
     sk_bytes = await callskey()  # bytes
-    decrypted_byted = decrypt(sk_bytes, coded_slogan)
+    decrypted_byted = ecies.decrypt(sk_bytes, coded_slogan)
     decrypted = codecs.decode(decrypted_byted)
     return decrypted
```

### Comparing `easyencryption-0.1.7.1/src/easyencryption/fernet.py` & `easyencryption-0.1.8/src/easyencryption/fernet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from cryptography.fernet import Fernet
-import os
+import os, cryptography
 
 async def genkey():
-  key = Fernet.generate_key()
+  key = cryptography.fernet.Fernet.generate_key()
   with open("symeasyencryption.key", "wb") as key_file:
     key_file.write(key)
   return key
 
 async def regenkey():
   if os.path.exists("symeasyencryption.key"):
     os.remove("symeasyencryption.key")
@@ -20,24 +19,24 @@
       key = open("symeasyencryption.key", "rb").read()
     return key
   except:
     await genkey()
     key = open("symeasyencryption.key", "rb").read()
     return key
 
-async def fernetencrypt(slogan):
+async def fernetencrypt(slogan:str):
   key = await callkey()
   slogan = slogan.encode()
-  a = Fernet(key)
+  a = cryptography.fernet.Fernet(key)
   coded_slogan = a.encrypt(slogan)
   return coded_slogan
 
-async def fernetdecrypt(coded_slogan):
+async def fernetdecrypt(coded_slogan:bytes):
   key = await callkey()
-  b = Fernet(key)
+  b = cryptography.fernet.Fernet(key)
   decoded_slogan = b.decrypt(coded_slogan)
   decoded_slogan = str(decoded_slogan)
   decoded_slogan = decoded_slogan[2:]
   decoded_slogan = decoded_slogan[:-1]
   return(decoded_slogan)
```

### Comparing `easyencryption-0.1.7.1/src/easyencryption/rsa.py` & `easyencryption-0.1.8/src/easyencryption/rsa.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from Crypto.PublicKey import RSA as rsa
-from Crypto.Cipher import PKCS1_OAEP
-import os
+import os, Crypto
 
 async def genkeys():
-    key = rsa.generate(2048)
+    key = Crypto.PublicKey.RSA.generate(2048)
     publickey = key.publickey().export_key()
     privatekey = key.export_key()
     with open("pubeasyencryption.key", "wb") as pub_key_file:
         pub_key_file.write(publickey)
     with open("priveasyencryption.key", "wb") as priv_key_file:
         priv_key_file.write(privatekey)
     keys = [publickey, privatekey]
@@ -22,44 +20,44 @@
 
 async def callpubkey():
   try:
     key = open("pubeasyencryption.key", "rb").read()
     if str(key) == "b''":
       await genkeys()
       key = open("pubeasyencryption.key", "rb").read()
-    key = rsa.import_key(key)
+    key = Crypto.PublicKey.RSA.import_key(key)
     return key
   except:
     await genkeys()
     key = open("pubeasyencryption.key", "rb").read()
-    key = rsa.import_key(key)
+    key = Crypto.PublicKey.RSA.import_key(key)
     return key
 
 async def callprivkey():
   try:
     key = open("priveasyencryption.key", "rb").read()
     if str(key) == "b''":
       await genkeys()
       key = open("priveasyencryption.key", "rb").read()
-    key = rsa.import_key(key)
+    key = Crypto.PublicKey.RSA.import_key(key)
     return key
   except:
     await genkeys()
     key = open("priveasyencryption.key", "rb").read()
-    key = rsa.import_key(key)
+    key = Crypto.PublicKey.RSA.import_key(key)
     return key
 
-async def rsaencrypt(slogan):
+async def rsaencrypt(slogan:str):
     key = await callpubkey()
-    encryptor = PKCS1_OAEP.new(key)
+    encryptor = Crypto.Cipher.PKCS1_OAEP.new(key)
     coded_slogan = encryptor.encrypt(slogan.encode("utf-8"))
     return coded_slogan
 
-async def rsadecrypt(coded_slogan):
+async def rsadecrypt(coded_slogan:bytes):
     key = await callprivkey()
-    decryptor = PKCS1_OAEP.new(key)
+    decryptor = Crypto.Cipher.PKCS1_OAEP.new(key)
     decoded_slogan = decryptor.decrypt(coded_slogan)
     decoded_slogan = str(decoded_slogan)
     decoded_slogan = decoded_slogan[2:]
     decoded_slogan = decoded_slogan[:-1]
     return decoded_slogan
```

### Comparing `easyencryption-0.1.7.1/src/easyencryption/sha.py` & `easyencryption-0.1.8/src/easyencryption/sha.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import hashlib
-import codecs
-import secrets
+import hashlib, codecs, secrets
 
 async def gensalt():
     generated_salt = secrets.token_hex(32)
     with open("hashsalt.key", "wb") as key_file:
         key_file.write(codecs.encode(generated_salt))
     return generated_salt
```

### Comparing `easyencryption-0.1.7.1/src/easyencryption.egg-info/PKG-INFO` & `easyencryption-0.1.8/src/easyencryption.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.7.1
+Version: 0.1.8
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
```

