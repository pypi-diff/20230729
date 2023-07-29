# Comparing `tmp/msumastro-1.2.4.tar.gz` & `tmp/msumastro-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msumastro-1.2.4.tar", last modified: Thu May 25 21:36:41 2023, max compression
+gzip compressed data, was "msumastro-1.2.5.tar", last modified: Sat Jul 29 17:32:49 2023, max compression
```

## Comparing `msumastro-1.2.4.tar` & `msumastro-1.2.5.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.599059 msumastro-1.2.4/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       35 2022-04-01 18:50:53.000000 msumastro-1.2.4/.gitattributes
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      187 2023-05-25 21:23:47.000000 msumastro-1.2.4/.gitignore
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      143 2022-04-01 18:50:53.000000 msumastro-1.2.4/.readthedocs.yml
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1254 2022-04-01 18:50:53.000000 msumastro-1.2.4/.travis.yml
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1573 2022-04-01 18:50:53.000000 msumastro-1.2.4/LICENSE.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      125 2022-04-01 18:50:53.000000 msumastro-1.2.4/MANIFEST.in
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      612 2023-05-25 21:36:41.599248 msumastro-1.2.4/PKG-INFO
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      976 2022-04-01 18:50:53.000000 msumastro-1.2.4/README.rst
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.552060 msumastro-1.2.4/docs/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4658 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/Makefile
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.540445 msumastro-1.2.4/docs/_templates/
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.553553 msumastro-1.2.4/docs/_templates/autosummary/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       42 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/_templates/autosummary/base.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       43 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/_templates/autosummary/class.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       44 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/_templates/autosummary/module.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7761 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/conf.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.554084 msumastro-1.2.4/docs/header_processing/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      772 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/header_processing/index.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      478 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/index.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4186 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/installation.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2099 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/overview.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       53 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/rtd-pip-requirements
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.555711 msumastro-1.2.4/docs/scripts/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    10924 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/scripts/automated_scripts.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2665 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/scripts/manual_processing.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     3825 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/scripts/scripts.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       55 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/xref.rst
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.557714 msumastro-1.2.4/msumastro/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       34 2023-05-25 21:23:47.000000 msumastro-1.2.4/msumastro/__init__.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5135 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/conftest.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2814 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/customlogger.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.564090 msumastro-1.2.4/msumastro/header_processing/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      150 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/header_processing/__init__.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    15954 2023-05-25 21:23:47.000000 msumastro-1.2.4/msumastro/header_processing/astrometry.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    18704 2023-05-25 21:27:40.000000 msumastro-1.2.4/msumastro/header_processing/feder.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     6568 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/header_processing/fitskeyword.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    30937 2022-06-01 17:57:03.000000 msumastro-1.2.4/msumastro/header_processing/patchers.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.567532 msumastro-1.2.4/msumastro/header_processing/tests/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/header_processing/tests/__init__.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1209 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/header_processing/tests/test_feder.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5359 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/header_processing/tests/test_fitskeyword.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    25392 2022-06-01 17:57:03.000000 msumastro-1.2.4/msumastro/header_processing/tests/test_patchers.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.574177 msumastro-1.2.4/msumastro/scripts/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/scripts/__init__.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4570 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/scripts/quick_add_keys_to_file.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    11249 2023-05-25 21:23:47.000000 msumastro-1.2.4/msumastro/scripts/run_astrometry.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7815 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/scripts/run_patch.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     9260 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/scripts/run_standard_header_process.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    13461 2023-05-25 21:23:47.000000 msumastro-1.2.4/msumastro/scripts/run_triage.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4983 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/scripts/script_helpers.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7342 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/scripts/sort_files.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.575309 msumastro-1.2.4/msumastro/scripts/tests/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/scripts/tests/__init__.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    25943 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/scripts/tests/test_scripts.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     6344 2022-04-01 21:53:04.000000 msumastro-1.2.4/msumastro/table_tree.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.577580 msumastro-1.2.4/msumastro/tests/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/__init__.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.598636 msumastro-1.2.4/msumastro/tests/data/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    25920 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/aspen_trimmed.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/biastest1.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/biastest2.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/biastest3.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/biastest4.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/biastest5.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5760 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/celestron_nightscape_10100_astro_fx_v106.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/darktest1.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/darktest2.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/darktest3.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/darktest4.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/darktest5.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    83520 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/flattest.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     8640 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/maximdl_5_21_header.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    46080 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/maximdl_5_23_header.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    46080 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/maximdl_6_16_header.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    31680 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/maximdl_6_18_header.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)   786240 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/neon-on-dome-10-sec-high-res-though-scope.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5760 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/uint16.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5760 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/uint16_missing_filter.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5760 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/uint16_no_pointing.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5760 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/uint16_not_m101.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      537 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7168 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/test_image_grouper.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.560437 msumastro-1.2.4/msumastro.egg-info/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      612 2023-05-25 21:36:41.000000 msumastro-1.2.4/msumastro.egg-info/PKG-INFO
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2570 2023-05-25 21:36:41.000000 msumastro-1.2.4/msumastro.egg-info/SOURCES.txt
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        1 2023-05-25 21:36:41.000000 msumastro-1.2.4/msumastro.egg-info/dependency_links.txt
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      416 2023-05-25 21:36:41.000000 msumastro-1.2.4/msumastro.egg-info/entry_points.txt
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        1 2023-05-25 21:36:41.000000 msumastro-1.2.4/msumastro.egg-info/not-zip-safe
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      111 2023-05-25 21:36:41.000000 msumastro-1.2.4/msumastro.egg-info/requires.txt
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       10 2023-05-25 21:36:41.000000 msumastro-1.2.4/msumastro.egg-info/top_level.txt
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      132 2023-05-25 21:23:47.000000 msumastro-1.2.4/pyproject.toml
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1529 2023-05-25 21:36:41.600008 msumastro-1.2.4/setup.cfg
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1039 2023-05-25 21:23:47.000000 msumastro-1.2.4/setup.py
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-07-29 17:32:49.615693 msumastro-1.2.5/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       35 2022-04-01 18:50:53.000000 msumastro-1.2.5/.gitattributes
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      187 2023-05-25 21:23:47.000000 msumastro-1.2.5/.gitignore
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      143 2022-04-01 18:50:53.000000 msumastro-1.2.5/.readthedocs.yml
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1254 2022-04-01 18:50:53.000000 msumastro-1.2.5/.travis.yml
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1573 2022-04-01 18:50:53.000000 msumastro-1.2.5/LICENSE.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      125 2022-04-01 18:50:53.000000 msumastro-1.2.5/MANIFEST.in
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      612 2023-07-29 17:32:49.615877 msumastro-1.2.5/PKG-INFO
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      976 2022-04-01 18:50:53.000000 msumastro-1.2.5/README.rst
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-07-29 17:32:49.545897 msumastro-1.2.5/docs/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4658 2022-04-01 18:50:53.000000 msumastro-1.2.5/docs/Makefile
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-07-29 17:32:49.532554 msumastro-1.2.5/docs/_templates/
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-07-29 17:32:49.547680 msumastro-1.2.5/docs/_templates/autosummary/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       42 2022-04-01 18:50:53.000000 msumastro-1.2.5/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       43 2022-04-01 18:50:53.000000 msumastro-1.2.5/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       44 2022-04-01 18:50:53.000000 msumastro-1.2.5/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7761 2022-04-01 18:50:53.000000 msumastro-1.2.5/docs/conf.py
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-07-29 17:32:49.548297 msumastro-1.2.5/docs/header_processing/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      772 2022-04-01 18:50:53.000000 msumastro-1.2.5/docs/header_processing/index.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      478 2022-04-01 18:50:53.000000 msumastro-1.2.5/docs/index.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4186 2022-04-01 18:50:53.000000 msumastro-1.2.5/docs/installation.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2099 2022-04-01 18:50:53.000000 msumastro-1.2.5/docs/overview.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       53 2022-04-01 18:50:53.000000 msumastro-1.2.5/docs/rtd-pip-requirements
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-07-29 17:32:49.550039 msumastro-1.2.5/docs/scripts/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    10924 2022-04-01 18:50:53.000000 msumastro-1.2.5/docs/scripts/automated_scripts.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2665 2022-04-01 18:50:53.000000 msumastro-1.2.5/docs/scripts/manual_processing.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     3825 2022-04-01 18:50:53.000000 msumastro-1.2.5/docs/scripts/scripts.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       55 2022-04-01 18:50:53.000000 msumastro-1.2.5/docs/xref.rst
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-07-29 17:32:49.552553 msumastro-1.2.5/msumastro/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       34 2023-05-25 21:23:47.000000 msumastro-1.2.5/msumastro/__init__.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5135 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/conftest.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2814 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/customlogger.py
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-07-29 17:32:49.560153 msumastro-1.2.5/msumastro/header_processing/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      150 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/header_processing/__init__.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    15954 2023-05-25 21:23:47.000000 msumastro-1.2.5/msumastro/header_processing/astrometry.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    18764 2023-07-29 17:30:18.000000 msumastro-1.2.5/msumastro/header_processing/feder.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     6568 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/header_processing/fitskeyword.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    30937 2022-06-01 17:57:03.000000 msumastro-1.2.5/msumastro/header_processing/patchers.py
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-07-29 17:32:49.564945 msumastro-1.2.5/msumastro/header_processing/tests/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/header_processing/tests/__init__.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1209 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/header_processing/tests/test_feder.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5359 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/header_processing/tests/test_fitskeyword.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    25392 2022-06-01 17:57:03.000000 msumastro-1.2.5/msumastro/header_processing/tests/test_patchers.py
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-07-29 17:32:49.571985 msumastro-1.2.5/msumastro/scripts/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/scripts/__init__.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4570 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/scripts/quick_add_keys_to_file.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    11249 2023-05-25 21:23:47.000000 msumastro-1.2.5/msumastro/scripts/run_astrometry.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7815 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/scripts/run_patch.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     9260 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/scripts/run_standard_header_process.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    13461 2023-05-25 21:23:47.000000 msumastro-1.2.5/msumastro/scripts/run_triage.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4983 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/scripts/script_helpers.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7342 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/scripts/sort_files.py
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-07-29 17:32:49.573092 msumastro-1.2.5/msumastro/scripts/tests/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/scripts/tests/__init__.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    25943 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/scripts/tests/test_scripts.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     6344 2022-04-01 21:53:04.000000 msumastro-1.2.5/msumastro/table_tree.py
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-07-29 17:32:49.575022 msumastro-1.2.5/msumastro/tests/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/__init__.py
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-07-29 17:32:49.615023 msumastro-1.2.5/msumastro/tests/data/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    25920 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/aspen_trimmed.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/biastest1.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/biastest2.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/biastest3.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/biastest4.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/biastest5.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5760 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/celestron_nightscape_10100_astro_fx_v106.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/darktest1.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/darktest2.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/darktest3.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/darktest4.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/darktest5.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    83520 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/flattest.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     8640 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/maximdl_5_21_header.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    46080 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/maximdl_5_23_header.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    46080 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/maximdl_6_16_header.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    31680 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/maximdl_6_18_header.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)   786240 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/neon-on-dome-10-sec-high-res-though-scope.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5760 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/uint16.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5760 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/uint16_missing_filter.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5760 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/uint16_no_pointing.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5760 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data/uint16_not_m101.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      537 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/data.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7168 2022-04-01 18:50:53.000000 msumastro-1.2.5/msumastro/tests/test_image_grouper.py
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-07-29 17:32:49.556522 msumastro-1.2.5/msumastro.egg-info/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      612 2023-07-29 17:32:49.000000 msumastro-1.2.5/msumastro.egg-info/PKG-INFO
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2570 2023-07-29 17:32:49.000000 msumastro-1.2.5/msumastro.egg-info/SOURCES.txt
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        1 2023-07-29 17:32:49.000000 msumastro-1.2.5/msumastro.egg-info/dependency_links.txt
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      416 2023-07-29 17:32:49.000000 msumastro-1.2.5/msumastro.egg-info/entry_points.txt
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        1 2023-07-29 17:32:49.000000 msumastro-1.2.5/msumastro.egg-info/not-zip-safe
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      111 2023-07-29 17:32:49.000000 msumastro-1.2.5/msumastro.egg-info/requires.txt
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       10 2023-07-29 17:32:49.000000 msumastro-1.2.5/msumastro.egg-info/top_level.txt
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      132 2023-05-25 21:23:47.000000 msumastro-1.2.5/pyproject.toml
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1529 2023-07-29 17:32:49.616614 msumastro-1.2.5/setup.cfg
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1039 2023-05-25 21:23:47.000000 msumastro-1.2.5/setup.py
```

### Comparing `msumastro-1.2.4/.travis.yml` & `msumastro-1.2.5/.travis.yml`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/LICENSE.rst` & `msumastro-1.2.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/PKG-INFO` & `msumastro-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msumastro
-Version: 1.2.4
+Version: 1.2.5
 Summary: Process FITS files
 Home-page: http://github.com/mwcraig/msumastro
 Author: Matt Craig
 Author-email: mattwcraig@gmail.com
 License: BSD 3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `msumastro-1.2.4/README.rst` & `msumastro-1.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/docs/Makefile` & `msumastro-1.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/docs/conf.py` & `msumastro-1.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/docs/header_processing/index.rst` & `msumastro-1.2.5/docs/header_processing/index.rst`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/docs/installation.rst` & `msumastro-1.2.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/docs/overview.rst` & `msumastro-1.2.5/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/docs/scripts/automated_scripts.rst` & `msumastro-1.2.5/docs/scripts/automated_scripts.rst`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/docs/scripts/manual_processing.rst` & `msumastro-1.2.5/docs/scripts/manual_processing.rst`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/docs/scripts/scripts.rst` & `msumastro-1.2.5/docs/scripts/scripts.rst`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/conftest.py` & `msumastro-1.2.5/msumastro/conftest.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/customlogger.py` & `msumastro-1.2.5/msumastro/customlogger.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/header_processing/astrometry.py` & `msumastro-1.2.5/msumastro/header_processing/astrometry.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/header_processing/feder.py` & `msumastro-1.2.5/msumastro/header_processing/feder.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,16 @@
         bad_keys = ['OBJECT', 'JD', 'JD-HELIO', 'OBJCTALT', 'OBJCTAZ',
                     'OBJCTHA', 'AIRMASS', 'OBSERVER']
         fits_name = ['MaxIm DL Version 6.16 190601 00KPP',
                      'MaxIm DL Version 6.17 190601 00KPP',
                      'MaxIm DL Version 6.18 190601 00KPP',
                      'MaxIm DL Version 6.27 220525 26KU2',
                      'MaxIm DL Version 6.29 220525 26KU2',
-                     'MaxIm DL Version 6.30 220525 26KU2'
+                     'MaxIm DL Version 6.30 220525 26KU2',
+                     'MaxIm DL Version 6.30 240628 2HVXS',
                      ]
         super(MaximDL6, self).__init__("MaxImDL",
                                        fits_name=fits_name,
                                        major_version=6,
                                        minor_version=30,
                                        bad_keywords=bad_keys,
                                        fits_keyword='SWCREATE'
```

### Comparing `msumastro-1.2.4/msumastro/header_processing/fitskeyword.py` & `msumastro-1.2.5/msumastro/header_processing/fitskeyword.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/header_processing/patchers.py` & `msumastro-1.2.5/msumastro/header_processing/patchers.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/header_processing/tests/test_feder.py` & `msumastro-1.2.5/msumastro/header_processing/tests/test_feder.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/header_processing/tests/test_fitskeyword.py` & `msumastro-1.2.5/msumastro/header_processing/tests/test_fitskeyword.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/header_processing/tests/test_patchers.py` & `msumastro-1.2.5/msumastro/header_processing/tests/test_patchers.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/scripts/quick_add_keys_to_file.py` & `msumastro-1.2.5/msumastro/scripts/quick_add_keys_to_file.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/scripts/run_astrometry.py` & `msumastro-1.2.5/msumastro/scripts/run_astrometry.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/scripts/run_patch.py` & `msumastro-1.2.5/msumastro/scripts/run_patch.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/scripts/run_standard_header_process.py` & `msumastro-1.2.5/msumastro/scripts/run_standard_header_process.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/scripts/run_triage.py` & `msumastro-1.2.5/msumastro/scripts/run_triage.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/scripts/script_helpers.py` & `msumastro-1.2.5/msumastro/scripts/script_helpers.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/scripts/sort_files.py` & `msumastro-1.2.5/msumastro/scripts/sort_files.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/scripts/tests/test_scripts.py` & `msumastro-1.2.5/msumastro/scripts/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/table_tree.py` & `msumastro-1.2.5/msumastro/table_tree.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/aspen_trimmed.fit` & `msumastro-1.2.5/msumastro/tests/data/aspen_trimmed.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/biastest1.fit` & `msumastro-1.2.5/msumastro/tests/data/biastest1.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/biastest2.fit` & `msumastro-1.2.5/msumastro/tests/data/biastest2.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/biastest3.fit` & `msumastro-1.2.5/msumastro/tests/data/biastest3.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/biastest4.fit` & `msumastro-1.2.5/msumastro/tests/data/biastest4.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/biastest5.fit` & `msumastro-1.2.5/msumastro/tests/data/biastest5.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/celestron_nightscape_10100_astro_fx_v106.fit` & `msumastro-1.2.5/msumastro/tests/data/celestron_nightscape_10100_astro_fx_v106.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/darktest1.fit` & `msumastro-1.2.5/msumastro/tests/data/darktest1.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/darktest2.fit` & `msumastro-1.2.5/msumastro/tests/data/darktest2.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/darktest3.fit` & `msumastro-1.2.5/msumastro/tests/data/darktest3.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/darktest4.fit` & `msumastro-1.2.5/msumastro/tests/data/darktest4.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/darktest5.fit` & `msumastro-1.2.5/msumastro/tests/data/darktest5.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/flattest.fit` & `msumastro-1.2.5/msumastro/tests/data/flattest.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/maximdl_5_21_header.fit` & `msumastro-1.2.5/msumastro/tests/data/maximdl_5_21_header.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/maximdl_5_23_header.fit` & `msumastro-1.2.5/msumastro/tests/data/maximdl_5_23_header.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/maximdl_6_16_header.fit` & `msumastro-1.2.5/msumastro/tests/data/maximdl_6_16_header.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/maximdl_6_18_header.fit` & `msumastro-1.2.5/msumastro/tests/data/maximdl_6_18_header.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/neon-on-dome-10-sec-high-res-though-scope.fit` & `msumastro-1.2.5/msumastro/tests/data/neon-on-dome-10-sec-high-res-though-scope.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/uint16.fit` & `msumastro-1.2.5/msumastro/tests/data/uint16.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/uint16_missing_filter.fit` & `msumastro-1.2.5/msumastro/tests/data/uint16_missing_filter.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/uint16_no_pointing.fit` & `msumastro-1.2.5/msumastro/tests/data/uint16_no_pointing.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data/uint16_not_m101.fit` & `msumastro-1.2.5/msumastro/tests/data/uint16_not_m101.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/data.py` & `msumastro-1.2.5/msumastro/tests/data.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro/tests/test_image_grouper.py` & `msumastro-1.2.5/msumastro/tests/test_image_grouper.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/msumastro.egg-info/PKG-INFO` & `msumastro-1.2.5/msumastro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msumastro
-Version: 1.2.4
+Version: 1.2.5
 Summary: Process FITS files
 Home-page: http://github.com/mwcraig/msumastro
 Author: Matt Craig
 Author-email: mattwcraig@gmail.com
 License: BSD 3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `msumastro-1.2.4/msumastro.egg-info/SOURCES.txt` & `msumastro-1.2.5/msumastro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/setup.cfg` & `msumastro-1.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.4/setup.py` & `msumastro-1.2.5/setup.py`

 * *Files identical despite different names*

