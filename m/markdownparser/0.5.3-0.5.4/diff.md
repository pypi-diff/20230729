# Comparing `tmp/markdownparser-0.5.3.tar.gz` & `tmp/markdownparser-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdownparser-0.5.3.tar", max compression
+gzip compressed data, was "markdownparser-0.5.4.tar", max compression
```

## Comparing `markdownparser-0.5.3.tar` & `markdownparser-0.5.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.5.3/LICENSE
--rw-r--r--   0        0        0       92 2023-06-06 07:15:33.183694 markdownparser-0.5.3/MarkdownParser/__init__.py
--rw-r--r--   0        0        0     5967 2023-07-21 08:41:10.601700 markdownparser-0.5.3/MarkdownParser/base_class.py
--rw-r--r--   0        0        0    24813 2023-07-21 08:38:15.300746 markdownparser-0.5.3/MarkdownParser/block_parser.py
--rw-r--r--   0        0        0     6816 2023-07-21 08:38:25.951898 markdownparser-0.5.3/MarkdownParser/core.py
--rw-r--r--   0        0        0     3283 2023-07-21 08:06:23.941552 markdownparser-0.5.3/MarkdownParser/preprocess_parser.py
--rw-r--r--   0        0        0    21734 2023-07-21 08:36:10.839905 markdownparser-0.5.3/MarkdownParser/tree_parser.py
--rw-r--r--   0        0        0      442 2023-07-21 08:44:58.581972 markdownparser-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     4827 2023-07-04 02:51:45.730014 markdownparser-0.5.3/README.md
--rw-r--r--   0        0        0     5600 1970-01-01 00:00:00.000000 markdownparser-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.5.4/LICENSE
+-rw-r--r--   0        0        0       92 2023-07-29 04:37:54.786227 markdownparser-0.5.4/MarkdownParser/__init__.py
+-rw-r--r--   0        0        0     5969 2023-07-29 05:13:27.554441 markdownparser-0.5.4/MarkdownParser/base_class.py
+-rw-r--r--   0        0        0    24817 2023-07-29 04:08:14.607222 markdownparser-0.5.4/MarkdownParser/block_parser.py
+-rw-r--r--   0        0        0     7072 2023-07-29 05:12:59.301866 markdownparser-0.5.4/MarkdownParser/core.py
+-rw-r--r--   0        0        0     3285 2023-07-29 04:08:11.133670 markdownparser-0.5.4/MarkdownParser/preprocess_parser.py
+-rw-r--r--   0        0        0    21736 2023-07-29 04:08:19.718060 markdownparser-0.5.4/MarkdownParser/tree_parser.py
+-rw-r--r--   0        0        0      442 2023-07-29 05:26:47.582005 markdownparser-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     4827 2023-07-04 02:51:45.730014 markdownparser-0.5.4/README.md
+-rw-r--r--   0        0        0     5600 1970-01-01 00:00:00.000000 markdownparser-0.5.4/PKG-INFO
```

### Comparing `markdownparser-0.5.3/LICENSE` & `markdownparser-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.3/MarkdownParser/base_class.py` & `markdownparser-0.5.4/MarkdownParser/base_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,14 +151,15 @@
             content += block.toHTML()
         if header_navigater:
             return f"{header_navigater}<div class='markdown-body'>{content}</div>"
         else:
             return f"<div class='markdown-body'>{content}</div>"
 
 
+
 class Handler:
     def __init__(self) -> None:
         self.RE: re.Pattern = None
         self.parser:Parser = None
 
     def match(self, text: str, *args):  # pragma: no cover
         if self.RE is None:
```

### Comparing `markdownparser-0.5.3/MarkdownParser/block_parser.py` & `markdownparser-0.5.4/MarkdownParser/block_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,14 +185,15 @@
         new_text = re.sub(self.RE, self.sub_func, text)
         self.parser.match(self.block, new_text)
         # 单匹配去掉外层 ComplexBlock
         if len(self.block.sub_blocks) == 1:
             self.block = self.block.sub_blocks[0]
         root.addBlock(self.block)
 
+
 class ExtensionBlockHandler(Handler):  # pragma: no cover
     # 自定义扩展
     # {% note %}
     # asdklja
     # {%end%}
 
     def __init__(self) -> None:
@@ -762,15 +763,15 @@
     def toHTML(self):
         # fix bug: 修复一些 <abc> 这种虽然不匹配网址, 但是会被 html 解析为标签的情况
         # 见 test14.md
         self.input["word"] = html.escape(self.input["word"])
         return self.input["word"]
 
 
-def buildBlockParser():
+def build_block_parser():
     # block parser 用于逐行处理文本, 并将结果解析为一颗未优化的树
     block_parser = BlockParser()
     block_parser.register(EmptyBlockHandler(), 100)
     block_parser.register(EscapeCharacterHandler(), 98)
     block_parser.register(SplitBlockHandler(), 95)
     block_parser.register(HierarchyIndentHandler(), 90)
     block_parser.register(HashHeaderHandler(), 80)
```

### Comparing `markdownparser-0.5.3/MarkdownParser/core.py` & `markdownparser-0.5.4/MarkdownParser/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,60 @@
-from .preprocess_parser import buildPreprocessParser
-from .block_parser import buildBlockParser
-from .tree_parser import buildTreeParser
+
+import os
+from .preprocess_parser import build_preprocess_parser
+from .block_parser import build_block_parser, HashHeaderBlock, Block
+from .tree_parser import build_tree_parser
 
 
 class Markdown:
     def __init__(self) -> None:
         self.build_parser()
 
     def build_parser(self):
-        self.preprocess_parser = buildPreprocessParser()
-        self.block_parser = buildBlockParser()
-        self.tree_parser = buildTreeParser()
+        self.preprocess_parser = build_preprocess_parser()
+        self.block_parser = build_block_parser()
+        self.tree_parser = build_tree_parser()
 
     def parse(self, text: str) -> str:
         # 去除空行/注释/html标签
         lines = self.preprocess_parser(text)
         # print(lines)
         # 逐行解析,得到一颗未优化的树
         root = self.block_parser(lines)
         # root.info()
         # 优化,得到正确的markdown解析树
         tree = self.tree_parser(root)
         # tree.info()
         # 输出到屏幕 / 导出html文件
         return tree.toHTML()
-
+    
     def parse_with_tag(self, text: str):
         # 去除空行/注释/html标签
         lines = self.preprocess_parser(text)
         # print(lines)
         # 逐行解析,得到一颗未优化的树
         root = self.block_parser(lines)
         # root.info()
         # 优化,得到正确的markdown解析树
         tree = self.tree_parser(root)
         # 输出到屏幕 / 导出html文件
-        header_navigater = self.get_header_list(tree)
+        header_navigater = self.get_toc(tree)
         return tree.toHTML(header_navigater)
 
-    def get_header_list(self, tree):
+    def get_toc(self, tree:Block):
+        '''
+        tree 为解析的目录树, 返回一个 html 目录树
+        '''
         UID = 0
         H0_block = []
-        activate_block = None  # 激活节点
+        activate_block: HashHeaderBlock = None  # 激活节点
         activate_block_level = 0
         for block in tree.sub_blocks:
             # 对所有 HashHeaderBlock 统计树结构
-            if block.block_name == "HashHeaderBlock":
+            if isinstance(block, HashHeaderBlock):
                 current_head_level = block.input["level"]
                 # 第一次匹配
                 if activate_block is None:
                     activate_block = block
                     activate_block_level = current_head_level
                     activate_block.parent_block = None
                     activate_block.UID = UID
@@ -113,15 +118,15 @@
     def get_header_navigator(self, H0_block):
         navigator_html = ""
         for block in H0_block:
             navigator_html += self._get_header_navigator(block)
         navigator_html = f'<div class="header-navigator">{navigator_html}</div>'
         return navigator_html
 
-    def _get_header_navigator(self, block):
+    def _get_header_navigator(self, block: HashHeaderBlock):
         navigator_html = ""
         level = block.input["level"]
         tag = f"h{str(level)}-{str(block.UID)}"
         word = block.to_href()
         if len(block.child_blocks) == 0:
             navigator_html = f'<ul><li><a href="#{tag}">{word}</a></li></ul>'
         else:
@@ -129,17 +134,15 @@
             for cblock in block.child_blocks:
                 sub_navigator_html += self._get_header_navigator(cblock)
             navigator_html = f'<ul><li><a href="#{tag}">{word}</a>{sub_navigator_html}</li></ul>'
 
         return navigator_html
 
 
-def parse(
-    text: str,
-) -> str:
+def parse(text: str) -> str:
     """
     解析 markdown 文本转 html
     """
     assert type(text) == str, "输入应为字符串"
 
     # 空输入
     if not text.strip():
@@ -149,20 +152,21 @@
     return md.parse(text)
 
 
 def parse_file(file_name: str) -> str:
     """
     解析 md 文件转 html
     """
+    if not os.path.exists(file_name): # pragma: no cover
+        print(f"fail to find {file_name}")
     with open(file_name, "r", encoding="utf-8") as f:
         text = f.read()
 
     return parse(text)
 
-
 def parse_toc(text: str) -> str:
     """
     解析 markdown 文本, 带目录树
     """
     assert type(text) == str, "输入应为字符串"
 
     # 空输入
```

### Comparing `markdownparser-0.5.3/MarkdownParser/preprocess_parser.py` & `markdownparser-0.5.4/MarkdownParser/preprocess_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         text = re.sub(r"^[\n]+", "", text)  # 去除开头连续空换行
         # text = re.sub(r'[\n]+$', '', text)                    # 去除结尾连续空换行
         # text = re.sub(r'[\n]{3,}', '\n\n', text)              # 去除连续换行
         # print(text)
         return text
 
 
-def buildPreprocessParser():
+def build_preprocess_parser():
     # preprocess parser 用于预处理空行/注释/HTML标签
     preprocess_parser = PreprocessParser()
     preprocess_parser.register(TabHandler(), priority=100)
     preprocess_parser.register(EscapeCharacterHandler(), priority=90)
     preprocess_parser.register(AnnotateHandler(), priority=85)
     preprocess_parser.register(HTMLLabelHandler(), priority=80)
     return preprocess_parser
```

### Comparing `markdownparser-0.5.3/MarkdownParser/tree_parser.py` & `markdownparser-0.5.4/MarkdownParser/tree_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,19 @@
     EmptyBlockHandler,
     EscapeCharacterHandler,
     PictureHandler,
     ReferenceHandler,
     SpecialTextHandler,
     TableHandler,
     TextHandler,
-    HTMLLabelHandler
+    HTMLLabelHandler,
 )
 from typing import List
 
 
-
 class TreeParser(Parser):
     def __init__(self) -> None:
         super().__init__()
 
     def __call__(self, root: Block):
         root.input["align_space_number"] = 0  # 用于 HierarchyEliminate 阶段的对齐空格调整
 
@@ -346,15 +345,15 @@
         self.RE = re.compile(r"(?<!\\)\|")
 
         # 初始化一个block parser 用于解析表格中出现的每一个表项
         # 只注册下面这些 Handler, 不解析其他的
         self.block_parser = BlockParser()
         self.block_parser.register(EmptyBlockHandler(), 100)
         self.block_parser.register(EscapeCharacterHandler(), 98)
-        self.block_parser.register(HTMLLabelHandler(),90)
+        self.block_parser.register(HTMLLabelHandler(), 90)
         self.block_parser.register(PictureHandler(), 15)
         self.block_parser.register(ReferenceHandler(), 10)
         self.block_parser.register(SpecialTextHandler(), 5)
         self.block_parser.register(TableHandler(), 4)
         self.block_parser.register(TextHandler(), 0)
         # 匹配的
         self.table_block_names = ["TableBlock"]
@@ -542,15 +541,15 @@
                 origin_text = block.input["text"]
                 # 替换以消除html元素影响
                 origin_text = re.sub("<", "&lt;", origin_text)
                 origin_text = re.sub(">", "&gt;", origin_text)
                 root.sub_blocks[i] = TextBlock(text=origin_text, word=origin_text)
 
 
-def buildTreeParser():
+def build_tree_parser():
     # tree parser 用于优化并得到正确的解析树
     tree_parser = TreeParser()
     tree_parser.register(HierarchyMerge(), 100)
     tree_parser.register(QuoteBlockMerge(), 95)
     tree_parser.register(CodeBlockOptimizer(), 90)
     tree_parser.register(HierarchyEliminate(), 85)
     tree_parser.register(OListSerialOptimizer(), 80)
```

### Comparing `markdownparser-0.5.3/README.md` & `markdownparser-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.3/PKG-INFO` & `markdownparser-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdownparser
-Version: 0.5.3
+Version: 0.5.4
 Summary: 
 Home-page: https://github.com/luzhixing12345/MarkdownParser
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

