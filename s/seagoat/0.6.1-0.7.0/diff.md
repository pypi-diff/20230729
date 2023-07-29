# Comparing `tmp/seagoat-0.6.1.tar.gz` & `tmp/seagoat-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seagoat-0.6.1.tar", max compression
+gzip compressed data, was "seagoat-0.7.0.tar", max compression
```

## Comparing `seagoat-0.6.1.tar` & `seagoat-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2023-07-28 15:07:44.886891 seagoat-0.6.1/LICENSE
--rw-r--r--   0        0        0     1847 2023-07-28 15:07:44.886891 seagoat-0.6.1/README.md
--rw-r--r--   0        0        0     3083 2023-07-28 15:07:45.666892 seagoat-0.6.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-28 15:07:44.894891 seagoat-0.6.1/seagoat/__init__.py
--rw-r--r--   0        0        0     1601 2023-07-28 15:07:44.894891 seagoat-0.6.1/seagoat/cache.py
--rw-r--r--   0        0        0     2955 2023-07-28 15:07:44.894891 seagoat-0.6.1/seagoat/cli.py
--rw-r--r--   0        0        0      196 2023-07-28 15:07:44.894891 seagoat-0.6.1/seagoat/common.py
--rw-r--r--   0        0        0     4512 2023-07-28 15:07:44.894891 seagoat-0.6.1/seagoat/engine.py
--rw-r--r--   0        0        0     3492 2023-07-28 15:07:44.894891 seagoat-0.6.1/seagoat/file.py
--rw-r--r--   0        0        0     2689 2023-07-28 15:07:44.894891 seagoat-0.6.1/seagoat/repository.py
--rw-r--r--   0        0        0     2021 2023-07-28 15:07:44.894891 seagoat-0.6.1/seagoat/result.py
--rw-r--r--   0        0        0     5624 2023-07-28 15:07:44.894891 seagoat-0.6.1/seagoat/server.py
--rw-r--r--   0        0        0     1878 2023-07-28 15:07:44.894891 seagoat-0.6.1/seagoat/sources/chroma.py
--rw-r--r--   0        0        0     1210 2023-07-28 15:07:44.894891 seagoat-0.6.1/seagoat/sources/ripgrep.py
--rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 seagoat-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-29 21:26:17.188030 seagoat-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1847 2023-07-29 21:26:17.188030 seagoat-0.7.0/README.md
+-rw-r--r--   0        0        0     3084 2023-07-29 21:26:17.964038 seagoat-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-29 21:26:17.192030 seagoat-0.7.0/seagoat/__init__.py
+-rw-r--r--   0        0        0     1601 2023-07-29 21:26:17.192030 seagoat-0.7.0/seagoat/cache.py
+-rw-r--r--   0        0        0     3103 2023-07-29 21:26:17.192030 seagoat-0.7.0/seagoat/cli.py
+-rw-r--r--   0        0        0      196 2023-07-29 21:26:17.192030 seagoat-0.7.0/seagoat/common.py
+-rw-r--r--   0        0        0     4512 2023-07-29 21:26:17.192030 seagoat-0.7.0/seagoat/engine.py
+-rw-r--r--   0        0        0     3492 2023-07-29 21:26:17.192030 seagoat-0.7.0/seagoat/file.py
+-rw-r--r--   0        0        0     2689 2023-07-29 21:26:17.192030 seagoat-0.7.0/seagoat/repository.py
+-rw-r--r--   0        0        0     2021 2023-07-29 21:26:17.192030 seagoat-0.7.0/seagoat/result.py
+-rw-r--r--   0        0        0     5766 2023-07-29 21:26:17.192030 seagoat-0.7.0/seagoat/server.py
+-rw-r--r--   0        0        0     1878 2023-07-29 21:26:17.196030 seagoat-0.7.0/seagoat/sources/chroma.py
+-rw-r--r--   0        0        0     1210 2023-07-29 21:26:17.196030 seagoat-0.7.0/seagoat/sources/ripgrep.py
+-rw-r--r--   0        0        0     2862 1970-01-01 00:00:00.000000 seagoat-0.7.0/PKG-INFO
```

### Comparing `seagoat-0.6.1/LICENSE` & `seagoat-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seagoat-0.6.1/README.md` & `seagoat-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `seagoat-0.6.1/pyproject.toml` & `seagoat-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "seagoat"
-version = "0.6.1"
+version = "0.7.0"
 description = "A semantic-code search engine"
 authors = ["Daniel Kantor <git@daniel-kantor.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.scripts]
 gt = "seagoat.cli:seagoat"
 seagoat = "seagoat.cli:seagoat"
 seagoat-server = "seagoat.server:server"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-chromadb = "^0.4.0"
+chromadb = "^0.3.26"
 gitpython = "^3.1.31"
 tqdm = "^4.65.0"
 appdirs = "^1.4.4"
 click = "^8.1.3"
 prompt-toolkit = "^3.0.38"
 blessed = "^1.20.0"
 pygments = "^2.15.1"
```

### Comparing `seagoat-0.6.1/seagoat/cache.py` & `seagoat-0.7.0/seagoat/cache.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.6.1/seagoat/cli.py` & `seagoat-0.7.0/seagoat/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,14 +74,17 @@
     Query your codebase for your QUERY in the Git repository REPO_PATH.
 
     Your query can either be text that you expect to find in a file,
     or a description of what you are looking for.
 
     When REPO_PATH is not specified, the current working directory is
     assumed to be the repository path.
+
+    In order to use seagoat in your repository, you need to run a server
+    that will analyze your codebase. Check seagoat-server --help for more
     """
     _, __, ___, server_address = load_server_info(get_server_info_file(repo_path))
     results = query_server(query, server_address)
 
     color_enabled = os.isatty(0) and not no_color
     for result in results:
         for result_line in result.get("lines", []):
```

### Comparing `seagoat-0.6.1/seagoat/engine.py` & `seagoat-0.7.0/seagoat/engine.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.6.1/seagoat/file.py` & `seagoat-0.7.0/seagoat/file.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.6.1/seagoat/repository.py` & `seagoat-0.7.0/seagoat/repository.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.6.1/seagoat/result.py` & `seagoat-0.7.0/seagoat/result.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.6.1/seagoat/server.py` & `seagoat-0.7.0/seagoat/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,19 @@
     host, port, _, server_address = load_server_info(server_info_file)
     click.echo(f"Server started at {server_address}")
     return server_address
 
 
 @click.group()
 def server():
-    pass
+    """
+    This server analyzes your codebase and creates vector embeddings for it.
+
+    You can query this server using the seagoat command.
+    """
 
 
 @server.command()
 @click.argument("repo_path")
 def start(repo_path):
     """Starts the server."""
     get_server(repo_path)
```

### Comparing `seagoat-0.6.1/seagoat/sources/chroma.py` & `seagoat-0.7.0/seagoat/sources/chroma.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.6.1/seagoat/sources/ripgrep.py` & `seagoat-0.7.0/seagoat/sources/ripgrep.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.6.1/PKG-INFO` & `seagoat-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: seagoat
-Version: 0.6.1
+Version: 0.7.0
 Summary: A semantic-code search engine
 License: MIT
 Author: Daniel Kantor
 Author-email: git@daniel-kantor.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: blessed (>=1.20.0,<2.0.0)
-Requires-Dist: chromadb (>=0.4.0,<0.5.0)
+Requires-Dist: chromadb (>=0.3.26,<0.4.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: flask (>=2.3.2,<3.0.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0)
```

