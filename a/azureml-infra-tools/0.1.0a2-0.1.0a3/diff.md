# Comparing `tmp/azureml_infra_tools-0.1.0a2.tar.gz` & `tmp/azureml_infra_tools-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azureml_infra_tools-0.1.0a2.tar", max compression
+gzip compressed data, was "azureml_infra_tools-0.1.0a3.tar", max compression
```

## Comparing `azureml_infra_tools-0.1.0a2.tar` & `azureml_infra_tools-0.1.0a3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-07-21 10:24:32.903782 azureml_infra_tools-0.1.0a2/LICENSE
--rw-r--r--   0        0        0     2699 2023-07-21 10:24:32.903782 azureml_infra_tools-0.1.0a2/README.md
--rw-r--r--   0        0        0     2079 2023-07-21 10:24:32.903782 azureml_infra_tools-0.1.0a2/azureml_infra_tools/__init__.py
--rw-r--r--   0        0        0     2415 2023-07-21 10:24:32.903782 azureml_infra_tools-0.1.0a2/azureml_infra_tools/cluster.py
--rw-r--r--   0        0        0     2868 2023-07-21 10:24:32.903782 azureml_infra_tools-0.1.0a2/azureml_infra_tools/credential.py
--rw-r--r--   0        0        0     1980 2023-07-21 10:24:32.903782 azureml_infra_tools-0.1.0a2/azureml_infra_tools/data.py
--rw-r--r--   0        0        0     2058 2023-07-21 10:24:32.903782 azureml_infra_tools-0.1.0a2/azureml_infra_tools/environment.py
--rw-r--r--   0        0        0      824 2023-07-21 10:24:32.907782 azureml_infra_tools-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     3604 1970-01-01 00:00:00.000000 azureml_infra_tools-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-21 11:51:19.763363 azureml_infra_tools-0.1.0a3/LICENSE
+-rw-r--r--   0        0        0     5826 2023-07-21 11:51:19.763363 azureml_infra_tools-0.1.0a3/README.md
+-rw-r--r--   0        0        0     3876 2023-07-21 11:51:19.763363 azureml_infra_tools-0.1.0a3/azureml_infra_tools/__init__.py
+-rw-r--r--   0        0        0     3489 2023-07-21 11:51:19.763363 azureml_infra_tools-0.1.0a3/azureml_infra_tools/cluster.py
+-rw-r--r--   0        0        0     3355 2023-07-21 11:51:19.763363 azureml_infra_tools-0.1.0a3/azureml_infra_tools/credential.py
+-rw-r--r--   0        0        0     2931 2023-07-21 11:51:19.763363 azureml_infra_tools-0.1.0a3/azureml_infra_tools/data.py
+-rw-r--r--   0        0        0     3283 2023-07-21 11:51:19.763363 azureml_infra_tools-0.1.0a3/azureml_infra_tools/environment.py
+-rw-r--r--   0        0        0      824 2023-07-21 11:51:19.763363 azureml_infra_tools-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0     6731 1970-01-01 00:00:00.000000 azureml_infra_tools-0.1.0a3/PKG-INFO
```

### Comparing `azureml_infra_tools-0.1.0a2/LICENSE` & `azureml_infra_tools-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `azureml_infra_tools-0.1.0a2/azureml_infra_tools/data.py` & `azureml_infra_tools-0.1.0a3/azureml_infra_tools/data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,68 @@
 """ Azure Data Class to upload data to Azure Machine Learning Studio
+
+Main functionalities:
+The AzureData class is designed to upload data to Azure Machine Learning Studio. It takes an AzureCredential object as
+input to authenticate with the Azure Machine Learning Studio. The class allows users to upload data to the studio and
+reuse existing datasets if they already exist.
+
+Methods:
+- __init__(self, azure_credential: AzureCredential, data_path: str, data_name: str, data_description: str, data_version:
+str): Initializes the AzureData object with the given parameters.
+- upload_data(self) -> Data: Uploads data to Azure Machine Learning Studio and returns the Azure Data object.
+
+Fields:
+- azure_credential: An AzureCredential object used to authenticate with Azure Machine Learning Studio.
+- data_path: The path to the data to be uploaded.
+- data_name: The name of the dataset.
+- data_description: A description of the dataset.
+- data_version: The version of the dataset.
 """
+
 from azure.ai.ml.constants import AssetTypes
 from azure.ai.ml.entities import Data
+import logging
 
 from azureml_infra_tools.credential import AzureCredential
 
 
-# import time
-
-
 class AzureData:
     """Azure Data Class
-    @param azure_credential: Azure Machine Learning client
-    @param data_path: (str) Path to data
-    @param dataset_name: (str) Name of dataset
-    @param dataset_description: (str) Description of dataset
-    @param data_version: (str) Version of dataset
+    @param azure_credential: (AzureCredential) An AzureCredential object used to authenticate with Azure Machine
+    Learning Studio.
+    @param data_path: (str) The path to the data to be uploaded.
+    @param data_name: (str) The name of the dataset.
+    @param data_description: (str) A description of the dataset.
+    @param data_version: (str) The version of the dataset.
     """
     data_version: str
 
-    def __init__(self, azure_credential: AzureCredential, data_path: str, dataset_name: str,
-                 dataset_description: str):
+    def __init__(self, azure_credential: AzureCredential, data_path: str, data_name: str,
+                 data_description: str, data_version: str):
         self.azure_credential = azure_credential
         self.data_path = data_path
-        self.dataset_name = dataset_name
-        self.dataset_description = dataset_description
-        # self.data_version = time.strftime("%Y.%m.%d.%H-%M-%S", time.gmtime())
-        self.data_version = "2023.07.11.14-33-41"
+        self.data_name = data_name
+        self.data_description = data_description
+        self.data_version = data_version
 
     def upload_data(self) -> Data:
         """Upload data to Azure Machine Learning Studio
         @return: Azure Data
         """
         try:
-            azure_data = self.azure_credential.ml_client.data.get(name=self.dataset_name, version="2023.07.11.14-33-41")
-            print(f"You already have a dataset named {self.dataset_name}, with the version "
-                  f"{self.data_version} we'll reuse it as is.")
+            azure_data = self.azure_credential.ml_client.data.get(name=self.data_name, version=self.data_version)
+            logging.info(f"You already have a dataset named {self.data_name}, with the version "
+                         f"{self.data_version} we'll reuse it as is.")
             return azure_data
         except Exception:
-            print("Uploading data to Azure Machine Learning Studio...")
+            logging.info("Uploading data to Azure Machine Learning Studio...")
             azure_data = Data(
-                name=self.dataset_name,
+                name=self.data_name,
                 version=self.data_version,
-                description=self.dataset_description,
+                description=self.data_description,
                 path=self.data_path,
                 type=AssetTypes.URI_FILE,
             )
             self.azure_credential.ml_client.data.create_or_update(azure_data)
-            print("Data uploaded successfully!")
+            logging.info("Data uploaded successfully!")
 
-            return azure_data
+            return azure_data
```

### Comparing `azureml_infra_tools-0.1.0a2/pyproject.toml` & `azureml_infra_tools-0.1.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "azureml-infra-tools"
-version = "0.1.0a2"
+version = "0.1.0a3"
 description = "azureml-infra-tools is a Python package providing high-level APIs for Azure Machine Learning. It simplifies setup of Azure ML infrastructures, manages datasets, and streamlines authentication. Designed for AI researchers, data scientists, and ML engineers, it boosts productivity and accelerates Azure ML projects."
 authors = ["Henrique Malta <vlezyitalia@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

