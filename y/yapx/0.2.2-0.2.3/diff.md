# Comparing `tmp/yapx-0.2.2.tar.gz` & `tmp/yapx-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yapx-0.2.2.tar", last modified: Fri Jul 28 04:52:45 2023, max compression
+gzip compressed data, was "yapx-0.2.3.tar", last modified: Sat Jul 29 00:02:49 2023, max compression
```

## Comparing `yapx-0.2.2.tar` & `yapx-0.2.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:52:45.706005 yapx-0.2.2/
--rw-r--r--   0 root         (0) root         (0)     1058 2023-07-28 04:48:20.000000 yapx-0.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4162 2023-07-28 04:52:45.706005 yapx-0.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2419 2023-07-28 04:48:20.000000 yapx-0.2.2/README.md
--rw-r--r--   0 root         (0) root         (0)     4885 2023-07-28 04:48:20.000000 yapx-0.2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 04:52:45.706005 yapx-0.2.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:52:45.694005 yapx-0.2.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:52:45.698005 yapx-0.2.2/src/yapx/
--rw-r--r--   0 root         (0) root         (0)     5155 2023-07-28 04:48:20.000000 yapx-0.2.2/src/yapx/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:52:45.702005 yapx-0.2.2/src/yapx/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     4901 2023-07-28 04:49:00.000000 yapx-0.2.2/src/yapx/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      148 2023-07-28 04:52:24.000000 yapx-0.2.2/src/yapx/__pycache__/__version__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     7098 2023-07-28 04:49:01.000000 yapx-0.2.2/src/yapx/__pycache__/actions.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     7626 2023-07-28 04:49:00.000000 yapx-0.2.2/src/yapx/__pycache__/arg.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)    27963 2023-07-28 04:49:00.000000 yapx-0.2.2/src/yapx/__pycache__/argument_parser.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      921 2023-07-28 04:49:00.000000 yapx-0.2.2/src/yapx/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      784 2023-07-28 04:49:01.000000 yapx-0.2.2/src/yapx/__pycache__/namespace.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     1550 2023-07-28 04:49:00.000000 yapx-0.2.2/src/yapx/__pycache__/types.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     4278 2023-07-28 04:49:01.000000 yapx-0.2.2/src/yapx/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 04:52:24.000000 yapx-0.2.2/src/yapx/__version__.py
--rw-r--r--   0 root         (0) root         (0)     9750 2023-07-28 04:48:20.000000 yapx-0.2.2/src/yapx/actions.py
--rw-r--r--   0 root         (0) root         (0)     9642 2023-07-28 04:48:20.000000 yapx-0.2.2/src/yapx/arg.py
--rw-r--r--   0 root         (0) root         (0)    44793 2023-07-28 04:48:20.000000 yapx-0.2.2/src/yapx/argument_parser.py
--rw-r--r--   0 root         (0) root         (0)      633 2023-07-28 04:48:20.000000 yapx-0.2.2/src/yapx/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-07-28 04:48:20.000000 yapx-0.2.2/src/yapx/namespace.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 04:48:20.000000 yapx-0.2.2/src/yapx/py.typed
--rw-r--r--   0 root         (0) root         (0)     1300 2023-07-28 04:48:20.000000 yapx-0.2.2/src/yapx/types.py
--rw-r--r--   0 root         (0) root         (0)     4211 2023-07-28 04:48:20.000000 yapx-0.2.2/src/yapx/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:52:45.702005 yapx-0.2.2/src/yapx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4162 2023-07-28 04:52:45.000000 yapx-0.2.2/src/yapx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      981 2023-07-28 04:52:45.000000 yapx-0.2.2/src/yapx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 04:52:45.000000 yapx-0.2.2/src/yapx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      770 2023-07-28 04:52:45.000000 yapx-0.2.2/src/yapx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-28 04:52:45.000000 yapx-0.2.2/src/yapx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:52:45.706005 yapx-0.2.2/tests/
--rw-r--r--   0 root         (0) root         (0)     5205 2023-07-28 04:48:20.000000 yapx-0.2.2/tests/test_actions.py
--rw-r--r--   0 root         (0) root         (0)    11974 2023-07-28 04:48:20.000000 yapx-0.2.2/tests/test_add_arguments.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-07-28 04:48:20.000000 yapx-0.2.2/tests/test_add_arguments_future.py
--rw-r--r--   0 root         (0) root         (0)     1260 2023-07-28 04:48:20.000000 yapx-0.2.2/tests/test_add_command.py
--rw-r--r--   0 root         (0) root         (0)     8186 2023-07-28 04:48:20.000000 yapx-0.2.2/tests/test_arg.py
--rw-r--r--   0 root         (0) root         (0)    25200 2023-07-28 04:48:20.000000 yapx-0.2.2/tests/test_run.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-07-28 04:48:20.000000 yapx-0.2.2/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 00:02:49.445670 yapx-0.2.3/
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-07-28 23:58:26.000000 yapx-0.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5528 2023-07-29 00:02:49.445670 yapx-0.2.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3785 2023-07-28 23:58:26.000000 yapx-0.2.3/README.md
+-rw-r--r--   0 root         (0) root         (0)     4885 2023-07-28 23:58:26.000000 yapx-0.2.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 00:02:49.445670 yapx-0.2.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 00:02:49.433670 yapx-0.2.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 00:02:49.437670 yapx-0.2.3/src/yapx/
+-rw-r--r--   0 root         (0) root         (0)     5155 2023-07-28 23:58:26.000000 yapx-0.2.3/src/yapx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 00:02:49.441670 yapx-0.2.3/src/yapx/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     4901 2023-07-28 23:59:06.000000 yapx-0.2.3/src/yapx/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-29 00:02:28.000000 yapx-0.2.3/src/yapx/__pycache__/__version__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     7098 2023-07-28 23:59:06.000000 yapx-0.2.3/src/yapx/__pycache__/actions.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     7626 2023-07-28 23:59:06.000000 yapx-0.2.3/src/yapx/__pycache__/arg.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)    28026 2023-07-28 23:59:06.000000 yapx-0.2.3/src/yapx/__pycache__/argument_parser.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      921 2023-07-28 23:59:06.000000 yapx-0.2.3/src/yapx/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      784 2023-07-28 23:59:07.000000 yapx-0.2.3/src/yapx/__pycache__/namespace.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-07-28 23:59:06.000000 yapx-0.2.3/src/yapx/__pycache__/types.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     4278 2023-07-28 23:59:06.000000 yapx-0.2.3/src/yapx/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-29 00:02:28.000000 yapx-0.2.3/src/yapx/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     9750 2023-07-28 23:58:26.000000 yapx-0.2.3/src/yapx/actions.py
+-rw-r--r--   0 root         (0) root         (0)     9642 2023-07-28 23:58:26.000000 yapx-0.2.3/src/yapx/arg.py
+-rw-r--r--   0 root         (0) root         (0)    45077 2023-07-28 23:58:26.000000 yapx-0.2.3/src/yapx/argument_parser.py
+-rw-r--r--   0 root         (0) root         (0)      633 2023-07-28 23:58:26.000000 yapx-0.2.3/src/yapx/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-28 23:58:26.000000 yapx-0.2.3/src/yapx/namespace.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 23:58:26.000000 yapx-0.2.3/src/yapx/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-07-28 23:58:26.000000 yapx-0.2.3/src/yapx/types.py
+-rw-r--r--   0 root         (0) root         (0)     4211 2023-07-28 23:58:26.000000 yapx-0.2.3/src/yapx/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 00:02:49.441670 yapx-0.2.3/src/yapx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5528 2023-07-29 00:02:49.000000 yapx-0.2.3/src/yapx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      981 2023-07-29 00:02:49.000000 yapx-0.2.3/src/yapx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 00:02:49.000000 yapx-0.2.3/src/yapx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      770 2023-07-29 00:02:49.000000 yapx-0.2.3/src/yapx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-29 00:02:49.000000 yapx-0.2.3/src/yapx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 00:02:49.445670 yapx-0.2.3/tests/
+-rw-r--r--   0 root         (0) root         (0)     5205 2023-07-28 23:58:26.000000 yapx-0.2.3/tests/test_actions.py
+-rw-r--r--   0 root         (0) root         (0)    11974 2023-07-28 23:58:26.000000 yapx-0.2.3/tests/test_add_arguments.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-07-28 23:58:26.000000 yapx-0.2.3/tests/test_add_arguments_future.py
+-rw-r--r--   0 root         (0) root         (0)     1260 2023-07-28 23:58:26.000000 yapx-0.2.3/tests/test_add_command.py
+-rw-r--r--   0 root         (0) root         (0)     8186 2023-07-28 23:58:26.000000 yapx-0.2.3/tests/test_arg.py
+-rw-r--r--   0 root         (0) root         (0)    25223 2023-07-28 23:58:26.000000 yapx-0.2.3/tests/test_run.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-07-28 23:58:26.000000 yapx-0.2.3/tests/test_utils.py
```

### Comparing `yapx-0.2.2/LICENSE` & `yapx-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yapx-0.2.2/PKG-INFO` & `yapx-0.2.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: yapx
-Version: 0.2.2
-Summary: The next generation of Python's Argparse.
-Author-email: Donald Mellenbruch <hello@f2dv.com>
-License: Copyright 2023 Donald Mellenbruch
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-Project-URL: Homepage, https://www.f2dv.com/r/yapx
-Project-URL: Repository, https://www.github.com/fresh2dev/yapx
-Project-URL: Funding, https://www.f2dv.com/fund
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-Provides-Extra: tests
-Provides-Extra: pydantic
-Provides-Extra: shtab
-Provides-Extra: rich
-Provides-Extra: tui
-Provides-Extra: extras
-License-File: LICENSE
-
 # yapx
 
 > The next generation of Python's Argparse.
 
 | Links         |                                       |
 |---------------|---------------------------------------|
 | Code Repo     | https://www.github.com/fresh2dev/yapx |
@@ -47,28 +18,57 @@
 [![GitHub issues](https://img.shields.io/github/issues-raw/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/yapx/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr-raw/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/yapx/pulls)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/yapx?color=blue&style=for-the-badge)](https://pypi.org/project/yapx)
 [![Docker Pulls](https://img.shields.io/docker/pulls/fresh2dev/yapx?color=blue&style=for-the-badge)](https://hub.docker.com/r/fresh2dev/yapx)
 [![Changelog](https://img.shields.io/website?down_message=unavailable&label=docs&style=for-the-badge&up_color=blue&up_message=available&url=https://www.f2dv.com/r/yapx/changelog)](https://www.f2dv.com/r/yapx/changelog)
 [![Funding](https://img.shields.io/badge/funding-%24%24%24-blue?style=for-the-badge)](https://www.f2dv.com/fund)
 
----
-
 ## Overview
 
-...
+Yapx is "yeah, another argparse extension" for building Python CLIs with the utmost simplicity.
+
+It works by reading type hints of Python functions and dataclasses, and uses them to construct an argparse `ArgumentParser`.
+
+Yapx features:
+
+- Support for subcommands
+- Support for lists in various forms: (positional) `1 2 3`, (multiple) `-x 1 -x 2 -x 3`, (multi-value) `-x 1 2 3`, (comma-separated), `-x 1, 2, 3`, (string) `-x '[1, 2, 3]'`
+- Support for dictionaries / key-value mappings such as `--values one=1 two=2 three=3`
+- Support for optional booleans: `--flag` / `--no-flag`
+- Support for feature flags: `--dev` / `--test` / `--prod`
+- Support for counting parameters: `-vvv`
+- Automatic "helpful" arguments: `--help`, `--help-all`, `--version`, etc.
+- Support for setting values from environment variables
 
 ## Install
 
-...
+Yapx has no 3rd-party dependencies out-of-the-box:
+
+```sh
+pip install yapx
+```
+
+Extras are available to unlock additional functionality:
+
+- `yapx[pydantic]`: enables support for additional types
+- `yapx[shtab]`: enables shell-completion
+- `yapx[rich]`: enables prettier help and error messages
+- `yapx[tui]`: enables experimental TUI support
+- `yapx[extras]`: enables each of the above
 
 ## Use
 
-...
+See notebooks of examples here:
+
+https://www.f2dv.com/r/yapx/page/overview
+
+Read more about yapx @ https://www.f2dv.com/r/yapx
 
 ## Support
 
 If this project delivers value to you, please [provide feedback](https://www.github.com/fresh2dev/yapx/issues), code contributions, and/or [funding](https://www.f2dv.com/fund).
 
+See all of my projects @ https://www.f2dv.com/projects
+
 *Brought to you by...*
 
 <a href="https://www.f2dv.com"><img src="https://img.fresh2.dev/fresh2dev.svg" style="filter: invert(50%);"></img></a>
```

#### html2text {}

```diff
@@ -1,54 +1,48 @@
-Metadata-Version: 2.1 Name: yapx Version: 0.2.2 Summary: The next generation of
-Python's Argparse. Author-email: Donald Mellenbruch
-f2dv.com> License: Copyright 2023 Donald Mellenbruch Permission is hereby
-granted, free of charge, to any person obtaining a copy of this software and
-associated documentation files (the "Software"), to deal in the Software
-without restriction, including without limitation the rights to use, copy,
-modify, merge, publish, distribute, sublicense, and/or sell copies of the
-Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions: The above copyright notice and this
-permission notice shall be included in all copies or substantial portions of
-the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
-EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
-OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://www.f2dv.com/r/yapx
-Project-URL: Repository, https://www.github.com/fresh2dev/yapx Project-URL:
-Funding, https://www.f2dv.com/fund Classifier: Programming Language :: Python
-:: 3 Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-
-Extra: dev Provides-Extra: docs Provides-Extra: tests Provides-Extra: pydantic
-Provides-Extra: shtab Provides-Extra: rich Provides-Extra: tui Provides-Extra:
-extras License-File: LICENSE # yapx > The next generation of Python's Argparse.
-| Links | | |---------------|---------------------------------------| | Code
-Repo | https://www.github.com/fresh2dev/yapx | | Mirror Repo | https://
-www.f2dv.com/r/yapx | | Documentation | https://www.f2dv.com/r/yapx | |
-Changelog | https://www.f2dv.com/r/yapx/changelog | | License | https://
-www.f2dv.com/r/yapx/license | | Funding | https://www.f2dv.com/fund | [![GitHub
-release (latest SemVer)](https://img.shields.io/github/v/release/fresh2dev/
-yapx?color=blue&style=for-the-badge)](https://www.f2dv.com/r/yapx/changelog) [!
-[GitHub Release Date](https://img.shields.io/github/release-date/fresh2dev/
-yapx?color=blue&style=for-the-badge)](https://www.f2dv.com/r/yapx/changelog) [!
-[License](https://img.shields.io/github/license/fresh2dev/
-yapx?color=blue&style=for-the-badge)](https://www.f2dv.com/r/yapx/license) [!
-[GitHub Repo stars](https://img.shields.io/github/stars/fresh2dev/
-yapx?color=blue&style=for-the-badge)](https://star-history.com/#fresh2dev/
-yapx&Date) [![GitHub issues](https://img.shields.io/github/issues-raw/
-fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/
-fresh2dev/yapx/issues) [![GitHub pull requests](https://img.shields.io/github/
-issues-pr-raw/fresh2dev/yapx?color=blue&style=for-the-badge)](https://
-www.github.com/fresh2dev/yapx/pulls) [![PyPI - Downloads](https://
-img.shields.io/pypi/dm/yapx?color=blue&style=for-the-badge)](https://pypi.org/
-project/yapx) [![Docker Pulls](https://img.shields.io/docker/pulls/fresh2dev/
-yapx?color=blue&style=for-the-badge)](https://hub.docker.com/r/fresh2dev/yapx)
-[![Changelog](https://img.shields.io/
-website?down_message=unavailable&label=docs&style=for-the-
+# yapx > The next generation of Python's Argparse. | Links | | |---------------
+|---------------------------------------| | Code Repo | https://www.github.com/
+fresh2dev/yapx | | Mirror Repo | https://www.f2dv.com/r/yapx | | Documentation
+| https://www.f2dv.com/r/yapx | | Changelog | https://www.f2dv.com/r/yapx/
+changelog | | License | https://www.f2dv.com/r/yapx/license | | Funding |
+https://www.f2dv.com/fund | [![GitHub release (latest SemVer)](https://
+img.shields.io/github/v/release/fresh2dev/yapx?color=blue&style=for-the-badge)]
+(https://www.f2dv.com/r/yapx/changelog) [![GitHub Release Date](https://
+img.shields.io/github/release-date/fresh2dev/yapx?color=blue&style=for-the-
+badge)](https://www.f2dv.com/r/yapx/changelog) [![License](https://
+img.shields.io/github/license/fresh2dev/yapx?color=blue&style=for-the-badge)]
+(https://www.f2dv.com/r/yapx/license) [![GitHub Repo stars](https://
+img.shields.io/github/stars/fresh2dev/yapx?color=blue&style=for-the-badge)]
+(https://star-history.com/#fresh2dev/yapx&Date) [![GitHub issues](https://
+img.shields.io/github/issues-raw/fresh2dev/yapx?color=blue&style=for-the-
+badge)](https://www.github.com/fresh2dev/yapx/issues) [![GitHub pull requests]
+(https://img.shields.io/github/issues-pr-raw/fresh2dev/
+yapx?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/yapx/
+pulls) [![PyPI - Downloads](https://img.shields.io/pypi/dm/
+yapx?color=blue&style=for-the-badge)](https://pypi.org/project/yapx) [![Docker
+Pulls](https://img.shields.io/docker/pulls/fresh2dev/yapx?color=blue&style=for-
+the-badge)](https://hub.docker.com/r/fresh2dev/yapx) [![Changelog](https://
+img.shields.io/website?down_message=unavailable&label=docs&style=for-the-
 badge&up_color=blue&up_message=available&url=https://www.f2dv.com/r/yapx/
 changelog)](https://www.f2dv.com/r/yapx/changelog) [![Funding](https://
 img.shields.io/badge/funding-%24%24%24-blue?style=for-the-badge)](https://
-www.f2dv.com/fund) --- ## Overview ... ## Install ... ## Use ... ## Support If
-this project delivers value to you, please [provide feedback](https://
-www.github.com/fresh2dev/yapx/issues), code contributions, and/or [funding]
-(https://www.f2dv.com/fund). *Brought to you by...* [https://img.fresh2.dev/
-fresh2dev.svg]
+www.f2dv.com/fund) ## Overview Yapx is "yeah, another argparse extension" for
+building Python CLIs with the utmost simplicity. It works by reading type hints
+of Python functions and dataclasses, and uses them to construct an argparse
+`ArgumentParser`. Yapx features: - Support for subcommands - Support for lists
+in various forms: (positional) `1 2 3`, (multiple) `-x 1 -x 2 -x 3`, (multi-
+value) `-x 1 2 3`, (comma-separated), `-x 1, 2, 3`, (string) `-x '[1, 2, 3]'` -
+Support for dictionaries / key-value mappings such as `--values one=1 two=2
+three=3` - Support for optional booleans: `--flag` / `--no-flag` - Support for
+feature flags: `--dev` / `--test` / `--prod` - Support for counting parameters:
+`-vvv` - Automatic "helpful" arguments: `--help`, `--help-all`, `--version`,
+etc. - Support for setting values from environment variables ## Install Yapx
+has no 3rd-party dependencies out-of-the-box: ```sh pip install yapx ``` Extras
+are available to unlock additional functionality: - `yapx[pydantic]`: enables
+support for additional types - `yapx[shtab]`: enables shell-completion - `yapx
+[rich]`: enables prettier help and error messages - `yapx[tui]`: enables
+experimental TUI support - `yapx[extras]`: enables each of the above ## Use See
+notebooks of examples here: https://www.f2dv.com/r/yapx/page/overview Read more
+about yapx @ https://www.f2dv.com/r/yapx ## Support If this project delivers
+value to you, please [provide feedback](https://www.github.com/fresh2dev/yapx/
+issues), code contributions, and/or [funding](https://www.f2dv.com/fund). See
+all of my projects @ https://www.f2dv.com/projects *Brought to you by...*
+[https://img.fresh2.dev/fresh2dev.svg]
```

### Comparing `yapx-0.2.2/pyproject.toml` & `yapx-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yapx-0.2.2/src/yapx/__init__.py` & `yapx-0.2.3/src/yapx/__init__.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.2/src/yapx/__pycache__/__init__.cpython-310.pyc` & `yapx-0.2.3/src/yapx/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 04:48:20 2023 UTC, .py size: 5155 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9448 c364 2314 0000  o........H.d#...
+00000000: 6f0d 0d0a 0000 0000 2256 c464 2314 0000  o......."V.d#...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000f 0000 0040 0000 0073 1402 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6403 6404 6c09  m.Z.m.Z...d.d.l.
 00000060: 6d0a 5a0a 6d0b 5a0b 0100 6403 6405 6c0c  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6403 6406 6c0d 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `yapx-0.2.2/src/yapx/__pycache__/actions.cpython-310.pyc` & `yapx-0.2.3/src/yapx/__pycache__/actions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 04:48:20 2023 UTC, .py size: 9750 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9448 c364 1626 0000  o........H.d.&..
+00000000: 6f0d 0d0a 0000 0000 2256 c464 1626 0000  o......."V.d.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 7201 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6400 6403 6c03 6d08 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6404 6c0a 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  d.l.m.Z.m.Z.m.Z.
```

### Comparing `yapx-0.2.2/src/yapx/__pycache__/arg.cpython-310.pyc` & `yapx-0.2.3/src/yapx/__pycache__/arg.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 04:48:20 2023 UTC, .py size: 9642 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9448 c364 aa25 0000  o........H.d.%..
+00000000: 6f0d 0d0a 0000 0000 2256 c464 aa25 0000  o......."V.d.%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0019 0000 0040 0000 0073 3c02 0000 5500  .....@...s<...U.
 00000030: 6400 6401 6c00 5a00 6400 6401 6c01 5a01  d.d.l.Z.d.d.l.Z.
 00000040: 6400 6402 6c02 6d03 5a03 0100 6400 6403  d.d.l.m.Z...d.d.
 00000050: 6c04 6d05 5a05 0100 6400 6404 6c06 6d07  l.m.Z...d.d.l.m.
 00000060: 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b  Z.m.Z.m.Z.m.Z.m.
 00000070: 5a0b 0100 6400 6405 6c0c 6d0d 5a0d 6d0e  Z...d.d.l.m.Z.m.
```

### Comparing `yapx-0.2.2/src/yapx/__pycache__/argument_parser.cpython-310.pyc` & `yapx-0.2.3/src/yapx/__pycache__/argument_parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 04:48:20 2023 UTC, .py size: 44793 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9448 c364 f9ae 0000  o........H.d....
+00000000: 6f0d 0d0a 0000 0000 2256 c464 15b0 0000  o......."V.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 c401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6402 6c02 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6400 6405 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
@@ -692,23 +692,23 @@
 00002b30: 0000 0072 5700 0000 da17 5f69 735f 6174  ...rW....._is_at
 00002b40: 7472 6962 7574 655f 696e 6865 7269 7465  tribute_inherite
 00002b50: 6495 0100 0073 0200 0000 0a02 7a26 4172  d....s......z&Ar
 00002b60: 6775 6d65 6e74 5061 7273 6572 2e5f 6973  gumentParser._is
 00002b70: 5f61 7474 7269 6275 7465 5f69 6e68 6572  _attribute_inher
 00002b80: 6974 6564 7266 0000 0063 0300 0000 0000  itedrf...c......
 00002b90: 0000 0000 0000 1900 0000 0900 0000 0300  ................
-00002ba0: 0000 73f2 0600 0074 007c 0283 0172 077c  ..s....t.|...r.|
+00002ba0: 0000 731c 0700 0074 007c 0283 0172 077c  ..s....t.|...r.|
 00002bb0: 0289 016e 0474 017c 0283 0189 017c 01a0  ...n.t.|.....|..
 00002bc0: 0288 006a 03a1 0172 1864 017d 037c 01a0  ...j...r.d.}.|..
-00002bd0: 047c 03a1 0101 007c 016a 0564 2269 0088  .|.....|.j.d"i..
+00002bd0: 047c 03a1 0101 007c 016a 0564 2469 0088  .|.....|.j.d$i..
 00002be0: 006a 0388 0169 01a4 018e 0101 0069 007d  .j...i.......i.}
 00002bf0: 0474 0674 0787 0087 0166 0264 0264 0384  .t.t.....f.d.d..
 00002c00: 0874 0888 0183 0183 0283 017d 0564 0464  .t.........}.d.d
 00002c10: 0584 007c 0544 0083 017d 0667 007d 077c  ...|.D...}.g.}.|
-00002c20: 0644 0090 035d 375c 027d 087d 097c 086a  .D...]7\.}.}.|.j
+00002c20: 0644 0090 035d 4c5c 027d 087d 097c 086a  .D...]L\.}.}.|.j
 00002c30: 097d 0a74 0a7c 0a74 0b83 0272 4f74 0c7c  .}.t.|.t...rOt.|
 00002c40: 0a83 017d 0a74 0a7c 0a74 0b83 0272 564a  ...}.t.|.t...rVJ
 00002c50: 0082 0174 0d6a 0e64 066b 0572 6074 0a7c  ...t.j.d.k.r`t.|
 00002c60: 0a74 0f83 0273 6788 00a0 107c 0aa1 0174  .t...sg....|...t
 00002c70: 1175 0072 6e88 006a 127c 0a64 0764 088d  .u.rn..j.|.d.d..
 00002c80: 027d 0a74 0a7c 0a74 1383 0272 a988 00a0  .}.t.|.t...r....
 00002c90: 147c 0aa1 0144 005d 137d 0b74 157c 0b74  .|...D.].}.t.|.t
@@ -721,1028 +721,1032 @@
 00002d00: 0272 b17c 0a6a 196e 0a74 0b7c 0a83 016a  .r.|.j.n.t.|...j
 00002d10: 1a64 0964 0a64 0b8d 0264 0c19 007d 0c7c  .d.d.d...d...}.|
 00002d20: 09a0 1b7c 086a 1ca1 0101 007c 096a 1d72  ...|.j.....|.j.r
 00002d30: df7c 086a 1e74 1f75 0172 d27c 086a 1e7c  .|.j.t.u.r.|.j.|
 00002d40: 095f 1e64 0d7c 095f 1d6e 0d7c 086a 2074  ._.d.|._.n.|.j t
 00002d50: 1f75 0172 df7c 08a0 20a1 007c 095f 1e64  .u.r.|.. ..|._.d
 00002d60: 0d7c 095f 1d88 00a0 107c 0aa1 017d 0d7c  .|._.....|...}.|
-00002d70: 0d90 0172 6f7c 0d90 0172 037c 0d74 2175  ...ro|...r.|.t!u
+00002d70: 0d90 0172 847c 0d90 0172 037c 0d74 2175  ...r.|...r.|.t!u
 00002d80: 0090 0172 0374 0688 00a0 227c 0aa1 0183  ...r.t...."|....
 00002d90: 017c 095f 237c 096a 2390 0172 0274 097c  .|._#|.j#..r.t.|
-00002da0: 096a 2364 0e19 0083 017d 0a6e 7774 247c  .j#d.....}.nwt$|
+00002da0: 096a 2364 0e19 0083 017d 0a6e 8c74 247c  .j#d.....}.n.t$|
 00002db0: 0d74 256a 266a 2783 0290 0172 1a88 006a  .t%j&j'....r...j
 00002dc0: 127c 0a64 0764 0f8d 027d 0a7c 096a 2890  .|.d.d...}.|.j(.
 00002dd0: 0173 1974 297c 095f 286e 3574 247c 0d74  .s.t)|._(n5t$|.t
 00002de0: 256a 266a 2a83 0290 0173 277c 0d74 2b75  %j&j*....s'|.t+u
 00002df0: 0090 0172 4888 006a 127c 0a64 0764 0f8d  ...rH..j.|.d.d..
 00002e00: 027d 0a7c 096a 2890 0173 477c 0d74 2b75  .}.|.j(..sG|.t+u
 00002e10: 0090 0172 3b74 2c7c 095f 286e 147c 0d74  ...r;t,|._(n.|.t
 00002e20: 2d75 0090 0172 4474 2e7c 095f 286e 0b74  -u...rDt.|._(n.t
 00002e30: 2f7c 095f 286e 0774 3090 0173 4f74 317c  /|._(n.t0..sOt1|
 00002e40: 0a83 0101 0074 247c 0a74 3283 0290 0172  .....t$|.t2....r
 00002e50: 5d64 1064 0584 007c 0a44 0083 017c 095f  ]d.d...|.D...|._
 00002e60: 2374 157c 0188 0083 0290 0172 6c74 3374  #t.|.......rlt3t
-00002e70: 347c 0a83 027c 016a 357c 096a 363c 0074  4|...|.j5|.j6<.t
-00002e80: 0b7d 0a6e 0b74 247c 0a74 3283 0290 0172  .}.n.t$|.t2....r
-00002e90: 7a74 067c 0a83 017c 095f 237c 0a7c 095f  zt.|...|._#|.|._
-00002ea0: 097c 09a0 37a1 007d 0e7c 0e64 113d 007c  .|..7..}.|.d.=.|
-00002eb0: 0ea0 3864 12a1 017d 0f7c 0f90 0173 8e67  ..8d...}.|...s.g
-00002ec0: 006e 0664 1364 0584 007c 0f44 0083 017d  .n.d.d...|.D...}
-00002ed0: 107c 0e64 1419 0090 0173 b17c 0ea0 3964  .|.d.....s.|..9d
-00002ee0: 15a1 0190 0173 b17c 1090 0173 ad64 167c  .....s.|...s.d.|
-00002ef0: 0e64 1719 00a0 3aa1 009b 0064 189d 036e  .d....:....d...n
-00002f00: 0164 197c 0e64 143c 007c 0e64 1a19 007d  .d.|.d.<.|.d...}
-00002f10: 117c 1090 0173 d27c 0e64 1a3d 007c 1190  .|...s.|.d.=.|..
-00002f20: 0173 ca7c 0ea0 3964 1ba1 0164 0075 0090  .s.|..9d...d.u..
-00002f30: 0172 ca64 1c7c 0e64 1b3c 0074 3374 347c  .r.d.|.d.<.t3t4|
-00002f40: 0a83 027c 0e64 1d3c 006e 4c7c 096a 0974  ...|.d.<.nL|.j.t
-00002f50: 3b75 0090 0172 fd74 157c 0188 0083 0290  ;u...r.t.|......
-00002f60: 0172 e774 3374 347c 0a83 027c 016a 357c  .r.t3t4|...|.j5|
-00002f70: 096a 363c 0064 1e44 005d 097d 127c 0ea0  .j6<.d.D.].}.|..
-00002f80: 387c 1264 00a1 0201 0090 0171 e97c 0e64  8|.d.......q.|.d
-00002f90: 1f19 0090 0173 fc74 3c7c 0e64 1f3c 006e  .....s.t<|.d.<.n
-00002fa0: 217c 096a 3d64 0e6b 0390 0272 0b74 3374  !|.j=d.k...r.t3t
-00002fb0: 347c 0a83 027c 0e64 1d3c 006e 137c 0a74  4|...|.d.<.n.|.t
-00002fc0: 3e75 0090 0272 1574 3f7c 0e64 1f3c 006e  >u...r.t?|.d.<.n
-00002fd0: 097c 0a74 0b75 0090 0272 1e74 407c 0e64  .|.t.u...r.t@|.d
-00002fe0: 1f3c 007c 086a 1e74 1f75 0190 0273 327c  .<.|.j.t.u...s2|
-00002ff0: 086a 2074 1f75 0190 0273 327c 0ea0 3964  .j t.u...s2|..9d
-00003000: 20a1 0164 0075 0190 0272 c97c 0ea0 3964   ..d.u...r.|..9d
-00003010: 1fa1 0190 0272 6574 247c 0e64 1f19 0074  .....ret$|.d...t
-00003020: 416a 4274 3c66 0283 0290 0272 6574 0964  AjBt<f.....ret.d
-00003030: 2164 2269 0083 0383 007d 137c 0e64 1f19  !d"i.....}.|.d..
-00003040: 007c 107c 0e64 1719 0064 238d 027c 017c  .|.|.d...d#..|.|
-00003050: 137c 0e64 2019 0064 248d 0301 0074 437c  .|.d ..d$....tC|
-00003060: 137c 0e64 1719 0083 027c 0e64 203c 006e  .|.d.....|.d <.n
-00003070: 0f64 1d7c 0e76 0090 0272 747c 0e64 1d19  .d.|.v...rt|.d..
-00003080: 007c 0e64 2019 0083 017c 0e64 203c 007c  .|.d ....|.d <.|
-00003090: 0ea0 3964 15a1 0190 0272 c97c 0e64 2019  ..9d.....r.|.d .
-000030a0: 007d 1474 0a7c 1474 0b83 0290 0273 8c74  .}.t.|.t.....s.t
-000030b0: 0a7c 1474 256a 266a 2a83 0290 0273 8f7c  .|.t%j&j*....s.|
-000030c0: 1467 017d 147c 1444 005d 377d 0b7c 0b7c  .g.}.|.D.]7}.|.|
-000030d0: 0e64 1519 0076 0190 0272 c774 0a7c 0b74  .d...v...r.t.|.t
-000030e0: 3283 0290 0272 a87c 0b6a 1c7c 0e64 1519  2....r.|.j.|.d..
-000030f0: 0076 0190 0272 c77c 0ea0 3964 1aa1 0190  .v...r.|..9d....
-00003100: 0273 b37c 0b64 0075 0090 0273 c764 257c  .s.|.d.u...s.d%|
-00003110: 0b9b 0064 267c 0e64 1719 009b 0064 277c  ...d&|.d.....d'|
-00003120: 0e64 1519 009b 009d 067d 037c 01a0 047c  .d.......}.|...|
-00003130: 03a1 0101 0090 0271 9164 287c 0c9b 009d  .......q.d(|....
-00003140: 0267 017d 157c 1190 0273 e674 157c 0ea0  .g.}.|...s.t.|..
-00003150: 3964 20a1 0174 0b83 0290 0272 e17c 15a0  9d ..t.....r.|..
-00003160: 4464 29a1 0101 006e 057c 15a0 4464 2aa1  Dd)....n.|..Dd*.
-00003170: 0101 007c 0ea0 3864 2b64 0da1 0290 0272  ...|..8d+d.....r
-00003180: f27c 15a0 4464 2ca1 0101 007c 096a 4590  .|..Dd,....|.jE.
-00003190: 0272 ff7c 15a0 4464 2d7c 096a 459b 009d  .r.|..Dd-|.jE...
-000031a0: 02a1 0101 0064 2e64 2fa0 467c 15a1 019b  .....d.d/.F|....
-000031b0: 009d 027d 167c 0ea0 3964 30a1 0190 0372  ...}.|..9d0....r
-000031c0: 187c 0e64 3005 0019 0064 317c 1617 0037  .|.d0....d1|...7
-000031d0: 0003 003c 006e 047c 167c 0e64 303c 007c  ...<.n.|.|.d0<.|
-000031e0: 0ea0 3864 3264 00a1 027d 177c 1790 0373  ..8d2d...}.|...s
-000031f0: 2c7c 1190 0372 2a64 336e 0164 347d 177c  ,|...r*d3n.d4}.|
-00003200: 04a0 397c 1764 00a1 027d 187c 1890 0373  ..9|.d...}.|...s
-00003210: 3e7c 01a0 477c 17a1 017d 187c 187c 047c  >|..G|...}.|.|.|
-00003220: 173c 007c 096a 4890 0372 697c 1190 0372  .<.|.jH..ri|...r
-00003230: 5064 357c 096a 369b 009d 027d 037c 01a0  Pd5|.j6....}.|..
-00003240: 047c 03a1 0101 007c 016a 497c 016a 4aa0  .|.....|.jI|.jJ.
-00003250: 3988 006a 4ba1 0119 007c 1719 00a0 447c  9..jK....|....D|
-00003260: 096a 367c 1090 0372 657c 1064 0c19 006e  .j6|...re|.d...n
-00003270: 0164 0066 02a1 0101 007c 186a 4c7c 1069  .d.f.....|.jL|.i
-00003280: 007c 0ea4 018e 0101 007c 07a0 447c 09a1  .|.......|..D|..
-00003290: 0101 0071 3e7c 0753 0029 364e 7a3e 5468  ...q>|.S.)6Nz>Th
-000032a0: 6973 2070 6172 7365 7220 616c 7265 6164  is parser alread
-000032b0: 7920 636f 6e74 6169 6e73 2061 7267 756d  y contains argum
-000032c0: 656e 7473 2066 726f 6d20 616e 6f74 6865  ents from anothe
-000032d0: 7220 6461 7461 636c 6173 732e 6301 0000  r dataclass.c...
-000032e0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-000032f0: 0013 0000 0073 1200 0000 8800 6a00 8801  .....s......j...
-00003300: 7c00 6a01 6401 8d02 0c00 5300 2902 4e72  |.j.d.....S.).Nr
-00003310: a300 0000 2902 72a4 0000 0072 9200 0000  ....).r....r....
-00003320: 2901 da01 66a9 02da 0363 6c73 5a05 6d6f  )...f....clsZ.mo
-00003330: 6465 6c72 5300 0000 7257 0000 0072 5e00  delrS...rW...r^.
-00003340: 0000 b201 0000 f302 0000 0012 007a 2f41  .............z/A
-00003350: 7267 756d 656e 7450 6172 7365 722e 5f61  rgumentParser._a
-00003360: 6464 5f61 7267 756d 656e 7473 2e3c 6c6f  dd_arguments.<lo
-00003370: 6361 6c73 3e2e 3c6c 616d 6264 613e 6301  cals>.<lambda>c.
-00003380: 0000 0000 0000 0000 0000 0002 0000 0007  ................
-00003390: 0000 0053 0000 0073 2000 0000 6700 7c00  ...S...s ...g.|.
-000033a0: 5d0c 7d01 7c01 7c01 6a00 a001 7402 7403  ].}.|.|.j...t.t.
-000033b0: 8300 a102 6602 9102 7102 5300 7253 0000  ....f...q.S.rS..
-000033c0: 0029 04da 086d 6574 6164 6174 61da 0367  .)...metadata..g
-000033d0: 6574 7221 0000 0072 2200 0000 7254 0000  etr!...r"...rT..
-000033e0: 0072 5300 0000 7253 0000 0072 5700 0000  .rS...rS...rW...
-000033f0: 7258 0000 00b7 0100 0073 0800 0000 0600  rX.......s......
-00003400: 0202 12ff 06ff 7a31 4172 6775 6d65 6e74  ......z1Argument
-00003410: 5061 7273 6572 2e5f 6164 645f 6172 6775  Parser._add_argu
-00003420: 6d65 6e74 732e 3c6c 6f63 616c 733e 2e3c  ments.<locals>.<
-00003430: 6c69 7374 636f 6d70 3e72 3d00 0000 5429  listcomp>r=...T)
-00003440: 01da 0d69 735f 756e 696f 6e5f 7479 7065  ...is_union_type
-00003450: da01 2e72 1700 0000 a901 da08 6d61 7873  ...r........maxs
-00003460: 706c 6974 e9ff ffff ff46 7201 0000 0029  plit.....Fr....)
-00003470: 01da 1061 7373 6572 745f 7072 696d 6974  ...assert_primit
-00003480: 6976 6563 0100 0000 0000 0000 0000 0000  ivec............
-00003490: 0200 0000 0300 0000 5300 0000 7312 0000  ........S...s...
-000034a0: 0067 007c 005d 057d 017c 016a 0091 0271  .g.|.].}.|.j...q
-000034b0: 0253 0072 5300 0000 a901 7292 0000 0072  .S.rS.....r....r
-000034c0: 5400 0000 7253 0000 0072 5300 0000 7257  T...rS...rS...rW
-000034d0: 0000 0072 5800 0000 1302 0000 72a8 0000  ...rX.......r...
-000034e0: 00da 0370 6f73 7267 0000 0063 0100 0000  ...posrg...c....
-000034f0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00003500: 5300 0000 731a 0000 0067 007c 005d 097d  S...s....g.|.].}
-00003510: 017c 01a0 0064 00a1 0172 027c 0191 0271  .|...d...r.|...q
-00003520: 0253 0029 0172 6500 0000 725f 0000 0072  .S.).re...r_...r
-00003530: 5400 0000 7253 0000 0072 5300 0000 7257  T...rS...rS...rW
-00003540: 0000 0072 5800 0000 2d02 0000 7302 0000  ...rX...-...s...
-00003550: 001a 00da 076d 6574 6176 6172 7264 0000  .....metavarrd..
-00003560: 00fa 013c da04 6465 7374 fa01 3e7a 073c  ...<..dest..>z.<
-00003570: 7661 6c75 653e da08 7265 7175 6972 6564  value>..required
-00003580: da05 6e61 7267 73fa 013f da04 7479 7065  ..nargs..?..type
-00003590: 2905 72ba 0000 0072 b800 0000 da05 636f  ).r....r......co
-000035a0: 6e73 7472 6400 0000 72b3 0000 0072 5900  nstrd...r....rY.
-000035b0: 0000 7263 0000 00da 0072 5300 0000 2902  ..rc.....rS...).
-000035c0: 7267 0000 0072 b500 0000 2903 7266 0000  rg...r....).rf..
-000035d0: 00da 096e 616d 6573 7061 6365 da06 7661  ...namespace..va
-000035e0: 6c75 6573 7a0f 496e 7661 6c69 6420 7661  luesz.Invalid va
-000035f0: 6c75 6520 277a 1027 2066 6f72 2061 7267  lue 'z.' for arg
-00003600: 756d 656e 7420 277a 1327 3b20 6d75 7374  ument 'z.'; must
-00003610: 2062 6520 6f6e 6520 6f66 3a20 7a06 5479   be one of: z.Ty
-00003620: 7065 3a20 7a16 4465 6661 756c 743a 2022  pe: z.Default: "
-00003630: 2528 6465 6661 756c 7429 7322 7a14 4465  %(default)s"z.De
-00003640: 6661 756c 743a 2025 2864 6566 6175 6c74  fault: %(default
-00003650: 2973 da09 6578 636c 7573 6976 657a 044d  )s..exclusivez.M
-00003660: 2e58 2e7a 0545 6e76 3a20 7a02 3e20 fa02  .X.z.Env: z.> ..
-00003670: 2c20 725a 0000 0072 7d00 0000 da05 6772  , rZ...r}.....gr
-00003680: 6f75 707a 1372 6571 7569 7265 6420 7061  oupz.required pa
-00003690: 7261 6d65 7465 7273 7a13 6f70 7469 6f6e  rametersz.option
-000036a0: 616c 2070 6172 616d 6574 6572 737a 3341  al parametersz3A
-000036b0: 206d 7574 7561 6c6c 792d 6578 636c 7573   mutually-exclus
-000036c0: 6976 6520 7061 7261 6d65 7465 7220 6361  ive parameter ca
-000036d0: 6e6e 6f74 2062 6520 7265 7175 6972 6564  nnot be required
-000036e0: 3a20 294d 7234 0000 0072 2500 0000 da0b  : )Mr4...r%.....
-000036f0: 6765 745f 6465 6661 756c 7472 4600 0000  get_defaultrF...
-00003700: 7282 0000 0072 9d00 0000 725d 0000 00da  r....r....r]....
-00003710: 0666 696c 7465 7272 0600 0000 72ba 0000  .filterr....r...
-00003720: 0072 3800 0000 726e 0000 0072 2300 0000  .r8...rn...r#...
-00003730: 727f 0000 00da 0c76 6572 7369 6f6e 5f69  r......version_i
-00003740: 6e66 6f72 3f00 0000 da10 5f67 6574 5f74  nfor?....._get_t
-00003750: 7970 655f 6f72 6967 696e 7215 0000 00da  ype_originr.....
-00003760: 1c5f 6578 7472 6163 745f 7479 7065 5f66  ._extract_type_f
-00003770: 726f 6d5f 636f 6e74 6169 6e65 7272 3c00  rom_containerr<.
-00003780: 0000 da12 5f67 6574 5f74 7970 655f 6d65  ...._get_type_me
-00003790: 7461 6461 7461 726d 0000 0072 0500 0000  tadatarm...r....
-000037a0: 7221 0000 0072 a900 0000 7295 0000 00da  r!...r....r.....
-000037b0: 0672 7370 6c69 74da 0873 6574 5f64 6573  .rsplit..set_des
-000037c0: 7472 9200 0000 72b7 0000 0072 6300 0000  tr....r....rc...
-000037d0: 7204 0000 00da 0f64 6566 6175 6c74 5f66  r......default_f
-000037e0: 6163 746f 7279 722a 0000 00da 0e5f 6765  actoryr*....._ge
-000037f0: 745f 7479 7065 5f61 7267 7372 6400 0000  t_type_argsrd...
-00003800: 7239 0000 00da 0b63 6f6c 6c65 6374 696f  r9.....collectio
-00003810: 6e73 da03 6162 63da 074d 6170 7069 6e67  ns..abc..Mapping
-00003820: 7259 0000 0072 1d00 0000 da08 4974 6572  rY...r......Iter
-00003830: 6162 6c65 da03 7365 7472 1f00 0000 da05  able..setr......
-00003840: 7475 706c 6572 2000 0000 721e 0000 0072  tupler ...r....r
-00003850: 3500 0000 7227 0000 0072 0700 0000 7208  5...r'...r....r.
-00003860: 0000 0072 3100 0000 7272 0000 0072 b500  ...r1...rr...r..
-00003870: 0000 da06 6173 6469 6374 7297 0000 0072  ....asdictr....r
-00003880: aa00 0000 da05 7570 7065 72da 0462 6f6f  ......upper..boo
-00003890: 6c72 1800 0000 72b8 0000 00da 0369 6e74  lr....r......int
-000038a0: 7219 0000 0072 1a00 0000 7274 0000 00da  r....r....rt....
-000038b0: 0641 6374 696f 6eda 0767 6574 6174 7472  .Action..getattr
-000038c0: da06 6170 7065 6e64 da08 5f65 6e76 5f76  ..append.._env_v
-000038d0: 6172 da04 6a6f 696e da12 6164 645f 6172  ar..join..add_ar
-000038e0: 6775 6d65 6e74 5f67 726f 7570 72bf 0000  gument_groupr...
-000038f0: 0072 7100 0000 da09 5f64 6566 6175 6c74  .rq....._default
-00003900: 7372 4500 0000 726f 0000 0029 1972 a700  srE...ro...).r..
-00003910: 0000 7266 0000 0072 8f00 0000 da03 6572  ..rf...r......er
-00003920: 725a 1170 6172 7365 725f 6172 675f 6772  rZ.parser_arg_gr
-00003930: 6f75 7073 5a0c 6e6f 7665 6c5f 6669 656c  oupsZ.novel_fiel
-00003940: 6473 5a10 6e6f 7665 6c5f 6669 656c 645f  dsZ.novel_field_
-00003950: 6172 6773 5a0a 6164 6465 645f 6172 6773  argsZ.added_args
-00003960: 5a03 666c 645a 1161 7267 7061 7273 655f  Z.fldZ.argparse_
-00003970: 6172 6775 6d65 6e74 da08 666c 645f 7479  argument..fld_ty
-00003980: 7065 7256 0000 005a 0968 656c 705f 7479  perV...Z.help_ty
-00003990: 7065 5a0f 666c 645f 7479 7065 5f6f 7269  peZ.fld_type_ori
-000039a0: 6769 6e72 5100 0000 7267 0000 0072 5000  ginrQ...rg...rP.
-000039b0: 0000 72b7 0000 00da 016b 5a0f 6475 6d6d  ..r......kZ.dumm
-000039c0: 795f 6e61 6d65 7370 6163 65da 0164 5a0e  y_namespace..dZ.
-000039d0: 6865 6c70 5f6d 7367 5f70 6172 7473 5a08  help_msg_partsZ.
-000039e0: 6865 6c70 5f6d 7367 72c1 0000 005a 0961  help_msgr....Z.a
-000039f0: 7267 5f67 726f 7570 7253 0000 0072 a600  rg_grouprS...r..
-00003a00: 0000 7257 0000 0072 9000 0000 9901 0000  ..rW...r........
-00003a10: 739c 0100 0008 0a06 0108 020c 0204 010a  s...............
-00003a20: 0116 0204 0202 0202 010c 0106 0102 fe04  ................
-00003a30: ff06 0702 0206 fe04 050e 0206 010a 0408  ................
-00003a40: 010e 0114 030e 0104 0102 0102 0106 fe0a  ................
-00003a50: 050e 0114 010a 0104 0102 800a 0214 030e  ................
-00003a60: 0104 0102 0102 0106 fe08 0708 ff14 0202  ................
-00003a70: fd0c 0606 020a 0108 0108 010a 010a 0106  ................
-00003a80: 010a 0206 0110 0110 0108 010e 0102 8010  ................
-00003a90: 0304 0102 0102 0106 fe08 0406 0102 800c  ................
-00003aa0: 0304 ff0a 0204 0202 0102 0106 fe08 040a  ................
-00003ab0: 0108 010a 0108 0106 0202 8006 0208 010c  ................
-00003ac0: 0210 010c 0202 0302 0102 010c fe06 070c  ................
-00003ad0: 020a 0106 0208 0206 010a 0202 0308 ff0c  ................
-00003ae0: 0202 fd16 061c 0206 ff08 0406 0206 0216  ................
-00003af0: 0108 0110 010c 010c 0102 0302 0102 010c  ................
-00003b00: fe08 0510 010a 0108 0102 800c 0210 010a  ................
-00003b10: 010a 020a 0108 020c 040c 0110 010e 0206  ................
-00003b20: 0108 0106 fe0e 0512 0102 0102 0106 0106  ................
-00003b30: fd14 050a 0114 010c 0308 010e 0102 0106  ................
-00003b40: 0106 fe06 0408 020e 0208 0204 fe10 0308  ................
-00003b50: 0304 fd0a 0312 0306 0104 ff02 ff0a 0404  ................
-00003b60: 800c 0206 0312 010c 010a 020e 020a 0108  ................
-00003b70: 0212 0110 020c 0216 0108 020c 0206 020e  ................
-00003b80: 010c 0206 020a 0108 0108 0206 0102 0204  ................
-00003b90: 0104 ff02 ff0a 0404 020c 0102 ff02 0202  ................
-00003ba0: fe02 0204 0210 0102 fe04 ff10 070c 0204  ................
-00003bb0: 027a 1d41 7267 756d 656e 7450 6172 7365  .z.ArgumentParse
-00003bc0: 722e 5f61 6464 5f61 7267 756d 656e 7473  r._add_arguments
-00003bd0: da01 7463 0100 0000 0000 0000 0000 0000  ..tc............
-00003be0: 0100 0000 0400 0000 4300 0000 730c 0000  ........C...s...
-00003bf0: 0074 007c 0064 0164 0083 0353 0029 024e  .t.|.d.d...S.).N
-00003c00: da0a 5f5f 6f72 6967 696e 5f5f a901 72d7  ..__origin__..r.
-00003c10: 0000 00a9 0172 e100 0000 7253 0000 0072  .....r....rS...r
-00003c20: 5300 0000 7257 0000 0072 c500 0000 ba02  S...rW...r......
-00003c30: 0000 f302 0000 000c 027a 1f41 7267 756d  .........z.Argum
-00003c40: 656e 7450 6172 7365 722e 5f67 6574 5f74  entParser._get_t
-00003c50: 7970 655f 6f72 6967 696e 6301 0000 0000  ype_originc.....
-00003c60: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-00003c70: 0000 00f3 0c00 0000 7400 7c00 6401 6402  ........t.|.d.d.
-00003c80: 8303 5300 2903 4eda 085f 5f61 7267 735f  ..S.).N..__args_
-00003c90: 5f72 5300 0000 72e3 0000 0072 e400 0000  _rS...r....r....
-00003ca0: 7253 0000 0072 5300 0000 7257 0000 0072  rS...rS...rW...r
-00003cb0: cb00 0000 be02 0000 72e5 0000 007a 1d41  ........r....z.A
-00003cc0: 7267 756d 656e 7450 6172 7365 722e 5f67  rgumentParser._g
-00003cd0: 6574 5f74 7970 655f 6172 6773 6301 0000  et_type_argsc...
-00003ce0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-00003cf0: 0043 0000 0072 e600 0000 2903 4eda 0c5f  .C...r....).N.._
-00003d00: 5f6d 6574 6164 6174 615f 5f72 5300 0000  _metadata__rS...
-00003d10: 72e3 0000 0072 e400 0000 7253 0000 0072  r....r....rS...r
-00003d20: 5300 0000 7257 0000 0072 c700 0000 c202  S...rW...r......
-00003d30: 0000 72e5 0000 007a 2141 7267 756d 656e  ..r....z!Argumen
-00003d40: 7450 6172 7365 722e 5f67 6574 5f74 7970  tParser._get_typ
-00003d50: 655f 6d65 7461 6461 7461 da0e 7479 7065  e_metadata..type
-00003d60: 5f63 6f6e 7461 696e 6572 72b0 0000 0072  _containerr....r
-00003d70: ab00 0000 6304 0000 0000 0000 0000 0000  ....c...........
-00003d80: 000b 0000 0003 0000 0043 0000 0073 1801  .........C...s..
-00003d90: 0000 7c03 7204 7400 6e04 7c00 a001 7c01  ..|.r.t.n.|...|.
-00003da0: a101 7d04 7c04 6400 7500 7215 7402 6401  ..}.|.d.u.r.t.d.
-00003db0: 7c01 6a03 9b00 9d02 8301 8201 7c00 a004  |.j.........|...
-00003dc0: 7c01 a101 7d05 6402 6403 8400 7c05 4400  |...}.d.d...|.D.
-00003dd0: 8301 7d06 7c04 7400 7500 7330 7405 7c04  ..}.|.t.u.s0t.|.
-00003de0: 7406 6a07 6a08 8302 7330 7c04 7409 7500  t.j.j...s0|.t.u.
-00003df0: 7240 740a 7c06 8301 6404 6b03 723b 7c06  r@t.|...d.k.r;|.
-00003e00: a00b a100 0100 6e2c 7c06 6405 1900 7d07  ......n,|.d...}.
-00003e10: 6e27 7405 7c04 7406 6a07 6a0c 8302 7261  n't.|.t.j.j...ra
-00003e20: 740a 7c06 8301 6406 6b03 7252 7c06 a00b  t.|...d.k.rR|...
-00003e30: a100 0100 6e15 7c06 5c02 7d08 7d09 7c08  ....n.|.\.}.}.|.
-00003e40: 740d 7501 725e 7402 6407 8301 8201 7c09  t.u.r^t.d.....|.
-00003e50: 7d07 6e06 740e 7367 740f 7c01 8301 0100  }.n.t.sgt.|.....
-00003e60: 7c06 736d 7402 6408 8301 8201 7c00 a001  |.smt.d.....|...
-00003e70: 7c07 a101 7d0a 7c0a 7400 7500 7280 7c00  |...}.|.t.u.r.|.
-00003e80: a010 7c07 a101 7d07 7c00 a001 7c07 a101  ..|...}.|...|...
-00003e90: 7d0a 7c02 728a 7c0a 728a 740e 738a 740f  }.|.r.|.r.t.s.t.
-00003ea0: 7c0a 8301 0100 7c07 5300 2909 4e7a 1f47  |.....|.S.).Nz.G
-00003eb0: 6976 656e 2074 7970 6520 6973 206e 6f74  iven type is not
-00003ec0: 2061 2063 6f6e 7461 696e 6572 3a20 6301   a container: c.
-00003ed0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00003ee0: 0000 0053 0000 0073 2000 0000 6700 7c00  ...S...s ...g.|.
-00003ef0: 5d0c 7d01 7c01 6400 7501 7202 7c01 7400  ].}.|.d.u.r.|.t.
-00003f00: 7501 7202 7c01 9102 7102 5300 2901 2e29  u.r.|...q.S.)..)
-00003f10: 0172 2b00 0000 2902 7255 0000 00da 0161  .r+...).rU.....a
-00003f20: 7253 0000 0072 5300 0000 7257 0000 0072  rS...rS...rW...r
-00003f30: 5800 0000 d802 0000 7304 0000 0006 001a  X.......s.......
-00003f40: 017a 3f41 7267 756d 656e 7450 6172 7365  .z?ArgumentParse
-00003f50: 722e 5f65 7874 7261 6374 5f74 7970 655f  r._extract_type_
-00003f60: 6672 6f6d 5f63 6f6e 7461 696e 6572 2e3c  from_container.<
-00003f70: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00003f80: 703e 7217 0000 0072 0100 0000 727c 0000  p>r....r....r|..
-00003f90: 007a 2244 6963 7469 6f6e 6172 7920 6b65  .z"Dictionary ke
-00003fa0: 7973 206d 7573 7420 6265 2074 7970 6520  ys must be type 
-00003fb0: 6073 7472 607a 1b54 6f6f 206d 616e 7920  `str`z.Too many 
-00003fc0: 7479 7065 7320 696e 2063 6f6e 7461 696e  types in contain
-00003fd0: 6572 2911 7215 0000 0072 c500 0000 da09  er).r....r......
-00003fe0: 5479 7065 4572 726f 7272 9500 0000 72cb  TypeErrorr....r.
-00003ff0: 0000 0072 3900 0000 72cc 0000 0072 cd00  ...r9...r....r..
-00004000: 0000 7211 0000 0072 d000 0000 7276 0000  ..r....r....rv..
-00004010: 00da 0563 6c65 6172 72ce 0000 0072 6e00  ...clearr....rn.
-00004020: 0000 7235 0000 0072 2700 0000 72c6 0000  ..r5...r'...r...
-00004030: 0029 0b72 a700 0000 72e9 0000 0072 b000  .).r....r....r..
-00004040: 0000 72ab 0000 005a 1574 7970 655f 636f  ..r....Z.type_co
-00004050: 6e74 6169 6e65 725f 6f72 6967 696e 5a13  ntainer_originZ.
-00004060: 7479 7065 5f63 6f6e 7461 696e 6572 5f61  type_container_a
-00004070: 7267 73da 0772 6573 756c 7473 5a16 7479  rgs..resultsZ.ty
-00004080: 7065 5f63 6f6e 7461 696e 6572 5f73 7562  pe_container_sub
-00004090: 7479 7065 5a08 6b65 795f 7479 7065 5a0a  typeZ.key_typeZ.
-000040a0: 7661 6c75 655f 7479 7065 5a1d 7479 7065  value_typeZ.type
-000040b0: 5f63 6f6e 7461 696e 6572 5f73 7562 7479  _container_subty
-000040c0: 7065 5f6f 7269 6769 6e72 5300 0000 7253  pe_originrS...rS
-000040d0: 0000 0072 5700 0000 72c6 0000 00c6 0200  ...rW...r.......
-000040e0: 0073 5400 0000 1008 02ff 0804 0201 0a01  .sT.............
-000040f0: 04ff 0a04 0602 0201 06ff 0807 0c01 02ff  ................
-00004100: 0802 0c02 0a01 0a02 0e01 0c01 0a01 0802  ................
-00004110: 0801 0801 0601 0401 0801 0402 0801 0a02  ................
-00004120: 0802 0401 0201 04ff 0a03 0203 02ff 0202  ................
-00004130: 02fe 0203 02fd 0805 0402 7a2b 4172 6775  ..........z+Argu
-00004140: 6d65 6e74 5061 7273 6572 2e5f 6578 7472  mentParser._extr
-00004150: 6163 745f 7479 7065 5f66 726f 6d5f 636f  act_type_from_co
-00004160: 6e74 6169 6e65 7263 0100 0000 0000 0000  ntainerc........
-00004170: 0000 0000 0200 0000 0600 0000 0b00 0000  ................
-00004180: 7364 0000 007c 01a0 0064 0164 02a1 027c  sd...|...d.d...|
-00004190: 0164 013c 007c 01a0 0064 0364 04a1 027c  .d.<.|...d.d...|
-000041a0: 0164 033c 007c 01a0 0064 0588 006a 01a1  .d.<.|...d...j..
-000041b0: 027c 0164 053c 007c 01a0 0064 0687 0066  .|.d.<.|...d...f
-000041c0: 0164 0764 0884 08a1 027c 0164 063c 0074  .d.d.....|.d.<.t
-000041d0: 0283 006a 0364 0969 007c 01a4 018e 0188  ...j.d.i.|......
-000041e0: 005f 0488 006a 0453 0029 0a4e 726c 0000  ._...j.S.).Nrl..
-000041f0: 005a 0863 6f6d 6d61 6e64 7372 b300 0000  .Z.commandsr....
-00004200: 7a09 3c43 4f4d 4d41 4e44 3e72 b500 0000  z.<COMMAND>r....
-00004210: da0c 7061 7273 6572 5f63 6c61 7373 6300  ..parser_classc.
-00004220: 0000 0000 0000 0000 0000 0001 0000 0006  ................
-00004230: 0000 001b 0000 0073 1e00 0000 7400 8800  .......s....t...
-00004240: 8301 6403 6900 7c00 a401 6401 8800 6a01  ..d.i.|...d...j.
-00004250: 6402 9c02 a401 8e01 5300 2904 4e54 2902  d.......S.).NT).
-00004260: 724f 0000 0072 4e00 0000 7253 0000 0029  rO...rN...rS...)
-00004270: 0272 ba00 0000 724e 0000 0029 0172 df00  .r....rN...).r..
-00004280: 0000 a901 7278 0000 0072 5300 0000 7257  ....rx...rS...rW
-00004290: 0000 0072 5e00 0000 0c03 0000 730c 0000  ...r^.......s...
-000042a0: 000a 0002 0102 ff02 0204 010a fd7a 2f41  .............z/A
-000042b0: 7267 756d 656e 7450 6172 7365 722e 6164  rgumentParser.ad
-000042c0: 645f 7375 6270 6172 7365 7273 2e3c 6c6f  d_subparsers.<lo
-000042d0: 6361 6c73 3e2e 3c6c 616d 6264 613e 7253  cals>.<lambda>rS
-000042e0: 0000 0029 0572 aa00 0000 7244 0000 0072  ...).r....rD...r
-000042f0: 6800 0000 da0e 6164 645f 7375 6270 6172  h.....add_subpar
-00004300: 7365 7273 726a 0000 0029 0272 7800 0000  sersrj...).rx...
-00004310: 7251 0000 0072 7900 0000 72ef 0000 0072  rQ...ry...r....r
-00004320: 5700 0000 72f0 0000 0006 0300 0073 1200  W...r........s..
-00004330: 0000 1001 1001 1201 0401 0201 0a01 08fe  ................
-00004340: 1409 0602 7a1d 4172 6775 6d65 6e74 5061  ....z.ArgumentPa
-00004350: 7273 6572 2e61 6464 5f73 7562 7061 7273  rser.add_subpars
-00004360: 6572 7363 0100 0000 0000 0000 0000 0000  ersc............
-00004370: 0200 0000 0400 0000 4300 0000 732c 0000  ........C...s,..
-00004380: 007c 006a 0044 005d 107d 0174 017c 0174  .|.j.D.].}.t.|.t
-00004390: 026a 0383 0272 137c 017c 005f 047c 006a  .j...r.|.|._.|.j
-000043a0: 0402 0001 0053 0071 0364 0053 0072 5c00  .....S.q.d.S.r\.
-000043b0: 0000 2905 da08 5f61 6374 696f 6e73 726d  ..)..._actionsrm
-000043c0: 0000 0072 7400 0000 7296 0000 0072 6a00  ...rt...r....rj.
-000043d0: 0000 2902 7278 0000 0072 ea00 0000 7253  ..).rx...r....rS
-000043e0: 0000 0072 5300 0000 7257 0000 0072 8c00  ...rS...rW...r..
-000043f0: 0000 1703 0000 7312 0000 000a 0102 0102  ......s.........
-00004400: 0104 0104 fe06 040a 0102 fb04 067a 2641  .............z&A
-00004410: 7267 756d 656e 7450 6172 7365 722e 5f66  rgumentParser._f
-00004420: 696e 645f 7375 6270 6172 7365 7273 5f61  ind_subparsers_a
-00004430: 6374 696f 6e63 0100 0000 0000 0000 0000  ctionc..........
-00004440: 0000 0100 0000 0200 0000 4300 0000 7336  ..........C...s6
-00004450: 0000 007c 006a 0064 0075 0172 087c 006a  ...|.j.d.u.r.|.j
-00004460: 0053 007c 006a 0172 177c 00a0 02a1 0001  .S.|.j.r.|......
-00004470: 007c 006a 0073 144a 0082 017c 006a 0053  .|.j.s.J...|.j.S
-00004480: 007c 00a0 03a1 0053 0072 5c00 0000 2904  .|.....S.r\...).
-00004490: 726a 0000 0072 8b00 0000 728c 0000 0072  rj...r....r....r
-000044a0: f000 0000 72ef 0000 0072 5300 0000 7253  ....r....rS...rS
-000044b0: 0000 0072 5700 0000 7277 0000 0021 0300  ...rW...rw...!..
-000044c0: 0073 0e00 0000 0a01 0601 0602 0801 0a01  .s..............
-000044d0: 0601 0802 7a25 4172 6775 6d65 6e74 5061  ....z%ArgumentPa
-000044e0: 7273 6572 2e5f 6765 745f 6f72 5f61 6464  rser._get_or_add
-000044f0: 5f73 7562 7061 7273 6572 7372 bd00 0000  _subparsersr....
-00004500: 6302 0000 0000 0000 0000 0000 0006 0000  c...............
-00004510: 0006 0000 0003 0000 0073 6e00 0000 7c00  .........sn...|.
-00004520: 6a00 a001 7402 8800 7c00 6a03 6400 8303  j...t...|.j.d...
-00004530: 6900 a102 7d02 7c02 a004 a100 4400 5d1d  i...}.|.....D.].
-00004540: 7d03 8700 6601 6401 6402 8408 7c03 4400  }...f.d.d...|.D.
-00004550: 8301 7d04 7405 7c04 8301 6403 6b04 722d  ..}.t.|...d.k.r-
-00004560: 6404 6405 a006 7c04 a101 1700 7d05 7c00  d.d...|.....}.|.
-00004570: a007 7c05 a101 0100 7110 7408 6406 6900  ..|.....q.t.d.i.
-00004580: 7409 8800 8301 a401 8e01 5300 2907 4e63  t.........S.).Nc
-00004590: 0100 0000 0000 0000 0000 0000 0400 0000  ................
-000045a0: 0500 0000 1300 0000 736c 0000 0067 007c  ........sl...g.|
-000045b0: 005d 325c 027d 017d 0274 0088 007c 0183  .]2\.}.}.t...|..
-000045c0: 0272 3474 0188 007c 0183 027d 0374 027c  .r4t...|...}.t.|
-000045d0: 0374 0383 0273 1c74 027c 0374 046a 056a  .t...s.t.|.t.j.j
-000045e0: 0683 0273 207c 0364 0075 0173 2e74 027c  ...s |.d.u.s.t.|
-000045f0: 0374 0383 0273 0274 027c 0374 046a 056a  .t...s.t.|.t.j.j
-00004600: 0683 0272 027c 0372 027c 0272 327c 026e  ...r.|.r.|.r2|.n
-00004610: 017c 0191 0271 0253 0072 5c00 0000 2907  .|...q.S.r\...).
-00004620: da07 6861 7361 7474 7272 d700 0000 7238  ..hasattrr....r8
-00004630: 0000 0072 6e00 0000 72cc 0000 0072 cd00  ...rn...r....r..
-00004640: 0000 72cf 0000 0029 0472 5500 0000 72b5  ..r....).rU...r.
-00004650: 0000 00da 0466 6c61 675a 0a61 7474 725f  .....flagZ.attr_
-00004660: 7661 6c75 65a9 0172 bd00 0000 7253 0000  value..r....rS..
-00004670: 0072 5700 0000 7258 0000 003b 0300 0073  .rW...rX...;...s
-00004680: 3000 0000 0600 0602 0801 02fd 0a04 0803  0...............
-00004690: 02f9 0208 0201 0601 02fe 02f8 080d 0803  ................
-000046a0: 02fd 0204 0201 0601 02fe 02fc 0208 02f8  ................
-000046b0: 0af4 060c 7a33 4172 6775 6d65 6e74 5061  ....z3ArgumentPa
-000046c0: 7273 6572 2e5f 706f 7374 5f70 6172 7365  rser._post_parse
-000046d0: 5f61 7267 732e 3c6c 6f63 616c 733e 2e3c  _args.<locals>.<
-000046e0: 6c69 7374 636f 6d70 3e72 1700 0000 7a28  listcomp>r....z(
-000046f0: 5468 6573 6520 6172 6775 6d65 6e74 7320  These arguments 
-00004700: 6172 6520 6d75 7475 616c 6c79 2065 7863  are mutually exc
-00004710: 6c75 7369 7665 3a20 72c0 0000 0072 5300  lusive: r....rS.
-00004720: 0000 290a 7271 0000 0072 aa00 0000 72d7  ..).rq...r....r.
-00004730: 0000 0072 4500 0000 72be 0000 0072 7600  ...rE...r....rv.
-00004740: 0000 72da 0000 0072 8200 0000 7228 0000  ..r....r....r(..
-00004750: 00da 0476 6172 7329 0672 7800 0000 72bd  ...vars).rx...r.
-00004760: 0000 005a 1266 756e 635f 6d78 5f61 7267  ...Z.func_mx_arg
-00004770: 5f67 726f 7570 735a 0667 5f61 7267 735a  _groupsZ.g_argsZ
-00004780: 0e6d 785f 666c 6167 735f 666f 756e 6472  .mx_flags_foundr
-00004790: dd00 0000 7253 0000 0072 f400 0000 7257  ....rS...r....rW
-000047a0: 0000 00da 105f 706f 7374 5f70 6172 7365  ....._post_parse
-000047b0: 5f61 7267 732c 0300 0073 2000 0000 0607  _args,...s .....
-000047c0: 0c01 0201 02fe 02fd 0c07 0a04 0202 06fe  ................
-000047d0: 0c19 0601 0201 06ff 0a03 0280 1202 7a1f  ..............z.
-000047e0: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
-000047f0: 706f 7374 5f70 6172 7365 5f61 7267 7363  post_parse_argsc
-00004800: 0300 0000 0000 0000 0000 0000 0500 0000  ................
-00004810: 0a00 0000 0300 0000 7352 0000 007a 0e74  ........sR...z.t
-00004820: 0083 006a 017c 017c 0264 018d 027d 037c  ...j.|.|.d...}.|
-00004830: 00a0 027c 03a1 0157 0053 0004 0074 0379  ...|...W.S...t.y
-00004840: 2801 007d 0401 007a 0e7c 00a0 0474 057c  (..}...z.|...t.|
-00004850: 0483 01a1 0101 0057 0059 0064 007d 047e  .......W.Y.d.}.~
-00004860: 0464 0053 0064 007d 047e 0477 0177 00a9  .d.S.d.}.~.w.w..
-00004870: 024e 2902 7250 0000 0072 bd00 0000 2906  .N).rP...r....).
-00004880: 7268 0000 00da 0a70 6172 7365 5f61 7267  rh.....parse_arg
-00004890: 7372 f600 0000 da0a 5661 6c75 6545 7272  sr......ValueErr
-000048a0: 6f72 7282 0000 0072 6e00 0000 2905 7278  orr....rn...).rx
-000048b0: 0000 0072 5000 0000 72bd 0000 00da 0670  ...rP...r......p
-000048c0: 6172 7365 64da 0165 7279 0000 0072 5300  arsed..ery...rS.
-000048d0: 0000 7257 0000 0072 f800 0000 5c03 0000  ..rW...r....\...
-000048e0: 7314 0000 0002 0506 0102 0102 0106 fe0c  s...............
-000048f0: 040e 011c 0108 8002 ff7a 1941 7267 756d  .........z.Argum
-00004900: 656e 7450 6172 7365 722e 7061 7273 655f  entParser.parse_
-00004910: 6172 6773 6303 0000 0000 0000 0000 0000  argsc...........
-00004920: 0006 0000 000a 0000 0003 0000 0073 5a00  .............sZ.
-00004930: 0000 7a12 7400 8300 6a01 7c01 7c02 6401  ..z.t...j.|.|.d.
-00004940: 8d02 5c02 7d03 7d04 7c00 a002 7c03 a101  ..\.}.}.|...|...
-00004950: 7c04 6602 5700 5300 0400 7403 792c 0100  |.f.W.S...t.y,..
-00004960: 7d05 0100 7a0e 7c00 a004 7405 7c05 8301  }...z.|...t.|...
-00004970: a101 0100 5700 5900 6400 7d05 7e05 6400  ....W.Y.d.}.~.d.
-00004980: 5300 6400 7d05 7e05 7701 7700 72f7 0000  S.d.}.~.w.w.r...
-00004990: 0029 0672 6800 0000 da10 7061 7273 655f  .).rh.....parse_
-000049a0: 6b6e 6f77 6e5f 6172 6773 72f6 0000 0072  known_argsr....r
-000049b0: f900 0000 7282 0000 0072 6e00 0000 2906  ....r....rn...).
-000049c0: 7278 0000 0072 5000 0000 72bd 0000 0072  rx...rP...r....r
-000049d0: fa00 0000 da07 756e 6b6e 6f77 6e72 fb00  ......unknownr..
-000049e0: 0000 7279 0000 0072 5300 0000 7257 0000  ..ry...rS...rW..
-000049f0: 0072 fc00 0000 6a03 0000 730e 0000 0002  .r....j...s.....
-00004a00: 0714 0110 010e 011c 0108 8002 ff7a 1f41  .............z.A
-00004a10: 7267 756d 656e 7450 6172 7365 722e 7061  rgumentParser.pa
-00004a20: 7273 655f 6b6e 6f77 6e5f 6172 6773 da18  rse_known_args..
-00004a30: 736b 6970 5f70 7964 616e 7469 635f 7661  skip_pydantic_va
-00004a40: 6c69 6461 7469 6f6e 6304 0000 0000 0000  lidationc.......
-00004a50: 0000 0000 0006 0000 0005 0000 0043 0000  .............C..
-00004a60: 0073 2200 0000 7c00 a000 7c01 a101 5c02  .s"...|...|...\.
-00004a70: 7d04 7d05 7c00 6a01 7c04 7c02 7c03 6401  }.}.|.j.|.|.|.d.
-00004a80: 8d03 7c05 6602 5300 2902 61c9 0200 0055  ..|.f.S.).a....U
-00004a90: 7365 2070 6172 7365 6420 6172 6773 2074  se parsed args t
-00004aa0: 6f20 696e 7374 616e 7469 6174 6520 7468  o instantiate th
-00004ab0: 6520 6769 7665 6e20 6461 7461 206d 6f64  e given data mod
-00004ac0: 656c 2e0a 0a20 2020 2020 2020 2041 7267  el...        Arg
-00004ad0: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
-00004ae0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00004af0: 2061 7267 735f 6d6f 6465 6c3a 0a20 2020   args_model:.   
-00004b00: 2020 2020 2020 2020 2073 6b69 705f 7079           skip_py
-00004b10: 6461 6e74 6963 5f76 616c 6964 6174 696f  dantic_validatio
-00004b20: 6e3a 0a0a 2020 2020 2020 2020 4578 616d  n:..        Exam
-00004b30: 706c 6573 3a0a 2020 2020 2020 2020 2020  ples:.          
-00004b40: 2020 3e3e 3e20 696d 706f 7274 2079 6170    >>> import yap
-00004b50: 780a 2020 2020 2020 2020 2020 2020 3e3e  x.            >>
-00004b60: 3e20 6672 6f6d 2064 6174 6163 6c61 7373  > from dataclass
-00004b70: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
-00004b80: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
-00004b90: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-00004ba0: 3e3e 3e20 4064 6174 6163 6c61 7373 0a20  >>> @dataclass. 
-00004bb0: 2020 2020 2020 2020 2020 202e 2e2e 2063             ... c
-00004bc0: 6c61 7373 2041 6464 4e75 6d73 3a0a 2020  lass AddNums:.  
-00004bd0: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
-00004be0: 2020 783a 2069 6e74 0a20 2020 2020 2020    x: int.       
-00004bf0: 2020 2020 202e 2e2e 2020 2020 2079 3a20       ...     y: 
-00004c00: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
-00004c10: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-00004c20: 3e3e 3e20 7061 7273 6572 203d 2079 6170  >>> parser = yap
-00004c30: 782e 4172 6775 6d65 6e74 5061 7273 6572  x.ArgumentParser
-00004c40: 2829 0a20 2020 2020 2020 2020 2020 203e  ().            >
-00004c50: 3e3e 2070 6172 7365 722e 6164 645f 6172  >> parser.add_ar
-00004c60: 6775 6d65 6e74 7328 4164 644e 756d 7329  guments(AddNums)
-00004c70: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
-00004c80: 2070 6172 7365 642c 2075 6e6b 6e6f 776e   parsed, unknown
-00004c90: 203d 2070 6172 7365 722e 7061 7273 655f   = parser.parse_
-00004ca0: 6b6e 6f77 6e5f 6172 6773 5f74 6f5f 6d6f  known_args_to_mo
-00004cb0: 6465 6c28 5b27 2d78 272c 2027 3127 2c20  del(['-x', '1', 
-00004cc0: 272d 7927 2c20 2732 272c 2027 2d7a 272c  '-y', '2', '-z',
-00004cd0: 2027 3327 5d29 0a20 2020 2020 2020 2020   '3']).         
-00004ce0: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
-00004cf0: 2020 203e 3e3e 2028 7061 7273 6564 2e78     >>> (parsed.x
-00004d00: 2c20 7061 7273 6564 2e79 290a 2020 2020  , parsed.y).    
-00004d10: 2020 2020 2020 2020 2831 2c20 3229 0a20          (1, 2). 
-00004d20: 2020 2020 2020 2020 2020 203e 3e3e 2075             >>> u
-00004d30: 6e6b 6e6f 776e 0a20 2020 2020 2020 2020  nknown.         
-00004d40: 2020 205b 272d 7a27 2c20 2733 275d 0a0a     ['-z', '3']..
-00004d50: 2020 2020 2020 2020 a903 7250 0000 0072          ..rP...r
-00004d60: 8f00 0000 72fe 0000 0029 0272 fc00 0000  ....r....).r....
-00004d70: da14 5f70 6172 7365 5f61 7267 735f 746f  .._parse_args_to
-00004d80: 5f6d 6f64 656c 2906 7278 0000 0072 5000  _model).rx...rP.
-00004d90: 0000 728f 0000 0072 fe00 0000 da0b 7061  ..r....r......pa
-00004da0: 7273 6564 5f61 7267 73da 0c75 6e6b 6e6f  rsed_args..unkno
-00004db0: 776e 5f61 7267 7372 5300 0000 7253 0000  wn_argsrS...rS..
-00004dc0: 0072 5700 0000 da19 7061 7273 655f 6b6e  .rW.....parse_kn
-00004dd0: 6f77 6e5f 6172 6773 5f74 6f5f 6d6f 6465  own_args_to_mode
-00004de0: 6c77 0300 0073 1000 0000 0e23 0403 0201  lw...s.....#....
-00004df0: 0201 0201 04fd 0205 04fa 7a28 4172 6775  ..........z(Argu
-00004e00: 6d65 6e74 5061 7273 6572 2e70 6172 7365  mentParser.parse
-00004e10: 5f6b 6e6f 776e 5f61 7267 735f 746f 5f6d  _known_args_to_m
-00004e20: 6f64 656c 6304 0000 0000 0000 0000 0000  odelc...........
-00004e30: 0005 0000 0005 0000 0043 0000 0073 1a00  .........C...s..
-00004e40: 0000 7c00 a000 7c01 a101 7d04 7c00 6a01  ..|...|...}.|.j.
-00004e50: 7c04 7c02 7c03 6401 8d03 5300 2902 617f  |.|.|.d...S.).a.
-00004e60: 0200 0055 7365 2070 6172 7365 6420 6172  ...Use parsed ar
-00004e70: 6773 2074 6f20 696e 7374 616e 7469 6174  gs to instantiat
-00004e80: 6520 7468 6520 6769 7665 6e20 6461 7461  e the given data
-00004e90: 206d 6f64 656c 2e0a 0a20 2020 2020 2020   model...       
-00004ea0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00004eb0: 2020 2061 7267 733a 0a20 2020 2020 2020     args:.       
-00004ec0: 2020 2020 2061 7267 735f 6d6f 6465 6c3a       args_model:
-00004ed0: 0a20 2020 2020 2020 2020 2020 2073 6b69  .            ski
-00004ee0: 705f 7079 6461 6e74 6963 5f76 616c 6964  p_pydantic_valid
-00004ef0: 6174 696f 6e3a 0a0a 2020 2020 2020 2020  ation:..        
-00004f00: 4578 616d 706c 6573 3a0a 2020 2020 2020  Examples:.      
-00004f10: 2020 2020 2020 3e3e 3e20 696d 706f 7274        >>> import
-00004f20: 2079 6170 780a 2020 2020 2020 2020 2020   yapx.          
-00004f30: 2020 3e3e 3e20 6672 6f6d 2064 6174 6163    >>> from datac
-00004f40: 6c61 7373 6573 2069 6d70 6f72 7420 6461  lasses import da
-00004f50: 7461 636c 6173 730a 2020 2020 2020 2020  taclass.        
-00004f60: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
-00004f70: 2020 2020 3e3e 3e20 4064 6174 6163 6c61      >>> @datacla
-00004f80: 7373 0a20 2020 2020 2020 2020 2020 202e  ss.            .
-00004f90: 2e2e 2063 6c61 7373 2041 6464 4e75 6d73  .. class AddNums
-00004fa0: 3a0a 2020 2020 2020 2020 2020 2020 2e2e  :.            ..
-00004fb0: 2e20 2020 2020 783a 2069 6e74 0a20 2020  .     x: int.   
-00004fc0: 2020 2020 2020 2020 202e 2e2e 2020 2020           ...    
-00004fd0: 2079 3a20 696e 740a 2020 2020 2020 2020   y: int.        
-00004fe0: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
-00004ff0: 2020 2020 3e3e 3e20 7061 7273 6572 203d      >>> parser =
-00005000: 2079 6170 782e 4172 6775 6d65 6e74 5061   yapx.ArgumentPa
-00005010: 7273 6572 2829 0a20 2020 2020 2020 2020  rser().         
-00005020: 2020 203e 3e3e 2070 6172 7365 722e 6164     >>> parser.ad
-00005030: 645f 6172 6775 6d65 6e74 7328 4164 644e  d_arguments(AddN
-00005040: 756d 7329 0a20 2020 2020 2020 2020 2020  ums).           
-00005050: 203e 3e3e 2070 6172 7365 6420 3d20 7061   >>> parsed = pa
-00005060: 7273 6572 2e70 6172 7365 5f61 7267 735f  rser.parse_args_
-00005070: 746f 5f6d 6f64 656c 285b 272d 7827 2c20  to_model(['-x', 
-00005080: 2731 272c 2027 2d79 272c 2027 3227 5d29  '1', '-y', '2'])
-00005090: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
-000050a0: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
-000050b0: 2028 7061 7273 6564 2e78 2c20 7061 7273   (parsed.x, pars
-000050c0: 6564 2e79 290a 2020 2020 2020 2020 2020  ed.y).          
-000050d0: 2020 2831 2c20 3229 0a0a 2020 2020 2020    (1, 2)..      
-000050e0: 2020 72ff 0000 0029 0272 f800 0000 7200    r....).r....r.
-000050f0: 0100 0029 0572 7800 0000 7250 0000 0072  ...).rx...rP...r
-00005100: 8f00 0000 72fe 0000 0072 0101 0000 7253  ....r....r....rS
-00005110: 0000 0072 5300 0000 7257 0000 00da 1370  ...rS...rW.....p
-00005120: 6172 7365 5f61 7267 735f 746f 5f6d 6f64  arse_args_to_mod
-00005130: 656c a503 0000 730c 0000 000a 1e04 0102  el....s.........
-00005140: 0102 0102 0106 fd7a 2241 7267 756d 656e  .......z"Argumen
-00005150: 7450 6172 7365 722e 7061 7273 655f 6172  tParser.parse_ar
-00005160: 6773 5f74 6f5f 6d6f 6465 6c63 0400 0000  gs_to_modelc....
-00005170: 0000 0000 0000 0000 0800 0000 0a00 0000  ................
-00005180: 4300 0000 73aa 0000 0074 007c 0183 017d  C...s....t.|...}
-00005190: 047c 0273 107c 04a0 017c 006a 02a1 017d  .|.s.|...|.j...}
-000051a0: 027c 0273 1074 0382 017c 006a 047c 047c  .|.s.t...|.j.|.|
-000051b0: 0264 018d 027d 0574 0572 4e7c 0373 4e7a  .d...}.t.rN|.sNz
-000051c0: 0d74 0074 067c 0283 0164 0569 007c 05a4  .t.t.|...d.i.|..
-000051d0: 018e 0183 017d 0557 006e 2504 0074 0779  .....}.W.n%..t.y
-000051e0: 4d01 007d 0601 007a 1964 0264 02a0 0864  M..}...z.d.d...d
-000051f0: 0364 0484 007c 06a0 09a1 0044 0083 01a1  .d...|.....D....
-00005200: 0117 007d 077c 00a0 0a7c 07a1 0101 0057  ...}.|...|.....W
-00005210: 0059 0064 007d 067e 066e 0564 007d 067e  .Y.d.}.~.n.d.}.~
-00005220: 0677 0177 007c 0264 0569 007c 05a4 018e  .w.w.|.d.i.|....
-00005230: 0153 0029 064e a902 da09 6172 6773 5f64  .S.).N....args_d
-00005240: 6963 7472 8f00 0000 727d 0000 0063 0100  ictr....r}...c..
-00005250: 0000 0000 0000 0000 0000 0200 0000 0600  ................
-00005260: 0000 7300 0000 732e 0000 0081 007c 005d  ..s...s......|.]
-00005270: 127d 0164 007c 0164 0119 0064 0219 009b  .}.d.|.d...d....
-00005280: 0064 037c 0164 0419 009b 0064 059d 0556  .d.|.d.....d...V
-00005290: 0001 0071 0264 0653 0029 077a 1845 7272  ...q.d.S.).z.Err
-000052a0: 6f72 2070 6172 7369 6e67 2061 7267 756d  or parsing argum
-000052b0: 656e 7420 60da 036c 6f63 7201 0000 007a  ent `..locr....z
-000052c0: 0360 3b20 da03 6d73 6772 ac00 0000 4e72  .`; ..msgr....Nr
-000052d0: 5300 0000 7254 0000 0072 5300 0000 7253  S...rT...rS...rS
-000052e0: 0000 0072 5700 0000 da09 3c67 656e 6578  ...rW.....<genex
-000052f0: 7072 3ee3 0300 0073 0a00 0000 0280 0400  pr>....s........
-00005300: 0202 1cff 0aff 7a36 4172 6775 6d65 6e74  ......z6Argument
-00005310: 5061 7273 6572 2e5f 7061 7273 655f 6172  Parser._parse_ar
-00005320: 6773 5f74 6f5f 6d6f 6465 6c2e 3c6c 6f63  gs_to_model.<loc
-00005330: 616c 733e 2e3c 6765 6e65 7870 723e 7253  als>.<genexpr>rS
-00005340: 0000 0029 0b72 f500 0000 72aa 0000 0072  ...).r....r....r
-00005350: 4600 0000 7226 0000 00da 165f 756e 696f  F...r&....._unio
-00005360: 6e5f 6172 6773 5f77 6974 685f 6d6f 6465  n_args_with_mode
-00005370: 6c72 3500 0000 7233 0000 0072 2e00 0000  lr5...r3...r....
-00005380: 72da 0000 00da 0665 7272 6f72 7372 8200  r......errorsr..
-00005390: 0000 2908 7278 0000 0072 5000 0000 728f  ..).rx...rP...r.
-000053a0: 0000 0072 fe00 0000 7201 0100 005a 0a61  ...r....r....Z.a
-000053b0: 7267 735f 756e 696f 6e72 fb00 0000 72dd  rgs_unionr....r.
-000053c0: 0000 0072 5300 0000 7253 0000 0072 5700  ...rS...rS...rW.
-000053d0: 0000 7200 0100 00ca 0300 0073 2c00 0000  ..r........s,...
-000053e0: 0806 0402 0c01 0401 0401 0402 0201 0201  ................
-000053f0: 06fe 0805 0202 0201 1001 08ff 0e03 0c01  ................
-00005400: 0602 0afe 1604 0880 02fb 0e07 7a23 4172  ............z#Ar
-00005410: 6775 6d65 6e74 5061 7273 6572 2e5f 7061  gumentParser._pa
-00005420: 7273 655f 6172 6773 5f74 6f5f 6d6f 6465  rse_args_to_mode
-00005430: 6c72 0601 0000 6302 0000 0000 0000 0000  lr....c.........
-00005440: 0000 0002 0000 0003 0000 0003 0000 0073  ...............s
-00005450: 1600 0000 8700 6601 6401 6402 8408 7c00  ......f.d.d...|.
-00005460: a000 a100 4400 8301 5300 2903 4e63 0100  ....D...S.).Nc..
-00005470: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00005480: 0000 1300 0000 7320 0000 0069 007c 005d  ......s ...i.|.]
-00005490: 0c5c 027d 017d 027c 0188 006a 0076 0072  .\.}.}.|...j.v.r
-000054a0: 027c 017c 0293 0271 0253 0072 5300 0000  .|.|...q.S.rS...
-000054b0: 72a1 0000 00a9 0372 5500 0000 72df 0000  r......rU...r...
-000054c0: 00da 0176 7294 0000 0072 5300 0000 7257  ...vr....rS...rW
-000054d0: 0000 00da 0a3c 6469 6374 636f 6d70 3ef0  .....<dictcomp>.
-000054e0: 0300 0072 6100 0000 7a39 4172 6775 6d65  ...ra...z9Argume
-000054f0: 6e74 5061 7273 6572 2e5f 756e 696f 6e5f  ntParser._union_
-00005500: 6172 6773 5f77 6974 685f 6d6f 6465 6c2e  args_with_model.
-00005510: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
-00005520: 6d70 3e29 0172 8d00 0000 7205 0100 0072  mp>).r....r....r
-00005530: 5300 0000 7294 0000 0072 5700 0000 720a  S...r....rW...r.
-00005540: 0100 00eb 0300 0073 0200 0000 1605 7a25  .......s......z%
-00005550: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
-00005560: 756e 696f 6e5f 6172 6773 5f77 6974 685f  union_args_with_
-00005570: 6d6f 6465 6c63 0200 0000 0000 0000 0000  modelc..........
-00005580: 0000 0600 0000 0400 0000 4300 0000 7380  ..........C...s.
-00005590: 0000 0064 007d 027c 016a 0072 157c 016a  ...d.}.|.j.r.|.j
-000055a0: 00a0 017c 016a 0264 0117 00a1 0173 157c  ...|.j.d.....s.|
-000055b0: 016a 00a0 03a1 00a0 04a1 007d 027c 0273  .j.........}.|.s
-000055c0: 1964 0053 0064 027d 0374 057c 0283 0144  .d.S.d.}.t.|...D
-000055d0: 005d 0c5c 027d 047d 057c 05a0 03a1 0073  .].\.}.}.|.....s
-000055e0: 2b7c 047d 0301 006e 0171 1f7c 0364 026b  +|.}...n.q.|.d.k
-000055f0: 0472 367c 0264 007c 0385 0219 007d 0264  .r6|.d.|.....}.d
-00005600: 03a0 0664 0464 0584 007c 0244 0083 01a1  ...d.d...|.D....
-00005610: 0153 0029 064e fa01 2872 0100 0000 727d  .S.).N..(r....r}
-00005620: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00005630: 0200 0000 0300 0000 7300 0000 7318 0000  ........s...s...
-00005640: 0081 007c 005d 077d 017c 01a0 00a1 0056  ...|.].}.|.....V
-00005650: 0001 0071 0264 0053 0072 5c00 0000 2901  ...q.d.S.r\...).
-00005660: da05 7374 7269 7072 5400 0000 7253 0000  ..striprT...rS..
-00005670: 0072 5300 0000 7257 0000 0072 0901 0000  .rS...rW...r....
-00005680: 0a04 0000 7304 0000 0002 8016 007a 4141  ....s........zAA
-00005690: 7267 756d 656e 7450 6172 7365 722e 5f67  rgumentParser._g
-000056a0: 6574 5f64 6573 6372 6970 7469 6f6e 5f66  et_description_f
-000056b0: 726f 6d5f 646f 6373 7472 696e 672e 3c6c  rom_docstring.<l
-000056c0: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
-000056d0: 2907 da07 5f5f 646f 635f 5f72 6000 0000  )...__doc__r`...
-000056e0: 7295 0000 0072 1001 0000 7299 0000 00da  r....r....r.....
-000056f0: 0965 6e75 6d65 7261 7465 72da 0000 0029  .enumerater....)
-00005700: 0672 a700 0000 728f 0000 005a 1164 6573  .r....r....Z.des
-00005710: 6372 6970 7469 6f6e 5f6c 696e 6573 5a12  cription_linesZ.
-00005720: 7465 7874 5f62 6c6f 636b 5f65 6e64 735f  text_block_ends_
-00005730: 6174 da01 69da 046c 696e 6572 5300 0000  at..i..linerS...
-00005740: 7253 0000 0072 5700 0000 7298 0000 00f2  rS...rW...r.....
-00005750: 0300 0073 2000 0000 0405 0c02 0801 04ff  ...s ...........
-00005760: 0e03 0402 0401 0402 1001 0801 0401 0401  ................
-00005770: 02fe 0804 0c01 1402 7a2e 4172 6775 6d65  ........z.Argume
-00005780: 6e74 5061 7273 6572 2e5f 6765 745f 6465  ntParser._get_de
-00005790: 7363 7269 7074 696f 6e5f 6672 6f6d 5f64  scription_from_d
-000057a0: 6f63 7374 7269 6e67 6303 0000 0000 0000  ocstringc.......
-000057b0: 0000 0000 0004 0000 0003 0000 0043 0000  .............C..
-000057c0: 0073 1c00 0000 7c00 a000 7c02 a101 7d03  .s....|...|...}.
-000057d0: 7c03 720c 7c03 7c01 5f01 6400 5300 6400  |.r.|.|._.d.S.d.
-000057e0: 5300 725c 0000 0029 0272 9800 0000 7249  S.r\...).r....rI
-000057f0: 0000 0029 0472 a700 0000 7266 0000 0072  ...).r....rf...r
-00005800: 8f00 0000 7249 0000 0072 5300 0000 7253  ....rI...rS...rS
-00005810: 0000 0072 5700 0000 da1f 5f73 6574 5f64  ...rW....._set_d
-00005820: 6573 6372 6970 7469 6f6e 5f66 726f 6d5f  escription_from_
-00005830: 646f 6373 7472 696e 670c 0400 0073 0800  docstring....s..
-00005840: 0000 0a06 0402 0a01 04ff 7a2e 4172 6775  ..........z.Argu
-00005850: 6d65 6e74 5061 7273 6572 2e5f 7365 745f  mentParser._set_
-00005860: 6465 7363 7269 7074 696f 6e5f 6672 6f6d  description_from
-00005870: 5f64 6f63 7374 7269 6e67 da0b 6c69 6e6b  _docstring..link
-00005880: 6564 5f66 756e 63da 0b72 656c 6179 5f76  ed_func..relay_v
-00005890: 616c 7565 6307 0000 0000 0000 0000 0000  aluec...........
-000058a0: 0017 0000 0007 0000 0003 0000 0073 e601  .............s..
-000058b0: 0000 6700 7d07 6900 7d08 6401 7d09 6401  ..g.}.i.}.d.}.d.
-000058c0: 7d0a 6401 7d0b 6401 7d0c 6401 7d0d 7400  }.d.}.d.}.d.}.t.
-000058d0: 7c02 8301 6a01 a002 a100 4400 5d43 7d0e  |...j.....D.]C}.
-000058e0: 7403 7c0e 8301 a004 6402 a101 7221 6403  t.|.....d...r!d.
-000058f0: 7d0c 7115 7403 7c0e 8301 a004 6404 a101  }.q.t.|.....d...
-00005900: 722b 6403 7d0a 7115 7c0e 6a05 6405 6b02  r+d.}.q.|.j.d.k.
-00005910: 7233 6403 7d0b 7115 7c0e 6a05 6406 6b02  r3d.}.q.|.j.d.k.
-00005920: 723b 6403 7d0d 7115 7c0e 6a05 6407 6b02  r;d.}.q.|.j.d.k.
-00005930: 7245 7c03 7c08 6407 3c00 7115 7c0e 6a05  rE|.|.d.<.q.|.j.
-00005940: 6408 6b02 724f 7c06 7c08 6408 3c00 7115  d.k.rO|.|.d.<.q.
-00005950: 7c0e 6a05 6409 6b02 7258 6403 7c08 6409  |.j.d.k.rXd.|.d.
-00005960: 3c00 7115 7c0a 7060 7c0c 7060 7c0b 7060  <.q.|.p`|.p`|.p`
-00005970: 7c0d 7d09 7c09 7373 7c05 7273 7406 640a  |.}.|.ss|.rst.d.
-00005980: 640b 8400 7400 7c05 8301 6a01 a002 a100  d...t.|...j.....
-00005990: 4400 8301 8301 7d09 7c04 7379 7407 7c02  D.....}.|.syt.|.
-000059a0: 8301 7d04 7c09 72e1 7c01 6a08 7c03 7c04  ..}.|.r.|.j.|.|.
-000059b0: 640c 8d02 5c02 7d0f 7d10 7c0c 7388 7c0d  d...\.}.}.|.s.|.
-000059c0: 72d6 6900 8900 7c00 8300 7d11 7c10 4400  r.i...|...}.|.D.
-000059d0: 5d24 7d12 7c12 a004 640d a101 72b3 7c12  ]$}.|...d...r.|.
-000059e0: 6a09 640e 640f 6410 8d02 6411 1900 7d13  j.d.d.d...d...}.
-000059f0: 7c13 a00a 640d a101 7d14 7c14 72b3 7c11  |...d...}.|.r.|.
-00005a00: 6a0b 7c13 6412 6400 6401 6413 8d04 0100  j.|.d.d.d.d.....
-00005a10: 7c13 8800 7c14 3c00 718f 7c11 6a0c 7c10  |...|.<.q.|.j.|.
-00005a20: 6414 8d01 5c02 7d15 7d10 8700 6601 6415  d...\.}.}...f.d.
-00005a30: 6416 8408 740d 7c15 8301 a00e a100 4400  d...t.|.......D.
-00005a40: 8301 7d16 7c0c 72d0 7c08 a00f 7c16 a101  ..}.|.r.|...|...
-00005a50: 0100 7c0d 72d6 7c16 7c08 6406 3c00 7c0a  ..|.r.|.|.d.<.|.
-00005a60: 72da 7c10 7d07 7c0b 72e0 7c10 7c08 6405  r.|.}.|.r.|.|.d.
-00005a70: 3c00 6e07 7c01 6a10 7c03 7c04 640c 8d02  <.n.|.j.|.|.d...
-00005a80: 7d0f 7c02 7c07 6900 740d 7c0f 8301 a401  }.|.|.i.t.|.....
-00005a90: 7c08 a401 8e01 5300 2917 4e46 7a02 2a2a  |.....S.).NFz.**
-00005aa0: 54da 012a da0b 5f65 7874 7261 5f61 7267  T..*.._extra_arg
-00005ab0: 73da 0d5f 6578 7472 615f 6b77 6172 6773  s.._extra_kwargs
-00005ac0: 5a09 5f61 6c6c 5f61 7267 735a 0c5f 7265  Z._all_argsZ._re
-00005ad0: 6c61 795f 7661 6c75 655a 105f 6361 6c6c  lay_valueZ._call
-00005ae0: 6564 5f66 726f 6d5f 636c 6963 0100 0000  ed_from_clic....
-00005af0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00005b00: 7300 0000 7328 0000 0081 007c 005d 0f7d  s...s(.....|.].}
-00005b10: 0174 007c 0183 01a0 0164 00a1 0170 0f7c  .t.|.....d...p.|
-00005b20: 016a 0264 0176 0056 0001 0071 0264 0253  .j.d.v.V...q.d.S
-00005b30: 0029 0372 1801 0000 2902 7219 0100 0072  .).r....).r....r
-00005b40: 1a01 0000 4e29 0372 6e00 0000 7260 0000  ....N).rn...r`..
-00005b50: 0072 9200 0000 2902 7255 0000 00da 0170  .r....).rU.....p
-00005b60: 7253 0000 0072 5300 0000 7257 0000 0072  rS...rS...rW...r
-00005b70: 0901 0000 4104 0000 730a 0000 0002 8004  ....A...s.......
-00005b80: 0002 0216 ff0a ff7a 2b41 7267 756d 656e  .......z+Argumen
-00005b90: 7450 6172 7365 722e 5f72 756e 5f66 756e  tParser._run_fun
-00005ba0: 632e 3c6c 6f63 616c 733e 2e3c 6765 6e65  c.<locals>.<gene
-00005bb0: 7870 723e 2902 7250 0000 0072 8f00 0000  xpr>).rP...r....
-00005bc0: 7265 0000 0072 5b00 0000 7217 0000 0072  re...r[...r....r
-00005bd0: ad00 0000 7201 0000 0072 b900 0000 2903  ....r....r....).
-00005be0: 72b8 0000 0072 6300 0000 72b7 0000 0029  r....rc...r....)
-00005bf0: 0172 5000 0000 6301 0000 0000 0000 0000  .rP...c.........
-00005c00: 0000 0003 0000 0004 0000 0013 0000 0073  ...............s
-00005c10: 1a00 0000 6900 7c00 5d09 5c02 7d01 7d02  ....i.|.].\.}.}.
-00005c20: 8800 7c01 1900 7c02 9302 7102 5300 7253  ..|...|...q.S.rS
-00005c30: 0000 0072 5300 0000 720c 0100 00a9 015a  ...rS...r......Z
-00005c40: 1075 6e6b 6e6f 776e 5f6e 616d 655f 6d61  .unknown_name_ma
-00005c50: 7072 5300 0000 7257 0000 0072 0e01 0000  prS...rW...r....
-00005c60: 6504 0000 7306 0000 0006 000e 0106 ff7a  e...s..........z
-00005c70: 2c41 7267 756d 656e 7450 6172 7365 722e  ,ArgumentParser.
-00005c80: 5f72 756e 5f66 756e 632e 3c6c 6f63 616c  _run_func.<local
-00005c90: 733e 2e3c 6469 6374 636f 6d70 3e29 1172  s>.<dictcomp>).r
-00005ca0: 0900 0000 da0a 7061 7261 6d65 7465 7273  ......parameters
-00005cb0: 72be 0000 0072 6e00 0000 7260 0000 0072  r....rn...r`...r
-00005cc0: 9200 0000 da03 616e 7972 2500 0000 7203  ......anyr%...r.
-00005cd0: 0100 00da 0573 706c 6974 da06 6c73 7472  .....split..lstr
-00005ce0: 6970 726f 0000 0072 fc00 0000 72f5 0000  ipro...r....r...
-00005cf0: 0072 8d00 0000 da06 7570 6461 7465 7204  .r......updater.
-00005d00: 0100 0029 1772 a700 0000 7266 0000 0072  ...).r....rf...r
-00005d10: 9c00 0000 7250 0000 0072 8f00 0000 7216  ....rP...r....r.
-00005d20: 0100 0072 1701 0000 5a09 6675 6e63 5f61  ...r....Z.func_a
-00005d30: 7267 735a 0b66 756e 635f 6b77 6172 6773  rgsZ.func_kwargs
-00005d40: 5a0d 6578 7472 615f 6172 6773 5f6f 6b5a  Z.extra_args_okZ
-00005d50: 0c61 6363 6570 7473 5f61 7267 735a 1261  .accepts_argsZ.a
-00005d60: 6363 6570 7473 5f65 7874 7261 5f61 7267  ccepts_extra_arg
-00005d70: 735a 0e61 6363 6570 7473 5f6b 7761 7267  sZ.accepts_kwarg
-00005d80: 735a 1461 6363 6570 7473 5f65 7874 7261  sZ.accepts_extra
-00005d90: 5f6b 7761 7267 7372 1b01 0000 5a0a 6d6f  _kwargsr....Z.mo
-00005da0: 6465 6c5f 696e 7374 7202 0100 005a 0e75  del_instr....Z.u
-00005db0: 6e6b 6e6f 776e 5f70 6172 7365 7272 5600  nknown_parserrV.
-00005dc0: 0000 5a06 785f 666c 6167 5a0b 785f 666c  ..Z.x_flagZ.x_fl
-00005dd0: 6167 5f62 6172 655a 0e70 6172 7365 645f  ag_bareZ.parsed_
-00005de0: 756e 6b6e 6f77 6e5a 0c65 7874 7261 5f6b  unknownZ.extra_k
-00005df0: 7761 7267 7372 5300 0000 721c 0100 0072  wargsrS...r....r
-00005e00: 5700 0000 da09 5f72 756e 5f66 756e 6317  W....._run_func.
-00005e10: 0400 0073 9000 0000 040a 0401 0402 0402  ...s............
-00005e20: 0401 0402 0401 1202 0e01 0601 0e01 0601  ................
-00005e30: 0a01 0601 0a01 0601 0a01 0a01 0a01 0a01  ................
-00005e40: 0a01 0801 0280 0e03 02ff 0804 0801 0c02  ................
-00005e50: 08fe 0405 0801 0403 0402 0201 0201 0afe  ................
-00005e60: 0805 0401 0601 0801 0a01 1201 0a01 0401  ................
-00005e70: 0401 0201 0201 0201 0201 06fc 0806 0280  ................
-00005e80: 0402 0201 0aff 0a04 0a01 06ff 0403 0a01  ................
-00005e90: 0401 0801 0402 0401 0402 0801 0280 0403  ................
-00005ea0: 0201 0201 06fe 1605 7a18 4172 6775 6d65  ........z.Argume
-00005eb0: 6e74 5061 7273 6572 2e5f 7275 6e5f 6675  ntParser._run_fu
-00005ec0: 6e63 da07 636f 6d6d 616e 64da 0b73 7562  nc..command..sub
-00005ed0: 636f 6d6d 616e 6473 da11 6e61 6d65 645f  commands..named_
-00005ee0: 7375 6263 6f6d 6d61 6e64 7363 0400 0000  subcommandsc....
-00005ef0: 0000 0000 0000 0000 0900 0000 0b00 0000  ................
-00005f00: 4b00 0000 73d2 0000 007c 0064 0369 007c  K...s....|.d.i.|
-00005f10: 04a4 018e 017d 057c 0172 2e74 007c 0183  .....}.|.r.t.|..
-00005f20: 017d 067c 006a 017c 057c 0664 018d 0201  .}.|.j.|.|.d....
-00005f30: 007c 05a0 027c 06a1 0101 007c 056a 0364  .|...|.....|.j.d
-00005f40: 0369 007c 006a 047c 017c 006a 057c 067c  .i.|.j.|.|.j.|.|
-00005f50: 006a 067c 017c 006a 077c 0669 04a4 018e  .j.|.|.j.|.i....
-00005f60: 0101 006e 147c 056a 0364 0369 007c 006a  ...n.|.j.d.i.|.j
-00005f70: 0564 007c 006a 0464 007c 006a 0764 007c  .d.|.j.d.|.j.d.|
-00005f80: 006a 0664 0069 04a4 018e 0101 007c 0272  .j.d.i.......|.r
-00005f90: 5574 087c 0283 0172 4b7c 0267 017d 027c  Ut.|...rK|.g.}.|
-00005fa0: 0244 005d 077d 077c 05a0 097c 07a1 0101  .D.].}.|...|....
-00005fb0: 0071 4d7c 0372 677c 03a0 0aa1 0044 005d  .qM|.rg|.....D.]
-00005fc0: 0b5c 027d 087d 077c 056a 097c 077c 0864  .\.}.}.|.j.|.|.d
-00005fd0: 028d 0201 0071 5b7c 0553 0029 044e 2902  .....q[|.S.).N).
-00005fe0: 7266 0000 0072 8f00 0000 72b1 0000 0072  rf...r....r....r
-00005ff0: 5300 0000 290b 7225 0000 0072 1501 0000  S...).r%...r....
-00006000: 7291 0000 0072 9d00 0000 7242 0000 0072  r....r....rB...r
-00006010: 4300 0000 7245 0000 0072 4600 0000 da08  C...rE...rF.....
-00006020: 6361 6c6c 6162 6c65 729e 0000 0072 8d00  callabler....r..
-00006030: 0000 2909 72a7 0000 0072 2301 0000 7224  ..).r....r#...r$
-00006040: 0100 0072 2501 0000 7251 0000 0072 6600  ...r%...rQ...rf.
-00006050: 0000 5a0e 726f 6f74 5f61 7267 5f6d 6f64  ..Z.root_arg_mod
-00006060: 656c 7256 0000 0072 9200 0000 7253 0000  elrV...r....rS..
-00006070: 0072 5300 0000 7257 0000 00da 0d5f 6275  .rS...rW....._bu
-00006080: 696c 645f 7061 7273 6572 7b04 0000 733e  ild_parser{...s>
-00006090: 0000 000e 0804 0208 0104 0102 0102 0106  ................
-000060a0: fe0a 0408 0106 0206 0106 0106 0102 fc08  ................
-000060b0: ff08 0906 0206 0106 0106 0102 fc06 ff04  ................
-000060c0: 0908 0106 0108 010c 0104 0210 0110 0104  ................
-000060d0: 027a 1c41 7267 756d 656e 7450 6172 7365  .z.ArgumentParse
-000060e0: 722e 5f62 7569 6c64 5f70 6172 7365 7229  r._build_parser)
-000060f0: 0272 5000 0000 da0c 6465 6661 756c 745f  .rP.....default_
-00006100: 6172 6773 da0b 7061 7273 6572 5f61 7267  args..parser_arg
-00006110: 7372 2801 0000 da0d 7061 7273 6572 5f6b  sr(.....parser_k
-00006120: 7761 7267 7363 0100 0000 0000 0000 0200  wargsc..........
-00006130: 0000 1100 0000 0900 0000 4f00 0000 7338  ..........O...s8
-00006140: 0100 007c 006a 007c 0369 007c 04a4 018e  ...|.j.|.i.|....
-00006150: 017d 057c 0164 0175 0072 1374 016a 0264  .}.|.d.u.r.t.j.d
-00006160: 0264 0185 0219 007d 017c 0173 197c 0272  .d.....}.|.s.|.r
-00006170: 197c 027d 017c 05a0 037c 01a1 015c 027d  .|.}.|...|...\.}
-00006180: 067d 0774 047c 0683 017d 087c 08a0 057c  .}.t.|...}.|...|
-00006190: 006a 06a1 017d 097c 08a0 057c 006a 07a1  .j...}.|...|.j..
-000061a0: 017d 0a7c 08a0 057c 006a 08a1 017d 0b7c  .}.|...|.j...}.|
-000061b0: 08a0 057c 006a 09a1 017d 0c7c 08a0 057c  ...|.j...}.|...|
-000061c0: 006a 0aa1 017d 0d64 017d 0e64 017d 0f7c  .j...}.d.}.d.}.|
-000061d0: 0972 527c 006a 0b7c 057c 097c 0a7c 0c7c  .rR|.j.|.|.|.|.|
-000061e0: 0164 038d 057d 0f74 0c7c 0f74 0d83 0272  .d...}.t.|.t...r
-000061f0: 697a 0674 0e7c 0f83 017d 0e57 006e 0d04  iz.t.|...}.W.n..
-00006200: 0074 0f79 6801 0001 0001 007c 0f7d 0e59  .t.yh......|.}.Y
-00006210: 006e 0377 007c 0f7d 0e7a 207c 0b72 7b7c  .n.w.|.}.z |.r{|
-00006220: 0c72 7b7c 006a 0b7c 057c 0c7c 0d7c 017c  .r{|.j.|.|.|.|.|
-00006230: 097c 0e64 048d 067d 0e57 0074 0c7c 0f74  .|.d...}.W.t.|.t
-00006240: 0d83 0272 8a7c 0f44 005d 067d 107c 0c73  ...r.|.D.].}.|.s
-00006250: 897c 107d 0e71 837c 0e53 0074 0c7c 0f74  .|.}.q.|.S.t.|.t
-00006260: 0d83 0272 9a7c 0f44 005d 077d 107c 0c73  ...r.|.D.].}.|.s
-00006270: 997c 107d 0e71 9377 0077 0029 0561 2d03  .|.}.q.w.w.).a-.
-00006280: 0000 5573 6520 6769 7665 6e20 6675 6e63  ..Use given func
-00006290: 7469 6f6e 7320 746f 2063 6f6e 7374 7275  tions to constru
-000062a0: 6374 2061 2043 4c49 2c20 7061 7273 6520  ct a CLI, parse 
-000062b0: 7468 6520 6172 6773 2c20 616e 6420 696e  the args, and in
-000062c0: 766f 6b65 2074 6865 2061 7070 726f 7072  voke the appropr
-000062d0: 6961 7465 2063 6f6d 6d61 6e64 2e0a 0a20  iate command... 
-000062e0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-000062f0: 2020 2020 2020 2020 202a 7061 7273 6572           *parser
-00006300: 5f61 7267 733a 0a20 2020 2020 2020 2020  _args:.         
-00006310: 2020 2061 7267 733a 0a20 2020 2020 2020     args:.       
-00006320: 2020 2020 2064 6566 6175 6c74 5f61 7267       default_arg
-00006330: 733a 0a20 2020 2020 2020 2020 2020 202a  s:.            *
-00006340: 2a70 6172 7365 725f 6b77 6172 6773 3a0a  *parser_kwargs:.
-00006350: 0a0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
-00006360: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00006370: 3e3e 3e20 696d 706f 7274 2079 6170 780a  >>> import yapx.
-00006380: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
-00006390: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-000063a0: 6465 6620 7072 696e 745f 6e75 6d73 282a  def print_nums(*
-000063b0: 6172 6773 293a 0a20 2020 2020 2020 2020  args):.         
-000063c0: 2020 202e 2e2e 2020 2020 2070 7269 6e74     ...     print
-000063d0: 2827 4172 6773 3a20 272c 202a 6172 6773  ('Args: ', *args
-000063e0: 290a 2020 2020 2020 2020 2020 2020 2e2e  ).            ..
-000063f0: 2e0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
-00006400: 3e20 6465 6620 6669 6e64 5f65 7665 6e73  > def find_evens
-00006410: 282a 6172 6773 293a 0a20 2020 2020 2020  (*args):.       
-00006420: 2020 2020 202e 2e2e 2020 2020 2072 6574       ...     ret
-00006430: 7572 6e20 5b78 2066 6f72 2078 2069 6e20  urn [x for x in 
-00006440: 6172 6773 2069 6620 696e 7428 7829 2025  args if int(x) %
-00006450: 2032 203d 3d20 305d 0a20 2020 2020 2020   2 == 0].       
-00006460: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
-00006470: 2020 2020 203e 3e3e 2064 6566 2066 696e       >>> def fin
-00006480: 645f 6f64 6473 282a 6172 6773 293a 0a20  d_odds(*args):. 
-00006490: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
-000064a0: 2020 2072 6574 7572 6e20 5b78 2066 6f72     return [x for
-000064b0: 2078 2069 6e20 6172 6773 2069 6620 696e   x in args if in
-000064c0: 7428 7829 2025 2032 2021 3d20 305d 0a20  t(x) % 2 != 0]. 
-000064d0: 2020 2020 2020 2020 2020 202e 2e2e 0a20             .... 
-000064e0: 2020 2020 2020 2020 2020 203e 3e3e 2063             >>> c
-000064f0: 6c69 5f61 7267 7320 3d20 5b27 6669 6e64  li_args = ['find
-00006500: 2d6f 6464 7327 2c20 2731 272c 2027 3227  -odds', '1', '2'
-00006510: 2c20 2733 272c 2027 3427 2c20 2735 275d  , '3', '4', '5']
-00006520: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
-00006530: 2079 6170 782e 7275 6e28 7072 696e 745f   yapx.run(print_
-00006540: 6e75 6d73 2c20 5b66 696e 645f 6576 656e  nums, [find_even
-00006550: 732c 2066 696e 645f 6f64 6473 5d2c 2061  s, find_odds], a
-00006560: 7267 733d 636c 695f 6172 6773 290a 2020  rgs=cli_args).  
-00006570: 2020 2020 2020 2020 2020 4172 6773 3a20            Args: 
-00006580: 2031 2032 2033 2034 2035 0a20 2020 2020   1 2 3 4 5.     
-00006590: 2020 2020 2020 205b 2731 272c 2027 3327         ['1', '3'
-000065a0: 2c20 2735 275d 0a20 2020 2020 2020 204e  , '5'].        N
-000065b0: 7217 0000 0029 0572 6600 0000 729c 0000  r....).rf...r...
-000065c0: 0072 8f00 0000 7216 0100 0072 5000 0000  .r....r....rP...
-000065d0: 2906 7266 0000 0072 9c00 0000 728f 0000  ).rf...r....r...
-000065e0: 0072 5000 0000 7216 0100 0072 1701 0000  .rP...r....r....
-000065f0: 2910 7227 0100 0072 7f00 0000 da04 6172  ).r'...r......ar
-00006600: 6776 72fc 0000 0072 f500 0000 72aa 0000  gvr....r....r...
-00006610: 0072 4200 0000 7243 0000 0072 4400 0000  .rB...rC...rD...
-00006620: 7245 0000 0072 4600 0000 7222 0100 0072  rE...rF...r"...r
-00006630: 3800 0000 720a 0000 00da 046e 6578 74da  8...r......next.
-00006640: 0d53 746f 7049 7465 7261 7469 6f6e 2911  .StopIteration).
-00006650: 72a7 0000 0072 5000 0000 7228 0100 0072  r....rP...r(...r
-00006660: 2901 0000 722a 0100 0072 6600 0000 5a0a  )...r*...rf...Z.
-00006670: 6b6e 6f77 6e5f 6172 6773 7286 0000 0072  known_argsr....r
-00006680: 0101 0000 5a09 726f 6f74 5f66 756e 635a  ....Z.root_funcZ
-00006690: 1472 6f6f 745f 6675 6e63 5f61 7267 735f  .root_func_args_
-000066a0: 6d6f 6465 6c5a 0c63 6f6d 6d61 6e64 5f6e  modelZ.command_n
-000066b0: 616d 655a 0c63 6f6d 6d61 6e64 5f66 756e  ameZ.command_fun
-000066c0: 635a 1763 6f6d 6d61 6e64 5f66 756e 635f  cZ.command_func_
-000066d0: 6172 6773 5f6d 6f64 656c 7217 0100 005a  args_modelr....Z
-000066e0: 0b72 6f6f 745f 7265 7375 6c74 5a0a 6765  .root_resultZ.ge
-000066f0: 6e5f 7265 7375 6c74 7253 0000 0072 5300  n_resultrS...rS.
-00006700: 0000 7257 0000 00da 045f 7275 6eaa 0400  ..rW....._run...
-00006710: 0073 7a00 0000 1023 0802 0e01 0802 0401  .sz....#........
-00006720: 0e03 0801 0402 0401 04ff 0403 0401 04ff  ................
-00006730: 0c03 0401 0401 04ff 0403 0401 04ff 0404  ................
-00006740: 0401 0402 0401 0201 0201 0201 0201 0201  ................
-00006750: 06fb 0a08 0201 0c01 0c01 0801 02ff 0403  ................
-00006760: 0202 0801 0401 0201 0201 0201 0201 0201  ................
-00006770: 0201 06fa 0280 0a09 0801 0401 0401 0280  ................
-00006780: 0402 0afb 0801 0401 0401 0280 02fd 0201  ................
-00006790: 7a13 4172 6775 6d65 6e74 5061 7273 6572  z.ArgumentParser
-000067a0: 2e5f 7275 6e29 024e 4672 5c00 0000 2902  ._run).NFr\...).
-000067b0: 4646 2902 4e4e 2903 4e4e 4629 034e 4e4e  FF).NN).NNF).NNN
-000067c0: 293a 7295 0000 00da 0a5f 5f6d 6f64 756c  ):r......__modul
-000067d0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-000067e0: 5f72 4200 0000 726e 0000 0072 a200 0000  _rB...rn...r....
-000067f0: 7243 0000 0072 4400 0000 7245 0000 0072  rC...rD...rE...r
-00006800: 4600 0000 722d 0000 0072 0c00 0000 7210  F...r-...r....r.
-00006810: 0000 0072 0f00 0000 7213 0000 0072 d400  ...r....r....r..
-00006820: 0000 7269 0000 0072 8200 0000 720b 0000  ..ri...r....r...
-00006830: 0072 8a00 0000 7215 0000 0072 0d00 0000  .r....r....r....
-00006840: 7229 0000 0072 9100 0000 7274 0000 0072  r)...r....rt...r
-00006850: 4100 0000 729b 0000 0072 9e00 0000 da0c  A...r....r......
-00006860: 7374 6174 6963 6d65 7468 6f64 72a4 0000  staticmethodr...
-00006870: 00da 0b63 6c61 7373 6d65 7468 6f64 7222  ...classmethodr"
-00006880: 0000 0072 9000 0000 72c5 0000 0072 1200  ...r....r....r..
-00006890: 0000 72cb 0000 0072 c700 0000 72c6 0000  ..r....r....r...
-000068a0: 0072 9600 0000 72f0 0000 0072 8c00 0000  .r....r....r....
-000068b0: 7277 0000 0072 2800 0000 72f6 0000 0072  rw...r(...r....r
-000068c0: 1100 0000 72f8 0000 0072 fc00 0000 7203  ....r....r....r.
-000068d0: 0100 0072 0401 0000 7200 0100 0072 0e00  ...r....r....r..
-000068e0: 0000 720a 0100 0072 9800 0000 7215 0100  ..r....r....r...
-000068f0: 0072 2201 0000 7227 0100 0072 2e01 0000  .r"...r'...r....
-00006900: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
-00006910: 5300 0000 7253 0000 0072 7900 0000 7257  S...rS...ry...rW
-00006920: 0000 0072 4100 0000 4c00 0000 73d4 0100  ...rA...L...s...
-00006930: 000a 000c 010c 010c 010c 010c 0102 0502  ................
-00006940: 0102 0102 0102 0102 0102 0102 0102 0106  ................
-00006950: f502 0202 fe06 0302 fd06 0402 fc06 0502  ................
-00006960: fb0a 0602 fa0a 0702 f90a 0802 f80a 0902  ................
-00006970: f706 0a02 f602 0b02 f502 0c0e f40e 7102  ..............q.
-00006980: 0602 0104 fd0a 0202 fe02 0302 fd02 040e  ................
-00006990: fc02 2e16 0202 fe02 030a fd02 3404 fd16  ............4...
-000069a0: 0202 fe06 0302 fd02 0402 fc04 050a fb02  ................
-000069b0: 6304 fd0a 0202 fe06 0302 fd02 0402 fc02  c...............
-000069c0: 050a fb02 0e1c 0102 0302 0104 0202 fe16  ................
-000069d0: 0302 fd06 040c fc00 7f00 7f02 2220 0102  ............" ..
-000069e0: 0324 0102 0324 0102 0302 0402 0104 fc06  .$...$..........
-000069f0: 0202 fe02 0302 fd02 0402 fc06 050c fb14  ................
-00006a00: 3f14 1110 0a02 0b04 0202 fe02 030a fd02  ?...............
-00006a10: 3202 0104 fd0a 0202 fe08 0302 fd02 040e  2...............
-00006a20: fc02 1002 0104 fd0a 0202 fe08 0302 fd0e  ................
-00006a30: 040e fc02 0f02 0102 0104 fc0a 0202 fe0a  ................
-00006a40: 0302 fd02 0402 fc0e 050a fb02 3002 0102  ............0...
-00006a50: 0104 fc0a 0202 fe0a 0302 fd02 0402 fc02  ................
-00006a60: 050a fb02 2802 0104 fc04 0202 fe0a 0302  ....(...........
-00006a70: fd02 0402 fc02 050a fb02 2102 010a 0102  ..........!.....
-00006a80: ff06 0202 fe0a 030c fd02 0602 0116 0202  ................
-00006a90: fe06 030c fd02 1902 0104 0202 fe16 0302  ................
-00006aa0: fd02 040c fc02 0a02 0602 0102 0104 f902  ................
-00006ab0: 0202 fe0a 0302 fd06 0402 fc0a 0502 fb0e  ................
-00006ac0: 0602 fa06 0702 f902 080c f802 6302 0302  ............c...
-00006ad0: 0102 0104 fc0e 0202 fe12 0302 fd16 0402  ................
-00006ae0: fc02 0502 fb02 060c fa02 2e02 0402 0106  ................
-00006af0: fc02 0202 fe0a 0302 fd0a 0402 fc02 0502  ................
-00006b00: fb02 0614 fa72 4100 0000 294e 7274 0000  .....rA...)Nrt..
-00006b10: 00da 0f63 6f6c 6c65 6374 696f 6e73 2e61  ...collections.a
-00006b20: 6263 72cc 0000 0072 7f00 0000 7202 0000  bcr....r....r...
-00006b30: 00da 0a63 6f6e 7465 7874 6c69 6272 0300  ...contextlibr..
-00006b40: 0000 da0b 6461 7461 636c 6173 7365 7372  ....dataclassesr
-00006b50: 0400 0000 7205 0000 0072 0600 0000 da04  ....r....r......
-00006b60: 656e 756d 7207 0000 00da 0966 756e 6374  enumr......funct
-00006b70: 6f6f 6c73 7208 0000 00da 0769 6e73 7065  oolsr......inspe
-00006b80: 6374 7209 0000 00da 0574 7970 6573 720a  ctr......typesr.
-00006b90: 0000 00da 0674 7970 696e 6772 0b00 0000  .....typingr....
-00006ba0: 720c 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
-00006bb0: 0f00 0000 7210 0000 0072 1100 0000 7212  ....r....r....r.
-00006bc0: 0000 0072 1300 0000 7214 0000 0072 1500  ...r....r....r..
-00006bd0: 0000 5a0d 706b 675f 7265 736f 7572 6365  ..Z.pkg_resource
-00006be0: 7372 1600 0000 da07 6163 7469 6f6e 7372  sr......actionsr
-00006bf0: 1800 0000 7219 0000 0072 1a00 0000 721b  ....r....r....r.
-00006c00: 0000 0072 1c00 0000 721d 0000 0072 1e00  ...r....r....r..
-00006c10: 0000 721f 0000 0072 2000 0000 da03 6172  ..r....r .....ar
-00006c20: 6772 2100 0000 7222 0000 0072 2300 0000  gr!...r"...r#...
-00006c30: 7224 0000 0072 2500 0000 da0a 6578 6365  r$...r%.....exce
-00006c40: 7074 696f 6e73 7226 0000 0072 2700 0000  ptionsr&...r'...
-00006c50: 72bd 0000 0072 2800 0000 7229 0000 0072  r....r(...r)...r
-00006c60: 2a00 0000 722b 0000 00da 0575 7469 6c73  *...r+.....utils
-00006c70: 722c 0000 0072 2d00 0000 722e 0000 0072  r,...r-...r....r
-00006c80: 2f00 0000 7230 0000 0072 3100 0000 7232  /...r0...r1...r2
-00006c90: 0000 0072 3300 0000 7234 0000 0072 3500  ...r3...r4...r5.
-00006ca0: 0000 7236 0000 0072 3700 0000 7238 0000  ..r6...r7...r8..
-00006cb0: 0072 3900 0000 72c4 0000 0072 3c00 0000  .r9...r....r<...
-00006cc0: 5a11 7479 7069 6e67 5f65 7874 656e 7369  Z.typing_extensi
-00006cd0: 6f6e 7372 3f00 0000 7240 0000 0072 4100  onsr?...r@...rA.
-00006ce0: 0000 7253 0000 0072 5300 0000 7253 0000  ..rS...rS...rS..
-00006cf0: 0072 5700 0000 da08 3c6d 6f64 756c 653e  .rW.....<module>
-00006d00: 0100 0000 7332 0000 0008 0008 0108 010c  ....s2..........
-00006d10: 010c 0114 010c 010c 010c 010c 0134 010c  .............4..
-00006d20: 0e2c 021c 0b10 070c 0114 0140 010a 110e  .,.........@....
-00006d30: 010c 020a 020c 0108 0216 03              ...........
+00002e70: 347c 0a83 027c 016a 357c 096a 363c 007c  4|...|.j5|.j6<.|
+00002e80: 096a 3790 0172 817c 096a 3864 0075 0090  .j7..r.|.j8d.u..
+00002e90: 0172 817c 096a 1d90 0172 7e64 117c 095f  .r.|.j...r~d.|._
+00002ea0: 386e 0364 127c 095f 3874 0b7d 0a6e 0b74  8n.d.|._8t.}.n.t
+00002eb0: 247c 0a74 3283 0290 0172 8f74 067c 0a83  $|.t2....r.t.|..
+00002ec0: 017c 095f 237c 0a7c 095f 097c 09a0 39a1  .|._#|.|._.|..9.
+00002ed0: 007d 0e7c 0e64 133d 007c 0ea0 3a64 14a1  .}.|.d.=.|..:d..
+00002ee0: 017d 0f7c 0f90 0173 a367 006e 0664 1564  .}.|...s.g.n.d.d
+00002ef0: 0584 007c 0f44 0083 017d 107c 0e64 1619  ...|.D...}.|.d..
+00002f00: 0090 0173 c67c 0ea0 3b64 17a1 0190 0173  ...s.|..;d.....s
+00002f10: c67c 1090 0173 c264 187c 0e64 1919 00a0  .|...s.d.|.d....
+00002f20: 3ca1 009b 0064 1a9d 036e 0164 1b7c 0e64  <....d...n.d.|.d
+00002f30: 163c 007c 0e64 1c19 007d 117c 1090 0173  .<.|.d...}.|...s
+00002f40: e77c 0e64 1c3d 007c 1190 0173 df7c 0ea0  .|.d.=.|...s.|..
+00002f50: 3b64 1da1 0164 0075 0090 0172 df64 1e7c  ;d...d.u...r.d.|
+00002f60: 0e64 1d3c 0074 3374 347c 0a83 027c 0e64  .d.<.t3t4|...|.d
+00002f70: 1f3c 006e 4c7c 096a 0974 3d75 0090 0272  .<.nL|.j.t=u...r
+00002f80: 1274 157c 0188 0083 0290 0172 fc74 3374  .t.|.......r.t3t
+00002f90: 347c 0a83 027c 016a 357c 096a 363c 0064  4|...|.j5|.j6<.d
+00002fa0: 2044 005d 097d 127c 0ea0 3a7c 1264 00a1   D.].}.|..:|.d..
+00002fb0: 0201 0090 0171 fe7c 0e64 2119 0090 0273  .....q.|.d!....s
+00002fc0: 1174 3e7c 0e64 213c 006e 217c 096a 3864  .t>|.d!<.n!|.j8d
+00002fd0: 0e6b 0390 0272 2074 3374 347c 0a83 027c  .k...r t3t4|...|
+00002fe0: 0e64 1f3c 006e 137c 0a74 3f75 0090 0272  .d.<.n.|.t?u...r
+00002ff0: 2a74 407c 0e64 213c 006e 097c 0a74 0b75  *t@|.d!<.n.|.t.u
+00003000: 0090 0272 3374 417c 0e64 213c 007c 086a  ...r3tA|.d!<.|.j
+00003010: 1e74 1f75 0190 0273 477c 086a 2074 1f75  .t.u...sG|.j t.u
+00003020: 0190 0273 477c 0ea0 3b64 22a1 0164 0075  ...sG|..;d"..d.u
+00003030: 0190 0272 de7c 0ea0 3b64 21a1 0190 0272  ...r.|..;d!....r
+00003040: 7a74 247c 0e64 2119 0074 426a 4374 3e66  zt$|.d!..tBjCt>f
+00003050: 0283 0290 0272 7a74 0964 2364 2469 0083  .....rzt.d#d$i..
+00003060: 0383 007d 137c 0e64 2119 007c 107c 0e64  ...}.|.d!..|.|.d
+00003070: 1919 0064 258d 027c 017c 137c 0e64 2219  ...d%..|.|.|.d".
+00003080: 0064 268d 0301 0074 447c 137c 0e64 1919  .d&....tD|.|.d..
+00003090: 0083 027c 0e64 223c 006e 0f64 1f7c 0e76  ...|.d"<.n.d.|.v
+000030a0: 0090 0272 897c 0e64 1f19 007c 0e64 2219  ...r.|.d...|.d".
+000030b0: 0083 017c 0e64 223c 007c 0ea0 3b64 17a1  ...|.d"<.|..;d..
+000030c0: 0190 0272 de7c 0e64 2219 007d 1474 0a7c  ...r.|.d"..}.t.|
+000030d0: 1474 0b83 0290 0273 a174 0a7c 1474 256a  .t.....s.t.|.t%j
+000030e0: 266a 2a83 0290 0273 a47c 1467 017d 147c  &j*....s.|.g.}.|
+000030f0: 1444 005d 377d 0b7c 0b7c 0e64 1719 0076  .D.]7}.|.|.d...v
+00003100: 0190 0272 dc74 0a7c 0b74 3283 0290 0272  ...r.t.|.t2....r
+00003110: bd7c 0b6a 1c7c 0e64 1719 0076 0190 0272  .|.j.|.d...v...r
+00003120: dc7c 0ea0 3b64 1ca1 0190 0273 c87c 0b64  .|..;d.....s.|.d
+00003130: 0075 0090 0273 dc64 277c 0b9b 0064 287c  .u...s.d'|...d(|
+00003140: 0e64 1919 009b 0064 297c 0e64 1719 009b  .d.....d)|.d....
+00003150: 009d 067d 037c 01a0 047c 03a1 0101 0090  ...}.|...|......
+00003160: 0271 a664 2a7c 0c9b 009d 0267 017d 157c  .q.d*|.....g.}.|
+00003170: 1190 0273 fb74 157c 0ea0 3b64 22a1 0174  ...s.t.|..;d"..t
+00003180: 0b83 0290 0272 f67c 15a0 4564 2ba1 0101  .....r.|..Ed+...
+00003190: 006e 057c 15a0 4564 2ca1 0101 007c 0ea0  .n.|..Ed,....|..
+000031a0: 3a64 2d64 0da1 0290 0372 077c 15a0 4564  :d-d.....r.|..Ed
+000031b0: 2ea1 0101 007c 096a 4690 0372 147c 15a0  .....|.jF..r.|..
+000031c0: 4564 2f7c 096a 469b 009d 02a1 0101 0064  Ed/|.jF........d
+000031d0: 3064 31a0 477c 15a1 019b 009d 027d 167c  0d1.G|.......}.|
+000031e0: 0ea0 3b64 32a1 0190 0372 2d7c 0e64 3205  ..;d2....r-|.d2.
+000031f0: 0019 0064 337c 1617 0037 0003 003c 006e  ...d3|...7...<.n
+00003200: 047c 167c 0e64 323c 007c 0ea0 3a64 3464  .|.|.d2<.|..:d4d
+00003210: 00a1 027d 177c 1790 0373 417c 1190 0372  ...}.|...sA|...r
+00003220: 3f64 356e 0164 367d 177c 04a0 3b7c 1764  ?d5n.d6}.|..;|.d
+00003230: 00a1 027d 187c 1890 0373 537c 01a0 487c  ...}.|...sS|..H|
+00003240: 17a1 017d 187c 187c 047c 173c 007c 096a  ...}.|.|.|.<.|.j
+00003250: 4990 0372 7e7c 1190 0372 6564 377c 096a  I..r~|...red7|.j
+00003260: 369b 009d 027d 037c 01a0 047c 03a1 0101  6....}.|...|....
+00003270: 007c 016a 4a7c 016a 4ba0 3b88 006a 4ca1  .|.jJ|.jK.;..jL.
+00003280: 0119 007c 1719 00a0 457c 096a 367c 1090  ...|....E|.j6|..
+00003290: 0372 7a7c 1064 0c19 006e 0164 0066 02a1  .rz|.d...n.d.f..
+000032a0: 0101 007c 186a 4d7c 1069 007c 0ea4 018e  ...|.jM|.i.|....
+000032b0: 0101 007c 07a0 457c 09a1 0101 0071 3e7c  ...|..E|.....q>|
+000032c0: 0753 0029 384e 7a3e 5468 6973 2070 6172  .S.)8Nz>This par
+000032d0: 7365 7220 616c 7265 6164 7920 636f 6e74  ser already cont
+000032e0: 6169 6e73 2061 7267 756d 656e 7473 2066  ains arguments f
+000032f0: 726f 6d20 616e 6f74 6865 7220 6461 7461  rom another data
+00003300: 636c 6173 732e 6301 0000 0000 0000 0000  class.c.........
+00003310: 0000 0001 0000 0004 0000 0013 0000 0073  ...............s
+00003320: 1200 0000 8800 6a00 8801 7c00 6a01 6401  ......j...|.j.d.
+00003330: 8d02 0c00 5300 2902 4e72 a300 0000 2902  ....S.).Nr....).
+00003340: 72a4 0000 0072 9200 0000 2901 da01 66a9  r....r....)...f.
+00003350: 02da 0363 6c73 5a05 6d6f 6465 6c72 5300  ...clsZ.modelrS.
+00003360: 0000 7257 0000 0072 5e00 0000 b201 0000  ..rW...r^.......
+00003370: f302 0000 0012 007a 2f41 7267 756d 656e  .......z/Argumen
+00003380: 7450 6172 7365 722e 5f61 6464 5f61 7267  tParser._add_arg
+00003390: 756d 656e 7473 2e3c 6c6f 6361 6c73 3e2e  uments.<locals>.
+000033a0: 3c6c 616d 6264 613e 6301 0000 0000 0000  <lambda>c.......
+000033b0: 0000 0000 0002 0000 0007 0000 0053 0000  .............S..
+000033c0: 0073 2000 0000 6700 7c00 5d0c 7d01 7c01  .s ...g.|.].}.|.
+000033d0: 7c01 6a00 a001 7402 7403 8300 a102 6602  |.j...t.t.....f.
+000033e0: 9102 7102 5300 7253 0000 0029 04da 086d  ..q.S.rS...)...m
+000033f0: 6574 6164 6174 61da 0367 6574 7221 0000  etadata..getr!..
+00003400: 0072 2200 0000 7254 0000 0072 5300 0000  .r"...rT...rS...
+00003410: 7253 0000 0072 5700 0000 7258 0000 00b7  rS...rW...rX....
+00003420: 0100 0073 0800 0000 0600 0202 12ff 06ff  ...s............
+00003430: 7a31 4172 6775 6d65 6e74 5061 7273 6572  z1ArgumentParser
+00003440: 2e5f 6164 645f 6172 6775 6d65 6e74 732e  ._add_arguments.
+00003450: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00003460: 6d70 3e72 3d00 0000 5429 01da 0d69 735f  mp>r=...T)...is_
+00003470: 756e 696f 6e5f 7479 7065 da01 2e72 1700  union_type...r..
+00003480: 0000 a901 da08 6d61 7873 706c 6974 e9ff  ......maxsplit..
+00003490: ffff ff46 7201 0000 0029 01da 1061 7373  ...Fr....)...ass
+000034a0: 6572 745f 7072 696d 6974 6976 6563 0100  ert_primitivec..
+000034b0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+000034c0: 0000 5300 0000 7312 0000 0067 007c 005d  ..S...s....g.|.]
+000034d0: 057d 017c 016a 0091 0271 0253 0072 5300  .}.|.j...q.S.rS.
+000034e0: 0000 a901 7292 0000 0072 5400 0000 7253  ....r....rT...rS
+000034f0: 0000 0072 5300 0000 7257 0000 0072 5800  ...rS...rW...rX.
+00003500: 0000 1302 0000 72a8 0000 00fa 012b da01  ......r......+..
+00003510: 2ada 0370 6f73 7267 0000 0063 0100 0000  *..posrg...c....
+00003520: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+00003530: 5300 0000 731a 0000 0067 007c 005d 097d  S...s....g.|.].}
+00003540: 017c 01a0 0064 00a1 0172 027c 0191 0271  .|...d...r.|...q
+00003550: 0253 0029 0172 6500 0000 725f 0000 0072  .S.).re...r_...r
+00003560: 5400 0000 7253 0000 0072 5300 0000 7257  T...rS...rS...rW
+00003570: 0000 0072 5800 0000 3302 0000 7302 0000  ...rX...3...s...
+00003580: 001a 00da 076d 6574 6176 6172 7264 0000  .....metavarrd..
+00003590: 00fa 013c da04 6465 7374 fa01 3e7a 073c  ...<..dest..>z.<
+000035a0: 7661 6c75 653e da08 7265 7175 6972 6564  value>..required
+000035b0: da05 6e61 7267 73fa 013f da04 7479 7065  ..nargs..?..type
+000035c0: 2905 72bc 0000 0072 ba00 0000 da05 636f  ).r....r......co
+000035d0: 6e73 7472 6400 0000 72b5 0000 0072 5900  nstrd...r....rY.
+000035e0: 0000 7263 0000 00da 0072 5300 0000 2902  ..rc.....rS...).
+000035f0: 7267 0000 0072 b700 0000 2903 7266 0000  rg...r....).rf..
+00003600: 00da 096e 616d 6573 7061 6365 da06 7661  ...namespace..va
+00003610: 6c75 6573 7a0f 496e 7661 6c69 6420 7661  luesz.Invalid va
+00003620: 6c75 6520 277a 1027 2066 6f72 2061 7267  lue 'z.' for arg
+00003630: 756d 656e 7420 277a 1327 3b20 6d75 7374  ument 'z.'; must
+00003640: 2062 6520 6f6e 6520 6f66 3a20 7a06 5479   be one of: z.Ty
+00003650: 7065 3a20 7a16 4465 6661 756c 743a 2022  pe: z.Default: "
+00003660: 2528 6465 6661 756c 7429 7322 7a14 4465  %(default)s"z.De
+00003670: 6661 756c 743a 2025 2864 6566 6175 6c74  fault: %(default
+00003680: 2973 da09 6578 636c 7573 6976 657a 044d  )s..exclusivez.M
+00003690: 2e58 2e7a 0545 6e76 3a20 7a02 3e20 fa02  .X.z.Env: z.> ..
+000036a0: 2c20 725a 0000 0072 7d00 0000 da05 6772  , rZ...r}.....gr
+000036b0: 6f75 707a 1372 6571 7569 7265 6420 7061  oupz.required pa
+000036c0: 7261 6d65 7465 7273 7a13 6f70 7469 6f6e  rametersz.option
+000036d0: 616c 2070 6172 616d 6574 6572 737a 3341  al parametersz3A
+000036e0: 206d 7574 7561 6c6c 792d 6578 636c 7573   mutually-exclus
+000036f0: 6976 6520 7061 7261 6d65 7465 7220 6361  ive parameter ca
+00003700: 6e6e 6f74 2062 6520 7265 7175 6972 6564  nnot be required
+00003710: 3a20 294e 7234 0000 0072 2500 0000 da0b  : )Nr4...r%.....
+00003720: 6765 745f 6465 6661 756c 7472 4600 0000  get_defaultrF...
+00003730: 7282 0000 0072 9d00 0000 725d 0000 00da  r....r....r]....
+00003740: 0666 696c 7465 7272 0600 0000 72bc 0000  .filterr....r...
+00003750: 0072 3800 0000 726e 0000 0072 2300 0000  .r8...rn...r#...
+00003760: 727f 0000 00da 0c76 6572 7369 6f6e 5f69  r......version_i
+00003770: 6e66 6f72 3f00 0000 da10 5f67 6574 5f74  nfor?....._get_t
+00003780: 7970 655f 6f72 6967 696e 7215 0000 00da  ype_originr.....
+00003790: 1c5f 6578 7472 6163 745f 7479 7065 5f66  ._extract_type_f
+000037a0: 726f 6d5f 636f 6e74 6169 6e65 7272 3c00  rom_containerr<.
+000037b0: 0000 da12 5f67 6574 5f74 7970 655f 6d65  ...._get_type_me
+000037c0: 7461 6461 7461 726d 0000 0072 0500 0000  tadatarm...r....
+000037d0: 7221 0000 0072 a900 0000 7295 0000 00da  r!...r....r.....
+000037e0: 0672 7370 6c69 74da 0873 6574 5f64 6573  .rsplit..set_des
+000037f0: 7472 9200 0000 72b9 0000 0072 6300 0000  tr....r....rc...
+00003800: 7204 0000 00da 0f64 6566 6175 6c74 5f66  r......default_f
+00003810: 6163 746f 7279 722a 0000 00da 0e5f 6765  actoryr*....._ge
+00003820: 745f 7479 7065 5f61 7267 7372 6400 0000  t_type_argsrd...
+00003830: 7239 0000 00da 0b63 6f6c 6c65 6374 696f  r9.....collectio
+00003840: 6e73 da03 6162 63da 074d 6170 7069 6e67  ns..abc..Mapping
+00003850: 7259 0000 0072 1d00 0000 da08 4974 6572  rY...r......Iter
+00003860: 6162 6c65 da03 7365 7472 1f00 0000 da05  able..setr......
+00003870: 7475 706c 6572 2000 0000 721e 0000 0072  tupler ...r....r
+00003880: 3500 0000 7227 0000 0072 0700 0000 7208  5...r'...r....r.
+00003890: 0000 0072 3100 0000 7272 0000 0072 b700  ...r1...rr...r..
+000038a0: 0000 72b4 0000 0072 ba00 0000 da06 6173  ..r....r......as
+000038b0: 6469 6374 7297 0000 0072 aa00 0000 da05  dictr....r......
+000038c0: 7570 7065 72da 0462 6f6f 6c72 1800 0000  upper..boolr....
+000038d0: da03 696e 7472 1900 0000 721a 0000 0072  ..intr....r....r
+000038e0: 7400 0000 da06 4163 7469 6f6e da07 6765  t.....Action..ge
+000038f0: 7461 7474 72da 0661 7070 656e 64da 085f  tattr..append.._
+00003900: 656e 765f 7661 72da 046a 6f69 6eda 1261  env_var..join..a
+00003910: 6464 5f61 7267 756d 656e 745f 6772 6f75  dd_argument_grou
+00003920: 7072 c100 0000 7271 0000 00da 095f 6465  pr....rq....._de
+00003930: 6661 756c 7473 7245 0000 0072 6f00 0000  faultsrE...ro...
+00003940: 2919 72a7 0000 0072 6600 0000 728f 0000  ).r....rf...r...
+00003950: 00da 0365 7272 5a11 7061 7273 6572 5f61  ...errZ.parser_a
+00003960: 7267 5f67 726f 7570 735a 0c6e 6f76 656c  rg_groupsZ.novel
+00003970: 5f66 6965 6c64 735a 106e 6f76 656c 5f66  _fieldsZ.novel_f
+00003980: 6965 6c64 5f61 7267 735a 0a61 6464 6564  ield_argsZ.added
+00003990: 5f61 7267 735a 0366 6c64 5a11 6172 6770  _argsZ.fldZ.argp
+000039a0: 6172 7365 5f61 7267 756d 656e 74da 0866  arse_argument..f
+000039b0: 6c64 5f74 7970 6572 5600 0000 5a09 6865  ld_typerV...Z.he
+000039c0: 6c70 5f74 7970 655a 0f66 6c64 5f74 7970  lp_typeZ.fld_typ
+000039d0: 655f 6f72 6967 696e 7251 0000 0072 6700  e_originrQ...rg.
+000039e0: 0000 7250 0000 0072 b900 0000 da01 6b5a  ..rP...r......kZ
+000039f0: 0f64 756d 6d79 5f6e 616d 6573 7061 6365  .dummy_namespace
+00003a00: da01 645a 0e68 656c 705f 6d73 675f 7061  ..dZ.help_msg_pa
+00003a10: 7274 735a 0868 656c 705f 6d73 6772 c300  rtsZ.help_msgr..
+00003a20: 0000 5a09 6172 675f 6772 6f75 7072 5300  ..Z.arg_grouprS.
+00003a30: 0000 72a6 0000 0072 5700 0000 7290 0000  ..r....rW...r...
+00003a40: 0099 0100 0073 a401 0000 080a 0601 0802  .....s..........
+00003a50: 0c02 0401 0a01 1602 0402 0202 0201 0c01  ................
+00003a60: 0601 02fe 04ff 0607 0202 06fe 0405 0e02  ................
+00003a70: 0601 0a04 0801 0e01 1403 0e01 0401 0201  ................
+00003a80: 0201 06fe 0a05 0e01 1401 0a01 0401 0280  ................
+00003a90: 0a02 1403 0e01 0401 0201 0201 06fe 0807  ................
+00003aa0: 08ff 1402 02fd 0c06 0602 0a01 0801 0801  ................
+00003ab0: 0a01 0a01 0601 0a02 0601 1001 1001 0801  ................
+00003ac0: 0e01 0280 1003 0401 0201 0201 06fe 0804  ................
+00003ad0: 0601 0280 0c03 04ff 0a02 0402 0201 0201  ................
+00003ae0: 06fe 0804 0a01 0801 0a01 0801 0602 0280  ................
+00003af0: 0602 0801 0c02 1001 0c02 0203 0201 0201  ................
+00003b00: 0cfe 1405 0801 0801 0602 0604 0c02 0a01  ................
+00003b10: 0602 0802 0601 0a02 0203 08ff 0c02 02fd  ................
+00003b20: 1606 1c02 06ff 0804 0602 0602 1601 0801  ................
+00003b30: 1001 0c01 0c01 0203 0201 0201 0cfe 0805  ................
+00003b40: 1001 0a01 0801 0280 0c02 1001 0a01 0a02  ................
+00003b50: 0a01 0802 0c04 0c01 1001 0e02 0601 0801  ................
+00003b60: 06fe 0e05 1201 0201 0201 0601 06fd 1405  ................
+00003b70: 0a01 1401 0c03 0801 0e01 0201 0601 06fe  ................
+00003b80: 0604 0802 0e02 0802 04fe 1003 0803 04fd  ................
+00003b90: 0a03 1203 0601 04ff 02ff 0a04 0480 0c02  ................
+00003ba0: 0603 1201 0c01 0a02 0e02 0a01 0802 1201  ................
+00003bb0: 1002 0c02 1601 0802 0c02 0602 0e01 0c02  ................
+00003bc0: 0602 0a01 0801 0802 0601 0202 0401 04ff  ................
+00003bd0: 02ff 0a04 0402 0c01 02ff 0202 02fe 0202  ................
+00003be0: 0402 1001 02fe 04ff 1007 0c02 0402 7a1d  ..............z.
+00003bf0: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
+00003c00: 6164 645f 6172 6775 6d65 6e74 73da 0174  add_arguments..t
+00003c10: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00003c20: 0004 0000 0043 0000 0073 0c00 0000 7400  .....C...s....t.
+00003c30: 7c00 6401 6400 8303 5300 2902 4eda 0a5f  |.d.d...S.).N.._
+00003c40: 5f6f 7269 6769 6e5f 5fa9 0172 d900 0000  _origin__..r....
+00003c50: a901 72e3 0000 0072 5300 0000 7253 0000  ..r....rS...rS..
+00003c60: 0072 5700 0000 72c7 0000 00c0 0200 00f3  .rW...r.........
+00003c70: 0200 0000 0c02 7a1f 4172 6775 6d65 6e74  ......z.Argument
+00003c80: 5061 7273 6572 2e5f 6765 745f 7479 7065  Parser._get_type
+00003c90: 5f6f 7269 6769 6e63 0100 0000 0000 0000  _originc........
+00003ca0: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
+00003cb0: f30c 0000 0074 007c 0064 0164 0283 0353  .....t.|.d.d...S
+00003cc0: 0029 034e da08 5f5f 6172 6773 5f5f 7253  .).N..__args__rS
+00003cd0: 0000 0072 e500 0000 72e6 0000 0072 5300  ...r....r....rS.
+00003ce0: 0000 7253 0000 0072 5700 0000 72cd 0000  ..rS...rW...r...
+00003cf0: 00c4 0200 0072 e700 0000 7a1d 4172 6775  .....r....z.Argu
+00003d00: 6d65 6e74 5061 7273 6572 2e5f 6765 745f  mentParser._get_
+00003d10: 7479 7065 5f61 7267 7363 0100 0000 0000  type_argsc......
+00003d20: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+00003d30: 0000 72e8 0000 0029 034e da0c 5f5f 6d65  ..r....).N..__me
+00003d40: 7461 6461 7461 5f5f 7253 0000 0072 e500  tadata__rS...r..
+00003d50: 0000 72e6 0000 0072 5300 0000 7253 0000  ..r....rS...rS..
+00003d60: 0072 5700 0000 72c9 0000 00c8 0200 0072  .rW...r........r
+00003d70: e700 0000 7a21 4172 6775 6d65 6e74 5061  ....z!ArgumentPa
+00003d80: 7273 6572 2e5f 6765 745f 7479 7065 5f6d  rser._get_type_m
+00003d90: 6574 6164 6174 61da 0e74 7970 655f 636f  etadata..type_co
+00003da0: 6e74 6169 6e65 7272 b000 0000 72ab 0000  ntainerr....r...
+00003db0: 0063 0400 0000 0000 0000 0000 0000 0b00  .c..............
+00003dc0: 0000 0300 0000 4300 0000 7318 0100 007c  ......C...s....|
+00003dd0: 0372 0474 006e 047c 00a0 017c 01a1 017d  .r.t.n.|...|...}
+00003de0: 047c 0464 0075 0072 1574 0264 017c 016a  .|.d.u.r.t.d.|.j
+00003df0: 039b 009d 0283 0182 017c 00a0 047c 01a1  .........|...|..
+00003e00: 017d 0564 0264 0384 007c 0544 0083 017d  .}.d.d...|.D...}
+00003e10: 067c 0474 0075 0073 3074 057c 0474 066a  .|.t.u.s0t.|.t.j
+00003e20: 076a 0883 0273 307c 0474 0975 0072 4074  .j...s0|.t.u.r@t
+00003e30: 0a7c 0683 0164 046b 0372 3b7c 06a0 0ba1  .|...d.k.r;|....
+00003e40: 0001 006e 2c7c 0664 0519 007d 076e 2774  ...n,|.d...}.n't
+00003e50: 057c 0474 066a 076a 0c83 0272 6174 0a7c  .|.t.j.j...rat.|
+00003e60: 0683 0164 066b 0372 527c 06a0 0ba1 0001  ...d.k.rR|......
+00003e70: 006e 157c 065c 027d 087d 097c 0874 0d75  .n.|.\.}.}.|.t.u
+00003e80: 0172 5e74 0264 0783 0182 017c 097d 076e  .r^t.d.....|.}.n
+00003e90: 0674 0e73 6774 0f7c 0183 0101 007c 0673  .t.sgt.|.....|.s
+00003ea0: 6d74 0264 0883 0182 017c 00a0 017c 07a1  mt.d.....|...|..
+00003eb0: 017d 0a7c 0a74 0075 0072 807c 00a0 107c  .}.|.t.u.r.|...|
+00003ec0: 07a1 017d 077c 00a0 017c 07a1 017d 0a7c  ...}.|...|...}.|
+00003ed0: 0272 8a7c 0a72 8a74 0e73 8a74 0f7c 0a83  .r.|.r.t.s.t.|..
+00003ee0: 0101 007c 0753 0029 094e 7a1f 4769 7665  ...|.S.).Nz.Give
+00003ef0: 6e20 7479 7065 2069 7320 6e6f 7420 6120  n type is not a 
+00003f00: 636f 6e74 6169 6e65 723a 2063 0100 0000  container: c....
+00003f10: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00003f20: 5300 0000 7320 0000 0067 007c 005d 0c7d  S...s ...g.|.].}
+00003f30: 017c 0164 0075 0172 027c 0174 0075 0172  .|.d.u.r.|.t.u.r
+00003f40: 027c 0191 0271 0253 0029 012e 2901 722b  .|...q.S.)..).r+
+00003f50: 0000 0029 0272 5500 0000 da01 6172 5300  ...).rU.....arS.
+00003f60: 0000 7253 0000 0072 5700 0000 7258 0000  ..rS...rW...rX..
+00003f70: 00de 0200 0073 0400 0000 0600 1a01 7a3f  .....s........z?
+00003f80: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
+00003f90: 6578 7472 6163 745f 7479 7065 5f66 726f  extract_type_fro
+00003fa0: 6d5f 636f 6e74 6169 6e65 722e 3c6c 6f63  m_container.<loc
+00003fb0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
+00003fc0: 1700 0000 7201 0000 0072 7c00 0000 7a22  ....r....r|...z"
+00003fd0: 4469 6374 696f 6e61 7279 206b 6579 7320  Dictionary keys 
+00003fe0: 6d75 7374 2062 6520 7479 7065 2060 7374  must be type `st
+00003ff0: 7260 7a1b 546f 6f20 6d61 6e79 2074 7970  r`z.Too many typ
+00004000: 6573 2069 6e20 636f 6e74 6169 6e65 7229  es in container)
+00004010: 1172 1500 0000 72c7 0000 00da 0954 7970  .r....r......Typ
+00004020: 6545 7272 6f72 7295 0000 0072 cd00 0000  eErrorr....r....
+00004030: 7239 0000 0072 ce00 0000 72cf 0000 0072  r9...r....r....r
+00004040: 1100 0000 72d2 0000 0072 7600 0000 da05  ....r....rv.....
+00004050: 636c 6561 7272 d000 0000 726e 0000 0072  clearr....rn...r
+00004060: 3500 0000 7227 0000 0072 c800 0000 290b  5...r'...r....).
+00004070: 72a7 0000 0072 eb00 0000 72b0 0000 0072  r....r....r....r
+00004080: ab00 0000 5a15 7479 7065 5f63 6f6e 7461  ....Z.type_conta
+00004090: 696e 6572 5f6f 7269 6769 6e5a 1374 7970  iner_originZ.typ
+000040a0: 655f 636f 6e74 6169 6e65 725f 6172 6773  e_container_args
+000040b0: da07 7265 7375 6c74 735a 1674 7970 655f  ..resultsZ.type_
+000040c0: 636f 6e74 6169 6e65 725f 7375 6274 7970  container_subtyp
+000040d0: 655a 086b 6579 5f74 7970 655a 0a76 616c  eZ.key_typeZ.val
+000040e0: 7565 5f74 7970 655a 1d74 7970 655f 636f  ue_typeZ.type_co
+000040f0: 6e74 6169 6e65 725f 7375 6274 7970 655f  ntainer_subtype_
+00004100: 6f72 6967 696e 7253 0000 0072 5300 0000  originrS...rS...
+00004110: 7257 0000 0072 c800 0000 cc02 0000 7354  rW...r........sT
+00004120: 0000 0010 0802 ff08 0402 010a 0104 ff0a  ................
+00004130: 0406 0202 0106 ff08 070c 0102 ff08 020c  ................
+00004140: 020a 010a 020e 010c 010a 0108 0208 0108  ................
+00004150: 0106 0104 0108 0104 0208 010a 0208 0204  ................
+00004160: 0102 0104 ff0a 0302 0302 ff02 0202 fe02  ................
+00004170: 0302 fd08 0504 027a 2b41 7267 756d 656e  .......z+Argumen
+00004180: 7450 6172 7365 722e 5f65 7874 7261 6374  tParser._extract
+00004190: 5f74 7970 655f 6672 6f6d 5f63 6f6e 7461  _type_from_conta
+000041a0: 696e 6572 6301 0000 0000 0000 0000 0000  inerc...........
+000041b0: 0002 0000 0006 0000 000b 0000 0073 6400  .............sd.
+000041c0: 0000 7c01 a000 6401 6402 a102 7c01 6401  ..|...d.d...|.d.
+000041d0: 3c00 7c01 a000 6403 6404 a102 7c01 6403  <.|...d.d...|.d.
+000041e0: 3c00 7c01 a000 6405 8800 6a01 a102 7c01  <.|...d...j...|.
+000041f0: 6405 3c00 7c01 a000 6406 8700 6601 6407  d.<.|...d...f.d.
+00004200: 6408 8408 a102 7c01 6406 3c00 7402 8300  d.....|.d.<.t...
+00004210: 6a03 6409 6900 7c01 a401 8e01 8800 5f04  j.d.i.|......._.
+00004220: 8800 6a04 5300 290a 4e72 6c00 0000 5a08  ..j.S.).Nrl...Z.
+00004230: 636f 6d6d 616e 6473 72b5 0000 007a 093c  commandsr....z.<
+00004240: 434f 4d4d 414e 443e 72b7 0000 00da 0c70  COMMAND>r......p
+00004250: 6172 7365 725f 636c 6173 7363 0000 0000  arser_classc....
+00004260: 0000 0000 0000 0000 0100 0000 0600 0000  ................
+00004270: 1b00 0000 731e 0000 0074 0088 0083 0164  ....s....t.....d
+00004280: 0369 007c 00a4 0164 0188 006a 0164 029c  .i.|...d...j.d..
+00004290: 02a4 018e 0153 0029 044e 5429 0272 4f00  .....S.).NT).rO.
+000042a0: 0000 724e 0000 0072 5300 0000 2902 72bc  ..rN...rS...).r.
+000042b0: 0000 0072 4e00 0000 2901 72e1 0000 00a9  ...rN...).r.....
+000042c0: 0172 7800 0000 7253 0000 0072 5700 0000  .rx...rS...rW...
+000042d0: 725e 0000 0012 0300 0073 0c00 0000 0a00  r^.......s......
+000042e0: 0201 02ff 0202 0401 0afd 7a2f 4172 6775  ..........z/Argu
+000042f0: 6d65 6e74 5061 7273 6572 2e61 6464 5f73  mentParser.add_s
+00004300: 7562 7061 7273 6572 732e 3c6c 6f63 616c  ubparsers.<local
+00004310: 733e 2e3c 6c61 6d62 6461 3e72 5300 0000  s>.<lambda>rS...
+00004320: 2905 72aa 0000 0072 4400 0000 7268 0000  ).r....rD...rh..
+00004330: 00da 0e61 6464 5f73 7562 7061 7273 6572  ...add_subparser
+00004340: 7372 6a00 0000 2902 7278 0000 0072 5100  srj...).rx...rQ.
+00004350: 0000 7279 0000 0072 f100 0000 7257 0000  ..ry...r....rW..
+00004360: 0072 f200 0000 0c03 0000 7312 0000 0010  .r........s.....
+00004370: 0110 0112 0104 0102 010a 0108 fe14 0906  ................
+00004380: 027a 1d41 7267 756d 656e 7450 6172 7365  .z.ArgumentParse
+00004390: 722e 6164 645f 7375 6270 6172 7365 7273  r.add_subparsers
+000043a0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000043b0: 0004 0000 0043 0000 0073 2c00 0000 7c00  .....C...s,...|.
+000043c0: 6a00 4400 5d10 7d01 7401 7c01 7402 6a03  j.D.].}.t.|.t.j.
+000043d0: 8302 7213 7c01 7c00 5f04 7c00 6a04 0200  ..r.|.|._.|.j...
+000043e0: 0100 5300 7103 6400 5300 725c 0000 0029  ..S.q.d.S.r\...)
+000043f0: 05da 085f 6163 7469 6f6e 7372 6d00 0000  ..._actionsrm...
+00004400: 7274 0000 0072 9600 0000 726a 0000 0029  rt...r....rj...)
+00004410: 0272 7800 0000 72ec 0000 0072 5300 0000  .rx...r....rS...
+00004420: 7253 0000 0072 5700 0000 728c 0000 001d  rS...rW...r.....
+00004430: 0300 0073 1200 0000 0a01 0201 0201 0401  ...s............
+00004440: 04fe 0604 0a01 02fb 0406 7a26 4172 6775  ..........z&Argu
+00004450: 6d65 6e74 5061 7273 6572 2e5f 6669 6e64  mentParser._find
+00004460: 5f73 7562 7061 7273 6572 735f 6163 7469  _subparsers_acti
+00004470: 6f6e 6301 0000 0000 0000 0000 0000 0001  onc.............
+00004480: 0000 0002 0000 0043 0000 0073 3600 0000  .......C...s6...
+00004490: 7c00 6a00 6400 7501 7208 7c00 6a00 5300  |.j.d.u.r.|.j.S.
+000044a0: 7c00 6a01 7217 7c00 a002 a100 0100 7c00  |.j.r.|.......|.
+000044b0: 6a00 7314 4a00 8201 7c00 6a00 5300 7c00  j.s.J...|.j.S.|.
+000044c0: a003 a100 5300 725c 0000 0029 0472 6a00  ....S.r\...).rj.
+000044d0: 0000 728b 0000 0072 8c00 0000 72f2 0000  ..r....r....r...
+000044e0: 0072 f100 0000 7253 0000 0072 5300 0000  .r....rS...rS...
+000044f0: 7257 0000 0072 7700 0000 2703 0000 730e  rW...rw...'...s.
+00004500: 0000 000a 0106 0106 0208 010a 0106 0108  ................
+00004510: 027a 2541 7267 756d 656e 7450 6172 7365  .z%ArgumentParse
+00004520: 722e 5f67 6574 5f6f 725f 6164 645f 7375  r._get_or_add_su
+00004530: 6270 6172 7365 7273 72bf 0000 0063 0200  bparsersr....c..
+00004540: 0000 0000 0000 0000 0000 0600 0000 0600  ................
+00004550: 0000 0300 0000 736e 0000 007c 006a 00a0  ......sn...|.j..
+00004560: 0174 0288 007c 006a 0364 0083 0369 00a1  .t...|.j.d...i..
+00004570: 027d 027c 02a0 04a1 0044 005d 1d7d 0387  .}.|.....D.].}..
+00004580: 0066 0164 0164 0284 087c 0344 0083 017d  .f.d.d...|.D...}
+00004590: 0474 057c 0483 0164 036b 0472 2d64 0464  .t.|...d.k.r-d.d
+000045a0: 05a0 067c 04a1 0117 007d 057c 00a0 077c  ...|.....}.|...|
+000045b0: 05a1 0101 0071 1074 0864 0669 0074 0988  .....q.t.d.i.t..
+000045c0: 0083 01a4 018e 0153 0029 074e 6301 0000  .......S.).Nc...
+000045d0: 0000 0000 0000 0000 0004 0000 0005 0000  ................
+000045e0: 0013 0000 0073 6c00 0000 6700 7c00 5d32  .....sl...g.|.]2
+000045f0: 5c02 7d01 7d02 7400 8800 7c01 8302 7234  \.}.}.t...|...r4
+00004600: 7401 8800 7c01 8302 7d03 7402 7c03 7403  t...|...}.t.|.t.
+00004610: 8302 731c 7402 7c03 7404 6a05 6a06 8302  ..s.t.|.t.j.j...
+00004620: 7320 7c03 6400 7501 732e 7402 7c03 7403  s |.d.u.s.t.|.t.
+00004630: 8302 7302 7402 7c03 7404 6a05 6a06 8302  ..s.t.|.t.j.j...
+00004640: 7202 7c03 7202 7c02 7232 7c02 6e01 7c01  r.|.r.|.r2|.n.|.
+00004650: 9102 7102 5300 725c 0000 0029 07da 0768  ..q.S.r\...)...h
+00004660: 6173 6174 7472 72d9 0000 0072 3800 0000  asattrr....r8...
+00004670: 726e 0000 0072 ce00 0000 72cf 0000 0072  rn...r....r....r
+00004680: d100 0000 2904 7255 0000 0072 b700 0000  ....).rU...r....
+00004690: da04 666c 6167 5a0a 6174 7472 5f76 616c  ..flagZ.attr_val
+000046a0: 7565 a901 72bf 0000 0072 5300 0000 7257  ue..r....rS...rW
+000046b0: 0000 0072 5800 0000 4103 0000 7330 0000  ...rX...A...s0..
+000046c0: 0006 0006 0208 0102 fd0a 0408 0302 f902  ................
+000046d0: 0802 0106 0102 fe02 f808 0d08 0302 fd02  ................
+000046e0: 0402 0106 0102 fe02 fc02 0802 f80a f406  ................
+000046f0: 0c7a 3341 7267 756d 656e 7450 6172 7365  .z3ArgumentParse
+00004700: 722e 5f70 6f73 745f 7061 7273 655f 6172  r._post_parse_ar
+00004710: 6773 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  gs.<locals>.<lis
+00004720: 7463 6f6d 703e 7217 0000 007a 2854 6865  tcomp>r....z(The
+00004730: 7365 2061 7267 756d 656e 7473 2061 7265  se arguments are
+00004740: 206d 7574 7561 6c6c 7920 6578 636c 7573   mutually exclus
+00004750: 6976 653a 2072 c200 0000 7253 0000 0029  ive: r....rS...)
+00004760: 0a72 7100 0000 72aa 0000 0072 d900 0000  .rq...r....r....
+00004770: 7245 0000 0072 c000 0000 7276 0000 0072  rE...r....rv...r
+00004780: dc00 0000 7282 0000 0072 2800 0000 da04  ....r....r(.....
+00004790: 7661 7273 2906 7278 0000 0072 bf00 0000  vars).rx...r....
+000047a0: 5a12 6675 6e63 5f6d 785f 6172 675f 6772  Z.func_mx_arg_gr
+000047b0: 6f75 7073 5a06 675f 6172 6773 5a0e 6d78  oupsZ.g_argsZ.mx
+000047c0: 5f66 6c61 6773 5f66 6f75 6e64 72df 0000  _flags_foundr...
+000047d0: 0072 5300 0000 72f6 0000 0072 5700 0000  .rS...r....rW...
+000047e0: da10 5f70 6f73 745f 7061 7273 655f 6172  .._post_parse_ar
+000047f0: 6773 3203 0000 7320 0000 0006 070c 0102  gs2...s ........
+00004800: 0102 fe02 fd0c 070a 0402 0206 fe0c 1906  ................
+00004810: 0102 0106 ff0a 0302 8012 027a 1f41 7267  ...........z.Arg
+00004820: 756d 656e 7450 6172 7365 722e 5f70 6f73  umentParser._pos
+00004830: 745f 7061 7273 655f 6172 6773 6303 0000  t_parse_argsc...
+00004840: 0000 0000 0000 0000 0005 0000 000a 0000  ................
+00004850: 0003 0000 0073 5200 0000 7a0e 7400 8300  .....sR...z.t...
+00004860: 6a01 7c01 7c02 6401 8d02 7d03 7c00 a002  j.|.|.d...}.|...
+00004870: 7c03 a101 5700 5300 0400 7403 7928 0100  |...W.S...t.y(..
+00004880: 7d04 0100 7a0e 7c00 a004 7405 7c04 8301  }...z.|...t.|...
+00004890: a101 0100 5700 5900 6400 7d04 7e04 6400  ....W.Y.d.}.~.d.
+000048a0: 5300 6400 7d04 7e04 7701 7700 a902 4e29  S.d.}.~.w.w...N)
+000048b0: 0272 5000 0000 72bf 0000 0029 0672 6800  .rP...r....).rh.
+000048c0: 0000 da0a 7061 7273 655f 6172 6773 72f8  ....parse_argsr.
+000048d0: 0000 00da 0a56 616c 7565 4572 726f 7272  .....ValueErrorr
+000048e0: 8200 0000 726e 0000 0029 0572 7800 0000  ....rn...).rx...
+000048f0: 7250 0000 0072 bf00 0000 da06 7061 7273  rP...r......pars
+00004900: 6564 da01 6572 7900 0000 7253 0000 0072  ed..ery...rS...r
+00004910: 5700 0000 72fa 0000 0062 0300 0073 1400  W...r....b...s..
+00004920: 0000 0205 0601 0201 0201 06fe 0c04 0e01  ................
+00004930: 1c01 0880 02ff 7a19 4172 6775 6d65 6e74  ......z.Argument
+00004940: 5061 7273 6572 2e70 6172 7365 5f61 7267  Parser.parse_arg
+00004950: 7363 0300 0000 0000 0000 0000 0000 0600  sc..............
+00004960: 0000 0a00 0000 0300 0000 735a 0000 007a  ..........sZ...z
+00004970: 1274 0083 006a 017c 017c 0264 018d 025c  .t...j.|.|.d...\
+00004980: 027d 037d 047c 00a0 027c 03a1 017c 0466  .}.}.|...|...|.f
+00004990: 0257 0053 0004 0074 0379 2c01 007d 0501  .W.S...t.y,..}..
+000049a0: 007a 0e7c 00a0 0474 057c 0583 01a1 0101  .z.|...t.|......
+000049b0: 0057 0059 0064 007d 057e 0564 0053 0064  .W.Y.d.}.~.d.S.d
+000049c0: 007d 057e 0577 0177 0072 f900 0000 2906  .}.~.w.w.r....).
+000049d0: 7268 0000 00da 1070 6172 7365 5f6b 6e6f  rh.....parse_kno
+000049e0: 776e 5f61 7267 7372 f800 0000 72fb 0000  wn_argsr....r...
+000049f0: 0072 8200 0000 726e 0000 0029 0672 7800  .r....rn...).rx.
+00004a00: 0000 7250 0000 0072 bf00 0000 72fc 0000  ..rP...r....r...
+00004a10: 00da 0775 6e6b 6e6f 776e 72fd 0000 0072  ...unknownr....r
+00004a20: 7900 0000 7253 0000 0072 5700 0000 72fe  y...rS...rW...r.
+00004a30: 0000 0070 0300 0073 0e00 0000 0207 1401  ...p...s........
+00004a40: 1001 0e01 1c01 0880 02ff 7a1f 4172 6775  ..........z.Argu
+00004a50: 6d65 6e74 5061 7273 6572 2e70 6172 7365  mentParser.parse
+00004a60: 5f6b 6e6f 776e 5f61 7267 73da 1873 6b69  _known_args..ski
+00004a70: 705f 7079 6461 6e74 6963 5f76 616c 6964  p_pydantic_valid
+00004a80: 6174 696f 6e63 0400 0000 0000 0000 0000  ationc..........
+00004a90: 0000 0600 0000 0500 0000 4300 0000 7322  ..........C...s"
+00004aa0: 0000 007c 00a0 007c 01a1 015c 027d 047d  ...|...|...\.}.}
+00004ab0: 057c 006a 017c 047c 027c 0364 018d 037c  .|.j.|.|.|.d...|
+00004ac0: 0566 0253 0029 0261 c902 0000 5573 6520  .f.S.).a....Use 
+00004ad0: 7061 7273 6564 2061 7267 7320 746f 2069  parsed args to i
+00004ae0: 6e73 7461 6e74 6961 7465 2074 6865 2067  nstantiate the g
+00004af0: 6976 656e 2064 6174 6120 6d6f 6465 6c2e  iven data model.
+00004b00: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00004b10: 2020 2020 2020 2020 2020 2020 6172 6773              args
+00004b20: 3a0a 2020 2020 2020 2020 2020 2020 6172  :.            ar
+00004b30: 6773 5f6d 6f64 656c 3a0a 2020 2020 2020  gs_model:.      
+00004b40: 2020 2020 2020 736b 6970 5f70 7964 616e        skip_pydan
+00004b50: 7469 635f 7661 6c69 6461 7469 6f6e 3a0a  tic_validation:.
+00004b60: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
+00004b70: 733a 0a20 2020 2020 2020 2020 2020 203e  s:.            >
+00004b80: 3e3e 2069 6d70 6f72 7420 7961 7078 0a20  >> import yapx. 
+00004b90: 2020 2020 2020 2020 2020 203e 3e3e 2066             >>> f
+00004ba0: 726f 6d20 6461 7461 636c 6173 7365 7320  rom dataclasses 
+00004bb0: 696d 706f 7274 2064 6174 6163 6c61 7373  import dataclass
+00004bc0: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+00004bd0: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+00004be0: 2040 6461 7461 636c 6173 730a 2020 2020   @dataclass.    
+00004bf0: 2020 2020 2020 2020 2e2e 2e20 636c 6173          ... clas
+00004c00: 7320 4164 644e 756d 733a 0a20 2020 2020  s AddNums:.     
+00004c10: 2020 2020 2020 202e 2e2e 2020 2020 2078         ...     x
+00004c20: 3a20 696e 740a 2020 2020 2020 2020 2020  : int.          
+00004c30: 2020 2e2e 2e20 2020 2020 793a 2069 6e74    ...     y: int
+00004c40: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+00004c50: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+00004c60: 2070 6172 7365 7220 3d20 7961 7078 2e41   parser = yapx.A
+00004c70: 7267 756d 656e 7450 6172 7365 7228 290a  rgumentParser().
+00004c80: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00004c90: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
+00004ca0: 656e 7473 2841 6464 4e75 6d73 290a 2020  ents(AddNums).  
+00004cb0: 2020 2020 2020 2020 2020 3e3e 3e20 7061            >>> pa
+00004cc0: 7273 6564 2c20 756e 6b6e 6f77 6e20 3d20  rsed, unknown = 
+00004cd0: 7061 7273 6572 2e70 6172 7365 5f6b 6e6f  parser.parse_kno
+00004ce0: 776e 5f61 7267 735f 746f 5f6d 6f64 656c  wn_args_to_model
+00004cf0: 285b 272d 7827 2c20 2731 272c 2027 2d79  (['-x', '1', '-y
+00004d00: 272c 2027 3227 2c20 272d 7a27 2c20 2733  ', '2', '-z', '3
+00004d10: 275d 290a 2020 2020 2020 2020 2020 2020  ']).            
+00004d20: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+00004d30: 3e3e 3e20 2870 6172 7365 642e 782c 2070  >>> (parsed.x, p
+00004d40: 6172 7365 642e 7929 0a20 2020 2020 2020  arsed.y).       
+00004d50: 2020 2020 2028 312c 2032 290a 2020 2020       (1, 2).    
+00004d60: 2020 2020 2020 2020 3e3e 3e20 756e 6b6e          >>> unkn
+00004d70: 6f77 6e0a 2020 2020 2020 2020 2020 2020  own.            
+00004d80: 5b27 2d7a 272c 2027 3327 5d0a 0a20 2020  ['-z', '3']..   
+00004d90: 2020 2020 20a9 0372 5000 0000 728f 0000       ..rP...r...
+00004da0: 0072 0001 0000 2902 72fe 0000 00da 145f  .r....).r......_
+00004db0: 7061 7273 655f 6172 6773 5f74 6f5f 6d6f  parse_args_to_mo
+00004dc0: 6465 6c29 0672 7800 0000 7250 0000 0072  del).rx...rP...r
+00004dd0: 8f00 0000 7200 0100 00da 0b70 6172 7365  ....r......parse
+00004de0: 645f 6172 6773 da0c 756e 6b6e 6f77 6e5f  d_args..unknown_
+00004df0: 6172 6773 7253 0000 0072 5300 0000 7257  argsrS...rS...rW
+00004e00: 0000 00da 1970 6172 7365 5f6b 6e6f 776e  .....parse_known
+00004e10: 5f61 7267 735f 746f 5f6d 6f64 656c 7d03  _args_to_model}.
+00004e20: 0000 7310 0000 000e 2304 0302 0102 0102  ..s.....#.......
+00004e30: 0104 fd02 0504 fa7a 2841 7267 756d 656e  .......z(Argumen
+00004e40: 7450 6172 7365 722e 7061 7273 655f 6b6e  tParser.parse_kn
+00004e50: 6f77 6e5f 6172 6773 5f74 6f5f 6d6f 6465  own_args_to_mode
+00004e60: 6c63 0400 0000 0000 0000 0000 0000 0500  lc..............
+00004e70: 0000 0500 0000 4300 0000 731a 0000 007c  ......C...s....|
+00004e80: 00a0 007c 01a1 017d 047c 006a 017c 047c  ...|...}.|.j.|.|
+00004e90: 027c 0364 018d 0353 0029 0261 7f02 0000  .|.d...S.).a....
+00004ea0: 5573 6520 7061 7273 6564 2061 7267 7320  Use parsed args 
+00004eb0: 746f 2069 6e73 7461 6e74 6961 7465 2074  to instantiate t
+00004ec0: 6865 2067 6976 656e 2064 6174 6120 6d6f  he given data mo
+00004ed0: 6465 6c2e 0a0a 2020 2020 2020 2020 4172  del...        Ar
+00004ee0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00004ef0: 6172 6773 3a0a 2020 2020 2020 2020 2020  args:.          
+00004f00: 2020 6172 6773 5f6d 6f64 656c 3a0a 2020    args_model:.  
+00004f10: 2020 2020 2020 2020 2020 736b 6970 5f70            skip_p
+00004f20: 7964 616e 7469 635f 7661 6c69 6461 7469  ydantic_validati
+00004f30: 6f6e 3a0a 0a20 2020 2020 2020 2045 7861  on:..        Exa
+00004f40: 6d70 6c65 733a 0a20 2020 2020 2020 2020  mples:.         
+00004f50: 2020 203e 3e3e 2069 6d70 6f72 7420 7961     >>> import ya
+00004f60: 7078 0a20 2020 2020 2020 2020 2020 203e  px.            >
+00004f70: 3e3e 2066 726f 6d20 6461 7461 636c 6173  >> from dataclas
+00004f80: 7365 7320 696d 706f 7274 2064 6174 6163  ses import datac
+00004f90: 6c61 7373 0a20 2020 2020 2020 2020 2020  lass.           
+00004fa0: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
+00004fb0: 203e 3e3e 2040 6461 7461 636c 6173 730a   >>> @dataclass.
+00004fc0: 2020 2020 2020 2020 2020 2020 2e2e 2e20              ... 
+00004fd0: 636c 6173 7320 4164 644e 756d 733a 0a20  class AddNums:. 
+00004fe0: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
+00004ff0: 2020 2078 3a20 696e 740a 2020 2020 2020     x: int.      
+00005000: 2020 2020 2020 2e2e 2e20 2020 2020 793a        ...     y:
+00005010: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
+00005020: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
+00005030: 203e 3e3e 2070 6172 7365 7220 3d20 7961   >>> parser = ya
+00005040: 7078 2e41 7267 756d 656e 7450 6172 7365  px.ArgumentParse
+00005050: 7228 290a 2020 2020 2020 2020 2020 2020  r().            
+00005060: 3e3e 3e20 7061 7273 6572 2e61 6464 5f61  >>> parser.add_a
+00005070: 7267 756d 656e 7473 2841 6464 4e75 6d73  rguments(AddNums
+00005080: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
+00005090: 3e20 7061 7273 6564 203d 2070 6172 7365  > parsed = parse
+000050a0: 722e 7061 7273 655f 6172 6773 5f74 6f5f  r.parse_args_to_
+000050b0: 6d6f 6465 6c28 5b27 2d78 272c 2027 3127  model(['-x', '1'
+000050c0: 2c20 272d 7927 2c20 2732 275d 290a 2020  , '-y', '2']).  
+000050d0: 2020 2020 2020 2020 2020 2e2e 2e0a 2020            ....  
+000050e0: 2020 2020 2020 2020 2020 3e3e 3e20 2870            >>> (p
+000050f0: 6172 7365 642e 782c 2070 6172 7365 642e  arsed.x, parsed.
+00005100: 7929 0a20 2020 2020 2020 2020 2020 2028  y).            (
+00005110: 312c 2032 290a 0a20 2020 2020 2020 2072  1, 2)..        r
+00005120: 0101 0000 2902 72fa 0000 0072 0201 0000  ....).r....r....
+00005130: 2905 7278 0000 0072 5000 0000 728f 0000  ).rx...rP...r...
+00005140: 0072 0001 0000 7203 0100 0072 5300 0000  .r....r....rS...
+00005150: 7253 0000 0072 5700 0000 da13 7061 7273  rS...rW.....pars
+00005160: 655f 6172 6773 5f74 6f5f 6d6f 6465 6cab  e_args_to_model.
+00005170: 0300 0073 0c00 0000 0a1e 0401 0201 0201  ...s............
+00005180: 0201 06fd 7a22 4172 6775 6d65 6e74 5061  ....z"ArgumentPa
+00005190: 7273 6572 2e70 6172 7365 5f61 7267 735f  rser.parse_args_
+000051a0: 746f 5f6d 6f64 656c 6304 0000 0000 0000  to_modelc.......
+000051b0: 0000 0000 0008 0000 000a 0000 0043 0000  .............C..
+000051c0: 0073 aa00 0000 7400 7c01 8301 7d04 7c02  .s....t.|...}.|.
+000051d0: 7310 7c04 a001 7c00 6a02 a101 7d02 7c02  s.|...|.j...}.|.
+000051e0: 7310 7403 8201 7c00 6a04 7c04 7c02 6401  s.t...|.j.|.|.d.
+000051f0: 8d02 7d05 7405 724e 7c03 734e 7a0d 7400  ..}.t.rN|.sNz.t.
+00005200: 7406 7c02 8301 6405 6900 7c05 a401 8e01  t.|...d.i.|.....
+00005210: 8301 7d05 5700 6e25 0400 7407 794d 0100  ..}.W.n%..t.yM..
+00005220: 7d06 0100 7a19 6402 6402 a008 6403 6404  }...z.d.d...d.d.
+00005230: 8400 7c06 a009 a100 4400 8301 a101 1700  ..|.....D.......
+00005240: 7d07 7c00 a00a 7c07 a101 0100 5700 5900  }.|...|.....W.Y.
+00005250: 6400 7d06 7e06 6e05 6400 7d06 7e06 7701  d.}.~.n.d.}.~.w.
+00005260: 7700 7c02 6405 6900 7c05 a401 8e01 5300  w.|.d.i.|.....S.
+00005270: 2906 4ea9 02da 0961 7267 735f 6469 6374  ).N....args_dict
+00005280: 728f 0000 0072 7d00 0000 6301 0000 0000  r....r}...c.....
+00005290: 0000 0000 0000 0002 0000 0006 0000 0073  ...............s
+000052a0: 0000 0073 2e00 0000 8100 7c00 5d12 7d01  ...s......|.].}.
+000052b0: 6400 7c01 6401 1900 6402 1900 9b00 6403  d.|.d...d.....d.
+000052c0: 7c01 6404 1900 9b00 6405 9d05 5600 0100  |.d.....d...V...
+000052d0: 7102 6406 5300 2907 7a18 4572 726f 7220  q.d.S.).z.Error 
+000052e0: 7061 7273 696e 6720 6172 6775 6d65 6e74  parsing argument
+000052f0: 2060 da03 6c6f 6372 0100 0000 7a03 603b   `..locr....z.`;
+00005300: 20da 036d 7367 72ac 0000 004e 7253 0000   ..msgr....NrS..
+00005310: 0072 5400 0000 7253 0000 0072 5300 0000  .rT...rS...rS...
+00005320: 7257 0000 00da 093c 6765 6e65 7870 723e  rW.....<genexpr>
+00005330: e903 0000 730a 0000 0002 8004 0002 021c  ....s...........
+00005340: ff0a ff7a 3641 7267 756d 656e 7450 6172  ...z6ArgumentPar
+00005350: 7365 722e 5f70 6172 7365 5f61 7267 735f  ser._parse_args_
+00005360: 746f 5f6d 6f64 656c 2e3c 6c6f 6361 6c73  to_model.<locals
+00005370: 3e2e 3c67 656e 6578 7072 3e72 5300 0000  >.<genexpr>rS...
+00005380: 290b 72f7 0000 0072 aa00 0000 7246 0000  ).r....r....rF..
+00005390: 0072 2600 0000 da16 5f75 6e69 6f6e 5f61  .r&....._union_a
+000053a0: 7267 735f 7769 7468 5f6d 6f64 656c 7235  rgs_with_modelr5
+000053b0: 0000 0072 3300 0000 722e 0000 0072 dc00  ...r3...r....r..
+000053c0: 0000 da06 6572 726f 7273 7282 0000 0029  ....errorsr....)
+000053d0: 0872 7800 0000 7250 0000 0072 8f00 0000  .rx...rP...r....
+000053e0: 7200 0100 0072 0301 0000 5a0a 6172 6773  r....r....Z.args
+000053f0: 5f75 6e69 6f6e 72fd 0000 0072 df00 0000  _unionr....r....
+00005400: 7253 0000 0072 5300 0000 7257 0000 0072  rS...rS...rW...r
+00005410: 0201 0000 d003 0000 732c 0000 0008 0604  ........s,......
+00005420: 020c 0104 0104 0104 0202 0102 0106 fe08  ................
+00005430: 0502 0202 0110 0108 ff0e 030c 0106 020a  ................
+00005440: fe16 0408 8002 fb0e 077a 2341 7267 756d  .........z#Argum
+00005450: 656e 7450 6172 7365 722e 5f70 6172 7365  entParser._parse
+00005460: 5f61 7267 735f 746f 5f6d 6f64 656c 7208  _args_to_modelr.
+00005470: 0100 0063 0200 0000 0000 0000 0000 0000  ...c............
+00005480: 0200 0000 0300 0000 0300 0000 7316 0000  ............s...
+00005490: 0087 0066 0164 0164 0284 087c 00a0 00a1  ...f.d.d...|....
+000054a0: 0044 0083 0153 0029 034e 6301 0000 0000  .D...S.).Nc.....
+000054b0: 0000 0000 0000 0003 0000 0004 0000 0013  ................
+000054c0: 0000 0073 2000 0000 6900 7c00 5d0c 5c02  ...s ...i.|.].\.
+000054d0: 7d01 7d02 7c01 8800 6a00 7600 7202 7c01  }.}.|...j.v.r.|.
+000054e0: 7c02 9302 7102 5300 7253 0000 0072 a100  |...q.S.rS...r..
+000054f0: 0000 a903 7255 0000 0072 e100 0000 da01  ....rU...r......
+00005500: 7672 9400 0000 7253 0000 0072 5700 0000  vr....rS...rW...
+00005510: da0a 3c64 6963 7463 6f6d 703e f603 0000  ..<dictcomp>....
+00005520: 7261 0000 007a 3941 7267 756d 656e 7450  ra...z9ArgumentP
+00005530: 6172 7365 722e 5f75 6e69 6f6e 5f61 7267  arser._union_arg
+00005540: 735f 7769 7468 5f6d 6f64 656c 2e3c 6c6f  s_with_model.<lo
+00005550: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
+00005560: 2901 728d 0000 0072 0701 0000 7253 0000  ).r....r....rS..
+00005570: 0072 9400 0000 7257 0000 0072 0c01 0000  .r....rW...r....
+00005580: f103 0000 7302 0000 0016 057a 2541 7267  ....s......z%Arg
+00005590: 756d 656e 7450 6172 7365 722e 5f75 6e69  umentParser._uni
+000055a0: 6f6e 5f61 7267 735f 7769 7468 5f6d 6f64  on_args_with_mod
+000055b0: 656c 6302 0000 0000 0000 0000 0000 0006  elc.............
+000055c0: 0000 0004 0000 0043 0000 0073 8000 0000  .......C...s....
+000055d0: 6400 7d02 7c01 6a00 7215 7c01 6a00 a001  d.}.|.j.r.|.j...
+000055e0: 7c01 6a02 6401 1700 a101 7315 7c01 6a00  |.j.d.....s.|.j.
+000055f0: a003 a100 a004 a100 7d02 7c02 7319 6400  ........}.|.s.d.
+00005600: 5300 6402 7d03 7405 7c02 8301 4400 5d0c  S.d.}.t.|...D.].
+00005610: 5c02 7d04 7d05 7c05 a003 a100 732b 7c04  \.}.}.|.....s+|.
+00005620: 7d03 0100 6e01 711f 7c03 6402 6b04 7236  }...n.q.|.d.k.r6
+00005630: 7c02 6400 7c03 8502 1900 7d02 6403 a006  |.d.|.....}.d...
+00005640: 6404 6405 8400 7c02 4400 8301 a101 5300  d.d...|.D.....S.
+00005650: 2906 4efa 0128 7201 0000 0072 7d00 0000  ).N..(r....r}...
+00005660: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00005670: 0003 0000 0073 0000 0073 1800 0000 8100  .....s...s......
+00005680: 7c00 5d07 7d01 7c01 a000 a100 5600 0100  |.].}.|.....V...
+00005690: 7102 6400 5300 725c 0000 0029 01da 0573  q.d.S.r\...)...s
+000056a0: 7472 6970 7254 0000 0072 5300 0000 7253  triprT...rS...rS
+000056b0: 0000 0072 5700 0000 720b 0100 0010 0400  ...rW...r.......
+000056c0: 0073 0400 0000 0280 1600 7a41 4172 6775  .s........zAArgu
+000056d0: 6d65 6e74 5061 7273 6572 2e5f 6765 745f  mentParser._get_
+000056e0: 6465 7363 7269 7074 696f 6e5f 6672 6f6d  description_from
+000056f0: 5f64 6f63 7374 7269 6e67 2e3c 6c6f 6361  _docstring.<loca
+00005700: 6c73 3e2e 3c67 656e 6578 7072 3e29 07da  ls>.<genexpr>)..
+00005710: 075f 5f64 6f63 5f5f 7260 0000 0072 9500  .__doc__r`...r..
+00005720: 0000 7212 0100 0072 9900 0000 da09 656e  ..r....r......en
+00005730: 756d 6572 6174 6572 dc00 0000 2906 72a7  umerater....).r.
+00005740: 0000 0072 8f00 0000 5a11 6465 7363 7269  ...r....Z.descri
+00005750: 7074 696f 6e5f 6c69 6e65 735a 1274 6578  ption_linesZ.tex
+00005760: 745f 626c 6f63 6b5f 656e 6473 5f61 74da  t_block_ends_at.
+00005770: 0169 da04 6c69 6e65 7253 0000 0072 5300  .i..linerS...rS.
+00005780: 0000 7257 0000 0072 9800 0000 f803 0000  ..rW...r........
+00005790: 7320 0000 0004 050c 0208 0104 ff0e 0304  s ..............
+000057a0: 0204 0104 0210 0108 0104 0104 0102 fe08  ................
+000057b0: 040c 0114 027a 2e41 7267 756d 656e 7450  .....z.ArgumentP
+000057c0: 6172 7365 722e 5f67 6574 5f64 6573 6372  arser._get_descr
+000057d0: 6970 7469 6f6e 5f66 726f 6d5f 646f 6373  iption_from_docs
+000057e0: 7472 696e 6763 0300 0000 0000 0000 0000  tringc..........
+000057f0: 0000 0400 0000 0300 0000 4300 0000 731c  ..........C...s.
+00005800: 0000 007c 00a0 007c 02a1 017d 037c 0372  ...|...|...}.|.r
+00005810: 0c7c 037c 015f 0164 0053 0064 0053 0072  .|.|._.d.S.d.S.r
+00005820: 5c00 0000 2902 7298 0000 0072 4900 0000  \...).r....rI...
+00005830: 2904 72a7 0000 0072 6600 0000 728f 0000  ).r....rf...r...
+00005840: 0072 4900 0000 7253 0000 0072 5300 0000  .rI...rS...rS...
+00005850: 7257 0000 00da 1f5f 7365 745f 6465 7363  rW....._set_desc
+00005860: 7269 7074 696f 6e5f 6672 6f6d 5f64 6f63  ription_from_doc
+00005870: 7374 7269 6e67 1204 0000 7308 0000 000a  string....s.....
+00005880: 0604 020a 0104 ff7a 2e41 7267 756d 656e  .......z.Argumen
+00005890: 7450 6172 7365 722e 5f73 6574 5f64 6573  tParser._set_des
+000058a0: 6372 6970 7469 6f6e 5f66 726f 6d5f 646f  cription_from_do
+000058b0: 6373 7472 696e 67da 0b6c 696e 6b65 645f  cstring..linked_
+000058c0: 6675 6e63 da0b 7265 6c61 795f 7661 6c75  func..relay_valu
+000058d0: 6563 0700 0000 0000 0000 0000 0000 1700  ec..............
+000058e0: 0000 0700 0000 0300 0000 73e6 0100 0067  ..........s....g
+000058f0: 007d 0769 007d 0864 017d 0964 017d 0a64  .}.i.}.d.}.d.}.d
+00005900: 017d 0b64 017d 0c64 017d 0d74 007c 0283  .}.d.}.d.}.t.|..
+00005910: 016a 01a0 02a1 0044 005d 437d 0e74 037c  .j.....D.]C}.t.|
+00005920: 0e83 01a0 0464 02a1 0172 2164 037d 0c71  .....d...r!d.}.q
+00005930: 1574 037c 0e83 01a0 0464 04a1 0172 2b64  .t.|.....d...r+d
+00005940: 037d 0a71 157c 0e6a 0564 056b 0272 3364  .}.q.|.j.d.k.r3d
+00005950: 037d 0b71 157c 0e6a 0564 066b 0272 3b64  .}.q.|.j.d.k.r;d
+00005960: 037d 0d71 157c 0e6a 0564 076b 0272 457c  .}.q.|.j.d.k.rE|
+00005970: 037c 0864 073c 0071 157c 0e6a 0564 086b  .|.d.<.q.|.j.d.k
+00005980: 0272 4f7c 067c 0864 083c 0071 157c 0e6a  .rO|.|.d.<.q.|.j
+00005990: 0564 096b 0272 5864 037c 0864 093c 0071  .d.k.rXd.|.d.<.q
+000059a0: 157c 0a70 607c 0c70 607c 0b70 607c 0d7d  .|.p`|.p`|.p`|.}
+000059b0: 097c 0973 737c 0572 7374 0664 0a64 0b84  .|.ss|.rst.d.d..
+000059c0: 0074 007c 0583 016a 01a0 02a1 0044 0083  .t.|...j.....D..
+000059d0: 0183 017d 097c 0473 7974 077c 0283 017d  ...}.|.syt.|...}
+000059e0: 047c 0972 e17c 016a 087c 037c 0464 0c8d  .|.r.|.j.|.|.d..
+000059f0: 025c 027d 0f7d 107c 0c73 887c 0d72 d669  .\.}.}.|.s.|.r.i
+00005a00: 0089 007c 0083 007d 117c 1044 005d 247d  ...|...}.|.D.]$}
+00005a10: 127c 12a0 0464 0da1 0172 b37c 126a 0964  .|...d...r.|.j.d
+00005a20: 0e64 0f64 108d 0264 1119 007d 137c 13a0  .d.d...d...}.|..
+00005a30: 0a64 0da1 017d 147c 1472 b37c 116a 0b7c  .d...}.|.r.|.j.|
+00005a40: 1364 1264 0064 0164 138d 0401 007c 1388  .d.d.d.d.....|..
+00005a50: 007c 143c 0071 8f7c 116a 0c7c 1064 148d  .|.<.q.|.j.|.d..
+00005a60: 015c 027d 157d 1087 0066 0164 1564 1684  .\.}.}...f.d.d..
+00005a70: 0874 0d7c 1583 01a0 0ea1 0044 0083 017d  .t.|.......D...}
+00005a80: 167c 0c72 d07c 08a0 0f7c 16a1 0101 007c  .|.r.|...|.....|
+00005a90: 0d72 d67c 167c 0864 063c 007c 0a72 da7c  .r.|.|.d.<.|.r.|
+00005aa0: 107d 077c 0b72 e07c 107c 0864 053c 006e  .}.|.r.|.|.d.<.n
+00005ab0: 077c 016a 107c 037c 0464 0c8d 027d 0f7c  .|.j.|.|.d...}.|
+00005ac0: 027c 0769 0074 0d7c 0f83 01a4 017c 08a4  .|.i.t.|.....|..
+00005ad0: 018e 0153 0029 174e 467a 022a 2a54 72b3  ...S.).NFz.**Tr.
+00005ae0: 0000 00da 0b5f 6578 7472 615f 6172 6773  ....._extra_args
+00005af0: da0d 5f65 7874 7261 5f6b 7761 7267 735a  .._extra_kwargsZ
+00005b00: 095f 616c 6c5f 6172 6773 5a0c 5f72 656c  ._all_argsZ._rel
+00005b10: 6179 5f76 616c 7565 5a10 5f63 616c 6c65  ay_valueZ._calle
+00005b20: 645f 6672 6f6d 5f63 6c69 6301 0000 0000  d_from_clic.....
+00005b30: 0000 0000 0000 0002 0000 0004 0000 0073  ...............s
+00005b40: 0000 0073 2800 0000 8100 7c00 5d0f 7d01  ...s(.....|.].}.
+00005b50: 7400 7c01 8301 a001 6400 a101 700f 7c01  t.|.....d...p.|.
+00005b60: 6a02 6401 7600 5600 0100 7102 6402 5300  j.d.v.V...q.d.S.
+00005b70: 2903 72b3 0000 0029 0272 1a01 0000 721b  ).r....).r....r.
+00005b80: 0100 004e 2903 726e 0000 0072 6000 0000  ...N).rn...r`...
+00005b90: 7292 0000 0029 0272 5500 0000 da01 7072  r....).rU.....pr
+00005ba0: 5300 0000 7253 0000 0072 5700 0000 720b  S...rS...rW...r.
+00005bb0: 0100 0047 0400 0073 0a00 0000 0280 0400  ...G...s........
+00005bc0: 0202 16ff 0aff 7a2b 4172 6775 6d65 6e74  ......z+Argument
+00005bd0: 5061 7273 6572 2e5f 7275 6e5f 6675 6e63  Parser._run_func
+00005be0: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
+00005bf0: 7072 3e29 0272 5000 0000 728f 0000 0072  pr>).rP...r....r
+00005c00: 6500 0000 725b 0000 0072 1700 0000 72ad  e...r[...r....r.
+00005c10: 0000 0072 0100 0000 72bb 0000 0029 0372  ...r....r....).r
+00005c20: ba00 0000 7263 0000 0072 b900 0000 2901  ....rc...r....).
+00005c30: 7250 0000 0063 0100 0000 0000 0000 0000  rP...c..........
+00005c40: 0000 0300 0000 0400 0000 1300 0000 731a  ..............s.
+00005c50: 0000 0069 007c 005d 095c 027d 017d 0288  ...i.|.].\.}.}..
+00005c60: 007c 0119 007c 0293 0271 0253 0072 5300  .|...|...q.S.rS.
+00005c70: 0000 7253 0000 0072 0e01 0000 a901 5a10  ..rS...r......Z.
+00005c80: 756e 6b6e 6f77 6e5f 6e61 6d65 5f6d 6170  unknown_name_map
+00005c90: 7253 0000 0072 5700 0000 7210 0100 006b  rS...rW...r....k
+00005ca0: 0400 0073 0600 0000 0600 0e01 06ff 7a2c  ...s..........z,
+00005cb0: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
+00005cc0: 7275 6e5f 6675 6e63 2e3c 6c6f 6361 6c73  run_func.<locals
+00005cd0: 3e2e 3c64 6963 7463 6f6d 703e 2911 7209  >.<dictcomp>).r.
+00005ce0: 0000 00da 0a70 6172 616d 6574 6572 7372  .....parametersr
+00005cf0: c000 0000 726e 0000 0072 6000 0000 7292  ....rn...r`...r.
+00005d00: 0000 00da 0361 6e79 7225 0000 0072 0501  .....anyr%...r..
+00005d10: 0000 da05 7370 6c69 74da 066c 7374 7269  ....split..lstri
+00005d20: 7072 6f00 0000 72fe 0000 0072 f700 0000  pro...r....r....
+00005d30: 728d 0000 00da 0675 7064 6174 6572 0601  r......updater..
+00005d40: 0000 2917 72a7 0000 0072 6600 0000 729c  ..).r....rf...r.
+00005d50: 0000 0072 5000 0000 728f 0000 0072 1801  ...rP...r....r..
+00005d60: 0000 7219 0100 005a 0966 756e 635f 6172  ..r....Z.func_ar
+00005d70: 6773 5a0b 6675 6e63 5f6b 7761 7267 735a  gsZ.func_kwargsZ
+00005d80: 0d65 7874 7261 5f61 7267 735f 6f6b 5a0c  .extra_args_okZ.
+00005d90: 6163 6365 7074 735f 6172 6773 5a12 6163  accepts_argsZ.ac
+00005da0: 6365 7074 735f 6578 7472 615f 6172 6773  cepts_extra_args
+00005db0: 5a0e 6163 6365 7074 735f 6b77 6172 6773  Z.accepts_kwargs
+00005dc0: 5a14 6163 6365 7074 735f 6578 7472 615f  Z.accepts_extra_
+00005dd0: 6b77 6172 6773 721c 0100 005a 0a6d 6f64  kwargsr....Z.mod
+00005de0: 656c 5f69 6e73 7472 0401 0000 5a0e 756e  el_instr....Z.un
+00005df0: 6b6e 6f77 6e5f 7061 7273 6572 7256 0000  known_parserrV..
+00005e00: 005a 0678 5f66 6c61 675a 0b78 5f66 6c61  .Z.x_flagZ.x_fla
+00005e10: 675f 6261 7265 5a0e 7061 7273 6564 5f75  g_bareZ.parsed_u
+00005e20: 6e6b 6e6f 776e 5a0c 6578 7472 615f 6b77  nknownZ.extra_kw
+00005e30: 6172 6773 7253 0000 0072 1d01 0000 7257  argsrS...r....rW
+00005e40: 0000 00da 095f 7275 6e5f 6675 6e63 1d04  ....._run_func..
+00005e50: 0000 7390 0000 0004 0a04 0104 0204 0204  ..s.............
+00005e60: 0104 0204 0112 020e 0106 010e 0106 010a  ................
+00005e70: 0106 010a 0106 010a 010a 010a 010a 010a  ................
+00005e80: 0108 0102 800e 0302 ff08 0408 010c 0208  ................
+00005e90: fe04 0508 0104 0304 0202 0102 010a fe08  ................
+00005ea0: 0504 0106 0108 010a 0112 010a 0104 0104  ................
+00005eb0: 0102 0102 0102 0102 0106 fc08 0602 8004  ................
+00005ec0: 0202 010a ff0a 040a 0106 ff04 030a 0104  ................
+00005ed0: 0108 0104 0204 0104 0208 0102 8004 0302  ................
+00005ee0: 0102 0106 fe16 057a 1841 7267 756d 656e  .......z.Argumen
+00005ef0: 7450 6172 7365 722e 5f72 756e 5f66 756e  tParser._run_fun
+00005f00: 63da 0763 6f6d 6d61 6e64 da0b 7375 6263  c..command..subc
+00005f10: 6f6d 6d61 6e64 73da 116e 616d 6564 5f73  ommands..named_s
+00005f20: 7562 636f 6d6d 616e 6473 6304 0000 0000  ubcommandsc.....
+00005f30: 0000 0000 0000 0009 0000 000b 0000 004b  ...............K
+00005f40: 0000 0073 d200 0000 7c00 6403 6900 7c04  ...s....|.d.i.|.
+00005f50: a401 8e01 7d05 7c01 722e 7400 7c01 8301  ....}.|.r.t.|...
+00005f60: 7d06 7c00 6a01 7c05 7c06 6401 8d02 0100  }.|.j.|.|.d.....
+00005f70: 7c05 a002 7c06 a101 0100 7c05 6a03 6403  |...|.....|.j.d.
+00005f80: 6900 7c00 6a04 7c01 7c00 6a05 7c06 7c00  i.|.j.|.|.j.|.|.
+00005f90: 6a06 7c01 7c00 6a07 7c06 6904 a401 8e01  j.|.|.j.|.i.....
+00005fa0: 0100 6e14 7c05 6a03 6403 6900 7c00 6a05  ..n.|.j.d.i.|.j.
+00005fb0: 6400 7c00 6a04 6400 7c00 6a07 6400 7c00  d.|.j.d.|.j.d.|.
+00005fc0: 6a06 6400 6904 a401 8e01 0100 7c02 7255  j.d.i.......|.rU
+00005fd0: 7408 7c02 8301 724b 7c02 6701 7d02 7c02  t.|...rK|.g.}.|.
+00005fe0: 4400 5d07 7d07 7c05 a009 7c07 a101 0100  D.].}.|...|.....
+00005ff0: 714d 7c03 7267 7c03 a00a a100 4400 5d0b  qM|.rg|.....D.].
+00006000: 5c02 7d08 7d07 7c05 6a09 7c07 7c08 6402  \.}.}.|.j.|.|.d.
+00006010: 8d02 0100 715b 7c05 5300 2904 4e29 0272  ....q[|.S.).N).r
+00006020: 6600 0000 728f 0000 0072 b100 0000 7253  f...r....r....rS
+00006030: 0000 0029 0b72 2500 0000 7217 0100 0072  ...).r%...r....r
+00006040: 9100 0000 729d 0000 0072 4200 0000 7243  ....r....rB...rC
+00006050: 0000 0072 4500 0000 7246 0000 00da 0863  ...rE...rF.....c
+00006060: 616c 6c61 626c 6572 9e00 0000 728d 0000  allabler....r...
+00006070: 0029 0972 a700 0000 7224 0100 0072 2501  .).r....r$...r%.
+00006080: 0000 7226 0100 0072 5100 0000 7266 0000  ..r&...rQ...rf..
+00006090: 005a 0e72 6f6f 745f 6172 675f 6d6f 6465  .Z.root_arg_mode
+000060a0: 6c72 5600 0000 7292 0000 0072 5300 0000  lrV...r....rS...
+000060b0: 7253 0000 0072 5700 0000 da0d 5f62 7569  rS...rW....._bui
+000060c0: 6c64 5f70 6172 7365 7281 0400 0073 3e00  ld_parser....s>.
+000060d0: 0000 0e08 0402 0801 0401 0201 0201 06fe  ................
+000060e0: 0a04 0801 0602 0601 0601 0601 02fc 08ff  ................
+000060f0: 0809 0602 0601 0601 0601 02fc 06ff 0409  ................
+00006100: 0801 0601 0801 0c01 0402 1001 1001 0402  ................
+00006110: 7a1c 4172 6775 6d65 6e74 5061 7273 6572  z.ArgumentParser
+00006120: 2e5f 6275 696c 645f 7061 7273 6572 2902  ._build_parser).
+00006130: 7250 0000 00da 0c64 6566 6175 6c74 5f61  rP.....default_a
+00006140: 7267 73da 0b70 6172 7365 725f 6172 6773  rgs..parser_args
+00006150: 7229 0100 00da 0d70 6172 7365 725f 6b77  r).....parser_kw
+00006160: 6172 6773 6301 0000 0000 0000 0002 0000  argsc...........
+00006170: 0011 0000 0009 0000 004f 0000 0073 3801  .........O...s8.
+00006180: 0000 7c00 6a00 7c03 6900 7c04 a401 8e01  ..|.j.|.i.|.....
+00006190: 7d05 7c01 6401 7500 7213 7401 6a02 6402  }.|.d.u.r.t.j.d.
+000061a0: 6401 8502 1900 7d01 7c01 7319 7c02 7219  d.....}.|.s.|.r.
+000061b0: 7c02 7d01 7c05 a003 7c01 a101 5c02 7d06  |.}.|...|...\.}.
+000061c0: 7d07 7404 7c06 8301 7d08 7c08 a005 7c00  }.t.|...}.|...|.
+000061d0: 6a06 a101 7d09 7c08 a005 7c00 6a07 a101  j...}.|...|.j...
+000061e0: 7d0a 7c08 a005 7c00 6a08 a101 7d0b 7c08  }.|...|.j...}.|.
+000061f0: a005 7c00 6a09 a101 7d0c 7c08 a005 7c00  ..|.j...}.|...|.
+00006200: 6a0a a101 7d0d 6401 7d0e 6401 7d0f 7c09  j...}.d.}.d.}.|.
+00006210: 7252 7c00 6a0b 7c05 7c09 7c0a 7c0c 7c01  rR|.j.|.|.|.|.|.
+00006220: 6403 8d05 7d0f 740c 7c0f 740d 8302 7269  d...}.t.|.t...ri
+00006230: 7a06 740e 7c0f 8301 7d0e 5700 6e0d 0400  z.t.|...}.W.n...
+00006240: 740f 7968 0100 0100 0100 7c0f 7d0e 5900  t.yh......|.}.Y.
+00006250: 6e03 7700 7c0f 7d0e 7a20 7c0b 727b 7c0c  n.w.|.}.z |.r{|.
+00006260: 727b 7c00 6a0b 7c05 7c0c 7c0d 7c01 7c09  r{|.j.|.|.|.|.|.
+00006270: 7c0e 6404 8d06 7d0e 5700 740c 7c0f 740d  |.d...}.W.t.|.t.
+00006280: 8302 728a 7c0f 4400 5d06 7d10 7c0c 7389  ..r.|.D.].}.|.s.
+00006290: 7c10 7d0e 7183 7c0e 5300 740c 7c0f 740d  |.}.q.|.S.t.|.t.
+000062a0: 8302 729a 7c0f 4400 5d07 7d10 7c0c 7399  ..r.|.D.].}.|.s.
+000062b0: 7c10 7d0e 7193 7700 7700 2905 612d 0300  |.}.q.w.w.).a-..
+000062c0: 0055 7365 2067 6976 656e 2066 756e 6374  .Use given funct
+000062d0: 696f 6e73 2074 6f20 636f 6e73 7472 7563  ions to construc
+000062e0: 7420 6120 434c 492c 2070 6172 7365 2074  t a CLI, parse t
+000062f0: 6865 2061 7267 732c 2061 6e64 2069 6e76  he args, and inv
+00006300: 6f6b 6520 7468 6520 6170 7072 6f70 7269  oke the appropri
+00006310: 6174 6520 636f 6d6d 616e 642e 0a0a 2020  ate command...  
+00006320: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00006330: 2020 2020 2020 2020 2a70 6172 7365 725f          *parser_
+00006340: 6172 6773 3a0a 2020 2020 2020 2020 2020  args:.          
+00006350: 2020 6172 6773 3a0a 2020 2020 2020 2020    args:.        
+00006360: 2020 2020 6465 6661 756c 745f 6172 6773      default_args
+00006370: 3a0a 2020 2020 2020 2020 2020 2020 2a2a  :.            **
+00006380: 7061 7273 6572 5f6b 7761 7267 733a 0a0a  parser_kwargs:..
+00006390: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
+000063a0: 733a 0a20 2020 2020 2020 2020 2020 203e  s:.            >
+000063b0: 3e3e 2069 6d70 6f72 7420 7961 7078 0a20  >> import yapx. 
+000063c0: 2020 2020 2020 2020 2020 202e 2e2e 0a20             .... 
+000063d0: 2020 2020 2020 2020 2020 203e 3e3e 2064             >>> d
+000063e0: 6566 2070 7269 6e74 5f6e 756d 7328 2a61  ef print_nums(*a
+000063f0: 7267 7329 3a0a 2020 2020 2020 2020 2020  rgs):.          
+00006400: 2020 2e2e 2e20 2020 2020 7072 696e 7428    ...     print(
+00006410: 2741 7267 733a 2027 2c20 2a61 7267 7329  'Args: ', *args)
+00006420: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+00006430: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+00006440: 2064 6566 2066 696e 645f 6576 656e 7328   def find_evens(
+00006450: 2a61 7267 7329 3a0a 2020 2020 2020 2020  *args):.        
+00006460: 2020 2020 2e2e 2e20 2020 2020 7265 7475      ...     retu
+00006470: 726e 205b 7820 666f 7220 7820 696e 2061  rn [x for x in a
+00006480: 7267 7320 6966 2069 6e74 2878 2920 2520  rgs if int(x) % 
+00006490: 3220 3d3d 2030 5d0a 2020 2020 2020 2020  2 == 0].        
+000064a0: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
+000064b0: 2020 2020 3e3e 3e20 6465 6620 6669 6e64      >>> def find
+000064c0: 5f6f 6464 7328 2a61 7267 7329 3a0a 2020  _odds(*args):.  
+000064d0: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
+000064e0: 2020 7265 7475 726e 205b 7820 666f 7220    return [x for 
+000064f0: 7820 696e 2061 7267 7320 6966 2069 6e74  x in args if int
+00006500: 2878 2920 2520 3220 213d 2030 5d0a 2020  (x) % 2 != 0].  
+00006510: 2020 2020 2020 2020 2020 2e2e 2e0a 2020            ....  
+00006520: 2020 2020 2020 2020 2020 3e3e 3e20 636c            >>> cl
+00006530: 695f 6172 6773 203d 205b 2766 696e 642d  i_args = ['find-
+00006540: 6f64 6473 272c 2027 3127 2c20 2732 272c  odds', '1', '2',
+00006550: 2027 3327 2c20 2734 272c 2027 3527 5d0a   '3', '4', '5'].
+00006560: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00006570: 7961 7078 2e72 756e 2870 7269 6e74 5f6e  yapx.run(print_n
+00006580: 756d 732c 205b 6669 6e64 5f65 7665 6e73  ums, [find_evens
+00006590: 2c20 6669 6e64 5f6f 6464 735d 2c20 6172  , find_odds], ar
+000065a0: 6773 3d63 6c69 5f61 7267 7329 0a20 2020  gs=cli_args).   
+000065b0: 2020 2020 2020 2020 2041 7267 733a 2020           Args:  
+000065c0: 3120 3220 3320 3420 350a 2020 2020 2020  1 2 3 4 5.      
+000065d0: 2020 2020 2020 5b27 3127 2c20 2733 272c        ['1', '3',
+000065e0: 2027 3527 5d0a 2020 2020 2020 2020 4e72   '5'].        Nr
+000065f0: 1700 0000 2905 7266 0000 0072 9c00 0000  ....).rf...r....
+00006600: 728f 0000 0072 1801 0000 7250 0000 0029  r....r....rP...)
+00006610: 0672 6600 0000 729c 0000 0072 8f00 0000  .rf...r....r....
+00006620: 7250 0000 0072 1801 0000 7219 0100 0029  rP...r....r....)
+00006630: 1072 2801 0000 727f 0000 00da 0461 7267  .r(...r......arg
+00006640: 7672 fe00 0000 72f7 0000 0072 aa00 0000  vr....r....r....
+00006650: 7242 0000 0072 4300 0000 7244 0000 0072  rB...rC...rD...r
+00006660: 4500 0000 7246 0000 0072 2301 0000 7238  E...rF...r#...r8
+00006670: 0000 0072 0a00 0000 da04 6e65 7874 da0d  ...r......next..
+00006680: 5374 6f70 4974 6572 6174 696f 6e29 1172  StopIteration).r
+00006690: a700 0000 7250 0000 0072 2901 0000 722a  ....rP...r)...r*
+000066a0: 0100 0072 2b01 0000 7266 0000 005a 0a6b  ...r+...rf...Z.k
+000066b0: 6e6f 776e 5f61 7267 7372 8600 0000 7203  nown_argsr....r.
+000066c0: 0100 005a 0972 6f6f 745f 6675 6e63 5a14  ...Z.root_funcZ.
+000066d0: 726f 6f74 5f66 756e 635f 6172 6773 5f6d  root_func_args_m
+000066e0: 6f64 656c 5a0c 636f 6d6d 616e 645f 6e61  odelZ.command_na
+000066f0: 6d65 5a0c 636f 6d6d 616e 645f 6675 6e63  meZ.command_func
+00006700: 5a17 636f 6d6d 616e 645f 6675 6e63 5f61  Z.command_func_a
+00006710: 7267 735f 6d6f 6465 6c72 1901 0000 5a0b  rgs_modelr....Z.
+00006720: 726f 6f74 5f72 6573 756c 745a 0a67 656e  root_resultZ.gen
+00006730: 5f72 6573 756c 7472 5300 0000 7253 0000  _resultrS...rS..
+00006740: 0072 5700 0000 da04 5f72 756e b004 0000  .rW....._run....
+00006750: 737a 0000 0010 2308 020e 0108 0204 010e  sz....#.........
+00006760: 0308 0104 0204 0104 ff04 0304 0104 ff0c  ................
+00006770: 0304 0104 0104 ff04 0304 0104 ff04 0404  ................
+00006780: 0104 0204 0102 0102 0102 0102 0102 0106  ................
+00006790: fb0a 0802 010c 010c 0108 0102 ff04 0302  ................
+000067a0: 0208 0104 0102 0102 0102 0102 0102 0102  ................
+000067b0: 0106 fa02 800a 0908 0104 0104 0102 8004  ................
+000067c0: 020a fb08 0104 0104 0102 8002 fd02 017a  ...............z
+000067d0: 1341 7267 756d 656e 7450 6172 7365 722e  .ArgumentParser.
+000067e0: 5f72 756e 2902 4e46 725c 0000 0029 0246  _run).NFr\...).F
+000067f0: 4629 024e 4e29 034e 4e46 2903 4e4e 4e29  F).NN).NNF).NNN)
+00006800: 3a72 9500 0000 da0a 5f5f 6d6f 6475 6c65  :r......__module
+00006810: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00006820: 7242 0000 0072 6e00 0000 72a2 0000 0072  rB...rn...r....r
+00006830: 4300 0000 7244 0000 0072 4500 0000 7246  C...rD...rE...rF
+00006840: 0000 0072 2d00 0000 720c 0000 0072 1000  ...r-...r....r..
+00006850: 0000 720f 0000 0072 1300 0000 72d6 0000  ..r....r....r...
+00006860: 0072 6900 0000 7282 0000 0072 0b00 0000  .ri...r....r....
+00006870: 728a 0000 0072 1500 0000 720d 0000 0072  r....r....r....r
+00006880: 2900 0000 7291 0000 0072 7400 0000 7241  )...r....rt...rA
+00006890: 0000 0072 9b00 0000 729e 0000 00da 0c73  ...r....r......s
+000068a0: 7461 7469 636d 6574 686f 6472 a400 0000  taticmethodr....
+000068b0: da0b 636c 6173 736d 6574 686f 6472 2200  ..classmethodr".
+000068c0: 0000 7290 0000 0072 c700 0000 7212 0000  ..r....r....r...
+000068d0: 0072 cd00 0000 72c9 0000 0072 c800 0000  .r....r....r....
+000068e0: 7296 0000 0072 f200 0000 728c 0000 0072  r....r....r....r
+000068f0: 7700 0000 7228 0000 0072 f800 0000 7211  w...r(...r....r.
+00006900: 0000 0072 fa00 0000 72fe 0000 0072 0501  ...r....r....r..
+00006910: 0000 7206 0100 0072 0201 0000 720e 0000  ..r....r....r...
+00006920: 0072 0c01 0000 7298 0000 0072 1701 0000  .r....r....r....
+00006930: 7223 0100 0072 2801 0000 722f 0100 00da  r#...r(...r/....
+00006940: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7253  .__classcell__rS
+00006950: 0000 0072 5300 0000 7279 0000 0072 5700  ...rS...ry...rW.
+00006960: 0000 7241 0000 004c 0000 0073 d401 0000  ..rA...L...s....
+00006970: 0a00 0c01 0c01 0c01 0c01 0c01 0205 0201  ................
+00006980: 0201 0201 0201 0201 0201 0201 0201 06f5  ................
+00006990: 0202 02fe 0603 02fd 0604 02fc 0605 02fb  ................
+000069a0: 0a06 02fa 0a07 02f9 0a08 02f8 0a09 02f7  ................
+000069b0: 060a 02f6 020b 02f5 020c 0ef4 0e71 0206  .............q..
+000069c0: 0201 04fd 0a02 02fe 0203 02fd 0204 0efc  ................
+000069d0: 022e 1602 02fe 0203 0afd 0234 04fd 1602  ...........4....
+000069e0: 02fe 0603 02fd 0204 02fc 0405 0afb 0263  ...............c
+000069f0: 04fd 0a02 02fe 0603 02fd 0204 02fc 0205  ................
+00006a00: 0afb 020e 1c01 0203 0201 0402 02fe 1603  ................
+00006a10: 02fd 0604 0cfc 007f 007f 0228 2001 0203  ...........( ...
+00006a20: 2401 0203 2401 0203 0204 0201 04fc 0602  $...$...........
+00006a30: 02fe 0203 02fd 0204 02fc 0605 0cfb 143f  ...............?
+00006a40: 1411 100a 020b 0402 02fe 0203 0afd 0232  ...............2
+00006a50: 0201 04fd 0a02 02fe 0803 02fd 0204 0efc  ................
+00006a60: 0210 0201 04fd 0a02 02fe 0803 02fd 0e04  ................
+00006a70: 0efc 020f 0201 0201 04fc 0a02 02fe 0a03  ................
+00006a80: 02fd 0204 02fc 0e05 0afb 0230 0201 0201  ...........0....
+00006a90: 04fc 0a02 02fe 0a03 02fd 0204 02fc 0205  ................
+00006aa0: 0afb 0228 0201 04fc 0402 02fe 0a03 02fd  ...(............
+00006ab0: 0204 02fc 0205 0afb 0221 0201 0a01 02ff  .........!......
+00006ac0: 0602 02fe 0a03 0cfd 0206 0201 1602 02fe  ................
+00006ad0: 0603 0cfd 0219 0201 0402 02fe 1603 02fd  ................
+00006ae0: 0204 0cfc 020a 0206 0201 0201 04f9 0202  ................
+00006af0: 02fe 0a03 02fd 0604 02fc 0a05 02fb 0e06  ................
+00006b00: 02fa 0607 02f9 0208 0cf8 0263 0203 0201  ...........c....
+00006b10: 0201 04fc 0e02 02fe 1203 02fd 1604 02fc  ................
+00006b20: 0205 02fb 0206 0cfa 022e 0204 0201 06fc  ................
+00006b30: 0202 02fe 0a03 02fd 0a04 02fc 0205 02fb  ................
+00006b40: 0206 14fa 7241 0000 0029 4e72 7400 0000  ....rA...)Nrt...
+00006b50: da0f 636f 6c6c 6563 7469 6f6e 732e 6162  ..collections.ab
+00006b60: 6372 ce00 0000 727f 0000 0072 0200 0000  cr....r....r....
+00006b70: da0a 636f 6e74 6578 746c 6962 7203 0000  ..contextlibr...
+00006b80: 00da 0b64 6174 6163 6c61 7373 6573 7204  ...dataclassesr.
+00006b90: 0000 0072 0500 0000 7206 0000 00da 0465  ...r....r......e
+00006ba0: 6e75 6d72 0700 0000 da09 6675 6e63 746f  numr......functo
+00006bb0: 6f6c 7372 0800 0000 da07 696e 7370 6563  olsr......inspec
+00006bc0: 7472 0900 0000 da05 7479 7065 7372 0a00  tr......typesr..
+00006bd0: 0000 da06 7479 7069 6e67 720b 0000 0072  ....typingr....r
+00006be0: 0c00 0000 720d 0000 0072 0e00 0000 720f  ....r....r....r.
+00006bf0: 0000 0072 1000 0000 7211 0000 0072 1200  ...r....r....r..
+00006c00: 0000 7213 0000 0072 1400 0000 7215 0000  ..r....r....r...
+00006c10: 005a 0d70 6b67 5f72 6573 6f75 7263 6573  .Z.pkg_resources
+00006c20: 7216 0000 00da 0761 6374 696f 6e73 7218  r......actionsr.
+00006c30: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
+00006c40: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+00006c50: 0072 1f00 0000 7220 0000 00da 0361 7267  .r....r .....arg
+00006c60: 7221 0000 0072 2200 0000 7223 0000 0072  r!...r"...r#...r
+00006c70: 2400 0000 7225 0000 00da 0a65 7863 6570  $...r%.....excep
+00006c80: 7469 6f6e 7372 2600 0000 7227 0000 0072  tionsr&...r'...r
+00006c90: bf00 0000 7228 0000 0072 2900 0000 722a  ....r(...r)...r*
+00006ca0: 0000 0072 2b00 0000 da05 7574 696c 7372  ...r+.....utilsr
+00006cb0: 2c00 0000 722d 0000 0072 2e00 0000 722f  ,...r-...r....r/
+00006cc0: 0000 0072 3000 0000 7231 0000 0072 3200  ...r0...r1...r2.
+00006cd0: 0000 7233 0000 0072 3400 0000 7235 0000  ..r3...r4...r5..
+00006ce0: 0072 3600 0000 7237 0000 0072 3800 0000  .r6...r7...r8...
+00006cf0: 7239 0000 0072 c600 0000 723c 0000 005a  r9...r....r<...Z
+00006d00: 1174 7970 696e 675f 6578 7465 6e73 696f  .typing_extensio
+00006d10: 6e73 723f 0000 0072 4000 0000 7241 0000  nsr?...r@...rA..
+00006d20: 0072 5300 0000 7253 0000 0072 5300 0000  .rS...rS...rS...
+00006d30: 7257 0000 00da 083c 6d6f 6475 6c65 3e01  rW.....<module>.
+00006d40: 0000 0073 3200 0000 0800 0801 0801 0c01  ...s2...........
+00006d50: 0c01 1401 0c01 0c01 0c01 0c01 3401 0c0e  ............4...
+00006d60: 2c02 1c0b 1007 0c01 1401 4001 0a11 0e01  ,.........@.....
+00006d70: 0c02 0a02 0c01 0802 1603                 ..........
```

### Comparing `yapx-0.2.2/src/yapx/__pycache__/exceptions.cpython-310.pyc` & `yapx-0.2.3/src/yapx/__pycache__/exceptions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 04:48:20 2023 UTC, .py size: 633 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9448 c364 7902 0000  o........H.dy...
+00000000: 6f0d 0d0a 0000 0000 2256 c464 7902 0000  o......."V.dy...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 4700  m.Z.m.Z.m.Z...G.
 00000050: 6403 6404 8400 6404 6506 8303 5a07 4700  d.d...d.e...Z.G.
 00000060: 6405 6406 8400 6406 6501 8303 5a08 0907  d.d...d.e...Z...
 00000070: 640c 6408 6505 6503 1900 6409 6504 6506  d.d.e.e...d.e.e.
```

### Comparing `yapx-0.2.2/src/yapx/__pycache__/types.cpython-310.pyc` & `yapx-0.2.3/src/yapx/__pycache__/types.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 04:48:20 2023 UTC, .py size: 1300 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9448 c364 1405 0000  o........H.d....
+00000000: 6f0d 0d0a 0000 0000 2256 c464 1405 0000  o......."V.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 e600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6500 6a0a 6404 6b05 7226 6400 6405  ..e.j.d.k.r&d.d.
 00000070: 6c03 6d0b 5a0b 0100 6e06 6400 6405 6c0c  l.m.Z...n.d.d.l.
```

### Comparing `yapx-0.2.2/src/yapx/__pycache__/utils.cpython-310.pyc` & `yapx-0.2.3/src/yapx/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 04:48:20 2023 UTC, .py size: 4211 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9448 c364 7310 0000  o........H.ds...
+00000000: 6f0d 0d0a 0000 0000 2256 c464 7310 0000  o......."V.ds...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 2803 0000 5500  .....@...s(...U.
 00000030: 6400 6401 6c00 5a00 6400 6402 6c01 6d02  d.d.l.Z.d.d.l.m.
 00000040: 5a02 0100 6400 6403 6c03 6d04 5a04 0100  Z...d.d.l.m.Z...
 00000050: 6400 6404 6c05 6d06 5a06 0100 6400 6405  d.d.l.m.Z...d.d.
 00000060: 6c07 6d08 5a08 0100 6400 6406 6c09 6d0a  l.m.Z...d.d.l.m.
 00000070: 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e  Z.m.Z.m.Z.m.Z.m.
```

### Comparing `yapx-0.2.2/src/yapx/actions.py` & `yapx-0.2.3/src/yapx/actions.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.2/src/yapx/arg.py` & `yapx-0.2.3/src/yapx/arg.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.2/src/yapx/argument_parser.py` & `yapx-0.2.3/src/yapx/argument_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -534,14 +534,20 @@
                         # store desired types for casting later
                         # pylint: disable=protected-access
                         parser._dest_type[argparse_argument.dest] = partial(
                             cast_type,
                             fld_type,
                         )
 
+                    if argparse_argument.pos and argparse_argument.nargs is None:
+                        if argparse_argument.required:
+                            argparse_argument.nargs = "+"
+                        else:
+                            argparse_argument.nargs = "*"
+
                     # type-containers must only contain strings
                     # until parsed by argparse.
                     fld_type = str
 
             elif try_issubclass(fld_type, Enum):
                 argparse_argument.choices = list(fld_type)
```

### Comparing `yapx-0.2.2/src/yapx/exceptions.py` & `yapx-0.2.3/src/yapx/exceptions.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.2/src/yapx/types.py` & `yapx-0.2.3/src/yapx/types.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.2/src/yapx/utils.py` & `yapx-0.2.3/src/yapx/utils.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.2/src/yapx.egg-info/SOURCES.txt` & `yapx-0.2.3/src/yapx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yapx-0.2.2/src/yapx.egg-info/requires.txt` & `yapx-0.2.3/src/yapx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `yapx-0.2.2/tests/test_actions.py` & `yapx-0.2.3/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.2/tests/test_add_arguments.py` & `yapx-0.2.3/tests/test_add_arguments.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.2/tests/test_add_arguments_future.py` & `yapx-0.2.3/tests/test_add_arguments_future.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.2/tests/test_add_command.py` & `yapx-0.2.3/tests/test_add_command.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.2/tests/test_arg.py` & `yapx-0.2.3/tests/test_arg.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.2/tests/test_run.py` & `yapx-0.2.3/tests/test_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,15 +486,15 @@
     def _func(
         this: Optional[List[str]] = yapx.arg(None, pos=True, exclusive=True),
         that: Optional[List[str]] = yapx.arg(None, exclusive=True),
     ) -> List[int]:
         return this, that
 
     # 1. ARRANGE
-    cli_args: List[str] = ["--that", "world"]
+    cli_args: List[str] = ["one", "two", "three", "--that", "world"]
 
     # 2. ACT
     result: List[Any] = yapx.run_patched(
         _func,
         test_args=cli_args,
         disable_pydantic=disable_pydantic,
     )
```

### Comparing `yapx-0.2.2/tests/test_utils.py` & `yapx-0.2.3/tests/test_utils.py`

 * *Files identical despite different names*

