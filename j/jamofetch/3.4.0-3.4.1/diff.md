# Comparing `tmp/jamofetch-3.4.0.tar.gz` & `tmp/jamofetch-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jamofetch-3.4.0.tar", max compression
+gzip compressed data, was "jamofetch-3.4.1.tar", max compression
```

## Comparing `jamofetch-3.4.0.tar` & `jamofetch-3.4.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4990 2023-07-18 02:59:06.097074 jamofetch-3.4.0/README.md
--rw-r--r--   0        0        0      522 2023-07-18 02:31:30.964121 jamofetch-3.4.0/pyproject.toml
--rw-r--r--   0        0        0      111 2023-07-07 23:08:25.647260 jamofetch-3.4.0/src/jamofetch/__init__.py
--rwxr-xr-x   0        0        0    10838 2023-07-18 02:30:40.133609 jamofetch-3.4.0/src/jamofetch/jamofetch.py
--rw-r--r--   0        0        0     5519 1970-01-01 00:00:00.000000 jamofetch-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4728 2023-07-21 01:16:33.706667 jamofetch-3.4.1/README.md
+-rw-r--r--   0        0        0      522 2023-07-21 01:14:48.920470 jamofetch-3.4.1/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-07-07 23:08:25.647260 jamofetch-3.4.1/src/jamofetch/__init__.py
+-rwxr-xr-x   0        0        0    10838 2023-07-18 02:30:40.133609 jamofetch-3.4.1/src/jamofetch/jamofetch.py
+-rw-r--r--   0        0        0     5257 1970-01-01 00:00:00.000000 jamofetch-3.4.1/PKG-INFO
```

### Comparing `jamofetch-3.4.0/README.md` & `jamofetch-3.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,18 @@
 # jamofetch
 thin wrapper on JAMO to allow sequence retrieval on Dori and at NERSC
 
 ## Installation
 Jamofetch requires python 3.8 or higher.
 
-### Adding via requirements.txt
-Include the following two lines in the requirements.txt of your project:
-```python
-jamofetch==3.4.0
---extra-index-url https://code.jgi.doe.gov/api/v4/projects/479/packages/pypi/simple
-```
-### Manual installation
-First option:
+Jamofetch is available on PyPi: https://pypi.org/project/jamofetch/.
 ```bash
-$ pip install jamofetch --index-url https://code.jgi.doe.gov/api/v4/projects/479/packages/pypi/simple
-```
-Second option:
-```bash
-$ pip install git+https://code.jgi.doe.gov/DNScott/jamofetch
+$ pip install jamofetch
 ```
+
 ## Usage
 See script **docs/demo_script.py** in the project for a sample script.
 
 Create a JamoFetcher:
 ```pthon
 from jamofetch.jamofetch import JamoFetcher, JamoLibSeq
 
@@ -101,10 +91,11 @@
 NPUNN realpath: /clusterfs/jgi/scratch/dsi/aa/dm_archive/sdm/pacbio/00/27/47/pbio-2747.27352.bc1001_BAK8A_OA--bc1001_BAK8A_OA.ccs.fastq.gz
 
 waiting for JAMO to provision sequence . . . .
 NOOHG sequence ready
 NPUNN sequence ready
 ```
 ## Credits
+Jamofetch uses Will Holtz's doejgi/jamo-dori Docker image to call JAMO on the Dori cluster.
 
 `jamofetch` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).
```

### Comparing `jamofetch-3.4.0/pyproject.toml` & `jamofetch-3.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jamofetch"
-version = "3.4.0"
+version = "3.4.1"
 description = "A thin wrapper to retrieve sequence from JAMO at NERSC and on Dori."
 authors = ["Duncan Scott"]
 license = "None"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
```

### Comparing `jamofetch-3.4.0/src/jamofetch/jamofetch.py` & `jamofetch-3.4.1/src/jamofetch/jamofetch.py`

 * *Files identical despite different names*

### Comparing `jamofetch-3.4.0/PKG-INFO` & `jamofetch-3.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jamofetch
-Version: 3.4.0
+Version: 3.4.1
 Summary: A thin wrapper to retrieve sequence from JAMO at NERSC and on Dori.
 License: None
 Author: Duncan Scott
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -15,29 +15,19 @@
 
 # jamofetch
 thin wrapper on JAMO to allow sequence retrieval on Dori and at NERSC
 
 ## Installation
 Jamofetch requires python 3.8 or higher.
 
-### Adding via requirements.txt
-Include the following two lines in the requirements.txt of your project:
-```python
-jamofetch==3.4.0
---extra-index-url https://code.jgi.doe.gov/api/v4/projects/479/packages/pypi/simple
-```
-### Manual installation
-First option:
+Jamofetch is available on PyPi: https://pypi.org/project/jamofetch/.
 ```bash
-$ pip install jamofetch --index-url https://code.jgi.doe.gov/api/v4/projects/479/packages/pypi/simple
-```
-Second option:
-```bash
-$ pip install git+https://code.jgi.doe.gov/DNScott/jamofetch
+$ pip install jamofetch
 ```
+
 ## Usage
 See script **docs/demo_script.py** in the project for a sample script.
 
 Create a JamoFetcher:
 ```pthon
 from jamofetch.jamofetch import JamoFetcher, JamoLibSeq
 
@@ -116,11 +106,12 @@
 NPUNN realpath: /clusterfs/jgi/scratch/dsi/aa/dm_archive/sdm/pacbio/00/27/47/pbio-2747.27352.bc1001_BAK8A_OA--bc1001_BAK8A_OA.ccs.fastq.gz
 
 waiting for JAMO to provision sequence . . . .
 NOOHG sequence ready
 NPUNN sequence ready
 ```
 ## Credits
+Jamofetch uses Will Holtz's doejgi/jamo-dori Docker image to call JAMO on the Dori cluster.
 
 `jamofetch` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).
```

