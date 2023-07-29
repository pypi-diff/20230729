# Comparing `tmp/sweet-pipes-0.3.0rc2.tar.gz` & `tmp/sweet-pipes-0.3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweet-pipes-0.3.0rc2.tar", last modified: Fri Jul 28 17:54:05 2023, max compression
+gzip compressed data, was "sweet-pipes-0.3.0rc3.tar", last modified: Sat Jul 29 21:47:22 2023, max compression
```

## Comparing `sweet-pipes-0.3.0rc2.tar` & `sweet-pipes-0.3.0rc3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-28 17:54:05.899269 sweet-pipes-0.3.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.891270 sweet-pipes-0.3.0rc2/sweet_pipes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/sweet_pipes/coco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/coco/coco_captions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/coco/coco_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/coco/coco_keypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/coco/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/sweet_pipes/conceptual_captions/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/conceptual_captions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/conceptual_captions/conceptual_captions_12m.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/conceptual_captions/conceptual_captions_3m.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/sweet_pipes/laion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/laion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/laion/laion_2b_en.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/sweet_pipes/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/utils/albumentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/utils/datapipes.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/utils/fileio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/sweet_pipes/waymo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/waymo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/sweet_pipes/waymo/waymo_open_motion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/waymo/waymo_open_motion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/waymo/waymo_open_motion/datapipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/waymo/waymo_open_motion/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/sweet_pipes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 17:54:05.000000 sweet-pipes-0.3.0rc2/sweet_pipes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-28 17:54:05.000000 sweet-pipes-0.3.0rc2/sweet_pipes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:54:05.000000 sweet-pipes-0.3.0rc2/sweet_pipes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-28 17:54:05.000000 sweet-pipes-0.3.0rc2/sweet_pipes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 17:54:05.000000 sweet-pipes-0.3.0rc2/sweet_pipes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/tests/test_missing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:47:22.192343 sweet-pipes-0.3.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-29 21:47:22.192343 sweet-pipes-0.3.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-29 21:47:22.192343 sweet-pipes-0.3.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:47:22.192343 sweet-pipes-0.3.0rc3/sweet_pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/sweet_pipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:47:22.192343 sweet-pipes-0.3.0rc3/sweet_pipes/coco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/sweet_pipes/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/sweet_pipes/coco/coco_captions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/sweet_pipes/coco/coco_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/sweet_pipes/coco/coco_keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/sweet_pipes/coco/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:47:22.192343 sweet-pipes-0.3.0rc3/sweet_pipes/conceptual_captions/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/sweet_pipes/conceptual_captions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/sweet_pipes/conceptual_captions/conceptual_captions_12m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/sweet_pipes/conceptual_captions/conceptual_captions_3m.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:47:22.192343 sweet-pipes-0.3.0rc3/sweet_pipes/laion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/sweet_pipes/laion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/sweet_pipes/laion/laion_2b_en.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:47:22.192343 sweet-pipes-0.3.0rc3/sweet_pipes/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/sweet_pipes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/sweet_pipes/utils/albumentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/sweet_pipes/utils/datapipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/sweet_pipes/utils/fileio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:47:22.192343 sweet-pipes-0.3.0rc3/sweet_pipes/waymo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/sweet_pipes/waymo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:47:22.192343 sweet-pipes-0.3.0rc3/sweet_pipes/waymo/waymo_open_motion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/sweet_pipes/waymo/waymo_open_motion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/sweet_pipes/waymo/waymo_open_motion/datapipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/sweet_pipes/waymo/waymo_open_motion/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:47:22.192343 sweet-pipes-0.3.0rc3/sweet_pipes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-29 21:47:22.000000 sweet-pipes-0.3.0rc3/sweet_pipes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-29 21:47:22.000000 sweet-pipes-0.3.0rc3/sweet_pipes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 21:47:22.000000 sweet-pipes-0.3.0rc3/sweet_pipes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-29 21:47:22.000000 sweet-pipes-0.3.0rc3/sweet_pipes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-29 21:47:22.000000 sweet-pipes-0.3.0rc3/sweet_pipes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:47:22.192343 sweet-pipes-0.3.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-29 21:47:10.000000 sweet-pipes-0.3.0rc3/tests/test_missing.py
```

### Comparing `sweet-pipes-0.3.0rc2/LICENSE` & `sweet-pipes-0.3.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc2/PKG-INFO` & `sweet-pipes-0.3.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweet-pipes
-Version: 0.3.0rc2
+Version: 0.3.0rc3
 Summary: project_description
 Home-page: https://github.com/fkodom/sweet-pipes
 Author: Frank Odom
 Author-email: frank.odom.iii@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `sweet-pipes-0.3.0rc2/README.md` & `sweet-pipes-0.3.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc2/setup.py` & `sweet-pipes-0.3.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc2/sweet_pipes/coco/coco_captions.py` & `sweet-pipes-0.3.0rc3/sweet_pipes/coco/coco_captions.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc2/sweet_pipes/coco/coco_detection.py` & `sweet-pipes-0.3.0rc3/sweet_pipes/coco/coco_detection.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc2/sweet_pipes/coco/coco_keypoints.py` & `sweet-pipes-0.3.0rc3/sweet_pipes/coco/coco_keypoints.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc2/sweet_pipes/coco/common.py` & `sweet-pipes-0.3.0rc3/sweet_pipes/coco/common.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc2/sweet_pipes/conceptual_captions/conceptual_captions_12m.py` & `sweet-pipes-0.3.0rc3/sweet_pipes/conceptual_captions/conceptual_captions_12m.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc2/sweet_pipes/conceptual_captions/conceptual_captions_3m.py` & `sweet-pipes-0.3.0rc3/sweet_pipes/conceptual_captions/conceptual_captions_3m.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc2/sweet_pipes/laion/laion_2b_en.py` & `sweet-pipes-0.3.0rc3/sweet_pipes/laion/laion_2b_en.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc2/sweet_pipes/utils/albumentations.py` & `sweet-pipes-0.3.0rc3/sweet_pipes/utils/albumentations.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc2/sweet_pipes/utils/datapipes.py` & `sweet-pipes-0.3.0rc3/sweet_pipes/utils/datapipes.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc2/sweet_pipes/utils/fileio.py` & `sweet-pipes-0.3.0rc3/sweet_pipes/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc2/sweet_pipes/waymo/waymo_open_motion/datapipe.py` & `sweet-pipes-0.3.0rc3/sweet_pipes/waymo/waymo_open_motion/datapipe.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 from concurrent.futures import Future, ThreadPoolExecutor
 from tempfile import NamedTemporaryFile
 from typing import Generator, IO, List, Literal, Optional, Tuple, TypeVar
 from urllib.parse import urlparse
 
 from gcloud.aio.storage import Storage
-from torchdata.datapipes.iter import IterDataPipe
+from torchdata.datapipes.iter import IterDataPipe, IterableWrapper
 from torchdata.datapipes.utils import StreamWrapper
 from tqdm import tqdm
 
 T = TypeVar("T")
 URL_TEMPLATE = (
     "gs://waymo_open_dataset_motion_v_1_2_0/uncompressed/{format}/"
     "{dataset_name}/{file_name}.tfrecord-{idx:05d}-of-01000"
@@ -117,20 +117,16 @@
         self.dp = dp
 
     def __iter__(self) -> Generator[T, None, None]:
         iterator = iter(self.dp)
         while True:
             try:
                 yield next(iterator)
-            except (MemoryError, OverflowError) as e:
-                logging.error(
-                    f"{type(e).__name__} encountered. Skipping sample.  {str(e)}"
-                )
-                breakpoint()
-                pass
+            except OverflowError as e:
+                logging.error(f"OverflowError encountered. Skipping sample.  {str(e)}")
             except StopIteration:
                 break
 
 
 def waymo_open_motion_datapipe(
     split: Literal["train", "validation", "test"],
     format: Literal["scenario", "tf_example"] = "tf_example",
```

### Comparing `sweet-pipes-0.3.0rc2/sweet_pipes.egg-info/PKG-INFO` & `sweet-pipes-0.3.0rc3/sweet_pipes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweet-pipes
-Version: 0.3.0rc2
+Version: 0.3.0rc3
 Summary: project_description
 Home-page: https://github.com/fkodom/sweet-pipes
 Author: Frank Odom
 Author-email: frank.odom.iii@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `sweet-pipes-0.3.0rc2/sweet_pipes.egg-info/SOURCES.txt` & `sweet-pipes-0.3.0rc3/sweet_pipes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

