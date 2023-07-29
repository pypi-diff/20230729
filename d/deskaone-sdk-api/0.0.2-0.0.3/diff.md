# Comparing `tmp/deskaone_sdk_api-0.0.2.tar.gz` & `tmp/deskaone_sdk_api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deskaone_sdk_api-0.0.2.tar", max compression
+gzip compressed data, was "deskaone_sdk_api-0.0.3.tar", max compression
```

## Comparing `deskaone_sdk_api-0.0.2.tar` & `deskaone_sdk_api-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      737 2023-07-03 11:53:18.312210 deskaone_sdk_api-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       28 2023-06-26 10:17:37.373451 deskaone_sdk_api-0.0.2/README.md
--rw-r--r--   0        0        0      356 2023-06-26 04:21:27.302553 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/__init__.py
--rw-r--r--   0        0        0     6184 2023-06-26 04:20:41.837278 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Client/__init__.py
--rw-r--r--   0        0        0      793 2023-06-26 04:19:31.636954 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Database/__init__.py
--rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Exceptions/__init__.py
--rw-r--r--   0        0        0     2931 2023-06-26 04:19:31.581954 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Internal/__init__.py
--rw-r--r--   0        0        0      460 2023-07-03 11:53:11.584451 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/__init__.py
--rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/AWSViker.py
--rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Color.py
--rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Crypto.py
--rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/ProgressBar.py
--rw-r--r--   0        0        0    38295 2023-07-03 11:52:57.986206 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Proxy.py
--rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Random.py
--rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Reset.py
--rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Reverse.py
--rw-r--r--   0        0        0     2956 2023-06-26 04:19:31.581954 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Timer.py
--rw-r--r--   0        0        0     3569 2023-06-26 04:19:31.581954 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Typer.py
--rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/UserAgent.py
--rw-r--r--   0        0        0     1264 1970-01-01 00:00:00.000000 deskaone_sdk_api-0.0.2/setup.py
--rw-r--r--   0        0        0     1131 1970-01-01 00:00:00.000000 deskaone_sdk_api-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      737 2023-07-29 12:59:25.168603 deskaone_sdk_api-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-06-26 10:17:37.373451 deskaone_sdk_api-0.0.3/README.md
+-rw-r--r--   0        0        0      356 2023-06-26 04:21:27.302553 deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/__init__.py
+-rw-r--r--   0        0        0     6184 2023-06-26 04:20:41.837278 deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Client/__init__.py
+-rw-r--r--   0        0        0      793 2023-06-26 04:19:31.636954 deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Database/__init__.py
+-rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Exceptions/__init__.py
+-rw-r--r--   0        0        0     3037 2023-07-29 12:25:39.969567 deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Internal/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-29 12:59:36.516570 deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/__init__.py
+-rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/AWSViker.py
+-rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/Color.py
+-rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/Crypto.py
+-rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/ProgressBar.py
+-rw-r--r--   0        0        0    38295 2023-07-03 11:52:57.986206 deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/Proxy.py
+-rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/Random.py
+-rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/Reset.py
+-rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/Reverse.py
+-rw-r--r--   0        0        0     2956 2023-06-26 04:19:31.581954 deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/Timer.py
+-rw-r--r--   0        0        0     3569 2023-06-26 04:19:31.581954 deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/Typer.py
+-rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/UserAgent.py
+-rw-r--r--   0        0        0     1264 1970-01-01 00:00:00.000000 deskaone_sdk_api-0.0.3/setup.py
+-rw-r--r--   0        0        0     1131 1970-01-01 00:00:00.000000 deskaone_sdk_api-0.0.3/PKG-INFO
```

### Comparing `deskaone_sdk_api-0.0.2/pyproject.toml` & `deskaone_sdk_api-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deskaone-sdk-api"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Antoni Oktha Fernandes <37358597+DesKaOne@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "deskaone_sdk_api", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Client/__init__.py` & `deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Database/__init__.py` & `deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Database/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Exceptions/__init__.py` & `deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Internal/__init__.py` & `deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Internal/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         params is Json/urlencode for POST/PUT or urlencode for GET
         """
         self.URL        = kwargs.get('URL')
         self.PARAMS     = kwargs.get('PARAMS')
         self.HEADERS    = kwargs.get('HEADERS')
         self.Session    = requests.Session()        
     
-    def Setup(self, *args, **kwargs):
+    def Setup(self, *args, **kwargs) -> dict:
         """A Internal Requests.
         
         Basic Usage::
 
             Internal(
                 URL     = str,
                 PARAMS  = str | JSON | URLENCODE,
@@ -58,16 +58,16 @@
             if self.METHODS == 'POST':Result = self.Session.post(self.URL, data=self.PARAMS, headers=self.HEADERS, timeout=self.TIMEOUT)
             elif self.METHODS == 'PUT':Result = self.Session.put(self.URL, data=self.PARAMS, headers=self.HEADERS, timeout=self.TIMEOUT)
             else:
                 if self.PARAMS is None:Result = self.Session.get(self.URL, headers=self.HEADERS, timeout=self.TIMEOUT)
                 else:Result = self.Session.get(self.URL, params=self.PARAMS, headers=self.HEADERS, timeout=self.TIMEOUT)
             self.Session.close()
             
-            try:return dict(json.loads(Result.text))
-            except:return str(Result.text)
+            try:return dict(Result = dict(json.loads(Result.text)), status_code = Result.status_code)
+            except:return dict(Result = str(Result.text), status_code = Result.status_code)
         except ProxyError as e:raise Error(f'ProxyError')
         except ConnectTimeout as e:raise Error(f'ConnectTimeout')
         except ConnectionError as e:raise Error(f'ConnectionError')
         except ReadTimeout as e:raise Error(f'ReadTimeout')
         except JSONDecodeError:raise Error(f'JSONDecodeError')
         except TooManyRedirects as e:raise Error(f'TooManyRedirects')
         except Exception as e:raise Exception(str(e))
```

### Comparing `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/AWSViker.py` & `deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/AWSViker.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Crypto.py` & `deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/Crypto.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/ProgressBar.py` & `deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Proxy.py` & `deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/Proxy.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Random.py` & `deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/Random.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Timer.py` & `deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/Timer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Typer.py` & `deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/Typer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/UserAgent.py` & `deskaone_sdk_api-0.0.3/src/deskaone_sdk_api/Utils/UserAgent.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.2/setup.py` & `deskaone_sdk_api-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
  'python-dotenv>=0.20.0,<0.21.0',
  'random-user-agent>=1.0.1,<2.0.0',
  'requests[socks]>=2.27.1,<3.0.0',
  'sqlalchemy==1.4.29']
 
 setup_kwargs = {
     'name': 'deskaone-sdk-api',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': '',
     'long_description': 'pip install deskaone-sdk-api',
     'author': 'Antoni Oktha Fernandes',
     'author_email': '37358597+DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `deskaone_sdk_api-0.0.2/PKG-INFO` & `deskaone_sdk_api-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deskaone-sdk-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: Antoni Oktha Fernandes
 Author-email: 37358597+DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

