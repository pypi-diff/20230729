# Comparing `tmp/pyqtclass-0.2.5.tar.gz` & `tmp/pyqtclass-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqtclass-0.2.5.tar", last modified: Sun Jul 23 05:26:43 2023, max compression
+gzip compressed data, was "pyqtclass-0.2.7.tar", last modified: Sat Jul 29 09:48:46 2023, max compression
```

## Comparing `pyqtclass-0.2.5.tar` & `pyqtclass-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 05:26:43.418889 pyqtclass-0.2.5/
--rw-rw-rw-   0        0        0     1086 2023-03-24 01:33:53.000000 pyqtclass-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     1088 2023-07-23 05:26:43.417889 pyqtclass-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      598 2023-07-23 05:09:29.000000 pyqtclass-0.2.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-23 05:26:43.418889 pyqtclass-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      835 2023-07-23 05:24:43.000000 pyqtclass-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-23 05:26:43.384881 pyqtclass-0.2.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-23 05:26:43.391882 pyqtclass-0.2.5/src/pyqtclass/
--rw-rw-rw-   0        0        0     6260 2023-07-23 05:23:46.000000 pyqtclass-0.2.5/src/pyqtclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-23 05:26:43.415889 pyqtclass-0.2.5/src/pyqtclass.egg-info/
--rw-rw-rw-   0        0        0     1088 2023-07-23 05:26:43.000000 pyqtclass-0.2.5/src/pyqtclass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-07-23 05:26:43.000000 pyqtclass-0.2.5/src/pyqtclass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 05:26:43.000000 pyqtclass-0.2.5/src/pyqtclass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-23 05:26:43.000000 pyqtclass-0.2.5/src/pyqtclass.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-23 05:26:43.000000 pyqtclass-0.2.5/src/pyqtclass.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 09:48:46.679868 pyqtclass-0.2.7/
+-rw-rw-rw-   0        0        0     1086 2023-03-24 01:33:53.000000 pyqtclass-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0     1094 2023-07-29 09:48:46.678868 pyqtclass-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      604 2023-07-29 09:47:21.000000 pyqtclass-0.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-29 09:48:46.679868 pyqtclass-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      835 2023-07-29 09:44:57.000000 pyqtclass-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:48:46.644861 pyqtclass-0.2.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-29 09:48:46.651861 pyqtclass-0.2.7/src/pyqtclass/
+-rw-rw-rw-   0        0        0     6274 2023-07-29 05:03:35.000000 pyqtclass-0.2.7/src/pyqtclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:48:46.675867 pyqtclass-0.2.7/src/pyqtclass.egg-info/
+-rw-rw-rw-   0        0        0     1094 2023-07-29 09:48:46.000000 pyqtclass-0.2.7/src/pyqtclass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-07-29 09:48:46.000000 pyqtclass-0.2.7/src/pyqtclass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 09:48:46.000000 pyqtclass-0.2.7/src/pyqtclass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-29 09:48:46.000000 pyqtclass-0.2.7/src/pyqtclass.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-29 09:48:46.000000 pyqtclass-0.2.7/src/pyqtclass.egg-info/top_level.txt
```

### Comparing `pyqtclass-0.2.5/LICENSE` & `pyqtclass-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqtclass-0.2.5/PKG-INFO` & `pyqtclass-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqtclass
-Version: 0.2.5
+Version: 0.2.7
 Summary: PyQt 기반으로 동작하는 객체들의 베이스클래스 모음 패키지
 Home-page: https://github.com/innovata/PyQtClasses
 Author: innovata
 Author-email: iinnovata@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 PyQt 기반으로 동작하는 'Worker 객체' 들의 베이스클래스 제공.
 
 WorkerSchedule 테이블 정보를 기반으로 MainApp, SubApp, Worker 의 동작시간을 제어할 수 있음.
 
 
 ### WorkerSchedule 테이블 예시
 
-![Alt text](<Docs/WorkerSchedule 테이블 예시.png>)
+![Alt text](<Docs/files/WorkerSchedule 테이블 예시.png>)
 
 #### 스키마 설명
 
     worker: Worker Class Name (string)
     stime: Start Time (string)
     etime: End Time (string)
     interval: Interval Time (seconds)
```

### Comparing `pyqtclass-0.2.5/README.md` & `pyqtclass-0.2.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 PyQt 기반으로 동작하는 'Worker 객체' 들의 베이스클래스 제공.
 
 WorkerSchedule 테이블 정보를 기반으로 MainApp, SubApp, Worker 의 동작시간을 제어할 수 있음.
 
 
 ### WorkerSchedule 테이블 예시
 
-![Alt text](<Docs/WorkerSchedule 테이블 예시.png>)
+![Alt text](<Docs/files/WorkerSchedule 테이블 예시.png>)
 
 #### 스키마 설명
 
     worker: Worker Class Name (string)
     stime: Start Time (string)
     etime: End Time (string)
     interval: Interval Time (seconds)
```

### Comparing `pyqtclass-0.2.5/setup.py` & `pyqtclass-0.2.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyqtclass",
-    version="0.2.5",
+    version="0.2.7",
     author="innovata",
     author_email="iinnovata@gmail.com",
     description='PyQt 기반으로 동작하는 객체들의 베이스클래스 모음 패키지',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f"https://github.com/innovata/PyQtClasses",
     classifiers=[
```

### Comparing `pyqtclass-0.2.5/src/pyqtclass/__init__.py` & `pyqtclass-0.2.7/src/pyqtclass/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 import re
 from time import sleep
 from datetime import datetime, timedelta
 
 
 from PyQt5.QtCore import QObject, pyqtSignal, pyqtSlot, QTimer, QThread
-from PyQt5.QtCore import *
 
 
 from ipylib.idebug import *
 from ipylib import idatetime
 
 
 
@@ -76,15 +75,15 @@
 """스케쥴로 움직이는 단독스레드형 객체"""
 class QBaseWorker(QBaseObject):
 
     # @ctracer
     def __init__(self, func, stime=None, etime=None, interval=60):
         super().__init__()
         self._isRunning = False
-        self.__func__ = func
+        self.__exec_func__ = func
         self.stime = stime
         self.etime = etime
         self._interval = interval
     # @ctracer
     def finish(self, *args):
         self.stop_alltimers()
         super().finish()
@@ -96,23 +95,25 @@
             self.start_timer('__WorkerRuntimeCheckTimer', self.__check_runtime__, self._interval)
             self.__check_runtime__()
     # @ctracer
     def __check_runtime__(self):
         t1 = idatetime.DatetimeParser(self.stime)
         t2 = idatetime.DatetimeParser(self.etime)
         t = datetime.now().astimezone()
-        if t1 <= t <= t2:
+        if t < t1: 
+            pass
+        elif t1 <= t <= t2:
             if self._isRunning: pass
             else: self.__exec_run__()
-        elif t < t1: pass
-        else: self.finish('동작시간종료', {'stime':self.stime, 'etime':self.etime})
+        else: 
+            self.finish('동작시간종료', {'stime':self.stime, 'etime':self.etime})
     # @ctracer
     def __exec_run__(self):
         self._isRunning = True
-        self.__func__()
+        self.__exec_func__()
 
 
 class ThreadGenerator(QBaseObject):
     terminated = pyqtSignal(str)
 
     # @ctracer
     def __init__(self, qobject, func='run', *args, **kwargs):
@@ -177,7 +178,9 @@
         else:
             self.keys.remove(k)
             delattr(self, k)
             self._report({'제거':k})
     def _report(self, *args):
         logtime = datetime.now().strftime('%H:%M:%S,%f')[:-3]
         print(logtime, [self.__datanm__, args, len(self.keys), self.keys])
+
+
```

### Comparing `pyqtclass-0.2.5/src/pyqtclass.egg-info/PKG-INFO` & `pyqtclass-0.2.7/src/pyqtclass.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqtclass
-Version: 0.2.5
+Version: 0.2.7
 Summary: PyQt 기반으로 동작하는 객체들의 베이스클래스 모음 패키지
 Home-page: https://github.com/innovata/PyQtClasses
 Author: innovata
 Author-email: iinnovata@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 PyQt 기반으로 동작하는 'Worker 객체' 들의 베이스클래스 제공.
 
 WorkerSchedule 테이블 정보를 기반으로 MainApp, SubApp, Worker 의 동작시간을 제어할 수 있음.
 
 
 ### WorkerSchedule 테이블 예시
 
-![Alt text](<Docs/WorkerSchedule 테이블 예시.png>)
+![Alt text](<Docs/files/WorkerSchedule 테이블 예시.png>)
 
 #### 스키마 설명
 
     worker: Worker Class Name (string)
     stime: Start Time (string)
     etime: End Time (string)
     interval: Interval Time (seconds)
```

