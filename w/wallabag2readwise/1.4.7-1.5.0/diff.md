# Comparing `tmp/wallabag2readwise-1.4.7.tar.gz` & `tmp/wallabag2readwise-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wallabag2readwise-1.4.7.tar", last modified: Mon May  1 20:01:11 2023, max compression
+gzip compressed data, was "wallabag2readwise-1.5.0.tar", last modified: Sat Jul 29 20:04:40 2023, max compression
```

## Comparing `wallabag2readwise-1.4.7.tar` & `wallabag2readwise-1.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:01:11.022897 wallabag2readwise-1.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-01 20:01:11.022897 wallabag2readwise-1.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 20:01:11.022897 wallabag2readwise-1.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:01:11.018897 wallabag2readwise-1.4.7/wallabag2readwise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/wallabag2readwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/wallabag2readwise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/wallabag2readwise/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/wallabag2readwise/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/wallabag2readwise/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/wallabag2readwise/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/wallabag2readwise/output.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/wallabag2readwise/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/wallabag2readwise/wallabag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:01:11.022897 wallabag2readwise-1.4.7/wallabag2readwise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-01 20:01:11.000000 wallabag2readwise-1.4.7/wallabag2readwise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-01 20:01:11.000000 wallabag2readwise-1.4.7/wallabag2readwise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:01:11.000000 wallabag2readwise-1.4.7/wallabag2readwise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-01 20:01:11.000000 wallabag2readwise-1.4.7/wallabag2readwise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-01 20:01:11.000000 wallabag2readwise-1.4.7/wallabag2readwise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 20:01:11.000000 wallabag2readwise-1.4.7/wallabag2readwise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:04:40.582051 wallabag2readwise-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-29 20:04:37.000000 wallabag2readwise-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-29 20:04:40.582051 wallabag2readwise-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-29 20:04:37.000000 wallabag2readwise-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 20:04:40.582051 wallabag2readwise-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-29 20:04:37.000000 wallabag2readwise-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:04:40.582051 wallabag2readwise-1.5.0/wallabag2readwise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 20:04:37.000000 wallabag2readwise-1.5.0/wallabag2readwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-29 20:04:37.000000 wallabag2readwise-1.5.0/wallabag2readwise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-07-29 20:04:37.000000 wallabag2readwise-1.5.0/wallabag2readwise/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-29 20:04:37.000000 wallabag2readwise-1.5.0/wallabag2readwise/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-07-29 20:04:37.000000 wallabag2readwise-1.5.0/wallabag2readwise/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-29 20:04:37.000000 wallabag2readwise-1.5.0/wallabag2readwise/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-29 20:04:37.000000 wallabag2readwise-1.5.0/wallabag2readwise/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-29 20:04:37.000000 wallabag2readwise-1.5.0/wallabag2readwise/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-29 20:04:37.000000 wallabag2readwise-1.5.0/wallabag2readwise/wallabag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:04:40.582051 wallabag2readwise-1.5.0/wallabag2readwise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-29 20:04:40.000000 wallabag2readwise-1.5.0/wallabag2readwise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-29 20:04:40.000000 wallabag2readwise-1.5.0/wallabag2readwise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 20:04:40.000000 wallabag2readwise-1.5.0/wallabag2readwise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-29 20:04:40.000000 wallabag2readwise-1.5.0/wallabag2readwise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-29 20:04:40.000000 wallabag2readwise-1.5.0/wallabag2readwise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 20:04:40.000000 wallabag2readwise-1.5.0/wallabag2readwise.egg-info/top_level.txt
```

### Comparing `wallabag2readwise-1.4.7/LICENSE` & `wallabag2readwise-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wallabag2readwise-1.4.7/PKG-INFO` & `wallabag2readwise-1.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wallabag2readwise
-Version: 1.4.7
+Version: 1.5.0
 Summary: Push wallabag annotations to Readwise highlights
 Home-page: https://github.com/rwxd/wallabag2readwise
 Author: rwxd
 Author-email: rwxd@pm.me
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -83,20 +83,26 @@
 Run continuously and push new annotations to Readwise every 60 minutes.
 (The container is automatically in daemon mode.)
 
 ```bash
 wallabag2readwise daemon --wait-time 60
 ```
 
-#### Import all Wallabag entries to Readwise reader
+#### Import all Wallabag entries to Readwise Reader
 
 ```bash
 wallabag2readwise reader
 ```
 
+#### Import all Readwise Reader Documents to Wallabag
+
+```bash
+wallabag2readwise wallabag
+```
+
 ### Configuration
 
 Get a new Readwise API Token from <https://readwise.io/access_token>.
 
 Create a new wallabag API client in your instance <https://my-wallabag.com/developer/client/create>.
 
 #### ENV Vars
```

### Comparing `wallabag2readwise-1.4.7/README.md` & `wallabag2readwise-1.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -69,20 +69,26 @@
 Run continuously and push new annotations to Readwise every 60 minutes.
 (The container is automatically in daemon mode.)
 
 ```bash
 wallabag2readwise daemon --wait-time 60
 ```
 
-#### Import all Wallabag entries to Readwise reader
+#### Import all Wallabag entries to Readwise Reader
 
 ```bash
 wallabag2readwise reader
 ```
 
+#### Import all Readwise Reader Documents to Wallabag
+
+```bash
+wallabag2readwise wallabag
+```
+
 ### Configuration
 
 Get a new Readwise API Token from <https://readwise.io/access_token>.
 
 Create a new wallabag API client in your instance <https://my-wallabag.com/developer/client/create>.
 
 #### ENV Vars
```

### Comparing `wallabag2readwise-1.4.7/setup.py` & `wallabag2readwise-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `wallabag2readwise-1.4.7/wallabag2readwise/misc.py` & `wallabag2readwise-1.5.0/wallabag2readwise/misc.py`

 * *Files identical despite different names*

### Comparing `wallabag2readwise-1.4.7/wallabag2readwise/models.py` & `wallabag2readwise-1.5.0/wallabag2readwise/models.py`

 * *Files identical despite different names*

### Comparing `wallabag2readwise-1.4.7/wallabag2readwise/wallabag.py` & `wallabag2readwise-1.5.0/wallabag2readwise/wallabag.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
                 'grant_type': 'password',
                 'client_id': self.client_id,
                 'client_secret': self.client_secret,
                 'username': self.user,
                 'password': self.password,
             },
         )
+        response.raise_for_status()
         data = response.json()
         return data['access_token']
 
     def get(self, endpoint: str, params: dict = {}) -> requests.Response:
         url = self.url + endpoint
         logger.debug(f'Getting "{url}" with params: {params}')
         response = self._session.get(url, params=params)
@@ -90,7 +91,12 @@
             yield WallabagAnnotation(
                 id=item['id'],
                 text=item['text'],
                 quote=item['quote'],
                 created_at=datetime.strptime(item['created_at'], '%y-%m-%dT%H:%M+%S'),
                 ranges=item['ranges'],
             )
+
+    def create_entry(self, url: str, params: dict = {}):
+        params.update({'url': url})
+        result = self.post('/api/entries.json', data=params)
+        result.raise_for_status()
```

### Comparing `wallabag2readwise-1.4.7/wallabag2readwise.egg-info/PKG-INFO` & `wallabag2readwise-1.5.0/wallabag2readwise.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wallabag2readwise
-Version: 1.4.7
+Version: 1.5.0
 Summary: Push wallabag annotations to Readwise highlights
 Home-page: https://github.com/rwxd/wallabag2readwise
 Author: rwxd
 Author-email: rwxd@pm.me
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -83,20 +83,26 @@
 Run continuously and push new annotations to Readwise every 60 minutes.
 (The container is automatically in daemon mode.)
 
 ```bash
 wallabag2readwise daemon --wait-time 60
 ```
 
-#### Import all Wallabag entries to Readwise reader
+#### Import all Wallabag entries to Readwise Reader
 
 ```bash
 wallabag2readwise reader
 ```
 
+#### Import all Readwise Reader Documents to Wallabag
+
+```bash
+wallabag2readwise wallabag
+```
+
 ### Configuration
 
 Get a new Readwise API Token from <https://readwise.io/access_token>.
 
 Create a new wallabag API client in your instance <https://my-wallabag.com/developer/client/create>.
 
 #### ENV Vars
```

### Comparing `wallabag2readwise-1.4.7/wallabag2readwise.egg-info/SOURCES.txt` & `wallabag2readwise-1.5.0/wallabag2readwise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

