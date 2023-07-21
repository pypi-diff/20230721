# Comparing `tmp/bert-for-sequence-classification-0.1.0.tar.gz` & `tmp/bert-for-sequence-classification-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert-for-sequence-classification-0.1.0.tar", last modified: Fri Jul 21 12:09:58 2023, max compression
+gzip compressed data, was "bert-for-sequence-classification-0.1.1.tar", last modified: Fri Jul 21 14:49:56 2023, max compression
```

## Comparing `bert-for-sequence-classification-0.1.0.tar` & `bert-for-sequence-classification-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:09:58.229441 bert-for-sequence-classification-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-21 12:09:58.229441 bert-for-sequence-classification-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:09:58.225441 bert-for-sequence-classification-0.1.0/bert_clf/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:09:58.225441 bert-for-sequence-classification-0.1.0/bert_clf/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:09:58.225441 bert-for-sequence-classification-0.1.0/bert_clf/src/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/core/BaseDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/core/BaseModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/core/Fabric.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/early_stopping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:09:58.229441 bert-for-sequence-classification-0.1.0/bert_clf/src/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/models/BertCLF.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/models/EncoderCLF.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:09:58.229441 bert-for-sequence-classification-0.1.0/bert_clf/src/pandas_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/pandas_dataset/PandasDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/pandas_dataset/SimpleDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/pandas_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/preparing_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/training_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:09:58.229441 bert-for-sequence-classification-0.1.0/bert_for_sequence_classification.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-21 12:09:58.000000 bert-for-sequence-classification-0.1.0/bert_for_sequence_classification.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-21 12:09:58.000000 bert-for-sequence-classification-0.1.0/bert_for_sequence_classification.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:09:58.000000 bert-for-sequence-classification-0.1.0/bert_for_sequence_classification.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 12:09:58.000000 bert-for-sequence-classification-0.1.0/bert_for_sequence_classification.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-21 12:09:58.000000 bert-for-sequence-classification-0.1.0/bert_for_sequence_classification.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 12:09:58.000000 bert-for-sequence-classification-0.1.0/bert_for_sequence_classification.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-21 12:09:58.229441 bert-for-sequence-classification-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:49:56.932968 bert-for-sequence-classification-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-21 14:49:56.932968 bert-for-sequence-classification-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:49:56.928968 bert-for-sequence-classification-0.1.1/bert_clf/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/bert_clf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/bert_clf/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:49:56.932968 bert-for-sequence-classification-0.1.1/bert_clf/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/bert_clf/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:49:56.932968 bert-for-sequence-classification-0.1.1/bert_clf/src/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/bert_clf/src/core/BaseDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/bert_clf/src/core/BaseModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/bert_clf/src/core/Fabric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/bert_clf/src/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/bert_clf/src/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/bert_clf/src/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/bert_clf/src/early_stopping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:49:56.932968 bert-for-sequence-classification-0.1.1/bert_clf/src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/bert_clf/src/models/BertCLF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/bert_clf/src/models/EncoderCLF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/bert_clf/src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:49:56.932968 bert-for-sequence-classification-0.1.1/bert_clf/src/pandas_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/bert_clf/src/pandas_dataset/PandasDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/bert_clf/src/pandas_dataset/SimpleDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/bert_clf/src/pandas_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/bert_clf/src/preparing_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/bert_clf/src/training_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/bert_clf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:49:56.932968 bert-for-sequence-classification-0.1.1/bert_for_sequence_classification.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-21 14:49:56.000000 bert-for-sequence-classification-0.1.1/bert_for_sequence_classification.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-21 14:49:56.000000 bert-for-sequence-classification-0.1.1/bert_for_sequence_classification.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:49:56.000000 bert-for-sequence-classification-0.1.1/bert_for_sequence_classification.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 14:49:56.000000 bert-for-sequence-classification-0.1.1/bert_for_sequence_classification.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-21 14:49:56.000000 bert-for-sequence-classification-0.1.1/bert_for_sequence_classification.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 14:49:56.000000 bert-for-sequence-classification-0.1.1/bert_for_sequence_classification.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-21 14:49:56.932968 bert-for-sequence-classification-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-21 14:49:42.000000 bert-for-sequence-classification-0.1.1/setup.py
```

### Comparing `bert-for-sequence-classification-0.1.0/LICENSE` & `bert-for-sequence-classification-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.1.0/PKG-INFO` & `bert-for-sequence-classification-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert-for-sequence-classification
-Version: 0.1.0
+Version: 0.1.1
 Summary: Easy fine-tuning for BERT models
 Author: Tatiana Iazykova
 Author-email: tania_yazykova@bk.ru
 Keywords: python,bert,deep learning,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `bert-for-sequence-classification-0.1.0/README.md` & `bert-for-sequence-classification-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.1.0/bert_clf/pipeline.py` & `bert-for-sequence-classification-0.1.1/bert_clf/pipeline.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.1.0/bert_clf/src/core/BaseDataset.py` & `bert-for-sequence-classification-0.1.1/bert_clf/src/core/BaseDataset.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.1.0/bert_clf/src/core/BaseModel.py` & `bert-for-sequence-classification-0.1.1/bert_clf/src/core/BaseModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 import os
 from typing import Dict, Optional
 
+import requests
 import torch
 import torch.nn as nn
+from tqdm.auto import tqdm
 from transformers import AutoTokenizer
 from abc import abstractmethod
 
 
 class BaseCLF(nn.Module):
 
     def __init__(
```

### Comparing `bert-for-sequence-classification-0.1.0/bert_clf/src/core/Fabric.py` & `bert-for-sequence-classification-0.1.1/bert_clf/src/core/Fabric.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.1.0/bert_clf/src/dataset.py` & `bert-for-sequence-classification-0.1.1/bert_clf/src/dataset.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.1.0/bert_clf/src/early_stopping.py` & `bert-for-sequence-classification-0.1.1/bert_clf/src/early_stopping.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.1.0/bert_clf/src/models/BertCLF.py` & `bert-for-sequence-classification-0.1.1/bert_clf/src/models/BertCLF.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.1.0/bert_clf/src/models/EncoderCLF.py` & `bert-for-sequence-classification-0.1.1/bert_clf/src/models/EncoderCLF.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import json
 import os
 from typing import Dict, Optional
 
 import torch
 import torch.nn as nn
+import wget
 from transformers import AutoModel, AutoConfig
 
 from bert_clf.src.core import BaseCLF
+from bert_clf.src.core.utils import SUPPORTED_MODELS
 
 
 class EncoderCLF(BaseCLF):
 
     def __init__(
             self,
             pretrained_model_name: str,
@@ -31,14 +33,41 @@
             self.fc = nn.Linear(out, len(self.mapper))
             self.load_state_dict(
                 torch.load(
                     os.path.join(pretrained_model_name, "state_dict.pth"), map_location='cpu'
                 )
             )
 
+        elif pretrained_model_name in SUPPORTED_MODELS:
+            self.pretrained_model = AutoModel.from_config(
+                AutoConfig.from_pretrained(self.tokenizer.name_or_path)
+            ).encoder
+
+            out = self.pretrained_model.config.d_model
+
+            id2label_path = os.path.expanduser("~/.cache/huggingface/language_identification_id2label.json")
+            state_dict_path = os.path.expanduser("~/.cache/huggingface/language_identification_state_dict.pth")
+
+            wget.download(
+                SUPPORTED_MODELS[pretrained_model_name]['id2label'],
+                id2label_path
+            )
+
+            with open(id2label_path) as f:
+                self.mapper = json.load(f)
+                self.mapper = {int(k): v for k, v in self.mapper.items()}
+            self.fc = nn.Linear(out, len(self.mapper))
+
+            wget.download(
+                SUPPORTED_MODELS[pretrained_model_name]['state_dict'],
+                state_dict_path
+            )
+
+            self.load_state_dict(torch.load(state_dict_path, map_location='cpu'))
+
         else:
             self.mapper = id2label
             self.pretrained_model = AutoModel.from_pretrained(
                 pretrained_model_name_or_path=pretrained_model_name).encoder
             out = self.pretrained_model.config.d_model
             self.fc = nn.Linear(out, len(self.mapper))
```

### Comparing `bert-for-sequence-classification-0.1.0/bert_clf/src/pandas_dataset/PandasDataset.py` & `bert-for-sequence-classification-0.1.1/bert_clf/src/pandas_dataset/PandasDataset.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.1.0/bert_clf/src/pandas_dataset/SimpleDataFrame.py` & `bert-for-sequence-classification-0.1.1/bert_clf/src/pandas_dataset/SimpleDataFrame.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.1.0/bert_clf/src/preparing_data_utils.py` & `bert-for-sequence-classification-0.1.1/bert_clf/src/preparing_data_utils.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.1.0/bert_clf/src/training_utils.py` & `bert-for-sequence-classification-0.1.1/bert_clf/src/training_utils.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.1.0/bert_clf/utils.py` & `bert-for-sequence-classification-0.1.1/bert_clf/utils.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.1.0/bert_for_sequence_classification.egg-info/PKG-INFO` & `bert-for-sequence-classification-0.1.1/bert_for_sequence_classification.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert-for-sequence-classification
-Version: 0.1.0
+Version: 0.1.1
 Summary: Easy fine-tuning for BERT models
 Author: Tatiana Iazykova
 Author-email: tania_yazykova@bk.ru
 Keywords: python,bert,deep learning,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `bert-for-sequence-classification-0.1.0/bert_for_sequence_classification.egg-info/SOURCES.txt` & `bert-for-sequence-classification-0.1.1/bert_for_sequence_classification.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 bert_clf/src/early_stopping.py
 bert_clf/src/preparing_data_utils.py
 bert_clf/src/training_utils.py
 bert_clf/src/core/BaseDataset.py
 bert_clf/src/core/BaseModel.py
 bert_clf/src/core/Fabric.py
 bert_clf/src/core/__init__.py
+bert_clf/src/core/utils.py
 bert_clf/src/models/BertCLF.py
 bert_clf/src/models/EncoderCLF.py
 bert_clf/src/models/__init__.py
 bert_clf/src/pandas_dataset/PandasDataset.py
 bert_clf/src/pandas_dataset/SimpleDataFrame.py
 bert_clf/src/pandas_dataset/__init__.py
 bert_for_sequence_classification.egg-info/PKG-INFO
```

### Comparing `bert-for-sequence-classification-0.1.0/setup.py` & `bert-for-sequence-classification-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bert-for-sequence-classification",
-    version='0.1.0',
+    version='0.1.1',
     author="Tatiana Iazykova",
     author_email="tania_yazykova@bk.ru",
     description='Easy fine-tuning for BERT models',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'bert-clf-train = bert_clf.pipeline:main',
         ],
     },
     install_requires=[
-        'transformers>=4.2.0',
+        'transformers>=4.21.0',
         'torch>=1.7.1',
         'numpy>=1.19.5',
         'pandas>=1.1.5',
         'scikit-learn>=1.0',
         'pyyaml>=6.0',
         'openpyxl>=3.0.9',
+        'wget',
+        'tqdm'
     ],
 
     keywords=['python', 'bert', 'deep learning', 'nlp'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

