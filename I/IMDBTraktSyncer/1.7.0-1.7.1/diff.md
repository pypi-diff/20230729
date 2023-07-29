# Comparing `tmp/IMDBTraktSyncer-1.7.0.tar.gz` & `tmp/IMDBTraktSyncer-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.7.0.tar", last modified: Sat Jul 29 10:47:31 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.7.1.tar", last modified: Sat Jul 29 12:04:50 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.7.0.tar` & `IMDBTraktSyncer-1.7.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 10:47:31.735836 IMDBTraktSyncer-1.7.0/
-drwxrwxrwx   0        0        0        0 2023-07-29 10:47:31.700848 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    40858 2023-07-29 10:44:06.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4624 2023-06-19 09:47:47.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4317 2023-06-19 09:47:23.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     6946 2023-06-27 06:49:08.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     1669 2023-06-25 00:09:11.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/errorLogger.py
--rw-rw-rw-   0        0        0    11362 2023-07-29 10:06:33.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0    10572 2023-07-29 08:41:16.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0    12192 2023-06-19 15:47:42.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:47:31.733846 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    12719 2023-07-29 10:47:31.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-07-29 10:47:31.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 10:47:31.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-07-29 10:47:31.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-07-29 10:47:31.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-29 10:47:31.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.7.0/LICENSE
--rw-rw-rw-   0        0        0    12719 2023-07-29 10:47:31.734845 IMDBTraktSyncer-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0    11972 2023-07-29 10:46:05.000000 IMDBTraktSyncer-1.7.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-29 10:47:31.735836 IMDBTraktSyncer-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1377 2023-07-29 10:46:25.000000 IMDBTraktSyncer-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 12:04:50.103719 IMDBTraktSyncer-1.7.1/
+drwxrwxrwx   0        0        0        0 2023-07-29 12:04:50.069297 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    41112 2023-07-29 12:00:01.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4624 2023-06-19 09:47:47.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4317 2023-06-19 09:47:23.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     6946 2023-06-27 06:49:08.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     1669 2023-06-25 00:09:11.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/errorLogger.py
+-rw-rw-rw-   0        0        0    11362 2023-07-29 10:06:33.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0    10572 2023-07-29 08:41:16.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0    12192 2023-06-19 15:47:42.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-07-29 12:04:50.100708 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    12719 2023-07-29 12:04:49.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-07-29 12:04:49.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 12:04:49.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-07-29 12:04:49.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-07-29 12:04:49.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-29 12:04:49.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.7.1/LICENSE
+-rw-rw-rw-   0        0        0    12719 2023-07-29 12:04:50.102708 IMDBTraktSyncer-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11972 2023-07-29 10:46:05.000000 IMDBTraktSyncer-1.7.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-29 12:04:50.103719 IMDBTraktSyncer-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2023-07-29 12:04:16.000000 IMDBTraktSyncer-1.7.1/setup.py
```

### Comparing `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,19 +149,21 @@
         for imdb_id, imdb_rating in imdb_ratings_dict.items():
             if imdb_id in trakt_ratings_dict:
                 trakt_rating = trakt_ratings_dict[imdb_id]
                 if imdb_rating['Rating'] != trakt_rating['Rating']:
                     imdb_date_added = datetime.fromisoformat(imdb_rating['Date_Added'])
                     trakt_date_added = datetime.fromisoformat(trakt_rating['Date_Added'])
                     
-                    # If IMDB rating is more recent, add the Trakt rating to the update list, and vice versa
-                    if imdb_date_added > trakt_date_added:
-                        trakt_ratings_to_update.append(imdb_rating)
-                    else:
-                        imdb_ratings_to_update.append(trakt_rating)
+                    # Check if ratings were added on different days
+                    if (imdb_date_added.year, imdb_date_added.month, imdb_date_added.day) != (trakt_date_added.year, trakt_date_added.month, trakt_date_added.day):
+                        # If IMDB rating is more recent, add the Trakt rating to the update list, and vice versa
+                        if imdb_date_added > trakt_date_added:
+                            trakt_ratings_to_update.append(imdb_rating)
+                        else:
+                            imdb_ratings_to_update.append(trakt_rating)
 
         # Update ratings_to_set
         imdb_ratings_to_set.extend(imdb_ratings_to_update)
         trakt_ratings_to_set.extend(trakt_ratings_to_update)
         
         # Filter out review items where the comment length is less than 600 characters
         def filter_by_comment_length(lst, min_comment_length=None):
```

### Comparing `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/errorLogger.py` & `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/errorLogger.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/imdbData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.7.0
+Version: 1.7.1
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.0/LICENSE` & `IMDBTraktSyncer-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.0/PKG-INFO` & `IMDBTraktSyncer-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.7.0
+Version: 1.7.1
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.7.0/README.md` & `IMDBTraktSyncer-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.0/setup.py` & `IMDBTraktSyncer-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.7.0'
+VERSION = '1.7.1'
 DESCRIPTION = 'A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

