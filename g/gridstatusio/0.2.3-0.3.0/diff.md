# Comparing `tmp/gridstatusio-0.2.3.tar.gz` & `tmp/gridstatusio-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/github/workspace/dist/.tmp-o9g5tupz/gridstatusio-0.2.3.tar", last modified: Mon Jul 17 14:52:05 2023, max compression
+gzip compressed data, was "/github/workspace/dist/.tmp-_7vu499n/gridstatusio-0.3.0.tar", last modified: Fri Jul 21 19:54:13 2023, max compression
```

## Comparing `gridstatusio-0.2.3.tar` & `gridstatusio-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/
--rw-r--r--   0 root         (0) root         (0)     1461 2023-07-17 14:51:49.000000 gridstatusio-0.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3293 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      883 2023-07-17 14:51:49.000000 gridstatusio-0.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/gridstatusio/
--rw-r--r--   0 root         (0) root         (0)       98 2023-07-17 14:51:49.000000 gridstatusio-0.2.3/gridstatusio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8735 2023-07-17 14:51:49.000000 gridstatusio-0.2.3/gridstatusio/gs_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/gridstatusio/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 14:51:49.000000 gridstatusio-0.2.3/gridstatusio/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1609 2023-07-17 14:51:49.000000 gridstatusio-0.2.3/gridstatusio/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 14:51:49.000000 gridstatusio-0.2.3/gridstatusio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/gridstatusio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3293 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/gridstatusio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      348 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/gridstatusio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/gridstatusio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      237 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/gridstatusio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/gridstatusio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2319 2023-07-17 14:51:49.000000 gridstatusio-0.2.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 14:52:05.000000 gridstatusio-0.2.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-07-21 19:53:58.000000 gridstatusio-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      883 2023-07-21 19:53:58.000000 gridstatusio-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/gridstatusio/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-21 19:53:58.000000 gridstatusio-0.3.0/gridstatusio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9887 2023-07-21 19:53:58.000000 gridstatusio-0.3.0/gridstatusio/gs_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/gridstatusio/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 19:53:58.000000 gridstatusio-0.3.0/gridstatusio/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5334 2023-07-21 19:53:58.000000 gridstatusio-0.3.0/gridstatusio/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 19:53:58.000000 gridstatusio-0.3.0/gridstatusio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/gridstatusio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/gridstatusio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/gridstatusio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/gridstatusio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/gridstatusio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/gridstatusio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-07-21 19:53:58.000000 gridstatusio-0.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/setup.cfg
```

### Comparing `gridstatusio-0.2.3/LICENSE` & `gridstatusio-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gridstatusio-0.2.3/PKG-INFO` & `gridstatusio-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridstatusio
-Version: 0.2.3
+Version: 0.3.0
 Summary: Python Client for GridStatus.io API
 Author-email: Max Kanter <kmax12@gmail.com>
 Maintainer-email: Max Kanter <kmax12@gmail.com>
 License: Copyright 2022 James Max Kanter
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

### Comparing `gridstatusio-0.2.3/README.md` & `gridstatusio-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gridstatusio-0.2.3/gridstatusio/gs_client.py` & `gridstatusio-0.3.0/gridstatusio/gs_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -136,31 +136,43 @@
             return matched_datasets
 
     def get_dataset(
         self,
         dataset,
         start=None,
         end=None,
+        columns=None,
         filter_column=None,
         filter_value=None,
+        filter_operator="=",
         limit=10000,
+        max_rows=None,
         tz=None,
         verbose=False,
     ):
         """Get a dataset from GridStatus.io API
 
         Parameters:
             dataset (str): The name of the dataset to fetch
             start (str): The start time of the data to fetch. If not provided,
                 defaults to the earliest available time for the dataset.
             end (str): The end time of the data to fetch. If not provided,
                 defaults to the latest available time for the dataset.
+            columns (list): The columns to fetch. If not provided,
+                defaults to all available columns.
             filter_column (str): The column to filter on
-            filter_value (str): The value to filter on
+            filter_value (str): The value to filter on. If filter operator is "in",
+                this should be a list of values.
+            filter_operator (str): The operator to use for the filter.
+                Defaults to "=". Possible values are "=",
+                "!=", ">", "<", ">=", "<=", "in".
             limit (int): The maximum number of rows to fetch at time.
+                Defaults to 10000.
+            max_rows (int): The maximum number of rows to fetch.
+                Defaults to None, which fetches all rows that match the request.
             tz (str): The timezone to convert utc timestamps to. Defaults to UTC.
             verbose (bool): If set to True, prints out the number
                 of rows fetched and the time taken to fetch them.
 
         Returns:
             pd.DataFrame: The dataset as a pandas dataframe
         """
@@ -183,19 +195,27 @@
 
             params = {
                 "start_time": start,
                 "end_time": end,
                 "limit": limit,
                 "return_format": "csv",
                 "page": page,
+                "max_rows": max_rows,
             }
             url = f"{self.host}/datasets/{dataset}/query/"
             if filter_column is not None:
+                if isinstance(filter_value, list) and filter_operator == "in":
+                    filter_value = ",".join(filter_value)
+
                 params["filter_column"] = filter_column
                 params["filter_value"] = filter_value
+                params["filter_operator"] = filter_operator
+
+            if columns is not None:
+                params["columns"] = ",".join(columns)
 
             response = self.get(url, params=params, verbose=verbose)
 
             df = pd.read_csv(io.StringIO(response.text))
             dfs.append(df)
 
             has_next_page = response.headers["x-has-next-page"] == "true"
@@ -225,26 +245,31 @@
             f"Average time per page: {round(total_time / (page - 1), 2)} seconds",
             "cyan",
         )
 
         # convert to datetime for any columns that end in _utc
         # or are of type object
         for col in df.columns:
-
             if df[col].dtype == "object" or col.endswith("_utc"):
                 try:
-                    df[col] = pd.to_datetime(df[col], utc=True)
+                    df[col] = pd.to_datetime(
+                        df[col],
+                        format="%Y-%m-%d %H:%M:%S%z",
+                        utc=True,
+                    )
+
+                    if tz != "UTC":
+                        df[col] = df[col].dt.tz_convert(tz)
+                        # rename with _utc suffix
+                        df = df.rename(
+                            columns={col: col.replace("_utc", "") + "_local"},
+                        )
                 except ValueError:
                     pass
 
-                if tz != "UTC":
-                    df[col] = df[col].dt.tz_convert(tz)
-                    # rename with _utc suffix
-                    df = df.rename(columns={col: col.replace("_utc", "") + "_local"})
-
         return df
 
 
 if __name__ == "__main__":
     import os
 
     client = GridStatusClient(api_key=os.getenv("GRIDSTATUS_API_KEY_TEST"))
```

### Comparing `gridstatusio-0.2.3/gridstatusio.egg-info/PKG-INFO` & `gridstatusio-0.3.0/gridstatusio.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridstatusio
-Version: 0.2.3
+Version: 0.3.0
 Summary: Python Client for GridStatus.io API
 Author-email: Max Kanter <kmax12@gmail.com>
 Maintainer-email: Max Kanter <kmax12@gmail.com>
 License: Copyright 2022 James Max Kanter
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

### Comparing `gridstatusio-0.2.3/pyproject.toml` & `gridstatusio-0.3.0/pyproject.toml`

 * *Files identical despite different names*

