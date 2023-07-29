# Comparing `tmp/pretix-sumup-1.0.2.tar.gz` & `tmp/pretix-sumup-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-sumup-1.0.2.tar", last modified: Sat Jul 22 09:41:41 2023, max compression
+gzip compressed data, was "pretix-sumup-1.0.3.tar", last modified: Sat Jul 29 18:27:35 2023, max compression
```

## Comparing `pretix-sumup-1.0.2.tar` & `pretix-sumup-1.0.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    33886 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-07-22 09:41:41.385984 pretix-sumup-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.377984 pretix-sumup-1.0.2/pretix_sumup/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.373984 pretix-sumup-1.0.2/pretix_sumup/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/locale/de_Informal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/locale/de_Informal/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/locale/django.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.373984 pretix-sumup-1.0.2/pretix_sumup/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.373984 pretix-sumup-1.0.2/pretix_sumup/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.373984 pretix-sumup-1.0.2/pretix_sumup/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.373984 pretix-sumup-1.0.2/pretix_sumup/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/static/pretix_sumup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/static/pretix_sumup/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.377984 pretix-sumup-1.0.2/pretix_sumup/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/checkout_confirm_render.html
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/control.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/email/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/email/order_pending.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/not_available.html
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/pending.html
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/prepare.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-07-22 09:41:41.000000 pretix-sumup-1.0.2/pretix_sumup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-22 09:41:41.000000 pretix-sumup-1.0.2/pretix_sumup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 09:41:41.000000 pretix-sumup-1.0.2/pretix_sumup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-22 09:41:41.000000 pretix-sumup-1.0.2/pretix_sumup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-22 09:41:41.000000 pretix-sumup-1.0.2/pretix_sumup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-22 09:41:41.385984 pretix-sumup-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.996590 pretix-sumup-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    33886 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-07-29 18:27:34.996590 pretix-sumup-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.992589 pretix-sumup-1.0.3/pretix_sumup/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.992589 pretix-sumup-1.0.3/pretix_sumup/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.988589 pretix-sumup-1.0.3/pretix_sumup/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.992589 pretix-sumup-1.0.3/pretix_sumup/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.992589 pretix-sumup-1.0.3/pretix_sumup/locale/de_Informal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.992589 pretix-sumup-1.0.3/pretix_sumup/locale/de_Informal/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/locale/django.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.988589 pretix-sumup-1.0.3/pretix_sumup/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.992589 pretix-sumup-1.0.3/pretix_sumup/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.992589 pretix-sumup-1.0.3/pretix_sumup/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.992589 pretix-sumup-1.0.3/pretix_sumup/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.992589 pretix-sumup-1.0.3/pretix_sumup/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.992589 pretix-sumup-1.0.3/pretix_sumup/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.992589 pretix-sumup-1.0.3/pretix_sumup/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.992589 pretix-sumup-1.0.3/pretix_sumup/static/pretix_sumup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/static/pretix_sumup/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.992589 pretix-sumup-1.0.3/pretix_sumup/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.996590 pretix-sumup-1.0.3/pretix_sumup/templates/pretix_sumup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/templates/pretix_sumup/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/templates/pretix_sumup/checkout_confirm_render.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/templates/pretix_sumup/control.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.996590 pretix-sumup-1.0.3/pretix_sumup/templates/pretix_sumup/email/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/templates/pretix_sumup/email/order_pending.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/templates/pretix_sumup/not_available.html
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/templates/pretix_sumup/pending.html
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pretix_sumup/templates/pretix_sumup/prepare.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.992589 pretix-sumup-1.0.3/pretix_sumup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-07-29 18:27:34.000000 pretix-sumup-1.0.3/pretix_sumup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-29 18:27:34.000000 pretix-sumup-1.0.3/pretix_sumup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 18:27:34.000000 pretix-sumup-1.0.3/pretix_sumup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-29 18:27:34.000000 pretix-sumup-1.0.3/pretix_sumup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-29 18:27:34.000000 pretix-sumup-1.0.3/pretix_sumup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-29 18:27:34.996590 pretix-sumup-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:27:34.996590 pretix-sumup-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-29 18:26:12.000000 pretix-sumup-1.0.3/tests/test_main.py
```

### Comparing `pretix-sumup-1.0.2/LICENSE` & `pretix-sumup-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.2/PKG-INFO` & `pretix-sumup-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-sumup
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sumup plugin
 Author-email: Ronan Le Meillat <ronan@highcanfly.club>
 Maintainer-email: Ronan Le Meillat <ronan@highcanfly.club>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
         Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `pretix-sumup-1.0.2/README.md` & `pretix-sumup-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.2/pretix_sumup/apps.py` & `pretix-sumup-1.0.3/pretix_sumup/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.2/pretix_sumup/locale/de/LC_MESSAGES/django.po` & `pretix-sumup-1.0.3/pretix_sumup/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.2/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-sumup-1.0.3/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.2/pretix_sumup/locale/django.pot` & `pretix-sumup-1.0.3/pretix_sumup/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.2/pretix_sumup/locale/es/LC_MESSAGES/django.po` & `pretix-sumup-1.0.3/pretix_sumup/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.2/pretix_sumup/locale/fr/LC_MESSAGES/django.po` & `pretix-sumup-1.0.3/pretix_sumup/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.2/pretix_sumup/locale/it/LC_MESSAGES/django.po` & `pretix-sumup-1.0.3/pretix_sumup/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.2/pretix_sumup/payment.py` & `pretix-sumup-1.0.3/pretix_sumup/payment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,35 @@
+from decimal import Decimal
 import json
 import requests
 import sys
 import uuid
 from collections import OrderedDict
 from django import forms
 from django.http import HttpRequest
 from django.template.loader import get_template
 from django.utils.crypto import get_random_string
 from django.utils.translation import get_language, gettext_lazy as _, to_locale
 from i18nfield.strings import LazyI18nString
-from pretix.base.models import OrderPayment
+from pretix.base.models import InvoiceAddress, Order, OrderPayment
 from pretix.base.payment import BasePaymentProvider
+from pretix.presale.views.cart import cart_session
 
 
 def getNonce(request):
     if "_sumup_nonce" not in request.session:
         request.session["_sumup_nonce"] = get_random_string(32)
     return request.session["_sumup_nonce"]
 
 
 class SumupPayment(BasePaymentProvider):
     identifier = "sumuppayment"
     verbose_name = _("Sumup Payment")
     abort_pending_allowed = True
+    ia = InvoiceAddress()
 
     @property
     def test_mode_message(self):
         return _(
             "In test mode, you can just manually mark this order as paid in the backend after it has been "
             "created."
         )
@@ -127,34 +130,51 @@
             file=sys.stderr,
         )
         if sumupResponse["status"] == "PAID":
             return True
         else:
             return False
 
-    def payment_form_render(self, request) -> str:
+    def payment_form_render(self, request: HttpRequest, total: Decimal, order: Order = None) -> str:
+        def get_invoice_address():
+            if order and getattr(order, 'invoice_address', None):
+                request._checkout_flow_invoice_address = order.invoice_address
+            if not hasattr(request, '_checkout_flow_invoice_address'):
+                cs = cart_session(request)
+                iapk = cs.get('invoice_address')
+                if not iapk:
+                    request._checkout_flow_invoice_address = InvoiceAddress()
+                else:
+                    try:
+                        request._checkout_flow_invoice_address = InvoiceAddress.objects.get(pk=iapk, order__isnull=True)
+                    except InvoiceAddress.DoesNotExist:
+                        request._checkout_flow_invoice_address = InvoiceAddress()
+            return request._checkout_flow_invoice_address
+        
         print("SumupPayment.payment_form_render", file=sys.stderr)
+        self.ia = get_invoice_address()
         ctx = {}
         template = get_template("pretix_sumup/prepare.html")
         return template.render(ctx)
 
     def checkout_prepare(self, request, cart):
         print("SumupPayment.checkout_prepare", file=sys.stderr)
         client_id = self.settings.get("client_id")
         secret = self.settings.get("secret")
         sumupid = self.settings.get("sumupid")
         sumupToken = self.sumup_get_token(client_id, secret)
+        cs = cart_session(request)
         if isinstance(sumupToken, str):
             sumupCheckoutResponse = self.sumup_create_checkout(
                 sumupToken,
                 sumupid,
                 str(cart["total"]),
-                "none@example.com",
-                "none",
-                "example",
+                cs["email"],
+                self.ia.name_parts["given_name"] if "given_name" in self.ia.name_parts else "John",
+                self.ia.name_parts["family_name"] if "family_name" in self.ia.name_parts else "Doe",
             )
             if sumupCheckoutResponse.status_code == 201:
                 print(
                     "SumupPayment.checkout_prepare OK: "
                     + str(sumupCheckoutResponse.content),
                     file=sys.stderr,
                 )
```

### Comparing `pretix-sumup-1.0.2/pretix_sumup/signals.py` & `pretix-sumup-1.0.3/pretix_sumup/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.2/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg` & `pretix-sumup-1.0.3/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html` & `pretix-sumup-1.0.3/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/control.html` & `pretix-sumup-1.0.3/pretix_sumup/templates/pretix_sumup/control.html`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.2/pretix_sumup.egg-info/PKG-INFO` & `pretix-sumup-1.0.3/pretix_sumup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-sumup
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sumup plugin
 Author-email: Ronan Le Meillat <ronan@highcanfly.club>
 Maintainer-email: Ronan Le Meillat <ronan@highcanfly.club>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
         Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `pretix-sumup-1.0.2/pretix_sumup.egg-info/SOURCES.txt` & `pretix-sumup-1.0.3/pretix_sumup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.2/pyproject.toml` & `pretix-sumup-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.2/setup.cfg` & `pretix-sumup-1.0.3/setup.cfg`

 * *Files identical despite different names*

