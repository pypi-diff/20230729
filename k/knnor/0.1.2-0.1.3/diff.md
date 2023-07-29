# Comparing `tmp/knnor-0.1.2.tar.gz` & `tmp/knnor-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knnor-0.1.2.tar", last modified: Sat Jul 29 13:53:32 2023, max compression
+gzip compressed data, was "knnor-0.1.3.tar", last modified: Sat Jul 29 13:59:39 2023, max compression
```

## Comparing `knnor-0.1.2.tar` & `knnor-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:53:32.852693 knnor-0.1.2/
--rw-r--r--   0 ashhadulislam   (503) staff       (20)     1063 2023-07-29 12:58:11.000000 knnor-0.1.2/LICENSE
--rw-r--r--   0 ashhadulislam   (503) staff       (20)       38 2023-07-29 12:58:11.000000 knnor-0.1.2/MANIFEST.in
--rw-r--r--   0 ashhadulislam   (503) staff       (20)      595 2023-07-29 13:53:32.852299 knnor-0.1.2/PKG-INFO
--rw-r--r--   0 ashhadulislam   (503) staff       (20)     5095 2023-07-29 12:58:11.000000 knnor-0.1.2/README.md
-drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:53:32.849708 knnor-0.1.2/knnor/
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 12:58:11.000000 knnor-0.1.2/knnor/__init__.py
--rw-r--r--   0 ashhadulislam   (503) staff       (20)    20806 2023-07-29 13:53:06.000000 knnor-0.1.2/knnor/data_augment.py
-drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:53:32.851838 knnor-0.1.2/knnor/tests/
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 12:58:11.000000 knnor-0.1.2/knnor/tests/__init__.py
--rw-r--r--   0 ashhadulislam   (503) staff       (20)      813 2023-07-29 12:58:11.000000 knnor-0.1.2/knnor/tests/test_augmented.py
-drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:53:32.851331 knnor-0.1.2/knnor.egg-info/
--rw-r--r--   0 ashhadulislam   (503) staff       (20)      595 2023-07-29 13:53:32.000000 knnor-0.1.2/knnor.egg-info/PKG-INFO
--rw-r--r--   0 ashhadulislam   (503) staff       (20)      304 2023-07-29 13:53:32.000000 knnor-0.1.2/knnor.egg-info/SOURCES.txt
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        1 2023-07-29 13:53:32.000000 knnor-0.1.2/knnor.egg-info/dependency_links.txt
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        1 2023-07-29 13:13:32.000000 knnor-0.1.2/knnor.egg-info/not-zip-safe
--rw-r--r--   0 ashhadulislam   (503) staff       (20)       19 2023-07-29 13:53:32.000000 knnor-0.1.2/knnor.egg-info/requires.txt
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        6 2023-07-29 13:53:32.000000 knnor-0.1.2/knnor.egg-info/top_level.txt
--rw-r--r--   0 ashhadulislam   (503) staff       (20)       38 2023-07-29 13:53:32.852796 knnor-0.1.2/setup.cfg
--rw-r--r--   0 ashhadulislam   (503) staff       (20)     1041 2023-07-29 13:53:19.000000 knnor-0.1.2/setup.py
+drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:59:39.746003 knnor-0.1.3/
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)     1063 2023-07-29 12:58:11.000000 knnor-0.1.3/LICENSE
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)       38 2023-07-29 12:58:11.000000 knnor-0.1.3/MANIFEST.in
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)      595 2023-07-29 13:59:39.745613 knnor-0.1.3/PKG-INFO
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)     5095 2023-07-29 12:58:11.000000 knnor-0.1.3/README.md
+drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:59:39.742529 knnor-0.1.3/knnor/
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 12:58:11.000000 knnor-0.1.3/knnor/__init__.py
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)    20808 2023-07-29 13:59:18.000000 knnor-0.1.3/knnor/data_augment.py
+drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:59:39.745121 knnor-0.1.3/knnor/tests/
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 12:58:11.000000 knnor-0.1.3/knnor/tests/__init__.py
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)      813 2023-07-29 12:58:11.000000 knnor-0.1.3/knnor/tests/test_augmented.py
+drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:59:39.744477 knnor-0.1.3/knnor.egg-info/
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)      595 2023-07-29 13:59:39.000000 knnor-0.1.3/knnor.egg-info/PKG-INFO
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)      304 2023-07-29 13:59:39.000000 knnor-0.1.3/knnor.egg-info/SOURCES.txt
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        1 2023-07-29 13:59:39.000000 knnor-0.1.3/knnor.egg-info/dependency_links.txt
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        1 2023-07-29 13:13:32.000000 knnor-0.1.3/knnor.egg-info/not-zip-safe
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)       19 2023-07-29 13:59:39.000000 knnor-0.1.3/knnor.egg-info/requires.txt
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        6 2023-07-29 13:59:39.000000 knnor-0.1.3/knnor.egg-info/top_level.txt
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)       38 2023-07-29 13:59:39.746184 knnor-0.1.3/setup.cfg
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)     1041 2023-07-29 13:59:33.000000 knnor-0.1.3/setup.py
```

### Comparing `knnor-0.1.2/LICENSE` & `knnor-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `knnor-0.1.2/PKG-INFO` & `knnor-0.1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knnor
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generic python library to perform augmentation of multi class data.
 Home-page: 
 Author: Ashhadul Islam, Sameer Brahim Belhaouari, Atiq Ur Rahman, Halima Bensmail
 Author-email: ashhadulislam@gmail.com, samir.brahim@gmail.com, atrehman2@hbku.edu.qa, hbensmail@hbku.edu.qa
 License: MIT
 Keywords: Binary Classification,Data Augmentation,Imabalnced Data,MultiClass Classification
 License-File: LICENSE
```

### Comparing `knnor-0.1.2/README.md` & `knnor-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `knnor-0.1.2/knnor/data_augment.py` & `knnor-0.1.3/knnor/data_augment.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         majority_label=-1
         for k,val in Counter(y).items():
             if val !=max_count:
                 minority_labels.append(k)
             else:
                 majority_label=k
         all_labels=list(Counter(y).keys())
-        print(minority_labels,majority_label,all_labels)       
+#         print(minority_labels,majority_label,all_labels)       
 
 
 
 
         X_all_new_minorities=[]
         y_all_new_minorities=[]
         for minority_label in minority_labels:
```

### Comparing `knnor-0.1.2/knnor/tests/test_augmented.py` & `knnor-0.1.3/knnor/tests/test_augmented.py`

 * *Files identical despite different names*

### Comparing `knnor-0.1.2/knnor.egg-info/PKG-INFO` & `knnor-0.1.3/knnor.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knnor
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generic python library to perform augmentation of multi class data.
 Home-page: 
 Author: Ashhadul Islam, Sameer Brahim Belhaouari, Atiq Ur Rahman, Halima Bensmail
 Author-email: ashhadulislam@gmail.com, samir.brahim@gmail.com, atrehman2@hbku.edu.qa, hbensmail@hbku.edu.qa
 License: MIT
 Keywords: Binary Classification,Data Augmentation,Imabalnced Data,MultiClass Classification
 License-File: LICENSE
```

### Comparing `knnor-0.1.2/setup.py` & `knnor-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
       name='knnor',
-      version='0.1.2',
+      version='0.1.3',
       description='Generic python library to perform augmentation of multi class data.',
       long_description='A generic package to help data scientists balance their dataset by increasing the datapoints for an imbalanced class. Supports multi class'
                   ,
       url='',
       author='Ashhadul Islam, Sameer Brahim Belhaouari, Atiq Ur Rahman, Halima Bensmail',
       author_email='ashhadulislam@gmail.com, samir.brahim@gmail.com, atrehman2@hbku.edu.qa, hbensmail@hbku.edu.qa',
       keywords='Binary Classification, Data Augmentation, Imabalnced Data, MultiClass Classification',
```

