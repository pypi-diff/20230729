# Comparing `tmp/mcptbr-0.1.9.tar.gz` & `tmp/mcptbr-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcptbr-0.1.9.tar", last modified: Thu Jul 27 20:53:52 2023, max compression
+gzip compressed data, was "mcptbr-0.2.0.tar", last modified: Fri Jul 28 22:56:59 2023, max compression
```

## Comparing `mcptbr-0.1.9.tar` & `mcptbr-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 20:53:52.155262 mcptbr-0.1.9/
--rw-rw-rw-   0        0        0      694 2023-07-27 20:53:52.155262 mcptbr-0.1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 20:53:52.139641 mcptbr-0.1.9/mcptbr/
--rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.1.9/mcptbr/__init__.py
--rw-rw-rw-   0        0        0     2202 2023-07-27 20:17:14.000000 mcptbr-0.1.9/mcptbr/model.py
-drwxrwxrwx   0        0        0        0 2023-07-27 20:53:52.155262 mcptbr-0.1.9/mcptbr.egg-info/
--rw-rw-rw-   0        0        0      694 2023-07-27 20:53:51.000000 mcptbr-0.1.9/mcptbr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-27 20:53:52.000000 mcptbr-0.1.9/mcptbr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 20:53:51.000000 mcptbr-0.1.9/mcptbr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-27 20:53:51.000000 mcptbr-0.1.9/mcptbr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-27 20:53:51.000000 mcptbr-0.1.9/mcptbr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 20:53:52.155262 mcptbr-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      626 2023-07-27 20:53:27.000000 mcptbr-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:56:59.751738 mcptbr-0.2.0/
+-rw-rw-rw-   0        0        0      234 2023-07-28 22:56:59.745768 mcptbr-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 22:56:59.725807 mcptbr-0.2.0/mcptbr/
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.2.0/mcptbr/__init__.py
+-rw-rw-rw-   0        0        0     2202 2023-07-27 20:17:14.000000 mcptbr-0.2.0/mcptbr/model.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:56:59.743772 mcptbr-0.2.0/mcptbr.egg-info/
+-rw-rw-rw-   0        0        0      234 2023-07-28 22:56:59.000000 mcptbr-0.2.0/mcptbr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-28 22:56:59.000000 mcptbr-0.2.0/mcptbr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 22:56:59.000000 mcptbr-0.2.0/mcptbr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-28 22:56:59.000000 mcptbr-0.2.0/mcptbr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 22:56:59.000000 mcptbr-0.2.0/mcptbr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 22:56:59.751738 mcptbr-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      602 2023-07-28 22:56:47.000000 mcptbr-0.2.0/setup.py
```

### Comparing `mcptbr-0.1.9/mcptbr/model.py` & `mcptbr-0.2.0/mcptbr/model.py`

 * *Files identical despite different names*

### Comparing `mcptbr-0.1.9/setup.py` & `mcptbr-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mcptbr',
-    version='0.1.9',
+    version='0.2.0',
     packages=find_packages(),
     install_requires=[
         "mcpi", # Dependências necessárias para sua biblioteca (se houver).
     ],
     author='Lucas Pereira',
     author_email='lucasthe2@gmail.com',
     description='Biblioteca para manipular o Minecraft através do python.',
-    long_description=open('README.md', encoding="utf-8").read(),
+    #long_description=open('README.md'),
     long_description_content_type='text/markdown',
     #url='https://github.com/seu_usuario/minha_biblioteca',
     license='MIT',  # Substitua pela licença adequada.
 )
```

