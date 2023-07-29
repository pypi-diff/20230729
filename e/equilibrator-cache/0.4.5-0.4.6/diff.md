# Comparing `tmp/equilibrator-cache-0.4.5.tar.gz` & `tmp/equilibrator-cache-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equilibrator-cache-0.4.5.tar", last modified: Fri Jul 28 03:13:20 2023, max compression
+gzip compressed data, was "equilibrator-cache-0.4.6.tar", last modified: Sat Jul 29 14:13:12 2023, max compression
```

## Comparing `equilibrator-cache-0.4.5.tar` & `equilibrator-cache-0.4.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:13:20.559857 equilibrator-cache-0.4.5/
--rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2470 2023-07-28 03:13:20.559857 equilibrator-cache-0.4.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1146 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1978 2023-07-28 03:13:20.560857 equilibrator-cache-0.4.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:13:20.551857 equilibrator-cache-0.4.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:13:20.560857 equilibrator-cache-0.4.5/src/equilibrator_cache/
--rw-rw-rw-   0 root         (0) root         (0)     2033 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-07-28 03:13:20.560857 equilibrator-cache-0.4.5/src/equilibrator_cache/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2398 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/api.py
--rw-rw-rw-   0 root         (0) root         (0)     7328 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/compatibility.py
--rw-rw-rw-   0 root         (0) root         (0)    12786 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/compound_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     1524 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:13:20.559857 equilibrator-cache-0.4.5/src/equilibrator_cache/models/
--rw-rw-rw-   0 root         (0) root         (0)     1905 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11380 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/models/compound.py
--rw-rw-rw-   0 root         (0) root         (0)     3234 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/models/compound_identifier.py
--rw-rw-rw-   0 root         (0) root         (0)     4205 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/models/compound_microspecies.py
--rw-rw-rw-   0 root         (0) root         (0)     2339 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/models/magnesium_dissociation_constant.py
--rw-rw-rw-   0 root         (0) root         (0)     2182 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/models/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     4442 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/models/registry.py
--rw-rw-rw-   0 root         (0) root         (0)    25544 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/reaction.py
--rw-rw-rw-   0 root         (0) root         (0)     4001 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/thermodynamic_constants.py
--rwxrwxrwx   0 root         (0) root         (0)     6665 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/zenodo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:13:20.557857 equilibrator-cache-0.4.5/src/equilibrator_cache.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2470 2023-07-28 03:13:20.000000 equilibrator-cache-0.4.5/src/equilibrator_cache.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-07-28 03:13:20.000000 equilibrator-cache-0.4.5/src/equilibrator_cache.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 03:13:20.000000 equilibrator-cache-0.4.5/src/equilibrator_cache.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      406 2023-07-28 03:13:20.000000 equilibrator-cache-0.4.5/src/equilibrator_cache.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-28 03:13:20.000000 equilibrator-cache-0.4.5/src/equilibrator_cache.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 03:13:20.000000 equilibrator-cache-0.4.5/src/equilibrator_cache.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)    68611 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:13:12.717951 equilibrator-cache-0.4.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-07-29 14:13:12.717951 equilibrator-cache-0.4.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1978 2023-07-29 14:13:12.718951 equilibrator-cache-0.4.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:13:12.710951 equilibrator-cache-0.4.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:13:12.718951 equilibrator-cache-0.4.6/src/equilibrator_cache/
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-07-29 14:13:12.718951 equilibrator-cache-0.4.6/src/equilibrator_cache/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2398 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     7328 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/compatibility.py
+-rw-rw-rw-   0 root         (0) root         (0)    12786 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/compound_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     1524 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:13:12.717951 equilibrator-cache-0.4.6/src/equilibrator_cache/models/
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11380 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/models/compound.py
+-rw-rw-rw-   0 root         (0) root         (0)     3234 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/models/compound_identifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     4205 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/models/compound_microspecies.py
+-rw-rw-rw-   0 root         (0) root         (0)     2339 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/models/magnesium_dissociation_constant.py
+-rw-rw-rw-   0 root         (0) root         (0)     2182 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/models/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     4442 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/models/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    25544 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/reaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4001 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/thermodynamic_constants.py
+-rwxrwxrwx   0 root         (0) root         (0)     6740 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/zenodo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:13:12.715951 equilibrator-cache-0.4.6/src/equilibrator_cache.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-07-29 14:13:12.000000 equilibrator-cache-0.4.6/src/equilibrator_cache.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-29 14:13:12.000000 equilibrator-cache-0.4.6/src/equilibrator_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 14:13:12.000000 equilibrator-cache-0.4.6/src/equilibrator_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      406 2023-07-29 14:13:12.000000 equilibrator-cache-0.4.6/src/equilibrator_cache.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-29 14:13:12.000000 equilibrator-cache-0.4.6/src/equilibrator_cache.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 14:13:12.000000 equilibrator-cache-0.4.6/src/equilibrator_cache.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/versioneer.py
```

### Comparing `equilibrator-cache-0.4.5/LICENSE` & `equilibrator-cache-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.5/PKG-INFO` & `equilibrator-cache-0.4.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-cache
-Version: 0.4.5
+Version: 0.4.6
 Summary: Cache application for compounds, reactions, and enzymes
 Home-page: https://gitlab.com/equilibrator/equilibrator-cache
 Download-URL: https://pypi.org/project/equilibrator-cache/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-cache
@@ -29,15 +29,15 @@
 License-File: LICENSE
 
 equilibrator-cache
 ==================
 
 [![pipeline status](https://gitlab.com/elad.noor/equilibrator-cache/badges/develop/pipeline.svg)](https://gitlab.com/elad.noor/equilibrator-cache/commits/develop)
 
-[![coverage report](https://gitlab.com/elad.noor/equilibrator-cache/badges/develop/coverage.svg)](https://gitlab.com/elad.noor/equilibrator-cache/commits/develop)
+[![codecov](https://codecov.io/gl/equilibrator/equilibrator-cache/branch/develop/graph/badge.svg?token=OxxaCqgaLs)](https://codecov.io/gl/equilibrator/equilibrator-cache)
 
 [![Join the chat at https://gitter.im/equilibrator-devs/equilibrator-api](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/equilibrator-devs/equilibrator-api?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 A database application for caching data used by eQuilibrator and related projects.
 Stored data includes compound names, structures, protonation state information,
 reaction and enzyme info, and cross-references to other databases.
 All compounds stored in equilibrator-cache are cross-referenced using
```

### Comparing `equilibrator-cache-0.4.5/README.md` & `equilibrator-cache-0.4.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 equilibrator-cache
 ==================
 
 [![pipeline status](https://gitlab.com/elad.noor/equilibrator-cache/badges/develop/pipeline.svg)](https://gitlab.com/elad.noor/equilibrator-cache/commits/develop)
 
-[![coverage report](https://gitlab.com/elad.noor/equilibrator-cache/badges/develop/coverage.svg)](https://gitlab.com/elad.noor/equilibrator-cache/commits/develop)
+[![codecov](https://codecov.io/gl/equilibrator/equilibrator-cache/branch/develop/graph/badge.svg?token=OxxaCqgaLs)](https://codecov.io/gl/equilibrator/equilibrator-cache)
 
 [![Join the chat at https://gitter.im/equilibrator-devs/equilibrator-api](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/equilibrator-devs/equilibrator-api?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 A database application for caching data used by eQuilibrator and related projects.
 Stored data includes compound names, structures, protonation state information,
 reaction and enzyme info, and cross-references to other databases.
 All compounds stored in equilibrator-cache are cross-referenced using
```

### Comparing `equilibrator-cache-0.4.5/setup.cfg` & `equilibrator-cache-0.4.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.5/setup.py` & `equilibrator-cache-0.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.5/src/equilibrator_cache/__init__.py` & `equilibrator-cache-0.4.6/src/equilibrator_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.5/src/equilibrator_cache/api.py` & `equilibrator-cache-0.4.6/src/equilibrator_cache/api.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.5/src/equilibrator_cache/compatibility.py` & `equilibrator-cache-0.4.6/src/equilibrator_cache/compatibility.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.5/src/equilibrator_cache/compound_cache.py` & `equilibrator-cache-0.4.6/src/equilibrator_cache/compound_cache.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.5/src/equilibrator_cache/exceptions.py` & `equilibrator-cache-0.4.6/src/equilibrator_cache/exceptions.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.5/src/equilibrator_cache/models/__init__.py` & `equilibrator-cache-0.4.6/src/equilibrator_cache/models/__init__.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.5/src/equilibrator_cache/models/compound.py` & `equilibrator-cache-0.4.6/src/equilibrator_cache/models/compound.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.5/src/equilibrator_cache/models/compound_identifier.py` & `equilibrator-cache-0.4.6/src/equilibrator_cache/models/compound_identifier.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.5/src/equilibrator_cache/models/compound_microspecies.py` & `equilibrator-cache-0.4.6/src/equilibrator_cache/models/compound_microspecies.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.5/src/equilibrator_cache/models/magnesium_dissociation_constant.py` & `equilibrator-cache-0.4.6/src/equilibrator_cache/models/magnesium_dissociation_constant.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.5/src/equilibrator_cache/models/mixins.py` & `equilibrator-cache-0.4.6/src/equilibrator_cache/models/mixins.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.5/src/equilibrator_cache/models/registry.py` & `equilibrator-cache-0.4.6/src/equilibrator_cache/models/registry.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.5/src/equilibrator_cache/reaction.py` & `equilibrator-cache-0.4.6/src/equilibrator_cache/reaction.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.5/src/equilibrator_cache/thermodynamic_constants.py` & `equilibrator-cache-0.4.6/src/equilibrator_cache/thermodynamic_constants.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.5/src/equilibrator_cache/zenodo.py` & `equilibrator-cache-0.4.6/src/equilibrator_cache/zenodo.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,18 @@
     BytesIO
         Bytes buffer of the downloaded file.
 
     """
     data = BytesIO()
     with client.stream("GET", url) as response:
         response.raise_for_status()
-        total = int(response.headers["Content-Length"])
+        try:
+            total = int(response.headers["Content-Length"])
+        except KeyError:
+            total = float("inf")
         md5 = response.headers["content-md5"]
 
         num_bytes = 0
         with tqdm(
             total=total, unit_scale=True, unit_divisor=1024, unit="B"
         ) as progress:
             for chunk in response.iter_bytes():
```

### Comparing `equilibrator-cache-0.4.5/src/equilibrator_cache.egg-info/PKG-INFO` & `equilibrator-cache-0.4.6/src/equilibrator_cache.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-cache
-Version: 0.4.5
+Version: 0.4.6
 Summary: Cache application for compounds, reactions, and enzymes
 Home-page: https://gitlab.com/equilibrator/equilibrator-cache
 Download-URL: https://pypi.org/project/equilibrator-cache/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-cache
@@ -29,15 +29,15 @@
 License-File: LICENSE
 
 equilibrator-cache
 ==================
 
 [![pipeline status](https://gitlab.com/elad.noor/equilibrator-cache/badges/develop/pipeline.svg)](https://gitlab.com/elad.noor/equilibrator-cache/commits/develop)
 
-[![coverage report](https://gitlab.com/elad.noor/equilibrator-cache/badges/develop/coverage.svg)](https://gitlab.com/elad.noor/equilibrator-cache/commits/develop)
+[![codecov](https://codecov.io/gl/equilibrator/equilibrator-cache/branch/develop/graph/badge.svg?token=OxxaCqgaLs)](https://codecov.io/gl/equilibrator/equilibrator-cache)
 
 [![Join the chat at https://gitter.im/equilibrator-devs/equilibrator-api](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/equilibrator-devs/equilibrator-api?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 A database application for caching data used by eQuilibrator and related projects.
 Stored data includes compound names, structures, protonation state information,
 reaction and enzyme info, and cross-references to other databases.
 All compounds stored in equilibrator-cache are cross-referenced using
```

### Comparing `equilibrator-cache-0.4.5/src/equilibrator_cache.egg-info/SOURCES.txt` & `equilibrator-cache-0.4.6/src/equilibrator_cache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.5/versioneer.py` & `equilibrator-cache-0.4.6/versioneer.py`

 * *Files identical despite different names*

