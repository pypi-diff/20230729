# Comparing `tmp/aiogram3_di-1.0.1.tar.gz` & `tmp/aiogram3_di-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram3_di-1.0.1.tar", last modified: Sat Jul 29 08:00:42 2023, max compression
+gzip compressed data, was "aiogram3_di-1.0.2.tar", last modified: Sat Jul 29 09:13:11 2023, max compression
```

## Comparing `aiogram3_di-1.0.1.tar` & `aiogram3_di-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-29 08:00:42.953884 aiogram3_di-1.0.1/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1075 2023-01-01 13:29:08.000000 aiogram3_di-1.0.1/LICENSE
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1285 2023-07-29 08:00:42.953884 aiogram3_di-1.0.1/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      997 2023-07-28 19:57:37.000000 aiogram3_di-1.0.1/README.md
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-29 08:00:42.953884 aiogram3_di-1.0.1/aiogram3_di/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      142 2023-07-28 19:36:21.000000 aiogram3_di-1.0.1/aiogram3_di/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-07-29 07:54:36.000000 aiogram3_di-1.0.1/aiogram3_di/_version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      289 2023-07-28 19:58:50.000000 aiogram3_di-1.0.1/aiogram3_di/depends.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      628 2023-07-29 07:32:25.000000 aiogram3_di-1.0.1/aiogram3_di/middleware.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3615 2023-07-29 07:46:05.000000 aiogram3_di-1.0.1/aiogram3_di/utils.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-29 08:00:42.953884 aiogram3_di-1.0.1/aiogram3_di.egg-info/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1285 2023-07-29 08:00:42.000000 aiogram3_di-1.0.1/aiogram3_di.egg-info/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      318 2023-07-29 08:00:42.000000 aiogram3_di-1.0.1/aiogram3_di.egg-info/SOURCES.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-07-29 08:00:42.000000 aiogram3_di-1.0.1/aiogram3_di.egg-info/dependency_links.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       17 2023-07-29 08:00:42.000000 aiogram3_di-1.0.1/aiogram3_di.egg-info/requires.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       12 2023-07-29 08:00:42.000000 aiogram3_di-1.0.1/aiogram3_di.egg-info/top_level.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-07-29 08:00:42.953884 aiogram3_di-1.0.1/setup.cfg
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      725 2023-07-28 20:04:06.000000 aiogram3_di-1.0.1/setup.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-29 09:13:11.390751 aiogram3_di-1.0.2/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1075 2023-01-01 13:29:08.000000 aiogram3_di-1.0.2/LICENSE
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1650 2023-07-29 09:13:11.390751 aiogram3_di-1.0.2/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      994 2023-07-29 09:11:26.000000 aiogram3_di-1.0.2/README.md
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-29 09:13:11.390751 aiogram3_di-1.0.2/aiogram3_di/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      142 2023-07-28 19:36:21.000000 aiogram3_di-1.0.2/aiogram3_di/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-07-29 09:11:56.000000 aiogram3_di-1.0.2/aiogram3_di/_version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      289 2023-07-28 19:58:50.000000 aiogram3_di-1.0.2/aiogram3_di/depends.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      628 2023-07-29 07:32:25.000000 aiogram3_di-1.0.2/aiogram3_di/middleware.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3615 2023-07-29 07:46:05.000000 aiogram3_di-1.0.2/aiogram3_di/utils.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-29 09:13:11.390751 aiogram3_di-1.0.2/aiogram3_di.egg-info/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1650 2023-07-29 09:13:11.000000 aiogram3_di-1.0.2/aiogram3_di.egg-info/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      318 2023-07-29 09:13:11.000000 aiogram3_di-1.0.2/aiogram3_di.egg-info/SOURCES.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-07-29 09:13:11.000000 aiogram3_di-1.0.2/aiogram3_di.egg-info/dependency_links.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       17 2023-07-29 09:13:11.000000 aiogram3_di-1.0.2/aiogram3_di.egg-info/requires.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       12 2023-07-29 09:13:11.000000 aiogram3_di-1.0.2/aiogram3_di.egg-info/top_level.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-07-29 09:13:11.390751 aiogram3_di-1.0.2/setup.cfg
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1071 2023-07-29 09:13:00.000000 aiogram3_di-1.0.2/setup.py
```

### Comparing `aiogram3_di-1.0.1/LICENSE` & `aiogram3_di-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram3_di-1.0.1/PKG-INFO` & `aiogram3_di-1.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,16 @@
-Metadata-Version: 2.1
-Name: aiogram3_di
-Version: 1.0.1
-Summary: Dependency Injection implementation for aiogram 3.
-Home-page: https://github.com/Vladyslav49/aiogram3_di
-Author: Vladyslav49
-License: MIT
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ### Example of usage
 
 ```python
 import logging
 from os import getenv
 from typing import Annotated
 
 from aiogram import Router, Bot, Dispatcher
 from aiogram.types import Message, User
-
 from aiogram3_di import DIMiddleware, Depends
 
 router = Router()
 
 
 def get_user_full_name(event_from_user: User) -> str:
     return event_from_user.full_name
@@ -46,14 +34,14 @@
 
 if __name__ == '__main__':
     main()
 ```
 
 ### Details
 
-It is inspired by [FastAPI]('https://github.com/tiangolo/fastapi').
+It is inspired by [FastAPI](https://github.com/tiangolo/fastapi).
 
 If you define a normal def, your function will be called in a different thread.
 
 ### License
 
 MIT
```

### Comparing `aiogram3_di-1.0.1/README.md` & `aiogram3_di-1.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,34 @@
+Metadata-Version: 2.1
+Name: aiogram3_di
+Version: 1.0.2
+Summary: Dependency Injection implementation for aiogram 3.
+Home-page: https://github.com/Vladyslav49/aiogram3_di
+Author: Vladyslav49
+Author-email: 
+License: MIT
+Keywords: Aiogram,Telegram,Bots,DI,Dependency Injection
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ### Example of usage
 
 ```python
 import logging
 from os import getenv
 from typing import Annotated
 
 from aiogram import Router, Bot, Dispatcher
 from aiogram.types import Message, User
-
 from aiogram3_di import DIMiddleware, Depends
 
 router = Router()
 
 
 def get_user_full_name(event_from_user: User) -> str:
     return event_from_user.full_name
@@ -35,14 +52,14 @@
 
 if __name__ == '__main__':
     main()
 ```
 
 ### Details
 
-It is inspired by [FastAPI]('https://github.com/tiangolo/fastapi').
+It is inspired by [FastAPI](https://github.com/tiangolo/fastapi).
 
 If you define a normal def, your function will be called in a different thread.
 
 ### License
 
 MIT
```

### Comparing `aiogram3_di-1.0.1/aiogram3_di/middleware.py` & `aiogram3_di-1.0.2/aiogram3_di/middleware.py`

 * *Files identical despite different names*

### Comparing `aiogram3_di-1.0.1/aiogram3_di/utils.py` & `aiogram3_di-1.0.2/aiogram3_di/utils.py`

 * *Files identical despite different names*

