# Comparing `tmp/metabase-api-python-0.0.1.tar.gz` & `tmp/metabase-api-python-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabase-api-python-0.0.1.tar", last modified: Sat Jul 29 08:50:48 2023, max compression
+gzip compressed data, was "metabase-api-python-0.0.2.tar", last modified: Sat Jul 29 09:43:58 2023, max compression
```

## Comparing `metabase-api-python-0.0.1.tar` & `metabase-api-python-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 08:50:48.903515 metabase-api-python-0.0.1/
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      586 2023-07-29 08:50:48.900440 metabase-api-python-0.0.1/PKG-INFO
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      996 2023-07-29 08:23:54.000000 metabase-api-python-0.0.1/README.md
-drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 08:50:48.780212 metabase-api-python-0.0.1/metabase_api/
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)        1 2023-07-29 08:37:26.000000 metabase-api-python-0.0.1/metabase_api/__init__.py
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      312 2023-07-29 08:37:21.000000 metabase-api-python-0.0.1/metabase_api/exceptions.py
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)     2822 2023-07-29 08:37:18.000000 metabase-api-python-0.0.1/metabase_api/metabase_api.py
-drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 08:50:48.877625 metabase-api-python-0.0.1/metabase_api_python.egg-info/
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      586 2023-07-29 08:50:48.000000 metabase-api-python-0.0.1/metabase_api_python.egg-info/PKG-INFO
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      313 2023-07-29 08:50:48.000000 metabase-api-python-0.0.1/metabase_api_python.egg-info/SOURCES.txt
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)        1 2023-07-29 08:50:48.000000 metabase-api-python-0.0.1/metabase_api_python.egg-info/dependency_links.txt
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)       17 2023-07-29 08:50:48.000000 metabase-api-python-0.0.1/metabase_api_python.egg-info/requires.txt
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)       13 2023-07-29 08:50:48.000000 metabase-api-python-0.0.1/metabase_api_python.egg-info/top_level.txt
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)       38 2023-07-29 08:50:48.904534 metabase-api-python-0.0.1/setup.cfg
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      806 2023-07-29 08:45:15.000000 metabase-api-python-0.0.1/setup.py
+drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 09:43:58.199158 metabase-api-python-0.0.2/
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      586 2023-07-29 09:43:58.196157 metabase-api-python-0.0.2/PKG-INFO
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)     2320 2023-07-29 09:32:12.000000 metabase-api-python-0.0.2/README.md
+drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 09:43:58.079415 metabase-api-python-0.0.2/metabase_api/
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)       38 2023-07-29 09:37:24.000000 metabase-api-python-0.0.2/metabase_api/__init__.py
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      312 2023-07-29 08:37:21.000000 metabase-api-python-0.0.2/metabase_api/exceptions.py
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)     2822 2023-07-29 09:39:56.000000 metabase-api-python-0.0.2/metabase_api/metabase_api.py
+drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 09:43:58.175128 metabase-api-python-0.0.2/metabase_api_python.egg-info/
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      586 2023-07-29 09:43:57.000000 metabase-api-python-0.0.2/metabase_api_python.egg-info/PKG-INFO
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      313 2023-07-29 09:43:57.000000 metabase-api-python-0.0.2/metabase_api_python.egg-info/SOURCES.txt
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)        1 2023-07-29 09:43:57.000000 metabase-api-python-0.0.2/metabase_api_python.egg-info/dependency_links.txt
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)       17 2023-07-29 09:43:57.000000 metabase-api-python-0.0.2/metabase_api_python.egg-info/requires.txt
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)       13 2023-07-29 09:43:57.000000 metabase-api-python-0.0.2/metabase_api_python.egg-info/top_level.txt
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)       38 2023-07-29 09:43:58.200157 metabase-api-python-0.0.2/setup.cfg
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      806 2023-07-29 09:42:08.000000 metabase-api-python-0.0.2/setup.py
```

### Comparing `metabase-api-python-0.0.1/PKG-INFO` & `metabase-api-python-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabase-api-python
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python wrapper for the Metabase REST API. This package provides easy-to-use functions to interact with Metabase programmatically, enabling operations like fetching data from saved questions, archiving or deleting cards, and more. Ideal for data engineers, data analysts, or anyone looking to integrate Metabase with their Python applications.
 Home-page: https://github.com/Cisco141632/metabase-api-python
 Author: Cisco141632
 Author-email: durgaprasad141632@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `metabase-api-python-0.0.1/metabase_api/metabase_api.py` & `metabase-api-python-0.0.2/metabase_api/metabase_api.py`

 * *Files identical despite different names*

### Comparing `metabase-api-python-0.0.1/metabase_api_python.egg-info/PKG-INFO` & `metabase-api-python-0.0.2/metabase_api_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabase-api-python
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python wrapper for the Metabase REST API. This package provides easy-to-use functions to interact with Metabase programmatically, enabling operations like fetching data from saved questions, archiving or deleting cards, and more. Ideal for data engineers, data analysts, or anyone looking to integrate Metabase with their Python applications.
 Home-page: https://github.com/Cisco141632/metabase-api-python
 Author: Cisco141632
 Author-email: durgaprasad141632@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `metabase-api-python-0.0.1/setup.py` & `metabase-api-python-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read requirements.txt file
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name='metabase-api-python',
-    version='0.0.1',
+    version='0.0.2',
     url='https://github.com/Cisco141632/metabase-api-python',
     author='Cisco141632',
     author_email='durgaprasad141632@gmail.com',
     description='A Python wrapper for the Metabase REST API. This package provides easy-to-use functions to interact with Metabase programmatically, enabling operations like fetching data from saved questions, archiving or deleting cards, and more. Ideal for data engineers, data analysts, or anyone looking to integrate Metabase with their Python applications.',
     packages=find_packages(),    
     install_requires=requirements,
 )
```

