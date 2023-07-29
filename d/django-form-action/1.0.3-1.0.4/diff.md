# Comparing `tmp/django-form-action-1.0.3.tar.gz` & `tmp/django-form-action-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-form-action-1.0.3.tar", last modified: Sat Jul 29 20:07:18 2023, max compression
+gzip compressed data, was "django-form-action-1.0.4.tar", last modified: Sat Jul 29 20:17:55 2023, max compression
```

## Comparing `django-form-action-1.0.3.tar` & `django-form-action-1.0.4.tar`

### file list

```diff
@@ -1,10 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:07:18.893686 django-form-action-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-29 20:07:01.000000 django-form-action-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-29 20:07:18.893686 django-form-action-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-29 20:07:01.000000 django-form-action-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:07:18.889686 django-form-action-1.0.3/django_form_action.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-29 20:07:18.000000 django-form-action-1.0.3/django_form_action.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:07:18.889686 django-form-action-1.0.3/form_action/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-29 20:07:01.000000 django-form-action-1.0.3/form_action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 20:07:18.893686 django-form-action-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-29 20:07:01.000000 django-form-action-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:17:55.448672 django-form-action-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-29 20:17:45.000000 django-form-action-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-29 20:17:55.448672 django-form-action-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-29 20:17:45.000000 django-form-action-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:17:55.448672 django-form-action-1.0.4/django_form_action.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-29 20:17:55.000000 django-form-action-1.0.4/django_form_action.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-29 20:17:55.000000 django-form-action-1.0.4/django_form_action.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 20:17:55.000000 django-form-action-1.0.4/django_form_action.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-29 20:17:55.000000 django-form-action-1.0.4/django_form_action.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-29 20:17:55.000000 django-form-action-1.0.4/django_form_action.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:17:55.448672 django-form-action-1.0.4/form_action/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-29 20:17:45.000000 django-form-action-1.0.4/form_action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-29 20:17:45.000000 django-form-action-1.0.4/form_action/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-29 20:17:45.000000 django-form-action-1.0.4/form_action/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-29 20:17:45.000000 django-form-action-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 20:17:55.448672 django-form-action-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-29 20:17:45.000000 django-form-action-1.0.4/setup.py
```

### Comparing `django-form-action-1.0.3/LICENSE` & `django-form-action-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-form-action-1.0.3/PKG-INFO` & `django-form-action-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-form-action
-Version: 1.0.3
+Version: 1.0.4
 Summary: Django action to add an intermediate page to parse form data
 Home-page: https://github.com/sandbox-pokhara/django-form-action
 Author: Pradish Bijukchhe
 Author-email: pradishbijukchhe@gmail.com
 Project-URL: Bug Tracker, https://github.com/sandbox-pokhara/django-form-action/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-form-action-1.0.3/README.md` & `django-form-action-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `django-form-action-1.0.3/setup.py` & `django-form-action-1.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-form-action",
-    version="1.0.3",
+    version="1.0.4",
     author="Pradish Bijukchhe",
     author_email="pradishbijukchhe@gmail.com",
     description="Django action to add an intermediate page to parse form data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sandbox-pokhara/django-form-action",
     project_urls={
```

