# Comparing `tmp/smatchpp-1.0.1.tar.gz` & `tmp/smatchpp-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smatchpp-1.0.1.tar", last modified: Fri Jul 21 07:44:27 2023, max compression
+gzip compressed data, was "smatchpp-1.0.2.tar", last modified: Fri Jul 21 07:50:21 2023, max compression
```

## Comparing `smatchpp-1.0.1.tar` & `smatchpp-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-21 07:44:27.326858 smatchpp-1.0.1/
--rw-rw-r--   0 user      (1000) user      (1000)    35149 2023-05-03 15:50:47.000000 smatchpp-1.0.1/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     8510 2023-07-21 07:44:27.326858 smatchpp-1.0.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     8112 2023-07-21 07:40:41.000000 smatchpp-1.0.1/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-21 07:44:27.326858 smatchpp-1.0.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      720 2023-07-21 07:44:22.000000 smatchpp-1.0.1/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-21 07:44:27.322858 smatchpp-1.0.1/smatchpp/
--rw-rw-r--   0 user      (1000) user      (1000)       32 2023-06-01 06:25:22.000000 smatchpp-1.0.1/smatchpp/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     7585 2023-06-01 07:10:33.000000 smatchpp-1.0.1/smatchpp/__main__.py
--rw-rw-r--   0 user      (1000) user      (1000)     5208 2023-07-17 07:11:06.000000 smatchpp-1.0.1/smatchpp/align.py
--rw-rw-r--   0 user      (1000) user      (1000)     6605 2023-07-17 07:04:27.000000 smatchpp-1.0.1/smatchpp/bindings.py
--rw-rw-r--   0 user      (1000) user      (1000)     8925 2023-07-18 09:38:55.000000 smatchpp-1.0.1/smatchpp/data_helpers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5656 2023-07-17 07:17:24.000000 smatchpp-1.0.1/smatchpp/eval_statistics.py
--rw-rw-r--   0 user      (1000) user      (1000)     4060 2023-07-17 07:23:27.000000 smatchpp-1.0.1/smatchpp/interfaces.py
--rw-rw-r--   0 user      (1000) user      (1000)      277 2023-05-24 07:48:18.000000 smatchpp-1.0.1/smatchpp/log_helper.py
--rw-rw-r--   0 user      (1000) user      (1000)    17411 2023-07-17 07:25:47.000000 smatchpp-1.0.1/smatchpp/preprocess.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-21 07:44:27.322858 smatchpp-1.0.1/smatchpp/resource/
--rw-rw-r--   0 user      (1000) user      (1000)     2779 2023-06-12 15:24:28.000000 smatchpp-1.0.1/smatchpp/resource/amr_aspects.json
--rw-rw-r--   0 user      (1000) user      (1000)     2882 2023-05-22 07:15:48.000000 smatchpp-1.0.1/smatchpp/resource/concept_groups.json
--rw-rw-r--   0 user      (1000) user      (1000)   660511 2023-05-21 13:06:20.000000 smatchpp-1.0.1/smatchpp/resource/propbank-amr-frames-arg-descr.txt
--rw-rw-r--   0 user      (1000) user      (1000)     2366 2023-05-02 06:25:10.000000 smatchpp-1.0.1/smatchpp/resource/reify_table.txt
--rw-rw-r--   0 user      (1000) user      (1000)     5038 2023-07-17 07:27:34.000000 smatchpp-1.0.1/smatchpp/score.py
--rw-rw-r--   0 user      (1000) user      (1000)    27505 2023-07-17 07:29:37.000000 smatchpp-1.0.1/smatchpp/solvers.py
--rw-rw-r--   0 user      (1000) user      (1000)     8443 2023-07-18 15:37:03.000000 smatchpp-1.0.1/smatchpp/subgraph_extraction.py
--rw-rw-r--   0 user      (1000) user      (1000)     5257 2023-07-18 09:43:26.000000 smatchpp-1.0.1/smatchpp/util.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-21 07:44:27.322858 smatchpp-1.0.1/smatchpp.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     8510 2023-07-21 07:44:27.000000 smatchpp-1.0.1/smatchpp.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      603 2023-07-21 07:44:27.000000 smatchpp-1.0.1/smatchpp.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-21 07:44:27.000000 smatchpp-1.0.1/smatchpp.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-07-21 07:44:27.000000 smatchpp-1.0.1/smatchpp.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-21 07:50:21.755867 smatchpp-1.0.2/
+-rw-rw-r--   0 user      (1000) user      (1000)    35149 2023-05-03 15:50:47.000000 smatchpp-1.0.2/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     8521 2023-07-21 07:50:21.755867 smatchpp-1.0.2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     8123 2023-07-21 07:49:33.000000 smatchpp-1.0.2/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-21 07:50:21.755867 smatchpp-1.0.2/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      720 2023-07-21 07:50:03.000000 smatchpp-1.0.2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-21 07:50:21.751867 smatchpp-1.0.2/smatchpp/
+-rw-rw-r--   0 user      (1000) user      (1000)       32 2023-06-01 06:25:22.000000 smatchpp-1.0.2/smatchpp/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7585 2023-06-01 07:10:33.000000 smatchpp-1.0.2/smatchpp/__main__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5208 2023-07-17 07:11:06.000000 smatchpp-1.0.2/smatchpp/align.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6605 2023-07-17 07:04:27.000000 smatchpp-1.0.2/smatchpp/bindings.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8925 2023-07-18 09:38:55.000000 smatchpp-1.0.2/smatchpp/data_helpers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5656 2023-07-17 07:17:24.000000 smatchpp-1.0.2/smatchpp/eval_statistics.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4060 2023-07-17 07:23:27.000000 smatchpp-1.0.2/smatchpp/interfaces.py
+-rw-rw-r--   0 user      (1000) user      (1000)      277 2023-05-24 07:48:18.000000 smatchpp-1.0.2/smatchpp/log_helper.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17411 2023-07-17 07:25:47.000000 smatchpp-1.0.2/smatchpp/preprocess.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-21 07:50:21.751867 smatchpp-1.0.2/smatchpp/resource/
+-rw-rw-r--   0 user      (1000) user      (1000)     2779 2023-06-12 15:24:28.000000 smatchpp-1.0.2/smatchpp/resource/amr_aspects.json
+-rw-rw-r--   0 user      (1000) user      (1000)     2882 2023-05-22 07:15:48.000000 smatchpp-1.0.2/smatchpp/resource/concept_groups.json
+-rw-rw-r--   0 user      (1000) user      (1000)   660511 2023-05-21 13:06:20.000000 smatchpp-1.0.2/smatchpp/resource/propbank-amr-frames-arg-descr.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     2366 2023-05-02 06:25:10.000000 smatchpp-1.0.2/smatchpp/resource/reify_table.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     5038 2023-07-17 07:27:34.000000 smatchpp-1.0.2/smatchpp/score.py
+-rw-rw-r--   0 user      (1000) user      (1000)    27505 2023-07-17 07:29:37.000000 smatchpp-1.0.2/smatchpp/solvers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8443 2023-07-18 15:37:03.000000 smatchpp-1.0.2/smatchpp/subgraph_extraction.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5257 2023-07-18 09:43:26.000000 smatchpp-1.0.2/smatchpp/util.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-21 07:50:21.751867 smatchpp-1.0.2/smatchpp.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     8521 2023-07-21 07:50:21.000000 smatchpp-1.0.2/smatchpp.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      603 2023-07-21 07:50:21.000000 smatchpp-1.0.2/smatchpp.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-21 07:50:21.000000 smatchpp-1.0.2/smatchpp.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-07-21 07:50:21.000000 smatchpp-1.0.2/smatchpp.egg-info/top_level.txt
```

### Comparing `smatchpp-1.0.1/LICENSE` & `smatchpp-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smatchpp-1.0.1/PKG-INFO` & `smatchpp-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: smatchpp
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package for graph processing
 Home-page: https://github.com/flipz357/smatchpp
 Author: Juri Opitz
 Author-email: opitz.sci@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SMATCH++
 
-The package focuses on handy processing of AMR graphs with a special focus on standardized evaluation of AMR graph parsers with Smatch (structural matching of graphs). A short overview of some features:
+The package allows handy processing of semantic graphs such as AMRs, with a special focus on standardized evaluation of graph parsers with Smatch (structural matching of graphs). A short overview of some features:
 
 - Simple AMR reading, AMR writing, different syntactic and semantic AMR standardization options
 - Alignment solvers including optimal ILP alignment, and optional graph compression
 - Evaluation scoring with bootstrap confidence intervals, micro and macro averages
 - AMR-targeted subgraph extraction and extended scoring for spatial, temporal, causal, and more meaning aspects
 
 Jump directly to [parser evaluation best practices](#basic-eval) or (new) [pip install](#pip-install) to use smatch++ and its options simply from within your python program. The following text also gives an overview over some options of Smatch++.
```

### Comparing `smatchpp-1.0.1/README.md` & `smatchpp-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # SMATCH++
 
-The package focuses on handy processing of AMR graphs with a special focus on standardized evaluation of AMR graph parsers with Smatch (structural matching of graphs). A short overview of some features:
+The package allows handy processing of semantic graphs such as AMRs, with a special focus on standardized evaluation of graph parsers with Smatch (structural matching of graphs). A short overview of some features:
 
 - Simple AMR reading, AMR writing, different syntactic and semantic AMR standardization options
 - Alignment solvers including optimal ILP alignment, and optional graph compression
 - Evaluation scoring with bootstrap confidence intervals, micro and macro averages
 - AMR-targeted subgraph extraction and extended scoring for spatial, temporal, causal, and more meaning aspects
 
 Jump directly to [parser evaluation best practices](#basic-eval) or (new) [pip install](#pip-install) to use smatch++ and its options simply from within your python program. The following text also gives an overview over some options of Smatch++.
```

### Comparing `smatchpp-1.0.1/setup.py` & `smatchpp-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='smatchpp',
-    version='1.0.1',    
+    version='1.0.2',    
     description='A Python package for graph processing',
     url='https://github.com/flipz357/smatchpp',
     author='Juri Opitz',
     author_email='opitz.sci@gmail.com',
     license='GPLv3',
     packages=['smatchpp'],
     long_description=long_description,
```

### Comparing `smatchpp-1.0.1/smatchpp/__main__.py` & `smatchpp-1.0.2/smatchpp/__main__.py`

 * *Files identical despite different names*

### Comparing `smatchpp-1.0.1/smatchpp/align.py` & `smatchpp-1.0.2/smatchpp/align.py`

 * *Files identical despite different names*

### Comparing `smatchpp-1.0.1/smatchpp/bindings.py` & `smatchpp-1.0.2/smatchpp/bindings.py`

 * *Files identical despite different names*

### Comparing `smatchpp-1.0.1/smatchpp/data_helpers.py` & `smatchpp-1.0.2/smatchpp/data_helpers.py`

 * *Files identical despite different names*

### Comparing `smatchpp-1.0.1/smatchpp/eval_statistics.py` & `smatchpp-1.0.2/smatchpp/eval_statistics.py`

 * *Files identical despite different names*

### Comparing `smatchpp-1.0.1/smatchpp/interfaces.py` & `smatchpp-1.0.2/smatchpp/interfaces.py`

 * *Files identical despite different names*

### Comparing `smatchpp-1.0.1/smatchpp/preprocess.py` & `smatchpp-1.0.2/smatchpp/preprocess.py`

 * *Files identical despite different names*

### Comparing `smatchpp-1.0.1/smatchpp/resource/amr_aspects.json` & `smatchpp-1.0.2/smatchpp/resource/amr_aspects.json`

 * *Files identical despite different names*

### Comparing `smatchpp-1.0.1/smatchpp/resource/concept_groups.json` & `smatchpp-1.0.2/smatchpp/resource/concept_groups.json`

 * *Files identical despite different names*

### Comparing `smatchpp-1.0.1/smatchpp/resource/propbank-amr-frames-arg-descr.txt` & `smatchpp-1.0.2/smatchpp/resource/propbank-amr-frames-arg-descr.txt`

 * *Files identical despite different names*

### Comparing `smatchpp-1.0.1/smatchpp/resource/reify_table.txt` & `smatchpp-1.0.2/smatchpp/resource/reify_table.txt`

 * *Files identical despite different names*

### Comparing `smatchpp-1.0.1/smatchpp/score.py` & `smatchpp-1.0.2/smatchpp/score.py`

 * *Files identical despite different names*

### Comparing `smatchpp-1.0.1/smatchpp/solvers.py` & `smatchpp-1.0.2/smatchpp/solvers.py`

 * *Files identical despite different names*

### Comparing `smatchpp-1.0.1/smatchpp/subgraph_extraction.py` & `smatchpp-1.0.2/smatchpp/subgraph_extraction.py`

 * *Files identical despite different names*

### Comparing `smatchpp-1.0.1/smatchpp/util.py` & `smatchpp-1.0.2/smatchpp/util.py`

 * *Files identical despite different names*

### Comparing `smatchpp-1.0.1/smatchpp.egg-info/PKG-INFO` & `smatchpp-1.0.2/smatchpp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: smatchpp
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package for graph processing
 Home-page: https://github.com/flipz357/smatchpp
 Author: Juri Opitz
 Author-email: opitz.sci@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SMATCH++
 
-The package focuses on handy processing of AMR graphs with a special focus on standardized evaluation of AMR graph parsers with Smatch (structural matching of graphs). A short overview of some features:
+The package allows handy processing of semantic graphs such as AMRs, with a special focus on standardized evaluation of graph parsers with Smatch (structural matching of graphs). A short overview of some features:
 
 - Simple AMR reading, AMR writing, different syntactic and semantic AMR standardization options
 - Alignment solvers including optimal ILP alignment, and optional graph compression
 - Evaluation scoring with bootstrap confidence intervals, micro and macro averages
 - AMR-targeted subgraph extraction and extended scoring for spatial, temporal, causal, and more meaning aspects
 
 Jump directly to [parser evaluation best practices](#basic-eval) or (new) [pip install](#pip-install) to use smatch++ and its options simply from within your python program. The following text also gives an overview over some options of Smatch++.
```

### Comparing `smatchpp-1.0.1/smatchpp.egg-info/SOURCES.txt` & `smatchpp-1.0.2/smatchpp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

