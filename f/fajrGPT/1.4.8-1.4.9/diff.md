# Comparing `tmp/fajrGPT-1.4.8.tar.gz` & `tmp/fajrGPT-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.4.8.tar", last modified: Fri Jul 28 11:36:53 2023, max compression
+gzip compressed data, was "fajrGPT-1.4.9.tar", last modified: Sat Jul 29 13:33:59 2023, max compression
```

## Comparing `fajrGPT-1.4.8.tar` & `fajrGPT-1.4.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-28 11:36:53.210594 fajrGPT-1.4.8/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.4.8/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-28 11:36:53.210364 fajrGPT-1.4.8/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.4.8/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-28 11:36:53.206649 fajrGPT-1.4.8/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.4.8/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.4.8/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)    19709 2023-07-28 11:35:48.000000 fajrGPT-1.4.8/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-28 11:36:53.210078 fajrGPT-1.4.8/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-28 11:36:53.000000 fajrGPT-1.4.8/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-28 11:36:53.000000 fajrGPT-1.4.8/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-28 11:36:53.000000 fajrGPT-1.4.8/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-28 11:36:53.000000 fajrGPT-1.4.8/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-28 11:36:53.000000 fajrGPT-1.4.8/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-28 11:36:53.000000 fajrGPT-1.4.8/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-28 11:36:53.210639 fajrGPT-1.4.8/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-07-28 11:36:05.000000 fajrGPT-1.4.8/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-29 13:33:59.644154 fajrGPT-1.4.9/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.4.9/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-29 13:33:59.643975 fajrGPT-1.4.9/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.4.9/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-29 13:33:59.642021 fajrGPT-1.4.9/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.4.9/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.4.9/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)    19713 2023-07-29 13:12:25.000000 fajrGPT-1.4.9/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-29 13:33:59.643757 fajrGPT-1.4.9/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-29 13:33:59.000000 fajrGPT-1.4.9/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-29 13:33:59.000000 fajrGPT-1.4.9/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-29 13:33:59.000000 fajrGPT-1.4.9/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-29 13:33:59.000000 fajrGPT-1.4.9/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       62 2023-07-29 13:33:59.000000 fajrGPT-1.4.9/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-29 13:33:59.000000 fajrGPT-1.4.9/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-29 13:33:59.644197 fajrGPT-1.4.9/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1148 2023-07-29 13:27:37.000000 fajrGPT-1.4.9/setup.py
```

### Comparing `fajrGPT-1.4.8/LICENSE` & `fajrGPT-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.8/PKG-INFO` & `fajrGPT-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.4.8
+Version: 1.4.9
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.4.8/README.md` & `fajrGPT-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.8/fajrGPT/quran_metadata.py` & `fajrGPT-1.4.9/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.8/fajrGPT/wake.py` & `fajrGPT-1.4.9/fajrGPT/wake.py`

 * *Files 1% similar despite different names*

```diff
@@ -424,15 +424,15 @@
     pygame.mixer.music.load(file_path)
 
     # Start playing the audio with volume 0
     pygame.mixer.music.set_volume(0.0)
     pygame.mixer.music.play()
 
     # if the transition time is longer than the audio, set it to the audio length
-    length_in_seconds = mp3(file_path).info.length
+    length_in_seconds = mp3.MP3(file_path).info.length
     if transition_time > length_in_seconds:
         transition_time = length_in_seconds * 0.5
 
     # Gradually increase the volume over 15 minutes in a separate thread
     gradually_change_volume(0.0, 1.0, transition_time)
 
     # Loop the audio until the stop_audio function is called
```

### Comparing `fajrGPT-1.4.8/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.4.9/fajrGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.4.8
+Version: 1.4.9
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.4.8/setup.py` & `fajrGPT-1.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.4.8",
+    version="1.4.9",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
@@ -22,14 +22,15 @@
     install_requires=[
         "click",
         "pygame",
         "pydub",
         "moviepy",
         "openai",
         "tqdm",
+        "mutagen",
         "TheQuranModule"
     ],
     entry_points={
         'console_scripts': [
             'fajrGPT=fajrGPT.wake:main',
         ],
     },
```

