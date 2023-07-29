# Comparing `tmp/mcptbr-0.2.3.tar.gz` & `tmp/mcptbr-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcptbr-0.2.3.tar", last modified: Fri Jul 28 23:48:07 2023, max compression
+gzip compressed data, was "mcptbr-0.2.4.tar", last modified: Sat Jul 29 00:32:51 2023, max compression
```

## Comparing `mcptbr-0.2.3.tar` & `mcptbr-0.2.4.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 23:48:07.136142 mcptbr-0.2.3/
--rw-rw-rw-   0        0        0      708 2023-07-28 23:48:07.135144 mcptbr-0.2.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 23:48:07.117209 mcptbr-0.2.3/mcptbr/
--rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.2.3/mcptbr/__init__.py
--rw-rw-rw-   0        0        0     2202 2023-07-27 20:17:14.000000 mcptbr-0.2.3/mcptbr/model.py
-drwxrwxrwx   0        0        0        0 2023-07-28 23:48:07.133150 mcptbr-0.2.3/mcptbr.egg-info/
--rw-rw-rw-   0        0        0      708 2023-07-28 23:48:06.000000 mcptbr-0.2.3/mcptbr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-28 23:48:06.000000 mcptbr-0.2.3/mcptbr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 23:48:06.000000 mcptbr-0.2.3/mcptbr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-28 23:48:06.000000 mcptbr-0.2.3/mcptbr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 23:48:06.000000 mcptbr-0.2.3/mcptbr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 23:48:07.137138 mcptbr-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1193 2023-07-28 23:47:34.000000 mcptbr-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 00:32:51.691728 mcptbr-0.2.4/
+-rw-rw-rw-   0        0        0      708 2023-07-29 00:32:51.688730 mcptbr-0.2.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 00:32:51.671775 mcptbr-0.2.4/mcptbr/
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.2.4/mcptbr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 00:32:51.686735 mcptbr-0.2.4/mcptbr.egg-info/
+-rw-rw-rw-   0        0        0      708 2023-07-29 00:32:51.000000 mcptbr-0.2.4/mcptbr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-07-29 00:32:51.000000 mcptbr-0.2.4/mcptbr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 00:32:51.000000 mcptbr-0.2.4/mcptbr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-29 00:32:51.000000 mcptbr-0.2.4/mcptbr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-29 00:32:51.000000 mcptbr-0.2.4/mcptbr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 00:32:51.691728 mcptbr-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1193 2023-07-29 00:32:07.000000 mcptbr-0.2.4/setup.py
```

### Comparing `mcptbr-0.2.3/PKG-INFO` & `mcptbr-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcptbr
-Version: 0.2.3
+Version: 0.2.4
 Summary: Biblioteca para manipular o Minecraft através do python.
 Author: Lucas Pereira
 Author-email: lucasthe2@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `mcptbr-0.2.3/mcptbr.egg-info/PKG-INFO` & `mcptbr-0.2.4/mcptbr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcptbr
-Version: 0.2.3
+Version: 0.2.4
 Summary: Biblioteca para manipular o Minecraft através do python.
 Author: Lucas Pereira
 Author-email: lucasthe2@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `mcptbr-0.2.3/setup.py` & `mcptbr-0.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 print(pegarPosicaoJogador())
 ```
 
 """
 
 setup(
     name='mcptbr',
-    version='0.2.3',
+    version='0.2.4',
     packages=find_packages(),
     install_requires=[
         "mcpi", # Dependências necessárias para sua biblioteca (se houver).
     ],
     author='Lucas Pereira',
     author_email='lucasthe2@gmail.com',
     description='Biblioteca para manipular o Minecraft através do python.',
```

