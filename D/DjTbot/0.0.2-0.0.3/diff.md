# Comparing `tmp/DjTbot-0.0.2-py3-none-any.whl.zip` & `tmp/DjTbot-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 18380 bytes, number of entries: 34
+Zip file size: 19004 bytes, number of entries: 36
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-29 18:39 DjTbot/__init__.py
 -rw-rw-rw-  2.0 fat      375 b- defN 23-Jul-29 18:46 DjTbot/admin.py
 -rw-rw-rw-  2.0 fat      602 b- defN 23-Jul-29 18:46 DjTbot/arguments.py
 -rw-rw-rw-  2.0 fat     3146 b- defN 23-Jul-29 18:46 DjTbot/commands.py
 -rw-rw-rw-  2.0 fat      423 b- defN 23-Jul-29 18:02 DjTbot/models.py
 -rw-rw-rw-  2.0 fat     1866 b- defN 23-Jul-29 18:40 DjTbot/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-29 18:05 DjTbot/core/__init__.py
@@ -25,12 +25,14 @@
 -rw-rw-rw-  2.0 fat      497 b- defN 23-Jul-29 18:46 DjTbot/management/commands/removeuserfromgroup.py
 -rw-rw-rw-  2.0 fat      415 b- defN 23-Jul-29 18:46 DjTbot/management/commands/rmgroup.py
 -rw-rw-rw-  2.0 fat      414 b- defN 23-Jul-29 18:46 DjTbot/management/commands/rmuser.py
 -rw-rw-rw-  2.0 fat      824 b- defN 23-Jul-29 18:46 DjTbot/management/commands/runbot.py
 -rw-rw-rw-  2.0 fat     1769 b- defN 23-Jul-29 18:46 DjTbot/management/commands/sendmessage.py
 -rw-rw-rw-  2.0 fat      834 b- defN 23-Jul-29 18:14 DjTbot/management/migrations/0001_initial.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-29 18:14 DjTbot/management/migrations/__init__.py
--rw-rw-rw-  2.0 fat     5811 b- defN 23-Jul-29 18:59 DjTbot-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-29 18:59 DjTbot-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-29 18:59 DjTbot-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2890 b- defN 23-Jul-29 18:59 DjTbot-0.0.2.dist-info/RECORD
-34 files, 36258 bytes uncompressed, 13684 bytes compressed:  62.3%
+-rw-rw-rw-  2.0 fat      834 b- defN 23-Jul-29 18:14 DjTbot/migrations/0001_initial.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-29 18:14 DjTbot/migrations/__init__.py
+-rw-rw-rw-  2.0 fat     5811 b- defN 23-Jul-29 20:05 DjTbot-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-29 20:05 DjTbot-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-29 20:05 DjTbot-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     3062 b- defN 23-Jul-29 20:05 DjTbot-0.0.3.dist-info/RECORD
+36 files, 37264 bytes uncompressed, 14032 bytes compressed:  62.3%
```

## zipnote {}

```diff
@@ -84,20 +84,26 @@
 
 Filename: DjTbot/management/migrations/0001_initial.py
 Comment: 
 
 Filename: DjTbot/management/migrations/__init__.py
 Comment: 
 
-Filename: DjTbot-0.0.2.dist-info/METADATA
+Filename: DjTbot/migrations/0001_initial.py
 Comment: 
 
-Filename: DjTbot-0.0.2.dist-info/WHEEL
+Filename: DjTbot/migrations/__init__.py
 Comment: 
 
-Filename: DjTbot-0.0.2.dist-info/top_level.txt
+Filename: DjTbot-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: DjTbot-0.0.2.dist-info/RECORD
+Filename: DjTbot-0.0.3.dist-info/WHEEL
+Comment: 
+
+Filename: DjTbot-0.0.3.dist-info/top_level.txt
+Comment: 
+
+Filename: DjTbot-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `DjTbot-0.0.2.dist-info/METADATA` & `DjTbot-0.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DjTbot
-Version: 0.0.2
+Version: 0.0.3
 Summary: Django Telegram Bot
 Home-page: https://git.herrerosolis.com/bots/DjTbot
 Download-URL: https://git.herrerosolis.com/bots/DjTbot/-/archive/master/DjTbot-master.tar.gz
 Author: Rafael Herrero Solis
 Author-email: rafahsolis@hotmail.com
 License: License :: OSI Approved :: MIT License
 Keywords: Django,Telegram,Bot
```

## Comparing `DjTbot-0.0.2.dist-info/RECORD` & `DjTbot-0.0.3.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -24,11 +24,13 @@
 DjTbot/management/commands/removeuserfromgroup.py,sha256=O7Hph7x_zvW0c773D294NjPKUPoBW_AHbeQWmNBozoA,497
 DjTbot/management/commands/rmgroup.py,sha256=jX7B-X8Y4Sf3dVr36xOBkH5LmQLOrzqK5GUkUrLbHlk,415
 DjTbot/management/commands/rmuser.py,sha256=ErQAGmja0mjUJUAhZ-tQu9FhJDvvkJV7cgEKnR_RM20,414
 DjTbot/management/commands/runbot.py,sha256=0FJJw8msloruVqVgpTZPcgGHRnqPEthxUNvkUf14ECg,824
 DjTbot/management/commands/sendmessage.py,sha256=jQRnGAjA9FnXhG7Zmyp8t6ls4xSkpjBNCY57rZhH1r0,1769
 DjTbot/management/migrations/0001_initial.py,sha256=GVM4LdsOGVHOwvL7CYpfy4ssYpSqFK0wnwjfSRt25Kg,834
 DjTbot/management/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-DjTbot-0.0.2.dist-info/METADATA,sha256=x_Z2d691WKsnjp3-8fckWPdIaEICPEB8UKRxr2fogOE,5811
-DjTbot-0.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-DjTbot-0.0.2.dist-info/top_level.txt,sha256=EPHNGmErmeMSdx4xASLhwqtKotkt-_WHnJFxZZSQ4rI,7
-DjTbot-0.0.2.dist-info/RECORD,,
+DjTbot/migrations/0001_initial.py,sha256=GVM4LdsOGVHOwvL7CYpfy4ssYpSqFK0wnwjfSRt25Kg,834
+DjTbot/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+DjTbot-0.0.3.dist-info/METADATA,sha256=2ytce8cMY0zJZUAYfLIVJXud2KCjoQIrXNrvL7AB94s,5811
+DjTbot-0.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+DjTbot-0.0.3.dist-info/top_level.txt,sha256=EPHNGmErmeMSdx4xASLhwqtKotkt-_WHnJFxZZSQ4rI,7
+DjTbot-0.0.3.dist-info/RECORD,,
```

