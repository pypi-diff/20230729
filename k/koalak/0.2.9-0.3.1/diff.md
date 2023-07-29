# Comparing `tmp/koalak-0.2.9.tar.gz` & `tmp/koalak-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koalak-0.2.9.tar", last modified: Sun Feb  6 20:26:21 2022, max compression
+gzip compressed data, was "koalak-0.3.1.tar", last modified: Sat Jul 29 20:02:18 2023, max compression
```

## Comparing `koalak-0.2.9.tar` & `koalak-0.3.1.tar`

### file list

```diff
@@ -1,76 +1,161 @@
-drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2022-02-06 20:26:20.997206 koalak-0.2.9/
--rw-r--r--   0 nazime    (1000) nazime    (1000)      305 2021-09-23 15:10:16.000000 koalak-0.2.9/.coveragerc
--rw-r--r--   0 nazime    (1000) nazime    (1000)      105 2021-08-16 18:26:39.000000 koalak-0.2.9/.isort.cfg
--rw-r--r--   0 nazime    (1000) nazime    (1000)     1831 2021-08-16 18:28:09.000000 koalak-0.2.9/.pre-commit-config.yaml
--rw-r--r--   0 nazime    (1000) nazime    (1000)      227 2021-08-13 11:09:56.000000 koalak-0.2.9/.readthedocs.yml
--rw-r--r--   0 nazime    (1000) nazime    (1000)      290 2021-08-13 11:09:56.000000 koalak-0.2.9/.travis.yml
--rw-r--r--   0 nazime    (1000) nazime    (1000)     1063 2021-08-13 11:09:56.000000 koalak-0.2.9/LICENSE
--rw-r--r--   0 nazime    (1000) nazime    (1000)      286 2021-08-13 11:09:56.000000 koalak-0.2.9/MANIFEST.in
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     1455 2022-02-06 20:26:20.997206 koalak-0.2.9/PKG-INFO
--rw-rw-r--   0 nazime    (1000) nazime    (1000)      360 2021-08-16 19:34:04.000000 koalak-0.2.9/README.md
--rw-r--r--   0 nazime    (1000) nazime    (1000)       86 2021-08-13 11:09:56.000000 koalak-0.2.9/codecov.yml
-drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2022-02-06 20:26:20.993206 koalak-0.2.9/docs/
--rw-r--r--   0 nazime    (1000) nazime    (1000)      634 2021-08-13 11:09:56.000000 koalak-0.2.9/docs/Makefile
--rw-r--r--   0 nazime    (1000) nazime    (1000)     1843 2021-08-13 11:09:56.000000 koalak-0.2.9/docs/conf.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)      427 2021-08-13 11:09:56.000000 koalak-0.2.9/docs/index.rst
--rw-r--r--   0 nazime    (1000) nazime    (1000)      795 2021-08-13 11:09:56.000000 koalak-0.2.9/docs/make.bat
--rw-r--r--   0 nazime    (1000) nazime    (1000)      121 2021-08-13 11:09:56.000000 koalak-0.2.9/pyproject.toml
--rw-r--r--   0 nazime    (1000) nazime    (1000)       73 2022-02-06 20:26:20.997206 koalak-0.2.9/setup.cfg
--rw-r--r--   0 nazime    (1000) nazime    (1000)     3075 2021-10-01 00:04:00.000000 koalak-0.2.9/setup.py
-drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2022-02-06 20:26:20.993206 koalak-0.2.9/src/
-drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2022-02-06 20:26:20.993206 koalak-0.2.9/src/koalak/
--rw-r--r--   0 nazime    (1000) nazime    (1000)      876 2021-10-01 13:18:57.000000 koalak-0.2.9/src/koalak/__init__.py
--rw-rw-r--   0 nazime    (1000) nazime    (1000)    22982 2022-02-05 22:29:09.000000 koalak-0.2.9/src/koalak/bases.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)      145 2022-02-06 20:24:39.000000 koalak-0.2.9/src/koalak/consts.py
-drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2022-02-06 20:26:20.997206 koalak-0.2.9/src/koalak/databases/
--rw-rw-r--   0 nazime    (1000) nazime    (1000)      234 2021-10-17 17:26:58.000000 koalak-0.2.9/src/koalak/databases/__init__.py
--rw-rw-r--   0 nazime    (1000) nazime    (1000)    12401 2022-02-05 21:58:18.000000 koalak-0.2.9/src/koalak/databases/databases.py
--rw-rw-r--   0 nazime    (1000) nazime    (1000)    21479 2021-10-01 12:23:01.000000 koalak-0.2.9/src/koalak/databases/helper_tests.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)    14471 2021-10-01 00:06:46.000000 koalak-0.2.9/src/koalak/databases/relationaldb.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)    22899 2021-10-01 00:06:46.000000 koalak-0.2.9/src/koalak/databases/relationaldb_sqlalchemy.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)    12756 2021-08-16 18:25:52.000000 koalak-0.2.9/src/koalak/decorators.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)      429 2021-08-13 11:09:56.000000 koalak-0.2.9/src/koalak/exceptions.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)      871 2021-10-01 00:07:23.000000 koalak-0.2.9/src/koalak/fixtures.py
-drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2022-02-06 20:26:20.997206 koalak-0.2.9/src/koalak/frameworks/
--rw-r--r--   0 nazime    (1000) nazime    (1000)        0 2021-08-13 11:09:56.000000 koalak-0.2.9/src/koalak/frameworks/__init__.py
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     6932 2021-10-01 11:35:39.000000 koalak-0.2.9/src/koalak/frameworks/home_structure.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)        0 2021-08-13 11:09:56.000000 koalak-0.2.9/src/koalak/frameworks/mkframework.py
-drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2022-02-06 20:26:20.997206 koalak-0.2.9/src/koalak/helpers/
--rw-r--r--   0 nazime    (1000) nazime    (1000)        0 2021-08-13 11:09:56.000000 koalak-0.2.9/src/koalak/helpers/__init__.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)     9027 2022-02-06 20:17:56.000000 koalak-0.2.9/src/koalak/helpers/argparse_helper.py
--rw-rw-r--   0 nazime    (1000) nazime    (1000)       77 2021-10-17 17:23:10.000000 koalak-0.2.9/src/koalak/helpers_test.py
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     3123 2021-09-23 15:18:05.000000 koalak-0.2.9/src/koalak/utils.py
-drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2022-02-06 20:26:20.993206 koalak-0.2.9/src/koalak.egg-info/
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     1455 2022-02-06 20:26:20.000000 koalak-0.2.9/src/koalak.egg-info/PKG-INFO
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     1646 2022-02-06 20:26:20.000000 koalak-0.2.9/src/koalak.egg-info/SOURCES.txt
--rw-rw-r--   0 nazime    (1000) nazime    (1000)        1 2022-02-06 20:26:20.000000 koalak-0.2.9/src/koalak.egg-info/dependency_links.txt
--rw-rw-r--   0 nazime    (1000) nazime    (1000)        1 2021-08-16 18:01:38.000000 koalak-0.2.9/src/koalak.egg-info/not-zip-safe
--rw-rw-r--   0 nazime    (1000) nazime    (1000)      217 2022-02-06 20:26:20.000000 koalak-0.2.9/src/koalak.egg-info/requires.txt
--rw-rw-r--   0 nazime    (1000) nazime    (1000)        7 2022-02-06 20:26:20.000000 koalak-0.2.9/src/koalak.egg-info/top_level.txt
-drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2022-02-06 20:26:20.997206 koalak-0.2.9/tests/
--rw-r--r--   0 nazime    (1000) nazime    (1000)        0 2021-08-13 11:09:56.000000 koalak-0.2.9/tests/__init__.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)     7817 2021-08-13 11:09:56.000000 koalak-0.2.9/tests/noatest_decorators_addinit.py
-drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2022-02-06 20:26:20.997206 koalak-0.2.9/tests/noptest_databases/
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     3717 2021-10-17 17:26:58.000000 koalak-0.2.9/tests/noptest_databases/test_dict_db.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)     2811 2021-10-17 17:26:58.000000 koalak-0.2.9/tests/noptest_databases/test_list_database.py
-drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2022-02-06 20:26:20.997206 koalak-0.2.9/tests/test_decorators/
--rw-r--r--   0 nazime    (1000) nazime    (1000)     8767 2021-08-16 18:24:44.000000 koalak-0.2.9/tests/test_decorators/atest_decorators_addinit.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)     3039 2021-08-16 18:18:15.000000 koalak-0.2.9/tests/test_decorators/test_add_postinit.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)     3779 2021-08-18 16:28:06.000000 koalak-0.2.9/tests/test_decorators/test_optionalargs.py
-drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2022-02-06 20:26:20.997206 koalak-0.2.9/tests/test_file_actions/
--rw-r--r--   0 nazime    (1000) nazime    (1000)     3367 2021-10-01 13:12:42.000000 koalak-0.2.9/tests/test_file_actions/test_bashrc.py
-drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2022-02-06 20:26:20.997206 koalak-0.2.9/tests/test_framework/
--rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2021-09-24 17:03:41.000000 koalak-0.2.9/tests/test_framework/__init__.py
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     2640 2021-09-25 14:51:22.000000 koalak-0.2.9/tests/test_framework/test_db_in_framework.py
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     2530 2021-10-01 13:09:16.000000 koalak-0.2.9/tests/test_framework/test_framework.py
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     2475 2021-09-25 15:00:24.000000 koalak-0.2.9/tests/test_framework/test_variables.py
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     1152 2021-10-01 14:21:32.000000 koalak-0.2.9/tests/test_framework_manager.py
-drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2022-02-06 20:26:20.997206 koalak-0.2.9/tests/test_helpers/
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     6154 2021-09-30 22:35:21.000000 koalak-0.2.9/tests/test_helpers/test_argparse_helper.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)     2103 2021-09-21 18:44:04.000000 koalak-0.2.9/tests/test_hooks.py
--rw-rw-r--   0 nazime    (1000) nazime    (1000)    10232 2021-09-23 15:18:05.000000 koalak-0.2.9/tests/test_init_home.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)     6669 2022-02-06 20:25:48.000000 koalak-0.2.9/tests/test_plugin_managers.py
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     3039 2021-10-01 13:19:28.000000 koalak-0.2.9/tests/test_simple.py
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     2486 2021-09-23 15:18:05.000000 koalak-0.2.9/tests/test_utils.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)        0 2021-08-13 11:09:56.000000 koalak-0.2.9/tests/utils.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)      976 2021-09-23 15:09:44.000000 koalak-0.2.9/tox.ini
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.491038 koalak-0.3.1/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      305 2023-06-24 11:05:31.000000 koalak-0.3.1/.coveragerc
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      244 2023-06-24 11:05:31.000000 koalak-0.3.1/.isort.cfg
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     1854 2023-06-24 11:05:31.000000 koalak-0.3.1/.pre-commit-config.yaml
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      227 2023-06-24 11:05:31.000000 koalak-0.3.1/.readthedocs.yml
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      290 2023-06-24 11:05:31.000000 koalak-0.3.1/.travis.yml
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     1063 2023-06-24 11:05:31.000000 koalak-0.3.1/LICENSE
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      335 2023-06-24 11:05:31.000000 koalak-0.3.1/MANIFEST.in
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     1500 2023-07-29 20:02:18.491038 koalak-0.3.1/PKG-INFO
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      397 2023-07-29 19:53:44.000000 koalak-0.3.1/README.md
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)       86 2023-06-24 11:05:31.000000 koalak-0.3.1/codecov.yml
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.483038 koalak-0.3.1/docs/
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.483038 koalak-0.3.1/docs/docs/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     1999 2023-06-24 11:05:31.000000 koalak-0.3.1/docs/docs/wordlistools_example.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2023-06-24 11:05:31.000000 koalak-0.3.1/docs/example.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     9954 2023-06-24 11:05:31.000000 koalak-0.3.1/docs/example_codegen.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      121 2023-06-24 11:05:31.000000 koalak-0.3.1/pyproject.toml
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)       73 2023-07-29 20:02:18.491038 koalak-0.3.1/setup.cfg
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     3331 2023-06-24 11:05:31.000000 koalak-0.3.1/setup.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.479038 koalak-0.3.1/src/
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.483038 koalak-0.3.1/src/koalak/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      748 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/__init__.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.483038 koalak-0.3.1/src/koalak/_deprecated/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/_deprecated/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     9276 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/_deprecated/argparse_helper.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.483038 koalak-0.3.1/src/koalak/_workinprogress/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/_workinprogress/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      871 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/_workinprogress/fixtures.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     4445 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/_workinprogress/multipleapi.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      188 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/all.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)    18553 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/bases.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      528 2023-07-29 20:00:37.000000 koalak-0.3.1/src/koalak/consts.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.483038 koalak-0.3.1/src/koalak/core/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      237 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/core/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)    11888 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/core/bases.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.483038 koalak-0.3.1/src/koalak/databases/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      234 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/databases/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/databases/bases.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)    12479 2023-07-29 19:58:27.000000 koalak-0.3.1/src/koalak/databases/databases.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)    21477 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/databases/helper_tests.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)    14470 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/databases/relationaldb.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)    25746 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/databases/relationaldb_sqlalchemy.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)    12821 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/decorators.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      429 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/exceptions.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.483038 koalak-0.3.1/src/koalak/frameworks/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/frameworks/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     6948 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/frameworks/home_structure.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/frameworks/mkframework.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.483038 koalak-0.3.1/src/koalak/iterpaths/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)       33 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/iterpaths/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)    15141 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/iterpaths/iterpaths.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.483038 koalak-0.3.1/src/koalak/list_of_dict/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)       37 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/list_of_dict/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     6976 2023-07-29 19:53:43.000000 koalak-0.3.1/src/koalak/list_of_dict/list_of_dict.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.483038 koalak-0.3.1/src/koalak/plugin_manager/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)       59 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/plugin_manager/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     4659 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/plugin_manager/constraints.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)    14503 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/plugin_manager/plugin_manager.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)       23 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/plugin_manager/plugin_runner.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.483038 koalak-0.3.1/src/koalak/relationaldb/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      209 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/relationaldb/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     3307 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/relationaldb/bases.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)    15554 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/relationaldb/conception.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)       18 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/relationaldb/consts.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.483038 koalak-0.3.1/src/koalak/relationaldb/data/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     7249 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/relationaldb/data/mongodb_template.jinja2
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      444 2023-07-29 19:15:44.000000 koalak-0.3.1/src/koalak/relationaldb/data/mongodb_template_one_cls.jinja2
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)       42 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/relationaldb/exceptions.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     8563 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/relationaldb/mongodb_builder.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/relationaldb/random_data_generation.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      388 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/relationaldb/utils.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.483038 koalak-0.3.1/src/koalak/selenium_automator/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     4316 2023-07-29 19:56:20.000000 koalak-0.3.1/src/koalak/selenium_automator/selenium_automator.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.483038 koalak-0.3.1/src/koalak/subcommand_parser/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)       48 2023-06-24 11:05:31.000000 koalak-0.3.1/src/koalak/subcommand_parser/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)    16009 2023-07-29 19:15:21.000000 koalak-0.3.1/src/koalak/subcommand_parser/subcommand_parser.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)    11970 2023-07-29 19:15:21.000000 koalak-0.3.1/src/koalak/utils.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.483038 koalak-0.3.1/src/koalak.egg-info/
+-rw-r--r--   0 nazime    (1000) nazime    (1000)     1500 2023-07-29 20:02:18.000000 koalak-0.3.1/src/koalak.egg-info/PKG-INFO
+-rw-r--r--   0 nazime    (1000) nazime    (1000)     4774 2023-07-29 20:02:18.000000 koalak-0.3.1/src/koalak.egg-info/SOURCES.txt
+-rw-r--r--   0 nazime    (1000) nazime    (1000)        1 2023-07-29 20:02:18.000000 koalak-0.3.1/src/koalak.egg-info/dependency_links.txt
+-rw-r--r--   0 nazime    (1000) nazime    (1000)        1 2023-07-29 19:01:24.000000 koalak-0.3.1/src/koalak.egg-info/not-zip-safe
+-rw-r--r--   0 nazime    (1000) nazime    (1000)      420 2023-07-29 20:02:18.000000 koalak-0.3.1/src/koalak.egg-info/requires.txt
+-rw-r--r--   0 nazime    (1000) nazime    (1000)        7 2023-07-29 20:02:18.000000 koalak-0.3.1/src/koalak.egg-info/top_level.txt
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.483038 koalak-0.3.1/tests/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/__init__.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.487038 koalak-0.3.1/tests/test_core/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_core/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     1712 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_core/test_entity_description.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     2543 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_core/test_generic_field.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     1071 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_core/test_named_unnamed_container.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     4314 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_core/test_object_storage.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.487038 koalak-0.3.1/tests/test_decorators/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_decorators/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     8767 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_decorators/atest_decorators_addinit.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     3039 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_decorators/test_add_postinit.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     5244 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_decorators/test_optionalargs.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.487038 koalak-0.3.1/tests/test_deprecated/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_deprecated/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     6182 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_deprecated/test_argparse_helper.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     2103 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_deprecated/test_hooks.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.487038 koalak-0.3.1/tests/test_framework/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_framework/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     2640 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_framework/test_db_in_framework.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.487038 koalak-0.3.1/tests/test_framework/test_file_actions/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_framework/test_file_actions/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     3367 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_framework/test_file_actions/test_bashrc.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     2530 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_framework/test_framework.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     1152 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_framework/test_framework_manager.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     3039 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_framework/test_simple.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     2475 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_framework/test_variables.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.487038 koalak-0.3.1/tests/test_iterpaths/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_iterpaths/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     1929 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_iterpaths/test_duplicates_only.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     3104 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_iterpaths/test_endswith.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     4300 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_iterpaths/test_filter_isearch.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     1807 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_iterpaths/test_iter_paths.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      147 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_iterpaths/test_iterpath_import.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     9538 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_iterpaths/test_plugins_directly.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     6022 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_iterpaths/test_search.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     2845 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_iterpaths/test_skip_duplicates.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     5165 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_iterpaths/test_startswith.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      365 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_iterpaths/utils_test_iterpath.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.487038 koalak-0.3.1/tests/test_koalak_utils/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_koalak_utils/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     2590 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_koalak_utils/test_data_to_csv.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     4759 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_koalak_utils/test_data_to_excel.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     1196 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_koalak_utils/test_str_find_all.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     4071 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_koalak_utils/test_utils.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.487038 koalak-0.3.1/tests/test_list_of_dict/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)    14408 2023-07-29 19:49:20.000000 koalak-0.3.1/tests/test_list_of_dict/test_list_of_dicts.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.491038 koalak-0.3.1/tests/test_plugin_managers/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_plugin_managers/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     1675 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_plugin_managers/test_plugin_manager_instances.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     3592 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_plugin_managers/test_plugin_manager_metadata.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     2159 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_plugin_managers/test_plugin_managers_abstract_plugins.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     2723 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_plugin_managers/test_plugin_managers_basics.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     2987 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_plugin_managers/test_plugin_managers_constraints.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      612 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_plugin_managers/test_plugin_managers_run.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     2695 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_plugin_managers/test_plugin_managers_unsorted.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.491038 koalak-0.3.1/tests/test_relationaldb/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_relationaldb/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      200 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_relationaldb/test_basic_operations.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)    11709 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_relationaldb/test_conception.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     3425 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_relationaldb/test_operations_create.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      801 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_relationaldb/test_operations_delete.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      263 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_relationaldb/test_operations_feed.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     5379 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_relationaldb/test_operations_read.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     5509 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_relationaldb/test_operations_update.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.491038 koalak-0.3.1/tests/test_subcommand_parser/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_subcommand_parser/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)    17015 2023-07-29 19:15:21.000000 koalak-0.3.1/tests/test_subcommand_parser/test_subcommand_parser.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.491038 koalak-0.3.1/tests/test_unsorted/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     7817 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_unsorted/noatest_decorators_addinit.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)    10232 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_unsorted/test_init_home.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.479038 koalak-0.3.1/tests/test_useless/
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-07-29 20:02:18.491038 koalak-0.3.1/tests/test_useless/noptest_databases/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        0 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_useless/noptest_databases/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     3727 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_useless/noptest_databases/test_dict_db.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     2821 2023-06-24 11:05:31.000000 koalak-0.3.1/tests/test_useless/noptest_databases/test_list_database.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      625 2023-06-24 11:05:31.000000 koalak-0.3.1/tox.ini
```

### Comparing `koalak-0.2.9/.pre-commit-config.yaml` & `koalak-0.3.1/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+exclude: 'BRAINSTORM/'
 repos:
   # Black
   - repo: https://github.com/psf/black
-    rev: 19.3b0
+    rev: 22.3.0
     hooks:
       - id: black
         language_version: python3
         args: [--safe, --quiet]
         # override until resolved: https://github.com/ambv/black/issues/402
         files: \.pyi?$
         types: []
```

### Comparing `koalak-0.2.9/LICENSE` & `koalak-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `koalak-0.2.9/PKG-INFO` & `koalak-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: koalak
-Version: 0.2.9
+Version: 0.3.1
 Summary: Framework manager, framework to create frameworks
 Home-page: https://github.com/nazime/koalak
 Author: Nazime LAKEHAL
 Author-email: nazime.lkh@gmail.com
 Maintainer: Nazime LAKEHAL
 Maintainer-email: nazime.lkh@gmail.com
 License: MIT
 Project-URL: Documentation, https://koalak.readthedocs.org/
 Project-URL: Bug Tracker, https://github.com/nazime/koalak/issues
 Project-URL: Source Code, https://github.com/nazime/koalak
 Description: # Koalak
         
-        Koalak is a collections of tools that helps me create my libraries, the library focus on creating plugins architectures. The project is currently under development, I shared the repository because it is used by my tool **wordlistools**.
+        Koalak is a collections of tools that helps me create my libraries, the library focus on creating plugins architectures.
+        The project is currently under development, I shared the repository because it is used by my tool **wordlistools**.
         
         Koala features
         
-        - Manage plugins for your project
-        - Allow you to create new plugins from project home directory
+        - Manage plugins for your project, more information on the wiki.
+        - Argparse wrapper to create CLI interfaces with subcommands easily
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tests
+Provides-Extra: dev
 Provides-Extra: travis
```

### Comparing `koalak-0.2.9/setup.py` & `koalak-0.3.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,17 +53,33 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
 ]
 
 # Packages information
 PACKAGES = find_packages(where="src")
 PACKAGE_DIR = {"": "src"}
-INSTALL_REQUIRES = ["sqlalchemy", "coloring", "attrs"]
+INSTALL_REQUIRES = [
+    "sqlalchemy",
+    "coloring",
+    "attrs",
+    "argcomplete",
+    "toml",
+    "black",
+    "typeguard>=4",
+    "rich",
+    "devtools",
+    # relationaldb
+    "pymongo",
+    "codeg",
+    "jinja2",
+    # for utils functions
+    "openpyxl",
+]
 EXTRAS_REQUIRE = {
-    "docs": ["sphinx"],
+    "docs": ["sphinx", "sphinxcontrib.napoleon", "sphinx-book-theme"],
     "tests": [
         "coverage",
         "hypothesis",
         "pytest>=4.3.0",  # 4.3.0 dropped last use of `convert`
     ],
 }
 EXTRAS_REQUIRE["dev"] = (
@@ -71,15 +87,15 @@
 )
 
 EXTRAS_REQUIRE["travis"] = EXTRAS_REQUIRE["dev"] + ["tox", "codecov"]
 PYTHON_REQUIRES = ">=3.6"
 
 ZIP_SAFE = False
 ENTRY_POINTS = {}
-INCLUDE_PACKAGE_DATA = False
+INCLUDE_PACKAGE_DATA = True
 PACKAGE_DATA = {"koala": ["data/*"]}
 
 if __name__ == "__main__":
     setup(
         # Metadata
         name=NAME,
         version=VERSION,
```

### Comparing `koalak-0.2.9/src/koalak/__init__.py` & `koalak-0.3.1/src/koalak/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 # Import decorators
-from koalak.helpers.argparse_helper import ArgparseSubcmdHelper
-
 from .bases import DirectoryDescription as D
 from .bases import FileDescription as F
-from .bases import frameworks, mkpluginmanager
+from .bases import frameworks
 
 # import databases
 from .databases import (
     BaseRelationalDB,
     Database,
     DictDB,
     JsonListDB,
     ListDB,
     RelationalDB,
     TxtListDB,
-    relationaldb,
 )
 from .decorators import add_post_init, addinit, optionalargs
 
 get_unique_framework_name = frameworks.get_unique_framework_name
 generate_unique_framework_name = frameworks.generate_unique_framework_name
 get_framework = frameworks.get_framework
 mkframework = frameworks.mkframework
@@ -26,11 +23,10 @@
 
 
 __all__ = [
     "generate_unique_framework_name",
     "get_framework",
     "mkframework",
     "get_frameworks",
-    "ArgparseSubcmdHelper",
     "F",
     "D",
 ]
```

### Comparing `koalak-0.2.9/src/koalak/bases.py` & `koalak-0.3.1/src/koalak/bases.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 import collections
-import glob
 import inspect
 import os
 import shutil
 import typing
+import warnings
 from string import Template
 from typing import Any, Callable, Dict, List, Union
 
+import attrs
 import coloring
+import toml
 from koalak.frameworks import home_structure
 from koalak.frameworks.home_structure import (
     DirectoryDescription,
     FileDescription,
     normalize_home_structure,
 )
 
 from . import databases, exceptions
 from .consts import HOMEPATH_NAME, PACKAGE_NAME
+from .plugin_manager import PluginManager
 
 """This module contain the main bases for the project koalak (framework, plugin managers, ...)"""
 
 
 def __init_subclass__(subcls, **kwargs):
-
     if "name" not in subcls.__dict__:
         raise ValueError(f"Base plugin must have the attribute 'name'")
 
     # add the plugin
     name = subcls.__dict__["name"]
     pm = subcls._fwm["plugin_manager"]
-    if name in pm._plugins:
+    if name in pm.plugins:
         raise exceptions.PluginAlreadyExistException(f"plugin {name} already exist")
 
-    pm._plugins[name] = subcls
+    pm.plugins[name] = subcls
 
     # abstract class
     if FwmConfig.is_abstract(subcls):
         pass
 
 
-def init_subclass(subcls, **kwargs):
-    subcls._pluginmanager._register(subcls)
-
-
 class FwmConfig:
     """Class responsible to handle internal config in objects
     like plugins. Ex: @abstract"""
 
     dict_name = PACKAGE_NAME
 
     @classmethod
@@ -99,164 +97,14 @@
         return len(self._dict_data) + len(self._list_data)
 
 
 class Plugin:
     pass
 
 
-def mkpluginmanager(*args, **kwargs):
-    return PluginManager(*args, **kwargs)
-
-
-class ConstraintAttr:
-    def __init__(self, name: str = None, type=None, inheritable: bool = True):
-        """
-
-        Args:
-            name: name of the class attribute
-            type: type of the class attribute
-            inheritable: if the attribute can be inherited (True)
-                or if each class must define the class attribute (False)
-        """
-        self.name = name
-        self.type = type
-        self.inheritable = inheritable
-
-    def check(self, plugin):
-        if self.name is None:
-            raise TypeError("Must set the attribute name")
-        if self.inheritable:
-            has_attr = hasattr(plugin, self.name)
-        else:
-            has_attr = self.name in plugin.__dict__
-
-        if not has_attr:
-            raise TypeError(
-                f"plugin {plugin.__name__!r} must have the class attribute {self.name!r}"
-            )
-
-        plugin_attr = getattr(plugin, self.name)
-        # Check type
-        if self.type is not None:
-            if not isinstance(plugin_attr, self.type):
-                raise TypeError(
-                    f"class attribute {self.name} must be of type {self.type}"
-                )
-
-
-class PluginManager(KoalakContainer):
-    """
-
-    How it work:
-
-    """
-
-    def __init__(self, name: str = None, *, homepath=None):
-        super().__init__()
-
-        # FIXME: plugin without name?
-        self.name: str = name
-        self.baseplugin = None
-        self.homepath = homepath
-        self._plugins = {}
-        self._initialized = False
-        self._constraints = []
-
-    def __repr__(self):
-        if self.name:
-            return f"<PluginManager [{self.name}]>"
-        else:
-            return f"<PluginManager>"
-
-    def __str__(self):
-        return self.__repr__()
-
-    def _assert_baseplugin(self):
-        if self.baseplugin is None:
-            raise TabError("BasePlugin not initiated!")
-
-    def _register(self, plugin):
-        if self.baseplugin is None:
-            raise TypeError(
-                "Can't register plugin without baseplugin. use mkbaseplugin before"
-            )
-
-        # Fixme: better think abstract class
-        is_abstract = "abstract" in plugin.__dict__
-        if not is_abstract:
-            # Check constraint before registring
-            for contraint in self._constraints:
-                contraint.check(plugin)
-
-            self._add_item(plugin, plugin.name)
-
-    def mkbaseplugin(self, baseplugin):
-        self.baseplugin = baseplugin
-        baseplugin._pluginmanager = self
-        baseplugin.__init_subclass__ = classmethod(init_subclass)
-
-        attrs_to_del = []  # we can't del in loop
-        for name, constraint in baseplugin.__dict__.items():
-            if isinstance(constraint, ConstraintAttr):
-                constraint.name = name
-                self._constraints.append(constraint)
-                attrs_to_del.append(name)
-        for attr_name in attrs_to_del:
-            delattr(baseplugin, attr_name)
-
-        # All custom plugins (loaded from home) have _is_home_plugin to True
-        self.baseplugin._is_home_plugin = False
-        return baseplugin
-
-    def init(self, _homepath_initialized: set = None):
-        _homepath_initialized = _homepath_initialized or set()
-        if self.homepath is None:
-            raise TypeError("You can not init a plugin mananger without homepath")
-
-        if self._initialized:
-            raise TypeError("Plugin Already initiated")
-        self._initialized = True
-
-        if self.homepath in _homepath_initialized:
-            return
-        self._init_home()
-        self._load_plugins()
-
-    def attr(self, type=None, inheritable=True):
-        return ConstraintAttr(type=type, inheritable=inheritable)
-
-    def get_home_plugins(self):
-        """Get plugins loaded from home/plugins"""
-        for e in self:
-            if e._is_home_plugin:
-                yield e
-
-    def _load_plugins(self):
-        """Load home plugins"""
-        for python_path in glob.glob(os.path.join(self.homepath, "*.py")):
-            with open(python_path) as f:
-                data = f.read()
-                execution_context = {}
-                exec(data, execution_context)
-                for object_name, object in execution_context.items():
-                    if inspect.isclass(object) and issubclass(object, self.baseplugin):
-                        if object is self.baseplugin:
-                            continue
-                        object._is_home_plugin = True
-
-    def _init_home(self):
-        if not self.homepath:
-            return
-        if not os.path.exists(self.homepath):
-            os.makedirs(self.homepath)
-        elif os.path.isfile(self.homepath):
-            raise NotADirectoryError("Home path is not a directory")
-        # else it's a directory already created
-
-
 class HookManager:
     def __init__(self, name, spec_func):
         self.name = name
         self.spec_func = spec_func
         self._hooks = {}
 
     def register(self, func):
@@ -326,34 +174,40 @@
         self,
         name: str = None,
         *,
         homepath: str = None,
         home_structure=None,
         variables: Dict[str, Any] = None,
         version: str = None,
+        config: Dict = None,
     ):
-
         # TODO: add param substitute_vars, to substitute variables on init?
         if variables is None:
             variables = {}
 
+        if config is None:
+            config = {}
+
         self.variables = FrameworkVariables(variables)
 
         self.name: str = name
         self.homepath: str = homepath
+        self.config = config
         if version is None:
             version = "0.0.0"
         self.version: str = version
         # The framework can be initialized if it has a name or a home path
         self._can_be_initialized = name or homepath
         if self._can_be_initialized and self.homepath is None:
             self.homepath = os.path.expanduser(
                 os.path.join("~", f".{HOMEPATH_NAME}", self.name)
             )
 
+        if self.homepath:
+            self.config_path = os.path.join(self.homepath, "config.toml")
         if home_structure is None:
             home_structure = []
         else:
             home_structure = normalize_home_structure(home_structure)
         self._home_structure = home_structure
         # self._plugin_managers: Dict[str, PluginManager] = {}
         self.plugin_managers = KoalakContainer()
@@ -404,14 +258,20 @@
         for plugin_manager in self.plugin_managers:
             homepath = plugin_manager.homepath
             plugin_manager.init(_homepath_initialized=homepath_initialized)
             homepath_initialized.add(homepath)
 
         # TODO: at the end init the framework database (version)
 
+        if os.path.exists(self.config_path):
+            self.config = toml.load(self.config_path)
+        else:
+            with open(self.config_path, "w") as f:
+                toml.dump(self.config, f)
+
     def _is_initialized(self):
         return os.path.isdir(self.homepath)
 
     def _init_home(self, parent_path=None, nodes=None):
         """Recursive function"""
         # FIXME: add support for nodes as list of string and dict
         # FIXME: see _normalize_home_node and skipped tests
@@ -473,15 +333,14 @@
         else:
             pass
             # TODO: raise not handled type
 
         return _mkhookmanager
 
     def mkpluginmanager(self, pluginmanager_name: str = None, homepath=None):
-
         if homepath is None and self.homepath:
             homepath = os.path.join(self.homepath, "plugins")
         elif homepath and self.homepath:
             homepath = os.path.join(self.homepath, homepath)
 
         pluginmanager = PluginManager(pluginmanager_name, homepath=homepath)
         self.plugin_managers._add_item(pluginmanager, pluginmanager_name)
@@ -502,22 +361,22 @@
             return base_cls
 
         return _mkplugin
 
     def get_plugins(self, plugin_manager_name: str):
         from warnings import warn
 
-        warn("get_plugins is deprecated use plugin_managers instead")
+        warn("get_plugins is _deprecated use plugin_managers instead")
 
         return self.plugin_managers[plugin_manager_name].get_plugins()
 
     def get_plugin_manager(self, plugin_manager_name: str) -> PluginManager:
         from warnings import warn
 
-        warn("get_plugin_manager is deprecated use plugin_managers[<name>] instead")
+        warn("get_plugin_manager is _deprecated use plugin_managers[<name>] instead")
         return self.plugin_managers[plugin_manager_name]
 
     def get_hook_manager(self, hook_manager_name: str) -> HookManager:
         return self._hook_managers[hook_manager_name]
 
     def get_hook_managers(self):
         return list(self._hook_managers.values())
@@ -656,45 +515,47 @@
         self,
         framework_name: str = None,
         *,
         homepath=None,
         home_structure=None,
         variables=None,
         version: str = None,
+        config: Dict = None,
     ) -> Framework:
         if framework_name and framework_name in self:
             raise exceptions.FrameworkAlreadyExistException(
                 f"Framework {framework_name} already exist"
             )
 
         framework = Framework(
             framework_name,
             homepath=homepath,
             home_structure=home_structure,
             variables=variables,
             version=version,
+            config=config,
         )
 
         self._add_item(framework, framework_name)
         return framework
 
     def get_framework(self, framework_name: str) -> Framework:
         import warnings
 
         warnings.warn(
-            "get_framework deprecated use frameworks[<name>] instead",
+            "get_framework _deprecated use frameworks[<name>] instead",
             DeprecationWarning,
         )
         return self[framework_name]
 
     def get_frameworks(self) -> List[Framework]:
         import warnings
 
         warnings.warn(
-            "get_frameworks deprecated use frameworks instead", DeprecationWarning
+            "get_frameworks _deprecated use frameworks instead", DeprecationWarning
         )
         return list(self)
 
     def generate_unique_framework_name(self):
         while True:
             self._unique_framework_name_counter += 1
             counter = self._unique_framework_name_counter
@@ -702,14 +563,14 @@
             if name not in self:
                 return name
 
     def get_unique_framework_name(self) -> str:
         import warnings
 
         warnings.warn(
-            "get_unique_framework_name deprecated use generate_unique_framework_name instead",
+            "get_unique_framework_name _deprecated use generate_unique_framework_name instead",
             DeprecationWarning,
         )
         return self.generate_unique_framework_name()
 
 
 frameworks = FrameworkManager()
```

### Comparing `koalak-0.2.9/src/koalak/databases/databases.py` & `koalak-0.3.1/src/koalak/databases/databases.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+# FIXME: THIS SCRIPT IS NOTE WORKING #
+# ================================== #
 import abc
 import collections
 import json
 import os
 import shutil
 import typing
 from typing import Any, List
 
 from koalak.utils import get_prefixed_callables_of_object, temp_pathname
 
 """
 Introduction:
 =============
 These databases are meant for light usage since they are slow/heavy
-and they sinc each time
+and they sync each time
 It is designed to be used as a builtin list or dict
 
 
 Existing similar project (using files):
 =======================================
 - sqlite
 - text/csv/json
```

### Comparing `koalak-0.2.9/src/koalak/databases/helper_tests.py` & `koalak-0.3.1/src/koalak/databases/helper_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,19 +75,17 @@
 
             l3 = [v2] + l
             assert l3 == [v2, v1]
             assert type(l3) is list
             assert list(l) == [v1]
 
     def test__del(self):
-
         v1, v2, v3 = self.values[:3]
 
         with temp_pathname() as path:
-
             l = self.cls(path, [v1, v2, v3], autosync=True)
             assert list(l) == [v1, v2, v3]
 
             del l[0]
             assert list(l) == [v2, v3]
             l = self.cls(path, autosync=True)
             assert list(l) == [v2, v3]
```

### Comparing `koalak-0.2.9/src/koalak/databases/relationaldb.py` & `koalak-0.3.1/src/koalak/databases/relationaldb.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,14 @@
         eq=None,
         order=None,
         on_setattr=None,
         # sqlalchemy attribute
         unique=None,
         ref=None,
     ):
-
         metadata = self.metadata(unique=unique, ref=ref)
         return attr.ib(  # noqa
             default=default,
             validator=validator,
             repr=repr,
             cmp=cmp,
             hash=hash,
```

### Comparing `koalak-0.2.9/src/koalak/databases/relationaldb_sqlalchemy.py` & `koalak-0.3.1/src/koalak/databases/relationaldb_sqlalchemy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """THIS CODE IS A WORK IN PROGRESS"""
 import collections
-import datetime
 import inspect
 import logging
 import typing
+from datetime import datetime
 
 import attr
 import coloring
 import sqlalchemy
 from koalak.consts import PACKAGE_NAME
 from koalak.decorators import add_post_init, optionalargs
 from sqlalchemy import (
@@ -19,98 +19,142 @@
     Integer,
     String,
     create_engine,
 )
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 
-logger = logging.getLogger("koala")
+logger = logging.getLogger("koalak")
 logger.setLevel(logging.DEBUG)
 
 try:
     typping_ForwardRef = typing.ForwardRef
 except AttributeError:
     typping_ForwardRef = typing._ForwardRef  # noqa
 
 
+class ProgrammingError(Exception):
+    """Things that should not happen!"""
+
+    pass
+
+
 """
 RelationalDB is a wrapper for sqlalchemy and attr to have
 a relational database with a better API and abstraction
 - no ID
 - specify relations with annoation (List["Animal"], Animal, ...)
 - use attr to create __init__, __repr__, ...
 See examples in test_relationaldb.py
 
 
 
 """
 
+"""
+TODO: Error tests
+- Default None -> Nullable True
+- Not null and default is None => error
+-
+"""
+AttribType = type(attr.ib())
+AttrNOTHING = attr.ib()._default
+
+
+def parse_typing_type(t):
+    if len(t.__args__) != 1:
+        raise ValueError("Annotation list must have one and only one argument")
+
+    return {"type": t._name, "name": t.__args__[0].__forward_arg__}
+
 
 @attr.s
-class BuildingRelationalAttribute:
+class ColumnMetadata:
     """Helper cls to build relational attribute"""
 
     name: str = attr.ib()
+    type = attr.ib(kw_only=True, default=None)
     many: bool = attr.ib(default=None)
-    atomic_type_name: str = attr.ib(
-        default=None
-    )  # type of the referenced table (without the List)
-    referenced_by: "BuildingRelationalAttribute" = attr.ib(default=None)
+    referenced_by: "ColumnMetadata" = attr.ib(default=None)
     attr_attribute = attr.ib(default=None)
+    unique = attr.ib(default=None)
+    nullable = attr.ib(default=None)
+    default = attr.ib(default=None)
 
     # this attribute is set to True by the class that contain this
     #  attribute, sins it is possible for an other class to create
     #  an attribute with ref (having exist=True we are sure that
     #  the attribute exist and it's not just a reference)
     exist = attr.ib(default=None)
 
-    def __attrs_post_init__(self):
-        if self.name == "age":
-            coloring.print_bred("AGE IS BUILT")
-            print(self)
-
     def update(
         self,
         *,
         many=None,
-        atomic_type_name=None,
+        type=None,
         referenced_by=None,
         attr_attribute=None,
         exist=None,
+        unique=None,
+        nullable=None,
+        default=None,
     ):
         for varname in [
             "exist",
             "many",
-            "atomic_type_name",
+            "type",
+            "unique",
             "referenced_by",
             "attr_attribute",
+            "nullable",
+            "default",
         ]:
             var = locals()[varname]
             if var is not None:
                 attr = getattr(self, varname)
                 if attr is not None:
                     # attr not None and var not None! they must be the same
                     if var is not attr:
                         raise ValueError(
                             f"Trying to update {varname} but it's already set to {attr} "
                         )
                 else:
                     setattr(self, varname, var)
 
+    def print(self):
+        print_str = f"\t{self.name}: "
+        if self.many:
+            print_str += "List["
+        print_str += f"{self.type}"
+        if self.many:
+            print_str += "]"
+
+        if self.unique:
+            print_str += " [unique]"
+        if self.nullable:
+            print_str += " [nullable]"
+        if self.referenced_by:
+            print_str += f" [{self.referenced_by}]"
+        if self.exist:
+            print_str += " [exists]"
+        coloring.print_bblue_violet(print_str)
 
-@attr.s
-class BuildingClass:
-    """Helper class to postpone building the ORM classes"""
 
-    name: str = attr.ib()
+@attr.s
+class TableMetadata:
+    """Helper class to postpone building the ORM classes
+    Contains all information about a table (name, indexes, ..., ...)"""
+
+    # cls_name is the only information that we always know
+    #   either we have it before decorating with @db.table
+    #   or it's name is referenced as an annotation in a column
+    cls_name: str = attr.ib()
+    table_name: str = attr.ib(default=None)  # tablename
     cls = attr.ib(default=None, init=False)
-    table_name: str = attr.ib(default=None, init=False)
-    attributes: typing.Dict[str, BuildingRelationalAttribute] = attr.ib(
-        factory=dict, init=False
-    )
+    columns: typing.Dict[str, ColumnMetadata] = attr.ib(factory=dict, init=False)
     orm_cls = attr.ib(default=None, init=False)
     # this attribute is set to True by the class that contain this
     #  attribute, sins it is possible for an other class to create
     #  an attribute with ref (having exist=True we are sure that
     #  the attribute exist and it's not just a reference)
     exist = attr.ib(default=None)
 
@@ -124,83 +168,104 @@
                     if var is not attr:
                         raise ValueError(
                             f"Trying to update {varname} but it's already set to {attr} "
                         )
                 else:
                     setattr(self, varname, var)
 
-    def get_or_create_attribute(
-        self, attribute_name: str
-    ) -> BuildingRelationalAttribute:
-        if attribute_name in self.attributes:
-            return self.attributes[attribute_name]
+    def print(self):
+        coloring.print_bblue(f"Table: {self.table_name} - {self.cls_name}")
+        for column in self.columns.values():
+            column.print()
+
+    def get_or_create_column(self, attribute_name: str) -> ColumnMetadata:
+        if attribute_name in self.columns:
+            return self.columns[attribute_name]
         else:
-            attribute = BuildingRelationalAttribute(attribute_name)
-            self.attributes[attribute_name] = attribute
+            attribute = ColumnMetadata(attribute_name)
+            self.columns[attribute_name] = attribute
             return attribute
 
 
-@attr.s
-class AttributeMetadata:
-    """Additional metadata to attr (use sqlalchemy attributes and RelatinalDB attributes)"""
-
-    unique: bool = attr.ib(default=None, kw_only=True)
-
-
 class RelationalDB:
     # TODO: add a new engine which is dict in contrast to SQLalchemy
     # it will have the same API, but it will store the classes
     # in memory with list and dicts and don't use SQL
     # TODO: add bijection argument (for friends, to add the same line twice)
     # TODO: add List of strings List[str] => and add a table with a foreign key
+    #   Ex: tags: List[str]  -> create table users_tags id_tag
     # TODO: use only annotation without db.attribute(): Ex: name: str  (like dataclass)
     # TODO: add the possibility ti use @db.table  and take the name cls.__name__
     # TODO: implement  lazy import
-    _map_cls_to_sqlalchemy_types = {str: String, int: Integer, bool: Boolean}
+    _map_cls_to_sqlalchemy_types = {
+        str: sqlalchemy.String,
+        int: sqlalchemy.Integer,
+        bool: sqlalchemy.Boolean,
+        datetime: sqlalchemy.DateTime,
+    }
     List = typing.List
 
     def __init__(self, uri: str = None, echo=None, autocommit=None):
+        """
+        RelationalDB is an aditional layer of abstration for relationaldb ORMs
+        This class is based on SQLAlchemy and attrs modules
+
+        Algorithm:
+            - Gather information for tables (table) and columns (attributes)
+              - add hook in init for each table/class to be able to autocommit
+            - call init() to built SQLAlchemy classes based on the gathered information
+
+        Global constraints:
+            - Mapped classes (with tables) must have unique names
+        """
         if uri is None:
             uri = ":memory:"
 
         if echo is None:
             echo = False
 
         if autocommit is None:
             autocommit = True
 
         self.uri = uri
         self.autocommit = autocommit
+        self.debug = echo
 
         # internal attributes
+        # FIXME: remove one of the three mapping
         self._map_cls_tablename = {}
         self._map_tablename_cls = {}
-        self._map_clsname_tablename = {}
 
         # sqlalchemy attributes
         self.engine = create_engine(f"sqlite:///{uri}", echo=echo)
         self.Session = sessionmaker(bind=self.engine)
         self.Base = declarative_base()
 
         # dictionary to hold classes to build at init()
-        self._building_class: typing.Dict[str, BuildingClass] = {}
+        self._clsname_to_table_metadata: typing.Dict[str, TableMetadata] = {}
 
     @property
     def query(self):
         return self.session.query
 
     @property
     def commit(self):
         return self.session.commit
 
-    datetime_now = datetime.datetime.utcnow
+    datetime_now = datetime.utcnow
+
+    def metadata(self, unique=None, nullable=None, target=None, ref=None):
+        if unique is None:
+            unique = False
+
+        if nullable is None:
+            nullable = False
 
-    def metadata(self, unique=True, nullable=False, target=None, ref=None):
         return {
-            "koala": {
+            "koalak": {
                 "unique": unique,
                 "nullable": nullable,
                 "target": target,
                 "ref": ref,
             }
         }
 
@@ -224,32 +289,33 @@
         on_setattr=None,
         # sqlalchemy attribute
         unique=None,
         nullable=None,
         target=None,
         ref=None,
     ):
-
         # check integrity of arguments
+
         if not nullable and default is None:
             assert TypeError(
                 f"An attribute can't be 'not nullable' and default is None in the same time"
             )
+
         # if default is None activate nullable to True by default
         if default is None and nullable is None:
             nullable = True
 
         if metadata is None:
             metadata = {}
         if nullable is None:
             nullable = False
         metadata.update(
             self.metadata(unique=unique, target=target, nullable=nullable, ref=ref)
         )
-        return attr.ib(  # noqa
+        attrib = attr.ib(  # noqa
             default=default,
             validator=validator,
             repr=repr,
             cmp=cmp,
             hash=hash,
             init=init,
             metadata=metadata,
@@ -257,345 +323,363 @@
             converter=converter,
             factory=factory,
             kw_only=kw_only,
             eq=eq,
             order=order,
             on_setattr=on_setattr,
         )
+        self.log(f"\tParsing attrib {attrib}")
+        coloring.print_red("metadata", attrib.metadata)
+        return attrib
+
+    def log(self, *args, **kwargs):
+        if self.debug:
+            print("[DEBUG]", *args, **kwargs)
 
     def table(self, table_name):
         """Create new table
-        How it works:
-        - Decorate the cls with attr to create the used methods (__init__, __repr__, ...)
-        - Hook the __init__ for autoadd
+
+        Algorithm:
+        This will only add metadata to create the table at init()
+        - Decorate the cls with attr module to create the used methods (__init__, __repr__, ...)
+        - Hook the __init__ for autocommit (so the class will add itself to session)
         - collect all needed information for relations (to add in init())
         - Create the sqlalchemy ORM cls that inherit from the original cls and the Base cls
          without the relations (relations will be added in init())
         - Return the ORM cls
         """
+        self.log(f"Creating table {table_name}")
+        self.print()
 
         def decorator(cls):
             """Register this class to build it when init() is called"""
+            # This code is executed after attr.ib and db.attribute constructions
             # check if cls name is unique
             cls_name = cls.__name__
-            if cls_name in self._building_class:
-                assert KeyError(f"Class {cls_name} already exist in the database")
+            table_metadata = self._get_or_create_table_metadata_by_clsname(cls_name)
+            table_metadata.update(table_name=table_name, cls=cls)
+
+            # TODO: check if cls exists
+            # if cls_name in self._clsname_to_table_metadata:
+            #    assert KeyError(f"Table with cls name {cls_name} already exists")
 
             # ======================================= #
             # decorate cls with attr (if not already) #
             # ======================================= #
             if not hasattr(cls, "__attrs_attrs__"):
+                # If columns are created with attr.ib and not db.attribute we add koalak metadata
+                # We have to create it here, before attr.s parse the attr.ib instances
+                for e in cls.__dict__.values():
+                    if not isinstance(e, AttribType):
+                        continue
+                    if "koalak" not in e.metadata:
+                        e.metadata["koalak"] = self.metadata()["koalak"]
+                    # FIXME: check if attr.ib and db.attribute are coherant
+
+                # Apply attr
                 cls = attr.s(cls)
+            else:
+                raise ValueError(
+                    f"Class {cls.__name__} must not be decorated with attr.s use db.table instead!"
+                )
 
             # ========================================== #
             # hook __init__ to add autocommit if enabled #
             # ========================================== #
             def postinit_autocommit(self_instance):
                 if self.autocommit:
                     self.session.add(self_instance)
                     # self.session.commit()
 
             # add postinit_autocommit to the cls
             cls = add_post_init(postinit_autocommit)(cls)
 
             # register cls and it's attributes
-            orm_cls = self._create_orm_cls_without_relations(cls, table_name)
+            # orm_cls = self._create_orm_cls_without_relations(cls, table_name)
+            self._add_table_metadata(cls, table_name)
             # building_cls = self._register_cls(cls, table_name)
 
-            return orm_cls
+            return cls
 
         return decorator
 
-    def _get_or_create_building_cls(self, cls_name: str) -> BuildingClass:
-        if cls_name in self._building_class:
-            return self._building_class[cls_name]
+    def print(self):
+        print("<----------BEGIN-------->")
+        for table in self._clsname_to_table_metadata.values():
+            table.print()
+            print()
+        print("<----------END-------->")
+
+    def _get_or_create_table_metadata_by_clsname(self, cls_name: str) -> TableMetadata:
+        if cls_name in self._clsname_to_table_metadata:
+            return self._clsname_to_table_metadata[cls_name]
         else:
-            building_cls = BuildingClass(cls_name)
-            self._building_class[cls_name] = building_cls
-            return building_cls
+            table_metadata = TableMetadata(cls_name)
+            self._clsname_to_table_metadata[cls_name] = table_metadata
+            return table_metadata
 
-    def _create_orm_cls_without_relations(self, cls, table_name):
-        """Create the ORM cls without relations. Relations will be added at init()"""
-
-        cls_name = cls.__name__
+    def _add_table_metadata(self, cls, table_name):
+        """Create the ORM cls without relations. Relations will be added when init() is called"""
 
         # get the building_class for this class
-        building_cls = self._get_or_create_building_cls(cls_name)
-        building_cls.update(cls=cls, table_name=table_name, exist=True)
+        cls_name = cls.__name__
+        table_metadata = self._get_or_create_table_metadata_by_clsname(cls_name)
+        table_metadata.update(exist=True)
 
-        building_attributes = building_cls.attributes
+        columns_metadata = table_metadata.columns
         attr_attributes = getattr(cls, "__attrs_attrs__")
-        sqlalchemy_attributes = {
+        """sqlalchemy_attributes = {
             "__tablename__": table_name,
             # Automatically add id
             "id": Column(Integer, primary_key=True),
-        }
+        }"""
 
         for attr_attribute in attr_attributes:
+            metadata = attr_attribute.metadata["koalak"]
+            if attr_attribute.default is None:
+                pass
+            coloring.print_green("attr", attr_attribute)
+            attribute_name = attr_attribute.name
 
-            # arguments for sqlalchemy.Column
-            logger.debug("attr_attribute %s", attr_attribute)
-            logger.debug("map tablename cls %s", self._map_tablename_cls)
-            logger.debug("map cls tablename %s", self._map_cls_tablename)
+            column_metadata = table_metadata.get_or_create_column(attribute_name)
 
-            attribute_name = attr_attribute.name
-            coloring.print_bgreen("Attribute", cls.__name__, attribute_name)
-            sqlalchemy_type = None
-            args = []
-            kwargs = {}
-            metadata = attr_attribute.metadata["koala"]
+            column_metadata.update(
+                unique=metadata["unique"], nullable=metadata["nullable"]
+            )
             # Get sqlalchemy column type
             attr_type = attr_attribute.type
-            if attribute_name == "age":
-                coloring.print_bred("Age here")
+            """
+            We can have the following types:
+            - Simple types (builtin)
+                - SQLAlchemy cls -> do nothing
+                - Known builtin type (int, float, bool, str, datetime) -> convert to SQLAlchemy cls
+            - Complicated types (relationship with other tables)
+                - Cls already present in our tables (cls already decorated with @db.table)
+                - Str -> convert it to cls in our table
+                - List["str"] or List[cls], many relation with the cls
+            - Else error!
+            """
+            self.print()
 
-            if isinstance(attr_type, sqlalchemy.sql.visitors.VisitableType):
+            if isinstance(attr_type, type(sqlalchemy.String)):
                 # sqlalchemy type (Integer, String, ...)
-                sqlalchemy_type = attr_type
-                print("in if")
+                column_metadata.update(type=attr_type, many=False)
             elif attr_type in self._map_cls_to_sqlalchemy_types:
-                print("in elif")
                 # convert builtin types  (int, str, bool, ...)
                 sqlalchemy_type = self._map_cls_to_sqlalchemy_types[attr_attribute.type]
-            else:
-                print("in else")
-                self._register_building_attribute(building_cls, attr_attribute)
-                # The type is a an other table, we don't build it now we juste
-                # collect information about it, to built it at init()
-                if isinstance(attr_type, str):
-                    # name of the cls
-                    clsname_type = attr_type
-                else:  # attr_type is ORM cls
-                    # cls_type = attr_type
-                    clsname_type = attr_type.__name__
-
-                del attr_type  # to avoid errors
+                column_metadata.update(type=attr_type, many=False)
+            elif isinstance(attr_type, (str, type(typing.List))) or (
+                isinstance(attr_type, type)
+                and attr_type.__name__ in self._clsname_to_table_metadata
+            ):
+                # Complicated type implying relations (one to many, many to many, one to one, ...)
+                self._add_relational_column(table_metadata, attr_attribute)
 
                 # check it cls type is the same as this cls
                 # if so, nullable must be True! (otherwise it's impossible to instantiate the object)
                 # TODO: move the check in _register_building_attribute?
-                if clsname_type == cls.__name__:
+                """if clsname_type == cls.__name__:
                     if not metadata["nullable"]:
                         # TODO: test this case (tell Yassmine?)
                         raise ValueError(
                             f"Attribute {attr_attribute.name!r} must be nullable when "
                             f"it's type is referencing to the same class ({cls.__name__!r})"
                         )
+                continue"""
+            else:
+                raise TypeError(f"Unknown type for attribute {attr_type}")
 
-                # Don't build anything, init() will build all the relations
-                continue
-
+            # table_metadata.get_or_create_column("")
             # Build kwargs
-
-            kwargs["unique"] = metadata["unique"]
-            kwargs["nullable"] = metadata["nullable"]
-            coloring.print_bmagenta("building column for", cls_name)
-            print("name", attribute_name)
-            print("type", sqlalchemy_type)
-            print("args", args)
-            print("kwargs", kwargs)
-            print()
+            # kwargs["unique"] = metadata["unique"]
+            # kwargs["nullable"] = metadata["nullable"]
             # Create the Column
-            sqlalchemy_attributes[attribute_name] = Column(
-                sqlalchemy_type, *args, **kwargs
-            )
-            if attribute_name == "age":
-                coloring.print_bred("finish building age collumn")
+            # sqlalchemy_attributes[attribute_name] = Column(
+            #     sqlalchemy_type, *args, **kwargs
+        #  )
+
         # sqlalchemy_attributes.update(sqlalchemy_attributes_later)
-        coloring.bblue("sqlalchemy attributes")
-        print(sqlalchemy_attributes)
         # ORM cls inherit from the decorated cls and self.Base
-        OrmCls = type(cls.__name__, (cls, self.Base), sqlalchemy_attributes)
+        # OrmCls = type(cls.__name__, (cls, self.Base), sqlalchemy_attributes)
         # ============================================================= #
         # Create a new cls that inherit from Base and the decorated cls #
         # ============================================================= #
-        self._map_tablename_cls[table_name] = OrmCls
-        self._map_cls_tablename[OrmCls] = table_name
+        # self._map_tablename_cls[table_name] = OrmCls
+        # self._map_cls_tablename[OrmCls] = table_name
 
-        building_cls.update(orm_cls=OrmCls)
-        return OrmCls
+        # table_metadata.update(orm_cls=OrmCls)
+        # return OrmCls
 
-    def _register_building_attribute(
-        self, cls_building: BuildingClass, attr_attribute
-    ) -> BuildingRelationalAttribute:
-        """Register an attribute"""
-
-        attr_name = attr_attribute.name
+    def _add_relational_column(
+        self, table_metadata: TableMetadata, attr_attribute
+    ) -> ColumnMetadata:
+        """Register a relational attribute (str or isinstance(type(List)) or cls"""
+        coloring.print_green(
+            "Adding relational attribute",
+            repr(table_metadata.table_name),
+            attr_attribute,
+        )
+        column_name = attr_attribute.name
         attr_type = attr_attribute.type
-        metadata = attr_attribute.metadata["koala"]
-        cls = cls_building.cls
+
+        # If it's a known Column class, get its name
+        if (
+            isinstance(attr_type, type)
+            and attr_type.__name__ in self._clsname_to_table_metadata
+        ):
+            attr_type = attr_type.__name__
+
+        metadata = attr_attribute.metadata["koalak"]
+
+        cls = table_metadata.cls
         cls_name = cls.__name__
-        building_attributes = cls_building.attributes
-        building_attribute = cls_building.get_or_create_attribute(attr_name)
-        building_attribute.update(attr_attribute=attr_attribute)
-        building_attribute.update(exist=True)
+        column_metadata = table_metadata.get_or_create_column(column_name)
+        column_metadata.update(attr_attribute=attr_attribute)
+        column_metadata.update(exist=True)
         # check if the attribute is typing.List to use a "many" relationship
-        many = False
-        if isinstance(attr_type, typing.GenericMeta):
-            if attr_type.__name__ == "List":
-                many = True
-                # check if List is empty (ex: List instead of List[Animal])
-                if not attr_type.__args__:  # noqa
-                    raise ValueError(
-                        f"List annotation for {cls_name}.{attr_name} can not be empty"
-                    )
-                attr_type = attr_type.__args__[0]  # noqa
 
-                # Check if the argument of List is a string
-                if isinstance(attr_type, typping_ForwardRef):
-                    attr_type = attr_type.__forward_arg__
-            else:
+        many = False
+        if isinstance(attr_type, type(typing.List)):
+            parsed_type = parse_typing_type(attr_type)
+            attr_type_type = parsed_type["type"]
+            if attr_type_type != "List":
                 raise ValueError(
                     f"Support only List annotation, don't support {attr_type}"
                 )
-        if not isinstance(attr_type, str):
-            attr_type = attr_type.__name__
-        atomic_type = attr_type
 
-        building_attribute.update(many=many, atomic_type_name=atomic_type)
+            many = True
+            attr_type = parsed_type["name"]  # noqa
 
+        atomic_type = attr_type
+        print("whoop", column_metadata)
+        column_metadata.print()
+        column_metadata.update(many=many, type=attr_type)
+        column_metadata.print()
         # build the ref_type if it doesn't exist
         ref_cls_name = atomic_type
-        ref_building_cls = self._get_or_create_building_cls(atomic_type)
+        ref_building_cls = self._get_or_create_table_metadata_by_clsname(atomic_type)
 
         # check if the attribute have a reference to an other one
         ref_attribute_name = metadata["ref"]
         if ref_attribute_name:
             # check: if the ref_class is already parsed check if ref attribute exist
             if ref_building_cls.exist:
                 # if ref_attribute_name not in
                 if (
-                    ref_attribute_name not in ref_building_cls.attributes
-                    or not ref_building_cls.attributes[ref_attribute_name].exist
+                    ref_attribute_name not in ref_building_cls.columns
+                    or not ref_building_cls.columns[ref_attribute_name].exist
                 ):
                     raise ValueError(
-                        f"{cls_building.name}.{attr_name} reference non existing attribute {ref_attribute_name}"
+                        f"{table_metadata.table_name}.{column_name} reference non existing attribute {ref_attribute_name}"
                     )
 
             # get the building_attribute
-            ref_building_attributes = ref_building_cls.attributes
-            building_attribute_ref = ref_building_cls.get_or_create_attribute(
+            ref_building_attributes = ref_building_cls.columns
+            building_attribute_ref = ref_building_cls.get_or_create_column(
                 ref_attribute_name
             )
 
-            building_attribute_ref.update(atomic_type_name=cls_name)
-            building_attribute_ref.update(referenced_by=building_attribute)
+            building_attribute_ref.update(type=cls_name)
+            building_attribute_ref.update(referenced_by=column_metadata)
 
-            coloring.print_balice_blue("attribuuuuutes :'(")
             # Check if reference are consistent
             if building_attribute_ref.referenced_by:
-                coloring.print_balice_blue("attribuuuuutes")
-                print("this attribute", building_attribute)
-                print("ref attribute", building_attribute_ref)
                 # check that class is consistent
                 #  ex: If Person have an attributes List[Animal] animals, ref=owner
                 #  owner must be of type Person!
-                ref_attomic_type = building_attribute_ref.atomic_type_name
-                print("ref_attomic_type", ref_attomic_type)
+                ref_attomic_type = building_attribute_ref.type
                 if ref_attomic_type and ref_attomic_type != cls_name:
                     raise ValueError(
-                        f"{cls_name}.{attr_name} reference {ref_cls_name}.{ref_attribute_name}, but "
+                        f"{cls_name}.{column_name} reference {ref_cls_name}.{ref_attribute_name}, but "
                         f" {ref_cls_name}.{ref_attribute_name} reference {ref_attomic_type} class"
                     )
                 ref_referenced_by_name = building_attribute_ref.referenced_by.name
 
-                if ref_referenced_by_name != attr_name:
+                if ref_referenced_by_name != column_name:
                     raise ValueError(
-                        f"The {cls_name}.{attr_name} reference {ref_cls_name}.{ref_attribute_name}"
+                        f"The {cls_name}.{column_name} reference {ref_cls_name}.{ref_attribute_name}"
                         f" but {ref_cls_name}.{ref_attribute_name} "
                         f"reference {cls_name}.{ref_referenced_by_name}"
                     )
 
-        return building_attribute
+        return column_metadata
 
     def init(self):
+        self.print()
+        # Check classes!
+        for table_metadata in self._clsname_to_table_metadata.values():
+            for column_metadata in table_metadata.columns.values():
+                for attribute_name in ["many", "unique", "nullable", "type"]:
+                    attribute_value = getattr(column_metadata, attribute_name)
+                    if attribute_value is None:
+                        raise ProgrammingError(
+                            f"In column {table_metadata.table_name}.{column_metadata.name}"
+                            f" attribute {attribute_name!r} is None"
+                        )
+
         # construict classes
-        for cls_name in self._building_class:
+        for cls_name in self._clsname_to_table_metadata:
             self._build_orm_relations(cls_name)
 
         self.Base.metadata.create_all(self.engine)
         self.session = self.Session()
 
     def _build_orm_relations(self, cls_name: str):
-        buildingn_cls = self._building_class[cls_name]
+        buildingn_cls = self._clsname_to_table_metadata[cls_name]
         cls = buildingn_cls.cls
         orm_cls = buildingn_cls.orm_cls
-        print("ORM relations", buildingn_cls)
-        print()
-        for building_attribute in buildingn_cls.attributes.values():
+        for building_attribute in buildingn_cls.columns.values():
             # Check if the attribute exist or if it's referenced but don't exist
             if not building_attribute.exist:
                 referenced_by = building_attribute.referenced_by
                 assert ValueError(
                     f"Attribute {building_attribute.name} is referenced by {referenced_by.name} but don't exist"
                 )
-            print("Buildin attribute", building_attribute)
             attr_attribute = building_attribute.attr_attribute
-            print("metadataaaaaaaa                ", repr(attr_attribute))
-            print("METADATA", building_attribute.name, cls_name)
-            metadata = attr_attribute.metadata["koala"]
+            metadata = attr_attribute.metadata["koalak"]
             ref = metadata["ref"]
             many = building_attribute.many
             if not ref:
                 ref_many = True
             else:
                 ref_many = True
 
-            if not isinstance(building_attribute.atomic_type_name, str):
-                ref_type = building_attribute.atomic_type_name.__name__
+            if not isinstance(building_attribute.type, str):
+                ref_type = building_attribute.type._name
             else:
-                ref_type = building_attribute.atomic_type_name
-            ref_building_cls = self._building_class[ref_type]
+                ref_type = building_attribute.type
+            ref_building_cls = self._clsname_to_table_metadata[ref_type]
             if not many and ref_many:
                 # one to many relations
                 self._build_one_to_many_relation(
                     buildingn_cls, ref_building_cls, building_attribute.name
                 )
 
     def _build_one_to_many_relation(
         self,
-        one_cls: BuildingClass,
-        many_cls: BuildingClass,
+        one_cls: TableMetadata,
+        many_cls: TableMetadata,
         one_attribute_name,
         one_relation=True,
     ):
         # add the foreign_key in the one_cls side
-        coloring.print_bgreen("Adding one_to_many_relation")
-        print(
-            "Adding one_to_many_relation for",
-            one_cls.name,
-            "to",
-            many_cls.name,
-            "with attribute",
-            repr(one_attribute_name),
-        )
-        print("Foreing key column")
+
         many_cls_id = f"{many_cls.table_name}.id"
 
         foreign_key = Column(Integer, ForeignKey(many_cls_id))
         foreign_key_name = f"{one_attribute_name}_id"
-        print("foreingkey", foreign_key)
         setattr(one_cls.orm_cls, foreign_key_name, foreign_key)
 
         if one_relation:
-            coloring.print_bcyan("add forein key for ", many_cls.name)
-            print("cls", many_cls.name)
-            print("foreign_keys", f"{one_cls.name}.{foreign_key_name}")
-            print("attribute", one_attribute_name)
-            print("remote_side", many_cls.orm_cls.id)
-
             relation = sqlalchemy.orm.relationship(
                 many_cls.name,
                 remote_side=many_cls.orm_cls.id,
                 foreign_keys=f"{one_cls.name}.{foreign_key_name}",
             )
             setattr(one_cls.orm_cls, one_attribute_name, relation)
-            # print(coloring.bred("relation"), one_cls.orm_cls, one_attribute_name, relation)
-
-        print("\n")
 
     def first(self, table, **kwargs):
         if isinstance(table, str):
             table = self._map_tablename_cls[table]
         return self.session.query(table).filter_by(**kwargs).first()
 
     def close(self):
@@ -608,10 +692,10 @@
         pass
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.commit()
 
 
 def relationaldb(
-    uri: str = None, *, echo: bool = None, autocommit: bool = None
+    uri: str = None, *, debug: bool = None, autocommit: bool = None
 ) -> RelationalDB:
-    return RelationalDB(uri, echo=echo, autocommit=autocommit)
+    return RelationalDB(uri, echo=debug, autocommit=autocommit)
```

### Comparing `koalak-0.2.9/src/koalak/decorators.py` & `koalak-0.3.1/src/koalak/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 
     # TODO: check that when creating an init (cls don't have one)
     # we create a init with a simple signature not *args, **kwargs
     names: in the cls class (TODO: change it in a namespace for this package)
         - __inits__
         - __post_inits__
     """
+
     # TODO: support multiple functions at once *init_functions
     def decorator(cls):
         if not hasattr(cls, "__inits__"):
             # create a new __init__
             dispatcher__init__ = factory_dispatcher__init__(cls)
             # replace the original __init__ by the dispathcer__init__
             cls.__inits__ = [cls.__init__]
@@ -331,15 +332,15 @@
         firstarg,
     )
 
     obj_is_method = is_future_method(decorator_to_decorate)
 
     def _refactored(obj_or_arg, args, kwargs, self=None):
         pre_args = []
-        if self:
+        if self is not None:  # this was if self and I took 3 hours to debug it!
             pre_args.append(self)
 
         # There are 3 possibility for the first argument
         #  None => decorator called with brackets =>
         if obj_or_arg is None or (
             firstarg is not None and isinstance(obj_or_arg, firstarg)
         ):
```

### Comparing `koalak-0.2.9/src/koalak/fixtures.py` & `koalak-0.3.1/src/koalak/_workinprogress/fixtures.py`

 * *Files identical despite different names*

### Comparing `koalak-0.2.9/src/koalak/frameworks/home_structure.py` & `koalak-0.3.1/src/koalak/frameworks/home_structure.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """These classes are here to create the home_structure when initiating a new framework
 
 """
 import os
 from string import Template
 from typing import Any, Dict, List, Union
 
-import attr
+import attrs
 
 """
 Functions to create directory (and files) structure easily
 
 see also:
 - https://stackoverflow.com/questions/26288551/render-json-to-directory-structure-in-python
 
@@ -36,34 +36,32 @@
         return actions
     else:
         raise TypeError(
             f"actions must be of type 'str' or {FileAction.__name__!r} or list"
         )
 
 
-@attr.s
+@attrs.define
 class FileDescription:
     """Used to describe file to create the home structure"""
 
-    name = attr.ib()
-    src = attr.ib(default=None)
-    content = attr.ib(default="")
-    substitute = attr.ib(default=False)
-    actions = attr.ib(
-        default=attr.Factory(list), converter=_file_description_action_converter
-    )
+    name = attrs.field()
+    src = attrs.field(default=None)
+    content = attrs.field(default="")
+    substitute = attrs.field(default=False)
+    actions = attrs.field(factory=list, converter=_file_description_action_converter)
 
 
-@attr.s
+@attrs.define
 class NormalizedFile:
     """Normalize FileDescription"""
 
-    path = attr.ib()
-    content = attr.ib()
-    framework = attr.ib()
+    path = attrs.field()
+    content = attrs.field()
+    framework = attrs.field()
 
 
 def normalize_file_description(
     file_description: FileDescription, parent_path, framework
 ):
     # FIXME: handle the case of big files (copy by chunk)? and test it
     # FIXME: when we have a source file? do we need to copy the permissions?
@@ -79,20 +77,20 @@
     if file_description.substitute:
         content = framework.substitute_string(content)
 
     path = os.path.join(parent_path, file_description.name)
     return NormalizedFile(path, content, framework)
 
 
-@attr.s
+@attrs.define
 class DirectoryDescription:
     """Used to describe directory to create the home structure"""
 
-    name = attr.ib()
-    nodes = attr.ib(default=attr.Factory(list))
+    name = attrs.field()
+    nodes = attrs.field(factory=list)
 
 
 # ======= #
 # ACTIONS #
 # ======= #
 
 
@@ -130,15 +128,14 @@
     def _get_add_to_bashrc(self, file: NormalizedFile):
         basename = os.path.basename(file.path)
         return self._add_to_bashrc_template.format(
             basename=basename, path=file.path, framework_name=file.framework.name
         )
 
     def after_normalize(self, file: NormalizedFile):
-
         with open(self.bashrcpath) as f:
             bashrc = f.read()
 
         add_to_bashrc = self._get_add_to_bashrc(file)
 
         if add_to_bashrc not in bashrc:
             with open(self.bashrcpath, "a") as f:
```

### Comparing `koalak-0.2.9/src/koalak/helpers/argparse_helper.py` & `koalak-0.3.1/src/koalak/_deprecated/argparse_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import inspect
 import sys
 import typing
 import warnings
 
+import argcomplete
 import coloring
 
 
 class ArgparseSubcmdHelper:
     """argparse class Helper for making subcommands easily
     To add a subcommand x implement the following methods/attributes
         def parser_x(self, parser): add arguments to the subcommand parser
@@ -28,14 +29,15 @@
 
 
     """
 
     prog = None
     description = None
     groups = None  # FIXME: not yet correctly implemented/tested
+    autocomplete = False
 
     # TODO: add a way to have an optional subcm (dont thtrow and error when called withotu subcmd)
     # TODO: improve the custom help! and test it
     def _parser_main(self, parser):
         """Hook to add arguments to the main parser (general arguments)"""
         pass
 
@@ -48,15 +50,16 @@
         # FIXME: imlement/test me
         if not self.groups:
             return
         SPACES = "    "
         color_help = getattr(self, "color_help", False)
         # header prog name and description
         prog = self.prog or sys.argv[0]
-        help = f"usage: {prog} [-h] <subcommand>\n\n"
+        help = getattr(self, "prolog", "")
+        help += f"usage: {prog} [-h] <subcommand>\n\n"
 
         if self.description:
             help += f"{self.description}\n\n"
 
         # get the longest command name for pretty print with tabulations
         # flatten all commands names in self.groups()
         grouped_commands_name = [
@@ -95,15 +98,15 @@
                     raise TypeError(
                         f"Command {cmd!r} can't be in a group because it don't exist (consider implementing 'run_{cmd}')"
                     )
                 description_command = getattr(self, f"description_{cmd}", "")
                 cmd_txt = cmd.ljust(max_command_length)
                 if color_help:
                     cmd_txt = coloring.colorize(cmd_txt, c="medium_purple")
-                help += f"{SPACES}{cmd_txt}{SPACES} {description_command}\n"
+                help += f"{SPACES}{cmd_txt}{SPACES}{description_command}\n"
             help += "\n"
 
         # change the help function
         self.parser.print_help = lambda file=None: print(help, file=file)
         # self.main_parser.print_usage = self.main_parser.print_help
 
     def __init__(self, parser=None, subcommand_depth=1):
@@ -189,18 +192,23 @@
             )
             subcommand = subcommand_cls(
                 parser=subcmd_parser, subcommand_depth=self.subcommand_depth + 1
             )
             setattr(self, f"_instance_command_{subcommand_name}", subcommand)
 
     def parse_args(self, args=None):
+        if self.autocomplete:
+            argcomplete.autocomplete(self.parser)
+
         return self.parser.parse_args(args)
 
     def run(self, args=None):
         """Run the main program"""
+        if self.autocomplete:
+            argcomplete.autocomplete(self.parser)
         parsed_args = self.parser.parse_args(args)
         self._run_main(parsed_args)  # hook to _run_main
         self._run(self, parsed_args)
 
     def _run(self, command, parsed_args, depth=1):
         """Search the subfunction to run recursivly"""
         if depth == 1:
@@ -221,11 +229,11 @@
                 command, f"_instance_command_{subcommand_name}"
             )
             self._run(subcommand_instance, parsed_args, depth + 1)
 
     def main(self, *args, **kwargs):
         """Deprecated run method"""
         warnings.warn(
-            "main will be deprecated in future version, use run instead",
+            "main will be _deprecated in future version, use run instead",
             PendingDeprecationWarning,
         )
         self.run(*args, **kwargs)
```

### Comparing `koalak-0.2.9/src/koalak.egg-info/PKG-INFO` & `koalak-0.3.1/src/koalak.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: koalak
-Version: 0.2.9
+Version: 0.3.1
 Summary: Framework manager, framework to create frameworks
 Home-page: https://github.com/nazime/koalak
 Author: Nazime LAKEHAL
 Author-email: nazime.lkh@gmail.com
 Maintainer: Nazime LAKEHAL
 Maintainer-email: nazime.lkh@gmail.com
 License: MIT
 Project-URL: Documentation, https://koalak.readthedocs.org/
 Project-URL: Bug Tracker, https://github.com/nazime/koalak/issues
 Project-URL: Source Code, https://github.com/nazime/koalak
 Description: # Koalak
         
-        Koalak is a collections of tools that helps me create my libraries, the library focus on creating plugins architectures. The project is currently under development, I shared the repository because it is used by my tool **wordlistools**.
+        Koalak is a collections of tools that helps me create my libraries, the library focus on creating plugins architectures.
+        The project is currently under development, I shared the repository because it is used by my tool **wordlistools**.
         
         Koala features
         
-        - Manage plugins for your project
-        - Allow you to create new plugins from project home directory
+        - Manage plugins for your project, more information on the wiki.
+        - Argparse wrapper to create CLI interfaces with subcommands easily
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tests
+Provides-Extra: dev
 Provides-Extra: travis
```

### Comparing `koalak-0.2.9/tests/noatest_decorators_addinit.py` & `koalak-0.3.1/tests/test_unsorted/noatest_decorators_addinit.py`

 * *Files identical despite different names*

### Comparing `koalak-0.2.9/tests/noptest_databases/test_dict_db.py` & `koalak-0.3.1/tests/test_useless/noptest_databases/test_dict_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tempfile
 
 import pytest
 from koalak.databases import JsonDictDB, TxtDictDB
-from koalak.helpers_test import HelperTestDictDB
+from koalak.databases.helper_tests import HelperTestDictDB
 from koalak.utils import temp_pathname
 
 
 # ---------------- TEST JsonDictDB --------------- #
 def test_jsondictdb_with_helper():
     HelperTestDictDB(JsonDictDB).test()
```

### Comparing `koalak-0.2.9/tests/noptest_databases/test_list_database.py` & `koalak-0.3.1/tests/test_useless/noptest_databases/test_list_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tempfile
 
 import pytest
 from koalak.databases import JsonListDB, TxtListDB
-from koalak.helpers_test import HelperTestListDatabase
+from koalak.databases.helper_tests import HelperTestListDatabase
 from koalak.utils import temp_pathname
 
 
 # ---------------- TEST ListJsonDatabase --------------- #
 def test_with_helper_json_db():
     HelperTestListDatabase(JsonListDB).test()
```

### Comparing `koalak-0.2.9/tests/test_decorators/atest_decorators_addinit.py` & `koalak-0.3.1/tests/test_decorators/atest_decorators_addinit.py`

 * *Files identical despite different names*

### Comparing `koalak-0.2.9/tests/test_decorators/test_add_postinit.py` & `koalak-0.3.1/tests/test_decorators/test_add_postinit.py`

 * *Files identical despite different names*

### Comparing `koalak-0.2.9/tests/test_decorators/test_optionalargs.py` & `koalak-0.3.1/tests/test_decorators/test_optionalargs.py`

 * *Files 23% similar despite different names*

```diff
@@ -178,14 +178,100 @@
     @d.add_attr(value=10)
     class D:
         pass
 
     assert D.x == 10
 
 
+def test_optionalargs_method_in_cls_with_firstarg():
+    class Decorator:
+        @optionalargs(firstarg=str)
+        def add_attr(self, obj, attr="x", value=5):
+            setattr(obj, attr, value)
+            return obj
+
+    d = Decorator()
+
+    @d.add_attr()
+    class A:
+        pass
+
+    assert A.x == 5
+
+    @d.add_attr
+    class B:
+        pass
+
+    assert B.x == 5
+
+    @d.add_attr(attr="y")
+    class C:
+        pass
+
+    assert C.y == 5
+
+    @d.add_attr(value=10)
+    class D:
+        pass
+
+    assert D.x == 10
+
+    @d.add_attr("z", value=10)
+    class D:
+        pass
+
+    assert D.z == 10
+
+
+def test_optionalargs_method_in_cls_with_firstarg_when_cls_have_methods():
+    # This is a test to avoid retrograding (I had the bug)
+    class Decorator:
+        # when having __len__ return 0 object will evaluate to false
+        # and will bug if we test without "is not None"
+        def __len__(self):
+            return 0
+
+        @optionalargs(firstarg=str)
+        def add_attr(self, obj, attr="x", value=5):
+            setattr(obj, attr, value)
+            return obj
+
+    d = Decorator()
+
+    @d.add_attr()
+    class A:
+        pass
+
+    assert A.x == 5
+
+    @d.add_attr
+    class B:
+        pass
+
+    assert B.x == 5
+
+    @d.add_attr(attr="y")
+    class C:
+        pass
+
+    assert C.y == 5
+
+    @d.add_attr(value=10)
+    class D:
+        pass
+
+    assert D.x == 10
+
+    @d.add_attr("z", value=10)
+    class D:
+        pass
+
+    assert D.z == 10
+
+
 def test_optionalargs_modifying_function():
     @optionalargs
     def add_x_to_result(func, x=1):
         @functools.wraps(func)
         def _func(*args, **kwargs):
             result = func(*args, **kwargs)
             return result + x
```

### Comparing `koalak-0.2.9/tests/test_file_actions/test_bashrc.py` & `koalak-0.3.1/tests/test_framework/test_file_actions/test_bashrc.py`

 * *Files identical despite different names*

### Comparing `koalak-0.2.9/tests/test_framework/test_db_in_framework.py` & `koalak-0.3.1/tests/test_framework/test_db_in_framework.py`

 * *Files identical despite different names*

### Comparing `koalak-0.2.9/tests/test_framework/test_framework.py` & `koalak-0.3.1/tests/test_framework/test_framework.py`

 * *Files identical despite different names*

### Comparing `koalak-0.2.9/tests/test_framework/test_variables.py` & `koalak-0.3.1/tests/test_framework/test_variables.py`

 * *Files identical despite different names*

### Comparing `koalak-0.2.9/tests/test_framework_manager.py` & `koalak-0.3.1/tests/test_framework/test_framework_manager.py`

 * *Files identical despite different names*

### Comparing `koalak-0.2.9/tests/test_helpers/test_argparse_helper.py` & `koalak-0.3.1/tests/test_deprecated/test_argparse_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 import shlex
 
 import pytest
-from koalak import ArgparseSubcmdHelper
+from koalak._deprecated.argparse_helper import ArgparseSubcmdHelper
 
 
 def test_run_cmd(capsys):
     class SimpleCommand(ArgparseSubcmdHelper):
         def parser_mycmd(self, parser):
             pass
```

### Comparing `koalak-0.2.9/tests/test_hooks.py` & `koalak-0.3.1/tests/test_deprecated/test_hooks.py`

 * *Files identical despite different names*

### Comparing `koalak-0.2.9/tests/test_init_home.py` & `koalak-0.3.1/tests/test_unsorted/test_init_home.py`

 * *Files identical despite different names*

### Comparing `koalak-0.2.9/tests/test_simple.py` & `koalak-0.3.1/tests/test_framework/test_simple.py`

 * *Files identical despite different names*

