# Comparing `tmp/Giraffe_View-0.0.8.tar.gz` & `tmp/Giraffe_View-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Giraffe_View-0.0.8.tar", last modified: Tue Jul 18 12:26:02 2023, max compression
+gzip compressed data, was "Giraffe_View-0.0.9.tar", last modified: Fri Jul 21 06:13:09 2023, max compression
```

## Comparing `Giraffe_View-0.0.8.tar` & `Giraffe_View-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 12:26:02.045840 Giraffe_View-0.0.8/
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 12:26:02.041840 Giraffe_View-0.0.8/Giraffe_View/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3288 2023-07-18 11:57:08.000000 Giraffe_View-0.0.8/Giraffe_View/GC_bias.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3658 2023-07-18 12:19:24.000000 Giraffe_View-0.0.8/Giraffe_View/Giraffe
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       57 2023-07-18 11:47:04.000000 Giraffe_View-0.0.8/Giraffe_View/__init__.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2835 2023-07-18 10:42:50.000000 Giraffe_View-0.0.8/Giraffe_View/estimated_read_accuracy.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4539 2023-07-18 10:42:50.000000 Giraffe_View-0.0.8/Giraffe_View/function.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4721 2023-07-18 12:03:26.000000 Giraffe_View-0.0.8/Giraffe_View/homopolymer.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2944 2023-07-18 10:42:50.000000 Giraffe_View-0.0.8/Giraffe_View/observed_read_accuracy.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5319 2023-07-18 10:42:50.000000 Giraffe_View-0.0.8/Giraffe_View/plot.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2156 2023-07-18 10:42:50.000000 Giraffe_View-0.0.8/Giraffe_View/regional_modification.py
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 12:26:02.045840 Giraffe_View-0.0.8/Giraffe_View.egg-info/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5167 2023-07-18 12:26:01.000000 Giraffe_View-0.0.8/Giraffe_View.egg-info/PKG-INFO
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      466 2023-07-18 12:26:02.000000 Giraffe_View-0.0.8/Giraffe_View.egg-info/SOURCES.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2023-07-18 12:26:01.000000 Giraffe_View-0.0.8/Giraffe_View.egg-info/dependency_links.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       65 2023-07-18 12:26:01.000000 Giraffe_View-0.0.8/Giraffe_View.egg-info/requires.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2023-07-18 12:26:01.000000 Giraffe_View-0.0.8/Giraffe_View.egg-info/top_level.txt
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2023-07-18 10:44:57.000000 Giraffe_View-0.0.8/LICENSE
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5167 2023-07-18 12:26:02.045840 Giraffe_View-0.0.8/PKG-INFO
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4774 2023-07-18 10:39:38.000000 Giraffe_View-0.0.8/README.md
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2023-07-18 12:26:02.045840 Giraffe_View-0.0.8/setup.cfg
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)      930 2023-07-18 12:25:57.000000 Giraffe_View-0.0.8/setup.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-21 06:13:09.812969 Giraffe_View-0.0.9/
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-21 06:13:09.812969 Giraffe_View-0.0.9/Giraffe_View/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       57 2023-07-18 11:47:04.000000 Giraffe_View-0.0.9/Giraffe_View/__init__.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2835 2023-07-18 10:42:50.000000 Giraffe_View-0.0.9/Giraffe_View/estimated_read_accuracy.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4539 2023-07-18 10:42:50.000000 Giraffe_View-0.0.9/Giraffe_View/function.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3288 2023-07-18 11:57:08.000000 Giraffe_View-0.0.9/Giraffe_View/gc_bias.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4721 2023-07-18 12:03:26.000000 Giraffe_View-0.0.9/Giraffe_View/homopolymer.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2944 2023-07-18 10:42:50.000000 Giraffe_View-0.0.9/Giraffe_View/observed_read_accuracy.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     5505 2023-07-21 05:59:39.000000 Giraffe_View-0.0.9/Giraffe_View/plot.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2156 2023-07-18 10:42:50.000000 Giraffe_View-0.0.9/Giraffe_View/regional_modification.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-21 06:13:09.812969 Giraffe_View-0.0.9/Giraffe_View.egg-info/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5055 2023-07-21 06:13:09.000000 Giraffe_View-0.0.9/Giraffe_View.egg-info/PKG-INFO
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      445 2023-07-21 06:13:09.000000 Giraffe_View-0.0.9/Giraffe_View.egg-info/SOURCES.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2023-07-21 06:13:09.000000 Giraffe_View-0.0.9/Giraffe_View.egg-info/dependency_links.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       64 2023-07-21 06:13:09.000000 Giraffe_View-0.0.9/Giraffe_View.egg-info/requires.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2023-07-21 06:13:09.000000 Giraffe_View-0.0.9/Giraffe_View.egg-info/top_level.txt
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2023-07-18 10:44:57.000000 Giraffe_View-0.0.9/LICENSE
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5055 2023-07-21 06:13:09.812969 Giraffe_View-0.0.9/PKG-INFO
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4662 2023-07-21 06:12:03.000000 Giraffe_View-0.0.9/README.md
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2023-07-21 06:13:09.812969 Giraffe_View-0.0.9/setup.cfg
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)      929 2023-07-21 06:07:29.000000 Giraffe_View-0.0.9/setup.py
```

### Comparing `Giraffe_View-0.0.8/Giraffe_View/GC_bias.py` & `Giraffe_View-0.0.9/Giraffe_View/gc_bias.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.8/Giraffe_View/estimated_read_accuracy.py` & `Giraffe_View-0.0.9/Giraffe_View/estimated_read_accuracy.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.8/Giraffe_View/function.py` & `Giraffe_View-0.0.9/Giraffe_View/function.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.8/Giraffe_View/homopolymer.py` & `Giraffe_View-0.0.9/Giraffe_View/homopolymer.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.8/Giraffe_View/observed_read_accuracy.py` & `Giraffe_View-0.0.9/Giraffe_View/observed_read_accuracy.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.8/Giraffe_View/plot.py` & `Giraffe_View-0.0.9/Giraffe_View/plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,19 +48,21 @@
 	    scale_x_discrete(name="Type", labels=c("Ins", "Del", "Sub")) +
 	    theme(axis.text=element_text(size=12, family = "Arial", color="black"),
 	          axis.title=element_text(size=12, family = "Arial", color="black"),
 	          legend.text = element_text(size=12, family = "Arial", color="black"))
 	  return(p)
 	}
 
-	A <- acc("results/quality/final_observed_accuracy.txt") + 
-		mismatch("results/quality/final_observed_accuracy.txt") + 
-		homo("results/quality/final_homo_summary.txt")
+	A <- acc("results/quality/final_observed_accuracy.txt") 
+	B <- mismatch("results/quality/final_observed_accuracy.txt")
+	C <- homo("results/quality/final_homo_summary.txt")
 	
-	ggsave("observe.png", A, path="./results/quality/", dpi=300, width=12, height=5)
+	ggsave("observe_accuracy.png", A, path="./results/quality/", dpi=300, width=12, height=5)
+	ggsave("observe_mismatch.png", B, path="./results/quality/", dpi=300, width=12, height=5)
+	ggsave("homopolymer_identification.png", C, path="./results/quality/", dpi=300, width=12, height=5)
 	'''
 	robjects.r(rscript)
 
 def plot_estimate():
 	rscript = '''
 	library(ggplot2)
 	library(reshape2)
@@ -74,15 +76,15 @@
 	    theme(axis.text=element_text(size=12, family = "Arial", color="black"),
 	          axis.title=element_text(size=12, family = "Arial", color="black"),
 	          legend.text = element_text(size=12, family = "Arial", color="black"))
 	  return(p)
 	}
 
 	A <- estimated("results/estimated/final_estimated_accuracy.txt")
-	ggsave("estimate.png", A, path="./results/estimated/", dpi=300, width=8, height=5)
+	ggsave("estimate.png", A, path="./results/estimated/", dpi=300)
 	'''
 	robjects.r(rscript)
 
 def plot_GC_bias():
 	rscript = '''
 	library(ggplot2)
 	library(patchwork)
@@ -112,8 +114,8 @@
 	          legend.title = element_blank(), legend.position = "bottom")
 	  return(p)
 	}
 
 	A <- bin_count("results/GC_bias/GC_bias_raw.txt")/GC_bias("results/GC_bias/final_GC_bias_nor.txt")
 	ggsave("GC_bias.png", A, path="./results/GC_bias/", dpi=300, width=8, height=5)
 	'''
-	robjects.r(rscript)
+	robjects.r(rscript)
```

### Comparing `Giraffe_View-0.0.8/Giraffe_View/regional_modification.py` & `Giraffe_View-0.0.9/Giraffe_View/regional_modification.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.8/Giraffe_View.egg-info/PKG-INFO` & `Giraffe_View-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Giraffe-View
-Version: 0.0.8
+Name: Giraffe_View
+Version: 0.0.9
 Summary: A small tool help assess and visualize the accuracy of a sequencing dataset,   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,70 +14,70 @@
 
 # Giraffe_View 
 
 **Giraffe_View** is designed to help assess and visualize the accuracy of a sequencing dataset, specifically for Oxford Nanopore Technologies (ONT) long-read sequencing including DNA and RNA data. There are four main functions to validate the read quality.
 
 - `observe`  calculates the observed read accuracy, mismatches porportion, and homopolymer identification.
 - `estimate`  calculates the estimated read accuracy, which is equal to Quality Score.
-- `GC_bias`  compares the relationship between GC content and read coverage.
+- `gc_bias`  compares the relationship between GC content and read coverage.
 - `modi` perform statistics on the distribution of modification based on the bed file.
 
 
 
 ## Install
 
-To use this software, you will need to install additional dependencies including samtools, minimap2, seqkit, pysam, numpy, and pandas. You can install these dependencies using the following command.
+To use this software, you need to install additional dependencies including samtools, minimap2, and seqkit for read processing and ggplot2 and patchwork for figure plotting.
+
+The following commands can help you to install the package  and dependencies.
 
 ```shell
-# for data processing
-pip install rpy2==3.0 pysam numpy pandas
-conda install -c bioconda -c conda-forge samtools minimap2 seqkit bedtools -y
+pip install Giraffe-View
 
-# for figure plotting
-conda install -c R ggplot2 patchwork -y
+conda install -c bioconda -c conda-forge samtools minimap2 seqkit bedtools -y
+conda install -c conda-forge r-ggplot2 r-patchwork -y
 ```
 
 
 
 ## General Usage
 
 Giraffe View is run simply with fllowing commands:
 
 ```shell
-python Giraffe_View.py --help
+giraffe -h
 ```
 
 ```shell
-usage: Giraffe_view [-h] {observe,modi,GC_bias,estimate} ...
+usage: giraffe [-h] {observe,modi,gc_bias,estimate} ...
 
 A tool to help you assess quality of your ONT data.
 
 positional arguments:
-  {observe,modi,GC_bias,estimate}
+  {observe,modi,gc_bias,estimate}
     observe             Observed quality in accuracy, mismatch, and homopolymer
     modi                Average modification proportion of regions
-    GC_bias             Relationship between GC content and depth
+    gc_bias             Relationship between GC content and depth
     estimate            Estimated read accuracy
 
 optional arguments:
   -h, --help            show this help message and exit
 ```
 
 
 
 The available sub-commands are:
 
 ### observe
 
 ```shell
-python Giraffe_View.py observe --help
+giraffe observe -h
 ```
 
 ```xshell
-usage: Giraffe_view observe [-h] --input <fastq> --ref <reference> [--cpu <number>]
+usage: giraffe observe [-h] --input <fastq> --ref <reference> [--cpu <number>]
 
 optional arguments:
   -h, --help         show this help message and exit
   --input <fastq>    input reads
   --ref <reference>  input reference
   --cpu <number>     number of cpu (default:10)
 ```
@@ -87,36 +87,36 @@
 - `cpu` - the number of CPUs will be used during processing.
 
 
 
 ### estimate  
 
 ```shell
-python Giraffe_View.py estimate --help
+giraffe estimate -h
 ```
 
 ```shell
-usage: Giraffe_view estimate [-h] --input <fastq> [--cpu <number>]
+usage: giraffe estimate [-h] --input <fastq> [--cpu <number>]
 
 optional arguments:
   -h, --help       show this help message and exit
   --input <fastq>  input reads
   --cpu <number>   number of cpu (default:10)
 ```
 
 
 
-### GC_bias
+### gc_bias
 
 ```shell
-python Giraffe_View.py GC_bias --help
+giraffe gc_bias -h
 ```
 
 ```shell
-usage: Giraffe_view GC_bias [-h] --ref <reference> --input <sam/bam> [--binsize]
+usage: giraffe gc_bias [-h] --ref <reference> --input <sam/bam> [--binsize]
 
 optional arguments:
   -h, --help         show this help message and exit
   --ref <reference>  input reference file
   --input <sam/bam>  input bam/sam file
   --binsize          input bin size (default:1000)
 ```
@@ -126,19 +126,19 @@
 - `binsize` - the length of bin. A bin is the smallest unit to count the read coverage and GC content.
 
 
 
 ### modi
 
 ```shell
-python Giraffe_View.py modi --help
+giraffe modi -h
 ```
 
 ```shell
-usage: Giraffe_view modi [-h] --input <bed> --ref <reference> [--cpu <number>]
+usage: giraffe modi [-h] --input <bed> --ref <reference> [--cpu <number>]
 
 optional arguments:
   -h, --help         show this help message and exit
   --input <bed>      input bed file
   --ref <reference>  input reference
   --cpu <number>     number of cpu (default:10)
 ```
@@ -177,8 +177,8 @@
 
 
 
 ## Developing
 
 - A example to show how to run
 - polish the result figures
-- run the homopolymer identification with multi-processes
+- run the homopolymer identification with multi-processed
```

### Comparing `Giraffe_View-0.0.8/LICENSE` & `Giraffe_View-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.8/PKG-INFO` & `Giraffe_View-0.0.9/Giraffe_View.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Giraffe_View
-Version: 0.0.8
+Name: Giraffe-View
+Version: 0.0.9
 Summary: A small tool help assess and visualize the accuracy of a sequencing dataset,   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,70 +14,70 @@
 
 # Giraffe_View 
 
 **Giraffe_View** is designed to help assess and visualize the accuracy of a sequencing dataset, specifically for Oxford Nanopore Technologies (ONT) long-read sequencing including DNA and RNA data. There are four main functions to validate the read quality.
 
 - `observe`  calculates the observed read accuracy, mismatches porportion, and homopolymer identification.
 - `estimate`  calculates the estimated read accuracy, which is equal to Quality Score.
-- `GC_bias`  compares the relationship between GC content and read coverage.
+- `gc_bias`  compares the relationship between GC content and read coverage.
 - `modi` perform statistics on the distribution of modification based on the bed file.
 
 
 
 ## Install
 
-To use this software, you will need to install additional dependencies including samtools, minimap2, seqkit, pysam, numpy, and pandas. You can install these dependencies using the following command.
+To use this software, you need to install additional dependencies including samtools, minimap2, and seqkit for read processing and ggplot2 and patchwork for figure plotting.
+
+The following commands can help you to install the package  and dependencies.
 
 ```shell
-# for data processing
-pip install rpy2==3.0 pysam numpy pandas
-conda install -c bioconda -c conda-forge samtools minimap2 seqkit bedtools -y
+pip install Giraffe-View
 
-# for figure plotting
-conda install -c R ggplot2 patchwork -y
+conda install -c bioconda -c conda-forge samtools minimap2 seqkit bedtools -y
+conda install -c conda-forge r-ggplot2 r-patchwork -y
 ```
 
 
 
 ## General Usage
 
 Giraffe View is run simply with fllowing commands:
 
 ```shell
-python Giraffe_View.py --help
+giraffe -h
 ```
 
 ```shell
-usage: Giraffe_view [-h] {observe,modi,GC_bias,estimate} ...
+usage: giraffe [-h] {observe,modi,gc_bias,estimate} ...
 
 A tool to help you assess quality of your ONT data.
 
 positional arguments:
-  {observe,modi,GC_bias,estimate}
+  {observe,modi,gc_bias,estimate}
     observe             Observed quality in accuracy, mismatch, and homopolymer
     modi                Average modification proportion of regions
-    GC_bias             Relationship between GC content and depth
+    gc_bias             Relationship between GC content and depth
     estimate            Estimated read accuracy
 
 optional arguments:
   -h, --help            show this help message and exit
 ```
 
 
 
 The available sub-commands are:
 
 ### observe
 
 ```shell
-python Giraffe_View.py observe --help
+giraffe observe -h
 ```
 
 ```xshell
-usage: Giraffe_view observe [-h] --input <fastq> --ref <reference> [--cpu <number>]
+usage: giraffe observe [-h] --input <fastq> --ref <reference> [--cpu <number>]
 
 optional arguments:
   -h, --help         show this help message and exit
   --input <fastq>    input reads
   --ref <reference>  input reference
   --cpu <number>     number of cpu (default:10)
 ```
@@ -87,36 +87,36 @@
 - `cpu` - the number of CPUs will be used during processing.
 
 
 
 ### estimate  
 
 ```shell
-python Giraffe_View.py estimate --help
+giraffe estimate -h
 ```
 
 ```shell
-usage: Giraffe_view estimate [-h] --input <fastq> [--cpu <number>]
+usage: giraffe estimate [-h] --input <fastq> [--cpu <number>]
 
 optional arguments:
   -h, --help       show this help message and exit
   --input <fastq>  input reads
   --cpu <number>   number of cpu (default:10)
 ```
 
 
 
-### GC_bias
+### gc_bias
 
 ```shell
-python Giraffe_View.py GC_bias --help
+giraffe gc_bias -h
 ```
 
 ```shell
-usage: Giraffe_view GC_bias [-h] --ref <reference> --input <sam/bam> [--binsize]
+usage: giraffe gc_bias [-h] --ref <reference> --input <sam/bam> [--binsize]
 
 optional arguments:
   -h, --help         show this help message and exit
   --ref <reference>  input reference file
   --input <sam/bam>  input bam/sam file
   --binsize          input bin size (default:1000)
 ```
@@ -126,19 +126,19 @@
 - `binsize` - the length of bin. A bin is the smallest unit to count the read coverage and GC content.
 
 
 
 ### modi
 
 ```shell
-python Giraffe_View.py modi --help
+giraffe modi -h
 ```
 
 ```shell
-usage: Giraffe_view modi [-h] --input <bed> --ref <reference> [--cpu <number>]
+usage: giraffe modi [-h] --input <bed> --ref <reference> [--cpu <number>]
 
 optional arguments:
   -h, --help         show this help message and exit
   --input <bed>      input bed file
   --ref <reference>  input reference
   --cpu <number>     number of cpu (default:10)
 ```
@@ -177,8 +177,8 @@
 
 
 
 ## Developing
 
 - A example to show how to run
 - polish the result figures
-- run the homopolymer identification with multi-processes
+- run the homopolymer identification with multi-processed
```

### Comparing `Giraffe_View-0.0.8/README.md` & `Giraffe_View-0.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 # Giraffe_View 
 
 **Giraffe_View** is designed to help assess and visualize the accuracy of a sequencing dataset, specifically for Oxford Nanopore Technologies (ONT) long-read sequencing including DNA and RNA data. There are four main functions to validate the read quality.
 
 - `observe`  calculates the observed read accuracy, mismatches porportion, and homopolymer identification.
 - `estimate`  calculates the estimated read accuracy, which is equal to Quality Score.
-- `GC_bias`  compares the relationship between GC content and read coverage.
+- `gc_bias`  compares the relationship between GC content and read coverage.
 - `modi` perform statistics on the distribution of modification based on the bed file.
 
 
 
 ## Install
 
-To use this software, you will need to install additional dependencies including samtools, minimap2, seqkit, pysam, numpy, and pandas. You can install these dependencies using the following command.
+To use this software, you need to install additional dependencies including samtools, minimap2, and seqkit for read processing and ggplot2 and patchwork for figure plotting.
+
+The following commands can help you to install the package  and dependencies.
 
 ```shell
-# for data processing
-pip install rpy2==3.0 pysam numpy pandas
-conda install -c bioconda -c conda-forge samtools minimap2 seqkit bedtools -y
+pip install Giraffe-View
 
-# for figure plotting
-conda install -c R ggplot2 patchwork -y
+conda install -c bioconda -c conda-forge samtools minimap2 seqkit bedtools -y
+conda install -c conda-forge r-ggplot2 r-patchwork -y
 ```
 
 
 
 ## General Usage
 
 Giraffe View is run simply with fllowing commands:
 
 ```shell
-python Giraffe_View.py --help
+giraffe -h
 ```
 
 ```shell
-usage: Giraffe_view [-h] {observe,modi,GC_bias,estimate} ...
+usage: giraffe [-h] {observe,modi,gc_bias,estimate} ...
 
 A tool to help you assess quality of your ONT data.
 
 positional arguments:
-  {observe,modi,GC_bias,estimate}
+  {observe,modi,gc_bias,estimate}
     observe             Observed quality in accuracy, mismatch, and homopolymer
     modi                Average modification proportion of regions
-    GC_bias             Relationship between GC content and depth
+    gc_bias             Relationship between GC content and depth
     estimate            Estimated read accuracy
 
 optional arguments:
   -h, --help            show this help message and exit
 ```
 
 
 
 The available sub-commands are:
 
 ### observe
 
 ```shell
-python Giraffe_View.py observe --help
+giraffe observe -h
 ```
 
 ```xshell
-usage: Giraffe_view observe [-h] --input <fastq> --ref <reference> [--cpu <number>]
+usage: giraffe observe [-h] --input <fastq> --ref <reference> [--cpu <number>]
 
 optional arguments:
   -h, --help         show this help message and exit
   --input <fastq>    input reads
   --ref <reference>  input reference
   --cpu <number>     number of cpu (default:10)
 ```
@@ -73,36 +73,36 @@
 - `cpu` - the number of CPUs will be used during processing.
 
 
 
 ### estimate  
 
 ```shell
-python Giraffe_View.py estimate --help
+giraffe estimate -h
 ```
 
 ```shell
-usage: Giraffe_view estimate [-h] --input <fastq> [--cpu <number>]
+usage: giraffe estimate [-h] --input <fastq> [--cpu <number>]
 
 optional arguments:
   -h, --help       show this help message and exit
   --input <fastq>  input reads
   --cpu <number>   number of cpu (default:10)
 ```
 
 
 
-### GC_bias
+### gc_bias
 
 ```shell
-python Giraffe_View.py GC_bias --help
+giraffe gc_bias -h
 ```
 
 ```shell
-usage: Giraffe_view GC_bias [-h] --ref <reference> --input <sam/bam> [--binsize]
+usage: giraffe gc_bias [-h] --ref <reference> --input <sam/bam> [--binsize]
 
 optional arguments:
   -h, --help         show this help message and exit
   --ref <reference>  input reference file
   --input <sam/bam>  input bam/sam file
   --binsize          input bin size (default:1000)
 ```
@@ -112,19 +112,19 @@
 - `binsize` - the length of bin. A bin is the smallest unit to count the read coverage and GC content.
 
 
 
 ### modi
 
 ```shell
-python Giraffe_View.py modi --help
+giraffe modi -h
 ```
 
 ```shell
-usage: Giraffe_view modi [-h] --input <bed> --ref <reference> [--cpu <number>]
+usage: giraffe modi [-h] --input <bed> --ref <reference> [--cpu <number>]
 
 optional arguments:
   -h, --help         show this help message and exit
   --input <bed>      input bed file
   --ref <reference>  input reference
   --cpu <number>     number of cpu (default:10)
 ```
@@ -163,8 +163,8 @@
 
 
 
 ## Developing
 
 - A example to show how to run
 - polish the result figures
-- run the homopolymer identification with multi-processes
+- run the homopolymer identification with multi-processed
```

### Comparing `Giraffe_View-0.0.8/setup.py` & `Giraffe_View-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="Giraffe_View",
-  version="0.0.8",
+  version="0.0.9",
   author="Xudong Liu",
   author_email="xudongliu98@gmail.com",
   description="A small tool help assess and visualize the accuracy of a sequencing dataset, \
   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/lxd98/Giraffe_View",
@@ -17,15 +17,15 @@
   classifiers=[
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   ],
   python_requires = '>=3.7, <=3.10',
   install_requires=[
-  'pysam == 0.21.0',
+  'pysam >= 0.17.0',
   'rpy2==3.0',
-  'numpy == 1.25.1',
-  'pandas == 2.0.3',
+  'numpy >= 1.7.0',
+  'pandas >= 1.5.0',
   'tqdm == 4.64.0'
   ],
   scripts = ["Giraffe_View/Giraffe"]
 )
```

