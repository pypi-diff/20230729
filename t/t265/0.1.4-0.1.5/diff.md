# Comparing `tmp/t265-0.1.4.tar.gz` & `tmp/t265-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t265-0.1.4.tar", last modified: Sat Jul 29 04:52:41 2023, max compression
+gzip compressed data, was "t265-0.1.5.tar", last modified: Sat Jul 29 05:04:33 2023, max compression
```

## Comparing `t265-0.1.4.tar` & `t265-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 yusuke    (1000) yusuke    (1000)        0 2023-07-29 04:52:41.373495 t265-0.1.4/
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       25 2023-07-18 00:54:55.000000 t265-0.1.4/MANIFEST.in
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)      549 2023-07-29 04:52:41.373495 t265-0.1.4/PKG-INFO
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       27 2023-07-18 01:21:38.000000 t265-0.1.4/requirements.txt
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       38 2023-07-29 04:52:41.373495 t265-0.1.4/setup.cfg
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)     1008 2023-07-29 04:50:35.000000 t265-0.1.4/setup.py
-drwxrwxr-x   0 yusuke    (1000) yusuke    (1000)        0 2023-07-29 04:52:41.373495 t265-0.1.4/t265/
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)     3931 2023-07-29 04:42:31.000000 t265-0.1.4/t265/Tracking.py
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       31 2023-07-18 00:54:55.000000 t265-0.1.4/t265/__init__.py
-drwxrwxr-x   0 yusuke    (1000) yusuke    (1000)        0 2023-07-29 04:52:41.373495 t265-0.1.4/t265.egg-info/
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)      549 2023-07-29 04:52:41.000000 t265-0.1.4/t265.egg-info/PKG-INFO
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)      210 2023-07-29 04:52:41.000000 t265-0.1.4/t265.egg-info/SOURCES.txt
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)        1 2023-07-29 04:52:41.000000 t265-0.1.4/t265.egg-info/dependency_links.txt
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       27 2023-07-29 04:52:41.000000 t265-0.1.4/t265.egg-info/requires.txt
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)        5 2023-07-29 04:52:41.000000 t265-0.1.4/t265.egg-info/top_level.txt
+drwxrwxr-x   0 yusuke    (1000) yusuke    (1000)        0 2023-07-29 05:04:33.981544 t265-0.1.5/
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       25 2023-07-18 00:54:55.000000 t265-0.1.5/MANIFEST.in
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)      549 2023-07-29 05:04:33.981544 t265-0.1.5/PKG-INFO
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       27 2023-07-18 01:21:38.000000 t265-0.1.5/requirements.txt
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       38 2023-07-29 05:04:33.985544 t265-0.1.5/setup.cfg
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)     1008 2023-07-29 05:02:30.000000 t265-0.1.5/setup.py
+drwxrwxr-x   0 yusuke    (1000) yusuke    (1000)        0 2023-07-29 05:04:33.981544 t265-0.1.5/t265/
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)     4282 2023-07-29 05:02:42.000000 t265-0.1.5/t265/Tracking.py
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       31 2023-07-18 00:54:55.000000 t265-0.1.5/t265/__init__.py
+drwxrwxr-x   0 yusuke    (1000) yusuke    (1000)        0 2023-07-29 05:04:33.981544 t265-0.1.5/t265.egg-info/
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)      549 2023-07-29 05:04:33.000000 t265-0.1.5/t265.egg-info/PKG-INFO
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)      210 2023-07-29 05:04:33.000000 t265-0.1.5/t265.egg-info/SOURCES.txt
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)        1 2023-07-29 05:04:33.000000 t265-0.1.5/t265.egg-info/dependency_links.txt
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       27 2023-07-29 05:04:33.000000 t265-0.1.5/t265.egg-info/requires.txt
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)        5 2023-07-29 05:04:33.000000 t265-0.1.5/t265.egg-info/top_level.txt
```

### Comparing `t265-0.1.4/PKG-INFO` & `t265-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t265
-Version: 0.1.4
+Version: 0.1.5
 Summary: t265 Tracking camera API wrapper
 Author: Yusuke Tanaka
 License: LGPLv3
 Project-URL: GitHub, https://github.com/Suke0811/Localization_T265
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Robot Framework
 Classifier: Intended Audience :: Developers
```

### Comparing `t265-0.1.4/setup.py` & `t265-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name='t265',
-    version='0.1.4',
+    version='0.1.5',
     description='t265 Tracking camera API wrapper',
     author='Yusuke Tanaka',
     license='LGPLv3',
     project_urls={'GitHub':'https://github.com/Suke0811/Localization_T265'},
     packages=find_packages(include=['t265', 't265.*']),
     install_requires=requirements,
     classifiers=[
```

### Comparing `t265-0.1.4/t265/Tracking.py` & `t265-0.1.5/t265/Tracking.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,16 +66,25 @@
                 frames = self.pipe.poll_for_frames()
             self.pose = frames.get_pose_frame()
         except RuntimeError:
             pass
         except KeyboardInterrupt:
             self.stop_tracking()
 
+    def get_translation(self, frame=None):
+        if frame is None:
+            return self._get_translation()
+        else:
+            T = self.get_matrix(frame)
+            if T is not None:
+                trans = T[0:3,3].flatten()
+                quat = R.from_matrix(T[0:3, 0:3]).as_quat()
+                return np.append(trans, quat)
 
-    def get_translation(self):
+    def _get_translation(self):
         if self.pose:
             trans = self._vector2np(self.pose.get_pose_data().translation)
             quat = self._quat2np(self.pose.get_pose_data().rotation)
             return np.append(trans, quat)
 
     def get_velocity(self):
         if self.pose:
@@ -87,15 +96,15 @@
         if self.pose:
             acc = self._vector2np(self.pose.get_pose_data().acceleration)
             ang_acc = self._vector2np(self.pose.get_pose_data().angular_acceleration)
             return np.append(acc, ang_acc)
 
     def get_matrix(self, frame=None):
         if self.pose:
-            trans = self.get_translation()
+            trans = self._get_translation()
             rot_mat = R.from_quat(trans[3:]).as_matrix()
             T = np.eye(4)
             T[0:3,0:3] = rot_mat
             T[0:3,3] = trans[0:3]
 
             if frame == 'ros':
                 rot = R.from_euler('xyz', [0, 90, 90], degrees=True).as_matrix()
@@ -118,12 +127,12 @@
     def __del__(self):
         self.stop_tracking()
 
 if __name__ == "__main__":
     track = Tracking()
     while True:
         track.update_pose(wait=True)
-        print("Position: {}".format(track.get_translation()))
+        print("Position: {}".format(track.get_translation('ros')))
         print(track.get_matrix('ros'))
         time.sleep(1)
         #print("Velocity: {}".format(track.get_velocity()))
         #print("Acceleration: {}\n".format(track.get_acceleration()))
```

### Comparing `t265-0.1.4/t265.egg-info/PKG-INFO` & `t265-0.1.5/t265.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t265
-Version: 0.1.4
+Version: 0.1.5
 Summary: t265 Tracking camera API wrapper
 Author: Yusuke Tanaka
 License: LGPLv3
 Project-URL: GitHub, https://github.com/Suke0811/Localization_T265
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Robot Framework
 Classifier: Intended Audience :: Developers
```

