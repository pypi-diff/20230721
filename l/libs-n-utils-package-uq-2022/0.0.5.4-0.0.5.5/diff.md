# Comparing `tmp/libs_n_utils_package_uq_2022-0.0.5.4.tar.gz` & `tmp/libs_n_utils_package_uq_2022-0.0.5.5.tar.gz`

## Comparing `libs_n_utils_package_uq_2022-0.0.5.4.tar` & `libs_n_utils_package_uq_2022-0.0.5.5.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rwxr-xr-x   0        0        0      449 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/how_to_package.txt
--rwxr-xr-x   0        0        0      694 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/.idea/libs_n_utils.iml
--rwxr-xr-x   0        0        0      917 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/.idea/misc.xml
--rwxr-xr-x   0        0        0      276 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/.idea/modules.xml
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/.idea/vcs.xml
--rwxr-xr-x   0        0        0    21978 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/.idea/workspace.xml
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/.idea/inspectionProfiles/profiles_settings.xml
--rwxr-xr-x   0        0        0     2909 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/3class_ds_select_save.py
--rwxr-xr-x   0        0        0     4168 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/MI_feature_importance.py
--rwxr-xr-x   0        0        0     7432 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/RF_feature_importance.py
--rwxr-xr-x   0        0        0     3367 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/RF_feimp_weighted_average_wasserstein.py
--rwxr-xr-x   0        0        0     2090 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/UNSW_NB15_data_preparation.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/__init__.py
--rwxr-xr-x   0        0        0     5956 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/alternate_feature_wasserstein.py
--rwxr-xr-x   0        0        0      346 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/attack_types.py
--rwxr-xr-x   0        0        0     1947 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/average_wasserstein.py
--rwxr-xr-x   0        0        0     7705 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/boruta_feature_selection.py
--rwxr-xr-x   0        0        0      613 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/boruta_visualisation.py
--rwxr-xr-x   0        0        0     1878 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/combine_2feather.py
--rwxr-xr-x   0        0        0     3105 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/combine_2pickles.py
--rwxr-xr-x   0        0        0     3274 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/combine_3pickles.py
--rwxr-xr-x   0        0        0     3851 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/combine_folder_csv.py
--rwxr-xr-x   0        0        0     1051 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/compare_pickle_files_in_folder.py
--rwxr-xr-x   0        0        0    25974 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/config_template.py
--rwxr-xr-x   0        0        0      767 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/csv_folder_to_feather_folder.py
--rwxr-xr-x   0        0        0      881 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/csv_folder_to_pickle_folder.py
--rwxr-xr-x   0        0        0      494 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/datasets_information.py
--rwxr-xr-x   0        0        0     1239 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/dict_manipulation.py
--rwxr-xr-x   0        0        0     3281 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/edit_CIC.py
--rwxr-xr-x   0        0        0     1443 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/edit_CIC_ton.py
--rwxr-xr-x   0        0        0     1112 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/feather_2m_sel_cols.py
--rwxr-xr-x   0        0        0     1298 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/feather_fldr_2_pickle_fldr.py
--rwxr-xr-x   0        0        0    12322 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/inter_dataset_feature_wasserstein.py
--rwxr-xr-x   0        0        0     3215 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/intra_dataset_feature_wasserstein.py
--rwxr-xr-x   0        0        0     2747 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_NN_functional.py
--rwxr-xr-x   0        0        0     6968 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_NN_models.py
--rwxr-xr-x   0        0        0     1984 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_binary_classification.py
--rwxr-xr-x   0        0        0     7534 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_data_preprocessing.py
--rwxr-xr-x   0        0        0     3982 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_dataframe_manipulation.py
--rwxr-xr-x   0        0        0     9110 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_embedding.py
--rwxr-xr-x   0        0        0    12691 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_feature_calculation.py
--rwxr-xr-x   0        0        0    10595 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_file_manipulation.py
--rwxr-xr-x   0        0        0     3294 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_flow.py
--rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_helpers.py
--rwxr-xr-x   0        0        0     3285 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_imbalance.py
--rwxr-xr-x   0        0        0     5253 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_pandas_extensions.py
--rwxr-xr-x   0        0        0    37599 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_plotters.py
--rwxr-xr-x   0        0        0      395 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_small_utils.py
--rwxr-xr-x   0        0        0     8975 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_stat_distribution.py
--rwxr-xr-x   0        0        0     5404 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/make_cics_compatible.py
--rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/make_unity_fi_pickle.py
--rwxr-xr-x   0        0        0     4390 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/my_easy_logger.py
--rwxr-xr-x   0        0        0    14129 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/netflow_preprocessing.py
--rwxr-xr-x   0        0        0     2332 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/pickle_fldr_2_feather_fldr.py
--rwxr-xr-x   0        0        0     1402 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/plot_MI_feature_importances.py
--rwxr-xr-x   0        0        0      949 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/plot_RF_feature_importance_differences.py
--rwxr-xr-x   0        0        0     1829 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/print_feature_selction_results.py
--rwxr-xr-x   0        0        0     1293 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/reading_txt_files.py
--rwxr-xr-x   0        0        0     4726 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/sample_save_fldr_datasets.py
--rwxr-xr-x   0        0        0     4879 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/weighted_average_alternate_wasserstein.py
--rwxr-xr-x   0        0        0     3332 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/weighted_average_wasserstein.py
--rwxr-xr-x   0        0        0    79057 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3-py3-none-any.whl
--rwxr-xr-x   0        0        0    51264 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3.tar.gz
--rwxr-xr-x   0        0        0    83488 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4-py3-none-any.whl
--rwxr-xr-x   0        0        0    56778 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4.tar.gz
--rwxr-xr-x   0        0        0    83488 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5-py3-none-any.whl
--rwxr-xr-x   0        0        0    83508 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1-py3-none-any.whl
--rwxr-xr-x   0        0        0    56775 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1.tar.gz
--rwxr-xr-x   0        0        0    56776 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.tar.gz
--rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/LICENSE
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/README.md
--rwxr-xr-x   0        0        0      596 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/pyproject.toml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.4/PKG-INFO
+-rwxr-xr-x   0        0        0      449 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/how_to_package.txt
+-rwxr-xr-x   0        0        0      694 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/.idea/libs_n_utils.iml
+-rwxr-xr-x   0        0        0     2889 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/.idea/misc.xml
+-rwxr-xr-x   0        0        0      276 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/.idea/modules.xml
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/.idea/vcs.xml
+-rwxr-xr-x   0        0        0    21836 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/.idea/workspace.xml
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/.idea/inspectionProfiles/profiles_settings.xml
+-rwxr-xr-x   0        0        0     2910 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/3class_ds_select_save.py
+-rwxr-xr-x   0        0        0     4170 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/MI_feature_importance.py
+-rwxr-xr-x   0        0        0     7434 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/RF_feature_importance.py
+-rwxr-xr-x   0        0        0     3370 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/RF_feimp_weighted_average_wasserstein.py
+-rwxr-xr-x   0        0        0     2042 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/UNSW_NB15_data_preparation.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/__init__.py
+-rwxr-xr-x   0        0        0     5959 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/alternate_feature_wasserstein.py
+-rwxr-xr-x   0        0        0      346 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/attack_types.py
+-rwxr-xr-x   0        0        0     1950 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/average_wasserstein.py
+-rwxr-xr-x   0        0        0     7707 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/boruta_feature_selection.py
+-rwxr-xr-x   0        0        0      613 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/boruta_visualisation.py
+-rwxr-xr-x   0        0        0     1879 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/combine_2feather.py
+-rwxr-xr-x   0        0        0     3106 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/combine_2pickles.py
+-rwxr-xr-x   0        0        0     3275 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/combine_3pickles.py
+-rwxr-xr-x   0        0        0     3853 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/combine_folder_csv.py
+-rwxr-xr-x   0        0        0      997 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/compare_pickle_files_in_folder.py
+-rwxr-xr-x   0        0        0    25974 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/config_template.py
+-rwxr-xr-x   0        0        0      769 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/csv_folder_to_feather_folder.py
+-rwxr-xr-x   0        0        0      883 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/csv_folder_to_pickle_folder.py
+-rwxr-xr-x   0        0        0      494 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/datasets_information.py
+-rwxr-xr-x   0        0        0     1239 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/dict_manipulation.py
+-rwxr-xr-x   0        0        0     3281 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/edit_CIC.py
+-rwxr-xr-x   0        0        0     1445 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/edit_CIC_ton.py
+-rwxr-xr-x   0        0        0     1112 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/feather_2m_sel_cols.py
+-rwxr-xr-x   0        0        0     1300 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/feather_fldr_2_pickle_fldr.py
+-rwxr-xr-x   0        0        0    12326 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/inter_dataset_feature_wasserstein.py
+-rwxr-xr-x   0        0        0     3219 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/intra_dataset_feature_wasserstein.py
+-rwxr-xr-x   0        0        0     2758 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_NN_functional.py
+-rwxr-xr-x   0        0        0     6969 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_NN_models.py
+-rwxr-xr-x   0        0        0     1970 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_binary_classification.py
+-rwxr-xr-x   0        0        0     7536 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_data_preprocessing.py
+-rwxr-xr-x   0        0        0     3983 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_dataframe_manipulation.py
+-rwxr-xr-x   0        0        0     9119 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_embedding.py
+-rwxr-xr-x   0        0        0    12694 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_feature_calculation.py
+-rwxr-xr-x   0        0        0    10597 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_file_manipulation.py
+-rwxr-xr-x   0        0        0     3295 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_flow.py
+-rwxr-xr-x   0        0        0     1284 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_helpers.py
+-rwxr-xr-x   0        0        0     3285 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_imbalance.py
+-rwxr-xr-x   0        0        0     5205 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_pandas_extensions.py
+-rwxr-xr-x   0        0        0    37608 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_plotters.py
+-rwxr-xr-x   0        0        0      395 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_small_utils.py
+-rwxr-xr-x   0        0        0     8979 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_stat_distribution.py
+-rwxr-xr-x   0        0        0     5405 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/make_cics_compatible.py
+-rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/make_unity_fi_pickle.py
+-rwxr-xr-x   0        0        0     4390 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/my_easy_logger.py
+-rwxr-xr-x   0        0        0    14129 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/netflow_preprocessing.py
+-rwxr-xr-x   0        0        0     2333 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/pickle_fldr_2_feather_fldr.py
+-rwxr-xr-x   0        0        0     1403 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/plot_MI_feature_importances.py
+-rwxr-xr-x   0        0        0      949 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/plot_RF_feature_importance_differences.py
+-rwxr-xr-x   0        0        0     1830 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/print_feature_selction_results.py
+-rwxr-xr-x   0        0        0     1293 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/reading_txt_files.py
+-rwxr-xr-x   0        0        0     4697 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/sample_save_fldr_datasets.py
+-rwxr-xr-x   0        0        0     4880 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/weighted_average_alternate_wasserstein.py
+-rwxr-xr-x   0        0        0     3335 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/weighted_average_wasserstein.py
+-rwxr-xr-x   0        0        0    79057 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3-py3-none-any.whl
+-rwxr-xr-x   0        0        0    51264 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3.tar.gz
+-rwxr-xr-x   0        0        0    83488 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4-py3-none-any.whl
+-rwxr-xr-x   0        0        0    56778 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4.tar.gz
+-rwxr-xr-x   0        0        0    83488 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5-py3-none-any.whl
+-rwxr-xr-x   0        0        0    83508 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1-py3-none-any.whl
+-rwxr-xr-x   0        0        0    56775 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1.tar.gz
+-rwxr-xr-x   0        0        0    56776 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.tar.gz
+-rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/LICENSE
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/README.md
+-rwxr-xr-x   0        0        0      636 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.5.5/PKG-INFO
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/.idea/libs_n_utils.iml` & `libs_n_utils_package_uq_2022-0.0.5.5/.idea/libs_n_utils.iml`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/.idea/misc.xml` & `libs_n_utils_package_uq_2022-0.0.5.5/.idea/misc.xml`

 * *Files 24% similar despite different names*

#### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/.idea/misc.xml` & `libs_n_utils_package_uq_2022-0.0.5.5/.idea/misc.xml`

```diff
@@ -1,22 +1,54 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ProjectRootManager" version="2" project-jdk-name="Python 3.8" project-jdk-type="Python SDK"/>
   <component name="UnattendedHostPersistenceState">
     <option name="openedFilesInfos">
       <list>
         <OpenedFileInfo>
-          <option name="caretOffset" value="775"/>
-          <option name="fileUrl" value="file://$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_plotters.py"/>
+          <option name="caretOffset" value="95"/>
+          <option name="fileUrl" value="file://$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/pickle_fldr_2_feather_fldr.py"/>
         </OpenedFileInfo>
         <OpenedFileInfo>
-          <option name="caretOffset" value="141"/>
-          <option name="fileUrl" value="file://$PROJECT_DIR$/pyproject.toml"/>
+          <option name="caretOffset" value="73"/>
+          <option name="fileUrl" value="file://$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/plot_MI_feature_importances.py"/>
         </OpenedFileInfo>
         <OpenedFileInfo>
-          <option name="caretOffset" value="299"/>
-          <option name="fileUrl" value="file://$PROJECT_DIR$/how_to_package.txt"/>
+          <option name="caretOffset" value="0"/>
+          <option name="fileUrl" value="file://$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/plot_RF_feature_importance_differences.py"/>
+        </OpenedFileInfo>
+        <OpenedFileInfo>
+          <option name="caretOffset" value="114"/>
+          <option name="fileUrl" value="file://$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/print_feature_selction_results.py"/>
+        </OpenedFileInfo>
+        <OpenedFileInfo>
+          <option name="caretOffset" value="0"/>
+          <option name="fileUrl" value="file://$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/reading_txt_files.py"/>
+        </OpenedFileInfo>
+        <OpenedFileInfo>
+          <option name="caretOffset" value="198"/>
+          <option name="fileUrl" value="file://$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/RF_feature_importance.py"/>
+        </OpenedFileInfo>
+        <OpenedFileInfo>
+          <option name="caretOffset" value="171"/>
+          <option name="fileUrl" value="file://$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/RF_feimp_weighted_average_wasserstein.py"/>
+        </OpenedFileInfo>
+        <OpenedFileInfo>
+          <option name="caretOffset" value="182"/>
+          <option name="fileUrl" value="file://$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/sample_save_fldr_datasets.py"/>
+        </OpenedFileInfo>
+        <OpenedFileInfo>
+          <option name="caretOffset" value="55"/>
+          <option name="fileUrl" value="file://$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/UNSW_NB15_data_preparation.py"/>
+        </OpenedFileInfo>
+        <OpenedFileInfo>
+          <option name="caretOffset" value="527"/>
+          <option name="fileUrl" value="file://$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/weighted_average_alternate_wasserstein.py"/>
+        </OpenedFileInfo>
+        <OpenedFileInfo>
+          <option name="caretOffset" value="0"/>
+          <option name="fileUrl" value="file://$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/weighted_average_wasserstein.py"/>
         </OpenedFileInfo>
       </list>
     </option>
   </component>
 </project>
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/.idea/workspace.xml` & `libs_n_utils_package_uq_2022-0.0.5.5/.idea/workspace.xml`

 * *Files 17% similar despite different names*

#### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/.idea/workspace.xml` & `libs_n_utils_package_uq_2022-0.0.5.5/.idea/workspace.xml`

```diff
@@ -3,80 +3,60 @@
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="9376521b-a775-41d3-aeae-0de3e0b78ca1" name="Changes" comment="">
       <change afterPath="$PROJECT_DIR$/dist/libs_n_utils_package_uq_2022-0.0.5.2-py3-none-any.whl" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/dist/libs_n_utils_package_uq_2022-0.0.5.2.tar.gz" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/dist/libs_n_utils_package_uq_2022-0.0.5.3-py3-none-any.whl" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/dist/libs_n_utils_package_uq_2022-0.0.5.3.tar.gz" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/dist/libs_n_utils_package_uq_2022-0.0.5.4-py3-none-any.whl" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/dist/libs_n_utils_package_uq_2022-0.0.5.4.tar.gz" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/how_to_package.txt" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3-py3-none-any.whl" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3.tar.gz" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4-py3-none-any.whl" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4.tar.gz" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5-py3-none-any.whl" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1-py3-none-any.whl" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1.tar.gz" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.tar.gz" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/.idea/libs_n_utils.iml" beforeDir="false" afterPath="$PROJECT_DIR$/.idea/libs_n_utils.iml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/3class_ds_select_save.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/3class_ds_select_save.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/MI_feature_importance.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/MI_feature_importance.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/RF_feature_importance.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/RF_feature_importance.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/RF_feimp_weighted_average_wasserstein.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/RF_feimp_weighted_average_wasserstein.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/UNSW_NB15_data_preparation.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/UNSW_NB15_data_preparation.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/alternate_feature_wasserstein.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/alternate_feature_wasserstein.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/attack_types.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/attack_types.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/average_wasserstein.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/average_wasserstein.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/boruta_feature_selection.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/boruta_feature_selection.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/boruta_visualisation.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/boruta_visualisation.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/combine_2feather.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/combine_2feather.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/combine_2pickles.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/combine_2pickles.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/combine_3pickles.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/combine_3pickles.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/combine_folder_csv.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/combine_folder_csv.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/compare_pickle_files_in_folder.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/compare_pickle_files_in_folder.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/config_template.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/config_template.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/csv_folder_to_feather_folder.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/csv_folder_to_feather_folder.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/csv_folder_to_pickle_folder.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/csv_folder_to_pickle_folder.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/datasets_information.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/datasets_information.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/dict_manipulation.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/dict_manipulation.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/edit_CIC.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/edit_CIC.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/edit_CIC_ton.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/edit_CIC_ton.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/feather_2m_sel_cols.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/feather_2m_sel_cols.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/feather_fldr_2_pickle_fldr.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/feather_fldr_2_pickle_fldr.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/inter_dataset_feature_wasserstein.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/inter_dataset_feature_wasserstein.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/intra_dataset_feature_wasserstein.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/intra_dataset_feature_wasserstein.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lib_NN_functional.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_NN_functional.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lib_NN_models.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_NN_models.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lib_binary_classification.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_binary_classification.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lib_data_preprocessing.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_data_preprocessing.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lib_dataframe_manipulation.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_dataframe_manipulation.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lib_embedding.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_embedding.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lib_feature_calculation.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_feature_calculation.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lib_file_manipulation.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_file_manipulation.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lib_flow.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_flow.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lib_helpers.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_helpers.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lib_imbalance.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_imbalance.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lib_pandas_extensions.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_pandas_extensions.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lib_plotters.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_plotters.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lib_small_utils.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_small_utils.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lib_stat_distribution.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_stat_distribution.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/LICENSE" beforeDir="false" afterPath="$PROJECT_DIR$/LICENSE" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/make_cics_compatible.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/make_cics_compatible.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/make_unity_fi_pickle.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/make_unity_fi_pickle.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/my_easy_logger.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/my_easy_logger.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/netflow_preprocessing.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/netflow_preprocessing.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/pickle_fldr_2_feather_fldr.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/pickle_fldr_2_feather_fldr.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/plot_MI_feature_importances.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/plot_MI_feature_importances.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/plot_RF_feature_importance_differences.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/plot_RF_feature_importance_differences.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/print_feature_selction_results.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/print_feature_selction_results.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/reading_txt_files.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/reading_txt_files.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/sample_save_fldr_datasets.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/sample_save_fldr_datasets.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/weighted_average_alternate_wasserstein.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/weighted_average_alternate_wasserstein.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/weighted_average_wasserstein.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/weighted_average_wasserstein.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/3class_ds_select_save.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/3class_ds_select_save.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/MI_feature_importance.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/MI_feature_importance.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/RF_feature_importance.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/RF_feature_importance.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/RF_feimp_weighted_average_wasserstein.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/RF_feimp_weighted_average_wasserstein.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/UNSW_NB15_data_preparation.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/UNSW_NB15_data_preparation.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/alternate_feature_wasserstein.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/alternate_feature_wasserstein.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/average_wasserstein.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/average_wasserstein.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/boruta_feature_selection.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/boruta_feature_selection.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/combine_2feather.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/combine_2feather.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/combine_2pickles.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/combine_2pickles.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/combine_3pickles.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/combine_3pickles.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/combine_folder_csv.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/combine_folder_csv.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/compare_pickle_files_in_folder.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/compare_pickle_files_in_folder.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/csv_folder_to_feather_folder.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/csv_folder_to_feather_folder.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/csv_folder_to_pickle_folder.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/csv_folder_to_pickle_folder.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/edit_CIC_ton.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/edit_CIC_ton.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/feather_fldr_2_pickle_fldr.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/feather_fldr_2_pickle_fldr.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/inter_dataset_feature_wasserstein.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/inter_dataset_feature_wasserstein.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/intra_dataset_feature_wasserstein.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/intra_dataset_feature_wasserstein.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_NN_functional.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_NN_functional.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_NN_models.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_NN_models.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_binary_classification.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_binary_classification.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_data_preprocessing.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_data_preprocessing.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_dataframe_manipulation.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_dataframe_manipulation.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_embedding.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_embedding.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_feature_calculation.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_feature_calculation.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_file_manipulation.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_file_manipulation.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_flow.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_flow.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_helpers.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_helpers.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_pandas_extensions.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_pandas_extensions.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_plotters.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_plotters.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_stat_distribution.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_stat_distribution.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/make_cics_compatible.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/make_cics_compatible.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/pickle_fldr_2_feather_fldr.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/pickle_fldr_2_feather_fldr.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/plot_MI_feature_importances.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/plot_MI_feature_importances.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/print_feature_selction_results.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/print_feature_selction_results.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/sample_save_fldr_datasets.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/sample_save_fldr_datasets.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/weighted_average_alternate_wasserstein.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/weighted_average_alternate_wasserstein.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/weighted_average_wasserstein.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/weighted_average_wasserstein.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -128,15 +108,15 @@
       <recent name="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022"/>
       <recent name="$PROJECT_DIR$"/>
       <recent name="$PROJECT_DIR$/src"/>
       <recent name="$PROJECT_DIR$/libs_n_utils_package_uq_2022"/>
       <recent name="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib"/>
     </key>
   </component>
-  <component name="RunManager" selected="Python.3class_ds_select_save">
+  <component name="RunManager" selected="Python.lib_plotters">
     <configuration name="3class_ds_select_save" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="libs_n_utils"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
@@ -173,16 +153,39 @@
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
+    <configuration name="lib_plotters" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
+      <module name="libs_n_utils"/>
+      <option name="INTERPRETER_OPTIONS" value=""/>
+      <option name="PARENT_ENVS" value="true"/>
+      <envs>
+        <env name="PYTHONUNBUFFERED" value="1"/>
+      </envs>
+      <option name="SDK_HOME" value=""/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022"/>
+      <option name="IS_MODULE_SDK" value="true"/>
+      <option name="ADD_CONTENT_ROOTS" value="true"/>
+      <option name="ADD_SOURCE_ROOTS" value="true"/>
+      <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
+      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_plotters.py"/>
+      <option name="PARAMETERS" value=""/>
+      <option name="SHOW_COMMAND_LINE" value="false"/>
+      <option name="EMULATE_TERMINAL" value="false"/>
+      <option name="MODULE_MODE" value="false"/>
+      <option name="REDIRECT_INPUT" value="false"/>
+      <option name="INPUT_FILE" value=""/>
+      <method v="2"/>
+    </configuration>
     <recent_temporary>
       <list>
+        <item itemvalue="Python.lib_plotters"/>
         <item itemvalue="Python.3class_ds_select_save"/>
         <item itemvalue="Python.lib_flow"/>
       </list>
     </recent_temporary>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
@@ -197,15 +200,15 @@
       <workItem from="1687399095619" duration="721000"/>
       <workItem from="1687400030423" duration="911000"/>
       <workItem from="1687401811808" duration="1325000"/>
       <workItem from="1687405150720" duration="364000"/>
       <workItem from="1689917617211" duration="599000"/>
       <workItem from="1689935473555" duration="319000"/>
       <workItem from="1689935880451" duration="1388000"/>
-      <workItem from="1689939409309" duration="2759000"/>
+      <workItem from="1689939409309" duration="3514000"/>
     </task>
     <task id="LOCAL-00001" summary="This is the commit to make a package">
       <created>1687400325662</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1687400325662</updated>
@@ -227,15 +230,22 @@
     <task id="LOCAL-00004" summary="This is the commit to make a package">
       <created>1687405210053</created>
       <option name="number" value="00004"/>
       <option name="presentableId" value="LOCAL-00004"/>
       <option name="project" value="LOCAL"/>
       <updated>1687405210053</updated>
     </task>
-    <option name="localTasksCounter" value="5"/>
+    <task id="LOCAL-00005" summary="This is the commit to make a package">
+      <created>1689943754085</created>
+      <option name="number" value="00005"/>
+      <option name="presentableId" value="LOCAL-00005"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1689943754085</updated>
+    </task>
+    <option name="localTasksCounter" value="6"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="VcsManagerConfiguration">
     <option name="ADD_EXTERNAL_FILES_SILENTLY" value="true"/>
@@ -251,15 +261,25 @@
           <option name="timeStamp" value="1"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/3class_ds_select_save.py</url>
           <line>13</line>
           <option name="timeStamp" value="2"/>
         </line-breakpoint>
+        <line-breakpoint enabled="true" type="python-line">
+          <url>file://$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib_plotters.py</url>
+          <line>5</line>
+          <option name="timeStamp" value="3"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" type="python-line">
+          <url>file://$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/boruta_visualisation.py</url>
+          <option name="timeStamp" value="4"/>
+        </line-breakpoint>
       </breakpoints>
     </breakpoint-manager>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
     <SUITE FILE_PATH="coverage/libs_n_utils$3class_ds_select_save.coverage" NAME="3class_ds_select_save Coverage Results" MODIFIED="1689935915825" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/src"/>
     <SUITE FILE_PATH="coverage/libs_n_utils$lib_flow.coverage" NAME="lib_flow Coverage Results" MODIFIED="1687401885232" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022/lib"/>
+    <SUITE FILE_PATH="coverage/libs_n_utils$lib_plotters.coverage" NAME="lib_plotters Coverage Results" MODIFIED="1689943953690" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/src/libs_n_utils_package_uq_2022"/>
   </component>
 </project>
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/3class_ds_select_save.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/3class_ds_select_save.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 
 import os
 import pickle
 import gc
 import inspect
-from my_easy_logger import my_logger
+from .my_easy_logger import my_logger
 import time
 
 filename = os.path.split(__file__)[1]
 
 
 def select_dos_rows(_src_fldr, _dst_fldr, new_name_ext='3class_'):
     func_name = inspect.stack()[0][3]
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/MI_feature_importance.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/MI_feature_importance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import inspect
 import os
 import _pickle as pickle
 import warnings
 import pandas as pd
-from intra_dataset_feature_wasserstein import get_dataset_prepared
+from .intra_dataset_feature_wasserstein import get_dataset_prepared
 import numpy as np
 from sklearn.feature_selection import mutual_info_regression, mutual_info_classif
-from my_easy_logger import my_logger, logger_cleaner
+from .my_easy_logger import my_logger, logger_cleaner
 
 script_name = os.path.split(__file__)[1][:-3]
 
 
 
 
 # ---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/RF_feature_importance.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/RF_feature_importance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
 import os
 import warnings
 import pandas as pd
 import _pickle as pickle
 from sklearn.ensemble import RandomForestClassifier
-from my_easy_logger import my_logger, logger_cleaner
-from intra_dataset_feature_wasserstein import get_dataset_prepared
+from .my_easy_logger import my_logger, logger_cleaner
+from .intra_dataset_feature_wasserstein import get_dataset_prepared
 
 script_name = os.path.split(__file__)[1][:-3]
 logger = my_logger(
     reporter_file_name=script_name,
     info_c='bold_blue',
     reporter_func_name=__name__,
     log_level='debug'
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/RF_feimp_weighted_average_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/RF_feimp_weighted_average_wasserstein.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import numpy as np
 import _pickle as pickle
-from intra_dataset_feature_wasserstein import plot_wasserstein_table
-from lib_plotters import draw_bar_chart
-from my_easy_logger import my_logger
+from .intra_dataset_feature_wasserstein import plot_wasserstein_table
+from .lib_plotters import draw_bar_chart
+from .my_easy_logger import my_logger
 
 script_name = os.path.split(__file__)[1]
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/UNSW_NB15_data_preparation.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/UNSW_NB15_data_preparation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import os
 import pandas as pd
 from pathlib import Path
 
-from sklearn.preprocessing import MinMaxScaler
-
 fldr = '/storage/datasets/originals/UNSW-NB15_CSV_Files/'
 info_file_addr = os.path.join(fldr, 'NUSW-NB15_features.csv')
 info_data = pd.read_csv(info_file_addr, encoding='unicode_escape')
 df_header = info_data['Name'].tolist()
 
 print("Loading files...")
 df = pd.DataFrame()
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/alternate_feature_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/alternate_feature_wasserstein.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 import inspect
 import os
 import _pickle as pickle
 import pandas as pd
 from scipy.stats import wasserstein_distance
 
-from intra_dataset_feature_wasserstein import get_dataset_prepared
-from lib_plotters import draw_bar_chart
-from my_easy_logger import my_logger, logger_cleaner
+from .intra_dataset_feature_wasserstein import get_dataset_prepared
+from .lib_plotters import draw_bar_chart
+from .my_easy_logger import my_logger, logger_cleaner
 
 script_name = os.path.split(__file__)[1][:-3]
 logger = my_logger(
     reporter_file_name=script_name,
     info_c='bold_blue',
     reporter_func_name=__name__,
     log_level='debug'
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/average_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/average_wasserstein.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import numpy as np
 import _pickle as pickle
-from intra_dataset_feature_wasserstein import plot_wasserstein_table
-from lib_plotters import draw_bar_chart
-from my_easy_logger import my_logger
+from .intra_dataset_feature_wasserstein import plot_wasserstein_table
+from .lib_plotters import draw_bar_chart
+from .my_easy_logger import my_logger
 
 script_name = os.path.split(__file__)[1]
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/boruta_feature_selection.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/boruta_feature_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import inspect
 import os
 import warnings
 import pandas as pd
 import _pickle as pickle
 from sklearn.ensemble import RandomForestClassifier
 from boruta import BorutaPy
-from my_easy_logger import my_logger, logger_cleaner
-from intra_dataset_feature_wasserstein import get_dataset_prepared
+from .my_easy_logger import my_logger, logger_cleaner
+from .intra_dataset_feature_wasserstein import get_dataset_prepared
 
 script_name = os.path.split(__file__)[1][:-3]
 logger = my_logger(
     reporter_file_name=script_name,
     info_c='bold_blue',
     reporter_func_name=__name__,
     log_level='debug'
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/boruta_visualisation.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/boruta_visualisation.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/combine_2feather.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/combine_2feather.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import pandas as pd
 import feather
-from my_easy_logger import my_logger
+from .my_easy_logger import my_logger
 
 filename = os.path.split(__file__)[1]
 
 
 def combine_2feather(feather_file1, feather_file2):
     logger_ = my_logger(reporter_file_name=filename,
                         reporter_func_name=__name__,
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/combine_2pickles.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/combine_2pickles.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import itertools
 import os
 import pandas as pd
 import pickle
 import gc
 from functools import lru_cache
 from datetime import datetime
-from my_easy_logger import my_logger, logger_cleaner
+from .my_easy_logger import my_logger, logger_cleaner
 
 scriptname = os.path.split(__file__)[1]
 
 @logger_cleaner
 @lru_cache()
 def combine_2pickle(pickle_file1, pickle_file2, **kwargs):
     func_name = inspect.stack()[0][3]
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/combine_3pickles.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/combine_3pickles.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import pandas as pd
 import pickle
 import gc
 import itertools
 from datetime import datetime
 from functools import lru_cache
-from my_easy_logger import my_logger, logger_cleaner
+from .my_easy_logger import my_logger, logger_cleaner
 
 scriptname = os.path.split(__file__)[1]
 
 
 # ~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X
 @logger_cleaner
 @lru_cache()
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/combine_folder_csv.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/combine_folder_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import pandas as pd
 import gc
 import _pickle as pickle
 import datetime
 
-from my_easy_logger import my_logger
-from lib_pandas_extensions import rapid_csv_read
+from .my_easy_logger import my_logger
+from .lib_pandas_extensions import rapid_csv_read
 
 filename = os.path.split(__file__)[1]
 
 
 
 if __name__ == '__main__':
     log_file = f'../../outputs/logs/{filename[:-3]}-' \
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/config_template.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/config_template.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/csv_folder_to_feather_folder.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/csv_folder_to_feather_folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
-from lib_file_manipulation import csvfile_2_featherfile
-from config_template import FlowMeter
+from .lib_file_manipulation import csvfile_2_featherfile
+from .config_template import FlowMeter
 
 cols = FlowMeter.columns
 
 csv_folder = '/storage/datasets/Comscentre2017/Elasticsearch_CSV_full_headers/'
 feather_folder = '/storage/datasets/Comscentre2017/feather/'
 
 if not os.path.isdir(feather_folder):
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/csv_folder_to_pickle_folder.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/csv_folder_to_pickle_folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
-from lib_file_manipulation import csvfile_2_picklefile
-from config_template import FlowMeter
+from .lib_file_manipulation import csvfile_2_picklefile
+from .config_template import FlowMeter
 
 
 cols = FlowMeter.columns
 
 csv_folder = '/storage/datasets/FlowMeter/csv/'
 pickle_folder = '/storage/datasets/FlowMeter/1pickle/'
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/dict_manipulation.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/dict_manipulation.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/edit_CIC.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/edit_CIC.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/edit_CIC_ton.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/edit_CIC_ton.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import pandas as pd
-from config_template import FlowMeter as FM
-from my_easy_logger import my_logger
+from .config_template import FlowMeter as FM
+from .my_easy_logger import my_logger
 import _pickle as pickle
 
 
 cols = FM.columns
 to_replace = FM.replace_these
 script_name = os.path.split(__file__)[1][:-3]
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/feather_2m_sel_cols.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/feather_2m_sel_cols.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/feather_fldr_2_pickle_fldr.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/feather_fldr_2_pickle_fldr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import gc
 import pandas as pd
 import _pickle as pickle
-from my_easy_logger import my_logger
-from pickle_fldr_2_feather_fldr import get_df_dtypes
+from .my_easy_logger import my_logger
+from .pickle_fldr_2_feather_fldr import get_df_dtypes
 
 filename = os.path.split(__file__)[1]
 
 
 
 if __name__ == '__main__':
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/inter_dataset_feature_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/inter_dataset_feature_wasserstein.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 import os
 import pickle
 import re
 
 import numpy as np
 
-from config_template import NetFlow_v2, FlowMeter
-from lib_plotters import plot_wasserstein_table
-from lib_stat_distribution import inter_dataset_wasserstein_table
-from my_easy_logger import my_logger, logger_cleaner
+from .config_template import NetFlow_v2, FlowMeter
+from .lib_plotters import plot_wasserstein_table
+from .lib_stat_distribution import inter_dataset_wasserstein_table
+from .my_easy_logger import my_logger, logger_cleaner
 
 script_name = os.path.split(__file__)[1][:-3]
 
 
 
 
 @logger_cleaner
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/intra_dataset_feature_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/intra_dataset_feature_wasserstein.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 This scripts computes the wasserstein distances between attack classes
 and plots them using heat-maps
 """
 
 import os
 
-from lib_data_preprocessing import get_dataset_prepared
-from lib_plotters import plot_wasserstein_table
-from lib_stat_distribution import intra_dataset_wasserstein_table
-from my_easy_logger import my_logger, logger_cleaner
+from .lib_data_preprocessing import get_dataset_prepared
+from .lib_plotters import plot_wasserstein_table
+from .lib_stat_distribution import intra_dataset_wasserstein_table
+from .my_easy_logger import my_logger, logger_cleaner
 
 script_name = os.path.split(__file__)[1][:-3]
 
 
 
 
 # ---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_NN_functional.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_NN_functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import inspect
 import tensorflow as tf
-from my_easy_logger import my_logger
+from .my_easy_logger import my_logger
+import os
 
 filename = os.path.split(__file__)[1]
 info_log_color = 'fg_bold_purple,bg_white'
 
 METRICS = [
     tf.keras.metrics.TruePositives(name='tp'),
     tf.keras.metrics.FalsePositives(name='fp'),
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_NN_models.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_NN_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 import os
 import tensorflow as tf
-from my_easy_logger import my_logger
+from .my_easy_logger import my_logger
 
 filename = os.path.split(__file__)[1]
 info_log_color = 'fg_bold_purple,bg_white'
 # TODO: BatchNormalization 
 
 # metrics for evaluation (not loss function) --------
 METRICS = [
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_binary_classification.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_binary_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
-# import psutil
-from my_easy_logger import my_logger
-from config_template import NetFlow_v2, NN
+from .my_easy_logger import my_logger
+from .config_template import NetFlow_v2, NN
 import inspect
 
 seed_ = NN.seeds
 script_name = os.path.split(__file__)[1][:-3]
 logger = my_logger(
     reporter_file_name=script_name,
     info_c='fg_blue,bg_black',
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_data_preprocessing.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_data_preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import os
 import _pickle as pickle
 import feather
 import numpy as np
 import pandas as pd
 from sklearn import preprocessing
 from sklearn.model_selection import train_test_split
-from lib_binary_classification import netflow_identifiers, seed_, netflow_columns
-from my_easy_logger import logger_cleaner
+from .lib_binary_classification import netflow_identifiers, seed_, netflow_columns
+from .my_easy_logger import logger_cleaner
 
 
 
 
 
 # ---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**
 @logger_cleaner
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_dataframe_manipulation.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_dataframe_manipulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 import numpy as np
 import os
 
-from my_easy_logger import my_logger
+from .my_easy_logger import my_logger
 
 filename = os.path.split(__file__)[1]
 info_log_color = 'fg_bold_purple,bg_white'
 
 
 # ######################################################################################################################
 def nunique_groups(dataframe, field_list, value_field=None, log_msg=None):
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_embedding.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import pandas as pd
 from sklearn.decomposition import PCA
 from sklearn.manifold import TSNE, LocallyLinearEmbedding, MDS, SpectralEmbedding
 from sklearn.preprocessing import StandardScaler, MinMaxScaler
 from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
 from sklearn.impute import SimpleImputer
 import numpy as np
-import config_template
-from lib_feature_calculation import features_calculation
-from my_easy_logger import logger_cleaner
+from . import config_template
+from .lib_feature_calculation import features_calculation
+from .my_easy_logger import logger_cleaner
 import matplotpyplot as plt
 
 script_name = os.path.split(__file__)[1]
 groupby_features = config_template.features.groupby_features
 features_class = config_template.features()
 ds_colors = config_template.plot_parameters.dataset_edgecolors
 ds_short_names = config_template.plot_parameters.dataset_shorts
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_feature_calculation.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_feature_calculation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 import _pickle as pickle
 import feather
 import pandas as pd
 import config_template
 import os
 from datetime import datetime
-from my_easy_logger import logger_cleaner
-from config_template import NetFlow_fields
-from lib_file_manipulation import create_ReadMe
+from .my_easy_logger import logger_cleaner
+from .config_template import NetFlow_fields
+from .lib_file_manipulation import create_ReadMe
 
 param_dic = config_template.plot_parameters.CDFplot_params_dic
 groupby_features = config_template.features.groupby_features
 features_class = config_template.features()
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_file_manipulation.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_file_manipulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import re
 import time
 import feather
 import _pickle as pickle
 import gc
 import pandas as pd
 
-from lib_pandas_extensions import rapid_csv_read
-from my_easy_logger import my_logger, logger_cleaner
+from .lib_pandas_extensions import rapid_csv_read
+from .my_easy_logger import my_logger, logger_cleaner
 
 filename = os.path.split(__file__)[1]
 info_log_color = 'fg_bold_black,bg_white'
 
 
 # ######################################################################################################################
 @logger_cleaner
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_flow.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 import pandas as pd
 import os
 
-from my_easy_logger import my_logger
+from .my_easy_logger import my_logger
 
 filename = os.path.split(__file__)[1]
 info_log_color = 'blue,bg_white'
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_helpers.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import inspect
 
-from my_easy_logger import my_logger
+from .my_easy_logger import my_logger
 
 filename = os.path.split(__file__)[1]
 info_log_color = 'black,bg_white'
 
 
 
 # ######################################################################################################################
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_imbalance.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_imbalance.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_pandas_extensions.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_pandas_extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # written by Liam
 
 import gc
 import numpy as np
 import pandas as pd
-from typing import List, Tuple, Union, Optional
 import sys
 import os
 
 
 def rapid_csv_read(file_path, sample_rows: int = 10_000, verbose: bool = False, max_rows=None, skip_rows=0,
                    full_resolution_float: bool = False, contains_na: bool = True, blank_is_na: bool = False,
                    usecols=None, **kwargs):
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_plotters.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_plotters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import dill
 import pandas as pd
 import seaborn as sns
 import numpy as np
 import os
-import config_template
+from . import config_template
 import matplotlib.transforms
 from matplotlib import pyplot as plt
 from plotly import express as px
-from my_easy_logger import logger_cleaner
-from lib_small_utils import random_hex_color
+from .my_easy_logger import logger_cleaner
+from .lib_small_utils import random_hex_color
 
 
 param_dic = config_template.plot_parameters.CDFplot_params_dic
 dataset_colors = config_template.plot_parameters.dataset_colors
 
 filename = os.path.split(__file__)[1]
 info_log_color = 'purple,bg_yellow'
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/lib_stat_distribution.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/lib_stat_distribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import pickle as pickle
 import sys
 
 import numpy as np
 from scipy.stats import wasserstein_distance
-from config_template import NN
-from lib_data_preprocessing import get_binary_prepared
-from lib_plotters import plot_hist_list
-from my_easy_logger import logger_cleaner
+from .config_template import NN
+from .lib_data_preprocessing import get_binary_prepared
+from .lib_plotters import plot_hist_list
+from .my_easy_logger import logger_cleaner
 
 seed_ = NN.seeds
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 @logger_cleaner
 def compute_CDF(_values_df, column=0, **kwargs):
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/make_cics_compatible.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/make_cics_compatible.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from config_template import FlowMeter as FM
+from .config_template import FlowMeter as FM
 
 
 CIC_IDS_2018 = ['ACK Flag Cnt', 'Active Max', 'Active Mean', 'Active Min', 'Active Std', 'Attack', 'Bwd Blk Rate Avg',
                 'Bwd Byts/b Avg', 'Bwd Header Len', 'Bwd IAT Max', 'Bwd IAT Mean', 'Bwd IAT Min', 'Bwd IAT Std',
                 'Bwd IAT Tot', 'Bwd PSH Flags', 'Bwd Pkt Len Max', 'Bwd Pkt Len Mean', 'Bwd Pkt Len Min',
                 'Bwd Pkt Len Std', 'Bwd Pkts/b Avg', 'Bwd Pkts/s', 'Bwd Seg Size Avg', 'Bwd URG Flags',
                 'CWE Flag Count', 'Down/Up Ratio', 'Dst IP', 'Dst Port', 'ECE Flag Cnt', 'FIN Flag Cnt',
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/make_unity_fi_pickle.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/make_unity_fi_pickle.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/my_easy_logger.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/my_easy_logger.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/netflow_preprocessing.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/netflow_preprocessing.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/pickle_fldr_2_feather_fldr.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/pickle_fldr_2_feather_fldr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import gc
 from typing import Dict, Any
 
 import pandas as pd
 import numpy as np
-from my_easy_logger import my_logger
+from .my_easy_logger import my_logger
 
 filename = os.path.split(__file__)[1]
 
 
 def get_df_dtypes(df, full_resolution_float: bool = False):
     dtype_map: Dict[Any, str] = {}
     for col in df.columns:
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/plot_MI_feature_importances.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/plot_MI_feature_importances.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import _pickle as pickle
 import os
 import matplotlib.pyplot as plt
-from lib_plotters import draw_bar_chart
+from .lib_plotters import draw_bar_chart
 
 fn = 'feature_importance_using_mi_39_features_NF-UNSW-NB15-v2_whole_rows.pickle'
 fldr = '/home/nids1/Desktop/ZSL_visualizations'
 addr = os.path.join(fldr, fn)
 mi_dict = pickle.load(open(addr, 'rb'))
 keys = list(mi_dict.keys())
 attacks = keys[:-1]
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/plot_RF_feature_importance_differences.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/plot_RF_feature_importance_differences.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/print_feature_selction_results.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/print_feature_selction_results.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import os
 import _pickle as pickle
 import math
 from scipy.stats import binom
 from datetime import datetime
-from my_easy_logger import my_logger
+from .my_easy_logger import my_logger
 
 
 filename = os.path.split(__file__)[1]
 
 
 def boruta_result_interpret(n_trial, rank_value_list, probability=0.5):
     # pmf = [binom.pmf(x, n_trial, probability) for x in range(n_trial + 1)]
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/reading_txt_files.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/reading_txt_files.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/sample_save_fldr_datasets.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/sample_save_fldr_datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 # Last update: -08-2021
 
 import os
 import _pickle as pickle
 import gc
-from datetime import datetime
-
 import pandas as pd
-
-from my_easy_logger import my_logger, logger_cleaner
-from config_template import NN
-from pickle_fldr_2_feather_fldr import get_df_dtypes
+from .my_easy_logger import my_logger, logger_cleaner
+from .config_template import NN
+from .pickle_fldr_2_feather_fldr import get_df_dtypes
 
 script_name = os.path.split(__file__)[1][:-3]
 
 
 # ---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*
 @logger_cleaner
 def sample_save_fldrs(_src_fldr, _dst_fldr, sample_number, *args, **kwargs):
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/weighted_average_alternate_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/weighted_average_alternate_wasserstein.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 to go without weights
 """
 
 
 import os
 import pickle
-from lib_plotters import draw_bar_chart
+from .lib_plotters import draw_bar_chart
 import pandas as pd
 
 
 # src_fldr = '/home/nids1/Desktop/ZSL_visualizations/NetFlow/'
 # save_fldr = '/home/nids1/Desktop/ZSL_visualizations/alternate_feature_wasserstein/'
 src_fldr = '/home/nids1/Desktop/ZSL_visualizations/original_ds/src/'
 save_fldr = '/home/nids1/Desktop/ZSL_visualizations/original_ds'
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/weighted_average_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/weighted_average_wasserstein.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import numpy as np
 import _pickle as pickle
-from intra_dataset_feature_wasserstein import plot_wasserstein_table
-from lib_plotters import draw_bar_chart
-from my_easy_logger import my_logger
+from .intra_dataset_feature_wasserstein import plot_wasserstein_table
+from .lib_plotters import draw_bar_chart
+from .my_easy_logger import my_logger
 
 script_name = os.path.split(__file__)[1]
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3-py3-none-any.whl` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3.tar.gz` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.3.tar.gz`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4-py3-none-any.whl` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4.tar.gz` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.4.tar.gz`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5-py3-none-any.whl` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1-py3-none-any.whl` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1.tar.gz` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.1.tar.gz`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.tar.gz` & `libs_n_utils_package_uq_2022-0.0.5.5/src/libs_n_utils_package_uq_2022/dist/libs_n_utils_package_uq_2022-0.0.5.tar.gz`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/LICENSE` & `libs_n_utils_package_uq_2022-0.0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/pyproject.toml` & `libs_n_utils_package_uq_2022-0.0.5.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "libs_n_utils_package_uq_2022"
-version = "0.0.5.4"
+version = "0.0.5.5"
 authors = [
   { name="siamak layeghy", email="siamak.layeghy@uq.net.au" },
 ]
-description = "A small library of utilities"
+description = "A small library of utilities, version 0.0.5.5 import issue is fixed."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `libs_n_utils_package_uq_2022-0.0.5.4/PKG-INFO` & `libs_n_utils_package_uq_2022-0.0.5.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: libs_n_utils_package_uq_2022
-Version: 0.0.5.4
-Summary: A small library of utilities
+Version: 0.0.5.5
+Summary: A small library of utilities, version 0.0.5.5 import issue is fixed.
 Project-URL: Homepage, https://github.com/layeghy/libs_n_utils
 Project-URL: Bug Tracker, https://github.com/layeghy/libs_n_utils/issues
 Author-email: siamak layeghy <siamak.layeghy@uq.net.au>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

