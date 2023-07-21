# Comparing `tmp/OpenFisca-Survey-Manager-1.1.2.tar.gz` & `tmp/OpenFisca-Survey-Manager-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFisca-Survey-Manager-1.1.2.tar", last modified: Thu Jul 20 14:42:07 2023, max compression
+gzip compressed data, was "OpenFisca-Survey-Manager-1.1.3.tar", last modified: Fri Jul 21 15:57:16 2023, max compression
```

## Comparing `OpenFisca-Survey-Manager-1.1.2.tar` & `OpenFisca-Survey-Manager-1.1.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:42:07.648917 OpenFisca-Survey-Manager-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)    18399 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    34499 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/LICENSE.AGPL.txt
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:42:07.640916 OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14346 2023-07-20 14:42:07.000000 OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2469 2023-07-20 14:42:07.000000 OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 14:42:07.000000 OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-20 14:42:07.000000 OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 14:42:07.000000 OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      759 2023-07-20 14:42:07.000000 OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-20 14:42:07.000000 OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    14346 2023-07-20 14:42:07.648917 OpenFisca-Survey-Manager-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13432 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:42:07.644916 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/
--rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17292 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/aggregates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:42:07.648917 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/
--rw-r--r--   0 runner    (1001) docker     (122)     3551 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv
--rw-r--r--   0 runner    (1001) docker     (122)      451 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_divisions.csv
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv
--rw-r--r--   0 runner    (1001) docker     (122)    12096 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv
--rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv
--rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)     9929 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/calmar.py
--rw-r--r--   0 runner    (1001) docker     (122)     3150 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/coicop.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/google_colab.py
--rw-r--r--   0 runner    (1001) docker     (122)    13357 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/input_dataframe_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)     4591 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/matching.py
--rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/read_dbf.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/read_sas.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/read_spss.py
--rw-r--r--   0 runner    (1001) docker     (122)    79765 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:42:07.648917 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    10047 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/scripts/build_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)    11312 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/statshelpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/survey_collections.py
--rw-r--r--   0 runner    (1001) docker     (122)    10119 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/surveys.py
--rw-r--r--   0 runner    (1001) docker     (122)     9552 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/temporary.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:42:07.648917 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:42:07.648917 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/data_files/
--rw-r--r--   0 runner    (1001) docker     (122)      381 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/data_files/config_template.ini
--rw-r--r--   0 runner    (1001) docker     (122)     3591 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_add_survey_to_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_calmar.py
--rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py
--rw-r--r--   0 runner    (1001) docker     (122)     5223 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_legislation_inflator.py
--rw-r--r--   0 runner    (1001) docker     (122)      989 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_marginal_tax_rate.py
--rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_matching.py
--rw-r--r--   0 runner    (1001) docker     (122)     4373 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_quantile.py
--rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_read_sas.py
--rw-r--r--   0 runner    (1001) docker     (122)    13724 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_summarize_variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_surveys.py
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_top_bottom_share.py
--rw-r--r--   0 runner    (1001) docker     (122)    10433 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-20 14:42:07.652917 OpenFisca-Survey-Manager-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3403 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:57:16.896867 OpenFisca-Survey-Manager-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    18571 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)    34499 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/LICENSE.AGPL.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:57:16.888867 OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14346 2023-07-21 15:57:16.000000 OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2469 2023-07-21 15:57:16.000000 OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 15:57:16.000000 OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-21 15:57:16.000000 OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 15:57:16.000000 OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      759 2023-07-21 15:57:16.000000 OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-21 15:57:16.000000 OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    14346 2023-07-21 15:57:16.896867 OpenFisca-Survey-Manager-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13432 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:57:16.892867 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/
+-rw-r--r--   0 runner    (1001) docker     (122)     2223 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17292 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/aggregates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:57:16.892867 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/
+-rw-r--r--   0 runner    (1001) docker     (122)     3551 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/nomenclature_coicop_source_by_divisions.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    12096 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9929 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/calmar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3147 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/coicop.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/google_colab.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13337 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/input_dataframe_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4606 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/read_dbf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/read_sas.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/read_spss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    79765 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:57:16.892867 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10027 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/scripts/build_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11312 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/statshelpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/survey_collections.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10119 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/surveys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9552 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/temporary.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:57:16.896867 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:57:16.896867 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/data_files/
+-rw-r--r--   0 runner    (1001) docker     (122)      381 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/data_files/config_template.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     3539 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_add_survey_to_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_calmar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5223 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_legislation_inflator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      989 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_marginal_tax_rate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4373 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (122)      792 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_read_sas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13736 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_summarize_variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_surveys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_top_bottom_share.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10433 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-21 15:57:16.896867 OpenFisca-Survey-Manager-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3403 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/setup.py
```

### Comparing `OpenFisca-Survey-Manager-1.1.2/CHANGELOG.md` & `OpenFisca-Survey-Manager-1.1.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 ﻿# Changelog
 
+### 1.1.3 [#263](https://github.com/openfisca/openfisca-survey-manager/pull/263)
+
+* Technical changes
+- Use importlib instead of pkg_resources to avoid deprecation warnings
+
 ### 1.1.2 [#262](https://github.com/openfisca/openfisca-survey-manager/pull/262)
 
 * Technical changes
   - Remove old `CircleCI` continuous integration configuration
   - Set `README` CI badge to current `GitHub Actions` CI
 
 ### 1.1.1 [#261](https://github.com/openfisca/openfisca-survey-manager/pull/261)
 
 * Technical changes
-  - Fix `Conda build` step in `publish-to-conda` GitHub Actions job  
+  - Fix `Conda build` step in `publish-to-conda` GitHub Actions job
     - Define `OpenFisca-Survey-Manager` package dependencies once for `PyPI` and `conda`
       - Use `setup.py` general requirement and extra requirements for `conda` package
       - Adapt `tables` library name to `pytables` for `conda`
   - Build `conda` package from repository sources instead of `PyPI` .tar.gz
 
 ## 1.1.0 [#260](https://github.com/openfisca/openfisca-survey-manager/pull/260)
```

### Comparing `OpenFisca-Survey-Manager-1.1.2/LICENSE.AGPL.txt` & `OpenFisca-Survey-Manager-1.1.3/LICENSE.AGPL.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/PKG-INFO` & `OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Survey-Manager
-Version: 1.1.2
+Version: 1.1.3
 Summary: A tool for managing survey/administrative data.
 Home-page: https://github.com/openfisca/openfisca-survey-manager
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: survey data
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/SOURCES.txt` & `OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/requires.txt` & `OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/PKG-INFO` & `OpenFisca-Survey-Manager-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Survey-Manager
-Version: 1.1.2
+Version: 1.1.3
 Summary: A tool for managing survey/administrative data.
 Home-page: https://github.com/openfisca/openfisca-survey-manager
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: survey data
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-Survey-Manager-1.1.2/README.md` & `OpenFisca-Survey-Manager-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/__init__.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,54 @@
+import importlib
 import logging
 import os
-import pkg_resources
-
+from pathlib import Path
 
 log = logging.getLogger(__name__)
 
+
+openfisca_survey_manager_location = Path(
+    importlib.metadata.distribution('openfisca-survey-manager').files[0]
+    ).parent
+
 # Hack for use at the CASD (shared user)
 # Use taxipp/.config/ directory if exists as default_config_files_directory
 try:
-    taxipp_location = pkg_resources.get_distribution('taxipp').location
+    taxipp_location = importlib.metadata.distribution('taxipp').files[0]
     default_config_files_directory = os.path.join(taxipp_location, '.config', 'openfisca-survey-manager')
-except pkg_resources.DistributionNotFound:
+except importlib.metadata.PackageNotFoundError:
     taxipp_location = None
 
 if taxipp_location is None or not os.path.exists(default_config_files_directory):
     default_config_files_directory = None
 
 
 # Hack for uising with france-data on a CI or locally
 try:
-    france_data_location = pkg_resources.get_distribution('openfisca-france_data').location
+    france_data_location = importlib.metadata.distribution('openfisca-france_data').files[0]
     from xdg import BaseDirectory
     default_config_files_directory = BaseDirectory.save_config_path('openfisca-survey-manager')
-except pkg_resources.DistributionNotFound:
+except importlib.metadata.PackageNotFoundError:
     france_data_location = None
 
 if france_data_location is None or not os.path.exists(default_config_files_directory):
     default_config_files_directory = None
 
 # Run CI when testing openfisca-survey-manager for example GitHub Actions
 test_config_files_directory = os.path.join(
-    pkg_resources.get_distribution('openfisca-survey-manager').location,
+    openfisca_survey_manager_location,
     'openfisca_survey_manager',
     'tests',
     'data_files',
     )
 
 with open(os.path.join(test_config_files_directory, 'config_template.ini')) as file:
     config_ini = file.read()
 
-config_ini = config_ini.format(location = pkg_resources.get_distribution('openfisca-survey-manager').location)
+config_ini = config_ini.format(location = openfisca_survey_manager_location)
 with open(os.path.join(test_config_files_directory, 'config.ini'), "w+") as file:
     file.write(config_ini)
 
 # GitHub Actions test
 is_in_ci = 'CI' in os.environ
 
 if is_in_ci and default_config_files_directory is None:
```

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/aggregates.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/calibration.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/calibration.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/calmar.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/calmar.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/coicop.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/coicop.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 import os
 import pandas as pd
-import pkg_resources
+import importlib
 
 
 log = logging.getLogger(__name__)
 
 
 legislation_directory = os.path.join(
-    pkg_resources.get_distribution('openfisca_survey_manager').location,
+    importlib.metadata.distribution('openfisca_survey_manager').files[0],
     'openfisca_survey_manager',
     'assets',
     )
 
 
 sub_levels = ['divisions', 'groupes', 'classes', 'sous_classes', 'postes']
 divisions = ['0{}'.format(i) for i in range(1, 10)] + ['11', '12']
```

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/config.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/config.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/google_colab.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/google_colab.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/input_dataframe_generator.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/input_dataframe_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,21 +4,20 @@
 import logging
 import os
 import random
 
 
 import numpy as np
 import pandas as pd
-import pkg_resources
 
 
 from openfisca_core import periods
 from openfisca_survey_manager.survey_collections import SurveyCollection
 from openfisca_survey_manager.surveys import Survey
-from openfisca_survey_manager import default_config_files_directory
+from openfisca_survey_manager import default_config_files_directory, openfisca_survey_manager_location
 
 
 log = logging.getLogger(__name__)
 
 
 def make_input_dataframe_by_entity(tax_benefit_system, nb_persons, nb_groups):
     """Generate a dictionnary of dataframes containing nb_persons persons spread in nb_groups groups.
@@ -191,15 +190,15 @@
         survey_collection = SurveyCollection.load(collection = collection, config_files_directory=config_files_directory)
     except configparser.NoOptionError as e:
         log.warning(f"set_table_in_survey configparser.NoOptionError : {e}")
         survey_collection = SurveyCollection(name = collection)
     except configparser.NoSectionError as e:  # For tests
         log.warning(f"set_table_in_survey configparser.NoSectionError : {e}")
         data_dir = os.path.join(
-            pkg_resources.get_distribution('openfisca-survey-manager').location,
+            openfisca_survey_manager_location,
             'openfisca_survey_manager',
             'tests',
             'data_files',
             )
         survey_collection = SurveyCollection(
             name = collection,
             config_files_directory = data_dir,
```

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/matching.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/matching.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-
-
 import logging
 import os
-import pkg_resources
-
 import pandas as pd
 
 
+from openfisca_survey_manager import openfisca_survey_manager_location
+
 log = logging.getLogger(__name__)
 
+
 config_files_directory = os.path.join(
-    pkg_resources.get_distribution('openfisca-survey-manager').location)
+    openfisca_survey_manager_location)
 
 
 def nnd_hotdeck_using_feather(receiver = None, donor = None, matching_variables = None, z_variables = None):
     """
     Not working
     """
     import feather
```

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/read_dbf.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/read_dbf.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/read_sas.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/read_sas.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/scenarios.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/scenarios.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/scripts/build_collection.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/scripts/build_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,21 @@
 
 import argparse
 import configparser
 import datetime
 import logging
 import os
 import pdb
-import pkg_resources
 import shutil
 import sys
 
 
 from openfisca_survey_manager.survey_collections import SurveyCollection
 from openfisca_survey_manager.surveys import Survey
-from openfisca_survey_manager import default_config_files_directory
+from openfisca_survey_manager import default_config_files_directory, openfisca_survey_manager_location
 
 app_name = os.path.splitext(os.path.basename(__file__))[0]
 log = logging.getLogger(app_name)
 
 
 def add_survey_to_collection(survey_name = None, survey_collection = None, sas_files = None, stata_files = None, csv_files = None):
     if sas_files is None:
@@ -154,15 +153,15 @@
         if config_files_do_not_exist:
             if templates_config_files_do_not_exist:
                 log.info("Creating configuration template files in {}".format(config_files_directory))
                 template_files = [
                     'raw_data_template.ini', 'config_template.ini'
                     ]
                 templates_config_files_directory = os.path.join(
-                    pkg_resources.get_distribution('openfisca-survey-manager').location,
+                    openfisca_survey_manager_location,
                     'openfisca_survey_manager',
                     'config_files_templates'
                     )
                 for template_file in template_files:
                     shutil.copy(
                         os.path.join(templates_config_files_directory, template_file),
                         os.path.join(config_files_directory, template_file),
```

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/statshelpers.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/statshelpers.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/survey_collections.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/survey_collections.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/surveys.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/surveys.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tables.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/temporary.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/temporary.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_add_survey_to_collection.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_add_survey_to_collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-
-
 import os
-import pkg_resources
 import pandas as pd
 import pytest
 
+
+from openfisca_survey_manager import openfisca_survey_manager_location
 from openfisca_survey_manager.survey_collections import SurveyCollection
 from openfisca_survey_manager.scripts.build_collection import add_survey_to_collection
 from openfisca_survey_manager.input_dataframe_generator import set_table_in_survey
 
+
 # GitLab Runner and GitHub Actions have env variable "CI" set by default
 is_in_ci = 'CI' in os.environ
 
 
 def test_add_survey_to_collection():
     # if is_in_ci:
     #     return
     name = 'fake'
     survey_name = 'fake_survey'
     data_dir = os.path.join(
-        pkg_resources.get_distribution('openfisca-survey-manager').location,
+        openfisca_survey_manager_location,
         'openfisca_survey_manager',
         'tests',
         'data_files',
         )
     survey_collection = SurveyCollection(name = name)
     saved_fake_survey_file_path = os.path.join(data_dir, 'help.sas7bdat')
     add_survey_to_collection(
@@ -37,15 +37,15 @@
 
 
 @pytest.mark.order(after="test_surveys.py::test_survey")
 def test_set_table_in_survey_first_year():
     # if is_in_ci:
     #     return
     data_dir = os.path.join(
-        pkg_resources.get_distribution('openfisca-survey-manager').location,
+        openfisca_survey_manager_location,
         'openfisca_survey_manager/tests/data_files',
         )
     input_dataframe = pd.DataFrame({"rfr": [1_000, 2_000, 100_000]})
     survey_name = 'test_set_table_in_survey_2020'
     collection = "fake"
     set_table_in_survey(input_dataframe, entity="foyer", period="2020", collection = collection, survey_name = survey_name, config_files_directory=data_dir)
 
@@ -61,15 +61,15 @@
 
 
 @pytest.mark.order(after="test_set_table_in_survey_first_year")
 def test_set_table_in_survey_second_year():
     # if is_in_ci:
     #     return
     data_dir = os.path.join(
-        pkg_resources.get_distribution('openfisca-survey-manager').location,
+        openfisca_survey_manager_location,
         'openfisca_survey_manager/tests/data_files',
         )
     input_dataframe = pd.DataFrame({"rfr": [1_021, 2_021, 100_021]})
     survey_name = 'test_set_table_in_survey_2021'
     collection = "fake"
     set_table_in_survey(input_dataframe, entity="foyer", period="2021", collection = collection, survey_name = survey_name, config_files_directory=data_dir)
```

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_calmar.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_calmar.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_legislation_inflator.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_legislation_inflator.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_marginal_tax_rate.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_marginal_tax_rate.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_matching.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_quantile.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_quantile.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_scenario.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_scenario.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-
 import shutil
-
-
 import logging
 import os
-import pkg_resources
 
 
 from openfisca_core.model_api import *  # noqa analysis:ignore
 from openfisca_core import periods
 from openfisca_core.tools import assert_near
 
 from openfisca_country_template import CountryTaxBenefitSystem
 
-
+from openfisca_survey_manager import openfisca_survey_manager_location
 from openfisca_survey_manager.input_dataframe_generator import (
     make_input_dataframe_by_entity,
     random_data_generator,
     randomly_init_variable,
     )
 from openfisca_survey_manager.scenarios import AbstractSurveyScenario
 
@@ -262,15 +258,15 @@
         simulation.calculate('rent', period) == input_data_frame_by_entity['household']['rent']
         ).all()
 
 
 def test_dump_survey_scenario():
     survey_scenario = create_randomly_initialized_survey_scenario()
     directory = os.path.join(
-        pkg_resources.get_distribution('openfisca-survey-manager').location,
+        openfisca_survey_manager_location,
         'openfisca_survey_manager',
         'tests',
         'data_files',
         'dump',
         )
     if os.path.exists(directory):
         shutil.rmtree(directory)
```

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_summarize_variables.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_summarize_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_surveys.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_surveys.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-
 import os
-import pkg_resources
 
 
+from openfisca_survey_manager import openfisca_survey_manager_location
 from openfisca_survey_manager.survey_collections import SurveyCollection
 from openfisca_survey_manager.surveys import Survey
 
 
 def test_survey():
     name = 'fake'
     data_dir = os.path.join(
-        pkg_resources.get_distribution('openfisca-survey-manager').location,
+        openfisca_survey_manager_location,
         'openfisca_survey_manager',
         'tests',
         'data_files',
         )
 
     survey_collection = SurveyCollection(
         name = name,
@@ -34,15 +33,15 @@
     survey.fill_hdf(source_format = 'sas')
 
 
 def test_survey_load():
     survey_name = 'test_set_table_in_survey_2021'
     collection = 'fake'
     data_dir = os.path.join(
-        pkg_resources.get_distribution('openfisca-survey-manager').location,
+        openfisca_survey_manager_location,
         'openfisca_survey_manager',
         'tests',
         'data_files',
         )
     survey_collection = SurveyCollection.load(
         collection=collection, config_files_directory=data_dir
         )
```

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/utils.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/utils.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/variables.py` & `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/setup.cfg` & `OpenFisca-Survey-Manager-1.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.2/setup.py` & `OpenFisca-Survey-Manager-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 
 doc_lines = __doc__.split('\n')
 
 
 setup(
     name = 'OpenFisca-Survey-Manager',
-    version = '1.1.2',
+    version = '1.1.3',
     author = 'OpenFisca Team',
     author_email = 'contact@openfisca.fr',
     classifiers = [classifier for classifier in classifiers.split('\n') if classifier],
     description = doc_lines[0],
     keywords = 'survey data',
     license = 'http://www.fsf.org/licensing/licenses/agpl-3.0.html',
     license_files = ("LICENSE.AGPL.txt",),
```

