# Comparing `tmp/aityz-1.0.2.1.tar.gz` & `tmp/aityz-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aityz-1.0.2.1.tar", last modified: Thu Jul 27 08:24:06 2023, max compression
+gzip compressed data, was "aityz-1.0.3.tar", last modified: Sat Jul 29 04:17:21 2023, max compression
```

## Comparing `aityz-1.0.2.1.tar` & `aityz-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 08:24:06.972301 aityz-1.0.2.1/
--rw-rw-rw-   0        0        0    35821 2023-07-26 03:38:00.000000 aityz-1.0.2.1/LICENSE
--rw-rw-rw-   0        0        0      449 2023-07-27 08:24:06.970011 aityz-1.0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-26 11:03:01.000000 aityz-1.0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 08:24:06.930048 aityz-1.0.2.1/aityz/
--rw-rw-rw-   0        0        0        0 2023-07-26 11:07:26.000000 aityz-1.0.2.1/aityz/__init__.py
--rw-rw-rw-   0        0        0     5781 2023-07-27 08:22:26.000000 aityz-1.0.2.1/aityz/encryption.py
--rw-rw-rw-   0        0        0      440 2023-07-26 11:05:19.000000 aityz-1.0.2.1/aityz/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-27 08:24:06.962069 aityz-1.0.2.1/aityz.egg-info/
--rw-rw-rw-   0        0        0      449 2023-07-27 08:24:06.000000 aityz-1.0.2.1/aityz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-27 08:24:06.000000 aityz-1.0.2.1/aityz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 08:24:06.000000 aityz-1.0.2.1/aityz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-27 08:24:06.000000 aityz-1.0.2.1/aityz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-27 08:24:06.000000 aityz-1.0.2.1/aityz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      625 2023-07-26 03:53:16.000000 aityz-1.0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 08:24:06.972301 aityz-1.0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      606 2023-07-27 08:24:02.000000 aityz-1.0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:17:21.873250 aityz-1.0.3/
+-rw-rw-rw-   0        0        0    35821 2023-07-26 03:38:00.000000 aityz-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      447 2023-07-29 04:17:21.869997 aityz-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-26 11:03:01.000000 aityz-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 04:17:21.837611 aityz-1.0.3/aityz/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:07:26.000000 aityz-1.0.3/aityz/__init__.py
+-rw-rw-rw-   0        0        0     8062 2023-07-29 04:17:04.000000 aityz-1.0.3/aityz/encryption.py
+-rw-rw-rw-   0        0        0      908 2023-07-27 23:50:25.000000 aityz-1.0.3/aityz/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:17:21.865808 aityz-1.0.3/aityz.egg-info/
+-rw-rw-rw-   0        0        0      447 2023-07-29 04:17:21.000000 aityz-1.0.3/aityz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-29 04:17:21.000000 aityz-1.0.3/aityz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 04:17:21.000000 aityz-1.0.3/aityz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-29 04:17:21.000000 aityz-1.0.3/aityz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-29 04:17:21.000000 aityz-1.0.3/aityz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      625 2023-07-26 03:53:16.000000 aityz-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-29 04:17:21.873250 aityz-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      604 2023-07-29 04:17:20.000000 aityz-1.0.3/setup.py
```

### Comparing `aityz-1.0.2.1/LICENSE` & `aityz-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aityz-1.0.2.1/aityz/encryption.py` & `aityz-1.0.3/aityz/encryption.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from aityz import exceptions
 import rsa
 from Crypto.Cipher import AES
 import base64
+import hashlib
 
 
 def pad(pad, length=16):
     """
     Pad a given string `pad` with spaces to a specified `length`.
 
     :param pad: The string to be padded.
@@ -67,15 +68,15 @@
     def encrypt(self, content):
         """
         Encrypts the given content using the RSA encryption algorithm.
 
         :param content: The content to be encrypted.
         :return: The encrypted content.
         """
-        return rsa.encrypt(content, self.Pub)
+        return rsa.encrypt(content.encode(), self.Pub)
 
     def encryptFile(self, filename, outputFile=None):
         """
         Encrypts the contents of the file with RSA encryption.
 
         :param filename: The path to the input file.
         :param outputFile: The path to the output file. (optional)
@@ -102,36 +103,51 @@
         if outputFile is not None:
             with open(outputFile, 'wb') as f:
                 f.write(Data)
         else:
             return Data
 
 
+def loadNonce(loc='nonce.txt'):
+    with open(loc, 'rb') as f:
+        nonce = f.read()
+    return nonce
+
+
 class AES256:
     def __init__(self, password, nonce=None):
         super().__init__()
-        self.key = password
+        self.key = pad(password)
         if len(password) % 16 != 0:
             password = pad(password)
         if nonce is None:
             self.cipher = AES.new(password.encode('utf8'), AES.MODE_EAX)
         else:
             self.cipher = AES.new(password.encode('utf8'), AES.MODE_EAX, nonce=nonce)
-        self.nonce = self.cipher.nonce
 
     def encrypt(self, content):
         enc, tag = self.cipher.encrypt_and_digest(content.encode('utf-8'))
         return enc, tag, self.cipher.nonce
 
     def getNonce(self):
         return self.cipher.nonce
 
     def decrypt(self, content):
         return self.cipher.decrypt(content)
 
+    def saveNonce(self, save='nonce.txt'):
+        with open(save, 'wb') as f:
+            f.write(self.cipher.nonce)
+
+    def verify(self, tag):
+        try:
+            return self.cipher.verify(tag)
+        except ValueError:
+            return 'Incorrect tag/corrupted message'
+
     def encryptFile(self, fileName, saveLoc=None):
         with open(fileName, 'r') as f:
             data = f.read()
         if saveLoc is not None:
             with open(saveLoc, 'w') as f:
                 f.write(str(self.cipher.encrypt(data.encode('utf-8'))))
         else:
@@ -147,7 +163,67 @@
             return str(self.cipher.decrypt(data.encode('utf-8')))
 
     def update(self, nonce=None):
         if nonce is None:
             self.cipher = AES.new(self.key, AES.MODE_EAX)
         else:
             self.cipher = AES.new(self.key, AES.MODE_EAX, nonce=nonce)
+
+
+class SHA3:
+    def __init__(self, size):
+        super().__init__()
+        if size != 224 and size != 256 and size != 384 and size != 512:
+            raise exceptions.SizeError()
+        if size == 224:
+            self.hasher = hashlib.sha3_224()
+        elif size == 256:
+            self.hasher = hashlib.sha3_256()
+        elif size == 384:
+            self.hasher = hashlib.sha3_384()
+        elif size == 512:
+            self.hasher = hashlib.sha3_512()
+
+    def encrypt(self, data: str):
+        self.hasher.update(data.encode('utf8'))
+        return self.hasher.hexdigest()
+
+
+class SHA2:
+    def __init__(self, size):
+        super().__init__()
+        if size != 224 and size != 256 and size != 384 and size != 512:
+            raise exceptions.SizeError()
+        if size == 224:
+            self.hasher = hashlib.sha224()
+        elif size == 256:
+            self.hasher = hashlib.sha256()
+        elif size == 384:
+            self.hasher = hashlib.sha384()
+        elif size == 512:
+            self.hasher = hashlib.sha512()
+
+    def encrypt(self, data: str):
+        self.hasher.update(data.encode('utf8'))
+        return self.hasher.hexdigest()
+
+
+class SHA1:  # It's no longer secure
+    def __init__(self, ignore=False):
+        if ignore is not True:
+            print('SHA-1 Hashing has been compromised. Use SHA-3 or SHA-2 Instead.')
+            print('If you would not like to see this warning pass ignore=True to this class next use.')
+        self.hasher = hashlib.sha1()
+
+    def encrypt(self, data: str):
+        self.hasher.update(data.encode())
+        return self.hasher.hexdigest()
+
+
+class Whirlpool:
+    def __init__(self):
+        self.hasher = hashlib.new('whirlpool')
+
+    def encrypt(self, data: str):
+        self.hasher.update(data.encode())
+        return self.hasher.hexdigest()
+
```

### Comparing `aityz-1.0.2.1/pyproject.toml` & `aityz-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aityz-1.0.2.1/setup.py` & `aityz-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aityz',
-    version='1.0.2.1',
+    version='1.0.3',
     packages=find_packages(),
     install_requires=[
         'rsa',
         'pycryptodome'
     ],
     author='Aityz',
     author_email='itzaityz@gmail.com',
```

