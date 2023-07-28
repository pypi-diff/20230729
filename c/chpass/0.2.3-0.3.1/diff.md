# Comparing `tmp/chpass-0.2.3.tar.gz` & `tmp/chpass-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chpass-0.2.3.tar", last modified: Sun Feb 19 22:05:16 2023, max compression
+gzip compressed data, was "chpass-0.3.1.tar", last modified: Fri Jul 28 22:28:21 2023, max compression
```

## Comparing `chpass-0.2.3.tar` & `chpass-0.3.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:16.490032 chpass-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-02-19 22:05:06.000000 chpass-0.2.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-19 22:05:06.000000 chpass-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-19 22:05:06.000000 chpass-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-02-19 22:05:16.490032 chpass-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-02-19 22:05:06.000000 chpass-0.2.3/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    37620 2023-02-19 22:05:06.000000 chpass-0.2.3/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-19 22:05:06.000000 chpass-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:16.486032 chpass-0.2.3/chpass/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:16.486032 chpass-0.2.3/chpass/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:16.486032 chpass-0.2.3/chpass/core/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/core/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/core/interfaces/file_adapter_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/core/object_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:16.486032 chpass-0.2.3/chpass/dal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/dal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/dal/chrome_db_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:16.486032 chpass-0.2.3/chpass/dal/db_adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/dal/db_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/dal/db_adapters/history_db_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/dal/db_adapters/logins_db_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/dal/db_adapters/top_sites_db_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/dal/db_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:16.486032 chpass-0.2.3/chpass/dal/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/dal/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/dal/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/dal/models/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/dal/models/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/dal/models/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/dal/models/topSite.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/dal/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:16.490032 chpass-0.2.3/chpass/dal/table_adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/dal/table_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/dal/table_adapters/downloads_table_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/dal/table_adapters/history_table_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/dal/table_adapters/logins_table_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/dal/table_adapters/top_sites_table_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:16.490032 chpass-0.2.3/chpass/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/exceptions/chrome_not_installed_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/exceptions/file_adapter_not_supported_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/exceptions/login_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/exceptions/operating_system_not_supported.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/exceptions/user_not_found_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:16.490032 chpass-0.2.3/chpass/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/services/bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/services/chrome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:16.490032 chpass-0.2.3/chpass/services/file_adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/services/file_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/services/file_adapters/csv_file_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/services/file_adapters/json_file_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-02-19 22:05:06.000000 chpass-0.2.3/chpass/services/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:16.486032 chpass-0.2.3/chpass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-02-19 22:05:16.000000 chpass-0.2.3/chpass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-02-19 22:05:16.000000 chpass-0.2.3/chpass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 22:05:16.000000 chpass-0.2.3/chpass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-19 22:05:16.000000 chpass-0.2.3/chpass.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-19 22:05:16.000000 chpass-0.2.3/chpass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-19 22:05:16.000000 chpass-0.2.3/chpass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-19 22:05:16.490032 chpass-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-02-19 22:05:06.000000 chpass-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:16.490032 chpass-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:16.490032 chpass-0.2.3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/integration/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:16.490032 chpass-0.2.3/tests/integration/dal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/integration/dal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/integration/dal/test_db_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/integration/dal/test_downloads_table_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/integration/dal/test_history_table_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/integration/dal/test_logins_table_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/integration/dal/test_top_sites_table_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/integration/test_export_all_data.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/integration/test_export_downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/integration/test_export_history.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/integration/test_export_passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/integration/test_export_profile_picture.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/integration/test_export_top_sites.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/integration/test_import_passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/integration/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/integration/test_profile_picture.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:16.490032 chpass-0.2.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/unit/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-02-19 22:05:06.000000 chpass-0.2.3/tests/unit/test_file_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:21.867574 chpass-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-07-28 22:28:11.000000 chpass-0.3.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 22:28:11.000000 chpass-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 22:28:11.000000 chpass-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 22:28:21.867574 chpass-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-28 22:28:11.000000 chpass-0.3.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    37620 2023-07-28 22:28:11.000000 chpass-0.3.1/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-28 22:28:11.000000 chpass-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:21.855574 chpass-0.3.1/chpass/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:21.855574 chpass-0.3.1/chpass/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:21.855574 chpass-0.3.1/chpass/core/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/core/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/core/interfaces/file_adapter_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/core/object_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:21.859574 chpass-0.3.1/chpass/dal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/dal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/dal/chrome_db_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:21.859574 chpass-0.3.1/chpass/dal/db_adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/dal/db_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/dal/db_adapters/history_db_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/dal/db_adapters/logins_db_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/dal/db_adapters/top_sites_db_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/dal/db_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:21.859574 chpass-0.3.1/chpass/dal/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/dal/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/dal/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/dal/models/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/dal/models/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/dal/models/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/dal/models/topSite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/dal/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:21.859574 chpass-0.3.1/chpass/dal/table_adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/dal/table_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/dal/table_adapters/downloads_table_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/dal/table_adapters/history_table_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/dal/table_adapters/logins_table_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/dal/table_adapters/top_sites_table_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:21.863574 chpass-0.3.1/chpass/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/exceptions/chrome_not_installed_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/exceptions/file_adapter_not_supported_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/exceptions/login_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/exceptions/operating_system_not_supported.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/exceptions/user_not_found_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:21.863574 chpass-0.3.1/chpass/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/services/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/services/chrome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:21.863574 chpass-0.3.1/chpass/services/file_adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/services/file_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/services/file_adapters/csv_file_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/services/file_adapters/json_file_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-28 22:28:11.000000 chpass-0.3.1/chpass/services/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:21.855574 chpass-0.3.1/chpass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 22:28:21.000000 chpass-0.3.1/chpass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-28 22:28:21.000000 chpass-0.3.1/chpass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:28:21.000000 chpass-0.3.1/chpass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-28 22:28:21.000000 chpass-0.3.1/chpass.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-28 22:28:21.000000 chpass-0.3.1/chpass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 22:28:21.000000 chpass-0.3.1/chpass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 22:28:21.867574 chpass-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-28 22:28:11.000000 chpass-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:21.863574 chpass-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:21.867574 chpass-0.3.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/integration/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:21.867574 chpass-0.3.1/tests/integration/dal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/integration/dal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/integration/dal/test_db_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/integration/dal/test_downloads_table_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/integration/dal/test_history_table_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/integration/dal/test_logins_table_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/integration/dal/test_top_sites_table_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/integration/test_export_all_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/integration/test_export_downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/integration/test_export_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/integration/test_export_passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/integration/test_export_profile_picture.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/integration/test_export_top_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/integration/test_import_passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/integration/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/integration/test_profile_picture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:21.867574 chpass-0.3.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/unit/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-28 22:28:11.000000 chpass-0.3.1/tests/unit/test_file_adapter.py
```

### Comparing `chpass-0.2.3/.pylintrc` & `chpass-0.3.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/LICENSE` & `chpass-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/PKG-INFO` & `chpass-0.3.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chpass
-Version: 0.2.3
+Version: 0.3.1
 Summary: Gather information from chrome
 Home-page: https://github.com/bengabay11/chpass
 Author: Ben Gabay
 Author-email: ben.gabay38@gmail.com
 License: License :: OSI Approved :: MIT License
 Keywords: chrome passwords
 Classifier: Programming Language :: Python :: 3
@@ -16,16 +16,15 @@
 
 # chpass
 
 Gather information from Chrome 🔑
 
 [![Unit Tests](https://github.com/bengabay11/chpass/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/bengabay11/chpass/actions/workflows/unit-tests.yml)
 [![Integration Tests](https://github.com/bengabay11/chpass/actions/workflows/integration-tests.yml/badge.svg)](https://github.com/bengabay11/chpass/actions/workflows/integration-tests.yml)
-[![python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue)](https://pypi.org/project/chpass/)
-[![platform](https://img.shields.io/badge/platform-windows%20%7C%20ubuntu%20%7C%20macos-lightgrey)](https://pypi.org/project/chpass/)
+[![python](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/chpass/)
 
 ## Features
 
 - import/export passwords
 - history
 - google account profile picture
 - downloads
```

### Comparing `chpass-0.2.3/Pipfile` & `chpass-0.3.1/Pipfile`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 pylint = ">=2.16.2"
 coverage = ">=7.1.0"
 pytest-cov = ">=4.0.0"
 
 [packages]
 sqlalchemy = ">=2.0.4"
 pattern-singleton = ">=1.2.0"
-pandas = ">=1.5.3"
+pandas = ">=2.0.3"
 
 [scripts]
 lint = "pylint --rcfile=.pylintrc chpass"
 unit-test = "pytest tests/unit"
 unit-test-cov = "pytest --cov=chpass tests/unit"
 integ-test = "pytest tests/integration"
 integ-test-cov = "pytest --cov=chpass tests/integration"
```

### Comparing `chpass-0.2.3/Pipfile.lock` & `chpass-0.3.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/README.md` & `chpass-0.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # chpass
 
 Gather information from Chrome 🔑
 
 [![Unit Tests](https://github.com/bengabay11/chpass/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/bengabay11/chpass/actions/workflows/unit-tests.yml)
 [![Integration Tests](https://github.com/bengabay11/chpass/actions/workflows/integration-tests.yml/badge.svg)](https://github.com/bengabay11/chpass/actions/workflows/integration-tests.yml)
-[![python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue)](https://pypi.org/project/chpass/)
-[![platform](https://img.shields.io/badge/platform-windows%20%7C%20ubuntu%20%7C%20macos-lightgrey)](https://pypi.org/project/chpass/)
+[![python](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/chpass/)
 
 ## Features
 
 - import/export passwords
 - history
 - google account profile picture
 - downloads
```

### Comparing `chpass-0.2.3/chpass/__init__.py` & `chpass-0.3.1/chpass/__init__.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/chpass/__main__.py` & `chpass-0.3.1/chpass/__main__.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/chpass/cli.py` & `chpass-0.3.1/chpass/cli.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/chpass/config.py` & `chpass-0.3.1/chpass/config.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/chpass/dal/chrome_db_adapter.py` & `chpass-0.3.1/chpass/dal/chrome_db_adapter.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/chpass/dal/db_adapters/history_db_adapter.py` & `chpass-0.3.1/chpass/dal/db_adapters/history_db_adapter.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/chpass/dal/db_adapters/logins_db_adapter.py` & `chpass-0.3.1/chpass/dal/db_adapters/logins_db_adapter.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/chpass/dal/db_adapters/top_sites_db_adapter.py` & `chpass-0.3.1/chpass/dal/db_adapters/top_sites_db_adapter.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/chpass/dal/db_connection.py` & `chpass-0.3.1/chpass/dal/db_connection.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/chpass/dal/models/download.py` & `chpass-0.3.1/chpass/dal/models/download.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/chpass/dal/models/login.py` & `chpass-0.3.1/chpass/dal/models/login.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/chpass/dal/table_adapters/logins_table_adapter.py` & `chpass-0.3.1/chpass/dal/table_adapters/logins_table_adapter.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/chpass/exceptions/file_adapter_not_supported_exception.py` & `chpass-0.3.1/chpass/exceptions/file_adapter_not_supported_exception.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/chpass/services/bytes.py` & `chpass-0.3.1/chpass/services/bytes.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/chpass/services/chrome.py` & `chpass-0.3.1/chpass/services/chrome.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/chpass/services/file_adapters/csv_file_adapter.py` & `chpass-0.3.1/chpass/services/file_adapters/csv_file_adapter.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/chpass/services/file_adapters/json_file_adapter.py` & `chpass-0.3.1/chpass/services/file_adapters/json_file_adapter.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/chpass/services/path.py` & `chpass-0.3.1/chpass/services/path.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/chpass.egg-info/PKG-INFO` & `chpass-0.3.1/chpass.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chpass
-Version: 0.2.3
+Version: 0.3.1
 Summary: Gather information from chrome
 Home-page: https://github.com/bengabay11/chpass
 Author: Ben Gabay
 Author-email: ben.gabay38@gmail.com
 License: License :: OSI Approved :: MIT License
 Keywords: chrome passwords
 Classifier: Programming Language :: Python :: 3
@@ -16,16 +16,15 @@
 
 # chpass
 
 Gather information from Chrome 🔑
 
 [![Unit Tests](https://github.com/bengabay11/chpass/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/bengabay11/chpass/actions/workflows/unit-tests.yml)
 [![Integration Tests](https://github.com/bengabay11/chpass/actions/workflows/integration-tests.yml/badge.svg)](https://github.com/bengabay11/chpass/actions/workflows/integration-tests.yml)
-[![python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue)](https://pypi.org/project/chpass/)
-[![platform](https://img.shields.io/badge/platform-windows%20%7C%20ubuntu%20%7C%20macos-lightgrey)](https://pypi.org/project/chpass/)
+[![python](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/chpass/)
 
 ## Features
 
 - import/export passwords
 - history
 - google account profile picture
 - downloads
```

### Comparing `chpass-0.2.3/chpass.egg-info/SOURCES.txt` & `chpass-0.3.1/chpass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/setup.py` & `chpass-0.3.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="chpass",
-    version="0.2.3",
+    version="0.3.1",
     author="Ben Gabay",
     author_email="ben.gabay38@gmail.com",
     license="License :: OSI Approved :: MIT License",
     description="Gather information from chrome",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bengabay11/chpass",
     packages=setuptools.find_packages(),
     install_requires=[
-        "sqlalchemy==1.3.18",
-        "pandas==1.3.1",
-        "pattern_singleton==1.2.0"
+        "sqlalchemy==2.0.4",
+        "pattern_singleton==1.2.0",
+        "pandas==2.0.3"
     ],
     python_requires=">=3",
     entry_points={
         'console_scripts': ['chpass = chpass.__init__:main'],
     },
     keywords="chrome passwords",
     classifiers=[
```

### Comparing `chpass-0.2.3/tests/integration/conftest.py` & `chpass-0.3.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/tests/integration/dal/test_db_connection.py` & `chpass-0.3.1/tests/integration/dal/test_db_connection.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/tests/integration/dal/test_logins_table_adapter.py` & `chpass-0.3.1/tests/integration/dal/test_logins_table_adapter.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/tests/integration/test_export_all_data.py` & `chpass-0.3.1/tests/integration/test_export_all_data.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/tests/integration/test_import_passwords.py` & `chpass-0.3.1/tests/integration/test_import_passwords.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/tests/integration/test_path.py` & `chpass-0.3.1/tests/integration/test_path.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/tests/integration/test_profile_picture.py` & `chpass-0.3.1/tests/integration/test_profile_picture.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/tests/unit/test_cli.py` & `chpass-0.3.1/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `chpass-0.2.3/tests/unit/test_file_adapter.py` & `chpass-0.3.1/tests/unit/test_file_adapter.py`

 * *Files identical despite different names*

