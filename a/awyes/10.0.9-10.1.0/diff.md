# Comparing `tmp/awyes-10.0.9.tar.gz` & `tmp/awyes-10.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awyes-10.0.9.tar", last modified: Fri Jul 28 06:01:26 2023, max compression
+gzip compressed data, was "awyes-10.1.0.tar", last modified: Sat Jul 29 21:29:58 2023, max compression
```

## Comparing `awyes-10.0.9.tar` & `awyes-10.1.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:01:26.781810 awyes-10.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 06:01:26.781810 awyes-10.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-28 06:01:04.000000 awyes-10.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 06:01:25.000000 awyes-10.0.9/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:01:26.781810 awyes-10.0.9/awyes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:01:04.000000 awyes-10.0.9/awyes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-28 06:01:04.000000 awyes-10.0.9/awyes/awyes.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-28 06:01:04.000000 awyes-10.0.9/awyes/awyes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-28 06:01:04.000000 awyes-10.0.9/awyes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:01:26.781810 awyes-10.0.9/awyes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 06:01:26.000000 awyes-10.0.9/awyes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 06:01:26.000000 awyes-10.0.9/awyes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 06:01:26.000000 awyes-10.0.9/awyes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 06:01:26.000000 awyes-10.0.9/awyes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 06:01:26.000000 awyes-10.0.9/awyes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 06:01:26.000000 awyes-10.0.9/awyes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 06:01:26.781810 awyes-10.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 06:01:04.000000 awyes-10.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:29:58.014737 awyes-10.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 21:29:58.014737 awyes-10.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-29 21:29:35.000000 awyes-10.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:29:58.010737 awyes-10.1.0/awyes/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 21:29:56.000000 awyes-10.1.0/awyes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-29 21:29:35.000000 awyes-10.1.0/awyes/awyes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-29 21:29:35.000000 awyes-10.1.0/awyes/awyes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-29 21:29:35.000000 awyes-10.1.0/awyes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:29:58.014737 awyes-10.1.0/awyes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 21:29:57.000000 awyes-10.1.0/awyes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-29 21:29:57.000000 awyes-10.1.0/awyes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 21:29:57.000000 awyes-10.1.0/awyes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-29 21:29:57.000000 awyes-10.1.0/awyes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 21:29:57.000000 awyes-10.1.0/awyes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 21:29:57.000000 awyes-10.1.0/awyes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 21:29:58.014737 awyes-10.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-29 21:29:35.000000 awyes-10.1.0/setup.py
```

### Comparing `awyes-10.0.9/PKG-INFO` & `awyes-10.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 10.0.9
+Version: 10.1.0
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-10.0.9/awyes/awyes.py` & `awyes-10.1.0/awyes/awyes.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 class Deployment:
     def __init__(self, path="", verbose=False):
         # Initialize paths and log settings
         self.path = path
         self.verbose = verbose
 
-        # Load the config and docker images
-        with open(normpath(self.path)) as config:
+        # Load the clients and config
+        with open(normpath(path)) as config:
             self.config = yaml.safe_load(config)
             self.clients = {
                 "os": os,
                 "s3": boto3.client("s3"),
                 "ecr": boto3.client("ecr"),
                 "sts": boto3.client("sts"),
                 "iam": boto3.client("iam"),
@@ -80,38 +80,38 @@
 
             return value
 
         return args
 
     def deploy(self):
         for node in self.get_topologically_sorted_nodes():
-            name = getattr(node, "name")
-            args = getattr(node, "args")
-            client = getattr(node, "client")
+            node_name = rgetattr(node, "name")
+            node_args = rgetattr(node, "args")
+            node_client = rgetattr(self.clients, rgetattr(node, "client"))
 
-            resource_name, action_name = name.split(".")
+            resource_name, action_name = node_name.split(".")
 
             try:
-                action = getattr(client, action_name)
-                value = action(**self.shared_lookup(args))
+                action = rgetattr(node_client, action_name)
+                value = action(**self.shared_lookup(node_args))
 
                 if self.verbose:
-                    print(f"setting value {value} for {name}")
+                    print(f"setting value {value} for {node_name}")
 
                 rsetattr(
                     context=self.config,
                     accessor=f"{resource_name}.{action_name}",
                     value=value,
                 )
             except Exception as e:
                 print("err: ", e)
 
 
 def main():
     _, *path = argv
-    path = path[0] if path else "./awyes"
+    path = path[0] if path else "./awyes.yml"
 
     Deployment(path=path).deploy()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `awyes-10.0.9/awyes/awyes_test.py` & `awyes-10.1.0/awyes/awyes_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import yaml
 from .awyes import Deployment
 
 
 class DeploymentTestSuccess(unittest.TestCase):
     def __init__(self, *args, **kwargs):
         super(DeploymentTestSuccess, self).__init__(*args, **kwargs)
-        self.good_yaml = yaml.safe_load("./test_data/good.yml")
+        self.good_yaml = yaml.safe_load("./awyes/test_data/good.yml")
 
-    def test_ordering(self):
-        d = Deployment(path="./test_data/good.yml")
+    def test_ordering_and_populated_fields(self):
+        d = Deployment(path="./awyes/test_data/good.yml")
         sorted_nodes = d.get_topologically_sorted_nodes()
         self.assertEqual(sorted_nodes, [
             {
                 'client': 'some_other_client',
                 'args': {'another': 'argument'},
                 'name': 'some_namespace.some_other_action',
                 'depends_on': []
```

### Comparing `awyes-10.0.9/awyes/utils.py` & `awyes-10.1.0/awyes/utils.py`

 * *Files identical despite different names*

### Comparing `awyes-10.0.9/awyes.egg-info/PKG-INFO` & `awyes-10.1.0/awyes.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 10.0.9
+Version: 10.1.0
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-10.0.9/setup.py` & `awyes-10.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import awyes
 from setuptools import setup, find_packages
 
 setup(
     name='awyes',
     author='Truman Purnell',
     author_email='truman.purnell@gmail.com',
+    version=awyes.__version__,
     description='A package for easy setup and management of resources on AWS',
     url='https://github.com/bb-labs/awyes',
     packages=find_packages(),
     install_requires=[
         'boto3',
         'docker',
         'pyyaml',
```

