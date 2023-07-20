# Comparing `tmp/mindsdb_forecast_visualizer-22.8.4.0.tar.gz` & `tmp/mindsdb_forecast_visualizer-23.7.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mindsdb_forecast_visualizer-22.8.4.0.tar", last modified: Mon Aug 22 23:31:02 2022, max compression
+gzip compressed data, was "dist/mindsdb_forecast_visualizer-23.7.4.1.tar", last modified: Thu Jul 20 22:46:07 2023, max compression
```

## Comparing `mindsdb_forecast_visualizer-22.8.4.0.tar` & `mindsdb_forecast_visualizer-23.7.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 23:31:02.000000 mindsdb_forecast_visualizer-22.8.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1792 2022-08-22 23:31:02.000000 mindsdb_forecast_visualizer-22.8.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-08-22 23:30:50.000000 mindsdb_forecast_visualizer-22.8.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 23:31:02.000000 mindsdb_forecast_visualizer-22.8.4.0/example/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 23:30:50.000000 mindsdb_forecast_visualizer-22.8.4.0/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1622 2022-08-22 23:30:50.000000 mindsdb_forecast_visualizer-22.8.4.0/example/train.py
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-08-22 23:30:50.000000 mindsdb_forecast_visualizer-22.8.4.0/example/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 23:31:02.000000 mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer/
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-08-22 23:30:50.000000 mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 23:30:50.000000 mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 23:31:02.000000 mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer/config/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-08-22 23:30:50.000000 mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-08-22 23:30:50.000000 mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 23:31:02.000000 mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer/core/
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-22 23:30:50.000000 mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-08-22 23:30:50.000000 mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer/core/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     8529 2022-08-22 23:30:50.000000 mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer/core/forecaster.py
--rw-r--r--   0 runner    (1001) docker     (121)     4474 2022-08-22 23:30:50.000000 mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer/core/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 23:31:02.000000 mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1792 2022-08-22 23:31:02.000000 mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-08-22 23:31:02.000000 mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 23:31:02.000000 mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-08-22 23:31:02.000000 mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-08-22 23:31:02.000000 mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-22 23:30:50.000000 mindsdb_forecast_visualizer-22.8.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 23:31:02.000000 mindsdb_forecast_visualizer-22.8.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-08-22 23:30:50.000000 mindsdb_forecast_visualizer-22.8.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:46:07.000000 mindsdb_forecast_visualizer-23.7.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-20 22:46:07.000000 mindsdb_forecast_visualizer-23.7.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-20 22:45:54.000000 mindsdb_forecast_visualizer-23.7.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:46:07.000000 mindsdb_forecast_visualizer-23.7.4.1/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:45:54.000000 mindsdb_forecast_visualizer-23.7.4.1/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-20 22:45:54.000000 mindsdb_forecast_visualizer-23.7.4.1/example/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-20 22:45:54.000000 mindsdb_forecast_visualizer-23.7.4.1/example/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:46:07.000000 mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-20 22:45:54.000000 mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:45:54.000000 mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:46:07.000000 mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 22:45:54.000000 mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-20 22:45:54.000000 mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:46:07.000000 mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 22:45:54.000000 mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-20 22:45:54.000000 mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer/core/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-07-20 22:45:54.000000 mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer/core/forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-20 22:45:54.000000 mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer/core/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:46:07.000000 mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-20 22:46:06.000000 mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-20 22:46:07.000000 mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 22:46:06.000000 mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-20 22:46:06.000000 mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-20 22:46:06.000000 mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-20 22:45:54.000000 mindsdb_forecast_visualizer-23.7.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 22:46:07.000000 mindsdb_forecast_visualizer-23.7.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-20 22:45:54.000000 mindsdb_forecast_visualizer-23.7.4.1/setup.py
```

### Comparing `mindsdb_forecast_visualizer-22.8.4.0/PKG-INFO` & `mindsdb_forecast_visualizer-23.7.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindsdb_forecast_visualizer
-Version: 22.8.4.0
+Version: 23.7.4.1
 Summary: Companion package to visualizer forecasts made with MindsDB predictors.
 Home-page: https://github.com/mindsdb/mindsdb_forecast_visualizer
 Author: MindsDB Inc
 Author-email: community@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb_forecast_visualizer
 Description: # MindsDB Forecast Visualizer
```

### Comparing `mindsdb_forecast_visualizer-22.8.4.0/README.md` & `mindsdb_forecast_visualizer-23.7.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mindsdb_forecast_visualizer-22.8.4.0/example/train.py` & `mindsdb_forecast_visualizer-23.7.4.1/example/train.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 import pandas as pd
 
-from lightwood.data.splitter import stratify
+from dataprep_ml.splitters import stratify
 from lightwood.api.high_level import ProblemDefinition, predictor_from_code, json_ai_from_problem, code_from_json_ai
 
 
 if __name__ == '__main__':
     # Load data and define the task
     df = pd.read_csv('./arrivals.csv')
     gby = ['Country']
     train_df, _, _ = stratify(df, pct_train=0.8, pct_dev=0, pct_test=0.2, stratify_on=gby, seed=1, reshuffle=False)
 
     pdef = ProblemDefinition.from_dict({'target': 'Traffic',      # column to forecast
+                                        'fit_on_all': False,
                                         'timeseries_settings': {
                                             'window': 10,         # qty of previous data to use when predicting
                                             'horizon': 5,         # forecast horizon length
                                             'order_by': 'T',
                                             'group_by': gby,
                                         }})
 
     # name and generate predictor code
     p_name = 'arrival_forecast_example'
     json_ai = json_ai_from_problem(train_df, problem_definition=pdef)
 
-    # specify a quick mixer for this example
+    # specify a quick mixer configuration for this example
     json_ai.model['args']['submodels'] = [
         {
-            "module": "ETSMixer",
-            "args": {}
+            "module": "SkTime",
+            "args": {
+                'model_path': '"theta.ThetaForecaster"',
+            }
         }
     ]
 
     # generate and train predictor
     predictor_class_code = code_from_json_ai(json_ai)
     predictor = predictor_from_code(predictor_class_code)
     predictor.learn(train_df)
 
     # save predictor and its code
     predictor.save(f'./{p_name}.pkl')
     with open(f'./{p_name}.py', 'wb') as fp:
         fp.write(predictor_class_code.encode('utf-8'))
-
```

### Comparing `mindsdb_forecast_visualizer-22.8.4.0/example/visualize.py` & `mindsdb_forecast_visualizer-23.7.4.1/example/visualize.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This example shows how to use the visualizer with a trained predictor.
 To train a Lightwood predictor, refer to example/train.py
 To visualize from a Jupyter notebook, refer to example/visualize.ipynb
 """
 import pandas as pd
-from lightwood.data.splitter import stratify
+from dataprep_ml.splitters import stratify
 from lightwood.api.high_level import predictor_from_state
 from mindsdb_forecast_visualizer.core.dispatcher import forecast
 
 
 if __name__ == '__main__':
 
     # Load predictor
@@ -24,16 +24,16 @@
                                      pct_train=0.8,
                                      pct_dev=0,
                                      pct_test=0.2,
                                      stratify_on=['Country'],
                                      seed=1,
                                      reshuffle=False)
 
-    # Specify series and plot
-    subset = None  # [{'Country': 'UK'}, {'Country': 'US'}]  # None will plot all available series
+    # Specify series and plot. `None` will plot all available series.
+    subset = [{'Country': 'UK'}, {'Country': 'US'}, {'Country': 'Japan'}, {'Country': 'NZ'}]
 
     forecast(
         predictor,
         query_df,
         subset=subset,
         backfill=train_df,
         show_insample=False
```

### Comparing `mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer/config/config.py` & `mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer/config/config.py`

 * *Files identical despite different names*

### Comparing `mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer/core/forecaster.py` & `mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer/core/forecaster.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import traceback
 from typing import Union
 from copy import deepcopy
 from itertools import product
 from collections import OrderedDict
+import datetime
 
+import numpy as np
 import pandas as pd
 from mindsdb_forecast_visualizer.core.plotter import plot
 
-from lightwood.data.cleaner import _standardize_datetime
+from dataprep_ml.cleaners import _standardize_datetime
 
 
 def forecast(model,
              data: pd.DataFrame,
              subset: Union[list, None] = None,
              show_anomaly: bool = False,
              renderer: str = 'browser',
@@ -29,15 +31,14 @@
     :param show_insample: if True, in-sample forecasts will be plotted for any available backfill data.
     :param predargs: arguments passed to the predictor when generating forecasts for the visualization.
     :param warm_start_offset: how many rows from the backfill dataframe should be appended at the start of `data` to serve as historical context for mixers that have a cold start (e.g. neural, gbm).
     """  # noqa
 
     if show_insample and len(backfill) == 0:
         raise Exception("You must pass a dataframe with the predictor's training data to show in-sample forecasts.")
-    predargs['time_format'] = 'infer'
 
     # instantiate series according to groups
     group_values = OrderedDict()
     tss = model.problem_definition.timeseries_settings
     gby = tss.group_by if tss.group_by is not None else []
     for g in gby:
         group_values[g] = list(data[g].unique())
@@ -54,22 +55,28 @@
         warm_start_offset = tss.window
 
     # extract each series, predict for it, then plot
     for g in groups:
         if g == ():
             g = '__default'
         try:
-            filtered_backfill, test_data = get_group(g, subset, data, backfill, group_keys, order)
+            filtered_backfill, filtered_data = get_group(g, subset, data, backfill, group_keys, order)
 
-            if test_data.shape[0] > 0:
+            if filtered_data.shape[0] > 0:
                 print(f'Plotting for group {g}...')
-                original_test_data = test_data
-                test_data = test_data.iloc[[0]]  # library only supports plotting first horizon inside test dataset
 
-                filtered_data = pd.concat([filtered_backfill.iloc[-warm_start_offset:], test_data])
+                # check offset for warm start
+                special_mixers = ['GluonTSMixer', 'NHitsMixer']
+                if hasattr(model.ensemble, 'indexes_by_accuracy') and \
+                        (model.mixers[model.ensemble.indexes_by_accuracy[0]].__class__.__name__ in special_mixers):
+                    filtered_data = pd.concat([filtered_backfill.iloc[-warm_start_offset:], filtered_data.iloc[[0]]])
+                else:
+                    filtered_data = pd.concat([filtered_backfill.iloc[-warm_start_offset:], filtered_data])
+
+
                 if not tss.allow_incomplete_history:
                     assert filtered_data.shape[0] > tss.window
 
                 # arrays to plot
                 pred_target = []
                 time_target = []
                 conf_lower = []
@@ -79,44 +86,47 @@
 
                 # add data to backfill, if any
                 if len(filtered_backfill) > 0:
                     real_target += [float(r) for r in filtered_backfill[target]]
 
                 # forecast & divide into in-sample and out-sample predictions, if required
                 if show_insample:
+                    offset = predargs.get('forecast_offset', 0)
                     predargs['forecast_offset'] = -len(filtered_backfill)
                     model_fit = model.predict(filtered_backfill, args=predargs)
+                    predargs['forecast_offset'] = offset
                 else:
                     model_fit = None
                     if len(filtered_backfill) > 0:
-                        time_target += [t for t in filtered_backfill[tss.order_by]]
                         pred_target += [None for _ in range(len(filtered_backfill))]
                         conf_lower += [None for _ in range(len(filtered_backfill))]
                         conf_upper += [None for _ in range(len(filtered_backfill))]
                         anomalies += [None for _ in range(len(filtered_backfill))]
 
                 predargs['forecast_offset'] = -warm_start_offset
                 model_forecast = model.predict(filtered_data, args=predargs).iloc[warm_start_offset:]
-                real_target += [r for r in original_test_data[target]][:tss.horizon]
+                filtered_data = filtered_data.iloc[warm_start_offset:]
+                real_target += [float(r) for r in filtered_data[target]][:tss.horizon]
 
-                # edge case: convert one-step-ahead predictions to unitary lists
+                # convert one-step-ahead predictions to unitary lists
                 if not isinstance(model_forecast['prediction'].iloc[0], list):
-                    for k in ['prediction', 'lower', 'upper'] + [f'order_{i}' for i in tss.order_by]:
+                    for k in ['prediction', 'lower', 'upper'] + [f'order_{tss.order_by}']:
                         model_forecast[k] = model_forecast[k].apply(lambda x: [x])
                         if show_insample:
                             model_fit[k] = model_fit[k].apply(lambda x: [x])
 
                 if show_insample:
                     pred_target += [p[0] for p in model_fit['prediction']]
                     conf_lower += [p[0] for p in model_fit['lower']]
                     conf_upper += [p[0] for p in model_fit['upper']]
+                    time_target += [p[0] for p in model_fit[f'order_{order}']]
                     if 'anomaly' in model_fit.columns:
                         anomalies += [p for p in model_fit['anomaly']]
 
-                # forecast always corresponds to predicted arrays for the first out-of-sample query data point
+                # forecast corresponds to predicted arrays for the first out-of-sample query data point
                 fcst = {
                     'prediction': model_forecast['prediction'].iloc[0],
                     'lower': model_forecast['lower'].iloc[0],
                     'upper': model_forecast['upper'].iloc[0]
                 }
 
                 # wrap if needed
@@ -130,18 +140,31 @@
                         fcst[k] = [v[0]]
                 else:
                     separate = True
 
                 pred_target += [p for p in fcst['prediction']]
                 conf_lower += [p for p in fcst['lower']]
                 conf_upper += [p for p in fcst['upper']]
-                time_target += [r for r in original_test_data[tss.order_by]][:tss.horizon]
+
+                # fix timestamps
+                time_target = [pd.to_datetime(p).timestamp() for p in filtered_data[order]]
+                try:
+                    delta = model.ts_analysis['deltas'][g]
+                except:
+                    delta = model.ts_analysis['deltas'].get(tuple([str(gg) for gg in g]),
+                                                            model.ts_analysis['deltas']['__default'])
+
+                for i in range(len(pred_target) - len(time_target)):
+                    time_target.insert(0, time_target[0] - delta)
+
+
+                time_target = [datetime.datetime.utcfromtimestamp(ts).strftime('%Y-%m-%d %H:%M:%S') for ts in time_target]
 
                 # round confidences
-                conf = model_forecast['confidence'].values.mean()
+                conf = np.array([np.array(l) for l in model_forecast['confidence'].values]).mean()
 
                 # set titles and legends
                 if g != ():
                     title = f'MindsDB T+{forecasting_window} forecast for group {g} (confidence: {conf})'
                 else:
                     title = f'MindsDB T+{forecasting_window} forecast (confidence: {conf})'
                 titles = {'title': title,
@@ -157,29 +180,31 @@
                            conf_upper,
                            fh_idx=len(pred_target)-tss.horizon,
                            renderer=renderer,
                            labels=titles,
                            anomalies=anomalies if show_anomaly else None,
                            separate=separate)
                 fig.show()
+            else:
+                print(f"No data for group {g}. Skipping...")
 
         except Exception:
             print(f"Error in group {g}:")
             print(traceback.format_exc())
 
 
 def get_group(g, subset, data, backfill, group_keys, order):
     filtered_data = pd.DataFrame() if g != () else data
     filtered_backfill = pd.DataFrame() if g != () else data
     group_dict = {k: v for k, v in zip(group_keys, g)}
 
     if subset is None or group_dict in subset:
-        filtered_data = deepcopy(data)
-        filtered_backfill = deepcopy(backfill)
+        filtered_data = data
+        filtered_backfill = backfill
         for k, v in group_dict.items():
-            filtered_data = filtered_data[filtered_data[k] == v]
-            filtered_backfill = filtered_backfill[filtered_backfill[k] == v]
+            filtered_data = deepcopy(filtered_data[filtered_data[k] == v])
+            filtered_backfill = deepcopy(filtered_backfill[filtered_backfill[k] == v])
 
     filtered_data = filtered_data.drop_duplicates(subset=order)
     filtered_backfill = filtered_backfill.drop_duplicates(subset=order)
 
     return filtered_backfill, filtered_data
```

### Comparing `mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer/core/plotter.py` & `mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer/core/plotter.py`

 * *Files identical despite different names*

### Comparing `mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer.egg-info/PKG-INFO` & `mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindsdb-forecast-visualizer
-Version: 22.8.4.0
+Version: 23.7.4.1
 Summary: Companion package to visualizer forecasts made with MindsDB predictors.
 Home-page: https://github.com/mindsdb/mindsdb_forecast_visualizer
 Author: MindsDB Inc
 Author-email: community@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb_forecast_visualizer
 Description: # MindsDB Forecast Visualizer
```

### Comparing `mindsdb_forecast_visualizer-22.8.4.0/mindsdb_forecast_visualizer.egg-info/SOURCES.txt` & `mindsdb_forecast_visualizer-23.7.4.1/mindsdb_forecast_visualizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mindsdb_forecast_visualizer-22.8.4.0/setup.py` & `mindsdb_forecast_visualizer-23.7.4.1/setup.py`

 * *Files identical despite different names*

