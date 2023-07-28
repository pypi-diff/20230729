# Comparing `tmp/auto_dns-0.1.0.tar.gz` & `tmp/auto_dns-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_dns-0.1.0.tar", max compression
+gzip compressed data, was "auto_dns-0.1.1.tar", max compression
```

## Comparing `auto_dns-0.1.0.tar` & `auto_dns-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-07-28 16:17:18.513872 auto_dns-0.1.0/README.rst
--rw-r--r--   0        0        0       44 2023-07-28 15:45:28.109851 auto_dns-0.1.0/auto_dns/__init__.py
--rw-r--r--   0        0        0       48 2023-07-28 16:13:43.785870 auto_dns-0.1.0/auto_dns/__main__.py
--rw-r--r--   0        0        0       60 2023-07-28 15:42:36.901849 auto_dns-0.1.0/auto_dns/dns_providers/__init__.py
--rw-r--r--   0        0        0      521 2023-07-28 14:42:23.845807 auto_dns-0.1.0/auto_dns/dns_providers/arvan.py
--rw-r--r--   0        0        0      415 2023-07-28 14:42:04.569807 auto_dns-0.1.0/auto_dns/dns_providers/base.py
--rw-r--r--   0        0        0      545 2023-07-28 14:43:06.905808 auto_dns-0.1.0/auto_dns/dns_providers/cloudflare.py
--rw-r--r--   0        0        0      111 2023-07-28 15:03:00.493821 auto_dns-0.1.0/auto_dns/exceptions.py
--rw-r--r--   0        0        0     3811 2023-07-28 16:11:09.341868 auto_dns-0.1.0/auto_dns/main.py
--rw-r--r--   0        0        0      451 2023-07-28 16:15:02.593871 auto_dns-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1904 2023-07-28 16:17:27.179005 auto_dns-0.1.0/setup.py
--rw-r--r--   0        0        0     1492 2023-07-28 16:17:27.179275 auto_dns-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-28 16:17:18.513872 auto_dns-0.1.1/README.rst
+-rw-r--r--   0        0        0       44 2023-07-28 15:45:28.109851 auto_dns-0.1.1/auto_dns/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-28 16:13:43.785870 auto_dns-0.1.1/auto_dns/__main__.py
+-rw-r--r--   0        0        0       60 2023-07-28 15:42:36.901849 auto_dns-0.1.1/auto_dns/dns_providers/__init__.py
+-rw-r--r--   0        0        0     3469 2023-07-28 22:31:27.362129 auto_dns-0.1.1/auto_dns/dns_providers/arvan.py
+-rw-r--r--   0        0        0      415 2023-07-28 14:42:04.569807 auto_dns-0.1.1/auto_dns/dns_providers/base.py
+-rw-r--r--   0        0        0      545 2023-07-28 14:43:06.905808 auto_dns-0.1.1/auto_dns/dns_providers/cloudflare.py
+-rw-r--r--   0        0        0      111 2023-07-28 15:03:00.493821 auto_dns-0.1.1/auto_dns/exceptions.py
+-rw-r--r--   0        0        0     5686 2023-07-28 22:32:14.234130 auto_dns-0.1.1/auto_dns/main.py
+-rw-r--r--   0        0        0      471 2023-07-28 22:35:36.306132 auto_dns-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1934 2023-07-28 22:35:39.431412 auto_dns-0.1.1/setup.py
+-rw-r--r--   0        0        0     1534 2023-07-28 22:35:39.431645 auto_dns-0.1.1/PKG-INFO
```

### Comparing `auto_dns-0.1.0/README.rst` & `auto_dns-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `auto_dns-0.1.0/auto_dns/dns_providers/arvan.py` & `auto_dns-0.1.1/auto_dns/dns_providers/cloudflare.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from .base import DNSProvider
 
 
-class Arvan(DNSProvider):
-    base_url = "https://napi.arvancloud.com/cdn/4.0/domains"
+class Cloudflare(DNSProvider):
+    base_url = "https://api.cloudflare.com/client/v4/zones"
 
     def get_record(self, domain, record_type):
-        # Implement Arvan's specific API calls
+        # Implement Cloudflare's specific API calls
         pass
 
     def create_record(self, record):
-        # Implement Arvan's specific API calls
+        # Implement Cloudflare's specific API calls
         pass
 
     def update_record(self, record):
-        # Implement Arvan's specific API calls
+        # Implement Cloudflare's specific API calls
         pass
 
     def delete_record(self, record):
-        # Implement Arvan's specific API calls
+        # Implement Cloudflare's specific API calls
         pass
```

### Comparing `auto_dns-0.1.0/auto_dns/main.py` & `auto_dns-0.1.1/auto_dns/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,84 @@
 import os
 import yaml
 import requests
 import typer
-from auto_dns.dns_providers.arvan import Arvan
-from auto_dns.dns_providers.cloudflare import Cloudflare
-from auto_dns.exceptions import UnsupportedProviderError
+from .dns_providers.arvan import Arvan
+from .dns_providers import Cloudflare
+from .exceptions import UnsupportedProviderError
+from tabulate import tabulate
 
 
 class DNSRecord:
-    def __init__(self, domain, record_type, ip):
+    def __init__(self, domain, record_type, ip, name):
         self.domain = domain
         self.record_type = record_type
         self.ip = ip
+        self.name = name
 
 
 class DDNS:
     def __init__(self, provider):
         self.provider = provider
 
-    def get_record(self, domain, record_type):
-        return self.provider.get_record(domain, record_type)
+    def get_record(self, domain, record_type=None, subdomain=None):
+        try:
+
+            records = self.provider.get_record(domain, record_type, subdomain)
+            if records is None:
+                print("No matching records found.")
+                return None
+
+            table = []
+            for item in records:
+                # Make sure 'value' key exists and it is a list
+                if "value" in item and isinstance(item["value"], list):
+                    for value in item["value"]:
+                        # Check if 'ip' key exists in the dictionary
+                        if "ip" in value:
+                            table.append(
+                                [
+                                    item.get("type", "N/A"),
+                                    item.get("name", "N/A"),
+                                    value["ip"],
+                                    item.get("ttl", "N/A"),
+                                    item.get("is_protected", "N/A"),
+                                ]
+                            )
+
+            print(
+                tabulate(
+                    table,
+                    headers=["Type", "Name", "IP", "TTL", "Is Protected"],
+                    tablefmt="pretty",
+                )
+            )
+            return records
+
+        except Exception as e:
+            print(f"Error getting records: {str(e)}")
+            return None
 
     def create_record(self, record):
-        self.provider.create_record(record)
+        try:
+            self.provider.create_record(record)
+        except Exception as e:
+            print(f"An exception occurred in DDNS create_record: {e}")
 
     def update_record(self, record):
-        self.provider.update_record(record)
+        try:
+            self.provider.update_record(record)
+        except Exception as e:
+            print(f"An exception occurred in DDNS update_record: {e}")
 
     def delete_record(self, record):
-        self.provider.delete_record(record)
+        try:
+            self.provider.delete_record(record)
+        except Exception as e:
+            print(f"An exception occurred in DDNS delete_record: {e}")
 
 
 DEFAULT_CONFIG_PATH = os.path.join(os.path.expanduser("~"), ".auto_ddns", "config.yaml")
 
 
 def get_public_ip():
     """Get the public IP address of the device."""
@@ -47,23 +93,25 @@
 
 def write_config(provider_name: str, api_key: str, config_file: str):
     config = {}
     if os.path.exists(config_file):
         with open(config_file, "r") as file:
             config = yaml.safe_load(file) or {}
     config[provider_name] = {"api_key": api_key}
+    os.makedirs(os.path.dirname(config_file), exist_ok=True)
     with open(config_file, "w") as file:
         yaml.dump(config, file)
 
 
 def get_provider(provider_name: str, config_file: str):
     if not os.path.exists(config_file):
         raise FileNotFoundError(f"Config file not found: {config_file}")
     with open(config_file) as file:
         config = yaml.safe_load(file)
+
     if provider_name == "arvan":
         return Arvan(config["arvan"]["api_key"])
     elif provider_name == "cloudflare":
         return Cloudflare(config["cloudflare"]["api_key"])
     else:
         raise UnsupportedProviderError(f"Unsupported provider: {provider_name}")
 
@@ -77,58 +125,68 @@
     if provider not in ["arvan", "cloudflare"]:
         raise UnsupportedProviderError(f"Unsupported provider: {provider}")
     write_config(provider, api_key, config_file)
 
 
 @app.command()
 def get(
-    domain: str, record_type: str, provider: str, config_file: str = DEFAULT_CONFIG_PATH
+    domain: str,
+    provider: str,
+    record_type: str = None,
+    name: str = None,
+    config_file: str = DEFAULT_CONFIG_PATH,
 ):
     provider_instance = get_provider(provider, config_file)
     ddns = DDNS(provider_instance)
-    print(ddns.get_record(domain, record_type))
+    ddns.get_record(domain, record_type, name)
 
 
 @app.command()
 def create(
     domain: str,
     record_type: str,
+    name: str,
     provider: str,
     ip: str = None,
     config_file: str = DEFAULT_CONFIG_PATH,
 ):
     provider_instance = get_provider(provider, config_file)
     ddns = DDNS(provider_instance)
     ip = ip or get_public_ip()
-    record = DNSRecord(domain, record_type, ip)
+    record = DNSRecord(domain, record_type, ip, name)
     ddns.create_record(record)
 
 
 @app.command()
 def update(
     domain: str,
+    name: str,
     record_type: str,
     provider: str,
     ip: str = None,
     config_file: str = DEFAULT_CONFIG_PATH,
 ):
     provider_instance = get_provider(provider, config_file)
     ddns = DDNS(provider_instance)
     ip = ip or get_public_ip()
-    record = DNSRecord(domain, record_type, ip)
+    record = DNSRecord(domain, record_type, ip, name)
     ddns.update_record(record)
 
 
 @app.command()
 def delete(
-    domain: str, record_type: str, provider: str, config_file: str = DEFAULT_CONFIG_PATH
+    domain: str,
+    record_type: str,
+    name: str,
+    provider: str,
+    config_file: str = DEFAULT_CONFIG_PATH,
 ):
     provider_instance = get_provider(provider, config_file)
     ddns = DDNS(provider_instance)
     record = DNSRecord(
-        domain, record_type, "192.168.1.1"
+        domain, record_type, "192.168.1.1", name
     )  # placeholder IP for delete operation
     ddns.delete_record(record)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `auto_dns-0.1.0/setup.py` & `auto_dns-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 packages = \
 ['auto_dns', 'auto_dns.dns_providers']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['PyYAML>=6.0.1,<7.0.0', 'requests>=2.31.0,<3.0.0', 'typer>=0.9.0,<0.10.0']
+['PyYAML>=6.0.1,<7.0.0',
+ 'requests>=2.31.0,<3.0.0',
+ 'tabulate>=0.9.0,<0.10.0',
+ 'typer>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['autodns = auto_dns:app']}
 
 setup_kwargs = {
     'name': 'auto-dns',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A DNS Python Library.',
     'long_description': '===================\nAuto DNS Python CLI\n===================\n\nAuto DNS is a Python command line application which automatically updates the DNS records of your domain using various DNS providers.\n\nSupported DNS providers:\n\n- Arvan\n- Cloudflare\n\nThis library is intended to be used on a system with a dynamic public IP that you want to map to a static domain name.\n\nInstallation\n============\n\nThe package can be installed using pip:\n\n.. code-block:: shell\n\n   $ pip install auto-dns\n\nOr if you prefer, you can use Poetry:\n\n.. code-block:: shell\n\n   $ poetry add auto-dns\n\nConfiguration\n=============\n\nTo configure a DNS provider API key, use the following command:\n\n.. code-block:: shell\n\n   $ autodns set_api_key <provider> <api_key>\n\nUsage\n=====\n\nTo update a DNS record with your current public IP, use the following command:\n\n.. code-block:: shell\n\n   $ autodns update <domain> <record_type> <provider>\n\nContributing\n============\n\nContributions are welcome! Please feel free to submit a Pull Request.\n\nLicense\n=======\n\nAuto DNS is released under the MIT License.\n',
     'author': 'Ali Tavallaie',
     'author_email': 'a.tavallaie@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `auto_dns-0.1.0/PKG-INFO` & `auto_dns-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: auto-dns
-Version: 0.1.0
+Version: 0.1.1
 Summary: A DNS Python Library.
 Author: Ali Tavallaie
 Author-email: a.tavallaie@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/x-rst
 
 ===================
 Auto DNS Python CLI
 ===================
```

