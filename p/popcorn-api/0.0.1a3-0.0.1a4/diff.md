# Comparing `tmp/popcorn_api-0.0.1a3.tar.gz` & `tmp/popcorn_api-0.0.1a4.tar.gz`

## Comparing `popcorn_api-0.0.1a3.tar` & `popcorn_api-0.0.1a4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 popcorn_api-0.0.1a3/src/.python-version
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 popcorn_api-0.0.1a3/src/popcorn_api/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 popcorn_api-0.0.1a3/src/popcorn_api/config.json
--rw-r--r--   0        0        0     8583 2020-02-02 00:00:00.000000 popcorn_api-0.0.1a3/src/popcorn_api/popcorn_api.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 popcorn_api-0.0.1a3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 popcorn_api-0.0.1a3/LICENSE
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 popcorn_api-0.0.1a3/README.md
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 popcorn_api-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 popcorn_api-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 popcorn_api-0.0.1a4/src/.python-version
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 popcorn_api-0.0.1a4/src/popcorn_api/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 popcorn_api-0.0.1a4/src/popcorn_api/config.json
+-rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 popcorn_api-0.0.1a4/src/popcorn_api/popcorn_api.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 popcorn_api-0.0.1a4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 popcorn_api-0.0.1a4/LICENSE
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 popcorn_api-0.0.1a4/README.md
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 popcorn_api-0.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 popcorn_api-0.0.1a4/PKG-INFO
```

### Comparing `popcorn_api-0.0.1a3/src/popcorn_api/popcorn_api.py` & `popcorn_api-0.0.1a4/src/popcorn_api/popcorn_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,20 @@
         except requests.exceptions.ConnectionError as e:
             self.log.error(f'Request to {url!r} failed with {e.__class__.__name__!r}')
             return None
 
         if req.status_code != 200:
             self.log.error(f'Request to {url!r} failed with status code {req.status_code!r}')
             return None
-        return req.json()
+        
+        try:
+            return req.json()
+        except json.JSONDecodeError as e:
+            self.log.error(f'Request to {url!r} did not return a valid json file')
+            return None
 
     def _api_urls(self, path: str) -> list[str]:
         """Gets a url with specified path for every known api
 
         Parameters
         ----------
         path : target path
```

### Comparing `popcorn_api-0.0.1a3/LICENSE` & `popcorn_api-0.0.1a4/LICENSE`

 * *Files identical despite different names*

