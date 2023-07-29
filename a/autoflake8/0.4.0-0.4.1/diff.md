# Comparing `tmp/autoflake8-0.4.0.tar.gz` & `tmp/autoflake8-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoflake8-0.4.0.tar", max compression
+gzip compressed data, was "autoflake8-0.4.1.tar", max compression
```

## Comparing `autoflake8-0.4.0.tar` & `autoflake8-0.4.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0      553 2022-08-24 05:58:46.644981 autoflake8-0.4.0/AUTHORS.rst
--rw-r--r--   0        0        0     1061 2022-08-24 05:58:46.644981 autoflake8-0.4.0/LICENSE
--rw-r--r--   0        0        0     5317 2022-08-24 05:58:46.644981 autoflake8-0.4.0/README.md
--rw-r--r--   0        0        0       58 2022-08-24 05:58:46.648981 autoflake8-0.4.0/autoflake8/__init__.py
--rw-r--r--   0        0        0     4894 2022-08-24 05:58:46.648981 autoflake8-0.4.0/autoflake8/cli.py
--rw-r--r--   0        0        0    24135 2022-08-24 05:58:46.648981 autoflake8-0.4.0/autoflake8/fix.py
--rw-r--r--   0        0        0     5916 2022-08-24 05:58:46.648981 autoflake8-0.4.0/autoflake8/multiline.py
--rw-r--r--   0        0        0     1088 2022-08-24 05:58:46.648981 autoflake8-0.4.0/autoflake8/pending_fix.py
--rw-r--r--   0        0        0     1261 2022-08-24 05:58:46.648981 autoflake8-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6318 2022-08-24 05:59:16.617551 autoflake8-0.4.0/setup.py
--rw-r--r--   0        0        0     6290 2022-08-24 05:59:16.618279 autoflake8-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      553 2023-07-29 01:13:29.287170 autoflake8-0.4.1/AUTHORS.rst
+-rw-r--r--   0        0        0     1061 2023-07-29 01:13:29.287170 autoflake8-0.4.1/LICENSE
+-rw-r--r--   0        0        0      111 2023-07-29 01:13:29.287170 autoflake8-0.4.1/README.md
+-rw-r--r--   0        0        0       58 2023-07-29 01:13:29.287170 autoflake8-0.4.1/autoflake8/__init__.py
+-rw-r--r--   0        0        0     4894 2023-07-29 01:13:29.287170 autoflake8-0.4.1/autoflake8/cli.py
+-rw-r--r--   0        0        0    24135 2023-07-29 01:13:29.287170 autoflake8-0.4.1/autoflake8/fix.py
+-rw-r--r--   0        0        0     5916 2023-07-29 01:13:29.287170 autoflake8-0.4.1/autoflake8/multiline.py
+-rw-r--r--   0        0        0     1088 2023-07-29 01:13:29.287170 autoflake8-0.4.1/autoflake8/pending_fix.py
+-rw-r--r--   0        0        0     1262 2023-07-29 01:13:29.287170 autoflake8-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1135 1970-01-01 00:00:00.000000 autoflake8-0.4.1/PKG-INFO
```

### Comparing `autoflake8-0.4.0/AUTHORS.rst` & `autoflake8-0.4.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `autoflake8-0.4.0/LICENSE` & `autoflake8-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autoflake8-0.4.0/autoflake8/cli.py` & `autoflake8-0.4.1/autoflake8/cli.py`

 * *Files identical despite different names*

### Comparing `autoflake8-0.4.0/autoflake8/fix.py` & `autoflake8-0.4.1/autoflake8/fix.py`

 * *Files identical despite different names*

### Comparing `autoflake8-0.4.0/autoflake8/multiline.py` & `autoflake8-0.4.1/autoflake8/multiline.py`

 * *Files identical despite different names*

### Comparing `autoflake8-0.4.0/autoflake8/pending_fix.py` & `autoflake8-0.4.1/autoflake8/pending_fix.py`

 * *Files identical despite different names*

### Comparing `autoflake8-0.4.0/pyproject.toml` & `autoflake8-0.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoflake8"
-version = "0.4.0"
+version = "0.4.1"
 description = "Tool to automatically fix some issues reported by flake8 (forked from autoflake)."
 authors = [
   "Francisco Souza <fsouza@users.noreply.github.com>",
 ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/fsouza/autoflake8"
@@ -32,17 +32,17 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pyflakes = ">= 2.3.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
-pytest-xdist = "^2.5.0"
-aiofiles = "^0.8.0"
+pytest = "^7.4.0"
+pytest-xdist = "^3.3.1"
+aiofiles = "^23.1.0"
 
 [tool.poetry.scripts]
 autoflake8 = "autoflake8.cli:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

