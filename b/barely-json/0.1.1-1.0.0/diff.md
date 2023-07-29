# Comparing `tmp/barely_json-0.1.1.tar.gz` & `tmp/barely_json-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/barely_json-0.1.1.tar", last modified: Fri May 12 21:15:56 2017, max compression
+gzip compressed data, was "/home/torf/projects/barely_json/dist/.tmp-qabgg_it/barely_json-1.0.0.tar", last modified: Sat Jul 29 14:56:06 2023, max compression
```

## Comparing `barely_json-0.1.1.tar` & `barely_json-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxr-x   0 torf      (1000) torf      (1000)        0 2017-05-12 21:15:56.000000 barely_json-0.1.1/
-drwxrwxr-x   0 torf      (1000) torf      (1000)        0 2017-05-12 21:15:56.000000 barely_json-0.1.1/barely_json/
--rw-rw-r--   0 torf      (1000) torf      (1000)     6041 2017-05-12 21:14:37.000000 barely_json-0.1.1/barely_json/__init__.py
--rw-rw-r--   0 torf      (1000) torf      (1000)       38 2017-05-12 21:15:56.000000 barely_json-0.1.1/setup.cfg
--rw-rw-r--   0 torf      (1000) torf      (1000)     1085 2017-05-12 15:38:23.000000 barely_json-0.1.1/LICENSE
--rw-rw-r--   0 torf      (1000) torf      (1000)      654 2017-05-12 21:14:05.000000 barely_json-0.1.1/CHANGELOG.md
--rw-rw-r--   0 torf      (1000) torf      (1000)     1017 2017-05-12 21:15:56.000000 barely_json-0.1.1/PKG-INFO
--rw-rw-r--   0 torf      (1000) torf      (1000)     3072 2017-05-12 20:51:20.000000 barely_json-0.1.1/README.md
--rw-rw-r--   0 torf      (1000) torf      (1000)       81 2017-05-12 16:11:35.000000 barely_json-0.1.1/MANIFEST.in
-drwxrwxr-x   0 torf      (1000) torf      (1000)        0 2017-05-12 21:15:56.000000 barely_json-0.1.1/barely_json.egg-info/
--rw-rw-r--   0 torf      (1000) torf      (1000)        1 2017-05-12 21:15:56.000000 barely_json-0.1.1/barely_json.egg-info/dependency_links.txt
--rw-rw-r--   0 torf      (1000) torf      (1000)     1017 2017-05-12 21:15:56.000000 barely_json-0.1.1/barely_json.egg-info/PKG-INFO
--rw-rw-r--   0 torf      (1000) torf      (1000)      266 2017-05-12 21:15:56.000000 barely_json-0.1.1/barely_json.egg-info/SOURCES.txt
--rw-rw-r--   0 torf      (1000) torf      (1000)       29 2017-05-12 21:15:56.000000 barely_json-0.1.1/barely_json.egg-info/requires.txt
--rw-rw-r--   0 torf      (1000) torf      (1000)       12 2017-05-12 21:15:56.000000 barely_json-0.1.1/barely_json.egg-info/top_level.txt
--rwxrwxr-x   0 torf      (1000) torf      (1000)     2102 2017-05-12 16:27:17.000000 barely_json-0.1.1/setup.py
--rw-rw-r--   0 torf      (1000) torf      (1000)      161 2017-05-11 21:09:45.000000 barely_json-0.1.1/requirements.txt
+drwxrwxr-x   0 torf      (1000) torf      (1000)        0 2023-07-29 14:56:06.000000 barely_json-1.0.0/
+-rw-rw-r--   0 torf      (1000) torf      (1000)     1343 2023-07-29 14:34:59.000000 barely_json-1.0.0/CHANGELOG.md
+-rw-rw-r--   0 torf      (1000) torf      (1000)     1085 2017-05-12 15:38:23.000000 barely_json-1.0.0/LICENSE
+-rw-rw-r--   0 torf      (1000) torf      (1000)       81 2017-05-12 16:11:35.000000 barely_json-1.0.0/MANIFEST.in
+-rw-rw-r--   0 torf      (1000) torf      (1000)     4010 2023-07-29 14:56:06.000000 barely_json-1.0.0/PKG-INFO
+-rw-rw-r--   0 torf      (1000) torf      (1000)     3168 2023-07-29 14:38:38.000000 barely_json-1.0.0/README.md
+drwxrwxr-x   0 torf      (1000) torf      (1000)        0 2023-07-29 14:56:06.000000 barely_json-1.0.0/barely_json/
+-rw-rw-r--   0 torf      (1000) torf      (1000)     5765 2023-07-29 14:32:24.000000 barely_json-1.0.0/barely_json/__init__.py
+drwxrwxr-x   0 torf      (1000) torf      (1000)        0 2023-07-29 14:56:06.000000 barely_json-1.0.0/barely_json.egg-info/
+-rw-rw-r--   0 torf      (1000) torf      (1000)     4010 2023-07-29 14:56:06.000000 barely_json-1.0.0/barely_json.egg-info/PKG-INFO
+-rw-rw-r--   0 torf      (1000) torf      (1000)      292 2023-07-29 14:56:06.000000 barely_json-1.0.0/barely_json.egg-info/SOURCES.txt
+-rw-rw-r--   0 torf      (1000) torf      (1000)        1 2023-07-29 14:56:06.000000 barely_json-1.0.0/barely_json.egg-info/dependency_links.txt
+-rw-rw-r--   0 torf      (1000) torf      (1000)       17 2023-07-29 14:56:06.000000 barely_json-1.0.0/barely_json.egg-info/requires.txt
+-rw-rw-r--   0 torf      (1000) torf      (1000)       12 2023-07-29 14:56:06.000000 barely_json-1.0.0/barely_json.egg-info/top_level.txt
+-rw-rw-r--   0 torf      (1000) torf      (1000)       17 2023-07-29 14:32:24.000000 barely_json-1.0.0/requirements.txt
+-rw-rw-r--   0 torf      (1000) torf      (1000)       38 2023-07-29 14:56:06.000000 barely_json-1.0.0/setup.cfg
+-rwxrwxr-x   0 torf      (1000) torf      (1000)     1860 2023-07-29 14:52:12.000000 barely_json-1.0.0/setup.py
+drwxrwxr-x   0 torf      (1000) torf      (1000)        0 2023-07-29 14:56:06.000000 barely_json-1.0.0/tests/
+-rw-rw-r--   0 torf      (1000) torf      (1000)     6589 2023-07-29 14:32:24.000000 barely_json-1.0.0/tests/test_barely_json.py
```

### Comparing `barely_json-0.1.1/barely_json/__init__.py` & `barely_json-1.0.0/barely_json/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 #!/usr/bin/env python
-# encoding: utf-8
 
 '''
 A very forgiving JSON parser.
 '''
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import codecs
 import re
 
-from six import iteritems
 from pyparsing import *
 
 
-__version__ = '0.1.1'
+__version__ = '1.0.0'
 
 
-class IllegalValue(object):
+class IllegalValue:
     '''
     A value that is illegal in JSON.
 
     ``parse`` wraps anything that isn't standard JSON into an
     ``IllegalValue`` instance. By default, these are then automatically
     resolved into standard Python types via ``resolve``. However, if you
     pass ``resolver=None`` to ``parse`` and your input contains illegal
@@ -37,15 +32,15 @@
         Constructor.
 
         ``source`` is a string.
         '''
         self.source = source
 
     def __str__(self):
-        return source
+        return self.source
 
     def __repr__(self):
         return '<{} {!r}>'.format(self.__class__.__name__, self.source)
 
     def __eq__(self, other):
         return (isinstance(other, self.__class__) and
                 other.source == self.source)
@@ -73,17 +68,15 @@
 ESCAPE_SEQUENCE_RE = re.compile(r'''
     ( \\U........      # 8-digit hex escapes
     | \\u....          # 4-digit hex escapes
     | \\x..            # 2-digit hex escapes
     | \\[0-7]{1,3}     # Octal escapes
     | \\N\{[^}]+\}     # Unicode characters by name
     | \\[\\'"abfnrtv]  # Single-character escapes
-    )''',
-    re.UNICODE | re.VERBOSE
-)
+    )''', re.UNICODE | re.VERBOSE)
 
 
 def decode_escapes(s):
     '''
     Decode string escape sequences.
     '''
     def decode_match(match):
@@ -179,23 +172,17 @@
 
     ``resolver`` is a function that maps strings to arbitrary values.
 
     All instances of ``IllegalValue`` in ``data`` are replaced by the
     result of feeding them into ``resolver``.
     '''
     if isinstance(data, list):
-        items = []
-        for item in data:
-            items.append(resolve(item, resolver))
-        return items
+        return [resolve(item, resolver) for item in data]
     if isinstance(data, dict):
-        items = {}
-        for key, value in iteritems(data):
-            items[resolve(key, resolver)] = resolve(value, resolver)
-        return items
+        return {resolve(key, resolver): resolve(value, resolver) for key, value in data.items()}
     if isinstance(data, IllegalValue):
         return resolver(data.source)
     return data
 
 
 def parse(s, resolver=default_resolver):
     '''
@@ -207,8 +194,7 @@
     callback or to a falsy value to modify or disable that mechanism.
     '''
     parsed = value.parseString(s, parseAll=True)
     data = parsed.asList()[0]
     if resolver:
         data = resolve(data, resolver=resolver)
     return data
-
```

### Comparing `barely_json-0.1.1/LICENSE` & `barely_json-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `barely_json-0.1.1/README.md` & `barely_json-1.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Barely JSON
 
-[![Travis CI badge](https://travis-ci.org/torfsen/barely_json.svg?branch=master)](https://travis-ci.org/torfsen/barely_json)
+[![GitHub Actions badge](https://github.com/torfsen/barely_json/actions/workflows/test.yml/badge.svg)](https://github.com/torfsen/barely_json/actions/workflows/test.yml)
 
 *A Python package for parsing data that only looks like JSON*
 
     from barely_json import parse
     print(parse('[what is this?, , {perhaps, json: no}]'))
 
     # Prints ['what is this?', '', {'perhaps': '', 'json': False}]
@@ -14,17 +14,15 @@
 No matter how you ended up with the data, now you want to parse it! However, most JSON parsers are pretty strict, so you're out of luck with your JSON-esque mess.
 
 That's where *Barely JSON* steps in and tries to parse anything that remotely looks like JSON. In addition to the pure parsing, *Barely JSON* will also try to post-process your data into suitable Python types even if your data provider uses, for example, `on` and `off` as boolean literals.
 
 
 # Installation
 
-The supported Python versions are 2.7 as well as 3.3 and later.
-
-As usual it's recommended to use a [virtualenv] to keep things tidy.
+The supported Python versions are 3.7 and later.
 
     pip install barely_json
 
 
 # Usage
 
 The main routine is `parse`:
@@ -66,28 +64,34 @@
 
 
 # License
 
 Distributed under the MIT license. See the file `LICENSE` for details.
 
 
+# Contributors
+
+* [@torfsen](https://github.com/torfsen)
+* [@tusharmakkar08](https://github.com/tusharmakkar08)
+* [@gvx](https://github.com/gvx)
+
+
 # Development
 
 Clone the repository:
 
     git clone https://github.com/torfsen/barely_json.git
     cd barely_json
 
-Install [tox] locally in a [virtualenv] if you haven't installed it globally:
+Install the development dependencies
 
-    virtualenv venv
-    source venv/bin/activate
-    pip install tox
+    pip install -r requirements-dev.txt
 
 Run the tests:
 
     tox
 
+For pull requests, the tests are run using GitHub actions.
+
 
 [virtualenv]: https://virtualenv.pypa.io
 [tox]: https://tox.readthedocs.io
-
```

### Comparing `barely_json-0.1.1/setup.py` & `barely_json-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,59 @@
 #!/usr/bin/env python
-# encoding: utf-8
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
-import io
 import os.path
 import re
 
 from setuptools import find_packages, setup
 
 HERE = os.path.dirname(__file__)
 
 # Extract version
 SOURCE_FILE = os.path.join(HERE, 'barely_json', '__init__.py')
 version = None
-with io.open(SOURCE_FILE, 'r', encoding='utf-8') as f:
+with open(SOURCE_FILE, 'r', encoding='utf-8') as f:
     for line in f:
         s = line.strip()
         m = re.match(r"""__version__\s*=\s*['"](.*)['"]""", line)
         if m:
             version = m.groups()[0]
 if not version:
     raise RuntimeError('Could not extract version from "%s".' % SOURCE_FILE)
 
 # Extract requirements
 REQUIREMENTS_FILE = os.path.join(HERE, 'requirements.txt')
-with io.open(REQUIREMENTS_FILE, 'r', encoding='utf-8') as f:
+with open(REQUIREMENTS_FILE, 'r') as f:
     requirements = f.readlines()
 
-long_description = """
-A lot of data is encoded in a format that is similar to JSON but not quite valid JSON. This module tries to be as forgiving as possible while parsing such data.
-""".strip()
+README_FILE = os.path.join(HERE, 'README.md')
+with open(README_FILE, 'r') as f:
+    long_description =f.read()
 
 setup(
     name='barely_json',
     description='Parse invalid, malformed and barely JSON-esque data',
     long_description=long_description,
+    long_description_content_type='text/markdown',
     url='https://github.com/torfsen/barely_json',
     version=version,
     license='MIT',
     keywords=['json'],
     classifiers=[
         # Reference: http://pypi.python.org/pypi?%3Aaction=list_classifiers
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 
     author='Florian Brucker',
     author_email='mail@florianbrucker.de',
 
     packages=find_packages(),
     install_requires=requirements,
 )
-
```

