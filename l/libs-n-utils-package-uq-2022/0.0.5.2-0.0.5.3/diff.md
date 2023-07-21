# Comparing `tmp/libs_n_utils_package_uq_2022-0.0.5.2.tar.gz` & `tmp/libs_n_utils_package_uq_2022-0.0.5.3.tar.gz`

## Comparing `libs_n_utils_package_uq_2022-0.0.5.2.tar` & `libs_n_utils_package_uq_2022-0.0.5.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rwxr-xr-x   0        0        0      449 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/how_to_package.txt
--rwxr-xr-x   0        0        0      591 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/.idea/libs_n_utils.iml
--rwxr-xr-x   0        0        0      917 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/.idea/misc.xml
--rwxr-xr-x   0        0        0      276 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/.idea/modules.xml
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/.idea/vcs.xml
--rwxr-xr-x   0        0        0    21750 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/.idea/workspace.xml
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/.idea/inspectionProfiles/profiles_settings.xml
--rwxr-xr-x   0        0        0     2909 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/3class_ds_select_save.py
--rwxr-xr-x   0        0        0     4168 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/MI_feature_importance.py
--rwxr-xr-x   0        0        0     7432 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/RF_feature_importance.py
--rwxr-xr-x   0        0        0     3367 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/RF_feimp_weighted_average_wasserstein.py
--rwxr-xr-x   0        0        0     2090 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/UNSW_NB15_data_preparation.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/__init__.py
--rwxr-xr-x   0        0        0     5956 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/alternate_feature_wasserstein.py
--rwxr-xr-x   0        0        0      346 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/attack_types.py
--rwxr-xr-x   0        0        0     1947 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/average_wasserstein.py
--rwxr-xr-x   0        0        0     7705 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/boruta_feature_selection.py
--rwxr-xr-x   0        0        0      613 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/boruta_visualisation.py
--rwxr-xr-x   0        0        0     1878 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/combine_2feather.py
--rwxr-xr-x   0        0        0     3105 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/combine_2pickles.py
--rwxr-xr-x   0        0        0     3274 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/combine_3pickles.py
--rwxr-xr-x   0        0        0     3851 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/combine_folder_csv.py
--rwxr-xr-x   0        0        0     1051 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/compare_pickle_files_in_folder.py
--rwxr-xr-x   0        0        0    25974 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/config_template.py
--rwxr-xr-x   0        0        0      767 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/csv_folder_to_feather_folder.py
--rwxr-xr-x   0        0        0      881 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/csv_folder_to_pickle_folder.py
--rwxr-xr-x   0        0        0      494 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/datasets_information.py
--rwxr-xr-x   0        0        0     1239 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/dict_manipulation.py
--rwxr-xr-x   0        0        0     3281 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/edit_CIC.py
--rwxr-xr-x   0        0        0     1443 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/edit_CIC_ton.py
--rwxr-xr-x   0        0        0     1112 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/feather_2m_sel_cols.py
--rwxr-xr-x   0        0        0     1298 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/feather_fldr_2_pickle_fldr.py
--rwxr-xr-x   0        0        0    12322 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/inter_dataset_feature_wasserstein.py
--rwxr-xr-x   0        0        0     3215 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/intra_dataset_feature_wasserstein.py
--rwxr-xr-x   0        0        0     2747 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_NN_functional.py
--rwxr-xr-x   0        0        0     6968 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_NN_models.py
--rwxr-xr-x   0        0        0     1984 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_binary_classification.py
--rwxr-xr-x   0        0        0     7534 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_data_preprocessing.py
--rwxr-xr-x   0        0        0     3982 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_dataframe_manipulation.py
--rwxr-xr-x   0        0        0     9110 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_embedding.py
--rwxr-xr-x   0        0        0    12691 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_feature_calculation.py
--rwxr-xr-x   0        0        0    10595 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_file_manipulation.py
--rwxr-xr-x   0        0        0     3294 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_flow.py
--rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_helpers.py
--rwxr-xr-x   0        0        0     3285 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_imbalance.py
--rwxr-xr-x   0        0        0     5253 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_pandas_extensions.py
--rwxr-xr-x   0        0        0    37599 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_plotters.py
--rwxr-xr-x   0        0        0      395 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_small_utils.py
--rwxr-xr-x   0        0        0     8975 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_stat_distribution.py
--rwxr-xr-x   0        0        0     5404 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/make_cics_compatible.py
--rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/make_unity_fi_pickle.py
--rwxr-xr-x   0        0        0     4390 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/my_easy_logger.py
--rwxr-xr-x   0        0        0    14129 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/netflow_preprocessing.py
--rwxr-xr-x   0        0        0     2332 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/pickle_fldr_2_feather_fldr.py
--rwxr-xr-x   0        0        0     1402 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/plot_MI_feature_importances.py
--rwxr-xr-x   0        0        0      949 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/plot_RF_feature_importance_differences.py
--rwxr-xr-x   0        0        0     1829 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/print_feature_selction_results.py
--rwxr-xr-x   0        0        0     1293 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/reading_txt_files.py
--rwxr-xr-x   0        0        0     4726 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/sample_save_fldr_datasets.py
--rwxr-xr-x   0        0        0     4879 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/weighted_average_alternate_wasserstein.py
--rwxr-xr-x   0        0        0     3332 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/weighted_average_wasserstein.py
--rwxr-xr-x   0        0        0    79057 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3-py3-none-any.whl
--rwxr-xr-x   0        0        0    51264 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3.tar.gz
--rwxr-xr-x   0        0        0    83488 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4-py3-none-any.whl
--rwxr-xr-x   0        0        0    56778 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4.tar.gz
--rwxr-xr-x   0        0        0    83488 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5-py3-none-any.whl
--rwxr-xr-x   0        0        0    83508 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1-py3-none-any.whl
--rwxr-xr-x   0        0        0    56775 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1.tar.gz
--rwxr-xr-x   0        0        0    56776 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.tar.gz
--rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/LICENSE
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/README.md
--rwxr-xr-x   0        0        0      596 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/pyproject.toml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.2/PKG-INFO
+-rwxr-xr-x   0        0        0      449 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/how_to_package.txt
+-rwxr-xr-x   0        0        0      694 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/.idea/libs_n_utils.iml
+-rwxr-xr-x   0        0        0     1135 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/.idea/misc.xml
+-rwxr-xr-x   0        0        0      276 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/.idea/modules.xml
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/.idea/vcs.xml
+-rwxr-xr-x   0        0        0    21978 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/.idea/workspace.xml
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/.idea/inspectionProfiles/profiles_settings.xml
+-rwxr-xr-x   0        0        0     2909 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/3class_ds_select_save.py
+-rwxr-xr-x   0        0        0     4168 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/MI_feature_importance.py
+-rwxr-xr-x   0        0        0     7432 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/RF_feature_importance.py
+-rwxr-xr-x   0        0        0     3367 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/RF_feimp_weighted_average_wasserstein.py
+-rwxr-xr-x   0        0        0     2090 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/UNSW_NB15_data_preparation.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/__init__.py
+-rwxr-xr-x   0        0        0     5956 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/alternate_feature_wasserstein.py
+-rwxr-xr-x   0        0        0      346 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/attack_types.py
+-rwxr-xr-x   0        0        0     1947 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/average_wasserstein.py
+-rwxr-xr-x   0        0        0     7705 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/boruta_feature_selection.py
+-rwxr-xr-x   0        0        0      613 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/boruta_visualisation.py
+-rwxr-xr-x   0        0        0     1878 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/combine_2feather.py
+-rwxr-xr-x   0        0        0     3105 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/combine_2pickles.py
+-rwxr-xr-x   0        0        0     3274 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/combine_3pickles.py
+-rwxr-xr-x   0        0        0     3851 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/combine_folder_csv.py
+-rwxr-xr-x   0        0        0     1051 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/compare_pickle_files_in_folder.py
+-rwxr-xr-x   0        0        0    25974 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/config_template.py
+-rwxr-xr-x   0        0        0      767 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/csv_folder_to_feather_folder.py
+-rwxr-xr-x   0        0        0      881 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/csv_folder_to_pickle_folder.py
+-rwxr-xr-x   0        0        0      494 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/datasets_information.py
+-rwxr-xr-x   0        0        0     1239 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/dict_manipulation.py
+-rwxr-xr-x   0        0        0     3281 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/edit_CIC.py
+-rwxr-xr-x   0        0        0     1443 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/edit_CIC_ton.py
+-rwxr-xr-x   0        0        0     1112 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/feather_2m_sel_cols.py
+-rwxr-xr-x   0        0        0     1298 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/feather_fldr_2_pickle_fldr.py
+-rwxr-xr-x   0        0        0    12322 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/inter_dataset_feature_wasserstein.py
+-rwxr-xr-x   0        0        0     3215 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/intra_dataset_feature_wasserstein.py
+-rwxr-xr-x   0        0        0     2747 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_NN_functional.py
+-rwxr-xr-x   0        0        0     6968 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_NN_models.py
+-rwxr-xr-x   0        0        0     1984 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_binary_classification.py
+-rwxr-xr-x   0        0        0     7534 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_data_preprocessing.py
+-rwxr-xr-x   0        0        0     3982 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_dataframe_manipulation.py
+-rwxr-xr-x   0        0        0     9110 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_embedding.py
+-rwxr-xr-x   0        0        0    12691 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_feature_calculation.py
+-rwxr-xr-x   0        0        0    10595 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_file_manipulation.py
+-rwxr-xr-x   0        0        0     3294 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_flow.py
+-rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_helpers.py
+-rwxr-xr-x   0        0        0     3285 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_imbalance.py
+-rwxr-xr-x   0        0        0     5253 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_pandas_extensions.py
+-rwxr-xr-x   0        0        0    37599 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_plotters.py
+-rwxr-xr-x   0        0        0      395 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_small_utils.py
+-rwxr-xr-x   0        0        0     8975 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_stat_distribution.py
+-rwxr-xr-x   0        0        0     5404 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/make_cics_compatible.py
+-rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/make_unity_fi_pickle.py
+-rwxr-xr-x   0        0        0     4390 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/my_easy_logger.py
+-rwxr-xr-x   0        0        0    14129 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/netflow_preprocessing.py
+-rwxr-xr-x   0        0        0     2332 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/pickle_fldr_2_feather_fldr.py
+-rwxr-xr-x   0        0        0     1402 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/plot_MI_feature_importances.py
+-rwxr-xr-x   0        0        0      949 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/plot_RF_feature_importance_differences.py
+-rwxr-xr-x   0        0        0     1829 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/print_feature_selction_results.py
+-rwxr-xr-x   0        0        0     1293 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/reading_txt_files.py
+-rwxr-xr-x   0        0        0     4726 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/sample_save_fldr_datasets.py
+-rwxr-xr-x   0        0        0     4879 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/weighted_average_alternate_wasserstein.py
+-rwxr-xr-x   0        0        0     3332 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/weighted_average_wasserstein.py
+-rwxr-xr-x   0        0        0    79057 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3-py3-none-any.whl
+-rwxr-xr-x   0        0        0    51264 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3.tar.gz
+-rwxr-xr-x   0        0        0    83488 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4-py3-none-any.whl
+-rwxr-xr-x   0        0        0    56778 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4.tar.gz
+-rwxr-xr-x   0        0        0    83488 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5-py3-none-any.whl
+-rwxr-xr-x   0        0        0    83508 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1-py3-none-any.whl
+-rwxr-xr-x   0        0        0    56775 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1.tar.gz
+-rwxr-xr-x   0        0        0    56776 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.tar.gz
+-rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/LICENSE
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/README.md
+-rwxr-xr-x   0        0        0      596 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.3/PKG-INFO
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/.idea/libs_n_utils.iml` & `libs_n_utils_package_uq_2022-0.0.5.3/.idea/libs_n_utils.iml`

 * *Files 10% similar despite different names*

#### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/.idea/libs_n_utils.iml` & `libs_n_utils_package_uq_2022-0.0.5.3/.idea/libs_n_utils.iml`

```diff
@@ -1,12 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <module type="PYTHON_MODULE" version="4">
   <component name="NewModuleRootManager">
     <content url="file://$MODULE_DIR$">
       <sourceFolder url="file://$MODULE_DIR$/src" isTestSource="false"/>
       <sourceFolder url="file://$MODULE_DIR$/src/libs_n_utils_package_uq_2022/lib" isTestSource="false"/>
       <sourceFolder url="file://$MODULE_DIR$/src/libs_n_utils_package_uq_2022/utilities" isTestSource="false"/>
+      <sourceFolder url="file://$MODULE_DIR$/src/libs_n_utils_package_uq_2022" isTestSource="false"/>
     </content>
     <orderEntry type="inheritedJdk"/>
     <orderEntry type="sourceFolder" forTests="false"/>
   </component>
 </module>
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/.idea/misc.xml` & `libs_n_utils_package_uq_2022-0.0.5.3/.idea/misc.xml`

 * *Files 12% similar despite different names*

#### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/.idea/misc.xml` & `libs_n_utils_package_uq_2022-0.0.5.3/.idea/misc.xml`

```diff
@@ -5,18 +5,22 @@
     <option name="openedFilesInfos">
       <list>
         <OpenedFileInfo>
           <option name="caretOffset" value="775"/>
           <option name="fileUrl" value="file://$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_plotters.py"/>
         </OpenedFileInfo>
         <OpenedFileInfo>
-          <option name="caretOffset" value="306"/>
+          <option name="caretOffset" value="154"/>
+          <option name="fileUrl" value="file://$PROJECT_DIR$/pyproject.toml"/>
+        </OpenedFileInfo>
+        <OpenedFileInfo>
+          <option name="caretOffset" value="299"/>
           <option name="fileUrl" value="file://$PROJECT_DIR$/how_to_package.txt"/>
         </OpenedFileInfo>
         <OpenedFileInfo>
-          <option name="caretOffset" value="327"/>
-          <option name="fileUrl" value="file://$PROJECT_DIR$/pyproject.toml"/>
+          <option name="caretOffset" value="0"/>
+          <option name="fileUrl" value="file://$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/config_template.py"/>
         </OpenedFileInfo>
       </list>
     </option>
   </component>
 </project>
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/.idea/workspace.xml` & `libs_n_utils_package_uq_2022-0.0.5.3/.idea/workspace.xml`

 * *Files 1% similar despite different names*

#### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/.idea/workspace.xml` & `libs_n_utils_package_uq_2022-0.0.5.3/.idea/workspace.xml`

```diff
@@ -1,14 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="9376521b-a775-41d3-aeae-0de3e0b78ca1" name="Changes" comment="">
+      <change afterPath="$PROJECT_DIR$/dist/libs_n_utils_package_uq_2022-0.0.5.2-py3-none-any.whl" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/dist/libs_n_utils_package_uq_2022-0.0.5.2.tar.gz" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/how_to_package.txt" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3-py3-none-any.whl" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3.tar.gz" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4-py3-none-any.whl" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4.tar.gz" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5-py3-none-any.whl" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1-py3-none-any.whl" afterDir="false"/>
@@ -195,15 +197,15 @@
       <workItem from="1687399095619" duration="721000"/>
       <workItem from="1687400030423" duration="911000"/>
       <workItem from="1687401811808" duration="1325000"/>
       <workItem from="1687405150720" duration="364000"/>
       <workItem from="1689917617211" duration="599000"/>
       <workItem from="1689935473555" duration="319000"/>
       <workItem from="1689935880451" duration="1388000"/>
-      <workItem from="1689939409309" duration="2442000"/>
+      <workItem from="1689939409309" duration="2759000"/>
     </task>
     <task id="LOCAL-00001" summary="This is the commit to make a package">
       <created>1687400325662</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1687400325662</updated>
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/3class_ds_select_save.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/3class_ds_select_save.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/MI_feature_importance.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/MI_feature_importance.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/RF_feature_importance.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/RF_feature_importance.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/RF_feimp_weighted_average_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/RF_feimp_weighted_average_wasserstein.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/UNSW_NB15_data_preparation.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/UNSW_NB15_data_preparation.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/alternate_feature_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/alternate_feature_wasserstein.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/average_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/average_wasserstein.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/boruta_feature_selection.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/boruta_feature_selection.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/boruta_visualisation.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/boruta_visualisation.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/combine_2feather.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/combine_2feather.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/combine_2pickles.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/combine_2pickles.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/combine_3pickles.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/combine_3pickles.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/combine_folder_csv.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/combine_folder_csv.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/compare_pickle_files_in_folder.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/compare_pickle_files_in_folder.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/config_template.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/config_template.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/csv_folder_to_feather_folder.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/csv_folder_to_feather_folder.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/csv_folder_to_pickle_folder.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/csv_folder_to_pickle_folder.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/dict_manipulation.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/dict_manipulation.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/edit_CIC.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/edit_CIC.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/edit_CIC_ton.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/edit_CIC_ton.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/feather_2m_sel_cols.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/feather_2m_sel_cols.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/feather_fldr_2_pickle_fldr.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/feather_fldr_2_pickle_fldr.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/inter_dataset_feature_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/inter_dataset_feature_wasserstein.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/intra_dataset_feature_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/intra_dataset_feature_wasserstein.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_NN_functional.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_NN_functional.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_NN_models.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_NN_models.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_binary_classification.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_binary_classification.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_data_preprocessing.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_dataframe_manipulation.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_dataframe_manipulation.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_embedding.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_embedding.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_feature_calculation.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_feature_calculation.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_file_manipulation.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_file_manipulation.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_flow.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_flow.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_helpers.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_helpers.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_imbalance.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_imbalance.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_pandas_extensions.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_pandas_extensions.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_plotters.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_plotters.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/lib_stat_distribution.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/lib_stat_distribution.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/make_cics_compatible.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/make_cics_compatible.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/make_unity_fi_pickle.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/make_unity_fi_pickle.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/my_easy_logger.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/my_easy_logger.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/netflow_preprocessing.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/netflow_preprocessing.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/pickle_fldr_2_feather_fldr.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/pickle_fldr_2_feather_fldr.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/plot_MI_feature_importances.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/plot_MI_feature_importances.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/plot_RF_feature_importance_differences.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/plot_RF_feature_importance_differences.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/print_feature_selction_results.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/print_feature_selction_results.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/reading_txt_files.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/reading_txt_files.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/sample_save_fldr_datasets.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/sample_save_fldr_datasets.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/weighted_average_alternate_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/weighted_average_alternate_wasserstein.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/weighted_average_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/weighted_average_wasserstein.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3-py3-none-any.whl` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3.tar.gz` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3.tar.gz`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4-py3-none-any.whl` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4.tar.gz` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4.tar.gz`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5-py3-none-any.whl` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1-py3-none-any.whl` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1.tar.gz` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1.tar.gz`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.tar.gz` & `libs_n_utils_package_uq_2022-0.0.5.3/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.tar.gz`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/LICENSE` & `libs_n_utils_package_uq_2022-0.0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/pyproject.toml` & `libs_n_utils_package_uq_2022-0.0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "libs_n_utils_package_uq_2022"
-version = "0.0.5.2"
+version = "0.0.5.3"
 authors = [
   { name="siamak layeghy", email="siamak.layeghy@uq.net.au" },
 ]
 description = "A small library of utilities"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.2/PKG-INFO` & `libs_n_utils_package_uq_2022-0.0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libs_n_utils_package_uq_2022
-Version: 0.0.5.2
+Version: 0.0.5.3
 Summary: A small library of utilities
 Project-URL: Homepage, https://github.com/layeghy/libs_n_utils
 Project-URL: Bug Tracker, https://github.com/layeghy/libs_n_utils/issues
 Author-email: siamak layeghy <siamak.layeghy@uq.net.au>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

