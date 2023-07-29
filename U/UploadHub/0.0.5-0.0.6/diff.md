# Comparing `tmp/UploadHub-0.0.5.tar.gz` & `tmp/UploadHub-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UploadHub-0.0.5.tar", last modified: Thu Jul 27 19:30:01 2023, max compression
+gzip compressed data, was "UploadHub-0.0.6.tar", last modified: Sat Jul 29 21:16:57 2023, max compression
```

## Comparing `UploadHub-0.0.5.tar` & `UploadHub-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 19:30:01.890541 UploadHub-0.0.5/
--rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:02.000000 UploadHub-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      516 2023-07-27 19:30:01.888539 UploadHub-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-18 18:43:42.000000 UploadHub-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 19:30:01.843536 UploadHub-0.0.5/UploadHub/
--rw-rw-rw-   0        0        0        0 2023-07-23 05:01:02.000000 UploadHub-0.0.5/UploadHub/__init__.py
--rw-rw-rw-   0        0        0      704 2023-07-23 05:09:33.000000 UploadHub-0.0.5/UploadHub/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 19:30:01.885537 UploadHub-0.0.5/UploadHub/data/
--rw-rw-rw-   0        0        0      112 2023-07-23 04:18:02.000000 UploadHub-0.0.5/UploadHub/data/config.json
--rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:06.000000 UploadHub-0.0.5/UploadHub/license.py
--rw-rw-rw-   0        0        0     9815 2023-07-23 05:09:52.000000 UploadHub-0.0.5/UploadHub/new.py
--rw-rw-rw-   0        0        0      651 2023-07-19 04:20:31.000000 UploadHub-0.0.5/UploadHub/setup.py
--rw-rw-rw-   0        0        0     8234 2023-07-27 19:28:22.000000 UploadHub-0.0.5/UploadHub/upload.py
--rw-rw-rw-   0        0        0     2345 2023-07-27 01:39:15.000000 UploadHub-0.0.5/UploadHub/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 19:30:01.881540 UploadHub-0.0.5/UploadHub.egg-info/
--rw-rw-rw-   0        0        0      516 2023-07-27 19:30:01.000000 UploadHub-0.0.5/UploadHub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-07-27 19:30:01.000000 UploadHub-0.0.5/UploadHub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 19:30:01.000000 UploadHub-0.0.5/UploadHub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-27 19:30:01.000000 UploadHub-0.0.5/UploadHub.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-27 19:30:01.000000 UploadHub-0.0.5/UploadHub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 19:30:01.891540 UploadHub-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      884 2023-07-27 19:29:53.000000 UploadHub-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:16:57.352767 UploadHub-0.0.6/
+-rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:02.000000 UploadHub-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      516 2023-07-29 21:16:57.350761 UploadHub-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-18 18:43:42.000000 UploadHub-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 21:16:57.294761 UploadHub-0.0.6/UploadHub/
+-rw-rw-rw-   0        0        0        0 2023-07-23 05:01:02.000000 UploadHub-0.0.6/UploadHub/__init__.py
+-rw-rw-rw-   0        0        0      722 2023-07-29 20:58:27.000000 UploadHub-0.0.6/UploadHub/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:16:57.348760 UploadHub-0.0.6/UploadHub/data/
+-rw-rw-rw-   0        0        0      112 2023-07-23 04:18:02.000000 UploadHub-0.0.6/UploadHub/data/config.json
+-rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:06.000000 UploadHub-0.0.6/UploadHub/license.py
+-rw-rw-rw-   0        0        0     9824 2023-07-29 20:58:38.000000 UploadHub-0.0.6/UploadHub/new.py
+-rw-rw-rw-   0        0        0      651 2023-07-19 04:20:31.000000 UploadHub-0.0.6/UploadHub/setup.py
+-rw-rw-rw-   0        0        0     8938 2023-07-29 21:16:05.000000 UploadHub-0.0.6/UploadHub/upload.py
+-rw-rw-rw-   0        0        0     2345 2023-07-27 01:39:15.000000 UploadHub-0.0.6/UploadHub/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:16:57.336772 UploadHub-0.0.6/UploadHub.egg-info/
+-rw-rw-rw-   0        0        0      516 2023-07-29 21:16:57.000000 UploadHub-0.0.6/UploadHub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-07-29 21:16:57.000000 UploadHub-0.0.6/UploadHub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 21:16:57.000000 UploadHub-0.0.6/UploadHub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-29 21:16:57.000000 UploadHub-0.0.6/UploadHub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-29 21:16:57.000000 UploadHub-0.0.6/UploadHub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 21:16:57.354762 UploadHub-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      884 2023-07-29 20:56:08.000000 UploadHub-0.0.6/setup.py
```

### Comparing `UploadHub-0.0.5/LICENSE` & `UploadHub-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.5/PKG-INFO` & `UploadHub-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UploadHub
-Version: 0.0.5
+Version: 0.0.6
 Summary: PYPI and GitHub package uploader.
 Author: Armando Chaparro
 Author-email: <pylejandria@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `UploadHub-0.0.5/UploadHub/__main__.py` & `UploadHub-0.0.6/UploadHub/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
-from .new import NewPackage
-from .upload import UploadPackage
+from UploadHub.new import NewPackage
+from UploadHub.upload import UploadPackage
 
 # TERMINAL ARGUMENTS
 parser = argparse.ArgumentParser(prog='UploadHub', description='Manages package uploads')
 parser.add_argument('mode')
 args = parser.parse_args()
 mode = args.mode
```

### Comparing `UploadHub-0.0.5/UploadHub/license.py` & `UploadHub-0.0.6/UploadHub/license.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.5/UploadHub/new.py` & `UploadHub-0.0.6/UploadHub/new.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import subprocess
 import ttkbootstrap as ttk
-from .utils import load_config, StatusBar
+from UploadHub.utils import load_config, StatusBar
 from tkinter.filedialog import askdirectory
 
 
 class NewPackage(ttk.Window):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `UploadHub-0.0.5/UploadHub/setup.py` & `UploadHub-0.0.6/UploadHub/setup.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.5/UploadHub/upload.py` & `UploadHub-0.0.6/UploadHub/upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 import subprocess
 import ttkbootstrap as ttk
-from .utils import StatusBar
+from UploadHub.utils import StatusBar
 from tkinter.filedialog import askdirectory
 
 
 class UploadPackage(ttk.Window):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         # VARIABLES
-        options = ['No', 'Yes']
+        options = ['Yes', 'No']
 
         # USER INTERFACE
         package_frame = ttk.LabelFrame(self, text='package Info')
         package_frame.pack(expand=True, fill='x', padx=10, pady=10)
         ttk.Label(package_frame, text='Package directory ').grid(row=0, column=0, sticky='w', padx=10, pady=(5, 0))
         self.package_dir = ttk.Entry(package_frame, width=70, state='readonly')
         self.package_dir.grid(row=0, column=1, sticky='w', padx=10, pady=(5, 0))
@@ -40,26 +40,30 @@
         self.commit_git.grid(row=1, column=1, sticky='w', padx=10, pady=5)
 
         files_frame = ttk.LabelFrame(self, text='File Info')
         files_frame.pack(expand=True, fill='x', padx=10, pady=10)
         ttk.Label(files_frame, text='Delete past version').grid(row=0, column=0, sticky='w', padx=10, pady=(5, 0))
         self.delete_past = ttk.Combobox(files_frame, width=10, values=options, state='readonly')
         self.delete_past.grid(row=0, column=1, sticky='w', padx=10, pady=(5, 0))
-        self.delete_past.current(1)
+        self.delete_past.current(0)
         ttk.Label(files_frame, text='Update version').grid(row=1, column=0, sticky='w', padx=10, pady=5)
         self.update_version = ttk.Combobox(files_frame, width=10, values=options, state='readonly')
         self.update_version.grid(row=1, column=1, sticky='w', padx=10, pady=5)
-        self.update_version.current(1)
+        self.update_version.current(0)
 
         pypi_frame = ttk.LabelFrame(self, text='Pypi Info')
         pypi_frame.pack(expand=True, fill='x', padx=10, pady=10)
         ttk.Label(pypi_frame, text='Upload to Pypi ').grid(row=0, column=0, sticky='w', padx=10, pady=5)
         self.upload_pypi = ttk.Combobox(pypi_frame, width=10, values=options, state='readonly')
         self.upload_pypi.grid(row=0, column=1, sticky='w', padx=10, pady=5)
         self.upload_pypi.current(0)
+        ttk.Label(pypi_frame, text='Pip install ').grid(row=1, column=0, sticky='w', padx=10, pady=5)
+        self.pip_install = ttk.Combobox(pypi_frame, width=10, values=options, state='readonly')
+        self.pip_install.grid(row=1, column=1, sticky='w', padx=10, pady=5)
+        self.pip_install.current(0)
 
         create_button = ttk.Button(self, text='Upload package...', bootstyle='success', command=self.upload_package)
         create_button.pack(expand=True, fill='x', padx=10, pady=10)
 
         self.status_bar = StatusBar(self)
         self.status_bar.pack(expand=True, fill='x')
 
@@ -144,14 +148,15 @@
         if not (version := self.check_entry(self.version)): return
         
         # GIT INFO
         push_git = self.push_git.get()
         delete_past = self.delete_past.get()
         update_version = self.update_version.get()
         upload_pypi = self.upload_pypi.get()
+        pip_install = self.pip_install.get()
         dist_folder = os.path.join(package_dir, 'dist')
 
         # DELETE PREVIOUS VERSIONS IF NEEDED
         if delete_past == 'Yes' and os.path.isdir(dist_folder):
             for file in os.listdir(dist_folder):
                 os.remove(os.path.join(dist_folder, file))
 
@@ -169,9 +174,20 @@
         
         # UPDATE GIT REPOSITORY IF NEEDED
         if push_git == 'Yes':
             if not (commit_git := self.check_entry(self.commit_git)): return
             self.run('git add .', package_dir)
             subprocess.run(['git', 'commit', '-m', f'"{commit_git}"'], cwd=package_dir)
             self.run('git push', package_dir)
+        
+        # UPGRADE PACKAGE
+        if pip_install == 'Yes':
+            package_name = package_dir.split('/')[-1]
+            self.run(f'pip install {package_name} --upgrade')
+            self.run(f'pip install {package_name} --upgrade')
 
         self.status_bar.info('Package successfully uploaded...')
+
+
+if __name__ == '__main__':
+    window = UploadPackage()
+    window.mainloop()
```

### Comparing `UploadHub-0.0.5/UploadHub/utils.py` & `UploadHub-0.0.6/UploadHub/utils.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.5/UploadHub.egg-info/PKG-INFO` & `UploadHub-0.0.6/UploadHub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UploadHub
-Version: 0.0.5
+Version: 0.0.6
 Summary: PYPI and GitHub package uploader.
 Author: Armando Chaparro
 Author-email: <pylejandria@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `UploadHub-0.0.5/setup.py` & `UploadHub-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'PYPI and GitHub package uploader.'
 LONG_DESCRIPTION = 'Manages all the commands to upload a package to PYPI and GitHub repo.'
 
 setup(
     name='UploadHub',
     version=VERSION,
     author="Armando Chaparro",
```

