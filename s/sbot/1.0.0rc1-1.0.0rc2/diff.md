# Comparing `tmp/sbot-1.0.0rc1.tar.gz` & `tmp/sbot-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbot-1.0.0rc1.tar", last modified: Mon Jul  3 20:11:02 2023, max compression
+gzip compressed data, was "sbot-1.0.0rc2.tar", last modified: Sat Jul 29 14:21:38 2023, max compression
```

## Comparing `sbot-1.0.0rc1.tar` & `sbot-1.0.0rc2.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.747489 sbot-1.0.0rc1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.747489 sbot-1.0.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/.github/workflows/test_build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.747489 sbot-1.0.0rc1/sbot/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-03 20:11:02.000000 sbot-1.0.0rc1/sbot/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/arduino.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/game_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/motor_board.py
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/power_board.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/robot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/serial_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/servo_board.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.747489 sbot-1.0.0rc1/sbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-03 20:11:02.000000 sbot-1.0.0rc1/sbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-03 20:11:02.000000 sbot-1.0.0rc1/sbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:11:02.000000 sbot-1.0.0rc1/sbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-03 20:11:02.000000 sbot-1.0.0rc1/sbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 20:11:02.000000 sbot-1.0.0rc1/sbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9535 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_arduino.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.743489 sbot-1.0.0rc1/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/tests/test_data/bad/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_data/bad/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/tests/test_data/empty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_data/empty/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/tests/test_data/missing_key/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_data/missing_key/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.743489 sbot-1.0.0rc1/tests/test_data/nested/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/tests/test_data/nested/valid/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_data/nested/valid/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/tests/test_data/not_object/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_data/not_object/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/tests/test_data/valid/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_data/valid/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9968 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_motor_board.py
--rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_power_board.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_sbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_serial_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_servo_board.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.508319 sbot-1.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.492318 sbot-1.0.0rc2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.496318 sbot-1.0.0rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/.github/workflows/test_build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-07-29 14:21:38.508319 sbot-1.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.500318 sbot-1.0.0rc2/sbot/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-29 14:21:38.000000 sbot-1.0.0rc2/sbot/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/arduino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/game_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/motor_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/power_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/serial_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/servo_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.500318 sbot-1.0.0rc2/sbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-07-29 14:21:38.000000 sbot-1.0.0rc2/sbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-29 14:21:38.000000 sbot-1.0.0rc2/sbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 14:21:38.000000 sbot-1.0.0rc2/sbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-29 14:21:38.000000 sbot-1.0.0rc2/sbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-29 14:21:38.000000 sbot-1.0.0rc2/sbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 14:21:38.508319 sbot-1.0.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.504318 sbot-1.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9535 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_arduino.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.492318 sbot-1.0.0rc2/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.504318 sbot-1.0.0rc2/tests/test_data/bad/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_data/bad/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.504318 sbot-1.0.0rc2/tests/test_data/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_data/empty/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.504318 sbot-1.0.0rc2/tests/test_data/missing_key/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_data/missing_key/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.492318 sbot-1.0.0rc2/tests/test_data/nested/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.504318 sbot-1.0.0rc2/tests/test_data/nested/valid/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_data/nested/valid/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.504318 sbot-1.0.0rc2/tests/test_data/not_object/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_data/not_object/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.504318 sbot-1.0.0rc2/tests/test_data/valid/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_data/valid/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9968 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_motor_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_power_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_sbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_serial_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_servo_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_timeout.py
```

### Comparing `sbot-1.0.0rc1/.github/dependabot.yml` & `sbot-1.0.0rc2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc1/.github/workflows/test_build.yml` & `sbot-1.0.0rc2/.github/workflows/test_build.yml`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc1/.gitignore` & `sbot-1.0.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc1/LICENSE` & `sbot-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc1/PKG-INFO` & `sbot-1.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbot
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: The robot API for the Smallpeice summer school
 Author-email: SourceBots <hello@sourcebots.co.uk>
 License: MIT License
         
         Copyright (c) 2019-21 Dan Trickey
         Copyright (c) 2023 SourceBots
         
@@ -77,22 +77,22 @@
 
 from sbot import Robot
 
 r = Robot()
 
 ```
 
-To disable the waiting for the start button, you can pass `wait_start=False` to the constructor.
-The `wait_start` method needs to be called before the metadata is available.
+To disable the waiting for the start button, you can pass `wait_for_start=False` to the constructor.
+The `wait_for_start` method needs to be called before the metadata is available.
 
 ```python
 
 from sbot import Robot
 
-r = Robot(wait_start=False)
+r = Robot(wait_for_start=False)
 
 # Setup in here
 
 r.wait_start()
 
 ```
```

### Comparing `sbot-1.0.0rc1/README.md` & `sbot-1.0.0rc2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,22 +35,22 @@
 
 from sbot import Robot
 
 r = Robot()
 
 ```
 
-To disable the waiting for the start button, you can pass `wait_start=False` to the constructor.
-The `wait_start` method needs to be called before the metadata is available.
+To disable the waiting for the start button, you can pass `wait_for_start=False` to the constructor.
+The `wait_for_start` method needs to be called before the metadata is available.
 
 ```python
 
 from sbot import Robot
 
-r = Robot(wait_start=False)
+r = Robot(wait_for_start=False)
 
 # Setup in here
 
 r.wait_start()
 
 ```
```

### Comparing `sbot-1.0.0rc1/pyproject.toml` & `sbot-1.0.0rc2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,16 @@
 authors = [{name = "SourceBots", email =  "hello@sourcebots.co.uk"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 dynamic = ["version"]
 requires-python = ">=3.8"
 dependencies = [
     "pyserial >=3,<4",
-    "april_vision >=2,<3",
+    "april_vision >=2.0.2,<3",
+    "typing-extensions; python_version<'3.10'",
 ]
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
     "Typing :: Typed",
     "Topic :: Education",
@@ -71,12 +72,11 @@
 [project.optional-dependencies]
 dev = [
     "flake8",
     "isort",
     "mypy",
     "build",
     "types-pyserial",
-    "typing-extensions; python_version<'3.10'",
     "pytest",
     "pytest-cov",
 ]
 vision = ["opencv-python-headless >=4,<5"]
```

### Comparing `sbot-1.0.0rc1/sbot/__init__.py` & `sbot-1.0.0rc2/sbot/__init__.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc1/sbot/arduino.py` & `sbot-1.0.0rc2/sbot/arduino.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc1/sbot/camera.py` & `sbot-1.0.0rc2/sbot/camera.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """An implementation of a camera board using the april_vision library."""
 import logging
 from pathlib import Path
 from typing import Callable, Dict, Iterable, List, Optional, Union
 
+from april_vision import CalibratedCamera, Frame
+from april_vision import Marker as AprilMarker
 from april_vision import (
-    CalibratedCamera, Frame, Marker, Processor, USBCamera, __version__,
-    calibrations, find_cameras, generate_marker_size_mapping,
+    Processor, USBCamera, __version__, calibrations,
+    find_cameras, generate_marker_size_mapping,
 )
 from april_vision.helpers import Base64Sender
 from numpy.typing import NDArray
 
+from .marker import Marker
 from .utils import Board, BoardIdentity
 
 LOGGER = logging.getLogger(__name__)
 
 
 class AprilCamera(Board):
     """
@@ -101,15 +104,16 @@
         Capture an image and identify fiducial markers.
 
         :param eager: Process the pose estimations of markers immediately,
             currently unused.
         :param frame: An image to detect markers in, instead of capturing a new one,
         :returns: list of markers that the camera could see.
         """
-        return self._cam.see(frame=frame)
+        markers = self._cam.see(frame=frame)
+        return [Marker.from_april_vision_marker(marker) for marker in markers]
 
     def capture(self) -> NDArray:
         """
         Get the raw image data from the camera.
 
         :returns: Camera pixel data
         """
@@ -136,15 +140,18 @@
         If a dict is given for tag_sizes, only marker IDs that are keys of the
         dict will be detected.
 
         :param tag_sizes: The size of the tags to use for pose estimation given in meters.
         """
         self._cam.set_marker_sizes(tag_sizes)
 
-    def _set_detection_hook(self, callback: Callable[[Frame, List[Marker]], None]) -> None:
+    def _set_detection_hook(
+        self,
+        callback: Callable[[Frame, List[AprilMarker]], None],
+    ) -> None:
         """
         Setup a callback to be run after each detection.
 
         The callback will be passed the frame and the list of markers that were detected.
 
         :param callback: The function to run after each detection.
         """
```

### Comparing `sbot-1.0.0rc1/sbot/exceptions.py` & `sbot-1.0.0rc2/sbot/exceptions.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc1/sbot/logging.py` & `sbot-1.0.0rc2/sbot/logging.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc1/sbot/metadata.py` & `sbot-1.0.0rc2/sbot/metadata.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc1/sbot/motor_board.py` & `sbot-1.0.0rc2/sbot/motor_board.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc1/sbot/power_board.py` & `sbot-1.0.0rc2/sbot/power_board.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc1/sbot/robot.py` & `sbot-1.0.0rc2/sbot/robot.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,30 +26,30 @@
     """
     The main robot class that provides access to all the boards.
 
     There can be only one instance of this class active in your operating
     system at a time, creating a second instance will raise an OSError.
 
     :param debug: Enable debug logging to the console, defaults to False
-    :param wait_start: Wait in the constructor until the start button is pressed,
+    :param wait_for_start: Wait in the constructor until the start button is pressed,
         defaults to True
     :param trace_logging: Enable trace level logging to the console, defaults to False
     :param manual_boards: A dictionary of board types to a list of serial port paths
         to allow for connecting to boards that are not automatically detected, defaults to None
     """
     __slots__ = (
         '_lock', '_metadata', '_power_board', '_motor_boards', '_servo_boards',
         '_arduinos', '_cameras',
     )
 
     def __init__(
         self,
         *,
         debug: bool = False,
-        wait_start: bool = True,
+        wait_for_start: bool = True,
         trace_logging: bool = False,
         manual_boards: dict[str, list[str]] | None = None,
     ) -> None:
         self._lock = obtain_lock()
         self._metadata: Metadata | None = None
 
         setup_logging(debug, trace_logging)
@@ -61,15 +61,15 @@
             self._init_aux_boards(manual_boards)
         else:
             self._init_power_board()
             self._init_aux_boards()
         self._init_camera()
         self._log_connected_boards()
 
-        if wait_start:
+        if wait_for_start:
             self.wait_start()
 
     def _init_power_board(self, manual_boards: list[str] | None = None) -> None:
         """
         Locate the PowerBoard and enable all the outputs to power the other boards.
 
         :param manual_boards: Serial port paths to also check for power boards,
```

### Comparing `sbot-1.0.0rc1/sbot/serial_wrapper.py` & `sbot-1.0.0rc2/sbot/serial_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
             :return: The return value of the original function.
             """
             attempt = 0
             while attempt < times:
                 try:
                     return func(*args, **kwargs)
                 except exceptions:
+                    time.sleep(attempt * 0.5)
                     attempt += 1
             return func(*args, **kwargs)
         return retryfn
     return decorator
 
 
 class SerialWrapper:
```

### Comparing `sbot-1.0.0rc1/sbot/servo_board.py` & `sbot-1.0.0rc2/sbot/servo_board.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc1/sbot/timeout.py` & `sbot-1.0.0rc2/sbot/timeout.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,59 @@
 """Functions for killing the robot after a certain amount of time."""
 import logging
+import os
 import signal
 import sys
+from threading import Timer
 from types import FrameType
+from typing import Optional
 
 logger = logging.getLogger(__name__)
 
-# TODO make this work on Windows
 
-
-def timeout_handler(signal_type: signal.Signals, stack_frame: FrameType) -> None:
+def timeout_handler(signal_type: int, stack_frame: Optional[FrameType]) -> None:
     """
-    Handle the `SIGALRM` to kill the current process.
+    Handle the timeout to kill the current process.
 
     This function is called when the timeout expires and will stop the robot's main process.
     In order for this to work, any threads that are created must be daemons.
 
     NOTE: This function is not called on Windows.
 
     :param signal_type: The sginal that triggered this handler
     :param stack_frame: The stack frame at the time of the signal
-    :raises SystemExit: To stop the robot's execution after the timeout
     """
-    raise SystemExit("Timeout expired: Game Over!")
+    logger.info("Timeout expired: Game Over!")
+    exit(0)
+
+
+def win_timeout_handler() -> None:
+    """
+    Kill the main process on Windows.
+
+    This function is called when the timeout expires and will stop the robot's main process.
+    In order for this to work, any threads that are created must be daemons.
+
+    NOTE: This function is only called on Windows.
+    """
+    logger.info("Timeout expired: Game Over!")
+    os.kill(os.getpid(), signal.SIGTERM)
 
 
 def kill_after_delay(timeout_seconds: int) -> None:
     """
     Kill the robot after a certain amount of time.
 
     Interrupts main process after the given delay.
 
-    NOTE: This functionality does not work on Windows,
-    so the robot will not stop after the timeout.
-
     :param timeout_seconds: The number of seconds to wait before killing the robot
     """
+
     if sys.platform == "win32":
-        logger.warning(
-            "Game timeout is not supported on Windows. "
-            "The code will not stop after the timeout.")
+        # Windows doesn't have SIGALRM,
+        # so we approximate its functionality using a delayed SIGTERM
+        timer = Timer(timeout_seconds, win_timeout_handler)
+        timer.start()
     else:
-        logger.debug(f"Kill Signal Timeout set: {timeout_seconds}s")
-        signal.signal(signal.SIGALRM, timeout_handler)  # type: ignore
+        signal.signal(signal.SIGALRM, timeout_handler)
         signal.alarm(timeout_seconds)
+    logger.debug(f"Kill Signal Timeout set: {timeout_seconds}s")
```

### Comparing `sbot-1.0.0rc1/sbot/utils.py` & `sbot-1.0.0rc2/sbot/utils.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc1/sbot.egg-info/PKG-INFO` & `sbot-1.0.0rc2/sbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbot
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: The robot API for the Smallpeice summer school
 Author-email: SourceBots <hello@sourcebots.co.uk>
 License: MIT License
         
         Copyright (c) 2019-21 Dan Trickey
         Copyright (c) 2023 SourceBots
         
@@ -77,22 +77,22 @@
 
 from sbot import Robot
 
 r = Robot()
 
 ```
 
-To disable the waiting for the start button, you can pass `wait_start=False` to the constructor.
-The `wait_start` method needs to be called before the metadata is available.
+To disable the waiting for the start button, you can pass `wait_for_start=False` to the constructor.
+The `wait_for_start` method needs to be called before the metadata is available.
 
 ```python
 
 from sbot import Robot
 
-r = Robot(wait_start=False)
+r = Robot(wait_for_start=False)
 
 # Setup in here
 
 r.wait_start()
 
 ```
```

### Comparing `sbot-1.0.0rc1/sbot.egg-info/SOURCES.txt` & `sbot-1.0.0rc2/sbot.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 sbot/__init__.py
 sbot/_version.py
 sbot/arduino.py
 sbot/camera.py
 sbot/exceptions.py
 sbot/game_specific.py
 sbot/logging.py
+sbot/marker.py
 sbot/metadata.py
 sbot/motor_board.py
 sbot/power_board.py
 sbot/py.typed
 sbot/robot.py
 sbot/serial_wrapper.py
 sbot/servo_board.py
```

### Comparing `sbot-1.0.0rc1/tests/conftest.py` & `sbot-1.0.0rc2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc1/tests/test_arduino.py` & `sbot-1.0.0rc2/tests/test_arduino.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc1/tests/test_metadata.py` & `sbot-1.0.0rc2/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc1/tests/test_motor_board.py` & `sbot-1.0.0rc2/tests/test_motor_board.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc1/tests/test_power_board.py` & `sbot-1.0.0rc2/tests/test_power_board.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc1/tests/test_sbot.py` & `sbot-1.0.0rc2/tests/test_sbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
     # Test that we can obtain a lock before creating a robot object
     lock = obtain_lock()
     assert isinstance(lock, socket.socket)
     lock.close()  # release the lock
 
     # Test that we can create a robot object
-    r = Robot(wait_start=False, manual_boards=manual_boards, debug=True)
+    r = Robot(wait_for_start=False, manual_boards=manual_boards, debug=True)
     assert caplog.record_tuples[1:] == [
         # First line contains the version number
         ('sbot.robot', logging.INFO, 'Found PowerBoard, serial: POW123'),
         ('sbot.robot', logging.INFO, 'Found MotorBoard, serial: MOT123'),
         ('sbot.robot', logging.INFO, 'Found ServoBoard, serial: TEST123'),
         ('sbot.robot', logging.INFO, 'Found Arduino, serial: test://'),
     ]
@@ -123,15 +123,15 @@
 
 
 @pytest.hookimpl(trylast=True)
 @pytest.mark.hardware
 def test_robot_discovery() -> None:
     """Test that we can discover all the boards when creating a Robot object."""
     from sbot import Robot
-    robot = Robot(wait_start=False)
+    robot = Robot(wait_for_start=False)
 
     # Test that we can access the singular boards
     power_asset_tag = robot.power_board.identify().asset_tag
     servo_asset_tag = robot.servo_board.identify().asset_tag
     motor_asset_tag = robot.motor_board.identify().asset_tag
 
     # Test that we can access the boards by asset tag
```

### Comparing `sbot-1.0.0rc1/tests/test_serial_wrapper.py` & `sbot-1.0.0rc2/tests/test_serial_wrapper.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc1/tests/test_servo_board.py` & `sbot-1.0.0rc2/tests/test_servo_board.py`

 * *Files identical despite different names*

