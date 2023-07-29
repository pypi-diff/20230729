# Comparing `tmp/frida-gadget-1.1.3.tar.gz` & `tmp/frida-gadget-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frida-gadget-1.1.3.tar", last modified: Fri Jul 21 17:16:03 2023, max compression
+gzip compressed data, was "frida-gadget-1.2.0.tar", last modified: Sat Jul 29 08:08:02 2023, max compression
```

## Comparing `frida-gadget-1.1.3.tar` & `frida-gadget-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 17:16:03.348886 frida-gadget-1.1.3/
--rw-rw-rw-   0        0        0     7738 2023-07-21 17:16:03.347887 frida-gadget-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     7067 2023-07-21 16:46:23.000000 frida-gadget-1.1.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-21 17:16:03.339887 frida-gadget-1.1.3/frida_gadget.egg-info/
--rw-rw-rw-   0        0        0     7738 2023-07-21 17:16:03.000000 frida-gadget-1.1.3/frida_gadget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-07-21 17:16:03.000000 frida-gadget-1.1.3/frida_gadget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 17:16:03.000000 frida-gadget-1.1.3/frida_gadget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-21 17:16:03.000000 frida-gadget-1.1.3/frida_gadget.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-07-21 17:16:03.000000 frida-gadget-1.1.3/frida_gadget.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-21 17:16:03.000000 frida-gadget-1.1.3/frida_gadget.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 17:16:03.343886 frida-gadget-1.1.3/scripts/
--rw-rw-rw-   0        0        0      699 2023-07-21 16:46:23.000000 frida-gadget-1.1.3/scripts/__init__.py
--rw-rw-rw-   0        0        0     8974 2023-07-21 17:09:05.000000 frida-gadget-1.1.3/scripts/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:16:03.344887 frida-gadget-1.1.3/scripts/files/
--rw-rw-rw-   0        0        0       84 2023-07-21 16:46:23.000000 frida-gadget-1.1.3/scripts/files/README.md
--rw-rw-rw-   0        0        0     3531 2023-07-21 16:46:23.000000 frida-gadget-1.1.3/scripts/frida_github.py
--rw-rw-rw-   0        0        0      648 2023-07-21 16:46:23.000000 frida-gadget-1.1.3/scripts/logger.py
--rw-rw-rw-   0        0        0       42 2023-07-21 17:16:03.348886 frida-gadget-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1471 2023-07-21 17:15:58.000000 frida-gadget-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:16:03.346887 frida-gadget-1.1.3/tests/
--rw-rw-rw-   0        0        0        0 2023-07-21 16:46:23.000000 frida-gadget-1.1.3/tests/__init__.py
--rw-rw-rw-   0        0        0      418 2023-07-21 16:46:23.000000 frida-gadget-1.1.3/tests/test_cli.py
+drwxr-xr-x   0 ksg        (501) staff       (20)        0 2023-07-29 08:08:02.064094 frida-gadget-1.2.0/
+-rw-r--r--   0 ksg        (501) staff       (20)     7953 2023-07-29 08:08:02.063630 frida-gadget-1.2.0/PKG-INFO
+-rw-r--r--   0 ksg        (501) staff       (20)     7300 2023-07-29 07:55:39.000000 frida-gadget-1.2.0/README.rst
+drwxr-xr-x   0 ksg        (501) staff       (20)        0 2023-07-29 08:08:02.061192 frida-gadget-1.2.0/frida_gadget.egg-info/
+-rw-r--r--   0 ksg        (501) staff       (20)     7953 2023-07-29 08:08:01.000000 frida-gadget-1.2.0/frida_gadget.egg-info/PKG-INFO
+-rw-r--r--   0 ksg        (501) staff       (20)      350 2023-07-29 08:08:02.000000 frida-gadget-1.2.0/frida_gadget.egg-info/SOURCES.txt
+-rw-r--r--   0 ksg        (501) staff       (20)        1 2023-07-29 08:08:01.000000 frida-gadget-1.2.0/frida_gadget.egg-info/dependency_links.txt
+-rw-r--r--   0 ksg        (501) staff       (20)       49 2023-07-29 08:08:01.000000 frida-gadget-1.2.0/frida_gadget.egg-info/entry_points.txt
+-rw-r--r--   0 ksg        (501) staff       (20)       62 2023-07-29 08:08:01.000000 frida-gadget-1.2.0/frida_gadget.egg-info/requires.txt
+-rw-r--r--   0 ksg        (501) staff       (20)       14 2023-07-29 08:08:01.000000 frida-gadget-1.2.0/frida_gadget.egg-info/top_level.txt
+drwxr-xr-x   0 ksg        (501) staff       (20)        0 2023-07-29 08:08:02.062314 frida-gadget-1.2.0/scripts/
+-rw-r--r--   0 ksg        (501) staff       (20)      676 2023-07-29 06:33:05.000000 frida-gadget-1.2.0/scripts/__init__.py
+-rw-r--r--   0 ksg        (501) staff       (20)     9175 2023-07-29 07:55:02.000000 frida-gadget-1.2.0/scripts/cli.py
+-rw-r--r--   0 ksg        (501) staff       (20)     3415 2023-07-29 06:33:05.000000 frida-gadget-1.2.0/scripts/frida_github.py
+-rw-r--r--   0 ksg        (501) staff       (20)      623 2023-07-29 06:33:05.000000 frida-gadget-1.2.0/scripts/logger.py
+-rw-r--r--   0 ksg        (501) staff       (20)       38 2023-07-29 08:08:02.064191 frida-gadget-1.2.0/setup.cfg
+-rw-r--r--   0 ksg        (501) staff       (20)     1419 2023-07-29 07:45:08.000000 frida-gadget-1.2.0/setup.py
+drwxr-xr-x   0 ksg        (501) staff       (20)        0 2023-07-29 08:08:02.063008 frida-gadget-1.2.0/tests/
+-rw-r--r--   0 ksg        (501) staff       (20)        0 2023-07-29 06:33:05.000000 frida-gadget-1.2.0/tests/__init__.py
+-rw-r--r--   0 ksg        (501) staff       (20)      403 2023-07-29 06:33:05.000000 frida-gadget-1.2.0/tests/test_cli.py
```

### Comparing `frida-gadget-1.1.3/PKG-INFO` & `frida-gadget-1.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,159 +1,168 @@
-Metadata-Version: 2.1
-Name: frida-gadget
-Version: 1.1.3
-Summary: Frida gadget into an APK
-Home-page: https://github.com/ksg97031/frida-gadget
-Author: ksg97031
-Author-email: ksg97031@gmail.com
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-
-frida-gadget
-============
-
-|Codacy-Grade| |Docker| |Libraries-Rank|
-
-
-| ``frida-gadget`` is a tool that can be used to patch APKs in order to utilize the `Frida gadget <https://frida.re/docs/gadget/>`_.
-
-Installation
-------------
-
-|Py-Versions| |PyPI-Downloads| |Libraries-Dependents|
-
-.. code:: sh
-
-    pip install frida-gadget
-    
-Prerequirement
-----------------
-
-| You should install Apktool and add it to your PATH environment variable.
-|   
-
-.. code:: sh
-
-   # Install Apktool on macOS
-   brew install apktool
-    
-   # Add Apktool to your PATH environment variable
-   export PATH=$PATH:$HOME/.brew/bin 
-
-| Other Platforms: `Install Guide <https://ibotpeaches.github.io/Apktool/install/>`_
-
-Usage
-------------
-
-.. code:: sh
-
-    $ frida-gadget --help
-      Usage: frida-gadget [OPTIONS] APK_PATH
-
-      Options:
-        --arch TEXT  Support [arm, arm64, x86]
-        --help       Show this message and exit.
-
-Example
-~~~~~~~
-.. code:: sh
-
-    $ frida-gadget handtrackinggpu.apk --arch arm64
-      [INFO] Auto-detected frida version: 16.1.3
-      [INFO] APK: '[REDACTED]\frida-gadget\tests\demo-apk\handtrackinggpu.apk'
-      [INFO] Gadget Architecture(--arch): arm64(default)
-      [DEBUG] Decompiling the target APK using apktool
-      [DEBUG] Downloading the frida gadget library for arm64
-      [DEBUG] Checking internet permission and extractNativeLibs settings
-      [DEBUG] Adding 'android.permission.INTERNET' permission to AndroidManifest.xml
-      [DEBUG] Searching for the main activity in the smali files
-      [DEBUG] Found the main activity at '[REDACTED]\frida-gadget\tests\demo-apk\handtrackinggpu\smali\com\google\mediapipe\apps\handtrackinggpu\MainActivity.smali'
-      [DEBUG] Locating the onCreate method and injecting the loadLibrary code
-      [DEBUG] Recompiling the new APK using apktool
-      [INFO] Success!
-
-      [INFO] Output: [REDACTED]\frida-gadget\tests\demo-apk\handtrackinggpu\dist\handtrackinggpu.apk
-      
-    $ unzip -l handtrackinggpu.apk | grep libfrida-gadget
-      21133848  09-15-2021 02:28   lib/arm64-v8a/libfrida-gadget-16.1.3-android-arm64.so 
-       
-loadLibrary code will be injected
-********************************************
-
-.. image:: https://github.com/ksg97031/frida-gadget/blob/trunk/images/decompile.png
-   :width: 600
-
-Easy to re-sign your app by ``apk-signer``
-********************************************
-
-.. code:: sh
-
-    $ apk-signer handtrackinggpu.apk
-      [Warning] Signing with default keystore.
-      [Warning] Please pass --key_path, --key_alias, --key_pass, --ks_pass parameter, if you want to use your keystore
-      handtrackinggpu-signed.apk
-     
-    $ adb install handtrackinggpu-signed.apk
-   
-   
-Similar Projects
------------------
-| https://github.com/sensepost/objection
-| https://github.com/NickstaDB/patch-apk
-
-
-.. |Coverage-Status| image:: https://img.shields.io/coveralls/github/ksg97031/frida-gadget/master?logo=coveralls
-   :target: https://coveralls.io/github/ksg97031/frida-gadget
-.. |Branch-Coverage-Status| image:: https://codecov.io/gh/ksg97031/frida-gadget/branch/master/graph/badge.svg
-   :target: https://codecov.io/gh/ksg97031/frida-gadget
-.. |Codacy-Grade| image:: https://app.codacy.com/project/badge/Grade/3f965571598f44549c7818f29cdcf177
-   :target: https://www.codacy.com/gh/ksg97031/frida-gadget/dashboard
-.. |CII Best Practices| image:: https://bestpractices.coreinfrastructure.org/projects/3264/badge
-   :target: https://bestpractices.coreinfrastructure.org/projects/3264
-.. |GitHub-Status| image:: https://img.shields.io/github/tag/ksg97031/frida-gadget.svg?maxAge=86400&logo=github&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/releases
-.. |GitHub-Forks| image:: https://img.shields.io/github/forks/ksg97031/frida-gadget.svg?logo=github&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/network
-.. |GitHub-Stars| image:: https://img.shields.io/github/stars/ksg97031/frida-gadget.svg?logo=github&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/stargazers
-.. |GitHub-Commits| image:: https://img.shields.io/github/commit-activity/y/ksg97031/frida-gadget.svg?logo=git&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/graphs/commit-activity
-.. |GitHub-Issues| image:: https://img.shields.io/github/issues-closed/ksg97031/frida-gadget.svg?logo=github&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/issues?q=
-.. |GitHub-PRs| image:: https://img.shields.io/github/issues-pr-closed/ksg97031/frida-gadget.svg?logo=github&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/pulls
-.. |GitHub-Contributions| image:: https://img.shields.io/github/contributors/ksg97031/frida-gadget.svg?logo=github&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/graphs/contributors
-.. |GitHub-Updated| image:: https://img.shields.io/github/last-commit/ksg97031/frida-gadget/master.svg?logo=github&logoColor=white&label=pushed
-   :target: https://github.com/ksg97031/frida-gadget/pulse
-.. |Gift-Casper| image:: https://img.shields.io/badge/dynamic/json.svg?color=ff69b4&label=gifts%20received&prefix=%C2%A3&query=%24..sum&url=https%3A%2F%2Fcaspersci.uk.to%2Fgifts.json
-   :target: https://cdcl.ml/sponsor
-.. |PyPI-Downloads| image:: https://static.pepy.tech/badge/frida-gadget
-   :target: https://pepy.tech/project/frida-gadget
-.. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/frida-gadget
-   :target: https://pypi.org/project/frida-gadget
-.. |Conda-Forge-Status| image:: https://img.shields.io/conda/v/conda-forge/frida-gadget.svg?label=conda-forge&logo=conda-forge
-   :target: https://anaconda.org/conda-forge/frida-gadget
-.. |Docker| image:: https://img.shields.io/badge/docker-pull-blue.svg?logo=docker&logoColor=white
-   :target: https://hub.docker.com/r/ksg97031/frida-gadget
-.. |Libraries-Rank| image:: https://img.shields.io/librariesio/sourcerank/pypi/frida-gadget.svg?logo=koding&logoColor=white
-   :target: https://libraries.io/pypi/frida-gadget
-.. |Libraries-Dependents| image:: https://img.shields.io/librariesio/dependent-repos/pypi/frida-gadget.svg?logo=koding&logoColor=white
-    :target: https://github.com/ksg97031/frida-gadget/network/dependents
-.. |OpenHub-Status| image:: https://www.openhub.net/p/frida-gadget/widgets/project_thin_badge?format=gif
-   :target: https://www.openhub.net/p/frida-gadget?ref=Thin+badge
-.. |awesome-python| image:: https://awesome.re/mentioned-badge.svg
-   :target: https://github.com/vinta/awesome-python
-.. |LICENCE| image:: https://img.shields.io/pypi/l/frida-gadget.svg
-   :target: https://raw.githubusercontent.com/ksg97031/frida-gadget/master/LICENCE
-.. |DOI| image:: https://img.shields.io/badge/DOI-10.5281/zenodo.595120-blue.svg
-   :target: https://doi.org/10.5281/zenodo.595120
-.. |binder-demo| image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/ksg97031/frida-gadget/master?filepath=DEMO.ipynb
+Metadata-Version: 2.1
+Name: frida-gadget
+Version: 1.2.0
+Summary: Frida gadget into an APK
+Home-page: https://github.com/ksg97031/frida-gadget
+Author: ksg97031
+Author-email: ksg97031@gmail.com
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
+
+frida-gadget
+============
+
+|Codacy-Grade| |Docker| |Libraries-Rank|
+
+
+| ``frida-gadget`` is a tool that can be used to patch APKs in order to utilize the `Frida gadget <https://frida.re/docs/gadget/>`_.
+| This tool automates the process of downloading the Frida gadget library and injecting the loadlibrary code into the main activity.
+
+Installation
+------------
+
+|Py-Versions| |PyPI-Downloads|
+
+.. code:: sh
+
+    pip install frida-gadget
+    
+Prerequirement
+----------------
+
+| You should install Apktool and add it to your PATH environment variable.
+|   
+
+.. code:: sh
+
+   # Install Apktool on macOS
+   brew install apktool
+    
+   # Add Apktool to your PATH environment variable
+   export PATH=$PATH:$HOME/.brew/bin 
+
+| Other Platforms: `Install Guide <https://ibotpeaches.github.io/Apktool/install/>`_
+
+Usage
+------------
+
+.. code:: sh
+
+    $ frida-gadget --help
+      Usage: frida-gadget [OPTIONS] APK_PATH
+
+         Patch an APK with the Frida gadget library
+
+         Args:     apk_path (str): Path of the target APK file     
+                   arch     (str): Target architecture of the device
+
+         Outputs:  Injected APK file
+
+      Options:
+         --arch TEXT       Support [arm, arm64, x86, x86_64]
+         --skip-decompile
+         --skip-recompile
+         --help            Show this message and exit.
+
+Example
+~~~~~~~
+.. code:: sh
+
+    $ frida-gadget handtrackinggpu.apk --arch arm64
+      [INFO] Auto-detected frida version: 16.1.3
+      [INFO] APK: '[REDACTED]\demo-apk\handtrackinggpu.apk'
+      [INFO] Gadget Architecture(--arch): arm64(default)
+      [DEBUG] Decompiling the target APK using apktool
+      [DEBUG] Downloading the frida gadget library for arm64
+      [DEBUG] Checking internet permission and extractNativeLibs settings
+      [DEBUG] Adding 'android.permission.INTERNET' permission to AndroidManifest.xml
+      [DEBUG] Searching for the main activity in the smali files
+      [DEBUG] Found the main activity at '[REDACTED]\frida-gadget\tests\demo-apk\handtrackinggpu\smali\com\google\mediapipe\apps\handtrackinggpu\MainActivity.smali'
+      [DEBUG] Locating the onCreate method and injecting the loadLibrary code
+      [DEBUG] Recompiling the new APK using apktool
+
+      [INFO] Success: [REDACTED]\demo-apk\handtrackinggpu\dist\handtrackinggpu.apk
+      
+    $ unzip -l handtrackinggpu.apk | grep libfrida-gadget
+      21133848  09-15-2021 02:28   lib/arm64-v8a/libfrida-gadget-16.1.3-android-arm64.so 
+       
+loadLibrary code will be injected
+********************************************
+
+.. image:: https://github.com/ksg97031/frida-gadget/blob/trunk/images/decompile.png
+   :width: 600
+
+Easy to re-sign your app by ``apk-signer``
+********************************************
+
+.. code:: sh
+
+    $ apk-signer handtrackinggpu.apk
+      [Warning] Signing with default keystore.
+      [Warning] Please pass --key_path, --key_alias, --key_pass, --ks_pass parameter, if you want to use your keystore
+      handtrackinggpu-signed.apk
+     
+    $ adb install handtrackinggpu-signed.apk
+   
+   
+Similar Projects
+-----------------
+| https://github.com/sensepost/objection
+| https://github.com/NickstaDB/patch-apk
+
+
+.. |Coverage-Status| image:: https://img.shields.io/coveralls/github/ksg97031/frida-gadget/master?logo=coveralls
+   :target: https://coveralls.io/github/ksg97031/frida-gadget
+.. |Branch-Coverage-Status| image:: https://codecov.io/gh/ksg97031/frida-gadget/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/ksg97031/frida-gadget
+.. |Codacy-Grade| image:: https://app.codacy.com/project/badge/Grade/3f965571598f44549c7818f29cdcf177
+   :target: https://www.codacy.com/gh/ksg97031/frida-gadget/dashboard
+.. |CII Best Practices| image:: https://bestpractices.coreinfrastructure.org/projects/3264/badge
+   :target: https://bestpractices.coreinfrastructure.org/projects/3264
+.. |GitHub-Status| image:: https://img.shields.io/github/tag/ksg97031/frida-gadget.svg?maxAge=86400&logo=github&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/releases
+.. |GitHub-Forks| image:: https://img.shields.io/github/forks/ksg97031/frida-gadget.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/network
+.. |GitHub-Stars| image:: https://img.shields.io/github/stars/ksg97031/frida-gadget.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/stargazers
+.. |GitHub-Commits| image:: https://img.shields.io/github/commit-activity/y/ksg97031/frida-gadget.svg?logo=git&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/graphs/commit-activity
+.. |GitHub-Issues| image:: https://img.shields.io/github/issues-closed/ksg97031/frida-gadget.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/issues?q=
+.. |GitHub-PRs| image:: https://img.shields.io/github/issues-pr-closed/ksg97031/frida-gadget.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/pulls
+.. |GitHub-Contributions| image:: https://img.shields.io/github/contributors/ksg97031/frida-gadget.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/graphs/contributors
+.. |GitHub-Updated| image:: https://img.shields.io/github/last-commit/ksg97031/frida-gadget/master.svg?logo=github&logoColor=white&label=pushed
+   :target: https://github.com/ksg97031/frida-gadget/pulse
+.. |Gift-Casper| image:: https://img.shields.io/badge/dynamic/json.svg?color=ff69b4&label=gifts%20received&prefix=%C2%A3&query=%24..sum&url=https%3A%2F%2Fcaspersci.uk.to%2Fgifts.json
+   :target: https://cdcl.ml/sponsor
+.. |PyPI-Downloads| image:: https://static.pepy.tech/badge/frida-gadget
+   :target: https://pepy.tech/project/frida-gadget
+.. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/frida-gadget
+   :target: https://pypi.org/project/frida-gadget
+.. |Conda-Forge-Status| image:: https://img.shields.io/conda/v/conda-forge/frida-gadget.svg?label=conda-forge&logo=conda-forge
+   :target: https://anaconda.org/conda-forge/frida-gadget
+.. |Docker| image:: https://img.shields.io/badge/docker-pull-blue.svg?logo=docker&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/pkgs/container/frida-gadget
+.. |Libraries-Rank| image:: https://img.shields.io/librariesio/sourcerank/pypi/frida-gadget.svg?logo=koding&logoColor=white
+   :target: https://libraries.io/pypi/frida-gadget
+.. |Libraries-Dependents| image:: https://img.shields.io/librariesio/dependent-repos/pypi/frida-gadget.svg?logo=koding&logoColor=white
+    :target: https://github.com/ksg97031/frida-gadget/network/dependents
+.. |OpenHub-Status| image:: https://www.openhub.net/p/frida-gadget/widgets/project_thin_badge?format=gif
+   :target: https://www.openhub.net/p/frida-gadget?ref=Thin+badge
+.. |awesome-python| image:: https://awesome.re/mentioned-badge.svg
+   :target: https://github.com/vinta/awesome-python
+.. |LICENCE| image:: https://img.shields.io/pypi/l/frida-gadget.svg
+   :target: https://raw.githubusercontent.com/ksg97031/frida-gadget/master/LICENCE
+.. |DOI| image:: https://img.shields.io/badge/DOI-10.5281/zenodo.595120-blue.svg
+   :target: https://doi.org/10.5281/zenodo.595120
+.. |binder-demo| image:: https://mybinder.org/badge_logo.svg
+   :target: https://mybinder.org/v2/gh/ksg97031/frida-gadget/master?filepath=DEMO.ipynb
```

### Comparing `frida-gadget-1.1.3/README.rst` & `frida-gadget-1.2.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,141 +1,150 @@
-frida-gadget
-============
-
-|Codacy-Grade| |Docker| |Libraries-Rank|
-
-
-| ``frida-gadget`` is a tool that can be used to patch APKs in order to utilize the `Frida gadget <https://frida.re/docs/gadget/>`_.
-
-Installation
-------------
-
-|Py-Versions| |PyPI-Downloads| |Libraries-Dependents|
-
-.. code:: sh
-
-    pip install frida-gadget
-    
-Prerequirement
-----------------
-
-| You should install Apktool and add it to your PATH environment variable.
-|   
-
-.. code:: sh
-
-   # Install Apktool on macOS
-   brew install apktool
-    
-   # Add Apktool to your PATH environment variable
-   export PATH=$PATH:$HOME/.brew/bin 
-
-| Other Platforms: `Install Guide <https://ibotpeaches.github.io/Apktool/install/>`_
-
-Usage
-------------
-
-.. code:: sh
-
-    $ frida-gadget --help
-      Usage: frida-gadget [OPTIONS] APK_PATH
-
-      Options:
-        --arch TEXT  Support [arm, arm64, x86]
-        --help       Show this message and exit.
-
-Example
-~~~~~~~
-.. code:: sh
-
-    $ frida-gadget handtrackinggpu.apk --arch arm64
-      [INFO] Auto-detected frida version: 16.1.3
-      [INFO] APK: '[REDACTED]\frida-gadget\tests\demo-apk\handtrackinggpu.apk'
-      [INFO] Gadget Architecture(--arch): arm64(default)
-      [DEBUG] Decompiling the target APK using apktool
-      [DEBUG] Downloading the frida gadget library for arm64
-      [DEBUG] Checking internet permission and extractNativeLibs settings
-      [DEBUG] Adding 'android.permission.INTERNET' permission to AndroidManifest.xml
-      [DEBUG] Searching for the main activity in the smali files
-      [DEBUG] Found the main activity at '[REDACTED]\frida-gadget\tests\demo-apk\handtrackinggpu\smali\com\google\mediapipe\apps\handtrackinggpu\MainActivity.smali'
-      [DEBUG] Locating the onCreate method and injecting the loadLibrary code
-      [DEBUG] Recompiling the new APK using apktool
-      [INFO] Success!
-
-      [INFO] Output: [REDACTED]\frida-gadget\tests\demo-apk\handtrackinggpu\dist\handtrackinggpu.apk
-      
-    $ unzip -l handtrackinggpu.apk | grep libfrida-gadget
-      21133848  09-15-2021 02:28   lib/arm64-v8a/libfrida-gadget-16.1.3-android-arm64.so 
-       
-loadLibrary code will be injected
-********************************************
-
-.. image:: https://github.com/ksg97031/frida-gadget/blob/trunk/images/decompile.png
-   :width: 600
-
-Easy to re-sign your app by ``apk-signer``
-********************************************
-
-.. code:: sh
-
-    $ apk-signer handtrackinggpu.apk
-      [Warning] Signing with default keystore.
-      [Warning] Please pass --key_path, --key_alias, --key_pass, --ks_pass parameter, if you want to use your keystore
-      handtrackinggpu-signed.apk
-     
-    $ adb install handtrackinggpu-signed.apk
-   
-   
-Similar Projects
------------------
-| https://github.com/sensepost/objection
-| https://github.com/NickstaDB/patch-apk
-
-
-.. |Coverage-Status| image:: https://img.shields.io/coveralls/github/ksg97031/frida-gadget/master?logo=coveralls
-   :target: https://coveralls.io/github/ksg97031/frida-gadget
-.. |Branch-Coverage-Status| image:: https://codecov.io/gh/ksg97031/frida-gadget/branch/master/graph/badge.svg
-   :target: https://codecov.io/gh/ksg97031/frida-gadget
-.. |Codacy-Grade| image:: https://app.codacy.com/project/badge/Grade/3f965571598f44549c7818f29cdcf177
-   :target: https://www.codacy.com/gh/ksg97031/frida-gadget/dashboard
-.. |CII Best Practices| image:: https://bestpractices.coreinfrastructure.org/projects/3264/badge
-   :target: https://bestpractices.coreinfrastructure.org/projects/3264
-.. |GitHub-Status| image:: https://img.shields.io/github/tag/ksg97031/frida-gadget.svg?maxAge=86400&logo=github&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/releases
-.. |GitHub-Forks| image:: https://img.shields.io/github/forks/ksg97031/frida-gadget.svg?logo=github&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/network
-.. |GitHub-Stars| image:: https://img.shields.io/github/stars/ksg97031/frida-gadget.svg?logo=github&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/stargazers
-.. |GitHub-Commits| image:: https://img.shields.io/github/commit-activity/y/ksg97031/frida-gadget.svg?logo=git&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/graphs/commit-activity
-.. |GitHub-Issues| image:: https://img.shields.io/github/issues-closed/ksg97031/frida-gadget.svg?logo=github&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/issues?q=
-.. |GitHub-PRs| image:: https://img.shields.io/github/issues-pr-closed/ksg97031/frida-gadget.svg?logo=github&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/pulls
-.. |GitHub-Contributions| image:: https://img.shields.io/github/contributors/ksg97031/frida-gadget.svg?logo=github&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/graphs/contributors
-.. |GitHub-Updated| image:: https://img.shields.io/github/last-commit/ksg97031/frida-gadget/master.svg?logo=github&logoColor=white&label=pushed
-   :target: https://github.com/ksg97031/frida-gadget/pulse
-.. |Gift-Casper| image:: https://img.shields.io/badge/dynamic/json.svg?color=ff69b4&label=gifts%20received&prefix=%C2%A3&query=%24..sum&url=https%3A%2F%2Fcaspersci.uk.to%2Fgifts.json
-   :target: https://cdcl.ml/sponsor
-.. |PyPI-Downloads| image:: https://static.pepy.tech/badge/frida-gadget
-   :target: https://pepy.tech/project/frida-gadget
-.. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/frida-gadget
-   :target: https://pypi.org/project/frida-gadget
-.. |Conda-Forge-Status| image:: https://img.shields.io/conda/v/conda-forge/frida-gadget.svg?label=conda-forge&logo=conda-forge
-   :target: https://anaconda.org/conda-forge/frida-gadget
-.. |Docker| image:: https://img.shields.io/badge/docker-pull-blue.svg?logo=docker&logoColor=white
-   :target: https://hub.docker.com/r/ksg97031/frida-gadget
-.. |Libraries-Rank| image:: https://img.shields.io/librariesio/sourcerank/pypi/frida-gadget.svg?logo=koding&logoColor=white
-   :target: https://libraries.io/pypi/frida-gadget
-.. |Libraries-Dependents| image:: https://img.shields.io/librariesio/dependent-repos/pypi/frida-gadget.svg?logo=koding&logoColor=white
-    :target: https://github.com/ksg97031/frida-gadget/network/dependents
-.. |OpenHub-Status| image:: https://www.openhub.net/p/frida-gadget/widgets/project_thin_badge?format=gif
-   :target: https://www.openhub.net/p/frida-gadget?ref=Thin+badge
-.. |awesome-python| image:: https://awesome.re/mentioned-badge.svg
-   :target: https://github.com/vinta/awesome-python
-.. |LICENCE| image:: https://img.shields.io/pypi/l/frida-gadget.svg
-   :target: https://raw.githubusercontent.com/ksg97031/frida-gadget/master/LICENCE
-.. |DOI| image:: https://img.shields.io/badge/DOI-10.5281/zenodo.595120-blue.svg
-   :target: https://doi.org/10.5281/zenodo.595120
-.. |binder-demo| image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/ksg97031/frida-gadget/master?filepath=DEMO.ipynb
+frida-gadget
+============
+
+|Codacy-Grade| |Docker| |Libraries-Rank|
+
+
+| ``frida-gadget`` is a tool that can be used to patch APKs in order to utilize the `Frida gadget <https://frida.re/docs/gadget/>`_.
+| This tool automates the process of downloading the Frida gadget library and injecting the loadlibrary code into the main activity.
+
+Installation
+------------
+
+|Py-Versions| |PyPI-Downloads|
+
+.. code:: sh
+
+    pip install frida-gadget
+    
+Prerequirement
+----------------
+
+| You should install Apktool and add it to your PATH environment variable.
+|   
+
+.. code:: sh
+
+   # Install Apktool on macOS
+   brew install apktool
+    
+   # Add Apktool to your PATH environment variable
+   export PATH=$PATH:$HOME/.brew/bin 
+
+| Other Platforms: `Install Guide <https://ibotpeaches.github.io/Apktool/install/>`_
+
+Usage
+------------
+
+.. code:: sh
+
+    $ frida-gadget --help
+      Usage: frida-gadget [OPTIONS] APK_PATH
+
+         Patch an APK with the Frida gadget library
+
+         Args:     apk_path (str): Path of the target APK file     
+                   arch     (str): Target architecture of the device
+
+         Outputs:  Injected APK file
+
+      Options:
+         --arch TEXT       Support [arm, arm64, x86, x86_64]
+         --skip-decompile
+         --skip-recompile
+         --help            Show this message and exit.
+
+Example
+~~~~~~~
+.. code:: sh
+
+    $ frida-gadget handtrackinggpu.apk --arch arm64
+      [INFO] Auto-detected frida version: 16.1.3
+      [INFO] APK: '[REDACTED]\demo-apk\handtrackinggpu.apk'
+      [INFO] Gadget Architecture(--arch): arm64(default)
+      [DEBUG] Decompiling the target APK using apktool
+      [DEBUG] Downloading the frida gadget library for arm64
+      [DEBUG] Checking internet permission and extractNativeLibs settings
+      [DEBUG] Adding 'android.permission.INTERNET' permission to AndroidManifest.xml
+      [DEBUG] Searching for the main activity in the smali files
+      [DEBUG] Found the main activity at '[REDACTED]\frida-gadget\tests\demo-apk\handtrackinggpu\smali\com\google\mediapipe\apps\handtrackinggpu\MainActivity.smali'
+      [DEBUG] Locating the onCreate method and injecting the loadLibrary code
+      [DEBUG] Recompiling the new APK using apktool
+
+      [INFO] Success: [REDACTED]\demo-apk\handtrackinggpu\dist\handtrackinggpu.apk
+      
+    $ unzip -l handtrackinggpu.apk | grep libfrida-gadget
+      21133848  09-15-2021 02:28   lib/arm64-v8a/libfrida-gadget-16.1.3-android-arm64.so 
+       
+loadLibrary code will be injected
+********************************************
+
+.. image:: https://github.com/ksg97031/frida-gadget/blob/trunk/images/decompile.png
+   :width: 600
+
+Easy to re-sign your app by ``apk-signer``
+********************************************
+
+.. code:: sh
+
+    $ apk-signer handtrackinggpu.apk
+      [Warning] Signing with default keystore.
+      [Warning] Please pass --key_path, --key_alias, --key_pass, --ks_pass parameter, if you want to use your keystore
+      handtrackinggpu-signed.apk
+     
+    $ adb install handtrackinggpu-signed.apk
+   
+   
+Similar Projects
+-----------------
+| https://github.com/sensepost/objection
+| https://github.com/NickstaDB/patch-apk
+
+
+.. |Coverage-Status| image:: https://img.shields.io/coveralls/github/ksg97031/frida-gadget/master?logo=coveralls
+   :target: https://coveralls.io/github/ksg97031/frida-gadget
+.. |Branch-Coverage-Status| image:: https://codecov.io/gh/ksg97031/frida-gadget/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/ksg97031/frida-gadget
+.. |Codacy-Grade| image:: https://app.codacy.com/project/badge/Grade/3f965571598f44549c7818f29cdcf177
+   :target: https://www.codacy.com/gh/ksg97031/frida-gadget/dashboard
+.. |CII Best Practices| image:: https://bestpractices.coreinfrastructure.org/projects/3264/badge
+   :target: https://bestpractices.coreinfrastructure.org/projects/3264
+.. |GitHub-Status| image:: https://img.shields.io/github/tag/ksg97031/frida-gadget.svg?maxAge=86400&logo=github&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/releases
+.. |GitHub-Forks| image:: https://img.shields.io/github/forks/ksg97031/frida-gadget.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/network
+.. |GitHub-Stars| image:: https://img.shields.io/github/stars/ksg97031/frida-gadget.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/stargazers
+.. |GitHub-Commits| image:: https://img.shields.io/github/commit-activity/y/ksg97031/frida-gadget.svg?logo=git&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/graphs/commit-activity
+.. |GitHub-Issues| image:: https://img.shields.io/github/issues-closed/ksg97031/frida-gadget.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/issues?q=
+.. |GitHub-PRs| image:: https://img.shields.io/github/issues-pr-closed/ksg97031/frida-gadget.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/pulls
+.. |GitHub-Contributions| image:: https://img.shields.io/github/contributors/ksg97031/frida-gadget.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/graphs/contributors
+.. |GitHub-Updated| image:: https://img.shields.io/github/last-commit/ksg97031/frida-gadget/master.svg?logo=github&logoColor=white&label=pushed
+   :target: https://github.com/ksg97031/frida-gadget/pulse
+.. |Gift-Casper| image:: https://img.shields.io/badge/dynamic/json.svg?color=ff69b4&label=gifts%20received&prefix=%C2%A3&query=%24..sum&url=https%3A%2F%2Fcaspersci.uk.to%2Fgifts.json
+   :target: https://cdcl.ml/sponsor
+.. |PyPI-Downloads| image:: https://static.pepy.tech/badge/frida-gadget
+   :target: https://pepy.tech/project/frida-gadget
+.. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/frida-gadget
+   :target: https://pypi.org/project/frida-gadget
+.. |Conda-Forge-Status| image:: https://img.shields.io/conda/v/conda-forge/frida-gadget.svg?label=conda-forge&logo=conda-forge
+   :target: https://anaconda.org/conda-forge/frida-gadget
+.. |Docker| image:: https://img.shields.io/badge/docker-pull-blue.svg?logo=docker&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/pkgs/container/frida-gadget
+.. |Libraries-Rank| image:: https://img.shields.io/librariesio/sourcerank/pypi/frida-gadget.svg?logo=koding&logoColor=white
+   :target: https://libraries.io/pypi/frida-gadget
+.. |Libraries-Dependents| image:: https://img.shields.io/librariesio/dependent-repos/pypi/frida-gadget.svg?logo=koding&logoColor=white
+    :target: https://github.com/ksg97031/frida-gadget/network/dependents
+.. |OpenHub-Status| image:: https://www.openhub.net/p/frida-gadget/widgets/project_thin_badge?format=gif
+   :target: https://www.openhub.net/p/frida-gadget?ref=Thin+badge
+.. |awesome-python| image:: https://awesome.re/mentioned-badge.svg
+   :target: https://github.com/vinta/awesome-python
+.. |LICENCE| image:: https://img.shields.io/pypi/l/frida-gadget.svg
+   :target: https://raw.githubusercontent.com/ksg97031/frida-gadget/master/LICENCE
+.. |DOI| image:: https://img.shields.io/badge/DOI-10.5281/zenodo.595120-blue.svg
+   :target: https://doi.org/10.5281/zenodo.595120
+.. |binder-demo| image:: https://mybinder.org/badge_logo.svg
+   :target: https://mybinder.org/v2/gh/ksg97031/frida-gadget/master?filepath=DEMO.ipynb
```

### Comparing `frida-gadget-1.1.3/frida_gadget.egg-info/PKG-INFO` & `frida-gadget-1.2.0/frida_gadget.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,159 +1,168 @@
-Metadata-Version: 2.1
-Name: frida-gadget
-Version: 1.1.3
-Summary: Frida gadget into an APK
-Home-page: https://github.com/ksg97031/frida-gadget
-Author: ksg97031
-Author-email: ksg97031@gmail.com
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-
-frida-gadget
-============
-
-|Codacy-Grade| |Docker| |Libraries-Rank|
-
-
-| ``frida-gadget`` is a tool that can be used to patch APKs in order to utilize the `Frida gadget <https://frida.re/docs/gadget/>`_.
-
-Installation
-------------
-
-|Py-Versions| |PyPI-Downloads| |Libraries-Dependents|
-
-.. code:: sh
-
-    pip install frida-gadget
-    
-Prerequirement
-----------------
-
-| You should install Apktool and add it to your PATH environment variable.
-|   
-
-.. code:: sh
-
-   # Install Apktool on macOS
-   brew install apktool
-    
-   # Add Apktool to your PATH environment variable
-   export PATH=$PATH:$HOME/.brew/bin 
-
-| Other Platforms: `Install Guide <https://ibotpeaches.github.io/Apktool/install/>`_
-
-Usage
-------------
-
-.. code:: sh
-
-    $ frida-gadget --help
-      Usage: frida-gadget [OPTIONS] APK_PATH
-
-      Options:
-        --arch TEXT  Support [arm, arm64, x86]
-        --help       Show this message and exit.
-
-Example
-~~~~~~~
-.. code:: sh
-
-    $ frida-gadget handtrackinggpu.apk --arch arm64
-      [INFO] Auto-detected frida version: 16.1.3
-      [INFO] APK: '[REDACTED]\frida-gadget\tests\demo-apk\handtrackinggpu.apk'
-      [INFO] Gadget Architecture(--arch): arm64(default)
-      [DEBUG] Decompiling the target APK using apktool
-      [DEBUG] Downloading the frida gadget library for arm64
-      [DEBUG] Checking internet permission and extractNativeLibs settings
-      [DEBUG] Adding 'android.permission.INTERNET' permission to AndroidManifest.xml
-      [DEBUG] Searching for the main activity in the smali files
-      [DEBUG] Found the main activity at '[REDACTED]\frida-gadget\tests\demo-apk\handtrackinggpu\smali\com\google\mediapipe\apps\handtrackinggpu\MainActivity.smali'
-      [DEBUG] Locating the onCreate method and injecting the loadLibrary code
-      [DEBUG] Recompiling the new APK using apktool
-      [INFO] Success!
-
-      [INFO] Output: [REDACTED]\frida-gadget\tests\demo-apk\handtrackinggpu\dist\handtrackinggpu.apk
-      
-    $ unzip -l handtrackinggpu.apk | grep libfrida-gadget
-      21133848  09-15-2021 02:28   lib/arm64-v8a/libfrida-gadget-16.1.3-android-arm64.so 
-       
-loadLibrary code will be injected
-********************************************
-
-.. image:: https://github.com/ksg97031/frida-gadget/blob/trunk/images/decompile.png
-   :width: 600
-
-Easy to re-sign your app by ``apk-signer``
-********************************************
-
-.. code:: sh
-
-    $ apk-signer handtrackinggpu.apk
-      [Warning] Signing with default keystore.
-      [Warning] Please pass --key_path, --key_alias, --key_pass, --ks_pass parameter, if you want to use your keystore
-      handtrackinggpu-signed.apk
-     
-    $ adb install handtrackinggpu-signed.apk
-   
-   
-Similar Projects
------------------
-| https://github.com/sensepost/objection
-| https://github.com/NickstaDB/patch-apk
-
-
-.. |Coverage-Status| image:: https://img.shields.io/coveralls/github/ksg97031/frida-gadget/master?logo=coveralls
-   :target: https://coveralls.io/github/ksg97031/frida-gadget
-.. |Branch-Coverage-Status| image:: https://codecov.io/gh/ksg97031/frida-gadget/branch/master/graph/badge.svg
-   :target: https://codecov.io/gh/ksg97031/frida-gadget
-.. |Codacy-Grade| image:: https://app.codacy.com/project/badge/Grade/3f965571598f44549c7818f29cdcf177
-   :target: https://www.codacy.com/gh/ksg97031/frida-gadget/dashboard
-.. |CII Best Practices| image:: https://bestpractices.coreinfrastructure.org/projects/3264/badge
-   :target: https://bestpractices.coreinfrastructure.org/projects/3264
-.. |GitHub-Status| image:: https://img.shields.io/github/tag/ksg97031/frida-gadget.svg?maxAge=86400&logo=github&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/releases
-.. |GitHub-Forks| image:: https://img.shields.io/github/forks/ksg97031/frida-gadget.svg?logo=github&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/network
-.. |GitHub-Stars| image:: https://img.shields.io/github/stars/ksg97031/frida-gadget.svg?logo=github&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/stargazers
-.. |GitHub-Commits| image:: https://img.shields.io/github/commit-activity/y/ksg97031/frida-gadget.svg?logo=git&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/graphs/commit-activity
-.. |GitHub-Issues| image:: https://img.shields.io/github/issues-closed/ksg97031/frida-gadget.svg?logo=github&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/issues?q=
-.. |GitHub-PRs| image:: https://img.shields.io/github/issues-pr-closed/ksg97031/frida-gadget.svg?logo=github&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/pulls
-.. |GitHub-Contributions| image:: https://img.shields.io/github/contributors/ksg97031/frida-gadget.svg?logo=github&logoColor=white
-   :target: https://github.com/ksg97031/frida-gadget/graphs/contributors
-.. |GitHub-Updated| image:: https://img.shields.io/github/last-commit/ksg97031/frida-gadget/master.svg?logo=github&logoColor=white&label=pushed
-   :target: https://github.com/ksg97031/frida-gadget/pulse
-.. |Gift-Casper| image:: https://img.shields.io/badge/dynamic/json.svg?color=ff69b4&label=gifts%20received&prefix=%C2%A3&query=%24..sum&url=https%3A%2F%2Fcaspersci.uk.to%2Fgifts.json
-   :target: https://cdcl.ml/sponsor
-.. |PyPI-Downloads| image:: https://static.pepy.tech/badge/frida-gadget
-   :target: https://pepy.tech/project/frida-gadget
-.. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/frida-gadget
-   :target: https://pypi.org/project/frida-gadget
-.. |Conda-Forge-Status| image:: https://img.shields.io/conda/v/conda-forge/frida-gadget.svg?label=conda-forge&logo=conda-forge
-   :target: https://anaconda.org/conda-forge/frida-gadget
-.. |Docker| image:: https://img.shields.io/badge/docker-pull-blue.svg?logo=docker&logoColor=white
-   :target: https://hub.docker.com/r/ksg97031/frida-gadget
-.. |Libraries-Rank| image:: https://img.shields.io/librariesio/sourcerank/pypi/frida-gadget.svg?logo=koding&logoColor=white
-   :target: https://libraries.io/pypi/frida-gadget
-.. |Libraries-Dependents| image:: https://img.shields.io/librariesio/dependent-repos/pypi/frida-gadget.svg?logo=koding&logoColor=white
-    :target: https://github.com/ksg97031/frida-gadget/network/dependents
-.. |OpenHub-Status| image:: https://www.openhub.net/p/frida-gadget/widgets/project_thin_badge?format=gif
-   :target: https://www.openhub.net/p/frida-gadget?ref=Thin+badge
-.. |awesome-python| image:: https://awesome.re/mentioned-badge.svg
-   :target: https://github.com/vinta/awesome-python
-.. |LICENCE| image:: https://img.shields.io/pypi/l/frida-gadget.svg
-   :target: https://raw.githubusercontent.com/ksg97031/frida-gadget/master/LICENCE
-.. |DOI| image:: https://img.shields.io/badge/DOI-10.5281/zenodo.595120-blue.svg
-   :target: https://doi.org/10.5281/zenodo.595120
-.. |binder-demo| image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/ksg97031/frida-gadget/master?filepath=DEMO.ipynb
+Metadata-Version: 2.1
+Name: frida-gadget
+Version: 1.2.0
+Summary: Frida gadget into an APK
+Home-page: https://github.com/ksg97031/frida-gadget
+Author: ksg97031
+Author-email: ksg97031@gmail.com
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
+
+frida-gadget
+============
+
+|Codacy-Grade| |Docker| |Libraries-Rank|
+
+
+| ``frida-gadget`` is a tool that can be used to patch APKs in order to utilize the `Frida gadget <https://frida.re/docs/gadget/>`_.
+| This tool automates the process of downloading the Frida gadget library and injecting the loadlibrary code into the main activity.
+
+Installation
+------------
+
+|Py-Versions| |PyPI-Downloads|
+
+.. code:: sh
+
+    pip install frida-gadget
+    
+Prerequirement
+----------------
+
+| You should install Apktool and add it to your PATH environment variable.
+|   
+
+.. code:: sh
+
+   # Install Apktool on macOS
+   brew install apktool
+    
+   # Add Apktool to your PATH environment variable
+   export PATH=$PATH:$HOME/.brew/bin 
+
+| Other Platforms: `Install Guide <https://ibotpeaches.github.io/Apktool/install/>`_
+
+Usage
+------------
+
+.. code:: sh
+
+    $ frida-gadget --help
+      Usage: frida-gadget [OPTIONS] APK_PATH
+
+         Patch an APK with the Frida gadget library
+
+         Args:     apk_path (str): Path of the target APK file     
+                   arch     (str): Target architecture of the device
+
+         Outputs:  Injected APK file
+
+      Options:
+         --arch TEXT       Support [arm, arm64, x86, x86_64]
+         --skip-decompile
+         --skip-recompile
+         --help            Show this message and exit.
+
+Example
+~~~~~~~
+.. code:: sh
+
+    $ frida-gadget handtrackinggpu.apk --arch arm64
+      [INFO] Auto-detected frida version: 16.1.3
+      [INFO] APK: '[REDACTED]\demo-apk\handtrackinggpu.apk'
+      [INFO] Gadget Architecture(--arch): arm64(default)
+      [DEBUG] Decompiling the target APK using apktool
+      [DEBUG] Downloading the frida gadget library for arm64
+      [DEBUG] Checking internet permission and extractNativeLibs settings
+      [DEBUG] Adding 'android.permission.INTERNET' permission to AndroidManifest.xml
+      [DEBUG] Searching for the main activity in the smali files
+      [DEBUG] Found the main activity at '[REDACTED]\frida-gadget\tests\demo-apk\handtrackinggpu\smali\com\google\mediapipe\apps\handtrackinggpu\MainActivity.smali'
+      [DEBUG] Locating the onCreate method and injecting the loadLibrary code
+      [DEBUG] Recompiling the new APK using apktool
+
+      [INFO] Success: [REDACTED]\demo-apk\handtrackinggpu\dist\handtrackinggpu.apk
+      
+    $ unzip -l handtrackinggpu.apk | grep libfrida-gadget
+      21133848  09-15-2021 02:28   lib/arm64-v8a/libfrida-gadget-16.1.3-android-arm64.so 
+       
+loadLibrary code will be injected
+********************************************
+
+.. image:: https://github.com/ksg97031/frida-gadget/blob/trunk/images/decompile.png
+   :width: 600
+
+Easy to re-sign your app by ``apk-signer``
+********************************************
+
+.. code:: sh
+
+    $ apk-signer handtrackinggpu.apk
+      [Warning] Signing with default keystore.
+      [Warning] Please pass --key_path, --key_alias, --key_pass, --ks_pass parameter, if you want to use your keystore
+      handtrackinggpu-signed.apk
+     
+    $ adb install handtrackinggpu-signed.apk
+   
+   
+Similar Projects
+-----------------
+| https://github.com/sensepost/objection
+| https://github.com/NickstaDB/patch-apk
+
+
+.. |Coverage-Status| image:: https://img.shields.io/coveralls/github/ksg97031/frida-gadget/master?logo=coveralls
+   :target: https://coveralls.io/github/ksg97031/frida-gadget
+.. |Branch-Coverage-Status| image:: https://codecov.io/gh/ksg97031/frida-gadget/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/ksg97031/frida-gadget
+.. |Codacy-Grade| image:: https://app.codacy.com/project/badge/Grade/3f965571598f44549c7818f29cdcf177
+   :target: https://www.codacy.com/gh/ksg97031/frida-gadget/dashboard
+.. |CII Best Practices| image:: https://bestpractices.coreinfrastructure.org/projects/3264/badge
+   :target: https://bestpractices.coreinfrastructure.org/projects/3264
+.. |GitHub-Status| image:: https://img.shields.io/github/tag/ksg97031/frida-gadget.svg?maxAge=86400&logo=github&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/releases
+.. |GitHub-Forks| image:: https://img.shields.io/github/forks/ksg97031/frida-gadget.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/network
+.. |GitHub-Stars| image:: https://img.shields.io/github/stars/ksg97031/frida-gadget.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/stargazers
+.. |GitHub-Commits| image:: https://img.shields.io/github/commit-activity/y/ksg97031/frida-gadget.svg?logo=git&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/graphs/commit-activity
+.. |GitHub-Issues| image:: https://img.shields.io/github/issues-closed/ksg97031/frida-gadget.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/issues?q=
+.. |GitHub-PRs| image:: https://img.shields.io/github/issues-pr-closed/ksg97031/frida-gadget.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/pulls
+.. |GitHub-Contributions| image:: https://img.shields.io/github/contributors/ksg97031/frida-gadget.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/graphs/contributors
+.. |GitHub-Updated| image:: https://img.shields.io/github/last-commit/ksg97031/frida-gadget/master.svg?logo=github&logoColor=white&label=pushed
+   :target: https://github.com/ksg97031/frida-gadget/pulse
+.. |Gift-Casper| image:: https://img.shields.io/badge/dynamic/json.svg?color=ff69b4&label=gifts%20received&prefix=%C2%A3&query=%24..sum&url=https%3A%2F%2Fcaspersci.uk.to%2Fgifts.json
+   :target: https://cdcl.ml/sponsor
+.. |PyPI-Downloads| image:: https://static.pepy.tech/badge/frida-gadget
+   :target: https://pepy.tech/project/frida-gadget
+.. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/frida-gadget
+   :target: https://pypi.org/project/frida-gadget
+.. |Conda-Forge-Status| image:: https://img.shields.io/conda/v/conda-forge/frida-gadget.svg?label=conda-forge&logo=conda-forge
+   :target: https://anaconda.org/conda-forge/frida-gadget
+.. |Docker| image:: https://img.shields.io/badge/docker-pull-blue.svg?logo=docker&logoColor=white
+   :target: https://github.com/ksg97031/frida-gadget/pkgs/container/frida-gadget
+.. |Libraries-Rank| image:: https://img.shields.io/librariesio/sourcerank/pypi/frida-gadget.svg?logo=koding&logoColor=white
+   :target: https://libraries.io/pypi/frida-gadget
+.. |Libraries-Dependents| image:: https://img.shields.io/librariesio/dependent-repos/pypi/frida-gadget.svg?logo=koding&logoColor=white
+    :target: https://github.com/ksg97031/frida-gadget/network/dependents
+.. |OpenHub-Status| image:: https://www.openhub.net/p/frida-gadget/widgets/project_thin_badge?format=gif
+   :target: https://www.openhub.net/p/frida-gadget?ref=Thin+badge
+.. |awesome-python| image:: https://awesome.re/mentioned-badge.svg
+   :target: https://github.com/vinta/awesome-python
+.. |LICENCE| image:: https://img.shields.io/pypi/l/frida-gadget.svg
+   :target: https://raw.githubusercontent.com/ksg97031/frida-gadget/master/LICENCE
+.. |DOI| image:: https://img.shields.io/badge/DOI-10.5281/zenodo.595120-blue.svg
+   :target: https://doi.org/10.5281/zenodo.595120
+.. |binder-demo| image:: https://mybinder.org/badge_logo.svg
+   :target: https://mybinder.org/v2/gh/ksg97031/frida-gadget/master?filepath=DEMO.ipynb
```

### Comparing `frida-gadget-1.1.3/scripts/__init__.py` & `frida-gadget-1.2.0/scripts/__init__.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-"""init file for scripts folder."""
-import sys
-import subprocess
-from .logger import logger
-
-
-def import_or_install(package):
-    """Function to install missing packages.
-
-    Args:
-        package (string): Name of the package to install.
-    """
-    try:
-        __import__(package)
-    except ImportError:
-        subprocess.check_call([sys.executable, '-m', 'pip', 'install', 'frida', '--user'])
-        logger.info('Try Again')
-        sys.exit(0)
-
-
-import_or_install('frida')  # Install missing packages
-INSTALLED_FRIDA_VERSION: str = __import__('frida').__version__  # Get installed frida version
-logger.info("Auto-detected frida version: %s", INSTALLED_FRIDA_VERSION)
+"""init file for scripts folder."""
+import sys
+import subprocess
+from .logger import logger
+
+
+def import_or_install(package):
+    """Function to install missing packages.
+
+    Args:
+        package (string): Name of the package to install.
+    """
+    try:
+        __import__(package)
+    except ImportError:
+        subprocess.check_call([sys.executable, '-m', 'pip', 'install', 'frida', '--user'])
+        logger.info('Try Again')
+        sys.exit(0)
+
+
+import_or_install('frida')  # Install missing packages
+INSTALLED_FRIDA_VERSION: str = __import__('frida').__version__  # Get installed frida version
+logger.info("Auto-detected frida version: %s", INSTALLED_FRIDA_VERSION)
```

### Comparing `frida-gadget-1.1.3/scripts/cli.py` & `frida-gadget-1.2.0/scripts/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,245 +1,258 @@
-"""Frida gadget injector for Android APK"""
-import os
-import sys
-import shutil
-import subprocess
-from shutil import which
-from pathlib import Path
-import click
-from androguard.core.bytecodes.apk import APK
-from .logger import logger
-from .frida_github import FridaGithub
-from . import INSTALLED_FRIDA_VERSION
-
-
-p = Path(__file__)
-ROOT_DIR = p.parent.resolve()
-TEMP_DIR = ROOT_DIR.joinpath('temp')
-FILE_DIR = ROOT_DIR.joinpath('files')
-
-APKTOOL = which("apktool")
-if not APKTOOL:
-    raise FileNotFoundError(
-        "Please download the 'apktool' and set it to your PATH environment.")
-
-def run_apktool(option, apk_path: str):
-    """Run apktool with option
-
-    Args:
-        option (list|str): option of apktool
-        apk_path (str): path of apk file
-
-    """
-    if isinstance(option, list):
-        cmd = [APKTOOL] + option + [apk_path]
-    else:
-        cmd = [APKTOOL, option, apk_path]
-
-    pipe = subprocess.PIPE
-    with subprocess.Popen(cmd, stdin=pipe, stdout=pipe, stderr=pipe) as process:
-        _, stderr = process.communicate(b"\n")
-        if process.returncode != 0:
-            raise subprocess.CalledProcessError(process.returncode, cmd, stderr)
-        return True
-
-def download_gadget(arch: str):
-    """Download the frida gadget library
-
-    Args:
-        arch (str): architecture of the device
-    """
-    frida_github = FridaGithub(INSTALLED_FRIDA_VERSION)
-    assets = frida_github.get_assets()
-    file = f'frida-gadget-{INSTALLED_FRIDA_VERSION}-android-{arch}.so.xz'
-    for asset in assets:
-        if asset['name'] == file:
-            logger.debug("Downloading the frida gadget library for %s", arch)
-            so_gadget_path = str(FILE_DIR.joinpath(file[:-3]))
-            return frida_github.download_gadget_so(asset['browser_download_url'], so_gadget_path)
-
-    raise FileNotFoundError(f"'{file}' not found in the github releases")
-
-def insert_loadlibary(decompiled_path, main_activity, load_library_name):
-    """Inject loadlibary code to main activity
-
-    Args:
-        text (str): smali code of the main activity
-    """
-    logger.debug('Searching for the main activity in the smali files')
-    target_smali = None
-    
-    target_relative_path = main_activity.replace(".", os.sep)
-    target_smali = decompiled_path.joinpath("smali", target_relative_path + ".smali")
-    if not target_smali or not target_smali.exists():
-        raise FileNotFoundError(f"The target class file {target_smali} was not found.")
-
-    logger.debug("Found the main activity at '%s'", str(target_smali))
-    text = target_smali.read_text()
-
-    text = text.replace(
-        "invoke-virtual {v0, v1}, Ljava/lang/Runtime;->exit(I)V", "")
-    text = text.split("\n")
-
-    # Find onCreate method and inject loadLibary code for frida gadget
-    logger.debug(
-        'Locating the onCreate method and injecting the loadLibrary code')
-    idx = 0
-    status = False
-    while idx != len(text):
-        line = text[idx].strip()
-        if line.startswith('.method') and "onCreate(" in line:
-            locals_line_bit = text[idx + 1].split(".locals ")
-            locals_variable_count = int(locals_line_bit[1])
-            locals_line_bit[1] = str(locals_variable_count + 1)
-            if load_library_name.startswith('lib'):
-                load_library_name = load_library_name[3:]
-
-            new_locals_line = ".locals ".join(locals_line_bit)
-            text[idx + 1] = new_locals_line
-
-            load_str = f'    const-string v{locals_variable_count}, "{load_library_name}"'
-            load_library = f'    invoke-static {{v{locals_variable_count}}}, \
-                Ljava/lang/System;->loadLibrary(Ljava/lang/String;)V'
-            text.insert(idx + 2, load_library)
-            text.insert(idx + 2, load_str)
-            status = True
-            break
-        idx += 1
-
-    if not status:
-        issue_url = 'https://github.com/ksg97031/frida-gadget/issues'
-        logger.error(
-            "Cannot find the onCreate method in the main activity.")
-        logger.error(
-            "Please report the issue at %s with the following information:", issue_url)
-        logger.error("APK Name: <Your APK Name>")
-        logger.error("APK Version: <Your APK Version>")
-        logger.error("Device/Emulator OS: <Your Device/Emulator OS>")
-        logger.error("Frida Version: <Your Frida Version>")
-        sys.exit(-1)
-
-    # Replace the smali file with the new one
-    target_smali.write_text("\n".join(text))
-
-def modify_manifest(decompiled_path):
-    """Modify manifest permssions
-
-    Args:
-        decompiled_path (str): decomplied path of apk file
-    """
-    # Add internet permission
-    logger.debug("Checking internet permission and extractNativeLibs settings")
-    android_manifest = decompiled_path.joinpath("AndroidManifest.xml")
-    txt = android_manifest.read_text(encoding="utf-8")
-    pos = txt.index('</manifest>')
-    permission = 'android.permission.INTERNET'
-
-    if permission not in txt:
-        logger.debug(
-            "Adding 'android.permission.INTERNET' permission to AndroidManifest.xml")
-        permissions_txt = f"<uses-permission android:name='{permission}'/>"
-        txt = txt[:pos] + permissions_txt + txt[pos:]
-
-    # Set extractNativeLibs to true
-    if ':extractNativeLibs="false"' in txt:
-        logger.debug('Editing the extractNativeLibs="true"')
-        txt = txt.replace(':extractNativeLibs="false"',
-                            ':extractNativeLibs="true"')
-    android_manifest.write_text(txt, encoding="utf-8")
-
-def inject_gadget_into_apk(apk_path:str, arch:str, decompiled_path:str):
-    """Inject frida gadget into an APK
-
-    Args:
-        apk (APK): path of apk file
-        arch (str): architecture of the device
-        decompiled_path (str): decomplied path of apk file
-
-    Raises:
-        FileNotFoundError: file not found
-        NotImplementedError: not implemented
-    """
-    apk = APK(apk_path)
-    gadget_path = download_gadget(arch) # Download gadget library
-    gadget_name = Path(gadget_path).name
-    main_activity = apk.get_main_activity()
-    # Apply permission to android manifest
-    modify_manifest(decompiled_path)
-
-    # Search the main activity from smali files
-    load_library_name = gadget_name[:-3]
-    insert_loadlibary(decompiled_path, main_activity, load_library_name)
-
-    # Copy the frida gadget library to the lib directory
-    lib = decompiled_path.joinpath('lib')
-    if not lib.exists():
-        lib.mkdir()
-    arch_dirnames = {'arm': 'armeabi-v7a', 'arm64': 'arm64-v8a'}
-    if arch not in arch_dirnames:
-        raise NotImplementedError(f"The architecture '{arch}' is not supported.")
-
-    arch_dirname = arch_dirnames[arch]
-    lib = lib.joinpath(arch_dirname)
-    if not lib.exists():
-        lib.mkdir()
-
-    lib_library_name = gadget_name
-    if not lib_library_name.startswith('lib'):
-        lib_library_name = 'lib' + gadget_name
-    shutil.copy(gadget_path, lib.joinpath(lib_library_name))
-
-    logger.debug('Recompiling the new APK using apktool')
-
-
-
-@click.command()
-@click.option('--arch', default="arm64", help='Support [arm, arm64, x86]')
-@click.argument('apk_path', type=click.Path(exists=True), required=True)
-def run(apk_path: str, arch: str):
-    """Patch an APK with the Frida gadget library
-
-    Args:
-        apk_path (str): Path of the target APK file
-        arch (str): Target architecture of the device
-
-    Outputs:
-        Injected APK file
-    """
-    assert apk_path.endswith('.apk')
-    apk_path = Path(apk_path)
-
-    logger.info("APK: '%s'", apk_path)
-    logger.info("Gadget Architecture(--arch): %s%s", arch, "(default)" if arch == "arm64" else "")
-
-    arch = arch.lower()
-    supported_archs = ['arm', 'arm64', 'x86']
-    if arch not in supported_archs:
-        logger.error(
-            "The --arch option only supports the following architectures: %s",
-            ", ".join(supported_archs)
-        )
-        sys.exit(-1)
-
-    # Make temp directory for decompile
-    logger.debug("Decompiling the target APK using apktool")
-    decompiled_path = TEMP_DIR.joinpath(str(apk_path.resolve())[:-4])
-    if decompiled_path.exists():
-        shutil.rmtree(decompiled_path)
-    decompiled_path.mkdir()
-
-    # APK decompile with apktool
-    run_apktool(['d', '-o', str(decompiled_path.resolve()), '-f'], str(apk_path.resolve()))
-
-    # Process if decompile is success
-    inject_gadget_into_apk(apk_path, arch, decompiled_path)
-
-    # Rebuild with apktool, print apk_path if process is success
-    run_apktool('b', str(decompiled_path.resolve()))
-    apk_path = decompiled_path.joinpath('dist', apk_path.name)
-    logger.info('Success!\n')
-    logger.info('Output: %s', str(apk_path.resolve()))
-
-
-if __name__ == '__main__':
-    # pylint: disable=no-value-for-parameter
-    run()
+"""Frida gadget injector for Android APK"""
+import os
+import sys
+import shutil
+import subprocess
+from shutil import which
+from pathlib import Path
+import click
+from androguard.core.bytecodes.apk import APK
+from .logger import logger
+from .frida_github import FridaGithub
+from . import INSTALLED_FRIDA_VERSION
+
+
+p = Path(__file__)
+ROOT_DIR = p.parent.resolve()
+TEMP_DIR = ROOT_DIR.joinpath('temp')
+FILE_DIR = ROOT_DIR.joinpath('files')
+
+APKTOOL = which("apktool")
+if not APKTOOL:
+    raise FileNotFoundError(
+        "Please download the 'apktool' and set it to your PATH environment.")
+
+def run_apktool(option, apk_path: str):
+    """Run apktool with option
+
+    Args:
+        option (list|str): option of apktool
+        apk_path (str): path of apk file
+
+    """
+    if isinstance(option, list):
+        cmd = [APKTOOL] + option + [apk_path]
+    else:
+        cmd = [APKTOOL, option, apk_path]
+
+    pipe = subprocess.PIPE
+    with subprocess.Popen(cmd, stdin=pipe, stdout=pipe, stderr=pipe) as process:
+        _, stderr = process.communicate(b"\n")
+        if process.returncode != 0:
+            raise subprocess.CalledProcessError(process.returncode, cmd, stderr)
+        return True
+
+def download_gadget(arch: str):
+    """Download the frida gadget library
+
+    Args:
+        arch (str): architecture of the device
+    """
+    frida_github = FridaGithub(INSTALLED_FRIDA_VERSION)
+    assets = frida_github.get_assets()
+    file = f'frida-gadget-{INSTALLED_FRIDA_VERSION}-android-{arch}.so.xz'
+    for asset in assets:
+        if asset['name'] == file:
+            logger.debug("Downloading the frida gadget library for %s", arch)
+            so_gadget_path = str(FILE_DIR.joinpath(file[:-3]))
+            return frida_github.download_gadget_so(asset['browser_download_url'], so_gadget_path)
+
+    raise FileNotFoundError(f"'{file}' not found in the github releases")
+
+def insert_loadlibary(decompiled_path, main_activity, load_library_name):
+    """Inject loadlibary code to main activity
+
+    Args:
+        text (str): smali code of the main activity
+    """
+    logger.debug('Searching for the main activity in the smali files')
+    target_smali = None
+
+    target_relative_path = main_activity.replace(".", os.sep)
+
+    for directory in decompiled_path.iterdir():
+        if directory.is_dir() and directory.name.startswith("smali"):
+            target_smali = directory.joinpath(target_relative_path + ".smali")
+            if target_smali.exists():
+                break
+
+    if not target_smali or not target_smali.exists():
+        raise FileNotFoundError(f"The target class file {target_smali} was not found.")
+
+    logger.debug("Found the main activity at '%s'", str(target_smali))
+    text = target_smali.read_text()
+
+    text = text.replace(
+        "invoke-virtual {v0, v1}, Ljava/lang/Runtime;->exit(I)V", "")
+    text = text.split("\n")
+
+
+    logger.debug(
+        'Locating the entrypoint method and injecting the loadLibrary code')
+    status = False
+    entrypoints = ["onCreate(", "<init>"]
+    for entrypoint in entrypoints:
+        idx = 0
+        while idx != len(text):
+            line = text[idx].strip()
+            if line.startswith('.method') and entrypoint in line:
+                locals_line_bit = text[idx + 1].split(".locals ")
+                locals_variable_count = int(locals_line_bit[1])
+                locals_line_bit[1] = str(locals_variable_count + 1)
+                if load_library_name.startswith('lib'):
+                    load_library_name = load_library_name[3:]
+
+                new_locals_line = ".locals ".join(locals_line_bit)
+                text[idx + 1] = new_locals_line
+
+                load_str = f'    const-string v{locals_variable_count}, "{load_library_name}"'
+                load_library = f'    invoke-static {{v{locals_variable_count}}}, \
+                    Ljava/lang/System;->loadLibrary(Ljava/lang/String;)V'
+                text.insert(idx + 2, load_library)
+                text.insert(idx + 2, load_str)
+                status = True
+                break
+            idx += 1
+
+        if status:
+            break
+
+    if not status:
+        issue_url = 'https://github.com/ksg97031/frida-gadget/issues'
+        logger.error(
+            "Cannot find the appropriate position in the main activity.")
+        logger.error(
+            "Please report the issue at %s with the following information:", issue_url)
+        logger.error("APK Name: <Your APK Name>")
+        logger.error("APK Version: <Your APK Version>")
+        logger.error("APKTOOL Version: <Your APKTOOL Version>")
+        sys.exit(-1)
+
+    # Replace the smali file with the new one
+    target_smali.write_text("\n".join(text))
+
+def modify_manifest(decompiled_path):
+    """Modify manifest permssions
+
+    Args:
+        decompiled_path (str): decomplied path of apk file
+    """
+    # Add internet permission
+    logger.debug("Checking internet permission and extractNativeLibs settings")
+    android_manifest = decompiled_path.joinpath("AndroidManifest.xml")
+    txt = android_manifest.read_text(encoding="utf-8")
+    pos = txt.index('</manifest>')
+    permission = 'android.permission.INTERNET'
+
+    if permission not in txt:
+        logger.debug(
+            "Adding 'android.permission.INTERNET' permission to AndroidManifest.xml")
+        permissions_txt = f"<uses-permission android:name='{permission}'/>"
+        txt = txt[:pos] + permissions_txt + txt[pos:]
+
+    # Set extractNativeLibs to true
+    if ':extractNativeLibs="false"' in txt:
+        logger.debug('Editing the extractNativeLibs="true"')
+        txt = txt.replace(':extractNativeLibs="false"',
+                            ':extractNativeLibs="true"')
+    android_manifest.write_text(txt, encoding="utf-8")
+
+def inject_gadget_into_apk(apk_path:str, arch:str, decompiled_path:str):
+    """Inject frida gadget into an APK
+
+    Args:
+        apk (APK): path of apk file
+        arch (str): architecture of the device
+        decompiled_path (str): decomplied path of apk file
+
+    Raises:
+        FileNotFoundError: file not found
+        NotImplementedError: not implemented
+    """
+    apk = APK(apk_path)
+    gadget_path = download_gadget(arch) # Download gadget library
+    gadget_name = Path(gadget_path).name
+    main_activity = apk.get_main_activity()
+    # Apply permission to android manifest
+    modify_manifest(decompiled_path)
+
+    # Search the main activity from smali files
+    load_library_name = gadget_name[:-3]
+    insert_loadlibary(decompiled_path, main_activity, load_library_name)
+
+    # Copy the frida gadget library to the lib directory
+    lib = decompiled_path.joinpath('lib')
+    if not lib.exists():
+        lib.mkdir()
+    arch_dirnames = {'arm': 'armeabi-v7a', 'x86':'x86', 'arm64': 'arm64-v8a', 'x86_64':'x86_64'}
+    if arch not in arch_dirnames:
+        raise NotImplementedError(f"The architecture '{arch}' is not supported.")
+
+    arch_dirname = arch_dirnames[arch]
+    lib = lib.joinpath(arch_dirname)
+    if not lib.exists():
+        lib.mkdir()
+
+    lib_library_name = gadget_name
+    if not lib_library_name.startswith('lib'):
+        lib_library_name = 'lib' + gadget_name
+    shutil.copy(gadget_path, lib.joinpath(lib_library_name))
+
+    logger.debug('Recompiling the new APK using apktool')
+
+
+
+@click.command()
+@click.option('--arch', default="arm64", help='Support [arm, arm64, x86, x86_64]')
+@click.option('--skip-decompile', is_flag=True)
+@click.option('--skip-recompile', is_flag=True)
+@click.argument('apk_path', type=click.Path(exists=True), required=True)
+def run(apk_path: str, skip_decompile:bool, skip_recompile:bool, arch: str):
+    """Patch an APK with the Frida gadget library
+
+    Args:
+        apk_path (str): Path of the target APK file
+        arch (str): Target architecture of the device
+
+    Outputs:
+        Injected APK file
+    """
+    apk_path = Path(apk_path)
+
+    logger.info("APK: '%s'", apk_path)
+    logger.info("Gadget Architecture(--arch): %s%s", arch, "(default)" if arch == "arm64" else "")
+
+    arch = arch.lower()
+    supported_archs = ['arm', 'arm64', 'x86', 'x86_64']
+    if arch not in supported_archs:
+        logger.error(
+            "The --arch option only supports the following architectures: %s",
+            ", ".join(supported_archs)
+        )
+        sys.exit(-1)
+
+    # Make temp directory for decompile
+   
+    decompiled_path = TEMP_DIR.joinpath(str(apk_path.resolve())[:-4])
+    if not skip_decompile:
+        logger.debug("Decompiling the target APK using apktool")
+        if decompiled_path.exists():
+            shutil.rmtree(decompiled_path)
+        decompiled_path.mkdir()
+
+        # APK decompile with apktool
+        run_apktool(['d', '-o', str(decompiled_path.resolve()), '-f'], str(apk_path.resolve()))
+
+    # Process if decompile is success
+    inject_gadget_into_apk(apk_path, arch, decompiled_path)
+
+    # Rebuild with apktool, print apk_path if process is success
+    if not skip_recompile:
+        run_apktool('b', str(decompiled_path.resolve()))
+        apk_path = decompiled_path.joinpath('dist', apk_path.name)
+        logger.info('Success: %s', str(apk_path.resolve()))
+
+
+if __name__ == '__main__':
+    # pylint: disable=no-value-for-parameter
+    run()
```

### Comparing `frida-gadget-1.1.3/scripts/frida_github.py` & `frida-gadget-1.2.0/scripts/frida_github.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-"""Github module for download frida gadget library"""
-# Base code is sourced from the GitHub repository of Objection.
-# Source: https://github.com/sensepost/objection/blob/master/objection/utils/patchers/github.py
-import lzma
-from pathlib import Path
-import requests
-
-class FridaGithub:
-    """ Interact with Github """
-
-    GITHUB_LATEST_RELEASE = 'https://api.github.com/repos/frida/frida/releases/latest'
-    GITHUB_TAGGED_RELEASE = 'https://api.github.com/repos/frida/frida/releases/tags/{tag}'
-
-    # the 'context' of this Github instance
-    gadget_version = None
-
-    def __init__(self, gadget_version: str = None):
-        """
-            Init a new instance of Github
-        """
-
-        if gadget_version:
-            self.gadget_version = gadget_version
-
-        self.request_cache = {}
-
-    def _call(self, endpoint: str) -> dict:
-        """
-            Make a call to Github and cache the response.
-
-            :param endpoint:
-            :return:
-        """
-
-        # return a cached response if possible
-        if endpoint in self.request_cache:
-            return self.request_cache[endpoint]
-
-        # get a new response
-        results = requests.get(endpoint, timeout=30).json()
-
-        # cache it
-        self.request_cache[endpoint] = results
-
-        # and return it
-        return results
-
-    def get_latest_version(self) -> str:
-        """
-            Call Github and get the tag_name of the latest
-            release.
-
-            :return:
-        """
-
-        self.gadget_version = self._call(self.GITHUB_LATEST_RELEASE)['tag_name']
-
-        return self.gadget_version
-
-    def get_assets(self) -> dict:
-        """
-            Gets the assets for the currently selected gadget_version.
-
-            :return:
-        """
-
-        assets = self._call(self.GITHUB_TAGGED_RELEASE.format(tag=self.gadget_version))
-
-        if 'assets' not in assets:
-            raise FileNotFoundError(
-                f'Unable to determine assets for gadget version \'{self.gadget_version}\'. '
-                'Are you sure this version is available on Github?')
-
-        return assets['assets']
-
-    def download_asset(self, url: str, output_file: str) -> None:
-        """
-            Download an asset from Github.
-
-            :param url:
-            :param output_file:
-            :return:
-        """
-
-        assert output_file.endswith('.xz')
-        filepath = Path(output_file)
-        if filepath.exists() and filepath.stat().st_size > 0:
-            return
-
-        response = requests.get(url, timeout=600, stream=True)
-        with open(output_file, 'wb') as asset:
-            for chunk in response.iter_content(chunk_size=1024):
-                if chunk:
-                    asset.write(chunk)
-
-    def download_gadget_so(self, url, gadget_fullpath: str) -> str:
-        """
-            Download the gadget library from Github.
-
-            :param gadget_path:
-            :return:
-        """
-
-        assert gadget_fullpath.endswith('.so')
-        if Path(gadget_fullpath).exists():
-            return gadget_fullpath
-
-        xz_gadget_fullpath = gadget_fullpath + ".xz"
-        self.download_asset(url, xz_gadget_fullpath)
-
-        with lzma.open(xz_gadget_fullpath, "rb") as lzma_file:
-            decompressed_data = lzma_file.read()
-        with open(gadget_fullpath, "wb") as gadget_file:
-            gadget_file.write(decompressed_data)
-
-        return gadget_fullpath
+"""Github module for download frida gadget library"""
+# Base code is sourced from the GitHub repository of Objection.
+# Source: https://github.com/sensepost/objection/blob/master/objection/utils/patchers/github.py
+import lzma
+from pathlib import Path
+import requests
+
+class FridaGithub:
+    """ Interact with Github """
+
+    GITHUB_LATEST_RELEASE = 'https://api.github.com/repos/frida/frida/releases/latest'
+    GITHUB_TAGGED_RELEASE = 'https://api.github.com/repos/frida/frida/releases/tags/{tag}'
+
+    # the 'context' of this Github instance
+    gadget_version = None
+
+    def __init__(self, gadget_version: str = None):
+        """
+            Init a new instance of Github
+        """
+
+        if gadget_version:
+            self.gadget_version = gadget_version
+
+        self.request_cache = {}
+
+    def _call(self, endpoint: str) -> dict:
+        """
+            Make a call to Github and cache the response.
+
+            :param endpoint:
+            :return:
+        """
+
+        # return a cached response if possible
+        if endpoint in self.request_cache:
+            return self.request_cache[endpoint]
+
+        # get a new response
+        results = requests.get(endpoint, timeout=30).json()
+
+        # cache it
+        self.request_cache[endpoint] = results
+
+        # and return it
+        return results
+
+    def get_latest_version(self) -> str:
+        """
+            Call Github and get the tag_name of the latest
+            release.
+
+            :return:
+        """
+
+        self.gadget_version = self._call(self.GITHUB_LATEST_RELEASE)['tag_name']
+
+        return self.gadget_version
+
+    def get_assets(self) -> dict:
+        """
+            Gets the assets for the currently selected gadget_version.
+
+            :return:
+        """
+
+        assets = self._call(self.GITHUB_TAGGED_RELEASE.format(tag=self.gadget_version))
+
+        if 'assets' not in assets:
+            raise FileNotFoundError(
+                f'Unable to determine assets for gadget version \'{self.gadget_version}\'. '
+                'Are you sure this version is available on Github?')
+
+        return assets['assets']
+
+    def download_asset(self, url: str, output_file: str) -> None:
+        """
+            Download an asset from Github.
+
+            :param url:
+            :param output_file:
+            :return:
+        """
+
+        assert output_file.endswith('.xz')
+        filepath = Path(output_file)
+        if filepath.exists() and filepath.stat().st_size > 0:
+            return
+
+        response = requests.get(url, timeout=600, stream=True)
+        with open(output_file, 'wb') as asset:
+            for chunk in response.iter_content(chunk_size=1024):
+                if chunk:
+                    asset.write(chunk)
+
+    def download_gadget_so(self, url, gadget_fullpath: str) -> str:
+        """
+            Download the gadget library from Github.
+
+            :param gadget_path:
+            :return:
+        """
+
+        assert gadget_fullpath.endswith('.so')
+        if Path(gadget_fullpath).exists():
+            return gadget_fullpath
+
+        xz_gadget_fullpath = gadget_fullpath + ".xz"
+        self.download_asset(url, xz_gadget_fullpath)
+
+        with lzma.open(xz_gadget_fullpath, "rb") as lzma_file:
+            decompressed_data = lzma_file.read()
+        with open(gadget_fullpath, "wb") as gadget_file:
+            gadget_file.write(decompressed_data)
+
+        return gadget_fullpath
```

