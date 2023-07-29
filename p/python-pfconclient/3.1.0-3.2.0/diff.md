# Comparing `tmp/python-pfconclient-3.1.0.tar.gz` & `tmp/python-pfconclient-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-pfconclient-3.1.0.tar", last modified: Tue Jul 25 16:30:13 2023, max compression
+gzip compressed data, was "python-pfconclient-3.2.0.tar", last modified: Sat Jul 29 17:18:36 2023, max compression
```

## Comparing `python-pfconclient-3.1.0.tar` & `python-pfconclient-3.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jbernal    (501) staff       (20)        0 2023-07-25 16:30:13.877142 python-pfconclient-3.1.0/
--rw-r--r--   0 jbernal    (501) staff       (20)     9002 2023-07-25 16:30:13.876743 python-pfconclient-3.1.0/PKG-INFO
--rw-r--r--   0 jbernal    (501) staff       (20)     6928 2023-07-21 22:52:15.000000 python-pfconclient-3.1.0/README.rst
-drwxr-xr-x   0 jbernal    (501) staff       (20)        0 2023-07-25 16:30:13.873203 python-pfconclient-3.1.0/bin/
--rwxr-xr-x   0 jbernal    (501) staff       (20)     8796 2023-07-21 22:52:15.000000 python-pfconclient-3.1.0/bin/pfconclient
-drwxr-xr-x   0 jbernal    (501) staff       (20)        0 2023-07-25 16:30:13.873926 python-pfconclient-3.1.0/pfconclient/
--rwxr-xr-x   0 jbernal    (501) staff       (20)        0 2020-05-04 16:56:02.000000 python-pfconclient-3.1.0/pfconclient/__init__.py
--rwxr-xr-x   0 jbernal    (501) staff       (20)    10138 2023-07-25 03:51:12.000000 python-pfconclient-3.1.0/pfconclient/client.py
--rwxr-xr-x   0 jbernal    (501) staff       (20)      247 2022-01-21 01:15:14.000000 python-pfconclient-3.1.0/pfconclient/exceptions.py
-drwxr-xr-x   0 jbernal    (501) staff       (20)        0 2023-07-25 16:30:13.876080 python-pfconclient-3.1.0/python_pfconclient.egg-info/
--rw-r--r--   0 jbernal    (501) staff       (20)     9002 2023-07-25 16:30:13.000000 python-pfconclient-3.1.0/python_pfconclient.egg-info/PKG-INFO
--rw-r--r--   0 jbernal    (501) staff       (20)      357 2023-07-25 16:30:13.000000 python-pfconclient-3.1.0/python_pfconclient.egg-info/SOURCES.txt
--rw-r--r--   0 jbernal    (501) staff       (20)        1 2023-07-25 16:30:13.000000 python-pfconclient-3.1.0/python_pfconclient.egg-info/dependency_links.txt
--rw-r--r--   0 jbernal    (501) staff       (20)        1 2021-01-08 19:12:41.000000 python-pfconclient-3.1.0/python_pfconclient.egg-info/not-zip-safe
--rw-r--r--   0 jbernal    (501) staff       (20)       17 2023-07-25 16:30:13.000000 python-pfconclient-3.1.0/python_pfconclient.egg-info/requires.txt
--rw-r--r--   0 jbernal    (501) staff       (20)       12 2023-07-25 16:30:13.000000 python-pfconclient-3.1.0/python_pfconclient.egg-info/top_level.txt
--rw-r--r--   0 jbernal    (501) staff       (20)       38 2023-07-25 16:30:13.877248 python-pfconclient-3.1.0/setup.cfg
--rw-r--r--   0 jbernal    (501) staff       (20)      829 2023-07-25 16:27:24.000000 python-pfconclient-3.1.0/setup.py
+drwxr-xr-x   0 jbernal    (501) staff       (20)        0 2023-07-29 17:18:36.921287 python-pfconclient-3.2.0/
+-rw-r--r--   0 jbernal    (501) staff       (20)     9002 2023-07-29 17:18:36.921033 python-pfconclient-3.2.0/PKG-INFO
+-rw-r--r--   0 jbernal    (501) staff       (20)     6928 2023-07-21 22:52:15.000000 python-pfconclient-3.2.0/README.rst
+drwxr-xr-x   0 jbernal    (501) staff       (20)        0 2023-07-29 17:18:36.918048 python-pfconclient-3.2.0/bin/
+-rwxr-xr-x   0 jbernal    (501) staff       (20)     8796 2023-07-21 22:52:15.000000 python-pfconclient-3.2.0/bin/pfconclient
+drwxr-xr-x   0 jbernal    (501) staff       (20)        0 2023-07-29 17:18:36.918650 python-pfconclient-3.2.0/pfconclient/
+-rwxr-xr-x   0 jbernal    (501) staff       (20)        0 2020-05-04 16:56:02.000000 python-pfconclient-3.2.0/pfconclient/__init__.py
+-rwxr-xr-x   0 jbernal    (501) staff       (20)    10541 2023-07-29 16:52:00.000000 python-pfconclient-3.2.0/pfconclient/client.py
+-rwxr-xr-x   0 jbernal    (501) staff       (20)      247 2022-01-21 01:15:14.000000 python-pfconclient-3.2.0/pfconclient/exceptions.py
+drwxr-xr-x   0 jbernal    (501) staff       (20)        0 2023-07-29 17:18:36.920668 python-pfconclient-3.2.0/python_pfconclient.egg-info/
+-rw-r--r--   0 jbernal    (501) staff       (20)     9002 2023-07-29 17:18:36.000000 python-pfconclient-3.2.0/python_pfconclient.egg-info/PKG-INFO
+-rw-r--r--   0 jbernal    (501) staff       (20)      357 2023-07-29 17:18:36.000000 python-pfconclient-3.2.0/python_pfconclient.egg-info/SOURCES.txt
+-rw-r--r--   0 jbernal    (501) staff       (20)        1 2023-07-29 17:18:36.000000 python-pfconclient-3.2.0/python_pfconclient.egg-info/dependency_links.txt
+-rw-r--r--   0 jbernal    (501) staff       (20)        1 2021-01-08 19:12:41.000000 python-pfconclient-3.2.0/python_pfconclient.egg-info/not-zip-safe
+-rw-r--r--   0 jbernal    (501) staff       (20)       17 2023-07-29 17:18:36.000000 python-pfconclient-3.2.0/python_pfconclient.egg-info/requires.txt
+-rw-r--r--   0 jbernal    (501) staff       (20)       12 2023-07-29 17:18:36.000000 python-pfconclient-3.2.0/python_pfconclient.egg-info/top_level.txt
+-rw-r--r--   0 jbernal    (501) staff       (20)       38 2023-07-29 17:18:36.921358 python-pfconclient-3.2.0/setup.cfg
+-rw-r--r--   0 jbernal    (501) staff       (20)      829 2023-07-29 17:16:13.000000 python-pfconclient-3.2.0/setup.py
```

### Comparing `python-pfconclient-3.1.0/PKG-INFO` & `python-pfconclient-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-pfconclient
-Version: 3.1.0
+Version: 3.2.0
 Summary: (Python) client for the Pfcon API
 Home-page: https://github.com/FNNDSC/python-pfconclient
 Author: FNNDSC
 Author-email: dev@babymri.org
 License: MIT
 Description: ##################
         python-pfconclient
```

### Comparing `python-pfconclient-3.1.0/README.rst` & `python-pfconclient-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-pfconclient-3.1.0/bin/pfconclient` & `python-pfconclient-3.2.0/bin/pfconclient`

 * *Files identical despite different names*

### Comparing `python-pfconclient-3.1.0/pfconclient/client.py` & `python-pfconclient-3.2.0/pfconclient/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,38 @@
 
 
 class Client(object):
     """
     A pfcon API client.
     """
 
-    def __init__(self, url, auth_token, pfcon_innetwork=False):
+    def __init__(self, url, auth_token):
         self.url = url
         self.set_auth_token(auth_token)
-        self.pfcon_innetwork = pfcon_innetwork
+        self.pfcon_innetwork = None
 
         # initial and maximum wait time (seconds) for exponential-backoff-based retries
         self.initial_wait = 2
         self.max_wait = 2**15
 
     def set_auth_token(self, auth_token):
         if not auth_token:
             raise PfconRequestInvalidTokenException(f'Invalid auth token: {auth_token}')
         self.auth_token = str(auth_token)
 
+    def get_server_info(self, timeout=30):
+        """
+        Get info about the PFCON server.
+        """
+        url = self.url + 'jobs/'
+        resp = self.get(url, timeout)
+        data = self.get_data_from_response(resp)
+        self.pfcon_innetwork = data.get('pfcon_innetwork')
+        return data
+
     def run_job(self, job_id, d_job_descriptors, input_dir, output_dir, timeout=1000):
         """
         Run a new job by taking the passed input_dir and output_dir as the
         local input and output directories for the plugin respectively.
         """
         # create job zip file content from local input_dir
         job_zip_file = self.create_zip_file(input_dir)
@@ -94,27 +104,31 @@
             else:
                 wait_time = self.initial_wait * 2 ** poll_num
                 poll_num += 1
         return status
 
     def get_job_json_data(self, job_id, job_output_path, timeout=1000):
         """
-        Get a job's JSON file content. This only works for pfcon in-network mode
+        Get a job's JSON file content. This only works for pfcon in-network mode.
         """
+        if self.pfcon_innetwork is None:
+            self.get_server_info()
+
         if not self.pfcon_innetwork:
             raise PfconRequestException('JSON data is only available for PFCON server '
                                         'operating in-network')
         url = self.url + 'jobs/' + job_id + '/file/?job_output_path=' + job_output_path
         resp = self.get(url, timeout)
         json_content = self.get_data_from_response(resp)
         return json_content
 
     def get_job_json_file(self, job_id, job_output_path, local_dir, timeout=1000):
         """
-        Get and save a job's zip file into a local directory.
+        Get and save a job's JSON file into a local directory. This only works for
+        pfcon in-network mode
         """
         if not os.path.exists(local_dir):
             os.makedirs(local_dir)
         json_content = self.get_job_json_data(job_id, job_output_path, timeout)
         fpath = os.path.join(local_dir, job_id + '.json')
         with open(fpath, 'w') as f:
             json.dump(json_content, f)
```

### Comparing `python-pfconclient-3.1.0/python_pfconclient.egg-info/PKG-INFO` & `python-pfconclient-3.2.0/python_pfconclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-pfconclient
-Version: 3.1.0
+Version: 3.2.0
 Summary: (Python) client for the Pfcon API
 Home-page: https://github.com/FNNDSC/python-pfconclient
 Author: FNNDSC
 Author-email: dev@babymri.org
 License: MIT
 Description: ##################
         python-pfconclient
```

### Comparing `python-pfconclient-3.1.0/setup.py` & `python-pfconclient-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open(path.join(path.dirname(path.abspath(__file__)), 'README.rst')) as f:
     readme = f.read()
 
 setup(
       name             =   'python-pfconclient',
-      version          =   '3.1.0',
+      version          =   '3.2.0',
       description      =   '(Python) client for the Pfcon API',
       long_description =   readme,
       author           =   'FNNDSC',
       author_email     =   'dev@babymri.org',
       url              =   'https://github.com/FNNDSC/python-pfconclient',
       packages         =   ['pfconclient'],
       install_requires =   ['requests>=2.27.1'],
```

