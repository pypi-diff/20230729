# Comparing `tmp/cryptul-0.0.3.tar.gz` & `tmp/cryptul-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptul-0.0.3.tar", last modified: Thu Jun 29 07:28:46 2023, max compression
+gzip compressed data, was "cryptul-0.0.4.tar", last modified: Sat Jul 29 10:55:48 2023, max compression
```

## Comparing `cryptul-0.0.3.tar` & `cryptul-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 frollo    (1000) frollo    (1000)        0 2023-06-29 07:28:46.128785 cryptul-0.0.3/
--rw-r--r--   0 frollo    (1000) frollo    (1000)      527 2023-06-29 07:28:46.128785 cryptul-0.0.3/PKG-INFO
--rw-r--r--   0 frollo    (1000) frollo    (1000)       40 2023-06-28 10:33:15.000000 cryptul-0.0.3/README.md
--rw-r--r--   0 frollo    (1000) frollo    (1000)      582 2023-06-29 07:22:51.000000 cryptul-0.0.3/pyproject.toml
--rw-r--r--   0 frollo    (1000) frollo    (1000)       38 2023-06-29 07:28:46.128785 cryptul-0.0.3/setup.cfg
-drwxr-xr-x   0 frollo    (1000) frollo    (1000)        0 2023-06-29 07:28:46.125451 cryptul-0.0.3/src/
-drwxr-xr-x   0 frollo    (1000) frollo    (1000)        0 2023-06-29 07:28:46.128785 cryptul-0.0.3/src/cryptul/
--rw-r--r--   0 frollo    (1000) frollo    (1000)       30 2023-06-28 11:41:14.000000 cryptul-0.0.3/src/cryptul/__init__.py
--rw-r--r--   0 frollo    (1000) frollo    (1000)    10574 2023-06-29 07:28:18.000000 cryptul-0.0.3/src/cryptul/_cryptul.py
-drwxr-xr-x   0 frollo    (1000) frollo    (1000)        0 2023-06-29 07:28:46.128785 cryptul-0.0.3/src/cryptul.egg-info/
--rw-r--r--   0 frollo    (1000) frollo    (1000)      527 2023-06-29 07:28:46.000000 cryptul-0.0.3/src/cryptul.egg-info/PKG-INFO
--rw-r--r--   0 frollo    (1000) frollo    (1000)      212 2023-06-29 07:28:46.000000 cryptul-0.0.3/src/cryptul.egg-info/SOURCES.txt
--rw-r--r--   0 frollo    (1000) frollo    (1000)        1 2023-06-29 07:28:46.000000 cryptul-0.0.3/src/cryptul.egg-info/dependency_links.txt
--rw-r--r--   0 frollo    (1000) frollo    (1000)        8 2023-06-29 07:28:46.000000 cryptul-0.0.3/src/cryptul.egg-info/top_level.txt
+drwxr-xr-x   0 frollo    (1000) frollo    (1000)        0 2023-07-29 10:55:48.879854 cryptul-0.0.4/
+-rw-r--r--   0 frollo    (1000) frollo    (1000)      527 2023-07-29 10:55:48.879854 cryptul-0.0.4/PKG-INFO
+-rw-r--r--   0 frollo    (1000) frollo    (1000)       40 2023-06-28 10:33:15.000000 cryptul-0.0.4/README.md
+-rw-r--r--   0 frollo    (1000) frollo    (1000)      631 2023-07-29 10:55:28.000000 cryptul-0.0.4/pyproject.toml
+-rw-r--r--   0 frollo    (1000) frollo    (1000)       38 2023-07-29 10:55:48.879854 cryptul-0.0.4/setup.cfg
+drwxr-xr-x   0 frollo    (1000) frollo    (1000)        0 2023-07-29 10:55:48.869854 cryptul-0.0.4/src/
+drwxr-xr-x   0 frollo    (1000) frollo    (1000)        0 2023-07-29 10:55:48.876521 cryptul-0.0.4/src/cryptul/
+-rw-r--r--   0 frollo    (1000) frollo    (1000)       30 2023-06-28 11:41:14.000000 cryptul-0.0.4/src/cryptul/__init__.py
+-rw-r--r--   0 frollo    (1000) frollo    (1000)    10435 2023-07-29 10:52:00.000000 cryptul-0.0.4/src/cryptul/_cryptul.py
+drwxr-xr-x   0 frollo    (1000) frollo    (1000)        0 2023-07-29 10:55:48.876521 cryptul-0.0.4/src/cryptul.egg-info/
+-rw-r--r--   0 frollo    (1000) frollo    (1000)      527 2023-07-29 10:55:48.000000 cryptul-0.0.4/src/cryptul.egg-info/PKG-INFO
+-rw-r--r--   0 frollo    (1000) frollo    (1000)      246 2023-07-29 10:55:48.000000 cryptul-0.0.4/src/cryptul.egg-info/SOURCES.txt
+-rw-r--r--   0 frollo    (1000) frollo    (1000)        1 2023-07-29 10:55:48.000000 cryptul-0.0.4/src/cryptul.egg-info/dependency_links.txt
+-rw-r--r--   0 frollo    (1000) frollo    (1000)       33 2023-07-29 10:55:48.000000 cryptul-0.0.4/src/cryptul.egg-info/requires.txt
+-rw-r--r--   0 frollo    (1000) frollo    (1000)        8 2023-07-29 10:55:48.000000 cryptul-0.0.4/src/cryptul.egg-info/top_level.txt
```

### Comparing `cryptul-0.0.3/PKG-INFO` & `cryptul-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptul
-Version: 0.0.3
+Version: 0.0.4
 Summary: A set of tools for crypto CTFs and more
 Author-email: Frollo <fral01@protonmail.com>
 Project-URL: Homepage, https://github.com/Frollamma/cryptul/
 Project-URL: Bug Tracker, https://github.com/Frollamma/cryptul/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cryptul-0.0.3/pyproject.toml` & `cryptul-0.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cryptul"
-version = "0.0.3"
-authors = [
-  { name="Frollo", email="fral01@protonmail.com" },
-]
+version = "0.0.4"
+authors = [{ name = "Frollo", email = "fral01@protonmail.com" }]
 description = "A set of tools for crypto CTFs and more"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
 ]
+dependencies = ["pycryptodome>=3.18.0", "sympy>=1.12"]
 
 [project.urls]
 "Homepage" = "https://github.com/Frollamma/cryptul/"
-"Bug Tracker" = "https://github.com/Frollamma/cryptul/issues"
+"Bug Tracker" = "https://github.com/Frollamma/cryptul/issues"
```

### Comparing `cryptul-0.0.3/src/cryptul/_cryptul.py` & `cryptul-0.0.4/src/cryptul/_cryptul.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+import math
+import random
 from string import printable
+
+from Crypto.Util.number import GCD, bytes_to_long, inverse, isPrime
 from Crypto.Util.Padding import pad
-from Crypto.Util.number import isPrime, inverse, bytes_to_long, GCD
-from sympy import Mod
-import random
-from sympy import integer_nthroot, sqrt
-import math
+from sympy import Mod, integer_nthroot, sqrt
 
 # Remember:
 # from sympy.ntheory import discrete_log as dlog
 # from Crypto.Util.number import long_to_bytes
 # import hashlib
 # from Crypto.Cipher import AES
 # from Crypto.Util.Padding import unpad
@@ -71,20 +71,20 @@
 # Block ciphers
 
 
 def split_in_blocks(message: bytes, block_length: int):
     number_of_full_blocks = len(message) // block_length
 
     blocks = [
-        message[i * block_length: (i + 1) * block_length]
+        message[i * block_length : (i + 1) * block_length]
         for i in range(number_of_full_blocks)
     ]
 
     if len(message) % block_length != 0:
-        blocks.append(pad(message[number_of_full_blocks + 1:], block_length))
+        blocks.append(pad(message[number_of_full_blocks + 1 :], block_length))
 
     return blocks
 
 
 # RSA
 
 # Hashing functions
@@ -116,16 +116,15 @@
         (r1, s1) is the first signature
         (r2, s2) is the second signature
         """
 
         if check:
             if not (
                 isinstance(p, int),
-                isinstance(q, int) and isinstance(
-                    g, int) and isinstance(y, int),
+                isinstance(q, int) and isinstance(g, int) and isinstance(y, int),
             ):
                 raise ValueError("p, q, g, y must be an integers")
 
             if not isinstance(k, int):
                 if k != None:
                     raise ValueError("k must be an integer or None")
             else:
@@ -152,16 +151,15 @@
                             "You have to set as integer at least one between h and g"
                         )
                     else:
                         g = pow(h, (p - 1) // q, p)
             else:
                 if h != None:
                     if g != pow(h, (p - 1) // q, p):
-                        raise ValueError(
-                            "g must be equal to pow(h, (p - 1) // q, p)")
+                        raise ValueError("g must be equal to pow(h, (p - 1) // q, p)")
 
             if not isinstance(y, int):
                 if y != None:
                     raise ValueError("y must be an integer or None")
                 else:
                     if x == None:
                         raise ValueError(
@@ -222,16 +220,15 @@
             r = Mod(pow(self.g, k, self.p), self.q)
             # r = pow(self.g, k, self.p) % self.q
             s = inverse(k, self.q) * Mod(self.H(message) + self.x * r, self.q)
 
         return r, s
 
     def verify(self, message: int, r: int, s: int):
-        a = pow(self.g, self.H(message) *
-                Mod(inverse(s, self.q), self.q), self.p)
+        a = pow(self.g, self.H(message) * Mod(inverse(s, self.q), self.q), self.p)
         b = pow(self.y, Mod(r * inverse(s, self.q), self.q), self.p)
 
         is_signature_valid = (a * b % self.p) % self.q == r
 
         return is_signature_valid
 
     def get_x_given_message_and_seed(self, m, r: int, s: int, k=None) -> int:
@@ -290,87 +287,75 @@
         # k2 = Mod((a - b) * e, self.q)
 
         return k0  # , k1, k2
 
 
 # RNG (Random number generation)
 class LCGCracker:
-    def __init__(self, x: list[int] = None, n = None, a = None, b = None):
+    def __init__(self, x: list[int] = None, n=None, a=None, b=None):
         self.x = x
         self.n = n
         self.a = a
         self.b = b
 
     def next(self):
         assert self.x and len(self.x) >= 1, "At least one value of x is required"
 
         last_index = len(self.x) - 1
-        next_value = Mod(self.a * self.x[last_index] + self.b, self.n)  
+        next_value = Mod(self.a * self.x[last_index] + self.b, self.n)
         self.x.append(next_value)
 
         return next_value
-    
+
     def get_b(self):
         assert self.n, "n is required"
         assert self.a, "a is required"
         assert self.x and len(self.x) >= 2, "At least two values of x are required"
 
         self.b = Mod(self.x[1] - self.a * self.x[0], self.n)
 
         return self.b
-    
+
     def get_a(self):
         assert self.n, "n is required"
         assert self.x and len(self.x) >= 3, "At least three values of x are required"
 
         h = self.x[2] - self.x[1]
         f = self.x[1] - self.x[0]
 
         self.a = Mod(h * inverse(f, self.n), self.n)
 
-        return self.a        
+        return self.a
 
     def get_n(self):
         """
-        Let x be a sequence generated with LCG, we want to get the modulus n, with this approach we can get it if we have "enough" values of x 
+        Let x be a sequence generated with LCG, we want to get the modulus n, with this approach we can get it if we have "enough" values of x
         """
         assert self.x and len(self.x) >= 4, "At least four values of x are required"
 
-    
-        t = [self.x[i+1] - self.x[i] for i in range(len(self.x) - 1)]
-        z = [t[i - 1] * t[i + 1] - t[i]**2 for i in range(1, len(t) - 1)]
+        t = [self.x[i + 1] - self.x[i] for i in range(len(self.x) - 1)]
+        z = [t[i - 1] * t[i + 1] - t[i] ** 2 for i in range(1, len(t) - 1)]
         self.n = math.gcd(*z)
 
         return self.n
 
+
 class RSA:
     def __init__(self, n, e=65537, d=None, p=None, q=None, phi=None):
         self.n = n
         self.e = e
         self.p = p
         self.q = q
         self.phi = phi
         self.d = d
 
         if p and q:
-            self.phi = (p-1)*(q-1)
-        
+            self.phi = (p - 1) * (q - 1)
+
         if self.phi:
             self.d = inverse(self.e, self.phi)
-    
+
     def encrypt(self, message: int):
         return pow(message, self.e, self.n)
-    
 
     def decrypt(self, enc_message: int):
         return pow(enc_message, self.d, self.n)
-
-
-
-
-
-
-
-        
-    
-
-
```

### Comparing `cryptul-0.0.3/src/cryptul.egg-info/PKG-INFO` & `cryptul-0.0.4/src/cryptul.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptul
-Version: 0.0.3
+Version: 0.0.4
 Summary: A set of tools for crypto CTFs and more
 Author-email: Frollo <fral01@protonmail.com>
 Project-URL: Homepage, https://github.com/Frollamma/cryptul/
 Project-URL: Bug Tracker, https://github.com/Frollamma/cryptul/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

