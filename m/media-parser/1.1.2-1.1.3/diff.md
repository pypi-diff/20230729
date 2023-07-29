# Comparing `tmp/media_parser-1.1.2.tar.gz` & `tmp/media_parser-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "media_parser-1.1.2.tar", max compression
+gzip compressed data, was "media_parser-1.1.3.tar", max compression
```

## Comparing `media_parser-1.1.2.tar` & `media_parser-1.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-07-29 02:19:44.797637 media_parser-1.1.2/LICENSE
--rw-r--r--   0        0        0     3046 2023-07-29 02:19:44.797637 media_parser-1.1.2/README.md
--rw-r--r--   0        0        0      273 2023-07-29 02:19:44.801637 media_parser-1.1.2/media_parser/__init__.py
--rw-r--r--   0        0        0     2280 2023-07-29 02:19:44.801637 media_parser-1.1.2/media_parser/client.py
--rw-r--r--   0        0        0      307 2023-07-29 02:19:44.801637 media_parser-1.1.2/media_parser/models/__init__.py
--rw-r--r--   0        0        0     4358 2023-07-29 02:19:44.801637 media_parser-1.1.2/media_parser/models/medias.py
--rw-r--r--   0        0        0     1405 2023-07-29 02:19:44.801637 media_parser-1.1.2/media_parser/models/server.py
--rw-r--r--   0        0        0     3039 2023-07-29 02:19:44.805637 media_parser-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     4991 1970-01-01 00:00:00.000000 media_parser-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-29 03:06:36.165151 media_parser-1.1.3/LICENSE
+-rw-r--r--   0        0        0     3683 2023-07-29 03:06:36.165151 media_parser-1.1.3/README.md
+-rw-r--r--   0        0        0      273 2023-07-29 03:06:36.169152 media_parser-1.1.3/media_parser/__init__.py
+-rw-r--r--   0        0        0     2280 2023-07-29 03:06:36.169152 media_parser-1.1.3/media_parser/client.py
+-rw-r--r--   0        0        0      307 2023-07-29 03:06:36.169152 media_parser-1.1.3/media_parser/models/__init__.py
+-rw-r--r--   0        0        0     4358 2023-07-29 03:06:36.169152 media_parser-1.1.3/media_parser/models/medias.py
+-rw-r--r--   0        0        0     1405 2023-07-29 03:06:36.169152 media_parser-1.1.3/media_parser/models/server.py
+-rw-r--r--   0        0        0     2997 2023-07-29 03:06:36.173152 media_parser-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5628 1970-01-01 00:00:00.000000 media_parser-1.1.3/PKG-INFO
```

### Comparing `media_parser-1.1.2/LICENSE` & `media_parser-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `media_parser-1.1.2/README.md` & `media_parser-1.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Media Parser
 
+[![Documentation Status](https://readthedocs.org/projects/media-parser/badge/?version=latest)](https://media-parser.readthedocs.io/?badge=latest)
+[![Build Docker image](https://github.com/jag-k/media-parser/actions/workflows/docker-image.yml/badge.svg)](https://github.com/jag-k/media-parser/actions/workflows/docker-image.yml)
+[![PyPI publish](https://github.com/jag-k/media-parser/actions/workflows/pypi-publish.yml/badge.svg)](https://github.com/jag-k/media-parser/actions/workflows/pypi-publish.yml)
+[![PyPI version](https://img.shields.io/pypi/v/media-parser?logo=pypi&label=media-parser)](https://pypi.org/project/media-parsers/)
+
 Server for parse Media by URL.
 
 ## Supported medias
 
 - [x] Youtube
 - [x] Tiktok
 - [x] Instagram
```

### Comparing `media_parser-1.1.2/media_parser/client.py` & `media_parser-1.1.3/media_parser/client.py`

 * *Files identical despite different names*

### Comparing `media_parser-1.1.2/media_parser/models/medias.py` & `media_parser-1.1.3/media_parser/models/medias.py`

 * *Files identical despite different names*

### Comparing `media_parser-1.1.2/media_parser/models/server.py` & `media_parser-1.1.3/media_parser/models/server.py`

 * *Files identical despite different names*

### Comparing `media_parser-1.1.2/pyproject.toml` & `media_parser-1.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "media-parser"
-version = "1.1.2"
+version = "1.1.3"
 description = "API for parsing media from social networks"
 authors = ["Jag_k <me@jagk.dev>"]
 maintainers = ["Jag_k <me@jagk.dev>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: FastAPI",
     "Framework :: Pydantic",
@@ -60,15 +60,15 @@
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.1.1"
 furo = "^2023.7.26"
 sphinxext-opengraph = "^0.8.2"
 sphinx-copybutton = "^0.5.2"
 sphinx-inline-tabs = "^2023.4.21"
 myst-parser = "^2.0.0"
-sphinx-autodoc2 = {git = "https://github.com/jag-k/sphinx-autodoc2"}
+sphinx-autodoc2 = "^0.4.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `media_parser-1.1.2/PKG-INFO` & `media_parser-1.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: media-parser
-Version: 1.1.2
+Version: 1.1.3
 Summary: API for parsing media from social networks
 Home-page: https://github.com/jag-k/media-parser#readme
 License: MIT
 Keywords: media-parser,poetry,tiktok,youtube,reddit,twitter
 Author: Jag_k
 Author-email: me@jagk.dev
 Maintainer: Jag_k
@@ -39,14 +39,19 @@
 Requires-Dist: uvicorn (>=0.23.1,<0.24.0) ; extra == "server" or extra == "all"
 Project-URL: Documentation, https://media-parser.rtfd.io
 Project-URL: Repository, https://github.com/jag-k/media-parser
 Description-Content-Type: text/markdown
 
 # Media Parser
 
+[![Documentation Status](https://readthedocs.org/projects/media-parser/badge/?version=latest)](https://media-parser.readthedocs.io/?badge=latest)
+[![Build Docker image](https://github.com/jag-k/media-parser/actions/workflows/docker-image.yml/badge.svg)](https://github.com/jag-k/media-parser/actions/workflows/docker-image.yml)
+[![PyPI publish](https://github.com/jag-k/media-parser/actions/workflows/pypi-publish.yml/badge.svg)](https://github.com/jag-k/media-parser/actions/workflows/pypi-publish.yml)
+[![PyPI version](https://img.shields.io/pypi/v/media-parser?logo=pypi&label=media-parser)](https://pypi.org/project/media-parsers/)
+
 Server for parse Media by URL.
 
 ## Supported medias
 
 - [x] Youtube
 - [x] Tiktok
 - [x] Instagram
```

