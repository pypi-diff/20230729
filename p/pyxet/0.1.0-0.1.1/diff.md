# Comparing `tmp/pyxet-0.1.0.tar.gz` & `tmp/pyxet-0.1.1.tar.gz`

## Comparing `pyxet-0.1.0.tar` & `pyxet-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 pyxet-0.1.0/Cargo.toml
--rw-r--r--   0        0        0      756 2023-07-28 20:45:38.000000 pyxet-0.1.0/.gitignore
--rw-r--r--   0        0        0     2100 2023-07-28 20:45:38.000000 pyxet-0.1.0/README.md
--rw-r--r--   0        0        0       84 2023-07-28 20:45:38.000000 pyxet-0.1.0/develop.sh
--rw-r--r--   0        0        0      654 2023-07-28 20:45:38.000000 pyxet-0.1.0/docs/Makefile
--rw-r--r--   0        0        0     1185 2023-07-28 20:45:38.000000 pyxet-0.1.0/docs/conf.py
--rw-r--r--   0        0        0    22791 2023-07-28 20:45:38.000000 pyxet-0.1.0/docs/images/logo.png
--rw-r--r--   0        0        0     1761 2023-07-28 20:45:38.000000 pyxet-0.1.0/docs/index.rst
--rw-r--r--   0        0        0      800 2023-07-28 20:45:38.000000 pyxet-0.1.0/docs/make.bat
--rw-r--r--   0        0        0     1088 2023-07-28 20:45:38.000000 pyxet-0.1.0/docs/markdowns/cli.md
--rw-r--r--   0        0        0     2239 2023-07-28 20:45:38.000000 pyxet-0.1.0/docs/markdowns/filesystem.md
--rw-r--r--   0        0        0      760 2023-07-28 20:45:38.000000 pyxet-0.1.0/docs/markdowns/git.md
--rw-r--r--   0        0        0     1399 2023-07-28 20:45:38.000000 pyxet-0.1.0/docs/markdowns/integrations.md
--rw-r--r--   0        0        0     1965 2023-07-28 20:45:38.000000 pyxet-0.1.0/docs/markdowns/mount.md
--rw-r--r--   0        0        0     3040 2023-07-28 20:45:38.000000 pyxet-0.1.0/docs/markdowns/quickstart.md
--rw-r--r--   0        0        0      209 2023-07-28 20:45:38.000000 pyxet-0.1.0/docs/markdowns/use_cases.md
--rw-r--r--   0        0        0       63 2023-07-28 20:45:38.000000 pyxet-0.1.0/docs/modules.rst
--rw-r--r--   0        0        0      231 2023-07-28 20:45:38.000000 pyxet-0.1.0/docs/pyxet.rst
--rw-r--r--   0        0        0     1762 2023-07-28 20:45:38.000000 pyxet-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1278 2023-07-28 20:45:38.000000 pyxet-0.1.0/pyxet/README.md
--rw-r--r--   0        0        0     2889 2023-07-28 20:45:38.000000 pyxet-0.1.0/pyxet/__init__.py
--rw-r--r--   0        0        0    27727 2023-07-28 20:45:38.000000 pyxet-0.1.0/pyxet/cli.py
--rw-r--r--   0        0        0    10521 2023-07-28 20:45:38.000000 pyxet-0.1.0/pyxet/commit_transaction.py
--rw-r--r--   0        0        0     3689 2023-07-28 20:45:38.000000 pyxet-0.1.0/pyxet/file_interface.py
--rw-r--r--   0        0        0    25270 2023-07-28 20:45:38.000000 pyxet-0.1.0/pyxet/file_system.py
--rw-r--r--   0        0        0     6547 2023-07-28 20:45:38.000000 pyxet-0.1.0/pyxet/pathlib.py
--rw-r--r--   0        0        0        0 2023-07-28 20:45:38.000000 pyxet-0.1.0/pyxet/rpyxet/__init__.py
--rw-r--r--   0        0        0     7538 2023-07-28 20:45:38.000000 pyxet-0.1.0/pyxet/url_parsing.py
--rw-r--r--   0        0        0       23 2023-07-28 20:45:38.000000 pyxet-0.1.0/pyxet/version.py
--rw-r--r--   0        0        0    21736 2023-07-28 20:45:38.000000 pyxet-0.1.0/src/lib.rs
--rw-r--r--   0        0        0     1898 2023-07-28 20:45:38.000000 pyxet-0.1.0/tests/arrow_test.py
--rw-r--r--   0        0        0     6906 2023-07-28 20:45:38.000000 pyxet-0.1.0/tests/file_test.py
--rw-r--r--   0        0        0     2333 2023-07-28 20:45:38.000000 pyxet-0.1.0/tests/fsspec_test.py
--rw-r--r--   0        0        0     1218 2023-07-28 20:45:38.000000 pyxet-0.1.0/tests/pandas_test.py
--rw-r--r--   0        0        0     2501 2023-07-28 20:45:38.000000 pyxet-0.1.0/tests/utils.py
--rw-r--r--   0        0        0   108092 2023-07-28 20:47:16.000000 pyxet-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     3650 1970-01-01 00:00:00.000000 pyxet-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 pyxet-0.1.1/Cargo.toml
+-rw-r--r--   0        0        0      756 2023-07-28 20:45:38.000000 pyxet-0.1.1/.gitignore
+-rw-r--r--   0        0        0     2100 2023-07-28 20:45:38.000000 pyxet-0.1.1/README.md
+-rw-r--r--   0        0        0       84 2023-07-28 20:45:38.000000 pyxet-0.1.1/develop.sh
+-rw-r--r--   0        0        0      654 2023-07-28 20:45:38.000000 pyxet-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0     1185 2023-07-28 20:45:38.000000 pyxet-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0    22791 2023-07-28 20:45:38.000000 pyxet-0.1.1/docs/images/logo.png
+-rw-r--r--   0        0        0     1761 2023-07-28 20:45:38.000000 pyxet-0.1.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-07-28 20:45:38.000000 pyxet-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0     1088 2023-07-28 20:45:38.000000 pyxet-0.1.1/docs/markdowns/cli.md
+-rw-r--r--   0        0        0     2239 2023-07-28 20:45:38.000000 pyxet-0.1.1/docs/markdowns/filesystem.md
+-rw-r--r--   0        0        0      760 2023-07-28 20:45:38.000000 pyxet-0.1.1/docs/markdowns/git.md
+-rw-r--r--   0        0        0     1399 2023-07-28 20:45:38.000000 pyxet-0.1.1/docs/markdowns/integrations.md
+-rw-r--r--   0        0        0     1965 2023-07-28 20:45:38.000000 pyxet-0.1.1/docs/markdowns/mount.md
+-rw-r--r--   0        0        0     3040 2023-07-28 20:45:38.000000 pyxet-0.1.1/docs/markdowns/quickstart.md
+-rw-r--r--   0        0        0      209 2023-07-28 20:45:38.000000 pyxet-0.1.1/docs/markdowns/use_cases.md
+-rw-r--r--   0        0        0       63 2023-07-28 20:45:38.000000 pyxet-0.1.1/docs/modules.rst
+-rw-r--r--   0        0        0      231 2023-07-28 20:45:38.000000 pyxet-0.1.1/docs/pyxet.rst
+-rw-r--r--   0        0        0     1762 2023-07-28 22:09:31.000000 pyxet-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1278 2023-07-28 20:45:38.000000 pyxet-0.1.1/pyxet/README.md
+-rw-r--r--   0        0        0     2889 2023-07-28 20:45:38.000000 pyxet-0.1.1/pyxet/__init__.py
+-rw-r--r--   0        0        0    27727 2023-07-28 20:45:38.000000 pyxet-0.1.1/pyxet/cli.py
+-rw-r--r--   0        0        0    10521 2023-07-28 20:45:38.000000 pyxet-0.1.1/pyxet/commit_transaction.py
+-rw-r--r--   0        0        0     3689 2023-07-28 20:45:38.000000 pyxet-0.1.1/pyxet/file_interface.py
+-rw-r--r--   0        0        0    25270 2023-07-28 20:45:38.000000 pyxet-0.1.1/pyxet/file_system.py
+-rw-r--r--   0        0        0     6547 2023-07-28 20:45:38.000000 pyxet-0.1.1/pyxet/pathlib.py
+-rw-r--r--   0        0        0        0 2023-07-28 20:45:38.000000 pyxet-0.1.1/pyxet/rpyxet/__init__.py
+-rw-r--r--   0        0        0     7538 2023-07-28 20:45:38.000000 pyxet-0.1.1/pyxet/url_parsing.py
+-rw-r--r--   0        0        0       23 2023-07-28 22:09:54.000000 pyxet-0.1.1/pyxet/version.py
+-rw-r--r--   0        0        0    21736 2023-07-28 20:45:38.000000 pyxet-0.1.1/src/lib.rs
+-rw-r--r--   0        0        0     1898 2023-07-28 20:45:38.000000 pyxet-0.1.1/tests/arrow_test.py
+-rw-r--r--   0        0        0     6906 2023-07-28 20:45:38.000000 pyxet-0.1.1/tests/file_test.py
+-rw-r--r--   0        0        0     2333 2023-07-28 20:45:38.000000 pyxet-0.1.1/tests/fsspec_test.py
+-rw-r--r--   0        0        0     1218 2023-07-28 20:45:38.000000 pyxet-0.1.1/tests/pandas_test.py
+-rw-r--r--   0        0        0     2501 2023-07-28 20:45:38.000000 pyxet-0.1.1/tests/utils.py
+-rw-r--r--   0        0        0   108092 2023-07-28 22:22:25.000000 pyxet-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     3650 1970-01-01 00:00:00.000000 pyxet-0.1.1/PKG-INFO
```

### Comparing `pyxet-0.1.0/Cargo.toml` & `pyxet-0.1.1/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b70 6163 6b61 6765 5d0d 0a6e 616d 6520  [package]..name 
 00000010: 3d20 2270 7978 6574 220d 0a76 6572 7369  = "pyxet"..versi
-00000020: 6f6e 203d 2022 302e 312e 3022 0d0a 6564  on = "0.1.0"..ed
+00000020: 6f6e 203d 2022 302e 312e 3122 0d0a 6564  on = "0.1.1"..ed
 00000030: 6974 696f 6e20 3d20 2232 3032 3122 0d0a  ition = "2021"..
 00000040: 0d0a 5b6c 6962 5d0d 0a23 2054 6865 206e  ..[lib]..# The n
 00000050: 616d 6520 6f66 2074 6865 206e 6174 6976  ame of the nativ
 00000060: 6520 6c69 6272 6172 792e 2054 6869 7320  e library. This 
 00000070: 6973 2074 6865 206e 616d 6520 7768 6963  is the name whic
 00000080: 6820 7769 6c6c 2062 6520 7573 6564 2069  h will be used i
 00000090: 6e20 5079 7468 6f6e 2074 6f20 696d 706f  n Python to impo
```

### Comparing `pyxet-0.1.0/.gitignore` & `pyxet-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/README.md` & `pyxet-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/docs/Makefile` & `pyxet-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/docs/conf.py` & `pyxet-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/docs/images/logo.png` & `pyxet-0.1.1/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/docs/index.rst` & `pyxet-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/docs/make.bat` & `pyxet-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/docs/markdowns/cli.md` & `pyxet-0.1.1/docs/markdowns/cli.md`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/docs/markdowns/filesystem.md` & `pyxet-0.1.1/docs/markdowns/filesystem.md`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/docs/markdowns/git.md` & `pyxet-0.1.1/docs/markdowns/git.md`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/docs/markdowns/integrations.md` & `pyxet-0.1.1/docs/markdowns/integrations.md`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/docs/markdowns/mount.md` & `pyxet-0.1.1/docs/markdowns/mount.md`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/docs/markdowns/quickstart.md` & `pyxet-0.1.1/docs/markdowns/quickstart.md`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/pyproject.toml` & `pyxet-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14.17,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "pyxet"
-version = "0.1.0"
+version = "0.1.1"
 description = "pyxet is a Python library that provides a lightweight interface for the XetHub platform."
 keywords = [
     "ai",
     "collaboration",
     "data-science",
     "developer-tools",
     "git",
```

### Comparing `pyxet-0.1.0/pyxet/README.md` & `pyxet-0.1.1/pyxet/README.md`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/pyxet/__init__.py` & `pyxet-0.1.1/pyxet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/pyxet/cli.py` & `pyxet-0.1.1/pyxet/cli.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/pyxet/commit_transaction.py` & `pyxet-0.1.1/pyxet/commit_transaction.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/pyxet/file_interface.py` & `pyxet-0.1.1/pyxet/file_interface.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/pyxet/file_system.py` & `pyxet-0.1.1/pyxet/file_system.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/pyxet/pathlib.py` & `pyxet-0.1.1/pyxet/pathlib.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/pyxet/url_parsing.py` & `pyxet-0.1.1/pyxet/url_parsing.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/src/lib.rs` & `pyxet-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/tests/arrow_test.py` & `pyxet-0.1.1/tests/arrow_test.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/tests/file_test.py` & `pyxet-0.1.1/tests/file_test.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/tests/fsspec_test.py` & `pyxet-0.1.1/tests/fsspec_test.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/tests/pandas_test.py` & `pyxet-0.1.1/tests/pandas_test.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/tests/utils.py` & `pyxet-0.1.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.0/Cargo.lock` & `pyxet-0.1.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,15 @@
 dependencies = [
  "byteorder",
 ]
 
 [[package]]
 name = "cache"
 version = "0.11.1"
-source = "git+https://github.com/xetdata/xet-core#5dbdc2cfb28e126681b48a4321da79815163ab98"
+source = "git+https://github.com/xetdata/xet-core#1ecd7570ea63ccbf6aba3d4876a4d822884bfbe0"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.13.1",
  "byteorder",
  "chrono",
  "lazy_static",
@@ -270,15 +270,15 @@
  "tracing-test",
  "utils",
 ]
 
 [[package]]
 name = "cas_client"
 version = "0.11.1"
-source = "git+https://github.com/xetdata/xet-core#5dbdc2cfb28e126681b48a4321da79815163ab98"
+source = "git+https://github.com/xetdata/xet-core#1ecd7570ea63ccbf6aba3d4876a4d822884bfbe0"
 dependencies = [
  "anyhow",
  "async-trait",
  "bincode",
  "bytes",
  "cache",
  "clap 2.34.0",
@@ -693,15 +693,15 @@
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "data_analysis"
 version = "0.11.1"
-source = "git+https://github.com/xetdata/xet-core#5dbdc2cfb28e126681b48a4321da79815163ab98"
+source = "git+https://github.com/xetdata/xet-core#1ecd7570ea63ccbf6aba3d4876a4d822884bfbe0"
 dependencies = [
  "approx",
  "cxx",
  "cxx-build",
  "float-cmp",
  "serde",
  "truncrate",
@@ -1095,15 +1095,15 @@
  "openssl-sys",
  "url",
 ]
 
 [[package]]
 name = "gitxetcore"
 version = "0.11.1"
-source = "git+https://github.com/xetdata/xet-core#5dbdc2cfb28e126681b48a4321da79815163ab98"
+source = "git+https://github.com/xetdata/xet-core#1ecd7570ea63ccbf6aba3d4876a4d822884bfbe0"
 dependencies = [
  "anyhow",
  "async-trait",
  "atoi",
  "atty",
  "base64 0.13.1",
  "bincode",
@@ -1545,15 +1545,15 @@
  "openssl-sys",
  "pkg-config",
 ]
 
 [[package]]
 name = "libmagic"
 version = "0.11.1"
-source = "git+https://github.com/xetdata/xet-core#5dbdc2cfb28e126681b48a4321da79815163ab98"
+source = "git+https://github.com/xetdata/xet-core#1ecd7570ea63ccbf6aba3d4876a4d822884bfbe0"
 dependencies = [
  "anyhow",
  "phf",
  "serde",
  "serde_json",
  "tracing",
  "tracing-attributes",
@@ -1654,15 +1654,15 @@
  "digest 0.9.0",
  "opaque-debug",
 ]
 
 [[package]]
 name = "mdb_shard"
 version = "0.11.1"
-source = "git+https://github.com/xetdata/xet-core#5dbdc2cfb28e126681b48a4321da79815163ab98"
+source = "git+https://github.com/xetdata/xet-core#1ecd7570ea63ccbf6aba3d4876a4d822884bfbe0"
 dependencies = [
  "anyhow",
  "async-scoped",
  "async-trait",
  "binary-heap-plus",
  "clap 3.2.23",
  "lazy_static",
@@ -1694,15 +1694,15 @@
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "merkledb"
 version = "0.11.1"
-source = "git+https://github.com/xetdata/xet-core#5dbdc2cfb28e126681b48a4321da79815163ab98"
+source = "git+https://github.com/xetdata/xet-core#1ecd7570ea63ccbf6aba3d4876a4d822884bfbe0"
 dependencies = [
  "async-trait",
  "bincode",
  "bitflags",
  "blake3",
  "clap 3.2.23",
  "futures",
@@ -1724,15 +1724,15 @@
  "tracing",
  "walkdir",
 ]
 
 [[package]]
 name = "merklehash"
 version = "0.11.1"
-source = "git+https://github.com/xetdata/xet-core#5dbdc2cfb28e126681b48a4321da79815163ab98"
+source = "git+https://github.com/xetdata/xet-core#1ecd7570ea63ccbf6aba3d4876a4d822884bfbe0"
 dependencies = [
  "blake3",
  "generic-array",
  "rand 0.8.5",
  "rand_chacha",
  "rand_core 0.6.4",
  "safe-transmute",
@@ -2168,15 +2168,15 @@
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "parutils"
 version = "0.11.1"
-source = "git+https://github.com/xetdata/xet-core#5dbdc2cfb28e126681b48a4321da79815163ab98"
+source = "git+https://github.com/xetdata/xet-core#1ecd7570ea63ccbf6aba3d4876a4d822884bfbe0"
 dependencies = [
  "anyhow",
  "async-scoped",
  "futures",
  "tokio",
 ]
 
@@ -2336,15 +2336,15 @@
 version = "0.3.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
 
 [[package]]
 name = "pointer_file"
 version = "0.11.1"
-source = "git+https://github.com/xetdata/xet-core#5dbdc2cfb28e126681b48a4321da79815163ab98"
+source = "git+https://github.com/xetdata/xet-core#1ecd7570ea63ccbf6aba3d4876a4d822884bfbe0"
 dependencies = [
  "toml",
  "tracing",
 ]
 
 [[package]]
 name = "ppv-lite86"
@@ -2420,15 +2420,15 @@
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "progress_reporting"
 version = "0.11.1"
-source = "git+https://github.com/xetdata/xet-core#5dbdc2cfb28e126681b48a4321da79815163ab98"
+source = "git+https://github.com/xetdata/xet-core#1ecd7570ea63ccbf6aba3d4876a4d822884bfbe0"
 dependencies = [
  "atty",
  "crossterm",
  "more-asserts 0.2.2",
  "tokio",
  "tracing",
  "utils",
@@ -2448,15 +2448,15 @@
  "protobuf",
  "thiserror",
 ]
 
 [[package]]
 name = "prometheus_dict_encoder"
 version = "0.11.1"
-source = "git+https://github.com/xetdata/xet-core#5dbdc2cfb28e126681b48a4321da79815163ab98"
+source = "git+https://github.com/xetdata/xet-core#1ecd7570ea63ccbf6aba3d4876a4d822884bfbe0"
 dependencies = [
  "memchr",
  "prometheus",
  "tracing",
 ]
 
 [[package]]
@@ -2611,15 +2611,15 @@
 checksum = "212d74540270e3a22eed5f0d4bbc0765dff20958d694e9d4f5ebe6e22778c422"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pyxet"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "anyhow",
  "cc",
  "futures",
  "gitxetcore",
  "libc",
  "pyo3",
@@ -2828,15 +2828,15 @@
 version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4389f1d5789befaf6029ebd9f7dac4af7f7e3d61b69d4f30e2ac02b57e7712b0"
 
 [[package]]
 name = "retry_strategy"
 version = "0.11.1"
-source = "git+https://github.com/xetdata/xet-core#5dbdc2cfb28e126681b48a4321da79815163ab98"
+source = "git+https://github.com/xetdata/xet-core#1ecd7570ea63ccbf6aba3d4876a4d822884bfbe0"
 dependencies = [
  "tokio-retry",
 ]
 
 [[package]]
 name = "ring"
 version = "0.16.20"
@@ -3025,15 +3025,15 @@
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "s3"
 version = "0.11.1"
-source = "git+https://github.com/xetdata/xet-core#5dbdc2cfb28e126681b48a4321da79815163ab98"
+source = "git+https://github.com/xetdata/xet-core#1ecd7570ea63ccbf6aba3d4876a4d822884bfbe0"
 dependencies = [
  "chrono",
  "more-asserts 0.3.1",
  "parutils",
  "pbr",
  "rusoto_core",
  "rusoto_s3",
@@ -3219,15 +3219,15 @@
  "keccak",
  "opaque-debug",
 ]
 
 [[package]]
 name = "shard_client"
 version = "0.11.1"
-source = "git+https://github.com/xetdata/xet-core#5dbdc2cfb28e126681b48a4321da79815163ab98"
+source = "git+https://github.com/xetdata/xet-core#1ecd7570ea63ccbf6aba3d4876a4d822884bfbe0"
 dependencies = [
  "anyhow",
  "async-trait",
  "bincode",
  "bytes",
  "cas_client",
  "clap 2.34.0",
@@ -4078,15 +4078,15 @@
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
 name = "utils"
 version = "0.11.1"
-source = "git+https://github.com/xetdata/xet-core#5dbdc2cfb28e126681b48a4321da79815163ab98"
+source = "git+https://github.com/xetdata/xet-core#1ecd7570ea63ccbf6aba3d4876a4d822884bfbe0"
 dependencies = [
  "anyhow",
  "chrono",
  "futures",
  "hashbrown",
  "hashring",
  "lazy_static",
@@ -4402,28 +4402,28 @@
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "xet_config"
 version = "0.11.1"
-source = "git+https://github.com/xetdata/xet-core#5dbdc2cfb28e126681b48a4321da79815163ab98"
+source = "git+https://github.com/xetdata/xet-core#1ecd7570ea63ccbf6aba3d4876a4d822884bfbe0"
 dependencies = [
  "config",
  "dirs",
  "serde",
  "thiserror",
  "toml",
  "tracing",
 ]
 
 [[package]]
 name = "xetblob"
 version = "0.11.1"
-source = "git+https://github.com/xetdata/xet-core#5dbdc2cfb28e126681b48a4321da79815163ab98"
+source = "git+https://github.com/xetdata/xet-core#1ecd7570ea63ccbf6aba3d4876a4d822884bfbe0"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.13.1",
  "blake3",
  "clap 3.2.23",
  "dirs",
```

### Comparing `pyxet-0.1.0/PKG-INFO` & `pyxet-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxet
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

