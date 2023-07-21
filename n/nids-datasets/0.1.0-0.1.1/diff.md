# Comparing `tmp/nids_datasets-0.1.0.tar.gz` & `tmp/nids_datasets-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nids_datasets-0.1.0.tar", last modified: Fri Jul 21 03:11:20 2023, max compression
+gzip compressed data, was "nids_datasets-0.1.1.tar", last modified: Fri Jul 21 03:14:04 2023, max compression
```

## Comparing `nids_datasets-0.1.0.tar` & `nids_datasets-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-21 03:11:20.932677 nids_datasets-0.1.0/
--rw-r--r--   0 rdp        (501) staff       (20)     8014 2023-07-21 03:11:20.932434 nids_datasets-0.1.0/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)     7381 2023-07-21 03:07:57.000000 nids_datasets-0.1.0/README.md
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-21 03:11:20.931328 nids_datasets-0.1.0/nids_datasets/
--rw-r--r--   0 rdp        (501) staff       (20)       41 2023-07-17 06:28:22.000000 nids_datasets-0.1.0/nids_datasets/__init__.py
--rw-r--r--   0 rdp        (501) staff       (20)    12833 2023-07-21 01:00:33.000000 nids_datasets-0.1.0/nids_datasets/dataset.py
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-21 03:11:20.932226 nids_datasets-0.1.0/nids_datasets.egg-info/
--rw-r--r--   0 rdp        (501) staff       (20)     8014 2023-07-21 03:11:20.000000 nids_datasets-0.1.0/nids_datasets.egg-info/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)      253 2023-07-21 03:11:20.000000 nids_datasets-0.1.0/nids_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-21 03:11:20.000000 nids_datasets-0.1.0/nids_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 rdp        (501) staff       (20)       98 2023-07-21 03:11:20.000000 nids_datasets-0.1.0/nids_datasets.egg-info/requires.txt
--rw-r--r--   0 rdp        (501) staff       (20)       14 2023-07-21 03:11:20.000000 nids_datasets-0.1.0/nids_datasets.egg-info/top_level.txt
--rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-21 03:11:20.932730 nids_datasets-0.1.0/setup.cfg
--rw-r--r--   0 rdp        (501) staff       (20)     1006 2023-07-21 03:10:51.000000 nids_datasets-0.1.0/setup.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-21 03:14:04.891750 nids_datasets-0.1.1/
+-rw-r--r--   0 rdp        (501) staff       (20)     7961 2023-07-21 03:14:04.891322 nids_datasets-0.1.1/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)     7381 2023-07-21 03:12:59.000000 nids_datasets-0.1.1/README.md
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-21 03:14:04.889925 nids_datasets-0.1.1/nids_datasets/
+-rw-r--r--   0 rdp        (501) staff       (20)       41 2023-07-17 06:28:22.000000 nids_datasets-0.1.1/nids_datasets/__init__.py
+-rw-r--r--   0 rdp        (501) staff       (20)    12833 2023-07-21 01:00:33.000000 nids_datasets-0.1.1/nids_datasets/dataset.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-21 03:14:04.891004 nids_datasets-0.1.1/nids_datasets.egg-info/
+-rw-r--r--   0 rdp        (501) staff       (20)     7961 2023-07-21 03:14:04.000000 nids_datasets-0.1.1/nids_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)      253 2023-07-21 03:14:04.000000 nids_datasets-0.1.1/nids_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-21 03:14:04.000000 nids_datasets-0.1.1/nids_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       98 2023-07-21 03:14:04.000000 nids_datasets-0.1.1/nids_datasets.egg-info/requires.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       14 2023-07-21 03:14:04.000000 nids_datasets-0.1.1/nids_datasets.egg-info/top_level.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-21 03:14:04.891808 nids_datasets-0.1.1/setup.cfg
+-rw-r--r--   0 rdp        (501) staff       (20)      953 2023-07-21 03:13:49.000000 nids_datasets-0.1.1/setup.py
```

### Comparing `nids_datasets-0.1.0/PKG-INFO` & `nids_datasets-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nids_datasets
-Version: 0.1.0
-Summary: Download and utilize specially curated and extracted datasets from the original CIC-IDS2017 and UNSW-NB15 datasets for Network Intrusion Detection (NIDS)
+Version: 0.1.1
+Summary: Download and utilize specially curated and extracted datasets from the original CIC-IDS2017 datasets
 Home-page: https://github.com/rdpahalavan/nids-datasets
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: Apache License 2.0
 Keywords: Dataset NIDS UNSW-NB15 CIC-IDS2017
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 
 # NIDS Datasets
 
-The `nids-datasets` package provides functionality to download and utilize specially curated and extracted datasets from the original CIC-IDS2017 and UNSW-NB15 datasets. These datasets, which initially were only flow datasets, have been enhanced to include packet-level information from the raw PCAP files. The dataset contains both packet-level and flow-level data for over 230 million packets, with 179 million packets from UNSW-NB15 and 54 million packets from CIC-IDS2017.
+The `nids-datasets` package provides functionality to download and utilize specially curated and extracted datasets from the original UNSW-NB15 and CIC-IDS2017 datasets. These datasets, which initially were only flow datasets, have been enhanced to include packet-level information from the raw PCAP files. The dataset contains both packet-level and flow-level data for over 230 million packets, with 179 million packets from UNSW-NB15 and 54 million packets from CIC-IDS2017.
 
 ## Installation
 
 Install the `nids-datasets` package using pip:
 
 ```shell
 pip install nids-datasets
```

### Comparing `nids_datasets-0.1.0/README.md` & `nids_datasets-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # NIDS Datasets
 
-The `nids-datasets` package provides functionality to download and utilize specially curated and extracted datasets from the original CIC-IDS2017 and UNSW-NB15 datasets. These datasets, which initially were only flow datasets, have been enhanced to include packet-level information from the raw PCAP files. The dataset contains both packet-level and flow-level data for over 230 million packets, with 179 million packets from UNSW-NB15 and 54 million packets from CIC-IDS2017.
+The `nids-datasets` package provides functionality to download and utilize specially curated and extracted datasets from the original UNSW-NB15 and CIC-IDS2017 datasets. These datasets, which initially were only flow datasets, have been enhanced to include packet-level information from the raw PCAP files. The dataset contains both packet-level and flow-level data for over 230 million packets, with 179 million packets from UNSW-NB15 and 54 million packets from CIC-IDS2017.
 
 ## Installation
 
 Install the `nids-datasets` package using pip:
 
 ```shell
 pip install nids-datasets
```

### Comparing `nids_datasets-0.1.0/nids_datasets/dataset.py` & `nids_datasets-0.1.1/nids_datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `nids_datasets-0.1.0/nids_datasets.egg-info/PKG-INFO` & `nids_datasets-0.1.1/nids_datasets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nids-datasets
-Version: 0.1.0
-Summary: Download and utilize specially curated and extracted datasets from the original CIC-IDS2017 and UNSW-NB15 datasets for Network Intrusion Detection (NIDS)
+Version: 0.1.1
+Summary: Download and utilize specially curated and extracted datasets from the original CIC-IDS2017 datasets
 Home-page: https://github.com/rdpahalavan/nids-datasets
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: Apache License 2.0
 Keywords: Dataset NIDS UNSW-NB15 CIC-IDS2017
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 
 # NIDS Datasets
 
-The `nids-datasets` package provides functionality to download and utilize specially curated and extracted datasets from the original CIC-IDS2017 and UNSW-NB15 datasets. These datasets, which initially were only flow datasets, have been enhanced to include packet-level information from the raw PCAP files. The dataset contains both packet-level and flow-level data for over 230 million packets, with 179 million packets from UNSW-NB15 and 54 million packets from CIC-IDS2017.
+The `nids-datasets` package provides functionality to download and utilize specially curated and extracted datasets from the original UNSW-NB15 and CIC-IDS2017 datasets. These datasets, which initially were only flow datasets, have been enhanced to include packet-level information from the raw PCAP files. The dataset contains both packet-level and flow-level data for over 230 million packets, with 179 million packets from UNSW-NB15 and 54 million packets from CIC-IDS2017.
 
 ## Installation
 
 Install the `nids-datasets` package using pip:
 
 ```shell
 pip install nids-datasets
```

### Comparing `nids_datasets-0.1.0/setup.py` & `nids_datasets-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='nids_datasets',
-    version='0.1.0',
-    description="Download and utilize specially curated and extracted datasets from the original CIC-IDS2017 and UNSW-NB15 datasets for Network Intrusion Detection (NIDS)",
+    version='0.1.1',
+    description="Download and utilize specially curated and extracted datasets from the original CIC-IDS2017 datasets",
     keywords="Dataset NIDS UNSW-NB15 CIC-IDS2017",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     author="Pahalavan R D",
     author_email='rdpahalavan24@gmail.com',
     packages=['nids_datasets'],
```

