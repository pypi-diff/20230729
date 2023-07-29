# Comparing `tmp/htagweb-0.4.3.tar.gz` & `tmp/htagweb-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagweb-0.4.3.tar", max compression
+gzip compressed data, was "htagweb-0.5.0.tar", max compression
```

## Comparing `htagweb-0.4.3.tar` & `htagweb-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2023-07-29 12:42:42.690832 htagweb-0.4.3/LICENSE
--rw-r--r--   0        0        0     3647 2023-07-29 12:42:42.690832 htagweb-0.4.3/README.md
--rw-r--r--   0        0        0      518 2023-07-29 12:42:42.974837 htagweb-0.4.3/htagweb/__init__.py
--rw-r--r--   0        0        0      421 2023-07-29 12:42:42.690832 htagweb-0.4.3/htagweb/__main__.py
--rw-r--r--   0        0        0     2521 2023-07-29 12:42:42.690832 htagweb-0.4.3/htagweb/crypto.py
--rw-r--r--   0        0        0    10753 2023-07-29 12:42:42.690832 htagweb-0.4.3/htagweb/htagserver.py
--rw-r--r--   0        0        0     3797 2023-07-29 12:42:42.690832 htagweb-0.4.3/htagweb/manager.py
--rw-r--r--   0        0        0     5577 2023-07-29 12:42:42.690832 htagweb-0.4.3/htagweb/uidprocess.py
--rw-r--r--   0        0        0     9925 2023-07-29 12:42:42.690832 htagweb-0.4.3/htagweb/webbase.py
--rw-r--r--   0        0        0     1124 2023-07-29 12:42:42.974837 htagweb-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     4849 1970-01-01 00:00:00.000000 htagweb-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-29 14:06:10.200728 htagweb-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3647 2023-07-29 14:06:10.200728 htagweb-0.5.0/README.md
+-rw-r--r--   0        0        0      518 2023-07-29 14:06:10.552768 htagweb-0.5.0/htagweb/__init__.py
+-rw-r--r--   0        0        0      670 2023-07-29 14:06:10.200728 htagweb-0.5.0/htagweb/__main__.py
+-rw-r--r--   0        0        0     2521 2023-07-29 14:06:10.200728 htagweb-0.5.0/htagweb/crypto.py
+-rw-r--r--   0        0        0    11719 2023-07-29 14:06:10.200728 htagweb-0.5.0/htagweb/htagserver.py
+-rw-r--r--   0        0        0     3797 2023-07-29 14:06:10.204728 htagweb-0.5.0/htagweb/manager.py
+-rw-r--r--   0        0        0     5577 2023-07-29 14:06:10.204728 htagweb-0.5.0/htagweb/uidprocess.py
+-rw-r--r--   0        0        0     9925 2023-07-29 14:06:10.204728 htagweb-0.5.0/htagweb/webbase.py
+-rw-r--r--   0        0        0     1124 2023-07-29 14:06:10.552768 htagweb-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4849 1970-01-01 00:00:00.000000 htagweb-0.5.0/PKG-INFO
```

### Comparing `htagweb-0.4.3/LICENSE` & `htagweb-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `htagweb-0.4.3/README.md` & `htagweb-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `htagweb-0.4.3/htagweb/__init__.py` & `htagweb-0.5.0/htagweb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 from .webbase import WebServer
 from .webbase import WebServerWS
 
 from .htagserver import HtagServer  # a completly different beast.
 
 __all__= ["WebServer","WebServerWS","HtagServer"]
 
-__version__ = "0.4.3" # auto updated
+__version__ = "0.5.0" # auto updated
```

### Comparing `htagweb-0.4.3/htagweb/crypto.py` & `htagweb-0.5.0/htagweb/crypto.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.4.3/htagweb/htagserver.py` & `htagweb-0.5.0/htagweb/htagserver.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
 import os
 import sys
 import json
 import uuid
 import inspect
 import logging
+import uvicorn
 import importlib
 
 from starlette.applications import Starlette
 from starlette.responses import HTMLResponse
 from starlette.applications import Starlette
 from starlette.routing import Route,WebSocketRoute
 from starlette.endpoints import WebSocketEndpoint
@@ -206,18 +207,29 @@
 }
 
 console.log("started")
 """
         self.hr=None
 
         if not path:
-            try:
-                klass=getClass("index:App")
-            except Exception as e:
-                klass=IndexApp
+            if websocket.app.index:
+                # there is a main htag'class for '/'
+                if isinstance(websocket.app.index,str):
+                    path=websocket.app.index
+                    if ":" in path:
+                        klass=getClass(path)
+                    else:
+                        klass=getClass(path+":App")
+                else:
+                    klass=websocket.app.index
+            else:
+                try:
+                    klass=getClass("index:App")
+                except Exception as e:
+                    klass=IndexApp
         else:
             try:
                 if ":" in path:
                     klass=getClass(path)
                 else:
                     klass=getClass(path+":App")
             except Exception as e:
@@ -246,15 +258,16 @@
         actions = await self.hr.interact(data["id"],data["method"],data["args"],data["kargs"],data.get("event"))
         await self._sendback( websocket, json.dumps(actions) )
 
     async def on_disconnect(self, websocket, close_code):
         del self.hr
 
 class HtagServer(Starlette):
-    def __init__(self,debug:bool=True,ssl:bool=False,session_size:int=10240,parano:bool=False):
+    def __init__(self,obj:"htag.Tag class or fqn"=None, debug:bool=True,ssl:bool=False,session_size:int=10240,parano:bool=False):
+        self.index = obj
         self.ssl=ssl
         self.parano = str(uuid.uuid4()) if parano else None
         Starlette.__init__( self,
             debug=debug,
             routes=[
                 Route('/', self._servehtagapp),
                 Route('/{path}', self._servehtagapp),
@@ -298,8 +311,18 @@
               </head>
               <body>loading</body>
             </html>
             """ % locals()
 
         return HTMLResponse( bootstrapHtmlPage )
 
+    def add_route(self,*a,**k):
+        """ insert route at the beginning ;-) """
+        super().add_route(*a,**k)
+        self.router.routes.insert(0, self.router.routes.pop() )
+
+    def run(self, host="0.0.0.0", port=8000, openBrowser=False):   # localhost, by default !!
+        if openBrowser:
+            import webbrowser
+            webbrowser.open_new_tab(f"http://localhost:{port}")
 
+        uvicorn.run(self, host=host, port=port)
```

### Comparing `htagweb-0.4.3/htagweb/manager.py` & `htagweb-0.5.0/htagweb/manager.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.4.3/htagweb/uidprocess.py` & `htagweb-0.5.0/htagweb/uidprocess.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.4.3/htagweb/webbase.py` & `htagweb-0.5.0/htagweb/webbase.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.4.3/pyproject.toml` & `htagweb-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagweb"
-version = "0.4.3" # auto-updated
+version = "0.5.0" # auto-updated
 description = "It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','webserver']
 homepage = "https://github.com/manatlan/htagweb"
 repository = "https://github.com/manatlan/htagweb"
```

### Comparing `htagweb-0.4.3/PKG-INFO` & `htagweb-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagweb
-Version: 0.4.3
+Version: 0.5.0
 Summary: It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)
 Home-page: https://github.com/manatlan/htagweb
 License: MIT
 Keywords: htag,webserver
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.8,<4.0
```

