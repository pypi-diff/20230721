# Comparing `tmp/catmux-0.3.2.tar.gz` & `tmp/catmux-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catmux-0.3.2.tar", last modified: Thu Apr 20 12:02:47 2023, max compression
+gzip compressed data, was "catmux-0.3.3.tar", last modified: Fri Jul 21 15:25:21 2023, max compression
```

## Comparing `catmux-0.3.2.tar` & `catmux-0.3.3.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-04-20 12:02:47.075002 catmux-0.3.2/
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1068 2023-04-04 19:35:47.000000 catmux-0.3.2/LICENSE
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     6129 2023-04-20 12:02:47.075002 catmux-0.3.2/PKG-INFO
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     5698 2023-04-04 19:35:47.000000 catmux-0.3.2/README.md
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-04-20 12:02:47.075002 catmux-0.3.2/catmux/
--rw-rw-r--   0 mauch     (1000) mauch     (1000)        0 2023-04-04 19:35:47.000000 catmux-0.3.2/catmux/__init__.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1477 2023-04-04 19:35:47.000000 catmux-0.3.2/catmux/prefix.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     8388 2023-04-04 19:35:47.000000 catmux-0.3.2/catmux/session.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     2172 2023-04-04 19:35:47.000000 catmux-0.3.2/catmux/split.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     2426 2023-04-04 19:35:47.000000 catmux-0.3.2/catmux/tmux_wrapper.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     3812 2023-04-04 19:35:47.000000 catmux-0.3.2/catmux/window.py
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-04-20 12:02:47.075002 catmux-0.3.2/catmux.egg-info/
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     6129 2023-04-20 12:02:47.000000 catmux-0.3.2/catmux.egg-info/PKG-INFO
--rw-rw-r--   0 mauch     (1000) mauch     (1000)      381 2023-04-20 12:02:47.000000 catmux-0.3.2/catmux.egg-info/SOURCES.txt
--rw-rw-r--   0 mauch     (1000) mauch     (1000)        1 2023-04-20 12:02:47.000000 catmux-0.3.2/catmux.egg-info/dependency_links.txt
--rw-rw-r--   0 mauch     (1000) mauch     (1000)        7 2023-04-20 12:02:47.000000 catmux-0.3.2/catmux.egg-info/requires.txt
--rw-rw-r--   0 mauch     (1000) mauch     (1000)        7 2023-04-20 12:02:47.000000 catmux-0.3.2/catmux.egg-info/top_level.txt
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-04-20 12:02:47.075002 catmux-0.3.2/etc/
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1984 2023-04-04 19:35:47.000000 catmux-0.3.2/etc/example_session.yaml
--rw-rw-r--   0 mauch     (1000) mauch     (1000)      810 2023-04-04 19:35:47.000000 catmux-0.3.2/etc/readme_tmux.txt
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1593 2023-04-04 19:35:47.000000 catmux-0.3.2/etc/tmux_default.conf
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-04-20 12:02:47.075002 catmux-0.3.2/script/
--rwxrwxr-x   0 mauch     (1000) mauch     (1000)     4646 2023-04-04 19:35:47.000000 catmux-0.3.2/script/catmux_create_session
--rw-rw-r--   0 mauch     (1000) mauch     (1000)       38 2023-04-20 12:02:47.075002 catmux-0.3.2/setup.cfg
--rw-rw-r--   0 mauch     (1000) mauch     (1000)      964 2023-04-20 12:00:07.000000 catmux-0.3.2/setup.py
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-07-21 15:25:21.172839 catmux-0.3.3/
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1068 2023-04-04 19:35:47.000000 catmux-0.3.3/LICENSE
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     6391 2023-07-21 15:25:21.172839 catmux-0.3.3/PKG-INFO
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     5940 2023-07-21 15:13:50.000000 catmux-0.3.3/README.md
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-07-21 15:25:21.172839 catmux-0.3.3/catmux/
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)        0 2023-04-04 19:35:47.000000 catmux-0.3.3/catmux/__init__.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)      210 2023-07-21 15:13:50.000000 catmux-0.3.3/catmux/exceptions.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1477 2023-04-04 19:35:47.000000 catmux-0.3.3/catmux/prefix.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     9333 2023-07-21 15:13:50.000000 catmux-0.3.3/catmux/session.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     2172 2023-04-04 19:35:47.000000 catmux-0.3.3/catmux/split.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     2426 2023-04-04 19:35:47.000000 catmux-0.3.3/catmux/tmux_wrapper.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     4066 2023-07-21 15:13:50.000000 catmux-0.3.3/catmux/window.py
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-07-21 15:25:21.172839 catmux-0.3.3/catmux.egg-info/
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     6391 2023-07-21 15:25:21.000000 catmux-0.3.3/catmux.egg-info/PKG-INFO
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)      444 2023-07-21 15:25:21.000000 catmux-0.3.3/catmux.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)        1 2023-07-21 15:25:21.000000 catmux-0.3.3/catmux.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)        7 2023-07-21 15:25:21.000000 catmux-0.3.3/catmux.egg-info/requires.txt
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)        7 2023-07-21 15:25:21.000000 catmux-0.3.3/catmux.egg-info/top_level.txt
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-07-21 15:25:21.172839 catmux-0.3.3/etc/
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1984 2023-07-21 13:14:52.000000 catmux-0.3.3/etc/example_session.yaml
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)      810 2023-04-04 19:35:47.000000 catmux-0.3.3/etc/readme_tmux.txt
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1593 2023-04-04 19:35:47.000000 catmux-0.3.3/etc/tmux_default.conf
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-07-21 15:25:21.172839 catmux-0.3.3/script/
+-rwxrwxr-x   0 mauch     (1000) mauch     (1000)     4797 2023-07-21 15:13:50.000000 catmux-0.3.3/script/catmux_create_session
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)       38 2023-07-21 15:25:21.172839 catmux-0.3.3/setup.cfg
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)      964 2023-07-21 15:23:08.000000 catmux-0.3.3/setup.py
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-07-21 15:25:21.172839 catmux-0.3.3/test/
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)      873 2023-07-21 14:44:10.000000 catmux-0.3.3/test/test_helpers.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     2159 2023-07-21 15:22:06.000000 catmux-0.3.3/test/test_parsing.py
```

### Comparing `catmux-0.3.2/LICENSE` & `catmux-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `catmux-0.3.2/PKG-INFO` & `catmux-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: catmux
-Version: 0.3.2
+Version: 0.3.3
 Summary: A tmux orchestration package.
 Home-page: https://github.com/fmauch/catmux
 Author: Felix Exner
 Author-email: felix_mauch@web.de
 License: MIT
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Catmux
+[![codecov](https://codecov.io/gh/fmauch/catmux/branch/master/graph/badge.svg?token=bPcdYrOBRK)](https://codecov.io/gh/fmauch/catmux)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## About
 Catmux is a little helper to run a tmux session with multiple windows and panes with just one
 command. It is inspired and functionally very similar to
 [tmuxinator](https://github.com/tmuxinator/tmuxinator), but without the project management feature
 which is in my opinion kind of an overhead.
 
@@ -120,7 +123,9 @@
 For ROS2, the same is achievable with `ros2 pkg prefix` but the yaml has to be installed (similar
 to, for example, a launch file) and the installation path has to be specified:
 ```
 catmux_create_session $(ros2 pkg prefix <your_package_name>)/path/to/the/installed/<your_catmux_session_config.yaml>
 
 # for example: $ catmux_create_session $(ros2 pkg prefix catmux_test_pkg)/share/catmux_test_pkg/catmux_session.yaml
 ```
+
+
```

### Comparing `catmux-0.3.2/README.md` & `catmux-0.3.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # Catmux
+[![codecov](https://codecov.io/gh/fmauch/catmux/branch/master/graph/badge.svg?token=bPcdYrOBRK)](https://codecov.io/gh/fmauch/catmux)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## About
 Catmux is a little helper to run a tmux session with multiple windows and panes with just one
 command. It is inspired and functionally very similar to
 [tmuxinator](https://github.com/tmuxinator/tmuxinator), but without the project management feature
 which is in my opinion kind of an overhead.
```

### Comparing `catmux-0.3.2/catmux/prefix.py` & `catmux-0.3.3/catmux/prefix.py`

 * *Files identical despite different names*

### Comparing `catmux-0.3.2/catmux/session.py` & `catmux-0.3.3/catmux/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 """Contains everything around the config file"""
 import re
 import yaml
 
 from catmux.window import Window
 import catmux.tmux_wrapper as tmux
+import catmux.exceptions as cme
 
 
 def check_boolean_field(boolean):
     if isinstance(boolean, bool):
         return boolean
     return boolean.lower() in ("yes", "true", "t", "1", True)
 
@@ -40,22 +41,24 @@
 class Session(object):
 
     """Parser for a config yaml file"""
 
     def __init__(self, server_name, session_name, runtime_params=None):
         """TODO: to be defined1."""
 
-        self._common = dict()
         self._server_name = server_name
         self._session_name = session_name
         self._parameters = dict()
         self._runtime_params = self._parse_overwrites(runtime_params)
         self._windows = list()
         self.__yaml_data = None
 
+        self._before_commands = list()
+        self._default_window = None
+
     def init_from_filepath(self, filepath):
         """Initializes the data from a file read from filepath."""
 
         try:
             self.__yaml_data = yaml.safe_load(open(filepath, "r"))
         except yaml.YAMLError as exc:
             print("Error while loading config file: %s", exc)
@@ -81,30 +84,35 @@
         for window in self._windows:
             window.create(first)
             if debug:
                 window.debug()
             first = False
 
         tmux_wrapper = tmux.TmuxWrapper(self._server_name)
-        if "default_window" in self._common:
+        if self._default_window:
             tmux_wrapper.tmux_call(
                 [
                     "select-window",
                     "-t",
-                    self._session_name + ":" + self._common["default_window"],
+                    self._session_name + ":" + self._default_window,
                 ]
             )
 
     def _parse_common(self):
         if self.__yaml_data is None:
             print("parse_common was called without yaml data loaded.")
             raise RuntimeError
 
         if "common" in self.__yaml_data:
-            self._common = self.__yaml_data["common"]
+            common = self.__yaml_data["common"]
+            if "before_commands" in common:
+                self._before_commands = common["before_commands"]
+
+            if "default_window" in common:
+                self._default_window = common["default_window"]
 
     def _parse_overwrites(self, data_string):
         """Separates a comma-separated list of foo=val1,bar=val2 into a dictionary."""
         if data_string is None:
             return None
 
         overwrites = dict()
@@ -164,60 +172,74 @@
             print("parse_windows was called without yaml data loaded.")
             raise RuntimeError
 
         if "windows" in self.__yaml_data:
             for window in self.__yaml_data["windows"]:
                 if "if" in window:
                     print("Detected if condition for window " + window["name"])
-                    if window["if"] not in self._parameters:
-                        print(
-                            "Skipping window "
-                            + window["name"]
-                            + " because parameter "
-                            + window["if"]
-                            + " was not found."
-                        )
-                        continue
-                    elif not check_boolean_field(self._parameters[window["if"]]):
-                        print(
-                            "Skipping window "
-                            + window["name"]
-                            + " because parameter "
-                            + window["if"]
-                            + " is switched off globally"
-                        )
-                        continue
-                    else:
-                        print(
-                            "condition fulfilled: {} == {}".format(
-                                window["if"], self._parameters[window["if"]]
+                    try:
+                        if_param = self._parameters[window["if"]]
+                        if window["if"] not in self._parameters:
+                            print(
+                                "Skipping window "
+                                + window["name"]
+                                + " because parameter "
+                                + window["if"]
+                                + " was not found."
+                            )
+                            continue
+                        elif not check_boolean_field(if_param):
+                            print(
+                                "Skipping window "
+                                + window["name"]
+                                + " because parameter "
+                                + window["if"]
+                                + " is switched off globally"
                             )
+                            continue
+                        else:
+                            print(
+                                "condition fulfilled: {} == {}".format(
+                                    window["if"], self._parameters[window["if"]]
+                                )
+                            )
+                    except KeyError:
+                        raise cme.InvalidConfig(
+                            f"Paramater '{window['if']}' not found in parameters."
                         )
                 if "unless" in window:
                     print("Detected unless condition for window " + window["name"])
-                    if check_boolean_field(self._parameters[window["unless"]]):
-                        print(
-                            "Skipping window "
-                            + window["name"]
-                            + " because parameter "
-                            + window["unless"]
-                            + " is switched on globally"
-                        )
-                        continue
-                    else:
-                        print(
-                            "condition fulfilled: {} == {}".format(
-                                window["unless"], self._parameters[window["unless"]]
+                    try:
+                        unless_param = self._parameters[window["unless"]]
+
+                        if check_boolean_field(unless_param):
+                            print(
+                                "Skipping window "
+                                + window["name"]
+                                + " because parameter "
+                                + window["unless"]
+                                + " is switched on globally"
                             )
+                            continue
+                        else:
+                            print(
+                                "condition fulfilled: {} == {}".format(
+                                    window["unless"], self._parameters[window["unless"]]
+                                )
+                            )
+                    except KeyError:
+                        raise cme.InvalidConfig(
+                            f"Paramater '{window['unless']}' not found in parameters."
                         )
 
                 kwargs = dict()
-                if "before_commands" in self._common:
-                    kwargs["before_commands"] = self._common["before_commands"]
+                kwargs["before_commands"] = [cmd for cmd in self._before_commands]
 
                 kwargs.update(window)
 
+                print(kwargs)
+
                 self._windows.append(
                     Window(self._server_name, self._session_name, **kwargs)
                 )
         else:
             print("No window section found in session config")
```

### Comparing `catmux-0.3.2/catmux/split.py` & `catmux-0.3.3/catmux/split.py`

 * *Files identical despite different names*

### Comparing `catmux-0.3.2/catmux/tmux_wrapper.py` & `catmux-0.3.3/catmux/tmux_wrapper.py`

 * *Files identical despite different names*

### Comparing `catmux-0.3.2/catmux/window.py` & `catmux-0.3.3/catmux/window.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,31 +24,39 @@
 # -- END LICENSE BLOCK ------------------------------------------------
 
 """Contains the Window object"""
 import time
 
 import catmux.tmux_wrapper as tmux
 from catmux.split import Split
+from catmux.exceptions import InvalidConfig
 
 
 class Window(object):
 
     """Class to represent a tmux window structure"""
 
     def __init__(self, server_name, session_name, **kwargs):
         """TODO: to be defined1."""
 
         self.server_name = server_name
         self.session_name = session_name
 
         split_list = kwargs.pop("splits", None)
-        if not split_list and "commands" in kwargs:
-            split_dict = dict()
-            split_dict["commands"] = kwargs.pop("commands")
-            split_list = [split_dict]
+        if not split_list:
+            if "commands" in kwargs:
+                split_dict = dict()
+                split_dict["commands"] = kwargs.pop("commands")
+                split_list = [split_dict]
+            else:
+                raise InvalidConfig(
+                    f"No splits and no commands given for window '{kwargs['name']}'."
+                )
+
+        print(split_list)
 
         self.splits = list()
         for split_data in split_list:
             self.splits.append(Split(**split_data))
 
         if kwargs is not None:
             for (key, value) in kwargs.items():
```

### Comparing `catmux-0.3.2/catmux.egg-info/PKG-INFO` & `catmux-0.3.3/catmux.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: catmux
-Version: 0.3.2
+Version: 0.3.3
 Summary: A tmux orchestration package.
 Home-page: https://github.com/fmauch/catmux
 Author: Felix Exner
 Author-email: felix_mauch@web.de
 License: MIT
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Catmux
+[![codecov](https://codecov.io/gh/fmauch/catmux/branch/master/graph/badge.svg?token=bPcdYrOBRK)](https://codecov.io/gh/fmauch/catmux)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## About
 Catmux is a little helper to run a tmux session with multiple windows and panes with just one
 command. It is inspired and functionally very similar to
 [tmuxinator](https://github.com/tmuxinator/tmuxinator), but without the project management feature
 which is in my opinion kind of an overhead.
 
@@ -120,7 +123,9 @@
 For ROS2, the same is achievable with `ros2 pkg prefix` but the yaml has to be installed (similar
 to, for example, a launch file) and the installation path has to be specified:
 ```
 catmux_create_session $(ros2 pkg prefix <your_package_name>)/path/to/the/installed/<your_catmux_session_config.yaml>
 
 # for example: $ catmux_create_session $(ros2 pkg prefix catmux_test_pkg)/share/catmux_test_pkg/catmux_session.yaml
 ```
+
+
```

### Comparing `catmux-0.3.2/etc/example_session.yaml` & `catmux-0.3.3/etc/example_session.yaml`

 * *Files identical despite different names*

### Comparing `catmux-0.3.2/etc/readme_tmux.txt` & `catmux-0.3.3/etc/readme_tmux.txt`

 * *Files identical despite different names*

### Comparing `catmux-0.3.2/etc/tmux_default.conf` & `catmux-0.3.3/etc/tmux_default.conf`

 * *Files identical despite different names*

### Comparing `catmux-0.3.2/script/catmux_create_session` & `catmux-0.3.3/script/catmux_create_session`

 * *Files 8% similar despite different names*

```diff
@@ -22,21 +22,23 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # -- END LICENSE BLOCK ------------------------------------------------
 
 from __future__ import print_function
 import os
+import logging
 import subprocess
 import sys
 
 import argparse
 
 from catmux.session import Session as CatmuxSession
 from catmux.prefix import get_prefix
+import catmux.exceptions
 
 
 def safe_call(cmd_list):
     """Makes a subprocess check_call and outputs a clear error message on failure and then exits"""
     try:
         subprocess.check_output(cmd_list)
         return True
@@ -81,15 +83,19 @@
     args = parse_arguments()
 
     session_config = CatmuxSession(
         server_name=args.server_name,
         session_name=args.session_name,
         runtime_params=args.overwrite,
     )
-    session_config.init_from_filepath(args.session_config)
+    try:
+        session_config.init_from_filepath(args.session_config)
+    except catmux.exceptions.InvalidConfig as err:
+        logging.error(err)
+        sys.exit(1)
 
     try:
         subprocess.check_call(
             ["tmux", "-L", args.server_name, "has-session", "-t", args.session_name]
         )
         print(
             'Session with name "{}" already exists. Not overwriting session.'.format(
```

### Comparing `catmux-0.3.2/setup.py` & `catmux-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="catmux",
-    version="0.3.2",
+    version="0.3.3",
     license="MIT",
     author="Felix Exner",
     author_email="felix_mauch@web.de",
     description="A tmux orchestration package.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fmauch/catmux",
```

