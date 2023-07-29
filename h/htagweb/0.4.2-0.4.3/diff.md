# Comparing `tmp/htagweb-0.4.2.tar.gz` & `tmp/htagweb-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagweb-0.4.2.tar", max compression
+gzip compressed data, was "htagweb-0.4.3.tar", max compression
```

## Comparing `htagweb-0.4.2.tar` & `htagweb-0.4.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2023-07-23 08:37:12.344180 htagweb-0.4.2/LICENSE
--rw-r--r--   0        0        0     3148 2023-07-23 08:37:12.344180 htagweb-0.4.2/README.md
--rw-r--r--   0        0        0      518 2023-07-23 08:37:12.920194 htagweb-0.4.2/htagweb/__init__.py
--rw-r--r--   0        0        0      421 2023-07-23 08:37:12.344180 htagweb-0.4.2/htagweb/__main__.py
--rw-r--r--   0        0        0     2521 2023-07-23 08:37:12.344180 htagweb-0.4.2/htagweb/crypto.py
--rw-r--r--   0        0        0    10670 2023-07-23 08:37:12.344180 htagweb-0.4.2/htagweb/htagserver.py
--rw-r--r--   0        0        0     3797 2023-07-23 08:37:12.344180 htagweb-0.4.2/htagweb/manager.py
--rw-r--r--   0        0        0     5659 2023-07-23 08:37:12.344180 htagweb-0.4.2/htagweb/uidprocess.py
--rw-r--r--   0        0        0     9925 2023-07-23 08:37:12.344180 htagweb-0.4.2/htagweb/webbase.py
--rw-r--r--   0        0        0     1124 2023-07-23 08:37:12.920194 htagweb-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     4350 1970-01-01 00:00:00.000000 htagweb-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-29 12:42:42.690832 htagweb-0.4.3/LICENSE
+-rw-r--r--   0        0        0     3647 2023-07-29 12:42:42.690832 htagweb-0.4.3/README.md
+-rw-r--r--   0        0        0      518 2023-07-29 12:42:42.974837 htagweb-0.4.3/htagweb/__init__.py
+-rw-r--r--   0        0        0      421 2023-07-29 12:42:42.690832 htagweb-0.4.3/htagweb/__main__.py
+-rw-r--r--   0        0        0     2521 2023-07-29 12:42:42.690832 htagweb-0.4.3/htagweb/crypto.py
+-rw-r--r--   0        0        0    10753 2023-07-29 12:42:42.690832 htagweb-0.4.3/htagweb/htagserver.py
+-rw-r--r--   0        0        0     3797 2023-07-29 12:42:42.690832 htagweb-0.4.3/htagweb/manager.py
+-rw-r--r--   0        0        0     5577 2023-07-29 12:42:42.690832 htagweb-0.4.3/htagweb/uidprocess.py
+-rw-r--r--   0        0        0     9925 2023-07-29 12:42:42.690832 htagweb-0.4.3/htagweb/webbase.py
+-rw-r--r--   0        0        0     1124 2023-07-29 12:42:42.974837 htagweb-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     4849 1970-01-01 00:00:00.000000 htagweb-0.4.3/PKG-INFO
```

### Comparing `htagweb-0.4.2/LICENSE` & `htagweb-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `htagweb-0.4.2/README.md` & `htagweb-0.4.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -83,7 +83,20 @@
 ```
 
 See a more advanced example in [examples folder](https://github.com/manatlan/htagweb/tree/master/examples)
 
 ```bash
 python3 examples/main.py
 ```
+
+# htagweb.HtagServer
+
+This is a new beast, which is available in this module, and __it's COMPLETLY different from ALL others htag runners__.
+See it like an "htag server", very useful during development phase. In console, type :
+
+```bash
+$ python3 -m htagweb
+```
+
+It will run a solid http/ws, with all htag/web features, and you can browse htag's apps in an html page.
+
+It's not the official way to expose htag's apps on the web. But I'm currently exploring that (because it's a lot lot simpler ;-)
```

### Comparing `htagweb-0.4.2/htagweb/__init__.py` & `htagweb-0.4.3/htagweb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 from .webbase import WebServer
 from .webbase import WebServerWS
 
 from .htagserver import HtagServer  # a completly different beast.
 
 __all__= ["WebServer","WebServerWS","HtagServer"]
 
-__version__ = "0.4.2" # auto updated
+__version__ = "0.4.3" # auto updated
```

### Comparing `htagweb-0.4.2/htagweb/crypto.py` & `htagweb-0.4.3/htagweb/crypto.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.4.2/htagweb/htagserver.py` & `htagweb-0.4.3/htagweb/htagserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,14 +272,15 @@
             jsparano += f"\nvar _PARANO_='{self.parano}'\n"
             jsparano += "\nasync function _read_(x) {return await decrypt(x,_PARANO_)}\n"
             jsparano += "\nasync function _write_(x) {return await encrypt(x,_PARANO_)}\n"
         else:
             jsparano = ""
             jsparano += "\nasync function _read_(x) {return x}\n"
             jsparano += "\nasync function _write_(x) {return x}\n"
+        #TODO: consider https://developer.chrome.com/blog/removing-document-write/
         bootstrapHtmlPage="""<!DOCTYPE html>
             <html>
               <head>
                     <script>
                     %(jsparano)s
                     // instanciate the WEBSOCKET
                     var _WS_ = new WebSocket("%(protocol)s://"+location.host+"/_WS_/%(path)s"+location.search);
```

### Comparing `htagweb-0.4.2/htagweb/manager.py` & `htagweb-0.4.3/htagweb/manager.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.4.2/htagweb/uidprocess.py` & `htagweb-0.4.3/htagweb/uidprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,14 @@
             session["ping"]="here"
             return f"hello {msg}"
 
         #==========================================================
         async def ht_create(self, fqn,js,init_params=None,renew=False):        # -> str
         #==========================================================
             """ HRenderer creator """
-            session["ht_create"]="here"
             if init_params is None : init_params=((),{})
 
             hr=HTS.get(fqn)
             if renew or (hr is None) or str(init_params)!=str(hr.init):
                 ##HRenderer(tagClass: type, js:str, exit_callback:Optional[Callable]=None, init= ((),{}), fullerror=False, statics=[], session=None ):
 
                 #--------------------------- fqn -> module, name
@@ -64,15 +63,14 @@
             return str(hr)
 
 
         #==========================================================
         async def ht_interact(self,fqn,data): # -> dict
         #==========================================================
             """ interact with hrenderer instance """
-            session["ht_interact"]="here"
             hr=HTS[fqn]
 
             #/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\ to simplify ut
             if data["id"]=="ut":
                 data["id"] = id(hr.tag) #only main tag ;-(
             #/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\
```

### Comparing `htagweb-0.4.2/htagweb/webbase.py` & `htagweb-0.4.3/htagweb/webbase.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.4.2/pyproject.toml` & `htagweb-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagweb"
-version = "0.4.2" # auto-updated
+version = "0.4.3" # auto-updated
 description = "It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','webserver']
 homepage = "https://github.com/manatlan/htagweb"
 repository = "https://github.com/manatlan/htagweb"
```

### Comparing `htagweb-0.4.2/PKG-INFO` & `htagweb-0.4.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagweb
-Version: 0.4.2
+Version: 0.4.3
 Summary: It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)
 Home-page: https://github.com/manatlan/htagweb
 License: MIT
 Keywords: htag,webserver
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -113,7 +113,20 @@
 
 See a more advanced example in [examples folder](https://github.com/manatlan/htagweb/tree/master/examples)
 
 ```bash
 python3 examples/main.py
 ```
 
+# htagweb.HtagServer
+
+This is a new beast, which is available in this module, and __it's COMPLETLY different from ALL others htag runners__.
+See it like an "htag server", very useful during development phase. In console, type :
+
+```bash
+$ python3 -m htagweb
+```
+
+It will run a solid http/ws, with all htag/web features, and you can browse htag's apps in an html page.
+
+It's not the official way to expose htag's apps on the web. But I'm currently exploring that (because it's a lot lot simpler ;-)
+
```

