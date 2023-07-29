# Comparing `tmp/tweety-ns-0.9.tar.gz` & `tmp/tweety-ns-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweety-ns-0.9.tar", last modified: Mon Jul 17 19:34:08 2023, max compression
+gzip compressed data, was "tweety-ns-0.9.5.tar", last modified: Sat Jul 29 16:09:33 2023, max compression
```

## Comparing `tweety-ns-0.9.tar` & `tweety-ns-0.9.5.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 19:34:08.046963 tweety-ns-0.9/
--rw-rw-rw-   0        0        0     1855 2023-07-17 19:34:08.046963 tweety-ns-0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1146 2023-07-05 12:23:35.000000 tweety-ns-0.9/README.md
--rw-rw-rw-   0        0        0      108 2021-11-15 09:32:36.000000 tweety-ns-0.9/pyproject.toml
--rw-rw-rw-   0        0        0      699 2023-07-17 19:34:08.047964 tweety-ns-0.9/setup.cfg
--rw-rw-rw-   0        0        0      800 2023-07-17 19:33:28.000000 tweety-ns-0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:34:07.997765 tweety-ns-0.9/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 19:34:08.021878 tweety-ns-0.9/src/tweety/
--rw-rw-rw-   0        0        0      230 2023-07-17 19:33:40.000000 tweety-ns-0.9/src/tweety/__init__.py
--rw-rw-rw-   0        0        0     2316 2023-07-17 19:22:53.000000 tweety-ns-0.9/src/tweety/auth.py
--rw-rw-rw-   0        0        0    10760 2023-07-17 18:55:39.000000 tweety-ns-0.9/src/tweety/bot.py
--rw-rw-rw-   0        0        0    30770 2023-07-17 19:26:27.000000 tweety-ns-0.9/src/tweety/builder.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:34:08.025777 tweety-ns-0.9/src/tweety/events/
--rw-rw-rw-   0        0        0       42 2023-07-04 06:05:54.000000 tweety-ns-0.9/src/tweety/events/__init__.py
--rw-rw-rw-   0        0        0     1768 2023-07-04 10:00:32.000000 tweety-ns-0.9/src/tweety/events/newmessage.py
--rw-rw-rw-   0        0        0    18741 2023-07-17 19:02:14.000000 tweety-ns-0.9/src/tweety/exceptions_.py
--rw-rw-rw-   0        0        0      282 2022-03-04 06:53:48.000000 tweety-ns-0.9/src/tweety/filters.py
--rw-rw-rw-   0        0        0     6829 2023-07-17 19:02:14.000000 tweety-ns-0.9/src/tweety/http.py
--rw-rw-rw-   0        0        0     1257 2023-07-09 18:45:36.000000 tweety-ns-0.9/src/tweety/session.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:34:08.036784 tweety-ns-0.9/src/tweety/types/
--rw-rw-rw-   0        0        0       58 2023-03-12 12:43:32.000000 tweety-ns-0.9/src/tweety/types/__init__.py
--rw-rw-rw-   0        0        0     9218 2023-07-05 09:26:20.000000 tweety-ns-0.9/src/tweety/types/inbox.py
--rw-rw-rw-   0        0        0     2631 2023-07-03 12:56:12.000000 tweety-ns-0.9/src/tweety/types/mentions.py
--rw-rw-rw-   0        0        0     3858 2023-07-17 19:07:38.000000 tweety-ns-0.9/src/tweety/types/n_types.py
--rw-rw-rw-   0        0        0     4325 2023-07-13 14:34:32.000000 tweety-ns-0.9/src/tweety/types/search.py
--rw-rw-rw-   0        0        0    30235 2023-07-09 18:41:29.000000 tweety-ns-0.9/src/tweety/types/twDataTypes.py
--rw-rw-rw-   0        0        0     3873 2023-07-05 07:09:50.000000 tweety-ns-0.9/src/tweety/types/usertweet.py
--rw-rw-rw-   0        0        0      483 2023-07-09 19:15:04.000000 tweety-ns-0.9/src/tweety/updates.py
--rw-rw-rw-   0        0        0      677 2023-07-04 06:34:07.000000 tweety-ns-0.9/src/tweety/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:34:08.044963 tweety-ns-0.9/src/tweety_ns.egg-info/
--rw-rw-rw-   0        0        0     1855 2023-07-17 19:34:07.000000 tweety-ns-0.9/src/tweety_ns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      703 2023-07-17 19:34:07.000000 tweety-ns-0.9/src/tweety_ns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 19:34:07.000000 tweety-ns-0.9/src/tweety_ns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-17 19:34:07.000000 tweety-ns-0.9/src/tweety_ns.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-17 19:34:07.000000 tweety-ns-0.9/src/tweety_ns.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 16:09:33.962332 tweety-ns-0.9.5/
+-rw-rw-rw-   0        0        0     1799 2023-07-29 16:09:33.962332 tweety-ns-0.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1088 2023-07-29 16:03:36.000000 tweety-ns-0.9.5/README.md
+-rw-rw-rw-   0        0        0      108 2021-11-15 09:32:36.000000 tweety-ns-0.9.5/pyproject.toml
+-rw-rw-rw-   0        0        0      701 2023-07-29 16:09:33.963234 tweety-ns-0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0      785 2023-07-29 16:02:59.000000 tweety-ns-0.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:09:33.924231 tweety-ns-0.9.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-29 16:09:33.942231 tweety-ns-0.9.5/src/tweety/
+-rw-rw-rw-   0        0        0      276 2023-07-29 16:03:51.000000 tweety-ns-0.9.5/src/tweety/__init__.py
+-rw-rw-rw-   0        0        0     3251 2023-07-27 17:28:49.000000 tweety-ns-0.9.5/src/tweety/auth.py
+-rw-rw-rw-   0        0        0     8655 2023-07-28 18:14:21.000000 tweety-ns-0.9.5/src/tweety/bot.py
+-rw-rw-rw-   0        0        0    38979 2023-07-28 18:07:04.000000 tweety-ns-0.9.5/src/tweety/builder.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:09:33.944257 tweety-ns-0.9.5/src/tweety/events/
+-rw-rw-rw-   0        0        0       42 2023-07-04 06:05:54.000000 tweety-ns-0.9.5/src/tweety/events/__init__.py
+-rw-rw-rw-   0        0        0     1768 2023-07-04 10:00:32.000000 tweety-ns-0.9.5/src/tweety/events/newmessage.py
+-rw-rw-rw-   0        0        0    19256 2023-07-29 08:49:51.000000 tweety-ns-0.9.5/src/tweety/exceptions_.py
+-rw-rw-rw-   0        0        0      635 2023-07-27 17:30:57.000000 tweety-ns-0.9.5/src/tweety/filters.py
+-rw-rw-rw-   0        0        0     7986 2023-07-29 14:39:05.000000 tweety-ns-0.9.5/src/tweety/http.py
+-rw-rw-rw-   0        0        0     1510 2023-07-26 20:41:00.000000 tweety-ns-0.9.5/src/tweety/session.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:09:33.956253 tweety-ns-0.9.5/src/tweety/types/
+-rw-rw-rw-   0        0        0      331 2023-07-27 10:28:18.000000 tweety-ns-0.9.5/src/tweety/types/__init__.py
+-rw-rw-rw-   0        0        0      951 2023-07-29 12:04:19.000000 tweety-ns-0.9.5/src/tweety/types/base.py
+-rw-rw-rw-   0        0        0     2741 2023-07-29 12:16:19.000000 tweety-ns-0.9.5/src/tweety/types/bookmarks.py
+-rw-rw-rw-   0        0        0     9347 2023-07-29 12:16:19.000000 tweety-ns-0.9.5/src/tweety/types/inbox.py
+-rw-rw-rw-   0        0        0     1823 2023-07-29 14:23:48.000000 tweety-ns-0.9.5/src/tweety/types/mentions.py
+-rw-rw-rw-   0        0        0     6573 2023-07-28 18:32:05.000000 tweety-ns-0.9.5/src/tweety/types/n_types.py
+-rw-rw-rw-   0        0        0     3982 2023-07-29 14:23:48.000000 tweety-ns-0.9.5/src/tweety/types/search.py
+-rw-rw-rw-   0        0        0    29877 2023-07-29 14:44:19.000000 tweety-ns-0.9.5/src/tweety/types/twDataTypes.py
+-rw-rw-rw-   0        0        0     3172 2023-07-29 14:23:48.000000 tweety-ns-0.9.5/src/tweety/types/usertweet.py
+-rw-rw-rw-   0        0        0      483 2023-07-09 19:15:04.000000 tweety-ns-0.9.5/src/tweety/updates.py
+-rw-rw-rw-   0        0        0     6463 2023-07-29 11:00:08.000000 tweety-ns-0.9.5/src/tweety/user.py
+-rw-rw-rw-   0        0        0     3102 2023-07-28 18:30:16.000000 tweety-ns-0.9.5/src/tweety/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:09:33.961230 tweety-ns-0.9.5/src/tweety_ns.egg-info/
+-rw-rw-rw-   0        0        0     1799 2023-07-29 16:09:33.000000 tweety-ns-0.9.5/src/tweety_ns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      777 2023-07-29 16:09:33.000000 tweety-ns-0.9.5/src/tweety_ns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 16:09:33.000000 tweety-ns-0.9.5/src/tweety_ns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-29 16:09:33.000000 tweety-ns-0.9.5/src/tweety_ns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-29 16:09:33.000000 tweety-ns-0.9.5/src/tweety_ns.egg-info/top_level.txt
```

### Comparing `tweety-ns-0.9/PKG-INFO` & `tweety-ns-0.9.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 0.9
+Version: 0.9.5
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
@@ -14,45 +14,44 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # tweety
-Twitter's API is annoying to work with, and has lots of limitations — luckily their frontend (JavaScript) has it's own API, which I reverse–engineered. No API rate limits. No restrictions. Extremely fast.
+Twitter's API is annoying to work with, and has lots of limitations — luckily their frontend (JavaScript) has it's own API, which I reverse–engineered. xtremely fast.
 
 [![Downloads](https://static.pepy.tech/personalized-badge/tweety-ns?period=total&units=international_system&left_color=orange&right_color=blue&left_text=Downloads)](https://pepy.tech/project/tweety-ns)
 ## Prerequisites
 
 Before you begin, ensure you have met the following requirements:
 
 * Internet Connection
 * Python 3.6+
 * httpx 
 * openpyxl
-* tqdm
 
 ## Installation: 
 ```bash
 pip install tweety-ns
 ```
 
 ## Keep synced with latest fixes
 
 ##### **Pip might not be always updated , so to keep everything synced.**
 
 ```bash
-pip install https://github.com/mahrtayyab/tweety/archive/main.zip --upgrade --force-reinstall
+pip install https://github.com/mahrtayyab/tweety/archive/main.zip --upgrade 
 ```
 
 ## A Quick Example:
 ```python
-  from tweety.bot import Twitter
+  from tweety import Twitter
   
-  app = Twitter()
+  app = Twitter("session")
   
   all_tweets = app.get_tweets("elonmusk")
   for tweet in all_tweets:
       print(tweet)
 ```
 
 Full Documentation and Changelogs are [here](https://mahrtayyab.github.io/tweety_docs/)
```

### Comparing `tweety-ns-0.9/README.md` & `tweety-ns-0.9.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # tweety
-Twitter's API is annoying to work with, and has lots of limitations — luckily their frontend (JavaScript) has it's own API, which I reverse–engineered. No API rate limits. No restrictions. Extremely fast.
+Twitter's API is annoying to work with, and has lots of limitations — luckily their frontend (JavaScript) has it's own API, which I reverse–engineered. xtremely fast.
 
 [![Downloads](https://static.pepy.tech/personalized-badge/tweety-ns?period=total&units=international_system&left_color=orange&right_color=blue&left_text=Downloads)](https://pepy.tech/project/tweety-ns)
 ## Prerequisites
 
 Before you begin, ensure you have met the following requirements:
 
 * Internet Connection
 * Python 3.6+
 * httpx 
 * openpyxl
-* tqdm
 
 ## Installation: 
 ```bash
 pip install tweety-ns
 ```
 
 ## Keep synced with latest fixes
 
 ##### **Pip might not be always updated , so to keep everything synced.**
 
 ```bash
-pip install https://github.com/mahrtayyab/tweety/archive/main.zip --upgrade --force-reinstall
+pip install https://github.com/mahrtayyab/tweety/archive/main.zip --upgrade 
 ```
 
 ## A Quick Example:
 ```python
-  from tweety.bot import Twitter
+  from tweety import Twitter
   
-  app = Twitter()
+  app = Twitter("session")
   
   all_tweets = app.get_tweets("elonmusk")
   for tweet in all_tweets:
       print(tweet)
 ```
 
 Full Documentation and Changelogs are [here](https://mahrtayyab.github.io/tweety_docs/)
```

### Comparing `tweety-ns-0.9/setup.cfg` & `tweety-ns-0.9.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 7765 6574 792d 6e73 0d0a 7665   = tweety-ns..ve
-00000020: 7273 696f 6e20 3d20 302e 390d 0a61 7574  rsion = 0.9..aut
-00000030: 686f 7220 3d20 5461 7979 6162 204b 6861  hor = Tayyab Kha
-00000040: 726c 0d0a 6175 7468 6f72 5f65 6d61 696c  rl..author_email
-00000050: 203d 2074 6179 7961 626d 6168 7240 676d   = tayyabmahr@gm
-00000060: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
-00000070: 7469 6f6e 203d 2041 6e20 6561 7379 2054  tion = An easy T
-00000080: 7769 7474 6572 2053 6372 6170 6572 0d0a  witter Scraper..
-00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000a0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
-000000b0: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
-000000c0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
-000000d0: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
-000000e0: 6e0d 0a75 726c 203d 2068 7474 7073 3a2f  n..url = https:/
-000000f0: 2f67 6974 6875 622e 636f 6d2f 6d61 6872  /github.com/mahr
-00000100: 7461 7979 6162 2f74 7765 6574 790d 0a70  tayyab/tweety..p
-00000110: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
-00000120: 0942 7567 2054 7261 636b 6572 203d 2068  .Bug Tracker = h
-00000130: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000140: 6d2f 6d61 6872 7461 7979 6162 2f74 7765  m/mahrtayyab/twe
-00000150: 6574 792f 6973 7375 6573 0d0a 0944 6f63  ety/issues...Doc
-00000160: 756d 656e 7461 7469 6f6e 203d 2068 7474  umentation = htt
-00000170: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000180: 6d61 6872 7461 7979 6162 2f74 7765 6574  mahrtayyab/tweet
-00000190: 790d 0a63 6c61 7373 6966 6965 7273 203d  y..classifiers =
-000001a0: 200d 0a09 5072 6f67 7261 6d6d 696e 6720   ...Programming 
-000001b0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000001c0: 6f6e 203a 3a20 330d 0a09 4c69 6365 6e73  on :: 3...Licens
-000001d0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-000001e0: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
-000001f0: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
-00000200: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
-00000210: 6e64 656e 740d 0a0d 0a5b 6f70 7469 6f6e  ndent....[option
-00000220: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
-00000230: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
-00000240: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
-00000250: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-00000260: 3e3d 332e 360d 0a0d 0a5b 6f70 7469 6f6e  >=3.6....[option
-00000270: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
-00000280: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
-00000290: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-000002a0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-000002b0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000020: 7273 696f 6e20 3d20 302e 392e 350d 0a61  rsion = 0.9.5..a
+00000030: 7574 686f 7220 3d20 5461 7979 6162 204b  uthor = Tayyab K
+00000040: 6861 726c 0d0a 6175 7468 6f72 5f65 6d61  harl..author_ema
+00000050: 696c 203d 2074 6179 7961 626d 6168 7240  il = tayyabmahr@
+00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
+00000070: 6970 7469 6f6e 203d 2041 6e20 6561 7379  iption = An easy
+00000080: 2054 7769 7474 6572 2053 6372 6170 6572   Twitter Scraper
+00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+000000a0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
+000000b0: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
+000000c0: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
+000000d0: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
+000000e0: 6f77 6e0d 0a75 726c 203d 2068 7474 7073  own..url = https
+000000f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d61  ://github.com/ma
+00000100: 6872 7461 7979 6162 2f74 7765 6574 790d  hrtayyab/tweety.
+00000110: 0a70 726f 6a65 6374 5f75 726c 7320 3d20  .project_urls = 
+00000120: 0d0a 0942 7567 2054 7261 636b 6572 203d  ...Bug Tracker =
+00000130: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000140: 636f 6d2f 6d61 6872 7461 7979 6162 2f74  com/mahrtayyab/t
+00000150: 7765 6574 792f 6973 7375 6573 0d0a 0944  weety/issues...D
+00000160: 6f63 756d 656e 7461 7469 6f6e 203d 2068  ocumentation = h
+00000170: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000180: 6d2f 6d61 6872 7461 7979 6162 2f74 7765  m/mahrtayyab/twe
+00000190: 6574 790d 0a63 6c61 7373 6966 6965 7273  ety..classifiers
+000001a0: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
+000001b0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000001c0: 7468 6f6e 203a 3a20 340d 0a09 4c69 6365  thon :: 4...Lice
+000001d0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+000001e0: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+000001f0: 7365 0d0a 094f 7065 7261 7469 6e67 2053  se...Operating S
+00000200: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
+00000210: 7065 6e64 656e 740d 0a0d 0a5b 6f70 7469  pendent....[opti
+00000220: 6f6e 735d 0d0a 7061 636b 6167 655f 6469  ons]..package_di
+00000230: 7220 3d20 0d0a 093d 2073 7263 0d0a 7061  r = ...= src..pa
+00000240: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
+00000250: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
+00000260: 3d20 3e3d 332e 360d 0a0d 0a5b 6f70 7469  = >=3.6....[opti
+00000270: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+00000280: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
+00000290: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+000002a0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+000002b0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `tweety-ns-0.9/setup.py` & `tweety-ns-0.9.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from distutils.core import setup
 
 setup(
     name='tweety-ns',
     packages=['tweety', 'tweety.types', 'tweety.events'],
-    version='0.9',
+    version='0.9.5',
     license='MIT',
     description='An easy Twitter Scraper',
     author='Tayyab Kharl',
     author_email='tayyabmahr@gmail.com',
     url='https://github.com/mahrtayyab/tweety',
     keywords=['TWITTER', 'TWITTER SCRAPE', 'SCRAPE TWEETS'],
     install_requires=[
         'beautifulsoup4',
         'openpyxl',
         'httpx',
         'dateutils',
-        'tqdm',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3'
```

### Comparing `tweety-ns-0.9/src/tweety/auth.py` & `tweety-ns-0.9.5/src/tweety/auth.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,54 @@
-from .exceptions_ import InvalidCredentials
+from http.cookiejar import MozillaCookieJar
+from .exceptions_ import InvalidCredentials, DeniedLogin
 from .builder import FlowData
 from .types.n_types import Cookies
 
 
 class AuthMethods:
 
     def connect(self):
+        """
+        This method will be used to connect to already saved session in disk
+        """
         if self.session.logged_in:
             self.request.set_cookies(str(self.session))
             self.user = self.get_user_info(self.request.username)
             self.session.set_session_user(self.user)
             self._is_connected = True
             return
 
     def sign_in(self, username, password, *, extra=None):
+        """
+        - This method can be used to sign in to Twitter using username and password
+        - It will also check for the saved session for the username in the disk
+
+        :param username: (`str`) Username of the user
+        :param password: (`str`) Password of the user
+        :param extra: ## NotImplemented
+        :return:
+        """
         if self.session.logged_in and self.session.user['username'] == username:
             try:
                 return self.connect()
             except InvalidCredentials:
                 pass
 
         _username = username
         _password = password
         _extra = extra
         self._login(_username, _password, _extra)
 
-    def load_cookies(self, cookies: [str, dict]):
+    def load_cookies(self, cookies: [str, dict, MozillaCookieJar]):
+        """
+        This method can be used to load the already authenticated cookies from Twitter
+
+        :param cookies:  (`str`, `dict`, `MozillaCookieJar`) The Cookies to load
+        :return:
+        """
         self.cookies = Cookies(cookies, False)
         self.logged_in = True
         self.session.save_session(self.cookies)
         self.connect()
 
     def _login(self, _username, _password, _extra):
         __login_url = "https://api.twitter.com/1.1/onboarding/task.json?flow_name=login"
@@ -47,12 +66,17 @@
                     self.logged_in = True
                     self.cookies = Cookies(response.headers['set-cookie'], True)
                     self.session.save_session(self.cookies)
                     self.connect()
                     return
                 __login_payload = __login_flow.get(__login_flow_state, json_=json_, username=_username, password=_password)
             else:
-                raise ValueError(response.text)
+                raise DeniedLogin(
+                    error_code=37,
+                    error_name="GenericAccessDenied",
+                    response=None,
+                    message=response.text
+                )
```

### Comparing `tweety-ns-0.9/src/tweety/bot.py` & `tweety-ns-0.9.5/src/tweety/bot.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 import functools
 import re
-from typing import Union
+from typing import Union, Generator
 
-from .types.n_types import Proxy
+from .types import Proxy, UserTweets, Search, User, Tweet, Trends
 from .exceptions_ import *
 from .session import Session
 from .http import Request
-from .types.usertweet import UserTweets
-from .types.search import Search
-from .types.mentions import Mention
-from .types.inbox import Inbox, SendMessage
-from .types.twDataTypes import User, Trends, Tweet
-from .utils import create_conversation_id
 
 
 def AuthRequired(f):
     @functools.wraps(f)
     def wrapper(self, *args, **kwargs):
         if self.user is None:
             raise AuthenticationRequired(200, "GenericForbidden", None)
@@ -33,66 +27,60 @@
         :param session_name: (`str`, `Session`) This is the name of the session which will be saved and can be loaded later
         :param proxy: (`dict` or `Proxy`) Provide the proxy you want to use while making a request
         """
 
         self._event_builders = []
         self.session = Session(session_name) if isinstance(session_name, str) else session_name
         self.logged_in = False
-        self.request = Request(max_retries=10, proxy=proxy)
+        self._proxy = proxy.get_dict() if isinstance(proxy, Proxy) else proxy
+        self.request = Request(max_retries=10, proxy=self._proxy)
         self.user = None
 
-    def get_user_info(self, username: str = None, banner_extensions: bool = False, image_extensions: bool = False):
+    def get_user_info(self, username: str = None) -> User:
         """
         Get the User Info of the specified username
 
         :param username: (`str`) username to get information of
-        :param banner_extensions: (`boolean`) Get the Banner extension on the user page
-        :param image_extensions: (`boolean`) Get the Image extension on the user page
 
         :return: .types.twDataTypes.User
         """
 
         user_raw = self.request.get_user(username)
 
-        if not banner_extensions or banner_extensions is False:
-            try:
-                del user_raw['data']['user']['result']['legacy']['profile_banner_extensions']
-            except KeyError:
-                pass
-
-        if not image_extensions or image_extensions is False:
-            try:
-                del user_raw['data']['user']['result']['legacy']['profile_image_extensions']
-            except KeyError:
-                pass
-
         return User(user_raw['data']['user']['result'])
 
     @property
-    def user_id(self):
+    def user_id(self) -> int:
         """
         Get the user unique twitter id
 
         :return: int
         """
         return self.user.id if self.user else None
 
-    def _get_user_id(self, username):
+    def _get_user_id(self, username) -> int:
         if isinstance(username, User):
-            user_id = username.rest_id
+            user_id = username.id
         elif isinstance(username, int):
             user_id = username
         elif isinstance(username, str) and str(username).isdigit():
             user_id = int(username)
         else:
-            user_id = self.get_user_info(username).rest_id
+            user_id = self.get_user_info(username).id
 
         return user_id
 
-    def get_tweets(self, username: Union[str, int, User], pages: int = 1, replies: bool = False, wait_time: int = 2, cursor: str = None):
+    def get_tweets(
+            self,
+            username: Union[str, int, User],
+            pages: int = 1,
+            replies: bool = False,
+            wait_time: int = 2,
+            cursor: str = None
+    ) -> UserTweets:
         """
          Get the tweets from a user
 
         :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
         :param: pages: (`int`) number of pages to be scraped
         :param: replies: (`boolean`) get the replied tweets of the user too
         :param: wait_time: (`int`) seconds to wait between multiple requests
@@ -103,20 +91,27 @@
         if wait_time is None:
             wait_time = 0
 
         user_id = self._get_user_id(username)
 
         userTweets = UserTweets(user_id, self.request, pages, replies, wait_time, cursor)
 
-        # TODO : Find proper way to run the generator
-        results = [i for i in userTweets.generator()]
+        results = list(userTweets.generator())
 
         return userTweets
 
-    def iter_tweets(self,  username: Union[str, int, User], pages: int = 1, replies: bool = False, wait_time: int = 2, cursor: str = None):
+    def iter_tweets(
+            self,
+            username: Union[str, int, User],
+            pages: int = 1,
+            replies: bool = False,
+            wait_time: int = 2,
+            cursor: str = None
+    ):
+
         """
          Generator for getting the tweets from a user
 
         :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
         :param: pages: (`int`) number of pages to be scraped
         :param: replies: (`boolean`) get the replied tweets of the user too
         :param: wait_time: (`int`) seconds to wait between multiple requests
@@ -152,15 +147,23 @@
                 if i['item']['content']['trend']['trendMetadata']['metaDescription']:
                     data['tweet_count'] = i['item']['content']['trend']['trendMetadata']['metaDescription']
             except:
                 pass
             trends.append(Trends(data))
         return trends
 
-    def search(self, keyword: str, pages: int = 1, filter_: str = None, wait_time: int = 2, cursor: str = None):
+    def search(
+            self,
+            keyword: str,
+            pages: int = 1,
+            filter_: str = None,
+            wait_time: int = 2,
+            cursor: str = None
+    ) -> Search:
+
         """
         Search for a keyword or hashtag on Twitter
 
         :param keyword: (`str`) The keyword which is supposed to be searched
         :param pages: (`int`) The number of pages to get
         :param filter_: (
            `str`| `filters.SearchFilters.Users()`| `filters.SearchFilters.Latest()` | `filters.SearchFilters.Photos()` | `filters.SearchFilters.Videos()`
@@ -172,20 +175,26 @@
         :return: .types.search.Search | if iter: (.types.search.Search, list[.types.twDataTypes.Tweet])
         """
         if wait_time is None:
             wait_time = 0
 
         search = Search(keyword, self.request, pages, filter_, wait_time, cursor)
 
-        # TODO : Find proper way to run the generator
-        results = [i for i in search.generator()]
+        results = list(search.generator())
 
         return search
 
-    def iter_search(self, keyword: str, pages: int = 1, filter_: str = None, wait_time: int = 2, cursor: str = None):
+    def iter_search(
+            self,
+            keyword: str,
+            pages: int = 1,
+            filter_: str = None,
+            wait_time: int = 2,
+            cursor: str = None
+    ):
         """
         Search for a keyword or hashtag on Twitter
 
         :param keyword: (`str`) The keyword which is supposed to be searched
         :param pages: (`int`) The number of pages to get
         :param filter_: (
            `str`| `filters.SearchFilters.Users()`| `filters.SearchFilters.Latest()` | `filters.SearchFilters.Photos()` | `filters.SearchFilters.Videos()`
@@ -199,52 +208,15 @@
         if wait_time is None:
             wait_time = 0
 
         search = Search(keyword, self.request, pages, filter_, wait_time, cursor)
 
         return search.generator()
 
-    def get_mentions(self, pages: int = 1, wait_time: int = 2, cursor: str = None):
-        """
-
-        :param pages: (`int`) The number of pages to get
-        :param wait_time: (`int`) seconds to wait between multiple requests
-        :param cursor: (`str`) Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-        :return:
-        """
-
-        if wait_time is None:
-            wait_time = 0
-
-        mentions = Mention(self.user.id, self.request, pages, wait_time, cursor)
-        results = [i for i in mentions.generator()]
-
-        return mentions
-
-    def get_inbox(self, user_id: Union[int, str, User] = None, cursor: str = None):
-        """
-        :param user_id : (`str`, `int`, `User`) User id or username of the user whom to get the messages of. Default is ALL
-        :param cursor: (`str`) Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-                                It is used to get the messages updates
-        :return:
-        """
-
-        if user_id:
-            user_id = self._get_user_id(user_id)
-
-        inbox = Inbox(user_id, self.request, cursor)
-
-        return inbox
-
-    def send_message(self, username: Union[str, int, User], text: str):
-        user_id = self._get_user_id(username)
-        conversation_id = create_conversation_id(self.user.id, user_id)
-        return SendMessage(self.request, conversation_id, text).send()
-
-    def tweet_detail(self, identifier: str):
+    def tweet_detail(self, identifier: str) -> Tweet:
         """
         Get Detail of a single tweet
 
         :param identifier: (`str`) The unique identifier of the tweet , either the `Tweet id` or `Tweet Link`
 
         :return: .types.twDataTypes.Tweet
         """
```

### Comparing `tweety-ns-0.9/src/tweety/builder.py` & `tweety-ns-0.9.5/src/tweety/builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import json
 from urllib.parse import urlencode
 import random
-import string
+from .exceptions_ import DeniedLogin
+from . import utils
 from functools import wraps
 
 REQUEST_USER_AGENT = 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36'
 REQUEST_PLATFORMS = ['Linux', 'Windows']
 
 
 def return_with_headers(func):
     @wraps(func)
     def wrapper(self, *arg, **kw):
-        method, url = func(self, *arg, **kw)
-        return dict(method=method, headers=self._get_headers(), url=url)
+        request_data = func(self, *arg, **kw)
+        if len(request_data) == 2:
+            return dict(method=request_data[0], headers=self._get_headers(), url=request_data[1])
+        else:
+            return dict(method=request_data[0], headers=self._get_headers(), url=request_data[1], json=request_data[2])
 
     return wrapper
 
 
 class UrlBuilder:
     URL_GUEST_TOKEN = "https://api.twitter.com/1.1/guest/activate.json"
     URL_API_INIT = "https://twitter.com/i/api/1.1/branch/init.json"
@@ -28,14 +32,18 @@
     URL_TWEET_DETAILS = "https://twitter.com/i/api/graphql/3XDB26fBve-MmjHaWTUZxA/TweetDetail"
     URL_AUSER_INBOX = "https://twitter.com/i/api/1.1/dm/user_updates.json"  # noqa
     URL_AUSER_TRUSTED_INBOX = "https://twitter.com/i/api/1.1/dm/inbox_timeline/trusted.json"  # noqa
     URL_AUSER_NOTIFICATION_MENTIONS = "https://twitter.com/i/api/2/notifications/mentions.json"  # noqa
     URL_AUSER_SETTINGS = "https://api.twitter.com/1.1/account/settings.json"  # noqa
     URL_AUSER_SEND_MESSAGE = "https://twitter.com/i/api/1.1/dm/new2.json"  # noqa
     URL_AUSER_CONVERSATION = "https://twitter.com/i/api/1.1/dm/conversation/{}.json"  # noqa
+    URL_AUSER_CREATE_TWEET = "https://twitter.com/i/api/graphql/tTsjMKyhajZvK4q76mpIBg/CreateTweet"  # noqa
+    URL_AUSER_CREATE_MEDIA = "https://upload.twitter.com/i/media/upload.json"  # noqa
+    URL_AUSER_CREATE_MEDIA_METADATA = "https://twitter.com/i/api/1.1/media/metadata/create.json"  # noqa
+    URL_AUSER_BOOKMARK = "https://twitter.com/i/api/graphql/bN6kl72VsPDRIGxDIhVu7A/Bookmarks"  # noqa
 
     def __init__(self):
         self.cookies = None
         self.user_id = None
         self.guest_token = None
 
     def set_cookies(self, cookies):
@@ -50,47 +58,47 @@
                 if len(split_cookie) == 2:
                     key = cookie.split("=")[0]
                     value = cookie.split("=")[1]
                     self.cookies[key] = value
 
     def _get_headers(self):
         headers = {
-            'authority': 'twitter.com',
-            'accept': '*/*',
-            'accept-language': 'en-PK,en;q=0.9',
-            'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
-            'content-type': 'application/x-www-form-urlencoded',
-            'referer': 'https://twitter.com/',
-            'sec-ch-ua': '"Not_A Brand";v="99", "Google Chrome";v="109", "Chromium";v="109"',
-            'sec-ch-ua-mobile': '?0',
-            'sec-ch-ua-platform': f'"{random.choice(REQUEST_PLATFORMS)}"',
-            'sec-fetch-dest': 'empty',
-            'sec-fetch-mode': 'cors',
-            'sec-fetch-site': 'same-site',
-            'user-agent': REQUEST_USER_AGENT,
-            'x-csrf-token': self._get_csrf(),
-            'x-twitter-active-user': 'yes',
-            'x-twitter-client-language': 'en',
+            # 'Authority': 'twitter.com',
+            'Accept': '*/*',
+            'Accept-Language': 'en-PK,en;q=0.9',
+            'Authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
+            'Content-Type': 'application/x-www-form-urlencoded',
+            'Referer': 'https://twitter.com/',
+            'Sec-Ch-Ua': '"Not_A Brand";v="99", "Google Chrome";v="109", "Chromium";v="109"',
+            'Sec-Ch-Ua-Mobile': '?0',
+            'Sec-Ch-Ua-Platform': f'"{random.choice(REQUEST_PLATFORMS)}"',
+            'Sec-Fetch-Dest': 'empty',
+            'Sec-Fetch-Mode': 'cors',
+            'Sec-Fetch-Site': 'same-site',
+            'User-Agent': REQUEST_USER_AGENT,
+            'X-Csrf-Token': self._get_csrf(),
+            'X-Twitter-Active-User': 'yes',
+            'X-Twitter-Client-Language': 'en',
         }
 
         if self.guest_token or self.cookies:
-            headers['content-type'] = 'application/json'
+            headers['Content-Type'] = 'application/json'
             # headers['referer'] = f'https://twitter.com/{self.username}'
-            headers['sec-fetch-site'] = 'same-origin'
+            headers['Sec-Fetch-Site'] = 'same-origin'
 
             if self.guest_token:
-                headers['x-guest-token'] = self.guest_token
+                headers['X-Guest-Token'] = self.guest_token
 
         return headers
 
     def _get_csrf(self):
         if self.cookies and self.cookies.get("ct0"):
             return self.cookies.get("ct0")
 
-        return ''.join(random.choices(string.ascii_letters + string.digits, k=32))
+        return utils.get_random_string(32)
 
     @staticmethod
     def _build(url, params):
         return "?".join([url, params])
 
     @return_with_headers
     def get_guest_token(self):
@@ -477,29 +485,167 @@
 
         if max_id:
             params['max_id'] = max_id
 
         return "GET", self._build(self.URL_AUSER_CONVERSATION.format(conversation_id), urlencode(params))
 
     @return_with_headers
-    def send_message(self):
+    def get_bookmarks(self, cursor=None):
+        variables = {"count": 20, "includePromotedContent": True}
+        features = {"graphql_timeline_v2_bookmark_timeline": True, "rweb_lists_timeline_redesign_enabled": True,
+                    "responsive_web_graphql_exclude_directive_enabled": True, "verified_phone_label_enabled": False,
+                    "creator_subscriptions_tweet_preview_api_enabled": True,
+                    "responsive_web_graphql_timeline_navigation_enabled": True,
+                    "responsive_web_graphql_skip_user_profile_image_extensions_enabled": False,
+                    "tweetypie_unmention_optimization_enabled": True, "responsive_web_edit_tweet_api_enabled": True,
+                    "graphql_is_translatable_rweb_tweet_is_translatable_enabled": True,
+                    "view_counts_everywhere_api_enabled": True, "longform_notetweets_consumption_enabled": True,
+                    "responsive_web_twitter_article_tweet_consumption_enabled": False,
+                    "tweet_awards_web_tipping_enabled": False, "freedom_of_speech_not_reach_fetch_enabled": True,
+                    "standardized_nudges_misinfo": True,
+                    "tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled": True,
+                    "longform_notetweets_rich_text_read_enabled": True,
+                    "longform_notetweets_inline_media_enabled": True,
+                    "responsive_web_media_download_video_enabled": False,
+                    "responsive_web_enhance_cards_enabled": False}
+        fieldToggles = {"withAuxiliaryUserLabels": False, "withArticleRichContentState": False}
+
+        if cursor:
+            variables['cursor'] = cursor
+
+        params = {'variables': str(json.dumps(variables)), 'features': str(json.dumps(features)),
+                  'fieldToggles': str(json.dumps(fieldToggles))}
+
+        return "GET", self._build(self.URL_AUSER_BOOKMARK, urlencode(params))
+
+    @return_with_headers
+    def send_message(self, conversation_id, text, media_id=None):
         params = {
             'ext': 'mediaColor,altText,mediaStats,highlightedLabel,hasNftAvatar,voiceInfo,birdwatchPivot,superFollowMetadata,unmentionInfo,editControl',
             'include_ext_alt_text': True,
             'include_ext_limited_action_results': True,
             'include_reply_count': '1',
             'tweet_mode': 'extended',
             'include_ext_views': True,
             'include_groups': True,
             'include_inbox_timelines': True,
             'include_ext_media_color': True,
             'supports_reactions': True,
         }
 
-        return "POST", self._build(self.URL_AUSER_SEND_MESSAGE, urlencode(params))
+        json_data = {
+            'conversation_id': conversation_id,
+            'recipient_ids': False,
+            'request_id': utils.create_request_id(),
+            'text': text,
+            'cards_platform': 'Web-12',
+            'include_cards': 1,
+            'include_quote_count': True,
+            'dm_users': False,
+        }
+        if media_id:
+            json_data['media_id'] = media_id
+
+        return "POST", self._build(self.URL_AUSER_SEND_MESSAGE, urlencode(params)), json_data
+
+    @return_with_headers
+    def create_tweet(self, text, files, filter_=None):
+        media_entities = utils.create_media_entities(files)
+        variables = {
+            'tweet_text': text,
+            'dark_request': False,
+            'media': {
+                'media_entities': media_entities,
+                'possibly_sensitive': False,
+            },
+            'semantic_annotation_ids': []
+        }
+
+        features = {
+            'tweetypie_unmention_optimization_enabled': True,
+            'responsive_web_edit_tweet_api_enabled': True,
+            'graphql_is_translatable_rweb_tweet_is_translatable_enabled': True,
+            'view_counts_everywhere_api_enabled': True,
+            'longform_notetweets_consumption_enabled': True,
+            'responsive_web_twitter_article_tweet_consumption_enabled': False,
+            'tweet_awards_web_tipping_enabled': False,
+            'longform_notetweets_rich_text_read_enabled': True,
+            'longform_notetweets_inline_media_enabled': True,
+            'responsive_web_graphql_exclude_directive_enabled': True,
+            'verified_phone_label_enabled': False,
+            'freedom_of_speech_not_reach_fetch_enabled': True,
+            'standardized_nudges_misinfo': True,
+            'tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled': True,
+            'responsive_web_media_download_video_enabled': False,
+            'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
+            'responsive_web_graphql_timeline_navigation_enabled': True,
+            'responsive_web_enhance_cards_enabled': False
+        }
+
+        fieldToggles = {
+            'withArticleRichContentState': False,
+            'withAuxiliaryUserLabels': False
+        }
+
+        if filter_:
+            variables['conversation_control'] = {"mode": filter_}
+
+        json_data = dict(
+            variables=variables,
+            features=features,
+            queryId=utils.create_query_id(),
+            fieldToggles=fieldToggles
+        )
+
+        return "POST", self.URL_AUSER_CREATE_TWEET, json_data
+
+    @return_with_headers
+    def set_media_metadata(self, media_id, alt_text, sensitive_tags):
+        if not sensitive_tags:
+            sensitive_tags = []
+
+        sensitive_media = utils.check_sensitive_media_tags(sensitive_tags)
+        json_data = {
+            'media_id': media_id,
+            'alt_text': {
+                'text': alt_text,
+            }
+        }
+        if sensitive_media:
+            json_data['sensitive_media_warning'] = sensitive_media
+
+        return "POST", self.URL_AUSER_CREATE_MEDIA_METADATA, json_data
+
+    @return_with_headers
+    def upload_media_init(self, size, mime_type, media_category):
+        params = {
+            'command': 'INIT',
+            'total_bytes': str(int(size)),
+            'media_type': mime_type,
+            'media_category': media_category,
+        }
+        return 'POST', self._build(self.URL_AUSER_CREATE_MEDIA, urlencode(params))
+
+    @return_with_headers
+    def upload_media_append(self, media_id, segment_index):
+        params = {
+            'command': 'APPEND',
+            'media_id': media_id,
+            'segment_index': segment_index,
+        }
+        return 'POST', self._build(self.URL_AUSER_CREATE_MEDIA, urlencode(params))
+
+    @return_with_headers
+    def upload_media_finalize(self, media_id, md5_hash):
+        params = {
+            'command': 'FINALIZE',
+            'media_id': media_id,
+            'original_md5': md5_hash,
+        }
+        return 'POST', self._build(self.URL_AUSER_CREATE_MEDIA, urlencode(params))
 
     @return_with_headers
     def aUser_settings(self):
         params = {
             'include_mention_filter': True,
             'include_nsfw_user_flag': True,
             'include_nsfw_admin_flag': True,
@@ -536,15 +682,15 @@
     @staticmethod
     def startFlow(json_, username, password):
         return {
             'input_flow_data': {
                 'flow_context': {
                     'debug_overrides': {},
                     'start_location': {
-                        'location': 'unknown',
+                        'location': 'manual_link',
                     },
                 },
             },
             'subtask_versions': {
                 'action_list': 2,
                 'alert_dialog': 1,
                 'app_download_cta': 1,
@@ -665,7 +811,52 @@
                     "enter_text": {
                         "text": getAlternate,
                         "link": "next_link"
                     }
                 }
             ]
         }
+
+    def LoginAcid(self, json_, username, password):
+        reason = json_['subtasks'][0]['enter_text']['secondary_text']['text']
+        print(reason)
+        getAlternate = input("> ")
+        return {
+            "flow_token": self.get_flow_token(json_),
+            "subtask_inputs": [
+                {
+                    "subtask_id": "LoginAcid",
+                    "enter_text": {
+                        "text": getAlternate,
+                        "link": "next_link"
+                    }
+                }
+            ]
+        }
+
+    def LoginTwoFactorAuthChallenge(self, json_, username, password):
+        reason = json_['subtasks'][0]['enter_text']['header']['primary_text']['text']
+        print(reason)
+        getAlternate = input("> ")
+        return {
+            "flow_token": self.get_flow_token(json_),
+            "subtask_inputs": [
+                {
+                    "subtask_id": "LoginTwoFactorAuthChallenge",
+                    "enter_text": {
+                        "text": getAlternate,
+                        "link": "next_link"
+                    }
+                }
+            ]
+        }
+
+    @staticmethod
+    def DenyLoginSubtask(json_, username, password):
+        text = json_['subtasks'][0]['cta']['primary_text']['text']
+        secondary_text = json_['subtasks'][0]['cta']['secondary_text']['text'].replace('\n', '')
+        raise DeniedLogin(
+            error_code=37,
+            error_name="GenericAccessDenied",
+            response=None,
+            message=f"{text} : {secondary_text}"
+        )
```

### Comparing `tweety-ns-0.9/src/tweety/events/newmessage.py` & `tweety-ns-0.9.5/src/tweety/events/newmessage.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.9/src/tweety/exceptions_.py` & `tweety-ns-0.9.5/src/tweety/exceptions_.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,14 +107,31 @@
         self.message = message
         self.error_code = error_code
         self.error_name = error_name
         self.response = response
         super().__init__(self.message)
 
 
+class DeniedLogin(Exception):
+    """
+        Exception Raised when the Twitter deny the login request ,
+        could be due to multiple login attempts (or failed attempts)
+
+        Attributes:
+            message -- explanation of the error
+    """
+
+    def __init__(self, error_code, error_name, response, message):
+        self.message = message
+        self.error_code = error_code
+        self.error_name = error_name
+        self.response = response
+        super().__init__(self.message)
+
+
 class InvalidCredentials(Exception):
     """
         Exception Raised when cookies credentials are invalid
 
         Attributes:
             message -- explanation of the error
     """
```

### Comparing `tweety-ns-0.9/src/tweety/http.py` & `tweety-ns-0.9.5/src/tweety/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import os
+from typing import Callable
+
 import httpx as s
-from tqdm import tqdm
 from .exceptions_ import GuestTokenNotFound, UnknownError, UserNotFound, InvalidCredentials
 from .types.n_types import GenericError
 from .utils import custom_json, create_request_id
 from .builder import UrlBuilder
 
-
 s.Response.json_ = custom_json
 
 
 class Request:
     def __init__(self, max_retries=10, proxy=None):
         self.user = None
         self.username = None
@@ -24,31 +24,35 @@
         self.__builder.set_cookies(cookies)
         self._verify_cookies()
 
     def set_user(self, user):
         self.user = user
         self.__builder.set_cookies(self.__session.cookies)
 
-    def __get_response__(self, return_raw=False, **request_data):
+    def __get_response__(self, return_raw=False, ignoreNoneData=False, **request_data):
         response = self.__session.request(**request_data)
         response_json = response.json_() # noqa
 
+        if ignoreNoneData and len(response.text) == 0:
+            return None
+
         if not response_json:
             raise UnknownError(
                 error_code=500,
                 error_name="Server Error",
                 response=response,
                 message="Unknown Error Occurs on Twitter"
             )
 
         if response_json.get("errors") and not response_json.get("data"):
             error = response_json['errors'][0]
             return GenericError(
                 response, error.get("code"), error.get("message")
             )
+
         if return_raw:
             return response
 
         return response_json
 
     def _get_guest_token(self, max_retries=10):
         for retry in range(max_retries):
@@ -119,14 +123,18 @@
         response = self.__get_response__(**self.__builder.tweet_detail(tweetId, cursor))
         return response
 
     def get_mentions(self, user_id, cursor=None):
         response = self.__get_response__(**self.__builder.get_mentions(cursor))
         return response
 
+    def get_bookmarks(self, cursor=None):
+        response = self.__get_response__(**self.__builder.get_bookmarks(cursor))
+        return response
+
     def get_inbox(self, user_id, cursor=None):
         response = self.__get_response__(**self.__builder.get_inbox(cursor))
         return response
 
     def get_trusted_inbox(self, max_id):
         response = self.__get_response__(**self.__builder.get_trusted_inbox(max_id))
         return response
@@ -135,49 +143,68 @@
         response = self.__get_response__(**self.__builder.get_untrusted_inbox(max_id, low_quality))
         return response
 
     def get_conversation(self, conversation_id, max_id=None):
         response = self.__get_response__(**self.__builder.get_conversation_with_messages(conversation_id, max_id))
         return response
 
-    def send_message(self, conversation_id, text):
-        request_id = create_request_id()
-        json_data = {
-            'conversation_id': conversation_id,
-            'recipient_ids': False,
-            'request_id': request_id,
-            'text': text,
-            'cards_platform': 'Web-12',
-            'include_cards': 1,
-            'include_quote_count': True,
-            'dm_users': False,
-        }
-        request_data = self.__builder.send_message()
-        request_data['json'] = json_data
+    def send_message(self, conversation_id, text, media_id):
+        request_data = self.__builder.send_message(conversation_id, text, media_id)
         response = self.__get_response__(**request_data)
         return response
 
-    def download_media(self, media_url, filename=None, show_progress=True):
+    def create_tweet(self, text, files, filter_):
+        request_data = self.__builder.create_tweet(text, files, filter_)
+        response = self.__get_response__(**request_data)
+        return response
+
+    def set_media_set_metadata(self, media_id, alt_text, sensitive_tags):
+        request_data = self.__builder.set_media_metadata(media_id, alt_text, sensitive_tags)
+        response = self.__get_response__(ignoreNoneData=True, **request_data)
+        print(response)
+        return response
+
+    def upload_media_init(self, size, mime_type, media_category):
+        request_data = self.__builder.upload_media_init(size, mime_type, media_category)
+        response = self.__get_response__(**request_data)
+        return response
+
+    def upload_media_append(self, media_id, payload, headers, segment_index):
+        request_data = self.__builder.upload_media_append(media_id, segment_index)
+        request_data['headers'].update(headers)
+        request_data['data'] = payload
+
+        response = self.__get_response__(ignoreNoneData=True, **request_data)
+        return response
+
+    def upload_media_finalize(self, media_id, md5_hash):
+        request_data = self.__builder.upload_media_finalize(media_id, md5_hash)
+        response = self.__get_response__(**request_data)
+        return response
+
+    def download_media(self, media_url, filename: str = None, progress_callback: Callable[[str, int, int], None] = None):
         filename = os.path.basename(media_url).split("?")[0] if not filename else filename
         headers = self.__session.headers
         oldReferer = headers.get('Referer')
 
         if media_url.startswith("https://ton.twitter.com"):
             headers['Referer'] = "https://twitter.com/"
             self.__session.header = headers
 
         with self.__session.stream('GET', media_url, follow_redirects=True) as response:
             response.raise_for_status()
-            content_length = int(response.headers['Content-Length'])
+            total_size = int(response.headers['Content-Length'])
+            downloaded = 0
             f = open(filename, 'wb')
-            if show_progress:
-                with tqdm(total=content_length, unit='B', unit_scale=True, desc=f"[{filename}]") as pbar:
-                    for chunk in response.iter_bytes(chunk_size=8192):
-                        f.write(chunk)
-                        pbar.update(len(chunk))
-            else:
-                for chunk in response.iter_bytes(chunk_size=8192):
-                    f.write(chunk)
+            for chunk in response.iter_bytes(chunk_size=8192):
+                f.write(chunk)
+                downloaded += len(chunk)
+
+                if progress_callback:
+                    progress_callback(filename, total_size, downloaded)
+
             f.close()
 
-        self.__session.header['Referer'] = oldReferer
+        if oldReferer:
+            self.__session.headers['Referer'] = oldReferer
+
         return filename
```

### Comparing `tweety-ns-0.9/src/tweety/session.py` & `tweety-ns-0.9.5/src/tweety/session.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import json
 import os.path
 
 
 class Session:
     def __init__(self, session_name):
         self.user = None
-        self.session_name = session_name
-        self.session_file_path = os.path.join(os.getcwd(), f"{self.session_name}.json")
+        self.session_name = os.path.basename(session_name)
+        self.session_file_path = self._get_session_file_path(session_name, self.session_name)
         self.logged_in = False
         self.cookies = ""
         self._load_session()
 
+    @staticmethod
+    def _get_session_file_path(session_path, session_name):
+        directory = os.path.dirname(session_path) or os.getcwd()
+        return os.path.abspath(os.path.join(directory, f"{session_name}.json"))
+
     def _load_session(self):
         if os.path.exists(self.session_file_path):
             with open(self.session_file_path, "r") as f:
                 session_data = json.load(f)
                 self.cookies = session_data['cookies']
                 self.user = session_data['user']
```

### Comparing `tweety-ns-0.9/src/tweety/types/inbox.py` & `tweety-ns-0.9.5/src/tweety/types/inbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,17 @@
         for conv in self.conversations:
             if str(conv.id) == conversation_id:
                 return conv
 
         return None
 
     def __getitem__(self, index):
+        if isinstance(index, str):
+            return getattr(self, index)
+
         return self.conversations[index]
 
     def __iter__(self):
         for __tweet in self.conversations:
             yield __tweet
 
     def __len__(self):
@@ -238,15 +241,16 @@
     def __repr__(self):
         return "Message(id={}, conversation_id={}, time={})".format(
             self.id, self.conversation_id, self.time
         )
 
 
 class SendMessage:
-    def __init__(self, http, conversation_id, text):
+    def __init__(self, http, conversation_id, text, file=None):
         self._conv = conversation_id
         self._text = text
         self._http = http
+        self._file = file
 
     def send(self):
-        response = self._http.send_message(self._conv, self._text)
+        response = self._http.send_message(self._conv, self._text, self._file)
         return Message(response['entries'][0]['message'], response, self._http)
```

### Comparing `tweety-ns-0.9/src/tweety/types/mentions.py` & `tweety-ns-0.9.5/src/tweety/types/bookmarks.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,82 +1,84 @@
-import time
-import traceback
-from . import Tweet, Excel, deprecated
+from . import Tweet, Excel
+from .base import BaseGeneratorClass
 
 
-class Mention(dict):
+class Bookmarks(BaseGeneratorClass):
     def __init__(self, user_id, http, pages=1, wait_time=2, cursor=None):
         super().__init__()
         self.tweets = []
         self.cursor = cursor
         self.is_next_page = True
         self.http = http
         self.user_id = user_id
         self.pages = pages
         self.wait_time = wait_time
 
+    @staticmethod
+    def _get_entries(response):
+        instructions = response['data']['bookmark_timeline_v2']['timeline']['instructions']
+        entries = []
+        for instruction in instructions:
+            if instruction.get("type") == "TimelineAddEntries":
+                entries.extend(instruction['entries'])
+
+        return entries
+
+    @staticmethod
+    def _get_tweet_content_key(response):
+        if str(response['entryId']).split("-")[0] == "tweet":
+            return [response['content']['itemContent']['tweet_results']['result']]
+
+        if str(response['entryId']).split("-")[0] == "user":
+            return [response['content']['itemContent']['user_results']['result']]
+
+        if str(response['entryId']).split("-")[0] == "homeConversation":
+            return [item['item']['itemContent']['tweet_results']['result'] for item in response["content"]["items"]]
+
+        return []
+
     def get_next_page(self):
         _tweets = []
         if self.is_next_page:
-            response = self.http.get_mentions(self.user_id, cursor=self.cursor)
+            response = self.http.get_bookmarks(cursor=self.cursor)
 
-            if not response['globalObjects']:
-                self.is_next_page = False
-                return self, _tweets
-
-            users = response['globalObjects']['users']
-            tweets = response['globalObjects']['tweets']
-            for tweet_id, tweet in tweets.items():
-                user = users.get(str(tweet['user_id']))
-                tweet['author'], tweet['rest_id'] = user, tweet_id
-                parsed = Tweet(response, tweet, self.http)
-                _tweets.append(parsed)
+            entries = self._get_entries(response)
+            for entry in entries:
+                tweets = self._get_tweet_content_key(entry)
+                for tweet in tweets:
+                    try:
+                        parsed = Tweet(tweet, self.http, response)
+                        self.tweets.append(parsed)
+                        _tweets.append(parsed)
+                    except:
+                        pass
 
             self.is_next_page = self._get_cursor(response)
 
             for tweet in _tweets:
                 self.tweets.append(tweet)
 
             self['tweets'] = self.tweets
             self['is_next_page'] = self.is_next_page
             self['cursor'] = self.cursor
 
-        return self, _tweets
-
-    def generator(self):
-        for page in range(1, int(self.pages) + 1):
-            _, tweets = self.get_next_page()
-
-            yield self, tweets
+        return _tweets
 
-            if self.is_next_page and page != self.pages:
-                time.sleep(self.wait_time)
-
-    def _get_cursor(self, response):
-        for instruction in response['timeline']['instructions']:
-            if instruction.get('addEntries'):
-                entries = instruction['addEntries']['entries']
-                for entry in entries:
-                    if str(entry['entryId']).split("-")[0] == "cursor":
-                        newCursor = entry['content']['operation']['cursor']['value']
-
-                        if newCursor == self.cursor:
-                            return False
-
-                        self.cursor = newCursor
-                        return True
-
-        return False
+    def to_xlsx(self, filename=None):
+        return Excel(self, filename)
 
     def __getitem__(self, index):
+        if isinstance(index, str):
+            return getattr(self, index)
+
         return self.tweets[index]
 
     def __iter__(self):
         for __tweet in self.tweets:
             yield __tweet
 
     def __len__(self):
         return len(self.tweets)
 
     def __repr__(self):
-        return f"Mentions(user_id={self.user_id}, count={self.__len__()})"
+        return f"Bookmarks(user_id={self.user_id}, count={self.__len__()})"
```

### Comparing `tweety-ns-0.9/src/tweety/types/search.py` & `tweety-ns-0.9.5/src/tweety/types/search.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,132 +1,112 @@
-import time
-import traceback
-
-from . import Tweet, Excel, User, deprecated
-
-
-class Search(dict):
-    def __init__(self, keyword, http, pages=1, filter_=None, wait_time=2, cursor=None):
-        super().__init__()
-        self.tweets = []
-        self.users = []
-        self.keyword = keyword
-        self.cursor = cursor
-        self.is_next_page = True
-        self.http = http
-        self.pages = pages
-        self.wait_time = wait_time
-        self.filter = filter_.lower().strip() if filter_ else None
-
-    def __repr__(self):
-        return "Search(keyword={}, count={}, filter={})".format(
-            self.keyword,
-            len(self.users) if self.filter == "users" else len(self.tweets),
-            self.filter
-        )
-
-    def get_next_page(self):
-        if self.is_next_page:
-            response = self.http.perform_search(self.keyword, self.cursor, self.filter)
-            thisTweets = self._parse_response(response)
-
-            self['is_next_page'] = self.is_next_page
-            self['cursor'] = self.cursor
-
-            return thisTweets
-
-        return []
-
-    @staticmethod
-    def _get_entries(response):
-        instructions = response['data']['search_by_raw_query']['search_timeline']['timeline']['instructions']
-        for instruction in instructions:
-            if instruction.get("type") == "TimelineAddEntries":
-                return instruction['entries']
-
-        return []
-
-    @staticmethod
-    def _get_tweet_content_key(response):
-        if str(response['entryId']).split("-")[0] == "tweet":
-            return [response['content']['itemContent']['tweet_results']['result']]
-
-        if str(response['entryId']).split("-")[0] == "user":
-            return [response['content']['itemContent']['user_results']['result']]
-
-        if str(response['entryId']).split("-")[0] == "homeConversation":
-            return [item['item']['itemContent']['tweet_results']['result'] for item in response["content"]["items"]]
-
-        return []
-
-    def _parse_response(self, response):
-        thisObjects = []
-        entries = self._get_entries(response)
-        for entry in entries:
-            if self.filter == "users":
-                users = self._get_tweet_content_key(entry)
-                for user in users:
-                    try:
-                        user = User(user)
-                        self.users.append(user)
-                        thisObjects.append(user)
-                    except:
-                        pass
-                self['users'] = self.users
-            else:
-                tweets = self._get_tweet_content_key(entry)
-                for tweet in tweets:
-                    try:
-                        parsed = Tweet(tweet, self.http, response)
-                        self.tweets.append(parsed)
-                        thisObjects.append(parsed)
-                    except:
-                        pass
-
-                self['tweets'] = self.tweets
-
-        self.is_next_page = self._get_cursor(entries)
-        return thisObjects
-
-    def _get_cursor(self, entries):
-        for entry in entries:
-            if str(entry['entryId']).split("-")[0] == "cursor":
-                if entry['content']['cursorType'] == "Bottom":
-                    newCursor = entry['content']['value']
-
-                    if newCursor == self.cursor:
-                        return False
-
-                    self.cursor = newCursor
-                    return True
-
-        return False
-
-    def generator(self):
-        for page in range(1, int(self.pages) + 1):
-            this_tweets = self.get_next_page()
-
-            yield self, this_tweets
-
-            if self.is_next_page and page != self.pages:
-                time.sleep(self.wait_time)
-
-        return self
-
-    def to_xlsx(self, filename=None):
-        if self.filter == "users":
-            return AttributeError("to_xlsx with 'users' filter isn't supported yet")
-        return Excel(self.tweets, f"search-{self.keyword}", filename)
-
-    def __getitem__(self, index):
-        if self.filter == "users":
-            return self.users[index]
-        else:
-            return self.tweets[index]
-
-    def __iter__(self):
-        if self.filter == "users":
-            for _user in self.users:
-                yield _user
-        else:
-            for _tweet in self.tweets:
-                yield _tweet
+import time
+from . import Tweet, Excel, User, deprecated
+from .base import BaseGeneratorClass
+
+
+class Search(BaseGeneratorClass):
+    def __init__(self, keyword, http, pages=1, filter_=None, wait_time=2, cursor=None):
+        super().__init__()
+        self.tweets = []
+        self.users = []
+        self.keyword = keyword
+        self.cursor = cursor
+        self.is_next_page = True
+        self.http = http
+        self.pages = pages
+        self.wait_time = wait_time
+        self.filter = filter_.lower().strip() if filter_ else None
+
+    def __repr__(self):
+        return "Search(keyword={}, count={}, filter={})".format(
+            self.keyword,
+            len(self.users) if self.filter == "users" else len(self.tweets),
+            self.filter
+        )
+
+    def get_next_page(self):
+        if self.is_next_page:
+            response = self.http.perform_search(self.keyword, self.cursor, self.filter)
+            thisTweets = self._parse_response(response)
+
+            self['is_next_page'] = self.is_next_page
+            self['cursor'] = self.cursor
+
+            return thisTweets
+
+        return []
+
+    @staticmethod
+    def _get_entries(response):
+        instructions = response['data']['search_by_raw_query']['search_timeline']['timeline']['instructions']
+        entries = []
+        for instruction in instructions:
+            if instruction.get("type") == "TimelineAddEntries":
+                entries.extend(instruction['entries'])
+            elif instruction.get("type") == "TimelineReplaceEntry":
+                entries.append(instruction['entry'])
+
+        return entries
+
+    @staticmethod
+    def _get_tweet_content_key(response):
+        if str(response['entryId']).split("-")[0] == "tweet":
+            return [response['content']['itemContent']['tweet_results']['result']]
+
+        if str(response['entryId']).split("-")[0] == "user":
+            return [response['content']['itemContent']['user_results']['result']]
+
+        if str(response['entryId']).split("-")[0] == "homeConversation":
+            return [item['item']['itemContent']['tweet_results']['result'] for item in response["content"]["items"]]
+
+        return []
+
+    def _parse_response(self, response):
+        thisObjects = []
+        entries = self._get_entries(response)
+        for entry in entries:
+            if self.filter == "users":
+                users = self._get_tweet_content_key(entry)
+                for user in users:
+                    try:
+                        user = User(user)
+                        self.users.append(user)
+                        thisObjects.append(user)
+                    except:
+                        pass
+                self['users'] = self.users
+            else:
+                tweets = self._get_tweet_content_key(entry)
+                for tweet in tweets:
+                    try:
+                        parsed = Tweet(tweet, self.http, response)
+                        self.tweets.append(parsed)
+                        thisObjects.append(parsed)
+                    except:
+                        pass
+
+                self['tweets'] = self.tweets
+
+        self.is_next_page = self._get_cursor(response)
+        return thisObjects
+
+    def to_xlsx(self, filename=None):
+        if self.filter == "users":
+            return AttributeError("to_xlsx with 'users' filter isn't supported yet")
+        return Excel(self.tweets, f"search-{self.keyword}", filename)
+
+    def __getitem__(self, index):
+        if isinstance(index, str):
+            return getattr(self, index)
+
+        if self.filter == "users":
+            return self.users[index]
+        else:
+            return self.tweets[index]
+
+    def __iter__(self):
+        if self.filter == "users":
+            for _user in self.users:
+                yield _user
+        else:
+            for _tweet in self.tweets:
+                yield _tweet
```

### Comparing `tweety-ns-0.9/src/tweety/types/twDataTypes.py` & `tweety-ns-0.9.5/src/tweety/types/twDataTypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,15 @@
 import re
 import sys
 import time
 import warnings
 from dateutil import parser
 import openpyxl
 import dateutil
-
-WORKBOOK_HEADERS = ['Date', 'Author', 'id', 'text', 'is_retweet', 'is_reply', 'language', 'likes',
-                    'retweet_count', 'source', 'medias', 'user_mentioned', 'urls', 'hashtags', 'symbols']
-
-
-def decodeBase64(encoded_string):
-    return str(base64.b64decode(bytes(encoded_string, "utf-8")))[2:-1]
+from ..utils import *
 
 
 def deprecated(func):
     """
 
     This is a decorator which can be used to mark functions
     as deprecated. It will result in a warning being emitted
@@ -30,19 +24,14 @@
         return func(*args, **kwargs)
     new_func.__name__ = func.__name__
     new_func.__doc__ = func.__doc__
     new_func.__dict__.update(func.__dict__)
     return new_func
 
 
-def bar_progress(current, total, width=80):
-    progress_message = "Downloading: %d%% [%d / %d] bytes" % (current / total * 100, current, total)
-    sys.stdout.write("\r" + progress_message)
-    sys.stdout.flush()
-
 
 class Excel:
     def __init__(self, tweets, filename=None, append=False):
         self.tweets = tweets
         self.filename = filename
         self.author = self._get_author()
         self._append = append
@@ -513,29 +502,29 @@
         for i in videoDict.get("variants"):
             if not i.get("content_type").split("/")[-1] == "x-mpegURL":
                 self.streams.append(Stream(i, videoDict.get("duration_millis", 0), videoDict.get("aspect_ratio"), self.__http))
 
     def __repr__(self):
         return f"Media(id={self.id}, type={self.type})"
 
-    def download(self, filename=None, show_progress=True):
+    def download(self, filename: str = None, progress_callback: Callable[[str, int, int], None] = None):
         if self.type == "photo":
-            return self.__http.download_media(self.direct_url, filename, show_progress)
+            return self.__http.download_media(self.direct_url, filename, progress_callback)
         elif self.type == "video":
             _res = [eval(stream.res) for stream in self.streams if stream.res]
             max_res = max(_res)
             for stream in self.streams:
                 if eval(stream.res) == max_res:
                     file_format = stream.content_type.split("/")[-1]
                     if not file_format == "x-mpegURL":
-                        return self.__http.download_media(stream.url, filename, show_progress)
+                        return self.__http.download_media(stream.url, filename, progress_callback)
         elif self.type == "animated_gif":
             file_format = self.streams[0].content_type.split("/")[-1]
             if not file_format == "x-mpegURL":
-                return self.__http.download_media(self.streams[0].url, filename, show_progress)
+                return self.__http.download_media(self.streams[0].url, filename, progress_callback)
         return None
 
 
 class Stream(dict):
     def __init__(self, videoDict, length, ratio, http):
         super().__init__()
         self.__dictionary = videoDict
@@ -558,16 +547,16 @@
             return f"{result[0]}*{result[1]}"
 
         return None
 
     def __repr__(self):
         return f"Stream(content_type={self.content_type}, length={self.length}, bitrate={self.bitrate}, res={self.res})"
 
-    def download(self, filename_=None, show_progress=False):
-        return self.__http.download_media(self.url, filename_, show_progress)
+    def download(self, filename: str = None, progress_callback: Callable[[str, int, int], None] = None):
+        return self.__http.download_media(self.url, filename, progress_callback)
 
 
 class MediaSize(dict):
     def __init__(self, name, data):
         super().__init__()
         self._json = data
         self.name = self['name'] = name
@@ -750,14 +739,15 @@
         self.profile_interstitial_type = self._get_key("profile_interstitial_type")
         self.protected = self._get_key("protected")
         self.screen_name = self.username = self._get_key("screen_name")
         self.statuses_count = self._get_key("statuses_count")
         self.translator_type = self._get_key("translator_type")
         self.verified = self._get_verified()
         self.can_dm = self._get_key("can_dm")
+        self.following = self._get_key("following", False)
         # self.verified_type = self._get_key("verified_type")
         self.possibly_sensitive = self._get_key("possibly_sensitive")
         self.pinned_tweets = self._get_key("pinned_tweet_ids_str")
         self.profile_url = "https://twitter.com/{}".format(self.screen_name)
 
         for k, v in vars(self).items():
             if not k.startswith("_"):
@@ -805,8 +795,8 @@
         if not keyValue and user.get(key):
             keyValue = user[key]
 
         if str(keyValue).isdigit():
             keyValue = int(keyValue)
 
         return keyValue
-        
+
```

### Comparing `tweety-ns-0.9/src/tweety/types/usertweet.py` & `tweety-ns-0.9.5/src/tweety/types/usertweet.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import time
-import traceback
-
 from .twDataTypes import TweetThread
 from ..exceptions_ import UserProtected, UserNotFound
 from . import Tweet, Excel, deprecated
+from .base import BaseGeneratorClass
 
 
-class UserTweets(dict):
+class UserTweets(BaseGeneratorClass):
     def __init__(self, user_id, http, pages=1, get_replies: bool = True, wait_time=2, cursor=None):
         super().__init__()
         self.tweets = []
         self.get_replies = get_replies
         self.cursor = cursor
         self.is_next_page = True
         self.http = http
@@ -60,59 +58,38 @@
                         parsed = TweetThread(tweets, self.http, response)
                     else:
                         parsed = Tweet(tweets[0], self.http, response)
                     _tweets.append(parsed)
                 except:
                     pass
 
-            self.is_next_page = self._get_cursor(entries)
+            self.is_next_page = self._get_cursor(response)
 
             for tweet in _tweets:
                 self.tweets.append(tweet)
 
             self['tweets'] = self.tweets
             self['is_next_page'] = self.is_next_page
             self['cursor'] = self.cursor
 
-        return self, _tweets
-
-    def generator(self):
-        for page in range(1, int(self.pages) + 1):
-            _, tweets = self.get_next_page()
-
-            yield self, tweets
-
-            if self.is_next_page and page != self.pages:
-                time.sleep(self.wait_time)
-
-    def _get_cursor(self, entries):
-        for entry in entries:
-            if str(entry['entryId']).split("-")[0] == "cursor":
-                if entry['content']['cursorType'] == "Bottom":
-                    newCursor = entry['content']['value']
-
-                    if newCursor == self.cursor:
-                        return False
-
-                    self.cursor = newCursor
-                    return True
-
-        return False
+        return _tweets
 
     def to_xlsx(self, filename=None):
         return Excel(self, filename)
 
     def __getitem__(self, index):
+        if isinstance(index, str):
+            return getattr(self, index)
+
         return self.tweets[index]
 
     def __iter__(self):
         for __tweet in self.tweets:
             yield __tweet
 
     def __len__(self):
         return len(self.tweets)
 
-    def __repr__(self):
-        return f"UserTweets(user_id={self.user_id}, count={self.__len__()})"
+
```

### Comparing `tweety-ns-0.9/src/tweety_ns.egg-info/PKG-INFO` & `tweety-ns-0.9.5/src/tweety_ns.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 0.9
+Version: 0.9.5
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
@@ -14,45 +14,44 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # tweety
-Twitter's API is annoying to work with, and has lots of limitations — luckily their frontend (JavaScript) has it's own API, which I reverse–engineered. No API rate limits. No restrictions. Extremely fast.
+Twitter's API is annoying to work with, and has lots of limitations — luckily their frontend (JavaScript) has it's own API, which I reverse–engineered. xtremely fast.
 
 [![Downloads](https://static.pepy.tech/personalized-badge/tweety-ns?period=total&units=international_system&left_color=orange&right_color=blue&left_text=Downloads)](https://pepy.tech/project/tweety-ns)
 ## Prerequisites
 
 Before you begin, ensure you have met the following requirements:
 
 * Internet Connection
 * Python 3.6+
 * httpx 
 * openpyxl
-* tqdm
 
 ## Installation: 
 ```bash
 pip install tweety-ns
 ```
 
 ## Keep synced with latest fixes
 
 ##### **Pip might not be always updated , so to keep everything synced.**
 
 ```bash
-pip install https://github.com/mahrtayyab/tweety/archive/main.zip --upgrade --force-reinstall
+pip install https://github.com/mahrtayyab/tweety/archive/main.zip --upgrade 
 ```
 
 ## A Quick Example:
 ```python
-  from tweety.bot import Twitter
+  from tweety import Twitter
   
-  app = Twitter()
+  app = Twitter("session")
   
   all_tweets = app.get_tweets("elonmusk")
   for tweet in all_tweets:
       print(tweet)
 ```
 
 Full Documentation and Changelogs are [here](https://mahrtayyab.github.io/tweety_docs/)
```

