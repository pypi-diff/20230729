# Comparing `tmp/csrfmap-0.0.2.tar.gz` & `tmp/csrfmap-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csrfmap-0.0.2.tar", last modified: Fri May 26 00:40:43 2023, max compression
+gzip compressed data, was "csrfmap-0.0.3.tar", max compression
```

## Comparing `csrfmap-0.0.2.tar` & `csrfmap-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,7 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:40:43.845135 csrfmap-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-26 00:40:29.000000 csrfmap-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-26 00:40:43.845135 csrfmap-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-26 00:40:29.000000 csrfmap-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:40:43.845135 csrfmap-0.0.2/csrfmap/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 00:40:29.000000 csrfmap-0.0.2/csrfmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-26 00:40:29.000000 csrfmap-0.0.2/csrfmap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-26 00:40:29.000000 csrfmap-0.0.2/csrfmap/__meta__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-26 00:40:29.000000 csrfmap-0.0.2/csrfmap/csrfmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-05-26 00:40:29.000000 csrfmap-0.0.2/csrfmap/payloads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:40:43.845135 csrfmap-0.0.2/csrfmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-26 00:40:43.000000 csrfmap-0.0.2/csrfmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-26 00:40:43.000000 csrfmap-0.0.2/csrfmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:40:43.000000 csrfmap-0.0.2/csrfmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-26 00:40:43.000000 csrfmap-0.0.2/csrfmap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:40:43.000000 csrfmap-0.0.2/csrfmap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 00:40:43.000000 csrfmap-0.0.2/csrfmap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 00:40:43.845135 csrfmap-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-26 00:40:29.000000 csrfmap-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:40:43.845135 csrfmap-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 00:40:29.000000 csrfmap-0.0.2/test/__init__.py
+-rw-r--r--   0        0        0     1078 2023-07-29 16:41:18.110315 csrfmap-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2765 2023-07-29 16:41:18.110315 csrfmap-0.0.3/README.md
+-rw-r--r--   0        0        0       46 2023-07-29 16:41:18.110315 csrfmap-0.0.3/csrfmap/__init__.py
+-rw-r--r--   0        0        0     3301 2023-07-29 16:41:18.110315 csrfmap-0.0.3/csrfmap/csrfmap.py
+-rw-r--r--   0        0        0     4987 2023-07-29 16:41:18.110315 csrfmap-0.0.3/csrfmap/payloads.py
+-rw-r--r--   0        0        0      449 2023-07-29 16:41:18.114315 csrfmap-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3210 1970-01-01 00:00:00.000000 csrfmap-0.0.3/PKG-INFO
```

### Comparing `csrfmap-0.0.2/LICENSE` & `csrfmap-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `csrfmap-0.0.2/README.md` & `csrfmap-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
 ```yaml
  _____ _____ _____ _____ _____ _____ _____ 
 |     |   __| __  |   __|     |  _  |  _  |
 |   --|__   |    -|   __| | | |     |   __|
 |_____|_____|__|__|__|  |_|_|_|__|__|__|   
                                                        
-                        v0.0.2 - @joaoviictorti 
+                        v0.0.3 - @joaoviictorti 
 
 options:
   -h, --help            show this help message and exit
   -a ACTION, -A ACTION  Insert action
   -m METHOD, -M METHOD  Insert method
   -p {form1,form2,json1,json2}
   -n NAME [NAME ...], -name NAME [NAME ...] Insert name
@@ -63,15 +63,15 @@
 csrfmap -a "http://exemplo.com" -m post -p form1 -n username password token -v victor password 132423542
 
  _____ _____ _____ _____ _____ _____ _____ 
 |     |   __| __  |   __|     |  _  |  _  |
 |   --|__   |    -|   __| | | |     |   __|
 |_____|_____|__|__|__|  |_|_|_|__|__|__|   
                                                        
-                        v0.0.2 - @joaoviictorti   
+                        v0.0.3 - @joaoviictorti   
 
 csrf.html:
 <!DOCTYPE html>
 <html lang="pt-br">
 <body>
 	<form action="http://exemplo.com" method="post">
 	<input name="username" value="victor" type="hidden"/>
```

#### html2text {}

```diff
@@ -11,20 +11,20 @@
 para tornÃ¡-lo Ãºtil para testadores de penetraÃ§Ã£o. # CaracterÃ­sticas - Gera
 payloads CSRF com foco em exploraÃ§Ã£o de falsificaÃ§Ã£o de requisiÃ§Ãµes entre
 sites. # Forma de utilizaÃ§Ã£o ```sh csrfmap -a "http://exemplo.com" -m post -
 t forminteraction -n username password token -v victor password 132423542 ```
 Isso exibirÃ¡ a ajuda para a ferramenta. Aqui estÃ£o todos os switches que ele
 suporta: ```yaml _____ _____ _____ _____ _____ _____ _____ | | __| __ | __| | _
 | _ | | --|__ | -| __| | | | | __| |_____|_____|__|__|__| |_|_|_|__|__|__|
-v0.0.2 - @joaoviictorti options: -h, --help show this help message and exit -
+v0.0.3 - @joaoviictorti options: -h, --help show this help message and exit -
 a ACTION, -A ACTION Insert action -m METHOD, -M METHOD Insert method -p
 {form1,form2,json1,json2} -n NAME [NAME ...], -name NAME [NAME ...] Insert name
 -v VALUE [VALUE ...], -value VALUE [VALUE ...] Insert values ``` # InstalaÃ§Ã£o
 csrfmap requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install
 csrfmap ``` # Executando csrfmap ```console csrfmap -a "http://exemplo.com" -
 m post -p form1 -n username password token -v victor password 132423542 _____
 _____ _____ _____ _____ _____ _____ | | __| __ | __| | _ | _ | | --|__ | -| __|
-| | | | __| |_____|_____|__|__|__| |_|_|_|__|__|__| v0.0.2 - @joaoviictorti
+| | | | __| |_____|_____|__|__|__| |_|_|_|__|__|__| v0.0.3 - @joaoviictorti
 csrf.html:
    [Submit]Enviar
 ``` [https://capsule-render.vercel.app/
 api?type=waving&color=0000FF&height=120&section=footer]
```

### Comparing `csrfmap-0.0.2/csrfmap/csrfmap.py` & `csrfmap-0.0.3/csrfmap/csrfmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 def banner():
     return """                      
  _____ _____ _____ _____ _____ _____ _____ 
 |     |   __| __  |   __|     |  _  |  _  |
 |   --|__   |    -|   __| | | |     |   __|
 |_____|_____|__|__|__|  |_|_|_|__|__|__|   
                                                        
-                        v0.0.2 - @joaoviictorti 
+                        v0.0.3 - @joaoviictorti 
     """
 def argumentos():
-    parser = argparse.ArgumentParser(prog=banner(),usage="csrfmap -a \"http://exemplo.com\" -m post -p form1 -n username password token",formatter_class=RawTextHelpFormatter)
-    parser.add_argument("--version",action="version",version="csrfmap 0.0.2")
+    parser = argparse.ArgumentParser(prog=banner(),usage="csrfmap -a \"http://exemplo.com\" -m post -p form2 -n username password token -v victor password 132423542",formatter_class=RawTextHelpFormatter)
+    parser.add_argument("--version",action="version",version="csrfmap 0.0.3")
     parser.add_argument("-a","-A",dest="action",action="store",type=str,required=True,help="Insert action")
     parser.add_argument("-m","-M",dest="method",action="store",type=str,required=True,help="Insert method")
     parser.add_argument("-p",dest="payload",action="store",type=str,help=False,choices=["form1","form2","json1","json2"])
     parser.add_argument("-n","-name",nargs="+",dest="name",action="store",required=True,help="Insert name")
     parser.add_argument("-v","-value",nargs="+",dest="value",action="store",required=False,default="__valor__",help="Insert values")
     args = parser.parse_args()
```

### Comparing `csrfmap-0.0.2/csrfmap/payloads.py` & `csrfmap-0.0.3/csrfmap/payloads.py`

 * *Files identical despite different names*

