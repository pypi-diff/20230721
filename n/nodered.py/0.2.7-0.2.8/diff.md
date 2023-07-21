# Comparing `tmp/nodered.py-0.2.7.tar.gz` & `tmp/nodered.py-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodered.py-0.2.7.tar", last modified: Tue Jul 18 09:12:28 2023, max compression
+gzip compressed data, was "nodered.py-0.2.8.tar", last modified: Fri Jul 21 09:36:13 2023, max compression
```

## Comparing `nodered.py-0.2.7.tar` & `nodered.py-0.2.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-18 09:12:28.790000 nodered.py-0.2.7/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.2.7/LICENSE
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2780 2023-07-18 09:12:28.880000 nodered.py-0.2.7/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2464 2023-07-18 09:07:11.000000 nodered.py-0.2.7/README.md
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-18 09:12:28.790000 nodered.py-0.2.7/nodered.py.egg-info/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2780 2023-07-18 09:12:28.000000 nodered.py-0.2.7/nodered.py.egg-info/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      599 2023-07-18 09:12:28.000000 nodered.py-0.2.7/nodered.py.egg-info/SOURCES.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-07-18 09:12:28.000000 nodered.py-0.2.7/nodered.py.egg-info/dependency_links.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-07-18 09:12:28.000000 nodered.py-0.2.7/nodered.py.egg-info/requires.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       74 2023-07-18 09:12:28.000000 nodered.py-0.2.7/nodered.py.egg-info/top_level.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.2.7/nodered.py.egg-info/zip-safe
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-18 09:12:28.790000 nodered.py-0.2.7/noderedpy/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      474 2023-07-18 08:37:06.000000 nodered.py-0.2.7/noderedpy/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    19526 2023-07-18 09:07:30.000000 nodered.py-0.2.7/noderedpy/_nodered.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4807 2023-07-10 01:12:44.000000 nodered.py-0.2.7/noderedpy/_property.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-18 09:12:28.790000 nodered.py-0.2.7/noderedpy/assets/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)   453665 2023-05-07 01:22:45.000000 nodered.py-0.2.7/noderedpy/assets/python-logo.png
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1260 2023-05-10 10:41:49.000000 nodered.py-0.2.7/noderedpy/decorator.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-18 09:12:28.790000 nodered.py-0.2.7/noderedpy/node-red-starter/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        8 2023-05-07 00:47:00.000000 nodered.py-0.2.7/noderedpy/node-red-starter/editorTheme.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1583 2023-07-18 08:40:46.000000 nodered.py-0.2.7/noderedpy/node-red-starter/index.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      266 2023-07-10 08:42:28.000000 nodered.py-0.2.7/noderedpy/node-red-starter/package.json
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-18 09:12:28.800000 nodered.py-0.2.7/noderedpy/templates/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     9689 2023-07-10 01:17:43.000000 nodered.py-0.2.7/noderedpy/templates/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      969 2023-05-10 10:44:16.000000 nodered.py-0.2.7/noderedpy/templates/template.html
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     5788 2023-07-11 11:51:18.000000 nodered.py-0.2.7/noderedpy/templates/template.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      290 2023-05-10 09:24:21.000000 nodered.py-0.2.7/noderedpy/templates/template.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-07-18 09:12:28.880000 nodered.py-0.2.7/setup.cfg
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1106 2023-06-02 04:28:29.000000 nodered.py-0.2.7/setup.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-21 09:36:13.550000 nodered.py-0.2.8/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.2.8/LICENSE
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2780 2023-07-21 09:36:13.630000 nodered.py-0.2.8/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2464 2023-07-18 09:07:11.000000 nodered.py-0.2.8/README.md
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-21 09:36:13.550000 nodered.py-0.2.8/nodered.py.egg-info/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2780 2023-07-21 09:36:13.000000 nodered.py-0.2.8/nodered.py.egg-info/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      599 2023-07-21 09:36:13.000000 nodered.py-0.2.8/nodered.py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-07-21 09:36:13.000000 nodered.py-0.2.8/nodered.py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-07-21 09:36:13.000000 nodered.py-0.2.8/nodered.py.egg-info/requires.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       74 2023-07-21 09:36:13.000000 nodered.py-0.2.8/nodered.py.egg-info/top_level.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.2.8/nodered.py.egg-info/zip-safe
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-21 09:36:13.550000 nodered.py-0.2.8/noderedpy/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      474 2023-07-21 08:45:36.000000 nodered.py-0.2.8/noderedpy/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    19526 2023-07-18 09:07:30.000000 nodered.py-0.2.8/noderedpy/_nodered.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     5037 2023-07-21 09:31:33.000000 nodered.py-0.2.8/noderedpy/_property.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-21 09:36:13.550000 nodered.py-0.2.8/noderedpy/assets/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)   453665 2023-05-07 01:22:45.000000 nodered.py-0.2.8/noderedpy/assets/python-logo.png
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1260 2023-05-10 10:41:49.000000 nodered.py-0.2.8/noderedpy/decorator.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-21 09:36:13.560000 nodered.py-0.2.8/noderedpy/node-red-starter/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        8 2023-05-07 00:47:00.000000 nodered.py-0.2.8/noderedpy/node-red-starter/editorTheme.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1583 2023-07-18 08:40:46.000000 nodered.py-0.2.8/noderedpy/node-red-starter/index.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      266 2023-07-10 08:42:28.000000 nodered.py-0.2.8/noderedpy/node-red-starter/package.json
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-21 09:36:13.560000 nodered.py-0.2.8/noderedpy/templates/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     9974 2023-07-21 09:29:12.000000 nodered.py-0.2.8/noderedpy/templates/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1056 2023-07-21 08:56:19.000000 nodered.py-0.2.8/noderedpy/templates/template.html
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     5801 2023-07-21 09:31:37.000000 nodered.py-0.2.8/noderedpy/templates/template.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      290 2023-05-10 09:24:21.000000 nodered.py-0.2.8/noderedpy/templates/template.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-07-21 09:36:13.630000 nodered.py-0.2.8/setup.cfg
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1106 2023-06-02 04:28:29.000000 nodered.py-0.2.8/setup.py
```

### Comparing `nodered.py-0.2.7/LICENSE` & `nodered.py-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.7/PKG-INFO` & `nodered.py-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.2.7
+Version: 0.2.8
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.2.7 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.8 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
```

### Comparing `nodered.py-0.2.7/README.md` & `nodered.py-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.7/nodered.py.egg-info/PKG-INFO` & `nodered.py-0.2.8/nodered.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.2.7
+Version: 0.2.8
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.2.7 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.8 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
```

### Comparing `nodered.py-0.2.7/nodered.py.egg-info/SOURCES.txt` & `nodered.py-0.2.8/nodered.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.7/noderedpy/_nodered.py` & `nodered.py-0.2.8/noderedpy/_nodered.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.7/noderedpy/_property.py` & `nodered.py-0.2.8/noderedpy/_property.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,36 +11,39 @@
         
     @property
     def display_name(self) -> str:
         return " ".join([
             item.capitalize()
             for item in self.name.split("_")
         ])
+    
+    @property
+    def var_name(self) -> str:
+        return f"np-var_{self.name}"
 
 class CodeProperty(Property):
     def __init__(self, name:str, default:str = "", language:str = None, height:int = 250, required:bool = False, display_icon:str = None):
         if not isinstance(default, str):
             raise TypeError("CodeProperty can accept types: [ 'dict', 'json string' ]")
         
         super().__init__(name, default, required, display_icon if display_icon else "fa fa-code")
         self.language, self.height =\
             language, height
 
 class InputProperty(Property):
     def __init__(self, name:str, default:Union[int, float, str] = None, required:bool = False, display_icon:str = None):
-        if not isinstance(default, (int, float, str)):
-            raise TypeError("InputProperty can accept types: [ 'int', 'float', 'str' ]")
-        
         if default is None:
             if isinstance(default, int):
                 default = 0
             elif isinstance(default, float):
                 default = 0.0
             else:
                 default = ""
+        elif not isinstance(default, (int, float, str)):
+            raise TypeError("InputProperty can accept types: [ 'int', 'float', 'str' ]")
 
         super().__init__(name, default, required, display_icon)
 
         if display_icon is None:
             if isinstance(default, (int, float)):
                 self.display_icon = "fa fa-sort-numeric-asc"
             else:
@@ -89,14 +92,20 @@
         super().__init__(name, default, required, display_icon if display_icon else "fa fa-check")
 
 class ComboBoxProperty(Property):
     def __init__(self, name:str, items:List[Any], default:str = None, required:bool = False, display_icon:str = None):
         if not isinstance(items, list):
             raise TypeError("items of ComboBoxProperty must be type: 'list'")
         
+        if default is None:
+            if len(items) > 0:
+                default = items[0]
+            else:
+                default = ""
+        
         super().__init__(name, default, required, display_icon if display_icon else "fa fa-filter")
         self.items = items
 
 # class FileProperty(Property):
 #     def __init__(self, name:str, default:str = None, required:bool = False, display_icon:str = None):
 #         super().__init__(name, default if default else "", required, display_icon if display_icon else "fa fa-file-text-o")
```

### Comparing `nodered.py-0.2.7/noderedpy/assets/python-logo.png` & `nodered.py-0.2.8/noderedpy/assets/python-logo.png`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.7/noderedpy/decorator.py` & `nodered.py-0.2.8/noderedpy/decorator.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.7/noderedpy/node-red-starter/index.js` & `nodered.py-0.2.8/noderedpy/node-red-starter/index.js`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.7/noderedpy/templates/__init__.py` & `nodered.py-0.2.8/noderedpy/templates/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,114 +39,114 @@
     for property in node.properties:
         if isinstance(property, InputProperty):
             properties_html.append(f"""
     <div class="form-row" style="margin-bottom:0px;">
         <label style="width:auto;"><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
     </div>
     <div class="form-row">
-        <input type="text" id="node-input-{property.name}" style="width:100%;">
+        <input type="text" id="node-input-{property.var_name}" style="width:100%;">
     </div>
 """)
             default_value = f'"{property.default}"' if isinstance(property.default, str) else str(property.default)
         elif isinstance(property, ListProperty):
             properties_html.append(f"""
     <div class="form-row" style="margin-bottom:0px;">
         <label style="width:auto;"><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
     </div>
-    <div class="form-row node-input-{property.name}-container-row">
-        <ol id="node-input-{property.name}-container" style="height:{property.height}px;"></ol>
+    <div class="form-row node-input-{property.var_name}-container-row">
+        <ol id="node-input-{property.var_name}-container" style="height:{property.height}px;"></ol>
     </div>
 """)
             properties_js_prepare.append('''
-            $("#node-input-''' + property.name + '''-container").editableList({
+            $("#node-input-''' + property.var_name + '''-container").editableList({
                 addItem: (container, idx, opt) => {
                     opt.idx = idx;
                     opt.value = opt.value ?? "";
 
                     container.css({ overflow: "hidden", display: "flex", "align-items": "center" });
                     $("<input>", { class: "input-list-item", type: "text", style:"flex:1;" }).val(opt.value).appendTo(container);
                 },
                 removable: true
             });
 
-            for (var item of this.''' + property.name + ''') {
-                $("#node-input-''' + property.name + '''-container").editableList("addItem", { value: item });
+            for (var item of node["''' + property.var_name + '''"]) {
+                $("#node-input-''' + property.var_name + '''-container").editableList("addItem", { value: item });
             }
 ''')
             properties_js_save.append('''
-            this.''' + property.name + ''' = [];
-            $("#node-input-''' + property.name + '''-container").editableList("items").each((_, item) => {
-                this.''' + property.name + '''.push(item.find("input.input-list-item").val());
+            node["''' + property.var_name + '''"] = [];
+            $("#node-input-''' + property.var_name + '''-container").editableList("items").each((_, item) => {
+                node["''' + property.var_name + '''"].push(item.find("input.input-list-item").val());
             });
 ''')
             default_value = str(property.default)
         elif isinstance(property, CodeProperty):
             properties_html.append(f"""
     <div class="form-row" style="margin-bottom:0px;">
         <label style="width:auto;"><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
     </div>
     <div class="form-row node-text-editor-row">
-        <div style="height:{property.height}px;" class="node-text-editor" id="node-input-{property.name}"></div>
+        <div style="height:{property.height}px;" class="node-text-editor" id="node-input-{property.var_name}"></div>
     </div>
 """)
             if property.language:
                 properties_js_prepare.append('''
-            this.''' + property.name + '''Editor = RED.editor.createEditor({
-                id: "node-input-''' + property.name + '''",
+            node["''' + property.var_name + '''Editor"] = RED.editor.createEditor({
+                id: "node-input-''' + property.var_name + '''",
                 mode: "ace/mode/''' + property.language + '''",
-                value: this.''' + property.name + ''',
+                value: node["''' + property.var_name + '''"],
                 focus: true
             });
 ''')
             else:
                 properties_js_prepare.append('''
-            this.''' + property.name + '''Editor = RED.editor.createEditor({
-                id: "node-input-''' + property.name + '''",
-                value: this.''' + property.name + ''',
+            node["''' + property.var_name + '''Editor"] = RED.editor.createEditor({
+                id: "node-input-''' + property.var_name + '''",
+                value: node["''' + property.var_name + '''"],
                 focus: true
             });
 ''')
             properties_js_cancel.append(f"""
-            this.{property.name}Editor.destroy();
-            delete this.{property.name}Editor;
+            node["{property.var_name}Editor"].destroy();
+            delete node["{property.var_name}Editor"];
 """)
             properties_js_save.append(f"""
-            $("#node-input-{property.name}").val(this.{property.name}Editor.getValue().trim());
-            this.{property.name}Editor.destroy();
-            delete this.{property.name}Editor;
+            $("#node-input-{property.var_name}").val(node["{property.var_name}Editor"].getValue().trim());
+            node["{property.var_name}Editor"].destroy();
+            delete node["{property.var_name}Editor"];
 """)
             default_value = f"`{property.default}`"
         elif isinstance(property, SpinnerProperty):
             properties_html.append(f"""
     <div class="form-row" style="margin-bottom:0px;">
         <label style="width:auto;"><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
     </div>
     <div class="form-row">
-        <input type="text" id="node-input-{property.name}" style="width:calc(100% - 22px);">
+        <input type="text" id="node-input-{property.var_name}" style="width:calc(100% - 22px);">
     </div>
 """)
             spinner_configs = []
             if property.min:
                 spinner_configs.append(f"                min: {property.min},")
             if property.max:
                 spinner_configs.append(f"                max: {property.max},")
             if property.step:
                 spinner_configs.append(f"                step: {property.step}")
 
             properties_js_prepare.append('''
-            $("#node-input-''' + property.name + '''").spinner({
+            $("#node-input-''' + property.var_name + '''").spinner({
                 ''' + "\n".join(spinner_configs) + '''
             });
 ''')
             default_value = str(property.default)
         elif isinstance(property, CheckBoxProperty):
             properties_html.append(f"""
     <div class="form-row">
         <label style="width:auto;"><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
-        <input type="checkbox" style="margin-left:10px;width:15px;height:15px;margin-bottom:5px;" id="node-input-{property.name}">
+        <input type="checkbox" style="margin-left:10px;width:15px;height:15px;margin-bottom:5px;" id="node-input-{property.var_name}">
     </div>
 """)
             default_value = "true" if property.default else "false"
         elif isinstance(property, ComboBoxProperty):
             options = "\n".join([
                 f"""
             <option value="{item}">{item}</option>
@@ -154,25 +154,25 @@
                 for item in property.items
             ])
             properties_html.append(f"""
     <div class="form-row" style="margin-bottom:0px;">
         <label style="width:auto;"><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
     </div>
     <div class="form-row">
-        <select id="node-input-{property.name}Select" style="width:100%;">
+        <select id="node-input-{property.var_name}Select" style="width:100%;">
 {options}
         </select>
-        <input type="text" id="node-input-{property.name}" style="display:none;">
+        <input type="text" id="node-input-{property.var_name}" style="display:none;">
     </div>
 """)
             properties_js_prepare.append('''
-            $("#node-input-''' + property.name + '''Select").val(this.''' + property.name + ''');
+            $("#node-input-''' + property.var_name + '''Select").val($("#node-input-''' + property.var_name + '''").val());
 ''')
             properties_js_save.append('''
-            $("#node-input-''' + property.name + '''").val($("#node-input-''' + property.name + ''';").val());
+            $("#node-input-''' + property.var_name + '''").val($("#node-input-''' + property.var_name + '''Select").val());
 ''')
             default_value = f'"{property.default}"' if isinstance(property.default, str) else str(property.default)
 #         elif isinstance(property, FileProperty):
 #             properties_html.append(f"""
 #     <div class="form-row" style="display:flex;flex-flow:row;align-items:center;">
 #         <label style="width:auto;margin-bottom:0px;"><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
 #         <input type="file" id="node-input-{property.name}" style="flex:1;">
@@ -193,15 +193,16 @@
 #             <tbody>
 #             </tbody>
 #         </table>
 #     </div>
 # """)
 
         if default_value:
-            properties_js.append("            " + property.name + ': { value: ' + default_value + ' }')
+            required = 'true' if property.required else 'false'
+            properties_js.append('            "' + property.var_name + '": { value: ' + default_value + ', required: ' + required + ' }')
 
     with open(os.path.join(__path__[0], "template.html"), "r", encoding = "utf-8") as tr:
         tt = tr.read()
 
     return tt.replace(
         "{$node_name}", node.name
     ).replace(
@@ -223,11 +224,11 @@
 def node_js(node:"noderedpy._nodered.Node", cache_dir:str) -> str:
     with open(os.path.join(__path__[0], "template.js"), "r", encoding = "utf-8") as tr:
         tt = tr.read()
 
     return tt.replace(
         "{$node_name}", node.name
     ).replace(
-        "{$node_properties}", str([ property.name for property in node.properties])
+        "{$node_properties}", str([ property.var_name for property in node.properties])
     ).replace(
         "{$cache_dir}", cache_dir
     )
```

### Comparing `nodered.py-0.2.7/noderedpy/templates/template.html` & `nodered.py-0.2.8/noderedpy/templates/template.html`

 * *Files 13% similar despite different names*

```diff
@@ -22,17 +22,20 @@
         },
         inputs: 1, outputs: 1,
         icon: {$node_icon},
         label: function() {
             return this.name;
         },
         oneditprepare: function() {
+            var node = this;
 {$properties_js_prepare}
         },
         oneditcancel: function() {
+            var node = this;
 {$properties_js_cancel}
         },
         oneditsave: function() {
+            var node = this;
 {$properties_js_save}
         }
     });
 </script>
```

### Comparing `nodered.py-0.2.7/noderedpy/templates/template.js` & `nodered.py-0.2.8/noderedpy/templates/template.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -60,15 +60,15 @@
             for (var name of {
                     $node_properties
                 }) {
                 var config_item = config[name];
                 if (typeof(config_item) == "string" && (config_item.startsWith("{") && config_item.endsWith("}"))) {
                     config_item = JSON.parse(config_item);
                 }
-                configToSend[name] = config_item;
+                configToSend[name.substring(7)] = config_item;
             }
 
             node.status({
                 fill: "green",
                 shape: "dot",
                 text: "Running"
             });
```

### Comparing `nodered.py-0.2.7/setup.py` & `nodered.py-0.2.8/setup.py`

 * *Files identical despite different names*

