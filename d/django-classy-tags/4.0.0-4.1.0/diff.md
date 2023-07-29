# Comparing `tmp/django-classy-tags-4.0.0.tar.gz` & `tmp/django-classy-tags-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-classy-tags-4.0.0.tar", last modified: Thu Dec  1 00:51:15 2022, max compression
+gzip compressed data, was "django-classy-tags-4.1.0.tar", last modified: Sat Jul 29 09:06:05 2023, max compression
```

## Comparing `django-classy-tags-4.0.0.tar` & `django-classy-tags-4.1.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 00:51:15.711333 django-classy-tags-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1486 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      154 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5204 2022-12-01 00:51:15.711333 django-classy-tags-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3956 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 00:51:15.707333 django-classy-tags-4.0.0/classytags/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/classytags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7162 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/classytags/arguments.py
--rw-r--r--   0 runner    (1001) docker     (122)     1321 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/classytags/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     5160 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/classytags/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     1989 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/classytags/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3327 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/classytags/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     7916 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/classytags/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     2647 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/classytags/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2722 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/classytags/values.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 00:51:15.707333 django-classy-tags-4.0.0/django_classy_tags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5204 2022-12-01 00:51:15.000000 django-classy-tags-4.0.0/django_classy_tags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1381 2022-12-01 00:51:15.000000 django-classy-tags-4.0.0/django_classy_tags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 00:51:15.000000 django-classy-tags-4.0.0/django_classy_tags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 00:51:15.000000 django-classy-tags-4.0.0/django_classy_tags.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       12 2022-12-01 00:51:15.000000 django-classy-tags-4.0.0/django_classy_tags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2022-12-01 00:51:15.000000 django-classy-tags-4.0.0/django_classy_tags.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1083 2022-12-01 00:51:15.711333 django-classy-tags-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1685 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 00:51:15.707333 django-classy-tags-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1297 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/context_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 00:51:15.707333 django-classy-tags-4.0.0/tests/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 00:51:15.711333 django-classy-tags-4.0.0/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      228 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/basic.html
--rw-r--r--   0 runner    (1001) docker     (122)      161 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/css.html
--rw-r--r--   0 runner    (1001) docker     (122)      260 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/css2.html
--rw-r--r--   0 runner    (1001) docker     (122)       88 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/easy_base.html
--rw-r--r--   0 runner    (1001) docker     (122)       79 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/easy_inherit.html
--rw-r--r--   0 runner    (1001) docker     (122)       90 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/eat.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 00:51:15.711333 django-classy-tags-4.0.0/tests/templates/errors/
--rw-r--r--   0 runner    (1001) docker     (122)       70 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/errors/failadd.html
--rw-r--r--   0 runner    (1001) docker     (122)      137 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/errors/failbase.html
--rw-r--r--   0 runner    (1001) docker     (122)      137 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/errors/failbase2.html
--rw-r--r--   0 runner    (1001) docker     (122)       74 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/errors/failinc.html
--rw-r--r--   0 runner    (1001) docker     (122)       43 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/errors/failrender.html
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/inclusion.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 00:51:15.711333 django-classy-tags-4.0.0/tests/templates/inherit/
--rw-r--r--   0 runner    (1001) docker     (122)      336 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/inherit/base.html
--rw-r--r--   0 runner    (1001) docker     (122)       90 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/inherit/baseinc.html
--rw-r--r--   0 runner    (1001) docker     (122)      193 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/inherit/extend.html
--rw-r--r--   0 runner    (1001) docker     (122)       32 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/inherit/extinc.html
--rw-r--r--   0 runner    (1001) docker     (122)      248 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/inherit/super_blocks.html
--rw-r--r--   0 runner    (1001) docker     (122)      122 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/named_end.html
--rw-r--r--   0 runner    (1001) docker     (122)      248 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/namespaces.html
--rw-r--r--   0 runner    (1001) docker     (122)      194 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/spaceless.html
--rw-r--r--   0 runner    (1001) docker     (122)        9 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/test.html
--rw-r--r--   0 runner    (1001) docker     (122)      251 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/variables.html
--rw-r--r--   0 runner    (1001) docker     (122)      169 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/with_data.html
--rw-r--r--   0 runner    (1001) docker     (122)      262 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/templates/yui.html
--rw-r--r--   0 runner    (1001) docker     (122)    57003 2022-12-01 00:51:02.000000 django-classy-tags-4.0.0/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:06:05.916200 django-classy-tags-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-29 09:06:05.916200 django-classy-tags-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:06:05.912200 django-classy-tags-4.1.0/classytags/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/classytags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/classytags/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/classytags/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/classytags/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/classytags/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/classytags/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/classytags/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/classytags/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/classytags/values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:06:05.912200 django-classy-tags-4.1.0/django_classy_tags.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-29 09:06:05.000000 django-classy-tags-4.1.0/django_classy_tags.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-29 09:06:05.000000 django-classy-tags-4.1.0/django_classy_tags.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 09:06:05.000000 django-classy-tags-4.1.0/django_classy_tags.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 09:06:05.000000 django-classy-tags-4.1.0/django_classy_tags.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-29 09:06:05.000000 django-classy-tags-4.1.0/django_classy_tags.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 09:06:05.000000 django-classy-tags-4.1.0/django_classy_tags.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-29 09:06:05.916200 django-classy-tags-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:06:05.912200 django-classy-tags-4.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/context_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:06:05.912200 django-classy-tags-4.1.0/tests/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:06:05.916200 django-classy-tags-4.1.0/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/basic.html
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/css.html
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/css2.html
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/easy_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/easy_inherit.html
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/eat.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:06:05.916200 django-classy-tags-4.1.0/tests/templates/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/errors/failadd.html
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/errors/failbase.html
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/errors/failbase2.html
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/errors/failinc.html
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/errors/failrender.html
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/inclusion.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:06:05.916200 django-classy-tags-4.1.0/tests/templates/inherit/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/inherit/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/inherit/baseinc.html
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/inherit/extend.html
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/inherit/extinc.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/inherit/super_blocks.html
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/named_end.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/namespaces.html
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/spaceless.html
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/test.html
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/variables.html
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/with_data.html
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/templates/yui.html
+-rw-r--r--   0 runner    (1001) docker     (123)    57003 2023-07-29 09:05:56.000000 django-classy-tags-4.1.0/tests/test_core.py
```

### Comparing `django-classy-tags-4.0.0/LICENSE` & `django-classy-tags-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-classy-tags-4.0.0/PKG-INFO` & `django-classy-tags-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: django-classy-tags
-Version: 4.0.0
+Version: 4.1.0
 Summary: Class based template tags for Django
 Home-page: https://github.com/django-cms/django-classy-tags
 Author: Jonas Obrist
 Author-email: ojiidotch@gmail.com
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 ==================
 Django Classy Tags
 ==================
```

### Comparing `django-classy-tags-4.0.0/README.rst` & `django-classy-tags-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-classy-tags-4.0.0/classytags/arguments.py` & `django-classy-tags-4.1.0/classytags/arguments.py`

 * *Files identical despite different names*

### Comparing `django-classy-tags-4.0.0/classytags/blocks.py` & `django-classy-tags-4.1.0/classytags/blocks.py`

 * *Files identical despite different names*

### Comparing `django-classy-tags-4.0.0/classytags/core.py` & `django-classy-tags-4.1.0/classytags/core.py`

 * *Files identical despite different names*

### Comparing `django-classy-tags-4.0.0/classytags/exceptions.py` & `django-classy-tags-4.1.0/classytags/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-classy-tags-4.0.0/classytags/helpers.py` & `django-classy-tags-4.1.0/classytags/helpers.py`

 * *Files identical despite different names*

### Comparing `django-classy-tags-4.0.0/classytags/parser.py` & `django-classy-tags-4.1.0/classytags/parser.py`

 * *Files identical despite different names*

### Comparing `django-classy-tags-4.0.0/classytags/utils.py` & `django-classy-tags-4.1.0/classytags/utils.py`

 * *Files identical despite different names*

### Comparing `django-classy-tags-4.0.0/classytags/values.py` & `django-classy-tags-4.1.0/classytags/values.py`

 * *Files identical despite different names*

### Comparing `django-classy-tags-4.0.0/django_classy_tags.egg-info/PKG-INFO` & `django-classy-tags-4.1.0/django_classy_tags.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: django-classy-tags
-Version: 4.0.0
+Version: 4.1.0
 Summary: Class based template tags for Django
 Home-page: https://github.com/django-cms/django-classy-tags
 Author: Jonas Obrist
 Author-email: ojiidotch@gmail.com
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 ==================
 Django Classy Tags
 ==================
```

### Comparing `django-classy-tags-4.0.0/django_classy_tags.egg-info/SOURCES.txt` & `django-classy-tags-4.1.0/django_classy_tags.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-classy-tags-4.0.0/setup.cfg` & `django-classy-tags-4.1.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 4.0.0
+current_version = 4.1.0
 commit = True
 tag = False
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `django-classy-tags-4.0.0/setup.py` & `django-classy-tags-4.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,44 +12,45 @@
 CLASSIFIERS = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Framework :: Django',
     'Framework :: Django :: 3.2',
     'Framework :: Django :: 4.0',
     'Framework :: Django :: 4.1',
+    'Framework :: Django :: 4.2',
     'Topic :: Internet :: WWW/HTTP',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     'Topic :: Software Development',
     'Topic :: Software Development :: Libraries',
 ]
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 setup(
     name='django-classy-tags',
-    version='4.0.0',
+    version='4.1.0',
     author='Jonas Obrist',
     author_email='ojiidotch@gmail.com',
     maintainer='Django CMS Association and contributors',
     maintainer_email='info@django-cms.org',
     url='https://github.com/django-cms/django-classy-tags',
     license='BSD',
     description='Class based template tags for Django',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     packages=find_packages(exclude=['tests']),
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     include_package_data=True,
     zip_safe=False,
     install_requires=REQUIREMENTS,
     classifiers=CLASSIFIERS,
     test_suite='tests.settings.run',
 )
```

### Comparing `django-classy-tags-4.0.0/tests/context_managers.py` & `django-classy-tags-4.1.0/tests/context_managers.py`

 * *Files identical despite different names*

### Comparing `django-classy-tags-4.0.0/tests/settings.py` & `django-classy-tags-4.1.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-classy-tags-4.0.0/tests/test_core.py` & `django-classy-tags-4.1.0/tests/test_core.py`

 * *Files identical despite different names*

