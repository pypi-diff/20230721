# Comparing `tmp/wizlib-0.7.0.tar.gz` & `tmp/wizlib-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizlib-0.7.0.tar", last modified: Thu Jul 20 05:15:05 2023, max compression
+gzip compressed data, was "wizlib-0.7.1.tar", last modified: Fri Jul 21 04:48:40 2023, max compression
```

## Comparing `wizlib-0.7.0.tar` & `wizlib-0.7.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 05:15:05.058683 wizlib-0.7.0/
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-20 05:14:16.000000 wizlib-0.7.0/.version
--rw-r--r--   0 root         (0) root         (0)     3988 2023-07-20 05:15:05.058683 wizlib-0.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3723 2023-07-20 05:14:56.000000 wizlib-0.7.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-07-20 05:14:56.000000 wizlib-0.7.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 05:15:05.058683 wizlib-0.7.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 05:15:05.055683 wizlib-0.7.0/test/
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-20 05:14:56.000000 wizlib-0.7.0/test/test_class_family.py
--rw-rw-rw-   0 root         (0) root         (0)     1793 2023-07-20 05:14:56.000000 wizlib-0.7.0/test/test_config_machine.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-07-20 05:14:56.000000 wizlib-0.7.0/test/test_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2023-07-20 05:14:56.000000 wizlib-0.7.0/test/test_super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 05:15:05.057683 wizlib-0.7.0/wizlib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 05:14:56.000000 wizlib-0.7.0/wizlib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4413 2023-07-20 05:14:56.000000 wizlib-0.7.0/wizlib/class_family.py
--rw-rw-rw-   0 root         (0) root         (0)     2168 2023-07-20 05:14:56.000000 wizlib-0.7.0/wizlib/command_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-07-20 05:14:56.000000 wizlib-0.7.0/wizlib/config_machine.py
--rw-rw-rw-   0 root         (0) root         (0)     1754 2023-07-20 05:14:56.000000 wizlib-0.7.0/wizlib/rlinput.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-07-20 05:14:56.000000 wizlib-0.7.0/wizlib/super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 05:15:05.058683 wizlib-0.7.0/wizlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3988 2023-07-20 05:15:05.000000 wizlib-0.7.0/wizlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2023-07-20 05:15:05.000000 wizlib-0.7.0/wizlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 05:15:05.000000 wizlib-0.7.0/wizlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-20 05:15:05.000000 wizlib-0.7.0/wizlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-20 05:15:05.000000 wizlib-0.7.0/wizlib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:48:40.650342 wizlib-0.7.1/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-21 04:47:50.000000 wizlib-0.7.1/.version
+-rw-r--r--   0 root         (0) root         (0)     5115 2023-07-21 04:48:40.650342 wizlib-0.7.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4850 2023-07-21 04:48:32.000000 wizlib-0.7.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-07-21 04:48:32.000000 wizlib-0.7.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 04:48:40.651342 wizlib-0.7.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:48:40.648342 wizlib-0.7.1/test/
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-21 04:48:32.000000 wizlib-0.7.1/test/test_class_family.py
+-rw-rw-rw-   0 root         (0) root         (0)     2366 2023-07-21 04:48:32.000000 wizlib-0.7.1/test/test_config_machine.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-07-21 04:48:32.000000 wizlib-0.7.1/test/test_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-07-21 04:48:32.000000 wizlib-0.7.1/test/test_super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:48:40.649342 wizlib-0.7.1/wizlib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-21 04:48:32.000000 wizlib-0.7.1/wizlib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4413 2023-07-21 04:48:32.000000 wizlib-0.7.1/wizlib/class_family.py
+-rw-rw-rw-   0 root         (0) root         (0)     2168 2023-07-21 04:48:32.000000 wizlib-0.7.1/wizlib/command_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1601 2023-07-21 04:48:32.000000 wizlib-0.7.1/wizlib/config_machine.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2023-07-21 04:48:32.000000 wizlib-0.7.1/wizlib/rlinput.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-07-21 04:48:32.000000 wizlib-0.7.1/wizlib/super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:48:40.650342 wizlib-0.7.1/wizlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5115 2023-07-21 04:48:40.000000 wizlib-0.7.1/wizlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-21 04:48:40.000000 wizlib-0.7.1/wizlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 04:48:40.000000 wizlib-0.7.1/wizlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-21 04:48:40.000000 wizlib-0.7.1/wizlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-21 04:48:40.000000 wizlib-0.7.1/wizlib.egg-info/top_level.txt
```

### Comparing `wizlib-0.7.0/PKG-INFO` & `wizlib-0.7.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: wizlib
-Version: 0.7.0
-Summary: A collection of Python modules that are useful across multiple projects
-Author-email: Francis Potter <wizlib@steampunkwizard.ca>
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # WizLib
 
 A collection of Python modules that might be useful across multiple projects
 
 ## ClassFamily
 
 A class family is a set of class definitions that use single inheritance
@@ -69,14 +60,46 @@
 
 c = NewChild()
 c.execute("Jane")
 ```
 
 ## CommandHandler
 
+## ConfigMachine
+
+Enables easy configuration across multiple levels. Tries each of the following approaches in order until one finds the required config option
+
+- First look for specific options (ie. `--gitlab-host`) on the command line, typically hyphenated
+- Then look for a specific env variable for that config setting in all caps, e.g. `GITLAB_HOST`
+- If those both fail, then look for a YAML configuration file:
+    - First identified with a `--config` / `-c` option on the command line
+    - Then with a path in the `APPNAME_CONFIG` environment variable - note all caps
+    - Then look in the local working directory for `.appname.yml`
+    - Then look for `~/.appname.yml` in the user's home directory
+
+Config files are in YAML, and look something like this:
+
+```yaml
+gitlab:
+  host: gitlab.com
+local:
+  root: $HOME/git
+```
+
+Note that nested labels in the config map to hyphenated command line options.
+
+To use the library:
+
+```python
+config = ConfigMachine('appname', args)
+host = config.get('gitlab-host')
+```
+
+This assumes that `args` represents the result of `ArgumentParser` - in otherwords, a `Namespace` object.
+
 ## RLInput
 
 Python supports the GNU readline approach, which enables tab completion, key mappings, and history with the `input()` function. But the documentation is cryptic, and the implementation differs between Linux and MacOS. RLInput makes it easy.
 
 ```python
 from wizlib.rlinput import rlinput
 ```
```

### Comparing `wizlib-0.7.0/pyproject.toml` & `wizlib-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wizlib-0.7.0/test/test_config_machine.py` & `wizlib-0.7.1/test/test_config_machine.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from unittest import TestCase
 from argparse import ArgumentParser
 import os
+from unittest.mock import patch
+from pathlib import Path
 
 from wizlib.config_machine import ConfigMachine
 
 
 class TestConfig(TestCase):
 
     def test_direct_arg(self):
@@ -51,7 +53,21 @@
 
     def test_specific_env_var(self):
         os.environ['MYAPP_CONFIG'] = 'test/data_config_machine/test-config.yml'
         config = ConfigMachine('myapp')
         f = config.get('bar-zing')
         del os.environ['MYAPP_CONFIG']
         self.assertEqual(f, 'ech')
+
+    def test_local_config_file(self):
+        with patch('pathlib.Path.cwd',
+                   lambda: Path('test/data_config_machine')):
+            config = ConfigMachine('myapp')
+            f = config.get('bar-zing')
+        self.assertEqual(f, 'ech')
+
+    def test_home_config_file(self):
+        with patch('pathlib.Path.home',
+                   lambda: Path('test/data_config_machine')):
+            config = ConfigMachine('myapp')
+            f = config.get('bar-zing')
+        self.assertEqual(f, 'ech')
```

### Comparing `wizlib-0.7.0/test/test_super_wrapper.py` & `wizlib-0.7.1/test/test_super_wrapper.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.7.0/wizlib/class_family.py` & `wizlib-0.7.1/wizlib/class_family.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.7.0/wizlib/command_handler.py` & `wizlib-0.7.1/wizlib/command_handler.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.7.0/wizlib/config_machine.py` & `wizlib-0.7.1/wizlib/config_machine.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,21 +20,24 @@
     args: Namespace = None
 
     @property
     def yaml(self):
         if hasattr(self, '_yaml'):
             return self._yaml
         if hasattr(self.args, 'config'):
-            pathstr = self.args.config
+            path = Path(self.args.config)
         elif (envvar := self.env(self.appname + '-config')):
-            pathstr = envvar
+            path = Path(envvar)
+        elif ((localpath := Path.cwd() / f".{self.appname}.yml").is_file()):
+            path = localpath
+        elif ((homepath := Path.home() / f".{self.appname}.yml").is_file()):
+            path = homepath
         else:
-            pathstr = None
-        if pathstr:
-            path = Path(pathstr)
+            path = None
+        if path:
             with open(path) as file:
                 self._yaml = load(file, Loader=Loader)
                 return self._yaml
 
     @staticmethod
     def env(name):
         if (envvar := name.upper().replace('-', '_')) in os.environ:
```

### Comparing `wizlib-0.7.0/wizlib/rlinput.py` & `wizlib-0.7.1/wizlib/rlinput.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.7.0/wizlib.egg-info/PKG-INFO` & `wizlib-0.7.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 0.7.0
+Version: 0.7.1
 Summary: A collection of Python modules that are useful across multiple projects
 Author-email: Francis Potter <wizlib@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WizLib
@@ -69,14 +69,46 @@
 
 c = NewChild()
 c.execute("Jane")
 ```
 
 ## CommandHandler
 
+## ConfigMachine
+
+Enables easy configuration across multiple levels. Tries each of the following approaches in order until one finds the required config option
+
+- First look for specific options (ie. `--gitlab-host`) on the command line, typically hyphenated
+- Then look for a specific env variable for that config setting in all caps, e.g. `GITLAB_HOST`
+- If those both fail, then look for a YAML configuration file:
+    - First identified with a `--config` / `-c` option on the command line
+    - Then with a path in the `APPNAME_CONFIG` environment variable - note all caps
+    - Then look in the local working directory for `.appname.yml`
+    - Then look for `~/.appname.yml` in the user's home directory
+
+Config files are in YAML, and look something like this:
+
+```yaml
+gitlab:
+  host: gitlab.com
+local:
+  root: $HOME/git
+```
+
+Note that nested labels in the config map to hyphenated command line options.
+
+To use the library:
+
+```python
+config = ConfigMachine('appname', args)
+host = config.get('gitlab-host')
+```
+
+This assumes that `args` represents the result of `ArgumentParser` - in otherwords, a `Namespace` object.
+
 ## RLInput
 
 Python supports the GNU readline approach, which enables tab completion, key mappings, and history with the `input()` function. But the documentation is cryptic, and the implementation differs between Linux and MacOS. RLInput makes it easy.
 
 ```python
 from wizlib.rlinput import rlinput
 ```
```

