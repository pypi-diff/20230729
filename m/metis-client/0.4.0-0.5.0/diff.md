# Comparing `tmp/metis_client-0.4.0.tar.gz` & `tmp/metis_client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metis_client-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "metis_client-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `metis_client-0.4.0.tar` & `metis_client-0.5.0.tar`

### file list

```diff
@@ -1,73 +1,74 @@
--rw-r--r--   0        0        0      372 2023-07-20 13:46:16.071964 metis_client-0.4.0/.flake8
--rw-r--r--   0        0        0      212 2023-07-20 13:46:16.071964 metis_client-0.4.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1396 2023-07-20 13:46:16.071964 metis_client-0.4.0/.github/workflows/linter.yml
--rw-r--r--   0        0        0      792 2023-07-20 13:46:16.071964 metis_client-0.4.0/.github/workflows/pr.yml
--rw-r--r--   0        0        0     1968 2023-07-20 13:46:16.071964 metis_client-0.4.0/.github/workflows/push.yml
--rw-r--r--   0        0        0      867 2023-07-20 13:46:16.071964 metis_client-0.4.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1338 2023-07-20 13:46:16.071964 metis_client-0.4.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1869 2023-07-20 13:46:16.071964 metis_client-0.4.0/.gitignore
--rw-r--r--   0        0        0      275 2023-07-20 13:46:16.071964 metis_client-0.4.0/.whitesource
--rw-r--r--   0        0        0     1019 2023-07-20 13:46:16.071964 metis_client-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0      492 2023-07-20 13:46:16.071964 metis_client-0.4.0/CITATION.cff
--rw-r--r--   0        0        0     2819 2023-07-20 13:46:16.071964 metis_client-0.4.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1452 2023-07-20 13:46:16.071964 metis_client-0.4.0/LICENSE
--rw-r--r--   0        0        0     1764 2023-07-20 13:46:16.071964 metis_client-0.4.0/README.md
--rw-r--r--   0        0        0      156 2023-07-20 13:46:16.071964 metis_client-0.4.0/examples/data/user_object_one.dat
--rw-r--r--   0        0        0     3517 2023-07-20 13:46:16.071964 metis_client-0.4.0/examples/example_async.py
--rw-r--r--   0        0        0     3240 2023-07-20 13:46:16.071964 metis_client-0.4.0/examples/example_sync.py
--rw-r--r--   0        0        0      241 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/__init__.py
--rw-r--r--   0        0        0    10738 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/client.py
--rw-r--r--   0        0        0      625 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/const.py
--rw-r--r--   0        0        0      691 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/__init__.py
--rw-r--r--   0        0        0      314 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/auth.py
--rw-r--r--   0        0        0      386 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/base.py
--rw-r--r--   0        0        0      625 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/calculation.py
--rw-r--r--   0        0        0     1355 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/collection.py
--rw-r--r--   0        0        0     1002 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/datasource.py
--rw-r--r--   0        0        0      405 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/error.py
--rw-r--r--   0        0        0     2214 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/event.py
--rw-r--r--   0        0        0      282 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/resp.py
--rw-r--r--   0        0        0      683 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/user.py
--rw-r--r--   0        0        0     1474 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/exc.py
--rw-r--r--   0        0        0     4342 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/helpers.py
--rw-r--r--   0        0        0    11184 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/metis.py
--rw-r--r--   0        0        0     4105 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/metis_async.py
--rw-r--r--   0        0        0      266 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/models/__init__.py
--rw-r--r--   0        0        0     2915 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/models/auth.py
--rw-r--r--   0        0        0      230 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/models/base.py
--rw-r--r--   0        0        0     2410 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/models/event.py
--rw-r--r--   0        0        0     1751 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/models/hub.py
--rw-r--r--   0        0        0     2770 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/models/subscription.py
--rw-r--r--   0        0        0        0 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/namespaces/__init__.py
--rw-r--r--   0        0        0      934 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/namespaces/base.py
--rw-r--r--   0        0        0      697 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/namespaces/calculations.py
--rw-r--r--   0        0        0     1439 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/namespaces/root.py
--rw-r--r--   0        0        0     2370 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/namespaces/stream.py
--rw-r--r--   0        0        0     1711 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/namespaces/v0.py
--rw-r--r--   0        0        0      942 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/namespaces/v0_auth.py
--rw-r--r--   0        0        0     7540 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/namespaces/v0_calculations.py
--rw-r--r--   0        0        0     3558 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/namespaces/v0_collections.py
--rw-r--r--   0        0        0     3849 2023-07-20 13:46:16.075964 metis_client-0.4.0/metis_client/namespaces/v0_datasources.py
--rw-r--r--   0        0        0     3447 2023-07-20 13:46:16.075964 metis_client-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      217 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/helpers.py
--rw-r--r--   0        0        0        0 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/models/__init__.py
--rw-r--r--   0        0        0      824 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/models/test_auth_no_auth.py
--rw-r--r--   0        0        0     3139 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/models/test_auth_password.py
--rw-r--r--   0        0        0     1175 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/models/test_auth_token.py
--rw-r--r--   0        0        0      484 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/models/test_event.py
--rw-r--r--   0        0        0      211 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/models/test_hub.py
--rw-r--r--   0        0        0      821 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/models/test_subscription.py
--rw-r--r--   0        0        0        0 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/namespaces/__init__.py
--rw-r--r--   0        0        0     1813 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/namespaces/test_calculations.py
--rw-r--r--   0        0        0     3763 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/namespaces/test_v0_auth.py
--rw-r--r--   0        0        0    12310 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/namespaces/test_v0_calculations.py
--rw-r--r--   0        0        0     7954 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/namespaces/test_v0_collections.py
--rw-r--r--   0        0        0    11277 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/namespaces/test_v0_datasources.py
--rw-r--r--   0        0        0    11235 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/test_client.py
--rw-r--r--   0        0        0      332 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/test_exc.py
--rw-r--r--   0        0        0     1023 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/test_helpers_convert_dict_items_to_datetime.py
--rw-r--r--   0        0        0      976 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/test_helpers_rfc3339.py
--rw-r--r--   0        0        0      655 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/test_metis.py
--rw-r--r--   0        0        0      236 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/test_metis_async.py
--rw-r--r--   0        0        0     3917 1970-01-01 00:00:00.000000 metis_client-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      415 2023-07-29 13:21:31.928786 metis_client-0.5.0/.flake8
+-rw-r--r--   0        0        0      212 2023-07-29 13:21:31.928786 metis_client-0.5.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1406 2023-07-29 13:21:31.928786 metis_client-0.5.0/.github/workflows/linter.yml
+-rw-r--r--   0        0        0      792 2023-07-29 13:21:31.928786 metis_client-0.5.0/.github/workflows/pr.yml
+-rw-r--r--   0        0        0     2014 2023-07-29 13:21:31.928786 metis_client-0.5.0/.github/workflows/push.yml
+-rw-r--r--   0        0        0      905 2023-07-29 13:21:31.928786 metis_client-0.5.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1338 2023-07-29 13:21:31.928786 metis_client-0.5.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1869 2023-07-29 13:21:31.928786 metis_client-0.5.0/.gitignore
+-rw-r--r--   0        0        0      275 2023-07-29 13:21:31.928786 metis_client-0.5.0/.whitesource
+-rw-r--r--   0        0        0     1103 2023-07-29 13:21:31.928786 metis_client-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0      492 2023-07-29 13:21:31.928786 metis_client-0.5.0/CITATION.cff
+-rw-r--r--   0        0        0     2819 2023-07-29 13:21:31.928786 metis_client-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1452 2023-07-29 13:21:31.928786 metis_client-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1764 2023-07-29 13:21:31.928786 metis_client-0.5.0/README.md
+-rw-r--r--   0        0        0      156 2023-07-29 13:21:31.928786 metis_client-0.5.0/examples/data/user_object_one.dat
+-rw-r--r--   0        0        0     3517 2023-07-29 13:21:31.928786 metis_client-0.5.0/examples/example_async.py
+-rw-r--r--   0        0        0     3240 2023-07-29 13:21:31.928786 metis_client-0.5.0/examples/example_sync.py
+-rw-r--r--   0        0        0      241 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/__init__.py
+-rw-r--r--   0        0        0    10776 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/client.py
+-rw-r--r--   0        0        0      625 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/const.py
+-rw-r--r--   0        0        0      691 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/dtos/__init__.py
+-rw-r--r--   0        0        0      314 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/dtos/auth.py
+-rw-r--r--   0        0        0      386 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/dtos/base.py
+-rw-r--r--   0        0        0      625 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/dtos/calculation.py
+-rw-r--r--   0        0        0     1355 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/dtos/collection.py
+-rw-r--r--   0        0        0     1002 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/dtos/datasource.py
+-rw-r--r--   0        0        0      405 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/dtos/error.py
+-rw-r--r--   0        0        0     2214 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/dtos/event.py
+-rw-r--r--   0        0        0      282 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/dtos/resp.py
+-rw-r--r--   0        0        0      683 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/dtos/user.py
+-rw-r--r--   0        0        0     1474 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/exc.py
+-rw-r--r--   0        0        0     4342 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/helpers.py
+-rw-r--r--   0        0        0    11184 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/metis.py
+-rw-r--r--   0        0        0     4105 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/metis_async.py
+-rw-r--r--   0        0        0      266 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/models/__init__.py
+-rw-r--r--   0        0        0     2915 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/models/auth.py
+-rw-r--r--   0        0        0      230 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/models/base.py
+-rw-r--r--   0        0        0     2410 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/models/event.py
+-rw-r--r--   0        0        0     1751 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/models/hub.py
+-rw-r--r--   0        0        0     2770 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/models/subscription.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/namespaces/__init__.py
+-rw-r--r--   0        0        0      934 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/namespaces/base.py
+-rw-r--r--   0        0        0      697 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/namespaces/calculations.py
+-rw-r--r--   0        0        0     1439 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/namespaces/root.py
+-rw-r--r--   0        0        0     2370 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/namespaces/stream.py
+-rw-r--r--   0        0        0     1711 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/namespaces/v0.py
+-rw-r--r--   0        0        0      942 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/namespaces/v0_auth.py
+-rw-r--r--   0        0        0     7540 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/namespaces/v0_calculations.py
+-rw-r--r--   0        0        0     3558 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/namespaces/v0_collections.py
+-rw-r--r--   0        0        0     3849 2023-07-29 13:21:31.928786 metis_client-0.5.0/metis_client/namespaces/v0_datasources.py
+-rw-r--r--   0        0        0     3158 2023-07-29 13:21:31.928786 metis_client-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-07-29 13:21:31.928786 metis_client-0.5.0/renovate.json
+-rw-r--r--   0        0        0        0 2023-07-29 13:21:31.928786 metis_client-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      217 2023-07-29 13:21:31.928786 metis_client-0.5.0/tests/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:21:31.928786 metis_client-0.5.0/tests/models/__init__.py
+-rw-r--r--   0        0        0      824 2023-07-29 13:21:31.928786 metis_client-0.5.0/tests/models/test_auth_no_auth.py
+-rw-r--r--   0        0        0     3139 2023-07-29 13:21:31.928786 metis_client-0.5.0/tests/models/test_auth_password.py
+-rw-r--r--   0        0        0     1175 2023-07-29 13:21:31.928786 metis_client-0.5.0/tests/models/test_auth_token.py
+-rw-r--r--   0        0        0      484 2023-07-29 13:21:31.928786 metis_client-0.5.0/tests/models/test_event.py
+-rw-r--r--   0        0        0      211 2023-07-29 13:21:31.932786 metis_client-0.5.0/tests/models/test_hub.py
+-rw-r--r--   0        0        0      821 2023-07-29 13:21:31.932786 metis_client-0.5.0/tests/models/test_subscription.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:21:31.932786 metis_client-0.5.0/tests/namespaces/__init__.py
+-rw-r--r--   0        0        0     1813 2023-07-29 13:21:31.932786 metis_client-0.5.0/tests/namespaces/test_calculations.py
+-rw-r--r--   0        0        0     3763 2023-07-29 13:21:31.932786 metis_client-0.5.0/tests/namespaces/test_v0_auth.py
+-rw-r--r--   0        0        0    12310 2023-07-29 13:21:31.932786 metis_client-0.5.0/tests/namespaces/test_v0_calculations.py
+-rw-r--r--   0        0        0     7954 2023-07-29 13:21:31.932786 metis_client-0.5.0/tests/namespaces/test_v0_collections.py
+-rw-r--r--   0        0        0    11277 2023-07-29 13:21:31.932786 metis_client-0.5.0/tests/namespaces/test_v0_datasources.py
+-rw-r--r--   0        0        0    11235 2023-07-29 13:21:31.932786 metis_client-0.5.0/tests/test_client.py
+-rw-r--r--   0        0        0      332 2023-07-29 13:21:31.932786 metis_client-0.5.0/tests/test_exc.py
+-rw-r--r--   0        0        0     1023 2023-07-29 13:21:31.932786 metis_client-0.5.0/tests/test_helpers_convert_dict_items_to_datetime.py
+-rw-r--r--   0        0        0      976 2023-07-29 13:21:31.932786 metis_client-0.5.0/tests/test_helpers_rfc3339.py
+-rw-r--r--   0        0        0      655 2023-07-29 13:21:31.932786 metis_client-0.5.0/tests/test_metis.py
+-rw-r--r--   0        0        0      236 2023-07-29 13:21:31.932786 metis_client-0.5.0/tests/test_metis_async.py
+-rw-r--r--   0        0        0     3917 1970-01-01 00:00:00.000000 metis_client-0.5.0/PKG-INFO
```

### Comparing `metis_client-0.4.0/.github/workflows/linter.yml` & `metis_client-0.5.0/.github/workflows/linter.yml`

 * *Files 20% similar despite different names*

```diff
@@ -45,13 +45,14 @@
         run: |
           find -name "*.py" -print0 | xargs -0 -n1 pyupgrade --py38-plus
 
       - name: isort
         run: isort -c --diff **/*.py
 
       - name: flake8
-        run: |
-          flake8 --exclude __init__.py
-          flake8 --extend-ignore=F401
+        run: flake8
 
       - name: pylint
         run: pylint metis_client tests examples
+
+      - name: pyupgrade
+        run: pyupgrade --py38-plus --keep-percent-format
```

### Comparing `metis_client-0.4.0/.github/workflows/pr.yml` & `metis_client-0.5.0/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/.github/workflows/push.yml` & `metis_client-0.5.0/.github/workflows/push.yml`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
   release:
     name: Bump version and create draft release
     runs-on: ubuntu-latest
     needs: test
     permissions:
       contents: write
+    concurrency:
+      group: release
 
     steps:
       - name: Checkout repository
         uses: actions/checkout@v3
         if: ${{ !env.ACT }} # skip during local actions testing
         with:
           fetch-depth: 0
@@ -35,37 +37,37 @@
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install .[release]
 
       - name: Create bump and changelog
         id: cz
-        if: github.repository == 'tilde-lab/metis-client'
-        uses: commitizen-tools/commitizen-action@e41bf7f2029bc8175af362badd6fd0860a329b0f
+        if: github.repository == 'metis-science/metis-client'
+        uses: commitizen-tools/commitizen-action@4498afe6f2f1c5993fb29f22db7b597538c00aae
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           changelog_increment_filename: .CHANGELOG-CURRENT.md
           push: true
           commit: true
 
       - name: Print new version
-        if: github.repository == 'tilde-lab/metis-client'
+        if: github.repository == 'metis-science/metis-client'
         run: echo "Bumped to version ${{ steps.cz.outputs.version }}"
 
       - name: Build
         run: flit build
 
       - name: Stop if no bump
         id: no-bump
         continue-on-error: true
         # will fail if not on exact tag
         run: git describe --tags --exact-match
 
       - name: Create Release Draft
-        uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844
+        uses: softprops/action-gh-release@c9b46fe7aad9f02afd89b12450b780f52dacfb2d
         if: steps.no-bump.outcome == 'success'
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         with:
           draft: true
           tag_name: v${{ steps.cz.outputs.version }}
           body_path: .CHANGELOG-CURRENT.md
```

### Comparing `metis_client-0.4.0/.github/workflows/release.yml` & `metis_client-0.5.0/.github/workflows/release.yml`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     types: [published]
 
   workflow_dispatch:
 
 jobs:
   pypi:
     runs-on: ubuntu-latest
+    concurrency:
+      group: release
 
     steps:
       - name: Checkout repository
         uses: actions/checkout@v3
         if: ${{ !env.ACT }} # skip during local actions testing
         with:
           fetch-depth: 0
```

### Comparing `metis_client-0.4.0/.github/workflows/test.yml` & `metis_client-0.5.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/.gitignore` & `metis_client-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/CHANGELOG.md` & `metis_client-0.5.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v0.5.0 (2023-07-27)
+
+### Feat
+
+- **namespaces**: check that engine is supported
+
 ## v0.4.0 (2023-06-25)
 
 ### Feat
 
 - **namespaces**: implements /calculations namespace, deprecate get_engines()
 - **MetisAPI**: timeouts
```

### Comparing `metis_client-0.4.0/CONTRIBUTING.md` & `metis_client-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/LICENSE` & `metis_client-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/README.md` & `metis_client-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/examples/example_async.py` & `metis_client-0.5.0/examples/example_async.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/examples/example_sync.py` & `metis_client-0.5.0/examples/example_sync.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/client.py` & `metis_client-0.5.0/metis_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Low level http and SSE client"""
 
 import sys
-from asyncio import CancelledError, TimeoutError as AsyncioTimeoutError, sleep
+from asyncio import CancelledError
+from asyncio import TimeoutError as AsyncioTimeoutError
+from asyncio import sleep
 from concurrent.futures import TimeoutError as FuturesTimeoutError
 from datetime import timedelta
 from json import JSONDecodeError
 from typing import Any, Optional, Union
 
 import aiohttp
 from aiohttp import ClientResponse, ClientTimeout, RequestInfo
```

### Comparing `metis_client-0.4.0/metis_client/const.py` & `metis_client-0.5.0/metis_client/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Constants for metis_client."""
 
 from __future__ import annotations
 
 from logging import Logger, getLogger
 from typing import Literal, Union
 
-PROJECT_VERSION = "0.4.0"
+PROJECT_VERSION = "0.5.0"
 PROJECT_NAME = "metis_client"
 
 # This is the default user agent,
 # but it is adviced to use your own when building out your application
 DEFAULT_USER_AGENT = f"metis_client/{PROJECT_VERSION}"
```

### Comparing `metis_client-0.4.0/metis_client/dtos/__init__.py` & `metis_client-0.5.0/metis_client/dtos/__init__.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/dtos/calculation.py` & `metis_client-0.5.0/metis_client/dtos/calculation.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/dtos/collection.py` & `metis_client-0.5.0/metis_client/dtos/collection.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/dtos/datasource.py` & `metis_client-0.5.0/metis_client/dtos/datasource.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/dtos/event.py` & `metis_client-0.5.0/metis_client/dtos/event.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/dtos/user.py` & `metis_client-0.5.0/metis_client/dtos/user.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/exc.py` & `metis_client-0.5.0/metis_client/exc.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/helpers.py` & `metis_client-0.5.0/metis_client/helpers.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/metis.py` & `metis_client-0.5.0/metis_client/metis.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/metis_async.py` & `metis_client-0.5.0/metis_client/metis_async.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/models/auth.py` & `metis_client-0.5.0/metis_client/models/auth.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/models/event.py` & `metis_client-0.5.0/metis_client/models/event.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/models/hub.py` & `metis_client-0.5.0/metis_client/models/hub.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/models/subscription.py` & `metis_client-0.5.0/metis_client/models/subscription.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/namespaces/base.py` & `metis_client-0.5.0/metis_client/namespaces/base.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/namespaces/calculations.py` & `metis_client-0.5.0/metis_client/namespaces/calculations.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/namespaces/root.py` & `metis_client-0.5.0/metis_client/namespaces/root.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/namespaces/stream.py` & `metis_client-0.5.0/metis_client/namespaces/stream.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/namespaces/v0.py` & `metis_client-0.5.0/metis_client/namespaces/v0.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/namespaces/v0_auth.py` & `metis_client-0.5.0/metis_client/namespaces/v0_auth.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/namespaces/v0_calculations.py` & `metis_client-0.5.0/metis_client/namespaces/v0_calculations.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/namespaces/v0_collections.py` & `metis_client-0.5.0/metis_client/namespaces/v0_collections.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/metis_client/namespaces/v0_datasources.py` & `metis_client-0.5.0/metis_client/namespaces/v0_datasources.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/pyproject.toml` & `metis_client-0.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 # build the package with [flit](https://flit.readthedocs.io)
 requires = ["flit_core >=3.4,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "metis-client"
-version = "0.4.0"
+version = "0.5.0"
 description = """Metis infra API client in Python"""
 authors = [{name = "Sergei Korolev", email = "knopki@duck.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: BSD License",
@@ -76,24 +76,15 @@
 remove-duplicate-keys = true
 remove-unused-variables = true
 
 [tool.black]
 target-version = ['py38', 'py39', 'py310', 'py311']
 
 [tool.isort]
-# see https://github.com/psf/black
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-combine_as_imports = true
-use_parentheses = true
-line_length = 88
-sections = ["FUTURE", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
-default_section = "THIRDPARTY"
-ensure_newline_before_comments = true
+profile = "black"
 py_version = 38
 
 [tool.mypy]
 python_version = "3.8"
 warn_return_any = true
 warn_unused_configs = true
 
@@ -129,15 +120,15 @@
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 addopts = "--cov=metis_client --cov-report=term --no-cov-on-fail --cov-fail-under=99"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.4.0"
 tag_format = "v$version"
 major_version_zero = true
 version_files = [
     "pyproject.toml:^version",
     "metis_client/const.py:^PROJECT_VERSION",
 ]
+version_provider = "pep621"
 update_changelog_on_bump = true
```

### Comparing `metis_client-0.4.0/tests/models/test_auth_no_auth.py` & `metis_client-0.5.0/tests/models/test_auth_no_auth.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/tests/models/test_auth_password.py` & `metis_client-0.5.0/tests/models/test_auth_password.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/tests/models/test_auth_token.py` & `metis_client-0.5.0/tests/models/test_auth_token.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/tests/models/test_subscription.py` & `metis_client-0.5.0/tests/models/test_subscription.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/tests/namespaces/test_calculations.py` & `metis_client-0.5.0/tests/namespaces/test_calculations.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/tests/namespaces/test_v0_auth.py` & `metis_client-0.5.0/tests/namespaces/test_v0_auth.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/tests/namespaces/test_v0_calculations.py` & `metis_client-0.5.0/tests/namespaces/test_v0_calculations.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/tests/namespaces/test_v0_collections.py` & `metis_client-0.5.0/tests/namespaces/test_v0_collections.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/tests/namespaces/test_v0_datasources.py` & `metis_client-0.5.0/tests/namespaces/test_v0_datasources.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/tests/test_client.py` & `metis_client-0.5.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/tests/test_helpers_convert_dict_items_to_datetime.py` & `metis_client-0.5.0/tests/test_helpers_convert_dict_items_to_datetime.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/tests/test_helpers_rfc3339.py` & `metis_client-0.5.0/tests/test_helpers_rfc3339.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/tests/test_metis.py` & `metis_client-0.5.0/tests/test_metis.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.4.0/PKG-INFO` & `metis_client-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metis-client
-Version: 0.4.0
+Version: 0.5.0
 Summary: Metis infra API client in Python
 Keywords: metis,client
 Author-email: Sergei Korolev <knopki@duck.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

