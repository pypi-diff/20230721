# Comparing `tmp/hype_html-2.0.0.tar.gz` & `tmp/hype_html-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hype_html-2.0.0.tar", max compression
+gzip compressed data, was "hype_html-2.0.1.tar", max compression
```

## Comparing `hype_html-2.0.0.tar` & `hype_html-2.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1060 2023-04-29 15:04:42.318609 hype_html-2.0.0/LICENSE
--rw-r--r--   0        0        0     3362 2023-07-21 01:05:21.615529 hype_html-2.0.0/README.md
--rw-r--r--   0        0        0     1060 2023-04-29 15:04:42.319608 hype_html-2.0.0/hype/LICENSE
--rw-r--r--   0        0        0     1196 2023-07-21 01:13:05.213072 hype_html-2.0.0/hype/__init__.py
--rw-r--r--   0        0        0     1426 2023-07-21 01:13:05.254020 hype_html-2.0.0/hype/asyncio/__init__.py
--rw-r--r--   0        0        0   185117 2023-07-20 00:29:20.745216 hype_html-2.0.0/hype/asyncio/element.py
--rw-r--r--   0        0        0   185077 2023-07-20 00:09:58.873643 hype_html-2.0.0/hype/element.py
--rw-r--r--   0        0        0        0 2023-04-29 16:08:45.852021 hype_html-2.0.0/hype/py.typed
--rw-r--r--   0        0        0      529 2023-07-21 01:30:01.598277 hype_html-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3956 1970-01-01 00:00:00.000000 hype_html-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-29 15:04:42.318609 hype_html-2.0.1/LICENSE
+-rw-r--r--   0        0        0     3362 2023-07-21 01:05:21.615529 hype_html-2.0.1/README.md
+-rw-r--r--   0        0        0     1060 2023-04-29 15:04:42.319608 hype_html-2.0.1/hype/LICENSE
+-rw-r--r--   0        0        0     1196 2023-07-21 03:40:06.266196 hype_html-2.0.1/hype/__init__.py
+-rw-r--r--   0        0        0     1426 2023-07-21 03:40:06.306296 hype_html-2.0.1/hype/asyncio/__init__.py
+-rw-r--r--   0        0        0   185102 2023-07-21 03:36:07.261516 hype_html-2.0.1/hype/asyncio/element.py
+-rw-r--r--   0        0        0   185077 2023-07-21 03:22:33.145794 hype_html-2.0.1/hype/element.py
+-rw-r--r--   0        0        0        0 2023-04-29 16:08:45.852021 hype_html-2.0.1/hype/py.typed
+-rw-r--r--   0        0        0      529 2023-07-21 03:40:19.296414 hype_html-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3956 1970-01-01 00:00:00.000000 hype_html-2.0.1/PKG-INFO
```

### Comparing `hype_html-2.0.0/LICENSE` & `hype_html-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hype_html-2.0.0/README.md` & `hype_html-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hype_html-2.0.0/hype/LICENSE` & `hype_html-2.0.1/hype/LICENSE`

 * *Files identical despite different names*

### Comparing `hype_html-2.0.0/hype/__init__.py` & `hype_html-2.0.1/hype/__init__.py`

 * *Files identical despite different names*

### Comparing `hype_html-2.0.0/hype/asyncio/__init__.py` & `hype_html-2.0.1/hype/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `hype_html-2.0.0/hype/asyncio/element.py` & `hype_html-2.0.1/hype/asyncio/element.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 # Documentation available at https://github.com/scrussell24/hype-html
 
 import enum
-from collections.abc import Awaitable
+import inspect
 from typing import Any, Optional, Tuple, Union
 
 
 class Indent(enum.Enum):
     TWO_SPACES = "  "
     FOUR_SPACES = "    "
     TAB = "\t"
@@ -80,28 +80,28 @@
             for k, v in self.props.items()
             if v is not None
         ]
         props = [p for p in props if p]
         prop_space = " " if len(props) else ""
 
         # indent
-        indent_chars = "\n" + "".join([indent.value for n in range(indent_level)])
+        indent_chars = "\n" + "".join([indent.value for _ in range(indent_level)])
         end_tag_indent = (
             indent_chars
             if any([True for el in self.inner_elements if isinstance(el, Element)])
             else ""
         )
 
         # elements
         els = []
         for a in self.inner_elements:
             if isinstance(a, Element):
                 els.append(await a.render(indent_level=indent_level + 1, indent=indent))
-            elif isinstance(a, Awaitable):
-                els.append(str(await a))
+            elif inspect.iscoroutinefunction(a):
+                els.append(str(await a()))
             else:
                 els.append(str(a))
 
         if self.self_closing:
             return f'{indent_chars}<{self.tag}{prop_space}{" ".join([p for p in props if p])}/>'
         return (
             f'{indent_chars}<{self.tag}{prop_space}{" ".join([p for p in props if p])}'
```

### Comparing `hype_html-2.0.0/hype/element.py` & `hype_html-2.0.1/hype/element.py`

 * *Files identical despite different names*

### Comparing `hype_html-2.0.0/pyproject.toml` & `hype_html-2.0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hype-html"
-version = "2.0.0"
+version = "2.0.1"
 description = "A minimal python dsl for generating html."
 authors = ["Scott Russell <me@scottrussell.net>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "hype"}]
 
 [tool.poetry.dependencies]
```

### Comparing `hype_html-2.0.0/PKG-INFO` & `hype_html-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hype-html
-Version: 2.0.0
+Version: 2.0.1
 Summary: A minimal python dsl for generating html.
 License: MIT
 Author: Scott Russell
 Author-email: me@scottrussell.net
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

