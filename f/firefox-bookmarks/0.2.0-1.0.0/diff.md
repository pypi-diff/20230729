# Comparing `tmp/firefox_bookmarks-0.2.0.tar.gz` & `tmp/firefox_bookmarks-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firefox_bookmarks-0.2.0.tar", max compression
+gzip compressed data, was "firefox_bookmarks-1.0.0.tar", max compression
```

## Comparing `firefox_bookmarks-0.2.0.tar` & `firefox_bookmarks-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      420 2023-07-23 11:43:23.291314 firefox_bookmarks-0.2.0/firefox_bookmarks/__init__.py
--rw-r--r--   0        0        0     1175 2023-07-23 11:43:23.293750 firefox_bookmarks-0.2.0/firefox_bookmarks/connect.py
--rw-r--r--   0        0        0      276 2023-07-22 14:07:55.049329 firefox_bookmarks-0.2.0/firefox_bookmarks/constants.py
--rw-r--r--   0        0        0     2280 2023-07-22 14:10:44.937368 firefox_bookmarks-0.2.0/firefox_bookmarks/locate.py
--rw-r--r--   0        0        0     3771 2023-07-23 11:43:23.295826 firefox_bookmarks-0.2.0/firefox_bookmarks/models.py
--rw-r--r--   0        0        0    35184 2023-07-21 16:18:12.325494 firefox_bookmarks-0.2.0/LICENSE
--rw-r--r--   0        0        0     1235 2023-07-23 11:43:48.655434 firefox_bookmarks-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      616 2023-07-23 08:35:10.919927 firefox_bookmarks-0.2.0/README.md
--rw-r--r--   0        0        0     1910 1970-01-01 00:00:00.000000 firefox_bookmarks-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    19028 2023-07-29 20:13:57.122984 firefox_bookmarks-1.0.0/firefox_bookmarks/__init__.py
+-rw-r--r--   0        0        0     4451 2023-07-29 20:13:57.138108 firefox_bookmarks-1.0.0/firefox_bookmarks/bookmark.py
+-rw-r--r--   0        0        0     1268 2023-07-25 08:53:37.841063 firefox_bookmarks-1.0.0/firefox_bookmarks/connect.py
+-rw-r--r--   0        0        0      437 2023-07-29 20:50:08.340724 firefox_bookmarks-1.0.0/firefox_bookmarks/constants.py
+-rw-r--r--   0        0        0     2391 2023-07-24 14:39:36.813164 firefox_bookmarks-1.0.0/firefox_bookmarks/locate.py
+-rw-r--r--   0        0        0     3974 2023-07-29 20:13:57.164801 firefox_bookmarks-1.0.0/firefox_bookmarks/models.py
+-rw-r--r--   0        0        0    35184 2023-07-21 16:18:12.325494 firefox_bookmarks-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1417 2023-07-29 20:48:57.651905 firefox_bookmarks-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2503 2023-07-29 20:39:23.972578 firefox_bookmarks-1.0.0/README.md
+-rw-r--r--   0        0        0     3921 1970-01-01 00:00:00.000000 firefox_bookmarks-1.0.0/PKG-INFO
```

### Comparing `firefox_bookmarks-0.2.0/firefox_bookmarks/connect.py` & `firefox_bookmarks-1.0.0/firefox_bookmarks/connect.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,7 +30,13 @@
     if database is None:
         database = SqliteDatabase(db_path)
     else:
         database.init(db_path)
     database.connect(reuse_if_open=True)
 
     return database
+
+
+__all__ = [
+    'connect_to_places_db',
+    'ProfileCriterion',  # For convenience
+]
```

### Comparing `firefox_bookmarks-0.2.0/firefox_bookmarks/locate.py` & `firefox_bookmarks-1.0.0/firefox_bookmarks/locate.py`

 * *Files 9% similar despite different names*

```diff
@@ -66,7 +66,14 @@
 
 def _last_modified(file_path: str) -> float:
     return os.path.getmtime(file_path)
 
 
 def _file_size(file_path: str) -> float:
     return os.path.getsize(file_path)
+
+
+__all__ = [
+    'locate_db',
+    'locate_db_candidates',
+    'ProfileCriterion',  # For convenience
+]
```

### Comparing `firefox_bookmarks-0.2.0/firefox_bookmarks/models.py` & `firefox_bookmarks-1.0.0/firefox_bookmarks/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from .constants import ProfileCriterion
 
 database_obj = SqliteDatabase(None)
 
 
 class _BaseModel(Model):
+    id = IntegerField(primary_key=True)
 
     class Meta:
         database = database_obj
 
 
 class FirefoxOrigin(_BaseModel):
     """Represents an entry in the `moz_origins` table"""
@@ -108,7 +109,16 @@
     from .connect import connect_to_places_db
 
     connect_to_places_db(
         database=database_obj,
         look_under_path=look_under_path,
         criterion=criterion,
     )
+
+
+__all__ = [
+    'connect_firefox_models',
+    'FirefoxBookmark',
+    'FirefoxPlace',
+    'FirefoxOrigin',
+    'ProfileCriterion',  # For convenience
+]
```

### Comparing `firefox_bookmarks-0.2.0/LICENSE` & `firefox_bookmarks-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `firefox_bookmarks-0.2.0/pyproject.toml` & `firefox_bookmarks-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 [tool.poetry]
 name = "firefox-bookmarks"
-version = "0.2.0"
+version = "1.0.0"
 description = "Manage your Firefox bookmarks with ease"
 authors = ["Aditya Rajput <adiraj20072002@gmail.com>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
-packages = [{include = "firefox_bookmarks"}]
+packages = [{ include = "firefox_bookmarks" }]
 repository = "https://github.com/BURG3R5/firefox-bookmarks"
 documentation = "https://github.com/BURG3R5/firefox-bookmarks"
 keywords = ["firefox", "bookmarks", "browser", "util"]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "Natural Language :: English",
     "Operating System :: Microsoft :: Windows :: Windows 10",
+    "Operating System :: Microsoft :: Windows :: Windows 11",
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux",
     "Topic :: Database",
     "Topic :: Internet :: WWW/HTTP :: Browsers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
 ]
 
+[tool.poetry.urls]
+Changelog = "https://github.com/BURG3R5/firefox-bookmarks/blob/main/CHANGELOG.md"
+
 [tool.poetry.dependencies]
 python = "^3.10"
 peewee = "^3.16.2"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.2.7"
 pre-commit = "^3.3.3"
```

