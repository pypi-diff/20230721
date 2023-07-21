# Comparing `tmp/aws_recommendation-0.2.6.tar.gz` & `tmp/aws_recommendation-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_recommendation-0.2.6.tar", last modified: Thu Jul 13 04:22:49 2023, max compression
+gzip compressed data, was "aws_recommendation-0.2.7.tar", last modified: Fri Jul 21 05:14:41 2023, max compression
```

## Comparing `aws_recommendation-0.2.6.tar` & `aws_recommendation-0.2.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 04:22:49.647840 aws_recommendation-0.2.6/
--rw-rw-rw-   0        0        0        0 2022-11-22 10:22:06.000000 aws_recommendation-0.2.6/LICENCE
--rw-rw-rw-   0        0        0     1220 2023-07-13 04:22:49.646837 aws_recommendation-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      868 2023-04-04 11:43:43.000000 aws_recommendation-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 04:22:49.628540 aws_recommendation-0.2.6/aws_recommendation/
--rw-rw-rw-   0        0        0     2329 2023-07-13 04:20:27.000000 aws_recommendation-0.2.6/aws_recommendation/__init__.py
--rw-rw-rw-   0        0        0     5487 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/cloudwatch.py
--rw-rw-rw-   0        0        0    11861 2023-07-13 04:02:57.000000 aws_recommendation-0.2.6/aws_recommendation/cost_estimations.py
--rw-rw-rw-   0        0        0     4296 2023-07-12 09:59:38.000000 aws_recommendation-0.2.6/aws_recommendation/dynamodb.py
--rw-rw-rw-   0        0        0    15213 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/ebs.py
--rw-rw-rw-   0        0        0    26661 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/ec2.py
--rw-rw-rw-   0        0        0     8961 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/elb.py
--rw-rw-rw-   0        0        0     4208 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/kms.py
--rw-rw-rw-   0        0        0    11638 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/rds.py
--rw-rw-rw-   0        0        0     5955 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/redshift.py
--rw-rw-rw-   0        0        0    11003 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/s3.py
--rw-rw-rw-   0        0        0     1726 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/truted_advisor.py
--rw-rw-rw-   0        0        0     5821 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-13 04:22:49.642866 aws_recommendation-0.2.6/aws_recommendation.egg-info/
--rw-rw-rw-   0        0        0     1220 2023-07-13 04:22:49.000000 aws_recommendation-0.2.6/aws_recommendation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      626 2023-07-13 04:22:49.000000 aws_recommendation-0.2.6/aws_recommendation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 04:22:49.000000 aws_recommendation-0.2.6/aws_recommendation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-13 04:22:49.000000 aws_recommendation-0.2.6/aws_recommendation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-13 04:22:49.000000 aws_recommendation-0.2.6/aws_recommendation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      525 2023-07-13 04:20:27.000000 aws_recommendation-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-13 04:22:49.648356 aws_recommendation-0.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-21 05:14:41.075827 aws_recommendation-0.2.7/
+-rw-rw-rw-   0        0        0        0 2022-11-22 10:22:06.000000 aws_recommendation-0.2.7/LICENCE
+-rw-rw-rw-   0        0        0     1220 2023-07-21 05:14:41.074826 aws_recommendation-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      868 2023-04-04 11:43:43.000000 aws_recommendation-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 05:14:41.056557 aws_recommendation-0.2.7/aws_recommendation/
+-rw-rw-rw-   0        0        0     2329 2023-07-21 05:14:13.000000 aws_recommendation-0.2.7/aws_recommendation/__init__.py
+-rw-rw-rw-   0        0        0     5487 2023-04-12 12:09:37.000000 aws_recommendation-0.2.7/aws_recommendation/cloudwatch.py
+-rw-rw-rw-   0        0        0    11861 2023-07-13 04:02:57.000000 aws_recommendation-0.2.7/aws_recommendation/cost_estimations.py
+-rw-rw-rw-   0        0        0     4296 2023-07-12 09:59:38.000000 aws_recommendation-0.2.7/aws_recommendation/dynamodb.py
+-rw-rw-rw-   0        0        0    15213 2023-04-12 12:09:37.000000 aws_recommendation-0.2.7/aws_recommendation/ebs.py
+-rw-rw-rw-   0        0        0    26661 2023-04-12 12:09:37.000000 aws_recommendation-0.2.7/aws_recommendation/ec2.py
+-rw-rw-rw-   0        0        0     8961 2023-04-12 12:09:37.000000 aws_recommendation-0.2.7/aws_recommendation/elb.py
+-rw-rw-rw-   0        0        0     4208 2023-04-12 12:09:37.000000 aws_recommendation-0.2.7/aws_recommendation/kms.py
+-rw-rw-rw-   0        0        0    11638 2023-04-12 12:09:37.000000 aws_recommendation-0.2.7/aws_recommendation/rds.py
+-rw-rw-rw-   0        0        0     5955 2023-04-12 12:09:37.000000 aws_recommendation-0.2.7/aws_recommendation/redshift.py
+-rw-rw-rw-   0        0        0    10955 2023-07-21 05:14:13.000000 aws_recommendation-0.2.7/aws_recommendation/s3.py
+-rw-rw-rw-   0        0        0     1726 2023-04-12 12:09:37.000000 aws_recommendation-0.2.7/aws_recommendation/truted_advisor.py
+-rw-rw-rw-   0        0        0     5821 2023-04-12 12:09:37.000000 aws_recommendation-0.2.7/aws_recommendation/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 05:14:41.071828 aws_recommendation-0.2.7/aws_recommendation.egg-info/
+-rw-rw-rw-   0        0        0     1220 2023-07-21 05:14:40.000000 aws_recommendation-0.2.7/aws_recommendation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      626 2023-07-21 05:14:40.000000 aws_recommendation-0.2.7/aws_recommendation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 05:14:40.000000 aws_recommendation-0.2.7/aws_recommendation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-21 05:14:40.000000 aws_recommendation-0.2.7/aws_recommendation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-21 05:14:40.000000 aws_recommendation-0.2.7/aws_recommendation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      525 2023-07-21 05:14:13.000000 aws_recommendation-0.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-21 05:14:41.075827 aws_recommendation-0.2.7/setup.cfg
```

### Comparing `aws_recommendation-0.2.6/PKG-INFO` & `aws_recommendation-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_recommendation
-Version: 0.2.6
+Version: 0.2.7
 Summary: Provides AWS recommendations
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `aws_recommendation-0.2.6/README.md` & `aws_recommendation-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.6/aws_recommendation/__init__.py` & `aws_recommendation-0.2.7/aws_recommendation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Any
 
 from botocore.exceptions import ClientError
 
 from boto3 import session
 
 __author__ = "Dheeraj Banodha"
-__version__ = '0.2.6'
+__version__ = '0.2.7'
 
 import logging
 
 from aws_recommendation.cloudwatch import cloudwatch
 from aws_recommendation.dynamodb import dynamodb
 from aws_recommendation.ebs import ebs
 from aws_recommendation.ec2 import ec2
```

### Comparing `aws_recommendation-0.2.6/aws_recommendation/cloudwatch.py` & `aws_recommendation-0.2.7/aws_recommendation/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.6/aws_recommendation/cost_estimations.py` & `aws_recommendation-0.2.7/aws_recommendation/cost_estimations.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.6/aws_recommendation/dynamodb.py` & `aws_recommendation-0.2.7/aws_recommendation/dynamodb.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.6/aws_recommendation/ebs.py` & `aws_recommendation-0.2.7/aws_recommendation/ebs.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.6/aws_recommendation/ec2.py` & `aws_recommendation-0.2.7/aws_recommendation/ec2.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.6/aws_recommendation/elb.py` & `aws_recommendation-0.2.7/aws_recommendation/elb.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.6/aws_recommendation/kms.py` & `aws_recommendation-0.2.7/aws_recommendation/kms.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.6/aws_recommendation/rds.py` & `aws_recommendation-0.2.7/aws_recommendation/rds.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.6/aws_recommendation/redshift.py` & `aws_recommendation-0.2.7/aws_recommendation/redshift.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.6/aws_recommendation/s3.py` & `aws_recommendation-0.2.7/aws_recommendation/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                     logger.info('---------S3 read access denied----------')
                     temp = {
                         'Service Name': 'S3',
                         'Id': bucket['Name'],
                         'Recommendation': 'Access Denied',
                         'Description': 'Access Denied',
                         'Metadata': {
-                            'Exception': str(traceback.format_exc())
+                            'Access Denied'
                         },
                         'Recommendation Reason': {
                             'Access Denied'
                         },
                         'Risk': 'Low',
                         'Savings': None,
                         'Source': 'Klera',
@@ -118,15 +118,15 @@
                     logger.info('---------S3 read access denied----------')
                     temp = {
                         'Service Name': 'S3',
                         'Id': 'Access Denied',
                         'Recommendation': 'Access Denied',
                         'Description': 'Access Denied',
                         'Metadata': {
-                            'Exception': str(traceback.format_exc())
+                            'Access Denied'
                         },
                         'Recommendation Reason': {
                             'Access Denied'
                         },
                         'Risk': 'Low',
                         'Savings': None,
                         'Source': 'Klera',
@@ -245,15 +245,15 @@
                     logger.info('---------S3 read access denied----------')
                     temp = {
                         'Service Name': 'S3',
                         'Id': 'Access Denied',
                         'Recommendation': 'Access Denied',
                         'Description': 'Access Denied',
                         'Metadata': {
-                            'Exception': str(traceback.format_exc())
+                            # 'Exception': str(traceback.format_exc())
                         },
                         'Recommendation Reason': {
                             'Access Denied'
                         },
                         'Risk': 'Low',
                         'Savings': None,
                         'Source': 'Klera',
```

### Comparing `aws_recommendation-0.2.6/aws_recommendation/truted_advisor.py` & `aws_recommendation-0.2.7/aws_recommendation/truted_advisor.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.6/aws_recommendation/utils.py` & `aws_recommendation-0.2.7/aws_recommendation/utils.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.6/aws_recommendation.egg-info/PKG-INFO` & `aws_recommendation-0.2.7/aws_recommendation.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-recommendation
-Version: 0.2.6
+Version: 0.2.7
 Summary: Provides AWS recommendations
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `aws_recommendation-0.2.6/aws_recommendation.egg-info/SOURCES.txt` & `aws_recommendation-0.2.7/aws_recommendation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.6/pyproject.toml` & `aws_recommendation-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aws_recommendation"
-version = "0.2.6"
+version = "0.2.7"
 authors = [
   { name="dheeraj.banodha", email="dheerajmbanodha@gmail.com" },
 ]
 description = "Provides AWS recommendations"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

