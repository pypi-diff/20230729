# Comparing `tmp/arts-2023.7.10.tar.gz` & `tmp/arts-2023.7.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arts-2023.7.10.tar", last modified: Sun Jul  9 07:15:16 2023, max compression
+gzip compressed data, was "arts-2023.7.29.tar", last modified: Sat Jul 29 13:12:05 2023, max compression
```

## Comparing `arts-2023.7.10.tar` & `arts-2023.7.29.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     2008 2023-07-09 05:21:16.311980 arts-2023.7.10/.gitignore
--rw-r--r--   0        0        0     1409 2023-07-09 07:13:27.518674 arts-2023.7.10/README.md
--rw-r--r--   0        0        0     3064 2023-07-03 07:43:10.621577 arts-2023.7.10/arts/[1]编程教程/Python/5分钟理清Python的时间操作/README.md
--rw-r--r--   0        0        0     3395 2023-06-24 07:55:32.849161 arts-2023.7.10/arts/[1]编程教程/Python/[1]成果展示/用37行代码实现AI五子棋/README.md
--rw-r--r--   0        0        0   132558 2023-06-24 07:41:37.503743 arts-2023.7.10/arts/[1]编程教程/Python/[1]成果展示/用37行代码实现AI五子棋/无颜色版.png
--rw-r--r--   0        0        0   135794 2023-06-24 07:38:22.760800 arts-2023.7.10/arts/[1]编程教程/Python/[1]成果展示/用37行代码实现AI五子棋/有颜色版.png
--rw-r--r--   0        0        0     2042 2023-06-24 05:45:38.711787 arts-2023.7.10/arts/[1]编程教程/Python/[2]其它/调用openAI进行连续对话/README.md
--rw-r--r--   0        0        0   254025 2023-06-14 02:25:03.834797 arts-2023.7.10/arts/[1]编程教程/Python/[2]其它/调用openAI进行连续对话/封面.jpg
--rw-r--r--   0        0        0    18019 2023-06-24 06:12:43.983353 arts-2023.7.10/arts/[1]编程教程/Python/数据库/操作MongoDB简明教程/README.md
--rw-r--r--   0        0        0    18733 2023-06-24 06:13:20.633561 arts-2023.7.10/arts/[1]编程教程/Python/数据库/操作MySQL简明教程/README.md
--rw-r--r--   0        0        0     8138 2023-06-24 05:44:39.242507 arts-2023.7.10/arts/[1]编程教程/Python/正则表达式/1、清洗自然灾害数据/README.md
--rw-r--r--   0        0        0   486729 2023-06-17 08:11:16.639983 arts-2023.7.10/arts/[1]编程教程/Python/正则表达式/1、清洗自然灾害数据/封面.png
--rw-r--r--   0        0        0     1447 2023-07-09 03:17:30.347956 arts-2023.7.10/arts/[2]批判·伪文艺/一元官司有意义吗？/README.md
--rw-r--r--   0        0        0     1742 2023-06-24 07:01:54.613165 arts-2023.7.10/arts/[4]论时事/评价在北京工体冲进场的梅西粉丝/README.md
--rw-r--r--   0        0        0   148143 2023-06-18 06:04:10.170676 arts-2023.7.10/arts/[4]论时事/评价在北京工体冲进场的梅西粉丝/封面.jpg
--rw-r--r--   0        0        0     1652 2023-06-23 06:48:35.450766 arts-2023.7.10/arts/[87]原创小说/天使传奇/1、被绑架/README.md
--rw-r--r--   0        0        0     7343 2023-06-23 06:29:16.614903 arts-2023.7.10/arts/[87]原创小说/陆小凤新传/燕山宝藏/第一章/README.md
--rw-r--r--   0        0        0   644251 2023-07-05 13:25:53.974953 arts-2023.7.10/arts/[88]原创UI/富文本笔记本/README.png
--rw-r--r--   0        0        0   793233 2023-07-05 13:25:39.829792 arts-2023.7.10/arts/[89]原创图片/捷鸟/README.jpg
--rw-r--r--   0        0        0     2114 2023-07-03 07:30:37.022832 arts-2023.7.10/arts/[8]万象思考/ChatGPT已经有自我意识了/README.md
--rw-r--r--   0        0        0      772 2023-06-23 06:31:13.738964 arts-2023.7.10/arts/[8]万象思考/万物为什么会遵循着物理定律？/README.md
--rw-r--r--   0        0        0     3693 2023-06-24 08:40:00.061857 arts-2023.7.10/arts/[8]万象思考/人权/人人平等是个伪概念/README.md
--rw-r--r--   0        0        0     5051 2023-06-24 08:20:27.835932 arts-2023.7.10/arts/[8]万象思考/人权/堕胎自由权/README.md
--rw-r--r--   0        0        0     1584 2023-06-23 06:49:51.732869 arts-2023.7.10/arts/[8]万象思考/什么是“迷信科学”？/README.md
--rw-r--r--   0        0        0     1672 2023-07-08 11:03:35.265812 arts-2023.7.10/arts/[8]万象思考/心理学中个案研究有意义吗？/README.md
--rw-r--r--   0        0        0     3149 2023-06-24 08:34:59.453148 arts-2023.7.10/arts/[8]万象思考/有无相生，难易相成的启发/README.md
--rw-r--r--   0        0        0     1226 2023-06-24 06:51:31.392036 arts-2023.7.10/arts/[8]万象思考/熵增都是坏的，熵减都是好的吗？/README.md
--rw-r--r--   0        0        0     1120 2023-07-08 16:03:09.173781 arts-2023.7.10/arts/[99]其它/现在的‘人工智能’是‘穷举智能’/README.md
--rw-r--r--   0        0        0     2976 2023-07-09 04:11:45.403508 arts-2023.7.10/arts/[99]其它/用均匀抽样作文件指纹的可靠性/README.md
--rw-r--r--   0        0        0     3353 2023-06-24 07:15:39.665620 arts-2023.7.10/arts/[9]时空遐想/轮回转世真的存在吗？/README.md
--rw-r--r--   0        0        0       35 2023-06-24 05:26:09.197796 arts-2023.7.10/arts/__init__.py
--rw-r--r--   0        0        0      412 2023-07-09 07:08:46.286344 arts-2023.7.10/arts/_core.py
--rw-r--r--   0        0        0      345 2023-07-09 07:14:25.121621 arts-2023.7.10/pyproject.toml
--rw-r--r--   0        0        0     1603 1970-01-01 00:00:00.000000 arts-2023.7.10/PKG-INFO
+-rw-r--r--   0        0        0     2008 2023-07-29 13:09:55.071754 arts-2023.7.29/.gitignore
+-rw-r--r--   0        0        0     1433 2023-07-29 07:40:45.952747 arts-2023.7.29/README.md
+-rw-r--r--   0        0        0     3395 2023-06-24 07:55:32.849161 arts-2023.7.29/arts/1-编程教程/Python/1-成果展示/用37行代码实现AI五子棋/README.md
+-rw-r--r--   0        0        0   132558 2023-06-24 07:41:37.503743 arts-2023.7.29/arts/1-编程教程/Python/1-成果展示/用37行代码实现AI五子棋/无颜色版.png
+-rw-r--r--   0        0        0   135794 2023-06-24 07:38:22.760800 arts-2023.7.29/arts/1-编程教程/Python/1-成果展示/用37行代码实现AI五子棋/有颜色版.png
+-rw-r--r--   0        0        0     4058 2023-07-29 12:15:15.415663 arts-2023.7.29/arts/1-编程教程/Python/10-编程题·万物皆可编码/渔夫垂钓/README.md
+-rw-r--r--   0        0        0     3064 2023-07-03 07:43:10.621577 arts-2023.7.29/arts/1-编程教程/Python/5分钟理清Python的时间操作/README.md
+-rw-r--r--   0        0        0    18019 2023-06-24 06:12:43.983353 arts-2023.7.29/arts/1-编程教程/Python/数据库/操作MongoDB简明教程/README.md
+-rw-r--r--   0        0        0    18733 2023-06-24 06:13:20.633561 arts-2023.7.29/arts/1-编程教程/Python/数据库/操作MySQL简明教程/README.md
+-rw-r--r--   0        0        0     8138 2023-06-24 05:44:39.242507 arts-2023.7.29/arts/1-编程教程/Python/正则表达式/1、清洗自然灾害数据/README.md
+-rw-r--r--   0        0        0   486729 2023-06-17 08:11:16.639983 arts-2023.7.29/arts/1-编程教程/Python/正则表达式/1、清洗自然灾害数据/封面.png
+-rw-r--r--   0        0        0     8143 2023-07-15 16:26:41.513121 arts-2023.7.29/arts/1-编程教程/Python/调用openAI进行连续对话/README.md
+-rw-r--r--   0        0        0   254025 2023-06-14 02:25:03.834797 arts-2023.7.29/arts/1-编程教程/Python/调用openAI进行连续对话/封面.jpg
+-rw-r--r--   0        0        0     1447 2023-07-09 03:17:30.347956 arts-2023.7.29/arts/2-批判·伪文艺/一元官司有意义吗？/README.md
+-rw-r--r--   0        0        0     1742 2023-06-24 07:01:54.613165 arts-2023.7.29/arts/4-论时事/评价在北京工体冲进场的梅西粉丝/README.md
+-rw-r--r--   0        0        0   148143 2023-06-18 06:04:10.170676 arts-2023.7.29/arts/4-论时事/评价在北京工体冲进场的梅西粉丝/封面.jpg
+-rw-r--r--   0        0        0     2114 2023-07-03 07:30:37.022832 arts-2023.7.29/arts/8-万象思考/ChatGPT已经有自我意识了/README.md
+-rw-r--r--   0        0        0      772 2023-06-23 06:31:13.738964 arts-2023.7.29/arts/8-万象思考/万物为什么会遵循着物理定律？/README.md
+-rw-r--r--   0        0        0     3693 2023-06-24 08:40:00.061857 arts-2023.7.29/arts/8-万象思考/人权/人人平等是个伪概念/README.md
+-rw-r--r--   0        0        0     5051 2023-06-24 08:20:27.835932 arts-2023.7.29/arts/8-万象思考/人权/堕胎自由权/README.md
+-rw-r--r--   0        0        0     1584 2023-06-23 06:49:51.732869 arts-2023.7.29/arts/8-万象思考/什么是“迷信科学”？/README.md
+-rw-r--r--   0        0        0     1672 2023-07-08 11:03:35.265812 arts-2023.7.29/arts/8-万象思考/心理学中个案研究有意义吗？/README.md
+-rw-r--r--   0        0        0     3149 2023-06-24 08:34:59.453148 arts-2023.7.29/arts/8-万象思考/有无相生，难易相成的启发/README.md
+-rw-r--r--   0        0        0     1226 2023-06-24 06:51:31.392036 arts-2023.7.29/arts/8-万象思考/熵增都是坏的，熵减都是好的吗？/README.md
+-rw-r--r--   0        0        0     1652 2023-06-23 06:48:35.450766 arts-2023.7.29/arts/87-原创小说/天使传奇/1、被绑架/README.md
+-rw-r--r--   0        0        0     7343 2023-06-23 06:29:16.614903 arts-2023.7.29/arts/87-原创小说/陆小凤新传/燕山宝藏/第一章/README.md
+-rw-r--r--   0        0        0   644251 2023-07-05 13:25:53.974953 arts-2023.7.29/arts/88-原创UI/富文本笔记本/README.png
+-rw-r--r--   0        0        0   793233 2023-07-05 13:25:39.829792 arts-2023.7.29/arts/89-原创图片/捷鸟/README.jpg
+-rw-r--r--   0        0        0     3353 2023-06-24 07:15:39.665620 arts-2023.7.29/arts/9-时空遐想/轮回转世真的存在吗？/README.md
+-rw-r--r--   0        0        0     1120 2023-07-08 16:03:09.173781 arts-2023.7.29/arts/99-其它/现在的‘人工智能’是‘穷举智能’/README.md
+-rw-r--r--   0        0        0     2976 2023-07-09 04:11:45.403508 arts-2023.7.29/arts/99-其它/用均匀抽样作文件指纹的可靠性/README.md
+-rw-r--r--   0        0        0       35 2023-06-24 05:26:09.197796 arts-2023.7.29/arts/__init__.py
+-rw-r--r--   0        0        0      412 2023-07-09 07:08:46.286344 arts-2023.7.29/arts/_core.py
+-rw-r--r--   0        0        0      345 2023-07-29 13:06:58.488800 arts-2023.7.29/pyproject.toml
+-rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 arts-2023.7.29/PKG-INFO
```

### Comparing `arts-2023.7.10/.gitignore` & `arts-2023.7.29/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 **/_ig_**
 *.zip
 *.cmd
 *.sql
 *.txt
 *.json
 
-**/_ii_**
+**/_ip_**
 *.mp4
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
```

### Comparing `arts-2023.7.10/README.md` & `arts-2023.7.29/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 
 ```
 pip install arts
 ```
 
 # 关于作者
 
-作者：lcctoor.com
+昵称：lcctoor.com
+
+域名：lcctoor.com
 
 邮箱：lcctoor@outlook.com
 
 [主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg)
 
 # 教程
```

### Comparing `arts-2023.7.10/arts/[1]编程教程/Python/5分钟理清Python的时间操作/README.md` & `arts-2023.7.29/arts/1-编程教程/Python/5分钟理清Python的时间操作/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[1]编程教程/Python/[1]成果展示/用37行代码实现AI五子棋/README.md` & `arts-2023.7.29/arts/1-编程教程/Python/1-成果展示/用37行代码实现AI五子棋/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[1]编程教程/Python/[1]成果展示/用37行代码实现AI五子棋/无颜色版.png` & `arts-2023.7.29/arts/1-编程教程/Python/1-成果展示/用37行代码实现AI五子棋/无颜色版.png`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[1]编程教程/Python/[1]成果展示/用37行代码实现AI五子棋/有颜色版.png` & `arts-2023.7.29/arts/1-编程教程/Python/1-成果展示/用37行代码实现AI五子棋/有颜色版.png`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[1]编程教程/Python/[2]其它/调用openAI进行连续对话/封面.jpg` & `arts-2023.7.29/arts/1-编程教程/Python/调用openAI进行连续对话/封面.jpg`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[1]编程教程/Python/数据库/操作MongoDB简明教程/README.md` & `arts-2023.7.29/arts/1-编程教程/Python/数据库/操作MongoDB简明教程/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[1]编程教程/Python/数据库/操作MySQL简明教程/README.md` & `arts-2023.7.29/arts/1-编程教程/Python/数据库/操作MySQL简明教程/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[1]编程教程/Python/正则表达式/1、清洗自然灾害数据/README.md` & `arts-2023.7.29/arts/1-编程教程/Python/正则表达式/1、清洗自然灾害数据/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[1]编程教程/Python/正则表达式/1、清洗自然灾害数据/封面.png` & `arts-2023.7.29/arts/1-编程教程/Python/正则表达式/1、清洗自然灾害数据/封面.png`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[2]批判·伪文艺/一元官司有意义吗？/README.md` & `arts-2023.7.29/arts/2-批判·伪文艺/一元官司有意义吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[4]论时事/评价在北京工体冲进场的梅西粉丝/README.md` & `arts-2023.7.29/arts/4-论时事/评价在北京工体冲进场的梅西粉丝/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[4]论时事/评价在北京工体冲进场的梅西粉丝/封面.jpg` & `arts-2023.7.29/arts/4-论时事/评价在北京工体冲进场的梅西粉丝/封面.jpg`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[87]原创小说/天使传奇/1、被绑架/README.md` & `arts-2023.7.29/arts/87-原创小说/天使传奇/1、被绑架/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[87]原创小说/陆小凤新传/燕山宝藏/第一章/README.md` & `arts-2023.7.29/arts/87-原创小说/陆小凤新传/燕山宝藏/第一章/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[88]原创UI/富文本笔记本/README.png` & `arts-2023.7.29/arts/88-原创UI/富文本笔记本/README.png`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[89]原创图片/捷鸟/README.jpg` & `arts-2023.7.29/arts/89-原创图片/捷鸟/README.jpg`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[8]万象思考/ChatGPT已经有自我意识了/README.md` & `arts-2023.7.29/arts/8-万象思考/ChatGPT已经有自我意识了/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[8]万象思考/万物为什么会遵循着物理定律？/README.md` & `arts-2023.7.29/arts/8-万象思考/万物为什么会遵循着物理定律？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[8]万象思考/人权/人人平等是个伪概念/README.md` & `arts-2023.7.29/arts/8-万象思考/人权/人人平等是个伪概念/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[8]万象思考/人权/堕胎自由权/README.md` & `arts-2023.7.29/arts/8-万象思考/人权/堕胎自由权/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[8]万象思考/什么是“迷信科学”？/README.md` & `arts-2023.7.29/arts/8-万象思考/什么是“迷信科学”？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[8]万象思考/心理学中个案研究有意义吗？/README.md` & `arts-2023.7.29/arts/8-万象思考/心理学中个案研究有意义吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[8]万象思考/有无相生，难易相成的启发/README.md` & `arts-2023.7.29/arts/8-万象思考/有无相生，难易相成的启发/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[8]万象思考/熵增都是坏的，熵减都是好的吗？/README.md` & `arts-2023.7.29/arts/8-万象思考/熵增都是坏的，熵减都是好的吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[99]其它/现在的‘人工智能’是‘穷举智能’/README.md` & `arts-2023.7.29/arts/99-其它/现在的‘人工智能’是‘穷举智能’/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[99]其它/用均匀抽样作文件指纹的可靠性/README.md` & `arts-2023.7.29/arts/99-其它/用均匀抽样作文件指纹的可靠性/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/arts/[9]时空遐想/轮回转世真的存在吗？/README.md` & `arts-2023.7.29/arts/9-时空遐想/轮回转世真的存在吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.7.10/PKG-INFO` & `arts-2023.7.29/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arts
-Version: 2023.7.10
+Version: 2023.7.29
 Summary: 快捷提取指定目录下所有子孙文件夹中的 README.* 文件
 Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # 项目描述
 
@@ -14,15 +14,17 @@
 
 ```
 pip install arts
 ```
 
 # 关于作者
 
-作者：lcctoor.com
+昵称：lcctoor.com
+
+域名：lcctoor.com
 
 邮箱：lcctoor@outlook.com
 
 [主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg)
 
 # 教程
```

