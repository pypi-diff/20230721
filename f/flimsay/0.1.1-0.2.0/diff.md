# Comparing `tmp/flimsay-0.1.1.tar.gz` & `tmp/flimsay-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flimsay-0.1.1.tar", last modified: Mon Jul 17 17:23:37 2023, max compression
+gzip compressed data, was "flimsay-0.2.0.tar", last modified: Fri Jul 21 13:36:28 2023, max compression
```

## Comparing `flimsay-0.1.1.tar` & `flimsay-0.2.0.tar`

### file list

```diff
@@ -1,64 +1,21 @@
-drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.454033 flimsay-0.1.1/
--rw-r--r--   0 sebastianpaez   (502) staff       (20)       60 2023-07-17 15:53:38.000000 flimsay-0.1.1/.gitignore
--rw-r--r--   0 sebastianpaez   (502) staff       (20)      639 2023-07-17 16:29:58.000000 flimsay-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 sebastianpaez   (502) staff       (20)     8531 2023-07-17 17:23:37.448237 flimsay-0.1.1/PKG-INFO
--rw-r--r--   0 sebastianpaez   (502) staff       (20)     7835 2023-07-17 08:59:32.000000 flimsay-0.1.1/README.md
--rw-r--r--   0 sebastianpaez   (502) staff       (20)     3846 2023-07-17 10:11:50.000000 flimsay-0.1.1/README.qmd
-drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.413510 flimsay-0.1.1/flimsay/
--rw-r--r--   0 sebastianpaez   (502) staff       (20)       74 2023-07-17 10:10:51.000000 flimsay-0.1.1/flimsay/__init__.py
--rw-r--r--   0 sebastianpaez   (502) staff       (20)     9109 2023-07-17 09:22:37.000000 flimsay-0.1.1/flimsay/blib.py
--rw-r--r--   0 sebastianpaez   (502) staff       (20)      472 2023-07-17 08:34:54.000000 flimsay-0.1.1/flimsay/cli.py
--rw-r--r--   0 sebastianpaez   (502) staff       (20)     1014 2023-07-14 08:29:17.000000 flimsay-0.1.1/flimsay/constants.py
--rw-r--r--   0 sebastianpaez   (502) staff       (20)     7017 2023-07-13 22:47:19.000000 flimsay-0.1.1/flimsay/data.py
--rw-r--r--   0 sebastianpaez   (502) staff       (20)    10778 2023-07-17 06:30:27.000000 flimsay-0.1.1/flimsay/features.py
--rw-r--r--   0 sebastianpaez   (502) staff       (20)     1320 2023-07-17 05:36:42.000000 flimsay-0.1.1/flimsay/mass.py
--rw-r--r--   0 sebastianpaez   (502) staff       (20)     2078 2023-07-17 16:24:59.000000 flimsay-0.1.1/flimsay/model.py
-drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.420386 flimsay-0.1.1/flimsay/weights/
--rw-r--r--   0 sebastianpaez   (502) staff       (20)  1750627 2023-07-17 16:09:46.000000 flimsay-0.1.1/flimsay/weights/ccs_model.txt
--rw-r--r--   0 sebastianpaez   (502) staff       (20)  2534003 2023-07-17 16:10:39.000000 flimsay-0.1.1/flimsay/weights/one_over_k0_model.txt
-drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.415657 flimsay-0.1.1/flimsay.egg-info/
--rw-r--r--   0 sebastianpaez   (502) staff       (20)     8531 2023-07-17 17:23:37.000000 flimsay-0.1.1/flimsay.egg-info/PKG-INFO
--rw-r--r--   0 sebastianpaez   (502) staff       (20)     1384 2023-07-17 17:23:37.000000 flimsay-0.1.1/flimsay.egg-info/SOURCES.txt
--rw-r--r--   0 sebastianpaez   (502) staff       (20)        1 2023-07-17 17:23:37.000000 flimsay-0.1.1/flimsay.egg-info/dependency_links.txt
--rw-r--r--   0 sebastianpaez   (502) staff       (20)       44 2023-07-17 17:23:37.000000 flimsay-0.1.1/flimsay.egg-info/entry_points.txt
--rw-r--r--   0 sebastianpaez   (502) staff       (20)      327 2023-07-17 17:23:37.000000 flimsay-0.1.1/flimsay.egg-info/requires.txt
--rw-r--r--   0 sebastianpaez   (502) staff       (20)        8 2023-07-17 17:23:37.000000 flimsay-0.1.1/flimsay.egg-info/top_level.txt
--rw-r--r--   0 sebastianpaez   (502) staff       (20)     3078 2023-07-17 17:02:52.000000 flimsay-0.1.1/pyproject.toml
--rw-r--r--   0 sebastianpaez   (502) staff       (20)       38 2023-07-17 17:23:37.454216 flimsay-0.1.1/setup.cfg
-drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.406264 flimsay-0.1.1/tests/
-drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.425155 flimsay-0.1.1/tests/unit_tests/
--rw-r--r--   0 sebastianpaez   (502) staff       (20)     2773 2023-07-17 16:28:12.000000 flimsay-0.1.1/tests/unit_tests/test_features.py
--rw-r--r--   0 sebastianpaez   (502) staff       (20)     2336 2023-07-17 16:28:29.000000 flimsay-0.1.1/tests/unit_tests/test_model.py
-drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.432263 flimsay-0.1.1/train/
-drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.433192 flimsay-0.1.1/train/.dvc/
--rw-r--r--   0 sebastianpaez   (502) staff       (20)       26 2023-07-10 16:32:37.000000 flimsay-0.1.1/train/.dvc/.gitignore
--rw-r--r--   0 sebastianpaez   (502) staff       (20)       28 2023-07-13 21:12:46.000000 flimsay-0.1.1/train/.dvc/config
--rw-r--r--   0 sebastianpaez   (502) staff       (20)      139 2023-07-10 16:32:37.000000 flimsay-0.1.1/train/.dvcignore
--rw-r--r--   0 sebastianpaez   (502) staff       (20)       20 2023-07-13 18:07:29.000000 flimsay-0.1.1/train/.gitignore
-drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.433847 flimsay-0.1.1/train/data/
--rw-r--r--   0 sebastianpaez   (502) staff       (20)       83 2023-07-14 05:54:25.000000 flimsay-0.1.1/train/data/.gitignore
--rw-r--r--   0 sebastianpaez   (502) staff       (20)     3113 2023-07-17 16:12:22.000000 flimsay-0.1.1/train/dvc.lock
--rw-r--r--   0 sebastianpaez   (502) staff       (20)     2254 2023-07-14 06:01:48.000000 flimsay-0.1.1/train/dvc.yaml
-drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.441917 flimsay-0.1.1/train/plots/
--rw-r--r--   0 sebastianpaez   (502) staff       (20)        0 2023-07-13 21:15:52.000000 flimsay-0.1.1/train/plots/.gitignore
--rw-r--r--   0 sebastianpaez   (502) staff       (20)    40022 2023-07-17 16:09:48.000000 flimsay-0.1.1/train/plots/ccs_cumulative_error.png
--rw-r--r--   0 sebastianpaez   (502) staff       (20)    17478 2023-07-17 16:09:47.000000 flimsay-0.1.1/train/plots/ccs_error.png
--rw-r--r--   0 sebastianpaez   (502) staff       (20)    28471 2023-07-17 16:09:47.000000 flimsay-0.1.1/train/plots/ccs_feature_importance.png
--rw-r--r--   0 sebastianpaez   (502) staff       (20)       60 2023-07-17 16:09:48.000000 flimsay-0.1.1/train/plots/ccs_model_metrics.toml
--rw-r--r--   0 sebastianpaez   (502) staff       (20)   118125 2023-07-17 16:09:47.000000 flimsay-0.1.1/train/plots/ccs_mz_vs_error.png
--rw-r--r--   0 sebastianpaez   (502) staff       (20)    71311 2023-07-17 16:09:47.000000 flimsay-0.1.1/train/plots/ccs_predicted_vs_real.png
--rw-r--r--   0 sebastianpaez   (502) staff       (20)    30423 2023-07-17 16:10:39.000000 flimsay-0.1.1/train/plots/one_over_k0_model_feature_importance.png
--rw-r--r--   0 sebastianpaez   (502) staff       (20)   185052 2023-07-17 16:10:40.000000 flimsay-0.1.1/train/plots/one_over_k0_model_ims_error.png
--rw-r--r--   0 sebastianpaez   (502) staff       (20)    42464 2023-07-17 16:10:40.000000 flimsay-0.1.1/train/plots/one_over_k0_model_ims_error_cumulative.png
--rw-r--r--   0 sebastianpaez   (502) staff       (20)    28422 2023-07-17 16:10:40.000000 flimsay-0.1.1/train/plots/one_over_k0_model_ims_error_hist.png
--rw-r--r--   0 sebastianpaez   (502) staff       (20)    90614 2023-07-17 16:10:41.000000 flimsay-0.1.1/train/plots/one_over_k0_model_ims_pred_vs_true.png
--rw-r--r--   0 sebastianpaez   (502) staff       (20)       66 2023-07-17 16:10:41.000000 flimsay-0.1.1/train/plots/one_over_k0_model_metrics.toml
-drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.444532 flimsay-0.1.1/train/scripts/
--rw-r--r--   0 sebastianpaez   (502) staff       (20)        0 2023-07-14 14:26:09.000000 flimsay-0.1.1/train/scripts/__init__.py
--rw-r--r--   0 sebastianpaez   (502) staff       (20)     4449 2023-07-14 15:40:08.000000 flimsay-0.1.1/train/scripts/dataset_utils.py
--rw-r--r--   0 sebastianpaez   (502) staff       (20)     7037 2023-07-14 15:40:08.000000 flimsay-0.1.1/train/scripts/train_1ok0.py
--rw-r--r--   0 sebastianpaez   (502) staff       (20)     5358 2023-07-14 15:40:08.000000 flimsay-0.1.1/train/scripts/train_ccs.py
-drwxr-xr-x   0 sebastianpaez   (502) staff       (20)        0 2023-07-17 17:23:37.446789 flimsay-0.1.1/train/weights/
--rw-r--r--   0 sebastianpaez   (502) staff       (20)        0 2023-07-13 18:07:02.000000 flimsay-0.1.1/train/weights/.gitignore
--rw-r--r--   0 sebastianpaez   (502) staff       (20)  1750627 2023-07-17 16:09:46.000000 flimsay-0.1.1/train/weights/ccs_model.txt
--rw-r--r--   0 sebastianpaez   (502) staff       (20)  2534003 2023-07-17 16:10:39.000000 flimsay-0.1.1/train/weights/one_over_k0_model.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:36:28.176071 flimsay-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-21 13:36:28.176071 flimsay-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-07-21 13:36:19.000000 flimsay-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:36:28.172071 flimsay-0.2.0/flimsay/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-21 13:31:28.000000 flimsay-0.2.0/flimsay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-07-21 13:31:28.000000 flimsay-0.2.0/flimsay/blib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-21 13:31:28.000000 flimsay-0.2.0/flimsay/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-21 13:31:28.000000 flimsay-0.2.0/flimsay/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-07-21 13:31:28.000000 flimsay-0.2.0/flimsay/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-07-21 13:31:28.000000 flimsay-0.2.0/flimsay/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-21 13:31:28.000000 flimsay-0.2.0/flimsay/mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-21 13:31:28.000000 flimsay-0.2.0/flimsay/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:36:28.176071 flimsay-0.2.0/flimsay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-21 13:36:28.000000 flimsay-0.2.0/flimsay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-21 13:36:28.000000 flimsay-0.2.0/flimsay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:36:28.000000 flimsay-0.2.0/flimsay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 13:36:28.000000 flimsay-0.2.0/flimsay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-21 13:36:28.000000 flimsay-0.2.0/flimsay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 13:36:28.000000 flimsay-0.2.0/flimsay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-21 13:31:28.000000 flimsay-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 13:36:28.176071 flimsay-0.2.0/setup.cfg
```

### Comparing `flimsay-0.1.1/PKG-INFO` & `flimsay-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flimsay
-Version: 0.1.1
+Version: 0.2.0
 Summary: A super simple fast IMS predictor
 Author-email: Sebastian Paez <spaez@talus.bio>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/TalusBio/flimsay
 Project-URL: Documentation, https://TalusBio.github.io/flimsay
 Keywords: proteomics,dia,ion mobility
 Classifier: Programming Language :: Python :: 3
@@ -17,14 +17,16 @@
 Provides-Extra: plot
 Provides-Extra: build
 Provides-Extra: dev
 
 # Flimsy: Fun/Fast Simple IMS Anyone like You can use.
 Sebastian Paez
 
+version = 0.2.0
+
 This repository implements a very simple LGBM model to predict ion
 mobility from peptides.
 
 ## Usage
 
 There are two main ways to interact with `flimsay`, one is using python
 and the other one is using the python api directly.
@@ -39,19 +41,19 @@
 $ flimsay fill_blib mylibrary.blib # This will add ion mobility data to a .blib file.
 ```
 
 ``` python
 ! flimsay fill_blib --help
 ```
 
-
-     Usage: flimsay fill_blib [OPTIONS] BLIB OUT_BLIB
-
-     Add ion mobility prediction to a .blib file.
-
+                                                                                    
+     Usage: flimsay fill_blib [OPTIONS] BLIB OUT_BLIB                               
+                                                                                    
+     Add ion mobility prediction to a .blib file.                                   
+                                                                                    
     ╭─ Options ────────────────────────────────────────────────────────────────────╮
     │ --overwrite      Whether to overwrite output file, if it exists              │
     │ --help           Show this message and exit.                                 │
     ╰──────────────────────────────────────────────────────────────────────────────╯
 
 ### Python
 
@@ -80,15 +82,15 @@
     stripped_sequence_name="Stripped_Seqs",
     calc_masses=True,
     default_charge=2,
 )
 df
 ```
 
-    2023-07-17 01:54:10.066 | WARNING  | flimsay.features:add_features:163 - Charge not provided, using default charge of 2
+    2023-07-21 13:32:38.680 | WARNING  | flimsay.features:add_features:163 - Charge not provided, using default charge of 2
 
 <div>
 <style scoped>
     .dataframe tbody tr th:only-of-type {
         vertical-align: middle;
     }
 &#10;    .dataframe tbody tr th {
@@ -130,15 +132,15 @@
 from flimsay.model import FlimsayModel
 
 model_instance = FlimsayModel()
 
 %timeit model_instance.predict_peptide("MYPEPTIDEK", charge=3)
 ```
 
-    135 µs ± 10.7 µs per loop (mean ± std. dev. of 7 runs, 10,000 loops each)
+    263 µs ± 11.5 µs per loop (mean ± std. dev. of 7 runs, 1,000 loops each)
 
 In my laptop that takes 133 microseconds per peptide, or roughly 7,500
 peptides per second.
 
 #### Batch Prediction
 
 ``` python
@@ -165,17 +167,17 @@
 df = add_features(df, stripped_sequence_name="Stripped_Seqs")
 
 
 # Now we get to run the prediction!
 %timeit model_instance.predict(df)
 ```
 
-    7.79 s ± 1.42 s per loop (mean ± std. dev. of 7 runs, 1 loop each)
+    23.8 s ± 72.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 
-In my system every million peptides is predicted in 8.86 seconds, that is
+In my system every million peptides is predicted in 8.86 seconds, that is  
 113,000 per second.
 
 ## Motivation
 
 There is a fair amount of data on CCS and ion mobility of peptides but
 only very few models actually use features that are directly
 interpretable.
@@ -195,43 +197,43 @@
 
 ``` python
 from flimsay.features import FEATURE_COLUMN_DESCRIPTIONS
 for k,v in FEATURE_COLUMN_DESCRIPTIONS.items():
     print(f">>> The Feature '{k}' is defined as: \n\t{v}")
 ```
 
-    >>> The Feature 'PrecursorMz' is defined as:
+    >>> The Feature 'PrecursorMz' is defined as: 
         Measured precursor m/z
-    >>> The Feature 'Mass' is defined as:
+    >>> The Feature 'Mass' is defined as: 
         Measured precursor mass (Da)
-    >>> The Feature 'PrecursorCharge' is defined as:
+    >>> The Feature 'PrecursorCharge' is defined as: 
         Measured precursor charge, from the isotope envelope
-    >>> The Feature 'PepLength' is defined as:
+    >>> The Feature 'PepLength' is defined as: 
         Length of the peptide sequence in amino acids
-    >>> The Feature 'NumBulky' is defined as:
+    >>> The Feature 'NumBulky' is defined as: 
         Number of bulky amino acids (LVIFWY)
-    >>> The Feature 'NumTiny' is defined as:
+    >>> The Feature 'NumTiny' is defined as: 
         Number of tiny amino acids (AS)
-    >>> The Feature 'NumProlines' is defined as:
+    >>> The Feature 'NumProlines' is defined as: 
         Number of proline residues
-    >>> The Feature 'NumGlycines' is defined as:
+    >>> The Feature 'NumGlycines' is defined as: 
         Number of glycine residues
-    >>> The Feature 'NumSerines' is defined as:
+    >>> The Feature 'NumSerines' is defined as: 
         Number of serine residues
-    >>> The Feature 'NumPos' is defined as:
+    >>> The Feature 'NumPos' is defined as: 
         Number of positive amino acids (KRH)
-    >>> The Feature 'PosIndexL' is defined as:
+    >>> The Feature 'PosIndexL' is defined as: 
         Relative position of the first positive amino acid (KRH)
-    >>> The Feature 'PosIndexR' is defined as:
+    >>> The Feature 'PosIndexR' is defined as: 
         Relative position of the last positive amino acid (KRH)
-    >>> The Feature 'NumNeg' is defined as:
+    >>> The Feature 'NumNeg' is defined as: 
         Number of negative amino acids (DE)
-    >>> The Feature 'NegIndexL' is defined as:
+    >>> The Feature 'NegIndexL' is defined as: 
         Relative position of the first negative amino acid (DE)
-    >>> The Feature 'NegIndexR' is defined as:
+    >>> The Feature 'NegIndexR' is defined as: 
         Relative position of the last negative amino acid (DE)
 
 ## Training
 
 Currently the training logic is handled using DVC (https://dvc.org).
 
 ``` shell
```

### Comparing `flimsay-0.1.1/README.md` & `flimsay-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Flimsy: Fun/Fast Simple IMS Anyone like You can use.
 Sebastian Paez
 
+version = 0.2.0
+
 This repository implements a very simple LGBM model to predict ion
 mobility from peptides.
 
 ## Usage
 
 There are two main ways to interact with `flimsay`, one is using python
 and the other one is using the python api directly.
@@ -19,19 +21,19 @@
 $ flimsay fill_blib mylibrary.blib # This will add ion mobility data to a .blib file.
 ```
 
 ``` python
 ! flimsay fill_blib --help
 ```
 
-
-     Usage: flimsay fill_blib [OPTIONS] BLIB OUT_BLIB
-
-     Add ion mobility prediction to a .blib file.
-
+                                                                                    
+     Usage: flimsay fill_blib [OPTIONS] BLIB OUT_BLIB                               
+                                                                                    
+     Add ion mobility prediction to a .blib file.                                   
+                                                                                    
     ╭─ Options ────────────────────────────────────────────────────────────────────╮
     │ --overwrite      Whether to overwrite output file, if it exists              │
     │ --help           Show this message and exit.                                 │
     ╰──────────────────────────────────────────────────────────────────────────────╯
 
 ### Python
 
@@ -60,15 +62,15 @@
     stripped_sequence_name="Stripped_Seqs",
     calc_masses=True,
     default_charge=2,
 )
 df
 ```
 
-    2023-07-17 01:54:10.066 | WARNING  | flimsay.features:add_features:163 - Charge not provided, using default charge of 2
+    2023-07-21 13:32:38.680 | WARNING  | flimsay.features:add_features:163 - Charge not provided, using default charge of 2
 
 <div>
 <style scoped>
     .dataframe tbody tr th:only-of-type {
         vertical-align: middle;
     }
 &#10;    .dataframe tbody tr th {
@@ -110,15 +112,15 @@
 from flimsay.model import FlimsayModel
 
 model_instance = FlimsayModel()
 
 %timeit model_instance.predict_peptide("MYPEPTIDEK", charge=3)
 ```
 
-    135 µs ± 10.7 µs per loop (mean ± std. dev. of 7 runs, 10,000 loops each)
+    263 µs ± 11.5 µs per loop (mean ± std. dev. of 7 runs, 1,000 loops each)
 
 In my laptop that takes 133 microseconds per peptide, or roughly 7,500
 peptides per second.
 
 #### Batch Prediction
 
 ``` python
@@ -145,17 +147,17 @@
 df = add_features(df, stripped_sequence_name="Stripped_Seqs")
 
 
 # Now we get to run the prediction!
 %timeit model_instance.predict(df)
 ```
 
-    7.79 s ± 1.42 s per loop (mean ± std. dev. of 7 runs, 1 loop each)
+    23.8 s ± 72.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 
-In my system every million peptides is predicted in 8.86 seconds, that is
+In my system every million peptides is predicted in 8.86 seconds, that is  
 113,000 per second.
 
 ## Motivation
 
 There is a fair amount of data on CCS and ion mobility of peptides but
 only very few models actually use features that are directly
 interpretable.
@@ -175,43 +177,43 @@
 
 ``` python
 from flimsay.features import FEATURE_COLUMN_DESCRIPTIONS
 for k,v in FEATURE_COLUMN_DESCRIPTIONS.items():
     print(f">>> The Feature '{k}' is defined as: \n\t{v}")
 ```
 
-    >>> The Feature 'PrecursorMz' is defined as:
+    >>> The Feature 'PrecursorMz' is defined as: 
         Measured precursor m/z
-    >>> The Feature 'Mass' is defined as:
+    >>> The Feature 'Mass' is defined as: 
         Measured precursor mass (Da)
-    >>> The Feature 'PrecursorCharge' is defined as:
+    >>> The Feature 'PrecursorCharge' is defined as: 
         Measured precursor charge, from the isotope envelope
-    >>> The Feature 'PepLength' is defined as:
+    >>> The Feature 'PepLength' is defined as: 
         Length of the peptide sequence in amino acids
-    >>> The Feature 'NumBulky' is defined as:
+    >>> The Feature 'NumBulky' is defined as: 
         Number of bulky amino acids (LVIFWY)
-    >>> The Feature 'NumTiny' is defined as:
+    >>> The Feature 'NumTiny' is defined as: 
         Number of tiny amino acids (AS)
-    >>> The Feature 'NumProlines' is defined as:
+    >>> The Feature 'NumProlines' is defined as: 
         Number of proline residues
-    >>> The Feature 'NumGlycines' is defined as:
+    >>> The Feature 'NumGlycines' is defined as: 
         Number of glycine residues
-    >>> The Feature 'NumSerines' is defined as:
+    >>> The Feature 'NumSerines' is defined as: 
         Number of serine residues
-    >>> The Feature 'NumPos' is defined as:
+    >>> The Feature 'NumPos' is defined as: 
         Number of positive amino acids (KRH)
-    >>> The Feature 'PosIndexL' is defined as:
+    >>> The Feature 'PosIndexL' is defined as: 
         Relative position of the first positive amino acid (KRH)
-    >>> The Feature 'PosIndexR' is defined as:
+    >>> The Feature 'PosIndexR' is defined as: 
         Relative position of the last positive amino acid (KRH)
-    >>> The Feature 'NumNeg' is defined as:
+    >>> The Feature 'NumNeg' is defined as: 
         Number of negative amino acids (DE)
-    >>> The Feature 'NegIndexL' is defined as:
+    >>> The Feature 'NegIndexL' is defined as: 
         Relative position of the first negative amino acid (DE)
-    >>> The Feature 'NegIndexR' is defined as:
+    >>> The Feature 'NegIndexR' is defined as: 
         Relative position of the last negative amino acid (DE)
 
 ## Training
 
 Currently the training logic is handled using DVC (https://dvc.org).
 
 ``` shell
```

### Comparing `flimsay-0.1.1/flimsay/blib.py` & `flimsay-0.2.0/flimsay/blib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import shutil
 import sqlite3
 from pathlib import Path
 
 import pandas as pd
 from loguru import logger
```

### Comparing `flimsay-0.1.1/flimsay/constants.py` & `flimsay-0.2.0/flimsay/constants.py`

 * *Files identical despite different names*

### Comparing `flimsay-0.1.1/flimsay/data.py` & `flimsay-0.2.0/flimsay/data.py`

 * *Files identical despite different names*

### Comparing `flimsay-0.1.1/flimsay/features.py` & `flimsay-0.2.0/flimsay/features.py`

 * *Files identical despite different names*

### Comparing `flimsay-0.1.1/flimsay/mass.py` & `flimsay-0.2.0/flimsay/mass.py`

 * *Files identical despite different names*

### Comparing `flimsay-0.1.1/flimsay/model.py` & `flimsay-0.2.0/flimsay/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from pathlib import Path
 
 import lightgbm as lgb
 import numpy as np
 import pandas as pd
 
 from .features import FEATURE_COLUMNS, seq_to_features
```

### Comparing `flimsay-0.1.1/flimsay.egg-info/PKG-INFO` & `flimsay-0.2.0/flimsay.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flimsay
-Version: 0.1.1
+Version: 0.2.0
 Summary: A super simple fast IMS predictor
 Author-email: Sebastian Paez <spaez@talus.bio>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/TalusBio/flimsay
 Project-URL: Documentation, https://TalusBio.github.io/flimsay
 Keywords: proteomics,dia,ion mobility
 Classifier: Programming Language :: Python :: 3
@@ -17,14 +17,16 @@
 Provides-Extra: plot
 Provides-Extra: build
 Provides-Extra: dev
 
 # Flimsy: Fun/Fast Simple IMS Anyone like You can use.
 Sebastian Paez
 
+version = 0.2.0
+
 This repository implements a very simple LGBM model to predict ion
 mobility from peptides.
 
 ## Usage
 
 There are two main ways to interact with `flimsay`, one is using python
 and the other one is using the python api directly.
@@ -39,19 +41,19 @@
 $ flimsay fill_blib mylibrary.blib # This will add ion mobility data to a .blib file.
 ```
 
 ``` python
 ! flimsay fill_blib --help
 ```
 
-
-     Usage: flimsay fill_blib [OPTIONS] BLIB OUT_BLIB
-
-     Add ion mobility prediction to a .blib file.
-
+                                                                                    
+     Usage: flimsay fill_blib [OPTIONS] BLIB OUT_BLIB                               
+                                                                                    
+     Add ion mobility prediction to a .blib file.                                   
+                                                                                    
     ╭─ Options ────────────────────────────────────────────────────────────────────╮
     │ --overwrite      Whether to overwrite output file, if it exists              │
     │ --help           Show this message and exit.                                 │
     ╰──────────────────────────────────────────────────────────────────────────────╯
 
 ### Python
 
@@ -80,15 +82,15 @@
     stripped_sequence_name="Stripped_Seqs",
     calc_masses=True,
     default_charge=2,
 )
 df
 ```
 
-    2023-07-17 01:54:10.066 | WARNING  | flimsay.features:add_features:163 - Charge not provided, using default charge of 2
+    2023-07-21 13:32:38.680 | WARNING  | flimsay.features:add_features:163 - Charge not provided, using default charge of 2
 
 <div>
 <style scoped>
     .dataframe tbody tr th:only-of-type {
         vertical-align: middle;
     }
 &#10;    .dataframe tbody tr th {
@@ -130,15 +132,15 @@
 from flimsay.model import FlimsayModel
 
 model_instance = FlimsayModel()
 
 %timeit model_instance.predict_peptide("MYPEPTIDEK", charge=3)
 ```
 
-    135 µs ± 10.7 µs per loop (mean ± std. dev. of 7 runs, 10,000 loops each)
+    263 µs ± 11.5 µs per loop (mean ± std. dev. of 7 runs, 1,000 loops each)
 
 In my laptop that takes 133 microseconds per peptide, or roughly 7,500
 peptides per second.
 
 #### Batch Prediction
 
 ``` python
@@ -165,17 +167,17 @@
 df = add_features(df, stripped_sequence_name="Stripped_Seqs")
 
 
 # Now we get to run the prediction!
 %timeit model_instance.predict(df)
 ```
 
-    7.79 s ± 1.42 s per loop (mean ± std. dev. of 7 runs, 1 loop each)
+    23.8 s ± 72.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 
-In my system every million peptides is predicted in 8.86 seconds, that is
+In my system every million peptides is predicted in 8.86 seconds, that is  
 113,000 per second.
 
 ## Motivation
 
 There is a fair amount of data on CCS and ion mobility of peptides but
 only very few models actually use features that are directly
 interpretable.
@@ -195,43 +197,43 @@
 
 ``` python
 from flimsay.features import FEATURE_COLUMN_DESCRIPTIONS
 for k,v in FEATURE_COLUMN_DESCRIPTIONS.items():
     print(f">>> The Feature '{k}' is defined as: \n\t{v}")
 ```
 
-    >>> The Feature 'PrecursorMz' is defined as:
+    >>> The Feature 'PrecursorMz' is defined as: 
         Measured precursor m/z
-    >>> The Feature 'Mass' is defined as:
+    >>> The Feature 'Mass' is defined as: 
         Measured precursor mass (Da)
-    >>> The Feature 'PrecursorCharge' is defined as:
+    >>> The Feature 'PrecursorCharge' is defined as: 
         Measured precursor charge, from the isotope envelope
-    >>> The Feature 'PepLength' is defined as:
+    >>> The Feature 'PepLength' is defined as: 
         Length of the peptide sequence in amino acids
-    >>> The Feature 'NumBulky' is defined as:
+    >>> The Feature 'NumBulky' is defined as: 
         Number of bulky amino acids (LVIFWY)
-    >>> The Feature 'NumTiny' is defined as:
+    >>> The Feature 'NumTiny' is defined as: 
         Number of tiny amino acids (AS)
-    >>> The Feature 'NumProlines' is defined as:
+    >>> The Feature 'NumProlines' is defined as: 
         Number of proline residues
-    >>> The Feature 'NumGlycines' is defined as:
+    >>> The Feature 'NumGlycines' is defined as: 
         Number of glycine residues
-    >>> The Feature 'NumSerines' is defined as:
+    >>> The Feature 'NumSerines' is defined as: 
         Number of serine residues
-    >>> The Feature 'NumPos' is defined as:
+    >>> The Feature 'NumPos' is defined as: 
         Number of positive amino acids (KRH)
-    >>> The Feature 'PosIndexL' is defined as:
+    >>> The Feature 'PosIndexL' is defined as: 
         Relative position of the first positive amino acid (KRH)
-    >>> The Feature 'PosIndexR' is defined as:
+    >>> The Feature 'PosIndexR' is defined as: 
         Relative position of the last positive amino acid (KRH)
-    >>> The Feature 'NumNeg' is defined as:
+    >>> The Feature 'NumNeg' is defined as: 
         Number of negative amino acids (DE)
-    >>> The Feature 'NegIndexL' is defined as:
+    >>> The Feature 'NegIndexL' is defined as: 
         Relative position of the first negative amino acid (DE)
-    >>> The Feature 'NegIndexR' is defined as:
+    >>> The Feature 'NegIndexR' is defined as: 
         Relative position of the last negative amino acid (DE)
 
 ## Training
 
 Currently the training logic is handled using DVC (https://dvc.org).
 
 ``` shell
```

### Comparing `flimsay-0.1.1/pyproject.toml` & `flimsay-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "flimsay"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
     {name = "Sebastian Paez", email = "spaez@talus.bio"},
 ]
 description = "A super simple fast IMS predictor"
 requires-python = ">=3.9,<3.12"
 keywords = ["proteomics", "dia", "ion mobility"]
 license = {text = "Apache 2.0"}
@@ -111,15 +111,15 @@
 target-version = ['py39', 'py310', 'py311']
 preview = true
 
 [tool.isort]
 profile = "black"
 
 [tool.bumpver]
-current_version = "0.1.1"
+current_version = "0.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

