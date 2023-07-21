# Comparing `tmp/sysml2py-0.3.1.tar.gz` & `tmp/sysml2py-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysml2py-0.3.1.tar", last modified: Tue Jul 11 03:41:28 2023, max compression
+gzip compressed data, was "sysml2py-0.4.0.tar", max compression
```

## Comparing `sysml2py-0.3.1.tar` & `sysml2py-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:41:28.403995 sysml2py-0.3.1/
--rw-r--r--   0 root         (0) root         (0)     1068 2023-07-11 03:41:18.000000 sysml2py-0.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3872 2023-07-11 03:41:28.403995 sysml2py-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3371 2023-07-11 03:41:18.000000 sysml2py-0.3.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1067 2023-07-11 03:41:19.000000 sysml2py-0.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 03:41:28.403995 sysml2py-0.3.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:41:28.399995 sysml2py-0.3.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:41:28.399995 sysml2py-0.3.1/src/sysml2py/
--rw-r--r--   0 root         (0) root         (0)     2313 2023-07-11 03:41:18.000000 sysml2py-0.3.1/src/sysml2py/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2250 2023-07-11 03:41:18.000000 sysml2py-0.3.1/src/sysml2py/formatting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:41:28.403995 sysml2py-0.3.1/src/sysml2py/grammar/
--rw-r--r--   0 root         (0) root         (0)    22296 2023-07-11 03:41:18.000000 sysml2py-0.3.1/src/sysml2py/grammar/KerML.tx
--rw-r--r--   0 root         (0) root         (0)    10762 2023-07-11 03:41:18.000000 sysml2py-0.3.1/src/sysml2py/grammar/KerMLExpressions.tx
--rw-r--r--   0 root         (0) root         (0)    48820 2023-07-11 03:41:18.000000 sysml2py-0.3.1/src/sysml2py/grammar/SysML.tx
--rw-r--r--   0 root         (0) root         (0)   100319 2023-07-11 03:41:18.000000 sysml2py-0.3.1/src/sysml2py/grammar/classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:41:28.403995 sysml2py-0.3.1/src/sysml2py/textx/
--rw-r--r--   0 root         (0) root         (0)     6279 2023-07-11 03:41:18.000000 sysml2py-0.3.1/src/sysml2py/textx/xtext_to_textx.py
--rw-r--r--   0 root         (0) root         (0)    20633 2023-07-11 03:41:18.000000 sysml2py-0.3.1/src/sysml2py/usage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:41:28.403995 sysml2py-0.3.1/sysml2py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3872 2023-07-11 03:41:28.000000 sysml2py-0.3.1/sysml2py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      404 2023-07-11 03:41:28.000000 sysml2py-0.3.1/sysml2py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 03:41:28.000000 sysml2py-0.3.1/sysml2py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-11 03:41:28.000000 sysml2py-0.3.1/sysml2py.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1068 2023-07-21 18:07:48.162754 sysml2py-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3757 2023-07-21 18:07:48.162754 sysml2py-0.4.0/README.md
+-rw-r--r--   0        0        0     1555 2023-07-21 18:07:49.086865 sysml2py-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3297 2023-07-21 18:07:48.162754 sysml2py-0.4.0/src/sysml2py/__init__.py
+-rw-r--r--   0        0        0     8052 2023-07-21 18:07:48.162754 sysml2py-0.4.0/src/sysml2py/definition.py
+-rw-r--r--   0        0        0     2297 2023-07-21 18:07:48.162754 sysml2py-0.4.0/src/sysml2py/formatting.py
+-rw-r--r--   0        0        0    22296 2023-07-21 18:07:48.162754 sysml2py-0.4.0/src/sysml2py/grammar/KerML.tx
+-rw-r--r--   0        0        0    10762 2023-07-21 18:07:48.162754 sysml2py-0.4.0/src/sysml2py/grammar/KerMLExpressions.tx
+-rw-r--r--   0        0        0    48820 2023-07-21 18:07:48.166754 sysml2py-0.4.0/src/sysml2py/grammar/SysML.tx
+-rw-r--r--   0        0        0   105604 2023-07-21 18:07:48.166754 sysml2py-0.4.0/src/sysml2py/grammar/classes.py
+-rw-r--r--   0        0        0    28524 2023-07-21 18:07:48.166754 sysml2py-0.4.0/src/sysml2py/textx/KerML.xtext
+-rw-r--r--   0        0        0    14284 2023-07-21 18:07:48.166754 sysml2py-0.4.0/src/sysml2py/textx/KerMLExpressions.xtext
+-rw-r--r--   0        0        0    60663 2023-07-21 18:07:48.166754 sysml2py-0.4.0/src/sysml2py/textx/SysML.xtext
+-rw-r--r--   0        0        0     6279 2023-07-21 18:07:48.166754 sysml2py-0.4.0/src/sysml2py/textx/xtext_to_textx.py
+-rw-r--r--   0        0        0    22976 2023-07-21 18:07:48.166754 sysml2py-0.4.0/src/sysml2py/usage.py
+-rw-r--r--   0        0        0     4266 1970-01-01 00:00:00.000000 sysml2py-0.4.0/PKG-INFO
```

### Comparing `sysml2py-0.3.1/LICENSE` & `sysml2py-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sysml2py-0.3.1/PKG-INFO` & `sysml2py-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,11 @@
-Metadata-Version: 2.1
-Name: sysml2py
-Version: 0.3.1
-Summary: SysML v2.0 Parser
-Author-email: Christopher Cox <chris.cox@westfall.io>
-Project-URL: Homepage, https://github.com/Westfall-io/sysml2py
-Project-URL: Bug Tracker, https://github.com/Westfall-io/sysml2py/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # sysml2py
-[![PyPI version](https://badge.fury.io/py/sysml2py.svg)](https://badge.fury.io/py/sysml2py)[![Coverage Status](https://coveralls.io/repos/github/Westfall-io/sysml2py/badge.svg)](https://coveralls.io/github/Westfall-io/sysml2py)![Docstring Coverage](https://raw.githubusercontent.com/Westfall-io/sysml2py/main/doc-cov.svg)
+[![PyPI version](https://badge.fury.io/py/sysml2py.svg)](https://badge.fury.io/py/sysml2py)[![PyPI status](https://img.shields.io/pypi/status/sysml2py.svg)](https://pypi.python.org/pypi/sysml2py/)[![Coverage Status](https://coveralls.io/repos/github/Westfall-io/sysml2py/badge.svg)](https://coveralls.io/github/Westfall-io/sysml2py)![Docstring Coverage](https://raw.githubusercontent.com/Westfall-io/sysml2py/main/doc-cov.svg)[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 
-:construction:This project is just starting and is alpha.:construction:
+[![Trello](https://img.shields.io/badge/Trello-%23026AA7.svg?style=for-the-badge&logo=Trello&logoColor=white)](https://trello.com/b/xHfFUzlk/sysml2py)
 
 ## Description
 sysml2py is an open source pure Python library for constructing python-based
 classes consistent with the [SysML v2.0 standard](https://github.com/Systems-Modeling/SysML-v2-Release).
 
 ## Requirements
 sysml2py requires the following Python packages:
@@ -94,10 +80,12 @@
    part camera {
       attribute mass;
    }
    item lens;
 }
 ```
 
+## Release Planning
+Development can be tracked via [Trello.](https://trello.com/b/xHfFUzlk/sysml2py)
 
 ## License
 sysml2py is released under the MIT license, hence allowing commercial use of the library.
```

### Comparing `sysml2py-0.3.1/README.md` & `sysml2py-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,27 @@
+Metadata-Version: 2.1
+Name: sysml2py
+Version: 0.4.0
+Summary: 
+Author: Christopher Cox
+Author-email: chris.cox@westfall.io
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: astropy (>=5.3.1,<6.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: textx (>=3.1.1,<4.0.0)
+Description-Content-Type: text/markdown
+
 # sysml2py
-[![PyPI version](https://badge.fury.io/py/sysml2py.svg)](https://badge.fury.io/py/sysml2py)[![Coverage Status](https://coveralls.io/repos/github/Westfall-io/sysml2py/badge.svg)](https://coveralls.io/github/Westfall-io/sysml2py)![Docstring Coverage](https://raw.githubusercontent.com/Westfall-io/sysml2py/main/doc-cov.svg)
+[![PyPI version](https://badge.fury.io/py/sysml2py.svg)](https://badge.fury.io/py/sysml2py)[![PyPI status](https://img.shields.io/pypi/status/sysml2py.svg)](https://pypi.python.org/pypi/sysml2py/)[![Coverage Status](https://coveralls.io/repos/github/Westfall-io/sysml2py/badge.svg)](https://coveralls.io/github/Westfall-io/sysml2py)![Docstring Coverage](https://raw.githubusercontent.com/Westfall-io/sysml2py/main/doc-cov.svg)[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 
-:construction:This project is just starting and is alpha.:construction:
+[![Trello](https://img.shields.io/badge/Trello-%23026AA7.svg?style=for-the-badge&logo=Trello&logoColor=white)](https://trello.com/b/xHfFUzlk/sysml2py)
 
 ## Description
 sysml2py is an open source pure Python library for constructing python-based
 classes consistent with the [SysML v2.0 standard](https://github.com/Systems-Modeling/SysML-v2-Release).
 
 ## Requirements
 sysml2py requires the following Python packages:
@@ -80,10 +96,13 @@
    part camera {
       attribute mass;
    }
    item lens;
 }
 ```
 
+## Release Planning
+Development can be tracked via [Trello.](https://trello.com/b/xHfFUzlk/sysml2py)
 
 ## License
 sysml2py is released under the MIT license, hence allowing commercial use of the library.
+
```

### Comparing `sysml2py-0.3.1/src/sysml2py/__init__.py` & `sysml2py-0.4.0/src/sysml2py/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,55 +5,47 @@
 
 @author: christophercox
 """
 
 __all__ = ["load", "loads"]
 __author__ = "Christopher Cox"
 
-from sysml2py.usage import Item, Attribute, Part
+from sysml2py.usage import Item, Attribute, Part, Port
+from sysml2py.definition import Model, Package
 
 
-def load(fp):
+def load_grammar(fp, formatting="json"):
     """SysML load from file pointer
 
     Deserialize ``fp`` (a ``.read()``-supporting file-like object containing
-    a SysML v2.0 document) to a Python dictionary object.
+    a SysML v2.0 document) or ``s`` (a ``str`` instance containing a SysML
+    v2.0 document) to a Python dictionary object.
 
     Parameters
     ----------
-    fp : _io.TextIOWrapper
-        File pointer to SysML v2.0 document
+    fp : _io.TextIOWrapper or str
+        File pointer to SysML v2.0 document or string instance of SysML v2.0
+        document
 
     Returns
     -------
     dict
         Dictionary version structured utilizing SysML v2.0 grammar with some
         modifications to support available python libraries.
 
     Raises
     ------
     TypeError
         Input was not _io.TextIOWrapper
 
     """
-    import io
 
-    if not isinstance(fp, io.TextIOWrapper):
-        raise TypeError(
-            f"the SysML object must be _io.TextIOWrapper, "
-            f"not {fp.__class__.__name__}"
-        )
-
-    return loads(fp.read())
-
-
-def loads(s, formatting="json"):
     """SysML load from string
 
-    Deserialize ``s`` (a ``str`` instance containing a SysML v2.0 document)
+    Deserialize
     to a Python dictionary object.
 
     Parameters
     ----------
     fp : str
         String-format SysML v2.0 document
 
@@ -65,14 +57,26 @@
 
     Raises
     ------
     TypeError
         Input was not str
 
     """
+    import io
+
+    if isinstance(fp, io.TextIOWrapper):
+        s = fp.read()
+    elif isinstance(fp, str):
+        s = fp
+    else:
+        raise TypeError(
+            f"the SysML object must be _io.TextIOWrapper or str "
+            f"not {fp.__class__.__name__}"
+        )
+
     import importlib.resources as pkg_resources
 
     from textx import metamodel_from_file, TextXSyntaxError
 
     import sysml2py
     from sysml2py.formatting import reformat
 
@@ -95,7 +99,45 @@
 
         sys.exit()
 
     if formatting == "json":
         return reformat(model)
     else:
         return model
+
+
+def load(fp):
+    """SysML load from file pointer
+
+    Deserialize ``fp`` (a ``.read()``-supporting file-like object containing
+    a SysML v2.0 document) to a Python dictionary object.
+
+    Parameters
+    ----------
+    fp : _io.TextIOWrapper
+        File pointer to SysML v2.0 document
+
+    Returns
+    -------
+    dict
+        Dictionary version structured utilizing SysML v2.0 grammar with some
+        modifications to support available python libraries.
+
+    Raises
+    ------
+    TypeError
+        Input was not _io.TextIOWrapper
+
+    """
+    import io
+
+    if not isinstance(fp, io.TextIOWrapper):
+        raise TypeError(
+            f"the SysML object must be _io.TextIOWrapper, "
+            f"not {fp.__class__.__name__}"
+        )
+
+    return loads(fp.read())
+
+
+def loads(s: str):
+    return Model().load(s)
```

### Comparing `sysml2py-0.3.1/src/sysml2py/formatting.py` & `sysml2py-0.4.0/src/sysml2py/formatting.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 """
 Created on Wed May 31 13:26:53 2023
 
 @author: christophercox
 """
 
 from sysml2py.grammar.classes import RootNamespace
-from sysml2py import Part
+
+# from sysml2py import Part
 
 
 def remove_classes(model):
     """An example docstring for a class definition."""
     if type(model) == type(dict()):
         output = {}
         for element in model:
@@ -48,29 +49,29 @@
     return model_out
 
 
 def classtree(model):
     return RootNamespace(model)
 
 
-def collapse(model):
-    """Take a classtree and collapse it into our special classes that
-    package all of the sub-grammar classes."""
-    output = []
-    if model.__class__.__name__ == "RootNamespace":
-        for child in model.children[0].children:
-            if child.__class__.__name__ == "UsageElement":
-                ue = child.children
-                if ue.__class__.__name__ == "OccurrenceUsageElement":
-                    se = ue.children
-                    if se.children.__class__.__name__ == "PartUsage":
-                        output.append(Part().load_from_grammar(se.children))
-                    else:
-                        pass
-                else:
-                    # OccurrenceUsageElement
-                    pass
-            else:
-                pass
-    else:
-        print("no")
-    return output
+# def collapse(model):
+#     """Take a classtree and collapse it into our special classes that
+#     package all of the sub-grammar classes."""
+#     output = []
+#     if model.__class__.__name__ == "RootNamespace":
+#         for child in model.children[0].children:
+#             if child.__class__.__name__ == "UsageElement":
+#                 ue = child.children
+#                 if ue.__class__.__name__ == "OccurrenceUsageElement":
+#                     se = ue.children
+#                     if se.children.__class__.__name__ == "PartUsage":
+#                         output.append(Part().load_from_grammar(se.children))
+#                     else:
+#                         pass
+#                 else:
+#                     # OccurrenceUsageElement
+#                     pass
+#             else:
+#                 pass
+#     else:
+#         print("no")
+#     return output
```

### Comparing `sysml2py-0.3.1/src/sysml2py/grammar/KerML.tx` & `sysml2py-0.4.0/src/sysml2py/grammar/KerML.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.3.1/src/sysml2py/grammar/KerMLExpressions.tx` & `sysml2py-0.4.0/src/sysml2py/grammar/KerMLExpressions.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.3.1/src/sysml2py/grammar/SysML.tx` & `sysml2py-0.4.0/src/sysml2py/grammar/SysML.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.3.1/src/sysml2py/grammar/classes.py` & `sysml2py-0.4.0/src/sysml2py/grammar/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 def beautify(string):
     level = 0
     lines = string.split("\n")
     ns = []
     # print(lines)
     for line in lines:
+        line = line.rstrip()
         if line == "}":
             level += -1
 
         ns.append(level * "   " + line)
 
         if line[-1] == "{":
             # Last character is new bracket
@@ -57,34 +58,48 @@
                 print(definition)
                 raise NotImplementedError("Not expecting any other root node names.")
         else:
             raise AttributeError("This does not seem to be valid.")
 
     def load_package_body(self, definition):
         for member in definition:
-            # Options here are PackageMember, ElementFilterMember, AliasMember, Import
-            if member["name"] == "PackageMember":
-                memberclass = PackageMember(member)
-            elif member["name"] == "ElementFilterMember":
-                raise NotImplementedError
-            elif member["name"] == "AliasMember":
-                raise NotImplementedError
-            elif member["name"] == "Import":
-                raise NotImplementedError
-            else:
-                raise AttributeError("Error")
+            if isinstance(member, dict):
+                # Options here are PackageMember, ElementFilterMember, AliasMember, Import
+                if member["name"] == "PackageMember":
+                    memberclass = PackageMember(member)
+                elif member["name"] == "ElementFilterMember":
+                    raise NotImplementedError
+                elif member["name"] == "AliasMember":
+                    raise NotImplementedError
+                elif member["name"] == "Import":
+                    raise NotImplementedError
+                else:
+                    print(member["name"])
+                    raise AttributeError("Error")
 
-            self.children.append(memberclass)
+                self.children.append(memberclass)
+            else:
+                print(member)
+                raise TypeError("Invalid definition, member was not type dict")
 
     def dump(self):
         output = []
         for child in self.children:
             output.append(child.dump())
         return beautify("\n".join(output))
 
+    def get_definition(self):
+        output = {
+            "name": "PackageBodyElement",  # !TODO This isn't always the case
+            "ownedRelationship": [],
+        }
+        for member in self.children:
+            output["ownedRelationship"].append(member.get_definition())
+        return output
+
 
 class DefinitionElement:
     def __init__(self, definition):
         self.children = []
         if valid_definition(definition, "DefinitionElement"):
             # This is a SysML Element
             if isinstance(definition["ownedRelatedElement"], str):
@@ -266,38 +281,49 @@
             output.append("end")
         if self.usage is not None:
             output.append(self.usage.dump())
         return " ".join(output)
 
 
 class PortDefinition:
-    def __init__(self, definition):
-        if valid_definition(definition, self.__class__.__name__):
-            self.keyword = "port def"
-            self.prefix = None
-            self.definition = None
-
-            if definition["prefix"] is not None:
-                self.prefix = DefinitionPrefix(definition["prefix"])
+    def __init__(self, definition=None):
+        self.keyword = "port def"
+        self.prefix = None
+        if definition is not None:
+            if valid_definition(definition, self.__class__.__name__):
+                if definition["prefix"] is not None:
+                    self.prefix = DefinitionPrefix(definition["prefix"])
 
-            if definition["definition"] is not None:
-                self.definition = Definition(definition["definition"])
+                if definition["definition"] is not None:
+                    self.definition = Definition(definition["definition"])
+                else:
+                    raise AttributeError("Definition is required.")
+        else:
+            self.definition = Definition()
 
     def dump(self):
         output = []
         if self.prefix is not None:
             output.append(self.prefix.dump())
 
         output.append(self.keyword)
 
         if self.definition is not None:
             output.append(self.definition.dump())
 
         return " ".join(output)
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__, "prefix": None}
+        if self.prefix is not None:
+            output["prefix"] = self.prefix.get_definition()
+
+        output["definition"] = self.definition.get_definition()
+        return output
+
 
 class DefinitionPrefix:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             self.prefix = None
             self.keywords = []
 
@@ -931,14 +957,21 @@
                 )
             else:
                 raise AttributeError("This does not seem to be valid.")
 
     def dump(self):
         return self.children.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "ownedRelatedElement": self.children.get_definition(),
+        }
+        return output
+
 
 class NonOccurrenceUsageElement:
     def __init__(self, definition):
         if valid_definition(definition, "NonOccurrenceUsageElement"):
             if definition["ownedRelatedElement"]["name"] == "DefaultReferenceUsage":
                 self.children = DefaultReferenceUsage(definition["ownedRelatedElement"])
             elif definition["ownedRelatedElement"]["name"] == "AttributeUsage":
@@ -953,39 +986,53 @@
     def get_definition(self):
         output = {"name": self.__class__.__name__}
         output["ownedRelatedElement"] = self.children.get_definition()
         return output
 
 
 class DefaultReferenceUsage:
-    def __init__(self, definition):
-        if valid_definition(definition, "DefaultReferenceUsage"):
-            if definition["prefix"] is not None:
-                self.prefix = RefPrefix(definition["prefix"])
-            else:
-                self.prefix = None
+    def __init__(self, definition=None):
+        self.prefix = None
+        self.valuepart = None
+        if definition is not None:
+            if valid_definition(definition, "DefaultReferenceUsage"):
+                if definition["prefix"] is not None:
+                    self.prefix = RefPrefix(definition["prefix"])
 
-            self.declaration = UsageDeclaration(definition["declaration"])
-            if definition["valuepart"] is not None:
-                self.valuepart = ValuePart(definition["valuepart"])
-            else:
-                self.valuepart = None
-            self.body = UsageBody(definition["body"])
+                self.declaration = UsageDeclaration(definition["declaration"])
+                if definition["valuepart"] is not None:
+                    self.valuepart = ValuePart(definition["valuepart"])
+
+                self.body = UsageBody(definition["body"])
+        else:
+            self.declaration = UsageDeclaration()
+            self.body = UsageBody()
 
     def dump(self):
         output = []
         if self.prefix is not None:
             output.append(self.prefix.dump())
         output.append(self.declaration.dump())
         if self.valuepart is not None:
             output.append(self.valuepart.dump())
         output.append(self.body.dump())
 
         return " ".join(output)
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__, "prefix": None, "valuepart": None}
+        if self.prefix is not None:
+            output["prefix"] = self.prefix.get_definition()
+
+        if self.valuepart is not None:
+            output["valuepart"] = self.valuepart.get_definition()
+        output["declaration"] = self.declaration.get_definition()
+        output["body"] = self.body.get_definition()
+        return output
+
 
 class ValuePart:
     def __init__(self, definition):
         if valid_definition(definition, "ValuePart"):
             if len(definition["ownedRelationship"]) == 0:
                 raise NotImplementedError
             else:
@@ -1728,38 +1775,51 @@
         for relationship in self.relationships:
             output.append(relationship.dump())
 
         return " ".join(output)
 
 
 class PortUsage:
-    def __init__(self, definition):
-        if valid_definition(definition, self.__class__.__name__):
-            self.prefix = None
-            self.keyword = "port"
-            self.usage = None
+    def __init__(self, definition=None):
+        self.keyword = "port"
+        if definition is not None:
+            if valid_definition(definition, self.__class__.__name__):
+                self.prefix = None
+                self.usage = None
 
-            if definition["prefix"] is not None:
-                self.prefix = OccurrenceUsagePrefix(definition["prefix"])
+                if definition["prefix"] is not None:
+                    self.prefix = OccurrenceUsagePrefix(definition["prefix"])
 
-            if definition["usage"] is not None:
-                self.usage = Usage(definition["usage"])
+                if definition["usage"] is not None:
+                    self.usage = Usage(definition["usage"])
+        else:
+            self.prefix = None
+            self.usage = Usage()
 
     def dump(self):
         output = []
         if self.prefix is not None:
             output.append(self.prefix.dump())
 
         output.append(self.keyword)
 
         if self.usage is not None:
             output.append(self.usage.dump())
 
         return " ".join(output)
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__, "prefix": None}
+        if self.prefix is not None:
+            output["prefix"] = self.prefix.get_definition()
+
+        output["usage"] = self.usage.get_definition()
+
+        return output
+
 
 class ConnectionUsage:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             self.prefix = None
             if definition["prefix"] is not None:
                 self.prefix = OccurrenceUsagePrefix(definition["prefix"])
@@ -1989,31 +2049,41 @@
         if self.isReference:
             output.append("ref")
 
         return " ".join(output)
 
 
 class RefPrefix:
-    def __init__(self, definition):
-        if valid_definition(definition, self.__class__.__name__):
-            if definition["direction"] is not None:
-                self.direction = FeatureDirection(definition["direction"])
-            else:
-                self.direction = None
+    def __init__(self, definition=None):
+        self.direction = None
+        if definition is not None:
+            if valid_definition(definition, self.__class__.__name__):
+                if definition["direction"] is not None:
+                    self.direction = FeatureDirection(definition["direction"])
 
-            self.isAbstract = definition["isAbstract"]
-            self.isVariation = definition["isVariation"]
-            self.isReadOnly = definition["isReadOnly"]
-            self.isDerived = definition["isDerived"]
-            self.isEnd = definition["isEnd"]
+                self.isAbstract = definition["isAbstract"]
+                self.isVariation = definition["isVariation"]
+                self.isReadOnly = definition["isReadOnly"]
+                self.isDerived = definition["isDerived"]
+                self.isEnd = definition["isEnd"]
+
+        else:
+            self.direction = FeatureDirection()
+            self.isAbstract = False
+            self.isVariation = False
+            self.isReadOnly = False
+            self.isDerived = False
+            self.isEnd = False
 
     def dump(self):
         output = []
         if self.direction is not None:
-            output.append(self.direction.dump())
+            direction = self.direction.dump()
+            if not direction == "":
+                output.append(direction)
 
         if self.isAbstract:
             output.append("abstract")
         elif self.isVariation:
             output.append("variation")
 
         if self.isReadOnly:
@@ -2023,31 +2093,58 @@
             output.append("derived")
 
         if self.isEnd:
             output.append("end")
 
         return " ".join(output)
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__}
+        output["isAbstract"] = self.isAbstract
+        output["isVariation"] = self.isVariation
+        output["isReadOnly"] = self.isReadOnly
+        output["isDerived"] = self.isDerived
+        output["isEnd"] = self.isEnd
+        output["direction"] = self.direction.get_definition()
+        return output
+
 
 class FeatureDirection:
-    def __init__(self, definition):
-        if valid_definition(definition, self.__class__.__name__):
-            self.isIn = definition["in"] == "in "
-            self.isOut = definition["out"] == "out"
-            self.isInOut = definition["inout"] == "inout"
+    def __init__(self, definition=None):
+        if definition is not None:
+            if valid_definition(definition, self.__class__.__name__):
+                self.isIn = definition["in"] == "in "
+                self.isOut = definition["out"] == "out"
+                self.isInOut = definition["inout"] == "inout"
+        else:
+            self.isIn = False
+            self.isOut = False
+            self.isInOut = False
 
     def dump(self):
         if self.isInOut:
             return "inout"
         elif self.isIn:
             return "in"
         elif self.isOut:
             return "out"
         else:
-            raise NotImplementedError
+            return ""
+
+    def get_definition(self):
+        output = {"name": self.__class__.__name__, "in": "", "out": "", "inout": ""}
+        if self.isIn:
+            output["in"] = "in "
+
+        if self.isOut:
+            output["out"] = "out"
+
+        if self.isInOut:
+            output["inout"] = "inout"
+        return output
 
 
 class ItemUsage:
     def __init__(self, definition=None):
         if definition is not None:
             if valid_definition(definition, "ItemUsage"):
                 self.prefix = None
@@ -2678,40 +2775,73 @@
             output.append(child.dump())
 
         if self.prefix is not None:
             return " ".join(filter(None, (self.prefix.dump(), "".join(output))))
         else:
             return "".join(output)
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "prefix": None,
+            "ownedRelationship": [],
+        }
+        if self.prefix is not None:
+            output["prefix"] = self.prefix.get_definition()
+
+        for child in self.children:
+            output["ownedRelatedElement"] = child.get_definition()
+
+        return output
+
 
 class MemberPrefix:
     def __init__(self, definition):
         if valid_definition(definition, "MemberPrefix"):
             self.visibility = VisibilityIndicator(definition["visibility"])
 
     def dump(self):
         return self.visibility.dump()
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__}
+        output["visibility"] = self.visibility.get_definition()
+        return output
+
 
 class Package:
-    def __init__(self, definition):
-        if valid_definition(definition, "Package"):
-            # Elements inside of a package
-            # ownedRelationship += PrefixMetadataMember
-            # declaration = PackageDeclaration
-            # body = PackageBody
+    def __init__(self, definition=None):
+        if definition is not None:
+            if valid_definition(definition, self.__class__.__name__):
+                # Elements inside of a package
+                # ownedRelationship += PrefixMetadataMember
+                # declaration = PackageDeclaration
+                # body = PackageBody
+                self.relationships = []
+                for rel in definition["ownedRelationship"]:
+                    self.relationships.append(json.dumps(rel))
+                self.declaration = PackageDeclaration(definition["declaration"])
+                self.body = PackageBody(definition["body"])
+        else:
             self.relationships = []
-            for rel in definition["ownedRelationship"]:
-                self.relationships.append(json.dumps(rel))
-            self.declaration = PackageDeclaration(definition["declaration"])
-            self.body = PackageBody(definition["body"])
+            self.declaration = PackageDeclaration()
+            self.body = PackageBody()
 
     def dump(self):
         return "".join([self.declaration.dump(), self.body.dump()])
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__, "ownedRelationship": []}
+        for rel in self.relationships:
+            output["ownedRelationship"] = rel.get_definition()
+        output["declaration"] = self.declaration.get_definition()
+        output["body"] = self.body.get_definition()
+
+        return output
+
 
 class Identification:
     def __init__(self, definition=None):
         if definition is not None:
             if valid_definition(definition, "Identification"):
                 if definition["declaredShortName"] == None:
                     self.declaredShortName = None
@@ -2737,56 +2867,74 @@
         output = {"name": self.__class__.__name__}
         output["declaredShortName"] = self.declaredShortName
         output["declaredName"] = self.declaredName
         return output
 
 
 class PackageDeclaration:
-    def __init__(self, definition):
-        if valid_definition(definition, "PackageDeclaration"):
-            self.identification = Identification(definition["identification"])
+    def __init__(self, definition=None):
+        if definition is not None:
+            if valid_definition(definition, "PackageDeclaration"):
+                self.identification = Identification(definition["identification"])
+        else:
+            self.identification = Identification()
 
     def dump(self):
         return "package " + self.identification.dump()
 
+    def get_definition(self):
+        return {
+            "name": self.__class__.__name__,
+            "identification": self.identification.get_definition(),
+        }
+
 
 class PackageBody:
-    def __init__(self, definition):
+    def __init__(self, definition=None):
         self.children = []
-        if valid_definition(definition, "PackageBody"):
-            if "ownedRelationship" in definition:
-                for relationship in definition["ownedRelationship"]:
-                    if "name" in relationship:
-                        if relationship["name"] == "PackageMember":
-                            self.children.append(PackageMember(relationship))
-                        elif relationship["name"] == "ElementFilterMember":
-                            raise NotImplementedError
-                        elif relationship["name"] == "AliasMember":
-                            self.children.append(AliasMember(relationship))
-                        elif relationship["name"] == "Import":
-                            self.children.append(Import(relationship))
+        if definition is not None:
+            if valid_definition(definition, "PackageBody"):
+                if "ownedRelationship" in definition:
+                    for relationship in definition["ownedRelationship"]:
+                        if "name" in relationship:
+                            if relationship["name"] == "PackageMember":
+                                self.children.append(PackageMember(relationship))
+                            elif relationship["name"] == "ElementFilterMember":
+                                raise NotImplementedError
+                            elif relationship["name"] == "AliasMember":
+                                self.children.append(AliasMember(relationship))
+                            elif relationship["name"] == "Import":
+                                self.children.append(Import(relationship))
+                            else:
+                                raise AttributeError(
+                                    "Failed to match this relationship"
+                                )
                         else:
-                            raise AttributeError("Failed to match this relationship")
-                    else:
-                        raise NotImplementedError
-            else:
-                raise NotImplementedError
-        else:
-            raise AttributeError("This does not seem to be valid.")
+                            raise NotImplementedError
+                else:
+                    raise NotImplementedError
+            # else: handled inside function
+        # else: no new definitions needed
 
     def dump(self):
         #!TODO This won't work
         if len(self.children) == 0:
             return ";"
         else:
             output = []
             for child in self.children:
                 output.append(child.dump())
             return " { \n" + "\n".join(output) + "\n}"
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__, "ownedRelationship": []}
+        for child in self.children:
+            output["ownedRelationship"].append(child.get_definition())
+        return output
+
 
 class AliasMember:
     def __init__(self, definition):
         if valid_definition(definition, "AliasMember"):
             if definition["prefix"] is not None:
                 self.prefix = MemberPrefix(definition["prefix"])
             else:
```

### Comparing `sysml2py-0.3.1/src/sysml2py/textx/xtext_to_textx.py` & `sysml2py-0.4.0/src/sysml2py/textx/xtext_to_textx.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.3.1/src/sysml2py/usage.py` & `sysml2py-0.4.0/src/sysml2py/usage.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 """
 Created on Fri Jun 30 23:23:31 2023
 
 @author: christophercox
 """
 
 
-import os
+# import os
 
-os.chdir(os.path.join(os.path.dirname(os.path.abspath(__file__)), ".."))
+# os.chdir(os.path.join(os.path.dirname(os.path.abspath(__file__)), ".."))
 
 import uuid as uuidlib
 
 import astropy.units as u
 
+from sysml2py.formatting import classtree
+
 from sysml2py.grammar.classes import (
     Identification,
     DefinitionBody,
     DefinitionBodyItem,
     FeatureSpecializationPart,
 )
 
@@ -26,163 +28,154 @@
     AttributeUsage,
     AttributeDefinition,
     ValuePart,
     PartUsage,
     PartDefinition,
     ItemUsage,
     ItemDefinition,
+    PortUsage,
+    PortDefinition,
+    DefaultReferenceUsage,
+    RefPrefix,
 )
 
 
 class Usage:
     def __init__(self):
         self.name = str(uuidlib.uuid4())
         self.children = []
         self.typedby = None
         return self
 
-    def usage_dump(self, child):
-        # This is a usage.
-
+    def _ensure_body(self, subgrammar="usage"):
         # Add children
         body = []
         for abc in self.children:
-            body.append(DefinitionBodyItem(abc.dump(child=True)).get_definition())
+            body.append(
+                DefinitionBodyItem(abc.dump(child="DefinitionBody")).get_definition()
+            )
 
         if len(body) > 0:
-            self.grammar.usage.completion.body.body = DefinitionBody(
+            getattr(self.grammar, subgrammar).completion.body.body = DefinitionBody(
                 {"name": "DefinitionBody", "ownedRelatedElement": body}
             )
+        return self
+
+    def usage_dump(self, child):
+        # This is a usage.
+
+        self._ensure_body("usage")
 
         # Add packaging
         package = {
             "name": "StructureUsageElement",
             "ownedRelatedElement": self.grammar.get_definition(),
         }
         package = {"name": "OccurrenceUsageElement", "ownedRelatedElement": package}
 
-        if child:
+        if child == "DefinitionBody":
             package = {
                 "name": "OccurrenceUsageMember",
                 "prefix": None,
                 "ownedRelatedElement": [package],
             }
+
             package = {"name": "DefinitionBodyItem", "ownedRelationship": [package]}
-        else:
-            # Add these packets to make this dump without parents
+        elif "PackageBody":
             package = {"name": "UsageElement", "ownedRelatedElement": package}
             package = {
                 "name": "PackageMember",
                 "ownedRelatedElement": package,
                 "prefix": None,
             }
-            package = {
-                "name": "PackageBodyElement",
-                "ownedRelationship": [package],
-                "prefix": None,
-            }
+
         return package
 
     def definition_dump(self, child):
         # This is a definition.
 
-        # Add children
-        body = []
-        for abc in self.children:
-            body.append(DefinitionBodyItem(abc.dump(child=True)).get_definition())
-        if len(body) > 0:
-            self.grammar.definition.completion.body.body = DefinitionBody(
-                {"name": "DefinitionBody", "ownedRelatedElement": body}
-            )
+        self._ensure_body("definition")
 
-        if child:
-            package = {
-                "name": "DefinitionElement",
-                "prefix": None,
-                "ownedRelatedElement": self.grammar.get_definition(),
-            }
+        package = {
+            "name": "DefinitionElement",
+            "ownedRelatedElement": self.grammar.get_definition(),
+        }
+
+        if child == "DefinitionBody":
             package = {
                 "name": "DefinitionMember",
                 "prefix": None,
                 "ownedRelatedElement": [package],
             }
+
             package = {"name": "DefinitionBodyItem", "ownedRelationship": [package]}
 
-        else:
+        elif child == "PackageBody":
             # Add these packets to make this dump without parents
-            package = {
-                "name": "DefinitionElement",
-                "ownedRelatedElement": self.grammar.get_definition(),
-            }
+
             package = {
                 "name": "PackageMember",
                 "ownedRelatedElement": package,
                 "prefix": None,
             }
-            package = {
-                "name": "PackageBodyElement",
-                "ownedRelationship": [package],
-                "prefix": None,
-            }
 
         return package
 
-    def dump(self, child=False):
+    def _get_definition(self, child=None):
         if "usage" in self.grammar.__dict__:
             package = self.usage_dump(child)
         else:
             package = self.definition_dump(child)
 
+        if child is None:
+            package = {
+                "name": "PackageBodyElement",
+                "ownedRelationship": [package],
+                "prefix": None,
+            }
+
         # Add the typed by definition to the package output
         if self.typedby is not None:
-            package["ownedRelationship"].insert(
-                0, self.typedby.dump(child)["ownedRelationship"][0]
-            )
+            if child is None:
+                package["ownedRelationship"].insert(
+                    0, self.typedby._get_definition(child="PackageBody")
+                )
+            elif child == "PackageBody":
+                package = [self.typedby._get_definition(child="PackageBody"), package]
+            else:
+                package["ownedRelationship"].insert(
+                    0, self.typedby._get_definition(child=child)["ownedRelationship"][0]
+                )
 
         return package
 
+    def dump(self, child=None):
+        return classtree(self._get_definition(child)).dump()
+
     def _set_name(self, name, short=False):
         if hasattr(self.grammar, "usage"):
-            if short:
-                if self.grammar.usage.declaration.declaration.identification is None:
-                    self.grammar.usage.declaration.declaration.identification = (
-                        Identification()
-                    )
-                self.grammar.usage.declaration.declaration.identification.declaredShortName = (
-                    "<" + name + ">"
-                )
+            path = self.grammar.usage.declaration.declaration
+        elif hasattr(self.grammar, "definition"):
+            path = self.grammar.definition.declaration
+        else:
+            if hasattr(self.grammar.declaration, "declaration"):
+                path = self.grammar.declaration.declaration
             else:
-                self.name = name
-                if self.grammar.usage.declaration.declaration.identification is None:
-                    self.grammar.usage.declaration.declaration.identification = (
-                        Identification()
-                    )
-                self.grammar.usage.declaration.declaration.identification.declaredName = (
-                    name
-                )
+                path = self.grammar.declaration
 
-            return self
+        if path.identification is None:
+            path.identification = Identification()
+
+        if short:
+            path.identification.declaredShortName = "<" + name + ">"
         else:
-            if short:
-                if self.grammar.definition.declaration.identification is None:
-                    self.grammar.definition.declaration.identification = (
-                        Identification()
-                    )
-                self.grammar.definition.declaration.identification.declaredShortName = (
-                    "<" + name + ">"
-                )
-            else:
-                self.name = name
-                if self.grammar.definition.declaration.identification is None:
-                    self.grammar.definition.declaration.identification = (
-                        Identification()
-                    )
-                self.grammar.definition.declaration.identification.declaredName = name
+            self.name = name
+            path.identification.declaredName = name
 
-            return self
+        return self
 
     def _get_name(self):
         return self.grammar.usage.declaration.declaration.identification.declaredName
 
     def _set_child(self, child):
         self.children.append(child)
         return self
@@ -248,42 +241,67 @@
                     )
         else:
             print(typed.grammar.__dict__)
             raise NotImplementedError
         return self
 
     def load_from_grammar(self, grammar):
+        #!TODO Typed By
         self.__init__()
         self.grammar = grammar
-        self.name = grammar.usage.declaration.declaration.identification.declaredName
-        if len(grammar.usage.completion.body.body.children) == 0:
-            pass
-        else:
-            for child in (
-                grammar.usage.completion.body.body.children[0].children[0].children
-            ):
-                if child.children.__class__.__name__ == "AttributeUsage":
-                    self.children.append(Attribute().load_from_grammar(child.children))
-                elif child.children.__class__.__name__ == "StructureUsageElement":
-                    if child.children.children.__class__.__name__ == "PartUsage":
-                        self.children.append(
-                            Part().load_from_grammar(child.children.children)
-                        )
-                    elif child.children.children.__class__.__name__ == "ItemUsage":
-                        self.children.append(
-                            Item().load_from_grammar(child.children.children)
-                        )
-                    else:
-                        print(child.children.children.__class__.__name__)
-                        raise NotImplementedError
+        children = []
+        if "usage" in self.grammar.__dict__:
+            # This is a usage
+            u_name = grammar.usage.declaration.declaration.identification.declaredName
+            a_children = grammar.usage.completion.body.body.children
+
+            if len(a_children) > 0:
+                children = a_children[0].children[0].children
+        else:
+            # This is a definition
+            u_name = grammar.definition.declaration.identification.declaredName
+            a_children = grammar.definition.body.children
+            if len(a_children) > 0:
+                children = a_children
+
+        if u_name is not None:
+            self.name = u_name
+
+        for child in children:
+            if child.children.__class__.__name__ == "AttributeUsage":
+                self.children.append(Attribute().load_from_grammar(child.children))
+            elif child.children.__class__.__name__ == "StructureUsageElement":
+                if child.children.children.__class__.__name__ == "PartUsage":
+                    self.children.append(
+                        Part().load_from_grammar(child.children.children)
+                    )
+                elif child.children.children.__class__.__name__ == "ItemUsage":
+                    self.children.append(
+                        Item().load_from_grammar(child.children.children)
+                    )
                 else:
-                    print(child.children.__class__.__name__)
+                    print(child.children.children.__class__.__name__)
                     raise NotImplementedError
+            else:
+                print(child.children.__class__.__name__)
+                raise NotImplementedError
+
         return self
 
+    def add_directed_feature(self, direction, name=str(uuidlib.uuid4())):
+        self._set_child(DefaultReference()._set_name(name).set_direction(direction))
+        return self
+
+    def modify_directed_feature(self, direction, name):
+        child = self._get_child(name)
+        if child is not None:
+            pass
+        else:
+            raise AttributeError("Invalid Feature Name or Chain")
+
 
 class Attribute(Usage):
     def __init__(self, definition=False, name=None):
         Usage.__init__(self)
 
         if definition:
             self.grammar = AttributeDefinition()
@@ -603,7 +621,89 @@
 class Item(Usage):
     def __init__(self, definition=False, name=None):
         Usage.__init__(self)
         if definition:
             self.grammar = ItemDefinition()
         else:
             self.grammar = ItemUsage()
+
+
+class Port(Usage):
+    def __init__(self, definition=False, name=None):
+        Usage.__init__(self)
+        if definition:
+            self.grammar = PortDefinition()
+        else:
+            self.grammar = PortUsage()
+
+
+class DefaultReference(Usage):
+    def __init__(self):
+        Usage.__init__(self)
+        self.grammar = DefaultReferenceUsage()
+
+    def set_direction(self, direction):
+        r = RefPrefix()
+        if direction == "in":
+            r.direction.isIn = True
+        elif direction == "out":
+            r.direction.isOut = True
+        elif direction == "inout":
+            r.direction.isInOut = True
+        else:
+            raise NotImplementedError
+        self.grammar.prefix = r
+        return self
+
+    def usage_dump(self, child):
+        # This is a usage.
+
+        self._ensure_body("definition")
+
+        # Add packaging
+        package = {
+            "name": "NonOccurrenceUsageElement",
+            "ownedRelatedElement": self.grammar.get_definition(),
+        }
+
+        if child == "DefinitionBody":
+            package = {
+                "name": "NonOccurrenceUsageMember",
+                "prefix": None,
+                "ownedRelatedElement": [package],
+            }
+
+            package = {"name": "DefinitionBodyItem", "ownedRelationship": [package]}
+        elif "PackageBody":
+            package = {"name": "UsageElement", "ownedRelatedElement": package}
+            package = {
+                "name": "PackageMember",
+                "ownedRelatedElement": package,
+                "prefix": None,
+            }
+
+        return package
+
+    def dump(self, child=None):
+        package = self.usage_dump(child)
+
+        if child is None:
+            package = {
+                "name": "PackageBodyElement",
+                "ownedRelationship": [package],
+                "prefix": None,
+            }
+
+        # Add the typed by definition to the package output
+        if self.typedby is not None:
+            if child is None:
+                package["ownedRelationship"].insert(
+                    0, self.typedby.dump(child="PackageBody")
+                )
+            elif child == "PackageBody":
+                package = [self.typedby.dump(child="PackageBody"), package]
+            else:
+                package["ownedRelationship"].insert(
+                    0, self.typedby.dump(child=child)["ownedRelationship"][0]
+                )
+
+        return package
```

