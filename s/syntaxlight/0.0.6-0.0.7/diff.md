# Comparing `tmp/syntaxlight-0.0.6.tar.gz` & `tmp/syntaxlight-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntaxlight-0.0.6.tar", max compression
+gzip compressed data, was "syntaxlight-0.0.7.tar", max compression
```

## Comparing `syntaxlight-0.0.6.tar` & `syntaxlight-0.0.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.0.6/LICENSE
--rw-r--r--   0        0        0      464 2023-07-28 02:44:41.315769 syntaxlight-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2183 2023-07-22 12:55:46.842043 syntaxlight-0.0.6/README.md
--rw-r--r--   0        0        0      209 2023-07-23 11:29:29.575296 syntaxlight-0.0.6/syntaxlight/__init__.py
--rw-r--r--   0        0        0    15135 2023-07-25 14:41:59.387948 syntaxlight-0.0.6/syntaxlight/ast.py
--rw-r--r--   0        0        0     2223 2023-07-19 06:56:41.644931 syntaxlight-0.0.6/syntaxlight/css/all.css
--rw-r--r--   0        0        0      665 2023-07-22 15:03:22.184483 syntaxlight-0.0.6/syntaxlight/css/bnf.css
--rw-r--r--   0        0        0     2118 2023-07-23 15:21:29.646891 syntaxlight-0.0.6/syntaxlight/css/c.css
--rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.0.6/syntaxlight/css/index.css
--rw-r--r--   0        0        0      529 2023-07-21 12:50:35.868013 syntaxlight-0.0.6/syntaxlight/css/json.css
--rw-r--r--   0        0        0     1101 2023-07-26 09:05:41.943038 syntaxlight-0.0.6/syntaxlight/css/lua.css
--rw-r--r--   0        0        0     2720 2023-07-20 08:04:28.110565 syntaxlight-0.0.6/syntaxlight/css/themes.json
--rw-r--r--   0        0        0      557 2023-07-19 08:11:34.232315 syntaxlight-0.0.6/syntaxlight/css/toml.css
--rw-r--r--   0        0        0      495 2023-07-19 08:15:19.310673 syntaxlight-0.0.6/syntaxlight/css/xml.css
--rw-r--r--   0        0        0     2428 2023-07-26 07:25:50.581952 syntaxlight-0.0.6/syntaxlight/error.py
--rw-r--r--   0        0        0     2011 2023-07-25 01:37:18.564742 syntaxlight-0.0.6/syntaxlight/example.py
--rw-r--r--   0        0        0     1664 2023-07-19 08:35:00.594467 syntaxlight-0.0.6/syntaxlight/export.py
--rw-r--r--   0        0        0     2733 2023-07-26 00:54:45.614318 syntaxlight-0.0.6/syntaxlight/gdt.py
--rw-r--r--   0        0        0      401 2023-07-24 09:03:19.313778 syntaxlight-0.0.6/syntaxlight/lexers/__init__.py
--rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.0.6/syntaxlight/lexers/bnf_lexer.py
--rw-r--r--   0        0        0    12468 2023-07-26 05:58:00.354541 syntaxlight-0.0.6/syntaxlight/lexers/c_lexer.py
--rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.0.6/syntaxlight/lexers/json_lexer.py
--rw-r--r--   0        0        0    22509 2023-07-26 07:30:31.563233 syntaxlight-0.0.6/syntaxlight/lexers/lexer.py
--rw-r--r--   0        0        0     8150 2023-07-26 08:57:37.822371 syntaxlight-0.0.6/syntaxlight/lexers/lua_lexer.py
--rw-r--r--   0        0        0     1801 2023-07-12 06:24:11.777365 syntaxlight-0.0.6/syntaxlight/lexers/shell_lexer.py
--rw-r--r--   0        0        0     3002 2023-07-26 02:47:58.836633 syntaxlight-0.0.6/syntaxlight/lexers/toml_lexer.py
--rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.0.6/syntaxlight/lexers/xml_lexer.py
--rw-r--r--   0        0        0      275 2023-07-25 01:05:05.983118 syntaxlight-0.0.6/syntaxlight/parsers/__init__.py
--rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.0.6/syntaxlight/parsers/bnf_parser.py
--rw-r--r--   0        0        0    98600 2023-07-26 01:24:49.618931 syntaxlight-0.0.6/syntaxlight/parsers/c_parser.py
--rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.0.6/syntaxlight/parsers/json_parser.py
--rw-r--r--   0        0        0    35078 2023-07-26 09:03:07.504849 syntaxlight-0.0.6/syntaxlight/parsers/lua_parser.py
--rw-r--r--   0        0        0    12749 2023-07-26 01:33:24.433880 syntaxlight-0.0.6/syntaxlight/parsers/parser.py
--rw-r--r--   0        0        0      405 2023-07-12 06:09:27.902688 syntaxlight-0.0.6/syntaxlight/parsers/shell_parser.py
--rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.0.6/syntaxlight/parsers/toml_parser.py
--rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.0.6/syntaxlight/parsers/xml_parser.py
--rw-r--r--   0        0        0     4250 2023-07-25 01:39:58.341430 syntaxlight-0.0.6/syntaxlight/syntax_parse.py
--rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.0.6/syntaxlight/template.html
--rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 syntaxlight-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.0.7/LICENSE
+-rw-r--r--   0        0        0      464 2023-07-29 03:47:46.141388 syntaxlight-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2183 2023-07-22 12:55:46.842043 syntaxlight-0.0.7/README.md
+-rw-r--r--   0        0        0      209 2023-07-23 11:29:29.575296 syntaxlight-0.0.7/syntaxlight/__init__.py
+-rw-r--r--   0        0        0    15135 2023-07-25 14:41:59.387948 syntaxlight-0.0.7/syntaxlight/ast.py
+-rw-r--r--   0        0        0     2223 2023-07-19 06:56:41.644931 syntaxlight-0.0.7/syntaxlight/css/all.css
+-rw-r--r--   0        0        0      665 2023-07-22 15:03:22.184483 syntaxlight-0.0.7/syntaxlight/css/bnf.css
+-rw-r--r--   0        0        0     2118 2023-07-23 15:21:29.646891 syntaxlight-0.0.7/syntaxlight/css/c.css
+-rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.0.7/syntaxlight/css/index.css
+-rw-r--r--   0        0        0      529 2023-07-21 12:50:35.868013 syntaxlight-0.0.7/syntaxlight/css/json.css
+-rw-r--r--   0        0        0     1101 2023-07-26 09:05:41.943038 syntaxlight-0.0.7/syntaxlight/css/lua.css
+-rw-r--r--   0        0        0     2720 2023-07-20 08:04:28.110565 syntaxlight-0.0.7/syntaxlight/css/themes.json
+-rw-r--r--   0        0        0      557 2023-07-19 08:11:34.232315 syntaxlight-0.0.7/syntaxlight/css/toml.css
+-rw-r--r--   0        0        0      495 2023-07-19 08:15:19.310673 syntaxlight-0.0.7/syntaxlight/css/xml.css
+-rw-r--r--   0        0        0     2428 2023-07-26 07:25:50.581952 syntaxlight-0.0.7/syntaxlight/error.py
+-rw-r--r--   0        0        0     2011 2023-07-25 01:37:18.564742 syntaxlight-0.0.7/syntaxlight/example.py
+-rw-r--r--   0        0        0     1664 2023-07-19 08:35:00.594467 syntaxlight-0.0.7/syntaxlight/export.py
+-rw-r--r--   0        0        0     2733 2023-07-26 00:54:45.614318 syntaxlight-0.0.7/syntaxlight/gdt.py
+-rw-r--r--   0        0        0      401 2023-07-24 09:03:19.313778 syntaxlight-0.0.7/syntaxlight/lexers/__init__.py
+-rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.0.7/syntaxlight/lexers/bnf_lexer.py
+-rw-r--r--   0        0        0    12514 2023-07-29 03:41:26.897980 syntaxlight-0.0.7/syntaxlight/lexers/c_lexer.py
+-rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.0.7/syntaxlight/lexers/json_lexer.py
+-rw-r--r--   0        0        0    22553 2023-07-29 03:44:53.825706 syntaxlight-0.0.7/syntaxlight/lexers/lexer.py
+-rw-r--r--   0        0        0     8150 2023-07-26 08:57:37.822371 syntaxlight-0.0.7/syntaxlight/lexers/lua_lexer.py
+-rw-r--r--   0        0        0     1801 2023-07-12 06:24:11.777365 syntaxlight-0.0.7/syntaxlight/lexers/shell_lexer.py
+-rw-r--r--   0        0        0     3002 2023-07-26 02:47:58.836633 syntaxlight-0.0.7/syntaxlight/lexers/toml_lexer.py
+-rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.0.7/syntaxlight/lexers/xml_lexer.py
+-rw-r--r--   0        0        0      275 2023-07-25 01:05:05.983118 syntaxlight-0.0.7/syntaxlight/parsers/__init__.py
+-rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.0.7/syntaxlight/parsers/bnf_parser.py
+-rw-r--r--   0        0        0    99058 2023-07-29 03:43:10.405548 syntaxlight-0.0.7/syntaxlight/parsers/c_parser.py
+-rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.0.7/syntaxlight/parsers/json_parser.py
+-rw-r--r--   0        0        0    35078 2023-07-26 09:03:07.504849 syntaxlight-0.0.7/syntaxlight/parsers/lua_parser.py
+-rw-r--r--   0        0        0    12749 2023-07-26 01:33:24.433880 syntaxlight-0.0.7/syntaxlight/parsers/parser.py
+-rw-r--r--   0        0        0      405 2023-07-12 06:09:27.902688 syntaxlight-0.0.7/syntaxlight/parsers/shell_parser.py
+-rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.0.7/syntaxlight/parsers/toml_parser.py
+-rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.0.7/syntaxlight/parsers/xml_parser.py
+-rw-r--r--   0        0        0     4250 2023-07-25 01:39:58.341430 syntaxlight-0.0.7/syntaxlight/syntax_parse.py
+-rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.0.7/syntaxlight/template.html
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 syntaxlight-0.0.7/PKG-INFO
```

### Comparing `syntaxlight-0.0.6/LICENSE` & `syntaxlight-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/README.md` & `syntaxlight-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/ast.py` & `syntaxlight-0.0.7/syntaxlight/ast.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/css/all.css` & `syntaxlight-0.0.7/syntaxlight/css/all.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/css/bnf.css` & `syntaxlight-0.0.7/syntaxlight/css/bnf.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/css/c.css` & `syntaxlight-0.0.7/syntaxlight/css/c.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/css/index.css` & `syntaxlight-0.0.7/syntaxlight/css/index.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/css/json.css` & `syntaxlight-0.0.7/syntaxlight/css/json.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/css/lua.css` & `syntaxlight-0.0.7/syntaxlight/css/lua.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/css/themes.json` & `syntaxlight-0.0.7/syntaxlight/css/themes.json`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/css/toml.css` & `syntaxlight-0.0.7/syntaxlight/css/toml.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/error.py` & `syntaxlight-0.0.7/syntaxlight/error.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/example.py` & `syntaxlight-0.0.7/syntaxlight/example.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/export.py` & `syntaxlight-0.0.7/syntaxlight/export.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/gdt.py` & `syntaxlight-0.0.7/syntaxlight/gdt.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/lexers/bnf_lexer.py` & `syntaxlight-0.0.7/syntaxlight/lexers/bnf_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/lexers/c_lexer.py` & `syntaxlight-0.0.7/syntaxlight/lexers/c_lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 
             if self.current_char == "/" and self.peek() == "/":
                 return self.get_comment("//", "\n")
             if self.current_char == "/" and self.peek() == "*":
                 return self.get_comment("/*", "*/")
 
             if self.current_char.isdigit():
-                return self.get_number()
+                return self.get_number(accept_hex=True, accept_bit=True,accept_p=True)
 
             if self.current_char.isalpha() or self.current_char == TokenType.UNDERLINE.value:
                 return self.get_id()
 
             if self.current_char == '"':
                 return self.get_string()
```

### Comparing `syntaxlight-0.0.6/syntaxlight/lexers/json_lexer.py` & `syntaxlight-0.0.7/syntaxlight/lexers/json_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/lexers/lexer.py` & `syntaxlight-0.0.7/syntaxlight/lexers/lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,14 +355,15 @@
          <digit> ::= [0-9]
         <digits> ::= <digit>*
         <number> ::= <digits>(.<digits>)?(E|e[+-]?<digits>)?
 
         @accept_float: 允许小数和科学计数法
         @accept_hex  : 允许16进制表示 0xfff
         @accept_bit  : 允许二进制表示 0b111
+        @accept_p    : 允许后面跟 P/p
         """
         bit_matching_status = False
         hex_matching_status = False
         def is_match_char(char:str) -> bool:
             
             if hex_matching_status:
                 return bool(re.match(r'[0-9a-fA-F]',char))
```

### Comparing `syntaxlight-0.0.6/syntaxlight/lexers/lua_lexer.py` & `syntaxlight-0.0.7/syntaxlight/lexers/lua_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/lexers/shell_lexer.py` & `syntaxlight-0.0.7/syntaxlight/lexers/shell_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/lexers/toml_lexer.py` & `syntaxlight-0.0.7/syntaxlight/lexers/toml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/lexers/xml_lexer.py` & `syntaxlight-0.0.7/syntaxlight/lexers/xml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/parsers/bnf_parser.py` & `syntaxlight-0.0.7/syntaxlight/parsers/bnf_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/parsers/c_parser.py` & `syntaxlight-0.0.7/syntaxlight/parsers/c_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -837,15 +837,28 @@
         <struct-or-union-specifier> ::= <struct-or-union> <identifier> ("{" {<struct-declaration>}* "}")?
                                       | <struct-or-union>              "{" {<struct-declaration>}* "}"
         """
         if self.current_token.type not in self.cfirst_set.struct_or_union_specifier:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be struct or union")
 
         node = Structure()
+        
         node.update(structure_type=self.struct_or_union())
+
+        # 对于如下情况
+        # typedef struct State State;
+        # struct State {
+        #     int c;
+        #     State *out;
+        #     State *out1;
+        #     int lastlist;
+        # };
+        # 将当前 struct 中当前 token: "State" 从 CTokenType.TYPEDEF_ID 恢复为TokenType.ID
+        if self.current_token.type == CTokenType.TYPEDEF_ID:
+            self.current_token.type = TokenType.ID
         if self.current_token.type == TokenType.ID:
             node.update(id=self.identifier())
         # else:
         #     # 匿名 struct
         #     if self.current_token.type != TokenType.LCURLY_BRACE:
         #         self.error(
         #             ErrorCode.UNEXPECTED_TOKEN,
@@ -1716,18 +1729,18 @@
 
         <function-definition> ::= <declaration-specifier>* <declarator> <declaration>* <compound-statement>
         """
         node = Declaration()
         if self.current_token.type in self.cfirst_set.static_assert_declaration:
             node.update(static_assert=self.static_assert_declaration())
             return node
-
+        
         declaration_specifiers: List[AST] = [self.declaration_sepcifier()]
         self._unknown_typedef_id_guess()
-
+        
         while self.current_token.type in self.cfirst_set.declaration_specifier:
             declaration_specifiers.append(self.declaration_sepcifier())
             self._unknown_typedef_id_guess()
 
         if self.current_token.type in self.cfirst_set.init_declarator_list:
             init_declarator_list = self.init_declarator_list()
             if self.current_token.type == TokenType.SEMI:
```

### Comparing `syntaxlight-0.0.6/syntaxlight/parsers/json_parser.py` & `syntaxlight-0.0.7/syntaxlight/parsers/json_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/parsers/lua_parser.py` & `syntaxlight-0.0.7/syntaxlight/parsers/lua_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/parsers/parser.py` & `syntaxlight-0.0.7/syntaxlight/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/parsers/toml_parser.py` & `syntaxlight-0.0.7/syntaxlight/parsers/toml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/parsers/xml_parser.py` & `syntaxlight-0.0.7/syntaxlight/parsers/xml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/syntaxlight/syntax_parse.py` & `syntaxlight-0.0.7/syntaxlight/syntax_parse.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.6/PKG-INFO` & `syntaxlight-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntaxlight
-Version: 0.0.6
+Version: 0.0.7
 Summary: syntax highlight based on EBNF
 Home-page: https://github.com/luzhixing12345/syntaxlight
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

