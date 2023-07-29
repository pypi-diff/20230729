# Comparing `tmp/sparqldataframe-0.1.1.tar.gz` & `tmp/sparqldataframe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparqldataframe-0.1.1.tar", last modified: Sat Jul 29 11:26:57 2023, max compression
+gzip compressed data, was "sparqldataframe-0.1.2.tar", last modified: Sat Jul 29 12:05:09 2023, max compression
```

## Comparing `sparqldataframe-0.1.1.tar` & `sparqldataframe-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 nikolai   (1000) nikolai   (1000)        0 2023-07-29 11:26:57.553032 sparqldataframe-0.1.1/
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     1073 2023-07-26 15:02:34.000000 sparqldataframe-0.1.1/LICENSE
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     2175 2023-07-29 11:26:57.553032 sparqldataframe-0.1.1/PKG-INFO
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     1169 2023-07-29 11:11:44.000000 sparqldataframe-0.1.1/README.md
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)       38 2023-07-29 11:26:57.553032 sparqldataframe-0.1.1/setup.cfg
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     2294 2023-07-29 11:25:59.000000 sparqldataframe-0.1.1/setup.py
-drwxrwxr-x   0 nikolai   (1000) nikolai   (1000)        0 2023-07-29 11:26:57.549033 sparqldataframe-0.1.1/sparqldataframe/
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     1100 2023-07-29 10:53:55.000000 sparqldataframe-0.1.1/sparqldataframe/__init__.py
-drwxrwxr-x   0 nikolai   (1000) nikolai   (1000)        0 2023-07-29 11:26:57.553032 sparqldataframe-0.1.1/sparqldataframe.egg-info/
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     2175 2023-07-29 11:26:56.000000 sparqldataframe-0.1.1/sparqldataframe.egg-info/PKG-INFO
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)      248 2023-07-29 11:26:57.000000 sparqldataframe-0.1.1/sparqldataframe.egg-info/SOURCES.txt
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)        1 2023-07-29 11:26:56.000000 sparqldataframe-0.1.1/sparqldataframe.egg-info/dependency_links.txt
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)       27 2023-07-29 11:26:57.000000 sparqldataframe-0.1.1/sparqldataframe.egg-info/requires.txt
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)       16 2023-07-29 11:26:57.000000 sparqldataframe-0.1.1/sparqldataframe.egg-info/top_level.txt
+drwxrwxr-x   0 nikolai   (1000) nikolai   (1000)        0 2023-07-29 12:05:09.366138 sparqldataframe-0.1.2/
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     1073 2023-07-26 15:02:34.000000 sparqldataframe-0.1.2/LICENSE
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     2357 2023-07-29 12:05:09.366138 sparqldataframe-0.1.2/PKG-INFO
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     1351 2023-07-29 11:51:46.000000 sparqldataframe-0.1.2/README.md
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)       38 2023-07-29 12:05:09.366138 sparqldataframe-0.1.2/setup.cfg
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     2294 2023-07-29 11:25:59.000000 sparqldataframe-0.1.2/setup.py
+drwxrwxr-x   0 nikolai   (1000) nikolai   (1000)        0 2023-07-29 12:05:09.366138 sparqldataframe-0.1.2/sparqldataframe/
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     1875 2023-07-29 12:03:10.000000 sparqldataframe-0.1.2/sparqldataframe/__init__.py
+drwxrwxr-x   0 nikolai   (1000) nikolai   (1000)        0 2023-07-29 12:05:09.366138 sparqldataframe-0.1.2/sparqldataframe.egg-info/
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     2357 2023-07-29 12:05:08.000000 sparqldataframe-0.1.2/sparqldataframe.egg-info/PKG-INFO
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)      248 2023-07-29 12:05:09.000000 sparqldataframe-0.1.2/sparqldataframe.egg-info/SOURCES.txt
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)        1 2023-07-29 12:05:08.000000 sparqldataframe-0.1.2/sparqldataframe.egg-info/dependency_links.txt
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)       27 2023-07-29 12:05:09.000000 sparqldataframe-0.1.2/sparqldataframe.egg-info/requires.txt
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)       16 2023-07-29 12:05:09.000000 sparqldataframe-0.1.2/sparqldataframe.egg-info/top_level.txt
```

### Comparing `sparqldataframe-0.1.1/LICENSE` & `sparqldataframe-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sparqldataframe-0.1.1/PKG-INFO` & `sparqldataframe-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparqldataframe
-Version: 0.1.1
+Version: 0.1.2
 Summary: Get a Pandas dataframe from SPARQL queries
 Home-page: https://github.com/njanakiev/sparqldataframe
 Author: Nikolai Janakiev
 Author-email: nikolai.janakiev@gmail.com
 License: MIT
 Platform: any
 Classifier: Environment :: Console
@@ -20,17 +20,15 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
----
-title: sparqldataframe
----
+# sparqldataframe
 
 [![image](https://img.shields.io/pypi/v/sparqldataframe.svg)](https://pypi.python.org/pypi/sparqldataframe)
 
 A Python library that can send
 [SPARQL](https://en.wikipedia.org/wiki/SPARQL) queries to a SPARQL
 endpoint and retrieve a [Pandas](http://pandas.pydata.org/) dataframe
 from the result.
@@ -46,21 +44,30 @@
 Here is an example how to run a SPARQL query on the
 [Wikidata](http://wikidata.org/) endpoint:
 
 ``` python
 import sparqldataframe
 
 sparql_query = """
+PREFIX wd: <http://www.wikidata.org/entity/>
+PREFIX wdt: <http://www.wikidata.org/prop/direct/>
+PREFIX wikibase: <http://wikiba.se/ontology#>
+PREFIX bd: <http://www.bigdata.com/rdf#>
+
 SELECT ?item ?itemLabel 
 WHERE {
   ?item wdt:P31 wd:Q146.
-  SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
+  SERVICE wikibase:label {
+    bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en".
+  }
 }
 """
-df = sparqldataframe.query("https://query.wikidata.org/sparql", sparql_query)
+df = sparqldataframe.query(
+  "https://query.wikidata.org/sparql",
+  sparql_query)
 ```
 
 Wikidata and [DBPedia](http://dbpedia.org/) can be both used without
 adding the SPARQL endpoint url by using the `wikidata_query()` and
 `dbpedia_query()` functions respectively:
 
 ``` python
```

### Comparing `sparqldataframe-0.1.1/README.md` & `sparqldataframe-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,8 @@
----
-title: sparqldataframe
----
+# sparqldataframe
 
 [![image](https://img.shields.io/pypi/v/sparqldataframe.svg)](https://pypi.python.org/pypi/sparqldataframe)
 
 A Python library that can send
 [SPARQL](https://en.wikipedia.org/wiki/SPARQL) queries to a SPARQL
 endpoint and retrieve a [Pandas](http://pandas.pydata.org/) dataframe
 from the result.
@@ -20,21 +18,30 @@
 Here is an example how to run a SPARQL query on the
 [Wikidata](http://wikidata.org/) endpoint:
 
 ``` python
 import sparqldataframe
 
 sparql_query = """
+PREFIX wd: <http://www.wikidata.org/entity/>
+PREFIX wdt: <http://www.wikidata.org/prop/direct/>
+PREFIX wikibase: <http://wikiba.se/ontology#>
+PREFIX bd: <http://www.bigdata.com/rdf#>
+
 SELECT ?item ?itemLabel 
 WHERE {
   ?item wdt:P31 wd:Q146.
-  SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
+  SERVICE wikibase:label {
+    bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en".
+  }
 }
 """
-df = sparqldataframe.query("https://query.wikidata.org/sparql", sparql_query)
+df = sparqldataframe.query(
+  "https://query.wikidata.org/sparql",
+  sparql_query)
 ```
 
 Wikidata and [DBPedia](http://dbpedia.org/) can be both used without
 adding the SPARQL endpoint url by using the `wikidata_query()` and
 `dbpedia_query()` functions respectively:
 
 ``` python
```

### Comparing `sparqldataframe-0.1.1/setup.py` & `sparqldataframe-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `sparqldataframe-0.1.1/sparqldataframe.egg-info/PKG-INFO` & `sparqldataframe-0.1.2/sparqldataframe.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparqldataframe
-Version: 0.1.1
+Version: 0.1.2
 Summary: Get a Pandas dataframe from SPARQL queries
 Home-page: https://github.com/njanakiev/sparqldataframe
 Author: Nikolai Janakiev
 Author-email: nikolai.janakiev@gmail.com
 License: MIT
 Platform: any
 Classifier: Environment :: Console
@@ -20,17 +20,15 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
----
-title: sparqldataframe
----
+# sparqldataframe
 
 [![image](https://img.shields.io/pypi/v/sparqldataframe.svg)](https://pypi.python.org/pypi/sparqldataframe)
 
 A Python library that can send
 [SPARQL](https://en.wikipedia.org/wiki/SPARQL) queries to a SPARQL
 endpoint and retrieve a [Pandas](http://pandas.pydata.org/) dataframe
 from the result.
@@ -46,21 +44,30 @@
 Here is an example how to run a SPARQL query on the
 [Wikidata](http://wikidata.org/) endpoint:
 
 ``` python
 import sparqldataframe
 
 sparql_query = """
+PREFIX wd: <http://www.wikidata.org/entity/>
+PREFIX wdt: <http://www.wikidata.org/prop/direct/>
+PREFIX wikibase: <http://wikiba.se/ontology#>
+PREFIX bd: <http://www.bigdata.com/rdf#>
+
 SELECT ?item ?itemLabel 
 WHERE {
   ?item wdt:P31 wd:Q146.
-  SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
+  SERVICE wikibase:label {
+    bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en".
+  }
 }
 """
-df = sparqldataframe.query("https://query.wikidata.org/sparql", sparql_query)
+df = sparqldataframe.query(
+  "https://query.wikidata.org/sparql",
+  sparql_query)
 ```
 
 Wikidata and [DBPedia](http://dbpedia.org/) can be both used without
 adding the SPARQL endpoint url by using the `wikidata_query()` and
 `dbpedia_query()` functions respectively:
 
 ``` python
```

