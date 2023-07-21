# Comparing `tmp/datamazing-2.0.0.tar.gz` & `tmp/datamazing-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamazing-2.0.0.tar", max compression
+gzip compressed data, was "datamazing-2.0.1.tar", max compression
```

## Comparing `datamazing-2.0.0.tar` & `datamazing-2.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2023-07-18 08:23:00.186902 datamazing-2.0.0/datamazing/__init__.py
--rw-r--r--   0        0        0      277 2023-07-18 08:23:00.186902 datamazing-2.0.0/datamazing/_conform.py
--rw-r--r--   0        0        0      402 2023-07-18 08:23:00.186902 datamazing-2.0.0/datamazing/pandas/__init__.py
--rw-r--r--   0        0        0      267 2023-07-18 08:23:00.186902 datamazing-2.0.0/datamazing/pandas/datacollection/__init__.py
--rw-r--r--   0        0        0      126 2023-07-18 08:23:00.186902 datamazing-2.0.0/datamazing/pandas/testing/__init__.py
--rw-r--r--   0        0        0      766 2023-07-18 08:23:00.186902 datamazing-2.0.0/datamazing/pandas/testing/assertions.py
--rw-r--r--   0        0        0     3818 2023-07-18 08:23:00.186902 datamazing-2.0.0/datamazing/pandas/testing/data.py
--rw-r--r--   0        0        0        0 2023-07-18 08:23:00.186902 datamazing-2.0.0/datamazing/pandas/transformations/__init__.py
--rw-r--r--   0        0        0      649 2023-07-18 08:23:00.186902 datamazing-2.0.0/datamazing/pandas/transformations/basic.py
--rw-r--r--   0        0        0     3497 2023-07-18 08:23:00.186902 datamazing-2.0.0/datamazing/pandas/transformations/grouping.py
--rw-r--r--   0        0        0     1012 2023-07-18 08:23:00.186902 datamazing-2.0.0/datamazing/pandas/transformations/resampling.py
--rw-r--r--   0        0        0      660 2023-07-18 08:23:00.186902 datamazing-2.0.0/datamazing/pandas/types.py
--rw-r--r--   0        0        0      184 2023-07-18 08:23:00.186902 datamazing-2.0.0/datamazing/pyspark/__init__.py
--rw-r--r--   0        0        0       92 2023-07-18 08:23:00.186902 datamazing-2.0.0/datamazing/pyspark/testing/__init__.py
--rw-r--r--   0        0        0      295 2023-07-18 08:23:00.186902 datamazing-2.0.0/datamazing/pyspark/testing/assertions.py
--rw-r--r--   0        0        0     2064 2023-07-18 08:23:00.186902 datamazing-2.0.0/datamazing/pyspark/testing/data.py
--rw-r--r--   0        0        0        0 2023-07-18 08:23:00.186902 datamazing-2.0.0/datamazing/pyspark/transformations/__init__.py
--rw-r--r--   0        0        0     3058 2023-07-18 08:23:00.186902 datamazing-2.0.0/datamazing/pyspark/transformations/grouping.py
--rw-r--r--   0        0        0      708 2023-07-18 08:23:00.186902 datamazing-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      454 1970-01-01 00:00:00.000000 datamazing-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/__init__.py
+-rw-r--r--   0        0        0      277 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/_conform.py
+-rw-r--r--   0        0        0      402 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/__init__.py
+-rw-r--r--   0        0        0      309 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/datacollection/__init__.py
+-rw-r--r--   0        0        0      126 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/testing/__init__.py
+-rw-r--r--   0        0        0      766 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/testing/assertions.py
+-rw-r--r--   0        0        0     4016 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/testing/data.py
+-rw-r--r--   0        0        0        0 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/transformations/__init__.py
+-rw-r--r--   0        0        0      649 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/transformations/basic.py
+-rw-r--r--   0        0        0     3497 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/transformations/grouping.py
+-rw-r--r--   0        0        0     1012 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/transformations/resampling.py
+-rw-r--r--   0        0        0      660 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/types.py
+-rw-r--r--   0        0        0      184 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pyspark/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pyspark/testing/__init__.py
+-rw-r--r--   0        0        0      295 2023-07-21 08:46:39.146649 datamazing-2.0.1/datamazing/pyspark/testing/assertions.py
+-rw-r--r--   0        0        0     2064 2023-07-21 08:46:39.146649 datamazing-2.0.1/datamazing/pyspark/testing/data.py
+-rw-r--r--   0        0        0        0 2023-07-21 08:46:39.146649 datamazing-2.0.1/datamazing/pyspark/transformations/__init__.py
+-rw-r--r--   0        0        0     3058 2023-07-21 08:46:39.146649 datamazing-2.0.1/datamazing/pyspark/transformations/grouping.py
+-rw-r--r--   0        0        0      708 2023-07-21 08:46:39.146649 datamazing-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      454 1970-01-01 00:00:00.000000 datamazing-2.0.1/PKG-INFO
```

### Comparing `datamazing-2.0.0/datamazing/pandas/testing/assertions.py` & `datamazing-2.0.1/datamazing/pandas/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `datamazing-2.0.0/datamazing/pandas/testing/data.py` & `datamazing-2.0.1/datamazing/pandas/testing/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,22 +102,29 @@
         >>> TestData(file_pattern="{table_name}.df.csv")
         """
         self.file_pattern = file_pattern
         self.subfolder = subfolder
         self.time_column = time_column
 
     def query(
-        self, table_name: str, time_interval: TimeInterval = None
+        self,
+        table_name: str,
+        time_interval: TimeInterval = None,
+        filters: dict[str, object] = None,
     ) -> pd.DataFrame:
         # get filename associated with table
         filename = self.file_pattern.format(table_name=table_name)
 
         df = read_df(filename, subfolder=self.subfolder)
 
         if time_interval:
             # filter to time interval
             is_after_start = df[self.time_column] >= time_interval.left
             is_before_end = df[self.time_column] <= time_interval.right
             is_in_interval = is_after_start & is_before_end
             df = df[is_in_interval]
 
+        if filters:
+            df = df[(df[filters.keys()] == filters.values()).all(axis=1)]
+            df = df.reset_index(drop=True)
+
         return df
```

### Comparing `datamazing-2.0.0/datamazing/pandas/transformations/basic.py` & `datamazing-2.0.1/datamazing/pandas/transformations/basic.py`

 * *Files identical despite different names*

### Comparing `datamazing-2.0.0/datamazing/pandas/transformations/grouping.py` & `datamazing-2.0.1/datamazing/pandas/transformations/grouping.py`

 * *Files identical despite different names*

### Comparing `datamazing-2.0.0/datamazing/pandas/transformations/resampling.py` & `datamazing-2.0.1/datamazing/pandas/transformations/resampling.py`

 * *Files identical despite different names*

### Comparing `datamazing-2.0.0/datamazing/pandas/types.py` & `datamazing-2.0.1/datamazing/pandas/types.py`

 * *Files identical despite different names*

### Comparing `datamazing-2.0.0/datamazing/pyspark/testing/data.py` & `datamazing-2.0.1/datamazing/pyspark/testing/data.py`

 * *Files identical despite different names*

### Comparing `datamazing-2.0.0/datamazing/pyspark/transformations/grouping.py` & `datamazing-2.0.1/datamazing/pyspark/transformations/grouping.py`

 * *Files identical despite different names*

### Comparing `datamazing-2.0.0/pyproject.toml` & `datamazing-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datamazing"
-version = "2.0.0"
+version = "2.0.1"
 description = "Package for working with pandas Dataset, but wit specialized functions used for Energinet"
 authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "datamazing" },
 ]
 
 [tool.poetry.dependencies]
```

