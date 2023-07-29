# Comparing `tmp/hyundai_kia_connect_api-3.3.9.tar.gz` & `tmp/hyundai_kia_connect_api-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyundai_kia_connect_api-3.3.9.tar", last modified: Mon Jul  3 13:39:50 2023, max compression
+gzip compressed data, was "hyundai_kia_connect_api-3.4.0.tar", last modified: Sat Jul 29 15:54:43 2023, max compression
```

## Comparing `hyundai_kia_connect_api-3.3.9.tar` & `hyundai_kia_connect_api-3.4.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:39:50.023350 hyundai_kia_connect_api-3.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-03 13:39:50.023350 hyundai_kia_connect_api-3.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:39:50.023350 hyundai_kia_connect_api-3.3.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:39:50.023350 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/ApiImpl.py
--rw-r--r--   0 runner    (1001) docker     (123)    23880 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/KiaUvoAPIUSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    29985 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/KiaUvoApiCA.py
--rw-r--r--   0 runner    (1001) docker     (123)    51311 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/KiaUvoApiCN.py
--rw-r--r--   0 runner    (1001) docker     (123)    53964 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/KiaUvoApiEU.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/Vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/VehicleManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:39:50.023350 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-03 13:39:50.000000 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-03 13:39:50.000000 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:39:50.000000 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:39:49.000000 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 13:39:50.000000 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 13:39:50.000000 hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-03 13:39:50.023350 hyundai_kia_connect_api-3.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-03 13:39:38.000000 hyundai_kia_connect_api-3.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:39:50.023350 hyundai_kia_connect_api-3.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/tests/ca_login_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/tests/eu_check_response_for_errors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-03 13:39:12.000000 hyundai_kia_connect_api-3.3.9/tests/eu_login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:54:43.385278 hyundai_kia_connect_api-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-29 15:54:43.385278 hyundai_kia_connect_api-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:54:43.381278 hyundai_kia_connect_api-3.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:54:43.385278 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/ApiImpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23950 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/KiaUvoAPIUSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29985 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/KiaUvoApiCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51311 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/KiaUvoApiCN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54198 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/KiaUvoApiEU.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/Vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/VehicleManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:54:43.385278 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-29 15:54:43.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-29 15:54:43.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 15:54:43.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 15:54:43.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 15:54:43.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 15:54:43.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-29 15:54:43.385278 hyundai_kia_connect_api-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-29 15:54:29.000000 hyundai_kia_connect_api-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:54:43.385278 hyundai_kia_connect_api-3.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/tests/ca_login_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/tests/eu_check_response_for_errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/tests/eu_login_test.py
```

### Comparing `hyundai_kia_connect_api-3.3.9/CONTRIBUTING.rst` & `hyundai_kia_connect_api-3.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.9/LICENSE` & `hyundai_kia_connect_api-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.9/PKG-INFO` & `hyundai_kia_connect_api-3.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyundai_kia_connect_api
-Version: 3.3.9
+Version: 3.4.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/fuatakgun/hyundai_kia_connect_api
 Author: Fuat Akgun
 Author-email: fuatakgun@gmail.com
 License: MIT license
 Keywords: hyundai_kia_connect_api
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -81,14 +81,15 @@
 
 The Bluelink App is reset to English for users who have set another language in the Bluelink App in Europe when using hyundai_kia_connect_api.
 To avoid this, you can pass the optional parameter language (default is "en") to the constructor of VehicleManager, e.g. for Dutch::
 
     vm = VehicleManager(region=2, brand=1, username="username@gmail.com", password="password", pin="1234", language="nl")
 
 Note: this is only implemented for Europe currently.
+
 For a list of language codes, see here: https://www.science.co.il/language/Codes.php. Currently in Europe the Bluelink App shows the following languages::
 
 - "en" English
 - "de" German
 - "fr" French
 - "it" Italian
 - "es" Spanish
```

### Comparing `hyundai_kia_connect_api-3.3.9/README.rst` & `hyundai_kia_connect_api-3.4.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 
 The Bluelink App is reset to English for users who have set another language in the Bluelink App in Europe when using hyundai_kia_connect_api.
 To avoid this, you can pass the optional parameter language (default is "en") to the constructor of VehicleManager, e.g. for Dutch::
 
     vm = VehicleManager(region=2, brand=1, username="username@gmail.com", password="password", pin="1234", language="nl")
 
 Note: this is only implemented for Europe currently.
+
 For a list of language codes, see here: https://www.science.co.il/language/Codes.php. Currently in Europe the Bluelink App shows the following languages::
 
 - "en" English
 - "de" German
 - "fr" French
 - "it" Italian
 - "es" Spanish
```

### Comparing `hyundai_kia_connect_api-3.3.9/docs/Makefile` & `hyundai_kia_connect_api-3.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.9/docs/conf.py` & `hyundai_kia_connect_api-3.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.9/docs/installation.rst` & `hyundai_kia_connect_api-3.4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.9/docs/make.bat` & `hyundai_kia_connect_api-3.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/ApiImpl.py` & `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/ApiImpl.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py` & `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,22 +28,28 @@
 
 
 class cipherAdapter(HTTPAdapter):
     """
     A HTTPAdapter that re-enables poor ciphers required by Hyundai.
     """
 
-    def init_poolmanager(self, *args, **kwargs):
+    def _setup_ssl_context(self):
         context = create_urllib3_context(ciphers=CIPHERS)
-        kwargs["ssl_context"] = context
+        context.options |= 0x4
+
+        return context
+
+    def init_poolmanager(self, *args, **kwargs):
+        kwargs["ssl_context"] = self._setup_ssl_context()
+
         return super().init_poolmanager(*args, **kwargs)
 
     def proxy_manager_for(self, *args, **kwargs):
-        context = create_urllib3_context(ciphers=CIPHERS)
-        kwargs["ssl_context"] = context
+        kwargs["ssl_context"] = self._setup_ssl_context()
+
         return super().proxy_manager_for(*args, **kwargs)
 
 
 class HyundaiBlueLinkAPIUSA(ApiImpl):
     """HyundaiBlueLinkAPIUSA"""
 
     # initialize with a timestamp which will allow the first fetch to occur
```

### Comparing `hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/KiaUvoAPIUSA.py` & `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/KiaUvoAPIUSA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/KiaUvoApiCA.py` & `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/KiaUvoApiCA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/KiaUvoApiCN.py` & `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/KiaUvoApiCN.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/KiaUvoApiEU.py` & `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/KiaUvoApiEU.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """KiaUvoApiEU.py"""
 # pylint:disable=missing-timeout,missing-class-docstring,missing-function-docstring,wildcard-import,unused-wildcard-import,invalid-name,logging-fstring-interpolation,broad-except,bare-except,super-init-not-called,unused-argument,line-too-long,too-many-lines
 
+import base64
 import random
 import datetime as dt
 import logging
 import re
 import uuid
 from time import sleep
 from urllib.parse import parse_qs, urlparse
 
 import pytz
 import requests
 from bs4 import BeautifulSoup
-from dateutil import tz, parser
+from dateutil import tz
 
 from .ApiImpl import (
     ApiImpl,
     ClimateRequestOptions,
 )
 from .Token import Token
 from .Vehicle import (
@@ -78,24 +79,27 @@
     Checks for errors in the API response.
     If an error is found, an exception is raised.
     retCode known values:
     - S: success
     - F: failure
     resCode / resMsg known values:
     - 0000: no error
+    - 4002:  "Invalid request body - invalid deviceId",
+             relogin will resolve but a bandaid.
     - 4004: "Duplicate request"
     - 4081: "Request timeout"
     - 5031: "Unavailable remote control - Service Temporary Unavailable"
     - 5091: "Exceeds number of requests"
     - 5921: "No Data Found v2 - No Data Found v2"
     - 9999: "Undefined Error - Response timeout"
     :param response: the API's JSON response
     """
 
     error_code_mapping = {
+        "4002": DeviceIDError,
         "4004": DuplicateRequestError,
         "4081": RequestTimeoutError,
         "5031": ServiceTemporaryUnavailable,
         "5091": RateLimitingError,
         "5921": NoDataFound,
         "9999": RequestTimeoutError,
     }
@@ -104,66 +108,71 @@
         _LOGGER.error(f"Unknown API response format: {response}")
         raise InvalidAPIResponseError()
 
     if response["retCode"] == "F":
         if response["resCode"] in error_code_mapping:
             raise error_code_mapping[response["resCode"]](response["resMsg"])
         else:
-            raise APIError(f"Server returned: '{response['resMsg']}'")
+            raise APIError(
+                f"Server returned:  '{response['rescode']}' '{response['resMsg']}'"
+            )
 
 
 class KiaUvoApiEU(ApiImpl):
     data_timezone = tz.gettz("Europe/Berlin")
     temperature_range = [x * 0.5 for x in range(28, 60)]
 
     def __init__(self, region: int, brand: int, language: str) -> None:
         self.stamps = None
 
         if language not in SUPPORTED_LANGUAGES_LIST:
             _LOGGER.warning(f"Unsupported language: {language}, fallback to en")
             language = "en"  # fallback to English
         self.LANGUAGE: str = language
+        self.brand: int = brand
 
-        if BRANDS[brand] == BRAND_KIA:
+        if BRANDS[self.brand] == BRAND_KIA:
             self.BASE_DOMAIN: str = "prd.eu-ccapi.kia.com"
             self.CCSP_SERVICE_ID: str = "fdc85c00-0a2f-4c64-bcb4-2cfb1500730a"
-            self.APP_ID: str = "e7bcd186-a5fd-410d-92cb-6876a42288bd"
+            self.APP_ID: str = "a2b8469b-30a3-4361-8e13-6fceea8fbe74"
             self.BASIC_AUTHORIZATION: str = (
                 "Basic ZmRjODVjMDAtMGEyZi00YzY0LWJjYjQtMmNmYjE1MDA3MzBhOnNlY3JldA=="
             )
             self.LOGIN_FORM_HOST = "eu-account.kia.com"
-        elif BRANDS[brand] == BRAND_HYUNDAI:
+            self.PUSH_TYPE = "APNS"
+        elif BRANDS[self.brand] == BRAND_HYUNDAI:
             self.BASE_DOMAIN: str = "prd.eu-ccapi.hyundai.com"
             self.CCSP_SERVICE_ID: str = "6d477c38-3ca4-4cf3-9557-2a1929a94654"
             self.APP_ID: str = "014d2225-8495-4735-812d-2616334fd15d"
             self.BASIC_AUTHORIZATION: str = "Basic NmQ0NzdjMzgtM2NhNC00Y2YzLTk1NTctMmExOTI5YTk0NjU0OktVeTQ5WHhQekxwTHVvSzB4aEJDNzdXNlZYaG10UVI5aVFobUlGampvWTRJcHhzVg=="  # noqa
             self.LOGIN_FORM_HOST = "eu-account.hyundai.com"
+            self.PUSH_TYPE = "GCM"
 
         self.BASE_URL: str = self.BASE_DOMAIN + ":8080"
         self.USER_API_URL: str = "https://" + self.BASE_URL + "/api/v1/user/"
         self.SPA_API_URL: str = "https://" + self.BASE_URL + "/api/v1/spa/"
         self.SPA_API_URL_V2: str = "https://" + self.BASE_URL + "/api/v2/spa/"
 
         self.CLIENT_ID: str = self.CCSP_SERVICE_ID
         self.GCM_SENDER_ID = 199360397125
 
-        if BRANDS[brand] == BRAND_KIA:
+        if BRANDS[self.brand] == BRAND_KIA:
             auth_client_id = "572e0304-5f8d-4b4c-9dd5-41aa84eed160"
             self.LOGIN_FORM_URL: str = (
                 "https://"
                 + self.LOGIN_FORM_HOST
                 + "/auth/realms/eukiaidm/protocol/openid-connect/auth?client_id="
                 + auth_client_id
                 + "&scope=openid%20profile%20email%20phone&response_type=code&hkid_session_reset=true&redirect_uri="  # noqa
                 + self.USER_API_URL
                 + "integration/redirect/login&ui_locales="
                 + self.LANGUAGE
                 + "&state=$service_id:$user_id"
             )
-        elif BRANDS[brand] == BRAND_HYUNDAI:
+        elif BRANDS[self.brand] == BRAND_HYUNDAI:
             auth_client_id = "64621b96-0f0d-11ec-82a8-0242ac130003"
             self.LOGIN_FORM_URL: str = (
                 "https://"
                 + self.LOGIN_FORM_HOST
                 + "/auth/realms/euhyundaiidm/protocol/openid-connect/auth?client_id="
                 + auth_client_id
                 + "&scope=openid%20profile%20email%20phone&response_type=code&hkid_session_reset=true&redirect_uri="  # noqa
@@ -171,15 +180,15 @@
                 + "integration/redirect/login&ui_locales="
                 + self.LANGUAGE
                 + "&state=$service_id:$user_id"
             )
 
         self.stamps_url: str = (
             "https://raw.githubusercontent.com/neoPix/bluelinky-stamps/master/"
-            + BRANDS[brand].lower()
+            + BRANDS[self.brand].lower()
             + "-"
             + self.APP_ID
             + ".v2.json"
         )
 
     def _get_authenticated_headers(self, token: Token) -> dict:
         return {
@@ -1056,59 +1065,55 @@
             url, json=body, headers=self._get_authenticated_headers(token)
         ).json()
         _LOGGER.debug(f"{DOMAIN} - Set Charge Limits Response: {response}")
         _check_response_for_errors(response)
         return response["msgId"]
 
     def _get_stamp(self) -> str:
-        if self.stamps is None:
-            self.stamps = requests.get(self.stamps_url).json()
-
-        frequency = self.stamps["frequency"]
-        generated_at = parser.isoparse(self.stamps["generated"])
-        position = int(
-            (dt.datetime.now(pytz.utc) - generated_at).total_seconds()
-            * 1000.0
-            / frequency
-        )
-        stamp_count = len(self.stamps["stamps"])
-        _LOGGER.debug(
-            f"{DOMAIN} - get_stamp {generated_at} {frequency} {position} {stamp_count} {((dt.datetime.now(pytz.utc) - generated_at).total_seconds() * 1000.0) / frequency}"  # noqa
-        )
-        if (position * 100.0) / stamp_count > 90:
-            self.stamps = None
-            return self._get_stamp()
+        if BRANDS[self.brand] == BRAND_KIA:
+            cfb = base64.b64decode(
+                "wLTVxwidmH8CfJYBWSnHD6E0huk0ozdiuygB4hLkM5XCgzAL1Dk5sE36d/bx5PFMbZs="
+            )
+        elif BRANDS[self.brand] == BRAND_HYUNDAI:
+            cfb = base64.b64decode(
+                "RFtoRq/vDXJmRndoZaZQyfOot7OrIqGVFj96iY2WL3yyH5Z/pUvlUhqmCxD2t+D65SQ="
+            )
         else:
-            return self.stamps["stamps"][position]
+            raise ValueError("Invalid brand")
+        raw_data = f"{self.APP_ID}:{int(dt.datetime.now().timestamp())}".encode()
+        result = bytes(b1 ^ b2 for b1, b2 in zip(cfb, raw_data))
+        return base64.b64encode(result).decode("utf-8")
 
     def _get_device_id(self, stamp: str):
-        my_hex = "%064x" % random.randrange(10**80)
+        my_hex = "%064x" % random.randrange(  # pylint: disable=consider-using-f-string
+            10**80
+        )
         registration_id = my_hex[:64]
         url = self.SPA_API_URL + "notifications/register"
         payload = {
             "pushRegId": registration_id,
-            "pushType": "APNS",
+            "pushType": self.PUSH_TYPE,
             "uuid": str(uuid.uuid4()),
         }
 
         headers = {
             "ccsp-service-id": self.CCSP_SERVICE_ID,
             "ccsp-application-id": self.APP_ID,
             "Stamp": stamp,
             "Content-Type": "application/json;charset=UTF-8",
             "Host": self.BASE_URL,
             "Connection": "Keep-Alive",
             "Accept-Encoding": "gzip",
             "User-Agent": USER_AGENT_OK_HTTP,
         }
 
+        _LOGGER.debug(f"{DOMAIN} - Get Device ID request: {url} {headers} {payload}")
         response = requests.post(url, headers=headers, json=payload)
         response = response.json()
         _check_response_for_errors(response)
-        _LOGGER.debug(f"{DOMAIN} - Get Device ID request: {headers} {payload}")
         _LOGGER.debug(f"{DOMAIN} - Get Device ID response: {response}")
 
         device_id = response["resMsg"]["deviceId"]
         return device_id
 
     def _get_cookies(self) -> dict:
         # Get Cookies #
```

### Comparing `hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/Vehicle.py` & `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/Vehicle.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/VehicleManager.py` & `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/VehicleManager.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/const.py` & `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/const.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/exceptions.py` & `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,22 @@
     """
     Raised upon receipt of an authentication error.
     """
 
     pass
 
 
+class DeviceIDError(AuthenticationError):
+    """
+    Raised upon receipt of an Invalid Device ID error.
+    """
+
+    pass
+
+
 class APIError(HyundaiKiaException):
     """
     Generic API error
     """
 
     pass
```

### Comparing `hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api/utils.py` & `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/utils.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api.egg-info/PKG-INFO` & `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyundai-kia-connect-api
-Version: 3.3.9
+Version: 3.4.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/fuatakgun/hyundai_kia_connect_api
 Author: Fuat Akgun
 Author-email: fuatakgun@gmail.com
 License: MIT license
 Keywords: hyundai_kia_connect_api
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -81,14 +81,15 @@
 
 The Bluelink App is reset to English for users who have set another language in the Bluelink App in Europe when using hyundai_kia_connect_api.
 To avoid this, you can pass the optional parameter language (default is "en") to the constructor of VehicleManager, e.g. for Dutch::
 
     vm = VehicleManager(region=2, brand=1, username="username@gmail.com", password="password", pin="1234", language="nl")
 
 Note: this is only implemented for Europe currently.
+
 For a list of language codes, see here: https://www.science.co.il/language/Codes.php. Currently in Europe the Bluelink App shows the following languages::
 
 - "en" English
 - "de" German
 - "fr" French
 - "it" Italian
 - "es" Spanish
```

### Comparing `hyundai_kia_connect_api-3.3.9/hyundai_kia_connect_api.egg-info/SOURCES.txt` & `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.9/setup.py` & `hyundai_kia_connect_api-3.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     name="hyundai_kia_connect_api",
     packages=find_packages(
         include=["hyundai_kia_connect_api", "hyundai_kia_connect_api.*"]
     ),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/fuatakgun/hyundai_kia_connect_api",
-    version="3.3.9",
+    version="3.4.0",
     zip_safe=False,
 )
```

### Comparing `hyundai_kia_connect_api-3.3.9/tests/ca_login_test.py` & `hyundai_kia_connect_api-3.4.0/tests/ca_login_test.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.9/tests/eu_check_response_for_errors_test.py` & `hyundai_kia_connect_api-3.4.0/tests/eu_check_response_for_errors_test.py`

 * *Files identical despite different names*

