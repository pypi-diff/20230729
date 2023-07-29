# Comparing `tmp/progfiguration-0.0.2a3.tar.gz` & `tmp/progfiguration-0.0.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progfiguration-0.0.2a3.tar", last modified: Mon Jul 24 04:15:21 2023, max compression
+gzip compressed data, was "progfiguration-0.0.2a4.tar", last modified: Sat Jul 29 02:40:25 2023, max compression
```

## Comparing `progfiguration-0.0.2a3.tar` & `progfiguration-0.0.2a4.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.742926 progfiguration-0.0.2a3/
--rw-------   0 mrled      (501) staff       (20)     2108 2023-07-24 04:15:21.742426 progfiguration-0.0.2a3/PKG-INFO
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.720476 progfiguration-0.0.2a3/progfiguration/
--rw-------   0 mrled      (501) staff       (20)      518 2023-07-23 23:23:06.000000 progfiguration-0.0.2a3/progfiguration/__init__.py
--rw-------   0 mrled      (501) staff       (20)     3635 2023-07-23 21:17:36.000000 progfiguration-0.0.2a3/progfiguration/age.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.725284 progfiguration-0.0.2a3/progfiguration/builddata/
--rw-r--r--   0 mrled      (501) staff       (20)      253 2023-07-22 05:43:26.000000 progfiguration-0.0.2a3/progfiguration/builddata/__init__.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.729733 progfiguration-0.0.2a3/progfiguration/cli/
--rw-------   0 mrled      (501) staff       (20)       41 2023-07-23 22:36:36.000000 progfiguration-0.0.2a3/progfiguration/cli/__init__.py
--rw-------   0 mrled      (501) staff       (20)     6705 2023-07-24 03:58:20.000000 progfiguration-0.0.2a3/progfiguration/cli/progfiguration_core_cmd.py
--rw-r--r--   0 mrled      (501) staff       (20)    21295 2023-07-23 23:30:07.000000 progfiguration-0.0.2a3/progfiguration/cli/progfiguration_site_cmd.py
--rw-r--r--   0 mrled      (501) staff       (20)     5863 2023-07-23 23:10:02.000000 progfiguration-0.0.2a3/progfiguration/cli/util.py
--rw-------   0 mrled      (501) staff       (20)     5927 2023-07-22 05:27:56.000000 progfiguration-0.0.2a3/progfiguration/cmd.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.732409 progfiguration-0.0.2a3/progfiguration/inventory/
--rw-------   0 mrled      (501) staff       (20)    17722 2023-07-23 23:22:00.000000 progfiguration-0.0.2a3/progfiguration/inventory/__init__.py
--rw-------   0 mrled      (501) staff       (20)      874 2023-07-22 04:24:12.000000 progfiguration-0.0.2a3/progfiguration/inventory/nodes.py
--rw-------   0 mrled      (501) staff       (20)     4613 2023-07-23 23:21:39.000000 progfiguration-0.0.2a3/progfiguration/inventory/roles.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.736630 progfiguration-0.0.2a3/progfiguration/localhost/
--rw-------   0 mrled      (501) staff       (20)    11082 2023-07-23 23:21:13.000000 progfiguration-0.0.2a3/progfiguration/localhost/__init__.py
--rw-------   0 mrled      (501) staff       (20)     1184 2023-07-22 04:24:17.000000 progfiguration-0.0.2a3/progfiguration/localhost/authorized_keys.py
--rw-------   0 mrled      (501) staff       (20)     6056 2023-07-22 04:24:20.000000 progfiguration-0.0.2a3/progfiguration/localhost/disks.py
--rw-------   0 mrled      (501) staff       (20)     3044 2023-07-22 04:24:22.000000 progfiguration-0.0.2a3/progfiguration/localhost/localusers.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.737320 progfiguration-0.0.2a3/progfiguration/progfigbuild/
--rw-r--r--   0 mrled      (501) staff       (20)    17408 2023-07-24 04:09:57.000000 progfiguration-0.0.2a3/progfiguration/progfigbuild/__init__.py
--rw-r--r--   0 mrled      (501) staff       (20)     2505 2023-07-22 05:35:59.000000 progfiguration-0.0.2a3/progfiguration/progfigsite_validator.py
--rw-------   0 mrled      (501) staff       (20)      912 2023-07-22 05:36:48.000000 progfiguration-0.0.2a3/progfiguration/progfigtypes.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.738344 progfiguration-0.0.2a3/progfiguration/remotebrute/
--rw-------   0 mrled      (501) staff       (20)     3117 2023-07-22 04:24:58.000000 progfiguration-0.0.2a3/progfiguration/remotebrute/__init__.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.739054 progfiguration-0.0.2a3/progfiguration/sitewrapper/
--rw-r--r--   0 mrled      (501) staff       (20)     3972 2023-07-22 04:26:29.000000 progfiguration-0.0.2a3/progfiguration/sitewrapper/__init__.py
--rw-------   0 mrled      (501) staff       (20)     1804 2023-07-22 05:39:58.000000 progfiguration-0.0.2a3/progfiguration/ssh.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.739686 progfiguration-0.0.2a3/progfiguration/temple/
--rw-------   0 mrled      (501) staff       (20)      744 2023-06-28 22:11:55.000000 progfiguration-0.0.2a3/progfiguration/temple/__init__.py
--rw-r--r--   0 mrled      (501) staff       (20)     1832 2023-07-23 22:41:01.000000 progfiguration-0.0.2a3/progfiguration/util.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.724654 progfiguration-0.0.2a3/progfiguration.egg-info/
--rw-------   0 mrled      (501) staff       (20)     2108 2023-07-24 04:15:21.000000 progfiguration-0.0.2a3/progfiguration.egg-info/PKG-INFO
--rw-------   0 mrled      (501) staff       (20)     1100 2023-07-24 04:15:21.000000 progfiguration-0.0.2a3/progfiguration.egg-info/SOURCES.txt
--rw-------   0 mrled      (501) staff       (20)        1 2023-07-24 04:15:21.000000 progfiguration-0.0.2a3/progfiguration.egg-info/dependency_links.txt
--rw-------   0 mrled      (501) staff       (20)       83 2023-07-24 04:15:21.000000 progfiguration-0.0.2a3/progfiguration.egg-info/entry_points.txt
--rw-------   0 mrled      (501) staff       (20)       43 2023-07-24 04:15:21.000000 progfiguration-0.0.2a3/progfiguration.egg-info/requires.txt
--rw-------   0 mrled      (501) staff       (20)       15 2023-07-24 04:15:21.000000 progfiguration-0.0.2a3/progfiguration.egg-info/top_level.txt
--rw-------   0 mrled      (501) staff       (20)      712 2023-07-24 04:14:18.000000 progfiguration-0.0.2a3/pyproject.toml
--rw-------   0 mrled      (501) staff       (20)     1771 2023-07-23 20:27:37.000000 progfiguration-0.0.2a3/readme.md
--rw-------   0 mrled      (501) staff       (20)       38 2023-07-24 04:15:21.743080 progfiguration-0.0.2a3/setup.cfg
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.741635 progfiguration-0.0.2a3/tests/
--rw-------   0 mrled      (501) staff       (20)     1293 2023-07-22 04:15:43.000000 progfiguration-0.0.2a3/tests/test_cmd.py
--rw-------   0 mrled      (501) staff       (20)     1778 2023-07-22 04:38:21.000000 progfiguration-0.0.2a3/tests/test_packaging.py
--rw-------   0 mrled      (501) staff       (20)     2321 2023-07-19 14:30:38.000000 progfiguration-0.0.2a3/tests/test_site.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 02:40:24.999884 progfiguration-0.0.2a4/
+-rw-------   0 mrled      (501) staff       (20)     1074 2023-07-24 04:31:40.000000 progfiguration-0.0.2a4/LICENSE
+-rw-------   0 mrled      (501) staff       (20)     3109 2023-07-29 02:40:24.999505 progfiguration-0.0.2a4/PKG-INFO
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 02:40:24.971332 progfiguration-0.0.2a4/progfiguration/
+-rw-------   0 mrled      (501) staff       (20)      518 2023-07-23 23:23:06.000000 progfiguration-0.0.2a4/progfiguration/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     3635 2023-07-23 21:17:36.000000 progfiguration-0.0.2a4/progfiguration/age.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 02:40:24.977712 progfiguration-0.0.2a4/progfiguration/builddata/
+-rw-r--r--   0 mrled      (501) staff       (20)      253 2023-07-22 05:43:26.000000 progfiguration-0.0.2a4/progfiguration/builddata/__init__.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 02:40:24.983137 progfiguration-0.0.2a4/progfiguration/cli/
+-rw-------   0 mrled      (501) staff       (20)       41 2023-07-23 22:36:36.000000 progfiguration-0.0.2a4/progfiguration/cli/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     6909 2023-07-29 02:11:37.000000 progfiguration-0.0.2a4/progfiguration/cli/progfiguration_core_cmd.py
+-rw-r--r--   0 mrled      (501) staff       (20)    21295 2023-07-23 23:30:07.000000 progfiguration-0.0.2a4/progfiguration/cli/progfiguration_site_cmd.py
+-rw-r--r--   0 mrled      (501) staff       (20)     5863 2023-07-23 23:10:02.000000 progfiguration-0.0.2a4/progfiguration/cli/util.py
+-rw-------   0 mrled      (501) staff       (20)     5927 2023-07-22 05:27:56.000000 progfiguration-0.0.2a4/progfiguration/cmd.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 02:40:24.986558 progfiguration-0.0.2a4/progfiguration/inventory/
+-rw-------   0 mrled      (501) staff       (20)    17727 2023-07-27 00:52:36.000000 progfiguration-0.0.2a4/progfiguration/inventory/__init__.py
+-rw-------   0 mrled      (501) staff       (20)      874 2023-07-22 04:24:12.000000 progfiguration-0.0.2a4/progfiguration/inventory/nodes.py
+-rw-------   0 mrled      (501) staff       (20)     4613 2023-07-23 23:21:39.000000 progfiguration-0.0.2a4/progfiguration/inventory/roles.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 02:40:24.991064 progfiguration-0.0.2a4/progfiguration/localhost/
+-rw-------   0 mrled      (501) staff       (20)    11082 2023-07-23 23:21:13.000000 progfiguration-0.0.2a4/progfiguration/localhost/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     1184 2023-07-22 04:24:17.000000 progfiguration-0.0.2a4/progfiguration/localhost/authorized_keys.py
+-rw-------   0 mrled      (501) staff       (20)     6056 2023-07-22 04:24:20.000000 progfiguration-0.0.2a4/progfiguration/localhost/disks.py
+-rw-------   0 mrled      (501) staff       (20)     3044 2023-07-22 04:24:22.000000 progfiguration-0.0.2a4/progfiguration/localhost/localusers.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 02:40:24.992329 progfiguration-0.0.2a4/progfiguration/progfigbuild/
+-rw-r--r--   0 mrled      (501) staff       (20)    17352 2023-07-25 04:49:02.000000 progfiguration-0.0.2a4/progfiguration/progfigbuild/__init__.py
+-rw-r--r--   0 mrled      (501) staff       (20)     2505 2023-07-22 05:35:59.000000 progfiguration-0.0.2a4/progfiguration/progfigsite_validator.py
+-rw-------   0 mrled      (501) staff       (20)      912 2023-07-22 05:36:48.000000 progfiguration-0.0.2a4/progfiguration/progfigtypes.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 02:40:24.993739 progfiguration-0.0.2a4/progfiguration/remotebrute/
+-rw-------   0 mrled      (501) staff       (20)     3117 2023-07-22 04:24:58.000000 progfiguration-0.0.2a4/progfiguration/remotebrute/__init__.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 02:40:24.994802 progfiguration-0.0.2a4/progfiguration/sitewrapper/
+-rw-r--r--   0 mrled      (501) staff       (20)     3972 2023-07-22 04:26:29.000000 progfiguration-0.0.2a4/progfiguration/sitewrapper/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     1804 2023-07-22 05:39:58.000000 progfiguration-0.0.2a4/progfiguration/ssh.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 02:40:24.995829 progfiguration-0.0.2a4/progfiguration/temple/
+-rw-------   0 mrled      (501) staff       (20)      744 2023-06-28 22:11:55.000000 progfiguration-0.0.2a4/progfiguration/temple/__init__.py
+-rw-r--r--   0 mrled      (501) staff       (20)     1832 2023-07-23 22:41:01.000000 progfiguration-0.0.2a4/progfiguration/util.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 02:40:24.976678 progfiguration-0.0.2a4/progfiguration.egg-info/
+-rw-------   0 mrled      (501) staff       (20)     3109 2023-07-29 02:40:24.000000 progfiguration-0.0.2a4/progfiguration.egg-info/PKG-INFO
+-rw-------   0 mrled      (501) staff       (20)     1108 2023-07-29 02:40:24.000000 progfiguration-0.0.2a4/progfiguration.egg-info/SOURCES.txt
+-rw-------   0 mrled      (501) staff       (20)        1 2023-07-29 02:40:24.000000 progfiguration-0.0.2a4/progfiguration.egg-info/dependency_links.txt
+-rw-------   0 mrled      (501) staff       (20)       83 2023-07-29 02:40:24.000000 progfiguration-0.0.2a4/progfiguration.egg-info/entry_points.txt
+-rw-------   0 mrled      (501) staff       (20)      184 2023-07-29 02:40:24.000000 progfiguration-0.0.2a4/progfiguration.egg-info/requires.txt
+-rw-------   0 mrled      (501) staff       (20)       15 2023-07-29 02:40:24.000000 progfiguration-0.0.2a4/progfiguration.egg-info/top_level.txt
+-rw-------   0 mrled      (501) staff       (20)     1076 2023-07-29 02:37:38.000000 progfiguration-0.0.2a4/pyproject.toml
+-rw-------   0 mrled      (501) staff       (20)     2718 2023-07-29 02:39:31.000000 progfiguration-0.0.2a4/readme.md
+-rw-------   0 mrled      (501) staff       (20)       38 2023-07-29 02:40:25.000074 progfiguration-0.0.2a4/setup.cfg
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 02:40:24.998584 progfiguration-0.0.2a4/tests/
+-rw-------   0 mrled      (501) staff       (20)     1293 2023-07-22 04:15:43.000000 progfiguration-0.0.2a4/tests/test_cmd.py
+-rw-------   0 mrled      (501) staff       (20)     1778 2023-07-22 04:38:21.000000 progfiguration-0.0.2a4/tests/test_packaging.py
+-rw-------   0 mrled      (501) staff       (20)     2321 2023-07-19 14:30:38.000000 progfiguration-0.0.2a4/tests/test_site.py
```

### Comparing `progfiguration-0.0.2a3/PKG-INFO` & `progfiguration-0.0.2a4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: progfiguration
-Version: 0.0.2a3
+Version: 0.0.2a4
 Summary: PROGramatic conFIGURATION for your infrastructure
 Author-email: Micah R Ledbetter <me@micahrl.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mrled/progfiguration
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: development
+Provides-Extra: ghpages-builder
+License-File: LICENSE
 
 # progfiguration
 
 PROGrammatic conFIGURATION.
 I'm tired of writing YAML when what I want to write is Python.
 
 ## Building and publishing
@@ -21,31 +23,32 @@
 python3 -m venv venv
 # Enter the venv
 . venv/bin/activate
 # Make sure pip is recent - required for our pyproject.toml-only package
 python3 -m pip install --upgrade pip
 # Install this directory as editable, and include development dependencies
 python3 -m pip install --editable '.[development]'
-# Run the documentation server on port 8000
-pdoc -p 8000 progfiguration &
 # Run unit tests
 python3 -m unittest
 # Run progfiguration itself
 progfiguration --help
-# Build a source-only distribution of the package
-python3 -m build -s
-# Upload it to PyPI
-twine upload dist/*
 ```
 
 We only actually need to build a source version of the package,
 because progfiguration expects that your progfigsite package will pull in the source code.
 We avoid building the binary version because it takes longer.
 
-The pdoc webserver will live reload as you make changes.
+### Building the documentation
+
+```sh
+# Build the docs once, without running a webserver
+sphinx-build -b html docs/ docs/_build/html
+# Build the docs whenever a change is detected, and run a webserver that supports automatic live reload
+sphinx-autobuild docs docs/_build/html &
+```
 
 ## Testing
 
 After entering the venv (see above), run unit tests with `python3 -m unittest`.
 You can modify the test run with a few environment variables:
 
 * `PROGFIGURATION_TEST_DEBUG=1`: Launch a debugger on any test failure or exception
@@ -55,12 +58,37 @@
 ## Building the example sites
 
 In the same venv as above:
 
 ```sh
 # Install the example progfigsite
 python3 -m pip install --editable 'tests/data/simple[development]'
-# Run the documentation server for both progfiguration and the example progfigsite
-pdoc -p 8000 progfiguration tests/data/simple/example_site &
 # Run the progfigsite itself
 progfigsite --help
 ```
+
+## Making a release
+
+1.  Check out the `master` branch.
+    Make sure your checkout is clean, with all changes committed to git and pushed to Github
+2.  Set the version in `pyproject.toml`.
+    Don't commit the change yet.
+    We'll read this file to determine the version to tag in git and push to PyPI.
+    *   This will require Python 3.11 because we parse the TOML file directly with `tomllib`.
+    *   We can't use `progfiguration version` for this because it will return the version as it was at install time.
+3.  Run the following:
+
+```sh
+version="$(python -c 'import tomllib; f=open("./pyproject.toml", "rb"); proj=tomllib.load(f); print(proj["project"]["version"])')"
+
+git commit pyproject.toml -m "Release version $version"
+
+git tag "v${version}" master
+git push origin "v${version}"
+
+# Build a source-only distribution of the package
+python3 -m build -s
+# Upload it to PyPI
+twine upload "dist/progfiguration-${version}.tar.gz"
+```
+
+The documentation will be updated with the lastest version number and content as well via Github Actions.
```

### Comparing `progfiguration-0.0.2a3/progfiguration/__init__.py` & `progfiguration-0.0.2a4/progfiguration/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/progfiguration/age.py` & `progfiguration-0.0.2a4/progfiguration/age.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/progfiguration/cli/progfiguration_core_cmd.py` & `progfiguration-0.0.2a4/progfiguration/cli/progfiguration_core_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,24 +31,27 @@
         progfigsite_filesystem_path = pathlib.Path(progfigsite.__file__).parent
     else:
         parser.error(f"Missing progfigsite path option")
 
     return (progfigsite, progfigsite_module_path, progfigsite_filesystem_path)
 
 
-def _action_version_core():
+def _action_version_core(quiet: bool = False):
     """Retrieve the version of progfiguration core"""
 
     coreversion = importlib.metadata.version("progfiguration")
-    result = [
-        f"progfiguration core:",
-        f"    path: {pathlib.Path(progfiguration.__file__).parent}",
-        f"    version: {coreversion}",
-    ]
-    print("\n".join(result))
+    if quiet:
+        print(coreversion)
+    else:
+        result = [
+            f"progfiguration core:",
+            f"    path: {pathlib.Path(progfiguration.__file__).parent}",
+            f"    version: {coreversion}",
+        ]
+        print("\n".join(result))
 
 
 def _action_validate(module_path: str):
     """Validate a progfigsite module
 
     Arguments:
         module_path -- The Python path to the progfigsite module
@@ -92,15 +95,16 @@
         type=str,
         help="The python path to a progfigsite package, like 'my_progfigsite' or 'one.two.three.progfigsite'. If neither this nor --progfigsite-filesystem-path is passed, look for a 'progfigsite' package in the Python path.",
     )
 
     subparsers = parser.add_subparsers(dest="action", required=True)
 
     # version-core subcommand
-    svn_core = subparsers.add_parser("version", description="Show progfiguration core version")
+    svn = subparsers.add_parser("version", description="Show progfiguration core version")
+    svn.add_argument("--quiet", "-q", action="store_true", help="Only print the version string")
 
     # build subcommand
     sub_build = subparsers.add_parser("build", parents=[site_opts], description="Build the package")
     sub_build_subparsers = sub_build.add_subparsers(dest="buildaction", required=True)
     sub_build_sub_pyz = sub_build_subparsers.add_parser(
         "pyz",
         description="Build a zipapp .pyz file containing the Python module. Must be run from an editable install.",
@@ -137,15 +141,15 @@
     parsed = parser.parse_args(arguments[1:])
 
     if parsed.debug:
         sys.excepthook = idb_excepthook
     configure_logging(parsed.log_stderr)
 
     if parsed.action == "version":
-        _action_version_core()
+        _action_version_core(quiet=parsed.quiet)
     elif parsed.action == "build":
         progfigsite, progfigsite_modpath, progfigsite_fspath = _find_progfigsite_module(parser, parsed)
         # TODO: how will sites extend this?
         if parsed.buildaction == "pyz":
             progfigbuild.build_progfigsite_zipapp(progfigsite_fspath, parsed.pyzfile)
         elif parsed.buildaction == "pip":
             progfigbuild.build_progfigsite_pip(
```

### Comparing `progfiguration-0.0.2a3/progfiguration/cli/progfiguration_site_cmd.py` & `progfiguration-0.0.2a4/progfiguration/cli/progfiguration_site_cmd.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/progfiguration/cli/util.py` & `progfiguration-0.0.2a4/progfiguration/cli/util.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/progfiguration/cmd.py` & `progfiguration-0.0.2a4/progfiguration/cmd.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/progfiguration/inventory/__init__.py` & `progfiguration-0.0.2a4/progfiguration/inventory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         TODO: weird API, maybe get rid of the .controller property
         """
 
         # Get the age key path for this node, if the node is specified and has a key defined
         current_node_age_key_path = None
         if current_node is not None:
             try:
-                current_node_age_key_path = self.node(current_node).age_key_path
+                current_node_age_key_path = self.node(current_node).node.age_key_path
             except (KeyError, ModuleNotFoundError):
                 pass
 
         def maybe_get_age_path() -> Optional[str]:
             """Find the age path to a private key if possible
 
             Lookup order, highest priority first:
```

### Comparing `progfiguration-0.0.2a3/progfiguration/inventory/nodes.py` & `progfiguration-0.0.2a4/progfiguration/inventory/nodes.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/progfiguration/inventory/roles.py` & `progfiguration-0.0.2a4/progfiguration/inventory/roles.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/progfiguration/localhost/__init__.py` & `progfiguration-0.0.2a4/progfiguration/localhost/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/progfiguration/localhost/authorized_keys.py` & `progfiguration-0.0.2a4/progfiguration/localhost/authorized_keys.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/progfiguration/localhost/disks.py` & `progfiguration-0.0.2a4/progfiguration/localhost/disks.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/progfiguration/localhost/localusers.py` & `progfiguration-0.0.2a4/progfiguration/localhost/localusers.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/progfiguration/progfigbuild/__init__.py` & `progfiguration-0.0.2a4/progfiguration/progfigbuild/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,44 +45,42 @@
     package_out_path: pathlib.Path,
     build_date: Optional[datetime] = None,
     progfiguration_package_path: Optional[pathlib.Path] = None,
     compression: int = zipfile.ZIP_STORED,
 ):
     """Build a .pyz zipapp progfigsite package
 
-    Args:
-        progfigsite_filesystem_path: The path to the progfigsite package, eg "/path/to/progfigsite"
-        package_out_path: The path where the zipfile will be written.
-        build_date: The build date to embed in the zipapp.
-            If None, the current UTC time will be used.
-        progfiguration_package_path: The path to the progfiguration package, eg "/path/to/progfiguration"
-            If None, the progfiguration package will be copied from the Python path.
-            This will only work if progfiguration is installed via pip
-            (probably in a venv, possibly editable with 'pip install -e')...
-            it won't work if you're running progfiguration itself from a zipapp for some reason.
-        compression: The compression level to use for the zipapp file.
-            This can be zipfile.ZIP_STORED (no compression) or zipfile.ZIP_DEFLATED (deflate compression).
-            ZIP_STORED (the default) is faster.
+    :param progfigsite_filesystem_path: The path to the progfigsite package, eg "/path/to/progfigsite".
+    :param package_out_path: The path where the zipfile will be written.
+    :param build_date: The build date to embed in the zipapp.
+        If None, the current UTC time will be used.
+    :param progfiguration_package_path: The path to the progfiguration package, eg "/path/to/progfiguration".
+        If None, the progfiguration package will be copied from the Python path.
+        This will only work if progfiguration is installed via pip
+        (probably in a venv, possibly editable with 'pip install -e')...
+        it won't work if you're running progfiguration itself from a zipapp for some reason.
+    :param compression: The compression level to use for the zipapp file.
+        This can be zipfile.ZIP_STORED (no compression) or zipfile.ZIP_DEFLATED (deflate compression).
+        ZIP_STORED (the default) is faster.
 
-    Returns:
-        The path to the zipapp file, eg "/path/to/my_progfigsite.pyz"
+    :return: The path to the zipapp file, eg "/path/to/my_progfigsite.pyz".
 
     What this function does:
 
     * Zip up the contents of the site package.
     * Place them inside a subdirectory called 'progfigsite'.
     * Add a __main__.py file to the root of the zip file.
     * Add the progfiguration package to the zip file.
     * Add a shebang to the beginning of the zip file.
 
     Inspired by the zipapp module code
     <https://github.com/python/cpython/blob/3.11/Lib/zipapp.py>
 
     We don't use the zipapp code itself because we want more control over what goes into the zipfile,
-    like ignoring __pycache__, *.dist-info, etc.
+    like ignoring __pycache__, \*.dist-info, etc.
 
     We don't need the ProgfigsitePythonPackagePreparer context manager here,
     because we don't need to inject build data into the filesystem before building the zipapp.
     We can inject the build data directly into the zipapp file.
     """
 
     if progfiguration_package_path is None:
@@ -178,24 +176,24 @@
     (see `progfigsite_project_path` and `progfigsite_filesystem_path` properties),
     and injecting build data into the filesystem
     like a version from progfigsite's `mint_version()` and the build date.
     When the context manager exits, the injected files are removed.
 
     You can use this to build a pip package with build and setuptools like this:
 
-    ```python
-    with ProgfigsitePythonPackagePreparer("/path/to/progfigsite") as preparer:
-        result = subprocess.run(
-            ["python", "-m", "build", "-s", "-o", preparer.package_out_path.as_posix(), preparer.progfigsite_project_path.as_posix()],
-            check=True,
-            capture_output=True,
-            cwd=preparer.progfigsite_project_path,
-        )
-    built_package_path = result.stdout.read()
-    ```
+    .. code-block:: python
+
+        with ProgfigsitePythonPackagePreparer("/path/to/progfigsite") as preparer:
+            result = subprocess.run(
+                ["python", "-m", "build", "-s", "-o", preparer.package_out_path.as_posix(), preparer.progfigsite_project_path.as_posix()],
+                check=True,
+                capture_output=True,
+                cwd=preparer.progfigsite_project_path,
+            )
+        built_package_path = result.stdout.read()
 
     See the implementation of `build_progfigsite_pip()` for a more complete example.
 
     If you want to modify the build in some way,
     or build another kind of package after we prepare the filesystem and inject build data,
     you can do that instead.
 
@@ -208,30 +206,30 @@
         progfigsite_filesystem_path: pathlib.Path,
         build_date: Optional[datetime] = None,
         progfiguration_package_path: Optional[pathlib.Path] = None,
         injections: Optional[List[InjectedFile]] = None,
         keep_injected_files: bool = False,
     ):
         """
-        Args:
-            progfigsite_filesystem_path: The path to the progfigsite package, eg "/path/to/progfigsite/src".
-            build_date: The build date to inject into the package.
-                If None, the current date will be used.
-            progfiguration_package_path: The path to the progfiguration package, eg "/path/to/progfiguration".
-                If None, the progfiguration package will be copied from the Python path.
-                This will only work if progfiguration is installed to the Python path
-                (probably by pip in a venv, and possibly editable with 'pip install -e').
-            injections: Build data we will inject into the filesystem before building the pip package.
-                These injections can go anywhere in the filesystem --
-                they aren't limited to the progfigsite package.
-                You can inject files into the project directory (containing the pyproject.toml),
-                the package directory (containing the actual Python package),
-                or maybe even somewhere else entirely.
-            keep_injected_files: If True, the injected files will be kept after the package is built.
-                You will need to remove them manually. Intended for debugging.
+
+        :param progfigsite_filesystem_path: The path to the progfigsite package, eg "/path/to/progfigsite/src".
+        :param build_date: The build date to inject into the package.
+            If None, the current date will be used.
+        :param progfiguration_package_path: The path to the progfiguration package, eg "/path/to/progfiguration".
+            If None, the progfiguration package will be copied from the Python path.
+            This will only work if progfiguration is installed to the Python path
+            (probably by pip in a venv, and possibly editable with 'pip install -e').
+        :param injections: Build data we will inject into the filesystem before building the pip package.
+            These injections can go anywhere in the filesystem --
+            they aren't limited to the progfigsite package.
+            You can inject files into the project directory (containing the pyproject.toml),
+            the package directory (containing the actual Python package),
+            or maybe even somewhere else entirely.
+        :param keep_injected_files: If True, the injected files will be kept after the package is built.
+            You will need to remove them manually. Intended for debugging.
         """
 
         self.progfigsite_filesystem_path = progfigsite_filesystem_path
         """The filesystem path to the progfigsite package, eg `/path/to/progfigsite/src`
 
         This PACKAGE directory should be the path to the Python package itself with an `__init__.py`.
         It might be inside a subfolder like "src" or "progfigsite" inside the PROJECT directory,
@@ -353,30 +351,28 @@
     package_out_path: pathlib.Path,
     build_date: Optional[datetime] = None,
     progfiguration_package_path: Optional[pathlib.Path] = None,
     keep_injected_files: bool = False,
 ) -> pathlib.Path:
     """Build a pip package
 
-    Args:
-        progfigsite_filesystem_path: The path to the progfigsite package, eg "/path/to/progfigsite"
-        package_out_path: The path where the zipfile will be written.
-        build_date: The build date to inject into the package.
-            If None, the current date will be used.
-        progfiguration_package_path: The path to the progfiguration package, eg "/path/to/progfiguration"
-            If None, the progfiguration package will be copied from the Python path.
-            This will only work if progfiguration is installed via pip
-            (probably in a venv, possibly editable with 'pip install -e')...
-            it won't work if you're running progfiguration itself from a zipapp for some reason.
-        keep_injected_files: If True, the injected files will be kept after the package is built.
-            You will need to remove them manually.
-            Intended for debugging.
+    :param progfigsite_filesystem_path: The path to the progfigsite package, eg "/path/to/progfigsite".
+    :param package_out_path: The path where the zipfile will be written.
+    :param build_date: The build date to inject into the package.
+        If None, the current date will be used.
+    :param progfiguration_package_path: The path to the progfiguration package, eg "/path/to/progfiguration".
+        If None, the progfiguration package will be copied from the Python path.
+        This will only work if progfiguration is installed via pip
+        (probably in a venv, possibly editable with 'pip install -e')...
+        it won't work if you're running progfiguration itself from a zipapp for some reason.
+    :param keep_injected_files: If True, the injected files will be kept after the package is built.
+        You will need to remove them manually.
+        Intended for debugging.
 
-    Returns:
-        The path to the pip package, eg "/path/to/my_progfigsite/dist/my_progfigsite-0.1.0.tar.gz"
+    :return: The path to the pip package, eg "/path/to/my_progfigsite/dist/my_progfigsite-0.1.0.tar.gz"
     """
 
     with ProgfigsitePythonPackagePreparer(
         progfigsite_filesystem_path,
         build_date=build_date,
         progfiguration_package_path=progfiguration_package_path,
         keep_injected_files=keep_injected_files,
```

### Comparing `progfiguration-0.0.2a3/progfiguration/progfigsite_validator.py` & `progfiguration-0.0.2a4/progfiguration/progfigsite_validator.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/progfiguration/progfigtypes.py` & `progfiguration-0.0.2a4/progfiguration/progfigtypes.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/progfiguration/remotebrute/__init__.py` & `progfiguration-0.0.2a4/progfiguration/remotebrute/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/progfiguration/sitewrapper/__init__.py` & `progfiguration-0.0.2a4/progfiguration/sitewrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/progfiguration/ssh.py` & `progfiguration-0.0.2a4/progfiguration/ssh.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/progfiguration/temple/__init__.py` & `progfiguration-0.0.2a4/progfiguration/temple/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/progfiguration/util.py` & `progfiguration-0.0.2a4/progfiguration/util.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/progfiguration.egg-info/PKG-INFO` & `progfiguration-0.0.2a4/progfiguration.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: progfiguration
-Version: 0.0.2a3
+Version: 0.0.2a4
 Summary: PROGramatic conFIGURATION for your infrastructure
 Author-email: Micah R Ledbetter <me@micahrl.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mrled/progfiguration
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: development
+Provides-Extra: ghpages-builder
+License-File: LICENSE
 
 # progfiguration
 
 PROGrammatic conFIGURATION.
 I'm tired of writing YAML when what I want to write is Python.
 
 ## Building and publishing
@@ -21,31 +23,32 @@
 python3 -m venv venv
 # Enter the venv
 . venv/bin/activate
 # Make sure pip is recent - required for our pyproject.toml-only package
 python3 -m pip install --upgrade pip
 # Install this directory as editable, and include development dependencies
 python3 -m pip install --editable '.[development]'
-# Run the documentation server on port 8000
-pdoc -p 8000 progfiguration &
 # Run unit tests
 python3 -m unittest
 # Run progfiguration itself
 progfiguration --help
-# Build a source-only distribution of the package
-python3 -m build -s
-# Upload it to PyPI
-twine upload dist/*
 ```
 
 We only actually need to build a source version of the package,
 because progfiguration expects that your progfigsite package will pull in the source code.
 We avoid building the binary version because it takes longer.
 
-The pdoc webserver will live reload as you make changes.
+### Building the documentation
+
+```sh
+# Build the docs once, without running a webserver
+sphinx-build -b html docs/ docs/_build/html
+# Build the docs whenever a change is detected, and run a webserver that supports automatic live reload
+sphinx-autobuild docs docs/_build/html &
+```
 
 ## Testing
 
 After entering the venv (see above), run unit tests with `python3 -m unittest`.
 You can modify the test run with a few environment variables:
 
 * `PROGFIGURATION_TEST_DEBUG=1`: Launch a debugger on any test failure or exception
@@ -55,12 +58,37 @@
 ## Building the example sites
 
 In the same venv as above:
 
 ```sh
 # Install the example progfigsite
 python3 -m pip install --editable 'tests/data/simple[development]'
-# Run the documentation server for both progfiguration and the example progfigsite
-pdoc -p 8000 progfiguration tests/data/simple/example_site &
 # Run the progfigsite itself
 progfigsite --help
 ```
+
+## Making a release
+
+1.  Check out the `master` branch.
+    Make sure your checkout is clean, with all changes committed to git and pushed to Github
+2.  Set the version in `pyproject.toml`.
+    Don't commit the change yet.
+    We'll read this file to determine the version to tag in git and push to PyPI.
+    *   This will require Python 3.11 because we parse the TOML file directly with `tomllib`.
+    *   We can't use `progfiguration version` for this because it will return the version as it was at install time.
+3.  Run the following:
+
+```sh
+version="$(python -c 'import tomllib; f=open("./pyproject.toml", "rb"); proj=tomllib.load(f); print(proj["project"]["version"])')"
+
+git commit pyproject.toml -m "Release version $version"
+
+git tag "v${version}" master
+git push origin "v${version}"
+
+# Build a source-only distribution of the package
+python3 -m build -s
+# Upload it to PyPI
+twine upload "dist/progfiguration-${version}.tar.gz"
+```
+
+The documentation will be updated with the lastest version number and content as well via Github Actions.
```

### Comparing `progfiguration-0.0.2a3/progfiguration.egg-info/SOURCES.txt` & `progfiguration-0.0.2a4/progfiguration.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 pyproject.toml
 readme.md
 progfiguration/__init__.py
 progfiguration/age.py
 progfiguration/cmd.py
 progfiguration/progfigsite_validator.py
 progfiguration/progfigtypes.py
```

### Comparing `progfiguration-0.0.2a3/pyproject.toml` & `progfiguration-0.0.2a4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,51 @@
 [build-system]
-requires = [
-    "pdoc",
-    "setuptools",
-]
+requires = ["pdoc", "setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "progfiguration"
-version = "0.0.2a3"
+version = "0.0.2a4"
 description = "PROGramatic conFIGURATION for your infrastructure"
-license = {text = "MIT"}
+license = { text = "MIT" }
 readme = "readme.md"
 requires-python = ">=3.10"
 
 [[project.authors]]
 name = "Micah R Ledbetter"
 email = "me@micahrl.com"
 
 [project.scripts]
 progfiguration = "progfiguration.cli.progfiguration_core_cmd:main"
 
 [project.optional-dependencies]
+
+# Used for local development
 development = [
     "black",
     "build",
+    "furo",             # Sphinx theme
     "mypy",
-    "pdoc",
+    "myst_parser",      # markdown support in Sphinx
+    "sphinx",
+    "sphinx-argparse",
+    "sphinx-autoapi",
+    "sphinx-autobuild",
     "twine",
 ]
 
+# Used by our Github Actions workflow to autopublish documentation
+ghpages-builder = [
+    "furo",
+    "myst_parser",
+    "sphinx",
+    "sphinx-argparse",
+    "sphinx-autoapi",
+]
+
 [project.urls]
 Homepage = "https://github.com/mrled/progfiguration"
 
 [tool.black]
 line-length = 120
 
 [tool.setuptools.package-data]
```

### Comparing `progfiguration-0.0.2a3/tests/test_cmd.py` & `progfiguration-0.0.2a4/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/tests/test_packaging.py` & `progfiguration-0.0.2a4/tests/test_packaging.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a3/tests/test_site.py` & `progfiguration-0.0.2a4/tests/test_site.py`

 * *Files identical despite different names*

