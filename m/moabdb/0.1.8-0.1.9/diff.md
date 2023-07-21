# Comparing `tmp/moabdb-0.1.8.tar.gz` & `tmp/moabdb-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moabdb-0.1.8.tar", last modified: Wed Dec  7 17:05:37 2022, max compression
+gzip compressed data, was "moabdb-0.1.9.tar", last modified: Wed Dec  7 17:08:44 2022, max compression
```

## Comparing `moabdb-0.1.8.tar` & `moabdb-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       26 2022-12-06 23:33:09.404552 moabdb-0.1.8/.gitignore
--rw-r--r--   0        0        0     1059 2022-12-06 23:33:09.405052 moabdb-0.1.8/LICENSE
--rw-r--r--   0        0        0       61 2022-12-06 23:33:09.405052 moabdb-0.1.8/README.md
--rw-r--r--   0        0        0      110 2022-12-07 17:05:30.053740 moabdb-0.1.8/moabdb/__init__.py
--rw-r--r--   0        0        0      579 2022-12-06 23:33:09.405553 moabdb-0.1.8/moabdb/globals.py
--rw-r--r--   0        0        0     3965 2022-12-07 17:05:22.117511 moabdb-0.1.8/moabdb/lib.py
--rw-r--r--   0        0        0     6783 2022-12-06 23:33:09.406054 moabdb-0.1.8/moabdb/protocol_pb2.py
--rw-r--r--   0        0        0     2340 2022-12-07 17:04:22.236241 moabdb-0.1.8/moabdb/timewindows.py
--rw-r--r--   0        0        0      500 2022-12-06 23:33:09.406554 moabdb-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      587 2022-12-06 23:33:09.407054 moabdb-0.1.8/tests/test.py
--rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 moabdb-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       26 2022-12-06 23:33:09.404552 moabdb-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1059 2022-12-06 23:33:09.405052 moabdb-0.1.9/LICENSE
+-rw-r--r--   0        0        0       61 2022-12-06 23:33:09.405052 moabdb-0.1.9/README.md
+-rw-r--r--   0        0        0      110 2022-12-07 17:08:14.731859 moabdb-0.1.9/moabdb/__init__.py
+-rw-r--r--   0        0        0      579 2022-12-06 23:33:09.405553 moabdb-0.1.9/moabdb/globals.py
+-rw-r--r--   0        0        0     3965 2022-12-07 17:05:22.117511 moabdb-0.1.9/moabdb/lib.py
+-rw-r--r--   0        0        0     6783 2022-12-06 23:33:09.406054 moabdb-0.1.9/moabdb/protocol_pb2.py
+-rw-r--r--   0        0        0     2345 2022-12-07 17:08:09.212180 moabdb-0.1.9/moabdb/timewindows.py
+-rw-r--r--   0        0        0      500 2022-12-06 23:33:09.406554 moabdb-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      587 2022-12-06 23:33:09.407054 moabdb-0.1.9/tests/test.py
+-rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 moabdb-0.1.9/PKG-INFO
```

### Comparing `moabdb-0.1.8/LICENSE` & `moabdb-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `moabdb-0.1.8/moabdb/globals.py` & `moabdb-0.1.9/moabdb/globals.py`

 * *Files identical despite different names*

### Comparing `moabdb-0.1.8/moabdb/lib.py` & `moabdb-0.1.9/moabdb/lib.py`

 * *Files identical despite different names*

### Comparing `moabdb-0.1.8/moabdb/protocol_pb2.py` & `moabdb-0.1.9/moabdb/protocol_pb2.py`

 * *Files identical despite different names*

### Comparing `moabdb-0.1.8/moabdb/timewindows.py` & `moabdb-0.1.9/moabdb/timewindows.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         new_time = base_timestamp + pd.DateOffset(weeks=tm_freq)
     elif str.upper(tm_unit) == 'M':
         new_time = base_timestamp + pd.DateOffset(months=tm_freq)
     elif str.upper(tm_unit) == 'Y':
         new_time = base_timestamp + pd.DateOffset(years=tm_freq)
     else:
         print("Unknown time unit, accepts: D, W, M, Y")
-    return(new_time.timestamp())
+    return(int(new_time.timestamp()))
 
 def _get_unix_dates(sample_len, start_dt, end_dt):
     # User provided sample length ...
 
     # ... but didn't provide anything else --> get recent sample
     if (end_dt is None) & (start_dt is None):
         today = datetime.now().strftime("%Y-%m-%d")
```

### Comparing `moabdb-0.1.8/tests/test.py` & `moabdb-0.1.9/tests/test.py`

 * *Files identical despite different names*

