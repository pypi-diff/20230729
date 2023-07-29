# Comparing `tmp/aiobaseclient-0.2.5.tar.gz` & `tmp/aiobaseclient-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiobaseclient-0.2.5.tar", last modified: Thu Jul 20 11:19:42 2023, max compression
+gzip compressed data, was "aiobaseclient-0.2.6.tar", last modified: Sat Jul 29 20:49:43 2023, max compression
```

## Comparing `aiobaseclient-0.2.5.tar` & `aiobaseclient-0.2.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-20 11:19:42.757535 aiobaseclient-0.2.5/
--rw-r--r--   0 pasha      (501) staff       (20)     1076 2022-10-25 06:23:07.000000 aiobaseclient-0.2.5/LICENSE
--rw-r--r--   0 pasha      (501) staff       (20)      303 2023-07-20 11:19:42.757727 aiobaseclient-0.2.5/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)       64 2022-10-25 06:23:07.000000 aiobaseclient-0.2.5/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-20 11:19:42.755326 aiobaseclient-0.2.5/aiobaseclient/
--rw-r--r--   0 pasha      (501) staff       (20)      110 2022-10-25 06:23:07.000000 aiobaseclient-0.2.5/aiobaseclient/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     9501 2023-07-20 11:14:12.000000 aiobaseclient-0.2.5/aiobaseclient/base.py
--rw-r--r--   0 pasha      (501) staff       (20)      968 2022-10-25 06:23:07.000000 aiobaseclient-0.2.5/aiobaseclient/exceptions.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-20 11:19:42.757146 aiobaseclient-0.2.5/aiobaseclient.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      303 2023-07-20 11:19:42.000000 aiobaseclient-0.2.5/aiobaseclient.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      302 2023-07-20 11:19:42.000000 aiobaseclient-0.2.5/aiobaseclient.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-20 11:19:42.000000 aiobaseclient-0.2.5/aiobaseclient.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)      151 2023-07-20 11:19:42.000000 aiobaseclient-0.2.5/aiobaseclient.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)       14 2023-07-20 11:19:42.000000 aiobaseclient-0.2.5/aiobaseclient.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)       89 2022-10-25 06:23:08.000000 aiobaseclient-0.2.5/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      653 2023-07-20 11:19:42.758456 aiobaseclient-0.2.5/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-29 20:49:43.336207 aiobaseclient-0.2.6/
+-rw-r--r--   0 pasha      (501) staff       (20)     1076 2022-10-25 06:23:07.000000 aiobaseclient-0.2.6/LICENSE
+-rw-r--r--   0 pasha      (501) staff       (20)      303 2023-07-29 20:49:43.336345 aiobaseclient-0.2.6/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)       64 2022-10-25 06:23:07.000000 aiobaseclient-0.2.6/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-29 20:49:43.333314 aiobaseclient-0.2.6/aiobaseclient/
+-rw-r--r--   0 pasha      (501) staff       (20)      110 2022-10-25 06:23:07.000000 aiobaseclient-0.2.6/aiobaseclient/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     9640 2023-07-29 20:49:00.000000 aiobaseclient-0.2.6/aiobaseclient/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)      968 2022-10-25 06:23:07.000000 aiobaseclient-0.2.6/aiobaseclient/exceptions.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-29 20:49:43.335889 aiobaseclient-0.2.6/aiobaseclient.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      303 2023-07-29 20:49:43.000000 aiobaseclient-0.2.6/aiobaseclient.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      302 2023-07-29 20:49:43.000000 aiobaseclient-0.2.6/aiobaseclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-29 20:49:43.000000 aiobaseclient-0.2.6/aiobaseclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      151 2023-07-29 20:49:43.000000 aiobaseclient-0.2.6/aiobaseclient.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       14 2023-07-29 20:49:43.000000 aiobaseclient-0.2.6/aiobaseclient.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       89 2022-10-25 06:23:08.000000 aiobaseclient-0.2.6/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      653 2023-07-29 20:49:43.337003 aiobaseclient-0.2.6/setup.cfg
```

### Comparing `aiobaseclient-0.2.5/LICENSE` & `aiobaseclient-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiobaseclient-0.2.5/aiobaseclient/base.py` & `aiobaseclient-0.2.6/aiobaseclient/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,18 @@
         if self.session:
             await self.session.close()
             self.session = None
 
     async def response_processor(self, response):
         text = await response.text()
         if response.status != 200:
-            raise ExternalServiceError(response.request.url, response.status, text)
+            if hasattr(response, 'request'):
+                raise ExternalServiceError(response.request.url, response.status, text)
+            else:
+                raise ExternalServiceError(None, response.status, text)
         return text
 
     async def __aenter__(self):
         await self.start()
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
```

### Comparing `aiobaseclient-0.2.5/aiobaseclient/exceptions.py` & `aiobaseclient-0.2.6/aiobaseclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiobaseclient-0.2.5/setup.cfg` & `aiobaseclient-0.2.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 classifiers = 
 	Topic :: Utilities
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = aiobaseclient
 python_requires = '>=3.8'
-version = 0.2.5
+version = 0.2.6
 url = https://github.com/izihawa/aiobaseclient
 
 [options]
 packages = find:
 install_requires = 
 	aiodns >= 2.0.0
 	aiohttp >= 3.6.3
```

