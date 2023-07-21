# Comparing `tmp/verify4py-1.0.0.tar.gz` & `tmp/verify4py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verify4py-1.0.0.tar", last modified: Fri Jul 21 04:06:24 2023, max compression
+gzip compressed data, was "verify4py-1.0.1.tar", last modified: Fri Jul 21 04:08:23 2023, max compression
```

## Comparing `verify4py-1.0.0.tar` & `verify4py-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-21 04:06:24.395022 verify4py-1.0.0/
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1065 2022-04-11 09:13:53.000000 verify4py-1.0.0/LICENSE
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     9382 2023-07-21 04:06:24.395022 verify4py-1.0.0/PKG-INFO
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     8817 2023-07-21 04:05:08.000000 verify4py-1.0.0/README.md
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       84 2022-04-11 09:22:24.000000 verify4py-1.0.0/pyproject.toml
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       38 2023-07-21 04:06:24.395022 verify4py-1.0.0/setup.cfg
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      901 2023-07-21 04:06:12.000000 verify4py-1.0.0/setup.py
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-21 04:06:24.391022 verify4py-1.0.0/src/
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-21 04:06:24.395022 verify4py-1.0.0/src/verify4py/
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    10980 2023-07-21 04:05:08.000000 verify4py-1.0.0/src/verify4py/Issuer.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     3815 2022-05-13 07:31:57.000000 verify4py-1.0.0/src/verify4py/JsonIssuer.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     2909 2022-07-06 07:22:13.000000 verify4py-1.0.0/src/verify4py/PdfIssuer.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     3662 2022-07-06 10:35:49.000000 verify4py-1.0.0/src/verify4py/UniversityDiplomaIssuer.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        0 2022-04-11 09:38:54.000000 verify4py-1.0.0/src/verify4py/__init__.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    27300 2023-07-21 04:05:08.000000 verify4py-1.0.0/src/verify4py/certify_sc_utils.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     2788 2022-05-10 06:21:26.000000 verify4py-1.0.0/src/verify4py/chainpoint.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1067 2022-07-06 08:44:53.000000 verify4py-1.0.0/src/verify4py/json_utils.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      689 2022-07-06 07:08:53.000000 verify4py-1.0.0/src/verify4py/pdf.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    19898 2022-07-04 09:06:21.000000 verify4py-1.0.0/src/verify4py/university_abi.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1526 2023-07-21 04:05:08.000000 verify4py-1.0.0/src/verify4py/utils.py
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-21 04:06:24.395022 verify4py-1.0.0/src/verify4py.egg-info/
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     9382 2023-07-21 04:06:24.000000 verify4py-1.0.0/src/verify4py.egg-info/PKG-INFO
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      537 2023-07-21 04:06:24.000000 verify4py-1.0.0/src/verify4py.egg-info/SOURCES.txt
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        1 2023-07-21 04:06:24.000000 verify4py-1.0.0/src/verify4py.egg-info/dependency_links.txt
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       42 2023-07-21 04:06:24.000000 verify4py-1.0.0/src/verify4py.egg-info/requires.txt
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       10 2023-07-21 04:06:24.000000 verify4py-1.0.0/src/verify4py.egg-info/top_level.txt
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-21 04:08:23.507861 verify4py-1.0.1/
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1065 2022-04-11 09:13:53.000000 verify4py-1.0.1/LICENSE
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     9388 2023-07-21 04:08:23.507861 verify4py-1.0.1/PKG-INFO
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     8817 2023-07-21 04:05:08.000000 verify4py-1.0.1/README.md
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       84 2022-04-11 09:22:24.000000 verify4py-1.0.1/pyproject.toml
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       38 2023-07-21 04:08:23.507861 verify4py-1.0.1/setup.cfg
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      907 2023-07-21 04:08:19.000000 verify4py-1.0.1/setup.py
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-21 04:08:23.503860 verify4py-1.0.1/src/
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-21 04:08:23.503860 verify4py-1.0.1/src/verify4py/
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    10980 2023-07-21 04:05:08.000000 verify4py-1.0.1/src/verify4py/Issuer.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     3815 2022-05-13 07:31:57.000000 verify4py-1.0.1/src/verify4py/JsonIssuer.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     2909 2022-07-06 07:22:13.000000 verify4py-1.0.1/src/verify4py/PdfIssuer.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     3662 2022-07-06 10:35:49.000000 verify4py-1.0.1/src/verify4py/UniversityDiplomaIssuer.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        0 2022-04-11 09:38:54.000000 verify4py-1.0.1/src/verify4py/__init__.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    27300 2023-07-21 04:05:08.000000 verify4py-1.0.1/src/verify4py/certify_sc_utils.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     2788 2022-05-10 06:21:26.000000 verify4py-1.0.1/src/verify4py/chainpoint.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1067 2022-07-06 08:44:53.000000 verify4py-1.0.1/src/verify4py/json_utils.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      689 2022-07-06 07:08:53.000000 verify4py-1.0.1/src/verify4py/pdf.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    19898 2022-07-04 09:06:21.000000 verify4py-1.0.1/src/verify4py/university_abi.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1526 2023-07-21 04:05:08.000000 verify4py-1.0.1/src/verify4py/utils.py
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-21 04:08:23.503860 verify4py-1.0.1/src/verify4py.egg-info/
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     9388 2023-07-21 04:08:23.000000 verify4py-1.0.1/src/verify4py.egg-info/PKG-INFO
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      537 2023-07-21 04:08:23.000000 verify4py-1.0.1/src/verify4py.egg-info/SOURCES.txt
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        1 2023-07-21 04:08:23.000000 verify4py-1.0.1/src/verify4py.egg-info/dependency_links.txt
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       42 2023-07-21 04:08:23.000000 verify4py-1.0.1/src/verify4py.egg-info/requires.txt
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       10 2023-07-21 04:08:23.000000 verify4py-1.0.1/src/verify4py.egg-info/top_level.txt
```

### Comparing `verify4py-1.0.0/LICENSE` & `verify4py-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.0/PKG-INFO` & `verify4py-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: verify4py
-Version: 1.0.0
+Version: 1.0.1
 Summary: Issue certificates using blockchain and smart contract
 Home-page: https://github.com/teo-mn/verify4py
 Author: Surenbayar Doloonjin
 Author-email: surenbayar@corex.mn
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/teo-mn/verify4py/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.6,<3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Verify4py 
 Verify4py нь сертификат, диплом, дансны хуулга зэрэг бичиг баримтыг блокчэйн дээр
 баталгаажуулж өгөх https://github.com/corex-mn/certify-sc ухаалаг гэрээтэй харьцдаг python хэлний сан юм.
```

### Comparing `verify4py-1.0.0/README.md` & `verify4py-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.0/setup.py` & `verify4py-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="verify4py",
-    version="1.0.0",
+    version="1.0.1",
     author="Surenbayar Doloonjin",
     author_email="surenbayar@corex.mn",
     description="Issue certificates using blockchain and smart contract",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/teo-mn/verify4py",
     project_urls={
@@ -18,10 +18,10 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.6",
+    python_requires=">=3.6,<3.11",
     install_requires=['web3==6.6.1', 'merkletools==1.0.3', 'pdfrw==0.3']
 )
```

### Comparing `verify4py-1.0.0/src/verify4py/Issuer.py` & `verify4py-1.0.1/src/verify4py/Issuer.py`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.0/src/verify4py/JsonIssuer.py` & `verify4py-1.0.1/src/verify4py/JsonIssuer.py`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.0/src/verify4py/PdfIssuer.py` & `verify4py-1.0.1/src/verify4py/PdfIssuer.py`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.0/src/verify4py/UniversityDiplomaIssuer.py` & `verify4py-1.0.1/src/verify4py/UniversityDiplomaIssuer.py`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.0/src/verify4py/certify_sc_utils.py` & `verify4py-1.0.1/src/verify4py/certify_sc_utils.py`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.0/src/verify4py/chainpoint.py` & `verify4py-1.0.1/src/verify4py/chainpoint.py`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.0/src/verify4py/json_utils.py` & `verify4py-1.0.1/src/verify4py/json_utils.py`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.0/src/verify4py/pdf.py` & `verify4py-1.0.1/src/verify4py/pdf.py`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.0/src/verify4py/university_abi.py` & `verify4py-1.0.1/src/verify4py/university_abi.py`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.0/src/verify4py/utils.py` & `verify4py-1.0.1/src/verify4py/utils.py`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.0/src/verify4py.egg-info/PKG-INFO` & `verify4py-1.0.1/src/verify4py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: verify4py
-Version: 1.0.0
+Version: 1.0.1
 Summary: Issue certificates using blockchain and smart contract
 Home-page: https://github.com/teo-mn/verify4py
 Author: Surenbayar Doloonjin
 Author-email: surenbayar@corex.mn
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/teo-mn/verify4py/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.6,<3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Verify4py 
 Verify4py нь сертификат, диплом, дансны хуулга зэрэг бичиг баримтыг блокчэйн дээр
 баталгаажуулж өгөх https://github.com/corex-mn/certify-sc ухаалаг гэрээтэй харьцдаг python хэлний сан юм.
```

### Comparing `verify4py-1.0.0/src/verify4py.egg-info/SOURCES.txt` & `verify4py-1.0.1/src/verify4py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

