# Comparing `tmp/drf-gears-0.6.23.tar.gz` & `tmp/drf-gears-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-gears-0.6.23.tar", last modified: Sat Jul 29 15:29:40 2023, max compression
+gzip compressed data, was "drf-gears-0.6.9.tar", last modified: Wed Aug 31 19:33:46 2022, max compression
```

## Comparing `drf-gears-0.6.23.tar` & `drf-gears-0.6.9.tar`

### file list

```diff
@@ -1,39 +1,37 @@
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-07-29 15:29:40.615768 drf-gears-0.6.23/
--rw-r--r--   0 alexander   (501) staff       (20)     1069 2022-08-31 14:23:16.000000 drf-gears-0.6.23/LICENSE
--rw-r--r--   0 alexander   (501) staff       (20)     9865 2023-07-29 15:29:40.614410 drf-gears-0.6.23/PKG-INFO
--rw-r--r--   0 alexander   (501) staff       (20)     8080 2022-08-31 06:54:14.000000 drf-gears-0.6.23/README.md
--rw-r--r--   0 alexander   (501) staff       (20)      553 2023-07-29 15:29:29.000000 drf-gears-0.6.23/pyproject.toml
--rw-r--r--   0 alexander   (501) staff       (20)       38 2023-07-29 15:29:40.615915 drf-gears-0.6.23/setup.cfg
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-07-29 15:29:40.593485 drf-gears-0.6.23/src/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 17:27:37.000000 drf-gears-0.6.23/src/__init__.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-07-29 15:29:40.595705 drf-gears-0.6.23/src/drf_gears.egg-info/
--rw-r--r--   0 alexander   (501) staff       (20)     9865 2023-07-29 15:29:40.000000 drf-gears-0.6.23/src/drf_gears.egg-info/PKG-INFO
--rw-r--r--   0 alexander   (501) staff       (20)      780 2023-07-29 15:29:40.000000 drf-gears-0.6.23/src/drf_gears.egg-info/SOURCES.txt
--rw-r--r--   0 alexander   (501) staff       (20)        1 2023-07-29 15:29:40.000000 drf-gears-0.6.23/src/drf_gears.egg-info/dependency_links.txt
--rw-r--r--   0 alexander   (501) staff       (20)       15 2023-07-29 15:29:40.000000 drf-gears-0.6.23/src/drf_gears.egg-info/top_level.txt
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-07-29 15:29:40.597615 drf-gears-0.6.23/src/gears/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 17:27:25.000000 drf-gears-0.6.23/src/gears/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)       43 2022-08-31 14:30:39.000000 drf-gears-0.6.23/src/gears/example.py
--rw-r--r--   0 alexander   (501) staff       (20)      523 2022-08-22 18:21:05.000000 drf-gears-0.6.23/src/gears/mixins.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-07-29 15:29:40.601055 drf-gears-0.6.23/src/gears/models/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.6.23/src/gears/models/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)     2287 2023-07-29 15:29:29.000000 drf-gears-0.6.23/src/gears/models/change.py
--rw-r--r--   0 alexander   (501) staff       (20)     3669 2022-08-31 20:29:26.000000 drf-gears-0.6.23/src/gears/models/jwt.py
--rw-r--r--   0 alexander   (501) staff       (20)      993 2022-09-15 17:18:53.000000 drf-gears-0.6.23/src/gears/models/singleton.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-07-29 15:29:40.607853 drf-gears-0.6.23/src/gears/renderers/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:39:27.000000 drf-gears-0.6.23/src/gears/renderers/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)     3346 2023-02-28 09:58:58.000000 drf-gears-0.6.23/src/gears/renderers/exception_handlers.py
--rw-r--r--   0 alexander   (501) staff       (20)      314 2022-08-31 16:39:41.000000 drf-gears-0.6.23/src/gears/renderers/mapping.py
--rw-r--r--   0 alexander   (501) staff       (20)     1795 2022-08-31 16:39:48.000000 drf-gears-0.6.23/src/gears/renderers/renderer.py
--rw-r--r--   0 alexander   (501) staff       (20)      385 2022-08-31 16:39:54.000000 drf-gears-0.6.23/src/gears/renderers/types.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-07-29 15:29:40.609023 drf-gears-0.6.23/src/gears/serializers/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.6.23/src/gears/serializers/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)      481 2022-08-31 16:40:18.000000 drf-gears-0.6.23/src/gears/serializers/jwt.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-07-29 15:29:40.610320 drf-gears-0.6.23/src/gears/views/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.6.23/src/gears/views/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)      353 2022-08-31 20:02:15.000000 drf-gears-0.6.23/src/gears/views/jwt.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-07-29 15:29:40.612806 drf-gears-0.6.23/src/gears/viewsets/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.6.23/src/gears/viewsets/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)      724 2022-08-31 16:40:43.000000 drf-gears-0.6.23/src/gears/viewsets/permissions.py
--rw-r--r--   0 alexander   (501) staff       (20)     1096 2022-08-31 16:40:48.000000 drf-gears-0.6.23/src/gears/viewsets/querysets.py
--rw-r--r--   0 alexander   (501) staff       (20)     1153 2022-08-31 16:40:56.000000 drf-gears-0.6.23/src/gears/viewsets/serializers.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-31 19:33:46.297888 drf-gears-0.6.9/
+-rw-r--r--   0 alexander   (501) staff       (20)     1069 2022-08-31 14:23:16.000000 drf-gears-0.6.9/LICENSE
+-rw-r--r--   0 alexander   (501) staff       (20)     9864 2022-08-31 19:33:46.297608 drf-gears-0.6.9/PKG-INFO
+-rw-r--r--   0 alexander   (501) staff       (20)     8080 2022-08-31 06:54:14.000000 drf-gears-0.6.9/README.md
+-rw-r--r--   0 alexander   (501) staff       (20)      552 2022-08-31 19:33:36.000000 drf-gears-0.6.9/pyproject.toml
+-rw-r--r--   0 alexander   (501) staff       (20)       38 2022-08-31 19:33:46.297980 drf-gears-0.6.9/setup.cfg
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-31 19:33:46.284198 drf-gears-0.6.9/src/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 17:27:37.000000 drf-gears-0.6.9/src/__init__.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-31 19:33:46.285231 drf-gears-0.6.9/src/drf_gears.egg-info/
+-rw-r--r--   0 alexander   (501) staff       (20)     9864 2022-08-31 19:33:46.000000 drf-gears-0.6.9/src/drf_gears.egg-info/PKG-INFO
+-rw-r--r--   0 alexander   (501) staff       (20)      723 2022-08-31 19:33:46.000000 drf-gears-0.6.9/src/drf_gears.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander   (501) staff       (20)        1 2022-08-31 19:33:46.000000 drf-gears-0.6.9/src/drf_gears.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander   (501) staff       (20)       15 2022-08-31 19:33:46.000000 drf-gears-0.6.9/src/drf_gears.egg-info/top_level.txt
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-31 19:33:46.286974 drf-gears-0.6.9/src/gears/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 17:27:25.000000 drf-gears-0.6.9/src/gears/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)       43 2022-08-31 14:30:39.000000 drf-gears-0.6.9/src/gears/example.py
+-rw-r--r--   0 alexander   (501) staff       (20)      523 2022-08-22 18:21:05.000000 drf-gears-0.6.9/src/gears/mixins.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-31 19:33:46.287975 drf-gears-0.6.9/src/gears/models/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.6.9/src/gears/models/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)     3770 2022-08-31 16:38:57.000000 drf-gears-0.6.9/src/gears/models/jwt.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-31 19:33:46.291837 drf-gears-0.6.9/src/gears/renderers/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:39:27.000000 drf-gears-0.6.9/src/gears/renderers/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)     3034 2022-08-31 16:39:35.000000 drf-gears-0.6.9/src/gears/renderers/exception_handlers.py
+-rw-r--r--   0 alexander   (501) staff       (20)      314 2022-08-31 16:39:41.000000 drf-gears-0.6.9/src/gears/renderers/mapping.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1795 2022-08-31 16:39:48.000000 drf-gears-0.6.9/src/gears/renderers/renderer.py
+-rw-r--r--   0 alexander   (501) staff       (20)      385 2022-08-31 16:39:54.000000 drf-gears-0.6.9/src/gears/renderers/types.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-31 19:33:46.293178 drf-gears-0.6.9/src/gears/serializers/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.6.9/src/gears/serializers/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)      481 2022-08-31 16:40:18.000000 drf-gears-0.6.9/src/gears/serializers/jwt.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-31 19:33:46.294063 drf-gears-0.6.9/src/gears/views/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.6.9/src/gears/views/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)      351 2022-08-31 17:10:11.000000 drf-gears-0.6.9/src/gears/views/jwt.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-08-31 19:33:46.296606 drf-gears-0.6.9/src/gears/viewsets/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2022-08-31 16:41:07.000000 drf-gears-0.6.9/src/gears/viewsets/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)      724 2022-08-31 16:40:43.000000 drf-gears-0.6.9/src/gears/viewsets/permissions.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1096 2022-08-31 16:40:48.000000 drf-gears-0.6.9/src/gears/viewsets/querysets.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1153 2022-08-31 16:40:56.000000 drf-gears-0.6.9/src/gears/viewsets/serializers.py
```

### Comparing `drf-gears-0.6.23/LICENSE` & `drf-gears-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-gears-0.6.23/PKG-INFO` & `drf-gears-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-gears
-Version: 0.6.23
+Version: 0.6.9
 Summary: Some gears collection for getting life a little bit better.
 Author-email: Alexander Yudkin <san4ezy@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `drf-gears-0.6.23/README.md` & `drf-gears-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `drf-gears-0.6.23/pyproject.toml` & `drf-gears-0.6.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "drf-gears"
-version = "0.6.23"
+version = "0.6.9"
 authors = [
   { name="Alexander Yudkin", email="san4ezy@gmail.com" },
 ]
 description = "Some gears collection for getting life a little bit better."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `drf-gears-0.6.23/src/drf_gears.egg-info/PKG-INFO` & `drf-gears-0.6.9/src/drf_gears.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-gears
-Version: 0.6.23
+Version: 0.6.9
 Summary: Some gears collection for getting life a little bit better.
 Author-email: Alexander Yudkin <san4ezy@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `drf-gears-0.6.23/src/drf_gears.egg-info/SOURCES.txt` & `drf-gears-0.6.9/src/drf_gears.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 src/drf_gears.egg-info/SOURCES.txt
 src/drf_gears.egg-info/dependency_links.txt
 src/drf_gears.egg-info/top_level.txt
 src/gears/__init__.py
 src/gears/example.py
 src/gears/mixins.py
 src/gears/models/__init__.py
-src/gears/models/change.py
 src/gears/models/jwt.py
-src/gears/models/singleton.py
 src/gears/renderers/__init__.py
 src/gears/renderers/exception_handlers.py
 src/gears/renderers/mapping.py
 src/gears/renderers/renderer.py
 src/gears/renderers/types.py
 src/gears/serializers/__init__.py
 src/gears/serializers/jwt.py
```

### Comparing `drf-gears-0.6.23/src/gears/mixins.py` & `drf-gears-0.6.9/src/gears/mixins.py`

 * *Files identical despite different names*

### Comparing `drf-gears-0.6.23/src/gears/models/jwt.py` & `drf-gears-0.6.9/src/gears/models/jwt.py`

 * *Files 11% similar despite different names*

```diff
@@ -68,15 +68,17 @@
         """
         This method must return a payload dictionary. Fill this method with needed logic
         for building a sensitive data payload you want to put into the token.
         
         :return: a payload dict 
         """
         
-        return {}
+        raise NotImplemented(
+            "You should override this method with a specific payload builder."
+        )
 
     def extend_token(self, token):
         """
         It takes a fresh token and extends it with an additional payload.
         There are two options: get_public_jwt_data and get_private_jwt_data. 
         :param token: a fresh valid RefreshToken
         :return: an extended RefreshToken
```

### Comparing `drf-gears-0.6.23/src/gears/renderers/exception_handlers.py` & `drf-gears-0.6.9/src/gears/renderers/exception_handlers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,65 @@
 from copy import copy
 
 from django.core.exceptions import PermissionDenied
-from django.http import Http404, HttpResponseNotFound
-from gears.renderers.mapping import RESPONSE_ERROR_MAPPING
-from gears.renderers.types import Error
+from django.http import Http404
 from rest_framework import exceptions
 from rest_framework import status
 
 from rest_framework.response import Response
 from rest_framework.views import set_rollback
 
+from .types import Error
+from .mapping import RESPONSE_ERROR_MAPPING
+
 
 class ExceptionHandler(object):
     default_code: str = 'unknown_error'
     default_description: str = 'Unknown error'
     default_status_code: str = status.HTTP_500_INTERNAL_SERVER_ERROR
     root_field_name: str = 'errors'
 
     def __init__(self, exc, context):
         self.exc = exc
         self.context = context
-        self.status_code = None
+        self.status_code = exc.status_code or self.default_status_code
         self.errors: list = []
         self.data = {}
-        self.headers = {}
 
     def _super(self):
         exc = self.exc
-        headers = {}
         if isinstance(exc, Http404):
-            exc = HttpResponseNotFound()
+            exc = exceptions.NotFound()
         elif isinstance(exc, PermissionDenied):
             exc = exceptions.PermissionDenied()
 
-        try:
-            self.status_code = exc.status_code
-        except AttributeError:
-            self.status_code = self.default_status_code
-
         if isinstance(exc, exceptions.APIException):
+            headers = {}
             if getattr(exc, 'auth_header', None):
                 headers['WWW-Authenticate'] = exc.auth_header
             if getattr(exc, 'wait', None):
                 headers['Retry-After'] = '%d' % exc.wait
             set_rollback()
 
             self.data = exc.detail
-        else:
-            self.data = str(exc)
-        self.headers = headers
-        self.exc = exc
+            self.exc = exc
+            self.headers = headers
 
     def process_list(self, detail: list, location):
         for v in detail:
             self.process(v, location=location)
 
     def process_dict(self, detail: dict, location):
         for k, v in detail.items():
             self.process(v, location=k)
 
     def process_error(self, detail, location):
-        if status.is_server_error(self.status_code):
-            raise self.exc
         self.errors.append(
             Error(
-                code=getattr(detail, 'code', self.default_code),
+                code=detail.code or self.default_code,
                 location=location,
                 description=str(detail) or self.default_description,
                 detail=None,
             )
         )
 
     def process(self, detail, location: str = None):
```

### Comparing `drf-gears-0.6.23/src/gears/renderers/renderer.py` & `drf-gears-0.6.9/src/gears/renderers/renderer.py`

 * *Files identical despite different names*

### Comparing `drf-gears-0.6.23/src/gears/viewsets/permissions.py` & `drf-gears-0.6.9/src/gears/viewsets/permissions.py`

 * *Files identical despite different names*

### Comparing `drf-gears-0.6.23/src/gears/viewsets/querysets.py` & `drf-gears-0.6.9/src/gears/viewsets/querysets.py`

 * *Files identical despite different names*

### Comparing `drf-gears-0.6.23/src/gears/viewsets/serializers.py` & `drf-gears-0.6.9/src/gears/viewsets/serializers.py`

 * *Files identical despite different names*

