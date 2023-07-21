# Comparing `tmp/gcloud-storage-manager-0.0.1.tar.gz` & `tmp/gcloud-storage-manager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcloud-storage-manager-0.0.1.tar", last modified: Mon Jun 26 15:54:45 2023, max compression
+gzip compressed data, was "gcloud-storage-manager-0.1.1.tar", last modified: Fri Jul 21 03:45:50 2023, max compression
```

## Comparing `gcloud-storage-manager-0.0.1.tar` & `gcloud-storage-manager-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-26 15:54:45.035238 gcloud-storage-manager-0.0.1/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1069 2023-06-26 15:50:43.000000 gcloud-storage-manager-0.0.1/LICENSE
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      461 2023-06-26 15:54:45.031238 gcloud-storage-manager-0.0.1/PKG-INFO
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1007 2023-06-26 15:48:32.000000 gcloud-storage-manager-0.0.1/README.md
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-26 15:54:45.031238 gcloud-storage-manager-0.0.1/gcloud_storage_manager/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      191 2023-06-26 15:40:23.000000 gcloud-storage-manager-0.0.1/gcloud_storage_manager/__init__.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      819 2023-06-26 15:22:55.000000 gcloud-storage-manager-0.0.1/gcloud_storage_manager/base.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2185 2023-06-26 15:26:22.000000 gcloud-storage-manager-0.0.1/gcloud_storage_manager/download.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      137 2023-06-26 15:23:45.000000 gcloud-storage-manager-0.0.1/gcloud_storage_manager/std_logging.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2656 2023-06-26 15:26:06.000000 gcloud-storage-manager-0.0.1/gcloud_storage_manager/upload.py
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-26 15:54:45.031238 gcloud-storage-manager-0.0.1/gcloud_storage_manager.egg-info/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      461 2023-06-26 15:54:44.000000 gcloud-storage-manager-0.0.1/gcloud_storage_manager.egg-info/PKG-INFO
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      444 2023-06-26 15:54:44.000000 gcloud-storage-manager-0.0.1/gcloud_storage_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        1 2023-06-26 15:54:44.000000 gcloud-storage-manager-0.0.1/gcloud_storage_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       29 2023-06-26 15:54:44.000000 gcloud-storage-manager-0.0.1/gcloud_storage_manager.egg-info/top_level.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       38 2023-06-26 15:54:45.035238 gcloud-storage-manager-0.0.1/setup.cfg
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      614 2023-06-26 15:50:36.000000 gcloud-storage-manager-0.0.1/setup.py
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-26 15:54:45.031238 gcloud-storage-manager-0.0.1/tests/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-26 15:31:54.000000 gcloud-storage-manager-0.0.1/tests/__init__.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     4092 2023-06-26 15:45:01.000000 gcloud-storage-manager-0.0.1/tests/test_download.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2880 2023-06-26 15:40:59.000000 gcloud-storage-manager-0.0.1/tests/test_upload.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 03:45:50.488035 gcloud-storage-manager-0.1.1/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1069 2023-06-26 15:50:43.000000 gcloud-storage-manager-0.1.1/LICENSE
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      461 2023-07-21 03:45:50.488035 gcloud-storage-manager-0.1.1/PKG-INFO
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      993 2023-07-21 03:37:53.000000 gcloud-storage-manager-0.1.1/README.md
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 03:45:50.484034 gcloud-storage-manager-0.1.1/gcloud_storage_manager/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      191 2023-06-26 15:40:23.000000 gcloud-storage-manager-0.1.1/gcloud_storage_manager/__init__.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      913 2023-07-21 03:29:32.000000 gcloud-storage-manager-0.1.1/gcloud_storage_manager/base.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2760 2023-07-21 03:37:53.000000 gcloud-storage-manager-0.1.1/gcloud_storage_manager/download.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      137 2023-06-26 15:23:45.000000 gcloud-storage-manager-0.1.1/gcloud_storage_manager/std_logging.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     3578 2023-07-21 03:42:10.000000 gcloud-storage-manager-0.1.1/gcloud_storage_manager/upload.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 03:45:50.488035 gcloud-storage-manager-0.1.1/gcloud_storage_manager.egg-info/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      461 2023-07-21 03:45:50.000000 gcloud-storage-manager-0.1.1/gcloud_storage_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      444 2023-07-21 03:45:50.000000 gcloud-storage-manager-0.1.1/gcloud_storage_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        1 2023-07-21 03:45:50.000000 gcloud-storage-manager-0.1.1/gcloud_storage_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       29 2023-07-21 03:45:50.000000 gcloud-storage-manager-0.1.1/gcloud_storage_manager.egg-info/top_level.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       38 2023-07-21 03:45:50.488035 gcloud-storage-manager-0.1.1/setup.cfg
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      614 2023-07-21 03:45:40.000000 gcloud-storage-manager-0.1.1/setup.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 03:45:50.488035 gcloud-storage-manager-0.1.1/tests/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-26 15:31:54.000000 gcloud-storage-manager-0.1.1/tests/__init__.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     4057 2023-07-21 03:37:59.000000 gcloud-storage-manager-0.1.1/tests/test_download.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2901 2023-07-21 03:41:59.000000 gcloud-storage-manager-0.1.1/tests/test_upload.py
```

### Comparing `gcloud-storage-manager-0.0.1/LICENSE` & `gcloud-storage-manager-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gcloud-storage-manager-0.0.1/README.md` & `gcloud-storage-manager-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ```
 from src.infra.storage import FileType, StorageFileDownloader
 
 downloader = StorageFileDownloader(
     bucket_name="test_bucket",
     dir_name="test_dir",
     dir_name_child="test_child_dir",
-    file_type=FileType("SVG", ".svg", "image/svg+xml"),
+    file_type=FileType(".svg", "image/svg+xml"),
     credentials_path="path/to/creds.json",
 )
 
 keys = ["test_char1", "test_char2"]
 result = downloader.load_files_all(keys)
 ```
 
@@ -26,15 +26,15 @@
 ```
 from src.infra.storage import FileType, StorageFileUploader
 
 uploader = StorageFileUploader(
     bucket_name="test_bucket",
     dir_name="test_dir",
     dir_name_child="test_child_dir",
-    file_type=FileType("SVG", ".svg", "image/svg+xml"),
+    file_type=FileType(".svg", "image/svg+xml"),
     credentials_path="path/to/creds.json",
 )
 
 uploader._upload_file("test_key", b"test bytes", False)
 ```
 
 # prerequest
```

### Comparing `gcloud-storage-manager-0.0.1/gcloud_storage_manager/base.py` & `gcloud-storage-manager-0.1.1/gcloud_storage_manager/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,21 +4,25 @@
 
 
 class FileType(NamedTuple):
     """
     File type information.
 
     e.g.
-    FileType("SVG", ".svg", "image/svg+xml")
+    FileType(".svg", "image/svg+xml")
     """
 
-    label: str
     extension: str
     content_type: str
 
+    @property
+    def label(self) -> str:
+        # e.g. ".svg" -> "SVG"
+        return self.extension[1:].upper()
+
 
 class BaseStorageFileHandler:
     def __init__(
         self,
         bucket_name: str,
         dir_name: str,
         dir_name_child: str,
```

### Comparing `gcloud-storage-manager-0.0.1/gcloud_storage_manager/download.py` & `gcloud-storage-manager-0.1.1/gcloud_storage_manager/download.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,71 @@
+from concurrent.futures import ThreadPoolExecutor, as_completed
 from typing import Dict, List
 
 from google.api_core.exceptions import GoogleAPIError
 from google.cloud import storage
-from tqdm import tqdm
 
-from gcloud_storage_manager.base import BaseStorageFileHandler
+from gcloud_storage_manager.base import BaseStorageFileHandler, FileType
 from gcloud_storage_manager.std_logging import logging
 
 
 class StorageFileDownloader(BaseStorageFileHandler):
     """
     Download files from cloud storage.
 
     e.g.
     downloader = StorageFileDownloader(
         bucket_name="test_bucket",
         dir_name="test_dir",
         dir_name_child="test_child_dir",
-        file_type=FileType("SVG", ".svg", "image/svg+xml"),
+        file_type=FileType(".svg", "image/svg+xml"),
         credentials_path="path/to/creds.json",
     )
     files = downloader.load_files_by_key("test_key")
     """
 
+    def __init__(
+        self,
+        bucket_name: str,
+        dir_name: str,
+        dir_name_child: str,
+        file_type: FileType,
+        credentials_path: str,
+        max_workers=5,
+    ):
+        super().__init__(
+            bucket_name, dir_name, dir_name_child, file_type, credentials_path
+        )
+        self.max_workers = max_workers
+
     def load_files_all(self, keys: List[str]) -> Dict[str, List[bytes]]:
         """
         Load files from cloud storage.
 
         e.g.
         keys = ["key1", "key2", "key3"]
         files = downloader.load_files_all(keys)
         """
         results: Dict[str, List[bytes]] = {}
 
         logging.info("Start of getting files from cloud storage")
-        with tqdm(total=len(keys), desc="Uploading", ncols=80) as pbar:
-            for key in keys:
+        with ThreadPoolExecutor(max_workers=self.max_workers) as executor:
+            futures_to_keys = {
+                executor.submit(self.load_files_by_key, key): key for key in keys
+            }
+            for future in as_completed(futures_to_keys):
+                key = futures_to_keys[future]
                 try:
                     results[key] = self.load_files_by_key(key)
                 except GoogleAPIError as e:
                     logging.info(
                         f"Failed to download {self.file_type.label} "
                         f"data for '{key}': {e}"
                     )
                     results[key] = []
-                pbar.update()
 
         logging.info("Finish of getting files from cloud storage")
 
         return results
 
     def load_files_by_key(self, key: str) -> List[bytes]:
         """
```

### Comparing `gcloud-storage-manager-0.0.1/gcloud_storage_manager/upload.py` & `gcloud-storage-manager-0.1.1/gcloud_storage_manager/upload.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,12 @@
+from concurrent.futures import ThreadPoolExecutor, as_completed
 from dataclasses import dataclass, field
 from typing import List, Tuple
 
-from tqdm import tqdm
-
-from gcloud_storage_manager.base import BaseStorageFileHandler
+from gcloud_storage_manager.base import BaseStorageFileHandler, FileType
 from gcloud_storage_manager.std_logging import logging
 
 
 @dataclass
 class UploadResult:
     success_count: int
     failure_count: int
@@ -24,38 +23,64 @@
     Upload files to cloud storage.
 
     e.g.
     uploader = StorageFileUploader(
         bucket_name="test_bucket",
         dir_name="test_dir",
         dir_name_child="test_child_dir",
-        file_type=FileType("SVG", ".svg", "image/svg+xml"),
+        file_type=FileType(".svg", "image/svg+xml"),
         credentials_path="path/to/creds.json",
     )
     result = uploader.upload_files(validated_files)
     """
 
+    def __init__(
+        self,
+        bucket_name: str,
+        dir_name: str,
+        dir_name_child: str,
+        file_type: FileType,
+        credentials_path: str,
+        max_workers=5,
+    ):
+        super().__init__(
+            bucket_name, dir_name, dir_name_child, file_type, credentials_path
+        )
+        self.max_workers = max_workers
+
     def upload_files(
         self,
         validated_files: List[Tuple[str, bytes]],  # (file_path, file_content)
         overwrite: bool = False,
     ) -> UploadResult:
         logging.info("Start of uploading files to cloud storage")
 
         success_count = 0
         failure_count = 0
         failed_keys: List[str] = []
-        with tqdm(total=len(validated_files), desc="Uploading", ncols=80) as pbar:
-            for file_path, file_content in validated_files:
-                if self._upload_file(file_path, file_content, overwrite):
-                    success_count += 1
-                else:
-                    failed_keys.append(file_path)
+        with ThreadPoolExecutor(max_workers=self.max_workers) as executor:
+            futures_to_file_paths = {
+                executor.submit(
+                    self._upload_file, file_path, file_content, overwrite
+                ): file_path
+                for file_path, file_content in validated_files
+            }
+            for future in as_completed(futures_to_file_paths):
+                file_path = futures_to_file_paths[future]
+                try:
+                    success = future.result()
+                    if success:
+                        success_count += 1
+                    else:
+                        failure_count += 1
+                        failed_keys.append(file_path)
+                except Exception as e:
                     failure_count += 1
-                pbar.update()
+                    failed_keys.append(file_path)
+                    logging.info(f"Error uploading '{file_path}': {e}")
 
         logging.info("End of uploading files to cloud storage")
 
         return UploadResult(success_count, failure_count, failed_keys)
 
     def _upload_file(
         self, file_path: str, file_content: bytes, overwrite: bool
@@ -65,18 +90,19 @@
 
         e.g.
         file_path = "test_path"
         file_content = b"test_content"
         overwrite = False
         uploader._upload_file(file_path, file_content, overwrite)
         """
+        if not self._file_match(file_path):
+            return False
+        full_file_path = f"{self.storage_base_dir}/{file_path}"
+
         try:
-            full_file_path = (
-                f"{self.storage_base_dir}/{file_path}{self.file_type.extension}"
-            )
             blob = self.bucket.blob(full_file_path)
             if blob.exists() and not overwrite:
                 return False
             blob.upload_from_string(
                 file_content, content_type=self.file_type.content_type
             )
             return True
```

### Comparing `gcloud-storage-manager-0.0.1/setup.py` & `gcloud-storage-manager-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="gcloud-storage-manager",
-    version="0.0.1",
+    version="0.1.1",
     description="A package to manage Google Cloud Storage",
     packages=find_packages(),
     install_requires=[],
     classifiers=[  # https://pypi.org/classifiers/
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `gcloud-storage-manager-0.0.1/tests/test_download.py` & `gcloud-storage-manager-0.1.1/tests/test_download.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def test__file_match(mock_storage_client):
     mock_storage_client.from_service_account_json.return_value = mock_storage_client
 
     downloader = StorageFileDownloader(
         bucket_name="test_bucket",
         dir_name="test_dir",
         dir_name_child="test_child_dir",
-        file_type=FileType("SVG", ".svg", "image/svg+xml"),
+        file_type=FileType(".svg", "image/svg+xml"),
         credentials_path="path/to/creds.json",
     )
 
     assert downloader._file_match("test_file.svg") is True
     assert downloader._file_match("test_file.jpg") is False
 
 
@@ -34,15 +34,15 @@
         mock_blob
     ]
 
     downloader = StorageFileDownloader(
         bucket_name="test_bucket",
         dir_name="test_dir",
         dir_name_child="test_child_dir",
-        file_type=FileType("SVG", ".svg", "image/svg+xml"),
+        file_type=FileType(".svg", "image/svg+xml"),
         credentials_path="path/to/creds.json",
     )
 
     result = downloader.load_files_by_key("test_char")
 
     assert len(result) == 1
     assert result[0] == b"test bytes"
@@ -60,15 +60,15 @@
         mock_blob
     ]
 
     downloader = StorageFileDownloader(
         bucket_name="test_bucket",
         dir_name="test_dir",
         dir_name_child="test_child_dir",
-        file_type=FileType("SVG", ".svg", "image/svg+xml"),
+        file_type=FileType(".svg", "image/svg+xml"),
         credentials_path="path/to/creds.json",
     )
 
     result = downloader.load_files_all(["test_char", "test_char_2"])
 
     assert len(result) == 2
     assert all(len(v) == 1 for v in result.values())
@@ -79,15 +79,15 @@
 def test__file_match_failed(mock_storage_client):
     mock_storage_client.from_service_account_json.return_value = mock_storage_client
 
     downloader = StorageFileDownloader(
         bucket_name="test_bucket",
         dir_name="test_dir",
         dir_name_child="test_child_dir",
-        file_type=FileType("SVG", ".svg", "image/svg+xml"),
+        file_type=FileType(".svg", "image/svg+xml"),
         credentials_path="path/to/creds.json",
     )
 
     assert downloader._file_match("test_file.svg") is True
     assert downloader._file_match("test_file.jpg") is False
 
 
@@ -103,15 +103,15 @@
         mock_blob
     ]
 
     downloader = StorageFileDownloader(
         bucket_name="test_bucket",
         dir_name="test_dir",
         dir_name_child="test_child_dir",
-        file_type=FileType("SVG", ".svg", "image/svg+xml"),
+        file_type=FileType(".svg", "image/svg+xml"),
         credentials_path="path/to/creds.json",
     )
 
     keys = ["test_char1", "test_char2"]
     result = downloader.load_files_all(keys)
 
     assert all(len(files) == 0 for files in result.values())
```

### Comparing `gcloud-storage-manager-0.0.1/tests/test_upload.py` & `gcloud-storage-manager-0.1.1/tests/test_upload.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,19 +39,19 @@
     mock_bucket.blob.return_value = mock_blob
     mock_blob.exists.return_value = False
 
     uploader = StorageFileUploader(
         bucket_name="test_bucket",
         dir_name="test_dir",
         dir_name_child="test_child_dir",
-        file_type=FileType("SVG", ".svg", "image/svg+xml"),
+        file_type=FileType(".svg", "image/svg+xml"),
         credentials_path="path/to/creds.json",
     )
 
-    uploader._upload_file("test_key", b"test bytes", False)
+    uploader._upload_file("test_key.svg", b"test bytes", False)
 
     mock_bucket.blob.assert_called_once_with("test_dir/test_child_dir/test_key.svg")
     mock_blob.upload_from_string.assert_called_once_with(
         b"test bytes", content_type="image/svg+xml"
     )
 
 
@@ -65,19 +65,22 @@
 def test_upload_files(mock_storage_client, mock_upload_file):
     mock_storage_client.from_service_account_json.return_value = mock_storage_client
 
     uploader = StorageFileUploader(
         bucket_name="test_bucket",
         dir_name="test_dir",
         dir_name_child="test_child_dir",
-        file_type=FileType("SVG", ".svg", "image/svg+xml"),
+        file_type=FileType(".svg", "image/svg+xml"),
         credentials_path="path/to/creds.json",
     )
 
-    validated_files = [("test_key1", b"test bytes1"), ("test_key2", b"test bytes2")]
+    validated_files = [
+        ("test_key1.svg", b"test bytes1"),
+        ("test_key2.svg", b"test bytes2"),
+    ]
     result = uploader.upload_files(validated_files, False)
 
     assert mock_upload_file.call_count == len(validated_files)
     for file in validated_files:
         mock_upload_file.assert_any_call(*file, False)
 
     assert result.success_count == len(validated_files)
```

