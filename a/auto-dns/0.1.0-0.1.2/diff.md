# Comparing `tmp/auto_dns-0.1.0.tar.gz` & `tmp/auto_dns-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_dns-0.1.0.tar", max compression
+gzip compressed data, was "auto_dns-0.1.2.tar", max compression
```

## Comparing `auto_dns-0.1.0.tar` & `auto_dns-0.1.2.tar`

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
+-rw-r--r--   0        0        0     1472 2023-07-28 23:19:26.174162 auto_dns-0.1.2/README.rst
+-rw-r--r--   0        0        0       44 2023-07-28 15:45:28.109851 auto_dns-0.1.2/auto_dns/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-28 16:13:43.785870 auto_dns-0.1.2/auto_dns/__main__.py
+-rw-r--r--   0        0        0       60 2023-07-28 15:42:36.901849 auto_dns-0.1.2/auto_dns/dns_providers/__init__.py
+-rw-r--r--   0        0        0     3481 2023-07-28 23:17:53.946161 auto_dns-0.1.2/auto_dns/dns_providers/arvan.py
+-rw-r--r--   0        0        0      415 2023-07-28 14:42:04.569807 auto_dns-0.1.2/auto_dns/dns_providers/base.py
+-rw-r--r--   0        0        0      545 2023-07-28 14:43:06.905808 auto_dns-0.1.2/auto_dns/dns_providers/cloudflare.py
+-rw-r--r--   0        0        0      111 2023-07-28 15:03:00.493821 auto_dns-0.1.2/auto_dns/exceptions.py
+-rw-r--r--   0        0        0     7112 2023-07-28 23:11:10.834156 auto_dns-0.1.2/auto_dns/main.py
+-rw-r--r--   0        0        0      471 2023-07-28 22:56:16.174146 auto_dns-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2360 2023-07-28 23:20:25.853256 auto_dns-0.1.2/setup.py
+-rw-r--r--   0        0        0     1942 2023-07-28 23:20:25.853499 auto_dns-0.1.2/PKG-INFO
```

### Comparing `auto_dns-0.1.0/auto_dns/dns_providers/arvan.py` & `auto_dns-0.1.2/auto_dns/dns_providers/cloudflare.py`

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

### Comparing `auto_dns-0.1.0/setup.py` & `auto_dns-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,24 +4,27 @@
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
+    'version': '0.1.2',
     'description': 'A DNS Python Library.',
-    'long_description': '===================\nAuto DNS Python CLI\n===================\n\nAuto DNS is a Python command line application which automatically updates the DNS records of your domain using various DNS providers.\n\nSupported DNS providers:\n\n- Arvan\n- Cloudflare\n\nThis library is intended to be used on a system with a dynamic public IP that you want to map to a static domain name.\n\nInstallation\n============\n\nThe package can be installed using pip:\n\n.. code-block:: shell\n\n   $ pip install auto-dns\n\nOr if you prefer, you can use Poetry:\n\n.. code-block:: shell\n\n   $ poetry add auto-dns\n\nConfiguration\n=============\n\nTo configure a DNS provider API key, use the following command:\n\n.. code-block:: shell\n\n   $ autodns set_api_key <provider> <api_key>\n\nUsage\n=====\n\nTo update a DNS record with your current public IP, use the following command:\n\n.. code-block:: shell\n\n   $ autodns update <domain> <record_type> <provider>\n\nContributing\n============\n\nContributions are welcome! Please feel free to submit a Pull Request.\n\nLicense\n=======\n\nAuto DNS is released under the MIT License.\n',
+    'long_description': '===================\nAuto DNS Python CLI\n===================\n\nAuto DNS is a Python command line application which automatically updates the DNS records of your domain using various DNS providers.\n\nSupported DNS providers:\n\n- Arvan\n- Cloudflare [coming soon]\n\nThis library is intended to be used on a system with a dynamic public IP that you want to map to a static domain name.\n\nInstallation\n============\n\nThe package can be installed using pip:\n\n.. code-block:: shell\n\n   $ pip install auto-dns\n\nOr if you prefer, you can use Poetry:\n\n.. code-block:: shell\n\n   $ poetry add auto-dns\n\nConfiguration\n=============\n\nTo configure a DNS provider API key, use the following command:\n\n.. code-block:: shell\n\n   $ autodns set_api_key <provider> <api_key>\n\nUsage\n=====\n\nTo create a DNS record:\n\n.. code-block:: shell\n\n   $ autodns create <domain> <record_type> <name> <provider> --ip <ip_address>\n\nTo update a DNS record with your current public IP, use the following command:\n\n.. code-block:: shell\n\n   $ autodns update <domain> <record_type> <name> <provider> --ip <ip_address>\n\nTo delete a DNS record:\n\n.. code-block:: shell\n\n   $ autodns delete <domain> <record_type> <name> <provider>\n\nTo get DNS records:\n\n.. code-block:: shell\n\n   $ autodns get_record <domain> <provider> --record-type <record_type> --name <name>\n\nContributing\n============\n\nContributions are welcome! Please feel free to submit a Pull Request.\n\nLicense\n=======\n\nAuto DNS is released under the MIT License.\n',
     'author': 'Ali Tavallaie',
     'author_email': 'a.tavallaie@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `auto_dns-0.1.0/PKG-INFO` & `auto_dns-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: auto-dns
-Version: 0.1.0
+Version: 0.1.2
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
 
 Auto DNS is a Python command line application which automatically updates the DNS records of your domain using various DNS providers.
 
 Supported DNS providers:
 
 - Arvan
-- Cloudflare
+- Cloudflare [coming soon]
 
 This library is intended to be used on a system with a dynamic public IP that you want to map to a static domain name.
 
 Installation
 ============
 
 The package can be installed using pip:
@@ -48,19 +49,37 @@
 .. code-block:: shell
 
    $ autodns set_api_key <provider> <api_key>
 
 Usage
 =====
 
+To create a DNS record:
+
+.. code-block:: shell
+
+   $ autodns create <domain> <record_type> <name> <provider> --ip <ip_address>
+
 To update a DNS record with your current public IP, use the following command:
 
 .. code-block:: shell
 
-   $ autodns update <domain> <record_type> <provider>
+   $ autodns update <domain> <record_type> <name> <provider> --ip <ip_address>
+
+To delete a DNS record:
+
+.. code-block:: shell
+
+   $ autodns delete <domain> <record_type> <name> <provider>
+
+To get DNS records:
+
+.. code-block:: shell
+
+   $ autodns get_record <domain> <provider> --record-type <record_type> --name <name>
 
 Contributing
 ============
 
 Contributions are welcome! Please feel free to submit a Pull Request.
 
 License
```

