# Comparing `tmp/metabase-api-python-0.0.4.tar.gz` & `tmp/metabase-api-python-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabase-api-python-0.0.4.tar", last modified: Sat Jul 29 10:22:52 2023, max compression
+gzip compressed data, was "metabase-api-python-0.0.5.tar", last modified: Sat Jul 29 10:32:28 2023, max compression
```

## Comparing `metabase-api-python-0.0.4.tar` & `metabase-api-python-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 10:22:52.206834 metabase-api-python-0.0.4/
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      586 2023-07-29 10:22:52.200836 metabase-api-python-0.0.4/PKG-INFO
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)     2320 2023-07-29 09:32:12.000000 metabase-api-python-0.0.4/README.md
-drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 10:22:51.924206 metabase-api-python-0.0.4/metabase_api/
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)       64 2023-07-29 10:15:35.000000 metabase-api-python-0.0.4/metabase_api/__init__.py
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      312 2023-07-29 08:37:21.000000 metabase-api-python-0.0.4/metabase_api/exceptions.py
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)     2699 2023-07-29 10:11:57.000000 metabase-api-python-0.0.4/metabase_api/metabase_api.py
-drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 10:22:52.152285 metabase-api-python-0.0.4/metabase_api_python.egg-info/
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      586 2023-07-29 10:22:51.000000 metabase-api-python-0.0.4/metabase_api_python.egg-info/PKG-INFO
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      313 2023-07-29 10:22:51.000000 metabase-api-python-0.0.4/metabase_api_python.egg-info/SOURCES.txt
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)        1 2023-07-29 10:22:51.000000 metabase-api-python-0.0.4/metabase_api_python.egg-info/dependency_links.txt
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)       17 2023-07-29 10:22:51.000000 metabase-api-python-0.0.4/metabase_api_python.egg-info/requires.txt
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)       13 2023-07-29 10:22:51.000000 metabase-api-python-0.0.4/metabase_api_python.egg-info/top_level.txt
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)       38 2023-07-29 10:22:52.209383 metabase-api-python-0.0.4/setup.cfg
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      806 2023-07-29 10:15:23.000000 metabase-api-python-0.0.4/setup.py
+drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 10:32:28.576439 metabase-api-python-0.0.5/
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      586 2023-07-29 10:32:28.571448 metabase-api-python-0.0.5/PKG-INFO
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)     2320 2023-07-29 09:32:12.000000 metabase-api-python-0.0.5/README.md
+drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 10:32:28.314871 metabase-api-python-0.0.5/metabase_api/
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)       38 2023-07-29 10:28:42.000000 metabase-api-python-0.0.5/metabase_api/__init__.py
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      312 2023-07-29 08:37:21.000000 metabase-api-python-0.0.5/metabase_api/exceptions.py
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)     2700 2023-07-29 10:31:47.000000 metabase-api-python-0.0.5/metabase_api/metabase_api.py
+drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 10:32:28.525908 metabase-api-python-0.0.5/metabase_api_python.egg-info/
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      586 2023-07-29 10:32:27.000000 metabase-api-python-0.0.5/metabase_api_python.egg-info/PKG-INFO
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      313 2023-07-29 10:32:28.000000 metabase-api-python-0.0.5/metabase_api_python.egg-info/SOURCES.txt
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)        1 2023-07-29 10:32:27.000000 metabase-api-python-0.0.5/metabase_api_python.egg-info/dependency_links.txt
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)       17 2023-07-29 10:32:27.000000 metabase-api-python-0.0.5/metabase_api_python.egg-info/requires.txt
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)       13 2023-07-29 10:32:27.000000 metabase-api-python-0.0.5/metabase_api_python.egg-info/top_level.txt
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)       38 2023-07-29 10:32:28.578666 metabase-api-python-0.0.5/setup.cfg
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      806 2023-07-29 10:31:54.000000 metabase-api-python-0.0.5/setup.py
```

### Comparing `metabase-api-python-0.0.4/PKG-INFO` & `metabase-api-python-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabase-api-python
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python wrapper for the Metabase REST API. This package provides easy-to-use functions to interact with Metabase programmatically, enabling operations like fetching data from saved questions, archiving or deleting cards, and more. Ideal for data engineers, data analysts, or anyone looking to integrate Metabase with their Python applications.
 Home-page: https://github.com/Cisco141632/metabase-api-python
 Author: Cisco141632
 Author-email: durgaprasad141632@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `metabase-api-python-0.0.4/README.md` & `metabase-api-python-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `metabase-api-python-0.0.4/metabase_api/metabase_api.py` & `metabase-api-python-0.0.5/metabase_api/metabase_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import requests
 from urllib.parse import urlencode
-from exceptions import *
+from .exceptions import *
 
 class MetabaseAPI():
 	def __init__(self, base_url=None,user_name=None,password=None):
 		self.base_url = base_url
 		self.user_name = user_name
 		self.password = password
 		self.access_token = self._get_access_token()
```

### Comparing `metabase-api-python-0.0.4/metabase_api_python.egg-info/PKG-INFO` & `metabase-api-python-0.0.5/metabase_api_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabase-api-python
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python wrapper for the Metabase REST API. This package provides easy-to-use functions to interact with Metabase programmatically, enabling operations like fetching data from saved questions, archiving or deleting cards, and more. Ideal for data engineers, data analysts, or anyone looking to integrate Metabase with their Python applications.
 Home-page: https://github.com/Cisco141632/metabase-api-python
 Author: Cisco141632
 Author-email: durgaprasad141632@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `metabase-api-python-0.0.4/setup.py` & `metabase-api-python-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read requirements.txt file
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name='metabase-api-python',
-    version='0.0.4',
+    version='0.0.5',
     url='https://github.com/Cisco141632/metabase-api-python',
     author='Cisco141632',
     author_email='durgaprasad141632@gmail.com',
     description='A Python wrapper for the Metabase REST API. This package provides easy-to-use functions to interact with Metabase programmatically, enabling operations like fetching data from saved questions, archiving or deleting cards, and more. Ideal for data engineers, data analysts, or anyone looking to integrate Metabase with their Python applications.',
     packages=find_packages(),    
     install_requires=requirements,
 )
```

