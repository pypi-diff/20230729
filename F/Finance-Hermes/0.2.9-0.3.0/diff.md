# Comparing `tmp/Finance-Hermes-0.2.9.tar.gz` & `tmp/Finance-Hermes-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Finance-Hermes-0.2.9.tar", last modified: Sat Jul 29 02:01:44 2023, max compression
+gzip compressed data, was "dist/Finance-Hermes-0.3.0.tar", last modified: Sat Jul 29 06:12:45 2023, max compression
```

## Comparing `Finance-Hermes-0.2.9.tar` & `Finance-Hermes-0.3.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/Finance_Hermes.egg-info/
--rw-r--r--   0 root         (0) root         (0)      233 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/Finance_Hermes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      829 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/Finance_Hermes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/Finance_Hermes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/Finance_Hermes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/Finance_Hermes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    11357 2022-11-01 07:48:09.000000 Finance-Hermes-0.2.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      358 2023-07-29 01:53:47.000000 Finance-Hermes-0.2.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      233 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      195 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-29 01:59:31.000000 Finance-Hermes-0.2.9/hermes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/factors/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.9/hermes/factors/__init__.py
--rw-r--r--   0 root         (0) root         (0)   339663 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/factors/base.c
--rw-r--r--   0 root         (0) root         (0)     4469 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/hermes/factors/base.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/factors/test/
--rw-r--r--   0 root         (0) root         (0)   241630 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/factors/test/factor_test.c
--rw-r--r--   0 root         (0) root         (0)     2056 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/hermes/factors/test/factor_test.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/kdutils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.9/hermes/kdutils/__init__.py
--rw-r--r--   0 root         (0) root         (0)   271147 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/kdutils/base.c
--rw-r--r--   0 root         (0) root         (0)     2338 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/hermes/kdutils/base.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/kdutils/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.9/hermes/kdutils/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)   678491 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/kdutils/core/fixes.c
--rw-r--r--   0 root         (0) root         (0)     9714 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/hermes/kdutils/core/fixes.pyx
--rw-r--r--   0 root         (0) root         (0)   392670 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/kdutils/core/helper.c
--rw-r--r--   0 root         (0) root         (0)     7825 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/hermes/kdutils/core/helper.pyx
--rw-r--r--   0 root         (0) root         (0)   190192 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/kdutils/create_id.c
--rw-r--r--   0 root         (0) root         (0)      870 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/hermes/kdutils/create_id.pyx
--rw-r--r--   0 root         (0) root         (0)   235985 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/kdutils/lazy.c
--rw-r--r--   0 root         (0) root         (0)     1578 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/hermes/kdutils/lazy.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/lzador/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/hermes/lzador/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161732 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/hermes/lzador/calculater.c
--rw-r--r--   0 root         (0) root         (0)      657 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/hermes/lzador/calculater.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/requirements/
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-29 01:51:21.000000 Finance-Hermes-0.2.9/requirements/py3.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 02:01:44.000000 Finance-Hermes-0.2.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3331 2023-07-29 01:55:31.000000 Finance-Hermes-0.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/Finance_Hermes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      233 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/Finance_Hermes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      829 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/Finance_Hermes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/Finance_Hermes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/Finance_Hermes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/Finance_Hermes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-11-01 07:48:09.000000 Finance-Hermes-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      358 2023-07-29 01:53:47.000000 Finance-Hermes-0.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      233 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      195 2022-11-06 15:36:04.000000 Finance-Hermes-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/hermes/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-29 06:12:04.000000 Finance-Hermes-0.3.0/hermes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/hermes/factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.3.0/hermes/factors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   339800 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/hermes/factors/base.c
+-rw-r--r--   0 root         (0) root         (0)     4452 2023-07-29 02:06:34.000000 Finance-Hermes-0.3.0/hermes/factors/base.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/hermes/factors/test/
+-rw-r--r--   0 root         (0) root         (0)   241941 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/hermes/factors/test/factor_test.c
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-07-29 06:11:05.000000 Finance-Hermes-0.3.0/hermes/factors/test/factor_test.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/hermes/kdutils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.3.0/hermes/kdutils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   271147 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.0/hermes/kdutils/base.c
+-rw-r--r--   0 root         (0) root         (0)     2338 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.0/hermes/kdutils/base.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/hermes/kdutils/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.3.0/hermes/kdutils/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   678491 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.0/hermes/kdutils/core/fixes.c
+-rw-r--r--   0 root         (0) root         (0)     9714 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.0/hermes/kdutils/core/fixes.pyx
+-rw-r--r--   0 root         (0) root         (0)   392670 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.0/hermes/kdutils/core/helper.c
+-rw-r--r--   0 root         (0) root         (0)     7825 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.0/hermes/kdutils/core/helper.pyx
+-rw-r--r--   0 root         (0) root         (0)   190192 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.0/hermes/kdutils/create_id.c
+-rw-r--r--   0 root         (0) root         (0)      870 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.0/hermes/kdutils/create_id.pyx
+-rw-r--r--   0 root         (0) root         (0)   235985 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.0/hermes/kdutils/lazy.c
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.0/hermes/kdutils/lazy.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/hermes/lzador/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.0/hermes/lzador/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161732 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.0/hermes/lzador/calculater.c
+-rw-r--r--   0 root         (0) root         (0)      657 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.0/hermes/lzador/calculater.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/requirements/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.0/requirements/py3.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3331 2023-07-29 01:55:31.000000 Finance-Hermes-0.3.0/setup.py
```

### Comparing `Finance-Hermes-0.2.9/Finance_Hermes.egg-info/SOURCES.txt` & `Finance-Hermes-0.3.0/Finance_Hermes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.9/LICENSE` & `Finance-Hermes-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.9/hermes/factors/base.c` & `Finance-Hermes-0.3.0/hermes/factors/base.c`

 * *Files 0% similar despite different names*

```diff
@@ -827,15 +827,15 @@
 static const char *__pyx_f[] = {
   "hermes/factors/base.pyx",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list;
 
-/* "hermes/factors/base.pyx":141
+/* "hermes/factors/base.pyx":140
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
 struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list {
@@ -3214,15 +3214,15 @@
       if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_name, __pyx_n_s_value) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
 
       /* "hermes/factors/base.pyx":133
  *             if data_format == 2:
  *                 data.name = 'value'
  *                 data = data.reset_index()             # <<<<<<<<<<<<<<
  *                 data['name'] = name
- * 
+ *         data.name = name
  */
       __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_5 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_5)) {
@@ -3240,16 +3240,16 @@
       __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_1);
       __pyx_t_1 = 0;
 
       /* "hermes/factors/base.pyx":134
  *                 data.name = 'value'
  *                 data = data.reset_index()
  *                 data['name'] = name             # <<<<<<<<<<<<<<
- * 
  *         data.name = name
+ *         data.category = self.category
  */
       if (unlikely(PyObject_SetItem(__pyx_v_data, __pyx_n_s_name, __pyx_v_name) < 0)) __PYX_ERR(0, 134, __pyx_L1_error)
 
       /* "hermes/factors/base.pyx":131
  *         if data_format == 1 or data_format == 2:
  *             data = data.stack()
  *             if data_format == 2:             # <<<<<<<<<<<<<<
@@ -3263,58 +3263,58 @@
  *         data_format = 1 if not hasattr(self,'_data_format') else self._data_format
  *         if data_format == 1 or data_format == 2:             # <<<<<<<<<<<<<<
  *             data = data.stack()
  *             if data_format == 2:
  */
   }
 
-  /* "hermes/factors/base.pyx":136
+  /* "hermes/factors/base.pyx":135
+ *                 data = data.reset_index()
  *                 data['name'] = name
- * 
  *         data.name = name             # <<<<<<<<<<<<<<
  *         data.category = self.category
  *         data.id = self._create_id(name=name, **kwargs)
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":137
- * 
+  /* "hermes/factors/base.pyx":136
+ *                 data['name'] = name
  *         data.name = name
  *         data.category = self.category             # <<<<<<<<<<<<<<
  *         data.id = self._create_id(name=name, **kwargs)
  *         return data
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_category); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_category); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_category, __pyx_t_1) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_category, __pyx_t_1) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":138
+  /* "hermes/factors/base.pyx":137
  *         data.name = name
  *         data.category = self.category
  *         data.id = self._create_id(name=name, **kwargs)             # <<<<<<<<<<<<<<
  *         return data
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_create_id_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_create_id_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
   __pyx_t_3 = __pyx_t_5;
   __pyx_t_5 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_3, __pyx_v_kwargs) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 138, __pyx_L1_error)
+  if (__Pyx_MergeKeywords(__pyx_t_3, __pyx_v_kwargs) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_id, __pyx_t_5) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_id, __pyx_t_5) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "hermes/factors/base.pyx":139
+  /* "hermes/factors/base.pyx":138
  *         data.category = self.category
  *         data.id = self._create_id(name=name, **kwargs)
  *         return data             # <<<<<<<<<<<<<<
  * 
  *     def factors_list(self):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -3341,15 +3341,15 @@
   __Pyx_XDECREF(__pyx_v_data_format);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":141
+/* "hermes/factors/base.pyx":140
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
 
@@ -3364,15 +3364,15 @@
   __pyx_r = __pyx_pf_6hermes_7factors_4base_10FactorBase_12factors_list(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":144
+/* "hermes/factors/base.pyx":143
  *         return list(
  *             filter(
  *                 lambda x: not x.startswith('_')  and             # <<<<<<<<<<<<<<
  *                 callable(getattr(self, x)), dir(self)))
  */
 
 /* Python wrapper */
@@ -3403,66 +3403,66 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda", 0);
   __pyx_outer_scope = (struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list *) __Pyx_CyFunction_GetClosure(__pyx_self);
   __pyx_cur_scope = __pyx_outer_scope;
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
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
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 144, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_6 = (!__pyx_t_5);
   if (__pyx_t_6) {
   } else {
-    __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 144, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L3_bool_binop_done;
   }
 
-  /* "hermes/factors/base.pyx":145
+  /* "hermes/factors/base.pyx":144
  *             filter(
  *                 lambda x: not x.startswith('_')  and
  *                 callable(getattr(self, x)), dir(self)))             # <<<<<<<<<<<<<<
  */
-  if (unlikely(!__pyx_cur_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 145, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 144, __pyx_L1_error) }
   __pyx_t_2 = __pyx_cur_scope->__pyx_v_self;
   __Pyx_INCREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_GetAttr(__pyx_t_2, __pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetAttr(__pyx_t_2, __pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __Pyx_PyCallable_Check(__pyx_t_3); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 145, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyCallable_Check(__pyx_t_3); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_L3_bool_binop_done:;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":144
+  /* "hermes/factors/base.pyx":143
  *         return list(
  *             filter(
  *                 lambda x: not x.startswith('_')  and             # <<<<<<<<<<<<<<
  *                 callable(getattr(self, x)), dir(self)))
  */
 
   /* function exit code */
@@ -3475,15 +3475,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":141
+/* "hermes/factors/base.pyx":140
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
 
@@ -3498,85 +3498,85 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("factors_list", 0);
   __pyx_cur_scope = (struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list *)__pyx_tp_new_6hermes_7factors_4base___pyx_scope_struct__factors_list(__pyx_ptype_6hermes_7factors_4base___pyx_scope_struct__factors_list, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 141, __pyx_L1_error)
+    __PYX_ERR(0, 140, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_self);
 
-  /* "hermes/factors/base.pyx":142
+  /* "hermes/factors/base.pyx":141
  * 
  *     def factors_list(self):
  *         return list(             # <<<<<<<<<<<<<<
  *             filter(
  *                 lambda x: not x.startswith('_')  and
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "hermes/factors/base.pyx":144
+  /* "hermes/factors/base.pyx":143
  *         return list(
  *             filter(
  *                 lambda x: not x.startswith('_')  and             # <<<<<<<<<<<<<<
  *                 callable(getattr(self, x)), dir(self)))
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_12factors_list_lambda, 0, __pyx_n_s_FactorBase_factors_list_locals_l, ((PyObject*)__pyx_cur_scope), __pyx_n_s_hermes_factors_base, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_12factors_list_lambda, 0, __pyx_n_s_FactorBase_factors_list_locals_l, ((PyObject*)__pyx_cur_scope), __pyx_n_s_hermes_factors_base, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "hermes/factors/base.pyx":145
+  /* "hermes/factors/base.pyx":144
  *             filter(
  *                 lambda x: not x.startswith('_')  and
  *                 callable(getattr(self, x)), dir(self)))             # <<<<<<<<<<<<<<
  */
   __pyx_t_2 = __pyx_cur_scope->__pyx_v_self;
   __Pyx_INCREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_Dir(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L1_error)
+  __pyx_t_3 = PyObject_Dir(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "hermes/factors/base.pyx":143
+  /* "hermes/factors/base.pyx":142
  *     def factors_list(self):
  *         return list(
  *             filter(             # <<<<<<<<<<<<<<
  *                 lambda x: not x.startswith('_')  and
  *                 callable(getattr(self, x)), dir(self)))
  */
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_filter, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_filter, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "hermes/factors/base.pyx":142
+  /* "hermes/factors/base.pyx":141
  * 
  *     def factors_list(self):
  *         return list(             # <<<<<<<<<<<<<<
  *             filter(
  *                 lambda x: not x.startswith('_')  and
  */
-  __pyx_t_2 = PySequence_List(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_t_2 = PySequence_List(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":141
+  /* "hermes/factors/base.pyx":140
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
 
@@ -3859,15 +3859,15 @@
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_kp_s_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 0, 1, 0},
   {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
   {&__pyx_n_s_with_metaclass, __pyx_k_with_metaclass, sizeof(__pyx_k_with_metaclass), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_filter = __Pyx_GetBuiltinName(__pyx_n_s_filter); if (!__pyx_builtin_filter) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_builtin_filter = __Pyx_GetBuiltinName(__pyx_n_s_filter); if (!__pyx_builtin_filter) __PYX_ERR(0, 142, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -4037,25 +4037,25 @@
  *         data_format = 1 if not hasattr(self,'_data_format') else self._data_format
  */
   __pyx_tuple__28 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_data, __pyx_n_s_name, __pyx_n_s_kwargs, __pyx_n_s_data_format_2); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
   __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_format_2, 126, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 126, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":141
+  /* "hermes/factors/base.pyx":140
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
-  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 141, __pyx_L1_error)
+  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 140, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__30);
   __Pyx_GIVEREF(__pyx_tuple__30);
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_factors_list, 141, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 141, __pyx_L1_error)
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_factors_list, 140, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 140, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -4106,15 +4106,15 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list.tp_dictoffset && __pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_6hermes_7factors_4base___pyx_scope_struct__factors_list = &__pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list;
@@ -5125,24 +5125,24 @@
  *         data_format = 1 if not hasattr(self,'_data_format') else self._data_format
  */
   __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_11_format, 0, __pyx_n_s_FactorBase__format, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_format_2, __pyx_t_4) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":141
+  /* "hermes/factors/base.pyx":140
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_13factors_list, 0, __pyx_n_s_FactorBase_factors_list, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 141, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_13factors_list, 0, __pyx_n_s_FactorBase_factors_list, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 140, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_factors_list, __pyx_t_4) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_factors_list, __pyx_t_4) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "hermes/factors/base.pyx":82
  * 
  * 
  * class FactorBase(six.with_metaclass(ABCMeta, ParamBase)):             # <<<<<<<<<<<<<<
  *
```

### Comparing `Finance-Hermes-0.2.9/hermes/factors/base.pyx` & `Finance-Hermes-0.3.0/hermes/factors/base.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,14 @@
         data_format = 1 if not hasattr(self,'_data_format') else self._data_format
         if data_format == 1 or data_format == 2:
             data = data.stack()
             if data_format == 2:
                 data.name = 'value'
                 data = data.reset_index()
                 data['name'] = name
-                
         data.name = name
         data.category = self.category
         data.id = self._create_id(name=name, **kwargs)
         return data
 
     def factors_list(self):
         return list(
```

### Comparing `Finance-Hermes-0.2.9/hermes/factors/test/factor_test.c` & `Finance-Hermes-0.3.0/hermes/factors/test/factor_test.c`

 * *Files 4% similar despite different names*

```diff
@@ -905,26 +905,26 @@
 #define __Pyx_DECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_DECREF(tmp);\
     } while (0)
 #define __Pyx_CLEAR(r)    do { PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);} while(0)
 #define __Pyx_XCLEAR(r)   do { if((r) != NULL) {PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);}} while(0)
 
+/* RaiseArgTupleInvalid.proto */
+static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
+    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
+
 /* RaiseDoubleKeywords.proto */
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
 static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
-/* RaiseArgTupleInvalid.proto */
-static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
-    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
-
 /* PyObjectSetAttrStr.proto */
 #if CYTHON_USE_TYPE_SLOTS
 #define __Pyx_PyObject_DelAttrStr(o,n) __Pyx_PyObject_SetAttrStr(o, n, NULL)
 static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value);
 #else
 #define __Pyx_PyObject_DelAttrStr(o,n)   PyObject_DelAttr(o,n)
 #define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
@@ -1277,19 +1277,21 @@
 static const char __pyx_k_init_self[] = "_init_self";
 static const char __pyx_k_metaclass[] = "__metaclass__";
 static const char __pyx_k_openPrice[] = "openPrice";
 static const char __pyx_k_FactorBase[] = "FactorBase";
 static const char __pyx_k_FactorTest[] = "FactorTest";
 static const char __pyx_k_closePrice[] = "closePrice";
 static const char __pyx_k_dy_q_ti_se[] = "dy_q_ti_se";
+static const char __pyx_k_data_format[] = "data_format";
 static const char __pyx_k_factor_test[] = "factor_test";
 static const char __pyx_k_marketValue[] = "marketValue";
 static const char __pyx_k_turnoverVol[] = "turnoverVol";
 static const char __pyx_k_dependencies[] = "dependencies";
 static const char __pyx_k_LongCallMixin[] = "LongCallMixin";
+static const char __pyx_k_data_format_2[] = "_data_format";
 static const char __pyx_k_ShortCallMixin[] = "ShortCallMixin";
 static const char __pyx_k_negMarketValue[] = "negMarketValue";
 static const char __pyx_k_totalshares_se[] = "totalshares_se";
 static const char __pyx_k_FactorTest_test1[] = "FactorTest.test1";
 static const char __pyx_k_FactorTest_test2[] = "FactorTest.test2";
 static const char __pyx_k_FactorTest_test3[] = "FactorTest.test3";
 static const char __pyx_k_FactorTest___init[] = "FactorTest.__init__";
@@ -1311,14 +1313,16 @@
 static PyObject *__pyx_n_s_ShortCallMixin;
 static PyObject *__pyx_n_s_category;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_closePrice;
 static PyObject *__pyx_n_s_close_se;
 static PyObject *__pyx_n_s_data;
 static PyObject *__pyx_n_s_data_2;
+static PyObject *__pyx_n_s_data_format;
+static PyObject *__pyx_n_s_data_format_2;
 static PyObject *__pyx_n_s_dependencies;
 static PyObject *__pyx_n_s_doc;
 static PyObject *__pyx_n_s_dy_q_evebitda_caldr_se;
 static PyObject *__pyx_n_s_dy_q_ti_se;
 static PyObject *__pyx_n_s_end_date;
 static PyObject *__pyx_n_s_factor1;
 static PyObject *__pyx_n_s_factor2;
@@ -1356,15 +1360,15 @@
 static PyObject *__pyx_n_s_test1;
 static PyObject *__pyx_n_s_test2;
 static PyObject *__pyx_n_s_test3;
 static PyObject *__pyx_n_s_test_2;
 static PyObject *__pyx_n_s_totalshares_se;
 static PyObject *__pyx_n_s_turnoverVol;
 static PyObject *__pyx_n_s_vwap;
-static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_kwargs); /* proto */
+static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data_format, PyObject *__pyx_v_kwargs); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_2_init_self(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test___defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_4test1(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data, CYTHON_UNUSED PyObject *__pyx_v_dependencies); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_2__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_6test2(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data, CYTHON_UNUSED PyObject *__pyx_v_dependencies); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_4__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_8test3(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data, CYTHON_UNUSED PyObject *__pyx_v_dependencies); /* proto */
@@ -1378,150 +1382,170 @@
 static PyObject *__pyx_codeobj__3;
 static PyObject *__pyx_codeobj__5;
 static PyObject *__pyx_codeobj__7;
 static PyObject *__pyx_codeobj__9;
 static PyObject *__pyx_codeobj__11;
 /* Late includes */
 
-/* "hermes/factors/test/factor_test.pyx":8
- * 
+/* "hermes/factors/test/factor_test.pyx":9
  * class FactorTest(FactorBase, LongCallMixin, ShortCallMixin):
- *     def __init__(self, **kwargs):             # <<<<<<<<<<<<<<
+ * 
+ *     def __init__(self, data_format, **kwargs):             # <<<<<<<<<<<<<<
  *         __str__ = 'factor_test'
  *         self.category = 'test'
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6hermes_7factors_4test_11factor_test_10FactorTest_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6hermes_7factors_4test_11factor_test_10FactorTest___init__[] = "FactorTest.__init__(self, **kwargs)";
+static char __pyx_doc_6hermes_7factors_4test_11factor_test_10FactorTest___init__[] = "FactorTest.__init__(self, data_format, **kwargs)";
 static PyMethodDef __pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6hermes_7factors_4test_11factor_test_10FactorTest_1__init__, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6hermes_7factors_4test_11factor_test_10FactorTest___init__};
 static PyObject *__pyx_pw_6hermes_7factors_4test_11factor_test_10FactorTest_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
+  PyObject *__pyx_v_data_format = 0;
   PyObject *__pyx_v_kwargs = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   __pyx_v_kwargs = PyDict_New(); if (unlikely(!__pyx_v_kwargs)) return NULL;
   __Pyx_GOTREF(__pyx_v_kwargs);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,0};
-    PyObject* values[1] = {0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_data_format,0};
+    PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data_format)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 9, __pyx_L3_error)
+        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 8, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 9, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
+    __pyx_v_data_format = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 8, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 9, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("hermes.factors.test.factor_test.FactorTest.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest___init__(__pyx_self, __pyx_v_self, __pyx_v_kwargs);
+  __pyx_r = __pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest___init__(__pyx_self, __pyx_v_self, __pyx_v_data_format, __pyx_v_kwargs);
 
   /* function exit code */
   __Pyx_XDECREF(__pyx_v_kwargs);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_kwargs) {
+static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data_format, PyObject *__pyx_v_kwargs) {
   CYTHON_UNUSED PyObject *__pyx_v___str__ = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "hermes/factors/test/factor_test.pyx":9
- * class FactorTest(FactorBase, LongCallMixin, ShortCallMixin):
- *     def __init__(self, **kwargs):
+  /* "hermes/factors/test/factor_test.pyx":10
+ * 
+ *     def __init__(self, data_format, **kwargs):
  *         __str__ = 'factor_test'             # <<<<<<<<<<<<<<
  *         self.category = 'test'
  *         self.name = ''
  */
   __Pyx_INCREF(__pyx_n_s_factor_test);
   __pyx_v___str__ = __pyx_n_s_factor_test;
 
-  /* "hermes/factors/test/factor_test.pyx":10
- *     def __init__(self, **kwargs):
+  /* "hermes/factors/test/factor_test.pyx":11
+ *     def __init__(self, data_format, **kwargs):
  *         __str__ = 'factor_test'
  *         self.category = 'test'             # <<<<<<<<<<<<<<
  *         self.name = ''
- *         self._data = self.init_data(**kwargs) if 'end_date' in kwargs else None
+ *         self._data_format = data_format
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_category, __pyx_n_s_test) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_category, __pyx_n_s_test) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
 
-  /* "hermes/factors/test/factor_test.pyx":11
+  /* "hermes/factors/test/factor_test.pyx":12
  *         __str__ = 'factor_test'
  *         self.category = 'test'
  *         self.name = ''             # <<<<<<<<<<<<<<
+ *         self._data_format = data_format
  *         self._data = self.init_data(**kwargs) if 'end_date' in kwargs else None
- * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_name, __pyx_kp_s_) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_name, __pyx_kp_s_) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
 
-  /* "hermes/factors/test/factor_test.pyx":12
+  /* "hermes/factors/test/factor_test.pyx":13
  *         self.category = 'test'
  *         self.name = ''
+ *         self._data_format = data_format             # <<<<<<<<<<<<<<
+ *         self._data = self.init_data(**kwargs) if 'end_date' in kwargs else None
+ * 
+ */
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_data_format_2, __pyx_v_data_format) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
+
+  /* "hermes/factors/test/factor_test.pyx":14
+ *         self.name = ''
+ *         self._data_format = data_format
  *         self._data = self.init_data(**kwargs) if 'end_date' in kwargs else None             # <<<<<<<<<<<<<<
  * 
  *     def _init_self(self, **kwargs):
  */
-  __pyx_t_2 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_end_date, __pyx_v_kwargs, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_end_date, __pyx_v_kwargs, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 14, __pyx_L1_error)
   if ((__pyx_t_2 != 0)) {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 12, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_v_kwargs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 12, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_v_kwargs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_1 = __pyx_t_4;
     __pyx_t_4 = 0;
   } else {
     __Pyx_INCREF(Py_None);
     __pyx_t_1 = Py_None;
   }
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_data, __pyx_t_1) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_data, __pyx_t_1) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":8
- * 
+  /* "hermes/factors/test/factor_test.pyx":9
  * class FactorTest(FactorBase, LongCallMixin, ShortCallMixin):
- *     def __init__(self, **kwargs):             # <<<<<<<<<<<<<<
+ * 
+ *     def __init__(self, data_format, **kwargs):             # <<<<<<<<<<<<<<
  *         __str__ = 'factor_test'
  *         self.category = 'test'
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
@@ -1534,15 +1558,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___str__);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/test/factor_test.pyx":14
+/* "hermes/factors/test/factor_test.pyx":16
  *         self._data = self.init_data(**kwargs) if 'end_date' in kwargs else None
  * 
  *     def _init_self(self, **kwargs):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
 
@@ -1576,26 +1600,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_init_self") < 0)) __PYX_ERR(0, 14, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_init_self") < 0)) __PYX_ERR(0, 16, __pyx_L3_error)
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
-  __Pyx_RaiseArgtupleInvalid("_init_self", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 14, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_init_self", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 16, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("hermes.factors.test.factor_test.FactorTest._init_self", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_2_init_self(__pyx_self, __pyx_v_self, __pyx_v_kwargs);
@@ -1614,57 +1638,41 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/test/factor_test.pyx":17
+/* "hermes/factors/test/factor_test.pyx":19
  *         pass
  * 
- *     def test1(self,             # <<<<<<<<<<<<<<
- *               data=None,
- *               dependencies=['openPrice', 'closePrice', 'vwap']):
+ *     def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap']):             # <<<<<<<<<<<<<<
+ *         data = self._data if data is None else data
+ *         close_se = data['openPrice']
  */
 
 static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test___defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__defaults__", 0);
   __Pyx_XDECREF(__pyx_r);
-
-  /* "hermes/factors/test/factor_test.pyx":18
- * 
- *     def test1(self,
- *               data=None,             # <<<<<<<<<<<<<<
- *               dependencies=['openPrice', 'closePrice', 'vwap']):
- *         data = self._data if data is None else data
- */
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)Py_None));
   __Pyx_GIVEREF(((PyObject *)Py_None));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_None));
   __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_dependencies);
   __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_dependencies);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_dependencies);
-
-  /* "hermes/factors/test/factor_test.pyx":17
- *         pass
- * 
- *     def test1(self,             # <<<<<<<<<<<<<<
- *               data=None,
- *               dependencies=['openPrice', 'closePrice', 'vwap']):
- */
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_2, 1, Py_None);
   __pyx_t_1 = 0;
@@ -1732,15 +1740,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dependencies);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "test1") < 0)) __PYX_ERR(0, 17, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "test1") < 0)) __PYX_ERR(0, 19, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -1751,15 +1759,15 @@
     }
     __pyx_v_self = values[0];
     __pyx_v_data = values[1];
     __pyx_v_dependencies = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("test1", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 17, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("test1", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 19, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("hermes.factors.test.factor_test.FactorTest.test1", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_4test1(__pyx_self, __pyx_v_self, __pyx_v_data, __pyx_v_dependencies);
 
@@ -1785,16 +1793,16 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("test1", 0);
   __Pyx_INCREF(__pyx_v_data);
 
   /* "hermes/factors/test/factor_test.pyx":20
- *               data=None,
- *               dependencies=['openPrice', 'closePrice', 'vwap']):
+ * 
+ *     def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap']):
  *         data = self._data if data is None else data             # <<<<<<<<<<<<<<
  *         close_se = data['openPrice']
  *         dy_q_ti_se = data['closePrice']
  */
   __pyx_t_2 = (__pyx_v_data == Py_None);
   if ((__pyx_t_2 != 0)) {
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 20, __pyx_L1_error)
@@ -1805,15 +1813,15 @@
     __Pyx_INCREF(__pyx_v_data);
     __pyx_t_1 = __pyx_v_data;
   }
   __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "hermes/factors/test/factor_test.pyx":21
- *               dependencies=['openPrice', 'closePrice', 'vwap']):
+ *     def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap']):
  *         data = self._data if data is None else data
  *         close_se = data['openPrice']             # <<<<<<<<<<<<<<
  *         dy_q_ti_se = data['closePrice']
  *         totalshares_se = data['vwap']
  */
   __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_openPrice); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
@@ -1862,37 +1870,37 @@
   __pyx_v_dy_q_evebitda_caldr_se = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "hermes/factors/test/factor_test.pyx":26
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan             # <<<<<<<<<<<<<<
- *         return self._format(dy_q_evebitda_caldr_se, "factor1")
+ *         return self._format(dy_q_evebitda_caldr_se, "test1")
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_nan); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "hermes/factors/test/factor_test.pyx":25
  *         totalshares_se = data['vwap']
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |             # <<<<<<<<<<<<<<
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan
- *         return self._format(dy_q_evebitda_caldr_se, "factor1")
+ *         return self._format(dy_q_evebitda_caldr_se, "test1")
  */
   __pyx_t_1 = PyObject_RichCompare(__pyx_v_dy_q_evebitda_caldr_se, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
 
   /* "hermes/factors/test/factor_test.pyx":26
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan             # <<<<<<<<<<<<<<
- *         return self._format(dy_q_evebitda_caldr_se, "factor1")
+ *         return self._format(dy_q_evebitda_caldr_se, "test1")
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_isinf); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
@@ -1913,30 +1921,30 @@
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
   /* "hermes/factors/test/factor_test.pyx":25
  *         totalshares_se = data['vwap']
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |             # <<<<<<<<<<<<<<
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan
- *         return self._format(dy_q_evebitda_caldr_se, "factor1")
+ *         return self._format(dy_q_evebitda_caldr_se, "test1")
  */
   __pyx_t_6 = PyNumber_Or(__pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (unlikely(PyObject_SetItem(__pyx_v_dy_q_evebitda_caldr_se, __pyx_t_6, __pyx_t_3) < 0)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "hermes/factors/test/factor_test.pyx":27
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan
- *         return self._format(dy_q_evebitda_caldr_se, "factor1")             # <<<<<<<<<<<<<<
+ *         return self._format(dy_q_evebitda_caldr_se, "test1")             # <<<<<<<<<<<<<<
  * 
- *     def test2(self,
+ *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_format); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_4 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
@@ -1947,55 +1955,55 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
       __pyx_t_7 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_6)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_dy_q_evebitda_caldr_se, __pyx_n_s_factor1};
+    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_dy_q_evebitda_caldr_se, __pyx_n_s_test1};
     __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_dy_q_evebitda_caldr_se, __pyx_n_s_factor1};
+    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_dy_q_evebitda_caldr_se, __pyx_n_s_test1};
     __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   {
     __pyx_t_1 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_v_dy_q_evebitda_caldr_se);
     __Pyx_GIVEREF(__pyx_v_dy_q_evebitda_caldr_se);
     PyTuple_SET_ITEM(__pyx_t_1, 0+__pyx_t_7, __pyx_v_dy_q_evebitda_caldr_se);
-    __Pyx_INCREF(__pyx_n_s_factor1);
-    __Pyx_GIVEREF(__pyx_n_s_factor1);
-    PyTuple_SET_ITEM(__pyx_t_1, 1+__pyx_t_7, __pyx_n_s_factor1);
+    __Pyx_INCREF(__pyx_n_s_test1);
+    __Pyx_GIVEREF(__pyx_n_s_test1);
+    PyTuple_SET_ITEM(__pyx_t_1, 1+__pyx_t_7, __pyx_n_s_test1);
     __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_1, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "hermes/factors/test/factor_test.pyx":17
+  /* "hermes/factors/test/factor_test.pyx":19
  *         pass
  * 
- *     def test1(self,             # <<<<<<<<<<<<<<
- *               data=None,
- *               dependencies=['openPrice', 'closePrice', 'vwap']):
+ *     def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap']):             # <<<<<<<<<<<<<<
+ *         data = self._data if data is None else data
+ *         close_se = data['openPrice']
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
@@ -2011,55 +2019,39 @@
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "hermes/factors/test/factor_test.pyx":29
- *         return self._format(dy_q_evebitda_caldr_se, "factor1")
+ *         return self._format(dy_q_evebitda_caldr_se, "test1")
  * 
- *     def test2(self,             # <<<<<<<<<<<<<<
- *               data=None,
- *               dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):
+ *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):             # <<<<<<<<<<<<<<
+ *         data = self._data if data is None else data
+ *         close_se = data['marketValue']
  */
 
 static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_2__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__defaults__", 0);
   __Pyx_XDECREF(__pyx_r);
-
-  /* "hermes/factors/test/factor_test.pyx":30
- * 
- *     def test2(self,
- *               data=None,             # <<<<<<<<<<<<<<
- *               dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):
- *         data = self._data if data is None else data
- */
   __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)Py_None));
   __Pyx_GIVEREF(((PyObject *)Py_None));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_None));
   __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_dependencies);
   __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_dependencies);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_dependencies);
-
-  /* "hermes/factors/test/factor_test.pyx":29
- *         return self._format(dy_q_evebitda_caldr_se, "factor1")
- * 
- *     def test2(self,             # <<<<<<<<<<<<<<
- *               data=None,
- *               dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):
- */
   __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_2, 1, Py_None);
@@ -2180,162 +2172,162 @@
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("test2", 0);
   __Pyx_INCREF(__pyx_v_data);
 
-  /* "hermes/factors/test/factor_test.pyx":32
- *               data=None,
- *               dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):
+  /* "hermes/factors/test/factor_test.pyx":30
+ * 
+ *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):
  *         data = self._data if data is None else data             # <<<<<<<<<<<<<<
  *         close_se = data['marketValue']
  *         dy_q_ti_se = data['turnoverVol']
  */
   __pyx_t_2 = (__pyx_v_data == Py_None);
   if ((__pyx_t_2 != 0)) {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 32, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   } else {
     __Pyx_INCREF(__pyx_v_data);
     __pyx_t_1 = __pyx_v_data;
   }
   __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":33
- *               dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):
+  /* "hermes/factors/test/factor_test.pyx":31
+ *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):
  *         data = self._data if data is None else data
  *         close_se = data['marketValue']             # <<<<<<<<<<<<<<
  *         dy_q_ti_se = data['turnoverVol']
  *         totalshares_se = data['negMarketValue']
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_marketValue); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_marketValue); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_close_se = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":34
+  /* "hermes/factors/test/factor_test.pyx":32
  *         data = self._data if data is None else data
  *         close_se = data['marketValue']
  *         dy_q_ti_se = data['turnoverVol']             # <<<<<<<<<<<<<<
  *         totalshares_se = data['negMarketValue']
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_turnoverVol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_turnoverVol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_dy_q_ti_se = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":35
+  /* "hermes/factors/test/factor_test.pyx":33
  *         close_se = data['marketValue']
  *         dy_q_ti_se = data['turnoverVol']
  *         totalshares_se = data['negMarketValue']             # <<<<<<<<<<<<<<
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_negMarketValue); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_negMarketValue); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_totalshares_se = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":36
+  /* "hermes/factors/test/factor_test.pyx":34
  *         dy_q_ti_se = data['turnoverVol']
  *         totalshares_se = data['negMarketValue']
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)             # <<<<<<<<<<<<<<
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan
  */
-  __pyx_t_1 = PyNumber_Multiply(__pyx_int_4, __pyx_v_dy_q_ti_se); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Multiply(__pyx_int_4, __pyx_v_dy_q_ti_se); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_v_totalshares_se); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_v_totalshares_se); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_v_close_se, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_v_close_se, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_dy_q_evebitda_caldr_se = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":38
+  /* "hermes/factors/test/factor_test.pyx":36
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan             # <<<<<<<<<<<<<<
- *         return self._format(dy_q_evebitda_caldr_se, "factor2")
+ *         return self._format(dy_q_evebitda_caldr_se, "test2")
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_nan); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_nan); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":37
+  /* "hermes/factors/test/factor_test.pyx":35
  *         totalshares_se = data['negMarketValue']
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |             # <<<<<<<<<<<<<<
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan
- *         return self._format(dy_q_evebitda_caldr_se, "factor2")
+ *         return self._format(dy_q_evebitda_caldr_se, "test2")
  */
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_dy_q_evebitda_caldr_se, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_dy_q_evebitda_caldr_se, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
 
-  /* "hermes/factors/test/factor_test.pyx":38
+  /* "hermes/factors/test/factor_test.pyx":36
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan             # <<<<<<<<<<<<<<
- *         return self._format(dy_q_evebitda_caldr_se, "factor2")
+ *         return self._format(dy_q_evebitda_caldr_se, "test2")
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_isinf); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_isinf); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 36, __pyx_L1_error)
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
   __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_5, __pyx_v_dy_q_evebitda_caldr_se) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_dy_q_evebitda_caldr_se);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 38, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":37
+  /* "hermes/factors/test/factor_test.pyx":35
  *         totalshares_se = data['negMarketValue']
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |             # <<<<<<<<<<<<<<
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan
- *         return self._format(dy_q_evebitda_caldr_se, "factor2")
+ *         return self._format(dy_q_evebitda_caldr_se, "test2")
  */
-  __pyx_t_6 = PyNumber_Or(__pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_6 = PyNumber_Or(__pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_v_dy_q_evebitda_caldr_se, __pyx_t_6, __pyx_t_3) < 0)) __PYX_ERR(0, 37, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_dy_q_evebitda_caldr_se, __pyx_t_6, __pyx_t_3) < 0)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":39
+  /* "hermes/factors/test/factor_test.pyx":37
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan
- *         return self._format(dy_q_evebitda_caldr_se, "factor2")             # <<<<<<<<<<<<<<
+ *         return self._format(dy_q_evebitda_caldr_se, "test2")             # <<<<<<<<<<<<<<
  * 
  *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice']):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_format); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_format); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_4 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -2343,55 +2335,55 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
       __pyx_t_7 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_6)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_dy_q_evebitda_caldr_se, __pyx_n_s_factor2};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 39, __pyx_L1_error)
+    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_dy_q_evebitda_caldr_se, __pyx_n_s_test2};
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_dy_q_evebitda_caldr_se, __pyx_n_s_factor2};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 39, __pyx_L1_error)
+    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_dy_q_evebitda_caldr_se, __pyx_n_s_test2};
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   {
-    __pyx_t_1 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_v_dy_q_evebitda_caldr_se);
     __Pyx_GIVEREF(__pyx_v_dy_q_evebitda_caldr_se);
     PyTuple_SET_ITEM(__pyx_t_1, 0+__pyx_t_7, __pyx_v_dy_q_evebitda_caldr_se);
-    __Pyx_INCREF(__pyx_n_s_factor2);
-    __Pyx_GIVEREF(__pyx_n_s_factor2);
-    PyTuple_SET_ITEM(__pyx_t_1, 1+__pyx_t_7, __pyx_n_s_factor2);
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_1, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 39, __pyx_L1_error)
+    __Pyx_INCREF(__pyx_n_s_test2);
+    __Pyx_GIVEREF(__pyx_n_s_test2);
+    PyTuple_SET_ITEM(__pyx_t_1, 1+__pyx_t_7, __pyx_n_s_test2);
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_1, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* "hermes/factors/test/factor_test.pyx":29
- *         return self._format(dy_q_evebitda_caldr_se, "factor1")
+ *         return self._format(dy_q_evebitda_caldr_se, "test1")
  * 
- *     def test2(self,             # <<<<<<<<<<<<<<
- *               data=None,
- *               dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):
+ *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):             # <<<<<<<<<<<<<<
+ *         data = self._data if data is None else data
+ *         close_se = data['marketValue']
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
@@ -2406,16 +2398,16 @@
   __Pyx_XDECREF(__pyx_v_dy_q_evebitda_caldr_se);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/test/factor_test.pyx":41
- *         return self._format(dy_q_evebitda_caldr_se, "factor2")
+/* "hermes/factors/test/factor_test.pyx":39
+ *         return self._format(dy_q_evebitda_caldr_se, "test2")
  * 
  *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice']):             # <<<<<<<<<<<<<<
  *         data = self._data if data is None else data
  *         turnoverVol = data['turnoverVol']
  */
 
 static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_4__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
@@ -2424,23 +2416,23 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__defaults__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)Py_None));
   __Pyx_GIVEREF(((PyObject *)Py_None));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_None));
   __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_self)->__pyx_arg_dependencies);
   __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_self)->__pyx_arg_dependencies);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_self)->__pyx_arg_dependencies);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_2, 1, Py_None);
   __pyx_t_1 = 0;
@@ -2508,15 +2500,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dependencies);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "test3") < 0)) __PYX_ERR(0, 41, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "test3") < 0)) __PYX_ERR(0, 39, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -2527,15 +2519,15 @@
     }
     __pyx_v_self = values[0];
     __pyx_v_data = values[1];
     __pyx_v_dependencies = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("test3", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 41, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("test3", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 39, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("hermes.factors.test.factor_test.FactorTest.test3", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_8test3(__pyx_self, __pyx_v_self, __pyx_v_data, __pyx_v_dependencies);
 
@@ -2561,92 +2553,92 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("test3", 0);
   __Pyx_INCREF(__pyx_v_data);
 
-  /* "hermes/factors/test/factor_test.pyx":42
+  /* "hermes/factors/test/factor_test.pyx":40
  * 
  *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice']):
  *         data = self._data if data is None else data             # <<<<<<<<<<<<<<
  *         turnoverVol = data['turnoverVol']
  *         closePrice = data['closePrice']
  */
   __pyx_t_2 = (__pyx_v_data == Py_None);
   if ((__pyx_t_2 != 0)) {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   } else {
     __Pyx_INCREF(__pyx_v_data);
     __pyx_t_1 = __pyx_v_data;
   }
   __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":43
+  /* "hermes/factors/test/factor_test.pyx":41
  *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice']):
  *         data = self._data if data is None else data
  *         turnoverVol = data['turnoverVol']             # <<<<<<<<<<<<<<
  *         closePrice = data['closePrice']
  *         factor1 = turnoverVol * closePrice
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_turnoverVol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_turnoverVol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_turnoverVol = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":44
+  /* "hermes/factors/test/factor_test.pyx":42
  *         data = self._data if data is None else data
  *         turnoverVol = data['turnoverVol']
  *         closePrice = data['closePrice']             # <<<<<<<<<<<<<<
  *         factor1 = turnoverVol * closePrice
  *         factor2 = turnoverVol + closePrice
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_closePrice); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_closePrice); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_closePrice = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":45
+  /* "hermes/factors/test/factor_test.pyx":43
  *         turnoverVol = data['turnoverVol']
  *         closePrice = data['closePrice']
  *         factor1 = turnoverVol * closePrice             # <<<<<<<<<<<<<<
  *         factor2 = turnoverVol + closePrice
  *         factors = {
  */
-  __pyx_t_1 = PyNumber_Multiply(__pyx_v_turnoverVol, __pyx_v_closePrice); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Multiply(__pyx_v_turnoverVol, __pyx_v_closePrice); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_factor1 = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":46
+  /* "hermes/factors/test/factor_test.pyx":44
  *         closePrice = data['closePrice']
  *         factor1 = turnoverVol * closePrice
  *         factor2 = turnoverVol + closePrice             # <<<<<<<<<<<<<<
  *         factors = {
  *             'factor3': self._format(factor1, "factor3"),
  */
-  __pyx_t_1 = PyNumber_Add(__pyx_v_turnoverVol, __pyx_v_closePrice); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_v_turnoverVol, __pyx_v_closePrice); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_factor2 = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":48
+  /* "hermes/factors/test/factor_test.pyx":46
  *         factor2 = turnoverVol + closePrice
  *         factors = {
  *             'factor3': self._format(factor1, "factor3"),             # <<<<<<<<<<<<<<
  *             'factor4': self._format(factor2, "factor4")
  *         }
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -2655,55 +2647,55 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_factor1, __pyx_n_s_factor3};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 48, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_factor1, __pyx_n_s_factor3};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 48, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 48, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_INCREF(__pyx_v_factor1);
     __Pyx_GIVEREF(__pyx_v_factor1);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_v_factor1);
     __Pyx_INCREF(__pyx_n_s_factor3);
     __Pyx_GIVEREF(__pyx_n_s_factor3);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_n_s_factor3);
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 48, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_factor3, __pyx_t_3) < 0) __PYX_ERR(0, 48, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_factor3, __pyx_t_3) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":49
+  /* "hermes/factors/test/factor_test.pyx":47
  *         factors = {
  *             'factor3': self._format(factor1, "factor3"),
  *             'factor4': self._format(factor2, "factor4")             # <<<<<<<<<<<<<<
  *         }
  *         return factors
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_7 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -2712,61 +2704,61 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_v_factor2, __pyx_n_s_factor4};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 47, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_v_factor2, __pyx_n_s_factor4};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 47, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 49, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 47, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_INCREF(__pyx_v_factor2);
     __Pyx_GIVEREF(__pyx_v_factor2);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_6, __pyx_v_factor2);
     __Pyx_INCREF(__pyx_n_s_factor4);
     __Pyx_GIVEREF(__pyx_n_s_factor4);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_6, __pyx_n_s_factor4);
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 47, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_factor4, __pyx_t_3) < 0) __PYX_ERR(0, 48, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_factor4, __pyx_t_3) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_factors = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":51
+  /* "hermes/factors/test/factor_test.pyx":49
  *             'factor4': self._format(factor2, "factor4")
  *         }
  *         return factors             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_factors);
   __pyx_r = __pyx_v_factors;
   goto __pyx_L0;
 
-  /* "hermes/factors/test/factor_test.pyx":41
- *         return self._format(dy_q_evebitda_caldr_se, "factor2")
+  /* "hermes/factors/test/factor_test.pyx":39
+ *         return self._format(dy_q_evebitda_caldr_se, "test2")
  * 
  *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice']):             # <<<<<<<<<<<<<<
  *         data = self._data if data is None else data
  *         turnoverVol = data['turnoverVol']
  */
 
   /* function exit code */
@@ -2848,14 +2840,16 @@
   {&__pyx_n_s_ShortCallMixin, __pyx_k_ShortCallMixin, sizeof(__pyx_k_ShortCallMixin), 0, 0, 1, 1},
   {&__pyx_n_s_category, __pyx_k_category, sizeof(__pyx_k_category), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_closePrice, __pyx_k_closePrice, sizeof(__pyx_k_closePrice), 0, 0, 1, 1},
   {&__pyx_n_s_close_se, __pyx_k_close_se, sizeof(__pyx_k_close_se), 0, 0, 1, 1},
   {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
   {&__pyx_n_s_data_2, __pyx_k_data_2, sizeof(__pyx_k_data_2), 0, 0, 1, 1},
+  {&__pyx_n_s_data_format, __pyx_k_data_format, sizeof(__pyx_k_data_format), 0, 0, 1, 1},
+  {&__pyx_n_s_data_format_2, __pyx_k_data_format_2, sizeof(__pyx_k_data_format_2), 0, 0, 1, 1},
   {&__pyx_n_s_dependencies, __pyx_k_dependencies, sizeof(__pyx_k_dependencies), 0, 0, 1, 1},
   {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
   {&__pyx_n_s_dy_q_evebitda_caldr_se, __pyx_k_dy_q_evebitda_caldr_se, sizeof(__pyx_k_dy_q_evebitda_caldr_se), 0, 0, 1, 1},
   {&__pyx_n_s_dy_q_ti_se, __pyx_k_dy_q_ti_se, sizeof(__pyx_k_dy_q_ti_se), 0, 0, 1, 1},
   {&__pyx_n_s_end_date, __pyx_k_end_date, sizeof(__pyx_k_end_date), 0, 0, 1, 1},
   {&__pyx_n_s_factor1, __pyx_k_factor1, sizeof(__pyx_k_factor1), 0, 0, 1, 1},
   {&__pyx_n_s_factor2, __pyx_k_factor2, sizeof(__pyx_k_factor2), 0, 0, 1, 1},
@@ -2903,73 +2897,73 @@
   return 0;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "hermes/factors/test/factor_test.pyx":8
- * 
+  /* "hermes/factors/test/factor_test.pyx":9
  * class FactorTest(FactorBase, LongCallMixin, ShortCallMixin):
- *     def __init__(self, **kwargs):             # <<<<<<<<<<<<<<
+ * 
+ *     def __init__(self, data_format, **kwargs):             # <<<<<<<<<<<<<<
  *         __str__ = 'factor_test'
  *         self.category = 'test'
  */
-  __pyx_tuple__2 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_kwargs, __pyx_n_s_str); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_data_format, __pyx_n_s_kwargs, __pyx_n_s_str); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_test_factor_test_2, __pyx_n_s_init, 8, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_test_factor_test_2, __pyx_n_s_init, 9, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 9, __pyx_L1_error)
 
-  /* "hermes/factors/test/factor_test.pyx":14
+  /* "hermes/factors/test/factor_test.pyx":16
  *         self._data = self.init_data(**kwargs) if 'end_date' in kwargs else None
  * 
  *     def _init_self(self, **kwargs):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
-  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_test_factor_test_2, __pyx_n_s_init_self, 14, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_test_factor_test_2, __pyx_n_s_init_self, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 16, __pyx_L1_error)
 
-  /* "hermes/factors/test/factor_test.pyx":17
+  /* "hermes/factors/test/factor_test.pyx":19
  *         pass
  * 
- *     def test1(self,             # <<<<<<<<<<<<<<
- *               data=None,
- *               dependencies=['openPrice', 'closePrice', 'vwap']):
+ *     def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap']):             # <<<<<<<<<<<<<<
+ *         data = self._data if data is None else data
+ *         close_se = data['openPrice']
  */
-  __pyx_tuple__6 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_data_2, __pyx_n_s_dependencies, __pyx_n_s_close_se, __pyx_n_s_dy_q_ti_se, __pyx_n_s_totalshares_se, __pyx_n_s_dy_q_evebitda_caldr_se); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_data_2, __pyx_n_s_dependencies, __pyx_n_s_close_se, __pyx_n_s_dy_q_ti_se, __pyx_n_s_totalshares_se, __pyx_n_s_dy_q_evebitda_caldr_se); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(3, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_test_factor_test_2, __pyx_n_s_test1, 17, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(3, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_test_factor_test_2, __pyx_n_s_test1, 19, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 19, __pyx_L1_error)
 
   /* "hermes/factors/test/factor_test.pyx":29
- *         return self._format(dy_q_evebitda_caldr_se, "factor1")
+ *         return self._format(dy_q_evebitda_caldr_se, "test1")
  * 
- *     def test2(self,             # <<<<<<<<<<<<<<
- *               data=None,
- *               dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):
+ *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):             # <<<<<<<<<<<<<<
+ *         data = self._data if data is None else data
+ *         close_se = data['marketValue']
  */
   __pyx_tuple__8 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_data_2, __pyx_n_s_dependencies, __pyx_n_s_close_se, __pyx_n_s_dy_q_ti_se, __pyx_n_s_totalshares_se, __pyx_n_s_dy_q_evebitda_caldr_se); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
   __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(3, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_test_factor_test_2, __pyx_n_s_test2, 29, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 29, __pyx_L1_error)
 
-  /* "hermes/factors/test/factor_test.pyx":41
- *         return self._format(dy_q_evebitda_caldr_se, "factor2")
+  /* "hermes/factors/test/factor_test.pyx":39
+ *         return self._format(dy_q_evebitda_caldr_se, "test2")
  * 
  *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice']):             # <<<<<<<<<<<<<<
  *         data = self._data if data is None else data
  *         turnoverVol = data['turnoverVol']
  */
-  __pyx_tuple__10 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_data_2, __pyx_n_s_dependencies, __pyx_n_s_turnoverVol, __pyx_n_s_closePrice, __pyx_n_s_factor1, __pyx_n_s_factor2, __pyx_n_s_factors); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_data_2, __pyx_n_s_dependencies, __pyx_n_s_turnoverVol, __pyx_n_s_closePrice, __pyx_n_s_factor1, __pyx_n_s_factor2, __pyx_n_s_factors); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_test_factor_test_2, __pyx_n_s_test3, 41, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_test_factor_test_2, __pyx_n_s_test3, 39, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -3310,16 +3304,16 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "hermes/factors/test/factor_test.pyx":7
  * 
  * 
  * class FactorTest(FactorBase, LongCallMixin, ShortCallMixin):             # <<<<<<<<<<<<<<
- *     def __init__(self, **kwargs):
- *         __str__ = 'factor_test'
+ * 
+ *     def __init__(self, data_format, **kwargs):
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FactorBase); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_LongCallMixin); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_ShortCallMixin); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
@@ -3335,56 +3329,48 @@
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_3, __pyx_t_4, __pyx_n_s_FactorTest, __pyx_n_s_FactorTest, (PyObject *) NULL, __pyx_n_s_hermes_factors_test_factor_test, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "hermes/factors/test/factor_test.pyx":8
- * 
+  /* "hermes/factors/test/factor_test.pyx":9
  * class FactorTest(FactorBase, LongCallMixin, ShortCallMixin):
- *     def __init__(self, **kwargs):             # <<<<<<<<<<<<<<
+ * 
+ *     def __init__(self, data_format, **kwargs):             # <<<<<<<<<<<<<<
  *         __str__ = 'factor_test'
  *         self.category = 'test'
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_1__init__, 0, __pyx_n_s_FactorTest___init, NULL, __pyx_n_s_hermes_factors_test_factor_test, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_1__init__, 0, __pyx_n_s_FactorTest___init, NULL, __pyx_n_s_hermes_factors_test_factor_test, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_2) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_2) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":14
+  /* "hermes/factors/test/factor_test.pyx":16
  *         self._data = self.init_data(**kwargs) if 'end_date' in kwargs else None
  * 
  *     def _init_self(self, **kwargs):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_3_init_self, 0, __pyx_n_s_FactorTest__init_self, NULL, __pyx_n_s_hermes_factors_test_factor_test, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_3_init_self, 0, __pyx_n_s_FactorTest__init_self, NULL, __pyx_n_s_hermes_factors_test_factor_test, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init_self, __pyx_t_2) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init_self, __pyx_t_2) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":17
+  /* "hermes/factors/test/factor_test.pyx":19
  *         pass
  * 
- *     def test1(self,             # <<<<<<<<<<<<<<
- *               data=None,
- *               dependencies=['openPrice', 'closePrice', 'vwap']):
- */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_5test1, 0, __pyx_n_s_FactorTest_test1, NULL, __pyx_n_s_hermes_factors_test_factor_test, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults), 1)) __PYX_ERR(0, 17, __pyx_L1_error)
-
-  /* "hermes/factors/test/factor_test.pyx":19
- *     def test1(self,
- *               data=None,
- *               dependencies=['openPrice', 'closePrice', 'vwap']):             # <<<<<<<<<<<<<<
+ *     def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap']):             # <<<<<<<<<<<<<<
  *         data = self._data if data is None else data
  *         close_se = data['openPrice']
  */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_5test1, 0, __pyx_n_s_FactorTest_test1, NULL, __pyx_n_s_hermes_factors_test_factor_test, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults), 1)) __PYX_ERR(0, 19, __pyx_L1_error)
   __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_n_s_openPrice);
   __Pyx_GIVEREF(__pyx_n_s_openPrice);
   PyList_SET_ITEM(__pyx_t_5, 0, __pyx_n_s_openPrice);
   __Pyx_INCREF(__pyx_n_s_closePrice);
   __Pyx_GIVEREF(__pyx_n_s_closePrice);
@@ -3392,36 +3378,28 @@
   __Pyx_INCREF(__pyx_n_s_vwap);
   __Pyx_GIVEREF(__pyx_n_s_vwap);
   PyList_SET_ITEM(__pyx_t_5, 2, __pyx_n_s_vwap);
   __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_t_2)->__pyx_arg_dependencies = __pyx_t_5;
   __Pyx_GIVEREF(__pyx_t_5);
   __pyx_t_5 = 0;
   __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_6hermes_7factors_4test_11factor_test___defaults__);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_test1, __pyx_t_2) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_test1, __pyx_t_2) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "hermes/factors/test/factor_test.pyx":29
- *         return self._format(dy_q_evebitda_caldr_se, "factor1")
+ *         return self._format(dy_q_evebitda_caldr_se, "test1")
  * 
- *     def test2(self,             # <<<<<<<<<<<<<<
- *               data=None,
- *               dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):
+ *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):             # <<<<<<<<<<<<<<
+ *         data = self._data if data is None else data
+ *         close_se = data['marketValue']
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_7test2, 0, __pyx_n_s_FactorTest_test2, NULL, __pyx_n_s_hermes_factors_test_factor_test, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults1), 1)) __PYX_ERR(0, 29, __pyx_L1_error)
-
-  /* "hermes/factors/test/factor_test.pyx":31
- *     def test2(self,
- *               data=None,
- *               dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):             # <<<<<<<<<<<<<<
- *         data = self._data if data is None else data
- *         close_se = data['marketValue']
- */
-  __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_n_s_marketValue);
   __Pyx_GIVEREF(__pyx_n_s_marketValue);
   PyList_SET_ITEM(__pyx_t_5, 0, __pyx_n_s_marketValue);
   __Pyx_INCREF(__pyx_n_s_turnoverVol);
   __Pyx_GIVEREF(__pyx_n_s_turnoverVol);
   PyList_SET_ITEM(__pyx_t_5, 1, __pyx_n_s_turnoverVol);
@@ -3431,45 +3409,45 @@
   __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_t_2)->__pyx_arg_dependencies = __pyx_t_5;
   __Pyx_GIVEREF(__pyx_t_5);
   __pyx_t_5 = 0;
   __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_6hermes_7factors_4test_11factor_test_2__defaults__);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_test2, __pyx_t_2) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":41
- *         return self._format(dy_q_evebitda_caldr_se, "factor2")
+  /* "hermes/factors/test/factor_test.pyx":39
+ *         return self._format(dy_q_evebitda_caldr_se, "test2")
  * 
  *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice']):             # <<<<<<<<<<<<<<
  *         data = self._data if data is None else data
  *         turnoverVol = data['turnoverVol']
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_9test3, 0, __pyx_n_s_FactorTest_test3, NULL, __pyx_n_s_hermes_factors_test_factor_test, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_9test3, 0, __pyx_n_s_FactorTest_test3, NULL, __pyx_n_s_hermes_factors_test_factor_test, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults2), 1)) __PYX_ERR(0, 41, __pyx_L1_error)
-  __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 41, __pyx_L1_error)
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults2), 1)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_n_s_turnoverVol);
   __Pyx_GIVEREF(__pyx_n_s_turnoverVol);
   PyList_SET_ITEM(__pyx_t_5, 0, __pyx_n_s_turnoverVol);
   __Pyx_INCREF(__pyx_n_s_closePrice);
   __Pyx_GIVEREF(__pyx_n_s_closePrice);
   PyList_SET_ITEM(__pyx_t_5, 1, __pyx_n_s_closePrice);
   __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_t_2)->__pyx_arg_dependencies = __pyx_t_5;
   __Pyx_GIVEREF(__pyx_t_5);
   __pyx_t_5 = 0;
   __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_6hermes_7factors_4test_11factor_test_4__defaults__);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_test3, __pyx_t_2) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_test3, __pyx_t_2) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "hermes/factors/test/factor_test.pyx":7
  * 
  * 
  * class FactorTest(FactorBase, LongCallMixin, ShortCallMixin):             # <<<<<<<<<<<<<<
- *     def __init__(self, **kwargs):
- *         __str__ = 'factor_test'
+ * 
+ *     def __init__(self, data_format, **kwargs):
  */
   __pyx_t_2 = __Pyx_Py3ClassCreate(__pyx_t_3, __pyx_n_s_FactorTest, __pyx_t_4, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_FactorTest, __pyx_t_2) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -3527,14 +3505,40 @@
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
 #endif
 
+/* RaiseArgTupleInvalid */
+static void __Pyx_RaiseArgtupleInvalid(
+    const char* func_name,
+    int exact,
+    Py_ssize_t num_min,
+    Py_ssize_t num_max,
+    Py_ssize_t num_found)
+{
+    Py_ssize_t num_expected;
+    const char *more_or_less;
+    if (num_found < num_min) {
+        num_expected = num_min;
+        more_or_less = "at least";
+    } else {
+        num_expected = num_max;
+        more_or_less = "at most";
+    }
+    if (exact) {
+        more_or_less = "exactly";
+    }
+    PyErr_Format(PyExc_TypeError,
+                 "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                 func_name, more_or_less, num_expected,
+                 (num_expected == 1) ? "" : "s", num_found);
+}
+
 /* RaiseDoubleKeywords */
 static void __Pyx_RaiseDoubleKeywordsError(
     const char* func_name,
     PyObject* kw_name)
 {
     PyErr_Format(PyExc_TypeError,
         #if PY_MAJOR_VERSION >= 3
@@ -3643,40 +3647,14 @@
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
-/* RaiseArgTupleInvalid */
-static void __Pyx_RaiseArgtupleInvalid(
-    const char* func_name,
-    int exact,
-    Py_ssize_t num_min,
-    Py_ssize_t num_max,
-    Py_ssize_t num_found)
-{
-    Py_ssize_t num_expected;
-    const char *more_or_less;
-    if (num_found < num_min) {
-        num_expected = num_min;
-        more_or_less = "at least";
-    } else {
-        num_expected = num_max;
-        more_or_less = "at most";
-    }
-    if (exact) {
-        more_or_less = "exactly";
-    }
-    PyErr_Format(PyExc_TypeError,
-                 "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
-                 func_name, more_or_less, num_expected,
-                 (num_expected == 1) ? "" : "s", num_found);
-}
-
 /* PyObjectSetAttrStr */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value) {
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_setattro))
         return tp->tp_setattro(obj, attr_name, value);
 #if PY_MAJOR_VERSION < 3
```

### Comparing `Finance-Hermes-0.2.9/hermes/factors/test/factor_test.pyx` & `Finance-Hermes-0.3.0/hermes/factors/test/factor_test.pyx`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 # -*- encoding:utf-8 -*-
 import pdb
 import numpy as np
 from hermes.factors.base import FactorBase, LongCallMixin, ShortCallMixin
 
 
 class FactorTest(FactorBase, LongCallMixin, ShortCallMixin):
-    def __init__(self, **kwargs):
+
+    def __init__(self, data_format, **kwargs):
         __str__ = 'factor_test'
         self.category = 'test'
         self.name = '测试因子'
+        self._data_format = data_format
         self._data = self.init_data(**kwargs) if 'end_date' in kwargs else None
 
     def _init_self(self, **kwargs):
         pass
-
-    def test1(self,
-              data=None,
-              dependencies=['openPrice', 'closePrice', 'vwap']):
+    
+    def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap']):
         data = self._data if data is None else data
         close_se = data['openPrice']
         dy_q_ti_se = data['closePrice']
         totalshares_se = data['vwap']
         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan
-        return self._format(dy_q_evebitda_caldr_se, "factor1")
-
-    def test2(self,
-              data=None,
-              dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):
+        return self._format(dy_q_evebitda_caldr_se, "test1")
+    
+    def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):
         data = self._data if data is None else data
         close_se = data['marketValue']
         dy_q_ti_se = data['turnoverVol']
         totalshares_se = data['negMarketValue']
         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan
-        return self._format(dy_q_evebitda_caldr_se, "factor2")
-
+        return self._format(dy_q_evebitda_caldr_se, "test2")
+    
     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice']):
         data = self._data if data is None else data
         turnoverVol = data['turnoverVol']
         closePrice = data['closePrice']
         factor1 = turnoverVol * closePrice
         factor2 = turnoverVol + closePrice
         factors = {
```

### Comparing `Finance-Hermes-0.2.9/hermes/kdutils/base.c` & `Finance-Hermes-0.3.0/hermes/kdutils/base.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.9/hermes/kdutils/base.pyx` & `Finance-Hermes-0.3.0/hermes/kdutils/base.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.9/hermes/kdutils/core/fixes.c` & `Finance-Hermes-0.3.0/hermes/kdutils/core/fixes.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.9/hermes/kdutils/core/fixes.pyx` & `Finance-Hermes-0.3.0/hermes/kdutils/core/fixes.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.9/hermes/kdutils/core/helper.c` & `Finance-Hermes-0.3.0/hermes/kdutils/core/helper.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.9/hermes/kdutils/core/helper.pyx` & `Finance-Hermes-0.3.0/hermes/kdutils/core/helper.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.9/hermes/kdutils/create_id.c` & `Finance-Hermes-0.3.0/hermes/kdutils/create_id.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.9/hermes/kdutils/create_id.pyx` & `Finance-Hermes-0.3.0/hermes/kdutils/create_id.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.9/hermes/kdutils/lazy.c` & `Finance-Hermes-0.3.0/hermes/kdutils/lazy.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.9/hermes/kdutils/lazy.pyx` & `Finance-Hermes-0.3.0/hermes/kdutils/lazy.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.9/hermes/lzador/calculater.c` & `Finance-Hermes-0.3.0/hermes/lzador/calculater.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.9/hermes/lzador/calculater.pyx` & `Finance-Hermes-0.3.0/hermes/lzador/calculater.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.9/setup.py` & `Finance-Hermes-0.3.0/setup.py`

 * *Files identical despite different names*

