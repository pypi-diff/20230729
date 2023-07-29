# Comparing `tmp/messageflux-0.3.1.tar.gz` & `tmp/messageflux-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messageflux-0.3.1.tar", last modified: Thu Jul 27 17:34:32 2023, max compression
+gzip compressed data, was "messageflux-0.3.2.tar", last modified: Sat Jul 29 07:16:22 2023, max compression
```

## Comparing `messageflux-0.3.1.tar` & `messageflux-0.3.2.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.725883 messageflux-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 17:34:19.000000 messageflux-0.3.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-27 17:34:19.000000 messageflux-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-27 17:34:19.000000 messageflux-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-27 17:34:32.725883 messageflux-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-27 17:34:19.000000 messageflux-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 17:34:21.000000 messageflux-0.3.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.713882 messageflux-0.3.1/_custom_build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:19.000000 messageflux-0.3.1/_custom_build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-27 17:34:19.000000 messageflux-0.3.1/_custom_build/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-27 17:34:19.000000 messageflux-0.3.1/_custom_build/make_all_extra_requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.717882 messageflux-0.3.1/messageflux/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/base_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/fastmessage_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.717882 messageflux-0.3.1/messageflux/iodevices/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.717882 messageflux-0.3.1/messageflux/iodevices/base/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/base/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/base/input_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/base/input_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/base/output_devices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.717882 messageflux-0.3.1/messageflux/iodevices/collection_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/collection_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/collection_device_wrapper/collection_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/collection_device_wrapper/collection_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.717882 messageflux-0.3.1/messageflux/iodevices/failover_output_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/failover_output_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.717882 messageflux-0.3.1/messageflux/iodevices/file_system/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/file_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/file_system/file_system_device_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24734 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/file_system/file_system_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/file_system/file_system_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/file_system/file_system_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.717882 messageflux-0.3.1/messageflux/iodevices/in_memory_device/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/in_memory_device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/in_memory_device/in_memory_device_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.721882 messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/message_store_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.721882 messageflux-0.3.1/messageflux/iodevices/objectstorage/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/objectstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/objectstorage/s3_message_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.721882 messageflux-0.3.1/messageflux/iodevices/objectstorage/s3api/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/objectstorage/s3api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/objectstorage/s3api/s3bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/objectstorage/s3api/s3client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.721882 messageflux-0.3.1/messageflux/iodevices/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/rabbitmq/fs_poison_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.721882 messageflux-0.3.1/messageflux/iodevices/round_robin_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/round_robin_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.721882 messageflux-0.3.1/messageflux/iodevices/short_circuit_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/short_circuit_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/short_circuit_device_wrapper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.721882 messageflux-0.3.1/messageflux/iodevices/transformer_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/transformer_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.721882 messageflux-0.3.1/messageflux/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/logging/LogType.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/logging/bulk_rotating_device_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/logging/bulk_rotating_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/logging/bulk_rotating_handler_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/logging/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/message_handling_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/metadata_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.725883 messageflux-0.3.1/messageflux/multiprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/multiprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/multiprocessing/multiprocessrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/multiprocessing/singleprocesshandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/pipeline_service.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/server_loop_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.725883 messageflux-0.3.1/messageflux/service_addons/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/service_addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/service_addons/loop_health_addon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.725883 messageflux-0.3.1/messageflux/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/utils/filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.717882 messageflux-0.3.1/messageflux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-27 17:34:32.000000 messageflux-0.3.1/messageflux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-27 17:34:32.000000 messageflux-0.3.1/messageflux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 17:34:32.000000 messageflux-0.3.1/messageflux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-27 17:34:32.000000 messageflux-0.3.1/messageflux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 17:34:32.000000 messageflux-0.3.1/messageflux.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-27 17:34:19.000000 messageflux-0.3.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-27 17:34:19.000000 messageflux-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-27 17:34:19.000000 messageflux-0.3.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-27 17:34:32.000000 messageflux-0.3.1/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-27 17:34:19.000000 messageflux-0.3.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 17:34:19.000000 messageflux-0.3.1/requirements-fastmessage.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 17:34:19.000000 messageflux-0.3.1/requirements-objectstorage.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 17:34:19.000000 messageflux-0.3.1/requirements-rabbitmq.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 17:34:19.000000 messageflux-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 17:34:32.725883 messageflux-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.460383 messageflux-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-29 07:16:11.000000 messageflux-0.3.2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-29 07:16:11.000000 messageflux-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-29 07:16:11.000000 messageflux-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-29 07:16:22.460383 messageflux-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-29 07:16:11.000000 messageflux-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 07:16:12.000000 messageflux-0.3.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.452383 messageflux-0.3.2/_custom_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:11.000000 messageflux-0.3.2/_custom_build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-29 07:16:11.000000 messageflux-0.3.2/_custom_build/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-29 07:16:11.000000 messageflux-0.3.2/_custom_build/make_all_extra_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.452383 messageflux-0.3.2/messageflux/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/fastmessage_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.452383 messageflux-0.3.2/messageflux/iodevices/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.452383 messageflux-0.3.2/messageflux/iodevices/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/base/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/base/input_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/base/input_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/base/output_devices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/collection_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/collection_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/collection_device_wrapper/collection_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/collection_device_wrapper/collection_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/failover_output_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/failover_output_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/file_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/file_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/file_system/file_system_device_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24734 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/file_system/file_system_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/file_system/file_system_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/file_system/file_system_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/in_memory_device/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/in_memory_device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/in_memory_device/in_memory_device_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/message_store_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/objectstorage/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/objectstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/objectstorage/s3_message_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/objectstorage/s3api/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/objectstorage/s3api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/objectstorage/s3api/s3bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/objectstorage/s3api/s3client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/rabbitmq/fs_poison_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/round_robin_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/round_robin_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.456383 messageflux-0.3.2/messageflux/iodevices/short_circuit_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/short_circuit_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/short_circuit_device_wrapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.460383 messageflux-0.3.2/messageflux/iodevices/transformer_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/transformer_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.460383 messageflux-0.3.2/messageflux/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/logging/LogType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/logging/bulk_rotating_device_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/logging/bulk_rotating_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/logging/bulk_rotating_handler_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/logging/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/message_handling_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/metadata_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.460383 messageflux-0.3.2/messageflux/multiprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/multiprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/multiprocessing/multiprocessrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/multiprocessing/singleprocesshandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/pipeline_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/server_loop_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.460383 messageflux-0.3.2/messageflux/service_addons/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/service_addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/service_addons/loop_health_addon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.460383 messageflux-0.3.2/messageflux/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-29 07:16:11.000000 messageflux-0.3.2/messageflux/utils/filesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:16:22.452383 messageflux-0.3.2/messageflux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-29 07:16:22.000000 messageflux-0.3.2/messageflux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-29 07:16:22.000000 messageflux-0.3.2/messageflux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 07:16:22.000000 messageflux-0.3.2/messageflux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-29 07:16:22.000000 messageflux-0.3.2/messageflux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-29 07:16:22.000000 messageflux-0.3.2/messageflux.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-29 07:16:11.000000 messageflux-0.3.2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-29 07:16:11.000000 messageflux-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-29 07:16:11.000000 messageflux-0.3.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-29 07:16:22.000000 messageflux-0.3.2/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-29 07:16:11.000000 messageflux-0.3.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 07:16:11.000000 messageflux-0.3.2/requirements-fastmessage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-29 07:16:11.000000 messageflux-0.3.2/requirements-objectstorage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 07:16:11.000000 messageflux-0.3.2/requirements-rabbitmq.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 07:16:11.000000 messageflux-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 07:16:22.460383 messageflux-0.3.2/setup.cfg
```

### Comparing `messageflux-0.3.1/LICENSE` & `messageflux-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/PKG-INFO` & `messageflux-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messageflux
-Version: 0.3.1
+Version: 0.3.2
 Author-email: Aviv Salem <avivsalem@gmail.com>
 Maintainer-email: Aviv Salem <avivsalem@gmail.com>, Nir Schulman <narsssx@gmail.com>, Rafael Zilberman <Zilberman.rafi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Avivsalem/MessageFlux/
 Project-URL: Documentation, https://messageflux.readthedocs.io/
 Platform: win32
 Platform: linux
```

### Comparing `messageflux-0.3.1/README.md` & `messageflux-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/_custom_build/make_all_extra_requirements.py` & `messageflux-0.3.2/_custom_build/make_all_extra_requirements.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/base_service.py` & `messageflux-0.3.2/messageflux/base_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/fastmessage_handler.py` & `messageflux-0.3.2/messageflux/fastmessage_handler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/base/__init__.py` & `messageflux-0.3.2/messageflux/iodevices/base/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/base/common.py` & `messageflux-0.3.2/messageflux/iodevices/base/common.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/base/input_devices.py` & `messageflux-0.3.2/messageflux/iodevices/base/input_devices.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/base/input_transaction.py` & `messageflux-0.3.2/messageflux/iodevices/base/input_transaction.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/base/output_devices.py` & `messageflux-0.3.2/messageflux/iodevices/base/output_devices.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/collection_device_wrapper/collection_input_device.py` & `messageflux-0.3.2/messageflux/iodevices/collection_device_wrapper/collection_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/collection_device_wrapper/collection_output_device.py` & `messageflux-0.3.2/messageflux/iodevices/collection_device_wrapper/collection_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py` & `messageflux-0.3.2/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/file_system/__init__.py` & `messageflux-0.3.2/messageflux/iodevices/file_system/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/file_system/file_system_device_manager_base.py` & `messageflux-0.3.2/messageflux/iodevices/file_system/file_system_device_manager_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/file_system/file_system_input_device.py` & `messageflux-0.3.2/messageflux/iodevices/file_system/file_system_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/file_system/file_system_output_device.py` & `messageflux-0.3.2/messageflux/iodevices/file_system/file_system_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/file_system/file_system_serializer.py` & `messageflux-0.3.2/messageflux/iodevices/file_system/file_system_serializer.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/in_memory_device/in_memory_device_manager.py` & `messageflux-0.3.2/messageflux/iodevices/in_memory_device/in_memory_device_manager.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py` & `messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/message_store_base.py` & `messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/message_store_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py` & `messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py` & `messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py` & `messageflux-0.3.2/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/objectstorage/s3_message_store.py` & `messageflux-0.3.2/messageflux/iodevices/objectstorage/s3_message_store.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/objectstorage/s3api/s3bucket.py` & `messageflux-0.3.2/messageflux/iodevices/objectstorage/s3api/s3bucket.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/objectstorage/s3api/s3client.py` & `messageflux-0.3.2/messageflux/iodevices/objectstorage/s3api/s3client.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/rabbitmq/fs_poison_counter.py` & `messageflux-0.3.2/messageflux/iodevices/rabbitmq/fs_poison_counter.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py` & `messageflux-0.3.2/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py` & `messageflux-0.3.2/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py` & `messageflux-0.3.2/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py` & `messageflux-0.3.2/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py` & `messageflux-0.3.2/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/short_circuit_device_wrapper/common.py` & `messageflux-0.3.2/messageflux/iodevices/short_circuit_device_wrapper/common.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py` & `messageflux-0.3.2/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py` & `messageflux-0.3.2/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py` & `messageflux-0.3.2/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py` & `messageflux-0.3.2/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py` & `messageflux-0.3.2/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/logging/bulk_rotating_device_handler.py` & `messageflux-0.3.2/messageflux/logging/bulk_rotating_device_handler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/logging/bulk_rotating_file_handler.py` & `messageflux-0.3.2/messageflux/logging/bulk_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/logging/bulk_rotating_handler_base.py` & `messageflux-0.3.2/messageflux/logging/bulk_rotating_handler_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/message_handling_service.py` & `messageflux-0.3.2/messageflux/message_handling_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/multiprocessing/multiprocessrunner.py` & `messageflux-0.3.2/messageflux/multiprocessing/multiprocessrunner.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/multiprocessing/singleprocesshandler.py` & `messageflux-0.3.2/messageflux/multiprocessing/singleprocesshandler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/pipeline_service.py` & `messageflux-0.3.2/messageflux/pipeline_service.py`

 * *Files 19% similar despite different names*

```diff
@@ -79,14 +79,19 @@
                  pipeline_handler: PipelineHandlerBase,
                  output_device_manager: Optional[OutputDeviceManager] = None,
                  **kwargs):
         super().__init__(**kwargs)
         self._output_device_manager = output_device_manager
         self._pipeline_handler = pipeline_handler
 
+    def _prepare_service(self):
+        super()._prepare_service()
+        if self._output_device_manager is not None:
+            self._output_device_manager.connect()
+
     def _handle_message_batch(self, batch: List[Tuple[InputDevice, ReadResult]]):
         for input_device, read_result in batch:
             pipeline_handler_result = self._pipeline_handler.handle_message(input_device, read_result)
             if pipeline_handler_result is not None:
                 if not isinstance(pipeline_handler_result, List):
                     pipeline_handler_result = [pipeline_handler_result]
                 for pipeline_result in pipeline_handler_result:
@@ -95,7 +100,14 @@
                                         f"'{pipeline_result.output_device_name}', "
                                         f"but no output_device_manager was given")
                         continue
 
                     output_device = self._output_device_manager.get_output_device(pipeline_result.output_device_name)
                     output_device.send_message(message=pipeline_result.message_bundle.message,
                                                device_headers=pipeline_result.message_bundle.device_headers)
+
+    def _finalize_service(self, exception: Optional[Exception] = None):
+        try:
+            super()._finalize_service(exception)
+        finally:
+            if self._output_device_manager is not None:
+                self._output_device_manager.disconnect()
```

### Comparing `messageflux-0.3.1/messageflux/server_loop_service.py` & `messageflux-0.3.2/messageflux/server_loop_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/service_addons/loop_health_addon.py` & `messageflux-0.3.2/messageflux/service_addons/loop_health_addon.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/utils/__init__.py` & `messageflux-0.3.2/messageflux/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/utils/context.py` & `messageflux-0.3.2/messageflux/utils/context.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux/utils/filesystem.py` & `messageflux-0.3.2/messageflux/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/messageflux.egg-info/PKG-INFO` & `messageflux-0.3.2/messageflux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messageflux
-Version: 0.3.1
+Version: 0.3.2
 Author-email: Aviv Salem <avivsalem@gmail.com>
 Maintainer-email: Aviv Salem <avivsalem@gmail.com>, Nir Schulman <narsssx@gmail.com>, Rafael Zilberman <Zilberman.rafi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Avivsalem/MessageFlux/
 Project-URL: Documentation, https://messageflux.readthedocs.io/
 Platform: win32
 Platform: linux
```

### Comparing `messageflux-0.3.1/messageflux.egg-info/SOURCES.txt` & `messageflux-0.3.2/messageflux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.1/pyproject.toml` & `messageflux-0.3.2/pyproject.toml`

 * *Files identical despite different names*

