# Comparing `tmp/zit-0.0.3a8.tar.gz` & `tmp/zit-0.0.3a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zit-0.0.3a8.tar", max compression
+gzip compressed data, was "zit-0.0.3a9.tar", max compression
```

## Comparing `zit-0.0.3a8.tar` & `zit-0.0.3a9.tar`

### file list

```diff
@@ -1,25 +1,20 @@
--rw-r--r--   0        0        0     1018 2023-07-13 15:00:21.846189 zit-0.0.3a8/pyproject.toml
--rw-r--r--   0        0        0       72 2022-01-10 03:44:16.795928 zit-0.0.3a8/zit/__init__.py
--rw-r--r--   0        0        0     1544 2023-04-14 12:30:48.576605 zit-0.0.3a8/zit/auth.py
--rw-r--r--   0        0        0      582 2023-07-07 04:26:24.431211 zit-0.0.3a8/zit/config.py
--rw-r--r--   0        0        0     8607 2023-07-10 18:46:59.264897 zit-0.0.3a8/zit/dashboard.py
--rw-r--r--   0        0        0       60 2023-06-15 21:58:13.307052 zit-0.0.3a8/zit/dataset/__init__.py
--rw-r--r--   0        0        0      407 2023-05-11 08:42:13.675272 zit-0.0.3a8/zit/dataset/build.py
--rw-r--r--   0        0        0        0 2023-06-15 21:56:33.152907 zit-0.0.3a8/zit/dataset/classification.py
--rw-r--r--   0        0        0     2029 2023-06-15 17:30:11.785818 zit-0.0.3a8/zit/dataset/convert.py
--rw-r--r--   0        0        0     1773 2023-07-13 14:23:28.427050 zit-0.0.3a8/zit/dataset/detection.py
--rw-r--r--   0        0        0      427 2023-05-11 07:24:56.576494 zit-0.0.3a8/zit/dataset/factory.py
--rw-r--r--   0        0        0        0 2023-05-11 05:37:14.408208 zit-0.0.3a8/zit/dataset/keypoints.py
--rw-r--r--   0        0        0    15749 2023-07-10 23:17:00.512707 zit-0.0.3a8/zit/dataset/manager.py
--rw-r--r--   0        0        0        0 2023-05-11 05:37:56.638196 zit-0.0.3a8/zit/dataset/multilabel_classification.py
--rw-r--r--   0        0        0        0 2023-05-11 05:36:54.588213 zit-0.0.3a8/zit/dataset/segmentation.py
--rw-r--r--   0        0        0    12010 2023-07-07 20:00:48.386764 zit-0.0.3a8/zit/formula.py
--rw-r--r--   0        0        0      617 2023-04-16 19:16:58.258259 zit-0.0.3a8/zit/main.py
--rw-r--r--   0        0        0      753 2023-07-12 06:53:22.944703 zit-0.0.3a8/zit/routes/__init__.py
--rw-r--r--   0        0        0      520 2023-06-18 22:26:38.078376 zit-0.0.3a8/zit/routes/dataset/annotations.py
--rw-r--r--   0        0        0      831 2023-06-18 22:58:55.749634 zit-0.0.3a8/zit/routes/dataset/categories.py
--rw-r--r--   0        0        0     3214 2023-06-18 21:57:11.118740 zit-0.0.3a8/zit/routes/dataset/images.py
--rw-r--r--   0        0        0     2358 2023-07-12 06:52:27.144711 zit-0.0.3a8/zit/routes/dataset/queries.py
--rw-r--r--   0        0        0      402 2023-07-13 14:58:24.916231 zit-0.0.3a8/zit/utils.py
--rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 zit-0.0.3a8/setup.py
--rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 zit-0.0.3a8/PKG-INFO
+-rw-r--r--   0        0        0     1018 2023-07-16 11:38:16.303174 zit-0.0.3a9/pyproject.toml
+-rw-r--r--   0        0        0       72 2022-01-10 03:44:16.795928 zit-0.0.3a9/zit/__init__.py
+-rw-r--r--   0        0        0     1544 2023-04-14 12:30:48.576605 zit-0.0.3a9/zit/auth.py
+-rw-r--r--   0        0        0      582 2023-07-07 04:26:24.431211 zit-0.0.3a9/zit/config.py
+-rw-r--r--   0        0        0     8607 2023-07-10 18:46:59.264897 zit-0.0.3a9/zit/dashboard.py
+-rw-r--r--   0        0        0       36 2023-07-16 11:33:53.583239 zit-0.0.3a9/zit/dataset/__init__.py
+-rw-r--r--   0        0        0     2070 2023-07-16 11:28:27.353317 zit-0.0.3a9/zit/dataset/build.py
+-rw-r--r--   0        0        0     2029 2023-06-15 17:30:11.785818 zit-0.0.3a9/zit/dataset/convert.py
+-rw-r--r--   0        0        0      639 2023-07-16 11:33:44.383241 zit-0.0.3a9/zit/dataset/factory.py
+-rw-r--r--   0        0        0    17219 2023-07-15 06:21:08.965297 zit-0.0.3a9/zit/dataset/manager.py
+-rw-r--r--   0        0        0    12010 2023-07-07 20:00:48.386764 zit-0.0.3a9/zit/formula.py
+-rw-r--r--   0        0        0      617 2023-04-16 19:16:58.258259 zit-0.0.3a9/zit/main.py
+-rw-r--r--   0        0        0      753 2023-07-12 06:53:22.944703 zit-0.0.3a9/zit/routes/__init__.py
+-rw-r--r--   0        0        0      520 2023-06-18 22:26:38.078376 zit-0.0.3a9/zit/routes/dataset/annotations.py
+-rw-r--r--   0        0        0      831 2023-06-18 22:58:55.749634 zit-0.0.3a9/zit/routes/dataset/categories.py
+-rw-r--r--   0        0        0     3214 2023-06-18 21:57:11.118740 zit-0.0.3a9/zit/routes/dataset/images.py
+-rw-r--r--   0        0        0     2519 2023-07-15 06:21:37.415290 zit-0.0.3a9/zit/routes/dataset/queries.py
+-rw-r--r--   0        0        0      402 2023-07-13 14:58:24.916231 zit-0.0.3a9/zit/utils.py
+-rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 zit-0.0.3a9/setup.py
+-rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 zit-0.0.3a9/PKG-INFO
```

### Comparing `zit-0.0.3a8/pyproject.toml` & `zit-0.0.3a9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zit"
-version = "0.0.3a8"
+version = "0.0.3a9"
 description = "ZitySpace CLI tool"
 authors = ["Rui Zheng <rui@zityspace.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 PyYAML = "^6.0"
@@ -46,10 +46,10 @@
 
 [tool.isort]
 profile = "black"
 skip = ["dist"]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.0.3a8"
+version = "0.0.3a9"
 version_files = ["pyproject.toml:version"]
 tag_format = "v$version"
```

### Comparing `zit-0.0.3a8/zit/auth.py` & `zit-0.0.3a9/zit/auth.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a8/zit/config.py` & `zit-0.0.3a9/zit/config.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a8/zit/dashboard.py` & `zit-0.0.3a9/zit/dashboard.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a8/zit/dataset/convert.py` & `zit-0.0.3a9/zit/dataset/convert.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a8/zit/dataset/manager.py` & `zit-0.0.3a9/zit/dataset/manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,26 @@
         self.anno_db = os.path.join(root_path, "anno.db")
         self.anno_df = None
 
         if task == "classification":
             self.required_fields = ["image_hash", "category"]
             self.unique_fields = ["image_hash"]
 
+        elif task == "multilabel_classification":
+            self.required_fields = ["image_hash", "categories"]
+            self.unique_fields = ["image_hash"]
+
+        elif task == "box_classification":
+            self.required_fields = ["image_hash", "x", "y", "w", "h", "category"]
+            self.unique_fields = ["image_hash", "x", "y", "w", "h"]
+
+        elif task == "box_multilabel_classification":
+            self.required_fields = ["image_hash", "x", "y", "w", "h", "categories"]
+            self.unique_fields = ["image_hash", "x", "y", "w", "h"]
+
         elif task == "detection":
             self.required_fields = ["image_hash", "x", "y", "w", "h", "category"]
             self.unique_fields = ["image_hash", "x", "y", "w", "h"]
 
         elif task == "instance_segmentation":
             # format refers to: polygon / rle / binary
             self.required_fields = ["image_hash", "mask", "category", "format"]
@@ -164,26 +176,38 @@
         records = self._transform_records(records)
 
         self.connect_db()
 
         if not self._table_exists("anno"):
             # create anno table here, this happens when annotate from scratch and sync annotations
             # to backend the first time
-            if self.task == "detection":
+            if self.task in ["detection", "box_classification"]:
                 self.cursor.execute(
                     "CREATE TABLE anno(image_hash VARCHAR, x INTEGER, y INTEGER, w INTEGER, h INTEGER, "
                     "category VARCHAR, timestamp_z VARCHAR, unique_hash_z VARCHAR)"
                 )
 
             elif self.task == "classification":
                 self.cursor.execute(
                     "CREATE TABLE anno(image_hash VARCHAR, category VARCHAR, timestamp_z VARCHAR, "
                     "unique_hash_z VARCHAR)"
                 )
 
+            elif self.task == "multilabel_classification":
+                self.cursor.execute(
+                    "CREATE TABLE anno(image_hash VARCHAR, categories VARCHAR, timestamp_z VARCHAR, "
+                    "unique_hash_z VARCHAR)"
+                )
+
+            elif self.task == "box_multilabel_classification":
+                self.cursor.execute(
+                    "CREATE TABLE anno(image_hash VARCHAR, x INTEGER, y INTEGER, w INTEGER, h INTEGER, "
+                    "categories VARCHAR, timestamp_z VARCHAR, unique_hash_z VARCHAR)"
+                )
+
             elif self.task == "instance_segmentation":
                 self.cursor.execute(
                     "CREATE TABLE anno(image_hash VARCHAR, mask STRUCT(closed BOOLEAN, hole BOOLEAN, points"
                     " DOUBLE[])[], category VARCHAR, format VARCHAR, timestamp_z VARCHAR, unique_hash_z VARCHAR)"
                 )
 
             elif self.task == "keypoints_detection":
@@ -217,15 +241,18 @@
         if not self._table_exists("anno") or not len(image_hashes):
             self.close_db()
             return {} if return_dict else pd.DataFrame()
 
         image_hashes_str = ", ".join([f"'{h}'" for h in image_hashes])
         res = self.cursor.execute(f"select * from anno where image_hash in ({image_hashes_str})").fetchdf()
 
-        if self.task == "detection":
+        if self.task in ["classification", "multilabel_classification"]:
+            res["type"] = "image"
+
+        elif self.task in ["detection", "box_classification", "box_multilabel_classification"]:
             res["type"] = "box"
 
         elif self.task == "instance_segmentation":
             res["type"] = "mask"
 
         elif self.task == "keypoints_detection":
             res["type"] = "keypoints"
@@ -281,14 +308,17 @@
     ):
         self.connect_db()
 
         if not self._table_exists("anno"):
             self.close_db()
             return
 
+        # TODO: multilabel classification
+
+        # single label classification
         self.cursor.execute(
             "update anno set category = ?, timestamp_z = ? where category = ?", [new_category, at, category]
         )
 
         if self.serving:
             self.anno_df = self.cursor.execute("select * from anno").fetchdf()
 
@@ -306,18 +336,21 @@
                     status_code=400,
                     detail=f"field {field} is required for task: {self.task}",
                 )
 
     def _sanitycheck_file(self, file_path: str):
         suffix = os.path.splitext(file_path)[1][1:]
 
-        if self.task == "classification":
-            raise NotImplementedError("classification task annotation file sanity check not implemented yet")
-
-        elif self.task == "detection":
+        if self.task in [
+            "classification",
+            "box_classification",
+            "multilabel_classification",
+            "box_multilabel_classification",
+            "detection",
+        ]:
             if suffix not in ["csv", "parquet"]:
                 raise HTTPException(
                     status_code=400,
                     detail=f"{file_path} not in one of the supported formats: csv, parquet",
                 )
 
         elif self.task in ["instance_segmentation", "keypoints_detection"]:
@@ -427,14 +460,16 @@
                             "unique_hash_z": anno["unique_hash_z"],
                         }
                     )
 
         else:
             records_ = [anno | {"image_hash": rec["image_hash"]} for rec in records for anno in rec["annotations"]]
 
+        # TODO multilabel classification
+
         if records_:
             # ensure required fields are present
             for field in self.required_fields:
                 if field not in records_[0]:
                     raise HTTPException(
                         status_code=400,
                         detail=f"field {field} is missing in annotation records",
```

### Comparing `zit-0.0.3a8/zit/formula.py` & `zit-0.0.3a9/zit/formula.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a8/zit/main.py` & `zit-0.0.3a9/zit/main.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a8/zit/routes/__init__.py` & `zit-0.0.3a9/zit/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a8/zit/routes/dataset/annotations.py` & `zit-0.0.3a9/zit/routes/dataset/annotations.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a8/zit/routes/dataset/categories.py` & `zit-0.0.3a9/zit/routes/dataset/categories.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a8/zit/routes/dataset/images.py` & `zit-0.0.3a9/zit/routes/dataset/images.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a8/zit/routes/dataset/queries.py` & `zit-0.0.3a9/zit/routes/dataset/queries.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,15 +29,18 @@
 
 
 def build_queries_router(params, manager: Manager, meta_serving: bool = False):
     queries_router = r = APIRouter(tags=["Dataset: Dataframe queries"])
 
     df = manager.anno_df.copy()
 
-    if manager.task == "detection":
+    if manager.task in ["classification", "multilabel_classification"]:
+        df["type"] = "image"
+
+    elif manager.task in ["detection", "box_classification", "box_multilabel_classification"]:
         df["type"] = "box"
 
     elif manager.task == "instance_segmentation":
         df["type"] = "mask"
 
     elif manager.task == "keypoints_detection":
         df["type"] = "keypoints"
```

### Comparing `zit-0.0.3a8/setup.py` & `zit-0.0.3a9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'websocket-client>=1.5.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['zit = zit.main:app']}
 
 setup_kwargs = {
     'name': 'zit',
-    'version': '0.0.3a8',
+    'version': '0.0.3a9',
     'description': 'ZitySpace CLI tool',
     'long_description': 'None',
     'author': 'Rui Zheng',
     'author_email': 'rui@zityspace.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `zit-0.0.3a8/PKG-INFO` & `zit-0.0.3a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zit
-Version: 0.0.3a8
+Version: 0.0.3a9
 Summary: ZitySpace CLI tool
 License: MIT
 Author: Rui Zheng
 Author-email: rui@zityspace.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

