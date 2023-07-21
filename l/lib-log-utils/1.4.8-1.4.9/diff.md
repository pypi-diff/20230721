# Comparing `tmp/lib_log_utils-1.4.8.tar.gz` & `tmp/lib_log_utils-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lib_log_utils-1.4.8.tar", last modified: Sat Aug  1 19:55:51 2020, max compression
+gzip compressed data, was "dist/lib_log_utils-1.4.9.tar", last modified: Sat Aug  8 13:46:16 2020, max compression
```

## Comparing `lib_log_utils-1.4.8.tar` & `lib_log_utils-1.4.9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-01 19:55:51.047504 lib_log_utils-1.4.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1778 2020-08-01 19:54:57.000000 lib_log_utils-1.4.8/CHANGES.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      124 2020-08-01 19:54:57.000000 lib_log_utils-1.4.8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    18463 2020-08-01 19:55:51.047504 lib_log_utils-1.4.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    14106 2020-08-01 19:55:50.000000 lib_log_utils-1.4.8/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-01 19:55:51.047504 lib_log_utils-1.4.8/lib_log_utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)      407 2020-08-01 19:54:57.000000 lib_log_utils-1.4.8/lib_log_utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      530 2020-08-01 19:54:57.000000 lib_log_utils-1.4.8/lib_log_utils/__init__conf__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15754 2020-08-01 19:54:57.000000 lib_log_utils-1.4.8/lib_log_utils/lib_log_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15875 2020-08-01 19:54:57.000000 lib_log_utils-1.4.8/lib_log_utils/lib_log_utils_cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7929 2020-08-01 19:54:57.000000 lib_log_utils-1.4.8/lib_log_utils/log_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12404 2020-08-01 19:54:57.000000 lib_log_utils-1.4.8/lib_log_utils/log_handlers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1770 2020-08-01 19:54:57.000000 lib_log_utils-1.4.8/lib_log_utils/log_levels.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6602 2020-08-01 19:54:57.000000 lib_log_utils-1.4.8/lib_log_utils/log_traceback.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-08-01 19:54:57.000000 lib_log_utils-1.4.8/lib_log_utils/py.typed
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-01 19:55:51.047504 lib_log_utils-1.4.8/lib_log_utils.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18463 2020-08-01 19:55:50.000000 lib_log_utils-1.4.8/lib_log_utils.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      577 2020-08-01 19:55:50.000000 lib_log_utils-1.4.8/lib_log_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-08-01 19:55:50.000000 lib_log_utils-1.4.8/lib_log_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       71 2020-08-01 19:55:50.000000 lib_log_utils-1.4.8/lib_log_utils.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-08-01 19:55:21.000000 lib_log_utils-1.4.8/lib_log_utils.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       85 2020-08-01 19:55:50.000000 lib_log_utils-1.4.8/lib_log_utils.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2020-08-01 19:55:50.000000 lib_log_utils-1.4.8/lib_log_utils.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      120 2020-08-01 19:55:51.051504 lib_log_utils-1.4.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     4254 2020-08-01 19:54:57.000000 lib_log_utils-1.4.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-08 13:46:16.000000 lib_log_utils-1.4.9/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-08 13:46:16.000000 lib_log_utils-1.4.9/lib_log_utils.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       85 2020-08-08 13:46:16.000000 lib_log_utils-1.4.9/lib_log_utils.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2020-08-08 13:46:16.000000 lib_log_utils-1.4.9/lib_log_utils.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-08-08 13:46:15.000000 lib_log_utils-1.4.9/lib_log_utils.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      592 2020-08-08 13:46:16.000000 lib_log_utils-1.4.9/lib_log_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-08-08 13:46:16.000000 lib_log_utils-1.4.9/lib_log_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       71 2020-08-08 13:46:16.000000 lib_log_utils-1.4.9/lib_log_utils.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17847 2020-08-08 13:46:16.000000 lib_log_utils-1.4.9/lib_log_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      592 2020-08-08 13:46:16.000000 lib_log_utils-1.4.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13570 2020-08-08 13:45:42.000000 lib_log_utils-1.4.9/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-08 13:46:16.000000 lib_log_utils-1.4.9/lib_log_utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      407 2020-08-08 13:45:42.000000 lib_log_utils-1.4.9/lib_log_utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6522 2020-08-08 13:45:42.000000 lib_log_utils-1.4.9/lib_log_utils/log_traceback.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7929 2020-08-08 13:45:42.000000 lib_log_utils-1.4.9/lib_log_utils/log_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-08-08 13:45:42.000000 lib_log_utils-1.4.9/lib_log_utils/py.typed
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12404 2020-08-08 13:45:42.000000 lib_log_utils-1.4.9/lib_log_utils/log_handlers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15754 2020-08-08 13:45:42.000000 lib_log_utils-1.4.9/lib_log_utils/lib_log_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1770 2020-08-08 13:45:42.000000 lib_log_utils-1.4.9/lib_log_utils/log_levels.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15875 2020-08-08 13:45:42.000000 lib_log_utils-1.4.9/lib_log_utils/lib_log_utils_cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      530 2020-08-08 13:45:42.000000 lib_log_utils-1.4.9/lib_log_utils/__init__conf__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4218 2020-08-08 13:45:42.000000 lib_log_utils-1.4.9/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      252 2020-08-08 13:45:42.000000 lib_log_utils-1.4.9/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      124 2020-08-08 13:45:42.000000 lib_log_utils-1.4.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1915 2020-08-08 13:45:42.000000 lib_log_utils-1.4.9/CHANGES.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17847 2020-08-08 13:46:16.000000 lib_log_utils-1.4.9/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `lib_log_utils-1.4.8/CHANGES.rst` & `lib_log_utils-1.4.9/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.4.9
+--------
+2020-08-08: service release
+    - fix documentation
+    - fix travis
+    - deprecate pycodestyle
+    - implement flake8
+
 v1.4.8
 ---------
 2020-08-01: fix doctests in windows
 
 v1.4.7
 ---------
 2020-08-01: fix pypi deploy
```

### Comparing `lib_log_utils-1.4.8/PKG-INFO` & `lib_log_utils-1.4.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: lib_log_utils
-Version: 1.4.8
+Version: 1.4.9
 Summary: colored log messages and banners from commandline and python
 Home-page: https://github.com/bitranox/lib_log_utils
 Author: Robert Nowotny
 Author-email: bitranox@gmail.com
 License: UNKNOWN
 Description: lib_log_utils
         =============
         
         
-        Version v1.4.8 as of 2020-08-01 see `Changelog`_
+        Version v1.4.9 as of 2020-08-08 see `Changelog`_
         
         |travis_build| |license| |jupyter| |pypi|
         
         |codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
         
         
         .. |travis_build| image:: https://img.shields.io/travis/bitranox/lib_log_utils/master.svg
@@ -62,15 +62,15 @@
         automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
         .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
         
         Python version required: 3.6.0 or newer
         
         tested on linux "bionic" with python 3.6, 3.7, 3.8, 3.8-dev, pypy3 - architectures: amd64, ppc64le, s390x, arm64
         
-        `good code coverage <https://codecov.io/gh/bitranox/lib_log_utils>`_, codestyle checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://travis-ci.org/bitranox/lib_log_utils>`_, automatic daily builds and monitoring
+        `good code coverage <https://codecov.io/gh/bitranox/lib_log_utils>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://travis-ci.org/bitranox/lib_log_utils>`_, automatic daily builds and monitoring
         
         ----
         
         - `Try it Online`_
         - `Usage`_
         - `Usage from Commandline`_
         - `Installation and Upgrade`_
@@ -252,40 +252,28 @@
         - Before You start, its highly recommended to update pip and setup tools:
         
         
         .. code-block:: bash
         
             python -m pip --upgrade pip
             python -m pip --upgrade setuptools
-            python -m pip --upgrade wheel
         
         - to install the latest release from PyPi via pip (recommended):
         
         .. code-block:: bash
         
-            # install latest release from PyPi
             python -m pip install --upgrade lib_log_utils
         
-            # test latest release from PyPi without installing (can be skipped)
-            python -m pip install lib_log_utils --install-option test
-        
-        - to install the latest development version from github via pip:
+        - to install the latest version from github via pip:
         
         
         .. code-block:: bash
         
-            # normal install
             python -m pip install --upgrade git+https://github.com/bitranox/lib_log_utils.git
         
-            # to test without installing (can be skipped)
-            python -m pip install git+https://github.com/bitranox/lib_log_utils.git --install-option test
-        
-            # to install and upgrade all dependencies regardless of version number
-            python -m pip install --upgrade git+https://github.com/bitranox/lib_log_utils.git --upgrade-strategy eager
-        
         
         - include it into Your requirements.txt:
         
         .. code-block:: bash
         
             # Insert following line in Your requirements.txt:
             # for the latest Release on pypi:
@@ -294,27 +282,21 @@
             # for the latest development version :
             lib_log_utils @ git+https://github.com/bitranox/lib_log_utils.git
         
             # to install and upgrade all modules mentioned in requirements.txt:
             python -m pip install --upgrade -r /<path>/requirements.txt
         
         
-        
         - to install the latest development version from source code:
         
         .. code-block:: bash
         
             # cd ~
             $ git clone https://github.com/bitranox/lib_log_utils.git
             $ cd lib_log_utils
-        
-            # to test without installing (can be skipped)
-            python setup.py test
-        
-            # normal install
             python setup.py install
         
         - via makefile:
           makefiles are a very convenient way to install. Here we can do much more,
           like installing virtual environments, clean caches and so on.
         
         .. code-block:: shell
@@ -370,14 +352,22 @@
         Changelog
         =========
         
         - new MAJOR version for incompatible API changes,
         - new MINOR version for added functionality in a backwards compatible manner
         - new PATCH version for backwards compatible bug fixes
         
+        v1.4.9
+        --------
+        2020-08-08: service release
+            - fix documentation
+            - fix travis
+            - deprecate pycodestyle
+            - implement flake8
+        
         v1.4.8
         ---------
         2020-08-01: fix doctests in windows
         
         v1.4.7
         ---------
         2020-08-01: fix pypi deploy
```

### Comparing `lib_log_utils-1.4.8/README.rst` & `lib_log_utils-1.4.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lib_log_utils
 =============
 
 
-Version v1.4.8 as of 2020-08-01 see `Changelog`_
+Version v1.4.9 as of 2020-08-08 see `Changelog`_
 
 |travis_build| |license| |jupyter| |pypi|
 
 |codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 .. |travis_build| image:: https://img.shields.io/travis/bitranox/lib_log_utils/master.svg
@@ -54,15 +54,15 @@
 automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.6.0 or newer
 
 tested on linux "bionic" with python 3.6, 3.7, 3.8, 3.8-dev, pypy3 - architectures: amd64, ppc64le, s390x, arm64
 
-`good code coverage <https://codecov.io/gh/bitranox/lib_log_utils>`_, codestyle checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://travis-ci.org/bitranox/lib_log_utils>`_, automatic daily builds and monitoring
+`good code coverage <https://codecov.io/gh/bitranox/lib_log_utils>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://travis-ci.org/bitranox/lib_log_utils>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -244,40 +244,28 @@
 - Before You start, its highly recommended to update pip and setup tools:
 
 
 .. code-block:: bash
 
     python -m pip --upgrade pip
     python -m pip --upgrade setuptools
-    python -m pip --upgrade wheel
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block:: bash
 
-    # install latest release from PyPi
     python -m pip install --upgrade lib_log_utils
 
-    # test latest release from PyPi without installing (can be skipped)
-    python -m pip install lib_log_utils --install-option test
-
-- to install the latest development version from github via pip:
+- to install the latest version from github via pip:
 
 
 .. code-block:: bash
 
-    # normal install
     python -m pip install --upgrade git+https://github.com/bitranox/lib_log_utils.git
 
-    # to test without installing (can be skipped)
-    python -m pip install git+https://github.com/bitranox/lib_log_utils.git --install-option test
-
-    # to install and upgrade all dependencies regardless of version number
-    python -m pip install --upgrade git+https://github.com/bitranox/lib_log_utils.git --upgrade-strategy eager
-
 
 - include it into Your requirements.txt:
 
 .. code-block:: bash
 
     # Insert following line in Your requirements.txt:
     # for the latest Release on pypi:
@@ -286,27 +274,21 @@
     # for the latest development version :
     lib_log_utils @ git+https://github.com/bitranox/lib_log_utils.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-
 - to install the latest development version from source code:
 
 .. code-block:: bash
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_log_utils.git
     $ cd lib_log_utils
-
-    # to test without installing (can be skipped)
-    python setup.py test
-
-    # normal install
     python setup.py install
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
@@ -362,14 +344,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.4.9
+--------
+2020-08-08: service release
+    - fix documentation
+    - fix travis
+    - deprecate pycodestyle
+    - implement flake8
+
 v1.4.8
 ---------
 2020-08-01: fix doctests in windows
 
 v1.4.7
 ---------
 2020-08-01: fix pypi deploy
```

### Comparing `lib_log_utils-1.4.8/lib_log_utils/__init__conf__.py` & `lib_log_utils-1.4.9/lib_log_utils/__init__conf__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 name = 'lib_log_utils'
 title = 'colored log messages and banners from commandline and python'
-version = 'v1.4.8'
+version = 'v1.4.9'
 url = 'https://github.com/bitranox/lib_log_utils'
 author = 'Robert Nowotny'
 author_email = 'bitranox@gmail.com'
 shell_command = 'log_util'
 
 
 def print_info() -> None:
     print("""\
 
 Info for lib_log_utils:
 
     colored log messages and banners from commandline and python
 
-    Version : v1.4.8
+    Version : v1.4.9
     Url     : https://github.com/bitranox/lib_log_utils
     Author  : Robert Nowotny
     Email   : bitranox@gmail.com""")
```

### Comparing `lib_log_utils-1.4.8/lib_log_utils/lib_log_utils.py` & `lib_log_utils-1.4.9/lib_log_utils/lib_log_utils.py`

 * *Files identical despite different names*

### Comparing `lib_log_utils-1.4.8/lib_log_utils/lib_log_utils_cli.py` & `lib_log_utils-1.4.9/lib_log_utils/lib_log_utils_cli.py`

 * *Files identical despite different names*

### Comparing `lib_log_utils-1.4.8/lib_log_utils/log_config.py` & `lib_log_utils-1.4.9/lib_log_utils/log_config.py`

 * *Files identical despite different names*

### Comparing `lib_log_utils-1.4.8/lib_log_utils/log_handlers.py` & `lib_log_utils-1.4.9/lib_log_utils/log_handlers.py`

 * *Files identical despite different names*

### Comparing `lib_log_utils-1.4.8/lib_log_utils/log_levels.py` & `lib_log_utils-1.4.9/lib_log_utils/log_levels.py`

 * *Files identical despite different names*

### Comparing `lib_log_utils-1.4.8/lib_log_utils/log_traceback.py` & `lib_log_utils-1.4.9/lib_log_utils/log_traceback.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,14 @@
     >>> print_stdout(exc_info)
 
     >>> # test stdout
     >>> exc_info.stdout=b'test'
     >>> print_stdout(exc_info)
 
     """
-    encoding = sys.getdefaultencoding()
     if hasattr(exc_info, 'stdout'):
         if exc_info.stdout is not None:
             assert isinstance(exc_info.stdout, bytes)
             print(b'STDOUT: ' + exc_info.stdout, file=sys.stderr)
 
 
 def print_stderr(exc_info: Any) -> None:
@@ -137,15 +136,14 @@
     >>> print_stderr(exc_info)
 
     >>> # test stdout
     >>> exc_info.stderr=b'test'
     >>> print_stderr(exc_info)
 
     """
-    encoding = sys.getdefaultencoding()
     if hasattr(exc_info, 'stderr'):
         if exc_info.stderr is not None:
             assert isinstance(exc_info.stderr, bytes)
             print(b'STDERR: ' + exc_info.stderr, file=sys.stderr)
 
 
 def log_stdout(exc_info: Any, log_level_exec_info: int) -> None:
```

### Comparing `lib_log_utils-1.4.8/lib_log_utils.egg-info/PKG-INFO` & `lib_log_utils-1.4.9/lib_log_utils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: lib-log-utils
-Version: 1.4.8
+Version: 1.4.9
 Summary: colored log messages and banners from commandline and python
 Home-page: https://github.com/bitranox/lib_log_utils
 Author: Robert Nowotny
 Author-email: bitranox@gmail.com
 License: UNKNOWN
 Description: lib_log_utils
         =============
         
         
-        Version v1.4.8 as of 2020-08-01 see `Changelog`_
+        Version v1.4.9 as of 2020-08-08 see `Changelog`_
         
         |travis_build| |license| |jupyter| |pypi|
         
         |codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
         
         
         .. |travis_build| image:: https://img.shields.io/travis/bitranox/lib_log_utils/master.svg
@@ -62,15 +62,15 @@
         automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
         .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
         
         Python version required: 3.6.0 or newer
         
         tested on linux "bionic" with python 3.6, 3.7, 3.8, 3.8-dev, pypy3 - architectures: amd64, ppc64le, s390x, arm64
         
-        `good code coverage <https://codecov.io/gh/bitranox/lib_log_utils>`_, codestyle checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://travis-ci.org/bitranox/lib_log_utils>`_, automatic daily builds and monitoring
+        `good code coverage <https://codecov.io/gh/bitranox/lib_log_utils>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://travis-ci.org/bitranox/lib_log_utils>`_, automatic daily builds and monitoring
         
         ----
         
         - `Try it Online`_
         - `Usage`_
         - `Usage from Commandline`_
         - `Installation and Upgrade`_
@@ -252,40 +252,28 @@
         - Before You start, its highly recommended to update pip and setup tools:
         
         
         .. code-block:: bash
         
             python -m pip --upgrade pip
             python -m pip --upgrade setuptools
-            python -m pip --upgrade wheel
         
         - to install the latest release from PyPi via pip (recommended):
         
         .. code-block:: bash
         
-            # install latest release from PyPi
             python -m pip install --upgrade lib_log_utils
         
-            # test latest release from PyPi without installing (can be skipped)
-            python -m pip install lib_log_utils --install-option test
-        
-        - to install the latest development version from github via pip:
+        - to install the latest version from github via pip:
         
         
         .. code-block:: bash
         
-            # normal install
             python -m pip install --upgrade git+https://github.com/bitranox/lib_log_utils.git
         
-            # to test without installing (can be skipped)
-            python -m pip install git+https://github.com/bitranox/lib_log_utils.git --install-option test
-        
-            # to install and upgrade all dependencies regardless of version number
-            python -m pip install --upgrade git+https://github.com/bitranox/lib_log_utils.git --upgrade-strategy eager
-        
         
         - include it into Your requirements.txt:
         
         .. code-block:: bash
         
             # Insert following line in Your requirements.txt:
             # for the latest Release on pypi:
@@ -294,27 +282,21 @@
             # for the latest development version :
             lib_log_utils @ git+https://github.com/bitranox/lib_log_utils.git
         
             # to install and upgrade all modules mentioned in requirements.txt:
             python -m pip install --upgrade -r /<path>/requirements.txt
         
         
-        
         - to install the latest development version from source code:
         
         .. code-block:: bash
         
             # cd ~
             $ git clone https://github.com/bitranox/lib_log_utils.git
             $ cd lib_log_utils
-        
-            # to test without installing (can be skipped)
-            python setup.py test
-        
-            # normal install
             python setup.py install
         
         - via makefile:
           makefiles are a very convenient way to install. Here we can do much more,
           like installing virtual environments, clean caches and so on.
         
         .. code-block:: shell
@@ -370,14 +352,22 @@
         Changelog
         =========
         
         - new MAJOR version for incompatible API changes,
         - new MINOR version for added functionality in a backwards compatible manner
         - new PATCH version for backwards compatible bug fixes
         
+        v1.4.9
+        --------
+        2020-08-08: service release
+            - fix documentation
+            - fix travis
+            - deprecate pycodestyle
+            - implement flake8
+        
         v1.4.8
         ---------
         2020-08-01: fix doctests in windows
         
         v1.4.7
         ---------
         2020-08-01: fix pypi deploy
```

### Comparing `lib_log_utils-1.4.8/lib_log_utils.egg-info/SOURCES.txt` & `lib_log_utils-1.4.9/lib_log_utils.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 CHANGES.rst
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 lib_log_utils/__init__.py
 lib_log_utils/__init__conf__.py
 lib_log_utils/lib_log_utils.py
 lib_log_utils/lib_log_utils_cli.py
 lib_log_utils/log_config.py
```

### Comparing `lib_log_utils-1.4.8/setup.py` & `lib_log_utils-1.4.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,110 +1,124 @@
-"""
-Setuptools entry point.
-see : https://docs.python.org/3.8/distutils/setupscript.html
-"""
+#!/usr/bin/env python3
 
 import codecs
 import os
 import pathlib
 from typing import Any, List, Dict
 
-from setuptools import setup                # type: ignore
+from setuptools import setup  # type: ignore
 from setuptools import find_packages
 
 
 def is_travis_deploy() -> bool:
-    if os.getenv('DEPLOY_SDIST', '') or os.getenv('DEPLOY_WHEEL', ''):
+    if os.getenv("DEPLOY_SDIST", "") or os.getenv("DEPLOY_WHEEL", ""):
         return is_tagged_commit()
+    else:
+        return False
 
 
 def is_tagged_commit() -> bool:
-    if 'TRAVIS_TAG' in os.environ:
-        if os.environ['TRAVIS_TAG']:
+    if "TRAVIS_TAG" in os.environ:
+        if os.environ["TRAVIS_TAG"]:
             return True
     return False
 
 
 def strip_links_from_required(l_required: List[str]) -> List[str]:
     """
     >>> required = ['lib_regexp @ git+https://github.com/bitranox/lib_regexp.git', 'test']
     >>> assert strip_links_from_required(required) == ['lib_regexp', 'test']
 
     """
-    l_req_stripped = list()                                        # type: List[str]
+    l_req_stripped: List[str] = list()
     for req in l_required:
-        req_stripped = req.split('@')[0].strip()
+        req_stripped = req.split("@")[0].strip()
         l_req_stripped.append(req_stripped)
     return l_req_stripped
 
 
-long_description = 'colored log messages and banners from commandline and python'   # will be overwritten with long_description if exists !
-path_readme = pathlib.Path(__file__).parent / 'README.rst'
+# will be overwritten with long_description if exists !
+long_description = "colored log messages and banners from commandline and python"
+path_readme = pathlib.Path(__file__).parent / "README.rst"
 
 if path_readme.exists():
     # noinspection PyBroadException
     try:
-        readme_content = codecs.open(str(path_readme), encoding='utf-8').read()
+        readme_content = codecs.open(str(path_readme), encoding="utf-8").read()
         long_description = readme_content
     except Exception:
         pass
 
 
 def get_requirements_from_file(requirements_filename: str) -> List[str]:
     """
     >>> assert len(get_requirements_from_file('requirements.txt')) > 0
     """
     l_requirements = list()
     try:
-        with open(str(pathlib.Path(__file__).parent / requirements_filename), mode='r') as requirements_file:
+        with open(
+            str(pathlib.Path(__file__).parent / requirements_filename), mode="r"
+        ) as requirements_file:
             for line in requirements_file:
                 line_data = get_line_data(line)
                 if line_data:
                     l_requirements.append(line_data)
     except FileNotFoundError:
         pass
     return l_requirements
 
 
 def get_line_data(line: str) -> str:
     line = line.strip()
-    if '#' in line:
-        line = line.split('#', 1)[0].strip()
+    if "#" in line:
+        line = line.split("#", 1)[0].strip()
     return line
 
 
-tests_require = get_requirements_from_file('requirements_test.txt')
-install_requires = get_requirements_from_file('requirements.txt')
+tests_require = get_requirements_from_file("requirements_test.txt")
+install_requires = get_requirements_from_file("requirements.txt")
 setup_requires = list(set(tests_require + install_requires))
 
 # for deploy on pypi we must not rely on imports from github
 if is_travis_deploy() and is_tagged_commit():
     setup_requires = strip_links_from_required(setup_requires)
     tests_require = strip_links_from_required(tests_require)
     install_requires = strip_links_from_required(install_requires)
 
 setup_kwargs: Dict[str, Any] = dict()
-setup_kwargs['name'] = 'lib_log_utils'
-setup_kwargs['version'] = 'v1.4.8'
-setup_kwargs['url'] = 'https://github.com/bitranox/lib_log_utils'
-setup_kwargs['packages'] = find_packages()
-setup_kwargs['package_data'] = {'lib_log_utils': ['py.typed', '*.pyi', '__init__.pyi']}
-setup_kwargs['description'] = 'colored log messages and banners from commandline and python'
-setup_kwargs['long_description'] = long_description
-setup_kwargs['long_description_content_type'] = 'text/x-rst'
-setup_kwargs['author'] = 'Robert Nowotny'
-setup_kwargs['author_email'] = 'bitranox@gmail.com'
-setup_kwargs['classifiers'] = ['Development Status :: 5 - Production/Stable', 'Intended Audience :: Developers', 'License :: OSI Approved :: MIT License', 'Natural Language :: English', 'Operating System :: OS Independent', 'Programming Language :: Python', 'Topic :: Software Development :: Libraries :: Python Modules']
-setup_kwargs['entry_points'] = {'console_scripts': ['log_util = lib_log_utils.lib_log_utils_cli:cli_main']}
+setup_kwargs["name"] = "lib_log_utils"
+setup_kwargs["version"] = "v1.4.9"
+setup_kwargs["url"] = "https://github.com/bitranox/lib_log_utils"
+setup_kwargs["packages"] = find_packages()
+setup_kwargs["package_data"] = {"lib_log_utils": ["py.typed", "*.pyi", "__init__.pyi"]}
+setup_kwargs[
+    "description"
+] = "colored log messages and banners from commandline and python"
+setup_kwargs["long_description"] = long_description
+setup_kwargs["long_description_content_type"] = "text/x-rst"
+setup_kwargs["author"] = "Robert Nowotny"
+setup_kwargs["author_email"] = "bitranox@gmail.com"
+setup_kwargs["classifiers"] = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Natural Language :: English",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+]
+setup_kwargs["entry_points"] = {
+    "console_scripts": ["log_util = lib_log_utils.lib_log_utils_cli:cli_main"]
+}
 # minimally needs to run tests - no project requirements here
-setup_kwargs['tests_require'] = tests_require
+setup_kwargs["tests_require"] = tests_require
 # specify what a project minimally needs to run correctly
-setup_kwargs['install_requires'] = install_requires
+setup_kwargs["install_requires"] = install_requires
 # minimally needs to run the setup script, dependencies needs also to put here for "setup.py install test"
 # dependencies must not be put here for pip install
-setup_kwargs['setup_requires'] = setup_requires
-setup_kwargs['python_requires'] = ">=3.6.0"
-setup_kwargs['zip_safe'] = False
+setup_kwargs["setup_requires"] = setup_requires
+setup_kwargs["python_requires"] = ">=3.6.0"
+setup_kwargs["zip_safe"] = False
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     setup(**setup_kwargs)
```

