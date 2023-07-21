# Comparing `tmp/nids_datasets-0.1.2.tar.gz` & `tmp/nids_datasets-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nids_datasets-0.1.2.tar", last modified: Fri Jul 21 03:15:59 2023, max compression
+gzip compressed data, was "nids_datasets-0.1.3.tar", last modified: Fri Jul 21 03:51:26 2023, max compression
```

## Comparing `nids_datasets-0.1.2.tar` & `nids_datasets-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-21 03:15:59.755012 nids_datasets-0.1.2/
--rw-r--r--   0 rdp        (501) staff       (20)     7975 2023-07-21 03:15:59.754770 nids_datasets-0.1.2/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)     7381 2023-07-21 03:12:59.000000 nids_datasets-0.1.2/README.md
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-21 03:15:59.753669 nids_datasets-0.1.2/nids_datasets/
--rw-r--r--   0 rdp        (501) staff       (20)       41 2023-07-17 06:28:22.000000 nids_datasets-0.1.2/nids_datasets/__init__.py
--rw-r--r--   0 rdp        (501) staff       (20)    12833 2023-07-21 01:00:33.000000 nids_datasets-0.1.2/nids_datasets/dataset.py
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-21 03:15:59.754542 nids_datasets-0.1.2/nids_datasets.egg-info/
--rw-r--r--   0 rdp        (501) staff       (20)     7975 2023-07-21 03:15:59.000000 nids_datasets-0.1.2/nids_datasets.egg-info/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)      253 2023-07-21 03:15:59.000000 nids_datasets-0.1.2/nids_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-21 03:15:59.000000 nids_datasets-0.1.2/nids_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 rdp        (501) staff       (20)       98 2023-07-21 03:15:59.000000 nids_datasets-0.1.2/nids_datasets.egg-info/requires.txt
--rw-r--r--   0 rdp        (501) staff       (20)       14 2023-07-21 03:15:59.000000 nids_datasets-0.1.2/nids_datasets.egg-info/top_level.txt
--rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-21 03:15:59.755065 nids_datasets-0.1.2/setup.cfg
--rw-r--r--   0 rdp        (501) staff       (20)      967 2023-07-21 03:15:52.000000 nids_datasets-0.1.2/setup.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-21 03:51:26.465011 nids_datasets-0.1.3/
+-rw-r--r--   0 rdp        (501) staff       (20)     8083 2023-07-21 03:51:26.464767 nids_datasets-0.1.3/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)     7489 2023-07-21 03:51:07.000000 nids_datasets-0.1.3/README.md
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-21 03:51:26.463674 nids_datasets-0.1.3/nids_datasets/
+-rw-r--r--   0 rdp        (501) staff       (20)       41 2023-07-17 06:28:22.000000 nids_datasets-0.1.3/nids_datasets/__init__.py
+-rw-r--r--   0 rdp        (501) staff       (20)    12833 2023-07-21 01:00:33.000000 nids_datasets-0.1.3/nids_datasets/dataset.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-21 03:51:26.464555 nids_datasets-0.1.3/nids_datasets.egg-info/
+-rw-r--r--   0 rdp        (501) staff       (20)     8083 2023-07-21 03:51:26.000000 nids_datasets-0.1.3/nids_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)      253 2023-07-21 03:51:26.000000 nids_datasets-0.1.3/nids_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-21 03:51:26.000000 nids_datasets-0.1.3/nids_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       98 2023-07-21 03:51:26.000000 nids_datasets-0.1.3/nids_datasets.egg-info/requires.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       14 2023-07-21 03:51:26.000000 nids_datasets-0.1.3/nids_datasets.egg-info/top_level.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-21 03:51:26.465061 nids_datasets-0.1.3/setup.cfg
+-rw-r--r--   0 rdp        (501) staff       (20)      967 2023-07-21 03:51:14.000000 nids_datasets-0.1.3/setup.py
```

### Comparing `nids_datasets-0.1.2/PKG-INFO` & `nids_datasets-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nids_datasets
-Version: 0.1.2
+Version: 0.1.3
 Summary: Download and utilize specially curated and extracted datasets from the original UNSW-NB15 and CIC-IDS2017 datasets
 Home-page: https://github.com/rdpahalavan/nids-datasets
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: Apache License 2.0
 Keywords: Dataset NIDS UNSW-NB15 CIC-IDS2017
 Classifier: Programming Language :: Python :: 3
@@ -29,15 +29,15 @@
 
 ```python
 from nids_datasets import Dataset, DatasetInfo
 ```
 
 ## Dataset Information
 
-The `nids-datasets` package currently supports two datasets: UNSW-NB15 and CIC-IDS2017. Each of these datasets contains a mix of normal traffic and different types of attack traffic, which are identified by their respective labels. The UNSW-NB15 dataset has 10 unique class labels, and the CIC-IDS2017 dataset has 24 unique class labels. 
+The `nids-datasets` package currently supports two datasets: [UNSW-NB15](https://research.unsw.edu.au/projects/unsw-nb15-dataset) and [CIC-IDS2017](https://www.unb.ca/cic/datasets/ids-2017.html). Each of these datasets contains a mix of normal traffic and different types of attack traffic, which are identified by their respective labels. The UNSW-NB15 dataset has 10 unique class labels, and the CIC-IDS2017 dataset has 24 unique class labels. 
 
 - UNSW-NB15 Labels: 'normal', 'exploits', 'dos', 'fuzzers', 'generic', 'reconnaissance', 'worms', 'shellcode', 'backdoor', 'analysis'
 - CIC-IDS2017 Labels: 'BENIGN', 'FTP-Patator', 'SSH-Patator', 'DoS slowloris', 'DoS Slowhttptest', 'DoS Hulk', 'Heartbleed', 'Web Attack – Brute Force', 'Web Attack – XSS', 'Web Attack – SQL Injection', 'Infiltration', 'Bot', 'PortScan', 'DDoS', 'normal', 'exploits', 'dos', 'fuzzers', 'generic', 'reconnaissance', 'worms', 'shellcode', 'backdoor', 'analysis', 'DoS GoldenEye'
 
 ## Subsets of the Dataset
 
 Each dataset consists of four subsets:
```

### Comparing `nids_datasets-0.1.2/README.md` & `nids_datasets-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ```python
 from nids_datasets import Dataset, DatasetInfo
 ```
 
 ## Dataset Information
 
-The `nids-datasets` package currently supports two datasets: UNSW-NB15 and CIC-IDS2017. Each of these datasets contains a mix of normal traffic and different types of attack traffic, which are identified by their respective labels. The UNSW-NB15 dataset has 10 unique class labels, and the CIC-IDS2017 dataset has 24 unique class labels. 
+The `nids-datasets` package currently supports two datasets: [UNSW-NB15](https://research.unsw.edu.au/projects/unsw-nb15-dataset) and [CIC-IDS2017](https://www.unb.ca/cic/datasets/ids-2017.html). Each of these datasets contains a mix of normal traffic and different types of attack traffic, which are identified by their respective labels. The UNSW-NB15 dataset has 10 unique class labels, and the CIC-IDS2017 dataset has 24 unique class labels. 
 
 - UNSW-NB15 Labels: 'normal', 'exploits', 'dos', 'fuzzers', 'generic', 'reconnaissance', 'worms', 'shellcode', 'backdoor', 'analysis'
 - CIC-IDS2017 Labels: 'BENIGN', 'FTP-Patator', 'SSH-Patator', 'DoS slowloris', 'DoS Slowhttptest', 'DoS Hulk', 'Heartbleed', 'Web Attack – Brute Force', 'Web Attack – XSS', 'Web Attack – SQL Injection', 'Infiltration', 'Bot', 'PortScan', 'DDoS', 'normal', 'exploits', 'dos', 'fuzzers', 'generic', 'reconnaissance', 'worms', 'shellcode', 'backdoor', 'analysis', 'DoS GoldenEye'
 
 ## Subsets of the Dataset
 
 Each dataset consists of four subsets:
```

### Comparing `nids_datasets-0.1.2/nids_datasets/dataset.py` & `nids_datasets-0.1.3/nids_datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `nids_datasets-0.1.2/nids_datasets.egg-info/PKG-INFO` & `nids_datasets-0.1.3/nids_datasets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nids-datasets
-Version: 0.1.2
+Version: 0.1.3
 Summary: Download and utilize specially curated and extracted datasets from the original UNSW-NB15 and CIC-IDS2017 datasets
 Home-page: https://github.com/rdpahalavan/nids-datasets
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: Apache License 2.0
 Keywords: Dataset NIDS UNSW-NB15 CIC-IDS2017
 Classifier: Programming Language :: Python :: 3
@@ -29,15 +29,15 @@
 
 ```python
 from nids_datasets import Dataset, DatasetInfo
 ```
 
 ## Dataset Information
 
-The `nids-datasets` package currently supports two datasets: UNSW-NB15 and CIC-IDS2017. Each of these datasets contains a mix of normal traffic and different types of attack traffic, which are identified by their respective labels. The UNSW-NB15 dataset has 10 unique class labels, and the CIC-IDS2017 dataset has 24 unique class labels. 
+The `nids-datasets` package currently supports two datasets: [UNSW-NB15](https://research.unsw.edu.au/projects/unsw-nb15-dataset) and [CIC-IDS2017](https://www.unb.ca/cic/datasets/ids-2017.html). Each of these datasets contains a mix of normal traffic and different types of attack traffic, which are identified by their respective labels. The UNSW-NB15 dataset has 10 unique class labels, and the CIC-IDS2017 dataset has 24 unique class labels. 
 
 - UNSW-NB15 Labels: 'normal', 'exploits', 'dos', 'fuzzers', 'generic', 'reconnaissance', 'worms', 'shellcode', 'backdoor', 'analysis'
 - CIC-IDS2017 Labels: 'BENIGN', 'FTP-Patator', 'SSH-Patator', 'DoS slowloris', 'DoS Slowhttptest', 'DoS Hulk', 'Heartbleed', 'Web Attack – Brute Force', 'Web Attack – XSS', 'Web Attack – SQL Injection', 'Infiltration', 'Bot', 'PortScan', 'DDoS', 'normal', 'exploits', 'dos', 'fuzzers', 'generic', 'reconnaissance', 'worms', 'shellcode', 'backdoor', 'analysis', 'DoS GoldenEye'
 
 ## Subsets of the Dataset
 
 Each dataset consists of four subsets:
```

### Comparing `nids_datasets-0.1.2/setup.py` & `nids_datasets-0.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='nids_datasets',
-    version='0.1.2',
+    version='0.1.3',
     description="Download and utilize specially curated and extracted datasets from the original UNSW-NB15 and CIC-IDS2017 datasets",
     keywords="Dataset NIDS UNSW-NB15 CIC-IDS2017",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     author="Pahalavan R D",
     author_email='rdpahalavan24@gmail.com',
```

