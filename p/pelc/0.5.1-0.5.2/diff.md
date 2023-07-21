# Comparing `tmp/pelc-0.5.1.tar.gz` & `tmp/pelc-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelc-0.5.1.tar", max compression
+gzip compressed data, was "pelc-0.5.2.tar", max compression
```

## Comparing `pelc-0.5.1.tar` & `pelc-0.5.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      153 2023-01-23 15:17:57.130463 pelc-0.5.1/pelc/__init__.py
--rw-r--r--   0        0        0     2124 2023-04-20 20:27:25.207099 pelc-0.5.1/pelc/_input_sanity_check.py
--rw-r--r--   0        0        0     2370 2023-04-03 06:26:08.645035 pelc-0.5.1/pelc/_open_epregistry_databases.py
--rw-r--r--   0        0        0     2380 2023-03-29 12:31:04.739936 pelc-0.5.1/pelc/_unexpected_alleles.py
--rw-r--r--   0        0        0     9731 2023-04-03 06:37:02.236620 pelc-0.5.1/pelc/batch_eplet_comp.py
--rw-r--r--   0        0        0     7935 2023-03-29 12:27:43.032924 pelc-0.5.1/pelc/batch_eplet_comp_aux.py
--rw-r--r--   0        0        0   115455 2023-01-11 14:48:35.472443 pelc-0.5.1/pelc/data/A.csv
--rw-r--r--   0        0        0   138339 2023-04-03 06:26:57.877645 pelc-0.5.1/pelc/data/A_False_A_.pickle
--rw-r--r--   0        0        0     6382 2023-04-03 06:27:12.022395 pelc-0.5.1/pelc/data/A_True_A_.pickle
--rw-r--r--   0        0        0   160035 2023-01-11 14:48:35.523080 pelc-0.5.1/pelc/data/B.csv
--rw-r--r--   0        0        0   209729 2023-04-03 06:26:57.893263 pelc-0.5.1/pelc/data/B_False_B_.pickle
--rw-r--r--   0        0        0    10304 2023-04-03 06:27:12.022395 pelc-0.5.1/pelc/data/B_True_B_.pickle
--rw-r--r--   0        0        0    46142 2023-01-11 14:48:35.546441 pelc-0.5.1/pelc/data/C.csv
--rw-r--r--   0        0        0    62050 2023-04-03 06:26:57.908987 pelc-0.5.1/pelc/data/C_False_C_.pickle
--rw-r--r--   0        0        0     3777 2023-04-03 06:27:12.022395 pelc-0.5.1/pelc/data/C_True_C_.pickle
--rw-r--r--   0        0        0    61100 2023-01-11 14:48:35.675866 pelc-0.5.1/pelc/data/DP.csv
--rw-r--r--   0        0        0   104070 2023-04-03 06:26:57.956271 pelc-0.5.1/pelc/data/DP_False_DPB1_.pickle
--rw-r--r--   0        0        0     9774 2023-04-03 06:27:08.976536 pelc-0.5.1/pelc/data/DP_True_DPB1_.pickle
--rw-r--r--   0        0        0    18294 2023-01-11 14:48:35.718263 pelc-0.5.1/pelc/data/DQ.csv
--rw-r--r--   0        0        0    34476 2023-04-03 06:26:57.940645 pelc-0.5.1/pelc/data/DQ_False_DQB1_.pickle
--rw-r--r--   0        0        0     2479 2023-04-03 06:27:08.976536 pelc-0.5.1/pelc/data/DQ_True_DQB1_.pickle
--rw-r--r--   0        0        0   169376 2023-01-11 14:48:35.855944 pelc-0.5.1/pelc/data/DR.csv
--rw-r--r--   0        0        0   320839 2023-04-03 06:26:57.925016 pelc-0.5.1/pelc/data/DR_False_DRB1_.pickle
--rw-r--r--   0        0        0    12678 2023-04-03 06:27:08.960909 pelc-0.5.1/pelc/data/DR_True_DRB1_.pickle
--rw-r--r--   0        0        0    13281 2023-01-11 15:29:16.746377 pelc-0.5.1/pelc/data/ep_data.csv
--rw-r--r--   0        0        0    16515 2023-04-03 06:26:57.956271 pelc-0.5.1/pelc/data/ep_data.pickle
--rw-r--r--   0        0        0      146 2023-01-09 17:00:55.194758 pelc-0.5.1/pelc/output_type.py
--rw-r--r--   0        0        0     3265 2023-04-03 06:35:26.318686 pelc-0.5.1/pelc/simple_comparison.py
--rw-r--r--   0        0        0      511 2023-04-20 20:29:45.988404 pelc-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     8793 2023-04-20 20:29:45.983993 pelc-0.5.1/README.md
--rw-r--r--   0        0        0     9539 1970-01-01 00:00:00.000000 pelc-0.5.1/setup.py
--rw-r--r--   0        0        0     9104 1970-01-01 00:00:00.000000 pelc-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      153 2023-01-23 15:17:57.130463 pelc-0.5.2/pelc/__init__.py
+-rw-r--r--   0        0        0     2124 2023-04-20 20:27:25.207099 pelc-0.5.2/pelc/_input_sanity_check.py
+-rw-r--r--   0        0        0     2370 2023-04-03 06:26:08.645035 pelc-0.5.2/pelc/_open_epregistry_databases.py
+-rw-r--r--   0        0        0     2380 2023-03-29 12:31:04.739936 pelc-0.5.2/pelc/_unexpected_alleles.py
+-rw-r--r--   0        0        0    10287 2023-07-21 13:34:31.293683 pelc-0.5.2/pelc/batch_eplet_comp.py
+-rw-r--r--   0        0        0     7935 2023-03-29 12:27:43.032924 pelc-0.5.2/pelc/batch_eplet_comp_aux.py
+-rw-r--r--   0        0        0   115455 2023-01-11 14:48:35.472443 pelc-0.5.2/pelc/data/A.csv
+-rw-r--r--   0        0        0   138339 2023-04-03 06:26:57.877645 pelc-0.5.2/pelc/data/A_False_A_.pickle
+-rw-r--r--   0        0        0     6382 2023-04-03 06:27:12.022395 pelc-0.5.2/pelc/data/A_True_A_.pickle
+-rw-r--r--   0        0        0   160035 2023-01-11 14:48:35.523080 pelc-0.5.2/pelc/data/B.csv
+-rw-r--r--   0        0        0   209729 2023-04-03 06:26:57.893263 pelc-0.5.2/pelc/data/B_False_B_.pickle
+-rw-r--r--   0        0        0    10304 2023-04-03 06:27:12.022395 pelc-0.5.2/pelc/data/B_True_B_.pickle
+-rw-r--r--   0        0        0    46142 2023-01-11 14:48:35.546441 pelc-0.5.2/pelc/data/C.csv
+-rw-r--r--   0        0        0    62050 2023-04-03 06:26:57.908987 pelc-0.5.2/pelc/data/C_False_C_.pickle
+-rw-r--r--   0        0        0     3777 2023-04-03 06:27:12.022395 pelc-0.5.2/pelc/data/C_True_C_.pickle
+-rw-r--r--   0        0        0    61100 2023-01-11 14:48:35.675866 pelc-0.5.2/pelc/data/DP.csv
+-rw-r--r--   0        0        0   104070 2023-04-03 06:26:57.956271 pelc-0.5.2/pelc/data/DP_False_DPB1_.pickle
+-rw-r--r--   0        0        0     9774 2023-04-03 06:27:08.976536 pelc-0.5.2/pelc/data/DP_True_DPB1_.pickle
+-rw-r--r--   0        0        0    18294 2023-01-11 14:48:35.718263 pelc-0.5.2/pelc/data/DQ.csv
+-rw-r--r--   0        0        0    34476 2023-04-03 06:26:57.940645 pelc-0.5.2/pelc/data/DQ_False_DQB1_.pickle
+-rw-r--r--   0        0        0     2479 2023-04-03 06:27:08.976536 pelc-0.5.2/pelc/data/DQ_True_DQB1_.pickle
+-rw-r--r--   0        0        0   169376 2023-01-11 14:48:35.855944 pelc-0.5.2/pelc/data/DR.csv
+-rw-r--r--   0        0        0   320839 2023-04-03 06:26:57.925016 pelc-0.5.2/pelc/data/DR_False_DRB1_.pickle
+-rw-r--r--   0        0        0    12678 2023-04-03 06:27:08.960909 pelc-0.5.2/pelc/data/DR_True_DRB1_.pickle
+-rw-r--r--   0        0        0    13281 2023-01-11 15:29:16.746377 pelc-0.5.2/pelc/data/ep_data.csv
+-rw-r--r--   0        0        0    16515 2023-04-03 06:26:57.956271 pelc-0.5.2/pelc/data/ep_data.pickle
+-rw-r--r--   0        0        0      146 2023-01-09 17:00:55.194758 pelc-0.5.2/pelc/output_type.py
+-rw-r--r--   0        0        0     3265 2023-04-03 06:35:26.318686 pelc-0.5.2/pelc/simple_comparison.py
+-rw-r--r--   0        0        0      511 2023-07-21 14:35:10.888718 pelc-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     9114 2023-07-21 14:35:10.891723 pelc-0.5.2/README.md
+-rw-r--r--   0        0        0     9864 1970-01-01 00:00:00.000000 pelc-0.5.2/setup.py
+-rw-r--r--   0        0        0     9420 1970-01-01 00:00:00.000000 pelc-0.5.2/PKG-INFO
```

### Comparing `pelc-0.5.1/pelc/_input_sanity_check.py` & `pelc-0.5.2/pelc/_input_sanity_check.py`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/_open_epregistry_databases.py` & `pelc-0.5.2/pelc/_open_epregistry_databases.py`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/_unexpected_alleles.py` & `pelc-0.5.2/pelc/_unexpected_alleles.py`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/batch_eplet_comp.py` & `pelc-0.5.2/pelc/batch_eplet_comp.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,18 @@
     :param simple_comparison: whether or not it's a simple allele to allele comparison in which case, the function
     _equal_amount_of_unknown_alleles is not called (checks are already made in simple_comparison.py and would not
     pass here given the column names).
 
     :return: None (if output_type is not None, the result will be saved on disk as a csv), or pandas.DataFrame
              (OutputType.COUNT_AND_DETAILS) or pandas.Series (OutputType.COUNT, or OutputType.ONLY_DETAILS) or
              tuple[pandas.DataFrame, pandas.DataFrame] (OutputType.FILTERED_TYPINGS)
+
+    :raises ValueError: if the number of unknown alleles is different for one donor and recipient pair or one allele is
+                        unknown whilst the other of the same locus isn't. Obviously doesn't raise anything if user
+                        inputs a homozygous like this: donor: A*01:01 A* and recipient: A*01:01 A*11:01.
     """
     if not class_i and not class_ii:
         logging.error(
             "User did not request class I eplet comparison nor did they request class II eplet comparison."
         )
 
     if exclude is not None:
@@ -68,17 +72,20 @@
 
     if not simple_comparison:
         if not _equal_amount_of_unknown_alleles(input_df_donor, input_df_recipient):
             # unknown alleles are the ones that were inputted as "A*", "B*", "C*", "DRB1*", "DRB345*", "DQA1*", "DQB1*",
             # "DPA1*" and/or "DPB1*". Here we are not talking about the alleles that are unknown to the database.
             logging.error(
                 "Either the number of unknown alleles is different for one donor and recipient pair or one allele is "
-                "uknown whilst the other of the same locus isn't."
+                "unknown whilst the other of the same locus isn't."
+            )
+            raise ValueError(
+                "Either the number of unknown alleles is different for one donor and recipient pair or one allele is "
+                "unknown whilst the other of the same locus isn't."
             )
-            return None
 
 
     df_a: pd.DataFrame
     df_b: pd.DataFrame
     df_c: pd.DataFrame
     df_dr: pd.DataFrame
     df_dq: pd.DataFrame
```

### Comparing `pelc-0.5.1/pelc/batch_eplet_comp_aux.py` & `pelc-0.5.2/pelc/batch_eplet_comp_aux.py`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/A.csv` & `pelc-0.5.2/pelc/data/A.csv`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/A_False_A_.pickle` & `pelc-0.5.2/pelc/data/A_False_A_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/A_True_A_.pickle` & `pelc-0.5.2/pelc/data/A_True_A_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/B.csv` & `pelc-0.5.2/pelc/data/B.csv`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/B_False_B_.pickle` & `pelc-0.5.2/pelc/data/B_False_B_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/B_True_B_.pickle` & `pelc-0.5.2/pelc/data/B_True_B_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/C.csv` & `pelc-0.5.2/pelc/data/C.csv`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/C_False_C_.pickle` & `pelc-0.5.2/pelc/data/C_False_C_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/C_True_C_.pickle` & `pelc-0.5.2/pelc/data/C_True_C_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/DP.csv` & `pelc-0.5.2/pelc/data/DP.csv`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/DP_False_DPB1_.pickle` & `pelc-0.5.2/pelc/data/DP_False_DPB1_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/DP_True_DPB1_.pickle` & `pelc-0.5.2/pelc/data/DP_True_DPB1_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/DQ.csv` & `pelc-0.5.2/pelc/data/DQ.csv`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/DQ_False_DQB1_.pickle` & `pelc-0.5.2/pelc/data/DQ_False_DQB1_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/DQ_True_DQB1_.pickle` & `pelc-0.5.2/pelc/data/DQ_True_DQB1_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/DR.csv` & `pelc-0.5.2/pelc/data/DR.csv`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/DR_False_DRB1_.pickle` & `pelc-0.5.2/pelc/data/DR_False_DRB1_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/DR_True_DRB1_.pickle` & `pelc-0.5.2/pelc/data/DR_True_DRB1_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/ep_data.csv` & `pelc-0.5.2/pelc/data/ep_data.csv`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/data/ep_data.pickle` & `pelc-0.5.2/pelc/data/ep_data.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/pelc/simple_comparison.py` & `pelc-0.5.2/pelc/simple_comparison.py`

 * *Files identical despite different names*

### Comparing `pelc-0.5.1/README.md` & `pelc-0.5.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 if __name__ == "__main__":
     input_path: str = "Template.xlsx"
 
     output_path: str = "MyOutput"
     input_df: pd.DataFrame = pd.read_excel(
         input_path,
         sheet_name="My Sheet",
-        index_col="Index"
+        index_col=0,
     )
 
     donordf: pd.DataFrame
     recipientdf: pd.DataFrame
     donordf, recipientdf = batch_eplet_comp_aux.split_dataframe(input_df)
 
     batch_eplet_comp.compute_epletic_load(
@@ -89,66 +89,71 @@
 
 
 #### Unit tests
 Tested on `Python 3.10.2` & `Python 3.11.1`.
 ```
 platform win32 -- Python 3.10.2, pytest-7.2.0, pluggy-1.0.0
 plugins: anyio-3.6.2, mypy-0.10.3
-collected 34 items
+collected 39 items
 
 unit_tests_mypy.py ..                                                    [  5%]
-unit_tests_simple.py .                                                   [  8%]
-pelc\__init__.py .                                                       [ 11%]
-pelc\_open_epregistry_databases.py .                                     [ 14%]
+unit_tests_simple.py .                                                   [  7%]
+pelc\__init__.py .                                                       [ 10%]
+pelc\_input_sanity_check.py .                                            [ 12%]
+pelc\_open_epregistry_databases.py .                                     [ 15%]
 pelc\_unexpected_alleles.py .                                            [ 17%]
 pelc\batch_eplet_comp.py .                                               [ 20%]
 pelc\batch_eplet_comp_aux.py .                                           [ 23%]
-pelc\output_type.py .                                                    [ 26%]
-pelc\simple_comparison.py .                                              [ 29%]
-tests\__init__.py .                                                      [ 32%]
-tests\base_loading_for_tests.py .                                        [ 35%]
-tests\test_eplet_mismatches.py .......                                   [ 55%]
+pelc\output_type.py .                                                    [ 25%]
+pelc\simple_comparison.py .                                              [ 28%]
+tests\__init__.py .                                                      [ 30%]
+tests\base_loading_for_tests.py .                                        [ 33%]
+tests\test_eplet_mismatches.py .........                                 [ 56%]
 tests\test_extract_key_to_rank_epletes.py ..                             [ 61%]
-tests\test_is_valid_allele.py ..                                         [ 67%]
-tests\test_pelc.py ..                                                    [ 73%]
-tests\test_same_locus.py ..                                              [ 79%]
+tests\test_is_valid_allele.py ..                                         [ 66%]
+tests\test_only_one_chromosome.py ..                                     [ 71%]
+tests\test_pelc.py ..                                                    [ 76%]
+tests\test_same_locus.py ..                                              [ 82%]
 tests\test_simple_comparison.py .....                                    [ 94%]
 tests\test_unexpected_alleles.py ..                                      [100%]
- =================================== mypy =====================================
+==================================== mypy =====================================
 
-Success: no issues found in 18 source files
- ============================= 34 passed in 16.23s ============================
+Success: no issues found in 20 source files
+============================= 39 passed in 32.56s =============================
 ```
+
 ```
 platform win32 -- Python 3.11.1, pytest-7.2.0, pluggy-1.0.0
 plugins: anyio-3.6.2, mypy-0.10.3
-collected 34 items
+collected 39 items
 
 unit_tests_mypy.py ..                                                    [  5%]
-unit_tests_simple.py .                                                   [  8%]
-pelc\__init__.py .                                                       [ 11%]
-pelc\_open_epregistry_databases.py .                                     [ 14%]
+unit_tests_simple.py .                                                   [  7%]
+pelc\__init__.py .                                                       [ 10%]
+pelc\_input_sanity_check.py .                                            [ 12%]
+pelc\_open_epregistry_databases.py .                                     [ 15%]
 pelc\_unexpected_alleles.py .                                            [ 17%]
 pelc\batch_eplet_comp.py .                                               [ 20%]
 pelc\batch_eplet_comp_aux.py .                                           [ 23%]
-pelc\output_type.py .                                                    [ 26%]
-pelc\simple_comparison.py .                                              [ 29%]
-tests\__init__.py .                                                      [ 32%]
-tests\base_loading_for_tests.py .                                        [ 35%]
-tests\test_eplet_mismatches.py .......                                   [ 55%]
+pelc\output_type.py .                                                    [ 25%]
+pelc\simple_comparison.py .                                              [ 28%]
+tests\__init__.py .                                                      [ 30%]
+tests\base_loading_for_tests.py .                                        [ 33%]
+tests\test_eplet_mismatches.py .........                                 [ 56%]
 tests\test_extract_key_to_rank_epletes.py ..                             [ 61%]
-tests\test_is_valid_allele.py ..                                         [ 67%]
-tests\test_pelc.py ..                                                    [ 73%]
-tests\test_same_locus.py ..                                              [ 79%]
+tests\test_is_valid_allele.py ..                                         [ 66%]
+tests\test_only_one_chromosome.py ..                                     [ 71%]
+tests\test_pelc.py ..                                                    [ 76%]
+tests\test_same_locus.py ..                                              [ 82%]
 tests\test_simple_comparison.py .....                                    [ 94%]
 tests\test_unexpected_alleles.py ..                                      [100%]
- =================================== mypy =====================================
+==================================== mypy =====================================
 
-Success: no issues found in 18 source files
- ============================= 34 passed in 14.95s ============================
+Success: no issues found in 20 source files
+============================= 39 passed in 32.56s =============================
 ```
 
 
 
 ### About the source code
 - Follows [PEP8](https://peps.python.org/pep-0008/) Style Guidelines.
 - All functions are unit-tested with [pytest](https://docs.pytest.org/en/stable/).
@@ -168,26 +173,26 @@
 If you use this software, please cite it as below.
 
 - APA:
 ```
 If you use this software, please cite it as below. 
 
 Lhotte, R., Clichet, V., Usureau, C. & Taupin, J. (2022). 
-Python Eplet Load Calculator (PELC) package (Version 0.5.1) [Computer software].
+Python Eplet Load Calculator (PELC) package (Version 0.5.2) [Computer software].
 https://doi.org/10.5281/zenodo.7254809
 ```
 
 - BibTeX:
 ```
 @software{lhotte_romain_2022_7526198,
   author       = {Lhotte, Romain and
                   Clichet, Valentin and
                   Usureau, Cédric and
                   Taupin, Jean-Luc},
   title        = {Python Eplet Load Calculator},
   month        = oct,
   year         = 2022,
   publisher    = {Zenodo},
-  version      = {0.5.1},
+  version      = {0.5.2},
   doi          = {10.5281/zenodo.7526198},
 }
 ```
```

### Comparing `pelc-0.5.1/setup.py` & `pelc-0.5.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 package_data = \
 {'': ['*'], 'pelc': ['data/*']}
 
 install_requires = \
 ['openpyxl>=3.0.10,<4.0.0',
  'pandas-stubs>=2.0.0.230412,<3.0.0.0',
- 'pandas>=1.5.1,<2.0.0']
+ 'pandas>=2.0.3,<3.0.0']
 
 setup_kwargs = {
     'name': 'pelc',
-    'version': '0.5.1',
+    'version': '0.5.2',
     'description': 'Python Eplet Load Calculator',
-    'long_description': '[![DOI](https://zenodo.org/badge/555576588.svg)](https://zenodo.org/badge/latestdoi/555576588)\n[![Downloads](https://pepy.tech/badge/pelc)](https://pepy.tech/project/pelc)\n# PELC (Python Eplet Load Calculator)\n\n### Overview\nPELC is a Python package designed to calculate efficiently the HLA Eplet Load (based on the\n[EpRegistry database](https://www.epregistry.com.br/)) between donors and recipients by loading in a pandas.DataFrame\nin `eplet_comparison.compute_epletic_load` the recipients\' and donors\' typings.  See minimal reproducible example for\nmore details.\n\n\n### Getting started\n#### Install from PyPI (recommended)\nTo use `pelc`, run `pip install pelc` in your terminal.\n\n\n#### Usage\n\n##### a. Comparing two alleles\nHere is a minimal example of how to use `pelc` to compare two alleles:\n```py\nfrom pelc.simple_comparison import simple_comparison\n\nsimple_comparison(\n    "A*68:01",\n    "A*68:02",\n    "output",  # file will be saved as output.csv in the current directory\n    verifiedonly=False,  # if True, only verified eplets will be considered, otherwise all eplets will be considered\n    interlocus2=True  # doesn\'t matter for class I alleles\n)\n```\nIn the `output.csv` file created in the current directory, you will find two rows: "In A&ast;68:02 but not in \nA&ast;68:01" and "In A&ast;68:01 but not in A&ast;68:02".\n\n##### b. Batch mode\nHere is a minimal example with the file [Template.xlsx](https://github.com/MICS-Lab/pelc/raw/main/Template.xlsx)\n(click to download):\n```py\nimport pandas as pd\n\nfrom pelc import batch_eplet_comp, batch_eplet_comp_aux, output_type\n\nif __name__ == "__main__":\n    input_path: str = "Template.xlsx"\n\n    output_path: str = "MyOutput"\n    input_df: pd.DataFrame = pd.read_excel(\n        input_path,\n        sheet_name="My Sheet",\n        index_col="Index"\n    )\n\n    donordf: pd.DataFrame\n    recipientdf: pd.DataFrame\n    donordf, recipientdf = batch_eplet_comp_aux.split_dataframe(input_df)\n\n    batch_eplet_comp.compute_epletic_load(\n        donordf,\n        recipientdf,\n        output_path,\n        output_type.OutputType.DETAILS_AND_COUNT,\n        class_i=True,  # Compute class I eplets comparison?\n        class_ii=True,  # Compute class II eplets comparison?\n        verifiedonly=False,  # How should the epletic charge be computed? Verified eplets only? Or all eplets?\n        exclude=None,  # list of indices to exclude\n        interlocus2=True  # whether or not to take into account interlocus eplets for HLA of class II\n    )\n```\nNote that if a typing is unknown, one can use `A*`, `B*`, ..., `DPB1*` as the allele name for **both** recipients and\ndonors. If the allele is unknown for only of the two individuals, it is necessary to use `A*`, `B*`, ..., `DPB1*` for\nboth individuals otherwise the eplet mismatch computation will not be performed for this donor / recipient pair.\n\n#### Advanced usage:\n##### a. Not taking into account all loci (if they are not typed for example)\nIf one wants to determine the eplet mismatches between a donor and a recipient but without taking into account\na certain locus, one can use `A*`, `B*`, ..., `DPB1*` as the allele name for both recipients and donors on this locus\nand the eplet mismatch computation will only take into account the loci filled in.\n\n##### b. Not creating a file but generating a pandas.DataFrame\nIf one wants to generate a `pandas.DataFrame` directly, the `output_path` argument of `simple_comparison` can be \nset to `None`. The `pandas.DataFrame` will be returned by the function. Same goes for `compute_epletic_load`.\n\n\n#### Exit codes:\n```\n- 55: an eplet did not match the regular expression \'^\\d+\' (ABC, DR, DQ or DP) and it also did not match the regular\nexpression \'^.[pqr]*(\\d+)\' (interlocus2) either.\n```\n\n\n#### Unit tests\nTested on `Python 3.10.2` & `Python 3.11.1`.\n```\nplatform win32 -- Python 3.10.2, pytest-7.2.0, pluggy-1.0.0\nplugins: anyio-3.6.2, mypy-0.10.3\ncollected 34 items\n\nunit_tests_mypy.py ..                                                    [  5%]\nunit_tests_simple.py .                                                   [  8%]\npelc\\__init__.py .                                                       [ 11%]\npelc\\_open_epregistry_databases.py .                                     [ 14%]\npelc\\_unexpected_alleles.py .                                            [ 17%]\npelc\\batch_eplet_comp.py .                                               [ 20%]\npelc\\batch_eplet_comp_aux.py .                                           [ 23%]\npelc\\output_type.py .                                                    [ 26%]\npelc\\simple_comparison.py .                                              [ 29%]\ntests\\__init__.py .                                                      [ 32%]\ntests\\base_loading_for_tests.py .                                        [ 35%]\ntests\\test_eplet_mismatches.py .......                                   [ 55%]\ntests\\test_extract_key_to_rank_epletes.py ..                             [ 61%]\ntests\\test_is_valid_allele.py ..                                         [ 67%]\ntests\\test_pelc.py ..                                                    [ 73%]\ntests\\test_same_locus.py ..                                              [ 79%]\ntests\\test_simple_comparison.py .....                                    [ 94%]\ntests\\test_unexpected_alleles.py ..                                      [100%]\n =================================== mypy =====================================\n\nSuccess: no issues found in 18 source files\n ============================= 34 passed in 16.23s ============================\n```\n```\nplatform win32 -- Python 3.11.1, pytest-7.2.0, pluggy-1.0.0\nplugins: anyio-3.6.2, mypy-0.10.3\ncollected 34 items\n\nunit_tests_mypy.py ..                                                    [  5%]\nunit_tests_simple.py .                                                   [  8%]\npelc\\__init__.py .                                                       [ 11%]\npelc\\_open_epregistry_databases.py .                                     [ 14%]\npelc\\_unexpected_alleles.py .                                            [ 17%]\npelc\\batch_eplet_comp.py .                                               [ 20%]\npelc\\batch_eplet_comp_aux.py .                                           [ 23%]\npelc\\output_type.py .                                                    [ 26%]\npelc\\simple_comparison.py .                                              [ 29%]\ntests\\__init__.py .                                                      [ 32%]\ntests\\base_loading_for_tests.py .                                        [ 35%]\ntests\\test_eplet_mismatches.py .......                                   [ 55%]\ntests\\test_extract_key_to_rank_epletes.py ..                             [ 61%]\ntests\\test_is_valid_allele.py ..                                         [ 67%]\ntests\\test_pelc.py ..                                                    [ 73%]\ntests\\test_same_locus.py ..                                              [ 79%]\ntests\\test_simple_comparison.py .....                                    [ 94%]\ntests\\test_unexpected_alleles.py ..                                      [100%]\n =================================== mypy =====================================\n\nSuccess: no issues found in 18 source files\n ============================= 34 passed in 14.95s ============================\n```\n\n\n\n### About the source code\n- Follows [PEP8](https://peps.python.org/pep-0008/) Style Guidelines.\n- All functions are unit-tested with [pytest](https://docs.pytest.org/en/stable/).\n- All variables are correctly type-hinted, reviewed with [static type checker](https://mypy.readthedocs.io/en/stable/)\n`mypy`.\n- All functions are documented with [docstrings](https://www.python.org/dev/peps/pep-0257/).\n\n\n\n### Useful links:\n- [Corresponding GitHub repository](https://github.com/MICS-Lab/pelc)\n- [Corresponding PyPI page](https://pypi.org/project/pelc)\n\n\n\n### Citation\nIf you use this software, please cite it as below.\n\n- APA:\n```\nIf you use this software, please cite it as below. \n\nLhotte, R., Clichet, V., Usureau, C. & Taupin, J. (2022). \nPython Eplet Load Calculator (PELC) package (Version 0.5.1) [Computer software].\nhttps://doi.org/10.5281/zenodo.7254809\n```\n\n- BibTeX:\n```\n@software{lhotte_romain_2022_7526198,\n  author       = {Lhotte, Romain and\n                  Clichet, Valentin and\n                  Usureau, Cédric and\n                  Taupin, Jean-Luc},\n  title        = {Python Eplet Load Calculator},\n  month        = oct,\n  year         = 2022,\n  publisher    = {Zenodo},\n  version      = {0.5.1},\n  doi          = {10.5281/zenodo.7526198},\n}\n```\n',
+    'long_description': '[![DOI](https://zenodo.org/badge/555576588.svg)](https://zenodo.org/badge/latestdoi/555576588)\n[![Downloads](https://pepy.tech/badge/pelc)](https://pepy.tech/project/pelc)\n# PELC (Python Eplet Load Calculator)\n\n### Overview\nPELC is a Python package designed to calculate efficiently the HLA Eplet Load (based on the\n[EpRegistry database](https://www.epregistry.com.br/)) between donors and recipients by loading in a pandas.DataFrame\nin `eplet_comparison.compute_epletic_load` the recipients\' and donors\' typings.  See minimal reproducible example for\nmore details.\n\n\n### Getting started\n#### Install from PyPI (recommended)\nTo use `pelc`, run `pip install pelc` in your terminal.\n\n\n#### Usage\n\n##### a. Comparing two alleles\nHere is a minimal example of how to use `pelc` to compare two alleles:\n```py\nfrom pelc.simple_comparison import simple_comparison\n\nsimple_comparison(\n    "A*68:01",\n    "A*68:02",\n    "output",  # file will be saved as output.csv in the current directory\n    verifiedonly=False,  # if True, only verified eplets will be considered, otherwise all eplets will be considered\n    interlocus2=True  # doesn\'t matter for class I alleles\n)\n```\nIn the `output.csv` file created in the current directory, you will find two rows: "In A&ast;68:02 but not in \nA&ast;68:01" and "In A&ast;68:01 but not in A&ast;68:02".\n\n##### b. Batch mode\nHere is a minimal example with the file [Template.xlsx](https://github.com/MICS-Lab/pelc/raw/main/Template.xlsx)\n(click to download):\n```py\nimport pandas as pd\n\nfrom pelc import batch_eplet_comp, batch_eplet_comp_aux, output_type\n\nif __name__ == "__main__":\n    input_path: str = "Template.xlsx"\n\n    output_path: str = "MyOutput"\n    input_df: pd.DataFrame = pd.read_excel(\n        input_path,\n        sheet_name="My Sheet",\n        index_col=0,\n    )\n\n    donordf: pd.DataFrame\n    recipientdf: pd.DataFrame\n    donordf, recipientdf = batch_eplet_comp_aux.split_dataframe(input_df)\n\n    batch_eplet_comp.compute_epletic_load(\n        donordf,\n        recipientdf,\n        output_path,\n        output_type.OutputType.DETAILS_AND_COUNT,\n        class_i=True,  # Compute class I eplets comparison?\n        class_ii=True,  # Compute class II eplets comparison?\n        verifiedonly=False,  # How should the epletic charge be computed? Verified eplets only? Or all eplets?\n        exclude=None,  # list of indices to exclude\n        interlocus2=True  # whether or not to take into account interlocus eplets for HLA of class II\n    )\n```\nNote that if a typing is unknown, one can use `A*`, `B*`, ..., `DPB1*` as the allele name for **both** recipients and\ndonors. If the allele is unknown for only of the two individuals, it is necessary to use `A*`, `B*`, ..., `DPB1*` for\nboth individuals otherwise the eplet mismatch computation will not be performed for this donor / recipient pair.\n\n#### Advanced usage:\n##### a. Not taking into account all loci (if they are not typed for example)\nIf one wants to determine the eplet mismatches between a donor and a recipient but without taking into account\na certain locus, one can use `A*`, `B*`, ..., `DPB1*` as the allele name for both recipients and donors on this locus\nand the eplet mismatch computation will only take into account the loci filled in.\n\n##### b. Not creating a file but generating a pandas.DataFrame\nIf one wants to generate a `pandas.DataFrame` directly, the `output_path` argument of `simple_comparison` can be \nset to `None`. The `pandas.DataFrame` will be returned by the function. Same goes for `compute_epletic_load`.\n\n\n#### Exit codes:\n```\n- 55: an eplet did not match the regular expression \'^\\d+\' (ABC, DR, DQ or DP) and it also did not match the regular\nexpression \'^.[pqr]*(\\d+)\' (interlocus2) either.\n```\n\n\n#### Unit tests\nTested on `Python 3.10.2` & `Python 3.11.1`.\n```\nplatform win32 -- Python 3.10.2, pytest-7.2.0, pluggy-1.0.0\nplugins: anyio-3.6.2, mypy-0.10.3\ncollected 39 items\n\nunit_tests_mypy.py ..                                                    [  5%]\nunit_tests_simple.py .                                                   [  7%]\npelc\\__init__.py .                                                       [ 10%]\npelc\\_input_sanity_check.py .                                            [ 12%]\npelc\\_open_epregistry_databases.py .                                     [ 15%]\npelc\\_unexpected_alleles.py .                                            [ 17%]\npelc\\batch_eplet_comp.py .                                               [ 20%]\npelc\\batch_eplet_comp_aux.py .                                           [ 23%]\npelc\\output_type.py .                                                    [ 25%]\npelc\\simple_comparison.py .                                              [ 28%]\ntests\\__init__.py .                                                      [ 30%]\ntests\\base_loading_for_tests.py .                                        [ 33%]\ntests\\test_eplet_mismatches.py .........                                 [ 56%]\ntests\\test_extract_key_to_rank_epletes.py ..                             [ 61%]\ntests\\test_is_valid_allele.py ..                                         [ 66%]\ntests\\test_only_one_chromosome.py ..                                     [ 71%]\ntests\\test_pelc.py ..                                                    [ 76%]\ntests\\test_same_locus.py ..                                              [ 82%]\ntests\\test_simple_comparison.py .....                                    [ 94%]\ntests\\test_unexpected_alleles.py ..                                      [100%]\n==================================== mypy =====================================\n\nSuccess: no issues found in 20 source files\n============================= 39 passed in 32.56s =============================\n```\n\n```\nplatform win32 -- Python 3.11.1, pytest-7.2.0, pluggy-1.0.0\nplugins: anyio-3.6.2, mypy-0.10.3\ncollected 39 items\n\nunit_tests_mypy.py ..                                                    [  5%]\nunit_tests_simple.py .                                                   [  7%]\npelc\\__init__.py .                                                       [ 10%]\npelc\\_input_sanity_check.py .                                            [ 12%]\npelc\\_open_epregistry_databases.py .                                     [ 15%]\npelc\\_unexpected_alleles.py .                                            [ 17%]\npelc\\batch_eplet_comp.py .                                               [ 20%]\npelc\\batch_eplet_comp_aux.py .                                           [ 23%]\npelc\\output_type.py .                                                    [ 25%]\npelc\\simple_comparison.py .                                              [ 28%]\ntests\\__init__.py .                                                      [ 30%]\ntests\\base_loading_for_tests.py .                                        [ 33%]\ntests\\test_eplet_mismatches.py .........                                 [ 56%]\ntests\\test_extract_key_to_rank_epletes.py ..                             [ 61%]\ntests\\test_is_valid_allele.py ..                                         [ 66%]\ntests\\test_only_one_chromosome.py ..                                     [ 71%]\ntests\\test_pelc.py ..                                                    [ 76%]\ntests\\test_same_locus.py ..                                              [ 82%]\ntests\\test_simple_comparison.py .....                                    [ 94%]\ntests\\test_unexpected_alleles.py ..                                      [100%]\n==================================== mypy =====================================\n\nSuccess: no issues found in 20 source files\n============================= 39 passed in 32.56s =============================\n```\n\n\n\n### About the source code\n- Follows [PEP8](https://peps.python.org/pep-0008/) Style Guidelines.\n- All functions are unit-tested with [pytest](https://docs.pytest.org/en/stable/).\n- All variables are correctly type-hinted, reviewed with [static type checker](https://mypy.readthedocs.io/en/stable/)\n`mypy`.\n- All functions are documented with [docstrings](https://www.python.org/dev/peps/pep-0257/).\n\n\n\n### Useful links:\n- [Corresponding GitHub repository](https://github.com/MICS-Lab/pelc)\n- [Corresponding PyPI page](https://pypi.org/project/pelc)\n\n\n\n### Citation\nIf you use this software, please cite it as below.\n\n- APA:\n```\nIf you use this software, please cite it as below. \n\nLhotte, R., Clichet, V., Usureau, C. & Taupin, J. (2022). \nPython Eplet Load Calculator (PELC) package (Version 0.5.2) [Computer software].\nhttps://doi.org/10.5281/zenodo.7254809\n```\n\n- BibTeX:\n```\n@software{lhotte_romain_2022_7526198,\n  author       = {Lhotte, Romain and\n                  Clichet, Valentin and\n                  Usureau, Cédric and\n                  Taupin, Jean-Luc},\n  title        = {Python Eplet Load Calculator},\n  month        = oct,\n  year         = 2022,\n  publisher    = {Zenodo},\n  version      = {0.5.2},\n  doi          = {10.5281/zenodo.7526198},\n}\n```\n',
     'author': 'JasonMendoza2008',
     'author_email': 'lhotteromain@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pelc-0.5.1/PKG-INFO` & `pelc-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pelc
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python Eplet Load Calculator
 Author: JasonMendoza2008
 Author-email: lhotteromain@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
-Requires-Dist: pandas (>=1.5.1,<2.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pandas-stubs (>=2.0.0.230412,<3.0.0.0)
 Description-Content-Type: text/markdown
 
 [![DOI](https://zenodo.org/badge/555576588.svg)](https://zenodo.org/badge/latestdoi/555576588)
 [![Downloads](https://pepy.tech/badge/pelc)](https://pepy.tech/project/pelc)
 # PELC (Python Eplet Load Calculator)
 
@@ -58,15 +58,15 @@
 if __name__ == "__main__":
     input_path: str = "Template.xlsx"
 
     output_path: str = "MyOutput"
     input_df: pd.DataFrame = pd.read_excel(
         input_path,
         sheet_name="My Sheet",
-        index_col="Index"
+        index_col=0,
     )
 
     donordf: pd.DataFrame
     recipientdf: pd.DataFrame
     donordf, recipientdf = batch_eplet_comp_aux.split_dataframe(input_df)
 
     batch_eplet_comp.compute_epletic_load(
@@ -104,66 +104,71 @@
 
 
 #### Unit tests
 Tested on `Python 3.10.2` & `Python 3.11.1`.
 ```
 platform win32 -- Python 3.10.2, pytest-7.2.0, pluggy-1.0.0
 plugins: anyio-3.6.2, mypy-0.10.3
-collected 34 items
+collected 39 items
 
 unit_tests_mypy.py ..                                                    [  5%]
-unit_tests_simple.py .                                                   [  8%]
-pelc\__init__.py .                                                       [ 11%]
-pelc\_open_epregistry_databases.py .                                     [ 14%]
+unit_tests_simple.py .                                                   [  7%]
+pelc\__init__.py .                                                       [ 10%]
+pelc\_input_sanity_check.py .                                            [ 12%]
+pelc\_open_epregistry_databases.py .                                     [ 15%]
 pelc\_unexpected_alleles.py .                                            [ 17%]
 pelc\batch_eplet_comp.py .                                               [ 20%]
 pelc\batch_eplet_comp_aux.py .                                           [ 23%]
-pelc\output_type.py .                                                    [ 26%]
-pelc\simple_comparison.py .                                              [ 29%]
-tests\__init__.py .                                                      [ 32%]
-tests\base_loading_for_tests.py .                                        [ 35%]
-tests\test_eplet_mismatches.py .......                                   [ 55%]
+pelc\output_type.py .                                                    [ 25%]
+pelc\simple_comparison.py .                                              [ 28%]
+tests\__init__.py .                                                      [ 30%]
+tests\base_loading_for_tests.py .                                        [ 33%]
+tests\test_eplet_mismatches.py .........                                 [ 56%]
 tests\test_extract_key_to_rank_epletes.py ..                             [ 61%]
-tests\test_is_valid_allele.py ..                                         [ 67%]
-tests\test_pelc.py ..                                                    [ 73%]
-tests\test_same_locus.py ..                                              [ 79%]
+tests\test_is_valid_allele.py ..                                         [ 66%]
+tests\test_only_one_chromosome.py ..                                     [ 71%]
+tests\test_pelc.py ..                                                    [ 76%]
+tests\test_same_locus.py ..                                              [ 82%]
 tests\test_simple_comparison.py .....                                    [ 94%]
 tests\test_unexpected_alleles.py ..                                      [100%]
- =================================== mypy =====================================
+==================================== mypy =====================================
 
-Success: no issues found in 18 source files
- ============================= 34 passed in 16.23s ============================
+Success: no issues found in 20 source files
+============================= 39 passed in 32.56s =============================
 ```
+
 ```
 platform win32 -- Python 3.11.1, pytest-7.2.0, pluggy-1.0.0
 plugins: anyio-3.6.2, mypy-0.10.3
-collected 34 items
+collected 39 items
 
 unit_tests_mypy.py ..                                                    [  5%]
-unit_tests_simple.py .                                                   [  8%]
-pelc\__init__.py .                                                       [ 11%]
-pelc\_open_epregistry_databases.py .                                     [ 14%]
+unit_tests_simple.py .                                                   [  7%]
+pelc\__init__.py .                                                       [ 10%]
+pelc\_input_sanity_check.py .                                            [ 12%]
+pelc\_open_epregistry_databases.py .                                     [ 15%]
 pelc\_unexpected_alleles.py .                                            [ 17%]
 pelc\batch_eplet_comp.py .                                               [ 20%]
 pelc\batch_eplet_comp_aux.py .                                           [ 23%]
-pelc\output_type.py .                                                    [ 26%]
-pelc\simple_comparison.py .                                              [ 29%]
-tests\__init__.py .                                                      [ 32%]
-tests\base_loading_for_tests.py .                                        [ 35%]
-tests\test_eplet_mismatches.py .......                                   [ 55%]
+pelc\output_type.py .                                                    [ 25%]
+pelc\simple_comparison.py .                                              [ 28%]
+tests\__init__.py .                                                      [ 30%]
+tests\base_loading_for_tests.py .                                        [ 33%]
+tests\test_eplet_mismatches.py .........                                 [ 56%]
 tests\test_extract_key_to_rank_epletes.py ..                             [ 61%]
-tests\test_is_valid_allele.py ..                                         [ 67%]
-tests\test_pelc.py ..                                                    [ 73%]
-tests\test_same_locus.py ..                                              [ 79%]
+tests\test_is_valid_allele.py ..                                         [ 66%]
+tests\test_only_one_chromosome.py ..                                     [ 71%]
+tests\test_pelc.py ..                                                    [ 76%]
+tests\test_same_locus.py ..                                              [ 82%]
 tests\test_simple_comparison.py .....                                    [ 94%]
 tests\test_unexpected_alleles.py ..                                      [100%]
- =================================== mypy =====================================
+==================================== mypy =====================================
 
-Success: no issues found in 18 source files
- ============================= 34 passed in 14.95s ============================
+Success: no issues found in 20 source files
+============================= 39 passed in 32.56s =============================
 ```
 
 
 
 ### About the source code
 - Follows [PEP8](https://peps.python.org/pep-0008/) Style Guidelines.
 - All functions are unit-tested with [pytest](https://docs.pytest.org/en/stable/).
@@ -183,27 +188,27 @@
 If you use this software, please cite it as below.
 
 - APA:
 ```
 If you use this software, please cite it as below. 
 
 Lhotte, R., Clichet, V., Usureau, C. & Taupin, J. (2022). 
-Python Eplet Load Calculator (PELC) package (Version 0.5.1) [Computer software].
+Python Eplet Load Calculator (PELC) package (Version 0.5.2) [Computer software].
 https://doi.org/10.5281/zenodo.7254809
 ```
 
 - BibTeX:
 ```
 @software{lhotte_romain_2022_7526198,
   author       = {Lhotte, Romain and
                   Clichet, Valentin and
                   Usureau, Cédric and
                   Taupin, Jean-Luc},
   title        = {Python Eplet Load Calculator},
   month        = oct,
   year         = 2022,
   publisher    = {Zenodo},
-  version      = {0.5.1},
+  version      = {0.5.2},
   doi          = {10.5281/zenodo.7526198},
 }
 ```
```

