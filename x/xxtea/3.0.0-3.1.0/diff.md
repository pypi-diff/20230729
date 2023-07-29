# Comparing `tmp/xxtea-3.0.0.tar.gz` & `tmp/xxtea-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xxtea-3.0.0.tar", last modified: Fri Apr 14 15:49:33 2023, max compression
+gzip compressed data, was "xxtea-3.1.0.tar", last modified: Sat Jul 29 15:05:37 2023, max compression
```

## Comparing `xxtea-3.0.0.tar` & `xxtea-3.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:49:33.410758 xxtea-3.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:49:33.406758 xxtea-3.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:49:33.410758 xxtea-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2759 2023-04-14 15:49:28.000000 xxtea-3.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-14 15:49:28.000000 xxtea-3.0.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-04-14 15:49:28.000000 xxtea-3.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-04-14 15:49:28.000000 xxtea-3.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-04-14 15:49:28.000000 xxtea-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-04-14 15:49:28.000000 xxtea-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6657 2023-04-14 15:49:33.410758 xxtea-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-04-14 15:49:28.000000 xxtea-3.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-04-14 15:49:28.000000 xxtea-3.0.0/bench.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      748 2023-04-14 15:49:28.000000 xxtea-3.0.0/bench.sh
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-14 15:49:33.410758 xxtea-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-04-14 15:49:28.000000 xxtea-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:49:33.410758 xxtea-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 15:49:28.000000 xxtea-3.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3778 2023-04-14 15:49:28.000000 xxtea-3.0.0/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (122)    12130 2023-04-14 15:49:28.000000 xxtea-3.0.0/xxtea.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:49:33.410758 xxtea-3.0.0/xxtea.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6657 2023-04-14 15:49:33.000000 xxtea-3.0.0/xxtea.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-04-14 15:49:33.000000 xxtea-3.0.0/xxtea.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 15:49:33.000000 xxtea-3.0.0/xxtea.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-14 15:49:33.000000 xxtea-3.0.0/xxtea.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 15:05:37.863187 xxtea-3.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 15:05:37.859187 xxtea-3.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 15:05:37.863187 xxtea-3.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2812 2023-07-29 15:05:31.000000 xxtea-3.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-07-29 15:05:31.000000 xxtea-3.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-29 15:05:31.000000 xxtea-3.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-07-29 15:05:31.000000 xxtea-3.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-07-29 15:05:31.000000 xxtea-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-07-29 15:05:31.000000 xxtea-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6657 2023-07-29 15:05:37.863187 xxtea-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-07-29 15:05:31.000000 xxtea-3.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-07-29 15:05:31.000000 xxtea-3.1.0/bench.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      748 2023-07-29 15:05:31.000000 xxtea-3.1.0/bench.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-29 15:05:37.863187 xxtea-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-07-29 15:05:31.000000 xxtea-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 15:05:37.863187 xxtea-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-29 15:05:31.000000 xxtea-3.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3778 2023-07-29 15:05:31.000000 xxtea-3.1.0/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11896 2023-07-29 15:05:31.000000 xxtea-3.1.0/xxtea.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 15:05:37.863187 xxtea-3.1.0/xxtea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6657 2023-07-29 15:05:37.000000 xxtea-3.1.0/xxtea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-07-29 15:05:37.000000 xxtea-3.1.0/xxtea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-29 15:05:37.000000 xxtea-3.1.0/xxtea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-29 15:05:37.000000 xxtea-3.1.0/xxtea.egg-info/top_level.txt
```

### Comparing `xxtea-3.0.0/.github/workflows/build.yml` & `xxtea-3.1.0/.github/workflows/build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,17 @@
         archs: ["x86_64, i686", "aarch64", "ppc64le", "s390x"]
         build: ["manylinux", "musllinux"]
         include:
           - os: windows-2019
             archs: "AMD64"
           - os: windows-2019
             archs: "x86"
-          - os: macos-10.15
+          - os: windows-2019
+            archs: "ARM64"
+          - os: macos-11
             archs: "x86_64, arm64"
 
     steps:
       - name: Disable git autocrlf
         run: |
           git config --global core.autocrlf false
           git config --global core.eol lf
```

### Comparing `xxtea-3.0.0/.github/workflows/test.yml` & `xxtea-3.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `xxtea-3.0.0/CHANGELOG.rst` & `xxtea-3.1.0/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 CHANGELOG
 --------------
 
+v3.1.0 2023/07/29
+~~~~~~~~~~~~~~~~~~~
+
+- Build windows arm64 wheels
+
+v3.0.0 2023/05/06
+~~~~~~~~~~~~~~~~~~~
+
+- Add support for Python 3.11
+- Fix Py_SET_SIZE for Python 2.x
+- Set up github actions and remove TravisCI and AppVeyor
+- Drop support for Python 2.7, 3.4 and 3.5. Now xxtea requires Python >= 3.6
+
 v2.1.0 2023/04/14
 ~~~~~~~~~~~~~~~~~~~
 
 - Drop support for EOL Python 2.7, 3.4 and 3.5
 - Add support for Python 3.9, 1.10 and 3.11
 
 v2.0.0 2020/01/24
```

### Comparing `xxtea-3.0.0/LICENSE` & `xxtea-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xxtea-3.0.0/PKG-INFO` & `xxtea-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xxtea
-Version: 3.0.0
+Version: 3.1.0
 Summary: xxtea is a simple block cipher
 Home-page: https://github.com/ifduyue/xxtea
 Author: Yue Du
 Author-email: ifduyue@gmail.com
 License: BSD
 Keywords: xxtea
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xxtea-3.0.0/README.rst` & `xxtea-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `xxtea-3.0.0/bench.py` & `xxtea-3.1.0/bench.py`

 * *Files identical despite different names*

### Comparing `xxtea-3.0.0/bench.sh` & `xxtea-3.1.0/bench.sh`

 * *Files identical despite different names*

### Comparing `xxtea-3.0.0/setup.py` & `xxtea-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `xxtea-3.0.0/tests/test.py` & `xxtea-3.1.0/tests/test.py`

 * *Files identical despite different names*

### Comparing `xxtea-3.0.0/xxtea.c` & `xxtea-3.1.0/xxtea.c`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  */
 
 
 #include <Python.h>
 #include <ctype.h>
 #include <stdio.h>
 
-#define VERSION "3.0.0"
+#define VERSION "3.1.0"
 
 #if PY_MAJOR_VERSION >= 3
 #define PyString_FromStringAndSize PyBytes_FromStringAndSize
 #define PyString_AS_STRING PyBytes_AsString
 #endif
 
 #if PY_VERSION_HEX < 0x030900A4 && !defined(Py_SET_SIZE)
@@ -411,53 +411,36 @@
     {"encrypt", (PyCFunction)xxtea_encrypt, METH_VARARGS | METH_KEYWORDS, xxtea_encrypt_doc},
     {"decrypt", (PyCFunction)xxtea_decrypt, METH_VARARGS | METH_KEYWORDS, xxtea_decrypt_doc},
     {"encrypt_hex", (PyCFunction)xxtea_encrypt_hex, METH_VARARGS | METH_KEYWORDS, xxtea_encrypt_hex_doc},
     {"decrypt_hex", (PyCFunction)xxtea_decrypt_hex, METH_VARARGS | METH_KEYWORDS, xxtea_decrypt_hex_doc},
     {NULL, NULL, 0, NULL}
 };
 
-#if PY_MAJOR_VERSION >= 3
-
 static struct PyModuleDef moduledef = {
     PyModuleDef_HEAD_INIT,
     "xxtea",
     NULL,
     -1,
     methods,
     NULL,
     NULL,
     NULL,
     NULL
 };
 
-#define INITERROR return NULL
 
 PyObject *PyInit_xxtea(void)
-
-#else
-
-#define INITERROR return
-
-void initxxtea(void)
-#endif
 {
-#if PY_MAJOR_VERSION >= 3
     module = PyModule_Create(&moduledef);
-#else
-    module = Py_InitModule("xxtea", methods);
-#endif
 
     if (module == NULL) {
-        INITERROR;
+        return NULL;
     }
     if (!(binascii = PyImport_ImportModule("binascii"))) {
         Py_DECREF(module);
-        INITERROR;
+        return NULL;
     }
 
     PyModule_AddStringConstant(module, "VERSION", VERSION);
 
-#if PY_MAJOR_VERSION >= 3
     return module;
-#endif
 }
-
```

### Comparing `xxtea-3.0.0/xxtea.egg-info/PKG-INFO` & `xxtea-3.1.0/xxtea.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xxtea
-Version: 3.0.0
+Version: 3.1.0
 Summary: xxtea is a simple block cipher
 Home-page: https://github.com/ifduyue/xxtea
 Author: Yue Du
 Author-email: ifduyue@gmail.com
 License: BSD
 Keywords: xxtea
 Classifier: Development Status :: 5 - Production/Stable
```

