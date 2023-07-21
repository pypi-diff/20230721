# Comparing `tmp/bert-for-sequence-classification-0.0.8.tar.gz` & `tmp/bert-for-sequence-classification-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert-for-sequence-classification-0.0.8.tar", last modified: Wed Jul 19 12:43:53 2023, max compression
+gzip compressed data, was "bert-for-sequence-classification-0.1.0.tar", last modified: Fri Jul 21 12:09:58 2023, max compression
```

## Comparing `bert-for-sequence-classification-0.0.8.tar` & `bert-for-sequence-classification-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:43:53.227833 bert-for-sequence-classification-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-19 12:43:53.227833 bert-for-sequence-classification-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:43:53.223833 bert-for-sequence-classification-0.0.8/bert_clf/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/bert_clf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/bert_clf/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:43:53.227833 bert-for-sequence-classification-0.0.8/bert_clf/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/bert_clf/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:43:53.227833 bert-for-sequence-classification-0.0.8/bert_clf/src/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/bert_clf/src/core/BaseDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/bert_clf/src/core/BaseModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/bert_clf/src/core/CLFFabric.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/bert_clf/src/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/bert_clf/src/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/bert_clf/src/early_stopping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:43:53.227833 bert-for-sequence-classification-0.0.8/bert_clf/src/models/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/bert_clf/src/models/BertCLF.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/bert_clf/src/models/EncoderCLF.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/bert_clf/src/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:43:53.227833 bert-for-sequence-classification-0.0.8/bert_clf/src/pandas_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/bert_clf/src/pandas_dataset/PandasDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/bert_clf/src/pandas_dataset/SimpleDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/bert_clf/src/pandas_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/bert_clf/src/preparing_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/bert_clf/src/training_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/bert_clf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:43:53.227833 bert-for-sequence-classification-0.0.8/bert_for_sequence_classification.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-19 12:43:53.000000 bert-for-sequence-classification-0.0.8/bert_for_sequence_classification.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-19 12:43:53.000000 bert-for-sequence-classification-0.0.8/bert_for_sequence_classification.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:43:53.000000 bert-for-sequence-classification-0.0.8/bert_for_sequence_classification.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-19 12:43:53.000000 bert-for-sequence-classification-0.0.8/bert_for_sequence_classification.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-19 12:43:53.000000 bert-for-sequence-classification-0.0.8/bert_for_sequence_classification.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 12:43:53.000000 bert-for-sequence-classification-0.0.8/bert_for_sequence_classification.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-19 12:43:53.227833 bert-for-sequence-classification-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-19 12:43:39.000000 bert-for-sequence-classification-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:09:58.229441 bert-for-sequence-classification-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-21 12:09:58.229441 bert-for-sequence-classification-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:09:58.225441 bert-for-sequence-classification-0.1.0/bert_clf/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:09:58.225441 bert-for-sequence-classification-0.1.0/bert_clf/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:09:58.225441 bert-for-sequence-classification-0.1.0/bert_clf/src/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/core/BaseDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/core/BaseModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/core/Fabric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/early_stopping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:09:58.229441 bert-for-sequence-classification-0.1.0/bert_clf/src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/models/BertCLF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/models/EncoderCLF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:09:58.229441 bert-for-sequence-classification-0.1.0/bert_clf/src/pandas_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/pandas_dataset/PandasDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/pandas_dataset/SimpleDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/pandas_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/preparing_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/src/training_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/bert_clf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:09:58.229441 bert-for-sequence-classification-0.1.0/bert_for_sequence_classification.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-21 12:09:58.000000 bert-for-sequence-classification-0.1.0/bert_for_sequence_classification.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-21 12:09:58.000000 bert-for-sequence-classification-0.1.0/bert_for_sequence_classification.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:09:58.000000 bert-for-sequence-classification-0.1.0/bert_for_sequence_classification.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 12:09:58.000000 bert-for-sequence-classification-0.1.0/bert_for_sequence_classification.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-21 12:09:58.000000 bert-for-sequence-classification-0.1.0/bert_for_sequence_classification.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 12:09:58.000000 bert-for-sequence-classification-0.1.0/bert_for_sequence_classification.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-21 12:09:58.229441 bert-for-sequence-classification-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-21 12:09:43.000000 bert-for-sequence-classification-0.1.0/setup.py
```

### Comparing `bert-for-sequence-classification-0.0.8/LICENSE` & `bert-for-sequence-classification-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.8/PKG-INFO` & `bert-for-sequence-classification-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert-for-sequence-classification
-Version: 0.0.8
+Version: 0.1.0
 Summary: Easy fine-tuning for BERT models
 Author: Tatiana Iazykova
 Author-email: tania_yazykova@bk.ru
 Keywords: python,bert,deep learning,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `bert-for-sequence-classification-0.0.8/README.md` & `bert-for-sequence-classification-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.8/bert_clf/pipeline.py` & `bert-for-sequence-classification-0.1.0/bert_clf/pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import os
 
 import numpy as np
 import torch
 import torch.optim as optim
 from sklearn.utils.class_weight import compute_class_weight
 
@@ -77,31 +76,15 @@
         criterion=criterion,
         optimizer=optimizer,
         num_epochs=config['training']['num_epochs'],
         average=config['training']['average_f1'],
         config=config
     )
 
-    if config['training']['save_state_dict']:
-        torch.save(
-            model.state_dict(),
-            os.path.join(config["training"]["output_dir"], "model.pth"),
-        )
-
-        with open(
-                os.path.join(config["training"]["output_dir"], 'label_mapper.json'),
-                mode='w',
-                encoding='utf-8'
-        ) as f:
-            json.dump(model.mapper, f, indent=4, ensure_ascii=False)
-    else:
-        torch.save(
-            model,
-            os.path.join(config["training"]["output_dir"], "model.pth"),
-        )
+    model.save_pretrained(path=config['training']['output_dir'])
 
 
 def main():
     parser = get_argparse()
     args = parser.parse_args()
 
     train(path_to_config=args.path_to_config)
```

### Comparing `bert-for-sequence-classification-0.0.8/bert_clf/src/core/BaseDataset.py` & `bert-for-sequence-classification-0.1.0/bert_clf/src/core/BaseDataset.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.8/bert_clf/src/core/BaseModel.py` & `bert-for-sequence-classification-0.1.0/bert_clf/src/core/BaseModel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from typing import Dict
+import json
+import os
+from typing import Dict, Optional
 
 import torch
 import torch.nn as nn
-from transformers import AutoTokenizer, AutoModel
+from transformers import AutoTokenizer
 from abc import abstractmethod
 
 
 class BaseCLF(nn.Module):
 
     def __init__(
             self,
             pretrained_model_name: str,
-            id2label: Dict[int, str],
-            dropout: float,
+            dropout: Optional[float] = 1e-6,
     ):
         super().__init__()
         self.tokenizer = AutoTokenizer.from_pretrained(pretrained_model_name_or_path=pretrained_model_name)
-        self.pretrained_model = AutoModel.from_pretrained(pretrained_model_name_or_path=pretrained_model_name)
         self.drop = nn.Dropout(dropout)
         self.act = nn.LogSoftmax(1)
-        self.mapper = id2label
-
 
     @abstractmethod
     def forward(self, texts: torch.Tensor) -> torch.Tensor:
         raise NotImplementedError
 
     def _predict(self, text: str) -> torch.Tensor:
         inputs = self.tokenizer.encode(text, return_tensors="pt", truncation=True)
@@ -42,7 +40,17 @@
     def predict_proba(self, text: str) -> Dict[str, float]:
         self.eval()
         with torch.no_grad():
             outputs = self._predict(text=text)
             probas = torch.nn.functional.softmax(outputs, dim=1).cpu().detach().numpy().tolist()[0]
             probas_dict = {self.mapper[i]: proba for i, proba in enumerate(probas)}
         return probas_dict
+
+    def save_pretrained(self, path: str):
+        self.tokenizer.save_pretrained(path)
+        self.pretrained_model.config.save_pretrained(path)
+        torch.save(
+            self.state_dict(),
+            os.path.join(path, "state_dict.pth")
+        )
+        with open(os.path.join(path, 'id2label.json'), mode='w', encoding='utf-8') as f:
+            json.dump(self.mapper, f, indent=4, ensure_ascii=False)
```

### Comparing `bert-for-sequence-classification-0.0.8/bert_clf/src/core/CLFFabric.py` & `bert-for-sequence-classification-0.1.0/bert_clf/src/core/Fabric.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.8/bert_clf/src/dataset.py` & `bert-for-sequence-classification-0.1.0/bert_clf/src/dataset.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.8/bert_clf/src/early_stopping.py` & `bert-for-sequence-classification-0.1.0/bert_clf/src/early_stopping.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.8/bert_clf/src/models/BertCLF.py` & `bert-for-sequence-classification-0.1.0/bert_clf/src/models/BertCLF.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,50 @@
-from typing import Dict
+import json
+import os
+from typing import Dict, Optional
 
 import torch
+from transformers import AutoModel, AutoConfig
 
 from bert_clf.src.core import BaseCLF
 import torch.nn as nn
 
 
 class BertCLF(BaseCLF):
 
     def __init__(
             self,
             pretrained_model_name: str,
-            id2label: Dict[int, str],
-            dropout: float,
+            id2label: Optional[Dict[int, str]] = None,
+            dropout: Optional[float] = 1e-6,
     ):
-        super().__init__(pretrained_model_name=pretrained_model_name, id2label=id2label, dropout=dropout)
-        out_bert = self.pretrained_model.config.hidden_size
-        self.fc = nn.Linear(out_bert, len(self.mapper))
+        super().__init__(pretrained_model_name=pretrained_model_name, dropout=dropout)
+
+        if os.path.exists(pretrained_model_name):
+            self.pretrained_model = AutoModel.from_config(
+                AutoConfig.from_pretrained(self.tokenizer.name_or_path)
+            )
+            out_bert = self.pretrained_model.config.hidden_size
+
+            with open(os.path.join(pretrained_model_name, "id2label.json")) as f:
+                self.mapper = json.load(f)
+                self.mapper = {int(k): v for k, v in self.mapper.items()}
+            self.fc = nn.Linear(out_bert, len(self.mapper))
+            self.load_state_dict(
+                torch.load(
+                    os.path.join(pretrained_model_name, "state_dict.pth"), map_location='cpu'
+                )
+            )
+
+        else:
+            self.mapper = id2label
+            self.pretrained_model = AutoModel.from_pretrained(
+                pretrained_model_name_or_path=pretrained_model_name)
+            out_bert = self.pretrained_model.config.hidden_size
+            self.fc = nn.Linear(out_bert, len(self.mapper))
 
     def forward(self, texts: torch.Tensor) -> torch.Tensor:
         mask = (texts != self.tokenizer.pad_token_id).long()
 
         hidden = self.pretrained_model(texts, attention_mask=mask)[0]
 
         dense_outputs = self.fc(self.drop(hidden[:, 0]))
```

### Comparing `bert-for-sequence-classification-0.0.8/bert_clf/src/models/EncoderCLF.py` & `bert-for-sequence-classification-0.1.0/bert_clf/src/models/EncoderCLF.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,50 @@
-from typing import Dict
+import json
+import os
+from typing import Dict, Optional
 
 import torch
 import torch.nn as nn
+from transformers import AutoModel, AutoConfig
 
 from bert_clf.src.core import BaseCLF
 
 
 class EncoderCLF(BaseCLF):
 
     def __init__(
             self,
             pretrained_model_name: str,
-            id2label: Dict[int, str],
-            dropout: float,
+            id2label: Optional[Dict[int, str]] = None,
+            dropout: Optional[float] = 1e-6,
     ):
-        super().__init__(pretrained_model_name=pretrained_model_name, id2label=id2label, dropout=dropout)
-        out = self.pretrained_model.config.d_model
-        self.fc = nn.Linear(out, len(self.mapper))
-        self.pretrained_model = self.pretrained_model.encoder
+        super().__init__(pretrained_model_name=pretrained_model_name, dropout=dropout)
+
+        if os.path.exists(pretrained_model_name):
+            self.pretrained_model = AutoModel.from_config(
+                AutoConfig.from_pretrained(self.tokenizer.name_or_path)
+            ).encoder
+            out = self.pretrained_model.config.d_model
+
+            with open(os.path.join(pretrained_model_name, "id2label.json")) as f:
+                self.mapper = json.load(f)
+                self.mapper = {int(k): v for k, v in self.mapper.items()}
+            self.fc = nn.Linear(out, len(self.mapper))
+            self.load_state_dict(
+                torch.load(
+                    os.path.join(pretrained_model_name, "state_dict.pth"), map_location='cpu'
+                )
+            )
+
+        else:
+            self.mapper = id2label
+            self.pretrained_model = AutoModel.from_pretrained(
+                pretrained_model_name_or_path=pretrained_model_name).encoder
+            out = self.pretrained_model.config.d_model
+            self.fc = nn.Linear(out, len(self.mapper))
 
     def forward(self, texts: torch.Tensor) -> torch.Tensor:
         mask = (texts != self.tokenizer.pad_token_id).long()
 
         hidden = self.pretrained_model(texts, attention_mask=mask)['last_hidden_state']
         hidden = hidden * mask.unsqueeze(-1)
         hidden = hidden.sum(dim=1) / mask.sum(dim=1).unsqueeze(-1)
```

### Comparing `bert-for-sequence-classification-0.0.8/bert_clf/src/pandas_dataset/PandasDataset.py` & `bert-for-sequence-classification-0.1.0/bert_clf/src/pandas_dataset/PandasDataset.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.8/bert_clf/src/pandas_dataset/SimpleDataFrame.py` & `bert-for-sequence-classification-0.1.0/bert_clf/src/pandas_dataset/SimpleDataFrame.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.8/bert_clf/src/preparing_data_utils.py` & `bert-for-sequence-classification-0.1.0/bert_clf/src/preparing_data_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     :param config: config with  all the necessary information for handling the data
     :param df: class object that has train and valid data
 
     :return: mapper and separated texts and labels
     """
 
-    id2label = {i: l for i, l in enumerate(df.train[config['data']['target_column']].unique())}
+    id2label = {i: l for i, l in enumerate(df.train[config['data']['target_column']].unique().tolist())}
     label2id = {l: i for i, l in id2label.items()}
     train_texts = df.train[config['data']['text_column']].to_list()
     valid_texts = df.test[config['data']['text_column']].to_list()
     train_targets = df.train[config['data']['target_column']].map(label2id).to_list()
 
     if len(set(df.test[config['data']['target_column']].to_list()).intersection(label2id)) != len(label2id):
         raise ValueError('Some labels in test are not present in train')
```

### Comparing `bert-for-sequence-classification-0.0.8/bert_clf/src/training_utils.py` & `bert-for-sequence-classification-0.1.0/bert_clf/src/training_utils.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.8/bert_clf/utils.py` & `bert-for-sequence-classification-0.1.0/bert_clf/utils.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.8/bert_for_sequence_classification.egg-info/PKG-INFO` & `bert-for-sequence-classification-0.1.0/bert_for_sequence_classification.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert-for-sequence-classification
-Version: 0.0.8
+Version: 0.1.0
 Summary: Easy fine-tuning for BERT models
 Author: Tatiana Iazykova
 Author-email: tania_yazykova@bk.ru
 Keywords: python,bert,deep learning,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `bert-for-sequence-classification-0.0.8/bert_for_sequence_classification.egg-info/SOURCES.txt` & `bert-for-sequence-classification-0.1.0/bert_for_sequence_classification.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 bert_clf/src/__init__.py
 bert_clf/src/dataset.py
 bert_clf/src/early_stopping.py
 bert_clf/src/preparing_data_utils.py
 bert_clf/src/training_utils.py
 bert_clf/src/core/BaseDataset.py
 bert_clf/src/core/BaseModel.py
-bert_clf/src/core/CLFFabric.py
+bert_clf/src/core/Fabric.py
 bert_clf/src/core/__init__.py
 bert_clf/src/models/BertCLF.py
 bert_clf/src/models/EncoderCLF.py
 bert_clf/src/models/__init__.py
 bert_clf/src/pandas_dataset/PandasDataset.py
 bert_clf/src/pandas_dataset/SimpleDataFrame.py
 bert_clf/src/pandas_dataset/__init__.py
```

### Comparing `bert-for-sequence-classification-0.0.8/setup.py` & `bert-for-sequence-classification-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bert-for-sequence-classification",
-    version='0.0.8',
+    version='0.1.0',
     author="Tatiana Iazykova",
     author_email="tania_yazykova@bk.ru",
     description='Easy fine-tuning for BERT models',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'bert-clf-train = bert_clf.pipeline:main',
```

