# Comparing `tmp/ytws-0.2.0.tar.gz` & `tmp/ytws-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytws-0.2.0.tar", last modified: Sat Jul 29 13:12:14 2023, max compression
+gzip compressed data, was "ytws-0.2.1.tar", last modified: Sat Jul 29 14:51:44 2023, max compression
```

## Comparing `ytws-0.2.0.tar` & `ytws-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 13:12:14.140997 ytws-0.2.0/
--rw-rw-rw-   0        0        0     1083 2023-07-26 21:38:04.000000 ytws-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     3758 2023-07-29 13:12:14.139998 ytws-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3218 2023-07-29 13:11:32.000000 ytws-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-29 13:12:14.140997 ytws-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1039 2023-07-29 13:07:45.000000 ytws-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 13:12:14.116378 ytws-0.2.0/src/
--rw-rw-rw-   0        0        0        0 2023-07-29 04:29:43.000000 ytws-0.2.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 13:12:14.118395 ytws-0.2.0/src/cli/
--rw-rw-rw-   0        0        0        0 2023-07-28 15:10:41.000000 ytws-0.2.0/src/cli/__init__.py
--rw-rw-rw-   0        0        0     3950 2023-07-29 11:41:43.000000 ytws-0.2.0/src/cli/main.py
-drwxrwxrwx   0        0        0        0 2023-07-29 13:12:14.121393 ytws-0.2.0/src/whisper/
--rw-rw-rw-   0        0        0        0 2023-07-28 15:10:41.000000 ytws-0.2.0/src/whisper/__init__.py
--rw-rw-rw-   0        0        0     1172 2023-07-29 12:14:33.000000 ytws-0.2.0/src/whisper/subtitles.py
--rw-rw-rw-   0        0        0     1082 2023-07-29 07:57:40.000000 ytws-0.2.0/src/whisper/transcribe.py
-drwxrwxrwx   0        0        0        0 2023-07-29 13:12:14.123393 ytws-0.2.0/src/youtube/
--rw-rw-rw-   0        0        0        0 2023-07-28 15:10:41.000000 ytws-0.2.0/src/youtube/__init__.py
--rw-rw-rw-   0        0        0     1019 2023-07-29 07:02:05.000000 ytws-0.2.0/src/youtube/download.py
-drwxrwxrwx   0        0        0        0 2023-07-29 13:12:14.138998 ytws-0.2.0/ytws.egg-info/
--rw-rw-rw-   0        0        0     3758 2023-07-29 13:12:14.000000 ytws-0.2.0/ytws.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-07-29 13:12:14.000000 ytws-0.2.0/ytws.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 13:12:14.000000 ytws-0.2.0/ytws.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-07-29 13:12:14.000000 ytws-0.2.0/ytws.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       66 2023-07-29 13:12:14.000000 ytws-0.2.0/ytws.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-29 13:12:14.000000 ytws-0.2.0/ytws.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 14:51:44.198868 ytws-0.2.1/
+-rw-rw-rw-   0        0        0     1083 2023-07-26 21:38:04.000000 ytws-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4099 2023-07-29 14:51:44.197869 ytws-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3559 2023-07-29 14:51:14.000000 ytws-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-29 14:51:44.198868 ytws-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1039 2023-07-29 14:50:42.000000 ytws-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:51:44.156191 ytws-0.2.1/src/
+-rw-rw-rw-   0        0        0        0 2023-07-29 04:29:43.000000 ytws-0.2.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:51:44.159192 ytws-0.2.1/src/cli/
+-rw-rw-rw-   0        0        0        0 2023-07-28 15:10:41.000000 ytws-0.2.1/src/cli/__init__.py
+-rw-rw-rw-   0        0        0     3950 2023-07-29 11:41:43.000000 ytws-0.2.1/src/cli/main.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:51:44.173223 ytws-0.2.1/src/whisper/
+-rw-rw-rw-   0        0        0        0 2023-07-28 15:10:41.000000 ytws-0.2.1/src/whisper/__init__.py
+-rw-rw-rw-   0        0        0     1172 2023-07-29 12:14:33.000000 ytws-0.2.1/src/whisper/subtitles.py
+-rw-rw-rw-   0        0        0     1082 2023-07-29 07:57:40.000000 ytws-0.2.1/src/whisper/transcribe.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:51:44.179225 ytws-0.2.1/src/youtube/
+-rw-rw-rw-   0        0        0        0 2023-07-28 15:10:41.000000 ytws-0.2.1/src/youtube/__init__.py
+-rw-rw-rw-   0        0        0     1019 2023-07-29 07:02:05.000000 ytws-0.2.1/src/youtube/download.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:51:44.196867 ytws-0.2.1/ytws.egg-info/
+-rw-rw-rw-   0        0        0     4099 2023-07-29 14:51:44.000000 ytws-0.2.1/ytws.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-07-29 14:51:44.000000 ytws-0.2.1/ytws.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 14:51:44.000000 ytws-0.2.1/ytws.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-07-29 14:51:44.000000 ytws-0.2.1/ytws.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       66 2023-07-29 14:51:44.000000 ytws-0.2.1/ytws.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-29 14:51:44.000000 ytws-0.2.1/ytws.egg-info/top_level.txt
```

### Comparing `ytws-0.2.0/LICENSE` & `ytws-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ytws-0.2.0/PKG-INFO` & `ytws-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-Metadata-Version: 2.1
-Name: ytws
-Version: 0.2.0
-Summary: YouTube Whisper - A YouTube Downloader with Transcription
-Home-page: https://github.com/faker2048/youtube-whisper
-Author: faker2048
-Author-email: nspyia2002@gmail.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 🎥 YTWS: YouTube Download and Subtitle Generation Tool 🔥
 
-![YTWS](https://images.unsplash.com/photo-1511379938547-c1f69419868d)
-
 YTWS is a command-line tool designed to download videos from YouTube and generate subtitles, all with the power of the efficient `faster-whisper`.
 
+
+## Features
+
+- **Easy to Use**: Get started without hassle.
+- **Fast Subtitle Generation**: Utilize `faster-whisper` for quick results.
+- **GPU Acceleration**: Simple guide for GPU utilization.
+- **Cross-Platform**: Works on Windows and Linux.
+
+These features make YTWS an efficient and user-friendly tool for downloading YouTube videos and generating subtitles.
+
 ## 💽 Installation
 You can easily install YTWS using the following commands:
+
+```bash
+pip install ytws
+```
+or 
 ```bash
 git clone https://github.com/faker2048/youtube-whisper
 cd youtube-whisper
 pip install .
 ```
 
 ### Preparations Before Running
```

### Comparing `ytws-0.2.0/README.md` & `ytws-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,43 @@
-# 🎥 YTWS: YouTube Download and Subtitle Generation Tool 🔥
+Metadata-Version: 2.1
+Name: ytws
+Version: 0.2.1
+Summary: YouTube Whisper - A YouTube Downloader with Transcription
+Home-page: https://github.com/faker2048/youtube-whisper
+Author: faker2048
+Author-email: nspyia2002@gmail.com
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-![YTWS](https://images.unsplash.com/photo-1511379938547-c1f69419868d)
+# 🎥 YTWS: YouTube Download and Subtitle Generation Tool 🔥
 
 YTWS is a command-line tool designed to download videos from YouTube and generate subtitles, all with the power of the efficient `faster-whisper`.
 
+
+## Features
+
+- **Easy to Use**: Get started without hassle.
+- **Fast Subtitle Generation**: Utilize `faster-whisper` for quick results.
+- **GPU Acceleration**: Simple guide for GPU utilization.
+- **Cross-Platform**: Works on Windows and Linux.
+
+These features make YTWS an efficient and user-friendly tool for downloading YouTube videos and generating subtitles.
+
 ## 💽 Installation
 You can easily install YTWS using the following commands:
+
+```bash
+pip install ytws
+```
+or 
 ```bash
 git clone https://github.com/faker2048/youtube-whisper
 cd youtube-whisper
 pip install .
 ```
 
 ### Preparations Before Running
```

### Comparing `ytws-0.2.0/setup.py` & `ytws-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ytws",
-    version="0.2.0",
+    version="0.2.1",
     description="YouTube Whisper - A YouTube Downloader with Transcription",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="faker2048",
     author_email="nspyia2002@gmail.com",
     url="https://github.com/faker2048/youtube-whisper",
     packages=find_packages(include=["src", "src.*"]),
```

### Comparing `ytws-0.2.0/src/cli/main.py` & `ytws-0.2.1/src/cli/main.py`

 * *Files identical despite different names*

### Comparing `ytws-0.2.0/src/whisper/subtitles.py` & `ytws-0.2.1/src/whisper/subtitles.py`

 * *Files identical despite different names*

### Comparing `ytws-0.2.0/src/whisper/transcribe.py` & `ytws-0.2.1/src/whisper/transcribe.py`

 * *Files identical despite different names*

### Comparing `ytws-0.2.0/src/youtube/download.py` & `ytws-0.2.1/src/youtube/download.py`

 * *Files identical despite different names*

### Comparing `ytws-0.2.0/ytws.egg-info/PKG-INFO` & `ytws-0.2.1/ytws.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 Metadata-Version: 2.1
 Name: ytws
-Version: 0.2.0
+Version: 0.2.1
 Summary: YouTube Whisper - A YouTube Downloader with Transcription
 Home-page: https://github.com/faker2048/youtube-whisper
 Author: faker2048
 Author-email: nspyia2002@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🎥 YTWS: YouTube Download and Subtitle Generation Tool 🔥
 
-![YTWS](https://images.unsplash.com/photo-1511379938547-c1f69419868d)
-
 YTWS is a command-line tool designed to download videos from YouTube and generate subtitles, all with the power of the efficient `faster-whisper`.
 
+
+## Features
+
+- **Easy to Use**: Get started without hassle.
+- **Fast Subtitle Generation**: Utilize `faster-whisper` for quick results.
+- **GPU Acceleration**: Simple guide for GPU utilization.
+- **Cross-Platform**: Works on Windows and Linux.
+
+These features make YTWS an efficient and user-friendly tool for downloading YouTube videos and generating subtitles.
+
 ## 💽 Installation
 You can easily install YTWS using the following commands:
+
+```bash
+pip install ytws
+```
+or 
 ```bash
 git clone https://github.com/faker2048/youtube-whisper
 cd youtube-whisper
 pip install .
 ```
 
 ### Preparations Before Running
```

