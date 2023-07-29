# Comparing `tmp/knnor-0.1.1.tar.gz` & `tmp/knnor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knnor-0.1.1.tar", last modified: Sat Jul 29 13:19:22 2023, max compression
+gzip compressed data, was "knnor-0.1.2.tar", last modified: Sat Jul 29 13:53:32 2023, max compression
```

## Comparing `knnor-0.1.1.tar` & `knnor-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:19:22.213071 knnor-0.1.1/
--rw-r--r--   0 ashhadulislam   (503) staff       (20)     1063 2023-07-29 12:58:11.000000 knnor-0.1.1/LICENSE
--rw-r--r--   0 ashhadulislam   (503) staff       (20)       38 2023-07-29 12:58:11.000000 knnor-0.1.1/MANIFEST.in
--rw-r--r--   0 ashhadulislam   (503) staff       (20)      595 2023-07-29 13:19:22.212584 knnor-0.1.1/PKG-INFO
--rw-r--r--   0 ashhadulislam   (503) staff       (20)     5095 2023-07-29 12:58:11.000000 knnor-0.1.1/README.md
-drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:19:22.209322 knnor-0.1.1/knnor/
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 12:58:11.000000 knnor-0.1.1/knnor/__init__.py
--rw-r--r--   0 ashhadulislam   (503) staff       (20)    20656 2023-07-29 13:18:41.000000 knnor-0.1.1/knnor/data_augment.py
-drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:19:22.212082 knnor-0.1.1/knnor/tests/
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 12:58:11.000000 knnor-0.1.1/knnor/tests/__init__.py
--rw-r--r--   0 ashhadulislam   (503) staff       (20)      813 2023-07-29 12:58:11.000000 knnor-0.1.1/knnor/tests/test_augmented.py
-drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:19:22.211345 knnor-0.1.1/knnor.egg-info/
--rw-r--r--   0 ashhadulislam   (503) staff       (20)      595 2023-07-29 13:19:22.000000 knnor-0.1.1/knnor.egg-info/PKG-INFO
--rw-r--r--   0 ashhadulislam   (503) staff       (20)      304 2023-07-29 13:19:22.000000 knnor-0.1.1/knnor.egg-info/SOURCES.txt
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        1 2023-07-29 13:19:22.000000 knnor-0.1.1/knnor.egg-info/dependency_links.txt
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        1 2023-07-29 13:13:32.000000 knnor-0.1.1/knnor.egg-info/not-zip-safe
--rw-r--r--   0 ashhadulislam   (503) staff       (20)       19 2023-07-29 13:19:22.000000 knnor-0.1.1/knnor.egg-info/requires.txt
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        6 2023-07-29 13:19:22.000000 knnor-0.1.1/knnor.egg-info/top_level.txt
--rw-r--r--   0 ashhadulislam   (503) staff       (20)       38 2023-07-29 13:19:22.213185 knnor-0.1.1/setup.cfg
--rw-r--r--   0 ashhadulislam   (503) staff       (20)     1041 2023-07-29 13:19:05.000000 knnor-0.1.1/setup.py
+drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:53:32.852693 knnor-0.1.2/
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)     1063 2023-07-29 12:58:11.000000 knnor-0.1.2/LICENSE
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)       38 2023-07-29 12:58:11.000000 knnor-0.1.2/MANIFEST.in
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)      595 2023-07-29 13:53:32.852299 knnor-0.1.2/PKG-INFO
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)     5095 2023-07-29 12:58:11.000000 knnor-0.1.2/README.md
+drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:53:32.849708 knnor-0.1.2/knnor/
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 12:58:11.000000 knnor-0.1.2/knnor/__init__.py
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)    20806 2023-07-29 13:53:06.000000 knnor-0.1.2/knnor/data_augment.py
+drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:53:32.851838 knnor-0.1.2/knnor/tests/
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 12:58:11.000000 knnor-0.1.2/knnor/tests/__init__.py
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)      813 2023-07-29 12:58:11.000000 knnor-0.1.2/knnor/tests/test_augmented.py
+drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:53:32.851331 knnor-0.1.2/knnor.egg-info/
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)      595 2023-07-29 13:53:32.000000 knnor-0.1.2/knnor.egg-info/PKG-INFO
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)      304 2023-07-29 13:53:32.000000 knnor-0.1.2/knnor.egg-info/SOURCES.txt
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        1 2023-07-29 13:53:32.000000 knnor-0.1.2/knnor.egg-info/dependency_links.txt
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        1 2023-07-29 13:13:32.000000 knnor-0.1.2/knnor.egg-info/not-zip-safe
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)       19 2023-07-29 13:53:32.000000 knnor-0.1.2/knnor.egg-info/requires.txt
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        6 2023-07-29 13:53:32.000000 knnor-0.1.2/knnor.egg-info/top_level.txt
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)       38 2023-07-29 13:53:32.852796 knnor-0.1.2/setup.cfg
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)     1041 2023-07-29 13:53:19.000000 knnor-0.1.2/setup.py
```

### Comparing `knnor-0.1.1/LICENSE` & `knnor-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `knnor-0.1.1/PKG-INFO` & `knnor-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knnor
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generic python library to perform augmentation of multi class data.
 Home-page: 
 Author: Ashhadul Islam, Sameer Brahim Belhaouari, Atiq Ur Rahman, Halima Bensmail
 Author-email: ashhadulislam@gmail.com, samir.brahim@gmail.com, atrehman2@hbku.edu.qa, hbensmail@hbku.edu.qa
 License: MIT
 Keywords: Binary Classification,Data Augmentation,Imabalnced Data,MultiClass Classification
 License-File: LICENSE
```

### Comparing `knnor-0.1.1/README.md` & `knnor-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `knnor-0.1.1/knnor/data_augment.py` & `knnor-0.1.2/knnor/data_augment.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,26 +168,26 @@
 
 
 
         X_all_new_minorities=[]
         y_all_new_minorities=[]
         for minority_label in minority_labels:
 
-            print("Minority label",minority_label)
+#             print("Minority label",minority_label)
 
             other_labels=list(set(all_labels)-set([minority_label]))
             print(minority_label,other_labels)
             X_maj=[]
             for i in range(X.shape[0]):
                 if y[i] in other_labels:
                     X_maj.append(X[i])
 
             X_maj=np.array(X_maj)
             X_min=X[y==minority_label]
-            print(X_maj.shape,X_min.shape,X.shape)
+#             print(X_maj.shape,X_min.shape,X.shape)
             # count to add
             N=self.count_to_add(X_min,max_count,proportion)
 #             print("Count to add ",N)
 
 
             internal_distance = np.linalg.norm(X_min - X_min[:,None], axis = -1)
             internal_distance = np.sort(internal_distance)    
@@ -528,35 +528,40 @@
 def main():
     '''
     x^2 + y^2 + z^2 < 15 => 0
     x^2 + y^2 + z^2 >= 15 => 1
     '''
     l=[
 
-    [1.0,2.0,1.0,0],
-    [1,3,1,0],
-    [2,1,2,0],
-    [3,2,1,0],
-    [3,1,1,0],
-
-    [1,3,4,1],
-    [1,4,3,1],
-    [1,4,4,1],
-
-    [2,3,3,1],
-    [2,3,4,1],
-    [2,4,3,1],
-    [2,4,4,1],
-
-    [3,2,2,1],
-    [3,3,2,1],
-    [3,3,2,1],
-    [3,4,2,1],
+        [1.0,2.0,1.0,0],
+        [1,3,1,0],
+        [2,1,2,0],
+        [3,2,1,0],
+        [3,1,1,0],
+
+        [1,3,4,1],
+        [1,4,3,1],
+        [1,4,4,1],
+
+        [2,3,3,1],
+        [2,3,4,1],
+        [2,4,3,1],
+        [2,4,4,1],
+
+        [3,2,2,1],
+        [3,3,2,1],
+        [3,3,2,1],
+        [3,4,2,1],
+        [4,3,1,1],
+
+        [5,8,9,2],
+        [6,9,8,2],
+        [5,9,9,2],
+        [5,9,9,2],
 
-    [4,3,1,1]
     ]
 
     l=np.array(l)
     X=l[:,:-1]
     y=l[:,-1]
     print("X=",X.shape,"y=",y.shape)
     print("Original Data:")
```

### Comparing `knnor-0.1.1/knnor/tests/test_augmented.py` & `knnor-0.1.2/knnor/tests/test_augmented.py`

 * *Files identical despite different names*

### Comparing `knnor-0.1.1/knnor.egg-info/PKG-INFO` & `knnor-0.1.2/knnor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knnor
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generic python library to perform augmentation of multi class data.
 Home-page: 
 Author: Ashhadul Islam, Sameer Brahim Belhaouari, Atiq Ur Rahman, Halima Bensmail
 Author-email: ashhadulislam@gmail.com, samir.brahim@gmail.com, atrehman2@hbku.edu.qa, hbensmail@hbku.edu.qa
 License: MIT
 Keywords: Binary Classification,Data Augmentation,Imabalnced Data,MultiClass Classification
 License-File: LICENSE
```

### Comparing `knnor-0.1.1/setup.py` & `knnor-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
       name='knnor',
-      version='0.1.1',
+      version='0.1.2',
       description='Generic python library to perform augmentation of multi class data.',
       long_description='A generic package to help data scientists balance their dataset by increasing the datapoints for an imbalanced class. Supports multi class'
                   ,
       url='',
       author='Ashhadul Islam, Sameer Brahim Belhaouari, Atiq Ur Rahman, Halima Bensmail',
       author_email='ashhadulislam@gmail.com, samir.brahim@gmail.com, atrehman2@hbku.edu.qa, hbensmail@hbku.edu.qa',
       keywords='Binary Classification, Data Augmentation, Imabalnced Data, MultiClass Classification',
```

