# Comparing `tmp/alibabacloud-ros-iact3-0.1.1.tar.gz` & `tmp/alibabacloud-ros-iact3-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud-ros-iact3-0.1.1.tar", last modified: Tue Apr 11 11:58:48 2023, max compression
+gzip compressed data, was "dist/alibabacloud-ros-iact3-0.1.2.tar", last modified: Fri Jul 21 07:29:29 2023, max compression
```

## Comparing `alibabacloud-ros-iact3-0.1.1.tar` & `alibabacloud-ros-iact3-0.1.2.tar`

### file list

```diff
@@ -1,49 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/
--rw-r--r--   0 root         (0) root         (0)      111 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10291 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7604 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/alibabacloud_ros_iact3.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10291 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/alibabacloud_ros_iact3.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      932 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/alibabacloud_ros_iact3.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/alibabacloud_ros_iact3.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1448 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/alibabacloud_ros_iact3.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/alibabacloud_ros_iact3.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/bin/
--rwxr-xr-x   0 root         (0) root         (0)      450 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/bin/iact3
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/iact3/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10773 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/
--rw-r--r--   0 root         (0) root         (0)       96 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4177 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/base.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/delete.py
--rw-r--r--   0 root         (0) root         (0)     4439 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/list.py
--rw-r--r--   0 root         (0) root         (0)     4160 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/test.py
--rw-r--r--   0 root         (0) root         (0)    18319 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/config.py
--rw-r--r--   0 root         (0) root         (0)      521 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    16055 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/generate_params.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/logger.py
--rwxr-xr-x   0 root         (0) root         (0)     1590 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/iact3/plugin/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7940 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/plugin/base_plugin.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/plugin/ecs.py
--rw-r--r--   0 root         (0) root         (0)     1096 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/plugin/error_code.py
--rw-r--r--   0 root         (0) root         (0)     3550 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/plugin/oss.py
--rw-r--r--   0 root         (0) root         (0)     6683 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/plugin/ros.py
--rw-r--r--   0 root         (0) root         (0)     1074 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/plugin/vpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/iact3/report/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/report/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9475 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/report/generate_reports.py
--rw-r--r--   0 root         (0) root         (0)     3805 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/report/html.css
--rw-r--r--   0 root         (0) root         (0)    13220 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/stack.py
--rw-r--r--   0 root         (0) root         (0)     3309 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/termial_print.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/iact3/testing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/testing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5916 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/testing/base.py
--rw-r--r--   0 root         (0) root         (0)     1356 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/testing/ros_stack.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/util.py
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)     1448 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1230 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10291 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7604 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/alibabacloud_ros_iact3.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10291 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/alibabacloud_ros_iact3.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/alibabacloud_ros_iact3.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/alibabacloud_ros_iact3.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/alibabacloud_ros_iact3.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/alibabacloud_ros_iact3.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/bin/
+-rwxr-xr-x   0 root         (0) root         (0)      450 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/bin/iact3
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10773 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/cli_modules/
+-rw-r--r--   0 root         (0) root         (0)      205 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/cli_modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4177 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/cli_modules/base.py
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/cli_modules/cost.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/cli_modules/delete.py
+-rw-r--r--   0 root         (0) root         (0)     4439 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/cli_modules/list.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/cli_modules/policy.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/cli_modules/preview.py
+-rw-r--r--   0 root         (0) root         (0)     4292 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/cli_modules/test.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/cli_modules/validate.py
+-rw-r--r--   0 root         (0) root         (0)    18487 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/config.py
+-rw-r--r--   0 root         (0) root         (0)      521 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    16055 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/generate_params.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/logger.py
+-rwxr-xr-x   0 root         (0) root         (0)     1590 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/plugin/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8040 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/plugin/base_plugin.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/plugin/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/plugin/error_code.py
+-rw-r--r--   0 root         (0) root         (0)     3550 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/plugin/oss.py
+-rw-r--r--   0 root         (0) root         (0)     8547 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/plugin/ros.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/plugin/vpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/report/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/report/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13884 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/report/generate_reports.py
+-rw-r--r--   0 root         (0) root         (0)     3805 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/report/html.css
+-rw-r--r--   0 root         (0) root         (0)    17804 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/stack.py
+-rw-r--r--   0 root         (0) root         (0)    13121 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/termial_print.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/testing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/testing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5951 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/testing/base.py
+-rw-r--r--   0 root         (0) root         (0)     2214 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/testing/ros_stack.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/iact3/util.py
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-07-21 07:29:29.000000 alibabacloud-ros-iact3-0.1.2/setup.py
```

### Comparing `alibabacloud-ros-iact3-0.1.1/PKG-INFO` & `alibabacloud-ros-iact3-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ros-iact3
-Version: 0.1.1
+Version: 0.1.2
 Summary: Iact3 is a tool that tests Terraform and ROS(Resource Orchestration Service) templates.
 Home-page: UNKNOWN
 Author: AlibabaCloud
 License: UNKNOWN
 Description: # What is iact3?
         
         Iact3(IaC Template Testing Tool) is a tool that tests [Terraform](https://developer.hashicorp.com/terraform) and [Alibaba Cloud ROS(Resource Orchestration Service)](https://www.alibabacloud.com/help/resource-orchestration-service) templates. It deploys your template in multiple Alibaba Cloud Regions and generates a report for each region via a simple configuration file.
```

### Comparing `alibabacloud-ros-iact3-0.1.1/README.md` & `alibabacloud-ros-iact3-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.1/alibabacloud_ros_iact3.egg-info/PKG-INFO` & `alibabacloud-ros-iact3-0.1.2/alibabacloud_ros_iact3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ros-iact3
-Version: 0.1.1
+Version: 0.1.2
 Summary: Iact3 is a tool that tests Terraform and ROS(Resource Orchestration Service) templates.
 Home-page: UNKNOWN
 Author: AlibabaCloud
 License: UNKNOWN
 Description: # What is iact3?
         
         Iact3(IaC Template Testing Tool) is a tool that tests [Terraform](https://developer.hashicorp.com/terraform) and [Alibaba Cloud ROS(Resource Orchestration Service)](https://www.alibabacloud.com/help/resource-orchestration-service) templates. It deploys your template in multiple Alibaba Cloud Regions and generates a report for each region via a simple configuration file.
```

### Comparing `alibabacloud-ros-iact3-0.1.1/alibabacloud_ros_iact3.egg-info/SOURCES.txt` & `alibabacloud-ros-iact3-0.1.2/alibabacloud_ros_iact3.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,17 +17,21 @@
 iact3/logger.py
 iact3/main.py
 iact3/stack.py
 iact3/termial_print.py
 iact3/util.py
 iact3/cli_modules/__init__.py
 iact3/cli_modules/base.py
+iact3/cli_modules/cost.py
 iact3/cli_modules/delete.py
 iact3/cli_modules/list.py
+iact3/cli_modules/policy.py
+iact3/cli_modules/preview.py
 iact3/cli_modules/test.py
+iact3/cli_modules/validate.py
 iact3/plugin/__init__.py
 iact3/plugin/base_plugin.py
 iact3/plugin/ecs.py
 iact3/plugin/error_code.py
 iact3/plugin/oss.py
 iact3/plugin/ros.py
 iact3/plugin/vpc.py
```

### Comparing `alibabacloud-ros-iact3-0.1.1/alibabacloud_ros_iact3.egg-info/requires.txt` & `alibabacloud-ros-iact3-0.1.2/alibabacloud_ros_iact3.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 aiofiles==22.1.0
-aiohttp==3.8.3
+aiohttp==3.8.5
 aiosignal==1.2.0
 alibabacloud-credentials==0.3.0
 alibabacloud-darabonba-array==0.1.0
 alibabacloud-darabonba-encode-util==0.0.1
 alibabacloud-darabonba-map==0.0.1
 alibabacloud-darabonba-signature-util==0.0.3
 alibabacloud-darabonba-string==0.0.4
@@ -23,15 +23,15 @@
 asynctest==0.13.0
 attrs==22.1.0
 backports.shutil-get-terminal-size==1.0.0
 certifi==2022.12.7
 charset-normalizer==2.1.1
 colorama==0.4.6
 crcmod==1.7
-cryptography==39.0.1
+cryptography==41.0.2
 dataclasses-jsonschema==2.16.0
 debtcollector==2.5.0
 decorator==5.1.1
 dulwich==0.20.50
 exceptiongroup==1.0.4
 frozenlist==1.3.1
 idna==3.4
@@ -52,15 +52,15 @@
 pycryptodome==3.16.0
 pyparsing==3.0.9
 pyrsistent==0.19.2
 python-dateutil==2.8.2
 pytz==2022.6
 PyYAML==6.0
 reprint==0.6.0
-requests==2.28.1
+requests==2.31.0
 retrying==1.3.4
 six==1.16.0
 tabulate==0.9.0
 tomli==2.0.1
 urllib3==1.26.12
 wrapt==1.14.1
 yarl==1.8.1
```

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/cli.py` & `alibabacloud-ros-iact3-0.1.2/iact3/cli.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/base.py` & `alibabacloud-ros-iact3-0.1.2/iact3/cli_modules/base.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/delete.py` & `alibabacloud-ros-iact3-0.1.2/iact3/cli_modules/delete.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/list.py` & `alibabacloud-ros-iact3-0.1.2/iact3/cli_modules/list.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/test.py` & `alibabacloud-ros-iact3-0.1.2/iact3/cli_modules/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,28 +27,30 @@
                   output_directory: str = None,
                   regions: str = None,
                   test_names: str = None,
                   no_delete: bool = False,
                   project_path: str = None,
                   keep_failed: bool = False,
                   dont_wait_for_delete: bool = False,
-                  generate_parameters: bool = False
+                  generate_parameters: bool = False,
+                  log_format: str = None
                   ) -> None:
         '''
         tests whether IaC templates are able to successfully launch
         :param template: path to a template
         :param config_file: path to a config file
         :param output_directory: path to an output directory
         :param regions: comma separated list of regions to test in
         :param test_names: comma separated list of tests to run
         :param no_delete: don't delete stacks after test is complete
         :param project_path: root path of the project relative to config file, template file and output file
         :param keep_failed: do not delete failed stacks
         :param dont_wait_for_delete: exits immediately after calling delete stack
         :param generate_parameters: generate pseudo parameters
+        :param log_format: comma separated list of log format (xml,json)
         :return: None
         '''
         # todo --failed param
         tests = await StackTest.from_file(
             template=template,
             project_config_file=config_file,
             no_delete=no_delete,
@@ -59,15 +61,15 @@
             test_names=test_names
         )
         if generate_parameters:
             Test._get_parameters(tests)
             return
 
         async with tests:
-            await tests.report(output_directory, project_path)
+            await tests.report(output_directory, project_path, log_format)
 
     @staticmethod
     async def clean(regions: str = None):
         '''
         Manually clean up the stacks which were created by Iact3
         :param regions: comma separated list of regions to delete from, default will scan all regions
         '''
@@ -93,14 +95,15 @@
         '''
         tests = await StackTest.from_file(
             template=template,
             project_config_file=config_file,
             regions=regions
         )
         Test._get_parameters(tests)
+    
 
     @staticmethod
     def _get_parameters(tests: StackTest):
         all_configs = tests.configs
         parameters = [
             {
                 'TestName': con.name,
```

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/config.py` & `alibabacloud-ros-iact3-0.1.2/iact3/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,15 +279,17 @@
                     raise Iact3Exception(f'failed to retrieve {template_url}: {ex}')
             else:
                 raise Iact3Exception(f'template url {template_url} is not legally.')
 
         tpl_path = result.pop(TEMPLATE_LOCATION, None)
         tpl_item = self._get_template_location(tpl_path)
         if tpl_item is None:
-            raise Iact3Exception(f'failed to retrieve {tpl_path}')
+            msg = f'Could not find template in {tpl_path or DEFAULT_TEMPLATE_PATH} directory' \
+                  f'Template files need end with .template.json or .template.yaml or .template.yml.'
+            raise Iact3Exception(msg)
         elif isinstance(tpl_item, dict):
             result[TEMPLATE_BODY] = json.dumps(tpl_item)
         else:
             file_path = Path(tpl_item).expanduser().resolve()
             if not file_path.is_file():
                 return result
             try:
```

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/exceptions.py` & `alibabacloud-ros-iact3-0.1.2/iact3/exceptions.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/generate_params.py` & `alibabacloud-ros-iact3-0.1.2/iact3/generate_params.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/main.py` & `alibabacloud-ros-iact3-0.1.2/iact3/main.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/plugin/base_plugin.py` & `alibabacloud-ros-iact3-0.1.2/iact3/plugin/base_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,23 +107,25 @@
         if not self._client:
             client = self.api_client()(self.config)
             if not self.endpoint:
                 self.endpoint = getattr(client, '_endpoint', '')
             return self.api_client()(self.config)
         return self._client
 
-    async def send_request(self, request_name: str, **kwargs) -> dict:
+    async def send_request(self, request_name: str, ignoreException: bool=False, **kwargs) -> dict:
         request = self._build_request(request_name, **kwargs)
         api_name = self._get_api_name(request_name)
         action_name = self._get_action_name(api_name)
         func = getattr(self.client, action_name)
         try:
             resp = await func(request, self.runtime_option)
-        except TeaException as ex:
+        except TeaException as ex:        
             LOG.debug(f'plugin exception: {self.product} {self.endpoint} {api_name} {request.to_map()} {ex.data}')
+            if ignoreException:
+                return ex.data
             raise ex
         if not isinstance(resp, TeaModel):
             LOG.error(f'plugin response: {self.product} {self.endpoint} {api_name} {request.to_map()} {resp}')
             raise TeaException(dict(
                 code=error_code.UNKNOWN_ERROR,
                 message='The response of TeaSDK is not TeaModel.',
                 data=resp
```

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/plugin/ecs.py` & `alibabacloud-ros-iact3-0.1.2/iact3/plugin/ecs.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/plugin/error_code.py` & `alibabacloud-ros-iact3-0.1.2/iact3/plugin/error_code.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/plugin/oss.py` & `alibabacloud-ros-iact3-0.1.2/iact3/plugin/oss.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/plugin/ros.py` & `alibabacloud-ros-iact3-0.1.2/iact3/plugin/ros.py`

 * *Files 21% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         self._convert_tags(tags, kwargs, tag_key='Tag')
         return await self.fetch_all('ListStacksRequest', kwargs, 'Stacks')
 
     async def list_stack_resources(self, stack_id):
         kwargs = dict(
             StackId=stack_id
         )
-        result = await self.send_request('ListStacksRequest', **kwargs)
+        result = await self.send_request('ListStackResourcesRequest', **kwargs)
         return result.get('Resources')
 
     async def get_stack_resource(self, stack_id, logical_resource_id, show_resource_attributes=False,
                                  resource_attributes=None):
         kwargs = dict(
             StackId=stack_id,
             LogicalResourceId=logical_resource_id
@@ -170,7 +170,50 @@
 
     async def get_template(self, template_id: str, template_version: str = None):
         kwargs = dict(
             TemplateId=template_id,
             TemplateVersion=template_version
         )
         return await self.send_request('GetTemplate', **kwargs)
+    
+    async def get_template_estimate_cost(self, template_body: str = None,
+                           parameters: dict = None, region_id: str = None,
+                           template_url: str = None):
+        kwargs = dict(
+            TemplateBody=template_body,
+            TemplateURL=template_url,
+            RegionId=region_id
+        )
+        self._convert_parameters(parameters, kwargs)
+        result = await self.send_request('GetTemplateEstimateCostRequest', **kwargs)
+        return result['Resources']
+    
+    async def validate_template(self, template_body: str = None,
+                                region_id: str = None, template_url: str = None):
+        kwargs = dict(
+            TemplateBody=template_body,
+            TemplateURL=template_url,
+            RegionId=region_id
+        )
+        result = await self.send_request('ValidateTemplateRequest', ignoreException=True, **kwargs)
+        return result
+    
+    async def preview_stack(self, template_body: str = None,
+                           parameters: dict = None, region_id: str = None,
+                           template_url: str = None, stack_name: str = None):
+        kwargs = dict(
+            TemplateBody=template_body,
+            TemplateURL=template_url,
+            RegionId=region_id,
+            StackName=stack_name
+        )
+        self._convert_parameters(parameters, kwargs)
+        result = await self.send_request('PreviewStackRequest', **kwargs)
+        return result['Stack']['Resources']
+    
+    async def generate_template_policy(self, template_body: str = None, template_url: str = None):
+        kwargs = dict(
+            TemplateBody=template_body,
+            TemplateURL=template_url
+        )
+        result = await self.send_request('GenerateTemplatePolicyRequest', ignoreException=True, **kwargs)
+        return result['Policy']
```

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/plugin/vpc.py` & `alibabacloud-ros-iact3-0.1.2/iact3/plugin/vpc.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/report/generate_reports.py` & `alibabacloud-ros-iact3-0.1.2/iact3/report/generate_reports.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import asyncio
 import datetime
 import json
+import xml.etree.ElementTree as ET
+import xml.dom.minidom as minidom
 import logging
 import os
 import textwrap
 import time
 from pathlib import Path
 
 import aiofiles
@@ -73,15 +75,15 @@
                                 text("Test Logs")
 
                             for stack in self._stacks.stacks:
                                 with tag("tr", "class= test-footer"):
                                     with tag("td", "colspan=5"):
                                         text("")
 
-                                LOG.info(f"Reporting on {str(stack.id)}")
+                                LOG.info(f'Start producing test reports for {stack.test_name} in {stack.region}...')
                                 test_name = stack.test_name
                                 status = stack.status
                                 stack_name = stack.name
                                 region = stack.region
                                 css = "class=test-green" if status == 'CREATE_COMPLETE' else 'class=test-red'
 
                                 with tag("tr"):
@@ -119,14 +121,15 @@
             json_result = {
                 'Result': test_result,
                 'Details': details
             }
             file_name = self._report_json_name
             with open(str(self._output_file / file_name), 'w', encoding='utf-8') as f:
                 json.dump(json_result, f, ensure_ascii=False)
+            LOG.info(f'The test report has been completed, you can view it in {self._output_file} directory.')
             return html_output
 
     async def get_events(self, stack: Stack):
         stack_events = await stack.events(refresh=True)
         events = []
         for event in stack_events:
             event_details = {
@@ -139,42 +142,121 @@
                 event_details["ResourceStatusReason"] = event.status_reason
             else:
                 event_details["ResourceStatusReason"] = ""
 
             events.append(event_details)
         return events
 
-    async def create_logs(self):
+    async def get_resources(self, stack: Stack):
+        stack_resources = await stack.resources(refresh=True)
+        resources = []
+        for resource in stack_resources:
+            resource_details = {
+                "TimeStamp": str(resource.last_updated_timestamp),
+                "ResourceStatus": resource.status,
+                "ResourceType": resource.type,
+                "LogicalResourceId": resource.logical_id,
+                "PhysicalResourceId": resource.physical_id
+            }
+            if resource.status_reason:
+                resource_details["ResourceStatusReason"] = resource.status_reason
+            else:
+                resource_details["ResourceStatusReason"] = ""
+            resources.append(resource_details)
+        return resources
+
+    async def create_logs(self, log_format:str):
+        if log_format:
+            log_formats = log_format.split(',')
+        else:
+            log_formats = []
         tasks = []
         file_names = []
         for stack in self._stacks.stacks:
-            file_name = f'{stack.name}-{stack.region}.txt'
-            task = asyncio.create_task(self.write_logs(stack, self._output_file / file_name))
+            file_name = f'{stack.name}-{stack.region}'
+            task = asyncio.create_task(self.write_logs(stack, self._output_file / file_name, log_formats))
             tasks.append(task)
-            file_names.append(file_name)
+            file_names.append(file_name + ".txt")
+            if "json" in log_formats:
+                file_names.append(file_name + ".json")
+            if "xml" in log_formats:
+                file_names.append(file_name + ".xml")
         await asyncio.gather(*tasks)
         file_names.append(self._report_json_name)
         return file_names
 
-    async def write_logs(self, stack: Stack, log_path: Path):
+    async def add_attr_minidom(self, doc: minidom.Document,father_node: minidom.Element, label, value):     
+        child = doc.createElement(label)
+        father_node.appendChild(child)
+        if isinstance(value, dict):
+            for k, v in value.items():
+                await self.add_attr_minidom(doc, child, k, v)
+            
+        elif isinstance(value, list):
+            for list_item in value:
+                await self.add_attr_minidom(doc, child, "item", list_item)
+        else:
+            child_content = doc.createTextNode(str(value))
+            child.appendChild(child_content)
+       
+    async def write_logs(self, stack: Stack, log_path: Path, log_formats: list):
         stack_name = stack.name
         region = stack.region
         stack_id = stack.id or ''
         parameters = stack.parameters
 
         events = await self.get_events(stack) if stack.id else []
 
+        resources = await self.get_resources(stack) if stack.id else []
+
         if stack.launch_succeeded:
             tested_result = 'Success'
             reason = 'Stack launch was successful'
         else:
             tested_result = 'Failed'
             reason = f'{stack.status}, {stack.status_reason}'
 
-        async with aiofiles.open(str(log_path), "a", encoding="utf-8") as log_output:
+        test_time = datetime.datetime.now().strftime("%A, %d. %B %Y %I:%M%p")
+
+        if "json" in log_formats:
+            with open(str(log_path)+'.json', 'w', encoding='utf-8') as log_output:       
+                json_output = {}
+                json_output["Region"] = region
+                json_output["StackName"] = stack_name
+                json_output["StackId"] = stack_id
+                json_output["Parameters"] = parameters
+                json_output["TestedResult"] = tested_result
+                json_output["ResultReason"] = str(reason)
+                json_output["Events"] = events
+                json_output["Resources"] = resources
+                json_output["TestTime"] = test_time
+                json.dump(json_output, log_output, ensure_ascii=False, indent=4)
+                log_output.close()
+        
+        if "xml" in log_formats:
+            with open(str(log_path)+'.xml', 'w', encoding='utf-8') as log_output:
+                xml_doc = minidom.Document()
+                root = xml_doc.createElement(f'{stack.name}-{stack.region}')
+                xml_doc.appendChild(root)
+
+                await self.add_attr_minidom(xml_doc, root, "Region", region)
+                await self.add_attr_minidom(xml_doc, root, "StackName", stack_name)
+                await self.add_attr_minidom(xml_doc, root, "StackId", stack_id)
+                await self.add_attr_minidom(xml_doc, root, "Parameters", parameters)
+                await self.add_attr_minidom(xml_doc, root, "TestedResult", tested_result)
+                await self.add_attr_minidom(xml_doc, root, "ResultReason", reason)
+                await self.add_attr_minidom(xml_doc, root, "Events", events)
+                await self.add_attr_minidom(xml_doc, root, "Resources", resources)
+                await self.add_attr_minidom(xml_doc, root, "TestTime", test_time)
+            
+                log_output.write(xml_doc.toprettyxml(indent="\t"))
+
+
+
+        async with aiofiles.open(str(log_path)+'.txt', "a", encoding="utf-8") as log_output:
             await log_output.write(
                 "------------------------------------------------------------------"
                 "-----------\n"
             )
             await log_output.write("Region: " + region + "\n")
             await log_output.write("StackName: " + stack_name + "\n")
             await log_output.write("StackId: " + stack_id + "\n")
@@ -208,20 +290,30 @@
             await log_output.write("Events:  \n")
             await log_output.writelines(tabulate.tabulate(events, headers="keys"))
             await log_output.write(
                 "\n****************************************************************"
                 "*************\n"
             )
             await log_output.write(
+                "******************************************************************"
+                "***********\n"
+            )
+            await log_output.write("Resources:  \n")
+            await log_output.write(tabulate.tabulate(resources, headers="keys"))
+            await log_output.write(
+                "\n****************************************************************"
+                "*************\n"
+            )
+            await log_output.write(
                 "------------------------------------------------------------------"
                 "-----------\n"
             )
             await log_output.write(
                 "Tested on: "
-                + datetime.datetime.now().strftime("%A, %d. %B %Y %I:%M%p")
+                + test_time
                 + "\n"
             )
             await log_output.write(
                 "------------------------------------------------------------------"
                 "-----------\n\n"
             )
             await log_output.close()
```

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/report/html.css` & `alibabacloud-ros-iact3-0.1.2/iact3/report/html.css`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/stack.py` & `alibabacloud-ros-iact3-0.1.2/iact3/stack.py`

 * *Files 22% similar despite different names*

```diff
@@ -107,15 +107,32 @@
 
     async def delete_stacks(self, **kwargs):
         stacks = self.stacks.filter(kwargs)
         stack_tasks = [
             asyncio.create_task(Stack.delete(stack)) for stack in stacks
         ]
         await asyncio.gather(*stack_tasks)
+    
+    async def get_stacks_price(self):
+        if self.stacks:
+            raise Iact3Exception('Stacker already initialised with stack objects')
+        self.tags.update(self._sys_tags)
+        stack_tasks = [
+            asyncio.create_task(Stack.get_price(test, self.tags, self.uid)) for test in self.tests
+        ]
+        self.stacks += await asyncio.gather(*stack_tasks)
 
+    async def preview_stacks_result(self):
+        if self.stacks:
+            raise Iact3Exception('Stacker already initialised with stack objects')
+        self.tags.update(self._sys_tags)
+        stack_tasks = [
+            asyncio.create_task(Stack.preview_stack_result(test, self.tags, self.uid)) for test in self.tests
+        ]
+        self.stacks += await asyncio.gather(*stack_tasks)
 
 def criteria_matches(kwargs: dict, instance):
     for k in kwargs:
         if not hasattr(instance, k):
             raise ValueError(f'{k} is not a valid property of {type(instance)}')
     for k, v in kwargs.items():
         ins_v = getattr(instance, k)
@@ -184,34 +201,36 @@
     ):
         uuid = uuid if uuid else uuid4()
         self.stack_id: str = stack_id
         self.test_name: str = test_name
         self.uuid: UUID = uuid
         self.logical_id: str = resource_dict['LogicalResourceId']
         self.type: str = resource_dict['ResourceType']
-        self.status: str = resource_dict['ResourceStatus']
+        # self.status: str = resource_dict['ResourceStatus']
+        self.status: str = resource_dict['Status']
         self.physical_id: str = ''
         self.last_updated_timestamp: datetime = datetime.fromtimestamp(0)
         self.status_reason: str = ''
         if 'PhysicalResourceId' in resource_dict.keys():
             self.physical_id = resource_dict['PhysicalResourceId']
-        if 'LastUpdatedTimestamp' in resource_dict.keys():
-            self.last_updated_timestamp = resource_dict['LastUpdatedTimestamp']
-        if 'ResourceStatusReason' in resource_dict.keys():
-            self.status_reason = resource_dict['ResourceStatusReason']
+        if 'UpdateTime' in resource_dict.keys():
+            self.last_updated_timestamp = resource_dict['UpdateTime']
+        if 'StatusReason' in resource_dict.keys():
+            self.status_reason = resource_dict['StatusReason']
 
     def __str__(self):
         return '<Resource {} {}>'.format(self.logical_id, self.status)
 
 
 class Stack:
 
     def __init__(self, region: str, stack_id: str, test_name: str = None,
                  uuid: UUID = None, status_reason: str = None, stack_name: str = None,
-                 parameters: dict = None, credential: CredentialClient = None):
+                 parameters: dict = None, credential: CredentialClient = None, 
+                 template_price: dict = None, preview_result: dict = None):
         self.test_name: str = test_name
         self.uuid: UUID = uuid if uuid else uuid4()
         self.id: str = stack_id
         self.region = region
         self.plugin: StackPlugin = StackPlugin(region_id=region, credential=credential)
         self.name = stack_name
         self.parameters = parameters
@@ -220,14 +239,16 @@
         self._status: str = ''
         self.status_reason: str = status_reason or ''
         self._launch_succeeded: bool = False
         self.auto_refresh_interval: timedelta = timedelta(seconds=60)
         self._last_event_refresh: datetime = datetime.fromtimestamp(0)
         self._last_resource_refresh: datetime = datetime.fromtimestamp(0)
         self.timer = Timer(self.auto_refresh_interval.total_seconds(), self.refresh)
+        self.template_price = template_price
+        self.preview_result = preview_result
 
     def __str__(self):
         return self.id
 
     def __repr__(self):
         return '<Stack object {} at {}>'.format(self.test_name, hex(id(self)))
 
@@ -308,14 +329,95 @@
             stack.timer.cancel()
             return stack
         stack = cls(region, stack_id, name, uuid, stack_name=stack_name,
                     parameters=parameters, credential=credential)
         await stack.refresh()
         return stack
 
+    @classmethod
+    async def get_price(cls, test: TestConfig, tags: dict = None, uuid: UUID = None):
+        parameters = test.parameters
+        template_args = test.template_config.to_dict()
+        name = test.test_name
+        if not tags:
+            tags = {}
+        tags.update({f'{IAC_NAME}-test-name': name})
+        region = test.region
+        credential = test.auth.credential
+        plugin = StackPlugin(region_id=test.region, credential=credential)
+        stack_name = f'{IAC_NAME}-{name}-{region}-{uuid4().hex[:8]}'
+        config_error = test.error
+        if config_error:
+            stack = cls(region, None, name, uuid,
+                        status_reason=getattr(config_error, 'message', 'Unknown error'),
+                        stack_name=stack_name, credential=credential)
+            stack.status = getattr(config_error, 'code', 'Unknown error')
+            stack._launch_succeeded = False
+            stack.timer.cancel()
+            return stack
+        try:
+            template_price = await plugin.get_template_estimate_cost(
+                parameters=parameters,
+                **template_args,
+                region_id=region
+            )
+        except TeaException as ex:
+            stack_id = None
+            stack = cls(region, stack_id, name, uuid, status_reason=ex.message,
+                        stack_name=stack_name, parameters=parameters, credential=credential)
+            stack.status = ex.code
+            stack._launch_succeeded = False
+            stack.timer.cancel()
+            return stack
+        stack_id = None
+        stack = cls(region, stack_id, name, uuid, stack_name=stack_name,
+                    parameters=parameters, credential=credential, template_price=template_price)
+        return stack
+    
+    @classmethod
+    async def preview_stack_result(cls, test: TestConfig, tags: dict = None, uuid: UUID = None):
+        parameters = test.parameters
+        template_args = test.template_config.to_dict()
+        name = test.test_name
+        if not tags:
+            tags = {}
+        tags.update({f'{IAC_NAME}-test-name': name})
+        region = test.region
+        credential = test.auth.credential
+        plugin = StackPlugin(region_id=test.region, credential=credential)
+        stack_name = f'{IAC_NAME}-{name}-{region}-{uuid4().hex[:8]}'
+        config_error = test.error
+        if config_error:
+            stack = cls(region, None, name, uuid,
+                        status_reason=getattr(config_error, 'message', 'Unknown error'),
+                        stack_name=stack_name, credential=credential)
+            stack.status = getattr(config_error, 'code', 'Unknown error')
+            stack._launch_succeeded = False
+            stack.timer.cancel()
+            return stack
+        try:
+            preview_result = await plugin.preview_stack(
+                parameters=parameters,
+                **template_args,
+                region_id=region,
+                stack_name=stack_name
+            )
+        except TeaException as ex:
+            stack_id = None
+            stack = cls(region, stack_id, name, uuid, status_reason=ex.message,
+                        stack_name=stack_name, parameters=parameters, credential=credential)
+            stack.status = ex.code
+            stack._launch_succeeded = False
+            stack.timer.cancel()
+            return stack
+        stack_id = None
+        stack = cls(region, stack_id, name, uuid, stack_name=stack_name,
+                    parameters=parameters, credential=credential, preview_result=preview_result)
+        return stack
+
     async def refresh(self, properties: bool = True, events: bool = False, resources: bool = False) -> None:
         if properties:
             await self.set_stack_properties()
         if events:
             await self._fetch_stack_events()
             self._last_event_refresh = datetime.now()
         if resources:
@@ -355,15 +457,15 @@
         return self._resources
 
     async def _fetch_stack_resources(self) -> None:
         self._last_resource_refresh = datetime.now()
         resources = Resources()
         stack_resources = await self.plugin.list_stack_resources(self.id)
         for res in stack_resources:
-            resources.append(res)
+            resources.append(Resource(self.id,res,self.test_name,self.uuid))
         self._resources = resources
 
     @staticmethod
     async def delete(stack) -> None:
         stack_id = stack.id
         if not stack_id:
             return
```

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/testing/base.py` & `alibabacloud-ros-iact3-0.1.2/iact3/testing/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 args[TEMPLATE_CONFIG] = {TEMPLATE_LOCATION: str(template_path)}
             else:
                 args[TEMPLATE_CONFIG] = {TEMPLATE_LOCATION: str(project_root)}
         else:
             project_path = DEFAULT_PROJECT_ROOT
             if template:
                 args[TEMPLATE_CONFIG] = {TEMPLATE_LOCATION: template}
-
+        
         base_config = BaseConfig.create(
             project_config_file=project_config_file or DEFAULT_CONFIG_FILE,
             args={PROJECT: args},
             project_path=project_path
         )
         project_name = base_config.project.name
         if not project_name:
@@ -93,21 +93,21 @@
                    no_delete=no_delete,
                    keep_failed=keep_failed,
                    dont_wait_for_delete=dont_wait_for_delete,
                    rerun_failed=rerun_failed,
                    oss_config=base_config.project.oss_config,
                    auth=base_config.general.auth)
 
-    async def report(self, output_directory, project_path=None):
+    async def report(self, output_directory, project_path=None, log_format=None):
         project_root = Path(project_path).expanduser().resolve() if project_path else DEFAULT_PROJECT_ROOT
         output_directory = output_directory or DEFAULT_OUTPUT_DIRECTORY
         report_path = project_root / output_directory
         report_path.mkdir(exist_ok=True)
         reporter = ReportBuilder(self.stacker, report_path)
-        file_names = await reporter.create_logs()
+        file_names = await reporter.create_logs(log_format)
         index = await reporter.generate_report()
         self._upload_to_oss(report_path, index, file_names)
 
     def _upload_to_oss(self, report_path: Path, index: str, file_names: list):
         bucket = self.oss_config.bucket_name
         region = self.oss_config.bucket_region
         if bucket and region:
```

### Comparing `alibabacloud-ros-iact3-0.1.1/iact3/util.py` & `alibabacloud-ros-iact3-0.1.2/iact3/util.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.1/requirements.txt` & `alibabacloud-ros-iact3-0.1.2/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 aiofiles==22.1.0
-aiohttp==3.8.3
+aiohttp==3.8.5
 aiosignal==1.2.0
 alibabacloud-credentials==0.3.0
 alibabacloud-darabonba-array==0.1.0
 alibabacloud-darabonba-encode-util==0.0.1
 alibabacloud-darabonba-map==0.0.1
 alibabacloud-darabonba-signature-util==0.0.3
 alibabacloud-darabonba-string==0.0.4
@@ -23,15 +23,15 @@
 asynctest==0.13.0
 attrs==22.1.0
 backports.shutil-get-terminal-size==1.0.0
 certifi==2022.12.7
 charset-normalizer==2.1.1
 colorama==0.4.6
 crcmod==1.7
-cryptography==39.0.1
+cryptography==41.0.2
 dataclasses-jsonschema==2.16.0
 debtcollector==2.5.0
 decorator==5.1.1
 dulwich==0.20.50
 exceptiongroup==1.0.4
 frozenlist==1.3.1
 idna==3.4
@@ -52,15 +52,15 @@
 pycryptodome==3.16.0
 pyparsing==3.0.9
 pyrsistent==0.19.2
 python-dateutil==2.8.2
 pytz==2022.6
 PyYAML==6.0
 reprint==0.6.0
-requests==2.28.1
+requests==2.31.0
 retrying==1.3.4
 six==1.16.0
 tabulate==0.9.0
 tomli==2.0.1
 urllib3==1.26.12
 wrapt==1.14.1
 yarl==1.8.1
```

### Comparing `alibabacloud-ros-iact3-0.1.1/setup.py` & `alibabacloud-ros-iact3-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("README.md") as fp:
     long_description = fp.read()
 
 
 setuptools.setup(
     name="alibabacloud-ros-iact3",
-    version="0.1.1",
+    version="0.1.2",
 
     description="Iact3 is a tool that tests Terraform and ROS(Resource Orchestration Service) templates.",
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     author="AlibabaCloud",
     packages=[
```

