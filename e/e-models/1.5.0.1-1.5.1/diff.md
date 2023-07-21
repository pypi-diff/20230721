# Comparing `tmp/e-models-1.5.0.1.tar.gz` & `tmp/e-models-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.5.0.1.tar", last modified: Wed Jul  5 14:19:23 2023, max compression
+gzip compressed data, was "e-models-1.5.1.tar", last modified: Fri Jul 21 18:31:03 2023, max compression
```

## Comparing `e-models-1.5.0.1.tar` & `e-models-1.5.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-05 14:19:23.073566 e-models-1.5.0.1/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.5.0.1/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3470 2023-07-05 14:19:23.073566 e-models-1.5.0.1/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2928 2023-06-01 14:06:43.000000 e-models-1.5.0.1/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-05 14:19:23.065566 e-models-1.5.0.1/e_models.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3470 2023-07-05 14:19:22.000000 e-models-1.5.0.1/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      655 2023-07-05 14:19:23.000000 e-models-1.5.0.1/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-07-05 14:19:22.000000 e-models-1.5.0.1/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        7 2023-07-05 14:19:22.000000 e-models-1.5.0.1/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-07-05 14:19:22.000000 e-models-1.5.0.1/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-05 14:19:23.069566 e-models-1.5.0.1/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       24 2023-07-05 14:17:51.000000 e-models-1.5.0.1/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-05-04 18:51:26.000000 e-models-1.5.0.1/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-05 14:19:23.069566 e-models-1.5.0.1/emodels/datasets/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.5.0.1/emodels/datasets/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12161 2023-07-05 14:16:27.000000 e-models-1.5.0.1/emodels/datasets/models.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1929 2023-07-05 14:16:56.000000 e-models-1.5.0.1/emodels/datasets/tokenizers.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4716 2023-06-23 22:38:40.000000 e-models-1.5.0.1/emodels/datasets/utils.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-05 14:19:23.069566 e-models-1.5.0.1/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35296 2023-06-08 13:46:29.000000 e-models-1.5.0.1/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.5.0.1/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.5.0.1/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.5.0.1/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.5.0.1/emodels/html2text/utils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.5.0.1/emodels/py.typed
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-05 14:19:23.073566 e-models-1.5.0.1/emodels/scrapyutils/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      137 2023-06-23 22:04:28.000000 e-models-1.5.0.1/emodels/scrapyutils/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2544 2023-06-23 22:05:11.000000 e-models-1.5.0.1/emodels/scrapyutils/loader.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4351 2023-06-23 21:34:47.000000 e-models-1.5.0.1/emodels/scrapyutils/response.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.5.0.1/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-07-05 14:19:23.073566 e-models-1.5.0.1/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      909 2023-07-05 14:17:41.000000 e-models-1.5.0.1/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-05 14:19:23.073566 e-models-1.5.0.1/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4951 2023-07-03 15:13:25.000000 e-models-1.5.0.1/tests/test_html2text.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7475 2023-06-23 23:01:17.000000 e-models-1.5.0.1/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-21 18:31:03.335693 e-models-1.5.1/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.5.1/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3468 2023-07-21 18:31:03.335693 e-models-1.5.1/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2928 2023-06-01 14:06:43.000000 e-models-1.5.1/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-21 18:31:03.331693 e-models-1.5.1/e_models.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3468 2023-07-21 18:31:03.000000 e-models-1.5.1/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      655 2023-07-21 18:31:03.000000 e-models-1.5.1/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-07-21 18:31:03.000000 e-models-1.5.1/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        7 2023-07-21 18:31:03.000000 e-models-1.5.1/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-07-21 18:31:03.000000 e-models-1.5.1/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-21 18:31:03.331693 e-models-1.5.1/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       22 2023-07-21 18:28:43.000000 e-models-1.5.1/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-05-04 18:51:26.000000 e-models-1.5.1/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-21 18:31:03.331693 e-models-1.5.1/emodels/datasets/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.5.1/emodels/datasets/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12161 2023-07-05 14:16:27.000000 e-models-1.5.1/emodels/datasets/models.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1929 2023-07-05 14:16:56.000000 e-models-1.5.1/emodels/datasets/tokenizers.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4716 2023-06-23 22:38:40.000000 e-models-1.5.1/emodels/datasets/utils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-21 18:31:03.331693 e-models-1.5.1/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35479 2023-07-21 16:26:32.000000 e-models-1.5.1/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.5.1/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.5.1/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.5.1/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.5.1/emodels/html2text/utils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.5.1/emodels/py.typed
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-21 18:31:03.331693 e-models-1.5.1/emodels/scrapyutils/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      137 2023-06-23 22:04:28.000000 e-models-1.5.1/emodels/scrapyutils/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2575 2023-07-21 17:45:38.000000 e-models-1.5.1/emodels/scrapyutils/loader.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6000 2023-07-21 18:26:42.000000 e-models-1.5.1/emodels/scrapyutils/response.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.5.1/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-07-21 18:31:03.335693 e-models-1.5.1/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      907 2023-07-21 18:28:27.000000 e-models-1.5.1/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-21 18:31:03.335693 e-models-1.5.1/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6346 2023-07-21 17:31:24.000000 e-models-1.5.1/tests/test_html2text.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8260 2023-07-21 18:10:59.000000 e-models-1.5.1/tests/test_scrapyutils.py
```

### Comparing `e-models-1.5.0.1/LICENSE` & `e-models-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.5.0.1/PKG-INFO` & `e-models-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.5.0.1
+Version: 1.5.1
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.5.0.1/README.md` & `e-models-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `e-models-1.5.0.1/e_models.egg-info/PKG-INFO` & `e-models-1.5.1/e_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.5.0.1
+Version: 1.5.1
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.5.0.1/e_models.egg-info/SOURCES.txt` & `e-models-1.5.1/e_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e-models-1.5.0.1/emodels/datasets/models.py` & `e-models-1.5.1/emodels/datasets/models.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.0.1/emodels/datasets/tokenizers.py` & `e-models-1.5.1/emodels/datasets/tokenizers.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.0.1/emodels/datasets/utils.py` & `e-models-1.5.1/emodels/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.0.1/emodels/html2text/__init__.py` & `e-models-1.5.1/emodels/html2text/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     def __init__(
         self,
         out: Optional[OutCallback] = None,
         baseurl: str = "",
         bodywidth: int = config.BODY_WIDTH,
         ids: bool = False,
         classes: bool = False,
+        extra_ids: Optional[List[str]] = None,
+        extra_classes: Optional[List[str]] = None
     ) -> None:
         """
         Input parameters:
             out: possible custom replacement for self.outtextf (which
                  appends lines of text).
             baseurl: base URL of the document we process
         """
@@ -135,14 +137,17 @@
         self.current_tag = ""
         self.ids = ids
         self.current_id: List[Tuple[str, bool | None]] = []
         self.classes = classes
         self.current_class: List[Tuple[str, bool | None]] = []
         self.within_table_row = 0
 
+        self.extra_ids: List[str] = extra_ids.copy() if extra_ids is not None else []
+        self.extra_classes: List[str] = extra_classes.copy() if extra_classes is not None else []
+
         config.UNIFIABLE["nbsp"] = "&nbsp_place_holder;"
 
     def feed(self, data: str) -> None:
         data = data.replace("</' + 'script>", "</ignore>")
         super().feed(data)
 
     def handle(self, data: str) -> str:
@@ -829,34 +834,33 @@
         self.o(data, puredata=True)
 
         if self.ids and self.current_id and not self.cdata_elem:
             attrid, delayed_attrid = self.current_id[-1]
             if rawdata:
                 if attrid:
                     self.out(f" <!--#{attrid}-->")
-                elif len(self.current_id) > 1:
-                    a, d = self.current_id[-2]
-                    if d:
-                        self.out(f" <!--#{a}-->")
-                        self.current_id = self.current_id[:-2] + [(a, False), self.current_id[-1]]
+                else:
+                    for a, d in self.current_id[:-1][::-1]:
+                        if d and a in self.extra_ids:
+                            self.out(f" <!--#{a}-->")
+                            break
             elif attrid and delayed_attrid is None:
-
                 self.current_id.pop()
                 self.current_id.append((attrid, True))
 
         if self.classes and self.current_class and not self.cdata_elem:
             attrclass, delayed_attrclass = self.current_class[-1]
             if rawdata:
                 if attrclass:
                     self.out(f" <!--.{attrclass}-->")
-                elif len(self.current_class) > 1:
-                    a, d = self.current_class[-2]
-                    if d:
-                        self.out(f" <!--.{a}-->")
-                        self.current_class = self.current_class[:-2] + [(a, False), self.current_class[-1]]
+                else:
+                    for a, d in self.current_class[:-1][::-1]:
+                        if d and a in self.extra_classes:
+                            self.out(f" <!--.{a}-->")
+                            break
             elif attrclass and delayed_attrclass is None:
                 self.current_class.pop()
                 self.current_class.append((attrclass, True))
 
     def charref(self, name: str) -> str:
         if name[0] in ["x", "X"]:
             c = int(name[1:], 16)
```

### Comparing `e-models-1.5.0.1/emodels/html2text/config.py` & `e-models-1.5.1/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.0.1/emodels/html2text/utils.py` & `e-models-1.5.1/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.0.1/emodels/scrapyutils/loader.py` & `e-models-1.5.1/emodels/scrapyutils/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,21 +41,22 @@
         self,
         attr: str,
         reg: str = "(.+?)",
         tid: Optional[str] = None,
         flags: int = 0,
         skip_prefix: str = DEFAULT_SKIP_PREFIX,
         strict_tid: bool = False,
+        idx: int = 0,
         *processors,
         **kw,
     ):
         if not self._check_valid_response():
             raise ValueError("context response type is not a valid TextResponse.")
         extracted = self.context["response"].text_re(
-            reg=reg, tid=tid, flags=flags, skip_prefix=skip_prefix, strict_tid=strict_tid, optimize=True
+            reg=reg, tid=tid, flags=flags, skip_prefix=skip_prefix, strict_tid=strict_tid, idx=idx, optimize=True
         )
         if extracted:
             t, s, e = extracted[0]
             if attr not in self.extract_indexes:
                 self.extract_indexes[attr] = (s, e)
                 self.add_value(attr, t, *processors, **kw)
```

### Comparing `e-models-1.5.0.1/setup.py` & `e-models-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.5.0.1',
+    version      = '1.5.1',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
```

### Comparing `e-models-1.5.0.1/tests/test_html2text.py` & `e-models-1.5.1/tests/test_html2text.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,26 +9,30 @@
         html = b"""
 <div id="did">
 <p>first line</p>
 <p class="pc0">this is a line</p>
 <p id="pid1">this is a line with id</p>
 <p id="pid2">this is another line with id</p>
 </div>
+<p>A final line<p>
         """
         response = ExtractTextResponse(url="http://example.com/example1.html", status=200, body=html)
+        response._add_extra_ids(["did"])
         expected = """first line <!--#did-->
 
-this is a line
+this is a line <!--#did-->
 
 this is a line with id <!--#pid1-->
 
 this is another line with id <!--#pid2-->
+
+A final line
 """
 
-        self.assertEqual(response.markdown_ids, expected)
+        self.assertEqual(expected, response.markdown_ids)
 
     def test_ids_ii(self):
         html = b"""
 <div class="did">
 <p>first line</p>
 <p class="pc0">this is a line</p>
 <p id="pid1">this is a line with id</p>
@@ -41,33 +45,37 @@
 this is a line
 
 this is a line with id <!--#pid1-->
 
 this is another line with id <!--#pid2-->
 """
 
-        self.assertEqual(response.markdown_ids, expected)
+        self.assertEqual(expected, response.markdown_ids)
 
     def test_classes(self):
         html = b"""
 <div class="did">
 <p>this is a line</p>
 <p class="pc1">this is a line with class</p>
 <p id="pid2">this is a line with id</p>
 </div>
+<p>A final line<p>
         """
         response = ExtractTextResponse(url="http://example.com/example2.html", status=200, body=html)
+        response._add_extra_classes(["did"])
         expected = """this is a line <!--.did-->
 
 this is a line with class <!--.pc1-->
 
-this is a line with id
+this is a line with id <!--.did-->
+
+A final line
 """
 
-        self.assertEqual(response.markdown_classes, expected)
+        self.assertEqual(expected, response.markdown_classes)
 
     def test_classes_ii(self):
         html = b"""
 <div id="did">
 <p>this is a line</p>
 <p class="pc1">this is a line with class</p>
 <p id="pid2">this is a line with id</p>
@@ -77,30 +85,30 @@
         expected = """this is a line
 
 this is a line with class <!--.pc1-->
 
 this is a line with id
 """
 
-        self.assertEqual(response.markdown_classes, expected)
+        self.assertEqual(expected, response.markdown_classes)
 
     def test_tables_plain(self):
         html = b"""
 <table><tr><td>Data 1</td><td>Data 2</td></tr>
 <tr><td>Data 3</td><td>Data 4</td></tr>
 <tr><td>Data 5</td><td>Data 6</td></tr>
 </table>
 """
 
         response = ExtractTextResponse(url="http://example.com/example2.html", status=200, body=html)
         expected = """| Data 1| Data 2|
 | Data 3| Data 4|
 | Data 5| Data 6|
 """
-        self.assertEqual(response.markdown, expected)
+        self.assertEqual(expected, response.markdown)
 
     def test_tables_with_header(self):
         html = b"""
 <table><tr><th>Head 1</th><th>Head 2</th></tr>
 <tr><td>Data 1</td><td>Data 2</td></tr>
 <tr><td>Data 3</td><td>Data 4</td></tr>
 </table>
@@ -109,15 +117,15 @@
 
         response = ExtractTextResponse(url="http://example.com/example2.html", status=200, body=html)
         expected = """| Head 1| Head 2|
 | ---|---|
 | Data 1| Data 2|
 | Data 3| Data 4|
 """
-        self.assertEqual(response.markdown, expected)
+        self.assertEqual(expected, response.markdown)
 
     def test_tables_with_br_line_breaks(self):
         html = b"""
 <table><tr><td>Data 1</td><td>Data 2</td></tr>
 <tr><td>Data 3</td><td>Data 4</td></tr>
 <tr><td>Data 5</td><td><p>Data 6</p></td></tr>
 <tr><td>Data 7</td><td>Data 8</td></tr>
@@ -127,15 +135,15 @@
         html2text.config.LINE_BREAK_WITHIN_TABLE = "<br>"
         response = ExtractTextResponse(url="http://example.com/example2.html", status=200, body=html)
         expected = """| Data 1| Data 2|
 | Data 3| Data 4|
 | Data 5| <br><br>Data 6<br><br>|
 | Data 7| Data 8|
 """
-        self.assertEqual(response.markdown, expected)
+        self.assertEqual(expected, response.markdown)
         html2text.config.LINE_BREAK_WITHIN_TABLE = saved
 
     def test_tables_with_line_breaks_default(self):
         html = b"""
 <table><tr><td>Data 1</td><td>Data 2</td></tr>
 <tr><td>Data 3</td><td>Data 4</td></tr>
 <tr><td>Data 5</td><td><p>Data 6</p></td></tr>
@@ -146,21 +154,72 @@
         expected = """| Data 1| Data 2|
 | Data 3| Data 4|
 | Data 5| \n\nData 6
 
 |
 | Data 7| Data 8|
 """
-        self.assertEqual(response.markdown, expected)
+        self.assertEqual(expected, response.markdown)
 
     def test_entities(self):
         html = b"""<div>There&nbsp;are&nbsp;spaces</div>"""
         response = ExtractTextResponse(url="http://example.com/example2.html", status=200, body=html)
         self.assertEqual(response.markdown, "There are spaces\n")
 
         html = b"""<div>There&amp;nbsp;are&amp;nbsp;spaces</div>"""
         response = ExtractTextResponse(url="http://example.com/example2.html", status=200, body=html)
         self.assertEqual(response.markdown, "There&nbsp;are&nbsp;spaces\n")
 
         html = b"""<div>There&nbspare&nbspspaces</div>"""
         response = ExtractTextResponse(url="http://example.com/example2.html", status=200, body=html)
-        self.assertEqual(response.markdown, "There are spaces\n")
+        self.assertEqual("There are spaces\n", response.markdown)
+
+    def test_ids_delayed(self):
+        html = b"""
+<div id="did">
+<span>
+<p>first line</p>
+<p class="pc0">this is a line</p>
+<p id="pid1">this is a line with id</p>
+<p id="pid2">this is another line with id</p>
+</span>
+</div>
+<p>A final line<p>
+        """
+        response = ExtractTextResponse(url="http://example.com/example1.html", status=200, body=html)
+        response._add_extra_ids(["did"])
+        expected = """first line <!--#did-->
+
+this is a line <!--#did-->
+
+this is a line with id <!--#pid1-->
+
+this is another line with id <!--#pid2-->
+
+A final line
+"""
+
+        self.assertEqual(expected, response.markdown_ids)
+
+    def test_classes_delayed(self):
+        html = b"""
+<div class="did">
+<span>
+<p>this is a line</p>
+<p class="pc1">this is a line with class</p>
+<p id="pid2">this is a line with id</p>
+</span>
+</div>
+<p>A final line<p>
+        """
+        response = ExtractTextResponse(url="http://example.com/example2.html", status=200, body=html)
+        response._add_extra_classes(["did"])
+        expected = """this is a line <!--.did-->
+
+this is a line with class <!--.pc1-->
+
+this is a line with id <!--.did-->
+
+A final line
+"""
+
+        self.assertEqual(expected, response.markdown_classes)
```

### Comparing `e-models-1.5.0.1/tests/test_scrapyutils.py` & `e-models-1.5.1/tests/test_scrapyutils.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     closing_date = Field()
     sublocation = Field()
     postal_code = Field()
     city = Field()
     state = Field()
     country = Field()
     response = Field()
+    locality = Field()
 
 
 class JobItemLoader(ExtractItemLoader):
     default_item_class = JobItem
     default_output_processor = TakeFirst()
 
 
@@ -70,15 +71,15 @@
     def tearDown(self):
         for col in "jobs", "business":
             fname = getattr(self, f"{col}_result_file")
             dname = os.path.dirname(fname)
             for f in os.listdir(dname):
                 os.remove(os.path.join(dname, f))
 
-    def test_example_one(self):
+    def test_case_one(self):
         tresponse = self.samples["https://careers.und.edu/jobs/job21.html"]
         loader = JobItemLoader(response=tresponse)
         loader.add_text_re("job_title", tid="#job_title_2_2")
         loader.add_text_re("employment_type", tid="#employment_type_2_2_0_0")
         loader.add_text_re("job_id", tid="#requisition_identifier_2_2_0")
         loader.add_text_re("description", r"(###\s+.+?)\*\*apply now\*\*", flags=re.S | re.I)
 
@@ -115,15 +116,15 @@
         self.assertEqual(data["markdown"][slice(*data["indexes"]["job_id"])], "492556")
         self.assertEqual(data["markdown"][slice(*data["indexes"]["employment_type"])], "Full-time Staff")
 
         self.assertEqual(data["markdown"][slice(*data["indexes"]["description"])], item["description"])
 
         self.assertTrue(response.text_re(tid=".job-field job-title"))
 
-    def test_example_two(self):
+    def test_case_two(self):
         response = self.samples["https://yell.com/result.html"].replace(cls=ExtractTextResponse)
 
         for r in response.css_split(".businessCapsule--mainRow"):
             loader = BusinessSearchItemLoader(response=r)
             loader.add_text_re("name", r"##(.+)")
             loader.add_text_re("phone", r"Tel([\s\d]+)", tid="#telephone")
             loader.add_text_re("website", r"Website\]\((.+?)\)")
@@ -166,7 +167,24 @@
         self.assertEqual(extracted[4]["address_alt"], "3 Ardconnel Terrace,  Inverness")
         self.assertEqual(
             extracted[5]["profile_url"], "https://yell.com/biz/jack-gowans-and-marc-dickson-inverness-901395225/"
         )
         self.assertEqual(extracted[6]["locality"], "Inverness")
         self.assertEqual(extracted[7]["street"], "York House, 20, Church St")
         self.assertEqual(extracted[8]["postal_code"], "IV1 1DF")
+
+    def test_case_three(self):
+        response = self.samples["https://npc.isolvedhire.com/jobs/857557.html"].replace(cls=ExtractTextResponse)
+        self.assertEqual(
+            response.text_re(tid=".job-items"),
+            [("Holbrook, AZ, USA", 461, 478), ("13.85", 487, 492), ("Hourly", 501, 507), ("Part Time", 516, 525)],
+        )
+
+        tresponse = self.samples["https://npc.isolvedhire.com/jobs/857557.html"]
+        loader = JobItemLoader(response=tresponse)
+
+        loader.add_text_re("locality", tid=".job-items")
+        loader.add_text_re("employment_type", tid=".job-items", idx=3)
+
+        item = loader.load_item()
+        self.assertEqual(item["locality"], "Holbrook, AZ, USA")
+        self.assertEqual(item["employment_type"], "Part Time")
```

