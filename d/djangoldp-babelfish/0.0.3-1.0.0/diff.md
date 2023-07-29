# Comparing `tmp/djangoldp_babelfish-0.0.3.tar.gz` & `tmp/djangoldp_babelfish-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_babelfish-0.0.3.tar", last modified: Thu Jul 20 17:44:38 2023, max compression
+gzip compressed data, was "dist/djangoldp_babelfish-1.0.0.tar", last modified: Sat Jul 29 09:01:57 2023, max compression
```

## Comparing `djangoldp_babelfish-0.0.3.tar` & `djangoldp_babelfish-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/
--rw-rw-rw-   0 root         (0) root         (0)     1979 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/
--rw-rw-rw-   0 root         (0) root         (0)     2092 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/views.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/models.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-20 17:44:35.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1938 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py
--rw-r--r--   0 root         (0) root         (0)      363 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish.egg-info/
--rw-r--r--   0 root         (0) root         (0)      363 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1979 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/
+-rw-rw-rw-   0 root         (0) root         (0)     3132 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      222 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-29 09:01:54.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py
+-rw-r--r--   0 root         (0) root         (0)      363 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      363 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      671 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish.egg-info/requires.txt
```

### Comparing `djangoldp_babelfish-0.0.3/README.md` & `djangoldp_babelfish-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-0.0.3/setup.cfg` & `djangoldp_babelfish-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-0.0.3/djangoldp_babelfish/views.py` & `djangoldp_babelfish-1.0.0/djangoldp_babelfish/views.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,86 @@
 from django.contrib.auth.decorators import login_required
 from django.http import JsonResponse
+from rest_framework.response import Response
+from django.conf import settings
+from djangoldp.views import LDPAPIView, NoCSRFAuthentication
 import requests
 
 
-@login_required
-def call_babelfish(request):
-    # Retrieve the user-specific access token
-    token_url = settings.BABELFISH_BASE_URL + '/oauth/token'
-    data = {
-        'client_id': request.user.babelfishprofile.client_id,
-        'client_secret': request.user.babelfishprofile.client_secret,
-        'grant_type': 'client_credentials',
-        'scope': 'write'
-    }
-    response = requests.post(token_url, data=data)
-    access_token = response.json().get('access_token')
-
-    # Call the service registration endpoint with the proper info
-    service_registration_url = settings.BABELFISH_BASE_URL + '/service/'  # Replace with the actual registration endpoint URL
-    headers = {'Authorization': f'Bearer {access_token}'}
-    json = {
-        "interface": {
-            "info": { "title": request.data.get('service_title') },
-            "servers": [{"url": request.data.get('service_url')}],
-            "party": request.data.get('service_party'),
-            "paths": {
-                "/api/validate": {
-                    "post": {
-                        "requestBody": {
-                            "content": {
-                                "application/json": {
-                                    "schema": {} 
+class BabelfishServiceCreate(LDPAPIView):
+    authentication_classes = (NoCSRFAuthentication,)
+
+    def post(self, request):
+        # Retrieve the user-specific access token
+        token_url = settings.BABELFISH_BASE_URL + '/oauth/token'
+        data = {
+            'client_id': request.user.babelfish_profile.client_id,
+            'client_secret': request.user.babelfish_profile.client_secret,
+            'grant_type': 'client_credentials',
+            'scope': 'write'
+        }
+        response = requests.post(token_url, data=data)
+        access_token = response.json().get('access_token')
+
+        print(access_token)
+        print(access_token)
+        print(access_token)
+        print(request.user)
+        print(request)
+        print(request.POST)
+        # Call the service registration endpoint with the proper info
+        service_registration_url = settings.BABELFISH_BASE_URL + '/service/'  # Replace with the actual registration endpoint URL
+        headers = {
+            'Authorization': f'Bearer {access_token}'
+        }
+
+        print(request.data.get('title'))
+
+        json = {
+            "interface": {
+                "info": { "title": request.data.get('title') },
+                "servers": [{"url": request.data.get('url')}],
+                "party": request.data.get('party'),
+                "paths": {
+                    "/api/validate": {
+                        "post": {
+                            "requestBody": {
+                                "content": {
+                                    "application/json": {
+                                        "schema": {} 
+                                    }
                                 }
                             }
                         }
                     }
                 }
+            },
+            "data": {
+                "description": request.data.get('description')
+            },
+            "governance": {
+                "dpv:hasProcessing": ["dpv:Use"],
+                "dpv:hasPurpose": "dpv:Purpose",
+                "dpv:hasExpiryTime": "6 months"
             }
-        },
-        "data": {
-            "description": request.data.get('service_description')
-        },
-        "governance": {
-            "dpv:hasProcessing": ["dpv:Use"],
-            "dpv:hasPurpose": "dpv:Purpose",
-            "dpv:hasExpiryTime": "6 months"
         }
-    }
-
-    response = requests.post(registration_url, headers=headers, json=json)
-    # Refresh the list of services to display the new one
 
-    if response.status_code != 201:
-        return JsonResponse({'message': 'Service registration failed'}, status=500)
+        try:
+            response = requests.post(service_registration_url, headers=headers, json=json)
+            response = response.json()
+        except Exception as e:
+            print(e)
+            print(e)
+            print(e)
+            print(e)
+            print(e)
+            print("HEHEHEHEHEEHHEHEEH")
+            return Response({'message': 'Service registration failed'}, status=500)
+
+        print(json)
+        response = requests.post(registration_url, headers=headers, json=json)
+        # Refresh the list of services to display the new one
+        print(response)
+        if response.status_code != 201:
+            return Response({'message': 'Service registration failed'}, status=500)
 
-    return JsonResponse({'message': 'Service properly registered'})
+        return Response({'message': 'Service properly registered'})
```

### Comparing `djangoldp_babelfish-0.0.3/djangoldp_babelfish/models.py` & `djangoldp_babelfish-1.0.0/djangoldp_babelfish/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-0.0.3/djangoldp_babelfish/migrations/0001_initial.py` & `djangoldp_babelfish-1.0.0/djangoldp_babelfish/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-0.0.3/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py` & `djangoldp_babelfish-1.0.0/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-0.0.3/djangoldp_babelfish.egg-info/SOURCES.txt` & `djangoldp_babelfish-1.0.0/djangoldp_babelfish.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.cfg
 setup.py
 djangoldp_babelfish/__init__.py
 djangoldp_babelfish/admin.py
 djangoldp_babelfish/apps.py
+djangoldp_babelfish/djangoldp_urls.py
 djangoldp_babelfish/models.py
 djangoldp_babelfish/views.py
 djangoldp_babelfish.egg-info/PKG-INFO
 djangoldp_babelfish.egg-info/SOURCES.txt
 djangoldp_babelfish.egg-info/dependency_links.txt
 djangoldp_babelfish.egg-info/requires.txt
 djangoldp_babelfish.egg-info/top_level.txt
```

