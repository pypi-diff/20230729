# Comparing `tmp/UploadHub-0.0.6.tar.gz` & `tmp/UploadHub-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UploadHub-0.0.6.tar", last modified: Sat Jul 29 21:16:57 2023, max compression
+gzip compressed data, was "UploadHub-0.0.7.tar", last modified: Sat Jul 29 21:45:03 2023, max compression
```

## Comparing `UploadHub-0.0.6.tar` & `UploadHub-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 21:16:57.352767 UploadHub-0.0.6/
--rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:02.000000 UploadHub-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      516 2023-07-29 21:16:57.350761 UploadHub-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-18 18:43:42.000000 UploadHub-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 21:16:57.294761 UploadHub-0.0.6/UploadHub/
--rw-rw-rw-   0        0        0        0 2023-07-23 05:01:02.000000 UploadHub-0.0.6/UploadHub/__init__.py
--rw-rw-rw-   0        0        0      722 2023-07-29 20:58:27.000000 UploadHub-0.0.6/UploadHub/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 21:16:57.348760 UploadHub-0.0.6/UploadHub/data/
--rw-rw-rw-   0        0        0      112 2023-07-23 04:18:02.000000 UploadHub-0.0.6/UploadHub/data/config.json
--rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:06.000000 UploadHub-0.0.6/UploadHub/license.py
--rw-rw-rw-   0        0        0     9824 2023-07-29 20:58:38.000000 UploadHub-0.0.6/UploadHub/new.py
--rw-rw-rw-   0        0        0      651 2023-07-19 04:20:31.000000 UploadHub-0.0.6/UploadHub/setup.py
--rw-rw-rw-   0        0        0     8938 2023-07-29 21:16:05.000000 UploadHub-0.0.6/UploadHub/upload.py
--rw-rw-rw-   0        0        0     2345 2023-07-27 01:39:15.000000 UploadHub-0.0.6/UploadHub/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-29 21:16:57.336772 UploadHub-0.0.6/UploadHub.egg-info/
--rw-rw-rw-   0        0        0      516 2023-07-29 21:16:57.000000 UploadHub-0.0.6/UploadHub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-07-29 21:16:57.000000 UploadHub-0.0.6/UploadHub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 21:16:57.000000 UploadHub-0.0.6/UploadHub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-29 21:16:57.000000 UploadHub-0.0.6/UploadHub.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-29 21:16:57.000000 UploadHub-0.0.6/UploadHub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 21:16:57.354762 UploadHub-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      884 2023-07-29 20:56:08.000000 UploadHub-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:45:03.628714 UploadHub-0.0.7/
+-rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:02.000000 UploadHub-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      516 2023-07-29 21:45:03.625713 UploadHub-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-18 18:43:42.000000 UploadHub-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 21:45:03.579712 UploadHub-0.0.7/UploadHub/
+-rw-rw-rw-   0        0        0        0 2023-07-23 05:01:02.000000 UploadHub-0.0.7/UploadHub/__init__.py
+-rw-rw-rw-   0        0        0      722 2023-07-29 20:58:27.000000 UploadHub-0.0.7/UploadHub/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:45:03.623727 UploadHub-0.0.7/UploadHub/data/
+-rw-rw-rw-   0        0        0      112 2023-07-23 04:18:02.000000 UploadHub-0.0.7/UploadHub/data/config.json
+-rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:06.000000 UploadHub-0.0.7/UploadHub/license.py
+-rw-rw-rw-   0        0        0     9824 2023-07-29 20:58:38.000000 UploadHub-0.0.7/UploadHub/new.py
+-rw-rw-rw-   0        0        0      651 2023-07-19 04:20:31.000000 UploadHub-0.0.7/UploadHub/setup.py
+-rw-rw-rw-   0        0        0     8972 2023-07-29 21:44:21.000000 UploadHub-0.0.7/UploadHub/upload.py
+-rw-rw-rw-   0        0        0     2345 2023-07-27 01:39:15.000000 UploadHub-0.0.7/UploadHub/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:45:03.620715 UploadHub-0.0.7/UploadHub.egg-info/
+-rw-rw-rw-   0        0        0      516 2023-07-29 21:45:03.000000 UploadHub-0.0.7/UploadHub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-07-29 21:45:03.000000 UploadHub-0.0.7/UploadHub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 21:45:03.000000 UploadHub-0.0.7/UploadHub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-29 21:45:03.000000 UploadHub-0.0.7/UploadHub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-29 21:45:03.000000 UploadHub-0.0.7/UploadHub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 21:45:03.629714 UploadHub-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      884 2023-07-29 21:44:27.000000 UploadHub-0.0.7/setup.py
```

### Comparing `UploadHub-0.0.6/LICENSE` & `UploadHub-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.6/PKG-INFO` & `UploadHub-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UploadHub
-Version: 0.0.6
+Version: 0.0.7
 Summary: PYPI and GitHub package uploader.
 Author: Armando Chaparro
 Author-email: <pylejandria@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `UploadHub-0.0.6/UploadHub/__main__.py` & `UploadHub-0.0.7/UploadHub/__main__.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.6/UploadHub/license.py` & `UploadHub-0.0.7/UploadHub/license.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.6/UploadHub/new.py` & `UploadHub-0.0.7/UploadHub/new.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.6/UploadHub/setup.py` & `UploadHub-0.0.7/UploadHub/setup.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.6/UploadHub/upload.py` & `UploadHub-0.0.7/UploadHub/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,16 +178,16 @@
             self.run('git add .', package_dir)
             subprocess.run(['git', 'commit', '-m', f'"{commit_git}"'], cwd=package_dir)
             self.run('git push', package_dir)
         
         # UPGRADE PACKAGE
         if pip_install == 'Yes':
             package_name = package_dir.split('/')[-1]
-            self.run(f'pip install {package_name} --upgrade')
-            self.run(f'pip install {package_name} --upgrade')
+            self.run(f'pip install {package_name} --upgrade', cwd=package_dir)
+            self.run(f'pip install {package_name} --upgrade', cwd=package_dir)
 
         self.status_bar.info('Package successfully uploaded...')
 
 
 if __name__ == '__main__':
     window = UploadPackage()
     window.mainloop()
```

### Comparing `UploadHub-0.0.6/UploadHub/utils.py` & `UploadHub-0.0.7/UploadHub/utils.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.6/UploadHub.egg-info/PKG-INFO` & `UploadHub-0.0.7/UploadHub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UploadHub
-Version: 0.0.6
+Version: 0.0.7
 Summary: PYPI and GitHub package uploader.
 Author: Armando Chaparro
 Author-email: <pylejandria@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `UploadHub-0.0.6/setup.py` & `UploadHub-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'PYPI and GitHub package uploader.'
 LONG_DESCRIPTION = 'Manages all the commands to upload a package to PYPI and GitHub repo.'
 
 setup(
     name='UploadHub',
     version=VERSION,
     author="Armando Chaparro",
```

