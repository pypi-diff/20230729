# Comparing `tmp/django-errors-2.1.0.tar.gz` & `tmp/django-errors-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-errors-2.1.0.tar", last modified: Sat Jul 29 14:14:17 2023, max compression
+gzip compressed data, was "django-errors-2.3.0.tar", last modified: Sat Jul 29 15:36:47 2023, max compression
```

## Comparing `django-errors-2.1.0.tar` & `django-errors-2.3.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.220628 django-errors-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-29 14:14:04.000000 django-errors-2.1.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-29 14:14:04.000000 django-errors-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-29 14:14:04.000000 django-errors-2.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-29 14:14:04.000000 django-errors-2.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-29 14:14:04.000000 django-errors-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-29 14:14:04.000000 django-errors-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-29 14:14:17.220628 django-errors-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-29 14:14:04.000000 django-errors-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-29 14:14:04.000000 django-errors-2.1.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-29 14:14:04.000000 django-errors-2.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)    29701 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/py310-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/py310-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/py311-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/py311-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/py38-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/py38-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/py39-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/py39-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-29 14:14:04.000000 django-errors-2.1.0/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-29 14:14:04.000000 django-errors-2.1.0/runtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-29 14:14:17.220628 django-errors-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-29 14:14:04.000000 django-errors-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.208628 django-errors-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/src/django_errors/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.208628 django-errors-2.1.0/src/django_errors/locale/cn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/cn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/cn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.208628 django-errors-2.1.0/src/django_errors/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.208628 django-errors-2.1.0/src/django_errors/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.208628 django-errors-2.1.0/src/django_errors/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/src/django_errors/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/src/django_errors/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/src/django_errors/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/src/django_errors/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/src/django_errors/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/src/django_errors/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/src/django_errors/locale/zh_hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/zh_hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/zh_hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.212628 django-errors-2.1.0/src/django_errors/locale/zh_hant/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/locale/zh_hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/locale/zh_hant/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/middleware/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors/templates/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/templates/errors/400.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/templates/errors/403.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/templates/errors/404.html
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/templates/errors/405.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/templates/errors/500.html
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-07-29 14:14:04.000000 django-errors-2.1.0/src/django_errors/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.216628 django-errors-2.1.0/src/django_errors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-29 14:14:17.000000 django-errors-2.1.0/src/django_errors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-29 14:14:17.000000 django-errors-2.1.0/src/django_errors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 14:14:17.000000 django-errors-2.1.0/src/django_errors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 14:14:17.000000 django-errors-2.1.0/src/django_errors.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-29 14:14:17.000000 django-errors-2.1.0/src/django_errors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 14:14:17.000000 django-errors-2.1.0/src/django_errors.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:17.220628 django-errors-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/test_errors_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/test_errors_locale_it.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/test_errors_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/test_errors_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/test_errors_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/views_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/views_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-29 14:14:04.000000 django-errors-2.1.0/tests/views_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-29 14:14:04.000000 django-errors-2.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.771132 django-errors-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-29 15:36:33.000000 django-errors-2.3.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-29 15:36:33.000000 django-errors-2.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-29 15:36:33.000000 django-errors-2.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-29 15:36:33.000000 django-errors-2.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-29 15:36:33.000000 django-errors-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-29 15:36:33.000000 django-errors-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-29 15:36:47.771132 django-errors-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-29 15:36:33.000000 django-errors-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-29 15:36:33.000000 django-errors-2.3.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-29 15:36:33.000000 django-errors-2.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)    29701 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/py310-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/py310-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/py311-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/py311-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/py38-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/py38-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/py39-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/py39-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-29 15:36:33.000000 django-errors-2.3.0/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-29 15:36:47.771132 django-errors-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-29 15:36:33.000000 django-errors-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.759132 django-errors-2.3.0/src/django_errors/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/cn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/cn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/cn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/zh_hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.767132 django-errors-2.3.0/src/django_errors/locale/zh_hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/zh_hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.759132 django-errors-2.3.0/src/django_errors/locale/zh_hant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.767132 django-errors-2.3.0/src/django_errors/locale/zh_hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/zh_hant/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.767132 django-errors-2.3.0/src/django_errors/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/middleware/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.767132 django-errors-2.3.0/src/django_errors/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.767132 django-errors-2.3.0/src/django_errors/templates/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/templates/errors/400.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/templates/errors/403.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/templates/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/templates/errors/405.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/templates/errors/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-29 15:36:47.000000 django-errors-2.3.0/src/django_errors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-29 15:36:47.000000 django-errors-2.3.0/src/django_errors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 15:36:47.000000 django-errors-2.3.0/src/django_errors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 15:36:47.000000 django-errors-2.3.0/src/django_errors.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-29 15:36:47.000000 django-errors-2.3.0/src/django_errors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 15:36:47.000000 django-errors-2.3.0/src/django_errors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.771132 django-errors-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/test_errors_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/test_errors_locale_it.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/test_errors_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/test_errors_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/test_errors_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/views_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/views_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/views_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-29 15:36:33.000000 django-errors-2.3.0/tox.ini
```

### Comparing `django-errors-2.1.0/.pre-commit-config.yaml` & `django-errors-2.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/LICENSE` & `django-errors-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/PKG-INFO` & `django-errors-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-errors
-Version: 2.1.0
+Version: 2.3.0
 Summary: Django application for handling server errors.
 Home-page: https://github.com/DLRSP/django-errors
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,errors
 Classifier: Development Status :: 4 - Beta
@@ -41,15 +41,15 @@
 [![PyPi python version](https://img.shields.io/pypi/pyversions/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 [![PyPi downloads](https://img.shields.io/pypi/dm/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 [![PyPi downloads](https://img.shields.io/pypi/dw/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 [![PyPi downloads](https://img.shields.io/pypi/dd/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 
 ## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-errors.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-errors.svg)
 
-## Test [![codecov.io](https://codecov.io/github/DLRSP/django-errors/coverage.svg?branch=master)](https://codecov.io/github/DLRSP/django-errors?branch=master) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-errors/master.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-errors/master) [![gitthub.com](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml/badge.svg)](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml)
+## Test [![codecov.io](https://codecov.io/github/DLRSP/django-errors/coverage.svg?branch=main)](https://codecov.io/github/DLRSP/django-errors?branch=main) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-errors/main.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-errors/main) [![gitthub.com](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml/badge.svg)](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml)
 
 ## Check Demo Project
 * Browser the demo app on-line on [Heroku](https://django-errors.herokuapp.com/)
 * Check the demo repo on [GitHub](https://github.com/DLRSP/example/tree/django-errors)
 
 ## Requirements
 -   Python 3.8+ supported.
```

### Comparing `django-errors-2.1.0/README.md` & `django-errors-2.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![PyPi python version](https://img.shields.io/pypi/pyversions/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 [![PyPi downloads](https://img.shields.io/pypi/dm/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 [![PyPi downloads](https://img.shields.io/pypi/dw/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 [![PyPi downloads](https://img.shields.io/pypi/dd/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 
 ## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-errors.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-errors.svg)
 
-## Test [![codecov.io](https://codecov.io/github/DLRSP/django-errors/coverage.svg?branch=master)](https://codecov.io/github/DLRSP/django-errors?branch=master) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-errors/master.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-errors/master) [![gitthub.com](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml/badge.svg)](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml)
+## Test [![codecov.io](https://codecov.io/github/DLRSP/django-errors/coverage.svg?branch=main)](https://codecov.io/github/DLRSP/django-errors?branch=main) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-errors/main.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-errors/main) [![gitthub.com](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml/badge.svg)](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml)
 
 ## Check Demo Project
 * Browser the demo app on-line on [Heroku](https://django-errors.herokuapp.com/)
 * Check the demo repo on [GitHub](https://github.com/DLRSP/example/tree/django-errors)
 
 ## Requirements
 -   Python 3.8+ supported.
```

### Comparing `django-errors-2.1.0/mkdocs.yml` & `django-errors-2.3.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/pyproject.toml` & `django-errors-2.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 django_find_project = false
 
 [tool.towncrier]
 package = "django_errors"
 package_dir = "src"
 filename = "CHANGELOG.rst"
 directory = "news/"
-version = "2.1.0"
+version = "2.3.0"
 
 # For rendering properly for this project
 issue_format = "`#{issue} <https://github.com/DLRSP/django-errors/issues/{issue}>`_"
 # template = "tools/news/template.rst"
 
 # Grouping of entries, within our changelog
 type = [
```

### Comparing `django-errors-2.1.0/requirements/docs.txt` & `django-errors-2.3.0/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/requirements/py310-django32.txt` & `django-errors-2.3.0/requirements/py310-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/requirements/py310-django42.txt` & `django-errors-2.3.0/requirements/py310-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/requirements/py311-django32.txt` & `django-errors-2.3.0/requirements/py311-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/requirements/py311-django42.txt` & `django-errors-2.3.0/requirements/py311-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/requirements/py38-django32.txt` & `django-errors-2.3.0/requirements/py38-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/requirements/py38-django42.txt` & `django-errors-2.3.0/requirements/py38-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/requirements/py39-django32.txt` & `django-errors-2.3.0/requirements/py39-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/requirements/py39-django42.txt` & `django-errors-2.3.0/requirements/py39-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/runtests.py` & `django-errors-2.3.0/runtests.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/setup.cfg` & `django-errors-2.3.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = django-errors
-version = 2.1.0
+version = 2.3.0
 url = https://github.com/DLRSP/django-errors
 author = DLRSP
 author_email = dlrsp.dev@gmail.com
 description = Django application for handling server errors.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `django-errors-2.1.0/setup.py` & `django-errors-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/src/django_errors/__init__.py` & `django-errors-2.3.0/src/django_errors/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 4. push to pypi + push to github
 5. bump the version, append '.dev0'
 6. git commit
 7. push to github (to avoid confusion)
 """
 import django
 
-__version__ = "2.1.0"
+__version__ = "2.3.0"
 __version_info__ = tuple(int(i) if i.isdigit() else i for i in __version__.split("."))
 __license__ = "MIT"
 __title__ = "django_errors"
 
 __author__ = "DLRSP"
 __copyright__ = "Copyright 2010-present DLRSP"
```

### Comparing `django-errors-2.1.0/src/django_errors/locale/cn/LC_MESSAGES/django.po` & `django-errors-2.3.0/src/django_errors/locale/cn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/src/django_errors/locale/de/LC_MESSAGES/django.po` & `django-errors-2.3.0/src/django_errors/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/src/django_errors/locale/en/LC_MESSAGES/django.po` & `django-errors-2.3.0/src/django_errors/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/src/django_errors/locale/es/LC_MESSAGES/django.po` & `django-errors-2.3.0/src/django_errors/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/src/django_errors/locale/fr/LC_MESSAGES/django.po` & `django-errors-2.3.0/src/django_errors/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/src/django_errors/locale/it/LC_MESSAGES/django.po` & `django-errors-2.3.0/src/django_errors/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/src/django_errors/locale/ja/LC_MESSAGES/django.po` & `django-errors-2.3.0/src/django_errors/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/src/django_errors/locale/lt/LC_MESSAGES/django.po` & `django-errors-2.3.0/src/django_errors/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/src/django_errors/locale/nl/LC_MESSAGES/django.po` & `django-errors-2.3.0/src/django_errors/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/src/django_errors/locale/ru/LC_MESSAGES/django.po` & `django-errors-2.3.0/src/django_errors/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/src/django_errors/locale/zh_hans/LC_MESSAGES/django.po` & `django-errors-2.3.0/src/django_errors/locale/zh_hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/src/django_errors/locale/zh_hant/LC_MESSAGES/django.po` & `django-errors-2.3.0/src/django_errors/locale/zh_hant/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/src/django_errors/views.py` & `django-errors-2.3.0/src/django_errors/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Django Views for django-errors module"""
 from django.conf import settings
 from django.http import (
     HttpResponseBadRequest,
     HttpResponseForbidden,
-    HttpResponseNotAllowed,
     HttpResponseNotFound,
     HttpResponseServerError,
 )
 from django.template import loader
 from django.utils.translation import gettext_lazy as _
 from django.views.decorators.http import require_http_methods
 
@@ -76,37 +75,14 @@
         "error_message": error_msg,
         "error_request_method": request.method,
         "exception": exception,
     }
     return HttpResponseNotFound(template.render(context, request))
 
 
-def custom_405(request, permitted_methods=None, exception=None):
-    """Custom Page for 405 error (Method Not Allowed). url: /405"""
-    if permitted_methods is None:
-        permitted_methods = ["GET", "POST"]
-    error = _("Method Not Allowed")
-    error_msg = _("Sorry, the used method is not allowed for the page with that URL.")
-    template = loader.get_template(
-        getattr(
-            settings,
-            "TEMPLATE_ERROR_405",
-            getattr(settings, "TEMPLATE_ERROR_ALL", "errors/405.html"),
-        )
-    )
-    context = {
-        "error": error,
-        "error_code": 405,
-        "error_message": error_msg,
-        "error_request_method": request.method,
-        "exception": exception,
-    }
-    return HttpResponseNotAllowed(permitted_methods, template.render(context, request))
-
-
 @require_http_methods(["GET"])
 def custom_500(request, exception=None):
     """Custom Page for 500 error (Internal Server Error). url: /500"""
     error = _("Internal Server Error")
     error_msg = _("Sorry, an error has occurred with the application.")
     template = loader.get_template(
         getattr(
```

### Comparing `django-errors-2.1.0/src/django_errors.egg-info/PKG-INFO` & `django-errors-2.3.0/src/django_errors.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-errors
-Version: 2.1.0
+Version: 2.3.0
 Summary: Django application for handling server errors.
 Home-page: https://github.com/DLRSP/django-errors
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,errors
 Classifier: Development Status :: 4 - Beta
@@ -41,15 +41,15 @@
 [![PyPi python version](https://img.shields.io/pypi/pyversions/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 [![PyPi downloads](https://img.shields.io/pypi/dm/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 [![PyPi downloads](https://img.shields.io/pypi/dw/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 [![PyPi downloads](https://img.shields.io/pypi/dd/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 
 ## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-errors.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-errors.svg)
 
-## Test [![codecov.io](https://codecov.io/github/DLRSP/django-errors/coverage.svg?branch=master)](https://codecov.io/github/DLRSP/django-errors?branch=master) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-errors/master.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-errors/master) [![gitthub.com](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml/badge.svg)](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml)
+## Test [![codecov.io](https://codecov.io/github/DLRSP/django-errors/coverage.svg?branch=main)](https://codecov.io/github/DLRSP/django-errors?branch=main) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-errors/main.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-errors/main) [![gitthub.com](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml/badge.svg)](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml)
 
 ## Check Demo Project
 * Browser the demo app on-line on [Heroku](https://django-errors.herokuapp.com/)
 * Check the demo repo on [GitHub](https://github.com/DLRSP/example/tree/django-errors)
 
 ## Requirements
 -   Python 3.8+ supported.
```

### Comparing `django-errors-2.1.0/src/django_errors.egg-info/SOURCES.txt` & `django-errors-2.3.0/src/django_errors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/tests/settings.py` & `django-errors-2.3.0/tests/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     "django.middleware.common.CommonMiddleware",
     "django.middleware.csrf.CsrfViewMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.middleware.locale.LocaleMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
     "django.middleware.clickjacking.XFrameOptionsMiddleware",
     "django.middleware.cache.FetchFromCacheMiddleware",
+    "django_errors.middleware.handler.HttpResponseNotAllowedMiddleware",
 )
 
 USE_TZ = True
 LANGUAGE_CODE = "en"
 USE_I18N = True
 
 STATIC_URL = "/static/"
```

### Comparing `django-errors-2.1.0/tests/test_errors.py` & `django-errors-2.3.0/tests/test_errors_exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,58 +13,44 @@
         """Set up common assets for tests"""
         LOGGER.debug("Tests setUp")
 
     def tearDown(self):
         """Remove Test Data"""
         LOGGER.debug("Tests tearDown")
 
-    def test_not_exist_urls(self):
-        """Test that redirects kicking in when trying to go to 404 page."""
-        LOGGER.debug("404 Test URL not exist")
-        response = self.client.get("/UrlShouldNotExist/", follow=True)
+    def test_400_exception_SuspiciousOperation(self):
+        """Test the url of 400 page."""
+        LOGGER.debug("400 Test raise exception SuspiciousOperation")
+        response = self.client.get("/test-exception-400/", follow=True)
+        LOGGER.debug(response)
+        self.assertEqual(400, response.status_code)
+        self.assertTemplateUsed(response, "errors/400.html")
+
+    def test_403_exception_PermissionDenied(self):
+        """Test the url of 403 page."""
+        LOGGER.debug("403 Test raise exception PermissionDenied")
+        response = self.client.get("/test-exception-403/", follow=True)
+        LOGGER.debug(response)
+        self.assertEqual(403, response.status_code)
+        self.assertTemplateUsed(response, "errors/403.html")
+
+    def test_404_exception_Http404(self):
+        """Test the url of 404 page."""
+        LOGGER.debug("404 raise exception Http404")
+        response = self.client.get("/test-exception-404/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(404, response.status_code)
         self.assertTemplateUsed(response, "errors/404.html")
 
-    def test_page_auth_protected(self):
-        """Test that redirects kicking in when trying to go to a page Auth protected."""
-        LOGGER.debug("Test URL accept only get")
-        response = self.client.get("/admin/", follow=True)
+    def test_500_exception_InternalError(self):
+        """Test the url of 500 page."""
+        LOGGER.debug("500 Test raise exception InternalError")
+        response = self.client.get("/500/", follow=True)
         LOGGER.debug(response)
-        # self.assertEqual(403, response.status_code)
-        # self.assertTemplateUsed(response, 'errors/403.html')
-        self.assertRedirects(response, "/admin/login/?next=%2Fadmin%2F")
-
-    def test_page_without_privileges(self):
-        """Test that redirects kicking in when trying to go to a page Auth protected."""
-        LOGGER.debug("Test URL accept only get")
-        response = self.client.get("/admin/", follow=True)
-        LOGGER.debug(response)
-        # self.assertEqual(403, response.status_code)
-        # self.assertTemplateUsed(response, 'errors/403.html')
-        self.assertRedirects(response, "/admin/login/?next=%2Fadmin%2F")
+        self.assertEqual(500, response.status_code)
+        self.assertTemplateUsed(response, "errors/500.html")
 
     # def test_X_redirect_urls(self):
-    #     """Test that redirects end urls"""
-    #     LOGGER.debug("Test X Redirect URLs")
-    #     response = self.client.get('/403/', follow=True)
-    #     self.assertRedirects(response, "http://testserver/admin/login/?next=/admin/")
-
-    def test_method_not_allowed_get(self):
-        """Test that redirects kicking in when trying
-        to use method GET on view accept only POST."""
-        LOGGER.debug("Test URL accept only get")
-        response = self.client.get("/test-method-only-post/", follow=True)
-        LOGGER.debug(response)
-        self.assertEqual(405, response.status_code)
-        # todo: 405 handle doesn't use custom view
-        # self.assertTemplateUsed(response, 'errors/405.html')
-
-    def test_method_not_allowed_post(self):
-        """Test that redirects kicking in when trying
-        to use method POST on view accept only GET."""
-        LOGGER.debug("Test URL accept only get")
-        response = self.client.post("/test-method-only-get/", follow=True)
-        LOGGER.debug(response)
-        self.assertEqual(405, response.status_code)
-        # todo: 405 handle doesn't use custom view
-        # self.assertTemplateUsed(response, 'errors/405.html')
+    # """Test that redirects end urls"""
+    # LOGGER.debug("Test X Redirect URLs")
+    # response = self.client.get('/403/', follow=True)
+    # self.assertRedirects(response, "http://testserver/admin/login/?next=/admin/")
```

### Comparing `django-errors-2.1.0/tests/test_errors_exceptions.py` & `django-errors-2.3.0/tests/test_errors_urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,44 +13,42 @@
         """Set up common assets for tests"""
         LOGGER.debug("Tests setUp")
 
     def tearDown(self):
         """Remove Test Data"""
         LOGGER.debug("Tests tearDown")
 
-    def test_400_exception_SuspiciousOperation(self):
+    def test_400_urls(self):
         """Test the url of 400 page."""
-        LOGGER.debug("400 Test raise exception SuspiciousOperation")
-        response = self.client.get("/test-exception-400/", follow=True)
+        LOGGER.debug("400 Test Redirect URLs")
+        response = self.client.get("/400/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(400, response.status_code)
-        self.assertTemplateUsed(response, "errors/400.html")
 
-    def test_403_exception_PermissionDenied(self):
+    def test_403_urls(self):
         """Test the url of 403 page."""
-        LOGGER.debug("403 Test raise exception PermissionDenied")
-        response = self.client.get("/test-exception-403/", follow=True)
+        LOGGER.debug("403 Test Redirect URLs")
+        response = self.client.get("/403/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(403, response.status_code)
-        self.assertTemplateUsed(response, "errors/403.html")
 
-    def test_404_exception_Http404(self):
+    def test_404_urls(self):
         """Test the url of 404 page."""
-        LOGGER.debug("404 raise exception Http404")
-        response = self.client.get("/test-exception-404/", follow=True)
+        LOGGER.debug("404 Test URLs")
+        response = self.client.get("/404/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(404, response.status_code)
-        self.assertTemplateUsed(response, "errors/404.html")
 
-    def test_500_exception_InternalError(self):
+    def test_not_exist_urls(self):
+        """Test that redirects kicking in when trying to go to 404 page."""
+        LOGGER.debug("404 Test Redirect URLs")
+        response = self.client.get("/UrlShouldNotExist/", follow=True)
+        LOGGER.debug(response)
+        self.assertEqual(404, response.status_code)
+
+    def test_500_urls(self):
         """Test the url of 500 page."""
-        LOGGER.debug("500 Test raise exception InternalError")
+        LOGGER.debug("500 Test Redirect URLs")
         response = self.client.get("/500/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(500, response.status_code)
         self.assertTemplateUsed(response, "errors/500.html")
-
-    # def test_X_redirect_urls(self):
-    # """Test that redirects end urls"""
-    # LOGGER.debug("Test X Redirect URLs")
-    # response = self.client.get('/403/', follow=True)
-    # self.assertRedirects(response, "http://testserver/admin/login/?next=/admin/")
```

### Comparing `django-errors-2.1.0/tests/test_errors_locale_it.py` & `django-errors-2.3.0/tests/test_errors_standard.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,77 +13,56 @@
         """Set up common assets for tests"""
         LOGGER.debug("Tests setUp")
 
     def tearDown(self):
         """Remove Test Data"""
         LOGGER.debug("Tests tearDown")
 
-    def test_400_template_locale_it(self):
+    def test_400_standard(self):
         """Test the url of 400 page."""
-        LOGGER.debug("400 Test URLs")
-        response = self.client.get("/it/test-template-400/", follow=True)
-        LOGGER.debug(response)
-        self.assertEqual(400, response.status_code)
-        self.assertContains(response, b"Brutta Richiesta", status_code=400, count=2)
+        LOGGER.debug("400 Test Standard view overwrite")
+        response = self.client.get("/400/", follow=True)
+        response_standard = self.client.get("/test-standard-400/", follow=True)
+        LOGGER.debug(response)
+        self.assertEqual(type(response), type(response_standard))
+        self.assertEqual(response.status_code, response_standard.status_code)
+        self.assertTemplateUsed(response, "errors/400.html")
 
-    def test_403_template_locale_it(self):
+    def test_403_standard(self):
         """Test the url of 403 page."""
-        LOGGER.debug("403 Test URLs")
-        response = self.client.get("/it/test-template-403/", follow=True)
+        LOGGER.debug("403 Test Redirect URLs")
+        response = self.client.get("/403/", follow=True)
+        response_standard = self.client.get("/test-standard-403/", follow=True)
         LOGGER.debug(response)
-        self.assertEqual(403, response.status_code)
+        self.assertEqual(type(response), type(response_standard))
+        self.assertEqual(response.status_code, response_standard.status_code)
         self.assertTemplateUsed(response, "errors/403.html")
-        self.assertContains(response, b"Permesso Negato", status_code=403, count=2)
-        self.assertContains(
-            response,
-            b"Non hai il permesso per vedere questa pagina!",
-            status_code=403,
-            count=1,
-        )
 
-    def test_404_template_locale_it(self):
+    def test_404_standard(self):
         """Test the url of 404 page."""
         LOGGER.debug("404 Test URLs")
-        response = self.client.get("/it/test-template-404/", follow=True)
+        response = self.client.get("/404/", follow=True)
+        response_standard = self.client.get("/test-standard-404/", follow=True)
         LOGGER.debug(response)
-        self.assertEqual(404, response.status_code)
-        self.assertContains(response, b"Pagina non trovata", status_code=404, count=2)
+        self.assertEqual(type(response), type(response_standard))
+        self.assertEqual(response.status_code, response_standard.status_code)
+        self.assertTemplateUsed(response, "errors/404.html")
 
-    def test_not_exist_urls_locale_it(self):
-        """Test that redirects kicking in when trying to go to 404 page."""
-        LOGGER.debug("404 Test Redirect URLs")
-        response = self.client.get("/it/UrlShouldNotExist/", follow=True)
-        LOGGER.debug(response)
-        print(response.content)
-        self.assertEqual(404, response.status_code)
-        self.assertContains(response, b"Pagina non trovata", status_code=404, count=2)
-
-    def test_405_template_get_locale_it(self):
-        """Test the url of 405 page."""
-        LOGGER.debug("405 Test URLs")
-        response = self.client.get("/it/test-template-405-get/", follow=True)
-        LOGGER.debug(response)
-        self.assertEqual(405, response.status_code)
-        self.assertContains(
-            response, b"Metodo non consentito", status_code=405, count=2
-        )
-
-    def test_405_template_post_locale_it(self):
-        """Test the url of 405 page."""
-        LOGGER.debug("405 Test URLs")
-        response = self.client.post("/it/test-template-405-post/", follow=True)
-        LOGGER.debug(response)
-        self.assertEqual(405, response.status_code)
-        self.assertContains(
-            response, b"Metodo non consentito", status_code=405, count=2
-        )
-
-    def test_500_template_locale_it(self):
-        """Test the url of 400 page."""
-        LOGGER.debug("500 Test URLs")
-        response = self.client.get("/it/test-template-500/", follow=True)
+    def test_405_standard(self):
+        """Test the url of 404 page."""
+        LOGGER.debug("405 Test GET URLs with only POST")
+        response = self.client.post("/400/", follow=True)
+        response_standard = self.client.get("/test-standard-405/", follow=True)
+        LOGGER.debug(response)
+        self.assertEqual(type(response), type(response_standard))
+        self.assertEqual(response.status_code, response_standard.status_code)
+        self.assertTemplateUsed(response, "errors/405.html")
+
+    def test_500_standard(self):
+        """Test the url of 500 page."""
+        LOGGER.debug("500 Test Redirect URLs")
+        response = self.client.get("/500/", follow=True)
+        response_standard = self.client.get("/test-standard-500/", follow=True)
         LOGGER.debug(response)
-        self.assertEqual(500, response.status_code)
+        self.assertEqual(type(response), type(response_standard))
+        self.assertEqual(response.status_code, response_standard.status_code)
         self.assertTemplateUsed(response, "errors/500.html")
-        self.assertContains(
-            response, b"Errore Interno del Server", status_code=500, count=2
-        )
```

### Comparing `django-errors-2.1.0/tests/test_errors_templates.py` & `django-errors-2.3.0/tests/test_errors_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,36 +63,35 @@
             status_code=404,
             count=1,
         )
 
     def test_405_template_get(self):
         """Test the url of 405 page."""
         LOGGER.debug("405 Test URLs")
-        response = self.client.get("/test-template-405-get/", follow=True)
+        response = self.client.get("/test-method-only-post/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(405, response.status_code)
         self.assertTemplateUsed(response, "errors/405.html")
         self.assertContains(
             response, b"Method Not Allowed (GET)[405]", status_code=405, count=1
         )
         self.assertContains(
             response, b"Method Not Allowed (GET)", status_code=405, count=2
         )
-        print(response.content)
         self.assertContains(
             response,
             b"Sorry, the used method is not allowed for the page with that URL.",
             status_code=405,
             count=1,
         )
 
     def test_405_template_post(self):
         """Test the url of 405 page."""
         LOGGER.debug("405 Test URLs")
-        response = self.client.post("/test-template-405-post/", follow=True)
+        response = self.client.post("/test-method-only-get/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(405, response.status_code)
         self.assertTemplateUsed(response, "errors/405.html")
         self.assertContains(
             response, b"Method Not Allowed (POST)[405]", status_code=405, count=1
         )
         self.assertContains(
```

### Comparing `django-errors-2.1.0/tests/test_errors_urls.py` & `django-errors-2.3.0/tests/test_errors.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,49 +13,58 @@
         """Set up common assets for tests"""
         LOGGER.debug("Tests setUp")
 
     def tearDown(self):
         """Remove Test Data"""
         LOGGER.debug("Tests tearDown")
 
-    def test_400_urls(self):
-        """Test the url of 400 page."""
-        LOGGER.debug("400 Test Redirect URLs")
-        response = self.client.get("/400/", follow=True)
-        LOGGER.debug(response)
-        self.assertEqual(400, response.status_code)
-
-    def test_403_urls(self):
-        """Test the url of 403 page."""
-        LOGGER.debug("403 Test Redirect URLs")
-        response = self.client.get("/403/", follow=True)
-        LOGGER.debug(response)
-        self.assertEqual(403, response.status_code)
-
-    def test_404_urls(self):
-        """Test the url of 404 page."""
-        LOGGER.debug("404 Test URLs")
-        response = self.client.get("/404/", follow=True)
-        LOGGER.debug(response)
-        self.assertEqual(404, response.status_code)
-
-    def test_405_urls(self):
-        """Test the url of 404 page."""
-        LOGGER.debug("405 Test GET URLs with only POST")
-        response = self.client.get("/405/", follow=True)
-        LOGGER.debug(response)
-        self.assertEqual(405, response.status_code)
-
     def test_not_exist_urls(self):
         """Test that redirects kicking in when trying to go to 404 page."""
-        LOGGER.debug("404 Test Redirect URLs")
+        LOGGER.debug("404 Test URL not exist")
         response = self.client.get("/UrlShouldNotExist/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(404, response.status_code)
+        self.assertTemplateUsed(response, "errors/404.html")
 
-    def test_500_urls(self):
-        """Test the url of 500 page."""
-        LOGGER.debug("500 Test Redirect URLs")
-        response = self.client.get("/500/", follow=True)
+    def test_page_auth_protected(self):
+        """Test that redirects kicking in when trying to go to a page Auth protected."""
+        LOGGER.debug("Test URL accept only get")
+        response = self.client.get("/admin/", follow=True)
+        LOGGER.debug(response)
+        # todo: test auth protected: NOT_AUTHORIZED (should be 401)
+        # self.assertEqual(403, response.status_code)
+        # self.assertTemplateUsed(response, 'errors/403.html')
+        self.assertRedirects(response, "/admin/login/?next=%2Fadmin%2F")
+
+    def test_page_without_privileges(self):
+        """Test that redirects kicking in when trying to go to a page Auth protected."""
+        LOGGER.debug("Test URL accept only get")
+        response = self.client.get("/admin/", follow=True)
+        LOGGER.debug(response)
+        # todo: test auth protected: NOT_AUTHORIZED (should be 401)
+        # self.assertEqual(403, response.status_code)
+        # self.assertTemplateUsed(response, 'errors/403.html')
+        self.assertRedirects(response, "/admin/login/?next=%2Fadmin%2F")
+
+    # def test_X_redirect_urls(self):
+    #     """Test that redirects end urls"""
+    #     LOGGER.debug("Test X Redirect URLs")
+    #     response = self.client.get('/403/', follow=True)
+    #     self.assertRedirects(response, "http://testserver/admin/login/?next=/admin/")
+
+    def test_method_not_allowed_get(self):
+        """Test that redirects kicking in when trying
+        to use method GET on view accept only POST."""
+        LOGGER.debug("Test URL accept only get")
+        response = self.client.get("/test-method-only-post/", follow=True)
         LOGGER.debug(response)
-        self.assertEqual(500, response.status_code)
-        self.assertTemplateUsed(response, "errors/500.html")
+        self.assertEqual(405, response.status_code)
+        self.assertTemplateUsed(response, "errors/405.html")
+
+    def test_method_not_allowed_post(self):
+        """Test that redirects kicking in when trying
+        to use method POST on view accept only GET."""
+        LOGGER.debug("Test URL accept only get")
+        response = self.client.post("/test-method-only-get/", follow=True)
+        LOGGER.debug(response)
+        self.assertEqual(405, response.status_code)
+        self.assertTemplateUsed(response, "errors/405.html")
```

### Comparing `django-errors-2.1.0/tests/urls.py` & `django-errors-2.3.0/tests/urls.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,16 +15,14 @@
     path("test-method-only-post/", views.test_view_405_only_post),
     path("test-exception-400/", views_exceptions.test_exception_400),
     path("test-exception-403/", views_exceptions.test_exception_403),
     path("test-exception-404/", views_exceptions.test_exception_404),
     path("test-template-400/", views_templates.test_template_400),
     path("test-template-403/", views_templates.test_template_403),
     path("test-template-404/", views_templates.test_template_404),
-    path("test-template-405-get/", views_templates.test_template_405_get),
-    path("test-template-405-post/", views_templates.test_template_405_post),
     path("test-template-500/", views_templates.test_template_500),
     path("test-standard-400/", views_standard.test_view_400),
     path("test-standard-403/", views_standard.test_view_403),
     path("test-standard-404/", views_standard.test_view_404),
     path("test-standard-405/", views_standard.test_view_405),
     path("test-standard-410/", views_standard.test_view_410),
     path("test-standard-500/", views_standard.test_view_500),
@@ -37,16 +35,14 @@
     path("test-method-only-post/", views.test_view_405_only_post),
     path("test-exception-400/", views_exceptions.test_exception_400),
     path("test-exception-403/", views_exceptions.test_exception_403),
     path("test-exception-404/", views_exceptions.test_exception_404),
     path("test-template-400/", views_templates.test_template_400),
     path("test-template-403/", views_templates.test_template_403),
     path("test-template-404/", views_templates.test_template_404),
-    path("test-template-405-get/", views_templates.test_template_405_get),
-    path("test-template-405-post/", views_templates.test_template_405_post),
     path("test-template-500/", views_templates.test_template_500),
     path("test-standard-400/", views_standard.test_view_400),
     path("test-standard-403/", views_standard.test_view_403),
     path("test-standard-404/", views_standard.test_view_404),
     path("test-standard-405/", views_standard.test_view_405),
     path("test-standard-410/", views_standard.test_view_410),
     path("test-standard-500/", views_standard.test_view_500),
@@ -59,12 +55,9 @@
 
 handler403 = errors_views.custom_403
 """ Handle 403 error """
 
 handler404 = errors_views.custom_404
 """ Handle 404 error """
 
-handler405 = errors_views.custom_405
-""" Handle 405 error """
-
 handler500 = errors_views.custom_500
 """ Handle 500 error """
```

### Comparing `django-errors-2.1.0/tests/views.py` & `django-errors-2.3.0/tests/views.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/tests/views_standard.py` & `django-errors-2.3.0/tests/views_standard.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.1.0/tox.ini` & `django-errors-2.3.0/tox.ini`

 * *Files identical despite different names*

