# Comparing `tmp/easyencryption-0.1.8.tar.gz` & `tmp/easyencryption-0.1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyencryption-0.1.8.tar", last modified: Sat Jul 29 16:51:12 2023, max compression
+gzip compressed data, was "easyencryption-0.1.8.1.tar", last modified: Sat Jul 29 16:54:34 2023, max compression
```

## Comparing `easyencryption-0.1.8.tar` & `easyencryption-0.1.8.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 16:51:12.891944 easyencryption-0.1.8/
--rw-rw-rw-   0        0        0     3514 2023-07-29 16:51:12.891944 easyencryption-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2258 2023-07-25 21:22:54.000000 easyencryption-0.1.8/README.md
--rw-rw-rw-   0        0        0      723 2023-07-29 16:51:12.892947 easyencryption-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1992 2023-07-29 16:50:50.000000 easyencryption-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 16:51:12.821581 easyencryption-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-29 16:51:12.874100 easyencryption-0.1.8/src/easyencryption/
--rw-rw-rw-   0        0        0      467 2023-07-29 16:43:27.000000 easyencryption-0.1.8/src/easyencryption/__init__.py
--rw-rw-rw-   0        0        0     1492 2023-07-29 16:46:57.000000 easyencryption-0.1.8/src/easyencryption/aes.py
--rw-rw-rw-   0        0        0     1672 2023-07-29 16:47:28.000000 easyencryption-0.1.8/src/easyencryption/custom.py
--rw-rw-rw-   0        0        0     1457 2023-07-29 16:48:16.000000 easyencryption-0.1.8/src/easyencryption/ecc.py
--rw-rw-rw-   0        0        0     1131 2023-07-29 16:48:48.000000 easyencryption-0.1.8/src/easyencryption/fernet.py
--rw-rw-rw-   0        0        0     2029 2023-07-29 16:50:15.000000 easyencryption-0.1.8/src/easyencryption/rsa.py
--rw-rw-rw-   0        0        0     2043 2023-07-29 16:50:30.000000 easyencryption-0.1.8/src/easyencryption/sha.py
--rw-rw-rw-   0        0        0     1878 2023-07-29 16:44:10.000000 easyencryption-0.1.8/src/easyencryption/xor.py
-drwxrwxrwx   0        0        0        0 2023-07-29 16:51:12.890944 easyencryption-0.1.8/src/easyencryption.egg-info/
--rw-rw-rw-   0        0        0     3514 2023-07-29 16:51:12.000000 easyencryption-0.1.8/src/easyencryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-07-29 16:51:12.000000 easyencryption-0.1.8/src/easyencryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 16:51:12.000000 easyencryption-0.1.8/src/easyencryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-29 16:51:12.000000 easyencryption-0.1.8/src/easyencryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-29 16:51:12.000000 easyencryption-0.1.8/src/easyencryption.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 16:54:34.349405 easyencryption-0.1.8.1/
+-rw-rw-rw-   0        0        0     3674 2023-07-29 16:54:34.350406 easyencryption-0.1.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2416 2023-07-29 16:53:46.000000 easyencryption-0.1.8.1/README.md
+-rw-rw-rw-   0        0        0      723 2023-07-29 16:54:34.351404 easyencryption-0.1.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1994 2023-07-29 16:54:20.000000 easyencryption-0.1.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:54:34.322880 easyencryption-0.1.8.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-29 16:54:34.332889 easyencryption-0.1.8.1/src/easyencryption/
+-rw-rw-rw-   0        0        0      467 2023-07-29 16:43:27.000000 easyencryption-0.1.8.1/src/easyencryption/__init__.py
+-rw-rw-rw-   0        0        0     1492 2023-07-29 16:46:57.000000 easyencryption-0.1.8.1/src/easyencryption/aes.py
+-rw-rw-rw-   0        0        0     1672 2023-07-29 16:47:28.000000 easyencryption-0.1.8.1/src/easyencryption/custom.py
+-rw-rw-rw-   0        0        0     1457 2023-07-29 16:48:16.000000 easyencryption-0.1.8.1/src/easyencryption/ecc.py
+-rw-rw-rw-   0        0        0     1131 2023-07-29 16:48:48.000000 easyencryption-0.1.8.1/src/easyencryption/fernet.py
+-rw-rw-rw-   0        0        0     2029 2023-07-29 16:50:15.000000 easyencryption-0.1.8.1/src/easyencryption/rsa.py
+-rw-rw-rw-   0        0        0     2043 2023-07-29 16:50:30.000000 easyencryption-0.1.8.1/src/easyencryption/sha.py
+-rw-rw-rw-   0        0        0     1878 2023-07-29 16:44:10.000000 easyencryption-0.1.8.1/src/easyencryption/xor.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:54:34.349405 easyencryption-0.1.8.1/src/easyencryption.egg-info/
+-rw-rw-rw-   0        0        0     3674 2023-07-29 16:54:34.000000 easyencryption-0.1.8.1/src/easyencryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-07-29 16:54:34.000000 easyencryption-0.1.8.1/src/easyencryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 16:54:34.000000 easyencryption-0.1.8.1/src/easyencryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-29 16:54:34.000000 easyencryption-0.1.8.1/src/easyencryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-29 16:54:34.000000 easyencryption-0.1.8.1/src/easyencryption.egg-info/top_level.txt
```

### Comparing `easyencryption-0.1.8/PKG-INFO` & `easyencryption-0.1.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.8
+Version: 0.1.8.1
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
@@ -33,14 +33,15 @@
 We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
 AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
 RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
 SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
 ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.
+XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.
 Custom - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA hashing because of the checking methods.<br /><br />
 
 This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
 
 **WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
 
 # Information
```

### Comparing `easyencryption-0.1.8/README.md` & `easyencryption-0.1.8.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
 AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
 RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
 SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
 ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.
+XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.
 Custom - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA hashing because of the checking methods.<br /><br />
 
 This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
 
 **WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
 
 # Information
```

### Comparing `easyencryption-0.1.8/setup.cfg` & `easyencryption-0.1.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8/setup.py` & `easyencryption-0.1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_desc = open("README.md", "r")
 long_description = long_desc.read()
 ##with open('src/easyencryption/__init__.py', 'r') as f:
     ##version = [line.split('=')[1].strip(" '\"") for line in f.read().splitlines() if line.startswith('__version__')][0]
-version = "0.1.8"
+version = "0.1.8.1"
 
 setup(
     name='easyencryption',
     version=version,
     description='A very easy way to encrypt data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `easyencryption-0.1.8/src/easyencryption/aes.py` & `easyencryption-0.1.8.1/src/easyencryption/aes.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8/src/easyencryption/custom.py` & `easyencryption-0.1.8.1/src/easyencryption/custom.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8/src/easyencryption/ecc.py` & `easyencryption-0.1.8.1/src/easyencryption/ecc.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8/src/easyencryption/fernet.py` & `easyencryption-0.1.8.1/src/easyencryption/fernet.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8/src/easyencryption/rsa.py` & `easyencryption-0.1.8.1/src/easyencryption/rsa.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8/src/easyencryption/sha.py` & `easyencryption-0.1.8.1/src/easyencryption/sha.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8/src/easyencryption/xor.py` & `easyencryption-0.1.8.1/src/easyencryption/xor.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8/src/easyencryption.egg-info/PKG-INFO` & `easyencryption-0.1.8.1/src/easyencryption.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.8
+Version: 0.1.8.1
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
@@ -33,14 +33,15 @@
 We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
 AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
 RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
 SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
 ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.
+XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.
 Custom - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA hashing because of the checking methods.<br /><br />
 
 This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
 
 **WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
 
 # Information
```

