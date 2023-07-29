# Comparing `tmp/uszipstats-0.2.tar.gz` & `tmp/uszipstats-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uszipstats-0.2.tar", last modified: Tue Jul 25 18:35:20 2023, max compression
+gzip compressed data, was "uszipstats-0.3.tar", last modified: Sat Jul 29 14:26:06 2023, max compression
```

## Comparing `uszipstats-0.2.tar` & `uszipstats-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-25 18:35:20.022297 uszipstats-0.2/
--rw-r--r--   0 vedantrathi   (501) staff       (20)     1065 2023-07-25 18:05:29.000000 uszipstats-0.2/LICENSE.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)      731 2023-07-25 18:35:20.022526 uszipstats-0.2/PKG-INFO
--rw-r--r--   0 vedantrathi   (501) staff       (20)       25 2023-07-25 18:05:28.000000 uszipstats-0.2/README.md
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-25 18:35:20.018427 uszipstats-0.2/code_zip/
--rw-r--r--   0 vedantrathi   (501) staff       (20)       23 2023-07-25 18:05:32.000000 uszipstats-0.2/code_zip/__init__.py
--rw-r--r--   0 vedantrathi   (501) staff       (20)    40386 2023-07-25 18:32:05.000000 uszipstats-0.2/code_zip/irs_data.py
--rw-r--r--   0 vedantrathi   (501) staff       (20)       79 2023-07-25 18:35:20.023264 uszipstats-0.2/setup.cfg
--rw-r--r--   0 vedantrathi   (501) staff       (20)     1663 2023-07-25 18:33:28.000000 uszipstats-0.2/setup.py
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-25 18:35:20.022028 uszipstats-0.2/uszipstats.egg-info/
--rw-r--r--   0 vedantrathi   (501) staff       (20)      731 2023-07-25 18:35:19.000000 uszipstats-0.2/uszipstats.egg-info/PKG-INFO
--rw-r--r--   0 vedantrathi   (501) staff       (20)      251 2023-07-25 18:35:19.000000 uszipstats-0.2/uszipstats.egg-info/SOURCES.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)        1 2023-07-25 18:35:19.000000 uszipstats-0.2/uszipstats.egg-info/dependency_links.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)       33 2023-07-25 18:35:19.000000 uszipstats-0.2/uszipstats.egg-info/requires.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)        9 2023-07-25 18:35:19.000000 uszipstats-0.2/uszipstats.egg-info/top_level.txt
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-29 14:26:06.200330 uszipstats-0.3/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     1065 2023-07-25 18:05:29.000000 uszipstats-0.3/LICENSE.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     1082 2023-07-29 14:26:06.200491 uszipstats-0.3/PKG-INFO
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      268 2023-07-29 14:15:46.000000 uszipstats-0.3/README.md
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-29 14:26:06.178034 uszipstats-0.3/code_zip/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       23 2023-07-25 19:42:59.000000 uszipstats-0.3/code_zip/__init__.py
+-rw-r--r--   0 vedantrathi   (501) staff       (20)    40386 2023-07-25 18:32:05.000000 uszipstats-0.3/code_zip/irs_data.py
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       79 2023-07-29 14:26:06.201761 uszipstats-0.3/setup.cfg
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     1803 2023-07-29 14:25:39.000000 uszipstats-0.3/setup.py
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-29 14:26:06.196521 uszipstats-0.3/uszipstats.egg-info/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     1082 2023-07-29 14:26:05.000000 uszipstats-0.3/uszipstats.egg-info/PKG-INFO
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      251 2023-07-29 14:26:06.000000 uszipstats-0.3/uszipstats.egg-info/SOURCES.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)        1 2023-07-29 14:26:05.000000 uszipstats-0.3/uszipstats.egg-info/dependency_links.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       33 2023-07-29 14:26:05.000000 uszipstats-0.3/uszipstats.egg-info/requires.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)        9 2023-07-29 14:26:05.000000 uszipstats-0.3/uszipstats.egg-info/top_level.txt
```

### Comparing `uszipstats-0.2/LICENSE.txt` & `uszipstats-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uszipstats-0.2/code_zip/irs_data.py` & `uszipstats-0.3/code_zip/irs_data.py`

 * *Files identical despite different names*

### Comparing `uszipstats-0.2/setup.py` & `uszipstats-0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,26 @@
+def read_readme():
+    with open('README.md', 'r', encoding='utf-8') as f:
+        return f.read()
+
 import setuptools
 setuptools.setup(
     name='uszipstats',         # How you named your package
     packages=['code_zip'],   # Chose the same as "name"
-    version='0.2',      # Start with a small number and increase it with every change you make
-    # Chose a license from here: https://help.github.com/articles/licensing-a-repository
+    version='0.3',      # Start with a small number and increase it with every change you make
     license='MIT',
-    description='sample package',   # Give a short description about your library
+    description='This package will provide the ability to access IRS data',   # Give a short description about your library
+    long_description=read_readme(),
+    long_description_content_type='text/markdown',
     author='VEDANT RATHI',                   # Type in your name
     author_email='vedrathi10@gmail.com',      # Type in your E-Mail
     # Provide either the link to your github or to your website
     url='https://github.com/vrathi101/uszipstats.git',
     # I explain this later on
-    download_url='https://github.com/vrathi101/uszipstats/archive/refs/tags/v_02.tar.gz',
+    download_url='https://github.com/vrathi101/uszipstats/archive/refs/tags/v_03.tar.gz',
     keywords=['DATA', 'FUNCTIONS'],   # Keywords that define your package best
     install_requires=[
         'pandas',
         'numpy',
         'requests',
         'matplotlib',
     ],
```

