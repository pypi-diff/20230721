# Comparing `tmp/mapclassify-2.5.0rc3.tar.gz` & `tmp/mapclassify-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapclassify-2.5.0rc3.tar", last modified: Sat Jan 14 04:05:37 2023, max compression
+gzip compressed data, was "mapclassify-2.6.0.tar", last modified: Fri Jul 21 20:35:33 2023, max compression
```

## Comparing `mapclassify-2.5.0rc3.tar` & `mapclassify-2.6.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:05:37.318543 mapclassify-2.5.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-01-14 04:05:37.318543 mapclassify-2.5.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:05:37.318543 mapclassify-2.5.0rc3/mapclassify/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/mapclassify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/mapclassify/_classify_API.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-01-14 04:05:37.318543 mapclassify-2.5.0rc3/mapclassify/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    78580 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/mapclassify/classifiers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:05:37.314543 mapclassify-2.5.0rc3/mapclassify/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/mapclassify/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:05:37.318543 mapclassify-2.5.0rc3/mapclassify/datasets/calemp/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/mapclassify/datasets/calemp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/mapclassify/datasets/calemp/calempdensity.csv
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/mapclassify/datasets/calemp/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/mapclassify/greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/mapclassify/pooling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:05:37.318543 mapclassify-2.5.0rc3/mapclassify/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/mapclassify/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/mapclassify/tests/test_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/mapclassify/tests/test_greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19896 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/mapclassify/tests/test_mapclassify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:05:37.314543 mapclassify-2.5.0rc3/mapclassify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-01-14 04:05:37.000000 mapclassify-2.5.0rc3/mapclassify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-01-14 04:05:37.000000 mapclassify-2.5.0rc3/mapclassify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-14 04:05:37.000000 mapclassify-2.5.0rc3/mapclassify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-14 04:05:37.000000 mapclassify-2.5.0rc3/mapclassify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-14 04:05:37.000000 mapclassify-2.5.0rc3/mapclassify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-14 04:05:37.000000 mapclassify-2.5.0rc3/mapclassify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/requirements_speedups.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/requirements_tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-01-14 04:05:37.318543 mapclassify-2.5.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-01-14 04:05:06.000000 mapclassify-2.5.0rc3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:35:33.465117 mapclassify-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-07-21 20:34:51.000000 mapclassify-2.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-21 20:34:51.000000 mapclassify-2.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-21 20:34:51.000000 mapclassify-2.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-07-21 20:35:33.465117 mapclassify-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-07-21 20:34:51.000000 mapclassify-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:35:33.465117 mapclassify-2.6.0/mapclassify/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-21 20:34:51.000000 mapclassify-2.6.0/mapclassify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-21 20:34:51.000000 mapclassify-2.6.0/mapclassify/_classify_API.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-21 20:35:33.465117 mapclassify-2.6.0/mapclassify/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81361 2023-07-21 20:34:51.000000 mapclassify-2.6.0/mapclassify/classifiers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:35:33.465117 mapclassify-2.6.0/mapclassify/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-21 20:34:51.000000 mapclassify-2.6.0/mapclassify/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:35:33.465117 mapclassify-2.6.0/mapclassify/datasets/calemp/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-21 20:34:51.000000 mapclassify-2.6.0/mapclassify/datasets/calemp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-21 20:34:51.000000 mapclassify-2.6.0/mapclassify/datasets/calemp/calempdensity.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-21 20:34:51.000000 mapclassify-2.6.0/mapclassify/datasets/calemp/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10886 2023-07-21 20:34:51.000000 mapclassify-2.6.0/mapclassify/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-21 20:34:51.000000 mapclassify-2.6.0/mapclassify/pooling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:35:33.465117 mapclassify-2.6.0/mapclassify/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:34:51.000000 mapclassify-2.6.0/mapclassify/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-21 20:34:51.000000 mapclassify-2.6.0/mapclassify/tests/test_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-07-21 20:34:51.000000 mapclassify-2.6.0/mapclassify/tests/test_greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21319 2023-07-21 20:34:51.000000 mapclassify-2.6.0/mapclassify/tests/test_mapclassify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:35:33.465117 mapclassify-2.6.0/mapclassify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-07-21 20:35:33.000000 mapclassify-2.6.0/mapclassify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-21 20:35:33.000000 mapclassify-2.6.0/mapclassify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:35:33.000000 mapclassify-2.6.0/mapclassify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:35:33.000000 mapclassify-2.6.0/mapclassify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-21 20:35:33.000000 mapclassify-2.6.0/mapclassify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 20:35:33.000000 mapclassify-2.6.0/mapclassify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 20:34:51.000000 mapclassify-2.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-21 20:34:51.000000 mapclassify-2.6.0/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 20:34:51.000000 mapclassify-2.6.0/requirements_speedups.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 20:34:51.000000 mapclassify-2.6.0/requirements_tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-21 20:35:33.465117 mapclassify-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-21 20:34:51.000000 mapclassify-2.6.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-07-21 20:34:51.000000 mapclassify-2.6.0/versioneer.py
```

### Comparing `mapclassify-2.5.0rc3/CHANGELOG.md` & `mapclassify-2.6.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `mapclassify-2.5.0rc3/LICENSE.txt` & `mapclassify-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapclassify-2.5.0rc3/PKG-INFO` & `mapclassify-2.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapclassify
-Version: 2.5.0rc3
+Version: 2.6.0
 Summary: Classification Schemes for Choropleth Maps.
 Home-page: https://github.com/pysal/mapclassify
 Maintainer: Serge Rey, Wei Kang
 Maintainer-email: sjsrey@gmail.com, weikang9009@gmail.com
 License: 3-Clause BSD
 Keywords: spatial statistics,geovisualizaiton
 Classifier: Development Status :: 5 - Production/Stable
@@ -265,14 +265,30 @@
      Interval        Count
 --------------------------
 [   0.13,    3.36] |    19
 (   3.36,   22.86] |    19
 (  22.86, 4111.45] |    20
 ```
 
+### PrettyBreaks
+```python
+>>> np.random.seed(123456)
+>>> x = np.random.randint(0, 10000, (100,1))
+>>> mapclassify.PrettyBreaks(x)
+Pretty
+
+      Interval         Count
+----------------------------
+[  300.00,  2000.00] |    23
+( 2000.00,  4000.00] |    15
+( 4000.00,  6000.00] |    18
+( 6000.00,  8000.00] |    24
+( 8000.00, 10000.00] |    20
+ ```
+
 ### StdMean
 
 ```python
 >>> mapclassify.StdMean(y)
 StdMean
 
      Interval        Count
@@ -345,14 +361,47 @@
 >>> bp.yb
 array([5, 1, 2, 3, 2, 1, 5, 1, 3, 3, 1, 2, 2, 1, 2, 2, 2, 1, 5, 2, 4, 1, 2,
        2, 1, 1, 3, 3, 3, 5, 3, 1, 3, 5, 2, 3, 5, 5, 4, 3, 5, 3, 5, 4, 2, 1,
        1, 4, 4, 3, 3, 1, 1, 2, 1, 4, 3, 2])
 
 ```
 
+### Binning new data
+
+```python
+>>> bp = mapclassify.BoxPlot(y)
+>>> bp
+BoxPlot
+
+     Interval        Count
+--------------------------
+(   -inf,  -52.88] |     0
+( -52.88,    2.57] |    15
+(   2.57,    9.36] |    14
+(   9.36,   39.53] |    14
+(  39.53,   94.97] |     6
+(  94.97, 4111.45] |     9
+>>> bp.find_bin([0, 7, 3000, 48])
+array([1, 2, 5, 4])
+
+```
+Note that `find_bin` does not recalibrate the classifier:
+```python
+>>> bp
+BoxPlot
+
+     Interval        Count
+--------------------------
+(   -inf,  -52.88] |     0
+( -52.88,    2.57] |    15
+(   2.57,    9.36] |    14
+(   9.36,   39.53] |    14
+(  39.53,   94.97] |     6
+(  94.97, 4111.45] |     9
+```
 ### Apply
 
 ```python
 >>> import mapclassify 
 >>> import pandas
 >>> from numpy import linspace as lsp
 >>> data = [lsp(3,8,num=10), lsp(10, 0, num=10), lsp(-5, 15, num=10)]
```

### Comparing `mapclassify-2.5.0rc3/README.md` & `mapclassify-2.6.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -238,14 +238,30 @@
      Interval        Count
 --------------------------
 [   0.13,    3.36] |    19
 (   3.36,   22.86] |    19
 (  22.86, 4111.45] |    20
 ```
 
+### PrettyBreaks
+```python
+>>> np.random.seed(123456)
+>>> x = np.random.randint(0, 10000, (100,1))
+>>> mapclassify.PrettyBreaks(x)
+Pretty
+
+      Interval         Count
+----------------------------
+[  300.00,  2000.00] |    23
+( 2000.00,  4000.00] |    15
+( 4000.00,  6000.00] |    18
+( 6000.00,  8000.00] |    24
+( 8000.00, 10000.00] |    20
+ ```
+
 ### StdMean
 
 ```python
 >>> mapclassify.StdMean(y)
 StdMean
 
      Interval        Count
@@ -318,14 +334,47 @@
 >>> bp.yb
 array([5, 1, 2, 3, 2, 1, 5, 1, 3, 3, 1, 2, 2, 1, 2, 2, 2, 1, 5, 2, 4, 1, 2,
        2, 1, 1, 3, 3, 3, 5, 3, 1, 3, 5, 2, 3, 5, 5, 4, 3, 5, 3, 5, 4, 2, 1,
        1, 4, 4, 3, 3, 1, 1, 2, 1, 4, 3, 2])
 
 ```
 
+### Binning new data
+
+```python
+>>> bp = mapclassify.BoxPlot(y)
+>>> bp
+BoxPlot
+
+     Interval        Count
+--------------------------
+(   -inf,  -52.88] |     0
+( -52.88,    2.57] |    15
+(   2.57,    9.36] |    14
+(   9.36,   39.53] |    14
+(  39.53,   94.97] |     6
+(  94.97, 4111.45] |     9
+>>> bp.find_bin([0, 7, 3000, 48])
+array([1, 2, 5, 4])
+
+```
+Note that `find_bin` does not recalibrate the classifier:
+```python
+>>> bp
+BoxPlot
+
+     Interval        Count
+--------------------------
+(   -inf,  -52.88] |     0
+( -52.88,    2.57] |    15
+(   2.57,    9.36] |    14
+(   9.36,   39.53] |    14
+(  39.53,   94.97] |     6
+(  94.97, 4111.45] |     9
+```
 ### Apply
 
 ```python
 >>> import mapclassify 
 >>> import pandas
 >>> from numpy import linspace as lsp
 >>> data = [lsp(3,8,num=10), lsp(10, 0, num=10), lsp(-5, 15, num=10)]
```

### Comparing `mapclassify-2.5.0rc3/mapclassify/__init__.py` & `mapclassify-2.6.0/mapclassify/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     JenksCaspallForced,
     JenksCaspallSampled,
     KClassifiers,
     MaximumBreaks,
     MaxP,
     NaturalBreaks,
     Percentiles,
+    PrettyBreaks,
     Quantiles,
     StdMean,
     UserDefined,
     gadf,
     load_example,
 )
 from .greedy import greedy
```

### Comparing `mapclassify-2.5.0rc3/mapclassify/_classify_API.py` & `mapclassify-2.6.0/mapclassify/_classify_API.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     JenksCaspall,
     JenksCaspallForced,
     JenksCaspallSampled,
     MaximumBreaks,
     MaxP,
     NaturalBreaks,
     Percentiles,
+    PrettyBreaks,
     Quantiles,
     StdMean,
     UserDefined,
 )
 
 __author__ = "Stefanie Lumnitz <stefanie.lumitz@gmail.com>"
 
@@ -29,14 +30,15 @@
     "jenkscaspallforced": JenksCaspallForced,
     "jenkscaspallsampled": JenksCaspallSampled,
     "maxp": MaxP,
     "maximumbreaks": MaximumBreaks,
     "naturalbreaks": NaturalBreaks,
     "quantiles": Quantiles,
     "percentiles": Percentiles,
+    "prettybreaks": PrettyBreaks,
     "stdmean": StdMean,
     "userdefined": UserDefined,
 }
 
 
 def classify(
     y,
@@ -46,14 +48,16 @@
     pct_sampled=0.10,
     truncate=True,
     hinge=1.5,
     multiples=[-2, -1, 1, 2],
     mindiff=0,
     initial=100,
     bins=None,
+    lowest=None,
+    anchor=False,
 ):
     """
 
     Classify your data with ``mapclassify.classify``.
     Input parameters are dependent on classifier used.
 
     Parameters
@@ -85,42 +89,51 @@
         Number of initial solutions to generate or number of runs when using
         ``natural_breaks`` or ``max_p_classifier``. Setting initial to ``0``
         will result in the quickest calculation of bins.
     bins : numpy.array (default None)
         :math:`(k,1)`, upper bounds of classes (have to be monotically
         increasing) if using ``user_defined`` classifier.
         Default is ``None``. For example: ``[20, max(y)]``.
+    lowest : float (default None)
+        Scalar minimum value of lowest class. Default is to set the minimum
+        to ``-inf`` if  ``y.min()`` > first upper bound (which will override
+        the default), otherwise minimum is set to ``y.min()``.
+    anchor : bool (default False)
+            Anchor upper bound of one class to the sample mean.
+
+
 
     Returns
     -------
     classifier : mapclassify.classifiers.MapClassifier
         Object containing bin ids for each observation (``.yb``),
         upper bounds of each class (``.bins``), number of classes (``.k``)
         and number of observations falling in each class (``.counts``).
 
     Notes
     -----
 
     Supported classifiers include:
 
     * ``quantiles``
-    * ``box_plot``
-    * ``equal_interval``
-    * ``fisher_jenks``
-    * ``fisher_jenks_sampled``
-    * ``headtail_breaks``
-    * ``jenks_caspall``
-    * ``jenks_caspall_sampled``
-    * ``jenks_caspall_forced``
-    * ``max_p``
-    * ``maximum_breaks``
-    * ``natural_breaks``
+    * ``boxplot``
+    * ``equalinterval``
+    * ``fisherjenks``
+    * ``fisherjenkssampled``
+    * ``headtailbreaks``
+    * ``jenkscaspall``
+    * ``jenkscaspallsampled``
+    * ``jenks_caspallforced``
+    * ``maxp``
+    * ``maximumbreaks``
+    * ``naturalbreaks``
     * ``percentiles``
-    * ``std_mean``
-    * ``user_defined``
+    * ``prettybreaks``
+    * ``stdmean``
+    * ``userdefined``
 
     Examples
     --------
 
     >>> import libpysal
     >>> import geopandas
     >>> from mapclassify import classify
@@ -172,31 +185,32 @@
     elif scheme == "headtailbreaks":
         classifier = _classifiers[scheme](y)
 
     elif scheme == "percentiles":
         classifier = _classifiers[scheme](y, pct)
 
     elif scheme == "stdmean":
-        classifier = _classifiers[scheme](y, multiples)
+        classifier = _classifiers[scheme](y, multiples, anchor)
 
     elif scheme == "jenkscaspallsampled":
         classifier = _classifiers[scheme](y, k, pct_sampled)
 
     elif scheme == "maximumbreaks":
         classifier = _classifiers[scheme](y, k, mindiff)
 
     elif scheme in ["naturalbreaks", "maxp"]:
         classifier = _classifiers[scheme](y, k, initial)
 
     elif scheme == "userdefined":
-        classifier = _classifiers[scheme](y, bins)
+        classifier = _classifiers[scheme](y, bins, lowest)
 
     elif scheme in [
         "equalinterval",
         "fisherjenks",
         "jenkscaspall",
         "jenkscaspallforced",
         "quantiles",
+        "prettybreaks",
     ]:
         classifier = _classifiers[scheme](y, k)
 
     return classifier
```

### Comparing `mapclassify-2.5.0rc3/mapclassify/classifiers.py` & `mapclassify-2.6.0/mapclassify/classifiers.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "JenksCaspallSampled",
     "HeadTailBreaks",
     "MaxP",
     "MaximumBreaks",
     "NaturalBreaks",
     "Quantiles",
     "Percentiles",
+    "PrettyBreaks",
     "StdMean",
     "UserDefined",
     "gadf",
     "KClassifiers",
     "CLASSIFIERS",
 ]
 
@@ -44,14 +45,15 @@
     "JenksCaspallForced",
     "JenksCaspallSampled",
     "MaxP",
     "MaximumBreaks",
     "NaturalBreaks",
     "Quantiles",
     "Percentiles",
+    "PrettyBreaks",
     "StdMean",
     "UserDefined",
 )
 
 K = 5  # default number of classes in any map scheme with this as an argument
 SEEDRANGE = 1000000  # range for drawing random ints from for Natural Breaks
 
@@ -450,14 +452,49 @@
         k -= 1
         l, r = cuts.pop(-1)
         binIds += (x > l) * (x <= r) * k
     counts = np.bincount(binIds, minlength=len(bins))
     return (binIds, counts)
 
 
+def _pretty_number(x, rounded=True):
+    exp = np.floor(np.log10(x))
+    f = x / 10**exp
+    if rounded:
+        if f < 1.5:
+            nf = 1.0
+        elif f < 3.0:
+            nf = 2.0
+        elif f < 7.0:
+            nf = 5.0
+        else:
+            nf = 10.0
+    else:
+        if f <= 1.0:
+            nf = 1.0
+        elif f <= 2.0:
+            nf = 2.0
+        elif f <= 5.0:
+            nf = 5.0
+        else:
+            nf = 10.0
+
+    return nf * 10.0**exp
+
+
+def _pretty(y, k=5):
+    low = y.min()
+    high = y.max()
+    rg = _pretty_number(high - low, False)
+    d = _pretty_number(rg / (k - 1), True)
+    miny = np.floor(low / d) * d
+    maxy = np.ceil(high / d) * d
+    return np.arange(miny, maxy + 0.5 * d, d)
+
+
 def load_example():
     """
     Helper function for doc tests
     """
     from .datasets import calemp
 
     return calemp.load()
@@ -1143,15 +1180,14 @@
     """
 
     def __init__(self, y):
         MapClassifier.__init__(self, y)
         self.name = "HeadTailBreaks"
 
     def _set_bins(self):
-
         x = self.y.copy()
         bins = []
         bins = head_tail_breaks(x, bins)
         self.bins = np.array(bins)
         self.k = len(self.bins)
 
 
@@ -1320,14 +1356,49 @@
             self._update(y, **kwargs)
         else:
             new = copy.deepcopy(self)
             new._update(y, **kwargs)
             return new
 
 
+class PrettyBreaks(MapClassifier):
+    def __init__(self, y, k=5):
+        """
+        Pretty breakpoints
+
+        Computes breaks that are equally spaced round values which
+        cover the range of values in `y`. The breaks are chosen so that
+        they are 1, 2, or 5 times a power of 10.
+
+
+        Parameters
+        ----------
+        y : array (n,1)
+            attribute to classify
+        k : int
+            The number of desired classes
+
+
+        Notes
+        -----
+        The number of classes may be different from the specified `k`,
+        as the rounding of the upper bounds takes precedent.
+
+        The lower bound of the first interval will be equal to the
+        minimum of the data.
+        """
+        self.k = k
+        MapClassifier.__init__(self, y)
+        self.name = "Pretty"
+
+    def _set_bins(self):
+        bins = _pretty(self.y, self.k)
+        self.bins = bins[1:]
+
+
 class BoxPlot(MapClassifier):
     """
     BoxPlot Map Classification.
 
     Parameters
     ----------
 
@@ -1517,33 +1588,46 @@
 
 class StdMean(MapClassifier):
     """
     Standard Deviation and Mean Map Classification.
 
     Parameters
     ----------
-
     y : numpy.array
-        :math:`(n,1)`, values to classify.
+        :math:`(n,1)`, values to classify
     multiples : numpy.array (default [-2, -1, 1, 2])
         The multiples of the standard deviation to add/subtract from
-        the sample mean to define the bins
+        the sample mean to define the bins.
+    anchor : bool (default False)
+        Anchor upper bound of one class to the sample mean.
+
 
     Attributes
     ----------
 
     yb : numpy.array
         :math:`(n,1)`, bin IDs for observations.
     bins : numpy.array
         :math:`(k,1)`, the upper bounds of each class.
     k : int
         The number of classes.
     counts : numpy.array
         :math:`(k,1)`, the number of observations falling in each class.
 
+    Notes
+    -----
+
+    If anchor is True, one of the intervals will have its closed upper bound
+    equal to the mean of y. Intermediate intervals will have widths equal to
+    the standard deviation of y. The first interval will be closed on the
+    minimum value of y, and the last interval will be closed on the maximum of
+    y. The first and last intervals may have widths different from the
+    intermediate intervals.
+
+
     Examples
     --------
 
     >>> import mapclassify
     >>> cal = mapclassify.load_example()
     >>> st = mapclassify.StdMean(cal)
     >>> st.k
@@ -1559,26 +1643,39 @@
     >>> st3 = mapclassify.StdMean(cal, multiples = [-3, -1.5, 1.5, 3])
     >>> st3.bins
     array([-1514.00758246,  -694.03973951,   945.8959464 ,  1765.86378936,
             4111.45      ])
 
     >>> list(st3.counts)
     [0, 0, 57, 0, 1]
-
+    >>> stda = mapclassify.StdMean(cal, anchor=True)
+    >>> stda.k
+    9
+    >>> stda.bins
+    array([ 125.92810345,  672.57333208, 1219.21856072, 1765.86378936,
+           2312.50901799, 2859.15424663, 3405.79947527, 3952.4447039 ,
+           4111.45      ])
+    >>> cal.mean(), cal.std(), cal.min(), cal.max()
+    (125.92810344827588, 546.6452286365233, 0.13, 4111.45)
     """
 
-    def __init__(self, y, multiples=[-2, -1, 1, 2]):
+    def __init__(self, y, multiples=[-2, -1, 1, 2], anchor=False):
         self.multiples = multiples
+        self.anchor = anchor
         MapClassifier.__init__(self, y)
         self.name = "StdMean"
 
     def _set_bins(self):
         y = self.y
         s = y.std(ddof=1)
         m = y.mean()
+        if self.anchor:
+            min_z = int((y.min() - m) / s)
+            max_z = int((y.max() - m) / s) + 1
+            self.multiples = list(range(min_z, max_z))
         cuts = [m + s * w for w in self.multiples]
         y_max = y.max()
         if cuts[-1] < y_max:
             cuts.append(y_max)
         self.bins = np.array(cuts)
         self.k = len(cuts)
 
@@ -1761,15 +1858,14 @@
     def __init__(self, y, k=K, initial=10):
         self.k = k
         self.init = initial
         MapClassifier.__init__(self, y)
         self.name = "NaturalBreaks"
 
     def _set_bins(self):
-
         x = self.y.copy()
         k = self.k
         values = np.array(x)
         uv = np.unique(values)
         uvk = len(uv)
         if uvk < k:
             warnings.warn(
```

### Comparing `mapclassify-2.5.0rc3/mapclassify/datasets/calemp/calempdensity.csv` & `mapclassify-2.6.0/mapclassify/datasets/calemp/calempdensity.csv`

 * *Files identical despite different names*

### Comparing `mapclassify-2.5.0rc3/mapclassify/greedy.py` & `mapclassify-2.6.0/mapclassify/greedy.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         color_areas[c] = 0
 
     if balance == "centroid":
         features = features.copy()
         features.geometry = features.geometry.centroid
         balance = "distance"
 
-    for (feature_id, n) in sorted_by_count:
+    for feature_id, n in sorted_by_count:
         # first work out which already assigned colors are adjacent to this feature
         adjacent_colors = set()
         for neighbour in sw.neighbors[feature_id]:
             if neighbour in feature_colors:
                 adjacent_colors.add(feature_colors[neighbour])
 
         # from the existing colors, work out which are available (ie non-adjacent)
@@ -108,15 +108,14 @@
                     if c in available_colors
                 }
 
                 distances = features.loc[other_features.keys()].distance(this_feature)
                 # calculate the min distance from this feature to the nearest
                 # feature with each assigned color
                 for other_feature_id, c in other_features.items():
-
                     distance = distances.loc[other_feature_id]
                     if distance < min_distances[c]:
                         min_distances[c] = distance
 
                 # choose color such that min distance is maximised!
                 # - ie we want MAXIMAL separation between features with the same color
                 feature_color = sorted(
```

### Comparing `mapclassify-2.5.0rc3/mapclassify/pooling.py` & `mapclassify-2.6.0/mapclassify/pooling.py`

 * *Files identical despite different names*

### Comparing `mapclassify-2.5.0rc3/mapclassify/tests/test_classify.py` & `mapclassify-2.6.0/mapclassify/tests/test_classify.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,18 @@
         _assertions(a, b)
 
     def test_percentiles(self):
         a = mapclassify.classify(self.x, "percentiles", pct=[25, 50, 75, 100])
         b = mapclassify.Percentiles(self.x, pct=[25, 50, 75, 100])
         _assertions(a, b)
 
+        a = mapclassify.classify(self.x, "prettybreaks")
+        b = mapclassify.PrettyBreaks(self.x)
+        _assertions(a, b)
+
     def test_jenks_caspall(self):
         a = mapclassify.classify(self.x, "JenksCaspall", k=3)
         b = mapclassify.JenksCaspall(self.x, k=3)
         _assertions(a, b)
 
     def test_jenks_caspall_forced(self):
         a = mapclassify.classify(self.x, "JenksCaspallForced", k=3)
```

### Comparing `mapclassify-2.5.0rc3/mapclassify/tests/test_greedy.py` & `mapclassify-2.6.0/mapclassify/tests/test_greedy.py`

 * *Files identical despite different names*

### Comparing `mapclassify-2.5.0rc3/mapclassify/tests/test_mapclassify.py` & `mapclassify-2.6.0/mapclassify/tests/test_mapclassify.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 
 
 class TestFindBin:
     def setup_method(self):
         self.V = load_example()
 
     def test_find_bin(self):
-
         toclass = [0, 1, 3, 5, 50, 70, 101, 202, 390, 505, 800, 5000, 5001]
         mc = FisherJenks(self.V, k=5)
         known = [0, 0, 0, 0, 0, 0, 1, 2, 3, 3, 4, 4, 4]
         numpy.testing.assert_array_equal(known, mc.find_bin(toclass))
 
         mc2 = FisherJenks(self.V, k=9)
         known = [0, 0, 0, 0, 2, 2, 3, 5, 7, 7, 8, 8, 8]
@@ -355,14 +354,25 @@
         V = numpy.array([1 + 2**-52, 1, 1])
         htb = HeadTailBreaks(V)
         assert htb.k == 2
         assert len(htb.counts) == 2
         numpy.testing.assert_array_almost_equal(htb.counts, numpy.array([2, 1]))
 
 
+class TestPrettyBreaks:
+    def setup_method(self):
+        self.V = load_example()
+
+    def test_pretty(self):
+        res = PrettyBreaks(self.V)
+        assert res.k == 5
+        numpy.testing.assert_array_equal(res.counts, [57, 0, 0, 0, 1])
+        numpy.testing.assert_array_equal(res.bins, list(range(1000, 6000, 1000)))
+
+
 class TestMapClassifier:
     def test_Map_Classifier(self):
         # map__classifier = Map_Classifier(y)
         assert True  # TODO: implement your test here
 
     def test___repr__(self):
         # map__classifier = Map_Classifier(y)
@@ -619,14 +629,46 @@
 
     def test_UserDefined_invariant(self):
         bins = [10, 20, 30, 40]
         ud = UserDefined(numpy.array([12, 12, 12]), bins)
         numpy.testing.assert_array_almost_equal(ud.bins, numpy.array([10, 20, 30, 40]))
         numpy.testing.assert_array_almost_equal(ud.counts, numpy.array([0, 3, 0, 0]))
 
+    def test_UserDefined_lowest(self):
+        bins = [20, max(self.V)]
+        ud = UserDefined(self.V, bins, lowest=-1.0)
+        numpy.testing.assert_array_almost_equal(ud.bins, numpy.array([20.0, 4111.45]))
+        numpy.testing.assert_array_almost_equal(ud.counts, numpy.array([37, 21]))
+        classes = ["[  -1.00,   20.00]", "(  20.00, 4111.45]"]
+        assert ud.get_legend_classes() == classes
+
+
+class TestStdMeanAnchor:
+    def setup_method(self):
+        self.V = load_example()
+
+    def test_StdMeanAnchor(self):
+        sm = StdMean(self.V, anchor=True)
+        bins = numpy.array(
+            [
+                125.92810345,
+                672.57333208,
+                1219.21856072,
+                1765.86378936,
+                2312.50901799,
+                2859.15424663,
+                3405.79947527,
+                3952.4447039,
+                4111.45,
+            ]
+        )
+        counts = numpy.array([50, 6, 1, 0, 0, 0, 0, 0, 1])
+        numpy.testing.assert_array_almost_equal(sm.bins, bins)
+        numpy.testing.assert_array_almost_equal(sm.counts, counts)
+
 
 class TestMaxP:
     def setup_method(self):
         self.V = load_example()
 
     def test_MaxP(self):
         numpy.random.seed(100)
```

### Comparing `mapclassify-2.5.0rc3/mapclassify.egg-info/PKG-INFO` & `mapclassify-2.6.0/mapclassify.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapclassify
-Version: 2.5.0rc3
+Version: 2.6.0
 Summary: Classification Schemes for Choropleth Maps.
 Home-page: https://github.com/pysal/mapclassify
 Maintainer: Serge Rey, Wei Kang
 Maintainer-email: sjsrey@gmail.com, weikang9009@gmail.com
 License: 3-Clause BSD
 Keywords: spatial statistics,geovisualizaiton
 Classifier: Development Status :: 5 - Production/Stable
@@ -265,14 +265,30 @@
      Interval        Count
 --------------------------
 [   0.13,    3.36] |    19
 (   3.36,   22.86] |    19
 (  22.86, 4111.45] |    20
 ```
 
+### PrettyBreaks
+```python
+>>> np.random.seed(123456)
+>>> x = np.random.randint(0, 10000, (100,1))
+>>> mapclassify.PrettyBreaks(x)
+Pretty
+
+      Interval         Count
+----------------------------
+[  300.00,  2000.00] |    23
+( 2000.00,  4000.00] |    15
+( 4000.00,  6000.00] |    18
+( 6000.00,  8000.00] |    24
+( 8000.00, 10000.00] |    20
+ ```
+
 ### StdMean
 
 ```python
 >>> mapclassify.StdMean(y)
 StdMean
 
      Interval        Count
@@ -345,14 +361,47 @@
 >>> bp.yb
 array([5, 1, 2, 3, 2, 1, 5, 1, 3, 3, 1, 2, 2, 1, 2, 2, 2, 1, 5, 2, 4, 1, 2,
        2, 1, 1, 3, 3, 3, 5, 3, 1, 3, 5, 2, 3, 5, 5, 4, 3, 5, 3, 5, 4, 2, 1,
        1, 4, 4, 3, 3, 1, 1, 2, 1, 4, 3, 2])
 
 ```
 
+### Binning new data
+
+```python
+>>> bp = mapclassify.BoxPlot(y)
+>>> bp
+BoxPlot
+
+     Interval        Count
+--------------------------
+(   -inf,  -52.88] |     0
+( -52.88,    2.57] |    15
+(   2.57,    9.36] |    14
+(   9.36,   39.53] |    14
+(  39.53,   94.97] |     6
+(  94.97, 4111.45] |     9
+>>> bp.find_bin([0, 7, 3000, 48])
+array([1, 2, 5, 4])
+
+```
+Note that `find_bin` does not recalibrate the classifier:
+```python
+>>> bp
+BoxPlot
+
+     Interval        Count
+--------------------------
+(   -inf,  -52.88] |     0
+( -52.88,    2.57] |    15
+(   2.57,    9.36] |    14
+(   9.36,   39.53] |    14
+(  39.53,   94.97] |     6
+(  94.97, 4111.45] |     9
+```
 ### Apply
 
 ```python
 >>> import mapclassify 
 >>> import pandas
 >>> from numpy import linspace as lsp
 >>> data = [lsp(3,8,num=10), lsp(10, 0, num=10), lsp(-5, 15, num=10)]
```

### Comparing `mapclassify-2.5.0rc3/mapclassify.egg-info/SOURCES.txt` & `mapclassify-2.6.0/mapclassify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapclassify-2.5.0rc3/setup.py` & `mapclassify-2.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `mapclassify-2.5.0rc3/versioneer.py` & `mapclassify-2.6.0/versioneer.py`

 * *Files identical despite different names*

