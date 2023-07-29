# Comparing `tmp/wwpdb.apps.editormodule-0.17.1.tar.gz` & `tmp/wwpdb.apps.editormodule-0.17.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.editormodule-0.17.1.tar", last modified: Tue Jun 27 12:59:41 2023, max compression
+gzip compressed data, was "wwpdb.apps.editormodule-0.17.2.tar", last modified: Sat Jul 29 12:28:50 2023, max compression
```

## Comparing `wwpdb.apps.editormodule-0.17.1.tar` & `wwpdb.apps.editormodule-0.17.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.219041 wwpdb.apps.editormodule-0.17.1/
--rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/LICENSE
--rwxr-xr-x   0 vsts      (1001) docker     (123)      110 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      759 2023-06-27 12:59:41.219041 wwpdb.apps.editormodule-0.17.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       51 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-27 12:59:41.219041 wwpdb.apps.editormodule-0.17.1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2209 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.211041 wwpdb.apps.editormodule-0.17.1/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.211041 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.211041 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/
--rw-r--r--   0 vsts      (1001) docker     (123)      152 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.215041 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      290 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/AccessConfigCifFiles.py
--rw-r--r--   0 vsts      (1001) docker     (123)      170 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/AccessTemplateFiles.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7792 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/EditorConfig.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)   144958 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif
--rw-r--r--   0 vsts      (1001) docker     (123)   212034 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.215041 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/depict/
--rwxr-xr-x   0 vsts      (1001) docker     (123)    52449 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/depict/EditorDepict.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.215041 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/
--rw-r--r--   0 vsts      (1001) docker     (123)     4873 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/EditorDataImport.py
--rw-r--r--   0 vsts      (1001) docker     (123)   163711 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/PdbxDataIo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8061 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1616 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.219041 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/
--rw-r--r--   0 vsts      (1001) docker     (123)     6211 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html
--rw-r--r--   0 vsts      (1001) docker     (123)      641 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html
--rw-r--r--   0 vsts      (1001) docker     (123)    13947 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html
--rw-r--r--   0 vsts      (1001) docker     (123)    17945 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html
--rw-r--r--   0 vsts      (1001) docker     (123)    15904 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html
--rw-r--r--   0 vsts      (1001) docker     (123)     3502 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_prototyping.html
--rw-r--r--   0 vsts      (1001) docker     (123)     2470 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.219041 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/webapp/
--rw-r--r--   0 vsts      (1001) docker     (123)    79034 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/webapp/EditorWebApp.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)    10750 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/webapp/WebRequest.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.211041 wwpdb.apps.editormodule-0.17.1/wwpdb.apps.editormodule.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      759 2023-06-27 12:59:41.000000 wwpdb.apps.editormodule-0.17.1/wwpdb.apps.editormodule.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1637 2023-06-27 12:59:41.000000 wwpdb.apps.editormodule-0.17.1/wwpdb.apps.editormodule.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-27 12:59:41.000000 wwpdb.apps.editormodule-0.17.1/wwpdb.apps.editormodule.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-27 12:59:28.000000 wwpdb.apps.editormodule-0.17.1/wwpdb.apps.editormodule.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      162 2023-06-27 12:59:41.000000 wwpdb.apps.editormodule-0.17.1/wwpdb.apps.editormodule.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-27 12:59:41.000000 wwpdb.apps.editormodule-0.17.1/wwpdb.apps.editormodule.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:28:50.889693 wwpdb.apps.editormodule-0.17.2/
+-rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/LICENSE
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      110 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      759 2023-07-29 12:28:50.889693 wwpdb.apps.editormodule-0.17.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       51 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-29 12:28:50.889693 wwpdb.apps.editormodule-0.17.2/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2209 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:28:50.885693 wwpdb.apps.editormodule-0.17.2/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:28:50.885693 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:28:50.885693 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/
+-rw-r--r--   0 vsts      (1001) docker     (123)      152 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:28:50.885693 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      290 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/config/AccessConfigCifFiles.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      170 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/config/AccessTemplateFiles.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7741 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/config/EditorConfig.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   144958 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif
+-rw-r--r--   0 vsts      (1001) docker     (123)   212034 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:28:50.885693 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/depict/
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    52449 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/depict/EditorDepict.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:28:50.885693 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/io/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4873 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/io/EditorDataImport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   163711 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/io/PdbxDataIo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8061 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1616 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:28:50.889693 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/templates/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6211 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      641 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html
+-rw-r--r--   0 vsts      (1001) docker     (123)    13947 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html
+-rw-r--r--   0 vsts      (1001) docker     (123)    17945 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html
+-rw-r--r--   0 vsts      (1001) docker     (123)    15904 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     3502 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/templates/editor_prototyping.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     2470 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:28:50.889693 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (123)    79034 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/webapp/EditorWebApp.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    10750 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/webapp/WebRequest.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:27:49.000000 wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:28:50.885693 wwpdb.apps.editormodule-0.17.2/wwpdb.apps.editormodule.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      759 2023-07-29 12:28:50.000000 wwpdb.apps.editormodule-0.17.2/wwpdb.apps.editormodule.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1637 2023-07-29 12:28:50.000000 wwpdb.apps.editormodule-0.17.2/wwpdb.apps.editormodule.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-29 12:28:50.000000 wwpdb.apps.editormodule-0.17.2/wwpdb.apps.editormodule.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-29 12:28:38.000000 wwpdb.apps.editormodule-0.17.2/wwpdb.apps.editormodule.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      162 2023-07-29 12:28:50.000000 wwpdb.apps.editormodule-0.17.2/wwpdb.apps.editormodule.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-07-29 12:28:50.000000 wwpdb.apps.editormodule-0.17.2/wwpdb.apps.editormodule.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.editormodule-0.17.1/LICENSE` & `wwpdb.apps.editormodule-0.17.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.1/PKG-INFO` & `wwpdb.apps.editormodule-0.17.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.editormodule
-Version: 0.17.1
+Version: 0.17.2
 Summary: wwPDB mmCIF form editor module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_editormodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.editormodule-0.17.1/setup.py` & `wwpdb.apps.editormodule-0.17.2/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/EditorConfig.py` & `wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/config/EditorConfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,14 @@
     arrReadOnlyCtgries = [
         "pdbx_chem_comp_depositor_info",
         "pdbx_chem_comp_instance_depositor_info",
         "pdbx_chem_comp_upload_depositor_info",
         "pdbx_entity_src_gen_depositor_info",
         "pdbx_helical_symmetry_depositor_info",
         "pdbx_point_symmetry_depositor_info",
-        "pdbx_struct_assembly_gen_depositor_info",
         "pdbx_struct_assembly_prop_depositor_info",
         "pdbx_struct_oper_list_depositor_info",
         "pdbx_struct_ref_seq_depositor_info",
         "pdbx_struct_ref_seq_dif_depositor_info",
         "struct_ref",
         "struct_ref_seq",
     ]
```

### Comparing `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif` & `wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif` & `wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/depict/EditorDepict.py` & `wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/depict/EditorDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/EditorDataImport.py` & `wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/io/EditorDataImport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/PdbxDataIo.py` & `wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/io/PdbxDataIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py` & `wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py` & `wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html` & `wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html` & `wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html` & `wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html` & `wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html` & `wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_prototyping.html` & `wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/templates/editor_prototyping.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html` & `wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/webapp/EditorWebApp.py` & `wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/webapp/EditorWebApp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/webapp/WebRequest.py` & `wwpdb.apps.editormodule-0.17.2/wwpdb/apps/editormodule/webapp/WebRequest.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.1/wwpdb.apps.editormodule.egg-info/PKG-INFO` & `wwpdb.apps.editormodule-0.17.2/wwpdb.apps.editormodule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.editormodule
-Version: 0.17.1
+Version: 0.17.2
 Summary: wwPDB mmCIF form editor module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_editormodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.editormodule-0.17.1/wwpdb.apps.editormodule.egg-info/SOURCES.txt` & `wwpdb.apps.editormodule-0.17.2/wwpdb.apps.editormodule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

