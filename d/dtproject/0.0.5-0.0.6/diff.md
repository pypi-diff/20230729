# Comparing `tmp/dtproject-0.0.5.tar.gz` & `tmp/dtproject-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtproject-0.0.5.tar", last modified: Wed Apr 26 13:48:24 2023, max compression
+gzip compressed data, was "dtproject-0.0.6.tar", last modified: Sat Jul 29 09:55:46 2023, max compression
```

## Comparing `dtproject-0.0.5.tar` & `dtproject-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-26 13:48:24.826359 dtproject-0.0.5/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      424 2023-04-26 13:48:24.826359 dtproject-0.0.5/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-04-26 13:48:24.826359 dtproject-0.0.5/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1765 2023-04-26 13:48:11.000000 dtproject-0.0.5/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-26 13:48:24.822359 dtproject-0.0.5/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-26 13:48:24.822359 dtproject-0.0.5/src/dtproject/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      163 2023-04-26 13:48:18.000000 dtproject-0.0.5/src/dtproject/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      418 2023-04-19 22:08:11.000000 dtproject-0.0.5/src/dtproject/configurations.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6721 2023-04-26 13:47:21.000000 dtproject-0.0.5/src/dtproject/constants.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    25965 2023-04-21 03:36:57.000000 dtproject-0.0.5/src/dtproject/dtproject.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      480 2023-04-20 03:25:31.000000 dtproject-0.0.5/src/dtproject/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6316 2023-04-20 03:28:28.000000 dtproject-0.0.5/src/dtproject/recipe.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-26 13:48:24.826359 dtproject-0.0.5/src/dtproject/utils/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 02:38:03.000000 dtproject-0.0.5/src/dtproject/utils/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1326 2023-04-20 14:46:26.000000 dtproject-0.0.5/src/dtproject/utils/docker.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1198 2023-04-20 03:17:17.000000 dtproject-0.0.5/src/dtproject/utils/misc.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-26 13:48:24.826359 dtproject-0.0.5/src/dtproject.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      424 2023-04-26 13:48:24.000000 dtproject-0.0.5/src/dtproject.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      446 2023-04-26 13:48:24.000000 dtproject-0.0.5/src/dtproject.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-04-26 13:48:24.000000 dtproject-0.0.5/src/dtproject.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       27 2023-04-26 13:48:24.000000 dtproject-0.0.5/src/dtproject.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       10 2023-04-26 13:48:24.000000 dtproject-0.0.5/src/dtproject.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-29 09:55:46.523868 dtproject-0.0.6/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      424 2023-07-29 09:55:46.523868 dtproject-0.0.6/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-07-29 09:55:46.523868 dtproject-0.0.6/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1765 2023-04-26 13:48:11.000000 dtproject-0.0.6/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-29 09:55:46.523868 dtproject-0.0.6/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-29 09:55:46.523868 dtproject-0.0.6/src/dtproject/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      163 2023-07-29 09:53:03.000000 dtproject-0.0.6/src/dtproject/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      418 2023-04-19 22:08:11.000000 dtproject-0.0.6/src/dtproject/configurations.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7003 2023-07-29 09:52:21.000000 dtproject-0.0.6/src/dtproject/constants.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    25965 2023-04-21 03:36:57.000000 dtproject-0.0.6/src/dtproject/dtproject.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      480 2023-04-20 03:25:31.000000 dtproject-0.0.6/src/dtproject/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6316 2023-04-20 03:28:28.000000 dtproject-0.0.6/src/dtproject/recipe.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-29 09:55:46.523868 dtproject-0.0.6/src/dtproject/utils/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 02:38:03.000000 dtproject-0.0.6/src/dtproject/utils/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1326 2023-04-20 14:46:26.000000 dtproject-0.0.6/src/dtproject/utils/docker.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1198 2023-04-20 03:17:17.000000 dtproject-0.0.6/src/dtproject/utils/misc.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-29 09:55:46.523868 dtproject-0.0.6/src/dtproject.egg-info/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      424 2023-07-29 09:55:46.000000 dtproject-0.0.6/src/dtproject.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      446 2023-07-29 09:55:46.000000 dtproject-0.0.6/src/dtproject.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-07-29 09:55:46.000000 dtproject-0.0.6/src/dtproject.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       27 2023-07-29 09:55:46.000000 dtproject-0.0.6/src/dtproject.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       10 2023-07-29 09:55:46.000000 dtproject-0.0.6/src/dtproject.egg-info/top_level.txt
```

### Comparing `dtproject-0.0.5/setup.py` & `dtproject-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `dtproject-0.0.5/src/dtproject/constants.py` & `dtproject-0.0.6/src/dtproject/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,19 +57,21 @@
                       Dict[ProjectTypeVersion,
                            Callable[[ProjectName], Tuple[RelativePath, ContainerPath]]]] = {
     # NOTE: these are not templates, they only serve the project matching their names
     "dt-commons": {
         "1": lambda _repo: ("code", "/packages/{:s}/".format(_repo)),
         "2": lambda _repo: ("", "/code/{:s}/".format(_repo)),
         "3": lambda _repo: ("", "/code/{:s}/".format(_repo)),
+        "4": lambda _repo: ("", "/code/{:s}/".format(_repo)),
     },
     "dt-ros-commons": {
         "1": lambda _repo: ("", "/code/catkin_ws/src/{:s}/".format(_repo)),
         "2": lambda _repo: ("", "/code/catkin_ws/src/{:s}/".format(_repo)),
         "3": lambda _repo: ("", "/code/catkin_ws/src/{:s}/".format(_repo)),
+        "4": lambda _repo: ("", "/code/catkin_ws/src/{:s}/".format(_repo)),
     },
     # NOTE: these are templates and are shared by multiple projects
     "template-basic": {
         "1": lambda _repo: ("code", "/packages/{:s}/".format(_repo)),
         "2": lambda _repo: ("", "/code/{:s}/".format(_repo)),
         "3": lambda _repo: ("", "/code/{:s}/".format(_repo)),
         "4": lambda _repo: ("", "/code/{:s}/".format(_repo)),
@@ -96,19 +98,21 @@
                              Dict[ProjectTypeVersion,
                                   Callable[[ProjectName], Tuple[RelativePath, ContainerPath]]]] = {
     # NOTE: these are not templates, they only serve the project matching their names
     "dt-commons": {
         "1": lambda _repo: ("launch.sh", "/launch/{:s}/launch.sh".format(_repo)),
         "2": lambda _repo: ("launchers", "/launch/{:s}".format(_repo)),
         "3": lambda _repo: ("launchers", "/launch/{:s}".format(_repo)),
+        "4": lambda _repo: ("launchers", "/launch/{:s}".format(_repo)),
     },
     "dt-ros-commons": {
         "1": lambda _repo: ("launch.sh", "/launch/{:s}/launch.sh".format(_repo)),
         "2": lambda _repo: ("launchers", "/launch/{:s}".format(_repo)),
         "3": lambda _repo: ("launchers", "/launch/{:s}".format(_repo)),
+        "4": lambda _repo: ("launchers", "/launch/{:s}".format(_repo)),
     },
     # NOTE: these are templates and are shared by multiple projects
     "template-basic": {
         "1": lambda _repo: ("launch.sh", "/launch/{:s}/launch.sh".format(_repo)),
         "2": lambda _repo: ("launchers", "/launch/{:s}".format(_repo)),
         "3": lambda _repo: ("launchers", "/launch/{:s}".format(_repo)),
         "4": lambda _repo: ("launchers", "/launch/{:s}".format(_repo)),
```

### Comparing `dtproject-0.0.5/src/dtproject/dtproject.py` & `dtproject-0.0.6/src/dtproject/dtproject.py`

 * *Files identical despite different names*

### Comparing `dtproject-0.0.5/src/dtproject/recipe.py` & `dtproject-0.0.6/src/dtproject/recipe.py`

 * *Files identical despite different names*

### Comparing `dtproject-0.0.5/src/dtproject/utils/docker.py` & `dtproject-0.0.6/src/dtproject/utils/docker.py`

 * *Files identical despite different names*

### Comparing `dtproject-0.0.5/src/dtproject/utils/misc.py` & `dtproject-0.0.6/src/dtproject/utils/misc.py`

 * *Files identical despite different names*

