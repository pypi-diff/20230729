# Comparing `tmp/botwinick_utils-0.0.2.tar.gz` & `tmp/botwinick_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\botwinick_utils-0.0.2.tar", last modified: Sat Oct 17 21:31:32 2020, max compression
+gzip compressed data, was "botwinick_utils-0.0.4.tar", last modified: Sat Jul 29 18:20:22 2023, max compression
```

## Comparing `botwinick_utils-0.0.2.tar` & `botwinick_utils-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2020-10-17 21:31:32.000000 botwinick_utils-0.0.2/
--rw-rw-rw-   0        0        0      823 2020-10-17 21:31:32.000000 botwinick_utils-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      167 2020-10-15 18:46:33.000000 botwinick_utils-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2020-10-17 21:31:31.000000 botwinick_utils-0.0.2/botwinick_utils/
--rw-rw-rw-   0        0        0      193 2020-10-15 18:50:25.000000 botwinick_utils-0.0.2/botwinick_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2020-10-17 21:31:31.000000 botwinick_utils-0.0.2/botwinick_utils/binary/
--rw-rw-rw-   0        0        0      269 2020-10-17 21:29:14.000000 botwinick_utils-0.0.2/botwinick_utils/binary/__init__.py
--rw-rw-rw-   0        0        0     2167 2020-10-17 21:30:02.000000 botwinick_utils-0.0.2/botwinick_utils/binary/b32.py
--rw-rw-rw-   0        0        0      108 2020-10-15 18:53:01.000000 botwinick_utils-0.0.2/botwinick_utils/compat.py
--rw-rw-rw-   0        0        0     2786 2020-08-28 20:10:42.000000 botwinick_utils-0.0.2/botwinick_utils/io.py
--rw-rw-rw-   0        0        0     1874 2020-08-28 20:22:50.000000 botwinick_utils-0.0.2/botwinick_utils/net.py
--rw-rw-rw-   0        0        0     5752 2020-08-28 20:39:08.000000 botwinick_utils-0.0.2/botwinick_utils/paths.py
-drwxrwxrwx   0        0        0        0 2020-10-17 21:31:32.000000 botwinick_utils-0.0.2/botwinick_utils/platforms/
--rw-rw-rw-   0        0        0     3680 2020-08-28 20:10:42.000000 botwinick_utils-0.0.2/botwinick_utils/platforms/__init__.py
--rw-rw-rw-   0        0        0     5491 2020-08-28 20:10:42.000000 botwinick_utils-0.0.2/botwinick_utils/platforms/linux.py
--rw-rw-rw-   0        0        0     7059 2020-09-29 22:46:34.000000 botwinick_utils-0.0.2/botwinick_utils/platforms/threading.py
--rw-rw-rw-   0        0        0     1552 2020-08-28 20:10:42.000000 botwinick_utils-0.0.2/botwinick_utils/pretty.py
--rw-rw-rw-   0        0        0     3952 2020-08-28 20:10:42.000000 botwinick_utils-0.0.2/botwinick_utils/regex.py
--rw-rw-rw-   0        0        0     2223 2020-10-16 01:26:56.000000 botwinick_utils-0.0.2/botwinick_utils/util.py
-drwxrwxrwx   0        0        0        0 2020-10-17 21:31:31.000000 botwinick_utils-0.0.2/botwinick_utils.egg-info/
--rw-rw-rw-   0        0        0      823 2020-10-17 21:31:31.000000 botwinick_utils-0.0.2/botwinick_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      588 2020-10-17 21:31:31.000000 botwinick_utils-0.0.2/botwinick_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-10-17 21:31:31.000000 botwinick_utils-0.0.2/botwinick_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2020-10-17 21:31:31.000000 botwinick_utils-0.0.2/botwinick_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2020-10-17 21:31:31.000000 botwinick_utils-0.0.2/botwinick_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-10-17 21:31:32.000000 botwinick_utils-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      925 2020-10-17 21:27:19.000000 botwinick_utils-0.0.2/setup.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-29 18:20:22.251235 botwinick_utils-0.0.4/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1551 2020-10-15 18:46:33.000000 botwinick_utils-0.0.4/LICENSE
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      743 2023-07-29 18:20:22.239218 botwinick_utils-0.0.4/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      167 2020-10-15 18:46:33.000000 botwinick_utils-0.0.4/README.md
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-29 18:20:21.485934 botwinick_utils-0.0.4/botwinick_utils/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      193 2020-10-15 18:50:25.000000 botwinick_utils-0.0.4/botwinick_utils/__init__.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-29 18:20:21.948446 botwinick_utils-0.0.4/botwinick_utils/binary/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      269 2020-10-17 21:29:14.000000 botwinick_utils-0.0.4/botwinick_utils/binary/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2328 2020-10-21 23:51:54.000000 botwinick_utils-0.0.4/botwinick_utils/binary/b32.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      108 2020-10-15 18:53:01.000000 botwinick_utils-0.0.4/botwinick_utils/compat.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2786 2020-08-28 20:10:42.000000 botwinick_utils-0.0.4/botwinick_utils/io.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7380 2023-07-29 18:18:40.000000 botwinick_utils-0.0.4/botwinick_utils/net.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5752 2020-08-28 20:39:08.000000 botwinick_utils-0.0.4/botwinick_utils/paths.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-29 18:20:22.151711 botwinick_utils-0.0.4/botwinick_utils/platforms/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3680 2020-08-28 20:10:42.000000 botwinick_utils-0.0.4/botwinick_utils/platforms/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5491 2020-08-28 20:10:42.000000 botwinick_utils-0.0.4/botwinick_utils/platforms/linux.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7059 2020-09-29 22:46:34.000000 botwinick_utils-0.0.4/botwinick_utils/platforms/threading.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1552 2020-08-28 20:10:42.000000 botwinick_utils-0.0.4/botwinick_utils/pretty.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3952 2020-08-28 20:10:42.000000 botwinick_utils-0.0.4/botwinick_utils/regex.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2223 2020-10-16 01:26:56.000000 botwinick_utils-0.0.4/botwinick_utils/util.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-29 18:20:21.795199 botwinick_utils-0.0.4/botwinick_utils.egg-info/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      743 2023-07-29 18:20:19.000000 botwinick_utils-0.0.4/botwinick_utils.egg-info/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      596 2023-07-29 18:20:20.000000 botwinick_utils-0.0.4/botwinick_utils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-29 18:20:19.000000 botwinick_utils-0.0.4/botwinick_utils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        4 2023-07-29 18:20:19.000000 botwinick_utils-0.0.4/botwinick_utils.egg-info/requires.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       16 2023-07-29 18:20:19.000000 botwinick_utils-0.0.4/botwinick_utils.egg-info/top_level.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-29 18:20:22.255219 botwinick_utils-0.0.4/setup.cfg
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      870 2023-07-29 18:16:31.000000 botwinick_utils-0.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `botwinick_utils-0.0.2/PKG-INFO` & `botwinick_utils-0.0.4/botwinick_utils.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-Metadata-Version: 2.1
-Name: botwinick_utils
-Version: 0.0.2
-Summary: Assorted Utilities and platform code
-Home-page: https://github.com/dbotwinick/botwinick_utils
-Author: Drew Botwinick
-Author-email: foss@drewbotwinick.com
-License: UNKNOWN
-Description: # botwinick_utils
-        Common Python Utilities. This is essentially just a staging area for existing code that hasn't been sent to a more specific repository or package.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=2.7, >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: botwinick-utils
+Version: 0.0.4
+Summary: Assorted Utilities and platform code
+Home-page: https://github.com/dbotwinick/botwinick_utils
+Author: Drew Botwinick
+Author-email: foss@drewbotwinick.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# botwinick_utils
+Common Python Utilities. This is essentially just a staging area for existing code that hasn't been sent to a more specific repository or package.
+
+
```

### Comparing `botwinick_utils-0.0.2/botwinick_utils/binary/b32.py` & `botwinick_utils-0.0.4/botwinick_utils/binary/b32.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,14 +42,16 @@
         struct = _BINARY_INTEGER_PACK
     elif data_type in string_types:
         struct = _BINARY_STRING_PACK
     else:
         raise ValueError('unsupported struct item type')
     size, length = bytes_size(shape, struct, return_length=True)
     data = f.read(size)  # type: bytes
+    if len(data) != size:
+        raise ValueError('bytes length mismatch between expected shape and file handle; expected=%d, actual=%d' % (size, len(data)))
     fmt = ''.join([struct[0]] + [struct[1]] * length)
     return wrapper_type(unpack(fmt, data))
 
 
 def pack_sequence(f, sequence):
     if isinstance(sequence[0], float):
         struct = _BINARY_FLOAT_PACK
```

### Comparing `botwinick_utils-0.0.2/botwinick_utils/io.py` & `botwinick_utils-0.0.4/botwinick_utils/io.py`

 * *Files identical despite different names*

### Comparing `botwinick_utils-0.0.2/botwinick_utils/paths.py` & `botwinick_utils-0.0.4/botwinick_utils/paths.py`

 * *Files identical despite different names*

### Comparing `botwinick_utils-0.0.2/botwinick_utils/platforms/__init__.py` & `botwinick_utils-0.0.4/botwinick_utils/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `botwinick_utils-0.0.2/botwinick_utils/platforms/linux.py` & `botwinick_utils-0.0.4/botwinick_utils/platforms/linux.py`

 * *Files identical despite different names*

### Comparing `botwinick_utils-0.0.2/botwinick_utils/platforms/threading.py` & `botwinick_utils-0.0.4/botwinick_utils/platforms/threading.py`

 * *Files identical despite different names*

### Comparing `botwinick_utils-0.0.2/botwinick_utils/pretty.py` & `botwinick_utils-0.0.4/botwinick_utils/pretty.py`

 * *Files identical despite different names*

### Comparing `botwinick_utils-0.0.2/botwinick_utils/regex.py` & `botwinick_utils-0.0.4/botwinick_utils/regex.py`

 * *Files identical despite different names*

### Comparing `botwinick_utils-0.0.2/botwinick_utils/util.py` & `botwinick_utils-0.0.4/botwinick_utils/util.py`

 * *Files identical despite different names*

### Comparing `botwinick_utils-0.0.2/botwinick_utils.egg-info/PKG-INFO` & `botwinick_utils-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-Metadata-Version: 2.1
-Name: botwinick-utils
-Version: 0.0.2
-Summary: Assorted Utilities and platform code
-Home-page: https://github.com/dbotwinick/botwinick_utils
-Author: Drew Botwinick
-Author-email: foss@drewbotwinick.com
-License: UNKNOWN
-Description: # botwinick_utils
-        Common Python Utilities. This is essentially just a staging area for existing code that hasn't been sent to a more specific repository or package.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=2.7, >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: botwinick_utils
+Version: 0.0.4
+Summary: Assorted Utilities and platform code
+Home-page: https://github.com/dbotwinick/botwinick_utils
+Author: Drew Botwinick
+Author-email: foss@drewbotwinick.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# botwinick_utils
+Common Python Utilities. This is essentially just a staging area for existing code that hasn't been sent to a more specific repository or package.
+
+
```

### Comparing `botwinick_utils-0.0.2/botwinick_utils.egg-info/SOURCES.txt` & `botwinick_utils-0.0.4/botwinick_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 botwinick_utils/__init__.py
 botwinick_utils/compat.py
 botwinick_utils/io.py
 botwinick_utils/net.py
 botwinick_utils/paths.py
```

### Comparing `botwinick_utils-0.0.2/setup.py` & `botwinick_utils-0.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,26 +3,25 @@
 import setuptools
 
 with open("README.md", 'r') as f:
     readme_txt = f.read()
 
 setuptools.setup(
     name="botwinick_utils",
-    version="0.0.2",
+    version="0.0.4",
     author="Drew Botwinick",
     author_email="foss@drewbotwinick.com",
     description="Assorted Utilities and platform code",
     long_description=readme_txt,
     long_description_content_type="text/markdown",
     url="https://github.com/dbotwinick/botwinick_utils",
     packages=setuptools.find_packages(),
     install_requires=['six'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
-        'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: BSD License',
         "Operating System :: OS Independent",
     ],
-    python_requires='>=2.7, >=3.6',
+    python_requires='>=3.9',
 )
```

