# Comparing `tmp/py-tldr-0.8.1.tar.gz` & `tmp/py-tldr-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-tldr-0.8.1.tar", last modified: Thu Jul 20 20:26:08 2023, max compression
+gzip compressed data, was "py-tldr-0.9.0.tar", last modified: Fri Jul 21 19:37:02 2023, max compression
```

## Comparing `py-tldr-0.8.1.tar` & `py-tldr-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:08.287676 py-tldr-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 20:25:57.000000 py-tldr-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-20 20:26:08.287676 py-tldr-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-20 20:25:57.000000 py-tldr-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-20 20:25:57.000000 py-tldr-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 20:26:08.287676 py-tldr-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:08.283676 py-tldr-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:08.287676 py-tldr-0.8.1/src/py_tldr/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-20 20:25:57.000000 py-tldr-0.8.1/src/py_tldr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-20 20:25:57.000000 py-tldr-0.8.1/src/py_tldr/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-07-20 20:25:57.000000 py-tldr-0.8.1/src/py_tldr/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-20 20:25:57.000000 py-tldr-0.8.1/src/py_tldr/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:08.287676 py-tldr-0.8.1/src/py_tldr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-20 20:26:08.000000 py-tldr-0.8.1/src/py_tldr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-20 20:26:08.000000 py-tldr-0.8.1/src/py_tldr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:26:08.000000 py-tldr-0.8.1/src/py_tldr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 20:26:08.000000 py-tldr-0.8.1/src/py_tldr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-20 20:26:08.000000 py-tldr-0.8.1/src/py_tldr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 20:26:08.000000 py-tldr-0.8.1/src/py_tldr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:08.287676 py-tldr-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-20 20:25:57.000000 py-tldr-0.8.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:37:02.940820 py-tldr-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 19:36:53.000000 py-tldr-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-21 19:37:02.940820 py-tldr-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-21 19:36:53.000000 py-tldr-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-21 19:36:53.000000 py-tldr-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 19:37:02.940820 py-tldr-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:37:02.936820 py-tldr-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:37:02.936820 py-tldr-0.9.0/src/py_tldr/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-21 19:36:53.000000 py-tldr-0.9.0/src/py_tldr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-07-21 19:36:53.000000 py-tldr-0.9.0/src/py_tldr/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-07-21 19:36:53.000000 py-tldr-0.9.0/src/py_tldr/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-21 19:36:53.000000 py-tldr-0.9.0/src/py_tldr/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:37:02.940820 py-tldr-0.9.0/src/py_tldr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-21 19:37:02.000000 py-tldr-0.9.0/src/py_tldr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-21 19:37:02.000000 py-tldr-0.9.0/src/py_tldr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:37:02.000000 py-tldr-0.9.0/src/py_tldr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 19:37:02.000000 py-tldr-0.9.0/src/py_tldr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-21 19:37:02.000000 py-tldr-0.9.0/src/py_tldr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 19:37:02.000000 py-tldr-0.9.0/src/py_tldr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:37:02.940820 py-tldr-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-21 19:36:53.000000 py-tldr-0.9.0/tests/test_cli.py
```

### Comparing `py-tldr-0.8.1/PKG-INFO` & `py-tldr-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-tldr
-Version: 0.8.1
+Version: 0.9.0
 Summary: New Python client for tldr pages
 Author-email: iamgodot <xugodot@gmail.com>
 License: MIT
 Project-URL: Issue Tracker, https://github.com/iamgodot/py-tldr/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -68,15 +68,15 @@
 
 Cache is enabled implicitly, with 24 hours as expiration time by default.
 
 A proxy url can be set for convenience, proxy envs such as `HTTP_PROXY` will also work.
 
 ## Support
 
-Python: 3.7, 3.8, 3.9
+Python: >=3.7
 
 OS: Not tested on Windows.
 
 ## Changelog
 
 See [CHANGELOG](docs/CHANGELOG.md)
```

### Comparing `py-tldr-0.8.1/README.md` & `py-tldr-0.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 Cache is enabled implicitly, with 24 hours as expiration time by default.
 
 A proxy url can be set for convenience, proxy envs such as `HTTP_PROXY` will also work.
 
 ## Support
 
-Python: 3.7, 3.8, 3.9
+Python: >=3.7
 
 OS: Not tested on Windows.
 
 ## Changelog
 
 See [CHANGELOG](docs/CHANGELOG.md)
```

### Comparing `py-tldr-0.8.1/pyproject.toml` & `py-tldr-0.9.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -64,32 +64,7 @@
 exclude = [".git", ".tox", "venv", "build", "__pypackages__"]
 line-length = 88
 per-file-ignores = {"src/py_tldr/__init__.py" = ["F401"]}
 src = ["src", "tests"]
 
 [tool.ruff.isort]
 known-first-party = ["py_tldr"]
-
-[tool.tbump]
-github_url = "https://github.com/iamgodot/py-tldr"
-
-[tool.tbump.version]
-current = "0.7.0"
-
-regex = '''
-  (?P<major>\d+)
-  \.
-  (?P<minor>\d+)
-  \.
-  (?P<patch>\d+)
-  '''
-
-[tool.tbump.git]
-message_template = "build: bump version to v{new_version}"
-tag_template = "v{new_version}"
-
-[[tool.tbump.file]]
-src = "src/py_tldr/__init__.py"
-
-[[tool.tbump.before_commit]]
-name = "Check changelog"
-cmd = "grep -q {new_version} docs/CHANGELOG.md"
```

### Comparing `py-tldr-0.8.1/src/py_tldr/__init__.py` & `py-tldr-0.9.0/src/py_tldr/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from logging.config import dictConfig
 from os import environ
 
 from .core import cli
 from .page import PageCache, PageFinder, PageFormatter
 
-__version__ = "0.8.1"
+__version__ = "0.9.0"
 
 
 logging_config = {
     "version": 1,
     "formatters": {
         "default": {
             "format": "[%(asctime)s] %(levelname)s in func `%(funcName)s` by logger `%(name)s`: %(message)s",  # NOQA
```

### Comparing `py-tldr-0.8.1/src/py_tldr/core.py` & `py-tldr-0.9.0/src/py_tldr/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 from copy import deepcopy
 from functools import partial
 from os import environ
 from pathlib import Path as LibPath
 
 import toml
-from click import Choice, argument, option, pass_context, secho
+from click import argument, option, pass_context, secho
 from click import command as command_
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 
 from py_tldr.page import DownloadError, PageFinder, PageFormatter
 from py_tldr.parse import parse_command, parse_language, parse_platform
 
@@ -112,21 +112,22 @@
     is_eager=True,
     expose_value=False,
     help="Open config file with an editor.",
 )
 @option(
     "-p",
     "--platform",
-    type=Choice(["android", "linux", "macos", "osx", "sunos", "windows"]),
-    default="linux",
-    help="Specify searching platform(macos as an alias of osx).",
+    type=str,
+    default="",
+    help="Possible values: android, linux, osx(macos), sunos, windows.",
 )
 @option(
     "-L",
     "--language",
+    type=str,
     default="en",
     help="Specify searching language(with no fallbacks), e.g. `en`.",
 )
 @option("-u", "--update", is_flag=True, help="Update local cache with all pages.")
 @argument("command", nargs=-1)
 @pass_context
 def cli(ctx, command, platform, language, update):
```

### Comparing `py-tldr-0.8.1/src/py_tldr/page.py` & `py-tldr-0.9.0/src/py_tldr/page.py`

 * *Files identical despite different names*

### Comparing `py-tldr-0.8.1/src/py_tldr/parse.py` & `py-tldr-0.9.0/src/py_tldr/parse.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         languages.append(lang)
     if "en" not in languages:
         languages.append("en")
     return [language.lower() for language in languages]
 
 
 def parse_platform(platform: str, config: Dict) -> str:
+    if platform.lower() not in ["android", "linux", "osx", "macos", "sunos", "windows"]:
+        platform = ""
     platform = platform or config.get("platform", "")
     if platform:
         platform = platform.lower()
     else:
         platform = guess_os()
     return "osx" if platform == "macos" else platform
```

### Comparing `py-tldr-0.8.1/src/py_tldr.egg-info/PKG-INFO` & `py-tldr-0.9.0/src/py_tldr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-tldr
-Version: 0.8.1
+Version: 0.9.0
 Summary: New Python client for tldr pages
 Author-email: iamgodot <xugodot@gmail.com>
 License: MIT
 Project-URL: Issue Tracker, https://github.com/iamgodot/py-tldr/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -68,15 +68,15 @@
 
 Cache is enabled implicitly, with 24 hours as expiration time by default.
 
 A proxy url can be set for convenience, proxy envs such as `HTTP_PROXY` will also work.
 
 ## Support
 
-Python: 3.7, 3.8, 3.9
+Python: >=3.7
 
 OS: Not tested on Windows.
 
 ## Changelog
 
 See [CHANGELOG](docs/CHANGELOG.md)
```

### Comparing `py-tldr-0.8.1/tests/test_cli.py` & `py-tldr-0.9.0/tests/test_cli.py`

 * *Files identical despite different names*

