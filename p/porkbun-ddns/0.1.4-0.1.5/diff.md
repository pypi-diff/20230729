# Comparing `tmp/porkbun_ddns-0.1.4-py3-none-any.whl.zip` & `tmp/porkbun_ddns-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8252 bytes, number of entries: 10
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-23 05:40 porkbun_ddns/__init__.py
--rw-r--r--  2.0 unx     2402 b- defN 23-Jul-23 05:40 porkbun_ddns/cli.py
--rw-r--r--  2.0 unx     1734 b- defN 23-Jul-23 05:40 porkbun_ddns/helpers.py
--rw-r--r--  2.0 unx     6923 b- defN 23-Jul-23 05:40 porkbun_ddns/porkbun_ddns.py
--rw-r--r--  2.0 unx     1061 b- defN 23-Jul-23 05:41 porkbun_ddns-0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     4488 b- defN 23-Jul-23 05:41 porkbun_ddns-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-23 05:41 porkbun_ddns-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 23-Jul-23 05:41 porkbun_ddns-0.1.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Jul-23 05:41 porkbun_ddns-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      831 b- defN 23-Jul-23 05:41 porkbun_ddns-0.1.4.dist-info/RECORD
-10 files, 17681 bytes uncompressed, 6824 bytes compressed:  61.4%
+Zip file size: 8418 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       82 b- defN 23-Jul-29 10:32 porkbun_ddns/__init__.py
+-rw-r--r--  2.0 unx     2708 b- defN 23-Jul-29 10:32 porkbun_ddns/cli.py
+-rw-r--r--  2.0 unx     1734 b- defN 23-Jul-29 10:32 porkbun_ddns/helpers.py
+-rw-r--r--  2.0 unx     8058 b- defN 23-Jul-29 10:32 porkbun_ddns/porkbun_ddns.py
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jul-29 10:32 porkbun_ddns-0.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4488 b- defN 23-Jul-29 10:32 porkbun_ddns-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-29 10:32 porkbun_ddns-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 23-Jul-29 10:32 porkbun_ddns-0.1.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Jul-29 10:32 porkbun_ddns-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      831 b- defN 23-Jul-29 10:32 porkbun_ddns-0.1.5.dist-info/RECORD
+10 files, 19122 bytes uncompressed, 6990 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: porkbun_ddns/helpers.py
 Comment: 
 
 Filename: porkbun_ddns/porkbun_ddns.py
 Comment: 
 
-Filename: porkbun_ddns-0.1.4.dist-info/LICENSE
+Filename: porkbun_ddns-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: porkbun_ddns-0.1.4.dist-info/METADATA
+Filename: porkbun_ddns-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: porkbun_ddns-0.1.4.dist-info/WHEEL
+Filename: porkbun_ddns-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: porkbun_ddns-0.1.4.dist-info/entry_points.txt
+Filename: porkbun_ddns-0.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: porkbun_ddns-0.1.4.dist-info/top_level.txt
+Filename: porkbun_ddns-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: porkbun_ddns-0.1.4.dist-info/RECORD
+Filename: porkbun_ddns-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## porkbun_ddns/cli.py

```diff
@@ -1,18 +1,18 @@
 import argparse
 import sys
 import traceback
 import logging
-from .porkbun_ddns import PorkbunDDNS, PorkbunDDNS_Error
+from porkbun_ddns import PorkbunDDNS, PorkbunDDNS_Error
 
 
 logger = logging.getLogger('porkbun_ddns')
-logger.setLevel(logging.DEBUG)
+logger.setLevel(logging.INFO)
 handler = logging.StreamHandler(sys.stdout)
-handler.setLevel(logging.DEBUG)
+handler.setLevel(logging.INFO)
 formatter = logging.Formatter('%(message)s')
 handler.setFormatter(formatter)
 logger.addHandler(handler)
 
 
 def main(argv=sys.argv[1:]):
     parser = argparse.ArgumentParser(
@@ -35,28 +35,37 @@
 
     ip = parser.add_mutually_exclusive_group()
     ip.add_argument('-4', '--ipv4-only', action='store_true',
                     help="Only set/update IPv4 A Records")
     ip.add_argument('-6', '--ipv6-only', action='store_true',
                     help="Only set/update IPv6 AAAA Records")
 
+    verbose = parser.add_mutually_exclusive_group()
+    verbose.add_argument('-v', '--verbose', action='store_true',
+                    help="Show Debug Output")
+
     if argv and len(argv) == 1:
         parser.print_help()
         exit(1)
     if not argv:
         parser.print_help()
         exit()
 
     args = parser.parse_args(argv)
 
     ipv4 = args.ipv4_only
     ipv6 = args.ipv6_only
     if not any([ipv4, ipv6]):
         ipv4 = ipv6 = True
 
+    if args.verbose:
+        logger.setLevel(logging.DEBUG)
+        for handler in logger.handlers:
+            handler.setLevel(logging.DEBUG)
+
     try:
         porkbun_ddns = PorkbunDDNS(config=args.config, domain=args.domain,
                                    public_ips=args.public_ips, fritzbox_ip=args.fritzbox,
                                    ipv4=ipv4, ipv6=ipv6)
         if args.subdomain:
             porkbun_ddns.set_subdomain(args.subdomain)
         porkbun_ddns.update_records()
```

## porkbun_ddns/porkbun_ddns.py

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 import logging
 import json
 import ipaddress
 import urllib.request
-from .helpers import get_ips_from_fritzbox
+from porkbun_ddns.helpers import get_ips_from_fritzbox
 
 logger = logging.getLogger('porkbun_ddns')
 
+
 class PorkbunDDNS_Error(Exception):
     pass
 
 
 class PorkbunDDNS():
     """A class for updating dynamic DNS records for a Porkbun domain.
     """
@@ -28,18 +29,19 @@
         if isinstance(config, dict):
             self.config = config
         else:
             if isinstance(config, str):
                 try:
                     self._load_config(config)
                 except FileNotFoundError as err:
-                    raise FileNotFoundError("Config path is invalid!\nPath:\n{}".format(config)) from err
+                    raise FileNotFoundError(
+                        "Config path is invalid!\nPath:\n{}".format(config)) from err
             else:
                 raise TypeError("Invalid config! Config should be a str (filepath) or dict!\nYour config:\n{}\nType: {}".format(
-                config, type(config)))
+                    config, type(config)))
 
         self._check_config()
         self.static_ips = public_ips
         self.domain = domain.lower()
         self.records = None
         self.fritzbox_ip = fritzbox_ip
         self.ipv4 = ipv4
@@ -129,44 +131,56 @@
         for ip in self.get_public_ips():
             record_type = "A" if ip.version == 4 else "AAAA"
             if self.fqdn in domain_names:
                 for i in self.records:
                     if i["name"] == self.fqdn:
                         # Overwrite ALIAS and CNAME
                         if i["type"] in ["ALIAS", "CNAME"]:
+                            logger.debug('Overwrite ALIAS and CNAME, with:\n{}'.format(json.dumps(
+                                {"name": self.fqdn, "type": record_type, "content": str(ip.exploded)})))
                             self._delete_record(i['id'])
                             self._create_records(ip, record_type)
                         # Update existing entry
                         if i["type"] == record_type and i['content'] != ip.exploded:
+                            logger.debug('Update existing entry, with:\n{}'.format(json.dumps(
+                                {"name": self.fqdn, "type": record_type, "content": str(ip.exploded)})))
                             self._delete_record(i['id'])
                             self._create_records(ip, record_type)
                         # Create missing A or AAAA entry
-                        if i["type"] not in ["ALIAS", "CNAME", record_type] and record_type not in [x['type'] for x in self.records if x['name'] == self.fqdn]:
+                        if i["type"] in ["A", "AAAA"] and record_type not in [x['type'] for x in self.records if x['name'] == self.fqdn]:
+                            logger.debug('Create missing A or AAAA entry, with:\n{}'.format(json.dumps(
+                                {"name": self.fqdn, "type": record_type, "content": str(ip.exploded)})))
                             self._create_records(ip, record_type)
+                            # Update records
+                            self.records = self.get_records()
                         # Everything is up to date
                         if i["type"] == record_type and i['content'] == ip.exploded:
                             logger.info('{}-Record of {} is up to date!'.format(
                                 i["type"], i["name"]))
             else:
+                logger.debug('Create new record, with:\n{}'.format(json.dumps(
+                    {"name": self.fqdn, "type": record_type, "content": str(ip.exploded)})))
                 # Create new record
                 self._create_records(ip, record_type)
+                # Update records
+                self.records = self.get_records()
 
     def _delete_record(self, domain_id: str):
         """Delete a DNS record with the given domain ID.
         """
 
         type, name, content = [(x['type'], x['name'], x['content'])
                                for x in self.records if x['id'] == domain_id][0]
         status = self._api("/dns/delete/" + self.domain + "/" + domain_id)
         logger.info('Deleting {}-Record for {} with content: {}, Status: {}'.format(type,
-              name, content, status["status"]))
+                                                                                    name, content, status["status"]))
 
     def _create_records(self, ip: ipaddress, record_type: str):
         """Create DNS records for the subdomain with the given IP address and type.
         """
 
         data = self.config.copy()
         data.update({"name": self.subdomain, "type": record_type,
                     "content": ip.exploded, "ttl": 600})
         status = self._api("/dns/create/" + self.domain, data)
         logger.info('Creating {}-Record for {} with content: {}, Status: {}'.format(record_type,
-              self.fqdn, ip.exploded, status["status"]))
+                                                                                    self.fqdn, ip.exploded, status["status"]))
```

## Comparing `porkbun_ddns-0.1.4.dist-info/LICENSE` & `porkbun_ddns-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `porkbun_ddns-0.1.4.dist-info/METADATA` & `porkbun_ddns-0.1.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porkbun-ddns
-Version: 0.1.4
+Version: 0.1.5
 Summary: A unofficial DDNS-Client for Porkbun domains
 Home-page: https://github.com/mietzen/porkbun-ddns
 Author: Nils Stein
 Author-email: github.nstein@mailbox.org
 License: MIT
 Keywords: porkbun ddns
 Classifier: Development Status :: 4 - Beta
```

