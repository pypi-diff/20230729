# Comparing `tmp/proxy.py-uxspoilers-plugin-2021.5.18.tar.gz` & `tmp/proxy.py-uxspoilers-plugin-2021.5.18.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxy.py-uxspoilers-plugin-2021.5.18.tar", last modified: Tue May 18 11:34:24 2021, max compression
+gzip compressed data, was "proxy.py-uxspoilers-plugin-2021.5.18.post1.tar", last modified: Sat Jul 29 10:11:30 2023, max compression
```

## Comparing `proxy.py-uxspoilers-plugin-2021.5.18.tar` & `proxy.py-uxspoilers-plugin-2021.5.18.post1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 11:34:24.591191 proxy.py-uxspoilers-plugin-2021.5.18/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-05-18 11:34:15.000000 proxy.py-uxspoilers-plugin-2021.5.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3156 2021-05-18 11:34:24.591191 proxy.py-uxspoilers-plugin-2021.5.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2102 2021-05-18 11:34:15.000000 proxy.py-uxspoilers-plugin-2021.5.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 11:34:24.591191 proxy.py-uxspoilers-plugin-2021.5.18/proxy.py_uxspoilers_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3156 2021-05-18 11:34:24.000000 proxy.py-uxspoilers-plugin-2021.5.18/proxy.py_uxspoilers_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      299 2021-05-18 11:34:24.000000 proxy.py-uxspoilers-plugin-2021.5.18/proxy.py_uxspoilers_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-18 11:34:24.000000 proxy.py-uxspoilers-plugin-2021.5.18/proxy.py_uxspoilers_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-05-18 11:34:24.000000 proxy.py-uxspoilers-plugin-2021.5.18/proxy.py_uxspoilers_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-05-18 11:34:24.000000 proxy.py-uxspoilers-plugin-2021.5.18/proxy.py_uxspoilers_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-05-18 11:34:24.591191 proxy.py-uxspoilers-plugin-2021.5.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1364 2021-05-18 11:34:15.000000 proxy.py-uxspoilers-plugin-2021.5.18/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2021-05-18 11:34:15.000000 proxy.py-uxspoilers-plugin-2021.5.18/uxspoilers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:11:30.806578 proxy.py-uxspoilers-plugin-2021.5.18.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-29 10:11:19.000000 proxy.py-uxspoilers-plugin-2021.5.18.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-29 10:11:30.806578 proxy.py-uxspoilers-plugin-2021.5.18.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-29 10:11:19.000000 proxy.py-uxspoilers-plugin-2021.5.18.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:11:30.806578 proxy.py-uxspoilers-plugin-2021.5.18.post1/proxy.py_uxspoilers_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-29 10:11:30.000000 proxy.py-uxspoilers-plugin-2021.5.18.post1/proxy.py_uxspoilers_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-29 10:11:30.000000 proxy.py-uxspoilers-plugin-2021.5.18.post1/proxy.py_uxspoilers_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:11:30.000000 proxy.py-uxspoilers-plugin-2021.5.18.post1/proxy.py_uxspoilers_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 10:11:30.000000 proxy.py-uxspoilers-plugin-2021.5.18.post1/proxy.py_uxspoilers_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 10:11:30.000000 proxy.py-uxspoilers-plugin-2021.5.18.post1/proxy.py_uxspoilers_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-29 10:11:30.806578 proxy.py-uxspoilers-plugin-2021.5.18.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-29 10:11:19.000000 proxy.py-uxspoilers-plugin-2021.5.18.post1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-29 10:11:19.000000 proxy.py-uxspoilers-plugin-2021.5.18.post1/uxspoilers.py
```

### Comparing `proxy.py-uxspoilers-plugin-2021.5.18/LICENSE` & `proxy.py-uxspoilers-plugin-2021.5.18.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `proxy.py-uxspoilers-plugin-2021.5.18/PKG-INFO` & `proxy.py-uxspoilers-plugin-2021.5.18.post1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,72 @@
 Metadata-Version: 2.1
 Name: proxy.py-uxspoilers-plugin
-Version: 2021.5.18
-Summary: UNKNOWN
+Version: 2021.5.18.post1
 Home-page: https://github.com/sakurai-youhei/proxy.py-uxspoilers-plugin
 Author: Youhei Sakurai
 Author-email: sakurai.youhei@gmail.com
 Maintainer: Youhei Sakurai
 Maintainer-email: sakurai.youhei@gmail.com
 License: MIT
-Description: # proxy.py-uxspoilers-plugin
-        
-        A plugin for [proxy.py](https://pypi.org/project/proxy.py/) to spoil UX of web browsing
-        
-        You can spoil User Experience of e.g. YouTube with a combination of [proxy.py](https://pypi.org/project/proxy.py/) plus [proxy.py-uxspoilers-plugin](https://pypi.org/project/proxy.py-uxspoilers-plugin/) and a kind of following [PAC](https://en.wikipedia.org/wiki/Proxy_auto-config)/[WPAD](https://en.wikipedia.org/wiki/Web_Proxy_Auto-Discovery_Protocol) file.
-        
-        ```javascript
-        function FindProxyForURL(url, host)
-        {
-            if (shExpMatch(host, "*youtube*") || shExpMatch(host, "*.googlevideo.com"))
-            {
-                return "PROXY ip-of-your-proxy:8899";
-            }
-            return "DIRECT";
-        }
-        ```
-        
-        Run your proxy server like this:
-        
-        ```console
-        proxy --hostname=0.0.0.0 --pac-file /path/to/wpad.dat --plugin uxspoilers.FixedRustyPumpPlugin --pause-seconds 3
-        ```
-        
-        Your `/etc/dhcp/dhcpd.conf` should look like this:
-        
-        ```ini
-        option wpad code 252 = text;
-        host target-device {
-            option wpad "http://ip-of-your-proxy:8899/wpad.dat";
-            hardware ethernet 2e:8d:8d:xx:xx:xx;
-        }
-        ```
-        
-        Or you may configure your browser's [PAC](https://en.wikipedia.org/wiki/Proxy_auto-config) with `http://ip-of-your-proxy:8899/wpad.dat` manually.
-        
-        ## Installation
-        
-        [![PyPI Version        ](https://img.shields.io/pypi/v/proxy.py-uxspoilers-plugin.svg)](https://pypi.org/project/proxy.py-uxspoilers-plugin/)
-        [![PyPI Downloads      ](https://img.shields.io/pypi/dm/proxy.py-uxspoilers-plugin.svg)](https://pypi.org/project/proxy.py-uxspoilers-plugin/)
-        
-        ```console
-        pip3 install proxy.py-uxspoilers-plugin
-        proxy --help --plugin uxspoilers.RandomRustyPumpPlugin
-        ```
-        
-        ### Docker
-        
-        [![Docker Pulls](https://img.shields.io/docker/pulls/sakuraiyouhei/proxy.py-uxspoilers-plugin)](https://hub.docker.com/r/sakuraiyouhei/proxy.py-uxspoilers-plugin/)
-        [![Image Size  ](https://img.shields.io/docker/image-size/sakuraiyouhei/proxy.py-uxspoilers-plugin)](https://hub.docker.com/r/sakuraiyouhei/proxy.py-uxspoilers-plugin/)
-        
-        ```console
-        docker run -it sakuraiyouhei/proxy.py-uxspoilers-plugin --help --plugin uxspoilers.RandomRustyPumpPlugin
-        ```
-        
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# proxy.py-uxspoilers-plugin
+
+A plugin for [proxy.py](https://pypi.org/project/proxy.py/) to spoil UX of web browsing
+
+You can spoil User Experience of e.g. YouTube with a combination of [proxy.py](https://pypi.org/project/proxy.py/) plus [proxy.py-uxspoilers-plugin](https://pypi.org/project/proxy.py-uxspoilers-plugin/) and a kind of following [PAC](https://en.wikipedia.org/wiki/Proxy_auto-config)/[WPAD](https://en.wikipedia.org/wiki/Web_Proxy_Auto-Discovery_Protocol) file.
+
+```javascript
+function FindProxyForURL(url, host)
+{
+    if (shExpMatch(host, "*youtube*") || shExpMatch(host, "*.googlevideo.com"))
+    {
+        return "PROXY ip-of-your-proxy:8899";
+    }
+    return "DIRECT";
+}
+```
+
+Run your proxy server like this:
+
+```console
+proxy --hostname=0.0.0.0 --pac-file /path/to/wpad.dat --plugin uxspoilers.FixedRustyPumpPlugin --pause-seconds 3
+```
+
+Your `/etc/dhcp/dhcpd.conf` should look like this:
+
+```ini
+option wpad code 252 = text;
+host target-device {
+    option wpad "http://ip-of-your-proxy:8899/wpad.dat";
+    hardware ethernet 2e:8d:8d:xx:xx:xx;
+}
+```
+
+Or you may configure your browser's [PAC](https://en.wikipedia.org/wiki/Proxy_auto-config) with `http://ip-of-your-proxy:8899/wpad.dat` manually.
+
+## Installation
+
+[![PyPI Version        ](https://img.shields.io/pypi/v/proxy.py-uxspoilers-plugin.svg)](https://pypi.org/project/proxy.py-uxspoilers-plugin/)
+[![PyPI Downloads      ](https://img.shields.io/pypi/dm/proxy.py-uxspoilers-plugin.svg)](https://pypi.org/project/proxy.py-uxspoilers-plugin/)
+
+```console
+pip3 install proxy.py-uxspoilers-plugin
+proxy --help --plugin uxspoilers.RandomRustyPumpPlugin
+```
+
+### Docker
+
+[![Docker Pulls](https://img.shields.io/docker/pulls/sakuraiyouhei/proxy.py-uxspoilers-plugin)](https://hub.docker.com/r/sakuraiyouhei/proxy.py-uxspoilers-plugin/)
+[![Image Size  ](https://img.shields.io/docker/image-size/sakuraiyouhei/proxy.py-uxspoilers-plugin)](https://hub.docker.com/r/sakuraiyouhei/proxy.py-uxspoilers-plugin/)
+
+```console
+docker run -it sakuraiyouhei/proxy.py-uxspoilers-plugin --help --plugin uxspoilers.RandomRustyPumpPlugin
+```
```

### Comparing `proxy.py-uxspoilers-plugin-2021.5.18/README.md` & `proxy.py-uxspoilers-plugin-2021.5.18.post1/README.md`

 * *Files identical despite different names*

### Comparing `proxy.py-uxspoilers-plugin-2021.5.18/proxy.py_uxspoilers_plugin.egg-info/PKG-INFO` & `proxy.py-uxspoilers-plugin-2021.5.18.post1/proxy.py_uxspoilers_plugin.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,72 @@
 Metadata-Version: 2.1
 Name: proxy.py-uxspoilers-plugin
-Version: 2021.5.18
-Summary: UNKNOWN
+Version: 2021.5.18.post1
 Home-page: https://github.com/sakurai-youhei/proxy.py-uxspoilers-plugin
 Author: Youhei Sakurai
 Author-email: sakurai.youhei@gmail.com
 Maintainer: Youhei Sakurai
 Maintainer-email: sakurai.youhei@gmail.com
 License: MIT
-Description: # proxy.py-uxspoilers-plugin
-        
-        A plugin for [proxy.py](https://pypi.org/project/proxy.py/) to spoil UX of web browsing
-        
-        You can spoil User Experience of e.g. YouTube with a combination of [proxy.py](https://pypi.org/project/proxy.py/) plus [proxy.py-uxspoilers-plugin](https://pypi.org/project/proxy.py-uxspoilers-plugin/) and a kind of following [PAC](https://en.wikipedia.org/wiki/Proxy_auto-config)/[WPAD](https://en.wikipedia.org/wiki/Web_Proxy_Auto-Discovery_Protocol) file.
-        
-        ```javascript
-        function FindProxyForURL(url, host)
-        {
-            if (shExpMatch(host, "*youtube*") || shExpMatch(host, "*.googlevideo.com"))
-            {
-                return "PROXY ip-of-your-proxy:8899";
-            }
-            return "DIRECT";
-        }
-        ```
-        
-        Run your proxy server like this:
-        
-        ```console
-        proxy --hostname=0.0.0.0 --pac-file /path/to/wpad.dat --plugin uxspoilers.FixedRustyPumpPlugin --pause-seconds 3
-        ```
-        
-        Your `/etc/dhcp/dhcpd.conf` should look like this:
-        
-        ```ini
-        option wpad code 252 = text;
-        host target-device {
-            option wpad "http://ip-of-your-proxy:8899/wpad.dat";
-            hardware ethernet 2e:8d:8d:xx:xx:xx;
-        }
-        ```
-        
-        Or you may configure your browser's [PAC](https://en.wikipedia.org/wiki/Proxy_auto-config) with `http://ip-of-your-proxy:8899/wpad.dat` manually.
-        
-        ## Installation
-        
-        [![PyPI Version        ](https://img.shields.io/pypi/v/proxy.py-uxspoilers-plugin.svg)](https://pypi.org/project/proxy.py-uxspoilers-plugin/)
-        [![PyPI Downloads      ](https://img.shields.io/pypi/dm/proxy.py-uxspoilers-plugin.svg)](https://pypi.org/project/proxy.py-uxspoilers-plugin/)
-        
-        ```console
-        pip3 install proxy.py-uxspoilers-plugin
-        proxy --help --plugin uxspoilers.RandomRustyPumpPlugin
-        ```
-        
-        ### Docker
-        
-        [![Docker Pulls](https://img.shields.io/docker/pulls/sakuraiyouhei/proxy.py-uxspoilers-plugin)](https://hub.docker.com/r/sakuraiyouhei/proxy.py-uxspoilers-plugin/)
-        [![Image Size  ](https://img.shields.io/docker/image-size/sakuraiyouhei/proxy.py-uxspoilers-plugin)](https://hub.docker.com/r/sakuraiyouhei/proxy.py-uxspoilers-plugin/)
-        
-        ```console
-        docker run -it sakuraiyouhei/proxy.py-uxspoilers-plugin --help --plugin uxspoilers.RandomRustyPumpPlugin
-        ```
-        
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# proxy.py-uxspoilers-plugin
+
+A plugin for [proxy.py](https://pypi.org/project/proxy.py/) to spoil UX of web browsing
+
+You can spoil User Experience of e.g. YouTube with a combination of [proxy.py](https://pypi.org/project/proxy.py/) plus [proxy.py-uxspoilers-plugin](https://pypi.org/project/proxy.py-uxspoilers-plugin/) and a kind of following [PAC](https://en.wikipedia.org/wiki/Proxy_auto-config)/[WPAD](https://en.wikipedia.org/wiki/Web_Proxy_Auto-Discovery_Protocol) file.
+
+```javascript
+function FindProxyForURL(url, host)
+{
+    if (shExpMatch(host, "*youtube*") || shExpMatch(host, "*.googlevideo.com"))
+    {
+        return "PROXY ip-of-your-proxy:8899";
+    }
+    return "DIRECT";
+}
+```
+
+Run your proxy server like this:
+
+```console
+proxy --hostname=0.0.0.0 --pac-file /path/to/wpad.dat --plugin uxspoilers.FixedRustyPumpPlugin --pause-seconds 3
+```
+
+Your `/etc/dhcp/dhcpd.conf` should look like this:
+
+```ini
+option wpad code 252 = text;
+host target-device {
+    option wpad "http://ip-of-your-proxy:8899/wpad.dat";
+    hardware ethernet 2e:8d:8d:xx:xx:xx;
+}
+```
+
+Or you may configure your browser's [PAC](https://en.wikipedia.org/wiki/Proxy_auto-config) with `http://ip-of-your-proxy:8899/wpad.dat` manually.
+
+## Installation
+
+[![PyPI Version        ](https://img.shields.io/pypi/v/proxy.py-uxspoilers-plugin.svg)](https://pypi.org/project/proxy.py-uxspoilers-plugin/)
+[![PyPI Downloads      ](https://img.shields.io/pypi/dm/proxy.py-uxspoilers-plugin.svg)](https://pypi.org/project/proxy.py-uxspoilers-plugin/)
+
+```console
+pip3 install proxy.py-uxspoilers-plugin
+proxy --help --plugin uxspoilers.RandomRustyPumpPlugin
+```
+
+### Docker
+
+[![Docker Pulls](https://img.shields.io/docker/pulls/sakuraiyouhei/proxy.py-uxspoilers-plugin)](https://hub.docker.com/r/sakuraiyouhei/proxy.py-uxspoilers-plugin/)
+[![Image Size  ](https://img.shields.io/docker/image-size/sakuraiyouhei/proxy.py-uxspoilers-plugin)](https://hub.docker.com/r/sakuraiyouhei/proxy.py-uxspoilers-plugin/)
+
+```console
+docker run -it sakuraiyouhei/proxy.py-uxspoilers-plugin --help --plugin uxspoilers.RandomRustyPumpPlugin
+```
```

### Comparing `proxy.py-uxspoilers-plugin-2021.5.18/setup.py` & `proxy.py-uxspoilers-plugin-2021.5.18.post1/setup.py`

 * *Files identical despite different names*

### Comparing `proxy.py-uxspoilers-plugin-2021.5.18/uxspoilers.py` & `proxy.py-uxspoilers-plugin-2021.5.18.post1/uxspoilers.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Optional
 
 from proxy.common.flag import flags
 from proxy.http.parser import HttpParser
 from proxy.http.proxy import HttpProxyBasePlugin
 
 
-__version__ = "2021.5.18"
+__version__ = "2021.5.18.post1"
 
 
 flags.add_argument('--pause-seconds',
                    type=float,
                    default=1.0,
                    help=('Default: 1.0.  Flag only applicable when '
                          'FixedRustyPumpPlugin is used for spoiling UX.'))
```

