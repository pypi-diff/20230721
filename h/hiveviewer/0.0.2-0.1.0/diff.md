# Comparing `tmp/hiveviewer-0.0.2.tar.gz` & `tmp/hiveviewer-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiveviewer-0.0.2.tar", last modified: Mon Jun 12 09:03:31 2023, max compression
+gzip compressed data, was "hiveviewer-0.1.0.tar", last modified: Fri Jul 21 04:24:06 2023, max compression
```

## Comparing `hiveviewer-0.0.2.tar` & `hiveviewer-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-12 09:03:31.078255 hiveviewer-0.0.2/
--rw-r--r--   0 yin        (501) staff       (20)     1066 2023-05-23 06:48:39.000000 hiveviewer-0.0.2/LICENSE
--rw-r--r--   0 yin        (501) staff       (20)     1130 2023-06-12 09:03:31.078126 hiveviewer-0.0.2/PKG-INFO
--rw-r--r--   0 yin        (501) staff       (20)      702 2023-06-07 09:53:26.000000 hiveviewer-0.0.2/README.md
--rw-r--r--   0 yin        (501) staff       (20)      327 2023-05-23 07:07:17.000000 hiveviewer-0.0.2/pyproject.toml
--rw-r--r--   0 yin        (501) staff       (20)       38 2023-06-12 09:03:31.078307 hiveviewer-0.0.2/setup.cfg
--rw-r--r--   0 yin        (501) staff       (20)      988 2023-06-12 09:03:28.000000 hiveviewer-0.0.2/setup.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-12 09:03:31.073349 hiveviewer-0.0.2/src/
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-12 09:03:31.074495 hiveviewer-0.0.2/src/hiveviewer/
--rw-r--r--   0 yin        (501) staff       (20)      105 2023-06-01 05:57:50.000000 hiveviewer-0.0.2/src/hiveviewer/__init__.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-12 09:03:31.075979 hiveviewer-0.0.2/src/hiveviewer/dataloader/
--rw-r--r--   0 yin        (501) staff       (20)      159 2023-06-08 09:03:04.000000 hiveviewer-0.0.2/src/hiveviewer/dataloader/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     3026 2023-06-08 09:05:52.000000 hiveviewer-0.0.2/src/hiveviewer/dataloader/base.py
--rw-r--r--   0 yin        (501) staff       (20)      529 2023-06-12 08:50:25.000000 hiveviewer-0.0.2/src/hiveviewer/dataloader/load_csv.py
--rw-r--r--   0 yin        (501) staff       (20)      522 2023-06-08 09:04:37.000000 hiveviewer-0.0.2/src/hiveviewer/dataloader/load_excel.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-12 09:03:31.076501 hiveviewer-0.0.2/src/hiveviewer/evaluation/
--rw-r--r--   0 yin        (501) staff       (20)       70 2023-06-01 05:57:50.000000 hiveviewer-0.0.2/src/hiveviewer/evaluation/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     2781 2023-06-05 12:52:22.000000 hiveviewer-0.0.2/src/hiveviewer/evaluation/calculate_auc.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-12 09:03:31.077019 hiveviewer-0.0.2/src/hiveviewer/sampling/
--rw-r--r--   0 yin        (501) staff       (20)      106 2023-05-25 06:14:02.000000 hiveviewer-0.0.2/src/hiveviewer/sampling/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)      667 2023-06-01 11:26:56.000000 hiveviewer-0.0.2/src/hiveviewer/sampling/base.py
--rw-r--r--   0 yin        (501) staff       (20)     2346 2023-06-01 11:45:32.000000 hiveviewer-0.0.2/src/hiveviewer/sampling/gini_sampler.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-12 09:03:31.077891 hiveviewer-0.0.2/src/hiveviewer/visualization/
--rw-r--r--   0 yin        (501) staff       (20)      301 2023-06-08 08:44:36.000000 hiveviewer-0.0.2/src/hiveviewer/visualization/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     8779 2023-06-12 09:02:43.000000 hiveviewer-0.0.2/src/hiveviewer/visualization/lorenz_curve.py
--rw-r--r--   0 yin        (501) staff       (20)     3371 2023-06-07 12:51:20.000000 hiveviewer-0.0.2/src/hiveviewer/visualization/plot_trisurf.py
--rw-r--r--   0 yin        (501) staff       (20)     3929 2023-06-08 08:44:36.000000 hiveviewer-0.0.2/src/hiveviewer/visualization/venn2.py
--rw-r--r--   0 yin        (501) staff       (20)     6601 2023-06-12 09:00:24.000000 hiveviewer-0.0.2/src/hiveviewer/visualization/venn3.py
--rw-r--r--   0 yin        (501) staff       (20)     2758 2023-06-08 08:44:36.000000 hiveviewer-0.0.2/src/hiveviewer/visualization/venn_base.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-12 09:03:31.075258 hiveviewer-0.0.2/src/hiveviewer.egg-info/
--rw-r--r--   0 yin        (501) staff       (20)     1130 2023-06-12 09:03:31.000000 hiveviewer-0.0.2/src/hiveviewer.egg-info/PKG-INFO
--rw-r--r--   0 yin        (501) staff       (20)      845 2023-06-12 09:03:31.000000 hiveviewer-0.0.2/src/hiveviewer.egg-info/SOURCES.txt
--rw-r--r--   0 yin        (501) staff       (20)        1 2023-06-12 09:03:31.000000 hiveviewer-0.0.2/src/hiveviewer.egg-info/dependency_links.txt
--rw-r--r--   0 yin        (501) staff       (20)       75 2023-06-12 09:03:31.000000 hiveviewer-0.0.2/src/hiveviewer.egg-info/requires.txt
--rw-r--r--   0 yin        (501) staff       (20)       11 2023-06-12 09:03:31.000000 hiveviewer-0.0.2/src/hiveviewer.egg-info/top_level.txt
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-21 04:24:06.436545 hiveviewer-0.1.0/
+-rw-r--r--   0 yin        (501) staff       (20)     1066 2023-07-19 11:32:11.000000 hiveviewer-0.1.0/LICENSE
+-rw-r--r--   0 yin        (501) staff       (20)     1126 2023-07-21 04:24:06.436431 hiveviewer-0.1.0/PKG-INFO
+-rw-r--r--   0 yin        (501) staff       (20)      735 2023-06-14 07:48:21.000000 hiveviewer-0.1.0/README.md
+-rw-r--r--   0 yin        (501) staff       (20)      327 2023-05-23 07:07:17.000000 hiveviewer-0.1.0/pyproject.toml
+-rw-r--r--   0 yin        (501) staff       (20)       38 2023-07-21 04:24:06.436595 hiveviewer-0.1.0/setup.cfg
+-rw-r--r--   0 yin        (501) staff       (20)      988 2023-07-21 04:23:33.000000 hiveviewer-0.1.0/setup.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-21 04:24:06.431531 hiveviewer-0.1.0/src/
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-21 04:24:06.432670 hiveviewer-0.1.0/src/hiveviewer/
+-rw-r--r--   0 yin        (501) staff       (20)      133 2023-07-19 11:32:15.000000 hiveviewer-0.1.0/src/hiveviewer/__init__.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-21 04:24:06.434121 hiveviewer-0.1.0/src/hiveviewer/dataloader/
+-rw-r--r--   0 yin        (501) staff       (20)      159 2023-07-21 02:45:47.000000 hiveviewer-0.1.0/src/hiveviewer/dataloader/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     3169 2023-07-21 04:18:15.000000 hiveviewer-0.1.0/src/hiveviewer/dataloader/base.py
+-rw-r--r--   0 yin        (501) staff       (20)      519 2023-07-21 03:59:25.000000 hiveviewer-0.1.0/src/hiveviewer/dataloader/load_csv.py
+-rw-r--r--   0 yin        (501) staff       (20)      512 2023-07-21 03:19:27.000000 hiveviewer-0.1.0/src/hiveviewer/dataloader/load_excel.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-21 04:24:06.434468 hiveviewer-0.1.0/src/hiveviewer/evaluation/
+-rw-r--r--   0 yin        (501) staff       (20)       64 2023-07-19 09:14:34.000000 hiveviewer-0.1.0/src/hiveviewer/evaluation/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     4567 2023-07-21 03:20:46.000000 hiveviewer-0.1.0/src/hiveviewer/evaluation/calculate_auc.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-21 04:24:06.434907 hiveviewer-0.1.0/src/hiveviewer/optimization/
+-rw-r--r--   0 yin        (501) staff       (20)      128 2023-07-19 08:12:07.000000 hiveviewer-0.1.0/src/hiveviewer/optimization/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)      770 2023-07-20 10:58:22.000000 hiveviewer-0.1.0/src/hiveviewer/optimization/base.py
+-rw-r--r--   0 yin        (501) staff       (20)     5220 2023-07-21 04:19:25.000000 hiveviewer-0.1.0/src/hiveviewer/optimization/profolio_objective.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-21 04:24:06.435339 hiveviewer-0.1.0/src/hiveviewer/sampling/
+-rw-r--r--   0 yin        (501) staff       (20)      106 2023-05-25 06:14:02.000000 hiveviewer-0.1.0/src/hiveviewer/sampling/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)      667 2023-07-18 12:12:04.000000 hiveviewer-0.1.0/src/hiveviewer/sampling/base.py
+-rw-r--r--   0 yin        (501) staff       (20)     2346 2023-07-19 08:03:56.000000 hiveviewer-0.1.0/src/hiveviewer/sampling/gini_sampler.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-21 04:24:06.436244 hiveviewer-0.1.0/src/hiveviewer/visualization/
+-rw-r--r--   0 yin        (501) staff       (20)      301 2023-06-08 08:44:36.000000 hiveviewer-0.1.0/src/hiveviewer/visualization/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     8779 2023-07-21 04:14:30.000000 hiveviewer-0.1.0/src/hiveviewer/visualization/lorenz_curve.py
+-rw-r--r--   0 yin        (501) staff       (20)     3371 2023-06-07 12:51:20.000000 hiveviewer-0.1.0/src/hiveviewer/visualization/plot_trisurf.py
+-rw-r--r--   0 yin        (501) staff       (20)     3929 2023-07-21 04:04:42.000000 hiveviewer-0.1.0/src/hiveviewer/visualization/venn2.py
+-rw-r--r--   0 yin        (501) staff       (20)     6601 2023-07-21 03:59:13.000000 hiveviewer-0.1.0/src/hiveviewer/visualization/venn3.py
+-rw-r--r--   0 yin        (501) staff       (20)     2758 2023-06-08 08:44:36.000000 hiveviewer-0.1.0/src/hiveviewer/visualization/venn_base.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-21 04:24:06.433491 hiveviewer-0.1.0/src/hiveviewer.egg-info/
+-rw-r--r--   0 yin        (501) staff       (20)     1126 2023-07-21 04:24:06.000000 hiveviewer-0.1.0/src/hiveviewer.egg-info/PKG-INFO
+-rw-r--r--   0 yin        (501) staff       (20)      971 2023-07-21 04:24:06.000000 hiveviewer-0.1.0/src/hiveviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 yin        (501) staff       (20)        1 2023-07-21 04:24:06.000000 hiveviewer-0.1.0/src/hiveviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 yin        (501) staff       (20)       75 2023-07-21 04:24:06.000000 hiveviewer-0.1.0/src/hiveviewer.egg-info/requires.txt
+-rw-r--r--   0 yin        (501) staff       (20)       11 2023-07-21 04:24:06.000000 hiveviewer-0.1.0/src/hiveviewer.egg-info/top_level.txt
```

### Comparing `hiveviewer-0.0.2/LICENSE` & `hiveviewer-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.0.2/PKG-INFO` & `hiveviewer-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 Metadata-Version: 2.1
 Name: hiveviewer
-Version: 0.0.2
+Version: 0.1.0
 Summary: Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.
 Home-page: https://github.com/yinsn/hiveviewer
 Author: Yin Cheng
 Author-email: yin.sjtu@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HiveViewer
 
 HiveViewer is a comprehensive Python toolkit designed to streamline data analysis tasks. This toolkit is tailored for working with large datasets, providing a suite of functionalities ranging from flexible data loading and processing to advanced evaluation metrics, data sampling, and data visualization.
 
 ## Installation
 
 You can install HiveViewer using pip:
 
 ```bash
-pip install hiveviewer
+pip install git+https://github.com/yinsn/hiveviewer.git
 ```
 
 ## Contributing
 
 We welcome contributions! If you're interested in enhancing the features of HiveViewer, please create a pull request.
 
 ## License
 
 HiveViewer is licensed under the MIT License.
 
 ## Acknowledgments
 
 We appreciate the community for your support and contributions. Thank you!
-
-
```

### Comparing `hiveviewer-0.0.2/README.md` & `hiveviewer-0.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 HiveViewer is a comprehensive Python toolkit designed to streamline data analysis tasks. This toolkit is tailored for working with large datasets, providing a suite of functionalities ranging from flexible data loading and processing to advanced evaluation metrics, data sampling, and data visualization.
 
 ## Installation
 
 You can install HiveViewer using pip:
 
 ```bash
-pip install hiveviewer
+pip install git+https://github.com/yinsn/hiveviewer.git
 ```
 
 ## Contributing
 
 We welcome contributions! If you're interested in enhancing the features of HiveViewer, please create a pull request.
 
 ## License
```

### Comparing `hiveviewer-0.0.2/setup.py` & `hiveviewer-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,20 @@
         "matplotlib_venn",
         "openpyxl",
     ],
 )
 
 setup(
     name="hiveviewer",
-    version="0.0.2",
+    version="0.1.0",
     author="Yin Cheng",
     author_email="yin.sjtu@gmail.com",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/yinsn/hiveviewer",
-    python_requires=">=3.7",
+    python_requires=">=3.6",
     description="Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.",
     packages=find_packages("src"),
     package_dir={"": "src"},
     install_requires=install_requires,
     include_package_data=True,
 )
```

### Comparing `hiveviewer-0.0.2/src/hiveviewer/dataloader/base.py` & `hiveviewer-0.1.0/src/hiveviewer/dataloader/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def column_name_spliting(self, delimiter: str = ".") -> None:
         """Split column names by delimiter."""
         columns = []
         if self.df is not None:
             for column in self.df.columns:
                 columns.append(column.split(delimiter)[-1])
-            self.df.columns = columns
+            self.df.columns = pd.Index(columns)
 
     def add_one_smoothing(self, column: str) -> None:
         """Add one smoothing to a column.
 
         :param column: column name
         """
         if self.df is not None:
@@ -72,23 +72,29 @@
         )
         valid_df = df[df[user_column].isin(valid_users)].copy()
         valid_df.reset_index(drop=True, inplace=True)
         return valid_df
 
     @staticmethod
     def clip_clean_count_with_group(
-        df: pd.DataFrame, groupby: str, clip_column: str, label_column: str
+        df: pd.DataFrame,
+        groupby: str,
+        label_column: str,
+        clip_column: Optional[str] = None,
     ) -> Tuple:
         """Clip and count with group.
 
         :param df: dataframe
         :param groupby: groupby column
         :param clip_column: column to clip
         :param label_column: label column
         """
         df_clean = BaseDataLoader.clean_one_label_users(
             df=df, user_column=groupby, label_column=label_column
         )
-        counts_df = BaseDataLoader.clip_and_sum_with_group(
-            df=df_clean, groupby=groupby, clip_column=clip_column
-        )
+        if clip_column is not None:
+            counts_df = BaseDataLoader.clip_and_sum_with_group(
+                df=df_clean, groupby=groupby, clip_column=clip_column
+            )
+        else:
+            counts_df = None
         return df_clean, counts_df
```

### Comparing `hiveviewer-0.0.2/src/hiveviewer/dataloader/load_csv.py` & `hiveviewer-0.1.0/src/hiveviewer/dataloader/load_csv.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 class CSVLoader(BaseDataLoader):
     "CSVLoader class for loading CSV files"
 
     def __init__(self, file_path: str, **kwargs: str):
         super().__init__(file_path, **kwargs)
         self.column_name_spliting()
 
-    def load_data(self) -> Optional[pd.DataFrame]:
+    def load_data(self) -> pd.DataFrame:
         """Load data from CSV file."""
         file_url = os.path.join(self.file_path, self.file_name) + ".csv"
         return pd.read_csv(file_url, low_memory=False)
```

### Comparing `hiveviewer-0.0.2/src/hiveviewer/sampling/base.py` & `hiveviewer-0.1.0/src/hiveviewer/sampling/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.0.2/src/hiveviewer/sampling/gini_sampler.py` & `hiveviewer-0.1.0/src/hiveviewer/sampling/gini_sampler.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.0.2/src/hiveviewer/visualization/lorenz_curve.py` & `hiveviewer-0.1.0/src/hiveviewer/visualization/lorenz_curve.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.0.2/src/hiveviewer/visualization/plot_trisurf.py` & `hiveviewer-0.1.0/src/hiveviewer/visualization/plot_trisurf.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.0.2/src/hiveviewer/visualization/venn2.py` & `hiveviewer-0.1.0/src/hiveviewer/visualization/venn2.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.0.2/src/hiveviewer/visualization/venn3.py` & `hiveviewer-0.1.0/src/hiveviewer/visualization/venn3.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.0.2/src/hiveviewer/visualization/venn_base.py` & `hiveviewer-0.1.0/src/hiveviewer/visualization/venn_base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.0.2/src/hiveviewer.egg-info/PKG-INFO` & `hiveviewer-0.1.0/src/hiveviewer.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 Metadata-Version: 2.1
 Name: hiveviewer
-Version: 0.0.2
+Version: 0.1.0
 Summary: Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.
 Home-page: https://github.com/yinsn/hiveviewer
 Author: Yin Cheng
 Author-email: yin.sjtu@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HiveViewer
 
 HiveViewer is a comprehensive Python toolkit designed to streamline data analysis tasks. This toolkit is tailored for working with large datasets, providing a suite of functionalities ranging from flexible data loading and processing to advanced evaluation metrics, data sampling, and data visualization.
 
 ## Installation
 
 You can install HiveViewer using pip:
 
 ```bash
-pip install hiveviewer
+pip install git+https://github.com/yinsn/hiveviewer.git
 ```
 
 ## Contributing
 
 We welcome contributions! If you're interested in enhancing the features of HiveViewer, please create a pull request.
 
 ## License
 
 HiveViewer is licensed under the MIT License.
 
 ## Acknowledgments
 
 We appreciate the community for your support and contributions. Thank you!
-
-
```

### Comparing `hiveviewer-0.0.2/src/hiveviewer.egg-info/SOURCES.txt` & `hiveviewer-0.1.0/src/hiveviewer.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 src/hiveviewer.egg-info/top_level.txt
 src/hiveviewer/dataloader/__init__.py
 src/hiveviewer/dataloader/base.py
 src/hiveviewer/dataloader/load_csv.py
 src/hiveviewer/dataloader/load_excel.py
 src/hiveviewer/evaluation/__init__.py
 src/hiveviewer/evaluation/calculate_auc.py
+src/hiveviewer/optimization/__init__.py
+src/hiveviewer/optimization/base.py
+src/hiveviewer/optimization/profolio_objective.py
 src/hiveviewer/sampling/__init__.py
 src/hiveviewer/sampling/base.py
 src/hiveviewer/sampling/gini_sampler.py
 src/hiveviewer/visualization/__init__.py
 src/hiveviewer/visualization/lorenz_curve.py
 src/hiveviewer/visualization/plot_trisurf.py
 src/hiveviewer/visualization/venn2.py
```

