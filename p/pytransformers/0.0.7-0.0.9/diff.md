# Comparing `tmp/pytransformers-0.0.7.tar.gz` & `tmp/pytransformers-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytransformers-0.0.7.tar", last modified: Sat Jul 29 19:14:49 2023, max compression
+gzip compressed data, was "pytransformers-0.0.9.tar", last modified: Sat Jul 29 19:31:06 2023, max compression
```

## Comparing `pytransformers-0.0.7.tar` & `pytransformers-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 omermajdi   (501) staff       (20)        0 2023-07-29 19:14:49.185224 pytransformers-0.0.7/
--rw-r--r--   0 omermajdi   (501) staff       (20)     1077 2023-07-29 19:14:43.000000 pytransformers-0.0.7/LICENSE
--rw-r--r--   0 omermajdi   (501) staff       (20)     7314 2023-07-29 19:14:49.185073 pytransformers-0.0.7/PKG-INFO
--rw-r--r--   0 omermajdi   (501) staff       (20)     6533 2023-07-29 18:57:07.000000 pytransformers-0.0.7/README.md
-drwxr-xr-x   0 omermajdi   (501) staff       (20)        0 2023-07-29 19:14:49.184154 pytransformers-0.0.7/pytransformers/
--rw-r--r--   0 omermajdi   (501) staff       (20)      278 2023-07-29 18:51:32.000000 pytransformers-0.0.7/pytransformers/__init__.py
--rw-r--r--   0 omermajdi   (501) staff       (20)    11773 2023-07-29 17:28:07.000000 pytransformers-0.0.7/pytransformers/transformer.py
-drwxr-xr-x   0 omermajdi   (501) staff       (20)        0 2023-07-29 19:14:49.184864 pytransformers-0.0.7/pytransformers.egg-info/
--rw-r--r--   0 omermajdi   (501) staff       (20)     7314 2023-07-29 19:14:49.000000 pytransformers-0.0.7/pytransformers.egg-info/PKG-INFO
--rw-r--r--   0 omermajdi   (501) staff       (20)      272 2023-07-29 19:14:49.000000 pytransformers-0.0.7/pytransformers.egg-info/SOURCES.txt
--rw-r--r--   0 omermajdi   (501) staff       (20)        1 2023-07-29 19:14:49.000000 pytransformers-0.0.7/pytransformers.egg-info/dependency_links.txt
--rw-r--r--   0 omermajdi   (501) staff       (20)       23 2023-07-29 19:14:49.000000 pytransformers-0.0.7/pytransformers.egg-info/requires.txt
--rw-r--r--   0 omermajdi   (501) staff       (20)       15 2023-07-29 19:14:49.000000 pytransformers-0.0.7/pytransformers.egg-info/top_level.txt
--rw-r--r--   0 omermajdi   (501) staff       (20)       38 2023-07-29 19:14:49.185278 pytransformers-0.0.7/setup.cfg
--rw-r--r--   0 omermajdi   (501) staff       (20)     1108 2023-07-29 19:11:34.000000 pytransformers-0.0.7/setup.py
+drwxr-xr-x   0 omermajdi   (501) staff       (20)        0 2023-07-29 19:31:06.277924 pytransformers-0.0.9/
+-rw-r--r--   0 omermajdi   (501) staff       (20)     1077 2023-07-29 19:14:43.000000 pytransformers-0.0.9/LICENSE
+-rw-r--r--   0 omermajdi   (501) staff       (20)     7322 2023-07-29 19:31:06.277777 pytransformers-0.0.9/PKG-INFO
+-rw-r--r--   0 omermajdi   (501) staff       (20)     6533 2023-07-29 18:57:07.000000 pytransformers-0.0.9/README.md
+drwxr-xr-x   0 omermajdi   (501) staff       (20)        0 2023-07-29 19:31:06.276794 pytransformers-0.0.9/pytransformers/
+-rw-r--r--   0 omermajdi   (501) staff       (20)      278 2023-07-29 18:51:32.000000 pytransformers-0.0.9/pytransformers/__init__.py
+-rw-r--r--   0 omermajdi   (501) staff       (20)    11773 2023-07-29 17:28:07.000000 pytransformers-0.0.9/pytransformers/transformer.py
+drwxr-xr-x   0 omermajdi   (501) staff       (20)        0 2023-07-29 19:31:06.277530 pytransformers-0.0.9/pytransformers.egg-info/
+-rw-r--r--   0 omermajdi   (501) staff       (20)     7322 2023-07-29 19:31:06.000000 pytransformers-0.0.9/pytransformers.egg-info/PKG-INFO
+-rw-r--r--   0 omermajdi   (501) staff       (20)      272 2023-07-29 19:31:06.000000 pytransformers-0.0.9/pytransformers.egg-info/SOURCES.txt
+-rw-r--r--   0 omermajdi   (501) staff       (20)        1 2023-07-29 19:31:06.000000 pytransformers-0.0.9/pytransformers.egg-info/dependency_links.txt
+-rw-r--r--   0 omermajdi   (501) staff       (20)       23 2023-07-29 19:31:06.000000 pytransformers-0.0.9/pytransformers.egg-info/requires.txt
+-rw-r--r--   0 omermajdi   (501) staff       (20)       15 2023-07-29 19:31:06.000000 pytransformers-0.0.9/pytransformers.egg-info/top_level.txt
+-rw-r--r--   0 omermajdi   (501) staff       (20)       38 2023-07-29 19:31:06.277979 pytransformers-0.0.9/setup.cfg
+-rw-r--r--   0 omermajdi   (501) staff       (20)     1093 2023-07-29 19:30:40.000000 pytransformers-0.0.9/setup.py
```

### Comparing `pytransformers-0.0.7/LICENSE` & `pytransformers-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytransformers-0.0.7/PKG-INFO` & `pytransformers-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pytransformers
-Version: 0.0.7
-Summary: create transformer models (articture behind chat GPTand other large language models)
+Version: 0.0.9
+Summary: create transformer models (Architecture behind chat GPT and other large language models)
 Home-page: UNKNOWN
 Author: omer mustafa
 Author-email: <omermustafacontact@gmail.com>
-License: MIT
+License: UNKNOWN
 Keywords: python,ai,Chat GPT,transformer model,transformers,bert,seq2seq,sequence to sequence,classification,chat bot,deep learning,keras
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `pytransformers-0.0.7/README.md` & `pytransformers-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pytransformers-0.0.7/pytransformers/transformer.py` & `pytransformers-0.0.9/pytransformers/transformer.py`

 * *Files identical despite different names*

### Comparing `pytransformers-0.0.7/pytransformers.egg-info/PKG-INFO` & `pytransformers-0.0.9/pytransformers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pytransformers
-Version: 0.0.7
-Summary: create transformer models (articture behind chat GPTand other large language models)
+Version: 0.0.9
+Summary: create transformer models (Architecture behind chat GPT and other large language models)
 Home-page: UNKNOWN
 Author: omer mustafa
 Author-email: <omermustafacontact@gmail.com>
-License: MIT
+License: UNKNOWN
 Keywords: python,ai,Chat GPT,transformer model,transformers,bert,seq2seq,sequence to sequence,classification,chat bot,deep learning,keras
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `pytransformers-0.0.7/setup.py` & `pytransformers-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from setuptools import setup, find_packages
 
 with open('README.md','r') as f:
     long_description = f.read()
 
-VERSION = '0.0.7'
-DESCRIPTION = 'create transformer models (articture behind chat GPTand other large language models)'
+VERSION = '0.0.9'
+DESCRIPTION = 'create transformer models (Architecture behind chat GPT and other large language models)'
 
 
 # Setting up
 setup(
     name="pytransformers",
     version=VERSION,
     author="omer mustafa",
     author_email="<omermustafacontact@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
-    license='MIT',
     long_description=long_description,
     packages=find_packages(),
     install_requires=['numpy','keras','tensorflow'],
     keywords=['python', 'ai', 'Chat GPT', 'transformer model', 'transformers', 'bert','seq2seq','sequence to sequence','classification','chat bot','deep learning','keras'],
     classifiers=[
         "Development Status :: 5 - Production/Stable", 
         "Intended Audience :: Developers",
```

