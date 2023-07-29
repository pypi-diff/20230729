# Comparing `tmp/cloudquery-plugin-sdk-0.0.6.tar.gz` & `tmp/cloudquery-plugin-sdk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudquery-plugin-sdk-0.0.6.tar", last modified: Fri Jul 28 12:48:07 2023, max compression
+gzip compressed data, was "cloudquery-plugin-sdk-0.0.7.tar", last modified: Sat Jul 29 19:42:17 2023, max compression
```

## Comparing `cloudquery-plugin-sdk-0.0.6.tar` & `cloudquery-plugin-sdk-0.0.7.tar`

### file list

```diff
@@ -1,70 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:48:07.322212 cloudquery-plugin-sdk-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-28 12:48:07.322212 cloudquery-plugin-sdk-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:48:07.310212 cloudquery-plugin-sdk-0.0.6/cloudquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:48:07.314212 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:48:07.314212 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/docs/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/docs/markdown_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:48:07.314212 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:48:07.314212 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/internal/memdb/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/internal/memdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/internal/memdb/memdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:48:07.314212 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/internal/servers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/internal/servers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:48:07.314212 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/internal/servers/discovery_v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/internal/servers/discovery_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/internal/servers/discovery_v1/discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:48:07.314212 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/internal/servers/plugin_v3/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/internal/servers/plugin_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/internal/servers/plugin_v3/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:48:07.314212 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/message/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/message/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/message/write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:48:07.314212 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:48:07.318212 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scalar/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scalar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scalar/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scalar/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scalar/date32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scalar/float64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scalar/int64.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scalar/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scalar/scalar_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scalar/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:48:07.318212 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scheduler/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scheduler/table_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:48:07.322212 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/schema/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/schema/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/schema/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/schema/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:48:07.322212 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/serve/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/serve/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:48:07.322212 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/transformers/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/transformers/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:48:07.322212 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/types/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/types/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:48:07.322212 cloudquery-plugin-sdk-0.0.6/cloudquery_plugin_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-28 12:48:07.000000 cloudquery-plugin-sdk-0.0.6/cloudquery_plugin_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-28 12:48:07.000000 cloudquery-plugin-sdk-0.0.6/cloudquery_plugin_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 12:48:07.000000 cloudquery-plugin-sdk-0.0.6/cloudquery_plugin_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 12:48:07.000000 cloudquery-plugin-sdk-0.0.6/cloudquery_plugin_sdk.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 12:48:07.000000 cloudquery-plugin-sdk-0.0.6/cloudquery_plugin_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-28 12:48:07.000000 cloudquery-plugin-sdk-0.0.6/cloudquery_plugin_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 12:48:07.000000 cloudquery-plugin-sdk-0.0.6/cloudquery_plugin_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 12:48:07.326212 cloudquery-plugin-sdk-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-28 12:47:41.000000 cloudquery-plugin-sdk-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.463659 cloudquery-plugin-sdk-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-29 19:42:17.463659 cloudquery-plugin-sdk-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.447659 cloudquery-plugin-sdk-0.0.7/cloudquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.455659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.455659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/docs/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/docs/markdown_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.455659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.455659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/memdb/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/memdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/memdb/memdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.455659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/servers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.459659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/servers/discovery_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/servers/discovery_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/servers/discovery_v1/discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.459659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/servers/plugin_v3/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/servers/plugin_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/servers/plugin_v3/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.459659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/message/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/message/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/message/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.459659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.463659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/date32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/date64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/scalar_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/uint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.463659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scheduler/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scheduler/table_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.463659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/schema/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/schema/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/schema/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/schema/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.463659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/serve/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.463659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/transformers/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/transformers/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.463659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/types/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/types/uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.463659 cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-29 19:42:17.000000 cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-29 19:42:17.000000 cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 19:42:17.000000 cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 19:42:17.000000 cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 19:42:17.000000 cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-29 19:42:17.000000 cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 19:42:17.000000 cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 19:42:17.467659 cloudquery-plugin-sdk-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/setup.py
```

### Comparing `cloudquery-plugin-sdk-0.0.6/PKG-INFO` & `cloudquery-plugin-sdk-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudquery-plugin-sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: CloudQuery Plugin SDK for Python
 Home-page: https://github.com/cloudquery/plugin-sdk-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/docs/generator.py` & `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/docs/generator.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/docs/markdown_templates.py` & `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/docs/markdown_templates.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/internal/memdb/memdb.py` & `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/memdb/memdb.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,22 +7,34 @@
 NAME = "memdb"
 VERSION = "development"
 
 
 class MemDB(plugin.Plugin):
     def __init__(self) -> None:
         super().__init__(NAME, VERSION)
-        self._tables: List[schema.Table] = [
-            schema.Table("test_table", [schema.Column("test_column", pa.int64())])
-        ]
-        self._memory_db: Dict[str, pa.record] = {
-            "test_table": pa.record_batch([pa.array([1, 2, 3])], names=["test_column"])
-        }
+        self._db: Dict[str, pa.RecordBatch] = {}
+        self._tables: Dict[str, schema.Table] = {}
 
     def get_tables(self, options: plugin.TableOptions = None) -> List[plugin.Table]:
-        return self._tables
+        tables = list(self._tables.values())
+        return schema.filter_dfs(tables, options.tables, options.skip_tables)
 
     def sync(
         self, options: plugin.SyncOptions
     ) -> Generator[message.SyncMessage, None, None]:
-        for table, record in self._memory_db.items():
+        for table, record in self._db.items():
             yield message.SyncInsertMessage(record)
+
+    def write(self, msg_iterator: Generator[message.WriteMessage, None, None]) -> None:
+        for msg in msg_iterator:
+            if type(msg) == message.WriteMigrateTableMessage:
+                if msg.table.name not in self._db:
+                    self._db[msg.table.name] = msg.table
+                    self._tables[msg.table.name] = msg.table
+            elif type(msg) == message.WriteInsertMessage:
+                table = schema.Table.from_arrow_schema(msg.record.schema)
+                self._db[table.name] = msg.record
+            else:
+                raise NotImplementedError(f"Unknown message type {type(msg)}")
+
+    def close(self) -> None:
+        self._db = {}
```

### Comparing `cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/plugin/plugin.py` & `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/plugin/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import queue
 from dataclasses import dataclass
-from typing import List
+from typing import List, Generator
 
 from cloudquery.sdk.schema import Table
+from cloudquery.sdk import message
 
 MIGRATE_MODE_STRINGS = ["safe", "force"]
 
 
 @dataclass
 class TableOptions:
     tables: List[str] = None
@@ -42,12 +43,15 @@
 
     def version(self) -> str:
         return self._version
 
     def get_tables(self, options: TableOptions) -> List[Table]:
         raise NotImplementedError()
 
-    def sync(self, options: SyncOptions, results: queue.Queue) -> None:
+    def sync(self, options: SyncOptions) -> Generator[message.SyncMessage, None, None]:
+        raise NotImplementedError()
+
+    def write(self, writer: Generator[message.WriteMessage, None, None]) -> None:
         raise NotImplementedError()
 
     def close(self) -> None:
-        pass
+        raise NotImplementedError()
```

### Comparing `cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scalar/binary.py` & `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/binary.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from cloudquery.sdk.scalar import Scalar, ScalarInvalidTypeError
 from .scalar import NULL_VALUE
 
 
 class Binary(Scalar):
-    def __init__(self, valid: bool = False, value: bytes = None):
-        self._valid = valid
-        self._value = value
-
     def __eq__(self, scalar: Scalar) -> bool:
         if scalar is None:
             return False
         if type(scalar) == Binary:
             return self._value == scalar._value and self._valid == scalar._valid
         return False
 
-    def __str__(self) -> str:
-        return str(self._value) if self._valid else NULL_VALUE
-
     @property
     def value(self):
         return self._value
 
-    def set(self, scalar):
-        if scalar is None:
+    def set(self, value: any):
+        if value is None:
+            return
+
+        if isinstance(value, Binary):
+            self._valid = value.is_valid
+            self._value = value.value
             return
 
-        if type(scalar) == bytes:
+        if type(value) == bytes:
             self._valid = True
-            self._value = scalar
-        elif type(scalar) == str:
+            self._value = value
+        elif type(value) == str:
             self._valid = True
-            self._value = scalar.encode()
+            self._value = value.encode()
         else:
-            raise ScalarInvalidTypeError("Invalid type for Binary scalar")
+            raise ScalarInvalidTypeError(
+                "Invalid type {} for Binary scalar".format(type(value))
+            )
```

### Comparing `cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scalar/bool.py` & `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/bool.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,37 +13,38 @@
     elif lower_input in false_strings:
         return False
     else:
         raise ScalarInvalidTypeError("Invalid boolean string: {}".format(input_string))
 
 
 class Bool(Scalar):
-    def __init__(self, valid: bool = False, value: bool = False) -> None:
-        self._valid = valid
-        self._value = value
-
     def __eq__(self, scalar: Scalar) -> bool:
         if scalar is None:
             return False
         if type(scalar) == Bool:
             return self._value == scalar._value and self._valid == scalar._valid
         return False
 
-    def __str__(self) -> str:
-        return str(self._value) if self._valid else NULL_VALUE
-
     @property
     def value(self):
         return self._value
 
     def set(self, value: Any):
         if value is None:
+            self._valid = False
+            return
+
+        if isinstance(value, Bool):
+            self._valid = value.is_valid
+            self._value = value.value
             return
 
         if type(value) == bool:
             self._value = value
         elif type(value) == str:
             self._value = parse_string_to_bool(value)
         else:
-            raise ScalarInvalidTypeError("Invalid type for Bool scalar")
+            raise ScalarInvalidTypeError(
+                "Invalid type {} for Bool scalar".format(type(value))
+            )
 
         self._valid = True
```

### Comparing `cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scalar/date32.py` & `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/date32.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from cloudquery.sdk.scalar import Scalar, ScalarInvalidTypeError, NULL_VALUE
 from datetime import datetime, time
 from typing import Any
 
 
 class Date32(Scalar):
-    def __init__(self, valid: bool = False, value: bool = False) -> None:
-        self._valid = valid
-        self._value = value
-
     def __eq__(self, scalar: Scalar) -> bool:
         if scalar is None:
             return False
         if type(scalar) == Date32:
             return self._value == scalar._value and self._valid == scalar._valid
         return False
 
-    def __str__(self) -> str:
-        return str(self._value) if self._valid else NULL_VALUE
-
     @property
     def value(self):
         return self._value
 
     def set(self, value: Any):
         if value is None:
+            self._valid = False
+            return
+
+        if isinstance(value, Date32):
+            self._valid = value.is_valid
+            self._value = value.value
             return
 
         if type(value) == datetime:
             self._value = value
         elif type(value) == str:
             self._value = datetime.strptime(value, "%Y-%m-%d")
         elif type(value) == time:
             self._value = datetime.combine(datetime.today(), value)
         else:
-            raise ScalarInvalidTypeError("Invalid type for Bool scalar")
+            raise ScalarInvalidTypeError(
+                "Invalid type {} for Date32 scalar".format(type(value))
+            )
 
         self._valid = True
```

### Comparing `cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scalar/float64.py` & `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/uuid.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,41 @@
+import uuid
 from cloudquery.sdk.scalar import Scalar, ScalarInvalidTypeError
 
 
-class Float64(Scalar):
-    def __init__(self, valid: bool = False, value: float = None):
-        self._valid = valid
-        self._value = value
+class UUID(Scalar):
+    def __init__(self, valid: bool = False, value: uuid.UUID = None):
+        super().__init__(valid, value)
 
     def __eq__(self, scalar: Scalar) -> bool:
         if scalar is None:
             return False
-        if type(scalar) == Float64:
+        if type(scalar) == UUID:
             return self._value == scalar._value and self._valid == scalar._valid
         return False
 
     @property
     def value(self):
         return self._value
 
-    def set(self, value):
+    def set(self, value: any):
         if value is None:
+            self._valid = False
             return
 
-        if type(value) == int:
-            self._value = float(value)
-        elif type(value) == float:
+        if isinstance(value, UUID):
+            self._valid = value.is_valid
+            self._value = value.value
+            return
+
+        if type(value) == uuid.UUID:
             self._value = value
         elif type(value) == str:
             try:
-                self._value = float(value)
-            except ValueError:
-                raise ScalarInvalidTypeError("Invalid type for Float64 scalar")
+                self._value = uuid.UUID(value)
+            except ValueError as e:
+                raise ScalarInvalidTypeError("Invalid type for UUID scalar") from e
         else:
-            raise ScalarInvalidTypeError("Invalid type for Binary scalar")
+            raise ScalarInvalidTypeError(
+                "Invalid type {} for UUID scalar".format(type(value))
+            )
         self._valid = True
```

### Comparing `cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scalar/int64.py` & `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/string.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 from cloudquery.sdk.scalar import Scalar, ScalarInvalidTypeError
+from .scalar import NULL_VALUE
 
 
-class Int64(Scalar):
-    def __init__(self, valid: bool = False, value: float = None):
-        self._valid = valid
-        self._value = value
-
+class String(Scalar):
     def __eq__(self, scalar: Scalar) -> bool:
         if scalar is None:
             return False
-        if type(scalar) == Int64:
+        if type(scalar) == String:
             return self._value == scalar._value and self._valid == scalar._valid
         return False
 
     @property
     def value(self):
         return self._value
 
-    def set(self, value):
+    def set(self, value: any):
         if value is None:
             return
 
-        if type(value) == int:
+        if isinstance(value, String):
+            self._valid = value._valid
+            self._value = value.value
+            return
+
+        if type(value) == str:
+            self._valid = True
             self._value = value
-        elif type(value) == float:
-            self._value = int(value)
-        elif type(value) == str:
-            try:
-                self._value = int(value)
-            except ValueError as e:
-                raise ScalarInvalidTypeError("Invalid type for Int64 scalar") from e
         else:
             raise ScalarInvalidTypeError(
-                "Invalid type {} for Int64 scalar".format(type(value))
+                "Invalid type {} for String scalar".format(type(value))
             )
-        self._valid = True
```

### Comparing `cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scheduler/scheduler.py` & `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scheduler/scheduler.py`

 * *Files 8% similar despite different names*

```diff
@@ -99,15 +99,26 @@
                 )
             else:
                 self._logger.debug(
                     "table resolver started", table=resolver.table.name, depth=depth
                 )
             total_resources = 0
             for item in resolver.resolve(client, parent_item):
-                resource = self.resolve_resource(resolver, client, parent_item, item)
+                try:
+                    resource = self.resolve_resource(
+                        resolver, client, parent_item, item
+                    )
+                except Exception as e:
+                    self._logger.error(
+                        "failed to resolve resource",
+                        table=resolver.table.name,
+                        depth=depth,
+                        exception=e,
+                    )
+                    continue
                 res.put(SyncInsertMessage(resource.to_arrow_record()))
                 for child_resolvers in resolver.child_resolvers:
                     self._pools[depth + 1].submit(
                         self.resolve_table,
                         child_resolvers,
                         depth + 1,
                         client,
```

### Comparing `cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/scheduler/table_resolver.py` & `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scheduler/table_resolver.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/schema/resource.py` & `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/schema/resource.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/schema/table.py` & `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/schema/table.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from typing import List, Generator, Any
-
+import fnmatch
 import pyarrow as pa
 
 from cloudquery.sdk.schema import arrow
 from .column import Column
 
 
 class Client:
@@ -49,14 +49,27 @@
     def primary_keys(self):
         return [column.name for column in self.columns if column.primary_key]
 
     @property
     def incremental_keys(self):
         return [column.name for column in self.columns if column.incremental_key]
 
+    @classmethod
+    def from_arrow_schema(cls, schema: pa.Schema) -> Table:
+        columns = []
+        for field in schema:
+            columns.append(Column.from_arrow_field(field))
+        return cls(
+            name=schema.metadata[arrow.METADATA_TABLE_NAME].decode("utf-8"),
+            columns=columns,
+            description=schema.metadata.get(arrow.METADATA_TABLE_DESCRIPTION).decode(
+                "utf-8"
+            ),
+        )
+
     def to_arrow_schema(self):
         fields = []
         md = {
             arrow.METADATA_TABLE_NAME: self.name,
             arrow.METADATA_TABLE_DESCRIPTION: self.description,
             # arrow.METADATA_CONSTRAINT_NAME:
         }
@@ -70,7 +83,24 @@
 
 
 def tables_to_arrow_schemas(tables: List[Table]):
     schemas = []
     for table in tables:
         schemas.append(table.to_arrow_schema())
     return schemas
+
+
+def filter_dfs(
+    tables: List[Table], include_tables: List[str], skip_tables: List[str]
+) -> List[Table]:
+    filtered: List[Table] = []
+    for table in tables:
+        matched = False
+        for include_table in include_tables:
+            if fnmatch.fnmatch(table.name, include_table):
+                matched = True
+        for skip_table in skip_tables:
+            if fnmatch.fnmatch(table.name, skip_table):
+                matched = False
+        if matched:
+            filtered.append(table)
+    return filtered
```

### Comparing `cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/serve/plugin.py` & `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/serve/plugin.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/transformers/openapi.py` & `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/transformers/openapi.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 from typing import Dict, List
 import pyarrow as pa
+from cloudquery.sdk.types import JSONType
 from cloudquery.sdk.schema import Column
 
 
 def oapi_type_to_arrow_type(field) -> pa.DataType:
     oapi_type = field.get("type")
     if oapi_type == "string":
         return pa.string()
     elif oapi_type == "number":
         return pa.int64()
+    elif oapi_type == "integer":
+        return pa.int64()
     elif oapi_type == "boolean":
         return pa.bool_()
+    elif oapi_type == "array":
+        return JSONType()
+    elif oapi_type == "object":
+        return JSONType()
+    elif oapi_type is None and "$ref" in field:
+        return JSONType()
     else:
         return pa.string()
 
 
-def oapi_properties_to_columns(properties: Dict) -> List[Column]:
+def oapi_definition_to_columns(definition: Dict) -> List[Column]:
     columns = []
-    for key, value in properties.items():
+    for key, value in definition["properties"].items():
+        column_type = oapi_type_to_arrow_type(value)
         columns.append(
-            Column(name=key, type=value, description=value.get("description"))
+            Column(name=key, type=column_type, description=value.get("description"))
         )
     return columns
```

### Comparing `cloudquery-plugin-sdk-0.0.6/cloudquery/sdk/types/uuid.py` & `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/types/uuid.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import pyarrow as pa
-import pyarrow
-import sys
 
 
-class UuidType(pa.PyExtensionType):
+class UUIDType(pa.PyExtensionType):
     def __init__(self):
         pa.PyExtensionType.__init__(self, pa.binary(16))
 
     def __reduce__(self):
-        return UuidType, ()
+        return UUIDType, ()
 
     def __arrow_ext_serialize__(self):
         # since we don't have a parameterized type, we don't need extra
         # metadata to be deserialized
         return b"uuid-serialized"
 
     @classmethod
     def __arrow_ext_deserialize__(self, storage_type, serialized):
         # return an instance of this subclass given the serialized
         # metadata.
-        return UuidType()
+        return UUIDType()
```

### Comparing `cloudquery-plugin-sdk-0.0.6/cloudquery_plugin_sdk.egg-info/PKG-INFO` & `cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudquery-plugin-sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: CloudQuery Plugin SDK for Python
 Home-page: https://github.com/cloudquery/plugin-sdk-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `cloudquery-plugin-sdk-0.0.6/cloudquery_plugin_sdk.egg-info/SOURCES.txt` & `cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -19,32 +19,41 @@
 cloudquery/sdk/message/write.py
 cloudquery/sdk/plugin/__init__.py
 cloudquery/sdk/plugin/plugin.py
 cloudquery/sdk/scalar/__init__.py
 cloudquery/sdk/scalar/binary.py
 cloudquery/sdk/scalar/bool.py
 cloudquery/sdk/scalar/date32.py
-cloudquery/sdk/scalar/float64.py
-cloudquery/sdk/scalar/int64.py
+cloudquery/sdk/scalar/date64.py
+cloudquery/sdk/scalar/float.py
+cloudquery/sdk/scalar/int.py
+cloudquery/sdk/scalar/json.py
+cloudquery/sdk/scalar/list.py
 cloudquery/sdk/scalar/scalar.py
 cloudquery/sdk/scalar/scalar_factory.py
+cloudquery/sdk/scalar/string.py
+cloudquery/sdk/scalar/timestamp.py
+cloudquery/sdk/scalar/uint.py
 cloudquery/sdk/scalar/uuid.py
+cloudquery/sdk/scalar/vector.py
 cloudquery/sdk/scheduler/__init__.py
 cloudquery/sdk/scheduler/scheduler.py
 cloudquery/sdk/scheduler/table_resolver.py
 cloudquery/sdk/schema/__init__.py
 cloudquery/sdk/schema/arrow.py
 cloudquery/sdk/schema/column.py
 cloudquery/sdk/schema/resource.py
 cloudquery/sdk/schema/table.py
 cloudquery/sdk/serve/__init__.py
 cloudquery/sdk/serve/plugin.py
 cloudquery/sdk/transformers/__init__.py
 cloudquery/sdk/transformers/openapi.py
 cloudquery/sdk/transformers/transformers.py
+cloudquery/sdk/types/__init__.py
+cloudquery/sdk/types/json.py
 cloudquery/sdk/types/uuid.py
 cloudquery_plugin_sdk.egg-info/PKG-INFO
 cloudquery_plugin_sdk.egg-info/SOURCES.txt
 cloudquery_plugin_sdk.egg-info/dependency_links.txt
 cloudquery_plugin_sdk.egg-info/namespace_packages.txt
 cloudquery_plugin_sdk.egg-info/not-zip-safe
 cloudquery_plugin_sdk.egg-info/requires.txt
```

### Comparing `cloudquery-plugin-sdk-0.0.6/setup.py` & `cloudquery-plugin-sdk-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 packages = [
     package
     for package in setuptools.PEP420PackageFinder.find()
     if package.startswith("cloudquery")
 ]
 setuptools.setup(
     name=name,
-    version="0.0.6",
+    version="0.0.7",
     description=description,
     long_description=long_description,
     author="CloudQuery LTD",
     author_email="pypi-packages@cloudquery.io",
     license="MPL-2.0",
     url=url,
     classifiers=[
```

