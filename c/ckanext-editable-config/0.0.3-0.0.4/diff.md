# Comparing `tmp/ckanext-editable-config-0.0.3.tar.gz` & `tmp/ckanext-editable-config-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-editable-config-0.0.3.tar", last modified: Thu Jul 13 11:05:40 2023, max compression
+gzip compressed data, was "ckanext-editable-config-0.0.4.tar", last modified: Fri Jul 28 22:50:04 2023, max compression
```

## Comparing `ckanext-editable-config-0.0.3.tar` & `ckanext-editable-config-0.0.4.tar`

### file list

```diff
@@ -1,60 +1,67 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.3/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      215 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.3/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4933 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4345 2023-06-19 21:13:09.000000 ckanext-editable-config-0.0.3/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.356833 ckanext-editable-config-0.0.3/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      202 2023-06-18 20:14:29.000000 ckanext-editable-config-0.0.3/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.356833 ckanext-editable-config-0.0.3/ckanext/editable_config/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext/editable_config/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      167 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/assets/script.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/assets/style.css
--rw-r--r--   0 sergey    (1000) sergey    (1000)      359 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      451 2023-06-19 12:53:41.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      200 2023-07-13 11:05:24.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/helpers.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext/editable_config/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:15:55.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6037 2023-07-07 13:06:54.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1589 2023-06-19 10:13:19.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2719 2023-06-19 20:17:49.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/logic/schema.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:16:21.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/logic/validators.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.356833 ckanext-editable-config-0.0.3/ckanext/editable_config/migration/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext/editable_config/migration/editable_config/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1834 2023-06-18 15:19:17.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/migration/editable_config/alembic.ini
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2148 2023-06-18 20:14:29.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/migration/editable_config/env.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2023-06-18 15:19:17.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/migration/editable_config/script.py.mako
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext/editable_config/migration/editable_config/versions/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      655 2023-06-18 19:08:06.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/migration/editable_config/versions/a8d116986c3f_create_editable_config_table.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext/editable_config/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       49 2023-06-18 19:08:06.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1859 2023-06-19 13:13:22.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/model/option.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4170 2023-07-13 11:05:24.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2605 2023-06-19 20:17:42.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/shared.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.356833 ckanext-editable-config-0.0.3/ckanext/editable_config/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext/editable_config/templates/admin/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      399 2023-07-13 11:05:24.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/templates/admin/base.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1254 2023-06-19 20:17:49.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 20:35:03.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4430 2023-06-19 20:17:49.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/logic/test_action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      750 2023-06-19 12:49:49.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/logic/test_schema.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 21:22:56.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3473 2023-06-19 20:17:49.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/model/test_option.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1609 2023-06-19 20:17:42.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/test_fixtures.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 19:08:32.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2911 2023-06-19 20:17:47.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/test_shared.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext_editable_config.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4933 2023-07-13 11:05:40.000000 ckanext-editable-config-0.0.3/ckanext_editable_config.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1788 2023-07-13 11:05:40.000000 ckanext-editable-config-0.0.3/ckanext_editable_config.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-07-13 11:05:40.000000 ckanext-editable-config-0.0.3/ckanext_editable_config.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2023-07-13 11:05:40.000000 ckanext-editable-config-0.0.3/ckanext_editable_config.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-13 11:05:40.000000 ckanext-editable-config-0.0.3/ckanext_editable_config.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-13 11:05:40.000000 ckanext-editable-config-0.0.3/ckanext_editable_config.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4324 2023-06-18 20:58:41.000000 ckanext-editable-config-0.0.3/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.3/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1691 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      505 2023-06-18 19:08:08.000000 ckanext-editable-config-0.0.3/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.4/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      215 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.4/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12795 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12207 2023-07-28 22:11:05.000000 ckanext-editable-config-0.0.4/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.963428 ckanext-editable-config-0.0.4/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      202 2023-06-18 20:14:29.000000 ckanext-editable-config-0.0.4/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/assets/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/assets/js/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      418 2023-07-28 22:08:36.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/assets/js/editable-config-toggle-field.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      167 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/assets/script.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/assets/style.css
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      356 2023-07-28 21:54:04.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1211 2023-07-28 16:17:04.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      636 2023-07-28 22:26:11.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/helpers.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:15:55.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6695 2023-07-28 22:10:23.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/logic/action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1782 2023-07-25 22:20:05.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2719 2023-06-19 20:17:49.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/logic/schema.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:16:21.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/logic/validators.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.963428 ckanext-editable-config-0.0.4/ckanext/editable_config/migration/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/migration/editable_config/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1834 2023-06-18 15:19:17.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/migration/editable_config/alembic.ini
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2148 2023-06-18 20:14:29.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/migration/editable_config/env.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2023-06-18 15:19:17.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/migration/editable_config/script.py.mako
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/migration/editable_config/versions/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      655 2023-06-18 19:08:06.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/migration/editable_config/versions/a8d116986c3f_create_editable_config_table.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       49 2023-06-18 19:08:06.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2492 2023-07-25 21:26:13.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/model/option.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4544 2023-07-28 21:56:38.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4130 2023-07-28 22:49:10.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/shared.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.963428 ckanext-editable-config-0.0.4/ckanext/editable_config/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/templates/admin/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      680 2023-07-28 16:20:12.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/templates/admin/base.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/templates/editable_config/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2307 2023-07-28 22:25:24.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/templates/editable_config/config.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/templates/editable_config/snippets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1033 2023-07-28 22:23:30.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/templates/editable_config/snippets/field.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1528 2023-07-25 22:45:15.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 20:35:03.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5025 2023-07-25 23:02:01.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/logic/test_action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      750 2023-06-19 12:49:49.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/logic/test_schema.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 21:22:56.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3473 2023-06-19 20:17:49.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/model/test_option.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1609 2023-06-19 20:17:42.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/test_fixtures.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 19:08:32.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3444 2023-07-25 22:45:46.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/test_shared.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1830 2023-07-28 22:26:11.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext_editable_config.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12795 2023-07-28 22:50:04.000000 ckanext-editable-config-0.0.4/ckanext_editable_config.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2019 2023-07-28 22:50:04.000000 ckanext-editable-config-0.0.4/ckanext_editable_config.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-07-28 22:50:04.000000 ckanext-editable-config-0.0.4/ckanext_editable_config.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2023-07-28 22:50:04.000000 ckanext-editable-config-0.0.4/ckanext_editable_config.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-28 22:50:04.000000 ckanext-editable-config-0.0.4/ckanext_editable_config.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-28 22:50:04.000000 ckanext-editable-config-0.0.4/ckanext_editable_config.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4324 2023-06-18 20:58:41.000000 ckanext-editable-config-0.0.4/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.4/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1691 2023-07-28 22:50:04.983430 ckanext-editable-config-0.0.4/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      505 2023-06-18 19:08:08.000000 ckanext-editable-config-0.0.4/setup.py
```

### Comparing `ckanext-editable-config-0.0.3/LICENSE` & `ckanext-editable-config-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.3/ckanext/editable_config/logic/action.py` & `ckanext-editable-config-0.0.4/ckanext/editable_config/logic/action.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,19 +21,46 @@
 class UpdateResult(TypedDict):
     change: dict[str, shared.OptionDict]
     revert: dict[str, shared.OptionDict]
     reset: dict[str, shared.OptionDict]
 
 
 @tk.side_effect_free
+def editable_config_last_check(
+    context: types.Context,
+    data_dict: dict[str, Any],
+) -> dict[str, Any]:
+    """Date and time of the last change detection cycle.
+
+    Returns:
+      last_check(str): ISO datetime
+
+    """
+    tk.check_access("editable_config_last_check", context, data_dict)
+
+    last_check = shared.apply_config_overrides.last_check
+    if not last_check:
+        raise tk.ValidationError({"last_check": ["Change detection disabled"]})
+    return {"last_check": last_check.isoformat()}
+
+
+@tk.side_effect_free
 @validate(schema.editable_config_list)
 def editable_config_list(
     context: types.Context,
     data_dict: dict[str, Any],
 ) -> dict[str, Any]:
+    """All editable config options. Every modified option includes dictionary
+    containing override details.
+
+    Returns:
+      editable option names(`dict[str, Any]`): dictionary with current
+      value and optional modification details
+
+    """
     tk.check_access("editable_config_list", context, data_dict)
 
     result: dict[str, Any] = {}
     for key in cd.iter_options(pattern=data_dict["pattern"]):
         option = cd[key]
         if not option.has_flag(Flag.editable):
             continue
@@ -44,15 +71,14 @@
             "value": shared.value_as_string(skey, tk.config[skey]),
             "option": opt.as_dict(context) if (opt := Option.get(skey)) else None,
         }
 
     return result
 
 
-@tk.side_effect_free
 @validate(schema.editable_config_update)
 def editable_config_update(
     context: types.Context,
     data_dict: dict[str, Any],
 ) -> UpdateResult:
     tk.check_access("editable_config_update", context, data_dict)
 
@@ -77,15 +103,14 @@
 
     if data_dict["apply"]:
         shared.apply_config_overrides(removed_keys=result["reset"])
 
     return result
 
 
-@tk.side_effect_free
 @validate(schema.editable_config_change)
 def editable_config_change(
     context: types.Context,
     data_dict: dict[str, Any],
 ) -> dict[str, shared.OptionDict]:
     tk.check_access("editable_config_change", context, data_dict)
     sess = context["session"]
@@ -115,15 +140,14 @@
     _, errors = cd.validate(CKANConfig(tk.config, **{key: value}))
     if errors:
         raise tk.ValidationError(errors)
 
     return Option.set(key, value)
 
 
-@tk.side_effect_free
 @validate(schema.editable_config_option_save)
 def editable_config_option_save(
     context: types.Context,
     data_dict: dict[str, Any],
 ) -> shared.OptionDict:
     tk.check_access("editable_config_option_save", context, data_dict)
     sess = context["session"]
@@ -139,15 +163,14 @@
 
     if data_dict["apply"]:
         shared.apply_config_overrides()
 
     return option.as_dict(tk.fresh_context(context))
 
 
-@tk.side_effect_free
 @validate(schema.editable_config_revert)
 def editable_config_revert(
     context: types.Context,
     data_dict: dict[str, Any],
 ) -> dict[str, shared.OptionDict]:
     tk.check_access("editable_config_revert", context, data_dict)
 
@@ -174,15 +197,14 @@
 
     if data_dict["apply"]:
         shared.apply_config_overrides()
 
     return result
 
 
-@tk.side_effect_free
 @validate(schema.editable_config_reset)
 def editable_config_reset(
     context: types.Context,
     data_dict: dict[str, Any],
 ) -> dict[str, shared.OptionDict]:
     tk.check_access("editable_config_reset", context, data_dict)
     sess = context["session"]
@@ -204,15 +226,14 @@
 
     if data_dict["apply"]:
         shared.apply_config_overrides(removed_keys=result)
 
     return result
 
 
-@tk.side_effect_free
 @validate(schema.editable_config_apply)
 def editable_config_apply(
     context: types.Context,
     data_dict: dict[str, Any],
 ) -> dict[str, Any]:
     tk.check_access("editable_config_apply", context, data_dict)
     count = shared.apply_config_overrides(removed_keys=data_dict["removed_keys"])
```

### Comparing `ckanext-editable-config-0.0.3/ckanext/editable_config/logic/auth.py` & `ckanext-editable-config-0.0.4/ckanext/editable_config/logic/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 def editable_config_access(
     context: types.Context,
     data_dict: dict[str, Any],
 ) -> types.AuthResult:
     return authz.is_authorized("sysadmin", context, data_dict)
 
 
+def editable_config_last_check(
+    context: types.Context,
+    data_dict: dict[str, Any],
+) -> types.AuthResult:
+    return authz.is_authorized("editable_config_access", context, data_dict)
+
+
 def editable_config_list(
     context: types.Context,
     data_dict: dict[str, Any],
 ) -> types.AuthResult:
     return authz.is_authorized("editable_config_access", context, data_dict)
```

### Comparing `ckanext-editable-config-0.0.3/ckanext/editable_config/logic/schema.py` & `ckanext-editable-config-0.0.4/ckanext/editable_config/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.3/ckanext/editable_config/migration/editable_config/alembic.ini` & `ckanext-editable-config-0.0.4/ckanext/editable_config/migration/editable_config/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.3/ckanext/editable_config/migration/editable_config/env.py` & `ckanext-editable-config-0.0.4/ckanext/editable_config/migration/editable_config/env.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.3/ckanext/editable_config/migration/editable_config/versions/a8d116986c3f_create_editable_config_table.py` & `ckanext-editable-config-0.0.4/ckanext/editable_config/migration/editable_config/versions/a8d116986c3f_create_editable_config_table.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.3/ckanext/editable_config/model/option.py` & `ckanext-editable-config-0.0.4/ckanext/editable_config/model/option.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,48 +19,65 @@
     key = sa.Column(sa.Text, primary_key=True)
     value = sa.Column(sa.Text, nullable=False)
     updated_at = sa.Column(sa.DateTime, nullable=False)
     prev_value = sa.Column(sa.Text, nullable=False)
 
     @classmethod
     def get(cls, key: str) -> Self | None:
+        """Search for option."""
         return cast(
             Self,
             model.Session.get(cls, key),
         )
 
     @classmethod
     def set(cls, key: str, value: Any) -> Self:
+        """Create/update an option."""
         option: Self
         safe_value = shared.value_as_string(key, value)
 
         if option := cls.get(key):
             option.value = safe_value
         else:
             option = cls(key=key, value=safe_value)
 
         option.prev_value = shared.value_as_string(key, tk.config[key])
         option.touch()
 
         return option
 
     def touch(self):
+        """Update modification date of the option."""
         self.updated_at = datetime.utcnow()
 
     def revert(self):
+        """Swap current and previous values of the option."""
         self.value, self.prev_value = self.prev_value, self.value
         self.touch()
 
     def as_dict(self, context: types.Context) -> shared.OptionDict:
+        """Convert option object into form appropriate for API response."""
         return cast(shared.OptionDict, table_dictize(self, context))
 
     @classmethod
     def is_updated_since(cls, last_update: datetime | None) -> bool:
-        return model.Session.query(cls.updated_since(last_update).exists()).scalar()
+        """Check if there are any registered config overrides.
+
+        If optional `last_update` is provided, check for updates that were made
+        after this moment.
+        """
+        q: Any = cls.updated_since(last_update).exists()
+        return model.Session.query(q).scalar()
 
     @classmethod
     def updated_since(cls, last_update: datetime | None) -> types.Query[Self]:
+        """All overriden config options.
+
+        If optional `last_update` is provided, return only options that were
+        updated after this moment.
+
+        """
         q = model.Session.query(cls)
         if last_update:
             q = q.filter(cls.updated_at > last_update)
 
         return q
```

### Comparing `ckanext-editable-config-0.0.3/ckanext/editable_config/plugin.py` & `ckanext-editable-config-0.0.4/ckanext/editable_config/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,46 +19,58 @@
 log = logging.getLogger(__name__)
 ENVVAR_DISABLE = "CKANEXT_EDITABLE_CONFIG_DISABLE"
 
 
 @tk.blanket.config_declarations
 @tk.blanket.actions
 @tk.blanket.helpers
+@tk.blanket.blueprints
 @tk.blanket.auth_functions
 class EditableConfigPlugin(plugins.SingletonPlugin):
     plugins.implements(plugins.IConfigurer, inherit=True)
     plugins.implements(plugins.IConfigurable, inherit=True)
     plugins.implements(plugins.IMiddleware, inherit=True)
-    plugins.implements(plugins.IConfigDeclaration, inherit=True)
 
     _editable_config_enabled: bool = True
 
     # IMiddleware
     def make_middleware(self, app: types.CKANApp, config: CKANConfig) -> types.CKANApp:
         if self._editable_config_enabled:
             app.before_request(self._apply_overrides)
+
         return app
 
     def _apply_overrides(self):
         shared.apply_config_overrides()
 
     # IConfigurer
     def update_config(self, config_: CKANConfig):
         tk.add_template_directory(config_, "templates")
+        tk.add_resource("assets", "editable_config")
 
         self._update_editable_flag(config.extra_editable(), True)
         self._update_editable_flag(config.blacklist(), False)
 
         if whitelist := config.whitelist():
             for key in cd.iter_options():
                 if key in whitelist:
                     continue
 
                 cd[key].flags &= ~Flag.editable
 
+        self._add_validators(config.additional_validators())
+
+    def _add_validators(self, validators: dict[str, str]):
+        for key, names in validators.items():
+            if key not in cd:
+                log.warning("%s is not declared", key)
+                continue
+            option = cd[Key.from_string(key)]
+            option.append_validators(names)
+
     def _update_editable_flag(self, keys: list[str], enable: bool):
         for key in keys:
             if key not in cd:
                 log.warning("%s is not declared", key)
                 continue
             option = cd[Key.from_string(key)]
             if enable:
@@ -70,14 +82,15 @@
     def configure(self, config_: CKANConfig):
         if tk.asbool(os.getenv(ENVVAR_DISABLE)):
             self._editable_config_enabled = False
             log.info(
                 "editable_config disabled because of environemnt variable: %s",
                 ENVVAR_DISABLE,
             )
+            return
 
         inspector = sa.inspect(model.meta.engine)
         self._editable_config_enabled = inspector.has_table("editable_config_option")
         if not self._editable_config_enabled:
             log.critical(
                 "editable_config disabled because of missing migration: %s",
                 "ckan db upgrade -p editable_config",
@@ -87,16 +100,17 @@
         stmt = sa.select(model.SystemInfo.key)
         legacy_modified: Iterable[str] = model.Session.scalars(stmt)
         editable = {
             str(op) for op in cd.iter_options() if cd[op].has_flag(Flag.editable)
         }
 
         if problems := (set(legacy_modified) & editable):
-            if tk.config["ckanext.editable_config.convert_core_overrides"]:
+            if config.convert_core_overrides():
                 self._convert_core_overrides(problems)
+
             else:
                 log.warning(
                     "Modification via core AdminUI will cause undefined behavior: %s",
                     problems,
                 )
 
         shared.apply_config_overrides()
@@ -106,23 +120,22 @@
         try:
             change = tk.get_action("editable_config_change")
         except KeyError:
             log.debug("Do not convert core overrides because plugin is not loaded yet")
             return
 
         q = model.Session.query(model.SystemInfo).filter(
-            model.SystemInfo.key.in_(names)
+            model.SystemInfo.key.in_(names),
         )
-        options = {
-            op.key: op.value
-            for op in
-            q
-        }
+        options = {op.key: op.value for op in q}
 
         log.debug("Convert core overrides into editable config: %s", options)
-        change({"ignore_auth": True}, {
-            "apply": False,
-            "options": options,
-        })
+        change(
+            {"ignore_auth": True},
+            {
+                "apply": False,
+                "options": options,
+            },
+        )
 
         q.delete()
         model.Session.commit()
```

### Comparing `ckanext-editable-config-0.0.3/ckanext/editable_config/tests/conftest.py` & `ckanext-editable-config-0.0.4/ckanext/editable_config/tests/conftest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 from __future__ import annotations
 
 import contextlib
+from typing import Any
 
 import pytest
 from pytest_factoryboy import register
 
 from ckan import model
 from ckan.tests import factories
 from ckan.tests.helpers import call_action
 
 from ckanext.editable_config.model import Option
+from ckanext.editable_config.shared import apply_config_overrides
+
+
+@pytest.fixture(autouse=True)
+def reset_last_check():
+    """Remove freezetime dates in future from config_overrides."""
+    apply_config_overrides._last_check = None
 
 
 @pytest.fixture(scope="session")
 def reset_db_once(reset_db, migrate_db_for):
     reset_db()
     migrate_db_for("editable_config")
 
@@ -32,15 +40,15 @@
 
     key = None
     value = None
 
     @classmethod
     @contextlib.contextmanager
     def autoclean(cls, *args, **kwargs):
-        option = cls(*args, **kwargs)
+        option: dict[str, Any] = cls(*args, **kwargs)
         try:
             yield option
         finally:
             call_action("editable_config_reset", keys=[option["key"]])
 
 
 @pytest.fixture()
```

### Comparing `ckanext-editable-config-0.0.3/ckanext/editable_config/tests/logic/test_action.py` & `ckanext-editable-config-0.0.4/ckanext/editable_config/tests/logic/test_action.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,14 +76,31 @@
 
     def test_valid(self, faker, ckan_config):
         """It works with valid option."""
         title = faker.sentence()
         call_action("editable_config_change", options={"ckan.site_title": title})
         assert ckan_config["ckan.site_title"] == title
 
+    @pytest.mark.ckan_config(config.EXTRA_EDITABLE, "ckan.datasets_per_page")
+    @pytest.mark.ckan_config(
+        config.ADDITIONAL_VALIDATORS,
+        {"ckan.datasets_per_page": "is_positive_integer"},
+    )
+    def test_additional_validators(self):
+        """Options are validated"""
+        with pytest.raises(tk.ValidationError):
+            call_action(
+                "editable_config_change",
+                options={"ckan.datasets_per_page": -1},
+            )
+        call_action(
+            "editable_config_change",
+            options={"ckan.datasets_per_page": 1},
+        )
+
 
 @pytest.mark.usefixtures("with_plugins", "non_clean_db", "with_autoclean")
 class TestRevert:
     def test_revert_missing(self):
         with pytest.raises(tk.ObjectNotFound):
             call_action("editable_config_revert", keys=["ckan.site_title"])
```

### Comparing `ckanext-editable-config-0.0.3/ckanext/editable_config/tests/logic/test_schema.py` & `ckanext-editable-config-0.0.4/ckanext/editable_config/tests/logic/test_schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.3/ckanext/editable_config/tests/model/test_option.py` & `ckanext-editable-config-0.0.4/ckanext/editable_config/tests/model/test_option.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.3/ckanext/editable_config/tests/test_fixtures.py` & `ckanext-editable-config-0.0.4/ckanext/editable_config/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.3/ckanext/editable_config/tests/test_shared.py` & `ckanext-editable-config-0.0.4/ckanext/editable_config/tests/test_shared.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import timedelta
 from typing import get_type_hints
 
 import pytest
 
 from ckan.tests.helpers import call_action
 
-from ckanext.editable_config import shared
+from ckanext.editable_config import config, shared
 from ckanext.editable_config.model import Option
 
 
 def test_optional_dict_is_up_to_date(faker):
     option = Option.set("ckan.site_title", faker.sentence()).as_dict({})
     assert option.keys() == get_type_hints(shared.OptionDict).keys()
 
@@ -22,23 +22,38 @@
     assert shared.value_as_string("ckan.plugins", ["hello", "world"]) == "hello world"
 
 
 @pytest.mark.usefixtures("with_plugins", "non_clean_db")
 class TestUpdater:
     def test_apply_new_updates(self, faker, ckan_config, freezer, autoclean_option):
         """New updates are applied."""
-        freezer.move_to(timedelta(days=1))
+        freezer.move_to(timedelta(seconds=1))
         key = autoclean_option["key"]
         value = faker.sentence()
 
         call_action("editable_config_change", options={key: value}, apply=False)
         assert ckan_config[key] != value
         assert shared.apply_config_overrides() == 1
         assert ckan_config[key] == value
 
+    @pytest.mark.ckan_config(config.CHARGE_TIMEOUT, 10)
+    def test_charge_timeout(self, faker, freezer, autoclean_option):
+        """New updates are applied."""
+        freezer.move_to(timedelta(seconds=5))
+
+        call_action(
+            "editable_config_change",
+            options={autoclean_option["key"]: faker.sentence()},
+            apply=False,
+        )
+        assert shared.apply_config_overrides() == 0
+
+        freezer.move_to(timedelta(seconds=6))
+        assert shared.apply_config_overrides() == 1
+
     def test_apply_old_updates(self, faker, ckan_config, freezer, autoclean_option):
         """Old updates are ignored."""
         freezer.move_to(timedelta(days=-1))
         key = autoclean_option["key"]
         value = faker.sentence()
         call_action("editable_config_change", options={key: value}, apply=False)
         assert shared.apply_config_overrides() == 0
```

### Comparing `ckanext-editable-config-0.0.3/ckanext_editable_config.egg-info/SOURCES.txt` & `ckanext-editable-config-0.0.4/ckanext_editable_config.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,29 +7,33 @@
 setup.py
 ckanext/__init__.py
 ckanext/editable_config/__init__.py
 ckanext/editable_config/config.py
 ckanext/editable_config/helpers.py
 ckanext/editable_config/plugin.py
 ckanext/editable_config/shared.py
+ckanext/editable_config/views.py
 ckanext/editable_config/assets/script.js
 ckanext/editable_config/assets/style.css
 ckanext/editable_config/assets/webassets.yml
+ckanext/editable_config/assets/js/editable-config-toggle-field.js
 ckanext/editable_config/logic/__init__.py
 ckanext/editable_config/logic/action.py
 ckanext/editable_config/logic/auth.py
 ckanext/editable_config/logic/schema.py
 ckanext/editable_config/logic/validators.py
 ckanext/editable_config/migration/editable_config/alembic.ini
 ckanext/editable_config/migration/editable_config/env.py
 ckanext/editable_config/migration/editable_config/script.py.mako
 ckanext/editable_config/migration/editable_config/versions/a8d116986c3f_create_editable_config_table.py
 ckanext/editable_config/model/__init__.py
 ckanext/editable_config/model/option.py
 ckanext/editable_config/templates/admin/base.html
+ckanext/editable_config/templates/editable_config/config.html
+ckanext/editable_config/templates/editable_config/snippets/field.html
 ckanext/editable_config/tests/__init__.py
 ckanext/editable_config/tests/conftest.py
 ckanext/editable_config/tests/test_fixtures.py
 ckanext/editable_config/tests/test_plugin.py
 ckanext/editable_config/tests/test_shared.py
 ckanext/editable_config/tests/logic/__init__.py
 ckanext/editable_config/tests/logic/test_action.py
```

### Comparing `ckanext-editable-config-0.0.3/pyproject.toml` & `ckanext-editable-config-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.3/setup.cfg` & `ckanext-editable-config-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-editable-config
-version = 0.0.3
+version = 0.0.4
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-editable-config
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```

