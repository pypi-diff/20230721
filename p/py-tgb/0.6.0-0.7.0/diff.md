# Comparing `tmp/py_tgb-0.6.0.tar.gz` & `tmp/py_tgb-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_tgb-0.6.0.tar", max compression
+gzip compressed data, was "py_tgb-0.7.0.tar", max compression
```

## Comparing `py_tgb-0.6.0.tar` & `py_tgb-0.7.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     2404 2023-06-28 16:06:29.349452 py_tgb-0.6.0/README.md
--rw-r--r--   0        0        0      748 2023-06-28 16:06:29.349452 py_tgb-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      177 2023-06-28 16:06:29.349452 py_tgb-0.6.0/tgb/datasets/dataset_scripts/MAG/mag.py
--rw-r--r--   0        0        0      820 2023-06-28 16:06:29.349452 py_tgb-0.6.0/tgb/datasets/dataset_scripts/MAG/old/plot_stats.py
--rw-r--r--   0        0        0     4740 2023-06-28 16:06:29.349452 py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbl-coin.py
--rw-r--r--   0        0        0     2497 2023-06-28 16:06:29.349452 py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbl-coin_neg_generator.py
--rw-r--r--   0        0        0     6912 2023-06-28 16:06:29.349452 py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbl-comment.py
--rw-r--r--   0        0        0     2499 2023-06-28 16:06:29.349452 py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbl-comment_neg_generator.py
--rw-r--r--   0        0        0     7781 2023-06-28 16:06:29.349452 py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbl-flight.py
--rw-r--r--   0        0        0     2499 2023-06-28 16:06:29.349452 py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbl-flight_neg_generator.py
--rw-r--r--   0        0        0     4777 2023-06-28 16:06:29.349452 py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbl-review.py
--rw-r--r--   0        0        0     2498 2023-06-28 16:06:29.349452 py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbl-review_neg_generator.py
--rw-r--r--   0        0        0     2543 2023-06-28 16:06:29.349452 py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbl-wiki_neg_generator.py
--rw-r--r--   0        0        0    19780 2023-06-28 16:06:29.349452 py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbn-genre.py
--rw-r--r--   0        0        0    11859 2023-06-28 16:06:29.349452 py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbn-reddit.py
--rw-r--r--   0        0        0     5927 2023-06-28 16:06:29.349452 py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbn-trade.py
--rw-r--r--   0        0        0    13839 2023-06-28 16:06:29.353452 py_tgb-0.6.0/tgb/linkproppred/dataset.py
--rw-r--r--   0        0        0     7532 2023-06-28 16:06:29.353452 py_tgb-0.6.0/tgb/linkproppred/dataset_pyg.py
--rw-r--r--   0        0        0     5869 2023-06-28 16:06:29.353452 py_tgb-0.6.0/tgb/linkproppred/evaluate.py
--rw-r--r--   0        0        0    14146 2023-06-28 16:06:29.353452 py_tgb-0.6.0/tgb/linkproppred/negative_generator.py
--rw-r--r--   0        0        0     5123 2023-06-28 16:06:29.353452 py_tgb-0.6.0/tgb/linkproppred/negative_sampler.py
--rw-r--r--   0        0        0    16181 2023-06-28 16:06:29.353452 py_tgb-0.6.0/tgb/nodeproppred/dataset.py
--rw-r--r--   0        0        0     7205 2023-06-28 16:06:29.353452 py_tgb-0.6.0/tgb/nodeproppred/dataset_pyg.py
--rw-r--r--   0        0        0     5336 2023-06-28 16:06:29.353452 py_tgb-0.6.0/tgb/nodeproppred/evaluate.py
--rw-r--r--   0        0        0     8691 2023-06-28 16:06:29.353452 py_tgb-0.6.0/tgb/utils/dataset_stats.py
--rw-r--r--   0        0        0     1725 2023-06-28 16:06:29.353452 py_tgb-0.6.0/tgb/utils/info.py
--rw-r--r--   0        0        0    27787 2023-06-28 16:06:29.353452 py_tgb-0.6.0/tgb/utils/pre_process.py
--rw-r--r--   0        0        0     2747 2023-06-28 16:06:29.353452 py_tgb-0.6.0/tgb/utils/stats.py
--rw-r--r--   0        0        0     2974 2023-06-28 16:06:29.353452 py_tgb-0.6.0/tgb/utils/utils.py
--rw-r--r--   0        0        0     3088 1970-01-01 00:00:00.000000 py_tgb-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     4351 2023-07-21 15:22:18.659359 py_tgb-0.7.0/README.md
+-rw-r--r--   0        0        0      748 2023-07-21 15:22:18.663359 py_tgb-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/MAG/mag.py
+-rw-r--r--   0        0        0      820 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/MAG/old/plot_stats.py
+-rw-r--r--   0        0        0     4740 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-coin.py
+-rw-r--r--   0        0        0     2497 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-coin_neg_generator.py
+-rw-r--r--   0        0        0     6912 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-comment.py
+-rw-r--r--   0        0        0     2499 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-comment_neg_generator.py
+-rw-r--r--   0        0        0     7781 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-flight.py
+-rw-r--r--   0        0        0     2499 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-flight_neg_generator.py
+-rw-r--r--   0        0        0     4777 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-review.py
+-rw-r--r--   0        0        0     2503 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-review_neg_generator.py
+-rw-r--r--   0        0        0     2543 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-wiki_neg_generator.py
+-rw-r--r--   0        0        0    19780 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbn-genre.py
+-rw-r--r--   0        0        0    11859 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbn-reddit.py
+-rw-r--r--   0        0        0     5927 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbn-trade.py
+-rw-r--r--   0        0        0      539 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/tgbn-arxiv/process_arxiv.py
+-rw-r--r--   0        0        0    13895 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/linkproppred/dataset.py
+-rw-r--r--   0        0        0     7532 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/linkproppred/dataset_pyg.py
+-rw-r--r--   0        0        0     5869 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/linkproppred/evaluate.py
+-rw-r--r--   0        0        0    14146 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/linkproppred/negative_generator.py
+-rw-r--r--   0        0        0     5123 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/linkproppred/negative_sampler.py
+-rw-r--r--   0        0        0    16293 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/nodeproppred/dataset.py
+-rw-r--r--   0        0        0     7205 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/nodeproppred/dataset_pyg.py
+-rw-r--r--   0        0        0     5336 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/nodeproppred/evaluate.py
+-rw-r--r--   0        0        0     8691 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/utils/dataset_stats.py
+-rw-r--r--   0        0        0     1827 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/utils/info.py
+-rw-r--r--   0        0        0    27787 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/utils/pre_process.py
+-rw-r--r--   0        0        0     2747 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/utils/stats.py
+-rw-r--r--   0        0        0     2974 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/utils/utils.py
+-rw-r--r--   0        0        0     5035 1970-01-01 00:00:00.000000 py_tgb-0.7.0/PKG-INFO
```

### Comparing `py_tgb-0.6.0/pyproject.toml` & `py_tgb-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-tgb"
-version = "0.6.0"
+version = "0.7.0"
 description = "Temporal Graph Benchmark project repo"
 authors = ["shenyang Huang <shenyang.huang@mail.mcgill.ca>", "Farimah Poursafaei", "Emanuele Rossi <emanuele.rossi1909@gmail.com>", "Jacob Danovitch <jacob.danovitch@mila.quebec>"]
 readme = "README.md"
 packages = [{include = "tgb"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `py_tgb-0.6.0/tgb/datasets/dataset_scripts/MAG/old/plot_stats.py` & `py_tgb-0.7.0/tgb/datasets/dataset_scripts/MAG/old/plot_stats.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbl-coin.py` & `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-coin.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbl-coin_neg_generator.py` & `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-coin_neg_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbl-comment.py` & `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-comment.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbl-comment_neg_generator.py` & `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-comment_neg_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbl-flight.py` & `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-flight.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbl-flight_neg_generator.py` & `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-flight_neg_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbl-review.py` & `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-review.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbl-review_neg_generator.py` & `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-review_neg_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def main():
     r"""
     Generate negative edges for the validation or test phase
     """
     print("*** Negative Sample Generation ***")
 
     # setting the required parameters
-    num_neg_e_per_pos = 20 #100
+    num_neg_e_per_pos = 100 #20 #100
     neg_sample_strategy = "hist_rnd" #"rnd"
     rnd_seed = 42
 
 
     name = "tgbl-review"
     dataset = PyGLinkPropPredDataset(name=name, root="datasets")
     train_mask = dataset.train_mask
```

### Comparing `py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbl-wiki_neg_generator.py` & `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-wiki_neg_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbn-genre.py` & `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbn-genre.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbn-reddit.py` & `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbn-reddit.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/datasets/dataset_scripts/tgbn-trade.py` & `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbn-trade.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/linkproppred/dataset.py` & `py_tgb-0.7.0/tgb/linkproppred/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,17 +203,18 @@
         sources = np.array(df["u"])
         destinations = np.array(df["i"])
         timestamps = np.array(df["ts"])
         edge_idxs = np.array(df["idx"])
         weights = np.array(df["w"])
 
         edge_label = np.ones(len(df))  # should be 1 for all pos edges
-        self._edge_feat = edge_feat + weights.reshape(
-            -1, 1
-        )  # reshape weights as feature if available
+        # self._edge_feat = edge_feat + weights.reshape(
+        #     -1, 1
+        # )  # reshape weights as feature if available #! to remove
+        self._edge_feat = edge_feat
         self._node_feat = node_feat
 
         full_data = {
             "sources": sources,
             "destinations": destinations,
             "timestamps": timestamps,
             "edge_idxs": edge_idxs,
```

### Comparing `py_tgb-0.6.0/tgb/linkproppred/dataset_pyg.py` & `py_tgb-0.7.0/tgb/linkproppred/dataset_pyg.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/linkproppred/evaluate.py` & `py_tgb-0.7.0/tgb/linkproppred/evaluate.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/linkproppred/negative_generator.py` & `py_tgb-0.7.0/tgb/linkproppred/negative_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/linkproppred/negative_sampler.py` & `py_tgb-0.7.0/tgb/linkproppred/negative_sampler.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/nodeproppred/dataset.py` & `py_tgb-0.7.0/tgb/nodeproppred/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,15 +298,15 @@
         Parameters:
             cur_t: current timestamp of the batch of edges
         Returns:
             ts: timestamp of the node labels
             source_idx: node ids
             labels: the stacked label vectors
         """
-        if self.label_ts_idx >= (self.label_ts.shape[0] - 1):
+        if self.label_ts_idx >= (self.label_ts.shape[0]):
             # for query that are after the last batch of labels
             return None
         else:
             ts = self.label_ts[self.label_ts_idx]
 
         if cur_t >= ts:
             self.label_ts_idx += 1  # move to the next ts
@@ -332,15 +332,18 @@
 
     def return_label_ts(self) -> int:
         """
         return the current label timestamp that the pointer is at
         Returns:
             ts: int, the timestamp of the node labels
         """
-        return self.label_ts[self.label_ts_idx]
+        if (self.label_ts_idx >= self.label_ts.shape[0]):
+            return self.label_ts[-1]
+        else:
+            return self.label_ts[self.label_ts_idx]
 
     @property
     def num_classes(self) -> int:
         """
         number of classes in the node label
         Returns:
             num_classes: int, number of classes
```

### Comparing `py_tgb-0.6.0/tgb/nodeproppred/dataset_pyg.py` & `py_tgb-0.7.0/tgb/nodeproppred/dataset_pyg.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/nodeproppred/evaluate.py` & `py_tgb-0.7.0/tgb/nodeproppred/evaluate.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/utils/dataset_stats.py` & `py_tgb-0.7.0/tgb/utils/dataset_stats.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/utils/info.py` & `py_tgb-0.7.0/tgb/utils/info.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     "tgbl-flight": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbl-flight.zip",
     "tgbl-comment": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbl-comment.zip",
     "tgbn-trade": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbn-trade.zip",
     "tgbn-genre": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbn-genre.zip",
     "tgbn-reddit": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbn-reddit.zip",
 }
 
-#"https://object-arbutus.cloud.computecanada.ca/tgb/wiki_neg.zip" for all negative samples of the wiki dataset
+#"https://object-arbutus.cloud.computecanada.ca/tgb/wiki_neg.zip" #for all negative samples of the wiki dataset
+#"https://object-arbutus.cloud.computecanada.ca/tgb/review_ns100.zip" #for 100 ns samples in review
 
 DATA_EVAL_METRIC_DICT = {
     "tgbl-wiki": "mrr",
     "tgbl-review": "mrr",
     "tgbl-coin": "mrr",
     "tgbl-comment": "mrr",
     "tgbl-flight": "mrr",
```

### Comparing `py_tgb-0.6.0/tgb/utils/pre_process.py` & `py_tgb-0.7.0/tgb/utils/pre_process.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/utils/stats.py` & `py_tgb-0.7.0/tgb/utils/stats.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.6.0/tgb/utils/utils.py` & `py_tgb-0.7.0/tgb/utils/utils.py`

 * *Files identical despite different names*

