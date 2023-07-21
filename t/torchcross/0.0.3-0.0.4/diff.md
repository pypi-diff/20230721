# Comparing `tmp/torchcross-0.0.3.tar.gz` & `tmp/torchcross-0.0.4.tar.gz`

## Comparing `torchcross-0.0.3.tar` & `torchcross-0.0.4.tar`

### file list

```diff
@@ -1,52 +1,43 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 torchcross-0.0.3/requirements.txt
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/test_task_source.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/.pytest_cache/README.md
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/meta_dataset/test_base.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/meta_dataset/test_collection.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/meta_dataset/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/meta_dataset/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/meta_dataset/.pytest_cache/README.md
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/meta_dataset/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/meta_dataset/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/meta_dataset/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/cd/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/cd/activations.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/cd/losses.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/cd/heads/__init__.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/cd/heads/classification.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/cd/metrics/__init__.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/cd/metrics/classification.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/data/__init__.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/data/task.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/data/task_source.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/data/metadataset/__init__.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/data/metadataset/base.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/data/metadataset/collection.py
--rw-r--r--   0        0        0    16946 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/data/metadataset/few_shot.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/data/metadataset/few_shot_dummies.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/__init__.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/cross_domain.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/episodic.py
--rw-r--r--   0        0        0     9720 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/maml.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/protonet.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/lightning/__init__.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/lightning/cross_domain.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/lightning/cross_domain_classifier.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/lightning/episodic.py
--rw-r--r--   0        0        0     6927 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/lightning/maml.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/lightning/mixins.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/utils/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/utils/collate_fn.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/utils/layers.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 torchcross-0.0.3/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 torchcross-0.0.3/LICENSE
--rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 torchcross-0.0.3/LICENSE.LESSER
--rw-r--r--   0        0        0     7234 2020-02-02 00:00:00.000000 torchcross-0.0.3/README.md
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 torchcross-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 torchcross-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 torchcross-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 torchcross-0.0.4/tests/data/test_task_source.py
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 torchcross-0.0.4/tests/data/meta_dataset/test_base.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 torchcross-0.0.4/tests/data/meta_dataset/test_collection.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/cd/__init__.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/cd/activations.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/cd/losses.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/cd/heads/__init__.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/cd/heads/classification.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/cd/metrics/__init__.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/cd/metrics/classification.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/data/__init__.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/data/dataset.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/data/task.py
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/data/task_source.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/data/metadataset/__init__.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/data/metadataset/base.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/data/metadataset/collection.py
+-rw-r--r--   0        0        0    16946 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/data/metadataset/few_shot.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/data/metadataset/few_shot_dummies.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/models/__init__.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/models/cross_domain.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/models/episodic.py
+-rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/models/maml.py
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/models/protonet.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/models/lightning/__init__.py
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/models/lightning/cross_domain.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/models/lightning/cross_domain_classifier.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/models/lightning/episodic.py
+-rw-r--r--   0        0        0     6927 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/models/lightning/maml.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/models/lightning/mixins.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/models/lightning/protonet.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/utils/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/utils/collate_fn.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/utils/layers.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 torchcross-0.0.4/torchcross/utils/loops.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 torchcross-0.0.4/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 torchcross-0.0.4/LICENSE
+-rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 torchcross-0.0.4/LICENSE.LESSER
+-rw-r--r--   0        0        0     7234 2020-02-02 00:00:00.000000 torchcross-0.0.4/README.md
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 torchcross-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 torchcross-0.0.4/PKG-INFO
```

### Comparing `torchcross-0.0.3/tests/data/test_task_source.py` & `torchcross-0.0.4/tests/data/test_task_source.py`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/tests/data/meta_dataset/test_base.py` & `torchcross-0.0.4/tests/data/meta_dataset/test_base.py`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/tests/data/meta_dataset/test_collection.py` & `torchcross-0.0.4/tests/data/meta_dataset/test_collection.py`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/torchcross/cd/activations.py` & `torchcross-0.0.4/torchcross/cd/activations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from functools import partial
 from typing import Callable
 
 import torch
+from torch.nn import functional as F
 
 from torchcross.data.task import TaskTarget
 
-__all__ = ["get_prob_func"]
+__all__ = ["get_prob_func", "get_log_prob_func"]
 
 def get_prob_func(
     task_target: TaskTarget,
 ) -> Callable[[torch.Tensor], torch.Tensor]:
     """Get the probability function for a given task target.
 
     Args:
@@ -25,7 +26,30 @@
             return torch.sigmoid
         case TaskTarget.ORDINAL_REGRESSION:
             return partial(torch.softmax, dim=-1)
         case TaskTarget.REGRESSION:
             return lambda x: x
         case target:
             raise NotImplementedError(f"Task target {target} not yet implemented")
+
+def get_log_prob_func(
+    task_target: TaskTarget,
+) -> Callable[[torch.Tensor], torch.Tensor]:
+    """Get the log probability function for a given task target.
+
+    Args:
+        task_target: The task target.
+
+    Returns:
+        A function to convert logits to log probabilities.
+    """
+    match task_target:
+        case TaskTarget.MULTICLASS_CLASSIFICATION:
+            return partial(torch.log_softmax, dim=-1)
+        case TaskTarget.MULTILABEL_CLASSIFICATION | TaskTarget.BINARY_CLASSIFICATION:
+            return F.logsigmoid
+        case TaskTarget.ORDINAL_REGRESSION:
+            return partial(torch.log_softmax, dim=-1)
+        case TaskTarget.REGRESSION:
+            return lambda x: x
+        case target:
+            raise NotImplementedError(f"Task target {target} not yet implemented")
```

### Comparing `torchcross-0.0.3/torchcross/cd/losses.py` & `torchcross-0.0.4/torchcross/cd/losses.py`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/torchcross/cd/heads/classification.py` & `torchcross-0.0.4/torchcross/cd/heads/classification.py`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/torchcross/cd/metrics/classification.py` & `torchcross-0.0.4/torchcross/cd/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/torchcross/data/task.py` & `torchcross-0.0.4/torchcross/data/task.py`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/torchcross/data/task_source.py` & `torchcross-0.0.4/torchcross/data/task_source.py`

 * *Files 17% similar despite different names*

```diff
@@ -104,41 +104,14 @@
             else:
                 yield self.collate_fn([self.task_source[i] for i in batch])
 
     def __len__(self):
         return len(self.batch_sampler)
 
 
-class RandomChainTaskSource(TaskSource, IterableDataset):
-    def __init__(self, task_sources: list[BatchedTaskSource]):
-        self.task_sources = task_sources
-
-    def __iter__(self):
-        iterators = [iter(ts) for ts in self.task_sources]
-        # Calculate the weights of each iterator based on the batched task source length
-        weights = [len(ts) for ts in self.task_sources]
-        task_descriptions = [
-            TaskDescription(ts.task_target, ts.classes, ts.task_identifier)
-            for ts in self.task_sources
-        ]
-        while iterators:
-            # Randomly select an iterator with a probability proportional to its weight
-            i = random.choices(range(len(self.task_sources)), weights=weights)[0]
-            selected_iterator = iterators[i]
-            try:
-                # Return one element from the selected iterator
-                yield next(selected_iterator), task_descriptions[i]
-            except StopIteration:
-                # The iterator is exhausted, so remove it from the list of iterators
-                iterators.remove(selected_iterator)
-
-    def __len__(self):
-        return sum(len(ts) for ts in self.task_sources)
-
-
 class ConcatTaskSource(TaskSource, ConcatDataset):
     datasets: list[TaskSource]
 
     def __getitem__(self, idx):
         if idx < 0:
             if -idx > len(self):
                 raise ValueError(
```

### Comparing `torchcross-0.0.3/torchcross/data/metadataset/__init__.py` & `torchcross-0.0.4/torchcross/data/metadataset/__init__.py`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/torchcross/data/metadataset/base.py` & `torchcross-0.0.4/torchcross/data/metadataset/base.py`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/torchcross/data/metadataset/collection.py` & `torchcross-0.0.4/torchcross/data/metadataset/collection.py`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/torchcross/data/metadataset/few_shot.py` & `torchcross-0.0.4/torchcross/data/metadataset/few_shot.py`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/torchcross/data/metadataset/few_shot_dummies.py` & `torchcross-0.0.4/torchcross/data/metadataset/few_shot_dummies.py`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/torchcross/models/cross_domain.py` & `torchcross-0.0.4/torchcross/models/cross_domain.py`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/torchcross/models/maml.py` & `torchcross-0.0.4/torchcross/models/maml.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,58 +9,28 @@
 
 from torchcross.cd.heads import new_classification_head
 from torchcross.cd.losses import get_loss_func
 from torchcross.data.task import TaskDescription, Task
 from torchcross.models.cross_domain import CrossDomainModel
 from torchcross.models.episodic import EpisodicModel
 from torchcross.utils.layers import Expand
+from torchcross.utils.loops import inner_loop, differentiable_inner_loop
 
 head_init_t = Literal[
     "default",
     "kaiming",
     "zero",
     "adaptive",
     "adaptive normal",
     "adaptive uniform",
     "unicorn",
     "proto",
 ]
 
 
-def inner_loop(
-    net: nn.Module,
-    optim: torchopt.Optimizer,
-    num_steps: int,
-    support_x: torch.Tensor,
-    support_y: torch.Tensor,
-    loss_func: Callable[[torch.Tensor, torch.Tensor], torch.Tensor],
-) -> None:
-    for _ in range(num_steps):
-        support_logit = net(support_x)
-        loss = loss_func(support_logit, support_y)
-        optim.zero_grad()  # zero gradients
-        loss.backward()  # backward
-        optim.step()  # step updates
-    optim.zero_grad()  # zero gradients
-
-
-def differentiable_inner_loop(
-    net: nn.Module,
-    optim: torchopt.MetaOptimizer,
-    num_steps: int,
-    support_x: torch.Tensor,
-    support_y: torch.Tensor,
-    loss_func: Callable[[torch.Tensor, torch.Tensor], torch.Tensor],
-) -> None:
-    for _ in range(num_steps):
-        support_logit = net(support_x)
-        loss = loss_func(support_logit, support_y)
-        optim.step(loss)
-
-
 class MAML(EpisodicModel):
     def __init__(
         self,
         backbone: nn.Module,
         num_backbone_features: int,
         task_description: TaskDescription,
         inner_optimizer: Callable[[torch.nn.Module], torchopt.MetaOptimizer],
```

### Comparing `torchcross-0.0.3/torchcross/models/lightning/cross_domain.py` & `torchcross-0.0.4/torchcross/models/lightning/cross_domain.py`

 * *Files 13% similar despite different names*

```diff
@@ -51,15 +51,23 @@
         self.log_dict(self.training_metrics)
 
     def validation_step(
         self,
         batch: tuple[tuple[torch.Tensor, torch.Tensor], TaskDescription],
         batch_idx: int,
     ):
-        metric_values, loss = self.get_metrics_and_loss(batch)
+        try:
+            metric_values, loss = self.get_metrics_and_loss(batch)
+        except RuntimeError:
+            print(batch[1].task_identifier)
+            print(batch[1].task_target)
+            print(batch[1].classes)
+            print(batch[0][1].shape)
+            print(batch[0][1].cpu().numpy())
+            raise
 
         self.update_metrics("val", metric_values)
 
         self.log("loss/val", loss, batch_size=len(batch), prog_bar=True)
         self.log_dict(self.validation_metrics, prog_bar=True)
 
     def test_step(
```

### Comparing `torchcross-0.0.3/torchcross/models/lightning/cross_domain_classifier.py` & `torchcross-0.0.4/torchcross/models/lightning/cross_domain_classifier.py`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/torchcross/models/lightning/episodic.py` & `torchcross-0.0.4/torchcross/models/lightning/episodic.py`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/torchcross/models/lightning/maml.py` & `torchcross-0.0.4/torchcross/models/lightning/maml.py`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/torchcross/models/lightning/mixins.py` & `torchcross-0.0.4/torchcross/models/lightning/mixins.py`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/torchcross/utils/__init__.py` & `torchcross-0.0.4/torchcross/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/LICENSE` & `torchcross-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/LICENSE.LESSER` & `torchcross-0.0.4/LICENSE.LESSER`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/README.md` & `torchcross-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.3/pyproject.toml` & `torchcross-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "torchcross"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="Stefano Woerner", email="stefano@woerner.eu" },
 ]
 description = "Easy-to-use PyTorch library for cross-domain learning, few-shot learning and meta-learning"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `torchcross-0.0.3/PKG-INFO` & `torchcross-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchcross
-Version: 0.0.3
+Version: 0.0.4
 Summary: Easy-to-use PyTorch library for cross-domain learning, few-shot learning and meta-learning
 Project-URL: Homepage, https://github.com/StefanoWoerner/torchcross
 Project-URL: Issue Tracker, https://github.com/StefanoWoerner/torchcross/issues
 Author-email: Stefano Woerner <stefano@woerner.eu>
 License-File: LICENSE
 License-File: LICENSE.LESSER
 Classifier: Intended Audience :: Developers
```

