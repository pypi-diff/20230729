# Comparing `tmp/mcptbr-0.2.0.tar.gz` & `tmp/mcptbr-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcptbr-0.2.0.tar", last modified: Fri Jul 28 22:56:59 2023, max compression
+gzip compressed data, was "mcptbr-0.2.1.tar", last modified: Fri Jul 28 23:09:08 2023, max compression
```

## Comparing `mcptbr-0.2.0.tar` & `mcptbr-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 22:56:59.751738 mcptbr-0.2.0/
--rw-rw-rw-   0        0        0      234 2023-07-28 22:56:59.745768 mcptbr-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 22:56:59.725807 mcptbr-0.2.0/mcptbr/
--rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.2.0/mcptbr/__init__.py
--rw-rw-rw-   0        0        0     2202 2023-07-27 20:17:14.000000 mcptbr-0.2.0/mcptbr/model.py
-drwxrwxrwx   0        0        0        0 2023-07-28 22:56:59.743772 mcptbr-0.2.0/mcptbr.egg-info/
--rw-rw-rw-   0        0        0      234 2023-07-28 22:56:59.000000 mcptbr-0.2.0/mcptbr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-28 22:56:59.000000 mcptbr-0.2.0/mcptbr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 22:56:59.000000 mcptbr-0.2.0/mcptbr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-28 22:56:59.000000 mcptbr-0.2.0/mcptbr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 22:56:59.000000 mcptbr-0.2.0/mcptbr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 22:56:59.751738 mcptbr-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      602 2023-07-28 22:56:47.000000 mcptbr-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 23:09:08.177033 mcptbr-0.2.1/
+-rw-rw-rw-   0        0        0      704 2023-07-28 23:09:08.176028 mcptbr-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 23:09:08.151558 mcptbr-0.2.1/mcptbr/
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.2.1/mcptbr/__init__.py
+-rw-rw-rw-   0        0        0     2202 2023-07-27 20:17:14.000000 mcptbr-0.2.1/mcptbr/model.py
+drwxrwxrwx   0        0        0        0 2023-07-28 23:09:08.171094 mcptbr-0.2.1/mcptbr.egg-info/
+-rw-rw-rw-   0        0        0      704 2023-07-28 23:09:07.000000 mcptbr-0.2.1/mcptbr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-28 23:09:08.000000 mcptbr-0.2.1/mcptbr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 23:09:07.000000 mcptbr-0.2.1/mcptbr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-28 23:09:07.000000 mcptbr-0.2.1/mcptbr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 23:09:07.000000 mcptbr-0.2.1/mcptbr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 23:09:08.178022 mcptbr-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      655 2023-07-28 23:09:04.000000 mcptbr-0.2.1/setup.py
```

### Comparing `mcptbr-0.2.0/mcptbr/model.py` & `mcptbr-0.2.1/mcptbr/model.py`

 * *Files identical despite different names*

### Comparing `mcptbr-0.2.0/setup.py` & `mcptbr-0.2.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from setuptools import setup, find_packages
+from pathlib import Path
 
 setup(
     name='mcptbr',
-    version='0.2.0',
+    version='0.2.1',
     packages=find_packages(),
     install_requires=[
         "mcpi", # Dependências necessárias para sua biblioteca (se houver).
     ],
     author='Lucas Pereira',
     author_email='lucasthe2@gmail.com',
     description='Biblioteca para manipular o Minecraft através do python.',
-    #long_description=open('README.md'),
+    long_description=Path("README.md").read_text(encoding="utf-8"),
     long_description_content_type='text/markdown',
     #url='https://github.com/seu_usuario/minha_biblioteca',
     license='MIT',  # Substitua pela licença adequada.
 )
```

