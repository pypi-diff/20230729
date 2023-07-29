# Comparing `tmp/Finance-Hermes-0.2.8.tar.gz` & `tmp/Finance-Hermes-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Finance-Hermes-0.2.8.tar", last modified: Wed Jul 12 05:13:55 2023, max compression
+gzip compressed data, was "dist/Finance-Hermes-0.2.9.tar", last modified: Sat Jul 29 02:01:44 2023, max compression
```

## Comparing `Finance-Hermes-0.2.8.tar` & `Finance-Hermes-0.2.9.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:13:55.000000 Finance-Hermes-0.2.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:13:55.000000 Finance-Hermes-0.2.8/Finance_Hermes.egg-info/
--rw-r--r--   0 root         (0) root         (0)      222 2023-07-12 05:13:54.000000 Finance-Hermes-0.2.8/Finance_Hermes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      751 2023-07-12 05:13:54.000000 Finance-Hermes-0.2.8/Finance_Hermes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 05:13:54.000000 Finance-Hermes-0.2.8/Finance_Hermes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-12 05:13:54.000000 Finance-Hermes-0.2.8/Finance_Hermes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-12 05:13:54.000000 Finance-Hermes-0.2.8/Finance_Hermes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      358 2023-06-24 10:42:40.000000 Finance-Hermes-0.2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      222 2023-07-12 05:13:55.000000 Finance-Hermes-0.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      195 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:13:55.000000 Finance-Hermes-0.2.8/hermes/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-12 05:12:02.000000 Finance-Hermes-0.2.8/hermes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:13:55.000000 Finance-Hermes-0.2.8/hermes/factors/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.8/hermes/factors/__init__.py
--rw-r--r--   0 root         (0) root         (0)   329352 2023-07-12 05:13:54.000000 Finance-Hermes-0.2.8/hermes/factors/base.c
--rw-r--r--   0 root         (0) root         (0)     4120 2023-07-12 05:13:03.000000 Finance-Hermes-0.2.8/hermes/factors/base.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:13:55.000000 Finance-Hermes-0.2.8/hermes/kdutils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.8/hermes/kdutils/__init__.py
--rw-r--r--   0 root         (0) root         (0)   271147 2023-06-24 10:51:00.000000 Finance-Hermes-0.2.8/hermes/kdutils/base.c
--rw-r--r--   0 root         (0) root         (0)     2338 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.8/hermes/kdutils/base.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:13:55.000000 Finance-Hermes-0.2.8/hermes/kdutils/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.8/hermes/kdutils/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)   678491 2023-06-24 10:39:53.000000 Finance-Hermes-0.2.8/hermes/kdutils/core/fixes.c
--rw-r--r--   0 root         (0) root         (0)     9714 2022-11-11 12:13:52.000000 Finance-Hermes-0.2.8/hermes/kdutils/core/fixes.pyx
--rw-r--r--   0 root         (0) root         (0)   392670 2023-06-24 10:39:53.000000 Finance-Hermes-0.2.8/hermes/kdutils/core/helper.c
--rw-r--r--   0 root         (0) root         (0)     7825 2022-11-11 12:13:52.000000 Finance-Hermes-0.2.8/hermes/kdutils/core/helper.pyx
--rw-r--r--   0 root         (0) root         (0)   190192 2023-06-24 10:51:00.000000 Finance-Hermes-0.2.8/hermes/kdutils/create_id.c
--rw-r--r--   0 root         (0) root         (0)      870 2023-06-21 21:57:15.000000 Finance-Hermes-0.2.8/hermes/kdutils/create_id.pyx
--rw-r--r--   0 root         (0) root         (0)   235985 2023-06-24 10:51:00.000000 Finance-Hermes-0.2.8/hermes/kdutils/lazy.c
--rw-r--r--   0 root         (0) root         (0)     1578 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.8/hermes/kdutils/lazy.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:13:55.000000 Finance-Hermes-0.2.8/hermes/lzador/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.8/hermes/lzador/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161732 2023-06-24 10:51:00.000000 Finance-Hermes-0.2.8/hermes/lzador/calculater.c
--rw-r--r--   0 root         (0) root         (0)      657 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.8/hermes/lzador/calculater.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:13:55.000000 Finance-Hermes-0.2.8/requirements/
--rw-r--r--   0 root         (0) root         (0)       90 2023-06-24 12:13:59.000000 Finance-Hermes-0.2.8/requirements/py3.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 05:13:55.000000 Finance-Hermes-0.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3292 2023-07-11 12:09:04.000000 Finance-Hermes-0.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/Finance_Hermes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      233 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/Finance_Hermes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      829 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/Finance_Hermes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/Finance_Hermes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/Finance_Hermes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/Finance_Hermes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-11-01 07:48:09.000000 Finance-Hermes-0.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      358 2023-07-29 01:53:47.000000 Finance-Hermes-0.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      233 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      195 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-29 01:59:31.000000 Finance-Hermes-0.2.9/hermes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.9/hermes/factors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   339663 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/factors/base.c
+-rw-r--r--   0 root         (0) root         (0)     4469 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/hermes/factors/base.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/factors/test/
+-rw-r--r--   0 root         (0) root         (0)   241630 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/factors/test/factor_test.c
+-rw-r--r--   0 root         (0) root         (0)     2056 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/hermes/factors/test/factor_test.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/kdutils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.9/hermes/kdutils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   271147 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/kdutils/base.c
+-rw-r--r--   0 root         (0) root         (0)     2338 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/hermes/kdutils/base.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/kdutils/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.9/hermes/kdutils/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   678491 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/kdutils/core/fixes.c
+-rw-r--r--   0 root         (0) root         (0)     9714 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/hermes/kdutils/core/fixes.pyx
+-rw-r--r--   0 root         (0) root         (0)   392670 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/kdutils/core/helper.c
+-rw-r--r--   0 root         (0) root         (0)     7825 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/hermes/kdutils/core/helper.pyx
+-rw-r--r--   0 root         (0) root         (0)   190192 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/kdutils/create_id.c
+-rw-r--r--   0 root         (0) root         (0)      870 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/hermes/kdutils/create_id.pyx
+-rw-r--r--   0 root         (0) root         (0)   235985 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/kdutils/lazy.c
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/hermes/kdutils/lazy.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/lzador/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/hermes/lzador/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161732 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/lzador/calculater.c
+-rw-r--r--   0 root         (0) root         (0)      657 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/hermes/lzador/calculater.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/requirements/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/requirements/py3.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3331 2023-07-29 01:55:31.000000 Finance-Hermes-0.2.9/setup.py
```

### Comparing `Finance-Hermes-0.2.8/Finance_Hermes.egg-info/SOURCES.txt` & `Finance-Hermes-0.2.9/Finance_Hermes.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 ./README.md
 Finance_Hermes.egg-info/PKG-INFO
 Finance_Hermes.egg-info/SOURCES.txt
 Finance_Hermes.egg-info/dependency_links.txt
 Finance_Hermes.egg-info/requires.txt
 Finance_Hermes.egg-info/top_level.txt
 hermes/__init__.py
 hermes/factors/__init__.py
 hermes/factors/base.c
 hermes/factors/base.pyx
+hermes/factors/test/factor_test.c
+hermes/factors/test/factor_test.pyx
 hermes/kdutils/__init__.py
 hermes/kdutils/base.c
 hermes/kdutils/base.pyx
 hermes/kdutils/create_id.c
 hermes/kdutils/create_id.pyx
 hermes/kdutils/lazy.c
 hermes/kdutils/lazy.pyx
```

### Comparing `Finance-Hermes-0.2.8/hermes/factors/base.c` & `Finance-Hermes-0.2.9/hermes/factors/base.c`

 * *Files 1% similar despite different names*

```diff
@@ -827,15 +827,15 @@
 static const char *__pyx_f[] = {
   "hermes/factors/base.pyx",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list;
 
-/* "hermes/factors/base.pyx":132
+/* "hermes/factors/base.pyx":141
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
 struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list {
@@ -1054,14 +1054,20 @@
 
 /* PySequenceContains.proto */
 static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
     int result = PySequence_Contains(seq, item);
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
+/* HasAttr.proto */
+static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
+
+/* PyIntCompare.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
+
 /* PyObjectSetAttrStr.proto */
 #if CYTHON_USE_TYPE_SLOTS
 #define __Pyx_PyObject_DelAttrStr(o,n) __Pyx_PyObject_SetAttrStr(o, n, NULL)
 static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value);
 #else
 #define __Pyx_PyObject_DelAttrStr(o,n)   PyObject_DelAttr(o,n)
 #define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
@@ -1348,14 +1354,15 @@
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_digit[] = "digit";
 static const char __pyx_k_dumps[] = "dumps";
 static const char __pyx_k_items[] = "items";
 static const char __pyx_k_short[] = "short";
 static const char __pyx_k_stack[] = "stack";
 static const char __pyx_k_utf_8[] = "utf-8";
+static const char __pyx_k_value[] = "value";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_filter[] = "filter";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_kwargs[] = "kwargs";
 static const char __pyx_k_method[] = "method";
 static const char __pyx_k_module[] = "__module__";
@@ -1387,19 +1394,22 @@
 static const char __pyx_k_signature[] = "signature";
 static const char __pyx_k_FactorBase[] = "FactorBase";
 static const char __pyx_k_ShortMixin[] = "ShortMixin";
 static const char __pyx_k_begin_date[] = "begin_date";
 static const char __pyx_k_parameters[] = "parameters";
 static const char __pyx_k_startswith[] = "startswith";
 static const char __pyx_k_create_id_2[] = "_create_id";
+static const char __pyx_k_data_format[] = "_data_format";
 static const char __pyx_k_func_module[] = "func_module";
 static const char __pyx_k_member_func[] = "member_func";
+static const char __pyx_k_reset_index[] = "reset_index";
 static const char __pyx_k_dependencies[] = "dependencies";
 static const char __pyx_k_factors_list[] = "factors_list";
 static const char __pyx_k_LongCallMixin[] = "LongCallMixin";
+static const char __pyx_k_data_format_2[] = "data_format";
 static const char __pyx_k_long_type_str[] = "long_type_str";
 static const char __pyx_k_ShortCallMixin[] = "ShortCallMixin";
 static const char __pyx_k_abstractmethod[] = "abstractmethod";
 static const char __pyx_k_short_type_str[] = "short_type_str";
 static const char __pyx_k_with_metaclass[] = "with_metaclass";
 static const char __pyx_k_FreezeAttrMixin[] = "FreezeAttrMixin";
 static const char __pyx_k_get_data_by_map[] = "get_data_by_map";
@@ -1459,14 +1469,16 @@
 static PyObject *__pyx_n_s_category;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_columns;
 static PyObject *__pyx_n_s_copy;
 static PyObject *__pyx_n_s_create_id;
 static PyObject *__pyx_n_s_create_id_2;
 static PyObject *__pyx_n_s_data;
+static PyObject *__pyx_n_s_data_format;
+static PyObject *__pyx_n_s_data_format_2;
 static PyObject *__pyx_n_s_ddb;
 static PyObject *__pyx_n_s_deepcopy;
 static PyObject *__pyx_n_s_default;
 static PyObject *__pyx_n_s_dependencies;
 static PyObject *__pyx_n_s_dependencies_list;
 static PyObject *__pyx_n_s_digit;
 static PyObject *__pyx_n_s_doc;
@@ -1513,24 +1525,26 @@
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_name_2;
 static PyObject *__pyx_n_s_original;
 static PyObject *__pyx_n_s_parameters;
 static PyObject *__pyx_n_s_pdb;
 static PyObject *__pyx_n_s_prepare;
 static PyObject *__pyx_n_s_qualname;
+static PyObject *__pyx_n_s_reset_index;
 static PyObject *__pyx_n_s_s;
 static PyObject *__pyx_n_s_self;
 static PyObject *__pyx_n_s_short;
 static PyObject *__pyx_n_s_short_type_str;
 static PyObject *__pyx_n_s_signature;
 static PyObject *__pyx_n_s_six;
 static PyObject *__pyx_n_s_stack;
 static PyObject *__pyx_n_s_startswith;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_kp_s_utf_8;
+static PyObject *__pyx_n_s_value;
 static PyObject *__pyx_n_s_with_metaclass;
 static PyObject *__pyx_pf_6hermes_7factors_4base_13LongCallMixin_long_type_str(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4base_13LongCallMixin_2expect_direction(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4base_10ShortMixin_short_type_str(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4base_10ShortMixin_2expect_direction(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4base_10ShortMixin_4short_type_str(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4base_10ShortMixin_6expect_direction(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
@@ -1543,14 +1557,16 @@
 static PyObject *__pyx_pf_6hermes_7factors_4base_10FactorBase_8_create_id(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_kwargs); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4base_10FactorBase_10_format(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data, PyObject *__pyx_v_name, PyObject *__pyx_v_kwargs); /* proto */
 static PyObject *__pyx_lambda_funcdef_lambda(PyObject *__pyx_self, PyObject *__pyx_v_x); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4base_10FactorBase_12factors_list(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_tp_new_6hermes_7factors_4base___pyx_scope_struct__factors_list(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_float_1_0;
 static PyObject *__pyx_float_neg_1_0;
+static PyObject *__pyx_int_1;
+static PyObject *__pyx_int_2;
 static PyObject *__pyx_int_10;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__12;
@@ -2099,15 +2115,15 @@
   __Pyx_RefNannySetupContext("__init__", 0);
 
   /* "hermes/factors/base.pyx":86
  *     def __init__(self, **kwargs):
  *         #
  *         self._init_self(**kwargs)             # <<<<<<<<<<<<<<
  * 
- *     @abstractmethod
+ * 
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_v_kwargs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -2130,15 +2146,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":89
+/* "hermes/factors/base.pyx":90
  * 
  *     @abstractmethod
  *     def _init_self(self, **kwargs):             # <<<<<<<<<<<<<<
  *         """"""
  *         pass
  */
 
@@ -2172,26 +2188,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_init_self") < 0)) __PYX_ERR(0, 89, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_init_self") < 0)) __PYX_ERR(0, 90, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_init_self", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 89, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_init_self", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 90, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("hermes.factors.base.FactorBase._init_self", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6hermes_7factors_4base_10FactorBase_2_init_self(__pyx_self, __pyx_v_self, __pyx_v_kwargs);
@@ -2210,15 +2226,15 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":93
+/* "hermes/factors/base.pyx":94
  *         pass
  * 
  *     def init_data(self, **kwargs):             # <<<<<<<<<<<<<<
  *         dependencies_list = self.get_dependencies()
  *         method = 'ddb' if 'method' not in kwargs else kwargs['method']
  */
 
@@ -2252,26 +2268,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "init_data") < 0)) __PYX_ERR(0, 93, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "init_data") < 0)) __PYX_ERR(0, 94, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("init_data", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 93, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("init_data", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 94, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("hermes.factors.base.FactorBase.init_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6hermes_7factors_4base_10FactorBase_4init_data(__pyx_self, __pyx_v_self, __pyx_v_kwargs);
@@ -2293,134 +2309,134 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("init_data", 0);
 
-  /* "hermes/factors/base.pyx":94
+  /* "hermes/factors/base.pyx":95
  * 
  *     def init_data(self, **kwargs):
  *         dependencies_list = self.get_dependencies()             # <<<<<<<<<<<<<<
  *         method = 'ddb' if 'method' not in kwargs else kwargs['method']
  *         data = get_data_by_map(columns=dependencies_list,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_dependencies); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_dependencies); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_dependencies_list = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":95
+  /* "hermes/factors/base.pyx":96
  *     def init_data(self, **kwargs):
  *         dependencies_list = self.get_dependencies()
  *         method = 'ddb' if 'method' not in kwargs else kwargs['method']             # <<<<<<<<<<<<<<
  *         data = get_data_by_map(columns=dependencies_list,
  *                       begin_date=kwargs['begin_date'],
  */
-  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_method, __pyx_v_kwargs, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_method, __pyx_v_kwargs, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 96, __pyx_L1_error)
   if ((__pyx_t_4 != 0)) {
     __Pyx_INCREF(__pyx_n_s_ddb);
     __pyx_t_1 = __pyx_n_s_ddb;
   } else {
-    __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_s_method); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_s_method); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 96, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
     __pyx_t_2 = 0;
   }
   __pyx_v_method = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":96
+  /* "hermes/factors/base.pyx":97
  *         dependencies_list = self.get_dependencies()
  *         method = 'ddb' if 'method' not in kwargs else kwargs['method']
  *         data = get_data_by_map(columns=dependencies_list,             # <<<<<<<<<<<<<<
  *                       begin_date=kwargs['begin_date'],
  *                       end_date=kwargs['end_date'],
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_get_data_by_map); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_get_data_by_map); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_columns, __pyx_v_dependencies_list) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_columns, __pyx_v_dependencies_list) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":97
+  /* "hermes/factors/base.pyx":98
  *         method = 'ddb' if 'method' not in kwargs else kwargs['method']
  *         data = get_data_by_map(columns=dependencies_list,
  *                       begin_date=kwargs['begin_date'],             # <<<<<<<<<<<<<<
  *                       end_date=kwargs['end_date'],
  *                       method=method)
  */
-  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_s_begin_date); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_s_begin_date); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_begin_date, __pyx_t_3) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_begin_date, __pyx_t_3) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "hermes/factors/base.pyx":98
+  /* "hermes/factors/base.pyx":99
  *         data = get_data_by_map(columns=dependencies_list,
  *                       begin_date=kwargs['begin_date'],
  *                       end_date=kwargs['end_date'],             # <<<<<<<<<<<<<<
  *                       method=method)
  *         return data
  */
-  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_s_end_date); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_s_end_date); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_end_date, __pyx_t_3) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_end_date, __pyx_t_3) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "hermes/factors/base.pyx":99
+  /* "hermes/factors/base.pyx":100
  *                       begin_date=kwargs['begin_date'],
  *                       end_date=kwargs['end_date'],
  *                       method=method)             # <<<<<<<<<<<<<<
  *         return data
  * 
  */
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_method, __pyx_v_method) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_method, __pyx_v_method) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":96
+  /* "hermes/factors/base.pyx":97
  *         dependencies_list = self.get_dependencies()
  *         method = 'ddb' if 'method' not in kwargs else kwargs['method']
  *         data = get_data_by_map(columns=dependencies_list,             # <<<<<<<<<<<<<<
  *                       begin_date=kwargs['begin_date'],
  *                       end_date=kwargs['end_date'],
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_data = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "hermes/factors/base.pyx":100
+  /* "hermes/factors/base.pyx":101
  *                       end_date=kwargs['end_date'],
  *                       method=method)
  *         return data             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_data);
   __pyx_r = __pyx_v_data;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":93
+  /* "hermes/factors/base.pyx":94
  *         pass
  * 
  *     def init_data(self, **kwargs):             # <<<<<<<<<<<<<<
  *         dependencies_list = self.get_dependencies()
  *         method = 'ddb' if 'method' not in kwargs else kwargs['method']
  */
 
@@ -2436,15 +2452,15 @@
   __Pyx_XDECREF(__pyx_v_method);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":104
+/* "hermes/factors/base.pyx":105
  * 
  * 
  *     def get_dependencies(self):             # <<<<<<<<<<<<<<
  *         dependencies_list = []
  *         member_func = self.factors_list()
  */
 
@@ -2481,222 +2497,222 @@
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_dependencies", 0);
 
-  /* "hermes/factors/base.pyx":105
+  /* "hermes/factors/base.pyx":106
  * 
  *     def get_dependencies(self):
  *         dependencies_list = []             # <<<<<<<<<<<<<<
  *         member_func = self.factors_list()
  *         for func in member_func:
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_dependencies_list = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":106
+  /* "hermes/factors/base.pyx":107
  *     def get_dependencies(self):
  *         dependencies_list = []
  *         member_func = self.factors_list()             # <<<<<<<<<<<<<<
  *         for func in member_func:
  *             func_module = getattr(self, func)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_factors_list); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_factors_list); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_member_func = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":107
+  /* "hermes/factors/base.pyx":108
  *         dependencies_list = []
  *         member_func = self.factors_list()
  *         for func in member_func:             # <<<<<<<<<<<<<<
  *             func_module = getattr(self, func)
  *             fun_param = inspect.signature(func_module).parameters
  */
   if (likely(PyList_CheckExact(__pyx_v_member_func)) || PyTuple_CheckExact(__pyx_v_member_func)) {
     __pyx_t_1 = __pyx_v_member_func; __Pyx_INCREF(__pyx_t_1); __pyx_t_4 = 0;
     __pyx_t_5 = NULL;
   } else {
-    __pyx_t_4 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_member_func); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __pyx_t_4 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_member_func); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __pyx_t_5 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 108, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_5)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 107, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 108, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
         if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 107, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 108, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
       __pyx_t_2 = __pyx_t_5(__pyx_t_1);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 107, __pyx_L1_error)
+          else __PYX_ERR(0, 108, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
     __Pyx_XDECREF_SET(__pyx_v_func, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "hermes/factors/base.pyx":108
+    /* "hermes/factors/base.pyx":109
  *         member_func = self.factors_list()
  *         for func in member_func:
  *             func_module = getattr(self, func)             # <<<<<<<<<<<<<<
  *             fun_param = inspect.signature(func_module).parameters
  *             if 'dependencies' in fun_param:
  */
-    __pyx_t_2 = __Pyx_GetAttr(__pyx_v_self, __pyx_v_func); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetAttr(__pyx_v_self, __pyx_v_func); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_XDECREF_SET(__pyx_v_func_module, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "hermes/factors/base.pyx":109
+    /* "hermes/factors/base.pyx":110
  *         for func in member_func:
  *             func_module = getattr(self, func)
  *             fun_param = inspect.signature(func_module).parameters             # <<<<<<<<<<<<<<
  *             if 'dependencies' in fun_param:
  *                 dependencies = fun_param['dependencies'].default
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_inspect); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 109, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_inspect); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 110, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_signature); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_signature); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 110, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_3, __pyx_v_func_module) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_func_module);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 109, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_parameters); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_parameters); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 110, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF_SET(__pyx_v_fun_param, __pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "hermes/factors/base.pyx":110
+    /* "hermes/factors/base.pyx":111
  *             func_module = getattr(self, func)
  *             fun_param = inspect.signature(func_module).parameters
  *             if 'dependencies' in fun_param:             # <<<<<<<<<<<<<<
  *                 dependencies = fun_param['dependencies'].default
  *                 dependencies_list += dependencies
  */
-    __pyx_t_7 = (__Pyx_PySequence_ContainsTF(__pyx_n_s_dependencies, __pyx_v_fun_param, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __pyx_t_7 = (__Pyx_PySequence_ContainsTF(__pyx_n_s_dependencies, __pyx_v_fun_param, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 111, __pyx_L1_error)
     __pyx_t_8 = (__pyx_t_7 != 0);
     if (__pyx_t_8) {
 
-      /* "hermes/factors/base.pyx":111
+      /* "hermes/factors/base.pyx":112
  *             fun_param = inspect.signature(func_module).parameters
  *             if 'dependencies' in fun_param:
  *                 dependencies = fun_param['dependencies'].default             # <<<<<<<<<<<<<<
  *                 dependencies_list += dependencies
  *         return list(set(dependencies_list))
  */
-      __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_fun_param, __pyx_n_s_dependencies); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 111, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_fun_param, __pyx_n_s_dependencies); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 112, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_default); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_default); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF_SET(__pyx_v_dependencies, __pyx_t_2);
       __pyx_t_2 = 0;
 
-      /* "hermes/factors/base.pyx":112
+      /* "hermes/factors/base.pyx":113
  *             if 'dependencies' in fun_param:
  *                 dependencies = fun_param['dependencies'].default
  *                 dependencies_list += dependencies             # <<<<<<<<<<<<<<
  *         return list(set(dependencies_list))
  * 
  */
-      __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_v_dependencies_list, __pyx_v_dependencies); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
+      __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_v_dependencies_list, __pyx_v_dependencies); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF_SET(__pyx_v_dependencies_list, __pyx_t_2);
       __pyx_t_2 = 0;
 
-      /* "hermes/factors/base.pyx":110
+      /* "hermes/factors/base.pyx":111
  *             func_module = getattr(self, func)
  *             fun_param = inspect.signature(func_module).parameters
  *             if 'dependencies' in fun_param:             # <<<<<<<<<<<<<<
  *                 dependencies = fun_param['dependencies'].default
  *                 dependencies_list += dependencies
  */
     }
 
-    /* "hermes/factors/base.pyx":107
+    /* "hermes/factors/base.pyx":108
  *         dependencies_list = []
  *         member_func = self.factors_list()
  *         for func in member_func:             # <<<<<<<<<<<<<<
  *             func_module = getattr(self, func)
  *             fun_param = inspect.signature(func_module).parameters
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":113
+  /* "hermes/factors/base.pyx":114
  *                 dependencies = fun_param['dependencies'].default
  *                 dependencies_list += dependencies
  *         return list(set(dependencies_list))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PySet_New(__pyx_v_dependencies_list); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_1 = PySet_New(__pyx_v_dependencies_list); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_2 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":104
+  /* "hermes/factors/base.pyx":105
  * 
  * 
  *     def get_dependencies(self):             # <<<<<<<<<<<<<<
  *         dependencies_list = []
  *         member_func = self.factors_list()
  */
 
@@ -2716,15 +2732,15 @@
   __Pyx_XDECREF(__pyx_v_fun_param);
   __Pyx_XDECREF(__pyx_v_dependencies);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":118
+/* "hermes/factors/base.pyx":119
  * 
  * 
  *     def _create_id(self, **kwargs):             # <<<<<<<<<<<<<<
  *         feature = copy.deepcopy(kwargs)
  *         feature['category'] = self.category
  */
 
@@ -2758,26 +2774,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_create_id") < 0)) __PYX_ERR(0, 118, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_create_id") < 0)) __PYX_ERR(0, 119, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_create_id", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 118, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_create_id", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 119, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("hermes.factors.base.FactorBase._create_id", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6hermes_7factors_4base_10FactorBase_8_create_id(__pyx_self, __pyx_v_self, __pyx_v_kwargs);
@@ -2800,103 +2816,103 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_create_id", 0);
 
-  /* "hermes/factors/base.pyx":119
+  /* "hermes/factors/base.pyx":120
  * 
  *     def _create_id(self, **kwargs):
  *         feature = copy.deepcopy(kwargs)             # <<<<<<<<<<<<<<
  *         feature['category'] = self.category
  *         s = hashlib.md5(
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_copy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_copy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_deepcopy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_deepcopy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_kwargs) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_kwargs);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_feature = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":120
+  /* "hermes/factors/base.pyx":121
  *     def _create_id(self, **kwargs):
  *         feature = copy.deepcopy(kwargs)
  *         feature['category'] = self.category             # <<<<<<<<<<<<<<
  *         s = hashlib.md5(
  *             json.dumps(feature).encode(encoding="utf-8")).hexdigest()
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_category); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_category); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyObject_SetItem(__pyx_v_feature, __pyx_n_s_category, __pyx_t_1) < 0)) __PYX_ERR(0, 120, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_feature, __pyx_n_s_category, __pyx_t_1) < 0)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":121
+  /* "hermes/factors/base.pyx":122
  *         feature = copy.deepcopy(kwargs)
  *         feature['category'] = self.category
  *         s = hashlib.md5(             # <<<<<<<<<<<<<<
  *             json.dumps(feature).encode(encoding="utf-8")).hexdigest()
  *         return "{0}".format(create_id(original=s, digit=10))
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_hashlib); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_hashlib); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_md5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 121, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_md5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "hermes/factors/base.pyx":122
+  /* "hermes/factors/base.pyx":123
  *         feature['category'] = self.category
  *         s = hashlib.md5(
  *             json.dumps(feature).encode(encoding="utf-8")).hexdigest()             # <<<<<<<<<<<<<<
  *         return "{0}".format(create_id(original=s, digit=10))
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_json); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_json); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_dumps); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_dumps); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_5, __pyx_v_feature) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_feature);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_encoding, __pyx_kp_s_utf_8) < 0) __PYX_ERR(0, 122, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 122, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_encoding, __pyx_kp_s_utf_8) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_2)) {
@@ -2905,55 +2921,55 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_hexdigest); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_hexdigest); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_s = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":123
+  /* "hermes/factors/base.pyx":124
  *         s = hashlib.md5(
  *             json.dumps(feature).encode(encoding="utf-8")).hexdigest()
  *         return "{0}".format(create_id(original=s, digit=10))             # <<<<<<<<<<<<<<
  * 
  *     def _format(self, data, name, **kwargs):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_0, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_0, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_create_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_create_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_original, __pyx_v_s) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_digit, __pyx_int_10) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 123, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_original, __pyx_v_s) < 0) __PYX_ERR(0, 124, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_digit, __pyx_int_10) < 0) __PYX_ERR(0, 124, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
@@ -2962,22 +2978,22 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 123, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":118
+  /* "hermes/factors/base.pyx":119
  * 
  * 
  *     def _create_id(self, **kwargs):             # <<<<<<<<<<<<<<
  *         feature = copy.deepcopy(kwargs)
  *         feature['category'] = self.category
  */
 
@@ -2995,20 +3011,20 @@
   __Pyx_XDECREF(__pyx_v_feature);
   __Pyx_XDECREF(__pyx_v_s);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":125
+/* "hermes/factors/base.pyx":126
  *         return "{0}".format(create_id(original=s, digit=10))
  * 
  *     def _format(self, data, name, **kwargs):             # <<<<<<<<<<<<<<
- *         data = data.stack()
- *         data.name = name
+ *         #0 matrix  1 serise  2 DatFrame
+ *         data_format = 1 if not hasattr(self,'_data_format') else self._data_format
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6hermes_7factors_4base_10FactorBase_11_format(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_6hermes_7factors_4base_10FactorBase_10_format[] = "FactorBase._format(self, data, name, **kwargs)";
 static PyMethodDef __pyx_mdef_6hermes_7factors_4base_10FactorBase_11_format = {"_format", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6hermes_7factors_4base_10FactorBase_11_format, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6hermes_7factors_4base_10FactorBase_10_format};
 static PyObject *__pyx_pw_6hermes_7factors_4base_10FactorBase_11_format(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -3045,40 +3061,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_format", 1, 3, 3, 1); __PYX_ERR(0, 125, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_format", 1, 3, 3, 1); __PYX_ERR(0, 126, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_format", 1, 3, 3, 2); __PYX_ERR(0, 125, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_format", 1, 3, 3, 2); __PYX_ERR(0, 126, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_format") < 0)) __PYX_ERR(0, 125, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_format") < 0)) __PYX_ERR(0, 126, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_self = values[0];
     __pyx_v_data = values[1];
     __pyx_v_name = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_format", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 125, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_format", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 126, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("hermes.factors.base.FactorBase._format", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6hermes_7factors_4base_10FactorBase_10_format(__pyx_self, __pyx_v_self, __pyx_v_data, __pyx_v_name, __pyx_v_kwargs);
@@ -3086,130 +3102,254 @@
   /* function exit code */
   __Pyx_XDECREF(__pyx_v_kwargs);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_6hermes_7factors_4base_10FactorBase_10_format(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data, PyObject *__pyx_v_name, PyObject *__pyx_v_kwargs) {
+  PyObject *__pyx_v_data_format = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
+  int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_format", 0);
   __Pyx_INCREF(__pyx_v_data);
 
-  /* "hermes/factors/base.pyx":126
- * 
+  /* "hermes/factors/base.pyx":128
  *     def _format(self, data, name, **kwargs):
- *         data = data.stack()             # <<<<<<<<<<<<<<
+ *         #0 matrix  1 serise  2 DatFrame
+ *         data_format = 1 if not hasattr(self,'_data_format') else self._data_format             # <<<<<<<<<<<<<<
+ *         if data_format == 1 or data_format == 2:
+ *             data = data.stack()
+ */
+  __pyx_t_2 = __Pyx_HasAttr(__pyx_v_self, __pyx_n_s_data_format); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 128, __pyx_L1_error)
+  if (((!(__pyx_t_2 != 0)) != 0)) {
+    __Pyx_INCREF(__pyx_int_1);
+    __pyx_t_1 = __pyx_int_1;
+  } else {
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_1 = __pyx_t_3;
+    __pyx_t_3 = 0;
+  }
+  __pyx_v_data_format = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "hermes/factors/base.pyx":129
+ *         #0 matrix  1 serise  2 DatFrame
+ *         data_format = 1 if not hasattr(self,'_data_format') else self._data_format
+ *         if data_format == 1 or data_format == 2:             # <<<<<<<<<<<<<<
+ *             data = data.stack()
+ *             if data_format == 2:
+ */
+  __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_data_format, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (!__pyx_t_4) {
+  } else {
+    __pyx_t_2 = __pyx_t_4;
+    goto __pyx_L4_bool_binop_done;
+  }
+  __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_data_format, __pyx_int_2, 2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __pyx_t_4;
+  __pyx_L4_bool_binop_done:;
+  if (__pyx_t_2) {
+
+    /* "hermes/factors/base.pyx":130
+ *         data_format = 1 if not hasattr(self,'_data_format') else self._data_format
+ *         if data_format == 1 or data_format == 2:
+ *             data = data.stack()             # <<<<<<<<<<<<<<
+ *             if data_format == 2:
+ *                 data.name = 'value'
+ */
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_stack); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_5 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
+      }
+    }
+    __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_1);
+    __pyx_t_1 = 0;
+
+    /* "hermes/factors/base.pyx":131
+ *         if data_format == 1 or data_format == 2:
+ *             data = data.stack()
+ *             if data_format == 2:             # <<<<<<<<<<<<<<
+ *                 data.name = 'value'
+ *                 data = data.reset_index()
+ */
+    __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_data_format, __pyx_int_2, 2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    if (__pyx_t_2) {
+
+      /* "hermes/factors/base.pyx":132
+ *             data = data.stack()
+ *             if data_format == 2:
+ *                 data.name = 'value'             # <<<<<<<<<<<<<<
+ *                 data = data.reset_index()
+ *                 data['name'] = name
+ */
+      if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_name, __pyx_n_s_value) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+
+      /* "hermes/factors/base.pyx":133
+ *             if data_format == 2:
+ *                 data.name = 'value'
+ *                 data = data.reset_index()             # <<<<<<<<<<<<<<
+ *                 data['name'] = name
+ * 
+ */
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_5 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
+        if (likely(__pyx_t_5)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+          __Pyx_INCREF(__pyx_t_5);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_3, function);
+        }
+      }
+      __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
+      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_1);
+      __pyx_t_1 = 0;
+
+      /* "hermes/factors/base.pyx":134
+ *                 data.name = 'value'
+ *                 data = data.reset_index()
+ *                 data['name'] = name             # <<<<<<<<<<<<<<
+ * 
  *         data.name = name
- *         data.category = self.category
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_stack); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      if (unlikely(PyObject_SetItem(__pyx_v_data, __pyx_n_s_name, __pyx_v_name) < 0)) __PYX_ERR(0, 134, __pyx_L1_error)
+
+      /* "hermes/factors/base.pyx":131
+ *         if data_format == 1 or data_format == 2:
+ *             data = data.stack()
+ *             if data_format == 2:             # <<<<<<<<<<<<<<
+ *                 data.name = 'value'
+ *                 data = data.reset_index()
+ */
     }
+
+    /* "hermes/factors/base.pyx":129
+ *         #0 matrix  1 serise  2 DatFrame
+ *         data_format = 1 if not hasattr(self,'_data_format') else self._data_format
+ *         if data_format == 1 or data_format == 2:             # <<<<<<<<<<<<<<
+ *             data = data.stack()
+ *             if data_format == 2:
+ */
   }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_1);
-  __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":127
- *     def _format(self, data, name, **kwargs):
- *         data = data.stack()
+  /* "hermes/factors/base.pyx":136
+ *                 data['name'] = name
+ * 
  *         data.name = name             # <<<<<<<<<<<<<<
  *         data.category = self.category
  *         data.id = self._create_id(name=name, **kwargs)
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":128
- *         data = data.stack()
+  /* "hermes/factors/base.pyx":137
+ * 
  *         data.name = name
  *         data.category = self.category             # <<<<<<<<<<<<<<
  *         data.id = self._create_id(name=name, **kwargs)
  *         return data
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_category); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_category); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_category, __pyx_t_1) < 0) __PYX_ERR(0, 128, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_category, __pyx_t_1) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":129
+  /* "hermes/factors/base.pyx":138
  *         data.name = name
  *         data.category = self.category
  *         data.id = self._create_id(name=name, **kwargs)             # <<<<<<<<<<<<<<
  *         return data
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_create_id_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_create_id_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 129, __pyx_L1_error)
-  __pyx_t_2 = __pyx_t_3;
-  __pyx_t_3 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 129, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
+  __pyx_t_3 = __pyx_t_5;
+  __pyx_t_5 = 0;
+  if (__Pyx_MergeKeywords(__pyx_t_3, __pyx_v_kwargs) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_id, __pyx_t_3) < 0) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_id, __pyx_t_5) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "hermes/factors/base.pyx":130
+  /* "hermes/factors/base.pyx":139
  *         data.category = self.category
  *         data.id = self._create_id(name=name, **kwargs)
  *         return data             # <<<<<<<<<<<<<<
  * 
  *     def factors_list(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_data);
   __pyx_r = __pyx_v_data;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":125
+  /* "hermes/factors/base.pyx":126
  *         return "{0}".format(create_id(original=s, digit=10))
  * 
  *     def _format(self, data, name, **kwargs):             # <<<<<<<<<<<<<<
- *         data = data.stack()
- *         data.name = name
+ *         #0 matrix  1 serise  2 DatFrame
+ *         data_format = 1 if not hasattr(self,'_data_format') else self._data_format
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("hermes.factors.base.FactorBase._format", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_data_format);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":132
+/* "hermes/factors/base.pyx":141
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
 
@@ -3224,15 +3364,15 @@
   __pyx_r = __pyx_pf_6hermes_7factors_4base_10FactorBase_12factors_list(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":135
+/* "hermes/factors/base.pyx":144
  *         return list(
  *             filter(
  *                 lambda x: not x.startswith('_')  and             # <<<<<<<<<<<<<<
  *                 callable(getattr(self, x)), dir(self)))
  */
 
 /* Python wrapper */
@@ -3263,66 +3403,66 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda", 0);
   __pyx_outer_scope = (struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list *) __Pyx_CyFunction_GetClosure(__pyx_self);
   __pyx_cur_scope = __pyx_outer_scope;
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_n_s_) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_s_);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 135, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_6 = (!__pyx_t_5);
   if (__pyx_t_6) {
   } else {
-    __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 135, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 144, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L3_bool_binop_done;
   }
 
-  /* "hermes/factors/base.pyx":136
+  /* "hermes/factors/base.pyx":145
  *             filter(
  *                 lambda x: not x.startswith('_')  and
  *                 callable(getattr(self, x)), dir(self)))             # <<<<<<<<<<<<<<
  */
-  if (unlikely(!__pyx_cur_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 136, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 145, __pyx_L1_error) }
   __pyx_t_2 = __pyx_cur_scope->__pyx_v_self;
   __Pyx_INCREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_GetAttr(__pyx_t_2, __pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetAttr(__pyx_t_2, __pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __Pyx_PyCallable_Check(__pyx_t_3); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyCallable_Check(__pyx_t_3); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_L3_bool_binop_done:;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":135
+  /* "hermes/factors/base.pyx":144
  *         return list(
  *             filter(
  *                 lambda x: not x.startswith('_')  and             # <<<<<<<<<<<<<<
  *                 callable(getattr(self, x)), dir(self)))
  */
 
   /* function exit code */
@@ -3335,15 +3475,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":132
+/* "hermes/factors/base.pyx":141
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
 
@@ -3358,85 +3498,85 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("factors_list", 0);
   __pyx_cur_scope = (struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list *)__pyx_tp_new_6hermes_7factors_4base___pyx_scope_struct__factors_list(__pyx_ptype_6hermes_7factors_4base___pyx_scope_struct__factors_list, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 132, __pyx_L1_error)
+    __PYX_ERR(0, 141, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_self);
 
-  /* "hermes/factors/base.pyx":133
+  /* "hermes/factors/base.pyx":142
  * 
  *     def factors_list(self):
  *         return list(             # <<<<<<<<<<<<<<
  *             filter(
  *                 lambda x: not x.startswith('_')  and
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "hermes/factors/base.pyx":135
+  /* "hermes/factors/base.pyx":144
  *         return list(
  *             filter(
  *                 lambda x: not x.startswith('_')  and             # <<<<<<<<<<<<<<
  *                 callable(getattr(self, x)), dir(self)))
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_12factors_list_lambda, 0, __pyx_n_s_FactorBase_factors_list_locals_l, ((PyObject*)__pyx_cur_scope), __pyx_n_s_hermes_factors_base, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_12factors_list_lambda, 0, __pyx_n_s_FactorBase_factors_list_locals_l, ((PyObject*)__pyx_cur_scope), __pyx_n_s_hermes_factors_base, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "hermes/factors/base.pyx":136
+  /* "hermes/factors/base.pyx":145
  *             filter(
  *                 lambda x: not x.startswith('_')  and
  *                 callable(getattr(self, x)), dir(self)))             # <<<<<<<<<<<<<<
  */
   __pyx_t_2 = __pyx_cur_scope->__pyx_v_self;
   __Pyx_INCREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_Dir(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_3 = PyObject_Dir(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "hermes/factors/base.pyx":134
+  /* "hermes/factors/base.pyx":143
  *     def factors_list(self):
  *         return list(
  *             filter(             # <<<<<<<<<<<<<<
  *                 lambda x: not x.startswith('_')  and
  *                 callable(getattr(self, x)), dir(self)))
  */
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_filter, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_filter, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "hermes/factors/base.pyx":133
+  /* "hermes/factors/base.pyx":142
  * 
  *     def factors_list(self):
  *         return list(             # <<<<<<<<<<<<<<
  *             filter(
  *                 lambda x: not x.startswith('_')  and
  */
-  __pyx_t_2 = PySequence_List(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_2 = PySequence_List(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":132
+  /* "hermes/factors/base.pyx":141
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
 
@@ -3647,14 +3787,16 @@
   {&__pyx_n_s_category, __pyx_k_category, sizeof(__pyx_k_category), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_columns, __pyx_k_columns, sizeof(__pyx_k_columns), 0, 0, 1, 1},
   {&__pyx_n_s_copy, __pyx_k_copy, sizeof(__pyx_k_copy), 0, 0, 1, 1},
   {&__pyx_n_s_create_id, __pyx_k_create_id, sizeof(__pyx_k_create_id), 0, 0, 1, 1},
   {&__pyx_n_s_create_id_2, __pyx_k_create_id_2, sizeof(__pyx_k_create_id_2), 0, 0, 1, 1},
   {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
+  {&__pyx_n_s_data_format, __pyx_k_data_format, sizeof(__pyx_k_data_format), 0, 0, 1, 1},
+  {&__pyx_n_s_data_format_2, __pyx_k_data_format_2, sizeof(__pyx_k_data_format_2), 0, 0, 1, 1},
   {&__pyx_n_s_ddb, __pyx_k_ddb, sizeof(__pyx_k_ddb), 0, 0, 1, 1},
   {&__pyx_n_s_deepcopy, __pyx_k_deepcopy, sizeof(__pyx_k_deepcopy), 0, 0, 1, 1},
   {&__pyx_n_s_default, __pyx_k_default, sizeof(__pyx_k_default), 0, 0, 1, 1},
   {&__pyx_n_s_dependencies, __pyx_k_dependencies, sizeof(__pyx_k_dependencies), 0, 0, 1, 1},
   {&__pyx_n_s_dependencies_list, __pyx_k_dependencies_list, sizeof(__pyx_k_dependencies_list), 0, 0, 1, 1},
   {&__pyx_n_s_digit, __pyx_k_digit, sizeof(__pyx_k_digit), 0, 0, 1, 1},
   {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
@@ -3701,29 +3843,31 @@
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
   {&__pyx_n_s_original, __pyx_k_original, sizeof(__pyx_k_original), 0, 0, 1, 1},
   {&__pyx_n_s_parameters, __pyx_k_parameters, sizeof(__pyx_k_parameters), 0, 0, 1, 1},
   {&__pyx_n_s_pdb, __pyx_k_pdb, sizeof(__pyx_k_pdb), 0, 0, 1, 1},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
   {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
+  {&__pyx_n_s_reset_index, __pyx_k_reset_index, sizeof(__pyx_k_reset_index), 0, 0, 1, 1},
   {&__pyx_n_s_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 0, 1, 1},
   {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
   {&__pyx_n_s_short, __pyx_k_short, sizeof(__pyx_k_short), 0, 0, 1, 1},
   {&__pyx_n_s_short_type_str, __pyx_k_short_type_str, sizeof(__pyx_k_short_type_str), 0, 0, 1, 1},
   {&__pyx_n_s_signature, __pyx_k_signature, sizeof(__pyx_k_signature), 0, 0, 1, 1},
   {&__pyx_n_s_six, __pyx_k_six, sizeof(__pyx_k_six), 0, 0, 1, 1},
   {&__pyx_n_s_stack, __pyx_k_stack, sizeof(__pyx_k_stack), 0, 0, 1, 1},
   {&__pyx_n_s_startswith, __pyx_k_startswith, sizeof(__pyx_k_startswith), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_kp_s_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 0, 1, 0},
+  {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
   {&__pyx_n_s_with_metaclass, __pyx_k_with_metaclass, sizeof(__pyx_k_with_metaclass), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_filter = __Pyx_GetBuiltinName(__pyx_n_s_filter); if (!__pyx_builtin_filter) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_builtin_filter = __Pyx_GetBuiltinName(__pyx_n_s_filter); if (!__pyx_builtin_filter) __PYX_ERR(0, 143, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -3833,96 +3977,98 @@
  *         self._init_self(**kwargs)
  */
   __pyx_tuple__18 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
   __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_init, 84, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 84, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":89
+  /* "hermes/factors/base.pyx":90
  * 
  *     @abstractmethod
  *     def _init_self(self, **kwargs):             # <<<<<<<<<<<<<<
  *         """"""
  *         pass
  */
-  __pyx_tuple__20 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_init_self, 89, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_init_self, 90, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 90, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":93
+  /* "hermes/factors/base.pyx":94
  *         pass
  * 
  *     def init_data(self, **kwargs):             # <<<<<<<<<<<<<<
  *         dependencies_list = self.get_dependencies()
  *         method = 'ddb' if 'method' not in kwargs else kwargs['method']
  */
-  __pyx_tuple__22 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_kwargs, __pyx_n_s_dependencies_list, __pyx_n_s_method, __pyx_n_s_data); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_kwargs, __pyx_n_s_dependencies_list, __pyx_n_s_method, __pyx_n_s_data); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_init_data, 93, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_init_data, 94, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 94, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":104
+  /* "hermes/factors/base.pyx":105
  * 
  * 
  *     def get_dependencies(self):             # <<<<<<<<<<<<<<
  *         dependencies_list = []
  *         member_func = self.factors_list()
  */
-  __pyx_tuple__24 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_dependencies_list, __pyx_n_s_member_func, __pyx_n_s_func, __pyx_n_s_func_module, __pyx_n_s_fun_param, __pyx_n_s_dependencies); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_dependencies_list, __pyx_n_s_member_func, __pyx_n_s_func, __pyx_n_s_func_module, __pyx_n_s_fun_param, __pyx_n_s_dependencies); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(1, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_get_dependencies, 104, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(1, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_get_dependencies, 105, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 105, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":118
+  /* "hermes/factors/base.pyx":119
  * 
  * 
  *     def _create_id(self, **kwargs):             # <<<<<<<<<<<<<<
  *         feature = copy.deepcopy(kwargs)
  *         feature['category'] = self.category
  */
-  __pyx_tuple__26 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_kwargs, __pyx_n_s_feature, __pyx_n_s_s); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_kwargs, __pyx_n_s_feature, __pyx_n_s_s); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_create_id_2, 118, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_create_id_2, 119, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 119, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":125
+  /* "hermes/factors/base.pyx":126
  *         return "{0}".format(create_id(original=s, digit=10))
  * 
  *     def _format(self, data, name, **kwargs):             # <<<<<<<<<<<<<<
- *         data = data.stack()
- *         data.name = name
+ *         #0 matrix  1 serise  2 DatFrame
+ *         data_format = 1 if not hasattr(self,'_data_format') else self._data_format
  */
-  __pyx_tuple__28 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_data, __pyx_n_s_name, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_data, __pyx_n_s_name, __pyx_n_s_kwargs, __pyx_n_s_data_format_2); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_format_2, 125, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_format_2, 126, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 126, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":132
+  /* "hermes/factors/base.pyx":141
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
-  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__30);
   __Pyx_GIVEREF(__pyx_tuple__30);
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_factors_list, 132, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_factors_list, 141, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 141, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_float_1_0 = PyFloat_FromDouble(1.0); if (unlikely(!__pyx_float_1_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_neg_1_0 = PyFloat_FromDouble(-1.0); if (unlikely(!__pyx_float_neg_1_0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_10 = PyInt_FromLong(10); if (unlikely(!__pyx_int_10)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -3960,15 +4106,15 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list.tp_dictoffset && __pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_6hermes_7factors_4base___pyx_scope_struct__factors_list = &__pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list;
@@ -4893,110 +5039,110 @@
  *         self._init_self(**kwargs)
  */
   __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_1__init__, 0, __pyx_n_s_FactorBase___init, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":88
- *         self._init_self(**kwargs)
+  /* "hermes/factors/base.pyx":89
+ * 
  * 
  *     @abstractmethod             # <<<<<<<<<<<<<<
  *     def _init_self(self, **kwargs):
  *         """"""
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_abstractmethod); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_abstractmethod); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "hermes/factors/base.pyx":89
+  /* "hermes/factors/base.pyx":90
  * 
  *     @abstractmethod
  *     def _init_self(self, **kwargs):             # <<<<<<<<<<<<<<
  *         """"""
  *         pass
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_3_init_self, 0, __pyx_n_s_FactorBase__init_self, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_3_init_self, 0, __pyx_n_s_FactorBase__init_self, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_7, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_init_self, __pyx_t_4) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_init_self, __pyx_t_4) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":93
+  /* "hermes/factors/base.pyx":94
  *         pass
  * 
  *     def init_data(self, **kwargs):             # <<<<<<<<<<<<<<
  *         dependencies_list = self.get_dependencies()
  *         method = 'ddb' if 'method' not in kwargs else kwargs['method']
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_5init_data, 0, __pyx_n_s_FactorBase_init_data, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_5init_data, 0, __pyx_n_s_FactorBase_init_data, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_init_data, __pyx_t_4) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_init_data, __pyx_t_4) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":104
+  /* "hermes/factors/base.pyx":105
  * 
  * 
  *     def get_dependencies(self):             # <<<<<<<<<<<<<<
  *         dependencies_list = []
  *         member_func = self.factors_list()
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_7get_dependencies, 0, __pyx_n_s_FactorBase_get_dependencies, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_7get_dependencies, 0, __pyx_n_s_FactorBase_get_dependencies, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_get_dependencies, __pyx_t_4) < 0) __PYX_ERR(0, 104, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_get_dependencies, __pyx_t_4) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":118
+  /* "hermes/factors/base.pyx":119
  * 
  * 
  *     def _create_id(self, **kwargs):             # <<<<<<<<<<<<<<
  *         feature = copy.deepcopy(kwargs)
  *         feature['category'] = self.category
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_9_create_id, 0, __pyx_n_s_FactorBase__create_id, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_9_create_id, 0, __pyx_n_s_FactorBase__create_id, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_create_id_2, __pyx_t_4) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_create_id_2, __pyx_t_4) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":125
+  /* "hermes/factors/base.pyx":126
  *         return "{0}".format(create_id(original=s, digit=10))
  * 
  *     def _format(self, data, name, **kwargs):             # <<<<<<<<<<<<<<
- *         data = data.stack()
- *         data.name = name
+ *         #0 matrix  1 serise  2 DatFrame
+ *         data_format = 1 if not hasattr(self,'_data_format') else self._data_format
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_11_format, 0, __pyx_n_s_FactorBase__format, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_11_format, 0, __pyx_n_s_FactorBase__format, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_format_2, __pyx_t_4) < 0) __PYX_ERR(0, 125, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_format_2, __pyx_t_4) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":132
+  /* "hermes/factors/base.pyx":141
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_13factors_list, 0, __pyx_n_s_FactorBase_factors_list, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_13factors_list, 0, __pyx_n_s_FactorBase_factors_list, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_factors_list, __pyx_t_4) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_factors_list, __pyx_t_4) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "hermes/factors/base.pyx":82
  * 
  * 
  * class FactorBase(six.with_metaclass(ABCMeta, ParamBase)):             # <<<<<<<<<<<<<<
  * 
@@ -5605,14 +5751,99 @@
     result = __Pyx_PyObject_Call(function, args, NULL);
     Py_DECREF(args);
     Py_DECREF(function);
 done:
     return result;
 }
 
+/* HasAttr */
+static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
+    PyObject *r;
+    if (unlikely(!__Pyx_PyBaseString_Check(n))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "hasattr(): attribute name must be string");
+        return -1;
+    }
+    r = __Pyx_GetAttr(o, n);
+    if (unlikely(!r)) {
+        PyErr_Clear();
+        return 0;
+    } else {
+        Py_DECREF(r);
+        return 1;
+    }
+}
+
+/* PyIntCompare */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, CYTHON_UNUSED long inplace) {
+    if (op1 == op2) {
+        Py_RETURN_TRUE;
+    }
+    #if PY_MAJOR_VERSION < 3
+    if (likely(PyInt_CheckExact(op1))) {
+        const long b = intval;
+        long a = PyInt_AS_LONG(op1);
+        if (a == b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+    }
+    #endif
+    #if CYTHON_USE_PYLONG_INTERNALS
+    if (likely(PyLong_CheckExact(op1))) {
+        int unequal;
+        unsigned long uintval;
+        Py_ssize_t size = Py_SIZE(op1);
+        const digit* digits = ((PyLongObject*)op1)->ob_digit;
+        if (intval == 0) {
+            if (size == 0) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+        } else if (intval < 0) {
+            if (size >= 0)
+                Py_RETURN_FALSE;
+            intval = -intval;
+            size = -size;
+        } else {
+            if (size <= 0)
+                Py_RETURN_FALSE;
+        }
+        uintval = (unsigned long) intval;
+#if PyLong_SHIFT * 4 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 4)) {
+            unequal = (size != 5) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[3] != ((uintval >> (3 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[4] != ((uintval >> (4 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+#if PyLong_SHIFT * 3 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 3)) {
+            unequal = (size != 4) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[3] != ((uintval >> (3 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+#if PyLong_SHIFT * 2 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 2)) {
+            unequal = (size != 3) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+#if PyLong_SHIFT * 1 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 1)) {
+            unequal = (size != 2) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+            unequal = (size != 1) || (((unsigned long) digits[0]) != (uintval & (unsigned long) PyLong_MASK));
+        if (unequal == 0) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+    }
+    #endif
+    if (PyFloat_CheckExact(op1)) {
+        const long b = intval;
+        double a = PyFloat_AS_DOUBLE(op1);
+        if ((double)a == (double)b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+    }
+    return (
+        PyObject_RichCompare(op1, op2, Py_EQ));
+}
+
 /* PyObjectSetAttrStr */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value) {
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_setattro))
         return tp->tp_setattro(obj, attr_name, value);
 #if PY_MAJOR_VERSION < 3
```

### Comparing `Finance-Hermes-0.2.8/hermes/factors/base.pyx` & `Finance-Hermes-0.2.9/hermes/factors/base.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 
 
 class FactorBase(six.with_metaclass(ABCMeta, ParamBase)):
 
     def __init__(self, **kwargs):
         # 子类继续完成自有的构造
         self._init_self(**kwargs)
+        
 
     @abstractmethod
     def _init_self(self, **kwargs):
         """子类因子针对可扩展参数的初始化"""
         pass
 
     def init_data(self, **kwargs):
@@ -119,15 +120,23 @@
         feature = copy.deepcopy(kwargs)
         feature['category'] = self.category
         s = hashlib.md5(
             json.dumps(feature).encode(encoding="utf-8")).hexdigest()
         return "{0}".format(create_id(original=s, digit=10))
 
     def _format(self, data, name, **kwargs):
-        data = data.stack()
+        #0 matrix  1 serise  2 DatFrame
+        data_format = 1 if not hasattr(self,'_data_format') else self._data_format
+        if data_format == 1 or data_format == 2:
+            data = data.stack()
+            if data_format == 2:
+                data.name = 'value'
+                data = data.reset_index()
+                data['name'] = name
+                
         data.name = name
         data.category = self.category
         data.id = self._create_id(name=name, **kwargs)
         return data
 
     def factors_list(self):
         return list(
```

### Comparing `Finance-Hermes-0.2.8/hermes/kdutils/base.c` & `Finance-Hermes-0.2.9/hermes/kdutils/base.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.8/hermes/kdutils/base.pyx` & `Finance-Hermes-0.2.9/hermes/kdutils/base.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.8/hermes/kdutils/core/fixes.c` & `Finance-Hermes-0.2.9/hermes/kdutils/core/fixes.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.8/hermes/kdutils/core/fixes.pyx` & `Finance-Hermes-0.2.9/hermes/kdutils/core/fixes.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.8/hermes/kdutils/core/helper.c` & `Finance-Hermes-0.2.9/hermes/kdutils/core/helper.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.8/hermes/kdutils/core/helper.pyx` & `Finance-Hermes-0.2.9/hermes/kdutils/core/helper.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.8/hermes/kdutils/create_id.c` & `Finance-Hermes-0.2.9/hermes/kdutils/create_id.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.8/hermes/kdutils/create_id.pyx` & `Finance-Hermes-0.2.9/hermes/kdutils/create_id.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.8/hermes/kdutils/lazy.c` & `Finance-Hermes-0.2.9/hermes/kdutils/lazy.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.8/hermes/kdutils/lazy.pyx` & `Finance-Hermes-0.2.9/hermes/kdutils/lazy.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.8/hermes/lzador/calculater.c` & `Finance-Hermes-0.2.9/hermes/lzador/calculater.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.8/hermes/lzador/calculater.pyx` & `Finance-Hermes-0.2.9/hermes/lzador/calculater.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.8/setup.py` & `Finance-Hermes-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,16 +69,16 @@
     import multiprocessing
     n_cpu = multiprocessing.cpu_count()
 else:
     n_cpu = 0
     
 
 
-ext_modules = ['hermes/kdutils/core/fixes.pyx','hermes/kdutils/core/helper.pyx','hermes/factors/base.pyx','hermes/kdutils/base.pyx','hermes/kdutils/create_id.pyx','hermes/kdutils/lazy.pyx',
-               'hermes/lzador/calculater.pyx']
+ext_modules = ['hermes/kdutils/core/fixes.pyx','hermes/kdutils/core/helper.pyx','hermes/factors/base.pyx', 'hermes/kdutils/base.pyx','hermes/kdutils/create_id.pyx','hermes/kdutils/lazy.pyx',
+               'hermes/lzador/calculater.pyx','hermes/factors/test/factor_test.pyx']
 
 def generate_extensions(ext_modules, line_trace=True):
 
     extensions = []
 
     if line_trace:
         print("define cython trace to True ...")
```

