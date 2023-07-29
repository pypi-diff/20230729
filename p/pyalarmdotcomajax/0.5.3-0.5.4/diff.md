# Comparing `tmp/pyalarmdotcomajax-0.5.3.tar.gz` & `tmp/pyalarmdotcomajax-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalarmdotcomajax-0.5.3.tar", last modified: Fri Jun  9 01:22:03 2023, max compression
+gzip compressed data, was "pyalarmdotcomajax-0.5.4.tar", last modified: Sat Jul 29 04:22:00 2023, max compression
```

## Comparing `pyalarmdotcomajax-0.5.3.tar` & `pyalarmdotcomajax-0.5.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:22:03.880803 pyalarmdotcomajax-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-06-09 01:22:03.880803 pyalarmdotcomajax-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:22:03.872803 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/
--rw-r--r--   0 runner    (1001) docker     (123)    47043 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20881 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:22:03.876803 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/
--rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/garage_door.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/image_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/water_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22829 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:22:03.876803 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:22:03.880803 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/garage_door.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/water_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:22:03.872803 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-06-09 01:22:03.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-09 01:22:03.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:22:03.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 01:22:03.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-09 01:22:03.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-09 01:22:03.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:22:03.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-09 01:22:03.880803 pyalarmdotcomajax-0.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:22:03.880803 pyalarmdotcomajax-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:22:03.880803 pyalarmdotcomajax-0.5.3/tests/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/tests/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/tests/test_device_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/tests/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/tests/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/tests/test_thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:22:00.508125 pyalarmdotcomajax-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-07-29 04:22:00.508125 pyalarmdotcomajax-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:22:00.504125 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/
+-rw-r--r--   0 runner    (1001) docker     (123)    47043 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20881 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:22:00.504125 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/garage_door.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/image_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22829 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:22:00.504125 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:22:00.508125 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/handler/garage_door.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/handler/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/handler/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/handler/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/handler/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/handler/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/handler/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/handler/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:22:00.504125 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-07-29 04:22:00.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-29 04:22:00.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 04:22:00.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-29 04:22:00.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-29 04:22:00.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 04:22:00.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 04:22:00.000000 pyalarmdotcomajax-0.5.4/pyalarmdotcomajax.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-29 04:22:00.508125 pyalarmdotcomajax-0.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:22:00.508125 pyalarmdotcomajax-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:22:00.508125 pyalarmdotcomajax-0.5.4/tests/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-29 04:21:46.000000 pyalarmdotcomajax-0.5.4/tests/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-29 04:21:47.000000 pyalarmdotcomajax-0.5.4/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-29 04:21:47.000000 pyalarmdotcomajax-0.5.4/tests/test_device_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-29 04:21:47.000000 pyalarmdotcomajax-0.5.4/tests/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-29 04:21:47.000000 pyalarmdotcomajax-0.5.4/tests/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-29 04:21:47.000000 pyalarmdotcomajax-0.5.4/tests/test_thermostat.py
```

### Comparing `pyalarmdotcomajax-0.5.3/LICENSE` & `pyalarmdotcomajax-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/PKG-INFO` & `pyalarmdotcomajax-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalarmdotcomajax
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python Interface for Alarm.com
 Home-page: https://github.com/pyalarmdotcom/pyalarmdotcomajax
 Author: Justin Wong
 Author-email: 46082645+uvjustin@users.noreply.github.com
 Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com, 466460+elahd@users.noreply.github.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.3 Summary: Python
+Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.4 Summary: Python
 Interface for Alarm.com Home-page: https://github.com/pyalarmdotcom/
 pyalarmdotcomajax Author: Justin Wong Author-email:
 46082645+uvjustin@users.noreply.github.com Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
 466460+elahd@users.noreply.github.com License: MIT Keywords: Alarm.com,Security
 System,Home Assistant Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English Classifier: Environment :: Web
```

### Comparing `pyalarmdotcomajax-0.5.3/README.md` & `pyalarmdotcomajax-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/__init__.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     CameraSkybellControllerExtension,
     ConfigurationOption,
     ControllerExtensions_t,
     ExtendedProperties,
 )
 from pyalarmdotcomajax.websockets.client import WebSocketClient, WebSocketState
 
-__version__ = "0.5.3"
+__version__ = "0.5.4"
 
 log = logging.getLogger(__name__)
 
 
 class ExtensionResults(TypedDict):
     """Results of multi-device extension calls."""
```

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/cli.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/cli.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/const.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/const.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/__init__.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/garage_door.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/garage_door.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/gate.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/gate.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/image_sensor.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/image_sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/light.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/light.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/lock.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/lock.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/partition.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/partition.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/registry.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/registry.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/sensor.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/thermostat.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/devices/thermostat.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/exceptions.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/extensions.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/extensions.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/helpers.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/helpers.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/client.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/client.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/const.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/const.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/__init__.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/garage_door.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/handler/garage_door.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/gate.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/handler/gate.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/light.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/handler/light.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/lock.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/handler/lock.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/partition.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/handler/partition.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/sensor.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/handler/sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/thermostat.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/handler/thermostat.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/water_sensor.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/handler/water_sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/messages.py` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax/websockets/messages.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/PKG-INFO` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalarmdotcomajax
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python Interface for Alarm.com
 Home-page: https://github.com/pyalarmdotcom/pyalarmdotcomajax
 Author: Justin Wong
 Author-email: 46082645+uvjustin@users.noreply.github.com
 Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com, 466460+elahd@users.noreply.github.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.3 Summary: Python
+Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.4 Summary: Python
 Interface for Alarm.com Home-page: https://github.com/pyalarmdotcom/
 pyalarmdotcomajax Author: Justin Wong Author-email:
 46082645+uvjustin@users.noreply.github.com Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
 466460+elahd@users.noreply.github.com License: MIT Keywords: Alarm.com,Security
 System,Home Assistant Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English Classifier: Environment :: Web
```

### Comparing `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/SOURCES.txt` & `pyalarmdotcomajax-0.5.4/pyalarmdotcomajax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/pyproject.toml` & `pyalarmdotcomajax-0.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 115
-target-version = ["py310"]
+target-version = ["py311"]
 exclude = 'generated'
 preview = "True"
 
 [tool.mypy]
-python_version = "3.10"
+python_version = "3.11"
 show_error_codes = true
 # follow_imports = "silent"
 ignore_missing_imports = true
 strict_equality = true
 warn_incomplete_stub = true
 warn_redundant_casts = true
 warn_unused_configs = true
@@ -34,15 +34,15 @@
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 norecursedirs = [".git", "testing_config"]
 asyncio_mode = "auto"
 
 [tool.ruff]
-target-version = "py310"
+target-version = "py311"
 unfixable = [
   "F841" # Unused variables
 ]
 exclude = ["examples", "pylint", "build"]
 select = [
   "B007", # Loop control variable {name} not used within loop body
   "B014", # Exception handler with duplicate exception
```

### Comparing `pyalarmdotcomajax-0.5.3/setup.cfg` & `pyalarmdotcomajax-0.5.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/tests/__init__.py` & `pyalarmdotcomajax-0.5.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/tests/conftest.py` & `pyalarmdotcomajax-0.5.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/tests/test_controller.py` & `pyalarmdotcomajax-0.5.4/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/tests/test_device_extensions.py` & `pyalarmdotcomajax-0.5.4/tests/test_device_extensions.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/tests/test_partition.py` & `pyalarmdotcomajax-0.5.4/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/tests/test_sensors.py` & `pyalarmdotcomajax-0.5.4/tests/test_sensors.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.3/tests/test_thermostat.py` & `pyalarmdotcomajax-0.5.4/tests/test_thermostat.py`

 * *Files identical despite different names*

