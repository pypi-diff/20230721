# Comparing `tmp/huhk-1.6.6.tar.gz` & `tmp/huhk-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhk-1.6.6.tar", last modified: Fri Jul 14 10:02:02 2023, max compression
+gzip compressed data, was "huhk-1.6.8.tar", last modified: Fri Jul 21 09:41:55 2023, max compression
```

## Comparing `huhk-1.6.6.tar` & `huhk-1.6.8.tar`

### file list

```diff
@@ -1,89 +1,138 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.327263 huhk-1.6.6/
--rw-rw-rw-   0        0        0      223 2023-07-14 10:02:02.326264 huhk-1.6.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.207981 huhk-1.6.6/huhk/
--rw-rw-rw-   0        0        0     1006 2023-07-14 07:11:08.000000 huhk-1.6.6/huhk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.228927 huhk-1.6.6/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0     4863 2023-07-14 08:57:28.000000 huhk-1.6.6/huhk/case_project/base_project.py
--rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0      790 2023-07-13 02:39:46.000000 huhk-1.6.6/huhk/case_project/main.py
--rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-14 10:02:01.000000 huhk-1.6.6/huhk/case_project/version.py
--rw-rw-rw-   0        0        0    29648 2023-07-14 08:31:42.000000 huhk-1.6.6/huhk/init_project.py
--rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.230922 huhk-1.6.6/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.254455 huhk-1.6.6/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.6/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.6.6/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.6.6/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.6.6/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.6.6/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.6.6/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.6.6/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.6.6/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.6.6/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.6.6/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.6.6/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    25687 2023-07-13 08:03:20.000000 huhk-1.6.6/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9212 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2473 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.217957 huhk-1.6.6/huhk.egg-info/
--rw-rw-rw-   0        0        0      223 2023-07-14 10:02:02.000000 huhk-1.6.6/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1987 2023-07-14 10:02:02.000000 huhk-1.6.6/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 10:02:02.000000 huhk-1.6.6/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-14 10:02:02.000000 huhk-1.6.6/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-07-14 10:02:02.000000 huhk-1.6.6/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-14 10:02:02.000000 huhk-1.6.6/huhk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.256449 huhk-1.6.6/service/
--rw-rw-rw-   0        0        0        0 2023-07-14 06:51:02.000000 huhk-1.6.6/service/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.268418 huhk-1.6.6/service/app_t/
--rw-rw-rw-   0        0        0      403 2023-07-14 07:07:28.000000 huhk-1.6.6/service/app_t/__init__.py
--rw-rw-rw-   0        0        0     7752 2023-07-14 01:51:05.000000 huhk-1.6.6/service/app_t/app_t_api.py
--rw-rw-rw-   0        0        0     7301 2023-07-14 01:51:05.000000 huhk-1.6.6/service/app_t/app_t_api_fun.py
--rw-rw-rw-   0        0        0     3353 2023-07-14 01:51:05.000000 huhk-1.6.6/service/app_t/app_t_assert.py
--rw-rw-rw-   0        0        0      890 2023-07-14 01:51:05.000000 huhk-1.6.6/service/app_t/app_t_fun.py
--rw-rw-rw-   0        0        0     4402 2023-07-14 01:51:05.000000 huhk-1.6.6/service/app_t/app_t_sql.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.278391 huhk-1.6.6/service/demo/
--rw-rw-rw-   0        0        0      407 2023-07-14 08:11:52.000000 huhk-1.6.6/service/demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.280388 huhk-1.6.6/service/demo/api/
--rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.6/service/demo/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.282380 huhk-1.6.6/service/demo/assert/
--rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.6/service/demo/assert/__init__.py
--rw-rw-rw-   0        0        0      871 2023-07-14 08:25:58.000000 huhk-1.6.6/service/demo/demo_api.py
--rw-rw-rw-   0        0        0      828 2023-07-14 08:25:58.000000 huhk-1.6.6/service/demo/demo_api_fun.py
--rw-rw-rw-   0        0        0      459 2023-07-14 08:25:58.000000 huhk-1.6.6/service/demo/demo_assert.py
--rw-rw-rw-   0        0        0      721 2023-07-14 08:25:58.000000 huhk-1.6.6/service/demo/demo_fun.py
--rw-rw-rw-   0        0        0      579 2023-07-14 08:25:58.000000 huhk-1.6.6/service/demo/demo_sql.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.287370 huhk-1.6.6/service/demo/fun/
--rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.6/service/demo/fun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.289363 huhk-1.6.6/service/demo/sql/
--rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.6/service/demo/sql/__init__.py
--rw-rw-rw-   0        0        0       42 2023-07-14 10:02:02.327263 huhk-1.6.6/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.6.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.292353 huhk-1.6.6/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.6/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.321277 huhk-1.6.6/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.6/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.6/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.6/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.6/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.6.6/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.6.6/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.6.6/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.6.6/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.6.6/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.6.6/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.6.6/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.6.6/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.6.6/testcase/apache/test_to_string.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.324269 huhk-1.6.6/testcase/app_t/
--rw-rw-rw-   0        0        0        0 2023-07-14 06:51:02.000000 huhk-1.6.6/testcase/app_t/__init__.py
--rw-rw-rw-   0        0        0     1923 2023-07-14 01:51:05.000000 huhk-1.6.6/testcase/app_t/test_api.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.259128 huhk-1.6.8/
+-rw-rw-rw-   0        0        0      223 2023-07-21 09:41:55.258140 huhk-1.6.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.062654 huhk-1.6.8/huhk/
+-rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.6.8/huhk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.085594 huhk-1.6.8/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0      790 2023-07-13 02:39:46.000000 huhk-1.6.8/huhk/case_project/main.py
+-rw-rw-rw-   0        0        0    15685 2023-07-21 09:14:03.000000 huhk-1.6.8/huhk/case_project/project_base.py
+-rw-rw-rw-   0        0        0     2099 2023-07-21 08:18:22.000000 huhk-1.6.8/huhk/case_project/project_init.py
+-rw-rw-rw-   0        0        0    14378 2023-07-21 09:35:52.000000 huhk-1.6.8/huhk/case_project/project_string.py
+-rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-21 09:41:54.000000 huhk-1.6.8/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0    13077 2023-07-21 08:30:09.000000 huhk-1.6.8/huhk/init_project.py
+-rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.087589 huhk-1.6.8/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.113520 huhk-1.6.8/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.8/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.6.8/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.6.8/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.6.8/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.6.8/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.6.8/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.6.8/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.6.8/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.6.8/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.6.8/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.6.8/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    26063 2023-07-21 01:52:10.000000 huhk-1.6.8/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0     9533 2023-07-21 02:12:55.000000 huhk-1.6.8/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2473 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.071631 huhk-1.6.8/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-07-21 09:41:54.000000 huhk-1.6.8/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3456 2023-07-21 09:41:54.000000 huhk-1.6.8/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 09:41:54.000000 huhk-1.6.8/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-21 09:41:54.000000 huhk-1.6.8/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-07-21 09:41:54.000000 huhk-1.6.8/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-21 09:41:54.000000 huhk-1.6.8/huhk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.115513 huhk-1.6.8/service/
+-rw-rw-rw-   0        0        0        0 2023-07-14 06:51:02.000000 huhk-1.6.8/service/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.125489 huhk-1.6.8/service/app_t/
+-rw-rw-rw-   0        0        0      402 2023-07-18 06:58:10.000000 huhk-1.6.8/service/app_t/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.127483 huhk-1.6.8/service/app_t/api/
+-rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.6.8/service/app_t/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.130475 huhk-1.6.8/service/app_t/api/open/
+-rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.6.8/service/app_t/api/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.139449 huhk-1.6.8/service/app_t/api/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.6.8/service/app_t/api/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0     3672 2023-07-21 08:42:38.000000 huhk-1.6.8/service/app_t/api/open/haohan/api_open_haohan_relation.py
+-rw-rw-rw-   0        0        0     3837 2023-07-21 08:42:38.000000 huhk-1.6.8/service/app_t/api/open/haohan/api_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.149423 huhk-1.6.8/service/app_t/api/points/
+-rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.6.8/service/app_t/api/points/__init__.py
+-rw-rw-rw-   0        0        0    18817 2023-07-21 08:42:38.000000 huhk-1.6.8/service/app_t/api/points/api_points_points.py
+-rw-rw-rw-   0        0        0    12332 2023-07-21 08:42:38.000000 huhk-1.6.8/service/app_t/api/points/api_points_pointsApp.py
+-rw-rw-rw-   0        0        0     6231 2023-07-19 03:10:22.000000 huhk-1.6.8/service/app_t/app_t_api.py
+-rw-rw-rw-   0        0        0     7301 2023-07-18 08:08:29.000000 huhk-1.6.8/service/app_t/app_t_api_fun.py
+-rw-rw-rw-   0        0        0     3353 2023-07-18 08:08:29.000000 huhk-1.6.8/service/app_t/app_t_assert.py
+-rw-rw-rw-   0        0        0      741 2023-07-21 09:24:51.000000 huhk-1.6.8/service/app_t/app_t_fun.py
+-rw-rw-rw-   0        0        0     4400 2023-07-21 06:34:11.000000 huhk-1.6.8/service/app_t/app_t_sql.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.150422 huhk-1.6.8/service/app_t/assert/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.6.8/service/app_t/assert/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.153412 huhk-1.6.8/service/app_t/assert/open/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.6.8/service/app_t/assert/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.162387 huhk-1.6.8/service/app_t/assert/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.6.8/service/app_t/assert/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      597 2023-07-21 02:24:25.000000 huhk-1.6.8/service/app_t/assert/open/haohan/assert_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      542 2023-07-21 02:21:18.000000 huhk-1.6.8/service/app_t/assert/open/haohan/assert_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.169368 huhk-1.6.8/service/app_t/assert/points/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.6.8/service/app_t/assert/points/__init__.py
+-rw-rw-rw-   0        0        0     1561 2023-07-21 02:21:18.000000 huhk-1.6.8/service/app_t/assert/points/assert_points_points.py
+-rw-rw-rw-   0        0        0     1224 2023-07-21 02:21:18.000000 huhk-1.6.8/service/app_t/assert/points/assert_points_pointsApp.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.171362 huhk-1.6.8/service/app_t/fun/
+-rw-rw-rw-   0        0        0        0 2023-07-18 07:32:47.000000 huhk-1.6.8/service/app_t/fun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.175358 huhk-1.6.8/service/app_t/fun/open/
+-rw-rw-rw-   0        0        0        0 2023-07-21 09:26:44.000000 huhk-1.6.8/service/app_t/fun/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.183332 huhk-1.6.8/service/app_t/fun/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-21 09:26:44.000000 huhk-1.6.8/service/app_t/fun/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      819 2023-07-21 09:36:16.000000 huhk-1.6.8/service/app_t/fun/open/haohan/fun_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      934 2023-07-21 09:36:16.000000 huhk-1.6.8/service/app_t/fun/open/haohan/fun_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.187320 huhk-1.6.8/service/app_t/fun/points/
+-rw-rw-rw-   0        0        0        0 2023-07-21 09:27:08.000000 huhk-1.6.8/service/app_t/fun/points/__init__.py
+-rw-rw-rw-   0        0        0      845 2023-07-21 09:36:16.000000 huhk-1.6.8/service/app_t/fun/points/fun_points_points.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.189315 huhk-1.6.8/service/app_t/sql/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:20:20.000000 huhk-1.6.8/service/app_t/sql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.192312 huhk-1.6.8/service/app_t/sql/open/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:20:21.000000 huhk-1.6.8/service/app_t/sql/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.199288 huhk-1.6.8/service/app_t/sql/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:20:21.000000 huhk-1.6.8/service/app_t/sql/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      570 2023-07-21 02:20:21.000000 huhk-1.6.8/service/app_t/sql/open/haohan/sql_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      566 2023-07-21 02:20:21.000000 huhk-1.6.8/service/app_t/sql/open/haohan/sql_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.204276 huhk-1.6.8/service/app_t/sql/points/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:20:21.000000 huhk-1.6.8/service/app_t/sql/points/__init__.py
+-rw-rw-rw-   0        0        0     1993 2023-07-21 02:20:21.000000 huhk-1.6.8/service/app_t/sql/points/sql_points_points.py
+-rw-rw-rw-   0        0        0     1528 2023-07-21 02:20:21.000000 huhk-1.6.8/service/app_t/sql/points/sql_points_pointsApp.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.216244 huhk-1.6.8/service/demo/
+-rw-rw-rw-   0        0        0      407 2023-07-14 08:11:52.000000 huhk-1.6.8/service/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.217242 huhk-1.6.8/service/demo/api/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.8/service/demo/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.219237 huhk-1.6.8/service/demo/assert/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.8/service/demo/assert/__init__.py
+-rw-rw-rw-   0        0        0      871 2023-07-18 06:50:22.000000 huhk-1.6.8/service/demo/demo_api.py
+-rw-rw-rw-   0        0        0      828 2023-07-18 06:50:22.000000 huhk-1.6.8/service/demo/demo_api_fun.py
+-rw-rw-rw-   0        0        0      459 2023-07-18 06:50:22.000000 huhk-1.6.8/service/demo/demo_assert.py
+-rw-rw-rw-   0        0        0      721 2023-07-18 06:50:22.000000 huhk-1.6.8/service/demo/demo_fun.py
+-rw-rw-rw-   0        0        0      579 2023-07-18 06:50:22.000000 huhk-1.6.8/service/demo/demo_sql.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.221232 huhk-1.6.8/service/demo/fun/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.8/service/demo/fun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.223227 huhk-1.6.8/service/demo/sql/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.8/service/demo/sql/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-21 09:41:55.259128 huhk-1.6.8/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.226216 huhk-1.6.8/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.8/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.252148 huhk-1.6.8/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.8/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.8/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.8/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.8/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.6.8/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.6.8/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.6.8/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.6.8/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.6.8/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.6.8/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.6.8/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.6.8/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.6.8/testcase/apache/test_to_string.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.256146 huhk-1.6.8/testcase/app_t/
+-rw-rw-rw-   0        0        0        0 2023-07-14 06:51:02.000000 huhk-1.6.8/testcase/app_t/__init__.py
+-rw-rw-rw-   0        0        0     1923 2023-07-18 08:08:29.000000 huhk-1.6.8/testcase/app_t/test_api.py
```

### Comparing `huhk-1.6.6/huhk/__init__.py` & `huhk-1.6.8/huhk/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,11 +11,8 @@
     projects_path = os.path.join(*projects_path_list[:projects_path_list.index("service")])
 elif "testcase" in projects_path_list:
     projects_path = os.path.join(*projects_path_list[:projects_path_list.index("testcase")])
 if ":" in projects_path:
     projects_path = projects_path.replace(":", ":" + os.path.sep)
 else:
     projects_path = os.path.sep + projects_path
-files_path = os.path.join(projects_path, "files")
-service_path = os.path.join(projects_path, "service")
-service_json_path = os.path.join(projects_path, "service", "service.json")
-testcase_path = os.path.join(projects_path, "testcase")
+
```

### Comparing `huhk-1.6.6/huhk/case_project/json_coder.py` & `huhk-1.6.8/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/huhk/case_project/main.py` & `huhk-1.6.8/huhk/case_project/main.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/huhk/case_project/setup_set.py` & `huhk-1.6.8/huhk/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/huhk/testcase/apache/beam_class.py` & `huhk-1.6.8/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/huhk/testcase/apache/data.py` & `huhk-1.6.8/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/huhk/testcase/apache/par_do.py` & `huhk-1.6.8/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.6.8/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/huhk/testcase/apache/test_fiter.py` & `huhk-1.6.8/huhk/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/huhk/testcase/apache/test_flatmap.py` & `huhk-1.6.8/huhk/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/huhk/testcase/apache/test_map.py` & `huhk-1.6.8/huhk/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/huhk/testcase/apache/test_par_do.py` & `huhk-1.6.8/huhk/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/huhk/testcase/apache/test_regex.py` & `huhk-1.6.8/huhk/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/huhk/testcase/apache/test_time.py` & `huhk-1.6.8/huhk/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/huhk/unit_apache_beam.py` & `huhk-1.6.8/huhk/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/huhk/unit_dict.py` & `huhk-1.6.8/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/huhk/unit_encryption.py` & `huhk-1.6.8/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/huhk/unit_fun.py` & `huhk-1.6.8/huhk/unit_fun.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,23 +77,28 @@
             return code
             test = re.match('^.\w.[A-Z]\d{4}$|^.\w.\d[A-Z]\d{3}$|^.\w.\d{2}[A-Z]\d{2}$|^.\w.\d{3}[A-Z]\d$|^.\w.\d{5}$',
                             code)
             if test:
                 return code
 
     @staticmethod
-    def write_file(file_path, value=""):
+    def write_file(file_path, value="", mode="w", encoding='utf-8', **kwargs):
         """写文件"""
-        with open(file_path, 'w', encoding='utf-8') as f:
-            f.write(value)
+        if mode in ("wb", "b"):
+            with open(file_path, "wb", **kwargs) as f:
+                f.write(value)
+        else:
+            with open(file_path, mode, encoding=encoding, **kwargs) as f:
+                f.write(value)
+
 
     @staticmethod
-    def read_file(file_path):
+    def read_file(file_path, mode="r"):
         """读文件"""
-        with open(file_path, 'r', encoding='utf-8') as f:
+        with open(file_path, mode, encoding='utf-8') as f:
             value = f.read()
         return value
 
     @staticmethod
     def log_info(msg):
         logger.info(str(msg))
 
@@ -121,24 +126,29 @@
         return time_array * 1000
 
     def data_str(self):
         return datetime.datetime.now().strftime("%Y-%m-%d")
 
     @staticmethod
     def mkdir_file(path, is_py=True):
-        if isinstance(path, (list, tuple)):
-            for i in path:
-                FunBase.mkdir_file(path=i, is_py=is_py)
-        else:
+        if isinstance(path, str):
+            if is_py and ".py" in path:
+                path = os.path.dirname(path)
             if not os.path.lexists(path):
                 if not os.path.lexists(os.path.dirname(path)):
                     FunBase.mkdir_file(path=os.path.dirname(path), is_py=is_py)
                 os.makedirs(path)
                 if is_py:
                     FunBase.write_file(os.path.join(path, "__init__.py"))
+        else:
+            try:
+                for i in path:
+                    FunBase.mkdir_file(path=i, is_py=is_py)
+            except Exception as e:
+                logger.error(str(e))
 
     # # 根据sql语句执行sql
     # def run_mysql(self, sql_str="", host="", user="", password="", database=""):
     #     sql_str = sql_str or self.sql_str
     #     if self._db.get(host+database):
     #         cursor = self._db.get(host+database)
     #     else:
@@ -594,14 +604,16 @@
         version = ".".join([str(i) for i in version_l])
 
         with open("huhk/case_project/version.py", "w", encoding="utf-8") as f:
             f.write("version='%s'\n" % version)
         return version
 
 
+
+
 if __name__ == '__main__':
     print(FunBase.get_version())
     # f = FunBase().faker()
 
     # print(f.name())  # 随机姓名
     # print(f.ipv4())  # 随机IP4地址
     # print(f.uri())  # 随机URI地址
```

### Comparing `huhk-1.6.6/huhk/unit_logger.py` & `huhk-1.6.8/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/huhk/unit_request.py` & `huhk-1.6.8/huhk/unit_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from requests import ReadTimeout, ConnectTimeout
 from requests.exceptions import MissingSchema
 from urllib.parse import urlencode
 from huhk.unit_dict import Dict
 from huhk.unit_logger import logger
 from openpyxl.reader.excel import load_workbook
-from huhk import admin_host, projects_path, files_path
+from huhk import admin_host, projects_path
 
 
 class UnitRequest:
     def __init__(self, ZEST_ENV=None, APP_KEY=None, TIMEOUT=30000):
         self.ZEST_ENV = ZEST_ENV
         self.APP_KEY = APP_KEY
         self.TIMEOUT = TIMEOUT
@@ -33,25 +33,25 @@
             url = url.split('{')[0]
             return url
         else:
             assert False, "字段：" + tmp[0][1:-1] + "，为必填字段"
     
     @staticmethod
     def unit_http_requester(method, url, params=None, data=None, headers=None, host=None, timeout=10000,
-                            init_headers={},
+                            init_headers=None,
                             _route="", _files=None, **kwargs):
         if headers.get("headers"):
-            _headers = init_headers
+            _headers = init_headers or {}
             tmp = headers.pop("headers")
             _headers.update(headers)
             if isinstance(tmp, dict):
                 _headers.update(tmp)
         else:
-            headers.pop("headers")
-            _headers = headers
+            _headers = init_headers or {}
+            _headers.update(headers)
 
         if url[0] == '/' and host:
             if _route and _route[0] != '/':
                 _route = '/' + _route
             url = host + _route + url
         if method.upper() == "GET":
             params = params or data
@@ -59,71 +59,67 @@
         logger.info("接口请求参数headers: %s" % str(_headers))
         logger.info("接口请求参数params: %s" % str(params)) if params else logger.info(
             "接口请求参数data: %s" % str(data))
         if "//" not in url:
             assert False, "url没有域名"
         time_s = time.time()
         try:
-            if "application/x-www-form-urlencoded" in str(_headers):
+            if method.upper() == "GET":
+                res = requests.request(method, url, params=params, json=data, headers=_headers,
+                                       timeout=timeout / 1000,
+                                       verify=False, cookies=kwargs.get('cookies', None))
+            elif "application/x-www-form-urlencoded" in str(_headers):
                 data = urlencode(data)
                 res = requests.request(method, url, data=data, headers=_headers, timeout=timeout / 1000,
                                        verify=False)
             elif "multipart/form-data" in str(_headers) and "file" in data.keys():
                 file = str(data.pop("file"))
                 if not os.path.isfile(file):
                     try:
                         out = requests.get(admin_host + '/files/file/', params={"value": file})
                         if "filename=" in str(out.raw.headers):
                             file_name = urllib.parse.unquote(re.findall(r'filename=(.+?)\'', str(out.raw.headers))[0])
-                            file = os.path.join(files_path, file_name)
+                            file = os.path.join(projects_path, "files", file_name)
                             with open(file, 'wb') as f:
                                 f.write(out.content)
                     except:
                         pass
                     if os.path.isfile(file):
                         pass
-                    elif os.path.isfile(os.path.join(files_path, file)):
-                        file = os.path.join(files_path, file)
+                    elif os.path.isfile(os.path.join(projects_path, "files", file)):
+                        file = os.path.join(projects_path, "files", file)
                     elif os.path.isfile(os.path.join(projects_path, file)):
                         file = os.path.join(projects_path, file)
                     else:
                         assert False, "对应的文件不存在"
                 data.update({'md5': hashlib.md5('%d_%d'.encode() % (0, int(time.time()))).hexdigest(),
                              'filesize': len(open(file, 'rb').read()), })
                 _files = {"file": (os.path.basename(file), open(file, 'rb'))} if file else {}
                 try:
                     del _headers['Content-Type']
                 except:
                     pass
-                if kwargs.get('cookies'):
-                    res = requests.request(method, url, params=params, data=data, files=_files,
-                                           headers=_headers, timeout=timeout / 1000, verify=False,
-                                           cookies=kwargs.get('cookies'))
-                else:
-                    res = requests.request(method, url, params=params, data=data, files=_files,
-                                           headers=_headers, timeout=timeout / 1000, verify=False)
+                res = requests.request(method, url, params=params, data=data, files=_files,
+                                       headers=_headers, timeout=timeout / 1000, verify=False,
+                                       cookies=kwargs.get('cookies'))
+
             else:
-                if kwargs.get('cookies'):
-                    res = requests.request(method, url, params=params, json=data, headers=_headers,
-                                           timeout=timeout / 1000,
-                                           verify=False, cookies=kwargs.get('cookies'))
-                else:
-                    res = requests.request(method, url, params=params, json=data, headers=_headers,
-                                           timeout=timeout / 1000,
-                                           verify=False)
+                res = requests.request(method, url, params=params, json=data, headers=_headers,
+                                       timeout=timeout / 1000,
+                                       verify=False, cookies=kwargs.get('cookies', None))
+
 
             logger.info("接口响应时间: %.3f毫秒" % (time.time() - time_s))
             try:
-                res.rsp = Dict(json.loads(res.text)) if res.text else Dict(
-                    {"code": -1, "msg": "该接口返回的数据为空字符串"})
+                res.rsp = Dict(json.loads(res.text)) if res.text else res.text
             except:
                 if "filename=" in str(res.raw.headers):
                     file_name = urllib.parse.unquote(re.findall(r'filename=(.+?)\'', str(res.raw.headers))[0])
                     if "xlsx" in file_name:
-                        file_path = os.path.join(files_path, file_name)
+                        file_path = os.path.join(projects_path, "files", file_name)
                         with open(file_path, 'wb') as f:
                             f.write(res.content)
                         wb = load_workbook(file_path)
                         ws = wb.active
                         rows = [[cell.value for cell in row] for row in ws]
                         try:
                             data = [{c1: c2 for c1, c2 in zip(rows[0], row)} for row in rows[1:]]
@@ -184,11 +180,27 @@
         return headers
     
     def http_requester(self, *args, **kwargs):
         _host = kwargs.get("_host", "HOST")
         host = self.variable.get(_host) if "//" not in _host else _host
         return self.unit_http_requester(*args, host=host, timeout=self.TIMEOUT, init_headers=self.init_headers(**kwargs), **kwargs)
 
+    @staticmethod
+    def is_assert_true(res):
+        code = [0, 200, "0000", "00000", "0", "200", "000"]
+        code_name = ["success", "ok", True, "OK", "Ok"]
+        assert_dict = {"code": code, "result": code_name, "msg": code_name, "success": code_name,
+                       "resultCode": code, "returnCode": code}
+        if res.status_code != 200:
+            return False
+        elif isinstance(res.rsp, dict):
+            for k, v in assert_dict.items():
+                if res.rsp.get(k) in v:
+                    return True
+            return False
+        else:
+            return True
+
 
 get_url = UnitRequest.get_url
 unit_http_requester = UnitRequest.unit_http_requester
 get_variable = UnitRequest().get_variable
```

### Comparing `huhk-1.6.6/huhk/unit_tasks.py` & `huhk-1.6.8/huhk/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/huhk/常用命令.py` & `huhk-1.6.8/huhk/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/service/app_t/app_t_api.py` & `huhk-1.6.8/service/app_t/app_t_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,13 @@
 import allure
 
 from service.app_t import http_requester
 from huhk.unit_request import get_url
 
 
-@allure.step(title="调接口：/open/haohan/relation/update")
-def open_haohan_relation_update(userId=None, headers=None, **kwargs):
-    """
-    浩瀚模块-关联关系-Y
-    up_time=1675665418
-
-    params: userId :  : 用户ID（数据类型：String）
-    params: headers : 请求头
-    ====================返回======================
-    """
-    _method = "GET"
-    _url = "/open/haohan/relation/update"
-
-    _headers = {
-    }
-    _headers.update({"headers": headers})
-
-    _data = {
-        "userId": userId,  # 用户ID（数据类型：String）
-    }
-
-    _params = {
-    }
-
-    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
-
-
-@allure.step(title="调接口：/open/haohan/rights/update")
-def open_haohan_rights_update(params=None, headers=None, **kwargs):
-    """
-    浩瀚模块 - 更改充电桩权益状态-Y
-    up_time=1675665629
-
-    params: params : object : 
-              data : string : 加密数据
-    params: headers : 请求头
-    ====================返回======================
-    """
-    _method = "POST"
-    _url = "/open/haohan/rights/update"
-
-    _headers = {
-        "Content-Type": "application/json",
-    }
-    _headers.update({"headers": headers})
-
-    _data = {
-        "params": params,
-    }
-
-    _params = {
-    }
-
-    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
-
-
-@allure.step(title="调接口：/points/pointsApp/signIn")
 def points_pointsApp_signIn(userId=None, headers=None, **kwargs):
     """
     APP-用户签到
     up_time=1676254515
 
     params: userId :  : 用户ID
     params: headers : 请求头
```

### Comparing `huhk-1.6.6/service/app_t/app_t_api_fun.py` & `huhk-1.6.8/service/app_t/app_t_api_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/service/app_t/app_t_assert.py` & `huhk-1.6.8/service/app_t/app_t_assert.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/service/app_t/app_t_fun.py` & `huhk-1.6.8/service/app_t/app_t_fun.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 import requests
 
+from huhk.unit_dict import Dict
 from huhk.unit_fun import FunBase
 from huhk import admin_host
 
 
-class App_TFun(FunBase):
+class AppTFun(FunBase):
     def __init__(self):
         super().__init__()
         self.res = None
-        self._v_endTime = None
-        self._v_beforeTime = None
-        self._list_endTime = []
-        self._list_beforeTime = []
-        self._v_params = None
-        self._v_userId = None
-
-    def run_mysql(self, sql_str):
-        # id是后台http://47.96.124.102/admin 项目数据库链接的id
-        out = requests.post(admin_host + "/sql/running_sql/", json={"id": 1, "sql_str": sql_str}).json()
+        self.output_value = Dict()
+        self.input_value = Dict()
+
+    def run_mysql(self, sql_str, db_id=1):
+        # 根据后台数据库配置id查询
+        out = requests.post(admin_host + "/sql/running_sql/", json={"id": db_id, "sql_str": sql_str}).json()
         if out.get("code") == "0000":
             return out.get("data")
         else:
             assert False, sql_str + str(out.get("msg"))
 
 
 if __name__ == '__main__':
-    f = App_TFun()
-    out = f.run_mysql("SELECT * FROM `t_accept_log`  LIMIT 1;")
+    f = AppTFun()
+    out = f.faker().name()
     print(out)
```

### Comparing `huhk-1.6.6/service/app_t/app_t_sql.py` & `huhk-1.6.8/service/app_t/app_t_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from service.app_t.app_t_fun import App_TFun
+from service.app_t.app_t_fun import AppTFun
 
 
-class App_TSql(App_TFun):
+class App_TSql(AppTFun):
 
     def sql_open_haohan_relation_update(self, **kwargs):
         # name = self.kwargs_pop(kwargs, 'name')  # 单独处理字段
         # self.kwargs_replace(kwargs, likes=[], ins=[], before_end=[])  # 模糊查询字段，数组包含查询字段，区间字段处理
         # kwargs["order_by"] = None  # 排序
         sql_str = self.get_sql_str("table", **kwargs)  # 生成sql语句
         # out = self.run_mysql(sql_str)  # 执行sql语句
```

### Comparing `huhk-1.6.6/service/demo/demo_api.py` & `huhk-1.6.8/service/demo/demo_api.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/service/demo/demo_api_fun.py` & `huhk-1.6.8/service/demo/demo_api_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/service/demo/demo_fun.py` & `huhk-1.6.8/service/demo/demo_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/service/demo/demo_sql.py` & `huhk-1.6.8/service/demo/demo_sql.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/testcase/apache/beam_class.py` & `huhk-1.6.8/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/testcase/apache/data.py` & `huhk-1.6.8/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/testcase/apache/par_do.py` & `huhk-1.6.8/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/testcase/apache/test_cogroupbykey.py` & `huhk-1.6.8/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/testcase/apache/test_fiter.py` & `huhk-1.6.8/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/testcase/apache/test_flatmap.py` & `huhk-1.6.8/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/testcase/apache/test_map.py` & `huhk-1.6.8/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/testcase/apache/test_par_do.py` & `huhk-1.6.8/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/testcase/apache/test_regex.py` & `huhk-1.6.8/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/testcase/apache/test_time.py` & `huhk-1.6.8/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.6/testcase/app_t/test_api.py` & `huhk-1.6.8/testcase/app_t/test_api.py`

 * *Files identical despite different names*

