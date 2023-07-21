# Comparing `tmp/bec_scihub-0.13.2.tar.gz` & `tmp/bec_scihub-0.13.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_scihub-0.13.2.tar", last modified: Fri Jul 21 07:52:33 2023, max compression
+gzip compressed data, was "bec_scihub-0.13.3.tar", last modified: Fri Jul 21 15:13:10 2023, max compression
```

## Comparing `bec_scihub-0.13.2.tar` & `bec_scihub-0.13.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:52:33.152458 bec_scihub-0.13.2/
--rw-r--r--   0 root         (0) root         (0)      478 2023-07-21 07:52:33.152458 bec_scihub-0.13.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:52:33.152458 bec_scihub-0.13.2/bec_scihub.egg-info/
--rw-r--r--   0 root         (0) root         (0)      478 2023-07-21 07:52:33.000000 bec_scihub-0.13.2/bec_scihub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      521 2023-07-21 07:52:33.000000 bec_scihub-0.13.2/bec_scihub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 07:52:33.000000 bec_scihub-0.13.2/bec_scihub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-21 07:52:33.000000 bec_scihub-0.13.2/bec_scihub.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-21 07:52:33.000000 bec_scihub-0.13.2/bec_scihub.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-21 07:52:33.000000 bec_scihub-0.13.2/bec_scihub.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:52:33.150458 bec_scihub-0.13.2/scihub/
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-08 15:47:18.000000 bec_scihub-0.13.2/scihub/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:52:33.151458 bec_scihub-0.13.2/scihub/scibec/
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-04-24 15:23:42.000000 bec_scihub-0.13.2/scihub/scibec/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7654 2023-06-28 15:37:05.000000 bec_scihub-0.13.2/scihub/scibec/config_handler.py
--rw-rw-rw-   0 root         (0) root         (0)    15033 2023-06-28 12:41:01.000000 bec_scihub-0.13.2/scihub/scibec/scibec.py
--rw-rw-rw-   0 root         (0) root         (0)     4428 2023-06-28 12:41:01.000000 bec_scihub-0.13.2/scihub/scibec/scibec_connector.py
--rw-rw-rw-   0 root         (0) root         (0)     4126 2023-06-28 12:41:01.000000 bec_scihub-0.13.2/scihub/scibec/scibec_metadata_handler.py
--rw-rw-rw-   0 root         (0) root         (0)      880 2023-04-24 15:23:42.000000 bec_scihub-0.13.2/scihub/scibec/scibec_validator.py
--rw-rw-rw-   0 root         (0) root         (0)      902 2023-06-28 12:41:01.000000 bec_scihub-0.13.2/scihub/scihub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:52:33.151458 bec_scihub-0.13.2/scihub/scilog/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-04-24 19:02:27.000000 bec_scihub-0.13.2/scihub/scilog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3330 2023-06-28 12:41:01.000000 bec_scihub-0.13.2/scihub/scilog/scilog.py
--rw-r--r--   0 root         (0) root         (0)      538 2023-07-21 07:52:33.153458 bec_scihub-0.13.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      921 2023-07-08 15:47:18.000000 bec_scihub-0.13.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:13:10.162795 bec_scihub-0.13.3/
+-rw-r--r--   0 root         (0) root         (0)      478 2023-07-21 15:13:10.162795 bec_scihub-0.13.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:13:10.161795 bec_scihub-0.13.3/bec_scihub.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      478 2023-07-21 15:13:10.000000 bec_scihub-0.13.3/bec_scihub.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      521 2023-07-21 15:13:10.000000 bec_scihub-0.13.3/bec_scihub.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:13:10.000000 bec_scihub-0.13.3/bec_scihub.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-21 15:13:10.000000 bec_scihub-0.13.3/bec_scihub.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-07-21 15:13:10.000000 bec_scihub-0.13.3/bec_scihub.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-21 15:13:10.000000 bec_scihub-0.13.3/bec_scihub.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:13:10.159795 bec_scihub-0.13.3/scihub/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-08 15:33:35.000000 bec_scihub-0.13.3/scihub/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:13:10.160795 bec_scihub-0.13.3/scihub/scibec/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-19 08:14:59.000000 bec_scihub-0.13.3/scihub/scibec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7654 2023-06-28 10:41:58.000000 bec_scihub-0.13.3/scihub/scibec/config_handler.py
+-rw-r--r--   0 root         (0) root         (0)    15033 2023-06-28 10:41:58.000000 bec_scihub-0.13.3/scihub/scibec/scibec.py
+-rw-r--r--   0 root         (0) root         (0)     4428 2023-06-28 10:41:58.000000 bec_scihub-0.13.3/scihub/scibec/scibec_connector.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2023-06-28 10:41:58.000000 bec_scihub-0.13.3/scihub/scibec/scibec_metadata_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)      880 2023-06-19 08:14:59.000000 bec_scihub-0.13.3/scihub/scibec/scibec_validator.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-06-28 10:41:58.000000 bec_scihub-0.13.3/scihub/scihub.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:13:10.160795 bec_scihub-0.13.3/scihub/scilog/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-19 08:14:59.000000 bec_scihub-0.13.3/scihub/scilog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3330 2023-06-28 10:41:58.000000 bec_scihub-0.13.3/scihub/scilog/scilog.py
+-rw-r--r--   0 root         (0) root         (0)      538 2023-07-21 15:13:10.162795 bec_scihub-0.13.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      940 2023-07-21 15:12:28.000000 bec_scihub-0.13.3/setup.py
```

### Comparing `bec_scihub-0.13.2/bec_scihub.egg-info/SOURCES.txt` & `bec_scihub-0.13.3/bec_scihub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.13.2/scihub/scibec/config_handler.py` & `bec_scihub-0.13.3/scihub/scibec/config_handler.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.13.2/scihub/scibec/scibec.py` & `bec_scihub-0.13.3/scihub/scibec/scibec.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.13.2/scihub/scibec/scibec_connector.py` & `bec_scihub-0.13.3/scihub/scibec/scibec_connector.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.13.2/scihub/scibec/scibec_metadata_handler.py` & `bec_scihub-0.13.3/scihub/scibec/scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.13.2/scihub/scibec/scibec_validator.py` & `bec_scihub-0.13.3/scihub/scibec/scibec_validator.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.13.2/scihub/scihub.py` & `bec_scihub-0.13.3/scihub/scihub.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.13.2/scihub/scilog/scilog.py` & `bec_scihub-0.13.3/scihub/scilog/scilog.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.13.2/setup.cfg` & `bec_scihub-0.13.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.13.2/setup.py` & `bec_scihub-0.13.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 
 
 if __name__ == "__main__":
     setup(
         install_requires=["msgpack", "pyyaml", "fastjsonschema", "python-dotenv"],
         version=get_version(),
         entry_points={"console_scripts": ["bec-scihub = scihub:main"]},
-        extras_require={"dev": ["pytest", "pytest-random-order", "coverage"]},
+        extras_require={"dev": ["pytest", "pytest-random-order", "coverage", "black", "pylint"]},
     )
     local_deps = [utils]
     for dep in local_deps:
         subprocess.run(f"pip install -e {dep}", shell=True, check=True)
```

