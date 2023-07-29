# Comparing `tmp/syntaxlight-0.0.7.tar.gz` & `tmp/syntaxlight-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntaxlight-0.0.7.tar", max compression
+gzip compressed data, was "syntaxlight-0.0.8.tar", max compression
```

## Comparing `syntaxlight-0.0.7.tar` & `syntaxlight-0.0.8.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.0.7/LICENSE
--rw-r--r--   0        0        0      464 2023-07-29 03:47:46.141388 syntaxlight-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2183 2023-07-22 12:55:46.842043 syntaxlight-0.0.7/README.md
--rw-r--r--   0        0        0      209 2023-07-23 11:29:29.575296 syntaxlight-0.0.7/syntaxlight/__init__.py
--rw-r--r--   0        0        0    15135 2023-07-25 14:41:59.387948 syntaxlight-0.0.7/syntaxlight/ast.py
--rw-r--r--   0        0        0     2223 2023-07-19 06:56:41.644931 syntaxlight-0.0.7/syntaxlight/css/all.css
--rw-r--r--   0        0        0      665 2023-07-22 15:03:22.184483 syntaxlight-0.0.7/syntaxlight/css/bnf.css
--rw-r--r--   0        0        0     2118 2023-07-23 15:21:29.646891 syntaxlight-0.0.7/syntaxlight/css/c.css
--rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.0.7/syntaxlight/css/index.css
--rw-r--r--   0        0        0      529 2023-07-21 12:50:35.868013 syntaxlight-0.0.7/syntaxlight/css/json.css
--rw-r--r--   0        0        0     1101 2023-07-26 09:05:41.943038 syntaxlight-0.0.7/syntaxlight/css/lua.css
--rw-r--r--   0        0        0     2720 2023-07-20 08:04:28.110565 syntaxlight-0.0.7/syntaxlight/css/themes.json
--rw-r--r--   0        0        0      557 2023-07-19 08:11:34.232315 syntaxlight-0.0.7/syntaxlight/css/toml.css
--rw-r--r--   0        0        0      495 2023-07-19 08:15:19.310673 syntaxlight-0.0.7/syntaxlight/css/xml.css
--rw-r--r--   0        0        0     2428 2023-07-26 07:25:50.581952 syntaxlight-0.0.7/syntaxlight/error.py
--rw-r--r--   0        0        0     2011 2023-07-25 01:37:18.564742 syntaxlight-0.0.7/syntaxlight/example.py
--rw-r--r--   0        0        0     1664 2023-07-19 08:35:00.594467 syntaxlight-0.0.7/syntaxlight/export.py
--rw-r--r--   0        0        0     2733 2023-07-26 00:54:45.614318 syntaxlight-0.0.7/syntaxlight/gdt.py
--rw-r--r--   0        0        0      401 2023-07-24 09:03:19.313778 syntaxlight-0.0.7/syntaxlight/lexers/__init__.py
--rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.0.7/syntaxlight/lexers/bnf_lexer.py
--rw-r--r--   0        0        0    12514 2023-07-29 03:41:26.897980 syntaxlight-0.0.7/syntaxlight/lexers/c_lexer.py
--rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.0.7/syntaxlight/lexers/json_lexer.py
--rw-r--r--   0        0        0    22553 2023-07-29 03:44:53.825706 syntaxlight-0.0.7/syntaxlight/lexers/lexer.py
--rw-r--r--   0        0        0     8150 2023-07-26 08:57:37.822371 syntaxlight-0.0.7/syntaxlight/lexers/lua_lexer.py
--rw-r--r--   0        0        0     1801 2023-07-12 06:24:11.777365 syntaxlight-0.0.7/syntaxlight/lexers/shell_lexer.py
--rw-r--r--   0        0        0     3002 2023-07-26 02:47:58.836633 syntaxlight-0.0.7/syntaxlight/lexers/toml_lexer.py
--rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.0.7/syntaxlight/lexers/xml_lexer.py
--rw-r--r--   0        0        0      275 2023-07-25 01:05:05.983118 syntaxlight-0.0.7/syntaxlight/parsers/__init__.py
--rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.0.7/syntaxlight/parsers/bnf_parser.py
--rw-r--r--   0        0        0    99058 2023-07-29 03:43:10.405548 syntaxlight-0.0.7/syntaxlight/parsers/c_parser.py
--rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.0.7/syntaxlight/parsers/json_parser.py
--rw-r--r--   0        0        0    35078 2023-07-26 09:03:07.504849 syntaxlight-0.0.7/syntaxlight/parsers/lua_parser.py
--rw-r--r--   0        0        0    12749 2023-07-26 01:33:24.433880 syntaxlight-0.0.7/syntaxlight/parsers/parser.py
--rw-r--r--   0        0        0      405 2023-07-12 06:09:27.902688 syntaxlight-0.0.7/syntaxlight/parsers/shell_parser.py
--rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.0.7/syntaxlight/parsers/toml_parser.py
--rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.0.7/syntaxlight/parsers/xml_parser.py
--rw-r--r--   0        0        0     4250 2023-07-25 01:39:58.341430 syntaxlight-0.0.7/syntaxlight/syntax_parse.py
--rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.0.7/syntaxlight/template.html
--rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 syntaxlight-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.0.8/LICENSE
+-rw-r--r--   0        0        0      464 2023-07-29 14:40:09.550161 syntaxlight-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2183 2023-07-22 12:55:46.842043 syntaxlight-0.0.8/README.md
+-rw-r--r--   0        0        0      187 2023-07-29 14:31:45.643282 syntaxlight-0.0.8/syntaxlight/__init__.py
+-rw-r--r--   0        0        0    15173 2023-07-29 13:02:30.287941 syntaxlight-0.0.8/syntaxlight/ast.py
+-rw-r--r--   0        0        0     2223 2023-07-29 13:42:32.821896 syntaxlight-0.0.8/syntaxlight/css/all.css
+-rw-r--r--   0        0        0      665 2023-07-22 15:03:22.184483 syntaxlight-0.0.8/syntaxlight/css/bnf.css
+-rw-r--r--   0        0        0     2118 2023-07-23 15:21:29.646891 syntaxlight-0.0.8/syntaxlight/css/c.css
+-rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.0.8/syntaxlight/css/index.css
+-rw-r--r--   0        0        0      529 2023-07-21 12:50:35.868013 syntaxlight-0.0.8/syntaxlight/css/json.css
+-rw-r--r--   0        0        0     1101 2023-07-26 09:05:41.943038 syntaxlight-0.0.8/syntaxlight/css/lua.css
+-rw-r--r--   0        0        0      744 2023-07-29 14:18:59.090972 syntaxlight-0.0.8/syntaxlight/css/shell.css
+-rw-r--r--   0        0        0     2812 2023-07-29 14:20:16.175242 syntaxlight-0.0.8/syntaxlight/css/themes.json
+-rw-r--r--   0        0        0      557 2023-07-19 08:11:34.232315 syntaxlight-0.0.8/syntaxlight/css/toml.css
+-rw-r--r--   0        0        0      495 2023-07-19 08:15:19.310673 syntaxlight-0.0.8/syntaxlight/css/xml.css
+-rw-r--r--   0        0        0     2428 2023-07-26 07:25:50.581952 syntaxlight-0.0.8/syntaxlight/error.py
+-rw-r--r--   0        0        0     2011 2023-07-25 01:37:18.564742 syntaxlight-0.0.8/syntaxlight/example.py
+-rw-r--r--   0        0        0     1666 2023-07-29 05:28:25.722849 syntaxlight-0.0.8/syntaxlight/export.py
+-rw-r--r--   0        0        0     2781 2023-07-29 13:56:47.817032 syntaxlight-0.0.8/syntaxlight/gdt.py
+-rw-r--r--   0        0        0      401 2023-07-24 09:03:19.313778 syntaxlight-0.0.8/syntaxlight/lexers/__init__.py
+-rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.0.8/syntaxlight/lexers/bnf_lexer.py
+-rw-r--r--   0        0        0    12514 2023-07-29 03:41:26.897980 syntaxlight-0.0.8/syntaxlight/lexers/c_lexer.py
+-rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.0.8/syntaxlight/lexers/json_lexer.py
+-rw-r--r--   0        0        0    22638 2023-07-29 13:36:11.005583 syntaxlight-0.0.8/syntaxlight/lexers/lexer.py
+-rw-r--r--   0        0        0     8150 2023-07-26 08:57:37.822371 syntaxlight-0.0.8/syntaxlight/lexers/lua_lexer.py
+-rw-r--r--   0        0        0     4077 2023-07-29 14:16:38.127889 syntaxlight-0.0.8/syntaxlight/lexers/shell_lexer.py
+-rw-r--r--   0        0        0     3002 2023-07-26 02:47:58.836633 syntaxlight-0.0.8/syntaxlight/lexers/toml_lexer.py
+-rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.0.8/syntaxlight/lexers/xml_lexer.py
+-rw-r--r--   0        0        0      275 2023-07-25 01:05:05.983118 syntaxlight-0.0.8/syntaxlight/parsers/__init__.py
+-rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.0.8/syntaxlight/parsers/bnf_parser.py
+-rw-r--r--   0        0        0    99058 2023-07-29 03:43:10.405548 syntaxlight-0.0.8/syntaxlight/parsers/c_parser.py
+-rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.0.8/syntaxlight/parsers/json_parser.py
+-rw-r--r--   0        0        0    35078 2023-07-26 09:03:07.504849 syntaxlight-0.0.8/syntaxlight/parsers/lua_parser.py
+-rw-r--r--   0        0        0    12778 2023-07-29 14:00:12.143979 syntaxlight-0.0.8/syntaxlight/parsers/parser.py
+-rw-r--r--   0        0        0     2344 2023-07-29 14:21:32.659521 syntaxlight-0.0.8/syntaxlight/parsers/shell_parser.py
+-rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.0.8/syntaxlight/parsers/toml_parser.py
+-rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.0.8/syntaxlight/parsers/xml_parser.py
+-rw-r--r--   0        0        0     4277 2023-07-29 13:01:51.131206 syntaxlight-0.0.8/syntaxlight/syntax_parse.py
+-rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.0.8/syntaxlight/template.html
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 syntaxlight-0.0.8/PKG-INFO
```

### Comparing `syntaxlight-0.0.7/LICENSE` & `syntaxlight-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/README.md` & `syntaxlight-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/ast.py` & `syntaxlight-0.0.8/syntaxlight/ast.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,14 +405,16 @@
         graphviz_content += self.dot_footer
         with open(self.image_name, "w", encoding="utf-8") as f:
             f.write(graphviz_content)
         print(f"ast tree saved in [{self.image_name}], view by grpahviz")
 
 
 def display_ast(node: AST, sub_roots: List[AST], save_ast_tree=False):
+    if node is None:
+        return
     node_visitor = NodeVisitor()
     node.visit(node_visitor)
     for sub_root in sub_roots:
         node_visitor.depth += 1
         sub_root.visit(node_visitor)
 
     if save_ast_tree:
```

### Comparing `syntaxlight-0.0.7/syntaxlight/css/all.css` & `syntaxlight-0.0.8/syntaxlight/css/all.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/css/bnf.css` & `syntaxlight-0.0.8/syntaxlight/css/bnf.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/css/c.css` & `syntaxlight-0.0.8/syntaxlight/css/c.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/css/index.css` & `syntaxlight-0.0.8/syntaxlight/css/index.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/css/json.css` & `syntaxlight-0.0.8/syntaxlight/css/json.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/css/lua.css` & `syntaxlight-0.0.8/syntaxlight/css/lua.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/css/themes.json` & `syntaxlight-0.0.8/syntaxlight/css/themes.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984567901234568%*

 * *Differences: {"'vscode'": "{'extension': {'shell': OrderedDict([('.Token.OPTION', 'color: #ABABAB;')])}}"}*

```diff
@@ -75,13 +75,16 @@
         "--struct": "#4EC9B0",
         "--type": "#569cd6",
         "--variant": "#88D6FE",
         "extension": {
             "json": {
                 ".Token.Keyword": "color: #327ED0;"
             },
+            "shell": {
+                ".Token.OPTION": "color: #ABABAB;"
+            },
             "toml": {
                 ".Token.Keyword": "color: #327ED0;"
             }
         }
     }
 }
```

### Comparing `syntaxlight-0.0.7/syntaxlight/css/toml.css` & `syntaxlight-0.0.8/syntaxlight/css/toml.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/error.py` & `syntaxlight-0.0.8/syntaxlight/error.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/example.py` & `syntaxlight-0.0.8/syntaxlight/example.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/export.py` & `syntaxlight-0.0.8/syntaxlight/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,7 +36,8 @@
 
             with open(export_name, "w", encoding="utf-8") as f:
                 f.write(css_content)
     else:
         print(f"unknown style {style}")
         print(f"supported style: {list(themes.keys())}")
         exit(1)
+
```

### Comparing `syntaxlight-0.0.7/syntaxlight/gdt.py` & `syntaxlight-0.0.8/syntaxlight/gdt.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     FUNCTION_CALL = "FunctionCall"
     TYPEDEF = "Typedefine"  # 自定义类型 / 未知类型
     PREPROCESS = "Preprocess"  # 预处理命令
     MACRO_DEFINE = "MacroDefine"  # 宏定义变量
     MACRO_FUNCTION = "MarcroFunction"  # 宏定义函数
     ENUMERATOR = "Enumerator"  # 枚举类
     ENUM_ID = "EnumID"  # 枚举类型
+    FORMAT = 'Format'
+    CONTROL = 'Control'
 
 
 class Descriptor(TypedDict):
     type: Enum
     scope: str
```

### Comparing `syntaxlight-0.0.7/syntaxlight/lexers/bnf_lexer.py` & `syntaxlight-0.0.8/syntaxlight/lexers/bnf_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/lexers/c_lexer.py` & `syntaxlight-0.0.8/syntaxlight/lexers/c_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/lexers/json_lexer.py` & `syntaxlight-0.0.8/syntaxlight/lexers/json_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/lexers/lexer.py` & `syntaxlight-0.0.8/syntaxlight/lexers/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     CYAN = 96
     WHITE = 97
 
 
 class Token:
     def __init__(self, type: Enum, value, line=None, column=None):
         self.type: Enum = type
-        self.value = value
+        self.value:str = value
         self.line: int = line
         self.column: int = column
         self.ast: None
         self.class_list = set()  # parser 语法分析阶段赋给 token
         self.class_list.add("Token")
         global GLOBAL_TOKEN_ID
         self._id = GLOBAL_TOKEN_ID
@@ -138,14 +138,17 @@
         return "Token[{ID}]({type}, {value}, position={lineno}:{column})".format(
             ID=self._id,
             type=self.type,
             value=repr(self.value),
             lineno=self.line,
             column=self.column,
         )
+    
+    def add_css(self, CSS: Enum):
+        self.class_list.add(CSS.value)
 
     def __repr__(self):
         return self.__str__()
 
 
 class Lexer:
     """
```

### Comparing `syntaxlight-0.0.7/syntaxlight/lexers/lua_lexer.py` & `syntaxlight-0.0.8/syntaxlight/lexers/lua_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/lexers/shell_lexer.py` & `syntaxlight-0.0.8/syntaxlight/lexers/toml_lexer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,77 @@
-
-
-from .lexer import Lexer, Token, TokenType, ErrorCode
+from .lexer import Lexer, Token, TokenType
+from ..error import ErrorCode
 from enum import Enum
 
-class ShellTokenType(Enum):
+
+class TomlTokenType(Enum):
     RESERVED_KEYWORD_START = "RESERVED_KEYWORD_START"
-    ALIAS = 'alias'
-    BG = 'bg'
-    BIND = 'bind'
-    BREAK = 'break'
-    BUILTIN = 'builtin'
-    CALLER = 'caller'
-    CASE = 'case'
-    CD = 'cd'
-    
+    TRUE = "true"
+    FALSE = "false"
     RESERVED_KEYWORD_END = "RESERVED_KEYWORD_END"
 
-class ShellLexer(Lexer):
+    DATE = "DATE"
+
 
-    def __init__(self, text: str, LanguageTokenType: Enum = ShellTokenType):
+class TomlLexer(Lexer):
+    def __init__(self, text: str, LanguageTokenType: Enum = TomlTokenType):
         super().__init__(text, LanguageTokenType)
 
-    def get_next_token(self) -> Token:
+    def get_next_token(self):
         while self.current_char is not None:
+            if self.current_char == "'" and self.peek(2) == "''":
+                return self.get_extend_str(("'''", "'''"))
+            if self.current_char == '"' and self.peek(2) == '""':
+                return self.get_extend_str(('"""', '"""'))
+
+            # TOML 单双引号都可以
+            if self.current_char in ('"', "'"):
+                return self.get_str()
+
             if self.current_char == TokenType.SPACE.value:
-                    return self.skip_whitespace()
+                return self.skip_whitespace()
 
             if self.current_char in self.invisible_characters:
                 return self.skip_invisiable_character()
 
+            if self.current_char == TokenType.HASH.value:
+                # match comment
+                return self.get_comment()
+
             if self.current_char.isdigit():
-                return self.get_number()
+                token = self.get_number()
+                # https://datatracker.ietf.org/doc/html/rfc3339
+                # a tricky implementation
+                if self.current_char in (TokenType.MINUS.value, TokenType.COLON.value):
+                    result = token.value
+                    while self.current_char is not None and self.current_char not in (
+                        TokenType.HASH.value,
+                        TokenType.CR.value,
+                        TokenType.LF.value,
+                    ):
+                        result += self.current_char
+                        self.advance()
+                    return Token(TomlTokenType.DATE, result, self.line, self.column - 1)
+                else:
+                    return token
+
+            if self.current_char.isalpha():
+                return self.get_id(extend_chars=["_"])
 
-            if self.current_char.isalnum() or self.current_char == '_':
-                return self.get_id(extend_chars=['_','-'])
             try:
                 token_type = TokenType(self.current_char)
-            except ValueError: # pragma: no cover
+            except ValueError:  # pragma: no cover
                 token = Token(None, self.current_char, self.line, self.column)
                 self.error(ErrorCode.UNKNOWN_CHARACTER, token)
             else:
                 token = Token(
                     type=token_type,
                     value=token_type.value,  # e.g. ';', '.', etc
                     line=self.line,
                     column=self.column,
                 )
                 self.advance()
                 return token
-            
-        # End of File
-        return Token(type=TokenType.EOF, value='EOF', line=self.line, column=self.column)
+
+        # EOF (end-of-file) token indicates that there is no more
+        # input left for lexical analysis
+        return Token(type=TokenType.EOF, value="EOF", line=self.line, column=self.column)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `syntaxlight-0.0.7/syntaxlight/lexers/xml_lexer.py` & `syntaxlight-0.0.8/syntaxlight/lexers/xml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/parsers/bnf_parser.py` & `syntaxlight-0.0.8/syntaxlight/parsers/bnf_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/parsers/c_parser.py` & `syntaxlight-0.0.8/syntaxlight/parsers/c_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/parsers/json_parser.py` & `syntaxlight-0.0.8/syntaxlight/parsers/json_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/parsers/lua_parser.py` & `syntaxlight-0.0.8/syntaxlight/parsers/lua_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/parsers/parser.py` & `syntaxlight-0.0.8/syntaxlight/parsers/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from enum import Enum
 from ..ast import AST, Keyword, add_ast_type, Identifier, Punctuator, String
 from typing import List
 import sys
 import html
 import traceback
 import re
+from ..gdt import CSS
 
 
 DEBUG = False
 DEBUG = True
 
 
 class Parser:
@@ -317,29 +318,29 @@
             node.register_token(self.eat(token_type))
         return node
 
     def string_inside_format(self, token: Token) -> List[String]:
         """
         取出其中格式化字符(如 %d %x \n) 并新建 token
         """
-        pattern = r"(%[0-9ldiufFeEgGxXoscpaAn]+|(?:\\\\|\\n|\\t|\\v|\\f))"
+        pattern = r"(%[0-9ldiufFeEgGxXoscpaAnYyMmHhSs]+|(?:\\\\|\\n|\\t|\\v|\\f))"
         sub_strings = re.split(pattern, token.value)
         new_asts = []
         line = token.line
         column = token.column - len(token.value)
         token_type = token.type
         for sub_string in sub_strings:
             if len(sub_string) == 0:
                 continue
             column += len(sub_string)
             token = Token(token_type, sub_string, line, column)
-            if bool(re.match(r"%[0-9ldiufFeEgGxXoscpaAn]+", sub_string)):
-                token.class_list.add("Format")
+            if bool(re.match(r"%[0-9ldiufFeEgGxXoscpaAnYyMmHhSs]+", sub_string)):
+                token.add_css(CSS.FORMAT)
             elif sub_string in ["\\n", "\\t", "\\f", "\\v", "\\a", "\\b", "\\\\"]:
-                token.class_list.add("Control")
+                token.add_css(CSS.CONTROL)
 
             self.manual_register_token(token)
             node = String(token.value)
             node.register_token([token])
             new_asts.append(node)
 
         self.manual_get_next_token()
```

### Comparing `syntaxlight-0.0.7/syntaxlight/parsers/toml_parser.py` & `syntaxlight-0.0.8/syntaxlight/parsers/toml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/parsers/xml_parser.py` & `syntaxlight-0.0.8/syntaxlight/parsers/xml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.7/syntaxlight/syntax_parse.py` & `syntaxlight-0.0.8/syntaxlight/syntax_parse.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 import os
 from .lexers import *
 from .error import Error
 from .parsers import *
 from .ast import display_ast
 import sys
+from typing import List, TypedDict
 
+class SyntaxDict(TypedDict):
+    lexer: Lexer
+    parser: Parser
+    suffix: List[str]
 
 SUPPORTED_SYNTAX = {
-    "json": {"lexer": JsonLexer, "parser": JsonParser, "suffix": ["json"]},
-    "c": {"lexer": CLexer, "parser": CParser, "suffix": ["c", "h"]},
-    "lua": {"lexer": LuaLexer, "parser": LuaParser, "suffix": ["lua"]},
-    "bnf": {"lexer": BNFLexer, "parser": BNFParser, "suffix": ["bnf"]},
-    "makefile": {"lexer": None, "parser": None, "suffix": ["Makefile", "mk", "mak", "makefile"]},
-    "java": {"lexer": None, "parser": None, "suffix": ["java"]},
-    "rust": {"lexer": None, "parser": None, "suffix": ["rs"]},
-    "javascript": {"lexer": None, "parser": None, "suffix": ["js"]},
-    "typescript": {"lexer": None, "parser": None, "suffix": ["ts", "tsx", "tsc"]},
-    "pascal": {"lexer": None, "parser": None, "suffix": ["pas"]},
-    "toml": {"lexer": TomlLexer, "parser": TomlParser, "suffix": ["toml"]},
-    "xml": {"lexer": XmlLexer, "parser": XmlParser, "suffix": ["xml"]},
-    "shell": {"lexer": ShellLexer, "parser": ShellParser, "suffix": ["sh"]},
+    "json": SyntaxDict(lexer=JsonLexer, parser=JsonParser, suffix=['json']),
+    "c": SyntaxDict(lexer=CLexer, parser=CParser, suffix=["c", "h"]),
+    "lua": SyntaxDict(lexer=LuaLexer, parser=LuaParser, suffix=['lua']),
+    "bnf": SyntaxDict(lexer=BNFLexer, parser=BNFParser, suffix=['bnf']),
+    "toml": SyntaxDict(lexer=TomlLexer, parser=TomlParser, suffix=['toml']),
+    "xml": SyntaxDict(lexer=XmlLexer, parser=XmlParser, suffix=['xml']),
+    "shell": SyntaxDict(lexer=ShellLexer, parser=ShellParser, suffix=['sh']),
+    "bash": SyntaxDict(lexer=ShellLexer, parser=ShellParser, suffix=['sh'])
 }
 
 
+def is_language_support(language: str):
+    """
+    检验 syntaxlight 是否支持当前语言
+    """
+    global SUPPORTED_SYNTAX
+    language = language.lower()
+    if language in SUPPORTED_SYNTAX:
+        return True
+    else:
+        return False
+
+
 def parse(
     text: str, language=None, file_path=None, show_error_context=True, save_ast_tree=False
 ) -> str:
     if len(text) == 0:
         return ""
 
     parser = get_parser(text, language)
```

### Comparing `syntaxlight-0.0.7/PKG-INFO` & `syntaxlight-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntaxlight
-Version: 0.0.7
+Version: 0.0.8
 Summary: syntax highlight based on EBNF
 Home-page: https://github.com/luzhixing12345/syntaxlight
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

