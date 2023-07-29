# Comparing `tmp/wingechr-datatools-0.1.0.tar.gz` & `tmp/wingechr-datatools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wingechr-datatools-0.1.0.tar", last modified: Mon Jul 24 14:07:07 2023, max compression
+gzip compressed data, was "wingechr-datatools-0.2.0.tar", last modified: Sat Jul 29 11:54:51 2023, max compression
```

## Comparing `wingechr-datatools-0.1.0.tar` & `wingechr-datatools-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 14:07:07.582560 wingechr-datatools-0.1.0/
--rw-rw-rw-   0        0        0      115 2023-07-24 14:05:47.000000 wingechr-datatools-0.1.0/.bumpversion.cfg
-drwxrwxrwx   0        0        0        0 2023-07-24 14:07:07.506430 wingechr-datatools-0.1.0/.github/
-drwxrwxrwx   0        0        0        0 2023-07-24 14:07:07.536665 wingechr-datatools-0.1.0/.github/workflows/
--rw-rw-rw-   0        0        0      898 2023-07-24 13:10:24.000000 wingechr-datatools-0.1.0/.github/workflows/test.yml
--rw-rw-rw-   0        0        0      100 2023-07-24 13:47:55.000000 wingechr-datatools-0.1.0/.gitignore
--rw-rw-rw-   0        0        0     1215 2023-07-24 13:10:24.000000 wingechr-datatools-0.1.0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      489 2023-07-24 14:07:07.582057 wingechr-datatools-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-07-24 13:10:24.000000 wingechr-datatools-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 14:07:07.550879 wingechr-datatools-0.1.0/datatools/
--rw-rw-rw-   0        0        0      144 2023-07-24 14:05:47.000000 wingechr-datatools-0.1.0/datatools/__init__.py
--rw-rw-rw-   0        0        0     5826 2023-07-24 14:05:47.000000 wingechr-datatools-0.1.0/datatools/__main__.py
--rw-rw-rw-   0        0        0      275 2023-07-24 14:05:47.000000 wingechr-datatools-0.1.0/datatools/exceptions.py
--rw-rw-rw-   0        0        0    17897 2023-07-24 14:05:47.000000 wingechr-datatools-0.1.0/datatools/storage.py
--rw-rw-rw-   0        0        0     5495 2023-07-24 14:05:47.000000 wingechr-datatools-0.1.0/datatools/utils.py
--rw-rw-rw-   0        0        0      136 2023-07-24 13:10:24.000000 wingechr-datatools-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 14:07:07.582560 wingechr-datatools-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1106 2023-07-24 14:07:03.000000 wingechr-datatools-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 14:07:07.559798 wingechr-datatools-0.1.0/tests/
--rw-rw-rw-   0        0        0      168 2023-07-24 13:10:24.000000 wingechr-datatools-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     3610 2023-07-24 14:05:47.000000 wingechr-datatools-0.1.0/tests/test_01_utils.py
--rw-rw-rw-   0        0        0     6153 2023-07-24 14:05:47.000000 wingechr-datatools-0.1.0/tests/test_02_storage.py
--rw-rw-rw-   0        0        0      106 2023-07-24 13:47:55.000000 wingechr-datatools-0.1.0/tox.ini
-drwxrwxrwx   0        0        0        0 2023-07-24 14:07:07.578928 wingechr-datatools-0.1.0/wingechr_datatools.egg-info/
--rw-rw-rw-   0        0        0      489 2023-07-24 14:07:07.000000 wingechr-datatools-0.1.0/wingechr_datatools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-07-24 14:07:07.000000 wingechr-datatools-0.1.0/wingechr_datatools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 14:07:07.000000 wingechr-datatools-0.1.0/wingechr_datatools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-24 14:07:07.000000 wingechr-datatools-0.1.0/wingechr_datatools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       70 2023-07-24 14:07:07.000000 wingechr-datatools-0.1.0/wingechr_datatools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-24 14:07:07.000000 wingechr-datatools-0.1.0/wingechr_datatools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 11:54:51.883850 wingechr-datatools-0.2.0/
+-rw-rw-rw-   0        0        0      115 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/.bumpversion.cfg
+drwxrwxrwx   0        0        0        0 2023-07-29 11:54:51.680285 wingechr-datatools-0.2.0/.github/
+drwxrwxrwx   0        0        0        0 2023-07-29 11:54:51.742725 wingechr-datatools-0.2.0/.github/workflows/
+-rw-rw-rw-   0        0        0      898 2023-07-24 13:10:24.000000 wingechr-datatools-0.2.0/.github/workflows/test.yml
+-rw-rw-rw-   0        0        0      116 2023-07-26 15:28:45.000000 wingechr-datatools-0.2.0/.gitignore
+-rw-rw-rw-   0        0        0     1215 2023-07-24 13:10:24.000000 wingechr-datatools-0.2.0/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0      489 2023-07-29 11:54:51.882869 wingechr-datatools-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 11:54:51.852726 wingechr-datatools-0.2.0/datatools/
+-rw-rw-rw-   0        0        0      220 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/datatools/__init__.py
+-rw-rw-rw-   0        0        0     3510 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/datatools/__main__.py
+-rw-rw-rw-   0        0        0     2292 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/datatools/cache.py
+-rw-rw-rw-   0        0        0      680 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/datatools/exceptions.py
+-rw-rw-rw-   0        0        0     3823 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/datatools/load.py
+-rw-rw-rw-   0        0        0    10530 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/datatools/storage.py
+-rw-rw-rw-   0        0        0    10349 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/datatools/utils.py
+-rw-rw-rw-   0        0        0      136 2023-07-24 13:10:24.000000 wingechr-datatools-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 11:54:51.883850 wingechr-datatools-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 11:54:51.865496 wingechr-datatools-0.2.0/tests/
+-rw-rw-rw-   0        0        0      289 2023-07-27 09:42:54.000000 wingechr-datatools-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     5006 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/tests/test_01_utils.py
+-rw-rw-rw-   0        0        0     6435 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/tests/test_02_storage.py
+-rw-rw-rw-   0        0        0      862 2023-07-26 15:28:45.000000 wingechr-datatools-0.2.0/tests/test_04_cache.py
+-rw-rw-rw-   0        0        0      921 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/tests/test_05_sql.py
+-rw-rw-rw-   0        0        0      117 2023-07-29 11:54:21.000000 wingechr-datatools-0.2.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-07-29 11:54:51.880850 wingechr-datatools-0.2.0/wingechr_datatools.egg-info/
+-rw-rw-rw-   0        0        0      489 2023-07-29 11:54:51.000000 wingechr-datatools-0.2.0/wingechr_datatools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-07-29 11:54:51.000000 wingechr-datatools-0.2.0/wingechr_datatools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 11:54:51.000000 wingechr-datatools-0.2.0/wingechr_datatools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-29 11:54:51.000000 wingechr-datatools-0.2.0/wingechr_datatools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      109 2023-07-29 11:54:51.000000 wingechr-datatools-0.2.0/wingechr_datatools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-29 11:54:51.000000 wingechr-datatools-0.2.0/wingechr_datatools.egg-info/top_level.txt
```

### Comparing `wingechr-datatools-0.1.0/.github/workflows/test.yml` & `wingechr-datatools-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `wingechr-datatools-0.1.0/.pre-commit-config.yaml` & `wingechr-datatools-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `wingechr-datatools-0.1.0/setup.py` & `wingechr-datatools-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,20 +8,24 @@
             "appdirs",
             "click",
             "coloredlogs",
             "jsonpath-ng>=1.5",
             "requests",
             "tzlocal",
             "unidecode",
+            "sqlalchemy>=2.0",
+            "sqlparse",
+            "pyodbc",
+            "pandas",
         ],
         name="wingechr-datatools",
         description=None,
         long_description=None,
         long_description_content_type="text/markdown",
-        version="0.1.0",
+        version="0.2.0",
         author="Christian Winger",
         author_email="c@wingechr.de",
         url="https://github.com/wingechr/datatools",
         platforms=["any"],
         license="Public Domain",
         project_urls={"Bug Tracker": "https://github.com/wingechr/datatools"},
         classifiers=[
```

### Comparing `wingechr-datatools-0.1.0/tests/test_02_storage.py` & `wingechr-datatools-0.2.0/tests/test_02_storage.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,183 +1,183 @@
-# coding: utf-8
 import logging
 import os
 import subprocess as sp
 import sys
+
+# import secrets
 import unittest
-from pathlib import Path
 from tempfile import TemporaryDirectory
-from threading import Thread
+from urllib.parse import urlsplit
 
+from datatools.cache import DEFAULT_FROM_BYTES
 from datatools.exceptions import DataDoesNotExists, DataExists, InvalidPath
-from datatools.storage import (
-    HASHED_DATA_PATH_PREFIX,
-    LocalStorage,
-    RemoteStorage,
-    StorageServer,
-    TestCliStorage,
-)
-from datatools.utils import (
+from datatools.storage import HASHED_DATA_PATH_PREFIX, Storage
+from datatools.utils import (  # exit_stack,
+    DEFAULT_BUFFER_SIZE,
+    as_uri,
     get_free_port,
     make_file_writable,
     normalize_path,
-    path_to_file_uri,
     wait_for_server,
 )
 
 from . import objects_euqal
 
-logging.basicConfig(
-    format="[%(asctime)s %(levelname)7s] %(message)s", level=logging.DEBUG
-)
 
+class MyTemporaryDirectory(TemporaryDirectory):
+    def __init__(self, *args, **kwargs):
+        self.tempdir = TemporaryDirectory(*args, **kwargs)
 
-class Test_01_LocalStorage(unittest.TestCase):
-    def setUp(self) -> None:
-        self.tempdir = TemporaryDirectory()
-        self.tempdir_path = self.tempdir.__enter__()
-        self.storage = LocalStorage(location=self.tempdir_path)
+    def __enter__(self):
+        return self.tempdir.__enter__()
 
-    def tearDown(self) -> None:
+    def __exit__(self, *args):
         # make files writable so cleanup can delete them
-        for rt, _ds, fs in os.walk(self.tempdir_path):
+        path = self.tempdir.name
+        for rt, _ds, fs in os.walk(path):
             for f in fs:
                 filepath = f"{rt}/{f}"
                 make_file_writable(filepath)
-        self.tempdir.__exit__(None, None, None)
+        # delete dir
+        self.tempdir.__exit__(*args)
+        logging.debug(f"DELETING {path}: {not os.path.exists(path)}")
+
+
+class TestBase(unittest.TestCase):
+    def setUp(self) -> None:
+        self.tempdir1 = MyTemporaryDirectory()
+        path_tempdir1 = self.tempdir1.__enter__()  # exit_stack.enter_context()
+        self.storage = Storage(location=path_tempdir1)
+
+        # set up static file server
+        self.tempdir2 = MyTemporaryDirectory()
+        self.static_dir = self.tempdir2.__enter__()  # exit_stack.enter_context()
+        port = get_free_port()
+        self.static_url = f"http://localhost:{port}"
+        self.http_proc = sp.Popen(
+            [
+                sys.executable,
+                "-m",
+                "http.server",
+                str(port),
+                "--directory",
+                self.static_dir,
+            ]
+        )
+        wait_for_server(self.static_url)
 
+    def tearDown(self) -> None:
+        self.http_proc.terminate()  # or kill
+        self.http_proc.wait()
+
+        self.tempdir1.__exit__(None, None, None)
+        self.tempdir2.__exit__(None, None, None)
+
+
+class Test_01_LocalStorage(TestBase):
     def test_storage(self):
         # create local instance in temporary dir
-        data = b"hello world"
+
+        # create large random data
+        # data = secrets.token_bytes(int(DEFAULT_BUFFER_SIZE * 1.5))
+        data = b"x" * int(DEFAULT_BUFFER_SIZE * 1.5)
+
         data_path_user = "/My/path"
         invalid_path = HASHED_DATA_PATH_PREFIX + "my/path"
 
-        # cannot save save data to hash subdir
+        logging.debug("Step 1: cannot save save data to hash subdir")
         self.assertRaises(
             InvalidPath,
             self.storage.data_put,
             data=data,
             data_path=invalid_path,
         )
-        # save data without path
+
+        logging.debug("Step 2a: save data without path")
         data_path = self.storage.data_put(data=data)
         self.assertTrue(data_path.startswith(HASHED_DATA_PATH_PREFIX))
 
-        # save data
+        # load this again
+        with self.storage.data_open(data_path) as file:
+            _data = file.read()
+        self.assertEqual(_data, data)
+
+        logging.debug("Step 2c: save with invalid path")
+        self.assertRaises(
+            InvalidPath,
+            self.storage.data_put,
+            data=data,
+            data_path="/my/data/file.metadata.json",  # .metadata. is not allowed
+        )
+
+        logging.debug("Step 2b: save data with path")
+        self.assertFalse(self.storage.data_exists(data_path_user))
         data_path = self.storage.data_put(data=data, data_path=data_path_user)
+        self.assertTrue(self.storage.data_exists(data_path_user))
         self.assertEqual(normalize_path(data_path_user), data_path)
-        # save again will fail
+
+        logging.debug("Step 2c: save again will fail")
         self.assertRaises(
             DataExists,
             self.storage.data_put,
             data=data,
             data_path=data_path_user,
         )
-        # read it
-        res = self.storage.data_get(data_path=data_path_user)
-        self.assertEqual(data, res)
-        # delete it ...
+
+        logging.debug("Step 3: read data")
+        with self.storage.data_open(data_path=data_path_user) as file:
+            _data = file.read()
+        self.assertEqual(data, _data)
+
+        logging.debug("Step 4a: delete")
         self.storage.data_delete(data_path=data_path_user)
-        # ... and deleting again does NOT raise an error ...
+
+        logging.debug("Step 4b: delete again")
         self.storage.data_delete(data_path=data_path_user)
         # reading now will raise error
         self.assertRaises(
-            DataDoesNotExists, self.storage.data_get, data_path=data_path_user
+            DataDoesNotExists, self.storage.data_open, data_path=data_path_user
         )
-        # ... and now we can save it again
+
+        logging.debug("Step 5: save again")
         self.storage.data_put(data=data, data_path=data_path_user)
 
-        # metadata can be saved independent of data
+        logging.debug("Step 5: save metadata")
         metadata = {"a": [1, 2, 3], "b.c[0]": "test"}
         self.storage.metadata_put(data_path=data_path_user, metadata=metadata)
 
-        # partial update
+        logging.debug("Step 5: update metadata")
         metadata = {"b.c[1]": "test2"}
         self.storage.metadata_put(data_path=data_path_user, metadata=metadata)
 
-        # get partial
+        logging.debug("Step 5: get metadata")
         metadata2 = self.storage.metadata_get(
             data_path=data_path_user, metadata_path="b.c"
         )
         self.assertTrue(objects_euqal(metadata2, ["test", "test2"]))
 
-
-class Test_02_RemoteStorage(Test_01_LocalStorage):
-    def setUp(self) -> None:
-        super().setUp()
-
-        port = get_free_port()
-        remote_location = f"http://localhost:{port}"
-        server = StorageServer(storage=self.storage, port=port)
-        Thread(target=server.serve_forever, daemon=True).start()
-        wait_for_server(remote_location)
-
-        self.storage = RemoteStorage(location=remote_location)
-
-
-class Test_03_TestCliStorage(Test_01_LocalStorage):
-    def setUp(self) -> None:
-        super().setUp()
-
-        # use self.storage from super() to get temp dir location
-        server_storage = TestCliStorage(location=self.tempdir_path)
-        port = get_free_port()
-        remote_location = f"http://localhost:{port}"
-
-        self.server_proc = server_storage.serve(port=port)
-        wait_for_server(remote_location)
-
-        # test static server process (to serve test files)
-        self.static_port = get_free_port()
-        self.http_proc = sp.Popen(
-            [
-                sys.executable,
-                "-m",
-                "http.server",
-                str(self.static_port),
-                "--directory",
-                self.tempdir_path,
-            ]
-        )
-        wait_for_server(f"http://localhost:{self.static_port}")
-
-        # create client
-        self.storage = TestCliStorage(location=remote_location)
-
-    def tearDown(self) -> None:
-        # shutdown server
-        self.server_proc.terminate()  # or kill
-        self.server_proc.wait()
-
-        self.http_proc.terminate()  # or kill
-        self.http_proc.wait()
-
-        super().tearDown()
-
-    def test_cli_read_uri(self):
-        # create file
-        filename = "test.txt"
-        filepath = self.tempdir_path + "/" + filename
-        data = b"hello world"
-        with open(filepath, "wb") as file:
-            file.write(data)
-
-        # read file://
-        expected_path = normalize_path(path_to_file_uri(Path(filepath).absolute()))
-        data_path = self.storage.data_put(data=filepath)
-        self.assertEqual(expected_path, data_path)
-
-        # read http://
-        url = f"http://user:passwd@localhost:{self.static_port}/{filename}#.anchor"
-        expected_path = "http/localhost/test.txt.anchor"
-        data_path = self.storage.data_put(data=url)
-        self.assertEqual(expected_path, data_path)
-
-        # this should auto save the source
-        source = self.storage.metadata_get(
-            data_path=data_path, metadata_path="source.path"
-        )
-        # url without credentials
-        exp_source = f"http://localhost:{self.static_port}/{filename}#.anchor"
-        self.assertEqual(source, exp_source)
-
-        print(self.storage.metadata_get(data_path=data_path))
+    def test_storage_autoload(self):
+        uri = "sqlite:///:memory:?q=select 1 as value#/query1"
+        self.assertRaises(DataDoesNotExists, self.storage.data_open, data_path=uri)
+
+        with self.storage.data_open(data_path=uri, auto_load_uri=True) as file:
+            data = file.read()
+        data = DEFAULT_FROM_BYTES(data)
+        self.assertEqual(data[0]["value"], 1)
+
+        # save test file
+        db_filepath = self.static_dir + "/test.db"
+        with open(db_filepath, "wb") as file:
+            pass
+
+        # platform independent: no baskslash, abspath, always starts with /
+        db_path = urlsplit(as_uri(db_filepath)).path
+        uri = f"sqlite://{db_path}?q=select 1 as value#/query1"
+        with self.storage.data_open(data_path=uri, auto_load_uri=True) as file:
+            data = file.read()
+        data = DEFAULT_FROM_BYTES(data)
+        self.assertEqual(data[0]["value"], 1)
+
+        uri = f"{self.static_url}/test.db"
+        with self.storage.data_open(data_path=uri, auto_load_uri=True) as file:
+            data = file.read()
+        self.assertEqual(data, b"")
```

### Comparing `wingechr-datatools-0.1.0/wingechr_datatools.egg-info/SOURCES.txt` & `wingechr-datatools-0.2.0/wingechr_datatools.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,19 +4,23 @@
 README.md
 requirements.txt
 setup.py
 tox.ini
 .github/workflows/test.yml
 datatools/__init__.py
 datatools/__main__.py
+datatools/cache.py
 datatools/exceptions.py
+datatools/load.py
 datatools/storage.py
 datatools/utils.py
 tests/__init__.py
 tests/test_01_utils.py
 tests/test_02_storage.py
+tests/test_04_cache.py
+tests/test_05_sql.py
 wingechr_datatools.egg-info/PKG-INFO
 wingechr_datatools.egg-info/SOURCES.txt
 wingechr_datatools.egg-info/dependency_links.txt
 wingechr_datatools.egg-info/entry_points.txt
 wingechr_datatools.egg-info/requires.txt
 wingechr_datatools.egg-info/top_level.txt
```

