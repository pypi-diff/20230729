# Comparing `tmp/django-statici18n-2.3.1.tar.gz` & `tmp/django-statici18n-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-statici18n-2.3.1.tar", last modified: Sun Aug 14 20:06:55 2022, max compression
+gzip compressed data, was "django-statici18n-2.4.0.tar", last modified: Sat Jul 29 13:10:26 2023, max compression
```

## Comparing `django-statici18n-2.3.1.tar` & `django-statici18n-2.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2022-08-14 20:06:54.998160 django-statici18n-2.3.1/
--rw-r--r--   0 zyegfryed   (501) staff       (20)     2792 2020-09-18 12:18:49.000000 django-statici18n-2.3.1/LICENSE
--rw-r--r--   0 zyegfryed   (501) staff       (20)       88 2020-09-18 12:18:49.000000 django-statici18n-2.3.1/MANIFEST.in
--rw-r--r--   0 zyegfryed   (501) staff       (20)     6083 2022-08-14 20:06:54.998543 django-statici18n-2.3.1/PKG-INFO
--rw-r--r--   0 zyegfryed   (501) staff       (20)     4168 2022-08-14 19:55:45.000000 django-statici18n-2.3.1/README.rst
--rw-r--r--   0 zyegfryed   (501) staff       (20)      358 2022-08-14 20:06:54.999608 django-statici18n-2.3.1/setup.cfg
--rw-r--r--   0 zyegfryed   (501) staff       (20)     1326 2022-08-14 20:00:53.000000 django-statici18n-2.3.1/setup.py
-drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2022-08-14 20:06:54.986898 django-statici18n-2.3.1/src/
-drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2022-08-14 20:06:54.993268 django-statici18n-2.3.1/src/django_statici18n.egg-info/
--rw-r--r--   0 zyegfryed   (501) staff       (20)     6083 2022-08-14 20:06:54.000000 django-statici18n-2.3.1/src/django_statici18n.egg-info/PKG-INFO
--rw-r--r--   0 zyegfryed   (501) staff       (20)      633 2022-08-14 20:06:54.000000 django-statici18n-2.3.1/src/django_statici18n.egg-info/SOURCES.txt
--rw-r--r--   0 zyegfryed   (501) staff       (20)        1 2022-08-14 20:06:54.000000 django-statici18n-2.3.1/src/django_statici18n.egg-info/dependency_links.txt
--rw-r--r--   0 zyegfryed   (501) staff       (20)        1 2020-09-18 12:32:22.000000 django-statici18n-2.3.1/src/django_statici18n.egg-info/not-zip-safe
--rw-r--r--   0 zyegfryed   (501) staff       (20)       32 2022-08-14 20:06:54.000000 django-statici18n-2.3.1/src/django_statici18n.egg-info/requires.txt
--rw-r--r--   0 zyegfryed   (501) staff       (20)       11 2022-08-14 20:06:54.000000 django-statici18n-2.3.1/src/django_statici18n.egg-info/top_level.txt
-drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2022-08-14 20:06:54.995395 django-statici18n-2.3.1/src/statici18n/
--rw-r--r--   0 zyegfryed   (501) staff       (20)      146 2022-08-14 20:00:53.000000 django-statici18n-2.3.1/src/statici18n/__init__.py
--rw-r--r--   0 zyegfryed   (501) staff       (20)      152 2020-10-04 11:35:11.000000 django-statici18n-2.3.1/src/statici18n/apps.py
--rw-r--r--   0 zyegfryed   (501) staff       (20)      697 2020-10-04 11:35:11.000000 django-statici18n-2.3.1/src/statici18n/conf.py
-drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2022-08-14 20:06:54.996000 django-statici18n-2.3.1/src/statici18n/management/
--rw-r--r--   0 zyegfryed   (501) staff       (20)        0 2020-09-18 12:18:49.000000 django-statici18n-2.3.1/src/statici18n/management/__init__.py
-drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2022-08-14 20:06:54.996766 django-statici18n-2.3.1/src/statici18n/management/commands/
--rw-r--r--   0 zyegfryed   (501) staff       (20)        0 2020-09-18 12:18:49.000000 django-statici18n-2.3.1/src/statici18n/management/commands/__init__.py
--rw-r--r--   0 zyegfryed   (501) staff       (20)     5354 2022-08-14 19:57:22.000000 django-statici18n-2.3.1/src/statici18n/management/commands/compilejsi18n.py
-drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2022-08-14 20:06:54.997649 django-statici18n-2.3.1/src/statici18n/templatetags/
--rw-r--r--   0 zyegfryed   (501) staff       (20)        0 2020-09-18 12:18:49.000000 django-statici18n-2.3.1/src/statici18n/templatetags/__init__.py
--rw-r--r--   0 zyegfryed   (501) staff       (20)     1107 2020-10-04 11:35:11.000000 django-statici18n-2.3.1/src/statici18n/templatetags/statici18n.py
--rw-r--r--   0 zyegfryed   (501) staff       (20)     1414 2022-08-14 19:57:22.000000 django-statici18n-2.3.1/src/statici18n/utils.py
+drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2023-07-29 13:10:26.389206 django-statici18n-2.4.0/
+-rw-r--r--   0 zyegfryed   (501) staff       (20)     2792 2020-09-18 12:18:49.000000 django-statici18n-2.4.0/LICENSE
+-rw-r--r--   0 zyegfryed   (501) staff       (20)       88 2020-09-18 12:18:49.000000 django-statici18n-2.4.0/MANIFEST.in
+-rw-r--r--   0 zyegfryed   (501) staff       (20)     6131 2023-07-29 13:10:26.389451 django-statici18n-2.4.0/PKG-INFO
+-rw-r--r--   0 zyegfryed   (501) staff       (20)     4165 2023-07-29 12:41:23.000000 django-statici18n-2.4.0/README.rst
+-rw-r--r--   0 zyegfryed   (501) staff       (20)      358 2023-07-29 13:10:26.390427 django-statici18n-2.4.0/setup.cfg
+-rw-r--r--   0 zyegfryed   (501) staff       (20)     1376 2023-07-29 13:05:41.000000 django-statici18n-2.4.0/setup.py
+drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2023-07-29 13:10:26.375795 django-statici18n-2.4.0/src/
+drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2023-07-29 13:10:26.384480 django-statici18n-2.4.0/src/django_statici18n.egg-info/
+-rw-r--r--   0 zyegfryed   (501) staff       (20)     6131 2023-07-29 13:10:26.000000 django-statici18n-2.4.0/src/django_statici18n.egg-info/PKG-INFO
+-rw-r--r--   0 zyegfryed   (501) staff       (20)      633 2023-07-29 13:10:26.000000 django-statici18n-2.4.0/src/django_statici18n.egg-info/SOURCES.txt
+-rw-r--r--   0 zyegfryed   (501) staff       (20)        1 2023-07-29 13:10:26.000000 django-statici18n-2.4.0/src/django_statici18n.egg-info/dependency_links.txt
+-rw-r--r--   0 zyegfryed   (501) staff       (20)        1 2020-09-18 12:32:22.000000 django-statici18n-2.4.0/src/django_statici18n.egg-info/not-zip-safe
+-rw-r--r--   0 zyegfryed   (501) staff       (20)       32 2023-07-29 13:10:26.000000 django-statici18n-2.4.0/src/django_statici18n.egg-info/requires.txt
+-rw-r--r--   0 zyegfryed   (501) staff       (20)       11 2023-07-29 13:10:26.000000 django-statici18n-2.4.0/src/django_statici18n.egg-info/top_level.txt
+drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2023-07-29 13:10:26.386589 django-statici18n-2.4.0/src/statici18n/
+-rw-r--r--   0 zyegfryed   (501) staff       (20)      146 2023-07-29 13:05:41.000000 django-statici18n-2.4.0/src/statici18n/__init__.py
+-rw-r--r--   0 zyegfryed   (501) staff       (20)      152 2020-10-04 11:35:11.000000 django-statici18n-2.4.0/src/statici18n/apps.py
+-rw-r--r--   0 zyegfryed   (501) staff       (20)      697 2020-10-04 11:35:11.000000 django-statici18n-2.4.0/src/statici18n/conf.py
+drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2023-07-29 13:10:26.387133 django-statici18n-2.4.0/src/statici18n/management/
+-rw-r--r--   0 zyegfryed   (501) staff       (20)        0 2020-09-18 12:18:49.000000 django-statici18n-2.4.0/src/statici18n/management/__init__.py
+drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2023-07-29 13:10:26.387882 django-statici18n-2.4.0/src/statici18n/management/commands/
+-rw-r--r--   0 zyegfryed   (501) staff       (20)        0 2020-09-18 12:18:49.000000 django-statici18n-2.4.0/src/statici18n/management/commands/__init__.py
+-rw-r--r--   0 zyegfryed   (501) staff       (20)     5354 2022-08-14 19:57:22.000000 django-statici18n-2.4.0/src/statici18n/management/commands/compilejsi18n.py
+drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2023-07-29 13:10:26.388683 django-statici18n-2.4.0/src/statici18n/templatetags/
+-rw-r--r--   0 zyegfryed   (501) staff       (20)        0 2020-09-18 12:18:49.000000 django-statici18n-2.4.0/src/statici18n/templatetags/__init__.py
+-rw-r--r--   0 zyegfryed   (501) staff       (20)     1107 2020-10-04 11:35:11.000000 django-statici18n-2.4.0/src/statici18n/templatetags/statici18n.py
+-rw-r--r--   0 zyegfryed   (501) staff       (20)     1414 2022-08-14 19:57:22.000000 django-statici18n-2.4.0/src/statici18n/utils.py
```

### Comparing `django-statici18n-2.3.1/LICENSE` & `django-statici18n-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-statici18n-2.3.1/PKG-INFO` & `django-statici18n-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: django-statici18n
-Version: 2.3.1
+Version: 2.4.0
 Summary: A Django app that compiles i18n JavaScript catalogs to static files.
 Home-page: http://django-statici18n.readthedocs.org/
 Author: Sebastien Fievet
 Author-email: zyegfryed@gmail.com
 License: BSD
 Project-URL: Source, https://github.com/zyegfryed/django-statici18n
 Description: django-statici18n
@@ -44,15 +44,15 @@
         .. _github.com/zyegfryed/django-statici18n: https://github.com/zyegfryed/django-statici18n
         
         Supported Django Versions
         -------------------------
         
         ``django-statici18n`` works with all the Django versions officially
         supported by the Django project. At this time of writing, these are the
-        3.2 (LTS), 4.0 and 4.1 series.
+        3.2 (LTS), 4.1, 4.2 series.
         
         Installation
         ------------
         
         1. Use your favorite Python packaging tool to install ``django-statici18n``
            from `PyPI`_, e.g.::
         
@@ -114,20 +114,20 @@
         
           .. code-block:: html+django
         
             {% load statici18n %}
             <script>{% inlinei18n LANGUAGE_CODE %}</script>
         
         .. _PyPI: http://pypi.python.org/pypi/django-statici18n
-        .. _translated: https://docs.djangoproject.com/en/2.2/topics/i18n/translation/#message-files
-        .. _compiled: https://docs.djangoproject.com/en/2.2/topics/i18n/translation/#compiling-message-files
-        .. _django.core.context_processors.i18n: https://docs.djangoproject.com/en/2.2/ref/templates/api/#django-template-context-processors-i18n
+        .. _translated: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#message-files
+        .. _compiled: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#compiling-message-files
+        .. _django.core.context_processors.i18n: https://docs.djangoproject.com/en/4.2/ref/templates/api/#django-template-context-processors-i18n
         .. _Upgrading templates to Django 1.8: https://docs.djangoproject.com/en/2.2/ref/templates/upgrading/
-        .. _dynamically generated script: https://docs.djangoproject.com/en/2.2/topics/i18n/translation/#using-the-javascript-translation-catalog
-        .. _django.contrib.staticfiles: https://docs.djangoproject.com/en/2.2/ref/contrib/staticfiles/
+        .. _dynamically generated script: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#using-the-javascript-translation-catalog
+        .. _django.contrib.staticfiles: https://docs.djangoproject.com/en/4.2/ref/contrib/staticfiles/
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -135,7 +135,8 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 1.2 Name: django-statici18n Version: 2.3.1 Summary: A Django
+Metadata-Version: 1.2 Name: django-statici18n Version: 2.4.0 Summary: A Django
 app that compiles i18n JavaScript catalogs to static files. Home-page: http://
 django-statici18n.readthedocs.org/ Author: Sebastien Fievet Author-email:
 zyegfryed@gmail.com License: BSD Project-URL: Source, https://github.com/
 zyegfryed/django-statici18n Description: django-statici18n ================= ..
 image:: https://github.com/zyegfryed/django-statici18n/actions/workflows/
 build.yml/badge.svg?branch=main :alt: Build Status :target: https://github.com/
 zyegfryed/django-statici18n/actions .. image:: https://codecov.io/gh/zyegfryed/
@@ -20,15 +20,15 @@
 `github.com/zyegfryed/django-statici18n`_ where you can also file tickets. ..
 _JSONCatalog view: https://docs.djangoproject.com/en/3.2/topics/i18n/
 translation/#the-jsoncatalog-view .. _adding an overhead: https://
 docs.djangoproject.com/en/3.2/topics/i18n/translation/#note-on-performance ..
 _github.com/zyegfryed/django-statici18n: https://github.com/zyegfryed/django-
 statici18n Supported Django Versions ------------------------- ``django-
 statici18n`` works with all the Django versions officially supported by the
-Django project. At this time of writing, these are the 3.2 (LTS), 4.0 and 4.1
+Django project. At this time of writing, these are the 3.2 (LTS), 4.1, 4.2
 series. Installation ------------ 1. Use your favorite Python packaging tool to
 install ``django-statici18n`` from `PyPI`_, e.g.:: pip install django-
 statici18n 2. Add ``'statici18n'`` to your ``INSTALLED_APPS`` setting::
 INSTALLED_APPS = [ # ... 'statici18n', ] 3. Once you have `translated`_ and
 `compiled`_ your messages, use the ``compilejsi18n`` management command::
 python manage.py compilejsi18n 4. Add the
 `django.core.context_processors.i18n`_ context processor to the
@@ -41,25 +41,26 @@
 jsi18n``. You can modify the output path and more options by tweaking ``django-
 statici18n`` settings. **(Optional)** The following step assumes you're using
 `django.contrib.staticfiles`_. 5. Edit your template(s) and use the provided
 template tag: .. code-block:: html+django {% load statici18n %}
  6. Or inline the JavaScript directly in your template: .. code-block::
 html+django {% load statici18n %}
  .. _PyPI: http://pypi.python.org/pypi/django-statici18n .. _translated: https:
-//docs.djangoproject.com/en/2.2/topics/i18n/translation/#message-files ..
-_compiled: https://docs.djangoproject.com/en/2.2/topics/i18n/translation/
+//docs.djangoproject.com/en/4.2/topics/i18n/translation/#message-files ..
+_compiled: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/
 #compiling-message-files .. _django.core.context_processors.i18n: https://
-docs.djangoproject.com/en/2.2/ref/templates/api/#django-template-context-
+docs.djangoproject.com/en/4.2/ref/templates/api/#django-template-context-
 processors-i18n .. _Upgrading templates to Django 1.8: https://
 docs.djangoproject.com/en/2.2/ref/templates/upgrading/ .. _dynamically
-generated script: https://docs.djangoproject.com/en/2.2/topics/i18n/
+generated script: https://docs.djangoproject.com/en/4.2/topics/i18n/
 translation/#using-the-javascript-translation-catalog ..
-_django.contrib.staticfiles: https://docs.djangoproject.com/en/2.2/ref/contrib/
+_django.contrib.staticfiles: https://docs.djangoproject.com/en/4.2/ref/contrib/
 staticfiles/ Platform: UNKNOWN Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11
```

### Comparing `django-statici18n-2.3.1/README.rst` & `django-statici18n-2.4.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 .. _github.com/zyegfryed/django-statici18n: https://github.com/zyegfryed/django-statici18n
 
 Supported Django Versions
 -------------------------
 
 ``django-statici18n`` works with all the Django versions officially
 supported by the Django project. At this time of writing, these are the
-3.2 (LTS), 4.0 and 4.1 series.
+3.2 (LTS), 4.1, 4.2 series.
 
 Installation
 ------------
 
 1. Use your favorite Python packaging tool to install ``django-statici18n``
    from `PyPI`_, e.g.::
 
@@ -105,13 +105,13 @@
 
   .. code-block:: html+django
 
     {% load statici18n %}
     <script>{% inlinei18n LANGUAGE_CODE %}</script>
 
 .. _PyPI: http://pypi.python.org/pypi/django-statici18n
-.. _translated: https://docs.djangoproject.com/en/2.2/topics/i18n/translation/#message-files
-.. _compiled: https://docs.djangoproject.com/en/2.2/topics/i18n/translation/#compiling-message-files
-.. _django.core.context_processors.i18n: https://docs.djangoproject.com/en/2.2/ref/templates/api/#django-template-context-processors-i18n
+.. _translated: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#message-files
+.. _compiled: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#compiling-message-files
+.. _django.core.context_processors.i18n: https://docs.djangoproject.com/en/4.2/ref/templates/api/#django-template-context-processors-i18n
 .. _Upgrading templates to Django 1.8: https://docs.djangoproject.com/en/2.2/ref/templates/upgrading/
-.. _dynamically generated script: https://docs.djangoproject.com/en/2.2/topics/i18n/translation/#using-the-javascript-translation-catalog
-.. _django.contrib.staticfiles: https://docs.djangoproject.com/en/2.2/ref/contrib/staticfiles/
+.. _dynamically generated script: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#using-the-javascript-translation-catalog
+.. _django.contrib.staticfiles: https://docs.djangoproject.com/en/4.2/ref/contrib/staticfiles/
```

#### html2text {}

```diff
@@ -16,19 +16,19 @@
 statici18n`_ where you can also file tickets. .. _JSONCatalog view: https://
 docs.djangoproject.com/en/3.2/topics/i18n/translation/#the-jsoncatalog-view ..
 _adding an overhead: https://docs.djangoproject.com/en/3.2/topics/i18n/
 translation/#note-on-performance .. _github.com/zyegfryed/django-statici18n:
 https://github.com/zyegfryed/django-statici18n Supported Django Versions ------
 ------------------- ``django-statici18n`` works with all the Django versions
 officially supported by the Django project. At this time of writing, these are
-the 3.2 (LTS), 4.0 and 4.1 series. Installation ------------ 1. Use your
-favorite Python packaging tool to install ``django-statici18n`` from `PyPI`_,
-e.g.:: pip install django-statici18n 2. Add ``'statici18n'`` to your
-``INSTALLED_APPS`` setting:: INSTALLED_APPS = [ # ... 'statici18n', ] 3. Once
-you have `translated`_ and `compiled`_ your messages, use the ``compilejsi18n``
+the 3.2 (LTS), 4.1, 4.2 series. Installation ------------ 1. Use your favorite
+Python packaging tool to install ``django-statici18n`` from `PyPI`_, e.g.:: pip
+install django-statici18n 2. Add ``'statici18n'`` to your ``INSTALLED_APPS``
+setting:: INSTALLED_APPS = [ # ... 'statici18n', ] 3. Once you have
+`translated`_ and `compiled`_ your messages, use the ``compilejsi18n``
 management command:: python manage.py compilejsi18n 4. Add the
 `django.core.context_processors.i18n`_ context processor to the
 ``context_processors`` section for your backend in the ``TEMPLATES`` setting -
 it should have already been set by Django:: TEMPLATES = [ { # ... 'OPTIONS':
 { 'context_processors': { # ... 'django.template.context_processors.i18n', },
 }, }, ] 5. Edit your template(s) and replace the `dynamically generated
 script`_ by the statically generated one: .. code-block:: html+django
@@ -36,17 +36,17 @@
 jsi18n``. You can modify the output path and more options by tweaking ``django-
 statici18n`` settings. **(Optional)** The following step assumes you're using
 `django.contrib.staticfiles`_. 5. Edit your template(s) and use the provided
 template tag: .. code-block:: html+django {% load statici18n %}
  6. Or inline the JavaScript directly in your template: .. code-block::
 html+django {% load statici18n %}
  .. _PyPI: http://pypi.python.org/pypi/django-statici18n .. _translated: https:
-//docs.djangoproject.com/en/2.2/topics/i18n/translation/#message-files ..
-_compiled: https://docs.djangoproject.com/en/2.2/topics/i18n/translation/
+//docs.djangoproject.com/en/4.2/topics/i18n/translation/#message-files ..
+_compiled: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/
 #compiling-message-files .. _django.core.context_processors.i18n: https://
-docs.djangoproject.com/en/2.2/ref/templates/api/#django-template-context-
+docs.djangoproject.com/en/4.2/ref/templates/api/#django-template-context-
 processors-i18n .. _Upgrading templates to Django 1.8: https://
 docs.djangoproject.com/en/2.2/ref/templates/upgrading/ .. _dynamically
-generated script: https://docs.djangoproject.com/en/2.2/topics/i18n/
+generated script: https://docs.djangoproject.com/en/4.2/topics/i18n/
 translation/#using-the-javascript-translation-catalog ..
-_django.contrib.staticfiles: https://docs.djangoproject.com/en/2.2/ref/contrib/
+_django.contrib.staticfiles: https://docs.djangoproject.com/en/4.2/ref/contrib/
 staticfiles/
```

### Comparing `django-statici18n-2.3.1/setup.py` & `django-statici18n-2.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name="django-statici18n",
-    version="2.3.1",
+    version="2.4.0",
     author="Sebastien Fievet",
     author_email="zyegfryed@gmail.com",
     url="http://django-statici18n.readthedocs.org/",
     description=("A Django app that compiles i18n JavaScript catalogs "
                  "to static files."),
     long_description=open("README.rst").read(),
     package_dir={"": "src"},
     packages=find_packages("src"),
     include_package_data=True,
     zip_safe=False,
     install_requires=[
-        "Django>=2.2",
+        "Django>=3.2",
         "django-appconf>=1.0",
     ],
     license="BSD",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
@@ -28,12 +28,13 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     project_urls={
         "Source": "https://github.com/zyegfryed/django-statici18n",
     },
 )
```

### Comparing `django-statici18n-2.3.1/src/django_statici18n.egg-info/PKG-INFO` & `django-statici18n-2.4.0/src/django_statici18n.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: django-statici18n
-Version: 2.3.1
+Version: 2.4.0
 Summary: A Django app that compiles i18n JavaScript catalogs to static files.
 Home-page: http://django-statici18n.readthedocs.org/
 Author: Sebastien Fievet
 Author-email: zyegfryed@gmail.com
 License: BSD
 Project-URL: Source, https://github.com/zyegfryed/django-statici18n
 Description: django-statici18n
@@ -44,15 +44,15 @@
         .. _github.com/zyegfryed/django-statici18n: https://github.com/zyegfryed/django-statici18n
         
         Supported Django Versions
         -------------------------
         
         ``django-statici18n`` works with all the Django versions officially
         supported by the Django project. At this time of writing, these are the
-        3.2 (LTS), 4.0 and 4.1 series.
+        3.2 (LTS), 4.1, 4.2 series.
         
         Installation
         ------------
         
         1. Use your favorite Python packaging tool to install ``django-statici18n``
            from `PyPI`_, e.g.::
         
@@ -114,20 +114,20 @@
         
           .. code-block:: html+django
         
             {% load statici18n %}
             <script>{% inlinei18n LANGUAGE_CODE %}</script>
         
         .. _PyPI: http://pypi.python.org/pypi/django-statici18n
-        .. _translated: https://docs.djangoproject.com/en/2.2/topics/i18n/translation/#message-files
-        .. _compiled: https://docs.djangoproject.com/en/2.2/topics/i18n/translation/#compiling-message-files
-        .. _django.core.context_processors.i18n: https://docs.djangoproject.com/en/2.2/ref/templates/api/#django-template-context-processors-i18n
+        .. _translated: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#message-files
+        .. _compiled: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#compiling-message-files
+        .. _django.core.context_processors.i18n: https://docs.djangoproject.com/en/4.2/ref/templates/api/#django-template-context-processors-i18n
         .. _Upgrading templates to Django 1.8: https://docs.djangoproject.com/en/2.2/ref/templates/upgrading/
-        .. _dynamically generated script: https://docs.djangoproject.com/en/2.2/topics/i18n/translation/#using-the-javascript-translation-catalog
-        .. _django.contrib.staticfiles: https://docs.djangoproject.com/en/2.2/ref/contrib/staticfiles/
+        .. _dynamically generated script: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#using-the-javascript-translation-catalog
+        .. _django.contrib.staticfiles: https://docs.djangoproject.com/en/4.2/ref/contrib/staticfiles/
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -135,7 +135,8 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 1.2 Name: django-statici18n Version: 2.3.1 Summary: A Django
+Metadata-Version: 1.2 Name: django-statici18n Version: 2.4.0 Summary: A Django
 app that compiles i18n JavaScript catalogs to static files. Home-page: http://
 django-statici18n.readthedocs.org/ Author: Sebastien Fievet Author-email:
 zyegfryed@gmail.com License: BSD Project-URL: Source, https://github.com/
 zyegfryed/django-statici18n Description: django-statici18n ================= ..
 image:: https://github.com/zyegfryed/django-statici18n/actions/workflows/
 build.yml/badge.svg?branch=main :alt: Build Status :target: https://github.com/
 zyegfryed/django-statici18n/actions .. image:: https://codecov.io/gh/zyegfryed/
@@ -20,15 +20,15 @@
 `github.com/zyegfryed/django-statici18n`_ where you can also file tickets. ..
 _JSONCatalog view: https://docs.djangoproject.com/en/3.2/topics/i18n/
 translation/#the-jsoncatalog-view .. _adding an overhead: https://
 docs.djangoproject.com/en/3.2/topics/i18n/translation/#note-on-performance ..
 _github.com/zyegfryed/django-statici18n: https://github.com/zyegfryed/django-
 statici18n Supported Django Versions ------------------------- ``django-
 statici18n`` works with all the Django versions officially supported by the
-Django project. At this time of writing, these are the 3.2 (LTS), 4.0 and 4.1
+Django project. At this time of writing, these are the 3.2 (LTS), 4.1, 4.2
 series. Installation ------------ 1. Use your favorite Python packaging tool to
 install ``django-statici18n`` from `PyPI`_, e.g.:: pip install django-
 statici18n 2. Add ``'statici18n'`` to your ``INSTALLED_APPS`` setting::
 INSTALLED_APPS = [ # ... 'statici18n', ] 3. Once you have `translated`_ and
 `compiled`_ your messages, use the ``compilejsi18n`` management command::
 python manage.py compilejsi18n 4. Add the
 `django.core.context_processors.i18n`_ context processor to the
@@ -41,25 +41,26 @@
 jsi18n``. You can modify the output path and more options by tweaking ``django-
 statici18n`` settings. **(Optional)** The following step assumes you're using
 `django.contrib.staticfiles`_. 5. Edit your template(s) and use the provided
 template tag: .. code-block:: html+django {% load statici18n %}
  6. Or inline the JavaScript directly in your template: .. code-block::
 html+django {% load statici18n %}
  .. _PyPI: http://pypi.python.org/pypi/django-statici18n .. _translated: https:
-//docs.djangoproject.com/en/2.2/topics/i18n/translation/#message-files ..
-_compiled: https://docs.djangoproject.com/en/2.2/topics/i18n/translation/
+//docs.djangoproject.com/en/4.2/topics/i18n/translation/#message-files ..
+_compiled: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/
 #compiling-message-files .. _django.core.context_processors.i18n: https://
-docs.djangoproject.com/en/2.2/ref/templates/api/#django-template-context-
+docs.djangoproject.com/en/4.2/ref/templates/api/#django-template-context-
 processors-i18n .. _Upgrading templates to Django 1.8: https://
 docs.djangoproject.com/en/2.2/ref/templates/upgrading/ .. _dynamically
-generated script: https://docs.djangoproject.com/en/2.2/topics/i18n/
+generated script: https://docs.djangoproject.com/en/4.2/topics/i18n/
 translation/#using-the-javascript-translation-catalog ..
-_django.contrib.staticfiles: https://docs.djangoproject.com/en/2.2/ref/contrib/
+_django.contrib.staticfiles: https://docs.djangoproject.com/en/4.2/ref/contrib/
 staticfiles/ Platform: UNKNOWN Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11
```

### Comparing `django-statici18n-2.3.1/src/django_statici18n.egg-info/SOURCES.txt` & `django-statici18n-2.4.0/src/django_statici18n.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-statici18n-2.3.1/src/statici18n/conf.py` & `django-statici18n-2.4.0/src/statici18n/conf.py`

 * *Files identical despite different names*

### Comparing `django-statici18n-2.3.1/src/statici18n/management/commands/compilejsi18n.py` & `django-statici18n-2.4.0/src/statici18n/management/commands/compilejsi18n.py`

 * *Files identical despite different names*

### Comparing `django-statici18n-2.3.1/src/statici18n/templatetags/statici18n.py` & `django-statici18n-2.4.0/src/statici18n/templatetags/statici18n.py`

 * *Files identical despite different names*

### Comparing `django-statici18n-2.3.1/src/statici18n/utils.py` & `django-statici18n-2.4.0/src/statici18n/utils.py`

 * *Files identical despite different names*

