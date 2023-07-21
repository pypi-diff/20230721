# Comparing `tmp/alibabacloud_dingtalk-2.0.25.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.25.tar", last modified: Wed Jul 19 03:10:17 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.26.tar", last modified: Fri Jul 21 10:56:53 2023, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.25.tar` & `alibabacloud_dingtalk-2.0.26.tar`

### file list

```diff
@@ -1,381 +1,381 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/
--rw-r--r--   0 root         (0) root         (0)    20272 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8552 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15385 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23314 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169621 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46194 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25682 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    27728 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90914 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   139242 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   165948 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   323041 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62246 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   202090 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   576378 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9614 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10132 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   142048 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   346941 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42229 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39942 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   106288 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10446 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123179 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   126888 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   172646 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124904 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   297108 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   392984 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42332 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23872 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33155 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30852 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223914 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   552073 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7385 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46898 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515455 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152480 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ding_phone_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13874 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ding_phone_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16265 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ding_phone_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56301 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    57073 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    75811 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   219916 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   278738 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150160 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   269893 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   195538 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   472940 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   731141 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   116546 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123749 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8259 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8976 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   316592 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   439557 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155788 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   302125 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13914 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21801 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4633 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4901 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138362 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18903 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    95111 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   139534 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302740 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   379213 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22430 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    31875 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    92472 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   610684 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   859772 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155140 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108695 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135110 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_activities_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_activities_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9852 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_activities_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14366 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_activities_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148979 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   177099 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54521 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31076 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40802 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7507 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76720 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137701 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123420 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60347 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69069 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   264898 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   419073 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/report_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/report_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8048 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/report_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    12289 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/report_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   174524 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94300 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   106806 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56986 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83842 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46018 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   361006 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503423 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26678 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    96217 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   353698 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53470 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    89290 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28559 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65344 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148231 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16170 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21677 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17519 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19158 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32757 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110849 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4269 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20486 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   130783 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32014 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    34941 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   179772 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   377816 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   464194 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   687148 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4490 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12583 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2685 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/
+-rw-r--r--   0 root         (0) root         (0)    20337 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8552 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15385 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23314 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169621 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25682 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    27728 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90914 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   139242 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   165948 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   323041 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62246 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   205984 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   590436 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9614 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10132 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   142048 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   346941 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42229 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39942 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   106288 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10446 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   126888 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   172646 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124904 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   297108 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   392984 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23872 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33155 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30852 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223914 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   552073 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46898 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515455 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152480 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13874 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16265 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56301 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    57073 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    75811 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   219916 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   278738 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   150160 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   269893 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   195538 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   472940 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   731141 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   116546 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123749 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8259 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8976 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   316592 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   439557 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155788 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   302125 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13914 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21801 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4901 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138362 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18903 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    95111 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   139534 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302740 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   379213 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22430 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    31875 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   610684 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   859772 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   155140 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108695 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135110 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_activities_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_activities_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9852 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_activities_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14366 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_activities_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   148979 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   177099 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54521 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40802 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137701 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123420 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60347 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69069 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   264898 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   419073 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/report_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/report_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8048 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/report_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    12289 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/report_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   174524 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94300 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   106806 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56986 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83842 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46018 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   361006 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503423 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26678 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    96217 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   353698 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53470 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    89290 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28559 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65344 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148231 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21677 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17519 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19158 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32757 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20486 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   130783 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32014 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    34941 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   179772 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   377816 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   464194 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   687148 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4490 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12583 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2685 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.25/ChangeLog.md` & `alibabacloud_dingtalk-2.0.26/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-19 Version: 2.0.25
+- Update AddOfficialAccountFollower.
+
 2023-07-17 Version: 2.0.24
 - Update AddOfficialAccountFollower.
 
 2023-07-12 Version: 2.0.23
 - Update AddOfficialAccountFollower.
 
 2023-07-05 Version: 2.0.22
```

### Comparing `alibabacloud_dingtalk-2.0.25/LICENSE` & `alibabacloud_dingtalk-2.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/PKG-INFO` & `alibabacloud_dingtalk-2.0.26/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.25
+Version: 2.0.26
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.25/README-CN.md` & `alibabacloud_dingtalk-2.0.26/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/README.md` & `alibabacloud_dingtalk-2.0.26/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1457,14 +1457,100 @@
         self,
         request: dingtalkbizfinance__1__0_models.GetSupplierRequest,
     ) -> dingtalkbizfinance__1__0_models.GetSupplierResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkbizfinance__1__0_models.GetSupplierHeaders()
         return await self.get_supplier_with_options_async(request, headers, runtime)
 
+    def get_yong_you_open_api_token_with_options(
+        self,
+        request: dingtalkbizfinance__1__0_models.GetYongYouOpenApiTokenRequest,
+        headers: dingtalkbizfinance__1__0_models.GetYongYouOpenApiTokenHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkbizfinance__1__0_models.GetYongYouOpenApiTokenResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetYongYouOpenApiToken',
+            version='bizfinance_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/bizfinance/yongyou/token',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkbizfinance__1__0_models.GetYongYouOpenApiTokenResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_yong_you_open_api_token_with_options_async(
+        self,
+        request: dingtalkbizfinance__1__0_models.GetYongYouOpenApiTokenRequest,
+        headers: dingtalkbizfinance__1__0_models.GetYongYouOpenApiTokenHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkbizfinance__1__0_models.GetYongYouOpenApiTokenResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetYongYouOpenApiToken',
+            version='bizfinance_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/bizfinance/yongyou/token',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkbizfinance__1__0_models.GetYongYouOpenApiTokenResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_yong_you_open_api_token(
+        self,
+        request: dingtalkbizfinance__1__0_models.GetYongYouOpenApiTokenRequest,
+    ) -> dingtalkbizfinance__1__0_models.GetYongYouOpenApiTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkbizfinance__1__0_models.GetYongYouOpenApiTokenHeaders()
+        return self.get_yong_you_open_api_token_with_options(request, headers, runtime)
+
+    async def get_yong_you_open_api_token_async(
+        self,
+        request: dingtalkbizfinance__1__0_models.GetYongYouOpenApiTokenRequest,
+    ) -> dingtalkbizfinance__1__0_models.GetYongYouOpenApiTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkbizfinance__1__0_models.GetYongYouOpenApiTokenHeaders()
+        return await self.get_yong_you_open_api_token_with_options_async(request, headers, runtime)
+
     def profession_benefit_consume_with_options(
         self,
         request: dingtalkbizfinance__1__0_models.ProfessionBenefitConsumeRequest,
         headers: dingtalkbizfinance__1__0_models.ProfessionBenefitConsumeHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkbizfinance__1__0_models.ProfessionBenefitConsumeResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4572,14 +4572,193 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetSupplierResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetYongYouOpenApiTokenHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class GetYongYouOpenApiTokenRequest(TeaModel):
+    def __init__(
+        self,
+        user_id: str = None,
+    ):
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class GetYongYouOpenApiTokenResponseBody(TeaModel):
+    def __init__(
+        self,
+        access_token: str = None,
+        app_name: str = None,
+        expires_in: str = None,
+        refresh_expires_in: str = None,
+        refresh_token: str = None,
+        scope: str = None,
+        sid: str = None,
+        yongyou_org_id: str = None,
+        yongyou_user_id: str = None,
+    ):
+        self.access_token = access_token
+        self.app_name = app_name
+        self.expires_in = expires_in
+        self.refresh_expires_in = refresh_expires_in
+        self.refresh_token = refresh_token
+        self.scope = scope
+        self.sid = sid
+        self.yongyou_org_id = yongyou_org_id
+        self.yongyou_user_id = yongyou_user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_token is not None:
+            result['accessToken'] = self.access_token
+        if self.app_name is not None:
+            result['appName'] = self.app_name
+        if self.expires_in is not None:
+            result['expiresIn'] = self.expires_in
+        if self.refresh_expires_in is not None:
+            result['refreshExpiresIn'] = self.refresh_expires_in
+        if self.refresh_token is not None:
+            result['refreshToken'] = self.refresh_token
+        if self.scope is not None:
+            result['scope'] = self.scope
+        if self.sid is not None:
+            result['sid'] = self.sid
+        if self.yongyou_org_id is not None:
+            result['yongyouOrgId'] = self.yongyou_org_id
+        if self.yongyou_user_id is not None:
+            result['yongyouUserId'] = self.yongyou_user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('accessToken') is not None:
+            self.access_token = m.get('accessToken')
+        if m.get('appName') is not None:
+            self.app_name = m.get('appName')
+        if m.get('expiresIn') is not None:
+            self.expires_in = m.get('expiresIn')
+        if m.get('refreshExpiresIn') is not None:
+            self.refresh_expires_in = m.get('refreshExpiresIn')
+        if m.get('refreshToken') is not None:
+            self.refresh_token = m.get('refreshToken')
+        if m.get('scope') is not None:
+            self.scope = m.get('scope')
+        if m.get('sid') is not None:
+            self.sid = m.get('sid')
+        if m.get('yongyouOrgId') is not None:
+            self.yongyou_org_id = m.get('yongyouOrgId')
+        if m.get('yongyouUserId') is not None:
+            self.yongyou_user_id = m.get('yongyouUserId')
+        return self
+
+
+class GetYongYouOpenApiTokenResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetYongYouOpenApiTokenResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetYongYouOpenApiTokenResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ProfessionBenefitConsumeHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -13529,14 +13708,77 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
+class UpdateInvoiceAndReceiptRelatedRequestGeneralInvoiceVOFlightItineraryDetails(TeaModel):
+    def __init__(
+        self,
+        carrier: str = None,
+        flight_number: str = None,
+        fly_date: str = None,
+        fly_from: str = None,
+        fly_time: str = None,
+        fly_to: str = None,
+        seat: str = None,
+    ):
+        self.carrier = carrier
+        self.flight_number = flight_number
+        self.fly_date = fly_date
+        self.fly_from = fly_from
+        self.fly_time = fly_time
+        self.fly_to = fly_to
+        self.seat = seat
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.carrier is not None:
+            result['carrier'] = self.carrier
+        if self.flight_number is not None:
+            result['flightNumber'] = self.flight_number
+        if self.fly_date is not None:
+            result['flyDate'] = self.fly_date
+        if self.fly_from is not None:
+            result['flyFrom'] = self.fly_from
+        if self.fly_time is not None:
+            result['flyTime'] = self.fly_time
+        if self.fly_to is not None:
+            result['flyTo'] = self.fly_to
+        if self.seat is not None:
+            result['seat'] = self.seat
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('carrier') is not None:
+            self.carrier = m.get('carrier')
+        if m.get('flightNumber') is not None:
+            self.flight_number = m.get('flightNumber')
+        if m.get('flyDate') is not None:
+            self.fly_date = m.get('flyDate')
+        if m.get('flyFrom') is not None:
+            self.fly_from = m.get('flyFrom')
+        if m.get('flyTime') is not None:
+            self.fly_time = m.get('flyTime')
+        if m.get('flyTo') is not None:
+            self.fly_to = m.get('flyTo')
+        if m.get('seat') is not None:
+            self.seat = m.get('seat')
+        return self
+
+
 class UpdateInvoiceAndReceiptRelatedRequestGeneralInvoiceVOGeneralInvoiceDetailVOList(TeaModel):
     def __init__(
         self,
         amount: str = None,
         goods_name: str = None,
         quantity: str = None,
         revenue_code: str = None,
@@ -13935,100 +14177,148 @@
         return self
 
 
 class UpdateInvoiceAndReceiptRelatedRequestGeneralInvoiceVO(TeaModel):
     def __init__(
         self,
         account_period: str = None,
+        agent_code: str = None,
         amount: str = None,
         amount_with_tax: str = None,
+        caac_development_fund: str = None,
         check_code: str = None,
         check_time: str = None,
+        city: str = None,
+        destination: str = None,
+        distance: str = None,
         drawer_name: str = None,
         drew_date: str = None,
         electronic_url: str = None,
+        entrance: str = None,
+        exit: str = None,
         finance_type: str = None,
+        flight_itinerary_details: List[UpdateInvoiceAndReceiptRelatedRequestGeneralInvoiceVOFlightItineraryDetails] = None,
+        fuel_surcharge: str = None,
         fund_type: str = None,
         general_invoice_detail_volist: List[UpdateInvoiceAndReceiptRelatedRequestGeneralInvoiceVOGeneralInvoiceDetailVOList] = None,
+        get_off_time: str = None,
+        get_on_time: str = None,
         image_url: str = None,
         invoice_code: str = None,
         invoice_no: str = None,
         invoice_status: str = None,
         invoice_type: str = None,
+        issue_by: str = None,
         machine_code: str = None,
         oil_flag: str = None,
+        origin: str = None,
+        passenger: str = None,
+        passenger_user_id: str = None,
         payee: str = None,
+        print_serial_number: str = None,
         process_inst_code: str = None,
         process_inst_type: str = None,
         purchaser_address: str = None,
         purchaser_bank_account: str = None,
         purchaser_bank_name_account: str = None,
         purchaser_name: str = None,
         purchaser_tax_no: str = None,
         purchaser_tel: str = None,
         remark: str = None,
+        seat_class: str = None,
         second_hand_car_invoice_detail_list: List[UpdateInvoiceAndReceiptRelatedRequestGeneralInvoiceVOSecondHandCarInvoiceDetailList] = None,
         seller_address: str = None,
         seller_bank_account: str = None,
         seller_bank_name_account: str = None,
         seller_name: str = None,
         seller_tax_no: str = None,
         seller_tel: str = None,
+        serial_no: str = None,
+        start_time: str = None,
         supply_sign: str = None,
+        surcharge: str = None,
         tax_amount: str = None,
+        train_no: str = None,
+        travel_date: str = None,
         used_vehicle_sale_detail_volist: List[UpdateInvoiceAndReceiptRelatedRequestGeneralInvoiceVOUsedVehicleSaleDetailVOList] = None,
         vehicle_sale_detail_volist: List[UpdateInvoiceAndReceiptRelatedRequestGeneralInvoiceVOVehicleSaleDetailVOList] = None,
         verify_status: str = None,
         voucher_code: str = None,
         voucher_status: str = None,
     ):
         self.account_period = account_period
+        self.agent_code = agent_code
         self.amount = amount
         self.amount_with_tax = amount_with_tax
+        self.caac_development_fund = caac_development_fund
         self.check_code = check_code
         self.check_time = check_time
+        self.city = city
+        self.destination = destination
+        self.distance = distance
         self.drawer_name = drawer_name
         self.drew_date = drew_date
         self.electronic_url = electronic_url
+        self.entrance = entrance
+        self.exit = exit
         self.finance_type = finance_type
+        self.flight_itinerary_details = flight_itinerary_details
+        self.fuel_surcharge = fuel_surcharge
         self.fund_type = fund_type
         self.general_invoice_detail_volist = general_invoice_detail_volist
+        self.get_off_time = get_off_time
+        self.get_on_time = get_on_time
         self.image_url = image_url
         self.invoice_code = invoice_code
         self.invoice_no = invoice_no
         self.invoice_status = invoice_status
         self.invoice_type = invoice_type
+        self.issue_by = issue_by
         self.machine_code = machine_code
         self.oil_flag = oil_flag
+        self.origin = origin
+        self.passenger = passenger
+        self.passenger_user_id = passenger_user_id
         self.payee = payee
+        self.print_serial_number = print_serial_number
         self.process_inst_code = process_inst_code
         self.process_inst_type = process_inst_type
         self.purchaser_address = purchaser_address
         self.purchaser_bank_account = purchaser_bank_account
         self.purchaser_bank_name_account = purchaser_bank_name_account
         self.purchaser_name = purchaser_name
         self.purchaser_tax_no = purchaser_tax_no
         self.purchaser_tel = purchaser_tel
         self.remark = remark
+        self.seat_class = seat_class
         self.second_hand_car_invoice_detail_list = second_hand_car_invoice_detail_list
         self.seller_address = seller_address
         self.seller_bank_account = seller_bank_account
         self.seller_bank_name_account = seller_bank_name_account
         self.seller_name = seller_name
         self.seller_tax_no = seller_tax_no
         self.seller_tel = seller_tel
+        self.serial_no = serial_no
+        self.start_time = start_time
         self.supply_sign = supply_sign
+        self.surcharge = surcharge
         self.tax_amount = tax_amount
+        self.train_no = train_no
+        self.travel_date = travel_date
         self.used_vehicle_sale_detail_volist = used_vehicle_sale_detail_volist
         self.vehicle_sale_detail_volist = vehicle_sale_detail_volist
         self.verify_status = verify_status
         self.voucher_code = voucher_code
         self.voucher_status = voucher_status
 
     def validate(self):
+        if self.flight_itinerary_details:
+            for k in self.flight_itinerary_details:
+                if k:
+                    k.validate()
         if self.general_invoice_detail_volist:
             for k in self.general_invoice_detail_volist:
                 if k:
                     k.validate()
         if self.second_hand_car_invoice_detail_list:
             for k in self.second_hand_car_invoice_detail_list:
                 if k:
@@ -14046,52 +14336,86 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.account_period is not None:
             result['accountPeriod'] = self.account_period
+        if self.agent_code is not None:
+            result['agentCode'] = self.agent_code
         if self.amount is not None:
             result['amount'] = self.amount
         if self.amount_with_tax is not None:
             result['amountWithTax'] = self.amount_with_tax
+        if self.caac_development_fund is not None:
+            result['caacDevelopmentFund'] = self.caac_development_fund
         if self.check_code is not None:
             result['checkCode'] = self.check_code
         if self.check_time is not None:
             result['checkTime'] = self.check_time
+        if self.city is not None:
+            result['city'] = self.city
+        if self.destination is not None:
+            result['destination'] = self.destination
+        if self.distance is not None:
+            result['distance'] = self.distance
         if self.drawer_name is not None:
             result['drawerName'] = self.drawer_name
         if self.drew_date is not None:
             result['drewDate'] = self.drew_date
         if self.electronic_url is not None:
             result['electronicUrl'] = self.electronic_url
+        if self.entrance is not None:
+            result['entrance'] = self.entrance
+        if self.exit is not None:
+            result['exit'] = self.exit
         if self.finance_type is not None:
             result['financeType'] = self.finance_type
+        result['flightItineraryDetails'] = []
+        if self.flight_itinerary_details is not None:
+            for k in self.flight_itinerary_details:
+                result['flightItineraryDetails'].append(k.to_map() if k else None)
+        if self.fuel_surcharge is not None:
+            result['fuelSurcharge'] = self.fuel_surcharge
         if self.fund_type is not None:
             result['fundType'] = self.fund_type
         result['generalInvoiceDetailVOList'] = []
         if self.general_invoice_detail_volist is not None:
             for k in self.general_invoice_detail_volist:
                 result['generalInvoiceDetailVOList'].append(k.to_map() if k else None)
+        if self.get_off_time is not None:
+            result['getOffTime'] = self.get_off_time
+        if self.get_on_time is not None:
+            result['getOnTime'] = self.get_on_time
         if self.image_url is not None:
             result['imageUrl'] = self.image_url
         if self.invoice_code is not None:
             result['invoiceCode'] = self.invoice_code
         if self.invoice_no is not None:
             result['invoiceNo'] = self.invoice_no
         if self.invoice_status is not None:
             result['invoiceStatus'] = self.invoice_status
         if self.invoice_type is not None:
             result['invoiceType'] = self.invoice_type
+        if self.issue_by is not None:
+            result['issueBy'] = self.issue_by
         if self.machine_code is not None:
             result['machineCode'] = self.machine_code
         if self.oil_flag is not None:
             result['oilFlag'] = self.oil_flag
+        if self.origin is not None:
+            result['origin'] = self.origin
+        if self.passenger is not None:
+            result['passenger'] = self.passenger
+        if self.passenger_user_id is not None:
+            result['passengerUserId'] = self.passenger_user_id
         if self.payee is not None:
             result['payee'] = self.payee
+        if self.print_serial_number is not None:
+            result['printSerialNumber'] = self.print_serial_number
         if self.process_inst_code is not None:
             result['processInstCode'] = self.process_inst_code
         if self.process_inst_type is not None:
             result['processInstType'] = self.process_inst_type
         if self.purchaser_address is not None:
             result['purchaserAddress'] = self.purchaser_address
         if self.purchaser_bank_account is not None:
@@ -14102,14 +14426,16 @@
             result['purchaserName'] = self.purchaser_name
         if self.purchaser_tax_no is not None:
             result['purchaserTaxNo'] = self.purchaser_tax_no
         if self.purchaser_tel is not None:
             result['purchaserTel'] = self.purchaser_tel
         if self.remark is not None:
             result['remark'] = self.remark
+        if self.seat_class is not None:
+            result['seatClass'] = self.seat_class
         result['secondHandCarInvoiceDetailList'] = []
         if self.second_hand_car_invoice_detail_list is not None:
             for k in self.second_hand_car_invoice_detail_list:
                 result['secondHandCarInvoiceDetailList'].append(k.to_map() if k else None)
         if self.seller_address is not None:
             result['sellerAddress'] = self.seller_address
         if self.seller_bank_account is not None:
@@ -14118,18 +14444,28 @@
             result['sellerBankNameAccount'] = self.seller_bank_name_account
         if self.seller_name is not None:
             result['sellerName'] = self.seller_name
         if self.seller_tax_no is not None:
             result['sellerTaxNo'] = self.seller_tax_no
         if self.seller_tel is not None:
             result['sellerTel'] = self.seller_tel
+        if self.serial_no is not None:
+            result['serialNo'] = self.serial_no
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
         if self.supply_sign is not None:
             result['supplySign'] = self.supply_sign
+        if self.surcharge is not None:
+            result['surcharge'] = self.surcharge
         if self.tax_amount is not None:
             result['taxAmount'] = self.tax_amount
+        if self.train_no is not None:
+            result['trainNo'] = self.train_no
+        if self.travel_date is not None:
+            result['travelDate'] = self.travel_date
         result['usedVehicleSaleDetailVOList'] = []
         if self.used_vehicle_sale_detail_volist is not None:
             for k in self.used_vehicle_sale_detail_volist:
                 result['usedVehicleSaleDetailVOList'].append(k.to_map() if k else None)
         result['vehicleSaleDetailVOList'] = []
         if self.vehicle_sale_detail_volist is not None:
             for k in self.vehicle_sale_detail_volist:
@@ -14142,53 +14478,88 @@
             result['voucherStatus'] = self.voucher_status
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('accountPeriod') is not None:
             self.account_period = m.get('accountPeriod')
+        if m.get('agentCode') is not None:
+            self.agent_code = m.get('agentCode')
         if m.get('amount') is not None:
             self.amount = m.get('amount')
         if m.get('amountWithTax') is not None:
             self.amount_with_tax = m.get('amountWithTax')
+        if m.get('caacDevelopmentFund') is not None:
+            self.caac_development_fund = m.get('caacDevelopmentFund')
         if m.get('checkCode') is not None:
             self.check_code = m.get('checkCode')
         if m.get('checkTime') is not None:
             self.check_time = m.get('checkTime')
+        if m.get('city') is not None:
+            self.city = m.get('city')
+        if m.get('destination') is not None:
+            self.destination = m.get('destination')
+        if m.get('distance') is not None:
+            self.distance = m.get('distance')
         if m.get('drawerName') is not None:
             self.drawer_name = m.get('drawerName')
         if m.get('drewDate') is not None:
             self.drew_date = m.get('drewDate')
         if m.get('electronicUrl') is not None:
             self.electronic_url = m.get('electronicUrl')
+        if m.get('entrance') is not None:
+            self.entrance = m.get('entrance')
+        if m.get('exit') is not None:
+            self.exit = m.get('exit')
         if m.get('financeType') is not None:
             self.finance_type = m.get('financeType')
+        self.flight_itinerary_details = []
+        if m.get('flightItineraryDetails') is not None:
+            for k in m.get('flightItineraryDetails'):
+                temp_model = UpdateInvoiceAndReceiptRelatedRequestGeneralInvoiceVOFlightItineraryDetails()
+                self.flight_itinerary_details.append(temp_model.from_map(k))
+        if m.get('fuelSurcharge') is not None:
+            self.fuel_surcharge = m.get('fuelSurcharge')
         if m.get('fundType') is not None:
             self.fund_type = m.get('fundType')
         self.general_invoice_detail_volist = []
         if m.get('generalInvoiceDetailVOList') is not None:
             for k in m.get('generalInvoiceDetailVOList'):
                 temp_model = UpdateInvoiceAndReceiptRelatedRequestGeneralInvoiceVOGeneralInvoiceDetailVOList()
                 self.general_invoice_detail_volist.append(temp_model.from_map(k))
+        if m.get('getOffTime') is not None:
+            self.get_off_time = m.get('getOffTime')
+        if m.get('getOnTime') is not None:
+            self.get_on_time = m.get('getOnTime')
         if m.get('imageUrl') is not None:
             self.image_url = m.get('imageUrl')
         if m.get('invoiceCode') is not None:
             self.invoice_code = m.get('invoiceCode')
         if m.get('invoiceNo') is not None:
             self.invoice_no = m.get('invoiceNo')
         if m.get('invoiceStatus') is not None:
             self.invoice_status = m.get('invoiceStatus')
         if m.get('invoiceType') is not None:
             self.invoice_type = m.get('invoiceType')
+        if m.get('issueBy') is not None:
+            self.issue_by = m.get('issueBy')
         if m.get('machineCode') is not None:
             self.machine_code = m.get('machineCode')
         if m.get('oilFlag') is not None:
             self.oil_flag = m.get('oilFlag')
+        if m.get('origin') is not None:
+            self.origin = m.get('origin')
+        if m.get('passenger') is not None:
+            self.passenger = m.get('passenger')
+        if m.get('passengerUserId') is not None:
+            self.passenger_user_id = m.get('passengerUserId')
         if m.get('payee') is not None:
             self.payee = m.get('payee')
+        if m.get('printSerialNumber') is not None:
+            self.print_serial_number = m.get('printSerialNumber')
         if m.get('processInstCode') is not None:
             self.process_inst_code = m.get('processInstCode')
         if m.get('processInstType') is not None:
             self.process_inst_type = m.get('processInstType')
         if m.get('purchaserAddress') is not None:
             self.purchaser_address = m.get('purchaserAddress')
         if m.get('purchaserBankAccount') is not None:
@@ -14199,14 +14570,16 @@
             self.purchaser_name = m.get('purchaserName')
         if m.get('purchaserTaxNo') is not None:
             self.purchaser_tax_no = m.get('purchaserTaxNo')
         if m.get('purchaserTel') is not None:
             self.purchaser_tel = m.get('purchaserTel')
         if m.get('remark') is not None:
             self.remark = m.get('remark')
+        if m.get('seatClass') is not None:
+            self.seat_class = m.get('seatClass')
         self.second_hand_car_invoice_detail_list = []
         if m.get('secondHandCarInvoiceDetailList') is not None:
             for k in m.get('secondHandCarInvoiceDetailList'):
                 temp_model = UpdateInvoiceAndReceiptRelatedRequestGeneralInvoiceVOSecondHandCarInvoiceDetailList()
                 self.second_hand_car_invoice_detail_list.append(temp_model.from_map(k))
         if m.get('sellerAddress') is not None:
             self.seller_address = m.get('sellerAddress')
@@ -14216,18 +14589,28 @@
             self.seller_bank_name_account = m.get('sellerBankNameAccount')
         if m.get('sellerName') is not None:
             self.seller_name = m.get('sellerName')
         if m.get('sellerTaxNo') is not None:
             self.seller_tax_no = m.get('sellerTaxNo')
         if m.get('sellerTel') is not None:
             self.seller_tel = m.get('sellerTel')
+        if m.get('serialNo') is not None:
+            self.serial_no = m.get('serialNo')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
         if m.get('supplySign') is not None:
             self.supply_sign = m.get('supplySign')
+        if m.get('surcharge') is not None:
+            self.surcharge = m.get('surcharge')
         if m.get('taxAmount') is not None:
             self.tax_amount = m.get('taxAmount')
+        if m.get('trainNo') is not None:
+            self.train_no = m.get('trainNo')
+        if m.get('travelDate') is not None:
+            self.travel_date = m.get('travelDate')
         self.used_vehicle_sale_detail_volist = []
         if m.get('usedVehicleSaleDetailVOList') is not None:
             for k in m.get('usedVehicleSaleDetailVOList'):
                 temp_model = UpdateInvoiceAndReceiptRelatedRequestGeneralInvoiceVOUsedVehicleSaleDetailVOList()
                 self.used_vehicle_sale_detail_volist.append(temp_model.from_map(k))
         self.vehicle_sale_detail_volist = []
         if m.get('vehicleSaleDetailVOList') is not None:
```

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ding_phone_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ding_phone_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ding_phone_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ding_phone_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_activities_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_activities_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_activities_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_activities_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/report_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/report_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/report_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/report_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.25
+Version: 2.0.26
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.25/setup.py` & `alibabacloud_dingtalk-2.0.26/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 19/07/2023
+Created on 21/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

