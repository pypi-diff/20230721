# Comparing `tmp/gtfs_kit-5.2.7.tar.gz` & `tmp/gtfs_kit-5.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtfs_kit-5.2.7.tar", max compression
+gzip compressed data, was "gtfs_kit-5.2.8.tar", max compression
```

## Comparing `gtfs_kit-5.2.7.tar` & `gtfs_kit-5.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1083 2023-03-22 02:01:30.167750 gtfs_kit-5.2.7/LICENSE.txt
--rw-r--r--   0        0        0     1937 2023-03-22 02:57:07.660723 gtfs_kit-5.2.7/README.rst
--rw-r--r--   0        0        0      304 2023-06-06 00:32:33.259560 gtfs_kit-5.2.7/gtfs_kit/__init__.py
--rw-r--r--   0        0        0     3426 2023-03-22 02:01:30.171750 gtfs_kit-5.2.7/gtfs_kit/calendar.py
--rw-r--r--   0        0        0    10692 2023-03-22 02:01:30.171750 gtfs_kit-5.2.7/gtfs_kit/cleaners.py
--rw-r--r--   0        0        0     6971 2023-03-22 02:01:30.171750 gtfs_kit-5.2.7/gtfs_kit/constants.py
--rw-r--r--   0        0        0    16515 2023-03-22 02:01:30.171750 gtfs_kit-5.2.7/gtfs_kit/feed.py
--rw-r--r--   0        0        0    20051 2023-06-06 00:32:33.259560 gtfs_kit-5.2.7/gtfs_kit/helpers.py
--rw-r--r--   0        0        0    35644 2023-04-26 03:24:57.537534 gtfs_kit-5.2.7/gtfs_kit/miscellany.py
--rw-r--r--   0        0        0    30517 2023-06-05 22:22:06.252172 gtfs_kit-5.2.7/gtfs_kit/routes.py
--rw-r--r--   0        0        0     6648 2023-03-22 02:01:30.171750 gtfs_kit-5.2.7/gtfs_kit/shapes.py
--rw-r--r--   0        0        0     6231 2023-03-22 02:01:30.171750 gtfs_kit-5.2.7/gtfs_kit/stop_times.py
--rw-r--r--   0        0        0    24935 2023-03-22 02:01:30.171750 gtfs_kit-5.2.7/gtfs_kit/stops.py
--rw-r--r--   0        0        0    21337 2023-03-22 02:01:30.171750 gtfs_kit-5.2.7/gtfs_kit/trips.py
--rw-r--r--   0        0        0    49077 2023-03-22 02:01:30.171750 gtfs_kit-5.2.7/gtfs_kit/validators.py
--rw-r--r--   0        0        0     1097 2023-06-06 00:32:33.259560 gtfs_kit-5.2.7/pyproject.toml
--rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 gtfs_kit-5.2.7/setup.py
--rw-r--r--   0        0        0     2926 1970-01-01 00:00:00.000000 gtfs_kit-5.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1083 2020-01-09 20:55:35.590106 gtfs_kit-5.2.8/LICENSE.txt
+-rw-r--r--   0        0        0     1937 2023-04-27 00:05:00.839952 gtfs_kit-5.2.8/README.rst
+-rw-r--r--   0        0        0      304 2023-07-21 01:27:30.175028 gtfs_kit-5.2.8/gtfs_kit/__init__.py
+-rw-r--r--   0        0        0     3426 2021-04-28 23:42:59.436692 gtfs_kit-5.2.8/gtfs_kit/calendar.py
+-rw-r--r--   0        0        0    10692 2022-04-12 04:10:10.474482 gtfs_kit-5.2.8/gtfs_kit/cleaners.py
+-rw-r--r--   0        0        0     6971 2022-01-17 03:01:47.667252 gtfs_kit-5.2.8/gtfs_kit/constants.py
+-rw-r--r--   0        0        0    16515 2022-04-13 02:04:39.526021 gtfs_kit-5.2.8/gtfs_kit/feed.py
+-rw-r--r--   0        0        0    20051 2023-07-21 01:27:30.175028 gtfs_kit-5.2.8/gtfs_kit/helpers.py
+-rw-r--r--   0        0        0    35644 2023-04-27 00:05:00.843952 gtfs_kit-5.2.8/gtfs_kit/miscellany.py
+-rw-r--r--   0        0        0    30642 2023-07-21 01:27:30.175028 gtfs_kit-5.2.8/gtfs_kit/routes.py
+-rw-r--r--   0        0        0     6648 2022-07-05 02:59:12.080231 gtfs_kit-5.2.8/gtfs_kit/shapes.py
+-rw-r--r--   0        0        0     6231 2022-04-13 02:04:39.526021 gtfs_kit-5.2.8/gtfs_kit/stop_times.py
+-rw-r--r--   0        0        0    24935 2022-04-26 01:06:51.650776 gtfs_kit-5.2.8/gtfs_kit/stops.py
+-rw-r--r--   0        0        0    21337 2021-11-25 21:52:10.392179 gtfs_kit-5.2.8/gtfs_kit/trips.py
+-rw-r--r--   0        0        0    49351 2023-07-21 01:27:30.175028 gtfs_kit-5.2.8/gtfs_kit/validators.py
+-rw-r--r--   0        0        0     1105 2023-07-21 01:27:30.179028 gtfs_kit-5.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 gtfs_kit-5.2.8/setup.py
+-rw-r--r--   0        0        0     2926 1970-01-01 00:00:00.000000 gtfs_kit-5.2.8/PKG-INFO
```

### Comparing `gtfs_kit-5.2.7/LICENSE.txt` & `gtfs_kit-5.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.7/README.rst` & `gtfs_kit-5.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.7/gtfs_kit/calendar.py` & `gtfs_kit-5.2.8/gtfs_kit/calendar.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.7/gtfs_kit/cleaners.py` & `gtfs_kit-5.2.8/gtfs_kit/cleaners.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.7/gtfs_kit/constants.py` & `gtfs_kit-5.2.8/gtfs_kit/constants.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.7/gtfs_kit/feed.py` & `gtfs_kit-5.2.8/gtfs_kit/feed.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.7/gtfs_kit/helpers.py` & `gtfs_kit-5.2.8/gtfs_kit/helpers.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.7/gtfs_kit/miscellany.py` & `gtfs_kit-5.2.8/gtfs_kit/miscellany.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.7/gtfs_kit/routes.py` & `gtfs_kit-5.2.8/gtfs_kit/routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     *,
     split_directions: bool = False,
 ) -> pd.DataFrame:
     """
     Compute stats for the given subset of trips stats (of the form output by the
     function :func:`.trips.compute_trip_stats`).
 
+    Ignore trips with zero duration, because they are defunct.
+
     If ``split_directions``, then separate the stats by trip direction (0 or 1).
     Use the headway start and end times to specify the time period for computing
     headway stats.
 
     Return a DataFrame with the columns
 
     - ``'route_id'``
@@ -90,16 +92,18 @@
 
     Raise a ValueError if ``split_directions`` and no non-NaN
     direction ID values present
     """
     if trip_stats_subset.empty:
         return pd.DataFrame()
 
+    # Remove defunct trips
+    f = trip_stats_subset.loc[lambda x: x["duration"] > 0].copy()
+
     # Convert trip start and end times to seconds to ease calculations below
-    f = trip_stats_subset.copy()
     f[["start_time", "end_time"]] = f[["start_time", "end_time"]].applymap(
         hp.timestr_to_seconds
     )
 
     headway_start = hp.timestr_to_seconds(headway_start_time)
     headway_end = hp.timestr_to_seconds(headway_end_time)
```

### Comparing `gtfs_kit-5.2.7/gtfs_kit/shapes.py` & `gtfs_kit-5.2.8/gtfs_kit/shapes.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.7/gtfs_kit/stop_times.py` & `gtfs_kit-5.2.8/gtfs_kit/stop_times.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.7/gtfs_kit/stops.py` & `gtfs_kit-5.2.8/gtfs_kit/stops.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.7/gtfs_kit/trips.py` & `gtfs_kit-5.2.8/gtfs_kit/trips.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.7/gtfs_kit/validators.py` & `gtfs_kit-5.2.8/gtfs_kit/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -636,48 +636,52 @@
 
     # Check trip_id
     problems = check_column_linked_id(
         problems, table, f, "trip_id", feed.trips, column_required=False
     )
 
     # Check combination of agency_id, route_id, trip_id
-    f["flag1"] = (
-        f.agency_id.notna().astype(int)
-        + f.route_id.notna().astype(int)
-        + f.trip_id.notna().astype(int)
-    )
-    cond = lambda x: x.flag1 > 1
-    problems = check_table(
-        problems,
-        table,
-        f,
-        cond,
-        "At most one of agency_id, route_id, trip_id can be given",
-    )
+    if {"agency_id", "route_id", "trip_id"} <= set(f.columns):
+        f["flag1"] = (
+            f["agency_id"].notna().astype(int)
+            + f["route_id"].notna().astype(int)
+            + f["trip_id"].notna().astype(int)
+        )
+        cond = lambda x: x.flag1 > 1
+        problems = check_table(
+            problems,
+            table,
+            f,
+            cond,
+            "At most one of agency_id, route_id, trip_id can be given",
+        )
 
     # Check organization_name
     problems = check_column(problems, table, f, "organization_name", valid_str)
 
     # Check is_producer, is_consumer, is_authority
     v = lambda x: pd.isna(x) or x in range(2)
     for col in ["is_producer", "is_operator", "is_authority"]:
         problems = check_column(problems, table, f, col, v, column_required=False)
 
     # Check combination of is_producer, is_consumer, is_authority
-    f["flag2"] = (
-        f.is_producer.fillna(0) + f.is_operator.fillna(0) + f.is_authority.fillna(0)
-    )
-    cond = lambda x: x.flag2 < 1
-    problems = check_table(
-        problems,
-        table,
-        f,
-        cond,
-        "At least one of is_producer, is_operator, or is_authority must be 1",
-    )
+    if {"is_producer", "is_operator", "is_authority"} <= set(f.columns):
+        f["flag2"] = (
+            f["is_producer"].fillna(0)
+            + f["is_operator"].fillna(0)
+            + f["is_authority"].fillna(0)
+        )
+        cond = lambda x: x.flag2 < 1
+        problems = check_table(
+            problems,
+            table,
+            f,
+            cond,
+            "At least one of is_producer, is_operator, or is_authority must be 1",
+        )
 
     # Check attribution_url
     problems = check_column(
         problems, table, f, "attribution_url", valid_url, column_required=False
     )
 
     # Check attribution_email
```

### Comparing `gtfs_kit-5.2.7/pyproject.toml` & `gtfs_kit-5.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gtfs_kit"
-version = "5.2.7"
+version = "5.2.8"
 description = "A Python 3.8+ library for analyzing GTFS feeds."
 authors = ["Alex Raichev <araichev@mrcagney.com>"]
 readme = "README.rst"
 license = "MIT"
 repository = "https://github.com/mrcagney/gtfs_kit"
 documentation = "https://mrcagney.github.io/gtfs_kit_docs"
 exclude = ["tests", "docs"]
@@ -42,8 +42,8 @@
     "slow: marks tests as slow (deselect with '-m \"not slow\"')",
     "serial",
 ]
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
 select = ["E", "F"]
-ignore = ["E501", "F401", "F403"]
+ignore = ["E501", "E731", "F401", "F403"]
```

### Comparing `gtfs_kit-5.2.7/setup.py` & `gtfs_kit-5.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'requests>=2',
  'rtree>=0',
  'shapely>=1.8',
  'utm>=0.6']
 
 setup_kwargs = {
     'name': 'gtfs-kit',
-    'version': '5.2.7',
+    'version': '5.2.8',
     'description': 'A Python 3.8+ library for analyzing GTFS feeds.',
     'long_description': "GTFS Kit\n********\n.. image:: https://github.com/mrcagney/gtfs_kit/actions/workflows/test.yml/badge.svg\n\nGTFS Kit is a Python 3.8+ library for analyzing `General Transit Feed Specification (GTFS) <https://en.wikipedia.org/wiki/GTFS>`_ data in memory without a database.\nIt uses Pandas and Shapely to do the heavy lifting.\n\n\nInstallation\n=============\n``poetry add gtfs_kit``.\n\n\nExamples\n========\nYou can find examples in the Jupyter notebook ``notebooks/examples.ipynb``.\n\n\nAuthors\n=========\n- Alex Raichev (2019-09), maintainer\n\n\nDocumentation\n=============\nDocumentation is built via Sphinx from the source code in the ``docs`` directory then published to Github Pages at `mrcagney.github.io/gtfs_kit_docs <https://mrcagney.github.io/gtfs_kit_docs>`_.\n\n\nNotes\n=====\n- This project's development status is Alpha.\n  I use GTFS Kit for work and change it breakingly to suit my needs.\n- This project uses semantic versioning.\n- I aim for GTFS Kit to handle `the current GTFS <https://developers.google.com/transit/gtfs/reference>`_.\n  In particular, i avoid handling `GTFS extensions <https://developers.google.com/transit/gtfs/reference/gtfs-extensions>`_.\n  That is the most reasonable scope boundary i can draw at present, given this project's tiny budget.\n  If you would like to fund me to expand that scope, feel free to email me.\n- Thanks to `MRCagney <http://www.mrcagney.com/>`_ for periodically donating to this project.\n- Constructive feedback and contributions are welcome.\n  Please issue pull requests from a feature branch into the ``develop`` branch and include tests.\n- GTFS time is measured relative noon minus 12 hours, which can mess things up when crossing into daylight savings time.\n  I don't think this issue causes any bugs in GTFS Kit, but you and i have been warned.\n  Thanks to user derhuerst for bringing this to my attention in `closed Issue 8 <https://github.com/mrcagney/gtfs_kit/issues/8#issue-1063633457>`_.\n",
     'author': 'Alex Raichev',
     'author_email': 'araichev@mrcagney.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mrcagney/gtfs_kit',
```

### Comparing `gtfs_kit-5.2.7/PKG-INFO` & `gtfs_kit-5.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtfs-kit
-Version: 5.2.7
+Version: 5.2.8
 Summary: A Python 3.8+ library for analyzing GTFS feeds.
 Home-page: https://github.com/mrcagney/gtfs_kit
 License: MIT
 Author: Alex Raichev
 Author-email: araichev@mrcagney.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
```

