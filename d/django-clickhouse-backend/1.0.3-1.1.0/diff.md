# Comparing `tmp/django-clickhouse-backend-1.0.3.tar.gz` & `tmp/django-clickhouse-backend-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-clickhouse-backend-1.0.3.tar", last modified: Thu Jun 29 15:05:02 2023, max compression
+gzip compressed data, was "django-clickhouse-backend-1.1.0.tar", last modified: Sat Jul 29 14:26:39 2023, max compression
```

## Comparing `django-clickhouse-backend-1.0.3.tar` & `django-clickhouse-backend-1.1.0.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.680181 django-clickhouse-backend-1.0.3/
--rw-rw-r--   0 wen       (1000) wen       (1000)     1067 2022-10-18 14:44:39.000000 django-clickhouse-backend-1.0.3/LICENSE
--rw-rw-r--   0 wen       (1000) wen       (1000)       34 2022-10-28 13:33:01.000000 django-clickhouse-backend-1.0.3/MANIFEST.in
--rw-rw-r--   0 wen       (1000) wen       (1000)    13838 2023-06-29 15:05:02.680181 django-clickhouse-backend-1.0.3/PKG-INFO
--rw-rw-r--   0 wen       (1000) wen       (1000)    12722 2023-06-22 14:45:45.000000 django-clickhouse-backend-1.0.3/README.md
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.668181 django-clickhouse-backend-1.0.3/clickhouse_backend/
--rw-rw-r--   0 wen       (1000) wen       (1000)        5 2023-06-22 14:45:45.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/VERSION
--rw-rw-r--   0 wen       (1000) wen       (1000)      102 2022-08-30 00:45:24.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/__init__.py
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.672181 django-clickhouse-backend-1.0.3/clickhouse_backend/backend/
--rw-rw-r--   0 wen       (1000) wen       (1000)        0 2022-08-30 00:45:24.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/backend/__init__.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     8557 2023-06-24 12:24:00.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/backend/base.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     1365 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/backend/client.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     1980 2023-01-04 14:13:06.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/backend/creation.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     5449 2023-06-24 14:50:47.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/backend/features.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     4360 2023-06-24 12:21:48.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/backend/introspection.py
--rw-rw-r--   0 wen       (1000) wen       (1000)    13424 2023-06-28 14:43:54.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/backend/operations.py
--rw-rw-r--   0 wen       (1000) wen       (1000)    24709 2023-06-24 07:04:29.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/backend/schema.py
--rw-rw-r--   0 wen       (1000) wen       (1000)      196 2023-06-24 07:04:29.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/compat.py
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.672181 django-clickhouse-backend-1.0.3/clickhouse_backend/driver/
--rw-rw-r--   0 wen       (1000) wen       (1000)      986 2023-06-28 13:03:21.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/driver/__init__.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     1975 2023-06-22 07:01:32.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/driver/client.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     4934 2023-06-22 14:45:45.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/driver/connection.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     3367 2023-06-28 14:52:51.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/driver/escape.py
--rw-rw-r--   0 wen       (1000) wen       (1000)      734 2022-10-15 03:05:40.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/driver/pool.py
--rw-rw-r--   0 wen       (1000) wen       (1000)       87 2023-06-28 14:43:54.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/driver/types.py
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.672181 django-clickhouse-backend-1.0.3/clickhouse_backend/idworker/
--rw-rw-r--   0 wen       (1000) wen       (1000)      495 2022-10-16 09:51:45.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/idworker/__init__.py
--rw-rw-r--   0 wen       (1000) wen       (1000)       78 2022-10-16 09:50:31.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/idworker/base.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     4120 2022-10-16 09:50:31.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/idworker/snowflake.py
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.672181 django-clickhouse-backend-1.0.3/clickhouse_backend/models/
--rw-rw-r--   0 wen       (1000) wen       (1000)      507 2023-06-27 13:26:54.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/__init__.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     1671 2023-06-27 12:46:23.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/base.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     3618 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/engines.py
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.676181 django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/
--rw-rw-r--   0 wen       (1000) wen       (1000)    15813 2023-06-26 14:58:38.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/__init__.py
--rw-rw-r--   0 wen       (1000) wen       (1000)    11632 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/array.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     2613 2023-06-24 13:02:34.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/base.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     4212 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/integer.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     1278 2023-06-29 14:56:49.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/json.py
--rw-rw-r--   0 wen       (1000) wen       (1000)    12991 2023-06-24 12:37:01.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/map.py
--rw-rw-r--   0 wen       (1000) wen       (1000)    13318 2023-06-27 14:52:42.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/tuple.py
--rw-rw-r--   0 wen       (1000) wen       (1000)       95 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/utils.py
--rw-rw-r--   0 wen       (1000) wen       (1000)      981 2023-06-21 11:54:13.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/functions.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     6459 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/indexes.py
--rw-rw-r--   0 wen       (1000) wen       (1000)      623 2022-10-26 15:41:29.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/query.py
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.676181 django-clickhouse-backend-1.0.3/clickhouse_backend/models/sql/
--rw-rw-r--   0 wen       (1000) wen       (1000)       46 2022-10-15 12:11:54.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/sql/__init__.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     7803 2023-06-24 07:04:29.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/sql/compiler.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     1418 2023-06-21 11:54:13.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/sql/query.py
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.680181 django-clickhouse-backend-1.0.3/clickhouse_backend/patch/
--rw-rw-r--   0 wen       (1000) wen       (1000)      138 2023-06-27 12:48:43.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/patch/__init__.py
--rw-rw-r--   0 wen       (1000) wen       (1000)      559 2023-06-28 14:56:30.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/patch/fields.py
--rw-rw-r--   0 wen       (1000) wen       (1000)      308 2023-06-27 12:46:23.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/patch/functions.py
--rw-rw-r--   0 wen       (1000) wen       (1000)      712 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/utils.py
--rw-rw-r--   0 wen       (1000) wen       (1000)      625 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/validators.py
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.680181 django-clickhouse-backend-1.0.3/django_clickhouse_backend.egg-info/
--rw-rw-r--   0 wen       (1000) wen       (1000)    13838 2023-06-29 15:05:02.000000 django-clickhouse-backend-1.0.3/django_clickhouse_backend.egg-info/PKG-INFO
--rw-rw-r--   0 wen       (1000) wen       (1000)     1882 2023-06-29 15:05:02.000000 django-clickhouse-backend-1.0.3/django_clickhouse_backend.egg-info/SOURCES.txt
--rw-rw-r--   0 wen       (1000) wen       (1000)        1 2023-06-29 15:05:02.000000 django-clickhouse-backend-1.0.3/django_clickhouse_backend.egg-info/dependency_links.txt
--rw-rw-r--   0 wen       (1000) wen       (1000)       60 2023-06-29 15:05:02.000000 django-clickhouse-backend-1.0.3/django_clickhouse_backend.egg-info/requires.txt
--rw-rw-r--   0 wen       (1000) wen       (1000)       19 2023-06-29 15:05:02.000000 django-clickhouse-backend-1.0.3/django_clickhouse_backend.egg-info/top_level.txt
--rw-rw-r--   0 wen       (1000) wen       (1000)       81 2022-08-30 00:45:24.000000 django-clickhouse-backend-1.0.3/pyproject.toml
--rw-rw-r--   0 wen       (1000) wen       (1000)       38 2023-06-29 15:05:02.680181 django-clickhouse-backend-1.0.3/setup.cfg
--rw-rw-r--   0 wen       (1000) wen       (1000)     1582 2023-06-24 07:04:29.000000 django-clickhouse-backend-1.0.3/setup.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-07-29 14:26:39.732665 django-clickhouse-backend-1.1.0/
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1067 2022-10-18 14:44:39.000000 django-clickhouse-backend-1.1.0/LICENSE
+-rw-rw-r--   0 wen       (1000) wen       (1000)       34 2022-10-28 13:33:01.000000 django-clickhouse-backend-1.1.0/MANIFEST.in
+-rw-rw-r--   0 wen       (1000) wen       (1000)    13984 2023-07-29 14:26:39.732665 django-clickhouse-backend-1.1.0/PKG-INFO
+-rw-rw-r--   0 wen       (1000) wen       (1000)    12868 2023-07-28 15:15:23.000000 django-clickhouse-backend-1.1.0/README.md
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-07-29 14:26:39.688664 django-clickhouse-backend-1.1.0/clickhouse_backend/
+-rw-rw-r--   0 wen       (1000) wen       (1000)        5 2023-07-28 15:15:23.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/VERSION
+-rw-rw-r--   0 wen       (1000) wen       (1000)      102 2022-08-30 00:45:24.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/__init__.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-07-29 14:26:39.696664 django-clickhouse-backend-1.1.0/clickhouse_backend/backend/
+-rw-rw-r--   0 wen       (1000) wen       (1000)        0 2022-08-30 00:45:24.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/backend/__init__.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     8557 2023-07-28 15:15:23.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/backend/base.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1365 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/backend/client.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1980 2023-01-04 14:13:06.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/backend/creation.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     5449 2023-06-29 15:11:48.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/backend/features.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     4360 2023-06-29 15:11:48.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/backend/introspection.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    13470 2023-07-28 15:15:23.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/backend/operations.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    25010 2023-07-28 15:15:23.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/backend/schema.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)      194 2023-07-28 15:15:23.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/compat.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-07-29 14:26:39.700664 django-clickhouse-backend-1.1.0/clickhouse_backend/driver/
+-rw-rw-r--   0 wen       (1000) wen       (1000)      986 2023-06-29 15:11:48.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/driver/__init__.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1987 2023-07-29 14:23:38.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/driver/client.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     4935 2023-07-28 15:15:23.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/driver/connection.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     3367 2023-06-29 15:11:48.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/driver/escape.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)      734 2022-10-15 03:05:40.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/driver/pool.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)       87 2023-06-29 15:11:48.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/driver/types.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-07-29 14:26:39.704665 django-clickhouse-backend-1.1.0/clickhouse_backend/idworker/
+-rw-rw-r--   0 wen       (1000) wen       (1000)      495 2022-10-16 09:51:45.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/idworker/__init__.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)       78 2022-10-16 09:50:31.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/idworker/base.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     4120 2022-10-16 09:50:31.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/idworker/snowflake.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-07-29 14:26:39.716665 django-clickhouse-backend-1.1.0/clickhouse_backend/models/
+-rw-rw-r--   0 wen       (1000) wen       (1000)      507 2023-06-29 15:11:48.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/models/__init__.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1671 2023-06-29 15:11:48.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/models/base.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     3618 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/models/engines.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-07-29 14:26:39.724665 django-clickhouse-backend-1.1.0/clickhouse_backend/models/fields/
+-rw-rw-r--   0 wen       (1000) wen       (1000)    15813 2023-06-29 15:11:48.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/models/fields/__init__.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    11632 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/models/fields/array.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     2613 2023-06-29 15:11:48.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/models/fields/base.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     4212 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/models/fields/integer.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1278 2023-06-29 15:11:48.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/models/fields/json.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    12991 2023-06-29 15:11:48.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/models/fields/map.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    13318 2023-06-29 15:11:48.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/models/fields/tuple.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)       95 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/models/fields/utils.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)      981 2023-06-21 11:54:13.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/models/functions.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     6459 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/models/indexes.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)      623 2022-10-26 15:41:29.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/models/query.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-07-29 14:26:39.728665 django-clickhouse-backend-1.1.0/clickhouse_backend/models/sql/
+-rw-rw-r--   0 wen       (1000) wen       (1000)       46 2022-10-15 12:11:54.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/models/sql/__init__.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     7761 2023-07-28 15:15:23.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/models/sql/compiler.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1418 2023-06-21 11:54:13.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/models/sql/query.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-07-29 14:26:39.728665 django-clickhouse-backend-1.1.0/clickhouse_backend/patch/
+-rw-rw-r--   0 wen       (1000) wen       (1000)      274 2023-07-28 15:15:23.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/patch/__init__.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-07-29 14:26:39.728665 django-clickhouse-backend-1.1.0/clickhouse_backend/patch/fields/
+-rw-rw-r--   0 wen       (1000) wen       (1000)      704 2023-07-28 15:15:23.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/patch/fields/__init__.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)      559 2023-07-28 15:15:23.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/patch/fields/json.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)      429 2023-07-28 15:15:23.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/patch/functions.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)      712 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/utils.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)      625 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.1.0/clickhouse_backend/validators.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-07-29 14:26:39.732665 django-clickhouse-backend-1.1.0/django_clickhouse_backend.egg-info/
+-rw-rw-r--   0 wen       (1000) wen       (1000)    13984 2023-07-29 14:26:39.000000 django-clickhouse-backend-1.1.0/django_clickhouse_backend.egg-info/PKG-INFO
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1931 2023-07-29 14:26:39.000000 django-clickhouse-backend-1.1.0/django_clickhouse_backend.egg-info/SOURCES.txt
+-rw-rw-r--   0 wen       (1000) wen       (1000)        1 2023-07-29 14:26:39.000000 django-clickhouse-backend-1.1.0/django_clickhouse_backend.egg-info/dependency_links.txt
+-rw-rw-r--   0 wen       (1000) wen       (1000)       60 2023-07-29 14:26:39.000000 django-clickhouse-backend-1.1.0/django_clickhouse_backend.egg-info/requires.txt
+-rw-rw-r--   0 wen       (1000) wen       (1000)       19 2023-07-29 14:26:39.000000 django-clickhouse-backend-1.1.0/django_clickhouse_backend.egg-info/top_level.txt
+-rw-rw-r--   0 wen       (1000) wen       (1000)       81 2022-08-30 00:45:24.000000 django-clickhouse-backend-1.1.0/pyproject.toml
+-rw-rw-r--   0 wen       (1000) wen       (1000)       38 2023-07-29 14:26:39.732665 django-clickhouse-backend-1.1.0/setup.cfg
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1582 2023-07-28 14:46:23.000000 django-clickhouse-backend-1.1.0/setup.py
```

### Comparing `django-clickhouse-backend-1.0.3/LICENSE` & `django-clickhouse-backend-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/PKG-INFO` & `django-clickhouse-backend-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-clickhouse-backend
-Version: 1.0.3
+Version: 1.1.0
 Summary: Django clickHouse database backend.
 Home-page: https://github.com/jayvynl/django-clickhouse-backend
 Author: Lin Zhiwen
 Author-email: zhiwenlin1116@gmail.com
 License: MIT
 Keywords: Django ClickHouse database backend engine driver
 Classifier: Framework :: Django
@@ -53,14 +53,16 @@
 **Notes:**
 
 - Not tested upon all versions of clickhouse-server, clickhouse-server 22.x.y.z or over is suggested.
 - Aggregation functions result in 0 or nan (Not NULL) when data set is empty. max/min/sum/count is 0, avg/STDDEV_POP/VAR_POP is nan.
 - In outer join, clickhouse will set missing columns to empty values (0 for number, empty string for text, unix epoch for date/datatime) instead of NULL. 
   So Count("book") resolve to 1 in a missing LEFT OUTER JOIN match, not 0.
   In aggregation expression Avg("book__rating", default=2.5), default=2.5 have no effect in a missing match.
+- Clickhouse does not support unique constraint and foreignkey constraint. `ForeignKey`, `ManyToManyField` and `OneToOneField` can be used with clickhouse backend, but no database level constraints will be added, so there could be some consistency problems.
+- Clickhouse does not support transaction. If any exception occurs during migrating, then your clickhouse database will be in an untracked state. Any migration should be full tested in test environment before deployed to production environment.
 
 **Requirements:**
 
 - [Python](https://www.python.org/) >= 3.7
 - [Django](https://docs.djangoproject.com/) >= 3.2
 - [clickhouse driver](https://github.com/mymarilyn/clickhouse-driver)
 - [clickhouse pool](https://github.com/ericmccarthy7/clickhouse-pool)
@@ -110,21 +112,17 @@
     },
     'clickhouse': {
         'ENGINE': 'clickhouse_backend.backend',
         'NAME': 'default',
         'HOST': 'localhost',
         'USER': 'DB_USER',
         'PASSWORD': 'DB_PASSWORD',
-        'TEST': {
-            'fake_transaction': True
-        }
     }
 }
 DATABASE_ROUTERS = ['dbrouters.ClickHouseRouter']
-DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'
 ```
 
 ```python
 # dbrouters.py
 from clickhouse_backend.models import ClickhouseModel
 
 def get_subclasses(class_):
@@ -168,16 +166,14 @@
 ```
 
 You should use [database router](https://docs.djangoproject.com/en/4.1/topics/db/multi-db/#automatic-database-routing) to
 automatically route your queries to the right database. In the preceding example, I write a database router which route all
 queries from subclasses of `clickhouse_backend.models.ClickhouseModel` or custom migrations with a `clickhouse` hint key to clickhouse.
 All other queries are routed to the default database (postgresql).
 
-`DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'` is required to working with django migration.
-More details will be covered in [DEFAULT_AUTO_FIELD](https://github.com/jayvynl/django-clickhouse-backend/blob/main/docs/Configurations.md#default_auto_field).
 
 ### Model Definition
 
 Clickhouse backend support django builtin fields and clickhouse specific fields.
 
 Read [fields documentation](https://github.com/jayvynl/django-clickhouse-backend/blob/main/docs/Fields.md) for more.
 
@@ -249,15 +245,15 @@
 ```
 
 this operation will generate migration file under apps/migrations/
 
 then we mirgrate
 
 ```shell
-$ python manage.py migrate
+$ python manage.py migrate --database clickhouse
 ```
 
 for the first time run, this operation will generate django_migrations table with create table sql like this
 
 ```sql
 > show create table django_migrations;
```

### Comparing `django-clickhouse-backend-1.0.3/README.md` & `django-clickhouse-backend-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 **Notes:**
 
 - Not tested upon all versions of clickhouse-server, clickhouse-server 22.x.y.z or over is suggested.
 - Aggregation functions result in 0 or nan (Not NULL) when data set is empty. max/min/sum/count is 0, avg/STDDEV_POP/VAR_POP is nan.
 - In outer join, clickhouse will set missing columns to empty values (0 for number, empty string for text, unix epoch for date/datatime) instead of NULL. 
   So Count("book") resolve to 1 in a missing LEFT OUTER JOIN match, not 0.
   In aggregation expression Avg("book__rating", default=2.5), default=2.5 have no effect in a missing match.
+- Clickhouse does not support unique constraint and foreignkey constraint. `ForeignKey`, `ManyToManyField` and `OneToOneField` can be used with clickhouse backend, but no database level constraints will be added, so there could be some consistency problems.
+- Clickhouse does not support transaction. If any exception occurs during migrating, then your clickhouse database will be in an untracked state. Any migration should be full tested in test environment before deployed to production environment.
 
 **Requirements:**
 
 - [Python](https://www.python.org/) >= 3.7
 - [Django](https://docs.djangoproject.com/) >= 3.2
 - [clickhouse driver](https://github.com/mymarilyn/clickhouse-driver)
 - [clickhouse pool](https://github.com/ericmccarthy7/clickhouse-pool)
@@ -81,21 +83,17 @@
     },
     'clickhouse': {
         'ENGINE': 'clickhouse_backend.backend',
         'NAME': 'default',
         'HOST': 'localhost',
         'USER': 'DB_USER',
         'PASSWORD': 'DB_PASSWORD',
-        'TEST': {
-            'fake_transaction': True
-        }
     }
 }
 DATABASE_ROUTERS = ['dbrouters.ClickHouseRouter']
-DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'
 ```
 
 ```python
 # dbrouters.py
 from clickhouse_backend.models import ClickhouseModel
 
 def get_subclasses(class_):
@@ -139,16 +137,14 @@
 ```
 
 You should use [database router](https://docs.djangoproject.com/en/4.1/topics/db/multi-db/#automatic-database-routing) to
 automatically route your queries to the right database. In the preceding example, I write a database router which route all
 queries from subclasses of `clickhouse_backend.models.ClickhouseModel` or custom migrations with a `clickhouse` hint key to clickhouse.
 All other queries are routed to the default database (postgresql).
 
-`DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'` is required to working with django migration.
-More details will be covered in [DEFAULT_AUTO_FIELD](https://github.com/jayvynl/django-clickhouse-backend/blob/main/docs/Configurations.md#default_auto_field).
 
 ### Model Definition
 
 Clickhouse backend support django builtin fields and clickhouse specific fields.
 
 Read [fields documentation](https://github.com/jayvynl/django-clickhouse-backend/blob/main/docs/Fields.md) for more.
 
@@ -220,15 +216,15 @@
 ```
 
 this operation will generate migration file under apps/migrations/
 
 then we mirgrate
 
 ```shell
-$ python manage.py migrate
+$ python manage.py migrate --database clickhouse
 ```
 
 for the first time run, this operation will generate django_migrations table with create table sql like this
 
 ```sql
 > show create table django_migrations;
```

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/backend/base.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/backend/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     display_name = "ClickHouse"
     # This dictionary maps Field objects to their associated ClickHouse column
     # types, as strings. Column-type strings can contain format strings; they'll
     # be interpolated against the values of Field.__dict__ before being output.
     # If a column type is set to None, it won't be included in the output.
     data_types = {
         # Django fields.
-        "SmallAutoField": "Int16",
-        "AutoField": "Int32",
+        "SmallAutoField": "Int64",
+        "AutoField": "Int64",
         "BigAutoField": "Int64",
         "IPAddressField": "IPv4",
         "GenericIPAddressField": "IPv6",
         "JSONField": "JSON",
         "BinaryField": "String",
         "CharField": "FixedString(%(max_length)s)",
         "DateField": "Date32",
```

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/backend/client.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/backend/client.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/backend/creation.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/backend/creation.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/backend/features.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/backend/features.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/backend/introspection.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/backend/introspection.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/backend/operations.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/backend/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
         # Django fields.
         "SmallIntegerField": (-32768, 32767),
         "IntegerField": (-2147483648, 2147483647),
         "BigIntegerField": (-9223372036854775808, 9223372036854775807),
         "PositiveBigIntegerField": (0, 18446744073709551615),
         "PositiveSmallIntegerField": (0, 65535),
         "PositiveIntegerField": (0, 4294967295),
-        "SmallAutoField": (-32768, 32767),
-        "AutoField": (-2147483648, 2147483647),
+        "SmallAutoField": (-9223372036854775808, 9223372036854775807),
+        "AutoField": (-9223372036854775808, 9223372036854775807),
         "BigAutoField": (-9223372036854775808, 9223372036854775807),
         # Clickhouse fields.
         "Int8Field": (-1 << 7, -1 ^ (-1 << 7)),
         "Int16Field": (-1 << 15, -1 ^ (-1 << 15)),
         "Int32Field": (-1 << 31, -1 ^ (-1 << 31)),
         "Int64Field": (-1 << 63, -1 ^ (-1 << 63)),
         "Int128Field": (-1 << 127, -1 ^ (-1 << 127)),
```

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/backend/schema.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/backend/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from django.db.backends.base.schema import (
     BaseDatabaseSchemaEditor,
     _related_non_m2m_objects,
 )
 from django.db.backends.ddl_references import (
     Expressions, IndexName, Statement, Table, Columns
 )
+from django.db.models.constraints import CheckConstraint, UniqueConstraint
 from django.db.models.expressions import ExpressionList
 from django.db.models.indexes import IndexExpression
 
 from clickhouse_backend import compat
 from clickhouse_backend.driver.escape import escape_param
 
 
@@ -78,17 +79,20 @@
             # Add the SQL to our big list.
             column_sqls.append("%s %s" % (
                 self.quote_name(field.column),
                 definition,
             ))
             constraints.append(self._column_check_sql(field))
         for constraint in model._meta.constraints:
-            constraints.append(
-                constraint.constraint_sql(model, self)
-            )
+            if isinstance(constraint, CheckConstraint):
+                constraints.append(
+                    constraint.constraint_sql(model, self)
+                )
+        if any(isinstance(c, UniqueConstraint) for c in model._meta.constraints):
+            warnings.warn("Clickhouse does not support unique constraint.")
 
         engine = self._get_engine(model)
         extra_parts = self._model_extra_sql(model, engine)
         sql = self.sql_create_table % {
             "table": self.quote_name(model._meta.db_table),
             "definition": ", ".join(
                 str(constraint)
```

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/driver/__init__.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/driver/client.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/driver/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 import time
 
 from clickhouse_driver import client
 
 from .escape import escape_params
 
-insert_pattern = re.compile(r'\s*insert\s+into', flags=re.IGNORECASE)
+insert_pattern = re.compile(r'\s*insert\s+into.+?values\s*', flags=re.IGNORECASE)
 
 
 class Client(client.Client):
     def __init__(self, *args, **kwargs):
         # https://clickhouse.com/docs/en/sql-reference/data-types/datetime/#usage-remarks
         # The clickhouse-client applies the server time zone by default
         # if a time zone isn’t explicitly set when initializing the data type.
```

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/driver/connection.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/driver/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from clickhouse_driver.dbapi import cursor
 from clickhouse_driver.dbapi import errors
 from clickhouse_pool.pool import ChPoolError
 
 from .escape import escape_params
 from .pool import ClickhousePool
 
-update_pattern = re.compile(r'\s*alter\s+table\s+(.+)\s+update.+where\s+(.+)', flags=re.IGNORECASE)
+update_pattern = re.compile(r'\s*alter\s+table\s+(.+)\s+update.+?where\s+(.+)', flags=re.IGNORECASE)
 
 
 def send_query(self, query, query_id=None, params=None):
     if not self.connected:
         self.connect()
 
     connection.write_varint(connection.ClientPacketTypes.QUERY, self.fout)
```

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/driver/escape.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/driver/escape.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/driver/pool.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/driver/pool.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/idworker/snowflake.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/idworker/snowflake.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/models/base.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/models/base.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/models/engines.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/models/engines.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/__init__.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/models/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/array.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/models/fields/array.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/base.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/models/fields/base.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/integer.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/models/fields/integer.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/json.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/models/fields/json.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/map.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/models/fields/map.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/tuple.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/models/fields/tuple.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/models/functions.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/models/functions.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/models/indexes.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/models/indexes.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/models/query.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/models/query.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/models/sql/compiler.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/models/sql/compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.db.models.fields import BigAutoField
+from django.db.models.fields import AutoFieldMixin
 from django.db.models.sql import compiler
 
 from clickhouse_backend import compat
 from clickhouse_backend.idworker import id_worker
 
 if compat.dj_ge42:
     from django.core.exceptions import FullResultSet
@@ -60,16 +60,16 @@
         # We don't need quote_name_unless_alias() here, since these are all
         # going to be column names (so we can avoid the extra overhead).
         qn = self.connection.ops.quote_name
         opts = self.query.get_meta()
         insert_statement = self.connection.ops.insert_statement()
 
         fields = self.query.fields
-        # For compatible with BigAutoField, add value generated by snowflake algorithm if needed.
-        absent_of_pk = isinstance(opts.pk, BigAutoField) and opts.pk not in fields
+        # Generate value for AutoField when needed.
+        absent_of_pk = isinstance(opts.pk, AutoFieldMixin) and opts.pk not in fields
         if absent_of_pk:
             fields = fields + [opts.pk]
             for obj in self.query.objs:
                 setattr(obj, opts.pk.attname, id_worker.get_id())
 
         result = [
             "%s %s(%s)" % (
```

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/models/sql/query.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/models/sql/query.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/patch/fields.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/patch/fields/json.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/utils.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/utils.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/clickhouse_backend/validators.py` & `django-clickhouse-backend-1.1.0/clickhouse_backend/validators.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.3/django_clickhouse_backend.egg-info/PKG-INFO` & `django-clickhouse-backend-1.1.0/django_clickhouse_backend.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-clickhouse-backend
-Version: 1.0.3
+Version: 1.1.0
 Summary: Django clickHouse database backend.
 Home-page: https://github.com/jayvynl/django-clickhouse-backend
 Author: Lin Zhiwen
 Author-email: zhiwenlin1116@gmail.com
 License: MIT
 Keywords: Django ClickHouse database backend engine driver
 Classifier: Framework :: Django
@@ -53,14 +53,16 @@
 **Notes:**
 
 - Not tested upon all versions of clickhouse-server, clickhouse-server 22.x.y.z or over is suggested.
 - Aggregation functions result in 0 or nan (Not NULL) when data set is empty. max/min/sum/count is 0, avg/STDDEV_POP/VAR_POP is nan.
 - In outer join, clickhouse will set missing columns to empty values (0 for number, empty string for text, unix epoch for date/datatime) instead of NULL. 
   So Count("book") resolve to 1 in a missing LEFT OUTER JOIN match, not 0.
   In aggregation expression Avg("book__rating", default=2.5), default=2.5 have no effect in a missing match.
+- Clickhouse does not support unique constraint and foreignkey constraint. `ForeignKey`, `ManyToManyField` and `OneToOneField` can be used with clickhouse backend, but no database level constraints will be added, so there could be some consistency problems.
+- Clickhouse does not support transaction. If any exception occurs during migrating, then your clickhouse database will be in an untracked state. Any migration should be full tested in test environment before deployed to production environment.
 
 **Requirements:**
 
 - [Python](https://www.python.org/) >= 3.7
 - [Django](https://docs.djangoproject.com/) >= 3.2
 - [clickhouse driver](https://github.com/mymarilyn/clickhouse-driver)
 - [clickhouse pool](https://github.com/ericmccarthy7/clickhouse-pool)
@@ -110,21 +112,17 @@
     },
     'clickhouse': {
         'ENGINE': 'clickhouse_backend.backend',
         'NAME': 'default',
         'HOST': 'localhost',
         'USER': 'DB_USER',
         'PASSWORD': 'DB_PASSWORD',
-        'TEST': {
-            'fake_transaction': True
-        }
     }
 }
 DATABASE_ROUTERS = ['dbrouters.ClickHouseRouter']
-DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'
 ```
 
 ```python
 # dbrouters.py
 from clickhouse_backend.models import ClickhouseModel
 
 def get_subclasses(class_):
@@ -168,16 +166,14 @@
 ```
 
 You should use [database router](https://docs.djangoproject.com/en/4.1/topics/db/multi-db/#automatic-database-routing) to
 automatically route your queries to the right database. In the preceding example, I write a database router which route all
 queries from subclasses of `clickhouse_backend.models.ClickhouseModel` or custom migrations with a `clickhouse` hint key to clickhouse.
 All other queries are routed to the default database (postgresql).
 
-`DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'` is required to working with django migration.
-More details will be covered in [DEFAULT_AUTO_FIELD](https://github.com/jayvynl/django-clickhouse-backend/blob/main/docs/Configurations.md#default_auto_field).
 
 ### Model Definition
 
 Clickhouse backend support django builtin fields and clickhouse specific fields.
 
 Read [fields documentation](https://github.com/jayvynl/django-clickhouse-backend/blob/main/docs/Fields.md) for more.
 
@@ -249,15 +245,15 @@
 ```
 
 this operation will generate migration file under apps/migrations/
 
 then we mirgrate
 
 ```shell
-$ python manage.py migrate
+$ python manage.py migrate --database clickhouse
 ```
 
 for the first time run, this operation will generate django_migrations table with create table sql like this
 
 ```sql
 > show create table django_migrations;
```

### Comparing `django-clickhouse-backend-1.0.3/django_clickhouse_backend.egg-info/SOURCES.txt` & `django-clickhouse-backend-1.1.0/django_clickhouse_backend.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 clickhouse_backend/models/fields/map.py
 clickhouse_backend/models/fields/tuple.py
 clickhouse_backend/models/fields/utils.py
 clickhouse_backend/models/sql/__init__.py
 clickhouse_backend/models/sql/compiler.py
 clickhouse_backend/models/sql/query.py
 clickhouse_backend/patch/__init__.py
-clickhouse_backend/patch/fields.py
 clickhouse_backend/patch/functions.py
+clickhouse_backend/patch/fields/__init__.py
+clickhouse_backend/patch/fields/json.py
 django_clickhouse_backend.egg-info/PKG-INFO
 django_clickhouse_backend.egg-info/SOURCES.txt
 django_clickhouse_backend.egg-info/dependency_links.txt
 django_clickhouse_backend.egg-info/requires.txt
 django_clickhouse_backend.egg-info/top_level.txt
```

### Comparing `django-clickhouse-backend-1.0.3/setup.py` & `django-clickhouse-backend-1.1.0/setup.py`

 * *Files identical despite different names*

