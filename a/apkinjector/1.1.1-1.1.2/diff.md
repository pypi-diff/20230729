# Comparing `tmp/apkinjector-1.1.1.tar.gz` & `tmp/apkinjector-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkinjector-1.1.1.tar", last modified: Thu Jul 27 18:28:52 2023, max compression
+gzip compressed data, was "apkinjector-1.1.2.tar", last modified: Sat Jul 29 17:07:51 2023, max compression
```

## Comparing `apkinjector-1.1.1.tar` & `apkinjector-1.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:28:52.702471 apkinjector-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-27 18:28:44.000000 apkinjector-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-27 18:28:52.702471 apkinjector-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-07-27 18:28:44.000000 apkinjector-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:28:52.702471 apkinjector-1.1.1/apkinjector/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-27 18:28:44.000000 apkinjector-1.1.1/apkinjector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16355 2023-07-27 18:28:44.000000 apkinjector-1.1.1/apkinjector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-27 18:28:44.000000 apkinjector-1.1.1/apkinjector/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-27 18:28:44.000000 apkinjector-1.1.1/apkinjector/apktool.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-27 18:28:44.000000 apkinjector-1.1.1/apkinjector/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-27 18:28:44.000000 apkinjector-1.1.1/apkinjector/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-27 18:28:44.000000 apkinjector-1.1.1/apkinjector/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-27 18:28:44.000000 apkinjector-1.1.1/apkinjector/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-27 18:28:44.000000 apkinjector-1.1.1/apkinjector/frida.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-27 18:28:44.000000 apkinjector-1.1.1/apkinjector/gadget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-27 18:28:44.000000 apkinjector-1.1.1/apkinjector/injector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-27 18:28:44.000000 apkinjector-1.1.1/apkinjector/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-27 18:28:44.000000 apkinjector-1.1.1/apkinjector/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-27 18:28:44.000000 apkinjector-1.1.1/apkinjector/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-27 18:28:44.000000 apkinjector-1.1.1/apkinjector/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-27 18:28:44.000000 apkinjector-1.1.1/apkinjector/uber_apk_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-27 18:28:44.000000 apkinjector-1.1.1/apkinjector/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:28:52.702471 apkinjector-1.1.1/apkinjector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-27 18:28:52.000000 apkinjector-1.1.1/apkinjector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-27 18:28:52.000000 apkinjector-1.1.1/apkinjector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:28:52.000000 apkinjector-1.1.1/apkinjector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-27 18:28:52.000000 apkinjector-1.1.1/apkinjector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-27 18:28:52.000000 apkinjector-1.1.1/apkinjector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 18:28:52.000000 apkinjector-1.1.1/apkinjector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 18:28:52.702471 apkinjector-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-27 18:28:44.000000 apkinjector-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:07:51.528080 apkinjector-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-29 17:07:38.000000 apkinjector-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-29 17:07:51.528080 apkinjector-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-07-29 17:07:38.000000 apkinjector-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:07:51.528080 apkinjector-1.1.2/apkinjector/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/apktool.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/frida.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/gadget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/injector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/uber_apk_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-29 17:07:38.000000 apkinjector-1.1.2/apkinjector/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:07:51.528080 apkinjector-1.1.2/apkinjector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-29 17:07:51.000000 apkinjector-1.1.2/apkinjector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-29 17:07:51.000000 apkinjector-1.1.2/apkinjector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 17:07:51.000000 apkinjector-1.1.2/apkinjector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-29 17:07:51.000000 apkinjector-1.1.2/apkinjector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-29 17:07:51.000000 apkinjector-1.1.2/apkinjector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-29 17:07:51.000000 apkinjector-1.1.2/apkinjector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 17:07:51.528080 apkinjector-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-29 17:07:38.000000 apkinjector-1.1.2/setup.py
```

### Comparing `apkinjector-1.1.1/LICENSE` & `apkinjector-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.1/PKG-INFO` & `apkinjector-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkinjector
-Version: 1.1.1
+Version: 1.1.2
 Summary: Utilities to help injecting libraries and frida in apks.
 Home-page: https://nitanmarcel.github.io/apkinjector
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK,INJECTION,INJECT
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkinjector-1.1.1/README.md` & `apkinjector-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.1/apkinjector/__init__.py` & `apkinjector-1.1.2/apkinjector/__init__.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.1/apkinjector/__main__.py` & `apkinjector-1.1.2/apkinjector/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,19 +229,21 @@
                       arch, ARCH.ARM, ARCH.ARM64, ARCH.X86, ARCH.X64)
         Java.install(progress_callback=_install_callback)
         gadget = Gadget.get_gadget_path(arch)
         if not gadget:
             Gadget.update(_install_callback)
             gadget = Gadget.get_gadget_path(arch)
     elif adb:
+        Adb.install(None, _install_callback)
         arch = Adb.get_architecture()
         if not arch:
             LOG.info('Waiting for adb device...')
             Adb.wait_for_device()
             arch = Adb.get_architecture()
+            print('yoo',arch)
         if not arch:
             LOG.error(
                 'Failed to connect to any device. Make sure you have adb installed, and the device is properly connected.')
         gadget = Gadget.get_gadget_path(arch)
         if not gadget:
             Gadget.update(_install_callback)
             gadget = Gadget.get_gadget_path(arch)
```

### Comparing `apkinjector-1.1.1/apkinjector/apktool.py` & `apkinjector-1.1.2/apkinjector/apktool.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.1/apkinjector/bundle.py` & `apkinjector-1.1.2/apkinjector/bundle.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.1/apkinjector/dependencies.py` & `apkinjector-1.1.2/apkinjector/dependencies.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.1/apkinjector/download.py` & `apkinjector-1.1.2/apkinjector/download.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.1/apkinjector/frida.py` & `apkinjector-1.1.2/apkinjector/frida.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.1/apkinjector/gadget.py` & `apkinjector-1.1.2/apkinjector/gadget.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.1/apkinjector/injector.py` & `apkinjector-1.1.2/apkinjector/injector.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.1/apkinjector/java.py` & `apkinjector-1.1.2/apkinjector/java.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.1/apkinjector/logger.py` & `apkinjector-1.1.2/apkinjector/logger.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.1/apkinjector/manifest.py` & `apkinjector-1.1.2/apkinjector/manifest.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.1/apkinjector/plugins.py` & `apkinjector-1.1.2/apkinjector/plugins.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.1/apkinjector/uber_apk_signer.py` & `apkinjector-1.1.2/apkinjector/uber_apk_signer.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.1/apkinjector/utils.py` & `apkinjector-1.1.2/apkinjector/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,17 @@
     Returns:
         Union[ARCH, None]: Converted abi to apkinjector.arch.Arch or None if the abi is not recognized.
     """
     mappings = {
         'armeabi-v7a': ARCH.ARM,
         'arm64_v8a': ARCH.ARM64,
         'x86': ARCH.X86,
-        'x86_64': ARCH.X64
+        'x86_64': ARCH.X64,
+        'arm64-v8a': ARCH.ARM64,
+        'armeabi_v7a': ARCH.ARM
     }
     if abi in mappings.keys():
         return mappings[abi]
     return None
 
 
 def arch_to_abi(arch: ARCH) -> Union[str, None]:
```

### Comparing `apkinjector-1.1.1/apkinjector.egg-info/PKG-INFO` & `apkinjector-1.1.2/apkinjector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkinjector
-Version: 1.1.1
+Version: 1.1.2
 Summary: Utilities to help injecting libraries and frida in apks.
 Home-page: https://nitanmarcel.github.io/apkinjector
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK,INJECTION,INJECT
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkinjector-1.1.1/apkinjector.egg-info/SOURCES.txt` & `apkinjector-1.1.2/apkinjector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apkinjector-1.1.1/setup.py` & `apkinjector-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='apkinjector',
-    version='1.1.1',
+    version='1.1.2',
     description='Utilities to help injecting libraries and frida in apks.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Marcel Alexandru Nitan',
     author_email='nitan.marcel@gmail.com',
     url='https://nitanmarcel.github.io/apkinjector',
     keywords=['FRIDA', 'APK', 'INJECTION', 'INJECT'],
```

