# Comparing `tmp/color-pprint-0.0.2.tar.gz` & `tmp/color-pprint-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "color-pprint-0.0.2.tar", last modified: Sat Jun 24 21:46:34 2023, max compression
+gzip compressed data, was "color-pprint-0.0.3.tar", last modified: Fri Jul 28 23:45:16 2023, max compression
```

## Comparing `color-pprint-0.0.2.tar` & `color-pprint-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 21:46:34.798798 color-pprint-0.0.2/
--rw-rw-rw-   0        0        0     1103 2022-11-17 15:06:57.000000 color-pprint-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       85 2022-11-17 14:36:53.000000 color-pprint-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2665 2023-06-24 21:46:34.799798 color-pprint-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1343 2022-11-17 18:47:11.000000 color-pprint-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 21:46:34.781809 color-pprint-0.0.2/color_pprint/
--rw-rw-rw-   0        0        0     1165 2022-11-17 15:06:57.000000 color-pprint-0.0.2/color_pprint/__init__.py
--rw-rw-rw-   0        0        0     5448 2022-11-18 00:13:51.000000 color-pprint-0.0.2/color_pprint/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:46:34.796800 color-pprint-0.0.2/color_pprint/ansi/
--rw-rw-rw-   0        0        0    11333 2023-06-24 21:33:23.000000 color-pprint-0.0.2/color_pprint/ansi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:46:34.794800 color-pprint-0.0.2/color_pprint.egg-info/
--rw-rw-rw-   0        0        0     2665 2023-06-24 21:46:34.000000 color-pprint-0.0.2/color_pprint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-06-24 21:46:34.000000 color-pprint-0.0.2/color_pprint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 21:46:34.000000 color-pprint-0.0.2/color_pprint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-06-24 21:46:34.000000 color-pprint-0.0.2/color_pprint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-24 21:46:34.000000 color-pprint-0.0.2/color_pprint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2022-11-17 17:54:03.000000 color-pprint-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-24 21:46:34.801796 color-pprint-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-06-24 21:38:58.000000 color-pprint-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:45:16.174033 color-pprint-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-28 23:44:58.000000 color-pprint-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-28 23:44:58.000000 color-pprint-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-28 23:45:16.174033 color-pprint-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-28 23:44:58.000000 color-pprint-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:45:16.174033 color-pprint-0.0.3/color_pprint/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-28 23:44:58.000000 color-pprint-0.0.3/color_pprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-28 23:44:58.000000 color-pprint-0.0.3/color_pprint/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:45:16.174033 color-pprint-0.0.3/color_pprint/ansi/
+-rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-07-28 23:44:58.000000 color-pprint-0.0.3/color_pprint/ansi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:45:16.174033 color-pprint-0.0.3/color_pprint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-28 23:45:16.000000 color-pprint-0.0.3/color_pprint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-28 23:45:16.000000 color-pprint-0.0.3/color_pprint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 23:45:16.000000 color-pprint-0.0.3/color_pprint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 23:45:16.000000 color-pprint-0.0.3/color_pprint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 23:45:16.000000 color-pprint-0.0.3/color_pprint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 23:44:58.000000 color-pprint-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 23:45:16.174033 color-pprint-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-28 23:44:58.000000 color-pprint-0.0.3/setup.py
```

### Comparing `color-pprint-0.0.2/LICENSE` & `color-pprint-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `color-pprint-0.0.2/PKG-INFO` & `color-pprint-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,78 @@
-Metadata-Version: 2.1
-Name: color-pprint
-Version: 0.0.2
-Summary: A simple package to pretty-print lists dicts, tuples, etc. with color and highlight. (documentation SOON)
-Home-page: https://github.com/mccoderpy/color-pprint
-Author: mccoder.py
-Author-email: mccuber04@outlook.de
-License: MIT
-Project-URL: Source, https://github.com/mccoderpy/color-pprint/
-Project-URL: Support, https://discord.gg/sb69muSqsg
-Project-URL: Issue Tracker, https://github.com/mccoderpy/color-pprint/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Printing
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Typing :: Typed
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# color-pprint
-
-A simple package to pretty-print [lists](https://docs.python.org/3/library/stdtypes.html#list), [dicts](https://docs.python.org/3/library/stdtypes.html#dict), [tuples](https://docs.python.org/3/library/stdtypes.html#tuple), etc. with color and highlight.
-
-Documentation SOON 	&#8482;
-
-### You need help? Or have ideas/feedback?
-___________________________________________
-
-Open an [Issue](https://github.com/mccoderpy/color-pprint/issues)/[Pull request](https://github.com/mccoderpy/color-pprint/pulls) on GitHub, join the [support-server](https://discord.gg/sb69muSqsg) or send me a direct-message on [Discord](https://discord.com/channels/@me): ``mccuber04#2960``
-
-### Installing
-_______________
-
-To install it from [PyPI](https://pypi.org/project/color-pprint) use:
-```sh
-# Linux/macOS
-python3 -m pip install -U color-pprint
-
-# Windows
-py -3 -m pip install -U color-pprint
-```
-
-To install it from [GitHub](https://github.com/mccoderpy/color-pprint) use:
-```sh
-# Linux/macOS
-python3 -m pip install -U git+https://github.com/mccoderpy/color-pprint.git
-
-# Windows
-py -m pip install -U git+https://github.com/mccoderpy/color-pprint.git
-```
-
-______________________________________
-
-**You want to support me by sponsoring my projects? -> [GitHub sponsors](https://github.com/sponsors/mccoderpy)**
+Metadata-Version: 2.1
+Name: color-pprint
+Version: 0.0.3
+Summary: A simple package to pretty-print lists dicts, tuples, etc. with color and highlight. (documentation SOON)
+Home-page: https://github.com/mccoderpy/color-pprint
+Author: mccoder.py
+Author-email: mccuber04@outlook.de
+License: MIT
+Project-URL: Source, https://github.com/mccoderpy/color-pprint/
+Project-URL: Support, https://discord.gg/sb69muSqsg
+Project-URL: Issue Tracker, https://github.com/mccoderpy/color-pprint/issues
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Printing
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# color-pprint
+
+--------------
+
+[![License](https://img.shields.io/github/license/mccoderpy/color-pprint?color=blue&style=for-the-badge&label=License&logo=github&logoColor=white)](./LICENSE)
+[![PyPI latest release version](https://img.shields.io/pypi/v/color-pprint?color=blue&style=for-the-badge&label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/color-pprint)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/color-pprint?style=for-the-badge)](https://pypi.org/project/color-pprint)
+[![PyPI downloads per Month](https://img.shields.io/pypi/dm/color-pprint?style=for-the-badge&logo=download&logoColor=white&color=blue)](https://pepy.tech/project/color-pprint)
+[![GitHub Release Date - Published_At](https://img.shields.io/github/release-date/mccoderpy/color-pprint?style=for-the-badge&label=last%20release)](https://github.com/mccoderpy/color-pprint/releases/latest)
+[![GitHub last commit](https://img.shields.io/github/last-commit/mccoderpy/color-pprint?style=for-the-badge&label=last%20commit&logo=github&logoColor=white)](https://github.com/mccoderpy/color-pprint/commits)
+
+___________________________________________
+
+A simple package to pretty-print [lists](https://docs.python.org/3/library/stdtypes.html#list), [dicts](https://docs.python.org/3/library/stdtypes.html#dict), [tuples](https://docs.python.org/3/library/stdtypes.html#tuple), etc. with color and highlight.
+
+Documentation SOON 	&#8482;
+
+### You need help? Or have ideas/feedback?
+___________________________________________
+
+Open an [Issue](https://github.com/mccoderpy/color-pprint/issues)/[Pull request](https://github.com/mccoderpy/color-pprint/pulls) on GitHub, join the [support-server](https://discord.gg/sb69muSqsg) or send me a direct-message on [Discord](https://discord.com/channels/@me): ``mccuber04``
+
+### Installing
+_______________
+
+To install it from [PyPI](https://pypi.org/project/color-pprint) use:
+```sh
+# Linux/macOS
+python3 -m pip install -U color-pprint
+
+# Windows
+py -3 -m pip install -U color-pprint
+```
+
+To install it from [GitHub](https://github.com/mccoderpy/color-pprint) use:
+```sh
+# Linux/macOS
+python3 -m pip install -U git+https://github.com/mccoderpy/color-pprint.git
+
+# Windows
+py -m pip install -U git+https://github.com/mccoderpy/color-pprint.git
+```
+
+______________________________________
+
+**You want to support me by sponsoring my projects? -> [GitHub sponsors](https://github.com/sponsors/mccoderpy)**
```

### Comparing `color-pprint-0.0.2/README.md` & `color-pprint-0.0.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,46 @@
-# color-pprint
-
-A simple package to pretty-print [lists](https://docs.python.org/3/library/stdtypes.html#list), [dicts](https://docs.python.org/3/library/stdtypes.html#dict), [tuples](https://docs.python.org/3/library/stdtypes.html#tuple), etc. with color and highlight.
-
-Documentation SOON 	&#8482;
-
-### You need help? Or have ideas/feedback?
-___________________________________________
-
-Open an [Issue](https://github.com/mccoderpy/color-pprint/issues)/[Pull request](https://github.com/mccoderpy/color-pprint/pulls) on GitHub, join the [support-server](https://discord.gg/sb69muSqsg) or send me a direct-message on [Discord](https://discord.com/channels/@me): ``mccuber04#2960``
-
-### Installing
-_______________
-
-To install it from [PyPI](https://pypi.org/project/color-pprint) use:
-```sh
-# Linux/macOS
-python3 -m pip install -U color-pprint
-
-# Windows
-py -3 -m pip install -U color-pprint
-```
-
-To install it from [GitHub](https://github.com/mccoderpy/color-pprint) use:
-```sh
-# Linux/macOS
-python3 -m pip install -U git+https://github.com/mccoderpy/color-pprint.git
-
-# Windows
-py -m pip install -U git+https://github.com/mccoderpy/color-pprint.git
-```
-
-______________________________________
-
+# color-pprint
+
+--------------
+
+[![License](https://img.shields.io/github/license/mccoderpy/color-pprint?color=blue&style=for-the-badge&label=License&logo=github&logoColor=white)](./LICENSE)
+[![PyPI latest release version](https://img.shields.io/pypi/v/color-pprint?color=blue&style=for-the-badge&label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/color-pprint)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/color-pprint?style=for-the-badge)](https://pypi.org/project/color-pprint)
+[![PyPI downloads per Month](https://img.shields.io/pypi/dm/color-pprint?style=for-the-badge&logo=download&logoColor=white&color=blue)](https://pepy.tech/project/color-pprint)
+[![GitHub Release Date - Published_At](https://img.shields.io/github/release-date/mccoderpy/color-pprint?style=for-the-badge&label=last%20release)](https://github.com/mccoderpy/color-pprint/releases/latest)
+[![GitHub last commit](https://img.shields.io/github/last-commit/mccoderpy/color-pprint?style=for-the-badge&label=last%20commit&logo=github&logoColor=white)](https://github.com/mccoderpy/color-pprint/commits)
+
+___________________________________________
+
+A simple package to pretty-print [lists](https://docs.python.org/3/library/stdtypes.html#list), [dicts](https://docs.python.org/3/library/stdtypes.html#dict), [tuples](https://docs.python.org/3/library/stdtypes.html#tuple), etc. with color and highlight.
+
+Documentation SOON 	&#8482;
+
+### You need help? Or have ideas/feedback?
+___________________________________________
+
+Open an [Issue](https://github.com/mccoderpy/color-pprint/issues)/[Pull request](https://github.com/mccoderpy/color-pprint/pulls) on GitHub, join the [support-server](https://discord.gg/sb69muSqsg) or send me a direct-message on [Discord](https://discord.com/channels/@me): ``mccuber04``
+
+### Installing
+_______________
+
+To install it from [PyPI](https://pypi.org/project/color-pprint) use:
+```sh
+# Linux/macOS
+python3 -m pip install -U color-pprint
+
+# Windows
+py -3 -m pip install -U color-pprint
+```
+
+To install it from [GitHub](https://github.com/mccoderpy/color-pprint) use:
+```sh
+# Linux/macOS
+python3 -m pip install -U git+https://github.com/mccoderpy/color-pprint.git
+
+# Windows
+py -m pip install -U git+https://github.com/mccoderpy/color-pprint.git
+```
+
+______________________________________
+
 **You want to support me by sponsoring my projects? -> [GitHub sponsors](https://github.com/sponsors/mccoderpy)**
```

### Comparing `color-pprint-0.0.2/color_pprint/__init__.py` & `color-pprint-0.0.3/color_pprint/__init__.py`

 * *Files identical despite different names*

### Comparing `color-pprint-0.0.2/color_pprint/__main__.py` & `color-pprint-0.0.3/color_pprint/__main__.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-# -*- coding: utf-8 -*-
-
-"""
-A simple package to pretty-print lists dicts, tuples, etc. with color and highlight
-
-The MIT License (MIT)
-
-Copyright (c) 2021-present mccoderpy
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-from __future__ import annotations
-
-import sys
-import json
-from . import *
-from os import PathLike
-
-
-def exit_with_help():
-    sys.exit(
-        "Usage:\n\n"
-        "<python> -m color_pprint [--ansi/-a] [--discord/-d] [--file/-f <FILE_TO_WRITE_TO>] <[value/PATH_TO_READ_FROM,]>\n\n"
-        "Example: \"py -m color_pprint --file ./test.json --discord '{\"hello\": \"world\", \"something\": 1234}'\""
-    )
-
-
-def open_file(path: PathLike):
-    return open(path, "a+", encoding='utf-8')
-
-
-if __name__ == '__main__':
-    args: list[str | PathLike] = sys.argv[1:]
-    if not args or '--help' in args:
-        print('A simple package to pretty-print lists dicts, tuples, etc. with color and highlight - (c) 2022-present mccoderpy')
-        exit_with_help()
-
-    values = []
-    mode = 'default'
-    file = sys.stdout
-    kwargs = {}
-
-    for i, option in enumerate(args):
-        if option.startswith('-'):
-            o = option.strip('-').lower()
-            if o in ('a', 'ansi'):
-                mode = 'ansi'
-            elif o in ('f', 'file'):
-                try:
-                    file_name = args.pop(i+1)
-                except IndexError:
-                    print('Missing file name after --file parameter')
-                    exit_with_help()
-                else:
-                    try:
-                        file = open_file(file_name)
-                    except OSError as exc:
-                        print(f'Failed to open file "{file_name}" due to {exc.__class__.__name__}:\n')
-                        raise exc from None
-            elif o in ('d', 'discord'):
-                kwargs.update(
-                    key_color="\u001B[31m",
-                    str_color="\u001B[33m"
-                )
-            else:
-                print(f'Invalid option "{option}"')
-                exit_with_help()
-        else:
-            values.append(option)
-
-    if not len(values):
-        exit_with_help()
-
-    if mode == 'ansi':
-        for index, input_or_path in enumerate(values):
-            try:
-                with open(input_or_path) as fp:
-                    value = json.load(fp)
-            except FileNotFoundError as exc:
-                print(f'Failed to parse input value at position {index} due to FileNotFoundError:\n')
-                raise exc from None
-            except OSError as origin_exc:
-                if origin_exc.strerror.startswith('Invalid argument'):  # expect it is not a valid path here
-                    try:
-                        value = json.loads(input_or_path)
-                    except json.JSONDecodeError as exc:
-                        print(f'Failed to parse input value at position {index} due to JSONDecodeError:\n')
-                        raise exc from None
-                else:  # Some other error occurred - re-raise
-                    print(f'Failed to parse input value at position {index} due to {origin_exc.__class__.__name__}:\n')
-                    raise origin_exc from None
-
-            print(color_dict(value, **kwargs), file=file)
-    else:
-        for index, input_or_path in enumerate(values):
-            try:
-                with open(input_or_path) as fp:
-                    value = json.load(fp)
-            except FileNotFoundError as exc:
-                print(f'Failed to parse input value at position {index} due to FileNotFoundError:\n')
-                raise exc from None
-            except OSError as origin_exc:
-                if origin_exc.strerror.startswith('Invalid argument'):  # expect it is not a valid path here
-                    try:
-                        value = json.loads(input_or_path)
-                    except json.JSONDecodeError as exc:
-                        print(f'Failed to parse input value at position {index} due to JSONDecodeError:\n')
-                        raise exc from None
-                else:  # Some other error occurred - re-raise
-                    print(f'Failed to parse input value at position {index} due to {origin_exc.__class__.__name__}:\n')
-                    raise origin_exc from None
-
-            cprint(value, file=file, ensure_ascii=False, **kwargs)
+# -*- coding: utf-8 -*-
+
+"""
+A simple package to pretty-print lists dicts, tuples, etc. with color and highlight
+
+The MIT License (MIT)
+
+Copyright (c) 2021-present mccoderpy
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+
+import sys
+import json
+from . import *
+from os import PathLike
+
+
+def exit_with_help():
+    sys.exit(
+        "Usage:\n\n"
+        "<python> -m color_pprint [--ansi/-a] [--discord/-d] [--file/-f <FILE_TO_WRITE_TO>] <[value/PATH_TO_READ_FROM,]>\n\n"
+        "Example: \"py -m color_pprint --file ./test.json --discord '{\"hello\": \"world\", \"something\": 1234}'\""
+    )
+
+
+def open_file(path: PathLike):
+    return open(path, "a+", encoding='utf-8')
+
+
+if __name__ == '__main__':
+    args: list[str | PathLike] = sys.argv[1:]
+    if not args or '--help' in args:
+        print('A simple package to pretty-print lists dicts, tuples, etc. with color and highlight - (c) 2022-present mccoderpy')
+        exit_with_help()
+
+    values = []
+    mode = 'default'
+    file = sys.stdout
+    kwargs = {}
+
+    for i, option in enumerate(args):
+        if option.startswith('-'):
+            o = option.strip('-').lower()
+            if o in ('a', 'ansi'):
+                mode = 'ansi'
+            elif o in ('f', 'file'):
+                try:
+                    file_name = args.pop(i+1)
+                except IndexError:
+                    print('Missing file name after --file parameter')
+                    exit_with_help()
+                else:
+                    try:
+                        file = open_file(file_name)
+                    except OSError as exc:
+                        print(f'Failed to open file "{file_name}" due to {exc.__class__.__name__}:\n')
+                        raise exc from None
+            elif o in ('d', 'discord'):
+                kwargs.update(
+                    key_color="\u001B[31m",
+                    str_color="\u001B[33m"
+                )
+            else:
+                print(f'Invalid option "{option}"')
+                exit_with_help()
+        else:
+            values.append(option)
+
+    if not len(values):
+        exit_with_help()
+
+    if mode == 'ansi':
+        for index, input_or_path in enumerate(values):
+            try:
+                with open(input_or_path) as fp:
+                    value = json.load(fp)
+            except FileNotFoundError as exc:
+                print(f'Failed to parse input value at position {index} due to FileNotFoundError:\n')
+                raise exc from None
+            except OSError as origin_exc:
+                if origin_exc.strerror.startswith('Invalid argument'):  # expect it is not a valid path here
+                    try:
+                        value = json.loads(input_or_path)
+                    except json.JSONDecodeError as exc:
+                        print(f'Failed to parse input value at position {index} due to JSONDecodeError:\n')
+                        raise exc from None
+                else:  # Some other error occurred - re-raise
+                    print(f'Failed to parse input value at position {index} due to {origin_exc.__class__.__name__}:\n')
+                    raise origin_exc from None
+
+            print(color_dict(value, **kwargs), file=file)
+    else:
+        for index, input_or_path in enumerate(values):
+            try:
+                with open(input_or_path) as fp:
+                    value = json.load(fp)
+            except FileNotFoundError as exc:
+                print(f'Failed to parse input value at position {index} due to FileNotFoundError:\n')
+                raise exc from None
+            except OSError as origin_exc:
+                if origin_exc.strerror.startswith('Invalid argument'):  # expect it is not a valid path here
+                    try:
+                        value = json.loads(input_or_path)
+                    except json.JSONDecodeError as exc:
+                        print(f'Failed to parse input value at position {index} due to JSONDecodeError:\n')
+                        raise exc from None
+                else:  # Some other error occurred - re-raise
+                    print(f'Failed to parse input value at position {index} due to {origin_exc.__class__.__name__}:\n')
+                    raise origin_exc from None
+
+            cprint(value, file=file, ensure_ascii=False, **kwargs)
```

### Comparing `color-pprint-0.0.2/color_pprint.egg-info/PKG-INFO` & `color-pprint-0.0.3/color_pprint.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,78 @@
-Metadata-Version: 2.1
-Name: color-pprint
-Version: 0.0.2
-Summary: A simple package to pretty-print lists dicts, tuples, etc. with color and highlight. (documentation SOON)
-Home-page: https://github.com/mccoderpy/color-pprint
-Author: mccoder.py
-Author-email: mccuber04@outlook.de
-License: MIT
-Project-URL: Source, https://github.com/mccoderpy/color-pprint/
-Project-URL: Support, https://discord.gg/sb69muSqsg
-Project-URL: Issue Tracker, https://github.com/mccoderpy/color-pprint/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Printing
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Typing :: Typed
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# color-pprint
-
-A simple package to pretty-print [lists](https://docs.python.org/3/library/stdtypes.html#list), [dicts](https://docs.python.org/3/library/stdtypes.html#dict), [tuples](https://docs.python.org/3/library/stdtypes.html#tuple), etc. with color and highlight.
-
-Documentation SOON 	&#8482;
-
-### You need help? Or have ideas/feedback?
-___________________________________________
-
-Open an [Issue](https://github.com/mccoderpy/color-pprint/issues)/[Pull request](https://github.com/mccoderpy/color-pprint/pulls) on GitHub, join the [support-server](https://discord.gg/sb69muSqsg) or send me a direct-message on [Discord](https://discord.com/channels/@me): ``mccuber04#2960``
-
-### Installing
-_______________
-
-To install it from [PyPI](https://pypi.org/project/color-pprint) use:
-```sh
-# Linux/macOS
-python3 -m pip install -U color-pprint
-
-# Windows
-py -3 -m pip install -U color-pprint
-```
-
-To install it from [GitHub](https://github.com/mccoderpy/color-pprint) use:
-```sh
-# Linux/macOS
-python3 -m pip install -U git+https://github.com/mccoderpy/color-pprint.git
-
-# Windows
-py -m pip install -U git+https://github.com/mccoderpy/color-pprint.git
-```
-
-______________________________________
-
-**You want to support me by sponsoring my projects? -> [GitHub sponsors](https://github.com/sponsors/mccoderpy)**
+Metadata-Version: 2.1
+Name: color-pprint
+Version: 0.0.3
+Summary: A simple package to pretty-print lists dicts, tuples, etc. with color and highlight. (documentation SOON)
+Home-page: https://github.com/mccoderpy/color-pprint
+Author: mccoder.py
+Author-email: mccuber04@outlook.de
+License: MIT
+Project-URL: Source, https://github.com/mccoderpy/color-pprint/
+Project-URL: Support, https://discord.gg/sb69muSqsg
+Project-URL: Issue Tracker, https://github.com/mccoderpy/color-pprint/issues
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Printing
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# color-pprint
+
+--------------
+
+[![License](https://img.shields.io/github/license/mccoderpy/color-pprint?color=blue&style=for-the-badge&label=License&logo=github&logoColor=white)](./LICENSE)
+[![PyPI latest release version](https://img.shields.io/pypi/v/color-pprint?color=blue&style=for-the-badge&label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/color-pprint)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/color-pprint?style=for-the-badge)](https://pypi.org/project/color-pprint)
+[![PyPI downloads per Month](https://img.shields.io/pypi/dm/color-pprint?style=for-the-badge&logo=download&logoColor=white&color=blue)](https://pepy.tech/project/color-pprint)
+[![GitHub Release Date - Published_At](https://img.shields.io/github/release-date/mccoderpy/color-pprint?style=for-the-badge&label=last%20release)](https://github.com/mccoderpy/color-pprint/releases/latest)
+[![GitHub last commit](https://img.shields.io/github/last-commit/mccoderpy/color-pprint?style=for-the-badge&label=last%20commit&logo=github&logoColor=white)](https://github.com/mccoderpy/color-pprint/commits)
+
+___________________________________________
+
+A simple package to pretty-print [lists](https://docs.python.org/3/library/stdtypes.html#list), [dicts](https://docs.python.org/3/library/stdtypes.html#dict), [tuples](https://docs.python.org/3/library/stdtypes.html#tuple), etc. with color and highlight.
+
+Documentation SOON 	&#8482;
+
+### You need help? Or have ideas/feedback?
+___________________________________________
+
+Open an [Issue](https://github.com/mccoderpy/color-pprint/issues)/[Pull request](https://github.com/mccoderpy/color-pprint/pulls) on GitHub, join the [support-server](https://discord.gg/sb69muSqsg) or send me a direct-message on [Discord](https://discord.com/channels/@me): ``mccuber04``
+
+### Installing
+_______________
+
+To install it from [PyPI](https://pypi.org/project/color-pprint) use:
+```sh
+# Linux/macOS
+python3 -m pip install -U color-pprint
+
+# Windows
+py -3 -m pip install -U color-pprint
+```
+
+To install it from [GitHub](https://github.com/mccoderpy/color-pprint) use:
+```sh
+# Linux/macOS
+python3 -m pip install -U git+https://github.com/mccoderpy/color-pprint.git
+
+# Windows
+py -m pip install -U git+https://github.com/mccoderpy/color-pprint.git
+```
+
+______________________________________
+
+**You want to support me by sponsoring my projects? -> [GitHub sponsors](https://github.com/sponsors/mccoderpy)**
```

### Comparing `color-pprint-0.0.2/setup.py` & `color-pprint-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,48 @@
-from setuptools import setup
-
-with open('README.md') as fp:
-    long_description = fp.read()
-
-setup(
-    name='color-pprint',
-    version='0.0.2',
-    url='https://github.com/mccoderpy/color-pprint',
-    project_urls={
-        'Source': 'https://github.com/mccoderpy/color-pprint/',
-        'Support': 'https://discord.gg/sb69muSqsg',
-        'Issue Tracker': 'https://github.com/mccoderpy/color-pprint/issues'
-    },
-    license='MIT',
-    description='A simple package to pretty-print lists dicts, tuples, etc. with color and highlight. (documentation SOON)',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author='mccoder.py',
-    author_email='mccuber04@outlook.de',
-    include_package_data=True,
-    packages=['color_pprint', 'color_pprint.ansi'],
-    classifiers=[
-        'Development Status :: 4 - Beta',
-        'License :: OSI Approved :: MIT License',
-        'Intended Audience :: Developers',
-        'Natural Language :: English',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Topic :: Printing',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Topic :: Utilities',
-        'Typing :: Typed'
-    ],
-    install_requires=[
-        'colorama>=0.3.7',
-        'multidict>=5.1.0'
-    ]
-)
+from setuptools import setup
+
+with open('README.md') as fp:
+    long_description = fp.read()
+
+setup(
+    name='color-pprint',
+    version='0.0.3',
+    url='https://github.com/mccoderpy/color-pprint',
+    project_urls={
+        'Source': 'https://github.com/mccoderpy/color-pprint/',
+        'Support': 'https://discord.gg/sb69muSqsg',
+        'Issue Tracker': 'https://github.com/mccoderpy/color-pprint/issues'
+    },
+    license='MIT',
+    description='A simple package to pretty-print lists dicts, tuples, etc. with color and highlight. (documentation SOON)',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    author='mccoder.py',
+    author_email='mccuber04@outlook.de',
+    include_package_data=True,
+    packages=['color_pprint', 'color_pprint.ansi'],
+    classifiers=[
+        'Development Status :: 4 - Beta',
+        'License :: OSI Approved :: MIT License',
+        'Intended Audience :: Developers',
+        'Natural Language :: English',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'Topic :: Printing',
+        'Topic :: Software Development :: Libraries',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Topic :: Utilities',
+        'Typing :: Typed'
+    ],
+    install_requires=[
+        'colorama>=0.3.7',
+        'multidict>=5.1.0',
+        'regex>=0.1.20120103'
+    ]
+)
```

