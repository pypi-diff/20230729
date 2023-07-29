# Comparing `tmp/urlfetch-1.2.2.tar.gz` & `tmp/urlfetch-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/urlfetch-1.2.2.tar", last modified: Sat Jul 11 12:34:27 2020, max compression
+gzip compressed data, was "dist/urlfetch-2.0.0.tar", last modified: Sat Jul 29 15:41:01 2023, max compression
```

## Comparing `urlfetch-1.2.2.tar` & `urlfetch-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 duyue      (501) staff       (20)        0 2020-07-11 12:34:27.000000 urlfetch-1.2.2/
--rw-r--r--   0 duyue      (501) staff       (20)     4009 2020-07-11 12:34:27.000000 urlfetch-1.2.2/PKG-INFO
--rw-r--r--   0 duyue      (501) staff       (20)     1313 2020-04-29 08:16:55.000000 urlfetch-1.2.2/LICENSE
--rw-r--r--   0 duyue      (501) staff       (20)    36031 2020-07-11 12:31:57.000000 urlfetch-1.2.2/urlfetch.py
--rw-r--r--   0 duyue      (501) staff       (20)       68 2013-11-09 02:41:08.000000 urlfetch-1.2.2/MANIFEST.in
--rw-r--r--   0 duyue      (501) staff       (20)   587726 2019-10-11 04:58:26.000000 urlfetch-1.2.2/urlfetch.useragents.list
--rw-r--r--   0 duyue      (501) staff       (20)     1550 2020-07-11 09:01:47.000000 urlfetch-1.2.2/setup.py
--rw-r--r--   0 duyue      (501) staff       (20)      118 2020-07-11 12:34:27.000000 urlfetch-1.2.2/setup.cfg
-drwxr-xr-x   0 duyue      (501) staff       (20)        0 2020-07-11 12:34:27.000000 urlfetch-1.2.2/urlfetch.egg-info/
--rw-r--r--   0 duyue      (501) staff       (20)     4009 2020-07-11 12:34:27.000000 urlfetch-1.2.2/urlfetch.egg-info/PKG-INFO
--rw-r--r--   0 duyue      (501) staff       (20)      214 2020-07-11 12:34:27.000000 urlfetch-1.2.2/urlfetch.egg-info/SOURCES.txt
--rw-r--r--   0 duyue      (501) staff       (20)        9 2020-07-11 12:34:27.000000 urlfetch-1.2.2/urlfetch.egg-info/top_level.txt
--rw-r--r--   0 duyue      (501) staff       (20)        1 2020-07-11 12:34:27.000000 urlfetch-1.2.2/urlfetch.egg-info/dependency_links.txt
--rw-r--r--   0 duyue      (501) staff       (20)     2164 2019-10-11 04:58:25.000000 urlfetch-1.2.2/README.rst
+drwxr-xr-x   0 duyue      (501) staff       (20)        0 2023-07-29 15:41:01.599151 urlfetch-2.0.0/
+-rw-r--r--   0 duyue      (501) staff       (20)     1313 2020-04-29 08:16:55.000000 urlfetch-2.0.0/LICENSE
+-rw-r--r--   0 duyue      (501) staff       (20)       68 2013-11-09 02:41:08.000000 urlfetch-2.0.0/MANIFEST.in
+-rw-r--r--   0 duyue      (501) staff       (20)     3802 2023-07-29 15:41:01.599362 urlfetch-2.0.0/PKG-INFO
+-rw-r--r--   0 duyue      (501) staff       (20)     2255 2023-07-29 15:10:56.000000 urlfetch-2.0.0/README.rst
+-rw-r--r--   0 duyue      (501) staff       (20)       97 2023-07-29 15:41:01.599961 urlfetch-2.0.0/setup.cfg
+-rw-r--r--   0 duyue      (501) staff       (20)     1176 2023-07-29 15:26:47.000000 urlfetch-2.0.0/setup.py
+drwxr-xr-x   0 duyue      (501) staff       (20)        0 2023-07-29 15:41:01.598774 urlfetch-2.0.0/urlfetch.egg-info/
+-rw-r--r--   0 duyue      (501) staff       (20)     3802 2023-07-29 15:41:01.000000 urlfetch-2.0.0/urlfetch.egg-info/PKG-INFO
+-rw-r--r--   0 duyue      (501) staff       (20)      214 2023-07-29 15:41:01.000000 urlfetch-2.0.0/urlfetch.egg-info/SOURCES.txt
+-rw-r--r--   0 duyue      (501) staff       (20)        1 2023-07-29 15:41:01.000000 urlfetch-2.0.0/urlfetch.egg-info/dependency_links.txt
+-rw-r--r--   0 duyue      (501) staff       (20)        9 2023-07-29 15:41:01.000000 urlfetch-2.0.0/urlfetch.egg-info/top_level.txt
+-rw-r--r--   0 duyue      (501) staff       (20)    34668 2023-07-29 15:32:59.000000 urlfetch-2.0.0/urlfetch.py
+-rw-r--r--   0 duyue      (501) staff       (20)   587726 2019-10-11 04:58:26.000000 urlfetch-2.0.0/urlfetch.useragents.list
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `urlfetch-1.2.2/PKG-INFO` & `urlfetch-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 1.1
 Name: urlfetch
-Version: 1.2.2
+Version: 2.0.0
 Summary: An easy to use HTTP client
 Home-page: https://github.com/ifduyue/urlfetch
 Author: Yue Du
 Author-email: ifduyue@gmail.com
 License: BSD
-Description: urlfetch |travis-badge| |furyio-badge|
+Description: urlfetch |github-actions-badge| |furyio-badge|
         ==========================================================
         
-        .. |travis-badge| image:: https://travis-ci.org/ifduyue/urlfetch.png
-            :target: https://travis-ci.org/ifduyue/urlfetch
+        .. |github-actions-badge| image:: https://github.com/ifduyue/urlfetch/actions/workflows/test.yml/badge.svg
+            :target: https://github.com/ifduyue/urlfetch/actions/workflows/test.yml
         
-        .. |furyio-badge| image:: https://badge.fury.io/py/urlfetch.png
-            :target: http://badge.fury.io/py/urlfetch
+        .. |furyio-badge| image:: https://badge.fury.io/gh/ifduyue%2Furlfetch.svg
+            :target: https://badge.fury.io/gh/ifduyue%2Furlfetch
         
         urlfetch is a simple, lightweight and easy to use HTTP client for Python.
         It is distributed as a single file module and has no depencencies other than the Python Standard Library.
         
         
         Highlights
         -------------
@@ -88,21 +88,15 @@
         under the PYTHONPATH.
         
         
 Keywords: httpclient urlfetch
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
```

### Comparing `urlfetch-1.2.2/LICENSE` & `urlfetch-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `urlfetch-1.2.2/urlfetch.py` & `urlfetch-2.0.0/urlfetch.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 An easy to use HTTP client based on httplib.
 
 :copyright: (c) 2011-2020 by Yue Du.
 :license: BSD 2-clause License, see LICENSE for more details.
 """
 
-__version__ = "1.2.2"
+__version__ = "2.0.0"
 __author__ = "Yue Du <ifduyue@gmail.com>"
 __url__ = "https://github.com/ifduyue/urlfetch"
 __license__ = "BSD 2-Clause License"
 
 import os, sys, base64, codecs, uuid, stat, time, socket
 import ssl
 from os.path import basename, dirname, abspath, join as pathjoin
@@ -23,40 +23,23 @@
 import re
 
 try:
     import simplejson as json
 except ImportError:
     import json
 
-py3k = sys.version_info >= (3, 0)
-support_source_address = (
-    sys.version_info >= (2, 7) and not py3k or sys.version_info >= (3, 2)
-)
-support_ssl_context = sys.version_info >= (2, 7, 9)
-
-if py3k:
-    from http.client import HTTPConnection, HTTPSConnection
-    from urllib.parse import urlencode
-    import urllib.parse as urlparse
-    import http.cookies as Cookie
-
-    basestring = (str, bytes)
-    unicode = str
-    b = lambda s: s.encode("latin-1")
-    u = lambda s: s
-else:
-    from httplib import HTTPConnection, HTTPSConnection
-    from urllib import urlencode
-    import urlparse
-    import Cookie
-
-    basestring = basestring
-    unicode = unicode
-    b = lambda s: s
-    u = lambda s: unicode(s, "unicode_escape")
+from http.client import HTTPConnection, HTTPSConnection
+from urllib.parse import urlencode
+import urllib.parse as urlparse
+import http.cookies as Cookie
+
+basestring = (str, bytes)
+unicode = str
+b = lambda s: s.encode("latin-1")
+u = lambda s: s
 
 __all__ = (
     "request",
     "fetch",
     "Session",
     "get",
     "head",
@@ -372,18 +355,15 @@
             'connection': 'close',
             'etag': '"13cc5e4-220f-4c36507ded580"',
             'date': 'Wed, 27 Jun 2012 06:50:30 GMT',
             'content-type': 'text/html',
             'x-cache-lookup': 'MISS from localhost:8080'
         }
         """
-        if py3k:
-            return dict((k.lower(), v) for k, v in self.getheaders())
-        else:
-            return dict(self.getheaders())
+        return dict((k.lower(), v) for k, v in self.getheaders())
 
     @cached_property
     def cookies(self):
         """Cookies in dict"""
         c = Cookie.SimpleCookie(self.getheader("set-cookie"))
         return dict((i.key, i.value) for i in c.values())
 
@@ -643,36 +623,24 @@
     :returns: A :class:`~urlfetch.Response` object
     :raises: :class:`URLError`, :class:`UrlfetchException`,
              :class:`TooManyRedirects`,
     """
 
     def make_connection(conn_type, host, port, timeout, source_address):
         """Return HTTP or HTTPS connection."""
-        if support_source_address:
-            kwargs = {"timeout": timeout, "source_address": source_address}
-        else:
-            kwargs = {"timeout": timeout}
-            if source_address is not None:
-                raise UrlfetchException(
-                    "source_address requires Python 2.7/3.2 or newer versions"
-                )
+        kwargs = {"timeout": timeout, "source_address": source_address}
 
         ssl_context = None
         if validate_certificate is False:
-            if not support_ssl_context:
-                raise UrlfetchException("validate_certificate requires Python 2.7.9 or newer versions")
             ssl_context = ssl._create_unverified_context()
 
         if conn_type == "http":
             conn = HTTPConnection(host, port, **kwargs)
         elif conn_type == "https":
-            if support_ssl_context:
-                conn = HTTPSConnection(host, port, context=ssl_context, **kwargs)
-            else:
-                conn = HTTPSConnection(host, port, **kwargs)
+            conn = HTTPSConnection(host, port, context=ssl_context, **kwargs)
         else:
             raise URLError("Unknown Connection Type: %s" % conn_type)
         return conn
 
     via_proxy = False
 
     method = method.upper()
@@ -890,37 +858,32 @@
     password, host, port and http_host
     """
     try:
         url = unicode(url)
     except UnicodeDecodeError:
         pass
 
-    if py3k:
-        make_utf8 = lambda x: x
-    else:
-        make_utf8 = lambda x: isinstance(x, unicode) and x.encode("utf-8") or x
-
     if "://" in url:
         scheme, url = url.split("://", 1)
     else:
         scheme = "http"
     url = "http://" + url
     parsed = urlparse.urlsplit(url)
     r = ObjectDict()
-    r["scheme"] = make_utf8(scheme)
-    r["netloc"] = make_utf8(parsed.netloc)
-    r["path"] = make_utf8(parsed.path)
-    r["query"] = make_utf8(parsed.query)
-    r["fragment"] = make_utf8(parsed.fragment)
-    r["uri"] = make_utf8(parsed.path)
+    r["scheme"] = scheme
+    r["netloc"] = parsed.netloc
+    r["path"] = parsed.path
+    r["query"] = parsed.query
+    r["fragment"] = parsed.fragment
+    r["uri"] = parsed.path
     if parsed.query:
-        r["uri"] += "?" + make_utf8(parsed.query)
-    r["username"] = make_utf8(parsed.username)
-    r["password"] = make_utf8(parsed.password)
-    host = make_utf8(parsed.hostname.encode("idna").decode("utf-8"))
+        r["uri"] += "?" + parsed.query
+    r["username"] = parsed.username
+    r["password"] = parsed.password
+    host = parsed.hostname.encode("idna").decode("utf-8")
     r["host"] = r["hostname"] = host
     try:
         r["port"] = parsed.port
     except ValueError:
         r["port"] = None
     if r["port"]:
         r["http_host"] = "%s:%d" % (r["host"], r["port"])
@@ -1083,15 +1046,15 @@
                 body.write(part_boundary)
                 writer(body).write(
                     "Content-Disposition: form-data; " 'name="%s"\r\n' % name
                 )
                 body.write(b"Content-Type: text/plain\r\n\r\n")
                 if isinstance(value, int):
                     value = str(value)
-                if py3k and isinstance(value, str):
+                if isinstance(value, str):
                     writer(body).write(value)
                 else:
                     body.write(value)
                 body.write(b"\r\n")
 
     for fieldname, f in files.items():
         if isinstance(f, tuple):
@@ -1118,15 +1081,15 @@
             body.write(b"Content-Type: application/octet-stream\r\n\r\n")
         else:
             writer(body).write(
                 'Content-Disposition: form-data; name="%s"' "\r\n" % name
             )
             body.write(b"Content-Type: text/plain\r\n\r\n")
 
-        if py3k and isinstance(value, str):
+        if isinstance(value, str):
             writer(body).write(value)
         else:
             body.write(value)
         body.write(b"\r\n")
 
     body.write(b("--" + boundary + "--\r\n"))
```

### Comparing `urlfetch-1.2.2/urlfetch.useragents.list` & `urlfetch-2.0.0/urlfetch.useragents.list`

 * *Files identical despite different names*

### Comparing `urlfetch-1.2.2/setup.py` & `urlfetch-2.0.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,28 +15,20 @@
     license="BSD",
     keywords="httpclient urlfetch",
     py_modules=['urlfetch'],
     data_files=[('', ['urlfetch.useragents.list'])],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.6',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.2',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: POSIX',
         'Operating System :: POSIX :: Linux',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ],
-    test_suite='tests.testall',
-    tests_require=['bottle', 'gunicorn==19.9.0'],
 )
```

### Comparing `urlfetch-1.2.2/urlfetch.egg-info/PKG-INFO` & `urlfetch-2.0.0/urlfetch.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 1.1
 Name: urlfetch
-Version: 1.2.2
+Version: 2.0.0
 Summary: An easy to use HTTP client
 Home-page: https://github.com/ifduyue/urlfetch
 Author: Yue Du
 Author-email: ifduyue@gmail.com
 License: BSD
-Description: urlfetch |travis-badge| |furyio-badge|
+Description: urlfetch |github-actions-badge| |furyio-badge|
         ==========================================================
         
-        .. |travis-badge| image:: https://travis-ci.org/ifduyue/urlfetch.png
-            :target: https://travis-ci.org/ifduyue/urlfetch
+        .. |github-actions-badge| image:: https://github.com/ifduyue/urlfetch/actions/workflows/test.yml/badge.svg
+            :target: https://github.com/ifduyue/urlfetch/actions/workflows/test.yml
         
-        .. |furyio-badge| image:: https://badge.fury.io/py/urlfetch.png
-            :target: http://badge.fury.io/py/urlfetch
+        .. |furyio-badge| image:: https://badge.fury.io/gh/ifduyue%2Furlfetch.svg
+            :target: https://badge.fury.io/gh/ifduyue%2Furlfetch
         
         urlfetch is a simple, lightweight and easy to use HTTP client for Python.
         It is distributed as a single file module and has no depencencies other than the Python Standard Library.
         
         
         Highlights
         -------------
@@ -88,21 +88,15 @@
         under the PYTHONPATH.
         
         
 Keywords: httpclient urlfetch
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
```

### Comparing `urlfetch-1.2.2/README.rst` & `urlfetch-2.0.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-urlfetch |travis-badge| |furyio-badge|
+urlfetch |github-actions-badge| |furyio-badge|
 ==========================================================
 
-.. |travis-badge| image:: https://travis-ci.org/ifduyue/urlfetch.png
-    :target: https://travis-ci.org/ifduyue/urlfetch
+.. |github-actions-badge| image:: https://github.com/ifduyue/urlfetch/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/ifduyue/urlfetch/actions/workflows/test.yml
 
-.. |furyio-badge| image:: https://badge.fury.io/py/urlfetch.png
-    :target: http://badge.fury.io/py/urlfetch
+.. |furyio-badge| image:: https://badge.fury.io/gh/ifduyue%2Furlfetch.svg
+    :target: https://badge.fury.io/gh/ifduyue%2Furlfetch
 
 urlfetch is a simple, lightweight and easy to use HTTP client for Python.
 It is distributed as a single file module and has no depencencies other than the Python Standard Library.
 
 
 Highlights
 -------------
```

