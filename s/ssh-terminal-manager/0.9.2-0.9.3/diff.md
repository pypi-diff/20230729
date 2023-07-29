# Comparing `tmp/ssh_terminal_manager-0.9.2.tar.gz` & `tmp/ssh_terminal_manager-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_terminal_manager-0.9.2.tar", last modified: Sun Jul 23 08:09:34 2023, max compression
+gzip compressed data, was "ssh_terminal_manager-0.9.3.tar", last modified: Sat Jul 29 10:49:55 2023, max compression
```

## Comparing `ssh_terminal_manager-0.9.2.tar` & `ssh_terminal_manager-0.9.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-23 08:09:34.449744 ssh_terminal_manager-0.9.2/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.9.2/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      864 2023-07-23 08:09:34.449744 ssh_terminal_manager-0.9.2/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      223 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.9.2/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      874 2023-07-23 08:09:05.000000 ssh_terminal_manager-0.9.2/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-23 08:09:34.449744 ssh_terminal_manager-0.9.2/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-23 08:09:34.445745 ssh_terminal_manager-0.9.2/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-23 08:09:34.445745 ssh_terminal_manager-0.9.2/src/ssh_terminal_manager/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8859 2023-07-23 04:56:11.000000 ssh_terminal_manager-0.9.2/src/ssh_terminal_manager/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      393 2023-07-23 04:56:11.000000 ssh_terminal_manager-0.9.2/src/ssh_terminal_manager/errors.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-23 08:09:34.449744 ssh_terminal_manager-0.9.2/src/ssh_terminal_manager.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      864 2023-07-23 08:09:34.000000 ssh_terminal_manager-0.9.2/src/ssh_terminal_manager.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      343 2023-07-23 08:09:34.000000 ssh_terminal_manager-0.9.2/src/ssh_terminal_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-23 08:09:34.000000 ssh_terminal_manager-0.9.2/src/ssh_terminal_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       70 2023-07-23 08:09:34.000000 ssh_terminal_manager-0.9.2/src/ssh_terminal_manager.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       21 2023-07-23 08:09:34.000000 ssh_terminal_manager-0.9.2/src/ssh_terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-29 10:49:55.442410 ssh_terminal_manager-0.9.3/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.9.3/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      864 2023-07-29 10:49:55.442410 ssh_terminal_manager-0.9.3/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      223 2023-07-25 07:37:47.000000 ssh_terminal_manager-0.9.3/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      901 2023-07-29 10:49:12.000000 ssh_terminal_manager-0.9.3/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-29 10:49:55.442410 ssh_terminal_manager-0.9.3/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-29 10:49:55.438410 ssh_terminal_manager-0.9.3/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-29 10:49:55.442410 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8824 2023-07-29 10:40:33.000000 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      393 2023-07-23 04:56:11.000000 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager/errors.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1797 2023-07-29 10:39:37.000000 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager/ping_client.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-29 10:49:55.442410 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      864 2023-07-29 10:49:55.000000 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      383 2023-07-29 10:49:55.000000 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-29 10:49:55.000000 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       91 2023-07-29 10:49:55.000000 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       21 2023-07-29 10:49:55.000000 ssh_terminal_manager-0.9.3/src/ssh_terminal_manager.egg-info/top_level.txt
```

### Comparing `ssh_terminal_manager-0.9.2/LICENSE` & `ssh_terminal_manager-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.9.2/PKG-INFO` & `ssh_terminal_manager-0.9.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh_terminal_manager
-Version: 0.9.2
+Version: 0.9.3
 Summary: Use terminal commands to control and monitor remote devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
 Keywords: ssh,terminal,console,shell,bash,cmd,power shell,commands,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssh_terminal_manager-0.9.2/pyproject.toml` & `ssh_terminal_manager-0.9.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_terminal_manager"
-version = "0.9.2"
+version = "0.9.3"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Use terminal commands to control and monitor remote devices"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3.10",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 keywords = [
-  "ssh", 
+  "ssh",
   "terminal",
   "console",
   "shell",
   "bash",
   "cmd",
   "power shell",
   "commands",
   "command line"
 ]
 dependencies = [
+  "async-timeout >= 4.0.2",
   "icmplib >= 3.0",
   "paramiko >= 3.2.0",
   "terminal-manager >= 0.9.2",
   "wakeonlan >= 3.0.0"
 ]
 
 [project.urls]
```

### Comparing `ssh_terminal_manager-0.9.2/src/ssh_terminal_manager/__init__.py` & `ssh_terminal_manager-0.9.3/src/ssh_terminal_manager/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 from .errors import (
     OfflineError,
     SSHAuthenticationError,
     SSHConnectError,
     SSHHostKeyUnknownError,
 )
+from .ping_client import PingClient
 
 _LOGGER = logging.getLogger(__name__)
 _TEST_COMMAND = Command("echo ''")
 
 ONLINE = "online"
 CONNECTED = "connected"
 
@@ -107,14 +108,15 @@
         self.username = username
         self.password = password
         self.key_filename = key_filename
         self.ssh_timeout = ssh_timeout
         self.ping_timeout = ping_timeout
         self._mac_address = None
         self.state = State(self)
+        self.ping_client = PingClient()
         self.client = paramiko.SSHClient()
         self.client.set_log_channel("paramiko")
         self.client.load_system_host_keys()
         self.client.set_missing_host_key_policy(
             paramiko.AutoAddPolicy if add_host_keys else CustomRejectPolicy
         )
 
@@ -243,25 +245,20 @@
             try:
                 await self.async_execute_command(_TEST_COMMAND)
                 return
             except CommandError:
                 pass
 
         try:
-            host = await icmplib.async_ping(
-                self.host,
-                count=1,
-                timeout=self.ping_timeout,
-                privileged=False,
-            )
+            online = await self.ping_client.async_ping(self.host, self.ping_timeout)
         except Exception as exc:  # pylint: disable=broad-except
-            self.logger.debug("%s: Ping request failed (%s)", self.name, exc)
+            self.logger.warning("%s: Ping request failed (%s)", self.name, exc)
             self.state.update(ONLINE, False)
         else:
-            self.state.update(ONLINE, host.is_alive)
+            self.state.update(ONLINE, online)
 
         if not self.state.online:
             if raise_errors:
                 raise OfflineError(f"Host is offline")
             return
 
         try:
```

### Comparing `ssh_terminal_manager-0.9.2/src/ssh_terminal_manager.egg-info/PKG-INFO` & `ssh_terminal_manager-0.9.3/src/ssh_terminal_manager.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-terminal-manager
-Version: 0.9.2
+Version: 0.9.3
 Summary: Use terminal commands to control and monitor remote devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
 Keywords: ssh,terminal,console,shell,bash,cmd,power shell,commands,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

