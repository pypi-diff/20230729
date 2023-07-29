# Comparing `tmp/markdownparser-0.5.4.tar.gz` & `tmp/markdownparser-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdownparser-0.5.4.tar", max compression
+gzip compressed data, was "markdownparser-0.5.5.tar", max compression
```

## Comparing `markdownparser-0.5.4.tar` & `markdownparser-0.5.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.5.4/LICENSE
--rw-r--r--   0        0        0       92 2023-07-29 04:37:54.786227 markdownparser-0.5.4/MarkdownParser/__init__.py
--rw-r--r--   0        0        0     5969 2023-07-29 05:13:27.554441 markdownparser-0.5.4/MarkdownParser/base_class.py
--rw-r--r--   0        0        0    24817 2023-07-29 04:08:14.607222 markdownparser-0.5.4/MarkdownParser/block_parser.py
--rw-r--r--   0        0        0     7072 2023-07-29 05:12:59.301866 markdownparser-0.5.4/MarkdownParser/core.py
--rw-r--r--   0        0        0     3285 2023-07-29 04:08:11.133670 markdownparser-0.5.4/MarkdownParser/preprocess_parser.py
--rw-r--r--   0        0        0    21736 2023-07-29 04:08:19.718060 markdownparser-0.5.4/MarkdownParser/tree_parser.py
--rw-r--r--   0        0        0      442 2023-07-29 05:26:47.582005 markdownparser-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     4827 2023-07-04 02:51:45.730014 markdownparser-0.5.4/README.md
--rw-r--r--   0        0        0     5600 1970-01-01 00:00:00.000000 markdownparser-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.5.5/LICENSE
+-rw-r--r--   0        0        0      123 2023-07-29 05:45:52.175866 markdownparser-0.5.5/MarkdownParser/__init__.py
+-rw-r--r--   0        0        0     5969 2023-07-29 05:13:27.554441 markdownparser-0.5.5/MarkdownParser/base_class.py
+-rw-r--r--   0        0        0    24817 2023-07-29 04:08:14.607222 markdownparser-0.5.5/MarkdownParser/block_parser.py
+-rw-r--r--   0        0        0     7072 2023-07-29 05:12:59.301866 markdownparser-0.5.5/MarkdownParser/core.py
+-rw-r--r--   0        0        0     3285 2023-07-29 04:08:11.133670 markdownparser-0.5.5/MarkdownParser/preprocess_parser.py
+-rw-r--r--   0        0        0    21736 2023-07-29 04:08:19.718060 markdownparser-0.5.5/MarkdownParser/tree_parser.py
+-rw-r--r--   0        0        0      442 2023-07-29 05:52:38.693129 markdownparser-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     4854 2023-07-29 05:52:22.923372 markdownparser-0.5.5/README.md
+-rw-r--r--   0        0        0     5627 1970-01-01 00:00:00.000000 markdownparser-0.5.5/PKG-INFO
```

### Comparing `markdownparser-0.5.4/LICENSE` & `markdownparser-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.4/MarkdownParser/base_class.py` & `markdownparser-0.5.5/MarkdownParser/base_class.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.4/MarkdownParser/block_parser.py` & `markdownparser-0.5.5/MarkdownParser/block_parser.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.4/MarkdownParser/core.py` & `markdownparser-0.5.5/MarkdownParser/core.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.4/MarkdownParser/preprocess_parser.py` & `markdownparser-0.5.5/MarkdownParser/preprocess_parser.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.4/MarkdownParser/tree_parser.py` & `markdownparser-0.5.5/MarkdownParser/tree_parser.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.4/README.md` & `markdownparser-0.5.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 # 解析 markdown 文本, 带目录树
 def parse_toc(text: str) -> str:
 
 # 解析 md 文件, 带目录树
 def parse_file_toc(file_name: str) -> str:
 ```
 
+接口类 Markdown, Block
+
 ## 结果预览与 Markdown 功能测试
 
 本仓库下提供了了一个快速验证转换结果的工具 generate.py
 
 ```bash
 python generate.py <FILE_NAME>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 install markdownparser ``` ## å¿«éä½¿ç¨ ```python import MarkdownParser html
 = MarkdownParser.parse('# Hello World!') print(html) #
 ****** Hello World! ******
 ``` æ¥å£å½æ° ```python # è§£æ markdown ææ¬è½¬ html def parse(text:
 str) -> str: # è§£æ md æä»¶è½¬ html def parse_file(file_name: str) -> str:
 # è§£æ markdown ææ¬, å¸¦ç®å½æ  def parse_toc(text: str) -> str: #
 è§£æ md æä»¶, å¸¦ç®å½æ  def parse_file_toc(file_name: str) -> str: ```
-## ç»æé¢è§ä¸ Markdown åè½æµè¯
+æ¥å£ç±» Markdown, Block ## ç»æé¢è§ä¸ Markdown åè½æµè¯
 æ¬ä»åºä¸æä¾äºäºä¸ä¸ªå¿«ééªè¯è½¬æ¢ç»æçå·¥å· generate.py
 ```bash python generate.py  # python generate.py ./testfiles/test1.md # python
 generate.py README.md ``` è¿è¡ä¼çæindex.html,
 ä½¿ç¨æµè§å¨æå¼çæçindex.htmlå³å¯ä¸æ¨é¢æçæ¸²æç»æå¯¹æ¯,
 README çæ¸²æç»æå¦ä¸æç¤º ![20230218202400](https://
 raw.githubusercontent.com/learner-lu/picbed/master/20230218202400.png) ##
 å®ç°æè·¯ [Markdownè§£æå¨çä»£ç å®ç°](https://www.bilibili.com/video/
```

### Comparing `markdownparser-0.5.4/PKG-INFO` & `markdownparser-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdownparser
-Version: 0.5.4
+Version: 0.5.5
 Summary: 
 Home-page: https://github.com/luzhixing12345/MarkdownParser
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -53,14 +53,16 @@
 # 解析 markdown 文本, 带目录树
 def parse_toc(text: str) -> str:
 
 # 解析 md 文件, 带目录树
 def parse_file_toc(file_name: str) -> str:
 ```
 
+接口类 Markdown, Block
+
 ## 结果预览与 Markdown 功能测试
 
 本仓库下提供了了一个快速验证转换结果的工具 generate.py
 
 ```bash
 python generate.py <FILE_NAME>
```

