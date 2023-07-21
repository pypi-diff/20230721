# Comparing `tmp/nicescad-0.0.1.tar.gz` & `tmp/nicescad-0.0.2.tar.gz`

## Comparing `nicescad-0.0.1.tar` & `nicescad-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 nicescad-0.0.1/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 nicescad-0.0.1/.pydevproject
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 nicescad-0.0.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 nicescad-0.0.1/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nicescad-0.0.1/examples/openjscad_logo.scad
--rw-r--r--   0        0        0   495635 2020-02-02 00:00:00.000000 nicescad-0.0.1/examples/openjscad_logo.stl
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nicescad-0.0.1/nicescad/__init__.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 nicescad-0.0.1/nicescad/local_filepicker.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 nicescad-0.0.1/nicescad/nicescad_cmd.py
--rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 nicescad-0.0.1/nicescad/openscad.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 nicescad-0.0.1/nicescad/profiler.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 nicescad-0.0.1/nicescad/version.py
--rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 nicescad-0.0.1/nicescad/webserver.py
--rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 nicescad-0.0.1/scripts/doc
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 nicescad-0.0.1/scripts/install
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 nicescad-0.0.1/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nicescad-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 nicescad-0.0.1/tests/basetest.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 nicescad-0.0.1/tests/test_openscad.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nicescad-0.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nicescad-0.0.1/LICENSE
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 nicescad-0.0.1/README.md
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 nicescad-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 nicescad-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 nicescad-0.0.2/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 nicescad-0.0.2/.pydevproject
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 nicescad-0.0.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 nicescad-0.0.2/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nicescad-0.0.2/examples/openjscad_logo.scad
+-rw-r--r--   0        0        0   495635 2020-02-02 00:00:00.000000 nicescad-0.0.2/examples/openjscad_logo.stl
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nicescad-0.0.2/nicescad/__init__.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 nicescad-0.0.2/nicescad/local_filepicker.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 nicescad-0.0.2/nicescad/nicescad_cmd.py
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 nicescad-0.0.2/nicescad/openscad.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 nicescad-0.0.2/nicescad/profiler.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 nicescad-0.0.2/nicescad/version.py
+-rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 nicescad-0.0.2/nicescad/webserver.py
+-rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 nicescad-0.0.2/scripts/doc
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 nicescad-0.0.2/scripts/install
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 nicescad-0.0.2/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nicescad-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 nicescad-0.0.2/tests/basetest.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 nicescad-0.0.2/tests/test_openscad.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nicescad-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nicescad-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 nicescad-0.0.2/README.md
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 nicescad-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 nicescad-0.0.2/PKG-INFO
```

### Comparing `nicescad-0.0.1/.github/workflows/build.yml` & `nicescad-0.0.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.1/.github/workflows/upload-to-pypi.yml` & `nicescad-0.0.2/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.1/examples/openjscad_logo.stl` & `nicescad-0.0.2/examples/openjscad_logo.stl`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.1/nicescad/local_filepicker.py` & `nicescad-0.0.2/nicescad/local_filepicker.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.1/nicescad/nicescad_cmd.py` & `nicescad-0.0.2/nicescad/nicescad_cmd.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.1/nicescad/openscad.py` & `nicescad-0.0.2/nicescad/openscad.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.1/nicescad/profiler.py` & `nicescad-0.0.2/nicescad/profiler.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.1/nicescad/version.py` & `nicescad-0.0.2/nicescad/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class Version(object):
     """
     Version handling for nicescad
     """
     name = "nicescad"
     version = nicescad.__version__
     date = '2023-07-19'
-    updated = '2023-07-19'
+    updated = '2023-07-21'
     description = 'Nice Scad',
     
     authors = 'Wolfgang Fahl'
     
     doc_url="https://github.com/WolfgangFahl/nicescad"
     chat_url="https://github.com/WolfgangFahl/nicescad/discussions"
     cm_url="https://github.com/WolfgangFahl/nicescad"
```

### Comparing `nicescad-0.0.1/nicescad/webserver.py` & `nicescad-0.0.2/nicescad/webserver.py`

 * *Files 21% similar despite different names*

```diff
@@ -48,58 +48,63 @@
             trace (bool, optional): Whether to include the traceback in the error message. Default is False.
         """
         if trace:
             self.error_msg = str(e) + "\n" + traceback.format_exc()
         else:
             self.error_msg = str(e)
         if self.error_area:
-            self.error_area.text=self.error_msg
+            self.error_area.set_value(self.error_msg)
         print(self.error_msg,file=sys.stderr)
 
  
-    def render(self, click_args):
+    def render(self, _click_args):
         """Renders the OpenScad string and updates the 3D scene with the result.
 
         Args:
             click_args (object): The click event arguments.
         """
         openscad_str = self.code_area.value
-        stl = self.oscad.openscad_str_to_file(openscad_str)
-        with self.scene:
-            self.scene.clear()
-            self.scene.stl("/stl/tmp.stl").move(x=-0.5).scale(0.06)
+        try:
+            _stl = self.oscad.openscad_str_to_file(openscad_str)
+            with self.scene:
+                self.scene.clear()
+                self.scene.stl("/stl/tmp.stl").move(x=-0.5).scale(0.06)
+        except Exception as ex:
+            self.handle_exception(ex,self.do_trace)    
             
-    def do_read_input(self, input: str):
+    def do_read_input(self, input_str: str):
         """Reads the given input.
 
         Args:
-            input (str): The input string representing a URL or local path.
+            input_str (str): The input string representing a URL or local path.
         """
-        if input.startswith('http://') or input.startswith('https://'):
-            response = requests.get(input)
+        if input_str.startswith('http://') or input_str.startswith('https://'):
+            response = requests.get(input_str)
             if response.status_code == 200:
                 return response.text
             else:
-                raise Exception(f'Unable to retrieve data from URL: {input}')
+                raise Exception(f'Unable to retrieve data from URL: {input_str}')
         else:
-            if os.path.exists(input):
-                with open(input, 'r') as file:
+            if os.path.exists(input_str):
+                with open(input_str, 'r') as file:
                     return file.read()
             else:
-                raise Exception(f'File does not exist: {input}')
+                raise Exception(f'File does not exist: {input_str}')
     
     def read_input(self, input: str):
         """Reads the given input and handles any exceptions.
 
         Args:
             input (str): The input string representing a URL or local file.
         """
-        self.input=input
         try:
             self.code = self.do_read_input(input)
+            self.input_input.set_value(input)
+            self.code_area.set_value(self.code)
+            self.error_area.set_value("")
             self.error_msg = None
         except Exception as e:
             self.code = None
             self.handle_exception(e, self.do_trace)
             
     def save_file(self):
         """Saves the current code to the last input file, if it was a local path."""
@@ -108,49 +113,91 @@
                 file.write(self.code)
         else:
             raise Exception('No local file to save to')
     
     async def open_file(self) -> None:
         """Opens a dialog."""
         result = await LocalFilePicker('~', multiple=True)
-        ui.notify(f'You chose {result}')
+        ui.notify(f'Opening {result}')
+        self.read_input(result)
     pass
+
+    def reload_file(self):
+        """
+        reload the input file
+        """
+        self.read_input(self.input)
+
+    def help(self):
+        """
+        show help dialog
+        """
+        pass
     
-    def menu(self):
+    def setup_menu(self):
         """Adds a link to the project's GitHub page in the web server's menu."""
-        ui.link('nicescad on GitHub', 'https://github.com/WolfgangFahl/nicescad')
-        with ui.row().classes('w-full items-center'):
-            result = ui.label().classes('mr-auto')
+        with ui.header() as self.header:
+            ui.label("nicescad")
             with ui.button(icon='menu'):
-                with ui.menu() as menu:
+                with ui.menu() as self.menu:
                     ui.menu_item('Open', self.open_file)
                     ui.menu_item('Save', self.save_file)
+                    ui.menu_item("Reload",self.reload_file)
                     ui.separator()
-                    ui.menu_item('Close', on_click=menu.close)
-       
+                    ui.menu_item('Help', on_click=self.help)
+        with ui.left_drawer().props('bordered').classes("w-4/12") as self.left_drawer:
+            ui.link('nicescad on GitHub', 'https://github.com/WolfgangFahl/nicescad')
+            pass
+    
+    def setup_footer(self):
+        """
+        setup the footer
+        """
+        with ui.footer() as self.footer:
+            ui.label("(c)2023 Wolfgang Fahl")
+            ui.link("Powered by nicegui","https://nicegui.io/").style("color: #fff") 
+  
+    def input_changed(self,cargs):
+        """
+        react on changed input
+        """
+        self.input=cargs.value
+        pass
+    
+    def code_changed(self,cargs):
+        """
+        react on changed code
+        """
+        self.code=cargs.value
+        pass
+        
     def home(self):
         """Generates the home page with a 3D viewer and a code editor."""
-        self.menu()
-        with ui.splitter() as splitter:
-            with splitter.before:
-                with ui.scene(width=1024, height=768) as scene:
-                    self.scene = scene
-                    scene.spot_light(distance=100, intensity=0.1).move(-10, 0, 10)
-            with splitter.after:
-                self.input_input=ui.input(value=self.input)
-                self.code_area = ui.textarea(value=self.code).props('clearable;rows=20')
-                self.error_area = ui.textarea()
-                ui.button('Render', on_click=self.render)
+        self.setup_menu()
+        with ui.column():
+            with ui.splitter() as splitter:
+                with splitter.before:
+                    with ui.scene(width=1024, height=768).classes("w-full") as scene:
+                        self.scene = scene
+                        scene.spot_light(distance=100, intensity=0.1).move(-10, 0, 10)
+                    with splitter.after:
+                        with ui.element("div").classes("w-full"):
+                            self.input_input=ui.input(
+                                value=self.input,
+                                on_change=self.input_changed).props("size=100")
+                            self.code_area = ui.textarea(value=self.code,on_change=self.code_changed).props('clearable').props("rows=25")
+                            ui.button('Render', on_click=self.render)
+        self.error_area = ui.textarea().classes("w-full").props("rows=10;cols=80;")        
+        self.setup_footer()        
         if self.args.input:
             self.read_input(self.args.input)
-  
         
     def settings(self):
         """Generates the settings page with a link to the project's GitHub page."""
-        self.menu()
+        self.setup_menu()
        
     def run(self, args):
         """Runs the UI of the web server.
 
         Args:
             args (list): The command line arguments.
         """
```

### Comparing `nicescad-0.0.1/scripts/doc` & `nicescad-0.0.2/scripts/doc`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.1/tests/basetest.py` & `nicescad-0.0.2/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.1/tests/test_openscad.py` & `nicescad-0.0.2/tests/test_openscad.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.1/.gitignore` & `nicescad-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.1/LICENSE` & `nicescad-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.1/README.md` & `nicescad-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,7 +7,11 @@
 [![PyPI Status](https://img.shields.io/pypi/v/nicescad.svg)](https://pypi.python.org/pypi/nicescad/)
 [![GitHub issues](https://img.shields.io/github/issues/WolfgangFahl/nicescad.svg)](https://github.com/WolfgangFahl/nicescad/issues)
 [![GitHub closed issues](https://img.shields.io/github/issues-closed/WolfgangFahl/nicescad.svg)](https://github.com/WolfgangFahl/nicescad/issues/?q=is%3Aissue+is%3Aclosed)
 [![License](https://img.shields.io/github/license/WolfgangFahl/nicescad.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
 ## Docs and Tutorials
 [Wiki](https://wiki.bitplan.com/index.php/nicescad)
+
+## Links
+* https://openscad.org/
+* https://nicegui.io
```

### Comparing `nicescad-0.0.1/pyproject.toml` & `nicescad-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.1/PKG-INFO` & `nicescad-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicescad
-Version: 0.0.1
+Version: 0.0.2
 Project-URL: Home, https://github.com/WolfgangFahl/nicescad
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/nicescad
 Project-URL: Source, https://github.com/WolfgangFahl/nicescad
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -38,7 +38,11 @@
 [![PyPI Status](https://img.shields.io/pypi/v/nicescad.svg)](https://pypi.python.org/pypi/nicescad/)
 [![GitHub issues](https://img.shields.io/github/issues/WolfgangFahl/nicescad.svg)](https://github.com/WolfgangFahl/nicescad/issues)
 [![GitHub closed issues](https://img.shields.io/github/issues-closed/WolfgangFahl/nicescad.svg)](https://github.com/WolfgangFahl/nicescad/issues/?q=is%3Aissue+is%3Aclosed)
 [![License](https://img.shields.io/github/license/WolfgangFahl/nicescad.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
 ## Docs and Tutorials
 [Wiki](https://wiki.bitplan.com/index.php/nicescad)
+
+## Links
+* https://openscad.org/
+* https://nicegui.io
```

