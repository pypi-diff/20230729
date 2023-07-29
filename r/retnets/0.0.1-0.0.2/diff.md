# Comparing `tmp/retnets-0.0.1.tar.gz` & `tmp/retnets-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retnets-0.0.1.tar", last modified: Fri Jul 28 21:36:39 2023, max compression
+gzip compressed data, was "retnets-0.0.2.tar", last modified: Sat Jul 29 19:05:08 2023, max compression
```

## Comparing `retnets-0.0.1.tar` & `retnets-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-28 21:36:39.763776 retnets-0.0.1/
--rw-r--r--   0 mac        (501) staff       (20)     3209 2023-07-28 21:36:39.763425 retnets-0.0.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     2364 2023-07-28 21:32:43.000000 retnets-0.0.1/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-28 21:36:39.760618 retnets-0.0.1/retnets/
--rw-r--r--   0 mac        (501) staff       (20)       36 2023-07-28 21:04:21.000000 retnets-0.0.1/retnets/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-28 21:36:39.762912 retnets-0.0.1/retnets.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     3209 2023-07-28 21:36:39.000000 retnets-0.0.1/retnets.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      192 2023-07-28 21:36:39.000000 retnets-0.0.1/retnets.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-28 21:36:39.000000 retnets-0.0.1/retnets.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       40 2023-07-28 21:36:39.000000 retnets-0.0.1/retnets.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        8 2023-07-28 21:36:39.000000 retnets-0.0.1/retnets.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-28 21:36:39.763891 retnets-0.0.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     1672 2023-07-28 21:35:23.000000 retnets-0.0.1/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 19:05:08.283182 retnets-0.0.2/
+-rw-r--r--   0 mac        (501) staff       (20)     3319 2023-07-29 19:05:08.282781 retnets-0.0.2/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     2353 2023-07-28 21:38:26.000000 retnets-0.0.2/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 19:05:08.278907 retnets-0.0.2/retnets/
+-rw-r--r--   0 mac        (501) staff       (20)       36 2023-07-29 19:01:19.000000 retnets-0.0.2/retnets/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 19:05:08.281993 retnets-0.0.2/retnets.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     3319 2023-07-29 19:05:08.000000 retnets-0.0.2/retnets.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      192 2023-07-29 19:05:08.000000 retnets-0.0.2/retnets.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-29 19:05:08.000000 retnets-0.0.2/retnets.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       40 2023-07-29 19:05:08.000000 retnets-0.0.2/retnets.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        8 2023-07-29 19:05:08.000000 retnets-0.0.2/retnets.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-29 19:05:08.283388 retnets-0.0.2/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     1822 2023-07-29 19:04:21.000000 retnets-0.0.2/setup.py
```

### Comparing `retnets-0.0.1/PKG-INFO` & `retnets-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: retnets
-Version: 0.0.1
+Version: 0.0.2
 Summary: RETNETS is a powerful package designed to facilitate the usage of the Retentive Network by AI engineers. Whether you are working with Torch or Tensorflow, RETNET provides seamless integration and empowers you to harness the potential of Retentive Network for your AI projects.
+Download-URL: https://github.com/useCallback/retnets.git
 Author: useCallback (Khalfoun Mohamed El Mehdi)
 Author-email: <contact.khalfoun@gmail.com>
+Project-URL: github, https://github.com/useCallback/retnets.git
 Keywords: retnet,retnets,retentive networks,LLM,large language models,ai,artificial intelligence
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
 # RETNETS (Retentive Networks) - PyPI Package
 
 ## Overview
 
-RETNETS is a powerful PyPI (pip) package designed to facilitate the usage of the Retentive Network by AI engineers. Whether you're working with Torch or Tensorflow, RETNET provides seamless integration and empowers you to harness the potential of Retentive Network for your AI projects.
+RETNETS is a powerful package designed to facilitate the usage of the Retentive Network by AI engineers. Whether you're working with Torch or Tensorflow, RETNET provides seamless integration and empowers you to harness the potential of Retentive Network for your AI projects.
 
 ## What is the Retentive Network?
 
 ## What is RETNET?
 
 RETNETS, or Retentive Network, is a revolutionary neural network architecture transforming large language models. It introduces the "retention mechanism," efficiently addressing inference and parallelism challenges faced by traditional Transformers.
```

### Comparing `retnets-0.0.1/README.md` & `retnets-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # RETNETS (Retentive Networks) - PyPI Package
 
 ## Overview
 
-RETNETS is a powerful PyPI (pip) package designed to facilitate the usage of the Retentive Network by AI engineers. Whether you're working with Torch or Tensorflow, RETNET provides seamless integration and empowers you to harness the potential of Retentive Network for your AI projects.
+RETNETS is a powerful package designed to facilitate the usage of the Retentive Network by AI engineers. Whether you're working with Torch or Tensorflow, RETNET provides seamless integration and empowers you to harness the potential of Retentive Network for your AI projects.
 
 ## What is the Retentive Network?
 
 ## What is RETNET?
 
 RETNETS, or Retentive Network, is a revolutionary neural network architecture transforming large language models. It introduces the "retention mechanism," efficiently addressing inference and parallelism challenges faced by traditional Transformers.
```

### Comparing `retnets-0.0.1/retnets.egg-info/PKG-INFO` & `retnets-0.0.2/retnets.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: retnets
-Version: 0.0.1
+Version: 0.0.2
 Summary: RETNETS is a powerful package designed to facilitate the usage of the Retentive Network by AI engineers. Whether you are working with Torch or Tensorflow, RETNET provides seamless integration and empowers you to harness the potential of Retentive Network for your AI projects.
+Download-URL: https://github.com/useCallback/retnets.git
 Author: useCallback (Khalfoun Mohamed El Mehdi)
 Author-email: <contact.khalfoun@gmail.com>
+Project-URL: github, https://github.com/useCallback/retnets.git
 Keywords: retnet,retnets,retentive networks,LLM,large language models,ai,artificial intelligence
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
 # RETNETS (Retentive Networks) - PyPI Package
 
 ## Overview
 
-RETNETS is a powerful PyPI (pip) package designed to facilitate the usage of the Retentive Network by AI engineers. Whether you're working with Torch or Tensorflow, RETNET provides seamless integration and empowers you to harness the potential of Retentive Network for your AI projects.
+RETNETS is a powerful package designed to facilitate the usage of the Retentive Network by AI engineers. Whether you're working with Torch or Tensorflow, RETNET provides seamless integration and empowers you to harness the potential of Retentive Network for your AI projects.
 
 ## What is the Retentive Network?
 
 ## What is RETNET?
 
 RETNETS, or Retentive Network, is a revolutionary neural network architecture transforming large language models. It introduces the "retention mechanism," efficiently addressing inference and parallelism challenges faced by traditional Transformers.
```

### Comparing `retnets-0.0.1/setup.py` & `retnets-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,28 +3,32 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'RETNETS is a powerful package designed to facilitate the usage of the Retentive Network by AI engineers. Whether you are working with Torch or Tensorflow, RETNET provides seamless integration and empowers you to harness the potential of Retentive Network for your AI projects.'
 LONG_DESCRIPTION = 'RETNETS is a powerful package designed to facilitate the usage of the Retentive Network by AI engineers. Whether you are working with Torch or Tensorflow, RETNET provides seamless integration and empowers you to harness the potential of Retentive Network for your AI projects.'
-
+project_urls = {
+    'github': 'https://github.com/useCallback/retnets.git',
+}
 # Setting up
 setup(
     name="retnets",
     version=VERSION,
     author="useCallback (Khalfoun Mohamed El Mehdi)",
     author_email="<contact.khalfoun@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
+    project_urls=project_urls,
+    download_url=project_urls['github'],
     install_requires=['torch', 'torchscale', 'fairseq', 'apex', 'fairscale'],
     keywords=['retnet', 'retnets', 'retentive networks',
               'LLM', 'large language models', 'ai', 'artificial intelligence'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

