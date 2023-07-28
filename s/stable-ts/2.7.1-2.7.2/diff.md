# Comparing `tmp/stable-ts-2.7.1.tar.gz` & `tmp/stable-ts-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-2.7.1.tar", last modified: Thu Jul 20 19:58:11 2023, max compression
+gzip compressed data, was "stable-ts-2.7.2.tar", last modified: Fri Jul 28 23:47:54 2023, max compression
```

## Comparing `stable-ts-2.7.1.tar` & `stable-ts-2.7.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 19:58:11.805999 stable-ts-2.7.1/
--rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.7.1/LICENSE
--rw-rw-rw-   0        0        0    11472 2023-07-20 19:58:11.804998 stable-ts-2.7.1/PKG-INFO
--rw-rw-rw-   0        0        0    11176 2023-07-20 19:47:30.000000 stable-ts-2.7.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-20 19:58:11.807000 stable-ts-2.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 19:58:11.731932 stable-ts-2.7.1/stable_ts.egg-info/
--rw-rw-rw-   0        0        0    11472 2023-07-20 19:58:11.000000 stable-ts-2.7.1/stable_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      627 2023-07-20 19:58:11.000000 stable-ts-2.7.1/stable_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 19:58:11.000000 stable-ts-2.7.1/stable_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-07-20 19:58:11.000000 stable-ts-2.7.1/stable_ts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-07-20 19:58:11.000000 stable-ts-2.7.1/stable_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-20 19:58:11.000000 stable-ts-2.7.1/stable_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-20 19:58:11.802997 stable-ts-2.7.1/stable_whisper/
--rw-rw-rw-   0        0        0      241 2023-07-13 00:23:52.000000 stable-ts-2.7.1/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.7.1/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       23 2023-07-20 19:40:56.000000 stable-ts-2.7.1/stable_whisper/_version.py
--rw-rw-rw-   0        0        0     8360 2023-07-13 00:08:53.000000 stable-ts-2.7.1/stable_whisper/audio.py
--rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.7.1/stable_whisper/decode.py
--rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.7.1/stable_whisper/enhancement.py
--rw-rw-rw-   0        0        0    12947 2023-07-13 00:22:18.000000 stable-ts-2.7.1/stable_whisper/non_whisper.py
--rw-rw-rw-   0        0        0     1645 2023-05-03 19:33:54.000000 stable-ts-2.7.1/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0    43551 2023-07-20 19:56:22.000000 stable-ts-2.7.1/stable_whisper/result.py
--rw-rw-rw-   0        0        0    14128 2023-07-12 23:15:05.000000 stable-ts-2.7.1/stable_whisper/stabilization.py
--rw-rw-rw-   0        0        0    20528 2023-05-08 02:53:22.000000 stable-ts-2.7.1/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.7.1/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.7.1/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0    53252 2023-07-13 00:20:47.000000 stable-ts-2.7.1/stable_whisper/whisper_word_level.py
+drwxrwxrwx   0        0        0        0 2023-07-28 23:47:54.101724 stable-ts-2.7.2/
+-rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.7.2/LICENSE
+-rw-rw-rw-   0        0        0    11472 2023-07-28 23:47:54.101724 stable-ts-2.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11176 2023-07-20 19:47:30.000000 stable-ts-2.7.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-28 23:47:54.102725 stable-ts-2.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 23:47:54.033451 stable-ts-2.7.2/stable_ts.egg-info/
+-rw-rw-rw-   0        0        0    11472 2023-07-28 23:47:53.000000 stable-ts-2.7.2/stable_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-07-28 23:47:53.000000 stable-ts-2.7.2/stable_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 23:47:53.000000 stable-ts-2.7.2/stable_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-07-28 23:47:53.000000 stable-ts-2.7.2/stable_ts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-07-28 23:47:53.000000 stable-ts-2.7.2/stable_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-28 23:47:53.000000 stable-ts-2.7.2/stable_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 23:47:54.098722 stable-ts-2.7.2/stable_whisper/
+-rw-rw-rw-   0        0        0      241 2023-07-13 00:23:52.000000 stable-ts-2.7.2/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.7.2/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-07-28 23:15:11.000000 stable-ts-2.7.2/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0     8360 2023-07-13 00:08:53.000000 stable-ts-2.7.2/stable_whisper/audio.py
+-rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.7.2/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.7.2/stable_whisper/enhancement.py
+-rw-rw-rw-   0        0        0    12947 2023-07-13 00:22:18.000000 stable-ts-2.7.2/stable_whisper/non_whisper.py
+-rw-rw-rw-   0        0        0     1645 2023-05-03 19:33:54.000000 stable-ts-2.7.2/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0    43529 2023-07-28 23:22:16.000000 stable-ts-2.7.2/stable_whisper/result.py
+-rw-rw-rw-   0        0        0    14128 2023-07-12 23:15:05.000000 stable-ts-2.7.2/stable_whisper/stabilization.py
+-rw-rw-rw-   0        0        0    20528 2023-05-08 02:53:22.000000 stable-ts-2.7.2/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.7.2/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.7.2/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0    53252 2023-07-13 00:20:47.000000 stable-ts-2.7.2/stable_whisper/whisper_word_level.py
```

### Comparing `stable-ts-2.7.1/LICENSE` & `stable-ts-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.1/PKG-INFO` & `stable-ts-2.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.7.1
+Version: 2.7.2
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.7.1/README.md` & `stable-ts-2.7.2/README.md`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.1/setup.py` & `stable-ts-2.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.1/stable_ts.egg-info/PKG-INFO` & `stable-ts-2.7.2/stable_ts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.7.1
+Version: 2.7.2
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.7.1/stable_ts.egg-info/SOURCES.txt` & `stable-ts-2.7.2/stable_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.1/stable_whisper/audio.py` & `stable-ts-2.7.2/stable_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.1/stable_whisper/decode.py` & `stable-ts-2.7.2/stable_whisper/decode.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.1/stable_whisper/enhancement.py` & `stable-ts-2.7.2/stable_whisper/enhancement.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.1/stable_whisper/non_whisper.py` & `stable-ts-2.7.2/stable_whisper/non_whisper.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.1/stable_whisper/quantization.py` & `stable-ts-2.7.2/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.1/stable_whisper/result.py` & `stable-ts-2.7.2/stable_whisper/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,21 +344,21 @@
                          silent_starts: np.ndarray,
                          silent_ends: np.ndarray,
                          min_word_dur: float = 0.1,
                          word_level: bool = True):
         if self.has_words:
             words = self.words if word_level or len(self.words) == 1 else [self.words[0], self.words[-1]]
             for w in words:
-                w.suppress_silence(silent_starts, silent_ends)
+                w.suppress_silence(silent_starts, silent_ends, min_word_dur)
             self.update_seg_with_words()
         else:
             suppress_silence(self,
                              silent_starts,
                              silent_ends,
-                             max((self.end - self.start) * .75, min_word_dur))
+                             min_word_dur)
 
         return self
 
     def get_locked_indices(self):
         locked_indices = [i
                           for i, (left, right) in enumerate(zip(self.words[1:], self.words[:-1]))
                           if left.left_locked or right.right_locked]
```

### Comparing `stable-ts-2.7.1/stable_whisper/stabilization.py` & `stable-ts-2.7.2/stable_whisper/stabilization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.1/stable_whisper/text_output.py` & `stable-ts-2.7.2/stable_whisper/text_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.1/stable_whisper/timing.py` & `stable-ts-2.7.2/stable_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.1/stable_whisper/video_output.py` & `stable-ts-2.7.2/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.1/stable_whisper/whisper_word_level.py` & `stable-ts-2.7.2/stable_whisper/whisper_word_level.py`

 * *Files identical despite different names*

