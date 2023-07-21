# Comparing `tmp/deepsearch_glm-0.1.0.tar.gz` & `tmp/deepsearch_glm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsearch_glm-0.1.0.tar", max compression
+gzip compressed data, was "deepsearch_glm-0.2.1.tar", max compression
```

## Comparing `deepsearch_glm-0.1.0.tar` & `deepsearch_glm-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1088 2023-07-08 03:50:49.893964 deepsearch_glm-0.1.0/LICENSE
--rw-r--r--   0        0        0     2984 2023-07-14 09:21:46.015603 deepsearch_glm-0.1.0/README.md
--rw-r--r--   0        0        0     1865 2023-07-19 11:33:20.262462 deepsearch_glm-0.1.0/build.py
--rw-r--r--   0        0        0        0 2023-07-08 03:50:49.913495 deepsearch_glm-0.1.0/deepsearch_glm/__init__.py
--rw-r--r--   0        0        0     3029 2023-07-19 07:59:42.945265 deepsearch_glm-0.1.0/deepsearch_glm/glm_create_from_docs.py
--rw-r--r--   0        0        0     4988 2023-07-14 09:21:46.051654 deepsearch_glm-0.1.0/deepsearch_glm/glm_docqa.py
--rw-r--r--   0        0        0     3137 2023-07-14 09:21:46.052650 deepsearch_glm-0.1.0/deepsearch_glm/glm_explore.py
--rw-r--r--   0        0        0     2937 2023-07-14 09:21:46.053534 deepsearch_glm-0.1.0/deepsearch_glm/glm_utils.py
--rw-r--r--   0        0        0     4321 2023-07-19 11:56:02.353186 deepsearch_glm-0.1.0/deepsearch_glm/nlp_analyse_docs.py
--rw-r--r--   0        0        0     3856 2023-07-15 04:44:33.063375 deepsearch_glm-0.1.0/deepsearch_glm/nlp_apply_on_docs.py
--rw-r--r--   0        0        0    21643 2023-07-19 10:33:19.659719 deepsearch_glm-0.1.0/deepsearch_glm/nlp_train_reference.py
--rw-r--r--   0        0        0     1819 2023-07-19 10:33:19.661841 deepsearch_glm-0.1.0/deepsearch_glm/nlp_utils.py
--rw-r--r--   0        0        0     8534 2023-07-14 09:21:46.056334 deepsearch_glm-0.1.0/deepsearch_glm/resources/confusables/confusablesRestricted.txt
--rw-r--r--   0        0        0   599388 2023-07-14 09:21:46.058795 deepsearch_glm-0.1.0/deepsearch_glm/resources/confusables/confusablesSummary.txt
--rw-r--r--   0        0        0       82 2023-07-14 09:21:46.059061 deepsearch_glm-0.1.0/deepsearch_glm/resources/confusables/note.txt
--rw-r--r--   0        0        0      679 2023-07-14 09:21:46.059828 deepsearch_glm-0.1.0/deepsearch_glm/resources/models/crf/part-of-speech/note.md
--rw-r--r--   0        0        0        0 2023-07-14 09:21:46.059928 deepsearch_glm-0.1.0/deepsearch_glm/resources/models/crf/reference/note.md
--rw-r--r--   0        0        0      188 2023-07-14 09:21:46.060169 deepsearch_glm-0.1.0/deepsearch_glm/resources/models/fasttext/language/note.md
--rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060269 deepsearch_glm-0.1.0/deepsearch_glm/resources/models/fasttext/person-name/note.md
--rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060409 deepsearch_glm-0.1.0/deepsearch_glm/resources/models/fasttext/semantic/note.md
--rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060599 deepsearch_glm-0.1.0/deepsearch_glm/resources/models/fasttext/topic/note.md
--rw-r--r--   0        0        0      801 2023-07-14 09:21:46.059514 deepsearch_glm-0.1.0/deepsearch_glm/resources/models.json
--rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060732 deepsearch_glm-0.1.0/deepsearch_glm/utils/__init__.py
--rw-r--r--   0        0        0     1803 2023-07-15 05:40:03.618146 deepsearch_glm-0.1.0/deepsearch_glm/utils/ds_query.py
--rw-r--r--   0        0        0     7364 2023-07-19 10:33:19.662906 deepsearch_glm-0.1.0/deepsearch_glm/utils/ds_utils.py
--rw-r--r--   0        0        0     1295 2023-07-19 10:33:19.663903 deepsearch_glm-0.1.0/deepsearch_glm/utils/load_pretrained_models.py
--rw-r--r--   0        0        0      728 2023-07-14 09:21:46.066778 deepsearch_glm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4006 1970-01-01 00:00:00.000000 deepsearch_glm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-07-08 03:50:49.893964 deepsearch_glm-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2984 2023-07-14 09:21:46.015603 deepsearch_glm-0.2.1/README.md
+-rw-r--r--   0        0        0     1840 2023-07-21 12:54:50.598456 deepsearch_glm-0.2.1/build.py
+-rw-r--r--   0        0        0        0 2023-07-08 03:50:49.913495 deepsearch_glm-0.2.1/deepsearch_glm/__init__.py
+-rw-r--r--   0        0        0     3029 2023-07-19 07:59:42.945265 deepsearch_glm-0.2.1/deepsearch_glm/glm_create_from_docs.py
+-rw-r--r--   0        0        0     4988 2023-07-14 09:21:46.051654 deepsearch_glm-0.2.1/deepsearch_glm/glm_docqa.py
+-rw-r--r--   0        0        0     3137 2023-07-14 09:21:46.052650 deepsearch_glm-0.2.1/deepsearch_glm/glm_explore.py
+-rw-r--r--   0        0        0     2937 2023-07-14 09:21:46.053534 deepsearch_glm-0.2.1/deepsearch_glm/glm_utils.py
+-rw-r--r--   0        0        0     4226 2023-07-21 07:26:03.085046 deepsearch_glm-0.2.1/deepsearch_glm/nlp_analyse_docs.py
+-rw-r--r--   0        0        0     3856 2023-07-20 05:17:22.733695 deepsearch_glm-0.2.1/deepsearch_glm/nlp_apply_on_docs.py
+-rw-r--r--   0        0        0     2161 2023-07-21 07:26:03.085678 deepsearch_glm-0.2.1/deepsearch_glm/nlp_apply_on_text.py
+-rw-r--r--   0        0        0    21643 2023-07-21 07:26:03.086794 deepsearch_glm-0.2.1/deepsearch_glm/nlp_train_reference.py
+-rw-r--r--   0        0        0     1819 2023-07-21 07:26:03.088127 deepsearch_glm-0.2.1/deepsearch_glm/nlp_utils.py
+-rw-r--r--   0        0        0     8534 2023-07-14 09:21:46.056334 deepsearch_glm-0.2.1/deepsearch_glm/resources/confusables/confusablesRestricted.txt
+-rw-r--r--   0        0        0   599388 2023-07-14 09:21:46.058795 deepsearch_glm-0.2.1/deepsearch_glm/resources/confusables/confusablesSummary.txt
+-rw-r--r--   0        0        0       82 2023-07-14 09:21:46.059061 deepsearch_glm-0.2.1/deepsearch_glm/resources/confusables/note.txt
+-rw-r--r--   0        0        0      679 2023-07-14 09:21:46.059828 deepsearch_glm-0.2.1/deepsearch_glm/resources/models/crf/part-of-speech/note.md
+-rw-r--r--   0        0        0        0 2023-07-14 09:21:46.059928 deepsearch_glm-0.2.1/deepsearch_glm/resources/models/crf/reference/note.md
+-rw-r--r--   0        0        0      188 2023-07-14 09:21:46.060169 deepsearch_glm-0.2.1/deepsearch_glm/resources/models/fasttext/language/note.md
+-rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060269 deepsearch_glm-0.2.1/deepsearch_glm/resources/models/fasttext/person-name/note.md
+-rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060409 deepsearch_glm-0.2.1/deepsearch_glm/resources/models/fasttext/semantic/note.md
+-rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060599 deepsearch_glm-0.2.1/deepsearch_glm/resources/models/fasttext/topic/note.md
+-rw-r--r--   0        0        0      801 2023-07-14 09:21:46.059514 deepsearch_glm-0.2.1/deepsearch_glm/resources/models.json
+-rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060732 deepsearch_glm-0.2.1/deepsearch_glm/utils/__init__.py
+-rw-r--r--   0        0        0     1803 2023-07-15 05:40:03.618146 deepsearch_glm-0.2.1/deepsearch_glm/utils/ds_query.py
+-rw-r--r--   0        0        0     7364 2023-07-21 07:26:03.089281 deepsearch_glm-0.2.1/deepsearch_glm/utils/ds_utils.py
+-rw-r--r--   0        0        0     1295 2023-07-21 07:26:03.090106 deepsearch_glm-0.2.1/deepsearch_glm/utils/load_pretrained_models.py
+-rw-r--r--   0        0        0      729 2023-07-21 12:54:50.600869 deepsearch_glm-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3957 1970-01-01 00:00:00.000000 deepsearch_glm-0.2.1/PKG-INFO
```

### Comparing `deepsearch_glm-0.1.0/LICENSE` & `deepsearch_glm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.1.0/README.md` & `deepsearch_glm-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.1.0/deepsearch_glm/glm_create_from_docs.py` & `deepsearch_glm-0.2.1/deepsearch_glm/glm_create_from_docs.py`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.1.0/deepsearch_glm/glm_docqa.py` & `deepsearch_glm-0.2.1/deepsearch_glm/glm_docqa.py`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.1.0/deepsearch_glm/glm_explore.py` & `deepsearch_glm-0.2.1/deepsearch_glm/glm_explore.py`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.1.0/deepsearch_glm/glm_utils.py` & `deepsearch_glm-0.2.1/deepsearch_glm/glm_utils.py`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.1.0/deepsearch_glm/nlp_analyse_docs.py` & `deepsearch_glm-0.2.1/deepsearch_glm/nlp_analyse_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,19 +146,14 @@
             refs = df[df["subj_path"]==path][["subj_path", "type", "subtype", "original"]]
             print(refs)            
                 
     return
 
 if __name__ == '__main__':
 
-    mdl = andromeda_nlp.nlp_model()
-    print(mdl.get_resources_path())
-    
-    exit(-1)
-    
     json_files = parse_arguments()
 
     for json_file in json_files:
 
         print(f" --> reading {json_file}")
         with open(json_file, "r") as fr:
             doc = json.load(fr)
```

### Comparing `deepsearch_glm-0.1.0/deepsearch_glm/nlp_apply_on_docs.py` & `deepsearch_glm-0.2.1/deepsearch_glm/nlp_apply_on_docs.py`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.1.0/deepsearch_glm/nlp_train_reference.py` & `deepsearch_glm-0.2.1/deepsearch_glm/nlp_train_reference.py`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.1.0/deepsearch_glm/nlp_utils.py` & `deepsearch_glm-0.2.1/deepsearch_glm/nlp_utils.py`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.1.0/deepsearch_glm/resources/confusables/confusablesRestricted.txt` & `deepsearch_glm-0.2.1/deepsearch_glm/resources/confusables/confusablesRestricted.txt`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.1.0/deepsearch_glm/resources/confusables/confusablesSummary.txt` & `deepsearch_glm-0.2.1/deepsearch_glm/resources/confusables/confusablesSummary.txt`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.1.0/deepsearch_glm/resources/models/crf/part-of-speech/note.md` & `deepsearch_glm-0.2.1/deepsearch_glm/resources/models/crf/part-of-speech/note.md`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.1.0/deepsearch_glm/resources/models.json` & `deepsearch_glm-0.2.1/deepsearch_glm/resources/models.json`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.1.0/deepsearch_glm/utils/ds_query.py` & `deepsearch_glm-0.2.1/deepsearch_glm/utils/ds_query.py`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.1.0/deepsearch_glm/utils/ds_utils.py` & `deepsearch_glm-0.2.1/deepsearch_glm/utils/ds_utils.py`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.1.0/deepsearch_glm/utils/load_pretrained_models.py` & `deepsearch_glm-0.2.1/deepsearch_glm/utils/load_pretrained_models.py`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.1.0/pyproject.toml` & `deepsearch_glm-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "deepsearch-glm"
-version = "0.1.0"
+version = "0.2.1"
 description = "Graph Language Models"
 authors = ["Peter Staar <taa@zurich.ibm.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "deepsearch_glm"}]
 include = [
     {path = "deepsearch_glm/*.so", format = "wheel"}
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 deepsearch-toolkit = "^0.19.1"
 textColor = "^3.0.1"
 tabulate = "^0.8.9"
 numpy = "^1.25.0"
 pandas = "^2.0.3"
 matplotlib = "^3.7.1"
 networkx = "^3.1"
```

### Comparing `deepsearch_glm-0.1.0/PKG-INFO` & `deepsearch_glm-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: deepsearch-glm
-Version: 0.1.0
+Version: 0.2.1
 Summary: Graph Language Models
 License: MIT
 Author: Peter Staar
 Author-email: taa@zurich.ibm.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: deepsearch-toolkit (>=0.19.1,<0.20.0)
 Requires-Dist: fastapi (>=0.99.0,<0.100.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: netwulf (>=0.1.5,<0.2.0)
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_nvph6c3a_/tmp0dqxltaw_TarContainer/0/27", line 141, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_nvph6c3a_/tmp0dqxltaw_TarContainer/0/27", line 141, column 0: CDATA terminal not found*

```diff
@@ -1,29 +1,28 @@
-Metadata-Version: 2.1 Name: deepsearch-glm Version: 0.1.0 Summary: Graph
+Metadata-Version: 2.1 Name: deepsearch-glm Version: 0.2.1 Summary: Graph
 Language Models License: MIT Author: Peter Staar Author-email:
-taa@zurich.ibm.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
+taa@zurich.ibm.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: deepsearch-toolkit (>=0.19.1,<0.20.0) Requires-Dist: fastapi
-(>=0.99.0,<0.100.0) Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-Dist:
-networkx (>=3.1,<4.0) Requires-Dist: netwulf (>=0.1.5,<0.2.0) Requires-Dist:
-numerize (>=0.12,<0.13) Requires-Dist: numpy (>=1.25.0,<2.0.0) Requires-Dist:
-pandas (>=2.0.3,<3.0.0) Requires-Dist: pybind11 (>=2.10.4,<3.0.0) Requires-
-Dist: python-dotenv (>=1.0.0,<2.0.0) Requires-Dist: tabulate (>=0.8.9,<0.9.0)
-Requires-Dist: textColor (>=3.0.1,<4.0.0) Requires-Dist: uvicorn
-(>=0.22.0,<0.23.0) Description-Content-Type: text/markdown # Graph Language
-Models ![build](https://github.com/DS4SD/deepsearch-glm/actions/workflows/
-cmake.yml/badge.svg) [![PyPI version](https://img.shields.io/pypi/v/deepsearch-
-glm)](https://pypi.org/project/deepsearch-glm/) [![PyPI - Python Version]
-(https://img.shields.io/pypi/pyversions/deepsearch-glm)](https://pypi.org/
-project/deepsearch-glm/) [![License MIT](https://img.shields.io/github/license/
-ds4sd/deepsearch-glm)](https://opensource.org/licenses/MIT) ## Install ###
-Python installation To use the python interface, first make sure all
-dependencies are installed. We use [poetry](https://python-poetry.org/docs/
-) for that. To install all the dependent python packages and get the python
-bindings, simply execute, ```sh poetry install ``` ### CXX compilation To
-compile from scratch, simply run the following command in the `deepsearch-glm`
-root folder to create the `build` directory, ```sh cmake -B ./build; ``` Next,
-compile the code from scratch, ```sh cmake --build ./build -j ``` ## Run using
-the Python Interface ### NLP and GLM examples To run the examples, simply do
-execute the scripts as `poetry run python
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Dist: deepsearch-toolkit (>=0.19.1,<0.20.0)
+Requires-Dist: fastapi (>=0.99.0,<0.100.0) Requires-Dist: matplotlib
+(>=3.7.1,<4.0.0) Requires-Dist: networkx (>=3.1,<4.0) Requires-Dist: netwulf
+(>=0.1.5,<0.2.0) Requires-Dist: numerize (>=0.12,<0.13) Requires-Dist: numpy
+(>=1.25.0,<2.0.0) Requires-Dist: pandas (>=2.0.3,<3.0.0) Requires-Dist:
+pybind11 (>=2.10.4,<3.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: tabulate (>=0.8.9,<0.9.0) Requires-Dist: textColor
+(>=3.0.1,<4.0.0) Requires-Dist: uvicorn (>=0.22.0,<0.23.0) Description-Content-
+Type: text/markdown # Graph Language Models ![build](https://github.com/DS4SD/
+deepsearch-glm/actions/workflows/cmake.yml/badge.svg) [![PyPI version](https://
+img.shields.io/pypi/v/deepsearch-glm)](https://pypi.org/project/deepsearch-glm/
+) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/deepsearch-
+glm)](https://pypi.org/project/deepsearch-glm/) [![License MIT](https://
+img.shields.io/github/license/ds4sd/deepsearch-glm)](https://opensource.org/
+licenses/MIT) ## Install ### Python installation To use the python interface,
+first make sure all dependencies are installed. We use [poetry](https://python-
+poetry.org/docs/) for that. To install all the dependent python packages and
+get the python bindings, simply execute, ```sh poetry install ``` ### CXX
+compilation To compile from scratch, simply run the following command in the
+`deepsearch-glm` root folder to create the `build` directory, ```sh cmake -B ./
+build; ``` Next, compile the code from scratch, ```sh cmake --build ./build -
+j ``` ## Run using the Python Interface ### NLP and GLM examples To run the
+examples, simply do execute the scripts as `poetry run python
```

