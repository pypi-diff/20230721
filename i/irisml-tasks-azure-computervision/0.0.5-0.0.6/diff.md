# Comparing `tmp/irisml-tasks-azure-computervision-0.0.5.tar.gz` & `tmp/irisml-tasks-azure-computervision-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml-tasks-azure-computervision-0.0.5.tar", last modified: Thu Jul 20 00:16:07 2023, max compression
+gzip compressed data, was "irisml-tasks-azure-computervision-0.0.6.tar", last modified: Fri Jul 21 00:57:49 2023, max compression
```

## Comparing `irisml-tasks-azure-computervision-0.0.5.tar` & `irisml-tasks-azure-computervision-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:16:07.151002 irisml-tasks-azure-computervision-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-20 00:13:37.000000 irisml-tasks-azure-computervision-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-20 00:16:07.151002 irisml-tasks-azure-computervision-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-20 00:13:37.000000 irisml-tasks-azure-computervision-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:16:07.147002 irisml-tasks-azure-computervision-0.0.5/irisml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:16:07.151002 irisml-tasks-azure-computervision-0.0.5/irisml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-20 00:13:37.000000 irisml-tasks-azure-computervision-0.0.5/irisml/tasks/create_azure_computervision_caption_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-20 00:13:37.000000 irisml-tasks-azure-computervision-0.0.5/irisml/tasks/create_azure_computervision_classification_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-20 00:13:37.000000 irisml-tasks-azure-computervision-0.0.5/irisml/tasks/create_azure_computervision_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-20 00:13:37.000000 irisml-tasks-azure-computervision-0.0.5/irisml/tasks/create_azure_computervision_ocr_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-20 00:13:37.000000 irisml-tasks-azure-computervision-0.0.5/irisml/tasks/delete_azure_computervision_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-07-20 00:13:37.000000 irisml-tasks-azure-computervision-0.0.5/irisml/tasks/train_azure_computervision_custom_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:16:07.151002 irisml-tasks-azure-computervision-0.0.5/irisml_tasks_azure_computervision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-20 00:16:07.000000 irisml-tasks-azure-computervision-0.0.5/irisml_tasks_azure_computervision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-20 00:16:07.000000 irisml-tasks-azure-computervision-0.0.5/irisml_tasks_azure_computervision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 00:16:07.000000 irisml-tasks-azure-computervision-0.0.5/irisml_tasks_azure_computervision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 00:16:07.000000 irisml-tasks-azure-computervision-0.0.5/irisml_tasks_azure_computervision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 00:16:07.000000 irisml-tasks-azure-computervision-0.0.5/irisml_tasks_azure_computervision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-20 00:13:37.000000 irisml-tasks-azure-computervision-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-20 00:16:07.155002 irisml-tasks-azure-computervision-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:16:07.151002 irisml-tasks-azure-computervision-0.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-20 00:13:37.000000 irisml-tasks-azure-computervision-0.0.5/test/test_create_azure_computervision_caption_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-20 00:13:37.000000 irisml-tasks-azure-computervision-0.0.5/test/test_create_azure_computervision_classification_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-20 00:13:37.000000 irisml-tasks-azure-computervision-0.0.5/test/test_create_azure_computervision_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-20 00:13:37.000000 irisml-tasks-azure-computervision-0.0.5/test/test_create_azure_computervision_ocr_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-20 00:13:37.000000 irisml-tasks-azure-computervision-0.0.5/test/test_delete_azure_computervision_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-20 00:13:37.000000 irisml-tasks-azure-computervision-0.0.5/test/test_train_azure_computervision_custom_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:57:49.539739 irisml-tasks-azure-computervision-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-21 00:57:49.539739 irisml-tasks-azure-computervision-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:57:49.535739 irisml-tasks-azure-computervision-0.0.6/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:57:49.535739 irisml-tasks-azure-computervision-0.0.6/irisml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/irisml/tasks/create_azure_computervision_caption_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/irisml/tasks/create_azure_computervision_classification_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/irisml/tasks/create_azure_computervision_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/irisml/tasks/create_azure_computervision_ocr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/irisml/tasks/delete_azure_computervision_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11782 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/irisml/tasks/train_azure_computervision_custom_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:57:49.535739 irisml-tasks-azure-computervision-0.0.6/irisml_tasks_azure_computervision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-21 00:57:49.000000 irisml-tasks-azure-computervision-0.0.6/irisml_tasks_azure_computervision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-21 00:57:49.000000 irisml-tasks-azure-computervision-0.0.6/irisml_tasks_azure_computervision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 00:57:49.000000 irisml-tasks-azure-computervision-0.0.6/irisml_tasks_azure_computervision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 00:57:49.000000 irisml-tasks-azure-computervision-0.0.6/irisml_tasks_azure_computervision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 00:57:49.000000 irisml-tasks-azure-computervision-0.0.6/irisml_tasks_azure_computervision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-21 00:57:49.539739 irisml-tasks-azure-computervision-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:57:49.539739 irisml-tasks-azure-computervision-0.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/test/test_create_azure_computervision_caption_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/test/test_create_azure_computervision_classification_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/test/test_create_azure_computervision_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/test/test_create_azure_computervision_ocr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/test/test_delete_azure_computervision_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/test/test_train_azure_computervision_custom_model.py
```

### Comparing `irisml-tasks-azure-computervision-0.0.5/LICENSE` & `irisml-tasks-azure-computervision-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.5/PKG-INFO` & `irisml-tasks-azure-computervision-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-azure-computervision
-Version: 0.0.5
+Version: 0.0.6
 Summary: Azure Computer Vision API tasks for IrisML
 Home-page: https://github.com/microsoft/irisml-tasks-azure-computervision
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-azure-computervision-0.0.5/README.md` & `irisml-tasks-azure-computervision-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.5/irisml/tasks/create_azure_computervision_caption_model.py` & `irisml-tasks-azure-computervision-0.0.6/irisml/tasks/create_azure_computervision_caption_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.5/irisml/tasks/create_azure_computervision_classification_model.py` & `irisml-tasks-azure-computervision-0.0.6/irisml/tasks/create_azure_computervision_classification_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.5/irisml/tasks/create_azure_computervision_custom_model.py` & `irisml-tasks-azure-computervision-0.0.6/irisml/tasks/create_azure_computervision_custom_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     Config:
         endpoint (str): Azure Computer Vision endpoint. Must start with https://.
         api_key (str): Azure Computer Vision API key.
         model_name (str): Custom model name to create.
         task_type (str): Task type. Either 'classification_multiclass' or 'object_detection'.
     """
-    VERSION = '0.1.1'
+    VERSION = '0.1.2'
 
     @dataclasses.dataclass
     class Inputs:
         class_names: typing.List[str]
 
     @dataclasses.dataclass
     class Config:
@@ -60,26 +60,31 @@
 
     def get_url(self, endpoint):
         return urllib.parse.urljoin(endpoint, f'/computervision/imageanalysis:analyze?api-version=2023-04-01-preview&model-name={self._model_name}')
 
 
 class AzureComputervisionCustomClassificationModel(AzureComputervisionCustomModel):
     def parse_response(self, response_body):
-        tags = response_body['customModelResult']['tagsResult']['values']
         predictions = [0] * len(self._class_names)
+        if 'tagsResult' not in response_body['customModelResult']:
+            return predictions
+        tags = response_body['customModelResult']['tagsResult']['values']
         for t in tags:
             predictions[self._class_names.index(t['name'])] = t['confidence']
         return predictions
 
     def collate_result(self, batch):
         return torch.tensor([b if b is not None else [0] * len(self._class_names) for b in batch])
 
 
 class AzureComputervisionCustomObjectDetectionModel(AzureComputervisionCustomModel):
     def parse_response(self, response_body):
+        if 'objectsResult' not in response_body['customModelResult']:
+            return torch.empty(0, 6, dtype=torch.float32)
+
         width = response_body['metadata']['width']
         height = response_body['metadata']['height']
         boxes = response_body['customModelResult']['objectsResult']['values']
         predictions = []
         for b in boxes:
             x = b['boundingBox']['x'] / width
             y = b['boundingBox']['y'] / height
```

### Comparing `irisml-tasks-azure-computervision-0.0.5/irisml/tasks/create_azure_computervision_ocr_model.py` & `irisml-tasks-azure-computervision-0.0.6/irisml/tasks/create_azure_computervision_ocr_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.5/irisml/tasks/delete_azure_computervision_custom_model.py` & `irisml-tasks-azure-computervision-0.0.6/irisml/tasks/delete_azure_computervision_custom_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.5/irisml/tasks/train_azure_computervision_custom_model.py` & `irisml-tasks-azure-computervision-0.0.6/irisml/tasks/train_azure_computervision_custom_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,17 @@
     Config:
         endpoint (str): Azure Computer Vision endpoint. Must start with https://.
         api_key (str): Azure Computer Vision API key.
         task_type (str): Task type. Must be one of 'classification_multiclass' or 'object_detection'.
         azure_storage_blob_container_url (str): Azure Storage Blob container URL. Make sure the Computer Vision API resrouce has access to this storage.
         budget_in_hours (int): Budget in hours.
         keep_dataset (bool): Keep the dataset in the container after training.
+        model_kind (str): Optional. Model kind. Must be one of 'Generic-Classifier', 'Generic-Detector', or 'Product-Recognizer'.
     """
-    VERSION = '0.1.2'
+    VERSION = '0.1.3'
     CACHE_ENABLED = False
 
     @dataclasses.dataclass
     class Inputs:
         dataset: torch.utils.data.Dataset
         class_names: typing.List[str]
         test_dataset: typing.Optional[torch.utils.data.Dataset] = None
@@ -44,14 +45,15 @@
     class Config:
         endpoint: str
         api_key: str
         task_type: typing.Literal['classification_multiclass', 'object_detection']
         azure_storage_blob_container_url: str
         budget_in_hours: int = 1
         keep_dataset: bool = False
+        model_kind: typing.Optional[typing.Literal['Generic-Classifier', 'Generic-Detector', 'Product-Recognizer']] = None
 
     @dataclasses.dataclass
     class Outputs:
         model_name: str
         accuracy_top1: typing.Optional[float] = None
         accuracy_top5: typing.Optional[float] = None
         average_precision: typing.Optional[float] = None
@@ -144,15 +146,16 @@
 
         for blob in container_client.list_blobs(name_starts_with=dataset_name):
             container_client.delete_blob(blob)
 
         self._uvs_client.unregister_dataset(dataset_name)
 
     def _train_model(self, dataset_name, model_name, test_dataset_name):
-        self._uvs_client.create_model(dataset_name, model_name, self.config.task_type, self.config.budget_in_hours, test_dataset_name)
+        model_kind = self.config.model_kind or {'classification_multiclass': 'Generic-Classifier', 'object_detection': 'Generic-Detector'}[self.config.task_type]
+        self._uvs_client.create_model(dataset_name, model_name, model_kind, self.config.budget_in_hours, test_dataset_name)
         logger.info(f"Training request sent. Waiting for training to complete... Training budget is {self.config.budget_in_hours} hours.")
         status = 'notstarted'
         while status in ['notstarted', 'training']:
             time.sleep(60)
             model = self._uvs_client.get_model(model_name)
             status = model['status'].lower()
 
@@ -187,23 +190,23 @@
         self._endpoint = endpoint
         self._headers = {'Ocp-Apim-Subscription-Key': api_key}
 
     @tenacity.retry(stop=tenacity.stop_after_attempt(3), retry=tenacity.retry_if_exception(_should_retry))
     def register_dataset(self, dataset_name, task_type, file_url):
         url = urllib.parse.urljoin(self._endpoint, f'/computervision/datasets/{dataset_name}?api-version=2023-04-01-preview')
         annotation_kind = {'classification_multiclass': 'imageClassification', 'object_detection': 'imageObjectDetection'}[task_type]
-        response = requests.put(url, headers=self._headers, json={'annotationKind': annotation_kind, 'annotationFileUris': [file_url]}, timeout=60)
+        request_body = {'annotationKind': annotation_kind, 'annotationFileUris': [file_url], 'authentication': {'kind': 'managedIdentity'}}
+        response = requests.put(url, headers=self._headers, json=request_body, timeout=60)
         response_json = response.json()
         logger.debug(f"API response: {response_json}")
         response.raise_for_status()
 
     @tenacity.retry(stop=tenacity.stop_after_attempt(3), retry=tenacity.retry_if_exception(_should_retry))
-    def create_model(self, dataset_name, model_name, task_type, budget_in_hours, test_dataset_name):
+    def create_model(self, dataset_name, model_name, model_kind, budget_in_hours, test_dataset_name):
         url = urllib.parse.urljoin(self._endpoint, f'/computervision/models/{model_name}?api-version=2023-04-01-preview')
-        model_kind = {'classification_multiclass': 'GenericClassifier', 'object_detection': 'GenericDetector'}[task_type]
         request_body = {'trainingParameters': {'timeBudgetInHours': budget_in_hours, 'trainingDatasetName': dataset_name, 'modelKind': model_kind}}
         if test_dataset_name:
             request_body['evaluationParameters'] = {'testDatasetName': test_dataset_name}
 
         response = requests.put(url, headers=self._headers, json=request_body, timeout=60)
         response_json = response.json()
         logger.debug(f"API response: {response_json}")
```

### Comparing `irisml-tasks-azure-computervision-0.0.5/irisml_tasks_azure_computervision.egg-info/PKG-INFO` & `irisml-tasks-azure-computervision-0.0.6/irisml_tasks_azure_computervision.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-azure-computervision
-Version: 0.0.5
+Version: 0.0.6
 Summary: Azure Computer Vision API tasks for IrisML
 Home-page: https://github.com/microsoft/irisml-tasks-azure-computervision
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-azure-computervision-0.0.5/irisml_tasks_azure_computervision.egg-info/SOURCES.txt` & `irisml-tasks-azure-computervision-0.0.6/irisml_tasks_azure_computervision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.5/setup.cfg` & `irisml-tasks-azure-computervision-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = irisml-tasks-azure-computervision
-version = 0.0.5
+version = 0.0.6
 url = https://github.com/microsoft/irisml-tasks-azure-computervision
 description = Azure Computer Vision API tasks for IrisML
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = irisdev
 license = MIT
```

### Comparing `irisml-tasks-azure-computervision-0.0.5/test/test_create_azure_computervision_caption_model.py` & `irisml-tasks-azure-computervision-0.0.6/test/test_create_azure_computervision_caption_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.5/test/test_create_azure_computervision_classification_model.py` & `irisml-tasks-azure-computervision-0.0.6/test/test_create_azure_computervision_classification_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.5/test/test_create_azure_computervision_custom_model.py` & `irisml-tasks-azure-computervision-0.0.6/test/test_create_azure_computervision_custom_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.5/test/test_create_azure_computervision_ocr_model.py` & `irisml-tasks-azure-computervision-0.0.6/test/test_create_azure_computervision_ocr_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.5/test/test_delete_azure_computervision_custom_model.py` & `irisml-tasks-azure-computervision-0.0.6/test/test_delete_azure_computervision_custom_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.5/test/test_train_azure_computervision_custom_model.py` & `irisml-tasks-azure-computervision-0.0.6/test/test_train_azure_computervision_custom_model.py`

 * *Files identical despite different names*

