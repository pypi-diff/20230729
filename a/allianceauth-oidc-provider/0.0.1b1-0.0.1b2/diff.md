# Comparing `tmp/allianceauth_oidc_provider-0.0.1b1.tar.gz` & `tmp/allianceauth_oidc_provider-0.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth_oidc_provider-0.0.1b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "allianceauth_oidc_provider-0.0.1b2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `allianceauth_oidc_provider-0.0.1b1.tar` & `allianceauth_oidc_provider-0.0.1b2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0      347 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/.coveragerc
--rw-r--r--   0        0        0     1342 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/.github/workflows/main.yml
--rw-r--r--   0        0        0      718 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2116 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/.gitignore
--rw-r--r--   0        0        0      631 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      139 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/.prettierignore
--rw-r--r--   0        0        0       88 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/.prettierrc
--rw-r--r--   0        0        0     1077 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/LICENSE
--rw-r--r--   0        0        0      629 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/Makefile
--rw-r--r--   0        0        0     3172 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/README.md
--rw-r--r--   0        0        0      122 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/__init__.py
--rw-r--r--   0        0        0      647 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/admin.py
--rw-r--r--   0        0        0      281 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/apps.py
--rw-r--r--   0        0        0        0 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/auth_hooks.py
--rw-r--r--   0        0        0      836 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/auth_provider.py
--rw-r--r--   0        0        0     3037 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/migrations/0001_initial.py
--rw-r--r--   0        0        0      613 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/migrations/0002_alter_allianceauthapplication_options_and_more.py
--rw-r--r--   0        0        0        0 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/migrations/__init__.py
--rw-r--r--   0        0        0      772 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/models.py
--rw-r--r--   0        0        0      186 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/signals.py
--rw-r--r--   0        0        0     1392 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/templates/allianceauth_oidc/authorize.html
--rw-r--r--   0        0        0     1294 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/templates/allianceauth_oidc/base.html
--rw-r--r--   0        0        0     2449 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/templates/allianceauth_oidc/denied.html
--rw-r--r--   0        0        0     1268 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/templates/allianceauth_oidc/logout_confirm.html
--rw-r--r--   0        0        0     7133 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/tests/__init__.py
--rw-r--r--   0        0        0    10339 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/tests/test_access.py
--rw-r--r--   0        0        0     1412 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/urls.py
--rw-r--r--   0        0        0     3830 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/views.py
--rw-r--r--   0        0        0     1333 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/pyproject.toml
--rw-r--r--   0        0        0      862 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/runtests.py
--rw-r--r--   0        0        0       67 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/tests/__init__.py
--rw-r--r--   0        0        0      627 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/tests/celery.py
--rw-r--r--   0        0        0     6622 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/tests/test_settings.py
--rw-r--r--   0        0        0      458 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/tests/urls.py
--rw-r--r--   0        0        0      103 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/tests/views.py
--rw-r--r--   0        0        0      290 2023-07-24 09:20:53.060801 allianceauth_oidc_provider-0.0.1b1/tox.ini
--rw-r--r--   0        0        0     4195 1970-01-01 00:00:00.000000 allianceauth_oidc_provider-0.0.1b1/PKG-INFO
+-rw-r--r--   0        0        0      347 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/.coveragerc
+-rw-r--r--   0        0        0     1342 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/.github/workflows/main.yml
+-rw-r--r--   0        0        0      718 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2116 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/.gitignore
+-rw-r--r--   0        0        0      631 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      139 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/.prettierignore
+-rw-r--r--   0        0        0       88 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/.prettierrc
+-rw-r--r--   0        0        0     1077 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/LICENSE
+-rw-r--r--   0        0        0      629 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/Makefile
+-rw-r--r--   0        0        0     3172 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/README.md
+-rw-r--r--   0        0        0      122 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/__init__.py
+-rw-r--r--   0        0        0      647 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/admin.py
+-rw-r--r--   0        0        0      281 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/apps.py
+-rw-r--r--   0        0        0        0 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/auth_hooks.py
+-rw-r--r--   0        0        0      836 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/auth_provider.py
+-rw-r--r--   0        0        0     3037 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/migrations/0001_initial.py
+-rw-r--r--   0        0        0      613 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/migrations/0002_alter_allianceauthapplication_options_and_more.py
+-rw-r--r--   0        0        0        0 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/migrations/__init__.py
+-rw-r--r--   0        0        0      772 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/models.py
+-rw-r--r--   0        0        0      186 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/signals.py
+-rw-r--r--   0        0        0      143 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/tasks.py
+-rw-r--r--   0        0        0     1392 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/templates/allianceauth_oidc/authorize.html
+-rw-r--r--   0        0        0     1294 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/templates/allianceauth_oidc/base.html
+-rw-r--r--   0        0        0     2449 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/templates/allianceauth_oidc/denied.html
+-rw-r--r--   0        0        0     1268 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/templates/allianceauth_oidc/logout_confirm.html
+-rw-r--r--   0        0        0     7133 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/tests/__init__.py
+-rw-r--r--   0        0        0    10339 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/tests/test_access.py
+-rw-r--r--   0        0        0     1412 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/urls.py
+-rw-r--r--   0        0        0     3830 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/views.py
+-rw-r--r--   0        0        0     1333 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/pyproject.toml
+-rw-r--r--   0        0        0      862 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/runtests.py
+-rw-r--r--   0        0        0       67 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/tests/__init__.py
+-rw-r--r--   0        0        0      627 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/tests/celery.py
+-rw-r--r--   0        0        0     6649 2023-07-29 11:27:24.349127 allianceauth_oidc_provider-0.0.1b2/tests/test_settings.py
+-rw-r--r--   0        0        0      458 2023-07-29 11:27:24.353127 allianceauth_oidc_provider-0.0.1b2/tests/urls.py
+-rw-r--r--   0        0        0      103 2023-07-29 11:27:24.353127 allianceauth_oidc_provider-0.0.1b2/tests/views.py
+-rw-r--r--   0        0        0      290 2023-07-29 11:27:24.353127 allianceauth_oidc_provider-0.0.1b2/tox.ini
+-rw-r--r--   0        0        0     4195 1970-01-01 00:00:00.000000 allianceauth_oidc_provider-0.0.1b2/PKG-INFO
```

### Comparing `allianceauth_oidc_provider-0.0.1b1/.github/workflows/main.yml` & `allianceauth_oidc_provider-0.0.1b2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/.github/workflows/publish.yml` & `allianceauth_oidc_provider-0.0.1b2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/.gitignore` & `allianceauth_oidc_provider-0.0.1b2/.gitignore`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/.pre-commit-config.yaml` & `allianceauth_oidc_provider-0.0.1b2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/LICENSE` & `allianceauth_oidc_provider-0.0.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/Makefile` & `allianceauth_oidc_provider-0.0.1b2/Makefile`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/README.md` & `allianceauth_oidc_provider-0.0.1b2/README.md`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/admin.py` & `allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/auth_provider.py` & `allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/auth_provider.py`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/migrations/0001_initial.py` & `allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/migrations/0002_alter_allianceauthapplication_options_and_more.py` & `allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/migrations/0002_alter_allianceauthapplication_options_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/models.py` & `allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/templates/allianceauth_oidc/authorize.html` & `allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/templates/allianceauth_oidc/authorize.html`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/templates/allianceauth_oidc/base.html` & `allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/templates/allianceauth_oidc/base.html`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/templates/allianceauth_oidc/denied.html` & `allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/templates/allianceauth_oidc/denied.html`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/templates/allianceauth_oidc/logout_confirm.html` & `allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/templates/allianceauth_oidc/logout_confirm.html`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/tests/__init__.py` & `allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/tests/test_access.py` & `allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/urls.py` & `allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/allianceauth_oidc/views.py` & `allianceauth_oidc_provider-0.0.1b2/allianceauth_oidc/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/pyproject.toml` & `allianceauth_oidc_provider-0.0.1b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/runtests.py` & `allianceauth_oidc_provider-0.0.1b2/runtests.py`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/tests/celery.py` & `allianceauth_oidc_provider-0.0.1b2/tests/celery.py`

 * *Files identical despite different names*

### Comparing `allianceauth_oidc_provider-0.0.1b1/tests/test_settings.py` & `allianceauth_oidc_provider-0.0.1b2/tests/test_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         }
     }
 }
 
 
 # This is a testing only key and not hooked up to anything so dont even bother...
 pkey = b'LS0tLS1CRUdJTiBSU0EgUFJJVkFURSBLRVktLS0tLQpNSUlKS1FJQkFBS0NBZ0VBc2Vmd1JuTTlneGgzbDBxekxrWThYQzZSdzZpS29sS2dDci9QM1ZURU9xb2FPa0xnCjFlRy9zSzlVSFI2Q1hxQy9obzhwbTJjNzRaMUM3QytxMXRZSThveXd3NEVTcHdSZUNZY2RJcWdLSFh3QzJ3UWoKa1hZekFCamVMT3F4YSs3NG0wV2dlVXB3S3lIWDc5bzJBc2ErQlphTi85SzNaQUNDMVh0MzFhZ1pwVURyT0pSbQpZRkQ3M3ZlMHcvUjJGbTVjY040Uml4azMwL2tEUXRxVUJvSzRZNTB5a3FCV1prMzFVM3k2Z21hbGNYdWtkd2pWClNJMXVGcWNQRWNuRnVVdzhmdVY2OVJDM0NkbkNmbm96MWRTaVZYdXplOWJDMHZIbUV0WDJhcXAxQzcwTnNKUUQKVmpYMnFOVER5QkVJd2paeWZYQksyYldTaEdzcEdXWU1nd1JWbjkvcDZhWHBMQVdGbEVwekI1ckNFS2xkR0pRSQo1ZHJ5OTZrZXVoSTdBK1N5NVoyWTF0UG9jOENvdXRZbkFzQmFWd2w1bVFrc244RE43K0xDakh1NmJZamczNzF3CjZqMEg0Zng4SnRHRGlQRzVSQVJSTHdnSmtvV2syYitldFE1NHllTHJQT3c1a3ViR05jeStnMXVVcU83aFA4aTQKeUx6YjZ0Y3ZVd3U2dHpCbUNQT0pjYW5NQU5MMER3NFRJR1hqeXJDdUUzZGNBSW9DcVVKOEp3eU55OUtDRmNKLwplWUt6VXRuR1h3VjViQ29XRFFsem82VTI5b0NLZmRFNVdNOXR6V0V3aDgvMFNXbUlLZXVQZllDTVBOdW54eWF2ClN3NVpUR2JQRGJCMHVaMm8vdkc5NTZqYVpKZEFFZXZoM1dXWll0V3E3d2JQZS9KTWI1VEp5aDBoUnFjQ0F3RUEKQVFLQ0FnQVBkd3NUQkxlSEt0eFNnWUxiOWUwUFVsa0hlaUk3QkJXM2VYOFhUV1FWZVczNFBKSVE1YVBsTndpSAowM3dmdjdlR2VmRnkrZUZodG1yMzN4anB2Z2RmRmszVFlPZi9Mc2tCNlFYbVdsY3V3dlg0bGY2RmlaSGJZMDRFCjk0M2V4UkpGWlNNVENCNkNFVm9WRnBIMVlkTm81dktIRjRrcm4wUEFUUkJZdVZrcFhXQlZOY2xFZkNXNDl5MTIKajB5b25JVmFwbU0rQlQ0dUpncGJpR2F2dmpOTExZSVU3dTB6elhrUy9kZTB1RG1QaU9EK0cvMTJaaHo0eVNMdApOKzRCTXBoYnE1VXBzbjlHMHZBdVVHOHJHbVhXS24rcXR6dU9YTXJVUGxkQ1pIanlRVWZzWHFGL29BZEdHK0M5CkJvWU5ZL0JGNlRvSWZOazB1NkFCL2pYK09hVTdzSGVZd1ptRHByb0lTMUFXNEVJRktiRld3SjRvM2tia2RkWkUKM0pjOW5oZ0JBYi83ZVV2andnNkdtMUpCYlYxd0RML3JpU0xmNnVkdCtwQlpCTUVZUG1PeStSMGlLeVBlRWZYTgpZaDg3Nks4U25kZ21laFY4cWlraGM1azZxV0FKOFVKRDB0dlBwWFltdHAzVko1R01nOUwxVEJiOGpGbU9pMGdaCnBhalZNM2h5Q3pQTnpJNDVSRTF3WSswVmp4cndyYis3R0lnTVZmV2Vzam1HQ3ErZTkramI2bEhlS3VRODdBdEoKbDNvM3cwa0Q2N1VISHM0aW5uTlBxUC9ISGdtZGxMaGQ0NlFGSTc1b0JmVllHb2FxYUJOMVVOWjVYa0ZMN0NCUApRUTRMR2I5Q3IrdVVRTmc3d3R1MUlqeXhQbGUwWEN0eVNJOXowRnlkWlE4NER3bHVjUUtDQVFFQTNuMVJ5UHlhClc0UDEwUzF5dVN3d09UbFJJWDAvYkFmK3NCQXg1YnMxQkdmWVZpaUxjdFVUUnd6WGNEY2RTdThtOVZTaEpJRjUKclRaNlIzbXNnWHNEWW1COVZFQ1ArY2NGa1NvQ05iNmhWdU1INWMrM1U4bGQ1cHNDY3BOQzA1NGJlK1RONmZwZwplbCt0WlhlK0tQWXRneGVsWDVkVW1PemQ0V1U5UUVBWWswaEFiL1dHMVp1NGpiVjVSS29NNVFreGxMemZGWkNjCnRIallnVVU4MUNIRHhOcGVHaFJOOXh3MThFdlJDVXNWeTlLQmhYTVhHaDUxTW13U1dpRkVjKzZJVWJkTmh2UkUKOCtqYSszdWo2ZVBaa1RLeXVhUXBENG0yRGpiUXpGS0s2ZzRIL2VsTmpnUVZqRVhNY2RVS0Z5LzFvYnE0aTY0cQoxNjF1dU1wUWdMS0ZpUUtDQVFFQXpMT1UrbTlTUDZnOWs0ckdRQXVpaDN2ZzRoU1h6em52MFc5NDV1T09kOG9KClNuTXBDUjZuUUdTSzFocDJRbUNuZHd5OEs3MGU1WS9IMXZIbDBJckZ0VVA1WjI1OGZka2pzZ0xGVFlJSjVRYmoKRDFQdTNSbGtaMnE5aFJnYlFIQ1N3T00rdmZYdHY4UUpZVWFDenpCdUplK1JqbDZzTkk0c2JDcW4yUEF0b1pTMApuNGpvYmx6ZDRpeUkzNjFtNVZwbjFCSTlULzVPOEViM1hKZlVhc1B4RVRaOG1xSVBWaGtxZUZJVmJyc3pZcTF6CklMMnhMSEw4ckVOREpNdno3QVhxT3RiTlJTOUJSTFVjM04rV01NRGhod2w4VGZVUFcrN21VQ0xrbnQrM0YyL08KZ0lOT0dXQ1lKa2NST0FDSlM1Vk1JcnlQb2pEN2plaE9CMnhrK1ZhT3J3S0NBUUFjSDRNakFLc1NQay9vTFBKLwpiWko2NlQvVUY5ellidnBHandWL29IWkhKRWs0T3MvRnFDRlRyYy9kbzFuVWl2NUZySGppQUd1ODlWSG5qdjI3Ck1DMXhWZmtCbVZlWm53cVpHdEpFc04vNzk1NmI4ZkdlYWFtdzZJOGFwSHFoL1M1RUx0dklZNW1tWGttd3RiNFgKdDJaeFY1L1R3WEUwRTF6SWpOOTlLNXp2b1Faa0lJajJuMFJveFRPYTlsUEM3N0tRdG44TVhzY3dHTVpsTUxkTApxU2p4elJodisza1BiMFZ5Sm1NNTVYL1B6OEFIZWxERlFHeFgvMGtpazJudnJZc1ZxVEhuaVNEZUkrVHFQT3F2Ck9kbmFmS29TeFNsYmlYQzF3MEFKVTdXemVDcVNjZGNYeUhSZzBzSFE4YmpnelhNakNsTWhkTlo5aExLbU1ReVQKOS96aEFvSUJBUURKS201czBudWN6V1IrRzNJS3ZLUmp5dXpNb1Bvemp6ZEx0ZVcxMmNsSGxZZ2QzeUJqc3ZrZwpnZTRpekd5TmZOajJXTkNQbDFMR3ZNN2lRR1RkMVpMSU9WM2ZOS2dwTVB3d1V5SzhzZCt4Y0Z3eDB3VTV5VnR2CmVtbDNZNkpjYUlVQUJCTERzZXlNZVVYU2orMjdXVmZWOWlJd0xIL0ZRamNMc2J1enFRemU3dm0ya21BQkhVaDgKbmRHQko3S29FSGxhNHZYWUtBNUJlU3hjbFdVTjZ6TjcrL1RtTGY4dVdKcnhGWkcwZVVuZFhxRjJlcFNrSHZpSwovYXI5ZldWZi9Nd2NPTDRQa0ludTBLSGx1ZUNxVnRNTDF0bU83eGJCL1B2Zm92clQydnplam1UOHpJMHl5VWVjCnpsaHdsYTVYVmdnMVZ1TTh2REJxVy9KYXZ6NVgvcVZIQW9JQkFRQ3grclFvRTdPRlV5OFNRb1pGVC9ybGZVQk0KV2ZnbUNLbXV6OFFIeW5aL1NsdEFiQS9weG5HTlcvOXRmTVlCMGtxN0l6dlQ2YUwxdmp2NHp2bHFGQ1pPZUpNUApyYXJoREhoZ01UZElyYWRNT1pnUjZxdlYrM3cvMHVFUDZvQ2N1aFdkekZKMFhXOE85UVZKVlN4K0NYdTRseWxGCklhbFBVdkpnalU0aUh3NFBUaUYwWXhoWVNYYXhaeHovZE9PcGdZQUVWWndveW10c1RQT1BqeXUySkppb0lsSVQKai9oeTNmODlNcnhCSmtadEtxNVVTUkdmSi9kR1dYQVJrSGhoaldlR3JocWdVUUlGT0NnUTVlS3puNTBVcEo5cApuMVdjeUJMVzVHdS9kanU0aTVmaGtQMU5MTHlwNWFQUFFLN2hrVyt2d2xaNUcxVzBlUm5KYldwSlZpRVIKLS0tLS1FTkQgUlNBIFBSSVZBVEUgS0VZLS0tLS0K'
-
+pkey = pkey.decode('utf-8')
 OAUTH2_PROVIDER_APPLICATION_MODEL = 'allianceauth_oidc.AllianceAuthApplication'
 OAUTH2_PROVIDER = {
     "OIDC_ENABLED": True,
     "OIDC_RSA_PRIVATE_KEY": base64.b64decode(pkey).decode(),
     "OAUTH2_VALIDATOR_CLASS": "allianceauth_oidc.auth_provider.AllianceAuthOAuth2Validator",
     "SCOPES": {
         "openid": "openid",
```

### Comparing `allianceauth_oidc_provider-0.0.1b1/PKG-INFO` & `allianceauth_oidc_provider-0.0.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-oidc-provider
-Version: 0.0.1b1
+Version: 0.0.1b2
 Summary: Alliance Auth OIDC Provider
 Author-email: AaronKable <aaronkable@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

