# Comparing `tmp/beewi_smartclim_ble-0.3.0.tar.gz` & `tmp/beewi_smartclim_ble-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beewi_smartclim_ble-0.3.0.tar", max compression
+gzip compressed data, was "beewi_smartclim_ble-0.4.0.tar", max compression
```

## Comparing `beewi_smartclim_ble-0.3.0.tar` & `beewi_smartclim_ble-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1067 2023-06-29 21:07:43.152213 beewi_smartclim_ble-0.3.0/LICENSE
--rw-r--r--   0        0        0     2477 2023-06-29 21:07:43.152213 beewi_smartclim_ble-0.3.0/README.md
--rw-r--r--   0        0        0     2257 2023-06-29 21:07:44.120238 beewi_smartclim_ble-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      122 2023-06-29 21:07:44.088237 beewi_smartclim_ble-0.3.0/src/smartclim_ble/__init__.py
--rw-r--r--   0        0        0     7106 2023-06-29 21:07:43.152213 beewi_smartclim_ble-0.3.0/src/smartclim_ble/parser.py
--rw-r--r--   0        0        0        0 2023-06-29 21:07:43.152213 beewi_smartclim_ble-0.3.0/src/smartclim_ble/py.typed
--rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 beewi_smartclim_ble-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-28 22:55:07.723258 beewi_smartclim_ble-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2477 2023-07-28 22:55:07.723258 beewi_smartclim_ble-0.4.0/README.md
+-rw-r--r--   0        0        0     2525 2023-07-28 22:55:08.499273 beewi_smartclim_ble-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      482 2023-07-28 22:55:08.467273 beewi_smartclim_ble-0.4.0/src/smartclim_ble/__init__.py
+-rw-r--r--   0        0        0      529 2023-07-28 22:55:07.723258 beewi_smartclim_ble-0.4.0/src/smartclim_ble/const.py
+-rw-r--r--   0        0        0     4534 2023-07-28 22:55:07.723258 beewi_smartclim_ble-0.4.0/src/smartclim_ble/parser.py
+-rw-r--r--   0        0        0        0 2023-07-28 22:55:07.723258 beewi_smartclim_ble-0.4.0/src/smartclim_ble/py.typed
+-rw-r--r--   0        0        0     3993 1970-01-01 00:00:00.000000 beewi_smartclim_ble-0.4.0/PKG-INFO
```

### Comparing `beewi_smartclim_ble-0.3.0/LICENSE` & `beewi_smartclim_ble-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beewi_smartclim_ble-0.3.0/README.md` & `beewi_smartclim_ble-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `beewi_smartclim_ble-0.3.0/pyproject.toml` & `beewi_smartclim_ble-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beewi-smartclim-ble"
-version = "0.3.0"
+version = "0.4.0"
 description = "Parser for the BeeWi SmartClim device"
 authors = ["f-davin <none@none.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/f-davin/hassis_beewi_smartclim.git"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
@@ -19,14 +19,20 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/f-davin/hassis_beewi_smartclim/issues"
 "Changelog" = "https://github.com/f-davin/hassis_beewi_smartclim/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
+
+home-assistant-bluetooth = ">=1.9.2"
+sensor-state-data = ">=2.17.1"
+bluetooth-sensor-state-data = ">=1.6.0"
+bleak-retry-connector = ">=2.13.0"
+bluetooth-data-tools = ">=0.3.1"
 bleak = ">=0.19.5"
 
 # Documentation Dependencies
 Sphinx = {version = "^5.0", optional = true}
 sphinx-rtd-theme = {version = "^1.0", optional = true}
 myst-parser = {version = "^0.18", optional = true}
 
@@ -36,14 +42,19 @@
     "sphinx",
     "sphinx-rtd-theme",
 ]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0"
 pytest-cov = "^3.0"
+black = "^23.3.0"
+isort = "^5.12.0"
+flake8 = "^6.0.0"
+mypy = "^1.3.0"
+pyupgrade = "^3.4.0"
 
 [tool.semantic_release]
 branch = "master"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/smartclim_ble/__init__.py:__version__"
 build_command = "pip install poetry && poetry build"
```

### Comparing `beewi_smartclim_ble-0.3.0/PKG-INFO` & `beewi_smartclim_ble-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beewi-smartclim-ble
-Version: 0.3.0
+Version: 0.4.0
 Summary: Parser for the BeeWi SmartClim device
 Home-page: https://github.com/f-davin/hassis_beewi_smartclim.git
 License: MIT
 Author: f-davin
 Author-email: none@none.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -16,15 +16,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=5.0,<6.0) ; extra == "docs"
 Requires-Dist: bleak (>=0.19.5)
+Requires-Dist: bleak-retry-connector (>=2.13.0)
+Requires-Dist: bluetooth-data-tools (>=0.3.1)
+Requires-Dist: bluetooth-sensor-state-data (>=1.6.0)
+Requires-Dist: home-assistant-bluetooth (>=1.9.2)
 Requires-Dist: myst-parser (>=0.18,<0.19) ; extra == "docs"
+Requires-Dist: sensor-state-data (>=2.17.1)
 Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0) ; extra == "docs"
 Project-URL: Bug Tracker, https://github.com/f-davin/hassis_beewi_smartclim/issues
 Project-URL: Changelog, https://github.com/f-davin/hassis_beewi_smartclim/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/f-davin/hassis_beewi_smartclim.git
 Description-Content-Type: text/markdown
 
 # BeeWi SmartClim BLE
```

