# Comparing `tmp/CipherProgram-0.0.3.tar.gz` & `tmp/CipherProgram-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CipherProgram-0.0.3.tar", last modified: Sat Jul 29 11:17:33 2023, max compression
+gzip compressed data, was "CipherProgram-0.0.4.tar", last modified: Sat Jul 29 11:23:19 2023, max compression
```

## Comparing `CipherProgram-0.0.3.tar` & `CipherProgram-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-29 11:17:33.707654 CipherProgram-0.0.3/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-29 11:17:33.703657 CipherProgram-0.0.3/Cipher/
--rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-07-28 20:46:04.000000 CipherProgram-0.0.3/Cipher/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)      627 2023-07-28 20:56:20.000000 CipherProgram-0.0.3/Cipher/main.py
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-29 11:17:33.707654 CipherProgram-0.0.3/CipherProgram.egg-info/
--rw-r--r--   0 cipher    (1000) cipher    (1000)      815 2023-07-29 11:17:33.000000 CipherProgram-0.0.3/CipherProgram.egg-info/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)      208 2023-07-29 11:17:33.000000 CipherProgram-0.0.3/CipherProgram.egg-info/SOURCES.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-07-29 11:17:33.000000 CipherProgram-0.0.3/CipherProgram.egg-info/dependency_links.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        7 2023-07-29 11:17:33.000000 CipherProgram-0.0.3/CipherProgram.egg-info/top_level.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1363 2023-07-28 20:08:20.000000 CipherProgram-0.0.3/LICENSE
--rw-r--r--   0 cipher    (1000) cipher    (1000)      815 2023-07-29 11:17:33.707654 CipherProgram-0.0.3/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)      428 2023-07-28 21:07:49.000000 CipherProgram-0.0.3/README.md
--rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-07-29 11:17:33.707654 CipherProgram-0.0.3/setup.cfg
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1256 2023-07-29 11:17:30.000000 CipherProgram-0.0.3/setup.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-29 11:23:19.183256 CipherProgram-0.0.4/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-29 11:23:19.178950 CipherProgram-0.0.4/Cipher/
+-rw-r--r--   0 cipher     (501) staff       (20)       20 2023-07-29 11:08:33.000000 CipherProgram-0.0.4/Cipher/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)      578 2023-07-29 11:21:12.000000 CipherProgram-0.0.4/Cipher/main.py
+-rw-r--r--   0 cipher     (501) staff       (20)      286 2023-07-29 11:22:33.000000 CipherProgram-0.0.4/Cipher/test.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-29 11:23:19.182659 CipherProgram-0.0.4/CipherProgram.egg-info/
+-rw-r--r--   0 cipher     (501) staff       (20)      790 2023-07-29 11:23:18.000000 CipherProgram-0.0.4/CipherProgram.egg-info/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)      223 2023-07-29 11:23:19.000000 CipherProgram-0.0.4/CipherProgram.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-29 11:23:18.000000 CipherProgram-0.0.4/CipherProgram.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher     (501) staff       (20)        7 2023-07-29 11:23:19.000000 CipherProgram-0.0.4/CipherProgram.egg-info/top_level.txt
+-rw-r--r--   0 cipher     (501) staff       (20)     1363 2023-07-29 11:08:33.000000 CipherProgram-0.0.4/LICENSE
+-rw-r--r--   0 cipher     (501) staff       (20)      790 2023-07-29 11:23:19.183025 CipherProgram-0.0.4/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)      403 2023-07-29 11:21:51.000000 CipherProgram-0.0.4/README.md
+-rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-29 11:23:19.183319 CipherProgram-0.0.4/setup.cfg
+-rw-r--r--   0 cipher     (501) staff       (20)     1256 2023-07-29 11:23:15.000000 CipherProgram-0.0.4/setup.py
```

### Comparing `CipherProgram-0.0.3/CipherProgram.egg-info/PKG-INFO` & `CipherProgram-0.0.4/CipherProgram.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CipherProgram
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/Cipher58/
 Download-URL: https://github.com/Cipher58/Cipher.git
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: The Unlicense
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 
 ```
 from Cipher import *
 
 key = 42
 original_text = input("You: ")
 
-cipher = Cipher(key, original_text)
+cipher = Cipher(key)
 
-encrypted_text = cipher.simple_xor_encrypt(original_text, key)
-decrypted_text = cipher.simple_xor_decrypt(encrypted_text, key)
+encrypted_text = cipher.simple_xor_encrypt(original_text)
+decrypted_text = cipher.simple_xor_decrypt(encrypted_text)
 
 print("Encrypted text:", encrypted_text)
 print("Decrypted text:", decrypted_text)
 ```
```

### Comparing `CipherProgram-0.0.3/LICENSE` & `CipherProgram-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CipherProgram-0.0.3/PKG-INFO` & `CipherProgram-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CipherProgram
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/Cipher58/
 Download-URL: https://github.com/Cipher58/Cipher.git
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: The Unlicense
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 
 ```
 from Cipher import *
 
 key = 42
 original_text = input("You: ")
 
-cipher = Cipher(key, original_text)
+cipher = Cipher(key)
 
-encrypted_text = cipher.simple_xor_encrypt(original_text, key)
-decrypted_text = cipher.simple_xor_decrypt(encrypted_text, key)
+encrypted_text = cipher.simple_xor_encrypt(original_text)
+decrypted_text = cipher.simple_xor_decrypt(encrypted_text)
 
 print("Encrypted text:", encrypted_text)
 print("Decrypted text:", decrypted_text)
 ```
```

### Comparing `CipherProgram-0.0.3/setup.py` & `CipherProgram-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="CipherProgram",
 
     # version of the module
-    version="0.0.3",
+    version="0.0.4",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Cipher.git',
 
     # your Email address
```

