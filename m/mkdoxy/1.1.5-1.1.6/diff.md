# Comparing `tmp/mkdoxy-1.1.5.tar.gz` & `tmp/mkdoxy-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdoxy-1.1.5.tar", last modified: Wed Jul 19 14:36:02 2023, max compression
+gzip compressed data, was "mkdoxy-1.1.6.tar", last modified: Fri Jul 21 14:25:28 2023, max compression
```

## Comparing `mkdoxy-1.1.5.tar` & `mkdoxy-1.1.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-19 14:36:02.495192 mkdoxy-1.1.5/
--rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-01-24 19:48:21.000000 mkdoxy-1.1.5/LICENSE
--rw-r--r--   0 kuba       (501) staff       (20)     5587 2023-07-19 14:36:02.495052 mkdoxy-1.1.5/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     4585 2023-07-13 14:42:53.000000 mkdoxy-1.1.5/README.md
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-19 14:36:02.490581 mkdoxy-1.1.5/mkdoxy/
--rw-r--r--   0 kuba       (501) staff       (20)     2628 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/DoxyTagParser.py
--rw-r--r--   0 kuba       (501) staff       (20)        0 2023-01-24 19:46:54.000000 mkdoxy-1.1.5/mkdoxy/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)      252 2023-01-25 07:25:08.000000 mkdoxy-1.1.5/mkdoxy/cache.py
--rw-r--r--   0 kuba       (501) staff       (20)     2947 2023-07-13 13:55:16.000000 mkdoxy-1.1.5/mkdoxy/constants.py
--rw-r--r--   0 kuba       (501) staff       (20)     4393 2023-07-17 11:27:23.000000 mkdoxy-1.1.5/mkdoxy/doxygen.py
--rw-r--r--   0 kuba       (501) staff       (20)     4443 2023-07-17 11:24:21.000000 mkdoxy-1.1.5/mkdoxy/doxyrun.py
--rw-r--r--   0 kuba       (501) staff       (20)     1980 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/finder.py
--rw-r--r--   0 kuba       (501) staff       (20)    11316 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/generatorAuto.py
--rw-r--r--   0 kuba       (501) staff       (20)    16236 2023-07-17 11:27:25.000000 mkdoxy-1.1.5/mkdoxy/generatorBase.py
--rw-r--r--   0 kuba       (501) staff       (20)    12051 2023-07-13 14:03:02.000000 mkdoxy-1.1.5/mkdoxy/generatorSnippets.py
--rw-r--r--   0 kuba       (501) staff       (20)     4471 2023-01-25 07:25:08.000000 mkdoxy-1.1.5/mkdoxy/markdown.py
--rw-r--r--   0 kuba       (501) staff       (20)    21472 2023-07-17 11:27:29.000000 mkdoxy-1.1.5/mkdoxy/node.py
--rw-r--r--   0 kuba       (501) staff       (20)     7770 2023-07-17 11:24:21.000000 mkdoxy-1.1.5/mkdoxy/plugin.py
--rw-r--r--   0 kuba       (501) staff       (20)     9288 2023-07-17 11:27:30.000000 mkdoxy-1.1.5/mkdoxy/property.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-19 14:36:02.494821 mkdoxy-1.1.5/mkdoxy/templates/
--rw-r--r--   0 kuba       (501) staff       (20)      517 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/annotated.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      380 2023-07-13 13:55:29.000000 mkdoxy-1.1.5/mkdoxy/templates/classes.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      544 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/code.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      613 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/error.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      164 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/example.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      581 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/examples.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      407 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/files.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      498 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/hierarchy.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      437 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/index.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      741 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/memDef.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     1698 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/memTab.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     4632 2023-07-17 11:23:05.000000 mkdoxy-1.1.5/mkdoxy/templates/member.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      426 2023-07-13 13:55:51.000000 mkdoxy-1.1.5/mkdoxy/templates/modules.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      413 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/namespaces.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/page.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      456 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/programlisting.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/relatedPages.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     3184 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/utils.py
--rw-r--r--   0 kuba       (501) staff       (20)     7390 2023-07-17 11:27:32.000000 mkdoxy-1.1.5/mkdoxy/xml_parser.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-19 14:36:02.491569 mkdoxy-1.1.5/mkdoxy.egg-info/
--rwxr-xr-x   0 kuba       (501) staff       (20)     5587 2023-07-19 14:36:02.000000 mkdoxy-1.1.5/mkdoxy.egg-info/PKG-INFO
--rwxr-xr-x   0 kuba       (501) staff       (20)     1072 2023-07-19 14:36:02.000000 mkdoxy-1.1.5/mkdoxy.egg-info/SOURCES.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        1 2023-07-19 14:36:02.000000 mkdoxy-1.1.5/mkdoxy.egg-info/dependency_links.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)       47 2023-07-19 14:36:02.000000 mkdoxy-1.1.5/mkdoxy.egg-info/entry_points.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)      143 2023-07-19 14:36:02.000000 mkdoxy-1.1.5/mkdoxy.egg-info/requires.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        7 2023-07-19 14:36:02.000000 mkdoxy-1.1.5/mkdoxy.egg-info/top_level.txt
--rw-r--r--   0 kuba       (501) staff       (20)       38 2023-07-19 14:36:02.495227 mkdoxy-1.1.5/setup.cfg
--rwxr-xr-x   0 kuba       (501) staff       (20)     1853 2023-07-19 14:34:47.000000 mkdoxy-1.1.5/setup.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-21 14:25:28.817957 mkdoxy-1.1.6/
+-rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-01-24 19:48:21.000000 mkdoxy-1.1.6/LICENSE
+-rw-r--r--   0 kuba       (501) staff       (20)     5587 2023-07-21 14:25:28.817730 mkdoxy-1.1.6/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     4585 2023-07-13 14:42:53.000000 mkdoxy-1.1.6/README.md
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-21 14:25:28.812502 mkdoxy-1.1.6/mkdoxy/
+-rw-r--r--   0 kuba       (501) staff       (20)     2629 2023-07-21 13:48:39.000000 mkdoxy-1.1.6/mkdoxy/DoxyTagParser.py
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2023-01-24 19:46:54.000000 mkdoxy-1.1.6/mkdoxy/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)      252 2023-01-25 07:25:08.000000 mkdoxy-1.1.6/mkdoxy/cache.py
+-rw-r--r--   0 kuba       (501) staff       (20)     2947 2023-07-13 13:55:16.000000 mkdoxy-1.1.6/mkdoxy/constants.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4393 2023-07-17 11:27:23.000000 mkdoxy-1.1.6/mkdoxy/doxygen.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4428 2023-07-21 13:48:39.000000 mkdoxy-1.1.6/mkdoxy/doxyrun.py
+-rw-r--r--   0 kuba       (501) staff       (20)     1982 2023-07-21 13:48:39.000000 mkdoxy-1.1.6/mkdoxy/finder.py
+-rw-r--r--   0 kuba       (501) staff       (20)    11316 2023-06-30 11:43:03.000000 mkdoxy-1.1.6/mkdoxy/generatorAuto.py
+-rw-r--r--   0 kuba       (501) staff       (20)    16212 2023-07-21 13:48:39.000000 mkdoxy-1.1.6/mkdoxy/generatorBase.py
+-rw-r--r--   0 kuba       (501) staff       (20)    11947 2023-07-21 13:48:39.000000 mkdoxy-1.1.6/mkdoxy/generatorSnippets.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4472 2023-07-21 13:48:39.000000 mkdoxy-1.1.6/mkdoxy/markdown.py
+-rw-r--r--   0 kuba       (501) staff       (20)    21472 2023-07-21 13:48:39.000000 mkdoxy-1.1.6/mkdoxy/node.py
+-rw-r--r--   0 kuba       (501) staff       (20)     7711 2023-07-21 13:48:39.000000 mkdoxy-1.1.6/mkdoxy/plugin.py
+-rw-r--r--   0 kuba       (501) staff       (20)     9288 2023-07-17 11:27:30.000000 mkdoxy-1.1.6/mkdoxy/property.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-21 14:25:28.817227 mkdoxy-1.1.6/mkdoxy/templates/
+-rw-r--r--   0 kuba       (501) staff       (20)      517 2023-06-30 11:43:03.000000 mkdoxy-1.1.6/mkdoxy/templates/annotated.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      380 2023-07-13 13:55:29.000000 mkdoxy-1.1.6/mkdoxy/templates/classes.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      544 2023-06-30 11:43:03.000000 mkdoxy-1.1.6/mkdoxy/templates/code.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      613 2023-06-30 11:43:03.000000 mkdoxy-1.1.6/mkdoxy/templates/error.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      164 2023-06-30 11:43:03.000000 mkdoxy-1.1.6/mkdoxy/templates/example.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      581 2023-06-30 11:43:03.000000 mkdoxy-1.1.6/mkdoxy/templates/examples.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      407 2023-06-30 11:43:03.000000 mkdoxy-1.1.6/mkdoxy/templates/files.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      498 2023-06-30 11:43:03.000000 mkdoxy-1.1.6/mkdoxy/templates/hierarchy.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      437 2023-06-30 11:43:03.000000 mkdoxy-1.1.6/mkdoxy/templates/index.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      741 2023-06-30 11:43:03.000000 mkdoxy-1.1.6/mkdoxy/templates/memDef.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     1698 2023-06-30 11:43:03.000000 mkdoxy-1.1.6/mkdoxy/templates/memTab.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     4632 2023-07-17 11:23:05.000000 mkdoxy-1.1.6/mkdoxy/templates/member.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      426 2023-07-13 13:55:51.000000 mkdoxy-1.1.6/mkdoxy/templates/modules.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      413 2023-06-30 11:43:03.000000 mkdoxy-1.1.6/mkdoxy/templates/namespaces.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.6/mkdoxy/templates/page.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      456 2023-06-30 11:43:03.000000 mkdoxy-1.1.6/mkdoxy/templates/programlisting.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.6/mkdoxy/templates/relatedPages.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     3110 2023-07-21 13:48:39.000000 mkdoxy-1.1.6/mkdoxy/utils.py
+-rw-r--r--   0 kuba       (501) staff       (20)     7457 2023-07-21 13:48:39.000000 mkdoxy-1.1.6/mkdoxy/xml_parser.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-21 14:25:28.813355 mkdoxy-1.1.6/mkdoxy.egg-info/
+-rwxr-xr-x   0 kuba       (501) staff       (20)     5587 2023-07-21 14:25:28.000000 mkdoxy-1.1.6/mkdoxy.egg-info/PKG-INFO
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1072 2023-07-21 14:25:28.000000 mkdoxy-1.1.6/mkdoxy.egg-info/SOURCES.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)        1 2023-07-21 14:25:28.000000 mkdoxy-1.1.6/mkdoxy.egg-info/dependency_links.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)       47 2023-07-21 14:25:28.000000 mkdoxy-1.1.6/mkdoxy.egg-info/entry_points.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)      124 2023-07-21 14:25:28.000000 mkdoxy-1.1.6/mkdoxy.egg-info/requires.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)        7 2023-07-21 14:25:28.000000 mkdoxy-1.1.6/mkdoxy.egg-info/top_level.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       38 2023-07-21 14:25:28.818001 mkdoxy-1.1.6/setup.cfg
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1830 2023-07-21 14:15:07.000000 mkdoxy-1.1.6/setup.py
```

### Comparing `mkdoxy-1.1.5/LICENSE` & `mkdoxy-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.5/PKG-INFO` & `mkdoxy-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdoxy
-Version: 1.1.5
+Version: 1.1.6
 Summary: MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 Home-page: https://github.com/JakubAndrysek/MkDoxy
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Project-URL: Source, https://github.com/JakubAndrysek/MkDoxy
 Project-URL: Documentation, https://mkdoxy.kubaandrysek.cz/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.5 Summary: MkDoxy â MkDocs +
+Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.6 Summary: MkDoxy â MkDocs +
 Doxygen = easy documentation generator with code snippets Home-page: https://
 github.com/JakubAndrysek/MkDoxy Author: Jakub AndrÃ½sek Author-email:
 email@kubaandrysek.cz License: MIT Project-URL: Source, https://github.com/
 JakubAndrysek/MkDoxy Project-URL: Documentation, https://
 mkdoxy.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/JakubAndrysek/
 MkDoxy/issues Project-URL: Funding, https://github.com/sponsors/jakubandrysek
 Keywords: mkdoxy,python,open-
```

### Comparing `mkdoxy-1.1.5/README.md` & `mkdoxy-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.5/mkdoxy/DoxyTagParser.py` & `mkdoxy-1.1.6/mkdoxy/DoxyTagParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 
+
 class DoxyTagParser:
 
     def __init__(
             self,
             markdown_page: str,
             debug: bool = False
     ):
```

### Comparing `mkdoxy-1.1.5/mkdoxy/constants.py` & `mkdoxy-1.1.6/mkdoxy/constants.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.5/mkdoxy/doxygen.py` & `mkdoxy-1.1.6/mkdoxy/doxygen.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.5/mkdoxy/doxyrun.py` & `mkdoxy-1.1.6/mkdoxy/doxyrun.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import hashlib
 import logging
-import tempfile
+
 from pathlib import Path, PurePath
-from subprocess import Popen, PIPE
+from subprocess import PIPE, Popen
 from typing import Optional
 
 log: logging.Logger = logging.getLogger("mkdocs")
 
 
 class DoxygenRun:
 	"""! Class for running Doxygen.
```

### Comparing `mkdoxy-1.1.5/mkdoxy/finder.py` & `mkdoxy-1.1.6/mkdoxy/finder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from typing import Dict
+
 from mkdoxy.constants import Kind
 from mkdoxy.doxygen import Doxygen
 from mkdoxy.utils import recursive_find, recursive_find_with_parent
-from typing import Dict
+
 
 class Finder:
 	def __init__(self, doxygen: Dict[str, Doxygen], debug: bool = False):
 		self.doxygen = doxygen
 		self.debug = debug
 
 	def _normalize(self, name: str) -> str:
```

### Comparing `mkdoxy-1.1.5/mkdoxy/generatorAuto.py` & `mkdoxy-1.1.6/mkdoxy/generatorAuto.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.5/mkdoxy/generatorBase.py` & `mkdoxy-1.1.6/mkdoxy/generatorBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import logging
 import os
 import string
 from typing import Dict
 
-from jinja2 import Template, FileSystemLoader, Environment, ChoiceLoader
+from jinja2 import Template
 from jinja2.exceptions import TemplateError
 from mkdocs import exceptions
 
 import mkdoxy
 from mkdoxy.constants import Kind
-from mkdoxy.node import Node, DummyNode
-from mkdoxy.utils import parseTemplateFile, merge_two_dicts, recursive_find_with_parent, recursive_find
+from mkdoxy.node import DummyNode, Node
+from mkdoxy.utils import (
+    merge_two_dicts,
+    parseTemplateFile,
+    recursive_find,
+    recursive_find_with_parent,
+)
 
 log: logging.Logger = logging.getLogger("mkdocs")
 
 
 LETTERS = string.ascii_lowercase + '~_@\\'
 
 class GeneratorBase:
```

### Comparing `mkdoxy-1.1.5/mkdoxy/generatorSnippets.py` & `mkdoxy-1.1.6/mkdoxy/generatorSnippets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import logging
 import pathlib
 import re
-import string
-from pprint import *
 
-from mkdocs.config import Config
+import yaml
 from mkdocs.structure import pages
-from mkdoxy.doxygen import Doxygen
-
-from mkdoxy.generatorBase import GeneratorBase
-from ruamel.yaml import YAML, YAMLError
 
+from mkdoxy.doxygen import Doxygen
 from mkdoxy.finder import Finder
+from mkdoxy.generatorBase import GeneratorBase
 from mkdoxy.node import Node
 
 log: logging.Logger = logging.getLogger("mkdocs")
 
 regexIncorrect = r"(?s)(?<!```yaml\n)(^::: doxy)(\.(?P<project>[a-zA-Z0-9_]+))?[\.]?[\s]*\n(?P<yaml>.*?)\s*\n(?:(?=\n)|(?=:::)|\Z)" # https://regex101.com/r/IYl25b/2
 regexLong= r"(?s)(?<!```yaml\n)(^::: doxy\.(?P<project>[a-zA-Z0-9_]+)\.(?P<argument>[a-zA-Z0-9_.]+))\s*\n(?P<yaml>.*?)(?:(?:(?:\r*\n)(?=\n))|(?=:::)|`|\Z)" #https://regex101.com/r/lIgOij/4
 regexShort = r"(?s)(?<!```yaml\n)(^::: doxy\.(?P<project>[a-zA-Z0-9_]+)\.(?P<argument>[a-zA-Z0-9_.]+))\s*\n(?:(?=\n)|(?=:::)|\Z)"# https://regex101.com/r/QnqxRc/2
@@ -108,17 +104,16 @@
 
 			replaceStr = self.call_doxy_by_name(snippet, project_name, argument, snippet_config)
 			self.replace_markdown(match.start(), match.end(), replaceStr)
 		return self.markdown
 
 	def try_load_yaml(self, yaml_raw: str, project: str, snippet: str, config: dict) -> dict:
 		try:
-			yaml = YAML()
-			return yaml.load(yaml_raw)
-		except YAMLError as e:
+			return yaml.safe_load(yaml_raw)
+		except yaml.YAMLError as e:
 			log.error(f"YAML error in {project} project on page {self.page.url}")
 			self.doxyError(
 				project,
 				config,
 				"YAML error",
 				"Check your YAML syntax",
 				"YAML snippet:",
```

### Comparing `mkdoxy-1.1.5/mkdoxy/markdown.py` & `mkdoxy-1.1.6/mkdoxy/markdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import List
 
+
 def escape(s: str) -> str:
 	ret = s.replace('*', '\\*')
 	ret = ret.replace('_', '\\_')
 	ret = ret.replace('<', '&lt;')
 	ret = ret.replace('>', '&gt;')
 	return ret.replace('|', '\|')
```

### Comparing `mkdoxy-1.1.5/mkdoxy/node.py` & `mkdoxy-1.1.6/mkdoxy/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 from xml.etree import ElementTree
 from xml.etree.ElementTree import Element as Element
 
 from mkdoxy.cache import Cache
-from mkdoxy.constants import Kind, Visibility, OVERLOAD_OPERATORS
+from mkdoxy.constants import OVERLOAD_OPERATORS, Kind, Visibility
 from mkdoxy.markdown import escape
 from mkdoxy.property import Property
 from mkdoxy.utils import split_safe
 from mkdoxy.xml_parser import XmlParser
 
 log: logging.Logger = logging.getLogger("mkdocs")
```

### Comparing `mkdoxy-1.1.5/mkdoxy/plugin.py` & `mkdoxy-1.1.6/mkdoxy/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,25 +5,24 @@
 """
 
 import logging
 import os
 from pathlib import Path, PurePath
 
 from mkdocs import exceptions
-from mkdocs.config import base, config_options, Config
+from mkdocs.config import Config, base, config_options
 from mkdocs.plugins import BasePlugin
 from mkdocs.structure import files, pages
 
 from mkdoxy.cache import Cache
 from mkdoxy.doxygen import Doxygen
 from mkdoxy.doxyrun import DoxygenRun
 from mkdoxy.generatorAuto import GeneratorAuto
 from mkdoxy.generatorBase import GeneratorBase
 from mkdoxy.generatorSnippets import GeneratorSnippets
-from mkdoxy.utils import check_enabled_markdown_extensions
 from mkdoxy.xml_parser import XmlParser
 
 log: logging.Logger = logging.getLogger("mkdocs")
 pluginName: str = "MkDoxy"
 
 
 class MkDoxy(BasePlugin):
```

### Comparing `mkdoxy-1.1.5/mkdoxy/property.py` & `mkdoxy-1.1.6/mkdoxy/property.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.5/mkdoxy/templates/annotated.jinja2` & `mkdoxy-1.1.6/mkdoxy/templates/annotated.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.5/mkdoxy/templates/code.jinja2` & `mkdoxy-1.1.6/mkdoxy/templates/code.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.5/mkdoxy/templates/error.jinja2` & `mkdoxy-1.1.6/mkdoxy/templates/error.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.5/mkdoxy/templates/examples.jinja2` & `mkdoxy-1.1.6/mkdoxy/templates/examples.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.5/mkdoxy/templates/memDef.jinja2` & `mkdoxy-1.1.6/mkdoxy/templates/memDef.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.5/mkdoxy/templates/memTab.jinja2` & `mkdoxy-1.1.6/mkdoxy/templates/memTab.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.5/mkdoxy/templates/member.jinja2` & `mkdoxy-1.1.6/mkdoxy/templates/member.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.5/mkdoxy/utils.py` & `mkdoxy-1.1.6/mkdoxy/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import re
 
+import yaml
 from mkdocs.config import Config
-from ruamel.yaml import YAML
 
 log: logging.Logger = logging.getLogger("mkdocs")
 
 
 regex = r"(-{3}|\.{3})\n(?P<meta>([\S\s])*)\n(-{3}|\.{3})\n(?P<template>([\S\s])*)"
 
 # Credits: https://stackoverflow.com/a/1630350
@@ -69,18 +69,16 @@
 
 
 def parseTemplateFile(templateFile: str):
 	match = re.match(regex, templateFile, re.MULTILINE)
 	if match:
 		template = match["template"]
 		meta = match["meta"]
-		yaml = YAML(typ='safe')
-		metaData = yaml.load(meta)
-		# yaml.dump(metaData, sys.stdout)
-		return template, metaData
+		metadata = yaml.safe_load(meta)
+		return template, metadata
 	return templateFile, {}
 
 
 def merge_two_dicts(base, new):
 	"https://stackoverflow.com/a/26853961"
 	result = base.copy()  # start with keys and values of x
 	result.update(new)  # modifies z with keys and values of y
```

### Comparing `mkdoxy-1.1.5/mkdoxy/xml_parser.py` & `mkdoxy-1.1.6/mkdoxy/xml_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,29 @@
 from xml.etree.ElementTree import Element as Element
 
 from mkdoxy.cache import Cache
-from mkdoxy.markdown import Md, MdRenderer, MdParagraph, MdTable, Code, MdTableRow, MdCodeBlock, MdTableCell, \
-    MdHeader, MdImage, MdList, MdBlockQuote, MdLink, MdBold, MdItalic, Text, Br
+from mkdoxy.markdown import (
+    Br,
+    Code,
+    Md,
+    MdBlockQuote,
+    MdBold,
+    MdCodeBlock,
+    MdHeader,
+    MdImage,
+    MdItalic,
+    MdLink,
+    MdList,
+    MdParagraph,
+    MdRenderer,
+    MdTable,
+    MdTableCell,
+    MdTableRow,
+    Text,
+)
 from mkdoxy.utils import lookahead
 
 SIMPLE_SECTIONS = {
 	'see': 'See also:',
 	'note': 'Note:',
 	'bug': 'Bug:',
 	'warning': 'Warning:',
```

### Comparing `mkdoxy-1.1.5/mkdoxy.egg-info/PKG-INFO` & `mkdoxy-1.1.6/mkdoxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdoxy
-Version: 1.1.5
+Version: 1.1.6
 Summary: MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 Home-page: https://github.com/JakubAndrysek/MkDoxy
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Project-URL: Source, https://github.com/JakubAndrysek/MkDoxy
 Project-URL: Documentation, https://mkdoxy.kubaandrysek.cz/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.5 Summary: MkDoxy â MkDocs +
+Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.6 Summary: MkDoxy â MkDocs +
 Doxygen = easy documentation generator with code snippets Home-page: https://
 github.com/JakubAndrysek/MkDoxy Author: Jakub AndrÃ½sek Author-email:
 email@kubaandrysek.cz License: MIT Project-URL: Source, https://github.com/
 JakubAndrysek/MkDoxy Project-URL: Documentation, https://
 mkdoxy.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/JakubAndrysek/
 MkDoxy/issues Project-URL: Funding, https://github.com/sponsors/jakubandrysek
 Keywords: mkdoxy,python,open-
```

### Comparing `mkdoxy-1.1.5/mkdoxy.egg-info/SOURCES.txt` & `mkdoxy-1.1.6/mkdoxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.5/setup.py` & `mkdoxy-1.1.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def requirements():
     with open('requirements.txt') as f:
         return f.read().splitlines()
 
 # https://pypi.org/project/mkdoxy/
 setup(
     name='mkdoxy',
-    version='1.1.5',
+    version='1.1.6',
     description='MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets',
     long_description=readme(),
     long_description_content_type='text/markdown',
     keywords='mkdoxy, python, open-source, documentation, mkdocs, doxygen, multilanguage, code-snippets, code, snippets, documentation-generator',
     url='https://github.com/JakubAndrysek/MkDoxy',
     author='Jakub Andrýsek',
     author_email='email@kubaandrysek.cz',
@@ -25,23 +25,23 @@
     project_urls={
         'Source': 'https://github.com/JakubAndrysek/MkDoxy',
         'Documentation': 'https://mkdoxy.kubaandrysek.cz/',
         'Tracker': 'https://github.com/JakubAndrysek/MkDoxy/issues',
         'Funding': 'https://github.com/sponsors/jakubandrysek',
     },
 
-    install_requires=['mkdocs', 'ruamel.yaml'],
+    install_requires=['mkdocs'],
     extras_require={
         "dev": [
             "mkdocs-material==9.1.18",
             "Jinja2~=3.1.2",
-            "ruamel.yaml~=0.17.32",
             "mkdocs-open-in-new-tab~=1.0.2",
             "pathlib~=1.0.1",
             "path~=16.7.1",
+            "isort~=5.12.0"
             ],
     },
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
```

