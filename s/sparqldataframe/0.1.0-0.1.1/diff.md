# Comparing `tmp/sparqldataframe-0.1.0.tar.gz` & `tmp/sparqldataframe-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sparqldataframe-0.1.0.tar", last modified: Sun Mar  3 13:09:14 2019, max compression
+gzip compressed data, was "sparqldataframe-0.1.1.tar", last modified: Sat Jul 29 11:26:57 2023, max compression
```

## Comparing `sparqldataframe-0.1.0.tar` & `sparqldataframe-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 kubuntu-user  (1000) kubuntu-user  (1000)        0 2019-03-03 13:09:14.000000 sparqldataframe-0.1.0/
--rw-rw-r--   0 kubuntu-user  (1000) kubuntu-user  (1000)     2725 2019-03-03 13:09:14.000000 sparqldataframe-0.1.0/PKG-INFO
--rw-rw-r--   0 kubuntu-user  (1000) kubuntu-user  (1000)     1330 2019-03-03 13:09:06.000000 sparqldataframe-0.1.0/README.rst
--rw-rw-r--   0 kubuntu-user  (1000) kubuntu-user  (1000)       38 2019-03-03 13:09:14.000000 sparqldataframe-0.1.0/setup.cfg
-drwxrwxr-x   0 kubuntu-user  (1000) kubuntu-user  (1000)        0 2019-03-03 13:09:14.000000 sparqldataframe-0.1.0/sparqldataframe.egg-info/
--rw-rw-r--   0 kubuntu-user  (1000) kubuntu-user  (1000)     2725 2019-03-03 13:09:13.000000 sparqldataframe-0.1.0/sparqldataframe.egg-info/PKG-INFO
--rw-rw-r--   0 kubuntu-user  (1000) kubuntu-user  (1000)      241 2019-03-03 13:09:13.000000 sparqldataframe-0.1.0/sparqldataframe.egg-info/SOURCES.txt
--rw-rw-r--   0 kubuntu-user  (1000) kubuntu-user  (1000)        1 2019-03-03 13:09:13.000000 sparqldataframe-0.1.0/sparqldataframe.egg-info/dependency_links.txt
--rw-rw-r--   0 kubuntu-user  (1000) kubuntu-user  (1000)       16 2019-03-03 13:09:13.000000 sparqldataframe-0.1.0/sparqldataframe.egg-info/requires.txt
--rw-rw-r--   0 kubuntu-user  (1000) kubuntu-user  (1000)       16 2019-03-03 13:09:13.000000 sparqldataframe-0.1.0/sparqldataframe.egg-info/top_level.txt
--rw-rw-r--   0 kubuntu-user  (1000) kubuntu-user  (1000)     1831 2019-03-03 12:34:57.000000 sparqldataframe-0.1.0/setup.py
-drwxrwxr-x   0 kubuntu-user  (1000) kubuntu-user  (1000)        0 2019-03-03 13:09:14.000000 sparqldataframe-0.1.0/sparqldataframe/
--rw-rw-r--   0 kubuntu-user  (1000) kubuntu-user  (1000)      932 2019-03-03 12:28:29.000000 sparqldataframe-0.1.0/sparqldataframe/__init__.py
+drwxrwxr-x   0 nikolai   (1000) nikolai   (1000)        0 2023-07-29 11:26:57.553032 sparqldataframe-0.1.1/
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     1073 2023-07-26 15:02:34.000000 sparqldataframe-0.1.1/LICENSE
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     2175 2023-07-29 11:26:57.553032 sparqldataframe-0.1.1/PKG-INFO
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     1169 2023-07-29 11:11:44.000000 sparqldataframe-0.1.1/README.md
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)       38 2023-07-29 11:26:57.553032 sparqldataframe-0.1.1/setup.cfg
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     2294 2023-07-29 11:25:59.000000 sparqldataframe-0.1.1/setup.py
+drwxrwxr-x   0 nikolai   (1000) nikolai   (1000)        0 2023-07-29 11:26:57.549033 sparqldataframe-0.1.1/sparqldataframe/
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     1100 2023-07-29 10:53:55.000000 sparqldataframe-0.1.1/sparqldataframe/__init__.py
+drwxrwxr-x   0 nikolai   (1000) nikolai   (1000)        0 2023-07-29 11:26:57.553032 sparqldataframe-0.1.1/sparqldataframe.egg-info/
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     2175 2023-07-29 11:26:56.000000 sparqldataframe-0.1.1/sparqldataframe.egg-info/PKG-INFO
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)      248 2023-07-29 11:26:57.000000 sparqldataframe-0.1.1/sparqldataframe.egg-info/SOURCES.txt
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)        1 2023-07-29 11:26:56.000000 sparqldataframe-0.1.1/sparqldataframe.egg-info/dependency_links.txt
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)       27 2023-07-29 11:26:57.000000 sparqldataframe-0.1.1/sparqldataframe.egg-info/requires.txt
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)       16 2023-07-29 11:26:57.000000 sparqldataframe-0.1.1/sparqldataframe.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sparqldataframe-0.1.0/PKG-INFO` & `sparqldataframe-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: sparqldataframe
-Version: 0.1.0
+Version: 0.1.1
 Summary: Get a Pandas dataframe from SPARQL queries
 Home-page: https://github.com/njanakiev/sparqldataframe
 Author: Nikolai Janakiev
 Author-email: nikolai.janakiev@gmail.com
 License: MIT
-Description: sparqldataframe
-        ===============
-        
-        .. image:: https://img.shields.io/pypi/v/sparqldataframe.svg
-                :target: https://pypi.python.org/pypi/sparqldataframe
-        
-        
-        A Python library that can send `SPARQL`_ queries to a SPARQL endpoint and retrieve a `Pandas`_ dataframe from the result.
-        
-        
-        Installation
-        ------------
-        
-        .. code-block:: bash
-        	
-        	pip install sparqldataframe
-        
-        
-        Usage
-        -----
-        
-        Here is an example how to run a SPARQL query on the `Wikidata`_ endpoint:
-        
-        .. code-block:: python
-        	
-        	import sparqldataframe
-        
-        	sparql_query = """
-        	SELECT ?item ?itemLabel 
-        	WHERE {
-        	  ?item wdt:P31 wd:Q146.
-        	  SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
-        	}
-        	"""
-        	df = sparqldataframe.query("https://query.wikidata.org/sparql", sparql_query)
-        
-        Wikidata and `DBPedia`_ can be both used without adding the SPARQL endpoint url by using the :code:`wikidata_query()` and :code:`dbpedia_query()` functions respectively:
-        
-        .. code-block:: python
-        
-        	df = sparqldataframe.wikidata_query(sparql_query)
-        	df = sparqldataframe.dbpedia_query(sparql_query)
-        
-        
-        License 
-        -------
-        
-        This project is licensed under the MIT license. See the `LICENSE`_ for details.
-        
-        
-        .. _SPARQL: https://en.wikipedia.org/wiki/SPARQL
-        .. _Wikidata: http://wikidata.org/
-        .. _DBPedia: http://dbpedia.org/
-        .. _Pandas: http://pandas.pydata.org/
-        .. _LICENSE: LICENSE
-        
 Platform: any
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
@@ -73,7 +17,60 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+---
+title: sparqldataframe
+---
+
+[![image](https://img.shields.io/pypi/v/sparqldataframe.svg)](https://pypi.python.org/pypi/sparqldataframe)
+
+A Python library that can send
+[SPARQL](https://en.wikipedia.org/wiki/SPARQL) queries to a SPARQL
+endpoint and retrieve a [Pandas](http://pandas.pydata.org/) dataframe
+from the result.
+
+# Installation
+
+``` bash
+pip install sparqldataframe
+```
+
+# Usage
+
+Here is an example how to run a SPARQL query on the
+[Wikidata](http://wikidata.org/) endpoint:
+
+``` python
+import sparqldataframe
+
+sparql_query = """
+SELECT ?item ?itemLabel 
+WHERE {
+  ?item wdt:P31 wd:Q146.
+  SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
+}
+"""
+df = sparqldataframe.query("https://query.wikidata.org/sparql", sparql_query)
+```
+
+Wikidata and [DBPedia](http://dbpedia.org/) can be both used without
+adding the SPARQL endpoint url by using the `wikidata_query()` and
+`dbpedia_query()` functions respectively:
+
+``` python
+df = sparqldataframe.wikidata_query(sparql_query)
+df = sparqldataframe.dbpedia_query(sparql_query)
+```
+
+# License
+
+This project is licensed under the MIT license. See the
+[LICENSE](LICENSE) for details.
+
+
```

### Comparing `sparqldataframe-0.1.0/sparqldataframe.egg-info/PKG-INFO` & `sparqldataframe-0.1.1/sparqldataframe.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: sparqldataframe
-Version: 0.1.0
+Version: 0.1.1
 Summary: Get a Pandas dataframe from SPARQL queries
 Home-page: https://github.com/njanakiev/sparqldataframe
 Author: Nikolai Janakiev
 Author-email: nikolai.janakiev@gmail.com
 License: MIT
-Description: sparqldataframe
-        ===============
-        
-        .. image:: https://img.shields.io/pypi/v/sparqldataframe.svg
-                :target: https://pypi.python.org/pypi/sparqldataframe
-        
-        
-        A Python library that can send `SPARQL`_ queries to a SPARQL endpoint and retrieve a `Pandas`_ dataframe from the result.
-        
-        
-        Installation
-        ------------
-        
-        .. code-block:: bash
-        	
-        	pip install sparqldataframe
-        
-        
-        Usage
-        -----
-        
-        Here is an example how to run a SPARQL query on the `Wikidata`_ endpoint:
-        
-        .. code-block:: python
-        	
-        	import sparqldataframe
-        
-        	sparql_query = """
-        	SELECT ?item ?itemLabel 
-        	WHERE {
-        	  ?item wdt:P31 wd:Q146.
-        	  SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
-        	}
-        	"""
-        	df = sparqldataframe.query("https://query.wikidata.org/sparql", sparql_query)
-        
-        Wikidata and `DBPedia`_ can be both used without adding the SPARQL endpoint url by using the :code:`wikidata_query()` and :code:`dbpedia_query()` functions respectively:
-        
-        .. code-block:: python
-        
-        	df = sparqldataframe.wikidata_query(sparql_query)
-        	df = sparqldataframe.dbpedia_query(sparql_query)
-        
-        
-        License 
-        -------
-        
-        This project is licensed under the MIT license. See the `LICENSE`_ for details.
-        
-        
-        .. _SPARQL: https://en.wikipedia.org/wiki/SPARQL
-        .. _Wikidata: http://wikidata.org/
-        .. _DBPedia: http://dbpedia.org/
-        .. _Pandas: http://pandas.pydata.org/
-        .. _LICENSE: LICENSE
-        
 Platform: any
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
@@ -73,7 +17,60 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+---
+title: sparqldataframe
+---
+
+[![image](https://img.shields.io/pypi/v/sparqldataframe.svg)](https://pypi.python.org/pypi/sparqldataframe)
+
+A Python library that can send
+[SPARQL](https://en.wikipedia.org/wiki/SPARQL) queries to a SPARQL
+endpoint and retrieve a [Pandas](http://pandas.pydata.org/) dataframe
+from the result.
+
+# Installation
+
+``` bash
+pip install sparqldataframe
+```
+
+# Usage
+
+Here is an example how to run a SPARQL query on the
+[Wikidata](http://wikidata.org/) endpoint:
+
+``` python
+import sparqldataframe
+
+sparql_query = """
+SELECT ?item ?itemLabel 
+WHERE {
+  ?item wdt:P31 wd:Q146.
+  SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
+}
+"""
+df = sparqldataframe.query("https://query.wikidata.org/sparql", sparql_query)
+```
+
+Wikidata and [DBPedia](http://dbpedia.org/) can be both used without
+adding the SPARQL endpoint url by using the `wikidata_query()` and
+`dbpedia_query()` functions respectively:
+
+``` python
+df = sparqldataframe.wikidata_query(sparql_query)
+df = sparqldataframe.dbpedia_query(sparql_query)
+```
+
+# License
+
+This project is licensed under the MIT license. See the
+[LICENSE](LICENSE) for details.
+
+
```

### Comparing `sparqldataframe-0.1.0/sparqldataframe/__init__.py` & `sparqldataframe-0.1.1/sparqldataframe/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 import pandas as pd
 from simplejson import JSONDecodeError
 import requests
 
 
 def dbpedia_query(sparql_query):
@@ -13,15 +13,23 @@
 def wikidata_query(sparql_query):
     url = 'https://query.wikidata.org/sparql'
     return query(url, sparql_query)
 
 
 def query(url, sparql_query):
     try:
-        r = requests.get(url, params={'format': 'json', 'query': sparql_query})
+        r = requests.get(
+            url,
+            params={
+                'format': 'json',
+                'query': sparql_query
+            },
+            headers={
+                "accept": "application/sparql-results+json"
+            })
         data = r.json()
     except JSONDecodeError as e:
         print(r.content)
         raise Exception('Invalid query')
 
     if ('results' in data) and ('bindings' in data['results']):
         columns = data['head']['vars']
```

