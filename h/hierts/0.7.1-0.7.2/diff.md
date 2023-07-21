# Comparing `tmp/hierts-0.7.1.tar.gz` & `tmp/hierts-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hierts-0.7.1.tar", last modified: Tue Jul  4 18:21:34 2023, max compression
+gzip compressed data, was "hierts-0.7.2.tar", last modified: Fri Jul 21 17:21:39 2023, max compression
```

## Comparing `hierts-0.7.1.tar` & `hierts-0.7.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 18:21:34.942240 hierts-0.7.1/
--rw-rw-rw-   0        0        0    10983 2022-07-06 12:50:59.000000 hierts-0.7.1/LICENSE
--rw-rw-rw-   0        0        0    14645 2023-07-04 18:21:34.942240 hierts-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     1589 2022-08-12 07:31:52.000000 hierts-0.7.1/README.md
--rw-rw-rw-   0        0        0      795 2023-07-04 18:21:21.000000 hierts-0.7.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 18:21:34.942240 hierts-0.7.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-04 18:21:34.918112 hierts-0.7.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-04 18:21:34.923113 hierts-0.7.1/src/hierts/
--rw-rw-rw-   0        0        0      153 2022-07-06 07:17:40.000000 hierts-0.7.1/src/hierts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 18:21:34.940240 hierts-0.7.1/src/hierts/_old/
--rw-rw-rw-   0        0        0    17256 2022-07-11 17:10:06.000000 hierts-0.7.1/src/hierts/_old/reconciliation.py
--rw-rw-rw-   0        0        0    25044 2023-07-04 18:19:55.000000 hierts-0.7.1/src/hierts/reconciliation.py
-drwxrwxrwx   0        0        0        0 2023-07-04 18:21:34.939240 hierts-0.7.1/src/hierts.egg-info/
--rw-rw-rw-   0        0        0    14645 2023-07-04 18:21:34.000000 hierts-0.7.1/src/hierts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-07-04 18:21:34.000000 hierts-0.7.1/src/hierts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 18:21:34.000000 hierts-0.7.1/src/hierts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-04 18:21:34.000000 hierts-0.7.1/src/hierts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-04 18:21:34.000000 hierts-0.7.1/src/hierts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 17:21:39.488857 hierts-0.7.2/
+-rw-rw-rw-   0        0        0    10983 2022-07-06 12:50:59.000000 hierts-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0    14645 2023-07-21 17:21:39.488857 hierts-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1589 2022-08-12 07:31:52.000000 hierts-0.7.2/README.md
+-rw-rw-rw-   0        0        0      795 2023-07-21 17:18:51.000000 hierts-0.7.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-21 17:21:39.489857 hierts-0.7.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-21 17:21:39.456825 hierts-0.7.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-21 17:21:39.463856 hierts-0.7.2/src/hierts/
+-rw-rw-rw-   0        0        0      153 2022-07-06 07:17:40.000000 hierts-0.7.2/src/hierts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 17:21:39.486858 hierts-0.7.2/src/hierts/_old/
+-rw-rw-rw-   0        0        0    17256 2022-07-11 17:10:06.000000 hierts-0.7.2/src/hierts/_old/reconciliation.py
+-rw-rw-rw-   0        0        0    26251 2023-07-21 17:06:45.000000 hierts-0.7.2/src/hierts/reconciliation.py
+drwxrwxrwx   0        0        0        0 2023-07-21 17:21:39.485858 hierts-0.7.2/src/hierts.egg-info/
+-rw-rw-rw-   0        0        0    14645 2023-07-21 17:21:39.000000 hierts-0.7.2/src/hierts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-07-21 17:21:39.000000 hierts-0.7.2/src/hierts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 17:21:39.000000 hierts-0.7.2/src/hierts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-21 17:21:39.000000 hierts-0.7.2/src/hierts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-21 17:21:39.000000 hierts-0.7.2/src/hierts.egg-info/top_level.txt
```

### Comparing `hierts-0.7.1/LICENSE` & `hierts-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hierts-0.7.1/PKG-INFO` & `hierts-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hierts
-Version: 0.7.1
+Version: 0.7.2
 Summary: Hierarchical time series reconciliation
 Author-email: Olivier Sprangers <o.r.sprangers@uva.nl>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `hierts-0.7.1/README.md` & `hierts-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `hierts-0.7.1/pyproject.toml` & `hierts-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hierts"
-version = "0.7.1"
+version = "0.7.2"
 authors = [
   { name="Olivier Sprangers", email="o.r.sprangers@uva.nl" },
 ]
 description = "Hierarchical time series reconciliation"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `hierts-0.7.1/src/hierts/_old/reconciliation.py` & `hierts-0.7.2/src/hierts/_old/reconciliation.py`

 * *Files identical despite different names*

### Comparing `hierts-0.7.1/src/hierts/reconciliation.py` & `hierts-0.7.2/src/hierts/reconciliation.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         residuals = yhat_train - y_train
         W = np.cov(residuals)
         UtW = Ut @ W
     elif method == 'mint_shrink':
         # Trace minimization using the shrunk empirical covariance matrix
         residuals = yhat_train - y_train
         residuals_mean = np.mean(residuals, axis=1)
-        residuals_std = np.std(residuals, axis=1)
+        residuals_std = np.maximum(np.std(residuals, axis=1), 1e-6)
         W = shrunk_covariance_schaferstrimmer(residuals, residuals_mean, residuals_std)
         UtW = Ut @ W
     elif method == 'erm':
         # Ref. eq. 18, 19 and 25 of Taieb, 2019. 
         Bt = np.linalg.inv(S.T @ S) @ S.T @ y_train
         P = (np.linalg.pinv(yhat_train.T) @ Bt.T).T
     elif method == 'erm_reg':
@@ -202,15 +202,15 @@
         :param name_bottom_timeseries: name for the bottom level time series in the hierarchy, defaults to 'bottom_timeseries'.
         :type name_bottom_timeseries: str
         
         :return: df_S, output dataframe containing the summing matrix of shape [(n_bottom_timeseries + n_aggregate_timeseries) x n_bottom_timeseries]. The number of aggregate time series is the result of applying all the required aggregations.
         :rtype: pd.DataFrame filled with np.float32
     
     """
-    print("'calc_summing_matrix' is deprecated. Please use hierarchy_cross_sectional to compute cross-sectional hierarchies")
+    print("'calc_summing_matrix' is deprecated. Please use hierarchy_cross_sectional to compute cross-sectional hierarchies.")
 
     return None
 
 def hierarchy_cross_sectional(df: pd.DataFrame, aggregations: List[List[str]], 
                         sparse: bool = False, name_bottom_timeseries: str = 'bottom_timeseries') -> pd.DataFrame:
     """Given a dataframe of timeseries and columns indicating their groupings, this function calculates a cross-sectional hierarchy according to a set of specified aggregations for the time series.
 
@@ -381,15 +381,15 @@
     
     """
     # Check to ensure correct inputs are given
     assert set(df_S.columns) == set(forecasts.index), 'Index of forecasts should match columns of df_S'
     # Convert df_S 
     if hasattr(df_S, "sparse"):
         print("S is sparse")
-        S = csc_matrix(df_S.sparse.to_coo())
+        S = df_S.sparse.to_coo().tocsc()
     else:
         print("S is dense")
         S = df_S.values
     # Bottom-up forecasts
     all_aggregations = df_S.index.get_level_values('Aggregation').unique()
     all_aggregations = all_aggregations.drop(name_bottom_timeseries)
     forecasts_bu = pd.DataFrame(index=df_S.index, columns=forecasts.columns)
@@ -410,31 +410,54 @@
         :type base: str
         
         :return: tuple containing (i) rmse for all methods, across all levels, and (ii) relative rmse for all methods, across all levels. 
         :rtype: Tuple[pd.DataFrame, pd.DataFrame]
     
     """
     # Input verification
-    assert base in forecasts_methods.index, f'Chosen base {base} not in index of forecasts_methods'
+    print("calc_level_method_rmse is deprecated as of version 0.8. Please use calc_level_method_error(error='rmse') instead.")
+
+    return None
+
+def calc_level_method_error(forecasts_methods: pd.DataFrame, actuals: pd.DataFrame, 
+                            metric: str = 'RMSE') -> pd.DataFrame:
+    """Calculate RMSE for each level, for each method for a set of forecasts.
     
-    # Compute rmse for all methods & levels
-    rmse_index = forecasts_methods.index.droplevel(['Value']).drop_duplicates()
-    rmse = pd.DataFrame(index=rmse_index, columns=['RMSE'], dtype=np.float64)
-    # rmse = pd.DataFrame()
+        :param forecasts_methods: dataframe containing forecasts for all reconciliation methods
+        :type forecasts_methods: pd.DataFrame
+        :param actuals: Dataframe containing the ground truth for all time series
+        :type actuals: pd.DataFrame
+        :param metric: metric to compute. Options are: ['RMSE', 'MAE']
+        :type metric: str
+                
+        :return: Error for all methods, across all levels.
+        :rtype: pd.DataFrame
+    
+    """   
+    # Compute error for all methods & levels
+    error_index = forecasts_methods.index.droplevel(['Value']).drop_duplicates()
+    error = pd.DataFrame(index=error_index, columns=[metric], dtype=np.float64)
     methods = forecasts_methods.index.get_level_values('Method').unique()
     for method in methods:
         forecasts_method = forecasts_methods.loc[method]
-        sq_error = ((forecasts_method - actuals.loc[:, forecasts_method.columns])**2).stack()
-        rmse_current = np.sqrt(sq_error.groupby(['Aggregation']).mean())
-        rmse.loc[(method, slice(None)), 'RMSE'] = rmse_current.loc[rmse.loc[method, 'RMSE'].index].values
-        rmse.loc[(method, 'All series'), 'RMSE'] = np.sqrt(sq_error.mean())
-        
-    rmse = rmse.sort_index().unstack(0)
+        if metric == "RMSE":
+            sq_error = ((forecasts_method - actuals.loc[:, forecasts_method.columns])**2).stack()
+            error_current = np.sqrt(sq_error.groupby(['Aggregation']).mean())
+            error.loc[(method, slice(None)), metric] = error_current.loc[error.loc[method, metric].index].values
+            error.loc[(method, 'All series'), metric] = np.sqrt(sq_error.mean())
+        elif metric == "MAE":
+            abs_error = np.abs(forecasts_method - actuals.loc[:, forecasts_method.columns]).stack()
+            error_current = abs_error.groupby(['Aggregation']).mean()
+            error.loc[(method, slice(None)), metric] = error_current.loc[error.loc[method, metric].index].values
+            error.loc[(method, 'All series'), metric] = abs_error.mean()
+        else:
+            raise NotImplementedError()
+
+    error = error.sort_index().unstack(0)
     # Sort by base, then put in order: Total first, bottom-level series (i.e. None) penultimate, aggregate
     # over all time series + aggregates ('All series') last
-    rmse.columns = rmse.columns.droplevel(0)
-    rmse = rmse[methods].sort_values(by=base, ascending=False)
-    index_cols = list(rmse.index.drop('All series')) + ['All series']
-    rmse = rmse.reindex(index = index_cols)
-    rel_rmse = rmse.div(rmse[base], axis=0)
+    error.columns = error.columns.droplevel(0)
+    # error = error[methods].sort_values(by=base, ascending=False)
+    index_cols = list(error.index.drop('All series')) + ['All series']
+    error = error.reindex(index = index_cols)
 
-    return rmse, rel_rmse
+    return error
```

### Comparing `hierts-0.7.1/src/hierts.egg-info/PKG-INFO` & `hierts-0.7.2/src/hierts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hierts
-Version: 0.7.1
+Version: 0.7.2
 Summary: Hierarchical time series reconciliation
 Author-email: Olivier Sprangers <o.r.sprangers@uva.nl>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

