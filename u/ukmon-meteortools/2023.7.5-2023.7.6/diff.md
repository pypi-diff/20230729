# Comparing `tmp/ukmon_meteortools-2023.7.5.tar.gz` & `tmp/ukmon_meteortools-2023.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukmon_meteortools-2023.7.5.tar", last modified: Sat Jul 29 10:37:56 2023, max compression
+gzip compressed data, was "ukmon_meteortools-2023.7.6.tar", last modified: Sat Jul 29 11:16:19 2023, max compression
```

## Comparing `ukmon_meteortools-2023.7.5.tar` & `ukmon_meteortools-2023.7.6.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 10:37:56.212915 ukmon_meteortools-2023.7.5/
--rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.7.5/LICENSE
--rw-rw-rw-   0        0        0    43083 2023-07-29 10:37:56.211922 ukmon_meteortools-2023.7.5/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.7.5/README.md
--rw-rw-rw-   0        0        0     2820 2023-07-29 10:37:26.000000 ukmon_meteortools-2023.7.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-29 10:37:56.213925 ukmon_meteortools-2023.7.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-29 10:37:56.095916 ukmon_meteortools-2023.7.5/tests/
--rw-rw-rw-   0        0        0     3619 2023-07-28 09:52:46.000000 ukmon_meteortools-2023.7.5/tests/test_apis.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:37:56.097924 ukmon_meteortools-2023.7.5/ukmon_meteortools/
--rw-rw-rw-   0        0        0     1177 2023-07-08 23:13:20.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 10:37:56.140920 ukmon_meteortools-2023.7.5/ukmon_meteortools/fileformats/
--rw-rw-rw-   0        0        0     8762 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/fileformats/UFOAnalyzerXML.py
--rw-rw-rw-   0        0        0     6211 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/fileformats/UFOCapXML.py
--rw-rw-rw-   0        0        0      664 2023-05-08 13:19:19.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/fileformats/__init__.py
--rw-rw-rw-   0        0        0    18716 2023-05-08 11:58:38.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/fileformats/ftpDetectInfo.py
--rw-rw-rw-   0        0        0     7318 2023-07-29 10:35:50.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/fileformats/imoWorkingShowerList.py
--rw-rw-rw-   0        0        0     5655 2023-07-22 20:32:11.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/fileformats/kmlHandlers.py
--rw-rw-rw-   0        0        0     2815 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/fileformats/platepar.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:37:56.153922 ukmon_meteortools-2023.7.5/ukmon_meteortools/rmsutils/
--rw-rw-rw-   0        0        0      652 2023-06-18 10:17:38.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/rmsutils/__init__.py
--rw-rw-rw-   0        0        0     1909 2023-05-02 20:41:57.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
--rw-rw-rw-   0        0        0     6077 2023-05-05 15:40:18.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/rmsutils/multiDayRadiant.py
--rw-rw-rw-   0        0        0     3763 2023-05-02 20:35:34.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/rmsutils/multiEventGroundMap.py
--rw-rw-rw-   0        0        0     5242 2023-05-05 16:20:15.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/rmsutils/multiTrackStack.py
--rw-rw-rw-   0        0        0     1372 2023-06-18 10:15:58.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/rmsutils/pickleToKml.py
--rw-rw-rw-   0        0        0     2297 2023-05-02 20:31:43.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
--rw-rw-rw-   0        0        0     2281 2023-05-02 20:31:31.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/rmsutils/plotRMSOrbits.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:37:56.163919 ukmon_meteortools-2023.7.5/ukmon_meteortools/share/
--rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
--rw-rw-rw-   0        0        0      525 2023-05-02 21:29:15.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/share/__init__.py
--rw-rw-rw-   0        0        0  1666256 2023-07-23 12:58:16.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/share/gmn_shower_table_20230518.npy
--rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/share/streamfulldata.npy
-drwxrwxrwx   0        0        0        0 2023-07-29 10:37:56.185931 ukmon_meteortools-2023.7.5/ukmon_meteortools/ukmondb/
--rw-rw-rw-   0        0        0     2094 2023-05-09 16:50:40.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/ukmondb/ECSVhandler.py
--rw-rw-rw-   0        0        0      879 2023-06-13 21:01:49.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/ukmondb/__init__.py
--rw-rw-rw-   0        0        0     3636 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/ukmondb/apiExampleCode.py
--rw-rw-rw-   0        0        0     1981 2023-05-08 19:28:35.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/ukmondb/getDetections.py
--rw-rw-rw-   0        0        0     4298 2023-05-19 20:56:49.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/ukmondb/getLiveImages.py
--rw-rw-rw-   0        0        0     1478 2023-05-08 21:25:36.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/ukmondb/trajPickle.py
--rw-rw-rw-   0        0        0     1795 2023-05-08 18:58:06.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/ukmondb/trajectoryKML.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:37:56.207915 ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/
--rw-rw-rw-   0        0        0    13798 2023-05-08 19:57:04.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/Math.py
--rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/VectorMaths.py
--rw-rw-rw-   0        0        0     1614 2023-07-04 17:34:08.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/__init__.py
--rw-rw-rw-   0        0        0     2519 2023-06-24 14:48:49.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/annotateImage.py
--rw-rw-rw-   0        0        0     1178 2023-05-08 13:25:56.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/convertSolLon.py
--rw-rw-rw-   0        0        0     2393 2023-05-07 12:29:44.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/drawFTPfile.py
--rw-rw-rw-   0        0        0     1454 2023-05-07 23:06:43.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/findNearDuplicates.py
--rw-rw-rw-   0        0        0     1405 2023-05-08 13:25:39.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/getActiveShowers.py
--rw-rw-rw-   0        0        0     3689 2023-05-08 12:09:09.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/getOverlappingFovs.py
--rw-rw-rw-   0        0        0     1046 2023-07-09 10:30:24.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/getRiseSet.py
--rw-rw-rw-   0        0        0     1693 2023-07-29 10:35:50.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/getShowerDates.py
--rw-rw-rw-   0        0        0     3429 2023-05-06 20:51:39.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/plotTrack.py
--rw-rw-rw-   0        0        0     8135 2023-07-26 19:17:48.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/sendAnEmail.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:37:56.131912 ukmon_meteortools-2023.7.5/ukmon_meteortools.egg-info/
--rw-rw-rw-   0        0        0    43083 2023-07-29 10:37:56.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1968 2023-07-29 10:37:56.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 10:37:56.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      609 2023-07-29 10:37:56.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-29 10:37:56.000000 ukmon_meteortools-2023.7.5/ukmon_meteortools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 11:16:19.962873 ukmon_meteortools-2023.7.6/
+-rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.7.6/LICENSE
+-rw-rw-rw-   0        0        0    43083 2023-07-29 11:16:19.960870 ukmon_meteortools-2023.7.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.7.6/README.md
+-rw-rw-rw-   0        0        0     2820 2023-07-29 11:15:50.000000 ukmon_meteortools-2023.7.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-29 11:16:19.963882 ukmon_meteortools-2023.7.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-29 11:16:19.855871 ukmon_meteortools-2023.7.6/tests/
+-rw-rw-rw-   0        0        0     3619 2023-07-28 09:52:46.000000 ukmon_meteortools-2023.7.6/tests/test_apis.py
+drwxrwxrwx   0        0        0        0 2023-07-29 11:16:19.857869 ukmon_meteortools-2023.7.6/ukmon_meteortools/
+-rw-rw-rw-   0        0        0     1177 2023-07-08 23:13:20.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 11:16:19.898870 ukmon_meteortools-2023.7.6/ukmon_meteortools/fileformats/
+-rw-rw-rw-   0        0        0     8762 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/fileformats/UFOAnalyzerXML.py
+-rw-rw-rw-   0        0        0     6211 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/fileformats/UFOCapXML.py
+-rw-rw-rw-   0        0        0      664 2023-05-08 13:19:19.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/fileformats/__init__.py
+-rw-rw-rw-   0        0        0    18716 2023-05-08 11:58:38.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/fileformats/ftpDetectInfo.py
+-rw-rw-rw-   0        0        0     7319 2023-07-29 11:13:55.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/fileformats/imoWorkingShowerList.py
+-rw-rw-rw-   0        0        0     5655 2023-07-22 20:32:11.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/fileformats/kmlHandlers.py
+-rw-rw-rw-   0        0        0     2815 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/fileformats/platepar.py
+drwxrwxrwx   0        0        0        0 2023-07-29 11:16:19.908869 ukmon_meteortools-2023.7.6/ukmon_meteortools/rmsutils/
+-rw-rw-rw-   0        0        0      652 2023-06-18 10:17:38.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/rmsutils/__init__.py
+-rw-rw-rw-   0        0        0     1909 2023-05-02 20:41:57.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
+-rw-rw-rw-   0        0        0     6077 2023-05-05 15:40:18.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/rmsutils/multiDayRadiant.py
+-rw-rw-rw-   0        0        0     3763 2023-05-02 20:35:34.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/rmsutils/multiEventGroundMap.py
+-rw-rw-rw-   0        0        0     5242 2023-05-05 16:20:15.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/rmsutils/multiTrackStack.py
+-rw-rw-rw-   0        0        0     1372 2023-06-18 10:15:58.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/rmsutils/pickleToKml.py
+-rw-rw-rw-   0        0        0     2297 2023-05-02 20:31:43.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
+-rw-rw-rw-   0        0        0     2281 2023-05-02 20:31:31.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/rmsutils/plotRMSOrbits.py
+drwxrwxrwx   0        0        0        0 2023-07-29 11:16:19.918871 ukmon_meteortools-2023.7.6/ukmon_meteortools/share/
+-rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
+-rw-rw-rw-   0        0        0      525 2023-05-02 21:29:15.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/share/__init__.py
+-rw-rw-rw-   0        0        0  1666256 2023-07-23 12:58:16.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/share/gmn_shower_table_20230518.npy
+-rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/share/streamfulldata.npy
+drwxrwxrwx   0        0        0        0 2023-07-29 11:16:19.938869 ukmon_meteortools-2023.7.6/ukmon_meteortools/ukmondb/
+-rw-rw-rw-   0        0        0     2094 2023-05-09 16:50:40.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/ukmondb/ECSVhandler.py
+-rw-rw-rw-   0        0        0      879 2023-06-13 21:01:49.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/ukmondb/__init__.py
+-rw-rw-rw-   0        0        0     3636 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/ukmondb/apiExampleCode.py
+-rw-rw-rw-   0        0        0     1981 2023-05-08 19:28:35.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/ukmondb/getDetections.py
+-rw-rw-rw-   0        0        0     4298 2023-05-19 20:56:49.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/ukmondb/getLiveImages.py
+-rw-rw-rw-   0        0        0     1478 2023-05-08 21:25:36.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/ukmondb/trajPickle.py
+-rw-rw-rw-   0        0        0     1795 2023-05-08 18:58:06.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/ukmondb/trajectoryKML.py
+drwxrwxrwx   0        0        0        0 2023-07-29 11:16:19.959877 ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/
+-rw-rw-rw-   0        0        0    13798 2023-05-08 19:57:04.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/Math.py
+-rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/VectorMaths.py
+-rw-rw-rw-   0        0        0     1614 2023-07-04 17:34:08.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/__init__.py
+-rw-rw-rw-   0        0        0     2519 2023-06-24 14:48:49.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/annotateImage.py
+-rw-rw-rw-   0        0        0     1178 2023-05-08 13:25:56.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/convertSolLon.py
+-rw-rw-rw-   0        0        0     2393 2023-05-07 12:29:44.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/drawFTPfile.py
+-rw-rw-rw-   0        0        0     1454 2023-05-07 23:06:43.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/findNearDuplicates.py
+-rw-rw-rw-   0        0        0     1405 2023-05-08 13:25:39.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/getActiveShowers.py
+-rw-rw-rw-   0        0        0     3689 2023-05-08 12:09:09.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/getOverlappingFovs.py
+-rw-rw-rw-   0        0        0     1046 2023-07-09 10:30:24.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/getRiseSet.py
+-rw-rw-rw-   0        0        0     1694 2023-07-29 11:13:41.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/getShowerDates.py
+-rw-rw-rw-   0        0        0     3429 2023-05-06 20:51:39.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/plotTrack.py
+-rw-rw-rw-   0        0        0     8135 2023-07-26 19:17:48.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/sendAnEmail.py
+drwxrwxrwx   0        0        0        0 2023-07-29 11:16:19.886871 ukmon_meteortools-2023.7.6/ukmon_meteortools.egg-info/
+-rw-rw-rw-   0        0        0    43083 2023-07-29 11:16:19.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1968 2023-07-29 11:16:19.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 11:16:19.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      609 2023-07-29 11:16:19.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-29 11:16:19.000000 ukmon_meteortools-2023.7.6/ukmon_meteortools.egg-info/top_level.txt
```

### Comparing `ukmon_meteortools-2023.7.5/LICENSE` & `ukmon_meteortools-2023.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/PKG-INFO` & `ukmon_meteortools-2023.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon_meteortools
-Version: 2023.7.5
+Version: 2023.7.6
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ukmon_meteortools-2023.7.5/README.md` & `ukmon_meteortools-2023.7.6/README.md`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/pyproject.toml` & `ukmon_meteortools-2023.7.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ukmon_meteortools"
-version = "2023.07.5"
+version = "2023.07.6"
 description = "Python Tools for Meteor Data Analysis"
 readme = "ukmon_meteortools/README.md"
 authors = [{ name = "Mark McIntyre", email = "ukmon@markmcintyreastro.co.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -75,15 +75,15 @@
 #[tool.setuptools.packages.find]
 #where = ["ukmon_meteortools"]
 
 [tool.setuptools.package-data]
 "*" = ["*.npy", "*.xml"]
 
 [tool.bumpver]
-current_version = "2023.07.5"
+current_version = "2023.07.6"
 version_pattern = "YYYY.0M.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `ukmon_meteortools-2023.7.5/tests/test_apis.py` & `ukmon_meteortools-2023.7.6/tests/test_apis.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/README.md` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/README.md`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/fileformats/UFOAnalyzerXML.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/fileformats/UFOAnalyzerXML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/fileformats/UFOCapXML.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/fileformats/UFOCapXML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/fileformats/__init__.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/fileformats/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/fileformats/ftpDetectInfo.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/fileformats/ftpDetectInfo.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/fileformats/imoWorkingShowerList.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/fileformats/imoWorkingShowerList.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self.showerlist = tmplist['meteor_shower_list']['shower']
         if fullstreamname is None:
             fullstreamname = os.path.join(datadir, 'share', 'streamfulldata.npy')
             if not os.path.isfile(fullstreamname):
                 datadir=os.path.split(os.path.abspath(__file__))[0]
                 fullstreamname = os.path.join(datadir, '..', 'share', 'streamfulldata.npy')
         self.fullstreamdata = np.load(fullstreamname)
-        print('initialised')
+        #print('initialised')
 
     
     def getShowerByCode(self, iaucode, useFull=False):
         ds = {'@id':None, 'IAU_code':None,'start':None, 'end':None, 
             'peak':None, 'r':None, 'name':None, 'V':None, 'ZHR':None, 'RA':None, 'DE':None, 'pksollon': None}
         got = None
         for shower in self.showerlist:
```

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/fileformats/kmlHandlers.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/fileformats/kmlHandlers.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/fileformats/platepar.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/fileformats/platepar.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/rmsutils/__init__.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/rmsutils/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/rmsutils/multiDayRadiant.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/rmsutils/multiDayRadiant.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/rmsutils/multiEventGroundMap.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/rmsutils/multiEventGroundMap.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/rmsutils/multiTrackStack.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/rmsutils/multiTrackStack.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/rmsutils/pickleToKml.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/rmsutils/pickleToKml.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/rmsutils/plotCAMSOrbits.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/rmsutils/plotCAMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/rmsutils/plotRMSOrbits.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/rmsutils/plotRMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/share/__init__.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/share/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/share/gmn_shower_table_20230518.npy` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/share/gmn_shower_table_20230518.npy`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/share/streamfulldata.npy` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/share/streamfulldata.npy`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/ukmondb/ECSVhandler.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/ukmondb/ECSVhandler.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/ukmondb/__init__.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/ukmondb/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/ukmondb/apiExampleCode.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/ukmondb/apiExampleCode.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/ukmondb/getDetections.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/ukmondb/getDetections.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/ukmondb/getLiveImages.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/ukmondb/getLiveImages.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/ukmondb/trajPickle.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/ukmondb/trajPickle.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/ukmondb/trajectoryKML.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/ukmondb/trajectoryKML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/Math.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/Math.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/VectorMaths.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/VectorMaths.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/__init__.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/annotateImage.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/annotateImage.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/convertSolLon.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/convertSolLon.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/drawFTPfile.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/drawFTPfile.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/findNearDuplicates.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/findNearDuplicates.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/getActiveShowers.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/getActiveShowers.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/getOverlappingFovs.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/getOverlappingFovs.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/getRiseSet.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/getRiseSet.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/getShowerDates.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/getShowerDates.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         dataPth   [string] path to the datafiles. Default None means data read from internal files. 
          
     Returns:  
         (id, full name, peak solar longitude, peak date mm-dd)  
     """
     sl = iwsl.IMOshowerList()
     mtch = sl.getShowerByCode(shwr)
-    print(mtch)
+    #print(mtch)
     if len(mtch) > 0:
         id = int(mtch['@id'])
         nam = mtch['name']
         pkdtstr = mtch['peak']
         dt = datetime.datetime.now()
         yr = dt.year
         mth = dt.month
```

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/plotTrack.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/plotTrack.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools/utils/sendAnEmail.py` & `ukmon_meteortools-2023.7.6/ukmon_meteortools/utils/sendAnEmail.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools.egg-info/PKG-INFO` & `ukmon_meteortools-2023.7.6/ukmon_meteortools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon-meteortools
-Version: 2023.7.5
+Version: 2023.7.6
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools.egg-info/SOURCES.txt` & `ukmon_meteortools-2023.7.6/ukmon_meteortools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.7.5/ukmon_meteortools.egg-info/requires.txt` & `ukmon_meteortools-2023.7.6/ukmon_meteortools.egg-info/requires.txt`

 * *Files identical despite different names*

