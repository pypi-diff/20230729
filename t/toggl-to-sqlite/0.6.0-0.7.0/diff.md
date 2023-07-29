# Comparing `tmp/toggl-to-sqlite-0.6.0.tar.gz` & `tmp/toggl-to-sqlite-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toggl-to-sqlite-0.6.0.tar", last modified: Tue Jan 11 04:13:28 2022, max compression
+gzip compressed data, was "toggl-to-sqlite-0.7.0.tar", last modified: Sat Jul 29 18:01:50 2023, max compression
```

## Comparing `toggl-to-sqlite-0.6.0.tar` & `toggl-to-sqlite-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 04:13:28.099027 toggl-to-sqlite-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-01-11 04:13:20.000000 toggl-to-sqlite-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3800 2022-01-11 04:13:28.099027 toggl-to-sqlite-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2788 2022-01-11 04:13:20.000000 toggl-to-sqlite-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-01-11 04:13:20.000000 toggl-to-sqlite-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-01-11 04:13:28.099027 toggl-to-sqlite-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1730 2022-01-11 04:13:20.000000 toggl-to-sqlite-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 04:13:28.099027 toggl-to-sqlite-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 04:13:28.099027 toggl-to-sqlite-0.6.0/src/toggl_to_sqlite/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-11 04:13:20.000000 toggl-to-sqlite-0.6.0/src/toggl_to_sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2285 2022-01-11 04:13:20.000000 toggl-to-sqlite-0.6.0/src/toggl_to_sqlite/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2614 2022-01-11 04:13:20.000000 toggl-to-sqlite-0.6.0/src/toggl_to_sqlite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 04:13:28.099027 toggl-to-sqlite-0.6.0/src/toggl_to_sqlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3800 2022-01-11 04:13:27.000000 toggl-to-sqlite-0.6.0/src/toggl_to_sqlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-01-11 04:13:27.000000 toggl-to-sqlite-0.6.0/src/toggl_to_sqlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-11 04:13:27.000000 toggl-to-sqlite-0.6.0/src/toggl_to_sqlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-01-11 04:13:27.000000 toggl-to-sqlite-0.6.0/src/toggl_to_sqlite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-01-11 04:13:27.000000 toggl-to-sqlite-0.6.0/src/toggl_to_sqlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-01-11 04:13:27.000000 toggl-to-sqlite-0.6.0/src/toggl_to_sqlite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:01:50.783314 toggl-to-sqlite-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-29 18:01:36.000000 toggl-to-sqlite-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-29 18:01:50.783314 toggl-to-sqlite-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-29 18:01:36.000000 toggl-to-sqlite-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-29 18:01:36.000000 toggl-to-sqlite-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-29 18:01:50.783314 toggl-to-sqlite-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:01:50.783314 toggl-to-sqlite-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:01:50.783314 toggl-to-sqlite-0.7.0/src/toggl_to_sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 18:01:36.000000 toggl-to-sqlite-0.7.0/src/toggl_to_sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-29 18:01:36.000000 toggl-to-sqlite-0.7.0/src/toggl_to_sqlite/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-29 18:01:36.000000 toggl-to-sqlite-0.7.0/src/toggl_to_sqlite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:01:50.783314 toggl-to-sqlite-0.7.0/src/toggl_to_sqlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-29 18:01:50.000000 toggl-to-sqlite-0.7.0/src/toggl_to_sqlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-29 18:01:50.000000 toggl-to-sqlite-0.7.0/src/toggl_to_sqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 18:01:50.000000 toggl-to-sqlite-0.7.0/src/toggl_to_sqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-29 18:01:50.000000 toggl-to-sqlite-0.7.0/src/toggl_to_sqlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 18:01:50.000000 toggl-to-sqlite-0.7.0/src/toggl_to_sqlite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:01:50.783314 toggl-to-sqlite-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-29 18:01:36.000000 toggl-to-sqlite-0.7.0/tests/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-07-29 18:01:36.000000 toggl-to-sqlite-0.7.0/tests/test_utils.py
```

### Comparing `toggl-to-sqlite-0.6.0/LICENSE` & `toggl-to-sqlite-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toggl-to-sqlite-0.6.0/PKG-INFO` & `toggl-to-sqlite-0.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: toggl-to-sqlite
-Version: 0.6.0
-Summary: Create a SQLite database containing data from your Toggl account
-Home-page: https://github.com/ryancheley/toggle-to-sqlite
+Version: 0.7.0
+Summary: ACreate a SQLite database containing data from your Toggl account
 Author: Ryan Cheley
-License: Apache License, Version 2.0
+License: Apache-2.0
 Project-URL: Issues, https://github.com/ryancheley/toggl-to-sqlite/issues
 Project-URL: CI, https://github.com/ryancheley/toggl-to-sqlite/actions
 Project-URL: Changelog, https://github.com/ryancheley/toggl-to-sqlite/releases
 Project-URL: Documentation, https://github.com/ryancheley/toggl-to-sqlite/blob/main/README.md
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # toggl-to-sqlite
 
 [![PyPI](https://img.shields.io/pypi/v/toggl-to-sqlite.svg)](https://pypi.org/project/toggl-to-sqlite/)
 [![GitHub changelog](https://img.shields.io/github/v/release/ryancheley/toggl-to-sqlite?include_prereleases&label=changelog)](https://github.com/ryancheley/toggl-to-sqlite/releases)
 [![Tests](https://github.com/ryancheley/toggl-to-sqlite/workflows/Test/badge.svg)](https://github.com/ryancheley/toggl-to-sqlite/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/ryancheley/toggl-to-sqlite/blob/main/LICENSE)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ryancheley/toggl-to-sqlite/main.svg)](https://results.pre-commit.ci/latest/github/ryancheley/toggl-to-sqlite/main)
+
 
 
 Create a SQLite database containing data from your [Toggl](https://toggl.com/) account.
 
 ## How to install
 
     $ pip install toggl-to-sqlite
@@ -97,9 +97,7 @@
 
 ```
 <!-- [[[end]]] -->
 
 ## Using with Datasette
 
 The SQLite database produced by this tool is designed to be browsed using [Datasette](https://datasette.readthedocs.io/). Use the [datasette-render-timestamps](https://github.com/simonw/datasette-render-timestamps) plugin to improve the display of the timestamp values.
-
-
```

### Comparing `toggl-to-sqlite-0.6.0/README.md` & `toggl-to-sqlite-0.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # toggl-to-sqlite
 
 [![PyPI](https://img.shields.io/pypi/v/toggl-to-sqlite.svg)](https://pypi.org/project/toggl-to-sqlite/)
 [![GitHub changelog](https://img.shields.io/github/v/release/ryancheley/toggl-to-sqlite?include_prereleases&label=changelog)](https://github.com/ryancheley/toggl-to-sqlite/releases)
 [![Tests](https://github.com/ryancheley/toggl-to-sqlite/workflows/Test/badge.svg)](https://github.com/ryancheley/toggl-to-sqlite/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/ryancheley/toggl-to-sqlite/blob/main/LICENSE)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ryancheley/toggl-to-sqlite/main.svg)](https://results.pre-commit.ci/latest/github/ryancheley/toggl-to-sqlite/main)
+
 
 
 Create a SQLite database containing data from your [Toggl](https://toggl.com/) account.
 
 ## How to install
 
     $ pip install toggl-to-sqlite
```

### Comparing `toggl-to-sqlite-0.6.0/setup.py` & `toggl-to-sqlite-0.7.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,52 @@
-import os
-
-from setuptools import setup
-
-VERSION = "0.6.0"
-
-
-def get_long_description():
-    with open(
-        os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
-        encoding="utf8",
-    ) as fp:
-        return fp.read()
-
-
-setup(
-    name="toggl-to-sqlite",
-    description="Create a SQLite database containing data from your Toggl account",
-    long_description=get_long_description(),
-    long_description_content_type="text/markdown",
-    author="Ryan Cheley",
-    project_urls={
-        "Issues": "https://github.com/ryancheley/toggl-to-sqlite/issues",
-        "CI": "https://github.com/ryancheley/toggl-to-sqlite/actions",
-        "Changelog": "https://github.com/ryancheley/toggl-to-sqlite/releases",
-        "Documentation": "https://github.com/ryancheley/toggl-to-sqlite/blob/main/README.md",
-    },
-    url="https://github.com/ryancheley/toggle-to-sqlite",
-    license="Apache License, Version 2.0",
-    version=VERSION,
-    packages=["toggl_to_sqlite"],
-    package_dir={"": "src"},
-    entry_points="""
-        [console_scripts]
-        toggl-to-sqlite=toggl_to_sqlite.cli:cli
-    """,
-    install_requires=["sqlite-utils>=2.4.4", "click", "requests", "requests_mock", "toml"],
-    extras_require={"test": ["pytest", "black", "isort", "coverage", "mypy", "cogapp", "pre-commit"]},
-    tests_require=["toggl-to-sqlite[test]"],
-    python_requires=">=3.6",
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Intended Audience :: Developers",
-        "Topic :: Utilities",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-    ],
-)
+[project]
+name = "toggl-to-sqlite"
+version = "0.7.0"
+description = "ACreate a SQLite database containing data from your Toggl account"
+readme = "README.md"
+authors = [{name = "Ryan Cheley"}]
+license = {text = "Apache-2.0"}
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "Topic :: Utilities",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+]
+dependencies = [
+    "sqlite-utils>=2.4.4",
+    "click",
+    "requests",
+    "requests_mock",
+    "toml",
+    "click",
+]
+
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project.urls]
+Issues = "https://github.com/ryancheley/toggl-to-sqlite/issues"
+CI = "https://github.com/ryancheley/toggl-to-sqlite/actions"
+Changelog = "https://github.com/ryancheley/toggl-to-sqlite/releases"
+Documentation = "https://github.com/ryancheley/toggl-to-sqlite/blob/main/README.md"
+
+[project.optional-dependencies]
+test = [
+    "pytest",
+    "black",
+    "isort",
+    "coverage",
+    "mypy",
+    "cogapp",
+    "pre-commit"
+]
+
+[tool.black]
+line-length = 130
+target-version = ['py311']
+include = '\.pyi?$'
+exclude = '(venv)'
```

### Comparing `toggl-to-sqlite-0.6.0/src/toggl_to_sqlite/cli.py` & `toggl-to-sqlite-0.7.0/src/toggl_to_sqlite/cli.py`

 * *Files identical despite different names*

### Comparing `toggl-to-sqlite-0.6.0/src/toggl_to_sqlite/utils.py` & `toggl-to-sqlite-0.7.0/src/toggl_to_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `toggl-to-sqlite-0.6.0/src/toggl_to_sqlite.egg-info/PKG-INFO` & `toggl-to-sqlite-0.7.0/src/toggl_to_sqlite.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: toggl-to-sqlite
-Version: 0.6.0
-Summary: Create a SQLite database containing data from your Toggl account
-Home-page: https://github.com/ryancheley/toggle-to-sqlite
+Version: 0.7.0
+Summary: ACreate a SQLite database containing data from your Toggl account
 Author: Ryan Cheley
-License: Apache License, Version 2.0
+License: Apache-2.0
 Project-URL: Issues, https://github.com/ryancheley/toggl-to-sqlite/issues
 Project-URL: CI, https://github.com/ryancheley/toggl-to-sqlite/actions
 Project-URL: Changelog, https://github.com/ryancheley/toggl-to-sqlite/releases
 Project-URL: Documentation, https://github.com/ryancheley/toggl-to-sqlite/blob/main/README.md
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # toggl-to-sqlite
 
 [![PyPI](https://img.shields.io/pypi/v/toggl-to-sqlite.svg)](https://pypi.org/project/toggl-to-sqlite/)
 [![GitHub changelog](https://img.shields.io/github/v/release/ryancheley/toggl-to-sqlite?include_prereleases&label=changelog)](https://github.com/ryancheley/toggl-to-sqlite/releases)
 [![Tests](https://github.com/ryancheley/toggl-to-sqlite/workflows/Test/badge.svg)](https://github.com/ryancheley/toggl-to-sqlite/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/ryancheley/toggl-to-sqlite/blob/main/LICENSE)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ryancheley/toggl-to-sqlite/main.svg)](https://results.pre-commit.ci/latest/github/ryancheley/toggl-to-sqlite/main)
+
 
 
 Create a SQLite database containing data from your [Toggl](https://toggl.com/) account.
 
 ## How to install
 
     $ pip install toggl-to-sqlite
@@ -97,9 +97,7 @@
 
 ```
 <!-- [[[end]]] -->
 
 ## Using with Datasette
 
 The SQLite database produced by this tool is designed to be browsed using [Datasette](https://datasette.readthedocs.io/). Use the [datasette-render-timestamps](https://github.com/simonw/datasette-render-timestamps) plugin to improve the display of the timestamp values.
-
-
```

