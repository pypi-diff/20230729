# Comparing `tmp/revmap-0.0.6.tar.gz` & `tmp/revmap-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revmap-0.0.6.tar", max compression
+gzip compressed data, was "revmap-0.0.7.tar", max compression
```

## Comparing `revmap-0.0.6.tar` & `revmap-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1078 2023-07-29 15:53:34.786997 revmap-0.0.6/LICENSE
--rw-r--r--   0        0        0     2145 2023-07-29 15:53:34.786997 revmap-0.0.6/README.md
--rw-r--r--   0        0        0      508 2023-07-29 15:53:34.790998 revmap-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       68 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/__init__.py
--rw-r--r--   0        0        0      554 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/encoded.py
--rw-r--r--   0        0        0       23 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/events/__init__.py
--rw-r--r--   0        0        0      311 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/events/keyboard.py
--rw-r--r--   0        0        0     4010 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/payloads.py
--rw-r--r--   0        0        0      999 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/revmap.py
--rw-r--r--   0        0        0       86 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/settings/__init__.py
--rw-r--r--   0        0        0      729 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/settings/color_settings.py
--rw-r--r--   0        0        0      706 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/settings/message_settings.py
--rw-r--r--   0        0        0      219 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/settings/variables.py
--rw-r--r--   0        0        0       57 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/utils/__init__.py
--rw-r--r--   0        0        0     2177 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/utils/commands.py
--rw-r--r--   0        0        0     3378 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/utils/generator_payloads.py
--rw-r--r--   0        0        0     1003 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/utils/validator_required.py
--rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 revmap-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-29 15:59:22.113285 revmap-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2195 2023-07-29 15:59:22.113285 revmap-0.0.7/README.md
+-rw-r--r--   0        0        0      508 2023-07-29 15:59:22.113285 revmap-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-07-29 15:59:22.113285 revmap-0.0.7/revmap/__init__.py
+-rw-r--r--   0        0        0      554 2023-07-29 15:59:22.113285 revmap-0.0.7/revmap/encoded.py
+-rw-r--r--   0        0        0       23 2023-07-29 15:59:22.113285 revmap-0.0.7/revmap/events/__init__.py
+-rw-r--r--   0        0        0      311 2023-07-29 15:59:22.113285 revmap-0.0.7/revmap/events/keyboard.py
+-rw-r--r--   0        0        0     4010 2023-07-29 15:59:22.113285 revmap-0.0.7/revmap/payloads.py
+-rw-r--r--   0        0        0      999 2023-07-29 15:59:22.113285 revmap-0.0.7/revmap/revmap.py
+-rw-r--r--   0        0        0       86 2023-07-29 15:59:22.117285 revmap-0.0.7/revmap/settings/__init__.py
+-rw-r--r--   0        0        0      729 2023-07-29 15:59:22.117285 revmap-0.0.7/revmap/settings/color_settings.py
+-rw-r--r--   0        0        0      706 2023-07-29 15:59:22.117285 revmap-0.0.7/revmap/settings/message_settings.py
+-rw-r--r--   0        0        0      219 2023-07-29 15:59:22.117285 revmap-0.0.7/revmap/settings/variables.py
+-rw-r--r--   0        0        0       57 2023-07-29 15:59:22.117285 revmap-0.0.7/revmap/utils/__init__.py
+-rw-r--r--   0        0        0     2177 2023-07-29 15:59:22.117285 revmap-0.0.7/revmap/utils/commands.py
+-rw-r--r--   0        0        0     3378 2023-07-29 15:59:22.117285 revmap-0.0.7/revmap/utils/generator_payloads.py
+-rw-r--r--   0        0        0     1003 2023-07-29 15:59:22.117285 revmap-0.0.7/revmap/utils/validator_required.py
+-rw-r--r--   0        0        0     2717 1970-01-01 00:00:00.000000 revmap-0.0.7/PKG-INFO
```

### Comparing `revmap-0.0.6/LICENSE` & `revmap-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `revmap-0.0.6/README.md` & `revmap-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ```
 Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
 ```yaml
  ___ ___ _ _ _____ ___ ___ 
 |  _| -_| | |     | .'| . |
 |_| |___|\_/|_|_|_|__,|  _|
                       |_|  
-        v0.0.6 - @joaoviictorti 
+        v0.0.7 - @joaoviictorti 
 
 options:
   -h, --help    show this help message and exit
   --version     show program's version number and exit
   --ip IP       Insert ip
   --port PORTA  Insert port
 ```
@@ -52,10 +52,10 @@
 
 ```sh
 pip3 install revmap
 ```
 
 # Executando revmap
 
-![logo_do_projeto](images/revmap_console.png)
+![logo_do_projeto](https://github.com/joaoviictorti/revmap/blob/main/images/revmap_console.png)
 
 <img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
```

#### html2text {}

```diff
@@ -14,14 +14,14 @@
 encodes, mantive um modelo consistentemente passivo para tornÃ¡-lo Ãºtil para
 testadores de penetraÃ§Ã£o. # CaracterÃ­sticas - Gera payloads de reverse shell
 para diversas linguagens de programaÃ§Ã£o (python, bash, powershell e etc) -
 Funcionalidade de realizar encode das payloads desejadas (Url encode, base64,
 hexadecimal e etc) # Forma de utilizaÃ§Ã£o ```sh revmap --ip 192.168.4.80 --
 port 4444 ``` Isso exibirÃ¡ a ajuda para a ferramenta. Aqui estÃ£o todos os
 switches que ele suporta: ```yaml ___ ___ _ _ _____ ___ ___ | _| -_| | | | .'|
-. | |_| |___|\_/|_|_|_|__,| _| |_| v0.0.6 - @joaoviictorti options: -h, --help
+. | |_| |___|\_/|_|_|_|__,| _| |_| v0.0.7 - @joaoviictorti options: -h, --help
 show this help message and exit --version show program's version number and
 exit --ip IP Insert ip --port PORTA Insert port ``` # InstalaÃ§Ã£o revmap
 requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install revmap ``` #
-Executando revmap ![logo_do_projeto](images/revmap_console.png) [https://
-capsule-render.vercel.app/
+Executando revmap ![logo_do_projeto](https://github.com/joaoviictorti/revmap/
+blob/main/images/revmap_console.png) [https://capsule-render.vercel.app/
 api?type=waving&color=0000FF&height=120&section=footer]
```

### Comparing `revmap-0.0.6/revmap/encoded.py` & `revmap-0.0.7/revmap/encoded.py`

 * *Files identical despite different names*

### Comparing `revmap-0.0.6/revmap/payloads.py` & `revmap-0.0.7/revmap/payloads.py`

 * *Files identical despite different names*

### Comparing `revmap-0.0.6/revmap/revmap.py` & `revmap-0.0.7/revmap/revmap.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 def argumentos() -> None:
     global args
     parser = argparse.ArgumentParser(
         prog=banner(),
         usage='revmap --ip 192.168.4.80 --port 4444',
         formatter_class=RawTextHelpFormatter,
     )
-    parser.add_argument('--version', action='version', version='revmap 0.0.6')
+    parser.add_argument('--version', action='version', version='revmap 0.0.7')
     parser.add_argument(
         '--ip',
         type=str,
         dest='ip',
         action='store',
         help='Insert ip',
         required=True,
```

### Comparing `revmap-0.0.6/revmap/settings/color_settings.py` & `revmap-0.0.7/revmap/settings/color_settings.py`

 * *Files identical despite different names*

### Comparing `revmap-0.0.6/revmap/settings/message_settings.py` & `revmap-0.0.7/revmap/settings/message_settings.py`

 * *Files identical despite different names*

### Comparing `revmap-0.0.6/revmap/utils/commands.py` & `revmap-0.0.7/revmap/utils/commands.py`

 * *Files identical despite different names*

### Comparing `revmap-0.0.6/revmap/utils/generator_payloads.py` & `revmap-0.0.7/revmap/utils/generator_payloads.py`

 * *Files identical despite different names*

### Comparing `revmap-0.0.6/revmap/utils/validator_required.py` & `revmap-0.0.7/revmap/utils/validator_required.py`

 * *Files identical despite different names*

### Comparing `revmap-0.0.6/PKG-INFO` & `revmap-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revmap
-Version: 0.0.6
+Version: 0.0.7
 Summary: Ferramenta que gera shell reverso em várias linguagens de programação e codifica
 Home-page: https://github.com/joaoviictorti/revmap
 License: MIT
 Author: João
 Author-email: joaovictorti08@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -48,15 +48,15 @@
 ```
 Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
 ```yaml
  ___ ___ _ _ _____ ___ ___ 
 |  _| -_| | |     | .'| . |
 |_| |___|\_/|_|_|_|__,|  _|
                       |_|  
-        v0.0.6 - @joaoviictorti 
+        v0.0.7 - @joaoviictorti 
 
 options:
   -h, --help    show this help message and exit
   --version     show program's version number and exit
   --ip IP       Insert ip
   --port PORTA  Insert port
 ```
@@ -67,11 +67,11 @@
 
 ```sh
 pip3 install revmap
 ```
 
 # Executando revmap
 
-![logo_do_projeto](images/revmap_console.png)
+![logo_do_projeto](https://github.com/joaoviictorti/revmap/blob/main/images/revmap_console.png)
 
 <img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: revmap Version: 0.0.6 Summary: Ferramenta que gera
+Metadata-Version: 2.1 Name: revmap Version: 0.0.7 Summary: Ferramenta que gera
 shell reverso em vÃ¡rias linguagens de programaÃ§Ã£o e codifica Home-page:
 https://github.com/joaoviictorti/revmap License: MIT Author: JoÃ£o Author-
 email: joaovictorti08@gmail.com Requires-Python: >=3.11,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
 prompt-toolkit (==3.0.36) Description-Content-Type: text/markdown [https://
 capsule-render.vercel.app/
@@ -21,14 +21,14 @@
 encodes, mantive um modelo consistentemente passivo para tornÃ¡-lo Ãºtil para
 testadores de penetraÃ§Ã£o. # CaracterÃ­sticas - Gera payloads de reverse shell
 para diversas linguagens de programaÃ§Ã£o (python, bash, powershell e etc) -
 Funcionalidade de realizar encode das payloads desejadas (Url encode, base64,
 hexadecimal e etc) # Forma de utilizaÃ§Ã£o ```sh revmap --ip 192.168.4.80 --
 port 4444 ``` Isso exibirÃ¡ a ajuda para a ferramenta. Aqui estÃ£o todos os
 switches que ele suporta: ```yaml ___ ___ _ _ _____ ___ ___ | _| -_| | | | .'|
-. | |_| |___|\_/|_|_|_|__,| _| |_| v0.0.6 - @joaoviictorti options: -h, --help
+. | |_| |___|\_/|_|_|_|__,| _| |_| v0.0.7 - @joaoviictorti options: -h, --help
 show this help message and exit --version show program's version number and
 exit --ip IP Insert ip --port PORTA Insert port ``` # InstalaÃ§Ã£o revmap
 requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install revmap ``` #
-Executando revmap ![logo_do_projeto](images/revmap_console.png) [https://
-capsule-render.vercel.app/
+Executando revmap ![logo_do_projeto](https://github.com/joaoviictorti/revmap/
+blob/main/images/revmap_console.png) [https://capsule-render.vercel.app/
 api?type=waving&color=0000FF&height=120&section=footer]
```

