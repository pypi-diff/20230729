# Comparing `tmp/nanoatp-0.3.4.tar.gz` & `tmp/nanoatp-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanoatp-0.3.4.tar", max compression
+gzip compressed data, was "nanoatp-0.3.5.tar", max compression
```

## Comparing `nanoatp-0.3.4.tar` & `nanoatp-0.3.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-02-24 19:04:39.038224 nanoatp-0.3.4/LICENSE
--rw-r--r--   0        0        0     4631 2023-04-29 17:30:20.383087 nanoatp-0.3.4/README.md
--rw-r--r--   0        0        0      283 2023-04-29 17:30:20.383570 nanoatp-0.3.4/nanoatp/__init__.py
--rw-r--r--   0        0        0     8669 2023-04-29 17:13:39.383183 nanoatp-0.3.4/nanoatp/bskyagent.py
--rw-r--r--   0        0        0     3034 2023-04-26 09:39:42.752327 nanoatp-0.3.4/nanoatp/richtext.py
--rw-r--r--   0        0        0      888 2023-04-29 17:30:20.384482 nanoatp-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     5477 1970-01-01 00:00:00.000000 nanoatp-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-24 19:04:39.038224 nanoatp-0.3.5/LICENSE
+-rw-r--r--   0        0        0     4631 2023-04-29 17:30:20.383087 nanoatp-0.3.5/README.md
+-rw-r--r--   0        0        0      283 2023-07-29 20:30:44.674736 nanoatp-0.3.5/nanoatp/__init__.py
+-rw-r--r--   0        0        0     9232 2023-05-02 13:59:29.967299 nanoatp-0.3.5/nanoatp/bskyagent.py
+-rw-r--r--   0        0        0     3034 2023-04-26 09:39:42.752327 nanoatp-0.3.5/nanoatp/richtext.py
+-rw-r--r--   0        0        0      885 2023-07-29 20:42:05.401625 nanoatp-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     5522 1970-01-01 00:00:00.000000 nanoatp-0.3.5/PKG-INFO
```

### Comparing `nanoatp-0.3.4/LICENSE` & `nanoatp-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoatp-0.3.4/README.md` & `nanoatp-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `nanoatp-0.3.4/nanoatp/bskyagent.py` & `nanoatp-0.3.5/nanoatp/bskyagent.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,14 +176,24 @@
         """https://github.com/bluesky-social/atproto/blob/main/lexicons/com/atproto/identity/resolveHandle.json"""
         params = {"handle": handle}
         response = self.requests.get(
             f"{self.service}/xrpc/com.atproto.identity.resolveHandle", headers=self.headers, params=params
         )
         return response.json()
 
+    def _graph_getBlocks(self, limit: int = 50, cursor: str = "") -> dict[str, Any]:
+        """https://github.com/bluesky-social/atproto/blob/main/lexicons/app/bsky/graph/getBlocks.json"""
+        params: dict[str, str | int] = {}
+        params.update({"limit": limit}) if limit != 50 else None  # 1 <= limit <= 100
+        params.update({"cursor": cursor}) if cursor != "" else None
+        response = self.requests.get(
+            f"{self.service}/xrpc/app.bsky.graph.getBlocks", headers=self.headers, params=params
+        )
+        return response.json()
+
 
 def parseAtUri(uri: str):
     """https://github.com/bluesky-social/atproto/blob/main/packages/uri/src/index.ts"""
     u = urlparse(uri)
     repo = u.netloc
     _, collection, rkey = u.path.split("/")
     return repo, collection, rkey
```

### Comparing `nanoatp-0.3.4/nanoatp/richtext.py` & `nanoatp-0.3.5/nanoatp/richtext.py`

 * *Files identical despite different names*

### Comparing `nanoatp-0.3.4/pyproject.toml` & `nanoatp-0.3.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "nanoatp"
-version = "0.3.4"
+version = "0.3.5"
 description = "A nano implementation of the AT Protocol for Python."
 license = "MIT"
 authors = ["Susumu OTA <1632335+susumuota@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/susumuota/nanoatp"
 repository = "https://github.com/susumuota/nanoatp"
 documentation = "https://github.com/susumuota/nanoatp#readme"
 keywords = ["atprotocol", "atproto", "bluesky"]
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9.16"
-requests = "^2.28.2"
+python = "^3.9"
+requests = "^2.31.0"
 tld = "^0.13"
 
 
 [tool.poetry.group.dev.dependencies]
-flake8 = "^6.0.0"
+flake8 = "^6.1.0"
 isort = "^5.12.0"
-black = "^23.3.0"
-pytest = "^7.3.0"
+black = "^23.7.0"
+pytest = "^7.4.0"
 pytest-watch = "^4.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
```

### Comparing `nanoatp-0.3.4/PKG-INFO` & `nanoatp-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nanoatp
-Version: 0.3.4
+Version: 0.3.5
 Summary: A nano implementation of the AT Protocol for Python.
 Home-page: https://github.com/susumuota/nanoatp
 License: MIT
 Keywords: atprotocol,atproto,bluesky
 Author: Susumu OTA
 Author-email: 1632335+susumuota@users.noreply.github.com
-Requires-Python: >=3.9.16,<4.0.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tld (>=0.13,<0.14)
 Project-URL: Documentation, https://github.com/susumuota/nanoatp#readme
 Project-URL: Repository, https://github.com/susumuota/nanoatp
 Description-Content-Type: text/markdown
 
 # nanoatp
```

