# Comparing `tmp/hype-html-1.1.3.tar.gz` & `tmp/hype_html-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hype-html-1.1.3.tar", last modified: Sat Apr 29 16:26:29 2023, max compression
+gzip compressed data, was "hype_html-2.0.0.tar", max compression
```

## Comparing `hype-html-1.1.3.tar` & `hype_html-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,10 @@
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 16:26:29.269300 hype-html-1.1.3/
--rw-r--r--   0 scott     (1000) scott     (1000)     1060 2023-04-29 15:04:42.000000 hype-html-1.1.3/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     3280 2023-04-29 16:26:29.269300 hype-html-1.1.3/PKG-INFO
--rw-r--r--   0 scott     (1000) scott     (1000)     2835 2023-04-29 15:04:42.000000 hype-html-1.1.3/README.md
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 16:26:29.248820 hype-html-1.1.3/hype/
--rw-r--r--   0 scott     (1000) scott     (1000)     3684 2023-04-29 15:35:23.000000 hype-html-1.1.3/hype/__init__.py
--rw-r--r--   0 scott     (1000) scott     (1000)   185067 2023-04-29 15:43:07.000000 hype-html-1.1.3/hype/element.py
--rw-r--r--   0 scott     (1000) scott     (1000)        0 2023-04-29 16:08:45.000000 hype-html-1.1.3/hype/py.typed
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 16:26:29.267292 hype-html-1.1.3/hype_html.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     3280 2023-04-29 16:26:29.000000 hype-html-1.1.3/hype_html.egg-info/PKG-INFO
--rw-r--r--   0 scott     (1000) scott     (1000)      205 2023-04-29 16:26:29.000000 hype-html-1.1.3/hype_html.egg-info/SOURCES.txt
--rw-r--r--   0 scott     (1000) scott     (1000)        1 2023-04-29 16:26:29.000000 hype-html-1.1.3/hype_html.egg-info/dependency_links.txt
--rw-r--r--   0 scott     (1000) scott     (1000)        5 2023-04-29 16:26:29.000000 hype-html-1.1.3/hype_html.egg-info/top_level.txt
--rw-r--r--   0 scott     (1000) scott     (1000)       38 2023-04-29 16:26:29.270295 hype-html-1.1.3/setup.cfg
--rw-r--r--   0 scott     (1000) scott     (1000)      701 2023-04-29 16:26:26.000000 hype-html-1.1.3/setup.py
+-rw-r--r--   0        0        0     1060 2023-04-29 15:04:42.318609 hype_html-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3362 2023-07-21 01:05:21.615529 hype_html-2.0.0/README.md
+-rw-r--r--   0        0        0     1060 2023-04-29 15:04:42.319608 hype_html-2.0.0/hype/LICENSE
+-rw-r--r--   0        0        0     1196 2023-07-21 01:13:05.213072 hype_html-2.0.0/hype/__init__.py
+-rw-r--r--   0        0        0     1426 2023-07-21 01:13:05.254020 hype_html-2.0.0/hype/asyncio/__init__.py
+-rw-r--r--   0        0        0   185117 2023-07-20 00:29:20.745216 hype_html-2.0.0/hype/asyncio/element.py
+-rw-r--r--   0        0        0   185077 2023-07-20 00:09:58.873643 hype_html-2.0.0/hype/element.py
+-rw-r--r--   0        0        0        0 2023-04-29 16:08:45.852021 hype_html-2.0.0/hype/py.typed
+-rw-r--r--   0        0        0      529 2023-07-21 01:30:01.598277 hype_html-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3956 1970-01-01 00:00:00.000000 hype_html-2.0.0/PKG-INFO
```

### Comparing `hype-html-1.1.3/LICENSE` & `hype_html-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hype-html-1.1.3/PKG-INFO` & `hype_html-2.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: hype-html
-Version: 1.1.3
+Version: 2.0.0
 Summary: A minimal python dsl for generating html.
-Home-page: https://github.com/scrussell24/hype-html
+License: MIT
 Author: Scott Russell
 Author-email: me@scottrussell.net
-Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # hype
 
 A minimal python dsl for generating html.
 
 ## Install
 
 Install via pip
 
 ```
 pip install hype-html
 ```
 
-Alteratively, in the spirit of removing dependencies, you could simply copy/paste the hype/element.py file into your project.
+Alternatively, in the spirit of removing dependencies, you could simply copy/paste the hype/element.py file into your project.
 
 ## Usage
 
 Hype exposes classes for each html tag.
 
 ```
 from hype import *
@@ -37,18 +40,18 @@
 
 print(doc)
 
 # <!DOCTYPE html>
 # <div>Hello World!</div>
 ```
 
-Elements can also be rendered by calling.
+Elements can also be rendered by calling their render method.
 
 ```
-doc() == str(doc)
+doc.render() == str(doc)
 ```
 ### Inner HTML
 
 Arguments passed in the element constructor are rendered using the str function and indented (if the element only has one argument it will not be indented.)
 
 ```
 body = Body(
@@ -63,15 +66,15 @@
 # <body>
 #   <h1>Hello World</h1>
 #   <p>This is a paragraph</p>Just a string
 #   <p>Another paragraph</p>
 # </body>
 ```
 
-Append to an elementes list of inner html elements.
+Append to an elements' list of inner html elements.
 
 ```
 body = Body(
     H1('Hello World'),
     P('This is a paragraph'),
     'Just a string'
 )
@@ -170,14 +173,37 @@
 print(div(indent=Indent.FOUR_SPACES))
 
 # <div>
 #    <h1>Header</h1>
 # </div>
 ```
 
+### Async Elements
+
+If your elements content's use coroutines you can use the async elements in hype.asyncio.
+
+The API is nearly identical with two main differences. Of course, the render method is a coroutine. Because of they do not render when calling the str function on them You must explicitly call their render method instead.
+
+```
+import ayncio
+
+from hype.asyncio import *
+
+
+div = Div(H1('Header'))
+
+result = asyncio.run(div.render)
+print(result)
+
+# <div>
+#    <h1>Header</h1>
+# </div>
+
+```
+
 <!-- ## Development
 
 ### Install
 
 ### Pre Processor
 
 ### Tests -->
```

### Comparing `hype-html-1.1.3/README.md` & `hype_html-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Install via pip
 
 ```
 pip install hype-html
 ```
 
-Alteratively, in the spirit of removing dependencies, you could simply copy/paste the hype/element.py file into your project.
+Alternatively, in the spirit of removing dependencies, you could simply copy/paste the hype/element.py file into your project.
 
 ## Usage
 
 Hype exposes classes for each html tag.
 
 ```
 from hype import *
@@ -23,18 +23,18 @@
 
 print(doc)
 
 # <!DOCTYPE html>
 # <div>Hello World!</div>
 ```
 
-Elements can also be rendered by calling.
+Elements can also be rendered by calling their render method.
 
 ```
-doc() == str(doc)
+doc.render() == str(doc)
 ```
 ### Inner HTML
 
 Arguments passed in the element constructor are rendered using the str function and indented (if the element only has one argument it will not be indented.)
 
 ```
 body = Body(
@@ -49,15 +49,15 @@
 # <body>
 #   <h1>Hello World</h1>
 #   <p>This is a paragraph</p>Just a string
 #   <p>Another paragraph</p>
 # </body>
 ```
 
-Append to an elementes list of inner html elements.
+Append to an elements' list of inner html elements.
 
 ```
 body = Body(
     H1('Hello World'),
     P('This is a paragraph'),
     'Just a string'
 )
@@ -156,14 +156,37 @@
 print(div(indent=Indent.FOUR_SPACES))
 
 # <div>
 #    <h1>Header</h1>
 # </div>
 ```
 
+### Async Elements
+
+If your elements content's use coroutines you can use the async elements in hype.asyncio.
+
+The API is nearly identical with two main differences. Of course, the render method is a coroutine. Because of they do not render when calling the str function on them You must explicitly call their render method instead.
+
+```
+import ayncio
+
+from hype.asyncio import *
+
+
+div = Div(H1('Header'))
+
+result = asyncio.run(div.render)
+print(result)
+
+# <div>
+#    <h1>Header</h1>
+# </div>
+
+```
+
 <!-- ## Development
 
 ### Install
 
 ### Pre Processor
 
 ### Tests -->
```

### Comparing `hype-html-1.1.3/hype/element.py` & `hype_html-2.0.0/hype/asyncio/element.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 # Documentation available at https://github.com/scrussell24/hype-html
 
 import enum
-from typing import Any, Tuple, Union, Optional
+from collections.abc import Awaitable
+from typing import Any, Optional, Tuple, Union
 
 
 class Indent(enum.Enum):
     TWO_SPACES = "  "
     FOUR_SPACES = "    "
     TAB = "\t"
 
@@ -66,15 +67,15 @@
         self.inner_elements.append(el)
 
     def attrs(self, **kwargs: str) -> None:
         for k, v in kwargs.items():
             key, val = self._process_attr(k, v)
             self.props[key] = val
 
-    def __call__(
+    async def render(
         self, indent_level: int = 0, indent: Indent = Indent.TWO_SPACES
     ) -> str:
         # props
         props = [
             self._create_attr_string(k, v)
             for k, v in self.props.items()
             if v is not None
@@ -90,28 +91,27 @@
             else ""
         )
 
         # elements
         els = []
         for a in self.inner_elements:
             if isinstance(a, Element):
-                els.append(a(indent_level=indent_level + 1, indent=indent))
+                els.append(await a.render(indent_level=indent_level + 1, indent=indent))
+            elif isinstance(a, Awaitable):
+                els.append(str(await a))
             else:
                 els.append(str(a))
 
         if self.self_closing:
             return f'{indent_chars}<{self.tag}{prop_space}{" ".join([p for p in props if p])}/>'
         return (
             f'{indent_chars}<{self.tag}{prop_space}{" ".join([p for p in props if p])}'
             f'>{"".join(els)}{end_tag_indent}</{self.tag}>'
         )
 
-    def __str__(self) -> str:
-        return self()
-
 
 class SelfClosingElement(Element):
     self_closing = True
 
     def __init__(self, **kwargs: Optional[str]):
         super().__init__(**kwargs)
 
@@ -119,26 +119,23 @@
 class Doc:
     def __init__(
         self, *args: Union[str, "Element"], indent: Indent = Indent.TWO_SPACES
     ):
         self.indent = indent
         self.elements = args
 
-    def __call__(self) -> str:
+    async def render(self) -> str:
         doc = "<!DOCTYPE html>"
         for el in self.elements:
             if isinstance(el, Element):
-                doc += el(indent=self.indent)
+                doc += await el.render(indent=self.indent)
             else:
                 doc += str(el)
         return doc
 
-    def __str__(self) -> str:
-        return self()
-
 
 # Below code is autogenerated by rendering the tmplt.element.py.j2 file
 
 
 class A(Element):
     tag = "a"
```

