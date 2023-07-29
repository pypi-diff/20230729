# Comparing `tmp/revmap-0.0.5.tar.gz` & `tmp/revmap-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revmap-0.0.5.tar", last modified: Thu Jun  8 13:25:05 2023, max compression
+gzip compressed data, was "revmap-0.0.6.tar", max compression
```

## Comparing `revmap-0.0.5.tar` & `revmap-0.0.6.tar`

### file list

```diff
@@ -1,35 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:05.222013 revmap-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-08 13:24:53.000000 revmap-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-08 13:25:05.222013 revmap-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-08 13:24:53.000000 revmap-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:05.222013 revmap-0.0.5/revmap/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/__meta__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/encoded.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:05.222013 revmap-0.0.5/revmap/events/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/events/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/revmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:05.222013 revmap-0.0.5/revmap/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/settings/color_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/settings/message_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/settings/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:05.222013 revmap-0.0.5/revmap/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/utils/generator_payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/utils/validator_required.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:05.222013 revmap-0.0.5/revmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-08 13:25:05.000000 revmap-0.0.5/revmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-08 13:25:05.000000 revmap-0.0.5/revmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:25:05.000000 revmap-0.0.5/revmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 13:25:05.000000 revmap-0.0.5/revmap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:25:05.000000 revmap-0.0.5/revmap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 13:25:05.000000 revmap-0.0.5/revmap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 13:25:05.222013 revmap-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-08 13:24:53.000000 revmap-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:05.222013 revmap-0.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:53.000000 revmap-0.0.5/test/__init__.py
+-rw-r--r--   0        0        0     1078 2023-07-29 15:53:34.786997 revmap-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2145 2023-07-29 15:53:34.786997 revmap-0.0.6/README.md
+-rw-r--r--   0        0        0      508 2023-07-29 15:53:34.790998 revmap-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/__init__.py
+-rw-r--r--   0        0        0      554 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/encoded.py
+-rw-r--r--   0        0        0       23 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/events/__init__.py
+-rw-r--r--   0        0        0      311 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/events/keyboard.py
+-rw-r--r--   0        0        0     4010 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/payloads.py
+-rw-r--r--   0        0        0      999 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/revmap.py
+-rw-r--r--   0        0        0       86 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/settings/__init__.py
+-rw-r--r--   0        0        0      729 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/settings/color_settings.py
+-rw-r--r--   0        0        0      706 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/settings/message_settings.py
+-rw-r--r--   0        0        0      219 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/settings/variables.py
+-rw-r--r--   0        0        0       57 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/utils/__init__.py
+-rw-r--r--   0        0        0     2177 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/utils/commands.py
+-rw-r--r--   0        0        0     3378 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/utils/generator_payloads.py
+-rw-r--r--   0        0        0     1003 2023-07-29 15:53:34.790998 revmap-0.0.6/revmap/utils/validator_required.py
+-rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 revmap-0.0.6/PKG-INFO
```

### Comparing `revmap-0.0.5/LICENSE` & `revmap-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `revmap-0.0.5/README.md` & `revmap-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ```
 Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
 ```yaml
  ___ ___ _ _ _____ ___ ___ 
 |  _| -_| | |     | .'| . |
 |_| |___|\_/|_|_|_|__,|  _|
                       |_|  
-        v0.0.5 - @joaoviictorti 
+        v0.0.6 - @joaoviictorti 
 
 options:
   -h, --help    show this help message and exit
   --version     show program's version number and exit
   --ip IP       Insert ip
   --port PORTA  Insert port
 ```
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
-. | |_| |___|\_/|_|_|_|__,| _| |_| v0.0.5 - @joaoviictorti options: -h, --help
+. | |_| |___|\_/|_|_|_|__,| _| |_| v0.0.6 - @joaoviictorti options: -h, --help
 show this help message and exit --version show program's version number and
 exit --ip IP Insert ip --port PORTA Insert port ``` # InstalaÃ§Ã£o revmap
 requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install revmap ``` #
 Executando revmap ![logo_do_projeto](images/revmap_console.png) [https://
 capsule-render.vercel.app/
 api?type=waving&color=0000FF&height=120&section=footer]
```

### Comparing `revmap-0.0.5/revmap/encoded.py` & `revmap-0.0.6/revmap/encoded.py`

 * *Files identical despite different names*

### Comparing `revmap-0.0.5/revmap/payloads.py` & `revmap-0.0.6/revmap/payloads.py`

 * *Files identical despite different names*

### Comparing `revmap-0.0.5/revmap/revmap.py` & `revmap-0.0.6/revmap/revmap.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 def banner() -> str:
     return """
  ___ ___ _ _ _____ ___ ___ 
 |  _| -_| | |     | .'| . |
 |_| |___|\_/|_|_|_|__,|  _|
                       |_|  
-        v0.0.5 - @joaoviictorti                          
+        v0.0.6 - @joaoviictorti                          
 """
 
 
 def argumentos() -> None:
     global args
     parser = argparse.ArgumentParser(
         prog=banner(),
         usage='revmap --ip 192.168.4.80 --port 4444',
         formatter_class=RawTextHelpFormatter,
     )
-    parser.add_argument('--version', action='version', version='revmap 0.0.5')
+    parser.add_argument('--version', action='version', version='revmap 0.0.6')
     parser.add_argument(
         '--ip',
         type=str,
         dest='ip',
         action='store',
         help='Insert ip',
         required=True,
```

### Comparing `revmap-0.0.5/revmap/settings/color_settings.py` & `revmap-0.0.6/revmap/settings/color_settings.py`

 * *Files identical despite different names*

### Comparing `revmap-0.0.5/revmap/settings/message_settings.py` & `revmap-0.0.6/revmap/settings/message_settings.py`

 * *Files identical despite different names*

### Comparing `revmap-0.0.5/revmap/utils/commands.py` & `revmap-0.0.6/revmap/utils/commands.py`

 * *Files identical despite different names*

### Comparing `revmap-0.0.5/revmap/utils/generator_payloads.py` & `revmap-0.0.6/revmap/utils/generator_payloads.py`

 * *Files identical despite different names*

### Comparing `revmap-0.0.5/revmap/utils/validator_required.py` & `revmap-0.0.6/revmap/utils/validator_required.py`

 * *Files identical despite different names*

