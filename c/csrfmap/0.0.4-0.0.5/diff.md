# Comparing `tmp/csrfmap-0.0.4.tar.gz` & `tmp/csrfmap-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csrfmap-0.0.4.tar", max compression
+gzip compressed data, was "csrfmap-0.0.5.tar", max compression
```

## Comparing `csrfmap-0.0.4.tar` & `csrfmap-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1078 2023-07-29 16:43:28.298677 csrfmap-0.0.4/LICENSE
--rw-r--r--   0        0        0     2755 2023-07-29 16:43:28.298677 csrfmap-0.0.4/README.md
--rw-r--r--   0        0        0       46 2023-07-29 16:43:28.298677 csrfmap-0.0.4/csrfmap/__init__.py
--rw-r--r--   0        0        0     3301 2023-07-29 16:43:28.298677 csrfmap-0.0.4/csrfmap/csrfmap.py
--rw-r--r--   0        0        0     4987 2023-07-29 16:43:28.298677 csrfmap-0.0.4/csrfmap/payloads.py
--rw-r--r--   0        0        0      449 2023-07-29 16:43:28.302677 csrfmap-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3200 1970-01-01 00:00:00.000000 csrfmap-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-29 16:44:27.022279 csrfmap-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2755 2023-07-29 16:44:27.022279 csrfmap-0.0.5/README.md
+-rw-r--r--   0        0        0       46 2023-07-29 16:44:27.026279 csrfmap-0.0.5/csrfmap/__init__.py
+-rw-r--r--   0        0        0     3301 2023-07-29 16:44:27.026279 csrfmap-0.0.5/csrfmap/csrfmap.py
+-rw-r--r--   0        0        0     4987 2023-07-29 16:44:27.026279 csrfmap-0.0.5/csrfmap/payloads.py
+-rw-r--r--   0        0        0      449 2023-07-29 16:44:27.026279 csrfmap-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3200 1970-01-01 00:00:00.000000 csrfmap-0.0.5/PKG-INFO
```

### Comparing `csrfmap-0.0.4/LICENSE` & `csrfmap-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `csrfmap-0.0.4/README.md` & `csrfmap-0.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
 ```yaml
  _____ _____ _____ _____ _____ _____ _____ 
 |     |   __| __  |   __|     |  _  |  _  |
 |   --|__   |    -|   __| | | |     |   __|
 |_____|_____|__|__|__|  |_|_|_|__|__|__|   
                                                        
-                        v0.0.3 - @joaoviictorti 
+                        v0.0.5 - @joaoviictorti 
 
 options:
   -h, --help            show this help message and exit
   -a ACTION, -A ACTION  Insert action
   -m METHOD, -M METHOD  Insert method
   -p {form1,form2,json1,json2}
   -n NAME [NAME ...], -name NAME [NAME ...] Insert name
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 para tornÃ¡-lo Ãºtil para testadores de penetraÃ§Ã£o. # CaracterÃ­sticas - Gera
 payloads CSRF com foco em exploraÃ§Ã£o de falsificaÃ§Ã£o de requisiÃ§Ãµes entre
 sites. # Forma de utilizaÃ§Ã£o ```sh csrfmap -a "http://exemplo.com" -m post -
 p form1 -n username password token -v victor password 132423542 ``` Isso
 exibirÃ¡ a ajuda para a ferramenta. Aqui estÃ£o todos os switches que ele
 suporta: ```yaml _____ _____ _____ _____ _____ _____ _____ | | __| __ | __| | _
 | _ | | --|__ | -| __| | | | | __| |_____|_____|__|__|__| |_|_|_|__|__|__|
-v0.0.3 - @joaoviictorti options: -h, --help show this help message and exit -
+v0.0.5 - @joaoviictorti options: -h, --help show this help message and exit -
 a ACTION, -A ACTION Insert action -m METHOD, -M METHOD Insert method -p
 {form1,form2,json1,json2} -n NAME [NAME ...], -name NAME [NAME ...] Insert name
 -v VALUE [VALUE ...], -value VALUE [VALUE ...] Insert values ``` # InstalaÃ§Ã£o
 csrfmap requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install
 csrfmap ``` # Executando csrfmap ```console csrfmap -a "http://exemplo.com" -
 m post -p form1 -n username password token -v victor password 132423542 _____
 _____ _____ _____ _____ _____ _____ | | __| __ | __| | _ | _ | | --|__ | -| __|
```

### Comparing `csrfmap-0.0.4/csrfmap/csrfmap.py` & `csrfmap-0.0.5/csrfmap/csrfmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 def banner():
     return """                      
  _____ _____ _____ _____ _____ _____ _____ 
 |     |   __| __  |   __|     |  _  |  _  |
 |   --|__   |    -|   __| | | |     |   __|
 |_____|_____|__|__|__|  |_|_|_|__|__|__|   
                                                        
-                        v0.0.4 - @joaoviictorti 
+                        v0.0.5 - @joaoviictorti 
     """
 def argumentos():
     parser = argparse.ArgumentParser(prog=banner(),usage="csrfmap -a \"http://exemplo.com\" -m post -p form2 -n username password token -v victor password 132423542",formatter_class=RawTextHelpFormatter)
-    parser.add_argument("--version",action="version",version="csrfmap 0.0.4")
+    parser.add_argument("--version",action="version",version="csrfmap 0.0.5")
     parser.add_argument("-a","-A",dest="action",action="store",type=str,required=True,help="Insert action")
     parser.add_argument("-m","-M",dest="method",action="store",type=str,required=True,help="Insert method")
     parser.add_argument("-p",dest="payload",action="store",type=str,help=False,choices=["form1","form2","json1","json2"])
     parser.add_argument("-n","-name",nargs="+",dest="name",action="store",required=True,help="Insert name")
     parser.add_argument("-v","-value",nargs="+",dest="value",action="store",required=False,default="__valor__",help="Insert values")
     args = parser.parse_args()
```

### Comparing `csrfmap-0.0.4/csrfmap/payloads.py` & `csrfmap-0.0.5/csrfmap/payloads.py`

 * *Files identical despite different names*

### Comparing `csrfmap-0.0.4/PKG-INFO` & `csrfmap-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csrfmap
-Version: 0.0.4
+Version: 0.0.5
 Summary: csrfmap (Payloads Cross Site Request Forgery)
 Home-page: https://github.com/joaoviictorti/csrfmap
 License: MIT
 Author: João
 Author-email: joaovictorti08@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -47,15 +47,15 @@
 Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
 ```yaml
  _____ _____ _____ _____ _____ _____ _____ 
 |     |   __| __  |   __|     |  _  |  _  |
 |   --|__   |    -|   __| | | |     |   __|
 |_____|_____|__|__|__|  |_|_|_|__|__|__|   
                                                        
-                        v0.0.3 - @joaoviictorti 
+                        v0.0.5 - @joaoviictorti 
 
 options:
   -h, --help            show this help message and exit
   -a ACTION, -A ACTION  Insert action
   -m METHOD, -M METHOD  Insert method
   -p {form1,form2,json1,json2}
   -n NAME [NAME ...], -name NAME [NAME ...] Insert name
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: csrfmap Version: 0.0.4 Summary: csrfmap (Payloads
+Metadata-Version: 2.1 Name: csrfmap Version: 0.0.5 Summary: csrfmap (Payloads
 Cross Site Request Forgery) Home-page: https://github.com/joaoviictorti/csrfmap
 License: MIT Author: JoÃ£o Author-email: joaovictorti08@gmail.com Requires-
 Python: >=3.11,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Description-Content-Type: text/markdown [https://
 capsule-render.vercel.app/
 api?type=waving&color=0000FF&height=120&section=header] [![Typing SVG](https://
@@ -17,15 +17,15 @@
 para tornÃ¡-lo Ãºtil para testadores de penetraÃ§Ã£o. # CaracterÃ­sticas - Gera
 payloads CSRF com foco em exploraÃ§Ã£o de falsificaÃ§Ã£o de requisiÃ§Ãµes entre
 sites. # Forma de utilizaÃ§Ã£o ```sh csrfmap -a "http://exemplo.com" -m post -
 p form1 -n username password token -v victor password 132423542 ``` Isso
 exibirÃ¡ a ajuda para a ferramenta. Aqui estÃ£o todos os switches que ele
 suporta: ```yaml _____ _____ _____ _____ _____ _____ _____ | | __| __ | __| | _
 | _ | | --|__ | -| __| | | | | __| |_____|_____|__|__|__| |_|_|_|__|__|__|
-v0.0.3 - @joaoviictorti options: -h, --help show this help message and exit -
+v0.0.5 - @joaoviictorti options: -h, --help show this help message and exit -
 a ACTION, -A ACTION Insert action -m METHOD, -M METHOD Insert method -p
 {form1,form2,json1,json2} -n NAME [NAME ...], -name NAME [NAME ...] Insert name
 -v VALUE [VALUE ...], -value VALUE [VALUE ...] Insert values ``` # InstalaÃ§Ã£o
 csrfmap requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install
 csrfmap ``` # Executando csrfmap ```console csrfmap -a "http://exemplo.com" -
 m post -p form1 -n username password token -v victor password 132423542 _____
 _____ _____ _____ _____ _____ _____ | | __| __ | __| | _ | _ | | --|__ | -| __|
```

