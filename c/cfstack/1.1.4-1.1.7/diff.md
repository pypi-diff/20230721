# Comparing `tmp/cfstack-1.1.4.tar.gz` & `tmp/cfstack-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfstack-1.1.4.tar", last modified: Thu Jul 20 20:08:39 2023, max compression
+gzip compressed data, was "cfstack-1.1.7.tar", last modified: Fri Jul 21 07:55:04 2023, max compression
```

## Comparing `cfstack-1.1.4.tar` & `cfstack-1.1.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 20:08:39.586564 cfstack-1.1.4/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)    35149 2023-07-18 17:43:42.000000 cfstack-1.1.4/LICENSE
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      406 2023-07-20 20:08:39.586564 cfstack-1.1.4/PKG-INFO
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)       38 2023-07-20 20:08:39.586564 cfstack-1.1.4/setup.cfg
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      581 2023-07-20 20:08:38.000000 cfstack-1.1.4/setup.py
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 20:08:39.582564 cfstack-1.1.4/src/
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 20:08:39.582564 cfstack-1.1.4/src/cfstack/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)       37 2023-07-19 16:32:24.000000 cfstack-1.1.4/src/cfstack/__init__.py
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 20:08:39.582564 cfstack-1.1.4/src/cfstack/changeset/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      141 2023-07-19 16:52:23.000000 cfstack-1.1.4/src/cfstack/changeset/__init__.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      687 2023-07-20 19:42:36.000000 cfstack-1.1.4/src/cfstack/changeset/check_changeset_status.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1170 2023-07-18 17:43:42.000000 cfstack-1.1.4/src/cfstack/changeset/create_changeset.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      364 2023-07-18 17:43:42.000000 cfstack-1.1.4/src/cfstack/changeset/delete_changeset.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      371 2023-07-18 17:43:42.000000 cfstack-1.1.4/src/cfstack/changeset/execute_changeset.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      332 2023-07-18 17:43:42.000000 cfstack-1.1.4/src/cfstack/changeset/generate_changesetname.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     5364 2023-07-20 20:08:25.000000 cfstack-1.1.4/src/cfstack/execute.py
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 20:08:39.582564 cfstack-1.1.4/src/cfstack/s3utility/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)       93 2023-07-19 16:52:54.000000 cfstack-1.1.4/src/cfstack/s3utility/__init__.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      126 2023-07-18 17:43:42.000000 cfstack-1.1.4/src/cfstack/s3utility/create_client.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      572 2023-07-18 17:43:42.000000 cfstack-1.1.4/src/cfstack/s3utility/delete_file_s3.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      523 2023-07-18 17:43:42.000000 cfstack-1.1.4/src/cfstack/s3utility/read_file_s3.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      720 2023-07-18 17:43:42.000000 cfstack-1.1.4/src/cfstack/s3utility/upload_file_s3.py
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 20:08:39.586564 cfstack-1.1.4/src/cfstack/stack/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      120 2023-07-19 16:53:56.000000 cfstack-1.1.4/src/cfstack/stack/__init__.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1067 2023-07-18 17:43:42.000000 cfstack-1.1.4/src/cfstack/stack/check_stack_delete_status.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      470 2023-07-18 17:43:42.000000 cfstack-1.1.4/src/cfstack/stack/check_stack_exists.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1049 2023-07-18 17:43:42.000000 cfstack-1.1.4/src/cfstack/stack/check_stack_update_status.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      392 2023-07-18 17:43:42.000000 cfstack-1.1.4/src/cfstack/stack/delete_stack.py
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 20:08:39.586564 cfstack-1.1.4/src/cfstack/utility/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      194 2023-07-19 16:54:47.000000 cfstack-1.1.4/src/cfstack/utility/__init__.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      955 2023-07-18 17:43:42.000000 cfstack-1.1.4/src/cfstack/utility/calculate_shamap.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1392 2023-07-18 17:43:42.000000 cfstack-1.1.4/src/cfstack/utility/compare_shamap.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      136 2023-07-18 17:43:42.000000 cfstack-1.1.4/src/cfstack/utility/create_client.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      949 2023-07-19 17:43:05.000000 cfstack-1.1.4/src/cfstack/utility/execute_delete.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1839 2023-07-20 19:43:33.000000 cfstack-1.1.4/src/cfstack/utility/execute_deploy.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1980 2023-07-18 17:43:42.000000 cfstack-1.1.4/src/cfstack/utility/first_time_upload.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      297 2023-07-18 17:43:42.000000 cfstack-1.1.4/src/cfstack/utility/parameter_preprocessing.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      917 2023-07-18 17:43:42.000000 cfstack-1.1.4/src/cfstack/utility/upload_template_s3.py
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 20:08:39.582564 cfstack-1.1.4/src/cfstack.egg-info/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      406 2023-07-20 20:08:39.000000 cfstack-1.1.4/src/cfstack.egg-info/PKG-INFO
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1236 2023-07-20 20:08:39.000000 cfstack-1.1.4/src/cfstack.egg-info/SOURCES.txt
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)        1 2023-07-20 20:08:39.000000 cfstack-1.1.4/src/cfstack.egg-info/dependency_links.txt
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)        6 2023-07-20 20:08:39.000000 cfstack-1.1.4/src/cfstack.egg-info/requires.txt
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)        8 2023-07-20 20:08:39.000000 cfstack-1.1.4/src/cfstack.egg-info/top_level.txt
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-21 07:55:04.865351 cfstack-1.1.7/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)    35149 2023-07-18 17:43:42.000000 cfstack-1.1.7/LICENSE
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      406 2023-07-21 07:55:04.865351 cfstack-1.1.7/PKG-INFO
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)       38 2023-07-21 07:55:04.865351 cfstack-1.1.7/setup.cfg
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      581 2023-07-21 07:54:31.000000 cfstack-1.1.7/setup.py
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-21 07:55:04.861350 cfstack-1.1.7/src/
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-21 07:55:04.861350 cfstack-1.1.7/src/cfstack/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)       37 2023-07-19 16:32:24.000000 cfstack-1.1.7/src/cfstack/__init__.py
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-21 07:55:04.865351 cfstack-1.1.7/src/cfstack/changeset/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      141 2023-07-19 16:52:23.000000 cfstack-1.1.7/src/cfstack/changeset/__init__.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      687 2023-07-20 19:42:36.000000 cfstack-1.1.7/src/cfstack/changeset/check_changeset_status.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1170 2023-07-18 17:43:42.000000 cfstack-1.1.7/src/cfstack/changeset/create_changeset.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      364 2023-07-18 17:43:42.000000 cfstack-1.1.7/src/cfstack/changeset/delete_changeset.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      371 2023-07-18 17:43:42.000000 cfstack-1.1.7/src/cfstack/changeset/execute_changeset.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      332 2023-07-18 17:43:42.000000 cfstack-1.1.7/src/cfstack/changeset/generate_changesetname.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     5331 2023-07-21 07:46:13.000000 cfstack-1.1.7/src/cfstack/execute.py
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-21 07:55:04.865351 cfstack-1.1.7/src/cfstack/s3utility/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)       93 2023-07-19 16:52:54.000000 cfstack-1.1.7/src/cfstack/s3utility/__init__.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      126 2023-07-18 17:43:42.000000 cfstack-1.1.7/src/cfstack/s3utility/create_client.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      572 2023-07-18 17:43:42.000000 cfstack-1.1.7/src/cfstack/s3utility/delete_file_s3.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      523 2023-07-18 17:43:42.000000 cfstack-1.1.7/src/cfstack/s3utility/read_file_s3.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      720 2023-07-18 17:43:42.000000 cfstack-1.1.7/src/cfstack/s3utility/upload_file_s3.py
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-21 07:55:04.865351 cfstack-1.1.7/src/cfstack/stack/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      120 2023-07-19 16:53:56.000000 cfstack-1.1.7/src/cfstack/stack/__init__.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1067 2023-07-18 17:43:42.000000 cfstack-1.1.7/src/cfstack/stack/check_stack_delete_status.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      470 2023-07-18 17:43:42.000000 cfstack-1.1.7/src/cfstack/stack/check_stack_exists.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1049 2023-07-18 17:43:42.000000 cfstack-1.1.7/src/cfstack/stack/check_stack_update_status.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      392 2023-07-18 17:43:42.000000 cfstack-1.1.7/src/cfstack/stack/delete_stack.py
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-21 07:55:04.865351 cfstack-1.1.7/src/cfstack/utility/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      194 2023-07-19 16:54:47.000000 cfstack-1.1.7/src/cfstack/utility/__init__.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      955 2023-07-18 17:43:42.000000 cfstack-1.1.7/src/cfstack/utility/calculate_shamap.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1392 2023-07-18 17:43:42.000000 cfstack-1.1.7/src/cfstack/utility/compare_shamap.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      136 2023-07-18 17:43:42.000000 cfstack-1.1.7/src/cfstack/utility/create_client.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      949 2023-07-19 17:43:05.000000 cfstack-1.1.7/src/cfstack/utility/execute_delete.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1839 2023-07-20 19:43:33.000000 cfstack-1.1.7/src/cfstack/utility/execute_deploy.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1980 2023-07-18 17:43:42.000000 cfstack-1.1.7/src/cfstack/utility/first_time_upload.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      297 2023-07-18 17:43:42.000000 cfstack-1.1.7/src/cfstack/utility/parameter_preprocessing.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      917 2023-07-18 17:43:42.000000 cfstack-1.1.7/src/cfstack/utility/upload_template_s3.py
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-21 07:55:04.865351 cfstack-1.1.7/src/cfstack.egg-info/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      406 2023-07-21 07:55:04.000000 cfstack-1.1.7/src/cfstack.egg-info/PKG-INFO
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1236 2023-07-21 07:55:04.000000 cfstack-1.1.7/src/cfstack.egg-info/SOURCES.txt
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)        1 2023-07-21 07:55:04.000000 cfstack-1.1.7/src/cfstack.egg-info/dependency_links.txt
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)        6 2023-07-21 07:55:04.000000 cfstack-1.1.7/src/cfstack.egg-info/requires.txt
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)        8 2023-07-21 07:55:04.000000 cfstack-1.1.7/src/cfstack.egg-info/top_level.txt
```

### Comparing `cfstack-1.1.4/LICENSE` & `cfstack-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.4/setup.py` & `cfstack-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open("src/README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='cfstack',
-    version='1.1.4',
+    version='1.1.7',
     description='A utility to manage CloudFormation stacks',
     packages=find_packages("src"),
     package_dir={"": "src"},
     install_requires=[
             "boto3"
     ],
     python_requires='>=3',
```

### Comparing `cfstack-1.1.4/src/cfstack/changeset/check_changeset_status.py` & `cfstack-1.1.7/src/cfstack/changeset/check_changeset_status.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.4/src/cfstack/changeset/create_changeset.py` & `cfstack-1.1.7/src/cfstack/changeset/create_changeset.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.4/src/cfstack/execute.py` & `cfstack-1.1.7/src/cfstack/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,9 +117,8 @@
             "FilePath":"prod_calc.json",
             "Key":"prod.json"   
         }
         upload_file_s3(s3client,prod_file_details,True)
     
     if no_change_instacks:
         print("No changes in any stack")
-    
-    return os._exit(status_code)
+
```

### Comparing `cfstack-1.1.4/src/cfstack/s3utility/delete_file_s3.py` & `cfstack-1.1.7/src/cfstack/s3utility/delete_file_s3.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.4/src/cfstack/s3utility/read_file_s3.py` & `cfstack-1.1.7/src/cfstack/s3utility/read_file_s3.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.4/src/cfstack/s3utility/upload_file_s3.py` & `cfstack-1.1.7/src/cfstack/s3utility/upload_file_s3.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.4/src/cfstack/stack/check_stack_delete_status.py` & `cfstack-1.1.7/src/cfstack/stack/check_stack_delete_status.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.4/src/cfstack/stack/check_stack_update_status.py` & `cfstack-1.1.7/src/cfstack/stack/check_stack_update_status.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.4/src/cfstack/utility/calculate_shamap.py` & `cfstack-1.1.7/src/cfstack/utility/calculate_shamap.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.4/src/cfstack/utility/compare_shamap.py` & `cfstack-1.1.7/src/cfstack/utility/compare_shamap.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.4/src/cfstack/utility/execute_delete.py` & `cfstack-1.1.7/src/cfstack/utility/execute_delete.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.4/src/cfstack/utility/execute_deploy.py` & `cfstack-1.1.7/src/cfstack/utility/execute_deploy.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.4/src/cfstack/utility/first_time_upload.py` & `cfstack-1.1.7/src/cfstack/utility/first_time_upload.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.4/src/cfstack/utility/upload_template_s3.py` & `cfstack-1.1.7/src/cfstack/utility/upload_template_s3.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.4/src/cfstack.egg-info/SOURCES.txt` & `cfstack-1.1.7/src/cfstack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

