# Comparing `tmp/pybio-0.3.8.tar.gz` & `tmp/pybio-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybio-0.3.8.tar", last modified: Thu Jun  1 10:29:11 2023, max compression
+gzip compressed data, was "pybio-0.3.9.tar", last modified: Tue Jun 13 13:30:33 2023, max compression
```

## Comparing `pybio-0.3.8.tar` & `pybio-0.3.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-01 10:29:11.014207 pybio-0.3.8/
--rw-rw-r--   0 rotg     (2023757) games       (20)     8857 2023-06-01 10:29:11.013775 pybio-0.3.8/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) games       (20)     8626 2023-04-28 08:19:03.000000 pybio-0.3.8/README.md
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-01 10:29:10.933599 pybio-0.3.8/pybio/
--rw-rw-r--   0 rotg     (2023757) games       (20)     7814 2023-05-03 14:56:57.000000 pybio-0.3.8/pybio/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-01 10:29:10.937919 pybio-0.3.8/pybio/config/
--rw-rw-r--   0 rotg     (2023757) games       (20)     1393 2023-05-31 12:19:35.000000 pybio-0.3.8/pybio/config/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-01 10:29:10.939244 pybio-0.3.8/pybio/core/
--rw-rw-r--   0 rotg     (2023757) games       (20)       98 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/core/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    27779 2023-05-11 11:48:32.000000 pybio-0.3.8/pybio/core/genomes.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-01 10:29:10.957484 pybio-0.3.8/pybio/data/
--rw-rw-r--   0 rotg     (2023757) games       (20)      877 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/data/Bam.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    16391 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/data/Bedgraph.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     4675 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/data/Bedgraph2.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1912 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/data/Fasta.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1244 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/data/Fastq.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1591 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/data/Gene.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      177 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/data/GeneFeature.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     3238 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/data/Gff3.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2777 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/data/Gtf.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      186 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/data/Sequence.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      906 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/data/Sissrs.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      956 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/data/TabReader.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2019 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/data/Wig.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2168 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/data/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-01 10:29:10.958565 pybio-0.3.8/pybio/expression/
--rw-rw-r--   0 rotg     (2023757) games       (20)     8831 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/expression/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-01 10:29:10.968073 pybio-0.3.8/pybio/map/
--rw-rw-r--   0 rotg     (2023757) games       (20)     2257 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/map/STAR.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      131 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/map/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1438 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/map/bowtie.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      580 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/map/nano.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1061 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/map/sege.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-01 10:29:10.985139 pybio-0.3.8/pybio/maths/
--rw-rw-r--   0 rotg     (2023757) games       (20)      974 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/maths/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    37335 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/maths/pstat.py
--rw-rw-r--   0 rotg     (2023757) games       (20)   151400 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/maths/stats.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-01 10:29:11.011218 pybio-0.3.8/pybio/path/
--rw-rw-r--   0 rotg     (2023757) games       (20)      347 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/path/__init__.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)     9827 2023-06-01 10:28:01.000000 pybio-0.3.8/pybio/pybio
--rw-rw-r--   0 rotg     (2023757) games       (20)      100 2023-04-26 07:30:50.000000 pybio-0.3.8/pybio/pybio.config.example
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-01 10:29:11.011728 pybio-0.3.8/pybio/sequence/
--rw-rw-r--   0 rotg     (2023757) games       (20)     5566 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/sequence/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-01 10:29:11.012916 pybio-0.3.8/pybio/utils/
--rw-rw-r--   0 rotg     (2023757) games       (20)    10199 2023-04-17 06:24:09.000000 pybio-0.3.8/pybio/utils/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-06-01 10:28:58.000000 pybio-0.3.8/pybio/version
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-01 10:29:10.936680 pybio-0.3.8/pybio.egg-info/
--rw-rw-r--   0 rotg     (2023757) games       (20)     8857 2023-06-01 10:29:10.934261 pybio-0.3.8/pybio.egg-info/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) games       (20)      892 2023-06-01 10:29:10.934640 pybio-0.3.8/pybio.egg-info/SOURCES.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-06-01 10:29:10.935031 pybio-0.3.8/pybio.egg-info/dependency_links.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-04-18 08:10:15.000000 pybio-0.3.8/pybio.egg-info/not-zip-safe
--rw-rw-r--   0 rotg     (2023757) games       (20)       32 2023-06-01 10:29:10.936175 pybio-0.3.8/pybio.egg-info/requires.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-06-01 10:29:10.936766 pybio-0.3.8/pybio.egg-info/top_level.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-06-01 10:29:11.014323 pybio-0.3.8/setup.cfg
--rw-rw-r--   0 rotg     (2023757) games       (20)      949 2023-04-17 08:00:52.000000 pybio-0.3.8/setup.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.557460 pybio-0.3.9/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     9263 2023-06-13 13:30:33.556998 pybio-0.3.9/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) games       (20)     9032 2023-06-05 13:06:07.000000 pybio-0.3.9/README.md
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.391168 pybio-0.3.9/pybio/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     7814 2023-05-03 14:56:57.000000 pybio-0.3.9/pybio/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.395238 pybio-0.3.9/pybio/config/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1482 2023-06-13 13:08:38.000000 pybio-0.3.9/pybio/config/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.396576 pybio-0.3.9/pybio/core/
+-rw-rw-r--   0 rotg     (2023757) games       (20)       98 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/core/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    27779 2023-05-11 11:48:32.000000 pybio-0.3.9/pybio/core/genomes.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.449869 pybio-0.3.9/pybio/data/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      877 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Bam.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    16391 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Bedgraph.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     4675 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Bedgraph2.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1912 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Fasta.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1244 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Fastq.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1591 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Gene.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      177 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/GeneFeature.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     3238 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Gff3.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2777 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Gtf.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      186 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Sequence.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      906 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Sissrs.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      956 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/TabReader.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2019 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Wig.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2168 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.450514 pybio-0.3.9/pybio/expression/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     8831 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/expression/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.482763 pybio-0.3.9/pybio/map/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2257 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/map/STAR.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      131 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/map/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1438 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/map/bowtie.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      580 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/map/nano.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1061 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/map/sege.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.503612 pybio-0.3.9/pybio/maths/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      974 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/maths/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    37335 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/maths/pstat.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)   151400 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/maths/stats.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.512562 pybio-0.3.9/pybio/path/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      347 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/path/__init__.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     9888 2023-06-13 12:59:21.000000 pybio-0.3.9/pybio/pybio
+-rw-rw-r--   0 rotg     (2023757) games       (20)      100 2023-04-26 07:30:50.000000 pybio-0.3.9/pybio/pybio.config.example
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.513209 pybio-0.3.9/pybio/sequence/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5566 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/sequence/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.535570 pybio-0.3.9/pybio/utils/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    10199 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/utils/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-06-13 13:30:19.000000 pybio-0.3.9/pybio/version
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.394517 pybio-0.3.9/pybio.egg-info/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     9263 2023-06-13 13:30:33.392073 pybio-0.3.9/pybio.egg-info/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) games       (20)      892 2023-06-13 13:30:33.392434 pybio-0.3.9/pybio.egg-info/SOURCES.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-06-13 13:30:33.392862 pybio-0.3.9/pybio.egg-info/dependency_links.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-04-18 08:10:15.000000 pybio-0.3.9/pybio.egg-info/not-zip-safe
+-rw-rw-r--   0 rotg     (2023757) games       (20)       32 2023-06-13 13:30:33.394022 pybio-0.3.9/pybio.egg-info/requires.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-06-13 13:30:33.394661 pybio-0.3.9/pybio.egg-info/top_level.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-06-13 13:30:33.557567 pybio-0.3.9/setup.cfg
+-rw-rw-r--   0 rotg     (2023757) games       (20)      949 2023-04-17 08:00:52.000000 pybio-0.3.9/setup.py
```

### Comparing `pybio-0.3.8/PKG-INFO` & `pybio-0.3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: pybio
-Version: 0.3.8
+Version: 0.3.9
 Summary: pybio genomics
 Home-page: https://github.com/grexor/pybio
 Author: Gregor Rot
 Author-email: gregor.rot@gmail.com
 Keywords: pybio,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 ## pybio: basic genomics toolset
 
 pybio is a Python framework for handling genomics operations and a direct interface to Ensembl genomes.
 
-Downloading an Ensembl genome+annotation takes one line: `pybio genome homo_sapiens`.
+Downloading an Ensembl genome+annotation takes one line:
+
+`$ pybio genome homo_sapiens`
 
 Features include genome+annotation download from Ensembl and processing with STAR and salmon, support of Fasta, Fastq, bedGraph and other file formats, motif sequence searches, and specific APA feautes like alternative polyadenylation site-pair classification (same-exon, skipped-exon, composite-exon) and more.
 
 ## Contents
 
 * [Installation](#installation)
 * [Quick Start](#Quick-Start)
@@ -30,15 +32,17 @@
 * [Authors](#authors)
 * [Reporting problems](#reporting-problems)
 
 ### Installation
 
 The easiest way to install pybio is running:
 
-`pip install pybio`
+`$ pip install pybio`
+
+Note that on some systems, pip is installing the executable scripts under `~/.local/bin`. However this folder is not in the PATH which will result in `command not found` if you try to run `$ pybio` on the command line. To fix this, please execute `export PATH="$PATH:~/.local/bin"` (and add this to your `.profile`). Another suggestion is to install inside a virtual environment (using `virtualenv`).
 
 If you would like instead to install the latest developmental version from this repository:
 
 ```
 # clone pybio repository locally
 git clone https://github.com/grexor/pybio.git
```

### Comparing `pybio-0.3.8/README.md` & `pybio-0.3.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 <picture><img src="media/pybio.png" width="70"/></picture>
 ## pybio: basic genomics toolset
 
 pybio is a Python framework for handling genomics operations and a direct interface to Ensembl genomes.
 
-Downloading an Ensembl genome+annotation takes one line: `pybio genome homo_sapiens`.
+Downloading an Ensembl genome+annotation takes one line:
+
+`$ pybio genome homo_sapiens`
 
 Features include genome+annotation download from Ensembl and processing with STAR and salmon, support of Fasta, Fastq, bedGraph and other file formats, motif sequence searches, and specific APA feautes like alternative polyadenylation site-pair classification (same-exon, skipped-exon, composite-exon) and more.
 
 ## Contents
 
 * [Installation](#installation)
 * [Quick Start](#Quick-Start)
@@ -20,15 +22,17 @@
 * [Authors](#authors)
 * [Reporting problems](#reporting-problems)
 
 ### Installation
 
 The easiest way to install pybio is running:
 
-`pip install pybio`
+`$ pip install pybio`
+
+Note that on some systems, pip is installing the executable scripts under `~/.local/bin`. However this folder is not in the PATH which will result in `command not found` if you try to run `$ pybio` on the command line. To fix this, please execute `export PATH="$PATH:~/.local/bin"` (and add this to your `.profile`). Another suggestion is to install inside a virtual environment (using `virtualenv`).
 
 If you would like instead to install the latest developmental version from this repository:
 
 ```
 # clone pybio repository locally
 git clone https://github.com/grexor/pybio.git
```

### Comparing `pybio-0.3.8/pybio/__init__.py` & `pybio-0.3.9/pybio/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/config/__init__.py` & `pybio-0.3.9/pybio/config/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import os
 import sys
 
+# pybio config file stored to ~/.pybio
+def config_fname():
+    config_fname = os.path.expanduser("~/.pybio")
+    return config_fname
+
 def init(genomes_folder=None):
     config_module = sys.modules[__name__]
     pybio_folder = os.path.abspath(os.path.join(os.path.abspath(__file__), "..", "..")) 
-    config_file = os.path.abspath(os.path.join(pybio_folder, "pybio.config"))
+    config_file = config_fname()
     config_example_file = os.path.abspath(os.path.join(pybio_folder, "pybio.config.example"))
     if not os.path.exists(config_file):
         config_example_file = os.path.abspath(os.path.join(pybio_folder, "pybio.config.example"))
         os.system(f"cp {config_example_file} {config_file}")
     config_lines = open(config_file).readlines()
     new_config = []
     for cline in config_lines:
```

### Comparing `pybio-0.3.8/pybio/core/genomes.py` & `pybio-0.3.9/pybio/core/genomes.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/data/Bam.py` & `pybio-0.3.9/pybio/data/Bam.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/data/Bedgraph.py` & `pybio-0.3.9/pybio/data/Bedgraph.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/data/Bedgraph2.py` & `pybio-0.3.9/pybio/data/Bedgraph2.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/data/Fasta.py` & `pybio-0.3.9/pybio/data/Fasta.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/data/Fastq.py` & `pybio-0.3.9/pybio/data/Fastq.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/data/Gene.py` & `pybio-0.3.9/pybio/data/Gene.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/data/Gff3.py` & `pybio-0.3.9/pybio/data/Gff3.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/data/Gtf.py` & `pybio-0.3.9/pybio/data/Gtf.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/data/Sissrs.py` & `pybio-0.3.9/pybio/data/Sissrs.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/data/TabReader.py` & `pybio-0.3.9/pybio/data/TabReader.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/data/Wig.py` & `pybio-0.3.9/pybio/data/Wig.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/data/__init__.py` & `pybio-0.3.9/pybio/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/expression/__init__.py` & `pybio-0.3.9/pybio/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/map/STAR.py` & `pybio-0.3.9/pybio/map/STAR.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/map/bowtie.py` & `pybio-0.3.9/pybio/map/bowtie.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/map/nano.py` & `pybio-0.3.9/pybio/map/nano.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/map/sege.py` & `pybio-0.3.9/pybio/map/sege.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/maths/__init__.py` & `pybio-0.3.9/pybio/maths/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/maths/pstat.py` & `pybio-0.3.9/pybio/maths/pstat.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/maths/stats.py` & `pybio-0.3.9/pybio/maths/stats.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/pybio` & `pybio-0.3.9/pybio/pybio`

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 
 Example:
 
 $ pybio sam2bam file1.sam file1.bam
 """
 
 print(f"[pybio] v{pybio.version}, https://github.com/grexor/pybio")
+print(f"[pybio] config file: {pybio.config.config_fname()}")
 print(f"[pybio] genomes folder: {pybio.config.genomes_folder}")
 print()
 
 if args.version:
     sys.exit(0)
 
 if len(args.commands)==0 and args.help:
```

### Comparing `pybio-0.3.8/pybio/sequence/__init__.py` & `pybio-0.3.9/pybio/sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio/utils/__init__.py` & `pybio-0.3.9/pybio/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/pybio.egg-info/PKG-INFO` & `pybio-0.3.9/pybio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: pybio
-Version: 0.3.8
+Version: 0.3.9
 Summary: pybio genomics
 Home-page: https://github.com/grexor/pybio
 Author: Gregor Rot
 Author-email: gregor.rot@gmail.com
 Keywords: pybio,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 ## pybio: basic genomics toolset
 
 pybio is a Python framework for handling genomics operations and a direct interface to Ensembl genomes.
 
-Downloading an Ensembl genome+annotation takes one line: `pybio genome homo_sapiens`.
+Downloading an Ensembl genome+annotation takes one line:
+
+`$ pybio genome homo_sapiens`
 
 Features include genome+annotation download from Ensembl and processing with STAR and salmon, support of Fasta, Fastq, bedGraph and other file formats, motif sequence searches, and specific APA feautes like alternative polyadenylation site-pair classification (same-exon, skipped-exon, composite-exon) and more.
 
 ## Contents
 
 * [Installation](#installation)
 * [Quick Start](#Quick-Start)
@@ -30,15 +32,17 @@
 * [Authors](#authors)
 * [Reporting problems](#reporting-problems)
 
 ### Installation
 
 The easiest way to install pybio is running:
 
-`pip install pybio`
+`$ pip install pybio`
+
+Note that on some systems, pip is installing the executable scripts under `~/.local/bin`. However this folder is not in the PATH which will result in `command not found` if you try to run `$ pybio` on the command line. To fix this, please execute `export PATH="$PATH:~/.local/bin"` (and add this to your `.profile`). Another suggestion is to install inside a virtual environment (using `virtualenv`).
 
 If you would like instead to install the latest developmental version from this repository:
 
 ```
 # clone pybio repository locally
 git clone https://github.com/grexor/pybio.git
```

### Comparing `pybio-0.3.8/pybio.egg-info/SOURCES.txt` & `pybio-0.3.9/pybio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybio-0.3.8/setup.py` & `pybio-0.3.9/setup.py`

 * *Files identical despite different names*

