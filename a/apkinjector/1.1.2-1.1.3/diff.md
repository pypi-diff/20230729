# Comparing `tmp/apkinjector-1.1.2.tar.gz` & `tmp/apkinjector-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkinjector-1.1.2.tar", last modified: Sat Jul 29 17:07:51 2023, max compression
+gzip compressed data, was "apkinjector-1.1.3.tar", last modified: Sat Jul 29 17:27:45 2023, max compression
```

## Comparing `apkinjector-1.1.2.tar` & `apkinjector-1.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:07:51.528080 apkinjector-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-29 17:07:38.000000 apkinjector-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-29 17:07:51.528080 apkinjector-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-07-29 17:07:38.000000 apkinjector-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:07:51.528080 apkinjector-1.1.2/apkinjector/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/apktool.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/frida.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/gadget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/injector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/uber_apk_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:07:51.528080 apkinjector-1.1.2/apkinjector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-29 17:07:51.000000 apkinjector-1.1.2/apkinjector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-29 17:07:51.000000 apkinjector-1.1.2/apkinjector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 17:07:51.000000 apkinjector-1.1.2/apkinjector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-29 17:07:51.000000 apkinjector-1.1.2/apkinjector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-29 17:07:51.000000 apkinjector-1.1.2/apkinjector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-29 17:07:51.000000 apkinjector-1.1.2/apkinjector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 17:07:51.528080 apkinjector-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-29 17:07:38.000000 apkinjector-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:27:45.396623 apkinjector-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-29 17:27:32.000000 apkinjector-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-29 17:27:45.396623 apkinjector-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-07-29 17:27:32.000000 apkinjector-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:27:45.392623 apkinjector-1.1.3/apkinjector/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-29 17:27:32.000000 apkinjector-1.1.3/apkinjector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-07-29 17:27:32.000000 apkinjector-1.1.3/apkinjector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-29 17:27:32.000000 apkinjector-1.1.3/apkinjector/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-29 17:27:32.000000 apkinjector-1.1.3/apkinjector/apktool.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-29 17:27:32.000000 apkinjector-1.1.3/apkinjector/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-29 17:27:32.000000 apkinjector-1.1.3/apkinjector/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-29 17:27:32.000000 apkinjector-1.1.3/apkinjector/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-29 17:27:32.000000 apkinjector-1.1.3/apkinjector/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-29 17:27:32.000000 apkinjector-1.1.3/apkinjector/frida.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-29 17:27:32.000000 apkinjector-1.1.3/apkinjector/gadget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-29 17:27:32.000000 apkinjector-1.1.3/apkinjector/injector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-29 17:27:32.000000 apkinjector-1.1.3/apkinjector/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-29 17:27:32.000000 apkinjector-1.1.3/apkinjector/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-29 17:27:32.000000 apkinjector-1.1.3/apkinjector/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-29 17:27:32.000000 apkinjector-1.1.3/apkinjector/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-29 17:27:32.000000 apkinjector-1.1.3/apkinjector/uber_apk_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-29 17:27:32.000000 apkinjector-1.1.3/apkinjector/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:27:45.396623 apkinjector-1.1.3/apkinjector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-29 17:27:45.000000 apkinjector-1.1.3/apkinjector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-29 17:27:45.000000 apkinjector-1.1.3/apkinjector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 17:27:45.000000 apkinjector-1.1.3/apkinjector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-29 17:27:45.000000 apkinjector-1.1.3/apkinjector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-29 17:27:45.000000 apkinjector-1.1.3/apkinjector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-29 17:27:45.000000 apkinjector-1.1.3/apkinjector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 17:27:45.396623 apkinjector-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-29 17:27:32.000000 apkinjector-1.1.3/setup.py
```

### Comparing `apkinjector-1.1.2/LICENSE` & `apkinjector-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.2/PKG-INFO` & `apkinjector-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkinjector
-Version: 1.1.2
+Version: 1.1.3
 Summary: Utilities to help injecting libraries and frida in apks.
 Home-page: https://nitanmarcel.github.io/apkinjector
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK,INJECTION,INJECT
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkinjector-1.1.2/README.md` & `apkinjector-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.2/apkinjector/__init__.py` & `apkinjector-1.1.3/apkinjector/__init__.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.2/apkinjector/__main__.py` & `apkinjector-1.1.3/apkinjector/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,14 @@
     elif adb:
         Adb.install(None, _install_callback)
         arch = Adb.get_architecture()
         if not arch:
             LOG.info('Waiting for adb device...')
             Adb.wait_for_device()
             arch = Adb.get_architecture()
-            print('yoo',arch)
         if not arch:
             LOG.error(
                 'Failed to connect to any device. Make sure you have adb installed, and the device is properly connected.')
         gadget = Gadget.get_gadget_path(arch)
         if not gadget:
             Gadget.update(_install_callback)
             gadget = Gadget.get_gadget_path(arch)
```

### Comparing `apkinjector-1.1.2/apkinjector/adb.py` & `apkinjector-1.1.3/apkinjector/adb.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
             exe = os.path.join(USER_DIRECTORIES.user_data_dir, 'platform-tools', 'adb')
             os.chmod(exe, 0o755) # set executable permission
             return exe
         if plat == 'Windows':
             return os.path.join(USER_DIRECTORIES.user_data_dir, 'platform-tools', 'adb')
         return None
     plat = platform.system()
+    if platform.machine() not in ['x86_64', 'amd64']:
+        return None
     uri = None
     if plat == 'Linux':
         uri = 'https://dl.google.com/android/repository/platform-tools_r29.0.5-linux.zip'
     if plat == 'Windows':
         uri = 'https://dl.google.com/android/repository/platform-tools_r29.0.5-windows.zip'
     if plat == 'Darwin':
         uri = 'https://dl.google.com/android/repository/platform-tools_r29.0.5-darwin.zip'
```

### Comparing `apkinjector-1.1.2/apkinjector/apktool.py` & `apkinjector-1.1.3/apkinjector/apktool.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.2/apkinjector/bundle.py` & `apkinjector-1.1.3/apkinjector/bundle.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.2/apkinjector/dependencies.py` & `apkinjector-1.1.3/apkinjector/dependencies.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.2/apkinjector/download.py` & `apkinjector-1.1.3/apkinjector/download.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.2/apkinjector/frida.py` & `apkinjector-1.1.3/apkinjector/frida.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.2/apkinjector/gadget.py` & `apkinjector-1.1.3/apkinjector/gadget.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.2/apkinjector/injector.py` & `apkinjector-1.1.3/apkinjector/injector.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.2/apkinjector/java.py` & `apkinjector-1.1.3/apkinjector/java.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.2/apkinjector/logger.py` & `apkinjector-1.1.3/apkinjector/logger.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.2/apkinjector/manifest.py` & `apkinjector-1.1.3/apkinjector/manifest.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.2/apkinjector/plugins.py` & `apkinjector-1.1.3/apkinjector/plugins.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.2/apkinjector/uber_apk_signer.py` & `apkinjector-1.1.3/apkinjector/uber_apk_signer.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.2/apkinjector/utils.py` & `apkinjector-1.1.3/apkinjector/utils.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.2/apkinjector.egg-info/PKG-INFO` & `apkinjector-1.1.3/apkinjector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkinjector
-Version: 1.1.2
+Version: 1.1.3
 Summary: Utilities to help injecting libraries and frida in apks.
 Home-page: https://nitanmarcel.github.io/apkinjector
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK,INJECTION,INJECT
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkinjector-1.1.2/apkinjector.egg-info/SOURCES.txt` & `apkinjector-1.1.3/apkinjector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.2/setup.py` & `apkinjector-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='apkinjector',
-    version='1.1.2',
+    version='1.1.3',
     description='Utilities to help injecting libraries and frida in apks.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Marcel Alexandru Nitan',
     author_email='nitan.marcel@gmail.com',
     url='https://nitanmarcel.github.io/apkinjector',
     keywords=['FRIDA', 'APK', 'INJECTION', 'INJECT'],
```
