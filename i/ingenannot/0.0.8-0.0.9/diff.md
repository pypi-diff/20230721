# Comparing `tmp/ingenannot-0.0.8.tar.gz` & `tmp/ingenannot-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ingenannot-0.0.8.tar", last modified: Tue Jul 18 07:38:58 2023, max compression
+gzip compressed data, was "ingenannot-0.0.9.tar", last modified: Fri Jul 21 09:56:56 2023, max compression
```

## Comparing `ingenannot-0.0.8.tar` & `ingenannot-0.0.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-07-18 07:38:58.572254 ingenannot-0.0.8/
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     7652 2022-11-02 13:47:42.000000 ingenannot-0.0.8/LICENSE
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     9860 2023-07-18 07:38:58.572254 ingenannot-0.0.8/PKG-INFO
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     9287 2023-07-18 07:37:47.000000 ingenannot-0.0.8/README.md
-drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-07-18 07:38:58.572254 ingenannot-0.0.8/ingenannot/
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)        0 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/__init__.py
-drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-07-18 07:38:58.572254 ingenannot-0.0.8/ingenannot/commands/
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     1465 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/commands/__init__.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     5847 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/commands/add_sqanti3_isoforms.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     5621 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/commands/aed.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     3432 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/commands/aed_compare.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2396 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/commands/clusterize.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       78 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/commands/command.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    14938 2022-11-09 07:30:49.000000 ingenannot-0.0.8/ingenannot/commands/compare.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     7949 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/commands/curation.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)      838 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/commands/effector_predictor_cmd.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4236 2022-11-09 07:30:49.000000 ingenannot-0.0.8/ingenannot/commands/exonerate_to_gff.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4746 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/commands/filter.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    30896 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/commands/isoform_ranking.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     7161 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/commands/rename.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    15953 2022-11-09 07:30:49.000000 ingenannot-0.0.8/ingenannot/commands/rescue_effectors.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    18638 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/commands/select.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     3263 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/commands/so_classification.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4193 2022-11-09 07:30:49.000000 ingenannot-0.0.8/ingenannot/commands/strand_annotation_filter.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    11578 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/commands/utr_refine.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4581 2022-12-14 14:37:30.000000 ingenannot-0.0.8/ingenannot/commands/validate.py
-drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-07-18 07:38:58.572254 ingenannot-0.0.8/ingenannot/entities/
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)        0 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/entities/__init__.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     1823 2022-11-09 07:30:49.000000 ingenannot-0.0.8/ingenannot/entities/cds.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     3672 2022-11-09 07:30:49.000000 ingenannot-0.0.8/ingenannot/entities/cluster.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2520 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/entities/exon.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4464 2023-02-20 14:31:58.000000 ingenannot-0.0.8/ingenannot/entities/gene.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)      290 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/entities/intron.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     5929 2022-11-09 07:30:49.000000 ingenannot-0.0.8/ingenannot/entities/metagene.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    18396 2023-02-20 14:31:58.000000 ingenannot-0.0.8/ingenannot/entities/transcript.py
--rwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)    39864 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/main.py
-drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-07-18 07:38:58.572254 ingenannot-0.0.8/ingenannot/utils/
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    27171 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/utils/__init__.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     8947 2023-02-20 14:31:58.000000 ingenannot-0.0.8/ingenannot/utils/annot_edit_distance.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    11180 2022-11-09 07:30:49.000000 ingenannot-0.0.8/ingenannot/utils/effector_predictor.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2111 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/utils/em_operators.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    15370 2023-02-20 14:31:58.000000 ingenannot-0.0.8/ingenannot/utils/gene_builder.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    11417 2022-12-14 10:01:33.000000 ingenannot-0.0.8/ingenannot/utils/gff_reader.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    13268 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/utils/graphics.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2835 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/utils/so_splicing_classifier.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2743 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/utils/statistics.py
--rwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)     8495 2023-02-02 08:36:33.000000 ingenannot-0.0.8/ingenannot/utils/stats.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     1673 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/utils/tool_checker.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       48 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/version.py
-drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-07-18 07:38:58.572254 ingenannot-0.0.8/ingenannot.egg-info/
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     9860 2023-07-18 07:38:58.000000 ingenannot-0.0.8/ingenannot.egg-info/PKG-INFO
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     1581 2023-07-18 07:38:58.000000 ingenannot-0.0.8/ingenannot.egg-info/SOURCES.txt
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)        1 2023-07-18 07:38:58.000000 ingenannot-0.0.8/ingenannot.egg-info/dependency_links.txt
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       52 2023-07-18 07:38:58.000000 ingenannot-0.0.8/ingenannot.egg-info/entry_points.txt
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       59 2023-07-18 07:38:58.000000 ingenannot-0.0.8/ingenannot.egg-info/requires.txt
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       11 2023-07-18 07:38:58.000000 ingenannot-0.0.8/ingenannot.egg-info/top_level.txt
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       38 2023-07-18 07:38:58.572254 ingenannot-0.0.8/setup.cfg
--rwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)     1831 2023-02-16 15:51:39.000000 ingenannot-0.0.8/setup.py
+drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-07-21 09:56:56.185260 ingenannot-0.0.9/
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     7652 2022-11-02 13:47:42.000000 ingenannot-0.0.9/LICENSE
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     9860 2023-07-21 09:56:56.185260 ingenannot-0.0.9/PKG-INFO
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     9287 2023-07-18 07:37:47.000000 ingenannot-0.0.9/README.md
+drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-07-21 09:56:56.175260 ingenannot-0.0.9/ingenannot/
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)        0 2022-11-02 13:47:42.000000 ingenannot-0.0.9/ingenannot/__init__.py
+drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-07-21 09:56:56.185260 ingenannot-0.0.9/ingenannot/commands/
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     1465 2023-07-18 07:37:47.000000 ingenannot-0.0.9/ingenannot/commands/__init__.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     5847 2022-11-02 13:47:42.000000 ingenannot-0.0.9/ingenannot/commands/add_sqanti3_isoforms.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     5621 2023-07-18 07:37:47.000000 ingenannot-0.0.9/ingenannot/commands/aed.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     3437 2023-07-21 09:53:26.000000 ingenannot-0.0.9/ingenannot/commands/aed_compare.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2396 2022-11-02 13:47:42.000000 ingenannot-0.0.9/ingenannot/commands/clusterize.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       78 2022-11-02 13:47:42.000000 ingenannot-0.0.9/ingenannot/commands/command.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    14938 2022-11-09 07:30:49.000000 ingenannot-0.0.9/ingenannot/commands/compare.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     7949 2023-07-18 07:37:47.000000 ingenannot-0.0.9/ingenannot/commands/curation.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)      838 2022-11-02 13:47:42.000000 ingenannot-0.0.9/ingenannot/commands/effector_predictor_cmd.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4236 2022-11-09 07:30:49.000000 ingenannot-0.0.9/ingenannot/commands/exonerate_to_gff.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4746 2022-11-02 13:47:42.000000 ingenannot-0.0.9/ingenannot/commands/filter.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    30896 2023-07-18 07:37:47.000000 ingenannot-0.0.9/ingenannot/commands/isoform_ranking.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     7161 2023-07-18 07:37:47.000000 ingenannot-0.0.9/ingenannot/commands/rename.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    15953 2022-11-09 07:30:49.000000 ingenannot-0.0.9/ingenannot/commands/rescue_effectors.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    18638 2023-07-18 07:37:47.000000 ingenannot-0.0.9/ingenannot/commands/select.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     3263 2022-11-02 13:47:42.000000 ingenannot-0.0.9/ingenannot/commands/so_classification.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4193 2022-11-09 07:30:49.000000 ingenannot-0.0.9/ingenannot/commands/strand_annotation_filter.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    11578 2023-07-18 07:37:47.000000 ingenannot-0.0.9/ingenannot/commands/utr_refine.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4581 2022-12-14 14:37:30.000000 ingenannot-0.0.9/ingenannot/commands/validate.py
+drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-07-21 09:56:56.185260 ingenannot-0.0.9/ingenannot/entities/
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)        0 2022-11-02 13:47:42.000000 ingenannot-0.0.9/ingenannot/entities/__init__.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     1823 2022-11-09 07:30:49.000000 ingenannot-0.0.9/ingenannot/entities/cds.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     3672 2022-11-09 07:30:49.000000 ingenannot-0.0.9/ingenannot/entities/cluster.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2520 2022-11-02 13:47:42.000000 ingenannot-0.0.9/ingenannot/entities/exon.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4464 2023-02-20 14:31:58.000000 ingenannot-0.0.9/ingenannot/entities/gene.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)      290 2022-11-02 13:47:42.000000 ingenannot-0.0.9/ingenannot/entities/intron.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     5929 2022-11-09 07:30:49.000000 ingenannot-0.0.9/ingenannot/entities/metagene.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    18396 2023-02-20 14:31:58.000000 ingenannot-0.0.9/ingenannot/entities/transcript.py
+-rwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)    39864 2023-07-18 07:37:47.000000 ingenannot-0.0.9/ingenannot/main.py
+drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-07-21 09:56:56.185260 ingenannot-0.0.9/ingenannot/utils/
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    27171 2023-07-18 07:37:47.000000 ingenannot-0.0.9/ingenannot/utils/__init__.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     8947 2023-02-20 14:31:58.000000 ingenannot-0.0.9/ingenannot/utils/annot_edit_distance.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    11180 2022-11-09 07:30:49.000000 ingenannot-0.0.9/ingenannot/utils/effector_predictor.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2111 2022-11-02 13:47:42.000000 ingenannot-0.0.9/ingenannot/utils/em_operators.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    15370 2023-02-20 14:31:58.000000 ingenannot-0.0.9/ingenannot/utils/gene_builder.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    11417 2022-12-14 10:01:33.000000 ingenannot-0.0.9/ingenannot/utils/gff_reader.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    13268 2023-07-18 07:37:47.000000 ingenannot-0.0.9/ingenannot/utils/graphics.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2835 2022-11-02 13:47:42.000000 ingenannot-0.0.9/ingenannot/utils/so_splicing_classifier.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2743 2023-07-18 07:37:47.000000 ingenannot-0.0.9/ingenannot/utils/statistics.py
+-rwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)     8495 2023-02-02 08:36:33.000000 ingenannot-0.0.9/ingenannot/utils/stats.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     1673 2022-11-02 13:47:42.000000 ingenannot-0.0.9/ingenannot/utils/tool_checker.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       48 2023-07-21 09:56:23.000000 ingenannot-0.0.9/ingenannot/version.py
+drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-07-21 09:56:56.185260 ingenannot-0.0.9/ingenannot.egg-info/
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     9860 2023-07-21 09:56:56.000000 ingenannot-0.0.9/ingenannot.egg-info/PKG-INFO
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     1581 2023-07-21 09:56:56.000000 ingenannot-0.0.9/ingenannot.egg-info/SOURCES.txt
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)        1 2023-07-21 09:56:56.000000 ingenannot-0.0.9/ingenannot.egg-info/dependency_links.txt
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       52 2023-07-21 09:56:56.000000 ingenannot-0.0.9/ingenannot.egg-info/entry_points.txt
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       59 2023-07-21 09:56:56.000000 ingenannot-0.0.9/ingenannot.egg-info/requires.txt
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       11 2023-07-21 09:56:56.000000 ingenannot-0.0.9/ingenannot.egg-info/top_level.txt
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       38 2023-07-21 09:56:56.185260 ingenannot-0.0.9/setup.cfg
+-rwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)     1831 2023-02-16 15:51:39.000000 ingenannot-0.0.9/setup.py
```

### Comparing `ingenannot-0.0.8/LICENSE` & `ingenannot-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/PKG-INFO` & `ingenannot-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingenannot
-Version: 0.0.8
+Version: 0.0.9
 Summary: InGenAnnot: Inspection of Gene Annotation
 Home-page: https://forgemia.inra.fr/bioger/ingenannot
 Author: Nicolas Lapalu
 Author-email: nicolas.lapalu@inrae.fr
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
```

### Comparing `ingenannot-0.0.8/README.md` & `ingenannot-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/commands/__init__.py` & `ingenannot-0.0.9/ingenannot/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/commands/add_sqanti3_isoforms.py` & `ingenannot-0.0.9/ingenannot/commands/add_sqanti3_isoforms.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/commands/aed.py` & `ingenannot-0.0.9/ingenannot/commands/aed.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/commands/aed_compare.py` & `ingenannot-0.0.9/ingenannot/commands/aed_compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         genes = Utils.extract_genes_from_fof(self.fof)
         Utils.get_aed_from_attributes(genes)
         Graphics.plot_cumulative_aed(sources, genes, "tr","cumulative_tr_AED.png",self.ncol)
         Graphics.plot_cumulative_aed(sources, genes, "pr","cumulative_pr_AED.png",self.ncol)
         Graphics.plot_cumulative_aed(sources, genes, "best","cumulative_best_AED.png",self.ncol)
 
         if self.statistics:
-            print(self.perform_stats(sources, genes).to_string())
+            print(self.perform_stats(sources, genes).to_csv(sep="\t"))
 
         return 0
 
     def perform_stats(self, sources, genes):
         """run statistics"""
 
         logging.info("Running statistics")
```

### Comparing `ingenannot-0.0.8/ingenannot/commands/clusterize.py` & `ingenannot-0.0.9/ingenannot/commands/clusterize.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/commands/compare.py` & `ingenannot-0.0.9/ingenannot/commands/compare.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/commands/curation.py` & `ingenannot-0.0.9/ingenannot/commands/curation.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/commands/effector_predictor_cmd.py` & `ingenannot-0.0.9/ingenannot/commands/effector_predictor_cmd.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/commands/exonerate_to_gff.py` & `ingenannot-0.0.9/ingenannot/commands/exonerate_to_gff.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/commands/filter.py` & `ingenannot-0.0.9/ingenannot/commands/filter.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/commands/isoform_ranking.py` & `ingenannot-0.0.9/ingenannot/commands/isoform_ranking.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/commands/rename.py` & `ingenannot-0.0.9/ingenannot/commands/rename.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/commands/rescue_effectors.py` & `ingenannot-0.0.9/ingenannot/commands/rescue_effectors.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/commands/select.py` & `ingenannot-0.0.9/ingenannot/commands/select.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/commands/so_classification.py` & `ingenannot-0.0.9/ingenannot/commands/so_classification.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/commands/strand_annotation_filter.py` & `ingenannot-0.0.9/ingenannot/commands/strand_annotation_filter.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/commands/utr_refine.py` & `ingenannot-0.0.9/ingenannot/commands/utr_refine.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/commands/validate.py` & `ingenannot-0.0.9/ingenannot/commands/validate.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/entities/cds.py` & `ingenannot-0.0.9/ingenannot/entities/cds.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/entities/cluster.py` & `ingenannot-0.0.9/ingenannot/entities/cluster.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/entities/exon.py` & `ingenannot-0.0.9/ingenannot/entities/exon.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/entities/gene.py` & `ingenannot-0.0.9/ingenannot/entities/gene.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/entities/metagene.py` & `ingenannot-0.0.9/ingenannot/entities/metagene.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/entities/transcript.py` & `ingenannot-0.0.9/ingenannot/entities/transcript.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/main.py` & `ingenannot-0.0.9/ingenannot/main.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/utils/__init__.py` & `ingenannot-0.0.9/ingenannot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/utils/annot_edit_distance.py` & `ingenannot-0.0.9/ingenannot/utils/annot_edit_distance.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/utils/effector_predictor.py` & `ingenannot-0.0.9/ingenannot/utils/effector_predictor.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/utils/em_operators.py` & `ingenannot-0.0.9/ingenannot/utils/em_operators.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/utils/gene_builder.py` & `ingenannot-0.0.9/ingenannot/utils/gene_builder.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/utils/gff_reader.py` & `ingenannot-0.0.9/ingenannot/utils/gff_reader.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/utils/graphics.py` & `ingenannot-0.0.9/ingenannot/utils/graphics.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/utils/so_splicing_classifier.py` & `ingenannot-0.0.9/ingenannot/utils/so_splicing_classifier.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/utils/statistics.py` & `ingenannot-0.0.9/ingenannot/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/utils/stats.py` & `ingenannot-0.0.9/ingenannot/utils/stats.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot/utils/tool_checker.py` & `ingenannot-0.0.9/ingenannot/utils/tool_checker.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/ingenannot.egg-info/PKG-INFO` & `ingenannot-0.0.9/ingenannot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingenannot
-Version: 0.0.8
+Version: 0.0.9
 Summary: InGenAnnot: Inspection of Gene Annotation
 Home-page: https://forgemia.inra.fr/bioger/ingenannot
 Author: Nicolas Lapalu
 Author-email: nicolas.lapalu@inrae.fr
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
```

### Comparing `ingenannot-0.0.8/ingenannot.egg-info/SOURCES.txt` & `ingenannot-0.0.9/ingenannot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.8/setup.py` & `ingenannot-0.0.9/setup.py`

 * *Files identical despite different names*

