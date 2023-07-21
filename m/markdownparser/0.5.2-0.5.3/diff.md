# Comparing `tmp/markdownparser-0.5.2.tar.gz` & `tmp/markdownparser-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdownparser-0.5.2.tar", max compression
+gzip compressed data, was "markdownparser-0.5.3.tar", max compression
```

## Comparing `markdownparser-0.5.2.tar` & `markdownparser-0.5.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.5.2/LICENSE
--rw-r--r--   0        0        0       92 2023-06-06 07:15:33.183694 markdownparser-0.5.2/MarkdownParser/__init__.py
--rw-r--r--   0        0        0     5714 2023-07-04 02:43:15.157813 markdownparser-0.5.2/MarkdownParser/base_class.py
--rw-r--r--   0        0        0    24198 2023-07-04 02:42:34.319849 markdownparser-0.5.2/MarkdownParser/block_parser.py
--rw-r--r--   0        0        0     6816 2023-07-04 02:43:23.168362 markdownparser-0.5.2/MarkdownParser/core.py
--rw-r--r--   0        0        0     3294 2023-07-04 02:43:24.968451 markdownparser-0.5.2/MarkdownParser/preprocess_parser.py
--rw-r--r--   0        0        0    21725 2023-07-04 02:43:27.560920 markdownparser-0.5.2/MarkdownParser/tree_parser.py
--rw-r--r--   0        0        0      442 2023-07-04 02:43:51.562365 markdownparser-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     4743 2023-07-04 02:30:14.376256 markdownparser-0.5.2/README.md
--rw-r--r--   0        0        0     5516 1970-01-01 00:00:00.000000 markdownparser-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.5.3/LICENSE
+-rw-r--r--   0        0        0       92 2023-06-06 07:15:33.183694 markdownparser-0.5.3/MarkdownParser/__init__.py
+-rw-r--r--   0        0        0     5967 2023-07-21 08:41:10.601700 markdownparser-0.5.3/MarkdownParser/base_class.py
+-rw-r--r--   0        0        0    24813 2023-07-21 08:38:15.300746 markdownparser-0.5.3/MarkdownParser/block_parser.py
+-rw-r--r--   0        0        0     6816 2023-07-21 08:38:25.951898 markdownparser-0.5.3/MarkdownParser/core.py
+-rw-r--r--   0        0        0     3283 2023-07-21 08:06:23.941552 markdownparser-0.5.3/MarkdownParser/preprocess_parser.py
+-rw-r--r--   0        0        0    21734 2023-07-21 08:36:10.839905 markdownparser-0.5.3/MarkdownParser/tree_parser.py
+-rw-r--r--   0        0        0      442 2023-07-21 08:44:58.581972 markdownparser-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     4827 2023-07-04 02:51:45.730014 markdownparser-0.5.3/README.md
+-rw-r--r--   0        0        0     5600 1970-01-01 00:00:00.000000 markdownparser-0.5.3/PKG-INFO
```

### Comparing `markdownparser-0.5.2/LICENSE` & `markdownparser-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.2/MarkdownParser/base_class.py` & `markdownparser-0.5.3/MarkdownParser/base_class.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import re
+from typing import List, Dict, Union
 
 
 class Container:
     # 用于记录全局解析时的中间变量替换
 
     def __init__(self) -> None:
-        self._container = {
+        self._container:Dict[str,Block] = {
             # block类名-唯一标识符 : block类对象
             #
         }
 
         self._counter = 0
         self.__str__ = self.__repr__
 
@@ -35,15 +36,15 @@
 
 
 CONTAINER = Container()
 
 
 class Parser:
     def __init__(self) -> None:
-        self._handlers = []  # 保存所有注册的方法
+        self._handlers:List[Dict[str, Handler]] = []  # 保存所有注册的方法
         self.is_sorted = False
 
     def _sort(self):
         # 按照优先级从高到低排序,使得解析时依次调用方法
         self._handlers.sort(key=lambda item: item["priority"], reverse=True)
 
     def __call__(self, *args, **kwargs):  # pragma: no cover
@@ -55,26 +56,29 @@
             self._sort()
         for method in self._handlers:
             name = method["name"]
             class_name = method["object"].__class__.__name__
             priority = method["priority"]
             print(f"[{name}]({priority}) : {class_name}")
 
-    def register(self, class_object: object, priority: int = 0) -> None:
-        new_method = {"priority": priority, "object": class_object}
-
+    def register(self, handler: "Handler", priority: int = 0) -> None:
+        handler.parser = self
+        new_method = {"priority": priority, "object": handler}
         self._handlers.append(new_method)
 
+    def match(self, root: "Block", text: str): # pragma: no cover
+        raise NotImplementedError
+
 
 class Block:
     def __init__(self, **kwargs) -> None:
-        self.input = kwargs
+        self.input:Dict[str, Union[str, Block]] = kwargs
         self.input["text"]: str  # 输入的纯文本,用于恢复原始信息
         self.input["word"]: str  # 解析提取后的核心文本信息
-        self.sub_blocks = []  # 子模块
+        self.sub_blocks: List[Block] = []  # 子模块
         self.block_name = self.__class__.__name__
 
     def register(self, class_object):
         global CONTAINER
         return CONTAINER.register(class_object)
 
     def restore(self, TextBlock):
@@ -148,29 +152,29 @@
         if header_navigater:
             return f"{header_navigater}<div class='markdown-body'>{content}</div>"
         else:
             return f"<div class='markdown-body'>{content}</div>"
 
 
 class Handler:
-    def __init__(self, parser=None) -> None:
-        self.RE = None
-        self.parser: Parser = parser
+    def __init__(self) -> None:
+        self.RE: re.Pattern = None
+        self.parser:Parser = None
 
     def match(self, text: str, *args):  # pragma: no cover
         if self.RE is None:
             raise NotImplementedError
 
         return bool(self.RE.search(text))
 
     def __call__(self, root: Block, text: str):  # pragma: no cover
         raise NotImplementedError
 
 
 class Optimizer:
     def __init__(self) -> None:
         # 优化器针对的Block
-        self.target_block_names = []
+        self.target_block_names:List[str] = []
         self.is_match = False
 
     def __call__(self, root: Block):  # pragma: no cover
         raise NotImplementedError
```

### Comparing `markdownparser-0.5.2/MarkdownParser/block_parser.py` & `markdownparser-0.5.3/MarkdownParser/block_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .base_class import Parser, Handler, Block, CONTAINER
 from typing import List
 import re
+import html
 
 
 class BlockParser(Parser):
     def __init__(self) -> None:
         super().__init__()
 
     def __call__(self, lines: List[str]):
@@ -62,16 +63,16 @@
     def toHTML(self):
         return ""
 
 
 class EmptyBlockHandler(Handler):
     # 处理空行
 
-    def __init__(self, parser) -> None:
-        super().__init__(parser)
+    def __init__(self) -> None:
+        super().__init__()
 
     def match(self, text: str):
         return not text.strip()
 
     def __call__(self, root: Block, text: str):
         root.addBlock(EmptyBlock(text=text))
 
@@ -81,34 +82,32 @@
         super().__init__(**kwargs)
 
     def toHTML(self):
         return ""
 
 
 class EscapeCharacterHandler(Handler):
-    # 解释一下这里
-    # 这里的方法名和preprocess_parser中有着同名方法EscapeCharacterHandler
-    # 这里用于处理恢复为纯文本后再处理的情况, 因为预处理阶段优先级较高
-    # 对于类似table的匹配会出现重新恢复文本,分割后再依次匹配的情况
+    # preprocess_parser中有着同名方法EscapeCharacterHandler
+    # 但修改了其 __call__ 参数
 
-    def __init__(self, parser=None) -> None:
-        super().__init__(parser)
+    def __init__(self) -> None:
+        super().__init__()
         self.RE = re.compile(r"\\(.)")
 
-    def subFunc(self, match):
+    def sub_func(self, match: re.Match):
         global CONTAINER
         word = match.group(1)
         block = EscapeCharacterBlock(word=word, text="\\" + word)
         replace_name = self.block.register(block)  # 注册并替换名字
         return replace_name
 
     def __call__(self, root: Block, text: str):
         self.block = ComplexBlock(text=text)
         # 替换所有匹配项并重新解析new_text
-        new_text = re.sub(self.RE, self.subFunc, text)
+        new_text = re.sub(self.RE, self.sub_func, text)
         self.parser.match(self.block, new_text)
         # 单匹配去掉外层 ComplexBlock
         if len(self.block.sub_blocks) == 1:
             self.block = self.block.sub_blocks[0]
         root.addBlock(self.block)
 
 
@@ -150,25 +149,58 @@
     def toHTML(self):
         if self.input["word"] in self.special_characters:
             return self.input["word"]
         else:
             return "\\" + self.input["word"]
 
 
-# 已废弃
+class HTMLLabelHandler(Handler):
+    # preprocess_parser 中有着同名方法 HTMLLabelHandler
+    # 但修改了其 __call__ 参数
+
+    def __init__(self) -> None:
+        super().__init__()
+
+        self.RE = re.compile(
+            r"""
+            (<div[\s\S]*?>[\s\S]*?<\/div>|         # div
+            <span[\s\S]*?>[\s\S]*?<\/span>|        # span
+            <p[\s\S]*?>[\s\S]*?<\/p>|            # p
+            <img[\s\S]*?>(?:<\/img>)?|   # image
+            <iframe[\s\S]*?>[\s\S]*?<\/iframe>|    # iframe
+            <br\/?>|
+            <kbd>[\s\S]*?</kbd>
+            )""",
+            re.VERBOSE,
+        )
+
+    def sub_func(self, match: re.Match):
+        global CONTAINER
+        src = match.group(0)
+        block = HTMLBlock(text=src, word=src)
+        return CONTAINER.register(block)
 
+    def __call__(self, root: Block, text: str):
+        self.block = ComplexBlock(text=text)
+        # 替换所有匹配项并重新解析new_text
+        new_text = re.sub(self.RE, self.sub_func, text)
+        self.parser.match(self.block, new_text)
+        # 单匹配去掉外层 ComplexBlock
+        if len(self.block.sub_blocks) == 1:
+            self.block = self.block.sub_blocks[0]
+        root.addBlock(self.block)
 
 class ExtensionBlockHandler(Handler):  # pragma: no cover
     # 自定义扩展
     # {% note %}
     # asdklja
     # {%end%}
 
-    def __init__(self, parser=None) -> None:
-        super().__init__(parser)
+    def __init__(self) -> None:
+        super().__init__()
         self.RE = re.compile(
             r"""(
             (^{[ ]*%[ ]*note[ ]*%[ ]*}[ ]*)|
             (^{[ ]*%[ ]*info[ ]*%[ ]*}[ ]*)|
             (^{[ ]*%[ ]*success[ ]*%[ ]*}[ ]*)|
             (^{[ ]*%[ ]*end[ ]*%[ ]*}[ ]*)
         )""",
@@ -198,16 +230,16 @@
         content = ""
         for block in self.sub_blocks:
             content += block.toHTML()
         return f'<div id="{tag}">{content}</div>'
 
 
 class SplitBlockHandler(Handler):
-    def __init__(self, parser) -> None:
-        super().__init__(parser)
+    def __init__(self) -> None:
+        super().__init__()
         self.RE = re.compile(r"^[-=\*]{3,} *$")  # 分隔符
 
     def __call__(self, root: Block, text: str):
         root.addBlock(SplitBlock(text=text))
 
 
 class SplitBlock(Block):
@@ -223,16 +255,16 @@
 
 class HierarchyIndentHandler(Handler):
     # 匹配层次缩进
     # - 123
     #   hello world
     #   good luck
 
-    def __init__(self, parser) -> None:
-        super().__init__(parser)
+    def __init__(self) -> None:
+        super().__init__()
         self.RE = re.compile(r"^([ ]{1,})(.*)")
 
     def __call__(self, root: Block, text: str):
         match_group = re.match(self.RE, text)
         space_number = len(match_group.group(1))
         word = match_group.group(2)
 
@@ -252,16 +284,16 @@
 
 class CodeBlockHandler(Handler):
     # 匹配代码段
     # ```python
     # a = 1
     # ```
 
-    def __init__(self, parser) -> None:
-        super().__init__(parser)
+    def __init__(self) -> None:
+        super().__init__()
         self.RE = re.compile(r"`{3,}(.*)")
 
     def __call__(self, root: Block, text: str):
         match_group = re.match(self.RE, text)
         language = match_group.group(1).strip()
 
         if language:
@@ -275,28 +307,25 @@
 class CodeBlock(Block):
     def __init__(self, **kwargs) -> None:
         # code用于在优化阶段用于整合所有的代码
         super().__init__(code="", **kwargs)
 
     def toHTML(self):
         code = self.input["code"]
-        code = re.sub("<", "&lt;", code)
-        code = re.sub(">", "&gt;", code)
+        code = html.escape(code)
         language = self.input["language"]
         return f'<pre><code class="language-{language}">{code}</code></pre>'
 
 
 class HashHeaderHandler(Handler):
     # 匹配标题
     # ### 123
 
-    def __init__(self, parser) -> None:
-        super().__init__(parser)
-        self.parser = parser
-
+    def __init__(self) -> None:
+        super().__init__()
         # #开头,1-6个#均可 + 一个空格 + 文字
         # Typora               r'(^#{1,6}) (.+)'
         # Markdown All in One  r'(^#{1,6}) (.?)'
         self.RE = re.compile(r"(^#{1,6}) (.+)")
 
     def __call__(self, root: Block, text: str):
         match_group = re.match(self.RE, text)
@@ -336,30 +365,30 @@
                 word += sblock.input["word"]
         else:
             word = self.sub_blocks[0].input["word"]
         return word
 
 
 class TaskListHandler(Handler):
-    def __init__(self, parser) -> None:
-        super().__init__(parser)
+    def __init__(self) -> None:
+        super().__init__()
         self.RE = re.compile(r"(?<=^[-+\*] )\[([ x])\] (.*)")
 
-    def subFunc(self, match: re.Match):
+    def sub_func(self, match: re.Match):
         is_complete = match.group(1)
         word = match.group(2)
 
         task_block = TaskListBlock(complete=is_complete, word=word, text=match.group())
         replace_name = self.block.register(task_block)  # 注册并替换名字
         return replace_name
 
     def __call__(self, root: Block, text: str):
         self.block = ComplexBlock(text=text)
         # 替换所有匹配项并重新解析new_text
-        new_text = re.sub(self.RE, self.subFunc, text)
+        new_text = re.sub(self.RE, self.sub_func, text)
         self.parser.match(self.block, new_text)
         # 单匹配去掉外层 ComplexBlock
         if len(self.block.sub_blocks) == 1:
             self.block = self.block.sub_blocks[0]
         root.addBlock(self.block)
 
 
@@ -374,16 +403,16 @@
 
 
 class OListHandler(Handler):
     # 匹配有序列表
     # 1. 123
     # 2. 123
 
-    def __init__(self, parser) -> None:
-        super().__init__(parser)
+    def __init__(self) -> None:
+        super().__init__()
         self.RE = re.compile(r"^(\d+)\. (.*)")
 
     def __call__(self, root: Block, text: str):
         match_group = re.match(self.RE, text)
         serial_number = match_group.group(1)
         align_space_number = len(serial_number) + 2
         word = match_group.group(2)
@@ -404,16 +433,16 @@
         for block in self.sub_blocks:
             content += block.toHTML()
         serial_number = self.input["serial_number"]
         return f'<ol start="{serial_number}"><li>{content}</li></ol>'
 
 
 class UListHandler(Handler):
-    def __init__(self, parser) -> None:
-        super().__init__(parser)
+    def __init__(self) -> None:
+        super().__init__()
         self.RE = re.compile(r"^[-+\*] (.*)")
 
     def __call__(self, root: Block, text: str):
         match_group = re.match(self.RE, text)
         word = match_group.group(1)
         align_space_number = 2
 
@@ -433,16 +462,16 @@
 
         return f"<ul><li>{content}</li></ul>"
 
 
 class QuoteHandler(Handler):
     # 匹配引用
     # > 123
-    def __init__(self, parser) -> None:
-        super().__init__(parser)
+    def __init__(self) -> None:
+        super().__init__()
         self.RE = re.compile(r"^>[ ]*(.*)")
 
     def __call__(self, root: Block, text: str):
         match_group = re.match(self.RE, text)
         word = match_group.group(1)
         block = QuoteBlock(word=word, text=text)
         self.parser.match(block, word)
@@ -461,29 +490,29 @@
         return f"<blockquote>{content}</blockquote>"
 
 
 class PictureHandler(Handler):
     # 匹配图片
     # ![asd](123)
 
-    def __init__(self, parser) -> None:
-        super().__init__(parser)
+    def __init__(self) -> None:
+        super().__init__()
         self.RE = re.compile(r"!\[([^\!\[\]]*?)\]\((.*?)\)")
 
-    def subFunc(self, match: re.Match):
+    def sub_func(self, match: re.Match):
         word = match.group(1)
         url = match.group(2)
         pic_block = PictureBlock(word=word, url=url, text=match.group())
         replace_name = self.block.register(pic_block)  # 注册并替换名字
         return replace_name
 
     def __call__(self, root: Block, text: str):
         self.block = ComplexBlock(text=text)
         # 替换所有匹配项并重新解析new_text
-        new_text = re.sub(self.RE, self.subFunc, text)
+        new_text = re.sub(self.RE, self.sub_func, text)
 
         self.parser.match(self.block, new_text)
         # 单匹配去掉外层 ComplexBlock
         if len(self.block.sub_blocks) == 1:
             self.block = self.block.sub_blocks[0]
 
         root.addBlock(self.block)
@@ -499,30 +528,30 @@
         return f'<img src="{url}" alt="{word}">'
 
 
 class ReferenceHandler(Handler):
     # 处理引用
     # [1](abc)
 
-    def __init__(self, parser) -> None:
-        super().__init__(parser)
+    def __init__(self) -> None:
+        super().__init__()
         # 匹配嵌套 + 忽略末尾多余 )
 
         # Typora               r'\[([^\[\]]*?)\]\((.*?)\)'
         # Markdown All in One  ...
         self.RE = re.compile(
             r"""(
             \[(.*?)\]\((.*?)\)|
-            <(https?:\/\/[\w\-_]+(?:\.[\w\-_]+)+(?:[\w\-\.,@?^=%&:\/~\+#]*[\w\-\@?^=%&\/~\+#])?)>|
-            \bhttps?:\/\/[\w\-_]+(?:\.[\w\-_]+)+(?:[\w\-\.,@?^=%&:\/~\+#]*[\w\-\@?^=%&\/~\+#])?\b
+            <(https?:\/\/[\w\-_]+(?:\.[\w\-_]+)+(?:[\w\-\.,@?^=%&:\/~\+#]*[\w\-\@?^=%&\/~\+#])?(?:;[\w\-\.,@?^=%&:\/~\+#=]*)?)>|
+            \bhttps?:\/\/[\w\-_]+(?:\.[\w\-_]+)+(?:[\w\-\.,@?^=%&:\/~\+#]*[\w\-\@?^=%&\/~\+#])?(?:;[\w\-\.,@?^=%&:\/~\+#=]*)?\b
         )""",
             re.VERBOSE,
         )
 
-    def subFunc(self, match: re.Match):
+    def sub_func(self, match: re.Match):
         word = match.group(2)
         url = match.group(3)
 
         if url is None:
             # <> 的匹配
             url = match.group(4)
             if url is None:
@@ -532,15 +561,15 @@
         ref_block = ReferenceBlock(word=word, url=url, text=match.group())
         replace_name = self.block.register(ref_block)  # 注册并替换名字
         return replace_name
 
     def __call__(self, root: Block, text: str):
         self.block = ComplexBlock(text=text)
         # 替换所有匹配项并重新解析new_text
-        new_text = re.sub(self.RE, self.subFunc, text)
+        new_text = re.sub(self.RE, self.sub_func, text)
         self.parser.match(self.block, new_text)
         # 单匹配去掉外层 ComplexBlock
         if len(self.block.sub_blocks) == 1:
             self.block = self.block.sub_blocks[0]
         root.addBlock(self.block)
 
 
@@ -559,16 +588,16 @@
         return f'<a href="{url}" target="{self.target}">{content}</a>'
 
 
 class SpecialTextHandler(Handler):
     # 处理特殊字符
     # 不考虑 * 的多级嵌套
 
-    def __init__(self, parser) -> None:
-        super().__init__(parser)
+    def __init__(self) -> None:
+        super().__init__()
         self.RE = re.compile(
             r"""(
             \*{3}(.+?)\*{3}|                           # 粗体+斜体
             \*{2}(.+?)\*{2}|                           # 粗体
             \*(.+?)\*|                                 # 斜体
             ~~(.+?)~~|                                 # 删除线
             ``(.+?)``|                                 # 高亮
@@ -581,28 +610,28 @@
             3: "bold",
             4: "italic",
             5: "delete",
             6: "highlight",
             7: "highlight",
         }
 
-    def subFunc(self, match: re.Match):
+    def sub_func(self, match: re.Match):
         for k, v in self.groupid_tag.items():
             if match.group(k):
                 word = match.group(k)
                 tag = v
                 break
         special_text_block = SpecialTextBlock(word=word, tag=tag, text=match.group())
         replace_name = self.block.register(special_text_block)  # 注册并替换名字
         return replace_name
 
     def __call__(self, root: Block, text: str):
         self.block = ComplexBlock(text=text)
         # 替换所有匹配项并重新解析new_text
-        new_text = re.sub(self.RE, self.subFunc, text)
+        new_text = re.sub(self.RE, self.sub_func, text)
 
         self.parser.match(self.block, new_text)
         # 单匹配去掉外层 ComplexBlock
         if len(self.block.sub_blocks) == 1:
             self.block = self.block.sub_blocks[0]
         root.addBlock(self.block)
 
@@ -628,16 +657,16 @@
             return f"<code>{content}</code>"
 
 
 class TableHandler(Handler):
     # 处理表格
     # 不想支持原生表格...
 
-    def __init__(self, parser) -> None:
-        super().__init__(parser)
+    def __init__(self) -> None:
+        super().__init__()
         self.RE = re.compile(r"^\|(?: *:?-{1,}:? *\|)+")  # 判断表格出现
 
     def __call__(self, root: Block, text: str):
         # 判断对齐方式
         lines = text.split("|")[1:-1]
         alignments = []
         for line in lines:
@@ -682,16 +711,16 @@
 
         return f"<table>{table_header_content}{table_items_content}</table>"
 
 
 class TextHandler(Handler):
     # 处理常规文本
 
-    def __init__(self, parser) -> None:
-        super().__init__(parser)
+    def __init__(self) -> None:
+        super().__init__()
 
     def match(self, text: str):
         return True
 
     def __call__(self, root: Block, text: str):
         global CONTAINER
         RE = re.compile(r"({-%.*?%-})")
@@ -729,31 +758,30 @@
 class TextBlock(Block):
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     def toHTML(self):
         # fix bug: 修复一些 <abc> 这种虽然不匹配网址, 但是会被 html 解析为标签的情况
         # 见 test14.md
-        self.input["word"] = self.input["word"].replace("<", "&lt").replace(">", "&gt")
-
+        self.input["word"] = html.escape(self.input["word"])
         return self.input["word"]
 
 
 def buildBlockParser():
     # block parser 用于逐行处理文本, 并将结果解析为一颗未优化的树
     block_parser = BlockParser()
-    block_parser.register(EmptyBlockHandler(block_parser), 100)
-    block_parser.register(EscapeCharacterHandler(block_parser), 98)
-    block_parser.register(SplitBlockHandler(block_parser), 95)
-    block_parser.register(HierarchyIndentHandler(block_parser), 90)
-    block_parser.register(HashHeaderHandler(block_parser), 80)
-    block_parser.register(TaskListHandler(block_parser), 70)
-    block_parser.register(OListHandler(block_parser), 60)
-    block_parser.register(UListHandler(block_parser), 50)
-    block_parser.register(QuoteHandler(block_parser), 40)
-    block_parser.register(CodeBlockHandler(block_parser), 30)
-    block_parser.register(PictureHandler(block_parser), 15)
-    block_parser.register(ReferenceHandler(block_parser), 10)
-    block_parser.register(SpecialTextHandler(block_parser), 5)
-    block_parser.register(TableHandler(block_parser), 4)
-    block_parser.register(TextHandler(block_parser), 0)
+    block_parser.register(EmptyBlockHandler(), 100)
+    block_parser.register(EscapeCharacterHandler(), 98)
+    block_parser.register(SplitBlockHandler(), 95)
+    block_parser.register(HierarchyIndentHandler(), 90)
+    block_parser.register(HashHeaderHandler(), 80)
+    block_parser.register(TaskListHandler(), 70)
+    block_parser.register(OListHandler(), 60)
+    block_parser.register(UListHandler(), 50)
+    block_parser.register(QuoteHandler(), 40)
+    block_parser.register(CodeBlockHandler(), 30)
+    block_parser.register(PictureHandler(), 15)
+    block_parser.register(ReferenceHandler(), 10)
+    block_parser.register(SpecialTextHandler(), 5)
+    block_parser.register(TableHandler(), 4)
+    block_parser.register(TextHandler(), 0)
     return block_parser
```

### Comparing `markdownparser-0.5.2/MarkdownParser/core.py` & `markdownparser-0.5.3/MarkdownParser/core.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.2/MarkdownParser/preprocess_parser.py` & `markdownparser-0.5.3/MarkdownParser/preprocess_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,42 +28,42 @@
 
         return text
 
 
 class EscapeCharacterHandler(Handler):
     # 处理转义字符
 
-    def __init__(self, parser=None) -> None:
-        super().__init__(parser)
+    def __init__(self) -> None:
+        super().__init__()
 
-    def subFunc(self, match):
+    def sub_func(self, match: re.Match):
         global CONTAINER
         word = match.group(1)
         block = EscapeCharacterBlock(word=word, text="\\" + word)
         return CONTAINER.register(block)
 
     def __call__(self, text: str):
-        text = re.sub(r"\\(.)", self.subFunc, text)
+        text = re.sub(r"\\(.)", self.sub_func, text)
         return text
 
 
 class AnnotateHandler(Handler):
     # 去除注释
 
-    def __init__(self, parser=None) -> None:
-        super().__init__(parser)
+    def __init__(self) -> None:
+        super().__init__()
 
-    def subFunc(self, match):
+    def sub_func(self, match: re.Match):
         global CONTAINER
         word = match.group()
         block = AnnotateBlock(word=word, text=word)
         return CONTAINER.register(block)
 
     def __call__(self, text: str):
-        text = re.sub(r"\<!--[\s\S]*?--\>", self.subFunc, text)  # 去除注释
+        text = re.sub(r"\<!--[\s\S]*?--\>", self.sub_func, text)  # 去除注释
         return text
 
 
 class HTMLLabelHandler(Handler):
     # TODO: 标签不自闭合的处理
 
     def __init__(self) -> None:
@@ -78,22 +78,22 @@
             <iframe[\s\S]*?>[\s\S]*?<\/iframe>|    # iframe
             <br\/?>|
             <kbd>[\s\S]*?</kbd>
             )""",
             re.VERBOSE,
         )
 
-    def __call__(self, text: str):
-        def subFunc(match):
-            global CONTAINER
-            src = match.group(0)
-            block = HTMLBlock(text=src, word=src)
-            return CONTAINER.register(block)
+    def sub_func(self, match: re.Match):
+        global CONTAINER
+        src = match.group(0)
+        block = HTMLBlock(text=src, word=src)
+        return CONTAINER.register(block)
 
-        text = re.sub(self.RE, subFunc, text)
+    def __call__(self, text: str):
+        text = re.sub(self.RE, self.sub_func, text)
         text = re.sub(r"^[\n]+", "", text)  # 去除开头连续空换行
         # text = re.sub(r'[\n]+$', '', text)                    # 去除结尾连续空换行
         # text = re.sub(r'[\n]{3,}', '\n\n', text)              # 去除连续换行
         # print(text)
         return text
```

### Comparing `markdownparser-0.5.2/MarkdownParser/tree_parser.py` & `markdownparser-0.5.3/MarkdownParser/tree_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,18 @@
     EmptyBlockHandler,
     EscapeCharacterHandler,
     PictureHandler,
     ReferenceHandler,
     SpecialTextHandler,
     TableHandler,
     TextHandler,
+    HTMLLabelHandler
 )
+from typing import List
+
 
 
 class TreeParser(Parser):
     def __init__(self) -> None:
         super().__init__()
 
     def __call__(self, root: Block):
@@ -337,38 +340,41 @@
         root.sub_blocks = new_sub_blocks
 
 
 class TableBlockOptimizer(Optimizer):
     def __init__(self) -> None:
         super().__init__()
         self.RE = re.compile(r"(?<!\\)\|")
-        self.block_parser = BlockParser()  # 初始化一个block parser 用于解析表格中出现的每一个表项,
+
+        # 初始化一个block parser 用于解析表格中出现的每一个表项
         # 只注册下面这些 Handler, 不解析其他的
-        self.block_parser.register(EmptyBlockHandler(self.block_parser), 100)
-        self.block_parser.register(EscapeCharacterHandler(self.block_parser), 98)
-        self.block_parser.register(PictureHandler(self.block_parser), 15)
-        self.block_parser.register(ReferenceHandler(self.block_parser), 10)
-        self.block_parser.register(SpecialTextHandler(self.block_parser), 5)
-        self.block_parser.register(TableHandler(self.block_parser), 4)
-        self.block_parser.register(TextHandler(self.block_parser), 0)
+        self.block_parser = BlockParser()
+        self.block_parser.register(EmptyBlockHandler(), 100)
+        self.block_parser.register(EscapeCharacterHandler(), 98)
+        self.block_parser.register(HTMLLabelHandler(),90)
+        self.block_parser.register(PictureHandler(), 15)
+        self.block_parser.register(ReferenceHandler(), 10)
+        self.block_parser.register(SpecialTextHandler(), 5)
+        self.block_parser.register(TableHandler(), 4)
+        self.block_parser.register(TextHandler(), 0)
         # 匹配的
         self.table_block_names = ["TableBlock"]
 
         # 表格匹配,其余中断
         self.header_block_names = ["TextBlock", "ComplexBlock"]
         self.body_block_names = ["TextBlock", "ComplexBlock", "TableBlock"]
 
     def _createTableBlock(self, header_block: Block, table_block: Block):
         # 判断header和table列是否匹配
         # 匹配返回一个TableBlock对象实例,用于后续补充表格
         # 不匹配返回None
         table_length = len(table_block.input["alignments"])
         header_text = header_block.input["text"]  # 获取原文
 
-        header = self.RE.split(header_text)
+        header: List[str] = self.RE.split(header_text)
         if len(header) - 2 != table_length:
             return None
 
         # 匹配,创建实例
         header = header[1:-1]
         for i in range(len(header)):
             header[i] = header[i].strip()
```

### Comparing `markdownparser-0.5.2/README.md` & `markdownparser-0.5.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -33,36 +33,29 @@
 # 解析 markdown 文本, 带目录树
 def parse_toc(text: str) -> str:
 
 # 解析 md 文件, 带目录树
 def parse_file_toc(file_name: str) -> str:
 ```
 
-## 测试
+## 结果预览与 Markdown 功能测试
+
+本仓库下提供了了一个快速验证转换结果的工具 generate.py
 
 ```bash
 python generate.py <FILE_NAME>
 
 # python generate.py ./testfiles/test1.md
 # python generate.py README.md
 ```
 
-运行会生成index.html, 使用浏览器打开生成的index.html即可与您的Markdown编辑器的预期渲染结果对比
+运行会生成index.html, 使用浏览器打开生成的index.html即可与您预期的渲染结果对比, README 的渲染结果如下所示
 
 ![20230218202400](https://raw.githubusercontent.com/learner-lu/picbed/master/20230218202400.png)
 
-代码覆盖率
-
-```bash
-pip install coverage
-
-coverage run -m unittest
-coverage html
-```
-
 ## 实现思路
 
 [Markdown解析器的代码实现](https://www.bilibili.com/video/BV1LA411X7X3)
 
 您可通过取消 [core.py](./MarkdownParser/core.py) 注释来获取树的结构
 
 ```python
@@ -83,16 +76,17 @@
 
 ## 不支持
 
 - 四个空格变为代码段
 - [^1]的引用方式
 - Setext 形式的标题
 - 上标 / 下标 / 下划线
+- `<details><summary></summary></details>` 折叠块
 
-## 补充说明
+## HTML 结果说明
 
 - 生成的结果如下 `<div class='markdown-body'>markdown内容</div>`
 - 代码段会根据语言加入一个类名便于后期高亮,例如 `class="language-cpp"`, 未定义语言则为 `language-UNKNOWN`
 - 默认导出的HTML中层级任务列表会有显示问题,这是因为使用了ul+li+checkbox的方式,您需要添加以下css样式修正
 
   ```css
   .markdown-body > ul>li:has(input) {
@@ -156,13 +150,12 @@
   <script id="MathJax-script" async
   src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js">
   </script>
   ```
 
   注意,这里仅支持很少一部分数学公式
 
-
-## 相关参考
+## 参考
 
 - [Github Markdown CSS](https://cdn.jsdelivr.net/npm/github-markdown-css@4.0.0/github-markdown.css)
 - [Mermaid API](https://mermaid.js.org/intro/#mermaid-api)
 - [MathJax](https://docs.mathjax.org/en/latest/web/start.html)
```

#### html2text {}

```diff
@@ -5,30 +5,31 @@
 install markdownparser ``` ## å¿«éä½¿ç¨ ```python import MarkdownParser html
 = MarkdownParser.parse('# Hello World!') print(html) #
 ****** Hello World! ******
 ``` æ¥å£å½æ° ```python # è§£æ markdown ææ¬è½¬ html def parse(text:
 str) -> str: # è§£æ md æä»¶è½¬ html def parse_file(file_name: str) -> str:
 # è§£æ markdown ææ¬, å¸¦ç®å½æ  def parse_toc(text: str) -> str: #
 è§£æ md æä»¶, å¸¦ç®å½æ  def parse_file_toc(file_name: str) -> str: ```
-## æµè¯ ```bash python generate.py  # python generate.py ./testfiles/test1.md
-# python generate.py README.md ``` è¿è¡ä¼çæindex.html,
-ä½¿ç¨æµè§å¨æå¼çæçindex.htmlå³å¯ä¸æ¨çMarkdownç¼è¾å¨çé¢ææ¸²æç»æå¯¹æ¯
-![20230218202400](https://raw.githubusercontent.com/learner-lu/picbed/master/
-20230218202400.png) ä»£ç è¦çç ```bash pip install coverage coverage run -
-m unittest coverage html ``` ## å®ç°æè·¯ [Markdownè§£æå¨çä»£ç å®ç°]
-(https://www.bilibili.com/video/BV1LA411X7X3) æ¨å¯éè¿åæ¶ [core.py](./
-MarkdownParser/core.py) æ³¨éæ¥è·åæ çç»æ ```python def parse(self,
-text: str) -> str: # å»é¤ç©ºè¡/æ³¨é/htmlæ ç­¾ lines =
-self.preprocess_parser(text) # print(lines) #
-éè¡è§£æ,å¾å°ä¸é¢æªä¼åçæ  root = self.block_parser(lines) #
-root.info() # ä¼å,å¾å°æ­£ç¡®çmarkdownè§£ææ  tree = self.tree_parser
-(root) # tree.info() # è¾åºå°å±å¹ / å¯¼åºhtmlæä»¶ return tree.toHTML()
-``` ## ä¸æ¯æ - åä¸ªç©ºæ ¼åä¸ºä»£ç æ®µ - [^1]çå¼ç¨æ¹å¼ - Setext
-å½¢å¼çæ é¢ - ä¸æ  / ä¸æ  / ä¸åçº¿ ## è¡¥åè¯´æ -
-çæçç»æå¦ä¸ `
+## ç»æé¢è§ä¸ Markdown åè½æµè¯
+æ¬ä»åºä¸æä¾äºäºä¸ä¸ªå¿«ééªè¯è½¬æ¢ç»æçå·¥å· generate.py
+```bash python generate.py  # python generate.py ./testfiles/test1.md # python
+generate.py README.md ``` è¿è¡ä¼çæindex.html,
+ä½¿ç¨æµè§å¨æå¼çæçindex.htmlå³å¯ä¸æ¨é¢æçæ¸²æç»æå¯¹æ¯,
+README çæ¸²æç»æå¦ä¸æç¤º ![20230218202400](https://
+raw.githubusercontent.com/learner-lu/picbed/master/20230218202400.png) ##
+å®ç°æè·¯ [Markdownè§£æå¨çä»£ç å®ç°](https://www.bilibili.com/video/
+BV1LA411X7X3) æ¨å¯éè¿åæ¶ [core.py](./MarkdownParser/core.py)
+æ³¨éæ¥è·åæ çç»æ ```python def parse(self, text: str) -> str: #
+å»é¤ç©ºè¡/æ³¨é/htmlæ ç­¾ lines = self.preprocess_parser(text) # print
+(lines) # éè¡è§£æ,å¾å°ä¸é¢æªä¼åçæ  root = self.block_parser
+(lines) # root.info() # ä¼å,å¾å°æ­£ç¡®çmarkdownè§£ææ  tree =
+self.tree_parser(root) # tree.info() # è¾åºå°å±å¹ / å¯¼åºhtmlæä»¶
+return tree.toHTML() ``` ## ä¸æ¯æ - åä¸ªç©ºæ ¼åä¸ºä»£ç æ®µ -
+[^1]çå¼ç¨æ¹å¼ - Setext å½¢å¼çæ é¢ - ä¸æ  / ä¸æ  / ä¸åçº¿ - ``
+æå å ## HTML ç»æè¯´æ - çæçç»æå¦ä¸ `
 markdownåå®¹
 ` - ä»£ç æ®µä¼æ ¹æ®è¯­è¨å å¥ä¸ä¸ªç±»åä¾¿äºåæé«äº®,ä¾å¦
 `class="language-cpp"`, æªå®ä¹è¯­è¨åä¸º `language-UNKNOWN` -
 é»è®¤å¯¼åºçHTMLä¸­å±çº§ä»»å¡åè¡¨ä¼ææ¾ç¤ºé®é¢,è¿æ¯å ä¸ºä½¿ç¨äºul+li+checkboxçæ¹å¼,æ¨éè¦æ·»å ä»¥ä¸cssæ ·å¼ä¿®æ­£
 ```css .markdown-body > ul>li:has(input) { padding-left: 0; margin-bottom: 0; }
 .markdown-body ul>li:has(input)>ul { list-style-type: none; padding-left: 8px;
 } ``` - æ¨å¯ä»¥ä½¿ç¨ `parse_toc` å° HashHeadBlock
@@ -47,11 +48,11 @@
 ` æ«å°¾æ·»å å¦ä¸ `
  ``` > **è¯·æ³¨æ**,
 ç±äºæ¬Markdownè§£æå¨çCodeBlockè§£æå¾å°çç±»åä¸º `language-
 mermaid`, èmermaidæä»¶æ¯æçç±»åæ ¼å¼ä¸º`mermaid`,
 æä»¥ä»£ç ä¸­æå¨ä¿®æ¹äº `language-mermaid` çç±»å -
 å¦ææ¨æ³æ·»å å¯¹Latexæ°å­¦å¬å¼çæ¯æ, å¯ä»¥å¨htmlé¡µé¢ `
 ` æ«å°¾æ·»å å¦ä¸ `
- ``` æ³¨æ,è¿éä»æ¯æå¾å°ä¸é¨åæ°å­¦å¬å¼ ## ç¸å³åè -
-[Github Markdown CSS](https://cdn.jsdelivr.net/npm/github-markdown-css@4.0.0/
-github-markdown.css) - [Mermaid API](https://mermaid.js.org/intro/#mermaid-api)
-- [MathJax](https://docs.mathjax.org/en/latest/web/start.html)
+ ``` æ³¨æ,è¿éä»æ¯æå¾å°ä¸é¨åæ°å­¦å¬å¼ ## åè - [Github
+Markdown CSS](https://cdn.jsdelivr.net/npm/github-markdown-css@4.0.0/github-
+markdown.css) - [Mermaid API](https://mermaid.js.org/intro/#mermaid-api) -
+[MathJax](https://docs.mathjax.org/en/latest/web/start.html)
```

### Comparing `markdownparser-0.5.2/PKG-INFO` & `markdownparser-0.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdownparser
-Version: 0.5.2
+Version: 0.5.3
 Summary: 
 Home-page: https://github.com/luzhixing12345/MarkdownParser
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -53,36 +53,29 @@
 # 解析 markdown 文本, 带目录树
 def parse_toc(text: str) -> str:
 
 # 解析 md 文件, 带目录树
 def parse_file_toc(file_name: str) -> str:
 ```
 
-## 测试
+## 结果预览与 Markdown 功能测试
+
+本仓库下提供了了一个快速验证转换结果的工具 generate.py
 
 ```bash
 python generate.py <FILE_NAME>
 
 # python generate.py ./testfiles/test1.md
 # python generate.py README.md
 ```
 
-运行会生成index.html, 使用浏览器打开生成的index.html即可与您的Markdown编辑器的预期渲染结果对比
+运行会生成index.html, 使用浏览器打开生成的index.html即可与您预期的渲染结果对比, README 的渲染结果如下所示
 
 ![20230218202400](https://raw.githubusercontent.com/learner-lu/picbed/master/20230218202400.png)
 
-代码覆盖率
-
-```bash
-pip install coverage
-
-coverage run -m unittest
-coverage html
-```
-
 ## 实现思路
 
 [Markdown解析器的代码实现](https://www.bilibili.com/video/BV1LA411X7X3)
 
 您可通过取消 [core.py](./MarkdownParser/core.py) 注释来获取树的结构
 
 ```python
@@ -103,16 +96,17 @@
 
 ## 不支持
 
 - 四个空格变为代码段
 - [^1]的引用方式
 - Setext 形式的标题
 - 上标 / 下标 / 下划线
+- `<details><summary></summary></details>` 折叠块
 
-## 补充说明
+## HTML 结果说明
 
 - 生成的结果如下 `<div class='markdown-body'>markdown内容</div>`
 - 代码段会根据语言加入一个类名便于后期高亮,例如 `class="language-cpp"`, 未定义语言则为 `language-UNKNOWN`
 - 默认导出的HTML中层级任务列表会有显示问题,这是因为使用了ul+li+checkbox的方式,您需要添加以下css样式修正
 
   ```css
   .markdown-body > ul>li:has(input) {
@@ -176,13 +170,12 @@
   <script id="MathJax-script" async
   src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js">
   </script>
   ```
 
   注意,这里仅支持很少一部分数学公式
 
-
-## 相关参考
+## 参考
 
 - [Github Markdown CSS](https://cdn.jsdelivr.net/npm/github-markdown-css@4.0.0/github-markdown.css)
 - [Mermaid API](https://mermaid.js.org/intro/#mermaid-api)
 - [MathJax](https://docs.mathjax.org/en/latest/web/start.html)
```

