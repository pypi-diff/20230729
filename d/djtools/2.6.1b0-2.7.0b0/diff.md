# Comparing `tmp/djtools-2.6.1b0.tar.gz` & `tmp/djtools-2.7.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djtools-2.6.1b0.tar", last modified: Wed Jul 26 19:15:13 2023, max compression
+gzip compressed data, was "djtools-2.7.0b0.tar", last modified: Sat Jul 29 19:28:59 2023, max compression
```

## Comparing `djtools-2.6.1b0.tar` & `djtools-2.7.0b0.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-26 19:15:13.742177 djtools-2.6.1b0/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 djtools-2.6.1b0/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 djtools-2.6.1b0/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)     2677 2023-07-26 19:15:13.742304 djtools-2.6.1b0/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1445 2023-07-26 18:56:00.000000 djtools-2.6.1b0/README.md
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-26 19:15:13.710611 djtools-2.6.1b0/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)     2541 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1885 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/__main__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-26 19:15:13.720596 djtools-2.6.1b0/djtools/collection/
--rw-r--r--   0 alrichards   (502) staff       (20)     1428 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/collection/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)    12876 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/collection/collections.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2914 2023-07-26 18:56:00.000000 djtools-2.6.1b0/djtools/collection/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2985 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/collection/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    27429 2023-07-26 18:56:00.000000 djtools-2.6.1b0/djtools/collection/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7697 2023-07-26 18:56:00.000000 djtools-2.6.1b0/djtools/collection/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)    15832 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/collection/playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2404 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/collection/shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    13886 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/collection/tracks.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-26 19:15:13.728238 djtools-2.6.1b0/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 djtools-2.6.1b0/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1179 2023-07-26 18:24:13.000000 djtools-2.6.1b0/djtools/configs/collection_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     1765 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1334 2023-07-26 19:13:43.000000 djtools-2.6.1b0/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    21130 2023-07-26 17:53:37.000000 djtools-2.6.1b0/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 djtools-2.6.1b0/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 djtools-2.6.1b0/djtools/configs/spotify_playlists.yaml
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-26 19:15:13.729254 djtools-2.6.1b0/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 djtools-2.6.1b0/djtools/logs/empty.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-26 19:15:13.733493 djtools-2.6.1b0/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      735 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3258 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    16599 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6053 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/spotify/playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-26 19:15:13.738879 djtools-2.6.1b0/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      874 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3693 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7682 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5415 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/sync/sync_operations.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-26 19:15:13.741757 djtools-2.6.1b0/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1409 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    10160 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 djtools-2.6.1b0/djtools/utils/url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-07-26 19:15:02.000000 djtools-2.6.1b0/djtools/version.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-26 19:15:13.713575 djtools-2.6.1b0/djtools.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)     2677 2023-07-26 19:15:13.000000 djtools-2.6.1b0/djtools.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1209 2023-07-26 19:15:13.000000 djtools-2.6.1b0/djtools.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-07-26 19:15:13.000000 djtools-2.6.1b0/djtools.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-07-26 19:15:13.000000 djtools-2.6.1b0/djtools.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-07-26 19:15:13.000000 djtools-2.6.1b0/djtools.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-07-26 19:15:13.000000 djtools-2.6.1b0/djtools.egg-info/top_level.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 djtools-2.6.1b0/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)       99 2023-07-26 19:15:13.742684 djtools-2.6.1b0/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2340 2023-07-24 23:14:57.000000 djtools-2.6.1b0/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:59.196725 djtools-2.7.0b0/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 djtools-2.7.0b0/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 djtools-2.7.0b0/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)     2864 2023-07-29 19:28:59.196855 djtools-2.7.0b0/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1632 2023-07-29 18:53:45.000000 djtools-2.7.0b0/README.md
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:59.166823 djtools-2.7.0b0/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2621 2023-07-29 19:17:36.000000 djtools-2.7.0b0/djtools/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1885 2023-07-29 19:17:36.000000 djtools-2.7.0b0/djtools/__main__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:59.180351 djtools-2.7.0b0/djtools/collection/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1428 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/collection/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    12876 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/collection/collections.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2914 2023-07-26 18:56:00.000000 djtools-2.7.0b0/djtools/collection/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2985 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/collection/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    27429 2023-07-26 18:56:00.000000 djtools-2.7.0b0/djtools/collection/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7697 2023-07-26 18:56:00.000000 djtools-2.7.0b0/djtools/collection/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    15832 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/collection/playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2404 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/collection/shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    13886 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/collection/tracks.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:59.185634 djtools-2.7.0b0/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 djtools-2.7.0b0/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1179 2023-07-26 18:24:13.000000 djtools-2.7.0b0/djtools/configs/collection_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     1765 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1495 2023-07-29 19:18:55.000000 djtools-2.7.0b0/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    22288 2023-07-29 18:53:45.000000 djtools-2.7.0b0/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 djtools-2.7.0b0/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:30.000000 djtools-2.7.0b0/djtools/configs/spotify_playlists.yaml
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:59.186326 djtools-2.7.0b0/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 djtools-2.7.0b0/djtools/logs/empty.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:59.189214 djtools-2.7.0b0/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      735 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3258 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    16599 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6053 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/spotify/playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:59.191517 djtools-2.7.0b0/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      874 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3693 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7682 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5343 2023-07-29 18:53:45.000000 djtools-2.7.0b0/djtools/sync/sync_operations.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:59.196253 djtools-2.7.0b0/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1441 2023-07-29 18:53:45.000000 djtools-2.7.0b0/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4233 2023-07-29 18:53:45.000000 djtools-2.7.0b0/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2130 2023-07-29 18:53:45.000000 djtools-2.7.0b0/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     9264 2023-07-29 18:53:45.000000 djtools-2.7.0b0/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1719 2023-07-29 19:24:52.000000 djtools-2.7.0b0/djtools/utils/normalize_audio.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5138 2023-07-29 19:24:55.000000 djtools-2.7.0b0/djtools/utils/process_recording.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 djtools-2.7.0b0/djtools/utils/url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-07-29 18:53:45.000000 djtools-2.7.0b0/djtools/version.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:59.172909 djtools-2.7.0b0/djtools.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2864 2023-07-29 19:28:59.000000 djtools-2.7.0b0/djtools.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1277 2023-07-29 19:28:59.000000 djtools-2.7.0b0/djtools.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-07-29 19:28:59.000000 djtools-2.7.0b0/djtools.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-07-29 19:28:59.000000 djtools-2.7.0b0/djtools.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      278 2023-07-29 19:28:59.000000 djtools-2.7.0b0/djtools.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-07-29 19:28:59.000000 djtools-2.7.0b0/djtools.egg-info/top_level.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 djtools-2.7.0b0/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)       99 2023-07-29 19:28:59.197283 djtools-2.7.0b0/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2361 2023-07-29 19:17:36.000000 djtools-2.7.0b0/setup.py
```

### Comparing `djtools-2.6.1b0/LICENSE` & `djtools-2.7.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/PKG-INFO` & `djtools-2.7.0b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djtools
-Version: 2.6.1b0
+Version: 2.7.0b0
 Summary: DJ Tools is a library for managing a collection of music.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 Keywords: DJ Rekordbox spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -31,21 +31,23 @@
 # DJ Tools
 [![image](https://img.shields.io/pypi/v/djtools.svg)](https://pypi.org/project/djtools/)
 
 Please see the [docs](https://a-rich.github.io/DJ-Tools/) for tutorials, how-to guides, conceptual guides, and references!
 
 # Release Plan
 * 2.6.1
+    - [ ] [Stability issues with requests to the search endpoint of the Spotify API](https://github.com/a-rich/DJ-Tools/issues/58)
+    - [ ] [Make Spotify API calls asynchronous](https://github.com/a-rich/DJ-Tools/issues/38)
+* 2.7.0
     - [x] Script for removing situation tags and resolving album, label, and year for tracks
     - [x] Allow `build_config` to accept an override for the path to `config.yaml`
     - [x] Fix missing typehints for the `NonEmptyListElementAction` class
     - [x] [Make PlaylistFilter implementations configurable](https://github.com/a-rich/DJ-Tools/issues/120)
     - [x] [Make MinimalDeepTechFilter more robust to the relative position of House and Techno tags](https://github.com/a-rich/DJ-Tools/issues/122)
-    - [ ] [Stability issues with requests to the search endpoint of the Spotify API](https://github.com/a-rich/DJ-Tools/issues/58)
-    - [ ] [Make Spotify API calls asynchronous](https://github.com/a-rich/DJ-Tools/issues/38)
-* 2.7.0
-    - [ ] [Improve Reddit submission title parsing in order to improve precision and recall of Spotify API search results](https://github.com/a-rich/DJ-Tools/issues/59)
-    - [ ] [Derive boolean algebra expressions that generate a given playlist](https://github.com/a-rich/DJ-Tools/issues/106)
+    - [x] [Standardize audio files](https://github.com/a-rich/DJ-Tools/issues/126)
+    - [x] [Process recorded file using Spotify playlist](https://github.com/a-rich/DJ-Tools/issues/127)
     - [ ] [Create graphic user interface for djtools](https://github.com/a-rich/DJ-Tools/issues/118)
+    - [ ] [Derive boolean algebra expressions that generate a given playlist](https://github.com/a-rich/DJ-Tools/issues/106)
+    - [ ] [Improve Reddit submission title parsing in order to improve precision and recall of Spotify API search results](https://github.com/a-rich/DJ-Tools/issues/59)
 
 # Contribution
 Please see the [CONTRIBUTING](CONTRIBUTING.md)
```

### Comparing `djtools-2.6.1b0/README.md` & `djtools-2.7.0b0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # DJ Tools
 [![image](https://img.shields.io/pypi/v/djtools.svg)](https://pypi.org/project/djtools/)
 
 Please see the [docs](https://a-rich.github.io/DJ-Tools/) for tutorials, how-to guides, conceptual guides, and references!
 
 # Release Plan
 * 2.6.1
+    - [ ] [Stability issues with requests to the search endpoint of the Spotify API](https://github.com/a-rich/DJ-Tools/issues/58)
+    - [ ] [Make Spotify API calls asynchronous](https://github.com/a-rich/DJ-Tools/issues/38)
+* 2.7.0
     - [x] Script for removing situation tags and resolving album, label, and year for tracks
     - [x] Allow `build_config` to accept an override for the path to `config.yaml`
     - [x] Fix missing typehints for the `NonEmptyListElementAction` class
     - [x] [Make PlaylistFilter implementations configurable](https://github.com/a-rich/DJ-Tools/issues/120)
     - [x] [Make MinimalDeepTechFilter more robust to the relative position of House and Techno tags](https://github.com/a-rich/DJ-Tools/issues/122)
-    - [ ] [Stability issues with requests to the search endpoint of the Spotify API](https://github.com/a-rich/DJ-Tools/issues/58)
-    - [ ] [Make Spotify API calls asynchronous](https://github.com/a-rich/DJ-Tools/issues/38)
-* 2.7.0
-    - [ ] [Improve Reddit submission title parsing in order to improve precision and recall of Spotify API search results](https://github.com/a-rich/DJ-Tools/issues/59)
-    - [ ] [Derive boolean algebra expressions that generate a given playlist](https://github.com/a-rich/DJ-Tools/issues/106)
+    - [x] [Standardize audio files](https://github.com/a-rich/DJ-Tools/issues/126)
+    - [x] [Process recorded file using Spotify playlist](https://github.com/a-rich/DJ-Tools/issues/127)
     - [ ] [Create graphic user interface for djtools](https://github.com/a-rich/DJ-Tools/issues/118)
+    - [ ] [Derive boolean algebra expressions that generate a given playlist](https://github.com/a-rich/DJ-Tools/issues/106)
+    - [ ] [Improve Reddit submission title parsing in order to improve precision and recall of Spotify API search results](https://github.com/a-rich/DJ-Tools/issues/59)
 
 # Contribution
 Please see the [CONTRIBUTING](CONTRIBUTING.md)
```

### Comparing `djtools-2.6.1b0/djtools/__init__.py` & `djtools-2.7.0b0/djtools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     upload_collection,
     upload_log,
     upload_music,
 )
 from .utils import (
     compare_tracks,
     initialize_logger,
+    normalize,
+    process_recording,
     UTILS_OPERATIONS,
     url_download,
 )
 from .version import __version__
 
 
 __all__ = (
@@ -42,14 +44,16 @@
     "COLLECTION_OPERATIONS",
     "collection_playlists",
     "compare_tracks",
     "copy_playlists",
     "download_collection",
     "download_music",
     "initialize_logger",
+    "normalize",
+    "process_recording",
     "shuffle_playlists",
     "spotify_playlist_from_upload",
     "spotify_playlists",
     "SPOTIFY_OPERATIONS",
     "SYNC_OPERATIONS",
     "upload_log",
     "upload_collection",
```

### Comparing `djtools-2.6.1b0/djtools/__main__.py` & `djtools-2.7.0b0/djtools/__main__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools/collection/__init__.py` & `djtools-2.7.0b0/djtools/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools/collection/collections.py` & `djtools-2.7.0b0/djtools/collection/collections.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools/collection/config.py` & `djtools-2.7.0b0/djtools/collection/config.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools/collection/copy_playlists.py` & `djtools-2.7.0b0/djtools/collection/copy_playlists.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools/collection/helpers.py` & `djtools-2.7.0b0/djtools/collection/helpers.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools/collection/playlist_builder.py` & `djtools-2.7.0b0/djtools/collection/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools/collection/playlists.py` & `djtools-2.7.0b0/djtools/collection/playlists.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools/collection/shuffle_playlists.py` & `djtools-2.7.0b0/djtools/collection/shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools/collection/tracks.py` & `djtools-2.7.0b0/djtools/collection/tracks.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools/configs/collection_playlists.yaml` & `djtools-2.7.0b0/djtools/configs/collection_playlists.yaml`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools/configs/config.py` & `djtools-2.7.0b0/djtools/configs/config.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools/configs/helpers.py` & `djtools-2.7.0b0/djtools/configs/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -430,42 +430,79 @@
             "list of local paths to tracks in the Beatcloud to determine if "
             "you have redundancies\n  - downloading audio files from a URL "
             "containing embedded audio (e.g. Soundcloud)"
         ),
         formatter_class=RawTextHelpFormatter,
     )
     utils_parser.add_argument(
+        "--audio-bitrate",
+        type=str,
+        help='Bitrate used to save files output by "--process-recording"',
+    )
+    utils_parser.add_argument(
+        "--audio-format",
+        type=str,
+        help='File format to save files output by "--process-recording"',
+    )
+    utils_parser.add_argument(
         "--check-tracks",
         action="store_true",
         help=(
             "Flag to trigger checking for track overlap between the Beatcloud "
-            'and "--check-tracks-local-dirs" and / or '
-            '"--check-tracks-spotify-playlists".'
+            'and "--local-dirs" and / or "--check-tracks-spotify-playlists".'
         ),
     )
     utils_parser.add_argument(
         "--check-tracks-fuzz-ratio",
         type=int,
         help=(
             "Minimum similarity to indicate overlap between Beatcloud and "
             "Spotify / local tracks."
         ),
     )
     utils_parser.add_argument(
-        "--check-tracks-local-dirs",
+        "--check-tracks-spotify-playlists",
+        type=str,
+        nargs="+",
+        help="List of Spotify playlist names to check against the Beatcloud.",
+    )
+    utils_parser.add_argument(
+        "--local-dirs",
         type=convert_to_paths,
         nargs="+",
         action=NonEmptyListElementAction,
         help="List of local directories to check against the Beatcloud.",
     )
     utils_parser.add_argument(
-        "--check-tracks-spotify-playlists",
+        "--normalize-audio",
+        action="store_true",
+        help='Flag to trigger normalizing audio files at "--local-dirs".',
+    )
+    utils_parser.add_argument(
+        "--normalize-audio-headroom",
+        type=float,
+        help="Amount of headroom in decibels to leave when normalizing audio.",
+    )
+    utils_parser.add_argument(
+        "--process-recording",
+        action="store_true",
+        help=(
+            "Flag to trigger processing an audio recording using a Spotify "
+            "playlist."
+        ),
+    )
+    utils_parser.add_argument(
+        "--recording-file",
+        type=convert_to_paths,
+        help='Audio recording to pair with "--recording-playlist".',
+    )
+    utils_parser.add_argument(
+        "--recording-playlist",
         type=str,
-        nargs="+",
-        help="List of Spotify playlist names to check against the Beatcloud.",
+        help='Spotify playlist to pair with "--recording-file".',
     )
     utils_parser.add_argument(
         "--url-download",
         type=str,
         help="URL to download audio file(s) from.",
     )
     utils_parser.add_argument(
```

### Comparing `djtools-2.6.1b0/djtools/spotify/__init__.py` & `djtools-2.7.0b0/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools/spotify/config.py` & `djtools-2.7.0b0/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools/spotify/helpers.py` & `djtools-2.7.0b0/djtools/spotify/helpers.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools/spotify/playlist_builder.py` & `djtools-2.7.0b0/djtools/spotify/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools/sync/__init__.py` & `djtools-2.7.0b0/djtools/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools/sync/config.py` & `djtools-2.7.0b0/djtools/sync/config.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools/sync/helpers.py` & `djtools-2.7.0b0/djtools/sync/helpers.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools/sync/sync_operations.py` & `djtools-2.7.0b0/djtools/sync/sync_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
         beatcloud_tracks: List of track artist - titles from S3.
     """
     if config.DOWNLOAD_SPOTIFY_PLAYLIST:
         user = config.DOWNLOAD_SPOTIFY_PLAYLIST.split("Uploads")[0].strip()
         beatcloud_tracks, beatcloud_matches = compare_tracks(
             config,
             beatcloud_tracks=beatcloud_tracks,
-            download_spotify_playlist=config.DOWNLOAD_SPOTIFY_PLAYLIST,
         )
         if not beatcloud_matches:
             logger.warning(
                 "No Beatcloud matches were found! Make sure you've supplied "
                 "to correct playlist name."
             )
             return beatcloud_tracks
```

### Comparing `djtools-2.6.1b0/djtools/utils/check_tracks.py` & `djtools-2.7.0b0/djtools/utils/check_tracks.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,58 +18,76 @@
 
 logger = logging.getLogger(__name__)
 
 
 def compare_tracks(
     config: BaseConfig,
     beatcloud_tracks: Optional[List[str]] = None,
-    download_spotify_playlist: Optional[str] = "",
 ) -> Tuple[List[str], List[str]]:
     """Compares tracks from Spotify / local with Beatcloud tracks.
     
     Gets track titles and artists from Spotify playlist(s) and / or file names
     from local directories, and get file names from the beatcloud. Then compute
     the Levenshtein similarity between their product in order to identify any
     overlapping tracks.
 
     Args:
         config: Configuration object.
         beatcloud_tracks: Cached list of tracks from S3.
-        download_spotify_playlist: Override CHECK_TRACKS_SPOTIFY_PLAYLISTS and
-            CHECK_TRACKS_LOCAL_DIRS and use this value instead.
 
     Returns:
         List of all tracks and list of full paths to matching Beatcloud tracks.
     """
-    if download_spotify_playlist:
-        cached_playlists = config.CHECK_TRACKS_SPOTIFY_PLAYLISTS
-        cached_local_dirs = config.CHECK_TRACKS_LOCAL_DIRS
-        config.CHECK_TRACKS_SPOTIFY_PLAYLISTS = [download_spotify_playlist]
-        config.CHECK_TRACKS_LOCAL_DIRS = []
+    if config.DOWNLOAD_SPOTIFY_PLAYLIST:
+        cached_local_dirs = config.LOCAL_DIRS
+        config.LOCAL_DIRS = []
 
     track_sets = []
     beatcloud_matches = []
-    if config.CHECK_TRACKS_SPOTIFY_PLAYLISTS:
-        tracks = get_spotify_tracks(config)
+    spotify_playlists = (
+        [config.DOWNLOAD_SPOTIFY_PLAYLIST]
+        if config.DOWNLOAD_SPOTIFY_PLAYLIST
+        else config.CHECK_TRACKS_SPOTIFY_PLAYLISTS
+    )
+    if spotify_playlists:
+        tracks = get_spotify_tracks(config, spotify_playlists)
         if not tracks:
+            if config.DOWNLOAD_SPOTIFY_PLAYLIST:
+                substring = "DOWNLOAD_SPOTIFY_PLAYLIST is a key"
+            else:
+                substring = (
+                    "CHECK_TRACKS_SPOTIFY_PLAYLISTS has one or more keys"
+                )
             logger.warning(
-                "There are no Spotify tracks; make sure "
-                "CHECK_TRACKS_SPOTIFY_PLAYLISTS has one or more keys from "
+                f"There are no Spotify tracks; make sure {substring} from "
                 "spotify_playlists.yaml"
             )
         else:
+            for playlist_name, playlist_tracks in tracks.items():
+                track_title_artists = []
+                for track in playlist_tracks:
+                    title = track["track"]["name"]
+                    artists = ", ".join([y["name"] for y in track["track"]["artists"]])
+                    track_title_artists.append(
+                        f"{artists} - {title}" if config.ARTIST_FIRST else f"{title} - {artists}"
+                    )
+                tracks[playlist_name] = track_title_artists
             track_sets.append((tracks, "Spotify Playlist Tracks"))
-    if config.CHECK_TRACKS_LOCAL_DIRS:
+    if config.LOCAL_DIRS:
         tracks = get_local_tracks(config)
         if not tracks:
             logger.warning(
-                "There are no local tracks; make sure CHECK_TRACKS_LOCAL_DIRS "
-                'has one or more directories containing one or more tracks'
+                "There are no local tracks; make sure LOCAL_DIRS has one or "
+                "more directories containing one or more tracks"
             )
         else:
+            tracks = {
+                key: [track.stem for track in value]
+                for key, value in tracks.items()
+            }
             track_sets.append((tracks, "Local Directory Tracks"))
 
     if not track_sets:
         return beatcloud_tracks, beatcloud_matches
 
     if not beatcloud_tracks:
         beatcloud_tracks = get_beatcloud_tracks()
@@ -89,12 +107,11 @@
             sorted(matches, key=itemgetter(0)), key=itemgetter(0)
         ):
             logger.info(f"{loc}:")
             for _, track, beatcloud_track, fuzz_ratio in matches:
                 beatcloud_matches.append(path_lookup[beatcloud_track])
                 logger.info(f"\t{fuzz_ratio}: {track} | {beatcloud_track}")
 
-    if download_spotify_playlist:
-        config.CHECK_TRACKS_SPOTIFY_PLAYLISTS = cached_playlists
-        config.CHECK_TRACKS_LOCAL_DIRS = cached_local_dirs
+    if config.DOWNLOAD_SPOTIFY_PLAYLIST:
+        config.LOCAL_DIRS = cached_local_dirs
 
     return beatcloud_tracks, beatcloud_matches
```

### Comparing `djtools-2.6.1b0/djtools/utils/helpers.py` & `djtools-2.7.0b0/djtools/utils/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from itertools import product
 import logging
 import logging.config
 import os
 from pathlib import Path
 from subprocess import check_output
 import tempfile
-from typing import Any, Dict, IO, List, Optional, Set, Tuple
+from typing import Dict, IO, List, Optional, Set, Tuple
 from unittest import mock
 
 from fuzzywuzzy import fuzz
 import spotipy
 from tqdm import tqdm
 
 from djtools.configs.config import BaseConfig
@@ -65,36 +65,14 @@
         data = "{}"
         if self._content:
             data = self._content
 
         return mock.mock_open(read_data=data)(*args, **kwargs)
 
 
-def add_tracks(result: Dict[str, Any], artist_first: bool) -> List[str]:
-    """Parses a page of Spotify API result tracks and returns a list of the
-        track titles and artist names.
-
-    Args:
-        result: Paged result of Spotify tracks.
-        artist_first: Whether or not artist should come before track title.
-
-    Returns:
-        Spotify track titles and artist names.
-    """
-    tracks = []
-    for track in result["items"]:
-        title = track["track"]["name"]
-        artists = ", ".join([y["name"] for y in track["track"]["artists"]])
-        tracks.append(
-            f"{artists} - {title}" if artist_first else f"{title} - {artists}"
-        )
-
-    return tracks
-
-
 def compute_distance(
     spotify_playlist: str,
     spotify_track: str,
     beatcloud_track: str,
     threshold: float,
 ) -> Tuple[str, float]:
     """Qualifies a match between a Spotify track and a beatcloud track using
@@ -186,87 +164,84 @@
     Args:
         config: Configuration object.
 
     Returns:
         Local file names keyed by parent directory.
     """
     local_dir_tracks = {}
-    for _dir in config.CHECK_TRACKS_LOCAL_DIRS:
+    for _dir in config.LOCAL_DIRS:
         if not _dir.exists():
             logger.warning(
                 f"{_dir} does not exist; will not be able to check its "
                 "contents against the beatcloud"
             )
             continue
-        files = [_file.stem for _file in _dir.rglob("**/*.*")]
+        files = list(_dir.rglob("**/*.*"))
         if files:
             local_dir_tracks[_dir] = files
     local_tracks_count = sum(len(x) for x in local_dir_tracks.values())
     logger.info(f"Got {local_tracks_count} files under local directories")
 
     return local_dir_tracks
 
 
 def get_playlist_tracks(
-    spotify: spotipy.Spotify, playlist_id: str, artist_first: bool
-) -> Set[str]:
+    spotify: spotipy.Spotify, playlist_id: str) -> List[Dict]:
     """Queries Spotify API for a playlist and pulls tracks from it.
 
     Args:
         spotify: Spotify client.
         playlist_id: Playlist ID of Spotify playlist to pull tracks from.
-        artist_first: Whether or not artist should come before track title.
 
     Raises:
         RuntimeError: Playlist_id must correspond with a valid Spotify playlist.
 
     Returns:
-        Spotify track titles and artist names from a given playlist.
+        List of Spotify track results.
     """
     try:
         playlist = spotify.playlist(playlist_id)
     except Exception:
         raise RuntimeError(
             f"Failed to get playlist with ID {playlist_id}"
         ) from Exception
 
     result = playlist["tracks"]
-    tracks = add_tracks(result, artist_first)
-
+    tracks = list(result["items"])
     while result["next"]:
         result = spotify.next(result)
-        tracks.extend(add_tracks(result, artist_first))
+        tracks.extend(list(result["items"]))
 
-    return set(tracks)
+    return tracks
 
 
-def get_spotify_tracks(config: BaseConfig) -> Dict[str, Set[str]]:
+def get_spotify_tracks(
+    config: BaseConfig, playlists: List[str]
+) -> Dict[str, List[Dict]]:
     """Aggregates the tracks from one or more Spotify playlists into a
         dictionary mapped with playlist names.
 
     Args:
         config: Configuration object.
+        playlists: List of Spotify playlist name.
     
     Returns:
-        Spotify track titles and artist names keyed by playlist name.
+        Spotify tracks keyed by playlist name.
     """
     spotify = get_spotify_client(config)
     playlist_ids = get_playlist_ids()
 
     playlist_tracks = {}
     _sum = 0
-    for playlist in config.CHECK_TRACKS_SPOTIFY_PLAYLISTS:
+    for playlist in playlists:
         playlist_id = playlist_ids.get(playlist)
         if not playlist_id:
             logger.error(f"{playlist} not in spotify_playlists.yaml")
             continue
-
-        playlist_tracks[playlist] = get_playlist_tracks(
-            spotify, playlist_id, config.ARTIST_FIRST
-        )
+        playlist_tracks[playlist] = get_playlist_tracks(spotify, playlist_id)
         length = len(playlist_tracks[playlist])
         logger.info(
             f'Got {length} track{"" if length == 1 else "s"} from Spotify '
             f'playlist "{playlist}"'
         )
         _sum += length
```

### Comparing `djtools-2.6.1b0/djtools/utils/url_download.py` & `djtools-2.7.0b0/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.1b0/djtools.egg-info/PKG-INFO` & `djtools-2.7.0b0/djtools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djtools
-Version: 2.6.1b0
+Version: 2.7.0b0
 Summary: DJ Tools is a library for managing a collection of music.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 Keywords: DJ Rekordbox spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -31,21 +31,23 @@
 # DJ Tools
 [![image](https://img.shields.io/pypi/v/djtools.svg)](https://pypi.org/project/djtools/)
 
 Please see the [docs](https://a-rich.github.io/DJ-Tools/) for tutorials, how-to guides, conceptual guides, and references!
 
 # Release Plan
 * 2.6.1
+    - [ ] [Stability issues with requests to the search endpoint of the Spotify API](https://github.com/a-rich/DJ-Tools/issues/58)
+    - [ ] [Make Spotify API calls asynchronous](https://github.com/a-rich/DJ-Tools/issues/38)
+* 2.7.0
     - [x] Script for removing situation tags and resolving album, label, and year for tracks
     - [x] Allow `build_config` to accept an override for the path to `config.yaml`
     - [x] Fix missing typehints for the `NonEmptyListElementAction` class
     - [x] [Make PlaylistFilter implementations configurable](https://github.com/a-rich/DJ-Tools/issues/120)
     - [x] [Make MinimalDeepTechFilter more robust to the relative position of House and Techno tags](https://github.com/a-rich/DJ-Tools/issues/122)
-    - [ ] [Stability issues with requests to the search endpoint of the Spotify API](https://github.com/a-rich/DJ-Tools/issues/58)
-    - [ ] [Make Spotify API calls asynchronous](https://github.com/a-rich/DJ-Tools/issues/38)
-* 2.7.0
-    - [ ] [Improve Reddit submission title parsing in order to improve precision and recall of Spotify API search results](https://github.com/a-rich/DJ-Tools/issues/59)
-    - [ ] [Derive boolean algebra expressions that generate a given playlist](https://github.com/a-rich/DJ-Tools/issues/106)
+    - [x] [Standardize audio files](https://github.com/a-rich/DJ-Tools/issues/126)
+    - [x] [Process recorded file using Spotify playlist](https://github.com/a-rich/DJ-Tools/issues/127)
     - [ ] [Create graphic user interface for djtools](https://github.com/a-rich/DJ-Tools/issues/118)
+    - [ ] [Derive boolean algebra expressions that generate a given playlist](https://github.com/a-rich/DJ-Tools/issues/106)
+    - [ ] [Improve Reddit submission title parsing in order to improve precision and recall of Spotify API search results](https://github.com/a-rich/DJ-Tools/issues/59)
 
 # Contribution
 Please see the [CONTRIBUTING](CONTRIBUTING.md)
```

### Comparing `djtools-2.6.1b0/djtools.egg-info/SOURCES.txt` & `djtools-2.7.0b0/djtools.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -38,8 +38,10 @@
 djtools/sync/config.py
 djtools/sync/helpers.py
 djtools/sync/sync_operations.py
 djtools/utils/__init__.py
 djtools/utils/check_tracks.py
 djtools/utils/config.py
 djtools/utils/helpers.py
+djtools/utils/normalize_audio.py
+djtools/utils/process_recording.py
 djtools/utils/url_download.py
```

### Comparing `djtools-2.6.1b0/setup.py` & `djtools-2.7.0b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 REQUIREMENTS = [
     "asyncpraw==7.6.1",
     "awscli==1.27.45",
     "beautifulsoup4==4.11.1",
     "fuzzywuzzy==0.18.0",
     "lxml==4.9.2",
     "pydantic==1.9.1",
+    "pydub==0.25.1",
     "pyperclip==1.8.2",
     "PyYAML==5.4.1",
     "requests==2.28.0",
     "setuptools==58.1.0",
     "spotipy==2.21.0",
     "tqdm==4.64.0",
     "youtube-dl==2021.12.17",
```

