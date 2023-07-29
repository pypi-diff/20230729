# Comparing `tmp/idefix_cli-2.3.3.tar.gz` & `tmp/idefix_cli-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idefix_cli-2.3.3.tar", last modified: Fri Jul 28 15:49:29 2023, max compression
+gzip compressed data, was "idefix_cli-2.4.0.tar", last modified: Sat Jul 29 16:55:02 2023, max compression
```

## Comparing `idefix_cli-2.3.3.tar` & `idefix_cli-2.4.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:49:29.342329 idefix_cli-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-28 15:49:29.342329 idefix_cli-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 15:49:29.342329 idefix_cli-2.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:49:29.334329 idefix_cli-2.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:49:29.334329 idefix_cli-2.3.3/src/idefix_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:49:29.338329 idefix_cli-2.3.3/src/idefix_cli/_commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_commands/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_commands/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_commands/read.py
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_commands/stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_commands/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_commands/write.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/src/idefix_cli/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:49:29.338329 idefix_cli-2.3.3/src/idefix_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-28 15:49:29.000000 idefix_cli-2.3.3/src/idefix_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 15:49:29.000000 idefix_cli-2.3.3/src/idefix_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:49:29.000000 idefix_cli-2.3.3/src/idefix_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-28 15:49:29.000000 idefix_cli-2.3.3/src/idefix_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-28 15:49:29.000000 idefix_cli-2.3.3/src/idefix_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 15:49:29.000000 idefix_cli-2.3.3/src/idefix_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:49:29.342329 idefix_cli-2.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_app_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-28 15:49:15.000000 idefix_cli-2.3.3/tests/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:55:02.340545 idefix_cli-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-29 16:55:02.340545 idefix_cli-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 16:55:02.340545 idefix_cli-2.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:55:02.336545 idefix_cli-2.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:55:02.336545 idefix_cli-2.4.0/src/idefix_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_backports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:55:02.340545 idefix_cli-2.4.0/src/idefix_cli/_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:55:02.340545 idefix_cli-2.4.0/src/idefix_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-29 16:55:02.000000 idefix_cli-2.4.0/src/idefix_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-29 16:55:02.000000 idefix_cli-2.4.0/src/idefix_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 16:55:02.000000 idefix_cli-2.4.0/src/idefix_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-29 16:55:02.000000 idefix_cli-2.4.0/src/idefix_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-29 16:55:02.000000 idefix_cli-2.4.0/src/idefix_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 16:55:02.000000 idefix_cli-2.4.0/src/idefix_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:55:02.340545 idefix_cli-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_app_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_write.py
```

### Comparing `idefix_cli-2.3.3/LICENSE` & `idefix_cli-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/PKG-INFO` & `idefix_cli-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idefix_cli
-Version: 2.3.3
+Version: 2.4.0
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
```

### Comparing `idefix_cli-2.3.3/README.md` & `idefix_cli-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/pyproject.toml` & `idefix_cli-2.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/src/idefix_cli/__main__.py` & `idefix_cli-2.4.0/src/idefix_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/src/idefix_cli/_backports.py` & `idefix_cli-2.4.0/src/idefix_cli/_backports.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/src/idefix_cli/_commands/clean.py` & `idefix_cli-2.4.0/src/idefix_cli/_commands/clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/src/idefix_cli/_commands/clone.py` & `idefix_cli-2.4.0/src/idefix_cli/_commands/clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/src/idefix_cli/_commands/conf.py` & `idefix_cli-2.4.0/src/idefix_cli/_commands/conf.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/src/idefix_cli/_commands/read.py` & `idefix_cli-2.4.0/src/idefix_cli/_commands/read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/src/idefix_cli/_commands/run.py` & `idefix_cli-2.4.0/src/idefix_cli/_commands/run.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/src/idefix_cli/_commands/stamp.py` & `idefix_cli-2.4.0/src/idefix_cli/_commands/stamp.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/src/idefix_cli/_commands/switch.py` & `idefix_cli-2.4.0/src/idefix_cli/_commands/switch.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/src/idefix_cli/_commands/write.py` & `idefix_cli-2.4.0/src/idefix_cli/_commands/write.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/src/idefix_cli/lib.py` & `idefix_cli-2.4.0/src/idefix_cli/lib.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/src/idefix_cli.egg-info/PKG-INFO` & `idefix_cli-2.4.0/src/idefix_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idefix-cli
-Version: 2.3.3
+Version: 2.4.0
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
```

### Comparing `idefix_cli-2.3.3/src/idefix_cli.egg-info/SOURCES.txt` & `idefix_cli-2.4.0/src/idefix_cli.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,23 +12,25 @@
 src/idefix_cli.egg-info/entry_points.txt
 src/idefix_cli.egg-info/requires.txt
 src/idefix_cli.egg-info/top_level.txt
 src/idefix_cli/_commands/__init__.py
 src/idefix_cli/_commands/clean.py
 src/idefix_cli/_commands/clone.py
 src/idefix_cli/_commands/conf.py
+src/idefix_cli/_commands/digest.py
 src/idefix_cli/_commands/read.py
 src/idefix_cli/_commands/run.py
 src/idefix_cli/_commands/stamp.py
 src/idefix_cli/_commands/switch.py
 src/idefix_cli/_commands/write.py
 tests/test_app_structure.py
 tests/test_clean.py
 tests/test_clone.py
 tests/test_commons.py
 tests/test_conf.py
+tests/test_digest.py
 tests/test_lib.py
 tests/test_read.py
 tests/test_run.py
 tests/test_stamp.py
 tests/test_ux.py
 tests/test_write.py
```

### Comparing `idefix_cli-2.3.3/tests/test_app_structure.py` & `idefix_cli-2.4.0/tests/test_app_structure.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/tests/test_clean.py` & `idefix_cli-2.4.0/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/tests/test_clone.py` & `idefix_cli-2.4.0/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/tests/test_commons.py` & `idefix_cli-2.4.0/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/tests/test_conf.py` & `idefix_cli-2.4.0/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/tests/test_read.py` & `idefix_cli-2.4.0/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/tests/test_run.py` & `idefix_cli-2.4.0/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/tests/test_stamp.py` & `idefix_cli-2.4.0/tests/test_stamp.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.3/tests/test_ux.py` & `idefix_cli-2.4.0/tests/test_ux.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,37 +6,46 @@
 from idefix_cli.__main__ import main
 
 if sys.version_info >= (3, 10):
     OPTIONAL_SEC = "options"
 else:
     OPTIONAL_SEC = "optional arguments"
 HELP_MESSAGE = (
-    "usage: idfx [-h] [-v] {clean,clone,conf,read,run,stamp,switch,write} ...\n"
+    "usage: idfx [-h] [-v] {clean,clone,conf,digest,read,run,stamp,switch,write} ...\n"
     "\n"
     f"{OPTIONAL_SEC}:\n"
     "  -h, --help            show this help message and exit\n"
     "  -v, --version         show program's version number and exit\n"
     "\n"
     "commands:\n"
-    "  {clean,clone,conf,read,run,stamp,switch,write}\n"
+    "  {clean,clone,conf,digest,read,run,stamp,switch,write}\n"
     "    clean               remove compilation files\n"
     "    clone               clone a problem directory\n"
     "    conf                configure Idefix\n"
+    "    digest              agregate performance data from log files as json\n"
     "    read                read an Idefix inifile and print it to json format\n"
     "    run                 run an Idefix problem\n"
     "    stamp               print relevant data for reproduction to stdout\n"
     "    switch              switch git branch in $IDEFIX_DIR using git checkout\n"
     "    write               write an Idefix inifile from a json string\n"
 )
 
 
+def get_lines(help_message: str) -> list[str]:
+    # skip the first lines because they differ between macos and linux
+    lines = iter(help_message.splitlines())
+    while not next(lines).startswith(OPTIONAL_SEC):
+        continue
+
+    return list(lines)
+
+
 @pytest.mark.usefixtures("isolated_conf_dir")
 def test_no_command_passed(capsys):
     ret = main([])
     with check:
         assert ret != 0
     out, err = capsys.readouterr()
     with check:
         assert out == ""
     with check:
-        # skip the first lines because they differ between macos and linux
-        assert err.splitlines()[2:] == HELP_MESSAGE.splitlines()[2:]
+        assert get_lines(err) == get_lines(HELP_MESSAGE)
```

### Comparing `idefix_cli-2.3.3/tests/test_write.py` & `idefix_cli-2.4.0/tests/test_write.py`

 * *Files identical despite different names*

