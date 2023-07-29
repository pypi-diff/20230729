# Comparing `tmp/django-errors-1.6.8.tar.gz` & `tmp/django-errors-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-errors-1.6.8.tar", last modified: Fri Jul 28 19:13:56 2023, max compression
+gzip compressed data, was "django-errors-2.1.0.tar", last modified: Sat Jul 29 14:14:17 2023, max compression
```

## Comparing `django-errors-1.6.8.tar` & `django-errors-2.1.0.tar`

### file list

```diff
@@ -1,81 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.610786 django-errors-1.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-28 19:13:44.000000 django-errors-1.6.8/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-28 19:13:44.000000 django-errors-1.6.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 19:13:44.000000 django-errors-1.6.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-28 19:13:44.000000 django-errors-1.6.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-28 19:13:44.000000 django-errors-1.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 19:13:44.000000 django-errors-1.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-28 19:13:56.610786 django-errors-1.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-28 19:13:44.000000 django-errors-1.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-28 19:13:44.000000 django-errors-1.6.8/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-28 19:13:44.000000 django-errors-1.6.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.606786 django-errors-1.6.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-28 19:13:44.000000 django-errors-1.6.8/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)    29701 2023-07-28 19:13:44.000000 django-errors-1.6.8/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-28 19:13:44.000000 django-errors-1.6.8/requirements/py310-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-07-28 19:13:44.000000 django-errors-1.6.8/requirements/py310-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-28 19:13:44.000000 django-errors-1.6.8/requirements/py311-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-28 19:13:44.000000 django-errors-1.6.8/requirements/py311-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-28 19:13:44.000000 django-errors-1.6.8/requirements/py38-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-28 19:13:44.000000 django-errors-1.6.8/requirements/py38-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-28 19:13:44.000000 django-errors-1.6.8/requirements/py39-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-07-28 19:13:44.000000 django-errors-1.6.8/requirements/py39-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 19:13:44.000000 django-errors-1.6.8/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-28 19:13:44.000000 django-errors-1.6.8/runtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-28 19:13:56.610786 django-errors-1.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-28 19:13:44.000000 django-errors-1.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.598785 django-errors-1.6.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.606786 django-errors-1.6.8/src/django_errors/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-28 19:13:44.000000 django-errors-1.6.8/src/django_errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-28 19:13:44.000000 django-errors-1.6.8/src/django_errors/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.602785 django-errors-1.6.8/src/django_errors/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.598785 django-errors-1.6.8/src/django_errors/locale/cn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.606786 django-errors-1.6.8/src/django_errors/locale/cn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-28 19:13:44.000000 django-errors-1.6.8/src/django_errors/locale/cn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.598785 django-errors-1.6.8/src/django_errors/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.606786 django-errors-1.6.8/src/django_errors/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-28 19:13:44.000000 django-errors-1.6.8/src/django_errors/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.602785 django-errors-1.6.8/src/django_errors/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.606786 django-errors-1.6.8/src/django_errors/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-28 19:13:44.000000 django-errors-1.6.8/src/django_errors/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.602785 django-errors-1.6.8/src/django_errors/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.606786 django-errors-1.6.8/src/django_errors/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-28 19:13:44.000000 django-errors-1.6.8/src/django_errors/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.602785 django-errors-1.6.8/src/django_errors/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.606786 django-errors-1.6.8/src/django_errors/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-28 19:13:44.000000 django-errors-1.6.8/src/django_errors/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.602785 django-errors-1.6.8/src/django_errors/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.606786 django-errors-1.6.8/src/django_errors/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-28 19:13:44.000000 django-errors-1.6.8/src/django_errors/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.602785 django-errors-1.6.8/src/django_errors/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.606786 django-errors-1.6.8/src/django_errors/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-28 19:13:44.000000 django-errors-1.6.8/src/django_errors/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.602785 django-errors-1.6.8/src/django_errors/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.606786 django-errors-1.6.8/src/django_errors/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-28 19:13:44.000000 django-errors-1.6.8/src/django_errors/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.606786 django-errors-1.6.8/src/django_errors/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:44.000000 django-errors-1.6.8/src/django_errors/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-28 19:13:44.000000 django-errors-1.6.8/src/django_errors/middleware/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.602785 django-errors-1.6.8/src/django_errors/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.610786 django-errors-1.6.8/src/django_errors/templates/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-28 19:13:44.000000 django-errors-1.6.8/src/django_errors/templates/errors/400.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-28 19:13:44.000000 django-errors-1.6.8/src/django_errors/templates/errors/403.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-28 19:13:44.000000 django-errors-1.6.8/src/django_errors/templates/errors/404.html
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-28 19:13:44.000000 django-errors-1.6.8/src/django_errors/templates/errors/405.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-28 19:13:44.000000 django-errors-1.6.8/src/django_errors/templates/errors/500.html
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-28 19:13:44.000000 django-errors-1.6.8/src/django_errors/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-28 19:13:44.000000 django-errors-1.6.8/src/django_errors/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.606786 django-errors-1.6.8/src/django_errors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-28 19:13:56.000000 django-errors-1.6.8/src/django_errors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-28 19:13:56.000000 django-errors-1.6.8/src/django_errors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:13:56.000000 django-errors-1.6.8/src/django_errors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:13:56.000000 django-errors-1.6.8/src/django_errors.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 19:13:56.000000 django-errors-1.6.8/src/django_errors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 19:13:56.000000 django-errors-1.6.8/src/django_errors.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:56.610786 django-errors-1.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:13:44.000000 django-errors-1.6.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-28 19:13:44.000000 django-errors-1.6.8/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-28 19:13:44.000000 django-errors-1.6.8/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-28 19:13:44.000000 django-errors-1.6.8/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 19:13:44.000000 django-errors-1.6.8/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-28 19:13:44.000000 django-errors-1.6.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.220628 django-errors-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-29 14:14:04.000000 django-errors-2.1.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-29 14:14:04.000000 django-errors-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-29 14:14:04.000000 django-errors-2.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-29 14:14:04.000000 django-errors-2.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-29 14:14:04.000000 django-errors-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-29 14:14:04.000000 django-errors-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-29 14:14:17.220628 django-errors-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-29 14:14:04.000000 django-errors-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-29 14:14:04.000000 django-errors-2.1.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-29 14:14:04.000000 django-errors-2.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)    29701 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/py310-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/py310-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/py311-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/py311-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/py38-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/py38-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/py39-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/py39-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-29 14:14:04.000000 django-errors-2.1.0/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-29 14:14:17.220628 django-errors-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-29 14:14:04.000000 django-errors-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.208628 django-errors-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/src/django_errors/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.208628 django-errors-2.1.0/src/django_errors/locale/cn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/cn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/cn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.208628 django-errors-2.1.0/src/django_errors/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.208628 django-errors-2.1.0/src/django_errors/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.208628 django-errors-2.1.0/src/django_errors/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/src/django_errors/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/src/django_errors/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/src/django_errors/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/src/django_errors/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/src/django_errors/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/src/django_errors/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/src/django_errors/locale/zh_hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/zh_hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/zh_hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/src/django_errors/locale/zh_hant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/zh_hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/zh_hant/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/middleware/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/templates/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/templates/errors/400.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/templates/errors/403.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/templates/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/templates/errors/405.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/templates/errors/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-29 14:14:17.000000 django-errors-2.1.0/src/django_errors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-29 14:14:17.000000 django-errors-2.1.0/src/django_errors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 14:14:17.000000 django-errors-2.1.0/src/django_errors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 14:14:17.000000 django-errors-2.1.0/src/django_errors.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-29 14:14:17.000000 django-errors-2.1.0/src/django_errors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 14:14:17.000000 django-errors-2.1.0/src/django_errors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.220628 django-errors-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/test_errors_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/test_errors_locale_it.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/test_errors_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/test_errors_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/test_errors_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/views_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/views_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/views_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-29 14:14:04.000000 django-errors-2.1.0/tox.ini
```

### Comparing `django-errors-1.6.8/.pre-commit-config.yaml` & `django-errors-2.1.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     exclude: .bumpversion.cfg
 - repo: https://github.com/asottile/pyupgrade
   rev: v3.9.0
   hooks:
   - id: pyupgrade
     args: [--py36-plus]
 - repo: https://github.com/psf/black
-  rev: 23.3.0
+  rev: 23.7.0
   hooks:
   - id: black
 - repo: https://github.com/asottile/blacken-docs
   rev: 1.15.0
   hooks:
   - id: blacken-docs
     additional_dependencies:
```

### Comparing `django-errors-1.6.8/LICENSE` & `django-errors-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.8/PKG-INFO` & `django-errors-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-errors
-Version: 1.6.8
+Version: 2.1.0
 Summary: Django application for handling server errors.
 Home-page: https://github.com/DLRSP/django-errors
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,errors
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-errors-1.6.8/README.md` & `django-errors-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.8/mkdocs.yml` & `django-errors-2.1.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.8/pyproject.toml` & `django-errors-2.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 django_find_project = false
 
 [tool.towncrier]
 package = "django_errors"
 package_dir = "src"
 filename = "CHANGELOG.rst"
 directory = "news/"
-version = "1.6.8"
+version = "2.1.0"
 
 # For rendering properly for this project
 issue_format = "`#{issue} <https://github.com/DLRSP/django-errors/issues/{issue}>`_"
 # template = "tools/news/template.rst"
 
 # Grouping of entries, within our changelog
 type = [
```

### Comparing `django-errors-1.6.8/requirements/docs.txt` & `django-errors-2.1.0/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.8/requirements/py310-django32.txt` & `django-errors-2.1.0/requirements/py310-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.8/requirements/py310-django42.txt` & `django-errors-2.1.0/requirements/py310-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.8/requirements/py311-django32.txt` & `django-errors-2.1.0/requirements/py311-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.8/requirements/py311-django42.txt` & `django-errors-2.1.0/requirements/py311-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.8/requirements/py38-django32.txt` & `django-errors-2.1.0/requirements/py38-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.8/requirements/py38-django42.txt` & `django-errors-2.1.0/requirements/py38-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.8/requirements/py39-django32.txt` & `django-errors-2.1.0/requirements/py39-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.8/requirements/py39-django42.txt` & `django-errors-2.1.0/requirements/py39-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.8/runtests.py` & `django-errors-2.1.0/runtests.py`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.8/setup.cfg` & `django-errors-2.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = django-errors
-version = 1.6.8
+version = 2.1.0
 url = https://github.com/DLRSP/django-errors
 author = DLRSP
 author_email = dlrsp.dev@gmail.com
 description = Django application for handling server errors.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `django-errors-1.6.8/setup.py` & `django-errors-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.8/src/django_errors/__init__.py` & `django-errors-2.1.0/src/django_errors/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 4. push to pypi + push to github
 5. bump the version, append '.dev0'
 6. git commit
 7. push to github (to avoid confusion)
 """
 import django
 
-__version__ = "1.6.8"
+__version__ = "2.1.0"
 __version_info__ = tuple(int(i) if i.isdigit() else i for i in __version__.split("."))
 __license__ = "MIT"
 __title__ = "django_errors"
 
 __author__ = "DLRSP"
 __copyright__ = "Copyright 2010-present DLRSP"
```

### Comparing `django-errors-1.6.8/src/django_errors/locale/cn/LC_MESSAGES/django.po` & `django-errors-2.1.0/src/django_errors/locale/cn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.8/src/django_errors/locale/de/LC_MESSAGES/django.po` & `django-errors-2.1.0/src/django_errors/locale/en/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-15 19:03+0100\n"
+"POT-Creation-Date: 2021-11-15 19:04+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: .\src\django_errors\middleware\handler.py:15
 msgid "Method Not Allowed"
 msgstr ""
 
 #: .\src\django_errors\middleware\handler.py:17
 msgid "Sorry, the used method is not allowed for the page with that URL."
```

### Comparing `django-errors-1.6.8/src/django_errors/locale/en/LC_MESSAGES/django.po` & `django-errors-2.1.0/src/django_errors/locale/lt/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,56 +4,58 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-15 19:04+0100\n"
+"POT-Creation-Date: 2021-11-15 18:38+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && (n"
+"%100<10 || n%100>=20) ? 1 : 2);\n"
 
 #: .\src\django_errors\middleware\handler.py:15
 msgid "Method Not Allowed"
 msgstr ""
 
-#: .\src\django_errors\middleware\handler.py:17
+#: .\src\django_errors\middleware\handler.py:16
 msgid "Sorry, the used method is not allowed for the page with that URL."
 msgstr ""
 
 #: .\src\django_errors\views.py:16
 msgid "Bad Request"
 msgstr ""
 
-#: .\src\django_errors\views.py:18
+#: .\src\django_errors\views.py:17
 msgid ""
 "The request could not be understood by the server due to malformed syntax."
 msgstr ""
 
-#: .\src\django_errors\views.py:28
+#: .\src\django_errors\views.py:26
 msgid "Permission Denied"
 msgstr ""
 
-#: .\src\django_errors\views.py:29
+#: .\src\django_errors\views.py:27
 msgid "You don't have permissions to see this page!"
 msgstr ""
 
-#: .\src\django_errors\views.py:38
+#: .\src\django_errors\views.py:36
 msgid "Page Not Found"
 msgstr ""
 
-#: .\src\django_errors\views.py:39
+#: .\src\django_errors\views.py:37
 msgid "Sorry, we don't have a page with that URL."
 msgstr ""
 
-#: .\src\django_errors\views.py:48
+#: .\src\django_errors\views.py:46
 msgid "Internal Server Error"
 msgstr ""
 
-#: .\src\django_errors\views.py:49
+#: .\src\django_errors\views.py:47
 msgid "Sorry, an error has occurred with the application."
 msgstr ""
```

### Comparing `django-errors-1.6.8/src/django_errors/locale/es/LC_MESSAGES/django.po` & `django-errors-2.1.0/src/django_errors/locale/fr/LC_MESSAGES/django.po`

 * *Files 16% similar despite different names*

```diff
@@ -4,57 +4,57 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-15 19:04+0100\n"
+"POT-Creation-Date: 2023-07-29 15:24+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: .\src\django_errors\middleware\handler.py:15
+#: .\middleware\handler.py:16 .\views.py:87
 msgid "Method Not Allowed"
 msgstr ""
 
-#: .\src\django_errors\middleware\handler.py:17
+#: .\middleware\handler.py:18 .\views.py:88
 msgid "Sorry, the used method is not allowed for the page with that URL."
 msgstr ""
 
-#: .\src\django_errors\views.py:16
+#: .\views.py:18
 msgid "Bad Request"
 msgstr ""
 
-#: .\src\django_errors\views.py:18
+#: .\views.py:20
 msgid ""
 "The request could not be understood by the server due to malformed syntax."
 msgstr ""
 
-#: .\src\django_errors\views.py:28
+#: .\views.py:42
 msgid "Permission Denied"
 msgstr ""
 
-#: .\src\django_errors\views.py:29
+#: .\views.py:43
 msgid "You don't have permissions to see this page!"
 msgstr ""
 
-#: .\src\django_errors\views.py:38
+#: .\views.py:64
 msgid "Page Not Found"
 msgstr ""
 
-#: .\src\django_errors\views.py:39
+#: .\views.py:65
 msgid "Sorry, we don't have a page with that URL."
 msgstr ""
 
-#: .\src\django_errors\views.py:48
+#: .\views.py:109
 msgid "Internal Server Error"
 msgstr ""
 
-#: .\src\django_errors\views.py:49
+#: .\views.py:110
 msgid "Sorry, an error has occurred with the application."
 msgstr ""
```

### Comparing `django-errors-1.6.8/src/django_errors/locale/fr/LC_MESSAGES/django.po` & `django-errors-2.1.0/src/django_errors/locale/de/LC_MESSAGES/django.po`

 * *Files 16% similar despite different names*

```diff
@@ -4,57 +4,57 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-15 19:04+0100\n"
+"POT-Creation-Date: 2023-07-29 15:24+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: .\src\django_errors\middleware\handler.py:15
+#: .\middleware\handler.py:16 .\views.py:87
 msgid "Method Not Allowed"
 msgstr ""
 
-#: .\src\django_errors\middleware\handler.py:17
+#: .\middleware\handler.py:18 .\views.py:88
 msgid "Sorry, the used method is not allowed for the page with that URL."
 msgstr ""
 
-#: .\src\django_errors\views.py:16
+#: .\views.py:18
 msgid "Bad Request"
 msgstr ""
 
-#: .\src\django_errors\views.py:18
+#: .\views.py:20
 msgid ""
 "The request could not be understood by the server due to malformed syntax."
 msgstr ""
 
-#: .\src\django_errors\views.py:28
+#: .\views.py:42
 msgid "Permission Denied"
 msgstr ""
 
-#: .\src\django_errors\views.py:29
+#: .\views.py:43
 msgid "You don't have permissions to see this page!"
 msgstr ""
 
-#: .\src\django_errors\views.py:38
+#: .\views.py:64
 msgid "Page Not Found"
 msgstr ""
 
-#: .\src\django_errors\views.py:39
+#: .\views.py:65
 msgid "Sorry, we don't have a page with that URL."
 msgstr ""
 
-#: .\src\django_errors\views.py:48
+#: .\views.py:109
 msgid "Internal Server Error"
 msgstr ""
 
-#: .\src\django_errors\views.py:49
+#: .\views.py:110
 msgid "Sorry, an error has occurred with the application."
 msgstr ""
```

### Comparing `django-errors-1.6.8/src/django_errors/locale/it/LC_MESSAGES/django.po` & `django-errors-2.1.0/src/django_errors/locale/ja/LC_MESSAGES/django.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,60 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
+#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: \n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-15 19:02+0100\n"
-"PO-Revision-Date: 2016-01-04 16:15+0100\n"
-"Last-Translator: \n"
-"Language-Team: \n"
-"Language: it\n"
+"POT-Creation-Date: 2023-07-29 15:24+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 1.8.6\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: .\src\django_errors\middleware\handler.py:15
+#: .\middleware\handler.py:16 .\views.py:87
 msgid "Method Not Allowed"
-msgstr "Metodo non consentito"
+msgstr ""
 
-#: .\src\django_errors\middleware\handler.py:17
+#: .\middleware\handler.py:18 .\views.py:88
 msgid "Sorry, the used method is not allowed for the page with that URL."
-msgstr "Scusa, il metodo usato non è consentito per la pagina con questo URL."
+msgstr ""
 
-#: .\src\django_errors\views.py:16
+#: .\views.py:18
 msgid "Bad Request"
-msgstr "Brutta Richiesta"
+msgstr ""
 
-#: .\src\django_errors\views.py:18
+#: .\views.py:20
 msgid ""
 "The request could not be understood by the server due to malformed syntax."
 msgstr ""
-"La richiesta non può essere compresa dal server a causa di sintassi errata."
 
-#: .\src\django_errors\views.py:28
+#: .\views.py:42
 msgid "Permission Denied"
-msgstr "Permesso Negato"
+msgstr ""
 
-#: .\src\django_errors\views.py:29
+#: .\views.py:43
 msgid "You don't have permissions to see this page!"
-msgstr "Non hai il permesso per vedere questa pagina!"
+msgstr ""
 
-#: .\src\django_errors\views.py:38
+#: .\views.py:64
 msgid "Page Not Found"
-msgstr "Pagina non trovata"
+msgstr ""
 
-#: .\src\django_errors\views.py:39
+#: .\views.py:65
 msgid "Sorry, we don't have a page with that URL."
-msgstr "Scusa, non abbiamo una pagina con questo URL."
+msgstr ""
 
-#: .\src\django_errors\views.py:48
+#: .\views.py:109
 msgid "Internal Server Error"
-msgstr "Errore Interno del Server"
+msgstr ""
 
-#: .\src\django_errors\views.py:49
+#: .\views.py:110
 msgid "Sorry, an error has occurred with the application."
-msgstr "Scusa, si è verificato un errore con il programma."
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-errors-1.6.8/src/django_errors/locale/lt/LC_MESSAGES/django.po` & `django-errors-2.1.0/src/django_errors/locale/nl/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -4,58 +4,57 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-15 18:38+0100\n"
+"POT-Creation-Date: 2023-07-29 15:25+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && (n"
-"%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: .\src\django_errors\middleware\handler.py:15
+#: .\middleware\handler.py:16 .\views.py:87
 msgid "Method Not Allowed"
 msgstr ""
 
-#: .\src\django_errors\middleware\handler.py:16
+#: .\middleware\handler.py:18 .\views.py:88
 msgid "Sorry, the used method is not allowed for the page with that URL."
 msgstr ""
 
-#: .\src\django_errors\views.py:16
+#: .\views.py:18
 msgid "Bad Request"
 msgstr ""
 
-#: .\src\django_errors\views.py:17
+#: .\views.py:20
 msgid ""
 "The request could not be understood by the server due to malformed syntax."
 msgstr ""
 
-#: .\src\django_errors\views.py:26
+#: .\views.py:42
 msgid "Permission Denied"
 msgstr ""
 
-#: .\src\django_errors\views.py:27
+#: .\views.py:43
 msgid "You don't have permissions to see this page!"
 msgstr ""
 
-#: .\src\django_errors\views.py:36
+#: .\views.py:64
 msgid "Page Not Found"
 msgstr ""
 
-#: .\src\django_errors\views.py:37
+#: .\views.py:65
 msgid "Sorry, we don't have a page with that URL."
 msgstr ""
 
-#: .\src\django_errors\views.py:46
+#: .\views.py:109
 msgid "Internal Server Error"
 msgstr ""
 
-#: .\src\django_errors\views.py:47
+#: .\views.py:110
 msgid "Sorry, an error has occurred with the application."
 msgstr ""
```

### Comparing `django-errors-1.6.8/src/django_errors/locale/ru/LC_MESSAGES/django.po` & `django-errors-2.1.0/src/django_errors/locale/es/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -4,58 +4,57 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-15 18:38+0100\n"
+"POT-Creation-Date: 2023-07-29 15:24+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: .\src\django_errors\middleware\handler.py:15
+#: .\middleware\handler.py:16 .\views.py:87
 msgid "Method Not Allowed"
 msgstr ""
 
-#: .\src\django_errors\middleware\handler.py:16
+#: .\middleware\handler.py:18 .\views.py:88
 msgid "Sorry, the used method is not allowed for the page with that URL."
 msgstr ""
 
-#: .\src\django_errors\views.py:16
+#: .\views.py:18
 msgid "Bad Request"
 msgstr ""
 
-#: .\src\django_errors\views.py:17
+#: .\views.py:20
 msgid ""
 "The request could not be understood by the server due to malformed syntax."
 msgstr ""
 
-#: .\src\django_errors\views.py:26
+#: .\views.py:42
 msgid "Permission Denied"
 msgstr ""
 
-#: .\src\django_errors\views.py:27
+#: .\views.py:43
 msgid "You don't have permissions to see this page!"
 msgstr ""
 
-#: .\src\django_errors\views.py:36
+#: .\views.py:64
 msgid "Page Not Found"
 msgstr ""
 
-#: .\src\django_errors\views.py:37
+#: .\views.py:65
 msgid "Sorry, we don't have a page with that URL."
 msgstr ""
 
-#: .\src\django_errors\views.py:46
+#: .\views.py:109
 msgid "Internal Server Error"
 msgstr ""
 
-#: .\src\django_errors\views.py:47
+#: .\views.py:110
 msgid "Sorry, an error has occurred with the application."
 msgstr ""
```

### Comparing `django-errors-1.6.8/src/django_errors/middleware/handler.py` & `django-errors-2.1.0/src/django_errors/middleware/handler.py`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.8/src/django_errors/views.py` & `django-errors-2.1.0/src/django_errors/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Django Views for django-errors module"""
 from django.conf import settings
 from django.http import (
     HttpResponseBadRequest,
     HttpResponseForbidden,
+    HttpResponseNotAllowed,
     HttpResponseNotFound,
     HttpResponseServerError,
 )
 from django.template import loader
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.views.decorators.http import require_http_methods
 
 
 @require_http_methods(["GET"])
 def custom_400(request, exception=None):
     """Custom Page for 400 error (Bad Request). url: /400"""
     error = _("Bad Request")
@@ -75,14 +76,37 @@
         "error_message": error_msg,
         "error_request_method": request.method,
         "exception": exception,
     }
     return HttpResponseNotFound(template.render(context, request))
 
 
+def custom_405(request, permitted_methods=None, exception=None):
+    """Custom Page for 405 error (Method Not Allowed). url: /405"""
+    if permitted_methods is None:
+        permitted_methods = ["GET", "POST"]
+    error = _("Method Not Allowed")
+    error_msg = _("Sorry, the used method is not allowed for the page with that URL.")
+    template = loader.get_template(
+        getattr(
+            settings,
+            "TEMPLATE_ERROR_405",
+            getattr(settings, "TEMPLATE_ERROR_ALL", "errors/405.html"),
+        )
+    )
+    context = {
+        "error": error,
+        "error_code": 405,
+        "error_message": error_msg,
+        "error_request_method": request.method,
+        "exception": exception,
+    }
+    return HttpResponseNotAllowed(permitted_methods, template.render(context, request))
+
+
 @require_http_methods(["GET"])
 def custom_500(request, exception=None):
     """Custom Page for 500 error (Internal Server Error). url: /500"""
     error = _("Internal Server Error")
     error_msg = _("Sorry, an error has occurred with the application.")
     template = loader.get_template(
         getattr(
```

### Comparing `django-errors-1.6.8/src/django_errors.egg-info/PKG-INFO` & `django-errors-2.1.0/src/django_errors.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-errors
-Version: 1.6.8
+Version: 2.1.0
 Summary: Django application for handling server errors.
 Home-page: https://github.com/DLRSP/django-errors
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,errors
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-errors-1.6.8/src/django_errors.egg-info/SOURCES.txt` & `django-errors-2.1.0/src/django_errors.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -34,21 +34,34 @@
 src/django_errors.egg-info/top_level.txt
 src/django_errors/locale/cn/LC_MESSAGES/django.po
 src/django_errors/locale/de/LC_MESSAGES/django.po
 src/django_errors/locale/en/LC_MESSAGES/django.po
 src/django_errors/locale/es/LC_MESSAGES/django.po
 src/django_errors/locale/fr/LC_MESSAGES/django.po
 src/django_errors/locale/it/LC_MESSAGES/django.po
+src/django_errors/locale/ja/LC_MESSAGES/django.po
 src/django_errors/locale/lt/LC_MESSAGES/django.po
+src/django_errors/locale/nl/LC_MESSAGES/django.po
 src/django_errors/locale/ru/LC_MESSAGES/django.po
+src/django_errors/locale/zh_hans/LC_MESSAGES/django.po
+src/django_errors/locale/zh_hant/LC_MESSAGES/django.po
 src/django_errors/middleware/__init__.py
 src/django_errors/middleware/handler.py
+src/django_errors/templates/base.html
 src/django_errors/templates/errors/400.html
 src/django_errors/templates/errors/403.html
 src/django_errors/templates/errors/404.html
 src/django_errors/templates/errors/405.html
 src/django_errors/templates/errors/500.html
 tests/__init__.py
 tests/settings.py
 tests/test_errors.py
+tests/test_errors_exceptions.py
+tests/test_errors_locale_it.py
+tests/test_errors_standard.py
+tests/test_errors_templates.py
+tests/test_errors_urls.py
 tests/urls.py
-tests/views.py
+tests/views.py
+tests/views_exceptions.py
+tests/views_standard.py
+tests/views_templates.py
```

### Comparing `django-errors-1.6.8/tests/test_errors.py` & `django-errors-2.1.0/tests/test_errors_urls.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,51 +16,46 @@
     def tearDown(self):
         """Remove Test Data"""
         LOGGER.debug("Tests tearDown")
 
     def test_400_urls(self):
         """Test the url of 400 page."""
         LOGGER.debug("400 Test Redirect URLs")
-        response = self.client.get("/test-400/", follow=True)
+        response = self.client.get("/400/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(400, response.status_code)
 
     def test_403_urls(self):
         """Test the url of 403 page."""
         LOGGER.debug("403 Test Redirect URLs")
-        response = self.client.get("/test-403/", follow=True)
+        response = self.client.get("/403/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(403, response.status_code)
 
     def test_404_urls(self):
         """Test the url of 404 page."""
         LOGGER.debug("404 Test URLs")
-        response = self.client.get("/test-404/", follow=True)
+        response = self.client.get("/404/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(404, response.status_code)
 
     def test_405_urls(self):
         """Test the url of 404 page."""
         LOGGER.debug("405 Test GET URLs with only POST")
-        response = self.client.get("/test-405/", follow=True)
+        response = self.client.get("/405/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(405, response.status_code)
 
     def test_not_exist_urls(self):
         """Test that redirects kicking in when trying to go to 404 page."""
         LOGGER.debug("404 Test Redirect URLs")
         response = self.client.get("/UrlShouldNotExist/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(404, response.status_code)
 
     def test_500_urls(self):
         """Test the url of 500 page."""
         LOGGER.debug("500 Test Redirect URLs")
-        response = self.client.get("/test-500/", follow=True)
+        response = self.client.get("/500/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(500, response.status_code)
-
-    # def test_X_redirect_urls(self):
-    # """Test that redirects end urls"""
-    # LOGGER.debug("Test X Redirect URLs")
-    # response = self.client.get('/403/', follow=True)
-    # self.assertRedirects(response, "http://testserver/admin/login/?next=/admin/")
+        self.assertTemplateUsed(response, "errors/500.html")
```

### Comparing `django-errors-1.6.8/tests/views.py` & `django-errors-2.1.0/tests/views_standard.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 """Test's view for django-errors"""
 from django.http import (
-    HttpResponse,
     HttpResponseBadRequest,
     HttpResponseForbidden,
+    HttpResponseGone,
     HttpResponseNotAllowed,
     HttpResponseNotFound,
     HttpResponseServerError,
 )
 from django.views.decorators.http import require_http_methods
 
 
-def test_view(request):
-    """Test's view"""
-    if request.method != "GET":
-        return HttpResponseNotFound("404 view")
-    return HttpResponse("Test view")
-
-
 def test_view_400(request):
     """Test's view code 400"""
-    return HttpResponseBadRequest("400 view")
+    return HttpResponseBadRequest()
 
 
 def test_view_403(request):
     """Test's view code 403"""
-    return HttpResponseForbidden("403 view")
+    return HttpResponseForbidden()
+
+
+def test_view_404(request):
+    """Test's view code 404"""
+    return HttpResponseNotFound()
 
 
 @require_http_methods(["POST"])
 def test_view_405(request):
     """Test's view code 405"""
-    return HttpResponseNotAllowed("405 view")
+    return HttpResponseNotAllowed(["POST"])
+
+
+def test_view_410(request):
+    """Test's view code 410"""
+    return HttpResponseGone()
 
 
 def test_view_500(request):
-    """Test's view code 400"""
-    return HttpResponseServerError("500 view")
+    """Test's view code 500"""
+    return HttpResponseServerError()
```

### Comparing `django-errors-1.6.8/tox.ini` & `django-errors-2.1.0/tox.ini`

 * *Files identical despite different names*

