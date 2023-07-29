# Comparing `tmp/zerocap_api_test-0.1.5.tar.gz` & `tmp/zerocap_api_test-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerocap_api_test-0.1.5.tar", last modified: Fri Jul 28 05:27:19 2023, max compression
+gzip compressed data, was "dist/zerocap_api_test-0.1.6.tar", last modified: Sat Jul 29 07:47:56 2023, max compression
```

## Comparing `zerocap_api_test-0.1.5.tar` & `zerocap_api_test-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-28 05:27:19.606649 zerocap_api_test-0.1.5/
--rw-r--r--   0 gao        (501) staff       (20)    11323 2023-07-26 06:32:00.000000 zerocap_api_test-0.1.5/LICENSE.txt
--rw-r--r--   0 gao        (501) staff       (20)     1620 2023-07-28 05:27:19.606205 zerocap_api_test-0.1.5/PKG-INFO
--rw-r--r--   0 gao        (501) staff       (20)     1240 2023-07-28 05:26:50.000000 zerocap_api_test-0.1.5/README.rst
--rw-r--r--   0 gao        (501) staff       (20)       38 2023-07-28 05:27:19.606772 zerocap_api_test-0.1.5/setup.cfg
--rw-r--r--   0 gao        (501) staff       (20)      792 2023-07-28 05:24:45.000000 zerocap_api_test-0.1.5/setup.py
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-28 05:27:19.604151 zerocap_api_test-0.1.5/zerocap_api_test/
--rw-r--r--   0 gao        (501) staff       (20)      121 2023-07-26 06:32:00.000000 zerocap_api_test-0.1.5/zerocap_api_test/__init__.py
--rw-r--r--   0 gao        (501) staff       (20)     7467 2023-07-28 05:18:21.000000 zerocap_api_test-0.1.5/zerocap_api_test/main.py
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-28 05:27:19.605719 zerocap_api_test-0.1.5/zerocap_api_test.egg-info/
--rw-r--r--   0 gao        (501) staff       (20)     1620 2023-07-28 05:27:19.000000 zerocap_api_test-0.1.5/zerocap_api_test.egg-info/PKG-INFO
--rw-r--r--   0 gao        (501) staff       (20)      284 2023-07-28 05:27:19.000000 zerocap_api_test-0.1.5/zerocap_api_test.egg-info/SOURCES.txt
--rw-r--r--   0 gao        (501) staff       (20)        1 2023-07-28 05:27:19.000000 zerocap_api_test-0.1.5/zerocap_api_test.egg-info/dependency_links.txt
--rw-r--r--   0 gao        (501) staff       (20)       19 2023-07-28 05:27:19.000000 zerocap_api_test-0.1.5/zerocap_api_test.egg-info/requires.txt
--rw-r--r--   0 gao        (501) staff       (20)       17 2023-07-28 05:27:19.000000 zerocap_api_test-0.1.5/zerocap_api_test.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 07:47:56.000000 zerocap_api_test-0.1.6/
+-rw-r--r--   0 mac        (501) staff       (20)    11323 2023-07-24 01:35:05.000000 zerocap_api_test-0.1.6/LICENSE.txt
+-rw-r--r--   0 mac        (501) staff       (20)      662 2023-07-29 07:47:56.000000 zerocap_api_test-0.1.6/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-29 07:47:56.000000 zerocap_api_test-0.1.6/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      791 2023-07-29 07:44:43.000000 zerocap_api_test-0.1.6/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 07:47:56.000000 zerocap_api_test-0.1.6/zerocap_api_test/
+-rw-r--r--   0 mac        (501) staff       (20)      121 2023-07-26 05:40:03.000000 zerocap_api_test-0.1.6/zerocap_api_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     8054 2023-07-29 07:35:17.000000 zerocap_api_test-0.1.6/zerocap_api_test/main.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 07:47:56.000000 zerocap_api_test-0.1.6/zerocap_api_test.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      662 2023-07-29 07:47:56.000000 zerocap_api_test-0.1.6/zerocap_api_test.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      273 2023-07-29 07:47:56.000000 zerocap_api_test-0.1.6/zerocap_api_test.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-29 07:47:56.000000 zerocap_api_test-0.1.6/zerocap_api_test.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       19 2023-07-29 07:47:56.000000 zerocap_api_test-0.1.6/zerocap_api_test.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       17 2023-07-29 07:47:56.000000 zerocap_api_test-0.1.6/zerocap_api_test.egg-info/top_level.txt
```

### Comparing `zerocap_api_test-0.1.5/LICENSE.txt` & `zerocap_api_test-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zerocap_api_test-0.1.5/setup.py` & `zerocap_api_test-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from distutils.core import setup
 from setuptools import find_packages
 
-with open("README.rst", "r") as f:
+with open("README.MD", "r") as f:
   long_description = f.read()
 
 REQUIRED = [
     'requests',
     'websocket'
 ]
 
 setup(name='zerocap_api_test',  # 包名
-      version='0.1.5',  # 版本号
+      version='0.1.6',  # 版本号
       description='zerocap_api',
       long_description=long_description,
       author='jiayu.gao',
       author_email='jiayu.gao@eigen.capital',
       url='',
       install_requires=REQUIRED,
       license='BSD License',
```

### Comparing `zerocap_api_test-0.1.5/zerocap_api_test/main.py` & `zerocap_api_test-0.1.6/zerocap_api_test/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 import json
 import hashlib
 import requests
 from websocket import create_connection
 
 
 class ZerocapWebsocketClient:
-    def __init__(self, api_key, api_secret):
+    def __init__(self, api_key: str, api_secret: str, environ: str = 'development'):
         self.api_key = api_key
         self.api_secret = api_secret
         self.market_websocket = None
         self.order_websocket = None
-        self.base_url = "wss://dma-api.defi.wiki/ws"
-        self.http_url = "https://dma-api.defi.wiki/orders"
+        if environ == "development":
+            self.base_url = "wss://dma-api.defi.wiki/ws"
+            self.http_url = "https://dma-api.defi.wiki/orders"
+        else:
+            self.base_url = "*"
+            self.http_url = "*"
         self.signature = self.hashing()
         self.verify_identity()
         
     def verify_identity(self):
         headers = {'Content-Type': 'application/json'}
         data = {"api_key": self.api_key, "signature": self.signature}
         url = f"{self.http_url}/api_key_signature_valid"
@@ -25,28 +29,28 @@
             raise Exception("Authentication failed")
         
     def hashing(self):
         return hmac.new(
             self.api_secret.encode("utf-8"), self.api_key.encode("utf-8"), hashlib.sha256
         ).hexdigest()
 
-    def get_params(self, channel):
+    def get_params(self, channel: str):
         data_type = ""
         if channel == "orders":
             data_type = "order,trader"
         elif channel == "market":
             data_type = "price"
             
         return {
             "api_key": self.api_key,
             "signature": self.signature,
             "data_type": data_type,
         }
 
-    def close(self, channel=None):
+    def close(self, channel: str = None):
         try:
             if channel == "orders" and self.order_websocket:
                 self.order_websocket.close()
             elif channel == "market" and self.market_websocket:
                 self.market_websocket.close()
             else:
                 if self.order_websocket:
@@ -82,19 +86,22 @@
                 yield message
         except Exception as e:
             self.close(channel="market")
             raise Exception(e)
 
 
 class ZerocapRestClient:
-    def __init__(self, api_key, api_secret):
+    def __init__(self, api_key: str, api_secret: str, environ: str = 'development'):
         self.api_key = api_key
         self.api_secret = api_secret
         signature = self.encryption_api_key()
-        self.base_url = "https://dma-api.defi.wiki/orders"
+        if environ == 'development':
+            self.base_url = "https://dma-api.defi.wiki/orders"
+        else:
+            self.base_url = "*"
         url = f"{self.base_url}/api_key_signature_valid"
         headers = {
             'Content-Type': 'application/json',
         }
         data = {
             "api_key": self.api_key,
             "signature": signature,
@@ -115,19 +122,28 @@
             self.api_secret.encode("utf-8"), self.api_key.encode("utf-8"), hashlib.sha256
         ).hexdigest()
 
     def encryption_api_key(self):
         signature = self.hashing()
         return signature
 
-    def create_order(self, symbol: str, side: str, type: str, amount: str, price: str, client_order_id: str,
-                     note: str, third_identity_id: str):
+    def create_order(
+            self,
+            symbol: str, 
+            side: str, 
+            type: str, 
+            amount: str, 
+            price: str, 
+            client_order_id: str, 
+            third_identity_id: str, 
+            note: str = ''
+        ):
         signature = self.encryption_api_key()
         if signature == "fail":
-            return "Create Order Api Key error"
+            raise Exception("Create Order Api Key error")
 
         url = f"{self.base_url}/create_order"
         headers = {
             'Content-Type': 'application/json',
         }
         data = {
             "symbol": symbol,
@@ -146,18 +162,22 @@
         response = requests.post(url, data=json.dumps(data), headers=headers)
         if response.status_code == 200:
             res = response.json()
             return res["data"]
         else:
             raise Exception(response.text)
 
-    def fetch_order(self, id: str, note: str = '', third_identity_id: str = ''):
+    def fetch_order(self, 
+            id: str, 
+            note: str = '', 
+            third_identity_id: str = ''
+        ):
         signature = self.encryption_api_key()
         if signature == "fail":
-            return "Fetch Order Api Key error"
+            raise Exception("Fetch Order Api Key error")
 
         url = f"{self.base_url}/fetch_order"
         headers = {
             'Content-Type': 'application/json',
         }
         data = {
             "id": id,
@@ -171,21 +191,31 @@
         response = requests.post(url, data=json.dumps(data), headers=headers)
         if response.status_code == 200:
             res = response.json()
             return res["data"]
         else:
             raise Exception(response.text)
 
-    def fetch_orders(self, symbol: str = '', start_datetime: int = '', end_datetime: int = 0, page: int = '',
-                     limit: int = '', ids: str = "", status: str = "", sort_order: str = "", order_type: str = "",
-                     side: str = "", third_identity_id: str = "", note: str = ""
-                     ):
+    def fetch_orders(self, 
+            symbol: str = '', 
+            start_datetime: int = 0, 
+            end_datetime: int = 0, 
+            page: int = 0,
+            limit: int = 500, 
+            ids: str = "", 
+            status: str = "", 
+            sort_order: str = "", 
+            order_type: str = "",
+            side: str = "", 
+            third_identity_id: str = "", 
+            note: str = ""
+        ):
         signature = self.encryption_api_key()
         if signature == "fail":
-            return "Fetch Orders Api Key error"
+            raise Exception("Fetch Orders Api Key error")
 
         url = f"{self.base_url}/fetch_orders"
         headers = {
             'Content-Type': 'application/json',
         }
         data = {
             "symbol": symbol,
```

