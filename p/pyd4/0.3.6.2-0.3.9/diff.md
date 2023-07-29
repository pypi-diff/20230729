# Comparing `tmp/pyd4-0.3.6.2.tar.gz` & `tmp/pyd4-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyd4-0.3.6.2.tar", last modified: Thu Jun 30 23:55:03 2022, max compression
+gzip compressed data, was "pyd4-0.3.9.tar", last modified: Sat Jul 29 15:05:16 2023, max compression
```

## Comparing `pyd4-0.3.6.2.tar` & `pyd4-0.3.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 haohou    (1001) haohou    (1000)        0 2022-06-30 23:55:03.902609 pyd4-0.3.6.2/
--rw-rw-r--   0 haohou    (1001) haohou    (1000)      270 2022-06-30 23:39:02.000000 pyd4-0.3.6.2/Cargo.toml
--rw-rw-r--   0 haohou    (1001) haohou    (1000)     4688 2022-06-30 23:55:03.902609 pyd4-0.3.6.2/PKG-INFO
--rw-rw-r--   0 haohou    (1001) haohou    (1000)     4214 2022-03-04 18:29:47.000000 pyd4-0.3.6.2/README.md
-drwxrwxr-x   0 haohou    (1001) haohou    (1000)        0 2022-06-30 23:55:03.902609 pyd4-0.3.6.2/pyd4/
--rw-rw-r--   0 haohou    (1001) haohou    (1000)    18222 2022-02-15 22:03:15.000000 pyd4-0.3.6.2/pyd4/__init__.py
-drwxrwxr-x   0 haohou    (1001) haohou    (1000)        0 2022-06-30 23:55:03.902609 pyd4-0.3.6.2/pyd4.egg-info/
--rw-rw-r--   0 haohou    (1001) haohou    (1000)     4688 2022-06-30 23:55:03.000000 pyd4-0.3.6.2/pyd4.egg-info/PKG-INFO
--rw-rw-r--   0 haohou    (1001) haohou    (1000)      216 2022-06-30 23:55:03.000000 pyd4-0.3.6.2/pyd4.egg-info/SOURCES.txt
--rw-rw-r--   0 haohou    (1001) haohou    (1000)        1 2022-06-30 23:55:03.000000 pyd4-0.3.6.2/pyd4.egg-info/dependency_links.txt
--rw-rw-r--   0 haohou    (1001) haohou    (1000)        1 2021-11-16 19:54:59.000000 pyd4-0.3.6.2/pyd4.egg-info/not-zip-safe
--rw-rw-r--   0 haohou    (1001) haohou    (1000)        6 2022-06-30 23:55:03.000000 pyd4-0.3.6.2/pyd4.egg-info/requires.txt
--rw-rw-r--   0 haohou    (1001) haohou    (1000)        5 2022-06-30 23:55:03.000000 pyd4-0.3.6.2/pyd4.egg-info/top_level.txt
--rw-rw-r--   0 haohou    (1001) haohou    (1000)      133 2021-11-16 19:31:34.000000 pyd4-0.3.6.2/pyproject.toml
--rw-rw-r--   0 haohou    (1001) haohou    (1000)       38 2022-06-30 23:55:03.902609 pyd4-0.3.6.2/setup.cfg
--rwxrwxr-x   0 haohou    (1001) haohou    (1000)     1718 2022-06-30 23:54:25.000000 pyd4-0.3.6.2/setup.py
-drwxrwxr-x   0 haohou    (1001) haohou    (1000)        0 2022-06-30 23:55:03.902609 pyd4-0.3.6.2/src/
--rw-rw-r--   0 haohou    (1001) haohou    (1000)     8084 2022-06-30 23:53:28.000000 pyd4-0.3.6.2/src/builder.rs
--rw-rw-r--   0 haohou    (1001) haohou    (1000)    10064 2022-02-14 18:09:04.000000 pyd4-0.3.6.2/src/d4file.rs
--rw-rw-r--   0 haohou    (1001) haohou    (1000)     2466 2022-01-25 23:11:45.000000 pyd4-0.3.6.2/src/iter.rs
--rw-rw-r--   0 haohou    (1001) haohou    (1000)     2725 2022-01-25 23:11:45.000000 pyd4-0.3.6.2/src/lib.rs
+drwxrwxr-x   0 haohou    (1001) haohou    (1000)        0 2023-07-29 15:05:16.539927 pyd4-0.3.9/
+-rw-rw-r--   0 haohou    (1001) haohou    (1000)      273 2023-07-29 14:05:48.000000 pyd4-0.3.9/Cargo.toml
+-rw-rw-r--   0 haohou    (1001) haohou    (1000)     4686 2023-07-29 15:05:16.539927 pyd4-0.3.9/PKG-INFO
+-rw-rw-r--   0 haohou    (1001) haohou    (1000)     4214 2023-07-29 13:59:08.000000 pyd4-0.3.9/README.md
+drwxrwxr-x   0 haohou    (1001) haohou    (1000)        0 2023-07-29 15:05:16.535927 pyd4-0.3.9/pyd4/
+-rw-rw-r--   0 haohou    (1001) haohou    (1000)    18222 2023-07-29 13:59:08.000000 pyd4-0.3.9/pyd4/__init__.py
+drwxrwxr-x   0 haohou    (1001) haohou    (1000)        0 2023-07-29 15:05:16.535927 pyd4-0.3.9/pyd4.egg-info/
+-rw-rw-r--   0 haohou    (1001) haohou    (1000)     4686 2023-07-29 15:05:16.000000 pyd4-0.3.9/pyd4.egg-info/PKG-INFO
+-rw-rw-r--   0 haohou    (1001) haohou    (1000)      216 2023-07-29 15:05:16.000000 pyd4-0.3.9/pyd4.egg-info/SOURCES.txt
+-rw-rw-r--   0 haohou    (1001) haohou    (1000)        1 2023-07-29 15:05:16.000000 pyd4-0.3.9/pyd4.egg-info/dependency_links.txt
+-rw-rw-r--   0 haohou    (1001) haohou    (1000)        1 2023-07-29 15:05:16.000000 pyd4-0.3.9/pyd4.egg-info/not-zip-safe
+-rw-rw-r--   0 haohou    (1001) haohou    (1000)        6 2023-07-29 15:05:16.000000 pyd4-0.3.9/pyd4.egg-info/requires.txt
+-rw-rw-r--   0 haohou    (1001) haohou    (1000)        5 2023-07-29 15:05:16.000000 pyd4-0.3.9/pyd4.egg-info/top_level.txt
+-rw-rw-r--   0 haohou    (1001) haohou    (1000)      133 2023-07-29 13:59:08.000000 pyd4-0.3.9/pyproject.toml
+-rw-rw-r--   0 haohou    (1001) haohou    (1000)       38 2023-07-29 15:05:16.539927 pyd4-0.3.9/setup.cfg
+-rwxrwxr-x   0 haohou    (1001) haohou    (1000)     1716 2023-07-29 15:04:02.000000 pyd4-0.3.9/setup.py
+drwxrwxr-x   0 haohou    (1001) haohou    (1000)        0 2023-07-29 15:05:16.539927 pyd4-0.3.9/src/
+-rw-rw-r--   0 haohou    (1001) haohou    (1000)     8084 2023-07-29 13:59:08.000000 pyd4-0.3.9/src/builder.rs
+-rw-rw-r--   0 haohou    (1001) haohou    (1000)    10064 2023-07-29 13:59:08.000000 pyd4-0.3.9/src/d4file.rs
+-rw-rw-r--   0 haohou    (1001) haohou    (1000)     2466 2023-07-29 13:59:08.000000 pyd4-0.3.9/src/iter.rs
+-rw-rw-r--   0 haohou    (1001) haohou    (1000)     2725 2023-07-29 13:59:08.000000 pyd4-0.3.9/src/lib.rs
```

### Comparing `pyd4-0.3.6.2/PKG-INFO` & `pyd4-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyd4
-Version: 0.3.6.2
+Version: 0.3.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyd4-0.3.6.2/README.md` & `pyd4-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pyd4-0.3.6.2/pyd4/__init__.py` & `pyd4-0.3.9/pyd4/__init__.py`

 * *Files identical despite different names*

### Comparing `pyd4-0.3.6.2/pyd4.egg-info/PKG-INFO` & `pyd4-0.3.9/pyd4.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyd4
-Version: 0.3.6.2
+Version: 0.3.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyd4-0.3.6.2/setup.py` & `pyd4-0.3.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 
 setup_requires = ["setuptools-rust>=0.10.1", "wheel"]
 install_requires = ["numpy"]
 
 setup(
     name="pyd4",
-    version="0.3.6.2",
+    version="0.3.9",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Rust",
         "Operating System :: POSIX",
```

### Comparing `pyd4-0.3.6.2/src/builder.rs` & `pyd4-0.3.9/src/builder.rs`

 * *Files identical despite different names*

### Comparing `pyd4-0.3.6.2/src/d4file.rs` & `pyd4-0.3.9/src/d4file.rs`

 * *Files identical despite different names*

### Comparing `pyd4-0.3.6.2/src/iter.rs` & `pyd4-0.3.9/src/iter.rs`

 * *Files identical despite different names*

### Comparing `pyd4-0.3.6.2/src/lib.rs` & `pyd4-0.3.9/src/lib.rs`

 * *Files identical despite different names*

