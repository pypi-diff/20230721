# Comparing `tmp/isogrids-0.0.1.tar.gz` & `tmp/isogrids-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isogrids-0.0.1.tar", last modified: Thu Jul 20 22:21:27 2023, max compression
+gzip compressed data, was "isogrids-0.0.2.tar", last modified: Thu Jul 20 22:36:31 2023, max compression
```

## Comparing `isogrids-0.0.1.tar` & `isogrids-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 22:21:27.813758 isogrids-0.0.1/
--rw-rw-r--   0 isaac     (1001) isaac     (1001)     1067 2023-07-20 21:36:59.000000 isogrids-0.0.1/LICENSE
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      766 2023-07-20 22:21:27.813758 isogrids-0.0.1/PKG-INFO
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      167 2023-07-20 22:21:00.000000 isogrids-0.0.1/README.md
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      671 2023-07-20 22:20:23.000000 isogrids-0.0.1/pyproject.toml
--rw-rw-r--   0 isaac     (1001) isaac     (1001)       38 2023-07-20 22:21:27.813758 isogrids-0.0.1/setup.cfg
-drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 22:21:27.813758 isogrids-0.0.1/src/
-drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 22:21:27.813758 isogrids-0.0.1/src/isogrids/
--rw-rw-r--   0 isaac     (1001) isaac     (1001)        0 2023-07-20 21:51:46.000000 isogrids-0.0.1/src/isogrids/__init__.py
--rw-rw-r--   0 isaac     (1001) isaac     (1001)       47 2023-07-13 20:48:01.000000 isogrids-0.0.1/src/isogrids/env.py
-drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 22:21:27.813758 isogrids-0.0.1/src/isogrids/environments/
-drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 22:21:27.813758 isogrids-0.0.1/src/isogrids/environments/house_env/
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      936 2023-07-20 20:10:36.000000 isogrids-0.0.1/src/isogrids/environments/house_env/build_houses.py
--rw-rw-r--   0 isaac     (1001) isaac     (1001)     1607 2023-07-20 16:34:31.000000 isogrids-0.0.1/src/isogrids/environments/house_env/house_furniture.py
--rw-rw-r--   0 isaac     (1001) isaac     (1001)    17828 2023-07-20 20:10:23.000000 isogrids-0.0.1/src/isogrids/environments/house_env/house_gen.py
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      703 2023-07-20 19:29:52.000000 isogrids-0.0.1/src/isogrids/environments/house_env/house_gen_timeout.py
--rw-rw-r--   0 isaac     (1001) isaac     (1001)     3221 2023-07-20 17:44:12.000000 isogrids-0.0.1/src/isogrids/environments/house_env/house_rooms.py
--rw-rw-r--   0 isaac     (1001) isaac     (1001)     2446 2023-07-20 19:14:35.000000 isogrids-0.0.1/src/isogrids/environments/house_env/plot_house_graph.py
-drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 22:21:27.813758 isogrids-0.0.1/src/isogrids.egg-info/
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      766 2023-07-20 22:21:27.000000 isogrids-0.0.1/src/isogrids.egg-info/PKG-INFO
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      541 2023-07-20 22:21:27.000000 isogrids-0.0.1/src/isogrids.egg-info/SOURCES.txt
--rw-rw-r--   0 isaac     (1001) isaac     (1001)        1 2023-07-20 22:21:27.000000 isogrids-0.0.1/src/isogrids.egg-info/dependency_links.txt
--rw-rw-r--   0 isaac     (1001) isaac     (1001)        9 2023-07-20 22:21:27.000000 isogrids-0.0.1/src/isogrids.egg-info/top_level.txt
+drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 22:36:31.720440 isogrids-0.0.2/
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)     1067 2023-07-20 21:36:59.000000 isogrids-0.0.2/LICENSE
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      760 2023-07-20 22:36:31.720440 isogrids-0.0.2/PKG-INFO
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      167 2023-07-20 22:21:00.000000 isogrids-0.0.2/README.md
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      665 2023-07-20 22:36:08.000000 isogrids-0.0.2/pyproject.toml
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)       38 2023-07-20 22:36:31.720440 isogrids-0.0.2/setup.cfg
+drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 22:36:31.720440 isogrids-0.0.2/src/
+drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 22:36:31.720440 isogrids-0.0.2/src/isogrids/
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)        0 2023-07-20 21:51:46.000000 isogrids-0.0.2/src/isogrids/__init__.py
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)       47 2023-07-13 20:48:01.000000 isogrids-0.0.2/src/isogrids/env.py
+drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 22:36:31.720440 isogrids-0.0.2/src/isogrids/environments/
+drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 22:36:31.720440 isogrids-0.0.2/src/isogrids/environments/house_env/
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      936 2023-07-20 20:10:36.000000 isogrids-0.0.2/src/isogrids/environments/house_env/build_houses.py
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)     1607 2023-07-20 16:34:31.000000 isogrids-0.0.2/src/isogrids/environments/house_env/house_furniture.py
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)    17828 2023-07-20 20:10:23.000000 isogrids-0.0.2/src/isogrids/environments/house_env/house_gen.py
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      703 2023-07-20 19:29:52.000000 isogrids-0.0.2/src/isogrids/environments/house_env/house_gen_timeout.py
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)     3221 2023-07-20 17:44:12.000000 isogrids-0.0.2/src/isogrids/environments/house_env/house_rooms.py
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)     2446 2023-07-20 19:14:35.000000 isogrids-0.0.2/src/isogrids/environments/house_env/plot_house_graph.py
+drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 22:36:31.720440 isogrids-0.0.2/src/isogrids.egg-info/
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      760 2023-07-20 22:36:31.000000 isogrids-0.0.2/src/isogrids.egg-info/PKG-INFO
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      541 2023-07-20 22:36:31.000000 isogrids-0.0.2/src/isogrids.egg-info/SOURCES.txt
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)        1 2023-07-20 22:36:31.000000 isogrids-0.0.2/src/isogrids.egg-info/dependency_links.txt
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)        9 2023-07-20 22:36:31.000000 isogrids-0.0.2/src/isogrids.egg-info/top_level.txt
```

### Comparing `isogrids-0.0.1/LICENSE` & `isogrids-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `isogrids-0.0.1/src/isogrids/environments/house_env/build_houses.py` & `isogrids-0.0.2/src/isogrids/environments/house_env/build_houses.py`

 * *Files identical despite different names*

### Comparing `isogrids-0.0.1/src/isogrids/environments/house_env/house_furniture.py` & `isogrids-0.0.2/src/isogrids/environments/house_env/house_furniture.py`

 * *Files identical despite different names*

### Comparing `isogrids-0.0.1/src/isogrids/environments/house_env/house_gen.py` & `isogrids-0.0.2/src/isogrids/environments/house_env/house_gen.py`

 * *Files identical despite different names*

### Comparing `isogrids-0.0.1/src/isogrids/environments/house_env/house_gen_timeout.py` & `isogrids-0.0.2/src/isogrids/environments/house_env/house_gen_timeout.py`

 * *Files identical despite different names*

### Comparing `isogrids-0.0.1/src/isogrids/environments/house_env/house_rooms.py` & `isogrids-0.0.2/src/isogrids/environments/house_env/house_rooms.py`

 * *Files identical despite different names*

### Comparing `isogrids-0.0.1/src/isogrids/environments/house_env/plot_house_graph.py` & `isogrids-0.0.2/src/isogrids/environments/house_env/plot_house_graph.py`

 * *Files identical despite different names*

### Comparing `isogrids-0.0.1/src/isogrids.egg-info/SOURCES.txt` & `isogrids-0.0.2/src/isogrids.egg-info/SOURCES.txt`

 * *Files identical despite different names*

