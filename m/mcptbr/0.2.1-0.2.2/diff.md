# Comparing `tmp/mcptbr-0.2.1.tar.gz` & `tmp/mcptbr-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcptbr-0.2.1.tar", last modified: Fri Jul 28 23:09:08 2023, max compression
+gzip compressed data, was "mcptbr-0.2.2.tar", last modified: Fri Jul 28 23:29:51 2023, max compression
```

## Comparing `mcptbr-0.2.1.tar` & `mcptbr-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 23:09:08.177033 mcptbr-0.2.1/
--rw-rw-rw-   0        0        0      704 2023-07-28 23:09:08.176028 mcptbr-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 23:09:08.151558 mcptbr-0.2.1/mcptbr/
--rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.2.1/mcptbr/__init__.py
--rw-rw-rw-   0        0        0     2202 2023-07-27 20:17:14.000000 mcptbr-0.2.1/mcptbr/model.py
-drwxrwxrwx   0        0        0        0 2023-07-28 23:09:08.171094 mcptbr-0.2.1/mcptbr.egg-info/
--rw-rw-rw-   0        0        0      704 2023-07-28 23:09:07.000000 mcptbr-0.2.1/mcptbr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-28 23:09:08.000000 mcptbr-0.2.1/mcptbr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 23:09:07.000000 mcptbr-0.2.1/mcptbr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-28 23:09:07.000000 mcptbr-0.2.1/mcptbr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 23:09:07.000000 mcptbr-0.2.1/mcptbr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 23:09:08.178022 mcptbr-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      655 2023-07-28 23:09:04.000000 mcptbr-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 23:29:51.027341 mcptbr-0.2.2/
+-rw-rw-rw-   0        0        0      704 2023-07-28 23:29:51.026344 mcptbr-0.2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 23:29:50.995429 mcptbr-0.2.2/mcptbr/
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.2.2/mcptbr/__init__.py
+-rw-rw-rw-   0        0        0     2202 2023-07-27 20:17:14.000000 mcptbr-0.2.2/mcptbr/model.py
+drwxrwxrwx   0        0        0        0 2023-07-28 23:29:51.022355 mcptbr-0.2.2/mcptbr.egg-info/
+-rw-rw-rw-   0        0        0      704 2023-07-28 23:29:50.000000 mcptbr-0.2.2/mcptbr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-28 23:29:50.000000 mcptbr-0.2.2/mcptbr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 23:29:50.000000 mcptbr-0.2.2/mcptbr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-28 23:29:50.000000 mcptbr-0.2.2/mcptbr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 23:29:50.000000 mcptbr-0.2.2/mcptbr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 23:29:51.027341 mcptbr-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      729 2023-07-28 23:27:59.000000 mcptbr-0.2.2/setup.py
```

### Comparing `mcptbr-0.2.1/PKG-INFO` & `mcptbr-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcptbr
-Version: 0.2.1
+Version: 0.2.2
 Summary: Biblioteca para manipular o Minecraft através do python.
 Author: Lucas Pereira
 Author-email: lucasthe2@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # mcptbr
```

### Comparing `mcptbr-0.2.1/mcptbr/model.py` & `mcptbr-0.2.2/mcptbr/model.py`

 * *Files identical despite different names*

### Comparing `mcptbr-0.2.1/mcptbr.egg-info/PKG-INFO` & `mcptbr-0.2.2/mcptbr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcptbr
-Version: 0.2.1
+Version: 0.2.2
 Summary: Biblioteca para manipular o Minecraft através do python.
 Author: Lucas Pereira
 Author-email: lucasthe2@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # mcptbr
```

### Comparing `mcptbr-0.2.1/setup.py` & `mcptbr-0.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
+
+
 setup(
     name='mcptbr',
-    version='0.2.1',
+    version='0.2.2',
     packages=find_packages(),
     install_requires=[
         "mcpi", # Dependências necessárias para sua biblioteca (se houver).
     ],
     author='Lucas Pereira',
     author_email='lucasthe2@gmail.com',
     description='Biblioteca para manipular o Minecraft através do python.',
     long_description=Path("README.md").read_text(encoding="utf-8"),
+    #long_description=Path("README.md").read_text(encoding="utf-8"),
     long_description_content_type='text/markdown',
     #url='https://github.com/seu_usuario/minha_biblioteca',
     license='MIT',  # Substitua pela licença adequada.
 )
```

