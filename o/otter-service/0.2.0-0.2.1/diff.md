# Comparing `tmp/otter_service-0.2.0.tar.gz` & `tmp/otter_service-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otter_service-0.2.0.tar", last modified: Thu Jul 20 18:05:03 2023, max compression
+gzip compressed data, was "otter_service-0.2.1.tar", last modified: Fri Jul 21 14:52:20 2023, max compression
```

## Comparing `otter_service-0.2.0.tar` & `otter_service-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-20 18:05:03.579800 otter_service-0.2.0/
--rw-r--r--   0 sean       (501) staff       (20)     1498 2021-10-24 00:07:22.000000 otter_service-0.2.0/LICENSE
--rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-20 18:05:03.580074 otter_service-0.2.0/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)     7704 2022-07-15 16:10:04.000000 otter_service-0.2.0/README.md
--rw-r--r--   0 sean       (501) staff       (20)      103 2023-07-20 15:40:45.000000 otter_service-0.2.0/pyproject.toml
--rw-r--r--   0 sean       (501) staff       (20)      786 2023-07-20 18:05:03.581045 otter_service-0.2.0/setup.cfg
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-20 18:05:03.564402 otter_service-0.2.0/src/
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-20 18:05:03.571563 otter_service-0.2.0/src/otter_service/
--rw-r--r--   0 sean       (501) staff       (20)       22 2023-07-20 17:59:45.000000 otter_service-0.2.0/src/otter_service/__init__.py
--rw-r--r--   0 sean       (501) staff       (20)     1753 2022-07-14 01:10:23.000000 otter_service-0.2.0/src/otter_service/access_sops_keys.py
--rw-r--r--   0 sean       (501) staff       (20)     1035 2022-09-01 01:54:36.000000 otter_service-0.2.0/src/otter_service/firestore-test.py
--rw-r--r--   0 sean       (501) staff       (20)     4985 2023-07-20 17:50:18.000000 otter_service-0.2.0/src/otter_service/grade_assignment.py
--rw-r--r--   0 sean       (501) staff       (20)    19879 2023-07-20 17:58:21.000000 otter_service-0.2.0/src/otter_service/otter_nb.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-20 18:05:03.575688 otter_service-0.2.0/src/otter_service/secrets/
--rw-r--r--   0 sean       (501) staff       (20)      983 2023-07-20 17:04:07.000000 otter_service-0.2.0/src/otter_service/secrets/gh_key.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1229 2022-06-11 00:39:08.000000 otter_service-0.2.0/src/otter_service/secrets/gke_key.yaml
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-20 18:05:03.574597 otter_service-0.2.0/src/otter_service.egg-info/
--rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-20 18:05:03.000000 otter_service-0.2.0/src/otter_service.egg-info/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)      584 2023-07-20 18:05:03.000000 otter_service-0.2.0/src/otter_service.egg-info/SOURCES.txt
--rw-r--r--   0 sean       (501) staff       (20)        1 2023-07-20 18:05:03.000000 otter_service-0.2.0/src/otter_service.egg-info/dependency_links.txt
--rw-r--r--   0 sean       (501) staff       (20)       62 2023-07-20 18:05:03.000000 otter_service-0.2.0/src/otter_service.egg-info/entry_points.txt
--rw-r--r--   0 sean       (501) staff       (20)       14 2023-07-20 18:05:03.000000 otter_service-0.2.0/src/otter_service.egg-info/top_level.txt
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-20 18:05:03.578943 otter_service-0.2.0/tests/
--rw-r--r--   0 sean       (501) staff       (20)      895 2022-06-18 01:43:56.000000 otter_service-0.2.0/tests/test_access_sops_keys.py
--rw-r--r--   0 sean       (501) staff       (20)     1416 2023-07-20 17:37:25.000000 otter_service-0.2.0/tests/test_grade_assignment.py
--rw-r--r--   0 sean       (501) staff       (20)     2090 2023-07-20 17:54:37.000000 otter_service-0.2.0/tests/test_otter_nb.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 14:52:20.473463 otter_service-0.2.1/
+-rw-r--r--   0 sean       (501) staff       (20)     1498 2021-10-24 00:07:22.000000 otter_service-0.2.1/LICENSE
+-rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-21 14:52:20.473740 otter_service-0.2.1/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)     7704 2022-07-15 16:10:04.000000 otter_service-0.2.1/README.md
+-rw-r--r--   0 sean       (501) staff       (20)      103 2023-07-20 15:40:45.000000 otter_service-0.2.1/pyproject.toml
+-rw-r--r--   0 sean       (501) staff       (20)      786 2023-07-21 14:52:20.474680 otter_service-0.2.1/setup.cfg
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 14:52:20.458041 otter_service-0.2.1/src/
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 14:52:20.463875 otter_service-0.2.1/src/otter_service/
+-rw-r--r--   0 sean       (501) staff       (20)       22 2023-07-21 14:51:32.000000 otter_service-0.2.1/src/otter_service/__init__.py
+-rw-r--r--   0 sean       (501) staff       (20)     1722 2023-07-21 00:46:58.000000 otter_service-0.2.1/src/otter_service/access_sops_keys.py
+-rw-r--r--   0 sean       (501) staff       (20)     1035 2022-09-01 01:54:36.000000 otter_service-0.2.1/src/otter_service/firestore-test.py
+-rw-r--r--   0 sean       (501) staff       (20)     4985 2023-07-20 18:36:10.000000 otter_service-0.2.1/src/otter_service/grade_assignment.py
+-rw-r--r--   0 sean       (501) staff       (20)    19879 2023-07-20 18:36:10.000000 otter_service-0.2.1/src/otter_service/otter_nb.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 14:52:20.468308 otter_service-0.2.1/src/otter_service/secrets/
+-rw-r--r--   0 sean       (501) staff       (20)      983 2023-07-20 18:36:10.000000 otter_service-0.2.1/src/otter_service/secrets/gh_key.yaml
+-rw-r--r--   0 sean       (501) staff       (20)     1229 2022-06-11 00:39:08.000000 otter_service-0.2.1/src/otter_service/secrets/gke_key.yaml
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 14:52:20.466970 otter_service-0.2.1/src/otter_service.egg-info/
+-rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-21 14:52:20.000000 otter_service-0.2.1/src/otter_service.egg-info/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)      584 2023-07-21 14:52:20.000000 otter_service-0.2.1/src/otter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 sean       (501) staff       (20)        1 2023-07-21 14:52:20.000000 otter_service-0.2.1/src/otter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 sean       (501) staff       (20)       62 2023-07-21 14:52:20.000000 otter_service-0.2.1/src/otter_service.egg-info/entry_points.txt
+-rw-r--r--   0 sean       (501) staff       (20)       14 2023-07-21 14:52:20.000000 otter_service-0.2.1/src/otter_service.egg-info/top_level.txt
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 14:52:20.472425 otter_service-0.2.1/tests/
+-rw-r--r--   0 sean       (501) staff       (20)      895 2022-06-18 01:43:56.000000 otter_service-0.2.1/tests/test_access_sops_keys.py
+-rw-r--r--   0 sean       (501) staff       (20)     1416 2023-07-20 18:36:10.000000 otter_service-0.2.1/tests/test_grade_assignment.py
+-rw-r--r--   0 sean       (501) staff       (20)     2090 2023-07-20 18:36:10.000000 otter_service-0.2.1/tests/test_otter_nb.py
```

### Comparing `otter_service-0.2.0/LICENSE` & `otter_service-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.0/PKG-INFO` & `otter_service-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter_service
-Version: 0.2.0
+Version: 0.2.1
 Summary: Grading Service for Edx 8x courses
 Home-page: https://github.com/data-8/otter-service
 Author: Vincent Su and Sean Morris
 Author-email: sean.smorris@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `otter_service-0.2.0/README.md` & `otter_service-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.0/setup.cfg` & `otter_service-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.0/src/otter_service/access_sops_keys.py` & `otter_service-0.2.1/src/otter_service/access_sops_keys.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import subprocess
-from pydantic import NoneBytes
 import yaml
 
 
 def get(key_name, sops_path=None, secrets_file=None) -> str:
     """
     This method first tries to decrypt sops file and then tries the
     environment. it will return an Exception if the key is not found
```

### Comparing `otter_service-0.2.0/src/otter_service/firestore-test.py` & `otter_service-0.2.1/src/otter_service/firestore-test.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.0/src/otter_service/grade_assignment.py` & `otter_service-0.2.1/src/otter_service/grade_assignment.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.0/src/otter_service/otter_nb.py` & `otter_service-0.2.1/src/otter_service/otter_nb.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.0/src/otter_service/secrets/gh_key.yaml` & `otter_service-0.2.1/src/otter_service/secrets/gh_key.yaml`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.0/src/otter_service/secrets/gke_key.yaml` & `otter_service-0.2.1/src/otter_service/secrets/gke_key.yaml`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.0/src/otter_service.egg-info/PKG-INFO` & `otter_service-0.2.1/src/otter_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-service
-Version: 0.2.0
+Version: 0.2.1
 Summary: Grading Service for Edx 8x courses
 Home-page: https://github.com/data-8/otter-service
 Author: Vincent Su and Sean Morris
 Author-email: sean.smorris@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `otter_service-0.2.0/src/otter_service.egg-info/SOURCES.txt` & `otter_service-0.2.1/src/otter_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.0/tests/test_access_sops_keys.py` & `otter_service-0.2.1/tests/test_access_sops_keys.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.0/tests/test_grade_assignment.py` & `otter_service-0.2.1/tests/test_grade_assignment.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.0/tests/test_otter_nb.py` & `otter_service-0.2.1/tests/test_otter_nb.py`

 * *Files identical despite different names*

