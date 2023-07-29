# Comparing `tmp/casbin-django-orm-adapter-1.0.2.tar.gz` & `tmp/casbin-django-orm-adapter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casbin-django-orm-adapter-1.0.2.tar", last modified: Mon Aug 15 00:54:53 2022, max compression
+gzip compressed data, was "casbin-django-orm-adapter-1.0.3.tar", last modified: Sat Jul 29 13:59:22 2023, max compression
```

## Comparing `casbin-django-orm-adapter-1.0.2.tar` & `casbin-django-orm-adapter-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 00:54:53.330249 casbin-django-orm-adapter-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-15 00:54:16.000000 casbin-django-orm-adapter-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4198 2022-08-15 00:54:53.330249 casbin-django-orm-adapter-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3474 2022-08-15 00:54:16.000000 casbin-django-orm-adapter-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 00:54:53.326249 casbin-django-orm-adapter-1.0.2/casbin_adapter/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-15 00:54:16.000000 casbin-django-orm-adapter-1.0.2/casbin_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-08-15 00:54:16.000000 casbin-django-orm-adapter-1.0.2/casbin_adapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-08-15 00:54:16.000000 casbin-django-orm-adapter-1.0.2/casbin_adapter/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-08-15 00:54:16.000000 casbin-django-orm-adapter-1.0.2/casbin_adapter/enforcer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 00:54:53.326249 casbin-django-orm-adapter-1.0.2/casbin_adapter/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-08-15 00:54:16.000000 casbin-django-orm-adapter-1.0.2/casbin_adapter/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-15 00:54:16.000000 casbin-django-orm-adapter-1.0.2/casbin_adapter/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-08-15 00:54:16.000000 casbin-django-orm-adapter-1.0.2/casbin_adapter/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-08-15 00:54:16.000000 casbin-django-orm-adapter-1.0.2/casbin_adapter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 00:54:53.330249 casbin-django-orm-adapter-1.0.2/casbin_django_orm_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4198 2022-08-15 00:54:53.000000 casbin-django-orm-adapter-1.0.2/casbin_django_orm_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-08-15 00:54:53.000000 casbin-django-orm-adapter-1.0.2/casbin_django_orm_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-15 00:54:53.000000 casbin-django-orm-adapter-1.0.2/casbin_django_orm_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-15 00:54:53.000000 casbin-django-orm-adapter-1.0.2/casbin_django_orm_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-15 00:54:53.000000 casbin-django-orm-adapter-1.0.2/casbin_django_orm_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-08-15 00:54:16.000000 casbin-django-orm-adapter-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-08-15 00:54:53.330249 casbin-django-orm-adapter-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-08-15 00:54:16.000000 casbin-django-orm-adapter-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:59:22.587983 casbin-django-orm-adapter-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-29 13:59:22.587983 casbin-django-orm-adapter-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:59:22.587983 casbin-django-orm-adapter-1.0.3/casbin_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/casbin_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/casbin_adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/casbin_adapter/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/casbin_adapter/enforcer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:59:22.587983 casbin-django-orm-adapter-1.0.3/casbin_adapter/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/casbin_adapter/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/casbin_adapter/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/casbin_adapter/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/casbin_adapter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:59:22.587983 casbin-django-orm-adapter-1.0.3/casbin_django_orm_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-29 13:59:22.000000 casbin-django-orm-adapter-1.0.3/casbin_django_orm_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-29 13:59:22.000000 casbin-django-orm-adapter-1.0.3/casbin_django_orm_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 13:59:22.000000 casbin-django-orm-adapter-1.0.3/casbin_django_orm_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 13:59:22.000000 casbin-django-orm-adapter-1.0.3/casbin_django_orm_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 13:59:22.000000 casbin-django-orm-adapter-1.0.3/casbin_django_orm_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-29 13:59:22.587983 casbin-django-orm-adapter-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:59:22.587983 casbin-django-orm-adapter-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/tests/test_adapter.py
```

### Comparing `casbin-django-orm-adapter-1.0.2/LICENSE` & `casbin-django-orm-adapter-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.0.2/PKG-INFO` & `casbin-django-orm-adapter-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: casbin-django-orm-adapter
-Version: 1.0.2
+Version: 1.0.3
 Summary: Django's ORM adapter for PyCasbin
 Home-page: https://github.com/pycasbin/django-orm-adapter
 Author: Yang Luo
 Author-email: hsluoyz@qq.com
 License: Apache 2.0
 Keywords: casbin,adapter,storage-driver,django,orm,django-orm,access-control,authorization
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django ORM Adapter for PyCasbin
@@ -84,17 +85,14 @@
 ```
 
 ## Configuration
 
 ### `CASBIN_MODEL`
 A string containing the file location of your casbin model.
 
-### `CASBIN_LOG_ENABLED`
-If `True`, enables logging. `False` by default.
-
 ### `CASBIN_ADAPTER`
 A string containing the adapter import path. Defaults to the django adapter shipped with this package: `casbin_adapter.adapter.Adapter`
 
 ### `CASBIN_ADAPTER_ARGS`
 A tuple of arguments to be passed into the constructor of the adapter specified
 in `CASBIN_ADAPTER`. Refer to adapters to see available arguments.
```

### Comparing `casbin-django-orm-adapter-1.0.2/README.md` & `casbin-django-orm-adapter-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,17 +65,14 @@
 ```
 
 ## Configuration
 
 ### `CASBIN_MODEL`
 A string containing the file location of your casbin model.
 
-### `CASBIN_LOG_ENABLED`
-If `True`, enables logging. `False` by default.
-
 ### `CASBIN_ADAPTER`
 A string containing the adapter import path. Defaults to the django adapter shipped with this package: `casbin_adapter.adapter.Adapter`
 
 ### `CASBIN_ADAPTER_ARGS`
 A tuple of arguments to be passed into the constructor of the adapter specified
 in `CASBIN_ADAPTER`. Refer to adapters to see available arguments.
```

### Comparing `casbin-django-orm-adapter-1.0.2/casbin_adapter/adapter.py` & `casbin-django-orm-adapter-1.0.3/casbin_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.0.2/casbin_adapter/enforcer.py` & `casbin-django-orm-adapter-1.0.3/casbin_adapter/enforcer.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,14 @@
             logger.info("Deferring casbin enforcer initialisation until django is ready")
 
     def _load(self):
         if self._initialized == False:
             logger.info("Performing deferred casbin enforcer initialisation")
             self._initialized = True
             model = getattr(settings, "CASBIN_MODEL")
-            enable_log = getattr(settings, "CASBIN_LOG_ENABLED", False)
             adapter_loc = getattr(settings, "CASBIN_ADAPTER", "casbin_adapter.adapter.Adapter")
             adapter_args = getattr(settings, "CASBIN_ADAPTER_ARGS", tuple())
             Adapter = import_class(adapter_loc)
             adapter = Adapter(*adapter_args)
 
             super().__init__(model, adapter)
             logger.debug("Casbin enforcer initialised")
```

### Comparing `casbin-django-orm-adapter-1.0.2/casbin_adapter/migrations/0001_initial.py` & `casbin-django-orm-adapter-1.0.3/casbin_adapter/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.0.2/casbin_adapter/models.py` & `casbin-django-orm-adapter-1.0.3/casbin_adapter/models.py`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.0.2/casbin_django_orm_adapter.egg-info/PKG-INFO` & `casbin-django-orm-adapter-1.0.3/casbin_django_orm_adapter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: casbin-django-orm-adapter
-Version: 1.0.2
+Version: 1.0.3
 Summary: Django's ORM adapter for PyCasbin
 Home-page: https://github.com/pycasbin/django-orm-adapter
 Author: Yang Luo
 Author-email: hsluoyz@qq.com
 License: Apache 2.0
 Keywords: casbin,adapter,storage-driver,django,orm,django-orm,access-control,authorization
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django ORM Adapter for PyCasbin
@@ -84,17 +85,14 @@
 ```
 
 ## Configuration
 
 ### `CASBIN_MODEL`
 A string containing the file location of your casbin model.
 
-### `CASBIN_LOG_ENABLED`
-If `True`, enables logging. `False` by default.
-
 ### `CASBIN_ADAPTER`
 A string containing the adapter import path. Defaults to the django adapter shipped with this package: `casbin_adapter.adapter.Adapter`
 
 ### `CASBIN_ADAPTER_ARGS`
 A tuple of arguments to be passed into the constructor of the adapter specified
 in `CASBIN_ADAPTER`. Refer to adapters to see available arguments.
```

### Comparing `casbin-django-orm-adapter-1.0.2/casbin_django_orm_adapter.egg-info/SOURCES.txt` & `casbin-django-orm-adapter-1.0.3/casbin_django_orm_adapter.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,8 +11,9 @@
 casbin_adapter/utils.py
 casbin_adapter/migrations/0001_initial.py
 casbin_adapter/migrations/__init__.py
 casbin_django_orm_adapter.egg-info/PKG-INFO
 casbin_django_orm_adapter.egg-info/SOURCES.txt
 casbin_django_orm_adapter.egg-info/dependency_links.txt
 casbin_django_orm_adapter.egg-info/requires.txt
-casbin_django_orm_adapter.egg-info/top_level.txt
+casbin_django_orm_adapter.egg-info/top_level.txt
+tests/test_adapter.py
```

### Comparing `casbin-django-orm-adapter-1.0.2/setup.py` & `casbin-django-orm-adapter-1.0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,12 +19,13 @@
     python_requires=">=3.7",
     license="Apache 2.0",
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     data_files=[desc_file],
 )
```

