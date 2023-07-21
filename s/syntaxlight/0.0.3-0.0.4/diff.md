# Comparing `tmp/syntaxlight-0.0.3.tar.gz` & `tmp/syntaxlight-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntaxlight-0.0.3.tar", max compression
+gzip compressed data, was "syntaxlight-0.0.4.tar", max compression
```

## Comparing `syntaxlight-0.0.3.tar` & `syntaxlight-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.0.3/LICENSE
--rw-r--r--   0        0        0      464 2023-07-20 10:03:28.191668 syntaxlight-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1632 2023-07-20 09:56:07.920078 syntaxlight-0.0.3/README.md
--rw-r--r--   0        0        0      191 2023-07-19 07:19:43.518938 syntaxlight-0.0.3/syntaxlight/__init__.py
--rw-r--r--   0        0        0    13864 2023-07-20 09:35:37.730553 syntaxlight-0.0.3/syntaxlight/ast.py
--rw-r--r--   0        0        0     2223 2023-07-19 06:56:41.644931 syntaxlight-0.0.3/syntaxlight/css/all.css
--rw-r--r--   0        0        0     2081 2023-07-19 08:12:53.632477 syntaxlight-0.0.3/syntaxlight/css/c.css
--rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.0.3/syntaxlight/css/index.css
--rw-r--r--   0        0        0      485 2023-07-19 08:11:30.544637 syntaxlight-0.0.3/syntaxlight/css/json.css
--rw-r--r--   0        0        0     2720 2023-07-20 08:04:28.110565 syntaxlight-0.0.3/syntaxlight/css/themes.json
--rw-r--r--   0        0        0      557 2023-07-19 08:11:34.232315 syntaxlight-0.0.3/syntaxlight/css/toml.css
--rw-r--r--   0        0        0      495 2023-07-19 08:15:19.310673 syntaxlight-0.0.3/syntaxlight/css/xml.css
--rw-r--r--   0        0        0     2379 2023-07-17 06:49:24.804921 syntaxlight-0.0.3/syntaxlight/error.py
--rw-r--r--   0        0        0     1995 2023-07-20 08:23:56.191983 syntaxlight-0.0.3/syntaxlight/example.py
--rw-r--r--   0        0        0     1664 2023-07-19 08:35:00.594467 syntaxlight-0.0.3/syntaxlight/export.py
--rw-r--r--   0        0        0      406 2023-07-12 03:19:24.095469 syntaxlight-0.0.3/syntaxlight/lexers/__init__.py
--rw-r--r--   0        0        0    12379 2023-07-19 02:03:36.729775 syntaxlight-0.0.3/syntaxlight/lexers/c_lexer.py
--rw-r--r--   0        0        0     2219 2023-07-04 09:22:19.741835 syntaxlight-0.0.3/syntaxlight/lexers/ebnf_lexer.py
--rw-r--r--   0        0        0     1864 2023-07-04 09:20:59.243201 syntaxlight-0.0.3/syntaxlight/lexers/json_lexer.py
--rw-r--r--   0        0        0    19627 2023-07-19 02:25:52.820410 syntaxlight-0.0.3/syntaxlight/lexers/lexer.py
--rw-r--r--   0        0        0     4090 2023-06-16 15:53:43.032864 syntaxlight-0.0.3/syntaxlight/lexers/lua_lexer.py
--rw-r--r--   0        0        0     1801 2023-07-12 06:24:11.777365 syntaxlight-0.0.3/syntaxlight/lexers/shell_lexer.py
--rw-r--r--   0        0        0     3538 2023-07-06 06:05:23.042009 syntaxlight-0.0.3/syntaxlight/lexers/toml_lexer.py
--rw-r--r--   0        0        0     4578 2023-07-11 14:54:57.917125 syntaxlight-0.0.3/syntaxlight/lexers/xml_lexer.py
--rw-r--r--   0        0        0      205 2023-07-12 06:09:50.252799 syntaxlight-0.0.3/syntaxlight/parsers/__init__.py
--rw-r--r--   0        0        0   100655 2023-07-20 10:00:41.507850 syntaxlight-0.0.3/syntaxlight/parsers/c_parser.py
--rw-r--r--   0        0        0      989 2023-07-04 09:23:16.797987 syntaxlight-0.0.3/syntaxlight/parsers/ebnf_parser.py
--rw-r--r--   0        0        0     5758 2023-07-10 15:27:05.012220 syntaxlight-0.0.3/syntaxlight/parsers/json_parser.py
--rw-r--r--   0        0        0     8883 2023-07-20 08:24:16.172052 syntaxlight-0.0.3/syntaxlight/parsers/parser.py
--rw-r--r--   0        0        0      405 2023-07-12 06:09:27.902688 syntaxlight-0.0.3/syntaxlight/parsers/shell_parser.py
--rw-r--r--   0        0        0    11786 2023-07-16 15:52:23.224969 syntaxlight-0.0.3/syntaxlight/parsers/toml_parser.py
--rw-r--r--   0        0        0     6531 2023-07-15 15:57:39.737127 syntaxlight-0.0.3/syntaxlight/parsers/xml_parser.py
--rw-r--r--   0        0        0     3835 2023-07-20 09:36:05.046073 syntaxlight-0.0.3/syntaxlight/syntax_parse.py
--rw-r--r--   0        0        0      405 2023-06-15 12:50:36.421265 syntaxlight-0.0.3/syntaxlight/template.html
--rw-r--r--   0        0        0     2274 1970-01-01 00:00:00.000000 syntaxlight-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.0.4/LICENSE
+-rw-r--r--   0        0        0      464 2023-07-21 06:02:06.182590 syntaxlight-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1632 2023-07-20 09:56:07.920078 syntaxlight-0.0.4/README.md
+-rw-r--r--   0        0        0      191 2023-07-19 07:19:43.518938 syntaxlight-0.0.4/syntaxlight/__init__.py
+-rw-r--r--   0        0        0    13864 2023-07-20 09:35:37.730553 syntaxlight-0.0.4/syntaxlight/ast.py
+-rw-r--r--   0        0        0     2223 2023-07-19 06:56:41.644931 syntaxlight-0.0.4/syntaxlight/css/all.css
+-rw-r--r--   0        0        0     2081 2023-07-19 08:12:53.632477 syntaxlight-0.0.4/syntaxlight/css/c.css
+-rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.0.4/syntaxlight/css/index.css
+-rw-r--r--   0        0        0      485 2023-07-19 08:11:30.544637 syntaxlight-0.0.4/syntaxlight/css/json.css
+-rw-r--r--   0        0        0     2720 2023-07-20 08:04:28.110565 syntaxlight-0.0.4/syntaxlight/css/themes.json
+-rw-r--r--   0        0        0      557 2023-07-19 08:11:34.232315 syntaxlight-0.0.4/syntaxlight/css/toml.css
+-rw-r--r--   0        0        0      495 2023-07-19 08:15:19.310673 syntaxlight-0.0.4/syntaxlight/css/xml.css
+-rw-r--r--   0        0        0     2379 2023-07-17 06:49:24.804921 syntaxlight-0.0.4/syntaxlight/error.py
+-rw-r--r--   0        0        0     1995 2023-07-21 06:00:15.010137 syntaxlight-0.0.4/syntaxlight/example.py
+-rw-r--r--   0        0        0     1664 2023-07-19 08:35:00.594467 syntaxlight-0.0.4/syntaxlight/export.py
+-rw-r--r--   0        0        0      406 2023-07-20 13:32:30.588909 syntaxlight-0.0.4/syntaxlight/lexers/__init__.py
+-rw-r--r--   0        0        0    12379 2023-07-19 02:03:36.729775 syntaxlight-0.0.4/syntaxlight/lexers/c_lexer.py
+-rw-r--r--   0        0        0     2219 2023-07-04 09:22:19.741835 syntaxlight-0.0.4/syntaxlight/lexers/ebnf_lexer.py
+-rw-r--r--   0        0        0     1864 2023-07-04 09:20:59.243201 syntaxlight-0.0.4/syntaxlight/lexers/json_lexer.py
+-rw-r--r--   0        0        0    19627 2023-07-19 02:25:52.820410 syntaxlight-0.0.4/syntaxlight/lexers/lexer.py
+-rw-r--r--   0        0        0     4090 2023-06-16 15:53:43.032864 syntaxlight-0.0.4/syntaxlight/lexers/lua_lexer.py
+-rw-r--r--   0        0        0     1801 2023-07-12 06:24:11.777365 syntaxlight-0.0.4/syntaxlight/lexers/shell_lexer.py
+-rw-r--r--   0        0        0     3538 2023-07-06 06:05:23.042009 syntaxlight-0.0.4/syntaxlight/lexers/toml_lexer.py
+-rw-r--r--   0        0        0     4578 2023-07-20 13:32:30.928035 syntaxlight-0.0.4/syntaxlight/lexers/xml_lexer.py
+-rw-r--r--   0        0        0      205 2023-07-12 06:09:50.252799 syntaxlight-0.0.4/syntaxlight/parsers/__init__.py
+-rw-r--r--   0        0        0   100677 2023-07-21 05:59:31.524515 syntaxlight-0.0.4/syntaxlight/parsers/c_parser.py
+-rw-r--r--   0        0        0      989 2023-07-04 09:23:16.797987 syntaxlight-0.0.4/syntaxlight/parsers/ebnf_parser.py
+-rw-r--r--   0        0        0     5758 2023-07-10 15:27:05.012220 syntaxlight-0.0.4/syntaxlight/parsers/json_parser.py
+-rw-r--r--   0        0        0     8881 2023-07-21 05:50:20.656491 syntaxlight-0.0.4/syntaxlight/parsers/parser.py
+-rw-r--r--   0        0        0      405 2023-07-12 06:09:27.902688 syntaxlight-0.0.4/syntaxlight/parsers/shell_parser.py
+-rw-r--r--   0        0        0    11786 2023-07-16 15:52:23.224969 syntaxlight-0.0.4/syntaxlight/parsers/toml_parser.py
+-rw-r--r--   0        0        0     6531 2023-07-15 15:57:39.737127 syntaxlight-0.0.4/syntaxlight/parsers/xml_parser.py
+-rw-r--r--   0        0        0     3835 2023-07-21 05:48:12.460063 syntaxlight-0.0.4/syntaxlight/syntax_parse.py
+-rw-r--r--   0        0        0      405 2023-06-15 12:50:36.421265 syntaxlight-0.0.4/syntaxlight/template.html
+-rw-r--r--   0        0        0     2274 1970-01-01 00:00:00.000000 syntaxlight-0.0.4/PKG-INFO
```

### Comparing `syntaxlight-0.0.3/LICENSE` & `syntaxlight-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/README.md` & `syntaxlight-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/ast.py` & `syntaxlight-0.0.4/syntaxlight/ast.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/css/all.css` & `syntaxlight-0.0.4/syntaxlight/css/all.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/css/c.css` & `syntaxlight-0.0.4/syntaxlight/css/c.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/css/index.css` & `syntaxlight-0.0.4/syntaxlight/css/index.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/css/themes.json` & `syntaxlight-0.0.4/syntaxlight/css/themes.json`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/css/toml.css` & `syntaxlight-0.0.4/syntaxlight/css/toml.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/error.py` & `syntaxlight-0.0.4/syntaxlight/error.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/example.py` & `syntaxlight-0.0.4/syntaxlight/example.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/export.py` & `syntaxlight-0.0.4/syntaxlight/export.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/lexers/c_lexer.py` & `syntaxlight-0.0.4/syntaxlight/lexers/c_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/lexers/ebnf_lexer.py` & `syntaxlight-0.0.4/syntaxlight/lexers/ebnf_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/lexers/json_lexer.py` & `syntaxlight-0.0.4/syntaxlight/lexers/json_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/lexers/lexer.py` & `syntaxlight-0.0.4/syntaxlight/lexers/lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/lexers/lua_lexer.py` & `syntaxlight-0.0.4/syntaxlight/lexers/lua_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/lexers/shell_lexer.py` & `syntaxlight-0.0.4/syntaxlight/lexers/shell_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/lexers/toml_lexer.py` & `syntaxlight-0.0.4/syntaxlight/lexers/toml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/lexers/xml_lexer.py` & `syntaxlight-0.0.4/syntaxlight/lexers/xml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/parsers/c_parser.py` & `syntaxlight-0.0.4/syntaxlight/parsers/c_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -681,17 +681,16 @@
         在这里没有办法区分, 需要查看 <declarator> 后面是否有<declaration>* 和 <compound-statement> 才可以确定是 <function-definition>
 
         @扩展文法
         添加 <group> <statement> 以适配宏定义与开头的陈述语句. C 默认不支持 if for 作为陈述语句, 这里添加对于代码段的扩展支持
         """
         # @修改文法
         # 当无 <declaration-specifier>* (无类型) 只有 <declarator> 的时候匹配 <function_definition>
-        if self.current_token.type in self.cfirst_set.declarator:
-            return self.function_definition()
-        elif self.current_token.type in self.cfirst_set.group:
+        self._unknown_typedef_id_guess()
+        if self.current_token.type in self.cfirst_set.group:
             return self.group()
         elif self.current_token.type in self.cfirst_set.declaration:
             return self.declaration()
         elif self.current_token.type in self.cfirst_set.statement:
             return self.statement()
         else:  # pragma: no cover
             self.error(
@@ -884,16 +883,18 @@
         #             ErrorCode.UNEXPECTED_TOKEN,
         #             "Declaration of anonymous struct must be a definition",
         #         )
         # struct or union 有定义 {}
         if self.current_token.type == TokenType.LCURLY_BRACE:
             node.register_token(self.eat(TokenType.LCURLY_BRACE))
             struct_declarations = []
+            self._unknown_typedef_id_guess()
             while self.current_token.type in self.cfirst_set.struct_declaration:
                 struct_declarations.append(self.struct_declaration())
+                self._unknown_typedef_id_guess()
             node.update(declarations=struct_declarations)
             node.register_token(self.eat(TokenType.RCURLY_BRACE))
 
             # 匿名 struct 且未定义成员
             if len(struct_declarations) == 0 and node.id is None:
                 self.warning("unnamed struct/union that defines no instances", node)
         add_ast_type(node.id, "StructClass")
```

### Comparing `syntaxlight-0.0.3/syntaxlight/parsers/ebnf_parser.py` & `syntaxlight-0.0.4/syntaxlight/parsers/ebnf_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/parsers/json_parser.py` & `syntaxlight-0.0.4/syntaxlight/parsers/json_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/parsers/parser.py` & `syntaxlight-0.0.4/syntaxlight/parsers/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ..ast import AST
 from typing import List
 import sys
 import html
 import traceback
 
 DEBUG = False
-# DEBUG = True
+DEBUG = True
 
 
 class Parser:
     def __init__(
         self, lexer, skip_invisible_characters=True, skip_space=True, display_warning=True
     ):
         self.lexer: Lexer = lexer
```

### Comparing `syntaxlight-0.0.3/syntaxlight/parsers/toml_parser.py` & `syntaxlight-0.0.4/syntaxlight/parsers/toml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/parsers/xml_parser.py` & `syntaxlight-0.0.4/syntaxlight/parsers/xml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/syntaxlight/syntax_parse.py` & `syntaxlight-0.0.4/syntaxlight/syntax_parse.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.3/PKG-INFO` & `syntaxlight-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntaxlight
-Version: 0.0.3
+Version: 0.0.4
 Summary: syntax highlight based on EBNF
 Home-page: https://github.com/luzhixing12345/syntaxlight
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

