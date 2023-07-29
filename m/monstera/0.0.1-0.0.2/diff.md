# Comparing `tmp/monstera-0.0.1.tar.gz` & `tmp/monstera-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monstera-0.0.1.tar", last modified: Thu Jul 27 18:51:04 2023, max compression
+gzip compressed data, was "monstera-0.0.2.tar", last modified: Fri Jul 28 23:56:35 2023, max compression
```

## Comparing `monstera-0.0.1.tar` & `monstera-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-27 18:51:04.073143 monstera-0.0.1/
--rw-r--r--   0 dishb      (502) staff       (20)     1099 2023-07-23 01:06:44.000000 monstera-0.0.1/LICENSE.md
--rw-r--r--   0 dishb      (502) staff       (20)     4103 2023-07-27 18:51:04.072447 monstera-0.0.1/PKG-INFO
--rw-r--r--   0 dishb      (502) staff       (20)     2990 2023-07-27 18:03:46.000000 monstera-0.0.1/README.md
-drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-27 18:51:04.063916 monstera-0.0.1/monstera/
--rw-r--r--   0 dishb      (502) staff       (20)     4950 2023-07-27 17:41:13.000000 monstera-0.0.1/monstera/__init__.py
--rw-r--r--   0 dishb      (502) staff       (20)     2848 2023-07-27 17:41:19.000000 monstera-0.0.1/monstera/__main__.py
-drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-27 18:51:04.071488 monstera-0.0.1/monstera.egg-info/
--rw-r--r--   0 dishb      (502) staff       (20)     4103 2023-07-27 18:51:04.000000 monstera-0.0.1/monstera.egg-info/PKG-INFO
--rw-r--r--   0 dishb      (502) staff       (20)      265 2023-07-27 18:51:04.000000 monstera-0.0.1/monstera.egg-info/SOURCES.txt
--rw-r--r--   0 dishb      (502) staff       (20)        1 2023-07-27 18:51:04.000000 monstera-0.0.1/monstera.egg-info/dependency_links.txt
--rw-r--r--   0 dishb      (502) staff       (20)       53 2023-07-27 18:51:04.000000 monstera-0.0.1/monstera.egg-info/entry_points.txt
--rw-r--r--   0 dishb      (502) staff       (20)       16 2023-07-27 18:51:04.000000 monstera-0.0.1/monstera.egg-info/requires.txt
--rw-r--r--   0 dishb      (502) staff       (20)        9 2023-07-27 18:51:04.000000 monstera-0.0.1/monstera.egg-info/top_level.txt
--rw-r--r--   0 dishb      (502) staff       (20)       38 2023-07-27 18:51:04.073345 monstera-0.0.1/setup.cfg
--rw-r--r--   0 dishb      (502) staff       (20)     2266 2023-07-27 18:39:23.000000 monstera-0.0.1/setup.py
+drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-28 23:56:35.098635 monstera-0.0.2/
+-rw-r--r--   0 dishb      (502) staff       (20)     1099 2023-07-28 01:34:18.000000 monstera-0.0.2/LICENSE.md
+-rw-r--r--   0 dishb      (502) staff       (20)     5737 2023-07-28 23:56:35.097747 monstera-0.0.2/PKG-INFO
+-rw-r--r--   0 dishb      (502) staff       (20)     4448 2023-07-28 23:11:49.000000 monstera-0.0.2/README.md
+drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-28 23:56:35.072533 monstera-0.0.2/monstera/
+-rw-r--r--   0 dishb      (502) staff       (20)     6303 2023-07-28 23:37:45.000000 monstera-0.0.2/monstera/__init__.py
+-rw-r--r--   0 dishb      (502) staff       (20)     4283 2023-07-28 02:31:08.000000 monstera-0.0.2/monstera/__main__.py
+drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-28 23:56:35.078935 monstera-0.0.2/monstera.egg-info/
+-rw-r--r--   0 dishb      (502) staff       (20)     5737 2023-07-28 23:56:35.000000 monstera-0.0.2/monstera.egg-info/PKG-INFO
+-rw-r--r--   0 dishb      (502) staff       (20)      311 2023-07-28 23:56:35.000000 monstera-0.0.2/monstera.egg-info/SOURCES.txt
+-rw-r--r--   0 dishb      (502) staff       (20)        1 2023-07-28 23:56:35.000000 monstera-0.0.2/monstera.egg-info/dependency_links.txt
+-rw-r--r--   0 dishb      (502) staff       (20)       53 2023-07-28 23:56:35.000000 monstera-0.0.2/monstera.egg-info/entry_points.txt
+-rw-r--r--   0 dishb      (502) staff       (20)       16 2023-07-28 23:56:35.000000 monstera-0.0.2/monstera.egg-info/requires.txt
+-rw-r--r--   0 dishb      (502) staff       (20)        9 2023-07-28 23:56:35.000000 monstera-0.0.2/monstera.egg-info/top_level.txt
+-rw-r--r--   0 dishb      (502) staff       (20)       38 2023-07-28 23:56:35.098886 monstera-0.0.2/setup.cfg
+-rw-r--r--   0 dishb      (502) staff       (20)     3620 2023-07-28 23:52:08.000000 monstera-0.0.2/setup.py
+drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-28 23:56:35.091733 monstera-0.0.2/tests/
+-rw-r--r--   0 dishb      (502) staff       (20)     3774 2023-07-28 19:32:17.000000 monstera-0.0.2/tests/test_monstera.py
+-rw-r--r--   0 dishb      (502) staff       (20)     3858 2023-07-28 19:31:28.000000 monstera-0.0.2/tests/test_python_m.py
```

### Comparing `monstera-0.0.1/LICENSE.md` & `monstera-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monstera-0.0.1/PKG-INFO` & `monstera-0.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1
-Name: monstera
-Version: 0.0.1
-Summary: A cross-platform CLI to quickly retrieve system information to make issue management easier.
-Home-page: https://github.com/dishb/monstera
-Author: Dishant B. (@dishb)
-Author-email: code.dishb@gmail.com
-License: MIT
-Project-URL: Documentation, https://github.com/dishb/monstera/tree/main/docs
-Project-URL: Source, https://github.com/dishb/monstera/
-Project-URL: Issue Tracker, https://github.com/dishb/monstera/issues
-Keywords: monstera,bug tracker,bug tracking,issue tracker,issue tracking,tool,developers,developing,monstera tool,dependencies,versions,file locations,python,cross-platform,python3
-Classifier: Intended Audience :: Education
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Topic :: Software Development :: Bug Tracking
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
+<!--
+MIT License
 
-![monstera's banner image](./assets/banner.png)
+Copyright (c) 2023 Dishant B. (@dishb) <code.dishb@gmail.com>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+-->
+
+![monstera's banner image](https://github.com/dishb/monstera/blob/2517642244aac49d978ed6b779cedb8e4fbb4681/assets/banner.png)
 
 # monstera
 
 A cross-platform CLI to quickly retrieve system information to make issue management easier.
 
 ## Features:
 A list of all the information collected:
@@ -71,15 +71,15 @@
     import monstera
 
     monstera.run()
     ```
 
 ## Contributing:
 To get started with contributing to `monstera`, follow this guide.
-It is recommended to read the [`./CONTRIBUTING.md`](https://github.com/dishb/monstera/blob/main/CONTRIBUTING.md) file.
+It is recommended to read the [`./.github/CONTRIBUTING.md`](https://github.com/dishb/monstera/blob/main/.github/CONTRIBUTING.md) file.
 
 1. Clone the repository:
 
     | OS Independent |
     | --- |
     | `git clone https://github.com/dishb/monstera` |
 
@@ -105,14 +105,18 @@
 
 4. Install `monstera` in edit mode:
 
     | macOS/Linux | Windows |
     | --- | --- |
     | `pip3 install -e .` | `pip install -e .` |
 
+## Code of Conduct
+This project is goverened by the Contributor Covenant Code of Conduct.
+We ask that you read the full Code of Conduct in the [`./.github/CODE_OF_CONDUCT.md`](https://github.com/dishb/monstera/blob/main/.github/CODE_OF_CONDUCT.md) file.
+
 ## License:
 This project is licensed under the `MIT License`. The full copyright can be found in the [`./LICENSE.md`](https://github.com/dishb/monstera/blob/main/LICENSE.md) file.
 
 ## Attribution
 
 The background photo in [`./assets/banner.png`](https://github.com/dishb/monstera/blob/main/assets/banner.png) is by [Gilles Lambert](https://unsplash.com/@gilleslambert?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/photos/mSK5nNsAsLY?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)
```

### Comparing `monstera-0.0.1/monstera/__init__.py` & `monstera-0.0.2/monstera/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,50 @@
+#
+# MIT License
+#
+# Copyright (c) 2023 Dishant B. (@dishb) <code.dishb@gmail.com>
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
+
 """
 monstera
 
 Author: Dishant B. (@dishb) code.dishb@gmail.com
 License: MIT License
 Source: https://github.com/dishb/monstera
 """
 
 import sys
 import platform
 from os.path import dirname
-from subprocess import run as sp_run
+from subprocess import CalledProcessError, run as sp_run
 from typing import Dict, List, Union
 
 import distro
 
 __source__ = "https://github.com/dishb/monstera"
 __license__ = "MIT License"
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __author__ = "Dishant B. (@dishb) <code.dishb@gmail.com>"
 __copyright__ = """
                 MIT License
 
                 Copyright (c) 2023 Dishant B. (@dishb) <code.dishb@gmail.com>
 
                 Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -78,19 +102,23 @@
         pip_cmd = "pip"
 
     pkg_vers = []
     pkg_locs = []
 
     if packages is not None:
         for pkg in packages:
-            output1 = sp_run([pip_cmd, "show", pkg], check = True, capture_output = True).stdout
-            output1 = output1.decode().split("\n")
-
-            pkg_locs.append(output1[7].split()[1])
-            pkg_vers.append(output1[1].split()[1])
+            try:
+                output1 = sp_run([pip_cmd, "show", pkg], check = True, capture_output = True).stdout
+                output1 = output1.decode().split("\n")
+
+                pkg_locs.append(output1[7].split()[1])
+                pkg_vers.append(output1[1].split()[1])
+            except CalledProcessError:
+                pkg_locs.append(f"{pkg} is not installed")
+                pkg_vers.append(f"{pkg} is not installed.")
 
     major = sys.version_info[0]
     minor = sys.version_info[1]
     patch = sys.version_info[2]
     level = sys.version_info[3]
     if level == "candidate":
         level = "release candidate"
```

