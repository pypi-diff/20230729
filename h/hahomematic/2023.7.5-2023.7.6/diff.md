# Comparing `tmp/hahomematic-2023.7.5.tar.gz` & `tmp/hahomematic-2023.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2023.7.5.tar", last modified: Tue Jul 25 18:58:55 2023, max compression
+gzip compressed data, was "hahomematic-2023.7.6.tar", last modified: Sat Jul 29 06:40:40 2023, max compression
```

## Comparing `hahomematic-2023.7.5.tar` & `hahomematic-2023.7.6.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:55.973132 hahomematic-2023.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-25 18:58:55.973132 hahomematic-2023.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:55.969132 hahomematic-2023.7.5/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:55.969132 hahomematic-2023.7.5/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)    16932 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/caches/visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    54335 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/central_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    47766 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14829 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (123)    29672 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/json_rpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:55.969132 hahomematic-2023.7.5/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:55.969132 hahomematic-2023.7.5/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    34405 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    26742 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    20557 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:55.969132 hahomematic-2023.7.5/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:55.973132 hahomematic-2023.7.5/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:55.973132 hahomematic-2023.7.5/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/xml_rpc_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:55.969132 hahomematic-2023.7.5/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-25 18:58:55.000000 hahomematic-2023.7.5/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-25 18:58:55.000000 hahomematic-2023.7.5/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:58:55.000000 hahomematic-2023.7.5/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:58:53.000000 hahomematic-2023.7.5/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-25 18:58:55.000000 hahomematic-2023.7.5/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 18:58:55.000000 hahomematic-2023.7.5/hahomematic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-25 18:58:55.973132 hahomematic-2023.7.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:40.512001 hahomematic-2023.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-29 06:40:40.512001 hahomematic-2023.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:40.508001 hahomematic-2023.7.6/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:40.508001 hahomematic-2023.7.6/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16932 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/caches/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55163 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/central_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48392 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27926 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/json_rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:40.508001 hahomematic-2023.7.6/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:40.508001 hahomematic-2023.7.6/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34405 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26754 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20557 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:40.512001 hahomematic-2023.7.6/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:40.512001 hahomematic-2023.7.6/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:40.512001 hahomematic-2023.7.6/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/xml_rpc_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:40.508001 hahomematic-2023.7.6/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-29 06:40:39.000000 hahomematic-2023.7.6/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-29 06:40:40.000000 hahomematic-2023.7.6/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 06:40:39.000000 hahomematic-2023.7.6/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 06:40:38.000000 hahomematic-2023.7.6/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-29 06:40:40.000000 hahomematic-2023.7.6/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-29 06:40:40.000000 hahomematic-2023.7.6/hahomematic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-29 06:40:40.512001 hahomematic-2023.7.6/setup.cfg
```

### Comparing `hahomematic-2023.7.5/LICENSE` & `hahomematic-2023.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/PKG-INFO` & `hahomematic-2023.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.7.5
+Version: 2023.7.6
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.7.5/README.md` & `hahomematic-2023.7.6/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/__init__.py` & `hahomematic-2023.7.6/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/caches/dynamic.py` & `hahomematic-2023.7.6/hahomematic/caches/dynamic.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         """Fetch names from backend."""
         if updated_within_seconds(
             last_update=self._last_updated, max_age_seconds=(MAX_CACHE_AGE / 2)
         ):
             return
         self.clear()
         _LOGGER.debug("load: Loading names for %s", self._central.name)
-        if client := self._central.get_primary_client():
+        if client := self._central.primary_client:
             await client.fetch_device_details()
         _LOGGER.debug("load: Loading rooms for %s", self._central.name)
         self._channel_rooms.clear()
         self._channel_rooms.update(await self._get_all_rooms())
         self._identify_device_room()
         _LOGGER.debug("load: Loading functions for %s", self._central.name)
         self._functions.clear()
@@ -78,25 +78,25 @@
 
     def add_device_channel_id(self, address: str, channel_id: str) -> None:
         """Add channel id for a channel."""
         self._device_channel_ids[address] = channel_id
 
     async def _get_all_rooms(self) -> dict[str, set[str]]:
         """Get all rooms, if available."""
-        if client := self._central.get_primary_client():
+        if client := self._central.primary_client:
             return await client.get_all_rooms()
         return {}
 
     def get_room(self, device_address: str) -> str | None:
         """Return room by device_address."""
         return self._device_room.get(device_address)
 
     async def _get_all_functions(self) -> dict[str, set[str]]:
         """Get all functions, if available."""
-        if client := self._central.get_primary_client():
+        if client := self._central.primary_client:
             return await client.get_all_functions()
         return {}
 
     def get_function_text(self, address: str) -> str | None:
         """Return function by address."""
         if functions := self._functions.get(address):
             return ",".join(functions)
@@ -159,15 +159,15 @@
         """Fetch device data from backend."""
         if updated_within_seconds(
             last_update=self._last_updated, max_age_seconds=(MAX_CACHE_AGE / 2)
         ):
             return
         self.clear()
         _LOGGER.debug("load: device data for %s", self._central.name)
-        if client := self._central.get_primary_client():
+        if client := self._central.primary_client:
             await client.fetch_all_device_data()
 
     async def refresh_entity_data(
         self, paramset_key: str | None = None, max_age_seconds: int = MAX_CACHE_AGE
     ) -> None:
         """Refresh entity data."""
         for entity in self._central.get_readable_entities():
```

### Comparing `hahomematic-2023.7.5/hahomematic/caches/persistent.py` & `hahomematic-2023.7.6/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/caches/visibility.py` & `hahomematic-2023.7.6/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/central_unit.py` & `hahomematic-2023.7.6/hahomematic/central_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         )
         self.paramset_descriptions: Final[ParamsetDescriptionCache] = ParamsetDescriptionCache(
             central=self
         )
         self.parameter_visibility: Final[ParameterVisibilityCache] = ParameterVisibilityCache(
             central=self
         )
-
+        self._primary_client: hmcl.Client | None = None
         # {interface_id, client}
         self._clients: Final[dict[str, hmcl.Client]] = {}
         # {{channel_address, parameter}, event_handle}
         self._entity_event_subscriptions: Final[dict[tuple[str, str], Any]] = {}
         # {unique_identifier, entity}
         self._entities: Final[dict[str, BaseEntity]] = {}
         # {unique_identifier, update_entity}
@@ -202,29 +202,45 @@
 
     @property
     def is_alive(self) -> bool:
         """Return if XmlRPC-Server is alive."""
         return all(client.is_callback_alive() for client in self._clients.values())
 
     @property
+    def primary_client(self) -> hmcl.Client | None:
+        """Return the primary client of the backend."""
+        if self._primary_client is not None:
+            return self._primary_client
+        if client := self._get_primary_client():
+            self._primary_client = client
+        return self._primary_client
+
+    @property
     def model(self) -> str | None:
         """Return the model of the backend. #CC."""
-        if not self._attr_model and (client := self.get_primary_client()):
+        if not self._attr_model and (client := self.primary_client):
             self._attr_model = client.model
         return self._attr_model
 
     @property
     def name(self) -> str:
         """Return the name of the backend. #CC."""
         return self._attr_name
 
     @property
+    def supports_ping_pong(self) -> bool:
+        """Return the backend supports ping pong."""
+        if primary_client := self.primary_client:
+            return primary_client.supports_ping_pong
+        return False
+
+    @property
     def system_information(self) -> SystemInformation:
         """Return the system_information of the backend."""
-        if client := self.get_primary_client():
+        if client := self.primary_client:
             return client.system_information
         return SystemInformation()
 
     @property
     def version(self) -> str | None:
         """Return the version of the backend. #CC."""
         if self._attr_version is None:
@@ -396,15 +412,15 @@
         if self.has_clients:
             _LOGGER.debug(
                 "CREATE_CLIENTS: All clients successfully created for %s",
                 self._attr_name,
             )
             return True
 
-        _LOGGER.warning("CREATE_CLIENTS failed for %s", self._attr_name)
+        _LOGGER.debug("CREATE_CLIENTS failed for %s", self._attr_name)
         return False
 
     async def _init_clients(self) -> None:
         """Init clients of control unit, and start connection checker."""
         for client in self._clients.values():
             if await client.proxy_init() == PROXY_INIT_SUCCESS:
                 _LOGGER.debug("INIT_CLIENTS: client for %s initialized", client.interface_id)
@@ -547,15 +563,15 @@
         for entity in self._entities.values():
             if (isinstance(entity, GenericEntity) and entity.is_readable) or isinstance(
                 entity, CustomEntity
             ):
                 readable_entities.append(entity)
         return readable_entities
 
-    def get_primary_client(self) -> hmcl.Client | None:
+    def _get_primary_client(self) -> hmcl.Client | None:
         """Return the client by interface_id or the first with a virtual remote."""
         client: hmcl.Client | None = None
         for client in self._clients.values():
             if isinstance(client, hmcl.ClientLocal):
                 return client
             if client.interface in IF_PRIMARY and client.available:
                 return client
@@ -850,44 +866,47 @@
 
     def has_entity(self, unique_identifier: str) -> bool:
         """Check if unique_identifier is already added."""
         return unique_identifier in self._entities
 
     def increase_ping_count(self, interface_id: str) -> None:
         """Increase the number of send ping events."""
-        with self._sema_ping_count:
-            if (ping_count := self._ping_count.get(interface_id)) is not None:
-                ping_count += 1
-                self._ping_count[interface_id] = ping_count
-                if ping_count > PING_PONG_MISMATCH_COUNT:
-                    self._fire_ping_pong_event(interface_id=interface_id)
-                _LOGGER.debug("Increase Ping count: %s, %i", interface_id, ping_count)
-            else:
-                self._ping_count[interface_id] = 1
+        if self.supports_ping_pong is True:
+            with self._sema_ping_count:
+                if (ping_count := self._ping_count.get(interface_id)) is not None:
+                    ping_count += 1
+                    self._ping_count[interface_id] = ping_count
+                    if ping_count > PING_PONG_MISMATCH_COUNT:
+                        self._fire_ping_pong_event(interface_id=interface_id)
+                    _LOGGER.debug("Increase Ping count: %s, %i", interface_id, ping_count)
+                else:
+                    self._ping_count[interface_id] = 1
 
     def _reduce_ping_count(self, interface_id: str) -> None:
         """Reduce the number of send ping events, by a received pong event."""
-        with self._sema_ping_count:
-            if (ping_count := self._ping_count.get(interface_id)) is not None:
-                ping_count -= 1
-                self._ping_count[interface_id] = ping_count
-                if ping_count < -PING_PONG_MISMATCH_COUNT:
-                    self._fire_ping_pong_event(interface_id=interface_id)
-                _LOGGER.debug("Reduce Ping count: %s, %i", interface_id, ping_count)
-            else:
-                self._ping_count[interface_id] = 0
+        if self.supports_ping_pong is True:
+            with self._sema_ping_count:
+                if (ping_count := self._ping_count.get(interface_id)) is not None:
+                    ping_count -= 1
+                    self._ping_count[interface_id] = ping_count
+                    if ping_count < -PING_PONG_MISMATCH_COUNT:
+                        self._fire_ping_pong_event(interface_id=interface_id)
+                    _LOGGER.debug("Reduce Ping count: %s, %i", interface_id, ping_count)
+                else:
+                    self._ping_count[interface_id] = 0
 
     def _fire_ping_pong_event(self, interface_id: str) -> None:
         """Fire an event about the ping pong status."""
         if self._ping_pong_fired:
             return
         message = (
             f"There is a mismatch between send ping events and received pong events for HA instance {self.config.name}. "
-            f"Looks like you are running multiple instances of HA with the same instance name configured for this integration. "
-            f"Re-add one instance! Otherwise one HA instance will not receive update events from your CCU."
+            f"Possible reason 1: You are running multiple instances of HA with the same instance name configured for this integration. "
+            f"Re-add one instance! Otherwise one HA instance will not receive update events from your CCU. "
+            f"Possible reason 2: Something is stuck on CCU, so try a restart."
         )
         event_data: dict[str, Any] = {
             ATTR_INTERFACE_ID: interface_id,
             ATTR_TYPE: HmInterfaceEventType.PINGPONG,
             ATTR_MESSAGE: message,
         }
         self.fire_ha_event_callback(
@@ -938,15 +957,15 @@
                 "async_add_executor_job: task cancelled for %s",
                 self._attr_name,
             )
             raise HaHomematicException from err
 
     async def execute_program(self, pid: str) -> bool:
         """Execute a program on CCU / Homegear."""
-        if client := self.get_primary_client():
+        if client := self.primary_client:
             return await client.execute_program(pid=pid)
         return False
 
     async def fetch_sysvar_data(self, include_internal: bool = True) -> None:
         """Fetch sysvar data for the hub. #CC."""
         await self._hub.fetch_sysvar_data(include_internal=include_internal)
 
@@ -962,15 +981,15 @@
             await self.device_data.load()
         await self.device_data.refresh_entity_data(
             paramset_key=paramset_key, max_age_seconds=max_age_seconds
         )
 
     async def get_system_variable(self, name: str) -> Any | None:
         """Get system variable from CCU / Homegear."""
-        if client := self.get_primary_client():
+        if client := self.primary_client:
             return await client.get_system_variable(name)
         return None
 
     async def set_system_variable(self, name: str, value: Any) -> None:
         """Set variable value on CCU/Homegear.  #CC."""
         if entity := self.sysvar_entities.get(name):
             await entity.send_variable(value=value)
@@ -1308,17 +1327,17 @@
 
     def __init__(self) -> None:
         """Init the CentralConnectionStatus."""
         self._json_issue: bool = False
         self._xml_proxy_issues: Final[list[str]] = []
 
     @property
-    def outgoing_issue(self) -> bool:
+    def json_issue(self) -> bool:
         """Return if there is an outgoing connection issue."""
-        return len(self._xml_proxy_issues) > 0
+        return self._json_issue
 
     def add_issue(self, issuer: ConnectionProblemIssuer) -> bool:
         """Add issue to collection."""
         if isinstance(issuer, JsonRpcAioHttpClient) and not self._json_issue:
             self._json_issue = True
             _LOGGER.debug("add_issue: add issue for JsonRpcAioHttpClient")
             return True
```

### Comparing `hahomematic-2023.7.5/hahomematic/client.py` & `hahomematic-2023.7.6/hahomematic/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,19 @@
         return self._attr_available
 
     @property
     @abstractmethod
     def model(self) -> str:
         """Return the model of the backend."""
 
+    @property
+    @abstractmethod
+    def supports_ping_pong(self) -> bool:
+        """Return the supports_ping_pong info of the backend."""
+
     async def proxy_init(self) -> int:
         """Init the proxy has to tell the CCU / Homegear where to send the events."""
         try:
             _LOGGER.debug("PROXY_INIT: init('%s', '%s')", self._config.init_url, self.interface_id)
             await self._proxy.init(self._config.init_url, self.interface_id)
             self._mark_all_devices_forced_availability(
                 forced_availability=HmForcedDeviceAvailability.NOT_SET
@@ -661,14 +666,19 @@
     """Client implementation for CCU backend."""
 
     @property
     def model(self) -> str:
         """Return the model of the backend."""
         return BACKEND_CCU
 
+    @property
+    def supports_ping_pong(self) -> bool:
+        """Return the supports_ping_pong info of the backend."""
+        return True
+
     async def fetch_device_details(self) -> None:
         """Get all names via JSON-RPS and store in data.NAMES."""
         if json_result := await self._json_rpc_client.get_device_details():
             for device in json_result:
                 self.central.device_details.add_name(
                     address=device[ATTR_ADDRESS], name=device[ATTR_NAME]
                 )
@@ -778,14 +788,19 @@
             return (
                 BACKEND_PYDEVCCU
                 if BACKEND_PYDEVCCU.lower() in self._config.version
                 else BACKEND_HOMEGEAR
             )
         return BACKEND_CCU
 
+    @property
+    def supports_ping_pong(self) -> bool:
+        """Return the supports_ping_pong info of the backend."""
+        return False
+
     async def fetch_all_device_data(self) -> None:
         """Fetch all device data from CCU."""
         return
 
     async def fetch_device_details(self) -> None:
         """Get all names from metadata (Homegear)."""
         _LOGGER.debug("FETCH_DEVICE_DETAILS: Fetching names via Metadata")
@@ -806,15 +821,16 @@
                 )
 
     async def check_connection_availability(self) -> bool:
         """Check if proxy is still initialized."""
         try:
             await self._proxy.clientServerInitialized(self.interface_id)
             self.last_updated = datetime.now()
-            self.central.increase_ping_count(interface_id=self.interface_id)
+            if self.supports_ping_pong:
+                self.central.increase_ping_count(interface_id=self.interface_id)
             return True
         except BaseHomematicException as hhe:
             _LOGGER.debug("CHECK_CONNECTION_AVAILABILITY failed: %s [%s]", hhe.name, hhe.args)
         self.last_updated = INIT_DATETIME
         return False
 
     async def execute_program(self, pid: str) -> bool:
@@ -887,14 +903,19 @@
         return True
 
     @property
     def model(self) -> str:
         """Return the model of the backend."""
         return BACKEND_LOCAL
 
+    @property
+    def supports_ping_pong(self) -> bool:
+        """Return the supports_ping_pong info of the backend."""
+        return False
+
     async def proxy_init(self) -> int:
         """Init the proxy has to tell the CCU / Homegear where to send the events."""
         return PROXY_INIT_SUCCESS
 
     async def proxy_de_init(self) -> int:
         """De-init to stop CCU from sending events for this remote."""
         return PROXY_DE_INIT_SUCCESS
@@ -1257,15 +1278,15 @@
     """Return client by interface_id."""
     for central in hmcu.CENTRAL_INSTANCES.values():
         if central.has_client(interface_id=interface_id):
             return central.get_client(interface_id=interface_id)
     return None
 
 
-@dataclass
+@dataclass(slots=True)
 class LocalRessources:
     """Dataclass with information for local client."""
 
     address_device_translation: dict[str, str]
     ignore_devices_on_create: list[str]
     package: str = "pydevccu"
     device_description_dir: str = "device_descriptions"
```

### Comparing `hahomematic-2023.7.5/hahomematic/const.py` & `hahomematic-2023.7.6/hahomematic/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,32 +47,29 @@
 ATTR_ADDRESS: Final = "address"
 ATTR_CALLBACK_HOST: Final = "callback_host"
 ATTR_CALLBACK_PORT: Final = "callback_port"
 ATTR_CHANNELS: Final = "channels"
 ATTR_CHANNEL_NO: Final = "channel_no"
 ATTR_CONFIG: Final = "config"
 ATTR_DEVICE_TYPE: Final = "device_type"
-ATTR_ERROR: Final = "error"
 ATTR_FIRMWARE: Final = "firmware"
 ATTR_HOST: Final = "host"
 ATTR_ID: Final = "id"
 ATTR_INTERFACE: Final = "interface"
 ATTR_INTERFACE_ID: Final = "interface_id"
 ATTR_IP: Final = "ip"
 ATTR_JSON_PORT: Final = "json_port"
 ATTR_MESSAGE: Final = "message"
 ATTR_MODEL: Final = "model"
 ATTR_NAME: Final = "name"
 ATTR_PARAMETER: Final = "parameter"
 ATTR_PARAMSET_KEY: Final = "paramsetKey"
 ATTR_PASSWORD: Final = "password"
 ATTR_PORT: Final = "port"
-ATTR_RESULT: Final = "result"
 ATTR_ROOM: Final = "room"
-ATTR_SESSION_ID: Final = "_session_id_"
 ATTR_TLS: Final = "tls"
 ATTR_TYPE: Final = "type"
 ATTR_USERNAME: Final = "username"
 ATTR_VALUE: Final = "value"
 ATTR_VALUE_KEY: Final = "valueKey"
 ATTR_VERIFY_TLS: Final = "verify_tls"
```

### Comparing `hahomematic-2023.7.5/hahomematic/decorators.py` & `hahomematic-2023.7.6/hahomematic/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/exceptions.py` & `hahomematic-2023.7.6/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/exporter.py` & `hahomematic-2023.7.6/hahomematic/exporter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/hmcli.py` & `hahomematic-2023.7.6/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/json_rpc_client.py` & `hahomematic-2023.7.6/hahomematic/json_rpc_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 from datetime import datetime
 import logging
 import os
 from pathlib import Path
 import re
 from typing import Any, Final
 
-from aiohttp import ClientConnectorError, ClientError, ClientSession
+from aiohttp import (
+    ClientConnectorCertificateError,
+    ClientConnectorError,
+    ClientError,
+    ClientSession,
+)
 import orjson
 
 from hahomematic import central_unit as hmcu, config
 from hahomematic.const import (
-    ATTR_ERROR,
     ATTR_NAME,
     ATTR_PASSWORD,
-    ATTR_RESULT,
-    ATTR_SESSION_ID,
     ATTR_USERNAME,
     DEFAULT_ENCODING,
     MAX_JSON_SESSION_AGE,
     PATH_JSON_RPC,
     PROGRAM_ID,
     PROGRAM_ISACTIVE,
     PROGRAM_ISINTERNAL,
@@ -42,22 +44,28 @@
     SYSVAR_NAME,
     SYSVAR_TYPE,
     SYSVAR_TYPE_NUMBER,
     SYSVAR_UNIT,
     SYSVAR_VALUE,
     SYSVAR_VALUE_LIST,
 )
-from hahomematic.exceptions import BaseHomematicException, ClientException
+from hahomematic.exceptions import ClientException
 from hahomematic.support import (
     ProgramData,
     SystemVariableData,
     get_tls_context,
     parse_sys_var,
 )
 
+P_ERROR = "error"
+P_RESULT = "result"
+SESSION_ID: Final = "_session_id_"
+
+ALLOWED_METHOD_ON_FAILURE = ("Session.login",)
+
 _LOGGER = logging.getLogger(__name__)
 
 
 class JsonRpcAioHttpClient:
     """Connection to CCU JSON-RPC Server."""
 
     def __init__(
@@ -72,15 +80,15 @@
     ) -> None:
         """Session setup."""
         self._client_session: Final = client_session
         self._connection_state: Final = connection_state
         self._username: Final = username
         self._password: Final = password
         self._tls: Final = tls
-        self._tls_context: Final = get_tls_context(verify_tls)
+        self._tls_context: Final = get_tls_context(verify_tls) if tls else None
         self._url: Final = f"{device_url}{PATH_JSON_RPC}"
         self._script_cache: Final[dict[str, str]] = {}
         self._last_session_id_refresh: datetime | None = None
         self._session_id: str | None = None
 
     @property
     def is_activated(self) -> bool:
@@ -95,38 +103,29 @@
             return self._session_id is not None
         if self._session_id:
             self._session_id = await self._do_renew_login(self._session_id)
         return self._session_id is not None
 
     async def _do_renew_login(self, session_id: str) -> str | None:
         """Renew JSON-RPC session or perform login."""
-        try:
-            if self._updated_within_seconds():
-                return session_id
-            method = "Session.renew"
-            response = await self._do_post(
-                session_id=session_id,
-                method=method,
-                extra_params={ATTR_SESSION_ID: session_id},
-            )
-            if (
-                response[ATTR_ERROR] is None
-                and response[ATTR_RESULT]
-                and response[ATTR_RESULT] is True
-            ):
-                self._last_session_id_refresh = datetime.now()
-                _LOGGER.debug("DO_RENEW_LOGIN: Method: %s [%s]", method, session_id)
-                return session_id
-            return await self._do_login()
-        except ClientError as cer:
-            _LOGGER.error(
-                "DO_RENEW_LOGIN failed: ClientError [%s] while renewing JSON-RPC session",
-                cer.args,
-            )
-            return None
+        if self._updated_within_seconds():
+            return session_id
+        method = "Session.renew"
+        response = await self._do_post(
+            session_id=session_id,
+            method=method,
+            extra_params={SESSION_ID: session_id},
+        )
+
+        if response[P_RESULT] and response[P_RESULT] is True:
+            self._last_session_id_refresh = datetime.now()
+            _LOGGER.debug("DO_RENEW_LOGIN: Method: %s [%s]", method, session_id)
+            return session_id
+
+        return await self._do_login()
 
     def _updated_within_seconds(self, max_age_seconds: int = MAX_JSON_SESSION_AGE) -> bool:
         """Check if session id has been updated within 90 seconds."""
         if self._last_session_id_refresh is None:
             return False
         delta = datetime.now() - self._last_session_id_refresh
         if delta.seconds < max_age_seconds:
@@ -136,42 +135,33 @@
     async def _do_login(self) -> str | None:
         """Login to CCU and return session."""
         if not self._has_credentials:
             _LOGGER.warning("DO_LOGIN failed: No credentials set")
             return None
 
         session_id: str | None = None
-        try:
-            params = {
-                ATTR_USERNAME: self._username,
-                ATTR_PASSWORD: self._password,
-            }
-            method = "Session.login"
-            response = await self._do_post(
-                session_id=False,
-                method=method,
-                extra_params=params,
-                use_default_params=False,
-            )
-            if response[ATTR_ERROR] is None and response[ATTR_RESULT]:
-                session_id = response[ATTR_RESULT]
 
-            _LOGGER.debug("DO_LOGIN: Method: %s [%s]", method, session_id)
+        params = {
+            ATTR_USERNAME: self._username,
+            ATTR_PASSWORD: self._password,
+        }
+        method = "Session.login"
+        response = await self._do_post(
+            session_id=False,
+            method=method,
+            extra_params=params,
+            use_default_params=False,
+        )
 
-            if not session_id:
-                _LOGGER.debug("DO_LOGIN failed: Unable to open session: %s", response[ATTR_ERROR])
-                return None
-            return session_id
-        except BaseHomematicException as hhe:
-            _LOGGER.error(
-                "DO_LOGIN failed: %s [%s] while logging in via JSON-RPC",
-                hhe.name,
-                hhe.args,
-            )
-            return None
+        _LOGGER.debug("DO_LOGIN: Method: %s [%s]", method, session_id)
+
+        if result := response[P_RESULT]:
+            session_id = result
+
+        return session_id
 
     async def _post(
         self,
         method: str,
         extra_params: dict[str, str] | None = None,
         use_default_params: bool = True,
         keep_session: bool = True,
@@ -180,29 +170,31 @@
         if keep_session:
             await self._login_or_renew()
             session_id = self._session_id
         else:
             session_id = await self._do_login()
 
         if not session_id:
-            _LOGGER.warning("POST failed: Error while logging in via JSON-RPC")
-            return {"error": "Unable to open session", "result": {}}
+            raise ClientException("Error while logging in")
 
-        _LOGGER.debug("POST: Method: %s, [%s]", method, extra_params)
         response = await self._do_post(
             session_id=session_id,
             method=method,
             extra_params=extra_params,
             use_default_params=use_default_params,
         )
 
+        if extra_params:
+            _LOGGER.debug("POST method: %s, [%s]", method, extra_params)
+        else:
+            _LOGGER.debug("POST method: %s", method)
+
         if not keep_session:
             await self._do_logout(session_id=session_id)
-        if (error := response["error"]) is not None:
-            raise ClientException(f"POST: error: {error}")
+
         return response
 
     async def _post_script(
         self,
         script_name: str,
         extra_params: dict[str, str] | None = None,
         keep_session: bool = True,
@@ -211,43 +203,37 @@
         if keep_session:
             await self._login_or_renew()
             session_id = self._session_id
         else:
             session_id = await self._do_login()
 
         if not session_id:
-            _LOGGER.debug("POST_SCRIPT failed: Error while logging in via JSON-RPC.")
-            return {"error": "Unable to open session", "result": {}}
+            raise ClientException("Error while logging in")
 
         if (script := self._get_script(script_name=script_name)) is None:
-            _LOGGER.warning("POST_SCRIPT failed: Script file for %s does not exist", script_name)
-            return {
-                "error": f"Script file for {script_name} does not exist",
-                "result": {},
-            }
+            raise ClientException(f"Script file for {script_name} does not exist")
 
         if extra_params:
             for variable, value in extra_params.items():
                 script = script.replace(f"##{variable}##", value)
 
         method = "ReGa.runScript"
         response = await self._do_post(
             session_id=session_id,
             method=method,
             extra_params={"script": script},
         )
-        if not response[ATTR_ERROR]:
-            response[ATTR_RESULT] = orjson.loads(response[ATTR_RESULT])
+
+        if not response[P_ERROR]:
+            response[P_RESULT] = orjson.loads(response[P_RESULT])
         _LOGGER.debug("POST_SCRIPT: Method: %s [%s]", method, script_name)
 
         if not keep_session:
             await self._do_logout(session_id=session_id)
 
-        if (error := response["error"]) is not None:
-            raise ClientException(f"post_script: error: {error}")
         return response
 
     def _get_script(self, script_name: str) -> str | None:
         """Return a script from the script cache. Load if required."""
         if script_name in self._script_cache:
             return self._script_cache[script_name]
 
@@ -261,25 +247,18 @@
         self,
         session_id: bool | str,
         method: str,
         extra_params: dict[str, str] | None = None,
         use_default_params: bool = True,
     ) -> dict[str, Any] | Any:
         """Reusable JSON-RPC POST function."""
-        if self._connection_state.outgoing_issue:
-            # Report 'Service Unavailable' if there is an outgoing issue
-            return {"error": "503", "result": {}}
         if not self._client_session:
-            no_session = "DO_POST failed: ClientSession not initialized."
-            _LOGGER.warning(no_session)
-            return {"error": no_session, "result": {}}
+            raise ClientException("ClientSession not initialized")
         if not self._has_credentials:
-            no_credentials = "DO_POST failed: No credentials set."
-            _LOGGER.warning(no_credentials)
-            return {"error": str(no_credentials), "result": {}}
+            raise ClientException("No credentials set")
 
         params = _get_params(session_id, extra_params, use_default_params)
 
         try:
             payload = orjson.dumps({"method": method, "params": params, "jsonrpc": "1.1", "id": 0})
 
             headers = {
@@ -296,104 +275,101 @@
                     ssl=self._tls_context,
                 )
             else:
                 response = await self._client_session.post(
                     self._url, data=payload, headers=headers, timeout=config.TIMEOUT
                 )
             if response.status == 200:
+                self._connection_state.remove_issue(issuer=self)
                 try:
-                    self._connection_state.remove_issue(issuer=self)
                     return await response.json(encoding="utf-8")
                 except ValueError as ver:
-                    _LOGGER.error(
-                        "DO_POST failed: ValueError [%s] Unable to parse JSON. "
-                        "Trying workaround",
+                    _LOGGER.debug(
+                        "DO_POST: ValueError [%s] Unable to parse JSON. Trying workaround",
                         ver.args,
                     )
                     # Workaround for bug in CCU
                     return orjson.loads((await response.json(encoding="utf-8")).replace("\\", ""))
             else:
-                _LOGGER.warning("DO_POST failed: Status: %i", response.status)
-                return {"error": response.status, "result": {}}
+                json_response = await response.json(encoding="utf-8")
+                message = f"Status: {response.status}"
+                if error := json_response[P_ERROR]:
+                    message = f"{message}: {error}"
+                raise ClientException(message)
+        except ClientConnectorCertificateError as cccerr:
+            message = f"ClientConnectorCertificateError[{cccerr}]"
+            if self._tls is False and cccerr.ssl is True:
+                message = (
+                    f"{message}. Possible reason: 'Automatic forwarding to HTTPS' is enabled in backend, "
+                    f"but this integration is not configured to use TLS"
+                )
+            raise ClientException(message) from cccerr
         except ClientConnectorError as err:
-            self._connection_state.add_issue(issuer=self)
-            _LOGGER.error("DO_POST failed: ClientConnectorError: %s", err)
-            return {"error": str(err), "result": {}}
+            raise ClientException from err
         except ClientError as cce:
-            _LOGGER.error("DO_POST failed: ClientError: %s", cce)
-            return {"error": str(cce), "result": {}}
-        except TypeError as ter:
-            _LOGGER.error("DO_POST failed: TypeError: %s", ter)
-            return {"error": str(ter), "result": {}}
-        except OSError as oer:
-            _LOGGER.error("DO_POST failed: OSError: %s", oer)
-            return {"error": str(oer), "result": {}}
-        except Exception as ex:
+            raise ClientException from cce
+        except (OSError, TypeError, Exception) as ex:
             raise ClientException from ex
 
     async def logout(self) -> None:
         """Logout of CCU."""
-        await self._do_logout(self._session_id)
+        try:
+            await self._do_logout(self._session_id)
+        except ClientException as clex:
+            self._handle_client_exception(method="LOGOUT", clex=clex)
+            return
 
     async def _do_logout(self, session_id: str | None) -> None:
         """Logout of CCU."""
         if not session_id:
             _LOGGER.debug("DO_LOGOUT: Not logged in. Not logging out.")
             return
-        try:
-            method = "Session.logout"
-            params = {"_session_id_": session_id}
-            response = await self._do_post(
-                session_id=session_id,
-                method=method,
-                extra_params=params,
-            )
-            _LOGGER.debug("DO_LOGOUT: Method: %s [%s]", method, session_id)
-            if response[ATTR_ERROR]:
-                _LOGGER.warning("DO_LOGOUT failed: Logout error: %s", response[ATTR_RESULT])
-        except ClientError as cer:
-            _LOGGER.error(
-                "LOGOUT failed: ClientError [%s] while logging in via JSON-RPC",
-                cer.args,
-            )
-        return
+
+        method = "Session.logout"
+        params = {"_session_id_": session_id}
+        await self._do_post(
+            session_id=session_id,
+            method=method,
+            extra_params=params,
+        )
+        _LOGGER.debug("DO_LOGOUT: Method: %s [%s]", method, session_id)
 
     @property
     def _has_credentials(self) -> bool:
         """Return if credentials are available."""
         return self._username is not None and self._username != "" and self._password is not None
 
     async def execute_program(self, pid: str) -> bool:
         """Execute a program on CCU / Homegear."""
-        _LOGGER.debug("EXECUTE_PROGRAM: Executing a program via JSON-RPC")
+        params = {
+            PROGRAM_ID: pid,
+        }
         try:
-            params = {
-                PROGRAM_ID: pid,
-            }
             response = await self._post("Program.execute", params)
+            _LOGGER.debug("EXECUTE_PROGRAM: Executing a program")
 
-            if json_result := response[ATTR_RESULT]:
-                res = json_result
+            if json_result := response[P_RESULT]:
                 _LOGGER.debug(
                     "EXECUTE_PROGRAM: Result while executing program: %s",
-                    str(res),
+                    str(json_result),
                 )
-        except BaseHomematicException as hhe:
-            _LOGGER.warning("EXECUTE_PROGRAM failed: %s [%s]", hhe.name, hhe.args)
+        except ClientException as clex:
+            self._handle_client_exception(method="EXECUTE_PROGRAM", clex=clex)
             return False
+
         return True
 
     async def set_system_variable(self, name: str, value: Any) -> bool:
         """Set a system variable on CCU / Homegear."""
-        _LOGGER.debug("SET_SYSTEM_VARIABLE: Setting System variable via JSON-RPC")
+
+        params = {
+            SYSVAR_NAME: name,
+            SYSVAR_VALUE: value,
+        }
         try:
-            params = {
-                SYSVAR_NAME: name,
-                SYSVAR_VALUE: value,
-            }
             if isinstance(value, bool):
                 params[SYSVAR_VALUE] = int(value)
                 response = await self._post("SysVar.setBool", params)
             elif isinstance(value, str):
                 if re.findall("<.*?>|&([a-z0-9]+|#[0-9]{1,6}|#x[0-9a-f]{1,6});", value):
                     _LOGGER.warning(
                         "SET_SYSTEM_VARIABLE failed: "
@@ -403,72 +379,79 @@
                     return False
                 response = await self._post_script(
                     script_name=REGA_SCRIPT_SET_SYSTEM_VARIABLE, extra_params=params
                 )
             else:
                 response = await self._post("SysVar.setFloat", params)
 
-            if json_result := response[ATTR_RESULT]:
-                res = json_result
+            _LOGGER.debug("SET_SYSTEM_VARIABLE: Setting System variable")
+            if json_result := response[P_RESULT]:
                 _LOGGER.debug(
                     "SET_SYSTEM_VARIABLE: Result while setting variable: %s",
-                    str(res),
+                    str(json_result),
                 )
-        except BaseHomematicException as hhe:
-            _LOGGER.warning("SET_SYSTEM_VARIABLE failed: %s [%s]", hhe.name, hhe.args)
+        except ClientException as clex:
+            self._handle_client_exception(method="SET_SYSTEM_VARIABLE failed", clex=clex)
             return False
+
         return True
 
     async def delete_system_variable(self, name: str) -> bool:
         """Delete a system variable from CCU / Homegear."""
-        _LOGGER.debug("DELETE_SYSTEM_VARIABLE: Getting System variable via JSON-RPC")
+        params = {SYSVAR_NAME: name}
         try:
-            params = {SYSVAR_NAME: name}
             response = await self._post(
                 "SysVar.deleteSysVarByName",
                 params,
             )
-            if json_result := response[ATTR_RESULT]:
+
+            _LOGGER.debug("DELETE_SYSTEM_VARIABLE: Getting System variable")
+            if json_result := response[P_RESULT]:
                 deleted = json_result
                 _LOGGER.debug("DELETE_SYSTEM_VARIABLE: Deleted: %s", str(deleted))
-        except BaseHomematicException as hhe:
-            _LOGGER.warning("DELETE_SYSTEM_VARIABLE failed: %s [%s]", hhe.name, hhe.args)
+        except ClientException as clex:
+            self._handle_client_exception(method="DELETE_SYSTEM_VARIABLE", clex=clex)
             return False
+
         return True
 
     async def get_system_variable(self, name: str) -> Any:
         """Get single system variable from CCU / Homegear."""
         var = None
-        _LOGGER.debug("GET_SYSTEM_VARIABLE: Getting System variable via JSON-RPC")
+
         try:
             params = {SYSVAR_NAME: name}
             response = await self._post(
                 "SysVar.getValueByName",
                 params,
             )
-            if json_result := response[ATTR_RESULT]:
+
+            _LOGGER.debug("GET_SYSTEM_VARIABLE: Getting System variable")
+            if json_result := response[P_RESULT]:
                 # This does not yet support strings
                 try:
                     var = float(json_result)
                 except Exception:
                     var = json_result == "true"
-        except BaseHomematicException as hhe:
-            _LOGGER.warning("GET_SYSTEM_VARIABLE failed: %s [%s]", hhe.name, hhe.args)
+        except ClientException as clex:
+            self._handle_client_exception(method="DELETE_SYSTEM_VARIABLE", clex=clex)
+            return None
 
         return var
 
     async def get_all_system_variables(self, include_internal: bool) -> list[SystemVariableData]:
         """Get all system variables from CCU / Homegear."""
         variables: list[SystemVariableData] = []
-        _LOGGER.debug("GET_ALL_SYSTEM_VARIABLES: Getting all system variables via JSON-RPC")
         try:
             response = await self._post(
                 "SysVar.getAll",
             )
-            if json_result := response[ATTR_RESULT]:
+
+            _LOGGER.debug("GET_ALL_SYSTEM_VARIABLES: Getting all system variables")
+            if json_result := response[P_RESULT]:
                 ext_markers = await self._get_system_variables_ext_markers()
                 for var in json_result:
                     is_internal = var[SYSVAR_ISINTERNAL]
                     if include_internal is False and is_internal is True:
                         continue
                     var_id = var[SYSVAR_ID]
                     name = var[SYSVAR_NAME]
@@ -508,134 +491,147 @@
                     except ValueError as verr:
                         _LOGGER.warning(
                             "GET_ALL_SYSTEM_VARIABLES failed: "
                             "ValueError [%s] Failed to parse SysVar %s ",
                             verr.args,
                             name,
                         )
-
-        except BaseHomematicException as hhe:
-            _LOGGER.warning("GET_ALL_SYSTEM_VARIABLES failed: %s [%s]", hhe.name, hhe.args)
+        except ClientException as clex:
+            self._handle_client_exception(method="GET_ALL_SYSTEM_VARIABLES", clex=clex)
+            return []
 
         return variables
 
     async def _get_system_variables_ext_markers(self) -> dict[str, Any]:
         """Get all system variables from CCU / Homegear."""
         ext_markers: dict[str, Any] = {}
-        _LOGGER.debug(
-            "GET_SYSTEM_VARIABLES_EXT_MARKERS: Getting system variables ext markersvia JSON-RPC"
-        )
-        try:
-            response = await self._post_script(script_name=REGA_SCRIPT_SYSTEM_VARIABLES_EXT_MARKER)
-            if json_result := response[ATTR_RESULT]:
-                for data in json_result:
-                    ext_markers[data[SYSVAR_ID]] = data[SYSVAR_HASEXTMARKER]
 
-        except BaseHomematicException as hhe:
-            _LOGGER.warning("GET_SYSTEM_VARIABLES_EXT_MARKERS failed: %s [%s]", hhe.name, hhe.args)
+        response = await self._post_script(script_name=REGA_SCRIPT_SYSTEM_VARIABLES_EXT_MARKER)
+
+        _LOGGER.debug("GET_SYSTEM_VARIABLES_EXT_MARKERS: Getting system variables ext markers")
+        if json_result := response[P_RESULT]:
+            for data in json_result:
+                ext_markers[data[SYSVAR_ID]] = data[SYSVAR_HASEXTMARKER]
 
         return ext_markers
 
     async def get_all_channel_ids_room(self) -> dict[str, set[str]]:
         """Get all channel_ids per room from CCU / Homegear."""
         channel_ids_room: dict[str, set[str]] = {}
-        _LOGGER.debug("GET_ALL_CHANNEL_IDS_PER_ROOM: Getting all rooms via JSON-RPC")
+
         try:
             response = await self._post(
                 "Room.getAll",
             )
-            if json_result := response[ATTR_RESULT]:
+
+            _LOGGER.debug("GET_ALL_CHANNEL_IDS_PER_ROOM: Getting all rooms")
+            if json_result := response[P_RESULT]:
                 for room in json_result:
                     if room["id"] not in channel_ids_room:
                         channel_ids_room[room["id"]] = set()
                     channel_ids_room[room["id"]].add(room["name"])
                     for channel_id in room["channelIds"]:
                         if channel_id not in channel_ids_room:
                             channel_ids_room[channel_id] = set()
                         channel_ids_room[channel_id].add(room["name"])
-        except BaseHomematicException as hhe:
-            _LOGGER.warning("GET_ALL_CHANNEL_IDS_PER_ROOM failed: %s [%s]", hhe.name, hhe.args)
+        except ClientException as clex:
+            self._handle_client_exception(method="GET_ALL_CHANNEL_IDS_PER_ROOM", clex=clex)
+            return {}
 
         return channel_ids_room
 
     async def get_all_channel_ids_function(self) -> dict[str, set[str]]:
         """Get all channel_ids per function from CCU / Homegear."""
         channel_ids_function: dict[str, set[str]] = {}
-        _LOGGER.debug("GET_ALL_CHANNEL_IDS_PER_FUNCTION: Getting all functions via JSON-RPC")
+
         try:
             response = await self._post(
                 "Subsection.getAll",
             )
-            if json_result := response[ATTR_RESULT]:
+
+            _LOGGER.debug("GET_ALL_CHANNEL_IDS_PER_FUNCTION: Getting all functions")
+            if json_result := response[P_RESULT]:
                 for function in json_result:
                     if function["id"] not in channel_ids_function:
                         channel_ids_function[function["id"]] = set()
                     channel_ids_function[function["id"]].add(function["name"])
                     for channel_id in function["channelIds"]:
                         if channel_id not in channel_ids_function:
                             channel_ids_function[channel_id] = set()
                         channel_ids_function[channel_id].add(function["name"])
-        except BaseHomematicException as hhe:
-            _LOGGER.warning("GET_ALL_CHANNEL_IDS_PER_FUNCTION failed: %s [%s]", hhe.name, hhe.args)
+        except ClientException as clex:
+            self._handle_client_exception(method="GET_ALL_CHANNEL_IDS_PER_FUNCTION", clex=clex)
+            return {}
 
         return channel_ids_function
 
     async def get_available_interfaces(self) -> list[str]:
         """Get all available interfaces from CCU / Homegear."""
         interfaces: list[str] = []
-        _LOGGER.debug("GET_AVAILABLE_INTERFACES: Getting all available interfaces via JSON-RPC")
+
         try:
             response = await self._post(
                 "Interface.listInterfaces",
             )
-            if json_result := response[ATTR_RESULT]:
+
+            _LOGGER.debug("GET_AVAILABLE_INTERFACES: Getting all available interfaces")
+            if json_result := response[P_RESULT]:
                 for interface in json_result:
                     interfaces.append(interface[ATTR_NAME])
-        except BaseHomematicException as hhe:
-            _LOGGER.warning("GET_AVAILABLE_INTERFACES failed: %s [%s]", hhe.name, hhe.args)
+        except ClientException as clex:
+            self._handle_client_exception(method="GET_AVAILABLE_INTERFACES", clex=clex)
+            return []
 
         return interfaces
 
     async def get_device_details(self) -> list[dict[str, Any]]:
         """Get the device details of the backend."""
-        device_details = []
-        _LOGGER.debug("GET_DEVICE_DETAILS: Getting the device details via JSON-RPC")
+        device_details: list[dict[str, Any]] = []
+
         try:
             response = await self._post(
                 method="Device.listAllDetail",
             )
-            if json_result := response[ATTR_RESULT]:
+
+            _LOGGER.debug("GET_DEVICE_DETAILS: Getting the device details")
+            if json_result := response[P_RESULT]:
                 device_details = json_result
-        except BaseHomematicException as hhe:
-            _LOGGER.warning("GET_DEVICE_DETAILS failed: %s [%s]", hhe.name, hhe.args)
+        except ClientException as clex:
+            self._handle_client_exception(method="GET_DEVICE_DETAILS", clex=clex)
+            return []
 
         return device_details
 
     async def get_all_device_data(self) -> dict[str, dict[str, dict[str, Any]]]:
         """Get the all device data of the backend."""
         all_device_data: dict[str, dict[str, dict[str, Any]]] = {}
-        _LOGGER.debug("GET_ALL_DEVICE_DATA: Getting all device data via JSON-RPC")
+
         try:
             response = await self._post_script(script_name=REGA_SCRIPT_FETCH_ALL_DEVICE_DATA)
-            if json_result := response[ATTR_RESULT]:
+
+            _LOGGER.debug("GET_ALL_DEVICE_DATA: Getting all device data")
+            if json_result := response[P_RESULT]:
                 all_device_data = _convert_to_values_cache(json_result)
-        except BaseHomematicException as hhe:
-            _LOGGER.warning("GET_ALL_DEVICE_DATA failed: %s [%s]", hhe.name, hhe.args)
+        except ClientException as clex:
+            self._handle_client_exception(method="GET_ALL_DEVICE_DATA", clex=clex)
+            return {}
 
         return all_device_data
 
     async def get_all_programs(self, include_internal: bool) -> list[ProgramData]:
         """Get the all programs of the backend."""
         all_programs: list[ProgramData] = []
-        _LOGGER.debug("GET_ALL_PROGRAMS: Getting all programs via JSON-RPC")
+
         try:
             response = await self._post(
                 method="Program.getAll",
             )
-            if json_result := response[ATTR_RESULT]:
+
+            _LOGGER.debug("GET_ALL_PROGRAMS: Getting all programs")
+            if json_result := response[P_RESULT]:
                 for prog in json_result:
                     is_internal = prog[PROGRAM_ISINTERNAL]
                     if include_internal is False and is_internal is True:
                         continue
                     pid = prog[PROGRAM_ID]
                     name = prog[PROGRAM_NAME]
                     is_active = prog[PROGRAM_ISACTIVE]
@@ -646,63 +642,77 @@
                             pid=pid,
                             name=name,
                             is_active=is_active,
                             is_internal=is_internal,
                             last_execute_time=last_execute_time,
                         )
                     )
-
-        except BaseHomematicException as hhe:
-            _LOGGER.warning("GET_ALL_PROGRAMS failed: %s [%s]", hhe.name, hhe.args)
+        except ClientException as clex:
+            self._handle_client_exception(method="GET_ALL_PROGRAMS", clex=clex)
+            return []
 
         return all_programs
 
     async def get_auth_enabled(self) -> bool | None:
         """Get the auth_enabled flag of the backend."""
         auth_enabled: bool | None = None
-        _LOGGER.debug("GET_AUTH_ENABLED: Getting the flag auth_enabled via JSON-RPC")
+
         try:
             response = await self._post(method="CCU.getAuthEnabled")
-            if (json_result := response[ATTR_RESULT]) is not None:
-                auth_enabled = bool(json_result)
-        except BaseHomematicException as hhe:
-            _LOGGER.warning("GET_AUTH_ENABLED failed: %s [%s]", hhe.name, hhe.args)
 
+            _LOGGER.debug("GET_AUTH_ENABLED: Getting the flag auth_enabled")
+            if (json_result := response[P_RESULT]) is not None:
+                auth_enabled = bool(json_result)
+        except ClientException as clex:
+            self._handle_client_exception(method="GET_AUTH_ENABLED", clex=clex)
+            return None
         return auth_enabled
 
     async def get_https_redirect_enabled(self) -> bool | None:
         """Get the auth_enabled flag of the backend."""
         https_redirect_enabled: bool | None = None
-        _LOGGER.debug(
-            "GET_HTTPS_REDIRECT_ENABLED: Getting the flag https_redirect_enabled via JSON-RPC"
-        )
+
         try:
             response = await self._post(method="CCU.getHttpsRedirectEnabled")
-            if (json_result := response[ATTR_RESULT]) is not None:
+
+            _LOGGER.debug("GET_HTTPS_REDIRECT_ENABLED: Getting the flag https_redirect_enabled")
+            if (json_result := response[P_RESULT]) is not None:
                 https_redirect_enabled = bool(json_result)
-        except BaseHomematicException as hhe:
-            _LOGGER.warning("GET_HTTPS_REDIRECT_ENABLED failed: %s [%s]", hhe.name, hhe.args)
+        except ClientException as clex:
+            self._handle_client_exception(method="GET_HTTPS_REDIRECT_ENABLED", clex=clex)
+            return None
 
         return https_redirect_enabled
 
     async def get_serial(self) -> str:
         """Get the serial of the backend."""
         serial = "unknown"
-        _LOGGER.debug("GET_SERIAL: Getting the backend serial via JSON-RPC")
+
         try:
             response = await self._post_script(script_name=REGA_SCRIPT_GET_SERIAL)
-            if json_result := response[ATTR_RESULT]:
+
+            _LOGGER.debug("GET_SERIAL: Getting the backend serial")
+            if json_result := response[P_RESULT]:
                 serial = json_result["serial"]
                 if len(serial) > 10:
                     serial = serial[-10:]
-        except BaseHomematicException as hhe:
-            _LOGGER.warning("GET_SERIAL failed: %s [%s]", hhe.name, hhe.args)
+        except ClientException as clex:
+            self._handle_client_exception(method="GET_SERIAL", clex=clex)
+            return serial
 
         return serial
 
+    def _handle_client_exception(self, method: str, clex: ClientException) -> None:
+        """Handle ClientException."""
+        if self._connection_state.json_issue:
+            _LOGGER.debug("%s failed: %s [%s]", method, clex.name, clex.args)
+        else:
+            self._connection_state.add_issue(issuer=self)
+            _LOGGER.error("%s failed: %s [%s]", method, clex.name, clex.args)
+
 
 def _get_params(
     session_id: bool | str,
     extra_params: dict[str, Any] | None,
     use_default_params: bool,
 ) -> dict[str, Any]:
     """Add additional params to default prams."""
```

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/__init__.py` & `hahomematic-2023.7.6/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/custom/__init__.py` & `hahomematic-2023.7.6/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/custom/climate.py` & `hahomematic-2023.7.6/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/custom/const.py` & `hahomematic-2023.7.6/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/custom/cover.py` & `hahomematic-2023.7.6/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/custom/definition.py` & `hahomematic-2023.7.6/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/custom/entity.py` & `hahomematic-2023.7.6/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/custom/light.py` & `hahomematic-2023.7.6/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/custom/lock.py` & `hahomematic-2023.7.6/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/custom/siren.py` & `hahomematic-2023.7.6/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/custom/support.py` & `hahomematic-2023.7.6/hahomematic/platforms/custom/support.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Support classes used by hahomematic custom entities."""
 from __future__ import annotations
 
 from collections.abc import Callable
 from dataclasses import dataclass
 
 
-@dataclass
+@dataclass(slots=True)
 class CustomConfig:
     """Data for custom entity creation."""
 
     func: Callable
     channels: tuple[int, ...]
     extended: ExtendedConfig | None = None
 
 
-@dataclass
+@dataclass(slots=True)
 class ExtendedConfig:
     """Extended data for custom entity creation."""
 
     fixed_channels: dict[int, dict[str, str]] | None = None
     additional_entities: dict[int | tuple[int, ...], tuple[str, ...]] | None = None
 
     @property
```

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/custom/switch.py` & `hahomematic-2023.7.6/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/device.py` & `hahomematic-2023.7.6/hahomematic/platforms/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -654,15 +654,15 @@
         ) != CacheEntry.empty() and updated_within_seconds(
             last_update=cache_entry.last_update, max_age_seconds=max_age_seconds
         ):
             return cache_entry.value
         return NO_CACHE_ENTRY
 
 
-@dataclass
+@dataclass(slots=True)
 class CacheEntry:
     """An entry for the value cache."""
 
     value: Any
     last_update: datetime
 
     @staticmethod
```

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/entity.py` & `hahomematic-2023.7.6/hahomematic/platforms/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/event.py` & `hahomematic-2023.7.6/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/generic/__init__.py` & `hahomematic-2023.7.6/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/generic/action.py` & `hahomematic-2023.7.6/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2023.7.6/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/generic/button.py` & `hahomematic-2023.7.6/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/generic/entity.py` & `hahomematic-2023.7.6/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/generic/number.py` & `hahomematic-2023.7.6/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/generic/select.py` & `hahomematic-2023.7.6/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/generic/sensor.py` & `hahomematic-2023.7.6/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/generic/switch.py` & `hahomematic-2023.7.6/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/hub/__init__.py` & `hahomematic-2023.7.6/hahomematic/platforms/hub/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         async with self._sema_fetch_programs:
             if self._central.available:
                 await self._update_program_entities(include_internal=include_internal)
 
     async def _update_program_entities(self, include_internal: bool) -> None:
         """Retrieve all program data and update program values."""
         programs: list[ProgramData] = []
-        if client := self._central.get_primary_client():
+        if client := self._central.primary_client:
             programs = await client.get_all_programs(include_internal=include_internal)
         if not programs:
             _LOGGER.debug(
                 "UPDATE_PROGRAM_ENTITIES: No programs received for %s",
                 self._central.name,
             )
             return
@@ -88,15 +88,15 @@
             self._central.fire_system_event_callback(
                 name=HH_EVENT_HUB_REFRESHED, new_hub_entities=new_programs
             )
 
     async def _update_sysvar_entities(self, include_internal: bool = True) -> None:
         """Retrieve all variable data and update hmvariable values."""
         variables: list[SystemVariableData] = []
-        if client := self._central.get_primary_client():
+        if client := self._central.primary_client:
             variables = await client.get_all_system_variables(include_internal=include_internal)
         if not variables:
             _LOGGER.debug(
                 "UPDATE_SYSVAR_ENTITIES: No sysvars received for %s",
                 self._central.name,
             )
             return
```

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2023.7.6/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/hub/button.py` & `hahomematic-2023.7.6/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/hub/entity.py` & `hahomematic-2023.7.6/hahomematic/platforms/hub/entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,12 +132,12 @@
 
         if self._attr_value != value:
             self._attr_value = value
             self.update_entity()
 
     async def send_variable(self, value: Any) -> None:
         """Set variable value on CCU/Homegear."""
-        if client := self.central.get_primary_client():
+        if client := self.central.primary_client:
             await client.set_system_variable(
                 name=self.ccu_var_name, value=parse_sys_var(self.data_type, value)
             )
         self.update_value(value=value)
```

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/hub/number.py` & `hahomematic-2023.7.6/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/hub/select.py` & `hahomematic-2023.7.6/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/hub/sensor.py` & `hahomematic-2023.7.6/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/hub/text.py` & `hahomematic-2023.7.6/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/support.py` & `hahomematic-2023.7.6/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/platforms/update.py` & `hahomematic-2023.7.6/hahomematic/platforms/update.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2023.7.6/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2023.7.6/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2023.7.6/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/support.py` & `hahomematic-2023.7.6/hahomematic/support.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,45 +231,45 @@
     """Search for a matching key in a collection."""
     for element in search_elements:
         if search_key.startswith(element):
             return element
     return None
 
 
-@dataclass
+@dataclass(slots=True)
 class HubData:
     """Dataclass for hub entities."""
 
     name: str
 
 
-@dataclass
+@dataclass(slots=True)
 class ProgramData(HubData):
     """Dataclass for programs."""
 
     pid: str
     is_active: bool
     is_internal: bool
     last_execute_time: str
 
 
-@dataclass
+@dataclass(slots=True)
 class SystemVariableData(HubData):
     """Dataclass for system variables."""
 
+    value: bool | float | int | str | None
     data_type: str | None = None
     unit: str | None = None
-    value: bool | float | int | str | None = None
     value_list: list[str] | None = None
     max_value: float | int | None = None
     min_value: float | int | None = None
     extended_sysvar: bool = False
 
 
-@dataclass
+@dataclass(slots=True)
 class SystemInformation:
     """System information of the backend."""
 
     available_interfaces: list[str] = field(default_factory=list)
     auth_enabled: bool | None = None
     https_redirect_enabled: bool | None = None
     serial: str | None = None
@@ -284,15 +284,15 @@
         if os.path.exists(os.path.join(cache_dir, file_name)):
             os.unlink(os.path.join(cache_dir, file_name))
 
     for file_to_delete in files_to_delete:
         _delete_file(file_name=f"{instance_name}_{file_to_delete}")
 
 
-@dataclass
+@dataclass(slots=True)
 class Channel:
     """dataclass for a device channel."""
 
     type: str
     address: str
 
     @property
```

### Comparing `hahomematic-2023.7.5/hahomematic/xml_rpc_proxy.py` & `hahomematic-2023.7.6/hahomematic/xml_rpc_proxy.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic/xml_rpc_server.py` & `hahomematic-2023.7.6/hahomematic/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/hahomematic.egg-info/PKG-INFO` & `hahomematic-2023.7.6/hahomematic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.7.5
+Version: 2023.7.6
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.7.5/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2023.7.6/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.5/pyproject.toml` & `hahomematic-2023.7.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2023.7.5"
+version     = "2023.7.6"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

