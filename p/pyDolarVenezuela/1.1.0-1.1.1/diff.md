# Comparing `tmp/pyDolarVenezuela-1.1.0-py3-none-any.whl.zip` & `tmp/pyDolarVenezuela-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6064 bytes, number of entries: 10
+Zip file size: 6121 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       98 b- defN 23-Jul-26 05:29 pyDolarVenezuela/__init__.py
 -rw-rw-rw-  2.0 fat      389 b- defN 23-Jul-26 03:29 pyDolarVenezuela/module_bcv.py
--rw-rw-rw-  2.0 fat      573 b- defN 23-Jul-26 04:17 pyDolarVenezuela/request.py
--rw-rw-rw-  2.0 fat     2962 b- defN 23-Jul-27 01:58 pyDolarVenezuela/scraping_monitor.py
+-rw-rw-rw-  2.0 fat      580 b- defN 23-Jul-29 04:40 pyDolarVenezuela/request.py
+-rw-rw-rw-  2.0 fat     3071 b- defN 23-Jul-29 05:38 pyDolarVenezuela/scraping_monitor.py
 -rw-rw-rw-  2.0 fat       81 b- defN 23-Jul-26 04:18 pyDolarVenezuela/util.py
--rw-rw-rw-  2.0 fat     1094 b- defN 23-Jul-27 02:03 pyDolarVenezuela-1.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3560 b- defN 23-Jul-27 02:03 pyDolarVenezuela-1.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-27 02:03 pyDolarVenezuela-1.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-27 02:03 pyDolarVenezuela-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      855 b- defN 23-Jul-27 02:03 pyDolarVenezuela-1.1.0.dist-info/RECORD
-10 files, 9721 bytes uncompressed, 4584 bytes compressed:  52.8%
+-rw-rw-rw-  2.0 fat     1094 b- defN 23-Jul-29 05:45 pyDolarVenezuela-1.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3560 b- defN 23-Jul-29 05:45 pyDolarVenezuela-1.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-29 05:45 pyDolarVenezuela-1.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-29 05:45 pyDolarVenezuela-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      855 b- defN 23-Jul-29 05:45 pyDolarVenezuela-1.1.1.dist-info/RECORD
+10 files, 9837 bytes uncompressed, 4641 bytes compressed:  52.8%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: pyDolarVenezuela/scraping_monitor.py
 Comment: 
 
 Filename: pyDolarVenezuela/util.py
 Comment: 
 
-Filename: pyDolarVenezuela-1.1.0.dist-info/LICENSE
+Filename: pyDolarVenezuela-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: pyDolarVenezuela-1.1.0.dist-info/METADATA
+Filename: pyDolarVenezuela-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pyDolarVenezuela-1.1.0.dist-info/WHEEL
+Filename: pyDolarVenezuela-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyDolarVenezuela-1.1.0.dist-info/top_level.txt
+Filename: pyDolarVenezuela-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyDolarVenezuela-1.1.0.dist-info/RECORD
+Filename: pyDolarVenezuela-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyDolarVenezuela/request.py

```diff
@@ -1,14 +1,14 @@
 import requests
 from requests import Response
 
 # headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3'}
 
 def ensure_200_and_return_content(response: Response) -> bytes:
     if not response.status_code == requests.codes.ok:
-        raise ValueError("Error de comunicación Alcambio. Codigo: {0}".format(response.status_code))
+        raise ValueError("Error de comunicación ExchangeMonitor. Codigo: {0}".format(response.status_code))
     return response.content
 
 def get_content_page(url: str) -> bytes:
     return ensure_200_and_return_content(
         requests.get(url=url)
     )
```

## pyDolarVenezuela/scraping_monitor.py

```diff
@@ -1,9 +1,9 @@
 from bs4 import BeautifulSoup
-import re
+from emoji import emojize
 
 from pyDolarVenezuela.request import get_content_page
 from pyDolarVenezuela.util import PAGINA_PRINCIPAL_EXCHANGE_MONITOR
 
 def _get_values_monitors(soup: BeautifulSoup):
     return [value for value in soup]
 
@@ -25,19 +25,19 @@
         all_monitors = _get_values_monitors(section_dolar_venezuela)
 
         self.all_monitors = {}
         self.all_monitors['value'] = {"date": date}
         i: int = 0
         for monitor in all_monitors:
             monitor = monitor.find("div", "module-table module-table-fecha")
+            change = str(monitor.find('p', 'cambio-por').text)
             data = {
-                "name": monitor.find('h6', 'nombre').text,
-                "unit": monitor.find('p', 'unidad').text,
+                "title": monitor.find('h6', 'nombre').text,
                 "price": str(monitor.find('p', 'precio').text).replace(',', '.'),
-                "change": monitor.find('p', 'cambio-por').text,
+                "change": ("\U00002B07" + change[1:] if change[0] == '▼' else "\U00002B06" + change[1:] if change[0] == '▲' else "" + change[1:]),
                 "last_update": monitor.find('p', 'fecha').text
             }
             self.all_monitors[f"{i}"] = data
             i += 1
     
     def get_value_monitors(self, monitor_code: str = None, name_property: str = None, prettify: bool = False):
         """
```

## Comparing `pyDolarVenezuela-1.1.0.dist-info/LICENSE` & `pyDolarVenezuela-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyDolarVenezuela-1.1.0.dist-info/METADATA` & `pyDolarVenezuela-1.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.1.0
+Version: 1.1.1
 Summary: esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/fcoagz/pydolarvenezuela
 Project-URL: Bug Tracker, https://github.com/fcoagz/pydolarvenezuela/issues
```

## Comparing `pyDolarVenezuela-1.1.0.dist-info/RECORD` & `pyDolarVenezuela-1.1.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pyDolarVenezuela/__init__.py,sha256=0GTmqLZwCOSXXMeTQ5l-GVI8bzSHdG1ptbaK8dNUjoo,98
 pyDolarVenezuela/module_bcv.py,sha256=IcxghFAml6nLh8LmHasJG3DFLzPSDF-7wXrfdGFP93M,389
-pyDolarVenezuela/request.py,sha256=55_ZjAKw-SupS4ugtXZWhSEZgqVy9mgz5DKUchQKH_4,573
-pyDolarVenezuela/scraping_monitor.py,sha256=B6lGHFWywZmpJtdv-9r-tROQP5ILERPZ1hwPwbQ2P6U,2962
+pyDolarVenezuela/request.py,sha256=7LZPonYkVglFEGOkBCjGo9Tl5EVdWOBGzvmewgvAUOo,580
+pyDolarVenezuela/scraping_monitor.py,sha256=oKNlgGh5WWNgys-kUopXUd5Mjy-SUjzSjquupiO_ewM,3071
 pyDolarVenezuela/util.py,sha256=9zypmUe_jZTpMkzyizPj5N9hJoH78tRyUHdfNw3EFfI,81
-pyDolarVenezuela-1.1.0.dist-info/LICENSE,sha256=yhyzG4KlBwvAy1K47aCyZbF5x8p9Evp9ehLARqdm4mM,1094
-pyDolarVenezuela-1.1.0.dist-info/METADATA,sha256=VmNR-Cw56-CW2wBub5a7pyHahgHUekWqXqUQKGZAnHQ,3560
-pyDolarVenezuela-1.1.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-pyDolarVenezuela-1.1.0.dist-info/top_level.txt,sha256=DqT65xfdAAw8yCgxoWQ1UWnzpZ-LGoBUkgMVnY0N8ro,17
-pyDolarVenezuela-1.1.0.dist-info/RECORD,,
+pyDolarVenezuela-1.1.1.dist-info/LICENSE,sha256=yhyzG4KlBwvAy1K47aCyZbF5x8p9Evp9ehLARqdm4mM,1094
+pyDolarVenezuela-1.1.1.dist-info/METADATA,sha256=mAsY_RWnVUCUP_8raUjDHXQHyVlxS2eogAxS8OkN-6Q,3560
+pyDolarVenezuela-1.1.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+pyDolarVenezuela-1.1.1.dist-info/top_level.txt,sha256=DqT65xfdAAw8yCgxoWQ1UWnzpZ-LGoBUkgMVnY0N8ro,17
+pyDolarVenezuela-1.1.1.dist-info/RECORD,,
```

