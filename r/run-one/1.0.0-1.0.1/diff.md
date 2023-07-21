# Comparing `tmp/run_one-1.0.0.tar.gz` & `tmp/run_one-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "run_one-1.0.0.tar", max compression
+gzip compressed data, was "run_one-1.0.1.tar", max compression
```

## Comparing `run_one-1.0.0.tar` & `run_one-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-07-21 00:58:44.845012 run_one-1.0.0/LICENSE
--rw-r--r--   0        0        0     1618 2023-07-21 00:58:44.845012 run_one-1.0.0/README.md
--rw-r--r--   0        0        0      741 2023-07-21 00:58:44.845012 run_one-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      345 2023-07-21 00:58:44.845012 run_one-1.0.0/run_one/__init__.py
--rw-r--r--   0        0        0      282 2023-07-21 00:58:44.845012 run_one-1.0.0/run_one/action_handlers/SleepHandler.py
--rw-r--r--   0        0        0     1877 2023-07-21 00:58:44.845012 run_one-1.0.0/run_one/action_handlers/TH2ActHandler.py
--rw-r--r--   0        0        0     1182 2023-07-21 00:58:44.845012 run_one-1.0.0/run_one/action_handlers/TH2ActSSHHandler.py
--rw-r--r--   0        0        0     3198 2023-07-21 00:58:44.845012 run_one-1.0.0/run_one/action_handlers/TH2Check1Handler.py
--rw-r--r--   0        0        0        0 2023-07-21 00:58:44.845012 run_one-1.0.0/run_one/action_handlers/__init__.py
--rw-r--r--   0        0        0      325 2023-07-21 00:58:44.845012 run_one-1.0.0/run_one/action_handlers/abstract_action_handler.py
--rw-r--r--   0        0        0      304 2023-07-21 00:58:44.845012 run_one-1.0.0/run_one/action_handlers/context.py
--rw-r--r--   0        0        0        0 2023-07-21 00:58:44.845012 run_one-1.0.0/run_one/processors/__init__.py
--rw-r--r--   0        0        0     1339 2023-07-21 00:58:44.845012 run_one-1.0.0/run_one/processors/abstract_processor.py
--rw-r--r--   0        0        0     4687 2023-07-21 00:58:44.845012 run_one-1.0.0/run_one/processors/th2_processor.py
--rw-r--r--   0        0        0        0 2023-07-21 00:58:44.845012 run_one-1.0.0/run_one/util/__init__.py
--rw-r--r--   0        0        0     1501 2023-07-21 00:58:44.845012 run_one-1.0.0/run_one/util/config.py
--rw-r--r--   0        0        0     3225 2023-07-21 00:58:44.845012 run_one-1.0.0/run_one/util/util.py
--rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 run_one-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-21 01:30:47.021902 run_one-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1618 2023-07-21 01:30:47.021902 run_one-1.0.1/README.md
+-rw-r--r--   0        0        0      741 2023-07-21 01:30:47.021902 run_one-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      345 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/__init__.py
+-rw-r--r--   0        0        0      282 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/action_handlers/SleepHandler.py
+-rw-r--r--   0        0        0     1877 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/action_handlers/TH2ActHandler.py
+-rw-r--r--   0        0        0     1182 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/action_handlers/TH2ActSSHHandler.py
+-rw-r--r--   0        0        0     3198 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/action_handlers/TH2Check1Handler.py
+-rw-r--r--   0        0        0        0 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/action_handlers/__init__.py
+-rw-r--r--   0        0        0      325 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/action_handlers/abstract_action_handler.py
+-rw-r--r--   0        0        0      304 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/action_handlers/context.py
+-rw-r--r--   0        0        0        0 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/processors/__init__.py
+-rw-r--r--   0        0        0     1339 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/processors/abstract_processor.py
+-rw-r--r--   0        0        0     4797 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/processors/th2_processor.py
+-rw-r--r--   0        0        0        0 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/util/__init__.py
+-rw-r--r--   0        0        0     1501 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/util/config.py
+-rw-r--r--   0        0        0     3225 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/util/util.py
+-rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 run_one-1.0.1/PKG-INFO
```

### Comparing `run_one-1.0.0/LICENSE` & `run_one-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `run_one-1.0.0/README.md` & `run_one-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `run_one-1.0.0/pyproject.toml` & `run_one-1.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "run-one"
-version = "1.0.0"
+version = "1.0.1"
 description = "Tool for parsing matrix files, extracting actions and processing them according to user defined logic"
 authors = ["TH2-devs <th2-devs@exactprosystems.com>"]
 readme = "README.md"
 license = "Apache License 2.0"
 homepage = "https://github.com/th2-net/run-one"
 repository = "https://github.com/th2-net/run-one"
 packages = [
```

### Comparing `run_one-1.0.0/run_one/action_handlers/TH2ActHandler.py` & `run_one-1.0.1/run_one/action_handlers/TH2ActHandler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.0/run_one/action_handlers/TH2ActSSHHandler.py` & `run_one-1.0.1/run_one/action_handlers/TH2ActSSHHandler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.0/run_one/action_handlers/TH2Check1Handler.py` & `run_one-1.0.1/run_one/action_handlers/TH2Check1Handler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.0/run_one/processors/abstract_processor.py` & `run_one-1.0.1/run_one/processors/abstract_processor.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.0/run_one/processors/th2_processor.py` & `run_one-1.0.1/run_one/processors/th2_processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,21 +84,23 @@
                 current_action_type = current_action.extra_data['Action']
 
                 self.logger.info(f'Processing {current_action_type} action '
                                  f'with ID = {current_action.extra_data.get("ID", "empty")}, '
                                  f'message type = {current_action.extra_data.get("MessageType", "none")},'
                                  f'description = {current_action.extra_data.get("Description", "empty")}')
 
-                action_handler = self.processed_actions.get(current_action_type)
-                if action_handler is not None:
-                    action_handler.process(action=current_action)
-
-                if previous_action is not None \
-                        and action_handler is not self.processed_actions.get(previous_action.extra_data['Action']):
-                    action_handler.on_action_change(previous_action, current_action)
+                current_action_handler = self.processed_actions.get(current_action_type)
+
+                if previous_action is not None:
+                    previous_action_handler = self.processed_actions.get(previous_action.extra_data['Action'])
+                    if current_action_handler is not previous_action_handler:
+                        previous_action_handler.on_action_change(previous_action, current_action)
+
+                if current_action_handler is not None:
+                    current_action_handler.process(action=current_action)
 
                 time.sleep(self._config.sleep)
 
             for handler in self.processed_actions.values():
                 handler.on_test_case_end()
 
             Context.clear()
```

### Comparing `run_one-1.0.0/run_one/util/config.py` & `run_one-1.0.1/run_one/util/config.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.0/run_one/util/util.py` & `run_one-1.0.1/run_one/util/util.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.0/PKG-INFO` & `run_one-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: run-one
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tool for parsing matrix files, extracting actions and processing them according to user defined logic
 Home-page: https://github.com/th2-net/run-one
 License: Apache-2.0
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

