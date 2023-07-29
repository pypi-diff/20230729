# Comparing `tmp/metabase-api-python-0.0.5.tar.gz` & `tmp/metabase-api-python-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabase-api-python-0.0.5.tar", last modified: Sat Jul 29 10:32:28 2023, max compression
+gzip compressed data, was "metabase-api-python-0.0.6.tar", last modified: Sat Jul 29 10:59:08 2023, max compression
```

## Comparing `metabase-api-python-0.0.5.tar` & `metabase-api-python-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 10:32:28.576439 metabase-api-python-0.0.5/
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      586 2023-07-29 10:32:28.571448 metabase-api-python-0.0.5/PKG-INFO
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)     2320 2023-07-29 09:32:12.000000 metabase-api-python-0.0.5/README.md
-drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 10:32:28.314871 metabase-api-python-0.0.5/metabase_api/
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)       38 2023-07-29 10:28:42.000000 metabase-api-python-0.0.5/metabase_api/__init__.py
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      312 2023-07-29 08:37:21.000000 metabase-api-python-0.0.5/metabase_api/exceptions.py
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)     2700 2023-07-29 10:31:47.000000 metabase-api-python-0.0.5/metabase_api/metabase_api.py
-drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 10:32:28.525908 metabase-api-python-0.0.5/metabase_api_python.egg-info/
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      586 2023-07-29 10:32:27.000000 metabase-api-python-0.0.5/metabase_api_python.egg-info/PKG-INFO
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      313 2023-07-29 10:32:28.000000 metabase-api-python-0.0.5/metabase_api_python.egg-info/SOURCES.txt
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)        1 2023-07-29 10:32:27.000000 metabase-api-python-0.0.5/metabase_api_python.egg-info/dependency_links.txt
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)       17 2023-07-29 10:32:27.000000 metabase-api-python-0.0.5/metabase_api_python.egg-info/requires.txt
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)       13 2023-07-29 10:32:27.000000 metabase-api-python-0.0.5/metabase_api_python.egg-info/top_level.txt
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)       38 2023-07-29 10:32:28.578666 metabase-api-python-0.0.5/setup.cfg
--rwxrwxrwx   0 cisco     (1000) cisco     (1000)      806 2023-07-29 10:31:54.000000 metabase-api-python-0.0.5/setup.py
+drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 10:59:08.231343 metabase-api-python-0.0.6/
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      586 2023-07-29 10:59:08.225799 metabase-api-python-0.0.6/PKG-INFO
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)     3686 2023-07-29 10:57:02.000000 metabase-api-python-0.0.6/README.md
+drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 10:59:07.946410 metabase-api-python-0.0.6/metabase_api_python/
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)       38 2023-07-29 10:58:00.000000 metabase-api-python-0.0.6/metabase_api_python/__init__.py
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      312 2023-07-29 08:37:21.000000 metabase-api-python-0.0.6/metabase_api_python/exceptions.py
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)     2700 2023-07-29 10:57:56.000000 metabase-api-python-0.0.6/metabase_api_python/metabase_api.py
+drwxrwxrwx   0 cisco     (1000) cisco     (1000)        0 2023-07-29 10:59:08.178632 metabase-api-python-0.0.6/metabase_api_python.egg-info/
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      586 2023-07-29 10:59:07.000000 metabase-api-python-0.0.6/metabase_api_python.egg-info/PKG-INFO
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      334 2023-07-29 10:59:07.000000 metabase-api-python-0.0.6/metabase_api_python.egg-info/SOURCES.txt
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)        1 2023-07-29 10:59:07.000000 metabase-api-python-0.0.6/metabase_api_python.egg-info/dependency_links.txt
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)       17 2023-07-29 10:59:07.000000 metabase-api-python-0.0.6/metabase_api_python.egg-info/requires.txt
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)       20 2023-07-29 10:59:07.000000 metabase-api-python-0.0.6/metabase_api_python.egg-info/top_level.txt
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)       38 2023-07-29 10:59:08.233345 metabase-api-python-0.0.6/setup.cfg
+-rwxrwxrwx   0 cisco     (1000) cisco     (1000)      806 2023-07-29 10:58:22.000000 metabase-api-python-0.0.6/setup.py
```

### Comparing `metabase-api-python-0.0.5/PKG-INFO` & `metabase-api-python-0.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabase-api-python
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python wrapper for the Metabase REST API. This package provides easy-to-use functions to interact with Metabase programmatically, enabling operations like fetching data from saved questions, archiving or deleting cards, and more. Ideal for data engineers, data analysts, or anyone looking to integrate Metabase with their Python applications.
 Home-page: https://github.com/Cisco141632/metabase-api-python
 Author: Cisco141632
 Author-email: durgaprasad141632@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `metabase-api-python-0.0.5/README.md` & `metabase-api-python-0.0.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -26,22 +26,61 @@
 - After installing Docker, you can check whether it's been installed correctly by opening a terminal and running the following command:
 
 
 ```shell
 docker --version
 ```
 
-### Steps
+### Steps For Metabase Setup
 
 1. **Pull the Metabase image from Docker Hub**
     - Open a terminal and run the following command: `docker pull metabase/metabase`
 
 2. **Run the Metabase Docker container**
     - Run the command: `docker run -d -p 3000:3000 --name metabase metabase/metabase`
 
 3. **Access Metabase**
     - Open your browser and visit `http://localhost:3000`
     - You will be greeted with the Metabase setup wizard. Follow the prompts to set up an account and connect your data sources.
 
 4. **Create and Save a Question**
     - In Metabase, create a new 'question' (a query or report), and save it to your 'Personal Collection' or any other collection.
 
+### Installing `metabase-api-python`
+
+Before you begin, make sure you have Python3 and pip3 installed on your system. If not, refer to the official Python [installation guide](https://www.python.org/downloads/) and pip [installation guide](https://pip.pypa.io/en/stable/installation/).
+
+
+Follow the steps below to install the `metabase-api-python` package:
+
+1. Open a terminal.
+
+2. If you're using a virtual environment (which is a good practice), make sure to activate it. If you're not, that's perfectly fine too.
+
+3. Use pip to install the `metabase-api-python` package from PyPi:
+
+    ```shell
+    pip3 install metabase-api-python
+    ```
+
+4. Now, you can use the `metabase-api-python` package in your Python scripts. Here's a basic example:
+
+    ```python
+    from metabase_api_python import MetabaseAPI
+
+	metabase_api = MetabaseAPI(
+		base_url="http://localhost:3000", 
+		user_name="YOUR_USERNAME", 
+		password="YOUR_PASSWORD"
+	)
+
+	print("Access Token is : ", metabase_api.access_token)
+    ```
+
+Please replace `YOUR_USERNAME` and `YOUR_PASSWORD` with your actual Metabase credentials. 
+
+Remember, always keep these credentials secure. Do not expose them in any places. 
+
+Note: The installation process might vary slightly depending on your operating system and the specific configuration of your Python environment.
+
+
+### Avalable Functions
```

### Comparing `metabase-api-python-0.0.5/metabase_api/metabase_api.py` & `metabase-api-python-0.0.6/metabase_api_python/metabase_api.py`

 * *Files identical despite different names*

### Comparing `metabase-api-python-0.0.5/metabase_api_python.egg-info/PKG-INFO` & `metabase-api-python-0.0.6/metabase_api_python.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabase-api-python
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python wrapper for the Metabase REST API. This package provides easy-to-use functions to interact with Metabase programmatically, enabling operations like fetching data from saved questions, archiving or deleting cards, and more. Ideal for data engineers, data analysts, or anyone looking to integrate Metabase with their Python applications.
 Home-page: https://github.com/Cisco141632/metabase-api-python
 Author: Cisco141632
 Author-email: durgaprasad141632@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `metabase-api-python-0.0.5/setup.py` & `metabase-api-python-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read requirements.txt file
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name='metabase-api-python',
-    version='0.0.5',
+    version='0.0.6',
     url='https://github.com/Cisco141632/metabase-api-python',
     author='Cisco141632',
     author_email='durgaprasad141632@gmail.com',
     description='A Python wrapper for the Metabase REST API. This package provides easy-to-use functions to interact with Metabase programmatically, enabling operations like fetching data from saved questions, archiving or deleting cards, and more. Ideal for data engineers, data analysts, or anyone looking to integrate Metabase with their Python applications.',
     packages=find_packages(),    
     install_requires=requirements,
 )
```

