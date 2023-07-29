# Comparing `tmp/django-errors-2.3.0.tar.gz` & `tmp/django-errors-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-errors-2.3.0.tar", last modified: Sat Jul 29 15:36:47 2023, max compression
+gzip compressed data, was "django-errors-2.3.2.tar", last modified: Sat Jul 29 16:17:48 2023, max compression
```

## Comparing `django-errors-2.3.0.tar` & `django-errors-2.3.2.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.771132 django-errors-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-29 15:36:33.000000 django-errors-2.3.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-29 15:36:33.000000 django-errors-2.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-29 15:36:33.000000 django-errors-2.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-29 15:36:33.000000 django-errors-2.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-29 15:36:33.000000 django-errors-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-29 15:36:33.000000 django-errors-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-29 15:36:47.771132 django-errors-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-29 15:36:33.000000 django-errors-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-29 15:36:33.000000 django-errors-2.3.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-29 15:36:33.000000 django-errors-2.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)    29701 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/py310-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/py310-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/py311-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/py311-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/py38-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/py38-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/py39-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/py39-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-29 15:36:33.000000 django-errors-2.3.0/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-29 15:36:33.000000 django-errors-2.3.0/runtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-29 15:36:47.771132 django-errors-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-29 15:36:33.000000 django-errors-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.759132 django-errors-2.3.0/src/django_errors/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/cn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/cn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/cn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.755132 django-errors-2.3.0/src/django_errors/locale/zh_hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.767132 django-errors-2.3.0/src/django_errors/locale/zh_hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/zh_hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.759132 django-errors-2.3.0/src/django_errors/locale/zh_hant/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.767132 django-errors-2.3.0/src/django_errors/locale/zh_hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/locale/zh_hant/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.767132 django-errors-2.3.0/src/django_errors/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/middleware/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.767132 django-errors-2.3.0/src/django_errors/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.767132 django-errors-2.3.0/src/django_errors/templates/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/templates/errors/400.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/templates/errors/403.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/templates/errors/404.html
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/templates/errors/405.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/templates/errors/500.html
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-29 15:36:33.000000 django-errors-2.3.0/src/django_errors/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.763132 django-errors-2.3.0/src/django_errors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-29 15:36:47.000000 django-errors-2.3.0/src/django_errors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-29 15:36:47.000000 django-errors-2.3.0/src/django_errors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 15:36:47.000000 django-errors-2.3.0/src/django_errors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 15:36:47.000000 django-errors-2.3.0/src/django_errors.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-29 15:36:47.000000 django-errors-2.3.0/src/django_errors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 15:36:47.000000 django-errors-2.3.0/src/django_errors.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:47.771132 django-errors-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/test_errors_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/test_errors_locale_it.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/test_errors_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/test_errors_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/test_errors_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/views_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/views_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-29 15:36:33.000000 django-errors-2.3.0/tests/views_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-29 15:36:33.000000 django-errors-2.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.664380 django-errors-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-29 16:17:34.000000 django-errors-2.3.2/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-29 16:17:34.000000 django-errors-2.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-29 16:17:34.000000 django-errors-2.3.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-29 16:17:34.000000 django-errors-2.3.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-29 16:17:34.000000 django-errors-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-29 16:17:34.000000 django-errors-2.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-29 16:17:48.664380 django-errors-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-29 16:17:34.000000 django-errors-2.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-29 16:17:34.000000 django-errors-2.3.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-29 16:17:34.000000 django-errors-2.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)    29213 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/py310-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/py310-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/py311-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/py311-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/py38-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/py38-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/py39-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/py39-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-29 16:17:34.000000 django-errors-2.3.2/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-29 16:17:48.664380 django-errors-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-29 16:17:34.000000 django-errors-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.648379 django-errors-2.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.652379 django-errors-2.3.2/src/django_errors/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.648379 django-errors-2.3.2/src/django_errors/locale/cn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/locale/cn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/cn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.648379 django-errors-2.3.2/src/django_errors/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.648379 django-errors-2.3.2/src/django_errors/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.648379 django-errors-2.3.2/src/django_errors/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.648379 django-errors-2.3.2/src/django_errors/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.652379 django-errors-2.3.2/src/django_errors/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.652379 django-errors-2.3.2/src/django_errors/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.652379 django-errors-2.3.2/src/django_errors/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.652379 django-errors-2.3.2/src/django_errors/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.652379 django-errors-2.3.2/src/django_errors/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.660380 django-errors-2.3.2/src/django_errors/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.652379 django-errors-2.3.2/src/django_errors/locale/zh_hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.660380 django-errors-2.3.2/src/django_errors/locale/zh_hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/zh_hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.652379 django-errors-2.3.2/src/django_errors/locale/zh_hant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.660380 django-errors-2.3.2/src/django_errors/locale/zh_hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/zh_hant/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.660380 django-errors-2.3.2/src/django_errors/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/middleware/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.660380 django-errors-2.3.2/src/django_errors/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.660380 django-errors-2.3.2/src/django_errors/templates/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/templates/errors/400.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/templates/errors/403.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/templates/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/templates/errors/405.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/templates/errors/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-29 16:17:48.000000 django-errors-2.3.2/src/django_errors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-29 16:17:48.000000 django-errors-2.3.2/src/django_errors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 16:17:48.000000 django-errors-2.3.2/src/django_errors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 16:17:48.000000 django-errors-2.3.2/src/django_errors.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-29 16:17:48.000000 django-errors-2.3.2/src/django_errors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 16:17:48.000000 django-errors-2.3.2/src/django_errors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.664380 django-errors-2.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/test_errors_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/test_errors_locale_it.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/test_errors_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/test_errors_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/test_errors_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/views_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/views_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/views_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-29 16:17:34.000000 django-errors-2.3.2/tox.ini
```

### Comparing `django-errors-2.3.0/.pre-commit-config.yaml` & `django-errors-2.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/LICENSE` & `django-errors-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/PKG-INFO` & `django-errors-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-errors
-Version: 2.3.0
+Version: 2.3.2
 Summary: Django application for handling server errors.
 Home-page: https://github.com/DLRSP/django-errors
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,errors
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-errors-2.3.0/README.md` & `django-errors-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/mkdocs.yml` & `django-errors-2.3.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/pyproject.toml` & `django-errors-2.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 django_find_project = false
 
 [tool.towncrier]
 package = "django_errors"
 package_dir = "src"
 filename = "CHANGELOG.rst"
 directory = "news/"
-version = "2.3.0"
+version = "2.3.2"
 
 # For rendering properly for this project
 issue_format = "`#{issue} <https://github.com/DLRSP/django-errors/issues/{issue}>`_"
 # template = "tools/news/template.rst"
 
 # Grouping of entries, within our changelog
 type = [
```

### Comparing `django-errors-2.3.0/requirements/docs.txt` & `django-errors-2.3.2/requirements/docs.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/docs.txt requirements/docs.in
 #
-certifi==2023.5.7 \
-    --hash=sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7 \
-    --hash=sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716
+certifi==2023.7.22 \
+    --hash=sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082 \
+    --hash=sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9
     # via requests
 charset-normalizer==3.2.0 \
     --hash=sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96 \
     --hash=sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c \
     --hash=sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710 \
     --hash=sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706 \
     --hash=sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020 \
@@ -105,20 +105,14 @@
     --hash=sha256:8d9b8cb1e80b9735e8717c9362079d3ce4c6e5ddeebedd0361b228c3a67a62f6 \
     --hash=sha256:e3d59b1c2c6ebb9dfa7a184daf3b6dd4914237e7488a1730a6d8f6f5d0b4187f
     # via mkdocs-git-revision-date-plugin
 idna==3.4 \
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
     # via requests
-importlib-metadata==6.8.0 \
-    --hash=sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb \
-    --hash=sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743
-    # via
-    #   markdown
-    #   mkdocs
 jinja2==3.1.2 \
     --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
     --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
     # via
     #   mkdocs
     #   mkdocs-git-revision-date-plugin
     #   mkdocs-material
@@ -185,24 +179,24 @@
     --hash=sha256:0096d52e9dad9939c3d975a774666af186eda617e6ca84df4c94dec30004f2a8 \
     --hash=sha256:70775750742b25c0d8f36c55aed03d24c3384d17c951b3175d898bd778ef0307
     # via mkdocs
 mkdocs==1.4.3 \
     --hash=sha256:5955093bbd4dd2e9403c5afaf57324ad8b04f16886512a3ee6ef828956481c57 \
     --hash=sha256:6ee46d309bda331aac915cd24aab882c179a933bd9e77b80ce7d2eaaa3f689dd
     # via
-    #   -r requirements/docs.in
+    #   -r docs.in
     #   mkdocs-git-revision-date-plugin
     #   mkdocs-material
 mkdocs-git-revision-date-plugin==0.3.2 \
     --hash=sha256:2e67956cb01823dd2418e2833f3623dee8604cdf223bddd005fe36226a56f6ef
-    # via -r requirements/docs.in
+    # via -r docs.in
 mkdocs-material==9.1.18 \
     --hash=sha256:5bcf8fb79ac2f253c0ffe93fa181cba87718c6438f459dc4180ac7418cc9a450 \
     --hash=sha256:981dd39979723d4cda7cfc77bbbe5e54922d5761a7af23fb8ba9edb52f114b13
-    # via -r requirements/docs.in
+    # via -r docs.in
 mkdocs-material-extensions==1.1.1 \
     --hash=sha256:9c003da71e2cc2493d910237448c672e00cefc800d3d6ae93d2fc69979e3bd93 \
     --hash=sha256:e41d9f38e4798b6617ad98ca8f7f1157b1e4385ac1459ca1e4ea219b556df945
     # via mkdocs-material
 packaging==23.1 \
     --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
     --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
@@ -399,11 +393,7 @@
     --hash=sha256:adfdeab2da79ea2f76f87eb42a3ab1966a5313e5a69a0213a3cc06ef692b0e96 \
     --hash=sha256:ba07e92756c97e3aca0912b5cbc4e5ad802f4557212788e72a72a47ff376950d \
     --hash=sha256:c07253088265c363d1ddf4b3cdb808d59a0468ecd017770ed716991620b8f77a \
     --hash=sha256:c9d8c8ec7efb887333cf71e328e39cffbf771d8f8f95d308ea4125bf5f90ba64 \
     --hash=sha256:d00e6be486affb5781468457b21a6cbe848c33ef43f9ea4a73b4882e5f188a44 \
     --hash=sha256:d429c2430c93b7903914e4db9a966c7f2b068dd2ebdd2fa9b9ce094c7d459f33
     # via mkdocs
-zipp==3.16.2 \
-    --hash=sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0 \
-    --hash=sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147
-    # via importlib-metadata
```

### Comparing `django-errors-2.3.0/requirements/py310-django32.txt` & `django-errors-2.3.2/requirements/py310-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/requirements/py310-django42.txt` & `django-errors-2.3.2/requirements/py310-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/requirements/py311-django32.txt` & `django-errors-2.3.2/requirements/py311-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/requirements/py311-django42.txt` & `django-errors-2.3.2/requirements/py311-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/requirements/py38-django32.txt` & `django-errors-2.3.2/requirements/py38-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/requirements/py38-django42.txt` & `django-errors-2.3.2/requirements/py38-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/requirements/py39-django32.txt` & `django-errors-2.3.2/requirements/py39-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/requirements/py39-django42.txt` & `django-errors-2.3.2/requirements/py39-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/runtests.py` & `django-errors-2.3.2/runtests.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/setup.cfg` & `django-errors-2.3.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = django-errors
-version = 2.3.0
+version = 2.3.2
 url = https://github.com/DLRSP/django-errors
 author = DLRSP
 author_email = dlrsp.dev@gmail.com
 description = Django application for handling server errors.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `django-errors-2.3.0/setup.py` & `django-errors-2.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/src/django_errors/locale/cn/LC_MESSAGES/django.po` & `django-errors-2.3.2/src/django_errors/locale/cn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/src/django_errors/locale/de/LC_MESSAGES/django.po` & `django-errors-2.3.2/src/django_errors/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/src/django_errors/locale/en/LC_MESSAGES/django.po` & `django-errors-2.3.2/src/django_errors/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/src/django_errors/locale/es/LC_MESSAGES/django.po` & `django-errors-2.3.2/src/django_errors/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/src/django_errors/locale/fr/LC_MESSAGES/django.po` & `django-errors-2.3.2/src/django_errors/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/src/django_errors/locale/it/LC_MESSAGES/django.po` & `django-errors-2.3.2/src/django_errors/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/src/django_errors/locale/ja/LC_MESSAGES/django.po` & `django-errors-2.3.2/src/django_errors/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/src/django_errors/locale/lt/LC_MESSAGES/django.po` & `django-errors-2.3.2/src/django_errors/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/src/django_errors/locale/nl/LC_MESSAGES/django.po` & `django-errors-2.3.2/src/django_errors/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/src/django_errors/locale/ru/LC_MESSAGES/django.po` & `django-errors-2.3.2/src/django_errors/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/src/django_errors/locale/zh_hans/LC_MESSAGES/django.po` & `django-errors-2.3.2/src/django_errors/locale/zh_hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/src/django_errors/locale/zh_hant/LC_MESSAGES/django.po` & `django-errors-2.3.2/src/django_errors/locale/zh_hant/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/src/django_errors/middleware/handler.py` & `django-errors-2.3.2/src/django_errors/middleware/handler.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/src/django_errors/views.py` & `django-errors-2.3.2/src/django_errors/views.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/src/django_errors.egg-info/PKG-INFO` & `django-errors-2.3.2/src/django_errors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-errors
-Version: 2.3.0
+Version: 2.3.2
 Summary: Django application for handling server errors.
 Home-page: https://github.com/DLRSP/django-errors
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,errors
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-errors-2.3.0/src/django_errors.egg-info/SOURCES.txt` & `django-errors-2.3.2/src/django_errors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/tests/settings.py` & `django-errors-2.3.2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/tests/test_errors.py` & `django-errors-2.3.2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/tests/test_errors_exceptions.py` & `django-errors-2.3.2/tests/test_errors_exceptions.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/tests/test_errors_locale_it.py` & `django-errors-2.3.2/tests/test_errors_locale_it.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,16 @@
             response, b"Metodo non consentito (POST)[405]", status_code=405, count=1
         )
         self.assertContains(
             response, b"Metodo non consentito (POST)", status_code=405, count=2
         )
         self.assertContains(
             response,
-            b"Scusa, il metodo usato non \xc3\xa8 consentito per la pagina con questo URL.",
+            b"Scusa, il metodo usato non \xc3\xa8 consentito "
+            b"per la pagina con questo URL.",
             status_code=405,
             count=1,
         )
 
     def test_405_template_post_locale_it(self):
         """Test the url of 405 page."""
         LOGGER.debug("405 Test URLs")
@@ -87,15 +88,16 @@
             response, b"Metodo non consentito (GET)[405]", status_code=405, count=1
         )
         self.assertContains(
             response, b"Metodo non consentito (GET)", status_code=405, count=2
         )
         self.assertContains(
             response,
-            b"Scusa, il metodo usato non \xc3\xa8 consentito per la pagina con questo URL.",
+            b"Scusa, il metodo usato non \xc3\xa8 consentito "
+            b"per la pagina con questo URL.",
             status_code=405,
             count=1,
         )
 
     def test_500_template_locale_it(self):
         """Test the url of 400 page."""
         LOGGER.debug("500 Test URLs")
```

### Comparing `django-errors-2.3.0/tests/test_errors_standard.py` & `django-errors-2.3.2/tests/test_errors_standard.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/tests/test_errors_templates.py` & `django-errors-2.3.2/tests/test_errors_templates.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/tests/test_errors_urls.py` & `django-errors-2.3.2/tests/test_errors_urls.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/tests/urls.py` & `django-errors-2.3.2/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/tests/views.py` & `django-errors-2.3.2/tests/views.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/tests/views_standard.py` & `django-errors-2.3.2/tests/views_standard.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/tests/views_templates.py` & `django-errors-2.3.2/tests/views_templates.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.0/tox.ini` & `django-errors-2.3.2/tox.ini`

 * *Files identical despite different names*

