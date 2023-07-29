# Comparing `tmp/djangoldp_babelfish-1.0.2.tar.gz` & `tmp/djangoldp_babelfish-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoldp_babelfish-1.0.2.tar", last modified: Sat Jul 29 09:46:57 2023, max compression
+gzip compressed data, was "djangoldp_babelfish-1.0.3.tar", last modified: Sat Jul 29 11:18:20 2023, max compression
```

## Comparing `djangoldp_babelfish-1.0.2.tar` & `djangoldp_babelfish-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:46:57.126579 djangoldp_babelfish-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      335 2023-07-29 09:46:57.126579 djangoldp_babelfish-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1979 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:46:57.126579 djangoldp_babelfish-1.0.2/djangoldp_babelfish/
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-29 09:46:54.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      222 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/djangoldp_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:46:57.126579 djangoldp_babelfish-1.0.2/djangoldp_babelfish/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:46:57.126579 djangoldp_babelfish-1.0.2/djangoldp_babelfish/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/management/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:46:57.126579 djangoldp_babelfish-1.0.2/djangoldp_babelfish/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1938 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3132 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:46:57.126579 djangoldp_babelfish-1.0.2/djangoldp_babelfish.egg-info/
--rw-r--r--   0 root         (0) root         (0)      335 2023-07-29 09:46:57.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      671 2023-07-29 09:46:57.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 09:46:57.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-29 09:46:57.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-29 09:46:57.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      662 2023-07-29 09:46:57.126579 djangoldp_babelfish-1.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 11:18:20.026262 djangoldp_babelfish-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      335 2023-07-29 11:18:20.026262 djangoldp_babelfish-1.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1979 2023-07-29 11:17:59.000000 djangoldp_babelfish-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 11:18:20.022262 djangoldp_babelfish-1.0.3/djangoldp_babelfish/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-29 11:18:17.000000 djangoldp_babelfish-1.0.3/djangoldp_babelfish/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-07-29 11:17:59.000000 djangoldp_babelfish-1.0.3/djangoldp_babelfish/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-29 11:17:59.000000 djangoldp_babelfish-1.0.3/djangoldp_babelfish/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      222 2023-07-29 11:17:59.000000 djangoldp_babelfish-1.0.3/djangoldp_babelfish/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 11:18:20.026262 djangoldp_babelfish-1.0.3/djangoldp_babelfish/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 11:18:00.000000 djangoldp_babelfish-1.0.3/djangoldp_babelfish/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 11:18:20.026262 djangoldp_babelfish-1.0.3/djangoldp_babelfish/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 11:18:00.000000 djangoldp_babelfish-1.0.3/djangoldp_babelfish/management/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 11:18:20.026262 djangoldp_babelfish-1.0.3/djangoldp_babelfish/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2023-07-29 11:17:59.000000 djangoldp_babelfish-1.0.3/djangoldp_babelfish/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-29 11:17:59.000000 djangoldp_babelfish-1.0.3/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 11:18:00.000000 djangoldp_babelfish-1.0.3/djangoldp_babelfish/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2961 2023-07-29 11:17:59.000000 djangoldp_babelfish-1.0.3/djangoldp_babelfish/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3236 2023-07-29 11:17:59.000000 djangoldp_babelfish-1.0.3/djangoldp_babelfish/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 11:18:20.026262 djangoldp_babelfish-1.0.3/djangoldp_babelfish.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      335 2023-07-29 11:18:19.000000 djangoldp_babelfish-1.0.3/djangoldp_babelfish.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      671 2023-07-29 11:18:19.000000 djangoldp_babelfish-1.0.3/djangoldp_babelfish.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 11:18:19.000000 djangoldp_babelfish-1.0.3/djangoldp_babelfish.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-29 11:18:19.000000 djangoldp_babelfish-1.0.3/djangoldp_babelfish.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-29 11:18:19.000000 djangoldp_babelfish-1.0.3/djangoldp_babelfish.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-07-29 11:18:20.026262 djangoldp_babelfish-1.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-29 11:17:59.000000 djangoldp_babelfish-1.0.3/setup.py
```

### Comparing `djangoldp_babelfish-1.0.2/README.md` & `djangoldp_babelfish-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.2/djangoldp_babelfish/migrations/0001_initial.py` & `djangoldp_babelfish-1.0.3/djangoldp_babelfish/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.2/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py` & `djangoldp_babelfish-1.0.3/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.2/djangoldp_babelfish/models.py` & `djangoldp_babelfish-1.0.3/djangoldp_babelfish/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,34 +22,34 @@
         auto_author = "user"
         serializer_fields = ['@id']
 
 @receiver(post_save, sender=settings.AUTH_USER_MODEL)
 def register_user_with_sib(sender, instance, created, **kwargs):
     if created or not hasattr(instance, 'babelfish_profile'):
         # Retrieve the access token using server-side settings
-        token_url = settings.BABELFISH_BASE_URL + '/oauth/token'  # Replace with the actual token API endpoint URL
+        token_url = getattr(settings, 'BABELFISH_BASE_URL', "https://babelfish.data-container.net") + '/oauth/token'  # Replace with the actual token API endpoint URL
         data = {
-            'client_id': settings.BABELFISH_CLIENT_ID,
-            'client_secret': settings.BABELFISH_CLIENT_SECRET,
+            'client_id': getattr(settings, 'BABELFISH_CLIENT_ID', ''),
+            'client_secret': getattr(settings, 'BABELFISH_CLIENT_SECRET', '') ,
             'grant_type': 'client_credentials',
             'scope': 'write'
         }
         response = requests.post(token_url, data=data)
         access_token = response.json().get('access_token')
 
         # Build a request to create the user in BabelFish and retrieve credentials
-        create_user_url = settings.BABELFISH_BASE_URL + '/user/'  # Replace with the actual create user endpoint URL
+        create_user_url = getattr(settings, "BABELFISH_BASE_URL", "https://babelfish.data-container.net") + '/user/'  # Replace with the actual create user endpoint URL
         headers = {
             'Authorization': 'Bearer ' + access_token,
             'Content-Type': 'application/json'
         }
         data = {
             'name': instance.name(),
             'email': instance.email,
-            'organization-id': settings.BABELFISH_ORGANISATION_ID,
+            'organization-id': getattr(settings, 'BABELFISH_ORGANISATION_ID', '811'),
         }
 
         try:
             response = requests.post(create_user_url, headers=headers, data=json.dumps(data))
             babelfish_profile_info = response.json()
         except Exception as e:
             print(e)
```

### Comparing `djangoldp_babelfish-1.0.2/djangoldp_babelfish/views.py` & `djangoldp_babelfish-1.0.3/djangoldp_babelfish/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class BabelfishServiceCreate(LDPAPIView):
     authentication_classes = (NoCSRFAuthentication,)
 
     def post(self, request):
         # Retrieve the user-specific access token
-        token_url = settings.BABELFISH_BASE_URL + '/oauth/token'
+        token_url = getattr(settings, 'BABELFISH_BASE_URL', "https://babelfish.data-container.net") + '/oauth/token'
         data = {
             'client_id': request.user.babelfish_profile.client_id,
             'client_secret': request.user.babelfish_profile.client_secret,
             'grant_type': 'client_credentials',
             'scope': 'write'
         }
         response = requests.post(token_url, data=data)
@@ -24,15 +24,15 @@
         print(access_token)
         print(access_token)
         print(access_token)
         print(request.user)
         print(request)
         print(request.POST)
         # Call the service registration endpoint with the proper info
-        service_registration_url = settings.BABELFISH_BASE_URL + '/service/'  # Replace with the actual registration endpoint URL
+        service_registration_url = getattr(settings, 'BABELFISH_BASE_URL', "https://babelfish.data-container.net") + '/service/'  # Replace with the actual registration endpoint URL
         headers = {
             'Authorization': f'Bearer {access_token}'
         }
 
         print(request.data.get('title'))
 
         json = {
```

### Comparing `djangoldp_babelfish-1.0.2/djangoldp_babelfish.egg-info/SOURCES.txt` & `djangoldp_babelfish-1.0.3/djangoldp_babelfish.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.2/setup.cfg` & `djangoldp_babelfish-1.0.3/setup.cfg`

 * *Files identical despite different names*

