# Comparing `tmp/flask-sqlalchemy-api-0.9.2.tar.gz` & `tmp/flask-sqlalchemy-api-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-sqlalchemy-api-0.9.2.tar", last modified: Fri Jul 28 14:46:33 2023, max compression
+gzip compressed data, was "flask-sqlalchemy-api-0.9.3.tar", last modified: Sat Jul 29 16:53:53 2023, max compression
```

## Comparing `flask-sqlalchemy-api-0.9.2.tar` & `flask-sqlalchemy-api-0.9.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-28 14:46:33.640259 flask-sqlalchemy-api-0.9.2/
--rw-r--r--   0 abc        (911) abc        (911)       39 2023-07-08 16:27:48.000000 flask-sqlalchemy-api-0.9.2/AUTHORS.txt
--rw-r--r--   0 abc        (911) abc        (911)      224 2023-07-08 17:52:28.000000 flask-sqlalchemy-api-0.9.2/CHANGES.md
--rw-r--r--   0 abc        (911) abc        (911)      450 2023-07-08 16:27:48.000000 flask-sqlalchemy-api-0.9.2/CLASSIFIERS.txt
--rw-r--r--   0 abc        (911) abc        (911)      177 2023-07-08 17:25:46.000000 flask-sqlalchemy-api-0.9.2/MANIFEST.in
--rw-r--r--   0 abc        (911) abc        (911)     4823 2023-07-28 14:46:33.640259 flask-sqlalchemy-api-0.9.2/PKG-INFO
--rw-r--r--   0 abc        (911) abc        (911)     3662 2023-07-28 14:39:20.000000 flask-sqlalchemy-api-0.9.2/README.md
--rw-r--r--   0 abc        (911) abc        (911)       23 2023-07-08 16:27:48.000000 flask-sqlalchemy-api-0.9.2/REQUIREMENTS.txt
-drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-28 14:46:33.640259 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api/
--rw-r--r--   0 abc        (911) abc        (911)       46 2023-07-26 15:36:37.000000 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api/__init__.py
--rw-r--r--   0 abc        (911) abc        (911)    12581 2023-07-28 14:35:32.000000 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api/main.py
-drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-28 14:46:33.640259 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api.egg-info/
--rw-r--r--   0 abc        (911) abc        (911)     4823 2023-07-28 14:46:33.000000 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api.egg-info/PKG-INFO
--rw-r--r--   0 abc        (911) abc        (911)      410 2023-07-28 14:46:33.000000 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api.egg-info/SOURCES.txt
--rw-r--r--   0 abc        (911) abc        (911)        1 2023-07-28 14:46:33.000000 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api.egg-info/dependency_links.txt
--rw-r--r--   0 abc        (911) abc        (911)        1 2023-07-28 14:46:33.000000 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api.egg-info/not-zip-safe
--rw-r--r--   0 abc        (911) abc        (911)       24 2023-07-28 14:46:33.000000 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api.egg-info/requires.txt
--rw-r--r--   0 abc        (911) abc        (911)       21 2023-07-28 14:46:33.000000 flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api.egg-info/top_level.txt
--rw-r--r--   0 abc        (911) abc        (911)       38 2023-07-28 14:46:33.640259 flask-sqlalchemy-api-0.9.2/setup.cfg
--rw-r--r--   0 abc        (911) abc        (911)     1411 2023-07-28 14:46:26.000000 flask-sqlalchemy-api-0.9.2/setup.py
+drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-29 16:53:53.339340 flask-sqlalchemy-api-0.9.3/
+-rw-r--r--   0 abc        (911) abc        (911)       39 2023-07-08 16:27:48.000000 flask-sqlalchemy-api-0.9.3/AUTHORS.txt
+-rw-r--r--   0 abc        (911) abc        (911)      224 2023-07-08 17:52:28.000000 flask-sqlalchemy-api-0.9.3/CHANGES.md
+-rw-r--r--   0 abc        (911) abc        (911)      450 2023-07-08 16:27:48.000000 flask-sqlalchemy-api-0.9.3/CLASSIFIERS.txt
+-rw-r--r--   0 abc        (911) abc        (911)      177 2023-07-08 17:25:46.000000 flask-sqlalchemy-api-0.9.3/MANIFEST.in
+-rw-r--r--   0 abc        (911) abc        (911)     4952 2023-07-29 16:53:53.339340 flask-sqlalchemy-api-0.9.3/PKG-INFO
+-rw-r--r--   0 abc        (911) abc        (911)     3791 2023-07-28 19:30:59.000000 flask-sqlalchemy-api-0.9.3/README.md
+-rw-r--r--   0 abc        (911) abc        (911)       23 2023-07-08 16:27:48.000000 flask-sqlalchemy-api-0.9.3/REQUIREMENTS.txt
+drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-29 16:53:53.335340 flask-sqlalchemy-api-0.9.3/flask_sqlalchemy_api/
+-rw-r--r--   0 abc        (911) abc        (911)       46 2023-07-26 15:36:37.000000 flask-sqlalchemy-api-0.9.3/flask_sqlalchemy_api/__init__.py
+-rw-r--r--   0 abc        (911) abc        (911)    13068 2023-07-29 16:51:55.000000 flask-sqlalchemy-api-0.9.3/flask_sqlalchemy_api/main.py
+drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-29 16:53:53.339340 flask-sqlalchemy-api-0.9.3/flask_sqlalchemy_api.egg-info/
+-rw-r--r--   0 abc        (911) abc        (911)     4952 2023-07-29 16:53:52.000000 flask-sqlalchemy-api-0.9.3/flask_sqlalchemy_api.egg-info/PKG-INFO
+-rw-r--r--   0 abc        (911) abc        (911)      410 2023-07-29 16:53:52.000000 flask-sqlalchemy-api-0.9.3/flask_sqlalchemy_api.egg-info/SOURCES.txt
+-rw-r--r--   0 abc        (911) abc        (911)        1 2023-07-29 16:53:52.000000 flask-sqlalchemy-api-0.9.3/flask_sqlalchemy_api.egg-info/dependency_links.txt
+-rw-r--r--   0 abc        (911) abc        (911)        1 2023-07-29 16:53:52.000000 flask-sqlalchemy-api-0.9.3/flask_sqlalchemy_api.egg-info/not-zip-safe
+-rw-r--r--   0 abc        (911) abc        (911)       24 2023-07-29 16:53:52.000000 flask-sqlalchemy-api-0.9.3/flask_sqlalchemy_api.egg-info/requires.txt
+-rw-r--r--   0 abc        (911) abc        (911)       21 2023-07-29 16:53:52.000000 flask-sqlalchemy-api-0.9.3/flask_sqlalchemy_api.egg-info/top_level.txt
+-rw-r--r--   0 abc        (911) abc        (911)       38 2023-07-29 16:53:53.339340 flask-sqlalchemy-api-0.9.3/setup.cfg
+-rw-r--r--   0 abc        (911) abc        (911)     1411 2023-07-29 16:51:30.000000 flask-sqlalchemy-api-0.9.3/setup.py
```

### Comparing `flask-sqlalchemy-api-0.9.2/PKG-INFO` & `flask-sqlalchemy-api-0.9.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-sqlalchemy-api
-Version: 0.9.2
+Version: 0.9.3
 Summary: flask-sqlalchemy-api extension for flask application
 Home-page: https://github.com/fraoustin/flask-sqlalchemy-api.git
 Author: Frédéric Aoustin
 Author-email: fraoustin@gmail.com
 License: UNKNOWN
 Platform: any
 Classifier: Programming Language :: Python
@@ -122,14 +122,15 @@
 
 You can 
 
 - specific url (default /api/v1) on ApiRest
 - add decorator (login, ...) in sample/sample1.py
 - specific endpoint
 - specific serialize: transform item to json
+- specific api action on column using the comment of column (add "not create by api", "not visible by api", "not update by api")
 
 ## Sample
 
 You can launch sample 0 and 1
 
     python sample/sample0.py &
     python sample/sample0_test.py
```

### Comparing `flask-sqlalchemy-api-0.9.2/README.md` & `flask-sqlalchemy-api-0.9.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 
 You can 
 
 - specific url (default /api/v1) on ApiRest
 - add decorator (login, ...) in sample/sample1.py
 - specific endpoint
 - specific serialize: transform item to json
+- specific api action on column using the comment of column (add "not create by api", "not visible by api", "not update by api")
 
 ## Sample
 
 You can launch sample 0 and 1
 
     python sample/sample0.py &
     python sample/sample0_test.py
```

### Comparing `flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api/main.py` & `flask-sqlalchemy-api-0.9.3/flask_sqlalchemy_api/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 from sqlalchemy import PrimaryKeyConstraint, UniqueConstraint, Integer, Float, BOOLEAN, Boolean, Enum
 from sqlalchemy.sql import text
 from sqlalchemy.orm.exc import UnmappedInstanceError
 from functools import wraps
 import logging
 import json
 
-__version__ = '0.9.2'
+__version__ = '0.9.3'
 
 SQLTYPE_TO_FLASKTYPE = {Integer: 'int', Float: 'float'}
 SQLTYPE_TO_SWAGGERTYPE = {Integer: 'integer', Float: 'number', BOOLEAN: 'boolean', Boolean: 'boolean'}
 
 
 def model_to_dict(obj):
-    return {c.name: getattr(obj, c.name) for c in obj.__table__.columns}
+    return {c.name: getattr(obj, c.name) for c in obj.__table__.columns if 'not visible by api' not in str(c.comment)}
 
 
 def getConstraint(cls):
     constraint = None
     if len([constraint for constraint in cls.__table__.constraints if isinstance(constraint, UniqueConstraint)]) > 0:
         constraint = [constraint for constraint in cls.__table__.constraints if isinstance(constraint, UniqueConstraint)][0]
     if len([constraint for constraint in cls.__table__.constraints if isinstance(constraint, PrimaryKeyConstraint)]) > 0:
@@ -38,31 +38,31 @@
     def __init__(self, item):
         super().__init__("Item not found %s" % item)
 
 
 def requestBody(obj, method):
     content = {"application/json": {"schema": {"type": "object", "properties": {}}}}
     if method == 'POST':
-        for c in [c for c in obj.__table__.columns if c.autoincrement is not True]:
+        for c in [c for c in obj.__table__.columns if c.autoincrement is not True and 'not create by api' not in str(c.comment)]:
             content["application/json"]["schema"]["properties"][c.name] = {"type": SQLTYPE_TO_SWAGGERTYPE.get(c.type.__class__, 'string')}
             if c.type.__class__ == Enum:
                 content["application/json"]["schema"]["properties"][c.name]["enum"] = [member for member in c]
         return content
     if method in ["PUT", "PATCH"]:
-        for c in obj.__table__.columns:
+        for c in [c for c in obj.__table__.columns if 'not update by api' not in str(c.comment)]:
             content["application/json"]["schema"]["properties"][c.name] = {"type": SQLTYPE_TO_SWAGGERTYPE.get(c.type.__class__, 'string')}
             if c.type.__class__ == Enum:
                 content["application/json"]["schema"]["properties"][c.name]["enum"] = [member for member in c]
         return content
     return None
 
 
 def responseBody(obj, method):
     content = {"application/json": {"schema": {"type": "object", "properties": {}}}}
-    for c in obj.__table__.columns:
+    for c in [c for c in obj.__table__.columns if 'not visible by api' not in str(c.comment)]:
         content["application/json"]["schema"]["properties"][c.name] = {"type": SQLTYPE_TO_SWAGGERTYPE.get(c.type.__class__, 'string')}
         if c.type.__class__ == Enum:
             content["application/json"]["schema"]["properties"][c.name]["enum"] = [member for member in c]
     if method == 'ALL':
         obj = content["application/json"]["schema"]
         content = {"application/json": {"schema": {"type": "array", "items": obj}}}
     return content
@@ -133,15 +133,15 @@
             self.add_url_rule(endpoint, 'patch_%s' % endpoint[1:], multi_decorators(decorators)(self._patch(cls, serialize)), methods=[method, ])
         logging.getLogger("werkzeug").info(" * add url rule %s for %s" % (endpoint, method))
         if endpoint.startswith(self._url_prefix):
             endpoint = endpoint[len(self._url_prefix):]
         if endpoint.split("/")[-1] == unique_endpoint(cls):
             endpoint = endpoint.split("/")[:-1] + ["{%s}" % endpoint.split("/")[-1].split(":")[1][:-1], ]
             endpoint = "/".join(endpoint)
-        swagger = {"paths": {endpoint: {method.lower(): {"tags": [cls.__name__.lower(),], "summary": "", "description": "", "operationId": "%s_%s" % (cls.__name__.lower(), method), "parameters": []}}}}
+        swagger = {"paths": {endpoint: {method.lower(): {"tags": [cls.__name__,], "summary": "", "description": "", "operationId": "%s_%s" % (cls.__name__.lower(), method), "parameters": []}}}}
         for column in parameters:
             parameter = {"name": column.name, "in": "path", "description": "", "required": True, "schema": {"type": SQLTYPE_TO_SWAGGERTYPE.get(column.type.__class__, 'string')}}
             swagger["paths"][endpoint][method.lower()]["parameters"].append(parameter)
         if method in ('POST', 'PUT', 'PATCH'):
             swagger["paths"][endpoint][method.lower()]["requestBody"] = {"description": "", "content": requestBody(cls, _origin_method)}
         swagger["paths"][endpoint][method.lower()]["responses"] = {}
         swagger["paths"][endpoint][method.lower()]["responses"]["200"] = {"description": "Successful operation", "content": responseBody(cls, _origin_method)}
@@ -161,14 +161,17 @@
         def fct(**kws):
             dct = {key: request.form.get(key) for key in request.form}
             if len(dct) == 0:
                 dct = json.loads(request.get_data())
             for col in [c.name for c in cls.__table__.columns if c.autoincrement is True]:
                 if col in dct:
                     del dct[col]
+            for col in [c.name for c in cls.__table__.columns if 'not create by api' in str(c.comment)]:
+                if col in dct:
+                    del dct[col]
             item = cls(**dct)
             self._db.session.add(item)
             self._db.session.commit()
             return serialize(item), 201
         return fct
 
     def _get(self, cls, serialize):
@@ -189,29 +192,29 @@
         def fct(**kws):
             item = self._db.one_or_404(self._db.select(cls).filter_by(**kws), description=f"{cls.__name__} with parameters {','.join(['%s:%s' % (kw, kws[kw]) for kw in kws])}.")
             dct = {key: request.form.get(key) for key in request.form}
             if len(dct) == 0:
                 dct = json.loads(request.get_data())
             for key in kws:
                 dct[key] = kws[key]
-            for col in [c.name for c in item.__table__.columns]:
+            for col in [c.name for c in item.__table__.columns if 'not update by api' not in str(c.comment)]:
                 item.__setattr__(col, dct.get(col))
             self._db.session.commit()
             return serialize(item), 200
         return fct
 
     def _patch(self, cls, serialize):
         def fct(**kws):
             item = self._db.one_or_404(self._db.select(cls).filter_by(**kws), description=f"{cls.__name__} with parameters {','.join(['%s:%s' % (kw, kws[kw]) for kw in kws])}.")
             dct = {key: request.form.get(key) for key in request.form}
             if len(dct) == 0:
                 dct = json.loads(request.get_data())
             for key in kws:
                 dct[key] = kws[key]
-            for col in [key for key in dct if key in item.__table__.columns]:
+            for col in [key for key in dct if key in item.__table__.columns and 'not update by api' not in str(item.__table__.columns[key].comment)]:
                 item.__setattr__(col, dct.get(col))
             self._db.session.commit()
             return serialize(item), 200
         return fct
 
     def register(self, app, options):
         try:
```

### Comparing `flask-sqlalchemy-api-0.9.2/flask_sqlalchemy_api.egg-info/PKG-INFO` & `flask-sqlalchemy-api-0.9.3/flask_sqlalchemy_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-sqlalchemy-api
-Version: 0.9.2
+Version: 0.9.3
 Summary: flask-sqlalchemy-api extension for flask application
 Home-page: https://github.com/fraoustin/flask-sqlalchemy-api.git
 Author: Frédéric Aoustin
 Author-email: fraoustin@gmail.com
 License: UNKNOWN
 Platform: any
 Classifier: Programming Language :: Python
@@ -122,14 +122,15 @@
 
 You can 
 
 - specific url (default /api/v1) on ApiRest
 - add decorator (login, ...) in sample/sample1.py
 - specific endpoint
 - specific serialize: transform item to json
+- specific api action on column using the comment of column (add "not create by api", "not visible by api", "not update by api")
 
 ## Sample
 
 You can launch sample 0 and 1
 
     python sample/sample0.py &
     python sample/sample0_test.py
```

### Comparing `flask-sqlalchemy-api-0.9.2/setup.py` & `flask-sqlalchemy-api-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     Setup for flask-sqlalchemy-api
 """
 
 import os
 from setuptools import setup, find_packages
 
-__version_info__ = (0, 9, 2)
+__version_info__ = (0, 9, 3)
 VERSION = '.'.join([str(val) for val in __version_info__])
 NAME = "flask-sqlalchemy-api"
 DESC = "flask-sqlalchemy-api extension for flask application"
 URLPKG = "https://github.com/fraoustin/flask-sqlalchemy-api.git"
 
 HERE = os.path.abspath(os.path.dirname(__file__))
```

