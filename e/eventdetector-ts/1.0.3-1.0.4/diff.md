# Comparing `tmp/eventdetector_ts-1.0.3.tar.gz` & `tmp/eventdetector_ts-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventdetector_ts-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "eventdetector_ts-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `eventdetector_ts-1.0.3.tar` & `eventdetector_ts-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1068 2023-07-20 12:55:07.352016 eventdetector_ts-1.0.3/LICENSE
--rw-r--r--   0        0        0     9448 2023-07-21 11:29:02.596156 eventdetector_ts-1.0.3/README.md
--rw-r--r--   0        0        0     6217 2023-07-20 17:52:46.056050 eventdetector_ts-1.0.3/eventdetector_ts/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 07:12:45.920022 eventdetector_ts-1.0.3/eventdetector_ts/data/__init__.py
--rw-r--r--   0        0        0    20770 2023-07-21 10:50:59.880128 eventdetector_ts-1.0.3/eventdetector_ts/data/helpers.py
--rw-r--r--   0        0        0     2168 2023-06-27 09:51:07.504172 eventdetector_ts-1.0.3/eventdetector_ts/data/interval.py
--rw-r--r--   0        0        0       64 2023-05-09 10:09:45.592180 eventdetector_ts-1.0.3/eventdetector_ts/metamodel/__init__.py
--rw-r--r--   0        0        0    21776 2023-07-21 10:50:59.964129 eventdetector_ts-1.0.3/eventdetector_ts/metamodel/meta_model.py
--rw-r--r--   0        0        0    12788 2023-07-21 10:50:59.944129 eventdetector_ts-1.0.3/eventdetector_ts/metamodel/utils.py
--rw-r--r--   0        0        0       60 2023-05-09 10:13:53.384183 eventdetector_ts-1.0.3/eventdetector_ts/models/__init__.py
--rw-r--r--   0        0        0     6836 2023-05-17 05:43:25.080012 eventdetector_ts-1.0.3/eventdetector_ts/models/helpers.py
--rw-r--r--   0        0        0    33455 2023-07-21 10:50:59.900128 eventdetector_ts-1.0.3/eventdetector_ts/models/models_builder.py
--rw-r--r--   0        0        0    12722 2023-07-21 10:51:06.600129 eventdetector_ts-1.0.3/eventdetector_ts/models/models_trainer.py
--rw-r--r--   0        0        0       53 2023-05-10 06:54:30.672029 eventdetector_ts-1.0.3/eventdetector_ts/optimization/__init__.py
--rw-r--r--   0        0        0      781 2023-05-15 09:49:54.420030 eventdetector_ts-1.0.3/eventdetector_ts/optimization/algorithms.py
--rw-r--r--   0        0        0    11507 2023-07-21 10:50:59.956128 eventdetector_ts-1.0.3/eventdetector_ts/optimization/event_extraction_pipeline.py
--rw-r--r--   0        0        0      180 2023-05-26 13:37:24.600319 eventdetector_ts-1.0.3/eventdetector_ts/plotter/__init__.py
--rw-r--r--   0        0        0     1358 2023-07-21 10:50:59.912129 eventdetector_ts-1.0.3/eventdetector_ts/plotter/helpers.py
--rw-r--r--   0        0        0    11202 2023-07-21 10:50:59.896129 eventdetector_ts-1.0.3/eventdetector_ts/plotter/plotter.py
--rw-r--r--   0        0        0       53 2023-05-23 06:48:12.328047 eventdetector_ts-1.0.3/eventdetector_ts/prediction/__init__.py
--rw-r--r--   0        0        0     7874 2023-07-21 10:50:59.876129 eventdetector_ts-1.0.3/eventdetector_ts/prediction/prediction.py
--rw-r--r--   0        0        0     1011 2023-07-21 10:50:59.968129 eventdetector_ts-1.0.3/eventdetector_ts/prediction/utils.py
--rw-r--r--   0        0        0     1472 2023-07-21 11:31:56.944159 eventdetector_ts-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    10837 1970-01-01 00:00:00.000000 eventdetector_ts-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-20 12:55:07.352016 eventdetector_ts-1.0.4/LICENSE
+-rw-r--r--   0        0        0     9461 2023-07-21 11:33:27.408160 eventdetector_ts-1.0.4/README.md
+-rw-r--r--   0        0        0     6217 2023-07-20 17:52:46.056050 eventdetector_ts-1.0.4/eventdetector_ts/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 07:12:45.920022 eventdetector_ts-1.0.4/eventdetector_ts/data/__init__.py
+-rw-r--r--   0        0        0    20804 2023-07-21 17:54:15.480210 eventdetector_ts-1.0.4/eventdetector_ts/data/helpers.py
+-rw-r--r--   0        0        0     2168 2023-07-21 16:36:06.500153 eventdetector_ts-1.0.4/eventdetector_ts/data/interval.py
+-rw-r--r--   0        0        0       64 2023-05-09 10:09:45.592180 eventdetector_ts-1.0.4/eventdetector_ts/metamodel/__init__.py
+-rw-r--r--   0        0        0    21779 2023-07-21 17:56:22.596212 eventdetector_ts-1.0.4/eventdetector_ts/metamodel/meta_model.py
+-rw-r--r--   0        0        0    12788 2023-07-21 11:37:16.692162 eventdetector_ts-1.0.4/eventdetector_ts/metamodel/utils.py
+-rw-r--r--   0        0        0       60 2023-05-09 10:13:53.384183 eventdetector_ts-1.0.4/eventdetector_ts/models/__init__.py
+-rw-r--r--   0        0        0     6836 2023-05-17 05:43:25.080012 eventdetector_ts-1.0.4/eventdetector_ts/models/helpers.py
+-rw-r--r--   0        0        0    33455 2023-07-21 10:50:59.900128 eventdetector_ts-1.0.4/eventdetector_ts/models/models_builder.py
+-rw-r--r--   0        0        0    12722 2023-07-21 10:51:06.600129 eventdetector_ts-1.0.4/eventdetector_ts/models/models_trainer.py
+-rw-r--r--   0        0        0       53 2023-05-10 06:54:30.672029 eventdetector_ts-1.0.4/eventdetector_ts/optimization/__init__.py
+-rw-r--r--   0        0        0      781 2023-05-15 09:49:54.420030 eventdetector_ts-1.0.4/eventdetector_ts/optimization/algorithms.py
+-rw-r--r--   0        0        0    11507 2023-07-21 16:36:06.500153 eventdetector_ts-1.0.4/eventdetector_ts/optimization/event_extraction_pipeline.py
+-rw-r--r--   0        0        0      180 2023-05-26 13:37:24.600319 eventdetector_ts-1.0.4/eventdetector_ts/plotter/__init__.py
+-rw-r--r--   0        0        0     1358 2023-07-21 10:50:59.912129 eventdetector_ts-1.0.4/eventdetector_ts/plotter/helpers.py
+-rw-r--r--   0        0        0    11202 2023-07-21 10:50:59.896129 eventdetector_ts-1.0.4/eventdetector_ts/plotter/plotter.py
+-rw-r--r--   0        0        0       53 2023-05-23 06:48:12.328047 eventdetector_ts-1.0.4/eventdetector_ts/prediction/__init__.py
+-rw-r--r--   0        0        0     7874 2023-07-21 10:50:59.876129 eventdetector_ts-1.0.4/eventdetector_ts/prediction/prediction.py
+-rw-r--r--   0        0        0     1011 2023-07-21 10:50:59.968129 eventdetector_ts-1.0.4/eventdetector_ts/prediction/utils.py
+-rw-r--r--   0        0        0     1472 2023-07-21 17:57:58.624213 eventdetector_ts-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    10850 1970-01-01 00:00:00.000000 eventdetector_ts-1.0.4/PKG-INFO
```

### Comparing `eventdetector_ts-1.0.3/LICENSE` & `eventdetector_ts-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.3/README.md` & `eventdetector_ts-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 Welcome to **Event Detector**, a Python package for detecting events in time series data. The emphasis of this package
 is on offering useful machine learning functionalities, such as customizing and fitting the model on multidimensional
 time series, training on large datasets, ensemble models, and providing rich support for event detection in time
 series.
 ## Installation
 ### Pypi installation
-<pre>
-pip install eventdetector-ts
+<pre><code>
+pip install eventdetector-ts</code>
 </pre>
 ### Manual installation
 To get started using **Event Detector**, simply follow the instructions below to install the required packages and
 dependencies.
 #### Clone the repository:
 
 <pre><code>git clone https://github.com/menouarazib/eventdetector.git
```

### Comparing `eventdetector_ts-1.0.3/eventdetector_ts/__init__.py` & `eventdetector_ts-1.0.4/eventdetector_ts/__init__.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.3/eventdetector_ts/data/helpers.py` & `eventdetector_ts-1.0.4/eventdetector_ts/data/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         dt = datetime.fromtimestamp(date)
     elif isinstance(date, str):
         dt = parser.parse(date, ignoretz=True)
     else:
         raise ValueError(f"Invalid date format {date}. Supported formats are str, pd.Timestamp, float, and int.")
 
     if to_timestamp:
-        return dt.timestamp()
+        return (dt - datetime(1970, 1, 1)).total_seconds()
     return dt
 
 
 def num_columns(lst: list) -> int:
     """
     Returns the number of columns in a list.
 
@@ -161,14 +161,15 @@
 
     if isinstance(events, list):
         nb_columns = num_columns(events)
         if nb_columns == 2:
             df = pd.DataFrame(events, columns=[column1, column2])
         elif nb_columns == 1:
             df = pd.DataFrame(events, columns=[column1])
+
             is2d = False
         else:
             raise ValueError(
                 f"The list of events is not compatible. The number of columns {nb_columns} should not exceed 2.")
     elif isinstance(events, pd.DataFrame):
         df = events
         columns = events.columns
@@ -189,15 +190,15 @@
     if is2d:
         df[column1] = df[column1].apply(lambda x: convert_time_to_datetime(x) / 2)
         df[column2] = df[column2].apply(lambda x: convert_time_to_datetime(x) / 2)
         df[MIDDLE_EVENT_LABEL] = df[column1] + df[column2]
     else:
         df[MIDDLE_EVENT_LABEL] = df[column1].apply(lambda x: convert_time_to_datetime(x))
 
-    df[MIDDLE_EVENT_LABEL] = df[MIDDLE_EVENT_LABEL].apply(lambda x: datetime.fromtimestamp(x))
+    df[MIDDLE_EVENT_LABEL] = df[MIDDLE_EVENT_LABEL].apply(lambda x: datetime.utcfromtimestamp(x))
     df = df[[MIDDLE_EVENT_LABEL]]
     df = df.sort_values(by=MIDDLE_EVENT_LABEL)
     return df
 
 
 def remove_close_events(events_df: pd.DataFrame, delta_unit_time: int, unit: TimeUnit) -> pd.DataFrame:
     """
@@ -274,16 +275,16 @@
 
     # Return the list of intervals
     return events_intervals
 
 
 def get_union_times_events(events_df: pd.DataFrame, partition_size: int, unit_time: TimeUnit) -> pd.DatetimeIndex:
     """
-    Given a DataFrame of events and a time partition size in unit time, computes a DatetimeIndex of all times during which
-    at least one event was taking place.
+    Given a DataFrame of events and a time partition size in unit time, computes a DatetimeIndex of all times during 
+    which at least one event was taking place.
 
     Args:
         events_df (pd.DataFrame): A DataFrame containing at least a MIDDLE_EVENT_LABEL column with the datetime
             of each event.
         partition_size (int): The size of the time partition to consider before and after each event.
         unit_time (TimeUnit): The unit time
```

### Comparing `eventdetector_ts-1.0.3/eventdetector_ts/data/interval.py` & `eventdetector_ts-1.0.4/eventdetector_ts/data/interval.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.3/eventdetector_ts/metamodel/meta_model.py` & `eventdetector_ts-1.0.4/eventdetector_ts/metamodel/meta_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,17 +283,19 @@
 
         Returns:
              None
         """
 
         logger_meta_model.info("Computes the middle date of events...")
         self.events = compute_middle_event(self.events)
+
         logger_meta_model.info("Removes events that occur too close together...")
         temp: int = len(self.events)
         self.events = remove_close_events(self.events, self.w_s, self.time_unit)
+
         logger_meta_model.warning(f"A total of {temp - len(self.events)}/{temp} events were removed due to overlapping")
         logger_meta_model.info("Convert events to intervals...")
         intervals = convert_events_to_intervals(self.events, self.w_s, self.time_unit)
 
         if self.time_window is not None:
             logger_meta_model.warning(f"time_window is provided = {self.time_window} {self.time_unit}s")
             events_times = get_union_times_events(self.events, self.time_window, self.time_unit)
@@ -302,14 +304,15 @@
         logger_meta_model.info("Computing overlapping partitions...")
         overlapping_partitions = convert_dataframe_to_overlapping_partitions(self.dataset, width=self.width,
                                                                              step=self.step,
                                                                              fill_method=self.fill_nan)
 
         logger_meta_model.info("Computing op...")
         self.x, self.y = op(dataset_as_overlapping_partitions=overlapping_partitions, events_as_intervals=intervals)
+
         # Convert x and y arrays to float32 for consistency
         self.x = np.asarray(self.x).astype('float32')
         self.y = np.asarray(self.y).astype('float32')
 
         self.optimization_data.set_overlapping_partitions(overlapping_partitions)
         self.optimization_data.set_true_events(self.events)
```

### Comparing `eventdetector_ts-1.0.3/eventdetector_ts/metamodel/utils.py` & `eventdetector_ts-1.0.4/eventdetector_ts/metamodel/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 import joblib
 import numpy as np
 import pandas as pd
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import StandardScaler, MinMaxScaler, RobustScaler
 
-from eventdetector_ts import MIN_MAX_SCALER, ROBUST_SCALER, SCALERS_DIR, FILL_NAN_ZEROS, FILL_NAN_FFILL, FILL_NAN_BFILL, \
-    FILL_NAN_MEDIAN, RNN_BIDIRECTIONAL, CONV_LSTM1D, RNN_ENCODER_DECODER, FFN, CNN_RNN, GRU, CNN, SELF_ATTENTION, \
-    LSTM, TYPE_TRAINING_AVERAGE, TYPE_TRAINING_FFN, STANDARD_SCALER
+from eventdetector_ts import MIN_MAX_SCALER, ROBUST_SCALER, SCALERS_DIR, FILL_NAN_ZEROS, FILL_NAN_FFILL, \
+    FILL_NAN_BFILL, FILL_NAN_MEDIAN, RNN_BIDIRECTIONAL, CONV_LSTM1D, RNN_ENCODER_DECODER, FFN, CNN_RNN, \
+    GRU, CNN, SELF_ATTENTION, LSTM, TYPE_TRAINING_AVERAGE, TYPE_TRAINING_FFN, STANDARD_SCALER
 from eventdetector_ts.data.helpers import InvalidArgumentError
 
 
 class DataSplitter:
     """
     A class for splitting and scaling data into training, test sets and applying scalers to each
     time step in the data.
```

### Comparing `eventdetector_ts-1.0.3/eventdetector_ts/models/helpers.py` & `eventdetector_ts-1.0.4/eventdetector_ts/models/helpers.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.3/eventdetector_ts/models/models_builder.py` & `eventdetector_ts-1.0.4/eventdetector_ts/models/models_builder.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.3/eventdetector_ts/models/models_trainer.py` & `eventdetector_ts-1.0.4/eventdetector_ts/models/models_trainer.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.3/eventdetector_ts/optimization/algorithms.py` & `eventdetector_ts-1.0.4/eventdetector_ts/optimization/algorithms.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.3/eventdetector_ts/optimization/event_extraction_pipeline.py` & `eventdetector_ts-1.0.4/eventdetector_ts/optimization/event_extraction_pipeline.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.3/eventdetector_ts/plotter/helpers.py` & `eventdetector_ts-1.0.4/eventdetector_ts/plotter/helpers.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.3/eventdetector_ts/plotter/plotter.py` & `eventdetector_ts-1.0.4/eventdetector_ts/plotter/plotter.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.3/eventdetector_ts/prediction/prediction.py` & `eventdetector_ts-1.0.4/eventdetector_ts/prediction/prediction.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.3/eventdetector_ts/prediction/utils.py` & `eventdetector_ts-1.0.4/eventdetector_ts/prediction/utils.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.3/pyproject.toml` & `eventdetector_ts-1.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length = 120
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "eventdetector_ts"
-version = "1.0.3"
+version = "1.0.4"
 description = "This package provides an easy-to-use and efficient solution for event detection in time series data. It includes various functionalities and tools that enable users to apply our framework to their own data sets and customize the detection process according to their specific needs."
 keywords = ["Event Detection", "Time Series", "Universal Approximation Theory", "Deep Learning", "Stacking Ensemble Learning"]
 authors = [
     { name = "Menouar Azib", email = "menouar.azib@akkodis.com" }
 ]
 
 maintainers = [
```

### Comparing `eventdetector_ts-1.0.3/PKG-INFO` & `eventdetector_ts-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventdetector_ts
-Version: 1.0.3
+Version: 1.0.4
 Summary: This package provides an easy-to-use and efficient solution for event detection in time series data. It includes various functionalities and tools that enable users to apply our framework to their own data sets and customize the detection process according to their specific needs.
 Keywords: Event Detection,Time Series,Universal Approximation Theory,Deep Learning,Stacking Ensemble Learning
 Author-email: Menouar Azib <menouar.azib@akkodis.com>
 Maintainer-email: Menouar Azib <menouar.azib@akkodis.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
@@ -33,16 +33,16 @@
 
 Welcome to **Event Detector**, a Python package for detecting events in time series data. The emphasis of this package
 is on offering useful machine learning functionalities, such as customizing and fitting the model on multidimensional
 time series, training on large datasets, ensemble models, and providing rich support for event detection in time
 series.
 ## Installation
 ### Pypi installation
-<pre>
-pip install eventdetector-ts
+<pre><code>
+pip install eventdetector-ts</code>
 </pre>
 ### Manual installation
 To get started using **Event Detector**, simply follow the instructions below to install the required packages and
 dependencies.
 #### Clone the repository:
 
 <pre><code>git clone https://github.com/menouarazib/eventdetector.git
```

