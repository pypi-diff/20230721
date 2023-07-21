# Comparing `tmp/OpenFisca-Survey-Manager-1.1.3.tar.gz` & `tmp/OpenFisca-Survey-Manager-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFisca-Survey-Manager-1.1.3.tar", last modified: Fri Jul 21 15:57:16 2023, max compression
+gzip compressed data, was "OpenFisca-Survey-Manager-1.1.4.tar", last modified: Fri Jul 21 17:47:02 2023, max compression
```

## Comparing `OpenFisca-Survey-Manager-1.1.3.tar` & `OpenFisca-Survey-Manager-1.1.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:57:16.896867 OpenFisca-Survey-Manager-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (122)    18571 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    34499 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/LICENSE.AGPL.txt
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:57:16.888867 OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14346 2023-07-21 15:57:16.000000 OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2469 2023-07-21 15:57:16.000000 OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 15:57:16.000000 OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-21 15:57:16.000000 OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 15:57:16.000000 OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      759 2023-07-21 15:57:16.000000 OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-21 15:57:16.000000 OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    14346 2023-07-21 15:57:16.896867 OpenFisca-Survey-Manager-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13432 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:57:16.892867 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/
--rw-r--r--   0 runner    (1001) docker     (122)     2223 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17292 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/aggregates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:57:16.892867 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/
--rw-r--r--   0 runner    (1001) docker     (122)     3551 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv
--rw-r--r--   0 runner    (1001) docker     (122)      451 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/nomenclature_coicop_source_by_divisions.csv
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv
--rw-r--r--   0 runner    (1001) docker     (122)    12096 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv
--rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv
--rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)     9929 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/calmar.py
--rw-r--r--   0 runner    (1001) docker     (122)     3147 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/coicop.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/google_colab.py
--rw-r--r--   0 runner    (1001) docker     (122)    13337 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/input_dataframe_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)     4606 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/matching.py
--rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/read_dbf.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/read_sas.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/read_spss.py
--rw-r--r--   0 runner    (1001) docker     (122)    79765 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:57:16.892867 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    10027 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/scripts/build_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)    11312 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/statshelpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/survey_collections.py
--rw-r--r--   0 runner    (1001) docker     (122)    10119 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/surveys.py
--rw-r--r--   0 runner    (1001) docker     (122)     9552 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/temporary.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:57:16.896867 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:57:16.896867 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/data_files/
--rw-r--r--   0 runner    (1001) docker     (122)      381 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/data_files/config_template.ini
--rw-r--r--   0 runner    (1001) docker     (122)     3539 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_add_survey_to_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_calmar.py
--rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py
--rw-r--r--   0 runner    (1001) docker     (122)     5223 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_legislation_inflator.py
--rw-r--r--   0 runner    (1001) docker     (122)      989 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_marginal_tax_rate.py
--rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_matching.py
--rw-r--r--   0 runner    (1001) docker     (122)     4373 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_quantile.py
--rw-r--r--   0 runner    (1001) docker     (122)      792 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_read_sas.py
--rw-r--r--   0 runner    (1001) docker     (122)    13736 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_summarize_variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_surveys.py
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_top_bottom_share.py
--rw-r--r--   0 runner    (1001) docker     (122)    10433 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-21 15:57:16.896867 OpenFisca-Survey-Manager-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3403 2023-07-21 15:56:48.000000 OpenFisca-Survey-Manager-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 17:47:02.218834 OpenFisca-Survey-Manager-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (122)    18741 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)    34499 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/LICENSE.AGPL.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 17:47:02.206834 OpenFisca-Survey-Manager-1.1.4/OpenFisca_Survey_Manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14346 2023-07-21 17:47:02.000000 OpenFisca-Survey-Manager-1.1.4/OpenFisca_Survey_Manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2469 2023-07-21 17:47:02.000000 OpenFisca-Survey-Manager-1.1.4/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 17:47:02.000000 OpenFisca-Survey-Manager-1.1.4/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-21 17:47:02.000000 OpenFisca-Survey-Manager-1.1.4/OpenFisca_Survey_Manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 17:47:01.000000 OpenFisca-Survey-Manager-1.1.4/OpenFisca_Survey_Manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      759 2023-07-21 17:47:02.000000 OpenFisca-Survey-Manager-1.1.4/OpenFisca_Survey_Manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-21 17:47:02.000000 OpenFisca-Survey-Manager-1.1.4/OpenFisca_Survey_Manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    14346 2023-07-21 17:47:02.218834 OpenFisca-Survey-Manager-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13432 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 17:47:02.210834 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/
+-rw-r--r--   0 runner    (1001) docker     (122)     2213 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17292 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/aggregates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 17:47:02.214835 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/assets/
+-rw-r--r--   0 runner    (1001) docker     (122)     3551 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/assets/nomenclature_coicop_source_by_divisions.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    12096 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9929 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/calmar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/coicop.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/google_colab.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13337 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/input_dataframe_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4606 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/read_dbf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/read_sas.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/read_spss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    79765 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 17:47:02.214835 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10027 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/scripts/build_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11312 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/statshelpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/survey_collections.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10119 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/surveys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9552 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/temporary.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 17:47:02.218834 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 17:47:02.218834 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/data_files/
+-rw-r--r--   0 runner    (1001) docker     (122)      381 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/data_files/config_template.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     3539 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_add_survey_to_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_calmar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5223 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_legislation_inflator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      989 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_marginal_tax_rate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4373 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (122)      792 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_read_sas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13736 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_summarize_variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_surveys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_top_bottom_share.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10433 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-21 17:47:02.218834 OpenFisca-Survey-Manager-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3403 2023-07-21 17:46:37.000000 OpenFisca-Survey-Manager-1.1.4/setup.py
```

### Comparing `OpenFisca-Survey-Manager-1.1.3/CHANGELOG.md` & `OpenFisca-Survey-Manager-1.1.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 ﻿# Changelog
 
+### 1.1.4 [#264](https://github.com/openfisca/openfisca-survey-manager/pull/264)
+
+* Technical changes
+- Change importlib metadata import to work with all Python version
+
 ### 1.1.3 [#263](https://github.com/openfisca/openfisca-survey-manager/pull/263)
 
 * Technical changes
 - Use importlib instead of pkg_resources to avoid deprecation warnings
 
 ### 1.1.2 [#262](https://github.com/openfisca/openfisca-survey-manager/pull/262)
```

### Comparing `OpenFisca-Survey-Manager-1.1.3/LICENSE.AGPL.txt` & `OpenFisca-Survey-Manager-1.1.4/LICENSE.AGPL.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/PKG-INFO` & `OpenFisca-Survey-Manager-1.1.4/OpenFisca_Survey_Manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Survey-Manager
-Version: 1.1.3
+Version: 1.1.4
 Summary: A tool for managing survey/administrative data.
 Home-page: https://github.com/openfisca/openfisca-survey-manager
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: survey data
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/SOURCES.txt` & `OpenFisca-Survey-Manager-1.1.4/OpenFisca_Survey_Manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/OpenFisca_Survey_Manager.egg-info/requires.txt` & `OpenFisca-Survey-Manager-1.1.4/OpenFisca_Survey_Manager.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/PKG-INFO` & `OpenFisca-Survey-Manager-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Survey-Manager
-Version: 1.1.3
+Version: 1.1.4
 Summary: A tool for managing survey/administrative data.
 Home-page: https://github.com/openfisca/openfisca-survey-manager
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: survey data
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-Survey-Manager-1.1.3/README.md` & `OpenFisca-Survey-Manager-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/__init__.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import importlib
+from importlib import metadata
 import logging
 import os
 from pathlib import Path
 
 log = logging.getLogger(__name__)
 
 
 openfisca_survey_manager_location = Path(
-    importlib.metadata.distribution('openfisca-survey-manager').files[0]
+    metadata.distribution('openfisca-survey-manager').files[0]
     ).parent
 
 # Hack for use at the CASD (shared user)
 # Use taxipp/.config/ directory if exists as default_config_files_directory
 try:
-    taxipp_location = importlib.metadata.distribution('taxipp').files[0]
+    taxipp_location = Path(metadata.distribution('taxipp').files[0]).parent
     default_config_files_directory = os.path.join(taxipp_location, '.config', 'openfisca-survey-manager')
-except importlib.metadata.PackageNotFoundError:
+except metadata.PackageNotFoundError:
     taxipp_location = None
 
 if taxipp_location is None or not os.path.exists(default_config_files_directory):
     default_config_files_directory = None
 
 
 # Hack for uising with france-data on a CI or locally
 try:
-    france_data_location = importlib.metadata.distribution('openfisca-france_data').files[0]
+    france_data_location = Path(metadata.distribution('openfisca-france_data').files[0]).parent
     from xdg import BaseDirectory
     default_config_files_directory = BaseDirectory.save_config_path('openfisca-survey-manager')
-except importlib.metadata.PackageNotFoundError:
+except metadata.PackageNotFoundError:
     france_data_location = None
 
 if france_data_location is None or not os.path.exists(default_config_files_directory):
     default_config_files_directory = None
 
 # Run CI when testing openfisca-survey-manager for example GitHub Actions
 test_config_files_directory = os.path.join(
```

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/aggregates.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/calibration.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/calibration.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/calmar.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/calmar.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/coicop.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/coicop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 import os
 import pandas as pd
-import importlib
 
 
+from openfisca_survey_manager import openfisca_survey_manager_location
+
 log = logging.getLogger(__name__)
 
 
 legislation_directory = os.path.join(
-    importlib.metadata.distribution('openfisca_survey_manager').files[0],
+    openfisca_survey_manager_location,
     'openfisca_survey_manager',
     'assets',
     )
 
 
 sub_levels = ['divisions', 'groupes', 'classes', 'sous_classes', 'postes']
 divisions = ['0{}'.format(i) for i in range(1, 10)] + ['11', '12']
```

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/config.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/config.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/google_colab.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/google_colab.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/input_dataframe_generator.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/input_dataframe_generator.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/matching.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/matching.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/read_dbf.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/read_dbf.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/read_sas.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/read_sas.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/scenarios.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/scenarios.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/scripts/build_collection.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/scripts/build_collection.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/statshelpers.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/statshelpers.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/survey_collections.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/survey_collections.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/surveys.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/surveys.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tables.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/temporary.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/temporary.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_add_survey_to_collection.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_add_survey_to_collection.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_calmar.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_calmar.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_legislation_inflator.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_legislation_inflator.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_marginal_tax_rate.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_marginal_tax_rate.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_matching.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_quantile.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_quantile.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_read_sas.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_read_sas.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_scenario.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_summarize_variables.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_summarize_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_surveys.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_surveys.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/utils.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/utils.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/openfisca_survey_manager/variables.py` & `OpenFisca-Survey-Manager-1.1.4/openfisca_survey_manager/variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/setup.cfg` & `OpenFisca-Survey-Manager-1.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.3/setup.py` & `OpenFisca-Survey-Manager-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 
 doc_lines = __doc__.split('\n')
 
 
 setup(
     name = 'OpenFisca-Survey-Manager',
-    version = '1.1.3',
+    version = '1.1.4',
     author = 'OpenFisca Team',
     author_email = 'contact@openfisca.fr',
     classifiers = [classifier for classifier in classifiers.split('\n') if classifier],
     description = doc_lines[0],
     keywords = 'survey data',
     license = 'http://www.fsf.org/licensing/licenses/agpl-3.0.html',
     license_files = ("LICENSE.AGPL.txt",),
```

