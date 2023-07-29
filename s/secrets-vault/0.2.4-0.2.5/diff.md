# Comparing `tmp/secrets-vault-0.2.4.tar.gz` & `tmp/secrets-vault-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrets-vault-0.2.4.tar", last modified: Sat Jul 29 10:59:17 2023, max compression
+gzip compressed data, was "secrets-vault-0.2.5.tar", last modified: Sat Jul 29 11:52:16 2023, max compression
```

## Comparing `secrets-vault-0.2.4.tar` & `secrets-vault-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:59:17.126016 secrets-vault-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-29 10:59:17.122016 secrets-vault-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:59:17.122016 secrets-vault-0.2.4/secrets_vault/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/secrets_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/secrets_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/secrets_vault/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/secrets_vault/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/secrets_vault/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/secrets_vault/vault.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/secrets_vault/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:59:17.122016 secrets-vault-0.2.4/secrets_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-29 10:59:17.000000 secrets-vault-0.2.4/secrets_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-29 10:59:17.000000 secrets-vault-0.2.4/secrets_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:59:17.000000 secrets-vault-0.2.4/secrets_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-29 10:59:17.000000 secrets-vault-0.2.4/secrets_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-29 10:59:17.000000 secrets-vault-0.2.4/secrets_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 10:59:17.000000 secrets-vault-0.2.4/secrets_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:59:17.126016 secrets-vault-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:59:17.122016 secrets-vault-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/tests/test_backwards_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-29 10:58:55.000000 secrets-vault-0.2.4/tests/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:52:16.834496 secrets-vault-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-07-29 11:52:16.834496 secrets-vault-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:52:16.830496 secrets-vault-0.2.5/secrets_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/secrets_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/secrets_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/secrets_vault/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/secrets_vault/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/secrets_vault/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/secrets_vault/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/secrets_vault/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:52:16.830496 secrets-vault-0.2.5/secrets_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-07-29 11:52:16.000000 secrets-vault-0.2.5/secrets_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-29 11:52:16.000000 secrets-vault-0.2.5/secrets_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 11:52:16.000000 secrets-vault-0.2.5/secrets_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-29 11:52:16.000000 secrets-vault-0.2.5/secrets_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-29 11:52:16.000000 secrets-vault-0.2.5/secrets_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 11:52:16.000000 secrets-vault-0.2.5/secrets_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 11:52:16.834496 secrets-vault-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:52:16.834496 secrets-vault-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/tests/test_backwards_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-29 11:51:47.000000 secrets-vault-0.2.5/tests/test_vault.py
```

### Comparing `secrets-vault-0.2.4/LICENSE` & `secrets-vault-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.4/PKG-INFO` & `secrets-vault-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.2.4
+Version: 0.2.5
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # secrets-vault
 
-Keep your app secrets encrypted in-repo, automatically decrypt on local dev or deploy.
+Simple tool to keep your app secrets encrypted in-repo, decrypt using a `master.key`.
 
-Inspired by Rails credentials - it pairs nicely with [mrsk](https://mrsk.dev). But it can be used as a standalone CLI tool or as a library. 
+The vault can be YAML (default) or JSON encoded, and is encrypted using [AES-GCM-256 authenticated encryption](https://cryptography.io/en/latest/hazmat/primitives/aead/#cryptography.hazmat.primitives.ciphers.aead.AESGCM).
 
-The vault is YAML encoded and encrypted using [AES-GCM-256 authenticated encryption](https://cryptography.io/en/latest/hazmat/primitives/aead/#cryptography.hazmat.primitives.ciphers.aead.AESGCM).
+Inspired by Rails credentials - it pairs nicely with [mrsk](https://mrsk.dev). But it can be used as a standalone CLI tool or as a library. 
 
 ## Quick start
 
 1. Install it:
 ```bash
 $ pip install secrets-vault
 ```
@@ -32,41 +32,43 @@
  ```bash
 $ secrets init
 
 Generated new secrets vault at ./secrets.yml.enc
 Generated new master key at ./master.key - keep it safe!
  ``` 
 
-3. Edit secrets:
+3. Open vault in your editor:
 ```bash
 $ secrets edit
 
->> Opening secrets file in editor...
-
 # Add your secrets below, comments are supported too.
 # dev:
 #     secret-key: abc123
 #
 # database-url: postgres://user:pass@localhost:5432/dev
 ```
 
 4. Read secrets:
 
 ```bash
-# Via CLI
 $ secrets get database-url
+
 > postgres://user:pass@localhost:5432/dev
 ```
 
-```python
-# In Python
-from secrets_vault import SecretsVault
+5. Consume secrets as environment variables:
 
-vault = SecretsVault()
-foo = vault.get('database-url')
+```bash
+$ secrets envify production -o dotenv
+
+$ cat .env
+
+> DATABASE_URL=postgres://...
+> REDIS_URL=redis://...
+> COOKIE_SECRET=abc123
 ```
 
 **Important:** You should keep the `master.key` secret, do NOT commit it. Ignore it in your `.gitignore` file. The `secrets.yml.enc` file is encrypted and can be committed.
 
 ## CLI usage
 
 You can view the help anytime by running `secrets --help`:
@@ -259,19 +261,21 @@
 ```bash
 $ $(secrets envify --export aws-credentials)
 $ echo $AWS_ACCESS_KEY_ID
 
 abc123
 ```
 
-Or dump multiple secrets to a dotenv file:
+Dump output to a dotenv file:
 
 ```bash
-$ secrets envify aws-credentials >> .env
-$ secrets envify database-url >> .env
+$ secrets envify aws-credentials -o dotenv
+$ cat .env
+> AWS_ACCESS_KEY_ID=abc123
+> AWS_SECRET_ACCESS_KEY=abc456
 ```
 
 ## Providing the master.key file
 
 ### File on disk
 By default, the vault will look for the master key in a file located at `./master.key`.
```

### Comparing `secrets-vault-0.2.4/README.md` & `secrets-vault-0.2.5/secrets_vault.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,29 @@
+Metadata-Version: 2.1
+Name: secrets-vault
+Version: 0.2.5
+Summary: Simple encrypted secrets for Python
+Home-page: https://github.com/anthonynsimon/secrets-vault
+Author: Anthony N. Simon
+License: MIT
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # secrets-vault
 
-Keep your app secrets encrypted in-repo, automatically decrypt on local dev or deploy.
+Simple tool to keep your app secrets encrypted in-repo, decrypt using a `master.key`.
 
-Inspired by Rails credentials - it pairs nicely with [mrsk](https://mrsk.dev). But it can be used as a standalone CLI tool or as a library. 
+The vault can be YAML (default) or JSON encoded, and is encrypted using [AES-GCM-256 authenticated encryption](https://cryptography.io/en/latest/hazmat/primitives/aead/#cryptography.hazmat.primitives.ciphers.aead.AESGCM).
 
-The vault is YAML encoded and encrypted using [AES-GCM-256 authenticated encryption](https://cryptography.io/en/latest/hazmat/primitives/aead/#cryptography.hazmat.primitives.ciphers.aead.AESGCM).
+Inspired by Rails credentials - it pairs nicely with [mrsk](https://mrsk.dev). But it can be used as a standalone CLI tool or as a library. 
 
 ## Quick start
 
 1. Install it:
 ```bash
 $ pip install secrets-vault
 ```
@@ -17,41 +32,43 @@
  ```bash
 $ secrets init
 
 Generated new secrets vault at ./secrets.yml.enc
 Generated new master key at ./master.key - keep it safe!
  ``` 
 
-3. Edit secrets:
+3. Open vault in your editor:
 ```bash
 $ secrets edit
 
->> Opening secrets file in editor...
-
 # Add your secrets below, comments are supported too.
 # dev:
 #     secret-key: abc123
 #
 # database-url: postgres://user:pass@localhost:5432/dev
 ```
 
 4. Read secrets:
 
 ```bash
-# Via CLI
 $ secrets get database-url
+
 > postgres://user:pass@localhost:5432/dev
 ```
 
-```python
-# In Python
-from secrets_vault import SecretsVault
+5. Consume secrets as environment variables:
 
-vault = SecretsVault()
-foo = vault.get('database-url')
+```bash
+$ secrets envify production -o dotenv
+
+$ cat .env
+
+> DATABASE_URL=postgres://...
+> REDIS_URL=redis://...
+> COOKIE_SECRET=abc123
 ```
 
 **Important:** You should keep the `master.key` secret, do NOT commit it. Ignore it in your `.gitignore` file. The `secrets.yml.enc` file is encrypted and can be committed.
 
 ## CLI usage
 
 You can view the help anytime by running `secrets --help`:
@@ -244,19 +261,21 @@
 ```bash
 $ $(secrets envify --export aws-credentials)
 $ echo $AWS_ACCESS_KEY_ID
 
 abc123
 ```
 
-Or dump multiple secrets to a dotenv file:
+Dump output to a dotenv file:
 
 ```bash
-$ secrets envify aws-credentials >> .env
-$ secrets envify database-url >> .env
+$ secrets envify aws-credentials -o dotenv
+$ cat .env
+> AWS_ACCESS_KEY_ID=abc123
+> AWS_SECRET_ACCESS_KEY=abc456
 ```
 
 ## Providing the master.key file
 
 ### File on disk
 By default, the vault will look for the master key in a file located at `./master.key`.
 
@@ -327,7 +346,9 @@
 
 Please check for any existing issues before openning a new Issue. If you'd like to work on something, please open a new Issue describing what you'd like to do before submitting a Pull Request.
 
 
 ## License
 
 See [LICENSE](https://github.com/anthonynsimon/secrets-vault/blob/master/LICENSE).
+
+
```

### Comparing `secrets-vault-0.2.4/secrets_vault/__main__.py` & `secrets-vault-0.2.5/secrets_vault/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 from secrets_vault import SecretsVault, exceptions, constants, __version__
 
 
 def serialize(v, format="yaml"):
     assert format in {"yaml", "json", "dotenv"}
 
+    if isinstance(v, bool) and format == "dotenv":
+        return "1" if v else "0"
     if not v:
         return ""
     if isinstance(v, str):
         return v
     if isinstance(v, int):
         return str(v)
     if isinstance(v, float):
```

### Comparing `secrets-vault-0.2.4/secrets_vault/backends.py` & `secrets-vault-0.2.5/secrets_vault/backends.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.4/secrets_vault/constants.py` & `secrets-vault-0.2.5/secrets_vault/constants.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.4/secrets_vault/vault.py` & `secrets-vault-0.2.5/secrets_vault/vault.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.4/secrets_vault.egg-info/PKG-INFO` & `secrets-vault-0.2.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,14 @@
-Metadata-Version: 2.1
-Name: secrets-vault
-Version: 0.2.4
-Summary: Simple encrypted secrets for Python
-Home-page: https://github.com/anthonynsimon/secrets-vault
-Author: Anthony N. Simon
-License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # secrets-vault
 
-Keep your app secrets encrypted in-repo, automatically decrypt on local dev or deploy.
+Simple tool to keep your app secrets encrypted in-repo, decrypt using a `master.key`.
 
-Inspired by Rails credentials - it pairs nicely with [mrsk](https://mrsk.dev). But it can be used as a standalone CLI tool or as a library. 
+The vault can be YAML (default) or JSON encoded, and is encrypted using [AES-GCM-256 authenticated encryption](https://cryptography.io/en/latest/hazmat/primitives/aead/#cryptography.hazmat.primitives.ciphers.aead.AESGCM).
 
-The vault is YAML encoded and encrypted using [AES-GCM-256 authenticated encryption](https://cryptography.io/en/latest/hazmat/primitives/aead/#cryptography.hazmat.primitives.ciphers.aead.AESGCM).
+Inspired by Rails credentials - it pairs nicely with [mrsk](https://mrsk.dev). But it can be used as a standalone CLI tool or as a library. 
 
 ## Quick start
 
 1. Install it:
 ```bash
 $ pip install secrets-vault
 ```
@@ -32,41 +17,43 @@
  ```bash
 $ secrets init
 
 Generated new secrets vault at ./secrets.yml.enc
 Generated new master key at ./master.key - keep it safe!
  ``` 
 
-3. Edit secrets:
+3. Open vault in your editor:
 ```bash
 $ secrets edit
 
->> Opening secrets file in editor...
-
 # Add your secrets below, comments are supported too.
 # dev:
 #     secret-key: abc123
 #
 # database-url: postgres://user:pass@localhost:5432/dev
 ```
 
 4. Read secrets:
 
 ```bash
-# Via CLI
 $ secrets get database-url
+
 > postgres://user:pass@localhost:5432/dev
 ```
 
-```python
-# In Python
-from secrets_vault import SecretsVault
+5. Consume secrets as environment variables:
 
-vault = SecretsVault()
-foo = vault.get('database-url')
+```bash
+$ secrets envify production -o dotenv
+
+$ cat .env
+
+> DATABASE_URL=postgres://...
+> REDIS_URL=redis://...
+> COOKIE_SECRET=abc123
 ```
 
 **Important:** You should keep the `master.key` secret, do NOT commit it. Ignore it in your `.gitignore` file. The `secrets.yml.enc` file is encrypted and can be committed.
 
 ## CLI usage
 
 You can view the help anytime by running `secrets --help`:
@@ -259,19 +246,21 @@
 ```bash
 $ $(secrets envify --export aws-credentials)
 $ echo $AWS_ACCESS_KEY_ID
 
 abc123
 ```
 
-Or dump multiple secrets to a dotenv file:
+Dump output to a dotenv file:
 
 ```bash
-$ secrets envify aws-credentials >> .env
-$ secrets envify database-url >> .env
+$ secrets envify aws-credentials -o dotenv
+$ cat .env
+> AWS_ACCESS_KEY_ID=abc123
+> AWS_SECRET_ACCESS_KEY=abc456
 ```
 
 ## Providing the master.key file
 
 ### File on disk
 By default, the vault will look for the master key in a file located at `./master.key`.
 
@@ -342,9 +331,7 @@
 
 Please check for any existing issues before openning a new Issue. If you'd like to work on something, please open a new Issue describing what you'd like to do before submitting a Pull Request.
 
 
 ## License
 
 See [LICENSE](https://github.com/anthonynsimon/secrets-vault/blob/master/LICENSE).
-
-
```

### Comparing `secrets-vault-0.2.4/setup.py` & `secrets-vault-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.4/tests/test_backends.py` & `secrets-vault-0.2.5/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.4/tests/test_backwards_compat.py` & `secrets-vault-0.2.5/tests/test_backwards_compat.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.4/tests/test_vault.py` & `secrets-vault-0.2.5/tests/test_vault.py`

 * *Files identical despite different names*

