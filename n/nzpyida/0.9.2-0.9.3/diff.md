# Comparing `tmp/nzpyida-0.9.2.tar.gz` & `tmp/nzpyida-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nzpyida-0.9.2.tar", last modified: Fri Jul 14 14:36:08 2023, max compression
+gzip compressed data, was "nzpyida-0.9.3.tar", last modified: Fri Jul 21 14:43:24 2023, max compression
```

## Comparing `nzpyida-0.9.2.tar` & `nzpyida-0.9.3.tar`

### file list

```diff
@@ -1,161 +1,163 @@
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.864126 nzpyida-0.9.2/
--rw-r--r--   0 mpl        (501) staff       (20)       74 2023-05-16 06:22:43.000000 nzpyida-0.9.2/.gitignore
--rw-r--r--   0 mpl        (501) staff       (20)     1562 2023-05-10 12:49:36.000000 nzpyida-0.9.2/LICENSE.txt
--rw-r--r--   0 mpl        (501) staff       (20)      262 2023-05-16 07:31:06.000000 nzpyida-0.9.2/MANIFEST.in
--rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-07-14 14:36:08.864207 nzpyida-0.9.2/PKG-INFO
--rw-r--r--   0 mpl        (501) staff       (20)     3748 2023-05-25 14:48:09.000000 nzpyida-0.9.2/README.md
--rw-r--r--   0 mpl        (501) staff       (20)        5 2023-07-14 11:52:20.000000 nzpyida-0.9.2/VERSION
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.825519 nzpyida-0.9.2/docs/
--rw-r--r--   0 mpl        (501) staff       (20)     6148 2023-05-10 08:22:56.000000 nzpyida-0.9.2/docs/.DS_Store
--rw-r--r--   0 mpl        (501) staff       (20)     7669 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/Makefile
--rw-r--r--   0 mpl        (501) staff       (20)     6997 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/make.bat
--rw-r--r--   0 mpl        (501) staff       (20)       41 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/requirements.txt
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.829037 nzpyida-0.9.2/docs/source/
--rw-r--r--   0 mpl        (501) staff       (20)      110 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/analytics.rst
--rw-r--r--   0 mpl        (501) staff       (20)     3433 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/base.rst
--rw-r--r--   0 mpl        (501) staff       (20)    12029 2023-07-14 11:58:59.000000 nzpyida-0.9.2/docs/source/conf.py
--rw-r--r--   0 mpl        (501) staff       (20)      419 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/exploration.rst
--rw-r--r--   0 mpl        (501) staff       (20)     6407 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/frame.rst
--rw-r--r--   0 mpl        (501) staff       (20)     2499 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/geoFrame.rst
--rw-r--r--   0 mpl        (501) staff       (20)     5123 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/geoSeries.rst
--rw-r--r--   0 mpl        (501) staff       (20)     4191 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/geospatial.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1740 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/ibm.png
--rw-r--r--   0 mpl        (501) staff       (20)     4041 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/index.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1557 2023-07-12 13:55:25.000000 nzpyida-0.9.2/docs/source/install.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1150 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/kc.ico
--rw-r--r--   0 mpl        (501) staff       (20)     2024 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/legal.rst
--rw-r--r--   0 mpl        (501) staff       (20)     2834 2023-06-20 14:25:25.000000 nzpyida-0.9.2/docs/source/predictive.rst
--rw-r--r--   0 mpl        (501) staff       (20)    23914 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/start.rst
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/transform.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1444 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/utils.rst
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.837618 nzpyida-0.9.2/nzpyida/
--rw-r--r--   0 mpl        (501) staff       (20)      901 2023-05-16 09:30:30.000000 nzpyida-0.9.2/nzpyida/__init__.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.841570 nzpyida-0.9.2/nzpyida/ae/
--rw-r--r--   0 mpl        (501) staff       (20)      893 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     3496 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/apply.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.843278 nzpyida-0.9.2/nzpyida/ae/client code examples/
--rw-r--r--   0 mpl        (501) staff       (20)     4080 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/client code examples/customer_churn_prediction_nps.py
--rw-r--r--   0 mpl        (501) staff       (20)     4929 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py
--rw-r--r--   0 mpl        (501) staff       (20)    10386 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py
--rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/client code examples/house_pricing.py
--rw-r--r--   0 mpl        (501) staff       (20)      231 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/client code examples/install_package_test.py
--rw-r--r--   0 mpl        (501) staff       (20)     4615 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/client code examples/stock_prediction_nps side.py
--rw-r--r--   0 mpl        (501) staff       (20)    12151 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py
--rw-r--r--   0 mpl        (501) staff       (20)     5983 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/groupedapply.py
--rw-r--r--   0 mpl        (501) staff       (20)     1645 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/install.py
--rw-r--r--   0 mpl        (501) staff       (20)     4399 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/result_builder.py
--rw-r--r--   0 mpl        (501) staff       (20)     7082 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/shaper.py
--rw-r--r--   0 mpl        (501) staff       (20)     3785 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/tapply.py
--rw-r--r--   0 mpl        (501) staff       (20)     6543 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/tapply_class.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.843481 nzpyida-0.9.2/nzpyida/ae/tests/
--rw-r--r--   0 mpl        (501) staff       (20)    22335 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/tests/test_pyida.py
--rw-r--r--   0 mpl        (501) staff       (20)     6392 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/aggregation.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.845094 nzpyida-0.9.2/nzpyida/analytics/
--rw-r--r--   0 mpl        (501) staff       (20)     2027 2023-06-20 14:25:25.000000 nzpyida-0.9.2/nzpyida/analytics/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     2320 2023-05-17 10:27:59.000000 nzpyida-0.9.2/nzpyida/analytics/auto_delete_context.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.845848 nzpyida-0.9.2/nzpyida/analytics/exploration/
--rw-r--r--   0 mpl        (501) staff       (20)      401 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/exploration/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     9102 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/exploration/distribution.py
--rw-r--r--   0 mpl        (501) staff       (20)    32901 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/exploration/relation_identification.py
--rw-r--r--   0 mpl        (501) staff       (20)     8695 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/model_manager.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.849957 nzpyida-0.9.2/nzpyida/analytics/predictive/
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)    13034 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)    29001 2023-06-20 14:25:25.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/bayesian_networks.py
--rw-r--r--   0 mpl        (501) staff       (20)    11482 2023-05-25 14:48:09.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/bisecting_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     8440 2023-07-14 08:41:28.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/classification.py
--rw-r--r--   0 mpl        (501) staff       (20)    10009 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/decision_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)     9450 2023-05-25 14:48:09.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/glm.py
--rw-r--r--   0 mpl        (501) staff       (20)    10920 2023-05-25 14:48:09.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     9603 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/knn.py
--rw-r--r--   0 mpl        (501) staff       (20)     5588 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/linear_regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     6019 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)     6258 2023-07-13 09:52:03.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/predictive_modeling.py
--rw-r--r--   0 mpl        (501) staff       (20)     5721 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     8356 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/regression_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)     8852 2023-05-25 14:48:09.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/timeseries.py
--rw-r--r--   0 mpl        (501) staff       (20)    12701 2023-05-25 14:48:09.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/two_step_clustering.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.854990 nzpyida-0.9.2/nzpyida/analytics/tests/
--rw-r--r--   0 mpl        (501) staff       (20)     3588 2023-07-06 15:07:05.000000 nzpyida-0.9.2/nzpyida/analytics/tests/conftest.py
--rw-r--r--   0 mpl        (501) staff       (20)     3439 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)     3666 2023-07-06 15:02:50.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_auto_delete_context.py
--rw-r--r--   0 mpl        (501) staff       (20)     6678 2023-06-20 14:25:25.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_bayesian_networks.py
--rw-r--r--   0 mpl        (501) staff       (20)     2397 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_bisecting_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     2067 2023-05-29 14:08:02.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_cross_validation.py
--rw-r--r--   0 mpl        (501) staff       (20)     2759 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_decision_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)     2482 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_discretization.py
--rw-r--r--   0 mpl        (501) staff       (20)     4035 2023-05-25 14:48:09.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_glm.py
--rw-r--r--   0 mpl        (501) staff       (20)     2265 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     2671 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_knn.py
--rw-r--r--   0 mpl        (501) staff       (20)     2504 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_linear_regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     3289 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_model_manager.py
--rw-r--r--   0 mpl        (501) staff       (20)     2695 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)     3041 2023-05-29 14:08:02.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_preparation.py
--rw-r--r--   0 mpl        (501) staff       (20)     2475 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_regression_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)    20233 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_relation_identification.py
--rw-r--r--   0 mpl        (501) staff       (20)     2195 2023-05-16 09:58:38.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_timeseries.py
--rw-r--r--   0 mpl        (501) staff       (20)     2419 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_two_step_clustering.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.855778 nzpyida-0.9.2/nzpyida/analytics/transform/
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/transform/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)    10667 2023-07-14 08:34:35.000000 nzpyida-0.9.2/nzpyida/analytics/transform/discretization.py
--rw-r--r--   0 mpl        (501) staff       (20)    10990 2023-07-12 13:55:25.000000 nzpyida-0.9.2/nzpyida/analytics/transform/preparation.py
--rw-r--r--   0 mpl        (501) staff       (20)     5176 2023-07-12 13:55:25.000000 nzpyida-0.9.2/nzpyida/analytics/utils.py
--rw-r--r--   0 mpl        (501) staff       (20)    93282 2023-05-26 14:10:56.000000 nzpyida-0.9.2/nzpyida/base.py
--rw-r--r--   0 mpl        (501) staff       (20)     2331 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/exceptions.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.857667 nzpyida-0.9.2/nzpyida/feature_selection/
--rw-r--r--   0 mpl        (501) staff       (20)      877 2023-05-25 14:48:09.000000 nzpyida-0.9.2/nzpyida/feature_selection/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     4562 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/feature_selection/chisquared.py
--rw-r--r--   0 mpl        (501) staff       (20)     5089 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/feature_selection/entropy.py
--rw-r--r--   0 mpl        (501) staff       (20)     4228 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/feature_selection/gain_ratio.py
--rw-r--r--   0 mpl        (501) staff       (20)     5106 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/feature_selection/gini.py
--rw-r--r--   0 mpl        (501) staff       (20)     3350 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/feature_selection/info_gain.py
--rw-r--r--   0 mpl        (501) staff       (20)     3100 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/feature_selection/private.py
--rw-r--r--   0 mpl        (501) staff       (20)     5235 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/feature_selection/symmetric_uncertainty.py
--rw-r--r--   0 mpl        (501) staff       (20)     4437 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/feature_selection/tstats.py
--rw-r--r--   0 mpl        (501) staff       (20)     7710 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/filtering.py
--rw-r--r--   0 mpl        (501) staff       (20)    90288 2023-07-14 10:27:18.000000 nzpyida-0.9.2/nzpyida/frame.py
--rw-r--r--   0 mpl        (501) staff       (20)     4998 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/indexing.py
--rw-r--r--   0 mpl        (501) staff       (20)    18273 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/internals.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.859285 nzpyida-0.9.2/nzpyida/sampledata/
--rw-r--r--   0 mpl        (501) staff       (20)      736 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/sampledata/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     1071 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/sampledata/iris.py
--rw-r--r--   0 mpl        (501) staff       (20)     3858 2023-07-14 08:41:35.000000 nzpyida-0.9.2/nzpyida/sampledata/iris.txt
--rw-r--r--   0 mpl        (501) staff       (20)     1255 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/sampledata/swiss.py
--rw-r--r--   0 mpl        (501) staff       (20)     1757 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/sampledata/swiss.txt
--rw-r--r--   0 mpl        (501) staff       (20)     1386 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/sampledata/titanic.py
--rw-r--r--   0 mpl        (501) staff       (20)    67702 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/sampledata/titanic.txt
--rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-06-19 09:03:41.000000 nzpyida-0.9.2/nzpyida/series.py
--rw-r--r--   0 mpl        (501) staff       (20)    13343 2023-07-06 15:02:38.000000 nzpyida-0.9.2/nzpyida/sql.py
--rw-r--r--   0 mpl        (501) staff       (20)    38179 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/statistics.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.863959 nzpyida-0.9.2/nzpyida/tests/
--rw-r--r--   0 mpl        (501) staff       (20)    13403 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/conftest.py
--rw-r--r--   0 mpl        (501) staff       (20)     3202 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_aggregation.py
--rw-r--r--   0 mpl        (501) staff       (20)     1368 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)     8668 2023-05-16 09:30:12.000000 nzpyida-0.9.2/nzpyida/tests/test_base.py
--rw-r--r--   0 mpl        (501) staff       (20)     6371 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_base_connexion.py
--rw-r--r--   0 mpl        (501) staff       (20)     6705 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_base_private.py
--rw-r--r--   0 mpl        (501) staff       (20)     9686 2023-05-16 09:30:06.000000 nzpyida-0.9.2/nzpyida/tests/test_base_table_manipulation.py
--rw-r--r--   0 mpl        (501) staff       (20)    23494 2023-05-25 14:48:09.000000 nzpyida-0.9.2/nzpyida/tests/test_feature_selection.py
--rw-r--r--   0 mpl        (501) staff       (20)     3146 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_filtering.py
--rw-r--r--   0 mpl        (501) staff       (20)    15208 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_frame.py
--rw-r--r--   0 mpl        (501) staff       (20)     1384 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_frame_connexion.py
--rw-r--r--   0 mpl        (501) staff       (20)     2403 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_frame_private.py
--rw-r--r--   0 mpl        (501) staff       (20)    11243 2023-05-16 09:30:18.000000 nzpyida-0.9.2/nzpyida/tests/test_geoFrame.py
--rw-r--r--   0 mpl        (501) staff       (20)    11342 2023-05-16 09:30:23.000000 nzpyida-0.9.2/nzpyida/tests/test_geoSeries.py
--rw-r--r--   0 mpl        (501) staff       (20)     2730 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_indexing.py
--rw-r--r--   0 mpl        (501) staff       (20)      968 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_internals.py
--rw-r--r--   0 mpl        (501) staff       (20)     1333 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     1336 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)      850 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_series.py
--rw-r--r--   0 mpl        (501) staff       (20)     1429 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_sorting.py
--rw-r--r--   0 mpl        (501) staff       (20)     8359 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_statistics.py
--rw-r--r--   0 mpl        (501) staff       (20)      987 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_utils.py
--rw-r--r--   0 mpl        (501) staff       (20)    11065 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/utils.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.838754 nzpyida-0.9.2/nzpyida.egg-info/
--rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-07-14 14:36:08.000000 nzpyida-0.9.2/nzpyida.egg-info/PKG-INFO
--rw-r--r--   0 mpl        (501) staff       (20)     4883 2023-07-14 14:36:08.000000 nzpyida-0.9.2/nzpyida.egg-info/SOURCES.txt
--rw-r--r--   0 mpl        (501) staff       (20)        1 2023-07-14 14:36:08.000000 nzpyida-0.9.2/nzpyida.egg-info/dependency_links.txt
--rw-r--r--   0 mpl        (501) staff       (20)      164 2023-07-14 14:36:08.000000 nzpyida-0.9.2/nzpyida.egg-info/requires.txt
--rw-r--r--   0 mpl        (501) staff       (20)        8 2023-07-14 14:36:08.000000 nzpyida-0.9.2/nzpyida.egg-info/top_level.txt
--rw-r--r--   0 mpl        (501) staff       (20)      213 2023-07-14 14:36:08.864483 nzpyida-0.9.2/setup.cfg
--rw-r--r--   0 mpl        (501) staff       (20)     3300 2023-07-14 11:55:18.000000 nzpyida-0.9.2/setup.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.209856 nzpyida-0.9.3/
+-rw-r--r--   0 mpl        (501) staff       (20)       74 2023-05-16 06:22:43.000000 nzpyida-0.9.3/.gitignore
+-rw-r--r--   0 mpl        (501) staff       (20)     1562 2023-05-10 12:49:36.000000 nzpyida-0.9.3/LICENSE.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      221 2023-07-21 14:42:45.000000 nzpyida-0.9.3/MANIFEST.in
+-rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-07-21 14:43:24.209985 nzpyida-0.9.3/PKG-INFO
+-rw-r--r--   0 mpl        (501) staff       (20)     3748 2023-05-25 14:48:09.000000 nzpyida-0.9.3/README.md
+-rw-r--r--   0 mpl        (501) staff       (20)        6 2023-07-21 14:42:45.000000 nzpyida-0.9.3/VERSION
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.186019 nzpyida-0.9.3/docs/
+-rw-r--r--   0 mpl        (501) staff       (20)     6148 2023-05-10 08:22:56.000000 nzpyida-0.9.3/docs/.DS_Store
+-rw-r--r--   0 mpl        (501) staff       (20)     7669 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/Makefile
+-rw-r--r--   0 mpl        (501) staff       (20)     6997 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/make.bat
+-rw-r--r--   0 mpl        (501) staff       (20)       41 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/requirements.txt
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.188608 nzpyida-0.9.3/docs/source/
+-rw-r--r--   0 mpl        (501) staff       (20)      110 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/source/analytics.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     3433 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/source/base.rst
+-rw-r--r--   0 mpl        (501) staff       (20)    12029 2023-07-21 10:38:04.000000 nzpyida-0.9.3/docs/source/conf.py
+-rw-r--r--   0 mpl        (501) staff       (20)      419 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/source/exploration.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     6407 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/source/frame.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     2500 2023-07-21 14:42:45.000000 nzpyida-0.9.3/docs/source/geo_frame.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     3560 2023-07-21 14:42:45.000000 nzpyida-0.9.3/docs/source/geo_series.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     3638 2023-07-21 14:42:45.000000 nzpyida-0.9.3/docs/source/geospatial.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1740 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/source/ibm.png
+-rw-r--r--   0 mpl        (501) staff       (20)     4059 2023-07-21 14:42:45.000000 nzpyida-0.9.3/docs/source/index.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1557 2023-07-21 10:38:04.000000 nzpyida-0.9.3/docs/source/install.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1150 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/source/kc.ico
+-rw-r--r--   0 mpl        (501) staff       (20)     2024 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/source/legal.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     2834 2023-06-20 14:25:25.000000 nzpyida-0.9.3/docs/source/predictive.rst
+-rw-r--r--   0 mpl        (501) staff       (20)    23915 2023-07-21 14:42:45.000000 nzpyida-0.9.3/docs/source/start.rst
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/source/transform.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1444 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/source/utils.rst
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.191058 nzpyida-0.9.3/nzpyida/
+-rw-r--r--   0 mpl        (501) staff       (20)     1016 2023-07-21 14:42:45.000000 nzpyida-0.9.3/nzpyida/__init__.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.193287 nzpyida-0.9.3/nzpyida/ae/
+-rw-r--r--   0 mpl        (501) staff       (20)      893 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3496 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/apply.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.194949 nzpyida-0.9.3/nzpyida/ae/client code examples/
+-rw-r--r--   0 mpl        (501) staff       (20)     4080 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/client code examples/customer_churn_prediction_nps.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4929 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10386 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/client code examples/house_pricing.py
+-rw-r--r--   0 mpl        (501) staff       (20)      231 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/client code examples/install_package_test.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4615 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/client code examples/stock_prediction_nps side.py
+-rw-r--r--   0 mpl        (501) staff       (20)    12151 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5983 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/groupedapply.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1645 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/install.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4399 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/result_builder.py
+-rw-r--r--   0 mpl        (501) staff       (20)     7082 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/shaper.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3785 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/tapply.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6543 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/tapply_class.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.195141 nzpyida-0.9.3/nzpyida/ae/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)    22335 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/tests/test_pyida.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6392 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/aggregation.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.195853 nzpyida-0.9.3/nzpyida/analytics/
+-rw-r--r--   0 mpl        (501) staff       (20)     2027 2023-06-20 14:25:25.000000 nzpyida-0.9.3/nzpyida/analytics/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2320 2023-05-17 10:27:59.000000 nzpyida-0.9.3/nzpyida/analytics/auto_delete_context.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.196346 nzpyida-0.9.3/nzpyida/analytics/exploration/
+-rw-r--r--   0 mpl        (501) staff       (20)      401 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/analytics/exploration/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9129 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/exploration/distribution.py
+-rw-r--r--   0 mpl        (501) staff       (20)    33218 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/exploration/relation_identification.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8695 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/analytics/model_manager.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.198935 nzpyida-0.9.3/nzpyida/analytics/predictive/
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)    13090 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)    29037 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/bayesian_networks.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11574 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/bisecting_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8585 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/classification.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10059 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/decision_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9562 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/glm.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10976 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9665 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/knn.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5637 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/linear_regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6069 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6285 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/predictive_modeling.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5767 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8390 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/regression_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8909 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/timeseries.py
+-rw-r--r--   0 mpl        (501) staff       (20)    12793 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/two_step_clustering.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.201843 nzpyida-0.9.3/nzpyida/analytics/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)     3588 2023-07-06 15:07:05.000000 nzpyida-0.9.3/nzpyida/analytics/tests/conftest.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3621 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3666 2023-07-06 15:02:50.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_auto_delete_context.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6796 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_bayesian_networks.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2435 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_bisecting_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2086 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_cross_validation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2835 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_decision_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2683 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_discretization.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4054 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_glm.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2303 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2747 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_knn.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2542 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_linear_regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3503 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_model_manager.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2771 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3067 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_preparation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2494 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_regression_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)    22367 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_relation_identification.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2195 2023-07-20 08:34:06.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_timeseries.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2457 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_two_step_clustering.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.202305 nzpyida-0.9.3/nzpyida/analytics/transform/
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/analytics/transform/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10647 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/transform/discretization.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11017 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/transform/preparation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5942 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/utils.py
+-rw-r--r--   0 mpl        (501) staff       (20)    93635 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/base.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2331 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/exceptions.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.204038 nzpyida-0.9.3/nzpyida/feature_selection/
+-rw-r--r--   0 mpl        (501) staff       (20)      877 2023-05-25 14:48:09.000000 nzpyida-0.9.3/nzpyida/feature_selection/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4562 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/feature_selection/chisquared.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5089 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/feature_selection/entropy.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4228 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/feature_selection/gain_ratio.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5106 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/feature_selection/gini.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3350 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/feature_selection/info_gain.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3100 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/feature_selection/private.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5235 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/feature_selection/symmetric_uncertainty.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4437 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/feature_selection/tstats.py
+-rw-r--r--   0 mpl        (501) staff       (20)     7710 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/filtering.py
+-rw-r--r--   0 mpl        (501) staff       (20)    90409 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/frame.py
+-rw-r--r--   0 mpl        (501) staff       (20)    37116 2023-07-21 14:42:45.000000 nzpyida-0.9.3/nzpyida/geo_frame.py
+-rw-r--r--   0 mpl        (501) staff       (20)    66784 2023-07-21 14:42:45.000000 nzpyida-0.9.3/nzpyida/geo_series.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4998 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/indexing.py
+-rw-r--r--   0 mpl        (501) staff       (20)    18287 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/internals.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.205429 nzpyida-0.9.3/nzpyida/sampledata/
+-rw-r--r--   0 mpl        (501) staff       (20)      736 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/sampledata/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1071 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/sampledata/iris.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3858 2023-07-14 08:41:35.000000 nzpyida-0.9.3/nzpyida/sampledata/iris.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     1255 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/sampledata/swiss.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1757 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/sampledata/swiss.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     1386 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/sampledata/titanic.py
+-rw-r--r--   0 mpl        (501) staff       (20)    67702 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/sampledata/titanic.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-06-19 09:03:41.000000 nzpyida-0.9.3/nzpyida/series.py
+-rw-r--r--   0 mpl        (501) staff       (20)    13343 2023-07-06 15:02:38.000000 nzpyida-0.9.3/nzpyida/sql.py
+-rw-r--r--   0 mpl        (501) staff       (20)    38179 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/statistics.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.209682 nzpyida-0.9.3/nzpyida/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)    13644 2023-07-21 14:42:45.000000 nzpyida-0.9.3/nzpyida/tests/conftest.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3202 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_aggregation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1368 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8685 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/tests/test_base.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6371 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_base_connexion.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6758 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/tests/test_base_private.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9694 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/tests/test_base_table_manipulation.py
+-rw-r--r--   0 mpl        (501) staff       (20)    23494 2023-07-19 07:48:15.000000 nzpyida-0.9.3/nzpyida/tests/test_feature_selection.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3146 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_filtering.py
+-rw-r--r--   0 mpl        (501) staff       (20)    15148 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/tests/test_frame.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1384 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_frame_connexion.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2403 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_frame_private.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9173 2023-07-21 14:42:45.000000 nzpyida-0.9.3/nzpyida/tests/test_geo_frame.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8966 2023-07-21 14:42:45.000000 nzpyida-0.9.3/nzpyida/tests/test_geo_series.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2730 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_indexing.py
+-rw-r--r--   0 mpl        (501) staff       (20)      968 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_internals.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1333 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1336 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)      850 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_series.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1429 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_sorting.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8359 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_statistics.py
+-rw-r--r--   0 mpl        (501) staff       (20)      987 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_utils.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11210 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/utils.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.191914 nzpyida-0.9.3/nzpyida.egg-info/
+-rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-07-21 14:43:24.000000 nzpyida-0.9.3/nzpyida.egg-info/PKG-INFO
+-rw-r--r--   0 mpl        (501) staff       (20)     4930 2023-07-21 14:43:24.000000 nzpyida-0.9.3/nzpyida.egg-info/SOURCES.txt
+-rw-r--r--   0 mpl        (501) staff       (20)        1 2023-07-21 14:43:24.000000 nzpyida-0.9.3/nzpyida.egg-info/dependency_links.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      164 2023-07-21 14:43:24.000000 nzpyida-0.9.3/nzpyida.egg-info/requires.txt
+-rw-r--r--   0 mpl        (501) staff       (20)        8 2023-07-21 14:43:24.000000 nzpyida-0.9.3/nzpyida.egg-info/top_level.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      213 2023-07-21 14:43:24.210278 nzpyida-0.9.3/setup.cfg
+-rw-r--r--   0 mpl        (501) staff       (20)     3300 2023-07-21 10:38:04.000000 nzpyida-0.9.3/setup.py
```

### Comparing `nzpyida-0.9.2/LICENSE.txt` & `nzpyida-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/PKG-INFO` & `nzpyida-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nzpyida
-Version: 0.9.2
+Version: 0.9.3
 Summary: Supports Custom ML/Analytics Execution Inside Netezza
 Home-page: https://github.com/ibm/nzpyida
 Author: IBM Corp.
 Author-email: mlabenski@ibm.com,pawel.mroz1@ibm.com
 License: BSD
 Project-URL: Documentation, https://nzpyida.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/IBM/nzpyida
```

### Comparing `nzpyida-0.9.2/README.md` & `nzpyida-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/docs/.DS_Store` & `nzpyida-0.9.3/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/docs/Makefile` & `nzpyida-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/docs/make.bat` & `nzpyida-0.9.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/docs/source/base.rst` & `nzpyida-0.9.3/docs/source/base.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/docs/source/conf.py` & `nzpyida-0.9.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/docs/source/frame.rst` & `nzpyida-0.9.3/docs/source/frame.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/docs/source/geoFrame.rst` & `nzpyida-0.9.3/docs/source/geo_frame.rst`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 this commands will always act on the “geometry” attribute.
 
 The “geometry” attribute – no matter its name – can be accessed through the geometry attribute
 of an IdaGeoDataFrame.
 
 Open an IdaGeoDataFrame
 =======================
-.. currentmodule:: nzpyida.geoFrame
+.. currentmodule:: nzpyida.geo_frame
 
 .. autoclass:: IdaGeoDataFrame
 
    .. automethod:: __init__
 
 Set geometry
 ------------
```

### Comparing `nzpyida-0.9.2/docs/source/geospatial.rst` & `nzpyida-0.9.3/docs/source/geospatial.rst`

 * *Files 7% similar despite different names*

```diff
@@ -29,42 +29,38 @@
 The latest version of nzpyida is available on the `Python Package Index`__.
 
 __ https://pypi.python.org/pypi/nzpyida
 
 How the spatial functions work
 ------------------------------
 
-The nzpyida-spatial functions translate geopandas-like syntax into SQL and uses a middleware API (pypyodbc/JayDeBeApi)
-to send it to an ODBC or JDBC-connected database for execution.
+The nzpyida-spatial functions translate geopandas-like syntax into SQL and uses a middleware API (nzpy/pypyodbc/JayDeBeApi)
+to send it to an nzpy, ODBC or JDBC-connected database for execution.
 The results are fetched and formatted into the corresponding data structure, for example, a GeoPandas.GeoDataframe.
 
 The following scenario illustrates how nzpyida works.
 
-Assuming that all ODBC connection parameters are correctly set, issue the following statements to connect to a
-database (in this case, a Netezza database with the name BLUDB) via ODBC:
-
-    >>> from nzpyida import IdaDataBase, IdaGeoDataFrame
-    >>> idadb = IdaDataBase('BLUDB')
-
+Assuming that you've got connection to the databased established via IdaDataBase object named 'idadb'. 
 We can create an IDA geo data frame that points to a sample table:
 
     >>> idadf = IdaGeoDataFrame(idadb, 'SAMPLES.GEO_COUNTY')
 
 Note that to create an IDA geo data frame using the IdaDataFrame object, we need to specify our previously opened
 IdaDataBase object, because it holds the connection.
 
 Now let us compute the area of the counties in the GEO_COUNTY table:
 
     >>> idadf['area'] = idadf['SHAPE'].area()
-         	OBJECTID 	NAME 	        SHAPE 	                                                 area
-         	1 	        Wilbarger 	MULTIPOLYGON (((-99.4756582604 33.8340108094, ... 	0.247254
-         	2 	        Austin 	        MULTIPOLYGON (((-96.6219873342 30.0442882117, ... 	0.162639
-         	3 	        Logan 	        MULTIPOLYGON (((-99.4497297204 46.6316377481, ... 	0.306589
-         	4 	        La Plata 	MULTIPOLYGON (((-107.4817473750 37.0000108736,... 	0.447591
-         	5 	        Randolph 	MULTIPOLYGON (((-91.2589262966 36.2578866492, ... 	0.170844
+    >>> idadf[["NAME", 'area']]
+        NAME		area
+        Wilbarger	0.247254
+     	Austin		0.162639
+     	Logan		0.306589
+        La Plata	0.447591
+     	Randolph	0.170844
 
 The result of the area will be stored as a new column 'area' in the Ida geo data frame.
 
 
 
 In the background, nzpyida-spatial looks for geometry columns in the table and builds an SQL request that returns
 the area of each geometry.
@@ -72,9 +68,9 @@
 
     SELECT \*,ST_Area(SHAPE) AS "area" FROM SAMPLES.GEO_COUNTY;
 
 
 It's as simple as that!
 
 .. toctree::
-   geoFrame.rst
-   geoSeries.rst
+   geo_frame.rst
+   geo_series.rst
```

### Comparing `nzpyida-0.9.2/docs/source/ibm.png` & `nzpyida-0.9.3/docs/source/ibm.png`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/docs/source/index.rst` & `nzpyida-0.9.3/docs/source/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 .. toctree::
    :maxdepth: 2
 
    install.rst
    start.rst
    base.rst
    frame.rst
+   geospatial.rst
    analytics.rst
    utils.rst
    legal.rst
 
 Contributors
 ============
```

### Comparing `nzpyida-0.9.2/docs/source/install.rst` & `nzpyida-0.9.3/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/docs/source/kc.ico` & `nzpyida-0.9.3/docs/source/kc.ico`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/docs/source/legal.rst` & `nzpyida-0.9.3/docs/source/legal.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/docs/source/predictive.rst` & `nzpyida-0.9.3/docs/source/predictive.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/docs/source/start.rst` & `nzpyida-0.9.3/docs/source/start.rst`

 * *Files 0% similar despite different names*

```diff
@@ -56,16 +56,16 @@
 After you download and install the nzjdbc3.jar file, you must include its location in the value of the CLASSPATH environment variable.
 
 >>> export CLASSPATH=PATH TO nzjdbc3.jar:$CLASSPATH
 
 The connection is done using the JDBC URL string.
 
 >>> from nzpyida import IdaDataBase
->>> jdbc_dsn = jdbc:netezza://IP ADDRESS:PORT/DATABASE NAME"
->>> idadb = IdaDataBase(jdbc_dsn, uid="USRENAME", pwd="PASSWORD")
+>>> jdbc_dsn = "jdbc:netezza://IP ADDRESS:PORT/DATABASE NAME"
+>>> idadb = IdaDataBase(jdbc_dsn, uid="USERNAME", pwd="PASSWORD")
 
 Conventions
 -----------
 
 Users need to create an IdaDataBase instance before they can create an IdaDataFrame. By convention, users should use only one instance of IdaDataBase per database. However, they may use several instances of IdaDataFrame objects per table and connection.
 
 Most methods of the IdaDataBase interface may change the data in the database (they are destructive). However, all methods of the IdaDataFrame interface do not change the physical data in the database. As a result, they can be used without any risk for the data integrity.
```

### Comparing `nzpyida-0.9.2/docs/source/utils.rst` & `nzpyida-0.9.3/docs/source/utils.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/__init__.py` & `nzpyida-0.9.3/nzpyida/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,11 +14,15 @@
 from __future__ import division
 from __future__ import absolute_import
 from future import standard_library
 standard_library.install_aliases()
 from .base import IdaDataBase
 from .frame import IdaDataFrame
 from .series import IdaSeries
+from .geo_frame import IdaGeoDataFrame
+from .geo_series import IdaGeoSeries
+
 
 __all__ = ['sampledata', 'tests', 'aggregation', 
 		   'base', 'exceptions', 'filtering', 'frame', 'indexing', 
-		   'internals', 'series', 'sql', 'statistics', 'utils', 'analytics']
+		   'internals', 'series', 'sql', 'statistics', 'utils', 'analytics',
+           'geo_frame', 'geo_series']
```

### Comparing `nzpyida-0.9.2/nzpyida/ae/__init__.py` & `nzpyida-0.9.3/nzpyida/ae/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/ae/apply.py` & `nzpyida-0.9.3/nzpyida/ae/apply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/ae/client code examples/customer_churn_prediction_nps.py` & `nzpyida-0.9.3/nzpyida/ae/client code examples/customer_churn_prediction_nps.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py` & `nzpyida-0.9.3/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py` & `nzpyida-0.9.3/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/ae/client code examples/house_pricing.py` & `nzpyida-0.9.3/nzpyida/ae/client code examples/house_pricing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/ae/client code examples/stock_prediction_nps side.py` & `nzpyida-0.9.3/nzpyida/ae/client code examples/stock_prediction_nps side.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py` & `nzpyida-0.9.3/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/ae/groupedapply.py` & `nzpyida-0.9.3/nzpyida/ae/groupedapply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/ae/install.py` & `nzpyida-0.9.3/nzpyida/ae/install.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/ae/result_builder.py` & `nzpyida-0.9.3/nzpyida/ae/result_builder.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/ae/shaper.py` & `nzpyida-0.9.3/nzpyida/ae/shaper.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/ae/tapply.py` & `nzpyida-0.9.3/nzpyida/ae/tapply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/ae/tapply_class.py` & `nzpyida-0.9.3/nzpyida/ae/tapply_class.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/ae/tests/test_pyida.py` & `nzpyida-0.9.3/nzpyida/ae/tests/test_pyida.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/aggregation.py` & `nzpyida-0.9.3/nzpyida/aggregation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/analytics/__init__.py` & `nzpyida-0.9.3/nzpyida/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/analytics/auto_delete_context.py` & `nzpyida-0.9.3/nzpyida/analytics/auto_delete_context.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/analytics/exploration/distribution.py` & `nzpyida-0.9.3/nzpyida/analytics/exploration/distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 This module consists of algorithms used to describe the empirical distribution
 of single attributes or the joint distribution of multiple—usually two—attributes.
 """
 
 from typing import List
 from nzpyida.frame import IdaDataFrame
-from nzpyida.analytics.utils import call_proc_df_in_out
+from nzpyida.analytics.utils import call_proc_df_in_out, q
 
 
 def moments(in_df: IdaDataFrame, in_column: str, by_column: str=None,
     out_table: str=None) -> IdaDataFrame:
     """
     Moments are quantities used to describe certain aspects of continuous attribute
     distributions. Of particular interest are the central moments or moments around
@@ -47,16 +47,16 @@
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
 
     params = {
-        'incolumn': in_column,
-        'by': by_column
+        'incolumn': q(in_column),
+        'by': q(by_column)
     }
     return call_proc_df_in_out(proc='MOMENTS', in_df=in_df, params=params, out_table=out_table)[0]
 
 def quantile(in_df: IdaDataFrame, in_column: str, quantiles: List[int],
     out_table: str=None) -> IdaDataFrame:
     """
     Quantiles constitute a convenient and intuitive description of continuous attribute
@@ -85,15 +85,15 @@
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
 
     params = {
-        'incolumn': in_column,
+        'incolumn': q(in_column),
         'quantiles': quantiles
     }
     return call_proc_df_in_out(proc='QUANTILE', in_df=in_df, params=params, out_table=out_table)[0]
 
 def outliers(in_df: IdaDataFrame, in_column: str, multiplier: float=1.5,
     out_table: str=None) -> IdaDataFrame:
     """
@@ -120,15 +120,15 @@
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
 
     params = {
-        'incolumn': in_column,
+        'incolumn': q(in_column),
         'multiplier': multiplier
     }
     return call_proc_df_in_out(proc='OUTLIERS', in_df=in_df, params=params, out_table=out_table)[0]
 
 def unitable(in_df: IdaDataFrame, in_column: str, out_table: str=None) -> IdaDataFrame:
     """
     A univariate frequency table describes the distribution of a discrete attribute
@@ -150,15 +150,15 @@
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
 
     params = {
-        'incolumn': in_column
+        'incolumn': q(in_column)
     }
     return call_proc_df_in_out(proc='UNITABLE', in_df=in_df, params=params, out_table=out_table)[0]
 
 def bitable(in_df: IdaDataFrame, in_column: List[str], freq: bool=False, cum: bool=False,
     out_table: str=None) -> IdaDataFrame:
     """
     A bivariate frequency table describes the joint probability distribution of two
@@ -190,15 +190,15 @@
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
 
     params = {
-        'incolumn': in_column,
+        'incolumn': q(in_column),
         'freq': freq,
         'cum': cum
     }
     return call_proc_df_in_out(proc='BITABLE', in_df=in_df, params=params, out_table=out_table)[0]
 
 def histogram(in_df: IdaDataFrame, in_column: str, nbreaks: int=None, right: bool=True,
     btable: str=None, bcolumn: str=None, density: bool=False, midpoints: bool=False,
@@ -259,18 +259,18 @@
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
 
     params = {
-        'incolumn': in_column,
+        'incolumn': q(in_column),
         'nbreaks': nbreaks,
         'right': right,
         'btable': btable,
-        'bcolumn': bcolumn,
+        'bcolumn': q(bcolumn),
         'density': density,
         'midpoints': midpoints,
         'freq': freq,
         'cum': cum
     }
     return call_proc_df_in_out(proc='HIST', in_df=in_df, params=params, out_table=out_table)[0]
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/exploration/relation_identification.py` & `nzpyida-0.9.3/nzpyida/analytics/exploration/relation_identification.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 """
 This module consists of algorithms used to detect and quantify relationships between attributes.
 """
 
 from nzpyida.analytics.utils import call_proc_df_in_out, make_temp_table_name, out_str_to_df
 from nzpyida.frame import IdaDataFrame
 from typing import List
+from nzpyida.analytics.utils import q
 import pandas as pd
 
 
 def corr(in_df: IdaDataFrame, in_column: List[str], by_column: str=None, out_table: str=None):
     """
     This stored procedure calculates the correlation between two numeric input columns, 
     either in the whole input table or within the groups defined in the column specified by parameter <by>. 
@@ -45,22 +46,22 @@
 
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
     params = {
-        'incolumn': in_column,
-        'by': by_column
+        'incolumn': q(in_column),
+        'by': q(by_column)
     }
     out_df = call_proc_df_in_out(proc="CORR", in_df=in_df, params=params, out_table=out_table)[0]
     temp_table = make_temp_table_name()
     query = f"""create table {temp_table} as
             select case when CORRELATION is null then 0 else CORRELATION
-            end as correlation {', ' + by_column if by_column else ''}
+            end as correlation {', "' + by_column + '"' if by_column else ''}
             from {out_table};
             drop table {out_table};
             alter table {temp_table} rename to {out_table};
             """
     in_df._idadb.ida_query(query)
     return out_df
 
@@ -91,16 +92,16 @@
 
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
     params = {
-        'incolumn': in_column,
-        'by': by_column
+        'incolumn': q(in_column),
+        'by': q(by_column)
     }
     return call_proc_df_in_out(proc="COV", in_df=in_df, params=params, out_table=out_table)[0]
 
 
 def covariance_matrix(in_df: IdaDataFrame, in_column: List[str], out_table: str=None, by_column: str=None):
     """
     This function calculates the matrix of covariances between 
@@ -129,16 +130,16 @@
 
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
     params = {
-        'incolumn': in_column,
-        'by': by_column
+        'incolumn': q(in_column),
+        'by': q(by_column)
     }
     return call_proc_df_in_out(proc="COVARIANCEMATRIX", in_df=in_df, params=params, out_table=out_table)[0]
 
 
 def spearman_corr(in_df: IdaDataFrame, in_column: List[str], by_column: str=None, out_table: str=None):
     """
     This function calculates the Spearman rank correlation 
@@ -169,22 +170,22 @@
 
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
     params = {
-        'incolumn': in_column,
-        'by': by_column
+        'incolumn': q(in_column),
+        'by': q(by_column)
     }
     temp_table = make_temp_table_name()
     if by_column:
         out_df =  call_proc_df_in_out(proc="SPEARMAN_CORR", in_df=in_df, params=params, out_table=out_table)[0]
         query = f"""create table {temp_table} as
-            select {by_column + ', '} case when RHO is null then 0 else RHO
+            select {'"' + by_column + '", '} case when RHO is null then 0 else RHO
             end as RHO, N
             from {out_table};
             drop table {out_table};
             alter table {temp_table} rename to {out_table};
             """
     else:
         output = call_proc_df_in_out(proc="SPEARMAN_CORR", in_df=in_df, params=params, out_table=out_table)[1]
@@ -225,16 +226,16 @@
 
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
     params = {
-        'incolumn': in_column,
-        'by': by_column
+        'incolumn': q(in_column),
+        'by': q(by_column)
     }
     return call_proc_df_in_out(proc="MUTUALINFO", in_df=in_df, params=params, out_table=out_table)[0]
 
 
 def chisq(in_df: IdaDataFrame, in_column: List[str], out_table: str=None, by_column: str=None):
     """
     This function calculates the Chi-square value between two input columns, either 
@@ -265,16 +266,16 @@
 
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
     params = {
-        'incolumn': in_column,
-        'by': by_column
+        'incolumn': q(in_column),
+        'by': q(by_column)
     }
     return call_proc_df_in_out(proc="CHISQ_TEST", in_df=in_df, params=params, out_table=out_table)[0]
 
 
 def t_me_test(in_df: IdaDataFrame, in_column: str, mean_value: float, by_column: str=None, out_table: str=None):
     """
     This function calculates the t-Student statistics of an input column with the expected mean, 
@@ -304,16 +305,16 @@
 
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
     params = {
-        'incolumn': in_column,
-        'by': by_column,
+        'incolumn': q(in_column),
+        'by': q(by_column),
         'mean': mean_value
     }
     return call_proc_df_in_out(proc="T_ME_TEST", in_df=in_df, params=params, out_table=out_table)[0]
 
 
 def t_umd_test(in_df: IdaDataFrame, in_column: str, class_column: str, out_table: str=None, by_column: str=None):
     """
@@ -345,17 +346,17 @@
 
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
     params = {
-        'incolumn': in_column,
-        'by': by_column,
-        'class': class_column
+        'incolumn': q(in_column),
+        'by': q(by_column),
+        'class': q(class_column)
     }
     return call_proc_df_in_out(proc="T_UMD_TEST", in_df=in_df, params=params, out_table=out_table)[0]
 
 def t_pmd_test(in_df: IdaDataFrame, in_column: List[str], expected_diff: float, out_table: str=None, by_column: str=None):
     """
     This function calculates the t-Student statistics of two paired columns, either in the whole 
     input table or within the groups defined in the column specified by parameter <by>. 
@@ -382,16 +383,16 @@
 
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
     params = {
-        'incolumn': in_column,
-        'by': by_column,
+        'incolumn': q(in_column),
+        'by': q(by_column),
         'expdiff': expected_diff
     }
     return call_proc_df_in_out(proc="T_PMD_TEST", in_df=in_df, params=params, out_table=out_table)[0]
 
 
 def t_ls_test(in_df: IdaDataFrame, in_column: List[str], slope: float, by_column: str=None, out_table: str=None):
     """
@@ -424,16 +425,16 @@
 
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
     params = {
-        'incolumn': in_column,
-        'by': by_column,
+        'incolumn': q(in_column),
+        'by': q(by_column),
         'slope': slope
     }
     return call_proc_df_in_out(proc="T_LS_TEST", in_df=in_df, params=params, out_table=out_table)[0]
 
 #error in documentation
 def mww_test(in_df: IdaDataFrame, in_column: str, class_column: str, by_column: str=None, out_table: str=None):
     """
@@ -463,17 +464,17 @@
 
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
     params = {
-        'incolumn': in_column,
-        'by': by_column,
-        'class': class_column
+        'incolumn': q(in_column),
+        'by': q(by_column),
+        'class': q(class_column)
     }
     if by_column:
         return call_proc_df_in_out(proc="MWW_TEST", in_df=in_df, params=params, out_table=out_table)[0]
     else:
         output_string = call_proc_df_in_out(proc="MWW_TEST", in_df=in_df, params=params, out_table=out_table)[1][0]
         return in_df._idadb.as_idadataframe(out_str_to_df(str(output_string)), tablename=out_table)
 
@@ -502,16 +503,16 @@
 
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
     params = {
-        'incolumn': in_column,
-        'by': by_column
+        'incolumn': q(in_column),
+        'by': q(by_column)
     }
     if by_column:
         return call_proc_df_in_out(proc="WILCOXON_TEST", in_df=in_df, params=params, out_table=out_table)[0]
     else:
         output_string = call_proc_df_in_out(proc="WILCOXON_TEST", in_df=in_df, params=params, out_table=out_table)[1][0]
         return in_df._idadb.as_idadataframe(out_str_to_df(str(output_string)), tablename=out_table)
 
@@ -541,21 +542,21 @@
 
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
     params = {
-        'incolumn': in_column,
-        'by': by_column
+        'incolumn': q(in_column),
+        'by': q(by_column)
     }
     return call_proc_df_in_out(proc="CANONICAL_CORR", in_df=in_df, params=params, out_table=out_table)[0]
 
 
-def anova_crd_test(in_df: IdaDataFrame, in_column: List[str], treatment: str, by_column: str=None, out_table: str=None):
+def anova_crd_test(in_df: IdaDataFrame, in_column: List[str], treatment_column: str, by_column: str=None, out_table: str=None):
     """
     This function analyzes the variance of one or several observations for different treatments. 
     It assumes that the input table contains one or several columns with numerical (double) 
     observation results of an experiment concerning treatments indicated by the treatment parameter.
 
     The One-way ANOVA considers independent samples (the treatments) while the Completely Randomized Design 
     considers equally sized "samples". The implementation covers both cases. For more information, 
@@ -565,52 +566,52 @@
     ----------
     in_df : IdaDataFrame
         the input data frame
 
     in_column : List[str]
         the input table observation columns, separated by a semi-colon (;) 
     
-    treatment : str
+    treatment_column : str
         the input table column identifying a unique treatment
 
     by_column : str, optional
         the input table column which uniquely identifies a group on which to perform ANOVA
     
     out_table : str, optional
         the output table
 
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
     params = {
-        'incolumn': in_column,
-        'by': by_column,
-        'treatment': treatment
+        'incolumn': q(in_column),
+        'by': q(by_column),
+        'treatment': q(treatment_column)
     }
     out_df = call_proc_df_in_out(proc="ANOVA_CRD_TEST", in_df=in_df, params=params, out_table=out_table)[0]
     temp_table = make_temp_table_name()
     usual_columns = ', '.join(['TOTNO', 'TOTSU', 'TOTMEAN', 'TOTSS', 'SSCTOT', 'SSCBETWEEN', 
                                       'DFBETWEEN', 'SSCWITHIN', 'DFWITHIN', 'F'])
     query = f"""create table {temp_table} as
             select {'INCOLUMN, ' if len(in_column)>1 else ''} 
-            {by_column + ', ' if by_column else ''} 
+            {'"' + by_column + '", ' if by_column else ''} 
             {usual_columns},
             case when p is null then 0 else p
             end as p 
             from {out_table};
             drop table {out_table};
             alter table {temp_table} rename to {out_table};
             """
     in_df._idadb.ida_query(query)
     return out_df
 
 
-def anova_rbd_test(in_df: IdaDataFrame, in_column: str, treatment: str, block: str, by_column: str=None, out_table: str=None):
+def anova_rbd_test(in_df: IdaDataFrame, in_column: str, treatment_column: str, block_column: str, by_column: str=None, out_table: str=None):
     """
     This function analyzes the variance of one or several observations for different blocks of treatments. 
     It assumes that the input table contains one or several columns with numerical (double) observation 
     results of an experiment concerning treatments indicated by the treatment parameter. 
     The treatments are performed repeatedly in various blocks, e.g. from different laboratories 
     where experiments are carried out. This means there are independent samples (treatments) 
     repeatedly drawn for each block. In particular, the number of observations 
@@ -637,41 +638,41 @@
     ----------
     in_df : IdaDataFrame
         the input data frame
 
     in_column : str
         the input table observation columns, separated by a semi-colon (;) 
     
-    treatment : str
+    treatment_column : str
         the input table column identifying a unique treatment
 
-    block : str
+    block_column : str
         the input table column identifying a unique block of treatments
         
     by_column : str, optional
         the input table column which uniquely identifies a group on which to perform ANOVA
     
     out_table : str, optional
         the output table
 
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
     params = {
-        'incolumn': in_column,
-        'by': by_column,
-        'treatment': treatment,
-        'block': block
+        'incolumn': q(in_column),
+        'by': q(by_column),
+        'treatment': q(treatment_column),
+        'block': q(block_column)
     }
     return call_proc_df_in_out(proc="ANOVA_RBD_TEST", in_df=in_df, params=params, out_table=out_table)[0]
 
 
-def manova_one_way_test(in_df: IdaDataFrame, in_column: str, factor1: str, id_column: str=None, by_column: str=None, 
+def manova_one_way_test(in_df: IdaDataFrame, in_column: str, factor1_column: str, id_column: str=None, by_column: str=None, 
                         table_type: str='trcv', out_table: str=None, timecheck: str=None):
     """
     This function performs one-way analysis of variance/covariance aiming to tell whether or not 
     the groups of data identified by factor1 have the same mean value in all dependent variables or not. 
     As an output 4 matrices (for each task) are produced that are stored in the output table 
     the first matrix describes the ground means of all dependent variables (row vector) 
     the second matrix describes the covariance table stat-istics and their p-values (row vector) 
@@ -683,15 +684,15 @@
     in_df : IdaDataFrame
         the input data frame
 
     in_column : str, optional
         the input table observation columns (dependent variables), separated by a semi-colon (;) 
         used for type='column' only, for type='trcv' these are the values for col-column greater equal 2 
     
-    factor1 : str, optional
+    factor1_column : str, optional
         the input table column identifying a first factor (so-called treatment in RBD/CRD nomenclature) 
         used for type='column' only, for type='trcv' these are the values for col-column equal 1
     
     id_column : str,  optional
         the input table column which uniquely identifies records used for type='column' only, 
         for type='trcv' not needed due to the structure of the table
 
@@ -714,44 +715,44 @@
 
     Returns
     -------
     IdaDataFrame
         the data frame with requested data
     """
     params = {
-        'incolumn': in_column,
-        'by': by_column,
-        'factor1': factor1,
+        'incolumn': q(in_column),
+        'by': q(by_column),
+        'factor1': q(factor1_column),
         'type': table_type,
-        'id': id_column,
+        'id': q(id_column),
         '_timecheck': timecheck
     }
     return call_proc_df_in_out(proc="MANOVA_ONE_WAY_TEST", in_df=in_df, params=params, out_table=out_table)[0]
 
 
-def manova_two_way_test(in_df: IdaDataFrame, in_column: str, factor1: str, factor2: str, table_type: str, 
+def manova_two_way_test(in_df: IdaDataFrame, in_column: str, factor1_column: str, factor2_column: str, table_type: str, 
                         id_column: str=None, by_column: str=None, out_table: str=None, timecheck: str=None):
     """
     This function performs Two-way analysis of variance/covariance aiming to tell whether or 
     not the groups of data identified by factor1 have the same mean value in all dependent variables or not.
 
     Parameters
     ----------
     in_df : IdaDataFrame
         the input data frame
 
     in_column : str
         the input table observation columns (dependent variables), separated by a semi-colon (;) 
         used for type='column' only, for type='trcv' these are the values for col-column greater equal 3 
     
-    factor1 : str
+    factor1_column : str
         the input table column identifying a first factor (so-called treatment in RBD/CRD nomenclature),
         used for type='column' only, for type='trcv' these are the values for col-column equal 1
     
-    factor2: str
+    factor2_column: str
         the input table column identifying a second factor (so-called block in RBD nomenclature),
         used for type='column' only, for type='trcv' these are the values for col-column equal 2
     
     table_type : str
         the input table form: either 'columns' or 'trcv' trcv stands for "id_task, row, column, value" 
         id_task must be positive integer >= 1. columns means the traditional table representation
     
@@ -774,16 +775,16 @@
 
     Returns
     -------
     IdaDataFrame
         the data fąrame with requested data
     """
     params = {
-        'incolumn': in_column,
-        'by': by_column,
-        'factor1': factor1,
-        'factor2': factor2,
+        'incolumn': q(in_column),
+        'by': q(by_column),
+        'factor1': q(factor1_column),
+        'factor2': q(factor2_column),
         'type': table_type,
-        'id': id_column,
+        'id': q(id_column),
         '_timecheck': timecheck
     }
     return call_proc_df_in_out(proc="MANOVA_TWO_WAY_TEST", in_df=in_df, params=params, out_table=out_table)[0]
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/model_manager.py` & `nzpyida-0.9.3/nzpyida/analytics/model_manager.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/analytics/predictive/association_rules.py` & `nzpyida-0.9.3/nzpyida/analytics/predictive/association_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 of data set scans. It can also perform efficiently, regardless of the threshold support.
 """
 
 from typing import List
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.predictive.predictive_modeling import PredictiveModeling
+from nzpyida.analytics.utils import q
 
 class ARule(PredictiveModeling):
     def __init__(self, idadb: IdaDataBase, model_name: str):
         """
         Creates Association Rules Class
 
         Parameters
@@ -138,17 +139,17 @@
             default - 0.5
             min - 0
             max - 1 
         """
         if support_type == 'percent' and not support:
             support = 5.0
         params = {
-            'tid': transaction_id_column,
-            'item': item_column,
-            'by': by_column,
+            'tid': q(transaction_id_column),
+            'item': q(item_column),
+            'by': q(by_column),
             'lvl': level,
             'maxsetsize': max_set_size,
             'support': support,
             'supporttype': support_type,
             'confidence': confidence
         }
 
@@ -244,17 +245,17 @@
 
         Returns
         -------
         IdaDataFrame
             the data frame containing output of a Association Rules model prediction
         """
         params = {
-            'tid': transaction_id_column,
-            'item': item_column,
-            'by': by_column,
+            'tid': q(transaction_id_column),
+            'item': q(item_column),
+            'by': q(by_column),
             'type': scoring_type,
             'namemap': name_map_column,
             'itemname': item_name_column,
             'itemnamemapped': item_name_mapped_column,
             'minsize': min_size,
             'maxsize': max_size,
             'minsupp': min_support,
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/predictive/bayesian_networks.py` & `nzpyida-0.9.3/nzpyida/analytics/predictive/bayesian_networks.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 """
 
 from typing import Tuple, List
 from nzpyida.analytics.model_manager import ModelManager
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.utils import map_to_props, materialize_df, make_temp_table_name
-from nzpyida.analytics.utils import get_auto_delete_context
+from nzpyida.analytics.utils import get_auto_delete_context, q
 from nzpyida.analytics.predictive.regression import Regression
 from nzpyida.analytics.predictive.predictive_modeling import PredictiveModeling
 
 
 class TreeBayesNetwork(Regression):
     def __init__(self, idadb: IdaDataBase, model_name: str):
         """
@@ -120,15 +120,15 @@
             detected automatically.
             (Remark: colPropertiesTable with "COLROLE" column with value 'objweight'
             is unsupported, i.e. same as 'ignore')
             (Remark: colPropertiesTable with "COLWEIGHT" column with value '<wgt>' is unsupported,
             i.e. same as '1')
         """
         params = {
-            'incolumn': in_columns,
+            'incolumn': q(in_columns),
             'coldeftype': col_def_type,
             'coldefrole': col_def_role,
             'colPropertiesTable': col_properties_table,
             'baseidx': base_index,
             'samplesize': sample_size,
             'talk': talk,
             'edgelabsort': edge_lab_sort
@@ -164,16 +164,16 @@
         
         Returns
         -------
         IdaDataFrame
             the data frame containing row identifiers and predicted target values
         """
         params = {
-            'id': id_column,
-            'target': target_column,
+            'id': q(id_column),
+            'target': q(target_column),
             'type': prediction_type
         }
         return self._predict(in_df, params, out_table)
     
 
     def score(self, in_df: IdaDataFrame, target_column: str=None, id_column: str=None,
               prediction_type: str='best') -> float:
@@ -198,17 +198,17 @@
 
         Returns
         -------
         float
             the model score
         """
         params = {
-            'id': id_column,
+            'id': q(id_column),
             'type': prediction_type,
-            'target': target_column
+            'target': q(target_column)
         }
         self.target_column_in_output = f"{target_column}_PRED"
         return self._score(in_df, params, target_column)
 
 
 
 class BinaryTreeBayesNetwork(TreeBayesNetwork):
@@ -246,15 +246,15 @@
         
         edge_lab_sort : str, optional
             if edge_lab_sort=yes then the left end of the edge will have a name lower 
             in alphabetic order than the right one
         """
         params = {
             'inmodel': in_model,
-            'class': class_column,
+            'class': q(class_column),
             'edge_lab_sort': edge_lab_sort
         }
         self._fit(in_df, params, needs_id=False)
 
 
 class MultiTreeBayesNetwork(TreeBayesNetwork):
     def __init__(self, idadb: IdaDataBase, model_name: str):
@@ -324,16 +324,16 @@
             detected automatically.
             (Remark: colPropertiesTable with "COLROLE" column with value 'objweight'
             is unsupported, i.e. same as 'ignore')
             (Remark: colPropertiesTable with "COLWEIGHT" column with value '<wgt>' is unsupported,
             i.e. same as '1')
         """
         params = {
-            'class': class_column,
-            'incolumn': in_columns,
+            'class': q(class_column),
+            'incolumn': q(in_columns),
             'coldeftype': col_def_type,
             'coldefrole': col_def_role,
             'colPropertiesTable': col_properties_table,
             'baseidx': base_index,
             'samplesize': sample_size,
             'talk': talk,
             'edgelabsort': edge_lab_sort
@@ -469,15 +469,15 @@
         Returns
         -------
         IdaDataFrame
             the data frame containing statistics
         """
         params = {
             'model': self.model_name,
-            'incolumn': in_columns,
+            'incolumn': q(in_columns),
             'coldeftype': col_def_type,
             'coldefrole': col_def_role,
             'colPropertiesTable': col_properties_table,
             'baseidx': base_index,
             'samplesize': sample_size,
             'talk': talk,
             'nocheck': no_check,
@@ -567,15 +567,15 @@
         Returns
         -------
         IdaDataFrame
             the data frame containing statistics
         """
         params = {
             'model': self.model_name,
-            'incolumn': in_columns,
+            'incolumn': q(in_columns),
             'coldeftype': col_def_type,
             'coldefrole': col_def_role,
             'colPropertiesTable': col_properties_table,
             'baseidx': base_index,
             'talk': talk,
             'nocheck': no_check,
             'edgelabsort': edge_lab_sort
@@ -663,15 +663,15 @@
         Returns
         -------
         IdaDataFrame
             the data frame containing statistics
         """
         params = {
             'model': self.model_name,
-            'incolumn': in_columns,
+            'incolumn': q(in_columns),
             'coldeftype': col_def_type,
             'coldefrole': col_def_role,
             'colPropertiesTable': col_properties_table,
             'baseidx': base_index,
             'talk': talk,
             'nocheck': no_check,
             'edgelabsort': edge_lab_sort
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/predictive/bisecting_kmeans.py` & `nzpyida-0.9.3/nzpyida/analytics/predictive/bisecting_kmeans.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 
 from typing import List
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.utils import map_to_props, make_temp_table_name
 from nzpyida.analytics.utils import get_auto_delete_context
 from nzpyida.analytics.predictive.predictive_modeling import PredictiveModeling
+from nzpyida.analytics.utils import q
+
 
 class BisectingKMeans(PredictiveModeling):
     """
     Divisive Clustering
     """
     def __init__(self, idadb: IdaDataBase, model_name: str):
         """
@@ -69,16 +71,16 @@
             it must be trained using fit() function before prediction or scoring is called.
         """
 
         super().__init__(idadb, model_name)
         self.fit_proc = 'DIVCLUSTER'
         self.predict_proc = 'PREDICT_DIVCLUSTER'
         self.score_proc = 'MSE'
-        self.target_column_in_output = 'CLUSTER_ID'
-        self.id_column_in_output = 'ID'
+        self.target_column_in_output = idadb.to_def_case('CLUSTER_ID')
+        self.id_column_in_output = idadb.to_def_case('ID')
         self.has_print_proc = True
 
     def fit(self, in_df: IdaDataFrame, id_column: str=None, target_column: str=None,
         in_columns: List[str]=None, col_def_type: str=None, col_def_role: str=None,
         col_properties_table: str=None, out_table: str=None, distance: str='euclidean',
         max_iter: int=5, min_split: int=5, max_depth: int=3, rand_seed: int=12345) -> IdaDataFrame:
         """
@@ -165,17 +167,17 @@
 
         auto_delete_context = None
         if not out_table:
             auto_delete_context = get_auto_delete_context('out_table')
             out_table = make_temp_table_name()
 
         params = {
-            'id': id_column,
-            'target': target_column,
-            'incolumn': in_columns,
+            'id': q(id_column),
+            'target': q(target_column),
+            'incolumn': q(in_columns),
             'coldeftype': col_def_type,
             'coldefrole': col_def_role,
             'colpropertiestable': col_properties_table,
             'distance': distance,
             'maxiter': max_iter,
             'minsplit': min_split,
             'maxdepth': max_depth,
@@ -214,15 +216,15 @@
         Returns
         -------
         IdaDataFrame
             the data frame containing row identifiers and predicted target values
         """
 
         params = {
-            'id': id_column,
+            'id': q(id_column),
             'level': level
         }
 
         return self._predict(in_df=in_df, params=params, out_table=out_table)
 
     def score(self, in_df: IdaDataFrame, target_column: str,
         id_column: str=None, level: int=-1) -> float:
@@ -248,12 +250,12 @@
         Returns
         -------
         float
             the model score
         """
 
         params = {
-            'id': id_column,
+            'id': q(id_column),
             'level': level
         }
 
         return self._score(in_df=in_df, predict_params=params, target_column=target_column)
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/predictive/classification.py` & `nzpyida-0.9.3/nzpyida/analytics/predictive/classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.utils import map_to_props, materialize_df, make_temp_table_name, \
 call_proc_df_in_out
 from nzpyida.analytics.utils import get_auto_delete_context
 from nzpyida.analytics.predictive.predictive_modeling import PredictiveModeling
 from nzpyida.analytics.model_manager import ModelManager
+from nzpyida.analytics.utils import q
 
 
 class Classification(PredictiveModeling):
     """
     Base class for classification algorithms.
     """
 
@@ -38,16 +39,16 @@
 
         model_name : str
             model name - if it exists in the database, it will be used, otherwise
             it must be trained using fit() function before prediction or scoring is called.
         """
 
         super().__init__(idadb, model_name)
-        self.target_column_in_output = 'CLASS'
-        self.id_column_in_output = 'ID'
+        self.target_column_in_output = idadb.to_def_case('CLASS')
+        self.id_column_in_output = idadb.to_def_case('ID')
         self.score_proc = 'CERROR'
         self.score_inv = True
         self.type = None
 
     def predict(self, in_df: IdaDataFrame, out_table: str=None,
         id_column: str=None) -> IdaDataFrame:
         """
@@ -63,15 +64,15 @@
 
         id_column : str, optional
             the input table column identifying a unique instance id
             Default: id column used to build the model
         """
 
         params = {
-            'id': id_column
+            'id': q(id_column)
         }
 
         return self._predict(in_df=in_df, params=params, out_table=out_table)
 
     def score(self, in_df: IdaDataFrame, target_column: str, id_column: str=None) -> float:
         """
         Scores the model. The model must exist.
@@ -91,15 +92,15 @@
         Returns
         -------
         float
             the model score
         """
 
         params = {
-            'id': id_column
+            'id': q(id_column)
         }
 
         return self._score(in_df=in_df, predict_params=params, target_column=target_column)
 
     def conf_matrix(self, in_df: IdaDataFrame, target_column: str, id_column: str=None,
         out_matrix_table: str=None) -> Tuple[IdaDataFrame, float, float]:
         """
@@ -130,28 +131,28 @@
             classification accuracy (ACC)
 
         float
             weighted classification accuracy (WACC)
         """
 
         params = {
-            'id': id_column,
-            'target': target_column
+            'id': q(id_column),
+            'target': q(target_column)
         }
         return self._conf_matrix(in_df, out_matrix_table, params)
         
     def _conf_matrix(self, in_df: IdaDataFrame, out_matrix_table: str=None,
                      params: dict={}) -> Tuple[IdaDataFrame, float, float]:
 
         if not isinstance(in_df, IdaDataFrame):
             raise TypeError("Argument in_df should be an IdaDataFrame")
 
         if not params.get('id'):
             if in_df.indexer:
-                params['id'] = in_df.indexer
+                params['id'] = q(in_df.indexer)
             else:
                 raise TypeError('Missing id column - either use id_column attribute or set '
                     'indexer column in the input data frame')
 
         out_table = make_temp_table_name()
 
         pred_view_needs_delete, true_view_needs_delete = False, False
@@ -164,17 +165,17 @@
             if not out_matrix_table:
                 auto_delete_context = get_auto_delete_context('out_matrix_table')
                 out_matrix_table = make_temp_table_name()
 
             params_s = map_to_props({
                 'resulttable': pred_view,
                 'intable': true_view,
-                'resultid': 'ID',
+                'resultid': self.idadb.to_def_case('ID'),
                 'id': params['id'],
-                'resulttarget': 'CLASS',
+                'resulttarget': self.idadb.to_def_case('CLASS'),
                 'target': params['target'],
                 'matrixTable': out_matrix_table
             })
             self.idadb.ida_query(f'call NZA..CONFUSION_MATRIX(\'{params_s}\')')
 
             if auto_delete_context:
                 auto_delete_context.add_table_to_delete(out_matrix_table)
@@ -227,16 +228,16 @@
         float
             classification accuracy (ACC) for all batches 
         """
         params = {
             'modelType': self.fit_proc,
             'model': self.model_name,
             'intable': in_df,
-            'id': id_column,
-            'target': target_column,
+            'id': q(id_column),
+            'target': q(target_column),
             'outtable': out_table,
             'folds': folds,
         }
         if isinstance(rand_seed, int):
             params['seed'] = rand_seed
         
         ModelManager(self.idadb).drop_model(self.model_name)
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/predictive/decision_trees.py` & `nzpyida-0.9.3/nzpyida/analytics/predictive/decision_trees.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 generalize better.
 """
 
 from typing import List
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.predictive.classification import Classification
+from nzpyida.analytics.utils import q
 
 
 class DecisionTreeClassifier(Classification):
     """
     Decision tree based classifier.
     """
 
@@ -168,17 +169,17 @@
                 frequent column statistics are kept.
                 If a numeric column contains more than <n> values, the values will be
                 discretized and the statistics will be collected on the discretized values.
             Indicating statistics=all is equal to statistics=values:100.
         """
 
         params = {
-            'id': id_column,
-            'target': target_column,
-            'incolumn': in_columns,
+            'id': q(id_column),
+            'target': q(target_column),
+            'incolumn': q(in_columns),
             'coldeftype': col_def_type,
             'coldefrole': col_def_role,
             'colpropertiestable': col_properties_table,
             'weights': weights,
             'eval': eval_measure,
             'minimprove': min_improve,
             'minsplit': min_split,
@@ -220,13 +221,13 @@
         Returns
         -------
         IdaDataFrame
             the data frame containing row identifiers and predicted target values
         """
 
         params = {
-            'id': id_column,
+            'id': q(id_column),
             'prob': prob,
             'outtableprob': out_table_prob
         }
 
         return self._predict(in_df=in_df, params=params, out_table=out_table)
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/predictive/glm.py` & `nzpyida-0.9.3/nzpyida/analytics/predictive/glm.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from nzpyida.analytics.utils import call_proc_df_in_out, make_temp_table_name, out_str_to_df
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from typing import List
 import pandas as pd
 from nzpyida.analytics.predictive.regression import Regression
+from nzpyida.analytics.utils import q
 
 
 class GLM(Regression):
     """ 
     General Linear Regression model
     """
     def __init__(self, idadb: IdaDataBase, model_name: str):
@@ -35,15 +36,16 @@
             model name - if it exists in the database, it will be used, otherwise
             it must be trained using fit() function before prediction or scoring is called.
         """
         super().__init__(idadb, model_name)
         self.fit_proc = "GLM"
         self.predict_proc = "PREDICT_GLM"
         self.has_print_proc = True
-        self.target_column_in_output = 'PRED'
+        self.target_column_in_output = idadb.to_def_case('PRED')
+        self.id_column_in_output = None
 
     
     def fit(self, in_df: IdaDataFrame, target_column: str, id_column: str=None, in_columns: List[str]=None,  
             intercept: bool=True, interaction: str='', family_param: float=-1, link: str='logit', 
             link_param: float=1, max_iter: int=20, epsilon: float=1e-3, tolerance: float=1e-7, 
             method: str='irls', trials: str='', debug: bool=False, col_def_type: str=None, 
             col_def_role: str=None, col_properties_table: str=None):
@@ -131,17 +133,17 @@
             the input table where column properties for the input dataframe columns are stored. 
             The format of this table is the output format of stored procedure nza..COLUMN_PROPER-TIES().
             If the parameter is undefined, the input table column properties will be detected automatically.
             (Remark: colPropertiesTable with "COLWEIGHT" column with value '<wgt>' is unsupported, i.e. same as '1')
         """
         params = {
             'family': self.family,
-            'target': target_column,
-            'id': id_column,
-            'incolumn': in_columns,
+            'target': q(target_column),
+            'id': q(id_column),
+            'incolumn': q(in_columns),
             'coldefrole': col_def_role,
             'coldeftype': col_def_type,
             'colPropertiesTable': col_properties_table,
             'intercept': intercept,
             'family_param': family_param,
             'link': link,
             'link_param': link_param,
@@ -150,15 +152,15 @@
             'tol': tolerance,
             'method': method,
             'debug': debug
         }
         if interaction:
             params['interaction'] = interaction
         if trials:
-            params['trials'] = trials
+            params['trials'] = q(trials)
 
         return self._fit(in_df=in_df, params=params)
 
     def predict(self, in_df: IdaDataFrame, out_table: str=None, id_column: str=None, 
                 debug: bool=False):
         """
         in_df : IdaDataFrame
@@ -175,15 +177,15 @@
         
         Returns
         -------
         IdaDataFrame
             the data frame containing row identifiers and predicted target values
         """
         params = {
-            'id': id_column,
+            'id': q(id_column),
             'debug': debug
         }
 
         return self._predict(in_df=in_df, params=params, out_table=out_table)
 
 class BernoulliRegressor(GLM):
     def __init__(self, idadb: IdaDataBase, model_name: str):
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/predictive/kmeans.py` & `nzpyida-0.9.3/nzpyida/analytics/predictive/kmeans.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 function to match instances against cluster centers
 """
 
 from typing import List
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.utils import map_to_props, make_temp_table_name
-from nzpyida.analytics.utils import get_auto_delete_context
+from nzpyida.analytics.utils import get_auto_delete_context, q
 from nzpyida.analytics.predictive.predictive_modeling import PredictiveModeling
 
 
 class KMeans(PredictiveModeling):
     """
     KMeans clustering.
     """
@@ -52,16 +52,16 @@
             it must be trained using fit() function before prediction or scoring is called.
         """
 
         super().__init__(idadb, model_name)
         self.fit_proc = 'KMEANS'
         self.predict_proc = 'PREDICT_KMEANS'
         self.score_proc = 'MSE'
-        self.target_column_in_output = 'CLUSTER_ID'
-        self.id_column_in_output = 'ID'
+        self.target_column_in_output = idadb.to_def_case('CLUSTER_ID')
+        self.id_column_in_output = idadb.to_def_case('ID')
         self.has_print_proc = True
 
     def fit(self, in_df: IdaDataFrame, id_column: str=None,
         in_columns: List[str]=None, col_def_type: str=None, col_def_role: str=None,
         col_properties_table: str=None, out_table: str=None, distance: str='norm_euclidean',
         k: int=3, max_iter: int=5, rand_seed: int=12345, id_based: bool=False,
         statistics: str=None, transform: str='L') -> IdaDataFrame:
@@ -170,27 +170,27 @@
 
         """
         if not isinstance(in_df, IdaDataFrame):
             raise TypeError("Argument in_df should be an IdaDataFrame")
 
         if not id_column:
             if in_df.indexer:
-                id_column = in_df.indexer
+                id_column = q(in_df.indexer)
             else:
                 raise TypeError('Missing id column - either use id_column attribute or set '
                     'indexer column in the input data frame')
 
         auto_delete_context = None
         if not out_table:
             auto_delete_context = get_auto_delete_context('out_table')
             out_table = make_temp_table_name()
 
         params = {
-            'id': id_column,
-            'incolumn': in_columns,
+            'id': q(id_column),
+            'incolumn': q(in_columns),
             'coldeftype': col_def_type,
             'coldefrole': col_def_role,
             'colpropertiestable': col_properties_table,
             'distance': distance,
             'k': k,
             'maxiter': max_iter,
             'randseed': rand_seed,
@@ -227,15 +227,15 @@
         Returns
         -------
         IdaDataFrame
             the data frame containing row identifiers and predicted target values
         """
 
         params = {
-            'id': id_column
+            'id': q(id_column)
         }
 
         return self._predict(in_df=in_df, params=params, out_table=out_table)
 
     def score(self, in_df: IdaDataFrame, target_column: str,
         id_column: str=None) -> float:
         """
@@ -256,11 +256,11 @@
         Returns
         -------
         float
             the model score
         """
 
         params = {
-            'id': id_column
+            'id': q(id_column)
         }
 
         return self._score(in_df=in_df, predict_params=params, target_column=target_column)
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/predictive/knn.py` & `nzpyida-0.9.3/nzpyida/analytics/predictive/knn.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 of this approach, which is to replace model creation by memorizing the
 training data set and using it appropriately to make predictions.
 """
 from typing import List
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.predictive.classification import Classification
+from nzpyida.analytics.utils import q
 
 
 class KNeighborsClassifier(Classification):
     """
     K-neighbors based classifier.
     """
 
@@ -82,17 +83,17 @@
         col_properties_table : str, optional
             the input table where column properties for the input table columns are stored.
             If the parameter is undefined, the input table column properties will be detected
             automatically.
         """
 
         params = {
-            'id': id_column,
-            'target': target_column,
-            'incolumn': in_columns,
+            'id': q(id_column),
+            'target': q(target_column),
+            'incolumn': q(in_columns),
             'coldeftype': col_def_type,
             'coldefrole': col_def_role,
             'colpropertiestable': col_properties_table,
         }
 
         self._fit(in_df=in_df, params=params)
 
@@ -143,15 +144,15 @@
         -------
         IdaDataFrame
             a data frame with id and predicted class
 
         """
 
         params = {
-            'id': id_column,
+            'id': q(id_column),
             'distance': distance,
             'k': k,
             'stand': stand,
             'fast': fast,
             'weights': weights
         }
 
@@ -202,16 +203,16 @@
         Returns
         -------
         float
             model classification error ratio
         """
 
         params = {
-            'id': id_column,
-            'target': target_column,
+            'id': q(id_column),
+            'target': q(target_column),
             'distance': distance,
             'k': k,
             'stand': stand,
             'fast': fast,
             'weights': weights
         }
 
@@ -245,16 +246,16 @@
         float
             classification accuracy (ACC)
 
         float
             weighted classification accuracy (WACC)
         """
         params = {
-            'id': id_column,
-            'target': target_column,
+            'id': q(id_column),
+            'target': q(target_column),
             'distance': distance,
             'k': k,
             'stand': stand,
             'fast': fast,
             'weights': weights
         }
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/predictive/linear_regression.py` & `nzpyida-0.9.3/nzpyida/analytics/predictive/linear_regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 linear relationships. It is the thing that limits its applicability, a linear
 model representation, that makes it fast, efficient, and easy to use (compared
 to more refined regression algorithms).
 """
 from typing import List
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
-
 from nzpyida.analytics.predictive.regression import Regression
+from nzpyida.analytics.utils import q
 
 
 class LinearRegression(Regression):
     """
     Linear regression predictive model.
     """
 
@@ -112,18 +112,18 @@
             The default has changed to true.
 
         calculate_diagnostics : bool, optional
             a flag indicating whether diagnostics information should be displayed
         """
 
         params = {
-            'id': id_column,
-            'target': target_column,
-            'nominalCols': nominal_colums,
-            'incolumn': in_columns,
+            'id': q(id_column),
+            'target': q(target_column),
+            'nominalCols': q(nominal_colums),
+            'incolumn': q(in_columns),
             'coldeftype': col_def_type,
             'coldefrole': col_def_role,
             'colpropertiestable': col_properties_table,
             'useSVDSolver': use_svd_solver,
             'intercept': intercept,
             'calculateDiagnostics': calculate_diagnostics
         }
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/predictive/naive_bayes.py` & `nzpyida-0.9.3/nzpyida/analytics/predictive/naive_bayes.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 cases it may be able to deliver similar results in a fraction of the
 computation time.
 """
 from typing import List
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.predictive.classification import Classification
+from nzpyida.analytics.utils import q
 
 class NaiveBayesClassifier(Classification):
     """
     Naive Bayes classifier
     """
     def __init__(self, idadb: IdaDataBase, model_name: str):
         """
@@ -95,17 +96,17 @@
             discretization type for numeric columns [ew, ef, em]
 
         bins : int, optional
             default number of bins for numeric columns
         """
 
         params = {
-            'id': id_column,
-            'target': target_column,
-            'incolumn': in_columns,
+            'id': q(id_column),
+            'target': q(target_column),
+            'incolumn': q(in_columns),
             'coldeftype': col_def_type,
             'coldefrole': col_def_role,
             'colpropertiestable': col_properties_table,
             'disc': disc,
             'bins': bins
         }
 
@@ -140,13 +141,13 @@
         Returns
         -------
         IdaDataFrame
             the data frame containing row identifiers and predicted target values
         """
 
         params = {
-            'id': id_column,
+            'id': q(id_column),
             'outtableProb': out_table_prob,
             'mestimation': mestimation
             }
 
         return self._predict(in_df=in_df, params=params, out_table=out_table)
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/predictive/predictive_modeling.py` & `nzpyida-0.9.3/nzpyida/analytics/predictive/predictive_modeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #-----------------------------------------------------------------------------
 """
 This module contains a class that is the base for all predictive algorithms.
 """
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.utils import map_to_props, materialize_df, make_temp_table_name
-from nzpyida.analytics.utils import call_proc_df_in_out
+from nzpyida.analytics.utils import call_proc_df_in_out, q
 from nzpyida.analytics.model_manager import ModelManager
 
 
 class PredictiveModeling:
     """
     Generic class for predictive modeling algorithms.
     """
@@ -61,15 +61,15 @@
             the dictionary of attributes used to build the model
         """
         if not isinstance(in_df, IdaDataFrame):
             raise TypeError("Argument in_df should be an IdaDataFrame")
 
         if not params.get('id', None) and needs_id:
             if in_df.indexer:
-                params['id'] = in_df.indexer
+                params['id'] = q(in_df.indexer)
             else:
                 raise TypeError('Missing id column - either use id_column attribute or set '
                     'indexer column in the input data frame')
 
         ModelManager(self.idadb).drop_model(self.model_name)
 
         temp_view_name, need_delete = materialize_df(in_df)
@@ -132,15 +132,15 @@
             the model score
         """
         if not isinstance(in_df, IdaDataFrame):
             raise TypeError("Argument in_df should be an IdaDataFrame")
 
         if not predict_params.get('id', None):
             if in_df.indexer:
-                predict_params['id'] = in_df.indexer
+                predict_params['id'] = q(in_df.indexer)
             else:
                 raise TypeError('Missing id column - either use id_column attribute or set '
                     'indexer column in the input data frame')
 
         out_table = make_temp_table_name()
 
         pred_view_needs_delete, true_view_needs_delete = False, False
@@ -152,20 +152,20 @@
             true_view, true_view_needs_delete = materialize_df(in_df)
 
             id_column = predict_params.get('id')
 
             params = map_to_props({
                 'pred_table': pred_view,
                 'true_table': true_view,
-                'pred_id': id_column if self.id_column_in_output is None
-                    else self.id_column_in_output,
-                'true_id': id_column,
-                'pred_column': target_column if self.target_column_in_output is None
-                    else self.target_column_in_output,
-                'true_column': target_column
+                'pred_id': q(id_column) if self.id_column_in_output is None
+                    else q(self.id_column_in_output),
+                'true_id': q(id_column),
+                'pred_column': q(target_column) if self.target_column_in_output is None
+                    else q(self.target_column_in_output),
+                'true_column': q(target_column)
             })
 
             res = self.idadb.ida_query(f'call NZA..{self.score_proc}(\'{params}\')')
             return 1-res[0] if self.score_inv else res[0]
         finally:
             self.idadb.drop_table(out_table)
             if pred_view_needs_delete:
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/predictive/regression.py` & `nzpyida-0.9.3/nzpyida/analytics/predictive/regression.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #-----------------------------------------------------------------------------
 """
 This module contains a class that is the base for all regression algorithms.
 """
 from typing import Dict
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
-from nzpyida.analytics.utils import map_to_props, materialize_df, make_temp_table_name
+from nzpyida.analytics.utils import map_to_props, materialize_df, make_temp_table_name, q
 from nzpyida.analytics.predictive.predictive_modeling import PredictiveModeling
 
 
 class Regression(PredictiveModeling):
     """
     Base class for regression algorithms.
     """
@@ -36,15 +36,15 @@
         model_name : str
             model name - if it exists in the database, it will be used, otherwise
             it must be trained using fit() function before prediction or scoring is called.
         """
 
         super().__init__(idadb, model_name)
         self.score_proc = 'MSE'
-        self.id_column_in_output = 'ID'
+        self.id_column_in_output = idadb.to_def_case('ID')
 
     def predict(self, in_df: IdaDataFrame, out_table: str=None,
         id_column: str=None) -> IdaDataFrame:
         """
         Makes predictions based on this model. The model must exist.
 
         Parameters
@@ -62,15 +62,15 @@
         Returns
         -------
         IdaDataFrame
             the data frame containing row identifiers and predicted target values
         """
 
         params = {
-            'id': id_column
+            'id': q(id_column)
         }
 
         return self._predict(in_df=in_df, params=params, out_table=out_table)
 
     def score(self, in_df: IdaDataFrame, target_column: str,
         id_column: str=None) -> float:
         """
@@ -91,15 +91,15 @@
         Returns
         -------
         float
             the model score
         """
 
         params = {
-            'id': id_column
+            'id': q(id_column)
         }
 
         return self._score(in_df=in_df, predict_params=params, target_column=target_column)
 
     def score_all(self, in_df: IdaDataFrame, target_column: str,
         id_column: str=None) -> Dict[str, float]:
         """
@@ -123,15 +123,15 @@
             the model scores in a dictionary with MSE, MAE, RSE and RAE as keys
         """
         if not isinstance(in_df, IdaDataFrame):
             raise TypeError("Argument in_df should be an IdaDataFrame")
 
         if not id_column:
             if in_df.indexer:
-                id_column = in_df.indexer
+                id_column = q(in_df.indexer)
             else:
                 raise TypeError('Missing id column - either use id_column attribute or set '
                     'indexer column in the input data frame')
 
         out_table = make_temp_table_name()
 
         pred_view_needs_delete, true_view_needs_delete = False, False
@@ -140,20 +140,20 @@
 
             pred_view, pred_view_needs_delete = materialize_df(pred_df)
             true_view, true_view_needs_delete = materialize_df(in_df)
 
             params = map_to_props({
                 'pred_table': pred_view,
                 'true_table': true_view,
-                'pred_id': id_column if self.id_column_in_output is None
-                    else self.id_column_in_output,
-                'true_id': id_column,
+                'pred_id': q(id_column) if self.id_column_in_output is None
+                    else q(self.id_column_in_output),
+                'true_id': q(id_column),
                 'pred_column': target_column if self.target_column_in_output is None
-                    else self.target_column_in_output,
-                'true_column': target_column
+                    else q(self.target_column_in_output),
+                'true_column': q(target_column)
             })
 
             res1 = pred_df.ida_query(f'call NZA..MSE(\'{params}\')')
             res2 = pred_df.ida_query(f'call NZA..MAE(\'{params}\')')
             res3 = pred_df.ida_query(f'call NZA..RSE(\'{params}\')')
             res4 = pred_df.ida_query(f'call NZA..RAE(\'{params}\')')
             res_dict = {
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/predictive/regression_trees.py` & `nzpyida-0.9.3/nzpyida/analytics/predictive/regression_trees.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 predicted values assigned to regions to which the domain is decomposed by
 the tree structure.
 """
 from typing import List
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.predictive.regression import Regression
-from nzpyida.analytics.utils import map_to_props
+from nzpyida.analytics.utils import map_to_props, q
 
 class DecisionTreeRegressor(Regression):
     """
     Decision tree based regressor
     """
     def __init__(self, idadb: IdaDataBase, model_name: str):
         """
@@ -45,15 +45,15 @@
             model name - if it exists in the database, it will be used, otherwise
             it must be trained using fit() function before prediction or scoring is called.
         """
 
         super().__init__(idadb, model_name)
         self.fit_proc = 'REGTREE'
         self.predict_proc = 'PREDICT_REGTREE'
-        self.target_column_in_output = "CLASS"
+        self.target_column_in_output = idadb.to_def_case("CLASS")
         self.has_print_proc = True
 
     def fit(self, in_df: IdaDataFrame, target_column: str, id_column: str=None,
         in_columns: List[str]=None, col_def_type: str=None, col_def_role: str=None,
         col_properties_table: str=None, eval_measure: str=None, min_improve: float=0.1,
         min_split: int=50, max_depth: int=10, val_table: str=None, qmeasure: str=None,
         statistics: str=None):
@@ -143,17 +143,17 @@
             If a numeric column contains more than <n> values, the values will be discretized
             and the stat-istics will be collected on the discretized values.
             Indicating statistics=all is equal to statistics=values:100.
 
         """
 
         params = {
-            'id': id_column,
-            'target': target_column,
-            'incolumn': in_columns,
+            'id': q(id_column),
+            'target': q(target_column),
+            'incolumn': q(in_columns),
             'coldeftype': col_def_type,
             'coldefrole': col_def_role,
             'colpropertiestable': col_properties_table,
             'eval': eval_measure,
             'minimprove': min_improve,
             'minsplit': min_split,
             'maxdepth': max_depth,
@@ -188,12 +188,12 @@
         Returns
         -------
         IdaDataFrame
             the data frame containing row identifiers and predicted target values
         """
 
         params = {
-            'id': id_column,
+            'id': q(id_column),
             'var': variance
             }
 
         return self._predict(in_df=in_df, params=params, out_table=out_table)
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/predictive/timeseries.py` & `nzpyida-0.9.3/nzpyida/analytics/predictive/timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 """
 from typing import List
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.predictive.predictive_modeling import PredictiveModeling
 from nzpyida.analytics.utils import call_proc_df_in_out
 from nzpyida.analytics.model_manager import ModelManager
+from nzpyida.analytics.utils import q as q0
+
 
 class TimeSeries(PredictiveModeling):
     """
     Time Series Model
     """
     def __init__(self, idadb: IdaDataBase, model_name: str):
         """
@@ -152,17 +154,17 @@
             the output table containing seasonally adjusted values. This parameter is not allowed 
             for algorithm=SpectralAnalysis or algorithm=ARIMA. If not specified, no output table 
             is written out
         """
 
         params = {
             'model': self.model_name,
-            'time': time_column,
-            'target': target_column,
-            'by': by_column,
+            'time': q0(time_column),
+            'target': q0(target_column),
+            'by': q0(by_column),
             'desctable': description_table,
             'algorithm': algorithm,
             'interpolationmethod': interpolation_method,
             'from': from_time,
             'to': to_time,
             'forecasthorizon': forecast_horizon,
             'forecasttimes': forecast_times,
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/predictive/two_step_clustering.py` & `nzpyida-0.9.3/nzpyida/analytics/predictive/two_step_clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 
 from typing import List
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.utils import map_to_props, make_temp_table_name
 from nzpyida.analytics.utils import get_auto_delete_context
 from nzpyida.analytics.predictive.predictive_modeling import PredictiveModeling
+from nzpyida.analytics.utils import q
+
 
 class TwoStepClustering(PredictiveModeling):
     """
     Divisive Clustering
     """
     def __init__(self, idadb: IdaDataBase, model_name: str):
         """
@@ -55,16 +57,16 @@
             it must be trained using fit() function before prediction or scoring is called.
         """
 
         super().__init__(idadb, model_name)
         self.fit_proc = 'TWOSTEP'
         self.predict_proc = 'PREDICT_TWOSTEP'
         self.score_proc = 'MSE'
-        self.target_column_in_output = 'CLUSTER_ID'
-        self.id_column_in_output = 'ID'
+        self.target_column_in_output = idadb.to_def_case('CLUSTER_ID')
+        self.id_column_in_output = idadb.to_def_case('ID')
         self.has_print_proc = True
 
     def fit(self, in_df: IdaDataFrame, id_column: str=None, target_column: str=None,
         in_columns: List[str]=None, col_def_type: str=None, col_def_role: str=None,
         col_properties_table: str=None, out_table: str=None, k: int=0, max_k: int=20, 
         bins: int=10, statistics: str=None, rand_seed: int=12345, distance: str='loglikelihood', 
         distance_threshold: float=None, distance_threshold_factor: float=2.0, 
@@ -197,17 +199,17 @@
 
         auto_delete_context = None
         if not out_table:
             auto_delete_context = get_auto_delete_context('out_table')
             out_table = make_temp_table_name()
 
         params = {
-            'id': id_column,
-            'target': target_column,
-            'incolumn': in_columns,
+            'id': q(id_column),
+            'target': q(target_column),
+            'incolumn': q(in_columns),
             'coldeftype': col_def_type,
             'coldefrole': col_def_role,
             'colpropertiestable': col_properties_table,
             'k': k,
             'maxk': max_k,
             'bins': bins,
             'statistics': statistics,
@@ -250,15 +252,15 @@
         Returns
         -------
         IdaDataFrame
             the data frame containing row identifiers and predicted target values
         """
 
         params = {
-            'id': id_column
+            'id': q(id_column)
         }
 
         return self._predict(in_df=in_df, params=params, out_table=out_table)
 
     def score(self, in_df: IdaDataFrame, target_column: str, id_column: str=None) -> float:
         """
         Scores the model. The model must exist.
@@ -278,11 +280,11 @@
         Returns
         -------
         float
             the model score
         """
 
         params = {
-            'id': id_column
+            'id': q(id_column)
         }
 
         return self._score(in_df=in_df, predict_params=params, target_column=target_column)
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/tests/conftest.py` & `nzpyida-0.9.3/nzpyida/analytics/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/analytics/tests/test_association_rules.py` & `nzpyida-0.9.3/nzpyida/analytics/tests/test_association_rules.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,21 +79,21 @@
     assert not mm.model_exists(MOD_NAME) 
 
     model.fit(idf_train, transaction_id_column='ID', item_column="PRODUCT", 
               support_type='absolute', support=2, confidence=0.4)
     assert mm.model_exists(MOD_NAME) 
 
     pred_ida = model.predict(idf_test, OUT_TABLE_PRED, max_conviction=1.25, 
-                       max_affinity=0.6, min_lift=1.0, min_leverage=0.03)
+                       max_affinity=0.6, min_lift=1.0, min_leverage=0.03, transaction_id_column='TID', item_column='ITEM')
     assert pred_ida
-    assert all(pred_ida.columns == ['GID', 'TID', 'LHS_SID', 'RHS_SID', 'LHS_ITEMS', 'RHS_ITEMS', 'SUPPORT',
-       'CONFIDENCE', 'LIFT', 'CONVICTION', 'AFFINITY', 'LEVERAGE'])
+    assert all(pred_ida.columns == idadb.to_def_case(['GID', 'TID', 'LHS_SID', 'RHS_SID', 'LHS_ITEMS', 'RHS_ITEMS', 'SUPPORT',
+       'CONFIDENCE', 'LIFT', 'CONVICTION', 'AFFINITY', 'LEVERAGE']))
     pred = pred_ida.as_dataframe()
-    assert all(pred["SUPPORT"].values >= 0.2)
-    assert all(pred["CONFIDENCE"].values >= 0.4)
-    assert all(pred["CONVICTION"].values <= 1.25)
-    assert all(pred["AFFINITY"].values <= 0.6)
-    assert all(pred["LIFT"].values >= 1.0)
-    assert all(pred["LEVERAGE"].values >=0.03)
+    assert all(pred[idadb.to_def_case("SUPPORT")].values >= 0.2)
+    assert all(pred[idadb.to_def_case("CONFIDENCE")].values >= 0.4)
+    assert all(pred[idadb.to_def_case("CONVICTION")].values <= 1.25)
+    assert all(pred[idadb.to_def_case("AFFINITY")].values <= 0.6)
+    assert all(pred[idadb.to_def_case("LIFT")].values >= 1.0)
+    assert all(pred[idadb.to_def_case("LEVERAGE")].values >=0.03)
 
     assert model.describe()
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/tests/test_auto_delete_context.py` & `nzpyida-0.9.3/nzpyida/analytics/tests/test_auto_delete_context.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/analytics/tests/test_bayesian_networks.py` & `nzpyida-0.9.3/nzpyida/analytics/tests/test_bayesian_networks.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,46 +81,46 @@
     assert not mm.model_exists(MOD_NAME)
 
     model.fit(idf_train, in_columns=["A", "B"])
     assert mm.model_exists(MOD_NAME)
 
     pred  = model.predict(idf_test, target_column="B", id_column="ID", out_table=OUT_TABLE_PRED)
     assert pred
-    assert all(pred.columns == ["ID", "B_PRED"])
+    assert all(pred.columns == ["ID", "B_" + idadb.to_def_case("PRED")])
     # assert any(round(x) == y for x, y in zip(list(pred.as_dataframe()['B_PRED'].values),  [2, 4, 2223, -999, 11112]))
 
 
 def test_binary_tree_bayes_network(idadb: IdaDataBase, mm: ModelManager, idf_train: IdaDataFrame ,
                                    idf_test: IdaDataFrame , clear_up):
     model = BinaryTreeBayesNetwork(idadb, MOD_NAME)
     assert model
     assert not mm.model_exists(MOD_NAME)
 
     model.fit(idf_train, in_columns=["A", "B"])
     assert mm.model_exists(MOD_NAME)
 
     pred  = model.predict(idf_test, target_column="B", id_column="ID", out_table=OUT_TABLE_PRED)
     assert pred
-    assert all(pred.columns == ["ID", "B_PRED"])
-    assert any(round(x) == y for x, y in zip(list(pred.head()['B_PRED'].values),  [2, 4, 2223, -999, 11112]))
+    assert all(pred.columns == ["ID", "B_" + idadb.to_def_case("PRED")])
+    assert any(round(x) == y for x, y in zip(list(pred.head()['B_'+idadb.to_def_case('PRED')].values),  [2, 4, 2223, -999, 11112]))
 
 
 def test_multi_tree_bayes_network(idadb: IdaDataBase, mm: ModelManager, idf_train_nom: IdaDataFrame ,
                                    idf_test_nom: IdaDataFrame , clear_up):
     model = MultiTreeBayesNetwork(idadb, MOD_NAME)
     assert model
     assert not mm.model_exists(MOD_NAME)
 
     model.fit(idf_train_nom, class_column= "C", in_columns=["A", "B"])
     assert mm.model_exists(MOD_NAME)
 
     pred  = model.predict(idf_test_nom, target_column="B", id_column="ID", out_table=OUT_TABLE_PRED)
     assert pred
-    assert all(pred.columns == ["ID", "B_PRED"])
-    assert any(round(x) == y for x, y in zip(list(pred.head()['B_PRED'].values),  [2, 4, 2223, -999, 11112]))
+    assert all(pred.columns == ["ID", "B_" + idadb.to_def_case("PRED")])
+    assert any(round(x) == y for x, y in zip(list(pred.head()['B_' + idadb.to_def_case('PRED')].values),  [2, 4, 2223, -999, 11112]))
 
 
 def test_tree_bayes_network_1g(idadb: IdaDataBase, mm: ModelManager, idf_train: IdaDataFrame,
                                clear_up):
     
     model = TreeBayesNetwork1G(idadb, MOD_NAME)
     assert model
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/tests/test_bisecting_kmeans.py` & `nzpyida-0.9.3/nzpyida/analytics/tests/test_bisecting_kmeans.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,13 +54,13 @@
     
     model.fit(idf_train, distance='manhattan', max_iter=4, min_split=3, max_depth=2,
               rand_seed=4321, out_table=OUT_TABLE_CLUST)
     assert mm.model_exists(MOD_NAME)
 
     pred = model.predict(idf_test, level=5, out_table=OUT_TABLE_PRED)
     assert pred
-    assert all(pred.columns == ['ID', 'CLUSTER_ID', 'DISTANCE'])
-    assert all(list(pred.as_dataframe()['CLUSTER_ID'].values))
+    assert all(pred.columns == idadb.to_def_case(['ID', 'CLUSTER_ID', 'DISTANCE']))
+    assert all(list(pred.as_dataframe()[idadb.to_def_case('CLUSTER_ID')].values))
 
     score = model.score(idf_test, target_column="A")
 
     assert score
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/tests/test_cross_validation.py` & `nzpyida-0.9.3/nzpyida/analytics/tests/test_cross_validation.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,8 +47,8 @@
     with AutoDeleteContext(idadb):
         df_cv, acc = model.cross_validation(idf, id_column="ID", target_column="B")
         assert acc
         assert acc > 0.99
 
         assert df_cv
         assert len(df_cv) == len(idf)
-        assert all(df_cv.columns == ["ID", "CLASS", "FOLD"])
+        assert all(df_cv.columns == idadb.to_def_case(["ID", "CLASS", "FOLD"]))
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/tests/test_decision_trees.py` & `nzpyida-0.9.3/nzpyida/analytics/tests/test_decision_trees.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,22 +54,22 @@
     assert not mm.model_exists(MOD_NAME)
     
     model.fit(idf_train, id_column="ID", target_column="B", eval_measure='gini', min_improve=0, min_split=200)
     assert mm.model_exists(MOD_NAME)
 
     pred = model.predict(idf_test, id_column="ID", out_table=OUT_TABLE_PRED)
     assert pred
-    assert all(pred.columns == ['ID', 'CLASS'])
-    assert list(pred.as_dataframe()['CLASS'].values) in (['p', 'n', 'n'], ['p', 'p', 'n'])
+    assert all(pred.columns == idadb.to_def_case(['ID', 'CLASS']))
+    assert list(pred.as_dataframe()[idadb.to_def_case('CLASS')].values) in (['p', 'n', 'n'], ['p', 'p', 'n'])
 
     score = model.score(idf_test, id_column="ID", target_column="B")
 
     assert score
     assert score >= 0.66
 
     cm, acc, wacc = model.conf_matrix(idf_test, id_column='ID', target_column='B', out_matrix_table=OUT_TABLE_CM)
     assert all([cm, acc, wacc])
-    assert all(cm.columns == ['REAL', 'PREDICTION', 'CNT'])
+    assert all(cm.columns == idadb.to_def_case(['REAL', 'PREDICTION', 'CNT']))
     assert len(cm) >= 2
-    assert sum(cm.as_dataframe()["CNT"].values) == 3
+    assert sum(cm.as_dataframe()[idadb.to_def_case("CNT")].values) == 3
     assert wacc >= 0.75
     assert acc >= 0.66
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/tests/test_discretization.py` & `nzpyida-0.9.3/nzpyida/analytics/tests/test_discretization.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,43 +26,43 @@
 
 def test_ewdisc(idadb: IdaDataBase, idf):
     with AutoDeleteContext(idadb):
         ewdisc = EWDisc(idadb, bins=5)
         bin_df = ewdisc.fit(idf)
         assert bin_df
         assert len(bin_df) == 4
-        assert all(bin_df.columns == ['COLNAME', 'BREAK'])
+        assert all(bin_df.columns == idadb.to_def_case(['COLNAME', 'BREAK']))
 
         ew_df = ewdisc.apply(idf, in_bin_df=bin_df, keep_org_values=True)
         assert ew_df
         assert len(ew_df) == len(idf)
-        assert all(ew_df.columns == ['A', 'DISC_A'])
-        assert set(ew_df['DISC_A'].head(10).values) == {'1', '2', '3', '4', '5'}
+        assert all(ew_df.columns == ['A', idadb.to_def_case('DISC') + '_A'])
+        assert set(ew_df[idadb.to_def_case('DISC') + '_A'].head(10).values) == {'1', '2', '3', '4', '5'}
 
 
 def test_efdisc(idadb: IdaDataBase, idf):
     with AutoDeleteContext(idadb):
         efdisc = EFDisc(idadb, bins=2)
         bin_df = efdisc.fit(idf)
         assert bin_df
         assert len(bin_df) == 1
-        assert all(bin_df.columns == ['COLNAME', 'BREAK'])
+        assert all(bin_df.columns == idadb.to_def_case(['COLNAME', 'BREAK']))
 
         ef_df = efdisc.apply(idf, in_bin_df=bin_df, keep_org_values=True)
         assert ef_df
         assert len(ef_df) == len(idf)
-        assert all(ef_df.columns == ['A', 'DISC_A'])
-        assert set(ef_df['DISC_A'].head(10).values) == {'1', '2'}
+        assert all(ef_df.columns == ['A', idadb.to_def_case('DISC') + '_A'])
+        assert set(ef_df[idadb.to_def_case('DISC') + '_A'].head(10).values) == {'1', '2'}
 
 
 def test_emdisc(idadb: IdaDataBase, idf):
     with AutoDeleteContext(idadb):
         emdisc = EMDisc(idadb, target='A')
         bin_df = emdisc.fit(idf)
         assert bin_df
-        assert all(bin_df.columns == ['COLNAME', 'BREAK'])
+        assert all(bin_df.columns == idadb.to_def_case(['COLNAME', 'BREAK']))
 
         em_df = emdisc.apply(idf, in_bin_df=bin_df, keep_org_values=True)
         assert em_df
         assert len(em_df) == len(idf)
-        assert all(em_df.columns == ['A', 'DISC_A'])
-        assert len(set(em_df['DISC_A'].head(10).values)) < len(idf)
+        assert all(em_df.columns == ['A', idadb.to_def_case('DISC') + '_A'])
+        assert len(set(em_df[idadb.to_def_case('DISC') + '_A'].head(10).values)) < len(idf)
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/tests/test_glm.py` & `nzpyida-0.9.3/nzpyida/analytics/tests/test_glm.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     for k, v in model_info["params"].items():
         params[k] = v
     model.fit(**params)
     assert mm.model_exists(MOD_NAME)
 
     pred = model.predict(idf_test, id_column="ID", out_table=OUT_TABLE_PRED)
     assert pred
-    assert all(pred.columns == ['ID', 'PRED'])
+    assert all(pred.columns == ['ID', idadb.to_def_case('PRED')])
     # assert any(round(x) == y for x, y in zip(list(pred.as_dataframe()['CLASS'].values),  [1, 4, 2223, -999, 11112]))
 
     score = model.score(idf_test, id_column="ID", target_column="B")
 
     assert score
 
     mse, mae, rse, rae = model.score_all(idf_test, id_column='ID', target_column='B')
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/tests/test_kmeans.py` & `nzpyida-0.9.3/nzpyida/analytics/tests/test_kmeans.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,13 +53,13 @@
     assert not mm.model_exists(MOD_NAME)
     
     model.fit(idf_train, k=3, out_table=OUT_TABLE_CLUST)
     assert mm.model_exists(MOD_NAME)
 
     pred = model.predict(idf_test, out_table=OUT_TABLE_PRED)
     assert pred
-    assert all(pred.columns == ['ID', 'CLUSTER_ID', 'DISTANCE'])
-    assert all(list(pred.as_dataframe()['CLUSTER_ID'].values))
+    assert all(pred.columns == idadb.to_def_case(['ID', 'CLUSTER_ID', 'DISTANCE']))
+    assert all(list(pred.as_dataframe()[idadb.to_def_case('CLUSTER_ID')].values))
 
     score = model.score(idf_test, target_column="A")
 
     assert score
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/tests/test_knn.py` & `nzpyida-0.9.3/nzpyida/analytics/tests/test_knn.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,22 +54,22 @@
     assert not mm.model_exists(MOD_NAME)
     
     model.fit(idf_train, id_column="ID", target_column="B")
     assert mm.model_exists(MOD_NAME)
 
     pred = model.predict(idf_test, id_column="ID", out_table=OUT_TABLE_PRED)
     assert pred
-    assert all(pred.columns == ['ID', 'CLASS'])
-    assert list(pred.head()['CLASS'].values) == ['p', 'n', 'n']
+    assert all(pred.columns == idadb.to_def_case(['ID', 'CLASS']))
+    assert list(pred.head()[idadb.to_def_case('CLASS')].values) == ['p', 'n', 'n']
 
     score = model.score(idf_test, id_column="ID", target_column="B")
 
     assert score
     assert 0.67 >= score >= 0.66
 
     cm, acc, wacc = model.conf_matrix(idf_test, id_column='ID', target_column='B', out_matrix_table=OUT_TABLE_CM)
     assert all([cm, acc, wacc])
-    assert all(cm.columns == ['REAL', 'PREDICTION', 'CNT'])
+    assert all(cm.columns == idadb.to_def_case(['REAL', 'PREDICTION', 'CNT']))
     assert len(cm) >= 3
-    assert sum(cm.as_dataframe()["CNT"].values) == 3
+    assert sum(cm.as_dataframe()[idadb.to_def_case("CNT")].values) == 3
     assert wacc == 0.75
     assert 0.67 >= acc >= 0.66
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/tests/test_linear_regression.py` & `nzpyida-0.9.3/nzpyida/analytics/tests/test_linear_regression.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,16 +54,16 @@
     assert not mm.model_exists(MOD_NAME)
     
     model.fit(idf_train, id_column="ID", target_column="B")
     assert mm.model_exists(MOD_NAME)
 
     pred = model.predict(idf_test, out_table=OUT_TABLE_PRED)
     assert pred
-    assert all(pred.columns == ['ID', 'B'])
-    assert any(round(x) == y for x, y in zip(list(pred.as_dataframe()['B'].values),  [1, 4, 2223, -999, 11112]))
+    assert all(pred.columns == idadb.to_def_case(['ID', 'B']))
+    assert any(round(x) == y for x, y in zip(list(pred.as_dataframe()[idadb.to_def_case('B')].values),  [1, 4, 2223, -999, 11112]))
 
     score = model.score(idf_test, target_column='B')
 
     assert score
     assert score < 0.001
 
     mse, mae, rse, rae = model.score_all(idf_test, target_column='B')
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/tests/test_model_manager.py` & `nzpyida-0.9.3/nzpyida/analytics/tests/test_model_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,29 +68,29 @@
     mm.alter_model(MOD_NAME_COPY, name=MOD_NAME, owner="INZAUSER", description="DecTree model",
                    copyright="Copyright (c) 2023. IBM Corp. All rights reserved.", category="DecTree")
     
     assert mm.model_exists(MOD_NAME)
 
     lm_ida = mm.list_models()
     lm = lm_ida.as_dataframe()
-    lm = lm[lm["MODELNAME"]==MOD_NAME]
+    lm = lm[lm[idadb.to_def_case("MODELNAME")]==idadb.to_def_case(MOD_NAME)]
     assert len(lm) == 1
-    assert lm["OWNER"].iloc[0] == "INZAUSER"
-    assert lm["DESCRIPTION"].iloc[0] == "DecTree model"
-    assert lm["COPYRIGHT"].iloc[0] == "Copyright (c) 2023. IBM Corp. All rights reserved."
-    assert lm["USERCATEGORY"].iloc[0] == "DecTree"
-    assert lm["CREATOR"].iloc[0] == "ADMIN"
-    assert lm["ALGORITHM"].iloc[0] == "Decision Tree"
+    assert lm[idadb.to_def_case("OWNER")].iloc[0] == idadb.to_def_case("INZAUSER")
+    assert lm[idadb.to_def_case("DESCRIPTION")].iloc[0] == "DecTree model"
+    assert lm[idadb.to_def_case("COPYRIGHT")].iloc[0] == "Copyright (c) 2023. IBM Corp. All rights reserved."
+    assert lm[idadb.to_def_case("USERCATEGORY")].iloc[0] == "DecTree"
+    assert lm[idadb.to_def_case("CREATOR")].iloc[0] == idadb.to_def_case("ADMIN")
+    assert lm[idadb.to_def_case("ALGORITHM")].iloc[0] == "Decision Tree"
 
     # test grant privileges
 
     mm.revoke_model(MOD_NAME, ["list", "update"], user=["INZAUSER"])
 
-    assert PRIVILEGES_OUTPUT1 in mm.list_privileges()
+    assert PRIVILEGES_OUTPUT1 in mm.list_privileges().upper()
 
     mm.grant_model(MOD_NAME, privilege=["list"], user=["INZAUSER"])
 
-    assert PRIVILEGES_OUTPUT2 in mm.list_privileges()
+    assert PRIVILEGES_OUTPUT2 in mm.list_privileges().upper()
 
-    assert PRIVILEGES_OUTPUT3 in mm.list_privileges(grant=True)
+    assert PRIVILEGES_OUTPUT3 in mm.list_privileges(grant=True).upper()
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/tests/test_naive_bayes.py` & `nzpyida-0.9.3/nzpyida/analytics/tests/test_naive_bayes.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,22 +54,22 @@
     assert not mm.model_exists(MOD_NAME)
     
     model.fit(idf_train, id_column="ID", target_column="B")
     assert mm.model_exists(MOD_NAME)
 
     pred = model.predict(idf_test, id_column="ID", out_table=OUT_TABLE_PRED)
     assert pred
-    assert all(pred.columns == ['ID', 'CLASS'])
-    assert list(pred.as_dataframe()['CLASS'].values) == ['p', 'n', 'n']
+    assert all(pred.columns == idadb.to_def_case(['ID', 'CLASS']))
+    assert list(pred.as_dataframe()[idadb.to_def_case('CLASS')].values) == ['p', 'n', 'n']
 
     score = model.score(idf_test, id_column="ID", target_column="B")
 
     assert score
     assert 0.67 >= score >= 0.66
 
     cm, acc, wacc = model.conf_matrix(idf_test, id_column='ID', target_column='B', out_matrix_table=OUT_TABLE_CM)
     assert all([cm, acc, wacc])
-    assert all(cm.columns == ['REAL', 'PREDICTION', 'CNT'])
+    assert all(cm.columns == idadb.to_def_case(['REAL', 'PREDICTION', 'CNT']))
     assert len(cm) >= 3
-    assert sum(cm.as_dataframe()["CNT"].values) == 3
+    assert sum(cm.as_dataframe()[idadb.to_def_case("CNT")].values) == 3
     assert wacc == 0.75
     assert 0.67 >= acc >= 0.66
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/tests/test_preparation.py` & `nzpyida-0.9.3/nzpyida/analytics/tests/test_preparation.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,19 +36,19 @@
     idf = idadb.as_idadataframe(df_train, tablename=TAB_NAME, clear_existing=True, indexer='ID')
     yield idf
     if idadb.exists_table(TAB_NAME):
         idadb.drop_table(TAB_NAME)
 
 def test_std_norm(idadb: IdaDataBase, clean_up, idf):
 
-    out_df = std_norm(idf, in_column=["A:S"], by_column=['B'], out_table=TAB_NAME_TEST)
+    out_df = std_norm(idf, in_column=['A:S'], by_column=['B'], out_table=TAB_NAME_TEST)
     assert out_df
     assert idadb.exists_table_or_view(TAB_NAME_TEST)
 
-    assert all(out_df.columns == ['B', 'ID', 'STD_A'])
+    assert all(out_df.columns == ['B', 'ID', 'std_A'])
 
     assert len(out_df) == len(idf)
 
 
 def test_random_sample(idadb: IdaDataBase, idf, clean_up):
     with AutoDeleteContext(idadb):
         sample_df = random_sample(idf, size=300, by_column=["B"], rand_seed=123)
@@ -76,9 +76,10 @@
     train_df, test_df = train_test_split(idf, TAB_NAME_TRAIN, TAB_NAME_TEST, fraction=0.8,
                                          id_column="ID")
     assert test_df
     assert test_df
     assert round(len(train_df)/len(idf), 1) == 0.8
     assert round(len(test_df)/len(idf), 1) == 0.2
 
-    assert not any(el in train_df['ID'].as_dataframe().values for el in test_df["ID"].as_dataframe().values)
+    train_pdf = train_df['ID'].as_dataframe()
+    assert not any(el in train_pdf.values for el in test_df["ID"].as_dataframe().values)
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/tests/test_regression_trees.py` & `nzpyida-0.9.3/nzpyida/analytics/tests/test_regression_trees.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     assert not mm.model_exists(MOD_NAME)
     
     model.fit(idf_train, id_column="ID", target_column="B", min_improve=0.001, min_split=200)
     assert mm.model_exists(MOD_NAME)
 
     pred = model.predict(idf_test, id_column="ID", out_table=OUT_TABLE_PRED)
     assert pred
-    assert all(pred.columns == ['ID', 'CLASS'])
+    assert all(pred.columns == idadb.to_def_case(['ID', 'CLASS']))
     # assert any(round(x) == y for x, y in zip(list(pred.as_dataframe()['CLASS'].values),  [1, 4, 2223, -999, 11112]))
 
     score = model.score(idf_test, id_column="ID", target_column="B")
 
     assert score
 
     mse, mae, rse, rae = model.score_all(idf_test, id_column='ID', target_column='B')
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/tests/test_timeseries.py` & `nzpyida-0.9.3/nzpyida/analytics/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/analytics/tests/test_two_step_clustering.py` & `nzpyida-0.9.3/nzpyida/analytics/tests/test_two_step_clustering.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,13 +54,13 @@
     
     model.fit(idf_train, distance='euclidean', max_k=5, bins=10, node_capacity=10, leaf_capacity=10,
               max_leaves=100, rand_seed=4321, out_table=OUT_TABLE_CLUST)
     assert mm.model_exists(MOD_NAME)
 
     pred = model.predict(idf_test, out_table=OUT_TABLE_PRED)
     assert pred
-    assert all(pred.columns == ['ID', 'CLUSTER_ID', 'DISTANCE'])
-    assert all(list(pred.head()['CLUSTER_ID'].values))
+    assert all(pred.columns == idadb.to_def_case(['ID', 'CLUSTER_ID', 'DISTANCE']))
+    assert all(list(pred.head()[idadb.to_def_case('CLUSTER_ID')].values))
 
     score = model.score(idf_test, target_column="A")
 
     assert score
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/transform/discretization.py` & `nzpyida-0.9.3/nzpyida/analytics/transform/discretization.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 information provided by the original attribute as possible. Data set discretization
 should preserve the relationship between the class and the discretized attributes
 if the data set is to be used for creation of a classification model.
 """
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.utils import map_to_props, materialize_df, make_temp_table_name
-from nzpyida.analytics.utils import get_auto_delete_context, call_proc_df_in_out
+from nzpyida.analytics.utils import get_auto_delete_context, call_proc_df_in_out, q
 from nzpyida.analytics.auto_delete_context import AutoDeleteContext
 
 
 class Discretization:
     """
     Generic class for handling data discretization.
     """
@@ -55,17 +55,17 @@
             the output table with dicretization bins
 
         Returns
         -------
         IdaDataFrame
             the data frame with discretization bins
         """
-        in_columns = ';'.join(['"' + x + '"' for x in in_df.columns])
+        in_columns = list(in_df.columns)
         params_dict = {
-            'incolumn': in_columns,
+            'incolumn': q(in_columns),
             'outtabletype': 'table'
         }
         params_dict.update(self.params)
 
         return call_proc_df_in_out(proc=self.proc, in_df=in_df, params=params_dict,
             out_table=out_table)[0]
 
@@ -272,15 +272,15 @@
 
         target : str
             the input table column containing a class label
         """
 
         super().__init__(idadb)
         self.proc = 'EMDISC'
-        self.params = {'target': target}
+        self.params = {'target': q(target)}
 
 def em_disc(in_df: IdaDataFrame, target: str, keep_org_values: bool=False, out_table: str=None):
     """
     Discretizes the given data frame based on minimizing entropy of the data 
     in the target column.
     This is a helper function that creates EMDisc class and then calls its fit() and
     apply() functions, returning the output from the latter.
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/transform/preparation.py` & `nzpyida-0.9.3/nzpyida/analytics/transform/preparation.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 This module contains function that can be used to prepare an input data
 frame for machine learning.
 """
 from typing import List, Tuple
 from nzpyida.frame import IdaDataFrame
 from nzpyida.analytics.utils import materialize_df, make_temp_table_name, \
-    get_auto_delete_context, call_proc_df_in_out, map_to_props
+    get_auto_delete_context, call_proc_df_in_out, map_to_props, q
 
 
 def std_norm(in_df: IdaDataFrame, in_column: List[str], id_column: str = None,
              by_column: str = None, out_table: str = None) -> IdaDataFrame:
     """
     Standardization and normalization transformations use the original continuous
     attribute a to generate a new continuous attribute a ' that has a different range
@@ -57,23 +57,23 @@
     Returns
     -------
     IdaDataFrame
         the data frame with requested transformations
     """
     if not id_column:
         if in_df.indexer:
-            id_column = in_df.indexer
+            id_column = q(in_df.indexer)
         else:
             raise TypeError('Missing id column - either use id_column attribute or set '
                             'indexer column in the input data frame')
 
     params = {
-        'id': id_column,
-        'incolumn': in_column,
-        'by': by_column
+        'id': q(id_column),
+        'incolumn': q(in_column),
+        'by': q(by_column)
     }
     return call_proc_df_in_out(proc='STD_NORM', in_df=in_df, params=params,
                                out_table=out_table, copy_indexer=True)[0]
 
 
 def impute_data(in_df: IdaDataFrame, in_column: str = None, method: str = None,
                 numeric_value: float = -1, nominal_value: str = 'missing', out_table: str = None) -> IdaDataFrame:
@@ -112,15 +112,15 @@
     Returns
     -------
     IdaDataFrame
         the data frame with requested transformations
     """
 
     params = {
-        'incolumn': in_column,
+        'incolumn': q(in_column),
         'method': method,
         'numericvalue': numeric_value,
         'nominalvalue': nominal_value
     }
     return call_proc_df_in_out(proc='IMPUTE_DATA', in_df=in_df, params=params,
                                out_table=out_table, copy_indexer=True)[0]
 
@@ -182,15 +182,15 @@
     IdaDataFrame
         the data frame with requested transformations
     """
 
     params = {
         'size': size,
         'fraction': fraction,
-        'by': by_column,
+        'by': q(by_column),
         'outsignature': out_signature,
         'randseed': rand_seed
     }
     return call_proc_df_in_out(proc='RANDOM_SAMPLE', in_df=in_df, params=params,
                                out_table=out_table, copy_indexer=True)[0]
 
 
@@ -230,15 +230,15 @@
     if not isinstance(in_df, IdaDataFrame):
         raise TypeError("Argument in_df should be an IdaDataFrame")
     
     if not id_column:
         if not in_df.indexer:
             raise ValueError("If dataframe has no indexer 'id_column' has to be provided")
         else:
-            id_column = in_df.indexer
+            id_column = q(in_df.indexer)
 
     if out_table_train and in_df._idadb.exists_table_or_view(out_table_train):
             in_df._idadb.drop_table(out_table_train)
     if out_table_test and in_df._idadb.exists_table_or_view(out_table_test):
             in_df._idadb.drop_table(out_table_test)
 
     temp_view_name, need_delete = materialize_df(in_df)
@@ -252,15 +252,15 @@
         auto_delete_context = get_auto_delete_context('out_table_test')
         out_table_test = make_temp_table_name()
 
     params = {
         'intable': temp_view_name,
         'traintable': out_table_train,
         'testtable': out_table_test,
-        'id': id_column,
+        'id': q(id_column),
         'fraction': fraction
     }
 
     if isinstance(rand_seed, float):
         params['seed'] = rand_seed
 
     params_s = map_to_props(params)
```

### Comparing `nzpyida-0.9.2/nzpyida/analytics/utils.py` & `nzpyida-0.9.3/nzpyida/analytics/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     bool
         should the object be dropped by the caller
     """
 
     if df.internal_state.views:
         temp_view_name = make_temp_table_name()
-        query = f'CREATE VIEW "{temp_view_name}" AS ({df.internal_state.get_state()})'
+        query = f'CREATE VIEW {temp_view_name} AS ({df.internal_state.get_state()})'
         df.ida_query(query, autocommit = True)
         return temp_view_name, True
     else:
         return df.tablename, False
 
 def make_temp_table_name(prefix: str='DATA_FRAME_') -> str:
     """
@@ -164,7 +164,34 @@
     for i in range(0, len(clean_str_split), 2):
         try:
             value = int(clean_str_split[i+1])
         except ValueError:
             value = clean_str_split[i+1]
         out_dict[clean_str_split[i].upper()] = [value]
     return  pd.DataFrame.from_dict(out_dict)
+
+def q(txt):
+    """
+    Quotes the given object. It supports the following types:
+    str - it will be quited, it it is not already quoted. Also strings in format A:B got quoting only for A part.
+    list - each item is quoted separately and the list is returned.
+    everything else - txt without modifications is returned
+
+    Parameters
+    ----------
+    txt
+        an object to quote
+
+    Returns
+    -------
+    Quited copy of the object
+    """
+    
+    if isinstance(txt, str) and (not txt.startswith('"') or not txt.endswith('"')):
+        if ':' in txt:
+            ix = txt.index(':')
+            return f'"{txt[:ix]}":{txt[ix+1:]}'
+        return f'"{txt}"'
+    elif isinstance(txt, list):
+        return [q(x) for x in txt]
+    else:
+        return txt
```

### Comparing `nzpyida-0.9.2/nzpyida/base.py` & `nzpyida-0.9.3/nzpyida/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #-----------------------------------------------------------------------------
-# Copyright (c) 2015, IBM Corp.
+# Copyright (c) 2015-2023, IBM Corp.
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
@@ -528,14 +528,15 @@
             #self.ida_query(query)
             #not anymore, reported problems with ODBC
             #better mention DB2GSE explicitly when accessing its functions
 
         # determine name of database
         if self._is_netezza_system():
             self._database_name = self.ida_scalar_query('select OBJNAME from _T_OBJECT where OBJID = CURRENT_DB;')
+            self._upper_cased = self.ida_scalar_query('select identifier_case;') == 'UPPERCASE'
         else:
             self._database_name = self.ida_scalar_query('select CURRENT_SERVER from SYSIBM.SYSDUMMY1')
 
         # Setting Autocommit and verbose environment variables
         set_autocommit(autocommit)
         set_verbose(verbose)
 
@@ -618,38 +619,33 @@
                 return cache
 
         where_part = ""
         if not show_all:
             where_part = ("AND TABSCHEMA = '%s' " % self.current_schema)
 
         if self._is_netezza_system():
-            query = ("SELECT SCHEMA as TABSCHEMA, TABLENAME as TABNAME, OWNER, 'T' as TYPE FROM _V_TABLE " +
-                     "WHERE DATABASE = '" + self._database_name + "' and OBJTYPE = 'TABLE' " + where_part +
-                     "UNION ALL " +
-                     "SELECT SCHEMA as TABSCHEMA, VIEWNAME as TABNAME, OWNER, 'V' as TYPE FROM _V_VIEW " +
-                     "WHERE DATABASE = '" + self._database_name + "' and OBJTYPE = 'VIEW' " + where_part)
             query = ("SELECT SCHEMA as TABSCHEMA, OBJNAME as TABNAME, OWNER, " +
-                             "CASE WHEN OBJTYPE = 'TABLE' THEN 'T' ELSE 'V' END AS TYPE " +
+                             "CASE WHEN UPPER(OBJTYPE) = 'TABLE' THEN 'T' ELSE 'V' END AS TYPE " +
                       "FROM _V_OBJECTS  " +
-                      "WHERE OBJTYPE in ('TABLE', 'VIEW') " + where_part +
+                      "WHERE UPPER(OBJTYPE) in ('TABLE', 'VIEW') " + where_part +
                       "ORDER BY TABSCHEMA, TABNAME")
         else:
             query = ("SELECT DISTINCT TABSCHEMA, TABNAME, OWNER, TYPE " +
                      "FROM SYSCAT.TABLES " +
                      "WHERE OWNERTYPE = 'U' " + where_part +
                      "ORDER BY TABSCHEMA, TABNAME")
 
         data = self.ida_query(query)
         
         # Workaround for some ODBC version which does not get the entire
         # string of the column name in the cursor descriptor. 
         # This is hardcoded, so be careful
         data.columns = ['TABSCHEMA', 'TABNAME', 'OWNER', 'TYPE']
         
-        data = self._upper_columns(data)
+        #data = self._upper_columns(data)
 
         # Db2 Warehouse FIX: schema "SAMPLES" and "GOSALES" saved with an extra blank,
         # By doing so, we delete the extra blank.
         # Note that this works because all cells are of type string.
 
         # OLD version, created an unexpected bug in some wrong ODBC version
         # TypeError: unorderable types: bytes() > int()
@@ -682,28 +678,28 @@
         0   DASHXXXXXX  KMEANS_10857_1434974511  DASHXXXXXX
         1   DASHXXXXXX  KMEANS_11726_1434977692  DASHXXXXXX
         2   DASHXXXXXX  KMEANS_11948_1434976568  DASHXXXXXX
         """
         if self._is_netezza_system():
             list_models_stmt = ("SELECT MODELNAME, OWNER, CREATED, STATE, MININGFUNCTION, ALGORITHM, USERCATEGORY " +
                                 "FROM INZA.V_NZA_MODELS")
-            result_columns =  ['modelname', 'owner', 'created', 'state','miningfunction', 'algorithm', 'usercategory']
+            #result_columns =  ['modelname', 'owner', 'created', 'state','miningfunction', 'algorithm', 'usercategory']
         else:
             list_models_stmt = "call IDAX.LIST_MODELS()"
             result_columns = ['modelschema', 'modelname', 'owner', 'created', 'state',
                               'miningfunction', 'algorithm', 'usercategory']
 
         data = self.ida_query(list_models_stmt)
 
-        data.columns = result_columns
+        #data.columns = result_columns
 
         # Workaround for some ODBC version which does not get the entire
         # string of the column name in the cursor descriptor. 
         # This is hardcoded, so be careful
-        data = self._upper_columns(data)
+        #data = self._upper_columns(data)
         return data
 
     def exists_table_or_view(self, objectname):
         """
         Check if a table or view exists in self.
 
         Parameters
@@ -814,15 +810,15 @@
         >>> idadb.exists_model("MODEL")
         True
         >>> idadb.exists_model("NOT_EXISTING")
         False
         >>> idadb.exists_model("NO_MODEL")
         TypeError : NO_MODEL exists but is not a model (of type '?')
         """
-        modelname = nzpyida.utils.check_modelname(modelname)
+        modelname = nzpyida.utils.check_modelname(modelname, self._upper_cased)
         if '.' in modelname:
             modelschema, modelname = modelname.split('.')
         else:
             modelschema = self.current_schema
 
         if self._is_netezza_system():
             # on Netezza the model schema part of the model name is ignored
@@ -964,23 +960,23 @@
         >>> idadb.is_model("MODEL")
         True
         >>> idadb.is_model("NO_MODEL")
         False
         >>> idadb.is_model("NOT_EXISTING")
         ValueError : NOT_EXISTING doesn't exist in database
         """
-        modelname = nzpyida.utils.check_modelname(modelname)
+        modelname = nzpyida.utils.check_modelname(modelname, self._upper_cased)
 
         if '.' in modelname:
             modelname_noschema = modelname.split('.')[-1]
         else:
             modelname_noschema = modelname
         data = self.show_models()
         if not data.empty:
-            if modelname_noschema in data['MODELNAME'].values:
+            if modelname_noschema in data[self.to_def_case('MODELNAME')].values:
                 return True
 
         # This part is executed if data is empty or model is not in data
         try:
             self.is_table_or_view(modelname)
         except:
             raise
@@ -1130,15 +1126,15 @@
         """
         if not isinstance(dataframe, pd.DataFrame):
             raise TypeError("Argument dataframe is not of type Pandas.DataFrame")
 
         if tablename is None:
                 tablename = self._get_valid_tablename(prefix="DATA_FRAME_")
 
-        tablename = nzpyida.utils.check_tablename(tablename)
+        tablename = nzpyida.utils.check_tablename(tablename, self._upper_cased)
 
         if primary_key is not None:
             if not isinstance(primary_key, six.string_types):
                 raise TypeError("The primary key argument should be a string")
             if primary_key not in dataframe.columns:
                 raise ValueError("The primary key should be the name of a column" +
                                  " in the given dataframe")
@@ -1319,15 +1315,15 @@
         -----
             Upper case characters and numbers, optionally separated by 
             underscores “_”, are valid characters.
         """
         # Actually we could support it for views too
         # Question : Is it better to accept an idadf as argument or rather the name of the table?
         oldname = idadf._name
-        newname = nzpyida.utils.check_tablename(newname)
+        newname = nzpyida.utils.check_tablename(newname, self._upper_cased)
 
         if self.is_table(idadf._name):
             if self._is_netezza_system():
                 query = "ALTER TABLE %s RENAME TO %s"%(idadf._name, newname)
             else:
                 query = "RENAME TABLE %s TO %s"%(idadf._name, newname)
             try:
@@ -1803,15 +1799,15 @@
         Check if an object of a certain type exists in Db2 Warehouse.
 
         Notes
         -----
         For more information, see exists_table_or_view, exists_table, 
         exists_view functions.
         """
-        objectname = nzpyida.utils.check_tablename(objectname)
+        objectname = nzpyida.utils.check_tablename(objectname, self._upper_cased)
 
         tablelist = self.show_tables(show_all=True)
         schema, name = self._get_name_and_schema(objectname)
         tablelist = tablelist[tablelist['TABSCHEMA'] == schema]
 
         if len(tablelist):
             if name in tablelist['TABNAME'].values:
@@ -1830,15 +1826,15 @@
         """
         Check if an existing object is of a certain type or in a list of types.
 
         Notes
         -----
         For more information, see is_table_or_view, is_table, is_view functions.
         """
-        objectname = nzpyida.utils.check_tablename(objectname)
+        objectname = nzpyida.utils.check_tablename(objectname, self._upper_cased)
 
         tablelist = self.show_tables(show_all=True)
         schema, name = self._get_name_and_schema(objectname)
         tablelist = tablelist[tablelist['TABSCHEMA'] == schema]
 
         if len(tablelist):
             if name in tablelist['TABNAME'].values:
@@ -1856,15 +1852,15 @@
         Admissible type values are "T" (table) and "V" (view)
 
         Notes
         -----
         For more information, seedrop_table and drop_view functions.
 
         """
-        objectname = nzpyida.utils.check_tablename(objectname)
+        objectname = nzpyida.utils.check_tablename(objectname, self._upper_cased)
 
         if object_type == "T":
             to_drop = "TABLE"
         elif object_type == "V":
             to_drop = "VIEW"
         else:
             raise ValueError("Unknown type to drop")
@@ -1968,15 +1964,15 @@
         >>> idadb._get_valid_tablename("MYDATA_")
         'MYDATA_65312_1434978215'
         >>> idadb._get_valid_tablename("mydata_")
         'MYDATA_78425_1434978215'
         >>> idadb._get_valid_tablename("mydata$")
         ValueError: Table name is not valid, only alphanumeric characters and underscores are allowed.
         """
-        prefix = nzpyida.utils.check_tablename(prefix)
+        prefix = nzpyida.utils.check_tablename(prefix, self._upper_cased)
         # We may assume that the generated name is unlikely to exist
         name = "%s%s_%s" % (prefix, random.randint(0, 100000), int(time()))
         return name
 
     def _get_valid_viewname(self, prefix="VIEW_"):
         """
         Convenience function : Alternative name for _get_valid_tablename.
@@ -2054,15 +2050,15 @@
             raise TypeError("_create_table is valid only for DataFrame objects")
 
         if primary_key is not None:
             if not isinstance(primary_key, six.string_types):
                 raise TypeError("primary_key argument should be a string")
 
         # Check the tablename
-        tablename = nzpyida.utils.check_tablename(tablename)
+        tablename = nzpyida.utils.check_tablename(tablename, self._upper_cased)
 
         # for Netezza we have to check if the schema exists already
         # otherwise we have to create it
         if self._is_netezza_system() & ("." in tablename):
             schemaname, tabname = tablename.split(".")
             if self.ida_scalar_query("SELECT COUNT(*) FROM _V_SCHEMA WHERE SCHEMA='%s'"%schemaname) == 0:
                 self.ida_query("CREATE SCHEMA " + schemaname)
@@ -2140,15 +2136,15 @@
         'IDAR_VIEW_4956'
         """
         if not isinstance(idadf, nzpyida.frame.IdaDataFrame):
             raise TypeError("_create_view is valid only for IdaDataFrame objects")
 
         # Check the viewname
         if viewname is not None:
-            viewname = nzpyida.utils.check_viewname(viewname)
+            viewname = nzpyida.utils.check_viewname(viewname, self._upper_cased)
         else:
             viewname = self._get_valid_viewname()
 
         self._prepare_and_execute("CREATE VIEW \"%s\" AS SELECT * FROM %s" % (viewname, idadf._name))
     
         # Save new view in cache
         if hasattr(self, "cache_show_tables"):
@@ -2181,15 +2177,15 @@
         TODO
         """
         if not isinstance(expression, six.string_types):
             raise TypeError("expression argument expected to be of string type")
 
         # Check the viewname
         if viewname is not None:
-            viewname = nzpyida.utils.check_viewname(viewname)
+            viewname = nzpyida.utils.check_viewname(viewname, self._upper_cased)
         else:
             viewname = self._get_valid_viewname()
 
         self._prepare_and_execute("CREATE VIEW \"%s\" AS %s" % (viewname, expression))
     
         # Save new view in cache
         if hasattr(self, "cache_show_tables"):
@@ -2215,15 +2211,15 @@
             If True, the INSERT statement is not printed. Avoids flooding the 
             console.
 
         """
         # TODO : Handle more datatypes
         if schema is None or schema.strip() == '':
             schema = self.current_schema
-        tablename = nzpyida.utils.check_tablename(tablename)
+        tablename = nzpyida.utils.check_tablename(tablename, self._upper_cased)
         column_string = '\"%s\"' % '\", \"'.join([str(x).strip() for x in dataframe.columns])
         row_string = ''
 
         # Save in a list columns that are booleans
         boolean_flaglist = []
         for column in dataframe.columns:
             if set(dataframe[column].unique()).issubset([True, False, 0, 1, np.nan]):
@@ -2324,15 +2320,15 @@
         >>> idadb._check_procedure('NOT_EXISTING')
         IdaDatabaseError: Function 'NOT_EXISTING' is not available.
         """
 
         if alg_name is None:
             alg_name = proc_name
         if self._is_netezza_system():
-            query = ("SELECT COUNT(*) FROM NZA.._V_PROCEDURE WHERE PROCEDURE='%s'") % proc_name
+            query = ("SELECT COUNT(*) FROM NZA.._V_PROCEDURE WHERE UPPER(PROCEDURE)='%s'") % proc_name
         else:
             query = ("SELECT COUNT(*) FROM SYSCAT.ROUTINES WHERE ROUTINENAME='%s" +
                      "' AND ROUTINEMODULENAME = 'IDAX'") % proc_name
         flag = self.ida_scalar_query(query)
 
         if int(flag) == False:
             raise IdaDataBaseError("Function '%s' is not available." % alg_name)
@@ -2460,8 +2456,20 @@
         nzpyida.utils._reset_attributes(self, attributes)
 
 
     def _is_netezza_system(self):
          """
          Checks if the underlying database system is Netezza.
          """
-         return self._database_system == 'netezza'
+         return self._database_system == 'netezza'
+
+    def to_def_case(self, text):
+        """
+        Converts the given object to the default case on this database.
+        The object can be a string or list of strings.
+        """
+        if isinstance(text, str):
+            return text.upper() if self._upper_cased else text.lower()
+        elif isinstance(text, list):
+            return [x.upper() if self._upper_cased else x.lower() for x in text]
+        else:
+            return text
```

### Comparing `nzpyida-0.9.2/nzpyida/exceptions.py` & `nzpyida-0.9.3/nzpyida/exceptions.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/feature_selection/__init__.py` & `nzpyida-0.9.3/nzpyida/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/feature_selection/chisquared.py` & `nzpyida-0.9.3/nzpyida/feature_selection/chisquared.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/feature_selection/entropy.py` & `nzpyida-0.9.3/nzpyida/feature_selection/entropy.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/feature_selection/gain_ratio.py` & `nzpyida-0.9.3/nzpyida/feature_selection/gain_ratio.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/feature_selection/gini.py` & `nzpyida-0.9.3/nzpyida/feature_selection/gini.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/feature_selection/info_gain.py` & `nzpyida-0.9.3/nzpyida/feature_selection/info_gain.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/feature_selection/private.py` & `nzpyida-0.9.3/nzpyida/feature_selection/private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/feature_selection/symmetric_uncertainty.py` & `nzpyida-0.9.3/nzpyida/feature_selection/symmetric_uncertainty.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/feature_selection/tstats.py` & `nzpyida-0.9.3/nzpyida/feature_selection/tstats.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/filtering.py` & `nzpyida-0.9.3/nzpyida/filtering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/frame.py` & `nzpyida-0.9.3/nzpyida/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #-----------------------------------------------------------------------------
-# Copyright (c) 2015, IBM Corp.
+# Copyright (c) 2015-2023, IBM Corp.
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
@@ -144,15 +144,15 @@
         >>> ida_iris = IdaDataFrame(idadb, "IRIS")
         """
         #TODO: Implement equality comparision between two IdaDataFrames
 
         if not idadb.__class__.__name__ == "IdaDataBase":
             idadb_class = idadb.__class__.__name__
             raise TypeError("Argument 'idadb' is of type %s, expected : IdaDataBase"%idadb_class)
-        tablename = nzpyida.utils.check_tablename(tablename)
+        tablename = nzpyida.utils.check_tablename(tablename, idadb._upper_cased)
 
         #idadb._reset_attributes("cache_show_tables")
 
         # TODO: Test what kind of error append when a table in use and cached
         # is suddently deleted
 
         if idadb.exists_table_or_view(tablename) is False:
@@ -1073,15 +1073,16 @@
                         order = " ORDER BY \"" + column + "\" ASC"
                     else:
                         order = ''
             data = self.ida_query("SELECT * FROM %s %s LIMIT %s "%(name, order, nrow))
 
             if data.shape[0] != 0:
                 if isinstance(self, nzpyida.IdaSeries):
-                    data = data[self.columns[0]]
+                    if not isinstance(data, pd.Series):
+                        data = data[self.column]
                 elif not 'SELECT ' in name:
                     columns = self.columns
                     data.columns = columns
 #                data = ibmdbpy.utils._convert_dtypes(self, data)
             return data
 
     # TODO : There is a warning in anaconda when there are missing values -> why ?
@@ -2291,22 +2292,22 @@
             """
             Decides if a column should be considered categorical or numerical
             """
             categorical_attributes = ['VARCHAR', 'CHARACTER VARYING', 'CHARACTER', 'VARGRAPHIC',
                                       'GRAPHIC', 'CLOB']
             numerical_attributes = ['SMALLINT', 'INTEGER', 'BIGINT', 'REAL',
                                     'DOUBLE', 'DOUBLE PRECISION', 'FLOAT', 'DECIMAL', 'NUMERIC']
-            if tup[0] in categorical_attributes:
+            if tup[0].upper() in categorical_attributes:
                 if factor_threshold is None:
                     return "CATEGORICAL"
                 elif tup[1] <= factor_threshold:
                     return "CATEGORICAL"
                 else:
                     return "STRING"
-            elif tup[0] in numerical_attributes:
+            elif tup[0].upper() in numerical_attributes:
                 if factor_threshold is None:
                     return "NUMERIC"
                 elif tup[1] > factor_threshold:
                     return "NUMERIC"
                 else:
                     return "CATEGORICAL"
             else:
@@ -2333,15 +2334,15 @@
         Examples
         --------
         >>> ida_iris._get_numerical_columns()
         ['sepal_length', 'sepal_width', 'petal_length', 'petal_width']
         """
         num = ['SMALLINT', 'INTEGER', 'BIGINT', 'REAL',
                             'DOUBLE', 'DOUBLE PRECISION', 'FLOAT', 'DECIMAL', 'NUMERIC']
-        return list(self.dtypes.loc[self.dtypes['TYPENAME'].isin(num)].index)
+        return list(self.dtypes.loc[self.dtypes['TYPENAME'].str.upper().isin(num)].index)
 
     def _get_categorical_columns(self):
         """
         Get the columns of self that are considered as categorical. Their data
         type in the database determines whether these columns are categorical.
         The following data types are considered categorical:
 
@@ -2354,15 +2355,15 @@
 
         Examples
         --------
         >>> ida_iris._get_categorical_columns()
         ['species']
         """
         cat = ['VARCHAR', 'CHARACTER', 'VARGRAPHIC', 'GRAPHIC', 'CLOB']
-        return list(self.dtypes.loc[self.dtypes['TYPENAME'].isin(cat)].index)
+        return list(self.dtypes.loc[self.dtypes['TYPENAME'].str.upper().isin(cat)].index)
 
     def _prepare_and_execute(self, query, autocommit = True, silent = False):
         """
         Prepare and execute a query.
 
         Parameters
         ----------
```

### Comparing `nzpyida-0.9.2/nzpyida/indexing.py` & `nzpyida-0.9.3/nzpyida/indexing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/internals.py` & `nzpyida-0.9.3/nzpyida/internals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #-----------------------------------------------------------------------------
-# Copyright (c) 2015, IBM Corp.
+# Copyright (c) 2015-2023, IBM Corp.
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
@@ -300,16 +300,16 @@
                     temp1 = ""
                 else:
                     order_by = ""
                     as_temp1 = "AS TEMP1"
                     temp1 = "TEMP1."
 
                 if self._idadf.indexer:
-                    query = ("SELECT " + columns + " FROM %s " + as_temp1 + " WHERE " +
-                             self._idadf.indexer + indexstring)
+                    query = ("SELECT " + columns + " FROM %s " + as_temp1 + " WHERE \"" +
+                             self._idadf.indexer + "\"" + indexstring)
                 else:
                     query = ("SELECT " + columns + " FROM (SELECT " + temp1 + "*, "+
                             "(ROW_NUMBER() OVER(" + order_by + ")-1) AS RN FROM %s " + as_temp1 + ") AS TEMP2 "+
                             "WHERE RN " + indexstring)
 
                 self.index = None
```

### Comparing `nzpyida-0.9.2/nzpyida/sampledata/__init__.py` & `nzpyida-0.9.3/nzpyida/sampledata/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/sampledata/iris.py` & `nzpyida-0.9.3/nzpyida/sampledata/iris.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/sampledata/iris.txt` & `nzpyida-0.9.3/nzpyida/sampledata/iris.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/sampledata/swiss.py` & `nzpyida-0.9.3/nzpyida/sampledata/swiss.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/sampledata/swiss.txt` & `nzpyida-0.9.3/nzpyida/sampledata/swiss.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/sampledata/titanic.py` & `nzpyida-0.9.3/nzpyida/sampledata/titanic.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/sampledata/titanic.txt` & `nzpyida-0.9.3/nzpyida/sampledata/titanic.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/series.py` & `nzpyida-0.9.3/nzpyida/series.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/sql.py` & `nzpyida-0.9.3/nzpyida/sql.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/statistics.py` & `nzpyida-0.9.3/nzpyida/statistics.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/tests/conftest.py` & `nzpyida-0.9.3/nzpyida/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,20 @@
         help="User ID")
     parser.addoption("--pwd", default='',
         help="Password")
     parser.addoption("--jdbc", default='',
         help="jdbc url string for JDBC connection")
     parser.addoption("--hostname", default='',
         help="hostname for nzpy connection")
+    parser.addoption("--esri", default='true',
+        help="is working on nzspatial_esri cartridge")
+
+@pytest.fixture(scope="session")
+def is_esri(request):
+    return True if request.config.getoption('--esri').lower() == 'true' else False
 
 def get_data(request):
     """
     Helper function that returns the dataset correponding to the table option
     (default, iris). Raise an error in case the dataset is not included in
     ibmdbpy or its name is unkown.
     """
```

### Comparing `nzpyida-0.9.2/nzpyida/tests/test_aggregation.py` & `nzpyida-0.9.3/nzpyida/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/tests/test_association_rules.py` & `nzpyida-0.9.3/nzpyida/tests/test_association_rules.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/tests/test_base.py` & `nzpyida-0.9.3/nzpyida/tests/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         df = idadb.show_models()
         assert isinstance(df, pandas.core.frame.DataFrame)
         if not df.empty:
             show_model_columns = ['MODELNAME', 'OWNER', 'CREATED', 'STATE',
                                   'MININGFUNCTION', 'ALGORITHM', 'USERCATEGORY']
             if not idadb._is_netezza_system():
                 show_model_columns =  ['MODELSCHEMA'] + show_model_columns
-            assert (list(df.columns) == show_model_columns)
+            assert (list(df.columns) == idadb.to_def_case(show_model_columns))
 
     def test_idadb_exists_table_or_view_positive0(self, idadb, idadf, idaview):
         assert(idadb.exists_table_or_view(idadf.name) == 1)
         assert(idadb.exists_table_or_view(idaview.name) == 1)
 
     @pytest.mark.skipif("'netezza' in config.getvalue('jdbc') or config.getvalue('hostname') != ''")
     def test_idadb_exists_table_or_view_positive(self, idadb, idadf, idaview, idageodf_county_view):
@@ -169,15 +169,15 @@
         with pytest.raises(ValueError):
             idadb.is_view("NOT_EXISTING_VIEW_130530496_4860385960")
 
     def test_idadb_is_model_positive(self, idadb, idadf_tmp):
         idadb.add_column_id(idadf_tmp, destructive = True)
         # Create a simple DecisionTreeClassifier model
         kmeans = DecisionTreeClassifier(idadb=idadb, model_name="Model_85584573777")
-        kmeans.fit(idadf_tmp, target_column='"species"')
+        kmeans.fit(idadf_tmp, target_column='species')
         assert(idadb.is_model(kmeans.model_name) == 1)
         try : idadb.drop_model(kmeans.model_name)
         except : pass
 
     def test_idadb_is_model_negative(self, idadb, idadf, idaview):
         assert(idadb.is_model(idadf.name) == 0)
         assert(idadb.is_model(idaview.name) == 0)
```

### Comparing `nzpyida-0.9.2/nzpyida/tests/test_base_connexion.py` & `nzpyida-0.9.3/nzpyida/tests/test_base_connexion.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/tests/test_base_private.py` & `nzpyida-0.9.3/nzpyida/tests/test_base_private.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #-----------------------------------------------------------------------------
-# Copyright (c) 2015, IBM Corp.
+# Copyright (c) 2015-2023, IBM Corp.
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
@@ -44,45 +44,45 @@
         tup = idadb._get_name_and_schema("TABLE")
         assert(tup[0] == idadb.current_schema)
         assert(tup[1] == "TABLE")
 
     def test_idadb_get_valid_tablename_default(self, idadb):
         tablename = idadb._get_valid_tablename()
         assert(isinstance(tablename, six.string_types))
-        assert("DATA_FRAME_" in tablename)
+        assert("DATA_FRAME_" in tablename.upper())
 
     def test_idadb_get_valid_tablename_custom(self, idadb):
         tablename = idadb._get_valid_tablename("MY_PERSONAL_PREFIX")
-        assert("MY_PERSONAL_PREFIX" in tablename)
+        assert("MY_PERSONAL_PREFIX" in tablename.upper())
 
     def test_idadb_get_valid_tablename_error(self, idadb):
         with pytest.raises(ValueError):
             idadb._get_valid_tablename("INCORRECT_PREFIX_ß%$")
 
     def test_idadb_get_valid_viewname_default(self, idadb):
         viewname = idadb._get_valid_viewname()
         assert(isinstance(viewname, six.string_types))
-        assert("VIEW_" in viewname)
+        assert("VIEW_" in viewname.upper())
 
     def test_idadb_get_valid_viewname_custom(self, idadb):
         viewname = idadb._get_valid_viewname("MY_PERSONAL_PREFIX")
-        assert("MY_PERSONAL_PREFIX" in viewname)
+        assert("MY_PERSONAL_PREFIX" in viewname.upper())
 
     def test_idadb_get_valid_viewname_error(self, idadb):
         with pytest.raises(ValueError):
             idadb._get_valid_viewname("INCORRECT_PREFIX_ß%$")
 
     def test_idadb_get_valid_modelname_default(self, idadb):
         modelname = idadb._get_valid_modelname()
         assert(isinstance(modelname, six.string_types))
-        assert("MODEL_" in modelname)
+        assert("MODEL_" in modelname.upper())
 
     def test_idadb_get_valid_modelname_custom(self, idadb):
         modelname = idadb._get_valid_modelname("MY_PERSONAL_PREFIX")
-        assert("MY_PERSONAL_PREFIX" in modelname)
+        assert("MY_PERSONAL_PREFIX" in modelname.upper())
 
     def test_idadb_get_valid_modelname_error(self, idadb):
         with pytest.raises(ValueError):
             idadb._get_valid_modelname("INCORRECT_PREFIX_ß%$")
 
     def test_idadb_create_table(self, idadb, df):
         try : idadb.drop_table("CREATE_TABLE_TEST_585960708904")
```

### Comparing `nzpyida-0.9.2/nzpyida/tests/test_base_table_manipulation.py` & `nzpyida-0.9.3/nzpyida/tests/test_base_table_manipulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         try:
             idadb.drop_table("TEST_RENAMED")
         except:
             pass
         original_name = idadf_tmp.tablename
         idadb.rename(idadf_tmp, "TEST_RENAMED")
         idadb.commit()
-        assert(idadf_tmp.name == "TEST_RENAMED")
+        assert(idadf_tmp.name.upper() == "TEST_RENAMED")
         assert(idadb.exists_table("TEST_RENAMED") == 1)
         assert(idadb.exists_table(original_name) == 0)
         idadb.rename(idadf_tmp, original_name)
 
     def test_idadb_rename_value_error(self, idadb, idadf):
         with pytest.raises(ValueError):
             idadb.rename(idadf, "T569ß4359**4\4%")
```

### Comparing `nzpyida-0.9.2/nzpyida/tests/test_feature_selection.py` & `nzpyida-0.9.3/nzpyida/tests/test_feature_selection.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/tests/test_filtering.py` & `nzpyida-0.9.3/nzpyida/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/tests/test_frame.py` & `nzpyida-0.9.3/nzpyida/tests/test_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #-----------------------------------------------------------------------------
-# Copyright (c) 2015, IBM Corp.
+# Copyright (c) 2015-2023, IBM Corp.
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
@@ -31,15 +31,14 @@
 class Test_OpenDataFrameObject(object):
 
     def test_idadf_attr_idadb(self, idadf):
         assert isinstance(idadf._idadb, IdaDataBase)
 
     def test_idadf_attr_name(self, idadf, df):
         assert isinstance(idadf.name, six.string_types)
-        assert idadf.name == idadf.schema + "." + "TEST_IBMDBPY"
         assert idadf.name == idadf.schema + "." + idadf.tablename
 
     def test_idadf_attr_schema(self, idadf):
         assert isinstance(idadf.schema, six.string_types)
 
     def test_idadf_attr_indexer(self, idadf):
         assert (isinstance(idadf.indexer, six.string_types)|(idadf.indexer is None))
```

### Comparing `nzpyida-0.9.2/nzpyida/tests/test_frame_connexion.py` & `nzpyida-0.9.3/nzpyida/tests/test_frame_connexion.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/tests/test_frame_private.py` & `nzpyida-0.9.3/nzpyida/tests/test_frame_private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/tests/test_indexing.py` & `nzpyida-0.9.3/nzpyida/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/tests/test_internals.py` & `nzpyida-0.9.3/nzpyida/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/tests/test_kmeans.py` & `nzpyida-0.9.3/nzpyida/tests/test_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/tests/test_naive_bayes.py` & `nzpyida-0.9.3/nzpyida/tests/test_naive_bayes.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/tests/test_series.py` & `nzpyida-0.9.3/nzpyida/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/tests/test_sorting.py` & `nzpyida-0.9.3/nzpyida/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/tests/test_statistics.py` & `nzpyida-0.9.3/nzpyida/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/tests/test_utils.py` & `nzpyida-0.9.3/nzpyida/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.2/nzpyida/utils.py` & `nzpyida-0.9.3/nzpyida/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #-----------------------------------------------------------------------------
-# Copyright (c) 2015, IBM Corp.
+# Copyright (c) 2015-2023, IBM Corp.
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
@@ -191,85 +191,85 @@
     df_out = deepcopy(df)
     while n > 0:
         df_2.columns = ["%s_extended_%s"%(column,n) for column in df.columns]
         df_out = pd.concat([df_out,df_2], axis = 1)
         n -= 1
     return df_out
 
-def check_tablename(tablename):
+def check_tablename(tablename, default_upper=True):
     """
-    Check if a string is upper case. This function converts the string to upper 
-    case and checks if it is a valid table name.
+    This function converts the string to the given case.
 
     Parameters
     ----------
     tablename : str
         string to be checked. 
 
+    default_upper : bool
+        should make the sting uppercese or lowercase
+
     Returns
     -------
     str
         Checked and upper cased table name.
 
     Notes
     -----
         Table names should consist of upper case characters or numbers that can
         be separated by underscores (“_”) characters.
     """
-    return _check_database_objectname(tablename, 'Table')
+    return _check_database_objectname(tablename, 'Table', default_upper)
 
-def check_viewname(viewname):
+def check_viewname(viewname, default_upper=True):
     """
     Convenience function for checking view names, which have the same prerequisites as table names.
     See the check_tablename documentation.
     """
-    return _check_database_objectname(viewname, 'View')
+    return _check_database_objectname(viewname, 'View', default_upper)
 
-def check_modelname(modelname):
+def check_modelname(modelname, default_upper=True):
     """
     Convenience function for checking model names, which have the same prerequisites as table names.
     See the check_tablename documentation.
     """
-    return _check_database_objectname(modelname, 'Model')
+    return _check_database_objectname(modelname, 'Model', default_upper)
 
 
-def _check_case(name):
+def _check_case(name, default_upper=True):
     """
-    Check if the name given as parameter is in upper case and convert it to 
-    upper cases.
+    Conerts case of the given text to upper case (if default_upper is set) or lower case.
     """
-    if name != name.upper():
-        warnings.warn("Mixed case names are not supported in database object names.", UserWarning)
-    return name.upper()
+    return name.upper() if default_upper else name.lower() 
 
 
-def _check_database_objectname(tablename, objecttype):
+def _check_database_objectname(tablename, objecttype, default_upper=True):
     """
-    Check if a string is upper case. This function converts the string to upper
-    case and checks if it is a valid database object (table, view or model) name.
+    Check if a string has the right case. This function converts the string to the upper
+    case if default_upper is set, and lower otherwise. It also checks if it is a valid 
+    database object (table, view or model) name.
 
     Parameters
     ----------
     tablename : str
         string to be checked.
 
     objecttype : str
             ''
 
     Returns
     -------
     str
-        Checked and upper cased database object name.
+        Checked and upper/lower cased database object name.
 
     Notes
     -----
         Database object names should consist of upper case characters or numbers that can
         be separated by underscores (“_”) characters.
     """
-    tablename = _check_case(tablename)
+    tablename = _check_case(tablename, default_upper)
     if not all([(char.isalnum() | (char == '_') | (char == '.')) for char in tablename]):
         raise ValueError("%s name '%s' is not valid, only alphanumeric characters and underscores are allowed."%(objecttype, tablename))
     if tablename.count(".") > 1:
         raise ValueError("%s name '%s' is not valid, only one '.' character is allowed."%(objecttype, tablename))
     return tablename
```

### Comparing `nzpyida-0.9.2/nzpyida.egg-info/PKG-INFO` & `nzpyida-0.9.3/nzpyida.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nzpyida
-Version: 0.9.2
+Version: 0.9.3
 Summary: Supports Custom ML/Analytics Execution Inside Netezza
 Home-page: https://github.com/ibm/nzpyida
 Author: IBM Corp.
 Author-email: mlabenski@ibm.com,pawel.mroz1@ibm.com
 License: BSD
 Project-URL: Documentation, https://nzpyida.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/IBM/nzpyida
```

### Comparing `nzpyida-0.9.2/nzpyida.egg-info/SOURCES.txt` & `nzpyida-0.9.3/nzpyida.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 docs/make.bat
 docs/requirements.txt
 docs/source/analytics.rst
 docs/source/base.rst
 docs/source/conf.py
 docs/source/exploration.rst
 docs/source/frame.rst
-docs/source/geoFrame.rst
-docs/source/geoSeries.rst
+docs/source/geo_frame.rst
+docs/source/geo_series.rst
 docs/source/geospatial.rst
 docs/source/ibm.png
 docs/source/index.rst
 docs/source/install.rst
 docs/source/kc.ico
 docs/source/legal.rst
 docs/source/predictive.rst
@@ -28,14 +28,16 @@
 docs/source/utils.rst
 nzpyida/__init__.py
 nzpyida/aggregation.py
 nzpyida/base.py
 nzpyida/exceptions.py
 nzpyida/filtering.py
 nzpyida/frame.py
+nzpyida/geo_frame.py
+nzpyida/geo_series.py
 nzpyida/indexing.py
 nzpyida/internals.py
 nzpyida/series.py
 nzpyida/sql.py
 nzpyida/statistics.py
 nzpyida/utils.py
 nzpyida.egg-info/PKG-INFO
@@ -128,16 +130,16 @@
 nzpyida/tests/test_base_private.py
 nzpyida/tests/test_base_table_manipulation.py
 nzpyida/tests/test_feature_selection.py
 nzpyida/tests/test_filtering.py
 nzpyida/tests/test_frame.py
 nzpyida/tests/test_frame_connexion.py
 nzpyida/tests/test_frame_private.py
-nzpyida/tests/test_geoFrame.py
-nzpyida/tests/test_geoSeries.py
+nzpyida/tests/test_geo_frame.py
+nzpyida/tests/test_geo_series.py
 nzpyida/tests/test_indexing.py
 nzpyida/tests/test_internals.py
 nzpyida/tests/test_kmeans.py
 nzpyida/tests/test_naive_bayes.py
 nzpyida/tests/test_series.py
 nzpyida/tests/test_sorting.py
 nzpyida/tests/test_statistics.py
```

### Comparing `nzpyida-0.9.2/setup.py` & `nzpyida-0.9.3/setup.py`

 * *Files identical despite different names*

