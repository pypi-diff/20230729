# Comparing `tmp/ukmon_meteortools-2023.7.7.tar.gz` & `tmp/ukmon_meteortools-2023.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukmon_meteortools-2023.7.7.tar", last modified: Sat Jul 29 11:27:23 2023, max compression
+gzip compressed data, was "ukmon_meteortools-2023.7.8.tar", last modified: Sat Jul 29 13:07:51 2023, max compression
```

## Comparing `ukmon_meteortools-2023.7.7.tar` & `ukmon_meteortools-2023.7.8.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 11:27:23.391105 ukmon_meteortools-2023.7.7/
--rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.7.7/LICENSE
--rw-rw-rw-   0        0        0    43083 2023-07-29 11:27:23.390104 ukmon_meteortools-2023.7.7/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.7.7/README.md
--rw-rw-rw-   0        0        0     2826 2023-07-29 11:26:27.000000 ukmon_meteortools-2023.7.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-29 11:27:23.391105 ukmon_meteortools-2023.7.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-29 11:27:23.262109 ukmon_meteortools-2023.7.7/tests/
--rw-rw-rw-   0        0        0     3619 2023-07-28 09:52:46.000000 ukmon_meteortools-2023.7.7/tests/test_apis.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:27:23.271114 ukmon_meteortools-2023.7.7/ukmon_meteortools/
--rw-rw-rw-   0        0        0     1177 2023-07-08 23:13:20.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 11:27:23.318105 ukmon_meteortools-2023.7.7/ukmon_meteortools/fileformats/
--rw-rw-rw-   0        0        0     8762 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/fileformats/UFOAnalyzerXML.py
--rw-rw-rw-   0        0        0     6211 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/fileformats/UFOCapXML.py
--rw-rw-rw-   0        0        0      664 2023-05-08 13:19:19.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/fileformats/__init__.py
--rw-rw-rw-   0        0        0    18716 2023-05-08 11:58:38.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/fileformats/ftpDetectInfo.py
--rw-rw-rw-   0        0        0     7319 2023-07-29 11:13:55.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/fileformats/imoWorkingShowerList.py
--rw-rw-rw-   0        0        0     5655 2023-07-22 20:32:11.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/fileformats/kmlHandlers.py
--rw-rw-rw-   0        0        0     2815 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/fileformats/platepar.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:27:23.332114 ukmon_meteortools-2023.7.7/ukmon_meteortools/rmsutils/
--rw-rw-rw-   0        0        0      652 2023-06-18 10:17:38.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/rmsutils/__init__.py
--rw-rw-rw-   0        0        0     1909 2023-05-02 20:41:57.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
--rw-rw-rw-   0        0        0     6077 2023-05-05 15:40:18.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/rmsutils/multiDayRadiant.py
--rw-rw-rw-   0        0        0     3763 2023-05-02 20:35:34.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/rmsutils/multiEventGroundMap.py
--rw-rw-rw-   0        0        0     5242 2023-05-05 16:20:15.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/rmsutils/multiTrackStack.py
--rw-rw-rw-   0        0        0     1372 2023-06-18 10:15:58.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/rmsutils/pickleToKml.py
--rw-rw-rw-   0        0        0     2297 2023-05-02 20:31:43.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
--rw-rw-rw-   0        0        0     2281 2023-05-02 20:31:31.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/rmsutils/plotRMSOrbits.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:27:23.340108 ukmon_meteortools-2023.7.7/ukmon_meteortools/share/
--rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
--rw-rw-rw-   0        0        0      525 2023-05-02 21:29:15.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/share/__init__.py
--rw-rw-rw-   0        0        0  1666256 2023-07-23 12:58:16.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/share/gmn_shower_table_20230518.npy
--rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/share/streamfulldata.npy
-drwxrwxrwx   0        0        0        0 2023-07-29 11:27:23.364105 ukmon_meteortools-2023.7.7/ukmon_meteortools/ukmondb/
--rw-rw-rw-   0        0        0     2094 2023-05-09 16:50:40.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/ukmondb/ECSVhandler.py
--rw-rw-rw-   0        0        0      879 2023-06-13 21:01:49.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/ukmondb/__init__.py
--rw-rw-rw-   0        0        0     3636 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/ukmondb/apiExampleCode.py
--rw-rw-rw-   0        0        0     1981 2023-05-08 19:28:35.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/ukmondb/getDetections.py
--rw-rw-rw-   0        0        0     4298 2023-05-19 20:56:49.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/ukmondb/getLiveImages.py
--rw-rw-rw-   0        0        0     1478 2023-05-08 21:25:36.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/ukmondb/trajPickle.py
--rw-rw-rw-   0        0        0     1795 2023-05-08 18:58:06.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/ukmondb/trajectoryKML.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:27:23.386108 ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/
--rw-rw-rw-   0        0        0    13798 2023-05-08 19:57:04.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/Math.py
--rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/VectorMaths.py
--rw-rw-rw-   0        0        0     1614 2023-07-04 17:34:08.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/__init__.py
--rw-rw-rw-   0        0        0     2519 2023-06-24 14:48:49.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/annotateImage.py
--rw-rw-rw-   0        0        0     1178 2023-05-08 13:25:56.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/convertSolLon.py
--rw-rw-rw-   0        0        0     2393 2023-05-07 12:29:44.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/drawFTPfile.py
--rw-rw-rw-   0        0        0     1454 2023-05-07 23:06:43.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/findNearDuplicates.py
--rw-rw-rw-   0        0        0     1405 2023-05-08 13:25:39.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/getActiveShowers.py
--rw-rw-rw-   0        0        0     3689 2023-05-08 12:09:09.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/getOverlappingFovs.py
--rw-rw-rw-   0        0        0     1046 2023-07-09 10:30:24.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/getRiseSet.py
--rw-rw-rw-   0        0        0     1694 2023-07-29 11:13:41.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/getShowerDates.py
--rw-rw-rw-   0        0        0     3429 2023-05-06 20:51:39.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/plotTrack.py
--rw-rw-rw-   0        0        0     8135 2023-07-26 19:17:48.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/sendAnEmail.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:27:23.304127 ukmon_meteortools-2023.7.7/ukmon_meteortools.egg-info/
--rw-rw-rw-   0        0        0    43083 2023-07-29 11:27:23.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1968 2023-07-29 11:27:23.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 11:27:23.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      642 2023-07-29 11:27:23.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-29 11:27:23.000000 ukmon_meteortools-2023.7.7/ukmon_meteortools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 13:07:51.270794 ukmon_meteortools-2023.7.8/
+-rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.7.8/LICENSE
+-rw-rw-rw-   0        0        0    43083 2023-07-29 13:07:51.269795 ukmon_meteortools-2023.7.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.7.8/README.md
+-rw-rw-rw-   0        0        0     2856 2023-07-29 13:07:27.000000 ukmon_meteortools-2023.7.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-29 13:07:51.270794 ukmon_meteortools-2023.7.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-29 13:07:51.176795 ukmon_meteortools-2023.7.8/tests/
+-rw-rw-rw-   0        0        0     3619 2023-07-28 09:52:46.000000 ukmon_meteortools-2023.7.8/tests/test_apis.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:07:51.177808 ukmon_meteortools-2023.7.8/ukmon_meteortools/
+-rw-rw-rw-   0        0        0     1177 2023-07-08 23:13:20.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 13:07:51.213795 ukmon_meteortools-2023.7.8/ukmon_meteortools/fileformats/
+-rw-rw-rw-   0        0        0     8762 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/fileformats/UFOAnalyzerXML.py
+-rw-rw-rw-   0        0        0     6211 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/fileformats/UFOCapXML.py
+-rw-rw-rw-   0        0        0      664 2023-05-08 13:19:19.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/fileformats/__init__.py
+-rw-rw-rw-   0        0        0    18716 2023-05-08 11:58:38.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/fileformats/ftpDetectInfo.py
+-rw-rw-rw-   0        0        0     7571 2023-07-29 12:54:28.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/fileformats/imoWorkingShowerList.py
+-rw-rw-rw-   0        0        0     5655 2023-07-22 20:32:11.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/fileformats/kmlHandlers.py
+-rw-rw-rw-   0        0        0     2815 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/fileformats/platepar.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:07:51.224795 ukmon_meteortools-2023.7.8/ukmon_meteortools/rmsutils/
+-rw-rw-rw-   0        0        0      652 2023-06-18 10:17:38.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/rmsutils/__init__.py
+-rw-rw-rw-   0        0        0     1909 2023-05-02 20:41:57.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
+-rw-rw-rw-   0        0        0     6077 2023-05-05 15:40:18.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/rmsutils/multiDayRadiant.py
+-rw-rw-rw-   0        0        0     3763 2023-05-02 20:35:34.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/rmsutils/multiEventGroundMap.py
+-rw-rw-rw-   0        0        0     5242 2023-05-05 16:20:15.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/rmsutils/multiTrackStack.py
+-rw-rw-rw-   0        0        0     1372 2023-06-18 10:15:58.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/rmsutils/pickleToKml.py
+-rw-rw-rw-   0        0        0     2297 2023-05-02 20:31:43.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
+-rw-rw-rw-   0        0        0     2281 2023-05-02 20:31:31.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/rmsutils/plotRMSOrbits.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:07:51.231793 ukmon_meteortools-2023.7.8/ukmon_meteortools/share/
+-rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
+-rw-rw-rw-   0        0        0      525 2023-05-02 21:29:15.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/share/__init__.py
+-rw-rw-rw-   0        0        0  1666256 2023-07-23 12:58:16.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/share/gmn_shower_table_20230518.npy
+-rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/share/streamfulldata.npy
+drwxrwxrwx   0        0        0        0 2023-07-29 13:07:51.248807 ukmon_meteortools-2023.7.8/ukmon_meteortools/ukmondb/
+-rw-rw-rw-   0        0        0     2094 2023-05-09 16:50:40.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/ukmondb/ECSVhandler.py
+-rw-rw-rw-   0        0        0      879 2023-06-13 21:01:49.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/ukmondb/__init__.py
+-rw-rw-rw-   0        0        0     3636 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/ukmondb/apiExampleCode.py
+-rw-rw-rw-   0        0        0     1981 2023-05-08 19:28:35.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/ukmondb/getDetections.py
+-rw-rw-rw-   0        0        0     4298 2023-05-19 20:56:49.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/ukmondb/getLiveImages.py
+-rw-rw-rw-   0        0        0     1478 2023-05-08 21:25:36.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/ukmondb/trajPickle.py
+-rw-rw-rw-   0        0        0     1795 2023-05-08 18:58:06.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/ukmondb/trajectoryKML.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:07:51.267795 ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/
+-rw-rw-rw-   0        0        0    13798 2023-05-08 19:57:04.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/Math.py
+-rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/VectorMaths.py
+-rw-rw-rw-   0        0        0     1614 2023-07-04 17:34:08.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/__init__.py
+-rw-rw-rw-   0        0        0     2519 2023-06-24 14:48:49.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/annotateImage.py
+-rw-rw-rw-   0        0        0     1178 2023-05-08 13:25:56.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/convertSolLon.py
+-rw-rw-rw-   0        0        0     2393 2023-05-07 12:29:44.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/drawFTPfile.py
+-rw-rw-rw-   0        0        0     1454 2023-05-07 23:06:43.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/findNearDuplicates.py
+-rw-rw-rw-   0        0        0     1405 2023-05-08 13:25:39.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/getActiveShowers.py
+-rw-rw-rw-   0        0        0     3689 2023-05-08 12:09:09.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/getOverlappingFovs.py
+-rw-rw-rw-   0        0        0     1046 2023-07-09 10:30:24.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/getRiseSet.py
+-rw-rw-rw-   0        0        0     1544 2023-07-29 13:00:17.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/getShowerDates.py
+-rw-rw-rw-   0        0        0     3429 2023-05-06 20:51:39.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/plotTrack.py
+-rw-rw-rw-   0        0        0     8135 2023-07-26 19:17:48.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/sendAnEmail.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:07:51.205795 ukmon_meteortools-2023.7.8/ukmon_meteortools.egg-info/
+-rw-rw-rw-   0        0        0    43083 2023-07-29 13:07:51.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1968 2023-07-29 13:07:51.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 13:07:51.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      675 2023-07-29 13:07:51.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-29 13:07:51.000000 ukmon_meteortools-2023.7.8/ukmon_meteortools.egg-info/top_level.txt
```

### Comparing `ukmon_meteortools-2023.7.7/LICENSE` & `ukmon_meteortools-2023.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/PKG-INFO` & `ukmon_meteortools-2023.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon_meteortools
-Version: 2023.7.7
+Version: 2023.7.8
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ukmon_meteortools-2023.7.7/README.md` & `ukmon_meteortools-2023.7.8/README.md`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/pyproject.toml` & `ukmon_meteortools-2023.7.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ukmon_meteortools"
-version = "2023.07.7"
+version = "2023.07.8"
 description = "Python Tools for Meteor Data Analysis"
 readme = "ukmon_meteortools/README.md"
 authors = [{ name = "Mark McIntyre", email = "ukmon@markmcintyreastro.co.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -39,15 +39,15 @@
     "xmltodict",
     "requests",
     "pyproj==1.9.6 ; python_version < '3.8' and platform_machine == 'armv7l'",
     "pyproj==2.6.1.post1 ; python_version < '3.8' and platform_machine != 'armv7l'",
     "pyproj==3.5.0 ; python_version >= '3.8'",
     "pdoc",
     "Cython",
-    "opencv-python",
+    "opencv-python; platform_machine != 'armv71'",
     "imageio",
     "scipy",
     "jplephem",
     "pyephem",
     "gitpython",
     "astropy",
     "pyqt5; platform_machine != 'aarch64'",
@@ -75,15 +75,15 @@
 #[tool.setuptools.packages.find]
 #where = ["ukmon_meteortools"]
 
 [tool.setuptools.package-data]
 "*" = ["*.npy", "*.xml"]
 
 [tool.bumpver]
-current_version = "2023.07.7"
+current_version = "2023.07.8"
 version_pattern = "YYYY.0M.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `ukmon_meteortools-2023.7.7/tests/test_apis.py` & `ukmon_meteortools-2023.7.8/tests/test_apis.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/README.md` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/README.md`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/fileformats/UFOAnalyzerXML.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/fileformats/UFOAnalyzerXML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/fileformats/UFOCapXML.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/fileformats/UFOCapXML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/fileformats/__init__.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/fileformats/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/fileformats/ftpDetectInfo.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/fileformats/ftpDetectInfo.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/fileformats/imoWorkingShowerList.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/fileformats/imoWorkingShowerList.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 
 import xmltodict
 import datetime
 import os
 import numpy as np
 from ukmon_meteortools.utils import jd2Date, sollon2jd
+import copy
 
 # imported from $SRC/share
 try:
     from majorminor import majorlist, minorlist
 except:
     majorlist = ['QUA', 'LYR', 'ETA', 'CAP', 'SDA', 'PER', 'AUR', 'ORI', 'NTA', 'STA', 'LEO', 'GEM', 'URS']
     minorlist = ['SPE','OCT','DRA','EGE','MON','HYD','COM','NOO']
@@ -47,49 +48,53 @@
         self.fullstreamdata = np.load(fullstreamname)
         #print('initialised')
 
     
     def getShowerByCode(self, iaucode, useFull=False):
         ds = {'@id':None, 'IAU_code':None,'start':None, 'end':None, 
             'peak':None, 'r':None, 'name':None, 'V':None, 'ZHR':None, 'RA':None, 'DE':None, 'pksollon': None}
-        got = None
+        ds2 = {'@id':None, 'IAU_code':None,'start':None, 'end':None, 
+            'peak':None, 'r':None, 'name':None, 'V':None, 'ZHR':None, 'RA':None, 'DE':None, 'pksollon': None}
         for shower in self.showerlist:
             if shower['IAU_code'] == iaucode:
-                got = shower
+                ds = shower
         pksollong = -1
         subset = self.fullstreamdata[np.where(self.fullstreamdata[:,3]==iaucode)]
         if subset is not None:
             mtch = [sh for sh in subset if sh[6] > '-1']
             if len(mtch) > 0:
-                ds['IAU_code'] = mtch[-1][3].strip()
-                ds['name'] = mtch[-1][4].strip()
-                ds['V'] = mtch[-1][12]
-                ds['@id'] = mtch[-1][1]
-                ds['RA'] = mtch[-1][8]
-                ds['DE'] = mtch[-1][9]
+                ds2 = copy.deepcopy(ds)
+                ds2['IAU_code'] = mtch[-1][3].strip()
+                ds2['name'] = mtch[-1][4].strip()
+                ds2['V'] = mtch[-1][12]
+                ds2['@id'] = mtch[-1][1]
+                ds2['RA'] = mtch[-1][8]
+                ds2['DE'] = mtch[-1][9]
 
                 pksollong = float(mtch[-1][7])
                 dt = datetime.datetime.now()
                 yr = dt.year
                 mth = dt.month
                 jd = sollon2jd(yr, mth, pksollong)
                 pkdt = jd2Date(jd, dt_obj=True)
-                ds['peak'] = pkdt.strftime('%h %d')
+                ds2['peak'] = pkdt.strftime('%h %d')
                 # start/end pop idx, ZHR not available in the IAU data
-                ds['start'] = (pkdt + datetime.timedelta(days=-2)).strftime('%h %d')
-                ds['end'] = (pkdt + datetime.timedelta(days=2)).strftime('%h %d')
-                ds['r'] = got['r']
-                ds['ZHR'] = got['ZHR']
-                ds['pksollon'] = pksollong
+                ds2['start'] = (pkdt + datetime.timedelta(days=-2)).strftime('%h %d')
+                ds2['end'] = (pkdt + datetime.timedelta(days=2)).strftime('%h %d')
+                ds2['pksollon'] = pksollong
+        #print(ds)
+        #print(ds2)
         if useFull is False:
-            got['pksollon'] = pksollong
-            got['@id'] = ds['@id']
-            return got
-        else:
+            ds['pksollon'] = pksollong
+            ds['@id'] = ds2['@id']
             return ds
+        else:
+            ds2['ZHR'] = ds['ZHR']
+            ds2['r'] = ds['r']
+            return ds2
 
     def getStart(self, iaucode, currdt=None):
         shower = self.getShowerByCode(iaucode)
         if currdt is None:
             now = datetime.datetime.today().year
             mth = datetime.datetime.today().month
         else:
```

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/fileformats/kmlHandlers.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/fileformats/kmlHandlers.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/fileformats/platepar.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/fileformats/platepar.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/rmsutils/__init__.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/rmsutils/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/rmsutils/multiDayRadiant.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/rmsutils/multiDayRadiant.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/rmsutils/multiEventGroundMap.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/rmsutils/multiEventGroundMap.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/rmsutils/multiTrackStack.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/rmsutils/multiTrackStack.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/rmsutils/pickleToKml.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/rmsutils/pickleToKml.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/rmsutils/plotCAMSOrbits.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/rmsutils/plotCAMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/rmsutils/plotRMSOrbits.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/rmsutils/plotRMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/share/__init__.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/share/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/share/gmn_shower_table_20230518.npy` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/share/gmn_shower_table_20230518.npy`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/share/streamfulldata.npy` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/share/streamfulldata.npy`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/ukmondb/ECSVhandler.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/ukmondb/ECSVhandler.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/ukmondb/__init__.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/ukmondb/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/ukmondb/apiExampleCode.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/ukmondb/apiExampleCode.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/ukmondb/getDetections.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/ukmondb/getDetections.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/ukmondb/getLiveImages.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/ukmondb/getLiveImages.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/ukmondb/trajPickle.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/ukmondb/trajPickle.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/ukmondb/trajectoryKML.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/ukmondb/trajectoryKML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/Math.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/Math.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/VectorMaths.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/VectorMaths.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/__init__.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/annotateImage.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/annotateImage.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/convertSolLon.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/convertSolLon.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/drawFTPfile.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/drawFTPfile.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/findNearDuplicates.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/findNearDuplicates.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/getActiveShowers.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/getActiveShowers.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/getOverlappingFovs.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/getOverlappingFovs.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/getRiseSet.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/getRiseSet.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/getShowerDates.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/getShowerDates.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 #
 # simple script to get the active shower list from the IMO working list
 
 import datetime
 
-from ukmon_meteortools.utils import jd2Date, sollon2jd
 from ukmon_meteortools.fileformats import imoWorkingShowerList as iwsl
 
 
 def getShowerDets(shwr, stringFmt=False, dataPth=None):
     """ Get details of a shower 
     
     Arguments:  
@@ -18,27 +17,23 @@
         dataPth   [string] path to the datafiles. Default None means data read from internal files. 
          
     Returns:  
         (id, full name, peak solar longitude, peak date mm-dd)  
     """
     sl = iwsl.IMOshowerList()
     mtch = sl.getShowerByCode(shwr)
-    #print(mtch)
-    if len(mtch) > 0:
+    if len(mtch) > 0 and mtch['@id'] is not None:
         id = int(mtch['@id'])
         nam = mtch['name']
         pkdtstr = mtch['peak']
         dt = datetime.datetime.now()
         yr = dt.year
-        mth = dt.month
         pkdt = datetime.datetime.strptime(f'{yr} {pkdtstr}','%Y %b %d')
-        pksollong = mtch['pksollon']
-        jd = sollon2jd(yr, mth, pksollong)
-        pkdt = jd2Date(jd, dt_obj=True)
         dtstr = pkdt.strftime('%m-%d')
+        pksollong = mtch['pksollon']
     else:
         id, nam, pksollong, dtstr = 0, 'Unknown', 0, 'Unknown'
     if stringFmt:
         return f"{pksollong},{dtstr},{nam},{shwr}"
     else:
         return id, nam, pksollong, dtstr
```

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/plotTrack.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/plotTrack.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools/utils/sendAnEmail.py` & `ukmon_meteortools-2023.7.8/ukmon_meteortools/utils/sendAnEmail.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools.egg-info/PKG-INFO` & `ukmon_meteortools-2023.7.8/ukmon_meteortools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon-meteortools
-Version: 2023.7.7
+Version: 2023.7.8
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools.egg-info/SOURCES.txt` & `ukmon_meteortools-2023.7.8/ukmon_meteortools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.7/ukmon_meteortools.egg-info/requires.txt` & `ukmon_meteortools-2023.7.8/ukmon_meteortools.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 Shapely
 simplekml
 s3fs
 xmltodict
 requests
 pdoc
 Cython
-opencv-python
 imageio
 scipy
 jplephem
 pyephem
 gitpython
 astropy
 basemap
 basemap-data-hires
 
 [:platform_machine != "aarch64"]
 pyqt5
 
+[:platform_machine != "armv71"]
+opencv-python
+
 [:python_version < "3.8" and platform_machine != "armv7l"]
 pyproj==2.6.1.post1
 
 [:python_version < "3.8" and platform_machine == "armv7l"]
 pyproj==1.9.6
 
 [:python_version <= "3.8"]
```

