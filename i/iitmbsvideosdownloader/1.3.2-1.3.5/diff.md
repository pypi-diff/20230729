# Comparing `tmp/iitmbsvideosdownloader-1.3.2.tar.gz` & `tmp/iitmbsvideosdownloader-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iitmbsvideosdownloader-1.3.2.tar", last modified: Fri Jun  9 12:42:05 2023, max compression
+gzip compressed data, was "iitmbsvideosdownloader-1.3.5.tar", last modified: Fri Jul 28 15:16:19 2023, max compression
```

## Comparing `iitmbsvideosdownloader-1.3.2.tar` & `iitmbsvideosdownloader-1.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-06-09 12:42:05.747823 iitmbsvideosdownloader-1.3.2/
--rwxrwxrwx   0 savi      (1000) savi      (1000)     1081 2023-02-09 17:48:29.000000 iitmbsvideosdownloader-1.3.2/LICENSE.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)      228 2023-06-09 12:42:05.754822 iitmbsvideosdownloader-1.3.2/PKG-INFO
--rwxrwxrwx   0 savi      (1000) savi      (1000)     2315 2023-02-11 12:05:04.000000 iitmbsvideosdownloader-1.3.2/README.md
-drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-06-09 12:42:04.972865 iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader/
--rwxrwxrwx   0 savi      (1000) savi      (1000)      318 2023-02-14 19:22:42.000000 iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader/SITES.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     3814 2023-02-11 11:11:49.000000 iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader/SUBJECTS.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-02-08 09:47:19.000000 iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader/__init__.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     7257 2023-02-24 19:05:01.000000 iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader/_downloader.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     7194 2023-03-06 19:44:07.000000 iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader/_functions.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     5753 2023-06-09 12:36:33.000000 iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader/_iitm.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     4630 2023-02-24 18:59:02.000000 iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader/iitmbsvideosdownloader.py
-drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-06-09 12:42:05.626186 iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader.egg-info/
--rwxrwxrwx   0 savi      (1000) savi      (1000)      228 2023-06-09 12:41:56.000000 iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader.egg-info/PKG-INFO
--rwxrwxrwx   0 savi      (1000) savi      (1000)      527 2023-06-09 12:41:57.000000 iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader.egg-info/SOURCES.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)        1 2023-06-09 12:41:56.000000 iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader.egg-info/dependency_links.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)       16 2023-06-09 12:41:56.000000 iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader.egg-info/requires.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)       23 2023-06-09 12:41:56.000000 iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader.egg-info/top_level.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)      107 2023-06-09 12:42:05.783512 iitmbsvideosdownloader-1.3.2/setup.cfg
--rwxrwxrwx   0 savi      (1000) savi      (1000)      438 2023-06-09 12:39:27.000000 iitmbsvideosdownloader-1.3.2/setup.py
+drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-07-28 15:16:19.179273 iitmbsvideosdownloader-1.3.5/
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     1081 2023-02-09 17:48:29.000000 iitmbsvideosdownloader-1.3.5/LICENSE.txt
+-rwxrwxrwx   0 savi      (1000) savi      (1000)      228 2023-07-28 15:16:19.185278 iitmbsvideosdownloader-1.3.5/PKG-INFO
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     2315 2023-02-11 12:05:04.000000 iitmbsvideosdownloader-1.3.5/README.md
+drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-07-28 15:16:18.332777 iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader/
+-rwxrwxrwx   0 savi      (1000) savi      (1000)      318 2023-02-14 19:22:42.000000 iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader/SITES.py
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     3814 2023-02-11 11:11:49.000000 iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader/SUBJECTS.py
+-rwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-02-08 09:47:19.000000 iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader/__init__.py
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     7257 2023-02-24 19:05:01.000000 iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader/_downloader.py
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     7194 2023-03-06 19:44:07.000000 iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader/_functions.py
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     5753 2023-06-09 12:36:33.000000 iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader/_iitm.py
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     4800 2023-07-28 15:12:04.000000 iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader/iitmbsvideosdownloader.py
+drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-07-28 15:16:19.059555 iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader.egg-info/
+-rwxrwxrwx   0 savi      (1000) savi      (1000)      228 2023-07-28 15:16:10.000000 iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader.egg-info/PKG-INFO
+-rwxrwxrwx   0 savi      (1000) savi      (1000)      527 2023-07-28 15:16:11.000000 iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader.egg-info/SOURCES.txt
+-rwxrwxrwx   0 savi      (1000) savi      (1000)        1 2023-07-28 15:16:10.000000 iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader.egg-info/dependency_links.txt
+-rwxrwxrwx   0 savi      (1000) savi      (1000)       17 2023-07-28 15:16:10.000000 iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader.egg-info/requires.txt
+-rwxrwxrwx   0 savi      (1000) savi      (1000)       23 2023-07-28 15:16:10.000000 iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader.egg-info/top_level.txt
+-rwxrwxrwx   0 savi      (1000) savi      (1000)      107 2023-07-28 15:16:19.216261 iitmbsvideosdownloader-1.3.5/setup.cfg
+-rwxrwxrwx   0 savi      (1000) savi      (1000)      439 2023-07-28 15:13:39.000000 iitmbsvideosdownloader-1.3.5/setup.py
```

### Comparing `iitmbsvideosdownloader-1.3.2/LICENSE.txt` & `iitmbsvideosdownloader-1.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-1.3.2/README.md` & `iitmbsvideosdownloader-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader/SUBJECTS.py` & `iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader/SUBJECTS.py`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader/_downloader.py` & `iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader/_downloader.py`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader/_functions.py` & `iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader/_functions.py`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader/_iitm.py` & `iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader/_iitm.py`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader/iitmbsvideosdownloader.py` & `iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader/iitmbsvideosdownloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,23 +67,26 @@
         options = webdriver.ChromeOptions()
         options.binary_location = self.BROWSER_LOCATION
         # options.binary_location = "C:/Program Files/Google/Chrome/Application/chrome.exe"
         prefs = {
             # "download.default_directory": DOWNLOAD_DIRECTORY,
             "download.prompt_for_download": False,
             "download.directory_upgrade": True,
-            "plugins.always_open_pdf_externally": True,
+            "plugins.always_open_pdf_externally": True
         }
 
         options.add_argument(f'profile-directory={self.PROFILE}')
         options.add_argument(f"user-data-dir={self.USER_DATA_DIRECTORY}")
 
         options.add_experimental_option("prefs", prefs)
         options.add_experimental_option("detach", True)
 
+        # service = ChromeService(executable_path=self.BROWSER_LOCATION)
+        options.add_argument("--start-maximized")
+        # options.add_argument("--headless")
         driver = webdriver.Chrome(options=options)
 
         i = 1
         # loop for each subject, makes sure all subjects are downloaded in their respected folders.
         for subject in self.SELECTED_SUBJECTS:
             subject_name = subject.name
             subject_code = subject.code
```

### Comparing `iitmbsvideosdownloader-1.3.2/iitmbsvideosdownloader.egg-info/SOURCES.txt` & `iitmbsvideosdownloader-1.3.5/iitmbsvideosdownloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

