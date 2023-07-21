# Comparing `tmp/lark-cython-0.0.7.tar.gz` & `tmp/lark-cython-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lark-cython-0.0.7.tar", last modified: Mon Jan 31 08:47:15 2022, max compression
+gzip compressed data, was "lark-cython-0.0.9.tar", last modified: Thu Feb 10 08:01:50 2022, max compression
```

## Comparing `lark-cython-0.0.7.tar` & `lark-cython-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-01-31 08:47:15.964229 lark-cython-0.0.7/
--rw-rw-rw-   0        0        0     1110 2022-01-26 09:14:08.000000 lark-cython-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       25 2022-01-26 11:33:08.000000 lark-cython-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      366 2022-01-31 08:47:15.963236 lark-cython-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      895 2022-01-31 08:46:37.000000 lark-cython-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2022-01-31 08:47:15.939229 lark-cython-0.0.7/lark_cython/
--rw-rw-rw-   0        0        0       21 2022-01-31 08:26:16.000000 lark-cython-0.0.7/lark_cython/__init__.py
--rw-rw-rw-   0        0        0  2320941 2022-01-31 08:31:32.000000 lark-cython-0.0.7/lark_cython/lark_cython.c
--rw-rw-rw-   0        0        0   479744 2022-01-31 08:31:36.000000 lark-cython-0.0.7/lark_cython/lark_cython.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0    37636 2022-01-31 08:31:21.000000 lark-cython-0.0.7/lark_cython/lark_cython.pyx
-drwxrwxrwx   0        0        0        0 2022-01-31 08:47:15.961229 lark-cython-0.0.7/lark_cython.egg-info/
--rw-rw-rw-   0        0        0      366 2022-01-31 08:47:15.000000 lark-cython-0.0.7/lark_cython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2022-01-31 08:47:15.000000 lark-cython-0.0.7/lark_cython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-31 08:47:15.000000 lark-cython-0.0.7/lark_cython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2022-01-31 08:47:15.000000 lark-cython-0.0.7/lark_cython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-01-31 08:47:15.000000 lark-cython-0.0.7/lark_cython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2022-01-26 11:33:08.000000 lark-cython-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-01-31 08:47:15.964229 lark-cython-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1084 2022-01-31 08:24:37.000000 lark-cython-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2022-02-10 08:01:50.268532 lark-cython-0.0.9/
+-rw-rw-rw-   0        0        0     1110 2022-01-26 09:14:08.000000 lark-cython-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       25 2022-01-26 11:33:08.000000 lark-cython-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      366 2022-02-10 08:01:50.268532 lark-cython-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1075 2022-02-07 09:15:43.000000 lark-cython-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-02-10 08:01:50.256512 lark-cython-0.0.9/lark_cython/
+-rw-rw-rw-   0        0        0       64 2022-02-10 08:01:42.000000 lark-cython-0.0.9/lark_cython/__init__.py
+-rw-rw-rw-   0        0        0  2320941 2022-02-10 08:00:42.000000 lark-cython-0.0.9/lark_cython/lark_cython.c
+-rw-rw-rw-   0        0        0   480768 2022-02-09 22:32:41.000000 lark-cython-0.0.9/lark_cython/lark_cython.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0    37636 2022-02-10 07:58:37.000000 lark-cython-0.0.9/lark_cython/lark_cython.pyx
+drwxrwxrwx   0        0        0        0 2022-02-10 08:01:50.267533 lark-cython-0.0.9/lark_cython.egg-info/
+-rw-rw-rw-   0        0        0      366 2022-02-10 08:01:50.000000 lark-cython-0.0.9/lark_cython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2022-02-10 08:01:50.000000 lark-cython-0.0.9/lark_cython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-02-10 08:01:50.000000 lark-cython-0.0.9/lark_cython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2022-02-10 08:01:50.000000 lark-cython-0.0.9/lark_cython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2022-02-10 08:01:50.000000 lark-cython-0.0.9/lark_cython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2022-01-26 11:33:08.000000 lark-cython-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-02-10 08:01:50.268532 lark-cython-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1088 2022-02-10 08:01:00.000000 lark-cython-0.0.9/setup.py
```

### Comparing `lark-cython-0.0.7/LICENSE` & `lark-cython-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lark-cython-0.0.7/README.md` & `lark-cython-0.0.9/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 # Lark-Cython
 
-Cython plugin for Lark, reimplementing the LALR parser &amp; lexer for better performance on CPython.
+Cython plugin for [Lark](https://github.com/lark-parser/lark), reimplementing the LALR parser &amp; lexer for better performance on CPython.
 
-**WIP**
+Install:
+
+```python
+pip install lark-cython
+```
 
 Usage:
 
 ```python
-from lark_cython import lark_cython
+import lark_cython
 
-parser = Lark(grammar, _plugins=lark_cython.plugins)
+parser = Lark(grammar, parser="lalr", _plugins=lark_cython.plugins)
 
 # Use Lark as you usually would, with a huge performance boost
 ```
 
+See the [examples](https://github.com/lark-parser/lark_cython/tree/master/examples) for more.
+
+
 ## Differences from Lark
 
 - `Token` instances do not inherit from `str`. You must use the `value` attribute to get the string.
 
 ## Other caveats
 
 - Postlexer isn't currently implemented
```

### Comparing `lark-cython-0.0.7/lark_cython/lark_cython.c` & `lark-cython-0.0.9/lark_cython/lark_cython.c`

 * *Files identical despite different names*

### Comparing `lark-cython-0.0.7/lark_cython/lark_cython.pyx` & `lark-cython-0.0.9/lark_cython/lark_cython.pyx`

 * *Files identical despite different names*

### Comparing `lark-cython-0.0.7/setup.py` & `lark-cython-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 except ImportError:
      def cythonize(*args, **kwargs):
          from Cython.Build import cythonize
          return cythonize(*args, **kwargs)
 
 setup(
     name = "lark-cython",
-    version = "0.0.7",
+    version = __version__,
     packages=find_packages(),
 
     ext_modules = cythonize('lark_cython/*.pyx'), # accepts a glob pattern
     requires = ['Cython'],
     install_requires = ['lark>=1.1.0', 'cython>=0.29.0', 'Cython>=0.29.0'],
     setup_requires=['Cython'],
```

