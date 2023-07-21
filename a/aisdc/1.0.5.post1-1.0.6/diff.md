# Comparing `tmp/aisdc-1.0.5.post1.tar.gz` & `tmp/aisdc-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aisdc-1.0.5.post1.tar", last modified: Thu Jun 29 10:47:39 2023, max compression
+gzip compressed data, was "aisdc-1.0.6.tar", last modified: Fri Jul 21 14:39:17 2023, max compression
```

## Comparing `aisdc-1.0.5.post1.tar` & `aisdc-1.0.6.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2022-12-04 22:46:52.000000 aisdc-1.0.5.post1/LICENSE
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5005 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3927 2023-05-17 12:52:16.000000 aisdc-1.0.5.post1/README.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/aisdc/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/__init__.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/aisdc/attacks/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/attacks/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      977 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/attacks/attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    23679 2023-06-29 10:39:36.000000 aisdc-1.0.5.post1/aisdc/attacks/attribute_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2166 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/attacks/dataset.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3616 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/attacks/failfast.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    26233 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/attacks/likelihood_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12913 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/attacks/report.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    30917 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/attacks/worst_case_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10176 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/generate_report.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11752 2023-05-17 12:52:16.000000 aisdc-1.0.5.post1/aisdc/metrics.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/aisdc/preprocessing/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/preprocessing/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    23420 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/preprocessing/loaders.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/aisdc/safemodel/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       61 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/safemodel/__init__.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/aisdc/safemodel/classifiers/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      310 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/safemodel/classifiers/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7491 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/safemodel/classifiers/dp_svc.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7620 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/safemodel/classifiers/new_model_template.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7221 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    20882 2023-06-21 12:33:24.000000 aisdc-1.0.5.post1/aisdc/safemodel/classifiers/safekeras.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6347 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/safemodel/classifiers/saferandomforestclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1912 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/safemodel/classifiers/safesvc.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1212 2023-05-11 14:01:54.000000 aisdc-1.0.5.post1/aisdc/safemodel/classifiers/safetf.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10821 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/safemodel/reporting.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4984 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/safemodel/rules.json
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    30820 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/safemodel/safemodel.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/aisdc.egg-info/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5005 2023-06-29 10:47:39.000000 aisdc-1.0.5.post1/aisdc.egg-info/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1484 2023-06-29 10:47:39.000000 aisdc-1.0.5.post1/aisdc.egg-info/SOURCES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-06-29 10:47:39.000000 aisdc-1.0.5.post1/aisdc.egg-info/dependency_links.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      186 2023-06-29 10:47:39.000000 aisdc-1.0.5.post1/aisdc.egg-info/requires.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        6 2023-06-29 10:47:39.000000 aisdc-1.0.5.post1/aisdc.egg-info/top_level.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/setup.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1890 2023-06-29 10:47:14.000000 aisdc-1.0.5.post1/setup.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/tests/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1598 2023-06-29 10:39:36.000000 aisdc-1.0.5.post1/tests/test_attacks.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2958 2023-06-29 10:39:36.000000 aisdc-1.0.5.post1/tests/test_attacks_dataset.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9109 2023-06-29 10:39:36.000000 aisdc-1.0.5.post1/tests/test_attacks_via_safemodel.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3390 2023-06-29 10:39:36.000000 aisdc-1.0.5.post1/tests/test_attribute_inference_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1470 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/tests/test_data_interface.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5595 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/tests/test_failfast.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6782 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/tests/test_generate_report.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8107 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/tests/test_lira_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6246 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/tests/test_loaders.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6804 2023-05-02 15:16:25.000000 aisdc-1.0.5.post1/tests/test_metrics.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8366 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/tests/test_safedecisiontreeclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    27082 2023-06-29 10:39:36.000000 aisdc-1.0.5.post1/tests/test_safekeras2.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    16955 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/tests/test_safemodel.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11863 2023-05-17 12:52:16.000000 aisdc-1.0.5.post1/tests/test_saferandomforestclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4891 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/tests/test_safesvc.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      365 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/tests/test_safetf.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    13595 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/tests/test_worst_case_attack.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-21 14:39:17.620421 aisdc-1.0.6/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2022-12-04 22:46:52.000000 aisdc-1.0.6/LICENSE
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4999 2023-07-21 14:39:17.620421 aisdc-1.0.6/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3927 2023-05-17 12:52:16.000000 aisdc-1.0.6/README.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-21 14:39:17.620421 aisdc-1.0.6/aisdc/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.6/aisdc/__init__.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-21 14:39:17.620421 aisdc-1.0.6/aisdc/attacks/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.6/aisdc/attacks/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1440 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/attacks/attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    22314 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/attacks/attack_report_formatter.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    26417 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/attacks/attribute_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3594 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/attacks/failfast.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    29545 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/attacks/likelihood_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6396 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/attacks/multiple_attacks.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    14337 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/attacks/report.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12493 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/attacks/target.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    35482 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/attacks/worst_case_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11793 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/metrics.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-21 14:39:17.620421 aisdc-1.0.6/aisdc/preprocessing/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.6/aisdc/preprocessing/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    23392 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/preprocessing/loaders.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-21 14:39:17.620421 aisdc-1.0.6/aisdc/safemodel/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       62 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/safemodel/__init__.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-21 14:39:17.620421 aisdc-1.0.6/aisdc/safemodel/classifiers/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      311 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/safemodel/classifiers/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7391 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/safemodel/classifiers/dp_svc.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7626 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/safemodel/classifiers/new_model_template.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7230 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    20902 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/safemodel/classifiers/safekeras.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6350 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/safemodel/classifiers/saferandomforestclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1914 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/safemodel/classifiers/safesvc.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1214 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/safemodel/classifiers/safetf.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10824 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/safemodel/reporting.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4984 2023-04-26 12:57:02.000000 aisdc-1.0.6/aisdc/safemodel/rules.json
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    28097 2023-07-21 14:08:54.000000 aisdc-1.0.6/aisdc/safemodel/safemodel.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-21 14:39:17.620421 aisdc-1.0.6/aisdc.egg-info/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4999 2023-07-21 14:39:17.000000 aisdc-1.0.6/aisdc.egg-info/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1571 2023-07-21 14:39:17.000000 aisdc-1.0.6/aisdc.egg-info/SOURCES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-07-21 14:39:17.000000 aisdc-1.0.6/aisdc.egg-info/dependency_links.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      200 2023-07-21 14:39:17.000000 aisdc-1.0.6/aisdc.egg-info/requires.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        6 2023-07-21 14:39:17.000000 aisdc-1.0.6/aisdc.egg-info/top_level.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-07-21 14:39:17.620421 aisdc-1.0.6/setup.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1909 2023-07-21 13:28:03.000000 aisdc-1.0.6/setup.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-21 14:39:17.620421 aisdc-1.0.6/tests/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    18938 2023-07-21 14:08:54.000000 aisdc-1.0.6/tests/test_attack_report_formatter.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1612 2023-07-21 14:08:54.000000 aisdc-1.0.6/tests/test_attacks.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5388 2023-07-21 14:08:54.000000 aisdc-1.0.6/tests/test_attacks_target.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6974 2023-07-21 14:08:54.000000 aisdc-1.0.6/tests/test_attacks_via_safemodel.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4024 2023-07-21 14:08:54.000000 aisdc-1.0.6/tests/test_attribute_inference_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1410 2023-07-21 14:08:54.000000 aisdc-1.0.6/tests/test_data_interface.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5724 2023-07-21 14:08:54.000000 aisdc-1.0.6/tests/test_failfast.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9277 2023-07-21 14:08:54.000000 aisdc-1.0.6/tests/test_lira_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6260 2023-07-21 14:08:54.000000 aisdc-1.0.6/tests/test_loaders.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6593 2023-07-21 14:08:54.000000 aisdc-1.0.6/tests/test_metrics.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7230 2023-07-21 14:08:54.000000 aisdc-1.0.6/tests/test_multiple_attacks.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8375 2023-07-21 14:08:54.000000 aisdc-1.0.6/tests/test_safedecisiontreeclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    26926 2023-07-21 14:08:54.000000 aisdc-1.0.6/tests/test_safekeras2.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    17031 2023-07-21 14:08:54.000000 aisdc-1.0.6/tests/test_safemodel.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11877 2023-07-21 14:08:54.000000 aisdc-1.0.6/tests/test_saferandomforestclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4866 2023-07-21 14:08:54.000000 aisdc-1.0.6/tests/test_safesvc.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      363 2023-07-21 14:08:54.000000 aisdc-1.0.6/tests/test_safetf.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    13329 2023-07-21 14:08:54.000000 aisdc-1.0.6/tests/test_worst_case_attack.py
```

### Comparing `aisdc-1.0.5.post1/LICENSE` & `aisdc-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5.post1/PKG-INFO` & `aisdc-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisdc
-Version: 1.0.5.post1
+Version: 1.0.6
 Summary: Tools for the statistical disclosure control of machine learning models
 Home-page: https://github.com/AI-SDC/AI-SDC
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,machine-learning,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aisdc-1.0.5.post1/README.md` & `aisdc-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5.post1/aisdc/attacks/attribute_attack.py` & `aisdc-1.0.6/aisdc/attacks/attribute_attack.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,198 +1,224 @@
-"""
-Attribute inference attacks.
-"""
+"""Attribute inference attacks."""
 
 from __future__ import annotations
 
+import argparse
 import json
 import logging
-
-# import pickle
-from typing import Any
+import os
+import uuid
+from datetime import datetime
 
 import matplotlib.pyplot as plt
 import multiprocess as mp
 import numpy as np
 from fpdf import FPDF
 from sklearn.base import BaseEstimator
 from sklearn.preprocessing import OneHotEncoder
 
 from aisdc.attacks import report
 from aisdc.attacks.attack import Attack
-from aisdc.attacks.dataset import Data
+from aisdc.attacks.attack_report_formatter import GenerateJSONModule
+from aisdc.attacks.target import Target
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("aia")
 
 COLOR_A: str = "#86bf91"  # training set plot colour
 COLOR_B: str = "steelblue"  # testing set plot colour
 
 
-class AttributeAttackArgs:
-    """Arguments for attribute inference."""
-
-    def __init__(self, **kwargs):
-        self.__dict__["report_name"] = None
-        self.__dict__["n_cpu"] = max(1, mp.cpu_count() - 1)
-        self.__dict__.update(kwargs)
-
-    def __str__(self):
-        return ",".join(
-            [f"{str(key)}: {str(value)}" for key, value in self.__dict__.items()]
-        )
-
-    def set_param(self, key: str, value: Any) -> None:
-        """Set a parameter"""
-        self.__dict__[key] = value
-
-    def get_args(self) -> dict:
-        """Return arguments"""
-        return self.__dict__
-
-
 class AttributeAttack(Attack):
     """Class to wrap the attribute inference attack code."""
 
-    def __init__(self, args: AttributeAttackArgs = AttributeAttackArgs()):
+    # pylint: disable=too-many-instance-attributes
+
+    def __init__(  # pylint: disable = too-many-arguments, too-many-locals
+        self,
+        output_dir: str = "output_attribute",
+        report_name: str = "aia_report",
+        n_cpu: int = max(1, mp.cpu_count() - 1),
+        attack_config_json_file_name: str = None,
+        target_path: str = None,
+    ) -> None:
+        """Constructs an object to execute an attribute inference attack.
+
+        Parameters
+        ----------
+        n_cpu : int
+            number of CPUs used to run the attack
+        output_dir : str
+            name of the directory where outputs are stored
+        report_name : str
+            name of the pdf and json output reports
+        attack_config_json_file_name : str
+            name of the configuration file to load parameters
+        target_path : str
+            path to the saved trained target model and target data
+        """
+        super().__init__()
+        self.n_cpu = n_cpu
+        self.output_dir = output_dir
+        self.report_name = report_name
+        self.attack_config_json_file_name = attack_config_json_file_name
+        self.target_path = target_path
+        if self.attack_config_json_file_name is not None:
+            self._update_params_from_config_file()
+        if not os.path.exists(self.output_dir):
+            os.makedirs(self.output_dir)
         self.attack_metrics: dict = {}
         self.metadata: dict = {}
-        self.args = args
 
     def __str__(self):
         return "Attribute inference attack"
 
-    def attack(self, dataset: Data, target_model: BaseEstimator) -> None:
-        """Programmatic attack entry point
+    def attack(self, target: Target) -> None:
+        """Programmatic attack entry point.
 
-        To be used when code has access to data class and trained target model
+        To be used when code has access to Target class and trained target model
 
         Parameters
         ----------
-        dataset: attacks.dataset.Data
-            dataset as a Data class object
-        target_model: sklearn.base.BaseEstimator
-            target model that inherits from an sklearn BaseEstimator
+        target : attacks.target.Target
+            target is a Target class object
         """
-        self.attack_metrics = _attribute_inference(
-            target_model, dataset, self.args.n_cpu
-        )
+        self.attack_metrics = _attribute_inference(target, self.n_cpu)
 
     def _construct_metadata(self) -> None:
         """Constructs the metadata object. Called by the reporting method."""
         self.metadata = {}
         self.metadata["experiment_details"] = {}
-        self.metadata["experiment_details"].update(self.args.__dict__)
+        self.metadata["experiment_details"] = self.get_params()
+
         self.metadata["attack"] = str(self)
 
     def make_report(self) -> dict:
         """Create the report.
 
-        Creates the output report. If self.args.report_name is not None, it will also save the
+        Creates the output report. If self.report_name is not None, it will also save the
         information in json and pdf formats.
 
         Returns
         -------
 
-        output: dict
+        output : dict
             Dictionary containing all attack output.
         """
         output = {}
-        logger.info("Starting report, report_name = %s", self.args.report_name)
-        output["attack_metrics"] = self.attack_metrics
+        report_dest = os.path.join(self.output_dir, self.report_name)
+        logger.info(
+            "Starting reports, pdf report name = %s, json report name = %s",
+            report_dest + ".pdf",
+            report_dest + ".json",
+        )
+        output["log_id"] = str(uuid.uuid4())
+        output["log_time"] = datetime.now().strftime("%d/%m/%Y %H:%M:%S")
         self._construct_metadata()
         output["metadata"] = self.metadata
-        if self.args.report_name is not None:
-            json_report = json.dumps(output, cls=report.NumpyArrayEncoder)
-            with open(f"{self.args.report_name}.json", "w", encoding="utf-8") as f:
-                f.write(json_report)
-            logger.info("Wrote report to %s", f"{self.args.report_name}.json")
-
-            pdf = create_aia_report(output)
-            pdf.output(f"{self.args.report_name}.pdf", "F")
-            logger.info("Wrote pdf report to %s", f"{self.args.report_name}.pdf")
+        output["attack_experiment_logger"] = self._get_attack_metrics_instances()
+
+        json_attack_formatter = GenerateJSONModule(report_dest + ".json")
+        json_report = json.dumps(output, cls=report.NumpyArrayEncoder)
+        json_attack_formatter.add_attack_output(json_report, "AttributeAttack")
+
+        pdf_report = create_aia_report(output, report_dest)
+        report.add_output_to_pdf(report_dest, pdf_report, "AttributeAttack")
+        logger.info(
+            "Wrote pdf report to %s and json report to %s",
+            report_dest + ".pdf",
+            report_dest + ".json",
+        )
         return output
 
+    def _get_attack_metrics_instances(self) -> dict:
+        """Constructs the instances metric calculated, during attacks."""
+        attack_metrics_experiment = {}
+        attack_metrics_instances = {}
+
+        attack_metrics_instances["instance_0"] = self.attack_metrics
+
+        attack_metrics_experiment["attack_instance_logger"] = attack_metrics_instances
+        return attack_metrics_experiment
+
 
 def _unique_max(confidences: list[float], threshold: float) -> bool:
     """Returns whether there is a unique maximum confidence value above
-    threshold."""
+    threshold.
+    """
     if len(confidences) > 0:
         max_conf = np.max(confidences)
         if max_conf < threshold:
             return False
         unique, count = np.unique(confidences, return_counts=True)
         for u, c in zip(unique, count):
             if c == 1 and u == max_conf:
                 return True
     return False
 
 
 def _get_inference_data(  # pylint: disable=too-many-locals
-    target_model: BaseEstimator, dataset: Data, feature_id: int, memberset: bool
+    target: Target, feature_id: int, memberset: bool
 ) -> tuple[np.ndarray, np.ndarray, float]:
     """Returns a dataset of each sample with the attributes to test."""
-    attack_feature: dict = dataset.features[feature_id]
+    attack_feature: dict = target.features[feature_id]
     indices: list[int] = attack_feature["indices"]
-    unique = np.unique(dataset.x_orig[:, feature_id])
+    unique = np.unique(target.x_orig[:, feature_id])
     n_unique: int = len(unique)
     if attack_feature["encoding"] == "onehot":
         onehot_enc = OneHotEncoder()
         values = onehot_enc.fit_transform(unique.reshape(-1, 1)).toarray()
     else:  # pragma: no cover
         # catch all, but can't be reached because this func only called via _infer
         # which is only called for categorical data
         values = unique
     # samples after encoding (e.g. one-hot)
-    samples: np.ndarray = dataset.x_train
+    samples: np.ndarray = target.x_train
     # samples before encoding (e.g. str)
-    samples_orig: np.ndarray = dataset.x_train_orig
+    samples_orig: np.ndarray = target.x_train_orig
     if not memberset:
-        samples = dataset.x_test
-        samples_orig = dataset.x_test_orig
+        samples = target.x_test
+        samples_orig = target.x_test_orig
     n_samples, x_dim = np.shape(samples)
     x_values = np.zeros((n_samples, n_unique, x_dim), dtype=np.float64)
-    y_values = target_model.predict(samples)
+    y_values = target.model.predict(samples)
     # for each sample to perform inference on
     # add each possible missing feature value
     for i, x in enumerate(samples):
         for j, value in enumerate(values):
             x_values[i][j] = np.copy(x)
             x_values[i][j][indices] = value
     _, counts = np.unique(samples_orig[:, feature_id], return_counts=True)
     baseline = (np.max(counts) / n_samples) * 100
     logger.debug("feature: %d x_values shape = %s", feature_id, np.shape(x_values))
     logger.debug("feature: %d y_values shape = %s", feature_id, np.shape(y_values))
     return x_values, y_values, baseline
 
 
 def _infer(  # pylint: disable=too-many-locals
-    target_model: BaseEstimator,
-    dataset: Data,
+    target: Target,
     feature_id: int,
     threshold: float,
     memberset: bool,
 ) -> tuple[int, int, float, int, int]:
     """
     For each possible missing value, compute the confidence scores and
     label with the target model; if the label matches the known target model
     label for the original sample, and the highest confidence score is unique,
     infer that attribute if the confidence score is greater than a threshold.
     """
     logger.debug("Commencing attack on feature %d set %d", feature_id, int(memberset))
     correct: int = 0  # number of correct inferences made
     total: int = 0  # total number of inferences made
-    x_values, y_values, baseline = _get_inference_data(
-        target_model, dataset, feature_id, memberset
-    )
+    x_values, y_values, baseline = _get_inference_data(target, feature_id, memberset)
     n_unique: int = len(x_values[1])
-    samples = dataset.x_train if memberset else dataset.x_test
+    samples = target.x_train if memberset else target.x_test
     for i, x in enumerate(x_values):  # each sample to perform inference on
         # get model confidence scores for all possible values for the sample
-        confidence = target_model.predict_proba(x)
+        confidence = target.model.predict_proba(x)
         conf = []  # confidences for each possible value with correct label
         attr = []  # features for each possible value with correct label
         # for each possible attribute value,
         # if the label matches the known target model label
         # then store the confidence score and the tested feature vector
         for j in range(n_unique):
             this_label = np.argmax(confidence[j])
@@ -370,51 +396,47 @@
 #     with open(filename + ".pickle", "rb") as handle:
 #         results = pickle.load(handle)
 #     plot_categorical_risk(results, savefile=savefile)
 #     plot_categorical_fraction(results, savefile=savefile)
 #     plot_quantitative_risk(results, savefile=savefile)
 
 
-def _infer_categorical(
-    target_model: BaseEstimator, dataset: Data, feature_id: int, threshold: float
-) -> dict:
+def _infer_categorical(target: Target, feature_id: int, threshold: float) -> dict:
     """Returns the training and test set risks of a categorical feature."""
     result: dict = {
-        "name": dataset.features[feature_id]["name"],
-        "train": _infer(target_model, dataset, feature_id, threshold, True),
-        "test": _infer(target_model, dataset, feature_id, threshold, False),
+        "name": target.features[feature_id]["name"],
+        "train": _infer(target, feature_id, threshold, True),
+        "test": _infer(target, feature_id, threshold, False),
     }
     return result
 
 
-def _is_categorical(dataset: Data, feature_id: int) -> bool:
+def _is_categorical(target: Target, feature_id: int) -> bool:
     """Returns whether a feature is categorical.
-    For simplicity, assumes integer datatypes are categorical."""
-    encoding: str = dataset.features[feature_id]["encoding"]
+    For simplicity, assumes integer datatypes are categorical.
+    """
+    encoding: str = target.features[feature_id]["encoding"]
     if encoding[:3] in ("str", "int") or encoding[:6] in ("onehot"):
         return True
     return False
 
 
 def _attack_brute_force(
-    target_model: BaseEstimator,
-    dataset: Data,
+    target: Target,
     features: list[int],
     n_cpu: int,
     attack_threshold: float = 0,
 ) -> list[dict]:
     """
     Performs a brute force attribute inference attack by computing the target
     model confidence scores for every value in the list and making an inference
     if there is a unique highest confidence score that exceeds attack_threshold.
     """
     logger.debug("Brute force attacking categorical features")
-    args = [
-        (target_model, dataset, feature_id, attack_threshold) for feature_id in features
-    ]
+    args = [(target, feature_id, attack_threshold) for feature_id in features]
     with mp.Pool(processes=n_cpu) as pool:  # pylint:disable=not-callable
         results = pool.starmap(_infer_categorical, args)
     return results
 
 
 def _get_bounds_risk_for_sample(  # pylint: disable=too-many-locals,too-many-arguments
     target_model: BaseEstimator,
@@ -428,36 +450,35 @@
 ) -> bool:
     """Returns a bool based on conditions surrounding upper and lower bounds of
     guesses that would lead to the same model confidence.
 
     Parameters
     ----------
 
-    target_model: BaseEstimator
+    target_model : BaseEstimator
         Trained target model.
-    feat_id: int
+    feat_id : int
         Index of missing feature.
-    feat_min: float
+    feat_min : float
         Minimum value of missing feature.
-    feat_max: float
+    feat_max : float
         Maximum value of missing feature.
-    sample: np.ndarray
+    sample : np.ndarray
         Original known feature vector.
-    c_min: float
+    c_min : float
         Defines the confidence threshold below which we say we don't care.
-    protection_limit: float
+    protection_limit : float
         Lower [upper] bound on estimated value must not be
         above[below] lower[upper] bounds e.g. 10% of value.
-    feat_n: int
+    feat_n : int
         Number of attribute values to test per sample.
 
     Returns
     -------
     A bool representing whether the quantitative feature is at risk for the sample.
-
     """
     # attribute values to test - linearly sampled
     x_feat = np.linspace(feat_min, feat_max, feat_n, endpoint=True)
     # get known label
     label: int = int(target_model.predict(sample.reshape(1, -1))[0])
     # a matrix containing feature vector with linearly spaced target attribute
     x1 = np.repeat(sample.reshape(1, -1), feat_n, axis=0)
@@ -521,83 +542,74 @@
     target_model: BaseEstimator,
     feature_name: str,
     feature_id: int,
     x_train: np.ndarray,
     x_test: np.ndarray,
 ) -> dict:
     """Returns a dictionary containing the training and test set risks of a
-    quantitative feature."""
+    quantitative feature.
+    """
     risk: dict = {
         "name": feature_name,
         "train": _get_bounds_risk_for_feature(target_model, feature_id, x_train),
         "test": _get_bounds_risk_for_feature(target_model, feature_id, x_test),
     }
     return risk
 
 
-def _get_bounds_risks(
-    target_model: BaseEstimator, dataset: Data, features: list[int], n_cpu: int
-) -> list[dict]:
+def _get_bounds_risks(target: Target, features: list[int], n_cpu: int) -> list[dict]:
     """Computes the bounds risk for all specified features."""
     logger.debug("Computing bounds risk for all specified features")
     args = [
         (
-            target_model,
-            dataset.features[feature_id]["name"],
+            target.model,
+            target.features[feature_id]["name"],
             feature_id,
-            dataset.x_train,
-            dataset.x_test,
+            target.x_train,
+            target.x_test,
         )
         for feature_id in features
     ]
     with mp.Pool(processes=n_cpu) as pool:  # pylint:disable=not-callable
         results = pool.starmap(_get_bounds_risk, args)
     return results
 
 
-def _attribute_inference(
-    target_model: BaseEstimator,
-    dataset: Data,
-    n_cpu: int,
-) -> dict:
-    """
-    Execute attribute inference attacks on a dataset given a trained model.
-    """
+def _attribute_inference(target: Target, n_cpu: int) -> dict:
+    """Execute attribute inference attacks on a target given a trained model."""
     # brute force attack categorical attributes using dataset unique values
-    logger.debug("Attacking dataset: %s", dataset.name)
+    logger.debug("Attacking dataset: %s", target.name)
     logger.debug("Attacking categorical attributes...")
     feature_list: list[int] = []
-    for feature in range(dataset.n_features):
-        if _is_categorical(dataset, feature):
+    for feature in range(target.n_features):
+        if _is_categorical(target, feature):
             feature_list.append(feature)
-    results_a: list[dict] = _attack_brute_force(
-        target_model, dataset, feature_list, n_cpu
-    )
+    results_a: list[dict] = _attack_brute_force(target, feature_list, n_cpu)
     # compute risk scores for quantitative attributes
     logger.debug("Attacking quantitative attributes...")
     feature_list = []
-    for feature in range(dataset.n_features):
-        if not _is_categorical(dataset, feature):
+    for feature in range(target.n_features):
+        if not _is_categorical(target, feature):
             feature_list.append(feature)
-    results_b: list[dict] = _get_bounds_risks(
-        target_model, dataset, feature_list, n_cpu
-    )
+    results_b: list[dict] = _get_bounds_risks(target, feature_list, n_cpu)
     # combine results into single object
     results: dict = {
-        "name": dataset.name,
+        "name": target.name,
         "categorical": results_a,
         "quantitative": results_b,
     }
     return results
 
 
 def create_aia_report(output: dict, name: str = "aia_report") -> FPDF:
     """Creates PDF report."""
-    aia_metrics = output["attack_metrics"]
     metadata = output["metadata"]
+    aia_metrics = output["attack_experiment_logger"]["attack_instance_logger"][
+        "instance_0"
+    ]
     plot_categorical_risk(aia_metrics, name)
     plot_categorical_fraction(aia_metrics, name)
     plot_quantitative_risk(aia_metrics, name)
     pdf = FPDF()
     pdf.add_page()
     pdf.set_xy(0, 0)
     report.title(pdf, "Attribute Inference Attack Report")
@@ -620,7 +632,65 @@
         pdf.image(name + "_cat_risk.png", x=None, y=None, w=150, h=0, type="", link="")
         pdf.image(name + "_cat_frac.png", x=None, y=None, w=150, h=0, type="", link="")
     if len(aia_metrics["quantitative"]) > 0:
         pdf.image(
             name + "_quant_risk.png", x=None, y=None, w=150, h=0, type="", link=""
         )
     return pdf
+
+
+def _run_attack_from_configfile(args):
+    """Run a command line attack based on saved files described in .json file."""
+    attack_obj = AttributeAttack(
+        attack_config_json_file_name=str(args.attack_config_json_file_name),
+        target_path=str(args.target_path),
+    )
+    target = Target()
+    target.load(attack_obj.target_path)
+    attack_obj.attack(target)
+    attack_obj.make_report()
+
+
+def main():
+    """Main method to parse args and invoke relevant code."""
+    parser = argparse.ArgumentParser(add_help=False)
+
+    subparsers = parser.add_subparsers()
+    attack_parser_config = subparsers.add_parser("run-attack-from-configfile")
+    attack_parser_config.add_argument(
+        "-j",
+        "--attack-config-json-file-name",
+        action="store",
+        required=True,
+        dest="attack_config_json_file_name",
+        type=str,
+        default="config_aia_cmd.json",
+        help=(
+            "Name of the .json file containing details for the run. Default = %(default)s"
+        ),
+    )
+
+    attack_parser_config.add_argument(
+        "-t",
+        "--attack-target-folder-path",
+        action="store",
+        required=True,
+        dest="target_path",
+        type=str,
+        default="aia_target",
+        help=(
+            """Name of the target directory to load the trained target model and the target data.
+        Default = %(default)s"""
+        ),
+    )
+
+    attack_parser_config.set_defaults(func=_run_attack_from_configfile)
+    args = parser.parse_args()
+    try:
+        args.func(args)
+    except AttributeError as e:  # pragma:no cover
+        print(e)
+        print("Invalid command. Try --help to get more details")
+
+
+if __name__ == "__main__":  # pragma:no cover
+    main()
```

### Comparing `aisdc-1.0.5.post1/aisdc/attacks/failfast.py` & `aisdc-1.0.6/aisdc/attacks/failfast.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-"""failfast.py - class to evaluate metric for fail fast option"""
+"""Failfast.py - class to evaluate metric for fail fast option."""
 
 from __future__ import annotations
 
 from typing import Any
 
 
 class FailFast:  # pylint: disable=too-many-instance-attributes
     """Class to check attack being successful or not for a given metric
     Note: An object of a FailFast is stateful and instance members
     (success_count and fail_count) will preserve values
     across repetitions for a test. For the new test
     a new object will require to be instantiated.
     """
 
-    def __init__(self, attack_obj_args: Any):
-        self.metric_name = attack_obj_args.attack_metric_success_name
-        self.metric_success_thresh = attack_obj_args.attack_metric_success_thresh
-        self.comp_type = attack_obj_args.attack_metric_success_comp_type
+    def __init__(self, attack_obj: Any):
+        self.metric_name = attack_obj.attack_metric_success_name
+        self.metric_success_thresh = attack_obj.attack_metric_success_thresh
+        self.comp_type = attack_obj.attack_metric_success_comp_type
         self.success_count = 0
         self.fail_count = 0
 
     # pylint: disable=too-many-branches
     def check_attack_success(self, metric_dict: dict) -> bool:
-        """A function to check if attack was successful for a given metric
+        """A function to check if attack was successful for a given metric.
 
         Parameters
         ----------
-        metric_dict: dict
+        metric_dict : dict
             a dictionary with all computed metric values
 
         Returns
         -------
-        success_status: bool
+        success_status : bool
             a boolean value is returned based on the comparison for a given threshold
 
         Notes
         -----
         If value of a given metric value has a value meeting the threshold based on
         the comparison type returns true otherwise it returns false. This function
         also counts how many times the attack was successful (i.e. true) and
@@ -66,27 +66,27 @@
     def _increment_success_count(self) -> int:
         self.success_count += 1
 
     def _incremenet_fail_count(self) -> int:
         self.fail_count += 1
 
     def get_success_count(self) -> int:
-        """Returns a count of attack being successful"""
+        """Returns a count of attack being successful."""
         return self.success_count
 
     def get_fail_count(self):
-        """Returns a count of attack being not successful"""
+        """Returns a count of attack being not successful."""
         return self.fail_count
 
     def get_attack_summary(self) -> dict:
-        """Returns a dictionary of counts of attack being successful and not successful"""
+        """Returns a dictionary of counts of attack being successful and not successful."""
         summary = {}
         summary["success_count"] = self.success_count
         summary["fail_count"] = self.fail_count
         return summary
 
-    def check_overall_attack_success(self, attack_obj_args: Any) -> bool:
-        """Returns true if the attack is successful for a given success count threshold"""
+    def check_overall_attack_success(self, attack_obj: Any) -> bool:
+        """Returns true if the attack is successful for a given success count threshold."""
         overall_success_status = False
-        if self.success_count >= attack_obj_args.attack_metric_success_count_thresh:
+        if self.success_count >= attack_obj.attack_metric_success_count_thresh:
             overall_success_status = True
         return overall_success_status
```

### Comparing `aisdc-1.0.5.post1/aisdc/attacks/likelihood_attack.py` & `aisdc-1.0.6/aisdc/attacks/likelihood_attack.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,236 +1,265 @@
-"""
-Likelihood testing scenario from https://arxiv.org/pdf/2112.03570.pdf
-"""
+"""Likelihood testing scenario from https://arxiv.org/pdf/2112.03570.pdf."""
 # pylint: disable = invalid-name
 # pylint: disable = too-many-branches
 
 from __future__ import annotations
 
 import argparse
 import importlib
 import json
 import logging
+import os
 import uuid
-from collections.abc import Hashable, Iterable
+from collections.abc import Iterable
 from datetime import datetime
-from typing import Any
 
 import numpy as np
 import sklearn
 from scipy.stats import norm
 from sklearn.datasets import load_breast_cancer
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import train_test_split
 
 from aisdc import metrics
 from aisdc.attacks import report
-from aisdc.attacks.attack import Attack, ConfigFile
-from aisdc.attacks.dataset import Data
+from aisdc.attacks.attack import Attack
+from aisdc.attacks.attack_report_formatter import GenerateJSONModule
+from aisdc.attacks.target import Target
 
 logging.basicConfig(level=logging.INFO)
 
 N_SHADOW_MODELS = 100  # Number of shadow models that should be trained
 EPS = 1e-16  # Used to avoid numerical issues in logit function
 P_THRESH = 0.05  # default significance threshold
 
 
 class DummyClassifier:
-    """A Dummy Classifier to allow this code to work with get_metrics"""
+    """A Dummy Classifier to allow this code to work with get_metrics."""
 
     def predict(self, test_X):
-        """Return an array of 1/0 depending on value in second column"""
+        """Return an array of 1/0 depending on value in second column."""
         return 1 * (test_X[:, 1] > 0.5)
 
     def predict_proba(self, test_X):
-        """Simply return the test_X"""
+        """Simply return the test_X."""
         return test_X
 
 
 def _logit(p: float) -> float:
-    """Standard logit function
+    """Standard logit function.
 
     Parameters
     ----------
-    p: float
+    p : float
         value to evaluate logit at
 
     Returns
     -------
-    li: float
+    li : float
         logit(p)
 
     Notes
     -----
     If p is close to 0 or 1, evaluating the log will result in numerical instabilities.
     This code thresholds p at EPS and 1 - EPS where EPS defaults at 1e-16.
     """
     if p > 1 - EPS:
         p = 1 - EPS
     p = max(p, EPS)
     li = np.log(p / (1 - p))
     return li
 
 
-class LIRAAttackArgs:
-    """LIRA Attack arguments"""
-
-    def __init__(self, **kwargs):
-        self.__dict__["n_shadow_models"] = N_SHADOW_MODELS
-        self.__dict__["n_shadow_rows_confidences_min"] = 10
-        self.__dict__["p_thresh"] = 0.05
-        self.__dict__["report_name"] = None
-        self.__dict__["training_data_filename"] = None
-        self.__dict__["test_data_filename"] = None
-        self.__dict__["training_preds_filename"] = None
-        self.__dict__["test_preds_filename"] = None
-        self.__dict__["target_model"] = None
-        self.__dict__["target_model_hyp"] = None
-        self.__dict__["attack_config_json_file_name"] = None
-        self.__dict__["shadow_models_fail_fast"] = False
-        self.__dict__.update(kwargs)
-        if self.__dict__["attack_config_json_file_name"] is not None:
-            configfile_obj = ConfigFile(self.__dict__["attack_config_json_file_name"])
-            configfile_obj.load_config_file_into_dict(self.__dict__)
-        # deleted for not enabling to appear in the output file
-        del self.__dict__["attack_config_json_file_name"]
-
-    def __str__(self):
-        return ",".join(
-            [f"{str(key)}: {str(value)}" for key, value in self.__dict__.items()]
-        )
-
-    def set_param(self, key: Hashable, value: Any) -> None:
-        """Set a parameter"""
-        self.__dict__[key] = value
-
-    def get_args(self) -> dict:
-        """Return arguments"""
-        return self.__dict__
+class LIRAAttack(Attack):
+    """The main LIRA Attack class."""
 
+    # pylint: disable=too-many-instance-attributes
 
-class LIRAAttack(Attack):
-    """The main LIRA Attack class"""
+    def __init__(  # pylint: disable = too-many-arguments, too-many-locals
+        self,
+        n_shadow_models: int = 100,
+        p_thresh: float = 0.05,
+        output_dir: str = "outputs_lira",
+        report_name: str = "report_lira",
+        training_data_filename: str = None,
+        test_data_filename: str = None,
+        training_preds_filename: str = None,
+        test_preds_filename: str = None,
+        target_model: list = None,
+        target_model_hyp: dict = None,
+        attack_config_json_file_name: str = None,
+        n_shadow_rows_confidences_min: int = 10,
+        shadow_models_fail_fast: bool = False,
+        target_path: str = None,
+    ) -> None:
+        """Constructs an object to execute a LIRA attack.
 
-    def __init__(self, args: LIRAAttackArgs = LIRAAttackArgs()) -> None:
+        Parameters
+        ----------
+        n_shadow_models : int
+            number of shadow models to be trained
+        p_thresh : float
+            threshold to determine significance of things. For instance auc_p_value and pdif_vals
+        output_dir : str
+            name of the directory where outputs are stored
+        report_name : str
+            name of the pdf and json output reports
+        training_data_filename : str
+            name of the data file for the training data (in-sample)
+        test_data_filename : str
+            name of the file for the test data (out-of-sample)
+        training_preds_filename : str
+            name of the file to keep predictions of the training data (in-sample)
+        test_preds_filename : str
+            name of the file to keep predictions of the test data (out-of-sample)
+        target_model : list
+            name of the module (i.e. classification module name such as 'sklearn.ensemble') and
+            attack model name (i.e. classification model name such as 'RandomForestClassifier')
+        target_model_hyp : dict
+            dictionary of hyper parameters for the target_model
+            such as min_sample_split, min_samples_leaf etc
+        attack_config_json_file_name : str
+            name of the configuration file to load parameters
+        n_shadow_rows_confidences_min : int
+            number of minimum number of confidences calculated for
+            each row in test data (out-of-sample)
+        shadow_models_fail_fast : bool
+            If true it stops repetitions earlier based on the given minimum
+            number of confidences for each row in the test data
+        target_path : str
+            path to the saved trained target model and target data
+        """
+        super().__init__()
+        self.n_shadow_models = n_shadow_models
+        self.p_thresh = p_thresh
+        self.output_dir = output_dir
+        self.report_name = report_name
+        self.training_data_filename = training_data_filename
+        self.test_data_filename = test_data_filename
+        self.training_preds_filename = training_preds_filename
+        self.test_preds_filename = test_preds_filename
+        self.target_model = target_model
+        self.target_model_hyp = target_model_hyp
+        self.attack_config_json_file_name = attack_config_json_file_name
+        self.n_shadow_rows_confidences_min = n_shadow_rows_confidences_min
+        self.shadow_models_fail_fast = shadow_models_fail_fast
+        self.target_path = target_path
+        if self.attack_config_json_file_name is not None:
+            self._update_params_from_config_file()
+        if not os.path.exists(self.output_dir):
+            os.makedirs(self.output_dir)
         self.attack_metrics = None
         self.attack_failfast_shadow_models_trained = None
-        self.dummy_attack_metrics = None
         self.metadata = None
-        self.args = args
 
     def __str__(self):
         return "LIRA Attack"
 
-    def attack(self, dataset: Data, target_model: sklearn.base.BaseEstimator) -> None:
+    def attack(self, target: Target) -> None:
         """Programmatic attack running
-        Runs a LIRA attack from a dataset object and a target model
+        Runs a LIRA attack from a Target object and a target model.
 
         Parameters
         ----------
-        dataset: attacks.dataset.Data
-            Dataset as an instance of the Data class. Needs to have x_train, x_test, y_train
-            and y_test set.
-        target_model: sklearn.base.BaseEstimator
-            Trained target model. Any class that implements the sklearn.base.BaseEstimator
-            interface (i.e. has fit, predict and predict_proba methods)
+        target : attacks.target.Target
+            target as an instance of the Target class. Needs to have x_train,
+            x_test, y_train and y_test set.
         """
 
-        shadow_clf = sklearn.base.clone(target_model)
+        shadow_clf = sklearn.base.clone(target.model)
 
-        dataset = self._check_and_update_dataset(dataset, target_model)
+        target = self._check_and_update_dataset(target)
 
         self.run_scenario_from_preds(
             shadow_clf,
-            dataset.x_train,
-            dataset.y_train,
-            target_model.predict_proba(dataset.x_train),
-            dataset.x_test,
-            dataset.y_test,
-            target_model.predict_proba(dataset.x_test),
-        )
-
-    def _check_and_update_dataset(
-        self, dataset: Data, target_model: sklearn.base.BaseEstimator
-    ) -> Data:
-        """Makes sure that it is ok to use the class variables to index the prediction
-        arrays. This has two steps:
-        1. Replacing the values in y_train with their position in target_model.classes (will
-           normally result in no change)
-        2. Removing from the test set any rows corresponding to classes that are not in the
-           training set.
+            target.x_train,
+            target.y_train,
+            target.model.predict_proba(target.x_train),
+            target.x_test,
+            target.y_test,
+            target.model.predict_proba(target.x_test),
+        )
+
+    def _check_and_update_dataset(self, target: Target) -> Target:
+        """
+        Makes sure that it is ok to use the class variables to index the
+        prediction arrays. This has two steps:
+        1. Replacing the values in y_train with their position in
+        target.model.classes (will normally result in no change)
+        2. Removing from the test set any rows corresponding to classes that
+        are not in the training set.
         """
         logger = logging.getLogger("_check_and_update_dataset")
         y_train_new = []
-        classes = list(target_model.classes_)  # pylint: disable = protected-access
-        for y in dataset.y_train:
+        classes = list(target.model.classes_)  # pylint: disable = protected-access
+        for y in target.y_train:
             y_train_new.append(classes.index(y))
 
-        dataset.y_train = np.array(y_train_new, int)
+        target.y_train = np.array(y_train_new, int)
 
         logger.info(
             "new ytrain has values and counts: %s",
-            f"{np.unique(dataset.y_train,return_counts=True)}",
+            f"{np.unique(target.y_train,return_counts=True)}",
         )
         ok_pos = []
         y_test_new = []
-        for i, y in enumerate(dataset.y_test):
+        for i, y in enumerate(target.y_test):
             if y in classes:
                 ok_pos.append(i)
                 y_test_new.append(classes.index(y))
 
-        if len(y_test_new) != len(dataset.x_test):
-            dataset.x_test = dataset.x_test[ok_pos, :]
-        dataset.y_test = np.array(y_test_new, int)
+        if len(y_test_new) != len(target.x_test):
+            target.x_test = target.x_test[ok_pos, :]
+        target.y_test = np.array(y_test_new, int)
         logger.info(
             "new ytest has values and counts: %s",
-            f"{np.unique(dataset.y_test,return_counts=True)}",
+            f"{np.unique(target.y_test,return_counts=True)}",
         )
 
-        return dataset
+        return target
 
     def run_scenario_from_preds(  # pylint: disable = too-many-statements, too-many-arguments, too-many-locals
         self,
         shadow_clf: sklearn.base.BaseEstimator,
         X_target_train: Iterable[float],
         y_target_train: Iterable[float],
         target_train_preds: Iterable[float],
         X_shadow_train: Iterable[float],
         y_shadow_train: Iterable[float],
         shadow_train_preds: Iterable[float],
     ) -> tuple[np.ndarray, np.ndarray, sklearn.base.BaseEstimator]:
         """Implements the likelihood test, using the "offline" version
-        See p.6 (top of second column) for details
+        See p.6 (top of second column) for details.
 
         Parameters
         ----------
-        shadow_clf: sklearn.Model
+        shadow_clf : sklearn.Model
             An sklearn classifier that will be trained to form the shadow model.
             All hyper-parameters should have been set.
-        X_target_train: np.ndarray
+        X_target_train : np.ndarray
             Data that was used to train the target model
-        y_target_train: np.ndarray
+        y_target_train : np.ndarray
             Labels that were used to train the target model
-        target_train_preds: np.ndarray
+        target_train_preds : np.ndarray
             Array of predictions produced by the target model on the training data
-        X_shadow_train: np.ndarray
+        X_shadow_train : np.ndarray
             Data that will be used to train the shadow models
-        y_shadow_train: np.ndarray
+        y_shadow_train : np.ndarray
             Labels that will be used to train the shadow model
-        shadow_train_preds: np.ndarray
+        shadow_train_preds : np.ndarray
             Array of predictions produced by the target model on the shadow data
 
-
         Returns
         -------
-        mia_scores: np.ndarray
+        mia_scores : np.ndarray
             Attack probabilities of belonging to the training set or not
-        mia_labels: np.ndarray
+        mia_labels : np.ndarray
             True labels of belonging to the training set or not
-        mia_cls: DummyClassifier
+        mia_cls : DummyClassifier
             A DummyClassifier that directly returns the scores for compatibility with code
             in metrics.py
 
         Examples
         --------
 
         >>> X, y = load_breast_cancer(return_X_y=True, as_frame=False)
@@ -262,15 +291,15 @@
         combined_y_train = np.hstack((y_target_train, y_shadow_train))
 
         train_row_to_confidence = {i: [] for i in range(n_train_rows)}
         shadow_row_to_confidence = {i: [] for i in range(n_shadow_rows)}
 
         # Train N_SHADOW_MODELS shadow models
         logger.info("Training shadow models")
-        for model_idx in range(self.args.n_shadow_models):
+        for model_idx in range(self.n_shadow_models):
             if model_idx % 10 == 0:
                 logger.info("Trained %d models", model_idx)
             # Pick the indices to use for training this one
             np.random.seed(model_idx)  # Reproducibility
             these_idx = np.random.choice(indices, n_train_rows, replace=False)
             temp_X_train = combined_X_train[these_idx, :]
             temp_y_train = combined_y_train[these_idx]
@@ -315,24 +344,24 @@
                         # catch-all
                         shadow_row_to_confidence[i].append(_logit(0))
 
             # Compute number of confidences for each row
             lengths_shadow_row_to_confidence = {
                 key: len(value) for key, value in shadow_row_to_confidence.items()
             }
-            n_shadow_confidences = self.args.n_shadow_rows_confidences_min
+            n_shadow_confidences = self.n_shadow_rows_confidences_min
             # Stop training of shadow models when shadow_model_fail_fast is True
             # and a minimum number of confidences specified by parameter
             # (n_shadow_rows_confidences_min) are computed for each row
             if (
                 not any(
                     value < n_shadow_confidences
                     for value in lengths_shadow_row_to_confidence.values()
                 )
-                and self.args.shadow_models_fail_fast
+                and self.shadow_models_fail_fast
             ):
                 break
         self.attack_failfast_shadow_models_trained = model_idx + 1
         # Do the test described in the paper in each case
         mia_scores = []
         mia_labels = []
         logger.info("Computing scores for train rows")
@@ -366,15 +395,15 @@
         mia_labels = np.array(mia_labels)
         y_pred_proba, y_test = metrics.get_probabilities(
             mia_clf, mia_scores, mia_labels, permute_rows=True
         )
         self.attack_metrics = [metrics.get_metrics(y_pred_proba, y_test)]
 
     def example(self) -> None:  # pylint: disable = too-many-locals
-        """Runs an example attack using data from sklearn
+        """Runs an example attack using data from sklearn.
 
         Generates example data, trains a classifier and tuns the attack
         """
         X, y = load_breast_cancer(return_X_y=True, as_frame=False)
         train_X, test_X, train_y, test_y = train_test_split(
             X, y, test_size=0.5, stratify=y
         )
@@ -387,81 +416,87 @@
             rf.predict_proba(train_X),
             test_X,
             test_y,
             rf.predict_proba(test_X),
         )
 
     def _construct_metadata(self) -> None:
-        """Constructs the metadata object. Called by the reporting method"""
+        """Constructs the metadata object. Called by the reporting method."""
         self.metadata = {}
         self.metadata["experiment_details"] = {}
-        self.metadata["experiment_details"].update(self.args.__dict__)
-        if "func" in self.metadata["experiment_details"]:
-            del self.metadata["experiment_details"]["func"]
+        self.metadata["experiment_details"] = self.get_params()
 
         self.metadata["global_metrics"] = {}
 
         pdif = np.exp(-self.attack_metrics[0]["PDIF01"])
 
         self.metadata["global_metrics"]["PDIF_sig"] = (
-            f"Significant at p={self.args.p_thresh}"
-            if pdif <= self.args.p_thresh
-            else f"Not significant at p={self.args.p_thresh}"
+            f"Significant at p={self.p_thresh}"
+            if pdif <= self.p_thresh
+            else f"Not significant at p={self.p_thresh}"
         )
 
         auc_p, auc_std = metrics.auc_p_val(
             self.attack_metrics[0]["AUC"],
             self.attack_metrics[0]["n_pos_test_examples"],
             self.attack_metrics[0]["n_neg_test_examples"],
         )
         self.metadata["global_metrics"]["AUC_sig"] = (
-            f"Significant at p={self.args.p_thresh}"
-            if auc_p <= self.args.p_thresh
-            else f"Not significant at p={self.args.p_thresh}"
+            f"Significant at p={self.p_thresh}"
+            if auc_p <= self.p_thresh
+            else f"Not significant at p={self.p_thresh}"
         )
         self.metadata["global_metrics"][
             "null_auc_3sd_range"
         ] = f"{0.5 - 3 * auc_std} -> {0.5 + 3 * auc_std}"
 
         self.metadata["attack"] = str(self)
 
     def make_report(self) -> dict:
-        """Create the report
+        """Create the report.
 
         Creates the output report. If self.args.report_name is not None, it will also save the
         information in json and pdf formats
 
         Returns
         -------
 
-        output: Dict
+        output : Dict
             Dictionary containing all attack output
         """
         logger = logging.getLogger("reporting")
-        logger.info("Starting report, report_name = %s", self.args.report_name)
+        report_dest = os.path.join(self.output_dir, self.report_name)
+        logger.info(
+            "Starting reports, pdf report name = %s, json report name = %s",
+            report_dest + ".pdf",
+            report_dest + ".json",
+        )
         output = {}
         output["log_id"] = str(uuid.uuid4())
         output["log_time"] = datetime.now().strftime("%d/%m/%Y %H:%M:%S")
         self._construct_metadata()
         output["metadata"] = self.metadata
         output["attack_experiment_logger"] = self._get_attack_metrics_instances()
 
-        if self.args.report_name is not None:
-            json_report = report.create_json_report(output)
-            with open(f"{self.args.report_name}.json", "w", encoding="utf-8") as f:
-                f.write(json_report)
-            logger.info("Wrote report to %s", f"{self.args.report_name}.json")
-
-            pdf_report = report.create_lr_report(output)
-            pdf_report.output(f"{self.args.report_name}.pdf", "F")
-            logger.info("Wrote pdf report to %s", f"{self.args.report_name}.pdf")
+        json_attack_formatter = GenerateJSONModule(report_dest + ".json")
+        json_report = report.create_json_report(output)
+        json_attack_formatter.add_attack_output(json_report, "LikelihoodAttack")
+
+        pdf_report = report.create_lr_report(output)
+        report.add_output_to_pdf(report_dest, pdf_report, "LikelihoodAttack")
+        logger.info(
+            "Wrote pdf report to %s and json report to %s",
+            report_dest + ".pdf",
+            report_dest + ".json",
+        )
+
         return output
 
     def _get_attack_metrics_instances(self) -> dict:
-        """Constructs the metadata object, after attacks"""
+        """Constructs the metadata object, after attacks."""
         attack_metrics_experiment = {}
         attack_metrics_instances = {}
 
         for rep, _ in enumerate(self.attack_metrics):
             self.attack_metrics[rep][
                 "n_shadow_models_trained"
             ] = self.attack_failfast_shadow_models_trained
@@ -503,88 +538,108 @@
             "target_model_hyp": {"min_samples_split": 2, "min_samples_leaf": 1},
         }
 
         with open("config.json", "w", encoding="utf-8") as f:
             f.write(json.dumps(config))
 
     def attack_from_config(self) -> None:  # pylint: disable = too-many-locals
-        """Runs an attack based on the args parsed from the command line"""
+        """Runs an attack based on the args parsed from the command line."""
         logger = logging.getLogger("run-attack")
-        logger.info(
-            "Loading training data csv from %s", self.args.training_data_filename
-        )
-        training_data = np.loadtxt(self.args.training_data_filename, delimiter=",")
+        logger.info("Loading training data csv from %s", self.training_data_filename)
+        training_data = np.loadtxt(self.training_data_filename, delimiter=",")
         train_X = training_data[:, :-1]
         train_y = training_data[:, -1].flatten().astype(int)
         logger.info("Loaded %d rows", len(train_X))
 
-        logger.info("Loading test data csv from %s", self.args.test_data_filename)
-        test_data = np.loadtxt(self.args.test_data_filename, delimiter=",")
+        logger.info("Loading test data csv from %s", self.test_data_filename)
+        test_data = np.loadtxt(self.test_data_filename, delimiter=",")
         test_X = test_data[:, :-1]
         test_y = test_data[:, -1].flatten().astype(int)
         logger.info("Loaded %d rows", len(test_X))
 
-        logger.info(
-            "Loading train predictions form %s", self.args.training_preds_filename
-        )
-        train_preds = np.loadtxt(self.args.training_preds_filename, delimiter=",")
+        logger.info("Loading train predictions form %s", self.training_preds_filename)
+        train_preds = np.loadtxt(self.training_preds_filename, delimiter=",")
         assert len(train_preds) == len(train_X)
 
-        logger.info("Loading test predictions form %s", self.args.test_preds_filename)
-        test_preds = np.loadtxt(self.args.test_preds_filename, delimiter=",")
+        logger.info("Loading test predictions form %s", self.test_preds_filename)
+        test_preds = np.loadtxt(self.test_preds_filename, delimiter=",")
         assert len(test_preds) == len(test_X)
-
-        clf_module_name, clf_class_name = self.args.target_model
-        module = importlib.import_module(clf_module_name)
-        clf_class = getattr(module, clf_class_name)
-        clf_params = self.args.target_model_hyp
-        clf = clf_class(**clf_params)
+        if self.target_model is not None:
+            clf_module_name, clf_class_name = self.target_model
+            module = importlib.import_module(clf_module_name)
+            clf_class = getattr(module, clf_class_name)
+            if self.target_model_hyp is not None:
+                clf_params = self.target_model_hyp
+                clf = clf_class(**clf_params)
         logger.info("Created model: %s", str(clf))
         self.run_scenario_from_preds(
             clf, train_X, train_y, train_preds, test_X, test_y, test_preds
         )
         logger.info("Computing metrics")
 
 
 # Methods invoked by command line script
 def _setup_example_data(args):
-    """Call the methods to setup some example data"""
-    lira_args = LIRAAttackArgs(**args.__dict__)
-    attack_obj = LIRAAttack(lira_args)
+    """Call the methods to setup some example data."""
+    attack_obj = LIRAAttack(
+        n_shadow_models=args.n_shadow_models,
+        n_shadow_rows_confidences_min=args.n_shadow_rows_confidences_min,
+        output_dir=args.output_dir,
+        report_name=args.report_name,
+        p_thresh=args.p_thresh,
+        shadow_models_fail_fast=args.shadow_models_fail_fast,
+    )
     attack_obj.setup_example_data()
 
 
 def _example(args):
-    """Call the methods to run an example"""
-    lira_args = LIRAAttackArgs(**args.__dict__)
-    attack_obj = LIRAAttack(lira_args)
+    """Call the methods to run an example."""
+    attack_obj = LIRAAttack(
+        n_shadow_models=args.n_shadow_models,
+        n_shadow_rows_confidences_min=args.n_shadow_rows_confidences_min,
+        output_dir=args.output_dir,
+        report_name=args.report_name,
+        p_thresh=args.p_thresh,
+        shadow_models_fail_fast=args.shadow_models_fail_fast,
+    )
     attack_obj.example()
     attack_obj.make_report()
 
 
 def _run_attack(args):
-    """Run a command line attack based on saved files described in .json file"""
-    lira_args = LIRAAttackArgs(**args.__dict__)
-    attack_obj = LIRAAttack(lira_args)
+    """Run a command line attack based on saved files described in .json file."""
+    # attack_obj = LIRAAttack(**args.__dict__)
+    attack_obj = LIRAAttack(
+        n_shadow_models=args.n_shadow_models,
+        n_shadow_rows_confidences_min=args.n_shadow_rows_confidences_min,
+        p_thresh=args.p_thresh,
+        output_dir=args.output_dir,
+        report_name=args.report_name,
+        shadow_models_fail_fast=args.shadow_models_fail_fast,
+        attack_config_json_file_name=args.attack_config_json_file_name,
+    )
     attack_obj.attack_from_config()
     attack_obj.make_report()
 
 
 def _run_attack_from_configfile(args):
-    """Run a command line attack based on saved files described in .json file"""
-    lira_args = LIRAAttackArgs(
-        attack_config_json_file_name=str(args.attack_config_json_file_name),
+    """Run a command line attack based on saved files described in .json file."""
+    attack_obj = LIRAAttack(
+        attack_config_json_file_name=args.attack_config_json_file_name,
+        target_path=str(args.target_path),
     )
-    attack_obj = LIRAAttack(lira_args)
-    attack_obj.attack_from_config()
+    print(args.attack_config_json_file_name)
+    target = Target()
+    target.load(attack_obj.target_path)
+    attack_obj.attack(target)
     attack_obj.make_report()
 
 
 def main():
-    """Main method to parse args and invoke relevant code"""
+    """Main method to parse args and invoke relevant code."""
     parser = argparse.ArgumentParser(add_help=False)
     parser.add_argument(
         "-s",
         "--n-shadow-models",
         type=int,
         required=False,
         default=N_SHADOW_MODELS,
@@ -603,22 +658,36 @@
         help=(
             """Number of confidences against rows in shadow data from the shadow models
             and works when --shadow-models-fail-fast = True. Default = %(default)d"""
         ),
     )
 
     parser.add_argument(
+        "--output-dir",
+        type=str,
+        action="store",
+        dest="output_dir",
+        default="output_lira",
+        required=False,
+        help=("Directory name where output files are stored. Default = %(default)s."),
+    )
+
+    parser.add_argument(
         "--report-name",
         type=str,
         action="store",
         dest="report_name",
+        default="report_lira",
         required=False,
-        default="lr_report",
-        help=("Output name for the report. Default = %(default)s"),
+        help=(
+            """Filename for the pdf and json output reports. Default = %(default)s.
+            Code will append .pdf and .json"""
+        ),
     )
+
     parser.add_argument(
         "-p",
         "--p-thresh",
         type=float,
         action="store",
         dest="p_thresh",
         required=False,
@@ -666,14 +735,28 @@
         type=str,
         default="config_lira_cmd.json",
         help=(
             "Name of the .json file containing details for the run. Default = %(default)s"
         ),
     )
 
+    attack_parser_config.add_argument(
+        "-t",
+        "--attack-target-folder-path",
+        action="store",
+        required=True,
+        dest="target_path",
+        type=str,
+        default="lira_target",
+        help=(
+            """Name of the target directory to load the trained target model and the target data.
+            Default = %(default)s"""
+        ),
+    )
+
     attack_parser_config.set_defaults(func=_run_attack_from_configfile)
 
     example_data_parser = subparsers.add_parser("setup-example-data")
     example_data_parser.set_defaults(func=_setup_example_data)
 
     args = parser.parse_args()
     try:
```

### Comparing `aisdc-1.0.5.post1/aisdc/attacks/report.py` & `aisdc-1.0.6/aisdc/attacks/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-"""Code for automatic report generation"""
+"""Code for automatic report generation."""
 import abc
 import json
+import os
 
 import numpy as np
 import pylab as plt
 from fpdf import FPDF
+from pypdf import PdfWriter
 
 # Adds a border to all pdf cells of set to 1 -- useful for debugging
 BORDER = 0
 
 DISPLAY_METRICS = [
     "AUC",
     "ACC",
@@ -70,83 +72,83 @@
         "being in the training set."
     ),
     "ACC": "The proportion of predictions that the attacker makes that are correct.",
 }
 
 
 class NumpyArrayEncoder(json.JSONEncoder):
-    """Json encoder that can cope with numpy arrays"""
+    """Json encoder that can cope with numpy arrays."""
 
     def default(self, o):
-        """If an object is an np.ndarray, convert to list"""
+        """If an object is an np.ndarray, convert to list."""
         if isinstance(o, np.ndarray):
             return o.tolist()
         if isinstance(o, np.int64):
             return int(o)
         if isinstance(o, np.int32):
             return int(o)
         if isinstance(o, abc.ABCMeta):
             return str(o)
         return json.JSONEncoder.default(self, o)
 
 
 def _write_dict(pdf, input_dict, indent=0, border=BORDER):
-    """Write a dictionary to the pdf"""
+    """Write a dictionary to the pdf."""
     for key, value in input_dict.items():
         pdf.set_font("arial", "B", 14)
         pdf.cell(75, 5, key, border, 1, "L")
         pdf.cell(indent, 0)
         pdf.set_font("arial", "", 12)
         pdf.multi_cell(150, 5, value, border, "L")
         pdf.ln(h=5)
 
 
 def title(pdf, text, border=BORDER, font_size=24, font_style="B"):
-    """Write a title block"""
+    """Write a title block."""
     pdf.set_font("arial", font_style, font_size)
     pdf.ln(h=5)
     pdf.cell(0, 0, text, border, 1, "C")
     pdf.ln(h=5)
 
 
 def subtitle(
     pdf, text, indent=10, border=BORDER, font_size=12, font_style="B"
 ):  # pylint: disable = too-many-arguments
-    """Write a subtitle block"""
+    """Write a subtitle block."""
     pdf.cell(indent, border=border)
     pdf.set_font("arial", font_style, font_size)
     pdf.cell(75, 10, text, border, 1)
 
 
 def line(
     pdf, text, indent=0, border=BORDER, font_size=11, font_style="", font="arial"
 ):  # pylint: disable = too-many-arguments
-    """Write a standard block"""
+    """Write a standard block."""
     if indent > 0:
         pdf.cell(indent, border=border)
     pdf.set_font(font, font_style, font_size)
     pdf.multi_cell(0, 5, text, border, 1)
 
 
 def _roc_plot_single(metrics, save_name):
-    """Create a roc_plot for a single experiment"""
+    """Create a roc_plot for a single experiment."""
     plt.figure()
     plt.plot([0, 1], [0, 1], "k--")
     plt.plot(metrics["fpr"], metrics["tpr"], "r", linewidth=2)
     plt.xscale("log")
     plt.yscale("log")
     plt.grid()
     plt.xlabel("True Positive Rate")
     plt.ylabel("False Positive Rate")
     plt.tight_layout()
     plt.savefig(save_name)
 
 
 def _roc_plot(metrics, dummy_metrics, save_name):
-    """Create a roc plot for multiple repetitions"""
+    """Create a roc plot for multiple repetitions."""
     plt.figure()
     plt.plot([0, 1], [0, 1], "k--")
     if dummy_metrics is None or len(dummy_metrics) == 0:
         do_dummy = False
     else:
         do_dummy = True
 
@@ -191,37 +193,36 @@
     plt.ylabel("True Positive Rate")
     plt.tight_layout()
     plt.grid()
     plt.savefig(save_name)
 
 
 def create_mia_report(attack_output: dict) -> FPDF:
-    """make a worst case membership inference report
+    """Make a worst case membership inference report.
 
     Parameters
     ----------
 
-    attack_output: dict
+    attack_output : dict
         dictionary with following items
 
             metadata: dict
                 dictionary of metadata
 
             attack_experiment_logger: dict
                 list of metrics as dictionary items for an experiment
 
             dummy_attack_experiment_logger: dict
                 list of metrics as dictionary items across dummy experiments
 
     Returns
     -------
 
-    pdf: fpdf.FPDF
+    pdf : fpdf.FPDF
         fpdf document object
-
     """
     # dummy_metrics = attack_output["dummy_attack_metrics"]
     dummy_metrics = []
     mia_metrics = [
         v
         for _, v in attack_output["attack_experiment_logger"][
             "attack_instance_logger"
@@ -230,15 +231,22 @@
     # mia_metrics = attack_output["attack_metrics"]
     metadata = attack_output["metadata"]
     if dummy_metrics is None or len(dummy_metrics) == 0:
         do_dummy = False
     else:
         do_dummy = True
 
-    _roc_plot(mia_metrics, dummy_metrics, "log_roc.png")
+    dest_log_roc = (
+        os.path.join(
+            metadata["experiment_details"]["output_dir"],
+            metadata["experiment_details"]["report_name"],
+        )
+        + "_log_roc.png"
+    )
+    _roc_plot(mia_metrics, dummy_metrics, dest_log_roc)
 
     pdf = FPDF()
     pdf.add_page()
     pdf.set_xy(0, 0)
     title(pdf, "WorstCase MIA attack result report")
     subtitle(pdf, "Introduction")
     line(pdf, INTRODUCTION)
@@ -287,65 +295,97 @@
                 vals = np.array([MAPPINGS[metric](v) for v in vals])
             text = (
                 f"{metric:>12} mean = {vals.mean():.2f}, var = {vals.var():.4f}, "
                 f"min = {vals.min():.2f}, max = {vals.max():.2f}"
             )
             line(pdf, text, font="courier")
 
-    pdf.add_page()
-    subtitle(pdf, "Log ROC")
-    pdf.image("log_roc.png", x=None, y=None, w=0, h=140, type="", link="")
-    pdf.set_font("arial", "", 12)
+    _add_log_roc_to_page(dest_log_roc, pdf)
     line(pdf, LOGROC_CAPTION)
 
     pdf.add_page()
     title(pdf, "Glossary")
     _write_dict(pdf, GLOSSARY)
 
     return pdf
 
 
+def add_output_to_pdf(report_dest: str, pdf_report: FPDF, attack_type: str) -> None:
+    """Creates pdf and appends contents if it already exists."""
+    if os.path.exists(report_dest + ".pdf"):
+        old_pdf = report_dest + ".pdf"
+        new_pdf = report_dest + "_new.pdf"
+        pdf_report.output(new_pdf)
+        merger = PdfWriter()
+        for pdf in [old_pdf, new_pdf]:
+            merger.append(pdf)
+        merger.write(old_pdf)
+        merger.close()
+        os.remove(new_pdf)
+    else:
+        pdf_report.output(report_dest + ".pdf")
+    if attack_type in ("WorstCaseAttack", "LikelihoodAttack"):
+        os.remove(report_dest + "_log_roc.png")
+    elif attack_type == "AttributeAttack":
+        os.remove(report_dest + "_cat_frac.png")
+        os.remove(report_dest + "_cat_risk.png")
+
+
+def _add_log_roc_to_page(log_roc: str = None, pdf_obj: FPDF = None):
+    if log_roc is not None:
+        pdf_obj.add_page()
+        subtitle(pdf_obj, "Log ROC")
+        pdf_obj.image(log_roc, x=None, y=None, w=0, h=140, type="", link="")
+        pdf_obj.set_font("arial", "", 12)
+
+
 def create_json_report(output):
-    """Create a report in json format for injestion by other tools"""
+    """Create a report in json format for injestion by other tools."""
     # Initial work, just dump mia_metrics and dummy_metrics into a json structure
     return json.dumps(output, cls=NumpyArrayEncoder)
 
 
 def create_lr_report(output: dict) -> FPDF:
-    """make a lira membership inference report
+    """Make a lira membership inference report.
 
     Parameters
     ----------
 
-    output: dict
+    output : dict
         dictionary with following items
 
         metadata: dict
                 dictionary of metadata
 
         attack_experiment_logger: dict
             list of metrics as dictionary items for an experiments
             In case of LIRA attack scenario, this will have dictionary
             items of attack_instance_logger that
             will have a single metrics dictionary
 
     Returns
     -------
 
-    pdf: fpdf.FPDF
+    pdf : fpdf.FPDF
         fpdf document object
-
     """
     mia_metrics = [
         v
         for _, v in output["attack_experiment_logger"]["attack_instance_logger"].items()
     ][0]
     # mia_metrics = output["attack_metrics"][0]
     metadata = output["metadata"]
-    _roc_plot_single(mia_metrics, "log_roc.png")
+    dest_log_roc = (
+        os.path.join(
+            metadata["experiment_details"]["output_dir"],
+            metadata["experiment_details"]["report_name"],
+        )
+        + "_log_roc.png"
+    )
+    _roc_plot_single(mia_metrics, dest_log_roc)
     pdf = FPDF()
     pdf.add_page()
     pdf.set_xy(0, 0)
     title(pdf, "Likelihood Ratio Attack Report")
     subtitle(pdf, "Introduction")
     subtitle(pdf, "Metadata")
     for key, value in metadata["experiment_details"].items():
@@ -356,11 +396,12 @@
     sub_metrics_dict = {
         key: val for key, val in mia_metrics.items() if isinstance(val, float)
     }
     for key, value in sub_metrics_dict.items():
         if key in MAPPINGS:
             value = MAPPINGS[key](value)
         line(pdf, f"{key:>30s}: {value:.4f}", font="courier")
+
     pdf.add_page()
     subtitle(pdf, "ROC Curve")
-    pdf.image("log_roc.png", x=None, y=None, w=0, h=140, type="", link="")
+    pdf.image(dest_log_roc, x=None, y=None, w=0, h=140, type="", link="")
     return pdf
```

### Comparing `aisdc-1.0.5.post1/aisdc/attacks/worst_case_attack.py` & `aisdc-1.0.6/aisdc/attacks/worst_case_attack.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,164 +1,232 @@
 """
-worst_case_attack.py
+Worst_case_attack.py.
 
 Runs a worst case attack based upon predictive probabilities stored in two .csv files
 """
 
 from __future__ import annotations
 
 import argparse
 import logging
+import os
 import uuid
-from collections.abc import Hashable
 from datetime import datetime
 from typing import Any
 
 import numpy as np
-import sklearn
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.metrics import confusion_matrix
 from sklearn.model_selection import train_test_split
 
 from aisdc import metrics
 from aisdc.attacks import report
-from aisdc.attacks.attack import Attack, ConfigFile
-from aisdc.attacks.dataset import Data
+from aisdc.attacks.attack import Attack
+from aisdc.attacks.attack_report_formatter import GenerateJSONModule
 from aisdc.attacks.failfast import FailFast
+from aisdc.attacks.target import Target
 
 logging.basicConfig(level=logging.INFO)
 
 P_THRESH = 0.05
 
 
-class WorstCaseAttackArgs:
-    """Arguments for worst case"""
-
-    def __init__(self, **kwargs):
-        self.__dict__["n_reps"] = 10
-        self.__dict__["p_thresh"] = 0.05
-        self.__dict__["n_dummy_reps"] = 1
-        self.__dict__["train_beta"] = 2
-        self.__dict__["test_beta"] = 2
-        self.__dict__["test_prop"] = 0.3
-        self.__dict__["n_rows_in"] = 1000
-        self.__dict__["n_rows_out"] = 1000
-        self.__dict__["training_preds_filename"] = None
-        self.__dict__["test_preds_filename"] = None
-        self.__dict__["report_name"] = None
-        self.__dict__["include_model_correct_feature"] = False
-        self.__dict__["sort_probs"] = True
-        self.__dict__["mia_attack_model"] = RandomForestClassifier
-        self.__dict__["mia_attack_model_hyp"] = {
-            "min_samples_split": 20,
-            "min_samples_leaf": 10,
-            "max_depth": 5,
-        }
-        self.__dict__["attack_metric_success_name"] = "P_HIGHER_AUC"
-        self.__dict__["attack_metric_success_thresh"] = 0.05
-        self.__dict__["attack_metric_success_comp_type"] = "lte"
-        self.__dict__["attack_metric_success_count_thresh"] = 5
-        self.__dict__["attack_fail_fast"] = False
-        self.__dict__["attack_config_json_file_name"] = None
-        self.__dict__.update(kwargs)
-        # Reading parameters from a json file
-        if self.__dict__["attack_config_json_file_name"] is not None:
-            configfile_obj = ConfigFile(self.__dict__["attack_config_json_file_name"])
-            configfile_obj.load_config_file_into_dict(self.__dict__)
-        # deleted for not enabling to appear in the output file
-        del self.__dict__["attack_config_json_file_name"]
-
-    def __str__(self):
-        return ",".join(
-            [f"{str(key)}: {str(value)}" for key, value in self.__dict__.items()]
-        )
-
-    def set_param(self, key: Hashable, value: Any) -> None:
-        """Set a parameter"""
-        self.__dict__[key] = value
-
-    def get_args(self) -> dict:
-        """Return arguments"""
-        return self.__dict__
+class WorstCaseAttack(Attack):
+    """Class to wrap the worst case attack code."""
 
+    # pylint: disable=too-many-instance-attributes
 
-class WorstCaseAttack(Attack):
-    """Class to wrap the worst case attack code"""
+    def __init__(  # pylint: disable = too-many-arguments, too-many-locals
+        self,
+        n_reps: int = 10,
+        p_thresh: float = 0.05,
+        n_dummy_reps: int = 1,
+        train_beta: int = 1,
+        test_beta: int = 1,
+        test_prop: float = 0.2,
+        n_rows_in: int = 1000,
+        n_rows_out: int = 1000,
+        training_preds_filename: str = None,
+        test_preds_filename: str = None,
+        output_dir: str = "output_worstcase",
+        report_name: str = "report_worstcase",
+        include_model_correct_feature: bool = False,
+        sort_probs: bool = True,
+        mia_attack_model: Any = RandomForestClassifier,
+        mia_attack_model_hyp: dict = None,
+        attack_metric_success_name: str = "P_HIGHER_AUC",
+        attack_metric_success_thresh: float = 0.05,
+        attack_metric_success_comp_type: str = "lte",
+        attack_metric_success_count_thresh: int = 5,
+        attack_fail_fast: bool = False,
+        attack_config_json_file_name: str = None,
+        target_path: str = None,
+    ) -> None:
+        """Constructs an object to execute a worst case attack.
 
-    def __init__(self, args: WorstCaseAttackArgs = WorstCaseAttackArgs()):
+        Parameters
+        ----------
+        n_reps : int
+            number of attacks to run -- in each iteration an attack model
+            is trained on a different subset of the data
+        p_thresh : float
+            threshold to determine significance of things. For instance auc_p_value and pdif_vals
+        n_dummy_reps : int
+            number of baseline (dummy) experiments to do
+        train_beta : int
+            value of b for beta distribution used to sample the in-sample (training) probabilities
+        test_beta : int
+            value of b for beta distribution used to sample the out-of-sample (test) probabilities
+        test_prop : float
+            proportion of data to use as a test set for the attack model
+        n_rows_in : int
+            number of rows for in-sample (training data)
+        n_rows_out : int
+            number of rows for out-of-sample (test data)
+        training_preds_filename : str
+            name of the file to keep predictions of the training data (in-sample)
+        test_preds_filename : str
+            name of the file to keep predictions of the test data (out-of-sample)
+        output_dir : str
+            name of the directory where outputs are stored
+        report_name : str
+            name of the pdf and json output reports
+        include_model_correct_feature : bool
+            inclusion of additional feature to hold whether or not the target model
+            made a correct prediction for each example
+        sort_probs : bool
+            true in case require to sort combine preds (from training and test)
+            to have highest probabilities in the first column
+        mia_attack_model : Any
+            name of the attack model such as RandomForestClassifier
+        mia_attack_model_hyp : dict
+            dictionary of hyper parameters for the mia_attack_model
+            such as min_sample_split, min_samples_leaf etc
+        attack_metric_success_name : str
+            name of metric to compute for the attack being successful
+        attack_metric_success_thresh : float
+            threshold for a given metric to measure attack being successful or not
+        attack_metric_success_comp_type : str
+            threshold comparison operator (i.e., gte: greater than or equal to, gt:
+            greater than, lte: less than or equal to, lt: less than,
+            eq: equal to and not_eq: not equal to)
+        attack_metric_success_count_thresh : int
+            a counter to record how many times an attack was successful
+            given that the threshold has fulfilled criteria for a given comparison type
+        attack_fail_fast : bool
+            If true it stops repetitions earlier based on the given attack metric
+            (i.e., attack_metric_success_name) considering the comparison type
+            (attack_metric_success_comp_type) satisfying a threshold
+            (i.e., attack_metric_success_thresh) for n
+            (attack_metric_success_count_thresh) number of times
+        attack_config_json_file_name : str
+            name of the configuration file to load parameters
+        target_path : str
+            path to the saved trained target model and target data
+        """
+
+        super().__init__()
+        self.n_reps = n_reps
+        self.p_thresh = p_thresh
+        self.n_dummy_reps = n_dummy_reps
+        self.train_beta = train_beta
+        self.test_beta = test_beta
+        self.test_prop = test_prop
+        self.n_rows_in = n_rows_in
+        self.n_rows_out = n_rows_out
+        self.training_preds_filename = training_preds_filename
+        self.test_preds_filename = test_preds_filename
+        self.output_dir = output_dir
+        self.report_name = report_name
+        self.include_model_correct_feature = include_model_correct_feature
+        self.sort_probs = sort_probs
+        self.mia_attack_model = mia_attack_model
+        if mia_attack_model_hyp is None:
+            self.mia_attack_model_hyp = {
+                "min_samples_split": 20,
+                "min_samples_leaf": 10,
+                "max_depth": 5,
+            }
+        else:
+            self.mia_attack_model_hyp = mia_attack_model_hyp
+        self.attack_metric_success_name = attack_metric_success_name
+        self.attack_metric_success_thresh = attack_metric_success_thresh
+        self.attack_metric_success_comp_type = attack_metric_success_comp_type
+        self.attack_metric_success_count_thresh = attack_metric_success_count_thresh
+        self.attack_fail_fast = attack_fail_fast
+        self.attack_config_json_file_name = attack_config_json_file_name
+        self.target_path = target_path
+        # Updating parameters from a configuration json file
+        if self.attack_config_json_file_name is not None:
+            self._update_params_from_config_file()
+        if not os.path.exists(self.output_dir):
+            os.makedirs(self.output_dir)
         self.attack_metrics = None
         self.attack_metric_failfast_summary = None
         self.dummy_attack_metrics = None
         self.dummy_attack_metric_failfast_summary = None
         self.metadata = None
-        self.args = args
 
     def __str__(self):
         return "WorstCase attack"
 
-    def attack(self, dataset: Data, target_model: sklearn.base.BaseEstimator) -> None:
-        """Programmatic attack entry point
+    def attack(self, target: Target) -> None:
+        """Programmatic attack entry point.
 
-        To be used when code has access to data class and trained target model
+        To be used when code has access to Target class and trained target model
 
         Parameters
         ----------
-        dataset: attacks.dataset.Data
-            dataset as a Data class object
-        target_model: sklearn.base.BaseEstimator
-            target model that inherits from an sklearn BaseEstimator
+        target : attacks.target.Target
+            target as a Target class object
         """
-        train_preds = target_model.predict_proba(dataset.x_train)
-        test_preds = target_model.predict_proba(dataset.x_test)
+        train_preds = target.model.predict_proba(target.x_train)
+        test_preds = target.model.predict_proba(target.x_test)
         train_correct = None
         test_correct = None
-        if self.args.include_model_correct_feature:
-            train_correct = 1 * (
-                dataset.y_train == target_model.predict(dataset.x_train)
-            )
-            test_correct = 1 * (dataset.y_test == target_model.predict(dataset.x_test))
+        if self.include_model_correct_feature:
+            train_correct = 1 * (target.y_train == target.model.predict(target.x_train))
+            test_correct = 1 * (target.y_test == target.model.predict(target.x_test))
 
         self.attack_from_preds(
             train_preds,
             test_preds,
             train_correct=train_correct,
             test_correct=test_correct,
         )
 
     def attack_from_prediction_files(self):
-        """Start an attack from saved prediction files
+        """Start an attack from saved prediction files.
 
         To be used when only saved predictions are available.
 
         Filenames for the saved prediction files to be specified in the arguments provided
         in the constructor
         """
-        train_preds = np.loadtxt(self.args.training_preds_filename, delimiter=",")
-        test_preds = np.loadtxt(self.args.test_preds_filename, delimiter=",")
+        train_preds = np.loadtxt(self.training_preds_filename, delimiter=",")
+        test_preds = np.loadtxt(self.test_preds_filename, delimiter=",")
         self.attack_from_preds(train_preds, test_preds)
 
     def attack_from_preds(  # pylint: disable=too-many-locals
         self,
         train_preds: np.ndarray,
         test_preds: np.ndarray,
         train_correct: np.ndarray = None,
         test_correct: np.ndarray = None,
     ) -> None:
         """
         Runs the attack based upon the predictions in train_preds and test_preds, and the params
-        stored in self.args
+        stored in self.args.
 
         Parameters
         ----------
-
-        train_preds: np.ndarray
+        train_preds : np.ndarray
             Array of train predictions. One row per example, one column per class (i.e. 2)
-        test_preds:  np.ndarray
+        test_preds : np.ndarray
             Array of test predictions. One row per example, one column per class (i.e. 2)
-
         """
         logger = logging.getLogger("attack-from-preds")
         logger.info("Running main attack repetitions")
         attack_metric_dict = self.run_attack_reps(
             train_preds,
             test_preds,
             train_correct=train_correct,
@@ -167,21 +235,24 @@
         self.attack_metrics = attack_metric_dict["mia_metrics"]
         self.attack_metric_failfast_summary = attack_metric_dict[
             "failfast_metric_summary"
         ]
 
         self.dummy_attack_metrics = []
         self.dummy_attack_metric_failfast_summary = []
-        if self.args.n_dummy_reps > 0:
+        if self.n_dummy_reps > 0:
             logger.info("Running dummy attack reps")
             n_train_rows = len(train_preds)
             n_test_rows = len(test_preds)
-            for _ in range(self.args.n_dummy_reps):
+            for _ in range(self.n_dummy_reps):
                 d_train_preds, d_test_preds = self.generate_arrays(
-                    n_train_rows, n_test_rows, self.args.train_beta, self.args.test_beta
+                    n_train_rows,
+                    n_test_rows,
+                    self.train_beta,
+                    self.test_beta,
                 )
                 temp_attack_metric_dict = self.run_attack_reps(
                     d_train_preds, d_test_preds
                 )
                 temp_metrics = temp_attack_metric_dict["mia_metrics"]
                 temp_metric_failfast_summary = temp_attack_metric_dict[
                     "failfast_metric_summary"
@@ -200,24 +271,25 @@
         test_preds: np.ndarray,
         train_correct: np.ndarray = None,
         test_correct: np.ndarray = None,
     ) -> tuple[np.ndarray, np.ndarray]:
         """Prepare training data and labels for attack model
         Combines the train and test preds into a single numpy array (optionally) sorting each
         row to have the highest probabilities in the first column. Constructs a label array that
-        has ones corresponding to training rows and zeros to testing rows."""
+        has ones corresponding to training rows and zeros to testing rows.
+        """
         logger = logging.getLogger("prep-attack-data")
-        if self.args.sort_probs:
+        if self.sort_probs:
             logger.info("Sorting probabilities to leave highest value in first column")
             train_preds = -np.sort(-train_preds, axis=1)
             test_preds = -np.sort(-test_preds, axis=1)
 
         logger.info("Creating MIA data")
 
-        if self.args.include_model_correct_feature and train_correct is not None:
+        if self.include_model_correct_feature and train_correct is not None:
             train_preds = np.hstack((train_preds, train_correct[:, None]))
             test_preds = np.hstack((test_preds, test_correct[:, None]))
 
         mi_x = np.vstack((train_preds, test_preds))
         mi_y = np.hstack((np.ones(len(train_preds)), np.zeros(len(test_preds))))
 
         return (mi_x, mi_y)
@@ -226,130 +298,125 @@
         self,
         train_preds: np.ndarray,
         test_preds: np.ndarray,
         train_correct: np.ndarray = None,
         test_correct: np.ndarray = None,
     ) -> dict:
         """
-        Run actual attack reps from train and test predictions
+        Run actual attack reps from train and test predictions.
 
         Parameters
         ----------
-        train_preds: np.ndarray
+        train_preds : np.ndarray
             predictions from the model on training (in-sample) data
-        test_preds: np.ndarray
+        test_preds : np.ndarray
             predictions from the model on testing (out-of-sample) data
 
         Returns
         -------
-        mia_metrics_dict: dict
+        mia_metrics_dict : dict
             a dictionary with two items including mia_metrics
             (a list of metric across repetitions) and failfast_metric_summary object
             (an object of FailFast class) to maintain summary of
             fail/success of attacks for a given metric of failfast option
         """
-        self.args.set_param("n_rows_in", len(train_preds))
-        self.args.set_param("n_rows_out", len(test_preds))
+        self.n_rows_in = len(train_preds)
+        self.n_rows_out = len(test_preds)
         logger = logging.getLogger("attack-reps")
         mi_x, mi_y = self._prepare_attack_data(
             train_preds, test_preds, train_correct, test_correct
         )
 
         mia_metrics = []
 
-        failfast_metric_summary = FailFast(self.args)
+        failfast_metric_summary = FailFast(self)
 
-        for rep in range(self.args.n_reps):
-            logger.info("Rep %d of %d", rep + 1, self.args.n_reps)
+        for rep in range(self.n_reps):
+            logger.info("Rep %d of %d", rep + 1, self.n_reps)
             mi_train_x, mi_test_x, mi_train_y, mi_test_y = train_test_split(
-                mi_x, mi_y, test_size=self.args.test_prop, stratify=mi_y
-            )
-            attack_classifier = self.args.mia_attack_model(
-                **self.args.mia_attack_model_hyp
+                mi_x, mi_y, test_size=self.test_prop, stratify=mi_y
             )
+            attack_classifier = self.mia_attack_model(**self.mia_attack_model_hyp)
             attack_classifier.fit(mi_train_x, mi_train_y)
             y_pred_proba, y_test = metrics.get_probabilities(
                 attack_classifier, mi_test_x, mi_test_y, permute_rows=True
             )
 
             mia_metrics.append(metrics.get_metrics(y_pred_proba, y_test))
 
-            if self.args.include_model_correct_feature and train_correct is not None:
+            if self.include_model_correct_feature and train_correct is not None:
                 # Compute the Yeom TPR and FPR
                 yeom_preds = mi_test_x[:, -1]
                 tn, fp, fn, tp = confusion_matrix(mi_test_y, yeom_preds).ravel()
                 mia_metrics[-1]["yeom_tpr"] = tp / (tp + fn)
                 mia_metrics[-1]["yeom_fpr"] = fp / (fp + tn)
                 mia_metrics[-1]["yeom_advantage"] = (
                     mia_metrics[-1]["yeom_tpr"] - mia_metrics[-1]["yeom_fpr"]
                 )
 
             failfast_metric_summary.check_attack_success(mia_metrics[rep])
 
             if (
-                failfast_metric_summary.check_overall_attack_success(self.args)
-                and self.args.attack_fail_fast
+                failfast_metric_summary.check_overall_attack_success(self)
+                and self.attack_fail_fast
             ):
                 break
 
         logger.info("Finished simulating attacks")
 
         mia_metrics_dict = {}
         mia_metrics_dict["mia_metrics"] = mia_metrics
         mia_metrics_dict["failfast_metric_summary"] = failfast_metric_summary
 
         return mia_metrics_dict
 
     def _get_global_metrics(self, attack_metrics: list) -> dict:
-        """Summarise metrics from a metric list
-
-        Arguments
-        ---------
-        attack_metrics: List
-            list of attack metrics dictionaries
+        """Summarise metrics from a metric list.
 
         Returns
         -------
-        global_metrics: Dict
+        global_metrics : Dict
             Dictionary of summary metrics
 
+        Arguments
+        ---------
+        attack_metrics: List
+            list of attack metrics dictionaries
         """
         global_metrics = {}
-        auc_p_vals = [
-            metrics.auc_p_val(
-                m["AUC"], m["n_pos_test_examples"], m["n_neg_test_examples"]
-            )[0]
-            for m in attack_metrics
-        ]
-
-        if len(attack_metrics) == 0:
-            return global_metrics
-
-        m = attack_metrics[0]
-        _, auc_std = metrics.auc_p_val(
-            0.5, m["n_pos_test_examples"], m["n_neg_test_examples"]
-        )
+        if attack_metrics is not None and len(attack_metrics) != 0:
+            auc_p_vals = [
+                metrics.auc_p_val(
+                    m["AUC"], m["n_pos_test_examples"], m["n_neg_test_examples"]
+                )[0]
+                for m in attack_metrics
+            ]
+
+            m = attack_metrics[0]
+            _, auc_std = metrics.auc_p_val(
+                0.5, m["n_pos_test_examples"], m["n_neg_test_examples"]
+            )
 
-        global_metrics[
-            "null_auc_3sd_range"
-        ] = f"{0.5 - 3*auc_std:.4f} -> {0.5 + 3*auc_std:.4f}"
-        global_metrics["n_sig_auc_p_vals"] = self._get_n_significant(
-            auc_p_vals, self.args.p_thresh
-        )
-        global_metrics["n_sig_auc_p_vals_corrected"] = self._get_n_significant(
-            auc_p_vals, self.args.p_thresh, bh_fdr_correction=True
-        )
+            global_metrics[
+                "null_auc_3sd_range"
+            ] = f"{0.5 - 3*auc_std:.4f} -> {0.5 + 3*auc_std:.4f}"
+            global_metrics["n_sig_auc_p_vals"] = self._get_n_significant(
+                auc_p_vals, self.p_thresh
+            )
+            global_metrics["n_sig_auc_p_vals_corrected"] = self._get_n_significant(
+                auc_p_vals, self.p_thresh, bh_fdr_correction=True
+            )
 
-        pdif_vals = [np.exp(-m["PDIF01"]) for m in attack_metrics]
-        global_metrics["n_sig_pdif_vals"] = self._get_n_significant(
-            pdif_vals, self.args.p_thresh
-        )
-        global_metrics["n_sig_pdif_vals_corrected"] = self._get_n_significant(
-            pdif_vals, self.args.p_thresh, bh_fdr_correction=True
-        )
+            pdif_vals = [np.exp(-m["PDIF01"]) for m in attack_metrics]
+            global_metrics["n_sig_pdif_vals"] = self._get_n_significant(
+                pdif_vals, self.p_thresh
+            )
+            global_metrics["n_sig_pdif_vals_corrected"] = self._get_n_significant(
+                pdif_vals, self.p_thresh, bh_fdr_correction=True
+            )
 
         return global_metrics
 
     def _get_n_significant(self, p_val_list, p_thresh, bh_fdr_correction=False):
         """
         Helper method to determine if values within a list of p-values are significant at
         p_thresh. Can perform multiple testing correction.
@@ -365,34 +432,33 @@
         if any(bh_sig_list):
             n_sig_bh = (np.where(bh_sig_list)[0]).max() + 1
         else:
             n_sig_bh = 0
         return n_sig_bh
 
     def _generate_array(self, n_rows: int, beta: float) -> np.ndarray:
-        """Generate a single array of predictions, used when doing baseline experiments
+        """Generate a single array of predictions, used when doing baseline experiments.
 
         Parameters
         ----------
-        n_rows: int
+        n_rows : int
             the number of rows worth of data to generate
-        beta: float
+        beta : float
             the beta parameter for sampling probabilities
 
         Returns
         -------
-        preds: np.ndarray
+        preds : np.ndarray
             Array of predictions. Two columns, n_rows rows
 
         Notes
         -----
 
         Examples
         --------
-
         """
 
         preds = np.zeros((n_rows, 2), float)
         for row_idx in range(n_rows):
             train_class = np.random.choice(2)
             train_prob = np.random.beta(1, beta)
             preds[row_idx, train_class] = train_prob
@@ -402,115 +468,112 @@
     def generate_arrays(
         self,
         n_rows_in: int,
         n_rows_out: int,
         train_beta: float = 2,
         test_beta: float = 2,
     ) -> tuple[np.ndarray, np.ndarray]:
-        """Generate train and test prediction arrays, used when computing baseline
+        """Generate train and test prediction arrays, used when computing baseline.
 
         Parameters
         ----------
-        n_rows_in: int
+        n_rows_in : int
             number of rows of in-sample (training) probabilities
-        n_rows_out: int
+        n_rows_out : int
             number of rows of out-of-sample (testing) probabilities
-        train_beta: float
+        train_beta : float
             beta value for generating train probabilities
-        test_beta: float:
+        test_beta : float:
             beta_value for generating test probabilities
 
         Returns
         -------
-        train_preds: np.ndarray
+        train_preds : np.ndarray
             Array of train predictions (n_rows x 2 columns)
-        test_preds: np.ndarray
+        test_preds : np.ndarray
             Array of test predictions (n_rows x 2 columns)
         """
         train_preds = self._generate_array(n_rows_in, train_beta)
         test_preds = self._generate_array(n_rows_out, test_beta)
         return train_preds, test_preds
 
     def make_dummy_data(self) -> None:
-        """Makes dummy data for testing functionality
+        """Makes dummy data for testing functionality.
 
         Parameters
         ----------
-        args: dict
+        args : dict
             Command line arguments
 
         Returns
         -------
 
         Notes
         -----
-
         Returns nothing but saves two .csv files
         """
         logger = logging.getLogger("dummy-data")
         logger.info(
             "Making dummy data with %d rows in and %d out",
-            self.args.n_rows_in,
-            self.args.n_rows_out,
+            self.n_rows_in,
+            self.n_rows_out,
         )
         logger.info("Generating rows")
         train_preds, test_preds = self.generate_arrays(
-            self.args.n_rows_in,
-            self.args.n_rows_out,
-            train_beta=self.args.train_beta,
-            test_beta=self.args.test_beta,
+            self.n_rows_in,
+            self.n_rows_out,
+            train_beta=self.train_beta,
+            test_beta=self.test_beta,
         )
         logger.info("Saving files")
-        np.savetxt(self.args.training_preds_filename, train_preds, delimiter=",")
-        np.savetxt(self.args.test_preds_filename, test_preds, delimiter=",")
+        np.savetxt(self.training_preds_filename, train_preds, delimiter=",")
+        np.savetxt(self.test_preds_filename, test_preds, delimiter=",")
 
     def _construct_metadata(self):
-        """Constructs the metadata object, after attacks"""
+        """Constructs the metadata object, after attacks."""
         self.metadata = {}
         # Store all args
         self.metadata["experiment_details"] = {}
-        self.metadata["experiment_details"].update(self.args.__dict__)
-        if "func" in self.metadata["experiment_details"]:
-            del self.metadata["experiment_details"]["func"]
+        self.metadata["experiment_details"] = self.get_params()
 
         self.metadata["attack"] = str(self)
 
         # Global metrics
         self.metadata["global_metrics"] = self._get_global_metrics(self.attack_metrics)
         self.metadata["baseline_global_metrics"] = self._get_global_metrics(
             self._unpack_dummy_attack_metrics_experiments_instances()
         )
 
     def _unpack_dummy_attack_metrics_experiments_instances(self) -> list:
-        """Constructs the metadata object, after attacks"""
+        """Constructs the metadata object, after attacks."""
         dummy_attack_metrics_instances = []
 
         for exp_rep, _ in enumerate(self.dummy_attack_metrics):
             temp_dummy_attack_metrics = self.dummy_attack_metrics[exp_rep]
             dummy_attack_metrics_instances += temp_dummy_attack_metrics
 
         return dummy_attack_metrics_instances
 
     def _get_attack_metrics_instances(self) -> dict:
-        """Constructs the metadata object, after attacks"""
+        """Constructs the metadata object, after attacks."""
         attack_metrics_experiment = {}
         attack_metrics_instances = {}
 
         for rep, _ in enumerate(self.attack_metrics):
             attack_metrics_instances["instance_" + str(rep)] = self.attack_metrics[rep]
 
         attack_metrics_experiment["attack_instance_logger"] = attack_metrics_instances
         attack_metrics_experiment[
             "attack_metric_failfast_summary"
         ] = self.attack_metric_failfast_summary.get_attack_summary()
 
         return attack_metrics_experiment
 
     def _get_dummy_attack_metrics_experiments_instances(self) -> dict:
-        """Constructs the metadata object, after attacks"""
+        """Constructs the metadata object, after attacks."""
         dummy_attack_metrics_experiments = {}
 
         for exp_rep, _ in enumerate(self.dummy_attack_metrics):
             temp_dummy_attack_metrics = self.dummy_attack_metrics[exp_rep]
             dummy_attack_metric_instances = {}
             for rep, _ in enumerate(temp_dummy_attack_metrics):
                 dummy_attack_metric_instances[
@@ -524,76 +587,93 @@
             dummy_attack_metrics_experiments[
                 "dummy_attack_metrics_experiment_" + str(exp_rep)
             ] = temp
 
         return dummy_attack_metrics_experiments
 
     def make_report(self) -> dict:
-        """Creates output dictionary structure"""
+        """Creates output dictionary structure and generates
+        pdf and json outputs if filenames are given.
+        """
         output = {}
         output["log_id"] = str(uuid.uuid4())
         output["log_time"] = datetime.now().strftime("%d/%m/%Y %H:%M:%S")
 
         self._construct_metadata()
         output["metadata"] = self.metadata
 
         output["attack_experiment_logger"] = self._get_attack_metrics_instances()
         output[
             "dummy_attack_experiments_logger"
         ] = self._get_dummy_attack_metrics_experiments_instances()
 
-        # output_for_pdf = {}
-        # output_for_pdf["attack_metrics"] = self.attack_metrics
-        # output_for_pdf[
-        #     "dummy_attack_metrics"
-        # ] = self._unpack_dummy_attack_metrics_experiments_instances()
-        # output_for_pdf["metadata"] = self.metadata
-
-        if self.args.report_name is not None:
-            json_report = report.create_json_report(output)
-            with open(f"{self.args.report_name}.json", "w", encoding="utf-8") as f:
-                f.write(json_report)
-
-            # pdf_report = report.create_mia_report(output_for_pdf)
-            pdf_report = report.create_mia_report(output)
-            pdf_report.output(f"{self.args.report_name}.pdf", "F")
+        report_dest = os.path.join(self.output_dir, self.report_name)
+        json_attack_formatter = GenerateJSONModule(report_dest + ".json")
+        json_report = report.create_json_report(output)
+        json_attack_formatter.add_attack_output(json_report, "WorstCaseAttack")
 
+        pdf_report = report.create_mia_report(output)
+        report.add_output_to_pdf(report_dest, pdf_report, "WorstCaseAttack")
         return output
 
 
 def _make_dummy_data(args):
-    """Initialise class and run dummy data creation"""
-    wc_args = WorstCaseAttackArgs(**args.__dict__)
-    wc_args.set_param("training_preds_filename", "train_preds.csv")
-    wc_args.set_param("test_preds_filename", "test_preds.csv")
-    attack_obj = WorstCaseAttack(wc_args)
+    """Initialise class and run dummy data creation."""
+    args.__dict__["training_preds_filename"] = "train_preds.csv"
+    args.__dict__["test_preds_filename"] = "test_preds.csv"
+    attack_obj = WorstCaseAttack(
+        train_beta=args.train_beta,
+        test_beta=args.test_beta,
+        n_rows_in=args.n_rows_in,
+        n_rows_out=args.n_rows_out,
+        training_preds_filename=args.training_preds_filename,
+        test_preds_filename=args.test_preds_filename,
+    )
     attack_obj.make_dummy_data()
 
 
 def _run_attack(args):
-    """Initialise class and run attack from prediction files"""
-    wc_args = WorstCaseAttackArgs(**args.__dict__)
-    attack_obj = WorstCaseAttack(wc_args)
+    """Initialise class and run attack from prediction files."""
+    attack_obj = WorstCaseAttack(
+        n_reps=args.n_reps,
+        p_thresh=args.p_thresh,
+        n_dummy_reps=args.n_dummy_reps,
+        train_beta=args.train_beta,
+        test_beta=args.test_beta,
+        test_prop=args.test_prop,
+        training_preds_filename=args.training_preds_filename,
+        test_preds_filename=args.test_preds_filename,
+        output_dir=args.output_dir,
+        report_name=args.report_name,
+        sort_probs=args.sort_probs,
+        attack_metric_success_name=args.attack_metric_success_name,
+        attack_metric_success_thresh=args.attack_metric_success_thresh,
+        attack_metric_success_comp_type=args.attack_metric_success_comp_type,
+        attack_metric_success_count_thresh=args.attack_metric_success_count_thresh,
+        attack_fail_fast=args.attack_fail_fast,
+    )
+    print(attack_obj.training_preds_filename)
     attack_obj.attack_from_prediction_files()
     _ = attack_obj.make_report()
 
 
 def _run_attack_from_configfile(args):
-    """Initialise class and run attack from prediction files
-    using config file"""
-    wc_args = WorstCaseAttackArgs(
+    """Initialise class and run attack from prediction files using config file."""
+    attack_obj = WorstCaseAttack(
         attack_config_json_file_name=str(args.attack_config_json_file_name),
+        target_path=str(args.target_path),
     )
-    attack_obj = WorstCaseAttack(wc_args)
-    attack_obj.attack_from_prediction_files()
+    target = Target()
+    target.load(attack_obj.target_path)
+    attack_obj.attack(target)
     _ = attack_obj.make_report()
 
 
 def main():
-    """main method to parse arguments and invoke relevant method"""
+    """Main method to parse arguments and invoke relevant method."""
     logger = logging.getLogger("main")
     parser = argparse.ArgumentParser(
         description=("Perform a worst case attack from saved model predictions")
     )
 
     subparsers = parser.add_subparsers()
     dummy_parser = subparsers.add_parser("make-dummy-data")
@@ -623,18 +703,17 @@
         "--train-beta",
         action="store",
         type=float,
         required=False,
         default=5,
         dest="train_beta",
         help=(
-            "Value of b parameter for beta distribution used to sample the in-sample "
-            "probabilities. "
-            "High values will give more extreme probabilities. Set this value higher than "
-            "--test-beta to see successful attacks. Default = %(default)f"
+            """Value of b parameter for beta distribution used to sample the in-sample
+            probabilities. High values will give more extreme probabilities. Set this
+            value higher than --test-beta to see successful attacks. Default = %(default)f"""
         ),
     )
 
     dummy_parser.add_argument(
         "--test-beta",
         action="store",
         type=float,
@@ -704,22 +783,33 @@
         help=(
             "Proportion of examples to be used for testing when fiting the attack model. "
             "Default = %(default)f"
         ),
     )
 
     attack_parser.add_argument(
+        "--output-dir",
+        type=str,
+        action="store",
+        dest="output_dir",
+        default="output_worstcase",
+        required=False,
+        help=("Directory name where output files are stored. Default = %(default)s."),
+    )
+
+    attack_parser.add_argument(
         "--report-name",
         type=str,
         action="store",
         dest="report_name",
-        default="worstcase_report",
+        default="report_worstcase",
         required=False,
         help=(
-            "Filename for the report output. Default = %(default)s. Code will append .pdf and .json"
+            """Filename for the pdf and json report outputs. Default = %(default)s.
+            Code will append .pdf and .json"""
         ),
     )
 
     attack_parser.add_argument(
         "--n-dummy-reps",
         type=int,
         action="store",
@@ -746,16 +836,15 @@
         "--train-beta",
         action="store",
         type=float,
         required=False,
         default=5,
         dest="train_beta",
         help=(
-            "Value of b parameter for beta distribution used to sample the in-sample "
-            "probabilities. "
+            "Value of b parameter for beta distribution used to sample the in-sample probabilities."
             "High values will give more extreme probabilities. Set this value higher than "
             "--test-beta to see successful attacks. Default = %(default)f"
         ),
     )
 
     attack_parser.add_argument(
         "--test-beta",
@@ -767,28 +856,16 @@
         help=(
             "Value of b parameter for beta distribution used to sample the out-of-sample "
             "probabilities. High values will give more extreme probabilities. Set this value "
             "lower than --train-beta to see successful attacks. Default = %(default)f"
         ),
     )
 
-    # Not currently possible from the command line as we cannot compute the correctness
-    # of predictions. Possibly to be added in the future
-    # attack_parser.add_argument(
-    #     "--include-correct",
-    #     action="store",
-    #     type=bool,
-    #     required=False,
-    #     default=False,
-    #     dest='include_model_correct_feature',
-    #     help=(
-    #         "Whether or not to include an additional feature into the MIA attack model that "
-    #         "holds whether or not the target model made a correct predicion for each example."
-    #     ),
-    # )
+    # --include-correct feature not supported as not currently possible from the command line
+    # as we cannot compute the correctness of predictions.
 
     attack_parser.add_argument(
         "--sort-probs",
         action="store",
         type=bool,
         default=True,
         required=False,
@@ -842,30 +919,28 @@
         "--attack-metric-success-count-thresh",
         action="store",
         type=int,
         default=2,
         required=False,
         dest="attack_metric_success_count_thresh",
         help=(
-            """for setting counter limit to stop further repetitions
-            given the attack is successful and the
-            --attack-fail-fast is true. Default = %(default)d"""
+            """for setting counter limit to stop further repetitions given the attack is
+             successful and the --attack-fail-fast is true. Default = %(default)d"""
         ),
     )
 
     attack_parser.add_argument(
         "--attack-fail-fast",
         action="store_true",
         required=False,
         dest="attack_fail_fast",
         help=(
             """to stop further repetitions when the given metric has fulfilled
             a criteria for a specified number of times (--attack-metric-success-count-thresh)
-            and this has a true status.
-            Default = %(default)s"""
+            and this has a true status. Default = %(default)s"""
         ),
     )
 
     attack_parser.set_defaults(func=_run_attack)
 
     attack_parser_config = subparsers.add_parser("run-attack-from-configfile")
     attack_parser_config.add_argument(
@@ -877,14 +952,28 @@
         type=str,
         default="config_worstcase_cmd.json",
         help=(
             "Name of the .json file containing details for the run. Default = %(default)s"
         ),
     )
 
+    attack_parser_config.add_argument(
+        "-t",
+        "--attack-target-folder-path",
+        action="store",
+        required=True,
+        dest="target_path",
+        type=str,
+        default="worstcase_target",
+        help=(
+            """Name of the target directory to load the trained target model and the target data.
+            Default = %(default)s"""
+        ),
+    )
+
     attack_parser_config.set_defaults(func=_run_attack_from_configfile)
 
     args = parser.parse_args()
 
     try:
         args.func(args)
     except AttributeError as e:  # pragma:no cover
```

### Comparing `aisdc-1.0.5.post1/aisdc/metrics.py` & `aisdc-1.0.6/aisdc/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Calculate metrics.
-"""
+"""Calculate metrics."""
 
 from __future__ import annotations
 
 from collections.abc import Iterable
 
 import numpy as np
 from scipy import interpolate
@@ -14,28 +12,30 @@
 # pylint: disable = invalid-name
 
 VAR_THRESH = 1e-2
 
 
 def _div(x: float, y: float, default: float) -> float:
     """Solve the problem of division by 0 and round up.
-    If y is non-zero, perform x/y and round to 8dp. If it is zero, return the default
+
+    If y is non-zero, perform x/y and round to 8dp. If it is zero, return the
+    default.
 
     Parameters
     ----------
-    x: float
+    x : float
         numerator
-    y: float
+    y : float
         denominator
-    default: float
+    default : float
         return value if y == 0
 
     Returns
     -------
-    division: float
+    division : float
         x / y, or default if y == 0
     """
     if y != 0:
         division = round(float(x / y), 8)
     else:
         division = float(default)
     return division
@@ -44,31 +44,32 @@
 def _tpr_at_fpr(
     y_true: Iterable[float],
     y_score: Iterable[float],
     fpr: float = 0.001,
     fpr_perc: bool = False,
 ) -> float:
     """Compute the TPR at a fixed FPR.
-    In particular, returns the TPR value corresponding to a particular FPR. Uses interpolation
-    to fill in gaps.
+
+    In particular, returns the TPR value corresponding to a particular FPR.
+    Uses interpolation to fill in gaps.
 
     Parameters
     ----------
-    y_true: Iterable[float]
+    y_true : Iterable[float]
         actual class labels
-    y_score: Iterable[float]
+    y_score : Iterable[float]
         predicted score
-    fpr: float
+    fpr : float
         false positive rate at which to compute true positive rate
-    fpr_perc: bool
+    fpr_perc : bool
         if the fpr is defined as a percentage
 
     Returns
     -------
-    tpr: float
+    tpr : float
         true positive rate at fpr
     """
 
     if fpr_perc:
         fpr /= 100.0
 
     fpr_vals, tpr_vals, thresh_vals = roc_curve(y_true, y_score)
@@ -78,30 +79,30 @@
     thresh = thresh_from_fpr(fpr)
     tpr = tpr_from_thresh(thresh)
 
     return tpr
 
 
 def _expected_auc_var(auc: float, num_pos: int, num_neg: int) -> float:
-    """ "Compute variance of AUC under assumption of uniform probabilities
-    uses the expression given as eqn (2) in  https://cs.nyu.edu/~mohri/pub/area.pdf
+    """Compute variance of AUC under assumption of uniform probabilities
+    uses the expression given as eqn (2) in  https://cs.nyu.edu/~mohri/pub/area.pdf.
 
     Parameters
     ----------
 
-    auc: float
+    auc : float
         auc value at which to compute the variance
-    num_pos: int
+    num_pos : int
         number of positive examples
-    num_neg: int
+    num_neg : int
         number of negative examples
 
     Returns
     -------
-    var: float
+    var : float
         null variance of AUC
     """
     p_xxy = p_xyy = 1 / 3
     var = (
         auc * (1 - auc)
         + (num_pos - 1) * (p_xxy - auc**2)
         + (num_neg - 1) * (p_xyy - auc**2)
@@ -122,35 +123,35 @@
     probability (that is, membership probabilities are essentially random) is also used
     as a metric (using a usual Gaussian approximation to binomial). If the p-value is
     low and the frequency difference is high (>0.5) then the MIA attack is successful
     for some samples.
 
     Parameters
     ----------
-    y: np.ndarray
+    y : np.ndarray
         true labels
-    yp: np.ndarray
+    yp : np.ndarray
         probabilities of labels, or monotonic transformation of probabilties
-    xprop: float
+    xprop : float
         proportion of samples with highest- and lowest- probability of membership to be
         considered
-    logp: bool
+    logp : bool
         convert p-values to log(p).
 
     Returns
     -------
-    maxd: float
+    maxd : float
         frequency of y=1 amongst proportion xprop of individuals with highest assessed
         membership probability
-    mind: float
+    mind : float
         frequency of y=1 amongst proportion xprop of individuals with lowest assessed
         membership probability
-    mmd: float
+    mmd : float
         difference between maxd and mind
-    pval: float
+    pval : float
         p-value or log-p value corresponding to mmd against null hypothesis that random
         variables corresponding to y and yp are independent.
 
     Notes
     -----
 
     Examples
@@ -184,30 +185,30 @@
             pval = np.log(pval)
 
     # Return
     return maxd, mind, mmd, pval
 
 
 def auc_p_val(auc: float, n_pos: int, n_neg: int) -> tuple[float, float]:
-    """Compute the p-value for a given AUC
+    """Compute the p-value for a given AUC.
 
     Parameters
     ----------
-    auc: float
+    auc : float
         Observed AUC value
-    n_pos: int
+    n_pos : int
         Number of positive examples
-    n_neg: int
+    n_neg : int
         Number of negative examples
 
     Returns
     -------
-    auc_p: float
+    auc_p : float
         p-value of observing an AUC > auc by chance
-    auc_std: float
+    auc_std : float
         standard deviation of the NULL AUC diustribution (mean = 0.5)
     """
     auc_std = np.sqrt(_expected_auc_var(0.5, n_pos, n_neg))
     auc_p = 1 - norm.cdf(auc, loc=0.5, scale=auc_std)
     return auc_p, auc_std
 
 
@@ -219,26 +220,26 @@
 ):
     """
     Given a prediction model and a dataset, calculate the predictions of the model for
     each data sample in probability format.
 
     Parameters
     ----------
-    clf: sklearn.Model
+    clf : sklearn.Model
         trained model
-    X_test: np.ndarray
+    X_test : np.ndarray
         test data matrix
-    y_test: np.ndarray
+    y_test : np.ndarray
         test data labels
-    permute_rows: boolean
+    permute_rows : boolean
         a flag to indicate whether rows should be permuted
 
     Returns
     -------
-    y_pred_proba: a list of probabilities for each sample in the dataset
+    y_pred_proba : a list of probabilities for each sample in the dataset
 
     Notes
     -----
     If permute_rows is set to true, y_test must also be supplied.
     The function will then return both the predicted probabilities and corresponding y_test
     """
 
@@ -261,27 +262,28 @@
 
 
 def get_metrics(  # pylint: disable=too-many-locals, too-many-statements
     y_pred_proba: np.ndarray, y_test: np.ndarray
 ):
     """
     Calculate metrics, including attacker advantage for MIA binary.
+
     Implemented as Definition 4 on https://arxiv.org/pdf/1709.01604.pdf
-    which is also implemented in tensorFlow-privacy https://github.com/tensorflow/privacy
+    which is also implemented in tensorFlow-privacy https://github.com/tensorflow/privacy.
 
     Parameters
     ----------
-    y_test: np.ndarray
+    y_test : np.ndarray
         test data labels
-    y_pred_proba: np.ndarray of shape [x,2] and type float
+    y_pred_proba : np.ndarray of shape [x,2] and type float
         predicted probabilities
 
     Returns
     -------
-    metrics: dict
+    metrics : dict
         dictionary of metric values
 
     Notes
     -----
     Includes the following metrics:
 
     * True positive rate or recall (TPR).
```

### Comparing `aisdc-1.0.5.post1/aisdc/preprocessing/loaders.py` & `aisdc-1.0.6/aisdc/preprocessing/loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-loaders.py
+Loaders.py
 A set of useful handlers to pull in datasets common to the project and perform the appropriate
-pre-processing
+pre-processing.
 """
 
 # pylint: disable=import-error, invalid-name, consider-using-with, too-many-return-statements
 
 import logging
 import os
 from collections import Counter
@@ -28,15 +28,15 @@
 
 
 PROJECT_ROOT_FOLDER = os.path.dirname(os.path.dirname(__file__))
 logger.info("ROOT PROJECT FOLDER = %s", PROJECT_ROOT_FOLDER)
 
 
 class UnknownDataset(Exception):
-    """Exception raised if the user passes a name that we don't recognise"""
+    """Exception raised if the user passes a name that we don't recognise."""
 
 
 class DataNotAvailable(Exception):
     """Exception raised if the user asks for a dataset that they do not have the data for. I.e.
     some datasets require a .csv file to have been downloaded.
     """
 
@@ -45,25 +45,25 @@
     dataset_name: str, data_folder: str = os.path.join(PROJECT_ROOT_FOLDER, "data")
 ) -> Tuple[pd.DataFrame, pd.DataFrame]:
     """Main entry method to return data in format sensible for sklearn. User passes a name and that
     dataset is returned as a tuple of pandas DataFrames (data, labels).
 
     Parameters
     ----------
-    dataset_name: str
+    dataset_name : str
         The name of the dataset to load
-    data_folder: str
+    data_folder : str
         The name of the local folder in which data is stored.
 
     Returns
     -------
 
-    X: pd.DataFrame
+    X : pd.DataFrame
         The input dataframe -- rows are examples, columns variables
-    y: pd.DataFrame
+    y : pd.DataFrame
         the target dataframe -- has a single column containing the target values
 
     Notes
     -----
 
     The following datasets are available:
     mimic2-iaccd (requires data download)
@@ -85,16 +85,14 @@
 
     These can be nested.
 
     Examples
     --------
     >>> X, y = get_data_sklearn("mimic2-iaccd") # pull the mimic2-iaccd data
     >>> X, y = get_data_sklearn("minmax iris") # pull the iris data and round continuous features
-
-
     """
     logger.info("DATASET FOLDER = %s", data_folder)
 
     if dataset_name.startswith("standard"):
         sub_name = dataset_name.split("standard")[1].strip()
         feature_df, target_df = get_data_sklearn(sub_name)
         for column in feature_df.columns:
@@ -151,27 +149,23 @@
         return _nursery()
     if dataset_name == "iris":
         return _iris()
     raise UnknownDataset(dataset_name)
 
 
 def _iris() -> Tuple[pd.DataFrame, pd.DataFrame]:
-    """
-    sklearn iris data - just first two classes
-    """
+    """Sklearn iris data - just first two classes."""
     X, y = load_iris(return_X_y=True, as_frame=True)
     X = X[y < 2]
     y = y[y < 2]
     return X, pd.DataFrame(y)
 
 
 def _nursery() -> Tuple[pd.DataFrame, pd.DataFrame]:
-    """
-    The sklearn nursery dataset
-    """
+    """The sklearn nursery dataset."""
 
     data = fetch_openml(data_id=26, as_frame=True)
 
     target_encoder = LabelEncoder()
     target_vals = target_encoder.fit_transform(data["target"].values)
     target_dataframe = pd.DataFrame({"target": target_vals})
 
@@ -185,17 +179,15 @@
 
 
 # Patched to support non-flattened images. Same behaviour as before except if called with
 # flatten=False explicitly.
 def _images_to_ndarray(
     images_dir: str, number_to_load: int, label: int, flatten: bool = True
 ) -> Tuple[np.array, np.array]:
-    """
-    Grab number_to_load images from the images_dir and create a np array and label array
-    """
+    """Grab number_to_load images from the images_dir and create a np array and label array."""
     folder_path = images_dir + os.sep
     images_names = sorted(os.listdir(folder_path))
     images_names = images_names[:number_to_load]
     # fix f or macosx
     if ".DS_Store" in images_names:  # pragma: no cover
         images_names.remove(".DS_Store")
 
@@ -211,15 +203,15 @@
 
 def _medical_mnist_loader(  # pylint: disable = too-many-locals
     data_folder: str, n_per_class: int, classes: List[str]
 ) -> Tuple[pd.DataFrame, pd.DataFrame]:
     """
     Load Medical MNIST into pandas format
     borrows heavily from: https://www.kaggle.com/harelshattenstein/medical-mnist-knn
-    Creates a binary classification
+    Creates a binary classification.
     """
 
     base_folder = os.path.join(
         data_folder,
         "kaggle-medical-mnist",
         "archive",
     )
@@ -274,15 +266,15 @@
 
 
 def _synth_ae(
     data_folder: str, n_rows: int = 5000
 ) -> Tuple[pd.DataFrame, pd.DataFrame]:
     """
     First norws (default 5000) rows from the Synthetic A&E data from NHS England
-    https://data.england.nhs.uk/dataset/a-e-synthetic-data/resource/81b068e5-6501-4840-a880-a8e7aa56890e # pylint: disable=line-too-long
+    https://data.england.nhs.uk/dataset/a-e-synthetic-data/resource/81b068e5-6501-4840-a880-a8e7aa56890e # pylint: disable=line-too-long.
     """
 
     file_path = os.path.join(
         data_folder, "AE_England_synthetic.csv"  #'A&E Synthetic Data.csv'
     )
 
     if not os.path.exists(file_path):
@@ -328,15 +320,15 @@
 
     return (X, y)
 
 
 def _indian_liver(data_folder: str) -> Tuple[pd.DataFrame, pd.DataFrame]:
     """
     Indian Liver Patient Dataset
-    https://archive.ics.uci.edu/ml/machine-learning-databases/00225/Indian%20Liver%20Patient%20Dataset%20(ILPD).csv # pylint: disable=line-too-long
+    https://archive.ics.uci.edu/ml/machine-learning-databases/00225/Indian%20Liver%20Patient%20Dataset%20(ILPD).csv # pylint: disable=line-too-long.
     """
     # (https://archive.ics.uci.edu/ml/datasets/ILPD+(Indian+Liver+Patient+Dataset)
     file_path = os.path.join(data_folder, "Indian Liver Patient Dataset (ILPD).csv")
     if not os.path.exists(file_path):
         help_message = f"""
 Data file {file_path} does not exist. Please download fhe file from:
 https://archive.ics.uci.edu/ml/datasets/ILPD+(Indian+Liver+Patient+Dataset
@@ -373,15 +365,15 @@
     liver_labels = pd.DataFrame({"class": encoded_labels})
     return (liver_data, liver_labels)
 
 
 def _in_hospital_mortality(data_folder: str) -> Tuple[pd.DataFrame, pd.DataFrame]:
     """
     In-hospital mortality data from this study:
-        https://datadryad.org/stash/dataset/doi:10.5061/dryad.0p2ngf1zd
+        https://datadryad.org/stash/dataset/doi:10.5061/dryad.0p2ngf1zd.
     """
     # Check the data has been downloaded. If not throw an exception with instructions on how to
     # download, and where to store
     files = ["data01.csv", "doi_10.5061_dryad.0p2ngf1zd__v5.zip"]
     file_path = [os.path.join(data_folder, f) for f in files]
 
     if not any(  # pylint: disable=use-a-generator
@@ -407,17 +399,15 @@
     encoded_labels = label_encoder.fit_transform(labels.values)
     labels = pd.DataFrame({"outcome": encoded_labels})
 
     return (features, labels)
 
 
 def _mimic_iaccd(data_folder: str) -> Tuple[pd.DataFrame, pd.DataFrame]:
-    """
-    Loads the mimic_iaccd data and performs Alba's pre-processing
-    """
+    """Loads the mimic_iaccd data and performs Alba's pre-processing."""
 
     # Check the data has been downloaded. If not throw an exception with instructions on how to
     # download, and where to store
     file_path = os.path.join(data_folder, "mimic2-iaccd", "1.0", "full_cohort_data.csv")
 
     if not os.path.exists(file_path):
         help_message = f"""
@@ -465,20 +455,19 @@
 
 def _texas_hospitals(
     data_folder: str,
 ) -> Tuple[pd.DataFrame, pd.DataFrame]:  # pragma: no cover
     # pylint: disable=too-many-statements, too-many-locals
     """
     Texas Hospitals Dataset
-    (https://www.dshs.texas.gov/THCIC/Hospitals/Download.shtm)
+    (https://www.dshs.texas.gov/THCIC/Hospitals/Download.shtm).
 
     Note: this has been tested repeated in the GRAIMatter project.
     However, for licensing reasons we cannot redistribute the data.
     Therefore it is omitted from CI test coverage and metrics.
-
     """
     file_list = [
         "PUDF-1Q2006-tab-delimited.zip",
         "PUDF-1Q2007-tab-delimited.zip",
         "PUDF-1Q2008-tab-delimited.zip",
         "PUDF-1Q2009-tab-delimited.zip",
         "PUDF-2Q2006-tab-delimited.zip",
```

### Comparing `aisdc-1.0.5.post1/aisdc/safemodel/classifiers/dp_svc.py` & `aisdc-1.0.6/aisdc/safemodel/classifiers/dp_svc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Differentially private SVC
 James Liley
-21/03/22
+21/03/22.
 """
 import logging
 from typing import Any
 
 import numpy as np
 from sklearn.linear_model import LogisticRegression
 from sklearn.svm import SVC
@@ -17,15 +17,15 @@
 # pylint: disable = invalid-name
 # pylint: disable=R0902: too-many-instance-attributes
 # pylint:disable = fixme
 
 
 class DPSVC:
     """
-    Wrapper for differentially private SVM, implemented according to the method in
+    Wrapper for differentially private SVM, implemented according to the method in.
 
     https://arxiv.org/pdf/0911.5708.pdf
 
     Essentially approximates an infinite-dimensional latent space (and corresponding kernel) with
     a finite dimensional latent space, and adds noise to the normal to the separating hyperplane
     in this latent space.
 
@@ -45,15 +45,14 @@
 
     where 1-zeta_i≤ y_i (w phi(x_i) + b), where phi maps x to the latent space and zeta_i ≥ 0.
     This is equivalent to minimising
 
     (1/2) ||w||_2 + C/n sum(l(y_i,f_w(x_i)))
 
     where l(x,y)=n*max(0,1- x.y), which is n-Lipschitz continuous in y (given x is in {-1,1})
-
     """
 
     def __init__(self, C=1.0, gamma="scale", dhat=1000, eps=10, **kwargs):
         self.svc = None
         self.gamma = gamma
         self.dpsvc_gamma = None
         self.dhat = dhat
@@ -66,23 +65,21 @@
         self.b = None
         self.classes_ = [0, 1]
         self.intercept = None
         self.noisy_weights = None
         self.set_params(**kwargs)
 
     def phi_hat(self, input_vector):
-        """Project a single feature"""
+        """Project a single feature."""
         vt1 = (self.rho * input_vector).sum(axis=1)
         vt = (self.dhat ** (-0.5)) * np.column_stack((np.cos(vt1), np.sin(vt1)))
         return vt.reshape(2 * self.dhat)
 
     def phi_hat_multi(self, input_features):
-        """
-        Compute feature space for a matrix of inputs
-        """
+        """Compute feature space for a matrix of inputs."""
         # TODO: could this be vectorised?
         n_data, _ = input_features.shape
         phi_hat = np.zeros((n_data, 2 * self.dhat), float)
         for i in range(n_data):
             phi_hat[i, :] = self.phi_hat(input_features[i, :])
         return phi_hat
 
@@ -95,17 +92,15 @@
         if y is None:
             phi_hat_y = phi_hat_x
         else:
             phi_hat_y = self.phi_hat_multi(y)
         return np.dot(phi_hat_x, phi_hat_y.T)
 
     def fit(self, train_features: Any, train_labels: Any) -> None:
-        """
-        Fit the model
-        """
+        """Fit the model."""
 
         # Check that the data passed is np.ndarray
         if not isinstance(train_features, np.ndarray) or not isinstance(
             train_labels, np.ndarray
         ):
             raise NotImplementedError("DPSCV needs np.ndarray inputs")
 
@@ -179,43 +174,35 @@
 
         local_logger.info("Fitting Platt scaling")
         self.platt_transform.fit(
             ypredn.reshape(-1, 1), train_labels
         )  # was called ptransform
 
     def set_params(self, **kwargs) -> None:
-        """
-        Set params
-        """
+        """Set params."""
         for key, value in kwargs.items():
             if key == "gamma":
                 self.gamma = value
             elif key == "eps":
                 self.eps = value
             elif key == "dhat":
                 self.dhat = value
             else:
                 local_logger.warning("Unsupported parameter: %s", key)
 
     def _raw_outputs(self, test_features: Any) -> np.ndarray:
-        """
-        Get the raw output, used by predict and predict_proba
-        """
+        """Get the raw output, used by predict and predict_proba."""
         projected_features = self.phi_hat_multi(test_features)
         out = np.dot(projected_features, self.noisy_weights) + self.intercept
         return out
 
     def predict(self, test_features: Any) -> np.ndarray:
-        """
-        Make predictions
-        """
+        """Make predictions."""
         out = self._raw_outputs(test_features)
         out = 1 * (out > 0)
         return out  # Predictions
 
     def predict_proba(self, test_features: Any) -> np.ndarray:
-        """
-        Predictive probabilities
-        """
+        """Predictive probabilities."""
         out = self._raw_outputs(test_features)
         pred_probs = self.platt_transform.predict_proba(out.reshape(-1, 1))
         return pred_probs
```

### Comparing `aisdc-1.0.5.post1/aisdc/safemodel/classifiers/new_model_template.py` & `aisdc-1.0.6/aisdc/safemodel/classifiers/new_model_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """This is a template for implementing supplementary models
    Obviously we have invented an sklearn ensemble called ModelToMakeSafer
    Replace this with details of the model you wish to create a wrapper for
-   and then remove the comment which disables the pylint warning"""
+   and then remove the comment which disables the pylint warning.
+"""
 
 # pylint: disable=duplicate-code
 
 from __future__ import annotations
 
 import copy
 from typing import Any
@@ -18,15 +19,15 @@
 from ..safemodel import SafeModel
 from .safedecisiontreeclassifier import decision_trees_are_equal
 
 
 def check_present(
     item: str, curr_separate: dict, saved_separate: dict
 ) -> tuple[str, bool]:
-    """checks item is present in both dicts and reports suitably"""
+    """Checks item is present in both dicts and reports suitably."""
     disclosive = False
     msg = ""
     if curr_separate[item] == "Absent" and saved_separate[item] == "Absent":
         disclosive = True
         msg += "Error: model has not been fitted to data.\n"
 
     elif curr_separate[item] == "Absent":
@@ -39,15 +40,15 @@
     return msg, disclosive
 
 
 class SafeModelToMakeSafe(SafeModel, ModelToMakeSafer):
     """Privacy protected ModelToMakeSafer."""
 
     def __init__(self, **kwargs: Any) -> None:
-        """Creates model and applies constraints to params"""
+        """Creates model and applies constraints to params."""
         SafeModel.__init__(self)
         self.k_anonymity = 0
         self.basemodel_paramnames = [
             "edit",
             "this",
             "list",
             "to",
@@ -86,15 +87,15 @@
 
     def additional_checks(  # pylint: disable=too-many-nested-blocks,too-many-branches
         self, curr_separate: dict, saved_separate: dict
     ) -> tuple[str, str]:
         """ModelToMakeSafer specific checks
         This example shows how to deal with instances of sklearn's tree class
         as base estimators in a forest (line 99)
-        or as single estimators (lines 114-118)
+        or as single estimators (lines 114-118).
         """
         msg = ""
         disclosive = False
         ## call the super function to deal with any items that are lists
         # msg, disclosive = super().additional_checks(curr_separate, saved_separate)
         # now the relevant ModelToMakeSafer specific things
         for item in self.examine_seperately_items:
@@ -147,21 +148,21 @@
                 diffs_list = list(diff(curr_separate[item], saved_separate[item]))
                 if len(diffs_list) > 0:
                     disclosive = True
                     msg += f"structure {item} has {len(diffs_list)} differences: {diffs_list}"
         return msg, disclosive
 
     def fit(self, x: np.ndarray, y: np.ndarray) -> None:
-        """Do fit and then store model dict"""
+        """Do fit and then store model dict."""
         super().fit(x, y)
         self.k_anonymity = self.get_k_anonymity(x)
         self.saved_model = copy.deepcopy(self.__dict__)
 
     def get_k_anonymity(self, x: np.ndarray) -> int:
-        """calculates the k-anonymity of a random forest model
+        """Calculates the k-anonymity of a random forest model
         as the minimum of the anonymity for each record.
         That is defined as the size of the set of records which
         appear in the same leaf as the record in every tree.
         """
 
         # dataset must be 2-D
         assert len(x.shape) == 2
```

### Comparing `aisdc-1.0.5.post1/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py` & `aisdc-1.0.6/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from ..safemodel import SafeModel
 
 
 def decision_trees_are_equal(
     tree1: DecisionTreeClassifier, tree2: DecisionTreeClassifier
 ) -> tuple[bool, str]:
     """Compares two estimators of type sklearn.tree
-    e.g. two decisionTreeClassifiers
+    e.g. two decisionTreeClassifiers.
     """
     msg = ""
     same = True
 
     try:
         tree1_dict = copy.deepcopy(tree1.__dict__)
         tree1_tree = tree1_dict.pop("tree_", "Absent")
@@ -58,15 +58,16 @@
     return same, msg
 
 
 def decision_tree_internal_trees_are_equal(
     tree1_tree: Any, tree2_tree: Any
 ) -> tuple[bool, str]:
     """Tests for equality of the internal structures in a sklearn.tree._tree
-    e.g. the structure, feature and threshold in each internal node etc."""
+    e.g. the structure, feature and threshold in each internal node etc.
+    """
 
     same = True
     msg = ""
     tree_internal_att_names = (
         "capacity",
         "children_left",
         "children_right",
@@ -113,15 +114,15 @@
     except BaseException as error:  # pylint:disable=broad-except #pragma:no cover
         msg += get_reporting_string(name="exception_occurred", error=error)
         # f"An exception occurred: {error}"
     return same, msg
 
 
 def get_tree_k_anonymity(thetree: DecisionTreeClassifier, X: Any) -> int:
-    """returns the smallest number of data items in any leaf"""
+    """Returns the smallest number of data items in any leaf."""
     leaves = thetree.apply(X)
     uniqs_counts = np.unique(leaves, return_counts=True)
     k_anonymity = np.min(uniqs_counts[1])
     # print(f' leaf ids {uniqs_counts[0]} and counts {uniqs_counts[1]}'
     #        f'the  k-anonymity of the tree is {k_anonymity}')
     return k_anonymity
 
@@ -164,15 +165,15 @@
         ]
         self.examine_seperately_items = ["tree_"]
         self.k_anonymity = 0
 
     def additional_checks(
         self, curr_separate: dict, saved_separate: dict
     ) -> tuple[str, str]:
-        """Decision Tree-specific checks"""
+        """Decision Tree-specific checks."""
         # call the super function to deal with any items that are lists
         # just in case we add any in the future
         msg, disclosive = super().additional_checks(curr_separate, saved_separate)
         # now deal with the decision-tree specific things
         # which for now means the attribute "tree_" which is a sklearn tree
         same, msg = decision_tree_internal_trees_are_equal(
             curr_separate["tree_"], saved_separate["tree_"]
@@ -187,14 +188,14 @@
             # )
 
         return msg, disclosive
 
     def fit(  # pylint: disable=arguments-differ
         self, x: np.ndarray, y: np.ndarray
     ) -> None:
-        """Do fit and then store k-anonymity and  model dict"""
+        """Do fit and then store k-anonymity and  model dict."""
         super().fit(x, y)
         # calculate k-anonymity her since we have the tainigf data
         leaves = self.apply(x)
         uniqs_counts = np.unique(leaves, return_counts=True)
         self.k_anonymity = np.min(uniqs_counts[1])
         self.saved_model = copy.deepcopy(self.__dict__)
```

### Comparing `aisdc-1.0.5.post1/aisdc/safemodel/classifiers/safekeras.py` & `aisdc-1.0.6/aisdc/safemodel/classifiers/safekeras.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-""" safekeras.py:
+"""Safekeras.py:
  Jim Smith, Andrew McCarty and Richard Preen
- UWE 2022
+ UWE 2022.
 """
 # general imports
 
 
 import os
 import warnings
 
@@ -39,15 +39,15 @@
 DP_CLASS_STRING2 = (
     "tensorflow_privacy.privacy.optimizers.dp_optimizer_keras."
     "make_keras_generic_optimizer_class.<locals>.DPOptimizerClass"
 )
 
 
 def same_configs(m1: Any, m2: Any) -> Tuple[bool, str]:
-    """Checks if two models havethe same architecture"""
+    """Checks if two models havethe same architecture."""
     num_layers = len(m1.layers)
     if len(m2.layers) != num_layers:
         errstr = get_reporting_string(name="different_layer_count")
         return False, errstr
     for layer in range(num_layers):
         m1_layer_config = m1.layers[layer].get_config()
         _ = m1_layer_config.pop("name")
@@ -72,15 +72,15 @@
                     msg += f"{match[i]}"  # pragma: no cover
             return False, msg
 
     return True, get_reporting_string(name="same_ann_config")
 
 
 def same_weights(m1: Any, m2: Any) -> Tuple[bool, str]:
-    """checks if two nets with same architecture havethe same weights"""
+    """Checks if two nets with same architecture havethe same weights."""
     num_layers = len(m1.layers)
     if num_layers != len(m2.layers):
         return False, "different numbers of layers"
     # layer 0 is input layer determined by data size
     for layer in range(1, num_layers):
         m1layer = m1.layers[layer].get_weights()
         m2layer = m2.layers[layer].get_weights()
@@ -92,18 +92,18 @@
             # print(type(m1d), m1d.shape)
             if not np.array_equal(m1d, m2d):  # pragma: no cover
                 return False, f"dimension {dim} of layer {layer} differs"
     return True, "weights match"
 
 
 def check_checkpoint_equality(v1: str, v2: str) -> Tuple[bool, str]:
-    """compares two checkpoints saved with tensorflow save_model
+    """Compares two checkpoints saved with tensorflow save_model
     On the assumption that the optimiser is not going to be saved,
     and that the model is going to be saved in frozen form
-    this only checks the architecture and weights layer by layer
+    this only checks the architecture and weights layer by layer.
     """
     msg = ""
     same = True
 
     try:
         model1 = tf.keras.models.load_model(v1)
     except Exception as e:  # pylint:disable=broad-except
@@ -129,15 +129,15 @@
         msg += weights_message
         same = False
 
     return same, msg
 
 
 def check_DP_used(optimizer) -> Tuple[bool, str]:
-    """checks whether the DP optimizer was actually the one used"""
+    """Checks whether the DP optimizer was actually the one used."""
 
     key_needed = "_was_dp_gradients_called"
     critical_val = optimizer.__dict__.get(key_needed, "missing")
 
     if critical_val is True:
         reason = get_reporting_string(name="dp_optimizer_run")
         DPused = True
@@ -156,42 +156,42 @@
         )  # pragma: no cover
         DPused = False  # pragma: no cover
 
     return DPused, reason
 
 
 def check_optimizer_allowed(optimizer) -> Tuple[bool, str]:
-    """checks if the model's optimizer is in our white-list
-    default setting is not allowed
+    """Checks if the model's optimizer is in our white-list
+    default setting is not allowed.
     """
     allowed = False
     opt_type = str(type(optimizer))
     reason = get_reporting_string(name="optimizer_not_allowed", optimizer=opt_type)
     if (DP_CLASS_STRING in opt_type) or (DP_CLASS_STRING2 in opt_type):
         allowed = True
         reason = get_reporting_string(name="optimizer_allowed", optimizer=opt_type)
 
     return allowed, reason
 
 
 def check_optimizer_is_DP(optimizer) -> Tuple[bool, str]:
-    """checks whether optimizer is one of tensorflow's DP versions"""
+    """Checks whether optimizer is one of tensorflow's DP versions."""
     DPused = False
     reason = "None"
     if "_was_dp_gradients_called" not in optimizer.__dict__:
         reason = get_reporting_string(name="no_dp_gradients_key")
     else:
         reason = get_reporting_string(name="found_dp_gradients_key")
         DPused = True
     return DPused, reason
 
 
 def load_safe_keras_model(name: str = "undefined") -> Tuple[bool, Any]:
     """
-    reads model from file in appropriate format.
+    Reads model from file in appropriate format.
     Optimizer is deliberately excluded in the save.
     This is to prevent possibility of restarting training,
     which could offer possible back door into attacks.
     Thus optimizer cannot be loaded.
     """
     the_model = None
     model_load_file = name
@@ -216,20 +216,20 @@
     # else
     return (False, msg)
 
 
 class SafeKerasModel(KerasModel, SafeModel):
     """Privacy Protected Wrapper around  tf.keras.Model class from tensorflow 2.8
     disabling pylont warnings about number of instance attributes
-    as this is necessarily complex
+    as this is necessarily complex.
     """
 
     # pylint: disable=too-many-instance-attributes
     def __init__(self, *args: Any, **kwargs: Any) -> None:
-        """Creates model and applies constraints to params"""
+        """Creates model and applies constraints to params."""
 
         # the_args = args
         the_kwargs = kwargs
 
         # initialise all the values that get provided as options to keras
         # and also l2 norm clipping and learning rates, batch sizes
         ##inputs = kwargs.get("inputs","notFound")
@@ -289,30 +289,31 @@
         _ = self.__dict__.pop("saved_model")
         super().preliminary_check(apply_constraints=True, verbose=True)
 
     def dp_epsilon_met(
         self, num_examples: int, batch_size: int = 0, epochs: int = 0
     ) -> Tuple[bool, str]:
         """Checks if epsilon is sufficient for Differential Privacy
-        Provides feedback to user if epsilon is not sufficient"""
+        Provides feedback to user if epsilon is not sufficient.
+        """
         privacy = compute_dp_sgd_privacy(
             n=num_examples,
             batch_size=batch_size,
             noise_multiplier=self.noise_multiplier,
             epochs=epochs,
             delta=self.delta,
         )
         ok = privacy[0] < self.min_epsilon
         return ok, privacy[0]
 
     def check_epsilon(
         self, num_samples: int, batch_size: int, epochs: int
     ) -> Tuple[bool, str]:
         """Computes the level of privacy guarantee is within recommended limits,
-        and produces feedback"
+        and produces feedback".
         """
         msg = ""
         ok = False
         if batch_size == 0:
             msg += get_reporting_string(name="division_by_zero")
             batch_size = 1
         (
@@ -436,15 +437,15 @@
         self.saved_was_dpused, self.saved_reason = check_DP_used(self.optimizer)
         self.saved_epsilon = self.current_epsilon
         return returnval
 
     def posthoc_check(self, verbose: bool = True) -> Tuple[str, bool]:
         """Checks whether model should be considered unsafe
         for example, has been changed since fit() was last run,
-        or does not meet DP policy
+        or does not meet DP policy.
         """
 
         disclosive = False
         msg = ""
 
         # have the model architecture or weights been changed?
         self.save("tfsaves/requested_model.tf")
@@ -511,26 +512,25 @@
 
     def save(self, name: str = "undefined") -> None:
         """Writes model to file in appropriate format.
 
         Parameters
         ----------
 
-        name: string
+        name : string
              The name of the file to save
 
         Returns
         -------
 
         Notes
         -----
 
         No return value
 
-
         Optimizer is deliberately excluded.
         To prevent possible to restart training and thus
         possible back door into attacks.
         """
 
         self.model_save_file = name
         while self.model_save_file == "undefined":
```

### Comparing `aisdc-1.0.5.post1/aisdc/safemodel/classifiers/saferandomforestclassifier.py` & `aisdc-1.0.6/aisdc/safemodel/classifiers/saferandomforestclassifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class SafeRandomForestClassifier(SafeModel, RandomForestClassifier):
     """Privacy protected Random Forest classifier."""
 
     def __init__(
         self, **kwargs: Any
     ) -> None:  # pylint: disable=too-many-instance-attributes
-        """Creates model and applies constraints to params"""
+        """Creates model and applies constraints to params."""
         SafeModel.__init__(self)
         self.basemodel_paramnames = [
             "n_estimators",
             "criterion",
             "max_depth",
             "min_samples_split",
             "min_samples_leaf",
@@ -61,15 +61,15 @@
         self.k_anonymity = 0
 
     def additional_checks(  # pylint: disable=too-many-nested-blocks,too-many-branches
         self, curr_separate: dict, saved_separate: dict
     ) -> tuple[str, str]:
         """Random Forest-specific checks
         would benefit from refactoring into simpler blocks perhaps.
-        NOTE that this is never called if the model has not been fitted
+        NOTE that this is never called if the model has not been fitted.
         """
         msg = ""
         disclosive = False
         # now the relevant random-forest specific things
         for item in self.examine_seperately_items:
             # template for class of things that make up forest
             if item == "base_estimator":
@@ -115,21 +115,21 @@
                     )
                     same = False
 
         return msg, disclosive
 
     # pylint: disable=arguments-differ
     def fit(self, x: np.ndarray, y: np.ndarray) -> None:
-        """Do fit and then store model dict"""
+        """Do fit and then store model dict."""
         super().fit(x, y)
         self.k_anonymity = self.get_k_anonymity(x)
         self.saved_model = copy.deepcopy(self.__dict__)
 
     def get_k_anonymity(self, x: np.ndarray) -> int:
-        """calculates the k-anonymity of a random forest model
+        """Calculates the k-anonymity of a random forest model
         as the minimum of the anonymity for each record.
         That is defined as the size of the set of records which
         appear in the same leaf as the record in every tree.
         """
 
         # dataset must be 2-D
         assert len(x.shape) == 2
```

### Comparing `aisdc-1.0.5.post1/aisdc/safemodel/classifiers/safesvc.py` & `aisdc-1.0.6/aisdc/safemodel/classifiers/safesvc.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,22 +28,22 @@
             "train_labels",
             "weights",
             "noisy_weights",
         ]
         self.examine_seperately_items = ["platt_transform", "svc"]
 
     def fit(self, train_features: np.ndarray, train_labels: np.ndarray) -> None:
-        """Do fit and then store model dict"""
+        """Do fit and then store model dict."""
         super().fit(train_features, train_labels)
         self.saved_model = copy.deepcopy(self.__dict__)
 
     def additional_checks(
         self, curr_separate: dict, saved_separate: dict
     ) -> tuple[str, str]:
-        """SVC specific checks"""
+        """SVC specific checks."""
         msg = ""
         disclosive = False
         for item in self.examine_seperately_items:
             diffs_list = list(
                 diff(curr_separate[item].__dict__, saved_separate[item].__dict__)
             )
             if len(diffs_list) > 0:
```

### Comparing `aisdc-1.0.5.post1/aisdc/safemodel/classifiers/safetf.py` & `aisdc-1.0.6/aisdc/safemodel/classifiers/safetf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-""" work in progress to allow use of the DPModel classes
+"""Work in progress to allow use of the DPModel classes
  Jim smith 2022
- When ready, linting of  the imports will be enabled
+ When ready, linting of  the imports will be enabled.
 """
 
 
 # pylint: disable=unused-import
 from typing import Any
 
 import tensorflow as tf
@@ -15,25 +15,25 @@
 from tensorflow_privacy.privacy.analysis import compute_dp_sgd_privacy
 from tensorflow_privacy.privacy.optimizers import dp_optimizer_keras
 
 from ..safemodel import SafeModel
 
 
 class Safe_tf_DPModel(SafeModel, DPModel):
-    """Privacy Protected tensorflow_privacy DP-SGD subclass of Keras model"""
+    """Privacy Protected tensorflow_privacy DP-SGD subclass of Keras model."""
 
     # remove comment once model starts to be populated
     # pylint:disable=super-init-not-called
     def __init__(
         self,
         l2_norm_clip: float,
         noise_multiplier: float,
         use_xla: bool,
         *args: any,
         **kwargs: any
     ) -> None:
-        """creates model and applies constraints to parameters"""
+        """Creates model and applies constraints to parameters."""
         # safemodel.__init__(self)
         # DPModel.__init__(self, **kwargs)
         # self.model_type: str = "tf_DPModel"
         # super().preliminary_check(apply_constraints=True, verbose=True)
         raise NotImplementedError
```

### Comparing `aisdc-1.0.5.post1/aisdc/safemodel/reporting.py` & `aisdc-1.0.6/aisdc/safemodel/reporting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-"""methods to producte standard reporting strings"""
+"""Methods to producte standard reporting strings."""
 
 
 def get_reporting_string(**kwargs):
-    """returns a standard formatted string from a diction of f-strings.
+    """Returns a standard formatted string from a diction of f-strings.
 
     Parameters
     ----------
 
-    name: string
+    name : string
          The dictionary key and the name of the string to return.
-    all-the-keywords: Any Type
+    all-the-keywords : Any Type
          one or more values expected in the f-string.
 
     Returns
     -------
 
-    msg: string
+    msg : string
          A standard message string.
 
     Notes
     -----
 
     Sometimes an f-string has no parameters.
     Sometimes there are multiple parameters embedded in the f-string.
-
     """
     the_kwargs = kwargs
 
     # check for the name used to reference the diction ary of f-strings
     # if no name is found return an error string
 
     inter_params = {
```

### Comparing `aisdc-1.0.5.post1/aisdc/safemodel/rules.json` & `aisdc-1.0.6/aisdc/safemodel/rules.json`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5.post1/aisdc/safemodel/safemodel.py` & `aisdc-1.0.6/aisdc/safemodel/safemodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,57 +10,52 @@
 import os
 import pathlib
 import pickle
 from pickle import PicklingError
 from typing import Any
 
 import joblib
-
-# import tensorflow as tf
 from dictdiffer import diff
 
-from aisdc.attacks import attribute_attack, dataset, report, worst_case_attack
-from aisdc.attacks.likelihood_attack import (  # pylint: disable = import-error
-    LIRAAttack,
-    LIRAAttackArgs,
-)
+from aisdc.attacks.attribute_attack import AttributeAttack
+from aisdc.attacks.likelihood_attack import LIRAAttack
+from aisdc.attacks.target import Target
+from aisdc.attacks.worst_case_attack import WorstCaseAttack
 
 # pylint : disable=too-many-branches
 from .reporting import get_reporting_string
 
 logger = logging.getLogger(__file__)
 logger.setLevel(logging.DEBUG)
 
 
 def check_min(key: str, val: Any, cur_val: Any) -> tuple[str, bool]:
     """Checks minimum value constraint.
 
     Parameters
     ----------
 
-    key: string
+    key : string
          The dictionary key to examine.
-    val: Any Type
+    val : Any Type
          The expected value of the key.
-    cur_val: Any Type
+    cur_val : Any Type
          The current value of the key.
     ..
 
     Returns
     -------
 
-    msg: string
+    msg : string
          A message string.
-    disclosive: bool
+    disclosive : bool
          A boolean value indicating whether the model is potentially disclosive.
 
     Notes
     -----
-
-
     """
     if isinstance(cur_val, (int, float)):
         if cur_val < val:
             disclosive = True
             msg = get_reporting_string(
                 name="less_than_min_value", key=key, cur_val=cur_val, val=val
             )
@@ -78,34 +73,31 @@
 
 def check_max(key: str, val: Any, cur_val: Any) -> tuple[str, bool]:
     """Checks maximum value constraint.
 
     Parameters
     ----------
 
-    key: string
+    key : string
          The dictionary key to examine.
-    val: Any Type
+    val : Any Type
          The expected value of the key.
-    cur_val: Any Type
+    cur_val : Any Type
          The current value of the key.
 
     Returns
     -------
 
-    msg: string
+    msg : string
          A message string.
-    disclosive: bool
+    disclosive : bool
          A boolean value indicating whether the model is potentially disclosive.
 
-
     Notes
     -----
-
-
     """
     if isinstance(cur_val, (int, float)):
         if cur_val > val:
             disclosive = True
             msg = get_reporting_string(
                 name="greater_than_max_value", key=key, cur_val=cur_val, val=val
             )
@@ -120,39 +112,34 @@
     )
     return msg, disclosive
 
 
 def check_equal(key: str, val: Any, cur_val: Any) -> tuple[str, bool]:
     """Checks equality value constraint.
 
-
-
     Parameters
     ----------
 
-    key: string
+    key : string
          The dictionary key to examine.
-    val: Any Type
+    val : Any Type
          The expected value of the key.
-    cur_val: Any Type
+    cur_val : Any Type
          The current value of the key.
 
     Returns
     -------
 
-    msg: string
+    msg : string
          A message string.
-    disclosive: bool
+    disclosive : bool
          A boolean value indicating whether the model is potentially disclosive.
 
-
     Notes
     -----
-
-
     """
     if cur_val != val:
         disclosive = True
         msg = get_reporting_string(
             name="different_than_fixed_value", key=key, cur_val=cur_val, val=val
         )
     else:
@@ -163,33 +150,31 @@
 
 def check_type(key: str, val: Any, cur_val: Any) -> tuple[str, bool]:
     """Checks the type of a value.
 
     Parameters
     ----------
 
-    key: string
+    key : string
          The dictionary key to examine.
-    val: Any Type
+    val : Any Type
          The expected value of the key.
-    cur_val: Any Type
+    cur_val : Any Type
          The current value of the key.
 
     Returns
     -------
 
-    msg: string
+    msg : string
          A message string.
-    disclosive: bool
+    disclosive : bool
          A boolean value indicating whether the model is potentially disclosive.
 
     Notes
     -----
-
-
     """
     if type(cur_val).__name__ != val:
         disclosive = True
         msg = get_reporting_string(
             name="different_than_recommended_type", key=key, cur_val=cur_val, val=val
         )
     else:
@@ -200,52 +185,46 @@
 
 class SafeModel:  # pylint: disable = too-many-instance-attributes
     """Privacy protected model base class.
 
     Attributes
     ----------
 
-    model_type: string
+    model_type : string
           A string describing the type of model. Default is "None".
     model:
           The Machine Learning Model.
     saved_model:
           A saved copy of the Machine Learning Model used for comparison.
-    ignore_items: list
+    ignore_items : list
           A list of items to ignore when comparing the model with the
           saved_model.
-    examine_separately_items: list
+    examine_separately_items : list
           A list of items to examine separately. These items are more
           complex datastructures that cannot be compared directly.
-    filename: string
+    filename : string
           A filename to save the model.
-    researcher: string
+    researcher : string
           The researcher user-id used for logging
 
-
-
     Notes
     -----
 
     Examples
     --------
     >>> safeRFModel = SafeRandomForestClassifier()
     >>> safeRFModel.fit(X, y)
     >>> safeRFModel.save(name="safe.pkl")
     >>> safeRFModel.preliminary_check()
-    >>> safeRFModel.request_release(filename="safe.pkl")
+    >>> safeRFModel.request_release(path="safe", ext="pkl", target=target)
     WARNING: model parameters may present a disclosure risk:
     - parameter min_samples_leaf = 1 identified as less than the recommended min value of 5.
     Changed parameter min_samples_leaf = 5.
 
     Model parameters are within recommended ranges.
-
-
-
-
     """
 
     def __init__(self) -> None:
         """Super class constructor, gets researcher name."""
         self.model_type: str = "None"
         self.model = None
         self.saved_model = None
@@ -259,15 +238,15 @@
         self.timestamp: str = "None"
         try:
             self.researcher = getpass.getuser()
         except (ImportError, KeyError, OSError):  # pragma: no cover
             self.researcher = "unknown"
 
     def get_params(self, deep=True):
-        """gets dictionary of parameter values
+        """Gets dictionary of parameter values
         restricted to those expected by base classifier.
         """
         the_params = {}
         for key, val in self.__dict__.items():
             if key in self.basemodel_paramnames:
                 the_params[key] = val
         if deep:
@@ -281,26 +260,25 @@
 
         Note this is overloaded in SafeKerasClassifer
         to deal with tensorflow specifics.
 
         Parameters
         ----------
 
-        name: string
+        name : string
              The name of the file to save
 
         Returns
         -------
 
         Notes
         -----
 
         No return value
 
-
         Optimizer is deliberately excluded.
         To prevent possible to restart training and thus
         possible back door into attacks.
         """
 
         self.model_save_file = name
         if self.model_save_file == "undefined":
@@ -424,15 +402,16 @@
             msg = get_reporting_string(name="changed_param_equal", key=key, val=val)
         return msg
 
     def __check_model_param(
         self, rule: dict, apply_constraints: bool
     ) -> tuple[str, bool]:
         """Checks whether a current model parameter violates a safe rule.
-        Optionally fixes violations."""
+        Optionally fixes violations.
+        """
         disclosive: bool = False
         msg: str = ""
         operator: str = rule["operator"]
         key: str = rule["keyword"]
         val: Any = rule["value"]
         cur_val: Any = getattr(self, key)
         if operator == "min":
@@ -451,15 +430,16 @@
             msg += self.__apply_constraints(operator, key, val, cur_val)
         return msg, disclosive
 
     def __check_model_param_and(
         self, rule: dict, apply_constraints: bool
     ) -> tuple[str, bool]:
         """Checks whether current model parameters violate a logical AND rule.
-        Optionally fixes violations."""
+        Optionally fixes violations.
+        """
         disclosive: bool = False
         msg: str = ""
         for arg in rule["subexpr"]:
             temp_msg, temp_disc = self.__check_model_param(arg, apply_constraints)
             msg += temp_msg
             if temp_disc:
                 disclosive = True
@@ -478,39 +458,35 @@
 
     def preliminary_check(
         self, verbose: bool = True, apply_constraints: bool = False
     ) -> tuple[str, bool]:
         """Checks whether current model parameters violate the safe rules.
         Optionally fixes violations.
 
-
         Parameters
         ----------
 
-        verbose: bool
+        verbose : bool
              A boolean value to determine increased output level.
 
-        apply_constraints: bool
+        apply_constraints : bool
              A boolean to determine whether identified constraints are
              to be upheld and applied.
 
         Returns
         -------
 
-        msg: string
+        msg : string
            A message string
-        disclosive: bool
+        disclosive : bool
            A boolean value indicating whether the model is potentially
            disclosive.
 
-
         Notes
         -----
-
-
         """
         disclosive: bool = False
         msg: str = ""
         notok_start = get_reporting_string(name="warn_possible_disclosure_risk")
         ok_start = get_reporting_string(name="within_recommended_ranges")
         rules: dict = self.__get_constraints()
         for rule in rules:
@@ -534,15 +510,15 @@
 
         if verbose:
             print("Preliminary checks: " + msg)
         return msg, disclosive
 
     def get_current_and_saved_models(self) -> tuple[dict, dict]:
         """Makes a copy of self.__dict__
-        and splits it into dicts for the current and saved versions
+        and splits it into dicts for the current and saved versions.
         """
         current_model = {}
 
         attribute_names_as_list = copy.copy(list(self.__dict__.keys()))
 
         for key in attribute_names_as_list:
             if key not in self.ignore_items:
@@ -570,17 +546,18 @@
             _ = saved_model.pop("saved_model", "Absent")
 
         return current_model, saved_model
 
     def examine_seperate_items(
         self, curr_vals: dict, saved_vals: dict
     ) -> tuple[str, bool]:
-        """comparison of more complex structures
+        """Comparison of more complex structures
         in the super class we just check these model-specific items exist
-        in both current and saved copies"""
+        in both current and saved copies.
+        """
         msg = ""
         disclosive = False
 
         for item in self.examine_seperately_items:
             if curr_vals[item] == "Absent" and saved_vals[item] == "Absent":
                 disclosive = True
                 msg += get_reporting_string(name="both_item_removed", item=item)
@@ -595,15 +572,15 @@
 
         if not disclosive:  # ok, so can call mode-specific extra checks
             msg, disclosive = self.additional_checks(curr_vals, saved_vals)
 
         return msg, disclosive
 
     def posthoc_check(self) -> tuple[str, bool]:  # pylint: disable=too-many-branches
-        """Checks whether model has been interfered with since fit() was last run"""
+        """Checks whether model has been interfered with since fit() was last run."""
 
         disclosive = False
         msg = ""
 
         current_model, saved_model = self.get_current_and_saved_models()
         if len(saved_model) == 0:
             msg = get_reporting_string(name="error_not_called_fit")
@@ -652,40 +629,36 @@
 
         return msg, disclosive
 
     def additional_checks(  # pylint: disable=too-many-branches
         self, curr_separate: dict, saved_separate: dict
     ) -> tuple[str, bool]:
         """Placeholder function for additional posthoc checks e.g. keras this
-        version just checks that any lists have the same contents
-
+        version just checks that any lists have the same contents.
 
         Parameters
         ----------
 
-        curr_separate: python dictionary
-
-        saved_separate: python dictionary
+        curr_separate : python dictionary
 
+        saved_separate : python dictionary
 
         Returns
         -------
 
-        msg: string
+        msg : string
         A message string
-        disclosive: bool
+        disclosive : bool
         A boolean value to indicate whether the model is potentially disclosive.
 
-
         Notes
         -----
 
         posthoc checking makes sure that the two dicts have the same set of
         keys as defined in the list self.examine_separately
-
         """
 
         msg = ""
         disclosive = False
         for item in self.examine_seperately_items:
             if isinstance(curr_separate[item], list):
                 if len(curr_separate[item]) != len(saved_separate[item]):
@@ -704,195 +677,132 @@
                                 f"for parameter list {item}.\n"
                             )
                             disclosive = True
                             break
 
         return msg, disclosive
 
-    def request_release(
-        self, filename: str = "undefined", data_obj: dataset.Data = None
-    ) -> None:  # pylint: disable=too-many-branches
+    def request_release(self, path: str, ext: str, target: Target = None) -> None:
         """Saves model to filename specified and creates a report for the TRE
         output checkers.
 
         Parameters
         ----------
-
-        filename: string
-        The filename used to save the model
-
-        dataobj: object of type Data
-        Contains train/test data and encoding dictionary needed to run attacks
-
-        Returns
-        -------
-
+        path : string
+            Path to save the outputs.
+        ext : str
+            File extension defining the model saved format, e.g., "pkl" or "sav".
+        target : attacks.target.Target
+            Contains model and dataset information.
 
         Notes
         -----
-         1. The dataset object is saved in a file called filebase_data.json
-         (where filebase= filename without the extension)
-         for reference/use by the TRE.
-         Data should never be held or stored with the model.
-         Clearly filebase_data.json mst never leave the TRE.
-         2. If data_obj is not null, then worst case MIA and attribute inference
-         attacks are called via run_attack.
-         Outputs from the attacks will be stored in filebase_attack_res.json
-
-
-
+        If target is not null, then worst case MIA and attribute inference
+        attacks are called via run_attack.
         """
-        if filename == "undefined":  # pragma: no cover
-            print("You must provide the name of the file you want to save your model")
-            print("For security reasons, this will overwrite previous versions")
+        # perform checks
+        msg_prel, disclosive_prel = self.preliminary_check(verbose=False)
+        msg_post, disclosive_post = self.posthoc_check()
+        # prepare results
+        output: dict = {
+            "researcher": self.researcher,
+            "model_type": self.model_type,
+            "details": msg_prel,
+        }
+        if hasattr(self, "k_anonymity"):
+            output["k_anonymity"] = str(self.k_anonymity)
+        if not disclosive_prel and not disclosive_post:
+            output["recommendation"] = "Proceed to next step of checking"
         else:
-            self.save(filename)
-            msg_prel, disclosive_prel = self.preliminary_check(verbose=False)
-            msg_post, disclosive_post = self.posthoc_check()
-
-            output: dict = {
-                "researcher": self.researcher,
-                "model_type": self.model_type,
-                "model_save_file": self.model_save_file,
-                "details": msg_prel,
-            }
-            if hasattr(self, "k_anonymity"):
-                output["k_anonymity"] = f"{self.k_anonymity}"
-            if not disclosive_prel and not disclosive_post:
-                output[
-                    "recommendation"
-                ] = f"Run file {filename} through next step of checking procedure"
-            else:
-                output["recommendation"] = "Do not allow release"
-                output["reason"] = msg_prel + msg_post
-
-            ##Run attacks programmatically if possible
-            if data_obj is not None:
-                # make filenames and save a copy of the data
-                with open(
-                    os.path.splitext(filename)[0] + "_data.pickle", "wb"
-                ) as handle:
-                    pickle.dump(data_obj, handle, protocol=pickle.HIGHEST_PROTOCOL)
-
-                for attack_name in ["worst_case", "lira", "attribute"]:
-                    output[f"{attack_name}_results"] = self.run_attack(
-                        data_obj,
-                        attack_name,
-                        f"{os.path.splitext(filename)[0]}_{attack_name}_res",
-                    )
-
-            now = datetime.datetime.now()
-            self.timestamp = str(now.strftime("%Y-%m-%d %H:%M:%S"))
-            output["timestamp"] = self.timestamp
-
-            outputfilename = self.researcher + "_checkfile.json"
-            data = [output]
-            # load existing results
-            if os.path.isfile(outputfilename):
-                with open(outputfilename, newline="", encoding="utf-8") as file:
-                    try:
-                        data = json.load(file)
-                        data.append(output)
-                    except json.decoder.JSONDecodeError:  # pragma: no cover
-                        logger.warning(
-                            "File %s could not be loaded - overwiting", outputfilename
-                        )
-
-            # write to disk
-            try:
-                with open(outputfilename, "w", newline="", encoding="utf-8") as file:
-                    json.dump(data, file, indent=4, cls=report.NumpyArrayEncoder)
-            except TypeError:  # pragma: no cover
-                logger.warning(
-                    "Error: safemodel could not write non-serialisable "
-                    " outputs to file %s",
-                    outputfilename,
+            output["recommendation"] = "Do not allow release"
+            output["reason"] = msg_prel + msg_post
+        # Run attacks programmatically if possible
+        attack_results_filename = os.path.normpath(f"{path}/attack_results.json")
+        os.makedirs(os.path.dirname(attack_results_filename), exist_ok=True)
+        if target is not None:
+            for attack_name in ["worst_case", "lira", "attribute"]:
+                output[f"{attack_name}_results"] = self.run_attack(
+                    target, attack_name, attack_results_filename
                 )
+        # add timestamp
+        now = datetime.datetime.now()
+        self.timestamp = str(now.strftime("%Y-%m-%d %H:%M:%S"))
+        output["timestamp"] = self.timestamp
+        data = [output]
+        # save output
+        if target is None:
+            target = Target(model=self)
+        target.add_safemodel_results(data)
+        target.save(path, ext)
 
     def run_attack(
         self,
-        data_obj: dataset.Data = None,
+        target: Target = None,
         attack_name: str = "worst_case",
+        outputdir: str = "RES",
         filename: str = "undefined",
     ) -> dict:
-        """Runs a specified attack on the trained model and saves a report to file
+        """Runs a specified attack on the trained model and saves a report to file.
 
         Parameters
         ----------
-        data_obj: Data
-        the dataset in the form of a Data object
-
-        attack_name: string
-
-        filebasename: string
-        Report will be saved to filebasename.json
-
+        target : Target
+            The target in the form of a Target object.
+        attack_name : str
+            Name of the attack to run.
+        filename : str
+            Name of a .json file to save report.
 
         Returns
         -------
-        dict of meta data results
+        dict
+            Metadata results.
 
         Notes
         -----
         Currently implement attack types are:
         Likelihood Ratio: lira
         Worst_Case Membership inference: worst_case
         Single Attribute Inference: attributes
         """
         if attack_name == "worst_case":
-            attack_args = worst_case_attack.WorstCaseAttackArgs(
+            attack_obj = WorstCaseAttack(
                 n_reps=10,
-                # number of baseline (dummy) experiments to do
                 n_dummy_reps=1,
-                # Threshold to determine significance of things
                 p_thresh=0.05,
-                # Filename arguments needed by the code, meaningless if run programmatically
-                in_sample_filename=None,
-                out_sample_filename=None,
-                # Proportion of data to use as a test set for the attack model;
+                training_preds_filename=None,
+                test_preds_filename=None,
                 test_prop=0.5,
-                # Report name is None - don't make json or pdf files
-                report_name=None,
+                output_dir=outputdir,
+                report_name=filename,
             )
-            attack_obj = worst_case_attack.WorstCaseAttack(attack_args)
-            attack_obj.attack(dataset=data_obj, target_model=self)
+            attack_obj.attack(target)
             output = attack_obj.make_report()
             metadata = output["metadata"]
-
         elif attack_name == "lira":
-            args = LIRAAttackArgs(
-                n_shadow_models=100, report_name="lira_example_report"
+            attack_obj = LIRAAttack(
+                n_shadow_models=100,
+                output_dir=outputdir,
+                report_name=filename,
             )
-            attack_obj = LIRAAttack(args)
-            attack_obj.attack(data_obj, self)
-            output = attack_obj.make_report()  # also makes .pdf and .json files
+            attack_obj.attack(target)
+            output = attack_obj.make_report()
             metadata = output["metadata"]
-
         elif attack_name == "attribute":
-            attack_args = attribute_attack.AttributeAttackArgs(
-                report_name="aia_example"
+            attack_obj = AttributeAttack(
+                output_dir=outputdir,
+                report_name=filename,
             )
-            attack_obj = attribute_attack.AttributeAttack(attack_args)
-            attack_obj.attack(data_obj, self)
+            attack_obj.attack(target)
             output = attack_obj.make_report()
             metadata = output["metadata"]
-
         else:
             metadata = {}
             metadata["outcome"] = "unrecognised attack type requested"
-
         print(f"attack {attack_name}, metadata {metadata}")
-
-        try:
-            with open(f"{filename}.json", "w", encoding="utf-8") as fp:
-                json.dump(metadata, fp, cls=report.NumpyArrayEncoder)
-        except TypeError:  # pragma: no cover
-            # not covered in tests as all atttacks prodice simple json so far
-            print(f"couldn't serialise metadata {metadata} for attack {attack_name}")
-
         return metadata
 
     def __str__(self) -> str:  # pragma: no cover
         """Returns string with model description.
-        No point writing a test, especially as it depends on username
+        No point writing a test, especially as it depends on username.
         """
         return self.model_type + " with parameters: " + str(self.__dict__)
```

### Comparing `aisdc-1.0.5.post1/aisdc.egg-info/PKG-INFO` & `aisdc-1.0.6/aisdc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisdc
-Version: 1.0.5.post1
+Version: 1.0.6
 Summary: Tools for the statistical disclosure control of machine learning models
 Home-page: https://github.com/AI-SDC/AI-SDC
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,machine-learning,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aisdc-1.0.5.post1/aisdc.egg-info/SOURCES.txt` & `aisdc-1.0.6/aisdc.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 LICENSE
 README.md
 setup.py
 aisdc/__init__.py
-aisdc/generate_report.py
 aisdc/metrics.py
 aisdc.egg-info/PKG-INFO
 aisdc.egg-info/SOURCES.txt
 aisdc.egg-info/dependency_links.txt
 aisdc.egg-info/requires.txt
 aisdc.egg-info/top_level.txt
 aisdc/attacks/__init__.py
 aisdc/attacks/attack.py
+aisdc/attacks/attack_report_formatter.py
 aisdc/attacks/attribute_attack.py
-aisdc/attacks/dataset.py
 aisdc/attacks/failfast.py
 aisdc/attacks/likelihood_attack.py
+aisdc/attacks/multiple_attacks.py
 aisdc/attacks/report.py
+aisdc/attacks/target.py
 aisdc/attacks/worst_case_attack.py
 aisdc/preprocessing/__init__.py
 aisdc/preprocessing/loaders.py
 aisdc/safemodel/__init__.py
 aisdc/safemodel/reporting.py
 aisdc/safemodel/rules.json
 aisdc/safemodel/safemodel.py
@@ -27,24 +28,25 @@
 aisdc/safemodel/classifiers/dp_svc.py
 aisdc/safemodel/classifiers/new_model_template.py
 aisdc/safemodel/classifiers/safedecisiontreeclassifier.py
 aisdc/safemodel/classifiers/safekeras.py
 aisdc/safemodel/classifiers/saferandomforestclassifier.py
 aisdc/safemodel/classifiers/safesvc.py
 aisdc/safemodel/classifiers/safetf.py
+tests/test_attack_report_formatter.py
 tests/test_attacks.py
-tests/test_attacks_dataset.py
+tests/test_attacks_target.py
 tests/test_attacks_via_safemodel.py
 tests/test_attribute_inference_attack.py
 tests/test_data_interface.py
 tests/test_failfast.py
-tests/test_generate_report.py
 tests/test_lira_attack.py
 tests/test_loaders.py
 tests/test_metrics.py
+tests/test_multiple_attacks.py
 tests/test_safedecisiontreeclassifier.py
 tests/test_safekeras2.py
 tests/test_safemodel.py
 tests/test_saferandomforestclassifier.py
 tests/test_safesvc.py
 tests/test_safetf.py
 tests/test_worst_case_attack.py
```

### Comparing `aisdc-1.0.5.post1/setup.py` & `aisdc-1.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="aisdc",
-    version="1.0.5.post1",
+    version="1.0.6",
     license="MIT",
     maintainer="Jim Smith",
     maintainer_email="james.smith@uwe.ac.uk",
     description="Tools for the statistical disclosure control of machine learning models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AI-SDC/AI-SDC",
@@ -28,14 +28,15 @@
         "numpy~=1.22.0",
         "pandas~=1.5.3",
         "scikit_learn~=1.1.3",
         "scipy~=1.9.0",
         "tensorflow~=2.12.0",
         "tensorflow_privacy==0.8.10",
         "uuid~=1.30",
+        "pypdf~=3.12.2",
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `aisdc-1.0.5.post1/tests/test_attacks.py` & `aisdc-1.0.6/tests/test_attacks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """Jim Smith October 2022
 tests to pick up odd cases not otherwise covered
-in code in the attacks folder
+in code in the attacks folder.
 """
 
 import numpy as np
 import pytest
 from fpdf import FPDF
 
-from aisdc.attacks import attack, dataset, report
+from aisdc.attacks import attack, report
+from aisdc.attacks.target import Target
 from aisdc.safemodel.classifiers import SafeDecisionTreeClassifier
 
 BORDER = 0
 
 
 def test_superclass():
-    """Test that the exceptions are raised if the superclass is called in error"""
+    """Test that the exceptions are raised if the superclass is called in error."""
+    model = SafeDecisionTreeClassifier()
+    target = Target(model=model)
     my_attack = attack.Attack()
-    dataset_obj = dataset.Data()
-    target_obj = SafeDecisionTreeClassifier()
     with pytest.raises(NotImplementedError):
-        my_attack.attack(target_obj, dataset_obj)
+        my_attack.attack(target)
     with pytest.raises(NotImplementedError):
         print(str(my_attack))  # .__str__()
 
 
 def test_NumpyArrayEncoder():
-    """conversion routine
-    from reports.py
+    """Conversion routine
+    from reports.py.
     """
 
     i32 = np.int32(2)
     i64 = np.int64(2)
     twoDarray = np.zeros((2, 2))
     my_encoder = report.NumpyArrayEncoder()
 
@@ -44,23 +45,23 @@
     assert isinstance(retval, list)
 
     with pytest.raises(TypeError):
         retval = my_encoder.default("a string")
 
 
 def test_line():
-    """code from report.py"""
+    """Code from report.py."""
     pdf = FPDF()
     pdf.add_page()
     report.line(pdf, "foo")
     pdf.close()
 
 
 def test_dict():
-    """code from report.py"""
+    """Code from report.py."""
     pdf = FPDF()
     pdf.add_page()
     mydict = {"a": "hello", "b": "world"}
     report._write_dict(  # pylint:disable=protected-access
         pdf, mydict, indent=0, border=BORDER
     )
     pdf.close()
```

### Comparing `aisdc-1.0.5.post1/tests/test_attribute_inference_attack.py` & `aisdc-1.0.6/tests/test_attribute_inference_attack.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 Example demonstrating the attribute inference attacks.
 
 Running
 -------
 
 Invoke this code from the root AI-SDC folder with
 python -m examples.attribute_inference_example
-
 """
+import json
 import os
+import shutil
+import sys
 
 # ignore unused imports because it depends on whether data file is present
 from sklearn.datasets import fetch_openml  # pylint:disable=unused-import
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.preprocessing import (  # pylint:disable=unused-import
     LabelEncoder,
     OneHotEncoder,
@@ -20,99 +22,119 @@
 
 from aisdc.attacks import attribute_attack  # pylint: disable = import-error
 from aisdc.attacks.attribute_attack import (
     _get_bounds_risk,
     _infer_categorical,
     _unique_max,
 )
-from tests.test_attacks_via_safemodel import get_nursery_dataset
+from tests.test_attacks_via_safemodel import get_target
 
 # pylint: disable = duplicate-code
 
 
 def cleanup_file(name: str):
-    """removes unwanted files or directory"""
-    if os.path.exists(name) and os.path.isfile(name):  # h5
-        os.remove(name)
+    """Removes unwanted files or directory."""
+    if os.path.exists(name):
+        if os.path.isfile(name):
+            os.remove(name)
+        elif os.path.isdir(name):
+            shutil.rmtree(name)
 
 
 def common_setup():
-    """basic commands to get ready to test some code"""
-    data = get_nursery_dataset()
+    """Basic commands to get ready to test some code."""
     model = RandomForestClassifier(bootstrap=False)
-    model.fit(data.x_train, data.y_train)
-    attack_args = attribute_attack.AttributeAttackArgs(
-        n_cpu=7, report_name="aia_report"
+    target = get_target(model)
+    model.fit(target.x_train, target.y_train)
+    attack_obj = attribute_attack.AttributeAttack(
+        n_cpu=7,
+        output_dir="test_output_aia",
+        report_name="test_attribute_attack",
     )
-
-    return data, model, attack_args
+    return target, attack_obj
 
 
 def test_attack_args():
-    """tests methods in the attack_args class"""
-    _, _, attack_args = common_setup()
-    _ = attack_args.__str__()  # pylint:disable=unnecessary-dunder-call
-    attack_args.set_param("newkey", True)
-    thedict = attack_args.get_args()
+    """Tests methods in the attack_args class."""
+    _, attack_obj = common_setup()
+    attack_obj.__dict__["newkey"] = True
+    thedict = attack_obj.__dict__
     assert thedict["newkey"] is True
 
 
 def test_unique_max():
-    """tests the _unique_max helper function"""
+    """Tests the _unique_max helper function."""
     has_unique = (0.3, 0.5, 0.2)
     no_unique = (0.5, 0.5)
     assert _unique_max(has_unique, 0.0) is True
     assert _unique_max(has_unique, 0.6) is False
     assert _unique_max(no_unique, 0.0) is False
 
 
 def test_categorical_via_modified_attack_brute_force():
-    """test lots of functionality for categoricals
-    using code from brute_force but without multiprocessing
+    """Test lots of functionality for categoricals
+    using code from brute_force but without multiprocessing.
     """
-    data, model, _ = common_setup()
+    target, _ = common_setup()
 
     threshold = 0
     feature = 0
     # make predictions
-    _infer_categorical(model, data, feature, threshold)
+    _infer_categorical(target, feature, threshold)
     # or don't because threshold is too high
     threshold = 999
-    _infer_categorical(model, data, feature, threshold)
+    _infer_categorical(target, feature, threshold)
 
 
 def test_continuous_via_modified_bounds_risk():
-    """tests a lot of the code for continuous variables
+    """Tests a lot of the code for continuous variables
     via a copy of the _get_bounds_risk()
-    modified not to use multiprocessing
+    modified not to use multiprocessing.
     """
-    data, model, _ = common_setup()
-    _ = _get_bounds_risk(model, "dummy", 8, data.x_train, data.x_test)
+    target, _ = common_setup()
+    _ = _get_bounds_risk(target.model, "dummy", 8, target.x_train, target.x_test)
 
 
 # test below covers a lot of the plotting etc.
 def test_AIA_on_nursery():
-    """tests running AIA on the nursery data
-    with an added continuous feature"""
-    data, model, attack_args = common_setup()
-
-    attack_obj = attribute_attack.AttributeAttack(attack_args)
-    attack_obj.attack(data, model)
+    """Tests running AIA on the nursery data
+    with an added continuous feature.
+    """
+    target, attack_obj = common_setup()
+    attack_obj.attack(target)
 
     output = attack_obj.make_report()
-    output = output["attack_metrics"]
+    output = output["attack_experiment_logger"]["attack_instance_logger"]["instance_0"]
+
+
+def test_AIA_on_nursery_from_cmd():
+    """Tests running AIA on the nursery data
+    with an added continuous feature.
+    """
+    target, _ = common_setup()
+    target.save(path="test_aia_target")
+
+    config = {
+        "n_cpu": 7,
+        "output_dir": "test_output_aia",
+        "report_name": "commandline_aia_exampl1_report",
+    }
+    with open("tests/test_config_aia_cmd.json", "w", encoding="utf-8") as f:
+        f.write(json.dumps(config))
+
+    os.system(
+        f"{sys.executable} -m aisdc.attacks.attribute_attack run-attack-from-configfile "
+        "--attack-config-json-file-name tests/test_config_aia_cmd.json "
+        "--attack-target-folder-path test_aia_target "
+    )
 
 
 def test_cleanup():
-    """tidies up any files created"""
+    """Tidies up any files created."""
     files_made = (
-        "delete-me.json",
-        "aia_example.json",
-        "aia_example.pdf",
-        "aia_report_cat_frac.png",
-        "aia_report_cat_risk.png",
-        "aia_report_quant_risk.png",
-        "aia_report.pdf",
-        "aia_report.json",
+        "test_output_aia/",
+        "test_aia_target/",
+        "test_attribute_attack.json",
+        "tests/test_config_aia_cmd.json",
     )
     for fname in files_made:
         cleanup_file(fname)
```

### Comparing `aisdc-1.0.5.post1/tests/test_data_interface.py` & `aisdc-1.0.6/tests/test_data_interface.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,43 @@
-"""
-Test the data interface code
-"""
+"""Test the data interface code."""
 
 import unittest
 
 import pandas as pd
 
 from aisdc.preprocessing.loaders import (  # pylint: disable = import-error
     UnknownDataset,
     get_data_sklearn,
 )
 
 
 class TestLoaders(unittest.TestCase):
-    """
-    Test the data loaders
-    """
+    """Test the data loaders."""
 
     def test_iris(self):
-        """Nursery data"""
+        """Nursery data."""
         feature_df, target_df = get_data_sklearn("iris")
         self.assertIsInstance(feature_df, pd.DataFrame)
         self.assertIsInstance(target_df, pd.DataFrame)
 
     def test_unknown(self):
-        """
-        Test that a nonsense string raises the correct exception
-        """
+        """Test that a nonsense string raises the correct exception."""
         with self.assertRaises(UnknownDataset):
             _, _ = get_data_sklearn("NONSENSE")
 
     def test_standard(self):
-        """
-        Test that standardisation creates standard features
-        """
+        """Test that standardisation creates standard features."""
         feature_df, _ = get_data_sklearn("standard iris")
         for column in feature_df.columns:
             temp = feature_df[column].mean()
             self.assertAlmostEqual(temp, 0.0)
             temp = feature_df[column].std()
             self.assertAlmostEqual(temp, 1.0)
 
     def test_minmax(self):
-        """
-        Test the minmax scaling
-        """
+        """Test the minmax scaling."""
         feature_df, _ = get_data_sklearn("minmax iris")
         for column in feature_df.columns:
             temp = feature_df[column].min()
             self.assertAlmostEqual(temp, 0.0)
             temp = feature_df[column].max()
             self.assertAlmostEqual(temp, 1.0)
```

### Comparing `aisdc-1.0.5.post1/tests/test_failfast.py` & `aisdc-1.0.6/tests/test_failfast.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,155 +1,157 @@
-"""test_worst_case_attack.py
-Copyright (C) Jim Smith 2022 <james.smith@uwe.ac.uk>
+"""Test_worst_case_attack.py
+Copyright (C) Jim Smith 2022 <james.smith@uwe.ac.uk>.
 """
 from aisdc.attacks import failfast, worst_case_attack  # pylint: disable = import-error
 
 
 def test_parse_boolean_argument():
-    """test all comparison operators and both options for attack
+    """Test all comparison operators and both options for attack
     being successful and not successful given a metric and
-    comparison operator with a threshold value"""
+    comparison operator with a threshold value.
+    """
     metrics = {}
     metrics["ACC"] = 0.9
     metrics["AUC"] = 0.8
     metrics["P_HIGHER_AUC"] = 0.05
 
     # Option 1
-    args = worst_case_attack.WorstCaseAttackArgs(
+    attack_obj = worst_case_attack.WorstCaseAttack(
         attack_metric_success_name="P_HIGHER_AUC",
         attack_metric_success_thresh=0.04,
         attack_metric_success_comp_type="lte",
     )
-    failfast_Obj = failfast.FailFast(args)
+    failfast_Obj = failfast.FailFast(attack_obj)
     assert not failfast_Obj.check_attack_success(metrics)
 
     # Option 2
-    args = worst_case_attack.WorstCaseAttackArgs(
+    attack_obj = worst_case_attack.WorstCaseAttack(
         attack_metric_success_name="P_HIGHER_AUC",
         attack_metric_success_thresh=0.06,
         attack_metric_success_comp_type="lte",
     )
-    failfast_Obj = failfast.FailFast(args)
+    failfast_Obj = failfast.FailFast(attack_obj)
     assert failfast_Obj.check_attack_success(metrics)
 
     # Option 3
-    args = worst_case_attack.WorstCaseAttackArgs(
+    attack_obj = worst_case_attack.WorstCaseAttack(
         attack_metric_success_name="P_HIGHER_AUC",
         attack_metric_success_thresh=0.04,
         attack_metric_success_comp_type="lt",
     )
-    failfast_Obj = failfast.FailFast(args)
+    failfast_Obj = failfast.FailFast(attack_obj)
     assert not failfast_Obj.check_attack_success(metrics)
 
     # Option 4
-    args = worst_case_attack.WorstCaseAttackArgs(
+    attack_obj = worst_case_attack.WorstCaseAttack(
         attack_metric_success_name="P_HIGHER_AUC",
         attack_metric_success_thresh=0.06,
         attack_metric_success_comp_type="lt",
     )
-    failfast_Obj = failfast.FailFast(args)
+    failfast_Obj = failfast.FailFast(attack_obj)
     assert failfast_Obj.check_attack_success(metrics)
 
     # Option 5
-    args = worst_case_attack.WorstCaseAttackArgs(
+    attack_obj = worst_case_attack.WorstCaseAttack(
         attack_metric_success_name="P_HIGHER_AUC",
         attack_metric_success_thresh=0.04,
         attack_metric_success_comp_type="gte",
     )
-    failfast_Obj = failfast.FailFast(args)
+    failfast_Obj = failfast.FailFast(attack_obj)
     assert failfast_Obj.check_attack_success(metrics)
 
     # Option 6
-    args = worst_case_attack.WorstCaseAttackArgs(
+    attack_obj = worst_case_attack.WorstCaseAttack(
         attack_metric_success_name="P_HIGHER_AUC",
         attack_metric_success_thresh=0.06,
         attack_metric_success_comp_type="gte",
     )
-    failfast_Obj = failfast.FailFast(args)
+    failfast_Obj = failfast.FailFast(attack_obj)
     assert not failfast_Obj.check_attack_success(metrics)
 
     # Option 7
-    args = worst_case_attack.WorstCaseAttackArgs(
+    attack_obj = worst_case_attack.WorstCaseAttack(
         attack_metric_success_name="P_HIGHER_AUC",
         attack_metric_success_thresh=0.04,
         attack_metric_success_comp_type="gt",
     )
-    failfast_Obj = failfast.FailFast(args)
+    failfast_Obj = failfast.FailFast(attack_obj)
     assert failfast_Obj.check_attack_success(metrics)
 
     # Option 8
-    args = worst_case_attack.WorstCaseAttackArgs(
+    attack_obj = worst_case_attack.WorstCaseAttack(
         attack_metric_success_name="P_HIGHER_AUC",
         attack_metric_success_thresh=0.06,
         attack_metric_success_comp_type="gt",
     )
-    failfast_Obj = failfast.FailFast(args)
+    failfast_Obj = failfast.FailFast(attack_obj)
     assert not failfast_Obj.check_attack_success(metrics)
 
     # Option 9
-    args = worst_case_attack.WorstCaseAttackArgs(
+    attack_obj = worst_case_attack.WorstCaseAttack(
         attack_metric_success_name="P_HIGHER_AUC",
         attack_metric_success_thresh=0.05,
         attack_metric_success_comp_type="eq",
     )
-    failfast_Obj = failfast.FailFast(args)
+    failfast_Obj = failfast.FailFast(attack_obj)
     assert failfast_Obj.check_attack_success(metrics)
 
     # Option 10
-    args = worst_case_attack.WorstCaseAttackArgs(
+    attack_obj = worst_case_attack.WorstCaseAttack(
         attack_metric_success_name="P_HIGHER_AUC",
         attack_metric_success_thresh=0.06,
         attack_metric_success_comp_type="eq",
     )
-    failfast_Obj = failfast.FailFast(args)
+    failfast_Obj = failfast.FailFast(attack_obj)
     assert not failfast_Obj.check_attack_success(metrics)
 
     # Option 11
-    args = worst_case_attack.WorstCaseAttackArgs(
+    attack_obj = worst_case_attack.WorstCaseAttack(
         attack_metric_success_name="P_HIGHER_AUC",
         attack_metric_success_thresh=0.05,
         attack_metric_success_comp_type="not_eq",
     )
-    failfast_Obj = failfast.FailFast(args)
+    failfast_Obj = failfast.FailFast(attack_obj)
     assert not failfast_Obj.check_attack_success(metrics)
 
     # Option 12
-    args = worst_case_attack.WorstCaseAttackArgs(
+    attack_obj = worst_case_attack.WorstCaseAttack(
         attack_metric_success_name="P_HIGHER_AUC",
         attack_metric_success_thresh=0.06,
         attack_metric_success_comp_type="not_eq",
     )
-    failfast_Obj = failfast.FailFast(args)
+    failfast_Obj = failfast.FailFast(attack_obj)
     assert failfast_Obj.check_attack_success(metrics)
 
     assert failfast_Obj.get_fail_count() == 0
 
 
 def test_attack_success_fail_counts_and_overall_attack_success():
-    """test success and fail counts of attacks for a given threshold
+    """Test success and fail counts of attacks for a given threshold
     of a given metric based on a given comparison operation and
     also test overall attack successes using
-    count threshold of attack being successful or not successful"""
+    count threshold of attack being successful or not successful.
+    """
     metrics = {}
     metrics["ACC"] = 0.9
     metrics["AUC"] = 0.8
     metrics["P_HIGHER_AUC"] = 0.08
-    args = worst_case_attack.WorstCaseAttackArgs(
+    attack_obj = worst_case_attack.WorstCaseAttack(
         attack_metric_success_name="P_HIGHER_AUC",
         attack_metric_success_thresh=0.05,
         attack_metric_success_comp_type="lte",
         attack_metric_success_count_thresh=3,
     )
-    failfast_Obj = failfast.FailFast(args)
+    failfast_Obj = failfast.FailFast(attack_obj)
     _ = failfast_Obj.check_attack_success(metrics)
     metrics["P_HIGHER_AUC"] = 0.07
     _ = failfast_Obj.check_attack_success(metrics)
     metrics["P_HIGHER_AUC"] = 0.03
     _ = failfast_Obj.check_attack_success(metrics)
-    assert not failfast_Obj.check_overall_attack_success(args)
+    assert not failfast_Obj.check_overall_attack_success(attack_obj)
     metrics["P_HIGHER_AUC"] = 0.02
     _ = failfast_Obj.check_attack_success(metrics)
     metrics["P_HIGHER_AUC"] = 0.01
     _ = failfast_Obj.check_attack_success(metrics)
     assert failfast_Obj.get_success_count() == 3
     assert failfast_Obj.get_fail_count() == 2
-    assert failfast_Obj.check_overall_attack_success(args)
+    assert failfast_Obj.check_overall_attack_success(attack_obj)
```

### Comparing `aisdc-1.0.5.post1/tests/test_lira_attack.py` & `aisdc-1.0.6/tests/test_lira_attack.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,83 +1,87 @@
-"""test_lira_attack.py
-Copyright (C) Jim Smith2022  <james.smith@uwe.ac.uk>
+"""Test_lira_attack.py
+Copyright (C) Jim Smith2022  <james.smith@uwe.ac.uk>.
 """
 # pylint: disable = duplicate-code
 
 import logging
 import os
+import shutil
 import sys
 from unittest import TestCase
 
 # import json
 from unittest.mock import patch
 
 import numpy as np
 from sklearn.datasets import load_breast_cancer
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import train_test_split
 
 from aisdc.attacks import likelihood_attack
-from aisdc.attacks.dataset import Data  # pylint: disable = import-error
 from aisdc.attacks.likelihood_attack import (  # pylint: disable = import-error
     DummyClassifier,
     LIRAAttack,
-    LIRAAttackArgs,
 )
+from aisdc.attacks.target import Target  # pylint: disable = import-error
 
 N_SHADOW_MODELS = 20
 
 logger = logging.getLogger(__file__)
 
 
 def clean_up(name):
-    """removes unwanted files or directory"""
-    if os.path.exists(name) and os.path.isfile(name):
-        os.remove(name)
+    """Removes unwanted files or directory."""
+    if os.path.exists(name):
+        if os.path.isfile(name):
+            os.remove(name)
+        elif os.path.isdir(name):
+            shutil.rmtree(name)
         logger.info("Removed %s", name)
 
 
 class TestDummyClassifier(TestCase):
-    """Test the dummy classifier class"""
+    """Test the dummy classifier class."""
 
     @classmethod
     def setUpClass(cls):
-        """Create a dummy classifier object"""
+        """Create a dummy classifier object."""
         cls.dummy = DummyClassifier()
         cls.X = np.array([[0.2, 0.8], [0.7, 0.3]])
 
     def test_predict_proba(self):
-        """Test the predict_proba method"""
+        """Test the predict_proba method."""
         pred_probs = self.dummy.predict_proba(self.X)
         assert np.array_equal(pred_probs, self.X)
 
     def test_predict(self):
-        """Test the predict method"""
+        """Test the predict method."""
         expected_output = np.array([1, 0])
         pred = self.dummy.predict(self.X)
         assert np.array_equal(pred, expected_output)
 
 
 class TestLiraAttack(TestCase):
-    """Test the LIRA attack code"""
+    """Test the LIRA attack code."""
 
     @classmethod
     def setUpClass(cls):
-        """Setup the common things for the class"""
+        """Setup the common things for the class."""
         logger.info("Setting up test class")
         X, y = load_breast_cancer(return_X_y=True, as_frame=False)
         cls.train_X, cls.test_X, cls.train_y, cls.test_y = train_test_split(
             X, y, test_size=0.3
         )
-        cls.dataset = Data()
-        cls.dataset.add_processed_data(cls.train_X, cls.train_y, cls.test_X, cls.test_y)
         cls.target_model = RandomForestClassifier(
             n_estimators=100, min_samples_split=2, min_samples_leaf=1
         )
         cls.target_model.fit(cls.train_X, cls.train_y)
+        cls.target = Target(cls.target_model)
+        cls.target.add_processed_data(cls.train_X, cls.train_y, cls.test_X, cls.test_y)
+        cls.target.save(path="test_lira_target")
 
         # Dump training and test data to csv
         np.savetxt(
             "train_data.csv",
             np.hstack((cls.train_X, cls.train_y[:, None])),
             delimiter=",",
         )
@@ -91,138 +95,170 @@
             delimiter=",",
         )
         np.savetxt(
             "test_preds.csv", cls.target_model.predict_proba(cls.test_X), delimiter=","
         )
 
     def test_lira_attack(self):
-        """tests the lira code two ways"""
-        args = LIRAAttackArgs(
+        """Tests the lira code two ways."""
+        attack_obj = LIRAAttack(
             n_shadow_models=N_SHADOW_MODELS,
-            report_name="lira_example_report",
+            output_dir="test_output_lira",
             attack_config_json_file_name="tests/lrconfig.json",
         )
-        attack_obj = LIRAAttack(args)
         attack_obj.setup_example_data()
         attack_obj.attack_from_config()
         attack_obj.example()
 
-        args2 = LIRAAttackArgs(
-            n_shadow_models=N_SHADOW_MODELS, report_name="lira_example2_report"
+        attack_obj2 = LIRAAttack(
+            n_shadow_models=N_SHADOW_MODELS,
+            output_dir="test_output_lira",
+            report_name="lira_example1_report",
         )
-        attack_obj2 = LIRAAttack(args2)
-        attack_obj2.attack(self.dataset, self.target_model)
+        attack_obj2.attack(self.target)
         output2 = attack_obj2.make_report()  # also makes .pdf and .json files
         n_shadow_models_trained = output2["attack_experiment_logger"][
             "attack_instance_logger"
         ]["instance_0"]["n_shadow_models_trained"]
         n_shadow_models = output2["metadata"]["experiment_details"]["n_shadow_models"]
         assert n_shadow_models_trained == n_shadow_models
 
     def test_check_and_update_dataset(self):
-        """test the code that removes items from test set with classes
-        not present in training set"""
-        args = LIRAAttackArgs(
-            n_shadow_models=N_SHADOW_MODELS, report_name="lira_example_report"
-        )
-        attack_obj = LIRAAttack(args)
+        """Test the code that removes items from test set with classes
+        not present in training set.
+        """
+
+        attack_obj = LIRAAttack(n_shadow_models=N_SHADOW_MODELS)
 
         # now make test[0] have a  class not present in training set#
         local_test_y = np.copy(self.test_y)
         local_test_y[0] = 5
-        local_dataset = Data()
-        local_dataset.add_processed_data(
+        local_target = Target(self.target_model)
+        local_target.add_processed_data(
             self.train_X, self.train_y, self.test_X, local_test_y
         )
         unique_classes_pre = set(local_test_y)
         n_test_examples_pre = len(local_test_y)
-        local_dataset = (
+        local_target = (
             attack_obj._check_and_update_dataset(  # pylint:disable=protected-access
-                local_dataset, self.target_model
+                local_target
             )
         )
 
-        unique_classes_post = set(local_dataset.y_test)
-        n_test_examples_post = len(local_dataset.y_test)
+        unique_classes_post = set(local_target.y_test)
+        n_test_examples_post = len(local_target.y_test)
 
-        self.assertNotEqual(local_dataset.y_test[0], 5)
+        self.assertNotEqual(local_target.y_test[0], 5)
         self.assertEqual(n_test_examples_pre - n_test_examples_post, 1)
         class_diff = unique_classes_pre - unique_classes_post  # set diff
         self.assertSetEqual(class_diff, {5})
 
     def test_main_example(self):
-        """test command line example"""
-        testargs = ["prog", "run-example"]
+        """Test command line example."""
+        testargs = [
+            "prog",
+            "run-example",
+            "--output-dir",
+            "test_output_lira",
+            "--report-name",
+            "commandline_lira_example2_report",
+        ]
         with patch.object(sys, "argv", testargs):
             likelihood_attack.main()
 
     def test_main_config(self):
-        """test command line with a config file"""
-        testargs = ["prog", "run-attack", "-j", "tests/lrconfig.json"]
+        """Test command line with a config file."""
+        testargs = [
+            "prog",
+            "run-attack",
+            "-j",
+            "tests/lrconfig.json",
+            "--output-dir",
+            "test_output_lira",
+            "--report-name",
+            "commandline_lira_example1_report",
+        ]
         with patch.object(sys, "argv", testargs):
             likelihood_attack.main()
 
     def test_main_from_configfile(self):
-        """test command line with a config file"""
+        """Test command line with a config file."""
         testargs = [
             "prog",
             "run-attack-from-configfile",
             "-j",
             "tests/lrconfig_cmd.json",
+            "-t",
+            "test_lira_target",
         ]
         with patch.object(sys, "argv", testargs):
             likelihood_attack.main()
 
     def test_main_example_data(self):
-        """test command line example data creation"""
+        """Test command line example data creation."""
         testargs = ["prog", "setup-example-data"]  # , "--j", "tests/lrconfig.json"]
         with patch.object(sys, "argv", testargs):
             likelihood_attack.main()
 
     def test_lira_attack_failfast_example(self):
-        """tests the lira code two ways"""
-        args = LIRAAttackArgs(
+        """Tests the lira code two ways."""
+        attack_obj = LIRAAttack(
             n_shadow_models=N_SHADOW_MODELS,
-            report_name="lira_example_report",
+            output_dir="test_output_lira",
             attack_config_json_file_name="tests/lrconfig.json",
             shadow_models_fail_fast=True,
             n_shadow_rows_confidences_min=10,
         )
-        attack_obj = LIRAAttack(args)
         attack_obj.setup_example_data()
         attack_obj.attack_from_config()
         attack_obj.example()
 
-    def test_lira_attack_failfast_from_scratch(self):
-        """Test by training a model from scratch"""
-        args = LIRAAttackArgs(
+    def test_lira_attack_failfast_from_scratch1(self):
+        """Test by training a model from scratch."""
+        attack_obj = LIRAAttack(
             n_shadow_models=N_SHADOW_MODELS,
-            report_name="lira_example3_failfast_report",
+            output_dir="test_output_lira",
+            report_name="lira_example2_failfast_report",
             attack_config_json_file_name="tests/lrconfig.json",
             shadow_models_fail_fast=True,
             n_shadow_rows_confidences_min=10,
         )
-        attack_obj = LIRAAttack(args)
-        attack_obj.attack(self.dataset, self.target_model)
+        attack_obj.attack(self.target)
         output = attack_obj.make_report()  # also makes .pdf and .json files
         n_shadow_models_trained = output["attack_experiment_logger"][
             "attack_instance_logger"
         ]["instance_0"]["n_shadow_models_trained"]
         n_shadow_models = output["metadata"]["experiment_details"]["n_shadow_models"]
         assert n_shadow_models_trained == n_shadow_models
 
+    def test_lira_attack_failfast_from_scratch2(self):
+        """Test by training a model from scratch."""
+        attack_obj = LIRAAttack(
+            n_shadow_models=150,
+            output_dir="test_output_lira",
+            report_name="lira_example3_failfast_report",
+            attack_config_json_file_name="tests/lrconfig.json",
+            shadow_models_fail_fast=True,
+            n_shadow_rows_confidences_min=10,
+        )
+        attack_obj.attack(self.target)
+        output = attack_obj.make_report()  # also makes .pdf and .json files
+        n_shadow_models_trained = output["attack_experiment_logger"][
+            "attack_instance_logger"
+        ]["instance_0"]["n_shadow_models_trained"]
+        n_shadow_models = output["metadata"]["experiment_details"]["n_shadow_models"]
+        assert n_shadow_models_trained < n_shadow_models
+
     @classmethod
     def tearDownClass(cls):
-        """cleans up various files made during the tests"""
+        """Cleans up various files made during the tests."""
         names = [
-            "lr_report.pdf",
-            "log_roc.png",
-            "lr_report.json",
-            "lira_example2_report.json",
-            "lira_example2_report.pdf",
+            "test_output_lira/",
+            "output_lira/",
+            "test_lira_target/",
             "test_preds.csv",
             "config.json",
             "train_preds.csv",
             "test_data.csv",
             "train_data.csv",
         ]
         for name in names:
```

### Comparing `aisdc-1.0.5.post1/tests/test_loaders.py` & `aisdc-1.0.6/tests/test_loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-"""test_loaders.py
+"""Test_loaders.py
 Series of functions to use with pytest to check the loaders classes
 Most use just the truncated files with first five examples of each class for brevity.
 Please access the datasets from the sources listed in preprocessing/loaders.py
 Please acknowledge those sources in any publications.
-Jim Smith 2022
+Jim Smith 2022.
 """
 import os
 import shutil
 
 import pytest
 
 from aisdc.preprocessing import loaders
@@ -31,15 +31,15 @@
 )
 
 preprocessing = ("standard", "minmax", "round")
 
 
 def test_get_sklearn_dataset():
     """Test ability to load some standard datasets
-    These loaders only return binary versions
+    These loaders only return binary versions.
     """
     # test preprocessing with iris for speed
     # just gets first two classes
     for routine in preprocessing:
         x_df, y_df = loaders.get_data_sklearn(routine + " iris")
         assert x_df.shape == (100, 4)
         assert y_df.shape == (100, 1)
@@ -52,15 +52,15 @@
     # nursery
     x_df, y_df = loaders.get_data_sklearn("nursery")
     assert x_df.shape == (12960, 27)
     assert y_df.shape == (12960, 1)
 
 
 def test_data_absent():
-    """Tests exceptions raised when datasets have not been downloaded"""
+    """Tests exceptions raised when datasets have not been downloaded."""
     # mimic2
     with pytest.raises(DataNotAvailable):
         _, _ = loaders.get_data_sklearn("mimic2-iaccd")
 
     # in house mortality
     with pytest.raises(DataNotAvailable):
         _, _ = loaders.get_data_sklearn("in-hospital-mortality")
@@ -95,23 +95,24 @@
 
     # unknown
     with pytest.raises(UnknownDataset):
         _, _ = loaders.get_data_sklearn("no such dataset")
 
 
 def test_mimic():
-    """load the mimic2 dataset"""
+    """Load the mimic2 dataset."""
     x_df, y_df = loaders.get_data_sklearn("mimic2-iaccd", DATA_FOLDER)
     assert x_df.shape == (1064, 38), f"x_df shape is {x_df.shape}"
     assert y_df.shape == (1064, 1)
 
 
 def test_in_hospital():
-    """tests loading the in hospital mortality data
-    in two different ways"""
+    """Tests loading the in hospital mortality data
+    in two different ways.
+    """
 
     zip_file_name = os.path.join(DATA_FOLDER, "doi_10.5061_dryad.0p2ngf1zd__v5.zip")
     new_file_name = os.path.join(DATA_FOLDER, "doi_10.5061_dryad.0p2ngf1zd__v5.renamed")
     # first attempt reads from zip file
 
     x_df, y_df = loaders.get_data_sklearn("in-hospital-mortality", DATA_FOLDER)
     assert x_df.shape == (428, 48), f"x_df shape is {x_df.shape}"
@@ -124,15 +125,15 @@
     assert y_df.shape == (428, 1)
 
     # then put the zip file back for next time we run this test
     os.rename(new_file_name, zip_file_name)
 
 
 def test_mnist():
-    """tests loading medical mnist data from different sources"""
+    """Tests loading medical mnist data from different sources."""
     # mnist 100
     # this ne assumes the zip file is present
     x_df, y_df = loaders.get_data_sklearn("medical-mnist-ab-v-br-100", DATA_FOLDER)
     assert x_df.shape == (10, 4096), f"x_df shape is {x_df.shape}"
     assert y_df.shape == (10, 1)
 
     # mnist 500
@@ -157,29 +158,29 @@
     # remove archive folder
     name = os.path.join(DATA_FOLDER, "kaggle-medical-mnist", "archive")
     if os.path.exists(name) and os.path.isdir(name):
         shutil.rmtree(name)
 
 
 def test_indian_liver():
-    """the indian liver dataloader"""
+    """The indian liver dataloader."""
     x_df, y_df = loaders.get_data_sklearn("indian liver", DATA_FOLDER)
     assert x_df.shape == (11, 10), f"x_df shape is {x_df.shape}"
     assert y_df.shape == (11, 1)
 
 
 def test_texas():
-    """the texas dataset has quite restrictive licenses arounbd copying.
+    """The texas dataset has quite restrictive licenses arounbd copying.
     Therefore it is omitted from the CI testing.
-    This code was fully tested during the GRAIMatter project
+    This code was fully tested during the GRAIMatter project.
     """
 
 
 def test_synth_ae():
-    """tests different versions of the  synthetic A&E dataset"""
+    """Tests different versions of the  synthetic A&E dataset."""
     x_df, y_df = loaders.get_data_sklearn("synth-ae", DATA_FOLDER)
     assert x_df.shape == (8, 16), f"x_df shape is {x_df.shape}"
     assert y_df.shape == (8, 1)
 
     # synthae-small
     x_df, y_df = loaders.get_data_sklearn("synth-ae-small", DATA_FOLDER)
     assert x_df.shape == (8, 16), f"x_df shape is {x_df.shape}"
```

### Comparing `aisdc-1.0.5.post1/tests/test_metrics.py` & `aisdc-1.0.6/tests/test_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Test the metrics
-"""
+"""Test the metrics."""
 
 import math
 import unittest
 
 import numpy as np
 import pytest
 
@@ -22,116 +20,94 @@
 TRUE_CLASS = np.array([0, 0, 0, 1, 1, 1])
 PREDICTED_PROBS = np.array(
     [[0.9, 0.1], [0.4, 0.6], [0.8, 0.2], [0.55, 0.45], [0.1, 0.9], [0.01, 0.99]]
 )
 
 
 class DummyClassifier:
-    """
-    Mocks the predict and predict_proba methods
-    """
+    """Mocks the predict and predict_proba methods."""
 
     def predict(self, _):
-        """
-        return dummy predictions
-        """
+        """Return dummy predictions."""
         return PREDICTED_CLASS
 
     def predict_proba(self, _):
-        """
-        return dummy predicted probabilities
-        """
+        """Return dummy predicted probabilities."""
         return PREDICTED_PROBS
 
 
 class TestInputExceptions(unittest.TestCase):
-    """
-    Test that the metrics.py errors with a helpful error message if an invalid shape is supplied
+    """Test that the metrics.py errors with a helpful error message if an
+    invalid shape is supplied.
     """
 
     def _create_fake_test_data(self):
         y_test = np.zeros(4)
         y_test[0] = 1
         return y_test
 
     def test_wrong_shape(self):
-        """
-        Test the check which ensures y_pred_proba is of shape [:,:]
-        """
+        """Test the check which ensures y_pred_proba is of shape [:,:]."""
         y_test = self._create_fake_test_data()
         with pytest.raises(ValueError):
             y_pred_proba = np.zeros((4, 2, 2))
             get_metrics(y_pred_proba, y_test)
 
     def test_wrong_size(self):
-        """
-        Test the check which ensures y_pred_proba is of size (:,2)
-        """
+        """Test the check which ensures y_pred_proba is of size (:,2)."""
         y_test = self._create_fake_test_data()
         with pytest.raises(ValueError):
             y_pred_proba = np.zeros((4, 4))
             get_metrics(y_pred_proba, y_test)
 
     def test_valid_input(self):
-        """
-        Test to make sure a valid array does not throw an exception
-        """
+        """Test to make sure a valid array does not throw an exception."""
         y_test = self._create_fake_test_data()
         y_pred_proba = np.zeros((4, 2))
 
         get_metrics(y_pred_proba, y_test)
 
 
 class TestProbabilities(unittest.TestCase):
-    """
-    Test the checks on the input parameters of the get_probabilites function
-    """
+    """Test the checks on the input parameters of the get_probabilites function."""
 
     def test_permute_rows_errors(self):
         """
         Test to make sure an error is thrown when permute_rows is set to True,
-        but no y_test is supplied
+        but no y_test is supplied.
         """
         clf = DummyClassifier()
         testX = []
 
         with pytest.raises(ValueError):
             get_probabilities(clf, testX, permute_rows=True)
 
     def test_permute_rows_with_permute_rows(self):
-        """
-        Test permute_rows = True succeeds
-        """
+        """Test permute_rows = True succeeds."""
 
         clf = DummyClassifier()
         testX = np.zeros((4, 2))
         testY = np.zeros((4, 2))
 
         get_probabilities(clf, testX, testY, permute_rows=True)
 
     def test_permute_rows_without_permute_rows(self):
-        """
-        Test permute_rows = False succeeds
-        """
+        """Test permute_rows = False succeeds."""
 
         clf = DummyClassifier()
         testX = np.zeros((4, 2))
 
         get_probabilities(clf, testX, permute_rows=False)
 
 
 class TestMetrics(unittest.TestCase):
-    """
-    Test the metrics with some dummy predictions
-    """
+    """Test the metrics with some dummy predictions."""
 
     def test_metrics(self):
-        """
-        Test each individual metric with dummy data
-        """
+        """Test each individual metric with dummy data."""
         clf = DummyClassifier()
         testX = []
         testy = TRUE_CLASS
         y_pred_proba = get_probabilities(clf, testX, testy, permute_rows=False)
         metrics = get_metrics(y_pred_proba, testy)
         self.assertAlmostEqual(metrics["TPR"], 2 / 3)
         self.assertAlmostEqual(metrics["FPR"], 1 / 3)
@@ -142,15 +118,15 @@
         self.assertAlmostEqual(metrics["FNR"], 1 / 3)
         self.assertAlmostEqual(metrics["ACC"], 4 / 6)
         self.assertAlmostEqual(metrics["F1score"], (8 / 9) / (2 / 3 + 2 / 3))
         self.assertAlmostEqual(metrics["Advantage"], 1 / 3)
         self.assertAlmostEqual(metrics["AUC"], 8 / 9)
 
     def test_mia_extremecase(self):
-        """test the extreme case mia in metrics.py"""
+        """Test the extreme case mia in metrics.py."""
 
         # create actual values
         y = np.zeros(50000)
         y[:25] = 1
         # exactly right and wrong predictions
         right = np.zeros(50000)
         right[:25] = 1
@@ -162,20 +138,18 @@
 
         # wrong predictions - probaility very close to 1 so logp=0
         _, _, _, pval = min_max_disc(y, wrong)
         assert math.isclose(pval, 0.0)
 
 
 class TestFPRatTPR(unittest.TestCase):
-    """
-    Test code that computes TPR at fixed FPR
-    """
+    """Test code that computes TPR at fixed FPR."""
 
     def test_tpr(self):
-        """Test tpr at fpr"""
+        """Test tpr at fpr."""
         y_true = TRUE_CLASS
         y_score = PREDICTED_PROBS[:, 1]
 
         tpr = _tpr_at_fpr(y_true, y_score, fpr=0)
         self.assertAlmostEqual(tpr, 2 / 3)
         tpr = _tpr_at_fpr(y_true, y_score, fpr=0.001)
         self.assertAlmostEqual(tpr, 2 / 3)
@@ -186,47 +160,41 @@
         tpr = _tpr_at_fpr(y_true, y_score, fpr=1.0)
         self.assertAlmostEqual(tpr, 1)
         tpr = _tpr_at_fpr(y_true, y_score, fpr_perc=True, fpr=100.0)
         self.assertAlmostEqual(tpr, 1)
 
 
 class Test_Div(unittest.TestCase):
-    """tests the _div functionality"""
+    """Tests the _div functionality."""
 
     def test_div(self):
-        """test div for y=1 and 0"""
+        """Test div for y=1 and 0."""
         result = _div(8.0, 1.0, 99.0)
         self.assertAlmostEqual(result, 8.0)
         result2 = _div(8.0, 0.0, 99.0)
         self.assertAlmostEqual(result2, 99.0)
 
 
 class TestExtreme(unittest.TestCase):
-    """
-    Test the extreme metrics
-    """
+    """Test the extreme metrics."""
 
     def test_extreme_default(self):
-        """
-        Tets with the dummy data
-        """
+        """Tets with the dummy data."""
         pred_probs = DummyClassifier().predict_proba(None)[:, 1]
         maxd, mind, mmd, _ = min_max_disc(TRUE_CLASS, pred_probs)
 
         # 10% of 6 is 1 so:
         # maxd should be 1 (the highest one is predicted as1)
         # mind should be 0 (the lowest one is not predicted as1)
         self.assertAlmostEqual(maxd, 1.0)
         self.assertAlmostEqual(mind, 0.0)
         self.assertAlmostEqual(mmd, 1.0)
 
     def test_extreme_higer_prop(self):
-        """
-        Tets with the dummy data but increase proportion to 0.5
-        """
+        """Tets with the dummy data but increase proportion to 0.5."""
         pred_probs = DummyClassifier().predict_proba(None)[:, 1]
         maxd, mind, mmd, _ = min_max_disc(TRUE_CLASS, pred_probs, x_prop=0.5)
 
         # 10% of 6 is 1 so:
         # maxd should be 1 (the highest one is predicted as1)
         # mind should be 0 (the lowest one is not predicted as1)
         self.assertAlmostEqual(maxd, 2 / 3)
```

### Comparing `aisdc-1.0.5.post1/tests/test_safedecisiontreeclassifier.py` & `aisdc-1.0.6/tests/test_safedecisiontreeclassifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,22 +22,22 @@
     y = np.asarray(iris["target"], dtype=np.float64)
     x = np.vstack([x, (7, 2.0, 4.5, 1)])
     y = np.append(y, 4)
     return x, y
 
 
 def test_reporting():
-    """Check that getting report name requires name"""
+    """Check that getting report name requires name."""
     correct_msg = "Error - get_reporting_string: No 'name' given"
     msg = reporting.get_reporting_string()
     assert msg == correct_msg
 
 
 def test_decision_trees_are_equal():
-    """test the code that compares two decision trees"""
+    """Test the code that compares two decision trees."""
     x1, y = get_data()
     model1 = SafeDecisionTreeClassifier(random_state=1)
     model1.fit(x1, y)
 
     # same
     model2 = SafeDecisionTreeClassifier(random_state=1)
     model2.fit(x1, y)
@@ -66,17 +66,17 @@
 
     # wrong type
     same, _ = decision_trees_are_equal(model1, "aString")
     assert same is False
 
 
 def test_get_tree_k_anonymity():
-    """getting k_anonymity
+    """Getting k_anonymity
     50 data points randomly split in 2, single layer
-    so k should be ~25
+    so k should be ~25.
     """
     x = np.random.rand(50, 2)
     y = np.ones(50)
     for i in range(x.shape[0]):
         if x[i][0] < 0.5:
             y[i] = 0
     model = SafeDecisionTreeClassifier(random_state=1, max_depth=1)
@@ -222,17 +222,18 @@
     correct_msg2 = part1 + part2 + part3 + part4
     print(f"Correct msg2 : {correct_msg2}\n" f"actual mesg2 : {msg2}")
     assert msg2 == correct_msg2
     assert disclosive2 is True
 
 
 def test_data_hiding():
-    """what if the hacking was really obscure
+    """What if the hacking was really obscure
     like putting something in the exceptions list
-     then adding data to current and saved copies"""
+     then adding data to current and saved copies.
+    """
     x, y = get_data()
     model = SafeDecisionTreeClassifier(random_state=1, min_samples_leaf=5)
     model.fit(x, y)
     # now the hack
     model.examine_seperately_items = ["tree_", "bad_string"]
     model.bad_string = "something disclosive"
     model.saved_model["bad_string"] = "something disclosive"
```

### Comparing `aisdc-1.0.5.post1/tests/test_safekeras2.py` & `aisdc-1.0.6/tests/test_safekeras2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """This module contains unit tests for SafeKerasModel."""
 
-import getpass
 import os
 import platform
 import shutil
 
 # shut tensorflow up
 import warnings
 
@@ -27,17 +26,24 @@
 EPOCHS = 1
 n_classes = 4
 # expected accuracy
 ACC = 0.325 if platform.system() == "Darwin" else 0.3583333492279053
 
 UNSAFE_ACC = 0.325 if platform.system() == "Darwin" else 0.3583333492279053
 
+RES_DIR = "RES"
+
+
+def clean():
+    """Removes unwanted results."""
+    shutil.rmtree(RES_DIR)
+
 
 def cleanup_file(name: str):
-    """removes unwanted files or directory"""
+    """Removes unwanted files or directory."""
     if os.path.exists(name) and os.path.isfile(name):  # h5
         os.remove(name)
     elif os.path.exists(name) and os.path.isdir(name):  # tf
         shutil.rmtree(name)
 
 
 def get_data():
@@ -52,15 +58,15 @@
     )
     y = tf.one_hot(y, n_classes)
     yval = tf.one_hot(yval, n_classes)
     return X, y, Xval, yval
 
 
 def make_small_model(num_hidden_layers=2):
-    "Make the keras model"
+    """Make the keras model."""
     # get data
     X, y, Xval, yval = get_data()
     # set seed and kernel initialisers for repeatability
     tf.random.set_seed(12345)
     initializer = tf.keras.initializers.Zeros()
     input_data = Input(shape=X[0].shape)
     xx = Dense(32, activation="relu", kernel_initializer=initializer)(input_data)
@@ -77,31 +83,31 @@
         epochs=EPOCHS,
     )
 
     return model, X, y, Xval, yval
 
 
 def check_init_completed(model: SafeKerasModel):
-    """basic checks for things that happen
-    at end of correct init
+    """Basic checks for things that happen
+    at end of correct init.
     """
     rightname = "KerasModel"
     assert (
         model.model_type == rightname
     ), "failed check for model type being set in init()"
     errstr = (
         "default value of noise_multiplier=0.5"
         "Should have been reset to value 0.7 in rules.json"
     )
     assert model.noise_multiplier == 0.7, errstr
 
 
 def test_init_variants():
     """Test alternative ways of calling init
-    do just with single layer for speed of testing
+    do just with single layer for speed of testing.
     """
     # get data
     X, _, _, _ = get_data()
     # set seed and kernel initialisers for repeatability
     tf.random.set_seed(12345)
     initializer = tf.keras.initializers.Zeros()
 
@@ -140,15 +146,15 @@
         batch_size=0,
     )
     errstr = "failed to correct batch_size=0 in init"
     assert model3.batch_size == 32, errstr
 
 
 def test_same_configs():  # pylint: disable=too-many-locals
-    """check whether tests for equal configuration work"""
+    """Check whether tests for equal configuration work."""
 
     model1, X, _, _, _ = make_small_model(num_hidden_layers=1)
     model2, _, _, _, _ = make_small_model(num_hidden_layers=2)
     model2a, _, _, _, _ = make_small_model(num_hidden_layers=2)
 
     # different numbers of layers
     same1, msg1 = safekeras.same_configs(model1, model2)
@@ -190,15 +196,15 @@
         name="param_changed_from_to", key="units", val="32", cur_val=64
     )
     errstr = f"got message: {msg3}\n" rf"expected.  : {correct_msg3}\."
     assert msg3 == correct_msg3, errstr
 
 
 def test_same_weights():  # pylint : disable=too-many-locals
-    """check the same weights method catches differences"""
+    """Check the same weights method catches differences."""
     # make models to test
     model1, X, _, _, _ = make_small_model(num_hidden_layers=1)
     model2, _, _, _, _ = make_small_model(num_hidden_layers=2)
     input_data = Input(shape=X[0].shape)
     initializer = tf.keras.initializers.Zeros()
     xx = Dense(64, activation="relu", kernel_initializer=initializer)(input_data)
     output = Dense(n_classes, activation="softmax", kernel_initializer=initializer)(xx)
@@ -225,15 +231,15 @@
         f"  {len(model1.layers[1].get_weights()[0][0])} units"
         f" but model2 has {len(model1a.layers[1].get_weights()[0][0])}.\n"
     )
     assert same3 is False, errstr
 
 
 def test_DP_optimizer_checks():
-    """tests the various checks that DP optimiser was used"""
+    """Tests the various checks that DP optimiser was used."""
     # make model
     model1, _, _, _, _ = make_small_model(num_hidden_layers=1)
     loss = tf.keras.losses.CategoricalCrossentropy(
         from_logits=False, reduction=tf.losses.Reduction.NONE
     )
 
     # compile with allowed optimizer and test check works for positive case
@@ -258,15 +264,15 @@
     opt_ok, msg = safekeras.check_optimizer_allowed(model1.optimizer)
     assert opt_ok is False, msg
     opt_is_dp, msg = safekeras.check_optimizer_is_DP(model1.optimizer)
     assert opt_is_dp is False, msg
 
 
 def test_DP_used():
-    """tests the various checks that DP optimiser was used"""
+    """Tests the various checks that DP optimiser was used."""
     # should pass aftyer model compiled **and** fitted with DP optimizer
     model1, X, y, Xval, yval = make_small_model(num_hidden_layers=1)
     loss = tf.keras.losses.CategoricalCrossentropy(
         from_logits=False, reduction=tf.losses.Reduction.NONE
     )
     model1.compile(loss=loss)
     dp_used, msg = safekeras.check_DP_used(model1.optimizer)
@@ -281,15 +287,15 @@
     super(SafeKerasModel, model2).compile(loss=loss, optimizer="SGD")
     model2.fit(X, y, validation_data=(Xval, yval), epochs=EPOCHS, batch_size=20)
     dp_used, msg = safekeras.check_DP_used(model2.optimizer)
     assert dp_used is False, msg
 
 
 def test_checkpoints_are_equal():
-    """test the check for checkpoint equality"""
+    """Test the check for checkpoint equality."""
     model1, X, y, Xval, yval = make_small_model(num_hidden_layers=1)
     loss = tf.keras.losses.CategoricalCrossentropy(
         from_logits=False, reduction=tf.losses.Reduction.NONE
     )
     model1.compile(loss=loss)
     model1.fit(X, y, validation_data=(Xval, yval), epochs=EPOCHS, batch_size=20)
     model1.save("fit.tf")
@@ -323,15 +329,15 @@
     assert same is False, msg
 
     for name in ("fit.tf", "fit2.tf", "refit.tf"):
         cleanup_file(name)
 
 
 def test_load():
-    """Tests the oading functionality"""
+    """Tests the oading functionality."""
 
     # make a model, train then save it
     model, X, y, Xval, yval = make_small_model()
     loss = tf.keras.losses.CategoricalCrossentropy(
         from_logits=False, reduction=tf.losses.Reduction.NONE
     )
     model.compile(loss=loss, optimizer=None)
@@ -353,26 +359,26 @@
     assert isinstance(ypred, np.ndarray)
 
     cleanup_file("keras_save.tf")
     cleanup_file("tfsaves")
 
 
 def test_keras_model_created():
-    "Test keras model"
+    """Test keras model."""
     model, _, _, _, _ = make_small_model()
     rightname = "KerasModel"
     assert (
         model.model_type == rightname
     ), "failed check for model type being set in init()"
     # noise multiplier should have been reset from default to one that matches rules.json
     assert model.noise_multiplier == 0.7
 
 
 def test_second_keras_model_created():
-    "Test second keras model"
+    """Test second keras model."""
     X, _, _, _ = get_data()
     tf.random.set_seed(12345)
     initializer = tf.keras.initializers.Zeros()
     input_data = Input(shape=X[0].shape)
     xx = Dense(128, activation="relu", kernel_initializer=initializer)(input_data)
     xx = Dense(128, activation="relu", kernel_initializer=initializer)(xx)
     xx = Dense(64, activation="relu", kernel_initializer=initializer)(xx)
@@ -396,15 +402,15 @@
         model2.model_type == rightname
     ), "failed check for second model type being set in init()"
     # noise multiplier should have been reset from default to one that matches rules.json
     assert model2.noise_multiplier == 0.7
 
 
 def test_keras_model_compiled_as_DP():
-    "Test Compile DP"
+    """Test Compile DP."""
     model, X, _, _, _ = make_small_model()
     loss = tf.keras.losses.CategoricalCrossentropy(
         from_logits=False, reduction=tf.losses.Reduction.NONE
     )
     model.compile(loss=loss, optimizer=None)
     isDP, _ = safekeras.check_optimizer_is_DP(model.optimizer)
     assert isDP, "failed check that optimizer is dP"
@@ -462,15 +468,15 @@
     msg, disclosive = model.preliminary_check()
     correct_msg = "Model parameters are within recommended ranges.\n"
     assert msg == correct_msg, "failed check params are within range"
     assert disclosive is False, "failed check disclosive is false"
 
 
 def test_keras_save_actions():
-    "Test save action"
+    """Test save action."""
     # create, compile and train model
     model, X, y, Xval, yval = make_small_model()
 
     loss = tf.keras.losses.CategoricalCrossentropy(
         from_logits=False, reduction=tf.losses.Reduction.NONE
     )
     model.compile(loss=loss, optimizer=None)
@@ -710,66 +716,52 @@
     correct_msg = "Model parameters are within recommended ranges.\n"
 
     assert msg == correct_msg, "failed check warning message incorrect"
     assert disclosive is False, "failed check disclosive is false"
 
 
 def test_create_checkfile():
-    """Test create checkfile"""
+    """Test create checkfile."""
     # create, compile and train model
     model, X, y, Xval, yval = make_small_model()
 
     loss = tf.keras.losses.CategoricalCrossentropy(
         from_logits=False, reduction=tf.losses.Reduction.NONE
     )
     model.compile(loss=loss, optimizer=None)
     model.fit(X, y, validation_data=(Xval, yval), epochs=EPOCHS, batch_size=20)
 
     # start with .tf and .h5 which should work
-    names = ("safekeras.tf", "safekeras.h5")
-    for name in names:
-        # clear existing files
-        cleanup_file(name)
-        # save file
+    exts = ("tf", "h5")
+    for ext in exts:
+        name = os.path.normpath(f"{RES_DIR}/model.{ext}")
+        os.makedirs(os.path.dirname(name), exist_ok=True)
+        # check save file
         model.save(name)
         assert os.path.exists(name), f"Failed test to save model as {name}"
-
-        model.request_release(name)
+        clean()
+        # check release
+        model.request_release(path=RES_DIR, ext=ext)
         assert os.path.exists(name), f"Failed test to save model as {name}"
-
-        researcher = getpass.getuser()
-        outputfilename = researcher + "_checkfile.json"
-        assert os.path.exists(
-            outputfilename
-        ), f"Failed test to save checkfile as {outputfilename}"
-
-        # Using readlines()
-        with open(outputfilename, encoding="utf-8") as file1:
-            lines = file1.readlines()
-
-        count = 0
-        # Strips the newline character
-        for line in lines:
-            count += 1
-            print(f"Line{count}: {line.strip()}")
-
-        # clean up
-        cleanup_file(name)
+        name = os.path.normpath(f"{RES_DIR}/target.json")
+        assert os.path.exists(name), "Failed test to save target.json"
+        clean()
 
     # now other versions which should not
-    names = ("safekeras.sav", "safekeras.pkl", "randomfilename", "undefined")
-    for name in names:
-        cleanup_file(name)
+    exts = ("sav", "pkl", "undefined")
+    for ext in exts:
+        name = os.path.normpath(f"{RES_DIR}/model.{ext}")
+        os.makedirs(os.path.dirname(name), exist_ok=True)
         model.save(name)
         assert os.path.exists(name) is False, f"Failed test NOT to save model as {name}"
-        cleanup_file(name)
+        clean()
 
 
 def test_posthoc_check():
-    """testing the posthoc checking function"""
+    """Testing the posthoc checking function."""
     # make a model, train then save it
     model, X, y, Xval, yval = make_small_model()
     loss = tf.keras.losses.CategoricalCrossentropy(
         from_logits=False, reduction=tf.losses.Reduction.NONE
     )
     model.compile(loss=loss, optimizer=None)
     model.fit(X, y, validation_data=(Xval, yval), epochs=1, batch_size=20)
@@ -787,9 +779,9 @@
     assert disclosive is True, "should pick up optimizer changed"
 
     cleanup_file("keras_save.tf")
     cleanup_file("tfsaves")
 
 
 def test_final_cleanup():
-    """clean up any files let around by other tests"""
+    """Clean up any files let around by other tests."""
     cleanup_file("tfsaves")
```

### Comparing `aisdc-1.0.5.post1/tests/test_safemodel.py` & `aisdc-1.0.6/tests/test_safemodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" tests for fnctionality in super class"""
+"""Tests for fnctionality in super class."""
 import copy
 import json
 import os
 import pickle
 
 import joblib
 import numpy as np
@@ -12,32 +12,32 @@
 from aisdc.safemodel.safemodel import SafeModel
 
 notok_start = get_reporting_string(name="warn_possible_disclosure_risk")
 ok_start = get_reporting_string(name="within_recommended_ranges")
 
 
 class DummyClassifier:
-    """Dummy Classifier that always returns predictions of zero"""
+    """Dummy Classifier that always returns predictions of zero."""
 
     # pylint: disable=too-many-arguments
     def __init__(
         self, at_least_5f=5.0, at_most_5i=5, exactly_boo="boo", keyA=True, keyB=True
     ):
-        """dummy init"""
+        """Dummy init."""
         self.at_least_5f = at_least_5f
         self.at_most_5i = at_most_5i
         self.exactly_boo = exactly_boo
         self.keyA = keyA
         self.keyB = keyB
 
     def fit(self, x: np.ndarray, y: np.ndarray):
-        """dummy fit"""
+        """Dummy fit."""
 
     def predict(self, x: np.ndarray):  # pragma: no cover
-        """predict all ones"""
+        """Predict all ones."""
         return np.ones(x.shape[0])
 
 
 def get_data():
     """Returns data for testing."""
     iris = datasets.load_iris()
     x = np.asarray(iris["data"], dtype=np.float64)
@@ -75,38 +75,38 @@
             "timestamp",
         ]
         # create an item to test additional_checks()
         self.examine_seperately_items = ["newthing"]
         self.newthing = ["myStringKey", "aString", "myIntKey", "42"]
 
     def set_params(self, **kwargs):  # pragma: no cover
-        """sets params"""
+        """Sets params."""
         for key, val in kwargs.items():  # pylint:disable=unused-variable
             self.key = val  # pylint:disable=attribute-defined-outside-init
 
     def fit(self, x: np.ndarray, y: np.ndarray):
-        """dummy fit"""
+        """Dummy fit."""
         self.saved_model = copy.deepcopy(self.__dict__)
 
 
 def test_params_checks_ok():
-    """test parameter  checks ok"""
+    """Test parameter  checks ok."""
     model = SafeDummyClassifier()
 
     correct_msg = ok_start
     msg, disclosive = model.preliminary_check()
     print(
         f"exactly_boo is {model.exactly_boo} with type{type(model.exactly_boo).__name__}"
     )
     assert msg == ok_start, f"Correct msg:\n{correct_msg}\nActual msg:\n{msg}\n"
     assert disclosive is False
 
 
 def test_params_checks_too_low():
-    """test parameter  checks too low"""
+    """Test parameter  checks too low."""
     model = SafeDummyClassifier()
 
     model.at_least_5f = 4.0
     msg, disclosive = model.preliminary_check()
     assert disclosive is True
     correct_msg = notok_start + get_reporting_string(
         name="less_than_min_value",
@@ -114,28 +114,28 @@
         cur_val=model.at_least_5f,
         val=5.0,
     )
     assert msg == correct_msg, f"Correct msg:\n{correct_msg}\nActual msg:\n{msg}\n"
 
 
 def test_params_checks_too_high():
-    """test parameter  checks too high"""
+    """Test parameter  checks too high."""
     model = SafeDummyClassifier()
 
     model.at_most_5i = 6
     msg, disclosive = model.preliminary_check()
     assert disclosive is True
     correct_msg = notok_start + get_reporting_string(
         name="greater_than_max_value", key="at_most_5i", cur_val=model.at_most_5i, val=5
     )
     assert msg == correct_msg, f"Correct msg:\n{correct_msg}\nActual msg:\n{msg}\n"
 
 
 def test_params_checks_not_equal():
-    """test parameter  checks not equal"""
+    """Test parameter  checks not equal."""
     model = SafeDummyClassifier()
 
     model.exactly_boo = "foo"
     msg, disclosive = model.preliminary_check()
     assert disclosive is True
     correct_msg = notok_start + get_reporting_string(
         name="different_than_fixed_value",
@@ -143,15 +143,15 @@
         cur_val=model.exactly_boo,
         val="boo",
     )
     assert msg == correct_msg, f"Correct msg:\n{correct_msg}\nActual msg:\n{msg}\n"
 
 
 def test_params_checks_wrong_type_str():
-    """test parameter  checks wrong type - strings given"""
+    """Test parameter  checks wrong type - strings given."""
     model = SafeDummyClassifier()
 
     model.at_least_5f = "five"
     model.at_most_5i = "five"
 
     msg, disclosive = model.preliminary_check()
     assert disclosive is True
@@ -181,15 +181,15 @@
         val="int",
     )
 
     assert msg == correct_msg, f"Correct msg:\n{correct_msg}\nActual msg:\n{msg}\n"
 
 
 def test_params_checks_wrong_type_float():
-    """test parameter  checks wrong_type_float"""
+    """Test parameter  checks wrong_type_float."""
     model = SafeDummyClassifier()
 
     model.exactly_boo = 5.0
     model.at_most_5i = 5.0
 
     _, disclosive = model.preliminary_check()
     assert disclosive is True
@@ -206,15 +206,15 @@
         key="exactly_5",
         cur_val=model.exactly_boo,
         val="int",
     )
 
 
 def test_params_checks_wrong_type_int():
-    """test parameter  checks wrong_type_intt"""
+    """Test parameter  checks wrong_type_intt."""
     model = SafeDummyClassifier()
 
     model.exactly_boo = 5
     model.at_least_5f = 5
 
     msg, disclosive = model.preliminary_check()
     assert disclosive is True
@@ -238,15 +238,15 @@
         cur_val=model.exactly_boo,
         val="boo",
     )
     assert msg == correct_msg, f"Correct msg:\n{correct_msg}\nActual msg:\n{msg}\n"
 
 
 def test_check_unknown_param():
-    """checks handling of malformed json rule"""
+    """Checks handling of malformed json rule."""
     # pylint:disable=protected-access,no-member
     model = SafeDummyClassifier()
     _, _ = model.preliminary_check()
     odd_rule = {"operator": "unknown", "keyword": "exactly_boo", "value": "some_val"}
     msg, disclosive = model._SafeModel__check_model_param(odd_rule, False)
     correct_msg = get_reporting_string(
         name="unknown_operator",
@@ -255,16 +255,16 @@
         cur_val="boo",
     )
     assert msg == correct_msg, f"Correct msg:\n{correct_msg}\nActual msg:\n{msg}\n"
     assert disclosive is False
 
 
 def test_check_model_param_or():
-    """tests or conditions in rules.json
-    the and condition is tested by the decision tree tests
+    """Tests or conditions in rules.json
+    the and condition is tested by the decision tree tests.
     """
     # ok
     model = SafeDummyClassifier()
     msg, disclosive = model.preliminary_check()
     correct_msg = ok_start
     assert msg == correct_msg, f"Correct msg:\n{correct_msg}\nActual msg:\n{msg}\n"
     assert disclosive is False
@@ -301,15 +301,15 @@
     correct_msg = notok_start + part1 + part2
     msg, disclosive = model.preliminary_check()
     assert msg == correct_msg, f"Correct msg:\n{correct_msg}\nActual msg:\n{msg}\n"
     assert disclosive is True
 
 
 def test_saves():
-    """checks that save functions as expected"""
+    """Checks that save functions as expected."""
     model = SafeDummyClassifier()
     x, y = get_data()
     model.fit(x, y)
 
     # no name provided
     model.save()
 
@@ -330,15 +330,15 @@
     # cleanup
     for name in ("dummy.pkl", "dummy.sav", "unpicklable.pkl", "unpicklable.sav"):
         if os.path.exists(name) and os.path.isfile(name):
             os.remove(name)
 
 
 def test_loads():
-    """basic check that making, changing,saving,loading model works"""
+    """Basic check that making, changing,saving,loading model works."""
     model = SafeDummyClassifier()
     x, y = get_data()
     model.fit(x, y)
     # change something in model
     model.exactly_boo = "this_should_be_present"
     assert model.exactly_boo == "this_should_be_present"
 
@@ -357,15 +357,15 @@
     # cleanup
     for name in ("dummy.pkl", "dummy.sav"):
         if os.path.exists(name) and os.path.isfile(name):
             os.remove(name)
 
 
 def test__apply_constraints():
-    """tests constraints can be applied as expected"""
+    """Tests constraints can be applied as expected."""
 
     # wrong type
     model = SafeDummyClassifier()
     model.at_least_5f = 3.9
     model.at_most_5i = 6.2
     model.exactly_boo = "five"
 
@@ -448,16 +448,16 @@
     correct_msg += get_reporting_string(
         name="changed_param_equal", key="exactly_boo", val="boo"
     )
     assert msg == correct_msg, f"Correct msg:\n{correct_msg}\nActual msg:\n{msg}\n"
 
 
 def test_get_saved_model_exception():
-    """tests the exception handling
-    in get_current_and_saved_models()
+    """Tests the exception handling
+    in get_current_and_saved_models().
     """
     model = SafeDummyClassifier()
     # add generator which can't be pickled or copied
 
     model.a_generator = (  # pylint: disable=attribute-defined-outside-init
         i for i in [1, 2, 3]
     )
@@ -465,18 +465,18 @@
     assert saved == {}  # since we haven;t called fit()
     assert (  # pylint: disable=consider-iterating-dictionary
         "a_generator" not in current.keys()
     )
 
 
 def test_generic_additional_tests():
-    """checks the class generic additional tests
+    """Checks the class generic additional tests
     for this purpose SafeDummyClassifier()
     defines
-    self.newthing = {"myStringKey": "aString", "myIntKey": 42}
+    self.newthing = {"myStringKey": "aString", "myIntKey": 42}.
     """
     model = SafeDummyClassifier()
     x, y = get_data()
     model.fit(x, y)
 
     # ok
     msg, disclosive = model.posthoc_check()
@@ -508,45 +508,46 @@
         f"{model.newthing}\n"
         f'{model.saved_model["newthing"]}'
     )
     assert msg == correct_msg, f"Correct msg:\n{correct_msg}\nActual msg:\n{msg}\n"
     assert disclosive is True
 
 
-def test_request_release_without_attcks():
-    """checks requestrelease code works and check the content of the json file"""
+def test_request_release_without_attacks():
+    """Checks requestrelease code works and check the content of the json file."""
     model = SafeDummyClassifier()
     x, y = get_data()
     model.fit(x, y)
     # give it k_anonymity
     model.k_anonymity = 5  # pylint: disable=attribute-defined-outside-init
 
     # no file provided, has k_anonymity
 
-    filename = "test.pkl"
-    json_filename = model.researcher + "_checkfile.json"
-    model.request_release(filename)
+    RES_DIR = "RES"
+    json_filename = os.path.normpath(f"{RES_DIR}/target.json")
+    model_filename = os.path.normpath(f"{RES_DIR}/model.pkl")
+
+    model.request_release(path=RES_DIR, ext="pkl")
 
     # check that pikle and the json files have been created
-    assert os.path.isfile(filename)
+    assert os.path.isfile(model_filename)
     assert os.path.isfile(json_filename)
 
     # check the content of the json file
-    with open(f"./{json_filename}", encoding="utf-8") as file:
+    with open(f"{json_filename}", encoding="utf-8") as file:
         json_data = json.load(file)
 
         details, _ = model.preliminary_check(verbose=False)
         msg_post, _ = model.posthoc_check()
         k_anonymity = f"{model.k_anonymity}"
         recommendation = "Do not allow release"
         reason = details + msg_post
 
         assert {
             "researcher": model.researcher,
             "model_type": model.model_type,
-            "model_save_file": filename,
             "details": details,
             "k_anonymity": k_anonymity,
             "recommendation": recommendation,
             "reason": reason,
             "timestamp": model.timestamp,
-        } in json_data
+        } in json_data["safemodel"]
```

### Comparing `aisdc-1.0.5.post1/tests/test_saferandomforestclassifier.py` & `aisdc-1.0.6/tests/test_saferandomforestclassifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 from aisdc.safemodel.classifiers import SafeRandomForestClassifier
 from aisdc.safemodel.reporting import get_reporting_string
 
 EXPECTED_ACC = 0.9470198675496688  # 5 estimators, min_samples_leaf 5
 
 
 class DummyClassifier:
-    """Dummy Classifier that always returns predictions of zero"""
+    """Dummy Classifier that always returns predictions of zero."""
 
     def __init__(self):
-        """empty init"""
+        """Empty init."""
 
     def fit(self, x: np.ndarray, y: np.ndarray):
-        """empty fit"""
+        """Empty fit."""
 
     def predict(self, x: np.ndarray):
-        """predict all ones"""
+        """Predict all ones."""
 
     #     return np.ones(x.shape[0])
 
 
 def get_data():
     """Returns data for testing."""
     iris = datasets.load_iris()
@@ -161,30 +161,31 @@
     # print(f'Correct: {correct_msg2}\n Actual: {msg2}')
 
     assert msg2 == correct_msg2, f"{msg2}\n should be {correct_msg2}"
     assert disclosive2 is True
 
 
 def test_not_fitted():
-    """posthoc_check() called on unfitred model
-    could have anything injected in classifier parameters"""
+    """Posthoc_check() called on unfitred model
+    could have anything injected in classifier parameters.
+    """
     unfitted_model = SafeRandomForestClassifier(random_state=1, n_estimators=5)
 
     # not fitted
     msg, disclosive = unfitted_model.posthoc_check()
     part1 = get_reporting_string(name="error_not_called_fit")
     part2 = get_reporting_string(name="recommend_do_not_release")
     correct_msg = part1 + part2
     assert msg == correct_msg, f"{msg}\n should be {correct_msg}"
     assert disclosive
 
 
 def test_randomforest_modeltype_changed():
-    """model type has been changed after fit()
-    in this this case to hide some data
+    """Model type has been changed after fit()
+    in this this case to hide some data.
     """
     x, y = get_data()
     model = SafeRandomForestClassifier(random_state=1, n_estimators=5)
     correct_msg = ""
     # check code that tests base_estimator_
     model.fit(x, y)
     model.base_estimator = "DummyClassifier()"
@@ -208,15 +209,15 @@
     print(f"Correct: {correct_msg} Actual: {msg}")
 
     assert msg == correct_msg, f"{msg}\n should be {correct_msg}"
     assert disclosive is True, "should have been flagged as disclosive"
 
 
 def test_randomforest_hacked_postfit_trees_removed():
-    """tests various combinations of removing trees"""
+    """Tests various combinations of removing trees."""
     x, y = get_data()
     model = SafeRandomForestClassifier(random_state=1, n_estimators=5)
     # code that checks estimators_ : one other or both missing or different number or size
     model.fit(x, y)
 
     # tree removed from current
     the_estimators = model.__dict__.pop("estimators_")
@@ -240,15 +241,15 @@
     correct_msg = get_reporting_string(name="saved_item_removed", item="estimators_")
     # print(f'Correct: {correct_msg} Actual: {msg}')
     assert disclosive, "should be flagged as disclosive"
     assert msg == correct_msg, f"{msg}\n should be {correct_msg}"
 
 
 def test_randomforest_hacked_postfit_trees_swapped():
-    """trees swapped with those from a different random forest"""
+    """Trees swapped with those from a different random forest."""
     x, y = get_data()
     model = SafeRandomForestClassifier(random_state=1, n_estimators=5)
     diffsizemodel = SafeRandomForestClassifier(
         random_state=1, n_estimators=5, max_depth=2
     )
 
     # code that checks estimators_ : one other or both missing or different number or size
@@ -276,15 +277,15 @@
     correct_msg = part1 + part2 + part3 + part4
     # print(f'Correct:\n{correct_msg} Actual:\n{msg}')
     assert msg == correct_msg, f"{msg}\n should be {correct_msg}"
     assert disclosive, "should be flagged as disclosive"
 
 
 def test_randomforest_hacked_postfit_moretrees():
-    """trees added after fit"""
+    """Trees added after fit."""
     x, y = get_data()
     model = SafeRandomForestClassifier(random_state=1, n_estimators=5)
     diffsizemodel = SafeRandomForestClassifier(random_state=1, n_estimators=10)
     model.fit(x, y)
     diffsizemodel.fit(x, y)
 
     # swap saved models
```

### Comparing `aisdc-1.0.5.post1/tests/test_safesvc.py` & `aisdc-1.0.6/tests/test_safesvc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Test the various models we have defined
-"""
+"""Test the various models we have defined."""
 
 import unittest
 
 import numpy as np
 from sklearn import datasets
 from sklearn.linear_model import LogisticRegression
 from sklearn.svm import SVC
@@ -18,22 +16,18 @@
     x = np.asarray(cancer["data"], dtype=np.float64)
     y = np.asarray(cancer["target"], dtype=np.float64)
 
     return x, y
 
 
 class TestDPSVC(unittest.TestCase):
-    """
-    Test the differentially private SVC
-    """
+    """Test the differentially private SVC."""
 
     def test_run(self):
-        """
-        Test the model runs
-        """
+        """Test the model runs."""
         dpsvc = SafeSVC()
         svc = SVC(kernel="rbf", gamma="scale", C=1.0, probability=True)
         x, y = get_data()
 
         dpsvc.fit(x, y)
         svc.fit(x, y)
 
@@ -87,23 +81,23 @@
         yplus = y + 5
         errstr = "DP SVC can only handle binary classification"
         with self.assertRaises(Exception) as context:
             model.fit(x, yplus)
         self.assertTrue(errstr in str(context.exception))
 
     def test_svc_gamma_zero(self):
-        """SafeSupportVectorClassifier still makes predictions if we provide daft params"""
+        """SafeSupportVectorClassifier still makes predictions if we provide daft params."""
         x, y = get_data()
         model = SafeSVC(gamma=0.0, eps=0.0)
         model.fit(x, y)
         predictions = model.predict(x)
         assert len(predictions) == len(x)
 
     def test_svc_gamma_auto(self):
-        """SafeSupportVectorClassifier still makes predictions if we provide daft params"""
+        """SafeSupportVectorClassifier still makes predictions if we provide daft params."""
         x, y = get_data()
         model = SafeSVC(gamma="auto")
         model.fit(x, y)
         assert model.gamma == 1.0 / x.shape[1]
 
     def test_svc_setparams(self):
         """SafeSupportVectorClassifier using unchanged values."""
```

### Comparing `aisdc-1.0.5.post1/tests/test_worst_case_attack.py` & `aisdc-1.0.6/tests/test_worst_case_attack.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,288 +1,293 @@
-"""test_worst_case_attack.py
-Copyright (C) Jim Smith 2022 <james.smith@uwe.ac.uk>
+"""Test_worst_case_attack.py
+Copyright (C) Jim Smith 2022 <james.smith@uwe.ac.uk>.
 """
 import json
 import os
+import shutil
 import sys
 from unittest.mock import patch
 
 import numpy as np
 import pytest
 from sklearn.datasets import load_breast_cancer
 from sklearn.model_selection import train_test_split
 from sklearn.svm import SVC
 
-from aisdc.attacks import dataset, worst_case_attack  # pylint: disable = import-error
+from aisdc.attacks import worst_case_attack  # pylint: disable = import-error
+from aisdc.attacks.target import Target
 
 
 def clean_up(name):
-    """removes unwanted files or directory"""
-    if os.path.exists(name) and os.path.isfile(name):
-        os.remove(name)
+    """Removes unwanted files or directory."""
+    if os.path.exists(name):
+        if os.path.isfile(name):
+            os.remove(name)
+        elif os.path.isdir(name):
+            shutil.rmtree(name)
 
 
 def test_config_file_arguments_parsin():
-    """tests reading parameters from the configuration file"""
+    """Tests reading parameters from the configuration file."""
     config = {
         "n_reps": 12,
         "n_dummy_reps": 2,
         "p_thresh": 0.06,
         "test_prop": 0.4,
-        "report_name": "programmatically_worstcase_report_test",
+        "output_dir": "test_output_worstcase",
+        "report_name": "programmatically_worstcase_example1_test",
     }
     with open("config_worstcase_test.json", "w", encoding="utf-8") as f:
         f.write(json.dumps(config))
-    args = worst_case_attack.WorstCaseAttackArgs(
+    attack_obj = worst_case_attack.WorstCaseAttack(
         attack_config_json_file_name="config_worstcase_test.json",
     )
-    assert args.__dict__["n_reps"] == config["n_reps"]
-    assert args.__dict__["n_dummy_reps"] == config["n_dummy_reps"]
-    assert args.__dict__["p_thresh"] == config["p_thresh"]
-    assert args.__dict__["test_prop"] == config["test_prop"]
-    assert args.__dict__["report_name"] == config["report_name"]
+    assert attack_obj.n_reps == config["n_reps"]
+    assert attack_obj.n_dummy_reps == config["n_dummy_reps"]
+    assert attack_obj.p_thresh == config["p_thresh"]
+    assert attack_obj.test_prop == config["test_prop"]
+    assert attack_obj.report_name == config["report_name"]
     os.remove("config_worstcase_test.json")
 
 
 def test_attack_from_predictions_cmd():
-    """Running attack using configuration file and prediction files"""
+    """Running attack using configuration file and prediction files."""
     X, y = load_breast_cancer(return_X_y=True, as_frame=False)
     train_X, test_X, train_y, test_y = train_test_split(X, y, test_size=0.3)
-    dataset_obj = dataset.Data()
-    dataset_obj.add_processed_data(train_X, train_y, test_X, test_y)
+    model = SVC(gamma=0.1, probability=True)
+    model.fit(train_X, train_y)
 
-    target_model = SVC(gamma=0.1, probability=True)
-    target_model.fit(train_X, train_y)
-    ytr_pred = target_model.predict_proba(train_X)
-    yte_pred = target_model.predict_proba(test_X)
+    ytr_pred = model.predict_proba(train_X)
+    yte_pred = model.predict_proba(test_X)
     np.savetxt("ypred_train.csv", ytr_pred, delimiter=",")
     np.savetxt("ypred_test.csv", yte_pred, delimiter=",")
 
+    target = Target(model=model)
+    target.add_processed_data(train_X, train_y, test_X, test_y)
+
+    target.save(path="test_worstcase_target")
+
     config = {
         "n_reps": 30,
         "n_dummy_reps": 2,
         "p_thresh": 0.05,
         "test_prop": 0.5,
+        "output_dir": "test_output_worstcase",
+        "report_name": "commandline_worstcase_example1_report",
         "training_preds_filename": "ypred_train.csv",
         "test_preds_filename": "ypred_test.csv",
         "attack_metric_success_name": "P_HIGHER_AUC",
         "attack_metric_success_thresh": 0.05,
         "attack_metric_success_comp_type": "lte",
         "attack_metric_success_count_thresh": 2,
         "attack_fail_fast": True,
     }
 
     with open("config_worstcase_cmd.json", "w", encoding="utf-8") as f:
         f.write(json.dumps(config))
     os.system(
         f"{sys.executable} -m aisdc.attacks.worst_case_attack run-attack-from-configfile "
         "--attack-config-json-file-name config_worstcase_cmd.json "
+        "--attack-target-folder-path test_worstcase_target "
     )
     os.remove("config_worstcase_cmd.json")
     os.remove("ypred_train.csv")
     os.remove("ypred_test.csv")
 
 
 def test_report_worstcase():
-    """tests worst case attack directly"""
+    """Tests worst case attack directly."""
     X, y = load_breast_cancer(return_X_y=True, as_frame=False)
     train_X, test_X, train_y, test_y = train_test_split(X, y, test_size=0.3)
-    dataset_obj = dataset.Data()
-    dataset_obj.add_processed_data(train_X, train_y, test_X, test_y)
 
-    target_model = SVC(gamma=0.1, probability=True)
-    target_model.fit(train_X, train_y)
-    _ = target_model.predict_proba(train_X)
-    _ = target_model.predict_proba(test_X)
+    model = SVC(gamma=0.1, probability=True)
+    model.fit(train_X, train_y)
+    _ = model.predict_proba(train_X)
+    _ = model.predict_proba(test_X)
+
+    target = Target(model=model)
+    target.add_processed_data(train_X, train_y, test_X, test_y)
 
-    args = worst_case_attack.WorstCaseAttackArgs(
+    # with multiple reps
+    attack_obj = worst_case_attack.WorstCaseAttack(
         # How many attacks to run -- in each the attack model is trained on a different
         # subset of the data
         n_reps=10,
         n_dummy_reps=1,
         p_thresh=0.05,
         training_preds_filename=None,
         test_preds_filename=None,
         test_prop=0.5,
-        report_name="test-10reps",
+        output_dir="test_output_worstcase",
     )
-
-    # with multiple reps
-    attack_obj = worst_case_attack.WorstCaseAttack(args)
-    attack_obj.attack(dataset_obj, target_model)
+    attack_obj.attack(target)
     # attack_obj.make_dummy_data() cause exception when used like this!
     _ = attack_obj.make_report()
 
     # with one rep
-    args = worst_case_attack.WorstCaseAttackArgs(
+    attack_obj = worst_case_attack.WorstCaseAttack(
         n_reps=1,
         n_dummy_reps=1,
         p_thresh=0.05,
         training_preds_filename=None,
         test_preds_filename=None,
         test_prop=0.5,
-        report_name="test-1rep",
+        output_dir="test_output_worstcase",
     )
-
-    attack_obj = worst_case_attack.WorstCaseAttack(args)
-    attack_obj.attack(dataset_obj, target_model)
+    attack_obj.attack(target)
     _ = attack_obj.make_report()
 
 
 def test_attack_with_correct_feature():
-    """Test the attack when the model correctness feature is used"""
+    """Test the attack when the model correctness feature is used."""
     X, y = load_breast_cancer(return_X_y=True, as_frame=False)
     train_X, test_X, train_y, test_y = train_test_split(X, y, test_size=0.3)
-    dataset_obj = dataset.Data()
-    dataset_obj.add_processed_data(train_X, train_y, test_X, test_y)
 
-    target_model = SVC(gamma=0.1, probability=True)
-    target_model.fit(train_X, train_y)
+    model = SVC(gamma=0.1, probability=True)
+    model.fit(train_X, train_y)
+
+    target = Target(model=model)
+    target.add_processed_data(train_X, train_y, test_X, test_y)
 
-    args = worst_case_attack.WorstCaseAttackArgs(
+    # with multiple reps
+    attack_obj = worst_case_attack.WorstCaseAttack(
         # How many attacks to run -- in each the attack model is trained on a different
         # subset of the data
         n_reps=1,
         n_dummy_reps=1,
         p_thresh=0.05,
         training_preds_filename=None,
         test_preds_filename=None,
         test_prop=0.5,
-        report_name="test-1rep",
+        report_name="test-1rep-programmatically_worstcase_example4_test",
         include_model_correct_feature=True,
     )
-
-    # with multiple reps
-    attack_obj = worst_case_attack.WorstCaseAttack(args)
-    attack_obj.attack(dataset_obj, target_model)
+    attack_obj.attack(target)
 
     # Check that attack_metrics has the Yeom metrics
     assert "yeom_tpr" in attack_obj.attack_metrics[0]
     assert "yeom_fpr" in attack_obj.attack_metrics[0]
     assert "yeom_advantage" in attack_obj.attack_metrics[0]
 
 
 def test_attack_from_predictions():
-    """checks code that runs attacks from predictions"""
+    """Checks code that runs attacks from predictions."""
 
     X, y = load_breast_cancer(return_X_y=True, as_frame=False)
     train_X, test_X, train_y, test_y = train_test_split(X, y, test_size=0.3)
-    dataset_obj = dataset.Data()
-    dataset_obj.add_processed_data(train_X, train_y, test_X, test_y)
 
-    target_model = SVC(gamma=0.1, probability=True)
-    target_model.fit(train_X, train_y)
-    ytr_pred = target_model.predict_proba(train_X)
-    yte_pred = target_model.predict_proba(test_X)
+    model = SVC(gamma=0.1, probability=True)
+    model.fit(train_X, train_y)
+    ytr_pred = model.predict_proba(train_X)
+    yte_pred = model.predict_proba(test_X)
     np.savetxt("ypred_train.csv", ytr_pred, delimiter=",")
     np.savetxt("ypred_test.csv", yte_pred, delimiter=",")
 
-    args = worst_case_attack.WorstCaseAttackArgs(
+    target = Target(model=model)
+    target.add_processed_data(train_X, train_y, test_X, test_y)
+
+    attack_obj = worst_case_attack.WorstCaseAttack(
         # How many attacks to run -- in each the attack model is trained on a different
         # subset of the data
         n_reps=10,
         n_dummy_reps=1,
         p_thresh=0.05,
         training_preds_filename="ypred_train.csv",
         test_preds_filename="ypred_test.csv",
         test_prop=0.5,
-        report_name="test-10reps",
+        output_dir="test_output_worstcase",
+        report_name="test-10reps-programmatically_worstcase_example5_test",
     )
 
-    assert args.get_args()["training_preds_filename"] == "ypred_train.csv"
-    print(args)
+    assert attack_obj.training_preds_filename == "ypred_train.csv"
 
     # with multiple reps
-    attack_obj = worst_case_attack.WorstCaseAttack(args)
     attack_obj.attack_from_prediction_files()
 
 
 def test_attack_from_predictions_no_dummy():
-    """checks code that runs attacks from predictions"""
+    """Checks code that runs attacks from predictions."""
 
     X, y = load_breast_cancer(return_X_y=True, as_frame=False)
     train_X, test_X, train_y, test_y = train_test_split(X, y, test_size=0.3)
-    dataset_obj = dataset.Data()
-    dataset_obj.add_processed_data(train_X, train_y, test_X, test_y)
 
-    target_model = SVC(gamma=0.1, probability=True)
-    target_model.fit(train_X, train_y)
-    ytr_pred = target_model.predict_proba(train_X)
-    yte_pred = target_model.predict_proba(test_X)
+    model = SVC(gamma=0.1, probability=True)
+    model.fit(train_X, train_y)
+    ytr_pred = model.predict_proba(train_X)
+    yte_pred = model.predict_proba(test_X)
     np.savetxt("ypred_train.csv", ytr_pred, delimiter=",")
     np.savetxt("ypred_test.csv", yte_pred, delimiter=",")
 
-    args = worst_case_attack.WorstCaseAttackArgs(
+    target = Target(model=model)
+    target.add_processed_data(train_X, train_y, test_X, test_y)
+
+    attack_obj = worst_case_attack.WorstCaseAttack(
         # How many attacks to run -- in each the attack model is trained on a different
         # subset of the data
         n_reps=10,
         n_dummy_reps=0,
         p_thresh=0.05,
         training_preds_filename="ypred_train.csv",
         test_preds_filename="ypred_test.csv",
         test_prop=0.5,
-        report_name="test-10reps",
+        output_dir="test_output_worstcase",
+        report_name="test-10reps-programmatically_worstcase_example6_test",
     )
 
-    assert args.get_args()["training_preds_filename"] == "ypred_train.csv"
-    print(args)
-
+    assert attack_obj.training_preds_filename == "ypred_train.csv"
+    print(attack_obj)
     # with multiple reps
-    attack_obj = worst_case_attack.WorstCaseAttack(args)
     attack_obj.attack_from_prediction_files()
 
 
 def test_dummy_data():
-    """test functionality around creating dummy data"""
-    args = worst_case_attack.WorstCaseAttackArgs(
+    """Test functionality around creating dummy data."""
+    attack_obj = worst_case_attack.WorstCaseAttack(
         # How many attacks to run -- in each the attack model is trained on a different
         # subset of the data
         n_reps=10,
         n_dummy_reps=1,
         p_thresh=0.05,
         training_preds_filename="ypred_train.csv",
         test_preds_filename="ypred_test.csv",
         test_prop=0.5,
-        report_name="test-10reps",
+        output_dir="test_output_worstcase",
+        report_name="test-10reps-programmatically_worstcase_example7_test",
     )
 
-    attack_obj = worst_case_attack.WorstCaseAttack(args)
     attack_obj.make_dummy_data()
 
 
 def test_attack_data_prep():
-    """test the method that prepares the attack data"""
-    args = worst_case_attack.WorstCaseAttackArgs()
-    attack_obj = worst_case_attack.WorstCaseAttack(args)
+    """Test the method that prepares the attack data."""
+    attack_obj = worst_case_attack.WorstCaseAttack()
     train_preds = np.array([[1, 0], [0, 1]], int)
     test_preds = np.array([[2, 0], [0, 2]], int)
 
     mi_x, mi_y = attack_obj._prepare_attack_data(  # pylint: disable=protected-access
         train_preds, test_preds
     )
     np.testing.assert_array_equal(mi_y, np.array([1, 1, 0, 0], np.int))
     # Test the x data produced. Each row should be sorted in descending order
     np.testing.assert_array_equal(mi_x, np.array([[1, 0], [1, 0], [2, 0], [2, 0]]))
-
     # With sort_probs = False, the rows of x should not be sorted
-    args = worst_case_attack.WorstCaseAttackArgs(sort_probs=False)
-    attack_obj = worst_case_attack.WorstCaseAttack(args)
+    attack_obj = worst_case_attack.WorstCaseAttack(sort_probs=False)
     mi_x, mi_y = attack_obj._prepare_attack_data(  # pylint: disable=protected-access
         train_preds, test_preds
     )
     np.testing.assert_array_equal(mi_y, np.array([1, 1, 0, 0], np.int))
     np.testing.assert_array_equal(mi_x, np.array([[1, 0], [0, 1], [2, 0], [0, 2]]))
 
 
 def test_attack_data_prep_with_correct_feature():
-    """test the method that prepares the attack data.
+    """Test the method that prepares the attack data.
     This time, testing that the model correctness values are added, are always
-    the final feature, and are not included in the sorting"""
-    args = worst_case_attack.WorstCaseAttackArgs(include_model_correct_feature=True)
-    attack_obj = worst_case_attack.WorstCaseAttack(args)
+    the final feature, and are not included in the sorting.
+    """
+    attack_obj = worst_case_attack.WorstCaseAttack(include_model_correct_feature=True)
     train_preds = np.array([[1, 0], [0, 1]], int)
     test_preds = np.array([[2, 0], [0, 2]], int)
     train_correct = np.array([1, 0], int)
     test_correct = np.array([0, 1], int)
 
     mi_x, mi_y = attack_obj._prepare_attack_data(  # pylint: disable=protected-access
         train_preds, test_preds, train_correct=train_correct, test_correct=test_correct
@@ -290,56 +295,55 @@
     np.testing.assert_array_equal(mi_y, np.array([1, 1, 0, 0], np.int))
     # Test the x data produced. Each row should be sorted in descending order
     np.testing.assert_array_equal(
         mi_x, np.array([[1, 0, 1], [1, 0, 0], [2, 0, 0], [2, 0, 1]])
     )
 
     # With sort_probs = False, the rows of x should not be sorted
-    args = worst_case_attack.WorstCaseAttackArgs(
+    attack_obj = worst_case_attack.WorstCaseAttack(
         sort_probs=False, include_model_correct_feature=True
     )
-    attack_obj = worst_case_attack.WorstCaseAttack(args)
     mi_x, mi_y = attack_obj._prepare_attack_data(  # pylint: disable=protected-access
         train_preds, test_preds, train_correct=train_correct, test_correct=test_correct
     )
     np.testing.assert_array_equal(mi_y, np.array([1, 1, 0, 0], np.int))
     np.testing.assert_array_equal(
         mi_x, np.array([[1, 0, 1], [0, 1, 0], [2, 0, 0], [0, 2, 1]])
     )
 
 
 def test_non_rf_mia():
     """Tests that it is possible to set the attack model via the args
     In this case, we set as a SVC. But we set probability to false. If the code does
     indeed try and use the SVC (as we want) it will fail as it will try and access
     the predict_proba which won't work if probability=False. Hence, if the code throws
-    an AttributeError we now it *is* trying to use the SVC"""
-
-    args = worst_case_attack.WorstCaseAttackArgs(
-        mia_attack_model=SVC,
-        mia_attack_model_hyp={"kernel": "rbf", "probability": False},
-    )
+    an AttributeError we now it *is* trying to use the SVC.
+    """
 
     X, y = load_breast_cancer(return_X_y=True, as_frame=False)
     train_X, test_X, train_y, test_y = train_test_split(X, y, test_size=0.3)
-    dataset_obj = dataset.Data()
-    dataset_obj.add_processed_data(train_X, train_y, test_X, test_y)
 
-    target_model = SVC(gamma=0.1, probability=True)
-    target_model.fit(train_X, train_y)
-    ytr_pred = target_model.predict_proba(train_X)
-    yte_pred = target_model.predict_proba(test_X)
+    model = SVC(gamma=0.1, probability=True)
+    model.fit(train_X, train_y)
+    ytr_pred = model.predict_proba(train_X)
+    yte_pred = model.predict_proba(test_X)
+
+    target = Target(model=model)
+    target.add_processed_data(train_X, train_y, test_X, test_y)
 
-    attack_obj = worst_case_attack.WorstCaseAttack(args)
+    attack_obj = worst_case_attack.WorstCaseAttack(
+        mia_attack_model=SVC,
+        mia_attack_model_hyp={"kernel": "rbf", "probability": False},
+    )
     with pytest.raises(AttributeError):
         attack_obj.attack_from_preds(ytr_pred, yte_pred)
 
 
 def test_main():
-    """test invocation via command line"""
+    """Test invocation via command line."""
 
     # option 1
     testargs = ["prog", "make-dummy-data"]
     with patch.object(sys, "argv", testargs):
         worst_case_attack.main()
 
     # option 2
@@ -351,23 +355,19 @@
 
     # testargs = ["prog", "run-attack","--no-such-arg"]
     # with patch.object(sys, 'argv', testargs):
     #    worst_case_attack.main()
 
 
 def test_cleanup():
-    """gets rid of files created during tests"""
+    """Gets rid of files created during tests."""
     names = [
-        "worstcase_report.pdf",
-        "log_roc.png",
-        "worstcase_report.json",
+        "test_output_worstcase/",
+        "output_worstcase/",
+        "test_worstcase_target/",
         "test_preds.csv",
         "train_preds.csv",
         "ypred_test.csv",
         "ypred_train.csv",
-        "test-1rep.pdf",
-        "test-1rep.json",
-        "test-10reps.pdf",
-        "test-10reps.json",
     ]
     for name in names:
         clean_up(name)
```

