# Comparing `tmp/pyhidra-0.5.1.tar.gz` & `tmp/pyhidra-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhidra-0.5.1.tar", last modified: Mon May 22 17:49:40 2023, max compression
+gzip compressed data, was "pyhidra-0.5.2.tar", last modified: Fri Jul 21 18:04:01 2023, max compression
```

## Comparing `pyhidra-0.5.1.tar` & `pyhidra-0.5.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:40.056700 pyhidra-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-22 17:49:27.000000 pyhidra-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-22 17:49:27.000000 pyhidra-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-05-22 17:49:40.056700 pyhidra-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-05-22 17:49:27.000000 pyhidra-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:40.036700 pyhidra-0.5.1/pyhidra/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/install_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:40.040700 pyhidra-0.5.1/pyhidra/java/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:40.044700 pyhidra-0.5.1/pyhidra/java/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/plugin/PyScriptProvider.java
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/plugin/PyhidraPlugin.java
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/plugin/PythonFieldExposer.java
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/plugin/completions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:40.044700 pyhidra-0.5.1/pyhidra/java/plugin/ghidra_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/plugin/ghidra_scripts/PyhidraBasics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:40.044700 pyhidra-0.5.1/pyhidra/java/plugin/interpreter/
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/plugin/interpreter/CancelAction.java
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/plugin/interpreter/InterpreterGhidraScript.java
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/plugin/interpreter/InterpreterTaskMonitor.java
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/plugin/interpreter/PyhidraInterpreterConnection.java
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/plugin/interpreter/RestartAction.java
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:40.056700 pyhidra-0.5.1/pyhidra/java/property/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/property/AbstractJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/property/BooleanJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/property/ByteJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/property/CharacterJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/property/DoubleJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/property/FloatJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/property/IntegerJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/property/JavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/property/JavaPropertyFactory.java
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/property/LongJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/property/ObjectJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/property/PropertyUtils.java
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/java/property/ShortJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/javac.py
--rw-r--r--   0 runner    (1001) docker     (123)    15281 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-22 17:49:27.000000 pyhidra-0.5.1/pyhidra/win_shortcut.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:40.040700 pyhidra-0.5.1/pyhidra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-05-22 17:49:39.000000 pyhidra-0.5.1/pyhidra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-22 17:49:40.000000 pyhidra-0.5.1/pyhidra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:49:39.000000 pyhidra-0.5.1/pyhidra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-22 17:49:39.000000 pyhidra-0.5.1/pyhidra.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:49:39.000000 pyhidra-0.5.1/pyhidra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-22 17:49:39.000000 pyhidra-0.5.1/pyhidra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 17:49:39.000000 pyhidra-0.5.1/pyhidra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-22 17:49:40.056700 pyhidra-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-22 17:49:27.000000 pyhidra-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:40.056700 pyhidra-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-22 17:49:27.000000 pyhidra-0.5.1/tests/test_argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-05-22 17:49:27.000000 pyhidra-0.5.1/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:04:01.689437 pyhidra-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-21 18:03:47.000000 pyhidra-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-21 18:03:47.000000 pyhidra-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-07-21 18:04:01.689437 pyhidra-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-07-21 18:03:47.000000 pyhidra-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:04:01.669436 pyhidra-0.5.2/pyhidra/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/install_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:04:01.673436 pyhidra-0.5.2/pyhidra/java/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:04:01.673436 pyhidra-0.5.2/pyhidra/java/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/plugin/PyScriptProvider.java
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/plugin/PyhidraPlugin.java
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/plugin/PythonFieldExposer.java
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/plugin/completions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:04:01.677436 pyhidra-0.5.2/pyhidra/java/plugin/ghidra_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/plugin/ghidra_scripts/PyhidraBasics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:04:01.677436 pyhidra-0.5.2/pyhidra/java/plugin/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/plugin/interpreter/CancelAction.java
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/plugin/interpreter/InterpreterGhidraScript.java
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/plugin/interpreter/InterpreterTaskMonitor.java
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/plugin/interpreter/PyhidraInterpreterConnection.java
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/plugin/interpreter/RestartAction.java
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:04:01.689437 pyhidra-0.5.2/pyhidra/java/property/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/property/AbstractJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/property/BooleanJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/property/ByteJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/property/CharacterJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/property/DoubleJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/property/FloatJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/property/IntegerJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/property/JavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/property/JavaPropertyFactory.java
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/property/LongJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/property/ObjectJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/property/PropertyUtils.java
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/java/property/ShortJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/javac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15281 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-21 18:03:47.000000 pyhidra-0.5.2/pyhidra/win_shortcut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:04:01.673436 pyhidra-0.5.2/pyhidra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-07-21 18:04:01.000000 pyhidra-0.5.2/pyhidra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-21 18:04:01.000000 pyhidra-0.5.2/pyhidra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 18:04:01.000000 pyhidra-0.5.2/pyhidra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-21 18:04:01.000000 pyhidra-0.5.2/pyhidra.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 18:04:01.000000 pyhidra-0.5.2/pyhidra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-21 18:04:01.000000 pyhidra-0.5.2/pyhidra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 18:04:01.000000 pyhidra-0.5.2/pyhidra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-21 18:04:01.689437 pyhidra-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-21 18:03:47.000000 pyhidra-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:04:01.689437 pyhidra-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-21 18:03:47.000000 pyhidra-0.5.2/tests/test_argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-07-21 18:03:47.000000 pyhidra-0.5.2/tests/test_core.py
```

### Comparing `pyhidra-0.5.1/LICENSE` & `pyhidra-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/PKG-INFO` & `pyhidra-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhidra
-Version: 0.5.1
+Version: 0.5.2
 Summary: Native CPython for Ghidra
 Home-page: https://github.com/Defense-Cyber-Crime-Center/pyhidra
 Author: DC3
 Author-email: dcci@dc3.mil
 License: MIT
 Keywords: ghidra
 Platform: any
```

### Comparing `pyhidra-0.5.1/README.md` & `pyhidra-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/__main__.py` & `pyhidra-0.5.2/pyhidra/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/core.py` & `pyhidra-0.5.2/pyhidra/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         return service.getLanguage(LanguageID(id))
     except LanguageNotFoundException:
         # suppress the java exception
         pass
     raise ValueError("Invalid Language ID: "+id)
 
 
-def _get_compiler_spec(lang: "Language", id: str) -> "CompilerSpec":
+def _get_compiler_spec(lang: "Language", id: str = None) -> "CompilerSpec":
     if id is None:
         return lang.getDefaultCompilerSpec()
     from ghidra.program.model.lang import CompilerSpecID, CompilerSpecNotFoundException
     try:
         return lang.getCompilerSpecByID(CompilerSpecID(id))
     except CompilerSpecNotFoundException:
         # suppress the java exception
@@ -80,18 +80,27 @@
                 program = project.openProgram("/", binary_path.name, False)
     except IOException:
         project = GhidraProject.createProject(project_location, project_name, False)
 
     if binary_path is not None and program is None:
         if language is None:
             program = project.importProgram(binary_path)
+            if program is None:
+                raise RuntimeError(f"Ghidra failed to import '{binary_path}'. Try providing a language manually.")
         else:
             lang = _get_language(language)
             comp = _get_compiler_spec(lang, compiler)
             program = project.importProgram(binary_path, lang, comp)
+            if program is None:
+                message = f"Ghidra failed to import '{binary_path}'. "
+                if compiler:
+                    message += f"The provided language/compiler pair ({language} / {compiler}) may be invalid."
+                else:
+                    message += f"The provided language ({language}) may be invalid."
+                raise ValueError(message)
         project.saveAs(program, "/", program.getName(), True)
 
     return project, program
 
 
 def _setup_script(project: "GhidraProject", program: "Program"):
     from pyhidra.script import PyGhidraScript
```

### Comparing `pyhidra-0.5.1/pyhidra/gui.py` & `pyhidra-0.5.2/pyhidra/gui.py`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/java/plugin/PyScriptProvider.java` & `pyhidra-0.5.2/pyhidra/java/plugin/PyScriptProvider.java`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/java/plugin/PyhidraPlugin.java` & `pyhidra-0.5.2/pyhidra/java/plugin/PyhidraPlugin.java`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/java/plugin/PythonFieldExposer.java` & `pyhidra-0.5.2/pyhidra/java/plugin/PythonFieldExposer.java`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/java/plugin/completions.py` & `pyhidra-0.5.2/pyhidra/java/plugin/completions.py`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/java/plugin/ghidra_scripts/PyhidraBasics.py` & `pyhidra-0.5.2/pyhidra/java/plugin/ghidra_scripts/PyhidraBasics.py`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/java/plugin/interpreter/CancelAction.java` & `pyhidra-0.5.2/pyhidra/java/plugin/interpreter/CancelAction.java`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/java/plugin/interpreter/InterpreterGhidraScript.java` & `pyhidra-0.5.2/pyhidra/java/plugin/interpreter/InterpreterGhidraScript.java`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/java/plugin/interpreter/InterpreterTaskMonitor.java` & `pyhidra-0.5.2/pyhidra/java/plugin/interpreter/InterpreterTaskMonitor.java`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/java/plugin/interpreter/PyhidraInterpreterConnection.java` & `pyhidra-0.5.2/pyhidra/java/plugin/interpreter/PyhidraInterpreterConnection.java`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/java/plugin/interpreter/RestartAction.java` & `pyhidra-0.5.2/pyhidra/java/plugin/interpreter/RestartAction.java`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/java/plugin/plugin.py` & `pyhidra-0.5.2/pyhidra/java/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/java/property/AbstractJavaProperty.java` & `pyhidra-0.5.2/pyhidra/java/property/AbstractJavaProperty.java`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/java/property/JavaPropertyFactory.java` & `pyhidra-0.5.2/pyhidra/java/property/JavaPropertyFactory.java`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/java/property/PropertyUtils.java` & `pyhidra-0.5.2/pyhidra/java/property/PropertyUtils.java`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/javac.py` & `pyhidra-0.5.2/pyhidra/javac.py`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/launcher.py` & `pyhidra-0.5.2/pyhidra/launcher.py`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/properties.py` & `pyhidra-0.5.2/pyhidra/properties.py`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/script.py` & `pyhidra-0.5.2/pyhidra/script.py`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/version.py` & `pyhidra-0.5.2/pyhidra/version.py`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra/win_shortcut.py` & `pyhidra-0.5.2/pyhidra/win_shortcut.py`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/pyhidra.egg-info/PKG-INFO` & `pyhidra-0.5.2/pyhidra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhidra
-Version: 0.5.1
+Version: 0.5.2
 Summary: Native CPython for Ghidra
 Home-page: https://github.com/Defense-Cyber-Crime-Center/pyhidra
 Author: DC3
 Author-email: dcci@dc3.mil
 License: MIT
 Keywords: ghidra
 Platform: any
```

### Comparing `pyhidra-0.5.1/pyhidra.egg-info/SOURCES.txt` & `pyhidra-0.5.2/pyhidra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/setup.cfg` & `pyhidra-0.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/tests/test_argparser.py` & `pyhidra-0.5.2/tests/test_argparser.py`

 * *Files identical despite different names*

### Comparing `pyhidra-0.5.1/tests/test_core.py` & `pyhidra-0.5.2/tests/test_core.py`

 * *Files identical despite different names*

