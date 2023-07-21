# Comparing `tmp/pyDataFitting-0.0.3.tar.gz` & `tmp/pyDataFitting-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDataFitting-0.0.3.tar", last modified: Fri Apr 14 12:37:04 2023, max compression
+gzip compressed data, was "pyDataFitting-0.0.4.tar", last modified: Fri Jul 21 14:15:03 2023, max compression
```

## Comparing `pyDataFitting-0.0.3.tar` & `pyDataFitting-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 12:37:04.730266 pyDataFitting-0.0.3/
--rw-rw-rw-   0        0        0     1095 2023-01-17 12:23:36.000000 pyDataFitting-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     5091 2023-04-14 12:37:05.533467 pyDataFitting-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4506 2023-04-14 10:10:48.000000 pyDataFitting-0.0.3/README.md
--rw-rw-rw-   0        0        0      110 2023-01-17 12:23:36.000000 pyDataFitting-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      722 2023-04-14 12:37:05.543903 pyDataFitting-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      273 2023-04-14 12:32:37.000000 pyDataFitting-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 12:37:04.802267 pyDataFitting-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 12:37:04.802267 pyDataFitting-0.0.3/src/pyDataFitting/
--rw-rw-rw-   0        0        0      208 2023-04-14 09:55:23.000000 pyDataFitting-0.0.3/src/pyDataFitting/__init__.py
--rw-rw-rw-   0        0        0     4067 2023-01-17 12:23:36.000000 pyDataFitting-0.0.3/src/pyDataFitting/linear_regression.py
--rw-rw-rw-   0        0        0     1669 2023-04-14 09:13:47.000000 pyDataFitting-0.0.3/src/pyDataFitting/model_diagnostics.py
--rw-rw-rw-   0        0        0    13711 2023-04-14 11:10:40.000000 pyDataFitting-0.0.3/src/pyDataFitting/model_tools.py
--rw-rw-rw-   0        0        0    58327 2023-01-17 12:23:36.000000 pyDataFitting-0.0.3/src/pyDataFitting/multivariate_regression.py
--rw-rw-rw-   0        0        0     6063 2023-01-17 12:23:36.000000 pyDataFitting-0.0.3/src/pyDataFitting/nonlinear_regression.py
--rw-rw-rw-   0        0        0    23760 2023-01-17 12:23:36.000000 pyDataFitting-0.0.3/src/pyDataFitting/polynomial_regression.py
-drwxrwxrwx   0        0        0        0 2023-04-14 12:37:04.810267 pyDataFitting-0.0.3/src/pyDataFitting.egg-info/
--rw-rw-rw-   0        0        0     5091 2023-04-14 12:37:04.000000 pyDataFitting-0.0.3/src/pyDataFitting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      708 2023-04-14 12:37:04.000000 pyDataFitting-0.0.3/src/pyDataFitting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 12:37:04.000000 pyDataFitting-0.0.3/src/pyDataFitting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-04-14 12:37:04.000000 pyDataFitting-0.0.3/src/pyDataFitting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-14 12:37:04.000000 pyDataFitting-0.0.3/src/pyDataFitting.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 12:37:04.814267 pyDataFitting-0.0.3/tests/
--rw-rw-rw-   0        0        0     2989 2023-04-14 11:51:38.000000 pyDataFitting-0.0.3/tests/test_model_tools.py
--rw-rw-rw-   0        0        0     2367 2023-04-14 12:16:08.000000 pyDataFitting-0.0.3/tests/test_nonlinear_regresssion.py
--rw-rw-rw-   0        0        0     3959 2023-01-17 12:23:36.000000 pyDataFitting-0.0.3/tests/test_piecewise_polynomial_fit.py
--rw-rw-rw-   0        0        0     3387 2023-01-17 12:23:36.000000 pyDataFitting-0.0.3/tests/test_polynomial_regression.py
--rw-rw-rw-   0        0        0     2413 2023-01-17 12:23:36.000000 pyDataFitting-0.0.3/tests/test_principal_component_regression.py
+drwxrwxrwx   0        0        0        0 2023-07-21 14:15:03.194839 pyDataFitting-0.0.4/
+-rw-rw-rw-   0        0        0     1095 2023-01-17 12:23:36.000000 pyDataFitting-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5256 2023-07-21 14:15:03.748299 pyDataFitting-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4671 2023-04-14 12:49:18.000000 pyDataFitting-0.0.4/README.md
+-rw-rw-rw-   0        0        0      110 2023-01-17 12:23:36.000000 pyDataFitting-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      722 2023-07-21 14:15:03.758595 pyDataFitting-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      273 2023-07-21 14:13:36.000000 pyDataFitting-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 14:15:03.194839 pyDataFitting-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-21 14:15:03.194839 pyDataFitting-0.0.4/src/pyDataFitting/
+-rw-rw-rw-   0        0        0      307 2023-04-14 13:25:24.000000 pyDataFitting-0.0.4/src/pyDataFitting/__init__.py
+-rw-rw-rw-   0        0        0     4067 2023-01-17 12:23:36.000000 pyDataFitting-0.0.4/src/pyDataFitting/linear_regression.py
+-rw-rw-rw-   0        0        0     1669 2023-04-14 09:13:47.000000 pyDataFitting-0.0.4/src/pyDataFitting/model_diagnostics.py
+-rw-rw-rw-   0        0        0    13711 2023-04-14 11:10:40.000000 pyDataFitting-0.0.4/src/pyDataFitting/model_tools.py
+-rw-rw-rw-   0        0        0     6063 2023-01-17 12:23:36.000000 pyDataFitting-0.0.4/src/pyDataFitting/nonlinear_regression.py
+-rw-rw-rw-   0        0        0    11118 2023-04-14 12:54:35.000000 pyDataFitting-0.0.4/src/pyDataFitting/partial_least_squares_regression.py
+-rw-rw-rw-   0        0        0    23760 2023-01-17 12:23:36.000000 pyDataFitting-0.0.4/src/pyDataFitting/polynomial_regression.py
+-rw-rw-rw-   0        0        0    47982 2023-06-07 14:43:30.000000 pyDataFitting-0.0.4/src/pyDataFitting/principle_component_regression.py
+drwxrwxrwx   0        0        0        0 2023-07-21 14:15:03.198839 pyDataFitting-0.0.4/src/pyDataFitting.egg-info/
+-rw-rw-rw-   0        0        0     5256 2023-07-21 14:15:03.000000 pyDataFitting-0.0.4/src/pyDataFitting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      769 2023-07-21 14:15:03.000000 pyDataFitting-0.0.4/src/pyDataFitting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 14:15:03.000000 pyDataFitting-0.0.4/src/pyDataFitting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-07-21 14:15:03.000000 pyDataFitting-0.0.4/src/pyDataFitting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-21 14:15:03.000000 pyDataFitting-0.0.4/src/pyDataFitting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 14:15:03.202839 pyDataFitting-0.0.4/tests/
+-rw-rw-rw-   0        0        0     2989 2023-04-14 11:51:38.000000 pyDataFitting-0.0.4/tests/test_model_tools.py
+-rw-rw-rw-   0        0        0     2367 2023-04-14 20:55:16.000000 pyDataFitting-0.0.4/tests/test_nonlinear_regresssion.py
+-rw-rw-rw-   0        0        0     3959 2023-01-17 12:23:36.000000 pyDataFitting-0.0.4/tests/test_piecewise_polynomial_fit.py
+-rw-rw-rw-   0        0        0     3387 2023-01-17 12:23:36.000000 pyDataFitting-0.0.4/tests/test_polynomial_regression.py
+-rw-rw-rw-   0        0        0     2396 2023-04-14 20:50:17.000000 pyDataFitting-0.0.4/tests/test_principal_component_regression.py
```

### Comparing `pyDataFitting-0.0.3/LICENSE` & `pyDataFitting-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.3/PKG-INFO` & `pyDataFitting-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDataFitting
-Version: 0.0.3
+Version: 0.0.4
 Summary: package for specialized regression
 Home-page: https://github.com/AlexanderSouthan/pyDataFitting
 Author: Alexander Southan
 Author-email: 72788772+AlexanderSouthan@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/AlexanderSouthan/pyDataFitting/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,14 +25,19 @@
 functions of my little_helpers repository and quite a few other, external
 packages like Numpy, Pandas, matplotlib, scikit-learn, statsmodels, Scipy.
 
 Install with:
 ```
 pip install pyDataFitting
 ```
+or download repository and run the following from repository folder to get the
+latest version that might not have made it to PyPI, yet:
+```
+pip install -e.
+```
 
 ## Linear regression (in linear_regression.py)
 * dataset_regression: Does a classical linear least squares regression. Treats
 the input data as a linear combination of the different components from
 reference data. Can be used for example to fit spectra of mixtures with spectra
 of pure components. Produces the same result like, but much faster than using
 sklearn.linear_model.LinearRegression().fit(...).
```

### Comparing `pyDataFitting-0.0.3/README.md` & `pyDataFitting-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 functions of my little_helpers repository and quite a few other, external
 packages like Numpy, Pandas, matplotlib, scikit-learn, statsmodels, Scipy.
 
 Install with:
 ```
 pip install pyDataFitting
 ```
+or download repository and run the following from repository folder to get the
+latest version that might not have made it to PyPI, yet:
+```
+pip install -e.
+```
 
 ## Linear regression (in linear_regression.py)
 * dataset_regression: Does a classical linear least squares regression. Treats
 the input data as a linear combination of the different components from
 reference data. Can be used for example to fit spectra of mixtures with spectra
 of pure components. Produces the same result like, but much faster than using
 sklearn.linear_model.LinearRegression().fit(...).
```

### Comparing `pyDataFitting-0.0.3/setup.cfg` & `pyDataFitting-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7944 6174 6146 6974 7469 6e67   = pyDataFitting
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 302e  ..version = 0.0.
-00000030: 330d 0a61 7574 686f 7220 3d20 416c 6578  3..author = Alex
+00000030: 340d 0a61 7574 686f 7220 3d20 416c 6578  4..author = Alex
 00000040: 616e 6465 7220 536f 7574 6861 6e0d 0a61  ander Southan..a
 00000050: 7574 686f 725f 656d 6169 6c20 3d20 3732  uthor_email = 72
 00000060: 3738 3837 3732 2b41 6c65 7861 6e64 6572  788772+Alexander
 00000070: 536f 7574 6861 6e40 7573 6572 732e 6e6f  Southan@users.no
 00000080: 7265 706c 792e 6769 7468 7562 2e63 6f6d  reply.github.com
 00000090: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 000000a0: 7061 636b 6167 6520 666f 7220 7370 6563  package for spec
```

### Comparing `pyDataFitting-0.0.3/src/pyDataFitting/linear_regression.py` & `pyDataFitting-0.0.4/src/pyDataFitting/linear_regression.py`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.3/src/pyDataFitting/model_diagnostics.py` & `pyDataFitting-0.0.4/src/pyDataFitting/model_diagnostics.py`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.3/src/pyDataFitting/model_tools.py` & `pyDataFitting-0.0.4/src/pyDataFitting/model_tools.py`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.3/src/pyDataFitting/multivariate_regression.py` & `pyDataFitting-0.0.4/src/pyDataFitting/principle_component_regression.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
 from matplotlib.cm import rainbow
 from mpl_toolkits.mplot3d import Axes3D
 from sklearn.decomposition import PCA
-from sklearn.cross_decomposition import PLSRegression
 from sklearn.preprocessing import StandardScaler
 from sklearn.model_selection import cross_val_predict
 from sklearn.metrics import mean_squared_error, r2_score
 import statsmodels.api as sm
+from statsmodels.formula.api import ols
 
-from little_helpers.statsmodel_wrapper import statsmodel_wrapper
+from little_helpers.statsmodel_wrapper import ols_wrapper
+from .model_tools import model_tools
 
 
 class principal_component_regression():
     """Class for performing principal component regression."""
 
     def __init__(self, x, y=None, x_names=None, y_names=None,
                  sample_names=None, scale_std=False):
@@ -118,16 +119,15 @@
             # the different PCA and PCR results
             self.sample_index = pd.Index(self.sample_names, name='Sample name')
             self.var_index = pd.Index(self.x_names, name='Variable name')
         elif isinstance(x, pd.DataFrame):
             self.sample_index = x.index
             self.var_index = x.columns
         else:
-            raise TypeError('x must either be np.ndarray or '
-                            'pd.DataFrame.')
+            raise TypeError('x must either be np.ndarray or pd.DataFrame.')
 
         y_c_index = pd.MultiIndex.from_product(
             [self.response_index, self.sample_index.values],
             names=['response name', 'sample number'])
         metrics_index = pd.MultiIndex.from_product(
             [self.response_index, ['r2_c', 'r2_cv', 'rmse_c', 'rmse_cv']],
             names=['response name', 'metrics type'])
@@ -153,22 +153,22 @@
 
         self.pca_objects = pd.Series([], dtype='object')
         self.pca_scores = pd.DataFrame([])
         self.pca_eigenvalues = pd.Series([], dtype='float64')
         self.pca_eigenvectors = pd.DataFrame([])
         self.pca_loadings = pd.DataFrame([])
         self.pca_explained_variance = pd.DataFrame([], columns=['each', 'cum'])
-        self.pca_results = pd.DataFrame([],
-                                        index=['Hotelling_T2', 'Q_residuals'])
-        self.pcr_models = pd.DataFrame([], dtype='object',
-                                       columns=self.response_index)
-        self.pcr_params = pd.DataFrame([], dtype='object',
-                                       columns=self.response_index)
-        self.pcr_used_pcs = pd.DataFrame([], dtype='object',
-                                         columns=self.response_index)
+        self.pca_results = pd.DataFrame(
+            [], index=['Hotelling_T2', 'Q_residuals'])
+        self.pcr_models = pd.DataFrame(
+            [], dtype='object', columns=self.response_index)
+        self.pcr_params = pd.DataFrame(
+            [], dtype='object', columns=self.response_index)
+        self.pcr_used_pcs = pd.DataFrame(
+            [], dtype='object', columns=self.response_index)
         self.pcr_corr_coef = pd.DataFrame([], columns=self.response_index)
         self.pcr_y_c = pd.DataFrame([], index=y_c_index)
         self.pcr_y_cv = pd.DataFrame([], index=y_c_index)
         self.pcr_metrics = pd.DataFrame([], index=metrics_index)
 
     def perform_pca(self, n_components, **kwargs):
         """
@@ -302,36 +302,41 @@
 
         reconstructed_data = pd.DataFrame(
             self.scaler.inverse_transform(reconstructed_data),
             index=self.x.index, columns=self.x.columns)
 
         return reconstructed_data
 
-    def pcr_fit(self, cv_percentage=20, mode='exp_var',
+    def pcr_fit(self, cv_percentage=20, mode='exp_var', model='linear',
                 **kwargs):
         """
         Perform principal component regression for one number of components.
 
-        One PCA object is generated for every number of components.
-        This is necessary in order to be able to use the PCA transform method
-        in self.predict. For example, the predicted sample values ('y') of the
-        training data ('c'), the corresponding predictions ('y') after
-        cross-validation ('cv'), the coefficient of determination ('r2') for
-        'c' and 'cv', and the root mean squared error ('rmse') for 'c' and 'cv'
-        are calculated.
+        The model used for the fit can be a linear or a non-linear model, as
+        supported by statsmodels ols object. One PCA object is generated for
+        every number of components. This is necessary in order to be able to
+        use the PCA transform method in self.predict. For example, the
+        predicted sample values ('y') of the training data ('c'), the
+        corresponding predictions ('y') after cross-validation ('cv'), the
+        coefficient of determination ('r2') for 'c' and 'cv', and the root mean
+        squared error ('rmse') for 'c' and 'cv' are calculated.
 
         Parameters
         ----------
         cv_percentage : float, optional
             Percentage of data used for cross-validation. The default is 20.
         mode : str, optional
             Determines if PCs used for regression are selected based on
             explained variance only ('exp_var'), only based on corellation
             with the data in self.y ('corr_coef'), or are given in a list based
             on the exlained variance order ('list'). Default is 'exp_var'.
+        model : str
+            The model used to fit the data. Can be any value allowed by
+            model_tools from pyDataFitting, such as 'linear', '2fi', '3fi',
+            'quadratic'.
         **kwargs :
             All **kwargs from sklearn.decomposition.PCA are allowed, see the
             documentation of that class for details.
         **kwargs if mode=='exp_var':
             n_components : int
                 The number of principal components used for the regression.
         **kwargs if mode=='corr_coef':
@@ -391,15 +396,15 @@
                              iterated_power=iterated_power,
                              random_state=random_state)
 
         # In each iteration in the following for loop, a multilinear regression
         # with the scores and only one of the responses given is performed. So
         # the loop iterates over the individual responses. This results in
         # one call of the fit and predict methods from the linear model objects
-        # per iteration. This is necessary for mode=='coord_coef' because for
+        # per iteration. This is necessary for mode=='corr_coef' because for
         # each response, different components may be used for regression.
         for curr_y in self.y_names:
             for curr_index, curr_scores in enumerate(
                     self.pca_scores.values.T):
                 self.pcr_corr_coef.at[curr_index+1, curr_y] = np.abs(
                     np.corrcoef(
                         curr_scores, self.y[curr_y])[0, 1])
@@ -413,32 +418,33 @@
                 self.pcr_used_pcs.at[n_components, curr_y] = np.flip(
                     np.argsort(self.pcr_corr_coef.loc[:, curr_y].values)[
                         -n_components:])+1
             elif mode == 'list':
                 self.pcr_used_pcs.at[n_components, curr_y] = np.array(pc_list)
 
             fit_scores = self.pca_scores.loc[
-                :, self.pcr_used_pcs.at[n_components, curr_y]].values
+                :, self.pcr_used_pcs.at[n_components, curr_y]]
 
-            # Build linear model
-            fit_scores = sm.add_constant(fit_scores)
-            self.pcr_models.at[n_components, curr_y] = sm.OLS(
-                self.y[curr_y], fit_scores)
+            # Build regression model, either linear or non-linear
+            param_names = ['PC' + str(nbr) for nbr in fit_scores.columns]
+            model_t = model_tools(model, param_names, response_name=curr_y)
+            fit_scores.columns = param_names
+            fit_scores[curr_y] = self.y[curr_y]
+            self.pcr_models.at[n_components, curr_y] = ols(
+                model_t.model_string(), fit_scores)
             self.pcr_params.at[n_components, curr_y] = (
                 self.pcr_models.at[n_components, curr_y].fit())
             # Predict sample values according to PCR model
             idx = pd.IndexSlice
             self.pcr_y_c.loc[idx[curr_y, :], n_components] = (
-                self.pcr_models.at[n_components, curr_y].predict(
-                    self.pcr_params.at[n_components, curr_y].params,
-                    fit_scores))
+                self.pcr_params.at[n_components, curr_y].predict())
             # Cross-validate the PCR model
             self.pcr_y_cv.loc[idx[curr_y, :], n_components] = (
-                cross_val_predict(statsmodel_wrapper(sm.OLS),
-                                  fit_scores, self.y[curr_y],
+                cross_val_predict(ols_wrapper(model_t.model_string(), curr_y),
+                                  fit_scores.iloc[:, :-1], self.y[curr_y],
                                   cv=round(100/cv_percentage)))
             # Calculate metrics for PCR model
             self.pcr_metrics.at[(curr_y, 'r2_c'), n_components] = r2_score(
                 self.y[curr_y], self.pcr_y_c.loc[
                     idx[curr_y, :], n_components], multioutput='raw_values')
             self.pcr_metrics.at[(curr_y, 'r2_cv'), n_components] = r2_score(
                 self.y[curr_y], self.pcr_y_cv.loc[
@@ -451,15 +457,15 @@
             self.pcr_metrics.at[(curr_y, 'rmse_cv'), n_components] = (
                 mean_squared_error(self.y[curr_y],
                                    self.pcr_y_cv.loc[idx[curr_y, :],
                                                      n_components],
                                    multioutput='raw_values', squared=False))
 
     def pcr_sweep(self, sweep_components=20, cv_percentage=20, mode='exp_var',
-                  **kwargs):
+                  model='linear', **kwargs):
         """
         Perform PCR for all number of components between 1 and n_components.
 
         Parameters
         ----------
         sweep_components : int, optional
             The upper limit of components used for PCR. The default is 20.
@@ -483,24 +489,24 @@
         """
         assert mode in ['exp_var', 'corr_coef'], (
             'No valid option for mode given. Remember that \'list\' is not '
             'allowed for this method because in this case information about '
             'the PCs used must already be known.')
 
         for ii in reversed(range(1, sweep_components+1)):
-            self.pcr_fit(cv_percentage=cv_percentage, mode=mode,
+            self.pcr_fit(cv_percentage=cv_percentage, mode=mode, model=model,
                          n_components=ii, **kwargs)
         # return self.pcr_results
 
     def predict(self, samples, n_components, sample_names=None):
         """
         Predict unknown sample target values.
 
         Currently works correct only for mode=='exp_var'. For
-        mode=='corr_coef', the tranformation has to be implemented independent
+        mode=='corr_coef', the transformation has to be implemented independent
         of the PCA object method.
 
         Parameters
         ----------
         samples : ndarray
             Sample data in the shape (n_samples, n_variables).
         n_components : int
@@ -973,268 +979,7 @@
             ax2.xaxis.set_label_position('top')
             ax2.set_xlabel('PC{} scores'.format(pc_numbers[0]))
             ax2.set_ylabel('PC{} scores'.format(pc_numbers[1]))
             ax2.set_zlabel('PC{} scores'.format(pc_numbers[2]))
             ax2.patch.set_alpha(0)
 
         return plots
-
-
-class pls_regression():
-    """Class for performing principal component regression."""
-
-    def __init__(self, x, y, scale_std=False):
-        """
-        Store input data and initialize results DataFrame.
-
-        Parameters
-        ----------
-        x : ndarray
-            Sample training data in the shape (n_samples, n_variables).
-        y : ndarray
-            Target values in the shape (n_samples,) for a single target or
-            (n_samples, n_targets) for multiple targets.
-
-        Returns
-        -------
-        None.
-
-        """
-        self.x_raw = x
-        self.y = y
-        self.scale_std = scale_std
-
-        self.scaler = StandardScaler(with_std=self.scale_std)
-        self.x = self.scaler.fit_transform(self.x_raw)
-
-        results_index = pd.MultiIndex.from_product(
-            [['plsr_objects', 'y', 'r2', 'mse', 'Hotelling_T2'], ['c', 'cv']],
-            names=['result_name', 'cal_or_crossval'])
-        results_columns = pd.Index(
-            [], name='n_components')
-        self.plsr_results = pd.DataFrame([], index=results_index,
-                                         columns=results_columns, dtype='object')
-
-    def plsr_fit(self, n_components, cv_percentage=10, **kwargs):
-        """
-        Perform partial least squares regression for one number of components.
-
-        Currently, one PLSR object is generated for every number of components.
-        I do not know if this is necessary, might be checked in the future.
-
-        Parameters
-        ----------
-        n_components : int
-            Number of components kept after PLSR.
-        cv_percentage : float, optional
-            Percentage of data used for cross-validation. The default is 10.
-        **kwargs :
-            All **kwargs from sklearn.cross_decomposition.PLSRegression are
-            allowed, see the documentation of those classes for details.
-
-        Returns
-        -------
-        DataFrame
-            Contains the predicted sample values ('y') of the training data
-            ('c'), the corresponding predictions ('y') after cross-validation
-            ('cv'), the coefficient of determination ('r2') for 'c' and 'cv',
-            and the mean squared error ('mse') for 'c' and 'cv' (given in the
-            DataFrame index). The DataFrame columns give the number of
-            components used to calculate the values.
-
-        """
-        # Create PLSR models
-        self.plsr_results.at[('plsr_objects', 'c'), n_components] = PLSRegression(
-            n_components=n_components, **kwargs)
-        self.plsr_results.at[('plsr_objects', 'c'), n_components].fit_transform(self.x, y=self.y)
-        # Predict sample values according to PLSR model
-        self.plsr_results.at[('y', 'c'), n_components] = self.predict(
-            self.x, n_components, scale=False)
-        # Cross-validate the PCR model
-        self.plsr_results.at[('y', 'cv'), n_components] = np.squeeze(
-            cross_val_predict(
-                self.plsr_results.at[('plsr_objects', 'c'), n_components], self.x, self.y,
-                cv=round(100/cv_percentage)))
-
-        # Calculate metrics for PLSR model
-        self.plsr_results.at[('r2', 'c'), n_components] = r2_score(
-            self.y, self.plsr_results.at[('y', 'c'), n_components],
-            multioutput='raw_values')
-        self.plsr_results.at[('r2', 'cv'), n_components] = r2_score(
-            self.y, self.plsr_results.at[('y', 'cv'), n_components],
-            multioutput='raw_values')
-        self.plsr_results.at[('mse', 'c'), n_components] = mean_squared_error(
-            self.y, self.plsr_results.at[('y', 'c'), n_components],
-            multioutput='raw_values')
-        self.plsr_results.at[('mse', 'cv'), n_components] = mean_squared_error(
-            self.y, self.plsr_results.at[('y', 'cv'), n_components],
-            multioutput='raw_values')
-
-        return self.plsr_results
-
-    def plsr_sweep(self, max_components=20, **kwargs):
-        """
-        Perform PLSR for all number of components between 1 and max_components.
-
-        Parameters
-        ----------
-        max_components : int, optional
-            The upper limit of components used for PLSR. The default is 20.
-        **kwargs :
-            The same **kwargs as in self.plsr_fit.
-
-        Returns
-        -------
-        DataFrame
-            See Docstring of self.plsr_fit.
-
-        """
-        for ii in range(1, max_components+1):
-            self.plsr_fit(ii, **kwargs)
-        return self.plsr_results
-
-    def predict(self, samples, n_components, scale=True):
-        """
-        Predict unknown sample target values.
-
-        Parameters
-        ----------
-        samples : ndarray
-            Sample data in the shape (n_samples, n_variables).
-        n_components : int
-            Number of components used in the PLSR model for the prediction.
-        scale : bool, optional
-            Defines if the sample data is scaled like the input data or not.
-            If called from within the class, should be False. Default is True.
-
-        Returns
-        -------
-        prediction : ndarray
-            Predicted target values in the shape (n_samples,) for a single
-            target or (n_samples, n_targets) for multiple targets.
-
-        """
-        if scale:
-            samples = self.scaler.transform(samples)
-
-        return np.squeeze(
-            self.plsr_results.at[('plsr_objects', 'c'), n_components].predict(samples))
-
-    def generate_plots(self, plot_names, response_number=0, **kwargs):
-        """
-        Generate some basic plots of partial least squares regression results.
-
-        Parameters
-        ----------
-        plot_names : list of str
-            List of plots to be generated. Allowed entries are
-            'actual_vs_pred' (actual target values vs. predicted values),
-            'r2_vs_comp' (coefficient of determination vs. number of
-            components), 'mse_vs_comp' (mean squared error vs. number of
-            components).
-        response_number : int, optional
-            Defines the index of the response from self.y to be plotted. 
-            Default is 0.
-        **kwargs :
-            n_components : int
-                Needed for plot_name 'actual_vs_pred'.
-            cv : boolean
-                State if cross-validation data should be plotted, too.
-                Default is False.
-        Returns
-        -------
-        plots : matplotlib plots
-            Plot objects, I do not know if anything can be done with this.
-
-        """
-        plots = []
-        plot_cv_data = kwargs.get('cv', False)
-        if 'actual_vs_pred' in plot_names:
-            n_components = kwargs.get('n_components')
-
-            if len(self.y.shape) == 1:
-                curr_y = self.y
-            else:
-                curr_y = self.y[:, response_number]
-                
-            if len(self.plsr_results.at[('y', 'c'), n_components].shape) == 1:
-                curr_c = self.plsr_results.at[('y', 'c'), n_components]
-            else:
-                curr_c = self.plsr_results.at[('y', 'c'), n_components][
-                    :, response_number]
-                
-            if len(self.plsr_results.at[('y', 'cv'), n_components].shape) == 1:
-                curr_cv = self.plsr_results.at[('y', 'cv'), n_components]
-            else:
-                curr_cv = self.plsr_results.at[('y', 'cv'), n_components][
-                    :, response_number]
-
-            z_c = np.polyfit(
-                curr_y, curr_c, 1)
-            z_cv = np.polyfit(
-                curr_y, curr_cv, 1)
-            with plt.style.context(('ggplot')):
-                fig1, ax1 = plt.subplots(figsize=(9, 5))
-                ax1.scatter(curr_y, curr_c, c='red', edgecolors='k')
-                if plot_cv_data:
-                    ax1.scatter(curr_y, curr_cv, c='blue', edgecolors='k')
-                    ax1.plot(curr_y, z_cv[1]+z_cv[0]*curr_y, c='blue',
-                             linewidth=1)
-                ax1.plot(curr_y, z_c[1]+z_c[0]*curr_y, c='red', linewidth=1)
-                ax1.plot(curr_y, curr_y, color='green', linewidth=1)
-                plt.title('$R^{2}$ (CV): '+str(
-                    self.plsr_results.loc[('r2', 'cv'), n_components]))
-                plt.xlabel('Measured')
-                plt.ylabel('Predicted')
-            plots.append(fig1)
-        if 'r2_vs_comp' in plot_names:
-            if len(self.plsr_results.loc['r2', 'c'][1]) == 1:
-                curr_c_r2 = self.plsr_results.loc['r2', 'c']
-            else:
-                curr_c_r2 = pd.DataFrame(
-                    self.plsr_results.loc['r2', 'c'].tolist()
-                    ).iloc[:, response_number]
-
-            if len(self.plsr_results.loc['r2', 'cv'][1]) == 1:
-                curr_cv_r2 = self.plsr_results.loc['r2', 'cv']
-            else:
-                curr_cv_r2 = pd.DataFrame(
-                    self.plsr_results.loc['r2', 'cv'].tolist()
-                    ).iloc[:, response_number]
-
-            with plt.style.context(('ggplot')):
-                fig2, ax2 = plt.subplots(figsize=(9, 5))
-                ax2.plot(
-                    curr_c_r2, linestyle='--', marker='o')
-                if plot_cv_data:
-                    ax2.plot(
-                        curr_cv_r2, linestyle='--', marker='o')
-                plt.ylabel('$R^{2}$')
-                plt.xlabel('Number of components')
-            plots.append(fig2)
-        if 'mse_vs_comp' in plot_names:
-            if len(self.plsr_results.loc['mse', 'c'][1]) == 1:
-                curr_c_mse = self.plsr_results.loc['mse', 'c']
-            else:
-                curr_c_mse = pd.DataFrame(
-                    self.plsr_results.loc['mse', 'c'].tolist()
-                    ).iloc[:, response_number]
-
-            if len(self.plsr_results.loc['mse', 'cv'][1]) == 1:
-                curr_cv_mse = self.plsr_results.loc['mse', 'cv']
-            else:
-                curr_cv_mse = pd.DataFrame(
-                    self.plsr_results.loc['mse', 'cv'].tolist()
-                    ).iloc[:, response_number]
-            
-            with plt.style.context(('ggplot')):
-                fig3, ax3 = plt.subplots(figsize=(9, 5))
-                ax3.plot(
-                    curr_c_mse, linestyle='--', marker='o')
-                if plot_cv_data:
-                    ax3.plot(
-                        curr_cv_mse, linestyle='--', marker='o')
-                plt.ylabel('MSE')
-                plt.xlabel('Number of components')
-            plots.append(fig3)
-
-        return plots
```

### Comparing `pyDataFitting-0.0.3/src/pyDataFitting/nonlinear_regression.py` & `pyDataFitting-0.0.4/src/pyDataFitting/nonlinear_regression.py`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.3/src/pyDataFitting/polynomial_regression.py` & `pyDataFitting-0.0.4/src/pyDataFitting/polynomial_regression.py`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.3/src/pyDataFitting.egg-info/PKG-INFO` & `pyDataFitting-0.0.4/src/pyDataFitting.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDataFitting
-Version: 0.0.3
+Version: 0.0.4
 Summary: package for specialized regression
 Home-page: https://github.com/AlexanderSouthan/pyDataFitting
 Author: Alexander Southan
 Author-email: 72788772+AlexanderSouthan@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/AlexanderSouthan/pyDataFitting/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,14 +25,19 @@
 functions of my little_helpers repository and quite a few other, external
 packages like Numpy, Pandas, matplotlib, scikit-learn, statsmodels, Scipy.
 
 Install with:
 ```
 pip install pyDataFitting
 ```
+or download repository and run the following from repository folder to get the
+latest version that might not have made it to PyPI, yet:
+```
+pip install -e.
+```
 
 ## Linear regression (in linear_regression.py)
 * dataset_regression: Does a classical linear least squares regression. Treats
 the input data as a linear combination of the different components from
 reference data. Can be used for example to fit spectra of mixtures with spectra
 of pure components. Produces the same result like, but much faster than using
 sklearn.linear_model.LinearRegression().fit(...).
```

### Comparing `pyDataFitting-0.0.3/src/pyDataFitting.egg-info/SOURCES.txt` & `pyDataFitting-0.0.4/src/pyDataFitting.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 pyproject.toml
 setup.cfg
 setup.py
 src/pyDataFitting/__init__.py
 src/pyDataFitting/linear_regression.py
 src/pyDataFitting/model_diagnostics.py
 src/pyDataFitting/model_tools.py
-src/pyDataFitting/multivariate_regression.py
 src/pyDataFitting/nonlinear_regression.py
+src/pyDataFitting/partial_least_squares_regression.py
 src/pyDataFitting/polynomial_regression.py
+src/pyDataFitting/principle_component_regression.py
 src/pyDataFitting.egg-info/PKG-INFO
 src/pyDataFitting.egg-info/SOURCES.txt
 src/pyDataFitting.egg-info/dependency_links.txt
 src/pyDataFitting.egg-info/requires.txt
 src/pyDataFitting.egg-info/top_level.txt
 tests/test_model_tools.py
 tests/test_nonlinear_regresssion.py
```

### Comparing `pyDataFitting-0.0.3/tests/test_model_tools.py` & `pyDataFitting-0.0.4/tests/test_model_tools.py`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.3/tests/test_nonlinear_regresssion.py` & `pyDataFitting-0.0.4/tests/test_nonlinear_regresssion.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,16 +42,16 @@
             {'m': [-100, 100], 'b': [-100, 100]},
             self.polynomial, x, y, alg='dual_annealing')
 
         self.assertAlmostEqual(evo_fit.params['b'], 10, 5)
         self.assertAlmostEqual(evo_fit.params['m'], 5, 5)
         self.assertAlmostEqual(lm_fit.params['b'], 10, 5)
         self.assertAlmostEqual(lm_fit.params['m'], 5, 5)
-        self.assertAlmostEqual(basinhopping_fit.params['b'], 10, 5)
-        self.assertAlmostEqual(basinhopping_fit.params['m'], 5, 5)
+        self.assertAlmostEqual(basinhopping_fit.params['b'], 10, 3)
+        self.assertAlmostEqual(basinhopping_fit.params['m'], 5, 3)
         # self.assertAlmostEqual(brute_fit.params['b'], 10, 4)
         # self.assertAlmostEqual(brute_fit.params['m'], 5, 4)
         # self.assertAlmostEqual(shgo_fit.params['b'], 10, 5)
         # self.assertAlmostEqual(shgo_fit.params['m'], 5, 5)
         self.assertAlmostEqual(dualannealing_fit.params['b'], 10, 5)
         self.assertAlmostEqual(dualannealing_fit.params['m'], 5, 5)
```

### Comparing `pyDataFitting-0.0.3/tests/test_piecewise_polynomial_fit.py` & `pyDataFitting-0.0.4/tests/test_piecewise_polynomial_fit.py`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.3/tests/test_polynomial_regression.py` & `pyDataFitting-0.0.4/tests/test_polynomial_regression.py`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.3/tests/test_principal_component_regression.py` & `pyDataFitting-0.0.4/tests/test_principal_component_regression.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 @author: Alexander Southan
 """
 
 import numpy as np
 import unittest
 
-from src.pyDataFitting import multivariate_regression
+from src.pyDataFitting import principal_component_regression
 from little_helpers.math_functions import gaussian
 
 
 class TestPrincipalComponentRegression(unittest.TestCase):
 
     def test_pcr(self):
 
@@ -44,15 +44,15 @@
 
         # The spectra of the mixtures are calculated.
         mixtures = np.empty((len(mix_coeffs), len(wavelengths)))
         for idx, curr_coeffs in enumerate(mix_coeffs):
             mixtures[idx] = (components.T*curr_coeffs).sum(axis=1)
 
         # A principal component regression is performed
-        pcr = multivariate_regression.principal_component_regression(
+        pcr = principal_component_regression(
             mixtures, y=mix_coeffs,
             x_names=np.round(wavelengths, 2).astype('str'),
             y_names=['Comp_{}'.format(idx)
                      for idx in range(mix_coeffs.shape[1])])
         pcr.pcr_fit(n_components=3)
 
         # The mixing coefficients should be found again by using the predict
```

