# Comparing `tmp/nanoCEM-0.0.2.3.tar.gz` & `tmp/nanoCEM-0.0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nanoCEM-0.0.2.3.tar", last modified: Thu Jul 20 08:06:12 2023, max compression
+gzip compressed data, was "dist/nanoCEM-0.0.2.4.tar", last modified: Fri Jul 21 02:53:22 2023, max compression
```

## Comparing `nanoCEM-0.0.2.3.tar` & `nanoCEM-0.0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-20 08:06:12.052271 nanoCEM-0.0.2.3/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.2.3/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10204 2023-07-20 08:06:12.048271 nanoCEM-0.0.2.3/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9621 2023-07-20 08:05:38.000000 nanoCEM-0.0.2.3/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-20 08:06:12.048271 nanoCEM-0.0.2.3/nanoCEM/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10038 2023-07-20 07:04:18.000000 nanoCEM-0.0.2.3/nanoCEM/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.2.3/nanoCEM/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-07-14 02:30:08.000000 nanoCEM-0.0.2.3/nanoCEM/cem_utils.py
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     8275 2023-07-20 06:58:56.000000 nanoCEM-0.0.2.3/nanoCEM/current_events_magnifier
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.2.3/nanoCEM/extract_sub_fast5_from_bam
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1846 2023-07-14 09:41:28.000000 nanoCEM-0.0.2.3/nanoCEM/extract_sub_fastq_from_bam
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.2.3/nanoCEM/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7847 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.3/nanoCEM/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11524 2023-07-15 03:17:36.000000 nanoCEM-0.0.2.3/nanoCEM/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13880 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.3/nanoCEM/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-20 08:06:12.048271 nanoCEM-0.0.2.3/nanoCEM.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10204 2023-07-20 08:06:12.000000 nanoCEM-0.0.2.3/nanoCEM.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      458 2023-07-20 08:06:12.000000 nanoCEM-0.0.2.3/nanoCEM.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-20 08:06:12.000000 nanoCEM-0.0.2.3/nanoCEM.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      137 2023-07-20 08:06:12.000000 nanoCEM-0.0.2.3/nanoCEM.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-20 08:06:12.000000 nanoCEM-0.0.2.3/nanoCEM.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-20 08:06:12.052271 nanoCEM-0.0.2.3/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1192 2023-07-20 08:05:38.000000 nanoCEM-0.0.2.3/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-21 02:53:22.262616 nanoCEM-0.0.2.4/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.2.4/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10208 2023-07-21 02:53:22.262616 nanoCEM-0.0.2.4/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9625 2023-07-20 11:04:47.000000 nanoCEM-0.0.2.4/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-21 02:53:22.262616 nanoCEM-0.0.2.4/nanoCEM/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10148 2023-07-21 02:50:56.000000 nanoCEM-0.0.2.4/nanoCEM/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.2.4/nanoCEM/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-07-14 02:30:08.000000 nanoCEM-0.0.2.4/nanoCEM/cem_utils.py
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     8385 2023-07-21 02:50:56.000000 nanoCEM-0.0.2.4/nanoCEM/current_events_magnifier
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.2.4/nanoCEM/extract_sub_fast5_from_bam
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1846 2023-07-14 09:41:28.000000 nanoCEM-0.0.2.4/nanoCEM/extract_sub_fastq_from_bam
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.2.4/nanoCEM/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7847 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.4/nanoCEM/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11524 2023-07-15 03:17:36.000000 nanoCEM-0.0.2.4/nanoCEM/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13880 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.4/nanoCEM/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-21 02:53:22.262616 nanoCEM-0.0.2.4/nanoCEM.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10208 2023-07-21 02:53:22.000000 nanoCEM-0.0.2.4/nanoCEM.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      458 2023-07-21 02:53:22.000000 nanoCEM-0.0.2.4/nanoCEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-21 02:53:22.000000 nanoCEM-0.0.2.4/nanoCEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      137 2023-07-21 02:53:22.000000 nanoCEM-0.0.2.4/nanoCEM.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-21 02:53:22.000000 nanoCEM-0.0.2.4/nanoCEM.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-21 02:53:22.262616 nanoCEM-0.0.2.4/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1192 2023-07-21 02:53:01.000000 nanoCEM-0.0.2.4/setup.py
```

### Comparing `nanoCEM-0.0.2.3/LICENSE` & `nanoCEM-0.0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.3/PKG-INFO` & `nanoCEM-0.0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.2.3
+Version: 0.0.2.4
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle program(tombo and f5c).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nanoCEM
 The nanopore current events magnifier (`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
-CEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
+NanoCEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
 
 It supports two re-squiggle pipeline(`Tombo` and `f5c`) and support `R9` and `R10`.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
 ## Example
 Here is an example to help the user confirm the installation of A2030 on 23S rRNA:
 ```sh
@@ -155,15 +155,15 @@
 multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
 extract_sub_fast5_from_bam -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
 # Remember to sample fastq if you sampled your fast5
 extract_sub_fastq_from_bam -i all.fastq -o final.fastq -b file.bam --chrom NR_103073.1 --pos 2030 
 ```
 ### 4 Re-squiggle
 #### 4.1 Tombo resquiggle (v1.5.0)
-Step 1 and 2 should run on your two sample respectively, before the step 5.
+Step 1 and 2 should run on your two sample respectively, before the step 3.
 1. Data format conversion
 
 If you did the subsample,skip this step and used ```subsample_single``` as the following input rather than ```single/```
 ```sh
 # assumed your fast5 file folder name is fast5/
 multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
 ```
```

### Comparing `nanoCEM-0.0.2.3/README.md` & `nanoCEM-0.0.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # nanoCEM
 The nanopore current events magnifier (`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
-CEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
+NanoCEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
 
 It supports two re-squiggle pipeline(`Tombo` and `f5c`) and support `R9` and `R10`.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
 ## Example
 Here is an example to help the user confirm the installation of A2030 on 23S rRNA:
 ```sh
@@ -141,15 +141,15 @@
 multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
 extract_sub_fast5_from_bam -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
 # Remember to sample fastq if you sampled your fast5
 extract_sub_fastq_from_bam -i all.fastq -o final.fastq -b file.bam --chrom NR_103073.1 --pos 2030 
 ```
 ### 4 Re-squiggle
 #### 4.1 Tombo resquiggle (v1.5.0)
-Step 1 and 2 should run on your two sample respectively, before the step 5.
+Step 1 and 2 should run on your two sample respectively, before the step 3.
 1. Data format conversion
 
 If you did the subsample,skip this step and used ```subsample_single``` as the following input rather than ```single/```
 ```sh
 # assumed your fast5 file folder name is fast5/
 multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
 ```
```

### Comparing `nanoCEM-0.0.2.3/nanoCEM/CE_magnifier_test.py` & `nanoCEM-0.0.2.4/nanoCEM/CE_magnifier_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 import argparse
 import os
 import time
 import warnings
-
+import copy
 import pandas as pd
 from plotnine.exceptions import PlotnineWarning
 
 from nanoCEM.cem_utils import read_fasta_to_dic, reverse_fasta
 from nanoCEM.plot import signal_plot
 
 warnings.filterwarnings("ignore", category=PlotnineWarning)
@@ -93,15 +93,15 @@
         raise RuntimeError("The position requested is too close to the border (pos-len>0 and pos+len<length of fasta)")
     base_list = fasta[args.chrom][args.pos - args.len:args.pos + args.len + 1].upper()
 
     if args.strand == '-':
         base_list = "".join(list(reversed(base_list)))
         base_list = reverse_fasta(base_list)
 
-    title = args.chrom + ':' + str(args.pos - args.len + 1) + '-' + str(args.pos + args.len + 2) + ':' + args.strand
+    title = args.chrom + ':' + str(args.pos - args.len + 1) + '-' + str(args.pos + args.len + 1) + ':' + args.strand
     if args.rna:
         base_list = base_list.replace("T", "U")
         print("Running RNA mode ...")
         title = 'RNA  ' + title
     else:
         print("Running DNA mode ...")
         title = 'DNA  ' + title
@@ -162,22 +162,26 @@
         except:
             args.control = None
         if args.control is None:
             df = df_wt
             df_wt['type'] = 'Single'
             title = title + '   Sample:' + str(aligned_num_wt)
 
-    category_data = [str(args.pos + x) for x in range(-args.len, args.len + 1)]
-    category = pd.api.types.CategoricalDtype(categories=category_data, ordered=True)
-    df['position'] = df['position'].astype(category)
+
 
     # draw_volin(df,results_path,args.pos,base_list,title)
     # draw_boxplot(df,results_path,args.pos,base_list,title)
     print("Start to generate plots and save  in " + results_path)
-    df.to_csv(results_path + '/feature.csv', index=None)
+    df_copy=copy.deepcopy(df)
+    df_copy['position'] = df_copy['position'].astype(int) + 1
+    df_copy.to_csv(results_path + '/feature.csv', index=None)
+
+    category_data = [str(args.pos + x) for x in range(-args.len, args.len + 1)]
+    category = pd.api.types.CategoricalDtype(categories=category_data, ordered=True)
+    df['position'] = df['position'].astype(category)
     # if args.function == 'f5c':
     #     if (args.rna and args.strand == '+') or (not args.rna and args.strand == '-'):
     #         args.pos = args.pos - args.base_shift
     #     else:
     #         args.pos = args.pos + args.base_shift
     percentile_filter = False
     if aligned_num_wt > 50 and aligned_num_ivt > 50:
```

### Comparing `nanoCEM-0.0.2.3/nanoCEM/cem_utils.py` & `nanoCEM-0.0.2.4/nanoCEM/cem_utils.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.3/nanoCEM/current_events_magnifier` & `nanoCEM-0.0.2.4/nanoCEM/current_events_magnifier`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 import argparse
 import os
 import time
 import warnings
-
+import copy
 import pandas as pd
 from plotnine.exceptions import PlotnineWarning
 
 from nanoCEM.cem_utils import read_fasta_to_dic, reverse_fasta
 from nanoCEM.plot import signal_plot
 
 warnings.filterwarnings("ignore", category=PlotnineWarning)
@@ -77,15 +77,15 @@
         raise RuntimeError("The position requested is too close to the border (pos-len>0 and pos+len<length of fasta)")
     base_list = fasta[args.chrom][args.pos - args.len:args.pos + args.len + 1].upper()
 
     if args.strand == '-':
         base_list = "".join(list(reversed(base_list)))
         base_list = reverse_fasta(base_list)
 
-    title = args.chrom + ':' + str(args.pos - args.len + 1) + '-' + str(args.pos + args.len + 2) + ':' + args.strand
+    title = args.chrom + ':' + str(args.pos - args.len + 1) + '-' + str(args.pos + args.len + 1) + ':' + args.strand
     if args.rna:
         base_list = base_list.replace("T", "U")
         print("Running RNA mode ...")
         title = 'RNA  ' + title
     else:
         print("Running DNA mode ...")
         title = 'DNA  ' + title
@@ -146,22 +146,26 @@
         except:
             args.control = None
         if args.control is None:
             df = df_wt
             df_wt['type'] = 'Single'
             title = title + '   Sample:' + str(aligned_num_wt)
 
-    category_data = [str(args.pos + x) for x in range(-args.len, args.len + 1)]
-    category = pd.api.types.CategoricalDtype(categories=category_data, ordered=True)
-    df['position'] = df['position'].astype(category)
+
 
     # draw_volin(df,results_path,args.pos,base_list,title)
     # draw_boxplot(df,results_path,args.pos,base_list,title)
     print("Start to generate plots and save  in " + results_path)
-    df.to_csv(results_path + '/feature.csv', index=None)
+    df_copy=copy.deepcopy(df)
+    df_copy['position'] = df_copy['position'].astype(int) + 1
+    df_copy.to_csv(results_path + '/feature.csv', index=None)
+
+    category_data = [str(args.pos + x) for x in range(-args.len, args.len + 1)]
+    category = pd.api.types.CategoricalDtype(categories=category_data, ordered=True)
+    df['position'] = df['position'].astype(category)
     # if args.function == 'f5c':
     #     if (args.rna and args.strand == '+') or (not args.rna and args.strand == '-'):
     #         args.pos = args.pos - args.base_shift
     #     else:
     #         args.pos = args.pos + args.base_shift
     percentile_filter = False
     if aligned_num_wt > 50 and aligned_num_ivt > 50:
```

### Comparing `nanoCEM-0.0.2.3/nanoCEM/extract_sub_fast5_from_bam` & `nanoCEM-0.0.2.4/nanoCEM/extract_sub_fast5_from_bam`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.3/nanoCEM/extract_sub_fastq_from_bam` & `nanoCEM-0.0.2.4/nanoCEM/extract_sub_fastq_from_bam`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.3/nanoCEM/normalization.py` & `nanoCEM-0.0.2.4/nanoCEM/normalization.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.3/nanoCEM/plot.py` & `nanoCEM-0.0.2.4/nanoCEM/plot.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.3/nanoCEM/read_f5c_resquiggle.py` & `nanoCEM-0.0.2.4/nanoCEM/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.3/nanoCEM/read_tombo_resquiggle.py` & `nanoCEM-0.0.2.4/nanoCEM/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.3/nanoCEM.egg-info/PKG-INFO` & `nanoCEM-0.0.2.4/nanoCEM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.2.3
+Version: 0.0.2.4
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle program(tombo and f5c).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nanoCEM
 The nanopore current events magnifier (`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
-CEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
+NanoCEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
 
 It supports two re-squiggle pipeline(`Tombo` and `f5c`) and support `R9` and `R10`.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
 ## Example
 Here is an example to help the user confirm the installation of A2030 on 23S rRNA:
 ```sh
@@ -155,15 +155,15 @@
 multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
 extract_sub_fast5_from_bam -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
 # Remember to sample fastq if you sampled your fast5
 extract_sub_fastq_from_bam -i all.fastq -o final.fastq -b file.bam --chrom NR_103073.1 --pos 2030 
 ```
 ### 4 Re-squiggle
 #### 4.1 Tombo resquiggle (v1.5.0)
-Step 1 and 2 should run on your two sample respectively, before the step 5.
+Step 1 and 2 should run on your two sample respectively, before the step 3.
 1. Data format conversion
 
 If you did the subsample,skip this step and used ```subsample_single``` as the following input rather than ```single/```
 ```sh
 # assumed your fast5 file folder name is fast5/
 multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
 ```
```

### Comparing `nanoCEM-0.0.2.3/setup.py` & `nanoCEM-0.0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoCEM",
-    version="0.0.2.3",
+    version="0.0.2.4",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle program(tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/nanoCEM",
```

