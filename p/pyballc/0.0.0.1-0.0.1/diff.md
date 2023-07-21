# Comparing `tmp/pyballc-0.0.0.1.tar.gz` & `tmp/pyballc-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyballc-0.0.0.1.tar", last modified: Fri Jul 21 20:59:56 2023, max compression
+gzip compressed data, was "pyballc-0.0.1.tar", last modified: Fri Jul 21 20:58:57 2023, max compression
```

## Comparing `pyballc-0.0.0.1.tar` & `pyballc-0.0.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxr-x   0 wtian    (44982) wtian    (44982)        0 2023-07-21 20:52:31.569518 pyballc-0.0.0.1/
--rw-rw-r--   0 wtian    (44982) wtian    (44982)    18092 2023-07-12 19:05:54.000000 pyballc-0.0.0.1/LICENSE
--rw-rw-r--   0 wtian    (44982) wtian    (44982)       60 2023-07-12 19:05:54.000000 pyballc-0.0.0.1/MANIFEST.in
--rw-rw-r--   0 wtian    (44982) wtian    (44982)      122 2023-07-21 20:52:31.568520 pyballc-0.0.0.1/PKG-INFO
--rw-rw-r--   0 wtian    (44982) wtian    (44982)      899 2023-07-12 19:22:28.000000 pyballc-0.0.0.1/README.md
-drwxrwxr-x   0 wtian    (44982) wtian    (44982)        0 2023-07-21 20:52:31.516520 pyballc-0.0.0.1/pyballc/
--rw-rw-r--   0 wtian    (44982) wtian    (44982)       31 2023-07-12 19:05:54.000000 pyballc-0.0.0.1/pyballc/__init__.py
--rwxrwxr-x   0 wtian    (44982) wtian    (44982)   364824 2023-07-21 20:51:40.000000 pyballc-0.0.0.1/pyballc/_pyballcools.so
--rw-rw-r--   0 wtian    (44982) wtian    (44982)     1739 2023-07-12 19:31:11.000000 pyballc-0.0.0.1/pyballc/pyballc.py
--rw-rw-r--   0 wtian    (44982) wtian    (44982)    15826 2023-07-12 19:05:54.000000 pyballc-0.0.0.1/pyballc/pyballcools.py
-drwxrwxr-x   0 wtian    (44982) wtian    (44982)        0 2023-07-21 20:52:31.546526 pyballc-0.0.0.1/pyballc.egg-info/
--rw-rw-r--   0 wtian    (44982) wtian    (44982)      122 2023-07-21 20:52:31.000000 pyballc-0.0.0.1/pyballc.egg-info/PKG-INFO
--rw-rw-r--   0 wtian    (44982) wtian    (44982)      278 2023-07-21 20:52:31.000000 pyballc-0.0.0.1/pyballc.egg-info/SOURCES.txt
--rw-rw-r--   0 wtian    (44982) wtian    (44982)        1 2023-07-21 20:52:31.000000 pyballc-0.0.0.1/pyballc.egg-info/dependency_links.txt
--rw-rw-r--   0 wtian    (44982) wtian    (44982)        6 2023-07-21 20:52:31.000000 pyballc-0.0.0.1/pyballc.egg-info/requires.txt
--rw-rw-r--   0 wtian    (44982) wtian    (44982)        8 2023-07-21 20:52:31.000000 pyballc-0.0.0.1/pyballc.egg-info/top_level.txt
--rw-rw-r--   0 wtian    (44982) wtian    (44982)       38 2023-07-21 20:52:31.569520 pyballc-0.0.0.1/setup.cfg
--rw-rw-r--   0 wtian    (44982) wtian    (44982)     2129 2023-07-21 20:52:29.000000 pyballc-0.0.0.1/setup.py
+drwxrwxr-x   0 wtian    (44982) wtian    (44982)        0 2023-07-21 20:51:32.701329 pyballc-0.0.1/
+-rw-rw-r--   0 wtian    (44982) wtian    (44982)    18092 2023-07-12 19:05:54.000000 pyballc-0.0.1/LICENSE
+-rw-rw-r--   0 wtian    (44982) wtian    (44982)       60 2023-07-12 19:05:54.000000 pyballc-0.0.1/MANIFEST.in
+-rw-rw-r--   0 wtian    (44982) wtian    (44982)      120 2023-07-21 20:51:32.700336 pyballc-0.0.1/PKG-INFO
+-rw-rw-r--   0 wtian    (44982) wtian    (44982)      899 2023-07-12 19:22:28.000000 pyballc-0.0.1/README.md
+drwxrwxr-x   0 wtian    (44982) wtian    (44982)        0 2023-07-21 20:51:31.929350 pyballc-0.0.1/pyballc/
+-rw-rw-r--   0 wtian    (44982) wtian    (44982)       31 2023-07-12 19:05:54.000000 pyballc-0.0.1/pyballc/__init__.py
+-rw-rw-r--   0 wtian    (44982) wtian    (44982)     1739 2023-07-12 19:31:11.000000 pyballc-0.0.1/pyballc/pyballc.py
+-rw-rw-r--   0 wtian    (44982) wtian    (44982)    15826 2023-07-12 19:05:54.000000 pyballc-0.0.1/pyballc/pyballcools.py
+drwxrwxr-x   0 wtian    (44982) wtian    (44982)        0 2023-07-21 20:51:31.991348 pyballc-0.0.1/pyballc.egg-info/
+-rw-rw-r--   0 wtian    (44982) wtian    (44982)      120 2023-07-21 20:51:31.000000 pyballc-0.0.1/pyballc.egg-info/PKG-INFO
+-rw-rw-r--   0 wtian    (44982) wtian    (44982)      254 2023-07-21 20:51:31.000000 pyballc-0.0.1/pyballc.egg-info/SOURCES.txt
+-rw-rw-r--   0 wtian    (44982) wtian    (44982)        1 2023-07-21 20:51:31.000000 pyballc-0.0.1/pyballc.egg-info/dependency_links.txt
+-rw-rw-r--   0 wtian    (44982) wtian    (44982)        6 2023-07-21 20:51:31.000000 pyballc-0.0.1/pyballc.egg-info/requires.txt
+-rw-rw-r--   0 wtian    (44982) wtian    (44982)        8 2023-07-21 20:51:31.000000 pyballc-0.0.1/pyballc.egg-info/top_level.txt
+-rw-rw-r--   0 wtian    (44982) wtian    (44982)       38 2023-07-21 20:51:32.701331 pyballc-0.0.1/setup.cfg
+-rw-rw-r--   0 wtian    (44982) wtian    (44982)     2127 2023-07-12 19:05:54.000000 pyballc-0.0.1/setup.py
```

### Comparing `pyballc-0.0.0.1/LICENSE` & `pyballc-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyballc-0.0.0.1/README.md` & `pyballc-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyballc-0.0.0.1/pyballc/pyballc.py` & `pyballc-0.0.1/pyballc/pyballc.py`

 * *Files identical despite different names*

### Comparing `pyballc-0.0.0.1/pyballc/pyballcools.py` & `pyballc-0.0.1/pyballc/pyballcools.py`

 * *Files identical despite different names*

### Comparing `pyballc-0.0.0.1/setup.py` & `pyballc-0.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     """Customized setuptools bdist_wheel command."""
     def run(self):
         custom_command()
         bdist_wheel.run(self)
 
 setup(
     name='pyballc',
-    version='0.0.0.1',
+    version='0.0.1',
     description='Python module for reading BAllC files',
     packages=find_packages(),
     cmdclass={
         'install': CustomInstallCommand,
         'bdist_egg': CustomBDistEggCommand,
         'bdist_wheel': CustomBDistWheelCommand,
     },
```

