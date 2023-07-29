# Comparing `tmp/secrets-vault-0.2.5.tar.gz` & `tmp/secrets-vault-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrets-vault-0.2.5.tar", last modified: Sat Jul 29 11:52:16 2023, max compression
+gzip compressed data, was "secrets-vault-0.2.6.tar", last modified: Sat Jul 29 18:29:02 2023, max compression
```

## Comparing `secrets-vault-0.2.5.tar` & `secrets-vault-0.2.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:52:16.834496 secrets-vault-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-07-29 11:52:16.834496 secrets-vault-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:52:16.830496 secrets-vault-0.2.5/secrets_vault/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/secrets_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/secrets_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/secrets_vault/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/secrets_vault/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/secrets_vault/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/secrets_vault/vault.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/secrets_vault/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:52:16.830496 secrets-vault-0.2.5/secrets_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-07-29 11:52:16.000000 secrets-vault-0.2.5/secrets_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-29 11:52:16.000000 secrets-vault-0.2.5/secrets_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 11:52:16.000000 secrets-vault-0.2.5/secrets_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-29 11:52:16.000000 secrets-vault-0.2.5/secrets_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-29 11:52:16.000000 secrets-vault-0.2.5/secrets_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 11:52:16.000000 secrets-vault-0.2.5/secrets_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 11:52:16.834496 secrets-vault-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:52:16.834496 secrets-vault-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/tests/test_backwards_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/tests/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:29:02.062596 secrets-vault-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-07-29 18:29:02.062596 secrets-vault-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:29:02.062596 secrets-vault-0.2.6/secrets_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/secrets_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/secrets_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/secrets_vault/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/secrets_vault/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/secrets_vault/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/secrets_vault/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/secrets_vault/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:29:02.062596 secrets-vault-0.2.6/secrets_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-07-29 18:29:01.000000 secrets-vault-0.2.6/secrets_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-29 18:29:02.000000 secrets-vault-0.2.6/secrets_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 18:29:01.000000 secrets-vault-0.2.6/secrets_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-29 18:29:01.000000 secrets-vault-0.2.6/secrets_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-29 18:29:01.000000 secrets-vault-0.2.6/secrets_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 18:29:01.000000 secrets-vault-0.2.6/secrets_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 18:29:02.062596 secrets-vault-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:29:02.062596 secrets-vault-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/tests/test_backwards_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/tests/test_vault.py
```

### Comparing `secrets-vault-0.2.5/LICENSE` & `secrets-vault-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.5/PKG-INFO` & `secrets-vault-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.2.5
+Version: 0.2.6
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -54,15 +54,15 @@
 
 > postgres://user:pass@localhost:5432/dev
 ```
 
 5. Consume secrets as environment variables:
 
 ```bash
-$ secrets envify production -o dotenv
+$ secrets envify -o dotenv
 
 $ cat .env
 
 > DATABASE_URL=postgres://...
 > REDIS_URL=redis://...
 > COOKIE_SECRET=abc123
 ```
@@ -264,16 +264,16 @@
 
 abc123
 ```
 
 Dump output to a dotenv file:
 
 ```bash
-$ secrets envify aws-credentials -o dotenv
-$ cat .env
+$ secrets envify aws-credentials -o .env.aws
+$ cat .env.aws
 > AWS_ACCESS_KEY_ID=abc123
 > AWS_SECRET_ACCESS_KEY=abc456
 ```
 
 ## Providing the master.key file
 
 ### File on disk
```

### Comparing `secrets-vault-0.2.5/README.md` & `secrets-vault-0.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 > postgres://user:pass@localhost:5432/dev
 ```
 
 5. Consume secrets as environment variables:
 
 ```bash
-$ secrets envify production -o dotenv
+$ secrets envify -o dotenv
 
 $ cat .env
 
 > DATABASE_URL=postgres://...
 > REDIS_URL=redis://...
 > COOKIE_SECRET=abc123
 ```
@@ -249,16 +249,16 @@
 
 abc123
 ```
 
 Dump output to a dotenv file:
 
 ```bash
-$ secrets envify aws-credentials -o dotenv
-$ cat .env
+$ secrets envify aws-credentials -o .env.aws
+$ cat .env.aws
 > AWS_ACCESS_KEY_ID=abc123
 > AWS_SECRET_ACCESS_KEY=abc456
 ```
 
 ## Providing the master.key file
 
 ### File on disk
```

### Comparing `secrets-vault-0.2.5/secrets_vault/__main__.py` & `secrets-vault-0.2.6/secrets_vault/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,36 +134,38 @@
     help="Prints a secret as an environment variable (eg. KEY=value). If no specific key is provided, all secrets are printed."
 )
 @click.argument("key", required=False)
 @click.option("-e", "--export", is_flag=True, help="Include the export modifier for each environment variable.")
 @click.option(
     "-o",
     "--output",
-    type=click.Choice(["dotenv", "stdout"]),
     default="stdout",
-    help="Output the result in the specified format.",
+    help="Output the result to stdout or a given dotenv file. For example --output .env.staging",
 )
 @click.option("--raw", is_flag=True, help="When raw mode is enabled, the key=value is printed as stored on the vault.")
 @click.pass_context
 def envify(ctx, key, export, output, raw):
     def serialize_key(k):
         return k if raw else k.upper().replace("-", "_")
 
     def write(obj):
         serialized = [
             f"{'export ' if export else ''}{serialize_key(k)}={serialize(v, 'dotenv')}" for k, v in obj.items()
         ]
-        if output == "dotenv":
-            with open(".env", "w") as f:
-                f.write("\n".join(serialized))
-        elif output == "stdout":
+        if output == "stdout":
             for line in serialized:
                 click.echo(line)
+        elif output == "dotenv":
+            with open(".env", "w") as f:
+                f.write("# generated by secrets-vault\n")
+                f.write("\n".join(serialized))
         else:
-            raise NotImplementedError(f"Unsupported output format: {output}")
+            with open(output, "w") as f:
+                f.write("# generated by secrets-vault\n")
+                f.write("\n".join(serialized))
 
     def handler(vault):
         if key:
             value = vault.get(key)
             if isinstance(value, dict):
                 write(value)
             else:
```

### Comparing `secrets-vault-0.2.5/secrets_vault/backends.py` & `secrets-vault-0.2.6/secrets_vault/backends.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.5/secrets_vault/constants.py` & `secrets-vault-0.2.6/secrets_vault/constants.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.5/secrets_vault/vault.py` & `secrets-vault-0.2.6/secrets_vault/vault.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.5/secrets_vault.egg-info/PKG-INFO` & `secrets-vault-0.2.6/secrets_vault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.2.5
+Version: 0.2.6
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -54,15 +54,15 @@
 
 > postgres://user:pass@localhost:5432/dev
 ```
 
 5. Consume secrets as environment variables:
 
 ```bash
-$ secrets envify production -o dotenv
+$ secrets envify -o dotenv
 
 $ cat .env
 
 > DATABASE_URL=postgres://...
 > REDIS_URL=redis://...
 > COOKIE_SECRET=abc123
 ```
@@ -264,16 +264,16 @@
 
 abc123
 ```
 
 Dump output to a dotenv file:
 
 ```bash
-$ secrets envify aws-credentials -o dotenv
-$ cat .env
+$ secrets envify aws-credentials -o .env.aws
+$ cat .env.aws
 > AWS_ACCESS_KEY_ID=abc123
 > AWS_SECRET_ACCESS_KEY=abc456
 ```
 
 ## Providing the master.key file
 
 ### File on disk
```

### Comparing `secrets-vault-0.2.5/setup.py` & `secrets-vault-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.5/tests/test_backends.py` & `secrets-vault-0.2.6/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.5/tests/test_backwards_compat.py` & `secrets-vault-0.2.6/tests/test_backwards_compat.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.5/tests/test_vault.py` & `secrets-vault-0.2.6/tests/test_vault.py`

 * *Files identical despite different names*

