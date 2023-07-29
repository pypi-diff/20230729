# Comparing `tmp/abstract_webtools-0.0.12.tar.gz` & `tmp/abstract_webtools-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_webtools-0.0.12.tar", last modified: Sat Jul 29 19:40:42 2023, max compression
+gzip compressed data, was "abstract_webtools-0.0.13.tar", last modified: Sat Jul 29 19:45:51 2023, max compression
```

## Comparing `abstract_webtools-0.0.12.tar` & `abstract_webtools-0.0.13.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:40:42.384369 abstract_webtools-0.0.12/
--rw-r--r--   0 root         (0) root         (0)     4913 2023-07-29 19:40:42.384369 abstract_webtools-0.0.12/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4273 2023-07-29 19:29:32.000000 abstract_webtools-0.0.12/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_webtools-0.0.12/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-07-29 19:40:42.384369 abstract_webtools-0.0.12/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1217 2023-07-29 19:39:27.000000 abstract_webtools-0.0.12/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:40:42.384369 abstract_webtools-0.0.12/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:40:42.384369 abstract_webtools-0.0.12/src/abstract_webtools/
--rw-rw-r--   0 root         (0) root         (0)       28 2023-07-29 19:28:16.000000 abstract_webtools-0.0.12/src/abstract_webtools/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1329 2023-07-29 19:09:21.000000 abstract_webtools-0.0.12/src/abstract_webtools/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:40:42.384369 abstract_webtools-0.0.12/src/abstract_webtools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4913 2023-07-29 19:40:42.000000 abstract_webtools-0.0.12/src/abstract_webtools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-07-29 19:40:42.000000 abstract_webtools-0.0.12/src/abstract_webtools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 19:40:42.000000 abstract_webtools-0.0.12/src/abstract_webtools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-29 19:40:42.000000 abstract_webtools-0.0.12/src/abstract_webtools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-29 19:40:42.000000 abstract_webtools-0.0.12/src/abstract_webtools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:45:51.244279 abstract_webtools-0.0.13/
+-rw-r--r--   0 root         (0) root         (0)     3788 2023-07-29 19:45:51.244279 abstract_webtools-0.0.13/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3111 2023-07-29 19:45:03.000000 abstract_webtools-0.0.13/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_webtools-0.0.13/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-29 19:45:51.244279 abstract_webtools-0.0.13/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1217 2023-07-29 19:45:13.000000 abstract_webtools-0.0.13/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:45:51.244279 abstract_webtools-0.0.13/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:45:51.244279 abstract_webtools-0.0.13/src/abstract_webtools/
+-rw-rw-r--   0 root         (0) root         (0)       28 2023-07-29 19:28:16.000000 abstract_webtools-0.0.13/src/abstract_webtools/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1329 2023-07-29 19:09:21.000000 abstract_webtools-0.0.13/src/abstract_webtools/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:45:51.244279 abstract_webtools-0.0.13/src/abstract_webtools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3788 2023-07-29 19:45:51.000000 abstract_webtools-0.0.13/src/abstract_webtools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-07-29 19:45:51.000000 abstract_webtools-0.0.13/src/abstract_webtools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 19:45:51.000000 abstract_webtools-0.0.13/src/abstract_webtools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-29 19:45:51.000000 abstract_webtools-0.0.13/src/abstract_webtools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-29 19:45:51.000000 abstract_webtools-0.0.13/src/abstract_webtools.egg-info/top_level.txt
```

### Comparing `abstract_webtools-0.0.12/PKG-INFO` & `abstract_webtools-0.0.13/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,45 @@
 Metadata-Version: 2.1
 Name: abstract_webtools
-Version: 0.0.12
+Version: 0.0.13
 Summary: Abstract Web Tools is a Python package that provides various utility functions for web scraping tasks. It is built on top of popular libraries such as `requests`, `BeautifulSoup`, and `urllib3` to simplify the process of fetching and parsing web content.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_webtools
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ```
-# abstract_webtools
-
-[![PyPI version](https://badge.fury.io/py/web-scraping-toolkit.svg)](https://badge.fury.io/py/web-scraping-toolkit)
-
-Abstract Web Tools is a Python package that provides various utility functions for web scraping tasks. It is built on top of popular libraries such as `requests`, `BeautifulSoup`, and `urllib3` to simplify the process of fetching and parsing web content.
+# abstract_webtools for parsing web content.
 
 ## Installation
 
 You can install the package via pip:
 
 ```bash
 pip install abstract_webtools
 ```
 
 ## Usage
 
-### Format URL
-
-The `format_url` function ensures that the URL has a valid format and adds the 'https://' prefix if missing.
-
-```python
-from abstract_webtools import format_url
-
-url = format_url('example.com')
-print(url)  # Output: 'https://example.com'
-```
-
 ### Get Status Code
 
 The `get_status` function fetches the status code of the URL.
 
 ```python
-from abstract_webtools import get_status
-
-status_code = get_status('https://www.example.com')
-print(status_code)  # Output: 200
-```
-
-### Clean URL
-
-The `clean_url` function returns a list of possible URL variations for a given URL.
-
-```python
-from abstract_webtools import clean_url
+from abstract_webtn_url
 
 urls = clean_url('https://example.com')
 print(urls)  # Output: ['https://example.com', 'http://example.com']
-```
-
-### Get Correct URL
-
-The `get_correct_url` function returns the correct URL from the possible variations by attempting HTTP requests.
-
-```python
-from abstract_webtools import get_correct_url
-
-url = get_correct_url('example.com')
-print(url)  # Output: 'https://example.com'
+tps://example.com'
 ```
 
 ### Try Request
 
 The `try_request` function makes HTTP requests to a URL and returns the response if successful.
 
 ```python
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_wgjym40g_/tmpqxapmjok_TarContainer/0/1", line 161, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_wgjym40g_/tmpqxapmjok_TarContainer/0/1", line 161, column 0: CDATA terminal not found*

```diff
@@ -1,41 +1,26 @@
-Metadata-Version: 2.1 Name: abstract_webtools Version: 0.0.12 Summary: Abstract
+Metadata-Version: 2.1 Name: abstract_webtools Version: 0.0.13 Summary: Abstract
 Web Tools is a Python package that provides various utility functions for web
 scraping tasks. It is built on top of popular libraries such as `requests`,
 `BeautifulSoup`, and `urllib3` to simplify the process of fetching and parsing
 web content. Home-page: https://github.com/AbstractEndeavors/
 abstract_essentials/tree/main/abstract_webtools Author: putkoff Author-email:
 partners@abstractendeavors.com Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.11 Requires-Python: >=3.6 Description-
-Content-Type: text/markdown ``` # abstract_webtools [![PyPI version](https://
-badge.fury.io/py/web-scraping-toolkit.svg)](https://badge.fury.io/py/web-
-scraping-toolkit) Abstract Web Tools is a Python package that provides various
-utility functions for web scraping tasks. It is built on top of popular
-libraries such as `requests`, `BeautifulSoup`, and `urllib3` to simplify the
-process of fetching and parsing web content. ## Installation You can install
-the package via pip: ```bash pip install abstract_webtools ``` ## Usage ###
-Format URL The `format_url` function ensures that the URL has a valid format
-and adds the 'https://' prefix if missing. ```python from abstract_webtools
-import format_url url = format_url('example.com') print(url) # Output: 'https:/
-/example.com' ``` ### Get Status Code The `get_status` function fetches the
-status code of the URL. ```python from abstract_webtools import get_status
-status_code = get_status('https://www.example.com') print(status_code) #
-Output: 200 ``` ### Clean URL The `clean_url` function returns a list of
-possible URL variations for a given URL. ```python from abstract_webtools
-import clean_url urls = clean_url('https://example.com') print(urls) # Output:
-['https://example.com', 'http://example.com'] ``` ### Get Correct URL The
-`get_correct_url` function returns the correct URL from the possible variations
-by attempting HTTP requests. ```python from abstract_webtools import
-get_correct_url url = get_correct_url('example.com') print(url) # Output:
-'https://example.com' ``` ### Try Request The `try_request` function makes HTTP
-requests to a URL and returns the response if successful. ```python from
-abstract_webtools import try_request response = try_request('https://
-www.example.com') print(response) # Output:
+Content-Type: text/markdown ``` # abstract_webtools for parsing web content. ##
+Installation You can install the package via pip: ```bash pip install
+abstract_webtools ``` ## Usage ### Get Status Code The `get_status` function
+fetches the status code of the URL. ```python from abstract_webtn_url urls =
+clean_url('https://example.com') print(urls) # Output: ['https://example.com',
+'http://example.com'] tps://example.com' ``` ### Try Request The `try_request`
+function makes HTTP requests to a URL and returns the response if successful.
+```python from abstract_webtools import try_request response = try_request
+('https://www.example.com') print(response) # Output:
 200]> ``` ### Is Valid URL The `is_valid` function checks whether a given URL
 is valid. ```python from abstract_webtools import is_valid valid = is_valid
 ('https://www.example.com') print(valid) # Output: True ``` ### Get Source Code
 The `get_Source_code` function fetches the source code of a URL with a custom
 user-agent. ```python from abstract_webtools import get_Source_code source_code
 = get_Source_code('https://www.example.com') print(source_code) # Output: HTML
 source code of the URL ``` ### Parse React Source The `parse_react_source`
```

### Comparing `abstract_webtools-0.0.12/setup.py` & `abstract_webtools-0.0.13/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_webtools',
-    version='0.0.12',
+    version='0.0.13',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='Abstract Web Tools is a Python package that provides various utility functions for web scraping tasks. It is built on top of popular libraries such as `requests`, `BeautifulSoup`, and `urllib3` to simplify the process of fetching and parsing web content.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_webtools',
     classifiers=[
```

### Comparing `abstract_webtools-0.0.12/src/abstract_webtools/main.py` & `abstract_webtools-0.0.13/src/abstract_webtools/main.py`

 * *Files identical despite different names*

### Comparing `abstract_webtools-0.0.12/src/abstract_webtools.egg-info/PKG-INFO` & `abstract_webtools-0.0.13/src/abstract_webtools.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,45 @@
 Metadata-Version: 2.1
 Name: abstract-webtools
-Version: 0.0.12
+Version: 0.0.13
 Summary: Abstract Web Tools is a Python package that provides various utility functions for web scraping tasks. It is built on top of popular libraries such as `requests`, `BeautifulSoup`, and `urllib3` to simplify the process of fetching and parsing web content.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_webtools
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ```
-# abstract_webtools
-
-[![PyPI version](https://badge.fury.io/py/web-scraping-toolkit.svg)](https://badge.fury.io/py/web-scraping-toolkit)
-
-Abstract Web Tools is a Python package that provides various utility functions for web scraping tasks. It is built on top of popular libraries such as `requests`, `BeautifulSoup`, and `urllib3` to simplify the process of fetching and parsing web content.
+# abstract_webtools for parsing web content.
 
 ## Installation
 
 You can install the package via pip:
 
 ```bash
 pip install abstract_webtools
 ```
 
 ## Usage
 
-### Format URL
-
-The `format_url` function ensures that the URL has a valid format and adds the 'https://' prefix if missing.
-
-```python
-from abstract_webtools import format_url
-
-url = format_url('example.com')
-print(url)  # Output: 'https://example.com'
-```
-
 ### Get Status Code
 
 The `get_status` function fetches the status code of the URL.
 
 ```python
-from abstract_webtools import get_status
-
-status_code = get_status('https://www.example.com')
-print(status_code)  # Output: 200
-```
-
-### Clean URL
-
-The `clean_url` function returns a list of possible URL variations for a given URL.
-
-```python
-from abstract_webtools import clean_url
+from abstract_webtn_url
 
 urls = clean_url('https://example.com')
 print(urls)  # Output: ['https://example.com', 'http://example.com']
-```
-
-### Get Correct URL
-
-The `get_correct_url` function returns the correct URL from the possible variations by attempting HTTP requests.
-
-```python
-from abstract_webtools import get_correct_url
-
-url = get_correct_url('example.com')
-print(url)  # Output: 'https://example.com'
+tps://example.com'
 ```
 
 ### Try Request
 
 The `try_request` function makes HTTP requests to a URL and returns the response if successful.
 
 ```python
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_wgjym40g_/tmpqxapmjok_TarContainer/0/11", line 161, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_wgjym40g_/tmpqxapmjok_TarContainer/0/11", line 161, column 0: CDATA terminal not found*

```diff
@@ -1,41 +1,26 @@
-Metadata-Version: 2.1 Name: abstract-webtools Version: 0.0.12 Summary: Abstract
+Metadata-Version: 2.1 Name: abstract-webtools Version: 0.0.13 Summary: Abstract
 Web Tools is a Python package that provides various utility functions for web
 scraping tasks. It is built on top of popular libraries such as `requests`,
 `BeautifulSoup`, and `urllib3` to simplify the process of fetching and parsing
 web content. Home-page: https://github.com/AbstractEndeavors/
 abstract_essentials/tree/main/abstract_webtools Author: putkoff Author-email:
 partners@abstractendeavors.com Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.11 Requires-Python: >=3.6 Description-
-Content-Type: text/markdown ``` # abstract_webtools [![PyPI version](https://
-badge.fury.io/py/web-scraping-toolkit.svg)](https://badge.fury.io/py/web-
-scraping-toolkit) Abstract Web Tools is a Python package that provides various
-utility functions for web scraping tasks. It is built on top of popular
-libraries such as `requests`, `BeautifulSoup`, and `urllib3` to simplify the
-process of fetching and parsing web content. ## Installation You can install
-the package via pip: ```bash pip install abstract_webtools ``` ## Usage ###
-Format URL The `format_url` function ensures that the URL has a valid format
-and adds the 'https://' prefix if missing. ```python from abstract_webtools
-import format_url url = format_url('example.com') print(url) # Output: 'https:/
-/example.com' ``` ### Get Status Code The `get_status` function fetches the
-status code of the URL. ```python from abstract_webtools import get_status
-status_code = get_status('https://www.example.com') print(status_code) #
-Output: 200 ``` ### Clean URL The `clean_url` function returns a list of
-possible URL variations for a given URL. ```python from abstract_webtools
-import clean_url urls = clean_url('https://example.com') print(urls) # Output:
-['https://example.com', 'http://example.com'] ``` ### Get Correct URL The
-`get_correct_url` function returns the correct URL from the possible variations
-by attempting HTTP requests. ```python from abstract_webtools import
-get_correct_url url = get_correct_url('example.com') print(url) # Output:
-'https://example.com' ``` ### Try Request The `try_request` function makes HTTP
-requests to a URL and returns the response if successful. ```python from
-abstract_webtools import try_request response = try_request('https://
-www.example.com') print(response) # Output:
+Content-Type: text/markdown ``` # abstract_webtools for parsing web content. ##
+Installation You can install the package via pip: ```bash pip install
+abstract_webtools ``` ## Usage ### Get Status Code The `get_status` function
+fetches the status code of the URL. ```python from abstract_webtn_url urls =
+clean_url('https://example.com') print(urls) # Output: ['https://example.com',
+'http://example.com'] tps://example.com' ``` ### Try Request The `try_request`
+function makes HTTP requests to a URL and returns the response if successful.
+```python from abstract_webtools import try_request response = try_request
+('https://www.example.com') print(response) # Output:
 200]> ``` ### Is Valid URL The `is_valid` function checks whether a given URL
 is valid. ```python from abstract_webtools import is_valid valid = is_valid
 ('https://www.example.com') print(valid) # Output: True ``` ### Get Source Code
 The `get_Source_code` function fetches the source code of a URL with a custom
 user-agent. ```python from abstract_webtools import get_Source_code source_code
 = get_Source_code('https://www.example.com') print(source_code) # Output: HTML
 source code of the URL ``` ### Parse React Source The `parse_react_source`
```

