# Comparing `tmp/yapx-0.2.3.tar.gz` & `tmp/yapx-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yapx-0.2.3.tar", last modified: Sat Jul 29 00:02:49 2023, max compression
+gzip compressed data, was "yapx-0.2.4.tar", last modified: Sat Jul 29 21:33:28 2023, max compression
```

## Comparing `yapx-0.2.3.tar` & `yapx-0.2.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 00:02:49.445670 yapx-0.2.3/
--rw-r--r--   0 root         (0) root         (0)     1058 2023-07-28 23:58:26.000000 yapx-0.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5528 2023-07-29 00:02:49.445670 yapx-0.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3785 2023-07-28 23:58:26.000000 yapx-0.2.3/README.md
--rw-r--r--   0 root         (0) root         (0)     4885 2023-07-28 23:58:26.000000 yapx-0.2.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 00:02:49.445670 yapx-0.2.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 00:02:49.433670 yapx-0.2.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 00:02:49.437670 yapx-0.2.3/src/yapx/
--rw-r--r--   0 root         (0) root         (0)     5155 2023-07-28 23:58:26.000000 yapx-0.2.3/src/yapx/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 00:02:49.441670 yapx-0.2.3/src/yapx/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     4901 2023-07-28 23:59:06.000000 yapx-0.2.3/src/yapx/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      148 2023-07-29 00:02:28.000000 yapx-0.2.3/src/yapx/__pycache__/__version__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     7098 2023-07-28 23:59:06.000000 yapx-0.2.3/src/yapx/__pycache__/actions.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     7626 2023-07-28 23:59:06.000000 yapx-0.2.3/src/yapx/__pycache__/arg.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)    28026 2023-07-28 23:59:06.000000 yapx-0.2.3/src/yapx/__pycache__/argument_parser.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      921 2023-07-28 23:59:06.000000 yapx-0.2.3/src/yapx/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      784 2023-07-28 23:59:07.000000 yapx-0.2.3/src/yapx/__pycache__/namespace.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     1550 2023-07-28 23:59:06.000000 yapx-0.2.3/src/yapx/__pycache__/types.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     4278 2023-07-28 23:59:06.000000 yapx-0.2.3/src/yapx/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-29 00:02:28.000000 yapx-0.2.3/src/yapx/__version__.py
--rw-r--r--   0 root         (0) root         (0)     9750 2023-07-28 23:58:26.000000 yapx-0.2.3/src/yapx/actions.py
--rw-r--r--   0 root         (0) root         (0)     9642 2023-07-28 23:58:26.000000 yapx-0.2.3/src/yapx/arg.py
--rw-r--r--   0 root         (0) root         (0)    45077 2023-07-28 23:58:26.000000 yapx-0.2.3/src/yapx/argument_parser.py
--rw-r--r--   0 root         (0) root         (0)      633 2023-07-28 23:58:26.000000 yapx-0.2.3/src/yapx/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-07-28 23:58:26.000000 yapx-0.2.3/src/yapx/namespace.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 23:58:26.000000 yapx-0.2.3/src/yapx/py.typed
--rw-r--r--   0 root         (0) root         (0)     1300 2023-07-28 23:58:26.000000 yapx-0.2.3/src/yapx/types.py
--rw-r--r--   0 root         (0) root         (0)     4211 2023-07-28 23:58:26.000000 yapx-0.2.3/src/yapx/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 00:02:49.441670 yapx-0.2.3/src/yapx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5528 2023-07-29 00:02:49.000000 yapx-0.2.3/src/yapx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      981 2023-07-29 00:02:49.000000 yapx-0.2.3/src/yapx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 00:02:49.000000 yapx-0.2.3/src/yapx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      770 2023-07-29 00:02:49.000000 yapx-0.2.3/src/yapx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-29 00:02:49.000000 yapx-0.2.3/src/yapx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 00:02:49.445670 yapx-0.2.3/tests/
--rw-r--r--   0 root         (0) root         (0)     5205 2023-07-28 23:58:26.000000 yapx-0.2.3/tests/test_actions.py
--rw-r--r--   0 root         (0) root         (0)    11974 2023-07-28 23:58:26.000000 yapx-0.2.3/tests/test_add_arguments.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-07-28 23:58:26.000000 yapx-0.2.3/tests/test_add_arguments_future.py
--rw-r--r--   0 root         (0) root         (0)     1260 2023-07-28 23:58:26.000000 yapx-0.2.3/tests/test_add_command.py
--rw-r--r--   0 root         (0) root         (0)     8186 2023-07-28 23:58:26.000000 yapx-0.2.3/tests/test_arg.py
--rw-r--r--   0 root         (0) root         (0)    25223 2023-07-28 23:58:26.000000 yapx-0.2.3/tests/test_run.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-07-28 23:58:26.000000 yapx-0.2.3/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 21:33:28.530760 yapx-0.2.4/
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-07-29 21:28:42.000000 yapx-0.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5528 2023-07-29 21:33:28.526760 yapx-0.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3785 2023-07-29 21:28:42.000000 yapx-0.2.4/README.md
+-rw-r--r--   0 root         (0) root         (0)     4885 2023-07-29 21:28:42.000000 yapx-0.2.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 21:33:28.530760 yapx-0.2.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 21:33:28.518760 yapx-0.2.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 21:33:28.522760 yapx-0.2.4/src/yapx/
+-rw-r--r--   0 root         (0) root         (0)     5155 2023-07-29 21:28:42.000000 yapx-0.2.4/src/yapx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 21:33:28.526760 yapx-0.2.4/src/yapx/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     4901 2023-07-29 21:29:21.000000 yapx-0.2.4/src/yapx/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-29 21:33:07.000000 yapx-0.2.4/src/yapx/__pycache__/__version__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     7098 2023-07-29 21:29:21.000000 yapx-0.2.4/src/yapx/__pycache__/actions.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     7626 2023-07-29 21:29:21.000000 yapx-0.2.4/src/yapx/__pycache__/arg.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)    28272 2023-07-29 21:29:21.000000 yapx-0.2.4/src/yapx/__pycache__/argument_parser.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      921 2023-07-29 21:29:21.000000 yapx-0.2.4/src/yapx/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      784 2023-07-29 21:29:21.000000 yapx-0.2.4/src/yapx/__pycache__/namespace.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-07-29 21:29:21.000000 yapx-0.2.4/src/yapx/__pycache__/types.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     4278 2023-07-29 21:29:21.000000 yapx-0.2.4/src/yapx/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-29 21:33:07.000000 yapx-0.2.4/src/yapx/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     9750 2023-07-29 21:28:42.000000 yapx-0.2.4/src/yapx/actions.py
+-rw-r--r--   0 root         (0) root         (0)     9642 2023-07-29 21:28:42.000000 yapx-0.2.4/src/yapx/arg.py
+-rw-r--r--   0 root         (0) root         (0)    45604 2023-07-29 21:28:42.000000 yapx-0.2.4/src/yapx/argument_parser.py
+-rw-r--r--   0 root         (0) root         (0)      633 2023-07-29 21:28:42.000000 yapx-0.2.4/src/yapx/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-29 21:28:42.000000 yapx-0.2.4/src/yapx/namespace.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 21:28:42.000000 yapx-0.2.4/src/yapx/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-07-29 21:28:42.000000 yapx-0.2.4/src/yapx/types.py
+-rw-r--r--   0 root         (0) root         (0)     4211 2023-07-29 21:28:42.000000 yapx-0.2.4/src/yapx/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 21:33:28.522760 yapx-0.2.4/src/yapx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5528 2023-07-29 21:33:28.000000 yapx-0.2.4/src/yapx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      981 2023-07-29 21:33:28.000000 yapx-0.2.4/src/yapx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 21:33:28.000000 yapx-0.2.4/src/yapx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      770 2023-07-29 21:33:28.000000 yapx-0.2.4/src/yapx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-29 21:33:28.000000 yapx-0.2.4/src/yapx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 21:33:28.526760 yapx-0.2.4/tests/
+-rw-r--r--   0 root         (0) root         (0)     5205 2023-07-29 21:28:42.000000 yapx-0.2.4/tests/test_actions.py
+-rw-r--r--   0 root         (0) root         (0)    11974 2023-07-29 21:28:42.000000 yapx-0.2.4/tests/test_add_arguments.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-07-29 21:28:42.000000 yapx-0.2.4/tests/test_add_arguments_future.py
+-rw-r--r--   0 root         (0) root         (0)     1260 2023-07-29 21:28:42.000000 yapx-0.2.4/tests/test_add_command.py
+-rw-r--r--   0 root         (0) root         (0)     8186 2023-07-29 21:28:42.000000 yapx-0.2.4/tests/test_arg.py
+-rw-r--r--   0 root         (0) root         (0)    25223 2023-07-29 21:28:42.000000 yapx-0.2.4/tests/test_run.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-07-29 21:28:42.000000 yapx-0.2.4/tests/test_utils.py
```

### Comparing `yapx-0.2.3/LICENSE` & `yapx-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yapx-0.2.3/PKG-INFO` & `yapx-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yapx
-Version: 0.2.3
+Version: 0.2.4
 Summary: The next generation of Python's Argparse.
 Author-email: Donald Mellenbruch <hello@f2dv.com>
 License: Copyright 2023 Donald Mellenbruch
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `yapx-0.2.3/README.md` & `yapx-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `yapx-0.2.3/pyproject.toml` & `yapx-0.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -62,21 +62,21 @@
 shtab = [
     "shtab==1.6.*",
 ]
 rich = [
     "rich-argparse==1.*",
 ]
 tui = [
-    "argparse-tui>=0.1.2,<1",
+    "argparse-tui>=0.2.0,<1",
 ]
 extras = [
     "pydantic>=1.10.3,<3",
     "shtab==1.6.2",
     "rich-argparse==1.*",
-    "argparse-tui>=0.1.2,<1",
+    "argparse-tui>=0.2.0,<1",
 ]
 
 [project.urls]
 Homepage = "https://www.f2dv.com/r/yapx"
 Repository = "https://www.github.com/fresh2dev/yapx"
 Funding = "https://www.f2dv.com/fund"
```

### Comparing `yapx-0.2.3/src/yapx/__init__.py` & `yapx-0.2.4/src/yapx/__init__.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.3/src/yapx/__pycache__/__init__.cpython-310.pyc` & `yapx-0.2.4/src/yapx/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 23:58:26 2023 UTC, .py size: 5155 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2256 c464 2314 0000  o......."V.d#...
+00000000: 6f0d 0d0a 0000 0000 8a84 c564 2314 0000  o..........d#...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000f 0000 0040 0000 0073 1402 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6403 6404 6c09  m.Z.m.Z...d.d.l.
 00000060: 6d0a 5a0a 6d0b 5a0b 0100 6403 6405 6c0c  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6403 6406 6c0d 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `yapx-0.2.3/src/yapx/__pycache__/actions.cpython-310.pyc` & `yapx-0.2.4/src/yapx/__pycache__/actions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 23:58:26 2023 UTC, .py size: 9750 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2256 c464 1626 0000  o......."V.d.&..
+00000000: 6f0d 0d0a 0000 0000 8a84 c564 1626 0000  o..........d.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 7201 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6400 6403 6c03 6d08 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6404 6c0a 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  d.l.m.Z.m.Z.m.Z.
```

### Comparing `yapx-0.2.3/src/yapx/__pycache__/arg.cpython-310.pyc` & `yapx-0.2.4/src/yapx/__pycache__/arg.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 23:58:26 2023 UTC, .py size: 9642 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2256 c464 aa25 0000  o......."V.d.%..
+00000000: 6f0d 0d0a 0000 0000 8a84 c564 aa25 0000  o..........d.%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0019 0000 0040 0000 0073 3c02 0000 5500  .....@...s<...U.
 00000030: 6400 6401 6c00 5a00 6400 6401 6c01 5a01  d.d.l.Z.d.d.l.Z.
 00000040: 6400 6402 6c02 6d03 5a03 0100 6400 6403  d.d.l.m.Z...d.d.
 00000050: 6c04 6d05 5a05 0100 6400 6404 6c06 6d07  l.m.Z...d.d.l.m.
 00000060: 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b  Z.m.Z.m.Z.m.Z.m.
 00000070: 5a0b 0100 6400 6405 6c0c 6d0d 5a0d 6d0e  Z...d.d.l.m.Z.m.
```

### Comparing `yapx-0.2.3/src/yapx/__pycache__/argument_parser.cpython-310.pyc` & `yapx-0.2.4/src/yapx/__pycache__/argument_parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 23:58:26 2023 UTC, .py size: 45077 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2256 c464 15b0 0000  o......."V.d....
+00000000: 6f0d 0d0a 0000 0000 8a84 c564 24b2 0000  o..........d$...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 c401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6402 6c02 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6400 6405 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
@@ -84,1669 +84,1684 @@
 00000530: 5f69 7369 6e73 7461 6e63 65da 0e74 7279  _isinstance..try
 00000540: 5f69 7373 7562 636c 6173 7329 02e9 0300  _issubclass)....
 00000550: 0000 e909 0000 0029 01da 0f5f 416e 6e6f  .......)..._Anno
 00000560: 7461 7465 6441 6c69 6173 a902 723a 0000  tatedAlias..r:..
 00000570: 00e9 0a00 0000 2901 da09 556e 696f 6e54  ......)...UnionT
 00000580: 7970 65da 0154 6300 0000 0000 0000 0000  ype..Tc.........
 00000590: 0000 0000 0000 0017 0000 0000 0000 0073  ...............s
-000005a0: 3c05 0000 6500 5a01 6400 5a02 5500 6401  <...e.Z.d.Z.U.d.
+000005a0: 4005 0000 6500 5a01 6400 5a02 5500 6401  @...e.Z.d.Z.U.d.
 000005b0: 5a03 6504 6505 6402 3c00 6403 5a06 6504  Z.e.e.d.<.d.Z.e.
 000005c0: 6505 6404 3c00 6405 5a07 6504 6505 6406  e.d.<.d.Z.e.e.d.
 000005d0: 3c00 6407 5a08 6504 6505 6408 3c00 6409  <.d.Z.e.e.d.<.d.
 000005e0: 5a09 6504 6505 640a 3c00 640b 640b 640b  Z.e.e.d.<.d.d.d.
-000005f0: 640b 640b 640b 640b 650a 640c 640d 9c09  d.d.d.d.e.d.d...
-00000600: 640e 650b 640f 650c 6504 1900 6410 650c  d.e.d.e.e...d.e.
-00000610: 6504 1900 6411 650c 6504 1900 6412 650c  e...d.e.e...d.e.
-00000620: 650d 6504 1900 1900 6413 650c 650d 6504  e.e.....d.e.e.e.
-00000630: 1900 1900 6414 650c 650d 6504 1900 1900  ....d.e.e.e.....
-00000640: 6415 650c 650d 6504 1900 1900 6416 650e  d.e.e.e.....d.e.
-00000650: 650b 1900 6417 650f 6418 650b 6616 8700  e...d.e.d.e.f...
-00000660: 6601 6419 641a 840e 5a10 641b 6504 6602  f.d.d...Z.d.e.f.
-00000670: 641c 641d 8404 5a11 090b 090c 646a 641e  d.d...Z.....djd.
-00000680: 650c 6512 6504 1900 1900 641f 650f 6420  e.e.e.....d.e.d 
-00000690: 640b 6606 8700 6601 6421 6422 840d 5a13  d.f...f.d!d"..Z.
-000006a0: 6423 6514 6515 6424 650b 6602 1900 650e  d#e.e.d$e.f...e.
-000006b0: 6516 1900 6602 1900 6420 640b 6604 6425  e...f...d d.f.d%
-000006c0: 6426 8404 5a17 090b 646b 6423 6514 6515  d&..Z...dkd#e.e.
-000006d0: 6424 650b 6602 1900 650e 6516 1900 6602  d$e.f...e.e...f.
-000006e0: 1900 6427 650c 6504 1900 6418 650b 6420  ..d'e.e...d.e.d 
-000006f0: 6518 6a19 6608 6428 6429 8405 5a1a 090b  e.j.f.d(d)..Z...
-00000700: 646b 642a 6515 6424 650b 6602 1900 6427  dkd*e.d$e.f...d'
-00000710: 650c 6504 1900 6418 650b 6420 640b 6608  e.e...d.e.d d.f.
-00000720: 642b 642c 8405 5a1b 651c 642d 650e 6516  d+d,..Z.e.d-e.e.
-00000730: 1900 642e 6504 6420 650f 6606 642f 6430  ..d.e.d e.f.d/d0
-00000740: 8404 8301 5a1d 651e 6431 6518 6a19 6423  ....Z.e.d1e.j.d#
-00000750: 6514 6515 6424 650b 6602 1900 650e 6516  e.e.d$e.f...e.e.
-00000760: 1900 6602 1900 6420 650d 651f 1900 6606  ..f...d e.e...f.
-00000770: 6432 6433 8404 8301 5a20 651c 6434 650e  d2d3....Z e.d4e.
-00000780: 650b 1900 6420 650c 650e 650b 1900 1900  e...d e.e.e.....
-00000790: 6604 6435 6436 8404 8301 5a21 651c 6434  f.d5d6....Z!e.d4
-000007a0: 650e 650b 1900 6420 6522 650e 650b 1900  e.e...d e"e.e...
-000007b0: 6424 6602 1900 6604 6437 6438 8404 8301  d$f...f.d7d8....
-000007c0: 5a23 651c 6434 650e 650b 1900 6420 6522  Z#e.d4e.e...d e"
-000007d0: 650e 650b 1900 6424 6602 1900 6604 6439  e.e...d$f...f.d9
-000007e0: 643a 8404 8301 5a24 651e 090c 090c 646c  d:....Z$e.....dl
-000007f0: 643b 650e 650b 1900 643c 650f 643d 650f  d;e.e...d<e.d=e.
-00000800: 6420 650e 650b 1900 6608 643e 643f 8405  d e.e...f.d>d?..
-00000810: 8301 5a25 6420 6518 6a26 6602 8700 6601  ..Z%d e.j&f...f.
-00000820: 6440 6441 840c 5a27 6420 650c 6518 6a26  d@dA..Z'd e.e.j&
-00000830: 1900 6602 6442 6443 8404 5a28 6420 6518  ..f.dBdC..Z(d e.
-00000840: 6a26 6602 6444 6445 8404 5a29 6446 6518  j&f.dDdE..Z)dFe.
-00000850: 6a2a 6420 652a 6604 6447 6448 8404 5a2b  j*d e*f.dGdH..Z+
-00000860: 090b 090b 646d 640e 650c 652c 6504 1900  ....dmd.e.e,e...
-00000870: 1900 6446 650c 6518 6a2a 1900 6420 652a  ..dFe.e.j*..d e*
-00000880: 6606 8700 6601 6449 644a 840d 5a2d 090b  f...f.dIdJ..Z-..
-00000890: 090b 646d 640e 650c 652c 6504 1900 1900  ..dmd.e.e,e.....
-000008a0: 6446 650c 6518 6a2a 1900 6420 6522 652a  dFe.e.j*..d e"e*
-000008b0: 650d 6504 1900 6602 1900 6606 8700 6601  e.e...f...f...f.
-000008c0: 644b 644c 840d 5a2e 090b 090b 090c 646e  dKdL..Z.......dn
-000008d0: 640e 650c 652c 6504 1900 1900 6423 650c  d.e.e,e.....d#e.
-000008e0: 650e 6516 1900 1900 644d 650f 6420 6522  e.e.....dMe.d e"
-000008f0: 6516 650d 6504 1900 6602 1900 6608 644e  e.e.e...f...f.dN
-00000900: 644f 8405 5a2f 090b 090b 090c 646e 640e  dO..Z/......dnd.
-00000910: 650c 652c 6504 1900 1900 6423 650c 650e  e.e,e.....d#e.e.
-00000920: 6516 1900 1900 644d 650f 6420 6516 6608  e.....dMe.d e.f.
-00000930: 6450 6451 8405 5a30 090b 090c 646a 640e  dPdQ..Z0....djd.
-00000940: 6518 6a2a 6423 650c 650e 6516 1900 1900  e.j*d#e.e.e.....
-00000950: 644d 650f 6420 6516 6608 6452 6453 8405  dMe.d e.f.dRdS..
-00000960: 5a31 651c 6454 6532 6504 650b 6602 1900  Z1e.dTe2e.e.f...
-00000970: 6423 650e 6516 1900 6420 6532 6504 650b  d#e.e...d e2e.e.
-00000980: 6602 1900 6606 6455 6456 8404 8301 5a33  f...f.dUdV....Z3
-00000990: 651e 6423 6514 6515 6424 650b 6602 1900  e.d#e.e.d$e.f...
-000009a0: 650e 6516 1900 6602 1900 6420 650c 6504  e.e...f...d e.e.
-000009b0: 1900 6604 6457 6458 8404 8301 5a34 651e  ..f.dWdX....Z4e.
-000009c0: 6431 6518 6a19 6423 6514 6515 6424 650b  d1e.j.d#e.e.d$e.
-000009d0: 6602 1900 650e 6516 1900 6602 1900 6420  f...e.e...f...d 
-000009e0: 640b 6606 6459 645a 8404 8301 5a35 651e  d.f.dYdZ....Z5e.
-000009f0: 090b 090b 090b 646f 6431 6400 642a 6515  ......dod1d.d*e.
-00000a00: 6424 650b 6602 1900 640e 650d 6504 1900  d$e.f...d.e.e...
-00000a10: 6423 650c 650e 650b 1900 1900 645b 650c  d#e.e.e.....d[e.
-00000a20: 6515 6424 650b 6602 1900 1900 645c 650c  e.d$e.f.....d\e.
-00000a30: 650b 1900 6420 650b 660e 645d 645e 8405  e...d e.f.d]d^..
-00000a40: 8301 5a36 651e 090b 090b 090b 646f 645f  ..Z6e.......dod_
-00000a50: 650c 6515 6424 650b 6602 1900 1900 6460  e.e.d$e.f.....d`
-00000a60: 650c 652c 6515 6424 650b 6602 1900 1900  e.e,e.d$e.f.....
-00000a70: 1900 6461 650c 6532 6504 6515 6424 650b  ..dae.e2e.e.d$e.
-00000a80: 6602 1900 6602 1900 1900 6418 650b 6420  f...f.....d.e.d 
-00000a90: 6400 660a 6462 6463 8405 8301 5a37 651e  d.f.dbdc....Z7e.
-00000aa0: 640b 640b 6464 9c02 6465 650b 640e 650c  d.d.dd..dee.d.e.
-00000ab0: 650d 6504 1900 1900 6466 650c 650d 6504  e.e.....dfe.e.e.
-00000ac0: 1900 1900 6467 650b 6420 650b 660a 6468  ....dge.d e.f.dh
-00000ad0: 6469 8406 8301 5a38 8700 0400 5a39 5300  di....Z8....Z9S.
-00000ae0: 2970 da0e 4172 6775 6d65 6e74 5061 7273  )p..ArgumentPars
-00000af0: 6572 5a0a 5f72 6f6f 745f 6675 6e63 da13  erZ._root_func..
-00000b00: 524f 4f54 5f46 554e 435f 4154 5452 5f4e  ROOT_FUNC_ATTR_N
-00000b10: 414d 455a 155f 726f 6f74 5f66 756e 635f  AMEZ._root_func_
-00000b20: 6172 6773 5f6d 6f64 656c da18 524f 4f54  args_model..ROOT
-00000b30: 5f46 554e 435f 4152 4753 5f41 5454 525f  _FUNC_ARGS_ATTR_
-00000b40: 4e41 4d45 5a08 5f63 6f6d 6d61 6e64 da0d  NAMEZ._command..
-00000b50: 434d 445f 4154 5452 5f4e 414d 455a 0d5f  CMD_ATTR_NAMEZ._
-00000b60: 636f 6d6d 616e 645f 6675 6e63 da12 434d  command_func..CM
-00000b70: 445f 4655 4e43 5f41 5454 525f 4e41 4d45  D_FUNC_ATTR_NAME
-00000b80: 5a18 5f63 6f6d 6d61 6e64 5f66 756e 635f  Z._command_func_
-00000b90: 6172 6773 5f6d 6f64 656c da17 434d 445f  args_model..CMD_
-00000ba0: 4655 4e43 5f41 5247 535f 4154 5452 5f4e  FUNC_ARGS_ATTR_N
-00000bb0: 414d 454e 4629 09da 0470 726f 67da 0c70  AMENF)...prog..p
-00000bc0: 726f 675f 7665 7273 696f 6eda 0b64 6573  rog_version..des
-00000bd0: 6372 6970 7469 6f6e da0a 6865 6c70 5f66  cription..help_f
-00000be0: 6c61 6773 da0d 7665 7273 696f 6e5f 666c  lags..version_fl
-00000bf0: 6167 73da 0974 7569 5f66 6c61 6773 da10  ags..tui_flags..
-00000c00: 636f 6d70 6c65 7469 6f6e 5f66 6c61 6773  completion_flags
-00000c10: da0f 666f 726d 6174 7465 725f 636c 6173  ..formatter_clas
-00000c20: 73da 0d5f 6973 5f73 7562 7061 7273 6572  s.._is_subparser
-00000c30: da04 6172 6773 7247 0000 0072 4800 0000  ..argsrG...rH...
-00000c40: 7249 0000 0072 4a00 0000 724b 0000 0072  rI...rJ...rK...r
-00000c50: 4c00 0000 724d 0000 0072 4e00 0000 724f  L...rM...rN...rO
-00000c60: 0000 00da 066b 7761 7267 7363 0100 0000  .....kwargsc....
-00000c70: 0000 0000 0900 0000 0d00 0000 0800 0000  ................
-00000c80: 0f00 0000 73ee 0100 0074 0083 006a 017c  ....s....t...j.|
-00000c90: 0a7c 017c 0972 0964 006e 017c 0364 017c  .|.|.r.d.n.|.d.|
-00000ca0: 0864 029c 047c 0ba4 018e 0101 0064 007c  .d...|.......d.|
-00000cb0: 005f 0264 037c 006a 035f 047c 0464 0075  ._.d.|.j._.|.d.u
-00000cc0: 0072 2164 0464 0567 027d 047c 0472 3974  .r!d.d.g.}.|.r9t
-00000cd0: 057c 0474 0683 0272 2b7c 0467 017d 047c  .|.t...r+|.g.}.|
-00000ce0: 006a 0764 0664 0784 007c 0444 0083 0174  .j.d.d...|.D...t
-00000cf0: 0864 0864 099c 028e 0101 0064 0a7c 005f  .d.d.......d.|._
-00000d00: 0974 0a64 0b64 0c84 0083 017c 005f 0b69  .t.d.d.....|._.i
-00000d10: 007c 005f 0c7c 0973 f17c 0472 5a64 0d64  .|._.|.s.|.rZd.d
-00000d20: 0784 007c 0444 0083 017d 0c7c 006a 077c  ...|.D...}.|.j.|
-00000d30: 0c74 0d64 0e64 099c 028e 0101 007c 0564  .t.d.d.......|.d
-00000d40: 0075 0072 6164 0f67 017d 057c 0572 9974  .u.rad.g.}.|.r.t
-00000d50: 057c 0574 0683 0272 6b7c 0567 017d 057c  .|.t...rk|.g.}.|
-00000d60: 006a 0e72 8a7c 0273 8a74 0f74 1083 018f  .j.r.|.s.t.t....
-00000d70: 0e01 0074 117c 006a 0e83 016a 127d 0257  ...t.|.j...j.}.W
-00000d80: 0064 0004 0004 0083 0301 006e 0831 0073  .d.........n.1.s
-00000d90: 8577 0101 0001 0001 0059 0001 007c 0272  .w.......Y...|.r
-00000da0: 997c 006a 077c 0564 1064 117c 029b 009d  .|.j.|.d.d.|....
-00000db0: 0264 1264 139c 038e 0101 007c 0764 0075  .d.d.......|.d.u
-00000dc0: 0072 a064 1467 017d 0774 1372 b97c 0772  .r.d.g.}.t.r.|.r
-00000dd0: b974 057c 0774 0683 0272 ac7c 0767 017d  .t.|.t...r.|.g.}
-00000de0: 077c 006a 077c 0774 1483 0074 156a 1674  .|.j.|.t...t.j.t
-00000df0: 1764 1564 169c 048e 0101 007c 0664 0075  .d.d.......|.d.u
-00000e00: 0072 c064 1767 017d 067c 0672 f374 1872  .r.d.g.}.|.r.t.r
-00000e10: f574 057c 0674 0683 0272 cc7c 0667 017d  .t.|.t...r.|.g.}
-00000e20: 0674 197c 0683 0164 186b 0272 e87c 0664  .t.|...d.k.r.|.d
-00000e30: 1919 00a0 1a64 1aa1 0173 e87c 00a0 1ba1  .....d...s.|....
-00000e40: 0001 0074 1c7c 007c 0664 1919 0064 1b64  ...t.|.|.d...d.d
-00000e50: 1c8d 0301 0064 0053 0074 1d7c 007c 0664  .....d.S.t.|.|.d
-00000e60: 1b64 1c8d 0301 0064 0053 0064 0053 0064  .d.....d.S.d.S.d
-00000e70: 0053 0064 0053 0029 1d4e 4629 0472 4700  .S.d.S.).NF).rG.
-00000e80: 0000 7249 0000 00da 0861 6464 5f68 656c  ..rI.....add_hel
-00000e90: 7072 4e00 0000 7a12 6865 6c70 6675 6c20  prN...z.helpful 
-00000ea0: 7061 7261 6d65 7465 7273 7a02 2d68 7a06  parametersz.-hz.
-00000eb0: 2d2d 6865 6c70 6301 0000 0000 0000 0000  --helpc.........
-00000ec0: 0000 0002 0000 0003 0000 0053 0000 0073  ...........S...s
-00000ed0: 1400 0000 6700 7c00 5d06 7d01 7c01 7202  ....g.|.].}.|.r.
-00000ee0: 7c01 9102 7102 5300 a900 7253 0000 00a9  |...q.S...rS....
-00000ef0: 02da 022e 30da 0178 7253 0000 0072 5300  ....0..xrS...rS.
-00000f00: 0000 fa26 2f64 726f 6e65 2f73 7263 2f73  ...&/drone/src/s
-00000f10: 7263 2f79 6170 782f 6172 6775 6d65 6e74  rc/yapx/argument
-00000f20: 5f70 6172 7365 722e 7079 da0a 3c6c 6973  _parser.py..<lis
-00000f30: 7463 6f6d 703e 7600 0000 7302 0000 0014  tcomp>v...s.....
-00000f40: 007a 2b41 7267 756d 656e 7450 6172 7365  .z+ArgumentParse
-00000f50: 722e 5f5f 696e 6974 5f5f 2e3c 6c6f 6361  r.__init__.<loca
-00000f60: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7a17  ls>.<listcomp>z.
-00000f70: 5368 6f77 2074 6869 7320 6865 6c70 206d  Show this help m
-00000f80: 6573 7361 6765 2e29 02da 0661 6374 696f  essage.)...actio
-00000f90: 6eda 0468 656c 70fa 013d 6300 0000 0000  n..help..=c.....
-00000fa0: 0000 0000 0000 0000 0000 0002 0000 0053  ...............S
-00000fb0: 0000 0073 0800 0000 7400 7401 8301 5300  ...s....t.t...S.
-00000fc0: a901 4e29 0272 0200 0000 da04 6c69 7374  ..N).r......list
-00000fd0: 7253 0000 0072 5300 0000 7253 0000 0072  rS...rS...rS...r
-00000fe0: 5700 0000 da08 3c6c 616d 6264 613e 8000  W.....<lambda>..
-00000ff0: 0000 7302 0000 0008 007a 2941 7267 756d  ..s......z)Argum
-00001000: 656e 7450 6172 7365 722e 5f5f 696e 6974  entParser.__init
-00001010: 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  __.<locals>.<lam
-00001020: 6264 613e 6301 0000 0000 0000 0000 0000  bda>c...........
-00001030: 0002 0000 0005 0000 0053 0000 0073 2000  .........S...s .
-00001040: 0000 6700 7c00 5d0c 7d01 7c01 a000 6400  ..g.|.].}.|...d.
-00001050: a101 7202 7c01 9b00 6401 9d02 9102 7102  ..r.|...d.....q.
-00001060: 5300 2902 7a02 2d2d 7a04 2d61 6c6c a901  S.).z.--z.-all..
-00001070: da0a 7374 6172 7473 7769 7468 7254 0000  ..startswithrT..
-00001080: 0072 5300 0000 7253 0000 0072 5700 0000  .rS...rS...rW...
-00001090: 7258 0000 0086 0000 00f3 0200 0000 2000  rX............ .
-000010a0: 7a1b 5368 6f77 2068 656c 7020 666f 7220  z.Show help for 
-000010b0: 616c 6c20 636f 6d6d 616e 6473 2e7a 092d  all commands.z.-
-000010c0: 2d76 6572 7369 6f6e da07 7665 7273 696f  -version..versio
-000010d0: 6e7a 0925 2870 726f 6729 7320 7a20 5368  nz.%(prog)s z Sh
-000010e0: 6f77 2074 6865 2070 726f 6772 616d 2076  ow the program v
-000010f0: 6572 7369 6f6e 206e 756d 6265 722e 2903  ersion number.).
-00001100: 7259 0000 0072 6200 0000 725a 0000 007a  rY...rb...rZ...z
-00001110: 182d 2d70 7269 6e74 2d73 6865 6c6c 2d63  .--print-shell-c
-00001120: 6f6d 706c 6574 696f 6e7a 1e50 7269 6e74  ompletionz.Print
-00001130: 2073 6865 6c6c 2063 6f6d 706c 6574 696f   shell completio
-00001140: 6e20 7363 7269 7074 2e29 0472 5900 0000  n script.).rY...
-00001150: da07 6465 6661 756c 74da 0763 686f 6963  ..default..choic
-00001160: 6573 725a 0000 007a 052d 2d74 7569 7217  esrZ...z.--tuir.
-00001170: 0000 0072 0100 0000 fa01 2d7a 2253 686f  ...r......-z"Sho
-00001180: 7720 5465 7874 7561 6c20 5573 6572 2049  w Textual User I
-00001190: 6e74 6572 6661 6365 2028 5455 4929 2e29  nterface (TUI).)
-000011a0: 03da 0670 6172 7365 72da 0e6f 7074 696f  ...parser..optio
-000011b0: 6e5f 7374 7269 6e67 7372 5a00 0000 291e  n_stringsrZ...).
-000011c0: da05 7375 7065 72da 085f 5f69 6e69 745f  ..super..__init_
-000011d0: 5fda 125f 7375 6270 6172 7365 7273 5f61  _.._subparsers_a
-000011e0: 6374 696f 6eda 0a5f 6f70 7469 6f6e 616c  ction.._optional
-000011f0: 73da 0574 6974 6c65 da0a 6973 696e 7374  s..title..isinst
-00001200: 616e 6365 da03 7374 72da 0c61 6464 5f61  ance..str..add_a
-00001210: 7267 756d 656e 7472 1b00 0000 da0c 6b76  rgumentr......kv
-00001220: 5f73 6570 6172 6174 6f72 7202 0000 00da  _separatorr.....
-00001230: 185f 6d75 7475 616c 6c79 5f65 7863 6c75  ._mutually_exclu
-00001240: 7369 7665 5f61 7267 73da 0a5f 6465 7374  sive_args.._dest
-00001250: 5f74 7970 6572 1c00 0000 7247 0000 0072  _typer....rG...r
-00001260: 0300 0000 da09 4578 6365 7074 696f 6e72  ......Exceptionr
-00001270: 1600 0000 7262 0000 0072 3600 0000 7232  ....rb...r6...r2
-00001280: 0000 00da 0861 7267 7061 7273 65da 0853  .....argparse..S
-00001290: 5550 5052 4553 5372 2c00 0000 7237 0000  UPPRESSr,...r7..
-000012a0: 00da 036c 656e 7260 0000 00da 165f 6765  ...lenr`....._ge
-000012b0: 745f 6f72 5f61 6464 5f73 7562 7061 7273  t_or_add_subpars
-000012c0: 6572 7372 3000 0000 722f 0000 0029 0dda  ersr0...r/...)..
-000012d0: 0473 656c 6672 4700 0000 7248 0000 0072  .selfrG...rH...r
-000012e0: 4900 0000 724a 0000 0072 4b00 0000 724c  I...rJ...rK...rL
-000012f0: 0000 0072 4d00 0000 724e 0000 0072 4f00  ...rM...rN...rO.
-00001300: 0000 7250 0000 0072 5100 0000 5a0e 6865  ..rP...rQ...Z.he
-00001310: 6c70 5f61 6c6c 5f66 6c61 6773 a901 da09  lp_all_flags....
-00001320: 5f5f 636c 6173 735f 5f72 5300 0000 7257  __class__rS...rW
-00001330: 0000 0072 6900 0000 5300 0000 73a0 0000  ...ri...S...s...
-00001340: 0006 0e02 0102 010a 0102 0102 0104 fb02  ................
-00001350: 0606 fa06 0908 0308 0208 0104 020a 0106  ................
-00001360: 0104 010c 0102 0102 0108 fd06 060a 0504  ................
-00001370: fd06 0504 0204 010e 0104 0102 0102 0102  ................
-00001380: 0108 fd08 0606 0104 020a 0106 010a 020a  ................
-00001390: 010e 011c ff04 0304 0102 0102 0108 0102  ................
-000013a0: 0108 fc08 0706 0108 020a 0106 0104 0202  ................
-000013b0: 0104 0104 0102 0102 0108 fb08 0806 0108  ................
-000013c0: 020a 0106 011a 0208 0102 0102 0106 0102  ................
-000013d0: 010a fd02 0602 0102 0102 010a fd04 c608  ................
-000013e0: 2e7a 1741 7267 756d 656e 7450 6172 7365  .z.ArgumentParse
-000013f0: 722e 5f5f 696e 6974 5f5f da07 6d65 7373  r.__init__..mess
-00001400: 6167 6563 0200 0000 0000 0000 0000 0000  agec............
-00001410: 0200 0000 0600 0000 4300 0000 7324 0000  ........C...s$..
-00001420: 007c 00a0 0074 016a 02a1 0101 007c 00a0  .|...t.j.....|..
-00001430: 0364 0164 027c 019b 0064 039d 03a1 0201  .d.d.|...d......
-00001440: 0064 0053 0029 044e e902 0000 007a 0765  .d.S.).N.....z.e
-00001450: 7272 6f72 3a20 da01 0a29 04da 0b70 7269  rror: ...)...pri
-00001460: 6e74 5f75 7361 6765 da03 7379 73da 0673  nt_usage..sys..s
-00001470: 7464 6572 72da 0465 7869 7429 0272 7800  tderr..exit).rx.
-00001480: 0000 727b 0000 0072 5300 0000 7253 0000  ..r{...rS...rS..
-00001490: 0072 5700 0000 da05 6572 726f 72c4 0000  .rW.....error...
-000014a0: 0073 0400 0000 0c01 1801 7a14 4172 6775  .s........z.Argu
-000014b0: 6d65 6e74 5061 7273 6572 2e65 7272 6f72  mentParser.error
-000014c0: da04 6669 6c65 da10 696e 636c 7564 655f  ..file..include_
-000014d0: 636f 6d6d 616e 6473 da06 7265 7475 726e  commands..return
-000014e0: 6303 0000 0000 0000 0000 0000 0008 0000  c...............
-000014f0: 0005 0000 0003 0000 0073 9c00 0000 6401  .........s....d.
-00001500: 7d03 7c03 6402 1400 6403 1700 7d04 7400  }.|.d...d...}.t.
-00001510: 8300 0100 7400 7c04 8301 0100 7400 6404  ....t.|.....t.d.
-00001520: 7c00 6a01 9b00 9d02 8301 0100 7400 7c04  |.j.........t.|.
-00001530: 8301 0100 7c00 6a02 7d05 7403 6a04 7c00  ....|.j.}.t.j.|.
-00001540: 5f02 7405 8300 a006 7c01 a101 0100 7c02  _.t.....|.....|.
-00001550: 7249 7c00 6a07 7249 7c00 6a08 6405 7500  rI|.j.rI|.j.d.u.
-00001560: 7237 7c00 a009 a100 7c00 5f08 7c00 6a08  r7|.....|._.|.j.
-00001570: 6a0a a00b a100 4400 5d0b 5c02 7d06 7d07  j.....D.].\.}.}.
-00001580: 7c07 6a06 7c01 7c02 6406 8d02 0100 713d  |.j.|.|.d.....q=
-00001590: 7c05 7c00 5f02 6405 5300 2907 6118 0200  |.|._.d.S.).a...
-000015a0: 0050 7269 6e74 2043 4c49 2068 656c 702e  .Print CLI help.
-000015b0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-000015c0: 2020 2020 2020 2020 2020 2020 696e 636c              incl
-000015d0: 7564 655f 636f 6d6d 616e 6473 3a20 6966  ude_commands: if
-000015e0: 2054 7275 652c 2061 6c73 6f20 7072 696e   True, also prin
-000015f0: 7420 6865 6c70 2066 6f72 2065 6163 6820  t help for each 
-00001600: 636f 6d6d 616e 642e 0a0a 2020 2020 2020  command...      
-00001610: 2020 4578 616d 706c 6573 3a0a 2020 2020    Examples:.    
-00001620: 2020 2020 2020 2020 3e3e 3e20 696d 706f          >>> impo
-00001630: 7274 2079 6170 780a 2020 2020 2020 2020  rt yapx.        
-00001640: 2020 2020 3e3e 3e20 6672 6f6d 2064 6174      >>> from dat
-00001650: 6163 6c61 7373 6573 2069 6d70 6f72 7420  aclasses import 
-00001660: 6461 7461 636c 6173 730a 2020 2020 2020  dataclass.      
-00001670: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
-00001680: 2020 2020 2020 3e3e 3e20 4064 6174 6163        >>> @datac
-00001690: 6c61 7373 0a20 2020 2020 2020 2020 2020  lass.           
-000016a0: 202e 2e2e 2063 6c61 7373 2041 6464 4e75   ... class AddNu
-000016b0: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-000016c0: 2e2e 2e20 2020 2020 783a 2069 6e74 0a20  ...     x: int. 
-000016d0: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
-000016e0: 2020 2079 3a20 696e 740a 2020 2020 2020     y: int.      
-000016f0: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
-00001700: 2020 2020 2020 3e3e 3e20 7061 7273 6572        >>> parser
-00001710: 203d 2079 6170 782e 4172 6775 6d65 6e74   = yapx.Argument
-00001720: 5061 7273 6572 2829 0a20 2020 2020 2020  Parser().       
-00001730: 2020 2020 203e 3e3e 2070 6172 7365 722e       >>> parser.
-00001740: 6164 645f 6172 6775 6d65 6e74 7328 4164  add_arguments(Ad
-00001750: 644e 756d 7329 0a20 2020 2020 2020 2020  dNums).         
-00001760: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
-00001770: 2020 203e 3e3e 2070 6172 7365 722e 7072     >>> parser.pr
-00001780: 696e 745f 6865 6c70 2869 6e63 6c75 6465  int_help(include
-00001790: 5f63 6f6d 6d61 6e64 733d 5472 7565 2920  _commands=True) 
-000017a0: 2023 646f 6374 6573 743a 202b 534b 4950   #doctest: +SKIP
-000017b0: 0a20 2020 2020 2020 20da 015f e950 0000  .        .._.P..
-000017c0: 0072 7d00 0000 7a02 2420 4e29 0172 8400  .r}...z.$ N).r..
-000017d0: 0000 290c da05 7072 696e 7472 4700 0000  ..)...printrG...
-000017e0: da05 7573 6167 6572 7400 0000 7275 0000  ..usagert...ru..
-000017f0: 0072 6800 0000 da0a 7072 696e 745f 6865  .rh.....print_he
-00001800: 6c70 da0b 5f73 7562 7061 7273 6572 7372  lp.._subparsersr
-00001810: 6a00 0000 da17 5f66 696e 645f 7375 6270  j....._find_subp
-00001820: 6172 7365 7273 5f61 6374 696f 6e72 6400  arsers_actionrd.
-00001830: 0000 da05 6974 656d 7329 0872 7800 0000  ....items).rx...
-00001840: 7283 0000 0072 8400 0000 5a08 7365 705f  r....r....Z.sep_
-00001850: 6368 6172 da09 7365 7061 7261 746f 7272  char..separatorr
-00001860: 8900 0000 5a07 5f63 686f 6963 655a 0973  ....Z._choiceZ.s
-00001870: 7562 7061 7273 6572 7279 0000 0072 5300  ubparserry...rS.
-00001880: 0000 7257 0000 0072 8a00 0000 c800 0000  ..rW...r........
-00001890: 731e 0000 0004 180c 0106 0108 0110 0108  s...............
-000018a0: 0106 0308 010c 020a 020a 010a 0114 0210  ................
-000018b0: 010a 027a 1941 7267 756d 656e 7450 6172  ...z.ArgumentPar
-000018c0: 7365 722e 7072 696e 745f 6865 6c70 da0a  ser.print_help..
-000018d0: 6172 6773 5f6d 6f64 656c 2e63 0200 0000  args_model.c....
-000018e0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-000018f0: 4300 0000 7310 0000 007c 00a0 007c 007c  C...s....|...|.|
-00001900: 01a1 0201 0064 0153 0029 0261 d605 0000  .....d.S.).a....
-00001910: 4164 6420 6172 6775 6d65 6e74 7320 6672  Add arguments fr
-00001920: 6f6d 2074 6865 2067 6976 656e 2066 756e  om the given fun
-00001930: 6374 696f 6e20 6f72 2064 6174 6166 7261  ction or datafra
-00001940: 6d65 2e0a 0a20 2020 2020 2020 2041 7267  me...        Arg
-00001950: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
-00001960: 7267 735f 6d6f 6465 6c3a 2061 2066 756e  rgs_model: a fun
-00001970: 6374 696f 6e20 6f72 2064 6174 6163 6c61  ction or datacla
-00001980: 7373 2066 726f 6d20 7768 6963 6820 746f  ss from which to
-00001990: 2064 6572 6976 6520 6172 6775 6d65 6e74   derive argument
-000019a0: 732e 0a0a 2020 2020 2020 2020 4578 616d  s...        Exam
-000019b0: 706c 6573 3a0a 2020 2020 2020 2020 2020  ples:.          
-000019c0: 2020 3e3e 3e20 696d 706f 7274 2079 6170    >>> import yap
-000019d0: 780a 2020 2020 2020 2020 2020 2020 3e3e  x.            >>
-000019e0: 3e20 6672 6f6d 2064 6174 6163 6c61 7373  > from dataclass
-000019f0: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
-00001a00: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
-00001a10: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-00001a20: 3e3e 3e20 4064 6174 6163 6c61 7373 0a20  >>> @dataclass. 
-00001a30: 2020 2020 2020 2020 2020 202e 2e2e 2063             ... c
-00001a40: 6c61 7373 2041 6464 4e75 6d73 3a0a 2020  lass AddNums:.  
-00001a50: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
-00001a60: 2020 783a 2069 6e74 0a20 2020 2020 2020    x: int.       
-00001a70: 2020 2020 202e 2e2e 2020 2020 2079 3a20       ...     y: 
-00001a80: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
-00001a90: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-00001aa0: 3e3e 3e20 7061 7273 6572 203d 2079 6170  >>> parser = yap
-00001ab0: 782e 4172 6775 6d65 6e74 5061 7273 6572  x.ArgumentParser
-00001ac0: 2829 0a20 2020 2020 2020 2020 2020 203e  ().            >
-00001ad0: 3e3e 2070 6172 7365 722e 6164 645f 6172  >> parser.add_ar
-00001ae0: 6775 6d65 6e74 7328 4164 644e 756d 7329  guments(AddNums)
-00001af0: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
-00001b00: 2070 6172 7365 722e 7365 745f 6465 6661   parser.set_defa
-00001b10: 756c 7473 285f 636f 6d6d 616e 645f 6675  ults(_command_fu
-00001b20: 6e63 3d6c 616d 6264 6120 782c 2079 3a20  nc=lambda x, y: 
-00001b30: 782b 7929 0a20 2020 2020 2020 2020 2020  x+y).           
-00001b40: 203e 3e3e 2070 6172 7365 6420 3d20 7061   >>> parsed = pa
-00001b50: 7273 6572 2e70 6172 7365 5f61 7267 7328  rser.parse_args(
-00001b60: 5b27 2d78 272c 2027 3127 2c20 272d 7927  ['-x', '1', '-y'
-00001b70: 2c20 2732 275d 290a 2020 2020 2020 2020  , '2']).        
-00001b80: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
-00001b90: 2020 2020 3e3e 3e20 2870 6172 7365 642e      >>> (parsed.
-00001ba0: 782c 2070 6172 7365 642e 7929 0a20 2020  x, parsed.y).   
-00001bb0: 2020 2020 2020 2020 2028 312c 2032 290a           (1, 2).
-00001bc0: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00001bd0: 7061 7273 6564 2e5f 636f 6d6d 616e 645f  parsed._command_
-00001be0: 6675 6e63 5f61 7267 735f 6d6f 6465 6c28  func_args_model(
-00001bf0: 783d 7061 7273 6564 2e78 2c20 793d 7061  x=parsed.x, y=pa
-00001c00: 7273 6564 2e79 290a 2020 2020 2020 2020  rsed.y).        
-00001c10: 2020 2020 4164 644e 756d 7328 783d 312c      AddNums(x=1,
-00001c20: 2079 3d32 290a 2020 2020 2020 2020 2020   y=2).          
-00001c30: 2020 3e3e 3e20 7061 7273 6564 2e5f 636f    >>> parsed._co
-00001c40: 6d6d 616e 645f 6675 6e63 2878 3d70 6172  mmand_func(x=par
-00001c50: 7365 642e 782c 2079 3d70 6172 7365 642e  sed.x, y=parsed.
-00001c60: 7929 0a20 2020 2020 2020 2020 2020 2033  y).            3
-00001c70: 0a0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
-00001c80: 3e20 696d 706f 7274 2079 6170 780a 2020  > import yapx.  
-00001c90: 2020 2020 2020 2020 2020 2e2e 2e0a 2020            ....  
-00001ca0: 2020 2020 2020 2020 2020 3e3e 3e20 6465            >>> de
-00001cb0: 6620 6164 645f 6e75 6d73 2878 3a20 696e  f add_nums(x: in
-00001cc0: 742c 2079 3a20 696e 7429 3a0a 2020 2020  t, y: int):.    
-00001cd0: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
-00001ce0: 7265 7475 726e 2078 202b 2079 0a20 2020  return x + y.   
-00001cf0: 2020 2020 2020 2020 202e 2e2e 0a20 2020           ....   
-00001d00: 2020 2020 2020 2020 203e 3e3e 2070 6172           >>> par
-00001d10: 7365 7220 3d20 7961 7078 2e41 7267 756d  ser = yapx.Argum
-00001d20: 656e 7450 6172 7365 7228 290a 2020 2020  entParser().    
-00001d30: 2020 2020 2020 2020 3e3e 3e20 7061 7273          >>> pars
-00001d40: 6572 2e61 6464 5f61 7267 756d 656e 7473  er.add_arguments
-00001d50: 2861 6464 5f6e 756d 7329 0a20 2020 2020  (add_nums).     
-00001d60: 2020 2020 2020 203e 3e3e 2070 6172 7365         >>> parse
-00001d70: 722e 7365 745f 6465 6661 756c 7473 285f  r.set_defaults(_
-00001d80: 636f 6d6d 616e 645f 6675 6e63 3d61 6464  command_func=add
-00001d90: 5f6e 756d 7329 0a20 2020 2020 2020 2020  _nums).         
-00001da0: 2020 203e 3e3e 2070 6172 7365 6420 3d20     >>> parsed = 
-00001db0: 7061 7273 6572 2e70 6172 7365 5f61 7267  parser.parse_arg
-00001dc0: 7328 5b27 2d78 272c 2027 3127 2c20 272d  s(['-x', '1', '-
-00001dd0: 7927 2c20 2732 275d 290a 2020 2020 2020  y', '2']).      
-00001de0: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
-00001df0: 2020 2020 2020 3e3e 3e20 2870 6172 7365        >>> (parse
-00001e00: 642e 782c 2070 6172 7365 642e 7929 0a20  d.x, parsed.y). 
-00001e10: 2020 2020 2020 2020 2020 2028 312c 2032             (1, 2
-00001e20: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
-00001e30: 3e20 7061 7273 6564 2e5f 636f 6d6d 616e  > parsed._comman
-00001e40: 645f 6675 6e63 5f61 7267 735f 6d6f 6465  d_func_args_mode
-00001e50: 6c28 783d 7061 7273 6564 2e78 2c20 793d  l(x=parsed.x, y=
-00001e60: 7061 7273 6564 2e79 290a 2020 2020 2020  parsed.y).      
-00001e70: 2020 2020 2020 4461 7461 636c 6173 735f        Dataclass_
-00001e80: 6164 645f 6e75 6d73 2878 3d31 2c20 793d  add_nums(x=1, y=
-00001e90: 3229 0a20 2020 2020 2020 2020 2020 203e  2).            >
-00001ea0: 3e3e 2070 6172 7365 642e 5f63 6f6d 6d61  >> parsed._comma
-00001eb0: 6e64 5f66 756e 6328 783d 7061 7273 6564  nd_func(x=parsed
-00001ec0: 2e78 2c20 793d 7061 7273 6564 2e79 290a  .x, y=parsed.y).
-00001ed0: 2020 2020 2020 2020 2020 2020 330a 2020              3.  
-00001ee0: 2020 2020 2020 4e29 01da 0e5f 6164 645f        N)..._add_
-00001ef0: 6172 6775 6d65 6e74 7329 0272 7800 0000  arguments).rx...
-00001f00: 728f 0000 0072 5300 0000 7253 0000 0072  r....rS...rS...r
-00001f10: 5700 0000 da0d 6164 645f 6172 6775 6d65  W.....add_argume
-00001f20: 6e74 73f6 0000 0073 0200 0000 102f 7a1c  nts....s...../z.
-00001f30: 4172 6775 6d65 6e74 5061 7273 6572 2e61  ArgumentParser.a
-00001f40: 6464 5f61 7267 756d 656e 7473 da04 6e61  dd_arguments..na
-00001f50: 6d65 6303 0000 0000 0000 0000 0000 0009  mec.............
-00001f60: 0000 0005 0000 004b 0000 0073 9800 0000  .......K...s....
-00001f70: 7c00 a000 a100 7d04 7c02 730b 7401 7c01  |.....}.|.s.t.|.
-00001f80: 6a02 8301 7d02 7403 7c04 7404 6a05 8302  j...}.t.|.t.j...
-00001f90: 7313 4a00 8201 7c03 a006 6401 6402 a102  s.J...|...d.d...
-00001fa0: 7d05 7c05 7221 7c05 6403 7c02 1700 3700  }.|.r!|.d.|...7.
-00001fb0: 7d05 7c00 6a07 7c01 6404 8d01 7d06 6402  }.|.j.|.d...}.d.
-00001fc0: 7d07 7c06 7231 7c06 a008 a100 6405 1900  }.|.r1|.....d...
-00001fd0: 7d07 7c04 6a09 7c02 6601 7c05 7c07 6406  }.|.j.|.f.|.|.d.
-00001fe0: 9c02 7c03 a401 8e01 7d08 7c06 7242 7c06  ..|.....}.|.rB|.
-00001ff0: 7c08 5f0a 7c01 724a 7c00 a00b 7c08 7c01  |._.|.rJ|...|.|.
-00002000: a102 0100 7c08 5300 2907 6159 0800 0043  ....|.S.).aY...C
-00002010: 7265 6174 6520 6120 6e65 7720 7375 6263  reate a new subc
-00002020: 6f6d 6d61 6e64 2061 6e64 2061 6464 2061  ommand and add a
-00002030: 7267 756d 656e 7473 2066 726f 6d20 7468  rguments from th
-00002040: 6520 6769 7665 6e20 6675 6e63 7469 6f6e  e given function
-00002050: 206f 7220 6461 7461 6672 616d 6520 746f   or dataframe to
-00002060: 2069 742e 0a0a 2020 2020 2020 2020 4172   it...        Ar
-00002070: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00002080: 6172 6773 5f6d 6f64 656c 3a20 6120 6675  args_model: a fu
-00002090: 6e63 7469 6f6e 206f 7220 6461 7461 636c  nction or datacl
-000020a0: 6173 7320 6672 6f6d 2077 6869 6368 2074  ass from which t
-000020b0: 6f20 6465 7269 7665 2061 7267 756d 656e  o derive argumen
-000020c0: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
-000020d0: 6e61 6d65 3a20 6e61 6d65 206f 6620 7468  name: name of th
-000020e0: 6520 636f 6d6d 616e 640a 0a20 2020 2020  e command..     
-000020f0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00002100: 2020 2020 2020 2020 7468 6520 6e65 7720          the new 
-00002110: 6172 6770 6172 7365 2073 7562 7061 7273  argparse subpars
-00002120: 6572 0a0a 2020 2020 2020 2020 4578 616d  er..        Exam
-00002130: 706c 6573 3a0a 2020 2020 2020 2020 2020  ples:.          
-00002140: 2020 3e3e 3e20 696d 706f 7274 2079 6170    >>> import yap
-00002150: 780a 2020 2020 2020 2020 2020 2020 3e3e  x.            >>
-00002160: 3e20 6672 6f6d 2064 6174 6163 6c61 7373  > from dataclass
-00002170: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
-00002180: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
-00002190: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-000021a0: 3e3e 3e20 4064 6174 6163 6c61 7373 0a20  >>> @dataclass. 
-000021b0: 2020 2020 2020 2020 2020 202e 2e2e 2063             ... c
-000021c0: 6c61 7373 2041 6464 4e75 6d73 3a0a 2020  lass AddNums:.  
-000021d0: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
-000021e0: 2020 783a 2069 6e74 0a20 2020 2020 2020    x: int.       
-000021f0: 2020 2020 202e 2e2e 2020 2020 2079 3a20       ...     y: 
-00002200: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
-00002210: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-00002220: 3e3e 3e20 7061 7273 6572 203d 2079 6170  >>> parser = yap
-00002230: 782e 4172 6775 6d65 6e74 5061 7273 6572  x.ArgumentParser
-00002240: 2829 0a20 2020 2020 2020 2020 2020 203e  ().            >
-00002250: 3e3e 2073 7562 7061 7273 6572 5f31 203d  >> subparser_1 =
-00002260: 2070 6172 7365 722e 6164 645f 636f 6d6d   parser.add_comm
-00002270: 616e 6428 4164 644e 756d 732c 206e 616d  and(AddNums, nam
-00002280: 653d 2761 6464 2729 0a20 2020 2020 2020  e='add').       
-00002290: 2020 2020 203e 3e3e 2073 7562 7061 7273       >>> subpars
-000022a0: 6572 5f31 2e73 6574 5f64 6566 6175 6c74  er_1.set_default
-000022b0: 7328 5f63 6f6d 6d61 6e64 5f66 756e 633d  s(_command_func=
-000022c0: 6c61 6d62 6461 2078 2c20 793a 2078 2b79  lambda x, y: x+y
-000022d0: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
-000022e0: 3e20 7375 6270 6172 7365 725f 3220 3d20  > subparser_2 = 
-000022f0: 7061 7273 6572 2e61 6464 5f63 6f6d 6d61  parser.add_comma
-00002300: 6e64 2841 6464 4e75 6d73 2c20 6e61 6d65  nd(AddNums, name
-00002310: 3d27 7375 6274 7261 6374 2729 0a20 2020  ='subtract').   
-00002320: 2020 2020 2020 2020 203e 3e3e 2073 7562           >>> sub
-00002330: 7061 7273 6572 5f32 2e73 6574 5f64 6566  parser_2.set_def
-00002340: 6175 6c74 7328 5f63 6f6d 6d61 6e64 5f66  aults(_command_f
-00002350: 756e 633d 6c61 6d62 6461 2078 2c20 793a  unc=lambda x, y:
-00002360: 2078 2d79 290a 2020 2020 2020 2020 2020   x-y).          
-00002370: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
-00002380: 2020 3e3e 3e20 7061 7273 6564 203d 2070    >>> parsed = p
-00002390: 6172 7365 722e 7061 7273 655f 6172 6773  arser.parse_args
-000023a0: 285b 2761 6464 272c 2027 2d78 272c 2027  (['add', '-x', '
-000023b0: 3127 2c20 272d 7927 2c20 2732 275d 290a  1', '-y', '2']).
-000023c0: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
-000023d0: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-000023e0: 2870 6172 7365 642e 782c 2070 6172 7365  (parsed.x, parse
-000023f0: 642e 7929 0a20 2020 2020 2020 2020 2020  d.y).           
-00002400: 2028 312c 2032 290a 2020 2020 2020 2020   (1, 2).        
-00002410: 2020 2020 3e3e 3e20 7061 7273 6564 2e5f      >>> parsed._
-00002420: 636f 6d6d 616e 645f 6675 6e63 5f61 7267  command_func_arg
-00002430: 735f 6d6f 6465 6c28 783d 7061 7273 6564  s_model(x=parsed
-00002440: 2e78 2c20 793d 7061 7273 6564 2e79 290a  .x, y=parsed.y).
-00002450: 2020 2020 2020 2020 2020 2020 4164 644e              AddN
-00002460: 756d 7328 783d 312c 2079 3d32 290a 2020  ums(x=1, y=2).  
-00002470: 2020 2020 2020 2020 2020 3e3e 3e20 7061            >>> pa
-00002480: 7273 6564 2e5f 636f 6d6d 616e 645f 6675  rsed._command_fu
-00002490: 6e63 2878 3d70 6172 7365 642e 782c 2079  nc(x=parsed.x, y
-000024a0: 3d70 6172 7365 642e 7929 0a20 2020 2020  =parsed.y).     
-000024b0: 2020 2020 2020 2033 0a0a 2020 2020 2020         3..      
-000024c0: 2020 2020 2020 3e3e 3e20 696d 706f 7274        >>> import
-000024d0: 2079 6170 780a 2020 2020 2020 2020 2020   yapx.          
-000024e0: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
-000024f0: 2020 3e3e 3e20 6465 6620 6164 645f 6e75    >>> def add_nu
-00002500: 6d73 2878 3a20 696e 742c 2079 3a20 696e  ms(x: int, y: in
-00002510: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-00002520: 2e2e 2e20 2020 2020 7265 7475 726e 2078  ...     return x
-00002530: 202b 2079 0a20 2020 2020 2020 2020 2020   + y.           
-00002540: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-00002550: 203e 3e3e 2064 6566 2073 7562 7472 6163   >>> def subtrac
-00002560: 745f 6e75 6d73 2878 3a20 696e 742c 2079  t_nums(x: int, y
-00002570: 3a20 696e 7429 3a0a 2020 2020 2020 2020  : int):.        
-00002580: 2020 2020 2e2e 2e20 2020 2020 7265 7475      ...     retu
-00002590: 726e 2078 202d 2079 0a20 2020 2020 2020  rn x - y.       
-000025a0: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
-000025b0: 2020 2020 203e 3e3e 2070 6172 7365 7220       >>> parser 
-000025c0: 3d20 7961 7078 2e41 7267 756d 656e 7450  = yapx.ArgumentP
-000025d0: 6172 7365 7228 290a 2020 2020 2020 2020  arser().        
-000025e0: 2020 2020 3e3e 3e20 7375 6270 6172 7365      >>> subparse
-000025f0: 725f 3120 3d20 7061 7273 6572 2e61 6464  r_1 = parser.add
-00002600: 5f63 6f6d 6d61 6e64 2861 6464 5f6e 756d  _command(add_num
-00002610: 732c 206e 616d 653d 2761 6464 2729 0a20  s, name='add'). 
-00002620: 2020 2020 2020 2020 2020 203e 3e3e 2073             >>> s
-00002630: 7562 7061 7273 6572 5f31 2e73 6574 5f64  ubparser_1.set_d
-00002640: 6566 6175 6c74 7328 5f63 6f6d 6d61 6e64  efaults(_command
-00002650: 5f66 756e 633d 6164 645f 6e75 6d73 290a  _func=add_nums).
-00002660: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00002670: 7375 6270 6172 7365 725f 3220 3d20 7061  subparser_2 = pa
-00002680: 7273 6572 2e61 6464 5f63 6f6d 6d61 6e64  rser.add_command
-00002690: 2873 7562 7472 6163 745f 6e75 6d73 2c20  (subtract_nums, 
-000026a0: 6e61 6d65 3d27 7375 6274 7261 6374 2729  name='subtract')
-000026b0: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
-000026c0: 2073 7562 7061 7273 6572 5f32 2e73 6574   subparser_2.set
-000026d0: 5f64 6566 6175 6c74 7328 5f63 6f6d 6d61  _defaults(_comma
-000026e0: 6e64 5f66 756e 633d 7375 6274 7261 6374  nd_func=subtract
-000026f0: 5f6e 756d 7329 0a20 2020 2020 2020 2020  _nums).         
-00002700: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
-00002710: 2020 203e 3e3e 2070 6172 7365 6420 3d20     >>> parsed = 
-00002720: 7061 7273 6572 2e70 6172 7365 5f61 7267  parser.parse_arg
-00002730: 7328 5b27 7375 6274 7261 6374 272c 2027  s(['subtract', '
-00002740: 2d78 272c 2027 3127 2c20 272d 7927 2c20  -x', '1', '-y', 
-00002750: 2732 275d 290a 2020 2020 2020 2020 2020  '2']).          
-00002760: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
-00002770: 2020 3e3e 3e20 2870 6172 7365 642e 782c    >>> (parsed.x,
-00002780: 2070 6172 7365 642e 7929 0a20 2020 2020   parsed.y).     
-00002790: 2020 2020 2020 2028 312c 2032 290a 2020         (1, 2).  
-000027a0: 2020 2020 2020 2020 2020 3e3e 3e20 7061            >>> pa
-000027b0: 7273 6564 2e5f 636f 6d6d 616e 645f 6675  rsed._command_fu
-000027c0: 6e63 5f61 7267 735f 6d6f 6465 6c28 783d  nc_args_model(x=
-000027d0: 7061 7273 6564 2e78 2c20 793d 7061 7273  parsed.x, y=pars
-000027e0: 6564 2e79 290a 2020 2020 2020 2020 2020  ed.y).          
-000027f0: 2020 4461 7461 636c 6173 735f 7375 6274    Dataclass_subt
-00002800: 7261 6374 5f6e 756d 7328 783d 312c 2079  ract_nums(x=1, y
-00002810: 3d32 290a 2020 2020 2020 2020 2020 2020  =2).            
-00002820: 3e3e 3e20 7061 7273 6564 2e5f 636f 6d6d  >>> parsed._comm
-00002830: 616e 645f 6675 6e63 2878 3d70 6172 7365  and_func(x=parse
-00002840: 642e 782c 2079 3d70 6172 7365 642e 7929  d.x, y=parsed.y)
-00002850: 0a20 2020 2020 2020 2020 2020 202d 310a  .            -1.
-00002860: 2020 2020 2020 2020 7247 0000 004e fa01          rG...N..
-00002870: 20a9 0172 8f00 0000 7201 0000 0029 0272   ..r....r....).r
-00002880: 4700 0000 725a 0000 0029 0c72 7700 0000  G...rZ...).rw...
-00002890: 7224 0000 00da 085f 5f6e 616d 655f 5f72  r$.....__name__r
-000028a0: 6d00 0000 7274 0000 00da 115f 5375 6250  m...rt....._SubP
-000028b0: 6172 7365 7273 4163 7469 6f6e da03 706f  arsersAction..po
-000028c0: 70da 1f5f 6765 745f 6465 7363 7269 7074  p.._get_descript
-000028d0: 696f 6e5f 6672 6f6d 5f64 6f63 7374 7269  ion_from_docstri
-000028e0: 6e67 da0a 7370 6c69 746c 696e 6573 da0a  ng..splitlines..
-000028f0: 6164 645f 7061 7273 6572 7249 0000 0072  add_parserrI...r
-00002900: 9000 0000 2909 7278 0000 0072 8f00 0000  ....).rx...r....
-00002910: 7292 0000 0072 5100 0000 5a0a 7375 6270  r....rQ...Z.subp
-00002920: 6172 7365 7273 7247 0000 005a 0f64 6573  arsersrG...Z.des
-00002930: 6372 6970 7469 6f6e 5f74 7874 5a08 6865  cription_txtZ.he
-00002940: 6c70 5f74 7874 7266 0000 0072 5300 0000  lp_txtrf...rS...
-00002950: 7253 0000 0072 5700 0000 da0b 6164 645f  rS...rW.....add_
-00002960: 636f 6d6d 616e 6427 0100 0073 3400 0000  command'...s4...
-00002970: 083e 0402 0a01 1003 0c01 0401 0c01 0404  .>..............
-00002980: 0201 06ff 0403 0401 0c01 0402 0201 02ff  ................
-00002990: 0202 0201 04fd 0204 06fc 0406 0601 0402  ................
-000029a0: 0c01 0402 7a1a 4172 6775 6d65 6e74 5061  ....z.ArgumentPa
-000029b0: 7273 6572 2e61 6464 5f63 6f6d 6d61 6e64  rser.add_command
-000029c0: da04 6675 6e63 6303 0000 0000 0000 0000  ..funcc.........
-000029d0: 0000 0005 0000 0005 0000 004b 0000 0073  ...........K...s
-000029e0: 4200 0000 7400 7c02 7205 7c02 6e02 7c01  B...t.|.r.|.n.|.
-000029f0: 6a01 8301 7d02 7c00 6a02 7c01 6601 6401  j...}.|.j.|.f.d.
-00002a00: 7c02 6901 7c03 a401 8e01 7d04 7c04 6a03  |.i.|.....}.|.j.
-00002a10: 6402 6900 7c00 6a04 7c01 6901 a401 8e01  d.i.|.j.|.i.....
-00002a20: 0100 6400 5300 2903 4e72 9200 0000 7253  ..d.S.).Nr....rS
-00002a30: 0000 0029 0572 2400 0000 7295 0000 0072  ...).r$...r....r
-00002a40: 9b00 0000 da0c 7365 745f 6465 6661 756c  ......set_defaul
-00002a50: 7473 7245 0000 0029 0572 7800 0000 729c  tsrE...).rx...r.
-00002a60: 0000 0072 9200 0000 7251 0000 0072 6600  ...r....rQ...rf.
-00002a70: 0000 7253 0000 0072 5300 0000 7257 0000  ..rS...rS...rW..
-00002a80: 00da 115f 7265 6769 7374 6572 5f63 6f6d  ..._register_com
-00002a90: 6d61 6e64 8701 0000 7312 0000 0012 0604  mand....s.......
-00002aa0: 0102 0104 ff02 0202 fe02 0306 fd1a 057a  ...............z
-00002ab0: 2041 7267 756d 656e 7450 6172 7365 722e   ArgumentParser.
-00002ac0: 5f72 6567 6973 7465 725f 636f 6d6d 616e  _register_comman
-00002ad0: 64da 0464 636c 73da 0461 7474 7263 0200  d..dcls..attrc..
-00002ae0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-00002af0: 0000 4300 0000 730a 0000 007c 017c 006a  ..C...s....|.|.j
-00002b00: 0076 0153 0072 5c00 0000 a901 da0f 5f5f  .v.S.r\.......__
-00002b10: 616e 6e6f 7461 7469 6f6e 735f 5fa9 0272  annotations__..r
-00002b20: 9f00 0000 72a0 0000 0072 5300 0000 7253  ....r....rS...rS
-00002b30: 0000 0072 5700 0000 da17 5f69 735f 6174  ...rW....._is_at
-00002b40: 7472 6962 7574 655f 696e 6865 7269 7465  tribute_inherite
-00002b50: 6495 0100 0073 0200 0000 0a02 7a26 4172  d....s......z&Ar
-00002b60: 6775 6d65 6e74 5061 7273 6572 2e5f 6973  gumentParser._is
-00002b70: 5f61 7474 7269 6275 7465 5f69 6e68 6572  _attribute_inher
-00002b80: 6974 6564 7266 0000 0063 0300 0000 0000  itedrf...c......
-00002b90: 0000 0000 0000 1900 0000 0900 0000 0300  ................
-00002ba0: 0000 731c 0700 0074 007c 0283 0172 077c  ..s....t.|...r.|
-00002bb0: 0289 016e 0474 017c 0283 0189 017c 01a0  ...n.t.|.....|..
-00002bc0: 0288 006a 03a1 0172 1864 017d 037c 01a0  ...j...r.d.}.|..
-00002bd0: 047c 03a1 0101 007c 016a 0564 2469 0088  .|.....|.j.d$i..
-00002be0: 006a 0388 0169 01a4 018e 0101 0069 007d  .j...i.......i.}
-00002bf0: 0474 0674 0787 0087 0166 0264 0264 0384  .t.t.....f.d.d..
-00002c00: 0874 0888 0183 0183 0283 017d 0564 0464  .t.........}.d.d
-00002c10: 0584 007c 0544 0083 017d 0667 007d 077c  ...|.D...}.g.}.|
-00002c20: 0644 0090 035d 4c5c 027d 087d 097c 086a  .D...]L\.}.}.|.j
-00002c30: 097d 0a74 0a7c 0a74 0b83 0272 4f74 0c7c  .}.t.|.t...rOt.|
-00002c40: 0a83 017d 0a74 0a7c 0a74 0b83 0272 564a  ...}.t.|.t...rVJ
-00002c50: 0082 0174 0d6a 0e64 066b 0572 6074 0a7c  ...t.j.d.k.r`t.|
-00002c60: 0a74 0f83 0273 6788 00a0 107c 0aa1 0174  .t...sg....|...t
-00002c70: 1175 0072 6e88 006a 127c 0a64 0764 088d  .u.rn..j.|.d.d..
-00002c80: 027d 0a74 0a7c 0a74 1383 0272 a988 00a0  .}.t.|.t...r....
-00002c90: 147c 0aa1 0144 005d 137d 0b74 157c 0b74  .|...D.].}.t.|.t
-00002ca0: 1683 0272 8b74 177c 0b6a 1876 0072 8b7c  ...r.t.|.j.v.r.|
-00002cb0: 0b6a 1874 1719 007d 0901 006e 0171 7888  .j.t...}...n.qx.
-00002cc0: 00a0 107c 0aa1 017d 0a74 0d6a 0e64 066b  ...|...}.t.j.d.k
-00002cd0: 0572 9b74 0a7c 0a74 0f83 0273 a288 00a0  .r.t.|.t...s....
-00002ce0: 107c 0aa1 0174 1175 0072 a988 006a 127c  .|...t.u.r...j.|
-00002cf0: 0a64 0764 088d 027d 0a74 0a7c 0a74 0983  .d.d...}.t.|.t..
-00002d00: 0272 b17c 0a6a 196e 0a74 0b7c 0a83 016a  .r.|.j.n.t.|...j
-00002d10: 1a64 0964 0a64 0b8d 0264 0c19 007d 0c7c  .d.d.d...d...}.|
-00002d20: 09a0 1b7c 086a 1ca1 0101 007c 096a 1d72  ...|.j.....|.j.r
-00002d30: df7c 086a 1e74 1f75 0172 d27c 086a 1e7c  .|.j.t.u.r.|.j.|
-00002d40: 095f 1e64 0d7c 095f 1d6e 0d7c 086a 2074  ._.d.|._.n.|.j t
-00002d50: 1f75 0172 df7c 08a0 20a1 007c 095f 1e64  .u.r.|.. ..|._.d
-00002d60: 0d7c 095f 1d88 00a0 107c 0aa1 017d 0d7c  .|._.....|...}.|
-00002d70: 0d90 0172 847c 0d90 0172 037c 0d74 2175  ...r.|...r.|.t!u
-00002d80: 0090 0172 0374 0688 00a0 227c 0aa1 0183  ...r.t...."|....
-00002d90: 017c 095f 237c 096a 2390 0172 0274 097c  .|._#|.j#..r.t.|
-00002da0: 096a 2364 0e19 0083 017d 0a6e 8c74 247c  .j#d.....}.n.t$|
-00002db0: 0d74 256a 266a 2783 0290 0172 1a88 006a  .t%j&j'....r...j
-00002dc0: 127c 0a64 0764 0f8d 027d 0a7c 096a 2890  .|.d.d...}.|.j(.
-00002dd0: 0173 1974 297c 095f 286e 3574 247c 0d74  .s.t)|._(n5t$|.t
-00002de0: 256a 266a 2a83 0290 0173 277c 0d74 2b75  %j&j*....s'|.t+u
-00002df0: 0090 0172 4888 006a 127c 0a64 0764 0f8d  ...rH..j.|.d.d..
-00002e00: 027d 0a7c 096a 2890 0173 477c 0d74 2b75  .}.|.j(..sG|.t+u
-00002e10: 0090 0172 3b74 2c7c 095f 286e 147c 0d74  ...r;t,|._(n.|.t
-00002e20: 2d75 0090 0172 4474 2e7c 095f 286e 0b74  -u...rDt.|._(n.t
-00002e30: 2f7c 095f 286e 0774 3090 0173 4f74 317c  /|._(n.t0..sOt1|
-00002e40: 0a83 0101 0074 247c 0a74 3283 0290 0172  .....t$|.t2....r
-00002e50: 5d64 1064 0584 007c 0a44 0083 017c 095f  ]d.d...|.D...|._
-00002e60: 2374 157c 0188 0083 0290 0172 6c74 3374  #t.|.......rlt3t
-00002e70: 347c 0a83 027c 016a 357c 096a 363c 007c  4|...|.j5|.j6<.|
-00002e80: 096a 3790 0172 817c 096a 3864 0075 0090  .j7..r.|.j8d.u..
-00002e90: 0172 817c 096a 1d90 0172 7e64 117c 095f  .r.|.j...r~d.|._
-00002ea0: 386e 0364 127c 095f 3874 0b7d 0a6e 0b74  8n.d.|._8t.}.n.t
-00002eb0: 247c 0a74 3283 0290 0172 8f74 067c 0a83  $|.t2....r.t.|..
-00002ec0: 017c 095f 237c 0a7c 095f 097c 09a0 39a1  .|._#|.|._.|..9.
-00002ed0: 007d 0e7c 0e64 133d 007c 0ea0 3a64 14a1  .}.|.d.=.|..:d..
-00002ee0: 017d 0f7c 0f90 0173 a367 006e 0664 1564  .}.|...s.g.n.d.d
-00002ef0: 0584 007c 0f44 0083 017d 107c 0e64 1619  ...|.D...}.|.d..
-00002f00: 0090 0173 c67c 0ea0 3b64 17a1 0190 0173  ...s.|..;d.....s
-00002f10: c67c 1090 0173 c264 187c 0e64 1919 00a0  .|...s.d.|.d....
-00002f20: 3ca1 009b 0064 1a9d 036e 0164 1b7c 0e64  <....d...n.d.|.d
-00002f30: 163c 007c 0e64 1c19 007d 117c 1090 0173  .<.|.d...}.|...s
-00002f40: e77c 0e64 1c3d 007c 1190 0173 df7c 0ea0  .|.d.=.|...s.|..
-00002f50: 3b64 1da1 0164 0075 0090 0172 df64 1e7c  ;d...d.u...r.d.|
-00002f60: 0e64 1d3c 0074 3374 347c 0a83 027c 0e64  .d.<.t3t4|...|.d
-00002f70: 1f3c 006e 4c7c 096a 0974 3d75 0090 0272  .<.nL|.j.t=u...r
-00002f80: 1274 157c 0188 0083 0290 0172 fc74 3374  .t.|.......r.t3t
-00002f90: 347c 0a83 027c 016a 357c 096a 363c 0064  4|...|.j5|.j6<.d
-00002fa0: 2044 005d 097d 127c 0ea0 3a7c 1264 00a1   D.].}.|..:|.d..
-00002fb0: 0201 0090 0171 fe7c 0e64 2119 0090 0273  .....q.|.d!....s
-00002fc0: 1174 3e7c 0e64 213c 006e 217c 096a 3864  .t>|.d!<.n!|.j8d
-00002fd0: 0e6b 0390 0272 2074 3374 347c 0a83 027c  .k...r t3t4|...|
-00002fe0: 0e64 1f3c 006e 137c 0a74 3f75 0090 0272  .d.<.n.|.t?u...r
-00002ff0: 2a74 407c 0e64 213c 006e 097c 0a74 0b75  *t@|.d!<.n.|.t.u
-00003000: 0090 0272 3374 417c 0e64 213c 007c 086a  ...r3tA|.d!<.|.j
-00003010: 1e74 1f75 0190 0273 477c 086a 2074 1f75  .t.u...sG|.j t.u
-00003020: 0190 0273 477c 0ea0 3b64 22a1 0164 0075  ...sG|..;d"..d.u
-00003030: 0190 0272 de7c 0ea0 3b64 21a1 0190 0272  ...r.|..;d!....r
-00003040: 7a74 247c 0e64 2119 0074 426a 4374 3e66  zt$|.d!..tBjCt>f
-00003050: 0283 0290 0272 7a74 0964 2364 2469 0083  .....rzt.d#d$i..
-00003060: 0383 007d 137c 0e64 2119 007c 107c 0e64  ...}.|.d!..|.|.d
-00003070: 1919 0064 258d 027c 017c 137c 0e64 2219  ...d%..|.|.|.d".
-00003080: 0064 268d 0301 0074 447c 137c 0e64 1919  .d&....tD|.|.d..
-00003090: 0083 027c 0e64 223c 006e 0f64 1f7c 0e76  ...|.d"<.n.d.|.v
-000030a0: 0090 0272 897c 0e64 1f19 007c 0e64 2219  ...r.|.d...|.d".
-000030b0: 0083 017c 0e64 223c 007c 0ea0 3b64 17a1  ...|.d"<.|..;d..
-000030c0: 0190 0272 de7c 0e64 2219 007d 1474 0a7c  ...r.|.d"..}.t.|
-000030d0: 1474 0b83 0290 0273 a174 0a7c 1474 256a  .t.....s.t.|.t%j
-000030e0: 266a 2a83 0290 0273 a47c 1467 017d 147c  &j*....s.|.g.}.|
-000030f0: 1444 005d 377d 0b7c 0b7c 0e64 1719 0076  .D.]7}.|.|.d...v
-00003100: 0190 0272 dc74 0a7c 0b74 3283 0290 0272  ...r.t.|.t2....r
-00003110: bd7c 0b6a 1c7c 0e64 1719 0076 0190 0272  .|.j.|.d...v...r
-00003120: dc7c 0ea0 3b64 1ca1 0190 0273 c87c 0b64  .|..;d.....s.|.d
-00003130: 0075 0090 0273 dc64 277c 0b9b 0064 287c  .u...s.d'|...d(|
-00003140: 0e64 1919 009b 0064 297c 0e64 1719 009b  .d.....d)|.d....
-00003150: 009d 067d 037c 01a0 047c 03a1 0101 0090  ...}.|...|......
-00003160: 0271 a664 2a7c 0c9b 009d 0267 017d 157c  .q.d*|.....g.}.|
-00003170: 1190 0273 fb74 157c 0ea0 3b64 22a1 0174  ...s.t.|..;d"..t
-00003180: 0b83 0290 0272 f67c 15a0 4564 2ba1 0101  .....r.|..Ed+...
-00003190: 006e 057c 15a0 4564 2ca1 0101 007c 0ea0  .n.|..Ed,....|..
-000031a0: 3a64 2d64 0da1 0290 0372 077c 15a0 4564  :d-d.....r.|..Ed
-000031b0: 2ea1 0101 007c 096a 4690 0372 147c 15a0  .....|.jF..r.|..
-000031c0: 4564 2f7c 096a 469b 009d 02a1 0101 0064  Ed/|.jF........d
-000031d0: 3064 31a0 477c 15a1 019b 009d 027d 167c  0d1.G|.......}.|
-000031e0: 0ea0 3b64 32a1 0190 0372 2d7c 0e64 3205  ..;d2....r-|.d2.
-000031f0: 0019 0064 337c 1617 0037 0003 003c 006e  ...d3|...7...<.n
-00003200: 047c 167c 0e64 323c 007c 0ea0 3a64 3464  .|.|.d2<.|..:d4d
-00003210: 00a1 027d 177c 1790 0373 417c 1190 0372  ...}.|...sA|...r
-00003220: 3f64 356e 0164 367d 177c 04a0 3b7c 1764  ?d5n.d6}.|..;|.d
-00003230: 00a1 027d 187c 1890 0373 537c 01a0 487c  ...}.|...sS|..H|
-00003240: 17a1 017d 187c 187c 047c 173c 007c 096a  ...}.|.|.|.<.|.j
-00003250: 4990 0372 7e7c 1190 0372 6564 377c 096a  I..r~|...red7|.j
-00003260: 369b 009d 027d 037c 01a0 047c 03a1 0101  6....}.|...|....
-00003270: 007c 016a 4a7c 016a 4ba0 3b88 006a 4ca1  .|.jJ|.jK.;..jL.
-00003280: 0119 007c 1719 00a0 457c 096a 367c 1090  ...|....E|.j6|..
-00003290: 0372 7a7c 1064 0c19 006e 0164 0066 02a1  .rz|.d...n.d.f..
-000032a0: 0101 007c 186a 4d7c 1069 007c 0ea4 018e  ...|.jM|.i.|....
-000032b0: 0101 007c 07a0 457c 09a1 0101 0071 3e7c  ...|..E|.....q>|
-000032c0: 0753 0029 384e 7a3e 5468 6973 2070 6172  .S.)8Nz>This par
-000032d0: 7365 7220 616c 7265 6164 7920 636f 6e74  ser already cont
-000032e0: 6169 6e73 2061 7267 756d 656e 7473 2066  ains arguments f
-000032f0: 726f 6d20 616e 6f74 6865 7220 6461 7461  rom another data
-00003300: 636c 6173 732e 6301 0000 0000 0000 0000  class.c.........
-00003310: 0000 0001 0000 0004 0000 0013 0000 0073  ...............s
-00003320: 1200 0000 8800 6a00 8801 7c00 6a01 6401  ......j...|.j.d.
-00003330: 8d02 0c00 5300 2902 4e72 a300 0000 2902  ....S.).Nr....).
-00003340: 72a4 0000 0072 9200 0000 2901 da01 66a9  r....r....)...f.
-00003350: 02da 0363 6c73 5a05 6d6f 6465 6c72 5300  ...clsZ.modelrS.
-00003360: 0000 7257 0000 0072 5e00 0000 b201 0000  ..rW...r^.......
-00003370: f302 0000 0012 007a 2f41 7267 756d 656e  .......z/Argumen
-00003380: 7450 6172 7365 722e 5f61 6464 5f61 7267  tParser._add_arg
-00003390: 756d 656e 7473 2e3c 6c6f 6361 6c73 3e2e  uments.<locals>.
-000033a0: 3c6c 616d 6264 613e 6301 0000 0000 0000  <lambda>c.......
-000033b0: 0000 0000 0002 0000 0007 0000 0053 0000  .............S..
-000033c0: 0073 2000 0000 6700 7c00 5d0c 7d01 7c01  .s ...g.|.].}.|.
-000033d0: 7c01 6a00 a001 7402 7403 8300 a102 6602  |.j...t.t.....f.
-000033e0: 9102 7102 5300 7253 0000 0029 04da 086d  ..q.S.rS...)...m
-000033f0: 6574 6164 6174 61da 0367 6574 7221 0000  etadata..getr!..
-00003400: 0072 2200 0000 7254 0000 0072 5300 0000  .r"...rT...rS...
-00003410: 7253 0000 0072 5700 0000 7258 0000 00b7  rS...rW...rX....
-00003420: 0100 0073 0800 0000 0600 0202 12ff 06ff  ...s............
-00003430: 7a31 4172 6775 6d65 6e74 5061 7273 6572  z1ArgumentParser
-00003440: 2e5f 6164 645f 6172 6775 6d65 6e74 732e  ._add_arguments.
-00003450: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00003460: 6d70 3e72 3d00 0000 5429 01da 0d69 735f  mp>r=...T)...is_
-00003470: 756e 696f 6e5f 7479 7065 da01 2e72 1700  union_type...r..
-00003480: 0000 a901 da08 6d61 7873 706c 6974 e9ff  ......maxsplit..
-00003490: ffff ff46 7201 0000 0029 01da 1061 7373  ...Fr....)...ass
-000034a0: 6572 745f 7072 696d 6974 6976 6563 0100  ert_primitivec..
-000034b0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-000034c0: 0000 5300 0000 7312 0000 0067 007c 005d  ..S...s....g.|.]
-000034d0: 057d 017c 016a 0091 0271 0253 0072 5300  .}.|.j...q.S.rS.
-000034e0: 0000 a901 7292 0000 0072 5400 0000 7253  ....r....rT...rS
-000034f0: 0000 0072 5300 0000 7257 0000 0072 5800  ...rS...rW...rX.
-00003500: 0000 1302 0000 72a8 0000 00fa 012b da01  ......r......+..
-00003510: 2ada 0370 6f73 7267 0000 0063 0100 0000  *..posrg...c....
-00003520: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00003530: 5300 0000 731a 0000 0067 007c 005d 097d  S...s....g.|.].}
-00003540: 017c 01a0 0064 00a1 0172 027c 0191 0271  .|...d...r.|...q
-00003550: 0253 0029 0172 6500 0000 725f 0000 0072  .S.).re...r_...r
-00003560: 5400 0000 7253 0000 0072 5300 0000 7257  T...rS...rS...rW
-00003570: 0000 0072 5800 0000 3302 0000 7302 0000  ...rX...3...s...
-00003580: 001a 00da 076d 6574 6176 6172 7264 0000  .....metavarrd..
-00003590: 00fa 013c da04 6465 7374 fa01 3e7a 073c  ...<..dest..>z.<
-000035a0: 7661 6c75 653e da08 7265 7175 6972 6564  value>..required
-000035b0: da05 6e61 7267 73fa 013f da04 7479 7065  ..nargs..?..type
-000035c0: 2905 72bc 0000 0072 ba00 0000 da05 636f  ).r....r......co
-000035d0: 6e73 7472 6400 0000 72b5 0000 0072 5900  nstrd...r....rY.
-000035e0: 0000 7263 0000 00da 0072 5300 0000 2902  ..rc.....rS...).
-000035f0: 7267 0000 0072 b700 0000 2903 7266 0000  rg...r....).rf..
-00003600: 00da 096e 616d 6573 7061 6365 da06 7661  ...namespace..va
-00003610: 6c75 6573 7a0f 496e 7661 6c69 6420 7661  luesz.Invalid va
-00003620: 6c75 6520 277a 1027 2066 6f72 2061 7267  lue 'z.' for arg
-00003630: 756d 656e 7420 277a 1327 3b20 6d75 7374  ument 'z.'; must
-00003640: 2062 6520 6f6e 6520 6f66 3a20 7a06 5479   be one of: z.Ty
-00003650: 7065 3a20 7a16 4465 6661 756c 743a 2022  pe: z.Default: "
-00003660: 2528 6465 6661 756c 7429 7322 7a14 4465  %(default)s"z.De
-00003670: 6661 756c 743a 2025 2864 6566 6175 6c74  fault: %(default
-00003680: 2973 da09 6578 636c 7573 6976 657a 044d  )s..exclusivez.M
-00003690: 2e58 2e7a 0545 6e76 3a20 7a02 3e20 fa02  .X.z.Env: z.> ..
-000036a0: 2c20 725a 0000 0072 7d00 0000 da05 6772  , rZ...r}.....gr
-000036b0: 6f75 707a 1372 6571 7569 7265 6420 7061  oupz.required pa
-000036c0: 7261 6d65 7465 7273 7a13 6f70 7469 6f6e  rametersz.option
-000036d0: 616c 2070 6172 616d 6574 6572 737a 3341  al parametersz3A
-000036e0: 206d 7574 7561 6c6c 792d 6578 636c 7573   mutually-exclus
-000036f0: 6976 6520 7061 7261 6d65 7465 7220 6361  ive parameter ca
-00003700: 6e6e 6f74 2062 6520 7265 7175 6972 6564  nnot be required
-00003710: 3a20 294e 7234 0000 0072 2500 0000 da0b  : )Nr4...r%.....
-00003720: 6765 745f 6465 6661 756c 7472 4600 0000  get_defaultrF...
-00003730: 7282 0000 0072 9d00 0000 725d 0000 00da  r....r....r]....
-00003740: 0666 696c 7465 7272 0600 0000 72bc 0000  .filterr....r...
-00003750: 0072 3800 0000 726e 0000 0072 2300 0000  .r8...rn...r#...
-00003760: 727f 0000 00da 0c76 6572 7369 6f6e 5f69  r......version_i
-00003770: 6e66 6f72 3f00 0000 da10 5f67 6574 5f74  nfor?....._get_t
-00003780: 7970 655f 6f72 6967 696e 7215 0000 00da  ype_originr.....
-00003790: 1c5f 6578 7472 6163 745f 7479 7065 5f66  ._extract_type_f
-000037a0: 726f 6d5f 636f 6e74 6169 6e65 7272 3c00  rom_containerr<.
-000037b0: 0000 da12 5f67 6574 5f74 7970 655f 6d65  ...._get_type_me
-000037c0: 7461 6461 7461 726d 0000 0072 0500 0000  tadatarm...r....
-000037d0: 7221 0000 0072 a900 0000 7295 0000 00da  r!...r....r.....
-000037e0: 0672 7370 6c69 74da 0873 6574 5f64 6573  .rsplit..set_des
-000037f0: 7472 9200 0000 72b9 0000 0072 6300 0000  tr....r....rc...
-00003800: 7204 0000 00da 0f64 6566 6175 6c74 5f66  r......default_f
-00003810: 6163 746f 7279 722a 0000 00da 0e5f 6765  actoryr*....._ge
-00003820: 745f 7479 7065 5f61 7267 7372 6400 0000  t_type_argsrd...
-00003830: 7239 0000 00da 0b63 6f6c 6c65 6374 696f  r9.....collectio
-00003840: 6e73 da03 6162 63da 074d 6170 7069 6e67  ns..abc..Mapping
-00003850: 7259 0000 0072 1d00 0000 da08 4974 6572  rY...r......Iter
-00003860: 6162 6c65 da03 7365 7472 1f00 0000 da05  able..setr......
-00003870: 7475 706c 6572 2000 0000 721e 0000 0072  tupler ...r....r
-00003880: 3500 0000 7227 0000 0072 0700 0000 7208  5...r'...r....r.
-00003890: 0000 0072 3100 0000 7272 0000 0072 b700  ...r1...rr...r..
-000038a0: 0000 72b4 0000 0072 ba00 0000 da06 6173  ..r....r......as
-000038b0: 6469 6374 7297 0000 0072 aa00 0000 da05  dictr....r......
-000038c0: 7570 7065 72da 0462 6f6f 6c72 1800 0000  upper..boolr....
-000038d0: da03 696e 7472 1900 0000 721a 0000 0072  ..intr....r....r
-000038e0: 7400 0000 da06 4163 7469 6f6e da07 6765  t.....Action..ge
-000038f0: 7461 7474 72da 0661 7070 656e 64da 085f  tattr..append.._
-00003900: 656e 765f 7661 72da 046a 6f69 6eda 1261  env_var..join..a
-00003910: 6464 5f61 7267 756d 656e 745f 6772 6f75  dd_argument_grou
-00003920: 7072 c100 0000 7271 0000 00da 095f 6465  pr....rq....._de
-00003930: 6661 756c 7473 7245 0000 0072 6f00 0000  faultsrE...ro...
-00003940: 2919 72a7 0000 0072 6600 0000 728f 0000  ).r....rf...r...
-00003950: 00da 0365 7272 5a11 7061 7273 6572 5f61  ...errZ.parser_a
-00003960: 7267 5f67 726f 7570 735a 0c6e 6f76 656c  rg_groupsZ.novel
-00003970: 5f66 6965 6c64 735a 106e 6f76 656c 5f66  _fieldsZ.novel_f
-00003980: 6965 6c64 5f61 7267 735a 0a61 6464 6564  ield_argsZ.added
-00003990: 5f61 7267 735a 0366 6c64 5a11 6172 6770  _argsZ.fldZ.argp
-000039a0: 6172 7365 5f61 7267 756d 656e 74da 0866  arse_argument..f
-000039b0: 6c64 5f74 7970 6572 5600 0000 5a09 6865  ld_typerV...Z.he
-000039c0: 6c70 5f74 7970 655a 0f66 6c64 5f74 7970  lp_typeZ.fld_typ
-000039d0: 655f 6f72 6967 696e 7251 0000 0072 6700  e_originrQ...rg.
-000039e0: 0000 7250 0000 0072 b900 0000 da01 6b5a  ..rP...r......kZ
-000039f0: 0f64 756d 6d79 5f6e 616d 6573 7061 6365  .dummy_namespace
-00003a00: da01 645a 0e68 656c 705f 6d73 675f 7061  ..dZ.help_msg_pa
-00003a10: 7274 735a 0868 656c 705f 6d73 6772 c300  rtsZ.help_msgr..
-00003a20: 0000 5a09 6172 675f 6772 6f75 7072 5300  ..Z.arg_grouprS.
-00003a30: 0000 72a6 0000 0072 5700 0000 7290 0000  ..r....rW...r...
-00003a40: 0099 0100 0073 a401 0000 080a 0601 0802  .....s..........
-00003a50: 0c02 0401 0a01 1602 0402 0202 0201 0c01  ................
-00003a60: 0601 02fe 04ff 0607 0202 06fe 0405 0e02  ................
-00003a70: 0601 0a04 0801 0e01 1403 0e01 0401 0201  ................
-00003a80: 0201 06fe 0a05 0e01 1401 0a01 0401 0280  ................
-00003a90: 0a02 1403 0e01 0401 0201 0201 06fe 0807  ................
-00003aa0: 08ff 1402 02fd 0c06 0602 0a01 0801 0801  ................
-00003ab0: 0a01 0a01 0601 0a02 0601 1001 1001 0801  ................
-00003ac0: 0e01 0280 1003 0401 0201 0201 06fe 0804  ................
-00003ad0: 0601 0280 0c03 04ff 0a02 0402 0201 0201  ................
-00003ae0: 06fe 0804 0a01 0801 0a01 0801 0602 0280  ................
-00003af0: 0602 0801 0c02 1001 0c02 0203 0201 0201  ................
-00003b00: 0cfe 1405 0801 0801 0602 0604 0c02 0a01  ................
-00003b10: 0602 0802 0601 0a02 0203 08ff 0c02 02fd  ................
-00003b20: 1606 1c02 06ff 0804 0602 0602 1601 0801  ................
-00003b30: 1001 0c01 0c01 0203 0201 0201 0cfe 0805  ................
-00003b40: 1001 0a01 0801 0280 0c02 1001 0a01 0a02  ................
-00003b50: 0a01 0802 0c04 0c01 1001 0e02 0601 0801  ................
-00003b60: 06fe 0e05 1201 0201 0201 0601 06fd 1405  ................
-00003b70: 0a01 1401 0c03 0801 0e01 0201 0601 06fe  ................
-00003b80: 0604 0802 0e02 0802 04fe 1003 0803 04fd  ................
-00003b90: 0a03 1203 0601 04ff 02ff 0a04 0480 0c02  ................
-00003ba0: 0603 1201 0c01 0a02 0e02 0a01 0802 1201  ................
-00003bb0: 1002 0c02 1601 0802 0c02 0602 0e01 0c02  ................
-00003bc0: 0602 0a01 0801 0802 0601 0202 0401 04ff  ................
-00003bd0: 02ff 0a04 0402 0c01 02ff 0202 02fe 0202  ................
-00003be0: 0402 1001 02fe 04ff 1007 0c02 0402 7a1d  ..............z.
-00003bf0: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
-00003c00: 6164 645f 6172 6775 6d65 6e74 73da 0174  add_arguments..t
-00003c10: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00003c20: 0004 0000 0043 0000 0073 0c00 0000 7400  .....C...s....t.
-00003c30: 7c00 6401 6400 8303 5300 2902 4eda 0a5f  |.d.d...S.).N.._
-00003c40: 5f6f 7269 6769 6e5f 5fa9 0172 d900 0000  _origin__..r....
-00003c50: a901 72e3 0000 0072 5300 0000 7253 0000  ..r....rS...rS..
-00003c60: 0072 5700 0000 72c7 0000 00c0 0200 00f3  .rW...r.........
-00003c70: 0200 0000 0c02 7a1f 4172 6775 6d65 6e74  ......z.Argument
-00003c80: 5061 7273 6572 2e5f 6765 745f 7479 7065  Parser._get_type
-00003c90: 5f6f 7269 6769 6e63 0100 0000 0000 0000  _originc........
-00003ca0: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
-00003cb0: f30c 0000 0074 007c 0064 0164 0283 0353  .....t.|.d.d...S
-00003cc0: 0029 034e da08 5f5f 6172 6773 5f5f 7253  .).N..__args__rS
-00003cd0: 0000 0072 e500 0000 72e6 0000 0072 5300  ...r....r....rS.
-00003ce0: 0000 7253 0000 0072 5700 0000 72cd 0000  ..rS...rW...r...
-00003cf0: 00c4 0200 0072 e700 0000 7a1d 4172 6775  .....r....z.Argu
-00003d00: 6d65 6e74 5061 7273 6572 2e5f 6765 745f  mentParser._get_
-00003d10: 7479 7065 5f61 7267 7363 0100 0000 0000  type_argsc......
-00003d20: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
-00003d30: 0000 72e8 0000 0029 034e da0c 5f5f 6d65  ..r....).N..__me
-00003d40: 7461 6461 7461 5f5f 7253 0000 0072 e500  tadata__rS...r..
-00003d50: 0000 72e6 0000 0072 5300 0000 7253 0000  ..r....rS...rS..
-00003d60: 0072 5700 0000 72c9 0000 00c8 0200 0072  .rW...r........r
-00003d70: e700 0000 7a21 4172 6775 6d65 6e74 5061  ....z!ArgumentPa
-00003d80: 7273 6572 2e5f 6765 745f 7479 7065 5f6d  rser._get_type_m
-00003d90: 6574 6164 6174 61da 0e74 7970 655f 636f  etadata..type_co
-00003da0: 6e74 6169 6e65 7272 b000 0000 72ab 0000  ntainerr....r...
-00003db0: 0063 0400 0000 0000 0000 0000 0000 0b00  .c..............
-00003dc0: 0000 0300 0000 4300 0000 7318 0100 007c  ......C...s....|
-00003dd0: 0372 0474 006e 047c 00a0 017c 01a1 017d  .r.t.n.|...|...}
-00003de0: 047c 0464 0075 0072 1574 0264 017c 016a  .|.d.u.r.t.d.|.j
-00003df0: 039b 009d 0283 0182 017c 00a0 047c 01a1  .........|...|..
-00003e00: 017d 0564 0264 0384 007c 0544 0083 017d  .}.d.d...|.D...}
-00003e10: 067c 0474 0075 0073 3074 057c 0474 066a  .|.t.u.s0t.|.t.j
-00003e20: 076a 0883 0273 307c 0474 0975 0072 4074  .j...s0|.t.u.r@t
-00003e30: 0a7c 0683 0164 046b 0372 3b7c 06a0 0ba1  .|...d.k.r;|....
-00003e40: 0001 006e 2c7c 0664 0519 007d 076e 2774  ...n,|.d...}.n't
-00003e50: 057c 0474 066a 076a 0c83 0272 6174 0a7c  .|.t.j.j...rat.|
-00003e60: 0683 0164 066b 0372 527c 06a0 0ba1 0001  ...d.k.rR|......
-00003e70: 006e 157c 065c 027d 087d 097c 0874 0d75  .n.|.\.}.}.|.t.u
-00003e80: 0172 5e74 0264 0783 0182 017c 097d 076e  .r^t.d.....|.}.n
-00003e90: 0674 0e73 6774 0f7c 0183 0101 007c 0673  .t.sgt.|.....|.s
-00003ea0: 6d74 0264 0883 0182 017c 00a0 017c 07a1  mt.d.....|...|..
-00003eb0: 017d 0a7c 0a74 0075 0072 807c 00a0 107c  .}.|.t.u.r.|...|
-00003ec0: 07a1 017d 077c 00a0 017c 07a1 017d 0a7c  ...}.|...|...}.|
-00003ed0: 0272 8a7c 0a72 8a74 0e73 8a74 0f7c 0a83  .r.|.r.t.s.t.|..
-00003ee0: 0101 007c 0753 0029 094e 7a1f 4769 7665  ...|.S.).Nz.Give
-00003ef0: 6e20 7479 7065 2069 7320 6e6f 7420 6120  n type is not a 
-00003f00: 636f 6e74 6169 6e65 723a 2063 0100 0000  container: c....
-00003f10: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00003f20: 5300 0000 7320 0000 0067 007c 005d 0c7d  S...s ...g.|.].}
-00003f30: 017c 0164 0075 0172 027c 0174 0075 0172  .|.d.u.r.|.t.u.r
-00003f40: 027c 0191 0271 0253 0029 012e 2901 722b  .|...q.S.)..).r+
-00003f50: 0000 0029 0272 5500 0000 da01 6172 5300  ...).rU.....arS.
-00003f60: 0000 7253 0000 0072 5700 0000 7258 0000  ..rS...rW...rX..
-00003f70: 00de 0200 0073 0400 0000 0600 1a01 7a3f  .....s........z?
-00003f80: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
-00003f90: 6578 7472 6163 745f 7479 7065 5f66 726f  extract_type_fro
-00003fa0: 6d5f 636f 6e74 6169 6e65 722e 3c6c 6f63  m_container.<loc
-00003fb0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
-00003fc0: 1700 0000 7201 0000 0072 7c00 0000 7a22  ....r....r|...z"
-00003fd0: 4469 6374 696f 6e61 7279 206b 6579 7320  Dictionary keys 
-00003fe0: 6d75 7374 2062 6520 7479 7065 2060 7374  must be type `st
-00003ff0: 7260 7a1b 546f 6f20 6d61 6e79 2074 7970  r`z.Too many typ
-00004000: 6573 2069 6e20 636f 6e74 6169 6e65 7229  es in container)
-00004010: 1172 1500 0000 72c7 0000 00da 0954 7970  .r....r......Typ
-00004020: 6545 7272 6f72 7295 0000 0072 cd00 0000  eErrorr....r....
-00004030: 7239 0000 0072 ce00 0000 72cf 0000 0072  r9...r....r....r
-00004040: 1100 0000 72d2 0000 0072 7600 0000 da05  ....r....rv.....
-00004050: 636c 6561 7272 d000 0000 726e 0000 0072  clearr....rn...r
-00004060: 3500 0000 7227 0000 0072 c800 0000 290b  5...r'...r....).
-00004070: 72a7 0000 0072 eb00 0000 72b0 0000 0072  r....r....r....r
-00004080: ab00 0000 5a15 7479 7065 5f63 6f6e 7461  ....Z.type_conta
-00004090: 696e 6572 5f6f 7269 6769 6e5a 1374 7970  iner_originZ.typ
-000040a0: 655f 636f 6e74 6169 6e65 725f 6172 6773  e_container_args
-000040b0: da07 7265 7375 6c74 735a 1674 7970 655f  ..resultsZ.type_
-000040c0: 636f 6e74 6169 6e65 725f 7375 6274 7970  container_subtyp
-000040d0: 655a 086b 6579 5f74 7970 655a 0a76 616c  eZ.key_typeZ.val
-000040e0: 7565 5f74 7970 655a 1d74 7970 655f 636f  ue_typeZ.type_co
-000040f0: 6e74 6169 6e65 725f 7375 6274 7970 655f  ntainer_subtype_
-00004100: 6f72 6967 696e 7253 0000 0072 5300 0000  originrS...rS...
-00004110: 7257 0000 0072 c800 0000 cc02 0000 7354  rW...r........sT
-00004120: 0000 0010 0802 ff08 0402 010a 0104 ff0a  ................
-00004130: 0406 0202 0106 ff08 070c 0102 ff08 020c  ................
-00004140: 020a 010a 020e 010c 010a 0108 0208 0108  ................
-00004150: 0106 0104 0108 0104 0208 010a 0208 0204  ................
-00004160: 0102 0104 ff0a 0302 0302 ff02 0202 fe02  ................
-00004170: 0302 fd08 0504 027a 2b41 7267 756d 656e  .......z+Argumen
-00004180: 7450 6172 7365 722e 5f65 7874 7261 6374  tParser._extract
-00004190: 5f74 7970 655f 6672 6f6d 5f63 6f6e 7461  _type_from_conta
-000041a0: 696e 6572 6301 0000 0000 0000 0000 0000  inerc...........
-000041b0: 0002 0000 0006 0000 000b 0000 0073 6400  .............sd.
-000041c0: 0000 7c01 a000 6401 6402 a102 7c01 6401  ..|...d.d...|.d.
-000041d0: 3c00 7c01 a000 6403 6404 a102 7c01 6403  <.|...d.d...|.d.
-000041e0: 3c00 7c01 a000 6405 8800 6a01 a102 7c01  <.|...d...j...|.
-000041f0: 6405 3c00 7c01 a000 6406 8700 6601 6407  d.<.|...d...f.d.
-00004200: 6408 8408 a102 7c01 6406 3c00 7402 8300  d.....|.d.<.t...
-00004210: 6a03 6409 6900 7c01 a401 8e01 8800 5f04  j.d.i.|......._.
-00004220: 8800 6a04 5300 290a 4e72 6c00 0000 5a08  ..j.S.).Nrl...Z.
-00004230: 636f 6d6d 616e 6473 72b5 0000 007a 093c  commandsr....z.<
-00004240: 434f 4d4d 414e 443e 72b7 0000 00da 0c70  COMMAND>r......p
-00004250: 6172 7365 725f 636c 6173 7363 0000 0000  arser_classc....
-00004260: 0000 0000 0000 0000 0100 0000 0600 0000  ................
-00004270: 1b00 0000 731e 0000 0074 0088 0083 0164  ....s....t.....d
-00004280: 0369 007c 00a4 0164 0188 006a 0164 029c  .i.|...d...j.d..
-00004290: 02a4 018e 0153 0029 044e 5429 0272 4f00  .....S.).NT).rO.
-000042a0: 0000 724e 0000 0072 5300 0000 2902 72bc  ..rN...rS...).r.
-000042b0: 0000 0072 4e00 0000 2901 72e1 0000 00a9  ...rN...).r.....
-000042c0: 0172 7800 0000 7253 0000 0072 5700 0000  .rx...rS...rW...
-000042d0: 725e 0000 0012 0300 0073 0c00 0000 0a00  r^.......s......
-000042e0: 0201 02ff 0202 0401 0afd 7a2f 4172 6775  ..........z/Argu
-000042f0: 6d65 6e74 5061 7273 6572 2e61 6464 5f73  mentParser.add_s
-00004300: 7562 7061 7273 6572 732e 3c6c 6f63 616c  ubparsers.<local
-00004310: 733e 2e3c 6c61 6d62 6461 3e72 5300 0000  s>.<lambda>rS...
-00004320: 2905 72aa 0000 0072 4400 0000 7268 0000  ).r....rD...rh..
-00004330: 00da 0e61 6464 5f73 7562 7061 7273 6572  ...add_subparser
-00004340: 7372 6a00 0000 2902 7278 0000 0072 5100  srj...).rx...rQ.
-00004350: 0000 7279 0000 0072 f100 0000 7257 0000  ..ry...r....rW..
-00004360: 0072 f200 0000 0c03 0000 7312 0000 0010  .r........s.....
-00004370: 0110 0112 0104 0102 010a 0108 fe14 0906  ................
-00004380: 027a 1d41 7267 756d 656e 7450 6172 7365  .z.ArgumentParse
-00004390: 722e 6164 645f 7375 6270 6172 7365 7273  r.add_subparsers
-000043a0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000043b0: 0004 0000 0043 0000 0073 2c00 0000 7c00  .....C...s,...|.
-000043c0: 6a00 4400 5d10 7d01 7401 7c01 7402 6a03  j.D.].}.t.|.t.j.
-000043d0: 8302 7213 7c01 7c00 5f04 7c00 6a04 0200  ..r.|.|._.|.j...
-000043e0: 0100 5300 7103 6400 5300 725c 0000 0029  ..S.q.d.S.r\...)
-000043f0: 05da 085f 6163 7469 6f6e 7372 6d00 0000  ..._actionsrm...
-00004400: 7274 0000 0072 9600 0000 726a 0000 0029  rt...r....rj...)
-00004410: 0272 7800 0000 72ec 0000 0072 5300 0000  .rx...r....rS...
-00004420: 7253 0000 0072 5700 0000 728c 0000 001d  rS...rW...r.....
-00004430: 0300 0073 1200 0000 0a01 0201 0201 0401  ...s............
-00004440: 04fe 0604 0a01 02fb 0406 7a26 4172 6775  ..........z&Argu
-00004450: 6d65 6e74 5061 7273 6572 2e5f 6669 6e64  mentParser._find
-00004460: 5f73 7562 7061 7273 6572 735f 6163 7469  _subparsers_acti
-00004470: 6f6e 6301 0000 0000 0000 0000 0000 0001  onc.............
-00004480: 0000 0002 0000 0043 0000 0073 3600 0000  .......C...s6...
-00004490: 7c00 6a00 6400 7501 7208 7c00 6a00 5300  |.j.d.u.r.|.j.S.
-000044a0: 7c00 6a01 7217 7c00 a002 a100 0100 7c00  |.j.r.|.......|.
-000044b0: 6a00 7314 4a00 8201 7c00 6a00 5300 7c00  j.s.J...|.j.S.|.
-000044c0: a003 a100 5300 725c 0000 0029 0472 6a00  ....S.r\...).rj.
-000044d0: 0000 728b 0000 0072 8c00 0000 72f2 0000  ..r....r....r...
-000044e0: 0072 f100 0000 7253 0000 0072 5300 0000  .r....rS...rS...
-000044f0: 7257 0000 0072 7700 0000 2703 0000 730e  rW...rw...'...s.
-00004500: 0000 000a 0106 0106 0208 010a 0106 0108  ................
-00004510: 027a 2541 7267 756d 656e 7450 6172 7365  .z%ArgumentParse
-00004520: 722e 5f67 6574 5f6f 725f 6164 645f 7375  r._get_or_add_su
-00004530: 6270 6172 7365 7273 72bf 0000 0063 0200  bparsersr....c..
-00004540: 0000 0000 0000 0000 0000 0600 0000 0600  ................
-00004550: 0000 0300 0000 736e 0000 007c 006a 00a0  ......sn...|.j..
-00004560: 0174 0288 007c 006a 0364 0083 0369 00a1  .t...|.j.d...i..
-00004570: 027d 027c 02a0 04a1 0044 005d 1d7d 0387  .}.|.....D.].}..
-00004580: 0066 0164 0164 0284 087c 0344 0083 017d  .f.d.d...|.D...}
-00004590: 0474 057c 0483 0164 036b 0472 2d64 0464  .t.|...d.k.r-d.d
-000045a0: 05a0 067c 04a1 0117 007d 057c 00a0 077c  ...|.....}.|...|
-000045b0: 05a1 0101 0071 1074 0864 0669 0074 0988  .....q.t.d.i.t..
-000045c0: 0083 01a4 018e 0153 0029 074e 6301 0000  .......S.).Nc...
-000045d0: 0000 0000 0000 0000 0004 0000 0005 0000  ................
-000045e0: 0013 0000 0073 6c00 0000 6700 7c00 5d32  .....sl...g.|.]2
-000045f0: 5c02 7d01 7d02 7400 8800 7c01 8302 7234  \.}.}.t...|...r4
-00004600: 7401 8800 7c01 8302 7d03 7402 7c03 7403  t...|...}.t.|.t.
-00004610: 8302 731c 7402 7c03 7404 6a05 6a06 8302  ..s.t.|.t.j.j...
-00004620: 7320 7c03 6400 7501 732e 7402 7c03 7403  s |.d.u.s.t.|.t.
-00004630: 8302 7302 7402 7c03 7404 6a05 6a06 8302  ..s.t.|.t.j.j...
-00004640: 7202 7c03 7202 7c02 7232 7c02 6e01 7c01  r.|.r.|.r2|.n.|.
-00004650: 9102 7102 5300 725c 0000 0029 07da 0768  ..q.S.r\...)...h
-00004660: 6173 6174 7472 72d9 0000 0072 3800 0000  asattrr....r8...
-00004670: 726e 0000 0072 ce00 0000 72cf 0000 0072  rn...r....r....r
-00004680: d100 0000 2904 7255 0000 0072 b700 0000  ....).rU...r....
-00004690: da04 666c 6167 5a0a 6174 7472 5f76 616c  ..flagZ.attr_val
-000046a0: 7565 a901 72bf 0000 0072 5300 0000 7257  ue..r....rS...rW
-000046b0: 0000 0072 5800 0000 4103 0000 7330 0000  ...rX...A...s0..
-000046c0: 0006 0006 0208 0102 fd0a 0408 0302 f902  ................
-000046d0: 0802 0106 0102 fe02 f808 0d08 0302 fd02  ................
-000046e0: 0402 0106 0102 fe02 fc02 0802 f80a f406  ................
-000046f0: 0c7a 3341 7267 756d 656e 7450 6172 7365  .z3ArgumentParse
-00004700: 722e 5f70 6f73 745f 7061 7273 655f 6172  r._post_parse_ar
-00004710: 6773 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  gs.<locals>.<lis
-00004720: 7463 6f6d 703e 7217 0000 007a 2854 6865  tcomp>r....z(The
-00004730: 7365 2061 7267 756d 656e 7473 2061 7265  se arguments are
-00004740: 206d 7574 7561 6c6c 7920 6578 636c 7573   mutually exclus
-00004750: 6976 653a 2072 c200 0000 7253 0000 0029  ive: r....rS...)
-00004760: 0a72 7100 0000 72aa 0000 0072 d900 0000  .rq...r....r....
-00004770: 7245 0000 0072 c000 0000 7276 0000 0072  rE...r....rv...r
-00004780: dc00 0000 7282 0000 0072 2800 0000 da04  ....r....r(.....
-00004790: 7661 7273 2906 7278 0000 0072 bf00 0000  vars).rx...r....
-000047a0: 5a12 6675 6e63 5f6d 785f 6172 675f 6772  Z.func_mx_arg_gr
-000047b0: 6f75 7073 5a06 675f 6172 6773 5a0e 6d78  oupsZ.g_argsZ.mx
-000047c0: 5f66 6c61 6773 5f66 6f75 6e64 72df 0000  _flags_foundr...
-000047d0: 0072 5300 0000 72f6 0000 0072 5700 0000  .rS...r....rW...
-000047e0: da10 5f70 6f73 745f 7061 7273 655f 6172  .._post_parse_ar
-000047f0: 6773 3203 0000 7320 0000 0006 070c 0102  gs2...s ........
-00004800: 0102 fe02 fd0c 070a 0402 0206 fe0c 1906  ................
-00004810: 0102 0106 ff0a 0302 8012 027a 1f41 7267  ...........z.Arg
-00004820: 756d 656e 7450 6172 7365 722e 5f70 6f73  umentParser._pos
-00004830: 745f 7061 7273 655f 6172 6773 6303 0000  t_parse_argsc...
-00004840: 0000 0000 0000 0000 0005 0000 000a 0000  ................
-00004850: 0003 0000 0073 5200 0000 7a0e 7400 8300  .....sR...z.t...
-00004860: 6a01 7c01 7c02 6401 8d02 7d03 7c00 a002  j.|.|.d...}.|...
-00004870: 7c03 a101 5700 5300 0400 7403 7928 0100  |...W.S...t.y(..
-00004880: 7d04 0100 7a0e 7c00 a004 7405 7c04 8301  }...z.|...t.|...
-00004890: a101 0100 5700 5900 6400 7d04 7e04 6400  ....W.Y.d.}.~.d.
-000048a0: 5300 6400 7d04 7e04 7701 7700 a902 4e29  S.d.}.~.w.w...N)
-000048b0: 0272 5000 0000 72bf 0000 0029 0672 6800  .rP...r....).rh.
-000048c0: 0000 da0a 7061 7273 655f 6172 6773 72f8  ....parse_argsr.
-000048d0: 0000 00da 0a56 616c 7565 4572 726f 7272  .....ValueErrorr
-000048e0: 8200 0000 726e 0000 0029 0572 7800 0000  ....rn...).rx...
-000048f0: 7250 0000 0072 bf00 0000 da06 7061 7273  rP...r......pars
-00004900: 6564 da01 6572 7900 0000 7253 0000 0072  ed..ery...rS...r
-00004910: 5700 0000 72fa 0000 0062 0300 0073 1400  W...r....b...s..
-00004920: 0000 0205 0601 0201 0201 06fe 0c04 0e01  ................
-00004930: 1c01 0880 02ff 7a19 4172 6775 6d65 6e74  ......z.Argument
-00004940: 5061 7273 6572 2e70 6172 7365 5f61 7267  Parser.parse_arg
-00004950: 7363 0300 0000 0000 0000 0000 0000 0600  sc..............
-00004960: 0000 0a00 0000 0300 0000 735a 0000 007a  ..........sZ...z
-00004970: 1274 0083 006a 017c 017c 0264 018d 025c  .t...j.|.|.d...\
-00004980: 027d 037d 047c 00a0 027c 03a1 017c 0466  .}.}.|...|...|.f
-00004990: 0257 0053 0004 0074 0379 2c01 007d 0501  .W.S...t.y,..}..
-000049a0: 007a 0e7c 00a0 0474 057c 0583 01a1 0101  .z.|...t.|......
-000049b0: 0057 0059 0064 007d 057e 0564 0053 0064  .W.Y.d.}.~.d.S.d
-000049c0: 007d 057e 0577 0177 0072 f900 0000 2906  .}.~.w.w.r....).
-000049d0: 7268 0000 00da 1070 6172 7365 5f6b 6e6f  rh.....parse_kno
-000049e0: 776e 5f61 7267 7372 f800 0000 72fb 0000  wn_argsr....r...
-000049f0: 0072 8200 0000 726e 0000 0029 0672 7800  .r....rn...).rx.
-00004a00: 0000 7250 0000 0072 bf00 0000 72fc 0000  ..rP...r....r...
-00004a10: 00da 0775 6e6b 6e6f 776e 72fd 0000 0072  ...unknownr....r
-00004a20: 7900 0000 7253 0000 0072 5700 0000 72fe  y...rS...rW...r.
-00004a30: 0000 0070 0300 0073 0e00 0000 0207 1401  ...p...s........
-00004a40: 1001 0e01 1c01 0880 02ff 7a1f 4172 6775  ..........z.Argu
-00004a50: 6d65 6e74 5061 7273 6572 2e70 6172 7365  mentParser.parse
-00004a60: 5f6b 6e6f 776e 5f61 7267 73da 1873 6b69  _known_args..ski
-00004a70: 705f 7079 6461 6e74 6963 5f76 616c 6964  p_pydantic_valid
-00004a80: 6174 696f 6e63 0400 0000 0000 0000 0000  ationc..........
-00004a90: 0000 0600 0000 0500 0000 4300 0000 7322  ..........C...s"
-00004aa0: 0000 007c 00a0 007c 01a1 015c 027d 047d  ...|...|...\.}.}
-00004ab0: 057c 006a 017c 047c 027c 0364 018d 037c  .|.j.|.|.|.d...|
-00004ac0: 0566 0253 0029 0261 c902 0000 5573 6520  .f.S.).a....Use 
-00004ad0: 7061 7273 6564 2061 7267 7320 746f 2069  parsed args to i
-00004ae0: 6e73 7461 6e74 6961 7465 2074 6865 2067  nstantiate the g
-00004af0: 6976 656e 2064 6174 6120 6d6f 6465 6c2e  iven data model.
-00004b00: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00004b10: 2020 2020 2020 2020 2020 2020 6172 6773              args
-00004b20: 3a0a 2020 2020 2020 2020 2020 2020 6172  :.            ar
-00004b30: 6773 5f6d 6f64 656c 3a0a 2020 2020 2020  gs_model:.      
-00004b40: 2020 2020 2020 736b 6970 5f70 7964 616e        skip_pydan
-00004b50: 7469 635f 7661 6c69 6461 7469 6f6e 3a0a  tic_validation:.
-00004b60: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-00004b70: 733a 0a20 2020 2020 2020 2020 2020 203e  s:.            >
-00004b80: 3e3e 2069 6d70 6f72 7420 7961 7078 0a20  >> import yapx. 
-00004b90: 2020 2020 2020 2020 2020 203e 3e3e 2066             >>> f
-00004ba0: 726f 6d20 6461 7461 636c 6173 7365 7320  rom dataclasses 
-00004bb0: 696d 706f 7274 2064 6174 6163 6c61 7373  import dataclass
-00004bc0: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
-00004bd0: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
-00004be0: 2040 6461 7461 636c 6173 730a 2020 2020   @dataclass.    
-00004bf0: 2020 2020 2020 2020 2e2e 2e20 636c 6173          ... clas
-00004c00: 7320 4164 644e 756d 733a 0a20 2020 2020  s AddNums:.     
-00004c10: 2020 2020 2020 202e 2e2e 2020 2020 2078         ...     x
-00004c20: 3a20 696e 740a 2020 2020 2020 2020 2020  : int.          
-00004c30: 2020 2e2e 2e20 2020 2020 793a 2069 6e74    ...     y: int
-00004c40: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
-00004c50: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
-00004c60: 2070 6172 7365 7220 3d20 7961 7078 2e41   parser = yapx.A
-00004c70: 7267 756d 656e 7450 6172 7365 7228 290a  rgumentParser().
-00004c80: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00004c90: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
-00004ca0: 656e 7473 2841 6464 4e75 6d73 290a 2020  ents(AddNums).  
-00004cb0: 2020 2020 2020 2020 2020 3e3e 3e20 7061            >>> pa
-00004cc0: 7273 6564 2c20 756e 6b6e 6f77 6e20 3d20  rsed, unknown = 
-00004cd0: 7061 7273 6572 2e70 6172 7365 5f6b 6e6f  parser.parse_kno
-00004ce0: 776e 5f61 7267 735f 746f 5f6d 6f64 656c  wn_args_to_model
-00004cf0: 285b 272d 7827 2c20 2731 272c 2027 2d79  (['-x', '1', '-y
-00004d00: 272c 2027 3227 2c20 272d 7a27 2c20 2733  ', '2', '-z', '3
-00004d10: 275d 290a 2020 2020 2020 2020 2020 2020  ']).            
-00004d20: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-00004d30: 3e3e 3e20 2870 6172 7365 642e 782c 2070  >>> (parsed.x, p
-00004d40: 6172 7365 642e 7929 0a20 2020 2020 2020  arsed.y).       
-00004d50: 2020 2020 2028 312c 2032 290a 2020 2020       (1, 2).    
-00004d60: 2020 2020 2020 2020 3e3e 3e20 756e 6b6e          >>> unkn
-00004d70: 6f77 6e0a 2020 2020 2020 2020 2020 2020  own.            
-00004d80: 5b27 2d7a 272c 2027 3327 5d0a 0a20 2020  ['-z', '3']..   
-00004d90: 2020 2020 20a9 0372 5000 0000 728f 0000       ..rP...r...
-00004da0: 0072 0001 0000 2902 72fe 0000 00da 145f  .r....).r......_
-00004db0: 7061 7273 655f 6172 6773 5f74 6f5f 6d6f  parse_args_to_mo
-00004dc0: 6465 6c29 0672 7800 0000 7250 0000 0072  del).rx...rP...r
-00004dd0: 8f00 0000 7200 0100 00da 0b70 6172 7365  ....r......parse
-00004de0: 645f 6172 6773 da0c 756e 6b6e 6f77 6e5f  d_args..unknown_
-00004df0: 6172 6773 7253 0000 0072 5300 0000 7257  argsrS...rS...rW
-00004e00: 0000 00da 1970 6172 7365 5f6b 6e6f 776e  .....parse_known
-00004e10: 5f61 7267 735f 746f 5f6d 6f64 656c 7d03  _args_to_model}.
-00004e20: 0000 7310 0000 000e 2304 0302 0102 0102  ..s.....#.......
-00004e30: 0104 fd02 0504 fa7a 2841 7267 756d 656e  .......z(Argumen
-00004e40: 7450 6172 7365 722e 7061 7273 655f 6b6e  tParser.parse_kn
-00004e50: 6f77 6e5f 6172 6773 5f74 6f5f 6d6f 6465  own_args_to_mode
-00004e60: 6c63 0400 0000 0000 0000 0000 0000 0500  lc..............
-00004e70: 0000 0500 0000 4300 0000 731a 0000 007c  ......C...s....|
-00004e80: 00a0 007c 01a1 017d 047c 006a 017c 047c  ...|...}.|.j.|.|
-00004e90: 027c 0364 018d 0353 0029 0261 7f02 0000  .|.d...S.).a....
-00004ea0: 5573 6520 7061 7273 6564 2061 7267 7320  Use parsed args 
-00004eb0: 746f 2069 6e73 7461 6e74 6961 7465 2074  to instantiate t
-00004ec0: 6865 2067 6976 656e 2064 6174 6120 6d6f  he given data mo
-00004ed0: 6465 6c2e 0a0a 2020 2020 2020 2020 4172  del...        Ar
-00004ee0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00004ef0: 6172 6773 3a0a 2020 2020 2020 2020 2020  args:.          
-00004f00: 2020 6172 6773 5f6d 6f64 656c 3a0a 2020    args_model:.  
-00004f10: 2020 2020 2020 2020 2020 736b 6970 5f70            skip_p
-00004f20: 7964 616e 7469 635f 7661 6c69 6461 7469  ydantic_validati
-00004f30: 6f6e 3a0a 0a20 2020 2020 2020 2045 7861  on:..        Exa
-00004f40: 6d70 6c65 733a 0a20 2020 2020 2020 2020  mples:.         
-00004f50: 2020 203e 3e3e 2069 6d70 6f72 7420 7961     >>> import ya
-00004f60: 7078 0a20 2020 2020 2020 2020 2020 203e  px.            >
-00004f70: 3e3e 2066 726f 6d20 6461 7461 636c 6173  >> from dataclas
-00004f80: 7365 7320 696d 706f 7274 2064 6174 6163  ses import datac
-00004f90: 6c61 7373 0a20 2020 2020 2020 2020 2020  lass.           
-00004fa0: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-00004fb0: 203e 3e3e 2040 6461 7461 636c 6173 730a   >>> @dataclass.
-00004fc0: 2020 2020 2020 2020 2020 2020 2e2e 2e20              ... 
-00004fd0: 636c 6173 7320 4164 644e 756d 733a 0a20  class AddNums:. 
-00004fe0: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
-00004ff0: 2020 2078 3a20 696e 740a 2020 2020 2020     x: int.      
-00005000: 2020 2020 2020 2e2e 2e20 2020 2020 793a        ...     y:
-00005010: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
-00005020: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-00005030: 203e 3e3e 2070 6172 7365 7220 3d20 7961   >>> parser = ya
-00005040: 7078 2e41 7267 756d 656e 7450 6172 7365  px.ArgumentParse
-00005050: 7228 290a 2020 2020 2020 2020 2020 2020  r().            
-00005060: 3e3e 3e20 7061 7273 6572 2e61 6464 5f61  >>> parser.add_a
-00005070: 7267 756d 656e 7473 2841 6464 4e75 6d73  rguments(AddNums
-00005080: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
-00005090: 3e20 7061 7273 6564 203d 2070 6172 7365  > parsed = parse
-000050a0: 722e 7061 7273 655f 6172 6773 5f74 6f5f  r.parse_args_to_
-000050b0: 6d6f 6465 6c28 5b27 2d78 272c 2027 3127  model(['-x', '1'
-000050c0: 2c20 272d 7927 2c20 2732 275d 290a 2020  , '-y', '2']).  
-000050d0: 2020 2020 2020 2020 2020 2e2e 2e0a 2020            ....  
-000050e0: 2020 2020 2020 2020 2020 3e3e 3e20 2870            >>> (p
-000050f0: 6172 7365 642e 782c 2070 6172 7365 642e  arsed.x, parsed.
-00005100: 7929 0a20 2020 2020 2020 2020 2020 2028  y).            (
-00005110: 312c 2032 290a 0a20 2020 2020 2020 2072  1, 2)..        r
-00005120: 0101 0000 2902 72fa 0000 0072 0201 0000  ....).r....r....
-00005130: 2905 7278 0000 0072 5000 0000 728f 0000  ).rx...rP...r...
-00005140: 0072 0001 0000 7203 0100 0072 5300 0000  .r....r....rS...
-00005150: 7253 0000 0072 5700 0000 da13 7061 7273  rS...rW.....pars
-00005160: 655f 6172 6773 5f74 6f5f 6d6f 6465 6cab  e_args_to_model.
-00005170: 0300 0073 0c00 0000 0a1e 0401 0201 0201  ...s............
-00005180: 0201 06fd 7a22 4172 6775 6d65 6e74 5061  ....z"ArgumentPa
-00005190: 7273 6572 2e70 6172 7365 5f61 7267 735f  rser.parse_args_
-000051a0: 746f 5f6d 6f64 656c 6304 0000 0000 0000  to_modelc.......
-000051b0: 0000 0000 0008 0000 000a 0000 0043 0000  .............C..
-000051c0: 0073 aa00 0000 7400 7c01 8301 7d04 7c02  .s....t.|...}.|.
-000051d0: 7310 7c04 a001 7c00 6a02 a101 7d02 7c02  s.|...|.j...}.|.
-000051e0: 7310 7403 8201 7c00 6a04 7c04 7c02 6401  s.t...|.j.|.|.d.
-000051f0: 8d02 7d05 7405 724e 7c03 734e 7a0d 7400  ..}.t.rN|.sNz.t.
-00005200: 7406 7c02 8301 6405 6900 7c05 a401 8e01  t.|...d.i.|.....
-00005210: 8301 7d05 5700 6e25 0400 7407 794d 0100  ..}.W.n%..t.yM..
-00005220: 7d06 0100 7a19 6402 6402 a008 6403 6404  }...z.d.d...d.d.
-00005230: 8400 7c06 a009 a100 4400 8301 a101 1700  ..|.....D.......
-00005240: 7d07 7c00 a00a 7c07 a101 0100 5700 5900  }.|...|.....W.Y.
-00005250: 6400 7d06 7e06 6e05 6400 7d06 7e06 7701  d.}.~.n.d.}.~.w.
-00005260: 7700 7c02 6405 6900 7c05 a401 8e01 5300  w.|.d.i.|.....S.
-00005270: 2906 4ea9 02da 0961 7267 735f 6469 6374  ).N....args_dict
-00005280: 728f 0000 0072 7d00 0000 6301 0000 0000  r....r}...c.....
-00005290: 0000 0000 0000 0002 0000 0006 0000 0073  ...............s
-000052a0: 0000 0073 2e00 0000 8100 7c00 5d12 7d01  ...s......|.].}.
-000052b0: 6400 7c01 6401 1900 6402 1900 9b00 6403  d.|.d...d.....d.
-000052c0: 7c01 6404 1900 9b00 6405 9d05 5600 0100  |.d.....d...V...
-000052d0: 7102 6406 5300 2907 7a18 4572 726f 7220  q.d.S.).z.Error 
-000052e0: 7061 7273 696e 6720 6172 6775 6d65 6e74  parsing argument
-000052f0: 2060 da03 6c6f 6372 0100 0000 7a03 603b   `..locr....z.`;
-00005300: 20da 036d 7367 72ac 0000 004e 7253 0000   ..msgr....NrS..
-00005310: 0072 5400 0000 7253 0000 0072 5300 0000  .rT...rS...rS...
-00005320: 7257 0000 00da 093c 6765 6e65 7870 723e  rW.....<genexpr>
-00005330: e903 0000 730a 0000 0002 8004 0002 021c  ....s...........
-00005340: ff0a ff7a 3641 7267 756d 656e 7450 6172  ...z6ArgumentPar
-00005350: 7365 722e 5f70 6172 7365 5f61 7267 735f  ser._parse_args_
-00005360: 746f 5f6d 6f64 656c 2e3c 6c6f 6361 6c73  to_model.<locals
-00005370: 3e2e 3c67 656e 6578 7072 3e72 5300 0000  >.<genexpr>rS...
-00005380: 290b 72f7 0000 0072 aa00 0000 7246 0000  ).r....r....rF..
-00005390: 0072 2600 0000 da16 5f75 6e69 6f6e 5f61  .r&....._union_a
-000053a0: 7267 735f 7769 7468 5f6d 6f64 656c 7235  rgs_with_modelr5
-000053b0: 0000 0072 3300 0000 722e 0000 0072 dc00  ...r3...r....r..
-000053c0: 0000 da06 6572 726f 7273 7282 0000 0029  ....errorsr....)
-000053d0: 0872 7800 0000 7250 0000 0072 8f00 0000  .rx...rP...r....
-000053e0: 7200 0100 0072 0301 0000 5a0a 6172 6773  r....r....Z.args
-000053f0: 5f75 6e69 6f6e 72fd 0000 0072 df00 0000  _unionr....r....
-00005400: 7253 0000 0072 5300 0000 7257 0000 0072  rS...rS...rW...r
-00005410: 0201 0000 d003 0000 732c 0000 0008 0604  ........s,......
-00005420: 020c 0104 0104 0104 0202 0102 0106 fe08  ................
-00005430: 0502 0202 0110 0108 ff0e 030c 0106 020a  ................
-00005440: fe16 0408 8002 fb0e 077a 2341 7267 756d  .........z#Argum
-00005450: 656e 7450 6172 7365 722e 5f70 6172 7365  entParser._parse
-00005460: 5f61 7267 735f 746f 5f6d 6f64 656c 7208  _args_to_modelr.
-00005470: 0100 0063 0200 0000 0000 0000 0000 0000  ...c............
-00005480: 0200 0000 0300 0000 0300 0000 7316 0000  ............s...
-00005490: 0087 0066 0164 0164 0284 087c 00a0 00a1  ...f.d.d...|....
-000054a0: 0044 0083 0153 0029 034e 6301 0000 0000  .D...S.).Nc.....
-000054b0: 0000 0000 0000 0003 0000 0004 0000 0013  ................
-000054c0: 0000 0073 2000 0000 6900 7c00 5d0c 5c02  ...s ...i.|.].\.
-000054d0: 7d01 7d02 7c01 8800 6a00 7600 7202 7c01  }.}.|...j.v.r.|.
-000054e0: 7c02 9302 7102 5300 7253 0000 0072 a100  |...q.S.rS...r..
-000054f0: 0000 a903 7255 0000 0072 e100 0000 da01  ....rU...r......
-00005500: 7672 9400 0000 7253 0000 0072 5700 0000  vr....rS...rW...
-00005510: da0a 3c64 6963 7463 6f6d 703e f603 0000  ..<dictcomp>....
-00005520: 7261 0000 007a 3941 7267 756d 656e 7450  ra...z9ArgumentP
-00005530: 6172 7365 722e 5f75 6e69 6f6e 5f61 7267  arser._union_arg
-00005540: 735f 7769 7468 5f6d 6f64 656c 2e3c 6c6f  s_with_model.<lo
-00005550: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
-00005560: 2901 728d 0000 0072 0701 0000 7253 0000  ).r....r....rS..
-00005570: 0072 9400 0000 7257 0000 0072 0c01 0000  .r....rW...r....
-00005580: f103 0000 7302 0000 0016 057a 2541 7267  ....s......z%Arg
-00005590: 756d 656e 7450 6172 7365 722e 5f75 6e69  umentParser._uni
-000055a0: 6f6e 5f61 7267 735f 7769 7468 5f6d 6f64  on_args_with_mod
-000055b0: 656c 6302 0000 0000 0000 0000 0000 0006  elc.............
-000055c0: 0000 0004 0000 0043 0000 0073 8000 0000  .......C...s....
-000055d0: 6400 7d02 7c01 6a00 7215 7c01 6a00 a001  d.}.|.j.r.|.j...
-000055e0: 7c01 6a02 6401 1700 a101 7315 7c01 6a00  |.j.d.....s.|.j.
-000055f0: a003 a100 a004 a100 7d02 7c02 7319 6400  ........}.|.s.d.
-00005600: 5300 6402 7d03 7405 7c02 8301 4400 5d0c  S.d.}.t.|...D.].
-00005610: 5c02 7d04 7d05 7c05 a003 a100 732b 7c04  \.}.}.|.....s+|.
-00005620: 7d03 0100 6e01 711f 7c03 6402 6b04 7236  }...n.q.|.d.k.r6
-00005630: 7c02 6400 7c03 8502 1900 7d02 6403 a006  |.d.|.....}.d...
-00005640: 6404 6405 8400 7c02 4400 8301 a101 5300  d.d...|.D.....S.
-00005650: 2906 4efa 0128 7201 0000 0072 7d00 0000  ).N..(r....r}...
-00005660: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00005670: 0003 0000 0073 0000 0073 1800 0000 8100  .....s...s......
-00005680: 7c00 5d07 7d01 7c01 a000 a100 5600 0100  |.].}.|.....V...
-00005690: 7102 6400 5300 725c 0000 0029 01da 0573  q.d.S.r\...)...s
-000056a0: 7472 6970 7254 0000 0072 5300 0000 7253  triprT...rS...rS
-000056b0: 0000 0072 5700 0000 720b 0100 0010 0400  ...rW...r.......
-000056c0: 0073 0400 0000 0280 1600 7a41 4172 6775  .s........zAArgu
-000056d0: 6d65 6e74 5061 7273 6572 2e5f 6765 745f  mentParser._get_
-000056e0: 6465 7363 7269 7074 696f 6e5f 6672 6f6d  description_from
-000056f0: 5f64 6f63 7374 7269 6e67 2e3c 6c6f 6361  _docstring.<loca
-00005700: 6c73 3e2e 3c67 656e 6578 7072 3e29 07da  ls>.<genexpr>)..
-00005710: 075f 5f64 6f63 5f5f 7260 0000 0072 9500  .__doc__r`...r..
-00005720: 0000 7212 0100 0072 9900 0000 da09 656e  ..r....r......en
-00005730: 756d 6572 6174 6572 dc00 0000 2906 72a7  umerater....).r.
-00005740: 0000 0072 8f00 0000 5a11 6465 7363 7269  ...r....Z.descri
-00005750: 7074 696f 6e5f 6c69 6e65 735a 1274 6578  ption_linesZ.tex
-00005760: 745f 626c 6f63 6b5f 656e 6473 5f61 74da  t_block_ends_at.
-00005770: 0169 da04 6c69 6e65 7253 0000 0072 5300  .i..linerS...rS.
-00005780: 0000 7257 0000 0072 9800 0000 f803 0000  ..rW...r........
-00005790: 7320 0000 0004 050c 0208 0104 ff0e 0304  s ..............
-000057a0: 0204 0104 0210 0108 0104 0104 0102 fe08  ................
-000057b0: 040c 0114 027a 2e41 7267 756d 656e 7450  .....z.ArgumentP
-000057c0: 6172 7365 722e 5f67 6574 5f64 6573 6372  arser._get_descr
-000057d0: 6970 7469 6f6e 5f66 726f 6d5f 646f 6373  iption_from_docs
-000057e0: 7472 696e 6763 0300 0000 0000 0000 0000  tringc..........
-000057f0: 0000 0400 0000 0300 0000 4300 0000 731c  ..........C...s.
-00005800: 0000 007c 00a0 007c 02a1 017d 037c 0372  ...|...|...}.|.r
-00005810: 0c7c 037c 015f 0164 0053 0064 0053 0072  .|.|._.d.S.d.S.r
-00005820: 5c00 0000 2902 7298 0000 0072 4900 0000  \...).r....rI...
-00005830: 2904 72a7 0000 0072 6600 0000 728f 0000  ).r....rf...r...
-00005840: 0072 4900 0000 7253 0000 0072 5300 0000  .rI...rS...rS...
-00005850: 7257 0000 00da 1f5f 7365 745f 6465 7363  rW....._set_desc
-00005860: 7269 7074 696f 6e5f 6672 6f6d 5f64 6f63  ription_from_doc
-00005870: 7374 7269 6e67 1204 0000 7308 0000 000a  string....s.....
-00005880: 0604 020a 0104 ff7a 2e41 7267 756d 656e  .......z.Argumen
-00005890: 7450 6172 7365 722e 5f73 6574 5f64 6573  tParser._set_des
-000058a0: 6372 6970 7469 6f6e 5f66 726f 6d5f 646f  cription_from_do
-000058b0: 6373 7472 696e 67da 0b6c 696e 6b65 645f  cstring..linked_
-000058c0: 6675 6e63 da0b 7265 6c61 795f 7661 6c75  func..relay_valu
-000058d0: 6563 0700 0000 0000 0000 0000 0000 1700  ec..............
-000058e0: 0000 0700 0000 0300 0000 73e6 0100 0067  ..........s....g
-000058f0: 007d 0769 007d 0864 017d 0964 017d 0a64  .}.i.}.d.}.d.}.d
-00005900: 017d 0b64 017d 0c64 017d 0d74 007c 0283  .}.d.}.d.}.t.|..
-00005910: 016a 01a0 02a1 0044 005d 437d 0e74 037c  .j.....D.]C}.t.|
-00005920: 0e83 01a0 0464 02a1 0172 2164 037d 0c71  .....d...r!d.}.q
-00005930: 1574 037c 0e83 01a0 0464 04a1 0172 2b64  .t.|.....d...r+d
-00005940: 037d 0a71 157c 0e6a 0564 056b 0272 3364  .}.q.|.j.d.k.r3d
-00005950: 037d 0b71 157c 0e6a 0564 066b 0272 3b64  .}.q.|.j.d.k.r;d
-00005960: 037d 0d71 157c 0e6a 0564 076b 0272 457c  .}.q.|.j.d.k.rE|
-00005970: 037c 0864 073c 0071 157c 0e6a 0564 086b  .|.d.<.q.|.j.d.k
-00005980: 0272 4f7c 067c 0864 083c 0071 157c 0e6a  .rO|.|.d.<.q.|.j
-00005990: 0564 096b 0272 5864 037c 0864 093c 0071  .d.k.rXd.|.d.<.q
-000059a0: 157c 0a70 607c 0c70 607c 0b70 607c 0d7d  .|.p`|.p`|.p`|.}
-000059b0: 097c 0973 737c 0572 7374 0664 0a64 0b84  .|.ss|.rst.d.d..
-000059c0: 0074 007c 0583 016a 01a0 02a1 0044 0083  .t.|...j.....D..
-000059d0: 0183 017d 097c 0473 7974 077c 0283 017d  ...}.|.syt.|...}
-000059e0: 047c 0972 e17c 016a 087c 037c 0464 0c8d  .|.r.|.j.|.|.d..
-000059f0: 025c 027d 0f7d 107c 0c73 887c 0d72 d669  .\.}.}.|.s.|.r.i
-00005a00: 0089 007c 0083 007d 117c 1044 005d 247d  ...|...}.|.D.]$}
-00005a10: 127c 12a0 0464 0da1 0172 b37c 126a 0964  .|...d...r.|.j.d
-00005a20: 0e64 0f64 108d 0264 1119 007d 137c 13a0  .d.d...d...}.|..
-00005a30: 0a64 0da1 017d 147c 1472 b37c 116a 0b7c  .d...}.|.r.|.j.|
-00005a40: 1364 1264 0064 0164 138d 0401 007c 1388  .d.d.d.d.....|..
-00005a50: 007c 143c 0071 8f7c 116a 0c7c 1064 148d  .|.<.q.|.j.|.d..
-00005a60: 015c 027d 157d 1087 0066 0164 1564 1684  .\.}.}...f.d.d..
-00005a70: 0874 0d7c 1583 01a0 0ea1 0044 0083 017d  .t.|.......D...}
-00005a80: 167c 0c72 d07c 08a0 0f7c 16a1 0101 007c  .|.r.|...|.....|
-00005a90: 0d72 d67c 167c 0864 063c 007c 0a72 da7c  .r.|.|.d.<.|.r.|
-00005aa0: 107d 077c 0b72 e07c 107c 0864 053c 006e  .}.|.r.|.|.d.<.n
-00005ab0: 077c 016a 107c 037c 0464 0c8d 027d 0f7c  .|.j.|.|.d...}.|
-00005ac0: 027c 0769 0074 0d7c 0f83 01a4 017c 08a4  .|.i.t.|.....|..
-00005ad0: 018e 0153 0029 174e 467a 022a 2a54 72b3  ...S.).NFz.**Tr.
-00005ae0: 0000 00da 0b5f 6578 7472 615f 6172 6773  ....._extra_args
-00005af0: da0d 5f65 7874 7261 5f6b 7761 7267 735a  .._extra_kwargsZ
-00005b00: 095f 616c 6c5f 6172 6773 5a0c 5f72 656c  ._all_argsZ._rel
-00005b10: 6179 5f76 616c 7565 5a10 5f63 616c 6c65  ay_valueZ._calle
-00005b20: 645f 6672 6f6d 5f63 6c69 6301 0000 0000  d_from_clic.....
-00005b30: 0000 0000 0000 0002 0000 0004 0000 0073  ...............s
-00005b40: 0000 0073 2800 0000 8100 7c00 5d0f 7d01  ...s(.....|.].}.
-00005b50: 7400 7c01 8301 a001 6400 a101 700f 7c01  t.|.....d...p.|.
-00005b60: 6a02 6401 7600 5600 0100 7102 6402 5300  j.d.v.V...q.d.S.
-00005b70: 2903 72b3 0000 0029 0272 1a01 0000 721b  ).r....).r....r.
-00005b80: 0100 004e 2903 726e 0000 0072 6000 0000  ...N).rn...r`...
-00005b90: 7292 0000 0029 0272 5500 0000 da01 7072  r....).rU.....pr
-00005ba0: 5300 0000 7253 0000 0072 5700 0000 720b  S...rS...rW...r.
-00005bb0: 0100 0047 0400 0073 0a00 0000 0280 0400  ...G...s........
-00005bc0: 0202 16ff 0aff 7a2b 4172 6775 6d65 6e74  ......z+Argument
-00005bd0: 5061 7273 6572 2e5f 7275 6e5f 6675 6e63  Parser._run_func
-00005be0: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
-00005bf0: 7072 3e29 0272 5000 0000 728f 0000 0072  pr>).rP...r....r
-00005c00: 6500 0000 725b 0000 0072 1700 0000 72ad  e...r[...r....r.
-00005c10: 0000 0072 0100 0000 72bb 0000 0029 0372  ...r....r....).r
-00005c20: ba00 0000 7263 0000 0072 b900 0000 2901  ....rc...r....).
-00005c30: 7250 0000 0063 0100 0000 0000 0000 0000  rP...c..........
-00005c40: 0000 0300 0000 0400 0000 1300 0000 731a  ..............s.
-00005c50: 0000 0069 007c 005d 095c 027d 017d 0288  ...i.|.].\.}.}..
-00005c60: 007c 0119 007c 0293 0271 0253 0072 5300  .|...|...q.S.rS.
-00005c70: 0000 7253 0000 0072 0e01 0000 a901 5a10  ..rS...r......Z.
-00005c80: 756e 6b6e 6f77 6e5f 6e61 6d65 5f6d 6170  unknown_name_map
-00005c90: 7253 0000 0072 5700 0000 7210 0100 006b  rS...rW...r....k
-00005ca0: 0400 0073 0600 0000 0600 0e01 06ff 7a2c  ...s..........z,
-00005cb0: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
-00005cc0: 7275 6e5f 6675 6e63 2e3c 6c6f 6361 6c73  run_func.<locals
-00005cd0: 3e2e 3c64 6963 7463 6f6d 703e 2911 7209  >.<dictcomp>).r.
-00005ce0: 0000 00da 0a70 6172 616d 6574 6572 7372  .....parametersr
-00005cf0: c000 0000 726e 0000 0072 6000 0000 7292  ....rn...r`...r.
-00005d00: 0000 00da 0361 6e79 7225 0000 0072 0501  .....anyr%...r..
-00005d10: 0000 da05 7370 6c69 74da 066c 7374 7269  ....split..lstri
-00005d20: 7072 6f00 0000 72fe 0000 0072 f700 0000  pro...r....r....
-00005d30: 728d 0000 00da 0675 7064 6174 6572 0601  r......updater..
-00005d40: 0000 2917 72a7 0000 0072 6600 0000 729c  ..).r....rf...r.
-00005d50: 0000 0072 5000 0000 728f 0000 0072 1801  ...rP...r....r..
-00005d60: 0000 7219 0100 005a 0966 756e 635f 6172  ..r....Z.func_ar
-00005d70: 6773 5a0b 6675 6e63 5f6b 7761 7267 735a  gsZ.func_kwargsZ
-00005d80: 0d65 7874 7261 5f61 7267 735f 6f6b 5a0c  .extra_args_okZ.
-00005d90: 6163 6365 7074 735f 6172 6773 5a12 6163  accepts_argsZ.ac
-00005da0: 6365 7074 735f 6578 7472 615f 6172 6773  cepts_extra_args
-00005db0: 5a0e 6163 6365 7074 735f 6b77 6172 6773  Z.accepts_kwargs
-00005dc0: 5a14 6163 6365 7074 735f 6578 7472 615f  Z.accepts_extra_
-00005dd0: 6b77 6172 6773 721c 0100 005a 0a6d 6f64  kwargsr....Z.mod
-00005de0: 656c 5f69 6e73 7472 0401 0000 5a0e 756e  el_instr....Z.un
-00005df0: 6b6e 6f77 6e5f 7061 7273 6572 7256 0000  known_parserrV..
-00005e00: 005a 0678 5f66 6c61 675a 0b78 5f66 6c61  .Z.x_flagZ.x_fla
-00005e10: 675f 6261 7265 5a0e 7061 7273 6564 5f75  g_bareZ.parsed_u
-00005e20: 6e6b 6e6f 776e 5a0c 6578 7472 615f 6b77  nknownZ.extra_kw
-00005e30: 6172 6773 7253 0000 0072 1d01 0000 7257  argsrS...r....rW
-00005e40: 0000 00da 095f 7275 6e5f 6675 6e63 1d04  ....._run_func..
-00005e50: 0000 7390 0000 0004 0a04 0104 0204 0204  ..s.............
-00005e60: 0104 0204 0112 020e 0106 010e 0106 010a  ................
-00005e70: 0106 010a 0106 010a 010a 010a 010a 010a  ................
-00005e80: 0108 0102 800e 0302 ff08 0408 010c 0208  ................
-00005e90: fe04 0508 0104 0304 0202 0102 010a fe08  ................
-00005ea0: 0504 0106 0108 010a 0112 010a 0104 0104  ................
-00005eb0: 0102 0102 0102 0102 0106 fc08 0602 8004  ................
-00005ec0: 0202 010a ff0a 040a 0106 ff04 030a 0104  ................
-00005ed0: 0108 0104 0204 0104 0208 0102 8004 0302  ................
-00005ee0: 0102 0106 fe16 057a 1841 7267 756d 656e  .......z.Argumen
-00005ef0: 7450 6172 7365 722e 5f72 756e 5f66 756e  tParser._run_fun
-00005f00: 63da 0763 6f6d 6d61 6e64 da0b 7375 6263  c..command..subc
-00005f10: 6f6d 6d61 6e64 73da 116e 616d 6564 5f73  ommands..named_s
-00005f20: 7562 636f 6d6d 616e 6473 6304 0000 0000  ubcommandsc.....
-00005f30: 0000 0000 0000 0009 0000 000b 0000 004b  ...............K
-00005f40: 0000 0073 d200 0000 7c00 6403 6900 7c04  ...s....|.d.i.|.
-00005f50: a401 8e01 7d05 7c01 722e 7400 7c01 8301  ....}.|.r.t.|...
-00005f60: 7d06 7c00 6a01 7c05 7c06 6401 8d02 0100  }.|.j.|.|.d.....
-00005f70: 7c05 a002 7c06 a101 0100 7c05 6a03 6403  |...|.....|.j.d.
-00005f80: 6900 7c00 6a04 7c01 7c00 6a05 7c06 7c00  i.|.j.|.|.j.|.|.
-00005f90: 6a06 7c01 7c00 6a07 7c06 6904 a401 8e01  j.|.|.j.|.i.....
-00005fa0: 0100 6e14 7c05 6a03 6403 6900 7c00 6a05  ..n.|.j.d.i.|.j.
-00005fb0: 6400 7c00 6a04 6400 7c00 6a07 6400 7c00  d.|.j.d.|.j.d.|.
-00005fc0: 6a06 6400 6904 a401 8e01 0100 7c02 7255  j.d.i.......|.rU
-00005fd0: 7408 7c02 8301 724b 7c02 6701 7d02 7c02  t.|...rK|.g.}.|.
-00005fe0: 4400 5d07 7d07 7c05 a009 7c07 a101 0100  D.].}.|...|.....
-00005ff0: 714d 7c03 7267 7c03 a00a a100 4400 5d0b  qM|.rg|.....D.].
-00006000: 5c02 7d08 7d07 7c05 6a09 7c07 7c08 6402  \.}.}.|.j.|.|.d.
-00006010: 8d02 0100 715b 7c05 5300 2904 4e29 0272  ....q[|.S.).N).r
-00006020: 6600 0000 728f 0000 0072 b100 0000 7253  f...r....r....rS
-00006030: 0000 0029 0b72 2500 0000 7217 0100 0072  ...).r%...r....r
-00006040: 9100 0000 729d 0000 0072 4200 0000 7243  ....r....rB...rC
-00006050: 0000 0072 4500 0000 7246 0000 00da 0863  ...rE...rF.....c
-00006060: 616c 6c61 626c 6572 9e00 0000 728d 0000  allabler....r...
-00006070: 0029 0972 a700 0000 7224 0100 0072 2501  .).r....r$...r%.
-00006080: 0000 7226 0100 0072 5100 0000 7266 0000  ..r&...rQ...rf..
-00006090: 005a 0e72 6f6f 745f 6172 675f 6d6f 6465  .Z.root_arg_mode
-000060a0: 6c72 5600 0000 7292 0000 0072 5300 0000  lrV...r....rS...
-000060b0: 7253 0000 0072 5700 0000 da0d 5f62 7569  rS...rW....._bui
-000060c0: 6c64 5f70 6172 7365 7281 0400 0073 3e00  ld_parser....s>.
-000060d0: 0000 0e08 0402 0801 0401 0201 0201 06fe  ................
-000060e0: 0a04 0801 0602 0601 0601 0601 02fc 08ff  ................
-000060f0: 0809 0602 0601 0601 0601 02fc 06ff 0409  ................
-00006100: 0801 0601 0801 0c01 0402 1001 1001 0402  ................
-00006110: 7a1c 4172 6775 6d65 6e74 5061 7273 6572  z.ArgumentParser
-00006120: 2e5f 6275 696c 645f 7061 7273 6572 2902  ._build_parser).
-00006130: 7250 0000 00da 0c64 6566 6175 6c74 5f61  rP.....default_a
-00006140: 7267 73da 0b70 6172 7365 725f 6172 6773  rgs..parser_args
-00006150: 7229 0100 00da 0d70 6172 7365 725f 6b77  r).....parser_kw
-00006160: 6172 6773 6301 0000 0000 0000 0002 0000  argsc...........
-00006170: 0011 0000 0009 0000 004f 0000 0073 3801  .........O...s8.
-00006180: 0000 7c00 6a00 7c03 6900 7c04 a401 8e01  ..|.j.|.i.|.....
-00006190: 7d05 7c01 6401 7500 7213 7401 6a02 6402  }.|.d.u.r.t.j.d.
-000061a0: 6401 8502 1900 7d01 7c01 7319 7c02 7219  d.....}.|.s.|.r.
-000061b0: 7c02 7d01 7c05 a003 7c01 a101 5c02 7d06  |.}.|...|...\.}.
-000061c0: 7d07 7404 7c06 8301 7d08 7c08 a005 7c00  }.t.|...}.|...|.
-000061d0: 6a06 a101 7d09 7c08 a005 7c00 6a07 a101  j...}.|...|.j...
-000061e0: 7d0a 7c08 a005 7c00 6a08 a101 7d0b 7c08  }.|...|.j...}.|.
-000061f0: a005 7c00 6a09 a101 7d0c 7c08 a005 7c00  ..|.j...}.|...|.
-00006200: 6a0a a101 7d0d 6401 7d0e 6401 7d0f 7c09  j...}.d.}.d.}.|.
-00006210: 7252 7c00 6a0b 7c05 7c09 7c0a 7c0c 7c01  rR|.j.|.|.|.|.|.
-00006220: 6403 8d05 7d0f 740c 7c0f 740d 8302 7269  d...}.t.|.t...ri
-00006230: 7a06 740e 7c0f 8301 7d0e 5700 6e0d 0400  z.t.|...}.W.n...
-00006240: 740f 7968 0100 0100 0100 7c0f 7d0e 5900  t.yh......|.}.Y.
-00006250: 6e03 7700 7c0f 7d0e 7a20 7c0b 727b 7c0c  n.w.|.}.z |.r{|.
-00006260: 727b 7c00 6a0b 7c05 7c0c 7c0d 7c01 7c09  r{|.j.|.|.|.|.|.
-00006270: 7c0e 6404 8d06 7d0e 5700 740c 7c0f 740d  |.d...}.W.t.|.t.
-00006280: 8302 728a 7c0f 4400 5d06 7d10 7c0c 7389  ..r.|.D.].}.|.s.
-00006290: 7c10 7d0e 7183 7c0e 5300 740c 7c0f 740d  |.}.q.|.S.t.|.t.
-000062a0: 8302 729a 7c0f 4400 5d07 7d10 7c0c 7399  ..r.|.D.].}.|.s.
-000062b0: 7c10 7d0e 7193 7700 7700 2905 612d 0300  |.}.q.w.w.).a-..
-000062c0: 0055 7365 2067 6976 656e 2066 756e 6374  .Use given funct
-000062d0: 696f 6e73 2074 6f20 636f 6e73 7472 7563  ions to construc
-000062e0: 7420 6120 434c 492c 2070 6172 7365 2074  t a CLI, parse t
-000062f0: 6865 2061 7267 732c 2061 6e64 2069 6e76  he args, and inv
-00006300: 6f6b 6520 7468 6520 6170 7072 6f70 7269  oke the appropri
-00006310: 6174 6520 636f 6d6d 616e 642e 0a0a 2020  ate command...  
-00006320: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00006330: 2020 2020 2020 2020 2a70 6172 7365 725f          *parser_
-00006340: 6172 6773 3a0a 2020 2020 2020 2020 2020  args:.          
-00006350: 2020 6172 6773 3a0a 2020 2020 2020 2020    args:.        
-00006360: 2020 2020 6465 6661 756c 745f 6172 6773      default_args
-00006370: 3a0a 2020 2020 2020 2020 2020 2020 2a2a  :.            **
-00006380: 7061 7273 6572 5f6b 7761 7267 733a 0a0a  parser_kwargs:..
-00006390: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-000063a0: 733a 0a20 2020 2020 2020 2020 2020 203e  s:.            >
-000063b0: 3e3e 2069 6d70 6f72 7420 7961 7078 0a20  >> import yapx. 
-000063c0: 2020 2020 2020 2020 2020 202e 2e2e 0a20             .... 
-000063d0: 2020 2020 2020 2020 2020 203e 3e3e 2064             >>> d
-000063e0: 6566 2070 7269 6e74 5f6e 756d 7328 2a61  ef print_nums(*a
-000063f0: 7267 7329 3a0a 2020 2020 2020 2020 2020  rgs):.          
-00006400: 2020 2e2e 2e20 2020 2020 7072 696e 7428    ...     print(
-00006410: 2741 7267 733a 2027 2c20 2a61 7267 7329  'Args: ', *args)
-00006420: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
-00006430: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
-00006440: 2064 6566 2066 696e 645f 6576 656e 7328   def find_evens(
-00006450: 2a61 7267 7329 3a0a 2020 2020 2020 2020  *args):.        
-00006460: 2020 2020 2e2e 2e20 2020 2020 7265 7475      ...     retu
-00006470: 726e 205b 7820 666f 7220 7820 696e 2061  rn [x for x in a
-00006480: 7267 7320 6966 2069 6e74 2878 2920 2520  rgs if int(x) % 
-00006490: 3220 3d3d 2030 5d0a 2020 2020 2020 2020  2 == 0].        
-000064a0: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
-000064b0: 2020 2020 3e3e 3e20 6465 6620 6669 6e64      >>> def find
-000064c0: 5f6f 6464 7328 2a61 7267 7329 3a0a 2020  _odds(*args):.  
-000064d0: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
-000064e0: 2020 7265 7475 726e 205b 7820 666f 7220    return [x for 
-000064f0: 7820 696e 2061 7267 7320 6966 2069 6e74  x in args if int
-00006500: 2878 2920 2520 3220 213d 2030 5d0a 2020  (x) % 2 != 0].  
-00006510: 2020 2020 2020 2020 2020 2e2e 2e0a 2020            ....  
-00006520: 2020 2020 2020 2020 2020 3e3e 3e20 636c            >>> cl
-00006530: 695f 6172 6773 203d 205b 2766 696e 642d  i_args = ['find-
-00006540: 6f64 6473 272c 2027 3127 2c20 2732 272c  odds', '1', '2',
-00006550: 2027 3327 2c20 2734 272c 2027 3527 5d0a   '3', '4', '5'].
-00006560: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00006570: 7961 7078 2e72 756e 2870 7269 6e74 5f6e  yapx.run(print_n
-00006580: 756d 732c 205b 6669 6e64 5f65 7665 6e73  ums, [find_evens
-00006590: 2c20 6669 6e64 5f6f 6464 735d 2c20 6172  , find_odds], ar
-000065a0: 6773 3d63 6c69 5f61 7267 7329 0a20 2020  gs=cli_args).   
-000065b0: 2020 2020 2020 2020 2041 7267 733a 2020           Args:  
-000065c0: 3120 3220 3320 3420 350a 2020 2020 2020  1 2 3 4 5.      
-000065d0: 2020 2020 2020 5b27 3127 2c20 2733 272c        ['1', '3',
-000065e0: 2027 3527 5d0a 2020 2020 2020 2020 4e72   '5'].        Nr
-000065f0: 1700 0000 2905 7266 0000 0072 9c00 0000  ....).rf...r....
-00006600: 728f 0000 0072 1801 0000 7250 0000 0029  r....r....rP...)
-00006610: 0672 6600 0000 729c 0000 0072 8f00 0000  .rf...r....r....
-00006620: 7250 0000 0072 1801 0000 7219 0100 0029  rP...r....r....)
-00006630: 1072 2801 0000 727f 0000 00da 0461 7267  .r(...r......arg
-00006640: 7672 fe00 0000 72f7 0000 0072 aa00 0000  vr....r....r....
-00006650: 7242 0000 0072 4300 0000 7244 0000 0072  rB...rC...rD...r
-00006660: 4500 0000 7246 0000 0072 2301 0000 7238  E...rF...r#...r8
-00006670: 0000 0072 0a00 0000 da04 6e65 7874 da0d  ...r......next..
-00006680: 5374 6f70 4974 6572 6174 696f 6e29 1172  StopIteration).r
-00006690: a700 0000 7250 0000 0072 2901 0000 722a  ....rP...r)...r*
-000066a0: 0100 0072 2b01 0000 7266 0000 005a 0a6b  ...r+...rf...Z.k
-000066b0: 6e6f 776e 5f61 7267 7372 8600 0000 7203  nown_argsr....r.
-000066c0: 0100 005a 0972 6f6f 745f 6675 6e63 5a14  ...Z.root_funcZ.
-000066d0: 726f 6f74 5f66 756e 635f 6172 6773 5f6d  root_func_args_m
-000066e0: 6f64 656c 5a0c 636f 6d6d 616e 645f 6e61  odelZ.command_na
-000066f0: 6d65 5a0c 636f 6d6d 616e 645f 6675 6e63  meZ.command_func
-00006700: 5a17 636f 6d6d 616e 645f 6675 6e63 5f61  Z.command_func_a
-00006710: 7267 735f 6d6f 6465 6c72 1901 0000 5a0b  rgs_modelr....Z.
-00006720: 726f 6f74 5f72 6573 756c 745a 0a67 656e  root_resultZ.gen
-00006730: 5f72 6573 756c 7472 5300 0000 7253 0000  _resultrS...rS..
-00006740: 0072 5700 0000 da04 5f72 756e b004 0000  .rW....._run....
-00006750: 737a 0000 0010 2308 020e 0108 0204 010e  sz....#.........
-00006760: 0308 0104 0204 0104 ff04 0304 0104 ff0c  ................
-00006770: 0304 0104 0104 ff04 0304 0104 ff04 0404  ................
-00006780: 0104 0204 0102 0102 0102 0102 0102 0106  ................
-00006790: fb0a 0802 010c 010c 0108 0102 ff04 0302  ................
-000067a0: 0208 0104 0102 0102 0102 0102 0102 0102  ................
-000067b0: 0106 fa02 800a 0908 0104 0104 0102 8004  ................
-000067c0: 020a fb08 0104 0104 0102 8002 fd02 017a  ...............z
-000067d0: 1341 7267 756d 656e 7450 6172 7365 722e  .ArgumentParser.
-000067e0: 5f72 756e 2902 4e46 725c 0000 0029 0246  _run).NFr\...).F
-000067f0: 4629 024e 4e29 034e 4e46 2903 4e4e 4e29  F).NN).NNF).NNN)
-00006800: 3a72 9500 0000 da0a 5f5f 6d6f 6475 6c65  :r......__module
-00006810: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00006820: 7242 0000 0072 6e00 0000 72a2 0000 0072  rB...rn...r....r
-00006830: 4300 0000 7244 0000 0072 4500 0000 7246  C...rD...rE...rF
-00006840: 0000 0072 2d00 0000 720c 0000 0072 1000  ...r-...r....r..
-00006850: 0000 720f 0000 0072 1300 0000 72d6 0000  ..r....r....r...
-00006860: 0072 6900 0000 7282 0000 0072 0b00 0000  .ri...r....r....
-00006870: 728a 0000 0072 1500 0000 720d 0000 0072  r....r....r....r
-00006880: 2900 0000 7291 0000 0072 7400 0000 7241  )...r....rt...rA
-00006890: 0000 0072 9b00 0000 729e 0000 00da 0c73  ...r....r......s
-000068a0: 7461 7469 636d 6574 686f 6472 a400 0000  taticmethodr....
-000068b0: da0b 636c 6173 736d 6574 686f 6472 2200  ..classmethodr".
-000068c0: 0000 7290 0000 0072 c700 0000 7212 0000  ..r....r....r...
-000068d0: 0072 cd00 0000 72c9 0000 0072 c800 0000  .r....r....r....
-000068e0: 7296 0000 0072 f200 0000 728c 0000 0072  r....r....r....r
-000068f0: 7700 0000 7228 0000 0072 f800 0000 7211  w...r(...r....r.
-00006900: 0000 0072 fa00 0000 72fe 0000 0072 0501  ...r....r....r..
-00006910: 0000 7206 0100 0072 0201 0000 720e 0000  ..r....r....r...
-00006920: 0072 0c01 0000 7298 0000 0072 1701 0000  .r....r....r....
-00006930: 7223 0100 0072 2801 0000 722f 0100 00da  r#...r(...r/....
-00006940: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7253  .__classcell__rS
-00006950: 0000 0072 5300 0000 7279 0000 0072 5700  ...rS...ry...rW.
-00006960: 0000 7241 0000 004c 0000 0073 d401 0000  ..rA...L...s....
-00006970: 0a00 0c01 0c01 0c01 0c01 0c01 0205 0201  ................
-00006980: 0201 0201 0201 0201 0201 0201 0201 06f5  ................
-00006990: 0202 02fe 0603 02fd 0604 02fc 0605 02fb  ................
-000069a0: 0a06 02fa 0a07 02f9 0a08 02f8 0a09 02f7  ................
-000069b0: 060a 02f6 020b 02f5 020c 0ef4 0e71 0206  .............q..
-000069c0: 0201 04fd 0a02 02fe 0203 02fd 0204 0efc  ................
-000069d0: 022e 1602 02fe 0203 0afd 0234 04fd 1602  ...........4....
-000069e0: 02fe 0603 02fd 0204 02fc 0405 0afb 0263  ...............c
-000069f0: 04fd 0a02 02fe 0603 02fd 0204 02fc 0205  ................
-00006a00: 0afb 020e 1c01 0203 0201 0402 02fe 1603  ................
-00006a10: 02fd 0604 0cfc 007f 007f 0228 2001 0203  ...........( ...
-00006a20: 2401 0203 2401 0203 0204 0201 04fc 0602  $...$...........
-00006a30: 02fe 0203 02fd 0204 02fc 0605 0cfb 143f  ...............?
-00006a40: 1411 100a 020b 0402 02fe 0203 0afd 0232  ...............2
-00006a50: 0201 04fd 0a02 02fe 0803 02fd 0204 0efc  ................
-00006a60: 0210 0201 04fd 0a02 02fe 0803 02fd 0e04  ................
-00006a70: 0efc 020f 0201 0201 04fc 0a02 02fe 0a03  ................
-00006a80: 02fd 0204 02fc 0e05 0afb 0230 0201 0201  ...........0....
-00006a90: 04fc 0a02 02fe 0a03 02fd 0204 02fc 0205  ................
-00006aa0: 0afb 0228 0201 04fc 0402 02fe 0a03 02fd  ...(............
-00006ab0: 0204 02fc 0205 0afb 0221 0201 0a01 02ff  .........!......
-00006ac0: 0602 02fe 0a03 0cfd 0206 0201 1602 02fe  ................
-00006ad0: 0603 0cfd 0219 0201 0402 02fe 1603 02fd  ................
-00006ae0: 0204 0cfc 020a 0206 0201 0201 04f9 0202  ................
-00006af0: 02fe 0a03 02fd 0604 02fc 0a05 02fb 0e06  ................
-00006b00: 02fa 0607 02f9 0208 0cf8 0263 0203 0201  ...........c....
-00006b10: 0201 04fc 0e02 02fe 1203 02fd 1604 02fc  ................
-00006b20: 0205 02fb 0206 0cfa 022e 0204 0201 06fc  ................
-00006b30: 0202 02fe 0a03 02fd 0a04 02fc 0205 02fb  ................
-00006b40: 0206 14fa 7241 0000 0029 4e72 7400 0000  ....rA...)Nrt...
-00006b50: da0f 636f 6c6c 6563 7469 6f6e 732e 6162  ..collections.ab
-00006b60: 6372 ce00 0000 727f 0000 0072 0200 0000  cr....r....r....
-00006b70: da0a 636f 6e74 6578 746c 6962 7203 0000  ..contextlibr...
-00006b80: 00da 0b64 6174 6163 6c61 7373 6573 7204  ...dataclassesr.
-00006b90: 0000 0072 0500 0000 7206 0000 00da 0465  ...r....r......e
-00006ba0: 6e75 6d72 0700 0000 da09 6675 6e63 746f  numr......functo
-00006bb0: 6f6c 7372 0800 0000 da07 696e 7370 6563  olsr......inspec
-00006bc0: 7472 0900 0000 da05 7479 7065 7372 0a00  tr......typesr..
-00006bd0: 0000 da06 7479 7069 6e67 720b 0000 0072  ....typingr....r
-00006be0: 0c00 0000 720d 0000 0072 0e00 0000 720f  ....r....r....r.
-00006bf0: 0000 0072 1000 0000 7211 0000 0072 1200  ...r....r....r..
-00006c00: 0000 7213 0000 0072 1400 0000 7215 0000  ..r....r....r...
-00006c10: 005a 0d70 6b67 5f72 6573 6f75 7263 6573  .Z.pkg_resources
-00006c20: 7216 0000 00da 0761 6374 696f 6e73 7218  r......actionsr.
-00006c30: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
-00006c40: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-00006c50: 0072 1f00 0000 7220 0000 00da 0361 7267  .r....r .....arg
-00006c60: 7221 0000 0072 2200 0000 7223 0000 0072  r!...r"...r#...r
-00006c70: 2400 0000 7225 0000 00da 0a65 7863 6570  $...r%.....excep
-00006c80: 7469 6f6e 7372 2600 0000 7227 0000 0072  tionsr&...r'...r
-00006c90: bf00 0000 7228 0000 0072 2900 0000 722a  ....r(...r)...r*
-00006ca0: 0000 0072 2b00 0000 da05 7574 696c 7372  ...r+.....utilsr
-00006cb0: 2c00 0000 722d 0000 0072 2e00 0000 722f  ,...r-...r....r/
-00006cc0: 0000 0072 3000 0000 7231 0000 0072 3200  ...r0...r1...r2.
-00006cd0: 0000 7233 0000 0072 3400 0000 7235 0000  ..r3...r4...r5..
-00006ce0: 0072 3600 0000 7237 0000 0072 3800 0000  .r6...r7...r8...
-00006cf0: 7239 0000 0072 c600 0000 723c 0000 005a  r9...r....r<...Z
-00006d00: 1174 7970 696e 675f 6578 7465 6e73 696f  .typing_extensio
-00006d10: 6e73 723f 0000 0072 4000 0000 7241 0000  nsr?...r@...rA..
-00006d20: 0072 5300 0000 7253 0000 0072 5300 0000  .rS...rS...rS...
-00006d30: 7257 0000 00da 083c 6d6f 6475 6c65 3e01  rW.....<module>.
-00006d40: 0000 0073 3200 0000 0800 0801 0801 0c01  ...s2...........
-00006d50: 0c01 1401 0c01 0c01 0c01 0c01 3401 0c0e  ............4...
-00006d60: 2c02 1c0b 1007 0c01 1401 4001 0a11 0e01  ,.........@.....
-00006d70: 0c02 0a02 0c01 0802 1603                 ..........
+000005f0: 640b 640b 640b 640b 650a 640b 640c 9c09  d.d.d.d.e.d.d...
+00000600: 640d 650b 640e 650c 6504 1900 640f 650c  d.e.d.e.e...d.e.
+00000610: 6504 1900 6410 650c 6504 1900 6411 650c  e...d.e.e...d.e.
+00000620: 650d 6504 1900 1900 6412 650c 650d 6504  e.e.....d.e.e.e.
+00000630: 1900 1900 6413 650c 650d 6504 1900 1900  ....d.e.e.e.....
+00000640: 6414 650c 650d 6504 1900 1900 6415 650e  d.e.e.e.....d.e.
+00000650: 650b 1900 6416 650c 6400 1900 6417 650b  e...d.e.d...d.e.
+00000660: 6616 8700 6601 6418 6419 840e 5a0f 641a  f...f.d.d...Z.d.
+00000670: 6504 6602 641b 641c 8404 5a10 090b 091d  e.f.d.d...Z.....
+00000680: 646a 641e 650c 6511 6504 1900 1900 641f  djd.e.e.e.....d.
+00000690: 6512 6420 640b 6606 8700 6601 6421 6422  e.d d.f...f.d!d"
+000006a0: 840d 5a13 6423 6514 6515 6424 650b 6602  ..Z.d#e.e.d$e.f.
+000006b0: 1900 650e 6516 1900 6602 1900 6420 640b  ..e.e...f...d d.
+000006c0: 6604 6425 6426 8404 5a17 090b 646b 6423  f.d%d&..Z...dkd#
+000006d0: 6514 6515 6424 650b 6602 1900 650e 6516  e.e.d$e.f...e.e.
+000006e0: 1900 6602 1900 6427 650c 6504 1900 6417  ..f...d'e.e...d.
+000006f0: 650b 6420 6518 6a19 6608 6428 6429 8405  e.d e.j.f.d(d)..
+00000700: 5a1a 090b 646b 642a 6515 6424 650b 6602  Z...dkd*e.d$e.f.
+00000710: 1900 6427 650c 6504 1900 6417 650b 6420  ..d'e.e...d.e.d 
+00000720: 640b 6608 642b 642c 8405 5a1b 651c 642d  d.f.d+d,..Z.e.d-
+00000730: 650e 6516 1900 642e 6504 6420 6512 6606  e.e...d.e.d e.f.
+00000740: 642f 6430 8404 8301 5a1d 651e 6431 6518  d/d0....Z.e.d1e.
+00000750: 6a19 6423 6514 6515 6424 650b 6602 1900  j.d#e.e.d$e.f...
+00000760: 650e 6516 1900 6602 1900 6420 650d 651f  e.e...f...d e.e.
+00000770: 1900 6606 6432 6433 8404 8301 5a20 651c  ..f.d2d3....Z e.
+00000780: 6434 650e 650b 1900 6420 650c 650e 650b  d4e.e...d e.e.e.
+00000790: 1900 1900 6604 6435 6436 8404 8301 5a21  ....f.d5d6....Z!
+000007a0: 651c 6434 650e 650b 1900 6420 6522 650e  e.d4e.e...d e"e.
+000007b0: 650b 1900 6424 6602 1900 6604 6437 6438  e...d$f...f.d7d8
+000007c0: 8404 8301 5a23 651c 6434 650e 650b 1900  ....Z#e.d4e.e...
+000007d0: 6420 6522 650e 650b 1900 6424 6602 1900  d e"e.e...d$f...
+000007e0: 6604 6439 643a 8404 8301 5a24 651e 091d  f.d9d:....Z$e...
+000007f0: 091d 646c 643b 650e 650b 1900 643c 6512  ..dld;e.e...d<e.
+00000800: 643d 6512 6420 650e 650b 1900 6608 643e  d=e.d e.e...f.d>
+00000810: 643f 8405 8301 5a25 6420 6518 6a26 6602  d?....Z%d e.j&f.
+00000820: 8700 6601 6440 6441 840c 5a27 6420 650c  ..f.d@dA..Z'd e.
+00000830: 6518 6a26 1900 6602 6442 6443 8404 5a28  e.j&..f.dBdC..Z(
+00000840: 6420 6518 6a26 6602 6444 6445 8404 5a29  d e.j&f.dDdE..Z)
+00000850: 6446 6518 6a2a 6420 652a 6604 6447 6448  dFe.j*d e*f.dGdH
+00000860: 8404 5a2b 090b 090b 646d 640d 650c 652c  ..Z+....dmd.e.e,
+00000870: 6504 1900 1900 6446 650c 6518 6a2a 1900  e.....dFe.e.j*..
+00000880: 6420 652a 6606 8700 6601 6449 644a 840d  d e*f...f.dIdJ..
+00000890: 5a2d 090b 090b 646d 640d 650c 652c 6504  Z-....dmd.e.e,e.
+000008a0: 1900 1900 6446 650c 6518 6a2a 1900 6420  ....dFe.e.j*..d 
+000008b0: 6522 652a 650d 6504 1900 6602 1900 6606  e"e*e.e...f...f.
+000008c0: 8700 6601 644b 644c 840d 5a2e 090b 090b  ..f.dKdL..Z.....
+000008d0: 091d 646e 640d 650c 652c 6504 1900 1900  ..dnd.e.e,e.....
+000008e0: 6423 650c 650e 6516 1900 1900 644d 6512  d#e.e.e.....dMe.
+000008f0: 6420 6522 6516 650d 6504 1900 6602 1900  d e"e.e.e...f...
+00000900: 6608 644e 644f 8405 5a2f 090b 090b 091d  f.dNdO..Z/......
+00000910: 646e 640d 650c 652c 6504 1900 1900 6423  dnd.e.e,e.....d#
+00000920: 650c 650e 6516 1900 1900 644d 6512 6420  e.e.e.....dMe.d 
+00000930: 6516 6608 6450 6451 8405 5a30 090b 091d  e.f.dPdQ..Z0....
+00000940: 646a 640d 6518 6a2a 6423 650c 650e 6516  djd.e.j*d#e.e.e.
+00000950: 1900 1900 644d 6512 6420 6516 6608 6452  ....dMe.d e.f.dR
+00000960: 6453 8405 5a31 651c 6454 6532 6504 650b  dS..Z1e.dTe2e.e.
+00000970: 6602 1900 6423 650e 6516 1900 6420 6532  f...d#e.e...d e2
+00000980: 6504 650b 6602 1900 6606 6455 6456 8404  e.e.f...f.dUdV..
+00000990: 8301 5a33 651e 6423 6514 6515 6424 650b  ..Z3e.d#e.e.d$e.
+000009a0: 6602 1900 650e 6516 1900 6602 1900 6420  f...e.e...f...d 
+000009b0: 650c 6504 1900 6604 6457 6458 8404 8301  e.e...f.dWdX....
+000009c0: 5a34 651e 6431 6518 6a19 6423 6514 6515  Z4e.d1e.j.d#e.e.
+000009d0: 6424 650b 6602 1900 650e 6516 1900 6602  d$e.f...e.e...f.
+000009e0: 1900 6420 640b 6606 6459 645a 8404 8301  ..d d.f.dYdZ....
+000009f0: 5a35 651e 090b 090b 090b 646f 6431 6400  Z5e.......dod1d.
+00000a00: 642a 6515 6424 650b 6602 1900 640d 650d  d*e.d$e.f...d.e.
+00000a10: 6504 1900 6423 650c 650e 650b 1900 1900  e...d#e.e.e.....
+00000a20: 645b 650c 6515 6424 650b 6602 1900 1900  d[e.e.d$e.f.....
+00000a30: 645c 650c 650b 1900 6420 650b 660e 645d  d\e.e...d e.f.d]
+00000a40: 645e 8405 8301 5a36 651e 090b 090b 090b  d^....Z6e.......
+00000a50: 646f 645f 650c 6515 6424 650b 6602 1900  dod_e.e.d$e.f...
+00000a60: 1900 6460 650c 652c 6515 6424 650b 6602  ..d`e.e,e.d$e.f.
+00000a70: 1900 1900 1900 6461 650c 6532 6504 6515  ......dae.e2e.e.
+00000a80: 6424 650b 6602 1900 6602 1900 1900 6417  d$e.f...f.....d.
+00000a90: 650b 6420 6400 660a 6462 6463 8405 8301  e.d d.f.dbdc....
+00000aa0: 5a37 651e 640b 640b 6464 9c02 6465 650b  Z7e.d.d.dd..dee.
+00000ab0: 640d 650c 650d 6504 1900 1900 6466 650c  d.e.e.e.....dfe.
+00000ac0: 650d 6504 1900 1900 6467 650b 6420 650b  e.e.....dge.d e.
+00000ad0: 660a 6468 6469 8406 8301 5a38 8700 0400  f.dhdi....Z8....
+00000ae0: 5a39 5300 2970 da0e 4172 6775 6d65 6e74  Z9S.)p..Argument
+00000af0: 5061 7273 6572 5a0a 5f72 6f6f 745f 6675  ParserZ._root_fu
+00000b00: 6e63 da13 524f 4f54 5f46 554e 435f 4154  nc..ROOT_FUNC_AT
+00000b10: 5452 5f4e 414d 455a 155f 726f 6f74 5f66  TR_NAMEZ._root_f
+00000b20: 756e 635f 6172 6773 5f6d 6f64 656c da18  unc_args_model..
+00000b30: 524f 4f54 5f46 554e 435f 4152 4753 5f41  ROOT_FUNC_ARGS_A
+00000b40: 5454 525f 4e41 4d45 5a08 5f63 6f6d 6d61  TTR_NAMEZ._comma
+00000b50: 6e64 da0d 434d 445f 4154 5452 5f4e 414d  nd..CMD_ATTR_NAM
+00000b60: 455a 0d5f 636f 6d6d 616e 645f 6675 6e63  EZ._command_func
+00000b70: da12 434d 445f 4655 4e43 5f41 5454 525f  ..CMD_FUNC_ATTR_
+00000b80: 4e41 4d45 5a18 5f63 6f6d 6d61 6e64 5f66  NAMEZ._command_f
+00000b90: 756e 635f 6172 6773 5f6d 6f64 656c da17  unc_args_model..
+00000ba0: 434d 445f 4655 4e43 5f41 5247 535f 4154  CMD_FUNC_ARGS_AT
+00000bb0: 5452 5f4e 414d 454e 2909 da04 7072 6f67  TR_NAMEN)...prog
+00000bc0: da0c 7072 6f67 5f76 6572 7369 6f6e da0b  ..prog_version..
+00000bd0: 6465 7363 7269 7074 696f 6eda 0a68 656c  description..hel
+00000be0: 705f 666c 6167 73da 0d76 6572 7369 6f6e  p_flags..version
+00000bf0: 5f66 6c61 6773 da09 7475 695f 666c 6167  _flags..tui_flag
+00000c00: 73da 1063 6f6d 706c 6574 696f 6e5f 666c  s..completion_fl
+00000c10: 6167 73da 0f66 6f72 6d61 7474 6572 5f63  ags..formatter_c
+00000c20: 6c61 7373 da0e 5f70 6172 656e 745f 7061  lass.._parent_pa
+00000c30: 7273 6572 da04 6172 6773 7247 0000 0072  rser..argsrG...r
+00000c40: 4800 0000 7249 0000 0072 4a00 0000 724b  H...rI...rJ...rK
+00000c50: 0000 0072 4c00 0000 724d 0000 0072 4e00  ...rL...rM...rN.
+00000c60: 0000 724f 0000 00da 066b 7761 7267 7363  ..rO.....kwargsc
+00000c70: 0100 0000 0000 0000 0900 0000 0e00 0000  ................
+00000c80: 0800 0000 0f00 0000 732e 0200 007c 0972  ........s....|.r
+00000c90: 1564 007d 037c 096a 007d 087c 0464 0075  .d.}.|.j.}.|.d.u
+00000ca0: 0072 0e7c 096a 017d 047c 0664 0075 0072  .r.|.j.}.|.d.u.r
+00000cb0: 157c 096a 027d 0674 0383 006a 047c 0a7c  .|.j.}.t...j.|.|
+00000cc0: 0164 017c 037c 0864 029c 047c 0ba4 018e  .d.|.|.d...|....
+00000cd0: 0101 007c 047c 005f 017c 067c 005f 0264  ...|.|._.|.|._.d
+00000ce0: 007c 005f 0564 037c 006a 065f 077c 0464  .|._.d.|.j._.|.d
+00000cf0: 0075 0072 3864 0464 0567 027d 047c 0472  .u.r8d.d.g.}.|.r
+00000d00: 4b74 087c 0474 0983 0272 427c 0467 017d  Kt.|.t...rB|.g.}
+00000d10: 047c 006a 0a7c 0474 0b64 0664 079c 028e  .|.j.|.t.d.d....
+00000d20: 0101 0064 087c 005f 0c74 0d64 0964 0a84  ...d.|._.t.d.d..
+00000d30: 0083 017c 005f 0e69 007c 005f 0f74 1072  ...|._.i.|._.t.r
+00000d40: 987c 0664 0075 0072 6264 0b67 017d 066e  .|.d.u.rbd.g.}.n
+00000d50: 0874 087c 0674 0983 0272 6a7c 0667 017d  .t.|.t...rj|.g.}
+00000d60: 0664 0c7d 0c74 117c 0683 0164 0d6b 0272  .d.}.t.|...d.k.r
+00000d70: 897c 0664 0e19 00a0 1264 0fa1 0173 897c  .|.d.....d...s.|
+00000d80: 0973 887c 00a0 13a1 0001 0074 147c 007c  .s.|.......t.|.|
+00000d90: 0664 0e19 007c 0c64 108d 0301 006e 0f64  .d...|.d.....n.d
+00000da0: 1164 1284 007c 0644 0083 017d 0674 157c  .d...|.D...}.t.|
+00000db0: 007c 097c 067c 0c64 138d 0401 007c 0990  .|.|.|.d.....|..
+00000dc0: 0173 117c 0472 ad64 1464 1284 007c 0444  .s.|.r.d.d...|.D
+00000dd0: 0083 017d 0d7c 006a 0a7c 0d74 1664 1564  ...}.|.j.|.t.d.d
+00000de0: 079c 028e 0101 007c 0564 0075 0072 b464  .......|.d.u.r.d
+00000df0: 1667 017d 057c 0572 ec74 087c 0574 0983  .g.}.|.r.t.|.t..
+00000e00: 0272 be7c 0567 017d 057c 006a 1772 dd7c  .r.|.g.}.|.j.r.|
+00000e10: 0273 dd74 1874 1983 018f 0e01 0074 1a7c  .s.t.t.......t.|
+00000e20: 006a 1783 016a 1b7d 0257 0064 0004 0004  .j...j.}.W.d....
+00000e30: 0083 0301 006e 0831 0073 d877 0101 0001  .....n.1.s.w....
+00000e40: 0001 0059 0001 007c 0272 ec7c 006a 0a7c  ...Y...|.r.|.j.|
+00000e50: 0564 1764 187c 029b 009d 0264 1964 1a9c  .d.d.|.....d.d..
+00000e60: 038e 0101 007c 0764 0075 0072 f364 1b67  .....|.d.u.r.d.g
+00000e70: 017d 0774 1c90 0172 137c 0790 0172 1574  .}.t...r.|...r.t
+00000e80: 087c 0774 0983 0290 0172 027c 0767 017d  .|.t.....r.|.g.}
+00000e90: 077c 006a 0a7c 0774 1d83 0074 1e6a 1f74  .|.j.|.t...t.j.t
+00000ea0: 2064 1c64 1d9c 048e 0101 0064 0053 0064   d.d.......d.S.d
+00000eb0: 0053 0064 0053 0064 0053 0029 1e4e 4629  .S.d.S.d.S.).NF)
+00000ec0: 0472 4700 0000 da08 6164 645f 6865 6c70  .rG.....add_help
+00000ed0: 7249 0000 0072 4e00 0000 7a12 6865 6c70  rI...rN...z.help
+00000ee0: 6675 6c20 7061 7261 6d65 7465 7273 7a02  ful parametersz.
+00000ef0: 2d68 7a06 2d2d 6865 6c70 7a17 5368 6f77  -hz.--helpz.Show
+00000f00: 2074 6869 7320 6865 6c70 206d 6573 7361   this help messa
+00000f10: 6765 2e29 02da 0661 6374 696f 6eda 0468  ge.)...action..h
+00000f20: 656c 70fa 013d 6300 0000 0000 0000 0000  elp..=c.........
+00000f30: 0000 0000 0000 0002 0000 0053 0000 0073  ...........S...s
+00000f40: 0800 0000 7400 7401 8301 5300 a901 4e29  ....t.t...S...N)
+00000f50: 0272 0200 0000 da04 6c69 7374 a900 7258  .r......list..rX
+00000f60: 0000 0072 5800 0000 fa26 2f64 726f 6e65  ...rX....&/drone
+00000f70: 2f73 7263 2f73 7263 2f79 6170 782f 6172  /src/src/yapx/ar
+00000f80: 6775 6d65 6e74 5f70 6172 7365 722e 7079  gument_parser.py
+00000f90: da08 3c6c 616d 6264 613e 8b00 0000 7302  ..<lambda>....s.
+00000fa0: 0000 0008 007a 2941 7267 756d 656e 7450  .....z)ArgumentP
+00000fb0: 6172 7365 722e 5f5f 696e 6974 5f5f 2e3c  arser.__init__.<
+00000fc0: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
+00000fd0: 7a05 2d2d 7475 697a 2253 686f 7720 5465  z.--tuiz"Show Te
+00000fe0: 7874 7561 6c20 5573 6572 2049 6e74 6572  xtual User Inter
+00000ff0: 6661 6365 2028 5455 4929 2e72 1700 0000  face (TUI).r....
+00001000: 7201 0000 00fa 012d 2903 da06 7061 7273  r......-)...pars
+00001010: 6572 da07 636f 6d6d 616e 6472 5400 0000  er..commandrT...
+00001020: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00001030: 0005 0000 0053 0000 0073 3a00 0000 6700  .....S...s:...g.
+00001040: 7c00 5d19 7d01 7c01 a000 6400 a101 720b  |.].}.|...d...r.
+00001050: 7c01 6e0f 7401 7c01 8301 6401 6b04 7216  |.n.t.|...d.k.r.
+00001060: 6402 7c01 9b00 9d02 6e04 6400 7c01 9b00  d.|.....n.d.|...
+00001070: 9d02 9102 7102 5300 2903 725b 0000 0072  ....q.S.).r[...r
+00001080: 1700 0000 fa02 2d2d 2902 da0a 7374 6172  ......--)...star
+00001090: 7473 7769 7468 da03 6c65 6ea9 02da 022e  tswith..len.....
+000010a0: 30da 0178 7258 0000 0072 5800 0000 7259  0..xrX...rX...rY
+000010b0: 0000 00da 0a3c 6c69 7374 636f 6d70 3ea0  .....<listcomp>.
+000010c0: 0000 0073 0800 0000 0600 0202 2cff 06ff  ...s........,...
+000010d0: 7a2b 4172 6775 6d65 6e74 5061 7273 6572  z+ArgumentParser
+000010e0: 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63 616c  .__init__.<local
+000010f0: 733e 2e3c 6c69 7374 636f 6d70 3e29 0472  s>.<listcomp>).r
+00001100: 5c00 0000 5a0d 7061 7265 6e74 5f70 6172  \...Z.parent_par
+00001110: 7365 72da 0e6f 7074 696f 6e5f 7374 7269  ser..option_stri
+00001120: 6e67 7372 5400 0000 6301 0000 0000 0000  ngsrT...c.......
+00001130: 0000 0000 0002 0000 0005 0000 0053 0000  .............S..
+00001140: 0073 2000 0000 6700 7c00 5d0c 7d01 7c01  .s ...g.|.].}.|.
+00001150: a000 6400 a101 7202 7c01 9b00 6401 9d02  ..d...r.|...d...
+00001160: 9102 7102 5300 2902 725e 0000 007a 042d  ..q.S.).r^...z.-
+00001170: 616c 6ca9 0172 5f00 0000 7261 0000 0072  all..r_...ra...r
+00001180: 5800 0000 7258 0000 0072 5900 0000 7264  X...rX...rY...rd
+00001190: 0000 00ad 0000 00f3 0200 0000 2000 7a1b  ............ .z.
+000011a0: 5368 6f77 2068 656c 7020 666f 7220 616c  Show help for al
+000011b0: 6c20 636f 6d6d 616e 6473 2e7a 092d 2d76  l commands.z.--v
+000011c0: 6572 7369 6f6e da07 7665 7273 696f 6e7a  ersion..versionz
+000011d0: 0925 2870 726f 6729 7320 7a20 5368 6f77  .%(prog)s z Show
+000011e0: 2074 6865 2070 726f 6772 616d 2076 6572   the program ver
+000011f0: 7369 6f6e 206e 756d 6265 722e 2903 7253  sion number.).rS
+00001200: 0000 0072 6800 0000 7254 0000 007a 182d  ...rh...rT...z.-
+00001210: 2d70 7269 6e74 2d73 6865 6c6c 2d63 6f6d  -print-shell-com
+00001220: 706c 6574 696f 6e7a 1e50 7269 6e74 2073  pletionz.Print s
+00001230: 6865 6c6c 2063 6f6d 706c 6574 696f 6e20  hell completion 
+00001240: 7363 7269 7074 2e29 0472 5300 0000 da07  script.).rS.....
+00001250: 6465 6661 756c 74da 0763 686f 6963 6573  default..choices
+00001260: 7254 0000 0029 2172 4e00 0000 5a0b 5f68  rT...)!rN...Z._h
+00001270: 656c 705f 666c 6167 735a 0a5f 7475 695f  elp_flagsZ._tui_
+00001280: 666c 6167 73da 0573 7570 6572 da08 5f5f  flags..super..__
+00001290: 696e 6974 5f5f da12 5f73 7562 7061 7273  init__.._subpars
+000012a0: 6572 735f 6163 7469 6f6e da0a 5f6f 7074  ers_action.._opt
+000012b0: 696f 6e61 6c73 da05 7469 746c 65da 0a69  ionals..title..i
+000012c0: 7369 6e73 7461 6e63 65da 0373 7472 da0c  sinstance..str..
+000012d0: 6164 645f 6172 6775 6d65 6e74 721b 0000  add_argumentr...
+000012e0: 00da 0c6b 765f 7365 7061 7261 746f 7272  ...kv_separatorr
+000012f0: 0200 0000 da18 5f6d 7574 7561 6c6c 795f  ......_mutually_
+00001300: 6578 636c 7573 6976 655f 6172 6773 da0a  exclusive_args..
+00001310: 5f64 6573 745f 7479 7065 7237 0000 0072  _dest_typer7...r
+00001320: 6000 0000 725f 0000 00da 165f 6765 745f  `...r_....._get_
+00001330: 6f72 5f61 6464 5f73 7562 7061 7273 6572  or_add_subparser
+00001340: 7372 3000 0000 722f 0000 0072 1c00 0000  sr0...r/...r....
+00001350: 7247 0000 0072 0300 0000 da09 4578 6365  rG...r......Exce
+00001360: 7074 696f 6e72 1600 0000 7268 0000 0072  ptionr....rh...r
+00001370: 3600 0000 7232 0000 00da 0861 7267 7061  6...r2.....argpa
+00001380: 7273 65da 0853 5550 5052 4553 5372 2c00  rse..SUPPRESSr,.
+00001390: 0000 290e da04 7365 6c66 7247 0000 0072  ..)...selfrG...r
+000013a0: 4800 0000 7249 0000 0072 4a00 0000 724b  H...rI...rJ...rK
+000013b0: 0000 0072 4c00 0000 724d 0000 0072 4e00  ...rL...rM...rN.
+000013c0: 0000 724f 0000 0072 5000 0000 7251 0000  ..rO...rP...rQ..
+000013d0: 005a 0874 7569 5f68 656c 705a 0e68 656c  .Z.tui_helpZ.hel
+000013e0: 705f 616c 6c5f 666c 6167 73a9 01da 095f  p_all_flags...._
+000013f0: 5f63 6c61 7373 5f5f 7258 0000 0072 5900  _class__rX...rY.
+00001400: 0000 726c 0000 0053 0000 0073 c000 0000  ..rl...S...s....
+00001410: 040e 0401 0601 0801 0601 0801 0601 0602  ................
+00001420: 0201 0201 0201 0201 0201 04fb 0206 06fa  ................
+00001430: 0609 0601 0602 0803 0802 0801 0402 0a01  ................
+00001440: 0601 0401 0201 0201 0201 08fd 0606 0a05  ................
+00001450: 04fd 0605 0402 0801 0801 0a01 0601 0402  ................
+00001460: 1a02 0401 0801 0201 0201 0601 0201 06fd  ................
+00001470: 0280 0606 0202 06fe 0204 0201 0201 0201  ................
+00001480: 0201 06fc 0607 0401 0e01 0401 0201 0201  ................
+00001490: 0201 08fd 0806 0601 0402 0a01 0601 0a02  ................
+000014a0: 0a01 0e01 1cff 0403 0401 0201 0201 0801  ................
+000014b0: 0201 08fc 0807 0601 0c02 0c01 0601 0402  ................
+000014c0: 0201 0401 0401 0201 0201 0cfb 04dd 081f  ................
+000014d0: 7a17 4172 6775 6d65 6e74 5061 7273 6572  z.ArgumentParser
+000014e0: 2e5f 5f69 6e69 745f 5fda 076d 6573 7361  .__init__..messa
+000014f0: 6765 6302 0000 0000 0000 0000 0000 0002  gec.............
+00001500: 0000 0006 0000 0043 0000 0073 2400 0000  .......C...s$...
+00001510: 7c00 a000 7401 6a02 a101 0100 7c00 a003  |...t.j.....|...
+00001520: 6401 6402 7c01 9b00 6403 9d03 a102 0100  d.d.|...d.......
+00001530: 6400 5300 2904 4ee9 0200 0000 7a07 6572  d.S.).N.....z.er
+00001540: 726f 723a 20da 010a 2904 da0b 7072 696e  ror: ...)...prin
+00001550: 745f 7573 6167 65da 0373 7973 da06 7374  t_usage..sys..st
+00001560: 6465 7272 da04 6578 6974 2902 727a 0000  derr..exit).rz..
+00001570: 0072 7d00 0000 7258 0000 0072 5800 0000  .r}...rX...rX...
+00001580: 7259 0000 00da 0565 7272 6f72 d600 0000  rY.....error....
+00001590: 7304 0000 000c 0118 017a 1441 7267 756d  s........z.Argum
+000015a0: 656e 7450 6172 7365 722e 6572 726f 7246  entParser.errorF
+000015b0: da04 6669 6c65 da10 696e 636c 7564 655f  ..file..include_
+000015c0: 636f 6d6d 616e 6473 da06 7265 7475 726e  commands..return
+000015d0: 6303 0000 0000 0000 0000 0000 0008 0000  c...............
+000015e0: 0005 0000 0003 0000 0073 9c00 0000 6401  .........s....d.
+000015f0: 7d03 7c03 6402 1400 6403 1700 7d04 7400  }.|.d...d...}.t.
+00001600: 8300 0100 7400 7c04 8301 0100 7400 6404  ....t.|.....t.d.
+00001610: 7c00 6a01 9b00 9d02 8301 0100 7400 7c04  |.j.........t.|.
+00001620: 8301 0100 7c00 6a02 7d05 7403 6a04 7c00  ....|.j.}.t.j.|.
+00001630: 5f02 7405 8300 a006 7c01 a101 0100 7c02  _.t.....|.....|.
+00001640: 7249 7c00 6a07 7249 7c00 6a08 6405 7500  rI|.j.rI|.j.d.u.
+00001650: 7237 7c00 a009 a100 7c00 5f08 7c00 6a08  r7|.....|._.|.j.
+00001660: 6a0a a00b a100 4400 5d0b 5c02 7d06 7d07  j.....D.].\.}.}.
+00001670: 7c07 6a06 7c01 7c02 6406 8d02 0100 713d  |.j.|.|.d.....q=
+00001680: 7c05 7c00 5f02 6405 5300 2907 6118 0200  |.|._.d.S.).a...
+00001690: 0050 7269 6e74 2043 4c49 2068 656c 702e  .Print CLI help.
+000016a0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+000016b0: 2020 2020 2020 2020 2020 2020 696e 636c              incl
+000016c0: 7564 655f 636f 6d6d 616e 6473 3a20 6966  ude_commands: if
+000016d0: 2054 7275 652c 2061 6c73 6f20 7072 696e   True, also prin
+000016e0: 7420 6865 6c70 2066 6f72 2065 6163 6820  t help for each 
+000016f0: 636f 6d6d 616e 642e 0a0a 2020 2020 2020  command...      
+00001700: 2020 4578 616d 706c 6573 3a0a 2020 2020    Examples:.    
+00001710: 2020 2020 2020 2020 3e3e 3e20 696d 706f          >>> impo
+00001720: 7274 2079 6170 780a 2020 2020 2020 2020  rt yapx.        
+00001730: 2020 2020 3e3e 3e20 6672 6f6d 2064 6174      >>> from dat
+00001740: 6163 6c61 7373 6573 2069 6d70 6f72 7420  aclasses import 
+00001750: 6461 7461 636c 6173 730a 2020 2020 2020  dataclass.      
+00001760: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
+00001770: 2020 2020 2020 3e3e 3e20 4064 6174 6163        >>> @datac
+00001780: 6c61 7373 0a20 2020 2020 2020 2020 2020  lass.           
+00001790: 202e 2e2e 2063 6c61 7373 2041 6464 4e75   ... class AddNu
+000017a0: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
+000017b0: 2e2e 2e20 2020 2020 783a 2069 6e74 0a20  ...     x: int. 
+000017c0: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
+000017d0: 2020 2079 3a20 696e 740a 2020 2020 2020     y: int.      
+000017e0: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
+000017f0: 2020 2020 2020 3e3e 3e20 7061 7273 6572        >>> parser
+00001800: 203d 2079 6170 782e 4172 6775 6d65 6e74   = yapx.Argument
+00001810: 5061 7273 6572 2829 0a20 2020 2020 2020  Parser().       
+00001820: 2020 2020 203e 3e3e 2070 6172 7365 722e       >>> parser.
+00001830: 6164 645f 6172 6775 6d65 6e74 7328 4164  add_arguments(Ad
+00001840: 644e 756d 7329 0a20 2020 2020 2020 2020  dNums).         
+00001850: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
+00001860: 2020 203e 3e3e 2070 6172 7365 722e 7072     >>> parser.pr
+00001870: 696e 745f 6865 6c70 2869 6e63 6c75 6465  int_help(include
+00001880: 5f63 6f6d 6d61 6e64 733d 5472 7565 2920  _commands=True) 
+00001890: 2023 646f 6374 6573 743a 202b 534b 4950   #doctest: +SKIP
+000018a0: 0a20 2020 2020 2020 20da 015f e950 0000  .        .._.P..
+000018b0: 0072 7f00 0000 7a02 2420 4e29 0172 8600  .r....z.$ N).r..
+000018c0: 0000 290c da05 7072 696e 7472 4700 0000  ..)...printrG...
+000018d0: da05 7573 6167 6572 7800 0000 7279 0000  ..usagerx...ry..
+000018e0: 0072 6b00 0000 da0a 7072 696e 745f 6865  .rk.....print_he
+000018f0: 6c70 da0b 5f73 7562 7061 7273 6572 7372  lp.._subparsersr
+00001900: 6d00 0000 da17 5f66 696e 645f 7375 6270  m....._find_subp
+00001910: 6172 7365 7273 5f61 6374 696f 6e72 6a00  arsers_actionrj.
+00001920: 0000 da05 6974 656d 7329 0872 7a00 0000  ....items).rz...
+00001930: 7285 0000 0072 8600 0000 5a08 7365 705f  r....r....Z.sep_
+00001940: 6368 6172 da09 7365 7061 7261 746f 7272  char..separatorr
+00001950: 8b00 0000 5a07 5f63 686f 6963 655a 0973  ....Z._choiceZ.s
+00001960: 7562 7061 7273 6572 727b 0000 0072 5800  ubparserr{...rX.
+00001970: 0000 7259 0000 0072 8c00 0000 da00 0000  ..rY...r........
+00001980: 731e 0000 0004 180c 0106 0108 0110 0108  s...............
+00001990: 0106 0308 010c 020a 020a 010a 0114 0210  ................
+000019a0: 010a 027a 1941 7267 756d 656e 7450 6172  ...z.ArgumentPar
+000019b0: 7365 722e 7072 696e 745f 6865 6c70 da0a  ser.print_help..
+000019c0: 6172 6773 5f6d 6f64 656c 2e63 0200 0000  args_model.c....
+000019d0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+000019e0: 4300 0000 7310 0000 007c 00a0 007c 007c  C...s....|...|.|
+000019f0: 01a1 0201 0064 0153 0029 0261 d605 0000  .....d.S.).a....
+00001a00: 4164 6420 6172 6775 6d65 6e74 7320 6672  Add arguments fr
+00001a10: 6f6d 2074 6865 2067 6976 656e 2066 756e  om the given fun
+00001a20: 6374 696f 6e20 6f72 2064 6174 6166 7261  ction or datafra
+00001a30: 6d65 2e0a 0a20 2020 2020 2020 2041 7267  me...        Arg
+00001a40: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
+00001a50: 7267 735f 6d6f 6465 6c3a 2061 2066 756e  rgs_model: a fun
+00001a60: 6374 696f 6e20 6f72 2064 6174 6163 6c61  ction or datacla
+00001a70: 7373 2066 726f 6d20 7768 6963 6820 746f  ss from which to
+00001a80: 2064 6572 6976 6520 6172 6775 6d65 6e74   derive argument
+00001a90: 732e 0a0a 2020 2020 2020 2020 4578 616d  s...        Exam
+00001aa0: 706c 6573 3a0a 2020 2020 2020 2020 2020  ples:.          
+00001ab0: 2020 3e3e 3e20 696d 706f 7274 2079 6170    >>> import yap
+00001ac0: 780a 2020 2020 2020 2020 2020 2020 3e3e  x.            >>
+00001ad0: 3e20 6672 6f6d 2064 6174 6163 6c61 7373  > from dataclass
+00001ae0: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00001af0: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
+00001b00: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+00001b10: 3e3e 3e20 4064 6174 6163 6c61 7373 0a20  >>> @dataclass. 
+00001b20: 2020 2020 2020 2020 2020 202e 2e2e 2063             ... c
+00001b30: 6c61 7373 2041 6464 4e75 6d73 3a0a 2020  lass AddNums:.  
+00001b40: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
+00001b50: 2020 783a 2069 6e74 0a20 2020 2020 2020    x: int.       
+00001b60: 2020 2020 202e 2e2e 2020 2020 2079 3a20       ...     y: 
+00001b70: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+00001b80: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+00001b90: 3e3e 3e20 7061 7273 6572 203d 2079 6170  >>> parser = yap
+00001ba0: 782e 4172 6775 6d65 6e74 5061 7273 6572  x.ArgumentParser
+00001bb0: 2829 0a20 2020 2020 2020 2020 2020 203e  ().            >
+00001bc0: 3e3e 2070 6172 7365 722e 6164 645f 6172  >> parser.add_ar
+00001bd0: 6775 6d65 6e74 7328 4164 644e 756d 7329  guments(AddNums)
+00001be0: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+00001bf0: 2070 6172 7365 722e 7365 745f 6465 6661   parser.set_defa
+00001c00: 756c 7473 285f 636f 6d6d 616e 645f 6675  ults(_command_fu
+00001c10: 6e63 3d6c 616d 6264 6120 782c 2079 3a20  nc=lambda x, y: 
+00001c20: 782b 7929 0a20 2020 2020 2020 2020 2020  x+y).           
+00001c30: 203e 3e3e 2070 6172 7365 6420 3d20 7061   >>> parsed = pa
+00001c40: 7273 6572 2e70 6172 7365 5f61 7267 7328  rser.parse_args(
+00001c50: 5b27 2d78 272c 2027 3127 2c20 272d 7927  ['-x', '1', '-y'
+00001c60: 2c20 2732 275d 290a 2020 2020 2020 2020  , '2']).        
+00001c70: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
+00001c80: 2020 2020 3e3e 3e20 2870 6172 7365 642e      >>> (parsed.
+00001c90: 782c 2070 6172 7365 642e 7929 0a20 2020  x, parsed.y).   
+00001ca0: 2020 2020 2020 2020 2028 312c 2032 290a           (1, 2).
+00001cb0: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00001cc0: 7061 7273 6564 2e5f 636f 6d6d 616e 645f  parsed._command_
+00001cd0: 6675 6e63 5f61 7267 735f 6d6f 6465 6c28  func_args_model(
+00001ce0: 783d 7061 7273 6564 2e78 2c20 793d 7061  x=parsed.x, y=pa
+00001cf0: 7273 6564 2e79 290a 2020 2020 2020 2020  rsed.y).        
+00001d00: 2020 2020 4164 644e 756d 7328 783d 312c      AddNums(x=1,
+00001d10: 2079 3d32 290a 2020 2020 2020 2020 2020   y=2).          
+00001d20: 2020 3e3e 3e20 7061 7273 6564 2e5f 636f    >>> parsed._co
+00001d30: 6d6d 616e 645f 6675 6e63 2878 3d70 6172  mmand_func(x=par
+00001d40: 7365 642e 782c 2079 3d70 6172 7365 642e  sed.x, y=parsed.
+00001d50: 7929 0a20 2020 2020 2020 2020 2020 2033  y).            3
+00001d60: 0a0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
+00001d70: 3e20 696d 706f 7274 2079 6170 780a 2020  > import yapx.  
+00001d80: 2020 2020 2020 2020 2020 2e2e 2e0a 2020            ....  
+00001d90: 2020 2020 2020 2020 2020 3e3e 3e20 6465            >>> de
+00001da0: 6620 6164 645f 6e75 6d73 2878 3a20 696e  f add_nums(x: in
+00001db0: 742c 2079 3a20 696e 7429 3a0a 2020 2020  t, y: int):.    
+00001dc0: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
+00001dd0: 7265 7475 726e 2078 202b 2079 0a20 2020  return x + y.   
+00001de0: 2020 2020 2020 2020 202e 2e2e 0a20 2020           ....   
+00001df0: 2020 2020 2020 2020 203e 3e3e 2070 6172           >>> par
+00001e00: 7365 7220 3d20 7961 7078 2e41 7267 756d  ser = yapx.Argum
+00001e10: 656e 7450 6172 7365 7228 290a 2020 2020  entParser().    
+00001e20: 2020 2020 2020 2020 3e3e 3e20 7061 7273          >>> pars
+00001e30: 6572 2e61 6464 5f61 7267 756d 656e 7473  er.add_arguments
+00001e40: 2861 6464 5f6e 756d 7329 0a20 2020 2020  (add_nums).     
+00001e50: 2020 2020 2020 203e 3e3e 2070 6172 7365         >>> parse
+00001e60: 722e 7365 745f 6465 6661 756c 7473 285f  r.set_defaults(_
+00001e70: 636f 6d6d 616e 645f 6675 6e63 3d61 6464  command_func=add
+00001e80: 5f6e 756d 7329 0a20 2020 2020 2020 2020  _nums).         
+00001e90: 2020 203e 3e3e 2070 6172 7365 6420 3d20     >>> parsed = 
+00001ea0: 7061 7273 6572 2e70 6172 7365 5f61 7267  parser.parse_arg
+00001eb0: 7328 5b27 2d78 272c 2027 3127 2c20 272d  s(['-x', '1', '-
+00001ec0: 7927 2c20 2732 275d 290a 2020 2020 2020  y', '2']).      
+00001ed0: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
+00001ee0: 2020 2020 2020 3e3e 3e20 2870 6172 7365        >>> (parse
+00001ef0: 642e 782c 2070 6172 7365 642e 7929 0a20  d.x, parsed.y). 
+00001f00: 2020 2020 2020 2020 2020 2028 312c 2032             (1, 2
+00001f10: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
+00001f20: 3e20 7061 7273 6564 2e5f 636f 6d6d 616e  > parsed._comman
+00001f30: 645f 6675 6e63 5f61 7267 735f 6d6f 6465  d_func_args_mode
+00001f40: 6c28 783d 7061 7273 6564 2e78 2c20 793d  l(x=parsed.x, y=
+00001f50: 7061 7273 6564 2e79 290a 2020 2020 2020  parsed.y).      
+00001f60: 2020 2020 2020 4461 7461 636c 6173 735f        Dataclass_
+00001f70: 6164 645f 6e75 6d73 2878 3d31 2c20 793d  add_nums(x=1, y=
+00001f80: 3229 0a20 2020 2020 2020 2020 2020 203e  2).            >
+00001f90: 3e3e 2070 6172 7365 642e 5f63 6f6d 6d61  >> parsed._comma
+00001fa0: 6e64 5f66 756e 6328 783d 7061 7273 6564  nd_func(x=parsed
+00001fb0: 2e78 2c20 793d 7061 7273 6564 2e79 290a  .x, y=parsed.y).
+00001fc0: 2020 2020 2020 2020 2020 2020 330a 2020              3.  
+00001fd0: 2020 2020 2020 4e29 01da 0e5f 6164 645f        N)..._add_
+00001fe0: 6172 6775 6d65 6e74 7329 0272 7a00 0000  arguments).rz...
+00001ff0: 7291 0000 0072 5800 0000 7258 0000 0072  r....rX...rX...r
+00002000: 5900 0000 da0d 6164 645f 6172 6775 6d65  Y.....add_argume
+00002010: 6e74 7308 0100 0073 0200 0000 102f 7a1c  nts....s...../z.
+00002020: 4172 6775 6d65 6e74 5061 7273 6572 2e61  ArgumentParser.a
+00002030: 6464 5f61 7267 756d 656e 7473 da04 6e61  dd_arguments..na
+00002040: 6d65 6303 0000 0000 0000 0000 0000 0009  mec.............
+00002050: 0000 0005 0000 004b 0000 0073 9800 0000  .......K...s....
+00002060: 7c00 a000 a100 7d04 7c02 730b 7401 7c01  |.....}.|.s.t.|.
+00002070: 6a02 8301 7d02 7403 7c04 7404 6a05 8302  j...}.t.|.t.j...
+00002080: 7313 4a00 8201 7c03 a006 6401 6402 a102  s.J...|...d.d...
+00002090: 7d05 7c05 7221 7c05 6403 7c02 1700 3700  }.|.r!|.d.|...7.
+000020a0: 7d05 7c00 6a07 7c01 6404 8d01 7d06 6402  }.|.j.|.d...}.d.
+000020b0: 7d07 7c06 7231 7c06 a008 a100 6405 1900  }.|.r1|.....d...
+000020c0: 7d07 7c04 6a09 7c02 6601 7c05 7c07 6406  }.|.j.|.f.|.|.d.
+000020d0: 9c02 7c03 a401 8e01 7d08 7c06 7242 7c06  ..|.....}.|.rB|.
+000020e0: 7c08 5f0a 7c01 724a 7c00 a00b 7c08 7c01  |._.|.rJ|...|.|.
+000020f0: a102 0100 7c08 5300 2907 6159 0800 0043  ....|.S.).aY...C
+00002100: 7265 6174 6520 6120 6e65 7720 7375 6263  reate a new subc
+00002110: 6f6d 6d61 6e64 2061 6e64 2061 6464 2061  ommand and add a
+00002120: 7267 756d 656e 7473 2066 726f 6d20 7468  rguments from th
+00002130: 6520 6769 7665 6e20 6675 6e63 7469 6f6e  e given function
+00002140: 206f 7220 6461 7461 6672 616d 6520 746f   or dataframe to
+00002150: 2069 742e 0a0a 2020 2020 2020 2020 4172   it...        Ar
+00002160: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00002170: 6172 6773 5f6d 6f64 656c 3a20 6120 6675  args_model: a fu
+00002180: 6e63 7469 6f6e 206f 7220 6461 7461 636c  nction or datacl
+00002190: 6173 7320 6672 6f6d 2077 6869 6368 2074  ass from which t
+000021a0: 6f20 6465 7269 7665 2061 7267 756d 656e  o derive argumen
+000021b0: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
+000021c0: 6e61 6d65 3a20 6e61 6d65 206f 6620 7468  name: name of th
+000021d0: 6520 636f 6d6d 616e 640a 0a20 2020 2020  e command..     
+000021e0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+000021f0: 2020 2020 2020 2020 7468 6520 6e65 7720          the new 
+00002200: 6172 6770 6172 7365 2073 7562 7061 7273  argparse subpars
+00002210: 6572 0a0a 2020 2020 2020 2020 4578 616d  er..        Exam
+00002220: 706c 6573 3a0a 2020 2020 2020 2020 2020  ples:.          
+00002230: 2020 3e3e 3e20 696d 706f 7274 2079 6170    >>> import yap
+00002240: 780a 2020 2020 2020 2020 2020 2020 3e3e  x.            >>
+00002250: 3e20 6672 6f6d 2064 6174 6163 6c61 7373  > from dataclass
+00002260: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00002270: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
+00002280: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+00002290: 3e3e 3e20 4064 6174 6163 6c61 7373 0a20  >>> @dataclass. 
+000022a0: 2020 2020 2020 2020 2020 202e 2e2e 2063             ... c
+000022b0: 6c61 7373 2041 6464 4e75 6d73 3a0a 2020  lass AddNums:.  
+000022c0: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
+000022d0: 2020 783a 2069 6e74 0a20 2020 2020 2020    x: int.       
+000022e0: 2020 2020 202e 2e2e 2020 2020 2079 3a20       ...     y: 
+000022f0: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+00002300: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+00002310: 3e3e 3e20 7061 7273 6572 203d 2079 6170  >>> parser = yap
+00002320: 782e 4172 6775 6d65 6e74 5061 7273 6572  x.ArgumentParser
+00002330: 2829 0a20 2020 2020 2020 2020 2020 203e  ().            >
+00002340: 3e3e 2073 7562 7061 7273 6572 5f31 203d  >> subparser_1 =
+00002350: 2070 6172 7365 722e 6164 645f 636f 6d6d   parser.add_comm
+00002360: 616e 6428 4164 644e 756d 732c 206e 616d  and(AddNums, nam
+00002370: 653d 2761 6464 2729 0a20 2020 2020 2020  e='add').       
+00002380: 2020 2020 203e 3e3e 2073 7562 7061 7273       >>> subpars
+00002390: 6572 5f31 2e73 6574 5f64 6566 6175 6c74  er_1.set_default
+000023a0: 7328 5f63 6f6d 6d61 6e64 5f66 756e 633d  s(_command_func=
+000023b0: 6c61 6d62 6461 2078 2c20 793a 2078 2b79  lambda x, y: x+y
+000023c0: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
+000023d0: 3e20 7375 6270 6172 7365 725f 3220 3d20  > subparser_2 = 
+000023e0: 7061 7273 6572 2e61 6464 5f63 6f6d 6d61  parser.add_comma
+000023f0: 6e64 2841 6464 4e75 6d73 2c20 6e61 6d65  nd(AddNums, name
+00002400: 3d27 7375 6274 7261 6374 2729 0a20 2020  ='subtract').   
+00002410: 2020 2020 2020 2020 203e 3e3e 2073 7562           >>> sub
+00002420: 7061 7273 6572 5f32 2e73 6574 5f64 6566  parser_2.set_def
+00002430: 6175 6c74 7328 5f63 6f6d 6d61 6e64 5f66  aults(_command_f
+00002440: 756e 633d 6c61 6d62 6461 2078 2c20 793a  unc=lambda x, y:
+00002450: 2078 2d79 290a 2020 2020 2020 2020 2020   x-y).          
+00002460: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
+00002470: 2020 3e3e 3e20 7061 7273 6564 203d 2070    >>> parsed = p
+00002480: 6172 7365 722e 7061 7273 655f 6172 6773  arser.parse_args
+00002490: 285b 2761 6464 272c 2027 2d78 272c 2027  (['add', '-x', '
+000024a0: 3127 2c20 272d 7927 2c20 2732 275d 290a  1', '-y', '2']).
+000024b0: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
+000024c0: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+000024d0: 2870 6172 7365 642e 782c 2070 6172 7365  (parsed.x, parse
+000024e0: 642e 7929 0a20 2020 2020 2020 2020 2020  d.y).           
+000024f0: 2028 312c 2032 290a 2020 2020 2020 2020   (1, 2).        
+00002500: 2020 2020 3e3e 3e20 7061 7273 6564 2e5f      >>> parsed._
+00002510: 636f 6d6d 616e 645f 6675 6e63 5f61 7267  command_func_arg
+00002520: 735f 6d6f 6465 6c28 783d 7061 7273 6564  s_model(x=parsed
+00002530: 2e78 2c20 793d 7061 7273 6564 2e79 290a  .x, y=parsed.y).
+00002540: 2020 2020 2020 2020 2020 2020 4164 644e              AddN
+00002550: 756d 7328 783d 312c 2079 3d32 290a 2020  ums(x=1, y=2).  
+00002560: 2020 2020 2020 2020 2020 3e3e 3e20 7061            >>> pa
+00002570: 7273 6564 2e5f 636f 6d6d 616e 645f 6675  rsed._command_fu
+00002580: 6e63 2878 3d70 6172 7365 642e 782c 2079  nc(x=parsed.x, y
+00002590: 3d70 6172 7365 642e 7929 0a20 2020 2020  =parsed.y).     
+000025a0: 2020 2020 2020 2033 0a0a 2020 2020 2020         3..      
+000025b0: 2020 2020 2020 3e3e 3e20 696d 706f 7274        >>> import
+000025c0: 2079 6170 780a 2020 2020 2020 2020 2020   yapx.          
+000025d0: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
+000025e0: 2020 3e3e 3e20 6465 6620 6164 645f 6e75    >>> def add_nu
+000025f0: 6d73 2878 3a20 696e 742c 2079 3a20 696e  ms(x: int, y: in
+00002600: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00002610: 2e2e 2e20 2020 2020 7265 7475 726e 2078  ...     return x
+00002620: 202b 2079 0a20 2020 2020 2020 2020 2020   + y.           
+00002630: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
+00002640: 203e 3e3e 2064 6566 2073 7562 7472 6163   >>> def subtrac
+00002650: 745f 6e75 6d73 2878 3a20 696e 742c 2079  t_nums(x: int, y
+00002660: 3a20 696e 7429 3a0a 2020 2020 2020 2020  : int):.        
+00002670: 2020 2020 2e2e 2e20 2020 2020 7265 7475      ...     retu
+00002680: 726e 2078 202d 2079 0a20 2020 2020 2020  rn x - y.       
+00002690: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
+000026a0: 2020 2020 203e 3e3e 2070 6172 7365 7220       >>> parser 
+000026b0: 3d20 7961 7078 2e41 7267 756d 656e 7450  = yapx.ArgumentP
+000026c0: 6172 7365 7228 290a 2020 2020 2020 2020  arser().        
+000026d0: 2020 2020 3e3e 3e20 7375 6270 6172 7365      >>> subparse
+000026e0: 725f 3120 3d20 7061 7273 6572 2e61 6464  r_1 = parser.add
+000026f0: 5f63 6f6d 6d61 6e64 2861 6464 5f6e 756d  _command(add_num
+00002700: 732c 206e 616d 653d 2761 6464 2729 0a20  s, name='add'). 
+00002710: 2020 2020 2020 2020 2020 203e 3e3e 2073             >>> s
+00002720: 7562 7061 7273 6572 5f31 2e73 6574 5f64  ubparser_1.set_d
+00002730: 6566 6175 6c74 7328 5f63 6f6d 6d61 6e64  efaults(_command
+00002740: 5f66 756e 633d 6164 645f 6e75 6d73 290a  _func=add_nums).
+00002750: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00002760: 7375 6270 6172 7365 725f 3220 3d20 7061  subparser_2 = pa
+00002770: 7273 6572 2e61 6464 5f63 6f6d 6d61 6e64  rser.add_command
+00002780: 2873 7562 7472 6163 745f 6e75 6d73 2c20  (subtract_nums, 
+00002790: 6e61 6d65 3d27 7375 6274 7261 6374 2729  name='subtract')
+000027a0: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+000027b0: 2073 7562 7061 7273 6572 5f32 2e73 6574   subparser_2.set
+000027c0: 5f64 6566 6175 6c74 7328 5f63 6f6d 6d61  _defaults(_comma
+000027d0: 6e64 5f66 756e 633d 7375 6274 7261 6374  nd_func=subtract
+000027e0: 5f6e 756d 7329 0a20 2020 2020 2020 2020  _nums).         
+000027f0: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
+00002800: 2020 203e 3e3e 2070 6172 7365 6420 3d20     >>> parsed = 
+00002810: 7061 7273 6572 2e70 6172 7365 5f61 7267  parser.parse_arg
+00002820: 7328 5b27 7375 6274 7261 6374 272c 2027  s(['subtract', '
+00002830: 2d78 272c 2027 3127 2c20 272d 7927 2c20  -x', '1', '-y', 
+00002840: 2732 275d 290a 2020 2020 2020 2020 2020  '2']).          
+00002850: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
+00002860: 2020 3e3e 3e20 2870 6172 7365 642e 782c    >>> (parsed.x,
+00002870: 2070 6172 7365 642e 7929 0a20 2020 2020   parsed.y).     
+00002880: 2020 2020 2020 2028 312c 2032 290a 2020         (1, 2).  
+00002890: 2020 2020 2020 2020 2020 3e3e 3e20 7061            >>> pa
+000028a0: 7273 6564 2e5f 636f 6d6d 616e 645f 6675  rsed._command_fu
+000028b0: 6e63 5f61 7267 735f 6d6f 6465 6c28 783d  nc_args_model(x=
+000028c0: 7061 7273 6564 2e78 2c20 793d 7061 7273  parsed.x, y=pars
+000028d0: 6564 2e79 290a 2020 2020 2020 2020 2020  ed.y).          
+000028e0: 2020 4461 7461 636c 6173 735f 7375 6274    Dataclass_subt
+000028f0: 7261 6374 5f6e 756d 7328 783d 312c 2079  ract_nums(x=1, y
+00002900: 3d32 290a 2020 2020 2020 2020 2020 2020  =2).            
+00002910: 3e3e 3e20 7061 7273 6564 2e5f 636f 6d6d  >>> parsed._comm
+00002920: 616e 645f 6675 6e63 2878 3d70 6172 7365  and_func(x=parse
+00002930: 642e 782c 2079 3d70 6172 7365 642e 7929  d.x, y=parsed.y)
+00002940: 0a20 2020 2020 2020 2020 2020 202d 310a  .            -1.
+00002950: 2020 2020 2020 2020 7247 0000 004e fa01          rG...N..
+00002960: 20a9 0172 9100 0000 7201 0000 0029 0272   ..r....r....).r
+00002970: 4700 0000 7254 0000 0029 0c72 7600 0000  G...rT...).rv...
+00002980: 7224 0000 00da 085f 5f6e 616d 655f 5f72  r$.....__name__r
+00002990: 7000 0000 7278 0000 00da 115f 5375 6250  p...rx....._SubP
+000029a0: 6172 7365 7273 4163 7469 6f6e da03 706f  arsersAction..po
+000029b0: 70da 1f5f 6765 745f 6465 7363 7269 7074  p.._get_descript
+000029c0: 696f 6e5f 6672 6f6d 5f64 6f63 7374 7269  ion_from_docstri
+000029d0: 6e67 da0a 7370 6c69 746c 696e 6573 da0a  ng..splitlines..
+000029e0: 6164 645f 7061 7273 6572 7249 0000 0072  add_parserrI...r
+000029f0: 9200 0000 2909 727a 0000 0072 9100 0000  ....).rz...r....
+00002a00: 7294 0000 0072 5100 0000 5a0a 7375 6270  r....rQ...Z.subp
+00002a10: 6172 7365 7273 7247 0000 005a 0f64 6573  arsersrG...Z.des
+00002a20: 6372 6970 7469 6f6e 5f74 7874 5a08 6865  cription_txtZ.he
+00002a30: 6c70 5f74 7874 725c 0000 0072 5800 0000  lp_txtr\...rX...
+00002a40: 7258 0000 0072 5900 0000 da0b 6164 645f  rX...rY.....add_
+00002a50: 636f 6d6d 616e 6439 0100 0073 3400 0000  command9...s4...
+00002a60: 083e 0402 0a01 1003 0c01 0401 0c01 0404  .>..............
+00002a70: 0201 06ff 0403 0401 0c01 0402 0201 02ff  ................
+00002a80: 0202 0201 04fd 0204 06fc 0406 0601 0402  ................
+00002a90: 0c01 0402 7a1a 4172 6775 6d65 6e74 5061  ....z.ArgumentPa
+00002aa0: 7273 6572 2e61 6464 5f63 6f6d 6d61 6e64  rser.add_command
+00002ab0: da04 6675 6e63 6303 0000 0000 0000 0000  ..funcc.........
+00002ac0: 0000 0005 0000 0005 0000 004b 0000 0073  ...........K...s
+00002ad0: 4200 0000 7400 7c02 7205 7c02 6e02 7c01  B...t.|.r.|.n.|.
+00002ae0: 6a01 8301 7d02 7c00 6a02 7c01 6601 6401  j...}.|.j.|.f.d.
+00002af0: 7c02 6901 7c03 a401 8e01 7d04 7c04 6a03  |.i.|.....}.|.j.
+00002b00: 6402 6900 7c00 6a04 7c01 6901 a401 8e01  d.i.|.j.|.i.....
+00002b10: 0100 6400 5300 2903 4e72 9400 0000 7258  ..d.S.).Nr....rX
+00002b20: 0000 0029 0572 2400 0000 7297 0000 0072  ...).r$...r....r
+00002b30: 9d00 0000 da0c 7365 745f 6465 6661 756c  ......set_defaul
+00002b40: 7473 7245 0000 0029 0572 7a00 0000 729e  tsrE...).rz...r.
+00002b50: 0000 0072 9400 0000 7251 0000 0072 5c00  ...r....rQ...r\.
+00002b60: 0000 7258 0000 0072 5800 0000 7259 0000  ..rX...rX...rY..
+00002b70: 00da 115f 7265 6769 7374 6572 5f63 6f6d  ..._register_com
+00002b80: 6d61 6e64 9901 0000 7312 0000 0012 0604  mand....s.......
+00002b90: 0102 0104 ff02 0202 fe02 0306 fd1a 057a  ...............z
+00002ba0: 2041 7267 756d 656e 7450 6172 7365 722e   ArgumentParser.
+00002bb0: 5f72 6567 6973 7465 725f 636f 6d6d 616e  _register_comman
+00002bc0: 64da 0464 636c 73da 0461 7474 7263 0200  d..dcls..attrc..
+00002bd0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00002be0: 0000 4300 0000 730a 0000 007c 017c 006a  ..C...s....|.|.j
+00002bf0: 0076 0153 0072 5600 0000 a901 da0f 5f5f  .v.S.rV.......__
+00002c00: 616e 6e6f 7461 7469 6f6e 735f 5fa9 0272  annotations__..r
+00002c10: a100 0000 72a2 0000 0072 5800 0000 7258  ....r....rX...rX
+00002c20: 0000 0072 5900 0000 da17 5f69 735f 6174  ...rY....._is_at
+00002c30: 7472 6962 7574 655f 696e 6865 7269 7465  tribute_inherite
+00002c40: 64a7 0100 0073 0200 0000 0a02 7a26 4172  d....s......z&Ar
+00002c50: 6775 6d65 6e74 5061 7273 6572 2e5f 6973  gumentParser._is
+00002c60: 5f61 7474 7269 6275 7465 5f69 6e68 6572  _attribute_inher
+00002c70: 6974 6564 725c 0000 0063 0300 0000 0000  itedr\...c......
+00002c80: 0000 0000 0000 1900 0000 0900 0000 0300  ................
+00002c90: 0000 731c 0700 0074 007c 0283 0172 077c  ..s....t.|...r.|
+00002ca0: 0289 016e 0474 017c 0283 0189 017c 01a0  ...n.t.|.....|..
+00002cb0: 0288 006a 03a1 0172 1864 017d 037c 01a0  ...j...r.d.}.|..
+00002cc0: 047c 03a1 0101 007c 016a 0564 2469 0088  .|.....|.j.d$i..
+00002cd0: 006a 0388 0169 01a4 018e 0101 0069 007d  .j...i.......i.}
+00002ce0: 0474 0674 0787 0087 0166 0264 0264 0384  .t.t.....f.d.d..
+00002cf0: 0874 0888 0183 0183 0283 017d 0564 0464  .t.........}.d.d
+00002d00: 0584 007c 0544 0083 017d 0667 007d 077c  ...|.D...}.g.}.|
+00002d10: 0644 0090 035d 4c5c 027d 087d 097c 086a  .D...]L\.}.}.|.j
+00002d20: 097d 0a74 0a7c 0a74 0b83 0272 4f74 0c7c  .}.t.|.t...rOt.|
+00002d30: 0a83 017d 0a74 0a7c 0a74 0b83 0272 564a  ...}.t.|.t...rVJ
+00002d40: 0082 0174 0d6a 0e64 066b 0572 6074 0a7c  ...t.j.d.k.r`t.|
+00002d50: 0a74 0f83 0273 6788 00a0 107c 0aa1 0174  .t...sg....|...t
+00002d60: 1175 0072 6e88 006a 127c 0a64 0764 088d  .u.rn..j.|.d.d..
+00002d70: 027d 0a74 0a7c 0a74 1383 0272 a988 00a0  .}.t.|.t...r....
+00002d80: 147c 0aa1 0144 005d 137d 0b74 157c 0b74  .|...D.].}.t.|.t
+00002d90: 1683 0272 8b74 177c 0b6a 1876 0072 8b7c  ...r.t.|.j.v.r.|
+00002da0: 0b6a 1874 1719 007d 0901 006e 0171 7888  .j.t...}...n.qx.
+00002db0: 00a0 107c 0aa1 017d 0a74 0d6a 0e64 066b  ...|...}.t.j.d.k
+00002dc0: 0572 9b74 0a7c 0a74 0f83 0273 a288 00a0  .r.t.|.t...s....
+00002dd0: 107c 0aa1 0174 1175 0072 a988 006a 127c  .|...t.u.r...j.|
+00002de0: 0a64 0764 088d 027d 0a74 0a7c 0a74 0983  .d.d...}.t.|.t..
+00002df0: 0272 b17c 0a6a 196e 0a74 0b7c 0a83 016a  .r.|.j.n.t.|...j
+00002e00: 1a64 0964 0a64 0b8d 0264 0c19 007d 0c7c  .d.d.d...d...}.|
+00002e10: 09a0 1b7c 086a 1ca1 0101 007c 096a 1d72  ...|.j.....|.j.r
+00002e20: df7c 086a 1e74 1f75 0172 d27c 086a 1e7c  .|.j.t.u.r.|.j.|
+00002e30: 095f 1e64 0d7c 095f 1d6e 0d7c 086a 2074  ._.d.|._.n.|.j t
+00002e40: 1f75 0172 df7c 08a0 20a1 007c 095f 1e64  .u.r.|.. ..|._.d
+00002e50: 0d7c 095f 1d88 00a0 107c 0aa1 017d 0d7c  .|._.....|...}.|
+00002e60: 0d90 0172 847c 0d90 0172 037c 0d74 2175  ...r.|...r.|.t!u
+00002e70: 0090 0172 0374 0688 00a0 227c 0aa1 0183  ...r.t...."|....
+00002e80: 017c 095f 237c 096a 2390 0172 0274 097c  .|._#|.j#..r.t.|
+00002e90: 096a 2364 0e19 0083 017d 0a6e 8c74 247c  .j#d.....}.n.t$|
+00002ea0: 0d74 256a 266a 2783 0290 0172 1a88 006a  .t%j&j'....r...j
+00002eb0: 127c 0a64 0764 0f8d 027d 0a7c 096a 2890  .|.d.d...}.|.j(.
+00002ec0: 0173 1974 297c 095f 286e 3574 247c 0d74  .s.t)|._(n5t$|.t
+00002ed0: 256a 266a 2a83 0290 0173 277c 0d74 2b75  %j&j*....s'|.t+u
+00002ee0: 0090 0172 4888 006a 127c 0a64 0764 0f8d  ...rH..j.|.d.d..
+00002ef0: 027d 0a7c 096a 2890 0173 477c 0d74 2b75  .}.|.j(..sG|.t+u
+00002f00: 0090 0172 3b74 2c7c 095f 286e 147c 0d74  ...r;t,|._(n.|.t
+00002f10: 2d75 0090 0172 4474 2e7c 095f 286e 0b74  -u...rDt.|._(n.t
+00002f20: 2f7c 095f 286e 0774 3090 0173 4f74 317c  /|._(n.t0..sOt1|
+00002f30: 0a83 0101 0074 247c 0a74 3283 0290 0172  .....t$|.t2....r
+00002f40: 5d64 1064 0584 007c 0a44 0083 017c 095f  ]d.d...|.D...|._
+00002f50: 2374 157c 0188 0083 0290 0172 6c74 3374  #t.|.......rlt3t
+00002f60: 347c 0a83 027c 016a 357c 096a 363c 007c  4|...|.j5|.j6<.|
+00002f70: 096a 3790 0172 817c 096a 3864 0075 0090  .j7..r.|.j8d.u..
+00002f80: 0172 817c 096a 1d90 0172 7e64 117c 095f  .r.|.j...r~d.|._
+00002f90: 386e 0364 127c 095f 3874 0b7d 0a6e 0b74  8n.d.|._8t.}.n.t
+00002fa0: 247c 0a74 3283 0290 0172 8f74 067c 0a83  $|.t2....r.t.|..
+00002fb0: 017c 095f 237c 0a7c 095f 097c 09a0 39a1  .|._#|.|._.|..9.
+00002fc0: 007d 0e7c 0e64 133d 007c 0ea0 3a64 14a1  .}.|.d.=.|..:d..
+00002fd0: 017d 0f7c 0f90 0173 a367 006e 0664 1564  .}.|...s.g.n.d.d
+00002fe0: 0584 007c 0f44 0083 017d 107c 0e64 1619  ...|.D...}.|.d..
+00002ff0: 0090 0173 c67c 0ea0 3b64 17a1 0190 0173  ...s.|..;d.....s
+00003000: c67c 1090 0173 c264 187c 0e64 1919 00a0  .|...s.d.|.d....
+00003010: 3ca1 009b 0064 1a9d 036e 0164 1b7c 0e64  <....d...n.d.|.d
+00003020: 163c 007c 0e64 1c19 007d 117c 1090 0173  .<.|.d...}.|...s
+00003030: e77c 0e64 1c3d 007c 1190 0173 df7c 0ea0  .|.d.=.|...s.|..
+00003040: 3b64 1da1 0164 0075 0090 0172 df64 1e7c  ;d...d.u...r.d.|
+00003050: 0e64 1d3c 0074 3374 347c 0a83 027c 0e64  .d.<.t3t4|...|.d
+00003060: 1f3c 006e 4c7c 096a 0974 3d75 0090 0272  .<.nL|.j.t=u...r
+00003070: 1274 157c 0188 0083 0290 0172 fc74 3374  .t.|.......r.t3t
+00003080: 347c 0a83 027c 016a 357c 096a 363c 0064  4|...|.j5|.j6<.d
+00003090: 2044 005d 097d 127c 0ea0 3a7c 1264 00a1   D.].}.|..:|.d..
+000030a0: 0201 0090 0171 fe7c 0e64 2119 0090 0273  .....q.|.d!....s
+000030b0: 1174 3e7c 0e64 213c 006e 217c 096a 3864  .t>|.d!<.n!|.j8d
+000030c0: 0e6b 0390 0272 2074 3374 347c 0a83 027c  .k...r t3t4|...|
+000030d0: 0e64 1f3c 006e 137c 0a74 3f75 0090 0272  .d.<.n.|.t?u...r
+000030e0: 2a74 407c 0e64 213c 006e 097c 0a74 0b75  *t@|.d!<.n.|.t.u
+000030f0: 0090 0272 3374 417c 0e64 213c 007c 086a  ...r3tA|.d!<.|.j
+00003100: 1e74 1f75 0190 0273 477c 086a 2074 1f75  .t.u...sG|.j t.u
+00003110: 0190 0273 477c 0ea0 3b64 22a1 0164 0075  ...sG|..;d"..d.u
+00003120: 0190 0272 de7c 0ea0 3b64 21a1 0190 0272  ...r.|..;d!....r
+00003130: 7a74 247c 0e64 2119 0074 426a 4374 3e66  zt$|.d!..tBjCt>f
+00003140: 0283 0290 0272 7a74 0964 2364 2469 0083  .....rzt.d#d$i..
+00003150: 0383 007d 137c 0e64 2119 007c 107c 0e64  ...}.|.d!..|.|.d
+00003160: 1919 0064 258d 027c 017c 137c 0e64 2219  ...d%..|.|.|.d".
+00003170: 0064 268d 0301 0074 447c 137c 0e64 1919  .d&....tD|.|.d..
+00003180: 0083 027c 0e64 223c 006e 0f64 1f7c 0e76  ...|.d"<.n.d.|.v
+00003190: 0090 0272 897c 0e64 1f19 007c 0e64 2219  ...r.|.d...|.d".
+000031a0: 0083 017c 0e64 223c 007c 0ea0 3b64 17a1  ...|.d"<.|..;d..
+000031b0: 0190 0272 de7c 0e64 2219 007d 1474 0a7c  ...r.|.d"..}.t.|
+000031c0: 1474 0b83 0290 0273 a174 0a7c 1474 256a  .t.....s.t.|.t%j
+000031d0: 266a 2a83 0290 0273 a47c 1467 017d 147c  &j*....s.|.g.}.|
+000031e0: 1444 005d 377d 0b7c 0b7c 0e64 1719 0076  .D.]7}.|.|.d...v
+000031f0: 0190 0272 dc74 0a7c 0b74 3283 0290 0272  ...r.t.|.t2....r
+00003200: bd7c 0b6a 1c7c 0e64 1719 0076 0190 0272  .|.j.|.d...v...r
+00003210: dc7c 0ea0 3b64 1ca1 0190 0273 c87c 0b64  .|..;d.....s.|.d
+00003220: 0075 0090 0273 dc64 277c 0b9b 0064 287c  .u...s.d'|...d(|
+00003230: 0e64 1919 009b 0064 297c 0e64 1719 009b  .d.....d)|.d....
+00003240: 009d 067d 037c 01a0 047c 03a1 0101 0090  ...}.|...|......
+00003250: 0271 a664 2a7c 0c9b 009d 0267 017d 157c  .q.d*|.....g.}.|
+00003260: 1190 0273 fb74 157c 0ea0 3b64 22a1 0174  ...s.t.|..;d"..t
+00003270: 0b83 0290 0272 f67c 15a0 4564 2ba1 0101  .....r.|..Ed+...
+00003280: 006e 057c 15a0 4564 2ca1 0101 007c 0ea0  .n.|..Ed,....|..
+00003290: 3a64 2d64 0da1 0290 0372 077c 15a0 4564  :d-d.....r.|..Ed
+000032a0: 2ea1 0101 007c 096a 4690 0372 147c 15a0  .....|.jF..r.|..
+000032b0: 4564 2f7c 096a 469b 009d 02a1 0101 0064  Ed/|.jF........d
+000032c0: 3064 31a0 477c 15a1 019b 009d 027d 167c  0d1.G|.......}.|
+000032d0: 0ea0 3b64 32a1 0190 0372 2d7c 0e64 3205  ..;d2....r-|.d2.
+000032e0: 0019 0064 337c 1617 0037 0003 003c 006e  ...d3|...7...<.n
+000032f0: 047c 167c 0e64 323c 007c 0ea0 3a64 3464  .|.|.d2<.|..:d4d
+00003300: 00a1 027d 177c 1790 0373 417c 1190 0372  ...}.|...sA|...r
+00003310: 3f64 356e 0164 367d 177c 04a0 3b7c 1764  ?d5n.d6}.|..;|.d
+00003320: 00a1 027d 187c 1890 0373 537c 01a0 487c  ...}.|...sS|..H|
+00003330: 17a1 017d 187c 187c 047c 173c 007c 096a  ...}.|.|.|.<.|.j
+00003340: 4990 0372 7e7c 1190 0372 6564 377c 096a  I..r~|...red7|.j
+00003350: 369b 009d 027d 037c 01a0 047c 03a1 0101  6....}.|...|....
+00003360: 007c 016a 4a7c 016a 4ba0 3b88 006a 4ca1  .|.jJ|.jK.;..jL.
+00003370: 0119 007c 1719 00a0 457c 096a 367c 1090  ...|....E|.j6|..
+00003380: 0372 7a7c 1064 0c19 006e 0164 0066 02a1  .rz|.d...n.d.f..
+00003390: 0101 007c 186a 4d7c 1069 007c 0ea4 018e  ...|.jM|.i.|....
+000033a0: 0101 007c 07a0 457c 09a1 0101 0071 3e7c  ...|..E|.....q>|
+000033b0: 0753 0029 384e 7a3e 5468 6973 2070 6172  .S.)8Nz>This par
+000033c0: 7365 7220 616c 7265 6164 7920 636f 6e74  ser already cont
+000033d0: 6169 6e73 2061 7267 756d 656e 7473 2066  ains arguments f
+000033e0: 726f 6d20 616e 6f74 6865 7220 6461 7461  rom another data
+000033f0: 636c 6173 732e 6301 0000 0000 0000 0000  class.c.........
+00003400: 0000 0001 0000 0004 0000 0013 0000 0073  ...............s
+00003410: 1200 0000 8800 6a00 8801 7c00 6a01 6401  ......j...|.j.d.
+00003420: 8d02 0c00 5300 2902 4e72 a500 0000 2902  ....S.).Nr....).
+00003430: 72a6 0000 0072 9400 0000 2901 da01 66a9  r....r....)...f.
+00003440: 02da 0363 6c73 5a05 6d6f 6465 6c72 5800  ...clsZ.modelrX.
+00003450: 0000 7259 0000 0072 5a00 0000 c401 0000  ..rY...rZ.......
+00003460: f302 0000 0012 007a 2f41 7267 756d 656e  .......z/Argumen
+00003470: 7450 6172 7365 722e 5f61 6464 5f61 7267  tParser._add_arg
+00003480: 756d 656e 7473 2e3c 6c6f 6361 6c73 3e2e  uments.<locals>.
+00003490: 3c6c 616d 6264 613e 6301 0000 0000 0000  <lambda>c.......
+000034a0: 0000 0000 0002 0000 0007 0000 0053 0000  .............S..
+000034b0: 0073 2000 0000 6700 7c00 5d0c 7d01 7c01  .s ...g.|.].}.|.
+000034c0: 7c01 6a00 a001 7402 7403 8300 a102 6602  |.j...t.t.....f.
+000034d0: 9102 7102 5300 7258 0000 0029 04da 086d  ..q.S.rX...)...m
+000034e0: 6574 6164 6174 61da 0367 6574 7221 0000  etadata..getr!..
+000034f0: 0072 2200 0000 7261 0000 0072 5800 0000  .r"...ra...rX...
+00003500: 7258 0000 0072 5900 0000 7264 0000 00c9  rX...rY...rd....
+00003510: 0100 0073 0800 0000 0600 0202 12ff 06ff  ...s............
+00003520: 7a31 4172 6775 6d65 6e74 5061 7273 6572  z1ArgumentParser
+00003530: 2e5f 6164 645f 6172 6775 6d65 6e74 732e  ._add_arguments.
+00003540: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00003550: 6d70 3e72 3d00 0000 5429 01da 0d69 735f  mp>r=...T)...is_
+00003560: 756e 696f 6e5f 7479 7065 da01 2e72 1700  union_type...r..
+00003570: 0000 a901 da08 6d61 7873 706c 6974 e9ff  ......maxsplit..
+00003580: ffff ff46 7201 0000 0029 01da 1061 7373  ...Fr....)...ass
+00003590: 6572 745f 7072 696d 6974 6976 6563 0100  ert_primitivec..
+000035a0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+000035b0: 0000 5300 0000 7312 0000 0067 007c 005d  ..S...s....g.|.]
+000035c0: 057d 017c 016a 0091 0271 0253 0072 5800  .}.|.j...q.S.rX.
+000035d0: 0000 a901 7294 0000 0072 6100 0000 7258  ....r....ra...rX
+000035e0: 0000 0072 5800 0000 7259 0000 0072 6400  ...rX...rY...rd.
+000035f0: 0000 2502 0000 72aa 0000 00fa 012b da01  ..%...r......+..
+00003600: 2ada 0370 6f73 7265 0000 0063 0100 0000  *..posre...c....
+00003610: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+00003620: 5300 0000 731a 0000 0067 007c 005d 097d  S...s....g.|.].}
+00003630: 017c 01a0 0064 00a1 0172 027c 0191 0271  .|...d...r.|...q
+00003640: 0253 0029 0172 5b00 0000 7266 0000 0072  .S.).r[...rf...r
+00003650: 6100 0000 7258 0000 0072 5800 0000 7259  a...rX...rX...rY
+00003660: 0000 0072 6400 0000 4502 0000 f302 0000  ...rd...E.......
+00003670: 001a 00da 076d 6574 6176 6172 726a 0000  .....metavarrj..
+00003680: 00fa 013c da04 6465 7374 fa01 3e7a 073c  ...<..dest..>z.<
+00003690: 7661 6c75 653e da08 7265 7175 6972 6564  value>..required
+000036a0: da05 6e61 7267 73fa 013f da04 7479 7065  ..nargs..?..type
+000036b0: 2905 72bf 0000 0072 bd00 0000 da05 636f  ).r....r......co
+000036c0: 6e73 7472 6a00 0000 72b8 0000 0072 5300  nstrj...r....rS.
+000036d0: 0000 7269 0000 00da 0072 5800 0000 2902  ..ri.....rX...).
+000036e0: 7265 0000 0072 ba00 0000 2903 725c 0000  re...r....).r\..
+000036f0: 00da 096e 616d 6573 7061 6365 da06 7661  ...namespace..va
+00003700: 6c75 6573 7a0f 496e 7661 6c69 6420 7661  luesz.Invalid va
+00003710: 6c75 6520 277a 1027 2066 6f72 2061 7267  lue 'z.' for arg
+00003720: 756d 656e 7420 277a 1327 3b20 6d75 7374  ument 'z.'; must
+00003730: 2062 6520 6f6e 6520 6f66 3a20 7a06 5479   be one of: z.Ty
+00003740: 7065 3a20 7a16 4465 6661 756c 743a 2022  pe: z.Default: "
+00003750: 2528 6465 6661 756c 7429 7322 7a14 4465  %(default)s"z.De
+00003760: 6661 756c 743a 2025 2864 6566 6175 6c74  fault: %(default
+00003770: 2973 da09 6578 636c 7573 6976 657a 044d  )s..exclusivez.M
+00003780: 2e58 2e7a 0545 6e76 3a20 7a02 3e20 fa02  .X.z.Env: z.> ..
+00003790: 2c20 7254 0000 0072 7f00 0000 da05 6772  , rT...r......gr
+000037a0: 6f75 707a 1372 6571 7569 7265 6420 7061  oupz.required pa
+000037b0: 7261 6d65 7465 7273 7a13 6f70 7469 6f6e  rametersz.option
+000037c0: 616c 2070 6172 616d 6574 6572 737a 3341  al parametersz3A
+000037d0: 206d 7574 7561 6c6c 792d 6578 636c 7573   mutually-exclus
+000037e0: 6976 6520 7061 7261 6d65 7465 7220 6361  ive parameter ca
+000037f0: 6e6e 6f74 2062 6520 7265 7175 6972 6564  nnot be required
+00003800: 3a20 294e 7234 0000 0072 2500 0000 da0b  : )Nr4...r%.....
+00003810: 6765 745f 6465 6661 756c 7472 4600 0000  get_defaultrF...
+00003820: 7284 0000 0072 9f00 0000 7257 0000 00da  r....r....rW....
+00003830: 0666 696c 7465 7272 0600 0000 72bf 0000  .filterr....r...
+00003840: 0072 3800 0000 7271 0000 0072 2300 0000  .r8...rq...r#...
+00003850: 7281 0000 00da 0c76 6572 7369 6f6e 5f69  r......version_i
+00003860: 6e66 6f72 3f00 0000 da10 5f67 6574 5f74  nfor?....._get_t
+00003870: 7970 655f 6f72 6967 696e 7215 0000 00da  ype_originr.....
+00003880: 1c5f 6578 7472 6163 745f 7479 7065 5f66  ._extract_type_f
+00003890: 726f 6d5f 636f 6e74 6169 6e65 7272 3c00  rom_containerr<.
+000038a0: 0000 da12 5f67 6574 5f74 7970 655f 6d65  ...._get_type_me
+000038b0: 7461 6461 7461 7270 0000 0072 0500 0000  tadatarp...r....
+000038c0: 7221 0000 0072 ab00 0000 7297 0000 00da  r!...r....r.....
+000038d0: 0672 7370 6c69 74da 0873 6574 5f64 6573  .rsplit..set_des
+000038e0: 7472 9400 0000 72bc 0000 0072 6900 0000  tr....r....ri...
+000038f0: 7204 0000 00da 0f64 6566 6175 6c74 5f66  r......default_f
+00003900: 6163 746f 7279 722a 0000 00da 0e5f 6765  actoryr*....._ge
+00003910: 745f 7479 7065 5f61 7267 7372 6a00 0000  t_type_argsrj...
+00003920: 7239 0000 00da 0b63 6f6c 6c65 6374 696f  r9.....collectio
+00003930: 6e73 da03 6162 63da 074d 6170 7069 6e67  ns..abc..Mapping
+00003940: 7253 0000 0072 1d00 0000 da08 4974 6572  rS...r......Iter
+00003950: 6162 6c65 da03 7365 7472 1f00 0000 da05  able..setr......
+00003960: 7475 706c 6572 2000 0000 721e 0000 0072  tupler ...r....r
+00003970: 3500 0000 7227 0000 0072 0700 0000 7208  5...r'...r....r.
+00003980: 0000 0072 3100 0000 7275 0000 0072 ba00  ...r1...ru...r..
+00003990: 0000 72b6 0000 0072 bd00 0000 da06 6173  ..r....r......as
+000039a0: 6469 6374 7299 0000 0072 ac00 0000 da05  dictr....r......
+000039b0: 7570 7065 72da 0462 6f6f 6c72 1800 0000  upper..boolr....
+000039c0: da03 696e 7472 1900 0000 721a 0000 0072  ..intr....r....r
+000039d0: 7800 0000 da06 4163 7469 6f6e da07 6765  x.....Action..ge
+000039e0: 7461 7474 72da 0661 7070 656e 64da 085f  tattr..append.._
+000039f0: 656e 765f 7661 72da 046a 6f69 6eda 1261  env_var..join..a
+00003a00: 6464 5f61 7267 756d 656e 745f 6772 6f75  dd_argument_grou
+00003a10: 7072 c400 0000 7274 0000 00da 095f 6465  pr....rt....._de
+00003a20: 6661 756c 7473 7245 0000 0072 7200 0000  faultsrE...rr...
+00003a30: 2919 72a9 0000 0072 5c00 0000 7291 0000  ).r....r\...r...
+00003a40: 00da 0365 7272 5a11 7061 7273 6572 5f61  ...errZ.parser_a
+00003a50: 7267 5f67 726f 7570 735a 0c6e 6f76 656c  rg_groupsZ.novel
+00003a60: 5f66 6965 6c64 735a 106e 6f76 656c 5f66  _fieldsZ.novel_f
+00003a70: 6965 6c64 5f61 7267 735a 0a61 6464 6564  ield_argsZ.added
+00003a80: 5f61 7267 735a 0366 6c64 5a11 6172 6770  _argsZ.fldZ.argp
+00003a90: 6172 7365 5f61 7267 756d 656e 74da 0866  arse_argument..f
+00003aa0: 6c64 5f74 7970 6572 6300 0000 5a09 6865  ld_typerc...Z.he
+00003ab0: 6c70 5f74 7970 655a 0f66 6c64 5f74 7970  lp_typeZ.fld_typ
+00003ac0: 655f 6f72 6967 696e 7251 0000 0072 6500  e_originrQ...re.
+00003ad0: 0000 7250 0000 0072 bc00 0000 da01 6b5a  ..rP...r......kZ
+00003ae0: 0f64 756d 6d79 5f6e 616d 6573 7061 6365  .dummy_namespace
+00003af0: da01 645a 0e68 656c 705f 6d73 675f 7061  ..dZ.help_msg_pa
+00003b00: 7274 735a 0868 656c 705f 6d73 6772 c600  rtsZ.help_msgr..
+00003b10: 0000 5a09 6172 675f 6772 6f75 7072 5800  ..Z.arg_grouprX.
+00003b20: 0000 72a8 0000 0072 5900 0000 7292 0000  ..r....rY...r...
+00003b30: 00ab 0100 0073 a401 0000 080a 0601 0802  .....s..........
+00003b40: 0c02 0401 0a01 1602 0402 0202 0201 0c01  ................
+00003b50: 0601 02fe 04ff 0607 0202 06fe 0405 0e02  ................
+00003b60: 0601 0a04 0801 0e01 1403 0e01 0401 0201  ................
+00003b70: 0201 06fe 0a05 0e01 1401 0a01 0401 0280  ................
+00003b80: 0a02 1403 0e01 0401 0201 0201 06fe 0807  ................
+00003b90: 08ff 1402 02fd 0c06 0602 0a01 0801 0801  ................
+00003ba0: 0a01 0a01 0601 0a02 0601 1001 1001 0801  ................
+00003bb0: 0e01 0280 1003 0401 0201 0201 06fe 0804  ................
+00003bc0: 0601 0280 0c03 04ff 0a02 0402 0201 0201  ................
+00003bd0: 06fe 0804 0a01 0801 0a01 0801 0602 0280  ................
+00003be0: 0602 0801 0c02 1001 0c02 0203 0201 0201  ................
+00003bf0: 0cfe 1405 0801 0801 0602 0604 0c02 0a01  ................
+00003c00: 0602 0802 0601 0a02 0203 08ff 0c02 02fd  ................
+00003c10: 1606 1c02 06ff 0804 0602 0602 1601 0801  ................
+00003c20: 1001 0c01 0c01 0203 0201 0201 0cfe 0805  ................
+00003c30: 1001 0a01 0801 0280 0c02 1001 0a01 0a02  ................
+00003c40: 0a01 0802 0c04 0c01 1001 0e02 0601 0801  ................
+00003c50: 06fe 0e05 1201 0201 0201 0601 06fd 1405  ................
+00003c60: 0a01 1401 0c03 0801 0e01 0201 0601 06fe  ................
+00003c70: 0604 0802 0e02 0802 04fe 1003 0803 04fd  ................
+00003c80: 0a03 1203 0601 04ff 02ff 0a04 0480 0c02  ................
+00003c90: 0603 1201 0c01 0a02 0e02 0a01 0802 1201  ................
+00003ca0: 1002 0c02 1601 0802 0c02 0602 0e01 0c02  ................
+00003cb0: 0602 0a01 0801 0802 0601 0202 0401 04ff  ................
+00003cc0: 02ff 0a04 0402 0c01 02ff 0202 02fe 0202  ................
+00003cd0: 0402 1001 02fe 04ff 1007 0c02 0402 7a1d  ..............z.
+00003ce0: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
+00003cf0: 6164 645f 6172 6775 6d65 6e74 73da 0174  add_arguments..t
+00003d00: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00003d10: 0004 0000 0043 0000 0073 0c00 0000 7400  .....C...s....t.
+00003d20: 7c00 6401 6400 8303 5300 2902 4eda 0a5f  |.d.d...S.).N.._
+00003d30: 5f6f 7269 6769 6e5f 5fa9 0172 dc00 0000  _origin__..r....
+00003d40: a901 72e6 0000 0072 5800 0000 7258 0000  ..r....rX...rX..
+00003d50: 0072 5900 0000 72ca 0000 00d2 0200 00f3  .rY...r.........
+00003d60: 0200 0000 0c02 7a1f 4172 6775 6d65 6e74  ......z.Argument
+00003d70: 5061 7273 6572 2e5f 6765 745f 7479 7065  Parser._get_type
+00003d80: 5f6f 7269 6769 6e63 0100 0000 0000 0000  _originc........
+00003d90: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
+00003da0: f30c 0000 0074 007c 0064 0164 0283 0353  .....t.|.d.d...S
+00003db0: 0029 034e da08 5f5f 6172 6773 5f5f 7258  .).N..__args__rX
+00003dc0: 0000 0072 e800 0000 72e9 0000 0072 5800  ...r....r....rX.
+00003dd0: 0000 7258 0000 0072 5900 0000 72d0 0000  ..rX...rY...r...
+00003de0: 00d6 0200 0072 ea00 0000 7a1d 4172 6775  .....r....z.Argu
+00003df0: 6d65 6e74 5061 7273 6572 2e5f 6765 745f  mentParser._get_
+00003e00: 7479 7065 5f61 7267 7363 0100 0000 0000  type_argsc......
+00003e10: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+00003e20: 0000 72eb 0000 0029 034e da0c 5f5f 6d65  ..r....).N..__me
+00003e30: 7461 6461 7461 5f5f 7258 0000 0072 e800  tadata__rX...r..
+00003e40: 0000 72e9 0000 0072 5800 0000 7258 0000  ..r....rX...rX..
+00003e50: 0072 5900 0000 72cc 0000 00da 0200 0072  .rY...r........r
+00003e60: ea00 0000 7a21 4172 6775 6d65 6e74 5061  ....z!ArgumentPa
+00003e70: 7273 6572 2e5f 6765 745f 7479 7065 5f6d  rser._get_type_m
+00003e80: 6574 6164 6174 61da 0e74 7970 655f 636f  etadata..type_co
+00003e90: 6e74 6169 6e65 7272 b200 0000 72ad 0000  ntainerr....r...
+00003ea0: 0063 0400 0000 0000 0000 0000 0000 0b00  .c..............
+00003eb0: 0000 0300 0000 4300 0000 7318 0100 007c  ......C...s....|
+00003ec0: 0372 0474 006e 047c 00a0 017c 01a1 017d  .r.t.n.|...|...}
+00003ed0: 047c 0464 0075 0072 1574 0264 017c 016a  .|.d.u.r.t.d.|.j
+00003ee0: 039b 009d 0283 0182 017c 00a0 047c 01a1  .........|...|..
+00003ef0: 017d 0564 0264 0384 007c 0544 0083 017d  .}.d.d...|.D...}
+00003f00: 067c 0474 0075 0073 3074 057c 0474 066a  .|.t.u.s0t.|.t.j
+00003f10: 076a 0883 0273 307c 0474 0975 0072 4074  .j...s0|.t.u.r@t
+00003f20: 0a7c 0683 0164 046b 0372 3b7c 06a0 0ba1  .|...d.k.r;|....
+00003f30: 0001 006e 2c7c 0664 0519 007d 076e 2774  ...n,|.d...}.n't
+00003f40: 057c 0474 066a 076a 0c83 0272 6174 0a7c  .|.t.j.j...rat.|
+00003f50: 0683 0164 066b 0372 527c 06a0 0ba1 0001  ...d.k.rR|......
+00003f60: 006e 157c 065c 027d 087d 097c 0874 0d75  .n.|.\.}.}.|.t.u
+00003f70: 0172 5e74 0264 0783 0182 017c 097d 076e  .r^t.d.....|.}.n
+00003f80: 0674 0e73 6774 0f7c 0183 0101 007c 0673  .t.sgt.|.....|.s
+00003f90: 6d74 0264 0883 0182 017c 00a0 017c 07a1  mt.d.....|...|..
+00003fa0: 017d 0a7c 0a74 0075 0072 807c 00a0 107c  .}.|.t.u.r.|...|
+00003fb0: 07a1 017d 077c 00a0 017c 07a1 017d 0a7c  ...}.|...|...}.|
+00003fc0: 0272 8a7c 0a72 8a74 0e73 8a74 0f7c 0a83  .r.|.r.t.s.t.|..
+00003fd0: 0101 007c 0753 0029 094e 7a1f 4769 7665  ...|.S.).Nz.Give
+00003fe0: 6e20 7479 7065 2069 7320 6e6f 7420 6120  n type is not a 
+00003ff0: 636f 6e74 6169 6e65 723a 2063 0100 0000  container: c....
+00004000: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00004010: 5300 0000 7320 0000 0067 007c 005d 0c7d  S...s ...g.|.].}
+00004020: 017c 0164 0075 0172 027c 0174 0075 0172  .|.d.u.r.|.t.u.r
+00004030: 027c 0191 0271 0253 0029 012e 2901 722b  .|...q.S.)..).r+
+00004040: 0000 0029 0272 6200 0000 da01 6172 5800  ...).rb.....arX.
+00004050: 0000 7258 0000 0072 5900 0000 7264 0000  ..rX...rY...rd..
+00004060: 00f0 0200 0073 0400 0000 0600 1a01 7a3f  .....s........z?
+00004070: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
+00004080: 6578 7472 6163 745f 7479 7065 5f66 726f  extract_type_fro
+00004090: 6d5f 636f 6e74 6169 6e65 722e 3c6c 6f63  m_container.<loc
+000040a0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
+000040b0: 1700 0000 7201 0000 0072 7e00 0000 7a22  ....r....r~...z"
+000040c0: 4469 6374 696f 6e61 7279 206b 6579 7320  Dictionary keys 
+000040d0: 6d75 7374 2062 6520 7479 7065 2060 7374  must be type `st
+000040e0: 7260 7a1b 546f 6f20 6d61 6e79 2074 7970  r`z.Too many typ
+000040f0: 6573 2069 6e20 636f 6e74 6169 6e65 7229  es in container)
+00004100: 1172 1500 0000 72ca 0000 00da 0954 7970  .r....r......Typ
+00004110: 6545 7272 6f72 7297 0000 0072 d000 0000  eErrorr....r....
+00004120: 7239 0000 0072 d100 0000 72d2 0000 0072  r9...r....r....r
+00004130: 1100 0000 72d5 0000 0072 6000 0000 da05  ....r....r`.....
+00004140: 636c 6561 7272 d300 0000 7271 0000 0072  clearr....rq...r
+00004150: 3500 0000 7227 0000 0072 cb00 0000 290b  5...r'...r....).
+00004160: 72a9 0000 0072 ee00 0000 72b2 0000 0072  r....r....r....r
+00004170: ad00 0000 5a15 7479 7065 5f63 6f6e 7461  ....Z.type_conta
+00004180: 696e 6572 5f6f 7269 6769 6e5a 1374 7970  iner_originZ.typ
+00004190: 655f 636f 6e74 6169 6e65 725f 6172 6773  e_container_args
+000041a0: da07 7265 7375 6c74 735a 1674 7970 655f  ..resultsZ.type_
+000041b0: 636f 6e74 6169 6e65 725f 7375 6274 7970  container_subtyp
+000041c0: 655a 086b 6579 5f74 7970 655a 0a76 616c  eZ.key_typeZ.val
+000041d0: 7565 5f74 7970 655a 1d74 7970 655f 636f  ue_typeZ.type_co
+000041e0: 6e74 6169 6e65 725f 7375 6274 7970 655f  ntainer_subtype_
+000041f0: 6f72 6967 696e 7258 0000 0072 5800 0000  originrX...rX...
+00004200: 7259 0000 0072 cb00 0000 de02 0000 7354  rY...r........sT
+00004210: 0000 0010 0802 ff08 0402 010a 0104 ff0a  ................
+00004220: 0406 0202 0106 ff08 070c 0102 ff08 020c  ................
+00004230: 020a 010a 020e 010c 010a 0108 0208 0108  ................
+00004240: 0106 0104 0108 0104 0208 010a 0208 0204  ................
+00004250: 0102 0104 ff0a 0302 0302 ff02 0202 fe02  ................
+00004260: 0302 fd08 0504 027a 2b41 7267 756d 656e  .......z+Argumen
+00004270: 7450 6172 7365 722e 5f65 7874 7261 6374  tParser._extract
+00004280: 5f74 7970 655f 6672 6f6d 5f63 6f6e 7461  _type_from_conta
+00004290: 696e 6572 6301 0000 0000 0000 0000 0000  inerc...........
+000042a0: 0005 0000 0006 0000 000b 0000 0073 6200  .............sb.
+000042b0: 0000 6401 6402 8800 6a00 6403 9c03 7d02  ..d.d...j.d...}.
+000042c0: 7c02 a001 a100 4400 5d0c 5c02 7d03 7d04  |.....D.].\.}.}.
+000042d0: 7c01 a002 7c03 7c04 a102 7c01 7c03 3c00  |...|.|...|.|.<.
+000042e0: 710b 7c01 a002 6404 8700 6601 6405 6406  q.|...d...f.d.d.
+000042f0: 8408 a102 7c01 6404 3c00 7403 8300 6a04  ....|.d.<.t...j.
+00004300: 6407 6900 7c01 a401 8e01 8800 5f05 8800  d.i.|......._...
+00004310: 6a05 5300 2908 4e5a 0863 6f6d 6d61 6e64  j.S.).NZ.command
+00004320: 737a 093c 434f 4d4d 414e 443e 2903 726f  sz.<COMMAND>).ro
+00004330: 0000 0072 b800 0000 72ba 0000 00da 0c70  ...r....r......p
+00004340: 6172 7365 725f 636c 6173 7363 0000 0000  arser_classc....
+00004350: 0000 0000 0000 0000 0100 0000 0500 0000  ................
+00004360: 1b00 0000 731a 0000 0074 0088 0083 0164  ....s....t.....d
+00004370: 0269 007c 00a4 0164 0188 0069 01a4 018e  .i.|...d...i....
+00004380: 0153 0029 034e 724f 0000 0072 5800 0000  .S.).NrO...rX...
+00004390: 2901 72bf 0000 0029 0172 e400 0000 a901  ).r....).r......
+000043a0: 727a 0000 0072 5800 0000 7259 0000 0072  rz...rX...rY...r
+000043b0: 5a00 0000 2903 0000 72b7 0000 007a 2f41  Z...)...r....z/A
+000043c0: 7267 756d 656e 7450 6172 7365 722e 6164  rgumentParser.ad
+000043d0: 645f 7375 6270 6172 7365 7273 2e3c 6c6f  d_subparsers.<lo
+000043e0: 6361 6c73 3e2e 3c6c 616d 6264 613e 7258  cals>.<lambda>rX
+000043f0: 0000 0029 0672 4400 0000 728f 0000 0072  ...).rD...r....r
+00004400: ac00 0000 726b 0000 00da 0e61 6464 5f73  ....rk.....add_s
+00004410: 7562 7061 7273 6572 7372 6d00 0000 2905  ubparsersrm...).
+00004420: 727a 0000 0072 5100 0000 5a0e 6465 6661  rz...rQ...Z.defa
+00004430: 756c 745f 6b77 6172 6773 72e4 0000 00da  ult_kwargsr.....
+00004440: 0176 727b 0000 0072 f400 0000 7259 0000  .vr{...r....rY..
+00004450: 0072 f500 0000 1e03 0000 7318 0000 0002  .r........s.....
+00004460: 0202 0104 0106 fd10 0512 0104 0202 010a  ................
+00004470: 0108 fe14 0506 027a 1d41 7267 756d 656e  .......z.Argumen
+00004480: 7450 6172 7365 722e 6164 645f 7375 6270  tParser.add_subp
+00004490: 6172 7365 7273 6301 0000 0000 0000 0000  arsersc.........
+000044a0: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+000044b0: 2c00 0000 7c00 6a00 4400 5d10 7d01 7401  ,...|.j.D.].}.t.
+000044c0: 7c01 7402 6a03 8302 7213 7c01 7c00 5f04  |.t.j...r.|.|._.
+000044d0: 7c00 6a04 0200 0100 5300 7103 6400 5300  |.j.....S.q.d.S.
+000044e0: 7256 0000 0029 05da 085f 6163 7469 6f6e  rV...)..._action
+000044f0: 7372 7000 0000 7278 0000 0072 9800 0000  srp...rx...r....
+00004500: 726d 0000 0029 0272 7a00 0000 72ef 0000  rm...).rz...r...
+00004510: 0072 5800 0000 7258 0000 0072 5900 0000  .rX...rX...rY...
+00004520: 728e 0000 0030 0300 0073 1200 0000 0a01  r....0...s......
+00004530: 0201 0201 0401 04fe 0604 0a01 02fb 0406  ................
+00004540: 7a26 4172 6775 6d65 6e74 5061 7273 6572  z&ArgumentParser
+00004550: 2e5f 6669 6e64 5f73 7562 7061 7273 6572  ._find_subparser
+00004560: 735f 6163 7469 6f6e 6301 0000 0000 0000  s_actionc.......
+00004570: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
+00004580: 0073 3600 0000 7c00 6a00 6400 7501 7208  .s6...|.j.d.u.r.
+00004590: 7c00 6a00 5300 7c00 6a01 7217 7c00 a002  |.j.S.|.j.r.|...
+000045a0: a100 0100 7c00 6a00 7314 4a00 8201 7c00  ....|.j.s.J...|.
+000045b0: 6a00 5300 7c00 a003 a100 5300 7256 0000  j.S.|.....S.rV..
+000045c0: 0029 0472 6d00 0000 728d 0000 0072 8e00  .).rm...r....r..
+000045d0: 0000 72f5 0000 0072 f400 0000 7258 0000  ..r....r....rX..
+000045e0: 0072 5800 0000 7259 0000 0072 7600 0000  .rX...rY...rv...
+000045f0: 3a03 0000 730e 0000 000a 0106 0106 0208  :...s...........
+00004600: 010a 0106 0108 027a 2541 7267 756d 656e  .......z%Argumen
+00004610: 7450 6172 7365 722e 5f67 6574 5f6f 725f  tParser._get_or_
+00004620: 6164 645f 7375 6270 6172 7365 7273 72c2  add_subparsersr.
+00004630: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00004640: 0600 0000 0600 0000 0300 0000 736e 0000  ............sn..
+00004650: 007c 006a 00a0 0174 0288 007c 006a 0364  .|.j...t...|.j.d
+00004660: 0083 0369 00a1 027d 027c 02a0 04a1 0044  ...i...}.|.....D
+00004670: 005d 1d7d 0387 0066 0164 0164 0284 087c  .].}...f.d.d...|
+00004680: 0344 0083 017d 0474 057c 0483 0164 036b  .D...}.t.|...d.k
+00004690: 0472 2d64 0464 05a0 067c 04a1 0117 007d  .r-d.d...|.....}
+000046a0: 057c 00a0 077c 05a1 0101 0071 1074 0864  .|...|.....q.t.d
+000046b0: 0669 0074 0988 0083 01a4 018e 0153 0029  .i.t.........S.)
+000046c0: 074e 6301 0000 0000 0000 0000 0000 0004  .Nc.............
+000046d0: 0000 0005 0000 0013 0000 0073 6c00 0000  ...........sl...
+000046e0: 6700 7c00 5d32 5c02 7d01 7d02 7400 8800  g.|.]2\.}.}.t...
+000046f0: 7c01 8302 7234 7401 8800 7c01 8302 7d03  |...r4t...|...}.
+00004700: 7402 7c03 7403 8302 731c 7402 7c03 7404  t.|.t...s.t.|.t.
+00004710: 6a05 6a06 8302 7320 7c03 6400 7501 732e  j.j...s |.d.u.s.
+00004720: 7402 7c03 7403 8302 7302 7402 7c03 7404  t.|.t...s.t.|.t.
+00004730: 6a05 6a06 8302 7202 7c03 7202 7c02 7232  j.j...r.|.r.|.r2
+00004740: 7c02 6e01 7c01 9102 7102 5300 7256 0000  |.n.|...q.S.rV..
+00004750: 0029 07da 0768 6173 6174 7472 72dc 0000  .)...hasattrr...
+00004760: 0072 3800 0000 7271 0000 0072 d100 0000  .r8...rq...r....
+00004770: 72d2 0000 0072 d400 0000 2904 7262 0000  r....r....).rb..
+00004780: 0072 ba00 0000 da04 666c 6167 5a0a 6174  .r......flagZ.at
+00004790: 7472 5f76 616c 7565 a901 72c2 0000 0072  tr_value..r....r
+000047a0: 5800 0000 7259 0000 0072 6400 0000 5403  X...rY...rd...T.
+000047b0: 0000 7330 0000 0006 0006 0208 0102 fd0a  ..s0............
+000047c0: 0408 0302 f902 0802 0106 0102 fe02 f808  ................
+000047d0: 0d08 0302 fd02 0402 0106 0102 fe02 fc02  ................
+000047e0: 0802 f80a f406 0c7a 3341 7267 756d 656e  .......z3Argumen
+000047f0: 7450 6172 7365 722e 5f70 6f73 745f 7061  tParser._post_pa
+00004800: 7273 655f 6172 6773 2e3c 6c6f 6361 6c73  rse_args.<locals
+00004810: 3e2e 3c6c 6973 7463 6f6d 703e 7217 0000  >.<listcomp>r...
+00004820: 007a 2854 6865 7365 2061 7267 756d 656e  .z(These argumen
+00004830: 7473 2061 7265 206d 7574 7561 6c6c 7920  ts are mutually 
+00004840: 6578 636c 7573 6976 653a 2072 c500 0000  exclusive: r....
+00004850: 7258 0000 0029 0a72 7400 0000 72ac 0000  rX...).rt...r...
+00004860: 0072 dc00 0000 7245 0000 0072 c300 0000  .r....rE...r....
+00004870: 7260 0000 0072 df00 0000 7284 0000 0072  r`...r....r....r
+00004880: 2800 0000 da04 7661 7273 2906 727a 0000  (.....vars).rz..
+00004890: 0072 c200 0000 5a12 6675 6e63 5f6d 785f  .r....Z.func_mx_
+000048a0: 6172 675f 6772 6f75 7073 5a06 675f 6172  arg_groupsZ.g_ar
+000048b0: 6773 5a0e 6d78 5f66 6c61 6773 5f66 6f75  gsZ.mx_flags_fou
+000048c0: 6e64 72e2 0000 0072 5800 0000 72fa 0000  ndr....rX...r...
+000048d0: 0072 5900 0000 da10 5f70 6f73 745f 7061  .rY....._post_pa
+000048e0: 7273 655f 6172 6773 4503 0000 7320 0000  rse_argsE...s ..
+000048f0: 0006 070c 0102 0102 fe02 fd0c 070a 0402  ................
+00004900: 0206 fe0c 1906 0102 0106 ff0a 0302 8012  ................
+00004910: 027a 1f41 7267 756d 656e 7450 6172 7365  .z.ArgumentParse
+00004920: 722e 5f70 6f73 745f 7061 7273 655f 6172  r._post_parse_ar
+00004930: 6773 6303 0000 0000 0000 0000 0000 0005  gsc.............
+00004940: 0000 000a 0000 0003 0000 0073 5200 0000  ...........sR...
+00004950: 7a0e 7400 8300 6a01 7c01 7c02 6401 8d02  z.t...j.|.|.d...
+00004960: 7d03 7c00 a002 7c03 a101 5700 5300 0400  }.|...|...W.S...
+00004970: 7403 7928 0100 7d04 0100 7a0e 7c00 a004  t.y(..}...z.|...
+00004980: 7405 7c04 8301 a101 0100 5700 5900 6400  t.|.......W.Y.d.
+00004990: 7d04 7e04 6400 5300 6400 7d04 7e04 7701  }.~.d.S.d.}.~.w.
+000049a0: 7700 a902 4e29 0272 5000 0000 72c2 0000  w...N).rP...r...
+000049b0: 0029 0672 6b00 0000 da0a 7061 7273 655f  .).rk.....parse_
+000049c0: 6172 6773 72fc 0000 00da 0a56 616c 7565  argsr......Value
+000049d0: 4572 726f 7272 8400 0000 7271 0000 0029  Errorr....rq...)
+000049e0: 0572 7a00 0000 7250 0000 0072 c200 0000  .rz...rP...r....
+000049f0: da06 7061 7273 6564 da01 6572 7b00 0000  ..parsed..er{...
+00004a00: 7258 0000 0072 5900 0000 72fe 0000 0075  rX...rY...r....u
+00004a10: 0300 0073 1400 0000 0205 0601 0201 0201  ...s............
+00004a20: 06fe 0c04 0e01 1c01 0880 02ff 7a19 4172  ............z.Ar
+00004a30: 6775 6d65 6e74 5061 7273 6572 2e70 6172  gumentParser.par
+00004a40: 7365 5f61 7267 7363 0300 0000 0000 0000  se_argsc........
+00004a50: 0000 0000 0600 0000 0a00 0000 0300 0000  ................
+00004a60: 735a 0000 007a 1274 0083 006a 017c 017c  sZ...z.t...j.|.|
+00004a70: 0264 018d 025c 027d 037d 047c 00a0 027c  .d...\.}.}.|...|
+00004a80: 03a1 017c 0466 0257 0053 0004 0074 0379  ...|.f.W.S...t.y
+00004a90: 2c01 007d 0501 007a 0e7c 00a0 0474 057c  ,..}...z.|...t.|
+00004aa0: 0583 01a1 0101 0057 0059 0064 007d 057e  .......W.Y.d.}.~
+00004ab0: 0564 0053 0064 007d 057e 0577 0177 0072  .d.S.d.}.~.w.w.r
+00004ac0: fd00 0000 2906 726b 0000 00da 1070 6172  ....).rk.....par
+00004ad0: 7365 5f6b 6e6f 776e 5f61 7267 7372 fc00  se_known_argsr..
+00004ae0: 0000 72ff 0000 0072 8400 0000 7271 0000  ..r....r....rq..
+00004af0: 0029 0672 7a00 0000 7250 0000 0072 c200  .).rz...rP...r..
+00004b00: 0000 7200 0100 00da 0775 6e6b 6e6f 776e  ..r......unknown
+00004b10: 7201 0100 0072 7b00 0000 7258 0000 0072  r....r{...rX...r
+00004b20: 5900 0000 7202 0100 0083 0300 0073 0e00  Y...r........s..
+00004b30: 0000 0207 1401 1001 0e01 1c01 0880 02ff  ................
+00004b40: 7a1f 4172 6775 6d65 6e74 5061 7273 6572  z.ArgumentParser
+00004b50: 2e70 6172 7365 5f6b 6e6f 776e 5f61 7267  .parse_known_arg
+00004b60: 73da 1873 6b69 705f 7079 6461 6e74 6963  s..skip_pydantic
+00004b70: 5f76 616c 6964 6174 696f 6e63 0400 0000  _validationc....
+00004b80: 0000 0000 0000 0000 0600 0000 0500 0000  ................
+00004b90: 4300 0000 7322 0000 007c 00a0 007c 01a1  C...s"...|...|..
+00004ba0: 015c 027d 047d 057c 006a 017c 047c 027c  .\.}.}.|.j.|.|.|
+00004bb0: 0364 018d 037c 0566 0253 0029 0261 c902  .d...|.f.S.).a..
+00004bc0: 0000 5573 6520 7061 7273 6564 2061 7267  ..Use parsed arg
+00004bd0: 7320 746f 2069 6e73 7461 6e74 6961 7465  s to instantiate
+00004be0: 2074 6865 2067 6976 656e 2064 6174 6120   the given data 
+00004bf0: 6d6f 6465 6c2e 0a0a 2020 2020 2020 2020  model...        
+00004c00: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00004c10: 2020 6172 6773 3a0a 2020 2020 2020 2020    args:.        
+00004c20: 2020 2020 6172 6773 5f6d 6f64 656c 3a0a      args_model:.
+00004c30: 2020 2020 2020 2020 2020 2020 736b 6970              skip
+00004c40: 5f70 7964 616e 7469 635f 7661 6c69 6461  _pydantic_valida
+00004c50: 7469 6f6e 3a0a 0a20 2020 2020 2020 2045  tion:..        E
+00004c60: 7861 6d70 6c65 733a 0a20 2020 2020 2020  xamples:.       
+00004c70: 2020 2020 203e 3e3e 2069 6d70 6f72 7420       >>> import 
+00004c80: 7961 7078 0a20 2020 2020 2020 2020 2020  yapx.           
+00004c90: 203e 3e3e 2066 726f 6d20 6461 7461 636c   >>> from datacl
+00004ca0: 6173 7365 7320 696d 706f 7274 2064 6174  asses import dat
+00004cb0: 6163 6c61 7373 0a20 2020 2020 2020 2020  aclass.         
+00004cc0: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
+00004cd0: 2020 203e 3e3e 2040 6461 7461 636c 6173     >>> @dataclas
+00004ce0: 730a 2020 2020 2020 2020 2020 2020 2e2e  s.            ..
+00004cf0: 2e20 636c 6173 7320 4164 644e 756d 733a  . class AddNums:
+00004d00: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+00004d10: 2020 2020 2078 3a20 696e 740a 2020 2020       x: int.    
+00004d20: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
+00004d30: 793a 2069 6e74 0a20 2020 2020 2020 2020  y: int.         
+00004d40: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
+00004d50: 2020 203e 3e3e 2070 6172 7365 7220 3d20     >>> parser = 
+00004d60: 7961 7078 2e41 7267 756d 656e 7450 6172  yapx.ArgumentPar
+00004d70: 7365 7228 290a 2020 2020 2020 2020 2020  ser().          
+00004d80: 2020 3e3e 3e20 7061 7273 6572 2e61 6464    >>> parser.add
+00004d90: 5f61 7267 756d 656e 7473 2841 6464 4e75  _arguments(AddNu
+00004da0: 6d73 290a 2020 2020 2020 2020 2020 2020  ms).            
+00004db0: 3e3e 3e20 7061 7273 6564 2c20 756e 6b6e  >>> parsed, unkn
+00004dc0: 6f77 6e20 3d20 7061 7273 6572 2e70 6172  own = parser.par
+00004dd0: 7365 5f6b 6e6f 776e 5f61 7267 735f 746f  se_known_args_to
+00004de0: 5f6d 6f64 656c 285b 272d 7827 2c20 2731  _model(['-x', '1
+00004df0: 272c 2027 2d79 272c 2027 3227 2c20 272d  ', '-y', '2', '-
+00004e00: 7a27 2c20 2733 275d 290a 2020 2020 2020  z', '3']).      
+00004e10: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
+00004e20: 2020 2020 2020 3e3e 3e20 2870 6172 7365        >>> (parse
+00004e30: 642e 782c 2070 6172 7365 642e 7929 0a20  d.x, parsed.y). 
+00004e40: 2020 2020 2020 2020 2020 2028 312c 2032             (1, 2
+00004e50: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
+00004e60: 3e20 756e 6b6e 6f77 6e0a 2020 2020 2020  > unknown.      
+00004e70: 2020 2020 2020 5b27 2d7a 272c 2027 3327        ['-z', '3'
+00004e80: 5d0a 0a20 2020 2020 2020 20a9 0372 5000  ]..        ..rP.
+00004e90: 0000 7291 0000 0072 0401 0000 2902 7202  ..r....r....).r.
+00004ea0: 0100 00da 145f 7061 7273 655f 6172 6773  ....._parse_args
+00004eb0: 5f74 6f5f 6d6f 6465 6c29 0672 7a00 0000  _to_model).rz...
+00004ec0: 7250 0000 0072 9100 0000 7204 0100 00da  rP...r....r.....
+00004ed0: 0b70 6172 7365 645f 6172 6773 da0c 756e  .parsed_args..un
+00004ee0: 6b6e 6f77 6e5f 6172 6773 7258 0000 0072  known_argsrX...r
+00004ef0: 5800 0000 7259 0000 00da 1970 6172 7365  X...rY.....parse
+00004f00: 5f6b 6e6f 776e 5f61 7267 735f 746f 5f6d  _known_args_to_m
+00004f10: 6f64 656c 9003 0000 7310 0000 000e 2304  odel....s.....#.
+00004f20: 0302 0102 0102 0104 fd02 0504 fa7a 2841  .............z(A
+00004f30: 7267 756d 656e 7450 6172 7365 722e 7061  rgumentParser.pa
+00004f40: 7273 655f 6b6e 6f77 6e5f 6172 6773 5f74  rse_known_args_t
+00004f50: 6f5f 6d6f 6465 6c63 0400 0000 0000 0000  o_modelc........
+00004f60: 0000 0000 0500 0000 0500 0000 4300 0000  ............C...
+00004f70: 731a 0000 007c 00a0 007c 01a1 017d 047c  s....|...|...}.|
+00004f80: 006a 017c 047c 027c 0364 018d 0353 0029  .j.|.|.|.d...S.)
+00004f90: 0261 7f02 0000 5573 6520 7061 7273 6564  .a....Use parsed
+00004fa0: 2061 7267 7320 746f 2069 6e73 7461 6e74   args to instant
+00004fb0: 6961 7465 2074 6865 2067 6976 656e 2064  iate the given d
+00004fc0: 6174 6120 6d6f 6465 6c2e 0a0a 2020 2020  ata model...    
+00004fd0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00004fe0: 2020 2020 2020 6172 6773 3a0a 2020 2020        args:.    
+00004ff0: 2020 2020 2020 2020 6172 6773 5f6d 6f64          args_mod
+00005000: 656c 3a0a 2020 2020 2020 2020 2020 2020  el:.            
+00005010: 736b 6970 5f70 7964 616e 7469 635f 7661  skip_pydantic_va
+00005020: 6c69 6461 7469 6f6e 3a0a 0a20 2020 2020  lidation:..     
+00005030: 2020 2045 7861 6d70 6c65 733a 0a20 2020     Examples:.   
+00005040: 2020 2020 2020 2020 203e 3e3e 2069 6d70           >>> imp
+00005050: 6f72 7420 7961 7078 0a20 2020 2020 2020  ort yapx.       
+00005060: 2020 2020 203e 3e3e 2066 726f 6d20 6461       >>> from da
+00005070: 7461 636c 6173 7365 7320 696d 706f 7274  taclasses import
+00005080: 2064 6174 6163 6c61 7373 0a20 2020 2020   dataclass.     
+00005090: 2020 2020 2020 202e 2e2e 0a20 2020 2020         ....     
+000050a0: 2020 2020 2020 203e 3e3e 2040 6461 7461         >>> @data
+000050b0: 636c 6173 730a 2020 2020 2020 2020 2020  class.          
+000050c0: 2020 2e2e 2e20 636c 6173 7320 4164 644e    ... class AddN
+000050d0: 756d 733a 0a20 2020 2020 2020 2020 2020  ums:.           
+000050e0: 202e 2e2e 2020 2020 2078 3a20 696e 740a   ...     x: int.
+000050f0: 2020 2020 2020 2020 2020 2020 2e2e 2e20              ... 
+00005100: 2020 2020 793a 2069 6e74 0a20 2020 2020      y: int.     
+00005110: 2020 2020 2020 202e 2e2e 0a20 2020 2020         ....     
+00005120: 2020 2020 2020 203e 3e3e 2070 6172 7365         >>> parse
+00005130: 7220 3d20 7961 7078 2e41 7267 756d 656e  r = yapx.Argumen
+00005140: 7450 6172 7365 7228 290a 2020 2020 2020  tParser().      
+00005150: 2020 2020 2020 3e3e 3e20 7061 7273 6572        >>> parser
+00005160: 2e61 6464 5f61 7267 756d 656e 7473 2841  .add_arguments(A
+00005170: 6464 4e75 6d73 290a 2020 2020 2020 2020  ddNums).        
+00005180: 2020 2020 3e3e 3e20 7061 7273 6564 203d      >>> parsed =
+00005190: 2070 6172 7365 722e 7061 7273 655f 6172   parser.parse_ar
+000051a0: 6773 5f74 6f5f 6d6f 6465 6c28 5b27 2d78  gs_to_model(['-x
+000051b0: 272c 2027 3127 2c20 272d 7927 2c20 2732  ', '1', '-y', '2
+000051c0: 275d 290a 2020 2020 2020 2020 2020 2020  ']).            
+000051d0: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+000051e0: 3e3e 3e20 2870 6172 7365 642e 782c 2070  >>> (parsed.x, p
+000051f0: 6172 7365 642e 7929 0a20 2020 2020 2020  arsed.y).       
+00005200: 2020 2020 2028 312c 2032 290a 0a20 2020       (1, 2)..   
+00005210: 2020 2020 2072 0501 0000 2902 72fe 0000       r....).r...
+00005220: 0072 0601 0000 2905 727a 0000 0072 5000  .r....).rz...rP.
+00005230: 0000 7291 0000 0072 0401 0000 7207 0100  ..r....r....r...
+00005240: 0072 5800 0000 7258 0000 0072 5900 0000  .rX...rX...rY...
+00005250: da13 7061 7273 655f 6172 6773 5f74 6f5f  ..parse_args_to_
+00005260: 6d6f 6465 6cbe 0300 0073 0c00 0000 0a1e  model....s......
+00005270: 0401 0201 0201 0201 06fd 7a22 4172 6775  ..........z"Argu
+00005280: 6d65 6e74 5061 7273 6572 2e70 6172 7365  mentParser.parse
+00005290: 5f61 7267 735f 746f 5f6d 6f64 656c 6304  _args_to_modelc.
+000052a0: 0000 0000 0000 0000 0000 0008 0000 000a  ................
+000052b0: 0000 0043 0000 0073 aa00 0000 7400 7c01  ...C...s....t.|.
+000052c0: 8301 7d04 7c02 7310 7c04 a001 7c00 6a02  ..}.|.s.|...|.j.
+000052d0: a101 7d02 7c02 7310 7403 8201 7c00 6a04  ..}.|.s.t...|.j.
+000052e0: 7c04 7c02 6401 8d02 7d05 7405 724e 7c03  |.|.d...}.t.rN|.
+000052f0: 734e 7a0d 7400 7406 7c02 8301 6405 6900  sNz.t.t.|...d.i.
+00005300: 7c05 a401 8e01 8301 7d05 5700 6e25 0400  |.......}.W.n%..
+00005310: 7407 794d 0100 7d06 0100 7a19 6402 6402  t.yM..}...z.d.d.
+00005320: a008 6403 6404 8400 7c06 a009 a100 4400  ..d.d...|.....D.
+00005330: 8301 a101 1700 7d07 7c00 a00a 7c07 a101  ......}.|...|...
+00005340: 0100 5700 5900 6400 7d06 7e06 6e05 6400  ..W.Y.d.}.~.n.d.
+00005350: 7d06 7e06 7701 7700 7c02 6405 6900 7c05  }.~.w.w.|.d.i.|.
+00005360: a401 8e01 5300 2906 4ea9 02da 0961 7267  ....S.).N....arg
+00005370: 735f 6469 6374 7291 0000 0072 7f00 0000  s_dictr....r....
+00005380: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00005390: 0006 0000 0073 0000 0073 2e00 0000 8100  .....s...s......
+000053a0: 7c00 5d12 7d01 6400 7c01 6401 1900 6402  |.].}.d.|.d...d.
+000053b0: 1900 9b00 6403 7c01 6404 1900 9b00 6405  ....d.|.d.....d.
+000053c0: 9d05 5600 0100 7102 6406 5300 2907 7a18  ..V...q.d.S.).z.
+000053d0: 4572 726f 7220 7061 7273 696e 6720 6172  Error parsing ar
+000053e0: 6775 6d65 6e74 2060 da03 6c6f 6372 0100  gument `..locr..
+000053f0: 0000 7a03 603b 20da 036d 7367 72ae 0000  ..z.`; ..msgr...
+00005400: 004e 7258 0000 0072 6100 0000 7258 0000  .NrX...ra...rX..
+00005410: 0072 5800 0000 7259 0000 00da 093c 6765  .rX...rY.....<ge
+00005420: 6e65 7870 723e fc03 0000 730a 0000 0002  nexpr>....s.....
+00005430: 8004 0002 021c ff0a ff7a 3641 7267 756d  .........z6Argum
+00005440: 656e 7450 6172 7365 722e 5f70 6172 7365  entParser._parse
+00005450: 5f61 7267 735f 746f 5f6d 6f64 656c 2e3c  _args_to_model.<
+00005460: 6c6f 6361 6c73 3e2e 3c67 656e 6578 7072  locals>.<genexpr
+00005470: 3e72 5800 0000 290b 72fb 0000 0072 ac00  >rX...).r....r..
+00005480: 0000 7246 0000 0072 2600 0000 da16 5f75  ..rF...r&....._u
+00005490: 6e69 6f6e 5f61 7267 735f 7769 7468 5f6d  nion_args_with_m
+000054a0: 6f64 656c 7235 0000 0072 3300 0000 722e  odelr5...r3...r.
+000054b0: 0000 0072 df00 0000 da06 6572 726f 7273  ...r......errors
+000054c0: 7284 0000 0029 0872 7a00 0000 7250 0000  r....).rz...rP..
+000054d0: 0072 9100 0000 7204 0100 0072 0701 0000  .r....r....r....
+000054e0: 5a0a 6172 6773 5f75 6e69 6f6e 7201 0100  Z.args_unionr...
+000054f0: 0072 e200 0000 7258 0000 0072 5800 0000  .r....rX...rX...
+00005500: 7259 0000 0072 0601 0000 e303 0000 732c  rY...r........s,
+00005510: 0000 0008 0604 020c 0104 0104 0104 0202  ................
+00005520: 0102 0106 fe08 0502 0202 0110 0108 ff0e  ................
+00005530: 030c 0106 020a fe16 0408 8002 fb0e 077a  ...............z
+00005540: 2341 7267 756d 656e 7450 6172 7365 722e  #ArgumentParser.
+00005550: 5f70 6172 7365 5f61 7267 735f 746f 5f6d  _parse_args_to_m
+00005560: 6f64 656c 720c 0100 0063 0200 0000 0000  odelr....c......
+00005570: 0000 0000 0000 0200 0000 0300 0000 0300  ................
+00005580: 0000 7316 0000 0087 0066 0164 0164 0284  ..s......f.d.d..
+00005590: 087c 00a0 00a1 0044 0083 0153 0029 034e  .|.....D...S.).N
+000055a0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+000055b0: 0004 0000 0013 0000 0073 2000 0000 6900  .........s ...i.
+000055c0: 7c00 5d0c 5c02 7d01 7d02 7c01 8800 6a00  |.].\.}.}.|...j.
+000055d0: 7600 7202 7c01 7c02 9302 7102 5300 7258  v.r.|.|...q.S.rX
+000055e0: 0000 0072 a300 0000 a903 7262 0000 0072  ...r......rb...r
+000055f0: e400 0000 72f6 0000 0072 9600 0000 7258  ....r....r....rX
+00005600: 0000 0072 5900 0000 da0a 3c64 6963 7463  ...rY.....<dictc
+00005610: 6f6d 703e 0904 0000 7267 0000 007a 3941  omp>....rg...z9A
+00005620: 7267 756d 656e 7450 6172 7365 722e 5f75  rgumentParser._u
+00005630: 6e69 6f6e 5f61 7267 735f 7769 7468 5f6d  nion_args_with_m
+00005640: 6f64 656c 2e3c 6c6f 6361 6c73 3e2e 3c64  odel.<locals>.<d
+00005650: 6963 7463 6f6d 703e 2901 728f 0000 0072  ictcomp>).r....r
+00005660: 0b01 0000 7258 0000 0072 9600 0000 7259  ....rX...r....rY
+00005670: 0000 0072 1001 0000 0404 0000 7302 0000  ...r........s...
+00005680: 0016 057a 2541 7267 756d 656e 7450 6172  ...z%ArgumentPar
+00005690: 7365 722e 5f75 6e69 6f6e 5f61 7267 735f  ser._union_args_
+000056a0: 7769 7468 5f6d 6f64 656c 6302 0000 0000  with_modelc.....
+000056b0: 0000 0000 0000 0006 0000 0004 0000 0043  ...............C
+000056c0: 0000 0073 8000 0000 6400 7d02 7c01 6a00  ...s....d.}.|.j.
+000056d0: 7215 7c01 6a00 a001 7c01 6a02 6401 1700  r.|.j...|.j.d...
+000056e0: a101 7315 7c01 6a00 a003 a100 a004 a100  ..s.|.j.........
+000056f0: 7d02 7c02 7319 6400 5300 6402 7d03 7405  }.|.s.d.S.d.}.t.
+00005700: 7c02 8301 4400 5d0c 5c02 7d04 7d05 7c05  |...D.].\.}.}.|.
+00005710: a003 a100 732b 7c04 7d03 0100 6e01 711f  ....s+|.}...n.q.
+00005720: 7c03 6402 6b04 7236 7c02 6400 7c03 8502  |.d.k.r6|.d.|...
+00005730: 1900 7d02 6403 a006 6404 6405 8400 7c02  ..}.d...d.d...|.
+00005740: 4400 8301 a101 5300 2906 4efa 0128 7201  D.....S.).N..(r.
+00005750: 0000 0072 7f00 0000 6301 0000 0000 0000  ...r....c.......
+00005760: 0000 0000 0002 0000 0003 0000 0073 0000  .............s..
+00005770: 0073 1800 0000 8100 7c00 5d07 7d01 7c01  .s......|.].}.|.
+00005780: a000 a100 5600 0100 7102 6400 5300 7256  ....V...q.d.S.rV
+00005790: 0000 0029 01da 0573 7472 6970 7261 0000  ...)...stripra..
+000057a0: 0072 5800 0000 7258 0000 0072 5900 0000  .rX...rX...rY...
+000057b0: 720f 0100 0023 0400 0073 0400 0000 0280  r....#...s......
+000057c0: 1600 7a41 4172 6775 6d65 6e74 5061 7273  ..zAArgumentPars
+000057d0: 6572 2e5f 6765 745f 6465 7363 7269 7074  er._get_descript
+000057e0: 696f 6e5f 6672 6f6d 5f64 6f63 7374 7269  ion_from_docstri
+000057f0: 6e67 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  ng.<locals>.<gen
+00005800: 6578 7072 3e29 07da 075f 5f64 6f63 5f5f  expr>)...__doc__
+00005810: 725f 0000 0072 9700 0000 7215 0100 0072  r_...r....r....r
+00005820: 9b00 0000 da09 656e 756d 6572 6174 6572  ......enumerater
+00005830: df00 0000 2906 72a9 0000 0072 9100 0000  ....).r....r....
+00005840: 5a11 6465 7363 7269 7074 696f 6e5f 6c69  Z.description_li
+00005850: 6e65 735a 1274 6578 745f 626c 6f63 6b5f  nesZ.text_block_
+00005860: 656e 6473 5f61 74da 0169 da04 6c69 6e65  ends_at..i..line
+00005870: 7258 0000 0072 5800 0000 7259 0000 0072  rX...rX...rY...r
+00005880: 9a00 0000 0b04 0000 7320 0000 0004 050c  ........s ......
+00005890: 0208 0104 ff0e 0304 0204 0104 0210 0108  ................
+000058a0: 0104 0104 0102 fe08 040c 0114 027a 2e41  .............z.A
+000058b0: 7267 756d 656e 7450 6172 7365 722e 5f67  rgumentParser._g
+000058c0: 6574 5f64 6573 6372 6970 7469 6f6e 5f66  et_description_f
+000058d0: 726f 6d5f 646f 6373 7472 696e 6763 0300  rom_docstringc..
+000058e0: 0000 0000 0000 0000 0000 0400 0000 0300  ................
+000058f0: 0000 4300 0000 731c 0000 007c 00a0 007c  ..C...s....|...|
+00005900: 02a1 017d 037c 0372 0c7c 037c 015f 0164  ...}.|.r.|.|._.d
+00005910: 0053 0064 0053 0072 5600 0000 2902 729a  .S.d.S.rV...).r.
+00005920: 0000 0072 4900 0000 2904 72a9 0000 0072  ...rI...).r....r
+00005930: 5c00 0000 7291 0000 0072 4900 0000 7258  \...r....rI...rX
+00005940: 0000 0072 5800 0000 7259 0000 00da 1f5f  ...rX...rY....._
+00005950: 7365 745f 6465 7363 7269 7074 696f 6e5f  set_description_
+00005960: 6672 6f6d 5f64 6f63 7374 7269 6e67 2504  from_docstring%.
+00005970: 0000 7308 0000 000a 0604 020a 0104 ff7a  ..s............z
+00005980: 2e41 7267 756d 656e 7450 6172 7365 722e  .ArgumentParser.
+00005990: 5f73 6574 5f64 6573 6372 6970 7469 6f6e  _set_description
+000059a0: 5f66 726f 6d5f 646f 6373 7472 696e 67da  _from_docstring.
+000059b0: 0b6c 696e 6b65 645f 6675 6e63 da0b 7265  .linked_func..re
+000059c0: 6c61 795f 7661 6c75 6563 0700 0000 0000  lay_valuec......
+000059d0: 0000 0000 0000 1700 0000 0700 0000 0300  ................
+000059e0: 0000 73e6 0100 0067 007d 0769 007d 0864  ..s....g.}.i.}.d
+000059f0: 017d 0964 017d 0a64 017d 0b64 017d 0c64  .}.d.}.d.}.d.}.d
+00005a00: 017d 0d74 007c 0283 016a 01a0 02a1 0044  .}.t.|...j.....D
+00005a10: 005d 437d 0e74 037c 0e83 01a0 0464 02a1  .]C}.t.|.....d..
+00005a20: 0172 2164 037d 0c71 1574 037c 0e83 01a0  .r!d.}.q.t.|....
+00005a30: 0464 04a1 0172 2b64 037d 0a71 157c 0e6a  .d...r+d.}.q.|.j
+00005a40: 0564 056b 0272 3364 037d 0b71 157c 0e6a  .d.k.r3d.}.q.|.j
+00005a50: 0564 066b 0272 3b64 037d 0d71 157c 0e6a  .d.k.r;d.}.q.|.j
+00005a60: 0564 076b 0272 457c 037c 0864 073c 0071  .d.k.rE|.|.d.<.q
+00005a70: 157c 0e6a 0564 086b 0272 4f7c 067c 0864  .|.j.d.k.rO|.|.d
+00005a80: 083c 0071 157c 0e6a 0564 096b 0272 5864  .<.q.|.j.d.k.rXd
+00005a90: 037c 0864 093c 0071 157c 0a70 607c 0c70  .|.d.<.q.|.p`|.p
+00005aa0: 607c 0b70 607c 0d7d 097c 0973 737c 0572  `|.p`|.}.|.ss|.r
+00005ab0: 7374 0664 0a64 0b84 0074 007c 0583 016a  st.d.d...t.|...j
+00005ac0: 01a0 02a1 0044 0083 0183 017d 097c 0473  .....D.....}.|.s
+00005ad0: 7974 077c 0283 017d 047c 0972 e17c 016a  yt.|...}.|.r.|.j
+00005ae0: 087c 037c 0464 0c8d 025c 027d 0f7d 107c  .|.|.d...\.}.}.|
+00005af0: 0c73 887c 0d72 d669 0089 007c 0083 007d  .s.|.r.i...|...}
+00005b00: 117c 1044 005d 247d 127c 12a0 0464 0da1  .|.D.]$}.|...d..
+00005b10: 0172 b37c 126a 0964 0e64 0f64 108d 0264  .r.|.j.d.d.d...d
+00005b20: 1119 007d 137c 13a0 0a64 0da1 017d 147c  ...}.|...d...}.|
+00005b30: 1472 b37c 116a 0b7c 1364 1264 0064 0164  .r.|.j.|.d.d.d.d
+00005b40: 138d 0401 007c 1388 007c 143c 0071 8f7c  .....|...|.<.q.|
+00005b50: 116a 0c7c 1064 148d 015c 027d 157d 1087  .j.|.d...\.}.}..
+00005b60: 0066 0164 1564 1684 0874 0d7c 1583 01a0  .f.d.d...t.|....
+00005b70: 0ea1 0044 0083 017d 167c 0c72 d07c 08a0  ...D...}.|.r.|..
+00005b80: 0f7c 16a1 0101 007c 0d72 d67c 167c 0864  .|.....|.r.|.|.d
+00005b90: 063c 007c 0a72 da7c 107d 077c 0b72 e07c  .<.|.r.|.}.|.r.|
+00005ba0: 107c 0864 053c 006e 077c 016a 107c 037c  .|.d.<.n.|.j.|.|
+00005bb0: 0464 0c8d 027d 0f7c 027c 0769 0074 0d7c  .d...}.|.|.i.t.|
+00005bc0: 0f83 01a4 017c 08a4 018e 0153 0029 174e  .....|.....S.).N
+00005bd0: 467a 022a 2a54 72b5 0000 00da 0b5f 6578  Fz.**Tr......_ex
+00005be0: 7472 615f 6172 6773 da0d 5f65 7874 7261  tra_args.._extra
+00005bf0: 5f6b 7761 7267 735a 095f 616c 6c5f 6172  _kwargsZ._all_ar
+00005c00: 6773 5a0c 5f72 656c 6179 5f76 616c 7565  gsZ._relay_value
+00005c10: 5a10 5f63 616c 6c65 645f 6672 6f6d 5f63  Z._called_from_c
+00005c20: 6c69 6301 0000 0000 0000 0000 0000 0002  lic.............
+00005c30: 0000 0004 0000 0073 0000 0073 2800 0000  .......s...s(...
+00005c40: 8100 7c00 5d0f 7d01 7400 7c01 8301 a001  ..|.].}.t.|.....
+00005c50: 6400 a101 700f 7c01 6a02 6401 7600 5600  d...p.|.j.d.v.V.
+00005c60: 0100 7102 6402 5300 2903 72b5 0000 0029  ..q.d.S.).r....)
+00005c70: 0272 1d01 0000 721e 0100 004e 2903 7271  .r....r....N).rq
+00005c80: 0000 0072 5f00 0000 7294 0000 0029 0272  ...r_...r....).r
+00005c90: 6200 0000 da01 7072 5800 0000 7258 0000  b.....prX...rX..
+00005ca0: 0072 5900 0000 720f 0100 005a 0400 0073  .rY...r....Z...s
+00005cb0: 0a00 0000 0280 0400 0202 16ff 0aff 7a2b  ..............z+
+00005cc0: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
+00005cd0: 7275 6e5f 6675 6e63 2e3c 6c6f 6361 6c73  run_func.<locals
+00005ce0: 3e2e 3c67 656e 6578 7072 3e29 0272 5000  >.<genexpr>).rP.
+00005cf0: 0000 7291 0000 0072 5b00 0000 7255 0000  ..r....r[...rU..
+00005d00: 0072 1700 0000 72af 0000 0072 0100 0000  .r....r....r....
+00005d10: 72be 0000 0029 0372 bd00 0000 7269 0000  r....).r....ri..
+00005d20: 0072 bc00 0000 2901 7250 0000 0063 0100  .r....).rP...c..
+00005d30: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00005d40: 0000 1300 0000 731a 0000 0069 007c 005d  ......s....i.|.]
+00005d50: 095c 027d 017d 0288 007c 0119 007c 0293  .\.}.}...|...|..
+00005d60: 0271 0253 0072 5800 0000 7258 0000 0072  .q.S.rX...rX...r
+00005d70: 1201 0000 a901 5a10 756e 6b6e 6f77 6e5f  ......Z.unknown_
+00005d80: 6e61 6d65 5f6d 6170 7258 0000 0072 5900  name_maprX...rY.
+00005d90: 0000 7213 0100 007e 0400 0073 0600 0000  ..r....~...s....
+00005da0: 0600 0e01 06ff 7a2c 4172 6775 6d65 6e74  ......z,Argument
+00005db0: 5061 7273 6572 2e5f 7275 6e5f 6675 6e63  Parser._run_func
+00005dc0: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
+00005dd0: 6f6d 703e 2911 7209 0000 00da 0a70 6172  omp>).r......par
+00005de0: 616d 6574 6572 7372 c300 0000 7271 0000  ametersr....rq..
+00005df0: 0072 5f00 0000 7294 0000 00da 0361 6e79  .r_...r......any
+00005e00: 7225 0000 0072 0901 0000 da05 7370 6c69  r%...r......spli
+00005e10: 74da 066c 7374 7269 7072 7200 0000 7202  t..lstriprr...r.
+00005e20: 0100 0072 fb00 0000 728f 0000 00da 0675  ...r....r......u
+00005e30: 7064 6174 6572 0a01 0000 2917 72a9 0000  pdater....).r...
+00005e40: 0072 5c00 0000 729e 0000 0072 5000 0000  .r\...r....rP...
+00005e50: 7291 0000 0072 1b01 0000 721c 0100 005a  r....r....r....Z
+00005e60: 0966 756e 635f 6172 6773 5a0b 6675 6e63  .func_argsZ.func
+00005e70: 5f6b 7761 7267 735a 0d65 7874 7261 5f61  _kwargsZ.extra_a
+00005e80: 7267 735f 6f6b 5a0c 6163 6365 7074 735f  rgs_okZ.accepts_
+00005e90: 6172 6773 5a12 6163 6365 7074 735f 6578  argsZ.accepts_ex
+00005ea0: 7472 615f 6172 6773 5a0e 6163 6365 7074  tra_argsZ.accept
+00005eb0: 735f 6b77 6172 6773 5a14 6163 6365 7074  s_kwargsZ.accept
+00005ec0: 735f 6578 7472 615f 6b77 6172 6773 721f  s_extra_kwargsr.
+00005ed0: 0100 005a 0a6d 6f64 656c 5f69 6e73 7472  ...Z.model_instr
+00005ee0: 0801 0000 5a0e 756e 6b6e 6f77 6e5f 7061  ....Z.unknown_pa
+00005ef0: 7273 6572 7263 0000 005a 0678 5f66 6c61  rserrc...Z.x_fla
+00005f00: 675a 0b78 5f66 6c61 675f 6261 7265 5a0e  gZ.x_flag_bareZ.
+00005f10: 7061 7273 6564 5f75 6e6b 6e6f 776e 5a0c  parsed_unknownZ.
+00005f20: 6578 7472 615f 6b77 6172 6773 7258 0000  extra_kwargsrX..
+00005f30: 0072 2001 0000 7259 0000 00da 095f 7275  .r ...rY....._ru
+00005f40: 6e5f 6675 6e63 3004 0000 7390 0000 0004  n_func0...s.....
+00005f50: 0a04 0104 0204 0204 0104 0204 0112 020e  ................
+00005f60: 0106 010e 0106 010a 0106 010a 0106 010a  ................
+00005f70: 010a 010a 010a 010a 0108 0102 800e 0302  ................
+00005f80: ff08 0408 010c 0208 fe04 0508 0104 0304  ................
+00005f90: 0202 0102 010a fe08 0504 0106 0108 010a  ................
+00005fa0: 0112 010a 0104 0104 0102 0102 0102 0102  ................
+00005fb0: 0106 fc08 0602 8004 0202 010a ff0a 040a  ................
+00005fc0: 0106 ff04 030a 0104 0108 0104 0204 0104  ................
+00005fd0: 0208 0102 8004 0302 0102 0106 fe16 057a  ...............z
+00005fe0: 1841 7267 756d 656e 7450 6172 7365 722e  .ArgumentParser.
+00005ff0: 5f72 756e 5f66 756e 6372 5d00 0000 da0b  _run_funcr].....
+00006000: 7375 6263 6f6d 6d61 6e64 73da 116e 616d  subcommands..nam
+00006010: 6564 5f73 7562 636f 6d6d 616e 6473 6304  ed_subcommandsc.
+00006020: 0000 0000 0000 0000 0000 0009 0000 000b  ................
+00006030: 0000 004b 0000 0073 d200 0000 7c00 6403  ...K...s....|.d.
+00006040: 6900 7c04 a401 8e01 7d05 7c01 722e 7400  i.|.....}.|.r.t.
+00006050: 7c01 8301 7d06 7c00 6a01 7c05 7c06 6401  |...}.|.j.|.|.d.
+00006060: 8d02 0100 7c05 a002 7c06 a101 0100 7c05  ....|...|.....|.
+00006070: 6a03 6403 6900 7c00 6a04 7c01 7c00 6a05  j.d.i.|.j.|.|.j.
+00006080: 7c06 7c00 6a06 7c01 7c00 6a07 7c06 6904  |.|.j.|.|.j.|.i.
+00006090: a401 8e01 0100 6e14 7c05 6a03 6403 6900  ......n.|.j.d.i.
+000060a0: 7c00 6a05 6400 7c00 6a04 6400 7c00 6a07  |.j.d.|.j.d.|.j.
+000060b0: 6400 7c00 6a06 6400 6904 a401 8e01 0100  d.|.j.d.i.......
+000060c0: 7c02 7255 7408 7c02 8301 724b 7c02 6701  |.rUt.|...rK|.g.
+000060d0: 7d02 7c02 4400 5d07 7d07 7c05 a009 7c07  }.|.D.].}.|...|.
+000060e0: a101 0100 714d 7c03 7267 7c03 a00a a100  ....qM|.rg|.....
+000060f0: 4400 5d0b 5c02 7d08 7d07 7c05 6a09 7c07  D.].\.}.}.|.j.|.
+00006100: 7c08 6402 8d02 0100 715b 7c05 5300 2904  |.d.....q[|.S.).
+00006110: 4e29 0272 5c00 0000 7291 0000 0072 b300  N).r\...r....r..
+00006120: 0000 7258 0000 0029 0b72 2500 0000 721a  ..rX...).r%...r.
+00006130: 0100 0072 9300 0000 729f 0000 0072 4200  ...r....r....rB.
+00006140: 0000 7243 0000 0072 4500 0000 7246 0000  ..rC...rE...rF..
+00006150: 00da 0863 616c 6c61 626c 6572 a000 0000  ...callabler....
+00006160: 728f 0000 0029 0972 a900 0000 725d 0000  r....).r....r]..
+00006170: 0072 2701 0000 7228 0100 0072 5100 0000  .r'...r(...rQ...
+00006180: 725c 0000 005a 0e72 6f6f 745f 6172 675f  r\...Z.root_arg_
+00006190: 6d6f 6465 6c72 6300 0000 7294 0000 0072  modelrc...r....r
+000061a0: 5800 0000 7258 0000 0072 5900 0000 da0d  X...rX...rY.....
+000061b0: 5f62 7569 6c64 5f70 6172 7365 7294 0400  _build_parser...
+000061c0: 0073 3e00 0000 0e08 0402 0801 0401 0201  .s>.............
+000061d0: 0201 06fe 0a04 0801 0602 0601 0601 0601  ................
+000061e0: 02fc 08ff 0809 0602 0601 0601 0601 02fc  ................
+000061f0: 06ff 0409 0801 0601 0801 0c01 0402 1001  ................
+00006200: 1001 0402 7a1c 4172 6775 6d65 6e74 5061  ....z.ArgumentPa
+00006210: 7273 6572 2e5f 6275 696c 645f 7061 7273  rser._build_pars
+00006220: 6572 2902 7250 0000 00da 0c64 6566 6175  er).rP.....defau
+00006230: 6c74 5f61 7267 73da 0b70 6172 7365 725f  lt_args..parser_
+00006240: 6172 6773 722b 0100 00da 0d70 6172 7365  argsr+.....parse
+00006250: 725f 6b77 6172 6773 6301 0000 0000 0000  r_kwargsc.......
+00006260: 0002 0000 0011 0000 0009 0000 004f 0000  .............O..
+00006270: 0073 3801 0000 7c00 6a00 7c03 6900 7c04  .s8...|.j.|.i.|.
+00006280: a401 8e01 7d05 7c01 6401 7500 7213 7401  ....}.|.d.u.r.t.
+00006290: 6a02 6402 6401 8502 1900 7d01 7c01 7319  j.d.d.....}.|.s.
+000062a0: 7c02 7219 7c02 7d01 7c05 a003 7c01 a101  |.r.|.}.|...|...
+000062b0: 5c02 7d06 7d07 7404 7c06 8301 7d08 7c08  \.}.}.t.|...}.|.
+000062c0: a005 7c00 6a06 a101 7d09 7c08 a005 7c00  ..|.j...}.|...|.
+000062d0: 6a07 a101 7d0a 7c08 a005 7c00 6a08 a101  j...}.|...|.j...
+000062e0: 7d0b 7c08 a005 7c00 6a09 a101 7d0c 7c08  }.|...|.j...}.|.
+000062f0: a005 7c00 6a0a a101 7d0d 6401 7d0e 6401  ..|.j...}.d.}.d.
+00006300: 7d0f 7c09 7252 7c00 6a0b 7c05 7c09 7c0a  }.|.rR|.j.|.|.|.
+00006310: 7c0c 7c01 6403 8d05 7d0f 740c 7c0f 740d  |.|.d...}.t.|.t.
+00006320: 8302 7269 7a06 740e 7c0f 8301 7d0e 5700  ..riz.t.|...}.W.
+00006330: 6e0d 0400 740f 7968 0100 0100 0100 7c0f  n...t.yh......|.
+00006340: 7d0e 5900 6e03 7700 7c0f 7d0e 7a20 7c0b  }.Y.n.w.|.}.z |.
+00006350: 727b 7c0c 727b 7c00 6a0b 7c05 7c0c 7c0d  r{|.r{|.j.|.|.|.
+00006360: 7c01 7c09 7c0e 6404 8d06 7d0e 5700 740c  |.|.|.d...}.W.t.
+00006370: 7c0f 740d 8302 728a 7c0f 4400 5d06 7d10  |.t...r.|.D.].}.
+00006380: 7c0c 7389 7c10 7d0e 7183 7c0e 5300 740c  |.s.|.}.q.|.S.t.
+00006390: 7c0f 740d 8302 729a 7c0f 4400 5d07 7d10  |.t...r.|.D.].}.
+000063a0: 7c0c 7399 7c10 7d0e 7193 7700 7700 2905  |.s.|.}.q.w.w.).
+000063b0: 612d 0300 0055 7365 2067 6976 656e 2066  a-...Use given f
+000063c0: 756e 6374 696f 6e73 2074 6f20 636f 6e73  unctions to cons
+000063d0: 7472 7563 7420 6120 434c 492c 2070 6172  truct a CLI, par
+000063e0: 7365 2074 6865 2061 7267 732c 2061 6e64  se the args, and
+000063f0: 2069 6e76 6f6b 6520 7468 6520 6170 7072   invoke the appr
+00006400: 6f70 7269 6174 6520 636f 6d6d 616e 642e  opriate command.
+00006410: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00006420: 2020 2020 2020 2020 2020 2020 2a70 6172              *par
+00006430: 7365 725f 6172 6773 3a0a 2020 2020 2020  ser_args:.      
+00006440: 2020 2020 2020 6172 6773 3a0a 2020 2020        args:.    
+00006450: 2020 2020 2020 2020 6465 6661 756c 745f          default_
+00006460: 6172 6773 3a0a 2020 2020 2020 2020 2020  args:.          
+00006470: 2020 2a2a 7061 7273 6572 5f6b 7761 7267    **parser_kwarg
+00006480: 733a 0a0a 0a20 2020 2020 2020 2045 7861  s:...        Exa
+00006490: 6d70 6c65 733a 0a20 2020 2020 2020 2020  mples:.         
+000064a0: 2020 203e 3e3e 2069 6d70 6f72 7420 7961     >>> import ya
+000064b0: 7078 0a20 2020 2020 2020 2020 2020 202e  px.            .
+000064c0: 2e2e 0a20 2020 2020 2020 2020 2020 203e  ...            >
+000064d0: 3e3e 2064 6566 2070 7269 6e74 5f6e 756d  >> def print_num
+000064e0: 7328 2a61 7267 7329 3a0a 2020 2020 2020  s(*args):.      
+000064f0: 2020 2020 2020 2e2e 2e20 2020 2020 7072        ...     pr
+00006500: 696e 7428 2741 7267 733a 2027 2c20 2a61  int('Args: ', *a
+00006510: 7267 7329 0a20 2020 2020 2020 2020 2020  rgs).           
+00006520: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
+00006530: 203e 3e3e 2064 6566 2066 696e 645f 6576   >>> def find_ev
+00006540: 656e 7328 2a61 7267 7329 3a0a 2020 2020  ens(*args):.    
+00006550: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
+00006560: 7265 7475 726e 205b 7820 666f 7220 7820  return [x for x 
+00006570: 696e 2061 7267 7320 6966 2069 6e74 2878  in args if int(x
+00006580: 2920 2520 3220 3d3d 2030 5d0a 2020 2020  ) % 2 == 0].    
+00006590: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
+000065a0: 2020 2020 2020 2020 3e3e 3e20 6465 6620          >>> def 
+000065b0: 6669 6e64 5f6f 6464 7328 2a61 7267 7329  find_odds(*args)
+000065c0: 3a0a 2020 2020 2020 2020 2020 2020 2e2e  :.            ..
+000065d0: 2e20 2020 2020 7265 7475 726e 205b 7820  .     return [x 
+000065e0: 666f 7220 7820 696e 2061 7267 7320 6966  for x in args if
+000065f0: 2069 6e74 2878 2920 2520 3220 213d 2030   int(x) % 2 != 0
+00006600: 5d0a 2020 2020 2020 2020 2020 2020 2e2e  ].            ..
+00006610: 2e0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
+00006620: 3e20 636c 695f 6172 6773 203d 205b 2766  > cli_args = ['f
+00006630: 696e 642d 6f64 6473 272c 2027 3127 2c20  ind-odds', '1', 
+00006640: 2732 272c 2027 3327 2c20 2734 272c 2027  '2', '3', '4', '
+00006650: 3527 5d0a 2020 2020 2020 2020 2020 2020  5'].            
+00006660: 3e3e 3e20 7961 7078 2e72 756e 2870 7269  >>> yapx.run(pri
+00006670: 6e74 5f6e 756d 732c 205b 6669 6e64 5f65  nt_nums, [find_e
+00006680: 7665 6e73 2c20 6669 6e64 5f6f 6464 735d  vens, find_odds]
+00006690: 2c20 6172 6773 3d63 6c69 5f61 7267 7329  , args=cli_args)
+000066a0: 0a20 2020 2020 2020 2020 2020 2041 7267  .            Arg
+000066b0: 733a 2020 3120 3220 3320 3420 350a 2020  s:  1 2 3 4 5.  
+000066c0: 2020 2020 2020 2020 2020 5b27 3127 2c20            ['1', 
+000066d0: 2733 272c 2027 3527 5d0a 2020 2020 2020  '3', '5'].      
+000066e0: 2020 4e72 1700 0000 2905 725c 0000 0072    Nr....).r\...r
+000066f0: 9e00 0000 7291 0000 0072 1b01 0000 7250  ....r....r....rP
+00006700: 0000 0029 0672 5c00 0000 729e 0000 0072  ...).r\...r....r
+00006710: 9100 0000 7250 0000 0072 1b01 0000 721c  ....rP...r....r.
+00006720: 0100 0029 1072 2a01 0000 7281 0000 00da  ...).r*...r.....
+00006730: 0461 7267 7672 0201 0000 72fb 0000 0072  .argvr....r....r
+00006740: ac00 0000 7242 0000 0072 4300 0000 7244  ....rB...rC...rD
+00006750: 0000 0072 4500 0000 7246 0000 0072 2601  ...rE...rF...r&.
+00006760: 0000 7238 0000 0072 0a00 0000 da04 6e65  ..r8...r......ne
+00006770: 7874 da0d 5374 6f70 4974 6572 6174 696f  xt..StopIteratio
+00006780: 6e29 1172 a900 0000 7250 0000 0072 2b01  n).r....rP...r+.
+00006790: 0000 722c 0100 0072 2d01 0000 725c 0000  ..r,...r-...r\..
+000067a0: 005a 0a6b 6e6f 776e 5f61 7267 7372 8800  .Z.known_argsr..
+000067b0: 0000 7207 0100 005a 0972 6f6f 745f 6675  ..r....Z.root_fu
+000067c0: 6e63 5a14 726f 6f74 5f66 756e 635f 6172  ncZ.root_func_ar
+000067d0: 6773 5f6d 6f64 656c 5a0c 636f 6d6d 616e  gs_modelZ.comman
+000067e0: 645f 6e61 6d65 5a0c 636f 6d6d 616e 645f  d_nameZ.command_
+000067f0: 6675 6e63 5a17 636f 6d6d 616e 645f 6675  funcZ.command_fu
+00006800: 6e63 5f61 7267 735f 6d6f 6465 6c72 1c01  nc_args_modelr..
+00006810: 0000 5a0b 726f 6f74 5f72 6573 756c 745a  ..Z.root_resultZ
+00006820: 0a67 656e 5f72 6573 756c 7472 5800 0000  .gen_resultrX...
+00006830: 7258 0000 0072 5900 0000 da04 5f72 756e  rX...rY....._run
+00006840: c304 0000 737a 0000 0010 2308 020e 0108  ....sz....#.....
+00006850: 0204 010e 0308 0104 0204 0104 ff04 0304  ................
+00006860: 0104 ff0c 0304 0104 0104 ff04 0304 0104  ................
+00006870: ff04 0404 0104 0204 0102 0102 0102 0102  ................
+00006880: 0102 0106 fb0a 0802 010c 010c 0108 0102  ................
+00006890: ff04 0302 0208 0104 0102 0102 0102 0102  ................
+000068a0: 0102 0102 0106 fa02 800a 0908 0104 0104  ................
+000068b0: 0102 8004 020a fb08 0104 0104 0102 8002  ................
+000068c0: fd02 017a 1341 7267 756d 656e 7450 6172  ...z.ArgumentPar
+000068d0: 7365 722e 5f72 756e 2902 4e46 7256 0000  ser._run).NFrV..
+000068e0: 0029 0246 4629 024e 4e29 034e 4e46 2903  .).FF).NN).NNF).
+000068f0: 4e4e 4e29 3a72 9700 0000 da0a 5f5f 6d6f  NNN):r......__mo
+00006900: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00006910: 6d65 5f5f 7242 0000 0072 7100 0000 72a4  me__rB...rq...r.
+00006920: 0000 0072 4300 0000 7244 0000 0072 4500  ...rC...rD...rE.
+00006930: 0000 7246 0000 0072 2d00 0000 720c 0000  ..rF...r-...r...
+00006940: 0072 1000 0000 720f 0000 0072 1300 0000  .r....r....r....
+00006950: 726c 0000 0072 8400 0000 720b 0000 0072  rl...r....r....r
+00006960: d900 0000 728c 0000 0072 1500 0000 720d  ....r....r....r.
+00006970: 0000 0072 2900 0000 7293 0000 0072 7800  ...r)...r....rx.
+00006980: 0000 7241 0000 0072 9d00 0000 72a0 0000  ..rA...r....r...
+00006990: 00da 0c73 7461 7469 636d 6574 686f 6472  ...staticmethodr
+000069a0: a600 0000 da0b 636c 6173 736d 6574 686f  ......classmetho
+000069b0: 6472 2200 0000 7292 0000 0072 ca00 0000  dr"...r....r....
+000069c0: 7212 0000 0072 d000 0000 72cc 0000 0072  r....r....r....r
+000069d0: cb00 0000 7298 0000 0072 f500 0000 728e  ....r....r....r.
+000069e0: 0000 0072 7600 0000 7228 0000 0072 fc00  ...rv...r(...r..
+000069f0: 0000 7211 0000 0072 fe00 0000 7202 0100  ..r....r....r...
+00006a00: 0072 0901 0000 720a 0100 0072 0601 0000  .r....r....r....
+00006a10: 720e 0000 0072 1001 0000 729a 0000 0072  r....r....r....r
+00006a20: 1a01 0000 7226 0100 0072 2a01 0000 7231  ....r&...r*...r1
+00006a30: 0100 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
+00006a40: 5f5f 7258 0000 0072 5800 0000 727b 0000  __rX...rX...r{..
+00006a50: 0072 5900 0000 7241 0000 004c 0000 0073  .rY...rA...L...s
+00006a60: d601 0000 0a00 0c01 0c01 0c01 0c01 0c01  ................
+00006a70: 0205 0201 0201 0201 0201 0201 0201 0201  ................
+00006a80: 0201 06f5 0202 02fe 0603 02fd 0604 02fc  ................
+00006a90: 0605 02fb 0a06 02fa 0a07 02f9 0a08 02f8  ................
+00006aa0: 0a09 02f7 060a 02f6 060b 02f5 020c 0ef4  ................
+00006ab0: 007f 0e04 0206 0201 04fd 0a02 02fe 0203  ................
+00006ac0: 02fd 0204 0efc 022e 1602 02fe 0203 0afd  ................
+00006ad0: 0234 04fd 1602 02fe 0603 02fd 0204 02fc  .4..............
+00006ae0: 0405 0afb 0263 04fd 0a02 02fe 0603 02fd  .....c..........
+00006af0: 0204 02fc 0205 0afb 020e 1c01 0203 0201  ................
+00006b00: 0402 02fe 1603 02fd 0604 0cfc 007f 007f  ................
+00006b10: 0228 2001 0203 2401 0203 2401 0203 0204  .( ...$...$.....
+00006b20: 0201 04fc 0602 02fe 0203 02fd 0204 02fc  ................
+00006b30: 0605 0cfb 143f 1412 100a 020b 0402 02fe  .....?..........
+00006b40: 0203 0afd 0232 0201 04fd 0a02 02fe 0803  .....2..........
+00006b50: 02fd 0204 0efc 0210 0201 04fd 0a02 02fe  ................
+00006b60: 0803 02fd 0e04 0efc 020f 0201 0201 04fc  ................
+00006b70: 0a02 02fe 0a03 02fd 0204 02fc 0e05 0afb  ................
+00006b80: 0230 0201 0201 04fc 0a02 02fe 0a03 02fd  .0..............
+00006b90: 0204 02fc 0205 0afb 0228 0201 04fc 0402  .........(......
+00006ba0: 02fe 0a03 02fd 0204 02fc 0205 0afb 0221  ...............!
+00006bb0: 0201 0a01 02ff 0602 02fe 0a03 0cfd 0206  ................
+00006bc0: 0201 1602 02fe 0603 0cfd 0219 0201 0402  ................
+00006bd0: 02fe 1603 02fd 0204 0cfc 020a 0206 0201  ................
+00006be0: 0201 04f9 0202 02fe 0a03 02fd 0604 02fc  ................
+00006bf0: 0a05 02fb 0e06 02fa 0607 02f9 0208 0cf8  ................
+00006c00: 0263 0203 0201 0201 04fc 0e02 02fe 1203  .c..............
+00006c10: 02fd 1604 02fc 0205 02fb 0206 0cfa 022e  ................
+00006c20: 0204 0201 06fc 0202 02fe 0a03 02fd 0a04  ................
+00006c30: 02fc 0205 02fb 0206 14fa 7241 0000 0029  ..........rA...)
+00006c40: 4e72 7800 0000 da0f 636f 6c6c 6563 7469  Nrx.....collecti
+00006c50: 6f6e 732e 6162 6372 d100 0000 7281 0000  ons.abcr....r...
+00006c60: 0072 0200 0000 da0a 636f 6e74 6578 746c  .r......contextl
+00006c70: 6962 7203 0000 00da 0b64 6174 6163 6c61  ibr......datacla
+00006c80: 7373 6573 7204 0000 0072 0500 0000 7206  ssesr....r....r.
+00006c90: 0000 00da 0465 6e75 6d72 0700 0000 da09  .....enumr......
+00006ca0: 6675 6e63 746f 6f6c 7372 0800 0000 da07  functoolsr......
+00006cb0: 696e 7370 6563 7472 0900 0000 da05 7479  inspectr......ty
+00006cc0: 7065 7372 0a00 0000 da06 7479 7069 6e67  pesr......typing
+00006cd0: 720b 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+00006ce0: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
+00006cf0: 0000 0072 1200 0000 7213 0000 0072 1400  ...r....r....r..
+00006d00: 0000 7215 0000 005a 0d70 6b67 5f72 6573  ..r....Z.pkg_res
+00006d10: 6f75 7263 6573 7216 0000 00da 0761 6374  ourcesr......act
+00006d20: 696f 6e73 7218 0000 0072 1900 0000 721a  ionsr....r....r.
+00006d30: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
+00006d40: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+00006d50: 00da 0361 7267 7221 0000 0072 2200 0000  ...argr!...r"...
+00006d60: 7223 0000 0072 2400 0000 7225 0000 00da  r#...r$...r%....
+00006d70: 0a65 7863 6570 7469 6f6e 7372 2600 0000  .exceptionsr&...
+00006d80: 7227 0000 0072 c200 0000 7228 0000 0072  r'...r....r(...r
+00006d90: 2900 0000 722a 0000 0072 2b00 0000 da05  )...r*...r+.....
+00006da0: 7574 696c 7372 2c00 0000 722d 0000 0072  utilsr,...r-...r
+00006db0: 2e00 0000 722f 0000 0072 3000 0000 7231  ....r/...r0...r1
+00006dc0: 0000 0072 3200 0000 7233 0000 0072 3400  ...r2...r3...r4.
+00006dd0: 0000 7235 0000 0072 3600 0000 7237 0000  ..r5...r6...r7..
+00006de0: 0072 3800 0000 7239 0000 0072 c900 0000  .r8...r9...r....
+00006df0: 723c 0000 005a 1174 7970 696e 675f 6578  r<...Z.typing_ex
+00006e00: 7465 6e73 696f 6e73 723f 0000 0072 4000  tensionsr?...r@.
+00006e10: 0000 7241 0000 0072 5800 0000 7258 0000  ..rA...rX...rX..
+00006e20: 0072 5800 0000 7259 0000 00da 083c 6d6f  .rX...rY.....<mo
+00006e30: 6475 6c65 3e01 0000 0073 3200 0000 0800  dule>....s2.....
+00006e40: 0801 0801 0c01 0c01 1401 0c01 0c01 0c01  ................
+00006e50: 0c01 3401 0c0e 2c02 1c0b 1007 0c01 1401  ..4...,.........
+00006e60: 4001 0a11 0e01 0c02 0a02 0c01 0802 1603  @...............
```

### Comparing `yapx-0.2.3/src/yapx/__pycache__/exceptions.cpython-310.pyc` & `yapx-0.2.4/src/yapx/__pycache__/exceptions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 23:58:26 2023 UTC, .py size: 633 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2256 c464 7902 0000  o......."V.dy...
+00000000: 6f0d 0d0a 0000 0000 8a84 c564 7902 0000  o..........dy...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 4700  m.Z.m.Z.m.Z...G.
 00000050: 6403 6404 8400 6404 6506 8303 5a07 4700  d.d...d.e...Z.G.
 00000060: 6405 6406 8400 6406 6501 8303 5a08 0907  d.d...d.e...Z...
 00000070: 640c 6408 6505 6503 1900 6409 6504 6506  d.d.e.e...d.e.e.
```

### Comparing `yapx-0.2.3/src/yapx/__pycache__/namespace.cpython-310.pyc` & `yapx-0.2.4/src/yapx/__pycache__/namespace.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 23:58:26 2023 UTC, .py size: 304 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2256 c464 3001 0000  o......."V.d0...
+00000000: 6f0d 0d0a 0000 0000 8a84 c564 3001 0000  o..........d0...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 6d01 5a02 0100 6400 6402 6c03  d.l.m.Z...d.d.l.
 00000040: 6d04 5a04 6d05 5a05 0100 4700 6403 6404  m.Z.m.Z...G.d.d.
 00000050: 8400 6404 6502 8303 5a01 6405 5300 2906  ..d.e...Z.d.S.).
 00000060: e900 0000 0029 01da 094e 616d 6573 7061  .....)...Namespa
 00000070: 6365 2902 da03 416e 79da 0444 6963 7463  ce)...Any..Dictc
```

### Comparing `yapx-0.2.3/src/yapx/__pycache__/types.cpython-310.pyc` & `yapx-0.2.4/src/yapx/__pycache__/types.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 23:58:26 2023 UTC, .py size: 1300 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2256 c464 1405 0000  o......."V.d....
+00000000: 6f0d 0d0a 0000 0000 8a84 c564 1405 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 e600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6500 6a0a 6404 6b05 7226 6400 6405  ..e.j.d.k.r&d.d.
 00000070: 6c03 6d0b 5a0b 0100 6e06 6400 6405 6c0c  l.m.Z...n.d.d.l.
```

### Comparing `yapx-0.2.3/src/yapx/__pycache__/utils.cpython-310.pyc` & `yapx-0.2.4/src/yapx/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 23:58:26 2023 UTC, .py size: 4211 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2256 c464 7310 0000  o......."V.ds...
+00000000: 6f0d 0d0a 0000 0000 8a84 c564 7310 0000  o..........ds...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 2803 0000 5500  .....@...s(...U.
 00000030: 6400 6401 6c00 5a00 6400 6402 6c01 6d02  d.d.l.Z.d.d.l.m.
 00000040: 5a02 0100 6400 6403 6c03 6d04 5a04 0100  Z...d.d.l.m.Z...
 00000050: 6400 6404 6c05 6d06 5a06 0100 6400 6405  d.d.l.m.Z...d.d.
 00000060: 6c07 6d08 5a08 0100 6400 6406 6c09 6d0a  l.m.Z...d.d.l.m.
 00000070: 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e  Z.m.Z.m.Z.m.Z.m.
```

### Comparing `yapx-0.2.3/src/yapx/actions.py` & `yapx-0.2.4/src/yapx/actions.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.3/src/yapx/arg.py` & `yapx-0.2.4/src/yapx/arg.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.3/src/yapx/argument_parser.py` & `yapx-0.2.4/src/yapx/argument_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,53 +87,92 @@
         prog_version: Optional[str] = None,
         description: Optional[str] = None,
         help_flags: Optional[List[str]] = None,
         version_flags: Optional[List[str]] = None,
         tui_flags: Optional[List[str]] = None,
         completion_flags: Optional[List[str]] = None,
         formatter_class: Type[Any] = RawTextHelpFormatter,
-        _is_subparser: bool = False,
+        _parent_parser: Optional["ArgumentParser"] = None,
         **kwargs: Any,
     ):
+        if _parent_parser:
+            description = None
+            formatter_class = _parent_parser.formatter_class
+            if help_flags is None:
+                help_flags = _parent_parser._help_flags
+            if tui_flags is None:
+                tui_flags = _parent_parser._tui_flags
+
         super().__init__(
             *args,
             prog=prog,
-            description=None if _is_subparser else description,
             add_help=False,
+            description=description,
             formatter_class=formatter_class,
             **kwargs,
         )
 
+        self._help_flags = help_flags
+        self._tui_flags = tui_flags
+
         self._subparsers_action: Optional[argparse._SubParsersAction] = None
 
         # self._positionals.title = "commands"
         self._optionals.title = "helpful parameters"
 
         if help_flags is None:
             help_flags = ["-h", "--help"]
 
         if help_flags:
             if isinstance(help_flags, str):
                 help_flags = [help_flags]
             self.add_argument(
-                *[x for x in help_flags if x],
+                *help_flags,
                 action=HelpAction,
                 help="Show this help message.",
             )
 
         self.kv_separator = "="
 
         self._mutually_exclusive_args: Dict[
             Optional[Callable[..., Any]],
             Dict[str, List[Tuple[str, Optional[str]]]],
         ] = defaultdict(lambda: defaultdict(list))
 
         self._dest_type: Dict[str, Union[type, Callable[[str], Any]]] = {}
 
-        if not _is_subparser:
+        if is_tui_available:
+            if tui_flags is None:
+                tui_flags = ["--tui"]
+            elif isinstance(tui_flags, str):
+                tui_flags = [tui_flags]
+
+            tui_help: str = "Show Textual User Interface (TUI)."
+
+            if len(tui_flags) == 1 and not tui_flags[0].startswith("-"):
+                if not _parent_parser:
+                    self._get_or_add_subparsers()
+                    add_tui_command(
+                        parser=self,
+                        command=tui_flags[0],
+                        help=tui_help,
+                    )
+            else:
+                tui_flags = [
+                    (x if x.startswith("-") else f"--{x}" if len(x) > 1 else f"-{x}")
+                    for x in tui_flags
+                ]
+                add_tui_argument(
+                    parser=self,
+                    parent_parser=_parent_parser,
+                    option_strings=tui_flags,
+                    help=tui_help,
+                )
+
+        if not _parent_parser:
             if help_flags:
                 help_all_flags = [f"{x}-all" for x in help_flags if x.startswith("--")]
                 self.add_argument(
                     *help_all_flags,
                     action=HelpAllAction,
                     help="Show help for all commands.",
                 )
@@ -168,35 +207,14 @@
                     *completion_flags,
                     action=completion_action(),
                     default=argparse.SUPPRESS,
                     choices=SUPPORTED_SHELLS,
                     help="Print shell completion script.",
                 )
 
-            if tui_flags is None:
-                tui_flags = ["--tui"]
-
-            if tui_flags and is_tui_available:
-                if isinstance(tui_flags, str):
-                    tui_flags = [tui_flags]
-
-                if len(tui_flags) == 1 and not tui_flags[0].startswith("-"):
-                    self._get_or_add_subparsers()
-                    add_tui_command(
-                        parser=self,
-                        option_strings=tui_flags[0],
-                        help="Show Textual User Interface (TUI).",
-                    )
-                else:
-                    add_tui_argument(
-                        parser=self,
-                        option_strings=tui_flags,
-                        help="Show Textual User Interface (TUI).",
-                    )
-
     def error(self, message: str):
         self.print_usage(sys.stderr)
         self.exit(2, f"error: {message}\n")
 
     def print_help(
         self,
         file: Optional[IO[str]] = None,
@@ -774,24 +792,25 @@
             and not is_pydantic_available
         ):
             raise_unsupported_type_error(type_container_subtype_origin)
 
         return type_container_subtype
 
     def add_subparsers(self, **kwargs) -> argparse._SubParsersAction:
-        kwargs["title"] = kwargs.get("title", "commands")
-        kwargs["metavar"] = kwargs.get("metavar", "<COMMAND>")
-        kwargs["dest"] = kwargs.get("dest", self.CMD_ATTR_NAME)
+        default_kwargs: Dict[str, Any] = {
+            "title": "commands",
+            "metavar": "<COMMAND>",
+            "dest": self.CMD_ATTR_NAME,
+        }
+        for k, v in default_kwargs.items():
+            kwargs[k] = kwargs.get(k, v)
+
         kwargs["parser_class"] = kwargs.get(
             "parser_class",
-            lambda **k: type(self)(
-                **k,
-                _is_subparser=True,
-                formatter_class=self.formatter_class,
-            ),
+            lambda **k: type(self)(**k, _parent_parser=self),
         )
 
         self._subparsers_action = super().add_subparsers(**kwargs)
 
         return self._subparsers_action
 
     def _find_subparsers_action(self) -> Optional[argparse._SubParsersAction]:
```

### Comparing `yapx-0.2.3/src/yapx/exceptions.py` & `yapx-0.2.4/src/yapx/exceptions.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.3/src/yapx/types.py` & `yapx-0.2.4/src/yapx/types.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.3/src/yapx/utils.py` & `yapx-0.2.4/src/yapx/utils.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.3/src/yapx.egg-info/PKG-INFO` & `yapx-0.2.4/src/yapx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yapx
-Version: 0.2.3
+Version: 0.2.4
 Summary: The next generation of Python's Argparse.
 Author-email: Donald Mellenbruch <hello@f2dv.com>
 License: Copyright 2023 Donald Mellenbruch
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `yapx-0.2.3/src/yapx.egg-info/SOURCES.txt` & `yapx-0.2.4/src/yapx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yapx-0.2.3/src/yapx.egg-info/requires.txt` & `yapx-0.2.4/src/yapx.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 mkdocs-autorefs==0.*
 mkdocs-include-dir-to-nav==1.*
 
 [extras]
 pydantic<3,>=1.10.3
 shtab==1.6.2
 rich-argparse==1.*
-argparse-tui<1,>=0.1.2
+argparse-tui<1,>=0.2.0
 
 [pydantic]
 pydantic<3,>=1.10.3
 
 [rich]
 rich-argparse==1.*
 
@@ -49,8 +49,8 @@
 pylint-pytest==1.*
 packaging==23.*
 pydantic<3,>=1.10.3
 shtab==1.6.*
 rich-argparse==1.*
 
 [tui]
-argparse-tui<1,>=0.1.2
+argparse-tui<1,>=0.2.0
```

### Comparing `yapx-0.2.3/tests/test_actions.py` & `yapx-0.2.4/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.3/tests/test_add_arguments.py` & `yapx-0.2.4/tests/test_add_arguments.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.3/tests/test_add_arguments_future.py` & `yapx-0.2.4/tests/test_add_arguments_future.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.3/tests/test_add_command.py` & `yapx-0.2.4/tests/test_add_command.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.3/tests/test_arg.py` & `yapx-0.2.4/tests/test_arg.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.3/tests/test_run.py` & `yapx-0.2.4/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.3/tests/test_utils.py` & `yapx-0.2.4/tests/test_utils.py`

 * *Files identical despite different names*

