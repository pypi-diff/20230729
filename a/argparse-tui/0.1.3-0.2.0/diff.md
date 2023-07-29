# Comparing `tmp/argparse-tui-0.1.3.tar.gz` & `tmp/argparse-tui-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argparse-tui-0.1.3.tar", last modified: Fri Jul 28 04:41:11 2023, max compression
+gzip compressed data, was "argparse-tui-0.2.0.tar", last modified: Sat Jul 29 21:22:21 2023, max compression
```

## Comparing `argparse-tui-0.1.3.tar` & `argparse-tui-0.2.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:41:11.491588 argparse-tui-0.1.3/
--rw-r--r--   0 root         (0) root         (0)     1058 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6475 2023-07-28 04:41:11.491588 argparse-tui-0.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4815 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/README.md
--rw-r--r--   0 root         (0) root         (0)     4710 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 04:41:11.491588 argparse-tui-0.1.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:41:11.475588 argparse-tui-0.1.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:41:11.479588 argparse-tui-0.1.3/src/argparse_tui/
--rw-r--r--   0 root         (0) root         (0)      208 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:41:11.483588 argparse-tui-0.1.3/src/argparse_tui/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      325 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-28 04:40:50.000000 argparse-tui-0.1.3/src/argparse_tui/__pycache__/__version__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     7696 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/__pycache__/argparse.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      312 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     1303 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/__pycache__/detect_run_string.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     7012 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/__pycache__/run_command.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     4197 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/__pycache__/schemas.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)    11857 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/__pycache__/tui.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 04:40:50.000000 argparse-tui-0.1.3/src/argparse_tui/__version__.py
--rw-r--r--   0 root         (0) root         (0)    11067 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/argparse.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/constants.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/detect_run_string.py
--rw-r--r--   0 root         (0) root         (0)    10938 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/run_command.py
--rw-r--r--   0 root         (0) root         (0)     3736 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/schemas.py
--rw-r--r--   0 root         (0) root         (0)    12871 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/tui.py
--rw-r--r--   0 root         (0) root         (0)     3859 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/tui.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:41:11.487588 argparse-tui-0.1.3/src/argparse_tui/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:41:11.487588 argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     3449 2023-07-28 04:38:02.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/about.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     4146 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/command_info.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     2573 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/command_tree.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     6957 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/form.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     3854 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/multiple_choice.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)    11469 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/parameter_controls.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     2647 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/about.py
--rw-r--r--   0 root         (0) root         (0)     4010 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/command_info.py
--rw-r--r--   0 root         (0) root         (0)     2246 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/command_tree.py
--rw-r--r--   0 root         (0) root         (0)     8067 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/form.py
--rw-r--r--   0 root         (0) root         (0)     2857 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/multiple_choice.py
--rw-r--r--   0 root         (0) root         (0)    16529 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/parameter_controls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:41:11.483588 argparse-tui-0.1.3/src/argparse_tui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6475 2023-07-28 04:41:11.000000 argparse-tui-0.1.3/src/argparse_tui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1724 2023-07-28 04:41:11.000000 argparse-tui-0.1.3/src/argparse_tui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 04:41:11.000000 argparse-tui-0.1.3/src/argparse_tui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      556 2023-07-28 04:41:11.000000 argparse-tui-0.1.3/src/argparse_tui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 04:41:11.000000 argparse-tui-0.1.3/src/argparse_tui.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:41:11.491588 argparse-tui-0.1.3/tests/
--rw-r--r--   0 root         (0) root         (0)     1611 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/tests/test_help_argparse.py
--rw-r--r--   0 root         (0) root         (0)     3897 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/tests/test_run_command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 21:22:21.375348 argparse-tui-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6475 2023-07-29 21:22:21.375348 argparse-tui-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4815 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     4710 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 21:22:21.375348 argparse-tui-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 21:22:21.363348 argparse-tui-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 21:22:21.367348 argparse-tui-0.2.0/src/argparse_tui/
+-rw-r--r--   0 root         (0) root         (0)      208 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/src/argparse_tui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 21:22:21.371348 argparse-tui-0.2.0/src/argparse_tui/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      325 2023-07-29 21:18:51.000000 argparse-tui-0.2.0/src/argparse_tui/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-29 21:22:00.000000 argparse-tui-0.2.0/src/argparse_tui/__pycache__/__version__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     8659 2023-07-29 21:18:51.000000 argparse-tui-0.2.0/src/argparse_tui/__pycache__/argparse.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      312 2023-07-29 21:18:51.000000 argparse-tui-0.2.0/src/argparse_tui/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-07-29 21:18:51.000000 argparse-tui-0.2.0/src/argparse_tui/__pycache__/detect_run_string.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     7012 2023-07-29 21:18:51.000000 argparse-tui-0.2.0/src/argparse_tui/__pycache__/run_command.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     4272 2023-07-29 21:18:51.000000 argparse-tui-0.2.0/src/argparse_tui/__pycache__/schemas.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)    11856 2023-07-29 21:18:51.000000 argparse-tui-0.2.0/src/argparse_tui/__pycache__/tui.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-29 21:22:00.000000 argparse-tui-0.2.0/src/argparse_tui/__version__.py
+-rw-r--r--   0 root         (0) root         (0)    12703 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/src/argparse_tui/argparse.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/src/argparse_tui/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/src/argparse_tui/detect_run_string.py
+-rw-r--r--   0 root         (0) root         (0)    10938 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/src/argparse_tui/run_command.py
+-rw-r--r--   0 root         (0) root         (0)     3988 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/src/argparse_tui/schemas.py
+-rw-r--r--   0 root         (0) root         (0)    12889 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/src/argparse_tui/tui.py
+-rw-r--r--   0 root         (0) root         (0)     3859 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/src/argparse_tui/tui.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 21:22:21.371348 argparse-tui-0.2.0/src/argparse_tui/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/src/argparse_tui/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 21:22:21.371348 argparse-tui-0.2.0/src/argparse_tui/widgets/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-29 21:18:51.000000 argparse-tui-0.2.0/src/argparse_tui/widgets/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-07-29 21:18:52.000000 argparse-tui-0.2.0/src/argparse_tui/widgets/__pycache__/about.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     4146 2023-07-29 21:18:51.000000 argparse-tui-0.2.0/src/argparse_tui/widgets/__pycache__/command_info.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     2573 2023-07-29 21:18:51.000000 argparse-tui-0.2.0/src/argparse_tui/widgets/__pycache__/command_tree.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     6957 2023-07-29 21:18:51.000000 argparse-tui-0.2.0/src/argparse_tui/widgets/__pycache__/form.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     3854 2023-07-29 21:18:51.000000 argparse-tui-0.2.0/src/argparse_tui/widgets/__pycache__/multiple_choice.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)    11469 2023-07-29 21:18:51.000000 argparse-tui-0.2.0/src/argparse_tui/widgets/__pycache__/parameter_controls.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     2647 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/src/argparse_tui/widgets/about.py
+-rw-r--r--   0 root         (0) root         (0)     4010 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/src/argparse_tui/widgets/command_info.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/src/argparse_tui/widgets/command_tree.py
+-rw-r--r--   0 root         (0) root         (0)     8067 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/src/argparse_tui/widgets/form.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/src/argparse_tui/widgets/multiple_choice.py
+-rw-r--r--   0 root         (0) root         (0)    16525 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/src/argparse_tui/widgets/parameter_controls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 21:22:21.367348 argparse-tui-0.2.0/src/argparse_tui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6475 2023-07-29 21:22:21.000000 argparse-tui-0.2.0/src/argparse_tui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1724 2023-07-29 21:22:21.000000 argparse-tui-0.2.0/src/argparse_tui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 21:22:21.000000 argparse-tui-0.2.0/src/argparse_tui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      556 2023-07-29 21:22:21.000000 argparse-tui-0.2.0/src/argparse_tui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-29 21:22:21.000000 argparse-tui-0.2.0/src/argparse_tui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 21:22:21.375348 argparse-tui-0.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/tests/test_help_argparse.py
+-rw-r--r--   0 root         (0) root         (0)     3897 2023-07-29 21:18:07.000000 argparse-tui-0.2.0/tests/test_run_command.py
```

### Comparing `argparse-tui-0.1.3/LICENSE` & `argparse-tui-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.3/PKG-INFO` & `argparse-tui-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argparse-tui
-Version: 0.1.3
+Version: 0.2.0
 Summary: Display your Python argparse parser as a TUI.
 Author-email: Donald Mellenbruch <hello@f2dv.com>
 License: Copyright 2023 Donald Mellenbruch
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `argparse-tui-0.1.3/README.md` & `argparse-tui-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.3/pyproject.toml` & `argparse-tui-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.3/src/argparse_tui/__pycache__/argparse.cpython-310.pyc` & `argparse-tui-0.2.0/src/argparse_tui/__pycache__/argparse.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 04:37:17 2023 UTC, .py size: 11067 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,481 +1,542 @@
-00000000: 6f0d 0d0a 0000 0000 fd45 c364 3b2b 0000  o........E.d;+..
+00000000: 6f0d 0d0a 0000 0000 0f82 c564 9f31 0000  o..........d.1..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0173 b000 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0173 cc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6403 6c04  Z.d.d.l.Z.d.d.l.
-00000050: 6d05 5a05 0100 6404 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
-00000060: 0100 6404 6406 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
-00000070: 6d0b 5a0b 6d0c 5a0c 0100 6404 6407 6c0d  m.Z.m.Z...d.d.l.
-00000080: 6d0e 5a0e 0100 0902 6425 6426 640e 640f  m.Z.....d%d&d.d.
-00000090: 8405 5a0f 0902 0902 6427 6428 6413 6414  ..Z.....d'd(d.d.
-000000a0: 8405 5a10 4700 6415 6416 8400 6416 6502  ..Z.G.d.d...d.e.
-000000b0: 6a11 8303 5a12 6402 6417 6502 6a13 6603  j...Z.d.d.e.j.f.
-000000c0: 6429 641d 641e 8405 5a14 6507 6417 6602  d)d.d...Z.e.d.f.
-000000d0: 642a 6423 6424 8405 5a15 6402 5300 292b  d*d#d$..Z.d.S.)+
-000000e0: e900 0000 0029 01da 0b61 6e6e 6f74 6174  .....)...annotat
-000000f0: 696f 6e73 4e29 01da 0341 6e79 e901 0000  ionsN)...Any....
-00000100: 0029 01da 1444 4546 4155 4c54 5f43 4f4d  .)...DEFAULT_COM
-00000110: 4d41 4e44 5f4e 414d 4529 04da 0e41 7267  MAND_NAME)...Arg
-00000120: 756d 656e 7453 6368 656d 61da 0b43 6f6d  umentSchema..Com
-00000130: 6d61 6e64 4e61 6d65 da0d 436f 6d6d 616e  mandName..Comman
-00000140: 6453 6368 656d 61da 0c4f 7074 696f 6e53  dSchema..OptionS
-00000150: 6368 656d 6129 01da 0354 7569 da06 7061  chema)...Tui..pa
-00000160: 7273 6572 fa17 6172 6770 6172 7365 2e41  rser..argparse.A
-00000170: 7267 756d 656e 7450 6172 7365 72da 0e63  rgumentParser..c
-00000180: 6d64 5f69 676e 6f72 656c 6973 74fa 246c  md_ignorelist.$l
-00000190: 6973 745b 6172 6770 6172 7365 2e41 7267  ist[argparse.Arg
-000001a0: 756d 656e 7450 6172 7365 725d 207c 204e  umentParser] | N
-000001b0: 6f6e 65da 0672 6574 7572 6efa 2064 6963  one..return. dic
-000001c0: 745b 436f 6d6d 616e 644e 616d 652c 2043  t[CommandName, C
-000001d0: 6f6d 6d61 6e64 5363 6865 6d61 5d63 0200  ommandSchema]c..
-000001e0: 0000 0000 0000 0000 0000 0400 0000 0500  ................
-000001f0: 0000 0300 0001 7332 0000 0009 0064 0a64  ......s2.....d.d
-00000200: 0b87 0087 0166 0264 0764 0884 0d89 0169  .....f.d.d.....i
-00000210: 007d 0274 0064 0983 017d 0388 017c 037c  .}.t.d...}...|.|
-00000220: 0083 027c 027c 033c 007c 0253 0029 0c4e  ...|.|.<.|.S.).N
-00000230: da08 636d 645f 6e61 6d65 7207 0000 0072  ..cmd_namer....r
-00000240: 0b00 0000 720c 0000 0072 0f00 0000 7208  ....r....r....r.
-00000250: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
-00000260: 1900 0000 1200 0000 1300 0001 7328 0300  ............s(..
-00000270: 0074 007c 007c 016a 0167 0067 0069 007c  .t.|.|.j.g.g.i.|
-00000280: 0264 018d 067d 0374 027c 0164 0264 0083  .d...}.t.|.d.d..
-00000290: 037d 047c 016a 0344 0090 015d 7c7d 0574  .}.|.j.D...]|}.t
-000002a0: 047c 0574 0583 0273 2574 066a 077c 056a  .|.t...s%t.j.|.j
-000002b0: 087c 056a 0966 0276 0072 2671 1474 047c  .|.j.f.v.r&q.t.|
-000002c0: 0574 066a 0a83 0272 517c 056a 0ba0 0ca1  .t.j...rQ|.j....
-000002d0: 0044 005d 1e5c 027d 067d 077c 076a 0174  .D.].\.}.}.|.j.t
-000002e0: 066a 076b 0372 4f88 0372 417c 0788 0376  .j.k.rO..rA|...v
-000002f0: 0172 4f88 0474 0d7c 0683 017c 077c 0364  .rO..t.|...|.|.d
-00000300: 038d 037c 036a 0e74 0d7c 0683 013c 0071  ...|.j.t.|...<.q
-00000310: 3171 1464 007d 087c 0472 5d7c 04a0 0f7c  1q.d.}.|.r]|...|
-00000320: 056a 107c 056a 11a1 027d 087c 0864 0075  .j.|.j...}.|.d.u
-00000330: 0072 6b7c 056a 0964 0075 0172 6b74 117c  .rk|.j.d.u.rkt.|
-00000340: 056a 0983 017d 0864 047d 0964 047d 0a64  .j...}.d.}.d.}.d
-00000350: 047d 0b7c 056a 1289 0067 0089 0174 047c  .}.|.j...g...t.|
-00000360: 0574 066a 1383 0272 7f64 057d 096e 5574  .t.j...r.d.}.nUt
-00000370: 047c 0574 066a 1483 0272 8864 057d 0a6e  .|.t.j...r.d.}.n
-00000380: 4c74 047c 0574 066a 1583 0272 9164 057d  Lt.|.t.j...r.d.}
-00000390: 0b6e 4374 166a 1764 066b 0572 9c74 047c  .nCt.j.d.k.r.t.|
-000003a0: 0574 066a 1883 0273 a374 117c 0583 016a  .t.j...s.t.|...j
-000003b0: 1964 076b 0272 d47c 0864 0075 0072 a974  .d.k.r.|.d.u.r.t
-000003c0: 1a7d 0864 057d 0b74 1b7c 0564 0883 0272  .}.d.}.t.|.d...r
-000003d0: be7c 056a 1c89 0187 0166 0164 0964 0a84  .|.j.....f.d.d..
-000003e0: 087c 056a 1244 0083 0189 006e 1664 0b89  .|.j.D.....n.d..
-000003f0: 0287 0266 0164 0c64 0a84 087c 056a 1244  ...f.d.d...|.j.D
-00000400: 0083 0189 0087 0066 0164 0d64 0a84 087c  .......f.d.d...|
-00000410: 056a 1244 0083 0189 0164 047d 0c64 047d  .j.D.....d.}.d.}
-00000420: 0d7c 056a 087d 0e7c 0e90 0172 2a7c 0ea0  .|.j.}.|...r*|..
-00000430: 1d64 0e74 1e7c 056a 0983 01a1 027d 0e64  .d.t.|.j.....}.d
-00000440: 0f7d 0f64 107d 107c 0ea0 1f7c 0fa1 017d  .}.d.}.|...|...}
-00000450: 117c 1164 116b 0590 0172 2a7c 0ea0 1f7c  .|.d.k...r*|...|
-00000460: 10a1 017d 127c 127c 116b 0490 0172 2a7c  ...}.|.|.k...r*|
-00000470: 0e7c 117c 1264 1217 0085 0219 007d 1364  .|.|.d.......}.d
-00000480: 1364 0a84 007c 1364 1264 1485 0219 00a0  .d...|.d.d......
-00000490: 2064 15a1 0144 0083 017d 1464 167c 1476   d...D...}.d.|.v
-000004a0: 007d 0c64 177c 1476 007d 0d74 217c 0c7c  .}.d.|.v.}.t!|.|
-000004b0: 0d67 0283 0190 0172 2a7c 0ea0 1d7c 1364  .g.....r*|...|.d
-000004c0: 18a1 027d 0e7c 056a 2264 1976 0090 0172  ...}.|.j"d.v...r
-000004d0: 3264 126e 107c 056a 2264 1a64 1b74 066a  2d.n.|.j"d.d.t.j
-000004e0: 2366 0376 0090 0172 3e64 146e 0474 247c  #f.v...r>d.n.t$|
-000004f0: 056a 2283 017d 157c 1564 116b 0090 0170  .j"..}.|.d.k...p
-00000500: 4b7c 1564 126b 047d 167c 056a 1290 0172  K|.d.k.}.|.j...r
-00000510: 7274 2588 007c 087c 0b7c 0988 017c 056a  rt%..|.|.|...|.j
-00000520: 267c 056a 097c 0e7c 056a 0b7c 0a7c 167c  &|.j.|.|.j.|.|.|
-00000530: 157c 0c7c 0d7c 0d90 0172 6764 1c6e 0164  .|.|.|...rgd.n.d
-00000540: 1864 1d8d 0f7d 177c 036a 27a0 287c 17a1  .d...}.|.j'.(|..
-00000550: 0101 0071 1474 297c 056a 107c 087c 056a  ...q.t)|.j.|.|.j
-00000560: 267c 056a 097c 0e7c 056a 0b7c 0a7c 167c  &|.j.|.|.j.|.|.|
-00000570: 157c 0c7c 0d7c 0d90 0172 8764 1c6e 0164  .|.|.|...r.d.n.d
-00000580: 1864 1e8d 0c7d 187c 036a 2aa0 287c 18a1  .d...}.|.j*.(|..
-00000590: 0101 0071 147c 0353 0029 1f4e 2906 da04  ...q.|.S.).N)...
-000005a0: 6e61 6d65 da09 646f 6373 7472 696e 67da  name..docstring.
-000005b0: 076f 7074 696f 6e73 da09 6172 6775 6d65  .options..argume
-000005c0: 6e74 73da 0b73 7562 636f 6d6d 616e 6473  nts..subcommands
-000005d0: da06 7061 7265 6e74 5a0a 5f64 6573 745f  ..parentZ._dest_
-000005e0: 7479 7065 2901 7217 0000 0046 5429 02e9  type).r....FT)..
-000005f0: 0300 0000 e909 0000 00da 1542 6f6f 6c65  ...........Boole
-00000600: 616e 4f70 7469 6f6e 616c 4163 7469 6f6e  anOptionalAction
-00000610: da18 5f6e 6567 6174 696f 6e5f 6f70 7469  .._negation_opti
-00000620: 6f6e 5f73 7472 696e 6773 6301 0000 0000  on_stringsc.....
-00000630: 0000 0000 0000 0002 0000 0004 0000 0013  ................
-00000640: 0000 01f3 1800 0000 6700 7c00 5d08 7d01  ........g.|.].}.
-00000650: 7c01 8800 7601 7202 7c01 9102 7102 5300  |...v.r.|...q.S.
-00000660: a900 721d 0000 00a9 02da 022e 30da 0178  ..r.........0..x
-00000670: 2901 da0e 7365 636f 6e64 6172 795f 6f70  )...secondary_op
-00000680: 7473 721d 0000 00fa 272f 6472 6f6e 652f  tsr.....'/drone/
-00000690: 7372 632f 7372 632f 6172 6770 6172 7365  src/src/argparse
-000006a0: 5f74 7569 2f61 7267 7061 7273 652e 7079  _tui/argparse.py
-000006b0: da0a 3c6c 6973 7463 6f6d 703e 5700 0000  ..<listcomp>W...
-000006c0: f302 0000 0018 007a 4769 6e74 726f 7370  .......zGintrosp
-000006d0: 6563 745f 6172 6770 6172 7365 5f70 6172  ect_argparse_par
-000006e0: 7365 722e 3c6c 6f63 616c 733e 2e70 726f  ser.<locals>.pro
-000006f0: 6365 7373 5f63 6f6d 6d61 6e64 2e3c 6c6f  cess_command.<lo
-00000700: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00000710: 7a05 2d2d 6e6f 2d63 0100 0000 0000 0000  z.--no-c........
-00000720: 0000 0000 0200 0000 0500 0000 1300 0001  ................
-00000730: 731a 0000 0067 007c 005d 097d 017c 01a0  s....g.|.].}.|..
-00000740: 0088 00a1 0173 027c 0191 0271 0253 0072  .....s.|...q.S.r
-00000750: 1d00 0000 2901 da0a 7374 6172 7473 7769  ....)...startswi
-00000760: 7468 721e 0000 0029 01da 1073 6563 6f6e  thr....)...secon
-00000770: 6461 7279 5f70 7265 6669 7872 1d00 0000  dary_prefixr....
-00000780: 7222 0000 0072 2300 0000 5a00 0000 730c  r"...r#...Z...s.
-00000790: 0000 0006 0002 0208 0102 fd02 0106 ff63  ...............c
-000007a0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000007b0: 0400 0000 1300 0001 721c 0000 0072 1d00  ........r....r..
-000007c0: 0000 721d 0000 0072 1e00 0000 2901 da04  ..r....r....)...
-000007d0: 6f70 7473 721d 0000 0072 2200 0000 7223  optsr....r"...r#
-000007e0: 0000 005f 0000 0072 2400 0000 7a0b 2528  ..._...r$...z.%(
-000007f0: 6465 6661 756c 7429 73fa 013c fa01 3e72  default)s..<..>r
-00000800: 0100 0000 7204 0000 0063 0100 0000 0000  ....r....c......
-00000810: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-00000820: 0001 7314 0000 0067 007c 005d 067d 017c  ..s....g.|.].}.|
-00000830: 01a0 00a1 0091 0271 0253 0072 1d00 0000  .......q.S.r....
-00000840: 2901 da05 7374 7269 7072 1e00 0000 721d  )...stripr....r.
-00000850: 0000 0072 1d00 0000 7222 0000 0072 2300  ...r....r"...r#.
-00000860: 0000 7000 0000 7302 0000 0014 00e9 ffff  ..p...s.........
-00000870: ffff fa01 2cda 0673 6563 7265 74da 0670  ....,..secret..p
-00000880: 726f 6d70 74da 0029 024e fa01 3ffa 012b  rompt..).N..?..+
-00000890: da01 2a7a 193c 2059 6f75 2077 696c 6c20  ..*z.< You will 
-000008a0: 6265 2070 726f 6d70 7465 642e 203e 290f  be prompted. >).
-000008b0: 7212 0000 00da 0474 7970 65da 0769 735f  r......type..is_
-000008c0: 666c 6167 5a08 636f 756e 7469 6e67 7221  flagZ.countingr!
-000008d0: 0000 00da 0872 6571 7569 7265 64da 0764  .....required..d
-000008e0: 6566 6175 6c74 da04 6865 6c70 da07 6368  efault..help..ch
-000008f0: 6f69 6365 73da 086d 756c 7469 706c 65da  oices..multiple.
-00000900: 0b6d 756c 7469 5f76 616c 7565 da05 6e61  .multi_value..na
-00000910: 7267 7372 2d00 0000 da09 7265 6164 5f6f  rgsr-.....read_o
-00000920: 6e6c 79da 0b70 6c61 6365 686f 6c64 6572  nly..placeholder
-00000930: 290c 7212 0000 0072 3300 0000 7235 0000  ).r....r3...r5..
-00000940: 0072 3600 0000 7237 0000 0072 3800 0000  .r6...r7...r8...
-00000950: 7239 0000 0072 3a00 0000 723b 0000 0072  r9...r:...r;...r
-00000960: 2d00 0000 723c 0000 0072 3d00 0000 292b  -...r<...r=...)+
-00000970: 7208 0000 00da 0b64 6573 6372 6970 7469  r......descripti
-00000980: 6f6e da07 6765 7461 7474 72da 085f 6163  on..getattr.._ac
-00000990: 7469 6f6e 73da 0a69 7369 6e73 7461 6e63  tions..isinstanc
-000009a0: 65da 0954 7569 4163 7469 6f6e da08 6172  e..TuiAction..ar
-000009b0: 6770 6172 7365 da08 5355 5050 5245 5353  gparse..SUPPRESS
-000009c0: 7237 0000 0072 3600 0000 da11 5f53 7562  r7...r6....._Sub
-000009d0: 5061 7273 6572 7341 6374 696f 6e72 3800  ParsersActionr8.
-000009e0: 0000 da05 6974 656d 7372 0700 0000 7216  ....itemsr....r.
-000009f0: 0000 00da 0367 6574 da04 6465 7374 7233  .....get..destr3
-00000a00: 0000 00da 0e6f 7074 696f 6e5f 7374 7269  .....option_stri
-00000a10: 6e67 73da 0c5f 436f 756e 7441 6374 696f  ngs.._CountActio
-00000a20: 6eda 0d5f 4170 7065 6e64 4163 7469 6f6e  n.._AppendAction
-00000a30: da11 5f53 746f 7265 436f 6e73 7441 6374  .._StoreConstAct
-00000a40: 696f 6eda 0373 7973 da0c 7665 7273 696f  ion..sys..versio
-00000a50: 6e5f 696e 666f 721a 0000 00da 085f 5f6e  n_infor......__n
-00000a60: 616d 655f 5fda 0462 6f6f 6cda 0768 6173  ame__..bool..has
-00000a70: 6174 7472 721b 0000 00da 0772 6570 6c61  attrr......repla
-00000a80: 6365 da03 7374 72da 0466 696e 64da 0573  ce..str..find..s
-00000a90: 706c 6974 da03 616e 7972 3b00 0000 da09  plit..anyr;.....
-00000aa0: 5245 4d41 494e 4445 52da 0369 6e74 7209  REMAINDER..intr.
-00000ab0: 0000 0072 3500 0000 7214 0000 00da 0661  ...r5...r......a
-00000ac0: 7070 656e 6472 0600 0000 7215 0000 0029  ppendr....r....)
-00000ad0: 1972 1100 0000 720b 0000 0072 1700 0000  .r....r....r....
-00000ae0: 5a08 636d 645f 6461 7461 5a0b 7061 7261  Z.cmd_dataZ.para
-00000af0: 6d5f 7479 7065 73da 0570 6172 616d 5a0e  m_types..paramZ.
-00000b00: 7375 6270 6172 7365 725f 6e61 6d65 5a09  subparser_nameZ.
-00000b10: 7375 6270 6172 7365 725a 0a70 6172 616d  subparserZ.param
-00000b20: 5f74 7970 655a 0b69 735f 636f 756e 7469  _typeZ.is_counti
-00000b30: 6e67 5a0b 6973 5f6d 756c 7469 706c 6572  ngZ.is_multipler
-00000b40: 3400 0000 5a09 6973 5f73 6563 7265 745a  4...Z.is_secretZ
-00000b50: 0969 735f 7072 6f6d 7074 5a0a 7061 7261  .is_promptZ.para
-00000b60: 6d5f 6865 6c70 5a0a 7461 675f 7072 6566  m_helpZ.tag_pref
-00000b70: 6978 5a0a 7461 675f 7375 6666 6978 5a09  ixZ.tag_suffixZ.
-00000b80: 7461 675f 7374 6172 745a 0774 6167 5f65  tag_startZ.tag_e
-00000b90: 6e64 5a07 7461 675f 7478 74da 0474 6167  ndZ.tag_txt..tag
-00000ba0: 7372 3b00 0000 723a 0000 005a 0b6f 7074  sr;...r:...Z.opt
-00000bb0: 696f 6e5f 6461 7461 5a0d 6172 6775 6d65  ion_dataZ.argume
-00000bc0: 6e74 5f64 6174 61a9 0272 0d00 0000 da0f  nt_data..r......
-00000bd0: 7072 6f63 6573 735f 636f 6d6d 616e 6429  process_command)
-00000be0: 0372 2700 0000 7221 0000 0072 2600 0000  .r'...r!...r&...
-00000bf0: 7222 0000 0072 5d00 0000 1000 0000 73f2  r"...r].......s.
-00000c00: 0000 0002 0502 0104 0102 0102 0102 0102  ................
-00000c10: 0106 fa0c 0a0c 020e 0104 0104 0106 fe02  ................
-00000c20: 040c 0212 010c 0102 0102 ff08 0102 0406  ................
-00000c30: 0102 0102 0104 fd04 fe06 0102 ff02 8002  ................
-00000c40: 0704 0204 0110 0112 020a 0104 0204 0104  ................
-00000c50: 0106 0204 010c 0206 010c 0106 010c 0106  ................
-00000c60: 010a 020a 0102 ff0e 0208 0304 0104 010a  ................
-00000c70: 0206 0216 0104 020a 0104 0206 fe14 0504  ................
-00000c80: 0404 0106 0106 0112 0104 0204 010a 010a  ................
-00000c90: 010a 010a 0110 011c 0108 0108 010e 010c  ................
-00000ca0: 010c 0404 ff14 0304 ff08 0202 fb12 0708  ................
-00000cb0: 0202 0102 0102 0102 0102 0102 0104 0104  ................
-00000cc0: 0102 0104 0102 0102 0102 0102 0102 010c  ................
-00000cd0: 0106 f10e 1102 0304 0102 0104 0104 0102  ................
-00000ce0: 0104 0102 0102 0102 0102 0102 010c 0106  ................
-00000cf0: f40e 0e04 027a 3369 6e74 726f 7370 6563  .....z3introspec
-00000d00: 745f 6172 6770 6172 7365 5f70 6172 7365  t_argparse_parse
-00000d10: 722e 3c6c 6f63 616c 733e 2e70 726f 6365  r.<locals>.proce
-00000d20: 7373 5f63 6f6d 6d61 6e64 da04 726f 6f74  ss_command..root
-00000d30: a901 4e29 0672 1100 0000 7207 0000 0072  ..N).r....r....r
-00000d40: 0b00 0000 720c 0000 0072 0f00 0000 7208  ....r....r....r.
-00000d50: 0000 0029 0172 0700 0000 2904 720b 0000  ...).r....).r...
-00000d60: 0072 0d00 0000 da04 6461 7461 5a0d 726f  .r......dataZ.ro
-00000d70: 6f74 5f63 6d64 5f6e 616d 6572 1d00 0000  ot_cmd_namer....
-00000d80: 725c 0000 0072 2200 0000 da1a 696e 7472  r\...r".....intr
-00000d90: 6f73 7065 6374 5f61 7267 7061 7273 655f  ospect_argparse_
-00000da0: 7061 7273 6572 0c00 0000 730e 0000 0002  parser....s.....
-00000db0: 0712 fd00 7f04 1708 020e 0104 0272 6100  .............ra.
-00000dc0: 0000 fa1d 6c69 7374 5b61 7267 7061 7273  ....list[argpars
-00000dd0: 652e 4172 6775 6d65 6e74 5061 7273 6572  e.ArgumentParser
-00000de0: 5dda 0e63 6f6d 6d61 6e64 5f66 696c 7465  ]..command_filte
-00000df0: 72fa 0a73 7472 207c 204e 6f6e 6563 0300  r..str | Nonec..
-00000e00: 0000 0000 0000 0000 0000 0300 0000 0500  ................
-00000e10: 0000 4300 0001 732e 0000 007c 0164 0175  ..C...s....|.d.u
-00000e20: 0072 077c 0067 017d 0174 0074 017c 007c  .r.|.g.}.t.t.|.|
-00000e30: 0164 028d 027c 006a 027c 0264 038d 03a0  .d...|.j.|.d....
-00000e40: 03a1 0001 0064 0153 0029 0461 1801 0000  .....d.S.).a....
-00000e50: 0a20 2020 2045 7861 6d70 6c65 733a 0a20  .    Examples:. 
-00000e60: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
-00000e70: 7420 6172 6770 6172 7365 0a20 2020 2020  t argparse.     
-00000e80: 2020 203e 3e3e 2066 726f 6d20 6172 6770     >>> from argp
-00000e90: 6172 7365 5f74 7569 2069 6d70 6f72 7420  arse_tui import 
-00000ea0: 696e 766f 6b65 5f74 7569 0a20 2020 2020  invoke_tui.     
-00000eb0: 2020 202e 2e2e 0a20 2020 2020 2020 203e     ....        >
-00000ec0: 3e3e 2070 6172 7365 7220 3d20 6172 6770  >> parser = argp
-00000ed0: 6172 7365 2e41 7267 756d 656e 7450 6172  arse.ArgumentPar
-00000ee0: 7365 7228 7072 6f67 3d22 6177 6573 6f6d  ser(prog="awesom
-00000ef0: 652d 6170 7022 290a 2020 2020 2020 2020  e-app").        
-00000f00: 3e3e 3e20 5f20 3d20 7061 7273 6572 2e61  >>> _ = parser.a
-00000f10: 6464 5f61 7267 756d 656e 7428 222d 2d76  dd_argument("--v
-00000f20: 616c 7565 2229 0a20 2020 2020 2020 202e  alue").        .
-00000f30: 2e2e 0a20 2020 2020 2020 203e 3e3e 2069  ...        >>> i
-00000f40: 6e76 6f6b 655f 7475 6928 7061 7273 6572  nvoke_tui(parser
-00000f50: 2920 2023 2064 6f63 7465 7374 3a20 2b53  )  # doctest: +S
-00000f60: 4b49 500a 2020 2020 4e29 0172 0d00 0000  KIP.    N).r....
-00000f70: 2902 5a08 6170 705f 6e61 6d65 7263 0000  ).Z.app_namerc..
-00000f80: 0029 0472 0a00 0000 7261 0000 00da 0470  .).r....ra.....p
-00000f90: 726f 67da 0372 756e 2903 720b 0000 0072  rog..run).r....r
-00000fa0: 0d00 0000 7263 0000 0072 1d00 0000 721d  ....rc...r....r.
-00000fb0: 0000 0072 2200 0000 da0a 696e 766f 6b65  ...r".....invoke
-00000fc0: 5f74 7569 ae00 0000 7310 0000 0008 1006  _tui....s.......
-00000fd0: 0102 020a 0104 0102 0104 fd0a 0472 6700  .............rg.
-00000fe0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000ff0: 0000 0006 0000 0000 0000 0173 3e00 0000  ...........s>...
-00001000: 6500 5a01 6400 5a02 6401 5a03 6504 6a05  e.Z.d.Z.d.Z.e.j.
-00001010: 6504 6a05 6402 6403 6403 6403 6606 6415  e.j.d.d.d.d.f.d.
-00001020: 8700 6601 6411 6412 840d 5a06 6416 6413  ..f.d.d...Z.d.d.
-00001030: 6414 8401 5a07 8700 0400 5a08 5300 2917  d...Z.....Z.S.).
-00001040: 7242 0000 0061 7501 0000 6172 6770 6172  rB...au...argpar
-00001050: 7365 2060 4163 7469 6f6e 6020 7468 6174  se `Action` that
-00001060: 2077 696c 6c20 616e 616c 797a 6520 7468   will analyze th
-00001070: 6520 7061 7273 6572 2061 6e64 2064 6973  e parser and dis
-00001080: 706c 6179 2061 2054 5549 2e0a 0a20 2020  play a TUI...   
-00001090: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
-000010a0: 2020 203e 3e3e 2069 6d70 6f72 7420 6172     >>> import ar
-000010b0: 6770 6172 7365 0a20 2020 2020 2020 203e  gparse.        >
-000010c0: 3e3e 2066 726f 6d20 6172 6770 6172 7365  >> from argparse
-000010d0: 5f74 7569 2069 6d70 6f72 7420 5475 6941  _tui import TuiA
-000010e0: 6374 696f 6e0a 2020 2020 2020 2020 2e2e  ction.        ..
-000010f0: 2e0a 2020 2020 2020 2020 3e3e 3e20 7061  ..        >>> pa
-00001100: 7273 6572 203d 2061 7267 7061 7273 652e  rser = argparse.
-00001110: 4172 6775 6d65 6e74 5061 7273 6572 2829  ArgumentParser()
-00001120: 0a20 2020 2020 2020 203e 3e3e 205f 203d  .        >>> _ =
-00001130: 2070 6172 7365 722e 6164 645f 6172 6775   parser.add_argu
-00001140: 6d65 6e74 2827 2d2d 7475 6927 2c20 6163  ment('--tui', ac
-00001150: 7469 6f6e 3d54 7569 4163 7469 6f6e 290a  tion=TuiAction).
-00001160: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
-00001170: 2020 2020 3e3e 3e20 7061 7273 6572 2e70      >>> parser.p
-00001180: 7269 6e74 5f75 7361 6765 2829 0a20 2020  rint_usage().   
-00001190: 2020 2020 2075 7361 6765 3a20 5f5f 6d61       usage: __ma
-000011a0: 696e 5f5f 2e70 7920 5b2d 685d 205b 2d2d  in__.py [-h] [--
-000011b0: 7475 6920 5b54 5549 5d5d 0a20 2020 20fa  tui [TUI]].    .
-000011c0: 104f 7065 6e20 5465 7874 7561 6c20 5549  .Open Textual UI
-000011d0: 2e4e 7249 0000 00fa 096c 6973 745b 7374  .NrI.....list[st
-000011e0: 725d 7248 0000 0072 5300 0000 7236 0000  r]rH...rS...r6..
-000011f0: 0072 0300 0000 7237 0000 0072 6400 0000  .r....r7...rd...
-00001200: da05 636f 6e73 74da 076d 6574 6176 6172  ..const..metavar
-00001210: 723b 0000 00fa 1069 6e74 207c 2073 7472  r;.....int | str
-00001220: 207c 204e 6f6e 65da 075f 6b77 6172 6773   | None.._kwargs
-00001230: 6308 0000 0000 0000 0000 0000 0009 0000  c...............
-00001240: 0009 0000 000b 0000 0173 2e00 0000 7400  .........s....t.
-00001250: 7401 7c00 8302 6a02 7c01 7c02 7c03 7c07  t.|...j.|.|.|.|.
-00001260: 6400 7500 720e 6401 6e01 7c07 7c04 7c05  d.u.r.d.n.|.|.|.
-00001270: 7c06 6402 8d07 0100 6400 5300 2903 4e72  |.d.....d.S.).Nr
-00001280: 3000 0000 2907 7249 0000 0072 4800 0000  0...).rI...rH...
-00001290: 7236 0000 0072 3b00 0000 7237 0000 0072  r6...r;...r7...r
-000012a0: 6a00 0000 726b 0000 0029 03da 0573 7570  j...rk...)...sup
-000012b0: 6572 7242 0000 00da 085f 5f69 6e69 745f  errB.....__init_
-000012c0: 5f29 09da 0473 656c 6672 4900 0000 7248  _)...selfrI...rH
-000012d0: 0000 0072 3600 0000 7237 0000 0072 6a00  ...r6...r7...rj.
-000012e0: 0000 726b 0000 0072 3b00 0000 726d 0000  ..rk...r;...rm..
-000012f0: 00a9 01da 095f 5f63 6c61 7373 5f5f 721d  .....__class__r.
-00001300: 0000 0072 2200 0000 726f 0000 00d6 0000  ...r"...ro......
-00001310: 0073 1200 0000 0a0b 0201 0201 0201 0e01  .s..............
-00001320: 0201 0201 0201 0af9 7a12 5475 6941 6374  ........z.TuiAct
-00001330: 696f 6e2e 5f5f 696e 6974 5f5f 6305 0000  ion.__init__c...
-00001340: 0000 0000 0000 0000 0006 0000 0005 0000  ................
-00001350: 0043 0000 0173 2800 0000 7400 7c02 6401  .C...s(...t.|.d.
-00001360: 7c01 8303 7d05 7401 7c05 7c01 6701 7c03  |...}.t.|.|.g.|.
-00001370: 6402 8d03 0100 7c01 a002 a100 0100 6400  d.....|.......d.
-00001380: 5300 2903 4eda 0e5f 7061 7265 6e74 5f70  S.).N.._parent_p
-00001390: 6172 7365 7229 0272 0d00 0000 7263 0000  arser).r....rc..
-000013a0: 0029 0372 3f00 0000 7267 0000 00da 0465  .).r?...rg.....e
-000013b0: 7869 7429 0672 7000 0000 720b 0000 00da  xit).rp...r.....
-000013c0: 096e 616d 6573 7061 6365 da06 7661 6c75  .namespace..valu
-000013d0: 6573 da0d 6f70 7469 6f6e 5f73 7472 696e  es..option_strin
-000013e0: 675a 0b72 6f6f 745f 7061 7273 6572 721d  gZ.root_parserr.
-000013f0: 0000 0072 1d00 0000 7222 0000 00da 085f  ...r....r"....._
-00001400: 5f63 616c 6c5f 5feb 0000 0073 0e00 0000  _call__....s....
-00001410: 0201 0201 0201 0201 04fd 1006 0c02 7a12  ..............z.
-00001420: 5475 6941 6374 696f 6e2e 5f5f 6361 6c6c  TuiAction.__call
-00001430: 5f5f 2910 7249 0000 0072 6900 0000 7248  __).rI...ri...rH
-00001440: 0000 0072 5300 0000 7236 0000 0072 0300  ...rS...r6...r..
-00001450: 0000 7237 0000 0072 6400 0000 726a 0000  ..r7...rd...rj..
-00001460: 0072 5300 0000 726b 0000 0072 5300 0000  .rS...rk...rS...
-00001470: 723b 0000 0072 6c00 0000 726d 0000 0072  r;...rl...rm...r
-00001480: 0300 0000 725f 0000 0029 0972 4f00 0000  ....r_...).rO...
-00001490: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-000014a0: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
-000014b0: 635f 5f72 4300 0000 7244 0000 0072 6f00  c__rC...rD...ro.
-000014c0: 0000 7278 0000 00da 0d5f 5f63 6c61 7373  ..rx.....__class
-000014d0: 6365 6c6c 5f5f 721d 0000 0072 1d00 0000  cell__r....r....
-000014e0: 7271 0000 0072 2200 0000 7242 0000 00c8  rq...r"...rB....
-000014f0: 0000 0073 1400 0000 0800 0401 0410 0401  ...s............
-00001500: 0201 0201 0201 0201 10f8 1215 7242 0000  ............rB..
-00001510: 0072 6800 0000 7249 0000 00fa 0f73 7472  .rh...rI.....str
-00001520: 207c 206c 6973 745b 7374 725d 7237 0000   | list[str]r7..
-00001530: 0072 5300 0000 da04 4e6f 6e65 6304 0000  .rS.....Nonec...
-00001540: 0000 0000 0000 0000 0005 0000 0007 0000  ................
-00001550: 004b 0000 0173 4e00 0000 7c01 7310 6401  .K...sN...|.s.d.
-00001560: 7400 a001 6402 6403 a102 a002 6403 a101  t...d.d.....d...
-00001570: 9b00 9d02 6701 7d01 6e08 7403 7c01 7404  ....g.}.n.t.|.t.
-00001580: 8302 7218 7c01 6701 7d01 7c00 6a05 7c01  ..r.|.g.}.|.j.|.
-00001590: 6404 7406 7c03 7c02 6405 9c04 7c04 a401  d.t.|.|.d...|...
-000015a0: 8e01 0100 6406 5300 2907 61dd 0100 000a  ....d.S.).a.....
-000015b0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-000015c0: 2020 2070 6172 7365 723a 2074 6865 2061     parser: the a
-000015d0: 7267 7061 7273 6520 7061 7273 6572 0a20  rgparse parser. 
-000015e0: 2020 2020 2020 206f 7074 696f 6e5f 7374         option_st
-000015f0: 7269 6e67 733a 206c 6973 7420 6f66 2043  rings: list of C
-00001600: 4c49 2066 6c61 6773 2074 6861 7420 7769  LI flags that wi
-00001610: 6c6c 2069 6e76 6f6b 6520 7468 6520 5455  ll invoke the TU
-00001620: 4920 2864 6566 6175 6c74 3d60 2d2d 7475  I (default=`--tu
-00001630: 6960 290a 2020 2020 2020 2020 6865 6c70  i`).        help
-00001640: 3a20 6865 6c70 206d 6573 7361 6765 2066  : help message f
-00001650: 6f72 2074 6865 2061 7267 756d 656e 740a  or the argument.
-00001660: 0a20 2020 2045 7861 6d70 6c65 733a 0a20  .    Examples:. 
-00001670: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
-00001680: 7420 6172 6770 6172 7365 0a20 2020 2020  t argparse.     
-00001690: 2020 203e 3e3e 2066 726f 6d20 6172 6770     >>> from argp
-000016a0: 6172 7365 5f74 7569 2069 6d70 6f72 7420  arse_tui import 
-000016b0: 6164 645f 7475 695f 6172 6775 6d65 6e74  add_tui_argument
-000016c0: 0a20 2020 2020 2020 202e 2e2e 0a20 2020  .        ....   
-000016d0: 2020 2020 203e 3e3e 2070 6172 7365 7220       >>> parser 
-000016e0: 3d20 6172 6770 6172 7365 2e41 7267 756d  = argparse.Argum
-000016f0: 656e 7450 6172 7365 7228 290a 2020 2020  entParser().    
-00001700: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
-00001710: 3e3e 3e20 6164 645f 7475 695f 6172 6775  >>> add_tui_argu
-00001720: 6d65 6e74 2870 6172 7365 7229 0a20 2020  ment(parser).   
-00001730: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
-00001740: 203e 3e3e 2070 6172 7365 722e 7072 696e   >>> parser.prin
-00001750: 745f 7573 6167 6528 290a 2020 2020 2020  t_usage().      
-00001760: 2020 7573 6167 653a 205f 5f6d 6169 6e5f    usage: __main_
-00001770: 5f2e 7079 205b 2d68 5d20 5b2d 2d74 7569  _.py [-h] [--tui
-00001780: 205b 434d 445d 5d0a 2020 2020 7a02 2d2d   [CMD]].    z.--
-00001790: da01 5fda 012d 5a03 434d 4429 0472 6b00  .._..-Z.CMD).rk.
-000017a0: 0000 da06 6163 7469 6f6e 7236 0000 0072  ....actionr6...r
-000017b0: 3700 0000 4e29 0772 0500 0000 7252 0000  7...N).r....rR..
-000017c0: 00da 066c 7374 7269 7072 4100 0000 7253  ...lstriprA...rS
-000017d0: 0000 00da 0c61 6464 5f61 7267 756d 656e  .....add_argumen
-000017e0: 7472 4200 0000 2905 720b 0000 0072 4900  trB...).r....rI.
-000017f0: 0000 7237 0000 0072 3600 0000 da06 6b77  ..r7...r6.....kw
-00001800: 6172 6773 721d 0000 0072 1d00 0000 7222  argsr....r....r"
-00001810: 0000 00da 1061 6464 5f74 7569 5f61 7267  .....add_tui_arg
-00001820: 756d 656e 74f7 0000 0073 1a00 0000 0419  ument....s......
-00001830: 1c01 0a01 0601 0402 0201 0201 0201 0201  ................
-00001840: 0201 04fb 0206 0afa 7285 0000 00da 0763  ........r......c
-00001850: 6f6d 6d61 6e64 7284 0000 0072 0300 0000  ommandr....r....
-00001860: fa1a 6172 6770 6172 7365 2e5f 5375 6250  ..argparse._SubP
-00001870: 6172 7365 7273 4163 7469 6f6e 6303 0000  arsersActionc...
-00001880: 0000 0000 0000 0000 0007 0000 0006 0000  ................
-00001890: 004b 0000 0173 7000 0000 7c00 6a00 6401  .K...sp...|.j.d.
-000018a0: 7500 720e 7c00 6a01 6407 6900 7c03 a401  u.r.|.j.d.i.|...
-000018b0: 8e01 7d04 6e10 7c00 6a02 4400 5d0c 7d05  ..}.n.|.j.D.].}.
-000018c0: 7403 7c05 7404 6a05 8302 721d 7c05 7d04  t.|.t.j...r.|.}.
-000018d0: 0100 6e01 7111 7c04 6a06 7c01 7404 6a07  ..n.q.|.j.|.t.j.
-000018e0: 7c02 6402 8d03 7d06 7c06 6a08 7c00 6403  |.d...}.|.j.|.d.
-000018f0: 8d01 0100 7409 7c06 6404 6701 6401 6405  ....t.|.d.g.d.d.
-00001900: 6406 8d04 0100 7c04 5300 2908 615a 0200  d.....|.S.).aZ..
-00001910: 000a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-00001920: 2020 2020 2070 6172 7365 723a 2074 6865       parser: the
-00001930: 2061 7267 7061 7273 6520 7061 7273 6572   argparse parser
-00001940: 0a20 2020 2020 2020 2063 6f6d 6d61 6e64  .        command
-00001950: 3a20 6e61 6d65 206f 6620 7468 6520 434c  : name of the CL
-00001960: 4920 636f 6d6d 616e 6420 7468 6174 2077  I command that w
-00001970: 696c 6c20 696e 766f 6b65 2074 6865 2054  ill invoke the T
-00001980: 5549 2028 6465 6661 756c 743d 6074 7569  UI (default=`tui
-00001990: 6029 0a20 2020 2020 2020 2068 656c 703a  `).        help:
-000019a0: 2068 656c 7020 6d65 7373 6167 6520 666f   help message fo
-000019b0: 7220 7468 6520 6172 6775 6d65 6e74 0a20  r the argument. 
-000019c0: 2020 2020 2020 202a 2a6b 7761 7267 733a         **kwargs:
-000019d0: 2069 6620 7375 6270 6172 7365 7273 2064   if subparsers d
-000019e0: 6f20 6e6f 7420 616c 7265 6164 7920 6578  o not already ex
-000019f0: 6973 742c 2063 7265 6174 6520 7769 7468  ist, create with
-00001a00: 2074 6865 7365 206b 7761 7267 732e 0a0a   these kwargs...
-00001a10: 2020 2020 4578 616d 706c 6573 3a0a 2020      Examples:.  
-00001a20: 2020 2020 2020 3e3e 3e20 696d 706f 7274        >>> import
-00001a30: 2061 7267 7061 7273 650a 2020 2020 2020   argparse.      
-00001a40: 2020 3e3e 3e20 6672 6f6d 2061 7267 7061    >>> from argpa
-00001a50: 7273 655f 7475 6920 696d 706f 7274 2061  rse_tui import a
-00001a60: 6464 5f74 7569 5f61 7267 756d 656e 740a  dd_tui_argument.
-00001a70: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
-00001a80: 2020 2020 3e3e 3e20 7061 7273 6572 203d      >>> parser =
-00001a90: 2061 7267 7061 7273 652e 4172 6775 6d65   argparse.Argume
-00001aa0: 6e74 5061 7273 6572 2829 0a20 2020 2020  ntParser().     
-00001ab0: 2020 203e 3e3e 2073 7562 7061 7273 6572     >>> subparser
-00001ac0: 7320 3d20 7061 7273 6572 2e61 6464 5f73  s = parser.add_s
-00001ad0: 7562 7061 7273 6572 7328 290a 2020 2020  ubparsers().    
-00001ae0: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
-00001af0: 3e3e 3e20 5f20 3d20 6164 645f 7475 695f  >>> _ = add_tui_
-00001b00: 636f 6d6d 616e 6428 7061 7273 6572 290a  command(parser).
-00001b10: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
-00001b20: 2020 2020 3e3e 3e20 7061 7273 6572 2e70      >>> parser.p
-00001b30: 7269 6e74 5f75 7361 6765 2829 0a20 2020  rint_usage().   
-00001b40: 2020 2020 2075 7361 6765 3a20 5f5f 6d61       usage: __ma
-00001b50: 696e 5f5f 2e70 7920 5b2d 685d 207b 7475  in__.py [-h] {tu
-00001b60: 697d 202e 2e2e 0a20 2020 204e 2902 723e  i} ....    N).r>
-00001b70: 0000 0072 3700 0000 2901 7273 0000 005a  ...r7...).rs...Z
-00001b80: 0a63 6d64 5f66 696c 7465 727a 0e43 6f6d  .cmd_filterz.Com
-00001b90: 6d61 6e64 2066 696c 7465 7229 0372 4900  mand filter).rI.
-00001ba0: 0000 7236 0000 0072 3700 0000 721d 0000  ..r6...r7...r...
-00001bb0: 0029 0ada 0b5f 7375 6270 6172 7365 7273  .)..._subparsers
-00001bc0: da0e 6164 645f 7375 6270 6172 7365 7273  ..add_subparsers
-00001bd0: 7240 0000 0072 4100 0000 7243 0000 0072  r@...rA...rC...r
-00001be0: 4500 0000 da0a 6164 645f 7061 7273 6572  E.....add_parser
-00001bf0: 7244 0000 00da 0c73 6574 5f64 6566 6175  rD.....set_defau
-00001c00: 6c74 7372 8500 0000 2907 720b 0000 0072  ltsr....).r....r
-00001c10: 8600 0000 7237 0000 0072 8400 0000 5a0a  ....r7...r....Z.
-00001c20: 7375 6270 6172 7365 7273 7281 0000 005a  subparsersr....Z
-00001c30: 0a74 7569 5f70 6172 7365 7272 1d00 0000  .tui_parserr....
-00001c40: 721d 0000 0072 2200 0000 da0f 6164 645f  r....r".....add_
-00001c50: 7475 695f 636f 6d6d 616e 641f 0100 0073  tui_command....s
-00001c60: 2800 0000 0a1c 1201 0a02 0c01 0401 0401  (...............
-00001c70: 02fe 0404 0201 0401 0201 06fd 0c05 0202  ................
-00001c80: 0201 0401 0201 0201 06fc 0407 728c 0000  ............r...
-00001c90: 0072 5f00 0000 2906 720b 0000 0072 0c00  .r_...).r....r..
-00001ca0: 0000 720d 0000 0072 0e00 0000 720f 0000  ..r....r....r...
-00001cb0: 0072 1000 0000 2902 4e4e 2906 720b 0000  .r....).NN).r...
-00001cc0: 0072 0c00 0000 720d 0000 0072 6200 0000  .r....r....rb...
-00001cd0: 7263 0000 0072 6400 0000 2908 720b 0000  rc...rd...).r...
-00001ce0: 0072 0c00 0000 7249 0000 0072 7d00 0000  .r....rI...r}...
-00001cf0: 7237 0000 0072 5300 0000 720f 0000 0072  r7...rS...r....r
-00001d00: 7e00 0000 290a 720b 0000 0072 0c00 0000  ~...).r....r....
-00001d10: 7286 0000 0072 5300 0000 7237 0000 0072  r....rS...r7...r
-00001d20: 5300 0000 7284 0000 0072 0300 0000 720f  S...r....r....r.
-00001d30: 0000 0072 8700 0000 2916 da0a 5f5f 6675  ...r....)...__fu
-00001d40: 7475 7265 5f5f 7202 0000 0072 4300 0000  ture__r....rC...
-00001d50: 724d 0000 00da 0674 7970 696e 6772 0300  rM.....typingr..
-00001d60: 0000 da09 636f 6e73 7461 6e74 7372 0500  ....constantsr..
-00001d70: 0000 5a07 7363 6865 6d61 7372 0600 0000  ..Z.schemasr....
-00001d80: 7207 0000 0072 0800 0000 7209 0000 00da  r....r....r.....
-00001d90: 0374 7569 720a 0000 0072 6100 0000 7267  .tuir....ra...rg
-00001da0: 0000 00da 0641 6374 696f 6e72 4200 0000  .....ActionrB...
-00001db0: 7244 0000 0072 8500 0000 728c 0000 0072  rD...r....r....r
-00001dc0: 1d00 0000 721d 0000 0072 1d00 0000 7222  ....r....r....r"
-00001dd0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00001de0: 0073 2a00 0000 0c00 0802 0801 0c01 0c02  .s*.............
-00001df0: 1801 0c01 0205 0cfe 007f 0225 0201 0cfd  ...........%....
-00001e00: 121a 0231 0201 0401 0cfc 022a 0201 10fd  ...1.......*....
+00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
+00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6406  ..d.d.l.m.Z...d.
+00000070: 6407 6c0a 6d0b 5a0b 0100 6406 6408 6c0c  d.l.m.Z...d.d.l.
+00000080: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  m.Z.m.Z.m.Z.m.Z.
+00000090: 0100 6406 6409 6c11 6d12 5a12 0100 0902  ..d.d.l.m.Z.....
+000000a0: 0902 642a 642b 6412 6413 8405 5a13 0902  ..d*d+d.d...Z...
+000000b0: 0902 642a 642c 6416 6417 8405 5a14 4700  ..d*d,d.d...Z.G.
+000000c0: 6418 6419 8400 6419 6502 6a15 8303 5a16  d.d...d.e.j...Z.
+000000d0: 6402 6402 641a 6502 6a17 6604 642d 6422  d.d.d.e.j.f.d-d"
+000000e0: 6423 8405 5a18 650b 641a 6602 642e 6428  d#..Z.e.d.f.d.d(
+000000f0: 6429 8405 5a19 6402 5300 292f e900 0000  d)..Z.d.S.)/....
+00000100: 0029 01da 0b61 6e6e 6f74 6174 696f 6e73  .)...annotations
+00000110: 4e29 01da 0873 7570 7072 6573 7329 01da  N)...suppress)..
+00000120: 0864 6565 7063 6f70 7929 01da 0341 6e79  .deepcopy)...Any
+00000130: e901 0000 0029 01da 1444 4546 4155 4c54  .....)...DEFAULT
+00000140: 5f43 4f4d 4d41 4e44 5f4e 414d 4529 04da  _COMMAND_NAME)..
+00000150: 0e41 7267 756d 656e 7453 6368 656d 61da  .ArgumentSchema.
+00000160: 0b43 6f6d 6d61 6e64 4e61 6d65 da0d 436f  .CommandName..Co
+00000170: 6d6d 616e 6453 6368 656d 61da 0c4f 7074  mmandSchema..Opt
+00000180: 696f 6e53 6368 656d 6129 01da 0354 7569  ionSchema)...Tui
+00000190: da06 7061 7273 6572 fa17 6172 6770 6172  ..parser..argpar
+000001a0: 7365 2e41 7267 756d 656e 7450 6172 7365  se.ArgumentParse
+000001b0: 72da 1473 7562 7061 7273 6572 5f69 676e  r..subparser_ign
+000001c0: 6f72 656c 6973 74fa 246c 6973 745b 6172  orelist.$list[ar
+000001d0: 6770 6172 7365 2e41 7267 756d 656e 7450  gparse.ArgumentP
+000001e0: 6172 7365 725d 207c 204e 6f6e 65da 0f76  arser] | None..v
+000001f0: 616c 7565 5f6f 7665 7272 6964 6573 fa15  alue_overrides..
+00000200: 6469 6374 5b73 7472 2c20 416e 795d 207c  dict[str, Any] |
+00000210: 204e 6f6e 65da 0672 6574 7572 6efa 2064   None..return. d
+00000220: 6963 745b 436f 6d6d 616e 644e 616d 652c  ict[CommandName,
+00000230: 2043 6f6d 6d61 6e64 5363 6865 6d61 5d63   CommandSchema]c
+00000240: 0300 0000 0000 0000 0000 0000 0500 0000  ................
+00000250: 0500 0000 0300 0001 7340 0000 0009 0064  ........s@.....d
+00000260: 0a64 0b87 0087 0187 0266 0364 0764 0884  .d.......f.d.d..
+00000270: 0d89 0069 007d 0374 0064 0983 017d 0488  ...i.}.t.d...}..
+00000280: 0264 0075 0072 1769 0089 0288 007c 047c  .d.u.r.i.....|.|
+00000290: 0083 027c 037c 043c 007c 0353 0029 0c4e  ...|.|.<.|.S.).N
+000002a0: da08 636d 645f 6e61 6d65 7209 0000 0072  ..cmd_namer....r
+000002b0: 0d00 0000 720e 0000 0072 1300 0000 720a  ....r....r....r.
+000002c0: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
+000002d0: 1800 0000 1100 0000 1300 0001 7312 0300  ............s...
+000002e0: 0074 007c 007c 016a 0167 0067 0069 007c  .t.|.|.j.g.g.i.|
+000002f0: 0264 018d 067d 0374 027c 0164 0264 0083  .d...}.t.|.d.d..
+00000300: 037d 047c 016a 0344 0090 015d 717d 0574  .}.|.j.D...]q}.t
+00000310: 047c 0574 0583 0273 2574 066a 077c 056a  .|.t...s%t.j.|.j
+00000320: 087c 056a 0966 0276 0072 2671 1474 047c  .|.j.f.v.r&q.t.|
+00000330: 0574 066a 0a83 0272 517c 056a 0ba0 0ca1  .t.j...rQ|.j....
+00000340: 0044 005d 1e5c 027d 067d 077c 076a 0174  .D.].\.}.}.|.j.t
+00000350: 066a 076b 0372 4f88 0472 417c 0788 0476  .j.k.rO..rA|...v
+00000360: 0172 4f88 0374 0d7c 0683 017c 077c 0364  .rO..t.|...|.|.d
+00000370: 038d 037c 036a 0e74 0d7c 0683 013c 0071  ...|.j.t.|...<.q
+00000380: 3171 1464 007d 087c 0472 5d7c 04a0 0f7c  1q.d.}.|.r]|...|
+00000390: 056a 107c 056a 11a1 027d 087c 0864 0075  .j.|.j...}.|.d.u
+000003a0: 0072 6b7c 056a 0964 0075 0172 6b74 117c  .rk|.j.d.u.rkt.|
+000003b0: 056a 0983 017d 0864 047d 0964 047d 0a64  .j...}.d.}.d.}.d
+000003c0: 047d 0b7c 056a 1289 0067 0089 0174 047c  .}.|.j...g...t.|
+000003d0: 0574 066a 1383 0272 7f64 057d 096e 5574  .t.j...r.d.}.nUt
+000003e0: 047c 0574 066a 1483 0272 8864 057d 0a6e  .|.t.j...r.d.}.n
+000003f0: 4c74 047c 0574 066a 1583 0272 9164 057d  Lt.|.t.j...r.d.}
+00000400: 0b6e 4374 166a 1764 066b 0572 9c74 047c  .nCt.j.d.k.r.t.|
+00000410: 0574 066a 1883 0273 a374 117c 0583 016a  .t.j...s.t.|...j
+00000420: 1964 076b 0272 d47c 0864 0075 0072 a974  .d.k.r.|.d.u.r.t
+00000430: 1a7d 0864 057d 0b74 1b7c 0564 0883 0272  .}.d.}.t.|.d...r
+00000440: be7c 056a 1c89 0187 0166 0164 0964 0a84  .|.j.....f.d.d..
+00000450: 087c 056a 1244 0083 0189 006e 1664 0b89  .|.j.D.....n.d..
+00000460: 0287 0266 0164 0c64 0a84 087c 056a 1244  ...f.d.d...|.j.D
+00000470: 0083 0189 0087 0066 0164 0d64 0a84 087c  .......f.d.d...|
+00000480: 056a 1244 0083 0189 0164 047d 0c7c 056a  .j.D.....d.}.|.j
+00000490: 087d 0d7c 0d90 0172 237c 0da0 1d64 0e74  .}.|...r#|...d.t
+000004a0: 1e7c 056a 0983 01a1 027d 0d64 0f7d 0e64  .|.j.....}.d.}.d
+000004b0: 107d 0f7c 0da0 1f7c 0ea1 017d 107c 1064  .}.|...|...}.|.d
+000004c0: 116b 0590 0172 237c 0da0 1f7c 0fa1 017d  .k...r#|...|...}
+000004d0: 117c 117c 106b 0490 0172 237c 0d7c 107c  .|.|.k...r#|.|.|
+000004e0: 1164 1217 0085 0219 007d 1264 1364 0a84  .d.......}.d.d..
+000004f0: 007c 1264 1264 1485 0219 00a0 2064 15a1  .|.d.d...... d..
+00000500: 0144 0083 017d 1364 167c 1376 007d 0c74  .D...}.d.|.v.}.t
+00000510: 217c 0c67 0183 0190 0172 237c 0da0 1d7c  !|.g.....r#|...|
+00000520: 1264 17a1 027d 0d7c 056a 2264 1876 0090  .d...}.|.j"d.v..
+00000530: 0172 2b64 126e 107c 056a 2264 1964 1a74  .r+d.n.|.j"d.d.t
+00000540: 066a 2366 0376 0090 0172 3764 146e 0474  .j#f.v...r7d.n.t
+00000550: 247c 056a 2283 017d 147c 1464 116b 0090  $|.j"..}.|.d.k..
+00000560: 0170 447c 1464 126b 047d 157c 056a 1290  .pD|.d.k.}.|.j..
+00000570: 0172 6974 2588 007c 087c 0b7c 0988 017c  .rit%..|.|.|...|
+00000580: 056a 267c 056a 0988 05a0 0f7c 056a 10a1  .j&|.j.....|.j..
+00000590: 017c 0d7c 056a 0b7c 0a7c 157c 147c 0c64  .|.|.j.|.|.|.|.d
+000005a0: 1b8d 0e7d 167c 036a 27a0 287c 16a1 0101  ...}.|.j'.(|....
+000005b0: 0071 1474 297c 056a 107c 087c 056a 267c  .q.t)|.j.|.|.j&|
+000005c0: 056a 0988 05a0 0f7c 056a 10a1 017c 0d7c  .j.....|.j...|.|
+000005d0: 056a 0b7c 0a7c 157c 147c 0c64 1c8d 0b7d  .j.|.|.|.|.d...}
+000005e0: 177c 036a 2aa0 287c 17a1 0101 0071 147c  .|.j*.(|.....q.|
+000005f0: 0353 0029 1d4e 2906 da04 6e61 6d65 da09  .S.).N)...name..
+00000600: 646f 6373 7472 696e 67da 076f 7074 696f  docstring..optio
+00000610: 6e73 da09 6172 6775 6d65 6e74 73da 0b73  ns..arguments..s
+00000620: 7562 636f 6d6d 616e 6473 da06 7061 7265  ubcommands..pare
+00000630: 6e74 5a0a 5f64 6573 745f 7479 7065 2901  ntZ._dest_type).
+00000640: 721b 0000 0046 5429 02e9 0300 0000 e909  r....FT)........
+00000650: 0000 00da 1542 6f6f 6c65 616e 4f70 7469  .....BooleanOpti
+00000660: 6f6e 616c 4163 7469 6f6e da18 5f6e 6567  onalAction.._neg
+00000670: 6174 696f 6e5f 6f70 7469 6f6e 5f73 7472  ation_option_str
+00000680: 696e 6773 6301 0000 0000 0000 0000 0000  ingsc...........
+00000690: 0002 0000 0004 0000 0013 0000 01f3 1800  ................
+000006a0: 0000 6700 7c00 5d08 7d01 7c01 8800 7601  ..g.|.].}.|...v.
+000006b0: 7202 7c01 9102 7102 5300 a900 7221 0000  r.|...q.S...r!..
+000006c0: 00a9 02da 022e 30da 0178 2901 da0e 7365  ......0..x)...se
+000006d0: 636f 6e64 6172 795f 6f70 7473 7221 0000  condary_optsr!..
+000006e0: 00fa 272f 6472 6f6e 652f 7372 632f 7372  ..'/drone/src/sr
+000006f0: 632f 6172 6770 6172 7365 5f74 7569 2f61  c/argparse_tui/a
+00000700: 7267 7061 7273 652e 7079 da0a 3c6c 6973  rgparse.py..<lis
+00000710: 7463 6f6d 703e 5b00 0000 f302 0000 0018  tcomp>[.........
+00000720: 007a 4769 6e74 726f 7370 6563 745f 6172  .zGintrospect_ar
+00000730: 6770 6172 7365 5f70 6172 7365 722e 3c6c  gparse_parser.<l
+00000740: 6f63 616c 733e 2e70 726f 6365 7373 5f63  ocals>.process_c
+00000750: 6f6d 6d61 6e64 2e3c 6c6f 6361 6c73 3e2e  ommand.<locals>.
+00000760: 3c6c 6973 7463 6f6d 703e 7a05 2d2d 6e6f  <listcomp>z.--no
+00000770: 2d63 0100 0000 0000 0000 0000 0000 0200  -c..............
+00000780: 0000 0500 0000 1300 0001 731a 0000 0067  ..........s....g
+00000790: 007c 005d 097d 017c 01a0 0088 00a1 0173  .|.].}.|.......s
+000007a0: 027c 0191 0271 0253 0072 2100 0000 2901  .|...q.S.r!...).
+000007b0: da0a 7374 6172 7473 7769 7468 7222 0000  ..startswithr"..
+000007c0: 0029 01da 1073 6563 6f6e 6461 7279 5f70  .)...secondary_p
+000007d0: 7265 6669 7872 2100 0000 7226 0000 0072  refixr!...r&...r
+000007e0: 2700 0000 5e00 0000 730c 0000 0006 0002  '...^...s.......
+000007f0: 0208 0102 fd02 0106 ff63 0100 0000 0000  .........c......
+00000800: 0000 0000 0000 0200 0000 0400 0000 1300  ................
+00000810: 0001 7220 0000 0072 2100 0000 7221 0000  ..r ...r!...r!..
+00000820: 0072 2200 0000 2901 da04 6f70 7473 7221  .r"...)...optsr!
+00000830: 0000 0072 2600 0000 7227 0000 0063 0000  ...r&...r'...c..
+00000840: 0072 2800 0000 7a0b 2528 6465 6661 756c  .r(...z.%(defaul
+00000850: 7429 73fa 013c fa01 3e72 0100 0000 7206  t)s..<..>r....r.
+00000860: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000870: 0200 0000 0400 0000 5300 0001 7314 0000  ........S...s...
+00000880: 0067 007c 005d 067d 017c 01a0 00a1 0091  .g.|.].}.|......
+00000890: 0271 0253 0072 2100 0000 2901 da05 7374  .q.S.r!...)...st
+000008a0: 7269 7072 2200 0000 7221 0000 0072 2100  ripr"...r!...r!.
+000008b0: 0000 7226 0000 0072 2700 0000 7300 0000  ..r&...r'...s...
+000008c0: 7302 0000 0014 00e9 ffff ffff fa01 2cda  s.............,.
+000008d0: 0673 6563 7265 74da 0029 024e fa01 3ffa  .secret..).N..?.
+000008e0: 012b da01 2a29 0e72 1600 0000 da04 7479  .+..*).r......ty
+000008f0: 7065 da07 6973 5f66 6c61 675a 0863 6f75  pe..is_flagZ.cou
+00000900: 6e74 696e 6772 2500 0000 da08 7265 7175  ntingr%.....requ
+00000910: 6972 6564 da07 6465 6661 756c 74da 0576  ired..default..v
+00000920: 616c 7565 da04 6865 6c70 da07 6368 6f69  alue..help..choi
+00000930: 6365 73da 086d 756c 7469 706c 65da 0b6d  ces..multiple..m
+00000940: 756c 7469 5f76 616c 7565 da05 6e61 7267  ulti_value..narg
+00000950: 7372 3100 0000 290b 7216 0000 0072 3600  sr1...).r....r6.
+00000960: 0000 7238 0000 0072 3900 0000 723a 0000  ..r8...r9...r:..
+00000970: 0072 3b00 0000 723c 0000 0072 3d00 0000  .r;...r<...r=...
+00000980: 723e 0000 0072 3f00 0000 7231 0000 0029  r>...r?...r1...)
+00000990: 2b72 0a00 0000 da0b 6465 7363 7269 7074  +r......descript
+000009a0: 696f 6eda 0767 6574 6174 7472 da08 5f61  ion..getattr.._a
+000009b0: 6374 696f 6e73 da0a 6973 696e 7374 616e  ctions..isinstan
+000009c0: 6365 da09 5475 6941 6374 696f 6eda 0861  ce..TuiAction..a
+000009d0: 7267 7061 7273 65da 0853 5550 5052 4553  rgparse..SUPPRES
+000009e0: 5372 3b00 0000 7239 0000 00da 115f 5375  Sr;...r9....._Su
+000009f0: 6250 6172 7365 7273 4163 7469 6f6e 723c  bParsersActionr<
+00000a00: 0000 00da 0569 7465 6d73 7209 0000 0072  .....itemsr....r
+00000a10: 1a00 0000 da03 6765 74da 0464 6573 7472  ......get..destr
+00000a20: 3600 0000 da0e 6f70 7469 6f6e 5f73 7472  6.....option_str
+00000a30: 696e 6773 da0c 5f43 6f75 6e74 4163 7469  ings.._CountActi
+00000a40: 6f6e da0d 5f41 7070 656e 6441 6374 696f  on.._AppendActio
+00000a50: 6eda 115f 5374 6f72 6543 6f6e 7374 4163  n.._StoreConstAc
+00000a60: 7469 6f6e da03 7379 73da 0c76 6572 7369  tion..sys..versi
+00000a70: 6f6e 5f69 6e66 6f72 1e00 0000 da08 5f5f  on_infor......__
+00000a80: 6e61 6d65 5f5f da04 626f 6f6c da07 6861  name__..bool..ha
+00000a90: 7361 7474 7272 1f00 0000 da07 7265 706c  sattrr......repl
+00000aa0: 6163 65da 0373 7472 da04 6669 6e64 da05  ace..str..find..
+00000ab0: 7370 6c69 74da 0361 6e79 723f 0000 00da  split..anyr?....
+00000ac0: 0952 454d 4149 4e44 4552 da03 696e 7472  .REMAINDER..intr
+00000ad0: 0b00 0000 7238 0000 0072 1800 0000 da06  ....r8...r......
+00000ae0: 6170 7065 6e64 7208 0000 0072 1900 0000  appendr....r....
+00000af0: 2918 7215 0000 0072 0d00 0000 721b 0000  ).r....r....r...
+00000b00: 005a 0863 6d64 5f64 6174 615a 0b70 6172  .Z.cmd_dataZ.par
+00000b10: 616d 5f74 7970 6573 da05 7061 7261 6d5a  am_types..paramZ
+00000b20: 0e73 7562 7061 7273 6572 5f6e 616d 65da  .subparser_name.
+00000b30: 0973 7562 7061 7273 6572 5a0a 7061 7261  .subparserZ.para
+00000b40: 6d5f 7479 7065 5a0b 6973 5f63 6f75 6e74  m_typeZ.is_count
+00000b50: 696e 675a 0b69 735f 6d75 6c74 6970 6c65  ingZ.is_multiple
+00000b60: 7237 0000 005a 0969 735f 7365 6372 6574  r7...Z.is_secret
+00000b70: 5a0a 7061 7261 6d5f 6865 6c70 5a0a 7461  Z.param_helpZ.ta
+00000b80: 675f 7072 6566 6978 5a0a 7461 675f 7375  g_prefixZ.tag_su
+00000b90: 6666 6978 5a09 7461 675f 7374 6172 745a  ffixZ.tag_startZ
+00000ba0: 0774 6167 5f65 6e64 5a07 7461 675f 7478  .tag_endZ.tag_tx
+00000bb0: 74da 0474 6167 7372 3f00 0000 723e 0000  t..tagsr?...r>..
+00000bc0: 005a 0b6f 7074 696f 6e5f 6461 7461 5a0d  .Z.option_dataZ.
+00000bd0: 6172 6775 6d65 6e74 5f64 6174 61a9 03da  argument_data...
+00000be0: 0f70 726f 6365 7373 5f63 6f6d 6d61 6e64  .process_command
+00000bf0: 720f 0000 0072 1100 0000 2903 722b 0000  r....r....).r+..
+00000c00: 0072 2500 0000 722a 0000 0072 2600 0000  .r%...r*...r&...
+00000c10: 7260 0000 0013 0000 0073 ea00 0000 0205  r`.......s......
+00000c20: 0201 0401 0201 0201 0201 0201 06fa 0c0a  ................
+00000c30: 0c02 0e01 0401 0401 06fe 0204 0c02 1201  ................
+00000c40: 0c01 0201 02ff 0802 0204 0601 0201 0201  ................
+00000c50: 04fd 04fe 0601 02ff 0280 0207 0402 0401  ................
+00000c60: 1001 1202 0a01 0402 0401 0401 0602 0401  ................
+00000c70: 0c02 0601 0c01 0601 0c01 0601 0a02 0a01  ................
+00000c80: 02ff 0e02 0803 0401 0401 0a02 0602 1601  ................
+00000c90: 0402 0a01 0402 06fe 1405 0404 0601 0601  ................
+00000ca0: 1201 0402 0401 0a01 0a01 0a01 0a01 1001  ................
+00000cb0: 1c01 0801 0c01 0c01 0c04 04ff 1403 04ff  ................
+00000cc0: 0802 02fb 1207 0802 0201 0201 0201 0201  ................
+00000cd0: 0201 0201 0401 0401 0a01 0201 0401 0201  ................
+00000ce0: 0201 0201 0201 06f2 0e10 0203 0401 0201  ................
+00000cf0: 0401 0401 0a01 0201 0401 0201 0201 0201  ................
+00000d00: 0201 06f5 0e0d 0402 7a33 696e 7472 6f73  ........z3intros
+00000d10: 7065 6374 5f61 7267 7061 7273 655f 7061  pect_argparse_pa
+00000d20: 7273 6572 2e3c 6c6f 6361 6c73 3e2e 7072  rser.<locals>.pr
+00000d30: 6f63 6573 735f 636f 6d6d 616e 64da 0472  ocess_command..r
+00000d40: 6f6f 74a9 014e 2906 7215 0000 0072 0900  oot..N).r....r..
+00000d50: 0000 720d 0000 0072 0e00 0000 7213 0000  ..r....r....r...
+00000d60: 0072 0a00 0000 2901 7209 0000 0029 0572  .r....).r....).r
+00000d70: 0d00 0000 720f 0000 0072 1100 0000 da04  ....r....r......
+00000d80: 6461 7461 5a0d 726f 6f74 5f63 6d64 5f6e  dataZ.root_cmd_n
+00000d90: 616d 6572 2100 0000 725f 0000 0072 2600  amer!...r_...r&.
+00000da0: 0000 da1a 696e 7472 6f73 7065 6374 5f61  ....introspect_a
+00000db0: 7267 7061 7273 655f 7061 7273 6572 0e00  rgparse_parser..
+00000dc0: 0000 7312 0000 0002 0814 fd00 7f04 1408  ..s.............
+00000dd0: 0208 0204 010e 0204 0272 6400 0000 da08  .........rd.....
+00000de0: 636c 695f 6172 6773 fa10 6c69 7374 5b73  cli_args..list[s
+00000df0: 7472 5d20 7c20 4e6f 6e65 6303 0000 0000  tr] | Nonec.....
+00000e00: 0000 0000 0000 000a 0000 0008 0000 0003  ................
+00000e10: 0000 0173 a800 0000 6401 7d03 6900 7d04  ...s....d.}.i.}.
+00000e20: 7c02 7241 7c02 4400 5d0b 7d05 7c05 a000  |.rA|.D.].}.|...
+00000e30: 6402 a101 7313 7c05 7d03 0100 6e01 7108  d...s.|.}...n.q.
+00000e40: 8700 6601 6403 6404 8408 8900 7401 7c00  ..f.d.d.....t.|.
+00000e50: 8301 7d06 8800 7c06 8301 0100 7402 7403  ..}...|.....t.t.
+00000e60: 8301 8f13 0100 7c06 a004 7c02 a101 5c02  ......|...|...\.
+00000e70: 7d07 7d08 7405 7c07 8301 7d04 5700 6401  }.}.t.|...}.W.d.
+00000e80: 0400 0400 8303 0100 6e08 3100 733c 7701  ........n.1.s<w.
+00000e90: 0100 0100 0100 5900 0100 7406 7c00 7c01  ......Y...t.|.|.
+00000ea0: 7c04 6405 8d03 7d09 7407 7c09 7c00 6a08  |.d...}.t.|.|.j.
+00000eb0: 7c03 6406 8d03 a009 a100 0100 6401 5300  |.d.........d.S.
+00000ec0: 2907 6118 0100 000a 2020 2020 4578 616d  ).a.....    Exam
+00000ed0: 706c 6573 3a0a 2020 2020 2020 2020 3e3e  ples:.        >>
+00000ee0: 3e20 696d 706f 7274 2061 7267 7061 7273  > import argpars
+00000ef0: 650a 2020 2020 2020 2020 3e3e 3e20 6672  e.        >>> fr
+00000f00: 6f6d 2061 7267 7061 7273 655f 7475 6920  om argparse_tui 
+00000f10: 696d 706f 7274 2069 6e76 6f6b 655f 7475  import invoke_tu
+00000f20: 690a 2020 2020 2020 2020 2e2e 2e0a 2020  i.        ....  
+00000f30: 2020 2020 2020 3e3e 3e20 7061 7273 6572        >>> parser
+00000f40: 203d 2061 7267 7061 7273 652e 4172 6775   = argparse.Argu
+00000f50: 6d65 6e74 5061 7273 6572 2870 726f 673d  mentParser(prog=
+00000f60: 2261 7765 736f 6d65 2d61 7070 2229 0a20  "awesome-app"). 
+00000f70: 2020 2020 2020 203e 3e3e 205f 203d 2070         >>> _ = p
+00000f80: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
+00000f90: 6e74 2822 2d2d 7661 6c75 6522 290a 2020  nt("--value").  
+00000fa0: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
+00000fb0: 2020 3e3e 3e20 696e 766f 6b65 5f74 7569    >>> invoke_tui
+00000fc0: 2870 6172 7365 7229 2020 2320 646f 6374  (parser)  # doct
+00000fd0: 6573 743a 202b 534b 4950 0a20 2020 204e  est: +SKIP.    N
+00000fe0: da01 2d63 0100 0000 0000 0000 0000 0000  ..-c............
+00000ff0: 0400 0000 0400 0000 1300 0001 7358 0000  ............sX..
+00001000: 007c 006a 0044 005d 057d 0164 017c 015f  .|.j.D.].}.d.|._
+00001010: 0171 037c 006a 0272 287c 006a 026a 0044  .q.|.j.r(|.j.j.D
+00001020: 005d 197d 0264 017c 025f 0174 037c 0274  .].}.d.|._.t.|.t
+00001030: 046a 0583 0272 277c 026a 06a0 07a1 0044  .j...r'|.j.....D
+00001040: 005d 067d 0388 007c 0383 0101 0071 2071  .].}...|.....q q
+00001050: 1064 0053 0064 0053 0029 024e 4629 0872  .d.S.d.S.).NF).r
+00001060: 4200 0000 7238 0000 00da 0b5f 7375 6270  B...r8....._subp
+00001070: 6172 7365 7273 7243 0000 0072 4500 0000  arsersrC...rE...
+00001080: 7247 0000 0072 3c00 0000 da06 7661 6c75  rG...r<.....valu
+00001090: 6573 2904 720d 0000 00da 0661 6374 696f  es).r......actio
+000010a0: 6e5a 0973 705f 6163 7469 6f6e 725d 0000  nZ.sp_actionr]..
+000010b0: 00a9 01da 155f 7365 745f 6163 7469 6f6e  ....._set_action
+000010c0: 735f 6f70 7469 6f6e 616c 7221 0000 0072  s_optionalr!...r
+000010d0: 2600 0000 726c 0000 00cc 0000 0073 1600  &...rl.......s..
+000010e0: 0000 0a03 0801 0603 0c01 0601 0c01 0e01  ................
+000010f0: 0a01 0280 04fb 0401 7a29 696e 766f 6b65  ........z)invoke
+00001100: 5f74 7569 2e3c 6c6f 6361 6c73 3e2e 5f73  _tui.<locals>._s
+00001110: 6574 5f61 6374 696f 6e73 5f6f 7074 696f  et_actions_optio
+00001120: 6e61 6c29 0272 0f00 0000 7211 0000 0029  nal).r....r....)
+00001130: 025a 0861 7070 5f6e 616d 655a 0e63 6f6d  .Z.app_nameZ.com
+00001140: 6d61 6e64 5f66 696c 7465 7229 0a72 2900  mand_filter).r).
+00001150: 0000 7204 0000 0072 0300 0000 da0a 5379  ..r....r......Sy
+00001160: 7374 656d 4578 6974 da10 7061 7273 655f  stemExit..parse_
+00001170: 6b6e 6f77 6e5f 6172 6773 da04 7661 7273  known_args..vars
+00001180: 7264 0000 0072 0c00 0000 da04 7072 6f67  rd...r......prog
+00001190: da03 7275 6e29 0a72 0d00 0000 720f 0000  ..run).r....r...
+000011a0: 0072 6500 0000 5a0a 636d 645f 6669 6c74  .re...Z.cmd_filt
+000011b0: 6572 5a0b 7061 7273 6564 5f61 7267 7372  erZ.parsed_argsr
+000011c0: 2400 0000 5a0b 7061 7273 6572 5f63 6f70  $...Z.parser_cop
+000011d0: 79da 096e 616d 6573 7061 6365 5a0d 5f75  y..namespaceZ._u
+000011e0: 6e6b 6e6f 776e 5f61 7267 73da 0773 6368  nknown_args..sch
+000011f0: 656d 6173 7221 0000 0072 6b00 0000 7226  emasr!...rk...r&
+00001200: 0000 00da 0a69 6e76 6f6b 655f 7475 69b2  .....invoke_tui.
+00001210: 0000 0073 3400 0000 0410 0401 0402 0801  ...s4...........
+00001220: 0a01 0401 0401 02fe 0c05 080e 0801 0a02  ................
+00001230: 0e01 0a01 1cfe 0204 0201 0201 0201 06fd  ................
+00001240: 0206 0201 0401 0201 04fd 0a04 7274 0000  ............rt..
+00001250: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00001260: 0000 0600 0000 0000 0001 733e 0000 0065  ..........s>...e
+00001270: 005a 0164 005a 0264 015a 0365 046a 0565  .Z.d.Z.d.Z.e.j.e
+00001280: 046a 0564 0264 0364 0364 0366 0664 1587  .j.d.d.d.d.f.d..
+00001290: 0066 0164 1164 1284 0d5a 0664 1664 1364  .f.d.d...Z.d.d.d
+000012a0: 1484 015a 0787 0004 005a 0853 0029 1772  ...Z.....Z.S.).r
+000012b0: 4400 0000 616f 0100 0061 7267 7061 7273  D...ao...argpars
+000012c0: 6520 6041 6374 696f 6e60 2074 6861 7420  e `Action` that 
+000012d0: 7769 6c6c 2061 6e61 6c79 7a65 2074 6865  will analyze the
+000012e0: 2070 6172 7365 7220 616e 6420 6469 7370   parser and disp
+000012f0: 6c61 7920 6120 5455 492e 0a0a 2020 2020  lay a TUI...    
+00001300: 4578 616d 706c 6573 3a0a 2020 2020 2020  Examples:.      
+00001310: 2020 3e3e 3e20 696d 706f 7274 2061 7267    >>> import arg
+00001320: 7061 7273 650a 2020 2020 2020 2020 3e3e  parse.        >>
+00001330: 3e20 6672 6f6d 2061 7267 7061 7273 655f  > from argparse_
+00001340: 7475 6920 696d 706f 7274 2054 7569 4163  tui import TuiAc
+00001350: 7469 6f6e 0a20 2020 2020 2020 202e 2e2e  tion.        ...
+00001360: 0a20 2020 2020 2020 203e 3e3e 2070 6172  .        >>> par
+00001370: 7365 7220 3d20 6172 6770 6172 7365 2e41  ser = argparse.A
+00001380: 7267 756d 656e 7450 6172 7365 7228 290a  rgumentParser().
+00001390: 2020 2020 2020 2020 3e3e 3e20 5f20 3d20          >>> _ = 
+000013a0: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
+000013b0: 656e 7428 272d 2d74 7569 272c 2061 6374  ent('--tui', act
+000013c0: 696f 6e3d 5475 6941 6374 696f 6e29 0a20  ion=TuiAction). 
+000013d0: 2020 2020 2020 202e 2e2e 0a20 2020 2020         ....     
+000013e0: 2020 203e 3e3e 2070 6172 7365 722e 7072     >>> parser.pr
+000013f0: 696e 745f 7573 6167 6528 290a 2020 2020  int_usage().    
+00001400: 2020 2020 7573 6167 653a 205f 5f6d 6169      usage: __mai
+00001410: 6e5f 5f2e 7079 205b 2d68 5d20 5b2d 2d74  n__.py [-h] [--t
+00001420: 7569 5d0a 2020 2020 fa10 4f70 656e 2054  ui].    ..Open T
+00001430: 6578 7475 616c 2055 492e 4e72 4b00 0000  extual UI.NrK...
+00001440: fa09 6c69 7374 5b73 7472 5d72 4a00 0000  ..list[str]rJ...
+00001450: 7255 0000 0072 3900 0000 7205 0000 0072  rU...r9...r....r
+00001460: 3b00 0000 fa0a 7374 7220 7c20 4e6f 6e65  ;.....str | None
+00001470: da05 636f 6e73 74da 076d 6574 6176 6172  ..const..metavar
+00001480: da0d 7061 7265 6e74 5f70 6172 7365 72fa  ..parent_parser.
+00001490: 1e61 7267 7061 7273 652e 4172 6775 6d65  .argparse.Argume
+000014a0: 6e74 5061 7273 6572 207c 204e 6f6e 65da  ntParser | None.
+000014b0: 075f 6b77 6172 6773 6308 0000 0000 0000  ._kwargsc.......
+000014c0: 0000 0000 0009 0000 0009 0000 000b 0000  ................
+000014d0: 0173 2800 0000 7400 7401 7c00 8302 6a02  .s(...t.t.|...j.
+000014e0: 7c01 7c02 7c03 6401 7c04 7c05 7c06 6402  |.|.|.d.|.|.|.d.
+000014f0: 8d07 0100 7c07 7c00 5f03 6400 5300 2903  ....|.|._.d.S.).
+00001500: 4e72 0100 0000 2907 724b 0000 0072 4a00  Nr....).rK...rJ.
+00001510: 0000 7239 0000 0072 3f00 0000 723b 0000  ..r9...r?...r;..
+00001520: 0072 7800 0000 7279 0000 0029 04da 0573  .rx...ry...)...s
+00001530: 7570 6572 7244 0000 00da 085f 5f69 6e69  uperrD.....__ini
+00001540: 745f 5fda 0e5f 7061 7265 6e74 5f70 6172  t__.._parent_par
+00001550: 7365 7229 09da 0473 656c 6672 4b00 0000  ser)...selfrK...
+00001560: 724a 0000 0072 3900 0000 723b 0000 0072  rJ...r9...r;...r
+00001570: 7800 0000 7279 0000 0072 7a00 0000 727c  x...ry...rz...r|
+00001580: 0000 00a9 01da 095f 5f63 6c61 7373 5f5f  .......__class__
+00001590: 7221 0000 0072 2600 0000 727e 0000 00fc  r!...r&...r~....
+000015a0: 0000 0073 1400 0000 0a0b 0201 0201 0201  ...s............
+000015b0: 0201 0201 0201 0201 06f9 0a09 7a12 5475  ............z.Tu
+000015c0: 6941 6374 696f 6e2e 5f5f 696e 6974 5f5f  iAction.__init__
+000015d0: 6305 0000 0000 0000 0000 0000 0008 0000  c...............
+000015e0: 0009 0000 0043 0000 0173 ce00 0000 7c00  .....C...s....|.
+000015f0: 6a00 7206 7c00 6a00 6e01 7c01 7d05 7c04  j.r.|.j.n.|.}.|.
+00001600: 720c 6700 6e02 7c01 6701 7d06 7401 6a02  r.g.n.|.g.}.t.j.
+00001610: 6401 6400 8502 1900 7d07 7c07 725a 7c04  d.d.....}.|.rZ|.
+00001620: 7237 7403 7404 8301 8f10 0100 7c07 a005  r7t.t.......|...
+00001630: 7c07 a006 7c04 a101 a101 0100 5700 6400  |...|.......W.d.
+00001640: 0400 0400 8303 0100 6e08 3100 7331 7701  ........n.1.s1w.
+00001650: 0100 0100 0100 5900 0100 6e23 7403 7404  ......Y...n#t.t.
+00001660: 8301 8f17 0100 7c07 a005 7c07 a006 7c00  ......|...|...|.
+00001670: 6a07 a008 a100 a009 6402 6403 a102 a101  j.......d.d.....
+00001680: a101 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
+00001690: 6e08 3100 7355 7701 0100 0100 0100 5900  n.1.sUw.......Y.
+000016a0: 0100 740a 7c05 7c06 7c07 6404 8d03 0100  ..t.|.|.|.d.....
+000016b0: 7c01 a00b a100 0100 6400 5300 2905 4e72  |.......d.S.).Nr
+000016c0: 0600 0000 da01 5f72 6700 0000 2902 720f  ......_rg...).r.
+000016d0: 0000 0072 6500 0000 290c 727f 0000 0072  ...re...).r....r
+000016e0: 4f00 0000 da04 6172 6776 7203 0000 00da  O.....argvr.....
+000016f0: 0a56 616c 7565 4572 726f 72da 0370 6f70  .ValueError..pop
+00001700: da05 696e 6465 7872 4a00 0000 da05 6c6f  ..indexrJ.....lo
+00001710: 7765 7272 5400 0000 7274 0000 00da 0465  werrT...rt.....e
+00001720: 7869 7429 0872 8000 0000 720d 0000 0072  xit).r....r....r
+00001730: 7200 0000 7269 0000 00da 0d6f 7074 696f  r...ri.....optio
+00001740: 6e5f 7374 7269 6e67 5a0b 726f 6f74 5f70  n_stringZ.root_p
+00001750: 6172 7365 7272 0f00 0000 7265 0000 0072  arserr....re...r
+00001760: 2100 0000 7221 0000 0072 2600 0000 da08  !...r!...r&.....
+00001770: 5f5f 6361 6c6c 5f5f 1201 0000 7326 0000  __call__....s&..
+00001780: 000e 0202 ff0e 030e 0204 0204 010a 0112  ................
+00001790: 011c ff02 800a 0320 011c ff02 0302 0102  ....... ........
+000017a0: 0102 0106 fd0c 067a 1254 7569 4163 7469  .......z.TuiActi
+000017b0: 6f6e 2e5f 5f63 616c 6c5f 5f29 1072 4b00  on.__call__).rK.
+000017c0: 0000 7276 0000 0072 4a00 0000 7255 0000  ..rv...rJ...rU..
+000017d0: 0072 3900 0000 7205 0000 0072 3b00 0000  .r9...r....r;...
+000017e0: 7277 0000 0072 7800 0000 7255 0000 0072  rw...rx...rU...r
+000017f0: 7900 0000 7255 0000 0072 7a00 0000 727b  y...rU...rz...r{
+00001800: 0000 0072 7c00 0000 7205 0000 0072 6200  ...r|...r....rb.
+00001810: 0000 2909 7251 0000 00da 0a5f 5f6d 6f64  ..).rQ.....__mod
+00001820: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00001830: 655f 5fda 075f 5f64 6f63 5f5f 7245 0000  e__..__doc__rE..
+00001840: 0072 4600 0000 727e 0000 0072 8b00 0000  .rF...r~...r....
+00001850: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
+00001860: 2100 0000 7221 0000 0072 8100 0000 7226  !...r!...r....r&
+00001870: 0000 0072 4400 0000 ee00 0000 7314 0000  ...rD.......s...
+00001880: 0008 0004 0104 1004 0102 0102 0102 0102  ................
+00001890: 0110 f812 1672 4400 0000 7275 0000 0072  .....rD...ru...r
+000018a0: 7a00 0000 727b 0000 0072 4b00 0000 fa16  z...r{...rK.....
+000018b0: 7374 7220 7c20 6c69 7374 5b73 7472 5d20  str | list[str] 
+000018c0: 7c20 4e6f 6e65 723b 0000 0072 5500 0000  | Noner;...rU...
+000018d0: da04 4e6f 6e65 6305 0000 0000 0000 0000  ..Nonec.........
+000018e0: 0000 0006 0000 0007 0000 004b 0000 0173  ...........K...s
+000018f0: 4e00 0000 7c02 7310 6401 7400 a001 6402  N...|.s.d.t...d.
+00001900: 6403 a102 a002 6403 a101 9b00 9d02 6701  d.....d.......g.
+00001910: 7d02 6e08 7403 7c02 7404 8302 7218 7c02  }.n.t.|.t...r.|.
+00001920: 6701 7d02 7c00 6a05 7c02 7406 7c04 7c03  g.}.|.j.|.t.|.|.
+00001930: 7c01 6404 9c04 7c05 a401 8e01 0100 6405  |.d...|.......d.
+00001940: 5300 2906 6126 0200 000a 0a20 2020 2041  S.).a&.....    A
+00001950: 7267 733a 0a20 2020 2020 2020 2070 6172  rgs:.        par
+00001960: 7365 723a 2074 6865 2061 7267 7061 7273  ser: the argpars
+00001970: 6520 7061 7273 6572 2074 6f20 6164 6420  e parser to add 
+00001980: 7468 6520 6172 6775 6d65 6e74 2074 6f2e  the argument to.
+00001990: 0a20 2020 2020 2020 2070 6172 656e 745f  .        parent_
+000019a0: 7061 7273 6572 3a20 7468 6520 7061 7265  parser: the pare
+000019b0: 6e74 206f 6620 7468 6520 6769 7665 6e20  nt of the given 
+000019c0: 7061 7273 6572 2e0a 2020 2020 2020 2020  parser..        
+000019d0: 6f70 7469 6f6e 5f73 7472 696e 6773 3a20  option_strings: 
+000019e0: 6c69 7374 206f 6620 434c 4920 666c 6167  list of CLI flag
+000019f0: 7320 7468 6174 2077 696c 6c20 696e 766f  s that will invo
+00001a00: 6b65 2074 6865 2054 5549 2028 6465 6661  ke the TUI (defa
+00001a10: 756c 743d 602d 2d74 7569 6029 0a20 2020  ult=`--tui`).   
+00001a20: 2020 2020 2068 656c 703a 2068 656c 7020       help: help 
+00001a30: 6d65 7373 6167 6520 666f 7220 7468 6520  message for the 
+00001a40: 6172 6775 6d65 6e74 0a0a 2020 2020 4578  argument..    Ex
+00001a50: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
+00001a60: 3e3e 3e20 696d 706f 7274 2061 7267 7061  >>> import argpa
+00001a70: 7273 650a 2020 2020 2020 2020 3e3e 3e20  rse.        >>> 
+00001a80: 6672 6f6d 2061 7267 7061 7273 655f 7475  from argparse_tu
+00001a90: 6920 696d 706f 7274 2061 6464 5f74 7569  i import add_tui
+00001aa0: 5f61 7267 756d 656e 740a 2020 2020 2020  _argument.      
+00001ab0: 2020 2e2e 2e0a 2020 2020 2020 2020 3e3e    ....        >>
+00001ac0: 3e20 7061 7273 6572 203d 2061 7267 7061  > parser = argpa
+00001ad0: 7273 652e 4172 6775 6d65 6e74 5061 7273  rse.ArgumentPars
+00001ae0: 6572 2829 0a20 2020 2020 2020 202e 2e2e  er().        ...
+00001af0: 0a20 2020 2020 2020 203e 3e3e 2061 6464  .        >>> add
+00001b00: 5f74 7569 5f61 7267 756d 656e 7428 7061  _tui_argument(pa
+00001b10: 7273 6572 290a 2020 2020 2020 2020 2e2e  rser).        ..
+00001b20: 2e0a 2020 2020 2020 2020 3e3e 3e20 7061  ..        >>> pa
+00001b30: 7273 6572 2e70 7269 6e74 5f75 7361 6765  rser.print_usage
+00001b40: 2829 0a20 2020 2020 2020 2075 7361 6765  ().        usage
+00001b50: 3a20 5f5f 6d61 696e 5f5f 2e70 7920 5b2d  : __main__.py [-
+00001b60: 685d 205b 2d2d 7475 695d 0a20 2020 207a  h] [--tui].    z
+00001b70: 022d 2d72 8300 0000 7267 0000 0029 0472  .--r....rg...).r
+00001b80: 6a00 0000 7239 0000 0072 3b00 0000 727a  j...r9...r;...rz
+00001b90: 0000 004e 2907 7207 0000 0072 5400 0000  ...N).r....rT...
+00001ba0: da06 6c73 7472 6970 7243 0000 0072 5500  ..lstriprC...rU.
+00001bb0: 0000 da0c 6164 645f 6172 6775 6d65 6e74  ....add_argument
+00001bc0: 7244 0000 0029 0672 0d00 0000 727a 0000  rD...).r....rz..
+00001bd0: 0072 4b00 0000 723b 0000 0072 3900 0000  .rK...r;...r9...
+00001be0: da06 6b77 6172 6773 7221 0000 0072 2100  ..kwargsr!...r!.
+00001bf0: 0000 7226 0000 00da 1061 6464 5f74 7569  ..r&.....add_tui
+00001c00: 5f61 7267 756d 656e 742b 0100 0073 1a00  _argument+...s..
+00001c10: 0000 041b 1c01 0a01 0601 0402 0201 0201  ................
+00001c20: 0201 0201 0201 04fb 0206 0afa 7295 0000  ............r...
+00001c30: 00da 0763 6f6d 6d61 6e64 7294 0000 0072  ...commandr....r
+00001c40: 0500 0000 fa1a 6172 6770 6172 7365 2e5f  ......argparse._
+00001c50: 5375 6250 6172 7365 7273 4163 7469 6f6e  SubParsersAction
+00001c60: 6303 0000 0000 0000 0000 0000 0007 0000  c...............
+00001c70: 0005 0000 004b 0000 0173 6200 0000 7c00  .....K...sb...|.
+00001c80: 6a00 6401 7500 720e 7c00 6a01 6404 6900  j.d.u.r.|.j.d.i.
+00001c90: 7c03 a401 8e01 7d04 6e10 7c00 6a02 4400  |.....}.n.|.j.D.
+00001ca0: 5d0c 7d05 7403 7c05 7404 6a05 8302 721d  ].}.t.|.t.j...r.
+00001cb0: 7c05 7d04 0100 6e01 7111 7c04 6a06 7c01  |.}...n.q.|.j.|.
+00001cc0: 7404 6a07 7c02 6402 8d03 7d06 7408 7c06  t.j.|.d...}.t.|.
+00001cd0: 7c00 7c01 6701 6403 8d03 0100 7c04 5300  |.|.g.d.....|.S.
+00001ce0: 2905 615a 0200 000a 0a20 2020 2041 7267  ).aZ.....    Arg
+00001cf0: 733a 0a20 2020 2020 2020 2070 6172 7365  s:.        parse
+00001d00: 723a 2074 6865 2061 7267 7061 7273 6520  r: the argparse 
+00001d10: 7061 7273 6572 0a20 2020 2020 2020 2063  parser.        c
+00001d20: 6f6d 6d61 6e64 3a20 6e61 6d65 206f 6620  ommand: name of 
+00001d30: 7468 6520 434c 4920 636f 6d6d 616e 6420  the CLI command 
+00001d40: 7468 6174 2077 696c 6c20 696e 766f 6b65  that will invoke
+00001d50: 2074 6865 2054 5549 2028 6465 6661 756c   the TUI (defaul
+00001d60: 743d 6074 7569 6029 0a20 2020 2020 2020  t=`tui`).       
+00001d70: 2068 656c 703a 2068 656c 7020 6d65 7373   help: help mess
+00001d80: 6167 6520 666f 7220 7468 6520 6172 6775  age for the argu
+00001d90: 6d65 6e74 0a20 2020 2020 2020 202a 2a6b  ment.        **k
+00001da0: 7761 7267 733a 2069 6620 7375 6270 6172  wargs: if subpar
+00001db0: 7365 7273 2064 6f20 6e6f 7420 616c 7265  sers do not alre
+00001dc0: 6164 7920 6578 6973 742c 2063 7265 6174  ady exist, creat
+00001dd0: 6520 7769 7468 2074 6865 7365 206b 7761  e with these kwa
+00001de0: 7267 732e 0a0a 2020 2020 4578 616d 706c  rgs...    Exampl
+00001df0: 6573 3a0a 2020 2020 2020 2020 3e3e 3e20  es:.        >>> 
+00001e00: 696d 706f 7274 2061 7267 7061 7273 650a  import argparse.
+00001e10: 2020 2020 2020 2020 3e3e 3e20 6672 6f6d          >>> from
+00001e20: 2061 7267 7061 7273 655f 7475 6920 696d   argparse_tui im
+00001e30: 706f 7274 2061 6464 5f74 7569 5f61 7267  port add_tui_arg
+00001e40: 756d 656e 740a 2020 2020 2020 2020 2e2e  ument.        ..
+00001e50: 2e0a 2020 2020 2020 2020 3e3e 3e20 7061  ..        >>> pa
+00001e60: 7273 6572 203d 2061 7267 7061 7273 652e  rser = argparse.
+00001e70: 4172 6775 6d65 6e74 5061 7273 6572 2829  ArgumentParser()
+00001e80: 0a20 2020 2020 2020 203e 3e3e 2073 7562  .        >>> sub
+00001e90: 7061 7273 6572 7320 3d20 7061 7273 6572  parsers = parser
+00001ea0: 2e61 6464 5f73 7562 7061 7273 6572 7328  .add_subparsers(
+00001eb0: 290a 2020 2020 2020 2020 2e2e 2e0a 2020  ).        ....  
+00001ec0: 2020 2020 2020 3e3e 3e20 5f20 3d20 6164        >>> _ = ad
+00001ed0: 645f 7475 695f 636f 6d6d 616e 6428 7061  d_tui_command(pa
+00001ee0: 7273 6572 290a 2020 2020 2020 2020 2e2e  rser).        ..
+00001ef0: 2e0a 2020 2020 2020 2020 3e3e 3e20 7061  ..        >>> pa
+00001f00: 7273 6572 2e70 7269 6e74 5f75 7361 6765  rser.print_usage
+00001f10: 2829 0a20 2020 2020 2020 2075 7361 6765  ().        usage
+00001f20: 3a20 5f5f 6d61 696e 5f5f 2e70 7920 5b2d  : __main__.py [-
+00001f30: 685d 207b 7475 697d 202e 2e2e 0a20 2020  h] {tui} ....   
+00001f40: 204e 2902 7240 0000 0072 3b00 0000 2902   N).r@...r;...).
+00001f50: 727a 0000 0072 4b00 0000 7221 0000 0029  rz...rK...r!...)
+00001f60: 0972 6800 0000 da0e 6164 645f 7375 6270  .rh.....add_subp
+00001f70: 6172 7365 7273 7242 0000 0072 4300 0000  arsersrB...rC...
+00001f80: 7245 0000 0072 4700 0000 da0a 6164 645f  rE...rG.....add_
+00001f90: 7061 7273 6572 7246 0000 0072 9500 0000  parserrF...r....
+00001fa0: 2907 720d 0000 0072 9600 0000 723b 0000  ).r....r....r;..
+00001fb0: 0072 9400 0000 5a0a 7375 6270 6172 7365  .r....Z.subparse
+00001fc0: 7273 726a 0000 005a 0a74 7569 5f70 6172  rsrj...Z.tui_par
+00001fd0: 7365 7272 2100 0000 7221 0000 0072 2600  serr!...r!...r&.
+00001fe0: 0000 da0f 6164 645f 7475 695f 636f 6d6d  ....add_tui_comm
+00001ff0: 616e 6455 0100 0073 2400 0000 0a1c 1201  andU...s$.......
+00002000: 0a02 0c01 0401 0401 02fe 0404 0201 0401  ................
+00002010: 0201 06fd 0206 0201 0201 0401 06fd 0406  ................
+00002020: 729a 0000 0029 024e 4e29 0872 0d00 0000  r....).NN).r....
+00002030: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+00002040: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
+00002050: 0000 0029 0672 0d00 0000 720e 0000 0072  ...).r....r....r
+00002060: 0f00 0000 7210 0000 0072 6500 0000 7266  ....r....re...rf
+00002070: 0000 0029 0a72 0d00 0000 720e 0000 0072  ...).r....r....r
+00002080: 7a00 0000 727b 0000 0072 4b00 0000 7290  z...r{...rK...r.
+00002090: 0000 0072 3b00 0000 7255 0000 0072 1300  ...r;...rU...r..
+000020a0: 0000 7291 0000 0029 0a72 0d00 0000 720e  ..r....).r....r.
+000020b0: 0000 0072 9600 0000 7255 0000 0072 3b00  ...r....rU...r;.
+000020c0: 0000 7255 0000 0072 9400 0000 7205 0000  ..rU...r....r...
+000020d0: 0072 1300 0000 7297 0000 0029 1ada 0a5f  .r....r....)..._
+000020e0: 5f66 7574 7572 655f 5f72 0200 0000 7245  _future__r....rE
+000020f0: 0000 0072 4f00 0000 da0a 636f 6e74 6578  ...rO.....contex
+00002100: 746c 6962 7203 0000 00da 0463 6f70 7972  tlibr......copyr
+00002110: 0400 0000 da06 7479 7069 6e67 7205 0000  ......typingr...
+00002120: 00da 0963 6f6e 7374 616e 7473 7207 0000  ...constantsr...
+00002130: 0072 7300 0000 7208 0000 0072 0900 0000  .rs...r....r....
+00002140: 720a 0000 0072 0b00 0000 da03 7475 6972  r....r......tuir
+00002150: 0c00 0000 7264 0000 0072 7400 0000 da06  ....rd...rt.....
+00002160: 4163 7469 6f6e 7244 0000 0072 4600 0000  ActionrD...rF...
+00002170: 7295 0000 0072 9a00 0000 7221 0000 0072  r....r....r!...r
+00002180: 2100 0000 7221 0000 0072 2600 0000 da08  !...r!...r&.....
+00002190: 3c6d 6f64 756c 653e 0100 0000 7332 0000  <module>....s2..
+000021a0: 000c 0008 0208 010c 010c 010c 010c 0218  ................
+000021b0: 010c 0102 0502 010c fd00 7f02 2702 010c  ............'...
+000021c0: fd12 3c02 3f02 0102 0104 010c fb02 2c02  ..<.?.........,.
+000021d0: 0110 fd                                  ...
```

### Comparing `argparse-tui-0.1.3/src/argparse_tui/__pycache__/detect_run_string.cpython-310.pyc` & `argparse-tui-0.2.0/src/argparse_tui/__pycache__/detect_run_string.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 04:37:17 2023 UTC, .py size: 1740 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 fd45 c364 cc06 0000  o........E.d....
+00000000: 6f0d 0d0a 0000 0000 0f82 c564 cc06 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 640b 6405 6406 8404 5a05 6402 6504  Z.d.d.d...Z.d.e.
 00000060: 6a06 6407 1900 6602 640c 6409 640a 8405  j.d...f.d.d.d...
 00000070: 5a07 6402 5300 290d e900 0000 0029 01da  Z.d.S.)......)..
```

### Comparing `argparse-tui-0.1.3/src/argparse_tui/__pycache__/run_command.cpython-310.pyc` & `argparse-tui-0.2.0/src/argparse_tui/__pycache__/run_command.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 04:37:17 2023 UTC, .py size: 10938 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 fd45 c364 ba2a 0000  o........E.d.*..
+00000000: 6f0d 0d0a 0000 0000 0f82 c564 ba2a 0000  o..........d.*..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 c400 0000 5500  .....@...s....U.
 00000030: 6400 6401 6c00 6d01 5a01 0100 6400 6402  d.d.l.m.Z...d.d.
 00000040: 6c02 5a02 6400 6402 6c03 5a03 6400 6403  l.Z.d.d.l.Z.d.d.
 00000050: 6c04 6d05 5a05 0100 6400 6404 6c06 6d07  l.m.Z...d.d.l.m.
 00000060: 5a07 0100 6400 6405 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000070: 5a0a 6d0b 5a0b 0100 6400 6406 6c0c 6d0d  Z.m.Z...d.d.l.m.
@@ -180,15 +180,15 @@
 00000b30: 206f 6620 7374 7269 6e67 7320 7468 6174   of strings that
 00000b40: 2063 616e 2062 6520 7061 7373 6564 2074   can be passed t
 00000b50: 6f20 7375 6270 726f 6365 7373 2e72 756e  o subprocess.run
 00000b60: 2074 6f20 6578 6563 7574 6520 7468 6520   to execute the 
 00000b70: 636f 6d6d 616e 642e 0a20 2020 2020 2020  command..       
 00000b80: 20a9 0172 2e00 0000 7209 0000 004e 2901   ..r....r....N).
 00000b90: da0c 5f74 6f5f 636c 695f 6172 6773 2904  .._to_cli_args).
-00000ba0: 721a 0000 0072 2c00 0000 722e 0000 005a  r....r,...r....Z
+00000ba0: 721a 0000 0072 2c00 0000 722e 0000 00da  r....r,...r.....
 00000bb0: 0863 6c69 5f61 7267 7372 1b00 0000 721b  .cli_argsr....r.
 00000bc0: 0000 0072 1c00 0000 da0b 746f 5f63 6c69  ...r......to_cli
 00000bd0: 5f61 7267 7352 0000 0073 0800 0000 0c0b  _argsR...s......
 00000be0: 0401 0c01 0402 7a1b 5573 6572 436f 6d6d  ......z.UserComm
 00000bf0: 616e 6444 6174 612e 746f 5f63 6c69 5f61  andData.to_cli_a
 00000c00: 7267 7363 0200 0000 0000 0000 0000 0000  rgsc............
 00000c10: 1c00 0000 0900 0000 4300 0001 73c8 0300  ........C...s...
@@ -263,71 +263,71 @@
 00001060: 0aff 7a2f 5573 6572 436f 6d6d 616e 6444  ..z/UserCommandD
 00001070: 6174 612e 5f74 6f5f 636c 695f 6172 6773  ata._to_cli_args
 00001080: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
 00001090: 7072 3e29 01da 036b 6579 2901 5463 0100  pr>)...key).Tc..
 000010a0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
 000010b0: 0000 7300 0001 7318 0000 0081 007c 005d  ..s...s......|.]
 000010c0: 077d 0174 007c 0183 0156 0001 0071 0264  .}.t.|...V...q.d
-000010d0: 0053 0072 3400 0000 2901 da03 6c65 6e29  .S.r4...)...len)
-000010e0: 0272 3600 0000 da0e 7375 6276 616c 7565  .r6.....subvalue
+000010d0: 0053 0072 3500 0000 2901 da03 6c65 6e29  .S.r5...)...len)
+000010e0: 0272 3700 0000 da0e 7375 6276 616c 7565  .r7.....subvalue
 000010f0: 5f74 7570 6c65 721b 0000 0072 1b00 0000  _tupler....r....
-00001100: 721c 0000 0072 3700 0000 ad00 0000 730a  r....r7.......s.
+00001100: 721c 0000 0072 3800 0000 ad00 0000 730a  r....r8.......s.
 00001110: 0000 0002 8004 0002 0206 ff0a ff63 0100  .............c..
 00001120: 0000 0000 0000 0000 0000 0300 0000 0300  ................
 00001130: 0000 7300 0001 731e 0000 0081 007c 005d  ..s...s......|.]
 00001140: 0a7d 017c 0144 005d 057d 027c 0256 0001  .}.|.D.].}.|.V..
-00001150: 0071 0671 0264 0053 0072 3400 0000 721b  .q.q.d.S.r4...r.
-00001160: 0000 0029 0372 3600 0000 723b 0000 005a  ...).r6...r;...Z
+00001150: 0071 0671 0264 0053 0072 3500 0000 721b  .q.q.d.S.r5...r.
+00001160: 0000 0029 0372 3700 0000 723c 0000 005a  ...).r7...r<...Z
 00001170: 0873 7562 7661 6c75 6572 1b00 0000 721b  .subvaluer....r.
-00001180: 0000 0072 1c00 0000 7237 0000 00b3 0000  ...r....r7......
+00001180: 0000 0072 1c00 0000 7238 0000 00b3 0000  ...r....r8......
 00001190: 0073 1000 0000 0280 0400 0202 0201 04fd  .s..............
 000011a0: 0203 02fe 0cff 7209 0000 00e9 0500 0000  ......r.........
 000011b0: 7a02 2d2d da01 2d63 0100 0000 0000 0000  z.--..-c........
 000011c0: 0000 0000 0200 0000 0400 0000 5300 0001  ............S...
 000011d0: f31a 0000 0067 007c 005d 097d 017c 0174  .....g.|.].}.|.t
 000011e0: 0083 006b 0372 027c 0191 0271 0253 0072  ...k.r.|...q.S.r
-000011f0: 1b00 0000 720f 0000 0072 3500 0000 721b  ....r....r5...r.
+000011f0: 1b00 0000 720f 0000 0072 3600 0000 721b  ....r....r6...r.
 00001200: 0000 0072 1b00 0000 721c 0000 00da 0a3c  ...r....r......<
 00001210: 6c69 7374 636f 6d70 3ecc 0000 00f3 0400  listcomp>.......
 00001220: 0000 0600 1401 7a30 5573 6572 436f 6d6d  ......z0UserComm
 00001230: 616e 6444 6174 612e 5f74 6f5f 636c 695f  andData._to_cli_
 00001240: 6172 6773 2e3c 6c6f 6361 6c73 3e2e 3c6c  args.<locals>.<l
 00001250: 6973 7463 6f6d 703e 6301 0000 0000 0000  istcomp>c.......
 00001260: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
-00001270: 0172 3e00 0000 721b 0000 0072 0f00 0000  .r>...r....r....
-00001280: 7235 0000 0072 1b00 0000 721b 0000 0072  r5...r....r....r
-00001290: 1c00 0000 723f 0000 00d3 0000 0072 4000  ....r?.......r@.
+00001270: 0172 3f00 0000 721b 0000 0072 0f00 0000  .r?...r....r....
+00001280: 7236 0000 0072 1b00 0000 721b 0000 0072  r6...r....r....r
+00001290: 1c00 0000 7240 0000 00d3 0000 0072 4100  ....r@.......rA.
 000012a0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-000012b0: 0000 0003 0000 0073 0000 0172 3300 0000  .......s...r3...
-000012c0: 7234 0000 0072 0f00 0000 7235 0000 0072  r4...r....r5...r
-000012d0: 1b00 0000 721b 0000 0072 1c00 0000 7237  ....r....r....r7
-000012e0: 0000 00da 0000 0072 3800 0000 6301 0000  .......r8...c...
+000012b0: 0000 0003 0000 0073 0000 0172 3400 0000  .......s...r4...
+000012c0: 7235 0000 0072 0f00 0000 7236 0000 0072  r5...r....r6...r
+000012d0: 1b00 0000 721b 0000 0072 1c00 0000 7238  ....r....r....r8
+000012e0: 0000 00da 0000 0072 3900 0000 6301 0000  .......r9...c...
 000012f0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
 00001300: 0073 0000 0173 1a00 0000 8100 7c00 5d08  .s...s......|.].
 00001310: 7d01 7c01 7400 8300 6b02 5600 0100 7102  }.|.t...k.V...q.
-00001320: 6400 5300 7234 0000 0072 0f00 0000 7235  d.S.r4...r....r5
+00001320: 6400 5300 7235 0000 0072 0f00 0000 7236  d.S.r5...r....r6
 00001330: 0000 0072 1b00 0000 721b 0000 0072 1c00  ...r....r....r..
-00001340: 0000 7237 0000 00e1 0000 0073 0400 0000  ..r7.......s....
+00001340: 0000 7238 0000 00e1 0000 0073 0400 0000  ..r8.......s....
 00001350: 0280 1800 7201 0000 0063 0100 0000 0000  ....r....c......
 00001360: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-00001370: 0001 723e 0000 0072 1b00 0000 720f 0000  ..r>...r....r...
-00001380: 0072 3500 0000 721b 0000 0072 1b00 0000  .r5...r....r....
-00001390: 721c 0000 0072 3f00 0000 ed00 0000 7240  r....r?.......r@
+00001370: 0001 723f 0000 0072 1b00 0000 720f 0000  ..r?...r....r...
+00001380: 0072 3600 0000 721b 0000 0072 1b00 0000  .r6...r....r....
+00001390: 721c 0000 0072 4000 0000 ed00 0000 7241  r....r@.......rA
 000013a0: 0000 0072 3000 0000 292d 7214 0000 0072  ...r0...)-r....r
 000013b0: 0300 0000 da04 6c69 7374 7227 0000 0072  ......listr'...r
 000013c0: 1700 0000 da08 6d75 6c74 6970 6c65 721d  ......multipler.
 000013d0: 0000 00da 0661 7070 656e 6472 1600 0000  .....appendr....
 000013e0: 720d 0000 00da 1270 726f 6365 7373 5f63  r......process_c
 000013f0: 6c69 5f6f 7074 696f 6eda 0676 616c 7565  li_option..value
 00001400: 73da 0764 6566 6175 6c74 da05 7475 706c  s..default..tupl
 00001410: 65da 0673 6f72 7465 64da 0969 7465 7274  e..sorted..itert
 00001420: 6f6f 6c73 da05 6368 6169 6eda 0d66 726f  ools..chain..fro
 00001430: 6d5f 6974 6572 6162 6c65 da03 616e 79da  m_iterable..any.
 00001440: 036d 6170 7211 0000 0072 1900 0000 da08  .mapr....r......
-00001450: 636f 756e 7469 6e67 da03 6d69 6e72 3a00  counting..minr:.
+00001450: 636f 756e 7469 6e67 da03 6d69 6e72 3b00  counting..minr;.
 00001460: 0000 da03 6d61 78da 0769 735f 666c 6167  ....max..is_flag
 00001470: da0e 7365 636f 6e64 6172 795f 6f70 7473  ..secondary_opts
 00001480: da06 7365 6372 6574 da06 6578 7465 6e64  ..secret..extend
 00001490: 7212 0000 00da 0373 756d da04 6e65 7874  r......sum..next
 000014a0: da03 696e 74da 0a56 616c 7565 4572 726f  ..int..ValueErro
 000014b0: 72da 0a73 7461 7274 7377 6974 68da 066c  r..startswith..l
 000014c0: 7374 7269 70da 0569 7465 6d73 da09 656e  strip..items..en
@@ -341,19 +341,19 @@
 00001540: 615a 0c64 6566 6175 6c74 5f64 6174 615a  aZ.default_dataZ
 00001550: 1066 6c61 7474 656e 6564 5f76 616c 7565  .flattened_value
 00001560: 735a 1266 6c61 7474 656e 6564 5f64 6566  sZ.flattened_def
 00001570: 6175 6c74 735a 0f76 616c 7565 735f 7375  aultsZ.values_su
 00001580: 7070 6c69 6564 5a13 7661 6c75 6573 5f61  ppliedZ.values_a
 00001590: 7265 5f64 6566 6175 6c74 73da 0b6f 7074  re_defaults..opt
 000015a0: 696f 6e5f 6e61 6d65 5a0c 6973 5f74 7275  ion_nameZ.is_tru
-000015b0: 655f 626f 6f6c 7251 0000 0072 5200 0000  e_boolrQ...rR...
+000015b0: 655f 626f 6f6c 7252 0000 0072 5300 0000  e_boolrR...rS...
 000015c0: 5a16 6c6f 6e67 6573 745f 7365 636f 6e64  Z.longest_second
 000015d0: 6172 795f 6e61 6d65 da05 636f 756e 745a  ary_name..countZ
 000015e0: 1163 6c65 616e 5f6f 7074 696f 6e5f 6e61  .clean_option_na
-000015f0: 6d65 7245 0000 00da 0673 6368 656d 61da  merE.....schema.
+000015f0: 6d65 7246 0000 00da 0673 6368 656d 61da  merF.....schema.
 00001600: 0864 6566 6175 6c74 735a 0e64 6566 6175  .defaultsZ.defau
 00001610: 6c74 5f76 616c 7565 735a 1173 7570 706c  lt_valuesZ.suppl
 00001620: 6965 645f 6465 6661 756c 7473 5a0f 7375  ied_defaultsZ.su
 00001630: 7070 6c69 6564 5f76 616c 7565 73da 0169  pplied_values..i
 00001640: da08 6172 6775 6d65 6e74 5a0f 7468 6973  ..argumentZ.this
 00001650: 5f61 7267 5f76 616c 7565 7372 1b00 0000  _arg_valuesr....
 00001660: 721b 0000 0072 1c00 0000 7231 0000 0063  r....r....r1...c
@@ -392,40 +392,40 @@
 00001870: 2020 2020 2020 2020 4120 7374 7269 6e67          A string
 00001880: 2072 6570 7265 7365 6e74 696e 6720 7468   representing th
 00001890: 6520 636f 6d6d 616e 6420 696e 766f 6361  e command invoca
 000018a0: 7469 6f6e 2e0a 2020 2020 2020 2020 5429  tion..        T)
 000018b0: 0272 2c00 0000 722e 0000 007a 033f 3f3f  .r,...r....z.???
 000018c0: 7a11 626f 6c64 2062 6c61 636b 206f 6e20  z.bold black on 
 000018d0: 7265 6429 01da 0573 7479 6c65 da01 2029  red)...style.. )
-000018e0: 0872 3200 0000 7243 0000 0072 1000 0000  .r2...rC...r....
+000018e0: 0872 3300 0000 7244 0000 0072 1000 0000  .r3...rD...r....
 000018f0: 7208 0000 00da 0573 686c 6578 da05 7175  r......shlex..qu
 00001900: 6f74 6572 1100 0000 da04 6a6f 696e 2905  oter......join).
-00001910: 721a 0000 0072 2c00 0000 725f 0000 005a  r....r,...r_...Z
+00001910: 721a 0000 0072 2c00 0000 7260 0000 005a  r....r,...r`...Z
 00001920: 1074 6578 745f 7265 6e64 6572 6162 6c65  .text_renderable
 00001930: 73da 0361 7267 721b 0000 0072 1b00 0000  s..argr....r....
 00001940: 721c 0000 00da 0d74 6f5f 636c 695f 7374  r......to_cli_st
 00001950: 7269 6e67 fb00 0000 7318 0000 0004 0802  ring....s.......
 00001960: 0102 0106 fe04 0508 0104 010a 0212 ff0a  ................
 00001970: 0206 fd0e 057a 1d55 7365 7243 6f6d 6d61  .....z.UserComma
 00001980: 6e64 4461 7461 2e74 6f5f 636c 695f 7374  ndData.to_cli_st
 00001990: 7269 6e67 2902 4646 2906 722c 0000 0072  ring).FF).r,...r
 000019a0: 2d00 0000 722e 0000 0072 2d00 0000 7218  -...r....r-...r.
 000019b0: 0000 0072 2f00 0000 2901 4629 0272 2e00  ...r/...).F).r..
 000019c0: 0000 722d 0000 0029 0472 2c00 0000 722d  ..r-...).r,...r-
 000019d0: 0000 0072 1800 0000 7208 0000 0029 0b72  ...r....r....).r
 000019e0: 1e00 0000 721f 0000 0072 2000 0000 7221  ....r....r ...r!
 000019f0: 0000 0072 2200 0000 7229 0000 0072 2a00  ...r"...r)...r*.
-00001a00: 0000 722b 0000 0072 3200 0000 7231 0000  ..r+...r2...r1..
-00001a10: 0072 6d00 0000 721b 0000 0072 1b00 0000  .rm...r....r....
+00001a00: 0000 722b 0000 0072 3300 0000 7231 0000  ..r+...r3...r1..
+00001a10: 0072 6e00 0000 721b 0000 0072 1b00 0000  .rn...r....r....
 00001a20: 721b 0000 0072 1c00 0000 7226 0000 003e  r....r....r&...>
 00001a30: 0000 0073 1c00 0000 0a00 0402 080b 0801  ...s............
 00001a40: 0801 0c01 0c01 0c01 0204 0201 0cfd 0c11  ................
 00001a50: 007f 1019 7226 0000 0029 1bda 0a5f 5f66  ....r&...)...__f
-00001a60: 7574 7572 655f 5f72 0200 0000 7249 0000  uture__r....rI..
-00001a70: 0072 6900 0000 da0b 636f 6c6c 6563 7469  .ri.....collecti
+00001a60: 7574 7572 655f 5f72 0200 0000 724a 0000  uture__r....rJ..
+00001a70: 0072 6a00 0000 da0b 636f 6c6c 6563 7469  .rj.....collecti
 00001a80: 6f6e 7372 0300 0000 da0b 6461 7461 636c  onsr......datacl
 00001a90: 6173 7365 7372 0400 0000 da06 7479 7069  assesr......typi
 00001aa0: 6e67 7205 0000 0072 0600 0000 7207 0000  ngr....r....r...
 00001ab0: 00da 0972 6963 682e 7465 7874 7208 0000  ...rich.textr...
 00001ac0: 00da 0773 6368 656d 6173 720a 0000 0072  ...schemasr....r
 00001ad0: 0b00 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
 00001ae0: 0000 005a 1a77 6964 6765 7473 2e70 6172  ...Z.widgets.par
```

### Comparing `argparse-tui-0.1.3/src/argparse_tui/__pycache__/schemas.cpython-310.pyc` & `argparse-tui-0.2.0/src/argparse_tui/__pycache__/schemas.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 04:37:17 2023 UTC, .py size: 3736 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 fd45 c364 980e 0000  o........E.d....
+00000000: 6f0d 0d0a 0000 0000 0f82 c564 940f 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 ba00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 0100 6406 6407 8400 5a0d 6504  m.Z...d.d...Z.e.
@@ -94,170 +94,174 @@
 000005d0: 1a43 686f 6963 6553 6368 656d 612e 5f5f  .ChoiceSchema.__
 000005e0: 706f 7374 5f69 6e69 745f 5f4e 2905 721d  post_init__N).r.
 000005f0: 0000 0072 1e00 0000 721f 0000 0072 2000  ...r....r....r .
 00000600: 0000 7226 0000 0072 0e00 0000 720e 0000  ..r&...r....r...
 00000610: 0072 0e00 0000 720f 0000 0072 2200 0000  .r....r....r"...
 00000620: 2200 0000 7306 0000 000a 0008 030c 0272  "...s..........r
 00000630: 2200 0000 6300 0000 0000 0000 0000 0000  "...c...........
-00000640: 0000 0000 0003 0000 0040 0000 0173 b400  .........@...s..
+00000640: 0000 0000 0003 0000 0040 0000 0173 c000  .........@...s..
 00000650: 0000 6500 5a01 6400 5a02 5500 6401 6503  ..e.Z.d.Z.U.d.e.
 00000660: 6402 3c00 6403 5a04 6404 6503 6405 3c00  d.<.d.Z.d.e.d.<.
 00000670: 6406 5a05 6407 6503 6408 3c00 6403 5a06  d.Z.d.e.d.<.d.Z.
 00000680: 6409 6503 640a 3c00 6507 6508 640b 8d01  d.e.d.<.e.e.d...
 00000690: 5a09 640c 6503 640d 3c00 6403 5a0a 640e  Z.d.e.d.<.d.Z.d.
-000006a0: 6503 640f 3c00 6403 5a0b 6410 6503 6411  e.d.<.d.Z.d.e.d.
-000006b0: 3c00 6406 5a0c 6407 6503 6412 3c00 6406  <.d.Z.d.e.d.<.d.
-000006c0: 5a0d 6407 6503 6413 3c00 6414 5a0e 6415  Z.d.e.d.<.d.Z.d.
-000006d0: 6503 6416 3c00 6406 5a0f 6407 6503 6417  e.d.<.d.Z.d.e.d.
-000006e0: 3c00 6406 5a10 6407 6503 6418 3c00 6419  <.d.Z.d.e.d.<.d.
-000006f0: 5a11 641a 6503 641b 3c00 641c 641d 8400  Z.d.e.d.<.d.d...
-00000700: 5a12 6403 5300 291e da0e 4172 6775 6d65  Z.d.S.)...Argume
-00000710: 6e74 5363 6865 6d61 7a0f 7374 7220 7c20  ntSchemaz.str | 
-00000720: 6c69 7374 5b73 7472 5dda 046e 616d 654e  list[str]..nameN
-00000730: 7a26 5479 7065 5b41 6e79 5d20 7c20 5365  z&Type[Any] | Se
-00000740: 7175 656e 6365 5b54 7970 655b 416e 795d  quence[Type[Any]
-00000750: 5d20 7c20 4e6f 6e65 da04 7479 7065 46da  ] | None..typeF.
-00000760: 0462 6f6f 6cda 0872 6571 7569 7265 64fa  .bool..required.
-00000770: 0a73 7472 207c 204e 6f6e 65da 0468 656c  .str | None..hel
-00000780: 70a9 01da 0f64 6566 6175 6c74 5f66 6163  p....default_fac
-00000790: 746f 7279 7a10 7374 7220 7c20 7475 706c  toryz.str | tupl
-000007a0: 655b 7374 725d da03 6b65 797a 204d 756c  e[str]..keyz Mul
-000007b0: 7469 5661 6c75 6550 6172 616d 4461 7461  tiValueParamData
-000007c0: 207c 2041 6e79 207c 204e 6f6e 65da 0764   | Any | None..d
-000007d0: 6566 6175 6c74 7a14 5365 7175 656e 6365  efaultz.Sequence
-000007e0: 5b73 7472 5d20 7c20 4e6f 6e65 7223 0000  [str] | Noner#..
-000007f0: 00da 086d 756c 7469 706c 65da 0b6d 756c  ...multiple..mul
-00000800: 7469 5f76 616c 7565 e901 0000 00da 0369  ti_value.......i
-00000810: 6e74 da05 6e61 7267 73da 0673 6563 7265  nt..nargs..secre
-00000820: 74da 0972 6561 645f 6f6e 6c79 da00 720b  t..read_only..r.
-00000830: 0000 00da 0b70 6c61 6365 686f 6c64 6572  .....placeholder
-00000840: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
-00000850: 0004 0000 0043 0000 0173 0401 0000 7400  .....C...s....t.
-00000860: 7c00 6a01 7402 8302 730d 7402 a003 7c00  |.j.t...s.t...|.
-00000870: 6a01 a101 7c00 5f01 7404 6701 7d01 7c00  j...|._.t.g.}.|.
-00000880: 6a05 7317 7c01 7c00 5f05 6e55 7400 7c00  j.s.|.|._.nUt.|.
-00000890: 6a05 7406 8302 7247 7c00 6a05 6a07 4400  j.t...rG|.j.j.D.
-000008a0: 5d0d 7d02 7400 7c02 7408 8302 722e 7c02  ].}.t.|.t...r.|.
-000008b0: 6701 7c00 5f05 0100 6e18 7121 7c00 6a05  g.|._...n.q!|.j.
-000008c0: 6a09 a00a a100 4400 5d0d 7d03 7400 7c03  j.....D.].}.t.|.
-000008d0: 7408 8302 7242 7c03 6701 7c00 5f05 0100  t...rB|.g.|._...
-000008e0: 6e04 7135 7c01 7c00 5f05 6e25 7400 7c00  n.q5|.|._.n%t.|.
-000008f0: 6a05 7408 8302 7253 7c00 6a05 6701 7c00  j.t...rS|.j.g.|.
-00000900: 5f05 6e19 740b 7c00 6a05 8301 6401 6b02  _.n.t.|.j...d.k.
-00000910: 726c 7400 7c00 6a05 6402 1900 740c 8302  rlt.|.j.d...t...
-00000920: 726c 7c00 6a05 6402 1900 6a0d 7c00 5f0d  rl|.j.d...j.|._.
-00000930: 7c01 7c00 5f05 7c00 6a0d 7278 6403 6404  |.|._.|.j.rxd.d.
-00000940: 8400 7c00 6a0d 4400 8301 7c00 5f0d 7c00  ..|.j.D...|._.|.
-00000950: 6a0e 7280 6405 7c00 5f0f 6400 5300 6400  j.r.d.|._.d.S.d.
-00000960: 5300 2906 4e72 3400 0000 7201 0000 0063  S.).Nr4...r....c
-00000970: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000980: 0400 0000 5300 0001 7314 0000 0067 007c  ....S...s....g.|
-00000990: 005d 067d 0174 007c 0183 0191 0271 0253  .].}.t.|.....q.S
-000009a0: 0072 0e00 0000 2901 720b 0000 0029 0272  .r....).r....).r
-000009b0: 1700 0000 da01 7872 0e00 0000 720e 0000  ......xr....r...
-000009c0: 0072 0f00 0000 7219 0000 005a 0000 0073  .r....r....Z...s
-000009d0: 0200 0000 1400 7a30 4172 6775 6d65 6e74  ......z0Argument
-000009e0: 5363 6865 6d61 2e5f 5f70 6f73 745f 696e  Schema.__post_in
-000009f0: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c6c  it__.<locals>.<l
-00000a00: 6973 7463 6f6d 703e 5429 1072 1500 0000  istcomp>T).r....
-00000a10: 7231 0000 0072 1100 0000 721c 0000 0072  r1...r....r....r
-00000a20: 0b00 0000 7229 0000 0072 0500 0000 da04  ....r)...r......
-00000a30: 6172 6773 7209 0000 00da 066b 7761 7267  argsr......kwarg
-00000a40: 7372 1200 0000 da03 6c65 6e72 2200 0000  sr......lenr"...
-00000a50: 7223 0000 0072 3300 0000 7232 0000 0029  r#...r3...r2...)
-00000a60: 0472 2500 0000 5a0c 6465 6661 756c 745f  .r%...Z.default_
-00000a70: 7479 7065 723b 0000 00da 0176 720e 0000  typer;.....vr...
-00000a80: 0072 0e00 0000 720f 0000 0072 2600 0000  .r....r....r&...
-00000a90: 3b00 0000 7338 0000 000c 010e 0106 0206  ;...s8..........
-00000aa0: 0208 010c 010c 040a 0108 0104 0102 fe10  ................
-00000ab0: 040a 0108 0104 0102 fe06 0402 800c 010c  ................
-00000ac0: 011e 010e 0206 0106 0212 0106 020a 0104  ................
-00000ad0: ff7a 1c41 7267 756d 656e 7453 6368 656d  .z.ArgumentSchem
-00000ae0: 612e 5f5f 706f 7374 5f69 6e69 745f 5f29  a.__post_init__)
-00000af0: 1372 1d00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00000b00: 7220 0000 0072 2900 0000 722b 0000 0072  r ...r)...r+...r
-00000b10: 2d00 0000 7204 0000 0072 1000 0000 7230  -...r....r....r0
-00000b20: 0000 0072 3100 0000 7223 0000 0072 3200  ...r1...r#...r2.
-00000b30: 0000 7233 0000 0072 3600 0000 7237 0000  ..r3...r6...r7..
-00000b40: 0072 3800 0000 723a 0000 0072 2600 0000  .r8...r:...r&...
-00000b50: 720e 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
-00000b60: 0f00 0000 7227 0000 002b 0000 0073 1e00  ....r'...+...s..
-00000b70: 0000 0a00 0802 0c01 0c01 0c01 1201 0c01  ................
-00000b80: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c02  ................
-00000b90: 7227 0000 0063 0000 0000 0000 0000 0000  r'...c..........
-00000ba0: 0000 0000 0000 0300 0000 4000 0001 7332  ..........@...s2
-00000bb0: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
-00000bc0: 0364 0265 0464 033c 0064 015a 0564 0265  .d.e.d.<.d.Z.d.e
-00000bd0: 0464 043c 0064 055a 0664 0665 0464 073c  .d.<.d.Z.d.e.d.<
-00000be0: 0064 0553 0029 08da 0c4f 7074 696f 6e53  .d.S.)...OptionS
-00000bf0: 6368 656d 6146 722a 0000 00da 0769 735f  chemaFr*.....is_
-00000c00: 666c 6167 da08 636f 756e 7469 6e67 4e7a  flag..countingNz
-00000c10: 106c 6973 745b 7374 725d 207c 204e 6f6e  .list[str] | Non
-00000c20: 65da 0e73 6563 6f6e 6461 7279 5f6f 7074  e..secondary_opt
-00000c30: 7329 0772 1d00 0000 721e 0000 0072 1f00  s).r....r....r..
-00000c40: 0000 7241 0000 0072 2000 0000 7242 0000  ..rA...r ...rB..
-00000c50: 0072 4300 0000 720e 0000 0072 0e00 0000  .rC...r....r....
-00000c60: 720e 0000 0072 0f00 0000 7240 0000 0060  r....r....r@...`
-00000c70: 0000 0073 0800 0000 0a00 0c02 0c01 1001  ...s............
-00000c80: 7240 0000 0063 0000 0000 0000 0000 0000  r@...c..........
-00000c90: 0000 0000 0000 0400 0000 4000 0001 7384  ..........@...s.
-00000ca0: 0000 0065 005a 0164 005a 0255 0064 0165  ...e.Z.d.Z.U.d.e
-00000cb0: 0364 023c 0064 035a 0464 0465 0364 053c  .d.<.d.Z.d.e.d.<
-00000cc0: 0065 0565 0664 068d 015a 0764 0765 0364  .e.e.d...Z.d.e.d
-00000cd0: 083c 0065 0565 0864 068d 015a 0964 0965  .<.e.e.d...Z.d.e
-00000ce0: 0364 0a3c 0065 0565 0864 068d 015a 0a64  .d.<.e.e.d...Z.d
-00000cf0: 0b65 0364 0c3c 0065 0565 0b64 068d 015a  .e.d.<.e.e.d...Z
-00000d00: 0c64 0d65 0364 0e3c 0064 035a 0d64 0f65  .d.e.d.<.d.Z.d.e
-00000d10: 0364 103c 0065 0e64 1564 1364 1484 0483  .d.<.e.d.d.d....
-00000d20: 015a 0f64 0353 0029 16da 0d43 6f6d 6d61  .Z.d.S.)...Comma
-00000d30: 6e64 5363 6865 6d61 da0b 436f 6d6d 616e  ndSchema..Comman
-00000d40: 644e 616d 6572 2800 0000 4e72 2c00 0000  dNamer(...Nr,...
-00000d50: da09 646f 6373 7472 696e 6772 2e00 0000  ..docstringr....
-00000d60: 720b 0000 0072 3000 0000 7a12 6c69 7374  r....r0...z.list
-00000d70: 5b4f 7074 696f 6e53 6368 656d 615d da07  [OptionSchema]..
-00000d80: 6f70 7469 6f6e 737a 146c 6973 745b 4172  optionsz.list[Ar
-00000d90: 6775 6d65 6e74 5363 6865 6d61 5dda 0961  gumentSchema]..a
-00000da0: 7267 756d 656e 7473 7a24 6469 6374 5b27  rgumentsz$dict['
-00000db0: 436f 6d6d 616e 644e 616d 6527 2c20 2743  CommandName', 'C
-00000dc0: 6f6d 6d61 6e64 5363 6865 6d61 275d da0b  ommandSchema']..
-00000dd0: 7375 6263 6f6d 6d61 6e64 737a 1627 436f  subcommandsz.'Co
-00000de0: 6d6d 616e 6453 6368 656d 6120 7c20 4e6f  mmandSchema | No
-00000df0: 6e65 27da 0670 6172 656e 7472 1300 0000  ne'..parentr....
-00000e00: fa15 6c69 7374 5b27 436f 6d6d 616e 6453  ..list['CommandS
-00000e10: 6368 656d 6127 5d63 0100 0000 0000 0000  chema']c........
-00000e20: 0000 0000 0300 0000 0300 0000 4300 0001  ............C...
-00000e30: 7334 0000 007c 007d 017c 0067 017d 0209  s4...|.}.|.g.}..
-00000e40: 007c 016a 007d 017c 0164 0075 0072 0e6e  .|.j.}.|.d.u.r.n
-00000e50: 067c 02a0 017c 01a1 0101 0071 0674 0274  .|...|.....q.t.t
-00000e60: 037c 0283 0183 0153 0029 014e 2904 724a  .|.....S.).N).rJ
-00000e70: 0000 00da 0661 7070 656e 6472 1a00 0000  .....appendr....
-00000e80: da08 7265 7665 7273 6564 2903 7225 0000  ..reversed).r%..
-00000e90: 00da 046e 6f64 65da 0470 6174 6872 0e00  ...node..pathr..
-00000ea0: 0000 720e 0000 0072 0f00 0000 da0e 7061  ..r....r......pa
-00000eb0: 7468 5f66 726f 6d5f 726f 6f74 7100 0000  th_from_rootq...
-00000ec0: 7312 0000 0004 0206 0102 0106 0108 0102  s...............
-00000ed0: 010a 0102 fc0c 057a 1c43 6f6d 6d61 6e64  .......z.Command
-00000ee0: 5363 6865 6d61 2e70 6174 685f 6672 6f6d  Schema.path_from
-00000ef0: 5f72 6f6f 7429 0272 1300 0000 724b 0000  _root).r....rK..
-00000f00: 0029 1072 1d00 0000 721e 0000 0072 1f00  .).r....r....r..
-00000f10: 0000 7220 0000 0072 4600 0000 7204 0000  ..r ...rF...r...
-00000f20: 0072 1000 0000 7230 0000 0072 1a00 0000  .r....r0...r....
-00000f30: 7247 0000 0072 4800 0000 da04 6469 6374  rG...rH.....dict
-00000f40: 7249 0000 0072 4a00 0000 da08 7072 6f70  rI...rJ.....prop
-00000f50: 6572 7479 7250 0000 0072 0e00 0000 720e  ertyrP...r....r.
-00000f60: 0000 0072 0e00 0000 720f 0000 0072 4400  ...r....r....rD.
-00000f70: 0000 6700 0000 7314 0000 000a 0008 020c  ..g...s.........
-00000f80: 0112 0112 0112 0112 010c 0102 0210 0172  ...............r
-00000f90: 4400 0000 7245 0000 0029 15da 0a5f 5f66  D...rE...)...__f
-00000fa0: 7574 7572 655f 5f72 0200 0000 720c 0000  uture__r....r...
-00000fb0: 00da 0b64 6174 6163 6c61 7373 6573 7203  ...dataclassesr.
-00000fc0: 0000 0072 0400 0000 da09 6675 6e63 746f  ...r......functo
-00000fd0: 6f6c 7372 0500 0000 da06 7479 7069 6e67  olsr......typing
-00000fe0: 7206 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
-00000ff0: 0900 0000 7210 0000 0072 1100 0000 7222  ....r....r....r"
-00001000: 0000 0072 2700 0000 7240 0000 0072 4400  ...r'...r@...rD.
-00001010: 0000 720b 0000 0072 4500 0000 720e 0000  ..r....rE...r...
-00001020: 0072 0e00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-00001030: da08 3c6d 6f64 756c 653e 0100 0000 7322  ..<module>....s"
-00001040: 0000 000c 0008 0210 010c 0118 0108 0302  ................
-00001050: 0410 0102 1410 0102 0810 0102 3412 0102  ............4...
-00001060: 0610 010e 15                             .....
+000006a0: 6503 640f 3c00 6403 5a0b 640e 6503 6410  e.d.<.d.Z.d.e.d.
+000006b0: 3c00 6403 5a0c 6411 6503 6412 3c00 6406  <.d.Z.d.e.d.<.d.
+000006c0: 5a0d 6407 6503 6413 3c00 6406 5a0e 6407  Z.d.e.d.<.d.Z.d.
+000006d0: 6503 6414 3c00 6415 5a0f 6416 6503 6417  e.d.<.d.Z.d.e.d.
+000006e0: 3c00 6406 5a10 6407 6503 6418 3c00 6406  <.d.Z.d.e.d.<.d.
+000006f0: 5a11 6407 6503 6419 3c00 641a 5a12 641b  Z.d.e.d.<.d.Z.d.
+00000700: 6503 641c 3c00 641d 641e 8400 5a13 6403  e.d.<.d.d...Z.d.
+00000710: 5300 291f da0e 4172 6775 6d65 6e74 5363  S.)...ArgumentSc
+00000720: 6865 6d61 7a0f 7374 7220 7c20 6c69 7374  hemaz.str | list
+00000730: 5b73 7472 5dda 046e 616d 654e 7a26 5479  [str]..nameNz&Ty
+00000740: 7065 5b41 6e79 5d20 7c20 5365 7175 656e  pe[Any] | Sequen
+00000750: 6365 5b54 7970 655b 416e 795d 5d20 7c20  ce[Type[Any]] | 
+00000760: 4e6f 6e65 da04 7479 7065 46da 0462 6f6f  None..typeF..boo
+00000770: 6cda 0872 6571 7569 7265 64fa 0a73 7472  l..required..str
+00000780: 207c 204e 6f6e 65da 0468 656c 70a9 01da   | None..help...
+00000790: 0f64 6566 6175 6c74 5f66 6163 746f 7279  .default_factory
+000007a0: 7a10 7374 7220 7c20 7475 706c 655b 7374  z.str | tuple[st
+000007b0: 725d da03 6b65 797a 204d 756c 7469 5661  r]..keyz MultiVa
+000007c0: 6c75 6550 6172 616d 4461 7461 207c 2041  lueParamData | A
+000007d0: 6e79 207c 204e 6f6e 65da 0764 6566 6175  ny | None..defau
+000007e0: 6c74 721b 0000 007a 1453 6571 7565 6e63  ltr....z.Sequenc
+000007f0: 655b 7374 725d 207c 204e 6f6e 6572 2300  e[str] | Noner#.
+00000800: 0000 da08 6d75 6c74 6970 6c65 da0b 6d75  ....multiple..mu
+00000810: 6c74 695f 7661 6c75 65e9 0100 0000 da03  lti_value.......
+00000820: 696e 74da 056e 6172 6773 da06 7365 6372  int..nargs..secr
+00000830: 6574 da09 7265 6164 5f6f 6e6c 79da 0072  et..read_only..r
+00000840: 0b00 0000 da0b 706c 6163 6568 6f6c 6465  ......placeholde
+00000850: 7263 0100 0000 0000 0000 0000 0000 0400  rc..............
+00000860: 0000 0400 0000 4300 0001 7332 0100 0074  ......C...s2...t
+00000870: 007c 006a 0174 0283 0273 0d74 02a0 037c  .|.j.t...s.t...|
+00000880: 006a 01a1 017c 005f 017c 006a 0464 0075  .j...|._.|.j.d.u
+00000890: 0072 177c 006a 017c 005f 046e 0d74 007c  .r.|.j.|._.n.t.|
+000008a0: 006a 0474 0283 0273 2474 02a0 037c 006a  .j.t...s$t...|.j
+000008b0: 04a1 017c 005f 0474 0567 017d 017c 006a  ...|._.t.g.}.|.j
+000008c0: 0673 2e7c 017c 005f 066e 5574 007c 006a  .s.|.|._.nUt.|.j
+000008d0: 0674 0783 0272 5e7c 006a 066a 0844 005d  .t...r^|.j.j.D.]
+000008e0: 0d7d 0274 007c 0274 0983 0272 457c 0267  .}.t.|.t...rE|.g
+000008f0: 017c 005f 0601 006e 1871 387c 006a 066a  .|._...n.q8|.j.j
+00000900: 0aa0 0ba1 0044 005d 0d7d 0374 007c 0374  .....D.].}.t.|.t
+00000910: 0983 0272 597c 0367 017c 005f 0601 006e  ...rY|.g.|._...n
+00000920: 0471 4c7c 017c 005f 066e 2574 007c 006a  .qL|.|._.n%t.|.j
+00000930: 0674 0983 0272 6a7c 006a 0667 017c 005f  .t...rj|.j.g.|._
+00000940: 066e 1974 0c7c 006a 0683 0164 016b 0272  .n.t.|.j...d.k.r
+00000950: 8374 007c 006a 0664 0219 0074 0d83 0272  .t.|.j.d...t...r
+00000960: 837c 006a 0664 0219 006a 0e7c 005f 0e7c  .|.j.d...j.|._.|
+00000970: 017c 005f 067c 006a 0e72 8f64 0364 0484  .|._.|.j.r.d.d..
+00000980: 007c 006a 0e44 0083 017c 005f 0e7c 006a  .|.j.D...|._.|.j
+00000990: 0f72 9764 057c 005f 1064 0053 0064 0053  .r.d.|._.d.S.d.S
+000009a0: 0029 064e 7234 0000 0072 0100 0000 6301  .).Nr4...r....c.
+000009b0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+000009c0: 0000 0053 0000 0173 1400 0000 6700 7c00  ...S...s....g.|.
+000009d0: 5d06 7d01 7400 7c01 8301 9102 7102 5300  ].}.t.|.....q.S.
+000009e0: 720e 0000 0029 0172 0b00 0000 2902 7217  r....).r....).r.
+000009f0: 0000 00da 0178 720e 0000 0072 0e00 0000  .....xr....r....
+00000a00: 720f 0000 0072 1900 0000 6000 0000 7302  r....r....`...s.
+00000a10: 0000 0014 007a 3041 7267 756d 656e 7453  .....z0ArgumentS
+00000a20: 6368 656d 612e 5f5f 706f 7374 5f69 6e69  chema.__post_ini
+00000a30: 745f 5f2e 3c6c 6f63 616c 733e 2e3c 6c69  t__.<locals>.<li
+00000a40: 7374 636f 6d70 3e54 2911 7215 0000 0072  stcomp>T).r....r
+00000a50: 3100 0000 7211 0000 0072 1c00 0000 721b  1...r....r....r.
+00000a60: 0000 0072 0b00 0000 7229 0000 0072 0500  ...r....r)...r..
+00000a70: 0000 da04 6172 6773 7209 0000 00da 066b  ....argsr......k
+00000a80: 7761 7267 7372 1200 0000 da03 6c65 6e72  wargsr......lenr
+00000a90: 2200 0000 7223 0000 0072 3300 0000 7232  "...r#...r3...r2
+00000aa0: 0000 0029 0472 2500 0000 5a0c 6465 6661  ...).r%...Z.defa
+00000ab0: 756c 745f 7479 7065 723b 0000 00da 0176  ult_typer;.....v
+00000ac0: 720e 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
+00000ad0: 2600 0000 3c00 0000 7340 0000 000c 010e  &...<...s@......
+00000ae0: 010a 020a 010c 010e 0106 0206 0208 010c  ................
+00000af0: 010c 040a 0108 0104 0102 fe10 040a 0108  ................
+00000b00: 0104 0102 fe06 0402 800c 010c 011e 010e  ................
+00000b10: 0206 0106 0212 0106 020a 0104 ff7a 1c41  .............z.A
+00000b20: 7267 756d 656e 7453 6368 656d 612e 5f5f  rgumentSchema.__
+00000b30: 706f 7374 5f69 6e69 745f 5f29 1472 1d00  post_init__).r..
+00000b40: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+00000b50: 0072 2900 0000 722b 0000 0072 2d00 0000  .r)...r+...r-...
+00000b60: 7204 0000 0072 1000 0000 7230 0000 0072  r....r....r0...r
+00000b70: 3100 0000 721b 0000 0072 2300 0000 7232  1...r....r#...r2
+00000b80: 0000 0072 3300 0000 7236 0000 0072 3700  ...r3...r6...r7.
+00000b90: 0000 7238 0000 0072 3a00 0000 7226 0000  ..r8...r:...r&..
+00000ba0: 0072 0e00 0000 720e 0000 0072 0e00 0000  .r....r....r....
+00000bb0: 720f 0000 0072 2700 0000 2b00 0000 7320  r....r'...+...s 
+00000bc0: 0000 000a 0008 020c 010c 010c 0112 010c  ................
+00000bd0: 010c 010c 010c 010c 010c 010c 010c 010c  ................
+00000be0: 010c 0272 2700 0000 6300 0000 0000 0000  ...r'...c.......
+00000bf0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00000c00: 0173 3200 0000 6500 5a01 6400 5a02 5500  .s2...e.Z.d.Z.U.
+00000c10: 6401 5a03 6402 6504 6403 3c00 6401 5a05  d.Z.d.e.d.<.d.Z.
+00000c20: 6402 6504 6404 3c00 6405 5a06 6406 6504  d.e.d.<.d.Z.d.e.
+00000c30: 6407 3c00 6405 5300 2908 da0c 4f70 7469  d.<.d.S.)...Opti
+00000c40: 6f6e 5363 6865 6d61 4672 2a00 0000 da07  onSchemaFr*.....
+00000c50: 6973 5f66 6c61 67da 0863 6f75 6e74 696e  is_flag..countin
+00000c60: 674e 7a10 6c69 7374 5b73 7472 5d20 7c20  gNz.list[str] | 
+00000c70: 4e6f 6e65 da0e 7365 636f 6e64 6172 795f  None..secondary_
+00000c80: 6f70 7473 2907 721d 0000 0072 1e00 0000  opts).r....r....
+00000c90: 721f 0000 0072 4100 0000 7220 0000 0072  r....rA...r ...r
+00000ca0: 4200 0000 7243 0000 0072 0e00 0000 720e  B...rC...r....r.
+00000cb0: 0000 0072 0e00 0000 720f 0000 0072 4000  ...r....r....r@.
+00000cc0: 0000 6600 0000 7308 0000 000a 000c 020c  ..f...s.........
+00000cd0: 0110 0172 4000 0000 6300 0000 0000 0000  ...r@...c.......
+00000ce0: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
+00000cf0: 0173 8400 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
+00000d00: 6401 6503 6402 3c00 6403 5a04 6404 6503  d.e.d.<.d.Z.d.e.
+00000d10: 6405 3c00 6505 6506 6406 8d01 5a07 6407  d.<.e.e.d...Z.d.
+00000d20: 6503 6408 3c00 6505 6508 6406 8d01 5a09  e.d.<.e.e.d...Z.
+00000d30: 6409 6503 640a 3c00 6505 6508 6406 8d01  d.e.d.<.e.e.d...
+00000d40: 5a0a 640b 6503 640c 3c00 6505 650b 6406  Z.d.e.d.<.e.e.d.
+00000d50: 8d01 5a0c 640d 6503 640e 3c00 6403 5a0d  ..Z.d.e.d.<.d.Z.
+00000d60: 640f 6503 6410 3c00 650e 6415 6413 6414  d.e.d.<.e.d.d.d.
+00000d70: 8404 8301 5a0f 6403 5300 2916 da0d 436f  ....Z.d.S.)...Co
+00000d80: 6d6d 616e 6453 6368 656d 61da 0b43 6f6d  mmandSchema..Com
+00000d90: 6d61 6e64 4e61 6d65 7228 0000 004e 722c  mandNamer(...Nr,
+00000da0: 0000 00da 0964 6f63 7374 7269 6e67 722e  .....docstringr.
+00000db0: 0000 0072 0b00 0000 7230 0000 007a 126c  ...r....r0...z.l
+00000dc0: 6973 745b 4f70 7469 6f6e 5363 6865 6d61  ist[OptionSchema
+00000dd0: 5dda 076f 7074 696f 6e73 7a14 6c69 7374  ]..optionsz.list
+00000de0: 5b41 7267 756d 656e 7453 6368 656d 615d  [ArgumentSchema]
+00000df0: da09 6172 6775 6d65 6e74 737a 2064 6963  ..argumentsz dic
+00000e00: 745b 436f 6d6d 616e 644e 616d 652c 2043  t[CommandName, C
+00000e10: 6f6d 6d61 6e64 5363 6865 6d61 5dda 0b73  ommandSchema]..s
+00000e20: 7562 636f 6d6d 616e 6473 7a14 436f 6d6d  ubcommandsz.Comm
+00000e30: 616e 6453 6368 656d 6120 7c20 4e6f 6e65  andSchema | None
+00000e40: da06 7061 7265 6e74 7213 0000 00fa 136c  ..parentr......l
+00000e50: 6973 745b 436f 6d6d 616e 6453 6368 656d  ist[CommandSchem
+00000e60: 615d 6301 0000 0000 0000 0000 0000 0003  a]c.............
+00000e70: 0000 0003 0000 0043 0000 0173 3400 0000  .......C...s4...
+00000e80: 7c00 7d01 7c00 6701 7d02 0900 7c01 6a00  |.}.|.g.}...|.j.
+00000e90: 7d01 7c01 6400 7500 720e 6e06 7c02 a001  }.|.d.u.r.n.|...
+00000ea0: 7c01 a101 0100 7106 7402 7403 7c02 8301  |.....q.t.t.|...
+00000eb0: 8301 5300 2901 4e29 0472 4a00 0000 da06  ..S.).N).rJ.....
+00000ec0: 6170 7065 6e64 721a 0000 00da 0872 6576  appendr......rev
+00000ed0: 6572 7365 6429 0372 2500 0000 da04 6e6f  ersed).r%.....no
+00000ee0: 6465 da04 7061 7468 720e 0000 0072 0e00  de..pathr....r..
+00000ef0: 0000 720f 0000 00da 0e70 6174 685f 6672  ..r......path_fr
+00000f00: 6f6d 5f72 6f6f 7477 0000 0073 1200 0000  om_rootw...s....
+00000f10: 0402 0601 0201 0601 0801 0201 0a01 02fc  ................
+00000f20: 0c05 7a1c 436f 6d6d 616e 6453 6368 656d  ..z.CommandSchem
+00000f30: 612e 7061 7468 5f66 726f 6d5f 726f 6f74  a.path_from_root
+00000f40: 2902 7213 0000 0072 4b00 0000 2910 721d  ).r....rK...).r.
+00000f50: 0000 0072 1e00 0000 721f 0000 0072 2000  ...r....r....r .
+00000f60: 0000 7246 0000 0072 0400 0000 7210 0000  ..rF...r....r...
+00000f70: 0072 3000 0000 721a 0000 0072 4700 0000  .r0...r....rG...
+00000f80: 7248 0000 00da 0464 6963 7472 4900 0000  rH.....dictrI...
+00000f90: 724a 0000 00da 0870 726f 7065 7274 7972  rJ.....propertyr
+00000fa0: 5000 0000 720e 0000 0072 0e00 0000 720e  P...r....r....r.
+00000fb0: 0000 0072 0f00 0000 7244 0000 006d 0000  ...r....rD...m..
+00000fc0: 0073 1400 0000 0a00 0802 0c01 1201 1201  .s..............
+00000fd0: 1201 1201 0c01 0202 1001 7244 0000 0072  ..........rD...r
+00000fe0: 4500 0000 2915 da0a 5f5f 6675 7475 7265  E...)...__future
+00000ff0: 5f5f 7202 0000 0072 0c00 0000 da0b 6461  __r....r......da
+00001000: 7461 636c 6173 7365 7372 0300 0000 7204  taclassesr....r.
+00001010: 0000 00da 0966 756e 6374 6f6f 6c73 7205  .....functoolsr.
+00001020: 0000 00da 0674 7970 696e 6772 0600 0000  .....typingr....
+00001030: 7207 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
+00001040: 1000 0000 7211 0000 0072 2200 0000 7227  ....r....r"...r'
+00001050: 0000 0072 4000 0000 7244 0000 0072 0b00  ...r@...rD...r..
+00001060: 0000 7245 0000 0072 0e00 0000 720e 0000  ..rE...r....r...
+00001070: 0072 0e00 0000 720f 0000 00da 083c 6d6f  .r....r......<mo
+00001080: 6475 6c65 3e01 0000 0073 2200 0000 0c00  dule>....s".....
+00001090: 0802 1001 0c01 1801 0803 0204 1001 0214  ................
+000010a0: 1001 0208 1001 023a 1201 0206 1001 0e15  .......:........
```

### Comparing `argparse-tui-0.1.3/src/argparse_tui/__pycache__/tui.cpython-310.pyc` & `argparse-tui-0.2.0/src/argparse_tui/__pycache__/tui.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 04:37:17 2023 UTC, .py size: 12871 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 fd45 c364 4732 0000  o........E.dG2..
+00000000: 6f0d 0d0a 0000 0000 0f82 c564 5932 0000  o..........dY2..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 a401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6400 6403 6c05 6d06 5a06 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d07 5a07 0100 6400 6405 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 5a09 0100 6400 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
@@ -74,16 +74,16 @@
 00000490: 5464 3d64 3e84 0483 015a 1165 0e65 126a  Td=d>....Z.e.e.j
 000004a0: 1383 0164 5564 4064 4184 0483 015a 1464  ...dUd@dA....Z.d
 000004b0: 5664 4364 4484 045a 1564 5764 4964 4a84  VdCdD..Z.dWdIdJ.
 000004c0: 045a 1664 5664 4b64 4c84 045a 1787 0004  .Z.dVdKdL..Z....
 000004d0: 005a 1853 0029 58da 0e43 6f6d 6d61 6e64  .Z.S.)X..Command
 000004e0: 4275 696c 6465 723e 0300 0000 fa13 636f  Builder>......co
 000004f0: 6d6d 616e 642d 6e61 6d65 2d73 796e 7461  mmand-name-synta
-00000500: 78fa 0e76 6572 7369 6f6e 2d73 7472 696e  x..version-strin
-00000510: 67da 0670 726f 6d70 747a 0663 7472 6c2b  g..promptz.ctrl+
+00000500: 78da 0670 726f 6d70 74fa 0e76 6572 7369  x..prompt..versi
+00000510: 6f6e 2d73 7472 696e 677a 0663 7472 6c2b  on-stringz.ctrl+
 00000520: 725a 0d63 6c6f 7365 5f61 6e64 5f72 756e  rZ.close_and_run
 00000530: 7a0b 5275 6e20 436f 6d6d 616e 6429 03da  z.Run Command)..
 00000540: 036b 6579 da06 6163 7469 6f6e da0b 6465  .key..action..de
 00000550: 7363 7269 7074 696f 6e7a 0663 7472 6c2b  scriptionz.ctrl+
 00000560: 795a 1363 6f70 795f 636f 6d6d 616e 645f  yZ.copy_command_
 00000570: 7374 7269 6e67 7a0c 436f 7079 2043 6f6d  stringz.Copy Com
 00000580: 6d61 6e64 7a0d 6374 726c 2b74 2c65 7363  mandz.ctrl+t,esc
@@ -144,15 +144,15 @@
 000008f0: 640d 8301 640f 6408 8d02 7d07 640a 7c07  d...d.d...}.d.|.
 00000900: 5f0e 7c07 5600 0100 740d 7411 740f 640d  _.|.V...t.t.t.d.
 00000910: 6410 6408 8d02 6411 6408 8d02 6412 6408  d.d...d.d...d.d.
 00000920: 8d02 5600 0100 5700 6400 0400 0400 8303  ..V...W.d.......
 00000930: 0100 6e08 3100 7391 7701 0100 0100 0100  ..n.1.s.w.......
 00000940: 5900 0100 7412 8300 5600 0100 6400 5300  Y...t...V...d.S.
 00000950: 2913 4e5a 0843 6f6d 6d61 6e64 73da 0162  ).NZ.Commands..b
-00000960: 2901 da05 7374 796c 6572 2b00 0000 da01  )...styler+.....
+00000960: 2901 da05 7374 796c 6572 2c00 0000 da01  )...styler,.....
 00000970: 0ada 0176 7a13 686f 6d65 2d63 6f6d 6d61  ...vz.home-comma
 00000980: 6e64 732d 6c61 6265 6c29 0172 3d00 0000  nds-label).r=...
 00000990: 7a0c 686f 6d65 2d73 6964 6562 6172 467a  z.home-sidebarFz
 000009a0: 0968 6f6d 652d 626f 6479 7a22 686f 6d65  .home-bodyz"home
 000009b0: 2d63 6f6d 6d61 6e64 2d64 6573 6372 6970  -command-descrip
 000009c0: 7469 6f6e 2d63 6f6e 7461 696e 6572 da00  tion-container..
 000009d0: 7a18 686f 6d65 2d63 6f6d 6d61 6e64 2d64  z.home-command-d
@@ -385,15 +385,15 @@
 00001800: 6602 7c06 a102 7d08 7c00 a007 6406 7408  f.|...}.|...d.t.
 00001810: a102 a009 7c08 a101 0100 6401 5300 6401  ....|.....d.S.d.
 00001820: 5300 2907 7a40 5570 6461 7465 2074 6865  S.).z@Update the
 00001830: 2070 7265 7669 6577 2062 6f78 2073 686f   preview box sho
 00001840: 7769 6e67 2074 6865 2063 6f6d 6d61 6e64  wing the command
 00001850: 2073 7472 696e 6720 746f 2062 6520 6578   string to be ex
 00001860: 6563 7574 6564 4e72 2a00 0000 7266 0000  ecutedNr*...rf..
-00001870: 0072 2c00 0000 7a02 2420 7a19 2368 6f6d  .r,...z.$ z.#hom
+00001870: 0072 2b00 0000 7a02 2420 7a19 2368 6f6d  .r+...z.$ z.#hom
 00001880: 652d 6578 6563 2d70 7265 7669 6577 2d73  e-exec-preview-s
 00001890: 7461 7469 6329 0a72 4200 0000 7250 0000  tatic).rB...rP..
 000018a0: 0072 0b00 0000 7236 0000 0072 5b00 0000  .r....r6...r[...
 000018b0: 7252 0000 0072 4400 0000 7280 0000 0072  rR...rD...r....r
 000018c0: 1a00 0000 728f 0000 0029 0972 4500 0000  ....r....).rE...
 000018d0: 7290 0000 0072 4200 0000 5a19 636f 6d6d  r....rB...Z.comm
 000018e0: 616e 645f 6e61 6d65 5f73 796e 7461 785f  and_name_syntax_
@@ -463,280 +463,279 @@
 00001ce0: 0102 0102 0102 0102 0104 fd0c 050c 010c  ................
 00001cf0: 010c 0104 f502 1402 0102 0110 f80a 140a  ................
 00001d00: 330a 070a 170a 030a 050c 0308 100c 0108  3...............
 00001d10: 080c 010a 070a 0912 1172 2900 0000 6300  .........r)...c.
 00001d20: 0000 0000 0000 0000 0000 0000 0000 0005  ................
 00001d30: 0000 0000 0000 0173 9200 0000 6500 5a01  .......s....e.Z.
 00001d40: 6400 5a02 6503 6504 8301 6a05 6401 1b00  d.Z.e.e...j.d...
-00001d50: 5a06 0902 0902 6429 642a 8700 6601 640b  Z.....d)d*..f.d.
-00001d60: 640c 840d 5a07 6508 642b 6410 6411 8404  d...Z.e.d+d.d...
-00001d70: 8301 5a09 6412 6413 8400 5a0a 650b 650c  ..Z.d.d...Z.e.e.
-00001d80: 6a0d 6414 8302 6415 6416 8400 8301 5a0e  j.d...d.d.....Z.
-00001d90: 6417 6402 6402 6418 9c03 642c 8700 6601  d.d.d.d...d,..f.
-00001da0: 641f 6420 840e 5a0f 642d 6421 6422 8404  d.d ..Z.d-d!d"..
-00001db0: 5a10 642d 6423 6424 8404 5a11 642e 6427  Z.d-d#d$..Z.d.d'
-00001dc0: 6428 8404 5a12 8700 0400 5a13 5300 292f  d(..Z.....Z.S.)/
+00001d50: 5a06 0902 0902 6428 6429 8700 6601 640b  Z.....d(d)..f.d.
+00001d60: 640c 840d 5a07 6508 642a 640f 6410 8404  d...Z.e.d*d.d...
+00001d70: 8301 5a09 6411 6412 8400 5a0a 650b 650c  ..Z.d.d...Z.e.e.
+00001d80: 6a0d 6413 8302 6414 6415 8400 8301 5a0e  j.d...d.d.....Z.
+00001d90: 6416 6402 6402 6417 9c03 642b 8700 6601  d.d.d.d...d+..f.
+00001da0: 641e 641f 840e 5a0f 642c 6420 6421 8404  d.d...Z.d,d d!..
+00001db0: 5a10 642c 6422 6423 8404 5a11 642d 6426  Z.d,d"d#..Z.d-d&
+00001dc0: 6427 8404 5a12 8700 0400 5a13 5300 292e  d'..Z.....Z.S.).
 00001dd0: da03 5475 697a 0874 7569 2e73 6373 734e  ..Tuiz.tui.scssN
 00001de0: 7234 0000 0072 3500 0000 7236 0000 0072  r4...r5...r6...r
 00001df0: 3900 0000 7238 0000 00da 0e63 6f6d 6d61  9...r8.....comma
 00001e00: 6e64 5f66 696c 7465 7272 4a00 0000 7258  nd_filterrJ...rX
 00001e10: 0000 0063 0500 0000 0000 0000 0000 0000  ...c............
-00001e20: 0700 0000 0800 0000 0300 0001 7312 0100  ............s...
+00001e20: 0700 0000 0800 0000 0300 0001 7316 0100  ............s...
 00001e30: 0074 0083 00a0 01a1 0001 0067 007c 005f  .t.........g.|._
 00001e40: 0264 017c 005f 0374 047c 01a0 05a1 0083  .d.|._.t.|......
-00001e50: 0164 0219 007d 0588 0072 497c 017c 0519  .d...}...rI|.|..
-00001e60: 006a 0672 4987 0066 0164 0364 0484 087c  .j.rI..f.d.d...|
+00001e50: 0164 0219 007d 0588 0072 4b7c 017c 0519  .d...}...rK|.|..
+00001e60: 006a 0672 4b87 0066 0164 0364 0484 087c  .j.rK..f.d.d...|
 00001e70: 017c 0519 006a 06a0 07a1 0044 0083 017d  .|...j.....D...}
 00001e80: 0674 087c 0683 0164 056b 0272 4474 0987  .t.|...d.k.rDt..
 00001e90: 0066 0164 0664 0784 0864 0844 0083 0183  .f.d.d...d.D....
 00001ea0: 0173 447c 067d 0174 047c 01a0 05a1 0083  .sD|.}.t.|......
-00001eb0: 0164 0219 007d 056e 057c 067c 017c 0519  .d...}.n.|.|.|..
-00001ec0: 005f 067c 017c 005f 0a74 0964 0964 0784  ._.|.|._.t.d.d..
-00001ed0: 007c 01a0 0ba1 0044 0083 0183 017c 005f  .|.....D.....|._
-00001ee0: 0c64 0a7c 005f 0d7c 0272 5f7c 026e 0274  .d.|._.|.r_|.n.t
-00001ef0: 0e83 007c 005f 0f7c 037c 005f 107c 006a  ...|._.|.|._.|.j
-00001f00: 1073 8774 1174 1283 018f 1001 0074 13a0  .s.t.t.......t..
-00001f10: 147c 006a 0fa1 017c 005f 1057 0064 0004  .|.j...|._.W.d..
-00001f20: 0004 0083 0301 0064 0053 0031 0073 8077  .......d.S.1.s.w
-00001f30: 0101 0001 0001 0059 0001 0064 0053 0064  .......Y...d.S.d
-00001f40: 0053 0029 0b4e 724f 0000 0072 0100 0000  .S.).NrO...r....
-00001f50: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00001f60: 0005 0000 0013 0000 0173 2000 0000 6900  .........s ...i.
-00001f70: 7c00 5d0c 5c02 7d01 7d02 7400 7c01 8800  |.].\.}.}.t.|...
-00001f80: 8302 7202 7c01 7c02 9302 7102 5300 7248  ..r.|.|...q.S.rH
-00001f90: 0000 0072 0400 0000 2903 726a 0000 00da  ...r....).rj....
-00001fa0: 016b 724e 0000 00a9 0172 9c00 0000 7248  .krN.....r....rH
-00001fb0: 0000 0072 4900 0000 da0a 3c64 6963 7463  ...rI.....<dictc
-00001fc0: 6f6d 703e 0401 0000 730c 0000 0006 0006  omp>....s.......
-00001fd0: 0208 0102 fd04 0106 ff7a 2054 7569 2e5f  .........z Tui._
-00001fe0: 5f69 6e69 745f 5f2e 3c6c 6f63 616c 733e  _init__.<locals>
-00001ff0: 2e3c 6469 6374 636f 6d70 3e72 1d00 0000  .<dictcomp>r....
-00002000: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00002010: 0003 0000 0033 0000 0173 1800 0000 8100  .....3...s......
-00002020: 7c00 5d07 7d01 7c01 8800 7600 5600 0100  |.].}.|...v.V...
-00002030: 7102 6400 5300 723f 0000 0072 4800 0000  q.d.S.r?...rH...
-00002040: 7269 0000 0072 9e00 0000 7248 0000 0072  ri...r....rH...r
-00002050: 4900 0000 726c 0000 0009 0100 0073 0800  I...rl.......s..
-00002060: 0000 0280 0400 0801 0aff 7a1f 5475 692e  ..........z.Tui.
-00002070: 5f5f 696e 6974 5f5f 2e3c 6c6f 6361 6c73  __init__.<locals
-00002080: 3e2e 3c67 656e 6578 7072 3e29 02da 012a  >.<genexpr>)...*
-00002090: fa01 3f63 0100 0000 0000 0000 0000 0000  ..?c............
-000020a0: 0200 0000 0200 0000 7300 0001 7316 0000  ........s...s...
-000020b0: 0081 007c 005d 067d 017c 016a 0056 0001  ...|.].}.|.j.V..
-000020c0: 0071 0264 0053 0072 3f00 0000 2901 da0b  .q.d.S.r?...)...
-000020d0: 7375 6263 6f6d 6d61 6e64 7329 0272 6a00  subcommands).rj.
-000020e0: 0000 724e 0000 0072 4800 0000 7248 0000  ..rN...rH...rH..
-000020f0: 0072 4900 0000 726c 0000 0013 0100 0073  .rI...rl.......s
-00002100: 0400 0000 0280 1400 4629 1572 4000 0000  ........F).r@...
-00002110: 7241 0000 0072 5f00 0000 725d 0000 00da  rA...r_...r]....
-00002120: 046c 6973 74da 046b 6579 7372 a200 0000  .list..keysr....
-00002130: da05 6974 656d 73da 036c 656e da03 616e  ..items..len..an
-00002140: 7972 3400 0000 da06 7661 6c75 6573 723a  yr4.....valuesr:
-00002150: 0000 0072 6000 0000 721e 0000 0072 3600  ...r`...r....r6.
-00002160: 0000 7238 0000 0072 0300 0000 da09 4578  ..r8...r......Ex
-00002170: 6365 7074 696f 6e72 2800 0000 7243 0000  ceptionr(...rC..
-00002180: 0029 0772 4500 0000 7234 0000 0072 3600  .).rE...r4...r6.
-00002190: 0000 7238 0000 0072 9c00 0000 da0d 726f  ..r8...r......ro
-000021a0: 6f74 5f63 6d64 5f6e 616d 655a 106d 6174  ot_cmd_nameZ.mat
-000021b0: 6368 696e 675f 7363 6865 6d61 7372 4600  ching_schemasrF.
-000021c0: 0000 729e 0000 0072 4900 0000 7241 0000  ..r....rI...rA..
-000021d0: 00f6 0000 0073 3000 0000 0a07 0602 0601  .....s0.........
-000021e0: 1002 0e01 0a01 0c02 06fe 1805 0201 08ff  ................
-000021f0: 0403 1201 0a03 0602 1801 0601 1002 0601  ................
-00002200: 0602 0a01 1001 22ff 04ff 7a0c 5475 692e  ......"...z.Tui.
-00002210: 5f5f 696e 6974 5f5f da04 6172 6773 7221  __init__..argsr!
-00002220: 0000 00fa 0527 5475 6927 6301 0000 0000  .....'Tui'c.....
-00002230: 0000 0000 0000 0006 0000 0004 0000 004f  ...............O
-00002240: 0000 0173 5200 0000 7c01 7306 7400 6401  ...sR...|.s.t.d.
-00002250: 8301 8201 7c01 6402 1900 7d03 7c03 6a01  ....|.d...}.|.j.
-00002260: 7c03 6901 7d04 7c01 6403 6400 8502 1900  |.i.}.|.d.d.....
-00002270: 4400 5d0b 7d05 7c03 7c05 5f02 7c05 7c03  D.].}.|.|._.|.|.
-00002280: 6a03 7c05 6a01 3c00 7115 7c00 7c04 6601  j.|.j.<.q.|.|.f.
-00002290: 6900 7c02 a401 8e01 5300 2904 4e7a 144e  i.|.....S.).Nz.N
-000022a0: 6f20 7363 6865 6d61 7320 7072 6f76 6964  o schemas provid
-000022b0: 6564 2e72 0100 0000 721d 0000 0029 04da  ed.r....r....)..
-000022c0: 0a56 616c 7565 4572 726f 7272 3c00 0000  .ValueErrorr<...
-000022d0: 7294 0000 0072 a200 0000 2906 da03 636c  r....r....)...cl
-000022e0: 7372 ab00 0000 da06 6b77 6172 6773 5a0b  sr......kwargsZ.
-000022f0: 726f 6f74 5f73 6368 656d 61da 0773 6368  root_schema..sch
-00002300: 656d 6173 5a06 7363 6865 6d61 7248 0000  emasZ.schemarH..
-00002310: 0072 4800 0000 7249 0000 00da 0c66 726f  .rH...rI.....fro
-00002320: 6d5f 7363 6865 6d61 731d 0100 0073 1000  m_schemas....s..
-00002330: 0000 0402 0801 0802 0a02 1002 0601 0e01  ................
-00002340: 1002 7a10 5475 692e 6672 6f6d 5f73 6368  ..z.Tui.from_sch
-00002350: 656d 6173 6301 0000 0000 0000 0000 0000  emasc...........
-00002360: 0001 0000 0008 0000 0043 0000 0173 2200  .........C...s".
-00002370: 0000 7c00 a000 7401 7c00 6a02 7c00 6a03  ..|...t.|.j.|.j.
-00002380: 7c00 6a04 7c00 6a05 6401 8d04 a101 0100  |.j.|.j.d.......
-00002390: 6400 5300 2902 4e29 0372 3600 0000 7238  d.S.).N).r6...r8
-000023a0: 0000 0072 3a00 0000 2906 7277 0000 0072  ...r:...).rw...r
-000023b0: 2900 0000 7234 0000 0072 3600 0000 7238  )...r4...r6...r8
-000023c0: 0000 0072 3a00 0000 7261 0000 0072 4800  ...r:...ra...rH.
-000023d0: 0000 7248 0000 0072 4900 0000 727d 0000  ..rH...rI...r}..
-000023e0: 002c 0100 0073 1000 0000 0401 0201 0401  .,...s..........
-000023f0: 0401 0401 0401 04fc 08ff 7a0c 5475 692e  ..........z.Tui.
-00002400: 6f6e 5f6d 6f75 6e74 7a11 2368 6f6d 652d  on_mountz.#home-
-00002410: 6578 6563 2d62 7574 746f 6e63 0100 0000  exec-buttonc....
-00002420: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00002430: 4300 0001 7312 0000 0064 017c 005f 007c  C...s....d.|._.|
-00002440: 00a0 01a1 0001 0064 0053 0072 5900 0000  .......d.S.rY...
-00002450: 2902 7260 0000 0072 3200 0000 7261 0000  ).r`...r2...ra..
-00002460: 0072 4800 0000 7248 0000 0072 4900 0000  .rH...rH...rI...
-00002470: da11 6f6e 5f62 7574 746f 6e5f 7072 6573  ..on_button_pres
-00002480: 7365 6436 0100 0073 0400 0000 0602 0c01  sed6...s........
-00002490: 7a15 5475 692e 6f6e 5f62 7574 746f 6e5f  z.Tui.on_button_
-000024a0: 7072 6573 7365 6446 a903 da08 6865 6164  pressedF....head
-000024b0: 6c65 7373 da04 7369 7a65 da0a 6175 746f  less..size..auto
-000024c0: 5f70 696c 6f74 72b4 0000 0072 3b00 0000  _pilotr....r;...
-000024d0: 72b5 0000 00fa 1674 7570 6c65 5b69 6e74  r......tuple[int
-000024e0: 2c20 696e 745d 207c 204e 6f6e 6572 b600  , int] | Noner..
-000024f0: 0000 fa1c 4175 746f 7069 6c6f 7443 616c  ....AutopilotCal
-00002500: 6c62 6163 6b54 7970 6520 7c20 4e6f 6e65  lbackType | None
-00002510: 6301 0000 0000 0000 0003 0000 0009 0000  c...............
-00002520: 000d 0000 0003 0000 0173 4201 0000 7a57  .........sB...zW
-00002530: 7400 8300 6a01 7c01 7c02 7c03 6401 8d03  t...j.|.|.|.d...
-00002540: 0100 5700 7c00 6a02 7252 7403 8300 7d04  ..W.|.j.rRt...}.
-00002550: 7c00 6a02 7254 7c00 6a04 7256 7c04 a005  |.j.rT|.j.rV|...
-00002560: 6402 7c00 6a06 9b00 6403 7c00 6a07 9b00  d.|.j...d.|.j...
-00002570: 6404 9d05 a101 0100 7408 a009 7c00 6a06  d.......t...|.j.
-00002580: a101 7d05 7c05 6405 1900 7d06 6700 7c05  ..}.|.d...}.g.|.
-00002590: a201 7c00 6a02 a201 7d07 740a 6a0b a00c  ..|.j...}.t.j...
-000025a0: a100 7d08 740a 6a0d a00e 740a a00f a100  ..}.t.j...t.....
-000025b0: 7c08 6406 1900 6702 a101 7c08 6406 3c00  |.d...g...|.d.<.
-000025c0: 740a a010 7c06 7c07 7c08 a103 0100 6400  t...|.|.|.....d.
-000025d0: 5300 6400 5300 6400 5300 6400 5300 7c00  S.d.S.d.S.d.S.|.
-000025e0: 6a02 729e 7403 8300 7d04 7c00 6a02 729f  j.r.t...}.|.j.r.
-000025f0: 7c00 6a04 72a0 7c04 a005 6402 7c00 6a06  |.j.r.|...d.|.j.
-00002600: 9b00 6403 7c00 6a07 9b00 6404 9d05 a101  ..d.|.j...d.....
-00002610: 0100 7408 a009 7c00 6a06 a101 7d05 7c05  ..t...|.j...}.|.
-00002620: 6405 1900 7d06 6700 7c05 a201 7c00 6a02  d...}.g.|...|.j.
-00002630: a201 7d07 740a 6a0b a00c a100 7d08 740a  ..}.t.j.....}.t.
-00002640: 6a0d a00e 740a a00f a100 7c08 6406 1900  j...t.....|.d...
-00002650: 6702 a101 7c08 6406 3c00 740a a010 7c06  g...|.d.<.t...|.
-00002660: 7c07 7c08 a103 0100 7700 7700 7700 7700  |.|.....w.w.w.w.
-00002670: 2907 4e72 b300 0000 7a10 5275 6e6e 696e  ).Nr....z.Runnin
-00002680: 6720 5b62 2063 7961 6e5d 7266 0000 007a  g [b cyan]rf...z
-00002690: 035b 2f5d 7201 0000 00da 0450 4154 4829  .[/]r......PATH)
-000026a0: 1172 4000 0000 7207 0000 0072 5f00 0000  .r@...r....r_...
-000026b0: 7209 0000 0072 6000 0000 da05 7072 696e  r....r`.....prin
-000026c0: 7472 3600 0000 725d 0000 0072 6700 0000  tr6...r]...rg...
-000026d0: da05 7370 6c69 74da 026f 73da 0765 6e76  ..split..os..env
-000026e0: 6972 6f6e 7264 0000 00da 0770 6174 6873  ironrd.....paths
-000026f0: 6570 7273 0000 00da 0667 6574 6377 64da  eprs.....getcwd.
-00002700: 0765 7865 6376 7065 2909 7245 0000 0072  .execvpe).rE...r
-00002710: b400 0000 72b5 0000 0072 b600 0000 da07  ....r....r......
-00002720: 636f 6e73 6f6c 655a 0e73 706c 6974 5f61  consoleZ.split_a
-00002730: 7070 5f6e 616d 655a 0c70 726f 6772 616d  pp_nameZ.program
-00002740: 5f6e 616d 65da 0961 7267 756d 656e 7473  _name..arguments
-00002750: da03 656e 7672 4600 0000 7248 0000 0072  ..envrF...rH...r
-00002760: 4900 0000 7207 0000 003b 0100 0073 3c00  I...r....;...s<.
-00002770: 0000 0207 1401 0602 0601 0c01 0401 1401  ................
-00002780: 04ff 0c04 0801 0e01 0a02 1c01 1201 04f3  ................
-00002790: 0802 06fe 0601 0c01 0401 1401 04ff 0c04  ................
-000027a0: 0801 0e01 0a02 1c01 1001 02f3 0402 7a07  ..............z.
-000027b0: 5475 692e 7275 6e63 0100 0000 0000 0000  Tui.runc........
-000027c0: 0000 0000 0200 0000 0800 0000 4300 0001  ............C...
-000027d0: 7330 0000 007a 077c 00a0 0074 01a1 017d  s0...z.|...t...}
-000027e0: 0157 006e 0a04 0074 0279 1101 0001 0001  .W.n...t.y......
-000027f0: 0059 0064 0053 0077 007c 01a0 03a1 0001  .Y.d.S.w.|......
-00002800: 0064 0053 0072 3f00 0000 2904 7280 0000  .d.S.r?...).r...
-00002810: 0072 2300 0000 7215 0000 0072 5300 0000  .r#...r....rS...
-00002820: 2902 7245 0000 0072 8600 0000 7248 0000  ).rE...r....rH..
-00002830: 0072 4800 0000 7249 0000 00da 1961 6374  .rH...rI.....act
-00002840: 696f 6e5f 666f 6375 735f 636f 6d6d 616e  ion_focus_comman
-00002850: 645f 7472 6565 5401 0000 730c 0000 0002  d_treeT...s.....
-00002860: 010e 010c 0106 0102 ff0c 037a 1d54 7569  ...........z.Tui
-00002870: 2e61 6374 696f 6e5f 666f 6375 735f 636f  .action_focus_co
-00002880: 6d6d 616e 645f 7472 6565 6301 0000 0000  mmand_treec.....
-00002890: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-000028a0: 0000 0173 1e00 0000 7c00 a000 7401 a101  ...s....|...t...
-000028b0: 7d01 7c00 a002 7403 7c01 6a04 8301 a101  }.|...t.|.j.....
-000028c0: 0100 6400 5300 723f 0000 0029 0572 8000  ..d.S.r?...).r..
-000028d0: 0000 7229 0000 0072 7700 0000 7222 0000  ..r)...rw...r"..
-000028e0: 0072 8200 0000 2902 7245 0000 005a 0f63  .r....).rE...Z.c
-000028f0: 6f6d 6d61 6e64 5f62 7569 6c64 6572 7248  ommand_builderrH
-00002900: 0000 0072 4800 0000 7249 0000 00da 1861  ...rH...rI.....a
-00002910: 6374 696f 6e5f 7368 6f77 5f63 6f6d 6d61  ction_show_comma
-00002920: 6e64 5f69 6e66 6f5c 0100 0073 0400 0000  nd_info\...s....
-00002930: 0a01 1401 7a1c 5475 692e 6163 7469 6f6e  ....z.Tui.action
-00002940: 5f73 686f 775f 636f 6d6d 616e 645f 696e  _show_command_in
-00002950: 666f da03 7572 6c72 3700 0000 6302 0000  fo..urlr7...c...
-00002960: 0000 0000 0000 0000 0002 0000 0002 0000  ................
-00002970: 0043 0000 0173 0c00 0000 7400 7c01 8301  .C...s....t.|...
-00002980: 0100 6401 5300 2902 7a69 5669 7369 7420  ..d.S.).ziVisit 
-00002990: 7468 6520 6769 7665 6e20 5552 4c2c 2076  the given URL, v
-000029a0: 6961 2074 6865 206f 7065 7261 7469 6e67  ia the operating
-000029b0: 2073 7973 7465 6d2e 0a0a 2020 2020 2020   system...      
-000029c0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-000029d0: 2020 2020 7572 6c3a 2054 6865 2055 524c      url: The URL
-000029e0: 2074 6f20 7669 7369 742e 0a20 2020 2020   to visit..     
-000029f0: 2020 204e 2901 da08 6f70 656e 5f75 726c     N)...open_url
-00002a00: 2902 7245 0000 0072 c600 0000 7248 0000  ).rE...r....rH..
-00002a10: 0072 4800 0000 7249 0000 00da 0c61 6374  .rH...rI.....act
-00002a20: 696f 6e5f 7669 7369 7460 0100 0073 0200  ion_visit`...s..
-00002a30: 0000 0c06 7a10 5475 692e 6163 7469 6f6e  ....z.Tui.action
-00002a40: 5f76 6973 6974 2902 4e4e 290a 7234 0000  _visit).NN).r4..
-00002a50: 0072 3500 0000 7236 0000 0072 3900 0000  .r5...r6...r9...
-00002a60: 7238 0000 0072 3900 0000 729c 0000 0072  r8...r9...r....r
-00002a70: 3900 0000 724a 0000 0072 5800 0000 2904  9...rJ...rX...).
-00002a80: 72ab 0000 0072 2100 0000 724a 0000 0072  r....r!...rJ...r
-00002a90: ac00 0000 2908 72b4 0000 0072 3b00 0000  ....).r....r;...
-00002aa0: 72b5 0000 0072 b700 0000 72b6 0000 0072  r....r....r....r
-00002ab0: b800 0000 724a 0000 0072 5800 0000 7296  ....rJ...rX...r.
-00002ac0: 0000 0029 0472 c600 0000 7237 0000 0072  ...).r....r7...r
-00002ad0: 4a00 0000 7258 0000 0029 1472 9700 0000  J...rX...).r....
-00002ae0: 7298 0000 0072 9900 0000 7206 0000 00da  r....r....r.....
-00002af0: 085f 5f66 696c 655f 5f72 9400 0000 5a08  .__file__r....Z.
-00002b00: 4353 535f 5041 5448 7241 0000 00da 0b63  CSS_PATHrA.....c
-00002b10: 6c61 7373 6d65 7468 6f64 72b1 0000 0072  lassmethodr....r
-00002b20: 7d00 0000 720d 0000 0072 1700 0000 5a07  }...r....r....Z.
-00002b30: 5072 6573 7365 6472 b200 0000 7207 0000  Pressedr....r...
-00002b40: 0072 c400 0000 72c5 0000 0072 c800 0000  .r....r....r....
-00002b50: 729a 0000 0072 4800 0000 7248 0000 0072  r....rH...rH...r
-00002b60: 4600 0000 7249 0000 0072 9b00 0000 f300  F...rI...r......
-00002b70: 0000 7322 0000 0008 000e 0102 0602 0110  ..s"............
-00002b80: fb02 270c 0108 0e0a 0a0a 0102 0702 0102  ..'.............
-00002b90: 0112 fb0a 190a 0812 0472 9b00 0000 2942  .........r....)B
-00002ba0: da0a 5f5f 6675 7475 7265 5f5f 7202 0000  ..__future__r...
-00002bb0: 0072 bc00 0000 7267 0000 0072 7000 0000  .r....rg...rp...
-00002bc0: da0a 636f 6e74 6578 746c 6962 7203 0000  ..contextlibr...
-00002bd0: 0072 0500 0000 da07 7061 7468 6c69 6272  .r......pathlibr
-00002be0: 0600 0000 da0a 7375 6270 726f 6365 7373  ......subprocess
-00002bf0: 7207 0000 005a 0a77 6562 6272 6f77 7365  r....Z.webbrowse
-00002c00: 7272 0800 0000 72c7 0000 005a 0c72 6963  rr....r....Z.ric
-00002c10: 682e 636f 6e73 6f6c 6572 0900 0000 5a10  h.consoler....Z.
-00002c20: 7269 6368 2e68 6967 686c 6967 6874 6572  rich.highlighter
-00002c30: 720a 0000 005a 0972 6963 682e 7465 7874  r....Z.rich.text
-00002c40: 720b 0000 005a 0774 6578 7475 616c 720c  r....Z.textualr.
-00002c50: 0000 0072 0d00 0000 5a0b 7465 7874 7561  ...r....Z.textua
-00002c60: 6c2e 6170 7072 0e00 0000 720f 0000 0072  l.appr....r....r
-00002c70: 1000 0000 5a0f 7465 7874 7561 6c2e 6269  ....Z.textual.bi
-00002c80: 6e64 696e 6772 1100 0000 5a12 7465 7874  ndingr....Z.text
-00002c90: 7561 6c2e 636f 6e74 6169 6e65 7273 7212  ual.containersr.
-00002ca0: 0000 0072 1300 0000 7214 0000 005a 1174  ...r....r....Z.t
-00002cb0: 6578 7475 616c 2e63 7373 2e71 7565 7279  extual.css.query
-00002cc0: 7215 0000 005a 0e74 6578 7475 616c 2e73  r....Z.textual.s
-00002cd0: 6372 6565 6e72 1600 0000 5a0f 7465 7874  creenr....Z.text
-00002ce0: 7561 6c2e 7769 6467 6574 7372 1700 0000  ual.widgetsr....
-00002cf0: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00002d00: 1b00 0000 5a14 7465 7874 7561 6c2e 7769  ....Z.textual.wi
-00002d10: 6467 6574 732e 7472 6565 721c 0000 0072  dgets.treer....r
-00002d20: 1e00 0000 5a0b 7275 6e5f 636f 6d6d 616e  ....Z.run_comman
-00002d30: 6472 1f00 0000 72b0 0000 0072 2000 0000  dr....r....r ...
-00002d40: 7221 0000 005a 1477 6964 6765 7473 2e63  r!...Z.widgets.c
-00002d50: 6f6d 6d61 6e64 5f69 6e66 6f72 2200 0000  ommand_infor"...
-00002d60: 5a14 7769 6467 6574 732e 636f 6d6d 616e  Z.widgets.comman
-00002d70: 645f 7472 6565 7223 0000 005a 0c77 6964  d_treer#...Z.wid
-00002d80: 6765 7473 2e66 6f72 6d72 2400 0000 5a17  gets.formr$...Z.
-00002d90: 7769 6467 6574 732e 6d75 6c74 6970 6c65  widgets.multiple
-00002da0: 5f63 686f 6963 6572 2500 0000 da0c 7665  _choicer%.....ve
-00002db0: 7273 696f 6e5f 696e 666f da09 696d 706f  rsion_info..impo
-00002dc0: 7274 6c69 6272 2800 0000 da12 696d 706f  rtlibr(.....impo
-00002dd0: 7274 6c69 625f 6d65 7461 6461 7461 7229  rtlib_metadatar)
-00002de0: 0000 0072 9b00 0000 7248 0000 0072 4800  ...r....rH...rH.
-00002df0: 0000 7248 0000 0072 4900 0000 da08 3c6d  ..rH...rI.....<m
-00002e00: 6f64 756c 653e 0100 0000 7342 0000 000c  odule>....sB....
-00002e10: 0008 0208 0108 010c 010c 010c 010c 010c  ................
-00002e20: 010c 020c 010c 0110 0114 010c 0114 010c  ................
-00002e30: 010c 011c 010c 010c 020c 0110 010c 010c  ................
-00002e40: 010c 010c 010a 020e 0108 0210 0300 7f14  ................
-00002e50: 4e                                       N
+00001eb0: 0164 0219 007d 056e 077c 0672 4b7c 067c  .d...}.n.|.rK|.|
+00001ec0: 017c 0519 005f 067c 017c 005f 0a74 0964  .|..._.|.|._.t.d
+00001ed0: 0964 0784 007c 01a0 0ba1 0044 0083 0183  .d...|.....D....
+00001ee0: 017c 005f 0c64 0a7c 005f 0d7c 0272 617c  .|._.d.|._.|.ra|
+00001ef0: 026e 0274 0e83 007c 005f 0f7c 037c 005f  .n.t...|._.|.|._
+00001f00: 107c 006a 1073 8974 1174 1283 018f 1001  .|.j.s.t.t......
+00001f10: 0074 13a0 147c 006a 0fa1 017c 005f 1057  .t...|.j...|._.W
+00001f20: 0064 0004 0004 0083 0301 0064 0053 0031  .d.........d.S.1
+00001f30: 0073 8277 0101 0001 0001 0059 0001 0064  .s.w.......Y...d
+00001f40: 0053 0064 0053 0029 0b4e 724f 0000 0072  .S.d.S.).NrO...r
+00001f50: 0100 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00001f60: 0003 0000 0005 0000 0013 0000 0173 2000  .............s .
+00001f70: 0000 6900 7c00 5d0c 5c02 7d01 7d02 7400  ..i.|.].\.}.}.t.
+00001f80: 7c01 8800 8302 7202 7c01 7c02 9302 7102  |.....r.|.|...q.
+00001f90: 5300 7248 0000 0072 0400 0000 2903 726a  S.rH...r....).rj
+00001fa0: 0000 00da 016b 724e 0000 00a9 0172 9c00  .....krN.....r..
+00001fb0: 0000 7248 0000 0072 4900 0000 da0a 3c64  ..rH...rI.....<d
+00001fc0: 6963 7463 6f6d 703e 0501 0000 730c 0000  ictcomp>....s...
+00001fd0: 0006 0006 0208 0102 fd04 0106 ff7a 2054  .............z T
+00001fe0: 7569 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63  ui.__init__.<loc
+00001ff0: 616c 733e 2e3c 6469 6374 636f 6d70 3e72  als>.<dictcomp>r
+00002000: 1d00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00002010: 0002 0000 0003 0000 0033 0000 0173 1800  .........3...s..
+00002020: 0000 8100 7c00 5d07 7d01 7c01 8800 7600  ....|.].}.|...v.
+00002030: 5600 0100 7102 6400 5300 723f 0000 0072  V...q.d.S.r?...r
+00002040: 4800 0000 7269 0000 0072 9e00 0000 7248  H...ri...r....rH
+00002050: 0000 0072 4900 0000 726c 0000 000a 0100  ...rI...rl......
+00002060: 0073 0800 0000 0280 0400 0801 0aff 7a1f  .s............z.
+00002070: 5475 692e 5f5f 696e 6974 5f5f 2e3c 6c6f  Tui.__init__.<lo
+00002080: 6361 6c73 3e2e 3c67 656e 6578 7072 3e29  cals>.<genexpr>)
+00002090: 02da 012a fa01 3f63 0100 0000 0000 0000  ...*..?c........
+000020a0: 0000 0000 0200 0000 0200 0000 7300 0001  ............s...
+000020b0: 7316 0000 0081 007c 005d 067d 017c 016a  s......|.].}.|.j
+000020c0: 0056 0001 0071 0264 0053 0072 3f00 0000  .V...q.d.S.r?...
+000020d0: 2901 da0b 7375 6263 6f6d 6d61 6e64 7329  )...subcommands)
+000020e0: 0272 6a00 0000 724e 0000 0072 4800 0000  .rj...rN...rH...
+000020f0: 7248 0000 0072 4900 0000 726c 0000 0014  rH...rI...rl....
+00002100: 0100 0073 0400 0000 0280 1400 4629 1572  ...s........F).r
+00002110: 4000 0000 7241 0000 0072 5f00 0000 725d  @...rA...r_...r]
+00002120: 0000 00da 046c 6973 74da 046b 6579 7372  .....list..keysr
+00002130: a200 0000 da05 6974 656d 73da 036c 656e  ......items..len
+00002140: da03 616e 7972 3400 0000 da06 7661 6c75  ..anyr4.....valu
+00002150: 6573 723a 0000 0072 6000 0000 721e 0000  esr:...r`...r...
+00002160: 0072 3600 0000 7238 0000 0072 0300 0000  .r6...r8...r....
+00002170: da09 4578 6365 7074 696f 6e72 2800 0000  ..Exceptionr(...
+00002180: 7243 0000 0029 0772 4500 0000 7234 0000  rC...).rE...r4..
+00002190: 0072 3600 0000 7238 0000 0072 9c00 0000  .r6...r8...r....
+000021a0: da0d 726f 6f74 5f63 6d64 5f6e 616d 655a  ..root_cmd_nameZ
+000021b0: 106d 6174 6368 696e 675f 7363 6865 6d61  .matching_schema
+000021c0: 7372 4600 0000 729e 0000 0072 4900 0000  srF...r....rI...
+000021d0: 7241 0000 00f6 0000 0073 3200 0000 0a07  rA.......s2.....
+000021e0: 0602 0601 1002 0e02 0a01 0c02 06fe 1805  ................
+000021f0: 0201 08ff 0403 1201 0402 0a01 0602 1801  ................
+00002200: 0601 1002 0601 0602 0a01 1001 22ff 04ff  ............"...
+00002210: 7a0c 5475 692e 5f5f 696e 6974 5f5f da04  z.Tui.__init__..
+00002220: 6172 6773 7221 0000 0063 0100 0000 0000  argsr!...c......
+00002230: 0000 0000 0000 0600 0000 0400 0000 4f00  ..............O.
+00002240: 0001 7352 0000 007c 0173 0674 0064 0183  ..sR...|.s.t.d..
+00002250: 0182 017c 0164 0219 007d 037c 036a 017c  ...|.d...}.|.j.|
+00002260: 0369 017d 047c 0164 0364 0085 0219 0044  .i.}.|.d.d.....D
+00002270: 005d 0b7d 057c 037c 055f 027c 057c 036a  .].}.|.|._.|.|.j
+00002280: 037c 056a 013c 0071 157c 007c 0466 0169  .|.j.<.q.|.|.f.i
+00002290: 007c 02a4 018e 0153 0029 044e 7a14 4e6f  .|.....S.).Nz.No
+000022a0: 2073 6368 656d 6173 2070 726f 7669 6465   schemas provide
+000022b0: 642e 7201 0000 0072 1d00 0000 2904 da0a  d.r....r....)...
+000022c0: 5661 6c75 6545 7272 6f72 723c 0000 0072  ValueErrorr<...r
+000022d0: 9400 0000 72a2 0000 0029 06da 0363 6c73  ....r....)...cls
+000022e0: 72ab 0000 00da 066b 7761 7267 735a 0b72  r......kwargsZ.r
+000022f0: 6f6f 745f 7363 6865 6d61 da07 7363 6865  oot_schema..sche
+00002300: 6d61 735a 0673 6368 656d 6172 4800 0000  masZ.schemarH...
+00002310: 7248 0000 0072 4900 0000 da0c 6672 6f6d  rH...rI.....from
+00002320: 5f73 6368 656d 6173 1e01 0000 7310 0000  _schemas....s...
+00002330: 0004 0208 0108 020a 0210 0206 010e 0110  ................
+00002340: 027a 1054 7569 2e66 726f 6d5f 7363 6865  .z.Tui.from_sche
+00002350: 6d61 7363 0100 0000 0000 0000 0000 0000  masc............
+00002360: 0100 0000 0800 0000 4300 0001 7322 0000  ........C...s"..
+00002370: 007c 00a0 0074 017c 006a 027c 006a 037c  .|...t.|.j.|.j.|
+00002380: 006a 047c 006a 0564 018d 04a1 0101 0064  .j.|.j.d.......d
+00002390: 0053 0029 024e 2903 7236 0000 0072 3800  .S.).N).r6...r8.
+000023a0: 0000 723a 0000 0029 0672 7700 0000 7229  ..r:...).rw...r)
+000023b0: 0000 0072 3400 0000 7236 0000 0072 3800  ...r4...r6...r8.
+000023c0: 0000 723a 0000 0072 6100 0000 7248 0000  ..r:...ra...rH..
+000023d0: 0072 4800 0000 7249 0000 0072 7d00 0000  .rH...rI...r}...
+000023e0: 2d01 0000 7310 0000 0004 0102 0104 0104  -...s...........
+000023f0: 0104 0104 0104 fc08 ff7a 0c54 7569 2e6f  .........z.Tui.o
+00002400: 6e5f 6d6f 756e 747a 1123 686f 6d65 2d65  n_mountz.#home-e
+00002410: 7865 632d 6275 7474 6f6e 6301 0000 0000  xec-buttonc.....
+00002420: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00002430: 0000 0173 1200 0000 6401 7c00 5f00 7c00  ...s....d.|._.|.
+00002440: a001 a100 0100 6400 5300 7259 0000 0029  ......d.S.rY...)
+00002450: 0272 6000 0000 7232 0000 0072 6100 0000  .r`...r2...ra...
+00002460: 7248 0000 0072 4800 0000 7249 0000 00da  rH...rH...rI....
+00002470: 116f 6e5f 6275 7474 6f6e 5f70 7265 7373  .on_button_press
+00002480: 6564 3701 0000 7304 0000 0006 020c 017a  ed7...s........z
+00002490: 1554 7569 2e6f 6e5f 6275 7474 6f6e 5f70  .Tui.on_button_p
+000024a0: 7265 7373 6564 46a9 03da 0868 6561 646c  ressedF....headl
+000024b0: 6573 73da 0473 697a 65da 0a61 7574 6f5f  ess..size..auto_
+000024c0: 7069 6c6f 7472 b300 0000 723b 0000 0072  pilotr....r;...r
+000024d0: b400 0000 fa16 7475 706c 655b 696e 742c  ......tuple[int,
+000024e0: 2069 6e74 5d20 7c20 4e6f 6e65 72b5 0000   int] | Noner...
+000024f0: 00fa 1c41 7574 6f70 696c 6f74 4361 6c6c  ...AutopilotCall
+00002500: 6261 636b 5479 7065 207c 204e 6f6e 6563  backType | Nonec
+00002510: 0100 0000 0000 0000 0300 0000 0900 0000  ................
+00002520: 0d00 0000 0300 0001 7342 0100 007a 5774  ........sB...zWt
+00002530: 0083 006a 017c 017c 027c 0364 018d 0301  ...j.|.|.|.d....
+00002540: 0057 007c 006a 0272 5274 0383 007d 047c  .W.|.j.rRt...}.|
+00002550: 006a 0272 547c 006a 0472 567c 04a0 0564  .j.rT|.j.rV|...d
+00002560: 027c 006a 069b 0064 037c 006a 079b 0064  .|.j...d.|.j...d
+00002570: 049d 05a1 0101 0074 08a0 097c 006a 06a1  .......t...|.j..
+00002580: 017d 057c 0564 0519 007d 0667 007c 05a2  .}.|.d...}.g.|..
+00002590: 017c 006a 02a2 017d 0774 0a6a 0ba0 0ca1  .|.j...}.t.j....
+000025a0: 007d 0874 0a6a 0da0 0e74 0aa0 0fa1 007c  .}.t.j...t.....|
+000025b0: 0864 0619 0067 02a1 017c 0864 063c 0074  .d...g...|.d.<.t
+000025c0: 0aa0 107c 067c 077c 08a1 0301 0064 0053  ...|.|.|.....d.S
+000025d0: 0064 0053 0064 0053 0064 0053 007c 006a  .d.S.d.S.d.S.|.j
+000025e0: 0272 9e74 0383 007d 047c 006a 0272 9f7c  .r.t...}.|.j.r.|
+000025f0: 006a 0472 a07c 04a0 0564 027c 006a 069b  .j.r.|...d.|.j..
+00002600: 0064 037c 006a 079b 0064 049d 05a1 0101  .d.|.j...d......
+00002610: 0074 08a0 097c 006a 06a1 017d 057c 0564  .t...|.j...}.|.d
+00002620: 0519 007d 0667 007c 05a2 017c 006a 02a2  ...}.g.|...|.j..
+00002630: 017d 0774 0a6a 0ba0 0ca1 007d 0874 0a6a  .}.t.j.....}.t.j
+00002640: 0da0 0e74 0aa0 0fa1 007c 0864 0619 0067  ...t.....|.d...g
+00002650: 02a1 017c 0864 063c 0074 0aa0 107c 067c  ...|.d.<.t...|.|
+00002660: 077c 08a1 0301 0077 0077 0077 0077 0029  .|.....w.w.w.w.)
+00002670: 074e 72b2 0000 007a 1052 756e 6e69 6e67  .Nr....z.Running
+00002680: 205b 6220 6379 616e 5d72 6600 0000 7a03   [b cyan]rf...z.
+00002690: 5b2f 5d72 0100 0000 da04 5041 5448 2911  [/]r......PATH).
+000026a0: 7240 0000 0072 0700 0000 725f 0000 0072  r@...r....r_...r
+000026b0: 0900 0000 7260 0000 00da 0570 7269 6e74  ....r`.....print
+000026c0: 7236 0000 0072 5d00 0000 7267 0000 00da  r6...r]...rg....
+000026d0: 0573 706c 6974 da02 6f73 da07 656e 7669  .split..os..envi
+000026e0: 726f 6e72 6400 0000 da07 7061 7468 7365  ronrd.....pathse
+000026f0: 7072 7300 0000 da06 6765 7463 7764 da07  prs.....getcwd..
+00002700: 6578 6563 7670 6529 0972 4500 0000 72b3  execvpe).rE...r.
+00002710: 0000 0072 b400 0000 72b5 0000 00da 0763  ...r....r......c
+00002720: 6f6e 736f 6c65 5a0e 7370 6c69 745f 6170  onsoleZ.split_ap
+00002730: 705f 6e61 6d65 5a0c 7072 6f67 7261 6d5f  p_nameZ.program_
+00002740: 6e61 6d65 da09 6172 6775 6d65 6e74 73da  name..arguments.
+00002750: 0365 6e76 7246 0000 0072 4800 0000 7249  .envrF...rH...rI
+00002760: 0000 0072 0700 0000 3c01 0000 733c 0000  ...r....<...s<..
+00002770: 0002 0714 0106 0206 010c 0104 0114 0104  ................
+00002780: ff0c 0408 010e 010a 021c 0112 0104 f308  ................
+00002790: 0206 fe06 010c 0104 0114 0104 ff0c 0408  ................
+000027a0: 010e 010a 021c 0110 0102 f304 027a 0754  .............z.T
+000027b0: 7569 2e72 756e 6301 0000 0000 0000 0000  ui.runc.........
+000027c0: 0000 0002 0000 0008 0000 0043 0000 0173  ...........C...s
+000027d0: 3000 0000 7a07 7c00 a000 7401 a101 7d01  0...z.|...t...}.
+000027e0: 5700 6e0a 0400 7402 7911 0100 0100 0100  W.n...t.y.......
+000027f0: 5900 6400 5300 7700 7c01 a003 a100 0100  Y.d.S.w.|.......
+00002800: 6400 5300 723f 0000 0029 0472 8000 0000  d.S.r?...).r....
+00002810: 7223 0000 0072 1500 0000 7253 0000 0029  r#...r....rS...)
+00002820: 0272 4500 0000 7286 0000 0072 4800 0000  .rE...r....rH...
+00002830: 7248 0000 0072 4900 0000 da19 6163 7469  rH...rI.....acti
+00002840: 6f6e 5f66 6f63 7573 5f63 6f6d 6d61 6e64  on_focus_command
+00002850: 5f74 7265 6555 0100 0073 0c00 0000 0201  _treeU...s......
+00002860: 0e01 0c01 0601 02ff 0c03 7a1d 5475 692e  ..........z.Tui.
+00002870: 6163 7469 6f6e 5f66 6f63 7573 5f63 6f6d  action_focus_com
+00002880: 6d61 6e64 5f74 7265 6563 0100 0000 0000  mand_treec......
+00002890: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
+000028a0: 0001 731e 0000 007c 00a0 0074 01a1 017d  ..s....|...t...}
+000028b0: 017c 00a0 0274 037c 016a 0483 01a1 0101  .|...t.|.j......
+000028c0: 0064 0053 0072 3f00 0000 2905 7280 0000  .d.S.r?...).r...
+000028d0: 0072 2900 0000 7277 0000 0072 2200 0000  .r)...rw...r"...
+000028e0: 7282 0000 0029 0272 4500 0000 5a0f 636f  r....).rE...Z.co
+000028f0: 6d6d 616e 645f 6275 696c 6465 7272 4800  mmand_builderrH.
+00002900: 0000 7248 0000 0072 4900 0000 da18 6163  ..rH...rI.....ac
+00002910: 7469 6f6e 5f73 686f 775f 636f 6d6d 616e  tion_show_comman
+00002920: 645f 696e 666f 5d01 0000 7304 0000 000a  d_info]...s.....
+00002930: 0114 017a 1c54 7569 2e61 6374 696f 6e5f  ...z.Tui.action_
+00002940: 7368 6f77 5f63 6f6d 6d61 6e64 5f69 6e66  show_command_inf
+00002950: 6fda 0375 726c 7237 0000 0063 0200 0000  o..urlr7...c....
+00002960: 0000 0000 0000 0000 0200 0000 0200 0000  ................
+00002970: 4300 0001 730c 0000 0074 007c 0183 0101  C...s....t.|....
+00002980: 0064 0153 0029 027a 6956 6973 6974 2074  .d.S.).ziVisit t
+00002990: 6865 2067 6976 656e 2055 524c 2c20 7669  he given URL, vi
+000029a0: 6120 7468 6520 6f70 6572 6174 696e 6720  a the operating 
+000029b0: 7379 7374 656d 2e0a 0a20 2020 2020 2020  system...       
+000029c0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+000029d0: 2020 2075 726c 3a20 5468 6520 5552 4c20     url: The URL 
+000029e0: 746f 2076 6973 6974 2e0a 2020 2020 2020  to visit..      
+000029f0: 2020 4e29 01da 086f 7065 6e5f 7572 6c29    N)...open_url)
+00002a00: 0272 4500 0000 72c5 0000 0072 4800 0000  .rE...r....rH...
+00002a10: 7248 0000 0072 4900 0000 da0c 6163 7469  rH...rI.....acti
+00002a20: 6f6e 5f76 6973 6974 6101 0000 7302 0000  on_visita...s...
+00002a30: 000c 067a 1054 7569 2e61 6374 696f 6e5f  ...z.Tui.action_
+00002a40: 7669 7369 7429 024e 4e29 0a72 3400 0000  visit).NN).r4...
+00002a50: 7235 0000 0072 3600 0000 7239 0000 0072  r5...r6...r9...r
+00002a60: 3800 0000 7239 0000 0072 9c00 0000 7239  8...r9...r....r9
+00002a70: 0000 0072 4a00 0000 7258 0000 0029 0472  ...rJ...rX...).r
+00002a80: ab00 0000 7221 0000 0072 4a00 0000 729b  ....r!...rJ...r.
+00002a90: 0000 0029 0872 b300 0000 723b 0000 0072  ...).r....r;...r
+00002aa0: b400 0000 72b6 0000 0072 b500 0000 72b7  ....r....r....r.
+00002ab0: 0000 0072 4a00 0000 7258 0000 0072 9600  ...rJ...rX...r..
+00002ac0: 0000 2904 72c5 0000 0072 3700 0000 724a  ..).r....r7...rJ
+00002ad0: 0000 0072 5800 0000 2914 7297 0000 0072  ...rX...).r....r
+00002ae0: 9800 0000 7299 0000 0072 0600 0000 da08  ....r....r......
+00002af0: 5f5f 6669 6c65 5f5f 7294 0000 005a 0843  __file__r....Z.C
+00002b00: 5353 5f50 4154 4872 4100 0000 da0b 636c  SS_PATHrA.....cl
+00002b10: 6173 736d 6574 686f 6472 b000 0000 727d  assmethodr....r}
+00002b20: 0000 0072 0d00 0000 7217 0000 005a 0750  ...r....r....Z.P
+00002b30: 7265 7373 6564 72b1 0000 0072 0700 0000  ressedr....r....
+00002b40: 72c3 0000 0072 c400 0000 72c7 0000 0072  r....r....r....r
+00002b50: 9a00 0000 7248 0000 0072 4800 0000 7246  ....rH...rH...rF
+00002b60: 0000 0072 4900 0000 729b 0000 00f3 0000  ...rI...r.......
+00002b70: 0073 2200 0000 0800 0e01 0206 0201 10fb  .s".............
+00002b80: 0228 0c01 080e 0a0a 0a01 0207 0201 0201  .(..............
+00002b90: 12fb 0a19 0a08 1204 729b 0000 0029 42da  ........r....)B.
+00002ba0: 0a5f 5f66 7574 7572 655f 5f72 0200 0000  .__future__r....
+00002bb0: 72bb 0000 0072 6700 0000 7270 0000 00da  r....rg...rp....
+00002bc0: 0a63 6f6e 7465 7874 6c69 6272 0300 0000  .contextlibr....
+00002bd0: 7205 0000 00da 0770 6174 686c 6962 7206  r......pathlibr.
+00002be0: 0000 00da 0a73 7562 7072 6f63 6573 7372  .....subprocessr
+00002bf0: 0700 0000 5a0a 7765 6262 726f 7773 6572  ....Z.webbrowser
+00002c00: 7208 0000 0072 c600 0000 5a0c 7269 6368  r....r....Z.rich
+00002c10: 2e63 6f6e 736f 6c65 7209 0000 005a 1072  .consoler....Z.r
+00002c20: 6963 682e 6869 6768 6c69 6768 7465 7272  ich.highlighterr
+00002c30: 0a00 0000 5a09 7269 6368 2e74 6578 7472  ....Z.rich.textr
+00002c40: 0b00 0000 5a07 7465 7874 7561 6c72 0c00  ....Z.textualr..
+00002c50: 0000 720d 0000 005a 0b74 6578 7475 616c  ..r....Z.textual
+00002c60: 2e61 7070 720e 0000 0072 0f00 0000 7210  .appr....r....r.
+00002c70: 0000 005a 0f74 6578 7475 616c 2e62 696e  ...Z.textual.bin
+00002c80: 6469 6e67 7211 0000 005a 1274 6578 7475  dingr....Z.textu
+00002c90: 616c 2e63 6f6e 7461 696e 6572 7372 1200  al.containersr..
+00002ca0: 0000 7213 0000 0072 1400 0000 5a11 7465  ..r....r....Z.te
+00002cb0: 7874 7561 6c2e 6373 732e 7175 6572 7972  xtual.css.queryr
+00002cc0: 1500 0000 5a0e 7465 7874 7561 6c2e 7363  ....Z.textual.sc
+00002cd0: 7265 656e 7216 0000 005a 0f74 6578 7475  reenr....Z.textu
+00002ce0: 616c 2e77 6964 6765 7473 7217 0000 0072  al.widgetsr....r
+00002cf0: 1800 0000 7219 0000 0072 1a00 0000 721b  ....r....r....r.
+00002d00: 0000 005a 1474 6578 7475 616c 2e77 6964  ...Z.textual.wid
+00002d10: 6765 7473 2e74 7265 6572 1c00 0000 721e  gets.treer....r.
+00002d20: 0000 005a 0b72 756e 5f63 6f6d 6d61 6e64  ...Z.run_command
+00002d30: 721f 0000 0072 af00 0000 7220 0000 0072  r....r....r ...r
+00002d40: 2100 0000 5a14 7769 6467 6574 732e 636f  !...Z.widgets.co
+00002d50: 6d6d 616e 645f 696e 666f 7222 0000 005a  mmand_infor"...Z
+00002d60: 1477 6964 6765 7473 2e63 6f6d 6d61 6e64  .widgets.command
+00002d70: 5f74 7265 6572 2300 0000 5a0c 7769 6467  _treer#...Z.widg
+00002d80: 6574 732e 666f 726d 7224 0000 005a 1777  ets.formr$...Z.w
+00002d90: 6964 6765 7473 2e6d 756c 7469 706c 655f  idgets.multiple_
+00002da0: 6368 6f69 6365 7225 0000 00da 0c76 6572  choicer%.....ver
+00002db0: 7369 6f6e 5f69 6e66 6fda 0969 6d70 6f72  sion_info..impor
+00002dc0: 746c 6962 7228 0000 00da 1269 6d70 6f72  tlibr(.....impor
+00002dd0: 746c 6962 5f6d 6574 6164 6174 6172 2900  tlib_metadatar).
+00002de0: 0000 729b 0000 0072 4800 0000 7248 0000  ..r....rH...rH..
+00002df0: 0072 4800 0000 7249 0000 00da 083c 6d6f  .rH...rI.....<mo
+00002e00: 6475 6c65 3e01 0000 0073 4200 0000 0c00  dule>....sB.....
+00002e10: 0802 0801 0801 0c01 0c01 0c01 0c01 0c01  ................
+00002e20: 0c02 0c01 0c01 1001 1401 0c01 1401 0c01  ................
+00002e30: 0c01 1c01 0c01 0c02 0c01 1001 0c01 0c01  ................
+00002e40: 0c01 0c01 0a02 0e01 0802 1003 007f 144e  ...............N
```

### Comparing `argparse-tui-0.1.3/src/argparse_tui/argparse.py` & `argparse-tui-0.2.0/src/argparse_tui/argparse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from __future__ import annotations
 
 import argparse
 import sys
+from contextlib import suppress
+from copy import deepcopy
 from typing import Any
 
 from .constants import DEFAULT_COMMAND_NAME
 from .schemas import ArgumentSchema, CommandName, CommandSchema, OptionSchema
 from .tui import Tui
 
 
 def introspect_argparse_parser(
     parser: argparse.ArgumentParser,
-    cmd_ignorelist: list[argparse.ArgumentParser] | None = None,
+    subparser_ignorelist: list[argparse.ArgumentParser] | None = None,
+    value_overrides: dict[str, Any] | None = None,
 ) -> dict[CommandName, CommandSchema]:
     def process_command(
         cmd_name: CommandName,
         parser: argparse.ArgumentParser,
         parent=None,
     ) -> CommandSchema:
         cmd_data = CommandSchema(
@@ -36,15 +39,16 @@
                 param.default,
             ]:
                 continue
 
             if isinstance(param, argparse._SubParsersAction):
                 for subparser_name, subparser in param.choices.items():
                     if subparser.description != argparse.SUPPRESS and (
-                        not cmd_ignorelist or subparser not in cmd_ignorelist
+                        not subparser_ignorelist
+                        or subparser not in subparser_ignorelist
                     ):
                         cmd_data.subcommands[
                             CommandName(subparser_name)
                         ] = process_command(
                             CommandName(subparser_name),
                             subparser,
                             parent=cmd_data,
@@ -90,33 +94,31 @@
                     opts = [
                         x
                         for x in param.option_strings
                         if not x.startswith(secondary_prefix)
                     ]
                     secondary_opts = [x for x in param.option_strings if x not in opts]
 
-            # look for these "tags" in the help text: "secret", "prompt"
+            # look for these "tags" in the help text: "secret"
             # if present, set variables and remove from the help text.
             is_secret: bool = False
-            is_prompt: bool = False
             param_help: str = param.help
             if param_help:
                 param_help = param_help.replace("%(default)s", str(param.default))
 
                 tag_prefix: str = "<"
                 tag_suffix: str = ">"
                 tag_start: int = param_help.find(tag_prefix)
                 if tag_start >= 0:
                     tag_end: int = param_help.find(tag_suffix)
                     if tag_end > tag_start:
                         tag_txt: str = param_help[tag_start : tag_end + 1]
                         tags: list[str] = [x.strip() for x in tag_txt[1:-1].split(",")]
                         is_secret = "secret" in tags
-                        is_prompt = "prompt" in tags
-                        if any([is_secret, is_prompt]):
+                        if any([is_secret]):
                             param_help = param_help.replace(tag_txt, "")
 
             nargs: int = (
                 1
                 if param.nargs in [None, "?"]
                 else -1
                 if param.nargs in ["+", "*", argparse.REMAINDER]
@@ -129,161 +131,213 @@
                     name=opts,
                     type=param_type,
                     is_flag=is_flag,
                     counting=is_counting,
                     secondary_opts=secondary_opts,
                     required=param.required,
                     default=param.default,
+                    value=value_overrides.get(param.dest),
                     help=param_help,
                     choices=param.choices,
                     multiple=is_multiple,
                     multi_value=multi_value,
                     nargs=nargs,
                     secret=is_secret,
-                    read_only=is_prompt,
-                    placeholder="< You will be prompted. >" if is_prompt else "",
                 )
                 cmd_data.options.append(option_data)
 
             else:
                 argument_data = ArgumentSchema(
                     name=param.dest,
                     type=param_type,
                     required=param.required,
                     default=param.default,
+                    value=value_overrides.get(param.dest),
                     help=param_help,
                     choices=param.choices,
                     multiple=is_multiple,
                     multi_value=multi_value,
                     nargs=nargs,
                     secret=is_secret,
-                    read_only=is_prompt,
-                    placeholder="< You will be prompted. >" if is_prompt else "",
                 )
                 cmd_data.arguments.append(argument_data)
 
         return cmd_data
 
     data: dict[CommandName, CommandSchema] = {}
 
     root_cmd_name = CommandName("root")
+
+    if value_overrides is None:
+        value_overrides = {}
+
     data[root_cmd_name] = process_command(root_cmd_name, parser)
 
     return data
 
 
 def invoke_tui(
     parser: argparse.ArgumentParser,
-    cmd_ignorelist: list[argparse.ArgumentParser] = None,
-    command_filter: str | None = None,
+    subparser_ignorelist: list[argparse.ArgumentParser] | None = None,
+    cli_args: list[str] | None = None,
 ):
     """
     Examples:
         >>> import argparse
         >>> from argparse_tui import invoke_tui
         ...
         >>> parser = argparse.ArgumentParser(prog="awesome-app")
         >>> _ = parser.add_argument("--value")
         ...
         >>> invoke_tui(parser)  # doctest: +SKIP
     """
 
-    if cmd_ignorelist is None:
-        cmd_ignorelist = [parser]
+    cmd_filter: str | None = None
+    parsed_args: dict[str, str] = {}
+
+    if cli_args:
+        for x in cli_args:
+            if not x.startswith("-"):
+                cmd_filter = x
+                break
+
+        # Make all args optional
+        def _set_actions_optional(parser):
+            # Update arguments
+
+            for action in parser._actions:
+                action.required = False
+
+            # Update subparsers
+            if parser._subparsers:
+                for sp_action in parser._subparsers._actions:
+                    sp_action.required = False
+                    if isinstance(sp_action, argparse._SubParsersAction):
+                        for subparser in sp_action.choices.values():
+                            _set_actions_optional(subparser)
+
+        parser_copy: argparse.ArgumentParser = deepcopy(parser)
+        _set_actions_optional(parser_copy)
+
+        with suppress(SystemExit):
+            namespace, _unknown_args = parser_copy.parse_known_args(cli_args)
+            parsed_args = vars(namespace)
+
+    schemas = introspect_argparse_parser(
+        parser,
+        subparser_ignorelist=subparser_ignorelist,
+        value_overrides=parsed_args,
+    )
 
     Tui(
-        introspect_argparse_parser(parser, cmd_ignorelist=cmd_ignorelist),
+        schemas,
         app_name=parser.prog,
-        command_filter=command_filter,
+        command_filter=cmd_filter,
     ).run()
 
 
 class TuiAction(argparse.Action):
     """argparse `Action` that will analyze the parser and display a TUI.
 
     Examples:
         >>> import argparse
         >>> from argparse_tui import TuiAction
         ...
         >>> parser = argparse.ArgumentParser()
         >>> _ = parser.add_argument('--tui', action=TuiAction)
         ...
         >>> parser.print_usage()
-        usage: __main__.py [-h] [--tui [TUI]]
+        usage: __main__.py [-h] [--tui]
     """
 
     def __init__(
         self,
         option_strings: list[str],
         dest: str = argparse.SUPPRESS,
         default: Any = argparse.SUPPRESS,
         help: str | None = "Open Textual UI.",
         const: str = None,
         metavar: str = None,
-        nargs: int | str | None = None,
+        parent_parser: argparse.ArgumentParser | None = None,
         **_kwargs: Any,
     ):
         super(TuiAction, self).__init__(
             option_strings=option_strings,
             dest=dest,
             default=default,
-            nargs="?" if nargs is None else nargs,
+            nargs=0,
             help=help,
             const=const,
             metavar=metavar,
         )
+        self._parent_parser = parent_parser
 
     def __call__(self, parser, namespace, values, option_string=None):
-        root_parser: argparse.ArgumentParser = getattr(
-            namespace,
-            "_parent_parser",
-            parser,
+        root_parser: argparse.ArgumentParser = (
+            self._parent_parser if self._parent_parser else parser
         )
+        subparser_ignorelist: list[str] = [] if option_string else [parser]
 
-        invoke_tui(root_parser, cmd_ignorelist=[parser], command_filter=values)
+        cli_args: list[str] = sys.argv[1:]
+
+        if cli_args:
+            if option_string:
+                with suppress(ValueError):
+                    cli_args.pop(cli_args.index(option_string))
+            else:
+                with suppress(ValueError):
+                    cli_args.pop(cli_args.index(self.dest.lower().replace("_", "-")))
+
+        invoke_tui(
+            root_parser,
+            subparser_ignorelist=subparser_ignorelist,
+            cli_args=cli_args,
+        )
 
         parser.exit()
 
 
 def add_tui_argument(
     parser: argparse.ArgumentParser,
-    option_strings: str | list[str] = None,
+    parent_parser: argparse.ArgumentParser | None = None,
+    option_strings: str | list[str] | None = None,
     help: str = "Open Textual UI.",
     default=argparse.SUPPRESS,
     **kwargs,
 ) -> None:
     """
 
     Args:
-        parser: the argparse parser
+        parser: the argparse parser to add the argument to.
+        parent_parser: the parent of the given parser.
         option_strings: list of CLI flags that will invoke the TUI (default=`--tui`)
         help: help message for the argument
 
     Examples:
         >>> import argparse
         >>> from argparse_tui import add_tui_argument
         ...
         >>> parser = argparse.ArgumentParser()
         ...
         >>> add_tui_argument(parser)
         ...
         >>> parser.print_usage()
-        usage: __main__.py [-h] [--tui [CMD]]
+        usage: __main__.py [-h] [--tui]
     """
     if not option_strings:
         option_strings = [f"--{DEFAULT_COMMAND_NAME.replace('_', '-').lstrip('-')}"]
     elif isinstance(option_strings, str):
         option_strings = [option_strings]
 
     parser.add_argument(
         *option_strings,
-        metavar="CMD",
         action=TuiAction,
         default=default,
         help=help,
+        parent_parser=parent_parser,
         **kwargs,
     )
 
 
 def add_tui_command(
     parser: argparse.ArgumentParser,
     command: str = DEFAULT_COMMAND_NAME,
@@ -321,17 +375,15 @@
                 break
 
     tui_parser = subparsers.add_parser(
         command,
         description=argparse.SUPPRESS,
         help=help,
     )
-    tui_parser.set_defaults(_parent_parser=parser)
 
     add_tui_argument(
         tui_parser,
-        option_strings=["cmd_filter"],
-        default=None,
-        help="Command filter",
+        parent_parser=parser,
+        option_strings=[command],
     )
 
     return subparsers
```

### Comparing `argparse-tui-0.1.3/src/argparse_tui/detect_run_string.py` & `argparse-tui-0.2.0/src/argparse_tui/detect_run_string.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.3/src/argparse_tui/run_command.py` & `argparse-tui-0.2.0/src/argparse_tui/run_command.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.3/src/argparse_tui/schemas.py` & `argparse-tui-0.2.0/src/argparse_tui/schemas.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,26 +44,32 @@
 class ArgumentSchema:
     name: str | list[str]
     type: Type[Any] | Sequence[Type[Any]] | None = None
     required: bool = False
     help: str | None = None
     key: str | tuple[str] = field(default_factory=generate_unique_id)
     default: MultiValueParamData | Any | None = None
+    value: MultiValueParamData | Any | None = None
     choices: Sequence[str] | None = None
     multiple: bool = False
     multi_value: bool = False
     nargs: int = 1
     secret: bool = False
     read_only: bool = False
     placeholder: str = ""
 
     def __post_init__(self):
         if not isinstance(self.default, MultiValueParamData):
             self.default = MultiValueParamData.process_cli_option(self.default)
 
+        if self.value is None:
+            self.value = self.default
+        elif not isinstance(self.value, MultiValueParamData):
+            self.value = MultiValueParamData.process_cli_option(self.value)
+
         default_type: list[Type[Any]] = [str]
 
         if not self.type:
             self.type = default_type
         elif isinstance(self.type, partial):
             # if this is an instance of `functools.partial`,
             # iterate over the args/kwargs looking for a type.
@@ -78,15 +84,15 @@
                         self.type = [v]
                         break
                 else:
                     self.type = default_type
         elif isinstance(self.type, Type):
             self.type = [self.type]
         elif len(self.type) == 1 and isinstance(self.type[0], ChoiceSchema):
-            # if there is only one type is it is a 'ChoiceSchema':
+            # if there is only one type and it is a 'ChoiceSchema':
             self.choices = self.type[0].choices
             self.type = default_type
 
         if self.choices:
             self.choices = [str(x) for x in self.choices]
 
         if self.multi_value:
@@ -103,19 +109,19 @@
 @dataclass
 class CommandSchema:
     name: CommandName
     docstring: str | None = None
     key: str = field(default_factory=generate_unique_id)
     options: list[OptionSchema] = field(default_factory=list)
     arguments: list[ArgumentSchema] = field(default_factory=list)
-    subcommands: dict["CommandName", "CommandSchema"] = field(default_factory=dict)
-    parent: "CommandSchema | None" = None
+    subcommands: dict[CommandName, CommandSchema] = field(default_factory=dict)
+    parent: CommandSchema | None = None
 
     @property
-    def path_from_root(self) -> list["CommandSchema"]:
+    def path_from_root(self) -> list[CommandSchema]:
         node = self
         path = [self]
         while True:
             node = node.parent
             if node is None:
                 break
             path.append(node)
```

### Comparing `argparse-tui-0.1.3/src/argparse_tui/tui.py` & `argparse-tui-0.2.0/src/argparse_tui/tui.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,42 +252,43 @@
     ) -> None:
         super().__init__()
 
         self.post_run_command: list[str] = []
         self.post_run_command_redacted: str = ""
 
         root_cmd_name: str = list(command_schemas.keys())[0]
+
         if command_filter and command_schemas[root_cmd_name].subcommands:
             matching_schemas: dict[CommandName, CommandSchema] = {
                 k: v
                 for k, v in command_schemas[root_cmd_name].subcommands.items()
                 if fnmatch(k, command_filter)
             }
             if len(matching_schemas) == 1 and not any(
-                x in command_filter for x in ("*", "?")
+                (x in command_filter) for x in ("*", "?")
             ):
                 command_schemas = matching_schemas
                 root_cmd_name = list(command_schemas.keys())[0]
                 #  app_name = app_name + " " + root_cmd_name
-            else:
+            elif matching_schemas:
                 command_schemas[root_cmd_name].subcommands = matching_schemas
 
         self.command_schemas = command_schemas
         self.is_grouped_cli = any(v.subcommands for v in command_schemas.values())
         self.execute_on_exit = False
 
         self.app_name = app_name if app_name else detect_run_string()
         self.app_version = app_version
 
         if not self.app_version:
             with suppress(Exception):
                 self.app_version = metadata.version(self.app_name)
 
     @classmethod
-    def from_schemas(cls, *args: CommandSchema, **kwargs) -> "Tui":
+    def from_schemas(cls, *args: CommandSchema, **kwargs) -> Tui:
         if not args:
             raise ValueError("No schemas provided.")
 
         root_schema = args[0]
 
         schemas: dict[CommandName, CommandSchema] = {root_schema.name: root_schema}
```

### Comparing `argparse-tui-0.1.3/src/argparse_tui/tui.scss` & `argparse-tui-0.2.0/src/argparse_tui/tui.scss`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/about.cpython-310.pyc` & `argparse-tui-0.2.0/src/argparse_tui/widgets/__pycache__/about.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 04:37:17 2023 UTC, .py size: 2647 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 fd45 c364 570a 0000  o........E.dW...
+00000000: 6f0d 0d0a 0000 0000 0f82 c564 570a 0000  o..........dW...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6401 6406 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/command_info.cpython-310.pyc` & `argparse-tui-0.2.0/src/argparse_tui/widgets/__pycache__/command_info.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 04:37:17 2023 UTC, .py size: 4010 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 fd45 c364 aa0f 0000  o........E.d....
+00000000: 6f0d 0d0a 0000 0000 0f82 c564 aa0f 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 ac00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/command_tree.cpython-310.pyc` & `argparse-tui-0.2.0/src/argparse_tui/widgets/__pycache__/command_tree.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 04:37:17 2023 UTC, .py size: 2246 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 fd45 c364 c608 0000  o........E.d....
+00000000: 6f0d 0d0a 0000 0000 0f82 c564 c608 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 7800 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6407  d.l.m.Z.m.Z...d.
```

### Comparing `argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/form.cpython-310.pyc` & `argparse-tui-0.2.0/src/argparse_tui/widgets/__pycache__/form.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 04:37:17 2023 UTC, .py size: 8067 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 fd45 c364 831f 0000  o........E.d....
+00000000: 6f0d 0d0a 0000 0000 0f82 c564 831f 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 c400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6400 6406 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/multiple_choice.cpython-310.pyc` & `argparse-tui-0.2.0/src/argparse_tui/widgets/__pycache__/multiple_choice.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 04:37:17 2023 UTC, .py size: 2857 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 fd45 c364 290b 0000  o........E.d)...
+00000000: 6f0d 0d0a 0000 0000 0f82 c564 290b 0000  o..........d)...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0173 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6400  d.l.m.Z.m.Z...d.
```

### Comparing `argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/parameter_controls.cpython-310.pyc` & `argparse-tui-0.2.0/src/argparse_tui/widgets/__pycache__/parameter_controls.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 04:37:17 2023 UTC, .py size: 16529 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 fd45 c364 9140 0000  o........E.d.@..
+00000000: 6f0d 0d0a 0000 0000 0f82 c564 8d40 0000  o..........d.@..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 3601 0000 5500  .....@...s6...U.
 00000030: 6400 6401 6c00 6d01 5a01 0100 6400 6402  d.d.l.m.Z...d.d.
 00000040: 6c02 5a02 6400 6403 6c02 6d03 5a03 0100  l.Z.d.d.l.m.Z...
 00000050: 6400 6404 6c04 6d05 5a05 6d06 5a06 6d07  d.d.l.m.Z.m.Z.m.
 00000060: 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b  Z.m.Z.m.Z.m.Z.m.
 00000070: 5a0b 0100 6400 6405 6c0c 6d0d 5a0d 0100  Z...d.d.l.m.Z...
@@ -258,167 +258,167 @@
 00001010: 6f74 6865 722d 6275 7474 6f6e 2d63 6f6e  other-button-con
 00001020: 7461 696e 6572 7a07 2b20 7661 6c75 65da  tainerz.+ value.
 00001030: 0773 7563 6365 7373 7a12 6164 642d 616e  .successz.add-an
 00001040: 6f74 6865 722d 6275 7474 6f6e 2902 da07  other-button)...
 00001050: 7661 7269 616e 7472 3c00 0000 7a1e 636f  variantr<...z.co
 00001060: 6d6d 616e 642d 666f 726d 2d63 6f6e 7472  mmand-form-contr
 00001070: 6f6c 2d68 656c 702d 7465 7874 291e 7237  ol-help-text).r7
-00001080: 0000 0072 3900 0000 da04 7479 7065 725e  ...r9.....typer^
-00001090: 0000 0072 4f00 0000 7258 0000 0072 2c00  ...rO...rX...r,.
-000010a0: 0000 721d 0000 00da 056e 6172 6773 da20  ..r......nargs. 
-000010b0: 5f6d 616b 655f 636f 6d6d 616e 645f 666f  _make_command_fo
-000010c0: 726d 5f63 6f6e 7472 6f6c 5f6c 6162 656c  rm_control_label
-000010d0: da08 7265 7175 6972 6564 7229 0000 0072  ..requiredr)...r
-000010e0: 3e00 0000 7216 0000 0072 5b00 0000 da12  >...r....r[.....
-000010f0: 6765 745f 636f 6e74 726f 6c5f 6d65 7468  get_control_meth
-00001100: 6f64 721b 0000 00da 036b 6579 da06 7661  odr......key..va
-00001110: 6c75 6573 da04 6c69 7374 da11 6d61 6b65  lues..list..make
-00001120: 5f77 6964 6765 745f 6772 6f75 7072 2100  _widget_groupr!.
-00001130: 0000 da03 6c65 6eda 0961 6464 5f63 6c61  ....len..add_cla
-00001140: 7373 da03 7a69 70da 145f 6170 706c 795f  ss..zip.._apply_
-00001150: 6465 6661 756c 745f 7661 6c75 6572 4300  default_valuerC.
-00001160: 0000 720f 0000 0072 1300 0000 7218 0000  ..r....r....r...
-00001170: 0029 1272 2e00 0000 7237 0000 0072 3900  .).r....r7...r9.
-00001180: 0000 5a0d 6172 6775 6d65 6e74 5f74 7970  ..Z.argument_typ
-00001190: 6572 5e00 0000 7256 0000 0072 5800 0000  er^...rV...rX...
-000011a0: da09 6973 5f6f 7074 696f 6e72 6700 0000  ..is_optionrg...
-000011b0: 725f 0000 005a 1366 6972 7374 5f66 6f63  r_...Z.first_foc
-000011c0: 7573 5f63 6f6e 7472 6f6c da0e 636f 6e74  us_control..cont
-000011d0: 726f 6c5f 6d65 7468 6f64 5a16 6d75 6c74  rol_methodZ.mult
-000011e0: 6970 6c65 5f63 686f 6963 655f 7769 6467  iple_choice_widg
-000011f0: 6574 5a13 6465 6661 756c 745f 7661 6c75  etZ.default_valu
-00001200: 655f 7475 706c 65da 0c77 6964 6765 745f  e_tuple..widget_
-00001210: 6772 6f75 70da 0d63 6f6e 7472 6f6c 5f67  group..control_g
-00001220: 726f 7570 da0d 6465 6661 756c 745f 7661  roup..default_va
-00001230: 6c75 65da 0e63 6f6e 7472 6f6c 5f77 6964  lue..control_wid
-00001240: 6765 7472 2600 0000 7226 0000 0072 2700  getr&...r&...r'.
-00001250: 0000 da07 636f 6d70 6f73 6563 0000 0073  ....composec...s
-00001260: 9200 0000 0280 0603 0601 0601 0601 1001  ................
-00001270: 0601 0a01 0601 0402 0201 0201 0201 0401  ................
-00001280: 0201 06fb 0208 02ff 0806 0801 0e01 0a02  ................
-00001290: 0405 0a01 06ff 0203 0201 0201 0201 0201  ................
-000012a0: 0401 06fb 0c07 0a04 0c01 0801 0c01 0a01  ................
-000012b0: 0206 0201 0201 0cfe 0c04 0601 0802 0401  ................
-000012c0: 0280 02f8 1cf8 0280 0a14 0c01 0801 0c01  ................
-000012d0: 0a01 0803 0601 0801 0401 0280 02fd 1cfb  ................
-000012e0: 0280 1cd1 0a3a 0601 1605 0c01 1201 1eff  .....:..........
-000012f0: 0604 1201 04ff 7a19 5061 7261 6d65 7465  ......z.Paramete
-00001300: 7243 6f6e 7472 6f6c 732e 636f 6d70 6f73  rControls.compos
-00001310: 65fa 1049 7465 7261 626c 655b 5769 6467  e..Iterable[Widg
-00001320: 6574 5d63 0100 0000 0000 0000 0000 0000  et]c............
-00001330: 0c00 0000 0700 0000 2300 0001 73b0 0000  ........#...s...
-00001340: 0081 007c 006a 007d 017c 016a 017d 027c  ...|.j.}.|.j.}.|
-00001350: 016a 0289 007c 016a 037d 037c 016a 047d  .j...|.j.}.|.j.}
-00001360: 047c 016a 057d 0574 067c 0174 0783 027d  .|.j.}.t.|.t...}
-00001370: 067c 00a0 087c 0388 007c 067c 057c 04a1  .|...|...|.|.|..
-00001380: 057d 0787 0066 0164 0164 0284 0874 097c  .}...f.d.d...t.|
-00001390: 016a 0a64 036b 0472 2f7c 016a 0a6e 0164  .j.d.k.r/|.j.n.d
-000013a0: 0383 0144 0083 017d 087c 0844 005d 1f7d  ...D...}.|.D.].}
-000013b0: 097c 016a 0b72 4174 0c7c 016a 0b64 048d  .|.j.rAt.|.j.d..
-000013c0: 017d 097c 006a 0d7c 0964 058d 017d 0a7c  .}.|.j.|.d...}.|
-000013d0: 0a7c 027c 077c 047c 017c 016a 0e83 057d  .|.|.|.|.|.j...}
-000013e0: 0b7c 0b45 0064 0648 0001 0071 3664 0653  .|.E.d.H...q6d.S
-000013f0: 0029 077a 5546 6f72 2074 6869 7320 6f70  .).zUFor this op
-00001400: 7469 6f6e 2c20 7969 656c 6420 6120 7369  tion, yield a si
-00001410: 6e67 6c65 2073 6574 206f 6620 7769 6467  ngle set of widg
-00001420: 6574 7320 7265 7175 6972 6564 2074 6f20  ets required to 
-00001430: 7265 6365 6976 6520 7573 6572 2069 6e70  receive user inp
-00001440: 7574 2066 6f72 2069 742e 6301 0000 0000  ut for it.c.....
-00001450: 0000 0000 0000 0002 0000 0005 0000 0013  ................
-00001460: 0000 0173 2800 0000 6700 7c00 5d10 7d01  ...s(...g.|.].}.
-00001470: 7c01 7400 8800 8301 6b00 720e 8800 7c01  |.t.....k.r...|.
-00001480: 1900 6e03 8800 6400 1900 9102 7102 5300  ..n...d.....q.S.
-00001490: 2901 7263 0000 0029 0172 6f00 0000 a902  ).rc...).ro.....
-000014a0: 724b 0000 00da 0169 a901 5a0e 7061 7261  rK.....i..Z.para
-000014b0: 6d65 7465 725f 7479 7065 7226 0000 0072  meter_typer&...r
-000014c0: 2700 0000 da0a 3c6c 6973 7463 6f6d 703e  '.....<listcomp>
-000014d0: d600 0000 7308 0000 0006 0002 021a ff06  ....s...........
-000014e0: ff7a 3750 6172 616d 6574 6572 436f 6e74  .z7ParameterCont
-000014f0: 726f 6c73 2e6d 616b 655f 7769 6467 6574  rols.make_widget
-00001500: 5f67 726f 7570 2e3c 6c6f 6361 6c73 3e2e  _group.<locals>.
-00001510: 3c6c 6973 7463 6f6d 703e 7261 0000 0072  <listcomp>ra...r
-00001520: 5a00 0000 725c 0000 004e 290f 7237 0000  Z...r\...N).r7..
-00001530: 0072 5e00 0000 7266 0000 0072 3900 0000  .r^...rf...r9...
-00001540: 7258 0000 0072 6900 0000 722c 0000 0072  rX...ri...r,...r
-00001550: 1d00 0000 7268 0000 00da 0572 616e 6765  ....rh.....range
-00001560: 7267 0000 0072 5b00 0000 721b 0000 0072  rg...r[...r....r
-00001570: 6a00 0000 726b 0000 0029 0c72 2e00 0000  j...rk...).r....
-00001580: 7237 0000 0072 5e00 0000 7239 0000 0072  r7...r^...r9...r
-00001590: 5800 0000 7269 0000 0072 7300 0000 725f  X...ri...rs...r_
-000015a0: 0000 005a 0f70 6172 616d 6574 6572 5f74  ...Z.parameter_t
-000015b0: 7970 6573 da05 5f74 7970 6572 7400 0000  ypes.._typert...
-000015c0: 5a0f 636f 6e74 726f 6c5f 7769 6467 6574  Z.control_widget
-000015d0: 7372 2600 0000 727d 0000 0072 2700 0000  sr&...r}...r'...
-000015e0: 726e 0000 00c4 0000 0073 3e00 0000 0280  rn.......s>.....
-000015f0: 0602 0601 0601 0601 0601 0601 0a01 0401  ................
-00001600: 0201 0201 0201 0201 0201 04fb 0a09 1602  ................
-00001610: 06fe 080a 0601 0c01 0c01 0201 0201 0201  ................
-00001620: 0201 0201 0401 04fb 0c07 04f5 7a23 5061  ............z#Pa
-00001630: 7261 6d65 7465 7243 6f6e 7472 6f6c 732e  rameterControls.
-00001640: 6d61 6b65 5f77 6964 6765 745f 6772 6f75  make_widget_grou
-00001650: 707a 132e 6164 642d 616e 6f74 6865 722d  pz..add-another-
-00001660: 6275 7474 6f6e da05 6576 656e 74fa 0e42  button..event..B
-00001670: 7574 746f 6e2e 5072 6573 7365 6463 0200  utton.Pressedc..
-00001680: 0000 0000 0000 0000 0000 0500 0000 0300  ................
-00001690: 0000 4300 0001 735c 0000 0074 007c 00a0  ..C...s\...t.|..
-000016a0: 01a1 0083 017d 027c 0264 0119 00a0 02a1  .....}.|.d......
-000016b0: 0001 0074 037c 028e 007d 0374 047c 0283  ...t.|...}.t.|..
-000016c0: 0164 026b 0172 1b7c 03a0 0564 03a1 0101  .d.k.r.|...d....
-000016d0: 007c 00a0 0674 07a1 017d 047c 04a0 087c  .|...t...}.|...|
-000016e0: 03a1 0101 007c 016a 096a 0a64 0464 058d  .....|.j.j.d.d..
-000016f0: 0101 0064 0053 0029 064e 7201 0000 0072  ...d.S.).Nr....r
-00001700: 6100 0000 7262 0000 0046 2901 da07 616e  a...rb...F)...an
-00001710: 696d 6174 6529 0b72 6d00 0000 726e 0000  imate).rm...rn..
-00001720: 00da 0566 6f63 7573 7221 0000 0072 6f00  ...focusr!...ro.
-00001730: 0000 7270 0000 0072 5200 0000 7229 0000  ..rp...rR...r)..
-00001740: 00da 056d 6f75 6e74 da06 6275 7474 6f6e  ...mount..button
-00001750: da0e 7363 726f 6c6c 5f76 6973 6962 6c65  ..scroll_visible
-00001760: 2905 722e 0000 0072 8100 0000 7275 0000  ).r....r....ru..
-00001770: 0072 7600 0000 5a18 636f 6e74 726f 6c5f  .rv...Z.control_
-00001780: 6772 6f75 7073 5f63 6f6e 7461 696e 6572  groups_container
-00001790: 7226 0000 0072 2600 0000 7227 0000 00da  r&...r&...r'....
-000017a0: 1861 6464 5f61 6e6f 7468 6572 5f77 6964  .add_another_wid
-000017b0: 6765 745f 6772 6f75 70ed 0000 0073 1000  get_group....s..
-000017c0: 0000 0c02 0c01 0801 0c01 0a01 0a01 0a01  ................
-000017d0: 1201 7a2a 5061 7261 6d65 7465 7243 6f6e  ..z*ParameterCon
-000017e0: 7472 6f6c 732e 6164 645f 616e 6f74 6865  trols.add_anothe
-000017f0: 725f 7769 6467 6574 5f67 726f 7570 7278  r_widget_grouprx
-00001800: 0000 0072 1f00 0000 7277 0000 0072 0400  ...r....rw...r..
-00001810: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
-00001820: 0000 0003 0000 0043 0000 0173 4c00 0000  .......C...sL...
-00001830: 7400 7c00 7401 8302 7212 7402 7c01 8301  t.|.t...r.t.|...
-00001840: 7c00 5f03 7c01 9b00 6401 9d02 7c00 5f04  |._.|...d...|._.
-00001850: 6402 5300 7400 7c00 7405 8302 7224 7402  d.S.t.|.t...r$t.
-00001860: 7c01 8301 7c00 5f03 7c01 9b00 6401 9d02  |...|._.|...d...
-00001870: 7c00 5f06 6402 5300 6402 5300 2903 7a35  |._.d.S.d.S.).z5
-00001880: 5365 7420 7468 6520 6465 6661 756c 7420  Set the default 
-00001890: 7661 6c75 6520 6f66 2061 2070 6172 616d  value of a param
-000018a0: 6574 6572 2d68 616e 646c 696e 6720 7769  eter-handling wi
-000018b0: 6467 6574 2e7a 0a20 2864 6566 6175 6c74  dget.z. (default
-000018c0: 294e 2907 722c 0000 0072 1500 0000 7247  )N).r,...r....rG
-000018d0: 0000 00da 0576 616c 7565 da0b 706c 6163  .....value..plac
+00001080: 0000 0072 3900 0000 da04 7479 7065 da05  ...r9.....type..
+00001090: 7661 6c75 6572 4f00 0000 7258 0000 0072  valuerO...rX...r
+000010a0: 2c00 0000 721d 0000 00da 056e 6172 6773  ,...r......nargs
+000010b0: da20 5f6d 616b 655f 636f 6d6d 616e 645f  . _make_command_
+000010c0: 666f 726d 5f63 6f6e 7472 6f6c 5f6c 6162  form_control_lab
+000010d0: 656c da08 7265 7175 6972 6564 7229 0000  el..requiredr)..
+000010e0: 0072 3e00 0000 7216 0000 0072 5b00 0000  .r>...r....r[...
+000010f0: da12 6765 745f 636f 6e74 726f 6c5f 6d65  ..get_control_me
+00001100: 7468 6f64 721b 0000 00da 036b 6579 da06  thodr......key..
+00001110: 7661 6c75 6573 da04 6c69 7374 da11 6d61  values..list..ma
+00001120: 6b65 5f77 6964 6765 745f 6772 6f75 7072  ke_widget_groupr
+00001130: 2100 0000 da03 6c65 6eda 0961 6464 5f63  !.....len..add_c
+00001140: 6c61 7373 da03 7a69 70da 145f 6170 706c  lass..zip.._appl
+00001150: 795f 6465 6661 756c 745f 7661 6c75 6572  y_default_valuer
+00001160: 4300 0000 720f 0000 0072 1300 0000 7218  C...r....r....r.
+00001170: 0000 0029 1272 2e00 0000 7237 0000 0072  ...).r....r7...r
+00001180: 3900 0000 5a0d 6172 6775 6d65 6e74 5f74  9...Z.argument_t
+00001190: 7970 6572 5e00 0000 7256 0000 0072 5800  yper^...rV...rX.
+000011a0: 0000 da09 6973 5f6f 7074 696f 6e72 6800  ....is_optionrh.
+000011b0: 0000 725f 0000 005a 1366 6972 7374 5f66  ..r_...Z.first_f
+000011c0: 6f63 7573 5f63 6f6e 7472 6f6c da0e 636f  ocus_control..co
+000011d0: 6e74 726f 6c5f 6d65 7468 6f64 5a16 6d75  ntrol_methodZ.mu
+000011e0: 6c74 6970 6c65 5f63 686f 6963 655f 7769  ltiple_choice_wi
+000011f0: 6467 6574 5a13 6465 6661 756c 745f 7661  dgetZ.default_va
+00001200: 6c75 655f 7475 706c 65da 0c77 6964 6765  lue_tuple..widge
+00001210: 745f 6772 6f75 70da 0d63 6f6e 7472 6f6c  t_group..control
+00001220: 5f67 726f 7570 da0d 6465 6661 756c 745f  _group..default_
+00001230: 7661 6c75 65da 0e63 6f6e 7472 6f6c 5f77  value..control_w
+00001240: 6964 6765 7472 2600 0000 7226 0000 0072  idgetr&...r&...r
+00001250: 2700 0000 da07 636f 6d70 6f73 6563 0000  '.....composec..
+00001260: 0073 9200 0000 0280 0603 0601 0601 0601  .s..............
+00001270: 1001 0601 0a01 0601 0402 0201 0201 0201  ................
+00001280: 0401 0201 06fb 0208 02ff 0806 0801 0e01  ................
+00001290: 0a02 0405 0a01 06ff 0203 0201 0201 0201  ................
+000012a0: 0201 0401 06fb 0c07 0a04 0c01 0801 0c01  ................
+000012b0: 0a01 0206 0201 0201 0cfe 0c04 0601 0802  ................
+000012c0: 0401 0280 02f8 1cf8 0280 0a14 0c01 0801  ................
+000012d0: 0c01 0a01 0803 0601 0801 0401 0280 02fd  ................
+000012e0: 1cfb 0280 1cd1 0a3a 0601 1605 0c01 1201  .......:........
+000012f0: 1eff 0604 1201 04ff 7a19 5061 7261 6d65  ........z.Parame
+00001300: 7465 7243 6f6e 7472 6f6c 732e 636f 6d70  terControls.comp
+00001310: 6f73 65fa 1049 7465 7261 626c 655b 5769  ose..Iterable[Wi
+00001320: 6467 6574 5d63 0100 0000 0000 0000 0000  dget]c..........
+00001330: 0000 0c00 0000 0700 0000 2300 0001 73b0  ..........#...s.
+00001340: 0000 0081 007c 006a 007d 017c 016a 017d  .....|.j.}.|.j.}
+00001350: 027c 016a 0289 007c 016a 037d 037c 016a  .|.j...|.j.}.|.j
+00001360: 047d 047c 016a 057d 0574 067c 0174 0783  .}.|.j.}.t.|.t..
+00001370: 027d 067c 00a0 087c 0388 007c 067c 057c  .}.|...|...|.|.|
+00001380: 04a1 057d 0787 0066 0164 0164 0284 0874  ...}...f.d.d...t
+00001390: 097c 016a 0a64 036b 0472 2f7c 016a 0a6e  .|.j.d.k.r/|.j.n
+000013a0: 0164 0383 0144 0083 017d 087c 0844 005d  .d...D...}.|.D.]
+000013b0: 1f7d 097c 016a 0b72 4174 0c7c 016a 0b64  .}.|.j.rAt.|.j.d
+000013c0: 048d 017d 097c 006a 0d7c 0964 058d 017d  ...}.|.j.|.d...}
+000013d0: 0a7c 0a7c 027c 077c 047c 017c 016a 0e83  .|.|.|.|.|.|.j..
+000013e0: 057d 0b7c 0b45 0064 0648 0001 0071 3664  .}.|.E.d.H...q6d
+000013f0: 0653 0029 077a 5546 6f72 2074 6869 7320  .S.).zUFor this 
+00001400: 6f70 7469 6f6e 2c20 7969 656c 6420 6120  option, yield a 
+00001410: 7369 6e67 6c65 2073 6574 206f 6620 7769  single set of wi
+00001420: 6467 6574 7320 7265 7175 6972 6564 2074  dgets required t
+00001430: 6f20 7265 6365 6976 6520 7573 6572 2069  o receive user i
+00001440: 6e70 7574 2066 6f72 2069 742e 6301 0000  nput for it.c...
+00001450: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+00001460: 0013 0000 0173 2800 0000 6700 7c00 5d10  .....s(...g.|.].
+00001470: 7d01 7c01 7400 8800 8301 6b00 720e 8800  }.|.t.....k.r...
+00001480: 7c01 1900 6e03 8800 6400 1900 9102 7102  |...n...d.....q.
+00001490: 5300 2901 7263 0000 0029 0172 7000 0000  S.).rc...).rp...
+000014a0: a902 724b 0000 00da 0169 a901 5a0e 7061  ..rK.....i..Z.pa
+000014b0: 7261 6d65 7465 725f 7479 7065 7226 0000  rameter_typer&..
+000014c0: 0072 2700 0000 da0a 3c6c 6973 7463 6f6d  .r'.....<listcom
+000014d0: 703e d600 0000 7308 0000 0006 0002 021a  p>....s.........
+000014e0: ff06 ff7a 3750 6172 616d 6574 6572 436f  ...z7ParameterCo
+000014f0: 6e74 726f 6c73 2e6d 616b 655f 7769 6467  ntrols.make_widg
+00001500: 6574 5f67 726f 7570 2e3c 6c6f 6361 6c73  et_group.<locals
+00001510: 3e2e 3c6c 6973 7463 6f6d 703e 7261 0000  >.<listcomp>ra..
+00001520: 0072 5a00 0000 725c 0000 004e 290f 7237  .rZ...r\...N).r7
+00001530: 0000 0072 6700 0000 7266 0000 0072 3900  ...rg...rf...r9.
+00001540: 0000 7258 0000 0072 6a00 0000 722c 0000  ..rX...rj...r,..
+00001550: 0072 1d00 0000 7269 0000 00da 0572 616e  .r....ri.....ran
+00001560: 6765 7268 0000 0072 5b00 0000 721b 0000  gerh...r[...r...
+00001570: 0072 6b00 0000 726c 0000 0029 0c72 2e00  .rk...rl...).r..
+00001580: 0000 7237 0000 0072 5e00 0000 7239 0000  ..r7...r^...r9..
+00001590: 0072 5800 0000 726a 0000 0072 7400 0000  .rX...rj...rt...
+000015a0: 725f 0000 005a 0f70 6172 616d 6574 6572  r_...Z.parameter
+000015b0: 5f74 7970 6573 da05 5f74 7970 6572 7500  _types.._typeru.
+000015c0: 0000 5a0f 636f 6e74 726f 6c5f 7769 6467  ..Z.control_widg
+000015d0: 6574 7372 2600 0000 727e 0000 0072 2700  etsr&...r~...r'.
+000015e0: 0000 726f 0000 00c4 0000 0073 3e00 0000  ..ro.......s>...
+000015f0: 0280 0602 0601 0601 0601 0601 0601 0a01  ................
+00001600: 0401 0201 0201 0201 0201 0201 04fb 0a09  ................
+00001610: 1602 06fe 080a 0601 0c01 0c01 0201 0201  ................
+00001620: 0201 0201 0201 0401 04fb 0c07 04f5 7a23  ..............z#
+00001630: 5061 7261 6d65 7465 7243 6f6e 7472 6f6c  ParameterControl
+00001640: 732e 6d61 6b65 5f77 6964 6765 745f 6772  s.make_widget_gr
+00001650: 6f75 707a 132e 6164 642d 616e 6f74 6865  oupz..add-anothe
+00001660: 722d 6275 7474 6f6e da05 6576 656e 74fa  r-button..event.
+00001670: 0e42 7574 746f 6e2e 5072 6573 7365 6463  .Button.Pressedc
+00001680: 0200 0000 0000 0000 0000 0000 0500 0000  ................
+00001690: 0300 0000 4300 0001 735c 0000 0074 007c  ....C...s\...t.|
+000016a0: 00a0 01a1 0083 017d 027c 0264 0119 00a0  .......}.|.d....
+000016b0: 02a1 0001 0074 037c 028e 007d 0374 047c  .....t.|...}.t.|
+000016c0: 0283 0164 026b 0172 1b7c 03a0 0564 03a1  ...d.k.r.|...d..
+000016d0: 0101 007c 00a0 0674 07a1 017d 047c 04a0  ...|...t...}.|..
+000016e0: 087c 03a1 0101 007c 016a 096a 0a64 0464  .|.....|.j.j.d.d
+000016f0: 058d 0101 0064 0053 0029 064e 7201 0000  .....d.S.).Nr...
+00001700: 0072 6100 0000 7262 0000 0046 2901 da07  .ra...rb...F)...
+00001710: 616e 696d 6174 6529 0b72 6e00 0000 726f  animate).rn...ro
+00001720: 0000 00da 0566 6f63 7573 7221 0000 0072  .....focusr!...r
+00001730: 7000 0000 7271 0000 0072 5200 0000 7229  p...rq...rR...r)
+00001740: 0000 00da 056d 6f75 6e74 da06 6275 7474  .....mount..butt
+00001750: 6f6e da0e 7363 726f 6c6c 5f76 6973 6962  on..scroll_visib
+00001760: 6c65 2905 722e 0000 0072 8200 0000 7276  le).r....r....rv
+00001770: 0000 0072 7700 0000 5a18 636f 6e74 726f  ...rw...Z.contro
+00001780: 6c5f 6772 6f75 7073 5f63 6f6e 7461 696e  l_groups_contain
+00001790: 6572 7226 0000 0072 2600 0000 7227 0000  err&...r&...r'..
+000017a0: 00da 1861 6464 5f61 6e6f 7468 6572 5f77  ...add_another_w
+000017b0: 6964 6765 745f 6772 6f75 70ed 0000 0073  idget_group....s
+000017c0: 1000 0000 0c02 0c01 0801 0c01 0a01 0a01  ................
+000017d0: 0a01 1201 7a2a 5061 7261 6d65 7465 7243  ....z*ParameterC
+000017e0: 6f6e 7472 6f6c 732e 6164 645f 616e 6f74  ontrols.add_anot
+000017f0: 6865 725f 7769 6467 6574 5f67 726f 7570  her_widget_group
+00001800: 7279 0000 0072 1f00 0000 7278 0000 0072  ry...r....rx...r
+00001810: 0400 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00001820: 0002 0000 0003 0000 0043 0000 0173 4c00  .........C...sL.
+00001830: 0000 7400 7c00 7401 8302 7212 7402 7c01  ..t.|.t...r.t.|.
+00001840: 8301 7c00 5f03 7c01 9b00 6401 9d02 7c00  ..|._.|...d...|.
+00001850: 5f04 6402 5300 7400 7c00 7405 8302 7224  _.d.S.t.|.t...r$
+00001860: 7402 7c01 8301 7c00 5f03 7c01 9b00 6401  t.|...|._.|...d.
+00001870: 9d02 7c00 5f06 6402 5300 6402 5300 2903  ..|._.d.S.d.S.).
+00001880: 7a35 5365 7420 7468 6520 6465 6661 756c  z5Set the defaul
+00001890: 7420 7661 6c75 6520 6f66 2061 2070 6172  t value of a par
+000018a0: 616d 6574 6572 2d68 616e 646c 696e 6720  ameter-handling 
+000018b0: 7769 6467 6574 2e7a 0a20 2864 6566 6175  widget.z. (defau
+000018c0: 6c74 294e 2907 722c 0000 0072 1500 0000  lt)N).r,...r....
+000018d0: 7247 0000 0072 6700 0000 da0b 706c 6163  rG...rg.....plac
 000018e0: 6568 6f6c 6465 7272 1700 0000 da06 7072  eholderr......pr
-000018f0: 6f6d 7074 2902 7278 0000 0072 7700 0000  ompt).rx...rw...
+000018f0: 6f6d 7074 2902 7279 0000 0072 7800 0000  ompt).ry...rx...
 00001900: 7226 0000 0072 2600 0000 7227 0000 0072  r&...r&...r'...r
-00001910: 7200 0000 f800 0000 730e 0000 000a 060a  r.......s.......
+00001910: 7300 0000 f800 0000 730e 0000 000a 060a  s.......s.......
 00001920: 0110 010a 010a 0110 0104 fe7a 2650 6172  ...........z&Par
 00001930: 616d 6574 6572 436f 6e74 726f 6c73 2e5f  ameterControls._
 00001940: 6170 706c 795f 6465 6661 756c 745f 7661  apply_default_va
 00001950: 6c75 65da 0763 6f6e 7472 6f6c 6301 0000  lue..controlc...
 00001960: 0000 0000 0000 0000 0001 0000 0003 0000  ................
 00001970: 0043 0000 0173 6400 0000 7400 7c00 7401  .C...sd...t.|.t.
 00001980: 8302 7208 7c00 6a02 5300 7400 7c00 7403  ..r.|.j.S.t.|.t.
 00001990: 8302 7218 7c00 6a04 6400 7500 7215 7405  ..r.|.j.d.u.r.t.
 000019a0: 8300 5300 7c00 6a04 5300 7400 7c00 7406  ..S.|.j.S.t.|.t.
 000019b0: 8302 7228 7c00 6a04 6401 6b02 7225 7405  ..r(|.j.d.k.r%t.
 000019c0: 8300 5300 7c00 6a04 5300 7400 7c00 7407  ..S.|.j.S.t.|.t.
 000019d0: 8302 7230 7c00 6a04 5300 6400 5300 2902  ..r0|.j.S.d.S.).
 000019e0: 4e72 4900 0000 2908 722c 0000 0072 1e00  NrI...).r,...r..
 000019f0: 0000 da08 7365 6c65 6374 6564 7217 0000  ....selectedr...
-00001a00: 0072 8900 0000 722a 0000 0072 1500 0000  .r....r*...r....
+00001a00: 0072 6700 0000 722a 0000 0072 1500 0000  .rg...r*...r....
 00001a10: 7214 0000 0029 0172 8c00 0000 7226 0000  r....).r....r&..
 00001a20: 0072 2600 0000 7227 0000 00da 175f 6765  .r&...r'....._ge
 00001a30: 745f 666f 726d 5f63 6f6e 7472 6f6c 5f76  t_form_control_v
 00001a40: 616c 7565 0501 0000 731c 0000 000a 0206  alue....s.......
 00001a50: 010a 010a 0106 0106 010a 010e 0202 ff04  ................
 00001a60: 0102 ff0a 0306 0104 ff7a 2950 6172 616d  .........z)Param
 00001a70: 6574 6572 436f 6e74 726f 6c73 2e5f 6765  eterControls._ge
@@ -448,39 +448,39 @@
 00001bf0: 0087 0166 0264 0464 0584 0874 0164 0174  ...f.d.d...t.d.t
 00001c00: 0288 0083 0188 0183 0344 0083 0153 0029  .........D...S.)
 00001c10: 064e 7201 0000 0072 6300 0000 7261 0000  .Nr....rc...ra..
 00001c20: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
 00001c30: 0000 0700 0000 1300 0001 7320 0000 0067  ..........s ...g
 00001c40: 007c 005d 0c7d 0174 0088 007c 017c 0188  .|.].}.t...|.|..
 00001c50: 0117 0085 0219 0083 0191 0271 0253 0072  ...........q.S.r
-00001c60: 2600 0000 2901 da05 7475 706c 6572 7b00  &...)...tupler{.
+00001c60: 2600 0000 2901 da05 7475 706c 6572 7c00  &...)...tupler|.
 00001c70: 0000 a902 728f 0000 0072 9100 0000 7226  ....r....r....r&
-00001c80: 0000 0072 2700 0000 727e 0000 0021 0100  ...r'...r~...!..
+00001c80: 0000 0072 2700 0000 727f 0000 0021 0100  ...r'...r....!..
 00001c90: 0073 0600 0000 0600 1401 06ff 7a48 5061  .s..........zHPa
 00001ca0: 7261 6d65 7465 7243 6f6e 7472 6f6c 732e  rameterControls.
 00001cb0: 6765 745f 7661 6c75 6573 2e3c 6c6f 6361  get_values.<loca
 00001cc0: 6c73 3e2e 6c69 7374 5f74 6f5f 7475 706c  ls>.list_to_tupl
 00001cd0: 6573 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  es.<locals>.<lis
-00001ce0: 7463 6f6d 703e 2903 7294 0000 0072 7f00  tcomp>).r....r..
-00001cf0: 0000 726f 0000 0072 9500 0000 7226 0000  ..ro...r....r&..
+00001ce0: 7463 6f6d 703e 2903 7294 0000 0072 8000  tcomp>).r....r..
+00001cf0: 0000 7270 0000 0072 9500 0000 7226 0000  ..rp...r....r&..
 00001d00: 0072 9500 0000 7227 0000 00da 0e6c 6973  .r....r'.....lis
 00001d10: 745f 746f 5f74 7570 6c65 7318 0100 0073  t_to_tuples....s
 00001d20: 0e00 0000 0804 0801 0801 0402 0c01 0e01  ................
 00001d30: 06ff 7a34 5061 7261 6d65 7465 7243 6f6e  ..z4ParameterCon
 00001d40: 7472 6f6c 732e 6765 745f 7661 6c75 6573  trols.get_values
 00001d50: 2e3c 6c6f 6361 6c73 3e2e 6c69 7374 5f74  .<locals>.list_t
 00001d60: 6f5f 7475 706c 6573 da01 2e72 6100 0000  o_tuples...ra...
 00001d70: 7201 0000 0029 0672 8f00 0000 7290 0000  r....).r....r...
 00001d80: 0072 9100 0000 7292 0000 0072 3f00 0000  .r....r....r?...
-00001d90: 7293 0000 0029 0e72 6d00 0000 da05 7175  r....).rm.....qu
-00001da0: 6572 7972 3700 0000 726b 0000 0072 6f00  eryr7...rk...ro.
+00001d90: 7293 0000 0029 0e72 6e00 0000 da05 7175  r....).rn.....qu
+00001da0: 6572 7972 3700 0000 726c 0000 0072 7000  eryr7...rl...rp.
 00001db0: 0000 722c 0000 0072 1e00 0000 720a 0000  ..r,...r....r...
 00001dc0: 0072 8e00 0000 721c 0000 00da 1270 726f  .r....r......pro
 00001dd0: 6365 7373 5f63 6c69 5f6f 7074 696f 6eda  cess_cli_option.
-00001de0: 0661 7070 656e 64da 036d 6178 7267 0000  .append..maxrg..
+00001de0: 0661 7070 656e 64da 036d 6178 7268 0000  .append..maxrh..
 00001df0: 0029 0672 2e00 0000 7296 0000 005a 0863  .).r....r....Z.c
 00001e00: 6f6e 7472 6f6c 7372 8c00 0000 5a0e 636f  ontrolsr....Z.co
 00001e10: 6e74 726f 6c5f 7661 6c75 6573 5a10 636f  ntrol_valuesZ.co
 00001e20: 6c6c 6563 7465 645f 7661 6c75 6573 7226  llected_valuesr&
 00001e30: 0000 0072 2600 0000 7227 0000 00da 0a67  ...r&...r'.....g
 00001e40: 6574 5f76 616c 7565 7314 0100 0073 1e00  et_values....s..
 00001e50: 0000 0a04 180d 1a02 0e06 0a01 0a01 0403  ................
@@ -501,15 +501,15 @@
 00001f40: 0000 721b 0000 0072 0300 0000 da13 6d61  ..r....r......ma
 00001f50: 6b65 5f63 686f 6963 655f 636f 6e74 726f  ke_choice_contro
 00001f60: 6c72 5b00 0000 723e 0000 00da 156d 616b  lr[...r>.....mak
 00001f70: 655f 6368 6563 6b62 6f78 5f63 6f6e 7472  e_checkbox_contr
 00001f80: 6f6c da11 6d61 6b65 5f74 6578 745f 636f  ol..make_text_co
 00001f90: 6e74 726f 6c29 0272 2e00 0000 725d 0000  ntrol).r....r]..
 00001fa0: 0072 2600 0000 7226 0000 0072 2700 0000  .r&...r&...r'...
-00001fb0: 726a 0000 0042 0100 0073 0a00 0000 0a04  rj...B...s......
+00001fb0: 726b 0000 0042 0100 0073 0a00 0000 0a04  rk...B...s......
 00001fc0: 1001 0802 0601 0602 7a24 5061 7261 6d65  ........z$Parame
 00001fd0: 7465 7243 6f6e 7472 6f6c 732e 6765 745f  terControls.get_
 00001fe0: 636f 6e74 726f 6c5f 6d65 7468 6f64 725e  control_methodr^
 00001ff0: 0000 0072 5f00 0000 fa0b 5465 7874 207c  ...r_.....Text |
 00002000: 204e 6f6e 6572 5800 0000 fa1d 4f70 7469   NonerX.....Opti
 00002010: 6f6e 5363 6865 6d61 207c 2041 7267 756d  onSchema | Argum
 00002020: 656e 7453 6368 656d 6172 6000 0000 7212  entSchemar`...r.
@@ -535,15 +535,15 @@
 00002160: 006a 0072 0c7c 006a 0064 0119 0064 0119  .j.r.|.j.d...d..
 00002170: 007d 006e 0374 0183 007d 0074 027c 0164  .}.n.t...}.t.|.d
 00002180: 0264 037c 049b 009d 027c 0064 048d 047d  .d.|.....|.d...}
 00002190: 057c 0556 0001 007c 0553 0029 054e 7201  .|.V...|.S.).Nr.
 000021a0: 0000 0054 7a16 636f 6d6d 616e 642d 666f  ...Tz.command-fo
 000021b0: 726d 2d63 6865 636b 626f 7820 2903 5a0c  rm-checkbox ).Z.
 000021c0: 6275 7474 6f6e 5f66 6972 7374 723c 0000  button_firstr<..
-000021d0: 0072 8900 0000 2903 726c 0000 0072 2a00  .r....).rl...r*.
+000021d0: 0072 6700 0000 2903 726d 0000 0072 2a00  .rg...).rm...r*.
 000021e0: 0000 7214 0000 0072 a700 0000 7226 0000  ..r....r....r&..
 000021f0: 0072 2600 0000 7227 0000 0072 a000 0000  .r&...r'...r....
 00002200: 5f01 0000 7318 0000 0002 8006 0810 0106  _...s...........
 00002210: 0202 0202 0102 0108 0102 0106 fc06 0604  ................
 00002220: 017a 2750 6172 616d 6574 6572 436f 6e74  .z'ParameterCont
 00002230: 726f 6c73 2e6d 616b 655f 6368 6563 6b62  rols.make_checkb
 00002240: 6f78 5f63 6f6e 7472 6f6c 725b 0000 00fa  ox_controlr[....
@@ -560,35 +560,35 @@
 000022f0: 6c65 2d63 686f 6963 6520 2902 723c 0000  le-choice ).r<..
 00002300: 00da 0864 6566 6175 6c74 7363 0100 0000  ...defaultsc....
 00002310: 0000 0000 0000 0000 0200 0000 0400 0000  ................
 00002320: 5300 0001 7314 0000 0067 007c 005d 067d  S...s....g.|.].}
 00002330: 017c 017c 0166 0291 0271 0253 0072 2600  .|.|.f...q.S.r&.
 00002340: 0000 7226 0000 0029 0272 4b00 0000 da06  ..r&...).rK.....
 00002350: 6368 6f69 6365 7226 0000 0072 2600 0000  choicer&...r&...
-00002360: 7227 0000 0072 7e00 0000 8c01 0000 f302  r'...r~.........
+00002360: 7227 0000 0072 7f00 0000 8c01 0000 f302  r'...r..........
 00002370: 0000 0014 007a 3950 6172 616d 6574 6572  .....z9Parameter
 00002380: 436f 6e74 726f 6c73 2e6d 616b 655f 6368  Controls.make_ch
 00002390: 6f69 6365 5f63 6f6e 7472 6f6c 2e3c 6c6f  oice_control.<lo
 000023a0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
 000023b0: 7a14 2063 6f6d 6d61 6e64 2d66 6f72 6d2d  z. command-form-
-000023c0: 7365 6c65 6374 7259 0000 0029 0472 6700  selectrY...).rg.
-000023d0: 0000 721e 0000 0072 6c00 0000 7217 0000  ..r....rl...r...
+000023c0: 7365 6c65 6374 7259 0000 0029 0472 6800  selectrY...).rh.
+000023d0: 0000 721e 0000 0072 6d00 0000 7217 0000  ..r....rm...r...
 000023e0: 0029 0872 5e00 0000 725f 0000 0072 5800  .).r^...r_...rX.
 000023f0: 0000 7237 0000 0072 6000 0000 725b 0000  ..r7...r`...r[..
 00002400: 005a 0c6d 756c 7469 5f63 686f 6963 65da  .Z.multi_choice.
 00002410: 0673 656c 6563 7472 2600 0000 7226 0000  .selectr&...r&..
 00002420: 0072 2700 0000 729f 0000 0075 0100 0073  .r'...r....u...s
 00002430: 2200 0000 0280 0a0a 0401 0402 0201 0201  "...............
 00002440: 0801 0401 06fd 0605 0401 0202 0c01 0801  ................
 00002450: 06fe 0604 0401 7a25 5061 7261 6d65 7465  ......z%Paramete
 00002460: 7243 6f6e 7472 6f6c 732e 6d61 6b65 5f63  rControls.make_c
 00002470: 686f 6963 655f 636f 6e74 726f 6cfa 0f73  hoice_control..s
 00002480: 7472 207c 206c 6973 745b 7374 725d da05  tr | list[str]..
 00002490: 7479 7065 73fa 0f6c 6973 745b 5479 7065  types..list[Type
-000024a0: 5b41 6e79 5d5d 7273 0000 00da 0b69 735f  [Any]]rs.....is_
+000024a0: 5b41 6e79 5d5d 7274 0000 00da 0b69 735f  [Any]]rt.....is_
 000024b0: 7265 7175 6972 6564 720c 0000 0063 0500  requiredr....c..
 000024c0: 0000 0000 0000 0000 0000 0700 0000 0a00  ................
 000024d0: 0000 4300 0001 7374 0000 0074 007c 0074  ..C...st...t.|.t
 000024e0: 0183 0272 087c 0067 016e 017c 007d 0574  ...r.|.g.n.|.}.t
 000024f0: 0264 0164 0264 038d 02a0 0364 0464 0584  .d.d.d.....d.d..
 00002500: 007c 0544 0083 01a1 017d 0574 02a0 047c  .|.D.....}.t...|
 00002510: 059b 0064 067c 0472 2164 076e 0164 089b  ...d.|.r!d.n.d..
@@ -597,15 +597,15 @@
 00002540: 0164 089b 009d 07a1 017d 067c 0653 0029  .d.......}.|.S.)
 00002550: 0f4e 7a03 202f 20da 0364 696d 2901 da05  .Nz. / ..dim)...
 00002560: 7374 796c 6563 0100 0000 0000 0000 0000  stylec..........
 00002570: 0000 0200 0000 0400 0000 5300 0001 7314  ..........S...s.
 00002580: 0000 0067 007c 005d 067d 0174 007c 0183  ...g.|.].}.t.|..
 00002590: 0191 0271 0253 0072 2600 0000 720b 0000  ...q.S.r&...r...
 000025a0: 0029 0272 4b00 0000 da01 6e72 2600 0000  .).rK.....nr&...
-000025b0: 7226 0000 0072 2700 0000 727e 0000 009c  r&...r'...r~....
+000025b0: 7226 0000 0072 2700 0000 727f 0000 009c  r&...r'...r.....
 000025c0: 0100 0072 ab00 0000 7a46 5061 7261 6d65  ...r....zFParame
 000025d0: 7465 7243 6f6e 7472 6f6c 732e 5f6d 616b  terControls._mak
 000025e0: 655f 636f 6d6d 616e 645f 666f 726d 5f63  e_command_form_c
 000025f0: 6f6e 7472 6f6c 5f6c 6162 656c 2e3c 6c6f  ontrol_label.<lo
 00002600: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
 00002610: 7a05 5b64 696d 5d7a 0920 6d75 6c74 6970  z.[dim]z. multip
 00002620: 6c65 7249 0000 007a 0220 3c7a 022c 2063  lerI...z. <z., c
@@ -620,42 +620,42 @@
 000026b0: 616b 655f 636f 6d6d 616e 645f 666f 726d  ake_command_form
 000026c0: 5f63 6f6e 7472 6f6c 5f6c 6162 656c 2e3c  _control_label.<
 000026d0: 6c6f 6361 6c73 3e2e 3c67 656e 6578 7072  locals>.<genexpr
 000026e0: 3e7a 053e 5b2f 5d20 7a14 205b 6220 7265  >z.>[/] z. [b re
 000026f0: 645d 2a5b 2f5d 7265 7175 6972 6564 2905  d]*[/]required).
 00002700: 722c 0000 0072 4700 0000 720c 0000 00da  r,...rG...r.....
 00002710: 046a 6f69 6eda 0b66 726f 6d5f 6d61 726b  .join..from_mark
-00002720: 7570 2907 7239 0000 0072 ae00 0000 7273  up).r9...r....rs
+00002720: 7570 2907 7239 0000 0072 ae00 0000 7274  up).r9...r....rt
 00002730: 0000 0072 b000 0000 7258 0000 00da 056e  ...r....rX.....n
 00002740: 616d 6573 da04 7465 7874 7226 0000 0072  ames..textr&...r
-00002750: 2600 0000 7227 0000 0072 6800 0000 9201  &...r'...rh.....
+00002750: 2600 0000 7227 0000 0072 6900 0000 9201  &...r'...ri.....
 00002760: 0000 730c 0000 0014 081c 0204 0138 0104  ..s..........8..
 00002770: ff04 047a 3250 6172 616d 6574 6572 436f  ...z2ParameterCo
 00002780: 6e74 726f 6c73 2e5f 6d61 6b65 5f63 6f6d  ntrols._make_com
 00002790: 6d61 6e64 5f66 6f72 6d5f 636f 6e74 726f  mand_form_contro
-000027a0: 6c5f 6c61 6265 6c54 7287 0000 0063 0200  l_labelTr....c..
+000027a0: 6c5f 6c61 6265 6c54 7288 0000 0063 0200  l_labelTr....c..
 000027b0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
 000027c0: 0000 4300 0001 731c 0000 007c 006a 0064  ..C...s....|.j.d
 000027d0: 0075 0172 0c7c 006a 00a0 01a1 0001 0064  .u.r.|.j.......d
 000027e0: 0053 0064 0053 0072 2b00 0000 2902 7243  .S.d.S.r+...).rC
-000027f0: 0000 0072 8400 0000 2902 722e 0000 0072  ...r....).r....r
-00002800: 8700 0000 7226 0000 0072 2600 0000 7227  ....r&...r&...r'
-00002810: 0000 0072 8400 0000 a301 0000 7306 0000  ...r........s...
+000027f0: 0000 0072 8500 0000 2902 722e 0000 0072  ...r....).r....r
+00002800: 8800 0000 7226 0000 0072 2600 0000 7227  ....r&...r&...r'
+00002810: 0000 0072 8500 0000 a301 0000 7306 0000  ...r........s...
 00002820: 000a 010e 0104 ff7a 1750 6172 616d 6574  .......z.Paramet
 00002830: 6572 436f 6e74 726f 6c73 2e66 6f63 7573  erControls.focus
 00002840: 2904 4e4e 4e46 290c 7237 0000 0072 3800  ).NNNF).r7...r8.
 00002850: 0000 7239 0000 0072 3a00 0000 723b 0000  ..r9...r:...r;..
 00002860: 0072 3a00 0000 723c 0000 0072 3a00 0000  .r:...r<...r:...
 00002870: 723d 0000 0072 3e00 0000 723f 0000 0072  r=...r>...r?...r
 00002880: 4000 0000 2904 7246 0000 0072 4700 0000  @...).rF...rG...
 00002890: 723f 0000 0072 3e00 0000 2902 723f 0000  r?...r>...).r?..
-000028a0: 0072 0e00 0000 2902 723f 0000 0072 7a00  .r....).r?...rz.
-000028b0: 0000 2904 7281 0000 0072 8200 0000 723f  ..).r....r....r?
-000028c0: 0000 0072 4000 0000 2906 7278 0000 0072  ...r@...).rx...r
-000028d0: 1f00 0000 7277 0000 0072 0400 0000 723f  ....rw...r....r?
+000028a0: 0072 0e00 0000 2902 723f 0000 0072 7b00  .r....).r?...r{.
+000028b0: 0000 2904 7282 0000 0072 8300 0000 723f  ..).r....r....r?
+000028c0: 0000 0072 4000 0000 2906 7279 0000 0072  ...r@...).ry...r
+000028d0: 1f00 0000 7278 0000 0072 0400 0000 723f  ....rx...r....r?
 000028e0: 0000 0072 4000 0000 2904 728c 0000 0072  ...r@...).r....r
 000028f0: 1f00 0000 723f 0000 0072 0400 0000 2902  ....r?...r....).
 00002900: 723f 0000 0072 1c00 0000 2904 725d 0000  r?...r....).r]..
 00002910: 0072 9d00 0000 723f 0000 0072 9e00 0000  .r....r?...r....
 00002920: 290c 725e 0000 0072 0400 0000 725f 0000  ).r^...r....r_..
 00002930: 0072 a200 0000 7258 0000 0072 3e00 0000  .r....rX...r>...
 00002940: 7237 0000 0072 a300 0000 7260 0000 0072  r7...r....r`...r
@@ -665,26 +665,26 @@
 00002980: 0000 0072 a300 0000 7260 0000 0072 4700  ...r....r`...rG.
 00002990: 0000 723f 0000 0072 1200 0000 290e 725e  ..r?...r....).r^
 000029a0: 0000 0072 1c00 0000 725f 0000 0072 a200  ...r....r_...r..
 000029b0: 0000 7258 0000 0072 3e00 0000 7237 0000  ..rX...r>...r7..
 000029c0: 0072 a300 0000 7260 0000 0072 4700 0000  .r....r`...rG...
 000029d0: 725b 0000 0072 a800 0000 723f 0000 0072  r[...r....r?...r
 000029e0: 1200 0000 290c 7239 0000 0072 ad00 0000  ....).r9...r....
-000029f0: 72ae 0000 0072 af00 0000 7273 0000 0072  r....r....rs...r
+000029f0: 72ae 0000 0072 af00 0000 7274 0000 0072  r....r....rt...r
 00002a00: 3e00 0000 72b0 0000 0072 3e00 0000 7258  >...r....r>...rX
 00002a10: 0000 0072 3e00 0000 723f 0000 0072 0c00  ...r>...r?...r..
-00002a20: 0000 2901 5429 0272 8700 0000 723e 0000  ..).T).r....r>..
+00002a20: 0000 2901 5429 0272 8800 0000 723e 0000  ..).T).r....r>..
 00002a30: 0029 1672 2300 0000 7224 0000 0072 2500  .).r#...r$...r%.
-00002a40: 0000 7242 0000 0072 5700 0000 7279 0000  ..rB...rW...ry..
-00002a50: 0072 6e00 0000 720d 0000 0072 1300 0000  .rn...r....r....
-00002a60: da07 5072 6573 7365 6472 8800 0000 da0c  ..Pressedr......
-00002a70: 7374 6174 6963 6d65 7468 6f64 7272 0000  staticmethodrr..
-00002a80: 0072 8e00 0000 729c 0000 0072 6a00 0000  .r....r....rj...
+00002a40: 0000 7242 0000 0072 5700 0000 727a 0000  ..rB...rW...rz..
+00002a50: 0072 6f00 0000 720d 0000 0072 1300 0000  .ro...r....r....
+00002a60: da07 5072 6573 7365 6472 8900 0000 da0c  ..Pressedr......
+00002a70: 7374 6174 6963 6d65 7468 6f64 7273 0000  staticmethodrs..
+00002a80: 0072 8e00 0000 729c 0000 0072 6b00 0000  .r....r....rk...
 00002a90: 72a1 0000 0072 a000 0000 729f 0000 0072  r....r....r....r
-00002aa0: 6800 0000 7284 0000 00da 0d5f 5f63 6c61  h...r......__cla
+00002aa0: 6900 0000 7285 0000 00da 0d5f 5f63 6c61  i...r......__cla
 00002ab0: 7373 6365 6c6c 5f5f 7226 0000 0072 2600  sscell__r&...r&.
 00002ac0: 0000 7244 0000 0072 2700 0000 7236 0000  ..rD...r'...r6..
 00002ad0: 0029 0000 0073 3400 0000 0800 0204 0201  .)...s4.........
 00002ae0: 0201 0201 10fa 0a0c 0a2d 0a61 0a29 0c01  .........-.a.)..
 00002af0: 020a 0c01 020c 0c01 0a0e 0a2e 020c 0c01  ................
 00002b00: 0210 0c01 0215 0c01 021c 0c01 1410 7236  ..............r6
 00002b10: 0000 0029 2eda 0a5f 5f66 7574 7572 655f  ...)...__future_
```

### Comparing `argparse-tui-0.1.3/src/argparse_tui/widgets/about.py` & `argparse-tui-0.2.0/src/argparse_tui/widgets/about.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.3/src/argparse_tui/widgets/command_info.py` & `argparse-tui-0.2.0/src/argparse_tui/widgets/command_info.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.3/src/argparse_tui/widgets/command_tree.py` & `argparse-tui-0.2.0/src/argparse_tui/widgets/command_tree.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.3/src/argparse_tui/widgets/form.py` & `argparse-tui-0.2.0/src/argparse_tui/widgets/form.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.3/src/argparse_tui/widgets/multiple_choice.py` & `argparse-tui-0.2.0/src/argparse_tui/widgets/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.3/src/argparse_tui/widgets/parameter_controls.py` & `argparse-tui-0.2.0/src/argparse_tui/widgets/parameter_controls.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
     def compose(self) -> ComposeResult:
         """Takes the schemas for each parameter of the current command, and converts it into a
         form consisting of Textual widgets."""
         schema = self.schema
         name = schema.name
         argument_type = schema.type
-        default = schema.default
+        default = schema.value
         help_text = getattr(schema, "help", "") or ""
         multiple = schema.multiple
         is_option = isinstance(schema, OptionSchema)
         nargs = schema.nargs
 
         label = self._make_command_form_control_label(
             name,
@@ -192,15 +192,15 @@
         # Render the dim help text below the form controls
         if help_text:
             yield Static(help_text, classes="command-form-control-help-text")
 
     def make_widget_group(self) -> Iterable[Widget]:
         """For this option, yield a single set of widgets required to receive user input for it."""
         schema = self.schema
-        default = schema.default
+        default = schema.value
         parameter_type = schema.type
         name = schema.name
         multiple = schema.multiple
         required = schema.required
         is_option = isinstance(schema, OptionSchema)
         label = self._make_command_form_control_label(
             name,
```

### Comparing `argparse-tui-0.1.3/src/argparse_tui.egg-info/PKG-INFO` & `argparse-tui-0.2.0/src/argparse_tui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argparse-tui
-Version: 0.1.3
+Version: 0.2.0
 Summary: Display your Python argparse parser as a TUI.
 Author-email: Donald Mellenbruch <hello@f2dv.com>
 License: Copyright 2023 Donald Mellenbruch
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `argparse-tui-0.1.3/src/argparse_tui.egg-info/SOURCES.txt` & `argparse-tui-0.2.0/src/argparse_tui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.3/src/argparse_tui.egg-info/requires.txt` & `argparse-tui-0.2.0/src/argparse_tui.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.3/tests/test_help_argparse.py` & `argparse-tui-0.2.0/tests/test_help_argparse.py`

 * *Files 21% similar despite different names*

```diff
@@ -33,26 +33,26 @@
 
 def test_default_help_argument(capsys):
     parser = argparse.ArgumentParser()
     add_tui_argument(parser)
     parser.print_help()
 
     result = capsys.readouterr()
-    assert re.search(r"--tui\s+\[CMD\]\s+Open Textual UI", result.out) is not None
+    assert re.search(r"--tui\s+Open Textual UI", result.out) is not None
 
 
 def test_custom_command_argument(capsys):
     parser = argparse.ArgumentParser()
     add_tui_argument(parser, option_strings="--custom")
     parser.print_help()
 
     result = capsys.readouterr()
-    assert re.search(r"--custom\s+\[CMD\]\s+Open Textual UI", result.out) is not None
+    assert re.search(r"--custom\s+Open Textual UI", result.out) is not None
 
 
 def test_custom_help_argument(capsys):
     parser = argparse.ArgumentParser()
     add_tui_argument(parser, help="Custom help")
     parser.print_help()
 
     result = capsys.readouterr()
-    assert re.search(r"--tui\s+\[CMD\]\s+Custom help", result.out) is not None
+    assert re.search(r"--tui\s+Custom help", result.out) is not None
```

### Comparing `argparse-tui-0.1.3/tests/test_run_command.py` & `argparse-tui-0.2.0/tests/test_run_command.py`

 * *Files identical despite different names*

