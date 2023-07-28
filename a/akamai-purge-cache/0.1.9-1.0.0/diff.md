# Comparing `tmp/akamai_purge_cache-0.1.9.tar.gz` & `tmp/akamai_purge_cache-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akamai_purge_cache-0.1.9.tar", max compression
+gzip compressed data, was "akamai_purge_cache-1.0.0.tar", max compression
```

## Comparing `akamai_purge_cache-0.1.9.tar` & `akamai_purge_cache-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rwxr-xr-x   0        0        0     1085 2023-07-26 00:30:10.895312 akamai_purge_cache-0.1.9/README.md
--rwxr-xr-x   0        0        0        0 2023-07-25 14:00:09.217851 akamai_purge_cache-0.1.9/akamai_purge_cache/__init__.py
--rwxr-xr-x   0        0        0      852 2023-07-25 19:52:16.805321 akamai_purge_cache-0.1.9/akamai_purge_cache/purge.py
--rwxr-xr-x   0        0        0      669 2023-07-28 21:30:33.709997 akamai_purge_cache-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1727 1970-01-01 00:00:00.000000 akamai_purge_cache-0.1.9/PKG-INFO
+-rwxr-xr-x   0        0        0     1085 2023-07-26 00:30:10.895312 akamai_purge_cache-1.0.0/README.md
+-rwxr-xr-x   0        0        0        0 2023-07-25 14:00:09.217851 akamai_purge_cache-1.0.0/akamai_purge_cache/__init__.py
+-rwxr-xr-x   0        0        0      852 2023-07-25 19:52:16.805321 akamai_purge_cache-1.0.0/akamai_purge_cache/purge.py
+-rwxr-xr-x   0        0        0      711 2023-07-28 22:16:59.487049 akamai_purge_cache-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1814 1970-01-01 00:00:00.000000 akamai_purge_cache-1.0.0/PKG-INFO
```

### Comparing `akamai_purge_cache-0.1.9/README.md` & `akamai_purge_cache-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `akamai_purge_cache-0.1.9/akamai_purge_cache/purge.py` & `akamai_purge_cache-1.0.0/akamai_purge_cache/purge.py`

 * *Files identical despite different names*

### Comparing `akamai_purge_cache-0.1.9/PKG-INFO` & `akamai_purge_cache-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: akamai-purge-cache
-Version: 0.1.9
+Version: 1.0.0
 Summary: Marriott CDN Team Fastpurge POC script
 Author: Alan Janis
 Author-email: alan.janis@marriott.com
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: awslambdaric (>=2.0.4,<3.0.0)
+Requires-Dist: certifi (>=2023.7.22,<2024.0.0)
 Requires-Dist: click (>=8.1.6,<9.0.0)
 Requires-Dist: edgegrid-python (>=1.3.1,<2.0.0)
 Requires-Dist: fastpurge (>=1.0.4,<2.0.0)
 Requires-Dist: monotonic (>=1.6,<2.0)
 Requires-Dist: more-executors (>=2.11.4,<3.0.0)
+Requires-Dist: urllib3 (>=2.0.4,<3.0.0)
 Description-Content-Type: text/markdown
 
 # akamai-purge-cache : interactive python script
 
 ## Python Script
 
 ```python
```

