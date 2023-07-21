# Comparing `tmp/starfyre-0.8.1.tar.gz` & `tmp/starfyre-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starfyre-0.8.1.tar", max compression
+gzip compressed data, was "starfyre-0.9.0.tar", max compression
```

## Comparing `starfyre-0.8.1.tar` & `starfyre-0.9.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     4751 2023-07-15 12:43:05.678508 starfyre-0.8.1/README.md
--rw-r--r--   0        0        0      454 2023-07-15 12:43:05.678508 starfyre-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      949 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/__init__.py
--rw-r--r--   0        0        0     1981 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/__main__.py
--rw-r--r--   0        0        0     5636 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/compiler.py
--rw-r--r--   0        0        0      535 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/component.py
--rw-r--r--   0        0        0     3550 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/dom_methods.py
--rw-r--r--   0        0        0      126 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/global_components.py
--rw-r--r--   0        0        0        0 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/js/__init__.py
--rw-r--r--   0        0        0     1093 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/js/store.js
--rw-r--r--   0        0        0     9071 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/parser.py
--rw-r--r--   0        0        0     3544 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/transpiler.py
--rw-r--r--   0        0        0     5289 1970-01-01 00:00:00.000000 starfyre-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     4751 2023-07-18 23:12:07.074555 starfyre-0.9.0/README.md
+-rw-r--r--   0        0        0      454 2023-07-18 23:12:07.074555 starfyre-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      984 2023-07-18 23:12:07.074555 starfyre-0.9.0/starfyre/__init__.py
+-rw-r--r--   0        0        0     2642 2023-07-18 23:12:07.074555 starfyre-0.9.0/starfyre/__main__.py
+-rw-r--r--   0        0        0     6535 2023-07-18 23:12:07.074555 starfyre-0.9.0/starfyre/compiler.py
+-rw-r--r--   0        0        0      535 2023-07-18 23:12:07.074555 starfyre-0.9.0/starfyre/component.py
+-rw-r--r--   0        0        0     3550 2023-07-18 23:12:07.074555 starfyre-0.9.0/starfyre/dom_methods.py
+-rw-r--r--   0        0        0      589 2023-07-18 23:12:07.074555 starfyre-0.9.0/starfyre/exceptions.py
+-rw-r--r--   0        0        0      126 2023-07-18 23:12:07.074555 starfyre-0.9.0/starfyre/global_components.py
+-rw-r--r--   0        0        0        0 2023-07-18 23:12:07.074555 starfyre-0.9.0/starfyre/js/__init__.py
+-rw-r--r--   0        0        0     1093 2023-07-18 23:12:07.074555 starfyre-0.9.0/starfyre/js/store.js
+-rw-r--r--   0        0        0    10848 2023-07-18 23:12:07.074555 starfyre-0.9.0/starfyre/parser.py
+-rw-r--r--   0        0        0     3544 2023-07-18 23:12:07.074555 starfyre-0.9.0/starfyre/transpiler.py
+-rw-r--r--   0        0        0     5289 1970-01-01 00:00:00.000000 starfyre-0.9.0/PKG-INFO
```

### Comparing `starfyre-0.8.1/README.md` & `starfyre-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `starfyre-0.8.1/starfyre/__init__.py` & `starfyre-0.9.0/starfyre/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 from starfyre.component import Component
 from .transpiler import transpile
 
 from .parser import RootParser
 
 
-def create_component(pyml="", css="", js="", client_side_python=""):
+def create_component(pyml="", css="", js="", client_side_python="", component_name=""):
     if client_side_python:
         new_js = transpile(client_side_python) + js
         js = new_js
 
     local_variables = inspect.currentframe().f_back.f_back.f_locals.copy()
     global_variables = inspect.currentframe().f_back.f_back.f_globals.copy()
 
-    parser = RootParser(local_variables, global_variables, css, js)
+    parser = RootParser(local_variables, global_variables, css, js, component_name)
     pyml = pyml.strip("\n").strip()
     parser.feed(pyml)
     parser.close()
     pyml_root = parser.get_root()
 
     if pyml_root is None:
         return Component("div", {}, [], {}, {}, uuid="store", js=js)
```

### Comparing `starfyre-0.8.1/starfyre/__main__.py` & `starfyre-0.9.0/starfyre/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,14 +12,25 @@
     dist_path = Path(path) / "dist"
     dist_path.mkdir(exist_ok=True)
     js_store = pkg_resources.path("starfyre.js", "store.js")
     shutil.copy(str(js_store), path + "/dist/store.js")
 
 
 def create_main_file(path):
+    """
+    Creates a main file in the build directory.
+    
+    This file will be used to run the project.
+    Every starfyre build will have an `__init__.py` file in the build directory.
+    And the `__init__.py` file will have a component that will render the root component. It will be named `app`.
+
+    You can have a look at the `test-application/build/__init__.py` file to see what it looks like.
+
+    The main file is also responsible for adding the `store.js` file to the `index.html` file.
+    """
     output_file_path = path + "/build/__main__.py"
     write_js_file(path)
 
     with open(output_file_path, "w") as f:
         f.write(
             """
 from . import app
@@ -59,21 +70,24 @@
 
     # Convert path to absolute path
     absolute_path = Path(path).resolve()
 
     if build:
         # Compile and build project
         init_file_path = absolute_path / "__init__.py"
+      
         compile(init_file_path.resolve())
+        # At this point, the project has been compiled and the build directory has been created.
+        # But there is no main file in the build directory.
         create_main_file(str(absolute_path))
 
         # Start/run project
         subprocess.run(
             [sys.executable, "-m", "build"],
             cwd=path,
             stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
+            stderr=None,
         )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `starfyre-0.8.1/starfyre/compiler.py` & `starfyre-0.9.0/starfyre/compiler.py`

 * *Files 24% similar despite different names*

```diff
@@ -123,15 +123,16 @@
 {pyml_lines}
 """, css="""
 {css_lines}
 """, js="""
 {js_lines}
 """, client_side_python="""
 {client_side_python}
-"""
+""",
+component_name="""{root_name}"""
 )
     return render_root(component)
 
 {root_name}=fx_{root_name}()
 '''
     else:
         return f'''
@@ -142,15 +143,16 @@
 {pyml_lines}
 """, css="""
 {css_lines}
 """, js="""
 {js_lines}
 """, client_side_python="""
 {client_side_python}
-"""
+""",
+component_name="""{root_name}"""
 )
     return component
 
 {root_name}=fx_{root_name}()
 '''
 
 
@@ -159,14 +161,21 @@
     css_lines,
     pyml_lines,
     js_lines,
     client_side_python,
     output_file_name,
     project_dir,
 ):
+    """
+    Transpiles a fyre file into a python file.
+
+    This function is responsible for:
+    - parsing the fyre file into python, css, pyml, js and client side python
+
+    """
     final_python_lines = ["".join(python_lines)]
 
     main_content = python_transpiled_string(
         pyml_lines, css_lines, js_lines, client_side_python, output_file_name
     )
 
     final_python_lines.append(main_content)
@@ -175,20 +184,29 @@
     output_file_name = project_dir / "build" / file_name
 
     with open(output_file_name, "w") as output_file:
         output_file.write("".join(final_python_lines))          #result of the transpiled
 
 
 def compile(entry_file_name):
+    """
+    Compiles a fyre project into a python project.
+    This function is responsible for:
+    - finding all fyre files in the project
+    - transpiling each fyre file into a python file.
+        - "transpiling" is used a bit loosely here. What we're really doing is slicing up the fyre file into different components and then inserting them into a python file.
+        - We have two functions important for us in python files `create_component` and `render_root`. 
+        - The `init.py` file will have a component that will render root and the rest of the files will have components that will be rendered inside the root component.
+    """
     project_dir = Path(os.path.dirname(entry_file_name))
 
     build_dir = project_dir / "build"
     build_dir.mkdir(exist_ok=True)
 
-    fyre_files = get_fyre_files(project_dir)
+    fyre_files = get_fyre_files(project_dir) 
 
     for fyre_file in fyre_files:
         python_file_name = fyre_file.replace(".fyre", ".py")
         python_lines, css_lines, pyml_lines, js_lines, client_side_python = parse(
             project_dir / fyre_file
         )
         transpile_to_python(
```

### Comparing `starfyre-0.8.1/starfyre/component.py` & `starfyre-0.9.0/starfyre/component.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.8.1/starfyre/dom_methods.py` & `starfyre-0.9.0/starfyre/dom_methods.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.8.1/starfyre/js/store.js` & `starfyre-0.9.0/starfyre/js/store.js`

 * *Files identical despite different names*

### Comparing `starfyre-0.8.1/starfyre/parser.py` & `starfyre-0.9.0/starfyre/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 from html.parser import HTMLParser
 from uuid import uuid4
 
 from starfyre.transpiler import transpile
 
 from .component import Component
+from .exceptions import UnknownTagError
 
 
 def extract_functions(obj):
     functions = {}
     for key, value in obj.items():
         if callable(value):
             functions[key] = value
@@ -16,17 +17,28 @@
     return functions
 
 
 class RootParser(HTMLParser):
     # this is the grammar for the parser
     # we need cover all the grammar rules
 
-    generic_tags = ["div", "p", "b", "span", "i", "button"]
+    generic_tags = {
+        "html", "div", "p", "b", "span", "i", "button", "head", "link", "meta", "style", "title",
+        "body", "section", "nav", "main", "hgroup", "h1", "h2", "h3", "h4", "h5", "h6",
+        "header", "footer", "aside", "article", "address", "blockquote", "dd", "dl", "dt",
+        "figcaption", "figure", "hr", "li", "ol", "ul", "menu", "pre", "a", "abbr", "bdi",
+        "bdo", "br", "cite", "code", "data", "em", "mark", "q", "s", "small", "strong", "sub",
+        "sup", "time", "u", "area", "audio", "img", "map", "track", "video", "embed", "iframe",
+        "picture", "object", "portal", "svg", "math", "canvas", "script", "noscript", "caption",
+        "col", "colgroup", "table", "tbody", "td", "tfoot", "th", "thead", "tr", "datalist",
+        "fieldlist", "form", "input", "label", "legend", "meter", "optgroup", "option", "output",
+        "progress", "select", "textarea", "details", "dialog", "summary"
+    }
 
-    def __init__(self, component_local_variables, component_global_variables, css, js):
+    def __init__(self, component_local_variables, component_global_variables, css, js, component_name):
         super().__init__()
         self.stack: list[tuple[Component, int]] = []
         self.children = []
         self.current_depth = 0
         self.css = css
         self.js = js
 
@@ -34,34 +46,37 @@
         self.local_variables = component_local_variables
         self.global_variables = component_global_variables
 
         self.components = self.extract_components(
             {**self.local_variables, **self.global_variables}
         )
         # populate the dict with the components
+        self.component_name = component_name
+        
 
     def extract_components(self, local_functions):
         components = {}
         for key, value in local_functions.items():
             if isinstance(value, Component):
                 components[key] = value
 
         return components
 
     def is_event_listener(self, name):
         return name.startswith("on")
-
+        
     def handle_starttag(self, tag, attrs):
         # logic should be to just create an empty component on start
         # and fill the contents on the end tag
         props = {}
         state = {}
         event_listeners = {}
         self.current_depth += 1
 
+        # extracting the attributes found in the tags
         for attr in attrs:
             if attr[1].startswith("{") and attr[1].endswith("}"):
                 attr_value = attr[1].strip("{").strip("}").strip(" ")
                 if self.is_event_listener(attr[0]):
                     event_handler = None
                     if attr_value in self.global_variables:
                         event_handler = self.global_variables[attr_value]
@@ -82,24 +97,31 @@
                         self.local_variables[attr_value]
                     ):
                         state[attr[0]] = self.local_variables[attr_value]
                         props[attr[0]] = self.local_variables[attr_value]()
             else:
                 props[attr[0]] = attr[1]
 
+        # if the tag is not found in the generic tags but found in custom components
         if tag not in self.generic_tags and tag in self.components:
             component = self.components[tag]
             tag = component.tag
             component.props = {**component.props, **props}
             component.state = {**component.state, **state}
-            component.event_listeners = {**component.event_listeners, **event_listeners}
+            component.event_listeners = {
+                **component.event_listeners, **event_listeners}
             self.stack.append((component, self.current_depth))
 
+
             return
 
+        # if the tag is not found in the generic tags and custom components
+        if tag not in self.generic_tags and tag not in self.components:
+            raise UnknownTagError(f'Unknown tag: "{tag}". Please review line {self.lineno} in your "{self.component_name}" component in the pyml code.')
+
         component = Component(
             tag,
             props,
             [],
             event_listeners,
             state,
             js=self.js,
@@ -108,14 +130,18 @@
         )
 
         # instead of assiging tags we assign uuids
         self.stack.append((component, self.current_depth))
         [(element[0].tag, element[1]) for element in self.stack]
 
     def handle_endtag(self, tag):
+        # if the tag is not found in the generic tags and custom components
+        if tag not in self.generic_tags and tag not in self.components:             
+            raise UnknownTagError(f'Unknown tag: "{tag}". Please review line {self.lineno} in your "{self.component_name}" component in the pyml code.')
+
         # we need to check if the tag is a default component or a custom component
         # if it is a custom component, we get the element from the custom components dict
         if tag not in self.generic_tags and tag in self.components:
             component = self.components[tag]
             tag = component.tag
 
         # need to check the if this is always true
@@ -146,23 +172,21 @@
         return signal.replace("()", f"('{uuid}')")
 
     def handle_data(self, data):
         # this is doing too much
         # lexing
         # parsing
 
-
         # this is a very minimal version of lexing
         # we should ideally be writing a separate layer for lexing
         data = data.strip().strip("\n").strip(" ")
         # regex to find all the elements that are wrapped in {}
 
         matches = re.findall(r"{(.*?)}", data)
 
-
         # parsing starts here
         state = {}
 
         parent_node, parent_depth = self.stack[-1]
         uuid = uuid4()
         component_signal = ""
```

### Comparing `starfyre-0.8.1/starfyre/transpiler.py` & `starfyre-0.9.0/starfyre/transpiler.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.8.1/PKG-INFO` & `starfyre-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starfyre
-Version: 0.8.1
+Version: 0.9.0
 Summary: A Python Framework for writing Reactive web Front-Ends
 License: BSD 2.0
 Author: Sanskar Jethi
 Author-email: sansyrox@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

