# Comparing `tmp/easyencryption-0.1.8.2.tar.gz` & `tmp/easyencryption-0.1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyencryption-0.1.8.2.tar", last modified: Sat Jul 29 17:01:05 2023, max compression
+gzip compressed data, was "easyencryption-0.1.8.3.tar", last modified: Sat Jul 29 17:21:43 2023, max compression
```

## Comparing `easyencryption-0.1.8.2.tar` & `easyencryption-0.1.8.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 17:01:05.527381 easyencryption-0.1.8.2/
--rw-rw-rw-   0        0        0     3674 2023-07-29 17:01:05.527381 easyencryption-0.1.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     2416 2023-07-29 16:53:46.000000 easyencryption-0.1.8.2/README.md
--rw-rw-rw-   0        0        0      723 2023-07-29 17:01:05.532386 easyencryption-0.1.8.2/setup.cfg
--rw-rw-rw-   0        0        0     1994 2023-07-29 17:00:54.000000 easyencryption-0.1.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 17:01:05.495380 easyencryption-0.1.8.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-29 17:01:05.513382 easyencryption-0.1.8.2/src/easyencryption/
--rw-rw-rw-   0        0        0      467 2023-07-29 16:43:27.000000 easyencryption-0.1.8.2/src/easyencryption/__init__.py
--rw-rw-rw-   0        0        0     1353 2023-07-29 17:00:49.000000 easyencryption-0.1.8.2/src/easyencryption/aes.py
--rw-rw-rw-   0        0        0     1672 2023-07-29 16:47:28.000000 easyencryption-0.1.8.2/src/easyencryption/custom.py
--rw-rw-rw-   0        0        0     1457 2023-07-29 16:48:16.000000 easyencryption-0.1.8.2/src/easyencryption/ecc.py
--rw-rw-rw-   0        0        0     1131 2023-07-29 16:48:48.000000 easyencryption-0.1.8.2/src/easyencryption/fernet.py
--rw-rw-rw-   0        0        0     2029 2023-07-29 16:50:15.000000 easyencryption-0.1.8.2/src/easyencryption/rsa.py
--rw-rw-rw-   0        0        0     2043 2023-07-29 16:50:30.000000 easyencryption-0.1.8.2/src/easyencryption/sha.py
--rw-rw-rw-   0        0        0     1878 2023-07-29 16:44:10.000000 easyencryption-0.1.8.2/src/easyencryption/xor.py
-drwxrwxrwx   0        0        0        0 2023-07-29 17:01:05.526381 easyencryption-0.1.8.2/src/easyencryption.egg-info/
--rw-rw-rw-   0        0        0     3674 2023-07-29 17:01:05.000000 easyencryption-0.1.8.2/src/easyencryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-07-29 17:01:05.000000 easyencryption-0.1.8.2/src/easyencryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 17:01:05.000000 easyencryption-0.1.8.2/src/easyencryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-29 17:01:05.000000 easyencryption-0.1.8.2/src/easyencryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-29 17:01:05.000000 easyencryption-0.1.8.2/src/easyencryption.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 17:21:43.493365 easyencryption-0.1.8.3/
+-rw-rw-rw-   0        0        0     3674 2023-07-29 17:21:43.493365 easyencryption-0.1.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2416 2023-07-29 16:53:46.000000 easyencryption-0.1.8.3/README.md
+-rw-rw-rw-   0        0        0      723 2023-07-29 17:21:43.495368 easyencryption-0.1.8.3/setup.cfg
+-rw-rw-rw-   0        0        0     1994 2023-07-29 17:21:31.000000 easyencryption-0.1.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:21:43.461286 easyencryption-0.1.8.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-29 17:21:43.478833 easyencryption-0.1.8.3/src/easyencryption/
+-rw-rw-rw-   0        0        0      467 2023-07-29 16:43:27.000000 easyencryption-0.1.8.3/src/easyencryption/__init__.py
+-rw-rw-rw-   0        0        0     1353 2023-07-29 17:00:49.000000 easyencryption-0.1.8.3/src/easyencryption/aes.py
+-rw-rw-rw-   0        0        0     1672 2023-07-29 16:47:28.000000 easyencryption-0.1.8.3/src/easyencryption/custom.py
+-rw-rw-rw-   0        0        0     1457 2023-07-29 16:48:16.000000 easyencryption-0.1.8.3/src/easyencryption/ecc.py
+-rw-rw-rw-   0        0        0     1097 2023-07-29 17:21:25.000000 easyencryption-0.1.8.3/src/easyencryption/fernet.py
+-rw-rw-rw-   0        0        0     2029 2023-07-29 16:50:15.000000 easyencryption-0.1.8.3/src/easyencryption/rsa.py
+-rw-rw-rw-   0        0        0     2043 2023-07-29 16:50:30.000000 easyencryption-0.1.8.3/src/easyencryption/sha.py
+-rw-rw-rw-   0        0        0     1878 2023-07-29 16:44:10.000000 easyencryption-0.1.8.3/src/easyencryption/xor.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:21:43.492367 easyencryption-0.1.8.3/src/easyencryption.egg-info/
+-rw-rw-rw-   0        0        0     3674 2023-07-29 17:21:43.000000 easyencryption-0.1.8.3/src/easyencryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-07-29 17:21:43.000000 easyencryption-0.1.8.3/src/easyencryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 17:21:43.000000 easyencryption-0.1.8.3/src/easyencryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-29 17:21:43.000000 easyencryption-0.1.8.3/src/easyencryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-29 17:21:43.000000 easyencryption-0.1.8.3/src/easyencryption.egg-info/top_level.txt
```

### Comparing `easyencryption-0.1.8.2/PKG-INFO` & `easyencryption-0.1.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.8.2
+Version: 0.1.8.3
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
```

### Comparing `easyencryption-0.1.8.2/README.md` & `easyencryption-0.1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.2/setup.cfg` & `easyencryption-0.1.8.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.2/setup.py` & `easyencryption-0.1.8.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_desc = open("README.md", "r")
 long_description = long_desc.read()
 ##with open('src/easyencryption/__init__.py', 'r') as f:
     ##version = [line.split('=')[1].strip(" '\"") for line in f.read().splitlines() if line.startswith('__version__')][0]
-version = "0.1.8.2"
+version = "0.1.8.3"
 
 setup(
     name='easyencryption',
     version=version,
     description='A very easy way to encrypt data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `easyencryption-0.1.8.2/src/easyencryption/aes.py` & `easyencryption-0.1.8.3/src/easyencryption/aes.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.2/src/easyencryption/custom.py` & `easyencryption-0.1.8.3/src/easyencryption/custom.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.2/src/easyencryption/ecc.py` & `easyencryption-0.1.8.3/src/easyencryption/ecc.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.2/src/easyencryption/fernet.py` & `easyencryption-0.1.8.3/src/easyencryption/fernet.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import os, cryptography
+import os
+from cryptography.fernet import Fernet
 
 async def genkey():
-  key = cryptography.fernet.Fernet.generate_key()
+  key = Fernet.generate_key()
   with open("symeasyencryption.key", "wb") as key_file:
     key_file.write(key)
   return key
 
 async def regenkey():
   if os.path.exists("symeasyencryption.key"):
     os.remove("symeasyencryption.key")
@@ -22,21 +23,21 @@
     await genkey()
     key = open("symeasyencryption.key", "rb").read()
     return key
 
 async def fernetencrypt(slogan:str):
   key = await callkey()
   slogan = slogan.encode()
-  a = cryptography.fernet.Fernet(key)
+  a = Fernet(key)
   coded_slogan = a.encrypt(slogan)
   return coded_slogan
 
 async def fernetdecrypt(coded_slogan:bytes):
   key = await callkey()
-  b = cryptography.fernet.Fernet(key)
+  b = Fernet(key)
   decoded_slogan = b.decrypt(coded_slogan)
   decoded_slogan = str(decoded_slogan)
   decoded_slogan = decoded_slogan[2:]
   decoded_slogan = decoded_slogan[:-1]
   return(decoded_slogan)
```

### Comparing `easyencryption-0.1.8.2/src/easyencryption/rsa.py` & `easyencryption-0.1.8.3/src/easyencryption/rsa.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.2/src/easyencryption/sha.py` & `easyencryption-0.1.8.3/src/easyencryption/sha.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.2/src/easyencryption/xor.py` & `easyencryption-0.1.8.3/src/easyencryption/xor.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.2/src/easyencryption.egg-info/PKG-INFO` & `easyencryption-0.1.8.3/src/easyencryption.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.8.2
+Version: 0.1.8.3
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
```

