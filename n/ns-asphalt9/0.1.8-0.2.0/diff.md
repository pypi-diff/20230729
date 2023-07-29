# Comparing `tmp/ns_asphalt9-0.1.8.tar.gz` & `tmp/ns_asphalt9-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_asphalt9-0.1.8.tar", last modified: Mon Jul 24 10:57:11 2023, max compression
+gzip compressed data, was "ns_asphalt9-0.2.0.tar", last modified: Sat Jul 29 04:00:49 2023, max compression
```

## Comparing `ns_asphalt9-0.1.8.tar` & `ns_asphalt9-0.2.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:57:11.654570 ns_asphalt9-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-24 10:57:11.654570 ns_asphalt9-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:57:11.650570 ns_asphalt9-0.1.8/ns_asphalt9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:57:11.654570 ns_asphalt9-0.1.8/ns_asphalt9/core/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:57:11.654570 ns_asphalt9-0.1.8/ns_asphalt9/core/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/actions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/actions/enter_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/actions/process_race.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/actions/select_car.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:57:11.654570 ns_asphalt9-0.1.8/ns_asphalt9/core/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23659 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/gui/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:57:11.654570 ns_asphalt9-0.1.8/ns_asphalt9/core/gui/images/
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/gui/images/help.png
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/gui/images/home.png
--rw-r--r--   0 runner    (1001) docker     (123)   202347 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/gui/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/gui/images/settings.png
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/page_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:57:11.654570 ns_asphalt9-0.1.8/ns_asphalt9/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/core/utils/track_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/ns_asphalt9/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:57:11.654570 ns_asphalt9-0.1.8/ns_asphalt9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-24 10:57:11.000000 ns_asphalt9-0.1.8/ns_asphalt9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-24 10:57:11.000000 ns_asphalt9-0.1.8/ns_asphalt9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:57:11.000000 ns_asphalt9-0.1.8/ns_asphalt9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 10:57:11.000000 ns_asphalt9-0.1.8/ns_asphalt9.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:57:11.000000 ns_asphalt9-0.1.8/ns_asphalt9.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-24 10:57:11.000000 ns_asphalt9-0.1.8/ns_asphalt9.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 10:57:11.000000 ns_asphalt9-0.1.8/ns_asphalt9.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-24 10:57:11.658570 ns_asphalt9-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:57:11.654570 ns_asphalt9-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-24 10:56:59.000000 ns_asphalt9-0.1.8/tests/test_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:00:49.075386 ns_asphalt9-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-29 04:00:49.075386 ns_asphalt9-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:00:49.067386 ns_asphalt9-0.2.0/ns_asphalt9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:00:49.071386 ns_asphalt9-0.2.0/ns_asphalt9/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:00:49.071386 ns_asphalt9-0.2.0/ns_asphalt9/core/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/actions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/actions/enter_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/actions/process_race.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/actions/select_car.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:00:49.071386 ns_asphalt9-0.2.0/ns_asphalt9/core/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27238 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/gui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:00:49.071386 ns_asphalt9-0.2.0/ns_asphalt9/core/gui/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/gui/images/help.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/gui/images/home.png
+-rw-r--r--   0 runner    (1001) docker     (123)   202347 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/gui/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/gui/images/settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/page_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:00:49.075386 ns_asphalt9-0.2.0/ns_asphalt9/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41726 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/utils/track_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25358 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/core/utils/track_navi_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/ns_asphalt9/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:00:49.071386 ns_asphalt9-0.2.0/ns_asphalt9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-29 04:00:49.000000 ns_asphalt9-0.2.0/ns_asphalt9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-29 04:00:49.000000 ns_asphalt9-0.2.0/ns_asphalt9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 04:00:49.000000 ns_asphalt9-0.2.0/ns_asphalt9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-29 04:00:49.000000 ns_asphalt9-0.2.0/ns_asphalt9.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 04:00:48.000000 ns_asphalt9-0.2.0/ns_asphalt9.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-29 04:00:49.000000 ns_asphalt9-0.2.0/ns_asphalt9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-29 04:00:49.000000 ns_asphalt9-0.2.0/ns_asphalt9.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-29 04:00:49.075386 ns_asphalt9-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:00:49.075386 ns_asphalt9-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-29 04:00:37.000000 ns_asphalt9-0.2.0/tests/test_pages.py
```

### Comparing `ns_asphalt9-0.1.8/LICENSE` & `ns_asphalt9-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.8/PKG-INFO` & `ns_asphalt9-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 0.1.8
+Version: 0.2.0
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.1.8/README.md` & `ns_asphalt9-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/core/actions/common.py` & `ns_asphalt9-0.2.0/ns_asphalt9/core/actions/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 from ..controller import pro, Buttons
-from .. import globals
+from .. import globals, consts
 
 
 def connect_controller():
     """连接手柄"""
     pro.press_buttons([Buttons.L, Buttons.R], down=1)
     time.sleep(1)
     pro.press_buttons([Buttons.A], down=0.5)
@@ -43,7 +43,20 @@
 def system_error():
     pro.press_group([Buttons.A] * 3, 3)
     _add_task()
 
 
 def loading_game():
     _add_task()
+
+
+def get_race_mode():
+    mode = globals.MODE if globals.MODE else globals.CONFIG["模式"]
+    if mode in [consts.mp_zh, consts.mp1_zh]:
+        if globals.CONFIG["模式"] == consts.mp3_zh:
+            return consts.mp3_zh
+        elif globals.CONFIG["模式"] == consts.mp2_zh:
+            return consts.mp2_zh
+        else:
+            return consts.mp1_zh
+    else:
+        return mode
```

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/core/actions/enter_page.py` & `ns_asphalt9-0.2.0/ns_asphalt9/core/actions/enter_page.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/core/actions/select_car.py` & `ns_asphalt9-0.2.0/ns_asphalt9/core/actions/select_car.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from .. import consts, globals, tasks
 from ..actions import process_race
 from ..controller import Buttons, pro
 from ..ocr import OCR
 from ..utils.log import logger
 from ..tasks import TaskManager
+from .common import get_race_mode
 
 
 def world_series_reset():
     division = globals.DIVISION
     if not division:
         division = "青铜"
     config = globals.CONFIG["多人一"][division]
@@ -66,23 +67,22 @@
 
 
 def legendary_hunt_position():
     return globals.CONFIG["传奇寻车"]["车库位置"]
 
 
 def get_race_config():
-    mode = globals.MODE if globals.MODE else globals.CONFIG["模式"]
+    mode = get_race_mode()
     logger.info(f"Get mode {mode} config.")
-    if mode in [consts.mp_zh, consts.mp1_zh]:
-        if globals.CONFIG["模式"] == consts.mp3_zh:
-            return mp3_position(), other_series_reset, consts.mp3_zh
-        elif globals.CONFIG["模式"] == consts.mp2_zh:
-            return other_series_position(), other_series_reset, consts.mp2_zh
-        else:
-            return world_series_positions(), world_series_reset, consts.mp1_zh
+    if mode == consts.mp3_zh:
+        return mp3_position(), other_series_reset, consts.mp3_zh
+    elif mode == consts.mp2_zh:
+        return other_series_position(), other_series_reset, consts.mp2_zh
+    elif mode == consts.mp1_zh:
+        return world_series_positions(), world_series_reset, consts.mp1_zh
     elif mode == consts.car_hunt_zh:
         return carhunt_position(), carhunt_reset, mode
     elif mode == consts.legendary_hunt_zh:
         return legendary_hunt_position(), carhunt_reset, mode
     else:
         return default_positions(), default_reset, mode
```

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/core/cache.py` & `ns_asphalt9-0.2.0/ns_asphalt9/core/cache.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/core/consts.py` & `ns_asphalt9-0.2.0/ns_asphalt9/core/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,16 @@
 grand_prix = "grand_prix"
 # 通行证页
 legend_pass = "legend_pass"
 # 无多人
 no_mp = "no_mp"
 # error code
 error_code = "error_code"
+# 选择用户
+select_user = "select_user"
 
 
 # 键盘与手柄映射
 KEY_MAPPING = {
     "6": "MINUS",
     "7": "PLUS",
     "[": "CAPTURE",
```

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/core/controller.py` & `ns_asphalt9-0.2.0/ns_asphalt9/core/controller.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/core/globals.py` & `ns_asphalt9-0.2.0/ns_asphalt9/core/globals.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/core/gui/app.py` & `ns_asphalt9-0.2.0/ns_asphalt9/core/gui/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,29 +174,49 @@
                 task_combobox.set(self.settings_data["任务"][row]["间隔"])
 
             self.setting_modules["任务"].append(
                 {"名称": task, "运行": task_box, "间隔": task_combobox}
             )
 
         # 多人一配置
-        self.tabview = customtkinter.CTkTabview(self.settings, width=340)
-        self.tabview.grid(
-            row=2, column=1, columnspan=2, padx=(20, 0), pady=(20, 0), sticky="nsew"
-        )
+        mp1_frame = customtkinter.CTkFrame(self.settings, width=340)
+        mp1_frame.grid(row=2, column=1, padx=(20, 0), pady=(20, 0), sticky="nsew")
 
         self.setting_modules["多人一"] = {}
 
+        navi_label = customtkinter.CTkLabel(
+            master=mp1_frame, text="自动选路:"
+        )
+        navi_label.grid(row=0, column=0, padx=10, pady=(10, 10))
+
+        enable_navi = customtkinter.CTkCheckBox(
+            master=mp1_frame, text="是否开启自动选路", command=self.save_settings
+        )
+        enable_navi.grid(row=0, column=1, pady=(10, 10), padx=(20, 0), sticky="ew")
+
+        self.setting_modules["多人一"]["自动选路"] = enable_navi
+
+        if self.settings_data and "自动选路" in self.settings_data["多人一"]:
+            if self.settings_data["多人一"]["自动选路"]:
+                enable_navi.select()
+
+        self.tabview = customtkinter.CTkTabview(mp1_frame, width=340)
+        self.tabview.grid(
+            row=1, column=0, columnspan=2, padx=(20, 0), pady=(20, 0), sticky="nsew"
+        )
+
         tabs = ["青铜", "白银", "黄金", "铂金"]
         for tab_index, tab_name in enumerate(tabs):
             self.setting_modules["多人一"][tab_name] = {}
             self.tabview.add(tab_name)
+
             car_level = customtkinter.CTkLabel(
                 master=self.tabview.tab(tab_name), text="车库等级:"
             )
-            car_level.grid(row=0, column=0, padx=10, pady=(10, 10))
+            car_level.grid(row=1, column=0, padx=10, pady=(10, 10))
             option_level = customtkinter.CTkOptionMenu(
                 self.tabview.tab(tab_name),
                 dynamic_resizing=False,
                 values=tabs[: tab_index + 1],
                 width=100,
                 height=28,
                 command=self.save_settings,
@@ -255,28 +275,43 @@
                 )
 
         # 多人二配置
         mp2_settings_frame = customtkinter.CTkFrame(self.settings, width=340)
         mp2_settings_frame.grid(
             row=3, column=1, columnspan=2, padx=(20, 0), pady=(20, 0), sticky="nsew"
         )
+        self.setting_modules["多人二"] = {}
+        navi_label = customtkinter.CTkLabel(
+                master=mp2_settings_frame, text="自动选路:"
+            )
+        navi_label.grid(row=0, column=0, padx=10, pady=(10, 10))
+
+        enable_navi = customtkinter.CTkCheckBox(
+            master=mp2_settings_frame, text="是否开启自动选路", command=self.save_settings
+        )
+        enable_navi.grid(row=0, column=1, pady=(10, 10), padx=(20, 0), sticky="ew")
+
+        self.setting_modules["多人二"]["自动选路"] = enable_navi
+
+        if self.settings_data and "自动选路" in self.settings_data["多人二"]:
+            if self.settings_data["多人二"]["自动选路"]:
+                enable_navi.select()
 
         car_position = customtkinter.CTkLabel(master=mp2_settings_frame, text="车库位置:")
 
         car_position.grid(row=1, column=0, padx=(15, 10), pady=(10, 10))
 
         row = customtkinter.CTkLabel(master=mp2_settings_frame, text="row")
 
         row.grid(row=1, column=1, padx=(0, 0), pady=(10, 10), sticky="nsew")
 
         col = customtkinter.CTkLabel(master=mp2_settings_frame, text="col")
 
         col.grid(row=1, column=2, padx=(0, 10), pady=(10, 10), sticky="nsew")
 
-        self.setting_modules["多人二"] = {}
         self.setting_modules["多人二"]["车库位置"] = []
 
         for r in range(6):
             option1 = customtkinter.CTkOptionMenu(
                 mp2_settings_frame,
                 dynamic_resizing=False,
                 values=[str(i) for i in range(0, 3)],
@@ -306,14 +341,30 @@
         # 寻车配置
         self.setting_modules["寻车"] = {}
         carhunt_setting_frame = customtkinter.CTkFrame(self.settings, width=340)
         carhunt_setting_frame.grid(
             row=4, column=1, columnspan=2, padx=(20, 0), pady=(20, 20), sticky="nsew"
         )
 
+        navi_label = customtkinter.CTkLabel(
+                master=carhunt_setting_frame, text="自动选路:"
+            )
+        navi_label.grid(row=0, column=0, padx=10, pady=(10, 10))
+
+        enable_navi = customtkinter.CTkCheckBox(
+            master=carhunt_setting_frame, text="是否开启自动选路", command=self.save_settings
+        )
+        enable_navi.grid(row=0, column=1, pady=(10, 10), padx=(20, 0), sticky="ew")
+
+        self.setting_modules["寻车"]["自动选路"] = enable_navi
+
+        if self.settings_data and "自动选路" in self.settings_data["寻车"]:
+            if self.settings_data["寻车"]["自动选路"]:
+                enable_navi.select()
+
         car_hunt_position = customtkinter.CTkLabel(
             master=carhunt_setting_frame, text="寻车位置:"
         )
         car_hunt_position.grid(row=1, column=0, padx=(15, 10), pady=(10, 10))
         position_option = customtkinter.CTkOptionMenu(
             carhunt_setting_frame,
             dynamic_resizing=False,
@@ -375,14 +426,30 @@
         # 传奇寻车配置
         self.setting_modules["传奇寻车"] = {}
         carhunt_setting_frame = customtkinter.CTkFrame(self.settings, width=340)
         carhunt_setting_frame.grid(
             row=5, column=1, columnspan=2, padx=(20, 0), pady=(20, 20), sticky="nsew"
         )
 
+        navi_label = customtkinter.CTkLabel(
+            master=carhunt_setting_frame, text="自动选路:"
+        )
+        navi_label.grid(row=0, column=0, padx=10, pady=(10, 10))
+
+        enable_navi = customtkinter.CTkCheckBox(
+            master=carhunt_setting_frame, text="是否开启自动选路", command=self.save_settings
+        )
+        enable_navi.grid(row=0, column=1, pady=(10, 10), padx=(20, 0), sticky="ew")
+
+        self.setting_modules["传奇寻车"]["自动选路"] = enable_navi
+
+        if self.settings_data and "自动选路" in self.settings_data["传奇寻车"]:
+            if self.settings_data["传奇寻车"]["自动选路"]:
+                enable_navi.select()
+
         car_hunt_position = customtkinter.CTkLabel(
             master=carhunt_setting_frame, text="寻车位置:"
         )
         car_hunt_position.grid(row=1, column=0, padx=(15, 10), pady=(10, 10))
         position_option = customtkinter.CTkOptionMenu(
             carhunt_setting_frame,
             dynamic_resizing=False,
@@ -441,32 +508,48 @@
                     option2.set(self.settings_data["传奇寻车"]["车库位置"][r]["col"])
             except IndexError:
                 pass
 
             self.setting_modules["传奇寻车"]["车库位置"].append({"row": option1, "col": option2})
 
         # 多人三配置
+        self.setting_modules["多人三"] = {}
         mp3_settings_frame = customtkinter.CTkFrame(self.settings, width=340)
         mp3_settings_frame.grid(
             row=6, column=1, columnspan=2, padx=(20, 0), pady=(20, 0), sticky="nsew"
         )
 
+        navi_label = customtkinter.CTkLabel(
+            master=mp3_settings_frame, text="自动选路:"
+        )
+        navi_label.grid(row=0, column=0, padx=10, pady=(10, 10))
+
+        enable_navi = customtkinter.CTkCheckBox(
+            master=mp3_settings_frame, text="是否开启自动选路", command=self.save_settings
+        )
+        enable_navi.grid(row=0, column=1, pady=(10, 10), padx=(20, 0), sticky="ew")
+
+        self.setting_modules["多人三"]["自动选路"] = enable_navi
+
+        if self.settings_data and "自动选路" in self.settings_data["多人三"]:
+            if self.settings_data["多人三"]["自动选路"]:
+                enable_navi.select()
+
         car_position = customtkinter.CTkLabel(master=mp3_settings_frame, text="车库位置:")
 
         car_position.grid(row=1, column=0, padx=(15, 10), pady=(10, 10))
 
         row = customtkinter.CTkLabel(master=mp3_settings_frame, text="row")
 
         row.grid(row=1, column=1, padx=(0, 0), pady=(10, 10), sticky="nsew")
 
         col = customtkinter.CTkLabel(master=mp3_settings_frame, text="col")
 
         col.grid(row=1, column=2, padx=(0, 10), pady=(10, 10), sticky="nsew")
 
-        self.setting_modules["多人三"] = {}
         self.setting_modules["多人三"]["车库位置"] = []
 
         for r in range(6):
             option1 = customtkinter.CTkOptionMenu(
                 mp3_settings_frame,
                 dynamic_resizing=False,
                 values=[str(i) for i in range(0, 3)],
```

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/core/gui/images/help.png` & `ns_asphalt9-0.2.0/ns_asphalt9/core/gui/images/help.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/core/gui/images/home.png` & `ns_asphalt9-0.2.0/ns_asphalt9/core/gui/images/home.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/core/gui/images/logo.png` & `ns_asphalt9-0.2.0/ns_asphalt9/core/gui/images/logo.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/core/gui/images/settings.png` & `ns_asphalt9-0.2.0/ns_asphalt9/core/gui/images/settings.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/core/ocr.py` & `ns_asphalt9-0.2.0/ns_asphalt9/core/ocr.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,18 +63,19 @@
         logger.info(f"ocr page map result = {text}")
         for track in track_data:
             if track["tracken"] in text:
                 logger.info(f"Get track = {track}")
                 return track
 
     @classmethod
-    def get_progress(cls):
+    def get_progress(cls, image_path):
         """识别进度"""
-        screenshot()
-        text = cls._get_text(crop=(150, 80, 400, 140), replace=True)
+        text = cls._get_text(
+            crop=(150, 80, 400, 140), replace=True, image_path=image_path
+        )
         pattern = r"\b\d{1,3}\b"
         match = re.search(pattern, text)
         if match:
             return int(match.group())
         return -1
 
     @classmethod
@@ -89,20 +90,21 @@
             filter=ImageFilter.SHARPEN,
             convert="L",
             replace=True,
         )
         return "PLAY" in text
 
     @classmethod
-    def has_next(cls):
+    def has_next(cls, image_path=""):
         """是否有NEXT按钮"""
         text = cls._get_text(
             crop=(1460, 900, 1750, 1040),
             filter=ImageFilter.SHARPEN,
             replace=True,
+            image_path=image_path,
         )
         return "NEXT" in text
 
     @classmethod
     def get_ticket(cls):
         """获取票数"""
         text = cls._get_text(
@@ -138,17 +140,25 @@
         )
         if re.findall("LEGENDARY HUNT(?!\sRIOT)", text):
             return True
         return False
 
     @classmethod
     def _get_text(
-        cls, crop=None, filter=None, convert=None, replace=None, config="--dpi 72"
+        cls,
+        crop=None,
+        filter=None,
+        convert=None,
+        replace=None,
+        config="--dpi 72",
+        image_path="",
     ):
-        img = Image.open(cls.filename)
+        if not image_path:
+            image_path = cls.filename
+        img = Image.open(image_path)
         if crop:
             img = img.crop(crop)
         if filter:
             img = img.filter(filter)
         if convert:
             img = img.convert(convert)
         text: str = pytesseract.image_to_string(img, lang="eng", config=config)
```

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/core/page_factory.py` & `ns_asphalt9-0.2.0/ns_asphalt9/core/page_factory.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/core/pages.py` & `ns_asphalt9-0.2.0/ns_asphalt9/core/pages.py`

 * *Files 0% similar despite different names*

```diff
@@ -604,7 +604,19 @@
     """无多人任务(大概率是网络问题)"""
 
     name = consts.no_mp
     feature = "NEW MULTIPLAYER SERIES.*COMING SOON"
     part_match = False
 
     action = staticmethod(actions.restart)
+
+
+@cache_decorator("page")
+class SelectUser(Page):
+    """选择用户界面"""
+
+    name = consts.select_user
+    feature = "Select a user"
+    part_match = False
+
+    action = staticmethod(pro.press_button)
+    args = (Buttons.A,)
```

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/core/tasks.py` & `ns_asphalt9-0.2.0/ns_asphalt9/core/tasks.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/core/utils/decorator.py` & `ns_asphalt9-0.2.0/ns_asphalt9/core/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/core/utils/log.py` & `ns_asphalt9-0.2.0/ns_asphalt9/core/utils/log.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/core/utils/timer.py` & `ns_asphalt9-0.2.0/ns_asphalt9/core/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9/main.py` & `ns_asphalt9-0.2.0/ns_asphalt9/main.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9.egg-info/PKG-INFO` & `ns_asphalt9-0.2.0/ns_asphalt9.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns-asphalt9
-Version: 0.1.8
+Version: 0.2.0
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.1.8/ns_asphalt9.egg-info/SOURCES.txt` & `ns_asphalt9-0.2.0/ns_asphalt9.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,8 +33,9 @@
 ns_asphalt9/core/gui/images/logo.png
 ns_asphalt9/core/gui/images/settings.png
 ns_asphalt9/core/utils/__init__.py
 ns_asphalt9/core/utils/decorator.py
 ns_asphalt9/core/utils/log.py
 ns_asphalt9/core/utils/timer.py
 ns_asphalt9/core/utils/track_data.py
+ns_asphalt9/core/utils/track_navi_data.py
 tests/test_pages.py
```

### Comparing `ns_asphalt9-0.1.8/setup.cfg` & `ns_asphalt9-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nxbt
-version = 0.1.8
+version = 0.2.0
 author = codehai
 author-email = wmpksb@gmail.com
 project_urls = 
 	Code = https://github.com/codehai/ns_asphalt9
 	Issue tracker = https://github.com/codehai/ns_asphalt9/issues
 license = GNU General Public License v3 (GPLv3)
 license-file = LICENSE
```

### Comparing `ns_asphalt9-0.1.8/tests/test_pages.py` & `ns_asphalt9-0.2.0/tests/test_pages.py`

 * *Files identical despite different names*

