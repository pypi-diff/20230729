# Comparing `tmp/mcptbr-0.2.5.tar.gz` & `tmp/mcptbr-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcptbr-0.2.5.tar", last modified: Sat Jul 29 00:40:02 2023, max compression
+gzip compressed data, was "mcptbr-0.2.6.tar", last modified: Sat Jul 29 00:49:00 2023, max compression
```

## Comparing `mcptbr-0.2.5.tar` & `mcptbr-0.2.6.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 00:40:02.236606 mcptbr-0.2.5/
--rw-rw-rw-   0        0        0      708 2023-07-29 00:40:02.233615 mcptbr-0.2.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 00:40:02.230621 mcptbr-0.2.5/mcptbr.egg-info/
--rw-rw-rw-   0        0        0      708 2023-07-29 00:40:01.000000 mcptbr-0.2.5/mcptbr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-07-29 00:40:02.000000 mcptbr-0.2.5/mcptbr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 00:40:01.000000 mcptbr-0.2.5/mcptbr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-29 00:40:01.000000 mcptbr-0.2.5/mcptbr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 00:40:01.000000 mcptbr-0.2.5/mcptbr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 00:40:02.237603 mcptbr-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1193 2023-07-29 00:39:32.000000 mcptbr-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 00:49:00.131554 mcptbr-0.2.6/
+-rw-rw-rw-   0        0        0      708 2023-07-29 00:49:00.129558 mcptbr-0.2.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 00:49:00.107618 mcptbr-0.2.6/mcptbr/
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.2.6/mcptbr/__init__.py
+-rw-rw-rw-   0        0        0     2206 2023-07-29 00:30:24.000000 mcptbr-0.2.6/mcptbr/minecraft.py
+drwxrwxrwx   0        0        0        0 2023-07-29 00:49:00.127564 mcptbr-0.2.6/mcptbr.egg-info/
+-rw-rw-rw-   0        0        0      708 2023-07-29 00:48:59.000000 mcptbr-0.2.6/mcptbr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-07-29 00:48:59.000000 mcptbr-0.2.6/mcptbr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 00:48:59.000000 mcptbr-0.2.6/mcptbr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-29 00:48:59.000000 mcptbr-0.2.6/mcptbr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-29 00:48:59.000000 mcptbr-0.2.6/mcptbr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 00:49:00.131554 mcptbr-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1193 2023-07-29 00:48:25.000000 mcptbr-0.2.6/setup.py
```

### Comparing `mcptbr-0.2.5/PKG-INFO` & `mcptbr-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcptbr
-Version: 0.2.5
+Version: 0.2.6
 Summary: Biblioteca para manipular o Minecraft através do python.
 Author: Lucas Pereira
 Author-email: lucasthe2@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `mcptbr-0.2.5/mcptbr.egg-info/PKG-INFO` & `mcptbr-0.2.6/mcptbr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcptbr
-Version: 0.2.5
+Version: 0.2.6
 Summary: Biblioteca para manipular o Minecraft através do python.
 Author: Lucas Pereira
 Author-email: lucasthe2@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `mcptbr-0.2.5/setup.py` & `mcptbr-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 print(pegarPosicaoJogador())
 ```
 
 """
 
 setup(
     name='mcptbr',
-    version='0.2.5',
+    version='0.2.6',
     packages=find_packages(),
     install_requires=[
         "mcpi", # Dependências necessárias para sua biblioteca (se houver).
     ],
     author='Lucas Pereira',
     author_email='lucasthe2@gmail.com',
     description='Biblioteca para manipular o Minecraft através do python.',
```

