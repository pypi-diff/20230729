# Comparing `tmp/pyTashriBS-0.1.tar.gz` & `tmp/pyTashriBS-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTashriBS-0.1.tar", last modified: Mon Jul  3 04:42:04 2023, max compression
+gzip compressed data, was "pyTashriBS-0.2.tar", last modified: Sat Jul 29 18:07:55 2023, max compression
```

## Comparing `pyTashriBS-0.1.tar` & `pyTashriBS-0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 04:42:04.002448 pyTashriBS-0.1/
--rw-rw-rw-   0        0        0    35149 2023-05-03 12:16:27.000000 pyTashriBS-0.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-03 04:42:03.981505 pyTashriBS-0.1/LegendBS/
--rw-rw-rw-   0        0        0        1 2023-07-03 02:57:45.000000 pyTashriBS-0.1/LegendBS/__init__.py
--rw-rw-rw-   0        0        0     6946 2023-07-03 02:57:45.000000 pyTashriBS-0.1/LegendBS/abuse.py
--rw-rw-rw-   0        0        0      745 2023-07-03 02:57:45.000000 pyTashriBS-0.1/LegendBS/banall.py
--rw-rw-rw-   0        0        0     2536 2023-07-03 02:57:45.000000 pyTashriBS-0.1/LegendBS/birthday.py
--rw-rw-rw-   0        0        0      369 2023-07-03 02:57:45.000000 pyTashriBS-0.1/LegendBS/error.py
--rw-rw-rw-   0        0        0      390 2023-07-03 02:57:45.000000 pyTashriBS-0.1/LegendBS/get_time.py
--rw-rw-rw-   0        0        0     2081 2023-07-03 02:57:45.000000 pyTashriBS-0.1/LegendBS/get_user.py
--rw-rw-rw-   0        0        0     1705 2023-07-03 02:57:45.000000 pyTashriBS-0.1/LegendBS/love.py
--rw-rw-rw-   0        0        0     3094 2023-07-03 02:57:45.000000 pyTashriBS-0.1/LegendBS/porn.py
--rw-rw-rw-   0        0        0    33658 2023-07-03 02:57:45.000000 pyTashriBS-0.1/LegendBS/raid.py
--rw-rw-rw-   0        0        0      899 2023-07-03 03:02:34.000000 pyTashriBS-0.1/LegendBS/start.py
--rw-rw-rw-   0        0        0     3028 2023-07-03 02:57:45.000000 pyTashriBS-0.1/LegendBS/start_bot.py
--rw-rw-rw-   0        0        0        1 2023-07-03 02:57:45.000000 pyTashriBS-0.1/LegendBS/start_help.py
--rw-rw-rw-   0        0        0     3528 2023-07-03 02:57:45.000000 pyTashriBS-0.1/LegendBS/startup.py
--rw-rw-rw-   0        0        0    17800 2023-07-03 02:57:45.000000 pyTashriBS-0.1/LegendBS/yup.py
--rw-rw-rw-   0        0        0     1001 2023-07-03 04:42:04.000452 pyTashriBS-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-05-03 12:16:27.000000 pyTashriBS-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 04:42:03.997462 pyTashriBS-0.1/pyTashriBS.egg-info/
--rw-rw-rw-   0        0        0     1001 2023-07-03 04:42:03.000000 pyTashriBS-0.1/pyTashriBS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2023-07-03 04:42:03.000000 pyTashriBS-0.1/pyTashriBS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 04:42:03.000000 pyTashriBS-0.1/pyTashriBS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-03 04:42:03.000000 pyTashriBS-0.1/pyTashriBS.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-03 04:42:03.000000 pyTashriBS-0.1/pyTashriBS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 04:42:04.003448 pyTashriBS-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1420 2023-07-03 04:39:04.000000 pyTashriBS-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 18:07:55.544377 pyTashriBS-0.2/
+-rw-rw-rw-   0        0        0    35149 2023-05-03 12:16:27.000000 pyTashriBS-0.2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-29 18:07:55.259235 pyTashriBS-0.2/LegendBS/
+-rw-rw-rw-   0        0        0        1 2023-07-03 02:57:45.000000 pyTashriBS-0.2/LegendBS/__init__.py
+-rw-rw-rw-   0        0        0     6946 2023-07-03 02:57:45.000000 pyTashriBS-0.2/LegendBS/abuse.py
+-rw-rw-rw-   0        0        0      745 2023-07-03 02:57:45.000000 pyTashriBS-0.2/LegendBS/banall.py
+-rw-rw-rw-   0        0        0     2536 2023-07-03 02:57:45.000000 pyTashriBS-0.2/LegendBS/birthday.py
+-rw-rw-rw-   0        0        0      369 2023-07-03 02:57:45.000000 pyTashriBS-0.2/LegendBS/error.py
+-rw-rw-rw-   0        0        0      390 2023-07-03 02:57:45.000000 pyTashriBS-0.2/LegendBS/get_time.py
+-rw-rw-rw-   0        0        0     2081 2023-07-03 02:57:45.000000 pyTashriBS-0.2/LegendBS/get_user.py
+-rw-rw-rw-   0        0        0     1705 2023-07-03 02:57:45.000000 pyTashriBS-0.2/LegendBS/love.py
+-rw-rw-rw-   0        0        0     3094 2023-07-03 02:57:45.000000 pyTashriBS-0.2/LegendBS/porn.py
+-rw-rw-rw-   0        0        0    33658 2023-07-03 02:57:45.000000 pyTashriBS-0.2/LegendBS/raid.py
+-rw-rw-rw-   0        0        0      899 2023-07-29 18:05:45.000000 pyTashriBS-0.2/LegendBS/start.py
+-rw-rw-rw-   0        0        0     3028 2023-07-03 02:57:45.000000 pyTashriBS-0.2/LegendBS/start_bot.py
+-rw-rw-rw-   0        0        0        1 2023-07-03 02:57:45.000000 pyTashriBS-0.2/LegendBS/start_help.py
+-rw-rw-rw-   0        0        0     3528 2023-07-03 02:57:45.000000 pyTashriBS-0.2/LegendBS/startup.py
+-rw-rw-rw-   0        0        0    17800 2023-07-03 02:57:45.000000 pyTashriBS-0.2/LegendBS/yup.py
+-rw-rw-rw-   0        0        0     1001 2023-07-29 18:07:55.545952 pyTashriBS-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-05-03 12:16:27.000000 pyTashriBS-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 18:07:55.472802 pyTashriBS-0.2/pyTashriBS.egg-info/
+-rw-rw-rw-   0        0        0     1001 2023-07-29 18:07:51.000000 pyTashriBS-0.2/pyTashriBS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      494 2023-07-29 18:07:51.000000 pyTashriBS-0.2/pyTashriBS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 18:07:51.000000 pyTashriBS-0.2/pyTashriBS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-29 18:07:51.000000 pyTashriBS-0.2/pyTashriBS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-29 18:07:51.000000 pyTashriBS-0.2/pyTashriBS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 18:07:55.553365 pyTashriBS-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1420 2023-07-29 18:06:19.000000 pyTashriBS-0.2/setup.py
```

### Comparing `pyTashriBS-0.1/LICENSE` & `pyTashriBS-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyTashriBS-0.1/LegendBS/abuse.py` & `pyTashriBS-0.2/LegendBS/abuse.py`

 * *Files identical despite different names*

### Comparing `pyTashriBS-0.1/LegendBS/banall.py` & `pyTashriBS-0.2/LegendBS/banall.py`

 * *Files identical despite different names*

### Comparing `pyTashriBS-0.1/LegendBS/birthday.py` & `pyTashriBS-0.2/LegendBS/birthday.py`

 * *Files identical despite different names*

### Comparing `pyTashriBS-0.1/LegendBS/get_user.py` & `pyTashriBS-0.2/LegendBS/get_user.py`

 * *Files identical despite different names*

### Comparing `pyTashriBS-0.1/LegendBS/love.py` & `pyTashriBS-0.2/LegendBS/love.py`

 * *Files identical despite different names*

### Comparing `pyTashriBS-0.1/LegendBS/porn.py` & `pyTashriBS-0.2/LegendBS/porn.py`

 * *Files identical despite different names*

### Comparing `pyTashriBS-0.1/LegendBS/raid.py` & `pyTashriBS-0.2/LegendBS/raid.py`

 * *Files identical despite different names*

### Comparing `pyTashriBS-0.1/LegendBS/start.py` & `pyTashriBS-0.2/LegendBS/start.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from pyrogram.types import InlineKeyboardButton
 
 async def start_cmd(Legend):
     x = await Legend.get_me()
     START_OP = [
         [
             InlineKeyboardButton(
-                text="🥀 Developer 🥀", url=f"https://t.me/Tashribots2342"
+                text="🥀 Developer 🥀", url=f"https://t.me/TashriBots"
             ),
             InlineKeyboardButton(
-                text="✨ Support ✨", url=f"https://t.me/TeamTashri"
+                text="✨ Support ✨", url=f"https://t.me/TashriChatting"
             ),
         ],
         [
             InlineKeyboardButton(
                 text="🧸 Add me in your group 🧸",
                 url=f"https://t.me/{x.username}?startgroup=true",
             ),
```

### Comparing `pyTashriBS-0.1/LegendBS/start_bot.py` & `pyTashriBS-0.2/LegendBS/start_bot.py`

 * *Files identical despite different names*

### Comparing `pyTashriBS-0.1/LegendBS/startup.py` & `pyTashriBS-0.2/LegendBS/startup.py`

 * *Files identical despite different names*

### Comparing `pyTashriBS-0.1/LegendBS/yup.py` & `pyTashriBS-0.2/LegendBS/yup.py`

 * *Files identical despite different names*

### Comparing `pyTashriBS-0.1/PKG-INFO` & `pyTashriBS-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTashriBS
-Version: 0.1
+Version: 0.2
 Summary: This is a simple package which is used in Spam Bot
 Home-page: https://github.com/Tashri2342/pyTashriBS
 Author: Tashri
 Author-email: Arunthakur2342@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyTashriBS,TashriBS
 Classifier: Framework :: AsyncIO
```

### Comparing `pyTashriBS-0.1/pyTashriBS.egg-info/PKG-INFO` & `pyTashriBS-0.2/pyTashriBS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTashriBS
-Version: 0.1
+Version: 0.2
 Summary: This is a simple package which is used in Spam Bot
 Home-page: https://github.com/Tashri2342/pyTashriBS
 Author: Tashri
 Author-email: Arunthakur2342@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyTashriBS,TashriBS
 Classifier: Framework :: AsyncIO
```

### Comparing `pyTashriBS-0.1/setup.py` & `pyTashriBS-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     sys.stderr.write( "Warning: Could not open README.md due %s\n" % error )
     
 
 setup(
     name="pyTashriBS",
     author="Tashri",
     author_email="Arunthakur2342@gmail.com",
-    version="0.1",
+    version="0.2",
     description="This is a simple package which is used in Spam Bot",
     long_description = readme_contents,
     long_description_content_type="text/markdown",
     url="https://github.com/Tashri2342/pyTashriBS",
     packages=find_packages(),
     license="GNU General Public License v3.0",
     include_package_data=True,
```

