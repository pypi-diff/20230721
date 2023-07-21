# Comparing `tmp/xiaobaisaf-2.3.4.tar.gz` & `tmp/xiaobaisaf-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaobaisaf-2.3.4.tar", last modified: Wed Jul  5 15:46:09 2023, max compression
+gzip compressed data, was "xiaobaisaf-2.3.5.tar", last modified: Fri Jul 21 15:48:02 2023, max compression
```

## Comparing `xiaobaisaf-2.3.4.tar` & `xiaobaisaf-2.3.5.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.802691 xiaobaisaf-2.3.4/
--rw-rw-rw-   0        0        0    35181 2023-06-27 16:34:34.000000 xiaobaisaf-2.3.4/LICENSE
--rw-rw-rw-   0        0        0    11921 2023-07-05 15:46:09.802691 xiaobaisaf-2.3.4/PKG-INFO
--rw-rw-rw-   0        0        0    11250 2023-07-05 15:45:45.000000 xiaobaisaf-2.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.525409 xiaobaisaf-2.3.4/saf/
--rw-rw-rw-   0        0        0     1436 2023-06-27 16:40:21.000000 xiaobaisaf-2.3.4/saf/__init__.py
--rw-rw-rw-   0        0        0      152 2023-07-05 15:45:45.000000 xiaobaisaf-2.3.4/saf/__version__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.544359 xiaobaisaf-2.3.4/saf/data/
--rw-rw-rw-   0        0        0      225 2023-06-27 16:34:35.000000 xiaobaisaf-2.3.4/saf/data/__init__.py
--rw-rw-rw-   0        0        0     2943 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.4/saf/data/config.py
--rw-rw-rw-   0        0        0     4286 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.4/saf/data/favicon.ico
-drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.552337 xiaobaisaf-2.3.4/saf/example/
--rw-rw-rw-   0        0        0      100 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.576274 xiaobaisaf-2.3.4/saf/example/api/
-drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.590235 xiaobaisaf-2.3.4/saf/example/api/Config/
--rw-rw-rw-   0        0        0      131 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/api/Config/__init__.py
--rw-rw-rw-   0        0        0     5086 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/api/Config/config.py
-drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.597218 xiaobaisaf-2.3.4/saf/example/api/TestCases/
--rw-rw-rw-   0        0        0      129 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/api/TestCases/__init__.py
--rw-rw-rw-   0        0        0     1438 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/api/TestCases/test_one_html_case_template.py
-drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.630129 xiaobaisaf-2.3.4/saf/example/api/Utils/
--rw-rw-rw-   0        0        0     1389 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.4/saf/example/api/Utils/ExcelUtils.py
--rw-rw-rw-   0        0        0     2099 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/api/Utils/YamlUtils.py
--rw-rw-rw-   0        0        0      308 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/api/Utils/__init__.py
--rw-rw-rw-   0        0        0     1111 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.4/saf/example/api/Utils/api_client.py
--rw-rw-rw-   0        0        0      285 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.4/saf/example/api/Utils/logger.py
--rw-rw-rw-   0        0        0      129 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/api/__init__.py
--rw-rw-rw-   0        0        0     1211 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/api/run.py
--rw-rw-rw-   0        0        0      549 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/api/send_email_script.py
-drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.636114 xiaobaisaf-2.3.4/saf/example/web/
-drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.676028 xiaobaisaf-2.3.4/saf/example/web/Cases/
--rw-rw-rw-   0        0        0      140 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/Cases/__init__.py
--rw-rw-rw-   0        0        0     2441 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/Cases/conftest.py
--rw-rw-rw-   0        0        0      930 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/Cases/test_xiaobai_case_allure.py
--rw-rw-rw-   0        0        0      962 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/Cases/test_xiaobai_case_submitBug.py
--rw-rw-rw-   0        0        0      320 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/Cases/test_xiaobai_case_v1.py
--rw-rw-rw-   0        0        0     1192 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/Cases/test_xiaobai_case_v2.py
--rw-rw-rw-   0        0        0      228 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/Cases/test_xiaobai_case_v3.py
-drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.683010 xiaobaisaf-2.3.4/saf/example/web/Utils/
--rw-rw-rw-   0        0        0     1389 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.4/saf/example/web/Utils/ExcelUtils.py
--rw-rw-rw-   0        0        0     2099 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.4/saf/example/web/Utils/YamlUtils.py
--rw-rw-rw-   0        0        0      308 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.4/saf/example/web/Utils/__init__.py
--rw-rw-rw-   0        0        0      285 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.4/saf/example/web/Utils/logger.py
--rw-rw-rw-   0        0        0      435 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.692983 xiaobaisaf-2.3.4/saf/example/web/pageObject/
--rw-rw-rw-   0        0        0      166 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/pageObject/__init__.py
--rw-rw-rw-   0        0        0      152 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/example/web/pageObject/register_page_element.py
-drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.785735 xiaobaisaf-2.3.4/saf/utils/
--rw-rw-rw-   0        0        0     8132 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.4/saf/utils/BugUtils.py
--rw-rw-rw-   0        0        0      130 2023-07-05 15:07:02.000000 xiaobaisaf-2.3.4/saf/utils/Demo.py
--rw-rw-rw-   0        0        0     2076 2023-06-27 16:40:34.000000 xiaobaisaf-2.3.4/saf/utils/MonitorAndroidDeviceGUI.py
--rw-rw-rw-   0        0        0     8917 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.4/saf/utils/MonitorAndroidPackageCLI.py
--rw-rw-rw-   0        0        0    14196 2023-07-05 15:45:45.000000 xiaobaisaf-2.3.4/saf/utils/MonitorAndroidPackageGUI.py
--rw-rw-rw-   0        0        0     7790 2023-06-30 17:18:46.000000 xiaobaisaf-2.3.4/saf/utils/MonitorAndroidPackagePower.py
--rw-rw-rw-   0        0        0     1462 2023-07-05 15:11:29.000000 xiaobaisaf-2.3.4/saf/utils/MonitorCANBus.py
--rw-rw-rw-   0        0        0     5933 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.4/saf/utils/MonitorDBs.py
--rw-rw-rw-   0        0        0     2099 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/utils/YamlUtils.py
--rw-rw-rw-   0        0        0      201 2023-06-27 16:34:35.000000 xiaobaisaf-2.3.4/saf/utils/__init__.py
--rw-rw-rw-   0        0        0     3061 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.4/saf/utils/downloadUtils.py
--rw-rw-rw-   0        0        0     1271 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.4/saf/utils/elementUtils.py
--rw-rw-rw-   0        0        0      660 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.4/saf/utils/imageUtils.py
--rw-rw-rw-   0        0        0     1369 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.4/saf/utils/networkSpeedUtils.py
--rw-rw-rw-   0        0        0      132 2023-06-27 16:40:21.000000 xiaobaisaf-2.3.4/saf/utils/osEnvUtils.py
--rw-rw-rw-   0        0        0     8924 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.4/saf/utils/selenium2POM.py
--rw-rw-rw-   0        0        0     2694 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.4/saf/utils/sendMsgUtils.py
--rw-rw-rw-   0        0        0     2549 2023-06-30 17:16:51.000000 xiaobaisaf-2.3.4/saf/utils/xiaobaicmd.py
--rw-rw-rw-   0        0        0       42 2023-07-05 15:46:09.802691 xiaobaisaf-2.3.4/setup.cfg
--rw-rw-rw-   0        0        0     2450 2023-06-28 17:25:03.000000 xiaobaisaf-2.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 15:46:09.801693 xiaobaisaf-2.3.4/xiaobaisaf.egg-info/
--rw-rw-rw-   0        0        0    11921 2023-07-05 15:46:09.000000 xiaobaisaf-2.3.4/xiaobaisaf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1838 2023-07-05 15:46:09.000000 xiaobaisaf-2.3.4/xiaobaisaf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 15:46:09.000000 xiaobaisaf-2.3.4/xiaobaisaf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-05 15:46:09.000000 xiaobaisaf-2.3.4/xiaobaisaf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      154 2023-07-05 15:46:09.000000 xiaobaisaf-2.3.4/xiaobaisaf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-05 15:46:09.000000 xiaobaisaf-2.3.4/xiaobaisaf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.533143 xiaobaisaf-2.3.5/
+-rw-rw-rw-   0        0        0    35181 2023-06-27 16:34:34.000000 xiaobaisaf-2.3.5/LICENSE
+-rw-rw-rw-   0        0        0    12129 2023-07-21 15:48:02.533143 xiaobaisaf-2.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0    11458 2023-07-21 15:37:05.000000 xiaobaisaf-2.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.505217 xiaobaisaf-2.3.5/saf/
+-rw-rw-rw-   0        0        0     1436 2023-06-27 16:40:21.000000 xiaobaisaf-2.3.5/saf/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-07-21 15:34:18.000000 xiaobaisaf-2.3.5/saf/__version__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.507212 xiaobaisaf-2.3.5/saf/data/
+-rw-rw-rw-   0        0        0      225 2023-06-27 16:34:35.000000 xiaobaisaf-2.3.5/saf/data/__init__.py
+-rw-rw-rw-   0        0        0     2943 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.5/saf/data/config.py
+-rw-rw-rw-   0        0        0     4286 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.5/saf/data/favicon.ico
+-rw-rw-rw-   0        0        0     1201 2023-06-26 08:03:27.000000 xiaobaisaf-2.3.5/saf/data/software_check.sh
+drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.508210 xiaobaisaf-2.3.5/saf/example/
+-rw-rw-rw-   0        0        0      100 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.509207 xiaobaisaf-2.3.5/saf/example/api/
+drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.510205 xiaobaisaf-2.3.5/saf/example/api/Config/
+-rw-rw-rw-   0        0        0      131 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/api/Config/__init__.py
+-rw-rw-rw-   0        0        0     5086 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/api/Config/config.py
+drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.511202 xiaobaisaf-2.3.5/saf/example/api/TestCases/
+-rw-rw-rw-   0        0        0      129 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/api/TestCases/__init__.py
+-rw-rw-rw-   0        0        0     1438 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/api/TestCases/test_one_html_case_template.py
+drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.514194 xiaobaisaf-2.3.5/saf/example/api/Utils/
+-rw-rw-rw-   0        0        0     1389 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.5/saf/example/api/Utils/ExcelUtils.py
+-rw-rw-rw-   0        0        0     2099 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/api/Utils/YamlUtils.py
+-rw-rw-rw-   0        0        0      308 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/api/Utils/__init__.py
+-rw-rw-rw-   0        0        0     1111 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.5/saf/example/api/Utils/api_client.py
+-rw-rw-rw-   0        0        0      285 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.5/saf/example/api/Utils/logger.py
+-rw-rw-rw-   0        0        0      129 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/api/__init__.py
+-rw-rw-rw-   0        0        0     1211 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/api/run.py
+-rw-rw-rw-   0        0        0      549 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/api/send_email_script.py
+drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.514194 xiaobaisaf-2.3.5/saf/example/web/
+drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.518183 xiaobaisaf-2.3.5/saf/example/web/Cases/
+-rw-rw-rw-   0        0        0      140 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/Cases/__init__.py
+-rw-rw-rw-   0        0        0     2441 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/Cases/conftest.py
+-rw-rw-rw-   0        0        0      930 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/Cases/test_xiaobai_case_allure.py
+-rw-rw-rw-   0        0        0      962 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/Cases/test_xiaobai_case_submitBug.py
+-rw-rw-rw-   0        0        0      320 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/Cases/test_xiaobai_case_v1.py
+-rw-rw-rw-   0        0        0     1192 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/Cases/test_xiaobai_case_v2.py
+-rw-rw-rw-   0        0        0      228 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/Cases/test_xiaobai_case_v3.py
+drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.519179 xiaobaisaf-2.3.5/saf/example/web/Utils/
+-rw-rw-rw-   0        0        0     1389 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.5/saf/example/web/Utils/ExcelUtils.py
+-rw-rw-rw-   0        0        0     2099 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.5/saf/example/web/Utils/YamlUtils.py
+-rw-rw-rw-   0        0        0      308 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.5/saf/example/web/Utils/__init__.py
+-rw-rw-rw-   0        0        0      285 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.5/saf/example/web/Utils/logger.py
+-rw-rw-rw-   0        0        0      435 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.520177 xiaobaisaf-2.3.5/saf/example/web/pageObject/
+-rw-rw-rw-   0        0        0      166 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/pageObject/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/pageObject/register_page_element.py
+drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.529154 xiaobaisaf-2.3.5/saf/utils/
+-rw-rw-rw-   0        0        0     8132 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.5/saf/utils/BugUtils.py
+-rw-rw-rw-   0        0        0      130 2023-07-05 15:07:02.000000 xiaobaisaf-2.3.5/saf/utils/Demo.py
+-rw-rw-rw-   0        0        0     2076 2023-06-27 16:40:34.000000 xiaobaisaf-2.3.5/saf/utils/MonitorAndroidDeviceGUI.py
+-rw-rw-rw-   0        0        0     8917 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.5/saf/utils/MonitorAndroidPackageCLI.py
+-rw-rw-rw-   0        0        0    14196 2023-07-05 15:45:45.000000 xiaobaisaf-2.3.5/saf/utils/MonitorAndroidPackageGUI.py
+-rw-rw-rw-   0        0        0     7790 2023-06-30 17:18:46.000000 xiaobaisaf-2.3.5/saf/utils/MonitorAndroidPackagePower.py
+-rw-rw-rw-   0        0        0     1583 2023-07-21 15:26:19.000000 xiaobaisaf-2.3.5/saf/utils/MonitorCANBus.py
+-rw-rw-rw-   0        0        0     5933 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.5/saf/utils/MonitorDBs.py
+-rw-rw-rw-   0        0        0     2099 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/utils/YamlUtils.py
+-rw-rw-rw-   0        0        0      201 2023-06-27 16:34:35.000000 xiaobaisaf-2.3.5/saf/utils/__init__.py
+-rw-rw-rw-   0        0        0     3061 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.5/saf/utils/downloadUtils.py
+-rw-rw-rw-   0        0        0     1271 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.5/saf/utils/elementUtils.py
+-rw-rw-rw-   0        0        0      660 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.5/saf/utils/imageUtils.py
+-rw-rw-rw-   0        0        0     1369 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.5/saf/utils/networkSpeedUtils.py
+-rw-rw-rw-   0        0        0      132 2023-06-27 16:40:21.000000 xiaobaisaf-2.3.5/saf/utils/osEnvUtils.py
+-rw-rw-rw-   0        0        0    11552 2023-07-21 15:48:01.000000 xiaobaisaf-2.3.5/saf/utils/selenium2POM.py
+-rw-rw-rw-   0        0        0     2694 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.5/saf/utils/sendMsgUtils.py
+-rw-rw-rw-   0        0        0     2549 2023-06-30 17:16:51.000000 xiaobaisaf-2.3.5/saf/utils/xiaobaicmd.py
+-rw-rw-rw-   0        0        0       42 2023-07-21 15:48:02.534140 xiaobaisaf-2.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     2514 2023-07-06 16:41:30.000000 xiaobaisaf-2.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.532146 xiaobaisaf-2.3.5/xiaobaisaf.egg-info/
+-rw-rw-rw-   0        0        0    12129 2023-07-21 15:48:02.000000 xiaobaisaf-2.3.5/xiaobaisaf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1865 2023-07-21 15:48:02.000000 xiaobaisaf-2.3.5/xiaobaisaf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 15:48:02.000000 xiaobaisaf-2.3.5/xiaobaisaf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-21 15:48:02.000000 xiaobaisaf-2.3.5/xiaobaisaf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      154 2023-07-21 15:48:02.000000 xiaobaisaf-2.3.5/xiaobaisaf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-21 15:48:02.000000 xiaobaisaf-2.3.5/xiaobaisaf.egg-info/top_level.txt
```

### Comparing `xiaobaisaf-2.3.4/LICENSE` & `xiaobaisaf-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/PKG-INFO` & `xiaobaisaf-2.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaobaisaf
-Version: 2.3.4
+Version: 2.3.5
 Summary: simple_automation_framework(简称：SAF)使用最简单的模式就可以实现需要功能和测试效果，也是xiaobaiauto2的简化版SAF继承了selenium、requests/httpx、appium、loguru、xiaobaiauto2、飞书机器人、钉钉机器人、企业微信机器人（暂时不支持）、禅道提单API
 Home-page: https://gitee.com/xiaobaikeji/simlpe_automation_framework
 Author: xiaobaiTser
 Author-email: 807447312@qq.com
 Keywords: saf test auto automation xiaobai xiaobaiauto2 test framework
 Requires-Python: >=3.6, <3.10
 Description-Content-Type: text/markdown
@@ -260,15 +260,15 @@
     - ('xiaobai', '12346', 200)
     - ('xiaohui', '123456', 200)
 ```
 
 ### saf>1.8 基于selenium完成正常的页面操作，工具会自动在当前目录下生成Pages目录，目录内会自动生成当前打开的所有页面的PageObject代码，命令如下：
 ```cmd
 xiaobaicmd -u URL 
-xiaobaicmd -url URL 
+xiaobaicmd --url URL 
 ```
 
 ### saf>1.9  基于adb实现监控Android设备中APP操作时实时生成XPath表达式及坐标等数据
 ```cmd
 xiaobaicmd -m gui             # 基于界面实时获取APP数据
 xiaobaicmd --monitor gui      # 基于界面实时获取APP数据
 xiaobaicmd -m cli             # 基于命令实时获取APP数据
@@ -315,27 +315,28 @@
 
 [163邮箱配置](http://help.163.com/09/1223/14/5R7P3QI100753VB8.html, "163邮箱配置")
 
 [QQ邮箱配置](https://service.mail.qq.com/cgi-bin/help?subtype=1&id=28&no=369, "QQ邮箱配置")
 
 ### 更新日志
 
-| version | info                     |
-|---------|--------------------------|
-| 1.0     | 基本实现web自动化模板功能           |
-| 1.1     | fix上个版本的BUG              |
-| 1.2     | 新增allure报告库及封装禅道提单接口     |
-| 1.3     | 新增jira提单接口               |
-| 1.4     | 新增pytest参数化样例            |
-| 1.5     | 优化pytest样例内容             |
-| 1.6     | 优化                       |
-| 1.7     | 新增基础环境检测功能               |
-| 1.8     | 新增API自动化模板               |
-| 1.9     | 新增xiaobaicmd -u命令        |
-| 2.0     | 新增xiaobaicmd -m命令        |
-| 2.1     | 新增xiaobaicmd --device命令  |
-| 2.2     | 优化xiaobaicmd --device命令  |
-| 2.3     | 新增实时监控Android设备耗电量       |
-| 2.3.1   | fix                      |
-| 2.3.2   | fix                      |
-| 2.3.3   | 新增实时监控Android当前APP的内存使用率 |
-| 2.3.4   | 优化xiaobaicmd -m gui效果展示  |
+| version | info                            |
+|---------|---------------------------------|
+| 1.0     | 基本实现web自动化模板功能                  |
+| 1.1     | fix上个版本的BUG                     |
+| 1.2     | 新增allure报告库及封装禅道提单接口            |
+| 1.3     | 新增jira提单接口                      |
+| 1.4     | 新增pytest参数化样例                   |
+| 1.5     | 优化pytest样例内容                    |
+| 1.6     | 优化                              |
+| 1.7     | 新增基础环境检测功能                      |
+| 1.8     | 新增API自动化模板                      |
+| 1.9     | 新增xiaobaicmd -u命令               |
+| 2.0     | 新增xiaobaicmd -m命令               |
+| 2.1     | 新增xiaobaicmd --device命令         |
+| 2.2     | 优化xiaobaicmd --device命令         |
+| 2.3     | 新增实时监控Android设备耗电量              |
+| 2.3.1   | fix                             |
+| 2.3.2   | fix                             |
+| 2.3.3   | 新增实时监控Android当前APP的内存使用率        |
+| 2.3.4   | 优化xiaobaicmd -m gui效果展示         |
+| 2.3.5   | 优化xiaobaicmd -u 转PO代码时xpath的表达式 |
```

### Comparing `xiaobaisaf-2.3.4/README.md` & `xiaobaisaf-2.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
     - ('xiaobai', '12346', 200)
     - ('xiaohui', '123456', 200)
 ```
 
 ### saf>1.8 基于selenium完成正常的页面操作，工具会自动在当前目录下生成Pages目录，目录内会自动生成当前打开的所有页面的PageObject代码，命令如下：
 ```cmd
 xiaobaicmd -u URL 
-xiaobaicmd -url URL 
+xiaobaicmd --url URL 
 ```
 
 ### saf>1.9  基于adb实现监控Android设备中APP操作时实时生成XPath表达式及坐标等数据
 ```cmd
 xiaobaicmd -m gui             # 基于界面实时获取APP数据
 xiaobaicmd --monitor gui      # 基于界面实时获取APP数据
 xiaobaicmd -m cli             # 基于命令实时获取APP数据
@@ -303,27 +303,28 @@
 
 [163邮箱配置](http://help.163.com/09/1223/14/5R7P3QI100753VB8.html, "163邮箱配置")
 
 [QQ邮箱配置](https://service.mail.qq.com/cgi-bin/help?subtype=1&id=28&no=369, "QQ邮箱配置")
 
 ### 更新日志
 
-| version | info                     |
-|---------|--------------------------|
-| 1.0     | 基本实现web自动化模板功能           |
-| 1.1     | fix上个版本的BUG              |
-| 1.2     | 新增allure报告库及封装禅道提单接口     |
-| 1.3     | 新增jira提单接口               |
-| 1.4     | 新增pytest参数化样例            |
-| 1.5     | 优化pytest样例内容             |
-| 1.6     | 优化                       |
-| 1.7     | 新增基础环境检测功能               |
-| 1.8     | 新增API自动化模板               |
-| 1.9     | 新增xiaobaicmd -u命令        |
-| 2.0     | 新增xiaobaicmd -m命令        |
-| 2.1     | 新增xiaobaicmd --device命令  |
-| 2.2     | 优化xiaobaicmd --device命令  |
-| 2.3     | 新增实时监控Android设备耗电量       |
-| 2.3.1   | fix                      |
-| 2.3.2   | fix                      |
-| 2.3.3   | 新增实时监控Android当前APP的内存使用率 |
-| 2.3.4   | 优化xiaobaicmd -m gui效果展示  |
+| version | info                            |
+|---------|---------------------------------|
+| 1.0     | 基本实现web自动化模板功能                  |
+| 1.1     | fix上个版本的BUG                     |
+| 1.2     | 新增allure报告库及封装禅道提单接口            |
+| 1.3     | 新增jira提单接口                      |
+| 1.4     | 新增pytest参数化样例                   |
+| 1.5     | 优化pytest样例内容                    |
+| 1.6     | 优化                              |
+| 1.7     | 新增基础环境检测功能                      |
+| 1.8     | 新增API自动化模板                      |
+| 1.9     | 新增xiaobaicmd -u命令               |
+| 2.0     | 新增xiaobaicmd -m命令               |
+| 2.1     | 新增xiaobaicmd --device命令         |
+| 2.2     | 优化xiaobaicmd --device命令         |
+| 2.3     | 新增实时监控Android设备耗电量              |
+| 2.3.1   | fix                             |
+| 2.3.2   | fix                             |
+| 2.3.3   | 新增实时监控Android当前APP的内存使用率        |
+| 2.3.4   | 优化xiaobaicmd -m gui效果展示         |
+| 2.3.5   | 优化xiaobaicmd -u 转PO代码时xpath的表达式 |
```

### Comparing `xiaobaisaf-2.3.4/saf/__init__.py` & `xiaobaisaf-2.3.5/saf/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/data/config.py` & `xiaobaisaf-2.3.5/saf/data/config.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/data/favicon.ico` & `xiaobaisaf-2.3.5/saf/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/example/api/Config/config.py` & `xiaobaisaf-2.3.5/saf/example/api/Config/config.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/example/api/TestCases/test_one_html_case_template.py` & `xiaobaisaf-2.3.5/saf/example/api/TestCases/test_one_html_case_template.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/example/api/Utils/ExcelUtils.py` & `xiaobaisaf-2.3.5/saf/example/api/Utils/ExcelUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/example/api/Utils/YamlUtils.py` & `xiaobaisaf-2.3.5/saf/example/api/Utils/YamlUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/example/api/Utils/api_client.py` & `xiaobaisaf-2.3.5/saf/example/api/Utils/api_client.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/example/api/run.py` & `xiaobaisaf-2.3.5/saf/example/api/run.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/example/api/send_email_script.py` & `xiaobaisaf-2.3.5/saf/example/api/send_email_script.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/example/web/Cases/conftest.py` & `xiaobaisaf-2.3.5/saf/example/web/Cases/conftest.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/example/web/Cases/test_xiaobai_case_allure.py` & `xiaobaisaf-2.3.5/saf/example/web/Cases/test_xiaobai_case_allure.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/example/web/Cases/test_xiaobai_case_submitBug.py` & `xiaobaisaf-2.3.5/saf/example/web/Cases/test_xiaobai_case_submitBug.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/example/web/Cases/test_xiaobai_case_v2.py` & `xiaobaisaf-2.3.5/saf/example/web/Cases/test_xiaobai_case_v2.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/example/web/Utils/ExcelUtils.py` & `xiaobaisaf-2.3.5/saf/example/web/Utils/ExcelUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/example/web/Utils/YamlUtils.py` & `xiaobaisaf-2.3.5/saf/example/web/Utils/YamlUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/utils/BugUtils.py` & `xiaobaisaf-2.3.5/saf/utils/BugUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/utils/MonitorAndroidDeviceGUI.py` & `xiaobaisaf-2.3.5/saf/utils/MonitorAndroidDeviceGUI.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/utils/MonitorAndroidPackageCLI.py` & `xiaobaisaf-2.3.5/saf/utils/MonitorAndroidPackageCLI.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/utils/MonitorAndroidPackageGUI.py` & `xiaobaisaf-2.3.5/saf/utils/MonitorAndroidPackageGUI.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/utils/MonitorAndroidPackagePower.py` & `xiaobaisaf-2.3.5/saf/utils/MonitorAndroidPackagePower.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/utils/MonitorDBs.py` & `xiaobaisaf-2.3.5/saf/utils/MonitorDBs.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/utils/YamlUtils.py` & `xiaobaisaf-2.3.5/saf/utils/YamlUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/utils/downloadUtils.py` & `xiaobaisaf-2.3.5/saf/utils/downloadUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/utils/elementUtils.py` & `xiaobaisaf-2.3.5/saf/utils/elementUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/utils/imageUtils.py` & `xiaobaisaf-2.3.5/saf/utils/imageUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/utils/networkSpeedUtils.py` & `xiaobaisaf-2.3.5/saf/utils/networkSpeedUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/utils/selenium2POM.py` & `xiaobaisaf-2.3.5/saf/utils/selenium2POM.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @Author: xiaobaiTser
 @Email : 807447312@qq.com
 @Time  : 2023/6/12 22:48
-@File  : HTML2POM.py
+@File  : selenium2POM.py
 '''
 import re
+import logging
+from time import sleep
 from os import path, mkdir, remove
 from bs4 import BeautifulSoup
+from lxml import etree
 from pypinyin import lazy_pinyin
 from selenium import webdriver
+from webdriver_manager.chrome import ChromeDriverManager
 from selenium.common.exceptions import NoSuchWindowException
 
 
 class PageListener:
     def __init__(self, start_url: str = 'https://www.baidu.com', dirname: str = '.', rewrite: bool = True):
         '''
         基于Selenium基础操作过程中将每页内容转为POM
         :param to_str       : True将结果转为字符串返回 ,False将结果写入到脚本，自动输出到Pages包中
         '''
+        self.PY_FILE_NAME_LIST = []
         if rewrite and path.exists(f'{dirname}/Pages'):
             try:
                 remove(f'{dirname}/Pages')
             except PermissionError as e:
                 pass
         if not path.exists(f'{dirname}/Pages'):
             mkdir('Pages')
@@ -32,155 +37,189 @@
                 f.write('''#! /usr/bin/env python
                 
 #********************************#
 #    欢迎使用自动生成POM代码工具      #
 #      Auther:xiaobaiTser        #
 #********************************#
 
+import logging
 from selenium import webdriver
+from webdriver_manager.chrome import ChromeDriverManager
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.action_chains import ActionChains
+
+driver = webdriver.Chrome(ChromeDriverManager(log_level=logging.CRITICAL).install())
                 ''')
                 f.close()
 
-        driver = webdriver.Chrome()
-        driver.get(start_url)
-        driver.implicitly_wait(30)
-        new_title = ''.join(re.findall('\w+', driver.title))
+        self.driver = webdriver.Chrome(ChromeDriverManager(log_level=logging.CRITICAL).install())
+        self.driver.get(start_url)
+        self.driver.implicitly_wait(30)
+        new_title = ''.join(re.findall('\w+', self.driver.title))
+        filename = "_".join(lazy_pinyin(new_title)).title()
+        new_filename = filename if self.PY_FILE_NAME_LIST.count(
+            filename) == 0 else f'{filename}_{self.PY_FILE_NAME_LIST.count(filename)}'
+        self.PY_FILE_NAME_LIST.append(filename)
         self.code2file(
-            code=self.identify_inputs_and_buttons(driver.current_url, driver.page_source),
-            filename=f'{dirname}/Pages/{"_".join(lazy_pinyin(new_title)).title()}.py')
+            code=self.identify_inputs_and_buttons(self.driver.current_url, self.driver.page_source),
+            filename=f'{dirname}/Pages/{new_filename}.py')
         # 监视浏览器URL变化、标签页变化
-        old_url = driver.current_url
-        old_handles = driver.window_handles
+        self.PageUrls = {self.driver.current_url}
+        self.PageHandles = self.driver.window_handles
         while True:
+            sleep(0.2)
             try:
-                new_url = driver.current_url
-                new_handles = driver.window_handles
-                if len(new_handles) > len(old_handles):
-                    driver.switch_to.window(list(set(new_handles)-set(old_handles))[0])
-                    new_title = ''.join(re.findall('\w+', driver.title))
-                    self.code2file(
-                        code=self.identify_inputs_and_buttons(driver.current_url, driver.page_source),
-                        filename=f'{dirname}/Pages/{"_".join(lazy_pinyin(new_title)).title()}.py')
-                    old_handles = new_handles
-                elif new_url != old_url:
-                    new_title = ''.join(re.findall('\w+', driver.title))
+                cur_url = self.driver.current_url
+                cur_handles = self.driver.window_handles
+                if cur_url not in self.PageUrls:
+                    self.PageUrls.add(cur_url)
+                    new_title = ''.join(re.findall('\w+', self.driver.title))
+                    filename = "_".join(lazy_pinyin(new_title)).title()
+                    new_filename = filename if self.PY_FILE_NAME_LIST.count(
+                        filename) == 0 else f'{filename}_{self.PY_FILE_NAME_LIST.count(filename)}'
+                    self.PY_FILE_NAME_LIST.append(filename)
                     self.code2file(
-                        code=self.identify_inputs_and_buttons(driver.current_url, driver.page_source),
-                        filename=f'{dirname}/Pages/{"_".join(lazy_pinyin(new_title)).title()}.py')
+                        code=self.identify_inputs_and_buttons(self.driver.current_url, self.driver.page_source),
+                        filename=f'{dirname}/Pages/{new_filename}.py')
+                if cur_handles != self.PageHandles:
+                    for handle in cur_handles:
+                        self.driver.switch_to.window(handle)
+                        if self.driver.current_url not in self.PageUrls:
+                            self.PageUrls.add(self.driver.current_url)
+                            new_title = ''.join(re.findall('\w+', self.driver.title))
+                            filename = "_".join(lazy_pinyin(new_title)).title()
+                            new_filename = filename if self.PY_FILE_NAME_LIST.count(
+                                filename) == 0 else f'{filename}_{self.PY_FILE_NAME_LIST.count(filename)}'
+                            self.PY_FILE_NAME_LIST.append(filename)
+                            self.code2file(
+                                code=self.identify_inputs_and_buttons(self.driver.current_url, self.driver.page_source),
+                                filename=f'{dirname}/Pages/{new_filename}.py')
+                    self.PageHandles = self.driver.window_handles
             except KeyboardInterrupt as e:
                 exit(-1)
             except NoSuchWindowException as e:
                 exit(-2)
 
-    @classmethod
-    def code2file(cls, code: str, filename: str = None):
+    def code2file(self, code: str, filename: str = None):
         with open(filename, 'w', encoding='UTF-8') as f:
             f.write(code)
             f.close()
             del f
 
-    @classmethod
-    def identify_inputs_and_buttons(cls, url, html):
+    def identify_inputs_and_buttons(self, url, html):
         '''
         1、解析HTML获取输入框与按钮并获取xpath表达式
         2、将输入框与按钮转为POM代码，一个页面单独一个脚本，一个脚本单独一个类
+        :param url:
         :param html:
         :return:
         '''
         soup = BeautifulSoup(html, 'html.parser')
         find_all_input = soup.find_all(['input', 'textarea'])
         find_all_button = soup.find_all('button')
         find_all_button.extend(soup.find_all('a'))
+        find_all_button.extend(soup.find_all('select'))
+        find_all_button.extend(soup.find_all('optgroup'))
+        find_all_button.extend(soup.find_all('option'))
         find_all_button.extend(soup.find_all('input', attrs={'type': ['button', 'submit']}))
         input_list = []
         button_list = []
         for input_tag in find_all_input:
             if input_tag not in soup.find_all('input', attrs={'type': ['button', 'submit', 'hidden']}):
                 input_name = input_tag.get('name') or input_tag.name
-                input_xpath = cls.get_xpath(input_tag)
+                input_xpath = self.get_xpath(input_tag)
                 if input_name:
                     input_list.append({'tag': input_tag, 'name': input_name, 'xpath': input_xpath})
         for button_tag in find_all_button:
             button_name = button_tag.get('name') or button_tag.text.strip() or button_tag.name
-            button_xpath = cls.get_xpath(button_tag)
+            button_xpath = self.get_xpath(button_tag)
             button_list.append({'tag': button_tag, 'name': button_name, 'xpath': button_xpath})
         title = '_'.join(lazy_pinyin(soup.select("title")[0].text)).upper()
         title = ''.join(re.findall('[0-9a-zA-Z_]+', title))
-        return cls.converter(page_name=title, url=url,
+        return self.converter(page_name=title, url=url,
                               input_list=input_list, button_list=button_list)
 
-    @classmethod
-    def get_xpath(cls, element):
+    def get_xpath(self, element):
         components = []
         child = element
         while child is not None:
             siblings = child.find_previous_siblings()
             index = len(siblings) + 1
             if child.name == 'html':
                 components.insert(0, '/html')
                 break
             if child.name == 'body':
                 components.insert(0, '/body')
                 break
+            else:
+                element_attrs_dict = child.attrs
+                for k, v in element_attrs_dict.items():
+                    if k in element_attrs_dict.keys() and '' != element_attrs_dict[k]:
+                        html = etree.HTML(self.driver.page_source)
+                        query_result = html.xpath(f'//{child.name}[@{k}="{element_attrs_dict[k]}"]')
+                        if len(query_result) == 1:
+                            components.insert(0, f'/{child.name}[@{k}="{element_attrs_dict[k]}"]')
+                            xpath = ''.join(components)
+                            xpath = xpath if xpath.startswith('/html') else '/' + xpath
+                            return xpath
+                        else:
+                            continue
             components.insert(0, f'/{child.name}[{index}]')
             child = child.parent
         xpath = ''.join(components)
         xpath = xpath if xpath.startswith('/html') else '/' + xpath
         return xpath
 
-    @classmethod
-    def converter(cls, page_name: str, url: str, input_list: list, button_list: list):
+    def converter(self, page_name: str, url: str, input_list: list, button_list: list):
         function_strings = []
         function_names = []
         function_strings.append('#! /usr/bin/env python')
         function_strings.append(f'')
         function_strings.append('#********************************#')
         function_strings.append('#    欢迎使用自动生成POM代码工具      #')
         function_strings.append('#      Auther:xiaobaiTser        #')
         function_strings.append('#********************************#')
         function_strings.append(f'')
         function_strings.append('from selenium.webdriver.common.by import By')
         function_strings.append(f'')
         function_strings.append(f'class {page_name}:')
         function_strings.append('\tdef __init__(self, driver):')
-        function_strings.append(f'\t\t# 当前URL: {url}')
+        function_strings.append(f'\t\t# 当前页面URL: {url}')
         function_strings.append('\t\tself.driver = driver')
         function_strings.append(f'')
         for input_item in input_list:
             function_name = "_".join(lazy_pinyin(input_item['name']))
             function_name = ''.join(re.findall('[0-9a-zA-Z_]+', function_name))
+            new_function_name = function_name if function_names.count(function_name) == 0 else \
+                f'{function_name}_{function_names.count(function_name)}'
             function_names.append(function_name)
-            if function_names.count(function_name) > 1:
-                function_name = f'{function_name}_{function_names.count(function_name)-1}'
             xpath = input_item['xpath']
-            function_strings.append(f'\tdef send_{function_name}(self, data):')
+            function_strings.append(f'\tdef send_{new_function_name}(self, data):')
             function_strings.append("\t\t'''")
             function_strings.append('\t\t当前元素：')
             input_item['tag'] = str(input_item['tag']).replace('\n', '\n\t\t')
             function_strings.append(f"\t\t{input_item['tag']}")
             function_strings.append("\t\t'''")
-            function_strings.append(f'\t\tself.driver.find_element(By.XPATH, "{xpath}").send_keys(data)')
+            function_strings.append(f'\t\tself.driver.find_element(By.XPATH, \'{xpath}\').send_keys(data)')
             function_strings.append(f'')
         for button_item in button_list:
             function_name = "_".join(lazy_pinyin(button_item['name']))
             function_name = ''.join(re.findall('[0-9a-zA-Z_]+', function_name))
+            new_function_name = function_name if function_names.count(function_name) == 0 else \
+                f'{function_name}_{function_names.count(function_name)}'
             function_names.append(function_name)
-            if function_names.count(function_name) > 1:
-                function_name = f'{function_name}_{function_names.count(function_name)-1}'
             xpath = button_item['xpath']
-            function_strings.append(f'\tdef click_{function_name}(self):')
+            function_strings.append(f'\tdef click_{new_function_name}(self):')
             function_strings.append("\t\t'''")
             function_strings.append('\t\t当前元素：')
             button_item['tag'] = str(button_item['tag']).replace('\n', '\n\t\t')
             function_strings.append(f"\t\t{button_item['tag']}")
             function_strings.append("\t\t'''")
-            function_strings.append(f'\t\tself.driver.find_element(By.XPATH, "{xpath}").click()')
+            function_strings.append(f'\t\tself.driver.find_element(By.XPATH, \'{xpath}\').click()')
             function_strings.append(f'')
         return '\n'.join(function_strings)
 
-# if __name__ == '__main__':
-#     PageListener()
+if __name__ == '__main__':
+    PageListener(start_url='https://www.zhiguanpo.com/#/')
```

### Comparing `xiaobaisaf-2.3.4/saf/utils/sendMsgUtils.py` & `xiaobaisaf-2.3.5/saf/utils/sendMsgUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/saf/utils/xiaobaicmd.py` & `xiaobaisaf-2.3.5/saf/utils/xiaobaicmd.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.4/setup.py` & `xiaobaisaf-2.3.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     entry_points={
         'console_scripts': [
             'xiaobaicmd = saf.utils.xiaobaicmd:main'
         ]
     },
     data_files=[
         ('favicon', ['saf/data/favicon.ico']),
+        ('software_check_sh', ['saf/data/software_check.sh']),
     ]
 )
 
 '''
 #python setup.py sdist bdist_wheel
 #python -m twine upload dist/*
 '''
```

### Comparing `xiaobaisaf-2.3.4/xiaobaisaf.egg-info/PKG-INFO` & `xiaobaisaf-2.3.5/xiaobaisaf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaobaisaf
-Version: 2.3.4
+Version: 2.3.5
 Summary: simple_automation_framework(简称：SAF)使用最简单的模式就可以实现需要功能和测试效果，也是xiaobaiauto2的简化版SAF继承了selenium、requests/httpx、appium、loguru、xiaobaiauto2、飞书机器人、钉钉机器人、企业微信机器人（暂时不支持）、禅道提单API
 Home-page: https://gitee.com/xiaobaikeji/simlpe_automation_framework
 Author: xiaobaiTser
 Author-email: 807447312@qq.com
 Keywords: saf test auto automation xiaobai xiaobaiauto2 test framework
 Requires-Python: >=3.6, <3.10
 Description-Content-Type: text/markdown
@@ -260,15 +260,15 @@
     - ('xiaobai', '12346', 200)
     - ('xiaohui', '123456', 200)
 ```
 
 ### saf>1.8 基于selenium完成正常的页面操作，工具会自动在当前目录下生成Pages目录，目录内会自动生成当前打开的所有页面的PageObject代码，命令如下：
 ```cmd
 xiaobaicmd -u URL 
-xiaobaicmd -url URL 
+xiaobaicmd --url URL 
 ```
 
 ### saf>1.9  基于adb实现监控Android设备中APP操作时实时生成XPath表达式及坐标等数据
 ```cmd
 xiaobaicmd -m gui             # 基于界面实时获取APP数据
 xiaobaicmd --monitor gui      # 基于界面实时获取APP数据
 xiaobaicmd -m cli             # 基于命令实时获取APP数据
@@ -315,27 +315,28 @@
 
 [163邮箱配置](http://help.163.com/09/1223/14/5R7P3QI100753VB8.html, "163邮箱配置")
 
 [QQ邮箱配置](https://service.mail.qq.com/cgi-bin/help?subtype=1&id=28&no=369, "QQ邮箱配置")
 
 ### 更新日志
 
-| version | info                     |
-|---------|--------------------------|
-| 1.0     | 基本实现web自动化模板功能           |
-| 1.1     | fix上个版本的BUG              |
-| 1.2     | 新增allure报告库及封装禅道提单接口     |
-| 1.3     | 新增jira提单接口               |
-| 1.4     | 新增pytest参数化样例            |
-| 1.5     | 优化pytest样例内容             |
-| 1.6     | 优化                       |
-| 1.7     | 新增基础环境检测功能               |
-| 1.8     | 新增API自动化模板               |
-| 1.9     | 新增xiaobaicmd -u命令        |
-| 2.0     | 新增xiaobaicmd -m命令        |
-| 2.1     | 新增xiaobaicmd --device命令  |
-| 2.2     | 优化xiaobaicmd --device命令  |
-| 2.3     | 新增实时监控Android设备耗电量       |
-| 2.3.1   | fix                      |
-| 2.3.2   | fix                      |
-| 2.3.3   | 新增实时监控Android当前APP的内存使用率 |
-| 2.3.4   | 优化xiaobaicmd -m gui效果展示  |
+| version | info                            |
+|---------|---------------------------------|
+| 1.0     | 基本实现web自动化模板功能                  |
+| 1.1     | fix上个版本的BUG                     |
+| 1.2     | 新增allure报告库及封装禅道提单接口            |
+| 1.3     | 新增jira提单接口                      |
+| 1.4     | 新增pytest参数化样例                   |
+| 1.5     | 优化pytest样例内容                    |
+| 1.6     | 优化                              |
+| 1.7     | 新增基础环境检测功能                      |
+| 1.8     | 新增API自动化模板                      |
+| 1.9     | 新增xiaobaicmd -u命令               |
+| 2.0     | 新增xiaobaicmd -m命令               |
+| 2.1     | 新增xiaobaicmd --device命令         |
+| 2.2     | 优化xiaobaicmd --device命令         |
+| 2.3     | 新增实时监控Android设备耗电量              |
+| 2.3.1   | fix                             |
+| 2.3.2   | fix                             |
+| 2.3.3   | 新增实时监控Android当前APP的内存使用率        |
+| 2.3.4   | 优化xiaobaicmd -m gui效果展示         |
+| 2.3.5   | 优化xiaobaicmd -u 转PO代码时xpath的表达式 |
```

### Comparing `xiaobaisaf-2.3.4/xiaobaisaf.egg-info/SOURCES.txt` & `xiaobaisaf-2.3.5/xiaobaisaf.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 saf/__init__.py
 saf/__version__.py
 saf/data/__init__.py
 saf/data/config.py
 saf/data/favicon.ico
+saf/data/software_check.sh
 saf/example/__init__.py
 saf/example/api/__init__.py
 saf/example/api/run.py
 saf/example/api/send_email_script.py
 saf/example/api/Config/__init__.py
 saf/example/api/Config/config.py
 saf/example/api/TestCases/__init__.py
```

