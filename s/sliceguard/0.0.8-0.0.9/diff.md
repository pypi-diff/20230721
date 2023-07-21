# Comparing `tmp/sliceguard-0.0.8.tar.gz` & `tmp/sliceguard-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliceguard-0.0.8.tar", last modified: Wed Jul 19 11:05:23 2023, max compression
+gzip compressed data, was "sliceguard-0.0.9.tar", last modified: Fri Jul 21 13:23:50 2023, max compression
```

## Comparing `sliceguard-0.0.8.tar` & `sliceguard-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-19 11:05:23.093813 sliceguard-0.0.8/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1065 2023-06-14 07:59:41.000000 sliceguard-0.0.8/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4245 2023-07-19 11:05:23.093813 sliceguard-0.0.8/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3590 2023-07-19 11:03:05.000000 sliceguard-0.0.8/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1088 2023-07-19 11:03:35.000000 sliceguard-0.0.8/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-19 11:05:23.093813 sliceguard-0.0.8/setup.cfg
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-19 11:05:23.093813 sliceguard-0.0.8/sliceguard/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       44 2023-07-05 08:28:25.000000 sliceguard-0.0.8/sliceguard/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    10000 2023-07-19 11:03:05.000000 sliceguard-0.0.8/sliceguard/detection.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4985 2023-07-19 11:03:05.000000 sliceguard-0.0.8/sliceguard/embedding_utils.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4378 2023-07-11 15:29:58.000000 sliceguard-0.0.8/sliceguard/explanation.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    11179 2023-07-19 11:03:05.000000 sliceguard-0.0.8/sliceguard/sliceguard.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     8800 2023-07-19 11:03:05.000000 sliceguard-0.0.8/sliceguard/utils.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-19 11:05:23.093813 sliceguard-0.0.8/sliceguard.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4245 2023-07-19 11:05:23.000000 sliceguard-0.0.8/sliceguard.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      374 2023-07-19 11:05:23.000000 sliceguard-0.0.8/sliceguard.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-19 11:05:23.000000 sliceguard-0.0.8/sliceguard.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      264 2023-07-19 11:05:23.000000 sliceguard-0.0.8/sliceguard.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2023-07-19 11:05:23.000000 sliceguard-0.0.8/sliceguard.egg-info/top_level.txt
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-19 11:05:23.093813 sliceguard-0.0.8/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4742 2023-07-11 15:29:58.000000 sliceguard-0.0.8/tests/test_sliceguard.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-21 13:23:50.351456 sliceguard-0.0.9/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1065 2023-06-14 07:59:41.000000 sliceguard-0.0.9/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4059 2023-07-21 13:23:50.351456 sliceguard-0.0.9/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3404 2023-07-21 13:21:02.000000 sliceguard-0.0.9/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1088 2023-07-21 13:23:08.000000 sliceguard-0.0.9/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-21 13:23:50.351456 sliceguard-0.0.9/setup.cfg
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-21 13:23:50.351456 sliceguard-0.0.9/sliceguard/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       44 2023-07-05 08:28:25.000000 sliceguard-0.0.9/sliceguard/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     8994 2023-07-21 13:21:02.000000 sliceguard-0.0.9/sliceguard/detection.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4985 2023-07-19 11:03:05.000000 sliceguard-0.0.9/sliceguard/embedding_utils.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4151 2023-07-21 13:21:02.000000 sliceguard-0.0.9/sliceguard/explanation.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    10689 2023-07-21 13:21:02.000000 sliceguard-0.0.9/sliceguard/sliceguard.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     8800 2023-07-19 11:03:05.000000 sliceguard-0.0.9/sliceguard/utils.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-21 13:23:50.351456 sliceguard-0.0.9/sliceguard.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4059 2023-07-21 13:23:50.000000 sliceguard-0.0.9/sliceguard.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      374 2023-07-21 13:23:50.000000 sliceguard-0.0.9/sliceguard.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-21 13:23:50.000000 sliceguard-0.0.9/sliceguard.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      264 2023-07-21 13:23:50.000000 sliceguard-0.0.9/sliceguard.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2023-07-21 13:23:50.000000 sliceguard-0.0.9/sliceguard.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-21 13:23:50.351456 sliceguard-0.0.9/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4742 2023-07-11 15:29:58.000000 sliceguard-0.0.9/tests/test_sliceguard.py
```

### Comparing `sliceguard-0.0.8/LICENSE` & `sliceguard-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.8/PKG-INFO` & `sliceguard-0.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliceguard
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library for detecting critical data slices in structured and unstructured data based on features, metadata and model predictions.
 Author-email: Renumics GmbH <info@renumics.com>, Daniel Klitzke <daniel.klitzke@renumics.com>
 Project-URL: Homepage, https://github.com/Renumics/sliceguard
 Project-URL: Bug Tracker, https://github.com/Renumics/sliceguard/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -62,20 +62,17 @@
 )
 sg.report()
 ```
 
 ## 🔧 Use case-specific examples
 * [Detecting issues in automatic speech recognition (ASR) models](examples/audio_issues_commonvoice_whisper.ipynb)
 * [Detecting issues in audio datasets (condition monitoring)](examples/audio_issues_condition_monitoring_dcase.ipynb)
+* [Selecting the best (and worst) generated images of Stable Diffusion](examples/stable_diffusion_evaluation.ipynb)
 
 
-Also check this post on Medium:
-
-[Evaluating automatic speech recognition models beyond global metrics — A tutorial using OpenAI’s Whisper as an example](https://medium.com/@daniel-klitzke/evaluating-automatic-speech-recognition-models-beyond-global-metrics-a-tutorial-using-openais-54b63c4dadbd)
-
 ## 🗺️ Public Roadmap
 - [x] Detection of problematic data slices
 - [x] Basic explanation of found issues via feature importances
 - [x] Limited embedding computation for images, audio, text
 - [x] Extended embedding support, e.g., more embedding models and allow precomputed embeddings
 - [x] Speed up embedding computation using datasets library
 - [ ] Soft Dependencies for embedding computation as torch dependencies are large
```

### Comparing `sliceguard-0.0.8/README.md` & `sliceguard-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -48,20 +48,17 @@
 )
 sg.report()
 ```
 
 ## 🔧 Use case-specific examples
 * [Detecting issues in automatic speech recognition (ASR) models](examples/audio_issues_commonvoice_whisper.ipynb)
 * [Detecting issues in audio datasets (condition monitoring)](examples/audio_issues_condition_monitoring_dcase.ipynb)
+* [Selecting the best (and worst) generated images of Stable Diffusion](examples/stable_diffusion_evaluation.ipynb)
 
 
-Also check this post on Medium:
-
-[Evaluating automatic speech recognition models beyond global metrics — A tutorial using OpenAI’s Whisper as an example](https://medium.com/@daniel-klitzke/evaluating-automatic-speech-recognition-models-beyond-global-metrics-a-tutorial-using-openais-54b63c4dadbd)
-
 ## 🗺️ Public Roadmap
 - [x] Detection of problematic data slices
 - [x] Basic explanation of found issues via feature importances
 - [x] Limited embedding computation for images, audio, text
 - [x] Extended embedding support, e.g., more embedding models and allow precomputed embeddings
 - [x] Speed up embedding computation using datasets library
 - [ ] Soft Dependencies for embedding computation as torch dependencies are large
```

### Comparing `sliceguard-0.0.8/pyproject.toml` & `sliceguard-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sliceguard"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Renumics GmbH", email="info@renumics.com"},
   { name="Daniel Klitzke", email="daniel.klitzke@renumics.com"}
 ]
 description = "A library for detecting critical data slices in structured and unstructured data based on features, metadata and model predictions."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `sliceguard-0.0.8/sliceguard/detection.py` & `sliceguard-0.0.9/sliceguard/detection.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 from hnne import HNNE
 import numpy as np
 import pandas as pd
 from fairlearn.metrics import MetricFrame
 from sklearn.cluster import HDBSCAN
 
+import matplotlib.pyplot as plt
+
 
 def generate_metric_frames(
     encoded_data: np.array,
     df: pd.DataFrame,
     y: str,
     y_pred: str,
     metric: Callable,
@@ -41,21 +43,24 @@
         partitions = hnne.hierarchy_parameters.partitions
 
         partitions = np.flip(
             partitions, axis=1
         )  # reverse the order of the hierarchy levels, go from coarse to fine
         partition_sizes = hnne.hierarchy_parameters.partition_sizes
         partition_levels = len(partition_sizes)
+
     except:
         # The projection might fail if there are not enough data points.
         # In this case just use other clustering approach as fallback.
-        print("Warning: Using hierarchical clustering failed. Probably the provided datapoints were not enough. HDBSCAN fallback might yield bad results!")
+        print(
+            "Warning: Using hierarchical clustering failed. Probably the provided datapoints were not enough. HDBSCAN fallback might yield bad results!"
+        )
         hdbscan = HDBSCAN(min_cluster_size=2)
         hdbscan.fit(encoded_data)
-        partitions=hdbscan.labels_[..., np.newaxis]
+        partitions = hdbscan.labels_[..., np.newaxis]
         partition_sizes = [len(np.unique(hdbscan.labels_))]
         partition_levels = len(partition_sizes)
         # TODO: This doesn't necessarily make sense as noisy samples will be treated as own cluster. However that is how it is now.
 
     clustering_cols = [f"clustering_{i}" for i in range(partition_levels)]
     clustering_df = pd.DataFrame(
         data=partitions, columns=clustering_cols, index=df.index
@@ -131,16 +136,14 @@
     if min_support is None:
         min_support = round(max(0.0025 * len(clustering_df), 5))
     print(
         f"Using {min_support} as minimum support for determining problematic clusters."
     )
     print(f"Using {min_drop} as minimum drop for determining problematic clusters.")
 
-    previous_group_df = None
-    previous_clustering_col = None
     for mf, clustering_col in zip(mfs, clustering_cols):
         # Calculate cluster support
         drops = (
             mf.overall.values[0] - mf.by_group.values[:, 0]
             if metric_mode == "max"
             else mf.by_group.values[:, 0] - mf.overall.values[0]
         )
@@ -216,29 +219,10 @@
         group_df["issue"] = False
 
         group_df.loc[
             (group_df[drop_col] >= min_drop) & (group_df[support_col] >= min_support),
             "issue",
         ] = True
 
-        # Unmark parent cluster if drop shows mostly on this level
-        if previous_group_df is not None:
-            for cluster, row in group_df.iterrows():
-                group_entries = clustering_df[clustering_df[clustering_col] == cluster]
-                assert (
-                    group_entries[previous_clustering_col].values[0]
-                    == group_entries[previous_clustering_col].values
-                ).all()
-                parent_cluster = group_entries[previous_clustering_col].values[0]
-
-                if (
-                    row[support_col] > min_support and row[drop_col] > min_drop
-                ):  # TODO Verify this rule makes sense, could cause larger clusters to be discarded because of one also bad subcluster
-                    previous_group_df.loc[parent_cluster, "issue"] = False
-                else:
-                    group_df.loc[cluster, "issue"] = False
-
         group_dfs.append(group_df)
 
-        previous_group_df = group_df
-        previous_clustering_col = clustering_col
     return group_dfs
```

### Comparing `sliceguard-0.0.8/sliceguard/embedding_utils.py` & `sliceguard-0.0.9/sliceguard/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.8/sliceguard/explanation.py` & `sliceguard-0.0.9/sliceguard/explanation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 from sklearn.preprocessing import LabelEncoder
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.metrics import f1_score
 
 
-def explain_clusters(features, feature_types, issue_df, df, prereduced_embeddings):
+def explain_clusters(features, feature_types, issues, df, prereduced_embeddings):
     """
     Method to generate explanations on why clusters are problematic or different from the rest of the data.
 
     :param features: The features to use for generating the explanations.
     :param feature_types: The previously inferred type of the features.
     :param issue_df: The dataframe containing the issues.
     :param: df: The dataframe containing the raw data.
@@ -58,22 +58,19 @@
             raise RuntimeError(
                 "Met unexpected feature type while generating explanations."
             )
 
     # Fit tree to generate feature importances
     # TODO: Potentially replace with simpler univariate mechanism, see also spotlight relevance score
     # TODO: Probably try shap or something similar
-    issue_df["issue_explanation"] = ""
 
-    for issue in issue_df["issue"].unique():
-        if issue == -1:  # Skip data points with no issues
-            continue
-        issue_indices_pandas = issue_df[issue_df["issue"] == issue].index
-        issue_indices_list = np.where(issue_df["issue"] == issue)[0]
-        y = np.zeros(len(issue_df))
+    for issue in issues:
+        issue_indices_pandas = issue["indices"]
+        issue_indices_list = np.where(df.index.isin(issue["indices"]))[0]
+        y = np.zeros(len(df))
         y[issue_indices_list] = 1
         clf = DecisionTreeClassifier(
             max_depth=3, max_features=4
         )  # keep the trees simple to not overfit
         clf.fit(classification_data, y)
 
         preds = clf.predict(classification_data)
@@ -94,11 +91,9 @@
         ordered_importances = importances[feature_order]
         ordered_features = np.array(features)[feature_order]
 
         # if f1 > 0.7: # only add explanation if it is succicient to classify cluster?
         importance_strings = []
         for f, i in zip(ordered_features[:3], ordered_importances[:3]):
             importance_strings.append(f"{f}, ({i:.2f})")
-        issue_df.loc[issue_indices_pandas, "issue_explanation"] = ", ".join(
-            importance_strings
-        )
-    return issue_df
+        issue["explanation"] = ", ".join(importance_strings)
+    return issues
```

### Comparing `sliceguard-0.0.8/sliceguard/sliceguard.py` & `sliceguard-0.0.9/sliceguard/sliceguard.py`

 * *Files 10% similar despite different names*

```diff
@@ -132,86 +132,80 @@
         )
 
         num_issues = np.sum([group_df["issue"].sum() for group_df in group_dfs])
 
         print(f"Identified {num_issues} problematic slices.")
 
         # Construct the issue dataframe that is returned by this method
-        issue_df = pd.DataFrame(data=[-1] * len(df), columns=["issue"], index=df.index)
-        issue_df["issue"] = issue_df["issue"].astype(int)
-        issue_df["issue_metric"] = np.nan
+        issues = []
 
         issue_index = 0
-        for _, (group_df, clustering_col, clustering_metric_col) in enumerate(
-            zip(group_dfs, clustering_cols, clustering_metric_cols)
-        ):
+        for hierarchy_level, (
+            group_df,
+            clustering_col,
+            clustering_metric_col,
+        ) in enumerate(zip(group_dfs, clustering_cols, clustering_metric_cols)):
             hierarchy_issues = group_df[group_df["issue"] == True].index
             for issue in hierarchy_issues:
+                current_issue = {"id": issue_index, "level": hierarchy_level}
                 issue_indices = clustering_df[
                     clustering_df[clustering_col] == issue
                 ].index.values
-                issue_df.loc[issue_indices, "issue"] = issue_index
+                current_issue["indices"] = issue_indices
+
                 issue_metric = clustering_df[clustering_df[clustering_col] == issue][
                     clustering_metric_col
                 ].values[0]
-                issue_df.loc[issue_indices, "issue_metric"] = issue_metric
+                current_issue["metric"] = issue_metric
+
+                issues.append(current_issue)
+
                 issue_index += 1
 
         # Derive rules that are characteristic for each identified problem slice
         # This is done to help understanding of the problem reason
         # First stage this will be only importance values!
-        issue_df = explain_clusters(
-            features, feature_types, issue_df, df, prereduced_embeddings
+        issues = explain_clusters(
+            features, feature_types, issues, df, prereduced_embeddings
         )
 
-        self._issue_df = issue_df
+        self._issues = issues
         self._clustering_df = clustering_df
         self._clustering_cols = clustering_cols
         self._metric_mode = metric_mode
         self._df = df
         self.embeddings = raw_embeddings
 
-        return issue_df
+        return issues
 
     def report(self, spotlight_dtype: Dict[str, spotlight.dtypes.base.DType] = {}):
         """
         Create an interactive report on the found issues in spotlight.
         :param spotlight_dtype: Define a datatype mapping for the interactive spotlight report. Will be passed to dtypes parameter of spotlight.show.
         """
         # Some basic checks
-        assert self._issue_df is not None
-        assert len(self._df) == len(self._issue_df)
-        assert all(self._df.index == self._issue_df.index)
+        assert self._issues is not None
 
-        df = pd.concat((self._df, self._issue_df), axis=1)
+        df = self._df.copy()
 
         # Insert embeddings if they were computed
         embedding_dtypes = {}
         for embedding_col, embeddings in self.embeddings.items():
             report_col_name = f"sg_emb_{embedding_col}"
             df[report_col_name] = [e.tolist() for e in embeddings]
             embedding_dtypes[report_col_name] = Embedding
 
         data_issue_severity = []
         data_issues = []
-        for issue in self._issue_df["issue"].unique():
-            if issue == -1:
-                continue
-            issue_rows = np.where(self._issue_df["issue"] == issue)[
+        for issue in self._issues:
+            issue_rows = np.where(df.index.isin(issue["indices"]))[
                 0
             ].tolist()  # Note: Has to be row index not pandas index!
-            issue_metric = self._issue_df[self._issue_df["issue"] == issue].iloc[0][
-                "issue_metric"
-            ]
-            issue_explanation = (
-                f"{issue_metric:.2f} -> "
-                + self._issue_df[self._issue_df["issue"] == issue].iloc[0][
-                    "issue_explanation"
-                ]
-            )
+            issue_metric = issue["metric"]
+            issue_explanation = f"{issue_metric:.2f} -> " + issue["explanation"]
 
             data_issue = DataIssue(
                 severity="medium",
                 title=issue_explanation,
                 description=issue_explanation,
                 rows=issue_rows,
             )
```

### Comparing `sliceguard-0.0.8/sliceguard/utils.py` & `sliceguard-0.0.9/sliceguard/utils.py`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.8/sliceguard.egg-info/PKG-INFO` & `sliceguard-0.0.9/sliceguard.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliceguard
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library for detecting critical data slices in structured and unstructured data based on features, metadata and model predictions.
 Author-email: Renumics GmbH <info@renumics.com>, Daniel Klitzke <daniel.klitzke@renumics.com>
 Project-URL: Homepage, https://github.com/Renumics/sliceguard
 Project-URL: Bug Tracker, https://github.com/Renumics/sliceguard/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -62,20 +62,17 @@
 )
 sg.report()
 ```
 
 ## 🔧 Use case-specific examples
 * [Detecting issues in automatic speech recognition (ASR) models](examples/audio_issues_commonvoice_whisper.ipynb)
 * [Detecting issues in audio datasets (condition monitoring)](examples/audio_issues_condition_monitoring_dcase.ipynb)
+* [Selecting the best (and worst) generated images of Stable Diffusion](examples/stable_diffusion_evaluation.ipynb)
 
 
-Also check this post on Medium:
-
-[Evaluating automatic speech recognition models beyond global metrics — A tutorial using OpenAI’s Whisper as an example](https://medium.com/@daniel-klitzke/evaluating-automatic-speech-recognition-models-beyond-global-metrics-a-tutorial-using-openais-54b63c4dadbd)
-
 ## 🗺️ Public Roadmap
 - [x] Detection of problematic data slices
 - [x] Basic explanation of found issues via feature importances
 - [x] Limited embedding computation for images, audio, text
 - [x] Extended embedding support, e.g., more embedding models and allow precomputed embeddings
 - [x] Speed up embedding computation using datasets library
 - [ ] Soft Dependencies for embedding computation as torch dependencies are large
```

### Comparing `sliceguard-0.0.8/tests/test_sliceguard.py` & `sliceguard-0.0.9/tests/test_sliceguard.py`

 * *Files identical despite different names*

