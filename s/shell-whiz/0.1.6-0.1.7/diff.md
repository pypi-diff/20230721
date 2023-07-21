# Comparing `tmp/shell_whiz-0.1.6.tar.gz` & `tmp/shell_whiz-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_whiz-0.1.6.tar", max compression
+gzip compressed data, was "shell_whiz-0.1.7.tar", max compression
```

## Comparing `shell_whiz-0.1.6.tar` & `shell_whiz-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-07-11 19:23:06.329766 shell_whiz-0.1.6/LICENSE
--rw-r--r--   0        0        0     1067 2023-07-11 19:23:06.329766 shell_whiz-0.1.6/README.md
--rw-r--r--   0        0        0      515 2023-07-11 19:23:06.329766 shell_whiz-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3874 2023-07-11 19:23:06.329766 shell_whiz-0.1.6/shell_whiz/__init__.py
--rw-r--r--   0        0        0       58 2023-07-11 19:23:06.329766 shell_whiz-0.1.6/shell_whiz/__main__.py
--rw-r--r--   0        0        0     1530 2023-07-11 19:23:06.329766 shell_whiz-0.1.6/shell_whiz/config.py
--rw-r--r--   0        0        0      194 2023-07-11 19:23:06.329766 shell_whiz-0.1.6/shell_whiz/constants.py
--rw-r--r--   0        0        0      108 2023-07-11 19:23:06.329766 shell_whiz-0.1.6/shell_whiz/exceptions.py
--rw-r--r--   0        0        0     7282 2023-07-11 19:23:06.329766 shell_whiz-0.1.6/shell_whiz/openai.py
--rw-r--r--   0        0        0     1624 1970-01-01 00:00:00.000000 shell_whiz-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-21 06:25:51.302699 shell_whiz-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1130 2023-07-21 06:25:51.302699 shell_whiz-0.1.7/README.md
+-rw-r--r--   0        0        0      515 2023-07-21 06:25:51.306699 shell_whiz-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3874 2023-07-21 06:25:51.306699 shell_whiz-0.1.7/shell_whiz/__init__.py
+-rw-r--r--   0        0        0       58 2023-07-21 06:25:51.306699 shell_whiz-0.1.7/shell_whiz/__main__.py
+-rw-r--r--   0        0        0     1686 2023-07-21 06:25:51.306699 shell_whiz-0.1.7/shell_whiz/config.py
+-rw-r--r--   0        0        0      194 2023-07-21 06:25:51.306699 shell_whiz-0.1.7/shell_whiz/constants.py
+-rw-r--r--   0        0        0      108 2023-07-21 06:25:51.306699 shell_whiz-0.1.7/shell_whiz/exceptions.py
+-rw-r--r--   0        0        0     7282 2023-07-21 06:25:51.306699 shell_whiz-0.1.7/shell_whiz/openai.py
+-rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 shell_whiz-0.1.7/PKG-INFO
```

### Comparing `shell_whiz-0.1.6/LICENSE` & `shell_whiz-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.6/README.md` & `shell_whiz-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ![PyPI](https://img.shields.io/pypi/v/shell-whiz)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/shell-whiz)
 ![GitHub stars](https://img.shields.io/github/stars/beimzhan/shell-whiz)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/beimzhan/shell-whiz)
 ![GitHub license](https://img.shields.io/github/license/beimzhan/shell-whiz)
 
 # Shell Whiz: AI assistant right in your terminal
 Shell Whiz will help you generate shell commands from your natural language queries. It is powered by OpenAI's `gpt-3.5-turbo` and is free to use.
```

### Comparing `shell_whiz-0.1.6/pyproject.toml` & `shell_whiz-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shell-whiz"
-version = "0.1.6"
+version = "0.1.7"
 description = "Shell Whiz: AI assistant right in your terminal"
 authors = ["Tamerlan Bimzhanov <bimzhanovt.net@gmail.com>"]
 readme = "README.md"
 packages = [{include = "shell_whiz"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `shell_whiz-0.1.6/shell_whiz/__init__.py` & `shell_whiz-0.1.7/shell_whiz/__init__.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.6/shell_whiz/config.py` & `shell_whiz-0.1.7/shell_whiz/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,20 @@
 import openai
 from inquirer.themes import GreenPassion
 
 
 def shell_whiz_config_file():
     if "XDG_CONFIG_HOME" in os.environ:
         config_dir = os.environ["XDG_CONFIG_HOME"]
-    else:
+    elif "APPDATA" in os.environ:  # for Windows
+        config_dir = os.environ["APPDATA"]
+    elif "HOME" in os.environ:
         config_dir = os.path.join(os.environ["HOME"], ".config")
+    else:
+        config_dir = os.getcwd()
 
     sw_config_dir = os.path.join(config_dir, "shell-whiz")
     sw_config_file = os.path.join(sw_config_dir, "config.json")
 
     return sw_config_dir, sw_config_file
```

### Comparing `shell_whiz-0.1.6/shell_whiz/openai.py` & `shell_whiz-0.1.7/shell_whiz/openai.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.6/PKG-INFO` & `shell_whiz-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: shell-whiz
-Version: 0.1.6
+Version: 0.1.7
 Summary: Shell Whiz: AI assistant right in your terminal
 Author: Tamerlan Bimzhanov
 Author-email: bimzhanovt.net@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: inquirer (>=3.1.3,<4.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: prompt-toolkit (>=3.0.39,<4.0.0)
 Requires-Dist: yaspin (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 ![PyPI](https://img.shields.io/pypi/v/shell-whiz)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/shell-whiz)
 ![GitHub stars](https://img.shields.io/github/stars/beimzhan/shell-whiz)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/beimzhan/shell-whiz)
 ![GitHub license](https://img.shields.io/github/license/beimzhan/shell-whiz)
 
 # Shell Whiz: AI assistant right in your terminal
 Shell Whiz will help you generate shell commands from your natural language queries. It is powered by OpenAI's `gpt-3.5-turbo` and is free to use.
```

