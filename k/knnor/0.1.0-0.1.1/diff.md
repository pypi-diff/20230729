# Comparing `tmp/knnor-0.1.0.tar.gz` & `tmp/knnor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/knnor-0.1.0.tar", last modified: Sat Jul 29 13:13:32 2023, max compression
+gzip compressed data, was "knnor-0.1.1.tar", last modified: Sat Jul 29 13:19:22 2023, max compression
```

## Comparing `knnor-0.1.0.tar` & `knnor-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:13:32.000000 knnor-0.1.0/
--rw-r--r--   0 ashhadulislam   (503) staff       (20)       38 2023-07-29 12:58:11.000000 knnor-0.1.0/MANIFEST.in
--rw-r--r--   0 ashhadulislam   (503) staff       (20)      610 2023-07-29 13:13:32.000000 knnor-0.1.0/PKG-INFO
--rw-r--r--   0 ashhadulislam   (503) staff       (20)     5095 2023-07-29 12:58:11.000000 knnor-0.1.0/README.md
-drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:13:32.000000 knnor-0.1.0/knnor/
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 12:58:11.000000 knnor-0.1.0/knnor/__init__.py
--rw-r--r--   0 ashhadulislam   (503) staff       (20)    20640 2023-07-29 13:02:07.000000 knnor-0.1.0/knnor/data_augment.py
-drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:13:32.000000 knnor-0.1.0/knnor/tests/
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 12:58:11.000000 knnor-0.1.0/knnor/tests/__init__.py
--rw-r--r--   0 ashhadulislam   (503) staff       (20)      813 2023-07-29 12:58:11.000000 knnor-0.1.0/knnor/tests/test_augmented.py
-drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:13:32.000000 knnor-0.1.0/knnor.egg-info/
--rw-r--r--   0 ashhadulislam   (503) staff       (20)      610 2023-07-29 13:13:32.000000 knnor-0.1.0/knnor.egg-info/PKG-INFO
--rw-r--r--   0 ashhadulislam   (503) staff       (20)      296 2023-07-29 13:13:32.000000 knnor-0.1.0/knnor.egg-info/SOURCES.txt
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        1 2023-07-29 13:13:32.000000 knnor-0.1.0/knnor.egg-info/dependency_links.txt
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        1 2023-07-29 13:13:32.000000 knnor-0.1.0/knnor.egg-info/not-zip-safe
--rw-r--r--   0 ashhadulislam   (503) staff       (20)       19 2023-07-29 13:13:32.000000 knnor-0.1.0/knnor.egg-info/requires.txt
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        6 2023-07-29 13:13:32.000000 knnor-0.1.0/knnor.egg-info/top_level.txt
--rw-r--r--   0 ashhadulislam   (503) staff       (20)       38 2023-07-29 13:13:32.000000 knnor-0.1.0/setup.cfg
--rw-r--r--   0 ashhadulislam   (503) staff       (20)     1041 2023-07-29 13:11:57.000000 knnor-0.1.0/setup.py
+drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:19:22.213071 knnor-0.1.1/
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)     1063 2023-07-29 12:58:11.000000 knnor-0.1.1/LICENSE
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)       38 2023-07-29 12:58:11.000000 knnor-0.1.1/MANIFEST.in
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)      595 2023-07-29 13:19:22.212584 knnor-0.1.1/PKG-INFO
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)     5095 2023-07-29 12:58:11.000000 knnor-0.1.1/README.md
+drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:19:22.209322 knnor-0.1.1/knnor/
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 12:58:11.000000 knnor-0.1.1/knnor/__init__.py
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)    20656 2023-07-29 13:18:41.000000 knnor-0.1.1/knnor/data_augment.py
+drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:19:22.212082 knnor-0.1.1/knnor/tests/
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 12:58:11.000000 knnor-0.1.1/knnor/tests/__init__.py
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)      813 2023-07-29 12:58:11.000000 knnor-0.1.1/knnor/tests/test_augmented.py
+drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:19:22.211345 knnor-0.1.1/knnor.egg-info/
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)      595 2023-07-29 13:19:22.000000 knnor-0.1.1/knnor.egg-info/PKG-INFO
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)      304 2023-07-29 13:19:22.000000 knnor-0.1.1/knnor.egg-info/SOURCES.txt
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        1 2023-07-29 13:19:22.000000 knnor-0.1.1/knnor.egg-info/dependency_links.txt
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        1 2023-07-29 13:13:32.000000 knnor-0.1.1/knnor.egg-info/not-zip-safe
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)       19 2023-07-29 13:19:22.000000 knnor-0.1.1/knnor.egg-info/requires.txt
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        6 2023-07-29 13:19:22.000000 knnor-0.1.1/knnor.egg-info/top_level.txt
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)       38 2023-07-29 13:19:22.213185 knnor-0.1.1/setup.cfg
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)     1041 2023-07-29 13:19:05.000000 knnor-0.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `knnor-0.1.0/PKG-INFO` & `knnor-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: knnor
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generic python library to perform augmentation of multi class data.
-Home-page: UNKNOWN
+Home-page: 
 Author: Ashhadul Islam, Sameer Brahim Belhaouari, Atiq Ur Rahman, Halima Bensmail
 Author-email: ashhadulislam@gmail.com, samir.brahim@gmail.com, atrehman2@hbku.edu.qa, hbensmail@hbku.edu.qa
 License: MIT
-Description: A generic package to help data scientists balance their dataset by increasing the datapoints for an imbalanced class. Supports multi class
 Keywords: Binary Classification,Data Augmentation,Imabalnced Data,MultiClass Classification
-Platform: UNKNOWN
+License-File: LICENSE
+
+A generic package to help data scientists balance their dataset by increasing the datapoints for an imbalanced class. Supports multi class
```

### Comparing `knnor-0.1.0/README.md` & `knnor-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `knnor-0.1.0/knnor/data_augment.py` & `knnor-0.1.1/knnor/data_augment.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,21 +143,21 @@
 #         return X_new_all, y_new_all, X_new_minority, y_new_minority
 
 
 
     def fit_resample(self,X,y,num_nbrs=3, prop_minority=0.5, max_dist=0.5, proportion=1):
         
         
-        print("SHape of y",y.shape)
-        print("Count",Counter(y))
+#         print("SHape of y",y.shape)
+#         print("Count",Counter(y))
 
 
         # get the minority count
         max_count=max(list(Counter(y).values()))
-        print("max is ",max_count)
+#         print("max is ",max_count)
 
         minority_labels=[]
         majority_label=-1
         for k,val in Counter(y).items():
             if val !=max_count:
                 minority_labels.append(k)
             else:
@@ -182,25 +182,25 @@
                     X_maj.append(X[i])
 
             X_maj=np.array(X_maj)
             X_min=X[y==minority_label]
             print(X_maj.shape,X_min.shape,X.shape)
             # count to add
             N=self.count_to_add(X_min,max_count,proportion)
-            print("Count to add ",N)
+#             print("Count to add ",N)
 
 
             internal_distance = np.linalg.norm(X_min - X_min[:,None], axis = -1)
             internal_distance = np.sort(internal_distance)    
 
             knd=internal_distance[:,num_nbrs] 
             knd_sorted = np.sort(knd)        
             threshold_dist = knd_sorted[math.floor(prop_minority*len(knd_sorted))]
 
-            print("Threshold distance is ",threshold_dist)    
+#             print("Threshold distance is ",threshold_dist)    
 
 
 
 
 
 
             threshold_cannot_use=10
@@ -222,21 +222,21 @@
                     # distance to all points of minority class
         #             val=np.sort( abs((X_min-v)*(X_min-v)).sum(axis=1) )            
                     posit=np.argsort(abs((X_min-v)*(X_min-v)).sum(axis=1))
                     kv = X_min[posit[1:num_nbrs+1],:]
                     alphak = random.uniform(0,max_dist)      
 
                     m0 = v
-                    print("Origin point",m0)
+#                     print("Origin point",m0)
                     # iterate for n_nbrs
                     for j in range(num_nbrs):
-                        print("Nbr",kv[j,:])
+#                         print("Nbr",kv[j,:])
                         m1 = m0 + alphak * (kv[j,:] - m0)
                         m0 = m1
-                        print("New point",m0)
+#                         print("New point",m0)
 
         #             can_use=True
                     # blind usage
                     X_new_minority.append(m0)
                     N-=1
                     if N==0:
                         break
```

### Comparing `knnor-0.1.0/knnor/tests/test_augmented.py` & `knnor-0.1.1/knnor/tests/test_augmented.py`

 * *Files identical despite different names*

### Comparing `knnor-0.1.0/knnor.egg-info/PKG-INFO` & `knnor-0.1.1/knnor.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: knnor
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generic python library to perform augmentation of multi class data.
-Home-page: UNKNOWN
+Home-page: 
 Author: Ashhadul Islam, Sameer Brahim Belhaouari, Atiq Ur Rahman, Halima Bensmail
 Author-email: ashhadulislam@gmail.com, samir.brahim@gmail.com, atrehman2@hbku.edu.qa, hbensmail@hbku.edu.qa
 License: MIT
-Description: A generic package to help data scientists balance their dataset by increasing the datapoints for an imbalanced class. Supports multi class
 Keywords: Binary Classification,Data Augmentation,Imabalnced Data,MultiClass Classification
-Platform: UNKNOWN
+License-File: LICENSE
+
+A generic package to help data scientists balance their dataset by increasing the datapoints for an imbalanced class. Supports multi class
```

### Comparing `knnor-0.1.0/setup.py` & `knnor-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
       name='knnor',
-      version='0.1.0',
+      version='0.1.1',
       description='Generic python library to perform augmentation of multi class data.',
       long_description='A generic package to help data scientists balance their dataset by increasing the datapoints for an imbalanced class. Supports multi class'
                   ,
       url='',
       author='Ashhadul Islam, Sameer Brahim Belhaouari, Atiq Ur Rahman, Halima Bensmail',
       author_email='ashhadulislam@gmail.com, samir.brahim@gmail.com, atrehman2@hbku.edu.qa, hbensmail@hbku.edu.qa',
       keywords='Binary Classification, Data Augmentation, Imabalnced Data, MultiClass Classification',
```

