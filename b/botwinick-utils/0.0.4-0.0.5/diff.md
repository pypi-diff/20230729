# Comparing `tmp/botwinick_utils-0.0.4.tar.gz` & `tmp/botwinick_utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botwinick_utils-0.0.4.tar", last modified: Sat Jul 29 18:20:22 2023, max compression
+gzip compressed data, was "botwinick_utils-0.0.5.tar", last modified: Sat Jul 29 18:36:11 2023, max compression
```

## Comparing `botwinick_utils-0.0.4.tar` & `botwinick_utils-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-29 18:20:22.251235 botwinick_utils-0.0.4/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1551 2020-10-15 18:46:33.000000 botwinick_utils-0.0.4/LICENSE
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      743 2023-07-29 18:20:22.239218 botwinick_utils-0.0.4/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      167 2020-10-15 18:46:33.000000 botwinick_utils-0.0.4/README.md
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-29 18:20:21.485934 botwinick_utils-0.0.4/botwinick_utils/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      193 2020-10-15 18:50:25.000000 botwinick_utils-0.0.4/botwinick_utils/__init__.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-29 18:20:21.948446 botwinick_utils-0.0.4/botwinick_utils/binary/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      269 2020-10-17 21:29:14.000000 botwinick_utils-0.0.4/botwinick_utils/binary/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2328 2020-10-21 23:51:54.000000 botwinick_utils-0.0.4/botwinick_utils/binary/b32.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      108 2020-10-15 18:53:01.000000 botwinick_utils-0.0.4/botwinick_utils/compat.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2786 2020-08-28 20:10:42.000000 botwinick_utils-0.0.4/botwinick_utils/io.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7380 2023-07-29 18:18:40.000000 botwinick_utils-0.0.4/botwinick_utils/net.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5752 2020-08-28 20:39:08.000000 botwinick_utils-0.0.4/botwinick_utils/paths.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-29 18:20:22.151711 botwinick_utils-0.0.4/botwinick_utils/platforms/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3680 2020-08-28 20:10:42.000000 botwinick_utils-0.0.4/botwinick_utils/platforms/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5491 2020-08-28 20:10:42.000000 botwinick_utils-0.0.4/botwinick_utils/platforms/linux.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7059 2020-09-29 22:46:34.000000 botwinick_utils-0.0.4/botwinick_utils/platforms/threading.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1552 2020-08-28 20:10:42.000000 botwinick_utils-0.0.4/botwinick_utils/pretty.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3952 2020-08-28 20:10:42.000000 botwinick_utils-0.0.4/botwinick_utils/regex.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2223 2020-10-16 01:26:56.000000 botwinick_utils-0.0.4/botwinick_utils/util.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-29 18:20:21.795199 botwinick_utils-0.0.4/botwinick_utils.egg-info/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      743 2023-07-29 18:20:19.000000 botwinick_utils-0.0.4/botwinick_utils.egg-info/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      596 2023-07-29 18:20:20.000000 botwinick_utils-0.0.4/botwinick_utils.egg-info/SOURCES.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-29 18:20:19.000000 botwinick_utils-0.0.4/botwinick_utils.egg-info/dependency_links.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        4 2023-07-29 18:20:19.000000 botwinick_utils-0.0.4/botwinick_utils.egg-info/requires.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       16 2023-07-29 18:20:19.000000 botwinick_utils-0.0.4/botwinick_utils.egg-info/top_level.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-29 18:20:22.255219 botwinick_utils-0.0.4/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      870 2023-07-29 18:16:31.000000 botwinick_utils-0.0.4/setup.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-29 18:36:11.055312 botwinick_utils-0.0.5/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1551 2020-10-15 18:46:33.000000 botwinick_utils-0.0.5/LICENSE
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      743 2023-07-29 18:36:11.040309 botwinick_utils-0.0.5/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      167 2020-10-15 18:46:33.000000 botwinick_utils-0.0.5/README.md
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-29 18:36:09.802568 botwinick_utils-0.0.5/botwinick_utils/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      193 2020-10-15 18:50:25.000000 botwinick_utils-0.0.5/botwinick_utils/__init__.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-29 18:36:10.514794 botwinick_utils-0.0.5/botwinick_utils/binary/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      269 2020-10-17 21:29:14.000000 botwinick_utils-0.0.5/botwinick_utils/binary/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2328 2020-10-21 23:51:54.000000 botwinick_utils-0.0.5/botwinick_utils/binary/b32.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      108 2020-10-15 18:53:01.000000 botwinick_utils-0.0.5/botwinick_utils/compat.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2786 2020-08-28 20:10:42.000000 botwinick_utils-0.0.5/botwinick_utils/io.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7614 2023-07-29 18:35:03.000000 botwinick_utils-0.0.5/botwinick_utils/net.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5752 2020-08-28 20:39:08.000000 botwinick_utils-0.0.5/botwinick_utils/paths.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-29 18:36:10.904073 botwinick_utils-0.0.5/botwinick_utils/platforms/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3680 2020-08-28 20:10:42.000000 botwinick_utils-0.0.5/botwinick_utils/platforms/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5491 2020-08-28 20:10:42.000000 botwinick_utils-0.0.5/botwinick_utils/platforms/linux.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7059 2020-09-29 22:46:34.000000 botwinick_utils-0.0.5/botwinick_utils/platforms/threading.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1552 2020-08-28 20:10:42.000000 botwinick_utils-0.0.5/botwinick_utils/pretty.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3952 2020-08-28 20:10:42.000000 botwinick_utils-0.0.5/botwinick_utils/regex.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2223 2020-10-16 01:26:56.000000 botwinick_utils-0.0.5/botwinick_utils/util.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-29 18:36:10.271539 botwinick_utils-0.0.5/botwinick_utils.egg-info/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      743 2023-07-29 18:36:06.000000 botwinick_utils-0.0.5/botwinick_utils.egg-info/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      596 2023-07-29 18:36:08.000000 botwinick_utils-0.0.5/botwinick_utils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-29 18:36:06.000000 botwinick_utils-0.0.5/botwinick_utils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        4 2023-07-29 18:36:06.000000 botwinick_utils-0.0.5/botwinick_utils.egg-info/requires.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       16 2023-07-29 18:36:06.000000 botwinick_utils-0.0.5/botwinick_utils.egg-info/top_level.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-29 18:36:11.060310 botwinick_utils-0.0.5/setup.cfg
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      870 2023-07-29 18:33:59.000000 botwinick_utils-0.0.5/setup.py
```

### Comparing `botwinick_utils-0.0.4/LICENSE` & `botwinick_utils-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `botwinick_utils-0.0.4/PKG-INFO` & `botwinick_utils-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botwinick_utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: Assorted Utilities and platform code
 Home-page: https://github.com/dbotwinick/botwinick_utils
 Author: Drew Botwinick
 Author-email: foss@drewbotwinick.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `botwinick_utils-0.0.4/botwinick_utils/binary/b32.py` & `botwinick_utils-0.0.5/botwinick_utils/binary/b32.py`

 * *Files identical despite different names*

### Comparing `botwinick_utils-0.0.4/botwinick_utils/io.py` & `botwinick_utils-0.0.5/botwinick_utils/io.py`

 * *Files identical despite different names*

### Comparing `botwinick_utils-0.0.4/botwinick_utils/net.py` & `botwinick_utils-0.0.5/botwinick_utils/net.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,65 +51,14 @@
             s.close()
     return result
 
 
 try:
     # TODO: Borrowed from pyrra code--finish separating out code from util/support code from pyrra and make that its own library
 
-    import netifaces
-
-
-    def system_ip_interfaces(excluded_adapters=('lo',), ipv4=True, ipv6=False, target_adapters=()):
-        """
-        Return system ip interfaces
-
-        NOTE: requires netifaces package and python 3.3+
-
-        :param excluded_adapters:
-        :param ipv4:
-        :param ipv6:
-        :param target_adapters:
-        :return:
-        """
-        result = []
-        interfaces = netifaces.interfaces()
-        for iface in interfaces:
-            if target_adapters and iface not in target_adapters:
-                continue
-            elif iface in excluded_adapters:
-                continue
-            data = netifaces.ifaddresses(iface)
-            if ipv4 and netifaces.AF_INET in data:
-                for a in data[netifaces.AF_INET]:
-                    result.append(IPv4Interface((a['addr'], a['netmask'])))
-            if ipv6 and netifaces.AF_INET6 in data:
-                for a in data[netifaces.AF_INET6]:
-                    result.append(IPv6Interface((a['addr'], a['netmask'])))
-
-        return result
-
-
-    def get_default_gateway(ipv4=True):
-        """
-        Return system ip interfaces
-
-        NOTE: requires netifaces package and python 3.3+
-
-        :param ipv4:
-        :return: gw_adapter_name, gw_ip
-        """
-        gw = netifaces.gateways()
-        gw_ip, gw_adapter = gw['default'][netifaces.AF_INET if ipv4 else netifaces.AF_INET6]
-        return gw_adapter, gw_ip
-except ImportError:
-    pass
-
-try:
-    # TODO: Borrowed from pyrra code--finish separating out code from util/support code from pyrra and make that its own library
-
     # noinspection PyCompatibility
     from ipaddress import (ip_network, IPv4Network, IPv6Network, IPv4Interface, IPv6Interface, ip_interface,
                            collapse_addresses)
 
 
     class SubnetGroup(object):
         _nets = None
@@ -138,14 +87,15 @@
                 return self
             else:
                 new_net = ip_network(new_net, strict=not allow_hosts)  # type: IPv4Network
 
             self._nets = list(collapse_addresses(nets + [new_net]))
             return self
 
+        # noinspection PyCompatibility
         def remove(self, exclude_net, allow_hosts=True):
             nets = self._nets
             if isinstance(exclude_net, (IPv4Network, IPv6Network)):
                 pass
             elif isinstance(exclude_net, SubnetGroup):
                 for net in exclude_net.children:
                     self.remove(net)
@@ -197,7 +147,61 @@
         pass
 
 
     PRIVATE_LANS = SubnetGroup('10.0.0.0/8', '172.16.0.0/12')
     ALL_PRIVATE_LANS = SubnetGroup('10.0.0.0/8', '172.16.0.0/12', '192.168.0.0/16')
 except ImportError:
     pass
+
+try:
+    # TODO: Borrowed from pyrra code--finish separating out code from util/support code from pyrra and make that its own library
+
+    import netifaces
+    # noinspection PyCompatibility
+    from ipaddress import (ip_network, IPv4Network, IPv6Network, IPv4Interface, IPv6Interface, ip_interface,
+                           collapse_addresses)
+
+
+    def system_ip_interfaces(excluded_adapters=('lo',), ipv4=True, ipv6=False, target_adapters=()):
+        """
+        Return system ip interfaces
+
+        NOTE: requires netifaces package and python 3.3+
+
+        :param excluded_adapters:
+        :param ipv4:
+        :param ipv6:
+        :param target_adapters:
+        :return:
+        """
+        result = []
+        interfaces = netifaces.interfaces()
+        for iface in interfaces:
+            if target_adapters and iface not in target_adapters:
+                continue
+            elif iface in excluded_adapters:
+                continue
+            data = netifaces.ifaddresses(iface)
+            if ipv4 and netifaces.AF_INET in data:
+                for a in data[netifaces.AF_INET]:
+                    result.append(IPv4Interface((a['addr'], a['netmask'])))
+            if ipv6 and netifaces.AF_INET6 in data:
+                for a in data[netifaces.AF_INET6]:
+                    result.append(IPv6Interface((a['addr'], a['netmask'])))
+
+        return result
+
+
+    def get_default_gateway(ipv4=True):
+        """
+        Return system ip interfaces
+
+        NOTE: requires netifaces package and python 3.3+
+
+        :param ipv4:
+        :return: gw_adapter_name, gw_ip
+        """
+        gw = netifaces.gateways()
+        gw_ip, gw_adapter = gw['default'][netifaces.AF_INET if ipv4 else netifaces.AF_INET6]
+        return gw_adapter, gw_ip
+except ImportError:
+    pass
```

### Comparing `botwinick_utils-0.0.4/botwinick_utils/paths.py` & `botwinick_utils-0.0.5/botwinick_utils/paths.py`

 * *Files identical despite different names*

### Comparing `botwinick_utils-0.0.4/botwinick_utils/platforms/__init__.py` & `botwinick_utils-0.0.5/botwinick_utils/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `botwinick_utils-0.0.4/botwinick_utils/platforms/linux.py` & `botwinick_utils-0.0.5/botwinick_utils/platforms/linux.py`

 * *Files identical despite different names*

### Comparing `botwinick_utils-0.0.4/botwinick_utils/platforms/threading.py` & `botwinick_utils-0.0.5/botwinick_utils/platforms/threading.py`

 * *Files identical despite different names*

### Comparing `botwinick_utils-0.0.4/botwinick_utils/pretty.py` & `botwinick_utils-0.0.5/botwinick_utils/pretty.py`

 * *Files identical despite different names*

### Comparing `botwinick_utils-0.0.4/botwinick_utils/regex.py` & `botwinick_utils-0.0.5/botwinick_utils/regex.py`

 * *Files identical despite different names*

### Comparing `botwinick_utils-0.0.4/botwinick_utils/util.py` & `botwinick_utils-0.0.5/botwinick_utils/util.py`

 * *Files identical despite different names*

### Comparing `botwinick_utils-0.0.4/botwinick_utils.egg-info/PKG-INFO` & `botwinick_utils-0.0.5/botwinick_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botwinick-utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: Assorted Utilities and platform code
 Home-page: https://github.com/dbotwinick/botwinick_utils
 Author: Drew Botwinick
 Author-email: foss@drewbotwinick.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `botwinick_utils-0.0.4/botwinick_utils.egg-info/SOURCES.txt` & `botwinick_utils-0.0.5/botwinick_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botwinick_utils-0.0.4/setup.py` & `botwinick_utils-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", 'r') as f:
     readme_txt = f.read()
 
 setuptools.setup(
     name="botwinick_utils",
-    version="0.0.4",
+    version="0.0.5",
     author="Drew Botwinick",
     author_email="foss@drewbotwinick.com",
     description="Assorted Utilities and platform code",
     long_description=readme_txt,
     long_description_content_type="text/markdown",
     url="https://github.com/dbotwinick/botwinick_utils",
     packages=setuptools.find_packages(),
```

