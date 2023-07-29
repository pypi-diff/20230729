# Comparing `tmp/jaraco.services-3.1.0.tar.gz` & `tmp/jaraco.services-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.services-3.1.0.tar", last modified: Fri Feb 12 03:10:22 2021, max compression
+gzip compressed data, was "jaraco.services-3.2.0.tar", last modified: Sat Jul 29 18:12:48 2023, max compression
```

## Comparing `jaraco.services-3.1.0.tar` & `jaraco.services-3.2.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-12 03:10:22.879882 jaraco.services-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-12 03:10:22.879882 jaraco.services-3.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-12 03:10:22.879882 jaraco.services-3.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/.github/workflows/automerge.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1804 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2021-02-12 03:10:22.879882 jaraco.services-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      714 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-12 03:10:22.879882 jaraco.services-3.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      756 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      395 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-12 03:10:22.879882 jaraco.services-3.1.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-12 03:10:22.879882 jaraco.services-3.1.0/jaraco/services/
--rw-r--r--   0 runner    (1001) docker     (121)    11370 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/jaraco/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/jaraco/services/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-12 03:10:22.879882 jaraco.services-3.1.0/jaraco.services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2021-02-12 03:10:22.000000 jaraco.services-3.1.0/jaraco.services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      539 2021-02-12 03:10:22.000000 jaraco.services-3.1.0/jaraco.services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-12 03:10:22.000000 jaraco.services-3.1.0/jaraco.services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      268 2021-02-12 03:10:22.000000 jaraco.services-3.1.0/jaraco.services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-02-12 03:10:22.000000 jaraco.services-3.1.0/jaraco.services.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      333 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2021-02-12 03:10:22.883882 jaraco.services-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    10139 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/skeleton.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-12 03:10:22.879882 jaraco.services-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      803 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (121)      719 2021-02-12 03:10:03.000000 jaraco.services-3.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:12:48.530076 jaraco.services-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:12:48.526076 jaraco.services-3.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:12:48.526076 jaraco.services-3.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-29 18:12:48.530076 jaraco.services-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:12:48.526076 jaraco.services-3.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:12:48.518076 jaraco.services-3.2.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:12:48.530076 jaraco.services-3.2.0/jaraco/services/
+-rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/jaraco/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/jaraco/services/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:12:48.526076 jaraco.services-3.2.0/jaraco.services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-29 18:12:48.000000 jaraco.services-3.2.0/jaraco.services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-29 18:12:48.000000 jaraco.services-3.2.0/jaraco.services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 18:12:48.000000 jaraco.services-3.2.0/jaraco.services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-29 18:12:48.000000 jaraco.services-3.2.0/jaraco.services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-29 18:12:48.000000 jaraco.services-3.2.0/jaraco.services.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-29 18:12:48.530076 jaraco.services-3.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:12:48.530076 jaraco.services-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/tox.ini
```

### Comparing `jaraco.services-3.1.0/CHANGES.rst` & `jaraco.services-3.2.0/NEWS.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v3.2.0
+======
+
+Features
+--------
+
+- Require Python 3.8 or later.
+
+
 v3.1.0
 ======
 
 * Require Python 3.6 or later.
 
 3.0
 ===
```

### Comparing `jaraco.services-3.1.0/LICENSE` & `jaraco.services-3.2.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jaraco.services-3.1.0/PKG-INFO` & `jaraco.services-3.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: jaraco.services
-Version: 3.1.0
+Version: 3.2.0
 Summary: Service orchestration and pytest plugins
 Home-page: https://github.com/jaraco/jaraco.services
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Description: .. image:: https://img.shields.io/pypi/v/jaraco.services.svg
-           :target: `PyPI link`_
-        
-        .. image:: https://img.shields.io/pypi/pyversions/jaraco.services.svg
-           :target: `PyPI link`_
-        
-        .. _PyPI link: https://pypi.org/project/jaraco.services
-        
-        .. image:: https://github.com/jaraco/jaraco.services/workflows/tests/badge.svg
-           :target: https://github.com/jaraco/jaraco.services/actions?query=workflow%3A%22tests%22
-           :alt: tests
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/psf/black
-           :alt: Code style: Black
-        
-        .. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-        ..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/v/jaraco.services.svg
+   :target: https://pypi.org/project/jaraco.services
+
+.. image:: https://img.shields.io/pypi/pyversions/jaraco.services.svg
+
+.. image:: https://github.com/jaraco/jaraco.services/workflows/tests/badge.svg
+   :target: https://github.com/jaraco/jaraco.services/actions?query=workflow%3A%22tests%22
+   :alt: tests
+
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: Black
+
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
+
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
+   :target: https://blog.jaraco.com/skeleton
```

### Comparing `jaraco.services-3.1.0/README.rst` & `jaraco.services-3.2.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 .. image:: https://img.shields.io/pypi/v/jaraco.services.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/jaraco.services
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.services.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/jaraco.services
 
 .. image:: https://github.com/jaraco/jaraco.services/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.services/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
+
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
+   :target: https://blog.jaraco.com/skeleton
```

### Comparing `jaraco.services-3.1.0/docs/conf.py` & `jaraco.services-3.2.0/docs/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,42 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-extensions = ['sphinx.ext.autodoc', 'jaraco.packaging.sphinx', 'rst.linker']
+extensions = [
+    'sphinx.ext.autodoc',
+    'jaraco.packaging.sphinx',
+]
 
 master_doc = "index"
+html_theme = "furo"
 
+# Link dates and other references in the changelog
+extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
                 pattern=r'(?m:^((?P<scm_version>v?\d+(\.\d+){1,2}))\n[-=]+\n)',
                 with_scm='{text}\n{rev[timestamp]:%d %b %Y}\n',
             ),
             dict(
                 pattern=r'PEP[- ](?P<pep_number>\d+)',
-                url='https://www.python.org/dev/peps/pep-{pep_number:0>4}/',
+                url='https://peps.python.org/pep-{pep_number:0>4}/',
             ),
         ],
     )
 }
+
+# Be strict about any broken references
+nitpicky = True
+
+# Include Python intersphinx mapping to prevent failures
+# jaraco/skeleton#51
+extensions += ['sphinx.ext.intersphinx']
+intersphinx_mapping = {
+    'python': ('https://docs.python.org/3', None),
+}
+
+# Preserve authored syntax for defaults
+autodoc_preserve_defaults = True
```

### Comparing `jaraco.services-3.1.0/jaraco/services/__init__.py` & `jaraco.services-3.2.0/jaraco/services/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     A class that manages services that may be required by some of the
     unit tests. ServiceManager will start up daemon services as
     subprocesses or threads and will stop them when requested or when
     destroyed.
     """
 
     def __init__(self, *args, **kwargs):
-        super(ServiceManager, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         msg = "ServiceManager is deprecated. Use fixtures instead."
         warnings.warn(msg, DeprecationWarning)
         self.failed = set()
 
     def __enter__(self):
         return self
 
@@ -202,15 +202,15 @@
         A service is external if there's another process already providing
         this service, typically detected by the port already being occupied.
         """
         return getattr(self, 'external', False)
 
     def stop(self):
         if self.is_running() and not self.is_external():
-            super(Subprocess, self).stop()
+            super().stop()
             self.process.terminate()
             self.process.wait()
             del self.process
 
     @properties.NonDataProperty
     def log_root(self):
         """
@@ -223,15 +223,15 @@
             os.makedirs(var_log)
         return var_log
 
     def get_log(self):
         log_name = self.__class__.__name__
         log_filename = os.path.join(self.log_root, log_name)
         log_file = open(log_filename, 'a')
-        self.log_reader = open(log_filename, 'r')
+        self.log_reader = open(log_filename)
         self.log_reader.seek(log_file.tell())
         return log_file
 
     def _get_more_data(self, file, timeout):
         """
         Return data from the file, if available. If no data is received
         by the timeout, then raise RuntimeError.
@@ -377,14 +377,14 @@
 
     def install(self):
         installer = self.installer.split()
         cmd = [self.python, '-m'] + installer + [self.package_spec]
         subprocess.check_call(cmd, env=self._run_env)
 
     def start(self):
-        super(PythonService, self).start()
+        super().start()
         self.create_env()
         self.install()
         output = (self.env_path / 'output.txt').open('ab')
         self.process = subprocess.Popen(
             self.command, env=self._run_env, stdout=output, stderr=subprocess.STDOUT
         )
```

### Comparing `jaraco.services-3.1.0/jaraco/services/paths.py` & `jaraco.services-3.2.0/jaraco/services/paths.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,43 +17,40 @@
     @abc.abstractproperty
     def exe(self):
         "The target executable"
 
     args: List[str] = []
     "Additional args to pass to the exe when testing for its suitability"
 
-    DEV_NULL = open(os.path.devnull, 'r+')
-
     @classmethod
     def resolve(cls):
         """
         Resolve an executable or raise RuntimeError if one
         cannot be found.
         """
         return cls.find_root() / cls.exe
 
     @classmethod
     def find_root(cls):
         try:
             result = next(cls.find_valid_roots())
         except StopIteration:
-            raise RuntimeError(
-                "{cls.__name__} unable to find executables".format(**locals())
-            )
+            raise RuntimeError(f"{cls.__name__} unable to find executables")
         return path.Path(result)
 
     @classmethod
     def find_valid_roots(cls):
         """
         Generate valid roots for the target executable based on the
         candidate paths.
         """
         return filter(cls.is_valid_root, cls.candidate_paths)
 
     @classmethod
     def is_valid_root(cls, root):
         try:
             cmd = [os.path.join(root, cls.exe)] + cls.args
-            subprocess.check_call(cmd, stdout=cls.DEV_NULL)
+            with open(os.path.devnull, 'r+', encoding='utf-8') as null:
+                subprocess.check_call(cmd, stdout=null)
         except OSError:
             return False
         return True
```

### Comparing `jaraco.services-3.1.0/jaraco.services.egg-info/PKG-INFO` & `jaraco.services-3.2.0/jaraco.services.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: jaraco.services
-Version: 3.1.0
+Version: 3.2.0
 Summary: Service orchestration and pytest plugins
 Home-page: https://github.com/jaraco/jaraco.services
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Description: .. image:: https://img.shields.io/pypi/v/jaraco.services.svg
-           :target: `PyPI link`_
-        
-        .. image:: https://img.shields.io/pypi/pyversions/jaraco.services.svg
-           :target: `PyPI link`_
-        
-        .. _PyPI link: https://pypi.org/project/jaraco.services
-        
-        .. image:: https://github.com/jaraco/jaraco.services/workflows/tests/badge.svg
-           :target: https://github.com/jaraco/jaraco.services/actions?query=workflow%3A%22tests%22
-           :alt: tests
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/psf/black
-           :alt: Code style: Black
-        
-        .. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-        ..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/v/jaraco.services.svg
+   :target: https://pypi.org/project/jaraco.services
+
+.. image:: https://img.shields.io/pypi/pyversions/jaraco.services.svg
+
+.. image:: https://github.com/jaraco/jaraco.services/workflows/tests/badge.svg
+   :target: https://github.com/jaraco/jaraco.services/actions?query=workflow%3A%22tests%22
+   :alt: tests
+
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: Black
+
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
+
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
+   :target: https://blog.jaraco.com/skeleton
```

### Comparing `jaraco.services-3.1.0/jaraco.services.egg-info/SOURCES.txt` & `jaraco.services-3.2.0/jaraco.services.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 .coveragerc
-.flake8
+.editorconfig
 .pre-commit-config.yaml
-.readthedocs.yml
-CHANGES.rst
+.readthedocs.yaml
 LICENSE
+NEWS.rst
 README.rst
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
-setup.py
-skeleton.md
+towncrier.toml
 tox.ini
-.github/workflows/automerge.yml
+.github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
 jaraco.services.egg-info/PKG-INFO
 jaraco.services.egg-info/SOURCES.txt
 jaraco.services.egg-info/dependency_links.txt
```

### Comparing `jaraco.services-3.1.0/setup.cfg` & `jaraco.services-3.2.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 [metadata]
-license_files = 
-	LICENSE
 name = jaraco.services
 author = Jason R. Coombs
 author_email = jaraco@jaraco.com
 description = Service orchestration and pytest plugins
 long_description = file:README.rst
 url = https://github.com/jaraco/jaraco.services
 classifiers = 
@@ -13,41 +11,45 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.6
+python_requires = >=3.8
 install_requires = 
 	portend
 	path
 	tempora
 	jaraco.classes
-setup_requires = setuptools_scm[toml] >= 3.4.1
 
 [options.packages.find]
 exclude = 
 	build*
+	dist*
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
-	pytest >= 3.5, !=3.7.3
-	pytest-checkdocs >= 1.2.3
-	pytest-flake8
-	pytest-black >= 0.3.7; python_implementation != "PyPy"
+	pytest >= 6
+	pytest-checkdocs >= 2.4
+	pytest-black >= 0.3.7; \
+	python_implementation != "PyPy"
 	pytest-cov
-	pytest-mypy; python_implementation != "PyPy"
-	pytest-enabler
+	pytest-mypy >= 0.9.1; \
+	python_implementation != "PyPy"
+	pytest-enabler >= 2.2
+	pytest-ruff
 docs = 
-	sphinx
-	jaraco.packaging >= 8.2
+	sphinx >= 3.5
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
 
 [options.entry_points]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `jaraco.services-3.1.0/tests/test_services.py` & `jaraco.services-3.2.0/tests/test_services.py`

 * *Files identical despite different names*

