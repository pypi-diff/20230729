# Comparing `tmp/metabase-api-python-0.0.6.tar.gz` & `tmp/metabase-api-python-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabase-api-python-0.0.6.tar", last modified: Sat Jul 29 10:59:08 2023, max compression
+gzip compressed data, was "metabase-api-python-0.0.7.tar", last modified: Sat Jul 29 11:12:46 2023, max compression
```

## Comparing `metabase-api-python-0.0.6.tar` & `metabase-api-python-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 10:59:08.231343 metabase-api-python-0.0.6/
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      586 2023-07-29 10:59:08.225799 metabase-api-python-0.0.6/PKG-INFO
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)     3686 2023-07-29 10:57:02.000000 metabase-api-python-0.0.6/README.md
-drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 10:59:07.946410 metabase-api-python-0.0.6/metabase_api_python/
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)       38 2023-07-29 10:58:00.000000 metabase-api-python-0.0.6/metabase_api_python/__init__.py
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      312 2023-07-29 08:37:21.000000 metabase-api-python-0.0.6/metabase_api_python/exceptions.py
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)     2700 2023-07-29 10:57:56.000000 metabase-api-python-0.0.6/metabase_api_python/metabase_api.py
-drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 10:59:08.178632 metabase-api-python-0.0.6/metabase_api_python.egg-info/
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      586 2023-07-29 10:59:07.000000 metabase-api-python-0.0.6/metabase_api_python.egg-info/PKG-INFO
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      334 2023-07-29 10:59:07.000000 metabase-api-python-0.0.6/metabase_api_python.egg-info/SOURCES.txt
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)        1 2023-07-29 10:59:07.000000 metabase-api-python-0.0.6/metabase_api_python.egg-info/dependency_links.txt
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)       17 2023-07-29 10:59:07.000000 metabase-api-python-0.0.6/metabase_api_python.egg-info/requires.txt
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)       20 2023-07-29 10:59:07.000000 metabase-api-python-0.0.6/metabase_api_python.egg-info/top_level.txt
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)       38 2023-07-29 10:59:08.233345 metabase-api-python-0.0.6/setup.cfg
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      806 2023-07-29 10:58:22.000000 metabase-api-python-0.0.6/setup.py
+drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 11:12:46.436524 metabase-api-python-0.0.7/
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      586 2023-07-29 11:12:46.430539 metabase-api-python-0.0.7/PKG-INFO
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)     3749 2023-07-29 11:10:54.000000 metabase-api-python-0.0.7/README.md
+drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 11:12:46.160199 metabase-api-python-0.0.7/metabase_api_python/
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)       38 2023-07-29 10:58:00.000000 metabase-api-python-0.0.7/metabase_api_python/__init__.py
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      312 2023-07-29 08:37:21.000000 metabase-api-python-0.0.7/metabase_api_python/exceptions.py
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)     2771 2023-07-29 11:09:54.000000 metabase-api-python-0.0.7/metabase_api_python/metabase_api.py
+drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 11:12:46.383158 metabase-api-python-0.0.7/metabase_api_python.egg-info/
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      586 2023-07-29 11:12:45.000000 metabase-api-python-0.0.7/metabase_api_python.egg-info/PKG-INFO
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      334 2023-07-29 11:12:45.000000 metabase-api-python-0.0.7/metabase_api_python.egg-info/SOURCES.txt
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)        1 2023-07-29 11:12:45.000000 metabase-api-python-0.0.7/metabase_api_python.egg-info/dependency_links.txt
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)       17 2023-07-29 11:12:45.000000 metabase-api-python-0.0.7/metabase_api_python.egg-info/requires.txt
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)       20 2023-07-29 11:12:45.000000 metabase-api-python-0.0.7/metabase_api_python.egg-info/top_level.txt
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)       38 2023-07-29 11:12:46.437533 metabase-api-python-0.0.7/setup.cfg
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      806 2023-07-29 11:12:10.000000 metabase-api-python-0.0.7/setup.py
```

### Comparing `metabase-api-python-0.0.6/PKG-INFO` & `metabase-api-python-0.0.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabase-api-python
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python wrapper for the Metabase REST API. This package provides easy-to-use functions to interact with Metabase programmatically, enabling operations like fetching data from saved questions, archiving or deleting cards, and more. Ideal for data engineers, data analysts, or anyone looking to integrate Metabase with their Python applications.
 Home-page: https://github.com/Cisco141632/metabase-api-python
 Author: Cisco141632
 Author-email: durgaprasad141632@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `metabase-api-python-0.0.6/README.md` & `metabase-api-python-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -79,8 +79,12 @@
 Please replace `YOUR_USERNAME` and `YOUR_PASSWORD` with your actual Metabase credentials. 
 
 Remember, always keep these credentials secure. Do not expose them in any places. 
 
 Note: The installation process might vary slightly depending on your operating system and the specific configuration of your Python environment.
 
 
-### Avalable Functions
+## Avalable Functions
+- get_data_from_question
+- archive_question
+- delete_question
+
```

### Comparing `metabase-api-python-0.0.6/metabase_api_python.egg-info/PKG-INFO` & `metabase-api-python-0.0.7/metabase_api_python.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabase-api-python
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python wrapper for the Metabase REST API. This package provides easy-to-use functions to interact with Metabase programmatically, enabling operations like fetching data from saved questions, archiving or deleting cards, and more. Ideal for data engineers, data analysts, or anyone looking to integrate Metabase with their Python applications.
 Home-page: https://github.com/Cisco141632/metabase-api-python
 Author: Cisco141632
 Author-email: durgaprasad141632@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `metabase-api-python-0.0.6/setup.py` & `metabase-api-python-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read requirements.txt file
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name='metabase-api-python',
-    version='0.0.6',
+    version='0.0.7',
     url='https://github.com/Cisco141632/metabase-api-python',
     author='Cisco141632',
     author_email='durgaprasad141632@gmail.com',
     description='A Python wrapper for the Metabase REST API. This package provides easy-to-use functions to interact with Metabase programmatically, enabling operations like fetching data from saved questions, archiving or deleting cards, and more. Ideal for data engineers, data analysts, or anyone looking to integrate Metabase with their Python applications.',
     packages=find_packages(),    
     install_requires=requirements,
 )
```

