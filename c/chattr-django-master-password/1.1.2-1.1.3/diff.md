# Comparing `tmp/chattr-django-master-password-1.1.2.tar.gz` & `tmp/chattr-django-master-password-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chattr-django-master-password-1.1.2.tar", last modified: Sun Mar  5 08:53:39 2023, max compression
+gzip compressed data, was "chattr-django-master-password-1.1.3.tar", last modified: Sat Jul 29 14:16:55 2023, max compression
```

## Comparing `chattr-django-master-password-1.1.2.tar` & `chattr-django-master-password-1.1.3.tar`

### file list

```diff
@@ -1,32 +1,30 @@
-drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-03-05 08:53:39.658959 chattr-django-master-password-1.1.2/
--rw-rw-r--   0 harsh     (1000) harsh     (1000)     1110 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.2/LICENSE
--rw-rw-r--   0 harsh     (1000) harsh     (1000)       37 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.2/MANIFEST.in
--rw-rw-r--   0 harsh     (1000) harsh     (1000)      395 2023-03-05 08:53:39.658959 chattr-django-master-password-1.1.2/PKG-INFO
--rw-rw-r--   0 harsh     (1000) harsh     (1000)        0 2023-03-05 08:50:10.000000 chattr-django-master-password-1.1.2/README.rst
-drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-03-05 08:53:39.658959 chattr-django-master-password-1.1.2/chattr_django_master_password/
--rw-rw-r--   0 harsh     (1000) harsh     (1000)       22 2023-03-05 08:50:10.000000 chattr-django-master-password-1.1.2/chattr_django_master_password/__init__.py
-drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-03-05 08:53:39.658959 chattr-django-master-password-1.1.2/chattr_django_master_password.egg-info/
--rw-rw-r--   0 harsh     (1000) harsh     (1000)      395 2023-03-05 08:53:39.000000 chattr-django-master-password-1.1.2/chattr_django_master_password.egg-info/PKG-INFO
--rw-rw-r--   0 harsh     (1000) harsh     (1000)      747 2023-03-05 08:53:39.000000 chattr-django-master-password-1.1.2/chattr_django_master_password.egg-info/SOURCES.txt
--rw-rw-r--   0 harsh     (1000) harsh     (1000)        1 2023-03-05 08:53:39.000000 chattr-django-master-password-1.1.2/chattr_django_master_password.egg-info/dependency_links.txt
--rw-rw-r--   0 harsh     (1000) harsh     (1000)      129 2023-03-05 08:53:39.000000 chattr-django-master-password-1.1.2/chattr_django_master_password.egg-info/requires.txt
--rw-rw-r--   0 harsh     (1000) harsh     (1000)       52 2023-03-05 08:53:39.000000 chattr-django-master-password-1.1.2/chattr_django_master_password.egg-info/top_level.txt
-drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-03-05 08:53:39.658959 chattr-django-master-password-1.1.2/master_password/
--rw-rw-r--   0 harsh     (1000) harsh     (1000)       55 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.2/master_password/__init__.py
--rw-rw-r--   0 harsh     (1000) harsh     (1000)      322 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.2/master_password/apps.py
--rw-rw-r--   0 harsh     (1000) harsh     (1000)     5033 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.2/master_password/auth.py
-drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-03-05 08:53:39.658959 chattr-django-master-password-1.1.2/master_password/management/
--rw-rw-r--   0 harsh     (1000) harsh     (1000)        0 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.2/master_password/management/__init__.py
-drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-03-05 08:53:39.658959 chattr-django-master-password-1.1.2/master_password/management/commands/
--rw-rw-r--   0 harsh     (1000) harsh     (1000)        0 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.2/master_password/management/commands/__init__.py
--rw-rw-r--   0 harsh     (1000) harsh     (1000)      797 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.2/master_password/management/commands/make_password.py
-drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-03-05 08:53:39.658959 chattr-django-master-password-1.1.2/master_password/tests/
--rw-rw-r--   0 harsh     (1000) harsh     (1000)        0 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.2/master_password/tests/__init__.py
--rw-rw-r--   0 harsh     (1000) harsh     (1000)     1448 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.2/master_password/tests/settings.py
--rw-rw-r--   0 harsh     (1000) harsh     (1000)     4212 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.2/master_password/tests/tests.py
--rw-rw-r--   0 harsh     (1000) harsh     (1000)      314 2023-03-05 08:50:10.000000 chattr-django-master-password-1.1.2/pyproject.toml
--rw-rw-r--   0 harsh     (1000) harsh     (1000)       99 2023-03-05 08:53:39.658959 chattr-django-master-password-1.1.2/setup.cfg
--rw-rw-r--   0 harsh     (1000) harsh     (1000)     1508 2023-03-05 08:51:23.000000 chattr-django-master-password-1.1.2/setup.py
-drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-03-05 08:53:39.658959 chattr-django-master-password-1.1.2/tests/
--rw-rw-r--   0 harsh     (1000) harsh     (1000)        0 2023-03-05 08:50:10.000000 chattr-django-master-password-1.1.2/tests/__init__.py
--rw-rw-r--   0 harsh     (1000) harsh     (1000)      110 2023-03-05 08:50:10.000000 chattr-django-master-password-1.1.2/tests/test_chattr_django_master_password.py
+drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-29 14:16:55.821877 chattr-django-master-password-1.1.3/
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)     1110 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.3/LICENSE
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)       37 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.3/MANIFEST.in
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)      395 2023-07-29 14:16:55.821877 chattr-django-master-password-1.1.3/PKG-INFO
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)        0 2023-03-05 08:50:10.000000 chattr-django-master-password-1.1.3/README.rst
+drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-29 14:16:55.817877 chattr-django-master-password-1.1.3/chattr_django_master_password.egg-info/
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)      395 2023-07-29 14:16:55.000000 chattr-django-master-password-1.1.3/chattr_django_master_password.egg-info/PKG-INFO
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)      705 2023-07-29 14:16:55.000000 chattr-django-master-password-1.1.3/chattr_django_master_password.egg-info/SOURCES.txt
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)        1 2023-07-29 14:16:55.000000 chattr-django-master-password-1.1.3/chattr_django_master_password.egg-info/dependency_links.txt
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)      129 2023-07-29 14:16:55.000000 chattr-django-master-password-1.1.3/chattr_django_master_password.egg-info/requires.txt
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)       22 2023-07-29 14:16:55.000000 chattr-django-master-password-1.1.3/chattr_django_master_password.egg-info/top_level.txt
+drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-29 14:16:55.821877 chattr-django-master-password-1.1.3/master_password/
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)       55 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.3/master_password/__init__.py
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)      322 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.3/master_password/apps.py
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)     5032 2023-07-29 14:05:13.000000 chattr-django-master-password-1.1.3/master_password/auth.py
+drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-29 14:16:55.821877 chattr-django-master-password-1.1.3/master_password/management/
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)        0 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.3/master_password/management/__init__.py
+drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-29 14:16:55.821877 chattr-django-master-password-1.1.3/master_password/management/commands/
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)        0 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.3/master_password/management/commands/__init__.py
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)      797 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.3/master_password/management/commands/make_password.py
+drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-29 14:16:55.821877 chattr-django-master-password-1.1.3/master_password/tests/
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)        0 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.3/master_password/tests/__init__.py
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)     1448 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.3/master_password/tests/settings.py
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)     4212 2022-11-08 07:09:02.000000 chattr-django-master-password-1.1.3/master_password/tests/tests.py
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)      314 2023-07-29 14:13:07.000000 chattr-django-master-password-1.1.3/pyproject.toml
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)       99 2023-07-29 14:16:55.821877 chattr-django-master-password-1.1.3/setup.cfg
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)     1508 2023-07-29 14:13:20.000000 chattr-django-master-password-1.1.3/setup.py
+drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-29 14:16:55.821877 chattr-django-master-password-1.1.3/tests/
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)        0 2023-03-05 08:50:10.000000 chattr-django-master-password-1.1.3/tests/__init__.py
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)      110 2023-03-05 08:50:10.000000 chattr-django-master-password-1.1.3/tests/test_chattr_django_master_password.py
```

### Comparing `chattr-django-master-password-1.1.2/LICENSE` & `chattr-django-master-password-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chattr-django-master-password-1.1.2/chattr_django_master_password.egg-info/SOURCES.txt` & `chattr-django-master-password-1.1.3/chattr_django_master_password.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
-chattr_django_master_password/__init__.py
 chattr_django_master_password.egg-info/PKG-INFO
 chattr_django_master_password.egg-info/SOURCES.txt
 chattr_django_master_password.egg-info/dependency_links.txt
 chattr_django_master_password.egg-info/requires.txt
 chattr_django_master_password.egg-info/top_level.txt
 master_password/__init__.py
 master_password/apps.py
```

### Comparing `chattr-django-master-password-1.1.2/master_password/auth.py` & `chattr-django-master-password-1.1.3/master_password/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import warnings
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.contrib.auth.backends import ModelBackend
 from django.contrib.auth.hashers import check_password, make_password
 from django.utils.module_loading import import_string
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 
 class MasterPasswordMixin(object):
     """
     Adds fallback master password authentication to an existing backend.
 
     On each subclass, you must define:
```

### Comparing `chattr-django-master-password-1.1.2/master_password/management/commands/make_password.py` & `chattr-django-master-password-1.1.3/master_password/management/commands/make_password.py`

 * *Files identical despite different names*

### Comparing `chattr-django-master-password-1.1.2/master_password/tests/settings.py` & `chattr-django-master-password-1.1.3/master_password/tests/settings.py`

 * *Files identical despite different names*

### Comparing `chattr-django-master-password-1.1.2/master_password/tests/tests.py` & `chattr-django-master-password-1.1.3/master_password/tests/tests.py`

 * *Files identical despite different names*

### Comparing `chattr-django-master-password-1.1.2/setup.py` & `chattr-django-master-password-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     else:
         print('Converting `README.md` to reStructuredText to use as long '
               'description.')
         long_description = pypandoc.convert('README.md', 'rst')
 
 setuptools.setup(
     name='chattr-django-master-password',
-    version='1.1.2',
+    version='1.1.3',
     author='Interaction Consortium',
     author_email='studio@interaction.net.au',
     url='https://github.com/ixc/django-master-password',
     description='Login as any user with a master password. Add master '
                 'password support to your custom authentication backend.',
     long_description=locals().get('long_description', ''),
     license='MIT',
```

