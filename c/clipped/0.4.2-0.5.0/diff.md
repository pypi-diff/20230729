# Comparing `tmp/clipped-0.4.2.tar.gz` & `tmp/clipped-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipped-0.4.2.tar", last modified: Fri Jun 30 18:49:07 2023, max compression
+gzip compressed data, was "clipped-0.5.0.tar", last modified: Sat Jul 29 14:27:20 2023, max compression
```

## Comparing `clipped-0.4.2.tar` & `clipped-0.5.0.tar`

### file list

```diff
@@ -1,83 +1,86 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:49:07.753022 clipped-0.4.2/
--rw-r--r--   0 mourad     (501) staff       (20)      174 2023-06-30 18:47:36.000000 clipped-0.4.2/MANIFEST.in
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-06-30 18:49:07.753114 clipped-0.4.2/PKG-INFO
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:49:07.742477 clipped-0.4.2/clipped/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/__init__.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:49:07.744466 clipped-0.4.2/clipped/config/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/config/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)       91 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/config/constants.py
--rw-r--r--   0 mourad     (501) staff       (20)      312 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/config/contexts.py
--rw-r--r--   0 mourad     (501) staff       (20)       40 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/config/exceptions.py
--rw-r--r--   0 mourad     (501) staff       (20)     8943 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/config/manager.py
--rw-r--r--   0 mourad     (501) staff       (20)     6138 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/config/parser.py
--rw-r--r--   0 mourad     (501) staff       (20)      527 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/config/patch_strategy.py
--rw-r--r--   0 mourad     (501) staff       (20)     4047 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/config/reader.py
--rw-r--r--   0 mourad     (501) staff       (20)    15121 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/config/schema.py
--rw-r--r--   0 mourad     (501) staff       (20)     8892 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/config/spec.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:49:07.745255 clipped-0.4.2/clipped/decorators/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/decorators/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)      646 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/decorators/cached_property.py
--rw-r--r--   0 mourad     (501) staff       (20)     4313 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/decorators/deprecation.py
--rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/decorators/memoization.py
--rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/decorators/signals.py
--rw-r--r--   0 mourad     (501) staff       (20)     6256 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/formatting.py
--rw-r--r--   0 mourad     (501) staff       (20)      824 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/manager_interface.py
--rw-r--r--   0 mourad     (501) staff       (20)      203 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/pkg.py
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/py.typed
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:49:07.747262 clipped-0.4.2/clipped/types/
--rw-r--r--   0 mourad     (501) staff       (20)     3914 2023-06-30 18:47:36.000000 clipped-0.4.2/clipped/types/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     1298 2023-06-30 18:47:36.000000 clipped-0.4.2/clipped/types/docker_image.py
--rw-r--r--   0 mourad     (501) staff       (20)     1889 2023-06-30 18:47:36.000000 clipped-0.4.2/clipped/types/email.py
--rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-06-30 18:47:36.000000 clipped-0.4.2/clipped/types/gcs.py
--rw-r--r--   0 mourad     (501) staff       (20)      698 2023-06-30 18:47:36.000000 clipped-0.4.2/clipped/types/lists.py
--rw-r--r--   0 mourad     (501) staff       (20)      158 2023-06-30 18:47:36.000000 clipped-0.4.2/clipped/types/numbers.py
--rw-r--r--   0 mourad     (501) staff       (20)     1142 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/types/ref_or_obj.py
--rw-r--r--   0 mourad     (501) staff       (20)     1019 2023-06-30 18:47:36.000000 clipped-0.4.2/clipped/types/s3.py
--rw-r--r--   0 mourad     (501) staff       (20)      965 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/types/strings.py
--rw-r--r--   0 mourad     (501) staff       (20)     1265 2023-06-30 18:47:36.000000 clipped-0.4.2/clipped/types/uri.py
--rw-r--r--   0 mourad     (501) staff       (20)      688 2023-06-30 18:47:36.000000 clipped-0.4.2/clipped/types/uuids.py
--rw-r--r--   0 mourad     (501) staff       (20)     3179 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/types/wasb.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:49:07.752893 clipped-0.4.2/clipped/utils/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     1655 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/assertions.py
--rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/bools.py
--rw-r--r--   0 mourad     (501) staff       (20)      143 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/click.py
--rw-r--r--   0 mourad     (501) staff       (20)      665 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/cmd.py
--rw-r--r--   0 mourad     (501) staff       (20)      570 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/coroutine.py
--rw-r--r--   0 mourad     (501) staff       (20)      755 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/csv.py
--rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/dates.py
--rw-r--r--   0 mourad     (501) staff       (20)     3358 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/dicts.py
--rw-r--r--   0 mourad     (501) staff       (20)      496 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/encoding.py
--rw-r--r--   0 mourad     (501) staff       (20)     1100 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/enums.py
--rw-r--r--   0 mourad     (501) staff       (20)     2001 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/env.py
--rw-r--r--   0 mourad     (501) staff       (20)     4737 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/git.py
--rw-r--r--   0 mourad     (501) staff       (20)     1827 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/hashing.py
--rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/http.py
--rw-r--r--   0 mourad     (501) staff       (20)     3363 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/humanize.py
--rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/imports.py
--rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/indentation.py
--rw-r--r--   0 mourad     (501) staff       (20)      420 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/json.py
--rw-r--r--   0 mourad     (501) staff       (20)     1269 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/lists.py
--rw-r--r--   0 mourad     (501) staff       (20)      113 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/logging.py
--rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/np.py
--rw-r--r--   0 mourad     (501) staff       (20)     8476 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/paths.py
--rw-r--r--   0 mourad     (501) staff       (20)      778 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/query_params.py
--rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/requests.py
--rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/responses.py
--rw-r--r--   0 mourad     (501) staff       (20)      595 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/sanitizers.py
--rw-r--r--   0 mourad     (501) staff       (20)      676 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/serialization.py
--rw-r--r--   0 mourad     (501) staff       (20)     2674 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/strings.py
--rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/tz.py
--rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/units.py
--rw-r--r--   0 mourad     (501) staff       (20)      282 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/urls.py
--rw-r--r--   0 mourad     (501) staff       (20)      614 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/validation.py
--rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/versions.py
--rw-r--r--   0 mourad     (501) staff       (20)     1060 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/workers.py
--rw-r--r--   0 mourad     (501) staff       (20)      546 2023-06-30 18:47:37.000000 clipped-0.4.2/clipped/utils/yaml.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:49:07.743012 clipped-0.4.2/clipped.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-06-30 18:49:07.000000 clipped-0.4.2/clipped.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1901 2023-06-30 18:49:07.000000 clipped-0.4.2/clipped.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-06-30 18:49:07.000000 clipped-0.4.2/clipped.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)        8 2023-06-30 18:49:07.000000 clipped-0.4.2/clipped.egg-info/top_level.txt
--rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-06-30 18:49:07.753572 clipped-0.4.2/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-06-30 18:47:36.000000 clipped-0.4.2/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-07-29 14:27:20.429494 clipped-0.5.0/
+-rw-r--r--   0 mourad     (501) staff       (20)      174 2023-07-29 14:25:20.000000 clipped-0.5.0/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-07-29 14:27:20.429582 clipped-0.5.0/PKG-INFO
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-07-29 14:27:20.419759 clipped-0.5.0/clipped/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/__init__.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-07-29 14:27:20.420566 clipped-0.5.0/clipped/compact/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/compact/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3143 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/compact/pydantic.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-07-29 14:27:20.421865 clipped-0.5.0/clipped/config/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/config/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)       91 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/config/constants.py
+-rw-r--r--   0 mourad     (501) staff       (20)      312 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/config/contexts.py
+-rw-r--r--   0 mourad     (501) staff       (20)       40 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/config/exceptions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8943 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/config/manager.py
+-rw-r--r--   0 mourad     (501) staff       (20)     6138 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/config/parser.py
+-rw-r--r--   0 mourad     (501) staff       (20)      527 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/config/patch_strategy.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4047 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/config/reader.py
+-rw-r--r--   0 mourad     (501) staff       (20)    15136 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/config/schema.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8892 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/config/spec.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-07-29 14:27:20.422556 clipped-0.5.0/clipped/decorators/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/decorators/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)      646 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/decorators/cached_property.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4313 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/decorators/deprecation.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/decorators/memoization.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/decorators/signals.py
+-rw-r--r--   0 mourad     (501) staff       (20)     6256 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/formatting.py
+-rw-r--r--   0 mourad     (501) staff       (20)      824 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/manager_interface.py
+-rw-r--r--   0 mourad     (501) staff       (20)      203 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/pkg.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/py.typed
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-07-29 14:27:20.424427 clipped-0.5.0/clipped/types/
+-rw-r--r--   0 mourad     (501) staff       (20)     3929 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/types/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1307 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/types/docker_image.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1883 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/types/email.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1027 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/types/gcs.py
+-rw-r--r--   0 mourad     (501) staff       (20)      707 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/types/lists.py
+-rw-r--r--   0 mourad     (501) staff       (20)      174 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/types/numbers.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1156 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/types/ref_or_obj.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1013 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/types/s3.py
+-rw-r--r--   0 mourad     (501) staff       (20)      974 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/types/strings.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1259 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/types/uri.py
+-rw-r--r--   0 mourad     (501) staff       (20)      713 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/types/uuids.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3173 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/types/wasb.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-07-29 14:27:20.429370 clipped-0.5.0/clipped/utils/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1655 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/assertions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/bools.py
+-rw-r--r--   0 mourad     (501) staff       (20)      143 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/click.py
+-rw-r--r--   0 mourad     (501) staff       (20)      665 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/cmd.py
+-rw-r--r--   0 mourad     (501) staff       (20)      570 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/coroutine.py
+-rw-r--r--   0 mourad     (501) staff       (20)      755 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/csv.py
+-rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/dates.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3358 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/dicts.py
+-rw-r--r--   0 mourad     (501) staff       (20)      496 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/encoding.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1100 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/enums.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2001 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/env.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4737 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/git.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1827 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/hashing.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/http.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3363 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/humanize.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/imports.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/indentation.py
+-rw-r--r--   0 mourad     (501) staff       (20)      420 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/json.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1269 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/lists.py
+-rw-r--r--   0 mourad     (501) staff       (20)      113 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/logging.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/np.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8476 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/paths.py
+-rw-r--r--   0 mourad     (501) staff       (20)      778 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/query_params.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/requests.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/responses.py
+-rw-r--r--   0 mourad     (501) staff       (20)      595 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/sanitizers.py
+-rw-r--r--   0 mourad     (501) staff       (20)      667 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/serialization.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2674 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/strings.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/tz.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/units.py
+-rw-r--r--   0 mourad     (501) staff       (20)      282 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/urls.py
+-rw-r--r--   0 mourad     (501) staff       (20)      614 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/validation.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/versions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1060 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/workers.py
+-rw-r--r--   0 mourad     (501) staff       (20)      546 2023-07-29 14:25:20.000000 clipped-0.5.0/clipped/utils/yaml.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-07-29 14:27:20.420275 clipped-0.5.0/clipped.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-07-29 14:27:20.000000 clipped-0.5.0/clipped.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1957 2023-07-29 14:27:20.000000 clipped-0.5.0/clipped.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2023-07-29 14:27:20.000000 clipped-0.5.0/clipped.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        8 2023-07-29 14:27:20.000000 clipped-0.5.0/clipped.egg-info/top_level.txt
+-rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-07-29 14:27:20.430129 clipped-0.5.0/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-07-29 14:25:20.000000 clipped-0.5.0/setup.py
```

### Comparing `clipped-0.4.2/PKG-INFO` & `clipped-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipped
-Version: 0.4.2
+Version: 0.5.0
 Summary: Common shortcuts and utils.
 Home-page: https://github.com/mmourafiq/clipped
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clipped Version: 0.4.2 Summary: Common shortcuts
+Metadata-Version: 2.1 Name: clipped Version: 0.5.0 Summary: Common shortcuts
 and utils. Home-page: https://github.com/mmourafiq/clipped Author: Mourad
 Mourafiq Author-email: mourad.mourafiq@gmail.com Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com License: Apache 2.0 Keywords:
 cli,configuration,utils,setup Platform: any Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: OS Independent Classifier:
```

### Comparing `clipped-0.4.2/clipped/config/manager.py` & `clipped-0.5.0/clipped/config/manager.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/config/parser.py` & `clipped-0.5.0/clipped/config/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import logging
 
 from typing import Any, Callable, List, Optional, Type, TypeVar
 
-from pydantic import PydanticTypeError, PydanticValueError, StrBytes, ValidationError
-from pydantic.parse import Protocol, load_str_bytes
-from pydantic.tools import NameFactory, _get_parsing_type
-
+from clipped.compact.pydantic import (
+    NameFactory,
+    Protocol,
+    PydanticTypeError,
+    PydanticValueError,
+    StrBytes,
+    ValidationError,
+    _get_parsing_type,
+    load_str_bytes,
+)
 from clipped.config.constants import NO_VALUE_FOUND
 from clipped.config.exceptions import SchemaError
 from clipped.decorators.memoization import memoize
 from clipped.utils.json import orjson_loads
 
 _logger = logging.getLogger("clipped.parser")
```

### Comparing `clipped-0.4.2/clipped/config/patch_strategy.py` & `clipped-0.5.0/clipped/config/patch_strategy.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/config/reader.py` & `clipped-0.5.0/clipped/config/reader.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/config/schema.py` & `clipped-0.5.0/clipped/config/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import functools
 import os
 import pprint
 
 from collections.abc import Mapping
 from typing import Any, Callable, Dict, List, Optional, Set, Union
 
-from pydantic import BaseModel, Extra
-
+from clipped.compact.pydantic import BaseModel, Extra
 from clipped.config.exceptions import SchemaError
 from clipped.config.patch_strategy import PatchStrategy
 from clipped.config.spec import ConfigSpec
 from clipped.utils.dicts import deep_update
 from clipped.utils.humanize import humanize_timesince
 from clipped.utils.json import orjson_dumps, orjson_loads
 from clipped.utils.strings import to_camel_case
```

### Comparing `clipped-0.4.2/clipped/config/spec.py` & `clipped-0.5.0/clipped/config/spec.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/decorators/cached_property.py` & `clipped-0.5.0/clipped/decorators/cached_property.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/decorators/deprecation.py` & `clipped-0.5.0/clipped/decorators/deprecation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/decorators/memoization.py` & `clipped-0.5.0/clipped/decorators/memoization.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/decorators/signals.py` & `clipped-0.5.0/clipped/decorators/signals.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/formatting.py` & `clipped-0.5.0/clipped/formatting.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/manager_interface.py` & `clipped-0.5.0/clipped/manager_interface.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/types/__init__.py` & `clipped-0.5.0/clipped/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 
 from typing import Any, Dict
 
-from pydantic import (
+from clipped.compact.pydantic import (
     ByteSize,
     ConstrainedBytes,
     ConstrainedDate,
     ConstrainedDecimal,
     ConstrainedFloat,
     ConstrainedFrozenSet,
     ConstrainedInt,
@@ -36,15 +36,14 @@
     StrBytes,
     StrictBool,
     StrictBytes,
     StrictFloat,
     StrictInt,
     StrictStr,
 )
-
 from clipped.types.docker_image import ImageStr
 from clipped.types.email import EmailStr
 from clipped.types.gcs import GcsPath
 from clipped.types.lists import ListStr
 from clipped.types.s3 import S3Path
 from clipped.types.strings import GenericStr
 from clipped.types.uri import Uri
```

### Comparing `clipped-0.4.2/clipped/types/docker_image.py` & `clipped-0.5.0/clipped/types/docker_image.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TYPE_CHECKING
 
 from clipped.config.constants import PARAM_REGEX
 
 if TYPE_CHECKING:
-    from pydantic.typing import CallableGenerator
+    from clipped.compact.pydantic import CallableGenerator
 
 
 def validate_image(image, allow_none=False):
     if not image:
         if allow_none:
             return
         else:
```

### Comparing `clipped-0.4.2/clipped/types/email.py` & `clipped-0.5.0/clipped/types/email.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import re
 
 from typing import TYPE_CHECKING
 
-from pydantic import StrictStr
-from pydantic.validators import strict_str_validator
+from clipped.compact.pydantic import StrictStr, strict_str_validator
 
 if TYPE_CHECKING:
-    from pydantic.typing import CallableGenerator
+    from clipped.compact.pydantic import CallableGenerator
 
 
 class EmailStr(StrictStr):
     USER_REGEX = re.compile(
         r"(^[-!#$%&'*+/=?^`{}|~\w]+(\.[-!#$%&'*+/=?^`{}|~\w]+)*\Z"  # dot-atom
         # quoted-string
         r'|^"([\001-\010\013\014\016-\037!#-\[\]-\177]'
```

### Comparing `clipped-0.4.2/clipped/types/gcs.py` & `clipped-0.5.0/clipped/types/s3.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 from typing import TYPE_CHECKING, Any, Dict
 
-from pydantic import AnyUrl
+from clipped.compact.pydantic import AnyUrl
 
 if TYPE_CHECKING:
-    from pydantic.config import BaseConfig
-    from pydantic.fields import ModelField
+    from clipped.compact.pydantic import BaseConfig, ModelField
 
 
-class GcsPath(AnyUrl):
-    allowed_schemes = {"gcs", "gs"}
+class S3Path(AnyUrl):
+    allowed_schemes = {"s3"}
 
     __slots__ = ()
 
     @classmethod
     def validate(
         cls, value: Any, field: "ModelField", config: "BaseConfig"
     ) -> "AnyUrl":
         if isinstance(value, Dict):
             _value = value.get("bucket")
             if not _value:
                 raise ValueError("Received a wrong bucket definition: %s", value)
             if "://" not in _value:
-                _value = "gs://{}".format(_value)
-            blob = value.get("blob")
-            if blob:
-                _value = "{}/{}".format(_value, blob)
+                _value = "s3://{}".format(_value)
+            key = value.get("key")
+            if key:
+                _value = "{}/{}".format(_value, key)
             value = _value
-        return super(GcsPath, cls).validate(value=value, field=field, config=config)
+        return super(S3Path, cls).validate(value=value, field=field, config=config)
 
     def to_param(self):
         return str(self)
 
     @property
     def structured(self):
-        return dict(bucket=self.host, blob=self.path.strip("/"))
+        return dict(bucket=self.host, key=self.path.strip("/"))
```

### Comparing `clipped-0.4.2/clipped/types/lists.py` & `clipped-0.5.0/clipped/types/lists.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TYPE_CHECKING
 
 from clipped.utils.lists import to_list
 
 if TYPE_CHECKING:
-    from pydantic.typing import CallableGenerator
+    from clipped.compact.pydantic import CallableGenerator
 
 
 class ListStr(list):
     @classmethod
     def __get_validators__(cls) -> "CallableGenerator":
         yield cls.validate
```

### Comparing `clipped-0.4.2/clipped/types/ref_or_obj.py` & `clipped-0.5.0/clipped/types/ref_or_obj.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from datetime import datetime, timedelta
 from typing import TYPE_CHECKING, Union
 
-from pydantic import StrictFloat, StrictInt, StrictStr
-from pydantic.validators import strict_str_validator
-
+from clipped.compact.pydantic import (
+    StrictFloat,
+    StrictInt,
+    StrictStr,
+    strict_str_validator,
+)
 from clipped.config.constants import PARAM_REGEX
 
 if TYPE_CHECKING:
-    from pydantic.typing import CallableGenerator
+    from clipped.compact.pydantic import CallableGenerator
 
 
 class RefField(StrictStr):
     @classmethod
     def __get_validators__(cls) -> "CallableGenerator":
         yield strict_str_validator
         yield cls.validate
```

### Comparing `clipped-0.4.2/clipped/types/s3.py` & `clipped-0.5.0/clipped/types/gcs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 from typing import TYPE_CHECKING, Any, Dict
 
-from pydantic import AnyUrl
+from clipped.compact.pydantic import AnyUrl
 
 if TYPE_CHECKING:
-    from pydantic.config import BaseConfig
-    from pydantic.fields import ModelField
+    from clipped.compact.pydantic import BaseConfig, ModelField
 
 
-class S3Path(AnyUrl):
-    allowed_schemes = {"s3"}
+class GcsPath(AnyUrl):
+    allowed_schemes = {"gcs", "gs"}
 
     __slots__ = ()
 
     @classmethod
     def validate(
         cls, value: Any, field: "ModelField", config: "BaseConfig"
     ) -> "AnyUrl":
         if isinstance(value, Dict):
             _value = value.get("bucket")
             if not _value:
                 raise ValueError("Received a wrong bucket definition: %s", value)
             if "://" not in _value:
-                _value = "s3://{}".format(_value)
-            key = value.get("key")
-            if key:
-                _value = "{}/{}".format(_value, key)
+                _value = "gs://{}".format(_value)
+            blob = value.get("blob")
+            if blob:
+                _value = "{}/{}".format(_value, blob)
             value = _value
-        return super(S3Path, cls).validate(value=value, field=field, config=config)
+        return super(GcsPath, cls).validate(value=value, field=field, config=config)
 
     def to_param(self):
         return str(self)
 
     @property
     def structured(self):
-        return dict(bucket=self.host, key=self.path.strip("/"))
+        return dict(bucket=self.host, blob=self.path.strip("/"))
```

### Comparing `clipped-0.4.2/clipped/types/strings.py` & `clipped-0.5.0/clipped/types/strings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import TYPE_CHECKING
 from uuid import UUID
 
 from clipped.utils.json import orjson_dumps
 
 if TYPE_CHECKING:
-    from pydantic.typing import CallableGenerator
+    from clipped.compact.pydantic import CallableGenerator
 
 
 class GenericStr(str):
     @classmethod
     def __get_validators__(cls) -> "CallableGenerator":
         yield cls.validate
```

### Comparing `clipped-0.4.2/clipped/types/uri.py` & `clipped-0.5.0/clipped/types/uri.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import TYPE_CHECKING, Any, Dict
 
-from pydantic import AnyUrl
+from clipped.compact.pydantic import AnyUrl
 
 if TYPE_CHECKING:
-    from pydantic.config import BaseConfig
-    from pydantic.fields import ModelField
+    from clipped.compact.pydantic import BaseConfig, ModelField
 
 
 class Uri(AnyUrl):
     __slots__ = ()
 
     @classmethod
     def validate(
```

### Comparing `clipped-0.4.2/clipped/types/uuids.py` & `clipped-0.5.0/clipped/types/uuids.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import TYPE_CHECKING
 from uuid import UUID
 
-from pydantic import StrictStr
+from clipped.compact.pydantic import StrictStr
 
 if TYPE_CHECKING:
-    from pydantic.typing import CallableGenerator
+    from clipped.compact.pydantic import CallableGenerator
 
 
 class UUIDStr(StrictStr):
     @classmethod
     def __get_validators__(cls) -> "CallableGenerator":
         yield cls.validate
```

### Comparing `clipped-0.4.2/clipped/types/wasb.py` & `clipped-0.5.0/clipped/types/wasb.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import re
 
 from typing import TYPE_CHECKING, Any, Dict
 from urllib.parse import urlparse
 
-from pydantic import AnyUrl
+from clipped.compact.pydantic import AnyUrl
 
 if TYPE_CHECKING:
-    from pydantic.config import BaseConfig
-    from pydantic.fields import ModelField
+    from clipped.compact.pydantic import BaseConfig, ModelField
 
 
 class WasbPath(AnyUrl):
     allowed_schemes = {"https", "wasb", "wasbs", "https", "az", "abfs"}
 
     __slots__ = ()
```

### Comparing `clipped-0.4.2/clipped/utils/assertions.py` & `clipped-0.5.0/clipped/utils/assertions.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/bools.py` & `clipped-0.5.0/clipped/utils/bools.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/cmd.py` & `clipped-0.5.0/clipped/utils/cmd.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/coroutine.py` & `clipped-0.5.0/clipped/utils/coroutine.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/csv.py` & `clipped-0.5.0/clipped/utils/csv.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/dates.py` & `clipped-0.5.0/clipped/utils/dates.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/dicts.py` & `clipped-0.5.0/clipped/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/enums.py` & `clipped-0.5.0/clipped/utils/enums.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/env.py` & `clipped-0.5.0/clipped/utils/env.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/git.py` & `clipped-0.5.0/clipped/utils/git.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/hashing.py` & `clipped-0.5.0/clipped/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/http.py` & `clipped-0.5.0/clipped/utils/http.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/humanize.py` & `clipped-0.5.0/clipped/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/imports.py` & `clipped-0.5.0/clipped/utils/imports.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/indentation.py` & `clipped-0.5.0/clipped/utils/indentation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/lists.py` & `clipped-0.5.0/clipped/utils/lists.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/np.py` & `clipped-0.5.0/clipped/utils/np.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/paths.py` & `clipped-0.5.0/clipped/utils/paths.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/query_params.py` & `clipped-0.5.0/clipped/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/requests.py` & `clipped-0.5.0/clipped/utils/requests.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/responses.py` & `clipped-0.5.0/clipped/utils/responses.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/sanitizers.py` & `clipped-0.5.0/clipped/utils/sanitizers.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/strings.py` & `clipped-0.5.0/clipped/utils/strings.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/tz.py` & `clipped-0.5.0/clipped/utils/tz.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/units.py` & `clipped-0.5.0/clipped/utils/units.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/validation.py` & `clipped-0.5.0/clipped/utils/validation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/versions.py` & `clipped-0.5.0/clipped/utils/versions.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/workers.py` & `clipped-0.5.0/clipped/utils/workers.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped/utils/yaml.py` & `clipped-0.5.0/clipped/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/clipped.egg-info/PKG-INFO` & `clipped-0.5.0/clipped.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipped
-Version: 0.4.2
+Version: 0.5.0
 Summary: Common shortcuts and utils.
 Home-page: https://github.com/mmourafiq/clipped
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clipped Version: 0.4.2 Summary: Common shortcuts
+Metadata-Version: 2.1 Name: clipped Version: 0.5.0 Summary: Common shortcuts
 and utils. Home-page: https://github.com/mmourafiq/clipped Author: Mourad
 Mourafiq Author-email: mourad.mourafiq@gmail.com Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com License: Apache 2.0 Keywords:
 cli,configuration,utils,setup Platform: any Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: OS Independent Classifier:
```

### Comparing `clipped-0.4.2/clipped.egg-info/SOURCES.txt` & `clipped-0.5.0/clipped.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 clipped/manager_interface.py
 clipped/pkg.py
 clipped/py.typed
 clipped.egg-info/PKG-INFO
 clipped.egg-info/SOURCES.txt
 clipped.egg-info/dependency_links.txt
 clipped.egg-info/top_level.txt
+clipped/compact/__init__.py
+clipped/compact/pydantic.py
 clipped/config/__init__.py
 clipped/config/constants.py
 clipped/config/contexts.py
 clipped/config/exceptions.py
 clipped/config/manager.py
 clipped/config/parser.py
 clipped/config/patch_strategy.py
```

### Comparing `clipped-0.4.2/setup.cfg` & `clipped-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `clipped-0.4.2/setup.py` & `clipped-0.5.0/setup.py`

 * *Files identical despite different names*

