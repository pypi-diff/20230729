# Comparing `tmp/localstack-extension-httpbin-0.1.0.dev2.tar.gz` & `tmp/localstack-extension-httpbin-0.1.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-extension-httpbin-0.1.0.dev2.tar", last modified: Sat Jul 29 01:01:06 2023, max compression
+gzip compressed data, was "localstack-extension-httpbin-0.1.0.dev3.tar", last modified: Sat Jul 29 01:17:30 2023, max compression
```

## Comparing `localstack-extension-httpbin-0.1.0.dev2.tar` & `localstack-extension-httpbin-0.1.0.dev3.tar`

### file list

```diff
@@ -1,28 +1,46 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 01:01:06.655071 localstack-extension-httpbin-0.1.0.dev2/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2158 2023-07-29 01:01:06.655071 localstack-extension-httpbin-0.1.0.dev2/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1850 2023-07-29 00:50:06.000000 localstack-extension-httpbin-0.1.0.dev2/README.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 01:01:06.651071 localstack-extension-httpbin-0.1.0.dev2/localstack_extension_httpbin.egg-info/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2158 2023-07-29 01:01:06.000000 localstack-extension-httpbin-0.1.0.dev2/localstack_extension_httpbin.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      852 2023-07-29 01:01:06.000000 localstack-extension-httpbin-0.1.0.dev2/localstack_extension_httpbin.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-29 01:01:06.000000 localstack-extension-httpbin-0.1.0.dev2/localstack_extension_httpbin.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       80 2023-07-29 01:01:06.000000 localstack-extension-httpbin-0.1.0.dev2/localstack_extension_httpbin.egg-info/entry_points.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-29 01:00:56.000000 localstack-extension-httpbin-0.1.0.dev2/localstack_extension_httpbin.egg-info/not-zip-safe
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       94 2023-07-29 01:01:06.000000 localstack-extension-httpbin-0.1.0.dev2/localstack_extension_httpbin.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       19 2023-07-29 01:01:06.000000 localstack-extension-httpbin-0.1.0.dev2/localstack_extension_httpbin.egg-info/top_level.txt
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 01:01:06.655071 localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       28 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1615 2023-07-29 00:43:47.000000 localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/extension.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      750 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/server.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 01:01:06.655071 localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/vendor/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       25 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/vendor/__init__.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 01:01:06.655071 localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/vendor/httpbin/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       45 2023-07-29 00:58:34.000000 localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/vendor/httpbin/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    44092 2023-07-29 00:59:06.000000 localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/vendor/httpbin/core.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2306 2023-07-29 00:46:13.000000 localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/vendor/httpbin/filters.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    13788 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/vendor/httpbin/helpers.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      681 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/vendor/httpbin/structures.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      588 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/vendor/httpbin/utils.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       23 2023-07-29 01:00:31.000000 localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/vendor/httpbin/version.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      524 2023-07-29 00:40:50.000000 localstack-extension-httpbin-0.1.0.dev2/pyproject.toml
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      728 2023-07-29 01:01:06.655071 localstack-extension-httpbin-0.1.0.dev2/setup.cfg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       60 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev2/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 01:17:30.458574 localstack-extension-httpbin-0.1.0.dev3/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2158 2023-07-29 01:17:30.458574 localstack-extension-httpbin-0.1.0.dev3/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1850 2023-07-29 00:50:06.000000 localstack-extension-httpbin-0.1.0.dev3/README.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 01:17:30.454573 localstack-extension-httpbin-0.1.0.dev3/localstack_extension_httpbin.egg-info/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2158 2023-07-29 01:17:30.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_extension_httpbin.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1685 2023-07-29 01:17:30.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_extension_httpbin.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-29 01:17:30.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_extension_httpbin.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       80 2023-07-29 01:17:30.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_extension_httpbin.egg-info/entry_points.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-29 01:17:18.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_extension_httpbin.egg-info/not-zip-safe
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       94 2023-07-29 01:17:30.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_extension_httpbin.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       19 2023-07-29 01:17:30.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_extension_httpbin.egg-info/top_level.txt
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 01:17:30.454573 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       28 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1827 2023-07-29 01:10:40.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/extension.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      750 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/server.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 01:17:30.454573 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       25 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/__init__.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 01:17:30.454573 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       45 2023-07-29 00:58:34.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    44092 2023-07-29 01:09:01.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/core.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2306 2023-07-29 00:46:13.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/filters.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    13788 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/helpers.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 01:17:30.454573 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/static/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    22382 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/static/favicon.ico
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      681 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/structures.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 01:17:30.454573 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/templates/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    14240 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/templates/UTF-8-demo.txt
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 01:17:30.458574 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/templates/flasgger/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10250 2023-07-29 00:44:43.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/templates/flasgger/index.html
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      467 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/templates/footer.html
+-rwxrwxr-x   0 thomas    (1000) thomas    (1000)     1419 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/templates/forms-post.html
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10840 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/templates/httpbin.1.html
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 01:17:30.458574 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/templates/images/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    35588 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/templates/images/jackal.jpg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8090 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/templates/images/pig_icon.png
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8984 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/templates/images/svg_logo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10568 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/templates/images/wolf_1.webp
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4628 2023-07-29 00:45:00.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/templates/index.html
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3742 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/templates/moby.html
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      523 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/templates/sample.xml
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      582 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/templates/trackingscripts.html
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      588 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/utils.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       23 2023-07-29 01:00:31.000000 localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/version.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      524 2023-07-29 00:40:50.000000 localstack-extension-httpbin-0.1.0.dev3/pyproject.toml
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      907 2023-07-29 01:17:30.458574 localstack-extension-httpbin-0.1.0.dev3/setup.cfg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       60 2023-07-29 00:35:56.000000 localstack-extension-httpbin-0.1.0.dev3/setup.py
```

### Comparing `localstack-extension-httpbin-0.1.0.dev2/PKG-INFO` & `localstack-extension-httpbin-0.1.0.dev3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-extension-httpbin
-Version: 0.1.0.dev2
+Version: 0.1.0.dev3
 Summary: LocalStack Extension: httpbin
 Home-page: https://github.com/localstack/localstack-extensions/tree/main/httpbin
 Author: LocalStack
 Author-email: info@localstack.cloud
 Description-Content-Type: text/markdown; charset=UTF-8
 
 LocalStack httpbin extension
```

### Comparing `localstack-extension-httpbin-0.1.0.dev2/README.md` & `localstack-extension-httpbin-0.1.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `localstack-extension-httpbin-0.1.0.dev2/localstack_extension_httpbin.egg-info/PKG-INFO` & `localstack-extension-httpbin-0.1.0.dev3/localstack_extension_httpbin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-extension-httpbin
-Version: 0.1.0.dev2
+Version: 0.1.0.dev3
 Summary: LocalStack Extension: httpbin
 Home-page: https://github.com/localstack/localstack-extensions/tree/main/httpbin
 Author: LocalStack
 Author-email: info@localstack.cloud
 Description-Content-Type: text/markdown; charset=UTF-8
 
 LocalStack httpbin extension
```

### Comparing `localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/extension.py` & `localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/extension.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,22 +23,27 @@
 
     def on_extension_load(self):
         level = logging.DEBUG if config.DEBUG else logging.INFO
         logging.getLogger("localstack_httpbin").setLevel(level=level)
         logging.getLogger("httpbin").setLevel(level=level)
 
     def on_platform_start(self):
+        from localstack_httpbin.vendor.httpbin import core
+        core.template['host'] = f"{self.get_public_hostname()}:{config.get_edge_port_http()}"
+
         self.server = HttpbinServer(get_free_tcp_port())
         LOG.debug("starting httpbin on %s", self.server.url)
         self.server.start()
 
-    def on_platform_ready(self):
+    def get_public_hostname(self) -> str:
         # FIXME: reconcile with LOCALSTACK_HOST, but this should be accessible via the host
-        hostname = f"{self.hostname_prefix}{constants.LOCALHOST_HOSTNAME}"
-        LOG.info("Serving httpbin on %s", get_edge_url(localstack_hostname=hostname))
+        return  f"{self.hostname_prefix}{constants.LOCALHOST_HOSTNAME}"
+
+    def on_platform_ready(self):
+        LOG.info("Serving httpbin on %s", get_edge_url(localstack_hostname=self.get_public_hostname()))
 
     def on_platform_shutdown(self):
         if self.server:
             self.server.shutdown()
 
     def update_gateway_routes(self, router: http.Router[http.RouteHandler]):
         endpoint = http.ProxyHandler(forward_base_url=self.server.url)
```

### Comparing `localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/server.py` & `localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/server.py`

 * *Files identical despite different names*

### Comparing `localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/vendor/httpbin/core.py` & `localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/core.py`

 * *Files identical despite different names*

### Comparing `localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/vendor/httpbin/filters.py` & `localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/vendor/httpbin/helpers.py` & `localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/helpers.py`

 * *Files identical despite different names*

### Comparing `localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/vendor/httpbin/structures.py` & `localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/structures.py`

 * *Files identical despite different names*

### Comparing `localstack-extension-httpbin-0.1.0.dev2/localstack_httpbin/vendor/httpbin/utils.py` & `localstack-extension-httpbin-0.1.0.dev3/localstack_httpbin/vendor/httpbin/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-extension-httpbin-0.1.0.dev2/pyproject.toml` & `localstack-extension-httpbin-0.1.0.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-extension-httpbin-0.1.0.dev2/setup.cfg` & `localstack-extension-httpbin-0.1.0.dev3/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = localstack-extension-httpbin
-version = 0.1.0.dev2
+version = 0.1.0.dev3
 url = https://github.com/localstack/localstack-extensions/tree/main/httpbin
 author = LocalStack
 author_email = info@localstack.cloud
 summary = LocalStack Extension: httpbin
 description = A simple HTTP Request & Response Service directly in LocalStack
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
@@ -23,11 +23,18 @@
 	gevent
 	flasgger
 
 [options.entry_points]
 localstack.extensions = 
 	httpbin = localstack_httpbin.extension:HttpbinExtension
 
+[options.package_data]
+localstack_httpbin = 
+	vendor/httpbin/static/*.*
+	vendor/httpbin/templates/*.*
+	vendor/httpbin/templates/flasgger/*.*
+	vendor/httpbin/templates/images/*.*
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

