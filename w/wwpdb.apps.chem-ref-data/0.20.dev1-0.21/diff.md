# Comparing `tmp/wwpdb.apps.chem_ref_data-0.20.dev1.tar.gz` & `tmp/wwpdb.apps.chem_ref_data-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.chem_ref_data-0.20.dev1.tar", last modified: Sun Apr 23 20:18:27 2023, max compression
+gzip compressed data, was "wwpdb.apps.chem_ref_data-0.21.tar", last modified: Sat Jul 29 12:32:13 2023, max compression
```

## Comparing `wwpdb.apps.chem_ref_data-0.20.dev1.tar` & `wwpdb.apps.chem_ref_data-0.21.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.749084 wwpdb.apps.chem_ref_data-0.20.dev1/
--rw-r--r--   0 vsts      (1001) docker     (123)      754 2023-04-23 20:18:27.749084 wwpdb.apps.chem_ref_data-0.20.dev1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       92 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-04-23 20:18:27.749084 wwpdb.apps.chem_ref_data-0.20.dev1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2528 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.741084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.741084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.741084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/
--rw-r--r--   0 vsts      (1001) docker     (123)       57 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.741084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/depict/
--rw-r--r--   0 vsts      (1001) docker     (123)     8619 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4349 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepictBootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.741084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/io/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.745084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/
--rw-r--r--   0 vsts      (1001) docker     (123)     8147 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/BirdReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5517 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/ChemCompReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)    26735 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/ChemRefReportDepictBootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3626 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/ReportUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.745084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/
--rw-r--r--   0 vsts      (1001) docker     (123)    19650 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemCompSearchIndexUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)      672 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearch.py
--rw-r--r--   0 vsts      (1001) docker     (123)    26652 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchBase.py
--rw-r--r--   0 vsts      (1001) docker     (123)    27353 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDef.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19563 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDepictBootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7816 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDuplicates.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2485 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/MiscUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.745084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)    18237 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataCvsUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11314 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbExec.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16203 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    28016 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataMiscUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3671 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/DownloadUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1111 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/OSVersion.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.749084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/webapp/
--rw-r--r--   0 vsts      (1001) docker     (123)    48578 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/webapp/ChemRefDataWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.741084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      754 2023-04-23 20:18:27.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1749 2023-04-23 20:18:27.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-23 20:18:27.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-23 20:18:09.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      336 2023-04-23 20:18:27.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-04-23 20:18:27.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:32:13.138862 wwpdb.apps.chem_ref_data-0.21/
+-rw-r--r--   0 vsts      (1001) docker     (123)      749 2023-07-29 12:32:13.138862 wwpdb.apps.chem_ref_data-0.21/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       92 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-29 12:32:13.138862 wwpdb.apps.chem_ref_data-0.21/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2528 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:32:13.126862 wwpdb.apps.chem_ref_data-0.21/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:32:13.130862 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:32:13.130862 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/
+-rw-r--r--   0 vsts      (1001) docker     (123)       57 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:32:13.130862 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/depict/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8619 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4349 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepictBootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:32:13.130862 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/io/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:32:13.130862 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/report/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8147 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/report/BirdReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5517 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/report/ChemCompReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    32306 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/report/ChemRefReportDepictBootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3626 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/report/ReportUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/report/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:32:13.134862 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/search/
+-rw-r--r--   0 vsts      (1001) docker     (123)    19650 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/search/ChemCompSearchIndexUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      672 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/search/ChemRefSearch.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    26693 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/search/ChemRefSearchBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    27353 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/search/ChemRefSearchDef.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19563 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/search/ChemRefSearchDepictBootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7816 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/search/ChemRefSearchDuplicates.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2485 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/search/MiscUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/search/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:32:13.138862 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18235 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/utils/ChemRefDataCvsUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11314 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbExec.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16203 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    28056 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/utils/ChemRefDataMiscUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3671 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/utils/DownloadUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1111 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/utils/OSVersion.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:32:13.138862 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (123)    48963 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/webapp/ChemRefDataWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-29 12:30:28.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:32:13.126862 wwpdb.apps.chem_ref_data-0.21/wwpdb.apps.chem_ref_data.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      749 2023-07-29 12:32:12.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb.apps.chem_ref_data.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1749 2023-07-29 12:32:13.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb.apps.chem_ref_data.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-29 12:32:12.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb.apps.chem_ref_data.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-29 12:31:58.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb.apps.chem_ref_data.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      336 2023-07-29 12:32:12.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb.apps.chem_ref_data.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-07-29 12:32:12.000000 wwpdb.apps.chem_ref_data-0.21/wwpdb.apps.chem_ref_data.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/PKG-INFO` & `wwpdb.apps.chem_ref_data-0.21/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.chem_ref_data
-Version: 0.20.dev1
+Version: 0.21
 Summary: wwPDB chemical reference admin application
 Home-page: https://github.com/rcsb/py-wwpdb_apps_chem_ref_data
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/setup.py` & `wwpdb.apps.chem_ref_data-0.21/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepict.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepictBootstrap.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepictBootstrap.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/BirdReport.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/report/BirdReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/ChemCompReport.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/report/ChemCompReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/ChemRefReportDepictBootstrap.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/report/ChemRefReportDepictBootstrap.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Date:  18-Feb-2013  Jdw
 #
 # Updates:
 #   2-Jun-2017 jdw add NGL viewer
 #   3-Jun-2017 jdw fix CSS for NGL panes & missing
 #  14-Jun-3017 jdw generalize the handling of coordinate files -
 #                  change markup of tabbable section to toggle and resist jump scrolling -
+#   Jun-2023 james smith add at-a-glance tab
 ##
 """
 Create tabular HTML reports from chemical reference definitions.
 
 This version uses Bootstrap CSS framework constructs.
 
 """
@@ -18,15 +19,17 @@
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Creative Commons Attribution 3.0 Unported"
 __version__ = "V0.01"
 
 import sys
 import random
-from wwpdb.apps.chem_ref_data.depict.ChemRefDataDepictBootstrap import ChemRefDataDepictBootstrap
+from wwpdb.apps.chem_ref_data.depict.ChemRefDataDepictBootstrap import (
+    ChemRefDataDepictBootstrap,
+)
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class ChemRefReportDepictBootstrap(ChemRefDataDepictBootstrap):
@@ -66,44 +69,62 @@
                 ("pdbx_chem_comp_audit", "audit", "row-wise"),
             ]
         elif self.__st.getStyleId() in ["BIRD_V1"]:
             self.__reportCategories = [
                 ("pdbx_reference_molecule_list", "molecule_list", "row-wise"),
                 ("pdbx_reference_molecule_family", "molecule_family", "row-wise"),
                 ("pdbx_reference_molecule_synonyms", "molecule_synonyms", "row-wise"),
-                ("pdbx_reference_molecule_annotation", "molecule_annotation", "row-wise"),
+                (
+                    "pdbx_reference_molecule_annotation",
+                    "molecule_annotation",
+                    "row-wise",
+                ),
                 ("pdbx_reference_molecule_features", "molecule_features", "row-wise"),
-                ("pdbx_reference_molecule_related_structures", "molecule_related_structures", "row-wise"),
+                (
+                    "pdbx_reference_molecule_related_structures",
+                    "molecule_related_structures",
+                    "row-wise",
+                ),
                 ("pdbx_reference_molecule_details", "details", "row-wise"),
                 ("citation", "citation", "row-wise"),
                 ("citation_author", "citation_author", "row-wise"),
                 ("pdbx_family_prd_audit", "family_prd_audit", "row-wise"),
                 #
                 ("pdbx_reference_molecule", "molecule", "column-wise"),
                 ("pdbx_reference_entity_list", "entity_list", "row-wise"),
                 ("pdbx_reference_entity_src_nat", "entity_src_nat", "row-wise"),
                 ("pdbx_reference_entity_poly", "entity_poly", "row-wise"),
                 ("pdbx_reference_entity_poly_seq", "entity_poly_seq", "row-wise"),
                 ("pdbx_reference_entity_sequence", "entity_sequence", "row-wise"),
-                ("pdbx_reference_entity_sequence_list", "entity_sequence_list", "row-wise"),
-                ("pdbx_reference_entity_subcomponents", "entity_subcomponents", "row-wise"),
+                (
+                    "pdbx_reference_entity_sequence_list",
+                    "entity_sequence_list",
+                    "row-wise",
+                ),
+                (
+                    "pdbx_reference_entity_subcomponents",
+                    "entity_subcomponents",
+                    "row-wise",
+                ),
                 ("pdbx_reference_entity_nonpoly", "entity_nonpoly", "row-wise"),
                 ("pdbx_reference_entity_link", "entity_link", "row-wise"),
                 ("pdbx_reference_entity_poly_link", "entity_poly_link", "row-wise"),
                 ("pdbx_prd_audit", "prd_audit", "row-wise"),
             ]
 
     def render(self, eD, style="tabs"):
         """ """
         if style in ["tabs"]:
             return self.__doRenderTabs(eD)
         elif style in ["accordion", "multiaccordion"]:
             return self.__doRenderAccordion(eD)
         else:
-            return self.__doRenderPage(eD)  # Due to missing inheritance, and eD variable was missing - never come through here
+            return self.__doRenderPage(
+                eD
+            )  # Due to missing inheritance, and eD variable was missing - never come through here
 
     def __doRenderTabs(self, eD):
         """Render a tabbed table set.
 
         Bootstrap markup template  --
 
         <div class="tabbable"> <!-- Only required for left/right tabs -->
@@ -125,96 +146,176 @@
         """
 
         idPrefix = "tab" + str(random.randint(0, 100000))
         catList = self.__reportCategories
         #
         if self.__debug:
             for ii, tup in enumerate(catList):
-                logger.debug("ChemRefReportDepict (doRenderTabs) ii %d  tup %r", ii, tup)
+                logger.debug(
+                    "ChemRefReportDepict (doRenderTabs) ii %d  tup %r", ii, tup
+                )
             for ii, (x, y, z) in enumerate(catList):
-                logger.debug("ChemRefReportDepict (doRenderTabs) ii %d  values  %s %s %s", ii, x, y, z)
+                logger.debug(
+                    "ChemRefReportDepict (doRenderTabs) ii %d  values  %s %s %s",
+                    ii,
+                    x,
+                    y,
+                    z,
+                )
         #
         oL = []
         #
         # need for URL construction --
         cD = eD["dataDict"]
         idCode = eD["idCode"]
         #
         #
         # Write the tabs --
         #
-        oL.append('<div id="%s_report_section" class="tabbable results-section">' % idCode)
+        oL.append(
+            '<div id="%s_report_section" class="tabbable results-section">' % idCode
+        )
         # add close/dismiss --
-        oL.append('<button type="button" class="close" data-target="#%s_report_section" data-dismiss="alert" style="margin:7px; padding:1px;> ' % idCode)
-        oL.append('   <span aria-hidden="true"> <i class="fa fa-times"></i></span><span class="sr-only">Close</span></button>')
+        oL.append(
+            '<button type="button" class="close" data-target="#%s_report_section" data-dismiss="alert" style="margin:7px; padding:1px;"> '
+            % idCode
+        )
+        oL.append(
+            '   <span aria-hidden="true"> <i class="fa fa-times"></i></span><span class="sr-only">Close</span></button>'
+        )
 
         oL.append('<ul class="nav nav-tabs">')
-        oL.append('<li><a  class="active" data-target="#%s-tabs-id" data-toggle="tab">%s' % (idPrefix, idCode))
-        oL.append('   <span aria-hidden="true"> <i class="fa fa-compress"></i></span><span class="sr-only">Close</span></a></li>')
+        oL.append(
+            '<li><a  class="active" data-target="#%s-tabs-id" data-toggle="tab">%s'
+            % (idPrefix, idCode)
+        )
+        oL.append(
+            '   <span aria-hidden="true"> <i class="fa fa-compress"></i></span><span class="sr-only">Close</span></a></li>'
+        )
         iSection = 0
         for ii, (catName, catNameAbbrev, catStyle) in enumerate(catList):
             # For only popuated categories
             if catName in cD and (len(cD[catName]) > 0):
-                oL.append('<li><a data-target="#%s-tabs-%d" data-toggle="tab">%s</a></li>' % (idPrefix, ii, catNameAbbrev))
+                oL.append(
+                    '<li><a data-target="#%s-tabs-%d" data-toggle="tab">%s</a></li>'
+                    % (idPrefix, ii, catNameAbbrev)
+                )
                 iSection = ii
         #
         if eD["imageRelativePath"] is not None:
-            oL.append('<li><a data-target="#%s-tabs-%d" data-toggle="tab">%s</a></li>' % (idPrefix, iSection + 1, "2D"))
+            oL.append(
+                '<li><a data-target="#%s-tabs-%d" data-toggle="tab">%s</a></li>'
+                % (idPrefix, iSection + 1, "2D")
+            )
         if eD["xyzRelativePath"] is not None:
-            oL.append('<li><a data-target="#%s-tabs-%d" data-toggle="tab" class="ngl-section-%s">%s</a></li>' % (idPrefix, iSection + 2, idCode, "3D"))
+            oL.append(
+                '<li><a data-target="#%s-tabs-%d" data-toggle="tab" class="jsmol-section-%s">%s</a></li>'
+                % (idPrefix, iSection + 2, idCode, "3D")
+            )
+        # at-a-glance for 3-or-5-letter cc id
+        if (
+            eD["imageRelativePath"] is not None
+            and eD["xyzRelativePath"] is not None
+            and (len(idCode) == 3 or len(idCode) == 5)
+        ):
+            oL.append(
+                '<li><a data-target="#%s-tabs-%d" data-toggle="tab" class="ataglance-section-%s">%s</a></li>'
+                % (idPrefix, iSection + 3, idCode, "at-a-glance")
+            )
+
         oL.append("</ul>")
         #
         # Write the tables --
         #
         oL.append('<div  class="tab-content"> ')
         #
         oL.append('<div class="tab-pane active"  id="%s-tabs-id"></div>' % (idPrefix))
 
         iSection = 0
         for ii, (catName, catNameAbbrev, catStyle) in enumerate(catList):
             # For only popuated categories
             if catName in cD and (len(cD[catName]) > 0):
                 oL.append('<div class="tab-pane"  id="%s-tabs-%d">' % (idPrefix, ii))
-                oL.append('<table class="table table-striped table-bordered table-condensed" id="%s-%s">' % (idPrefix, catName))
+                oL.append(
+                    '<table class="table table-striped table-bordered table-condensed" id="%s-%s">'
+                    % (idPrefix, catName)
+                )
                 if catStyle == "column-wise":
                     self.__renderTableColumnWise(catName, cD[catName][0], oL)
                 else:
                     self.__renderTableRowWise(catName, cD[catName], oL)
 
                 oL.append("</table>")
                 oL.append("</div>")
                 iSection = ii
         #  2D image
         if eD["imageRelativePath"] is not None:
-            oL.append('<div class="tab-pane"  id="%s-tabs-%d">' % (idPrefix, iSection + 1))
-            oL.append('<img src="%s" alt="%s" height="%d" width="%d">' % (eD["imageRelativePath"], idCode, 700, 700))
+            oL.append(
+                '<div class="tab-pane"  id="%s-tabs-%d">' % (idPrefix, iSection + 1)
+            )
+            oL.append(
+                '<img src="%s" alt="%s" height="%d" width="%d">'
+                % (eD["imageRelativePath"], idCode, 700, 700)
+            )
             oL.append("</div>")
 
         # 3D app
         if eD["xyzRelativePath"] is not None:
             hasExpt = eD["hasExpt"]
             hasIdeal = eD["hasIdeal"]
-            oL.append('<div class="tab-pane ngl-class-expt-%s ngl-class-ideal-%s" data-payload="%s" id="%s-tabs-%d">' % (idCode, idCode, idCode, idPrefix, iSection + 2))
+            oL.append(
+                '<div style="overflow:visible;" class="tab-pane jsmol-class-expt-%s jsmol-class-ideal-%s" data-payload="%s" id="%s-tabs-%d">'
+                % (idCode, idCode, idCode, idPrefix, iSection + 2)
+            )
 
-            oL.append('<div class="row">')
+            oL.append('<div style="display:flex;">')
             #             # h5 is ~15px + 20 vert margin
             if hasExpt:
-                oL.append('  <div style="display:inline-block; float:left; border: 2px solid lightgray; width:645px; height:645px; margin:2px; padding:1px; ">')
-                oL.append('     <h5 class="text-center">Experimental Coordinate Data</h5>')
-                oL.append('     <div id="%s_ngl_expt"  style="width:600px; height:600px;"></div>' % idCode)
+                oL.append(
+                    '  <div id="%s_jsmol_expt" style="display:inline-block; float:left; border: 2px solid lightgray; width:645px; height:645px; margin:2px; padding:1px; ">'
+                    % idCode
+                )
                 oL.append("  </div>")
             if hasIdeal:
-                oL.append('  <div style="display:inline-block; float:left; border: 2px solid lightgray; width:645px; height:645px; margin:2px; padding:1px; ">')
-                oL.append('    <h5 class="text-center">Ideal Coordinate Data</h5>')
-                oL.append('    <div id="%s_ngl_ideal" style=" width:600px; height:600px;"></div>' % idCode)
+                oL.append(
+                    '  <div id="%s_jsmol_ideal" style="display:inline-block; float:left; border: 2px solid lightgray; width:645px; height:645px; margin:2px; padding:1px; ">'
+                    % idCode
+                )
                 oL.append("  </div>")
 
             oL.append("</div>")
 
             oL.append("</div>")
+
+        # At-a-glance for 3-or-5-letter cc id
+        if (
+            eD["imageRelativePath"] is not None
+            and eD["xyzRelativePath"] is not None
+            and (len(idCode) == 3 or len(idCode) == 5)
+        ):
+            oL.append(
+                '<div style="padding:10px;background-color:white;overflow:visible;" class="tab-pane tab-flex" id="%s-tabs-%d">'
+                % (idPrefix, iSection + 3)
+            )
+            oL.append(
+                '<table style="margin-right:20px;position:relative;display:inline-table;width:100ch;" id="%s-%s">'
+                % (idPrefix, "chem_comp")
+            )
+            self.__renderTableAtAGlance("chem_comp", cD["chem_comp"][0], oL)
+            oL.append("</table>")
+            oL.append(
+                '<img style="position:relative;display:inline-table;border:1px solid gray;" src="%s" alt="%s" height="%d" width="%d">'
+                % (eD["imageRelativePath"], idCode, 500, 500)
+            )
+            oL.append(
+                '<div id="%s_ataglance_ideal" style="position:relative;display:inline-table;border:1px solid lightgray;width:500px;height:500px;">'
+                % idCode
+            )
+            oL.append("</div>")
+            oL.append("</div>")
         #
         oL.append("</div>")
         oL.append("</div>")
         #
         return oL
 
     def __doRenderAccordion(self, eD):
@@ -264,20 +365,28 @@
         for ii, (catName, catNameAbbrev, catStyle) in enumerate(catList):
             # For only popuated categories
             if catName in cD and (len(cD[catName]) > 0):
                 active = "in" if isFirst else ""
                 idSection = idPrefix + "-sec-" + str(ii)
                 oL.append('<div class="accordion-group">')
                 oL.append('<div class="accordion-heading">')
-                oL.append('<a class="accordion-toggle" data-toggle="collapse" data-parent="#%s" href="#%s">%s</a>' % (idTop, idSection, catNameAbbrev))
+                oL.append(
+                    '<a class="accordion-toggle" data-toggle="collapse" data-parent="#%s" href="#%s">%s</a>'
+                    % (idTop, idSection, catNameAbbrev)
+                )
                 oL.append("</div>")
-                oL.append('<div id="%s" class="accordion-body collapse %s">' % (idSection, active))
+                oL.append(
+                    '<div id="%s" class="accordion-body collapse %s">'
+                    % (idSection, active)
+                )
                 oL.append('<div  class="accordion-inner">')
                 #
-                oL.append('<table class="table table-striped table-bordered table-condensed">')
+                oL.append(
+                    '<table class="table table-striped table-bordered table-condensed">'
+                )
                 if catStyle == "column-wise":
                     self.__renderTableColumnWise(catName, cD[catName][0], oL)
                 else:
                     self.__renderTableRowWise(catName, cD[catName], oL)
                 oL.append("</table>")
                 #
                 oL.append("</div>")
@@ -309,37 +418,46 @@
         oL.append("<br/>")
 
         #
         cD = eD["dataDict"]
 
         for catName in ["chem_comp"]:
             if catName in cD and (len(cD[catName]) > 0):
-
                 oL.append('<div class="sectionbar1">')
-                oL.append('  <a class="sectionbar1" href="" id="toggle_section_%s">Show</a> Category: %s' % (catName, catName))
+                oL.append(
+                    '  <a class="sectionbar1" href="" id="toggle_section_%s">Show</a> Category: %s'
+                    % (catName, catName)
+                )
                 oL.append("</div>")
 
-                oL.append('<div style="display: block;" id="d_%s" class="displaynone">' % catName)
+                oL.append(
+                    '<div style="display: block;" id="d_%s" class="displaynone">'
+                    % catName
+                )
                 oL.append('<table id="%s">' % catName)
                 self.__renderTableColumnWise(catName, cD[catName][0], oL)
                 oL.append("</table>")
                 oL.append("</div>")
         #
         # <div class="sb0"><a class="sb0" href="" id="toggle_section_XXXX">Show</a></div> <div class="sb1">Category:  Entity Reference</div>
         #
         for catName in tableList:
             if catName in cD and (len(cD[catName]) > 0):
-
                 oL.append('<div class="sb0">')
-                oL.append('  <a class="sb0" href="" id="toggle_section_%s">Show</a>' % catName)
+                oL.append(
+                    '  <a class="sb0" href="" id="toggle_section_%s">Show</a>' % catName
+                )
                 oL.append("</div>")
                 oL.append('<div class="sb1">Category: %s </div>' % catName)
                 oL.append("<br />")
 
-                oL.append('<div style="display: block;" id="d_%s" class="displaynone">' % catName)
+                oL.append(
+                    '<div style="display: block;" id="d_%s" class="displaynone">'
+                    % catName
+                )
                 oL.append('<table id="%s">' % catName)
                 if catName in ["pdbx_reference_molecule"]:
                     self.__renderTableColumnWise(catName, cD[catName][0], oL)
                 else:
                     self.__renderTableRowWise(catName, cD[catName], oL)
                 oL.append("</table>")
                 oL.append("</div>")
@@ -355,16 +473,15 @@
         to the left of column values.
         """
 
         #
         iCol = 0
         self.__markupRow(catName, rD)
         #
-        for (itemName, itemDefault) in self.__st.getItemNameAndDefaultList(catName):
-
+        for itemName, itemDefault in self.__st.getItemNameAndDefaultList(catName):
             if itemName in rD:
                 itemValue = rD[itemName]
             else:
                 itemValue = itemDefault
 
             oL.append("<tr>")
             oL.append("<td>%s</td>" % self.__attributePart(itemName))
@@ -387,19 +504,58 @@
         for row in rL:
             self.__markupRow(catName, row)
             self.__renderRow(catName, row, iRow, oL, insertDefault=False)
             iRow += 1
         #
         #
 
-    def __renderRow(self, catName, row, iRow, oL, insertDefault=False):  # pylint: disable=unused-argument
+    def __renderTableAtAGlance(self, catName, rD, oL):
+        """One-column rendering"""
+        #
+        # iCol = 0
+        self.__markupRow(catName, rD)
+        #
+        lst = self.__st.getItemNameAndDefaultList(catName)
+        d = {k: v for k, v in lst}
+        # reorder keys for at-a-glance
+        keys = [
+            ("_chem_comp.id", "ID"),
+            ("_chem_comp.pdbx_release_status", "Status"),
+            ("_chem_comp.name", "Name"),
+            ("_chem_comp.pdbx_synonyms", "Synonyms"),
+            ("_chem_comp.formula", "Formula"),
+            ("_chem_comp.formula_weight", "Formula weight"),
+            ("_chem_comp.pdbx_formal_charge", "Formal charge"),
+            ("_chem_comp.type", "Type"),
+            ("_chem_comp.pdbx_type", "Pdbx_type"),
+            ("_chem_comp.mon_nstd_parent_comp_id", "Parent"),
+            ("_chem_comp.pdbx_subcomponent_list", "Subcomponents"),
+            ("_chem_comp.pdbx_replaces", "Replace"),
+            ("_chem_comp.pdbx_replaced_by", "Replace by"),
+            (
+                "_chem_comp.pdbx_model_coordinates_missing_flag",
+                "Model coordinates missing",
+            ),
+            ("_chem_comp.pdbx_model_coordinates_db_code", "Model PDB code"),
+            ("_chem_comp.pdbx_initial_date", "Initial date"),
+            ("_chem_comp.pdbx_modified_date", "Modified date"),
+            ("_chem_comp.pdbx_processing_site", "Site"),
+        ]
+        for k, v in keys:
+            oL.append("<tr>")
+            oL.append("<td>%s:&nbsp%s</td>" % (v, rD[k] if k in rD else d[k]))
+            oL.append("</tr>")
+
+    def __renderRow(
+        self, catName, row, iRow, oL, insertDefault=False
+    ):  # pylint: disable=unused-argument
         """Render a row in a multirow table."""
         oL.append("<tr>")
         #
-        for (itemName, itemDefault) in self.__st.getItemNameAndDefaultList(catName):
+        for itemName, itemDefault in self.__st.getItemNameAndDefaultList(catName):
             if insertDefault:
                 itemValue = itemDefault
             elif itemName in row:
                 itemValue = row[itemName]
             else:
                 itemValue = itemDefault
 
@@ -412,25 +568,36 @@
         #
         rst = cVal
         try:
             if cName in ["family", "prd"]:
                 rst = '<a class="app-ref-report"  href="#">%s</a>' % cVal
             elif cName in ["cc"]:
                 rpt = '<a class="app-ref-report"  href="#">%s</a>' % cVal
-                le = '<a target="_blank" href="http://ligand-expo.rcsb.org/pyapps/ldHandler.py?formid=cc-index-search&operation=ccid&target=%s">(LE)</a>' % cVal
+                le = (
+                    '<a target="_blank" href="http://ligand-expo.rcsb.org/pyapps/ldHandler.py?formid=cc-index-search&operation=ccid&target=%s">(LE)</a>'
+                    % cVal
+                )
                 rst = "%s &nbsp; %s" % (rpt, le)
             elif cName in ["id"]:
                 if cVal.startswith("PRD_") or cVal.startswith("FAM_"):
                     rst = '<a class="app-ref-report"  href="#">%s</a>' % cVal
                 else:
                     rpt = '<a class="app-ref-report"  href="#">%s</a>' % cVal
-                    le = '<a target="_blank" href="http://ligand-expo.rcsb.org/pyapps/ldHandler.py?formid=cc-index-search&operation=ccid&target=%s">(LE)</a>' % cVal
+                    le = (
+                        '<a target="_blank" href="http://ligand-expo.rcsb.org/pyapps/ldHandler.py?formid=cc-index-search&operation=ccid&target=%s">(LE)</a>'
+                        % cVal
+                    )
                     rst = "%s &nbsp; %s" % (rpt, le)
         except Exception as e:
-            logger.info("ChemRefReportDepict (markuplinks) failing cName %r cVal %r %r", cName, cVal, str(e))
+            logger.info(
+                "ChemRefReportDepict (markuplinks) failing cName %r cVal %r %r",
+                cName,
+                cVal,
+                str(e),
+            )
             logger.exception("Failure in __markupLinks")
         return rst
 
     def __markupRow(self, catName, rD):
         """Markup a row (row dictionary) in the input category."""
         if catName == "pdbx_reference_molecule_list":
             itemName = "_pdbx_reference_molecule_list.prd_id"
@@ -463,50 +630,87 @@
         if catName == "pdbx_reference_molecule_details":
             itemName1 = "_pdbx_reference_molecule_details.source"
             itemName2 = "_pdbx_reference_molecule_details.source_id"
             if itemName1 in rD:
                 srcType = str(rD[itemName1]).upper()
                 srcValue = rD[itemName2]
                 if srcType == "DOI" and len(srcValue) > 2:
-                    rD[itemName2] = '<a target="_blank" href="http://dx.doi.org/%s">%s</a>' % (srcValue, srcValue)
+                    rD[
+                        itemName2
+                    ] = '<a target="_blank" href="http://dx.doi.org/%s">%s</a>' % (
+                        srcValue,
+                        srcValue,
+                    )
                 if srcType == "PUBMED" and len(srcValue) > 2:
-                    rD[itemName2] = '<a target="_blank" href="http://www.ncbi.nlm.nih.gov/sites/entrez?cmd=search&db=pubmed&term=%s">%s</a>' % (srcValue, srcValue)
+                    rD[itemName2] = (
+                        '<a target="_blank" href="http://www.ncbi.nlm.nih.gov/sites/entrez?cmd=search&db=pubmed&term=%s">%s</a>'
+                        % (srcValue, srcValue)
+                    )
                 if srcType == "DRUGBANK" and len(srcValue) > 2:
-                    rD[itemName2] = '<a target="_blank" href="http://www.drugbank.ca/cgi-bin/getCard.cgi?CARD=%s">%s</a>' % (srcValue, srcValue)
+                    rD[itemName2] = (
+                        '<a target="_blank" href="http://www.drugbank.ca/cgi-bin/getCard.cgi?CARD=%s">%s</a>'
+                        % (srcValue, srcValue)
+                    )
                 if srcType == "PUBCHEM" and len(srcValue) > 2:
-                    rD[itemName2] = '<a target="_blank" href="http://pubchem.ncbi.nlm.nih.gov/summary/summary.cgi?cid=%s">%s</a>' % (srcValue, srcValue)
+                    rD[itemName2] = (
+                        '<a target="_blank" href="http://pubchem.ncbi.nlm.nih.gov/summary/summary.cgi?cid=%s">%s</a>'
+                        % (srcValue, srcValue)
+                    )
 
                 if srcType == "URL" and len(srcValue) > 2:
-                    rD[itemName2] = '<a target="_blank" href="%s">%s</a>' % (srcValue, srcValue)
+                    rD[itemName2] = '<a target="_blank" href="%s">%s</a>' % (
+                        srcValue,
+                        srcValue,
+                    )
 
                 if srcType == "PMCID" and len(srcValue) > 2:
-                    rD[itemName2] = '<a target="_blank" href="http://www.ncbi.nlm.nih.gov/pmc/?term=%s">%s</a>' % (srcValue, srcValue)
+                    rD[itemName2] = (
+                        '<a target="_blank" href="http://www.ncbi.nlm.nih.gov/pmc/?term=%s">%s</a>'
+                        % (srcValue, srcValue)
+                    )
 
                 if srcType == "PMC" and len(srcValue) > 2:
-                    rD[itemName2] = '<a target="_blank" href="http://www.ncbi.nlm.nih.gov/pmc/?term=%s">%s</a>' % (srcValue, srcValue)
+                    rD[itemName2] = (
+                        '<a target="_blank" href="http://www.ncbi.nlm.nih.gov/pmc/?term=%s">%s</a>'
+                        % (srcValue, srcValue)
+                    )
 
                 if srcType == "UNIPROT" and len(srcValue) > 2:
-                    rD[itemName2] = '<a target="_blank" href="http://www.uniprot.org/uniprot/%s">%s</a>' % (srcValue, srcValue)
+                    rD[itemName2] = (
+                        '<a target="_blank" href="http://www.uniprot.org/uniprot/%s">%s</a>'
+                        % (srcValue, srcValue)
+                    )
 
         if catName == "citation":
             itemName = "_citation.pdbx_database_id_DOI"
             if itemName in rD and len(rD[itemName]) > 1:
                 itemValue = rD[itemName]
-                rD[itemName] = '<a target="_blank" href="http://dx.doi.org/%s">%s</a>' % (itemValue, itemValue)
+                rD[
+                    itemName
+                ] = '<a target="_blank" href="http://dx.doi.org/%s">%s</a>' % (
+                    itemValue,
+                    itemValue,
+                )
             itemName = "_citation.pdbx_database_id_PubMed"
             if itemName in rD and len(rD[itemName]) > 1:
                 itemValue = rD[itemName]
-                rD[itemName] = '<a target="_blank" href="http://www.ncbi.nlm.nih.gov/sites/entrez?cmd=search&db=pubmed&term=%s">%s</a>' % (itemValue, itemValue)
+                rD[itemName] = (
+                    '<a target="_blank" href="http://www.ncbi.nlm.nih.gov/sites/entrez?cmd=search&db=pubmed&term=%s">%s</a>'
+                    % (itemValue, itemValue)
+                )
 
         if catName == "pdbx_reference_molecule":
             itemName = "_pdbx_reference_molecule.representative_PDB_id_code"
             if itemName in rD:
                 itemValue = rD[itemName]
                 if len(itemValue) > 3:
-                    rD[itemName] = '<a target="_blank" href="http://www.rcsb.org/pdb/explore/explore.do?structureId=%s">%s</a>' % (itemValue, itemValue)
+                    rD[itemName] = (
+                        '<a target="_blank" href="http://www.rcsb.org/pdb/explore/explore.do?structureId=%s">%s</a>'
+                        % (itemValue, itemValue)
+                    )
 
             itemName = "_pdbx_reference_molecule.chem_comp_id"
             if itemName in rD:
                 itemValue = rD[itemName]
                 if len(itemValue) >= 3:
                     rD[itemName] = self.__markupLinks("cc", itemValue)
         if catName == "pdbx_reference_entity_nonpoly":
@@ -526,15 +730,14 @@
                 itemValue = rD[itemName]
                 if len(itemValue) >= 3:
                     rD[itemName] = self.__markupLinks("cc", itemValue)
 
     # ------
 
     def __jQueryReportScript1(self, tableList, eD, oL):
-
         # Context that will get encoded for call back --
         filePath = eD["filePath"]
         localPath = eD["localPath"]
         localRelativePath = eD["localRelativePath"]
         sessionId = eD["sessionId"]
         editOpNumber = eD["editOpNumber"]
         blockId = eD["blockId"]
@@ -575,15 +778,17 @@
         for t in tableList[:-1]:
             tS += "#toggle_section_%s, " % t
         tS += "#toggle_section_%s" % tableList[-1]
 
         oL.append('$("%s").click(function() {' % tS)
         oL.append('        myConsoleLog("TOGGLE VALUE "+$(this).text());')
         # oL.append('        $(this).parents("div").filter(":first").next().toggle(400);')
-        oL.append('        $(this).parents("div").filter(":first").next().next().next().toggle(400);')
+        oL.append(
+            '        $(this).parents("div").filter(":first").next().next().next().toggle(400);'
+        )
         oL.append('        $(this).text($(this).text() == "Show" ? "Hide" : "Show");')
         oL.append("        return false;")
         oL.append(" });")
 
         oL.append(' $(".sb0").corner("round");')
         oL.append(' $(".sb1").corner("round");')
         #
```

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/ReportUtils.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/report/ReportUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemCompSearchIndexUtils.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/search/ChemCompSearchIndexUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearch.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/search/ChemRefSearch.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchBase.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/search/ChemRefSearchBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -592,15 +592,15 @@
             #
             dTitle = self._getSearchDefDisplayTitle(sType)
             if len(dTitle) > 0:
                 searchNameD = dTitle
             else:
                 searchNameD = searchName
             #
-            displayTitle = "Results for: %s <i>%s</i> %s &nbsp;&nbsp; (%d)" % (searchNameD, cTypeD, ",".join(stdSearchTargetList), len(rList))
+            displayTitle = "Results for: %s <i>%s</i> <span class='stdSearchTargetList'>%s</span> &nbsp;&nbsp; (%d)" % (searchNameD, cTypeD, ",".join(stdSearchTargetList), len(rList))
             # oL = []
             sD[rId]["resultlist"] = rList
             sD[rId]["columnList"] = cList
             sD[rId]["columnWidthList"] = wdList
             sD[rId]["searchType"] = sType
             sD[rId]["compareType"] = cType
             sD[rId]["displayTitle"] = displayTitle
```

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDef.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/search/ChemRefSearchDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDepictBootstrap.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/search/ChemRefSearchDepictBootstrap.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDuplicates.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/search/ChemRefSearchDuplicates.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/MiscUtils.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/search/MiscUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataCvsUtils.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/utils/ChemRefDataCvsUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         cvsProjectName = self.__pI.assignCvsProjectName(repType="CC")
         dataS = "ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
         dataList = [(cvsProjectName, a, True) for a in dataS]
 
         # Extended CCD support
         ext_ccd = self.__cIAppCc.get_extended_ccd_supp()
         if ext_ccd:
-            dataList += [("cvsProjectName", a + b, True) for a in dataS for b in dataS]
+            dataList += [(cvsProjectName, a + b, True) for a in dataS for b in dataS]
 
         #
         mpu = MultiProcUtil(verbose=self.__debug)
         mpu.set(workerObj=self.__vc, workerMethod="updateList")
         ok, failList, _resultList, diagList = mpu.runMulti(dataList=dataList, numProc=numProc)
         endTime = time.time()
         if self.__verbose:
```

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbExec.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbExec.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbUtils.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataMiscUtils.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/utils/ChemRefDataMiscUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,16 @@
 
         tempPath = dstPath + suffix
 
         # Remove from previous round
         if os.path.exists(tempPath):
             os.remove(tempPath)
 
-        os.link(dstPath, tempPath)
+        if os.path.exists(dstPath):
+            os.link(dstPath, tempPath)
 
         os.rename(srcPath, dstPath)
 
     def __makeTempPath(self, inpPath):
         try:
             pid = str(os.getpid())
             return inpPath + pid
```

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/DownloadUtils.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/utils/DownloadUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/OSVersion.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/utils/OSVersion.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/webapp/ChemRefDataWebApp.py` & `wwpdb.apps.chem_ref_data-0.21/wwpdb/apps/chem_ref_data/webapp/ChemRefDataWebApp.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,14 @@
                 rC.setStatus(statusMsg="Reports completed")
                 rC.set("webPathList", webPathList)
                 rC.set("idCodeList", myIdList)
             else:
                 rC.setError(errMsg="Report preparation failed")
 
         elif operation in ["check", "cvsupdate", "cvsadd"]:
-
             logPath = os.path.join(self.__sessionPath, rootName + "-cif-check.log")
             self.__removeFile(logPath)
             hasDiags = self.__makeCifCheckReport(filePath, logPath)
             if hasDiags:
                 du = DownloadUtils(self.__reqObj, verbose=self.__verbose, log=self.__lfh)
                 du.fetchFile(logPath)
                 aTagList.append(du.getAnchorTag())
@@ -705,14 +704,20 @@
         #
         searchTypeInput = self.__reqObj.getValue("searchType")
         searchType, queryType, inputType, compareType = self.__getSearchType(searchTypeInput)
         #
         logger.info(
             "searchType %r queryType %r searchTarget %r inputType %r compareType %r appsHtdocsPath %r", searchType, queryType, searchTarget, inputType, compareType, appsHtdocsPath
         )
+        # enable comma-separated lists or hyphen-separated ranges in search box
+        if searchType.startswith("CCD_CC_ID") or searchType.startswith("BIRD_PRD_ID"):
+            searchTarget = searchTarget.replace(",", " ")
+        elif searchType == "CCD_FORMULA_WEIGHT" or searchType == "CCDIDX_FORMULA_WEIGHT_RANGE":
+            searchTarget = searchTarget.replace("-", " ")
+        #
         self.__getSession()
         self.__reqObj.setReturnFormat(return_format="json")
         rC = ResponseContent(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
 
         #
         rD = {}
         try:
@@ -849,15 +854,14 @@
             return self.__chemRefSupportFileUpdateOp()
         elif operation == "updateindexfiles":
             return self.__chemRefIndexFileUpdateOp()
         else:
             return self.__chemRefSyncCvsOp(repositoryType=None)
 
     def __chemRefSupportFileUpdateOp(self):
-
         self.__getSession()
         logger.info("+ChemRefDataWebAppWorker._chemRefSupportFileUpdateOp() starting with session %s", self.__sessionPath)
 
         self.__reqObj.setReturnFormat(return_format="json")
         rC = ResponseContent(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
 
         ok = self.__chemRefSupportFiles()
@@ -882,15 +886,14 @@
             ok = ok1 and ok2 and ok3
         except:  # noqa: E722 pylint: disable=bare-except
             logger.exception("Failure in __chemRefSupportFiles")
             ok = False
         return ok
 
     def __chemRefIndexFileUpdateOp(self):
-
         self.__getSession()
         logger.info("+ChemRefDataWebAppWorker._chemRefIndexFileUpdateOp() starting with session %s", self.__sessionPath)
 
         self.__reqObj.setReturnFormat(return_format="json")
         rC = ResponseContent(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
 
         ok = self.__chemRefIndexFiles()
@@ -944,15 +947,14 @@
                 hL.append("<br />".join(tL))
 
             rC.setError(errMsg="Repository SYNC completed with diagnostics  <br />" + "<br />".join(hL))
 
         return rC
 
     def __chemRefDatabaseUpdateOp(self, referenceDatabase="CC"):
-
         self.__getSession()
         logger.info("+ChemRefDataWebAppWorker._chemRefDatabaseUpdateOp() starting with session %s", self.__sessionPath)
 
         self.__reqObj.setReturnFormat(return_format="json")
         rC = ResponseContent(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
 
         crdbu = ChemRefDataDbUtils(self.__reqObj, verbose=self.__debug, log=self.__lfh)
```

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/PKG-INFO` & `wwpdb.apps.chem_ref_data-0.21/wwpdb.apps.chem_ref_data.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.chem-ref-data
-Version: 0.20.dev1
+Version: 0.21
 Summary: wwPDB chemical reference admin application
 Home-page: https://github.com/rcsb/py-wwpdb_apps_chem_ref_data
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/SOURCES.txt` & `wwpdb.apps.chem_ref_data-0.21/wwpdb.apps.chem_ref_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

