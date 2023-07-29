# Comparing `tmp/proxy.py-uxspoilers-plugin-2021.5.18.post1.tar.gz` & `tmp/proxy.py-uxspoilers-plugin-2021.5.18.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxy.py-uxspoilers-plugin-2021.5.18.post1.tar", last modified: Sat Jul 29 10:11:30 2023, max compression
+gzip compressed data, was "proxy.py-uxspoilers-plugin-2021.5.18.post2.tar", last modified: Sat Jul 29 10:15:01 2023, max compression
```

## Comparing `proxy.py-uxspoilers-plugin-2021.5.18.post1.tar` & `proxy.py-uxspoilers-plugin-2021.5.18.post2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:11:30.806578 proxy.py-uxspoilers-plugin-2021.5.18.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-29 10:11:19.000000 proxy.py-uxspoilers-plugin-2021.5.18.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-29 10:11:30.806578 proxy.py-uxspoilers-plugin-2021.5.18.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-29 10:11:19.000000 proxy.py-uxspoilers-plugin-2021.5.18.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:11:30.806578 proxy.py-uxspoilers-plugin-2021.5.18.post1/proxy.py_uxspoilers_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-29 10:11:30.000000 proxy.py-uxspoilers-plugin-2021.5.18.post1/proxy.py_uxspoilers_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-29 10:11:30.000000 proxy.py-uxspoilers-plugin-2021.5.18.post1/proxy.py_uxspoilers_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:11:30.000000 proxy.py-uxspoilers-plugin-2021.5.18.post1/proxy.py_uxspoilers_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 10:11:30.000000 proxy.py-uxspoilers-plugin-2021.5.18.post1/proxy.py_uxspoilers_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 10:11:30.000000 proxy.py-uxspoilers-plugin-2021.5.18.post1/proxy.py_uxspoilers_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-29 10:11:30.806578 proxy.py-uxspoilers-plugin-2021.5.18.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-29 10:11:19.000000 proxy.py-uxspoilers-plugin-2021.5.18.post1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-29 10:11:19.000000 proxy.py-uxspoilers-plugin-2021.5.18.post1/uxspoilers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:15:01.460741 proxy.py-uxspoilers-plugin-2021.5.18.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-29 10:14:53.000000 proxy.py-uxspoilers-plugin-2021.5.18.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-29 10:15:01.460741 proxy.py-uxspoilers-plugin-2021.5.18.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-29 10:14:53.000000 proxy.py-uxspoilers-plugin-2021.5.18.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:15:01.460741 proxy.py-uxspoilers-plugin-2021.5.18.post2/proxy.py_uxspoilers_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-29 10:15:01.000000 proxy.py-uxspoilers-plugin-2021.5.18.post2/proxy.py_uxspoilers_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-29 10:15:01.000000 proxy.py-uxspoilers-plugin-2021.5.18.post2/proxy.py_uxspoilers_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:15:01.000000 proxy.py-uxspoilers-plugin-2021.5.18.post2/proxy.py_uxspoilers_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 10:15:01.000000 proxy.py-uxspoilers-plugin-2021.5.18.post2/proxy.py_uxspoilers_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 10:15:01.000000 proxy.py-uxspoilers-plugin-2021.5.18.post2/proxy.py_uxspoilers_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-29 10:15:01.464741 proxy.py-uxspoilers-plugin-2021.5.18.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-29 10:14:53.000000 proxy.py-uxspoilers-plugin-2021.5.18.post2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-29 10:14:53.000000 proxy.py-uxspoilers-plugin-2021.5.18.post2/uxspoilers.py
```

### Comparing `proxy.py-uxspoilers-plugin-2021.5.18.post1/LICENSE` & `proxy.py-uxspoilers-plugin-2021.5.18.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `proxy.py-uxspoilers-plugin-2021.5.18.post1/PKG-INFO` & `proxy.py-uxspoilers-plugin-2021.5.18.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxy.py-uxspoilers-plugin
-Version: 2021.5.18.post1
+Version: 2021.5.18.post2
 Home-page: https://github.com/sakurai-youhei/proxy.py-uxspoilers-plugin
 Author: Youhei Sakurai
 Author-email: sakurai.youhei@gmail.com
 Maintainer: Youhei Sakurai
 Maintainer-email: sakurai.youhei@gmail.com
 License: MIT
 Platform: any
```

### Comparing `proxy.py-uxspoilers-plugin-2021.5.18.post1/README.md` & `proxy.py-uxspoilers-plugin-2021.5.18.post2/README.md`

 * *Files identical despite different names*

### Comparing `proxy.py-uxspoilers-plugin-2021.5.18.post1/proxy.py_uxspoilers_plugin.egg-info/PKG-INFO` & `proxy.py-uxspoilers-plugin-2021.5.18.post2/proxy.py_uxspoilers_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxy.py-uxspoilers-plugin
-Version: 2021.5.18.post1
+Version: 2021.5.18.post2
 Home-page: https://github.com/sakurai-youhei/proxy.py-uxspoilers-plugin
 Author: Youhei Sakurai
 Author-email: sakurai.youhei@gmail.com
 Maintainer: Youhei Sakurai
 Maintainer-email: sakurai.youhei@gmail.com
 License: MIT
 Platform: any
```

### Comparing `proxy.py-uxspoilers-plugin-2021.5.18.post1/setup.py` & `proxy.py-uxspoilers-plugin-2021.5.18.post2/setup.py`

 * *Files identical despite different names*

### Comparing `proxy.py-uxspoilers-plugin-2021.5.18.post1/uxspoilers.py` & `proxy.py-uxspoilers-plugin-2021.5.18.post2/uxspoilers.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Optional
 
 from proxy.common.flag import flags
 from proxy.http.parser import HttpParser
 from proxy.http.proxy import HttpProxyBasePlugin
 
 
-__version__ = "2021.5.18.post1"
+__version__ = "2021.5.18.post2"
 
 
 flags.add_argument('--pause-seconds',
                    type=float,
                    default=1.0,
                    help=('Default: 1.0.  Flag only applicable when '
                          'FixedRustyPumpPlugin is used for spoiling UX.'))
```

