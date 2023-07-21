# Comparing `tmp/certify4py-0.1.5.tar.gz` & `tmp/certify4py-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certify4py-0.1.5.tar", last modified: Wed Jul  5 10:34:47 2023, max compression
+gzip compressed data, was "certify4py-0.1.6.tar", last modified: Fri Jul 21 03:17:25 2023, max compression
```

## Comparing `certify4py-0.1.5.tar` & `certify4py-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-05 10:34:47.468239 certify4py-0.1.5/
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1063 2023-07-05 10:33:01.000000 certify4py-0.1.5/LICENSE
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     9334 2023-07-05 10:34:47.468239 certify4py-0.1.5/PKG-INFO
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     8768 2023-07-05 10:33:01.000000 certify4py-0.1.5/README.md
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       84 2023-07-05 10:33:01.000000 certify4py-0.1.5/pyproject.toml
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       38 2023-07-05 10:34:47.468239 certify4py-0.1.5/setup.cfg
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      829 2023-07-05 10:33:01.000000 certify4py-0.1.5/setup.py
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-05 10:34:47.468239 certify4py-0.1.5/src/
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-05 10:34:47.468239 certify4py-0.1.5/src/certify4py/
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    10961 2023-07-05 10:33:01.000000 certify4py-0.1.5/src/certify4py/Issuer.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     4320 2023-07-05 10:33:01.000000 certify4py-0.1.5/src/certify4py/UniversityDiplomaIssuer.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-05 10:33:01.000000 certify4py-0.1.5/src/certify4py/__init__.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    27276 2023-07-05 10:33:01.000000 certify4py-0.1.5/src/certify4py/certify_sc_utils.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     2788 2023-07-05 10:33:01.000000 certify4py-0.1.5/src/certify4py/chainpoint.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1067 2023-07-05 10:33:01.000000 certify4py-0.1.5/src/certify4py/json_utils.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      689 2023-07-05 10:33:01.000000 certify4py-0.1.5/src/certify4py/pdf.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    19898 2023-07-05 10:33:01.000000 certify4py-0.1.5/src/certify4py/university_abi.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1525 2023-07-05 10:33:01.000000 certify4py-0.1.5/src/certify4py/utils.py
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-05 10:34:47.468239 certify4py-0.1.5/src/certify4py.egg-info/
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     9334 2023-07-05 10:34:47.000000 certify4py-0.1.5/src/certify4py.egg-info/PKG-INFO
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      459 2023-07-05 10:34:47.000000 certify4py-0.1.5/src/certify4py.egg-info/SOURCES.txt
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        1 2023-07-05 10:34:47.000000 certify4py-0.1.5/src/certify4py.egg-info/dependency_links.txt
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       11 2023-07-05 10:34:47.000000 certify4py-0.1.5/src/certify4py.egg-info/top_level.txt
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-21 03:17:25.196149 certify4py-0.1.6/
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1063 2023-07-05 10:33:01.000000 certify4py-0.1.6/LICENSE
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     9340 2023-07-21 03:17:25.196149 certify4py-0.1.6/PKG-INFO
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     8768 2023-07-05 10:33:01.000000 certify4py-0.1.6/README.md
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       84 2023-07-05 10:33:01.000000 certify4py-0.1.6/pyproject.toml
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       38 2023-07-21 03:17:25.196149 certify4py-0.1.6/setup.cfg
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      909 2023-07-21 03:17:23.000000 certify4py-0.1.6/setup.py
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-21 03:17:25.192149 certify4py-0.1.6/src/
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-21 03:17:25.196149 certify4py-0.1.6/src/certify4py/
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    10961 2023-07-05 10:33:01.000000 certify4py-0.1.6/src/certify4py/Issuer.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     4320 2023-07-05 10:33:01.000000 certify4py-0.1.6/src/certify4py/UniversityDiplomaIssuer.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-05 10:33:01.000000 certify4py-0.1.6/src/certify4py/__init__.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    27276 2023-07-05 10:33:01.000000 certify4py-0.1.6/src/certify4py/certify_sc_utils.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     2788 2023-07-05 10:33:01.000000 certify4py-0.1.6/src/certify4py/chainpoint.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1067 2023-07-05 10:33:01.000000 certify4py-0.1.6/src/certify4py/json_utils.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      689 2023-07-05 10:33:01.000000 certify4py-0.1.6/src/certify4py/pdf.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    19898 2023-07-05 10:33:01.000000 certify4py-0.1.6/src/certify4py/university_abi.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1525 2023-07-05 10:33:01.000000 certify4py-0.1.6/src/certify4py/utils.py
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-21 03:17:25.196149 certify4py-0.1.6/src/certify4py.egg-info/
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     9340 2023-07-21 03:17:24.000000 certify4py-0.1.6/src/certify4py.egg-info/PKG-INFO
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      496 2023-07-21 03:17:25.000000 certify4py-0.1.6/src/certify4py.egg-info/SOURCES.txt
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        1 2023-07-21 03:17:24.000000 certify4py-0.1.6/src/certify4py.egg-info/dependency_links.txt
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       43 2023-07-21 03:17:25.000000 certify4py-0.1.6/src/certify4py.egg-info/requires.txt
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       11 2023-07-21 03:17:25.000000 certify4py-0.1.6/src/certify4py.egg-info/top_level.txt
```

### Comparing `certify4py-0.1.5/LICENSE` & `certify4py-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `certify4py-0.1.5/PKG-INFO` & `certify4py-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: certify4py
-Version: 0.1.5
+Version: 0.1.6
 Summary: Issue certificates using blockchain and smart contract
 Home-page: https://github.com/teo-mn/certify4py
 Author: Surenbayar Doloonjin
 Author-email: surenbayar@teo.mn
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/teo-mn/certify4py/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.6,<3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Certify4py 
 Certify4py нь цахим сертификат, дипломыг блокчэйн дээр
 баталгаажуулж өгөх https://github.com/teo-mn/certify-sc ухаалаг гэрээтэй харьцдаг python хэлний сан юм.
 Уг ухаалаг гэрээ нь ИДС-ын дипломыг блокчэйнд баталгаажуулах стандарт бөгөөд дэлгэрэнгүйг дээрх линкээс харна уу.
```

### Comparing `certify4py-0.1.5/README.md` & `certify4py-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `certify4py-0.1.5/setup.py` & `certify4py-0.1.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="certify4py",
-    version="0.1.5",
+    version="0.1.6",
     author="Surenbayar Doloonjin",
     author_email="surenbayar@teo.mn",
     description="Issue certificates using blockchain and smart contract",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/teo-mn/certify4py",
     project_urls={
@@ -18,9 +18,10 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.6",
+    python_requires=">=3.6,<3.11",
+    install_requires=['web3==5.28.0', 'merkletools==1.0.3', 'pdfrw==0.3']
 )
```

### Comparing `certify4py-0.1.5/src/certify4py/Issuer.py` & `certify4py-0.1.6/src/certify4py/Issuer.py`

 * *Files identical despite different names*

### Comparing `certify4py-0.1.5/src/certify4py/UniversityDiplomaIssuer.py` & `certify4py-0.1.6/src/certify4py/UniversityDiplomaIssuer.py`

 * *Files identical despite different names*

### Comparing `certify4py-0.1.5/src/certify4py/certify_sc_utils.py` & `certify4py-0.1.6/src/certify4py/certify_sc_utils.py`

 * *Files identical despite different names*

### Comparing `certify4py-0.1.5/src/certify4py/chainpoint.py` & `certify4py-0.1.6/src/certify4py/chainpoint.py`

 * *Files identical despite different names*

### Comparing `certify4py-0.1.5/src/certify4py/json_utils.py` & `certify4py-0.1.6/src/certify4py/json_utils.py`

 * *Files identical despite different names*

### Comparing `certify4py-0.1.5/src/certify4py/pdf.py` & `certify4py-0.1.6/src/certify4py/pdf.py`

 * *Files identical despite different names*

### Comparing `certify4py-0.1.5/src/certify4py/university_abi.py` & `certify4py-0.1.6/src/certify4py/university_abi.py`

 * *Files identical despite different names*

### Comparing `certify4py-0.1.5/src/certify4py/utils.py` & `certify4py-0.1.6/src/certify4py/utils.py`

 * *Files identical despite different names*

### Comparing `certify4py-0.1.5/src/certify4py.egg-info/PKG-INFO` & `certify4py-0.1.6/src/certify4py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: certify4py
-Version: 0.1.5
+Version: 0.1.6
 Summary: Issue certificates using blockchain and smart contract
 Home-page: https://github.com/teo-mn/certify4py
 Author: Surenbayar Doloonjin
 Author-email: surenbayar@teo.mn
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/teo-mn/certify4py/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.6,<3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Certify4py 
 Certify4py нь цахим сертификат, дипломыг блокчэйн дээр
 баталгаажуулж өгөх https://github.com/teo-mn/certify-sc ухаалаг гэрээтэй харьцдаг python хэлний сан юм.
 Уг ухаалаг гэрээ нь ИДС-ын дипломыг блокчэйнд баталгаажуулах стандарт бөгөөд дэлгэрэнгүйг дээрх линкээс харна уу.
```

