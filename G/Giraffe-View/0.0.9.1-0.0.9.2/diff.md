# Comparing `tmp/Giraffe_View-0.0.9.1.tar.gz` & `tmp/Giraffe_View-0.0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Giraffe_View-0.0.9.1.tar", last modified: Fri Jul 21 06:16:18 2023, max compression
+gzip compressed data, was "Giraffe_View-0.0.9.2.tar", last modified: Fri Jul 21 06:38:23 2023, max compression
```

## Comparing `Giraffe_View-0.0.9.1.tar` & `Giraffe_View-0.0.9.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-21 06:16:18.748794 Giraffe_View-0.0.9.1/
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-21 06:16:18.744794 Giraffe_View-0.0.9.1/Giraffe_View/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       57 2023-07-18 11:47:04.000000 Giraffe_View-0.0.9.1/Giraffe_View/__init__.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2835 2023-07-18 10:42:50.000000 Giraffe_View-0.0.9.1/Giraffe_View/estimated_read_accuracy.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4539 2023-07-18 10:42:50.000000 Giraffe_View-0.0.9.1/Giraffe_View/function.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3288 2023-07-18 11:57:08.000000 Giraffe_View-0.0.9.1/Giraffe_View/gc_bias.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3655 2023-07-21 06:09:08.000000 Giraffe_View-0.0.9.1/Giraffe_View/giraffe
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4721 2023-07-18 12:03:26.000000 Giraffe_View-0.0.9.1/Giraffe_View/homopolymer.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2944 2023-07-18 10:42:50.000000 Giraffe_View-0.0.9.1/Giraffe_View/observed_read_accuracy.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     5505 2023-07-21 05:59:39.000000 Giraffe_View-0.0.9.1/Giraffe_View/plot.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2156 2023-07-18 10:42:50.000000 Giraffe_View-0.0.9.1/Giraffe_View/regional_modification.py
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-21 06:16:18.744794 Giraffe_View-0.0.9.1/Giraffe_View.egg-info/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5057 2023-07-21 06:16:18.000000 Giraffe_View-0.0.9.1/Giraffe_View.egg-info/PKG-INFO
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      466 2023-07-21 06:16:18.000000 Giraffe_View-0.0.9.1/Giraffe_View.egg-info/SOURCES.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2023-07-21 06:16:18.000000 Giraffe_View-0.0.9.1/Giraffe_View.egg-info/dependency_links.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       64 2023-07-21 06:16:18.000000 Giraffe_View-0.0.9.1/Giraffe_View.egg-info/requires.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2023-07-21 06:16:18.000000 Giraffe_View-0.0.9.1/Giraffe_View.egg-info/top_level.txt
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2023-07-18 10:44:57.000000 Giraffe_View-0.0.9.1/LICENSE
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5057 2023-07-21 06:16:18.748794 Giraffe_View-0.0.9.1/PKG-INFO
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4662 2023-07-21 06:12:03.000000 Giraffe_View-0.0.9.1/README.md
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2023-07-21 06:16:18.748794 Giraffe_View-0.0.9.1/setup.cfg
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)      931 2023-07-21 06:16:04.000000 Giraffe_View-0.0.9.1/setup.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-21 06:38:23.269874 Giraffe_View-0.0.9.2/
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-21 06:38:23.265874 Giraffe_View-0.0.9.2/Giraffe_View/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       57 2023-07-18 11:47:04.000000 Giraffe_View-0.0.9.2/Giraffe_View/__init__.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2835 2023-07-18 10:42:50.000000 Giraffe_View-0.0.9.2/Giraffe_View/estimated_read_accuracy.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4539 2023-07-18 10:42:50.000000 Giraffe_View-0.0.9.2/Giraffe_View/function.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3288 2023-07-18 11:57:08.000000 Giraffe_View-0.0.9.2/Giraffe_View/gc_bias.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4357 2023-07-21 06:37:43.000000 Giraffe_View-0.0.9.2/Giraffe_View/giraffe
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4721 2023-07-18 12:03:26.000000 Giraffe_View-0.0.9.2/Giraffe_View/homopolymer.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2944 2023-07-18 10:42:50.000000 Giraffe_View-0.0.9.2/Giraffe_View/observed_read_accuracy.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     5505 2023-07-21 05:59:39.000000 Giraffe_View-0.0.9.2/Giraffe_View/plot.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2156 2023-07-18 10:42:50.000000 Giraffe_View-0.0.9.2/Giraffe_View/regional_modification.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-21 06:38:23.269874 Giraffe_View-0.0.9.2/Giraffe_View.egg-info/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5057 2023-07-21 06:38:23.000000 Giraffe_View-0.0.9.2/Giraffe_View.egg-info/PKG-INFO
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      466 2023-07-21 06:38:23.000000 Giraffe_View-0.0.9.2/Giraffe_View.egg-info/SOURCES.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2023-07-21 06:38:23.000000 Giraffe_View-0.0.9.2/Giraffe_View.egg-info/dependency_links.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       64 2023-07-21 06:38:23.000000 Giraffe_View-0.0.9.2/Giraffe_View.egg-info/requires.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2023-07-21 06:38:23.000000 Giraffe_View-0.0.9.2/Giraffe_View.egg-info/top_level.txt
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2023-07-18 10:44:57.000000 Giraffe_View-0.0.9.2/LICENSE
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5057 2023-07-21 06:38:23.269874 Giraffe_View-0.0.9.2/PKG-INFO
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4662 2023-07-21 06:12:03.000000 Giraffe_View-0.0.9.2/README.md
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2023-07-21 06:38:23.269874 Giraffe_View-0.0.9.2/setup.cfg
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)      931 2023-07-21 06:18:35.000000 Giraffe_View-0.0.9.2/setup.py
```

### Comparing `Giraffe_View-0.0.9.1/Giraffe_View/estimated_read_accuracy.py` & `Giraffe_View-0.0.9.2/Giraffe_View/estimated_read_accuracy.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.1/Giraffe_View/function.py` & `Giraffe_View-0.0.9.2/Giraffe_View/function.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.1/Giraffe_View/gc_bias.py` & `Giraffe_View-0.0.9.2/Giraffe_View/gc_bias.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.1/Giraffe_View/giraffe` & `Giraffe_View-0.0.9.2/Giraffe_View/giraffe`

 * *Files 12% similar despite different names*

```diff
@@ -7,78 +7,97 @@
 from Giraffe_View.gc_bias import *
 from Giraffe_View.estimated_read_accuracy import *
 from Giraffe_View.regional_modification import *
 from Giraffe_View.plot import *
 
 def observed(args):
     Data_process(args.input, args.ref, args.cpu)
-
     print("Start observed accuracy analysis!")
     observed_accuracy("results/quality/tmp.sort.bam")
-    
     print("Start homopolymer identification!")
+
     homopolymer_from_bam("results/quality/tmp.sort.bam")
     homopolymer_summary_1("results/quality/homo.txt")
     homopolymer_summary_2()
-    # Rplot("quality.R")
+    
+    if args.plot:
+        print("Start plotting!")
+        plot_observe()
+        print("Analysis finished!")
+    else:
+        print("Analysis finished!")
+
 
 def methylation(args):
     mkdir_d("regional_modification")
     methylation_calculation(args.input, args.ref, args.cpu)
 
+
 def GC_bias(args):
     mkdir_d("GC_bias")
     compute_GC_bias(args.ref, args.input, args.binsize)
     merge_CG_content_and_depth(args.binsize)
 
+    if args.plot:
+        print("Start plotting!")
+        plot_GC_bias()
+        print("Analysis finished!")
+    else:
+        print("Analysis finished!")
+
 def estimated(args):
     mkdir_d("estimated")
     calculate_estimated_accuracy(args.input, args.cpu)
+    
+    if args.plot:
+        print("Start plotting!")
+        plot_estimate()
+        print("Analysis finished!")
+    else:
+        print("Analysis finished!")
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(prog="giraffe", description="A tool to help you assess quality of ONT data.")
 
     # Define subparsers
     subparsers = parser.add_subparsers(dest='function', help="")
     observed_parser = subparsers.add_parser('observe', help='Observed quality in accuracy, mismatch, and homopolymer')
     observed_parser.add_argument("--input", type=str, metavar="<fastq>", required=True, help="input reads")
     observed_parser.add_argument("--ref", type=str, metavar="<reference>", required=True, help="input reference")
     observed_parser.add_argument("--cpu", type=int, metavar="<number>", required=False, help="number of cpu (default:10)", default=10)
+    observed_parser.add_argument("--plot", required=False, help="Results visualization", action='store_true')
 
     estimated_parser = subparsers.add_parser('estimate', help='Estimated read accuracy')
     estimated_parser.add_argument("--input", type=str, metavar="<fastq>", required=True, help="input reads")
     estimated_parser.add_argument("--cpu", type=int, metavar="<number>", required=False, help="number of cpu (default:10)", default=10)
-
+    estimated_parser.add_argument("--plot", required=False, help="Results visualization", action='store_true')
 
     methylation_parser = subparsers.add_parser('modi', help='Average modification proportion of regions')
     methylation_parser.add_argument("--input", type=str, metavar="<bed>", required=True, help="input bed file")
     methylation_parser.add_argument("--ref", type=str, metavar="<reference>", required=True, help="input reference")
     methylation_parser.add_argument("--cpu", type=int, metavar="<number>", required=False, help="number of cpu (default:10)", default=10)
 
     GC_bias_parser = subparsers.add_parser('gc_bias', help='Relationship between GC content and depth')
     GC_bias_parser.add_argument("--ref", type=str, metavar="<reference>", required=True, help="input reference file")
     GC_bias_parser.add_argument("--input", type=str, metavar="<sam/bam>", required=True, help="input bam/sam file")
     GC_bias_parser.add_argument("--binsize", type=int, metavar="", required=False, help="input bin size (default:1000)", default=1000)
-
+    GC_bias_parser.add_argument("--plot", required=False, help="Results visualization", action='store_true')
 
     # Add function to print help if no arguments are provided
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         sys.exit(1)
 
     args = parser.parse_args()
 
     # Call the appropriate function based on the subparser used
     if args.function == "observe":
         observed(args)
-        plot_observe()
 
     elif args.function == "modi":
         methylation(args)
-    
-    elif args.function == "GC_bias":
+
+    elif args.function == "gc_bias":
         GC_bias(args)
-        plot_GC_bias()
-    
+
     elif args.function == "estimate":
         estimated(args)
-        plot_estimate()
```

### Comparing `Giraffe_View-0.0.9.1/Giraffe_View/homopolymer.py` & `Giraffe_View-0.0.9.2/Giraffe_View/homopolymer.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.1/Giraffe_View/observed_read_accuracy.py` & `Giraffe_View-0.0.9.2/Giraffe_View/observed_read_accuracy.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.1/Giraffe_View/plot.py` & `Giraffe_View-0.0.9.2/Giraffe_View/plot.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.1/Giraffe_View/regional_modification.py` & `Giraffe_View-0.0.9.2/Giraffe_View/regional_modification.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.1/Giraffe_View.egg-info/PKG-INFO` & `Giraffe_View-0.0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Giraffe-View
-Version: 0.0.9.1
+Name: Giraffe_View
+Version: 0.0.9.2
 Summary: A small tool help assess and visualize the accuracy of a sequencing dataset,   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Giraffe_View-0.0.9.1/LICENSE` & `Giraffe_View-0.0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.1/PKG-INFO` & `Giraffe_View-0.0.9.2/Giraffe_View.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Giraffe_View
-Version: 0.0.9.1
+Name: Giraffe-View
+Version: 0.0.9.2
 Summary: A small tool help assess and visualize the accuracy of a sequencing dataset,   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Giraffe_View-0.0.9.1/README.md` & `Giraffe_View-0.0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.1/setup.py` & `Giraffe_View-0.0.9.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="Giraffe_View",
-  version="0.0.9.1",
+  version="0.0.9.2",
   author="Xudong Liu",
   author_email="xudongliu98@gmail.com",
   description="A small tool help assess and visualize the accuracy of a sequencing dataset, \
   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/lxd98/Giraffe_View",
```

