# Comparing `tmp/pydevicetree-0.0.8.tar.gz` & `tmp/pydevicetree-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydevicetree-0.0.8.tar", last modified: Wed Nov 27 19:00:20 2019, max compression
+gzip compressed data, was "dist/pydevicetree-0.0.9.tar", last modified: Mon Dec  2 19:45:24 2019, max compression
```

## Comparing `pydevicetree-0.0.8.tar` & `pydevicetree-0.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 nathanielg  (1180) nathanielg  (1180)        0 2019-11-27 19:00:20.000000 pydevicetree-0.0.8/
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)       37 2019-11-06 23:32:46.000000 pydevicetree-0.0.8/MANIFEST.in
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     5305 2019-11-27 19:00:20.000000 pydevicetree-0.0.8/PKG-INFO
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3532 2019-11-26 18:39:52.000000 pydevicetree-0.0.8/README.md
-drwxrwxr-x   0 nathanielg  (1180) nathanielg  (1180)        0 2019-11-27 19:00:20.000000 pydevicetree-0.0.8/pydevicetree/
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)      162 2019-11-07 00:18:55.000000 pydevicetree-0.0.8/pydevicetree/__init__.py
-drwxrwxr-x   0 nathanielg  (1180) nathanielg  (1180)        0 2019-11-27 19:00:20.000000 pydevicetree-0.0.8/pydevicetree/ast/
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)      451 2019-11-25 22:08:36.000000 pydevicetree-0.0.8/pydevicetree/ast/__init__.py
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     1205 2019-11-14 04:36:43.000000 pydevicetree-0.0.8/pydevicetree/ast/directive.py
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)      856 2019-11-13 23:03:22.000000 pydevicetree-0.0.8/pydevicetree/ast/helpers.py
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)    18572 2019-11-27 18:55:15.000000 pydevicetree-0.0.8/pydevicetree/ast/node.py
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     9402 2019-11-27 18:55:15.000000 pydevicetree-0.0.8/pydevicetree/ast/property.py
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3803 2019-11-15 21:39:22.000000 pydevicetree-0.0.8/pydevicetree/ast/reference.py
-drwxrwxr-x   0 nathanielg  (1180) nathanielg  (1180)        0 2019-11-27 19:00:20.000000 pydevicetree-0.0.8/pydevicetree/source/
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)      170 2019-11-08 22:25:50.000000 pydevicetree-0.0.8/pydevicetree/source/__init__.py
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     2918 2019-11-14 04:36:43.000000 pydevicetree-0.0.8/pydevicetree/source/grammar.py
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     7376 2019-11-14 04:36:43.000000 pydevicetree-0.0.8/pydevicetree/source/parser.py
-drwxrwxr-x   0 nathanielg  (1180) nathanielg  (1180)        0 2019-11-27 19:00:20.000000 pydevicetree-0.0.8/pydevicetree.egg-info/
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     5305 2019-11-27 19:00:20.000000 pydevicetree-0.0.8/pydevicetree.egg-info/PKG-INFO
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     1278 2019-11-27 19:00:20.000000 pydevicetree-0.0.8/pydevicetree.egg-info/SOURCES.txt
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)        1 2019-11-27 19:00:20.000000 pydevicetree-0.0.8/pydevicetree.egg-info/dependency_links.txt
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)       15 2019-11-27 19:00:20.000000 pydevicetree-0.0.8/pydevicetree.egg-info/requires.txt
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)       19 2019-11-27 19:00:20.000000 pydevicetree-0.0.8/pydevicetree.egg-info/top_level.txt
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)       38 2019-11-27 19:00:20.000000 pydevicetree-0.0.8/setup.cfg
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)      864 2019-11-27 18:59:57.000000 pydevicetree-0.0.8/setup.py
-drwxrwxr-x   0 nathanielg  (1180) nathanielg  (1180)        0 2019-11-27 19:00:20.000000 pydevicetree-0.0.8/tests/
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)       94 2019-11-06 21:20:36.000000 pydevicetree-0.0.8/tests/__init__.py
-drwxrwxr-x   0 nathanielg  (1180) nathanielg  (1180)        0 2019-11-27 19:00:20.000000 pydevicetree-0.0.8/tests/devicetrees/
-drwxrwxr-x   0 nathanielg  (1180) nathanielg  (1180)        0 2019-11-27 19:00:20.000000 pydevicetree-0.0.8/tests/devicetrees/include/
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)      361 2019-11-06 21:22:06.000000 pydevicetree-0.0.8/tests/devicetrees/include/base.dts
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)      247 2019-11-08 22:21:27.000000 pydevicetree-0.0.8/tests/devicetrees/include/overlay.dtsi
-drwxrwxr-x   0 nathanielg  (1180) nathanielg  (1180)        0 2019-11-27 19:00:20.000000 pydevicetree-0.0.8/tests/devicetrees/sifive/
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     1938 2019-11-06 21:22:39.000000 pydevicetree-0.0.8/tests/devicetrees/sifive/e20.dts
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     2818 2019-11-06 21:22:39.000000 pydevicetree-0.0.8/tests/devicetrees/sifive/e21.dts
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     2819 2019-11-06 21:22:39.000000 pydevicetree-0.0.8/tests/devicetrees/sifive/e24.dts
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3240 2019-11-06 21:22:39.000000 pydevicetree-0.0.8/tests/devicetrees/sifive/e31.dts
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3241 2019-11-06 21:22:39.000000 pydevicetree-0.0.8/tests/devicetrees/sifive/e34.dts
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3221 2019-11-06 21:22:39.000000 pydevicetree-0.0.8/tests/devicetrees/sifive/e76.dts
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     6527 2019-11-06 21:22:39.000000 pydevicetree-0.0.8/tests/devicetrees/sifive/e76mc.dts
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     2824 2019-11-06 21:22:39.000000 pydevicetree-0.0.8/tests/devicetrees/sifive/s21.dts
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3385 2019-11-06 21:22:39.000000 pydevicetree-0.0.8/tests/devicetrees/sifive/s51.dts
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3248 2019-11-06 21:22:39.000000 pydevicetree-0.0.8/tests/devicetrees/sifive/s54.dts
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3224 2019-11-06 21:22:39.000000 pydevicetree-0.0.8/tests/devicetrees/sifive/s76.dts
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     6531 2019-11-06 21:22:39.000000 pydevicetree-0.0.8/tests/devicetrees/sifive/s76mc.dts
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3133 2019-11-06 21:22:39.000000 pydevicetree-0.0.8/tests/devicetrees/sifive/u52.dts
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     4004 2019-11-06 21:22:39.000000 pydevicetree-0.0.8/tests/devicetrees/sifive/u54.dts
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     8403 2019-11-06 21:22:39.000000 pydevicetree-0.0.8/tests/devicetrees/sifive/u54mc.dts
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3843 2019-11-06 21:22:39.000000 pydevicetree-0.0.8/tests/devicetrees/sifive/u74.dts
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     7722 2019-11-06 21:22:39.000000 pydevicetree-0.0.8/tests/devicetrees/sifive/u74mc.dts
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     7046 2019-11-27 18:55:15.000000 pydevicetree-0.0.8/tests/test_devicetree.py
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     1065 2019-11-13 20:33:05.000000 pydevicetree-0.0.8/tests/test_exceptions.py
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     2054 2019-11-06 21:20:39.000000 pydevicetree-0.0.8/tests/test_full_trees.py
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3737 2019-11-14 04:36:43.000000 pydevicetree-0.0.8/tests/test_grammar.py
--rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     1470 2019-11-06 21:20:40.000000 pydevicetree-0.0.8/tests/test_overlay.py
+drwxrwxr-x   0 nathanielg  (1180) nathanielg  (1180)        0 2019-12-02 19:45:24.000000 pydevicetree-0.0.9/
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)       37 2019-11-06 23:32:46.000000 pydevicetree-0.0.9/MANIFEST.in
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     5305 2019-12-02 19:45:24.000000 pydevicetree-0.0.9/PKG-INFO
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3532 2019-11-26 18:39:52.000000 pydevicetree-0.0.9/README.md
+drwxrwxr-x   0 nathanielg  (1180) nathanielg  (1180)        0 2019-12-02 19:45:24.000000 pydevicetree-0.0.9/pydevicetree/
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)      162 2019-11-07 00:18:55.000000 pydevicetree-0.0.9/pydevicetree/__init__.py
+drwxrwxr-x   0 nathanielg  (1180) nathanielg  (1180)        0 2019-12-02 19:45:24.000000 pydevicetree-0.0.9/pydevicetree/ast/
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)      451 2019-11-25 22:08:36.000000 pydevicetree-0.0.9/pydevicetree/ast/__init__.py
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     1563 2019-12-02 18:46:30.000000 pydevicetree-0.0.9/pydevicetree/ast/directive.py
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)      856 2019-11-13 23:03:22.000000 pydevicetree-0.0.9/pydevicetree/ast/helpers.py
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)    18632 2019-12-02 18:46:30.000000 pydevicetree-0.0.9/pydevicetree/ast/node.py
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     9402 2019-11-27 18:55:15.000000 pydevicetree-0.0.9/pydevicetree/ast/property.py
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3803 2019-11-15 21:39:22.000000 pydevicetree-0.0.9/pydevicetree/ast/reference.py
+drwxrwxr-x   0 nathanielg  (1180) nathanielg  (1180)        0 2019-12-02 19:45:24.000000 pydevicetree-0.0.9/pydevicetree/source/
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)      170 2019-11-08 22:25:50.000000 pydevicetree-0.0.9/pydevicetree/source/__init__.py
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3043 2019-12-02 18:46:30.000000 pydevicetree-0.0.9/pydevicetree/source/grammar.py
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     7434 2019-12-02 18:46:30.000000 pydevicetree-0.0.9/pydevicetree/source/parser.py
+drwxrwxr-x   0 nathanielg  (1180) nathanielg  (1180)        0 2019-12-02 19:45:24.000000 pydevicetree-0.0.9/pydevicetree.egg-info/
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     5305 2019-12-02 19:45:24.000000 pydevicetree-0.0.9/pydevicetree.egg-info/PKG-INFO
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     1278 2019-12-02 19:45:24.000000 pydevicetree-0.0.9/pydevicetree.egg-info/SOURCES.txt
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)        1 2019-12-02 19:45:24.000000 pydevicetree-0.0.9/pydevicetree.egg-info/dependency_links.txt
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)       15 2019-12-02 19:45:24.000000 pydevicetree-0.0.9/pydevicetree.egg-info/requires.txt
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)       19 2019-12-02 19:45:24.000000 pydevicetree-0.0.9/pydevicetree.egg-info/top_level.txt
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)       38 2019-12-02 19:45:24.000000 pydevicetree-0.0.9/setup.cfg
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)      864 2019-12-02 19:44:38.000000 pydevicetree-0.0.9/setup.py
+drwxrwxr-x   0 nathanielg  (1180) nathanielg  (1180)        0 2019-12-02 19:45:24.000000 pydevicetree-0.0.9/tests/
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)       94 2019-11-06 21:20:36.000000 pydevicetree-0.0.9/tests/__init__.py
+drwxrwxr-x   0 nathanielg  (1180) nathanielg  (1180)        0 2019-12-02 19:45:24.000000 pydevicetree-0.0.9/tests/devicetrees/
+drwxrwxr-x   0 nathanielg  (1180) nathanielg  (1180)        0 2019-12-02 19:45:24.000000 pydevicetree-0.0.9/tests/devicetrees/include/
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)      360 2019-12-02 18:46:30.000000 pydevicetree-0.0.9/tests/devicetrees/include/base.dts
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)      247 2019-11-08 22:21:27.000000 pydevicetree-0.0.9/tests/devicetrees/include/overlay.dtsi
+drwxrwxr-x   0 nathanielg  (1180) nathanielg  (1180)        0 2019-12-02 19:45:24.000000 pydevicetree-0.0.9/tests/devicetrees/sifive/
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     1938 2019-11-06 21:22:39.000000 pydevicetree-0.0.9/tests/devicetrees/sifive/e20.dts
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     2818 2019-11-06 21:22:39.000000 pydevicetree-0.0.9/tests/devicetrees/sifive/e21.dts
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     2819 2019-11-06 21:22:39.000000 pydevicetree-0.0.9/tests/devicetrees/sifive/e24.dts
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3240 2019-11-06 21:22:39.000000 pydevicetree-0.0.9/tests/devicetrees/sifive/e31.dts
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3241 2019-11-06 21:22:39.000000 pydevicetree-0.0.9/tests/devicetrees/sifive/e34.dts
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3221 2019-11-06 21:22:39.000000 pydevicetree-0.0.9/tests/devicetrees/sifive/e76.dts
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     6527 2019-11-06 21:22:39.000000 pydevicetree-0.0.9/tests/devicetrees/sifive/e76mc.dts
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     2824 2019-11-06 21:22:39.000000 pydevicetree-0.0.9/tests/devicetrees/sifive/s21.dts
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3385 2019-11-06 21:22:39.000000 pydevicetree-0.0.9/tests/devicetrees/sifive/s51.dts
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3248 2019-11-06 21:22:39.000000 pydevicetree-0.0.9/tests/devicetrees/sifive/s54.dts
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3224 2019-11-06 21:22:39.000000 pydevicetree-0.0.9/tests/devicetrees/sifive/s76.dts
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     6531 2019-11-06 21:22:39.000000 pydevicetree-0.0.9/tests/devicetrees/sifive/s76mc.dts
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3133 2019-11-06 21:22:39.000000 pydevicetree-0.0.9/tests/devicetrees/sifive/u52.dts
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     4004 2019-11-06 21:22:39.000000 pydevicetree-0.0.9/tests/devicetrees/sifive/u54.dts
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     8403 2019-11-06 21:22:39.000000 pydevicetree-0.0.9/tests/devicetrees/sifive/u54mc.dts
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3843 2019-11-06 21:22:39.000000 pydevicetree-0.0.9/tests/devicetrees/sifive/u74.dts
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     7722 2019-11-06 21:22:39.000000 pydevicetree-0.0.9/tests/devicetrees/sifive/u74mc.dts
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     7228 2019-12-02 18:46:30.000000 pydevicetree-0.0.9/tests/test_devicetree.py
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     1065 2019-11-13 20:33:05.000000 pydevicetree-0.0.9/tests/test_exceptions.py
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     2054 2019-11-06 21:20:39.000000 pydevicetree-0.0.9/tests/test_full_trees.py
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     3737 2019-11-14 04:36:43.000000 pydevicetree-0.0.9/tests/test_grammar.py
+-rw-rw-r--   0 nathanielg  (1180) nathanielg  (1180)     1470 2019-11-06 21:20:40.000000 pydevicetree-0.0.9/tests/test_overlay.py
```

### Comparing `pydevicetree-0.0.8/PKG-INFO` & `pydevicetree-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydevicetree
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library for parsing Devicetree Source v1
 Home-page: https://github.com/sifive/pydevicetree
 Author: Nathaniel Graff
 Author-email: nathaniel.graff@sifive.com
 License: UNKNOWN
 Description: # pydevicetree
```

### Comparing `pydevicetree-0.0.8/README.md` & `pydevicetree-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/pydevicetree/ast/directive.py` & `pydevicetree-0.0.9/pydevicetree/ast/directive.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # Copyright (c) 2019 SiFive Inc.
 # SPDX-License-Identifier: Apache-2.0
 
 from typing import Any
 
-from pydevicetree.ast.helpers import formatLevel
+from pydevicetree.ast.helpers import formatLevel, wrapStrings
 
 class Directive:
     """Represents a Devicetree directive
 
     Directives in Devicetree source are statements of the form
 
         /directive-name/ [option1 [option2 [...]]];
@@ -32,10 +32,15 @@
         return "<Directive %s>" % self.directive
 
     def __str__(self) -> str:
         return self.to_dts()
 
     def to_dts(self, level: int = 0) -> str:
         """Format the Directive in Devicetree Source format"""
-        if self.option:
-            return formatLevel(level, "%s %s;\n" % (self.directive, self.option))
+        if isinstance(self.option, list):
+            return formatLevel(level, "%s %s;\n" % (self.directive,
+                                                    wrapStrings(self.option)))
+        if isinstance(self.option, str):
+            if self.directive == "/include/":
+                return formatLevel(level, "%s \"%s\"\n" % (self.directive, self.option))
+            return formatLevel(level, "%s \"%s\";\n" % (self.directive, self.option))
         return formatLevel(level, "%s;\n" % self.directive)
```

### Comparing `pydevicetree-0.0.8/pydevicetree/ast/helpers.py` & `pydevicetree-0.0.9/pydevicetree/ast/helpers.py`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/pydevicetree/ast/node.py` & `pydevicetree-0.0.9/pydevicetree/ast/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,16 +399,17 @@
 
         Node.__init__(self, label=None, name="", address=None,
                       properties=properties, directives=directives, children=children)
 
         for node in self.children:
             node.parent = self
 
-        reference_nodes = filter(lambda node: isinstance(node, NodeReference), self.all_nodes())
-        for refnode in cast(List[NodeReference], reference_nodes):
+        reference_nodes = self.filter(lambda n: isinstance(n, NodeReference))
+        for refnode in reference_nodes:
+            refnode = cast(NodeReference, refnode)
             node = refnode.resolve_reference(self)
 
             if refnode.parent:
                 cast(Node, refnode.parent).remove_child(refnode)
 
             node.properties += refnode.properties
             node.directives += refnode.directives
@@ -456,16 +457,18 @@
     @staticmethod
     def parseFile(filename: str, followIncludes: bool = False) -> 'Devicetree':
         """Parse a file and return a Devicetree object"""
         # pylint: disable=import-outside-toplevel,cyclic-import
         from pydevicetree.source import parseTree
         with open(filename, 'r') as f:
             contents = f.read()
-        pwd = os.path.dirname(filename) + "/"
-        return parseTree(contents, pwd, followIncludes)
+        dirname = os.path.dirname(filename)
+        if dirname != "":
+            dirname += "/"
+        return parseTree(contents, dirname, followIncludes)
 
     def all_nodes(self) -> Iterable[Node]:
         """Get an iterable over all nodes in the tree"""
         return self.child_nodes()
 
     def root(self) -> Node:
         """Get the root node of the tree"""
```

### Comparing `pydevicetree-0.0.8/pydevicetree/ast/property.py` & `pydevicetree-0.0.9/pydevicetree/ast/property.py`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/pydevicetree/ast/reference.py` & `pydevicetree-0.0.9/pydevicetree/ast/reference.py`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/pydevicetree/source/grammar.py` & `pydevicetree-0.0.9/pydevicetree/source/grammar.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,19 @@
 stringlist = p.delimitedList(string)
 node_path = p.Combine(p.Literal("/") + \
         p.delimitedList(node_name, delim="/", combine=True)).setResultsName("path") + \
         p.Optional(p.Literal("@").suppress() + unit_address("address"))
 path_reference = p.Literal("&{").suppress() + node_path + p.Literal("}").suppress()
 label_reference = p.Literal("&").suppress() + label
 reference = path_reference ^ label_reference
-directive = p.QuotedString(quoteChar="/", unquoteResults=False) + \
-        p.Optional(string ^ property_name ^ node_name ^ reference ^ \
-                (integer * 2)) + p.Literal(";").suppress()
+include_directive = p.Literal("/include/") + p.QuotedString(quoteChar='"')
+generic_directive = p.QuotedString(quoteChar="/", unquoteResults=False) + \
+        p.Optional(string ^ property_name ^ node_name ^ reference ^ (integer * 2)) + \
+        p.Literal(";").suppress()
+directive = include_directive ^ generic_directive
 
 operator = p.oneOf("~ ! * / + - << >> < <= > >= == != & ^ | && ||")
 arith_expr = p.Forward()
 ternary_element = arith_expr ^ integer
 ternary_expr = ternary_element + p.Literal("?") + ternary_element + p.Literal(":") + ternary_element
 arith_expr = p.nestedExpr(content=(p.OneOrMore(operator ^ integer) ^ ternary_expr))
```

### Comparing `pydevicetree-0.0.8/pydevicetree/source/parser.py` & `pydevicetree-0.0.9/pydevicetree/source/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,16 @@
                     e.option = pwd + e.option
 
                 with open(e.option, 'r') as f:
                     contents = f.read()
 
                 elements += parseElements(contents)
 
+                del elements[elements.asList().index(e)]
+
 def parseElements(dts, pwd="", followIncludes=False):
     """Parses a string into a list of elements"""
     elements = grammar.devicetree.parseString(dts, parseAll=True)
     parentNodes(elements)
     if followIncludes:
         recurseIncludeFiles(elements, pwd)
     return elements
```

### Comparing `pydevicetree-0.0.8/pydevicetree.egg-info/PKG-INFO` & `pydevicetree-0.0.9/pydevicetree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydevicetree
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library for parsing Devicetree Source v1
 Home-page: https://github.com/sifive/pydevicetree
 Author: Nathaniel Graff
 Author-email: nathaniel.graff@sifive.com
 License: UNKNOWN
 Description: # pydevicetree
```

### Comparing `pydevicetree-0.0.8/pydevicetree.egg-info/SOURCES.txt` & `pydevicetree-0.0.9/pydevicetree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/setup.py` & `pydevicetree-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setuptools.setup(
         name="pydevicetree",
-        version="0.0.8",
+        version="0.0.9",
         author="Nathaniel Graff",
         author_email="nathaniel.graff@sifive.com",
         description="A library for parsing Devicetree Source v1",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/sifive/pydevicetree",
         packages=setuptools.find_packages(),
```

### Comparing `pydevicetree-0.0.8/tests/devicetrees/sifive/e20.dts` & `pydevicetree-0.0.9/tests/devicetrees/sifive/e20.dts`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/devicetrees/sifive/e21.dts` & `pydevicetree-0.0.9/tests/devicetrees/sifive/e21.dts`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/devicetrees/sifive/e24.dts` & `pydevicetree-0.0.9/tests/devicetrees/sifive/e24.dts`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/devicetrees/sifive/e31.dts` & `pydevicetree-0.0.9/tests/devicetrees/sifive/e31.dts`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/devicetrees/sifive/e34.dts` & `pydevicetree-0.0.9/tests/devicetrees/sifive/e34.dts`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/devicetrees/sifive/e76.dts` & `pydevicetree-0.0.9/tests/devicetrees/sifive/e76.dts`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/devicetrees/sifive/e76mc.dts` & `pydevicetree-0.0.9/tests/devicetrees/sifive/e76mc.dts`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/devicetrees/sifive/s21.dts` & `pydevicetree-0.0.9/tests/devicetrees/sifive/s21.dts`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/devicetrees/sifive/s51.dts` & `pydevicetree-0.0.9/tests/devicetrees/sifive/s51.dts`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/devicetrees/sifive/s54.dts` & `pydevicetree-0.0.9/tests/devicetrees/sifive/s54.dts`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/devicetrees/sifive/s76.dts` & `pydevicetree-0.0.9/tests/devicetrees/sifive/s76.dts`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/devicetrees/sifive/s76mc.dts` & `pydevicetree-0.0.9/tests/devicetrees/sifive/s76mc.dts`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/devicetrees/sifive/u52.dts` & `pydevicetree-0.0.9/tests/devicetrees/sifive/u52.dts`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/devicetrees/sifive/u54.dts` & `pydevicetree-0.0.9/tests/devicetrees/sifive/u54.dts`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/devicetrees/sifive/u54mc.dts` & `pydevicetree-0.0.9/tests/devicetrees/sifive/u54mc.dts`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/devicetrees/sifive/u74.dts` & `pydevicetree-0.0.9/tests/devicetrees/sifive/u74.dts`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/devicetrees/sifive/u74mc.dts` & `pydevicetree-0.0.9/tests/devicetrees/sifive/u74mc.dts`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/test_devicetree.py` & `pydevicetree-0.0.9/tests/test_devicetree.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,18 @@
         self.assertEqual(type(soc), Node)
         self.assertEqual(len(soc.children), 1)
 
         delete_property = self.tree.get_by_path("/soc/delete-property")
         self.assertEqual(type(delete_property), Node)
         self.assertEqual(delete_property.get_field("delete-me"), None)
 
+    def test_include_directive(self):
+        tree = Devicetree.from_dts("/include/ \"foo.dtsi\"")
+        self.assertEqual(tree.directives[0].to_dts(), "/include/ \"foo.dtsi\"\n")
+
     def test_get_by_label(self):
         cpu0 = self.tree.get_by_label("cpu0")
         self.assertEqual(cpu0.name, "cpu")
         self.assertEqual(cpu0.address, 0)
         self.assertEqual(cpu0.get_field("compatible"), "riscv")
 
     def test_get_field(self):
```

### Comparing `pydevicetree-0.0.8/tests/test_exceptions.py` & `pydevicetree-0.0.9/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/test_full_trees.py` & `pydevicetree-0.0.9/tests/test_full_trees.py`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/test_grammar.py` & `pydevicetree-0.0.9/tests/test_grammar.py`

 * *Files identical despite different names*

### Comparing `pydevicetree-0.0.8/tests/test_overlay.py` & `pydevicetree-0.0.9/tests/test_overlay.py`

 * *Files identical despite different names*

