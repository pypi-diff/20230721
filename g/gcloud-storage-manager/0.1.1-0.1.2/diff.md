# Comparing `tmp/gcloud-storage-manager-0.1.1.tar.gz` & `tmp/gcloud-storage-manager-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcloud-storage-manager-0.1.1.tar", last modified: Fri Jul 21 03:45:50 2023, max compression
+gzip compressed data, was "gcloud-storage-manager-0.1.2.tar", last modified: Fri Jul 21 04:18:09 2023, max compression
```

## Comparing `gcloud-storage-manager-0.1.1.tar` & `gcloud-storage-manager-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 03:45:50.488035 gcloud-storage-manager-0.1.1/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1069 2023-06-26 15:50:43.000000 gcloud-storage-manager-0.1.1/LICENSE
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      461 2023-07-21 03:45:50.488035 gcloud-storage-manager-0.1.1/PKG-INFO
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      993 2023-07-21 03:37:53.000000 gcloud-storage-manager-0.1.1/README.md
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 03:45:50.484034 gcloud-storage-manager-0.1.1/gcloud_storage_manager/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      191 2023-06-26 15:40:23.000000 gcloud-storage-manager-0.1.1/gcloud_storage_manager/__init__.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      913 2023-07-21 03:29:32.000000 gcloud-storage-manager-0.1.1/gcloud_storage_manager/base.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2760 2023-07-21 03:37:53.000000 gcloud-storage-manager-0.1.1/gcloud_storage_manager/download.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      137 2023-06-26 15:23:45.000000 gcloud-storage-manager-0.1.1/gcloud_storage_manager/std_logging.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     3578 2023-07-21 03:42:10.000000 gcloud-storage-manager-0.1.1/gcloud_storage_manager/upload.py
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 03:45:50.488035 gcloud-storage-manager-0.1.1/gcloud_storage_manager.egg-info/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      461 2023-07-21 03:45:50.000000 gcloud-storage-manager-0.1.1/gcloud_storage_manager.egg-info/PKG-INFO
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      444 2023-07-21 03:45:50.000000 gcloud-storage-manager-0.1.1/gcloud_storage_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        1 2023-07-21 03:45:50.000000 gcloud-storage-manager-0.1.1/gcloud_storage_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       29 2023-07-21 03:45:50.000000 gcloud-storage-manager-0.1.1/gcloud_storage_manager.egg-info/top_level.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       38 2023-07-21 03:45:50.488035 gcloud-storage-manager-0.1.1/setup.cfg
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      614 2023-07-21 03:45:40.000000 gcloud-storage-manager-0.1.1/setup.py
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 03:45:50.488035 gcloud-storage-manager-0.1.1/tests/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-26 15:31:54.000000 gcloud-storage-manager-0.1.1/tests/__init__.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     4057 2023-07-21 03:37:59.000000 gcloud-storage-manager-0.1.1/tests/test_download.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2901 2023-07-21 03:41:59.000000 gcloud-storage-manager-0.1.1/tests/test_upload.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 04:18:09.980633 gcloud-storage-manager-0.1.2/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1069 2023-06-26 15:50:43.000000 gcloud-storage-manager-0.1.2/LICENSE
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      461 2023-07-21 04:18:09.980633 gcloud-storage-manager-0.1.2/PKG-INFO
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      997 2023-07-21 03:46:57.000000 gcloud-storage-manager-0.1.2/README.md
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 04:18:09.976633 gcloud-storage-manager-0.1.2/gcloud_storage_manager/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      191 2023-06-26 15:40:23.000000 gcloud-storage-manager-0.1.2/gcloud_storage_manager/__init__.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      913 2023-07-21 03:29:32.000000 gcloud-storage-manager-0.1.2/gcloud_storage_manager/base.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2829 2023-07-21 04:17:41.000000 gcloud-storage-manager-0.1.2/gcloud_storage_manager/download.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      137 2023-06-26 15:23:45.000000 gcloud-storage-manager-0.1.2/gcloud_storage_manager/std_logging.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     3643 2023-07-21 04:16:50.000000 gcloud-storage-manager-0.1.2/gcloud_storage_manager/upload.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 04:18:09.976633 gcloud-storage-manager-0.1.2/gcloud_storage_manager.egg-info/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      461 2023-07-21 04:18:09.000000 gcloud-storage-manager-0.1.2/gcloud_storage_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      444 2023-07-21 04:18:09.000000 gcloud-storage-manager-0.1.2/gcloud_storage_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        1 2023-07-21 04:18:09.000000 gcloud-storage-manager-0.1.2/gcloud_storage_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       29 2023-07-21 04:18:09.000000 gcloud-storage-manager-0.1.2/gcloud_storage_manager.egg-info/top_level.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       38 2023-07-21 04:18:09.980633 gcloud-storage-manager-0.1.2/setup.cfg
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      614 2023-07-21 04:18:08.000000 gcloud-storage-manager-0.1.2/setup.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 04:18:09.980633 gcloud-storage-manager-0.1.2/tests/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-26 15:31:54.000000 gcloud-storage-manager-0.1.2/tests/__init__.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     4057 2023-07-21 03:37:59.000000 gcloud-storage-manager-0.1.2/tests/test_download.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2901 2023-07-21 03:41:59.000000 gcloud-storage-manager-0.1.2/tests/test_upload.py
```

### Comparing `gcloud-storage-manager-0.1.1/LICENSE` & `gcloud-storage-manager-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gcloud-storage-manager-0.1.1/README.md` & `gcloud-storage-manager-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,14 @@
     bucket_name="test_bucket",
     dir_name="test_dir",
     dir_name_child="test_child_dir",
     file_type=FileType(".svg", "image/svg+xml"),
     credentials_path="path/to/creds.json",
 )
 
-uploader._upload_file("test_key", b"test bytes", False)
+uploader._upload_file("test_key.svg", b"test bytes", False)
 ```
 
 # prerequest
 - program can read gcloud json key file from the project environment
 - gcloud storage api is activated and backet is already created
```

### Comparing `gcloud-storage-manager-0.1.1/gcloud_storage_manager/base.py` & `gcloud-storage-manager-0.1.2/gcloud_storage_manager/base.py`

 * *Files identical despite different names*

### Comparing `gcloud-storage-manager-0.1.1/gcloud_storage_manager/download.py` & `gcloud-storage-manager-0.1.2/gcloud_storage_manager/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,10 +77,11 @@
         """
         file_path_prefix = f"{self.storage_base_dir}/{key}"
         blobs = self.bucket.list_blobs(prefix=file_path_prefix)
         files = []
         for blob_ in blobs:
             blob: storage.Blob = blob_
             file_name: str = blob.name
-            if self._file_match(file_name):
-                files.append(blob.download_as_bytes())
+            if not self._file_match(file_name):
+                logging.info(f"Invalid file extension: {file_name}")
+            files.append(blob.download_as_bytes())
         return files
```

### Comparing `gcloud-storage-manager-0.1.1/gcloud_storage_manager/upload.py` & `gcloud-storage-manager-0.1.2/gcloud_storage_manager/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
         e.g.
         file_path = "test_path"
         file_content = b"test_content"
         overwrite = False
         uploader._upload_file(file_path, file_content, overwrite)
         """
         if not self._file_match(file_path):
+            logging.info(f"Invalid file extension: {file_path}")
             return False
         full_file_path = f"{self.storage_base_dir}/{file_path}"
 
         try:
             blob = self.bucket.blob(full_file_path)
             if blob.exists() and not overwrite:
                 return False
```

### Comparing `gcloud-storage-manager-0.1.1/setup.py` & `gcloud-storage-manager-0.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="gcloud-storage-manager",
-    version="0.1.1",
+    version="0.1.2",
     description="A package to manage Google Cloud Storage",
     packages=find_packages(),
     install_requires=[],
     classifiers=[  # https://pypi.org/classifiers/
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `gcloud-storage-manager-0.1.1/tests/test_download.py` & `gcloud-storage-manager-0.1.2/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `gcloud-storage-manager-0.1.1/tests/test_upload.py` & `gcloud-storage-manager-0.1.2/tests/test_upload.py`

 * *Files identical despite different names*

