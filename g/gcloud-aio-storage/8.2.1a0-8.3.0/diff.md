# Comparing `tmp/gcloud_aio_storage-8.2.1a0.tar.gz` & `tmp/gcloud_aio_storage-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcloud_aio_storage-8.2.1a0.tar", max compression
+gzip compressed data, was "gcloud_aio_storage-8.3.0.tar", max compression
```

## Comparing `gcloud_aio_storage-8.2.1a0.tar` & `gcloud_aio_storage-8.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-05-23 16:55:11.370564 gcloud_aio_storage-8.2.1a0/LICENSE
--rw-r--r--   0        0        0     1284 2023-05-23 16:55:11.370564 gcloud_aio_storage-8.2.1a0/README.rst
--rw-r--r--   0        0        0      212 2023-05-23 16:55:11.370564 gcloud_aio_storage-8.2.1a0/gcloud/__init__.py
--rw-r--r--   0        0        0      212 2023-05-23 16:55:11.370564 gcloud_aio_storage-8.2.1a0/gcloud/aio/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 16:55:11.370564 gcloud_aio_storage-8.2.1a0/gcloud/aio/py.typed
--rw-r--r--   0        0        0     5560 2023-05-23 16:55:11.370564 gcloud_aio_storage-8.2.1a0/gcloud/aio/storage/__init__.py
--rw-r--r--   0        0        0     7396 2023-05-23 16:55:11.370564 gcloud_aio_storage-8.2.1a0/gcloud/aio/storage/blob.py
--rw-r--r--   0        0        0     2787 2023-05-23 16:55:11.370564 gcloud_aio_storage-8.2.1a0/gcloud/aio/storage/bucket.py
--rw-r--r--   0        0        0       70 2023-05-23 16:55:11.370564 gcloud_aio_storage-8.2.1a0/gcloud/aio/storage/constants.py
--rw-r--r--   0        0        0        0 2023-05-23 16:55:11.370564 gcloud_aio_storage-8.2.1a0/gcloud/aio/storage/py.typed
--rw-r--r--   0        0        0    29008 2023-05-23 16:55:11.370564 gcloud_aio_storage-8.2.1a0/gcloud/aio/storage/storage.py
--rw-r--r--   0        0        0        0 2023-05-23 16:55:11.370564 gcloud_aio_storage-8.2.1a0/gcloud/py.typed
--rw-r--r--   0        0        0     1102 2023-05-23 16:55:11.370564 gcloud_aio_storage-8.2.1a0/pyproject.toml
--rw-r--r--   0        0        0     2393 1970-01-01 00:00:00.000000 gcloud_aio_storage-8.2.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-21 16:35:25.743663 gcloud_aio_storage-8.3.0/LICENSE
+-rw-r--r--   0        0        0     1284 2023-07-21 16:35:25.743663 gcloud_aio_storage-8.3.0/README.rst
+-rw-r--r--   0        0        0      212 2023-07-21 16:35:25.743663 gcloud_aio_storage-8.3.0/gcloud/__init__.py
+-rw-r--r--   0        0        0      212 2023-07-21 16:35:25.743663 gcloud_aio_storage-8.3.0/gcloud/aio/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:35:25.743663 gcloud_aio_storage-8.3.0/gcloud/aio/py.typed
+-rw-r--r--   0        0        0     5560 2023-07-21 16:35:25.743663 gcloud_aio_storage-8.3.0/gcloud/aio/storage/__init__.py
+-rw-r--r--   0        0        0     7396 2023-07-21 16:35:25.743663 gcloud_aio_storage-8.3.0/gcloud/aio/storage/blob.py
+-rw-r--r--   0        0        0     2787 2023-07-21 16:35:25.743663 gcloud_aio_storage-8.3.0/gcloud/aio/storage/bucket.py
+-rw-r--r--   0        0        0       70 2023-07-21 16:35:25.743663 gcloud_aio_storage-8.3.0/gcloud/aio/storage/constants.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:35:25.743663 gcloud_aio_storage-8.3.0/gcloud/aio/storage/py.typed
+-rw-r--r--   0        0        0    29008 2023-07-21 16:35:25.743663 gcloud_aio_storage-8.3.0/gcloud/aio/storage/storage.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:35:25.743663 gcloud_aio_storage-8.3.0/gcloud/py.typed
+-rw-r--r--   0        0        0     1100 2023-07-21 16:35:25.743663 gcloud_aio_storage-8.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2391 1970-01-01 00:00:00.000000 gcloud_aio_storage-8.3.0/PKG-INFO
```

### Comparing `gcloud_aio_storage-8.2.1a0/LICENSE` & `gcloud_aio_storage-8.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gcloud_aio_storage-8.2.1a0/README.rst` & `gcloud_aio_storage-8.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `gcloud_aio_storage-8.2.1a0/gcloud/aio/storage/__init__.py` & `gcloud_aio_storage-8.3.0/gcloud/aio/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `gcloud_aio_storage-8.2.1a0/gcloud/aio/storage/blob.py` & `gcloud_aio_storage-8.3.0/gcloud/aio/storage/blob.py`

 * *Files identical despite different names*

### Comparing `gcloud_aio_storage-8.2.1a0/gcloud/aio/storage/bucket.py` & `gcloud_aio_storage-8.3.0/gcloud/aio/storage/bucket.py`

 * *Files identical despite different names*

### Comparing `gcloud_aio_storage-8.2.1a0/gcloud/aio/storage/storage.py` & `gcloud_aio_storage-8.3.0/gcloud/aio/storage/storage.py`

 * *Files identical despite different names*

### Comparing `gcloud_aio_storage-8.2.1a0/pyproject.toml` & `gcloud_aio_storage-8.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gcloud-aio-storage"
-version = "8.2.1a0"
+version = "8.3.0"
 description = "Python Client for Google Cloud Storage"
 readme = "README.rst"
 
 repository = "https://github.com/talkiq/gcloud-aio"
 authors = ["Vi Engineering <voiceai-eng@dialpad.com>"]
 license = "MIT"
```

### Comparing `gcloud_aio_storage-8.2.1a0/PKG-INFO` & `gcloud_aio_storage-8.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcloud-aio-storage
-Version: 8.2.1a0
+Version: 8.3.0
 Summary: Python Client for Google Cloud Storage
 Home-page: https://github.com/talkiq/gcloud-aio
 License: MIT
 Author: Vi Engineering
 Author-email: voiceai-eng@dialpad.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

