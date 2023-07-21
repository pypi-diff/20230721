# Comparing `tmp/mypy-gpt-1.0.1.tar.gz` & `tmp/mypy-gpt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-gpt-1.0.1.tar", last modified: Fri Jul 21 19:02:12 2023, max compression
+gzip compressed data, was "mypy-gpt-1.0.2.tar", last modified: Fri Jul 21 19:12:59 2023, max compression
```

## Comparing `mypy-gpt-1.0.1.tar` & `mypy-gpt-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 19:02:12.579358 mypy-gpt-1.0.1/
--rw-rw-rw-   0        0        0    35184 2023-07-21 03:02:01.000000 mypy-gpt-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      313 2023-07-21 19:02:12.578358 mypy-gpt-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2181 2023-07-21 18:29:39.000000 mypy-gpt-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 19:02:12.557356 mypy-gpt-1.0.1/mypy_gpt/
--rw-rw-rw-   0        0        0        0 2023-07-21 18:55:16.000000 mypy-gpt-1.0.1/mypy_gpt/__init__.py
--rw-rw-rw-   0        0        0       33 2023-07-21 18:55:16.000000 mypy-gpt-1.0.1/mypy_gpt/__main__.py
--rw-rw-rw-   0        0        0     9926 2023-07-21 18:55:16.000000 mypy-gpt-1.0.1/mypy_gpt/mypygpt.py
-drwxrwxrwx   0        0        0        0 2023-07-21 19:02:12.577358 mypy-gpt-1.0.1/mypy_gpt.egg-info/
--rw-rw-rw-   0        0        0      313 2023-07-21 19:02:12.000000 mypy-gpt-1.0.1/mypy_gpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-07-21 19:02:12.000000 mypy-gpt-1.0.1/mypy_gpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 19:02:12.000000 mypy-gpt-1.0.1/mypy_gpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-21 19:02:12.000000 mypy-gpt-1.0.1/mypy_gpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 19:02:12.000000 mypy-gpt-1.0.1/mypy_gpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 19:02:12.579358 mypy-gpt-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      748 2023-07-21 19:02:07.000000 mypy-gpt-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 19:12:59.675932 mypy-gpt-1.0.2/
+-rw-rw-rw-   0        0        0    35184 2023-07-21 03:02:01.000000 mypy-gpt-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-07-21 19:08:18.000000 mypy-gpt-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      311 2023-07-21 19:12:59.675425 mypy-gpt-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2181 2023-07-21 18:29:39.000000 mypy-gpt-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 19:12:59.661804 mypy-gpt-1.0.2/mypy_gpt/
+-rw-rw-rw-   0        0        0        0 2023-07-21 18:55:16.000000 mypy-gpt-1.0.2/mypy_gpt/__init__.py
+-rw-rw-rw-   0        0        0       33 2023-07-21 18:55:16.000000 mypy-gpt-1.0.2/mypy_gpt/__main__.py
+-rw-rw-rw-   0        0        0     9926 2023-07-21 18:55:16.000000 mypy-gpt-1.0.2/mypy_gpt/mypygpt.py
+drwxrwxrwx   0        0        0        0 2023-07-21 19:12:59.674371 mypy-gpt-1.0.2/mypy_gpt.egg-info/
+-rw-rw-rw-   0        0        0      311 2023-07-21 19:12:59.000000 mypy-gpt-1.0.2/mypy_gpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-07-21 19:12:59.000000 mypy-gpt-1.0.2/mypy_gpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 19:12:59.000000 mypy-gpt-1.0.2/mypy_gpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-21 19:12:59.000000 mypy-gpt-1.0.2/mypy_gpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 19:12:59.000000 mypy-gpt-1.0.2/mypy_gpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       36 2023-07-21 18:56:44.000000 mypy-gpt-1.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 19:12:59.675932 mypy-gpt-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2023-07-21 19:12:09.000000 mypy-gpt-1.0.2/setup.py
```

### Comparing `mypy-gpt-1.0.1/LICENSE` & `mypy-gpt-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-gpt-1.0.1/README.md` & `mypy-gpt-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mypy-gpt-1.0.1/mypy_gpt/mypygpt.py` & `mypy-gpt-1.0.2/mypy_gpt/mypygpt.py`

 * *Files identical despite different names*

