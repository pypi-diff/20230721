# Comparing `tmp/eventdetector_ts-1.0.1.tar.gz` & `tmp/eventdetector_ts-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventdetector_ts-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "eventdetector_ts-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `eventdetector_ts-1.0.1.tar` & `eventdetector_ts-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1068 2023-07-20 12:55:07.352016 eventdetector_ts-1.0.1/LICENSE
--rw-r--r--   0        0        0     9226 2023-07-21 10:57:01.268133 eventdetector_ts-1.0.1/README.md
--rw-r--r--   0        0        0     6217 2023-07-20 17:52:46.056050 eventdetector_ts-1.0.1/eventdetector_ts/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 07:12:45.920022 eventdetector_ts-1.0.1/eventdetector_ts/data/__init__.py
--rw-r--r--   0        0        0    20770 2023-07-21 10:50:59.880128 eventdetector_ts-1.0.1/eventdetector_ts/data/helpers.py
--rw-r--r--   0        0        0     2168 2023-06-27 09:51:07.504172 eventdetector_ts-1.0.1/eventdetector_ts/data/interval.py
--rw-r--r--   0        0        0       64 2023-05-09 10:09:45.592180 eventdetector_ts-1.0.1/eventdetector_ts/metamodel/__init__.py
--rw-r--r--   0        0        0    21776 2023-07-21 10:50:59.964129 eventdetector_ts-1.0.1/eventdetector_ts/metamodel/meta_model.py
--rw-r--r--   0        0        0    12788 2023-07-21 10:50:59.944129 eventdetector_ts-1.0.1/eventdetector_ts/metamodel/utils.py
--rw-r--r--   0        0        0       60 2023-05-09 10:13:53.384183 eventdetector_ts-1.0.1/eventdetector_ts/models/__init__.py
--rw-r--r--   0        0        0     6836 2023-05-17 05:43:25.080012 eventdetector_ts-1.0.1/eventdetector_ts/models/helpers.py
--rw-r--r--   0        0        0    33455 2023-07-21 10:50:59.900128 eventdetector_ts-1.0.1/eventdetector_ts/models/models_builder.py
--rw-r--r--   0        0        0    12722 2023-07-21 10:51:06.600129 eventdetector_ts-1.0.1/eventdetector_ts/models/models_trainer.py
--rw-r--r--   0        0        0       53 2023-05-10 06:54:30.672029 eventdetector_ts-1.0.1/eventdetector_ts/optimization/__init__.py
--rw-r--r--   0        0        0      781 2023-05-15 09:49:54.420030 eventdetector_ts-1.0.1/eventdetector_ts/optimization/algorithms.py
--rw-r--r--   0        0        0    11507 2023-07-21 10:50:59.956128 eventdetector_ts-1.0.1/eventdetector_ts/optimization/event_extraction_pipeline.py
--rw-r--r--   0        0        0      180 2023-05-26 13:37:24.600319 eventdetector_ts-1.0.1/eventdetector_ts/plotter/__init__.py
--rw-r--r--   0        0        0     1358 2023-07-21 10:50:59.912129 eventdetector_ts-1.0.1/eventdetector_ts/plotter/helpers.py
--rw-r--r--   0        0        0    11202 2023-07-21 10:50:59.896129 eventdetector_ts-1.0.1/eventdetector_ts/plotter/plotter.py
--rw-r--r--   0        0        0       53 2023-05-23 06:48:12.328047 eventdetector_ts-1.0.1/eventdetector_ts/prediction/__init__.py
--rw-r--r--   0        0        0     7874 2023-07-21 10:50:59.876129 eventdetector_ts-1.0.1/eventdetector_ts/prediction/prediction.py
--rw-r--r--   0        0        0     1011 2023-07-21 10:50:59.968129 eventdetector_ts-1.0.1/eventdetector_ts/prediction/utils.py
--rw-r--r--   0        0        0     1472 2023-07-21 11:05:13.344139 eventdetector_ts-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    10615 1970-01-01 00:00:00.000000 eventdetector_ts-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-20 12:55:07.352016 eventdetector_ts-1.0.2/LICENSE
+-rw-r--r--   0        0        0     9360 2023-07-21 11:19:33.336150 eventdetector_ts-1.0.2/README.md
+-rw-r--r--   0        0        0     6217 2023-07-20 17:52:46.056050 eventdetector_ts-1.0.2/eventdetector_ts/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 07:12:45.920022 eventdetector_ts-1.0.2/eventdetector_ts/data/__init__.py
+-rw-r--r--   0        0        0    20770 2023-07-21 10:50:59.880128 eventdetector_ts-1.0.2/eventdetector_ts/data/helpers.py
+-rw-r--r--   0        0        0     2168 2023-06-27 09:51:07.504172 eventdetector_ts-1.0.2/eventdetector_ts/data/interval.py
+-rw-r--r--   0        0        0       64 2023-05-09 10:09:45.592180 eventdetector_ts-1.0.2/eventdetector_ts/metamodel/__init__.py
+-rw-r--r--   0        0        0    21776 2023-07-21 10:50:59.964129 eventdetector_ts-1.0.2/eventdetector_ts/metamodel/meta_model.py
+-rw-r--r--   0        0        0    12788 2023-07-21 10:50:59.944129 eventdetector_ts-1.0.2/eventdetector_ts/metamodel/utils.py
+-rw-r--r--   0        0        0       60 2023-05-09 10:13:53.384183 eventdetector_ts-1.0.2/eventdetector_ts/models/__init__.py
+-rw-r--r--   0        0        0     6836 2023-05-17 05:43:25.080012 eventdetector_ts-1.0.2/eventdetector_ts/models/helpers.py
+-rw-r--r--   0        0        0    33455 2023-07-21 10:50:59.900128 eventdetector_ts-1.0.2/eventdetector_ts/models/models_builder.py
+-rw-r--r--   0        0        0    12722 2023-07-21 10:51:06.600129 eventdetector_ts-1.0.2/eventdetector_ts/models/models_trainer.py
+-rw-r--r--   0        0        0       53 2023-05-10 06:54:30.672029 eventdetector_ts-1.0.2/eventdetector_ts/optimization/__init__.py
+-rw-r--r--   0        0        0      781 2023-05-15 09:49:54.420030 eventdetector_ts-1.0.2/eventdetector_ts/optimization/algorithms.py
+-rw-r--r--   0        0        0    11507 2023-07-21 10:50:59.956128 eventdetector_ts-1.0.2/eventdetector_ts/optimization/event_extraction_pipeline.py
+-rw-r--r--   0        0        0      180 2023-05-26 13:37:24.600319 eventdetector_ts-1.0.2/eventdetector_ts/plotter/__init__.py
+-rw-r--r--   0        0        0     1358 2023-07-21 10:50:59.912129 eventdetector_ts-1.0.2/eventdetector_ts/plotter/helpers.py
+-rw-r--r--   0        0        0    11202 2023-07-21 10:50:59.896129 eventdetector_ts-1.0.2/eventdetector_ts/plotter/plotter.py
+-rw-r--r--   0        0        0       53 2023-05-23 06:48:12.328047 eventdetector_ts-1.0.2/eventdetector_ts/prediction/__init__.py
+-rw-r--r--   0        0        0     7874 2023-07-21 10:50:59.876129 eventdetector_ts-1.0.2/eventdetector_ts/prediction/prediction.py
+-rw-r--r--   0        0        0     1011 2023-07-21 10:50:59.968129 eventdetector_ts-1.0.2/eventdetector_ts/prediction/utils.py
+-rw-r--r--   0        0        0     1472 2023-07-21 11:20:16.256150 eventdetector_ts-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    10749 1970-01-01 00:00:00.000000 eventdetector_ts-1.0.2/PKG-INFO
```

### Comparing `eventdetector_ts-1.0.1/LICENSE` & `eventdetector_ts-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.1/README.md` & `eventdetector_ts-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,20 +84,20 @@
 | Martian bow shock | 0.9021   | 0.9455    | 0.8626   |
 | Credit card fraud | 0.8372   | 0.9643    | 0.7397   |
 
 #### Training and Validation Losses
 
 The Figure below showcases the training loss and validation loss of the stacked models during the training process on the Martian bow shock and credit card fraud cases. The stacked models used in this evaluation consist of two feedforward neural networks (`FFN_0`, `FFN_1`) with distinct configurations of hyperparameters. The low losses observed in both cases indicate that the meta model has successfully learned the underlying patterns, justifying the obtained good metrics.
 
-![Training and validation losses](images/losses_mex_ccf.png)
+![Training and validation losses](https://raw.githubusercontent.com/menouarazib/eventdetector/master/images/losses_mex_ccf.png)
 
 #### Comparison of Predicted `op` and True `op`
 The Figure below illustrates the comparison between the predicted $op$ values and the true $op$ values on the Martian bow shock (`delta = 180` seconds) and credit card fraud (`delta = 3` seconds) datasets.
 
-![Comparison of predicted `op` and true `op`](images/op_mex_ccf.png)
+![Comparison of predicted `op` and true `op`](https://raw.githubusercontent.com/menouarazib/eventdetector/master/images/op_mex_ccf.png)
 
 ## MetaModel Arguments:
 
 Argument | Description
    ---------------------------- | --------------------------------------------------------------
    output_dir | The name or path of the directory where all outputs will be saved. If `output_dir` is a folder name, it will create the full path.
    dataset | The input dataset as `pd.DataFrame`.
```

### Comparing `eventdetector_ts-1.0.1/eventdetector_ts/__init__.py` & `eventdetector_ts-1.0.2/eventdetector_ts/__init__.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.1/eventdetector_ts/data/helpers.py` & `eventdetector_ts-1.0.2/eventdetector_ts/data/helpers.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.1/eventdetector_ts/data/interval.py` & `eventdetector_ts-1.0.2/eventdetector_ts/data/interval.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.1/eventdetector_ts/metamodel/meta_model.py` & `eventdetector_ts-1.0.2/eventdetector_ts/metamodel/meta_model.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.1/eventdetector_ts/metamodel/utils.py` & `eventdetector_ts-1.0.2/eventdetector_ts/metamodel/utils.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.1/eventdetector_ts/models/helpers.py` & `eventdetector_ts-1.0.2/eventdetector_ts/models/helpers.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.1/eventdetector_ts/models/models_builder.py` & `eventdetector_ts-1.0.2/eventdetector_ts/models/models_builder.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.1/eventdetector_ts/models/models_trainer.py` & `eventdetector_ts-1.0.2/eventdetector_ts/models/models_trainer.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.1/eventdetector_ts/optimization/algorithms.py` & `eventdetector_ts-1.0.2/eventdetector_ts/optimization/algorithms.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.1/eventdetector_ts/optimization/event_extraction_pipeline.py` & `eventdetector_ts-1.0.2/eventdetector_ts/optimization/event_extraction_pipeline.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.1/eventdetector_ts/plotter/helpers.py` & `eventdetector_ts-1.0.2/eventdetector_ts/plotter/helpers.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.1/eventdetector_ts/plotter/plotter.py` & `eventdetector_ts-1.0.2/eventdetector_ts/plotter/plotter.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.1/eventdetector_ts/prediction/prediction.py` & `eventdetector_ts-1.0.2/eventdetector_ts/prediction/prediction.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.1/eventdetector_ts/prediction/utils.py` & `eventdetector_ts-1.0.2/eventdetector_ts/prediction/utils.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.1/pyproject.toml` & `eventdetector_ts-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length = 120
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "eventdetector_ts"
-version = "1.0.1"
+version = "1.0.2"
 description = "This package provides an easy-to-use and efficient solution for event detection in time series data. It includes various functionalities and tools that enable users to apply our framework to their own data sets and customize the detection process according to their specific needs."
 keywords = ["Event Detection", "Time Series", "Universal Approximation Theory", "Deep Learning", "Stacking Ensemble Learning"]
 authors = [
     { name = "Menouar Azib", email = "menouar.azib@akkodis.com" }
 ]
 
 maintainers = [
```

### Comparing `eventdetector_ts-1.0.1/PKG-INFO` & `eventdetector_ts-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventdetector_ts
-Version: 1.0.1
+Version: 1.0.2
 Summary: This package provides an easy-to-use and efficient solution for event detection in time series data. It includes various functionalities and tools that enable users to apply our framework to their own data sets and customize the detection process according to their specific needs.
 Keywords: Event Detection,Time Series,Universal Approximation Theory,Deep Learning,Stacking Ensemble Learning
 Author-email: Menouar Azib <menouar.azib@akkodis.com>
 Maintainer-email: Menouar Azib <menouar.azib@akkodis.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
@@ -114,20 +114,20 @@
 | Martian bow shock | 0.9021   | 0.9455    | 0.8626   |
 | Credit card fraud | 0.8372   | 0.9643    | 0.7397   |
 
 #### Training and Validation Losses
 
 The Figure below showcases the training loss and validation loss of the stacked models during the training process on the Martian bow shock and credit card fraud cases. The stacked models used in this evaluation consist of two feedforward neural networks (`FFN_0`, `FFN_1`) with distinct configurations of hyperparameters. The low losses observed in both cases indicate that the meta model has successfully learned the underlying patterns, justifying the obtained good metrics.
 
-![Training and validation losses](images/losses_mex_ccf.png)
+![Training and validation losses](https://raw.githubusercontent.com/menouarazib/eventdetector/master/images/losses_mex_ccf.png)
 
 #### Comparison of Predicted `op` and True `op`
 The Figure below illustrates the comparison between the predicted $op$ values and the true $op$ values on the Martian bow shock (`delta = 180` seconds) and credit card fraud (`delta = 3` seconds) datasets.
 
-![Comparison of predicted `op` and true `op`](images/op_mex_ccf.png)
+![Comparison of predicted `op` and true `op`](https://raw.githubusercontent.com/menouarazib/eventdetector/master/images/op_mex_ccf.png)
 
 ## MetaModel Arguments:
 
 Argument | Description
    ---------------------------- | --------------------------------------------------------------
    output_dir | The name or path of the directory where all outputs will be saved. If `output_dir` is a folder name, it will create the full path.
    dataset | The input dataset as `pd.DataFrame`.
```

