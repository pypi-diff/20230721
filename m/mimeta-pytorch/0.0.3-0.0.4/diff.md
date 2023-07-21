# Comparing `tmp/mimeta_pytorch-0.0.3.tar.gz` & `tmp/mimeta_pytorch-0.0.4.tar.gz`

## Comparing `mimeta_pytorch-0.0.3.tar` & `mimeta_pytorch-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/requirements.txt
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/examples/cross_domain_maml.py
--rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/examples/cross_domain_pretraining.py
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/examples/imagenet-pretrained.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/mimeta/__init__.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/mimeta/batches.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/mimeta/logger.py
--rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/mimeta/mimeta.py
--rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/mimeta/task_presampling.py
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/mimeta/tasks.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/LICENSE
--rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/LICENSE.LESSER
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/README.md
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.4/examples/cross_domain_maml.py
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.4/examples/cross_domain_pretraining.py
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.4/examples/imagenet-pretrained.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.4/mimeta/__init__.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.4/mimeta/batches.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.4/mimeta/logger.py
+-rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.4/mimeta/mimeta.py
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.4/mimeta/task_presampling.py
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.4/mimeta/tasks.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.4/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.4/LICENSE
+-rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.4/LICENSE.LESSER
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.4/README.md
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.4/PKG-INFO
```

### Comparing `mimeta_pytorch-0.0.3/examples/cross_domain_maml.py` & `mimeta_pytorch-0.0.4/examples/cross_domain_maml.py`

 * *Files identical despite different names*

### Comparing `mimeta_pytorch-0.0.3/examples/cross_domain_pretraining.py` & `mimeta_pytorch-0.0.4/examples/cross_domain_pretraining.py`

 * *Files identical despite different names*

### Comparing `mimeta_pytorch-0.0.3/examples/imagenet-pretrained.py` & `mimeta_pytorch-0.0.4/examples/imagenet-pretrained.py`

 * *Files identical despite different names*

### Comparing `mimeta_pytorch-0.0.3/mimeta/batches.py` & `mimeta_pytorch-0.0.4/mimeta/batches.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional, Callable
 
-from torchcross.data import RandomChainTaskSource, BatchedTaskSource
+from torchcross.data import RandomInterleaveDataset, BatchedTaskSource
 from .logger import logger
 from .mimeta import MIMeta
 
 
-class MultiMIMetaBatchTaskSource(RandomChainTaskSource):
+class MultiMIMetaBatchTaskSource(RandomInterleaveDataset):
     def __init__(
         self,
         mimeta_data_path: str,
         task_ids: list[tuple[str, str]],
         batch_size: int,
         shuffle: bool = True,
         drop_last: bool = False,
@@ -42,11 +42,12 @@
         batched_task_sources = [
             BatchedTaskSource(
                 task_source=task_source,
                 batch_size=batch_size,
                 shuffle=shuffle,
                 drop_last=drop_last,
                 collate_fn=collate_fn,
+                with_task_description=True,
             )
             for task_source in unbatched_task_sources
         ]
         super().__init__(batched_task_sources)
```

### Comparing `mimeta_pytorch-0.0.3/mimeta/mimeta.py` & `mimeta_pytorch-0.0.4/mimeta/mimeta.py`

 * *Files identical despite different names*

### Comparing `mimeta_pytorch-0.0.3/mimeta/task_presampling.py` & `mimeta_pytorch-0.0.4/mimeta/task_presampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,13 +121,13 @@
     parser.add_argument("--save_path", type=str, default="data/MIMeta_presampled")
     args = parser.parse_args()
     data_path = args.data_path
     save_path = args.save_path
 
     print("Available tasks:")
     print(available_tasks(data_path))
-    #save_few_shot_tasks(data_path, save_path)
+    save_few_shot_tasks(data_path, save_path)
     save_random_few_shot_tasks(data_path, save_path)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `mimeta_pytorch-0.0.3/mimeta/tasks.py` & `mimeta_pytorch-0.0.4/mimeta/tasks.py`

 * *Files identical despite different names*

### Comparing `mimeta_pytorch-0.0.3/LICENSE` & `mimeta_pytorch-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mimeta_pytorch-0.0.3/LICENSE.LESSER` & `mimeta_pytorch-0.0.4/LICENSE.LESSER`

 * *Files identical despite different names*

### Comparing `mimeta_pytorch-0.0.3/README.md` & `mimeta_pytorch-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 for generating batches from multiple MIMeta tasks and for generating few-shot insttances
 of multiple MIMeta tasks.
 
 ### Examples
 
 See the [examples](examples) directory for examples on how to use MIMeta in conjunction
 with TorchCross.
-- [`imagenet_pretrained.py`](examples/imagenet_pretraining.py) shows how you can test
+- [`imagenet_pretrained.py`](examples/imagenet_pretrained.py) shows how you can test
   pre-trained models on a few-shot instance of a MIMeta task.
 - [`cross_domain_pretraining.py`](examples/cross_domain_pretraining.py) shows how you
   can perform cross-domain pre-training on different MIMeta tasks and then test the
   pre-trained model on a few-shot instance of a MIMeta task.
 - [`cross_domain_maml.py`](examples/cross_domain_maml.py) shows how you can perform
   cross-domain meta-learning with [MAML](https://arxiv.org/abs/1703.03400) on different
   MIMeta tasks and then test the meta-learned model on multiple few-shot instances of a
```

### Comparing `mimeta_pytorch-0.0.3/pyproject.toml` & `mimeta_pytorch-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mimeta-pytorch"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="Stefano Woerner", email="stefano@woerner.eu" },
 ]
 description = "Library for using the MIMeta dataset"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -26,13 +26,13 @@
 dependencies = [
     "h5py~=3.8.0",
     "numpy~=1.24.3",
     "torch~=2.0.0",
     "PyYAML~=6.0",
     "Pillow~=9.5.0",
     "torchvision~=0.15.1",
-    "torchcross~=0.0.3",
+    "torchcross~=0.0.4",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/StefanoWoerner/mimeta-pytorch"
 "Issue Tracker" = "https://github.com/StefanoWoerner/mimeta-pytorch/issues"
```

### Comparing `mimeta_pytorch-0.0.3/PKG-INFO` & `mimeta_pytorch-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeta-pytorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library for using the MIMeta dataset
 Project-URL: Homepage, https://github.com/StefanoWoerner/mimeta-pytorch
 Project-URL: Issue Tracker, https://github.com/StefanoWoerner/mimeta-pytorch/issues
 Author-email: Stefano Woerner <stefano@woerner.eu>
 License-File: LICENSE
 License-File: LICENSE.LESSER
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.10
 Requires-Dist: h5py~=3.8.0
 Requires-Dist: numpy~=1.24.3
 Requires-Dist: pillow~=9.5.0
 Requires-Dist: pyyaml~=6.0
-Requires-Dist: torchcross~=0.0.3
+Requires-Dist: torchcross~=0.0.4
 Requires-Dist: torchvision~=0.15.1
 Requires-Dist: torch~=2.0.0
 Description-Content-Type: text/markdown
 
 # MIMeta for PyTorch
 
 ## Medical Imaging Meta Dataset
@@ -102,15 +102,15 @@
 for generating batches from multiple MIMeta tasks and for generating few-shot insttances
 of multiple MIMeta tasks.
 
 ### Examples
 
 See the [examples](examples) directory for examples on how to use MIMeta in conjunction
 with TorchCross.
-- [`imagenet_pretrained.py`](examples/imagenet_pretraining.py) shows how you can test
+- [`imagenet_pretrained.py`](examples/imagenet_pretrained.py) shows how you can test
   pre-trained models on a few-shot instance of a MIMeta task.
 - [`cross_domain_pretraining.py`](examples/cross_domain_pretraining.py) shows how you
   can perform cross-domain pre-training on different MIMeta tasks and then test the
   pre-trained model on a few-shot instance of a MIMeta task.
 - [`cross_domain_maml.py`](examples/cross_domain_maml.py) shows how you can perform
   cross-domain meta-learning with [MAML](https://arxiv.org/abs/1703.03400) on different
   MIMeta tasks and then test the meta-learned model on multiple few-shot instances of a
```

