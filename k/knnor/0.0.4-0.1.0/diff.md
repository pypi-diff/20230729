# Comparing `tmp/knnor-0.0.4.tar.gz` & `tmp/knnor-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/knnor-0.0.4.tar", last modified: Sun Feb 20 23:43:43 2022, max compression
+gzip compressed data, was "dist/knnor-0.1.0.tar", last modified: Sat Jul 29 13:13:32 2023, max compression
```

## Comparing `knnor-0.0.4.tar` & `knnor-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2022-02-20 23:43:43.000000 knnor-0.0.4/
--rw-r--r--   0 ashhadulislam   (503) staff       (20)     1063 2022-02-20 23:39:57.000000 knnor-0.0.4/LICENSE
--rw-r--r--   0 ashhadulislam   (503) staff       (20)       38 2022-02-20 23:39:57.000000 knnor-0.0.4/MANIFEST.in
--rw-r--r--   0 ashhadulislam   (503) staff       (20)      561 2022-02-20 23:43:43.000000 knnor-0.0.4/PKG-INFO
--rw-r--r--   0 ashhadulislam   (503) staff       (20)     5095 2022-02-20 23:39:57.000000 knnor-0.0.4/README.md
-drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2022-02-20 23:43:43.000000 knnor-0.0.4/knnor/
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        0 2022-02-20 23:39:57.000000 knnor-0.0.4/knnor/__init__.py
--rw-r--r--   0 ashhadulislam   (503) staff       (20)    16348 2022-02-20 23:40:47.000000 knnor-0.0.4/knnor/data_augment.py
-drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2022-02-20 23:43:43.000000 knnor-0.0.4/knnor/tests/
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        0 2022-02-20 23:39:57.000000 knnor-0.0.4/knnor/tests/__init__.py
--rw-r--r--   0 ashhadulislam   (503) staff       (20)      813 2022-02-20 23:39:57.000000 knnor-0.0.4/knnor/tests/test_augmented.py
-drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2022-02-20 23:43:43.000000 knnor-0.0.4/knnor.egg-info/
--rw-r--r--   0 ashhadulislam   (503) staff       (20)      561 2022-02-20 23:43:43.000000 knnor-0.0.4/knnor.egg-info/PKG-INFO
--rw-r--r--   0 ashhadulislam   (503) staff       (20)      304 2022-02-20 23:43:43.000000 knnor-0.0.4/knnor.egg-info/SOURCES.txt
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        1 2022-02-20 23:43:43.000000 knnor-0.0.4/knnor.egg-info/dependency_links.txt
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        1 2022-02-20 23:43:43.000000 knnor-0.0.4/knnor.egg-info/not-zip-safe
--rw-r--r--   0 ashhadulislam   (503) staff       (20)       19 2022-02-20 23:43:43.000000 knnor-0.0.4/knnor.egg-info/requires.txt
--rw-r--r--   0 ashhadulislam   (503) staff       (20)        6 2022-02-20 23:43:43.000000 knnor-0.0.4/knnor.egg-info/top_level.txt
--rw-r--r--   0 ashhadulislam   (503) staff       (20)       38 2022-02-20 23:43:43.000000 knnor-0.0.4/setup.cfg
--rw-r--r--   0 ashhadulislam   (503) staff       (20)      980 2022-02-20 23:41:06.000000 knnor-0.0.4/setup.py
+drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:13:32.000000 knnor-0.1.0/
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)       38 2023-07-29 12:58:11.000000 knnor-0.1.0/MANIFEST.in
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)      610 2023-07-29 13:13:32.000000 knnor-0.1.0/PKG-INFO
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)     5095 2023-07-29 12:58:11.000000 knnor-0.1.0/README.md
+drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:13:32.000000 knnor-0.1.0/knnor/
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 12:58:11.000000 knnor-0.1.0/knnor/__init__.py
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)    20640 2023-07-29 13:02:07.000000 knnor-0.1.0/knnor/data_augment.py
+drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:13:32.000000 knnor-0.1.0/knnor/tests/
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 12:58:11.000000 knnor-0.1.0/knnor/tests/__init__.py
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)      813 2023-07-29 12:58:11.000000 knnor-0.1.0/knnor/tests/test_augmented.py
+drwxr-xr-x   0 ashhadulislam   (503) staff       (20)        0 2023-07-29 13:13:32.000000 knnor-0.1.0/knnor.egg-info/
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)      610 2023-07-29 13:13:32.000000 knnor-0.1.0/knnor.egg-info/PKG-INFO
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)      296 2023-07-29 13:13:32.000000 knnor-0.1.0/knnor.egg-info/SOURCES.txt
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        1 2023-07-29 13:13:32.000000 knnor-0.1.0/knnor.egg-info/dependency_links.txt
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        1 2023-07-29 13:13:32.000000 knnor-0.1.0/knnor.egg-info/not-zip-safe
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)       19 2023-07-29 13:13:32.000000 knnor-0.1.0/knnor.egg-info/requires.txt
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)        6 2023-07-29 13:13:32.000000 knnor-0.1.0/knnor.egg-info/top_level.txt
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)       38 2023-07-29 13:13:32.000000 knnor-0.1.0/setup.cfg
+-rw-r--r--   0 ashhadulislam   (503) staff       (20)     1041 2023-07-29 13:11:57.000000 knnor-0.1.0/setup.py
```

### Comparing `knnor-0.0.4/PKG-INFO` & `knnor-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.0
 Name: knnor
-Version: 0.0.4
-Summary: Generic python library to perform augmentation of data
+Version: 0.1.0
+Summary: Generic python library to perform augmentation of multi class data.
 Home-page: UNKNOWN
 Author: Ashhadul Islam, Sameer Brahim Belhaouari, Atiq Ur Rahman, Halima Bensmail
 Author-email: ashhadulislam@gmail.com, samir.brahim@gmail.com, atrehman2@hbku.edu.qa, hbensmail@hbku.edu.qa
 License: MIT
-Keywords: Binary Classification,Data Augmentation,Imabalnced Data
+Description: A generic package to help data scientists balance their dataset by increasing the datapoints for an imbalanced class. Supports multi class
+Keywords: Binary Classification,Data Augmentation,Imabalnced Data,MultiClass Classification
 Platform: UNKNOWN
-License-File: LICENSE
-
-A generic package to help data scientists balance their dataset by increasing the datapoints for an imbalanced class.
-
```

### Comparing `knnor-0.0.4/README.md` & `knnor-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `knnor-0.0.4/knnor/data_augment.py` & `knnor-0.1.0/knnor/data_augment.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,152 +1,267 @@
 import numpy as np
 import random
 # from imblearn.over_sampling import SMOTE 
-
+from collections import Counter
 # following libraries for classification test
 # import test_nn
 
 import math
 
 
 class KNNOR:
 
 
-    # def knnor_over_sample(X,y,n_to_sample,num_neighbors,proportion,max_dist_point,intra=True):
-    def fit_resample(self,X,y,**params):
-        threshold_cannot_use=10
-
-        # check for number of neighbors
-        if 'num_neighbors' in params.keys():
-            num_neighbors=params['num_neighbors']
-        else:
-            good_neighbor_count=self.good_count_neighbors(X,y)
-            if good_neighbor_count<=1:
-                print("Too few neighbors")
-                return X,y
-            num_neighbors=random.randrange(1,good_neighbor_count)
 
+#     def fit_resample(self,X,y,**params):
+#         threshold_cannot_use=10
 
-        if 'max_dist_point' in params.keys():
-            max_dist_point=params['max_dist_point']
-        else:
-            max_dist_point=self.max_threshold_dist(X,y,num_neighbors)
+#         # check for number of neighbors
+#         if 'num_neighbors' in params.keys():
+#             num_neighbors=params['num_neighbors']
+#         else:
+#             good_neighbor_count=self.good_count_neighbors(X,y)
+#             if good_neighbor_count<=1:
+#                 print("Too few neighbors")
+#                 return X,y
+#             num_neighbors=random.randrange(1,good_neighbor_count)
+
+
+#         if 'max_dist_point' in params.keys():
+#             max_dist_point=params['max_dist_point']
+#         else:
+#             max_dist_point=self.max_threshold_dist(X,y,num_neighbors)
+
+#         if 'proportion_minority' in params.keys():
+#             '''
+#             proportion of minority population to use
+#             '''
+#             proportion_minority=params['proportion_minority']
+#             inter=False
+#         else:
+#             proportion_intra=self.calculate_distance_threshold(X,y,num_neighbors,intra=False)
+#             proportion_minority=proportion_intra
+#             inter=True
 
-        if 'proportion_minority' in params.keys():
-            '''
-            proportion of minority population to use
-            '''
-            proportion_minority=params['proportion_minority']
-            inter=False
-        else:
-            proportion_intra=self.calculate_distance_threshold(X,y,num_neighbors,intra=False)
-            proportion_minority=proportion_intra
-            inter=True
 
 
+#         if not self.check_enough_minorities(X,y,num_neighbors):
+#             print("Too few minorities")
+#             return X,y
+
+#         if 'final_proportion' in params.keys():
+#             '''
+#             final minority pop = what percentage of majority pop
+#             '''
+#             final_proportion=params['final_proportion']
+            
+#         else:
+#             final_proportion=1
+
 
-        if not self.check_enough_minorities(X,y,num_neighbors):
-            print("Too few minorities")
-            return X,y
+#         n_to_sample=self.calculate_count_to_add(X,y,final_proportion)
 
-        if 'final_proportion' in params.keys():
-            '''
-            final minority pop = what percentage of majority pop
-            '''
-            final_proportion=params['final_proportion']
+#         original_n_neighbors=num_neighbors
+#         original_max_dist_point=max_dist_point    
+#         original_proportion=proportion_minority
+        
+#         minority_label,minority_indices=self.get_minority_label_index(X,y)
+#         X_minority=X[minority_indices]
+#         y_minority=y[minority_indices]
+#         majority_indices=[]
+#         for i in range(0,y.shape[0]):
+#             if i not in minority_indices:
+#                 majority_indices.append(i)
+#         print(len(majority_indices),len(minority_indices),y.shape)
+#         X_majority=X[majority_indices]
+#         y_majority=y[majority_indices]
+        
+#         if not inter:
+#             internal_distance = np.linalg.norm(X_minority - X_minority[:,None], axis = -1)
+#             internal_distance = np.sort(internal_distance)
+#             knd=internal_distance[:,num_neighbors]        
+#             knd_sorted = np.sort(knd)        
+#         else:
+#             external_distance=np.linalg.norm(X_majority - X_minority[:,None], axis = -1)
+#             external_distance = np.sort(external_distance)
+#             knd=external_distance[:,num_neighbors]   
+#             knd_sorted=-np.sort(-knd)
             
-        else:
-            final_proportion=1
+#         threshold_dist = knd_sorted[math.floor(proportion_minority*len(knd_sorted))]
+            
+#         X_new_minority=[]
+#         N = n_to_sample
+#         consecutive_cannot_use=0
+#         while N>0:
+#             for i in range(X_minority.shape[0]):
+#                 if inter:
+#                     if knd[i]>threshold_dist:
+#                         continue
+#                 else:
+#                     if knd[i]<threshold_dist:
+#                         continue
+#                 if N==0:
+#                     break
+#                 v = X_minority[i,:]
+#                 val=np.sort( abs((X_minority-v)*(X_minority-v)).sum(axis=1) )
+#                 # sort neighbors by distance
+#                 # obviously will have to ignore the 
+#                 # first term as its a distance to iteself
+#                 # which wil be 0
+#                 posit=np.argsort(abs((X_minority-v)*(X_minority-v)).sum(axis=1))
+#                 kv = X_minority[posit[1:num_neighbors+1],:]
+#                 alphak = random.uniform(0,max_dist_point)
+#                 m0 = v
+#                 for j in range(num_neighbors):
+#                     m1 = m0 + alphak * (kv[j,:] - m0)
+#                     m0 = m1
+#                 num_neighbors_to_test=math.floor(math.sqrt(num_neighbors))
+#                 can_use=self.predict_classification(X,y,m0, num_neighbors_to_test,minority_label)
+#                 can_use=can_use and not(self.check_duplicates(m0,X_minority))
+#                 can_use=can_use and not(self.check_duplicates(m0,X_new_minority))                            
+#                 if can_use:
+#                     consecutive_cannot_use=0
+#                     num_neighbors=min(num_neighbors+1,original_n_neighbors)
+#                     max_dist_point=min(max_dist_point+0.01,original_max_dist_point)
+#                     proportion_minority=max(proportion_minority-0.01,original_proportion)
+#                     threshold_dist = knd_sorted[math.floor(proportion_minority*len(knd_sorted))]                
+#                     X_new_minority.append(m0)
+#                     N-=1
+#                 else:
+#                     consecutive_cannot_use+=1
+#                     if consecutive_cannot_use>=threshold_cannot_use:
+#                         num_neighbors=max(num_neighbors-1,2)
+#                         max_dist_point=max(max_dist_point-0.01,0.01)
+#                         proportion_minority=min(proportion_minority+0.01,0.9)
+#                         threshold_dist = knd_sorted[math.floor(proportion_minority*len(knd_sorted))]
+#                         consecutive_cannot_use=0
+
+#         y_new_minority=[minority_label for i in range(len(X_new_minority))]        
+#         X_new_minority=np.array(X_new_minority)
+#         X_new_all=np.concatenate((X, X_new_minority), axis=0)
+#         y_new_all=np.concatenate((y, y_new_minority), axis=0)
+        
+#         return X_new_all, y_new_all, X_new_minority, y_new_minority
+
+
+
+    def fit_resample(self,X,y,num_nbrs=3, prop_minority=0.5, max_dist=0.5, proportion=1):
+        
+        
+        print("SHape of y",y.shape)
+        print("Count",Counter(y))
+
+
+        # get the minority count
+        max_count=max(list(Counter(y).values()))
+        print("max is ",max_count)
+
+        minority_labels=[]
+        majority_label=-1
+        for k,val in Counter(y).items():
+            if val !=max_count:
+                minority_labels.append(k)
+            else:
+                majority_label=k
+        all_labels=list(Counter(y).keys())
+        print(minority_labels,majority_label,all_labels)       
+
+
+
+
+        X_all_new_minorities=[]
+        y_all_new_minorities=[]
+        for minority_label in minority_labels:
+
+            print("Minority label",minority_label)
+
+            other_labels=list(set(all_labels)-set([minority_label]))
+            print(minority_label,other_labels)
+            X_maj=[]
+            for i in range(X.shape[0]):
+                if y[i] in other_labels:
+                    X_maj.append(X[i])
+
+            X_maj=np.array(X_maj)
+            X_min=X[y==minority_label]
+            print(X_maj.shape,X_min.shape,X.shape)
+            # count to add
+            N=self.count_to_add(X_min,max_count,proportion)
+            print("Count to add ",N)
 
 
-        n_to_sample=self.calculate_count_to_add(X,y,final_proportion)
+            internal_distance = np.linalg.norm(X_min - X_min[:,None], axis = -1)
+            internal_distance = np.sort(internal_distance)    
 
-        original_n_neighbors=num_neighbors
-        original_max_dist_point=max_dist_point    
-        original_proportion=proportion_minority
-        
-        minority_label,minority_indices=self.get_minority_label_index(X,y)
-        X_minority=X[minority_indices]
-        y_minority=y[minority_indices]
-        majority_indices=[]
-        for i in range(0,y.shape[0]):
-            if i not in minority_indices:
-                majority_indices.append(i)
-        print(len(majority_indices),len(minority_indices),y.shape)
-        X_majority=X[majority_indices]
-        y_majority=y[majority_indices]
-        
-        if not inter:
-            internal_distance = np.linalg.norm(X_minority - X_minority[:,None], axis = -1)
-            internal_distance = np.sort(internal_distance)
-            knd=internal_distance[:,num_neighbors]        
+            knd=internal_distance[:,num_nbrs] 
             knd_sorted = np.sort(knd)        
-        else:
-            external_distance=np.linalg.norm(X_majority - X_minority[:,None], axis = -1)
-            external_distance = np.sort(external_distance)
-            knd=external_distance[:,num_neighbors]   
-            knd_sorted=-np.sort(-knd)
-            
-        threshold_dist = knd_sorted[math.floor(proportion_minority*len(knd_sorted))]
-            
-        X_new_minority=[]
-        N = n_to_sample
-        consecutive_cannot_use=0
-        while N>0:
-            for i in range(X_minority.shape[0]):
-                if inter:
+            threshold_dist = knd_sorted[math.floor(prop_minority*len(knd_sorted))]
+
+            print("Threshold distance is ",threshold_dist)    
+
+
+
+
+
+
+            threshold_cannot_use=10
+            original_n_neighbors=num_nbrs
+            original_max_dist_point=max_dist
+            original_proportion=prop_minority    
+
+            consecutive_cannot_use=0
+            X_new_minority=[]
+            while N>0:
+                for i in range(X_min.shape[0]):
                     if knd[i]>threshold_dist:
-                        continue
-                else:
-                    if knd[i]<threshold_dist:
-                        continue
-                if N==0:
-                    break
-                v = X_minority[i,:]
-                val=np.sort( abs((X_minority-v)*(X_minority-v)).sum(axis=1) )
-                # sort neighbors by distance
-                # obviously will have to ignore the 
-                # first term as its a distance to iteself
-                # which wil be 0
-                posit=np.argsort(abs((X_minority-v)*(X_minority-v)).sum(axis=1))
-                kv = X_minority[posit[1:num_neighbors+1],:]
-                alphak = random.uniform(0,max_dist_point)
-                m0 = v
-                for j in range(num_neighbors):
-                    m1 = m0 + alphak * (kv[j,:] - m0)
-                    m0 = m1
-                num_neighbors_to_test=math.floor(math.sqrt(num_neighbors))
-                can_use=self.predict_classification(X,y,m0, num_neighbors_to_test,minority_label)
-                can_use=can_use and not(self.check_duplicates(m0,X_minority))
-                can_use=can_use and not(self.check_duplicates(m0,X_new_minority))                            
-                if can_use:
-                    consecutive_cannot_use=0
-                    num_neighbors=min(num_neighbors+1,original_n_neighbors)
-                    max_dist_point=min(max_dist_point+0.01,original_max_dist_point)
-                    proportion_minority=max(proportion_minority-0.01,original_proportion)
-                    threshold_dist = knd_sorted[math.floor(proportion_minority*len(knd_sorted))]                
+                        continue        
+                    if N==0:
+                        break
+
+                    # get the start point
+                    v = X_min[i,:]
+                    # distance to all points of minority class
+        #             val=np.sort( abs((X_min-v)*(X_min-v)).sum(axis=1) )            
+                    posit=np.argsort(abs((X_min-v)*(X_min-v)).sum(axis=1))
+                    kv = X_min[posit[1:num_nbrs+1],:]
+                    alphak = random.uniform(0,max_dist)      
+
+                    m0 = v
+                    print("Origin point",m0)
+                    # iterate for n_nbrs
+                    for j in range(num_nbrs):
+                        print("Nbr",kv[j,:])
+                        m1 = m0 + alphak * (kv[j,:] - m0)
+                        m0 = m1
+                        print("New point",m0)
+
+        #             can_use=True
+                    # blind usage
                     X_new_minority.append(m0)
                     N-=1
-                else:
-                    consecutive_cannot_use+=1
-                    if consecutive_cannot_use>=threshold_cannot_use:
-                        num_neighbors=max(num_neighbors-1,2)
-                        max_dist_point=max(max_dist_point-0.01,0.01)
-                        proportion_minority=min(proportion_minority+0.01,0.9)
-                        threshold_dist = knd_sorted[math.floor(proportion_minority*len(knd_sorted))]
-                        consecutive_cannot_use=0
-
-        y_new_minority=[minority_label for i in range(len(X_new_minority))]        
-        X_new_minority=np.array(X_new_minority)
-        X_new_all=np.concatenate((X, X_new_minority), axis=0)
-        y_new_all=np.concatenate((y, y_new_minority), axis=0)
-        
-        return X_new_all, y_new_all, X_new_minority, y_new_minority
+                    if N==0:
+                        break
 
 
+            X_new_minority=np.array(X_new_minority)
+    #         print(X_new_minority.shape,"created")
+    #         print("*"*10)
+            y_new_minority=[minority_label for i in range(X_new_minority.shape[0])]    
+            X_all_new_minorities.append(X_new_minority)
+            y_all_new_minorities.append(y_new_minority)
+
+        X_all_new_minorities=np.concatenate(X_all_new_minorities)
+        y_all_new_minorities=np.concatenate(y_all_new_minorities)
+
+    #     print(X_all_new_minorities.shape,y_all_new_minorities.shape)
+        print(X.shape,X_all_new_minorities.shape)
+
+        X_resampled=np.concatenate([X,X_all_new_minorities])
+        y_resampled=np.concatenate([y,y_all_new_minorities])
+        return X_resampled,y_resampled,X_all_new_minorities,y_all_new_minorities
 
 
 
 
     def predict_classification(self,X,y,new_vector, num_neighbors_to_test,expected_class_index):
         '''
         this function is used to validate
@@ -236,16 +351,16 @@
     # https://stackoverflow.com/questions/20618804/how-to-smooth-a-curve-in-the-right-way
 
     def savitzky_golay(self,y, window_size, order, deriv=0, rate=1):         
         import numpy as np
         from math import factorial
         
         try:
-            window_size = np.abs(np.int(window_size))
-            order = np.abs(np.int(order))
+            window_size = np.abs(int(window_size))
+            order = np.abs(int(order))
         except ValueError:
             raise ValueError("window_size and order have to be of type int")
         if window_size % 2 != 1 or window_size < 1:
             raise TypeError("window_size size must be a positive odd number")
         if window_size < order + 2:
             raise TypeError("window_size is too small for the polynomials order")
         order_range = range(order+1)
@@ -373,31 +488,37 @@
         '''
         minority_label,minority_indices=self.get_minority_label_index(X,y)
         if len(minority_indices)<=num_neighbors:
             print("You want to use ",num_neighbors,"neighbors, but minority data size = ",len(minority_indices))
             return False
         return True
 
-
-    def calculate_count_to_add(self,X,y,final_proportion):
-        '''
-        Calculate the number of artificial points to be generated so that
-        (count_minority_existing+count_artificial_minority)/count_majority_existing=final_proportion
-        '''
-        minority_label,minority_indices=self.get_minority_label_index(X,y)
-        majority_indices=[]
-        for i in range(0,y.shape[0]):
-            if i not in minority_indices:
-                majority_indices.append(i)
-        count_minority=len(minority_indices)
-        count_majority=len(majority_indices)
-        new_minority=int((final_proportion*count_majority)-count_minority)
-        if new_minority<1:
-            return -1
-        return new_minority
+    def count_to_add(self,X_min,max_count,proportion):
+        N1=max_count
+        N2=X_min.shape[0]
+    #     print("maj count",N1,"min count",N2)
+        count_to_add = int(N1*proportion)-N2
+        return count_to_add
+
+#     def calculate_count_to_add(self,X,y,final_proportion):
+#         '''
+#         Calculate the number of artificial points to be generated so that
+#         (count_minority_existing+count_artificial_minority)/count_majority_existing=final_proportion
+#         '''
+#         minority_label,minority_indices=self.get_minority_label_index(X,y)
+#         majority_indices=[]
+#         for i in range(0,y.shape[0]):
+#             if i not in minority_indices:
+#                 majority_indices.append(i)
+#         count_minority=len(minority_indices)
+#         count_majority=len(majority_indices)
+#         new_minority=int((final_proportion*count_majority)-count_minority)
+#         if new_minority<1:
+#             return -1
+#         return new_minority
 
 
 
 
 
 
 
@@ -406,18 +527,18 @@
 # below code is used to test the code
 def main():
     '''
     x^2 + y^2 + z^2 < 15 => 0
     x^2 + y^2 + z^2 >= 15 => 1
     '''
     l=[
-    
+
     [1.0,2.0,1.0,0],
     [1,3,1,0],
-    [2,1,1,0],
+    [2,1,2,0],
     [3,2,1,0],
     [3,1,1,0],
 
     [1,3,4,1],
     [1,4,3,1],
     [1,4,4,1],
 
@@ -438,25 +559,22 @@
     X=l[:,:-1]
     y=l[:,-1]
     print("X=",X.shape,"y=",y.shape)
     print("Original Data:")
     print(l)
     print("************************************")
 
-    
+
     knnor=KNNOR()
     X_new,y_new,_,_=knnor.fit_resample(X,y)
     y_new=y_new.reshape(-1,1)
     print(X_new.shape,y_new.shape)
 
     print("KNNOR Data:")
     new_data=np.append(X_new, y_new, axis=1)
     print(new_data)
     print("************************************")
 
-    
-
-
-
 
 if __name__=="__main__":
     main()
+
```

### Comparing `knnor-0.0.4/knnor/tests/test_augmented.py` & `knnor-0.1.0/knnor/tests/test_augmented.py`

 * *Files identical despite different names*

### Comparing `knnor-0.0.4/knnor.egg-info/PKG-INFO` & `knnor-0.1.0/knnor.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.0
 Name: knnor
-Version: 0.0.4
-Summary: Generic python library to perform augmentation of data
+Version: 0.1.0
+Summary: Generic python library to perform augmentation of multi class data.
 Home-page: UNKNOWN
 Author: Ashhadul Islam, Sameer Brahim Belhaouari, Atiq Ur Rahman, Halima Bensmail
 Author-email: ashhadulislam@gmail.com, samir.brahim@gmail.com, atrehman2@hbku.edu.qa, hbensmail@hbku.edu.qa
 License: MIT
-Keywords: Binary Classification,Data Augmentation,Imabalnced Data
+Description: A generic package to help data scientists balance their dataset by increasing the datapoints for an imbalanced class. Supports multi class
+Keywords: Binary Classification,Data Augmentation,Imabalnced Data,MultiClass Classification
 Platform: UNKNOWN
-License-File: LICENSE
-
-A generic package to help data scientists balance their dataset by increasing the datapoints for an imbalanced class.
-
```

### Comparing `knnor-0.0.4/setup.py` & `knnor-0.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
       name='knnor',
-      version='0.0.4',
-      description='Generic python library to perform augmentation of data',
-      long_description='A generic package to help data scientists balance their dataset by increasing the datapoints for an imbalanced class.'
+      version='0.1.0',
+      description='Generic python library to perform augmentation of multi class data.',
+      long_description='A generic package to help data scientists balance their dataset by increasing the datapoints for an imbalanced class. Supports multi class'
                   ,
       url='',
       author='Ashhadul Islam, Sameer Brahim Belhaouari, Atiq Ur Rahman, Halima Bensmail',
       author_email='ashhadulislam@gmail.com, samir.brahim@gmail.com, atrehman2@hbku.edu.qa, hbensmail@hbku.edu.qa',
-      keywords='Binary Classification, Data Augmentation, Imabalnced Data',
+      keywords='Binary Classification, Data Augmentation, Imabalnced Data, MultiClass Classification',
       license='MIT',
       packages=setuptools.find_packages(),
       install_requires=[            
             "numpy",
             "scikit-learn"
       ],
       test_suite='nose.collector',
```

