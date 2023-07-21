# Comparing `tmp/TEST_TC-1.1.4.tar.gz` & `tmp/TEST_TC-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TEST_TC-1.1.4.tar", last modified: Thu Jul 20 16:26:49 2023, max compression
+gzip compressed data, was "TEST_TC-1.1.5.tar", last modified: Fri Jul 21 11:33:04 2023, max compression
```

## Comparing `TEST_TC-1.1.4.tar` & `TEST_TC-1.1.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.205072 TEST_TC-1.1.4/
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.137490 TEST_TC-1.1.4/LIB_tc/
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.155483 TEST_TC-1.1.4/LIB_tc/TEST_TC.egg-info/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-20 16:26:49.000000 TEST_TC-1.1.4/LIB_tc/TEST_TC.egg-info/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1284 2023-07-20 16:26:49.000000 TEST_TC-1.1.4/LIB_tc/TEST_TC.egg-info/SOURCES.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 16:26:49.000000 TEST_TC-1.1.4/LIB_tc/TEST_TC.egg-info/dependency_links.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      341 2023-07-20 16:26:49.000000 TEST_TC-1.1.4/LIB_tc/TEST_TC.egg-info/requires.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        8 2023-07-20 16:26:49.000000 TEST_TC-1.1.4/LIB_tc/TEST_TC.egg-info/top_level.txt
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.158217 TEST_TC-1.1.4/LIB_tc/test_tc/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-07-20 16:26:06.000000 TEST_TC-1.1.4/LIB_tc/test_tc/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.168143 TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6535 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/experiment.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7719 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/job.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    24471 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/models.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15714 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/utils.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.172160 TEST_TC-1.1.4/LIB_tc/test_tc/analytics/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/analytics/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5777 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/analytics/evaluationMetrics.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.177008 TEST_TC-1.1.4/LIB_tc/test_tc/datahandler/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/datahandler/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7303 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/datahandler/datahandler.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.181374 TEST_TC-1.1.4/LIB_tc/test_tc/datapreparation/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/datapreparation/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4014 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/datapreparation/preprocessing.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    25441 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/datapreparation/utils.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.182443 TEST_TC-1.1.4/LIB_tc/test_tc/dataset/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/dataset/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.187916 TEST_TC-1.1.4/LIB_tc/test_tc/datavisualization/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/datavisualization/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    13008 2023-07-20 16:25:46.000000 TEST_TC-1.1.4/LIB_tc/test_tc/datavisualization/plotPrediction.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14693 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14566 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/datavisualization/visualization.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.200823 TEST_TC-1.1.4/LIB_tc/test_tc/utility/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/utility/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2822 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/utility/check_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16272 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/utility/configuration_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1515 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/utility/constants.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1849 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/utility/exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2440 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/utility/resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6048 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/utility/tele_logger.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-20 16:26:49.203823 TEST_TC-1.1.4/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1873 2023-06-28 16:32:49.000000 TEST_TC-1.1.4/README.md
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1323 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/pyproject.toml
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-07-20 16:26:49.205072 TEST_TC-1.1.4/setup.cfg
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-21 11:33:04.638342 TEST_TC-1.1.5/
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-21 11:33:04.520886 TEST_TC-1.1.5/LIB_tc/
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-21 11:33:04.548358 TEST_TC-1.1.5/LIB_tc/TEST_TC.egg-info/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-21 11:33:04.000000 TEST_TC-1.1.5/LIB_tc/TEST_TC.egg-info/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1284 2023-07-21 11:33:04.000000 TEST_TC-1.1.5/LIB_tc/TEST_TC.egg-info/SOURCES.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-21 11:33:04.000000 TEST_TC-1.1.5/LIB_tc/TEST_TC.egg-info/dependency_links.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      341 2023-07-21 11:33:04.000000 TEST_TC-1.1.5/LIB_tc/TEST_TC.egg-info/requires.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        8 2023-07-21 11:33:04.000000 TEST_TC-1.1.5/LIB_tc/TEST_TC.egg-info/top_level.txt
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-21 11:33:04.551359 TEST_TC-1.1.5/LIB_tc/test_tc/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-07-21 11:28:38.000000 TEST_TC-1.1.5/LIB_tc/test_tc/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-21 11:33:04.567116 TEST_TC-1.1.5/LIB_tc/test_tc/algorithms/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/LIB_tc/test_tc/algorithms/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6535 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/LIB_tc/test_tc/algorithms/experiment.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7761 2023-07-21 11:28:30.000000 TEST_TC-1.1.5/LIB_tc/test_tc/algorithms/job.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    24476 2023-07-21 11:28:30.000000 TEST_TC-1.1.5/LIB_tc/test_tc/algorithms/models.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15885 2023-07-21 11:28:30.000000 TEST_TC-1.1.5/LIB_tc/test_tc/algorithms/utils.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-21 11:33:04.573416 TEST_TC-1.1.5/LIB_tc/test_tc/analytics/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/LIB_tc/test_tc/analytics/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6464 2023-07-21 11:28:30.000000 TEST_TC-1.1.5/LIB_tc/test_tc/analytics/evaluationMetrics.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-21 11:33:04.580183 TEST_TC-1.1.5/LIB_tc/test_tc/datahandler/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/LIB_tc/test_tc/datahandler/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7303 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/LIB_tc/test_tc/datahandler/datahandler.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-21 11:33:04.592219 TEST_TC-1.1.5/LIB_tc/test_tc/datapreparation/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/LIB_tc/test_tc/datapreparation/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4014 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/LIB_tc/test_tc/datapreparation/preprocessing.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    25441 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/LIB_tc/test_tc/datapreparation/utils.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-21 11:33:04.596220 TEST_TC-1.1.5/LIB_tc/test_tc/dataset/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/LIB_tc/test_tc/dataset/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-21 11:33:04.609046 TEST_TC-1.1.5/LIB_tc/test_tc/datavisualization/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/LIB_tc/test_tc/datavisualization/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    13008 2023-07-21 11:28:15.000000 TEST_TC-1.1.5/LIB_tc/test_tc/datavisualization/plotPrediction.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14693 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14566 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/LIB_tc/test_tc/datavisualization/visualization.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-21 11:33:04.633373 TEST_TC-1.1.5/LIB_tc/test_tc/utility/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/LIB_tc/test_tc/utility/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2822 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/LIB_tc/test_tc/utility/check_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16272 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/LIB_tc/test_tc/utility/configuration_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1515 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/LIB_tc/test_tc/utility/constants.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1849 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/LIB_tc/test_tc/utility/exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2440 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/LIB_tc/test_tc/utility/resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6048 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/LIB_tc/test_tc/utility/tele_logger.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-21 11:33:04.636926 TEST_TC-1.1.5/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1873 2023-06-28 16:32:49.000000 TEST_TC-1.1.5/README.md
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1323 2023-07-20 16:00:24.000000 TEST_TC-1.1.5/pyproject.toml
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-07-21 11:33:04.638342 TEST_TC-1.1.5/setup.cfg
```

### Comparing `TEST_TC-1.1.4/LIB_tc/TEST_TC.egg-info/SOURCES.txt` & `TEST_TC-1.1.5/LIB_tc/TEST_TC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/experiment.py` & `TEST_TC-1.1.5/LIB_tc/test_tc/algorithms/experiment.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/job.py` & `TEST_TC-1.1.5/LIB_tc/test_tc/algorithms/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
             best_reconciler = os.listdir(os.path.join(best_run.artifact_uri, folder_best_reconcile))[0]
             reconciler_uri = f"runs:/{best_run['run_id']}/{folder_best_reconcile}/{best_reconciler}"
             self.best_reconciler = mlflow.sklearn.load_model(reconciler_uri)
 
             path_artifacts = os.path.join(best_run.artifact_uri, 'dataframes')
             with open(os.path.join(path_artifacts, 'tags.json'), 'r') as f:
                 tmp = json.load(f)
+
             valid_true = pd.read_parquet(os.path.join(path_artifacts, 'valid_real.parquet'))
             valid_pred = pd.read_parquet(os.path.join(path_artifacts, 'valid_pred.parquet'))
             test_true  = pd.read_parquet(os.path.join(path_artifacts, 'test_real.parquet'))
             test_pred  = pd.read_parquet(os.path.join(path_artifacts, 'test_pred.parquet'))
 
             self.X_true = pd.concat([valid_true, test_true])
             self.X_pred = pd.concat([valid_pred, test_pred])
@@ -159,20 +160,20 @@
         logger.info("START Predicting Future data.", important=True)
 
         self.find_best_run(decision_function=decision_function)
         self.make_future_dataset(start_date=start_date, num_forecast_periods=num_forecast_periods)
         forecast_model = self.Model.predict(self.future_df)
 
         if self.apply_hierarchical:
-            logger.info("Applying Hierarchical Reconciliation method.")
-
             try:
                 reconcile = f'{self.best_reconciler.__class__.__name__}(method="{self.best_reconciler.method}")'
             except AttributeError:
                 reconcile = f'{self.best_reconciler.__class__.__name__}()'
+            
+            logger.info(f'Applying Hierarchical Reconciliation Model: {reconcile}', important=True)
 
             HRM = HierarchicalReconcileModel(model_name=self.model_name, S=self.S, tags=self.tags, reconciler=reconcile)
             forecast_rec = HRM.fit_predict(X_true=self.X_true, X_pred=self.X_pred, X_future_pred=forecast_model, as_output=True)
 
             return forecast_model, forecast_rec
         else:
             return forecast_model, None
```

### Comparing `TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/models.py` & `TEST_TC-1.1.5/LIB_tc/test_tc/algorithms/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,17 +301,17 @@
         self.model_name = model_name
         self.S          = S
         self.tags       = tags
 
         self.max_na_ratio = max_na_ratio
 
         if reconciler == None:
-            self.reconciler = [BottomUp(),MinTrace(method='mint_shrink'),
-                    MinTrace(method='ols'),TopDown(method= 'average_proportions'),
-                    TopDown(method= 'proportion_averages')]
+            self.reconciler = [BottomUp(),
+                        TopDown(method= 'average_proportions'),TopDown(method= 'proportion_averages')]
+                    # MinTrace(method='mint_shrink'),MinTrace(method='ols')
         else:
             if isinstance(reconciler, str):
                 self.reconciler = [eval(reconciler)]
             elif isinstance(reconciler, list):
                 self.reconciler = reconciler
             else:
                 self.reconciler = [reconciler]
```

### Comparing `TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/utils.py` & `TEST_TC-1.1.5/LIB_tc/test_tc/algorithms/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         elif type(config_hyperparameters[param]) == dict:
             check_not_in_iterable(obj=param, iterable=list(default_steps.keys()), func=get_module_and_function(),
                                   attached_message=f'Parameter {param} do NOT have a default setting, add it inside the config/default_steps.toml')
 
             grid_parameters[param] = generate_values(config_hyperparameters[param], default_step = default_steps[param])
 
         else:
-            raise ValueError(f' The value datetype of {param} is not valid')
+            raise ValueError(f' The value datatype of {param} is not valid')
     return grid_parameters
 
 def model_tuning(model: Type[Callable], evaluator: Type[EvaluateModel], unique_id: str,
                  grid_params: Dict[str, List[Union[str, bool, int, float]]], 
                  train_df: pd.DataFrame, validation_df: pd.DataFrame,
                  decision_function: str = 'rmse*0.5 + mae*0.5') -> Dict[str, Union[str, bool, int, float]]:
     """
@@ -290,26 +290,26 @@
 
     return df
 
 
 def mlflow_log_artifact(predict_real_folder: str, experiment_name: str, 
                         df_to_save: List[Tuple[pd.DataFrame, str]] =None,
                         json_to_save: List[Tuple[Dict[str, List[str]], str]] =None):
-    """_summary_
+    """The function logs, if provided, the dataframes and the jsons on MLFlow
 
     Parameters
     ----------
     predict_real_folder : str
-        _description_
+        The local folder to temporary save the data
     experiment_name : str
-        _description_
+        The name of the experiment
     df_to_save : List[Tuple[pd.DataFrame, str]], optional
-        _description_, by default None
+        The list of tuples (dataframes, filename) to save , by default None
     json_to_save : List[Tuple[Dict[str, List[str]], str]], optional
-        _description_, by default None
+        The list of tuples (dict, filename) to save, by default None
     """
         
     logger.info('START logging results.', important=True)
 
     save_data_folder = os.path.join(predict_real_folder, experiment_name)
 
     # If there are dataframes to save, apply the function
```

### Comparing `TEST_TC-1.1.4/LIB_tc/test_tc/analytics/evaluationMetrics.py` & `TEST_TC-1.1.5/LIB_tc/test_tc/analytics/evaluationMetrics.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import pandas as pd
 import numpy as np
 from sklearn.metrics import mean_squared_error, r2_score, mean_absolute_error, mean_absolute_percentage_error
 
+from ..utility.check_utils import check_not_isinstance
+from ..utility.resources import get_module_and_function
 from ..utility.exceptions import ColumnNotFound
 from ..utility.tele_logger import logger
 
 
 class EvaluateModel():
     def __init__(self, date_true: str, date_pred: str, y_true: str, y_pred: str, upper_95: str, lower_95: str):
         """_summary_
@@ -21,14 +23,20 @@
         y_pred : str
             Target column name for the predicted datasets
         upper_95 : str
             Column name for Upper CI at 95%
         lower_95 : str
             Column name for Lower CI at 95%
         """
+        check_not_isinstance(obj = date_true, data_type = str, func= get_module_and_function())
+        check_not_isinstance(obj = date_pred, data_type = str, func= get_module_and_function())
+        check_not_isinstance(obj = y_true, data_type = str, func= get_module_and_function())
+        check_not_isinstance(obj = y_pred, data_type = str, func= get_module_and_function())
+        check_not_isinstance(obj = upper_95, data_type = str, func= get_module_and_function())
+        check_not_isinstance(obj = lower_95, data_type = str, func= get_module_and_function())
         self.date_true = date_true
         self.date_pred = date_pred
         self.y_true = y_true
         self.y_pred = y_pred
         self.upper_95 = upper_95
         self.lower_95 = lower_95
```

### Comparing `TEST_TC-1.1.4/LIB_tc/test_tc/datahandler/datahandler.py` & `TEST_TC-1.1.5/LIB_tc/test_tc/datahandler/datahandler.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.4/LIB_tc/test_tc/datapreparation/preprocessing.py` & `TEST_TC-1.1.5/LIB_tc/test_tc/datapreparation/preprocessing.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.4/LIB_tc/test_tc/datapreparation/utils.py` & `TEST_TC-1.1.5/LIB_tc/test_tc/datapreparation/utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.4/LIB_tc/test_tc/datavisualization/plotPrediction.py` & `TEST_TC-1.1.5/LIB_tc/test_tc/datavisualization/plotPrediction.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.4/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py` & `TEST_TC-1.1.5/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.4/LIB_tc/test_tc/datavisualization/visualization.py` & `TEST_TC-1.1.5/LIB_tc/test_tc/datavisualization/visualization.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.4/LIB_tc/test_tc/utility/check_utils.py` & `TEST_TC-1.1.5/LIB_tc/test_tc/utility/check_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.4/LIB_tc/test_tc/utility/configuration_utils.py` & `TEST_TC-1.1.5/LIB_tc/test_tc/utility/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.4/LIB_tc/test_tc/utility/constants.py` & `TEST_TC-1.1.5/LIB_tc/test_tc/utility/constants.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.4/LIB_tc/test_tc/utility/exceptions.py` & `TEST_TC-1.1.5/LIB_tc/test_tc/utility/exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.4/LIB_tc/test_tc/utility/resources.py` & `TEST_TC-1.1.5/LIB_tc/test_tc/utility/resources.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.4/LIB_tc/test_tc/utility/tele_logger.py` & `TEST_TC-1.1.5/LIB_tc/test_tc/utility/tele_logger.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.4/README.md` & `TEST_TC-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.4/pyproject.toml` & `TEST_TC-1.1.5/pyproject.toml`

 * *Files identical despite different names*

