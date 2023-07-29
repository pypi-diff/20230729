# Comparing `tmp/django-webstack-1.5.0.tar.gz` & `tmp/django-webstack-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-webstack-1.5.0.tar", last modified: Sat Jul 29 07:28:26 2023, max compression
+gzip compressed data, was "django-webstack-1.5.1.tar", last modified: Sat Jul 29 08:04:22 2023, max compression
```

## Comparing `django-webstack-1.5.0.tar` & `django-webstack-1.5.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:28:26.110288 django-webstack-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-29 07:28:13.000000 django-webstack-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-29 07:28:13.000000 django-webstack-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-29 07:28:26.110288 django-webstack-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-29 07:28:13.000000 django-webstack-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:28:26.102288 django-webstack-1.5.0/django_webstack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-29 07:28:26.000000 django-webstack-1.5.0/django_webstack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-29 07:28:26.000000 django-webstack-1.5.0/django_webstack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 07:28:26.000000 django-webstack-1.5.0/django_webstack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-29 07:28:26.000000 django-webstack-1.5.0/django_webstack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 07:28:26.000000 django-webstack-1.5.0/django_webstack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 07:28:26.110288 django-webstack-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-29 07:28:24.000000 django-webstack-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:28:26.106288 django-webstack-1.5.0/webstack/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:28:26.106288 django-webstack-1.5.0/webstack/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/migrations/0002_auto_20230724_1835.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/migrations/0003_auto_20230725_1401.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:28:26.102288 django-webstack-1.5.0/webstack/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:28:26.102288 django-webstack-1.5.0/webstack/static/webstack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:28:26.102288 django-webstack-1.5.0/webstack/static/webstack/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:28:26.106288 django-webstack-1.5.0/webstack/static/webstack/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/static/webstack/assets/css/nav.css
--rw-r--r--   0 runner    (1001) docker     (123)   178177 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/static/webstack/assets/css/xenon-components.css
--rw-r--r--   0 runner    (1001) docker     (123)   213030 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/static/webstack/assets/css/xenon-core.css
--rw-r--r--   0 runner    (1001) docker     (123)    58514 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/static/webstack/assets/css/xenon-forms.css
--rw-r--r--   0 runner    (1001) docker     (123)   288245 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/static/webstack/assets/css/xenon-skins.css
--rw-r--r--   0 runner    (1001) docker     (123)   699452 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/static/webstack/assets/css/xenon.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:28:26.106288 django-webstack-1.5.0/webstack/static/webstack/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/static/webstack/assets/images/favicon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/static/webstack/assets/images/logo-collapsed@2x.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/static/webstack/assets/images/logo@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)  1392068 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/static/webstack/assets/images/preview.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:28:26.110288 django-webstack-1.5.0/webstack/static/webstack/assets/js/
--rwxr-xr-x   0 runner    (1001) docker     (123)    98785 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/static/webstack/assets/js/TweenMax.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/static/webstack/assets/js/joinable.js
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/static/webstack/assets/js/lozad.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     1880 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/static/webstack/assets/js/resizeable.js
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/static/webstack/assets/js/xenon-api.js
--rw-r--r--   0 runner    (1001) docker     (123)    44384 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/static/webstack/assets/js/xenon-custom.js
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/static/webstack/assets/js/xenon-toggles.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:28:26.102288 django-webstack-1.5.0/webstack/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:28:26.110288 django-webstack-1.5.0/webstack/templates/webstack/
--rw-r--r--   0 runner    (1001) docker     (123)     9808 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/templates/webstack/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/templates/webstack/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-29 07:28:13.000000 django-webstack-1.5.0/webstack/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:04:22.748079 django-webstack-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-29 08:04:08.000000 django-webstack-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-29 08:04:08.000000 django-webstack-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-29 08:04:22.748079 django-webstack-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-29 08:04:08.000000 django-webstack-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:04:22.744079 django-webstack-1.5.1/django_webstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-29 08:04:22.000000 django-webstack-1.5.1/django_webstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-29 08:04:22.000000 django-webstack-1.5.1/django_webstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 08:04:22.000000 django-webstack-1.5.1/django_webstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-29 08:04:22.000000 django-webstack-1.5.1/django_webstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 08:04:22.000000 django-webstack-1.5.1/django_webstack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 08:04:22.748079 django-webstack-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-29 08:04:20.000000 django-webstack-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:04:22.744079 django-webstack-1.5.1/webstack/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:04:22.744079 django-webstack-1.5.1/webstack/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/migrations/0002_auto_20230724_1835.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/migrations/0003_auto_20230725_1401.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:04:22.740079 django-webstack-1.5.1/webstack/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:04:22.740079 django-webstack-1.5.1/webstack/static/webstack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:04:22.740079 django-webstack-1.5.1/webstack/static/webstack/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:04:22.744079 django-webstack-1.5.1/webstack/static/webstack/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/static/webstack/assets/css/nav.css
+-rw-r--r--   0 runner    (1001) docker     (123)   178177 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/static/webstack/assets/css/xenon-components.css
+-rw-r--r--   0 runner    (1001) docker     (123)   213030 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/static/webstack/assets/css/xenon-core.css
+-rw-r--r--   0 runner    (1001) docker     (123)    58514 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/static/webstack/assets/css/xenon-forms.css
+-rw-r--r--   0 runner    (1001) docker     (123)   288245 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/static/webstack/assets/css/xenon-skins.css
+-rw-r--r--   0 runner    (1001) docker     (123)   699452 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/static/webstack/assets/css/xenon.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:04:22.744079 django-webstack-1.5.1/webstack/static/webstack/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/static/webstack/assets/images/favicon.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/static/webstack/assets/images/logo-collapsed@2x.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/static/webstack/assets/images/logo@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1392068 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/static/webstack/assets/images/preview.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:04:22.748079 django-webstack-1.5.1/webstack/static/webstack/assets/js/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    98785 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/static/webstack/assets/js/TweenMax.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/static/webstack/assets/js/joinable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/static/webstack/assets/js/lozad.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1880 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/static/webstack/assets/js/resizeable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/static/webstack/assets/js/xenon-api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44384 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/static/webstack/assets/js/xenon-custom.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/static/webstack/assets/js/xenon-toggles.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:04:22.740079 django-webstack-1.5.1/webstack/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:04:22.748079 django-webstack-1.5.1/webstack/templates/webstack/
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/templates/webstack/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/templates/webstack/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-29 08:04:08.000000 django-webstack-1.5.1/webstack/views.py
```

### Comparing `django-webstack-1.5.0/LICENSE` & `django-webstack-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/PKG-INFO` & `django-webstack-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webstack
-Version: 1.5.0
+Version: 1.5.1
 Summary: webstack of Django
 Home-page: https://github.com/Hopetree/django-webstack
 Author: Hopetree
 Author-email: zlwork2014@163.com
 Keywords: django webstack navigation
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-webstack Version: 1.5.0 Summary: webstack of
+Metadata-Version: 2.1 Name: django-webstack Version: 1.5.1 Summary: webstack of
 Django Home-page: https://github.com/Hopetree/django-webstack Author: Hopetree
 Author-email: zlwork2014@163.com Keywords: django webstack navigation
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-webstack-1.5.0/README.md` & `django-webstack-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/django_webstack.egg-info/PKG-INFO` & `django-webstack-1.5.1/django_webstack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webstack
-Version: 1.5.0
+Version: 1.5.1
 Summary: webstack of Django
 Home-page: https://github.com/Hopetree/django-webstack
 Author: Hopetree
 Author-email: zlwork2014@163.com
 Keywords: django webstack navigation
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-webstack Version: 1.5.0 Summary: webstack of
+Metadata-Version: 2.1 Name: django-webstack Version: 1.5.1 Summary: webstack of
 Django Home-page: https://github.com/Hopetree/django-webstack Author: Hopetree
 Author-email: zlwork2014@163.com Keywords: django webstack navigation
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-webstack-1.5.0/django_webstack.egg-info/SOURCES.txt` & `django-webstack-1.5.1/django_webstack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/setup.py` & `django-webstack-1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 # Author: https://github.com/Hopetree
 # Date: 2023/7/24
 from setuptools import find_packages, setup
 
 # 这里的版本号根据tag去动态设置
-VERSION = '1.5.0'
+VERSION = '1.5.1'
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(
     name='django-webstack',
     version=VERSION,
```

### Comparing `django-webstack-1.5.0/webstack/admin.py` & `django-webstack-1.5.1/webstack/admin.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/migrations/0001_initial.py` & `django-webstack-1.5.1/webstack/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/migrations/0002_auto_20230724_1835.py` & `django-webstack-1.5.1/webstack/migrations/0002_auto_20230724_1835.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/migrations/0003_auto_20230725_1401.py` & `django-webstack-1.5.1/webstack/migrations/0003_auto_20230725_1401.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/models.py` & `django-webstack-1.5.1/webstack/models.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/static/webstack/assets/css/nav.css` & `django-webstack-1.5.1/webstack/static/webstack/assets/css/nav.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/static/webstack/assets/css/xenon-components.css` & `django-webstack-1.5.1/webstack/static/webstack/assets/css/xenon-components.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/static/webstack/assets/css/xenon-core.css` & `django-webstack-1.5.1/webstack/static/webstack/assets/css/xenon-core.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/static/webstack/assets/css/xenon-forms.css` & `django-webstack-1.5.1/webstack/static/webstack/assets/css/xenon-forms.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/static/webstack/assets/css/xenon-skins.css` & `django-webstack-1.5.1/webstack/static/webstack/assets/css/xenon-skins.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/static/webstack/assets/css/xenon.css` & `django-webstack-1.5.1/webstack/static/webstack/assets/css/xenon.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/static/webstack/assets/images/favicon.png` & `django-webstack-1.5.1/webstack/static/webstack/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/static/webstack/assets/images/logo-collapsed@2x.png` & `django-webstack-1.5.1/webstack/static/webstack/assets/images/logo-collapsed@2x.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/static/webstack/assets/images/logo@2x.png` & `django-webstack-1.5.1/webstack/static/webstack/assets/images/logo@2x.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/static/webstack/assets/images/preview.gif` & `django-webstack-1.5.1/webstack/static/webstack/assets/images/preview.gif`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/static/webstack/assets/js/TweenMax.min.js` & `django-webstack-1.5.1/webstack/static/webstack/assets/js/TweenMax.min.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/static/webstack/assets/js/joinable.js` & `django-webstack-1.5.1/webstack/static/webstack/assets/js/joinable.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/static/webstack/assets/js/lozad.js` & `django-webstack-1.5.1/webstack/static/webstack/assets/js/lozad.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/static/webstack/assets/js/resizeable.js` & `django-webstack-1.5.1/webstack/static/webstack/assets/js/resizeable.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/static/webstack/assets/js/xenon-api.js` & `django-webstack-1.5.1/webstack/static/webstack/assets/js/xenon-api.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/static/webstack/assets/js/xenon-custom.js` & `django-webstack-1.5.1/webstack/static/webstack/assets/js/xenon-custom.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/static/webstack/assets/js/xenon-toggles.js` & `django-webstack-1.5.1/webstack/static/webstack/assets/js/xenon-toggles.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.0/webstack/templates/webstack/base.html` & `django-webstack-1.5.1/webstack/templates/webstack/base.html`

 * *Files 6% similar despite different names*

```diff
@@ -12,27 +12,46 @@
     <link href="https://cdn.bootcss.com/twitter-bootstrap/3.0.2/css/bootstrap.min.css" rel="stylesheet">
     <link rel="stylesheet" href="{% static 'webstack/assets/css/xenon-core.css' %}">
     <link rel="stylesheet" href="{% static 'webstack/assets/css/xenon-components.css' %}">
     <link rel="stylesheet" href="{% static 'webstack/assets/css/xenon-skins.css' %}">
     <link rel="stylesheet" href="{% static 'webstack/assets/css/nav.css' %}">
     <script src="https://cdn.bootcss.com/jquery/1.11.1/jquery.min.js"></script>
     <style>
+        .sidebar-menu {
+            width: 200px;
+        }
+
+        .sidebar-menu .logo-env {
+            padding: 18px 8px;
+        }
+
+        .sidebar-menu .main-menu {
+            padding-left: 14px;
+            padding-right: 14px;
+        }
+
         .sidebar-menu .main-menu a {
             padding: 14px 4px;
         }
 
         .sidebar-menu .main-menu a > i {
             margin-right: 8px;
             width: 18px;
             max-height: 18px;
         }
 
         .sidebar-menu .main-menu ul li a {
             padding-left: 34px;
         }
+
+        @media screen and (min-width: 768px) {
+            .sidebar-menu.collapsed {
+                width: 66px;
+            }
+        }
     </style>
     {% block top-file %}{% endblock %}
 </head>
 
 <body class="page-body">
 <!-- skin-white -->
 <div class="page-container">
@@ -103,29 +122,29 @@
                 {% if second_menu.get_site_list %}
                     <h4 class="text-gray" id="{{ second_menu.name }}">
                         <i class="{{ second_menu.icon }}" style="margin-right: 7px;"></i>
                         {{ second_menu.name }}
                     </h4>
                     <div class="row">
                         {% for web in second_menu.get_site_list %}
-                            <div class="col-sm-3">
+                            <div class="col-sm-2">
                                 <div class="xe-widget xe-conversations box2 label-info"
                                      onclick="window.open('{{ web.link }}', '_blank')" data-toggle="tooltip"
                                      data-placement="bottom" title="" data-original-title="{{ web.description }}">
                                     <div class="xe-comment-entry">
                                         <a class="xe-user-img">
                                             <img data-src="{{ web.logo.url }}"
                                                  class="lozad img-circle"
                                                  width="40">
                                         </a>
                                         <div class="xe-comment">
                                             <a href="#" class="xe-user-name overflowClip_1">
                                                 <strong>{{ web.name }}</strong>
                                             </a>
-                                            <p class="overflowClip_2">{{ web.description }}</p>
+                                            <p class="overflowClip_2 text-small">{{ web.description }}</p>
                                         </div>
                                     </div>
                                 </div>
                             </div>
 
                         {% endfor %}
                     </div>
```

### Comparing `django-webstack-1.5.0/webstack/templates/webstack/index.html` & `django-webstack-1.5.1/webstack/templates/webstack/index.html`

 * *Files identical despite different names*

