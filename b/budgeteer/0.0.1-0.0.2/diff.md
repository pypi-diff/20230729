# Comparing `tmp/budgeteer-0.0.1.tar.gz` & `tmp/budgeteer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "budgeteer-0.0.1.tar", last modified: Sat Jul 29 12:17:37 2023, max compression
+gzip compressed data, was "budgeteer-0.0.2.tar", last modified: Sat Jul 29 12:59:18 2023, max compression
```

## Comparing `budgeteer-0.0.1.tar` & `budgeteer-0.0.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:17:37.749358 budgeteer-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-29 12:17:09.000000 budgeteer-0.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-29 12:17:09.000000 budgeteer-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-07-29 12:17:37.749358 budgeteer-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-29 12:17:09.000000 budgeteer-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:17:37.737357 budgeteer-0.0.1/budgeteer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:17:09.000000 budgeteer-0.0.1/budgeteer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-29 12:17:09.000000 budgeteer-0.0.1/budgeteer/budget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:17:37.741357 budgeteer-0.0.1/budgeteer/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:17:09.000000 budgeteer-0.0.1/budgeteer/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-29 12:17:09.000000 budgeteer-0.0.1/budgeteer/providers/common_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-07-29 12:17:09.000000 budgeteer-0.0.1/budgeteer/providers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:17:37.741357 budgeteer-0.0.1/budgeteer/providers/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:17:09.000000 budgeteer-0.0.1/budgeteer/providers/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-29 12:17:09.000000 budgeteer-0.0.1/budgeteer/providers/http_requests/cache_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-07-29 12:17:09.000000 budgeteer-0.0.1/budgeteer/providers/http_requests/cloudflare_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-07-29 12:17:09.000000 budgeteer-0.0.1/budgeteer/providers/http_requests/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-29 12:17:09.000000 budgeteer-0.0.1/budgeteer/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-29 12:17:09.000000 budgeteer-0.0.1/budgeteer/providers/sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-07-29 12:17:09.000000 budgeteer-0.0.1/budgeteer/providers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:17:37.741357 budgeteer-0.0.1/budgeteer/web_interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:17:09.000000 budgeteer-0.0.1/budgeteer/web_interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:17:37.737357 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:17:37.741357 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:17:37.745358 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    85787 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-f1fc251a.js
--rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js
--rw-r--r--   0 runner    (1001) docker     (123)    67407 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-4b662da7.js
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-80cecced.js
--rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js
--rw-r--r--   0 runner    (1001) docker     (123)   231964 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css
--rw-r--r--   0 runner    (1001) docker     (123)    60654 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js
--rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76081 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css
--rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/date-format-parse-388037e5.js
--rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css
--rw-r--r--   0 runner    (1001) docker     (123)    21588 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/index-f9a1f1e7.js
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-datepicker-next-3bf3781e.css
--rw-r--r--   0 runner    (1001) docker     (123)    31419 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-datepicker-next-98f94a3e.js
--rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-b19737a8.js
--rw-r--r--   0 runner    (1001) docker     (123)    51150 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-86ed02bf.js
--rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-22d603d9.js
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-39f44738.js
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-29 12:17:36.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-07-29 12:17:09.000000 budgeteer-0.0.1/budgeteer/web_interface/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:17:37.737357 budgeteer-0.0.1/budgeteer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-29 12:17:37.000000 budgeteer-0.0.1/budgeteer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 12:17:37.749358 budgeteer-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-29 12:17:09.000000 budgeteer-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:59:18.447676 budgeteer-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-29 12:58:50.000000 budgeteer-0.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-29 12:58:50.000000 budgeteer-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-29 12:59:18.447676 budgeteer-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-29 12:58:50.000000 budgeteer-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:59:18.439676 budgeteer-0.0.2/budgeteer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:58:50.000000 budgeteer-0.0.2/budgeteer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-29 12:58:50.000000 budgeteer-0.0.2/budgeteer/budget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:59:18.439676 budgeteer-0.0.2/budgeteer/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:58:50.000000 budgeteer-0.0.2/budgeteer/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-29 12:58:50.000000 budgeteer-0.0.2/budgeteer/providers/common_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-07-29 12:58:50.000000 budgeteer-0.0.2/budgeteer/providers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:59:18.439676 budgeteer-0.0.2/budgeteer/providers/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:58:50.000000 budgeteer-0.0.2/budgeteer/providers/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-29 12:58:50.000000 budgeteer-0.0.2/budgeteer/providers/http_requests/cache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-07-29 12:58:50.000000 budgeteer-0.0.2/budgeteer/providers/http_requests/cloudflare_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-07-29 12:58:50.000000 budgeteer-0.0.2/budgeteer/providers/http_requests/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-29 12:58:50.000000 budgeteer-0.0.2/budgeteer/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-29 12:58:50.000000 budgeteer-0.0.2/budgeteer/providers/sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-07-29 12:58:50.000000 budgeteer-0.0.2/budgeteer/providers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:59:18.439676 budgeteer-0.0.2/budgeteer/web_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:58:50.000000 budgeteer-0.0.2/budgeteer/web_interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:59:18.439676 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:59:18.443676 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:59:18.447676 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    85787 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-f1fc251a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    67407 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-4b662da7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-80cecced.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js
+-rw-r--r--   0 runner    (1001) docker     (123)   231964 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css
+-rw-r--r--   0 runner    (1001) docker     (123)    60654 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js
+-rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76081 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css
+-rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/date-format-parse-388037e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/index-93e69acd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-datepicker-next-3bf3781e.css
+-rw-r--r--   0 runner    (1001) docker     (123)    31419 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-datepicker-next-98f94a3e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-b19737a8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    51150 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-86ed02bf.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-22d603d9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-39f44738.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-29 12:59:17.000000 budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-07-29 12:58:50.000000 budgeteer-0.0.2/budgeteer/web_interface/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:59:18.439676 budgeteer-0.0.2/budgeteer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-29 12:59:18.000000 budgeteer-0.0.2/budgeteer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-07-29 12:59:18.000000 budgeteer-0.0.2/budgeteer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:59:18.000000 budgeteer-0.0.2/budgeteer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-29 12:59:18.000000 budgeteer-0.0.2/budgeteer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:59:18.000000 budgeteer-0.0.2/budgeteer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 12:59:18.000000 budgeteer-0.0.2/budgeteer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-29 12:59:18.000000 budgeteer-0.0.2/budgeteer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 12:59:18.447676 budgeteer-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-29 12:58:50.000000 budgeteer-0.0.2/setup.py
```

### Comparing `budgeteer-0.0.1/LICENSE.md` & `budgeteer-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/PKG-INFO` & `budgeteer-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: budgeteer
-Version: 0.0.1
-Summary: Automate downloads using predefined sites and the My JDownloader API
-Home-page: https://github.com/rix1337/BudgeTeer
-Author: rix1337
-Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # BudgeTeer
 
 <img src="https://raw.githubusercontent.com/rix1337/BudgeTeer/main/budgeteer/web_interface/vuejs_frontend/public/favicon.ico" data-canonical-src="https://raw.githubusercontent.com/rix1337/BudgeTeer/main/budgeteer/web_interface/vuejs_frontend/public/favicon.ico" width="64" height="64" />
 
 Einfacher Überblick über das eigene Budget 
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/rix1337/BudgeTeer/CreateRelease.yml?branch=main)](https://github.com/rix1337/BudgeTeer/actions/workflows/CreateRelease.yml)
@@ -79,9 +64,8 @@
   werden.
 
 ### Windows Build
 
 * Jedem [Release](https://github.com/rix1337/BudgeTeer/releases) wird eine selbstständig unter Windows lauffähige
   Version des BudgeTeers beigefügt.
 * Hierfür müssen weder Python, noch die Zusatzpakete installiert werden.
-* Einfach die jeweilige Exe herunterladen und ausführen bzw. bei Updates die Exe ersetzen.
-
+* Einfach die jeweilige Exe herunterladen und ausführen bzw. bei Updates die Exe ersetzen.
```

### Comparing `budgeteer-0.0.1/README.md` & `budgeteer-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: budgeteer
+Version: 0.0.2
+Summary: Einfacher Überblick über das eigene Budget
+Home-page: https://github.com/rix1337/BudgeTeer
+Author: rix1337
+Author-email: 
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # BudgeTeer
 
 <img src="https://raw.githubusercontent.com/rix1337/BudgeTeer/main/budgeteer/web_interface/vuejs_frontend/public/favicon.ico" data-canonical-src="https://raw.githubusercontent.com/rix1337/BudgeTeer/main/budgeteer/web_interface/vuejs_frontend/public/favicon.ico" width="64" height="64" />
 
 Einfacher Überblick über das eigene Budget 
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/rix1337/BudgeTeer/CreateRelease.yml?branch=main)](https://github.com/rix1337/BudgeTeer/actions/workflows/CreateRelease.yml)
@@ -64,8 +79,9 @@
   werden.
 
 ### Windows Build
 
 * Jedem [Release](https://github.com/rix1337/BudgeTeer/releases) wird eine selbstständig unter Windows lauffähige
   Version des BudgeTeers beigefügt.
 * Hierfür müssen weder Python, noch die Zusatzpakete installiert werden.
-* Einfach die jeweilige Exe herunterladen und ausführen bzw. bei Updates die Exe ersetzen.
+* Einfach die jeweilige Exe herunterladen und ausführen bzw. bei Updates die Exe ersetzen.
+
```

### Comparing `budgeteer-0.0.1/budgeteer/budget.py` & `budgeteer-0.0.2/budgeteer/budget.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         shared_state_lock = manager.Lock()
         shared_state.set_state(shared_state_dict, shared_state_lock)
 
         parser = argparse.ArgumentParser()
         parser.add_argument("--log-level", help="Legt fest, wie genau geloggt wird (INFO, DEBUG)")
         parser.add_argument("--config", help="Legt den Ablageort für Einstellungen und Logs fest")
         parser.add_argument("--port", help="Legt den Port des Webservers fest")
+        parser.add_argument("--test_run", action='store_true', help="Intern: Führt einen Testlauf durch")
         parser.add_argument("--docker", action='store_true',
                             help="Intern: Sperre Pfad und Port auf Docker-Standardwerte")
         arguments = parser.parse_args()
 
         shared_state.set_initial_values(arguments.docker)
 
         sys.stdout = Unbuffered(sys.stdout)
@@ -76,16 +77,21 @@
             print('Der Webserver ist erreichbar unter "' + local_address + '"')
 
         shared_state.set_connection_info(local_address, port, prefix, docker)
 
         BudgetConfig("BudgeTeer").remove_redundant_entries()
         remove_redundant_db_tables(shared_state.values["dbfile"])
 
-        process_web_server = multiprocessing.Process(target=web_server, args=(shared_state_dict, shared_state_lock,))
-        process_web_server.start()
+        if not arguments.test_run:
+            process_web_server = multiprocessing.Process(target=web_server,
+                                                         args=(shared_state_dict, shared_state_lock,))
+            process_web_server.start()
+        else:
+            print("Testlauf aktiviert, Webserver wird nicht gestartet")
+            sys.exit(0)
 
         def signal_handler(sig, frame):
             process_web_server.terminate()
             sys.exit(0)
 
         signal.signal(signal.SIGINT, signal_handler)
         print('Drücke [Strg] + [C] zum Beenden')
```

### Comparing `budgeteer-0.0.1/budgeteer/providers/common_functions.py` & `budgeteer-0.0.2/budgeteer/providers/common_functions.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/providers/config.py` & `budgeteer-0.0.2/budgeteer/providers/config.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/providers/http_requests/cache_handler.py` & `budgeteer-0.0.2/budgeteer/providers/http_requests/cache_handler.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/providers/http_requests/cloudflare_handlers.py` & `budgeteer-0.0.2/budgeteer/providers/http_requests/cloudflare_handlers.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/providers/http_requests/request_handler.py` & `budgeteer-0.0.2/budgeteer/providers/http_requests/request_handler.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/providers/shared_state.py` & `budgeteer-0.0.2/budgeteer/providers/shared_state.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/providers/sqlite_database.py` & `budgeteer-0.0.2/budgeteer/providers/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/providers/version.py` & `budgeteer-0.0.2/budgeteer/providers/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import re
 from distutils.version import StrictVersion
 from urllib.request import urlopen
 
 
 def get_version():
-    return "0.0.1"
+    return "0.0.2"
 
 
 def create_version_file():
     version = get_version()
     version_clean = re.sub('[^\d\.]', '', version)
     if "a" in version:
         suffix = version.split("a")[1]
```

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-f1fc251a.js` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-f1fc251a.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-4b662da7.js` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-4b662da7.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-80cecced.js` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-80cecced.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/date-format-parse-388037e5.js` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/date-format-parse-388037e5.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/index-f9a1f1e7.js` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/index-93e69acd.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,43 +1,43 @@
 import {
     c as R,
-    b as K,
-    e as L,
-    D as o,
-    E as a,
+    b as T,
+    e as P,
+    D as a,
+    E as i,
     G as e,
-    q as w,
-    S as B,
-    Q as f,
-    s as P,
+    q as $,
+    S,
+    Q as v,
+    s as L,
     u as s,
-    B as $,
-    N as G,
+    B as k,
+    N as z,
     R as E,
-    X as j,
+    X as O,
     a0 as V,
-    a1 as N,
-    a2 as z,
-    Z as A
+    a1 as K,
+    a2 as I,
+    Z as G
 } from "./@vue-4b662da7.js";
 import {
-    u as T,
-    c as I
+    u as N,
+    c as W
 } from "./vuex-39f44738.js";
 import {
-    a as S
+    a as C
 } from "./axios-4a70c6fc.js";
 import {
-    c as Y,
-    a as H
+    c as A,
+    a as Y
 } from "./vue-router-b19737a8.js";
 import "./bootstrap-85852bd1.js"; /* empty css                        */
 import {
-    u as D,
-    s as W,
+    u as U,
+    s as H,
     T as F
 } from "./vue-toastification-22d603d9.js";
 import {
     s as q,
     p as X,
     d as Q,
     a as Z
@@ -53,54 +53,54 @@
     a as et
 } from "./@vueuse-80cecced.js";
 import "./@popperjs-8746c87e.js";
 import "./date-format-parse-388037e5.js";
 (function() {
     const t = document.createElement("link").relList;
     if (t && t.supports && t.supports("modulepreload")) return;
-    for (const n of document.querySelectorAll('link[rel="modulepreload"]')) g(n);
+    for (const n of document.querySelectorAll('link[rel="modulepreload"]')) f(n);
     new MutationObserver(n => {
         for (const l of n)
             if (l.type === "childList")
-                for (const u of l.addedNodes) u.tagName === "LINK" && u.rel === "modulepreload" && g(u)
+                for (const p of l.addedNodes) p.tagName === "LINK" && p.rel === "modulepreload" && f(p)
     }).observe(document, {
         childList: !0,
         subtree: !0
     });
 
-    function v(n) {
+    function m(n) {
         const l = {};
         return n.integrity && (l.integrity = n.integrity), n.referrerPolicy && (l.referrerPolicy = n.referrerPolicy), n.crossOrigin === "use-credentials" ? l.credentials = "include" : n.crossOrigin === "anonymous" ? l.credentials = "omit" : l.credentials = "same-origin", l
     }
 
-    function g(n) {
+    function f(n) {
         if (n.ep) return;
         n.ep = !0;
-        const l = v(n);
+        const l = m(n);
         fetch(n.href, l)
     }
 })();
 const st = {
         class: "container"
     },
-    nt = {
+    ot = {
         class: "row my-3"
     },
-    ot = {
+    nt = {
         class: "col-md-10 offset-md-1"
     },
     at = {
         class: "card text-center shadow my-3"
     },
     it = {
         class: "card-header"
     },
     lt = e("h1", null, [e("i", {
         class: "bi bi-cash-coin"
-    }), w(" BudgeTeer ")], -1),
+    }), $(" BudgeTeer ")], -1),
     ct = e("a", {
         href: "https://github.com/rix1337/BudgeTeer/releases/latest",
         target: "_blank"
     }, "RiX", -1),
     rt = {
         key: 0
     },
@@ -111,82 +111,107 @@
         class: "row justify-content-center mt-2"
     },
     pt = e("i", {
         class: "bi bi-gear"
     }, null, -1),
     bt = {
         __name: "Head",
-        setup(p) {
-            const t = T();
-            D(), R(() => {});
-            const v = K(""),
-                g = K(!1);
+        setup(h) {
+            const t = N(),
+                m = U();
+            R(() => {
+                p(), setInterval(p, 300 * 1e3)
+            });
+
+            function f() {
+                window.open("https://github.com/rix1337/BudgeTeer/releases/latest", "_blank")
+            }
+            const n = T(""),
+                l = T(!1);
+
+            function p() {
+                C.get("api/version/").then(function(_) {
+                    n.value = _.data.version.ver, console.info("%c BudgeTeer %c ".concat(n.value, " "), "color: white; background: #303030; font-weight: 700; font-size: 24px; font-family: Monospace;", "color: #303030; background: white; font-weight: 700; font-size: 24px; font-family: Monospace;"), console.info("%c ❤ Projekt unterstützen %c ".concat("https://github.com/sponsors/rix1337 ❤", " "), "color: white; background: #dc3545; font-weight: 700;", "color: #dc3545; background: white; font-weight: 700;"), l.value = _.data.version.update_ready, t.commit("setDocker", _.data.version.docker), l.value && (c("BudgeTeer - Update verfügbar! - "), console.log("Update steht bereit! Weitere Informationen unter https://github.com/rix1337/BudgeTeer/releases/latest"), m.info(`Update steht bereit! Weitere Informationen unter:
+https://github.com/rix1337/BudgeTeer/releases/latest`, {
+                        timeout: 15e3,
+                        onClick: f
+                    }))
+                }, function() {
+                    console.log("Konnte Version nicht abrufen!"), m.error("Konnte Version nicht abrufen!")
+                })
+            }
+
+            function c(_) {
+                document.title = _, setTimeout(function() {
+                    c(_.substr(1) + _.substr(0, 1))
+                }, 200)
+            }
 
-            function n() {
+            function r() {
                 t.commit("getSettings")
             }
-            const l = L({
+            const y = P({
                     get() {
-                        let c = 0;
-                        for (let b = 0; b < t.state.data.open_transactions.length; b++) {
-                            let _ = parseFloat(t.state.data.open_transactions[b].amount);
-                            isNaN(_) || (c += _)
+                        let _ = 0;
+                        for (let u = 0; u < t.state.data.open_transactions.length; u++) {
+                            let o = parseFloat(t.state.data.open_transactions[u].amount);
+                            isNaN(o) || (_ += o)
                         }
-                        let i = 0;
-                        for (let b = 0; b < t.state.data.balances.length; b++) {
-                            let _ = parseFloat(t.state.data.balances[b].balance);
-                            !isNaN(_) && t.state.data.balances[b].type === "checking" && (i += _)
+                        let d = 0;
+                        for (let u = 0; u < t.state.data.balances.length; u++) {
+                            let o = parseFloat(t.state.data.balances[u].balance);
+                            !isNaN(o) && t.state.data.balances[u].type === "checking" && (d += o)
                         }
-                        let y = 0;
-                        for (let b = 0; b < t.state.data.budgets.length; b++)
-                            for (let _ = 0; _ < t.state.data.budgets[b].entries.length; _++) {
-                                let d = parseFloat(t.state.data.budgets[b].entries[_].amount);
-                                !isNaN(d) && !t.state.data.budgets[b].entries[_].booked && (y += d)
+                        let b = 0;
+                        for (let u = 0; u < t.state.data.budgets.length; u++)
+                            for (let o = 0; o < t.state.data.budgets[u].entries.length; o++) {
+                                let M = parseFloat(t.state.data.budgets[u].entries[o].amount);
+                                !isNaN(M) && !t.state.data.budgets[u].entries[o].booked && (b += M)
                             }
-                        return parseFloat(i + c + y).toFixed(2)
+                        return parseFloat(d + _ + b).toFixed(2)
                     }
                 }),
-                u = K(new Date().toLocaleString("default", {
+                B = T(new Date().toLocaleString("default", {
                     month: "long"
                 }));
-            return (c, i) => (o(), a("div", st, [e("div", nt, [e("div", ot, [e("div", at, [e("div", it, [lt, e("p", null, [w("Projekt von "), ct, w(" " + B(v.value) + " ", 1), g.value ? (o(), a("span", rt, " (Update verfügbar!)")) : f("", !0)])]), e("div", dt, [e("div", ut, [e("h2", null, "Restbudget " + B(u.value) + ": " + B(l.value) + " €", 1), e("div", {
+            return (_, d) => (a(), i("div", st, [e("div", ot, [e("div", nt, [e("div", at, [e("div", it, [lt, e("p", null, [$("Projekt von "), ct, $(" " + S(n.value) + " ", 1), l.value ? (a(), i("span", rt, " (Update verfügbar!)")) : v("", !0)])]), e("div", dt, [e("div", ut, [e("h2", null, "Restbudget " + S(B.value) + ": " + S(y.value) + " €", 1), e("div", {
                 class: "col-md-auto p-1"
             }, [e("button", {
                 "aria-controls": "offcanvasBottomSettings",
                 class: "btn btn-outline-primary",
                 "data-bs-target": "#offcanvasBottomSettings",
                 "data-bs-toggle": "offcanvas",
                 type: "button",
-                onClick: n
-            }, [pt, w(" Einstellungen ")])])])])])])])]))
+                onClick: r
+            }, [pt, $(" Einstellungen ")])])])])])])])]))
         }
     };
 const _t = {
         class: "text-center"
     },
     ht = {
         id: "offcanvasBottomSettings",
         "aria-labelledby": "offcanvasBottomSettingsLabel",
         class: "offcanvas offcanvas-bottom",
         tabindex: "-1"
     },
-    mt = e("div", {
+    gt = e("div", {
         class: "offcanvas-header"
     }, [e("h3", {
         id: "offcanvasBottomSettingsLabel",
         class: "offcanvas-title"
     }, [e("i", {
         class: "bi bi-gear"
-    }), w(" Einstellungen")]), e("button", {
+    }), $(" Einstellungen")]), e("button", {
         "aria-label": "Close",
         class: "btn-close text-reset",
         "data-bs-dismiss": "offcanvas",
         type: "button"
     })], -1),
-    gt = {
+    mt = {
         class: "offcanvas-body"
     },
     ft = {
         key: 0
     },
     vt = {
         key: 1,
@@ -215,255 +240,255 @@
     },
     wt = {
         class: "accordion-body"
     },
     Ct = {
         key: 0
     },
-    St = {
+    Bt = {
         key: 0,
         class: "spinner-border spinner-border-sm",
         role: "status"
     },
-    Bt = {
+    St = {
         key: 1,
         class: "bi bi-save"
     },
     Vt = {
         key: 1,
         class: "btn btn-dark disabled"
     },
-    Kt = e("span", {
+    Tt = e("span", {
         class: "spinner-border spinner-border-sm",
         role: "status"
     }, null, -1),
-    Nt = {
+    Kt = {
         __name: "Settings",
-        setup(p) {
-            const t = T(),
-                v = D();
-
-            function g() {
-                n.value = !0, S.post("api/settings/", t.state.settings).then(function() {
-                    console.log("Einstellungen gespeichert! Neustart des BudgeTeers wird dringend empfohlen!"), v.success("Einstellungen gespeichert! Neustart des BudgeTeers wird dringend empfohlen!"), t.commit("getSettings"), n.value = !1
+        setup(h) {
+            const t = N(),
+                m = U();
+
+            function f() {
+                n.value = !0, C.post("api/settings/", t.state.settings).then(function() {
+                    console.log("Einstellungen gespeichert! Neustart des BudgeTeers wird dringend empfohlen!"), m.success("Einstellungen gespeichert! Neustart des BudgeTeers wird dringend empfohlen!"), t.commit("getSettings"), n.value = !1
                 }, function() {
-                    t.commit("getSettings"), n.value = !1, console.log("Konnte Einstellungen nicht speichern! Bitte die angegebenen Werte auf Richtigkeit prüfen."), v.error("Konnte Einstellungen nicht speichern! Bitte die angegebenen Werte auf Richtigkeit prüfen.")
+                    t.commit("getSettings"), n.value = !1, console.log("Konnte Einstellungen nicht speichern! Bitte die angegebenen Werte auf Richtigkeit prüfen."), m.error("Konnte Einstellungen nicht speichern! Bitte die angegebenen Werte auf Richtigkeit prüfen.")
                 })
             }
-            const n = K(!1),
-                l = L(() => t.state.settings.general.auth_hash.length > 0);
+            const n = T(!1),
+                l = P(() => t.state.settings.general.auth_hash.length > 0);
 
-            function u() {
+            function p() {
                 q("settings")
             }
-            return (c, i) => {
-                const y = P("FormKit");
-                return o(), a("div", _t, [e("div", ht, [mt, e("div", gt, [s(t).state.misc.loaded_settings ? f("", !0) : (o(), a("h4", ft, "Einstellungen werden geladen...")), s(t).state.misc.loaded_settings ? (o(), a("div", vt, [$(y, {
+            return (c, r) => {
+                const y = L("FormKit");
+                return a(), i("div", _t, [e("div", ht, [gt, e("div", mt, [s(t).state.misc.loaded_settings ? v("", !0) : (a(), i("h4", ft, "Einstellungen werden geladen...")), s(t).state.misc.loaded_settings ? (a(), i("div", vt, [k(y, {
                     id: "settings",
                     actions: !1,
                     "incomplete-message": "Es müssen alle Felder korrekt ausgefüllt werden! Fehler sind rot markiert.",
                     "messages-class": "text-danger mt-4",
                     type: "form",
-                    onSubmit: i[4] || (i[4] = b => g())
+                    onSubmit: r[4] || (r[4] = B => f())
                 }, {
-                    default: G(({
-                        value: b
-                    }) => [e("div", kt, [$t, e("div", yt, [e("div", wt, [s(t).state.misc.docker ? f("", !0) : (o(), a("div", Ct, [$(y, {
+                    default: z(({
+                        value: B
+                    }) => [e("div", kt, [$t, e("div", yt, [e("div", wt, [s(t).state.misc.docker ? v("", !0) : (a(), i("div", Ct, [k(y, {
                         modelValue: s(t).state.settings.general.port,
-                        "onUpdate:modelValue": i[0] || (i[0] = _ => s(t).state.settings.general.port = _),
+                        "onUpdate:modelValue": r[0] || (r[0] = _ => s(t).state.settings.general.port = _),
                         help: "Hier den Port des Webservers wählen.",
                         "help-class": "text-muted",
                         "input-class": "form-control bg-light mb-2",
                         label: "Port",
                         "messages-class": "text-danger",
                         "outer-class": "mb-4",
                         placeholder: "Bspw. 9090",
                         type: "number",
                         validation: "required|between:1024,65535",
                         "validation-visibility": "live"
-                    }, null, 8, ["modelValue"])])), $(y, {
+                    }, null, 8, ["modelValue"])])), k(y, {
                         modelValue: s(t).state.settings.general.prefix,
-                        "onUpdate:modelValue": i[1] || (i[1] = _ => s(t).state.settings.general.prefix = _),
+                        "onUpdate:modelValue": r[1] || (r[1] = _ => s(t).state.settings.general.prefix = _),
                         help: "Hier den Prefix des Webservers wählen (nützlich für Reverse-Proxies).",
                         "help-class": "text-muted",
                         "input-class": "form-control bg-light mb-2",
                         label: "Prefix",
                         "messages-class": "text-danger",
                         "outer-class": "mb-4",
                         placeholder: "Bspw. feedcrawler",
                         type: "text",
                         validation: "alpha",
                         "validation-visibility": "live"
-                    }, null, 8, ["modelValue"]), $(y, {
+                    }, null, 8, ["modelValue"]), k(y, {
                         modelValue: s(t).state.settings.general.auth_user,
-                        "onUpdate:modelValue": i[2] || (i[2] = _ => s(t).state.settings.general.auth_user = _),
-                        validation: b.auth_hash ? "required" : "",
+                        "onUpdate:modelValue": r[2] || (r[2] = _ => s(t).state.settings.general.auth_user = _),
+                        validation: B.auth_hash ? "required" : "",
                         help: "Hier den Nutzernamen für BudgeTeer eingeben.",
                         "help-class": "text-muted",
                         "input-class": "form-control bg-light mb-2",
                         label: "Nutzername",
                         "messages-class": "text-danger",
                         name: "auth_user",
                         "outer-class": "mb-4",
                         placeholder: "Bspw. rix1337",
                         type: "text"
-                    }, null, 8, ["modelValue", "validation"]), $(y, {
+                    }, null, 8, ["modelValue", "validation"]), k(y, {
                         modelValue: s(t).state.settings.general.auth_hash,
-                        "onUpdate:modelValue": i[3] || (i[3] = _ => s(t).state.settings.general.auth_hash = _),
-                        validation: l.value && b.auth_user ? "required|length:6" : "",
+                        "onUpdate:modelValue": r[3] || (r[3] = _ => s(t).state.settings.general.auth_hash = _),
+                        validation: l.value && B.auth_user ? "required|length:6" : "",
                         help: "Hier das Passwort für BudgeTeer angeben.",
                         "help-class": "text-muted",
                         "input-class": "form-control bg-light mb-2",
                         label: "Passwort",
                         "messages-class": "text-danger",
                         name: "auth_hash",
                         "outer-class": "mb-4",
                         placeholder: "Bspw. ●●●●●●●●",
                         type: "password",
                         "validation-visibility": "live"
                     }, null, 8, ["modelValue", "validation"])])])])]),
                     _: 1
-                })])) : f("", !0), e("div", null, [s(t).state.misc.loaded_settings ? (o(), a("button", {
+                })])) : v("", !0), e("div", null, [s(t).state.misc.loaded_settings ? (a(), i("button", {
                     key: 0,
                     class: "btn btn-primary mt-4",
                     type: "submit",
-                    onClick: u
-                }, [n.value ? (o(), a("span", St)) : f("", !0), n.value ? f("", !0) : (o(), a("i", Bt)), w(" Speichern ")])) : (o(), a("button", Vt, [Kt, w(" Lädt... ")]))])])])])
+                    onClick: p
+                }, [n.value ? (a(), i("span", Bt)) : v("", !0), n.value ? v("", !0) : (a(), i("i", St)), $(" Speichern ")])) : (a(), i("button", Vt, [Tt, $(" Lädt... ")]))])])])])
             }
         }
     },
-    Tt = {
+    Nt = {
         class: "container"
     },
-    Dt = {
+    Ut = {
         class: "row my-3"
     },
-    Ut = {
+    Dt = {
         class: "col-md-10 offset-md-1"
     },
-    Et = {
+    Mt = {
         class: "card text-center shadow my-3"
     },
-    Ft = e("div", {
+    Et = e("div", {
         class: "card-header"
     }, [e("h1", null, [e("i", {
         class: "bi bi-clock-history"
-    }), w(" Offene Transaktionen ")])], -1),
-    Mt = {
+    }), $(" Offene Transaktionen ")])], -1),
+    Ft = {
         class: "card-body"
     },
     jt = {
         class: "row justify-content-center mt-2"
     },
     Ot = {
         class: "input-group"
     },
-    Lt = {
+    Pt = {
         class: "input-group-prepend"
     },
-    Pt = ["onUpdate:modelValue"],
+    Lt = ["onUpdate:modelValue"],
     Rt = ["onUpdate:modelValue"],
-    Gt = e("div", {
+    zt = e("div", {
         class: "input-group-append"
     }, [e("span", {
         class: "input-group-text"
     }, " €")], -1),
-    zt = {
+    It = {
         class: "input-group-append"
     },
-    At = ["onClick"],
-    It = e("i", {
+    Gt = ["onClick"],
+    Wt = e("i", {
         class: "bi bi-arrow-up"
     }, null, -1),
-    Yt = [It],
-    Ht = ["onClick"],
-    Wt = e("i", {
+    At = [Wt],
+    Yt = ["onClick"],
+    Ht = e("i", {
         class: "bi bi-arrow-down"
     }, null, -1),
-    qt = [Wt],
+    qt = [Ht],
     Xt = ["onClick"],
     Qt = e("i", {
         class: "bi bi-trash3"
     }, null, -1),
     Zt = [Qt],
     Jt = {
         class: "row justify-content-center mt-2"
     },
     xt = {
         __name: "Transactions",
-        setup(p) {
-            const t = T(),
-                v = D();
+        setup(h) {
+            const t = N(),
+                m = U();
             t.commit("getOpenTransactions");
 
-            function g(n) {
-                S.post("api/json/" + n + "/", t.state.data.open_transactions).then(function() {
+            function f(n) {
+                C.post("api/json/" + n + "/", t.state.data.open_transactions).then(function() {
                     console.log(n + " gespeichert.")
                 }, function() {
-                    t.commit("getSettings"), console.log("Konnte " + n + " nicht speichern!"), v.error("Konnte " + n + " nicht speichern!")
+                    t.commit("getSettings"), console.log("Konnte " + n + " nicht speichern!"), m.error("Konnte " + n + " nicht speichern!")
                 })
             }
-            return (n, l) => (o(), a("div", Tt, [e("div", Dt, [e("div", Ut, [e("div", Et, [Ft, e("div", Mt, [e("div", jt, [(o(!0), a(E, null, j(s(t).state.data.open_transactions, (u, c) => (o(), a("div", {
-                key: u,
+            return (n, l) => (a(), i("div", Nt, [e("div", Ut, [e("div", Dt, [e("div", Mt, [Et, e("div", Ft, [e("div", jt, [(a(!0), i(E, null, O(s(t).state.data.open_transactions, (p, c) => (a(), i("div", {
+                key: p,
                 class: "transaction"
-            }, [e("div", Ot, [e("div", Lt, [V(e("input", {
-                "onUpdate:modelValue": i => s(t).state.data.open_transactions[c].label = i,
+            }, [e("div", Ot, [e("div", Pt, [V(e("input", {
+                "onUpdate:modelValue": r => s(t).state.data.open_transactions[c].label = r,
                 class: "form-control"
-            }, null, 8, Pt), [
-                [N, s(t).state.data.open_transactions[c].label]
+            }, null, 8, Lt), [
+                [K, s(t).state.data.open_transactions[c].label]
             ])]), V(e("input", {
-                "onUpdate:modelValue": i => s(t).state.data.open_transactions[c].amount = i,
+                "onUpdate:modelValue": r => s(t).state.data.open_transactions[c].amount = r,
                 type: "number",
                 step: "0.01",
                 class: "form-control"
             }, null, 8, Rt), [
-                [N, s(t).state.data.open_transactions[c].amount]
-            ]), Gt, e("div", zt, [e("button", {
+                [K, s(t).state.data.open_transactions[c].amount]
+            ]), zt, e("div", It, [e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: i => s(t).state.data.open_transactions.splice(c - 1, 0, s(t).state.data.open_transactions.splice(c, 1)[0])
-            }, Yt, 8, At), e("button", {
+                onClick: r => s(t).state.data.open_transactions.splice(c - 1, 0, s(t).state.data.open_transactions.splice(c, 1)[0])
+            }, At, 8, Gt), e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: i => s(t).state.data.open_transactions.splice(c + 1, 0, s(t).state.data.open_transactions.splice(c, 1)[0])
-            }, qt, 8, Ht), e("button", {
+                onClick: r => s(t).state.data.open_transactions.splice(c + 1, 0, s(t).state.data.open_transactions.splice(c, 1)[0])
+            }, qt, 8, Yt), e("button", {
                 class: "btn btn-outline-danger",
                 type: "button",
-                onClick: i => s(t).state.data.open_transactions.splice(c, 1)
+                onClick: r => s(t).state.data.open_transactions.splice(c, 1)
             }, Zt, 8, Xt)])])]))), 128)), e("div", Jt, [e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: l[0] || (l[0] = u => s(t).state.data.open_transactions.push({
+                onClick: l[0] || (l[0] = p => s(t).state.data.open_transactions.push({
                     label: "",
                     amount: ""
                 }))
             }, " Transaktion hinzufügen "), e("button", {
                 class: "btn btn-outline-success",
                 type: "button",
-                onClick: l[1] || (l[1] = u => g("open_transactions"))
+                onClick: l[1] || (l[1] = p => f("open_transactions"))
             }, " Speichern ")])])])])])])]))
         }
     },
     te = {
         class: "container"
     },
     ee = {
         class: "row my-3"
     },
     se = {
         class: "col-md-10 offset-md-1"
     },
-    ne = {
+    oe = {
         class: "card text-center shadow my-3"
     },
-    oe = e("div", {
+    ne = e("div", {
         class: "card-header"
     }, [e("h1", null, [e("i", {
         class: "bi bi-bar-chart-line-fill"
-    }), w(" Kontostände ")])], -1),
+    }), $(" Kontostände ")])], -1),
     ae = {
         class: "card-body"
     },
     ie = {
         class: "row justify-content-center mt-2"
     },
     le = {
@@ -486,145 +511,145 @@
     be = ["disabled", "onUpdate:modelValue"],
     _e = e("option", {
         value: "checking"
     }, "Girokonto", -1),
     he = e("option", {
         value: "savings"
     }, "Sparkonto", -1),
-    me = [_e, he],
-    ge = {
+    ge = [_e, he],
+    me = {
         key: 1,
         class: "input-group-append"
     },
     fe = ["onClick"],
     ve = e("i", {
         class: "bi bi-arrow-up"
     }, null, -1),
     ke = [ve],
     $e = ["onClick"],
     ye = e("i", {
         class: "bi bi-arrow-down"
     }, null, -1),
     we = [ye],
     Ce = ["onClick"],
-    Se = e("i", {
+    Be = e("i", {
         class: "bi bi-trash3"
     }, null, -1),
-    Be = [Se],
+    Se = [Be],
     Ve = {
         key: 0,
         class: "row justify-content-center mt-2"
     },
-    Ke = {
+    Te = {
         __name: "Balances",
-        setup(p) {
-            const t = T(),
-                v = D();
+        setup(h) {
+            const t = N(),
+                m = U();
             t.commit("getBalances");
 
-            function g(n) {
-                S.post("api/json/" + n + "/", t.state.data.balances).then(function() {
+            function f(n) {
+                C.post("api/json/" + n + "/", t.state.data.balances).then(function() {
                     console.log(n + " gespeichert.")
                 }, function() {
-                    t.commit("getSettings"), console.log("Konnte " + n + " nicht speichern!"), v.error("Konnte " + n + " nicht speichern!")
+                    t.commit("getSettings"), console.log("Konnte " + n + " nicht speichern!"), m.error("Konnte " + n + " nicht speichern!")
                 })
             }
-            return (n, l) => (o(), a("div", te, [e("div", ee, [e("div", se, [e("div", ne, [oe, e("div", ae, [e("div", ie, [(o(!0), a(E, null, j(s(t).state.data.balances, (u, c) => (o(), a("div", {
-                key: u,
+            return (n, l) => (a(), i("div", te, [e("div", ee, [e("div", se, [e("div", oe, [ne, e("div", ae, [e("div", ie, [(a(!0), i(E, null, O(s(t).state.data.balances, (p, c) => (a(), i("div", {
+                key: p,
                 class: "balance"
             }, [e("div", le, [e("div", ce, [V(e("input", {
                 disabled: s(t).state.locked,
-                "onUpdate:modelValue": i => s(t).state.data.balances[c].label = i,
+                "onUpdate:modelValue": r => s(t).state.data.balances[c].label = r,
                 class: "form-control"
             }, null, 8, re), [
-                [N, s(t).state.data.balances[c].label]
+                [K, s(t).state.data.balances[c].label]
             ])]), V(e("input", {
                 disabled: s(t).state.locked,
-                "onUpdate:modelValue": i => s(t).state.data.balances[c].balance = i,
+                "onUpdate:modelValue": r => s(t).state.data.balances[c].balance = r,
                 type: "number",
                 step: "0.01",
                 class: "form-control"
             }, null, 8, de), [
-                [N, s(t).state.data.balances[c].balance]
-            ]), ue, s(t).state.locked ? f("", !0) : (o(), a("div", pe, [V(e("select", {
+                [K, s(t).state.data.balances[c].balance]
+            ]), ue, s(t).state.locked ? v("", !0) : (a(), i("div", pe, [V(e("select", {
                 disabled: s(t).state.locked,
-                "onUpdate:modelValue": i => s(t).state.data.balances[c].type = i,
+                "onUpdate:modelValue": r => s(t).state.data.balances[c].type = r,
                 class: "form-control"
-            }, me, 8, be), [
-                [z, s(t).state.data.balances[c].type]
-            ])])), s(t).state.locked ? f("", !0) : (o(), a("div", ge, [e("button", {
+            }, ge, 8, be), [
+                [I, s(t).state.data.balances[c].type]
+            ])])), s(t).state.locked ? v("", !0) : (a(), i("div", me, [e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: i => s(t).state.data.balances.splice(c - 1, 0, s(t).state.data.balances.splice(c, 1)[0])
+                onClick: r => s(t).state.data.balances.splice(c - 1, 0, s(t).state.data.balances.splice(c, 1)[0])
             }, ke, 8, fe), e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: i => s(t).state.data.balances.splice(c + 1, 0, s(t).state.data.balances.splice(c, 1)[0])
+                onClick: r => s(t).state.data.balances.splice(c + 1, 0, s(t).state.data.balances.splice(c, 1)[0])
             }, we, 8, $e), e("button", {
                 class: "btn btn-outline-danger",
                 type: "button",
-                onClick: i => s(t).state.data.balances.splice(c, 1)
-            }, Be, 8, Ce)]))])]))), 128)), s(t).state.locked ? f("", !0) : (o(), a("div", Ve, [e("button", {
+                onClick: r => s(t).state.data.balances.splice(c, 1)
+            }, Se, 8, Ce)]))])]))), 128)), s(t).state.locked ? v("", !0) : (a(), i("div", Ve, [e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: l[0] || (l[0] = u => s(t).state.data.balances.push({
+                onClick: l[0] || (l[0] = p => s(t).state.data.balances.push({
                     label: "",
                     amount: ""
                 }))
             }, " Konto hinzufügen "), e("button", {
                 class: "btn btn-outline-success",
                 type: "button",
-                onClick: l[1] || (l[1] = u => g("balances"))
+                onClick: l[1] || (l[1] = p => f("balances"))
             }, " Speichern ")]))])])])])])]))
         }
     },
-    Ne = {
+    Ke = {
         class: "container"
     },
-    Te = {
+    Ne = {
         class: "row my-3"
     },
-    De = {
+    Ue = {
         class: "col-md-10 offset-md-1"
     },
-    Ue = {
+    De = {
         class: "card text-center shadow my-3"
     },
-    Ee = {
+    Me = {
         class: "card-header"
     },
-    Fe = e("i", {
+    Ee = e("i", {
         class: "bi bi-currency-euro"
     }, null, -1),
-    Me = {
+    Fe = {
         class: "col-md-auto p-1"
     },
     je = ["disabled"],
     Oe = e("i", {
         class: "bi bi-arrow-left"
     }, null, -1),
-    Le = [Oe],
-    Pe = ["disabled"],
+    Pe = [Oe],
+    Le = ["disabled"],
     Re = e("i", {
         class: "bi bi-arrow-right"
     }, null, -1),
-    Ge = [Re],
-    ze = {
+    ze = [Re],
+    Ie = {
         class: "card-body"
     },
-    Ae = {
+    Ge = {
         class: "row justify-content-center mt-2"
     },
-    Ie = {
+    We = {
         class: "accordion",
         id: "accordionBudgets"
     },
-    Ye = ["id"],
-    He = ["data-bs-target", "aria-controls"],
-    We = ["id", "aria-labelledby"],
+    Ae = ["id"],
+    Ye = ["data-bs-target", "aria-controls"],
+    He = ["id", "aria-labelledby"],
     qe = {
         class: "accordion-body"
     },
     Xe = {
         key: 0,
         class: "input-group"
     },
@@ -642,16 +667,16 @@
         key: 0,
         class: "input-group-append"
     },
     es = ["onClick"],
     ss = e("i", {
         class: "bi bi-x"
     }, null, -1),
-    ns = [ss],
-    os = ["onClick"],
+    os = [ss],
+    ns = ["onClick"],
     as = e("i", {
         class: "bi bi-arrow-up"
     }, null, -1),
     is = [as],
     ls = ["onClick"],
     cs = e("i", {
         class: "bi bi-arrow-down"
@@ -665,232 +690,232 @@
     bs = {
         class: "input-group-append"
     },
     _s = ["onClick"],
     hs = e("i", {
         class: "bi bi-check2"
     }, null, -1),
-    ms = [hs],
-    gs = {
+    gs = [hs],
+    ms = {
         key: 1
     },
     fs = ["onClick"],
     vs = {
         class: "row justify-content-center mt-2"
     },
     ks = {
         __name: "Budgets",
-        setup(p) {
-            const t = T(),
-                v = D();
+        setup(h) {
+            const t = N(),
+                m = U();
             t.commit("getBudgets");
 
-            function g(d) {
-                S.post("api/json/" + d + "/", t.state.data.budgets).then(function() {
+            function f(d) {
+                C.post("api/json/" + d + "/", t.state.data.budgets).then(function() {
                     console.log(d + " gespeichert.")
                 }, function() {
-                    t.commit("getSettings"), console.log("Konnte " + d + " nicht speichern!"), v.error("Konnte " + d + " nicht speichern!")
+                    t.commit("getSettings"), console.log("Konnte " + d + " nicht speichern!"), m.error("Konnte " + d + " nicht speichern!")
                 })
             }
 
             function n(d) {
                 return parseFloat(d).toFixed(2)
             }
 
             function l(d) {
-                let h = 0;
-                for (let k = 0; k < t.state.data.budgets[d].entries.length; k++)
-                    if (!u || !t.state.data.budgets[d].entries[k].booked || !u()) {
-                        let r = parseFloat(t.state.data.budgets[d].entries[k].amount);
-                        isNaN(r) || (h += r)
-                    } return n(h)
+                let b = 0;
+                for (let u = 0; u < t.state.data.budgets[d].entries.length; u++)
+                    if (!p || !t.state.data.budgets[d].entries[u].booked || !p()) {
+                        let o = parseFloat(t.state.data.budgets[d].entries[u].amount);
+                        isNaN(o) || (b += o)
+                    } return n(b)
             }
 
-            function u() {
+            function p() {
                 let d = new Date(c.value),
-                    h = new Date;
-                return d.getMonth() === h.getMonth() && d.getFullYear() === h.getFullYear()
+                    b = new Date;
+                return d.getMonth() === b.getMonth() && d.getFullYear() === b.getFullYear()
             }
-            const c = K(new Date().toISOString().slice(0, 7)),
-                i = K(0);
+            const c = T(new Date().toISOString().slice(0, 7)),
+                r = T(0);
 
             function y(d) {
-                i.value += d;
-                let h = new Date().setMonth(new Date().getMonth() + i.value);
-                c.value = new Date(h).toISOString().slice(0, 7)
+                r.value += d;
+                let b = new Date().setMonth(new Date().getMonth() + r.value);
+                c.value = new Date(b).toISOString().slice(0, 7)
             }
 
-            function b(d) {
-                return t.state.locked && u() ? !d.booked && _(d) : !0
+            function B(d) {
+                return t.state.locked && p() ? !d.booked && _(d) : !0
             }
 
             function _(d) {
-                let h = new Date(c.value),
-                    k = new Date("1970-01-01"),
-                    r = new Date("2100-01-01");
-                return d.valid_from_to[0] !== null && (k = new Date(d.valid_from_to[0])), d.valid_from_to[1] !== null && (r = new Date(d.valid_from_to[1])), h >= k && h <= r
+                let b = new Date(c.value),
+                    u = new Date("1970-01-01"),
+                    o = new Date("2100-01-01");
+                return d.valid_from_to[0] !== null && (u = new Date(d.valid_from_to[0])), d.valid_from_to[1] !== null && (o = new Date(d.valid_from_to[1])), b >= u && b <= o
             }
-            return (d, h) => (o(), a("div", Ne, [e("div", Te, [e("div", De, [e("div", Ue, [e("div", Ee, [e("h1", null, [Fe, w(" Budgets " + B(c.value), 1)]), e("div", Me, [e("button", {
-                disabled: i.value <= 0,
+            return (d, b) => (a(), i("div", Ke, [e("div", Ne, [e("div", Ue, [e("div", De, [e("div", Me, [e("h1", null, [Ee, $(" Budgets " + S(c.value), 1)]), e("div", Fe, [e("button", {
+                disabled: r.value <= 0,
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: h[0] || (h[0] = k => y(-1))
-            }, Le, 8, je), e("button", {
-                disabled: i.value >= 13,
+                onClick: b[0] || (b[0] = u => y(-1))
+            }, Pe, 8, je), e("button", {
+                disabled: r.value >= 13,
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: h[1] || (h[1] = k => y(1))
-            }, Ge, 8, Pe)])]), e("div", ze, [e("div", Ae, [e("div", Ie, [(o(!0), a(E, null, j(s(t).state.data.budgets, (k, r) => (o(), a("div", {
-                key: k,
+                onClick: b[1] || (b[1] = u => y(1))
+            }, ze, 8, Le)])]), e("div", Ie, [e("div", Ge, [e("div", We, [(a(!0), i(E, null, O(s(t).state.data.budgets, (u, o) => (a(), i("div", {
+                key: u,
                 class: "accordion-item"
             }, [e("h2", {
                 class: "accordion-header",
-                id: "heading" + r
+                id: "heading" + o
             }, [e("button", {
                 class: "accordion-button collapsed",
                 type: "button",
                 "data-bs-toggle": "collapse",
-                "data-bs-target": "#collapse" + r,
+                "data-bs-target": "#collapse" + o,
                 "aria-expanded": "false",
-                "aria-controls": "collapse" + r
-            }, B(s(t).state.data.budgets[r].category) + ": " + B(l(r)) + " € ", 9, He)], 8, Ye), e("div", {
-                id: "collapse" + r,
+                "aria-controls": "collapse" + o
+            }, S(s(t).state.data.budgets[o].category) + ": " + S(l(o)) + " € ", 9, Ye)], 8, Ae), e("div", {
+                id: "collapse" + o,
                 class: "accordion-collapse collapse",
-                "aria-labelledby": "heading" + r,
+                "aria-labelledby": "heading" + o,
                 "data-bs-parent": "#accordionBudgets"
-            }, [e("div", qe, [(o(!0), a(E, null, j(s(t).state.data.budgets[r].entries, (O, m) => (o(), a("div", {
-                key: O
-            }, [b(s(t).state.data.budgets[r].entries[m]) ? (o(), a("div", Xe, [e("div", Qe, [V(e("input", {
+            }, [e("div", qe, [(a(!0), i(E, null, O(s(t).state.data.budgets[o].entries, (M, g) => (a(), i("div", {
+                key: M
+            }, [B(s(t).state.data.budgets[o].entries[g]) ? (a(), i("div", Xe, [e("div", Qe, [V(e("input", {
                 disabled: s(t).state.locked,
-                "onUpdate:modelValue": C => s(t).state.data.budgets[r].entries[m].label = C,
+                "onUpdate:modelValue": w => s(t).state.data.budgets[o].entries[g].label = w,
                 class: "form-control"
             }, null, 8, Ze), [
-                [N, s(t).state.data.budgets[r].entries[m].label]
+                [K, s(t).state.data.budgets[o].entries[g].label]
             ])]), V(e("input", {
                 disabled: s(t).state.locked,
-                "onUpdate:modelValue": C => s(t).state.data.budgets[r].entries[m].amount = C,
+                "onUpdate:modelValue": w => s(t).state.data.budgets[o].entries[g].amount = w,
                 type: "number",
                 step: "0.01",
                 class: "form-control"
             }, null, 8, Je), [
-                [N, s(t).state.data.budgets[r].entries[m].amount]
-            ]), xe, s(t).state.locked ? f("", !0) : (o(), a("div", ts, [u() && s(t).state.data.budgets[r].entries[m].booked ? (o(), a("button", {
+                [K, s(t).state.data.budgets[o].entries[g].amount]
+            ]), xe, s(t).state.locked ? v("", !0) : (a(), i("div", ts, [p() && s(t).state.data.budgets[o].entries[g].booked ? (a(), i("button", {
                 key: 0,
                 class: "btn btn-outline-danger",
                 type: "button",
-                onClick: C => s(t).state.data.budgets[r].entries[m].booked = !1
-            }, ns, 8, es)) : f("", !0), e("button", {
+                onClick: w => s(t).state.data.budgets[o].entries[g].booked = !1
+            }, os, 8, es)) : v("", !0), e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: C => s(t).state.data.budgets[r].entries.splice(m - 1, 0, s(t).state.data.budgets[r].entries.splice(m, 1)[r])
-            }, is, 8, os), e("button", {
+                onClick: w => s(t).state.data.budgets[o].entries.splice(g - 1, 0, s(t).state.data.budgets[o].entries.splice(g, 1)[o])
+            }, is, 8, ns), e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: C => s(t).state.data.budgets[r].entries.splice(m + 1, 0, s(t).state.data.budgets[r].entries.splice(m, 1)[r])
+                onClick: w => s(t).state.data.budgets[o].entries.splice(g + 1, 0, s(t).state.data.budgets[o].entries.splice(g, 1)[o])
             }, rs, 8, ls), e("button", {
                 class: "btn btn-outline-danger",
                 type: "button",
-                onClick: C => s(t).state.data.budgets[r].entries.splice(m, 1)
-            }, ps, 8, ds)])), e("div", bs, [u() && s(t).state.locked && !s(t).state.data.budgets[r].entries[m].booked ? (o(), a("button", {
+                onClick: w => s(t).state.data.budgets[o].entries.splice(g, 1)
+            }, ps, 8, ds)])), e("div", bs, [p() && s(t).state.locked && !s(t).state.data.budgets[o].entries[g].booked ? (a(), i("button", {
                 key: 0,
                 class: "btn btn-outline-success",
                 type: "button",
-                onClick: C => s(t).state.data.budgets[r].entries[m].booked = !0
-            }, ms, 8, _s)) : f("", !0)])])) : f("", !0), s(t).state.locked ? f("", !0) : (o(), a("div", gs, [w(" Aktiv: " + B(s(t).state.data.budgets[r].entries[m].valid_from_to) + " ", 1), $(s(J), {
-                value: s(t).state.data.budgets[r].entries[m].valid_from_to,
-                "onUpdate:value": C => s(t).state.data.budgets[r].entries[m].valid_from_to = C,
+                onClick: w => s(t).state.data.budgets[o].entries[g].booked = !0
+            }, gs, 8, _s)) : v("", !0)])])) : v("", !0), s(t).state.locked ? v("", !0) : (a(), i("div", ms, [$(" Aktiv: " + S(s(t).state.data.budgets[o].entries[g].valid_from_to) + " ", 1), k(s(J), {
+                value: s(t).state.data.budgets[o].entries[g].valid_from_to,
+                "onUpdate:value": w => s(t).state.data.budgets[o].entries[g].valid_from_to = w,
                 type: "month",
                 format: "MMMM YYYY",
                 range: "true"
-            }, null, 8, ["value", "onUpdate:value"])]))]))), 128)), s(t).state.locked ? f("", !0) : (o(), a("button", {
+            }, null, 8, ["value", "onUpdate:value"])]))]))), 128)), s(t).state.locked ? v("", !0) : (a(), i("button", {
                 key: 0,
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: O => s(t).state.data.budgets[r].entries.push({
+                onClick: M => s(t).state.data.budgets[o].entries.push({
                     label: "",
                     amount: "",
                     valid_from_to: [null, null],
                     booked: !1
                 })
-            }, " Eintrag hinzufügen ", 8, fs))])], 8, We)]))), 128))]), e("div", vs, [s(t).state.locked ? f("", !0) : (o(), a("button", {
+            }, " Eintrag hinzufügen ", 8, fs))])], 8, He)]))), 128))]), e("div", vs, [s(t).state.locked ? v("", !0) : (a(), i("button", {
                 key: 0,
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: h[2] || (h[2] = k => s(t).state.data.budgets.push({
+                onClick: b[2] || (b[2] = u => s(t).state.data.budgets.push({
                     category: "ToDo",
                     amount: "",
                     entries: []
                 }))
             }, " Kategorie hinzufügen ")), e("button", {
                 class: "btn btn-outline-success",
                 type: "button",
-                onClick: h[3] || (h[3] = k => g("budgets"))
+                onClick: b[3] || (b[3] = u => f("budgets"))
             }, " Speichern ")])])])])])])]))
         }
     },
     $s = {
         __name: "_Main",
-        setup(p) {
-            return (t, v) => (o(), a("main", null, [$(bt), $(xt), $(Ke), $(ks), $(Nt)]))
+        setup(h) {
+            return (t, m) => (a(), i("main", null, [k(bt), k(xt), k(Te), k(ks), k(Kt)]))
         }
     },
-    ys = Y({
-        history: H(),
+    ys = A({
+        history: Y(),
         routes: [{
             path: "/:pathMatch(.*)*",
             component: $s
         }]
     });
 const ws = {
         class: "sticky-bottom float-end"
     },
     Cs = e("i", {
         class: "bi bi-unlock"
     }, null, -1),
-    Ss = [Cs],
-    Bs = e("i", {
+    Bs = [Cs],
+    Ss = e("i", {
         class: "bi bi-lock"
     }, null, -1),
-    Vs = [Bs],
-    Ks = {
+    Vs = [Ss],
+    Ts = {
         key: 0,
         class: "bi bi-sun"
     },
-    Ns = {
+    Ks = {
         key: 1,
         class: "bi bi-moon-stars"
     },
-    Ts = {
+    Ns = {
         __name: "App",
-        setup(p) {
+        setup(h) {
             const t = tt(),
-                v = et(t),
-                g = T();
+                m = et(t),
+                f = N();
             return (n, l) => {
-                const u = P("router-view");
-                return o(), a(E, null, [$(u), e("div", ws, [s(g).state.locked ? (o(), a("button", {
+                const p = L("router-view");
+                return a(), i(E, null, [k(p), e("div", ws, [s(f).state.locked ? (a(), i("button", {
                     key: 0,
                     class: "btn btn-outline-success",
                     type: "button",
-                    onClick: l[0] || (l[0] = c => s(g).commit("setLocked", !1))
-                }, Ss)) : (o(), a("button", {
+                    onClick: l[0] || (l[0] = c => s(f).commit("setLocked", !1))
+                }, Bs)) : (a(), i("button", {
                     key: 1,
                     class: "btn btn-outline-danger",
                     type: "button",
-                    onClick: l[1] || (l[1] = c => s(g).commit("setLocked", !0))
+                    onClick: l[1] || (l[1] = c => s(f).commit("setLocked", !0))
                 }, Vs)), e("button", {
                     type: "button",
                     class: "btn btn-outline-secondary bg-dark m-3 text-warning",
-                    onClick: l[2] || (l[2] = c => s(v)())
-                }, [s(t) ? (o(), a("i", Ks)) : (o(), a("i", Ns))])])], 64)
+                    onClick: l[2] || (l[2] = c => s(m)())
+                }, [s(t) ? (a(), i("i", Ts)) : (a(), i("i", Ks))])])], 64)
             }
         }
     },
-    M = D(),
-    Ds = I({
+    j = U(),
+    Us = W({
         state() {
             return {
                 data: {
                     balances: [],
                     open_transactions: [],
                     budgets: []
                 },
@@ -899,54 +924,54 @@
                 misc: {
                     loaded_settings: !1,
                     docker: !1
                 }
             }
         },
         mutations: {
-            getSettings(p) {
-                S.get("api/settings/").then(function(t) {
-                    p.settings = t.data.settings, p.misc.loaded_settings = !0
+            getSettings(h) {
+                C.get("api/settings/").then(function(t) {
+                    h.settings = t.data.settings, h.misc.loaded_settings = !0
                 }, function() {
-                    console.log("Konnte Einstellungen nicht abrufen!"), M.error("Konnte Einstellungen nicht abrufen!")
+                    console.log("Konnte Einstellungen nicht abrufen!"), j.error("Konnte Einstellungen nicht abrufen!")
                 })
             },
-            getBalances(p) {
-                S.get("api/json/balances/").then(function(t) {
-                    p.data.balances = t.data.balances
+            getBalances(h) {
+                C.get("api/json/balances/").then(function(t) {
+                    h.data.balances = t.data.balances
                 }, function() {
-                    console.log("Konnte Kontostände nicht abrufen!"), M.error("Konnte Kontostände nicht abrufen!")
+                    console.log("Konnte Kontostände nicht abrufen!"), j.error("Konnte Kontostände nicht abrufen!")
                 })
             },
-            getOpenTransactions(p) {
-                S.get("api/json/open_transactions/").then(function(t) {
-                    p.data.open_transactions = t.data.open_transactions
+            getOpenTransactions(h) {
+                C.get("api/json/open_transactions/").then(function(t) {
+                    h.data.open_transactions = t.data.open_transactions
                 }, function() {
-                    console.log("Konnte offene Transaktionen nicht abrufen!"), M.error("Konnte offene Transaktionen nicht abrufen!")
+                    console.log("Konnte offene Transaktionen nicht abrufen!"), j.error("Konnte offene Transaktionen nicht abrufen!")
                 })
             },
-            getBudgets(p) {
-                S.get("api/json/budgets/").then(function(t) {
-                    p.data.budgets = t.data.budgets
+            getBudgets(h) {
+                C.get("api/json/budgets/").then(function(t) {
+                    h.data.budgets = t.data.budgets
                 }, function() {
-                    console.log("Konnte Budgets nicht abrufen!"), M.error("Konnte Budgets nicht abrufen!")
+                    console.log("Konnte Budgets nicht abrufen!"), j.error("Konnte Budgets nicht abrufen!")
                 })
             },
-            setDocker(p, t) {
-                p.misc.docker = t
+            setDocker(h, t) {
+                h.misc.docker = t
             },
-            setLocked(p, t) {
-                p.locked = t
+            setLocked(h, t) {
+                h.locked = t
             }
         }
     }),
-    U = A(Ts);
-U.use(Ds);
-U.use(ys);
-U.use(W, {
+    D = G(Ns);
+D.use(Us);
+D.use(ys);
+D.use(H, {
     position: "top-center",
     draggable: !1,
     maxToasts: 1,
     bodyClassName: ["toast-body"],
     toastDefaults: {
         [F.ERROR]: {
             icon: "bi bi-exclamation-triangle"
@@ -959,15 +984,15 @@
         },
         [F.SUCCESS]: {
             icon: "bi bi-check-circle-fill",
             timeout: 3e3
         }
     }
 });
-U.use(x);
-U.use(X, Q({
+D.use(x);
+D.use(X, Q({
     locales: {
         de: Z
     },
     locale: "de"
 }));
-U.mount("#app");
+D.mount("#app");
```

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-datepicker-next-3bf3781e.css` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-datepicker-next-3bf3781e.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-datepicker-next-98f94a3e.js` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-datepicker-next-98f94a3e.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-b19737a8.js` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-b19737a8.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-86ed02bf.js` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-86ed02bf.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-22d603d9.js` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-22d603d9.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-39f44738.js` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-39f44738.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/vuejs_frontend/dist/index.html` & `budgeteer-0.0.2/budgeteer/web_interface/vuejs_frontend/dist/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <head>
     <meta charset="UTF-8">
     <meta content="width=device-width, initial-scale=1, shrink-to-fit=no" name="viewport">
 
     <link href="./favicon.ico" rel="icon" type="image/x-icon">
 
     <title>BudgeTeer</title>
-  <script type="module" crossorigin src="./assets/index-f9a1f1e7.js"></script>
+  <script type="module" crossorigin src="./assets/index-93e69acd.js"></script>
   <link rel="modulepreload" crossorigin href="./assets/@vue-4b662da7.js">
   <link rel="modulepreload" crossorigin href="./assets/vuex-39f44738.js">
   <link rel="modulepreload" crossorigin href="./assets/axios-4a70c6fc.js">
   <link rel="modulepreload" crossorigin href="./assets/vue-router-b19737a8.js">
   <link rel="modulepreload" crossorigin href="./assets/@popperjs-8746c87e.js">
   <link rel="modulepreload" crossorigin href="./assets/bootstrap-85852bd1.js">
   <link rel="modulepreload" crossorigin href="./assets/vue-toastification-22d603d9.js">
```

### Comparing `budgeteer-0.0.1/budgeteer/web_interface/web_server.py` & `budgeteer-0.0.2/budgeteer/web_interface/web_server.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.0.1/budgeteer.egg-info/PKG-INFO` & `budgeteer-0.0.2/budgeteer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: budgeteer
-Version: 0.0.1
-Summary: Automate downloads using predefined sites and the My JDownloader API
+Version: 0.0.2
+Summary: Einfacher Überblick über das eigene Budget
 Home-page: https://github.com/rix1337/BudgeTeer
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `budgeteer-0.0.1/budgeteer.egg-info/SOURCES.txt` & `budgeteer-0.0.2/budgeteer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css
 budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
 budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css
 budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
 budgeteer/web_interface/vuejs_frontend/dist/assets/date-format-parse-388037e5.js
+budgeteer/web_interface/vuejs_frontend/dist/assets/index-93e69acd.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css
-budgeteer/web_interface/vuejs_frontend/dist/assets/index-f9a1f1e7.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
 budgeteer/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/vue-datepicker-next-3bf3781e.css
 budgeteer/web_interface/vuejs_frontend/dist/assets/vue-datepicker-next-98f94a3e.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-b19737a8.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-86ed02bf.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-22d603d9.js
```

### Comparing `budgeteer-0.0.1/setup.py` & `budgeteer-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     required = f.read().splitlines()
 
 setuptools.setup(
     name="budgeteer",
     version=get_version(),
     author="rix1337",
     author_email="",
-    description="Automate downloads using predefined sites and the My JDownloader API",
+    description="Einfacher Überblick über das eigene Budget",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rix1337/BudgeTeer",
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=required,
     zip_safe=False,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

