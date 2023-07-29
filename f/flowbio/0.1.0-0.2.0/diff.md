# Comparing `tmp/flowbio-0.1.0-py3-none-any.whl.zip` & `tmp/flowbio-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,13 @@
-Zip file size: 2015 bytes, number of entries: 6
--rw-r--r--  2.0 unx       76 b- defN 22-Sep-12 10:26 flowbio/__init__.py
--rw-r--r--  2.0 unx      837 b- defN 22-Sep-13 15:51 flowbio/client.py
--rw-r--r--  2.0 unx      846 b- defN 22-Sep-17 14:19 flowbio-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Sep-17 14:19 flowbio-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 22-Sep-17 14:19 flowbio-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      443 b- defN 22-Sep-17 14:19 flowbio-0.1.0.dist-info/RECORD
-6 files, 2302 bytes uncompressed, 1209 bytes compressed:  47.5%
+Zip file size: 7251 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       76 b- defN 23-Jul-26 00:14 flowbio/__init__.py
+-rw-r--r--  2.0 unx     2091 b- defN 23-Jul-26 01:33 flowbio/client.py
+-rw-r--r--  2.0 unx     3122 b- defN 23-Jul-25 23:50 flowbio/mutations.py
+-rw-r--r--  2.0 unx     1422 b- defN 23-Jul-25 23:57 flowbio/queries.py
+-rw-r--r--  2.0 unx      517 b- defN 23-Jul-25 23:57 flowbio/samples.py
+-rw-r--r--  2.0 unx     8942 b- defN 23-Jul-26 00:30 flowbio/upload.py
+-rw-r--r--  2.0 unx     1071 b- defN 23-Jul-29 21:17 flowbio-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1737 b- defN 23-Jul-29 21:17 flowbio-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-29 21:17 flowbio-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-29 21:17 flowbio-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jul-29 21:17 flowbio-0.2.0.dist-info/RECORD
+11 files, 19911 bytes uncompressed, 5857 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -1,19 +1,34 @@
 Filename: flowbio/__init__.py
 Comment: 
 
 Filename: flowbio/client.py
 Comment: 
 
-Filename: flowbio-0.1.0.dist-info/METADATA
+Filename: flowbio/mutations.py
 Comment: 
 
-Filename: flowbio-0.1.0.dist-info/WHEEL
+Filename: flowbio/queries.py
 Comment: 
 
-Filename: flowbio-0.1.0.dist-info/top_level.txt
+Filename: flowbio/samples.py
 Comment: 
 
-Filename: flowbio-0.1.0.dist-info/RECORD
+Filename: flowbio/upload.py
+Comment: 
+
+Filename: flowbio-0.2.0.dist-info/LICENSE
+Comment: 
+
+Filename: flowbio-0.2.0.dist-info/METADATA
+Comment: 
+
+Filename: flowbio-0.2.0.dist-info/WHEEL
+Comment: 
+
+Filename: flowbio-0.2.0.dist-info/top_level.txt
+Comment: 
+
+Filename: flowbio-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flowbio/__init__.py

```diff
@@ -1,4 +1,4 @@
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 __author__ = "Sam Ireland"
 
 from .client import Client
```

## flowbio/client.py

```diff
@@ -1,25 +1,66 @@
 import kirjava
+import time
+from .upload import UploadClient
+from .samples import SamplesClient
 
-class Client(kirjava.Client):
+class GraphQlError(Exception):
+    pass
+
+
+
+class Client(kirjava.Client, UploadClient, SamplesClient):
+
+    def __init__(self, url="https://api.flow.bio/graphql"):        
+        super().__init__(url)
+        self.last_token_refresh = None
+
+
+    def execute(self, *args, check_token=True, **kwargs):
+        __doc__ = kirjava.Client.execute.__doc__
+
+        if self.last_token_refresh and check_token:
+            age = time.time() - self.last_token_refresh
+            if age > 60 * 20: self.refresh_token()
+        resp = super().execute(*args, **kwargs)
+        if "errors" in resp:
+            raise GraphQlError(resp["errors"])
+        return resp
     
+
     def login(self, username, password):
-        """Acquires the relevant access token for the client."""
+        """Acquires the relevant access token for the client.
+        
+        :param str username: The username of the user.
+        :param str password: The password of the user."""
         
         response = self.execute("""mutation login(
             $username: String! $password: String!
         ) { login(username: $username password: $password) {
             accessToken
         } }""", variables={"username": username, "password": password})
+        self.last_token_refresh = time.time()
         token = response["data"]["login"]["accessToken"]
         self.headers["Authorization"] = token
     
 
+    def refresh_token(self):
+        """Refreshes the access token."""
+        
+        response = self.execute("{ accessToken }", check_token=False)
+        self.last_token_refresh = time.time()
+        token = response["data"]["accessToken"]
+        self.headers["Authorization"] = token
+    
+
     def user(self, username):
-        """Returns a user object."""
+        """Returns a user object.
+        
+        :param str username: The username of the user.
+        :rtype: ``dict``"""
 
         response = self.execute("""query user(
             $username: String!
         ) { user(username: $username) {
             id username name
         } }""", variables={"username": username})
         return response["data"]["user"]
```

