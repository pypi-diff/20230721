# Comparing `tmp/pymoises-1.0.0.tar.gz` & `tmp/pymoises-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymoises-1.0.0.tar", last modified: Thu Jul 20 23:25:44 2023, max compression
+gzip compressed data, was "pymoises-1.0.1.tar", last modified: Fri Jul 21 17:35:27 2023, max compression
```

## Comparing `pymoises-1.0.0.tar` & `pymoises-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-20 23:25:44.763238 pymoises-1.0.0/
--rw-r--r--   0 bryan     (1000) bryan     (1000)      176 2023-07-20 23:25:44.753238 pymoises-1.0.0/PKG-INFO
--rw-r--r--   0 bryan     (1000) bryan     (1000)       12 2023-07-20 18:30:18.000000 pymoises-1.0.0/README.md
-drwxr-xr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-20 23:25:44.743238 pymoises-1.0.0/pymoises/
--rw-r--r--   0 bryan     (1000) bryan     (1000)     1872 2023-07-20 18:30:18.000000 pymoises-1.0.0/pymoises/Transactions.py
--rw-r--r--   0 bryan     (1000) bryan     (1000)       69 2023-07-20 18:30:18.000000 pymoises-1.0.0/pymoises/__init__.py
--rw-r--r--   0 bryan     (1000) bryan     (1000)     4149 2023-07-20 18:30:18.000000 pymoises-1.0.0/pymoises/customer.py
-drwxr-xr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-20 23:25:44.753238 pymoises-1.0.0/pymoises/dto/
--rw-r--r--   0 bryan     (1000) bryan     (1000)       42 2023-07-20 18:30:18.000000 pymoises-1.0.0/pymoises/dto/__init__.py
-drwxr-xr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-20 23:25:44.753238 pymoises-1.0.0/pymoises/dto/input/
--rw-r--r--   0 bryan     (1000) bryan     (1000)       51 2023-07-20 18:30:18.000000 pymoises-1.0.0/pymoises/dto/input/__init__.py
-drwxr-xr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-20 23:25:44.753238 pymoises-1.0.0/pymoises/dto/input/customer/
--rw-r--r--   0 bryan     (1000) bryan     (1000)       49 2023-07-20 18:30:18.000000 pymoises-1.0.0/pymoises/dto/input/customer/__init__.py
--rw-r--r--   0 bryan     (1000) bryan     (1000)      516 2023-07-20 18:30:18.000000 pymoises-1.0.0/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py
-drwxr-xr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-20 23:25:44.753238 pymoises-1.0.0/pymoises/dto/input/transaction/
--rw-r--r--   0 bryan     (1000) bryan     (1000)       43 2023-07-20 18:30:18.000000 pymoises-1.0.0/pymoises/dto/input/transaction/__init__.py
--rw-r--r--   0 bryan     (1000) bryan     (1000)      509 2023-07-20 18:30:18.000000 pymoises-1.0.0/pymoises/dto/input/transaction/create_transaction_input_dto.py
-drwxr-xr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-20 23:25:44.753238 pymoises-1.0.0/pymoises/dto/output/
--rw-r--r--   0 bryan     (1000) bryan     (1000)       50 2023-07-20 18:30:18.000000 pymoises-1.0.0/pymoises/dto/output/__init__.py
-drwxr-xr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-20 23:25:44.753238 pymoises-1.0.0/pymoises/dto/output/customer/
--rw-r--r--   0 bryan     (1000) bryan     (1000)       34 2023-07-20 18:30:18.000000 pymoises-1.0.0/pymoises/dto/output/customer/__init__.py
--rw-r--r--   0 bryan     (1000) bryan     (1000)     1159 2023-07-20 18:30:18.000000 pymoises-1.0.0/pymoises/dto/output/customer/customer_output_dto.py
-drwxr-xr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-20 23:25:44.753238 pymoises-1.0.0/pymoises/dto/output/transaction/
--rw-r--r--   0 bryan     (1000) bryan     (1000)       37 2023-07-20 18:30:18.000000 pymoises-1.0.0/pymoises/dto/output/transaction/__init__.py
--rw-r--r--   0 bryan     (1000) bryan     (1000)      538 2023-07-20 18:30:18.000000 pymoises-1.0.0/pymoises/dto/output/transaction/transaction_output_dto.py
-drwxr-xr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-20 23:25:44.753238 pymoises-1.0.0/pymoises.egg-info/
--rw-r--r--   0 bryan     (1000) bryan     (1000)      176 2023-07-20 23:25:44.000000 pymoises-1.0.0/pymoises.egg-info/PKG-INFO
--rw-r--r--   0 bryan     (1000) bryan     (1000)      739 2023-07-20 23:25:44.000000 pymoises-1.0.0/pymoises.egg-info/SOURCES.txt
--rw-r--r--   0 bryan     (1000) bryan     (1000)        1 2023-07-20 23:25:44.000000 pymoises-1.0.0/pymoises.egg-info/dependency_links.txt
--rw-r--r--   0 bryan     (1000) bryan     (1000)       21 2023-07-20 23:25:44.000000 pymoises-1.0.0/pymoises.egg-info/requires.txt
--rw-r--r--   0 bryan     (1000) bryan     (1000)        9 2023-07-20 23:25:44.000000 pymoises-1.0.0/pymoises.egg-info/top_level.txt
--rw-r--r--   0 bryan     (1000) bryan     (1000)       38 2023-07-20 23:25:44.763238 pymoises-1.0.0/setup.cfg
--rw-r--r--   0 bryan     (1000) bryan     (1000)      496 2023-07-20 23:24:17.000000 pymoises-1.0.0/setup.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.361974 pymoises-1.0.1/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      176 2023-07-21 17:35:27.361974 pymoises-1.0.1/PKG-INFO
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       12 2023-06-28 15:16:17.000000 pymoises-1.0.1/README.md
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.357974 pymoises-1.0.1/pymoises/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1872 2023-06-28 19:09:41.000000 pymoises-1.0.1/pymoises/Transactions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       69 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     6731 2023-07-17 16:20:39.000000 pymoises-1.0.1/pymoises/customer.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.357974 pymoises-1.0.1/pymoises/dto/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       42 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/__init__.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.357974 pymoises-1.0.1/pymoises/dto/input/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       51 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/input/__init__.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.357974 pymoises-1.0.1/pymoises/dto/input/customer/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       49 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/input/customer/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      516 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.361974 pymoises-1.0.1/pymoises/dto/input/transaction/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       43 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/input/transaction/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      509 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/input/transaction/create_transaction_input_dto.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.361974 pymoises-1.0.1/pymoises/dto/output/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       50 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/output/__init__.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.361974 pymoises-1.0.1/pymoises/dto/output/customer/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       69 2023-07-17 15:32:32.000000 pymoises-1.0.1/pymoises/dto/output/customer/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1159 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/output/customer/customer_output_dto.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      907 2023-07-17 15:29:47.000000 pymoises-1.0.1/pymoises/dto/output/customer/moveLead_output_dto.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.361974 pymoises-1.0.1/pymoises/dto/output/transaction/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       37 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/output/transaction/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      538 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/output/transaction/transaction_output_dto.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.357974 pymoises-1.0.1/pymoises.egg-info/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      176 2023-07-21 17:35:27.000000 pymoises-1.0.1/pymoises.egg-info/PKG-INFO
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      791 2023-07-21 17:35:27.000000 pymoises-1.0.1/pymoises.egg-info/SOURCES.txt
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)        1 2023-07-21 17:35:27.000000 pymoises-1.0.1/pymoises.egg-info/dependency_links.txt
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       21 2023-07-21 17:35:27.000000 pymoises-1.0.1/pymoises.egg-info/requires.txt
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)        9 2023-07-21 17:35:27.000000 pymoises-1.0.1/pymoises.egg-info/top_level.txt
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       38 2023-07-21 17:35:27.361974 pymoises-1.0.1/setup.cfg
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      504 2023-07-21 17:35:06.000000 pymoises-1.0.1/setup.py
```

### Comparing `pymoises-1.0.0/pymoises/Transactions.py` & `pymoises-1.0.1/pymoises/Transactions.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.0/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py` & `pymoises-1.0.1/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.0/pymoises/dto/output/customer/customer_output_dto.py` & `pymoises-1.0.1/pymoises/dto/output/customer/customer_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.0/pymoises/dto/output/transaction/transaction_output_dto.py` & `pymoises-1.0.1/pymoises/dto/output/transaction/transaction_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.0/pymoises.egg-info/SOURCES.txt` & `pymoises-1.0.1/pymoises.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,9 +13,10 @@
 pymoises/dto/input/customer/__init__.py
 pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py
 pymoises/dto/input/transaction/__init__.py
 pymoises/dto/input/transaction/create_transaction_input_dto.py
 pymoises/dto/output/__init__.py
 pymoises/dto/output/customer/__init__.py
 pymoises/dto/output/customer/customer_output_dto.py
+pymoises/dto/output/customer/moveLead_output_dto.py
 pymoises/dto/output/transaction/__init__.py
 pymoises/dto/output/transaction/transaction_output_dto.py
```

