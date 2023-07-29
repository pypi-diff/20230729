# Comparing `tmp/streamlit_bls_connection-0.5.tar.gz` & `tmp/streamlit_bls_connection-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_bls_connection-0.5.tar", last modified: Sat Jul 29 16:44:38 2023, max compression
+gzip compressed data, was "streamlit_bls_connection-0.6.tar", last modified: Sat Jul 29 21:11:12 2023, max compression
```

## Comparing `streamlit_bls_connection-0.5.tar` & `streamlit_bls_connection-0.6.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 16:44:38.947064 streamlit_bls_connection-0.5/
--rw-rw-rw-   0        0        0     1089 2023-07-29 16:30:01.000000 streamlit_bls_connection-0.5/LICENSE
--rw-rw-rw-   0        0        0      763 2023-07-29 16:44:38.947064 streamlit_bls_connection-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1248 2023-07-29 03:47:40.000000 streamlit_bls_connection-0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-29 16:44:38.947064 streamlit_bls_connection-0.5/setup.cfg
--rw-rw-rw-   0        0        0     1094 2023-07-29 16:44:28.000000 streamlit_bls_connection-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 16:44:38.893945 streamlit_bls_connection-0.5/streamlit_bls_connection/
--rw-rw-rw-   0        0        0       65 2023-07-29 16:22:24.000000 streamlit_bls_connection-0.5/streamlit_bls_connection/__init__.py
--rw-rw-rw-   0        0        0     3645 2023-07-25 22:28:07.000000 streamlit_bls_connection-0.5/streamlit_bls_connection/bls_connection.py
-drwxrwxrwx   0        0        0        0 2023-07-29 16:44:38.945575 streamlit_bls_connection-0.5/streamlit_bls_connection.egg-info/
--rw-rw-rw-   0        0        0      763 2023-07-29 16:44:38.000000 streamlit_bls_connection-0.5/streamlit_bls_connection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-07-29 16:44:38.000000 streamlit_bls_connection-0.5/streamlit_bls_connection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 16:44:38.000000 streamlit_bls_connection-0.5/streamlit_bls_connection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-29 16:44:38.000000 streamlit_bls_connection-0.5/streamlit_bls_connection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-07-29 16:44:38.000000 streamlit_bls_connection-0.5/streamlit_bls_connection.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 21:11:12.990549 streamlit_bls_connection-0.6/
+-rw-rw-rw-   0        0        0     1089 2023-07-29 16:30:01.000000 streamlit_bls_connection-0.6/LICENSE
+-rw-rw-rw-   0        0        0     2263 2023-07-29 21:11:12.990549 streamlit_bls_connection-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1412 2023-07-29 21:07:32.000000 streamlit_bls_connection-0.6/README.md
+-rw-rw-rw-   0        0        0      389 2023-07-29 21:09:36.000000 streamlit_bls_connection-0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-29 21:11:12.991558 streamlit_bls_connection-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1188 2023-07-29 21:09:23.000000 streamlit_bls_connection-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:11:12.940014 streamlit_bls_connection-0.6/streamlit_bls_connection/
+-rw-rw-rw-   0        0        0       65 2023-07-29 16:22:24.000000 streamlit_bls_connection-0.6/streamlit_bls_connection/__init__.py
+-rw-rw-rw-   0        0        0     3645 2023-07-25 22:28:07.000000 streamlit_bls_connection-0.6/streamlit_bls_connection/bls_connection.py
+-rw-rw-rw-   0        0        0       33 2023-07-29 21:09:47.000000 streamlit_bls_connection-0.6/streamlit_bls_connection/version.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:11:12.989531 streamlit_bls_connection-0.6/streamlit_bls_connection.egg-info/
+-rw-rw-rw-   0        0        0     2263 2023-07-29 21:11:12.000000 streamlit_bls_connection-0.6/streamlit_bls_connection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-07-29 21:11:12.000000 streamlit_bls_connection-0.6/streamlit_bls_connection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 21:11:12.000000 streamlit_bls_connection-0.6/streamlit_bls_connection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-29 21:11:12.000000 streamlit_bls_connection-0.6/streamlit_bls_connection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-29 21:11:12.000000 streamlit_bls_connection-0.6/streamlit_bls_connection.egg-info/top_level.txt
```

### Comparing `streamlit_bls_connection-0.5/LICENSE` & `streamlit_bls_connection-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_bls_connection-0.5/README.md` & `streamlit_bls_connection-0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -30,9 +30,15 @@
 gas_df = dataframes_dict['APU000074714']
 electricity_df = dataframes_dict['APU000072610']
 
 # Step 5: Show Dataframes in Streamlit
 st.dataframe(gas_df, electricity_df)
 ```
 
+## Requirements
+- Python 3.8 and above
+
 ## License
-This project is licensed under the MIT License. See the LICENSE file for details.
+This project is licensed under the MIT License. See the LICENSE file for details.
+
+## Contact
+For questions, suggestions, or contributions, please visit my [GitHub Profile](https://github.com/tonyhollaar).
```

### Comparing `streamlit_bls_connection-0.5/setup.py` & `streamlit_bls_connection-0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='streamlit_bls_connection',
-    version='0.5',
+    version='0.6',
     license='MIT',  
     description='A package to fetch Bureau of Labor Statistics data using Streamlit',
+    long_description=long_description,  
+    long_description_content_type='text/markdown',
     author='Tony Hollaar',
     author_email='thollaar@gmail.com',
     url='https://github.com/tonyhollaar/',
     download_url='https://github.com/tonyhollaar/streamlit_bls_connection/archive/refs/tags/v4.tar.gz',
     packages=find_packages(),
     keywords=['streamlit', 'api', 'bls'],  # <-- Comma added here
     install_requires=[
```

### Comparing `streamlit_bls_connection-0.5/streamlit_bls_connection/bls_connection.py` & `streamlit_bls_connection-0.6/streamlit_bls_connection/bls_connection.py`

 * *Files identical despite different names*

