# Comparing `tmp/gcloud-storage-manager-0.1.2.tar.gz` & `tmp/gcloud-storage-manager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcloud-storage-manager-0.1.2.tar", last modified: Fri Jul 21 04:18:09 2023, max compression
+gzip compressed data, was "gcloud-storage-manager-0.2.0.tar", last modified: Fri Jul 21 07:40:26 2023, max compression
```

## Comparing `gcloud-storage-manager-0.1.2.tar` & `gcloud-storage-manager-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 04:18:09.980633 gcloud-storage-manager-0.1.2/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1069 2023-06-26 15:50:43.000000 gcloud-storage-manager-0.1.2/LICENSE
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      461 2023-07-21 04:18:09.980633 gcloud-storage-manager-0.1.2/PKG-INFO
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      997 2023-07-21 03:46:57.000000 gcloud-storage-manager-0.1.2/README.md
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 04:18:09.976633 gcloud-storage-manager-0.1.2/gcloud_storage_manager/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      191 2023-06-26 15:40:23.000000 gcloud-storage-manager-0.1.2/gcloud_storage_manager/__init__.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      913 2023-07-21 03:29:32.000000 gcloud-storage-manager-0.1.2/gcloud_storage_manager/base.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2829 2023-07-21 04:17:41.000000 gcloud-storage-manager-0.1.2/gcloud_storage_manager/download.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      137 2023-06-26 15:23:45.000000 gcloud-storage-manager-0.1.2/gcloud_storage_manager/std_logging.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     3643 2023-07-21 04:16:50.000000 gcloud-storage-manager-0.1.2/gcloud_storage_manager/upload.py
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 04:18:09.976633 gcloud-storage-manager-0.1.2/gcloud_storage_manager.egg-info/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      461 2023-07-21 04:18:09.000000 gcloud-storage-manager-0.1.2/gcloud_storage_manager.egg-info/PKG-INFO
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      444 2023-07-21 04:18:09.000000 gcloud-storage-manager-0.1.2/gcloud_storage_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        1 2023-07-21 04:18:09.000000 gcloud-storage-manager-0.1.2/gcloud_storage_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       29 2023-07-21 04:18:09.000000 gcloud-storage-manager-0.1.2/gcloud_storage_manager.egg-info/top_level.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       38 2023-07-21 04:18:09.980633 gcloud-storage-manager-0.1.2/setup.cfg
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      614 2023-07-21 04:18:08.000000 gcloud-storage-manager-0.1.2/setup.py
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 04:18:09.980633 gcloud-storage-manager-0.1.2/tests/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-26 15:31:54.000000 gcloud-storage-manager-0.1.2/tests/__init__.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     4057 2023-07-21 03:37:59.000000 gcloud-storage-manager-0.1.2/tests/test_download.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2901 2023-07-21 03:41:59.000000 gcloud-storage-manager-0.1.2/tests/test_upload.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 07:40:26.911223 gcloud-storage-manager-0.2.0/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1069 2023-06-26 15:50:43.000000 gcloud-storage-manager-0.2.0/LICENSE
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      461 2023-07-21 07:40:26.911223 gcloud-storage-manager-0.2.0/PKG-INFO
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      997 2023-07-21 03:46:57.000000 gcloud-storage-manager-0.2.0/README.md
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 07:40:26.907223 gcloud-storage-manager-0.2.0/gcloud_storage_manager/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      191 2023-06-26 15:40:23.000000 gcloud-storage-manager-0.2.0/gcloud_storage_manager/__init__.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      913 2023-07-21 03:29:32.000000 gcloud-storage-manager-0.2.0/gcloud_storage_manager/base.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2713 2023-07-21 07:37:49.000000 gcloud-storage-manager-0.2.0/gcloud_storage_manager/download.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      137 2023-06-26 15:23:45.000000 gcloud-storage-manager-0.2.0/gcloud_storage_manager/std_logging.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     3563 2023-07-21 07:20:09.000000 gcloud-storage-manager-0.2.0/gcloud_storage_manager/upload.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 07:40:26.907223 gcloud-storage-manager-0.2.0/gcloud_storage_manager.egg-info/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      461 2023-07-21 07:40:26.000000 gcloud-storage-manager-0.2.0/gcloud_storage_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      444 2023-07-21 07:40:26.000000 gcloud-storage-manager-0.2.0/gcloud_storage_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        1 2023-07-21 07:40:26.000000 gcloud-storage-manager-0.2.0/gcloud_storage_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       29 2023-07-21 07:40:26.000000 gcloud-storage-manager-0.2.0/gcloud_storage_manager.egg-info/top_level.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       38 2023-07-21 07:40:26.911223 gcloud-storage-manager-0.2.0/setup.cfg
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      614 2023-07-21 07:40:17.000000 gcloud-storage-manager-0.2.0/setup.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-07-21 07:40:26.911223 gcloud-storage-manager-0.2.0/tests/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-26 15:31:54.000000 gcloud-storage-manager-0.2.0/tests/__init__.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     4170 2023-07-21 07:39:15.000000 gcloud-storage-manager-0.2.0/tests/test_download.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     2967 2023-07-21 07:14:08.000000 gcloud-storage-manager-0.2.0/tests/test_upload.py
```

### Comparing `gcloud-storage-manager-0.1.2/LICENSE` & `gcloud-storage-manager-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gcloud-storage-manager-0.1.2/README.md` & `gcloud-storage-manager-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gcloud-storage-manager-0.1.2/gcloud_storage_manager/base.py` & `gcloud-storage-manager-0.2.0/gcloud_storage_manager/base.py`

 * *Files identical despite different names*

### Comparing `gcloud-storage-manager-0.1.2/gcloud_storage_manager/upload.py` & `gcloud-storage-manager-0.2.0/gcloud_storage_manager/upload.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from concurrent.futures import ThreadPoolExecutor, as_completed
+import asyncio
 from dataclasses import dataclass, field
 from typing import List, Tuple
 
 from gcloud_storage_manager.base import BaseStorageFileHandler, FileType
 from gcloud_storage_manager.std_logging import logging
 
 
@@ -43,70 +43,73 @@
         max_workers=5,
     ):
         super().__init__(
             bucket_name, dir_name, dir_name_child, file_type, credentials_path
         )
         self.max_workers = max_workers
 
-    def upload_files(
+    async def upload_files(
         self,
         validated_files: List[Tuple[str, bytes]],  # (file_path, file_content)
         overwrite: bool = False,
     ) -> UploadResult:
         logging.info("Start of uploading files to cloud storage")
 
         success_count = 0
         failure_count = 0
         failed_keys: List[str] = []
-        with ThreadPoolExecutor(max_workers=self.max_workers) as executor:
-            futures_to_file_paths = {
-                executor.submit(
-                    self._upload_file, file_path, file_content, overwrite
-                ): file_path
-                for file_path, file_content in validated_files
-            }
-            for future in as_completed(futures_to_file_paths):
-                file_path = futures_to_file_paths[future]
-                try:
-                    success = future.result()
-                    if success:
-                        success_count += 1
-                    else:
-                        failure_count += 1
-                        failed_keys.append(file_path)
-                except Exception as e:
-                    failure_count += 1
-                    failed_keys.append(file_path)
-                    logging.info(f"Error uploading '{file_path}': {e}")
+
+        upload_tasks = (
+            self._upload_file(file_path, file_content, overwrite)
+            for file_path, file_content in validated_files
+        )
+
+        results = await asyncio.gather(*upload_tasks, return_exceptions=True)
+
+        for result, file_path in zip(
+            results, [file_path for file_path, file_content in validated_files]
+        ):
+            if isinstance(result, Exception):
+                failure_count += 1
+                failed_keys.append(file_path)
+                logging.info(f"Error uploading '{file_path}': {result}")
+            elif result:
+                success_count += 1
+            else:
+                failure_count += 1
+                failed_keys.append(file_path)
 
         logging.info("End of uploading files to cloud storage")
 
         return UploadResult(success_count, failure_count, failed_keys)
 
-    def _upload_file(
+    async def _upload_file(
         self, file_path: str, file_content: bytes, overwrite: bool
     ) -> bool:
         """
         Upload a file to cloud storage.
 
         e.g.
         file_path = "test_path"
         file_content = b"test_content"
         overwrite = False
         uploader._upload_file(file_path, file_content, overwrite)
         """
         if not self._file_match(file_path):
-            logging.info(f"Invalid file extension: {file_path}")
+            logging.warning(f"Invalid file extension: {file_path}")
             return False
         full_file_path = f"{self.storage_base_dir}/{file_path}"
 
         try:
-            blob = self.bucket.blob(full_file_path)
-            if blob.exists() and not overwrite:
+            blob = await asyncio.to_thread(self.bucket.blob, full_file_path)
+            exists = await asyncio.to_thread(blob.exists)
+            if exists and not overwrite:
                 return False
-            blob.upload_from_string(
-                file_content, content_type=self.file_type.content_type
+            await asyncio.to_thread(
+                blob.upload_from_string,
+                file_content,
+                content_type=self.file_type.content_type,
             )
             return True
         except Exception as e:
-            logging.info(f"Error uploading '{full_file_path}': {e}")
+            logging.warning(f"Error uploading '{full_file_path}': {e}")
             return False
```

### Comparing `gcloud-storage-manager-0.1.2/setup.py` & `gcloud-storage-manager-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="gcloud-storage-manager",
-    version="0.1.2",
+    version="0.2.0",
     description="A package to manage Google Cloud Storage",
     packages=find_packages(),
     install_requires=[],
     classifiers=[  # https://pypi.org/classifiers/
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `gcloud-storage-manager-0.1.2/tests/test_download.py` & `gcloud-storage-manager-0.2.0/tests/test_download.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from unittest.mock import Mock, patch
 
+import pytest
 from google.api_core.exceptions import GoogleAPIError
 from google.cloud import storage
 
 from gcloud_storage_manager import FileType, StorageFileDownloader
 
 
 @patch("google.cloud.storage.Client")
@@ -19,15 +20,16 @@
     )
 
     assert downloader._file_match("test_file.svg") is True
     assert downloader._file_match("test_file.jpg") is False
 
 
 @patch("google.cloud.storage.Client")
-def test_load_files_by_key(mock_storage_client):
+@pytest.mark.asyncio
+async def test_load_files_by_key(mock_storage_client):
     # Create a mock Blob object to return as part of our mocked bucket.list_blobs
     mock_blob = Mock(spec=storage.Blob)
     mock_blob.download_as_bytes.return_value = b"test bytes"
     mock_blob.name = "test_file.svg"
 
     # Mock the storage Client's from_service_account_json
     mock_storage_client.from_service_account_json.return_value.bucket.return_value.list_blobs.return_value = [
@@ -38,22 +40,23 @@
         bucket_name="test_bucket",
         dir_name="test_dir",
         dir_name_child="test_child_dir",
         file_type=FileType(".svg", "image/svg+xml"),
         credentials_path="path/to/creds.json",
     )
 
-    result = downloader.load_files_by_key("test_char")
+    result = await downloader.load_files_by_key("test_char")
 
     assert len(result) == 1
     assert result[0] == b"test bytes"
 
 
 @patch("google.cloud.storage.Client")
-def test_load_files_all(mock_storage_client):
+@pytest.mark.asyncio
+async def test_load_files_all(mock_storage_client):
     # Create a mock Blob object to return as part of our mocked bucket.list_blobs
     mock_blob = Mock(spec=storage.Blob)
     mock_blob.download_as_bytes.return_value = b"test bytes"
     mock_blob.name = "test_file.svg"
 
     # Mock the storage Client's from_service_account_json
     mock_storage_client.from_service_account_json.return_value.bucket.return_value.list_blobs.return_value = [
@@ -64,15 +67,15 @@
         bucket_name="test_bucket",
         dir_name="test_dir",
         dir_name_child="test_child_dir",
         file_type=FileType(".svg", "image/svg+xml"),
         credentials_path="path/to/creds.json",
     )
 
-    result = downloader.load_files_all(["test_char", "test_char_2"])
+    result = await downloader.load_files_all(["test_char", "test_char_2"])
 
     assert len(result) == 2
     assert all(len(v) == 1 for v in result.values())
     assert all(v[0] == b"test bytes" for v in result.values())
 
 
 @patch("google.cloud.storage.Client")
@@ -88,15 +91,16 @@
     )
 
     assert downloader._file_match("test_file.svg") is True
     assert downloader._file_match("test_file.jpg") is False
 
 
 @patch("google.cloud.storage.Client")
-def test_load_files_all_handle_api_error(mock_storage_client):
+@pytest.mark.asyncio
+async def test_load_files_all_handle_api_error(mock_storage_client):
     # Create a mock Blob object to return as part of our mocked bucket.list_blobs
     mock_blob = Mock(spec=storage.Blob)
     mock_blob.download_as_bytes.side_effect = GoogleAPIError("test error")
     mock_blob.name = "test_file.svg"
 
     # Mock the storage Client's from_service_account_json
     mock_storage_client.from_service_account_json.return_value.bucket.return_value.list_blobs.return_value = [
@@ -108,10 +112,10 @@
         dir_name="test_dir",
         dir_name_child="test_child_dir",
         file_type=FileType(".svg", "image/svg+xml"),
         credentials_path="path/to/creds.json",
     )
 
     keys = ["test_char1", "test_char2"]
-    result = downloader.load_files_all(keys)
+    result = await downloader.load_files_all(keys)
 
     assert all(len(files) == 0 for files in result.values())
```

### Comparing `gcloud-storage-manager-0.1.2/tests/test_upload.py` & `gcloud-storage-manager-0.2.0/tests/test_upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,59 +29,61 @@
     result_no_error = UploadResult(success_count=5, failure_count=0, failed_keys=[])
     assert result_no_error.has_errors is False
 
 
 @patch("google.cloud.storage.Client")
 @patch("google.cloud.storage.Bucket")
 @patch("google.cloud.storage.Blob")
-def test_upload_file(mock_blob, mock_bucket, mock_storage_client):
+@pytest.mark.asyncio
+async def test_upload_file(mock_blob, mock_bucket, mock_storage_client):
     mock_storage_client.from_service_account_json.return_value = mock_storage_client
     mock_storage_client.bucket.return_value = mock_bucket
     mock_bucket.blob.return_value = mock_blob
     mock_blob.exists.return_value = False
 
     uploader = StorageFileUploader(
         bucket_name="test_bucket",
         dir_name="test_dir",
         dir_name_child="test_child_dir",
         file_type=FileType(".svg", "image/svg+xml"),
         credentials_path="path/to/creds.json",
     )
 
-    uploader._upload_file("test_key.svg", b"test bytes", False)
+    await uploader._upload_file("test_key.svg", b"test bytes", False)
 
     mock_bucket.blob.assert_called_once_with("test_dir/test_child_dir/test_key.svg")
     mock_blob.upload_from_string.assert_called_once_with(
         b"test bytes", content_type="image/svg+xml"
     )
 
 
 @pytest.fixture
 def mock_upload_file():
     with patch.object(StorageFileUploader, "_upload_file", return_value=True) as _mock:
         yield _mock
 
 
 @patch("google.cloud.storage.Client")
-def test_upload_files(mock_storage_client, mock_upload_file):
+@pytest.mark.asyncio
+async def test_upload_files(mock_storage_client, mock_upload_file):
     mock_storage_client.from_service_account_json.return_value = mock_storage_client
 
     uploader = StorageFileUploader(
         bucket_name="test_bucket",
         dir_name="test_dir",
         dir_name_child="test_child_dir",
         file_type=FileType(".svg", "image/svg+xml"),
         credentials_path="path/to/creds.json",
     )
 
     validated_files = [
         ("test_key1.svg", b"test bytes1"),
         ("test_key2.svg", b"test bytes2"),
     ]
-    result = uploader.upload_files(validated_files, False)
+    result = await uploader.upload_files(validated_files, False)
 
     assert mock_upload_file.call_count == len(validated_files)
     for file in validated_files:
         mock_upload_file.assert_any_call(*file, False)
 
     assert result.success_count == len(validated_files)
     assert result.failure_count == 0
```

