# Comparing `tmp/mmlab-lightning-1.0.7.tar.gz` & `tmp/mmlab-lightning-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmlab-lightning-1.0.7.tar", last modified: Wed May 31 04:05:36 2023, max compression
+gzip compressed data, was "mmlab-lightning-1.1.0.tar", last modified: Fri Jul 21 09:08:48 2023, max compression
```

## Comparing `mmlab-lightning-1.0.7.tar` & `mmlab-lightning-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:05:36.958094 mmlab-lightning-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-31 04:05:36.958094 mmlab-lightning-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:05:36.958094 mmlab-lightning-1.0.7/mmlab_lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/mmlab_lightning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:05:36.958094 mmlab-lightning-1.0.7/mmlab_lightning/datasets/
--rwxr-xr-x   0 runner    (1001) docker     (123)       78 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/mmlab_lightning/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/mmlab_lightning/datasets/mmlab_dataset_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:05:36.958094 mmlab-lightning-1.0.7/mmlab_lightning/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/mmlab_lightning/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/mmlab_lightning/models/mmlab_model_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:05:36.958094 mmlab-lightning-1.0.7/mmlab_lightning/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/mmlab_lightning/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:05:36.958094 mmlab-lightning-1.0.7/mmlab_lightning/tools/config/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/mmlab_lightning/tools/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/mmlab_lightning/tools/config/get_mmconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:05:36.958094 mmlab-lightning-1.0.7/mmlab_lightning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-31 04:05:36.000000 mmlab-lightning-1.0.7/mmlab_lightning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-31 04:05:36.000000 mmlab-lightning-1.0.7/mmlab_lightning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:05:36.000000 mmlab-lightning-1.0.7/mmlab_lightning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-31 04:05:36.000000 mmlab-lightning-1.0.7/mmlab_lightning.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-31 04:05:36.000000 mmlab-lightning-1.0.7/mmlab_lightning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 04:05:36.000000 mmlab-lightning-1.0.7/mmlab_lightning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 04:05:36.958094 mmlab-lightning-1.0.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1647 2023-05-31 04:05:08.000000 mmlab-lightning-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:08:48.472156 mmlab-lightning-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-21 09:08:35.000000 mmlab-lightning-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-21 09:08:48.472156 mmlab-lightning-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-21 09:08:35.000000 mmlab-lightning-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:08:48.472156 mmlab-lightning-1.1.0/mmlab_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-21 09:08:35.000000 mmlab-lightning-1.1.0/mmlab_lightning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:08:48.472156 mmlab-lightning-1.1.0/mmlab_lightning/datasets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       78 2023-07-21 09:08:35.000000 mmlab-lightning-1.1.0/mmlab_lightning/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-21 09:08:35.000000 mmlab-lightning-1.1.0/mmlab_lightning/datasets/mmlab_dataset_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:08:48.472156 mmlab-lightning-1.1.0/mmlab_lightning/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-07-21 09:08:35.000000 mmlab-lightning-1.1.0/mmlab_lightning/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-21 09:08:35.000000 mmlab-lightning-1.1.0/mmlab_lightning/models/mmlab_model_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:08:48.472156 mmlab-lightning-1.1.0/mmlab_lightning/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-21 09:08:35.000000 mmlab-lightning-1.1.0/mmlab_lightning/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:08:48.472156 mmlab-lightning-1.1.0/mmlab_lightning/tools/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 09:08:35.000000 mmlab-lightning-1.1.0/mmlab_lightning/tools/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-21 09:08:35.000000 mmlab-lightning-1.1.0/mmlab_lightning/tools/config/get_mmconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:08:48.472156 mmlab-lightning-1.1.0/mmlab_lightning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-21 09:08:48.000000 mmlab-lightning-1.1.0/mmlab_lightning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-21 09:08:48.000000 mmlab-lightning-1.1.0/mmlab_lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:08:48.000000 mmlab-lightning-1.1.0/mmlab_lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-21 09:08:48.000000 mmlab-lightning-1.1.0/mmlab_lightning.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 09:08:48.000000 mmlab-lightning-1.1.0/mmlab_lightning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 09:08:48.000000 mmlab-lightning-1.1.0/mmlab_lightning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 09:08:48.472156 mmlab-lightning-1.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1647 2023-07-21 09:08:35.000000 mmlab-lightning-1.1.0/setup.py
```

### Comparing `mmlab-lightning-1.0.7/LICENSE` & `mmlab-lightning-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mmlab-lightning-1.0.7/PKG-INFO` & `mmlab-lightning-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmlab-lightning
-Version: 1.0.7
+Version: 1.1.0
 Summary: A wrapper for mmlab repos to use in project_template.
 Home-page: https://github.com/shenmishajing/mmlab_lightning
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/mmlab_lightning
 Project-URL: Issue tracker, https://github.com/shenmishajing/mmlab_lightning/issues
```

### Comparing `mmlab-lightning-1.0.7/README.md` & `mmlab-lightning-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mmlab-lightning-1.0.7/mmlab_lightning/datasets/mmlab_dataset_adapter.py` & `mmlab-lightning-1.1.0/mmlab_lightning/datasets/mmlab_dataset_adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 from functools import partial
 
 from lightning.pytorch.cli import instantiate_class
-from mmengine.dataset import COLLATE_FUNCTIONS
-
 from lightning_template.datasets import LightningDataModule
+from mmengine.dataset import COLLATE_FUNCTIONS
 
 
 class MMLabDataSetAdapter(LightningDataModule):
-    def __init__(self, evaluator_cfg: dict, visualizer_cfg: dict, *args, **kwargs):
+    def __init__(self, visualizer_cfg: dict, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.evaluator_cfg = self.get_split_config(evaluator_cfg)
         self.visualizer_cfg = self.get_split_config(visualizer_cfg)
 
-        self.evaluators = {}
         self.visualizers = {}
 
     def setup(self, stage=None):
         super().setup(stage)
 
         for name in self.split_names:
-            self.evaluators[name] = instantiate_class((), self.evaluator_cfg[name])
             self.visualizers[name] = instantiate_class((), self.visualizer_cfg[name])
 
             if hasattr(self.datasets[name], "metainfo"):
                 self.evaluators[name].dataset_meta = self.datasets[name].metainfo
                 self.visualizers[name].dataset_meta = self.datasets[name].metainfo
 
     def _build_collate_fn(self, collate_fn_cfg):
```

### Comparing `mmlab-lightning-1.0.7/mmlab_lightning/models/mmlab_model_adapter.py` & `mmlab-lightning-1.1.0/mmlab_lightning/models/mmlab_model_adapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,48 +37,51 @@
 
     def on_test_start(self):
         self.set_data_preprocessor_device()
 
     def on_predict_start(self):
         self.set_data_preprocessor_device()
 
-    def forward(self, batch, mode="loss"):
+    def forward(self, batch, *args, mode="loss", **kwargs):
         self.batch_size = len(batch["inputs"])
         batch = self.model.data_preprocessor(batch, mode != "predict")
         return self.model._run_forward(batch, mode=mode)
 
+    def _loss_step(self, batch, output, *args, **kwargs):
+        _, log_dict = self.model.parse_losses(output)
+        return log_dict
+
+    def metric_step(self, batch, output, *args, split="val", **kwargs):
+        if self.evaluators[split]:
+            self.evaluators[split].process(output, batch)
+
+    def on_metric_epoch_end(self, *args, split="val", **kwargs):
+        return self.evaluators[split].evaluate(len(self.datasets[split]))
+
     def forward_step(self, batch, *args, split="val", **kwargs):
-        outputs = self(batch, mode="predict")
-        self.trainer.datamodule.evaluators[split].process(outputs, batch)
-        return outputs
-
-    def on_forward_epoch_end(self, *args, split="val", **kwargs):
-        log_vars = self.trainer.datamodule.evaluators[split].evaluate(
-            len(self.trainer.datamodule.datasets[split])
+        return super().forward_step(
+            batch,
+            *args,
+            split=split,
+            mode="loss" if split == "train" else "predict",
+            **kwargs
         )
-        self.log_dict(self.flatten_dict(log_vars, split), sync_dist=True)
-        return log_vars
 
     def on_train_epoch_start(self) -> None:
         message_hub = MessageHub.get_current_instance()
         message_hub.update_info(
             "epoch", self.trainer.fit_loop.epoch_progress.current.completed
         )
         return super().on_train_epoch_start()
 
     def on_train_batch_start(self, batch: Any, batch_idx: int) -> int | None:
         message_hub = MessageHub.get_current_instance()
         message_hub.update_info("iter", self.trainer.global_step)
         return super().on_train_batch_start(batch, batch_idx)
 
-    def training_step(self, batch, *args, **kwargs):
-        _, log_vars = self.model.parse_losses(self(batch))
-        self.log_dict(self.flatten_dict(log_vars))
-        return log_vars
-
     def predict_forward(self, batch, *args, **kwargs):
         predict_result = {"predict_outputs": self(batch, mode="predict")}
 
         batch = self.model.data_preprocessor(batch)
         if isinstance(batch, (list, tuple)):
             batch = {"inputs": batch[0], "data_samples": batch[1]}
         predict_result.update(batch)
```

### Comparing `mmlab-lightning-1.0.7/mmlab_lightning.egg-info/PKG-INFO` & `mmlab-lightning-1.1.0/mmlab_lightning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmlab-lightning
-Version: 1.0.7
+Version: 1.1.0
 Summary: A wrapper for mmlab repos to use in project_template.
 Home-page: https://github.com/shenmishajing/mmlab_lightning
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/mmlab_lightning
 Project-URL: Issue tracker, https://github.com/shenmishajing/mmlab_lightning/issues
```

### Comparing `mmlab-lightning-1.0.7/mmlab_lightning.egg-info/SOURCES.txt` & `mmlab-lightning-1.1.0/mmlab_lightning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmlab-lightning-1.0.7/setup.py` & `mmlab-lightning-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="mmlab-lightning",
-    version="1.0.7",
+    version="1.1.0",
     description="A wrapper for mmlab repos to use in project_template.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="shenmishajing",
     author_email="shenmishajing@gmail.com",
     url="https://github.com/shenmishajing/mmlab_lightning",
     project_urls={
```

