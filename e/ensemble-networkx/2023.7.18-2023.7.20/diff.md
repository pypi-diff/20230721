# Comparing `tmp/ensemble_networkx-2023.7.18.tar.gz` & `tmp/ensemble_networkx-2023.7.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensemble_networkx-2023.7.18.tar", last modified: Tue Jul 18 19:15:29 2023, max compression
+gzip compressed data, was "ensemble_networkx-2023.7.20.tar", last modified: Thu Jul 20 23:51:19 2023, max compression
```

## Comparing `ensemble_networkx-2023.7.18.tar` & `ensemble_networkx-2023.7.20.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-07-18 19:15:29.468668 ensemble_networkx-2023.7.18/
--rw-------   0 jespinoz  (3456) staff       (20)     1563 2023-07-18 19:13:30.000000 ensemble_networkx-2023.7.18/LICENSE
--rw-r--r--   0 jespinoz  (3456) staff       (20)      281 2023-07-18 19:15:29.468349 ensemble_networkx-2023.7.18/PKG-INFO
--rw-------   0 jespinoz  (3456) staff       (20)    12928 2023-07-18 19:15:16.000000 ensemble_networkx-2023.7.18/README.md
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-07-18 19:15:29.465787 ensemble_networkx-2023.7.18/ensemble_networkx/
--rw-------   0 jespinoz  (3456) staff       (20)     2986 2023-07-18 18:45:57.000000 ensemble_networkx-2023.7.18/ensemble_networkx/__init__.py
--rw-------   0 jespinoz  (3456) staff       (20)   117136 2023-07-18 19:11:44.000000 ensemble_networkx-2023.7.18/ensemble_networkx/ensemble_networkx.py
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-07-18 19:15:29.467862 ensemble_networkx-2023.7.18/ensemble_networkx.egg-info/
--rw-------   0 jespinoz  (3456) staff       (20)      281 2023-07-18 19:15:29.000000 ensemble_networkx-2023.7.18/ensemble_networkx.egg-info/PKG-INFO
--rw-------   0 jespinoz  (3456) staff       (20)      299 2023-07-18 19:15:29.000000 ensemble_networkx-2023.7.18/ensemble_networkx.egg-info/SOURCES.txt
--rw-------   0 jespinoz  (3456) staff       (20)        1 2023-07-18 19:15:29.000000 ensemble_networkx-2023.7.18/ensemble_networkx.egg-info/dependency_links.txt
--rw-------   0 jespinoz  (3456) staff       (20)      116 2023-07-18 19:15:29.000000 ensemble_networkx-2023.7.18/ensemble_networkx.egg-info/requires.txt
--rw-------   0 jespinoz  (3456) staff       (20)       18 2023-07-18 19:15:29.000000 ensemble_networkx-2023.7.18/ensemble_networkx.egg-info/top_level.txt
--rw-r--r--   0 jespinoz  (3456) staff       (20)       38 2023-07-18 19:15:29.468798 ensemble_networkx-2023.7.18/setup.cfg
--rw-------   0 jespinoz  (3456) staff       (20)      886 2022-02-09 21:02:44.000000 ensemble_networkx-2023.7.18/setup.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-07-20 23:51:19.596314 ensemble_networkx-2023.7.20/
+-rw-r--r--   0 jespinoz  (3456) staff       (20)     1563 2023-07-20 23:44:01.000000 ensemble_networkx-2023.7.20/LICENSE
+-rw-r--r--   0 jespinoz  (3456) staff       (20)      253 2023-07-20 23:51:19.595895 ensemble_networkx-2023.7.20/PKG-INFO
+-rw-r--r--   0 jespinoz  (3456) staff       (20)    14514 2023-07-20 23:44:01.000000 ensemble_networkx-2023.7.20/README.md
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-07-20 23:51:19.592320 ensemble_networkx-2023.7.20/ensemble_networkx/
+-rw-r--r--   0 jespinoz  (3456) staff       (20)      990 2023-07-20 23:44:03.000000 ensemble_networkx-2023.7.20/ensemble_networkx/__init__.py
+-rw-r--r--   0 jespinoz  (3456) staff       (20)   119235 2023-07-20 23:44:03.000000 ensemble_networkx-2023.7.20/ensemble_networkx/ensemble_networkx.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-07-20 23:51:19.595283 ensemble_networkx-2023.7.20/ensemble_networkx.egg-info/
+-rw-------   0 jespinoz  (3456) staff       (20)      253 2023-07-20 23:51:19.000000 ensemble_networkx-2023.7.20/ensemble_networkx.egg-info/PKG-INFO
+-rw-------   0 jespinoz  (3456) staff       (20)      299 2023-07-20 23:51:19.000000 ensemble_networkx-2023.7.20/ensemble_networkx.egg-info/SOURCES.txt
+-rw-------   0 jespinoz  (3456) staff       (20)        1 2023-07-20 23:51:19.000000 ensemble_networkx-2023.7.20/ensemble_networkx.egg-info/dependency_links.txt
+-rw-------   0 jespinoz  (3456) staff       (20)      115 2023-07-20 23:51:19.000000 ensemble_networkx-2023.7.20/ensemble_networkx.egg-info/requires.txt
+-rw-------   0 jespinoz  (3456) staff       (20)       18 2023-07-20 23:51:19.000000 ensemble_networkx-2023.7.20/ensemble_networkx.egg-info/top_level.txt
+-rw-r--r--   0 jespinoz  (3456) staff       (20)       38 2023-07-20 23:51:19.596456 ensemble_networkx-2023.7.20/setup.cfg
+-rw-r--r--   0 jespinoz  (3456) staff       (20)      885 2023-07-20 23:44:01.000000 ensemble_networkx-2023.7.20/setup.py
```

### Comparing `ensemble_networkx-2023.7.18/LICENSE` & `ensemble_networkx-2023.7.20/LICENSE`

 * *Files identical despite different names*

### Comparing `ensemble_networkx-2023.7.18/README.md` & `ensemble_networkx-2023.7.20/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 ### Ensemble NetworkX
 High-level [Ensemble](https://en.wikipedia.org/wiki/Ensemble_averaging_(machine_learning)) Network implementations in Python.  Built on top of [NetworkX](https://github.com/networkx/networkx) and [Pandas](https://pandas.pydata.org/).  
 
 #### Dependencies:
 Compatible for Python 3.
 
-    pandas >= 1
+    panda
     numpy
-    scipy >= 1
-    networkx >= 2
-    matplotlib >= 3
-    soothsayer_utils >= 2021.03.08
-    compositional >= 2020.05.19
+    scipy
+    networkx
+    matplotlib
+    soothsayer_utils
+    compositional
     
 #### Citations (Debut):
    
 
 
    * Nabwera HM+, Espinoza JL+, Worwui A, Betts M, Okoi C, Sesay AK, Bancroft R, Agbla SC, Jarju S, Bradbury RS, Colley M, Jallow AT, Liu J, Houpt ER, Prentice AM, Antonio M, Bernstein RM, Dupont CL+, Kwambana-Adams BA+. *Interactions between fecal gut microbiome, enteric pathogens, and energy regulating hormones among acutely malnourished rural Gambian children*. EBioMedicine. 2021 Oct 22;73:103644. [doi: 10.1016/j.ebiom.2021.103644](https://doi.org/10.1016/j.ebiom.2021.103644). PMID: 34695658.
 
@@ -92,15 +92,54 @@
 # (sepal_length, petal_length)  0.880692  0.000268 -0.107437  0.235619   
 # (petal_width, sepal_length)   0.834140  0.000442 -0.275487 -0.219778   
 # (sepal_width, petal_length)  -0.304403  0.003472 -0.363377  0.059179   
 # (sepal_width, petal_width)   -0.285237  0.003466 -0.606118  0.264103 
 
 ```
 
-##### Simple case of creating sample-specific perturbation networks
+##### Simple case of an ensemble network for binary data using Mathew's Correlation Coefficient (MCC)
+
+```
+# Create ensemble network using MCC for binary data
+n,m = 1000, 100
+X_binary = pd.DataFrame(
+    data=np.random.RandomState(0).choice([0,1], size=(n,m)),
+    index=map(lambda i: f"sample_{i}", range(n)),
+    columns=map(lambda j:f"feature_{j}", range(m)),
+)
+ens_binary = enx.EnsembleAssociationNetwork(name="Binary", edge_type="association")
+ens_binary.fit(X=X_binary, metric="mcc",  n_iter=100, stats_summary=[np.mean,np.var], copy_ensemble=True)
+print(ens_binary)
+
+# ====================================================
+# EnsembleAssociationNetwork(Name:Binary, Metric: mcc)
+# ====================================================
+#     * Number of nodes (None): 100
+#     * Number of edges (association): 4950
+#     * Observation type: None
+#     ------------------------------------------------
+#     | Parameters
+#     ------------------------------------------------
+#     * n_iter: 100
+#     * sampling_size: 618
+#     * random_state: 0
+#     * with_replacement: False
+#     * transformation: None
+#     * memory: 4.894 MB
+#     ------------------------------------------------
+#     | Data
+#     ------------------------------------------------
+#     * Features (n=1000, m=100, memory=821.352 KB)
+#     * Ensemble (memory=3.777 MB)
+#     * Statistics (['mean', 'var', 'normaltest|stat', 'normaltest|p_value'], memory=322.398 KB)
+```
+
+##### Simple case of creating sample-specific perturbation networks for compositional data using [Rho Proportionality](https://pubmed.ncbi.nlm.nih.gov/26762323/)
+
+Iris data isn't compositional but this is for demonstration since they are positive values.
 
 
 ```python
 # Create ensemble network
 sspn_rho = enx.SampleSpecificPerturbationNetwork(name="Iris", node_type="leaf measurement", edge_type="association", observation_type="specimen")
 sspn_rho.fit(X=X, y=y, metric="rho", reference="setosa", n_iter=100, stats_summary=[np.mean,np.var], copy_ensemble=True)
```

### Comparing `ensemble_networkx-2023.7.18/ensemble_networkx/ensemble_networkx.py` & `ensemble_networkx-2023.7.20/ensemble_networkx/ensemble_networkx.py`

 * *Files 1% similar despite different names*

```diff
@@ -767,14 +767,71 @@
 
     # Add labels
     if labels is not None:
         result = pd.DataFrame(result, index=labels, columns=labels)
 
     return result
 
+# Matthews correlation coefficient
+def pairwise_mcc(X:pd.DataFrame, checks=True):
+    """
+    # Description
+    Returns a correlation table containing Matthews correlation coefficients for a given matrix (np.array or pd.dataframe) of binary, categorical variables.
+    This implementation was created as an alternative to Scikit-Learn's implementation as a measure of dependency reduction.
+
+    # Scikit-Learn implementation of MCC:
+    https://scikit-learn.org/stable/modules/generated/sklearn.metrics.matthews_corrcoef.html
+    
+    # Parameters
+        * X:
+            - NumPy array or Pandas dataframe
+    Output: 
+        pd.DataFrame or np.array of pairwise MCC values
+    """
+    # Checks
+    if checks:
+        n_dimensions = len(X.shape)
+        assert n_dimensions in {2}, "`X` must be 2D"
+        assert np.all(X == X.astype(bool)), "`X` must be either dtype boolean or integers[0,1]"
+
+    # Convert input data to a NumPy array
+    # index=None
+    components=None
+    if isinstance(X, pd.DataFrame):
+        # index = X.index
+        features = X.columns
+        X = X.values
+        
+    X = X.astype(bool)
+    
+    # Shape of matrix
+    n,m = X.shape
+
+    # Calculate pairwise MCC values
+    N11 = (X[:, None] & X[:, :, None]).sum(axis=0)
+    N10 = (X[:, None] & ~X[:, :, None]).sum(axis=0)
+    N01 = (~X[:, None] & X[:, :, None]).sum(axis=0)
+    N00 = (~X[:, None] & ~X[:, :, None]).sum(axis=0)
+    denominator = np.sqrt((N11 + N10) * (N11 + N01) * (N00 + N10) * (N00 + N01))
+    denominator[denominator == 0] = 1  # Handle division by zero case
+
+    output = (N11 * N00 - N10 * N01) / denominator
+
+    # Fill the lower triangular part with the symmetric values
+    output[np.tril_indices(m, k=-1)] = output.T[np.tril_indices(m, k=-1)]
+
+    # Set diagonal elements to 1.0
+    np.fill_diagonal(output, 1.0)
+
+    # Return the result as a DataFrame if the input was a DataFrame
+    if features is not None:
+        output = pd.DataFrame(output, index=features, columns=features)
+        
+    return output
+
 # =======================================================
 # Classes
 # =======================================================
 # Symmetrical dataframes represented as augment pd.Series
 class Symmetric(object):
     """
     An indexable symmetric matrix stored as the lower triangle for space.
@@ -1638,24 +1695,26 @@
         metric_name = None
         if hasattr(metric, "__call__"):
             if not function_is_pairwise:
                 function = metric
                 metric_name = function.__name__
                 metric = lambda X: self._pandas_association(X=X, metric=function)
 
-        acceptable_metrics = {"rho", "phi", "biweight_midcorrelation", "spearman", "pearson", "kendall"}
+        acceptable_metrics = {"rho", "phi", "biweight_midcorrelation", "spearman", "pearson", "kendall","mcc"}
         if isinstance(metric, str):
             assert_acceptable_arguments(metric, acceptable_metrics)
             metric_name = metric
             if metric == "rho":
                 metric = pairwise_rho
             if metric == "phi":
                 metric = pairwise_phi
             if metric == "biweight_midcorrelation":
                 metric = pairwise_biweight_midcorrelation
+            if metric == "mcc":
+                metric = pairwise_mcc
             if metric in {"spearman", "pearson", "kendall"}:
                 association = metric
                 metric = lambda X: self._pandas_association(X=X, metric=association)
                 # def metric(X, metric):
                 #     return self._pandas_association(X=X, metric=association)
 
                 
@@ -1754,16 +1813,15 @@
             stats_summary = []
         if hasattr(stats_summary, "__call__"):
             stats_summary = [stats_summary]
         stats_summary = list(stats_summary)
             
         for func in (stats_tests + stats_summary):
             assert hasattr(func, "__name__")
-        
-
+            
         # Associations
         ensemble = np.empty((n_iter, number_of_edges))
         ensemble[:] = np.nan
         for i, index in pv(enumerate(draws), description="Computing associations ({})".format(self.name), total=n_iter, unit=" draws"):
             # Compute associations with current draw
             df_associations = metric(X.loc[index])
```

### Comparing `ensemble_networkx-2023.7.18/setup.py` & `ensemble_networkx-2023.7.20/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,10 +22,10 @@
         "pandas >= 1",
         "numpy >= 1.16",
         'scipy >= 1',
         "networkx >= 2",
         "igraph",
         "xarray >= 0.15",
         "soothsayer_utils >= 2022.2.9",
-        "compositional >= 2020.12.16",
+        "compositional >= 2023.7.20",
       ],
 )
```

