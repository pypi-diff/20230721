# Comparing `tmp/varya-0.0.6a1-py3-none-any.whl.zip` & `tmp/varya-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,27 @@
-Zip file size: 4314 bytes, number of entries: 9
--rw-r--r--  2.0 unx      206 b- defN 23-Mar-12 11:02 varya/__init__.py
+Zip file size: 14511 bytes, number of entries: 25
+-rw-r--r--  2.0 unx      204 b- defN 23-Jul-21 11:03 varya/__init__.py
 -rw-r--r--  2.0 unx     2140 b- defN 23-Mar-11 04:33 varya/compose/__compose.py
--rw-r--r--  2.0 unx       44 b- defN 23-Mar-11 05:45 varya/compose/__init__.py
--rw-r--r--  2.0 unx     3227 b- defN 23-Mar-12 11:02 varya/compose/core.py
--rw-r--r--  2.0 unx     1519 b- defN 23-Mar-12 11:02 varya-0.0.6a1.dist-info/LICENSE
--rw-r--r--  2.0 unx      558 b- defN 23-Mar-12 11:02 varya-0.0.6a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-12 11:02 varya-0.0.6a1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Mar-12 11:02 varya-0.0.6a1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      698 b- defN 23-Mar-12 11:02 varya-0.0.6a1.dist-info/RECORD
-9 files, 8491 bytes uncompressed, 3112 bytes compressed:  63.3%
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-29 21:29 varya/compose/__init__.py
+-rw-r--r--  2.0 unx     3271 b- defN 23-Jul-21 10:50 varya/compose/core.py
+-rw-r--r--  2.0 unx      295 b- defN 23-Apr-23 00:07 varya/metrics/__init__.py
+-rw-r--r--  2.0 unx      949 b- defN 23-Jun-29 21:28 varya/metrics/classification.py
+-rw-r--r--  2.0 unx     2085 b- defN 23-Jun-29 21:28 varya/metrics/regression.py
+-rw-r--r--  2.0 unx       74 b- defN 23-Mar-16 06:58 varya/model_selection/__init__.py
+-rw-r--r--  2.0 unx     6789 b- defN 23-Jun-29 22:50 varya/model_selection/_split.py
+-rw-r--r--  2.0 unx       74 b- defN 23-Mar-16 06:58 varya/preprocessing/__init__.py
+-rw-r--r--  2.0 unx     4251 b- defN 23-Mar-16 06:58 varya/preprocessing/_split.py
+-rw-r--r--  2.0 unx      777 b- defN 23-Jun-29 23:08 varya/utils/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 23:34 varya/utils/distances.py
+-rw-r--r--  2.0 unx      726 b- defN 23-Jun-29 21:24 varya/utils/probe.py
+-rw-r--r--  2.0 unx      671 b- defN 23-Jun-29 23:08 varya/utils/recast.py
+-rw-r--r--  2.0 unx      263 b- defN 23-Jun-29 22:40 varya/utils/tools.py
+-rw-r--r--  2.0 unx     2438 b- defN 23-Apr-22 23:47 varya/utils/validation.py
+-rw-r--r--  2.0 unx     1108 b- defN 23-Jun-29 23:07 varya/utils/verify.py
+-rw-r--r--  2.0 unx      619 b- defN 23-Mar-13 07:42 varya/utlis/__init__.py
+-rw-r--r--  2.0 unx     2463 b- defN 23-Mar-13 07:37 varya/utlis/validation.py
+-rw-r--r--  2.0 unx     1519 b- defN 23-Jul-21 11:03 varya-0.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      585 b- defN 23-Jul-21 11:03 varya-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 11:03 varya-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-21 11:03 varya-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1995 b- defN 23-Jul-21 11:03 varya-0.1.0.dist-info/RECORD
+25 files, 33445 bytes uncompressed, 11295 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -6,23 +6,71 @@
 
 Filename: varya/compose/__init__.py
 Comment: 
 
 Filename: varya/compose/core.py
 Comment: 
 
-Filename: varya-0.0.6a1.dist-info/LICENSE
+Filename: varya/metrics/__init__.py
 Comment: 
 
-Filename: varya-0.0.6a1.dist-info/METADATA
+Filename: varya/metrics/classification.py
 Comment: 
 
-Filename: varya-0.0.6a1.dist-info/WHEEL
+Filename: varya/metrics/regression.py
 Comment: 
 
-Filename: varya-0.0.6a1.dist-info/top_level.txt
+Filename: varya/model_selection/__init__.py
 Comment: 
 
-Filename: varya-0.0.6a1.dist-info/RECORD
+Filename: varya/model_selection/_split.py
+Comment: 
+
+Filename: varya/preprocessing/__init__.py
+Comment: 
+
+Filename: varya/preprocessing/_split.py
+Comment: 
+
+Filename: varya/utils/__init__.py
+Comment: 
+
+Filename: varya/utils/distances.py
+Comment: 
+
+Filename: varya/utils/probe.py
+Comment: 
+
+Filename: varya/utils/recast.py
+Comment: 
+
+Filename: varya/utils/tools.py
+Comment: 
+
+Filename: varya/utils/validation.py
+Comment: 
+
+Filename: varya/utils/verify.py
+Comment: 
+
+Filename: varya/utlis/__init__.py
+Comment: 
+
+Filename: varya/utlis/validation.py
+Comment: 
+
+Filename: varya-0.1.0.dist-info/LICENSE
+Comment: 
+
+Filename: varya-0.1.0.dist-info/METADATA
+Comment: 
+
+Filename: varya-0.1.0.dist-info/WHEEL
+Comment: 
+
+Filename: varya-0.1.0.dist-info/top_level.txt
+Comment: 
+
+Filename: varya-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## varya/__init__.py

```diff
@@ -1,6 +1,6 @@
-__version__ = '0.0.6a1'
+__version__ = '0.1.0'
 __author__ = 'Kritik Seth'
 __maintainer__ = __author__
 __license__ = 'BSD 3-Clause License'
 __url__ = 'https://github.com/varya-ml/varya'
 __connect__ = 'https://www.kritikseth.com/'
```

## varya/compose/__init__.py

```diff
@@ -1,3 +1,5 @@
 from .core import Datum
 
-__all__ = ['Datum']
+__all__ = [
+    'Datum'
+]
```

## varya/compose/core.py

```diff
@@ -1,16 +1,21 @@
 import pandas
 import numpy
 import torch
+from torch.utils.data import Dataset
 
-class Datum:
+from ..utils.recast import (
+    recast_to_tensor
+)
+
+class Datum(Dataset):
 
     """
     Data formatter, converts heterogenous data types to homogenous torch tensors.
-
+    
     Parameters
     ----------
     data / X : pandas.core.frame.DataFrame / pandas.core.series.Series / numpy.ndarray / torch.tensor
     target / y : str / int / pandas.core.frame.DataFrame / pandas.core.series.Series / numpy.ndarray / torch.tensor
     column_names : list of strings
     target_name : string
 
@@ -18,34 +23,35 @@
 
     def __init__(self, data=None, target=None):
         
         self._data = None
         self._target = None
         self.column_names = None
         self.target_name = None
+        self.id_datum = None
 
         self.data = data
         self.target = target
 
     @property
     def data(self):
-        return self._recast(self._data)
+        return recast_to_tensor(self._data)
 
     @data.setter
     def data(self, data):
 
         self._data = data
         if isinstance(data, (pandas.core.frame.DataFrame, pandas.core.series.Series)):
             self.column_names = data.columns.tolist()
 
     @property
     def target(self):
 
         if self._target is not None:
-            return self._recast(self._target).view(-1, 1)
+            return recast_to_tensor(self._target).view(-1, 1)
         else:
             return self._target
 
     @target.setter
     def target(self, target):
         
         if target is None:
@@ -57,17 +63,17 @@
             self._data = self._data.drop([target], axis=1)
             self.target_name = target            
             self.column_names = self._data.columns.tolist()
 
         elif isinstance(target, int):
             self.column_names = None
             self.target_name = None
-            self._data = self._recast(self._data)
+            self._data = recast_to_tensor(self._data)
             self._target = self._data[:, target]
-            self._data = self._data[:, np.arange(self._data.shape[1]) != target]
+            self._data = self._data[:, numpy.arange(self._data.shape[1]) != target]
         
         elif isinstance(target, (pandas.core.frame.DataFrame, pandas.core.series.Series,
                                  numpy.ndarray,
                                  torch.Tensor)):
             self._target = target
             if isinstance(target, (pandas.core.frame.DataFrame, pandas.core.series.Series)):
                 self.target_name = target.name
@@ -78,32 +84,21 @@
     
     @property
     def columns(self):
         return self.data.shape[1]
     
     @property
     def shape(self):
-        return (self.rows(), self.columns())
-
-    def _recast(self, datum):
-
-        if isinstance(datum, (pandas.core.frame.DataFrame, pandas.core.series.Series)):
-            return torch.from_numpy(datum.values)
-        
-        if isinstance(datum, numpy.ndarray):
-            return torch.from_numpy(datum)
-
-        if isinstance(datum, torch.Tensor):
-            return datum
+        return (self.rows, self.columns)
     
     def recast(self):
 
-        self._data = self._recast(self._data)
+        self._data = recast_to_tensor(self._data)
         if self._target is not None:
-            self._target = self._recast(self._target).view(-1, 1)
+            self._target = recast_to_tensor(self._target).view(-1, 1)
     
     @property
     def X(self):
         return self.data
     
     @X.setter
     def X(self, X):
@@ -111,8 +106,17 @@
     
     @property
     def y(self):
         return self.target
     
     @y.setter
     def y(self, y):
-        self.target = y
+        self.target = y
+
+    def __len__(self):
+        return self.rows
+    
+    def __getitem__(self, index):
+        if self.target is not None:
+            return self.data[index], self.target[index]
+        else:
+            return self.data[index]
```

## Comparing `varya-0.0.6a1.dist-info/LICENSE` & `varya-0.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

