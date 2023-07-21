# Comparing `tmp/stereosite-1.0.3.tar.gz` & `tmp/stereosite-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stereosite-1.0.3.tar", last modified: Thu Jul 20 07:28:08 2023, max compression
+gzip compressed data, was "dist/stereosite-1.0.4.tar", last modified: Fri Jul 21 02:24:08 2023, max compression
```

## Comparing `stereosite-1.0.3.tar` & `stereosite-1.0.4.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-20 07:28:08.000000 stereosite-1.0.3/
--rw-r--r--   0 liuxing    (501) staff       (20)      236 2023-07-20 03:14:46.000000 stereosite-1.0.3/.gitignore
--rw-r--r--   0 liuxing    (501) staff       (20)     1064 2023-07-17 05:57:26.000000 stereosite-1.0.3/LICENSE
--rw-r--r--   0 liuxing    (501) staff       (20)     1683 2023-07-20 07:28:08.000000 stereosite-1.0.3/PKG-INFO
--rw-r--r--   0 liuxing    (501) staff       (20)     4950 2023-07-20 07:03:43.000000 stereosite-1.0.3/README.rst
--rw-r--r--   0 liuxing    (501) staff       (20)       38 2023-07-20 07:28:08.000000 stereosite-1.0.3/setup.cfg
--rw-r--r--   0 liuxing    (501) staff       (20)      703 2023-07-20 07:19:49.000000 stereosite-1.0.3/setup.py
-drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-20 07:28:08.000000 stereosite-1.0.3/stereosite/
--rw-r--r--   0 liuxing    (501) staff       (20)        0 2023-07-11 10:28:46.000000 stereosite-1.0.3/stereosite/__init__.py
-drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-20 07:28:08.000000 stereosite-1.0.3/stereosite/cn/
--rw-r--r--   0 liuxing    (501) staff       (20)       45 2023-07-18 07:12:27.000000 stereosite-1.0.3/stereosite/cn/__init__.py
--rw-r--r--   0 liuxing    (501) staff       (20)     8212 2023-07-19 03:31:03.000000 stereosite-1.0.3/stereosite/cn/cellneighbor.py
--rw-r--r--   0 liuxing    (501) staff       (20)    16966 2023-07-18 07:46:36.000000 stereosite-1.0.3/stereosite/cn/deconvolution.py
-drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-20 07:28:08.000000 stereosite-1.0.3/stereosite/datasets/
-drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-20 07:28:08.000000 stereosite-1.0.3/stereosite/datasets/LR_database/
--rw-r--r--   0 liuxing    (501) staff       (20)   251825 2023-07-12 02:43:39.000000 stereosite-1.0.3/stereosite/datasets/LR_database/CellChatDB.human.csv
--rw-r--r--   0 liuxing    (501) staff       (20)   262735 2023-07-12 02:44:06.000000 stereosite-1.0.3/stereosite/datasets/LR_database/CellChatDB.mouse.csv
--rw-r--r--   0 liuxing    (501) staff       (20)  5181168 2022-11-23 08:38:59.000000 stereosite-1.0.3/stereosite/datasets/LR_database/cellphoneDB_interactions.csv
--rw-r--r--   0 liuxing    (501) staff       (20) 40854370 2023-02-22 01:27:09.000000 stereosite-1.0.3/stereosite/datasets/LR_database/interactions.csv
-drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-20 07:28:08.000000 stereosite-1.0.3/stereosite/datasets/biomart/
--rw-r--r--   0 liuxing    (501) staff       (20)  2499142 2023-07-12 02:40:34.000000 stereosite-1.0.3/stereosite/datasets/biomart/human_to_mouse_biomart_export.csv
--rw-r--r--   0 liuxing    (501) staff       (20)  2387385 2023-07-12 02:40:39.000000 stereosite-1.0.3/stereosite/datasets/biomart/mouse_to_human_biomart_export.csv
-drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-20 07:28:08.000000 stereosite-1.0.3/stereosite/plot/
--rw-r--r--   0 liuxing    (501) staff       (20)       44 2023-07-11 10:23:47.000000 stereosite-1.0.3/stereosite/plot/__init__.py
--rw-r--r--   0 liuxing    (501) staff       (20)     2405 2023-07-18 09:43:28.000000 stereosite-1.0.3/stereosite/plot/cellneighbor.py
--rw-r--r--   0 liuxing    (501) staff       (20)     6648 2023-07-19 01:52:33.000000 stereosite-1.0.3/stereosite/plot/intensity.py
--rw-r--r--   0 liuxing    (501) staff       (20)     3722 2023-07-12 02:26:36.000000 stereosite-1.0.3/stereosite/plot/mask.py
--rw-r--r--   0 liuxing    (501) staff       (20)    17982 2023-07-12 08:48:10.000000 stereosite-1.0.3/stereosite/plot/scii.py
-drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-20 07:28:08.000000 stereosite-1.0.3/stereosite/read/
--rw-r--r--   0 liuxing    (501) staff       (20)       46 2023-07-11 10:23:38.000000 stereosite-1.0.3/stereosite/read/__init__.py
--rw-r--r--   0 liuxing    (501) staff       (20)     6645 2023-07-18 06:52:32.000000 stereosite-1.0.3/stereosite/read/gem.py
--rw-r--r--   0 liuxing    (501) staff       (20)    19738 2023-07-18 09:36:55.000000 stereosite-1.0.3/stereosite/scii.py
-drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-20 07:28:08.000000 stereosite-1.0.3/stereosite.egg-info/
--rw-r--r--   0 liuxing    (501) staff       (20)     1683 2023-07-20 07:28:08.000000 stereosite-1.0.3/stereosite.egg-info/PKG-INFO
--rw-r--r--   0 liuxing    (501) staff       (20)      933 2023-07-20 07:28:08.000000 stereosite-1.0.3/stereosite.egg-info/SOURCES.txt
--rw-r--r--   0 liuxing    (501) staff       (20)        1 2023-07-20 07:28:08.000000 stereosite-1.0.3/stereosite.egg-info/dependency_links.txt
--rw-r--r--   0 liuxing    (501) staff       (20)       44 2023-07-20 07:28:08.000000 stereosite-1.0.3/stereosite.egg-info/requires.txt
--rw-r--r--   0 liuxing    (501) staff       (20)       11 2023-07-20 07:28:08.000000 stereosite-1.0.3/stereosite.egg-info/top_level.txt
-drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-20 07:28:08.000000 stereosite-1.0.3/tests/
--rw-r--r--   0 liuxing    (501) staff       (20)   710400 2023-07-20 07:12:39.000000 stereosite-1.0.3/tests/code_test.ipynb
--rw-r--r--   0 liuxing    (501) staff       (20)  1769695 2023-07-20 02:59:40.000000 stereosite-1.0.3/tests/inf_aver_noCAF.csv
--rw-r--r--   0 liuxing    (501) staff       (20)   911784 2023-07-20 02:59:40.000000 stereosite-1.0.3/tests/test_adata.h5ad
+drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-21 02:24:08.000000 stereosite-1.0.4/
+-rw-r--r--   0 liuxing    (501) staff       (20)      236 2023-07-20 03:14:46.000000 stereosite-1.0.4/.gitignore
+-rw-r--r--   0 liuxing    (501) staff       (20)     1064 2023-07-17 05:57:26.000000 stereosite-1.0.4/LICENSE
+-rw-r--r--   0 liuxing    (501) staff       (20)     1683 2023-07-21 02:24:08.000000 stereosite-1.0.4/PKG-INFO
+-rw-r--r--   0 liuxing    (501) staff       (20)     1377 2023-07-20 07:27:43.000000 stereosite-1.0.4/PYPI.rst
+-rw-r--r--   0 liuxing    (501) staff       (20)     4950 2023-07-20 07:03:43.000000 stereosite-1.0.4/README.rst
+-rw-r--r--   0 liuxing    (501) staff       (20)       38 2023-07-21 02:24:08.000000 stereosite-1.0.4/setup.cfg
+-rw-r--r--   0 liuxing    (501) staff       (20)      703 2023-07-21 02:24:01.000000 stereosite-1.0.4/setup.py
+drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-21 02:24:08.000000 stereosite-1.0.4/stereosite/
+-rw-r--r--   0 liuxing    (501) staff       (20)        0 2023-07-11 10:28:46.000000 stereosite-1.0.4/stereosite/__init__.py
+drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-21 02:24:08.000000 stereosite-1.0.4/stereosite/cn/
+-rw-r--r--   0 liuxing    (501) staff       (20)       45 2023-07-18 07:12:27.000000 stereosite-1.0.4/stereosite/cn/__init__.py
+-rw-r--r--   0 liuxing    (501) staff       (20)     8212 2023-07-19 03:31:03.000000 stereosite-1.0.4/stereosite/cn/cellneighbor.py
+-rw-r--r--   0 liuxing    (501) staff       (20)    16966 2023-07-18 07:46:36.000000 stereosite-1.0.4/stereosite/cn/deconvolution.py
+drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-21 02:24:08.000000 stereosite-1.0.4/stereosite/datasets/
+drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-21 02:24:08.000000 stereosite-1.0.4/stereosite/datasets/LR_database/
+-rw-r--r--   0 liuxing    (501) staff       (20)   251825 2023-07-12 02:43:39.000000 stereosite-1.0.4/stereosite/datasets/LR_database/CellChatDB.human.csv
+-rw-r--r--   0 liuxing    (501) staff       (20)   262735 2023-07-12 02:44:06.000000 stereosite-1.0.4/stereosite/datasets/LR_database/CellChatDB.mouse.csv
+-rw-r--r--   0 liuxing    (501) staff       (20)  5181168 2022-11-23 08:38:59.000000 stereosite-1.0.4/stereosite/datasets/LR_database/cellphoneDB_interactions.csv
+-rw-r--r--   0 liuxing    (501) staff       (20) 40854370 2023-02-22 01:27:09.000000 stereosite-1.0.4/stereosite/datasets/LR_database/interactions.csv
+drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-21 02:24:08.000000 stereosite-1.0.4/stereosite/datasets/biomart/
+-rw-r--r--   0 liuxing    (501) staff       (20)  2499142 2023-07-12 02:40:34.000000 stereosite-1.0.4/stereosite/datasets/biomart/human_to_mouse_biomart_export.csv
+-rw-r--r--   0 liuxing    (501) staff       (20)  2387385 2023-07-12 02:40:39.000000 stereosite-1.0.4/stereosite/datasets/biomart/mouse_to_human_biomart_export.csv
+drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-21 02:24:08.000000 stereosite-1.0.4/stereosite/plot/
+-rw-r--r--   0 liuxing    (501) staff       (20)       44 2023-07-11 10:23:47.000000 stereosite-1.0.4/stereosite/plot/__init__.py
+-rw-r--r--   0 liuxing    (501) staff       (20)     2405 2023-07-18 09:43:28.000000 stereosite-1.0.4/stereosite/plot/cellneighbor.py
+-rw-r--r--   0 liuxing    (501) staff       (20)     6648 2023-07-19 01:52:33.000000 stereosite-1.0.4/stereosite/plot/intensity.py
+-rw-r--r--   0 liuxing    (501) staff       (20)     3722 2023-07-12 02:26:36.000000 stereosite-1.0.4/stereosite/plot/mask.py
+-rw-r--r--   0 liuxing    (501) staff       (20)    17982 2023-07-12 08:48:10.000000 stereosite-1.0.4/stereosite/plot/scii.py
+drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-21 02:24:08.000000 stereosite-1.0.4/stereosite/read/
+-rw-r--r--   0 liuxing    (501) staff       (20)       46 2023-07-11 10:23:38.000000 stereosite-1.0.4/stereosite/read/__init__.py
+-rw-r--r--   0 liuxing    (501) staff       (20)     6645 2023-07-18 06:52:32.000000 stereosite-1.0.4/stereosite/read/gem.py
+-rw-r--r--   0 liuxing    (501) staff       (20)    19738 2023-07-18 09:36:55.000000 stereosite-1.0.4/stereosite/scii.py
+drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-21 02:24:08.000000 stereosite-1.0.4/stereosite.egg-info/
+-rw-r--r--   0 liuxing    (501) staff       (20)     1683 2023-07-21 02:24:08.000000 stereosite-1.0.4/stereosite.egg-info/PKG-INFO
+-rw-r--r--   0 liuxing    (501) staff       (20)      942 2023-07-21 02:24:08.000000 stereosite-1.0.4/stereosite.egg-info/SOURCES.txt
+-rw-r--r--   0 liuxing    (501) staff       (20)        1 2023-07-21 02:24:08.000000 stereosite-1.0.4/stereosite.egg-info/dependency_links.txt
+-rw-r--r--   0 liuxing    (501) staff       (20)       44 2023-07-21 02:24:08.000000 stereosite-1.0.4/stereosite.egg-info/requires.txt
+-rw-r--r--   0 liuxing    (501) staff       (20)       11 2023-07-21 02:24:08.000000 stereosite-1.0.4/stereosite.egg-info/top_level.txt
+drwxr-xr-x   0 liuxing    (501) staff       (20)        0 2023-07-21 02:24:08.000000 stereosite-1.0.4/tests/
+-rw-r--r--   0 liuxing    (501) staff       (20)   710400 2023-07-20 07:12:39.000000 stereosite-1.0.4/tests/code_test.ipynb
+-rw-r--r--   0 liuxing    (501) staff       (20)  1769695 2023-07-20 02:59:40.000000 stereosite-1.0.4/tests/inf_aver_noCAF.csv
+-rw-r--r--   0 liuxing    (501) staff       (20)   911784 2023-07-20 02:59:40.000000 stereosite-1.0.4/tests/test_adata.h5ad
```

### Comparing `stereosite-1.0.3/LICENSE` & `stereosite-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stereosite-1.0.3/PKG-INFO` & `stereosite-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stereosite
-Version: 1.0.3
+Version: 1.0.4
 Summary: Analysis spatial transcriptomics data
 Home-page: https://github.com/STOmics/StereoSiTE
 Author: LiuXing
 Author-email: liuxing2@genomics.cn
 License: MIT License
 Keywords: spatial cell interaction intensity
 Platform: any
```

### Comparing `stereosite-1.0.3/README.rst` & `stereosite-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `stereosite-1.0.3/setup.py` & `stereosite-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from  setuptools import setup, find_packages
 
 with open("PYPI.rst", "r") as f:
     long_description = f.read()
 
 setup(
     name='stereosite',
-    version='1.0.3',
+    version='1.0.4',
     author='LiuXing',
     author_email='liuxing2@genomics.cn',
     description=('Analysis spatial transcriptomics data'),
     long_description=long_description,
     license='MIT License',
     keywords='spatial cell interaction intensity',
     url="https://github.com/STOmics/StereoSiTE",
```

### Comparing `stereosite-1.0.3/stereosite/cn/cellneighbor.py` & `stereosite-1.0.4/stereosite/cn/cellneighbor.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.0.3/stereosite/cn/deconvolution.py` & `stereosite-1.0.4/stereosite/cn/deconvolution.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.0.3/stereosite/datasets/LR_database/CellChatDB.human.csv` & `stereosite-1.0.4/stereosite/datasets/LR_database/CellChatDB.human.csv`

 * *Files identical despite different names*

### Comparing `stereosite-1.0.3/stereosite/datasets/LR_database/CellChatDB.mouse.csv` & `stereosite-1.0.4/stereosite/datasets/LR_database/CellChatDB.mouse.csv`

 * *Files identical despite different names*

### Comparing `stereosite-1.0.3/stereosite/datasets/LR_database/cellphoneDB_interactions.csv` & `stereosite-1.0.4/stereosite/datasets/LR_database/cellphoneDB_interactions.csv`

 * *Files identical despite different names*

### Comparing `stereosite-1.0.3/stereosite/datasets/LR_database/interactions.csv` & `stereosite-1.0.4/stereosite/datasets/LR_database/interactions.csv`

 * *Files identical despite different names*

### Comparing `stereosite-1.0.3/stereosite/datasets/biomart/human_to_mouse_biomart_export.csv` & `stereosite-1.0.4/stereosite/datasets/biomart/human_to_mouse_biomart_export.csv`

 * *Files identical despite different names*

### Comparing `stereosite-1.0.3/stereosite/datasets/biomart/mouse_to_human_biomart_export.csv` & `stereosite-1.0.4/stereosite/datasets/biomart/mouse_to_human_biomart_export.csv`

 * *Files identical despite different names*

### Comparing `stereosite-1.0.3/stereosite/plot/cellneighbor.py` & `stereosite-1.0.4/stereosite/plot/cellneighbor.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.0.3/stereosite/plot/intensity.py` & `stereosite-1.0.4/stereosite/plot/intensity.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.0.3/stereosite/plot/mask.py` & `stereosite-1.0.4/stereosite/plot/mask.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.0.3/stereosite/plot/scii.py` & `stereosite-1.0.4/stereosite/plot/scii.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.0.3/stereosite/read/gem.py` & `stereosite-1.0.4/stereosite/read/gem.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.0.3/stereosite/scii.py` & `stereosite-1.0.4/stereosite/scii.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.0.3/stereosite.egg-info/PKG-INFO` & `stereosite-1.0.4/stereosite.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stereosite
-Version: 1.0.3
+Version: 1.0.4
 Summary: Analysis spatial transcriptomics data
 Home-page: https://github.com/STOmics/StereoSiTE
 Author: LiuXing
 Author-email: liuxing2@genomics.cn
 License: MIT License
 Keywords: spatial cell interaction intensity
 Platform: any
```

### Comparing `stereosite-1.0.3/stereosite.egg-info/SOURCES.txt` & `stereosite-1.0.4/stereosite.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 LICENSE
+PYPI.rst
 README.rst
 setup.py
 stereosite/__init__.py
 stereosite/scii.py
 stereosite.egg-info/PKG-INFO
 stereosite.egg-info/SOURCES.txt
 stereosite.egg-info/dependency_links.txt
```

### Comparing `stereosite-1.0.3/tests/code_test.ipynb` & `stereosite-1.0.4/tests/code_test.ipynb`

 * *Files identical despite different names*

### Comparing `stereosite-1.0.3/tests/inf_aver_noCAF.csv` & `stereosite-1.0.4/tests/inf_aver_noCAF.csv`

 * *Files identical despite different names*

### Comparing `stereosite-1.0.3/tests/test_adata.h5ad` & `stereosite-1.0.4/tests/test_adata.h5ad`

 * *Files identical despite different names*

