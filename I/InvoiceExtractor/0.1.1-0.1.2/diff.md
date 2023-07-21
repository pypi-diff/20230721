# Comparing `tmp/InvoiceExtractor-0.1.1.tar.gz` & `tmp/InvoiceExtractor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InvoiceExtractor-0.1.1.tar", last modified: Fri Jul 21 15:40:35 2023, max compression
+gzip compressed data, was "InvoiceExtractor-0.1.2.tar", last modified: Fri Jul 21 16:07:34 2023, max compression
```

## Comparing `InvoiceExtractor-0.1.1.tar` & `InvoiceExtractor-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 aybarsb    (501) staff       (20)        0 2023-07-21 15:40:35.725087 InvoiceExtractor-0.1.1/
-drwxr-xr-x   0 aybarsb    (501) staff       (20)        0 2023-07-21 15:40:35.723879 InvoiceExtractor-0.1.1/InvoiceExtractor.egg-info/
--rw-r--r--   0 aybarsb    (501) staff       (20)     4453 2023-07-21 15:40:35.000000 InvoiceExtractor-0.1.1/InvoiceExtractor.egg-info/PKG-INFO
--rw-r--r--   0 aybarsb    (501) staff       (20)      345 2023-07-21 15:40:35.000000 InvoiceExtractor-0.1.1/InvoiceExtractor.egg-info/SOURCES.txt
--rw-r--r--   0 aybarsb    (501) staff       (20)        1 2023-07-21 15:40:35.000000 InvoiceExtractor-0.1.1/InvoiceExtractor.egg-info/dependency_links.txt
--rw-r--r--   0 aybarsb    (501) staff       (20)       65 2023-07-21 15:40:35.000000 InvoiceExtractor-0.1.1/InvoiceExtractor.egg-info/entry_points.txt
--rw-r--r--   0 aybarsb    (501) staff       (20)      120 2023-07-21 15:40:35.000000 InvoiceExtractor-0.1.1/InvoiceExtractor.egg-info/requires.txt
--rw-r--r--   0 aybarsb    (501) staff       (20)       18 2023-07-21 15:40:35.000000 InvoiceExtractor-0.1.1/InvoiceExtractor.egg-info/top_level.txt
--rw-r--r--   0 aybarsb    (501) staff       (20)     4453 2023-07-21 15:40:35.724954 InvoiceExtractor-0.1.1/PKG-INFO
--rw-r--r--   0 aybarsb    (501) staff       (20)     4217 2023-07-21 15:24:54.000000 InvoiceExtractor-0.1.1/README.md
-drwxr-xr-x   0 aybarsb    (501) staff       (20)        0 2023-07-21 15:40:35.724632 InvoiceExtractor-0.1.1/invoice_extractor/
--rw-r--r--   0 aybarsb    (501) staff       (20)        1 2023-07-21 13:15:27.000000 InvoiceExtractor-0.1.1/invoice_extractor/__init__.py
--rw-r--r--   0 aybarsb    (501) staff       (20)     2826 2023-07-21 11:15:30.000000 InvoiceExtractor-0.1.1/invoice_extractor/extract.py
--rw-r--r--   0 aybarsb    (501) staff       (20)     4957 2023-07-21 15:16:43.000000 InvoiceExtractor-0.1.1/invoice_extractor/main.py
--rw-r--r--   0 aybarsb    (501) staff       (20)       38 2023-07-21 15:40:35.725123 InvoiceExtractor-0.1.1/setup.cfg
--rw-r--r--   0 aybarsb    (501) staff       (20)      797 2023-07-21 15:40:33.000000 InvoiceExtractor-0.1.1/setup.py
+drwxr-xr-x   0 aybarsb    (501) staff       (20)        0 2023-07-21 16:07:34.201028 InvoiceExtractor-0.1.2/
+drwxr-xr-x   0 aybarsb    (501) staff       (20)        0 2023-07-21 16:07:34.200146 InvoiceExtractor-0.1.2/InvoiceExtractor.egg-info/
+-rw-r--r--   0 aybarsb    (501) staff       (20)     4453 2023-07-21 16:07:34.000000 InvoiceExtractor-0.1.2/InvoiceExtractor.egg-info/PKG-INFO
+-rw-r--r--   0 aybarsb    (501) staff       (20)      355 2023-07-21 16:07:34.000000 InvoiceExtractor-0.1.2/InvoiceExtractor.egg-info/SOURCES.txt
+-rw-r--r--   0 aybarsb    (501) staff       (20)        1 2023-07-21 16:07:34.000000 InvoiceExtractor-0.1.2/InvoiceExtractor.egg-info/dependency_links.txt
+-rw-r--r--   0 aybarsb    (501) staff       (20)       65 2023-07-21 16:07:34.000000 InvoiceExtractor-0.1.2/InvoiceExtractor.egg-info/entry_points.txt
+-rw-r--r--   0 aybarsb    (501) staff       (20)      120 2023-07-21 16:07:34.000000 InvoiceExtractor-0.1.2/InvoiceExtractor.egg-info/requires.txt
+-rw-r--r--   0 aybarsb    (501) staff       (20)       18 2023-07-21 16:07:34.000000 InvoiceExtractor-0.1.2/InvoiceExtractor.egg-info/top_level.txt
+-rw-r--r--   0 aybarsb    (501) staff       (20)     4453 2023-07-21 16:07:34.201095 InvoiceExtractor-0.1.2/PKG-INFO
+-rw-r--r--   0 aybarsb    (501) staff       (20)     4217 2023-07-21 15:24:54.000000 InvoiceExtractor-0.1.2/README.md
+drwxr-xr-x   0 aybarsb    (501) staff       (20)        0 2023-07-21 16:07:34.200802 InvoiceExtractor-0.1.2/invoice_extractor/
+-rw-r--r--   0 aybarsb    (501) staff       (20)        1 2023-07-21 13:15:27.000000 InvoiceExtractor-0.1.2/invoice_extractor/__init__.py
+-rw-r--r--   0 aybarsb    (501) staff       (20)     2826 2023-07-21 11:15:30.000000 InvoiceExtractor-0.1.2/invoice_extractor/extract.py
+-rw-r--r--   0 aybarsb    (501) staff       (20)     4957 2023-07-21 15:16:43.000000 InvoiceExtractor-0.1.2/invoice_extractor/main.py
+-rw-r--r--   0 aybarsb    (501) staff       (20)       91 2023-07-21 16:07:34.201339 InvoiceExtractor-0.1.2/setup.cfg
+-rw-r--r--   0 aybarsb    (501) staff       (20)      827 2023-07-21 16:07:20.000000 InvoiceExtractor-0.1.2/setup.py
```

### Comparing `InvoiceExtractor-0.1.1/InvoiceExtractor.egg-info/PKG-INFO` & `InvoiceExtractor-0.1.2/InvoiceExtractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InvoiceExtractor
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for extracting data from invoices.
 Home-page: https://github.com/ybrs/invoice-extractor
 Author: Aybars Badur
 Description-Content-Type: text/markdown
 
 # Invoice Extractor
```

### Comparing `InvoiceExtractor-0.1.1/PKG-INFO` & `InvoiceExtractor-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InvoiceExtractor
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for extracting data from invoices.
 Home-page: https://github.com/ybrs/invoice-extractor
 Author: Aybars Badur
 Description-Content-Type: text/markdown
 
 # Invoice Extractor
```

### Comparing `InvoiceExtractor-0.1.1/README.md` & `InvoiceExtractor-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `InvoiceExtractor-0.1.1/invoice_extractor/extract.py` & `InvoiceExtractor-0.1.2/invoice_extractor/extract.py`

 * *Files identical despite different names*

### Comparing `InvoiceExtractor-0.1.1/invoice_extractor/main.py` & `InvoiceExtractor-0.1.2/invoice_extractor/main.py`

 * *Files identical despite different names*

### Comparing `InvoiceExtractor-0.1.1/setup.py` & `InvoiceExtractor-0.1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from setuptools import setup, find_packages
 
-# Read the dependencies from requirements.txt
-with open('requirements.txt', 'r') as file:
-    install_requires = file.read().splitlines()
+install_requires = """
+pdfplumber==0.10.1
+langchain==0.0.238
+openai==0.27.8
+pdfplumber==0.10.1
+pdfminer==20191125
+click==8.1.6
+openpyxl==3.1.2
+""".strip().splitlines()
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='InvoiceExtractor',
-    version='0.1.1',
+    version='0.1.2',
     author='Aybars Badur',
     include_package_data=True,
     description='A Python package for extracting data from invoices.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ybrs/invoice-extractor',
     packages=find_packages(),
```

