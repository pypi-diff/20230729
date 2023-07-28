# Comparing `tmp/mcptbr-0.2.2.tar.gz` & `tmp/mcptbr-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcptbr-0.2.2.tar", last modified: Fri Jul 28 23:29:51 2023, max compression
+gzip compressed data, was "mcptbr-0.2.3.tar", last modified: Fri Jul 28 23:48:07 2023, max compression
```

## Comparing `mcptbr-0.2.2.tar` & `mcptbr-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 23:29:51.027341 mcptbr-0.2.2/
--rw-rw-rw-   0        0        0      704 2023-07-28 23:29:51.026344 mcptbr-0.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 23:29:50.995429 mcptbr-0.2.2/mcptbr/
--rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.2.2/mcptbr/__init__.py
--rw-rw-rw-   0        0        0     2202 2023-07-27 20:17:14.000000 mcptbr-0.2.2/mcptbr/model.py
-drwxrwxrwx   0        0        0        0 2023-07-28 23:29:51.022355 mcptbr-0.2.2/mcptbr.egg-info/
--rw-rw-rw-   0        0        0      704 2023-07-28 23:29:50.000000 mcptbr-0.2.2/mcptbr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-28 23:29:50.000000 mcptbr-0.2.2/mcptbr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 23:29:50.000000 mcptbr-0.2.2/mcptbr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-28 23:29:50.000000 mcptbr-0.2.2/mcptbr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 23:29:50.000000 mcptbr-0.2.2/mcptbr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 23:29:51.027341 mcptbr-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      729 2023-07-28 23:27:59.000000 mcptbr-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 23:48:07.136142 mcptbr-0.2.3/
+-rw-rw-rw-   0        0        0      708 2023-07-28 23:48:07.135144 mcptbr-0.2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 23:48:07.117209 mcptbr-0.2.3/mcptbr/
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.2.3/mcptbr/__init__.py
+-rw-rw-rw-   0        0        0     2202 2023-07-27 20:17:14.000000 mcptbr-0.2.3/mcptbr/model.py
+drwxrwxrwx   0        0        0        0 2023-07-28 23:48:07.133150 mcptbr-0.2.3/mcptbr.egg-info/
+-rw-rw-rw-   0        0        0      708 2023-07-28 23:48:06.000000 mcptbr-0.2.3/mcptbr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-28 23:48:06.000000 mcptbr-0.2.3/mcptbr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 23:48:06.000000 mcptbr-0.2.3/mcptbr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-28 23:48:06.000000 mcptbr-0.2.3/mcptbr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 23:48:06.000000 mcptbr-0.2.3/mcptbr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 23:48:07.137138 mcptbr-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1193 2023-07-28 23:47:34.000000 mcptbr-0.2.3/setup.py
```

### Comparing `mcptbr-0.2.2/PKG-INFO` & `mcptbr-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: mcptbr
-Version: 0.2.2
+Version: 0.2.3
 Summary: Biblioteca para manipular o Minecraft através do python.
 Author: Lucas Pereira
 Author-email: lucasthe2@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
+
 # mcptbr
 
 
 mcptbr é uma pequena biblioteca que permite o usuário a manipular blocos do Minecraft com python.
 
 ## Para quem serve?
 Material criado para os alunos do curso de programação em python no Minecraft.
@@ -29,7 +30,8 @@
 ## Exemplo de uso
 ```
 from mcptbr.model import *
 
 
 print(pegarPosicaoJogador())
 ```
+
```

### Comparing `mcptbr-0.2.2/mcptbr/model.py` & `mcptbr-0.2.3/mcptbr/model.py`

 * *Files identical despite different names*

### Comparing `mcptbr-0.2.2/mcptbr.egg-info/PKG-INFO` & `mcptbr-0.2.3/mcptbr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: mcptbr
-Version: 0.2.2
+Version: 0.2.3
 Summary: Biblioteca para manipular o Minecraft através do python.
 Author: Lucas Pereira
 Author-email: lucasthe2@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
+
 # mcptbr
 
 
 mcptbr é uma pequena biblioteca que permite o usuário a manipular blocos do Minecraft com python.
 
 ## Para quem serve?
 Material criado para os alunos do curso de programação em python no Minecraft.
@@ -29,7 +30,8 @@
 ## Exemplo de uso
 ```
 from mcptbr.model import *
 
 
 print(pegarPosicaoJogador())
 ```
+
```

