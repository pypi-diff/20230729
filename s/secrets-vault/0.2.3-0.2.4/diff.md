# Comparing `tmp/secrets-vault-0.2.3.tar.gz` & `tmp/secrets-vault-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrets-vault-0.2.3.tar", last modified: Thu Jul 27 14:25:14 2023, max compression
+gzip compressed data, was "secrets-vault-0.2.4.tar", last modified: Sat Jul 29 10:59:17 2023, max compression
```

## Comparing `secrets-vault-0.2.3.tar` & `secrets-vault-0.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:25:14.695639 secrets-vault-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-27 14:25:14.695639 secrets-vault-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:25:14.691639 secrets-vault-0.2.3/secrets_vault/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/secrets_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/secrets_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/secrets_vault/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/secrets_vault/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/secrets_vault/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/secrets_vault/vault.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/secrets_vault/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:25:14.691639 secrets-vault-0.2.3/secrets_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-27 14:25:14.000000 secrets-vault-0.2.3/secrets_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-27 14:25:14.000000 secrets-vault-0.2.3/secrets_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:25:14.000000 secrets-vault-0.2.3/secrets_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 14:25:14.000000 secrets-vault-0.2.3/secrets_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 14:25:14.000000 secrets-vault-0.2.3/secrets_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 14:25:14.000000 secrets-vault-0.2.3/secrets_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 14:25:14.695639 secrets-vault-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:25:14.695639 secrets-vault-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/tests/test_backwards_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/tests/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:59:17.126016 secrets-vault-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-29 10:59:17.122016 secrets-vault-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:59:17.122016 secrets-vault-0.2.4/secrets_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/secrets_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/secrets_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/secrets_vault/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/secrets_vault/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/secrets_vault/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/secrets_vault/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/secrets_vault/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:59:17.122016 secrets-vault-0.2.4/secrets_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-29 10:59:17.000000 secrets-vault-0.2.4/secrets_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-29 10:59:17.000000 secrets-vault-0.2.4/secrets_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:59:17.000000 secrets-vault-0.2.4/secrets_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-29 10:59:17.000000 secrets-vault-0.2.4/secrets_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-29 10:59:17.000000 secrets-vault-0.2.4/secrets_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 10:59:17.000000 secrets-vault-0.2.4/secrets_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:59:17.126016 secrets-vault-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:59:17.122016 secrets-vault-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/tests/test_backwards_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/tests/test_vault.py
```

### Comparing `secrets-vault-0.2.3/LICENSE` & `secrets-vault-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.3/PKG-INFO` & `secrets-vault-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.2.3
+Version: 0.2.4
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `secrets-vault-0.2.3/README.md` & `secrets-vault-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.3/secrets_vault/__main__.py` & `secrets-vault-0.2.4/secrets_vault/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,32 +128,50 @@
     with_vault(ctx, handler)
 
 
 @cli.command(
     help="Prints a secret as an environment variable (eg. KEY=value). If no specific key is provided, all secrets are printed."
 )
 @click.argument("key", required=False)
-@click.option("--export", is_flag=True, help="Include the export modified for each environment variable.")
+@click.option("-e", "--export", is_flag=True, help="Include the export modifier for each environment variable.")
+@click.option(
+    "-o",
+    "--output",
+    type=click.Choice(["dotenv", "stdout"]),
+    default="stdout",
+    help="Output the result in the specified format.",
+)
+@click.option("--raw", is_flag=True, help="When raw mode is enabled, the key=value is printed as stored on the vault.")
 @click.pass_context
-def envify(ctx, key, export):
-    puts = lambda k, v: click.echo(
-        f"{'export ' if export else ''}{k.upper().replace('-', '_')}={serialize(v, 'dotenv')}"
-    )
+def envify(ctx, key, export, output, raw):
+    def serialize_key(k):
+        return k if raw else k.upper().replace("-", "_")
+
+    def write(obj):
+        serialized = [
+            f"{'export ' if export else ''}{serialize_key(k)}={serialize(v, 'dotenv')}" for k, v in obj.items()
+        ]
+        if output == "dotenv":
+            with open(".env", "w") as f:
+                f.write("\n".join(serialized))
+        elif output == "stdout":
+            for line in serialized:
+                click.echo(line)
+        else:
+            raise NotImplementedError(f"Unsupported output format: {output}")
 
     def handler(vault):
         if key:
             value = vault.get(key)
             if isinstance(value, dict):
-                for k, v in value.items():
-                    puts(k, v)
+                write(value)
             else:
-                puts(key, value)
+                write({key: value})
         else:
-            for k, v in vault.secrets.items():
-                puts(k, v)
+            write(vault.secrets)
 
     with_vault(ctx, handler)
 
 
 @cli.command(
     help="Store a secret. If the secret already exists, it will be overwritten. For example: `secrets set foo bar`"
 )
```

### Comparing `secrets-vault-0.2.3/secrets_vault/backends.py` & `secrets-vault-0.2.4/secrets_vault/backends.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.3/secrets_vault/constants.py` & `secrets-vault-0.2.4/secrets_vault/constants.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.3/secrets_vault/vault.py` & `secrets-vault-0.2.4/secrets_vault/vault.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.3/secrets_vault.egg-info/PKG-INFO` & `secrets-vault-0.2.4/secrets_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.2.3
+Version: 0.2.4
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `secrets-vault-0.2.3/setup.py` & `secrets-vault-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.3/tests/test_backends.py` & `secrets-vault-0.2.4/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.3/tests/test_backwards_compat.py` & `secrets-vault-0.2.4/tests/test_backwards_compat.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.3/tests/test_vault.py` & `secrets-vault-0.2.4/tests/test_vault.py`

 * *Files identical despite different names*

