# Comparing `tmp/porkbun_ddns-0.1.5-py3-none-any.whl.zip` & `tmp/porkbun_ddns-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8418 bytes, number of entries: 10
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-29 10:32 porkbun_ddns/__init__.py
--rw-r--r--  2.0 unx     2708 b- defN 23-Jul-29 10:32 porkbun_ddns/cli.py
--rw-r--r--  2.0 unx     1734 b- defN 23-Jul-29 10:32 porkbun_ddns/helpers.py
--rw-r--r--  2.0 unx     8058 b- defN 23-Jul-29 10:32 porkbun_ddns/porkbun_ddns.py
--rw-r--r--  2.0 unx     1061 b- defN 23-Jul-29 10:32 porkbun_ddns-0.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     4488 b- defN 23-Jul-29 10:32 porkbun_ddns-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-29 10:32 porkbun_ddns-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 23-Jul-29 10:32 porkbun_ddns-0.1.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Jul-29 10:32 porkbun_ddns-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      831 b- defN 23-Jul-29 10:32 porkbun_ddns-0.1.5.dist-info/RECORD
-10 files, 19122 bytes uncompressed, 6990 bytes compressed:  63.4%
+Zip file size: 8408 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       82 b- defN 23-Jul-29 11:17 porkbun_ddns/__init__.py
+-rw-r--r--  2.0 unx     2708 b- defN 23-Jul-29 11:17 porkbun_ddns/cli.py
+-rw-r--r--  2.0 unx     1734 b- defN 23-Jul-29 11:17 porkbun_ddns/helpers.py
+-rw-r--r--  2.0 unx     8058 b- defN 23-Jul-29 11:17 porkbun_ddns/porkbun_ddns.py
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jul-29 11:18 porkbun_ddns-0.1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4493 b- defN 23-Jul-29 11:18 porkbun_ddns-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-29 11:18 porkbun_ddns-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 23-Jul-29 11:18 porkbun_ddns-0.1.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Jul-29 11:18 porkbun_ddns-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      831 b- defN 23-Jul-29 11:18 porkbun_ddns-0.1.6.dist-info/RECORD
+10 files, 19127 bytes uncompressed, 6980 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: porkbun_ddns/helpers.py
 Comment: 
 
 Filename: porkbun_ddns/porkbun_ddns.py
 Comment: 
 
-Filename: porkbun_ddns-0.1.5.dist-info/LICENSE
+Filename: porkbun_ddns-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: porkbun_ddns-0.1.5.dist-info/METADATA
+Filename: porkbun_ddns-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: porkbun_ddns-0.1.5.dist-info/WHEEL
+Filename: porkbun_ddns-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: porkbun_ddns-0.1.5.dist-info/entry_points.txt
+Filename: porkbun_ddns-0.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: porkbun_ddns-0.1.5.dist-info/top_level.txt
+Filename: porkbun_ddns-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: porkbun_ddns-0.1.5.dist-info/RECORD
+Filename: porkbun_ddns-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `porkbun_ddns-0.1.5.dist-info/LICENSE` & `porkbun_ddns-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `porkbun_ddns-0.1.5.dist-info/METADATA` & `porkbun_ddns-0.1.6.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porkbun-ddns
-Version: 0.1.5
+Version: 0.1.6
 Summary: A unofficial DDNS-Client for Porkbun domains
 Home-page: https://github.com/mietzen/porkbun-ddns
 Author: Nils Stein
 Author-email: github.nstein@mailbox.org
 License: MIT
 Keywords: porkbun ddns
 Classifier: Development Status :: 4 - Beta
@@ -53,14 +53,15 @@
   -h, --help            show this help message and exit
   -i [PUBLIC_IPS ...], --public-ips [PUBLIC_IPS ...]
                         Public IPs (v4 and or v6)
   -f FRITZBOX, --fritzbox FRITZBOX
                         IP or Domain of your Fritz!Box
   -4, --ipv4-only       Only set/update IPv4 A Records
   -6, --ipv6-only       Only set/update IPv6 AAAA Records
+  -v, --verbose         Show Debug Output
 ```
 
 Examples:
 
 ```shell
 $ porkbun-ddns "./config.json" domain.com my_subdomain
 
@@ -91,15 +92,15 @@
       SECRETAPIKEY: "<YOUR-SECRETAPIKEY>" # Your Porkbun Secret-API-Key
       APIKEY: "<YOUR-APIKEY>" # Your Porkbun API-Key
       # PUBLIC_IPS: "1.2.3.4,2001:043e::1" # Set if you got static IP's
       # FRITZBOX: "192.168.178.1" # Use Fritz!BOX to obtain Public IP's
       # SLEEP: "300" # Seconds to sleep between DynDNS runs
       # IPV4_ONLY: "FALSE" # Only set IPv4 address
       # IPV6_ONLY: "FALSE" # Only set IPv6 address
-      PYTHONUNBUFFERED: 1 # sent stdout and stderr straight to the terminal
+      # DEBUG: "FALSE" # DEBUG LOGGING
     restart: unless-stopped
 ```
 
 # Python
 
 ```python
 from porkbun_ddns import PorkbunDDNS
```

