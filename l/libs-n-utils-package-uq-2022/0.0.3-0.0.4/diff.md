# Comparing `tmp/libs_n_utils_package_uq_2022-0.0.3.tar.gz` & `tmp/libs_n_utils_package_uq_2022-0.0.4.tar.gz`

## Comparing `libs_n_utils_package_uq_2022-0.0.3.tar` & `libs_n_utils_package_uq_2022-0.0.4.tar`

### file list

```diff
@@ -1,57 +1,5 @@
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/__init__.py
--rwxr-xr-x   0        0        0     2751 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_NN_functional.py
--rwxr-xr-x   0        0        0     6972 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_NN_models.py
--rwxr-xr-x   0        0        0     1992 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_binary_classification.py
--rwxr-xr-x   0        0        0     7538 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_data_preprocessing.py
--rwxr-xr-x   0        0        0     3986 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_dataframe_manipulation.py
--rwxr-xr-x   0        0        0     9122 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_embedding.py
--rwxr-xr-x   0        0        0    12695 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_feature_calculation.py
--rwxr-xr-x   0        0        0    10603 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_file_manipulation.py
--rwxr-xr-x   0        0        0     3298 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_flow.py
--rwxr-xr-x   0        0        0     1287 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_helpers.py
--rwxr-xr-x   0        0        0     3285 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_imbalance.py
--rwxr-xr-x   0        0        0     5253 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_pandas_extensions.py
--rwxr-xr-x   0        0        0    37603 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_plotters.py
--rwxr-xr-x   0        0        0      395 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_small_utils.py
--rwxr-xr-x   0        0        0     8979 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_stat_distribution.py
--rwxr-xr-x   0        0        0     4390 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/my_easy_logger.py
--rwxr-xr-x   0        0        0     2913 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/3class_ds_select_save.py
--rwxr-xr-x   0        0        0     4168 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/MI_feature_importance.py
--rwxr-xr-x   0        0        0     7436 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/RF_feature_importance.py
--rwxr-xr-x   0        0        0     3375 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/RF_feimp_weighted_average_wasserstein.py
--rwxr-xr-x   0        0        0     2090 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/UNSW_NB15_data_preparation.py
--rwxr-xr-x   0        0        0     5964 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/alternate_feature_wasserstein.py
--rwxr-xr-x   0        0        0      346 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/attack_types.py
--rwxr-xr-x   0        0        0     1955 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/average_wasserstein.py
--rwxr-xr-x   0        0        0     7709 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/boruta_feature_selection.py
--rwxr-xr-x   0        0        0      613 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/boruta_visualisation.py
--rwxr-xr-x   0        0        0     1882 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/combine_2feather.py
--rwxr-xr-x   0        0        0     3109 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/combine_2pickles.py
--rwxr-xr-x   0        0        0     3278 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/combine_3pickles.py
--rwxr-xr-x   0        0        0     3859 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/combine_folder_csv.py
--rwxr-xr-x   0        0        0     1051 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/compare_pickle_files_in_folder.py
--rwxr-xr-x   0        0        0      771 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/csv_folder_to_feather_folder.py
--rwxr-xr-x   0        0        0      893 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/csv_folder_to_pickle_folder.py
--rwxr-xr-x   0        0        0      494 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/datasets_information.py
--rwxr-xr-x   0        0        0     1239 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/dict_manipulation.py
--rwxr-xr-x   0        0        0     3289 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/edit_CIC.py
--rwxr-xr-x   0        0        0     1443 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/edit_CIC_ton.py
--rwxr-xr-x   0        0        0     1112 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/feather_2m_sel_cols.py
--rwxr-xr-x   0        0        0     1298 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/feather_fldr_2_pickle_fldr.py
--rwxr-xr-x   0        0        0    12334 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/inter_dataset_feature_wasserstein.py
--rwxr-xr-x   0        0        0     3231 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/intra_dataset_feature_wasserstein.py
--rwxr-xr-x   0        0        0     5404 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/make_cics_compatible.py
--rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/make_unity_fi_pickle.py
--rwxr-xr-x   0        0        0    14129 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/netflow_preprocessing.py
--rwxr-xr-x   0        0        0     2332 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/pickle_fldr_2_feather_fldr.py
--rwxr-xr-x   0        0        0     1406 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/plot_MI_feature_importances.py
--rwxr-xr-x   0        0        0      949 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/plot_RF_feature_importance_differences.py
--rwxr-xr-x   0        0        0     1833 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/print_feature_selction_results.py
--rwxr-xr-x   0        0        0     1293 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/reading_txt_files.py
--rwxr-xr-x   0        0        0     4730 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/sample_save_fldr_datasets.py
--rwxr-xr-x   0        0        0     4883 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/weighted_average_alternate_wasserstein.py
--rwxr-xr-x   0        0        0     3340 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/weighted_average_wasserstein.py
--rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/LICENSE
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/README.md
--rwxr-xr-x   0        0        0      594 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.4/__init__.py
+-rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.4/LICENSE
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.4/README.md
+-rwxr-xr-x   0        0        0      594 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.4/PKG-INFO
```

### Comparing `libs_n_utils_package_uq_2022-0.0.3/LICENSE` & `libs_n_utils_package_uq_2022-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.3/pyproject.toml` & `libs_n_utils_package_uq_2022-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "libs_n_utils_package_uq_2022"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="siamak layeghy", email="siamak.layeghy@uq.net.au" },
 ]
 description = "A small library of utilities"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `libs_n_utils_package_uq_2022-0.0.3/PKG-INFO` & `libs_n_utils_package_uq_2022-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libs_n_utils_package_uq_2022
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small library of utilities
 Project-URL: Homepage, https://github.com/layeghy/libs_n_utils
 Project-URL: Bug Tracker, https://github.com/layeghy/libs_n_utils/issues
 Author-email: siamak layeghy <siamak.layeghy@uq.net.au>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

