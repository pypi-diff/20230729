# Comparing `tmp/teelebot-2.3.4-py3-none-any.whl.zip` & `tmp/teelebot-2.3.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 40905 bytes, number of entries: 20
+Zip file size: 40922 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat     4301 b- defN 23-Jul-12 14:12 teelebot/__init__.py
 -rw-rw-rw-  2.0 fat      165 b- defN 23-May-08 17:02 teelebot/__main__.py
--rw-rw-rw-  2.0 fat    33199 b- defN 23-May-29 02:04 teelebot/bot.py
+-rw-rw-rw-  2.0 fat    33248 b- defN 23-Jul-29 14:48 teelebot/bot.py
 -rw-rw-rw-  2.0 fat     7248 b- defN 23-Jul-12 13:37 teelebot/buffer.py
 -rw-rw-rw-  2.0 fat     1581 b- defN 23-May-15 07:43 teelebot/common.py
 -rw-rw-rw-  2.0 fat    23439 b- defN 23-Jul-12 13:37 teelebot/handler.py
--rw-rw-rw-  2.0 fat     1807 b- defN 23-May-03 00:00 teelebot/logger.py
+-rw-rw-rw-  2.0 fat     1869 b- defN 23-Jul-29 14:48 teelebot/logger.py
 -rw-rw-rw-  2.0 fat     7235 b- defN 23-Jul-12 13:37 teelebot/metadata.py
 -rw-rw-rw-  2.0 fat      809 b- defN 23-Jul-12 14:13 teelebot/polling.py
 -rw-rw-rw-  2.0 fat     3917 b- defN 23-Jul-12 13:38 teelebot/request.py
 -rw-rw-rw-  2.0 fat     4307 b- defN 23-Jul-12 13:38 teelebot/schedule.py
--rw-rw-rw-  2.0 fat      483 b- defN 23-Jul-12 13:38 teelebot/version.py
+-rw-rw-rw-  2.0 fat      483 b- defN 23-Jul-29 14:48 teelebot/version.py
 -rw-rw-rw-  2.0 fat     2744 b- defN 23-Jul-12 14:14 teelebot/webhook.py
--rw-rw-rw-  2.0 fat    35823 b- defN 23-Jul-12 14:37 teelebot-2.3.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9719 b- defN 23-Jul-12 14:37 teelebot-2.3.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 14:37 teelebot-2.3.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       43 b- defN 23-Jul-12 14:37 teelebot-2.3.4.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-12 14:37 teelebot-2.3.4.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Jul-12 14:37 teelebot-2.3.4.dist-info/zip-safe
--rw-rw-r--  2.0 fat     1558 b- defN 23-Jul-12 14:37 teelebot-2.3.4.dist-info/RECORD
-20 files, 138481 bytes uncompressed, 38399 bytes compressed:  72.3%
+-rw-rw-rw-  2.0 fat    35823 b- defN 23-Jul-29 15:15 teelebot-2.3.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9719 b- defN 23-Jul-29 15:15 teelebot-2.3.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-29 15:15 teelebot-2.3.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       43 b- defN 23-Jul-29 15:15 teelebot-2.3.5.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-29 15:15 teelebot-2.3.5.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Jul-29 15:15 teelebot-2.3.5.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     1558 b- defN 23-Jul-29 15:15 teelebot-2.3.5.dist-info/RECORD
+20 files, 138592 bytes uncompressed, 38416 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -33,29 +33,29 @@
 
 Filename: teelebot/version.py
 Comment: 
 
 Filename: teelebot/webhook.py
 Comment: 
 
-Filename: teelebot-2.3.4.dist-info/LICENSE
+Filename: teelebot-2.3.5.dist-info/LICENSE
 Comment: 
 
-Filename: teelebot-2.3.4.dist-info/METADATA
+Filename: teelebot-2.3.5.dist-info/METADATA
 Comment: 
 
-Filename: teelebot-2.3.4.dist-info/WHEEL
+Filename: teelebot-2.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: teelebot-2.3.4.dist-info/entry_points.txt
+Filename: teelebot-2.3.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: teelebot-2.3.4.dist-info/top_level.txt
+Filename: teelebot-2.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: teelebot-2.3.4.dist-info/zip-safe
+Filename: teelebot-2.3.5.dist-info/zip-safe
 Comment: 
 
-Filename: teelebot-2.3.4.dist-info/RECORD
+Filename: teelebot-2.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## teelebot/bot.py

```diff
@@ -1,12 +1,12 @@
 # -*- coding:utf-8 -*-
 """
 @description: A Python-based Telegram Bot framework
 @creation date: 2019-08-13
-@last modification: 2023-05-29
+@last modification: 2023-07-29
 @author: Pluto (github:plutobell)
 """
 import time
 import sys
 import os
 import copy
 import types
@@ -350,36 +350,38 @@
             message_type = "unknown"
 
         return message_type, message
 
     def __logging_for_pluginRun(self, message, plugin):
         title = ""  # INFO Log
         user_name = ""
+        from_id = ""
 
         if message["chat"]["type"] == "private":
             if "first_name" in message["chat"].keys():
                 title += message["chat"]["first_name"]
             if "last_name" in message["chat"].keys():
                 if "first_name" in message["chat"].keys():
                     title += " " + message["chat"]["last_name"]
                 else:
                     title += message["chat"]["last_name"]
         elif "title" in message["chat"].keys():
             title = message["chat"]["title"]
+
         if "reply_markup" in message.keys() and \
                 message["message_type"] == "callback_query_data":
             from_id = message["click_user"]["id"]
             if "first_name" in message["click_user"].keys():
                 user_name += message["click_user"]["first_name"]
             if "last_name" in message["click_user"].keys():
                 if "first_name" in message["click_user"].keys():
                     user_name += " " + message["click_user"]["last_name"]
                 else:
                     user_name += message["chat"]["last_name"]
-        else:
+        elif "from" in message.keys():
             from_id = message["from"]["id"]
             if "first_name" in message["from"].keys():
                 user_name += message["from"]["first_name"]
             if "last_name" in message["from"].keys():
                 if "first_name" in message["from"].keys():
                     user_name += " " + message["from"]["last_name"]
                 else:
```

## teelebot/logger.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding:utf-8 -*-
 '''
 @creation date: 2019-11-15
-@last modification: 2023-05-03
+@last modification: 2023-07-29
 '''
 import logging
 
 
 BLACK, RED, GREEN, YELLOW, BLUE, MAGENTA, CYAN, WHITE = range(8)
 
 RESET_SEQ = "\033[0m"
@@ -44,15 +44,16 @@
 
 class ColoredLogger(logging.Logger):
     FORMAT = "[$BOLD%(asctime)s][$RESET%(levelname)s] %(message)s"
     COLOR_FORMAT = formatter_message(FORMAT, True)
     def __init__(self, name):
         logging.Logger.__init__(self, name, logging.INFO)
 
-        color_formatter = ColoredFormatter(self.COLOR_FORMAT)
+        color_format = formatter_message(self.COLOR_FORMAT, True)
+        color_formatter = ColoredFormatter(color_format)
 
         console = logging.StreamHandler()
         console.setFormatter(color_formatter)
 
         self.addHandler(console)
         return
```

## teelebot/version.py

```diff
@@ -1,16 +1,16 @@
 # -*- coding:utf-8 -*-
 """
 @description: A Python-based Telegram Bot framework
 @creation date: 2019-11-15
-@last modification: 2023-07-12
+@last modification: 2023-07-29
 @author: Pluto (github:plutobell)
 """
 
-__version__ = "2.3.4"
+__version__ = "2.3.5"
 
 __author__ = "Pluto"
 __email__ = "hi@ojoll.com"
 __blog__ = "https://ojoll.com"
 __github__ = "https://github.com/plutobell/teelebot"
 __description__ = "teelebot is a Python-based Telegram Bot framework with a plugin system that supports hot reload and hot loading."
```

## Comparing `teelebot-2.3.4.dist-info/LICENSE` & `teelebot-2.3.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `teelebot-2.3.4.dist-info/METADATA` & `teelebot-2.3.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teelebot
-Version: 2.3.4
+Version: 2.3.5
 Summary: teelebot is a Python-based Telegram Bot framework with a plugin system that supports hot reload and hot loading.
 Home-page: https://ojoll.com
 Author: Pluto
 Author-email: hi@ojoll.com
 License: GPLv3
 Keywords: teelebot telegram bot telegram bot api telegram
 Classifier: Programming Language :: Python :: 3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: teelebot Version: 2.3.4 Summary: teelebot is a
+Metadata-Version: 2.1 Name: teelebot Version: 2.3.5 Summary: teelebot is a
 Python-based Telegram Bot framework with a plugin system that supports hot
 reload and hot loading. Home-page: https://ojoll.com Author: Pluto Author-
 email: hi@ojoll.com License: GPLv3 Keywords: teelebot telegram bot telegram bot
 api telegram Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Classifier: License :: OSI Approved :: GNU
 General Public License v3 (GPLv3) Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: requests
```

## Comparing `teelebot-2.3.4.dist-info/RECORD` & `teelebot-2.3.5.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 teelebot/__init__.py,sha256=izTaxR9BNZlwoIXdHhP_3pwMipIsEOVhXwYJs5llJXE,4301
 teelebot/__main__.py,sha256=_j6f3hj0VtlcCsabcIvuS0uBI0NVbCVwmH138tqYGFo,165
-teelebot/bot.py,sha256=79U_AoWjkSfAa1hetAK_pCtUh_rBObYcWoxLthyt9Xw,33199
+teelebot/bot.py,sha256=ybcunoTicReae1fQNJREb_ymU2S8YAHzB1bb0Xm56B0,33248
 teelebot/buffer.py,sha256=dKlomQ9aJP4v0TNukChxyGM-oAUBcOv803oW5POeils,7248
 teelebot/common.py,sha256=RHSqpXXmAJ3jFrWOTubgTavfSu0FprHNQyX0llvJ680,1581
 teelebot/handler.py,sha256=qfmlrPZlA7_LtguM3ItnLPMyQ_-0qS3x-WAI3DHcpow,23439
-teelebot/logger.py,sha256=_QWA2Kbj-JWNYDtgeK6IE7q34Brxrq6cUgHEH4YTu2M,1807
+teelebot/logger.py,sha256=I7UJxLdxRz5HxzwEgBPf_gILZuDlPCLwZPxioIahS2A,1869
 teelebot/metadata.py,sha256=pxezwNWaSmBpEACdij-ubvsFtUYwpbJd1GMS9x2SMfM,7235
 teelebot/polling.py,sha256=YAXUqN_XngnykSE0TmpF8O2twQ6wqF1n6lZ6JowmO8A,809
 teelebot/request.py,sha256=PuYRtKYdzGkpxXNO6M_xhfs26o1Lh2W4w5EFPJPjVKM,3917
 teelebot/schedule.py,sha256=7ANts-y4OUW1_5yedpSk3FNRJ5aVAwYVkC-umQohzlQ,4307
-teelebot/version.py,sha256=Pg94QGm-B-6Ozw6cCXtwJe_WR5TgNo9a3VQoXVxmXKc,483
+teelebot/version.py,sha256=xMOs_zzejgn2abkweR3HlXVOBpOLnGXU33qkXvhKmaA,483
 teelebot/webhook.py,sha256=YT0SAuCImdxrYx2_-sB0IQ3vSkG8RZbwxPs7h5QG0cI,2744
-teelebot-2.3.4.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
-teelebot-2.3.4.dist-info/METADATA,sha256=vPqaBLHRuNxjp8ic7FlJlyKaxEg1Mw3qd37fw8ySveo,9719
-teelebot-2.3.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-teelebot-2.3.4.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
-teelebot-2.3.4.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
-teelebot-2.3.4.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-teelebot-2.3.4.dist-info/RECORD,,
+teelebot-2.3.5.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
+teelebot-2.3.5.dist-info/METADATA,sha256=q0K4vQbKipoUpj0-3V44yFdnwVS7Jul69-HMZfZ8XbA,9719
+teelebot-2.3.5.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+teelebot-2.3.5.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
+teelebot-2.3.5.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
+teelebot-2.3.5.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+teelebot-2.3.5.dist-info/RECORD,,
```

