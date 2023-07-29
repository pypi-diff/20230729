# Comparing `tmp/dockerfile-3.2.0.tar.gz` & `tmp/dockerfile-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockerfile-3.2.0.tar", last modified: Sun Sep 12 20:09:16 2021, max compression
+gzip compressed data, was "dockerfile-3.3.0.tar", last modified: Sat Jul 29 20:20:41 2023, max compression
```

## Comparing `dockerfile-3.2.0.tar` & `dockerfile-3.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2021-09-12 20:09:16.855506 dockerfile-3.2.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2021-09-12 19:21:29.000000 dockerfile-3.2.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)       39 2021-09-12 20:08:53.000000 dockerfile-3.2.0/MANIFEST.in
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3646 2021-09-12 20:09:16.855506 dockerfile-3.2.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2777 2021-09-12 19:21:29.000000 dockerfile-3.2.0/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2021-09-12 20:09:16.855506 dockerfile-3.2.0/dockerfile.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3646 2021-09-12 20:09:16.000000 dockerfile-3.2.0/dockerfile.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      244 2021-09-12 20:09:16.000000 dockerfile-3.2.0/dockerfile.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2021-09-12 20:09:16.000000 dockerfile-3.2.0/dockerfile.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       11 2021-09-12 20:09:16.000000 dockerfile-3.2.0/dockerfile.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)      129 2021-09-12 20:08:53.000000 dockerfile-3.2.0/go.mod
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2321 2021-09-12 19:21:29.000000 dockerfile-3.2.0/parse.go
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2657 2021-09-12 20:08:53.000000 dockerfile-3.2.0/parse_test.go
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2021-09-12 20:09:16.855506 dockerfile-3.2.0/pylib/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3819 2021-09-12 19:21:29.000000 dockerfile-3.2.0/pylib/main.go
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2370 2021-09-12 19:21:29.000000 dockerfile-3.2.0/pylib/support.c
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1234 2021-09-12 20:09:16.855506 dockerfile-3.2.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)      824 2021-09-12 20:08:53.000000 dockerfile-3.2.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 20:20:41.039392 dockerfile-3.3.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-07-29 20:05:50.000000 dockerfile-3.3.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       39 2023-07-29 20:05:50.000000 dockerfile-3.3.0/MANIFEST.in
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3229 2023-07-29 20:20:41.039392 dockerfile-3.3.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2582 2023-07-29 20:05:50.000000 dockerfile-3.3.0/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 20:20:41.039392 dockerfile-3.3.0/dockerfile.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3229 2023-07-29 20:20:40.000000 dockerfile-3.3.0/dockerfile.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      244 2023-07-29 20:20:41.000000 dockerfile-3.3.0/dockerfile.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-07-29 20:20:40.000000 dockerfile-3.3.0/dockerfile.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       11 2023-07-29 20:20:40.000000 dockerfile-3.3.0/dockerfile.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      129 2023-07-29 20:05:50.000000 dockerfile-3.3.0/go.mod
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2321 2023-07-29 20:05:50.000000 dockerfile-3.3.0/parse.go
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2657 2023-07-29 20:05:50.000000 dockerfile-3.3.0/parse_test.go
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 20:20:41.039392 dockerfile-3.3.0/pylib/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3819 2023-07-29 20:05:50.000000 dockerfile-3.3.0/pylib/main.go
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2370 2023-07-29 20:05:50.000000 dockerfile-3.3.0/pylib/support.c
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1049 2023-07-29 20:20:41.039392 dockerfile-3.3.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      860 2023-07-29 20:05:50.000000 dockerfile-3.3.0/setup.py
```

### Comparing `dockerfile-3.2.0/LICENSE` & `dockerfile-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dockerfile-3.2.0/PKG-INFO` & `dockerfile-3.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 Metadata-Version: 2.1
 Name: dockerfile
-Version: 3.2.0
+Version: 3.3.0
 Summary: Parse a dockerfile into a high-level representation using the official go parser.
 Home-page: https://github.com/asottile/dockerfile
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.1
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://asottile.visualstudio.com/asottile/_apis/build/status/asottile.dockerfile?branchName=master)](https://asottile.visualstudio.com/asottile/_build/latest?definitionId=14&branchName=master)
-[![Build status](https://ci.appveyor.com/api/projects/status/l5kj12ysd49xul1l?svg=true)](https://ci.appveyor.com/project/asottile/dockerfile)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/dockerfile/master.svg)](https://results.pre-commit.ci/latest/github/asottile/dockerfile/master)
+[![build status](https://github.com/asottile/dockerfile/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/dockerfile/actions/workflows/main.yml)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/dockerfile/main.svg)](https://results.pre-commit.ci/latest/github/asottile/dockerfile/main)
 
 dockerfile
 ==========
 
 The goal of this repository is to provide a wrapper around
 [docker/docker](https://github.com/docker/docker)'s parser for dockerfiles.
 
@@ -96,9 +90,7 @@
 ```
 go get github.com/asottile/dockerfile
 ```
 
 ### Usage
 
 [godoc](https://godoc.org/github.com/asottile/dockerfile)
-
-
```

### Comparing `dockerfile-3.2.0/README.md` & `dockerfile-3.3.0/dockerfile.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,26 @@
-[![Build Status](https://asottile.visualstudio.com/asottile/_apis/build/status/asottile.dockerfile?branchName=master)](https://asottile.visualstudio.com/asottile/_build/latest?definitionId=14&branchName=master)
-[![Build status](https://ci.appveyor.com/api/projects/status/l5kj12ysd49xul1l?svg=true)](https://ci.appveyor.com/project/asottile/dockerfile)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/dockerfile/master.svg)](https://results.pre-commit.ci/latest/github/asottile/dockerfile/master)
+Metadata-Version: 2.1
+Name: dockerfile
+Version: 3.3.0
+Summary: Parse a dockerfile into a high-level representation using the official go parser.
+Home-page: https://github.com/asottile/dockerfile
+Author: Anthony Sottile
+Author-email: asottile@umich.edu
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![build status](https://github.com/asottile/dockerfile/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/dockerfile/actions/workflows/main.yml)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/dockerfile/main.svg)](https://results.pre-commit.ci/latest/github/asottile/dockerfile/main)
 
 dockerfile
 ==========
 
 The goal of this repository is to provide a wrapper around
 [docker/docker](https://github.com/docker/docker)'s parser for dockerfiles.
```

### Comparing `dockerfile-3.2.0/parse.go` & `dockerfile-3.3.0/parse.go`

 * *Files identical despite different names*

### Comparing `dockerfile-3.2.0/parse_test.go` & `dockerfile-3.3.0/parse_test.go`

 * *Files identical despite different names*

### Comparing `dockerfile-3.2.0/pylib/main.go` & `dockerfile-3.3.0/pylib/main.go`

 * *Files identical despite different names*

### Comparing `dockerfile-3.2.0/pylib/support.c` & `dockerfile-3.3.0/pylib/support.c`

 * *Files identical despite different names*

