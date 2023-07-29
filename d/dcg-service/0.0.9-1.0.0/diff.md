# Comparing `tmp/dcg_service-0.0.9.tar.gz` & `tmp/dcg_service-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcg_service-0.0.9.tar", last modified: Tue Jul 18 13:00:52 2023, max compression
+gzip compressed data, was "dcg_service-1.0.0.tar", last modified: Sat Jul 29 08:43:55 2023, max compression
```

## Comparing `dcg_service-0.0.9.tar` & `dcg_service-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-18 13:00:52.512735 dcg_service-0.0.9/
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1073 2023-07-12 05:37:10.000000 dcg_service-0.0.9/LICENCE
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6923 2023-07-18 13:00:52.500735 dcg_service-0.0.9/PKG-INFO
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6376 2023-07-12 07:13:10.000000 dcg_service-0.0.9/README.md
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      629 2023-07-18 12:55:13.000000 dcg_service-0.0.9/pyproject.toml
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      103 2023-07-17 06:04:33.000000 dcg_service-0.0.9/requirement.txt
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)       38 2023-07-18 13:00:52.512735 dcg_service-0.0.9/setup.cfg
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-18 13:00:52.480736 dcg_service-0.0.9/src/
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-18 13:00:52.484736 dcg_service-0.0.9/src/dcg_service/
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-12 05:23:41.000000 dcg_service-0.0.9/src/dcg_service/__init__.py
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-18 13:00:52.500735 dcg_service-0.0.9/src/dcg_service/core/
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      298 2023-07-10 10:49:06.000000 dcg_service-0.0.9/src/dcg_service/core/__init__.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2683 2023-07-18 12:26:17.000000 dcg_service-0.0.9/src/dcg_service/core/authentication.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      833 2023-07-17 13:54:47.000000 dcg_service-0.0.9/src/dcg_service/core/encryption.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     7591 2023-07-17 13:56:57.000000 dcg_service-0.0.9/src/dcg_service/core/events.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2889 2023-07-13 06:38:05.000000 dcg_service-0.0.9/src/dcg_service/core/exceptions.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2319 2023-07-10 09:24:25.000000 dcg_service-0.0.9/src/dcg_service/core/filters.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      618 2023-07-10 10:39:56.000000 dcg_service-0.0.9/src/dcg_service/core/logger.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2691 2023-07-18 12:54:48.000000 dcg_service-0.0.9/src/dcg_service/core/permissions.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     3038 2023-07-18 12:25:40.000000 dcg_service-0.0.9/src/dcg_service/core/request_client.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1341 2023-07-13 06:38:22.000000 dcg_service-0.0.9/src/dcg_service/core/response.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)    16189 2023-07-12 05:41:48.000000 dcg_service-0.0.9/src/dcg_service/core/services.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1077 2023-07-17 14:04:57.000000 dcg_service-0.0.9/src/dcg_service/core/utils.py
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-18 13:00:52.488736 dcg_service-0.0.9/src/dcg_service.egg-info/
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6923 2023-07-18 13:00:52.000000 dcg_service-0.0.9/src/dcg_service.egg-info/PKG-INFO
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      677 2023-07-18 13:00:52.000000 dcg_service-0.0.9/src/dcg_service.egg-info/SOURCES.txt
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)        1 2023-07-18 13:00:52.000000 dcg_service-0.0.9/src/dcg_service.egg-info/dependency_links.txt
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      104 2023-07-18 13:00:52.000000 dcg_service-0.0.9/src/dcg_service.egg-info/requires.txt
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)       12 2023-07-18 13:00:52.000000 dcg_service-0.0.9/src/dcg_service.egg-info/top_level.txt
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-29 08:43:55.249016 dcg_service-1.0.0/
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1073 2023-07-12 05:37:10.000000 dcg_service-1.0.0/LICENCE
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6879 2023-07-29 08:43:55.249016 dcg_service-1.0.0/PKG-INFO
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6376 2023-07-12 07:13:10.000000 dcg_service-1.0.0/README.md
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      585 2023-07-29 04:19:47.000000 dcg_service-1.0.0/pyproject.toml
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      116 2023-07-29 04:20:53.000000 dcg_service-1.0.0/requirement.txt
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)       38 2023-07-29 08:43:55.249016 dcg_service-1.0.0/setup.cfg
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-29 08:43:55.241016 dcg_service-1.0.0/src/
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-29 08:43:55.245016 dcg_service-1.0.0/src/dcg_service/
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-12 05:23:41.000000 dcg_service-1.0.0/src/dcg_service/__init__.py
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-29 08:43:55.249016 dcg_service-1.0.0/src/dcg_service/core/
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      298 2023-07-10 10:49:06.000000 dcg_service-1.0.0/src/dcg_service/core/__init__.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2683 2023-07-18 12:26:17.000000 dcg_service-1.0.0/src/dcg_service/core/authentication.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2378 2023-07-29 05:43:24.000000 dcg_service-1.0.0/src/dcg_service/core/encryption.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     8115 2023-07-29 04:46:39.000000 dcg_service-1.0.0/src/dcg_service/core/events.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     4988 2023-07-29 05:42:10.000000 dcg_service-1.0.0/src/dcg_service/core/exceptions.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2319 2023-07-10 09:24:25.000000 dcg_service-1.0.0/src/dcg_service/core/filters.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      618 2023-07-10 10:39:56.000000 dcg_service-1.0.0/src/dcg_service/core/logger.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2926 2023-07-19 06:15:57.000000 dcg_service-1.0.0/src/dcg_service/core/permissions.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     3038 2023-07-18 12:25:40.000000 dcg_service-1.0.0/src/dcg_service/core/request_client.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1341 2023-07-13 06:38:22.000000 dcg_service-1.0.0/src/dcg_service/core/response.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)    16746 2023-07-29 08:31:31.000000 dcg_service-1.0.0/src/dcg_service/core/services.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     7789 2023-07-29 05:38:38.000000 dcg_service-1.0.0/src/dcg_service/core/utils.py
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-29 08:43:55.245016 dcg_service-1.0.0/src/dcg_service.egg-info/
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6879 2023-07-29 08:43:55.000000 dcg_service-1.0.0/src/dcg_service.egg-info/PKG-INFO
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      677 2023-07-29 08:43:55.000000 dcg_service-1.0.0/src/dcg_service.egg-info/SOURCES.txt
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)        1 2023-07-29 08:43:55.000000 dcg_service-1.0.0/src/dcg_service.egg-info/dependency_links.txt
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      117 2023-07-29 08:43:55.000000 dcg_service-1.0.0/src/dcg_service.egg-info/requires.txt
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)       12 2023-07-29 08:43:55.000000 dcg_service-1.0.0/src/dcg_service.egg-info/top_level.txt
```

### Comparing `dcg_service-0.0.9/LICENCE` & `dcg_service-1.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.9/PKG-INFO` & `dcg_service-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dcg_service
-Version: 0.0.9
-Summary: Package for DCG DOT Compliance Group, used for flask based projects.
+Version: 1.0.0
+Summary: DCG DOT Compliance Group
 Author-email: Aman Kumar <amankumar@zapbuild.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `dcg_service-0.0.9/README.md` & `dcg_service-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.9/pyproject.toml` & `dcg_service-1.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "dcg_service"
-version = "0.0.9"
+version = "1.0.0"
 authors = [
   { name="Aman Kumar", email="amankumar@zapbuild.com" },
 ]
-description = "Package for DCG DOT Compliance Group, used for flask based projects."
+description = "DCG DOT Compliance Group"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `dcg_service-0.0.9/src/dcg_service/core/authentication.py` & `dcg_service-1.0.0/src/dcg_service/core/authentication.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.9/src/dcg_service/core/events.py` & `dcg_service-1.0.0/src/dcg_service/core/events.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,25 @@
 import inspect as module_inspect
 from datetime import datetime, date
 
 from elasticsearch_dsl import Search
 from flask import request
 from flask_sqlalchemy.model import Model
 from sqlalchemy import event as alchemy_event, inspect
-from . import EsClient, exceptions, ACTIVITY_INDEX, EXCLUDE_MODEL_EVENTS, EVENTS, APP_MODELS
+from . import EsClient, exceptions, APP_MODELS
+
+DEFAULT_ACTIVITY_INDEX = 'logs'
+DEFAULT_EVENTS = ['after_insert', 'before_update']
+
+try:
+    from . import ACTIVITY_INDEX, EXCLUDE_MODEL_EVENTS, EVENTS
+except:
+    ACTIVITY_INDEX = DEFAULT_ACTIVITY_INDEX
+    EXCLUDE_MODEL_EVENTS = []
+    EVENTS = DEFAULT_EVENTS
 
 
 class BaseEvents(object):
     """
     Base events class.
     """
     events = []
@@ -73,45 +83,52 @@
         """
         Push user activity logs to Elasticsearch.
         """
 
         if old_data is None:
             old_data = {}
 
+        # Make sure `request` is available and headers contain "Request-Id".
         request_id = request.headers.get("Request-Id")
+
         activity_data = {
             "Table": table_name,
             "OldData": old_data,
             "NewData": new_data,
             "Activity": activity
         }
-        search = Search(using=EsClient, index=ACTIVITY_INDEX).query(
-            "match", RequestID=request_id)
+
+        # Assuming `EsClient` is properly imported and initialized.
+
+        search = Search(using=EsClient, index=ACTIVITY_INDEX).query("match", RequestID=request_id)
+
         try:
             response = search.execute()
             hits = response.hits
+
             if hits:
                 # Retrieve the first matching document and update the activity array
                 hit = hits[0]
                 index_id = hit.meta.id
-                existing_activities = json.loads(getattr(hit, 'Activities', "[]"))
+                existing_activities = json.loads(
+                    getattr(hit, 'Activities', "[]"))  # Deserialize existing_activities if present.
                 existing_activities.append(activity_data)
                 update_body = {
                     "doc": {
-                        "Activities": json.dumps(existing_activities)
+                        "Activities": json.dumps(existing_activities)  # Serialize existing_activities before updating.
                     }
                 }
                 EsClient.update(index=ACTIVITY_INDEX, id=index_id, body=update_body)
                 EsClient.indices.refresh(index=ACTIVITY_INDEX)
             else:
                 log_body = {
                     "RequestID": request_id,
                     "Activities": json.dumps([activity_data])
+                    # Serialize activity_data before inserting a new document.
                 }
-                # Create a new document with the request ID and the activity array
                 EsClient.index(index=ACTIVITY_INDEX, body=log_body)
                 EsClient.indices.refresh(index=ACTIVITY_INDEX)
         except Exception as error:
             print("Error saving activity: %s" % str(error))
 
     @classmethod
     def get_history(cls, mapped_obj, target, column):
@@ -152,14 +169,16 @@
                 return value.value if value else None
             elif isinstance(value, (datetime, date)):
                 return value.isoformat()
             elif isinstance(value, Decimal):
                 return float(value)
             else:
                 return None
+        except Exception:
+            return str(value)
 
     def get_model_data(self, target, history=False):
         """
         Get model/columns data from model instance.
         """
         old_data = {}
         new_data = {}
```

### Comparing `dcg_service-0.0.9/src/dcg_service/core/filters.py` & `dcg_service-1.0.0/src/dcg_service/core/filters.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.9/src/dcg_service/core/logger.py` & `dcg_service-1.0.0/src/dcg_service/core/logger.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.9/src/dcg_service/core/permissions.py` & `dcg_service-1.0.0/src/dcg_service/core/permissions.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,17 +72,22 @@
     """
 
     def internal_request_deco(func):
         if allow_internal_request:
             @wraps(func)
             def wrapper(*args, **kwargs):
                 request_internal_key = get_internal_key_header(request.headers)
-                if request_internal_key == os.environ['INTERNAL_SERVICE_KEY']:
+                if request_internal_key == INTERNAL_SERVICE_KEY:
                     setattr(request, 'is_internal_request', True)
                 else:
-                    return is_authenticated(func)
+                    token = get_authorization_header(request.headers)
+                    try:
+                        user = authenticate(token)
+                        setattr(request, 'user', user)
+                    except AuthException as error:
+                        return error.as_json()
                 return func(*args, **kwargs)
             return wrapper
         else:
             return is_authenticated(func)
 
     return internal_request_deco
```

### Comparing `dcg_service-0.0.9/src/dcg_service/core/request_client.py` & `dcg_service-1.0.0/src/dcg_service/core/request_client.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.9/src/dcg_service/core/response.py` & `dcg_service-1.0.0/src/dcg_service/core/response.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.9/src/dcg_service/core/services.py` & `dcg_service-1.0.0/src/dcg_service/core/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,18 @@
         if len(response.hits) < 1:
             if raise_exception:
                 raise APIException("Service not found", 404)
         else:
             self._service_details = response.hits[0]
             self.is_valid_service = True
 
+    @staticmethod
+    def percentage(part, whole):
+        return (float(part) * float(whole)) / 100
+
     @property
     def total_commission(self):
         return self._total_commission
 
     @property
     def service_details(self):
         if not self._service_details:
@@ -168,18 +172,14 @@
                     unit = obj.unit_to - (obj.unit_from - 1)
 
             obj.total_price = unit * obj.price
             self._total_commission += self.get_tier_commission(obj.total_price, obj)
             self._total_price += obj.total_price
         return self._total_price, self._total_commission
 
-    @staticmethod
-    def percentage(part, whole):
-        return (float(part) * float(whole)) / 100
-
     def get_flat_commission(self, service_price):
         """
         If Service is flat calculate commission from ServiceCommissions.
         If The commission_type is Flat return commission as figure value.
         If The commission_type is PERCENTAGE Calculate commission
         by ((service_total_price*commission.figure_value)/100).
         """
@@ -292,36 +292,46 @@
         """
         total_price = self.total_price
         coupons_to_apply = list()
 
         # service_list to validate dependent service condition
         service_list = kwargs.get('service_list') or list()
         coupon_code_list = kwargs.get('coupon_code_list') or list()
+        availed_coupons = kwargs.get('availed_coupons') or list()
         service = self.service_details
         service_coupons = service.coupons or list()
 
         if coupon_code:
             coupon_code_list.append(coupon_code)
 
         for c_code in coupon_code_list:
             coupons_to_apply += list(
                 filter(
-                    lambda coup: coup.code == c_code, service_coupons
+                    lambda coup: coup.code == c_code and coup.code not in availed_coupons, service_coupons
                 )
             )
 
         for coupon in service_coupons:
             if coupon.is_auto_apply:
                 coupons_to_apply.append(coupon)
 
-        coupons_to_apply = list(
-            filter(
-                lambda coupon_obj: coupon_obj.min_amount_for_coupon < total_price, coupons_to_apply
-            )
-        )
+        filtered_coupon_list = []
+
+        for coupon in coupons_to_apply:
+            if coupon.coupon_type == 'PERCENTAGE':
+                coupon_value = self.percentage(total_price, coupon.coupon_value)
+                if coupon.min_amount_for_coupon < coupon_value:
+                    coupon.coupon_value = min([coupon_value, coupon.max_discount])
+                    filtered_coupon_list.append(coupon)
+            else:
+                coupon_value = coupon.coupon_value
+                if total_price > coupon_value:
+                    filtered_coupon_list.append(coupon)
+
+        coupons_to_apply = filtered_coupon_list
 
         if coupons_to_apply:
             coupon_to_be_apply = self._get_coupon_with_max_discount(coupons_to_apply)
             if coupon_to_be_apply.dependent_services:
                 is_valid_coupon = any(
                     dependent.service_id in service_list for dependent in coupon_to_be_apply.dependent_services
                 )
@@ -337,15 +347,15 @@
                 self._coupon_code = coupon_to_be_apply.code
 
         return self._total_discount, self._coupon_code
 
     @classmethod
     def _get_coupon_with_max_discount(cls, coupon_list):
         if coupon_list:
-            return max(coupon_list, key=lambda k: k.max_discount)
+            return max(coupon_list, key=lambda k: k.coupon_value)
 
     @classmethod
     def _remove_coupon_from_list(cls, coupon_code, coupon_list):
         coupons_to_apply = []
 
         for coupon in coupon_list:
             if coupon.code != coupon_code:
```

### Comparing `dcg_service-0.0.9/src/dcg_service.egg-info/PKG-INFO` & `dcg_service-1.0.0/src/dcg_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dcg-service
-Version: 0.0.9
-Summary: Package for DCG DOT Compliance Group, used for flask based projects.
+Version: 1.0.0
+Summary: DCG DOT Compliance Group
 Author-email: Aman Kumar <amankumar@zapbuild.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `dcg_service-0.0.9/src/dcg_service.egg-info/SOURCES.txt` & `dcg_service-1.0.0/src/dcg_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

