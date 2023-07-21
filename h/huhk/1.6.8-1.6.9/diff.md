# Comparing `tmp/huhk-1.6.8.tar.gz` & `tmp/huhk-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhk-1.6.8.tar", last modified: Fri Jul 21 09:41:55 2023, max compression
+gzip compressed data, was "huhk-1.6.9.tar", last modified: Fri Jul 21 09:54:10 2023, max compression
```

## Comparing `huhk-1.6.8.tar` & `huhk-1.6.9.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.259128 huhk-1.6.8/
--rw-rw-rw-   0        0        0      223 2023-07-21 09:41:55.258140 huhk-1.6.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.062654 huhk-1.6.8/huhk/
--rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.6.8/huhk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.085594 huhk-1.6.8/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0      790 2023-07-13 02:39:46.000000 huhk-1.6.8/huhk/case_project/main.py
--rw-rw-rw-   0        0        0    15685 2023-07-21 09:14:03.000000 huhk-1.6.8/huhk/case_project/project_base.py
--rw-rw-rw-   0        0        0     2099 2023-07-21 08:18:22.000000 huhk-1.6.8/huhk/case_project/project_init.py
--rw-rw-rw-   0        0        0    14378 2023-07-21 09:35:52.000000 huhk-1.6.8/huhk/case_project/project_string.py
--rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-21 09:41:54.000000 huhk-1.6.8/huhk/case_project/version.py
--rw-rw-rw-   0        0        0    13077 2023-07-21 08:30:09.000000 huhk-1.6.8/huhk/init_project.py
--rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.087589 huhk-1.6.8/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.113520 huhk-1.6.8/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.8/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.6.8/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.6.8/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.6.8/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.6.8/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.6.8/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.6.8/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.6.8/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.6.8/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.6.8/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.6.8/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    26063 2023-07-21 01:52:10.000000 huhk-1.6.8/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9533 2023-07-21 02:12:55.000000 huhk-1.6.8/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2473 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.6.8/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.071631 huhk-1.6.8/huhk.egg-info/
--rw-rw-rw-   0        0        0      223 2023-07-21 09:41:54.000000 huhk-1.6.8/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3456 2023-07-21 09:41:54.000000 huhk-1.6.8/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 09:41:54.000000 huhk-1.6.8/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-21 09:41:54.000000 huhk-1.6.8/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-07-21 09:41:54.000000 huhk-1.6.8/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-21 09:41:54.000000 huhk-1.6.8/huhk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.115513 huhk-1.6.8/service/
--rw-rw-rw-   0        0        0        0 2023-07-14 06:51:02.000000 huhk-1.6.8/service/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.125489 huhk-1.6.8/service/app_t/
--rw-rw-rw-   0        0        0      402 2023-07-18 06:58:10.000000 huhk-1.6.8/service/app_t/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.127483 huhk-1.6.8/service/app_t/api/
--rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.6.8/service/app_t/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.130475 huhk-1.6.8/service/app_t/api/open/
--rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.6.8/service/app_t/api/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.139449 huhk-1.6.8/service/app_t/api/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.6.8/service/app_t/api/open/haohan/__init__.py
--rw-rw-rw-   0        0        0     3672 2023-07-21 08:42:38.000000 huhk-1.6.8/service/app_t/api/open/haohan/api_open_haohan_relation.py
--rw-rw-rw-   0        0        0     3837 2023-07-21 08:42:38.000000 huhk-1.6.8/service/app_t/api/open/haohan/api_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.149423 huhk-1.6.8/service/app_t/api/points/
--rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.6.8/service/app_t/api/points/__init__.py
--rw-rw-rw-   0        0        0    18817 2023-07-21 08:42:38.000000 huhk-1.6.8/service/app_t/api/points/api_points_points.py
--rw-rw-rw-   0        0        0    12332 2023-07-21 08:42:38.000000 huhk-1.6.8/service/app_t/api/points/api_points_pointsApp.py
--rw-rw-rw-   0        0        0     6231 2023-07-19 03:10:22.000000 huhk-1.6.8/service/app_t/app_t_api.py
--rw-rw-rw-   0        0        0     7301 2023-07-18 08:08:29.000000 huhk-1.6.8/service/app_t/app_t_api_fun.py
--rw-rw-rw-   0        0        0     3353 2023-07-18 08:08:29.000000 huhk-1.6.8/service/app_t/app_t_assert.py
--rw-rw-rw-   0        0        0      741 2023-07-21 09:24:51.000000 huhk-1.6.8/service/app_t/app_t_fun.py
--rw-rw-rw-   0        0        0     4400 2023-07-21 06:34:11.000000 huhk-1.6.8/service/app_t/app_t_sql.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.150422 huhk-1.6.8/service/app_t/assert/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.6.8/service/app_t/assert/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.153412 huhk-1.6.8/service/app_t/assert/open/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.6.8/service/app_t/assert/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.162387 huhk-1.6.8/service/app_t/assert/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.6.8/service/app_t/assert/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      597 2023-07-21 02:24:25.000000 huhk-1.6.8/service/app_t/assert/open/haohan/assert_open_haohan_relation.py
--rw-rw-rw-   0        0        0      542 2023-07-21 02:21:18.000000 huhk-1.6.8/service/app_t/assert/open/haohan/assert_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.169368 huhk-1.6.8/service/app_t/assert/points/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.6.8/service/app_t/assert/points/__init__.py
--rw-rw-rw-   0        0        0     1561 2023-07-21 02:21:18.000000 huhk-1.6.8/service/app_t/assert/points/assert_points_points.py
--rw-rw-rw-   0        0        0     1224 2023-07-21 02:21:18.000000 huhk-1.6.8/service/app_t/assert/points/assert_points_pointsApp.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.171362 huhk-1.6.8/service/app_t/fun/
--rw-rw-rw-   0        0        0        0 2023-07-18 07:32:47.000000 huhk-1.6.8/service/app_t/fun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.175358 huhk-1.6.8/service/app_t/fun/open/
--rw-rw-rw-   0        0        0        0 2023-07-21 09:26:44.000000 huhk-1.6.8/service/app_t/fun/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.183332 huhk-1.6.8/service/app_t/fun/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-21 09:26:44.000000 huhk-1.6.8/service/app_t/fun/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      819 2023-07-21 09:36:16.000000 huhk-1.6.8/service/app_t/fun/open/haohan/fun_open_haohan_relation.py
--rw-rw-rw-   0        0        0      934 2023-07-21 09:36:16.000000 huhk-1.6.8/service/app_t/fun/open/haohan/fun_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.187320 huhk-1.6.8/service/app_t/fun/points/
--rw-rw-rw-   0        0        0        0 2023-07-21 09:27:08.000000 huhk-1.6.8/service/app_t/fun/points/__init__.py
--rw-rw-rw-   0        0        0      845 2023-07-21 09:36:16.000000 huhk-1.6.8/service/app_t/fun/points/fun_points_points.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.189315 huhk-1.6.8/service/app_t/sql/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:20:20.000000 huhk-1.6.8/service/app_t/sql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.192312 huhk-1.6.8/service/app_t/sql/open/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:20:21.000000 huhk-1.6.8/service/app_t/sql/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.199288 huhk-1.6.8/service/app_t/sql/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:20:21.000000 huhk-1.6.8/service/app_t/sql/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      570 2023-07-21 02:20:21.000000 huhk-1.6.8/service/app_t/sql/open/haohan/sql_open_haohan_relation.py
--rw-rw-rw-   0        0        0      566 2023-07-21 02:20:21.000000 huhk-1.6.8/service/app_t/sql/open/haohan/sql_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.204276 huhk-1.6.8/service/app_t/sql/points/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:20:21.000000 huhk-1.6.8/service/app_t/sql/points/__init__.py
--rw-rw-rw-   0        0        0     1993 2023-07-21 02:20:21.000000 huhk-1.6.8/service/app_t/sql/points/sql_points_points.py
--rw-rw-rw-   0        0        0     1528 2023-07-21 02:20:21.000000 huhk-1.6.8/service/app_t/sql/points/sql_points_pointsApp.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.216244 huhk-1.6.8/service/demo/
--rw-rw-rw-   0        0        0      407 2023-07-14 08:11:52.000000 huhk-1.6.8/service/demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.217242 huhk-1.6.8/service/demo/api/
--rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.8/service/demo/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.219237 huhk-1.6.8/service/demo/assert/
--rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.8/service/demo/assert/__init__.py
--rw-rw-rw-   0        0        0      871 2023-07-18 06:50:22.000000 huhk-1.6.8/service/demo/demo_api.py
--rw-rw-rw-   0        0        0      828 2023-07-18 06:50:22.000000 huhk-1.6.8/service/demo/demo_api_fun.py
--rw-rw-rw-   0        0        0      459 2023-07-18 06:50:22.000000 huhk-1.6.8/service/demo/demo_assert.py
--rw-rw-rw-   0        0        0      721 2023-07-18 06:50:22.000000 huhk-1.6.8/service/demo/demo_fun.py
--rw-rw-rw-   0        0        0      579 2023-07-18 06:50:22.000000 huhk-1.6.8/service/demo/demo_sql.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.221232 huhk-1.6.8/service/demo/fun/
--rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.8/service/demo/fun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.223227 huhk-1.6.8/service/demo/sql/
--rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.8/service/demo/sql/__init__.py
--rw-rw-rw-   0        0        0       42 2023-07-21 09:41:55.259128 huhk-1.6.8/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.6.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.226216 huhk-1.6.8/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.8/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.252148 huhk-1.6.8/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.8/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.8/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.8/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.8/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.6.8/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.6.8/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.6.8/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.6.8/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.6.8/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.6.8/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.6.8/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.6.8/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.6.8/testcase/apache/test_to_string.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:41:55.256146 huhk-1.6.8/testcase/app_t/
--rw-rw-rw-   0        0        0        0 2023-07-14 06:51:02.000000 huhk-1.6.8/testcase/app_t/__init__.py
--rw-rw-rw-   0        0        0     1923 2023-07-18 08:08:29.000000 huhk-1.6.8/testcase/app_t/test_api.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.206579 huhk-1.6.9/
+-rw-rw-rw-   0        0        0      223 2023-07-21 09:54:10.205616 huhk-1.6.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:09.961799 huhk-1.6.9/huhk/
+-rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.6.9/huhk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:09.988724 huhk-1.6.9/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0      790 2023-07-13 02:39:46.000000 huhk-1.6.9/huhk/case_project/main.py
+-rw-rw-rw-   0        0        0    15661 2023-07-21 09:53:53.000000 huhk-1.6.9/huhk/case_project/project_base.py
+-rw-rw-rw-   0        0        0     2099 2023-07-21 08:18:22.000000 huhk-1.6.9/huhk/case_project/project_init.py
+-rw-rw-rw-   0        0        0    14745 2023-07-21 09:53:53.000000 huhk-1.6.9/huhk/case_project/project_string.py
+-rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-21 09:54:09.000000 huhk-1.6.9/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0    13077 2023-07-21 08:30:09.000000 huhk-1.6.9/huhk/init_project.py
+-rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:09.990718 huhk-1.6.9/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.033605 huhk-1.6.9/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.9/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.6.9/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.6.9/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.6.9/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.6.9/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.6.9/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.6.9/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.6.9/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.6.9/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.6.9/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.6.9/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    26063 2023-07-21 01:52:10.000000 huhk-1.6.9/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0     9533 2023-07-21 02:12:55.000000 huhk-1.6.9/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2473 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:09.972768 huhk-1.6.9/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-07-21 09:54:09.000000 huhk-1.6.9/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3456 2023-07-21 09:54:09.000000 huhk-1.6.9/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 09:54:09.000000 huhk-1.6.9/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-21 09:54:09.000000 huhk-1.6.9/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-07-21 09:54:09.000000 huhk-1.6.9/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-21 09:54:09.000000 huhk-1.6.9/huhk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.037597 huhk-1.6.9/service/
+-rw-rw-rw-   0        0        0        0 2023-07-14 06:51:02.000000 huhk-1.6.9/service/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.052554 huhk-1.6.9/service/app_t/
+-rw-rw-rw-   0        0        0      402 2023-07-18 06:58:10.000000 huhk-1.6.9/service/app_t/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.056546 huhk-1.6.9/service/app_t/api/
+-rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.6.9/service/app_t/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.059539 huhk-1.6.9/service/app_t/api/open/
+-rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.6.9/service/app_t/api/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.069509 huhk-1.6.9/service/app_t/api/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.6.9/service/app_t/api/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0     3672 2023-07-21 08:42:38.000000 huhk-1.6.9/service/app_t/api/open/haohan/api_open_haohan_relation.py
+-rw-rw-rw-   0        0        0     3837 2023-07-21 08:42:38.000000 huhk-1.6.9/service/app_t/api/open/haohan/api_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.081479 huhk-1.6.9/service/app_t/api/points/
+-rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.6.9/service/app_t/api/points/__init__.py
+-rw-rw-rw-   0        0        0    18817 2023-07-21 08:42:38.000000 huhk-1.6.9/service/app_t/api/points/api_points_points.py
+-rw-rw-rw-   0        0        0    12332 2023-07-21 08:42:38.000000 huhk-1.6.9/service/app_t/api/points/api_points_pointsApp.py
+-rw-rw-rw-   0        0        0     6231 2023-07-19 03:10:22.000000 huhk-1.6.9/service/app_t/app_t_api.py
+-rw-rw-rw-   0        0        0     7301 2023-07-18 08:08:29.000000 huhk-1.6.9/service/app_t/app_t_api_fun.py
+-rw-rw-rw-   0        0        0     3353 2023-07-18 08:08:29.000000 huhk-1.6.9/service/app_t/app_t_assert.py
+-rw-rw-rw-   0        0        0      754 2023-07-21 09:47:48.000000 huhk-1.6.9/service/app_t/app_t_fun.py
+-rw-rw-rw-   0        0        0     4400 2023-07-21 06:34:11.000000 huhk-1.6.9/service/app_t/app_t_sql.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.083470 huhk-1.6.9/service/app_t/assert/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.6.9/service/app_t/assert/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.086463 huhk-1.6.9/service/app_t/assert/open/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.6.9/service/app_t/assert/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.094444 huhk-1.6.9/service/app_t/assert/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.6.9/service/app_t/assert/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      597 2023-07-21 02:24:25.000000 huhk-1.6.9/service/app_t/assert/open/haohan/assert_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      542 2023-07-21 02:21:18.000000 huhk-1.6.9/service/app_t/assert/open/haohan/assert_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.100428 huhk-1.6.9/service/app_t/assert/points/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.6.9/service/app_t/assert/points/__init__.py
+-rw-rw-rw-   0        0        0     1561 2023-07-21 02:21:18.000000 huhk-1.6.9/service/app_t/assert/points/assert_points_points.py
+-rw-rw-rw-   0        0        0     1224 2023-07-21 02:21:18.000000 huhk-1.6.9/service/app_t/assert/points/assert_points_pointsApp.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.101426 huhk-1.6.9/service/app_t/fun/
+-rw-rw-rw-   0        0        0        0 2023-07-18 07:32:47.000000 huhk-1.6.9/service/app_t/fun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.104416 huhk-1.6.9/service/app_t/fun/open/
+-rw-rw-rw-   0        0        0        0 2023-07-21 09:26:44.000000 huhk-1.6.9/service/app_t/fun/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.111396 huhk-1.6.9/service/app_t/fun/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-21 09:26:44.000000 huhk-1.6.9/service/app_t/fun/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      819 2023-07-21 09:36:16.000000 huhk-1.6.9/service/app_t/fun/open/haohan/fun_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      934 2023-07-21 09:36:16.000000 huhk-1.6.9/service/app_t/fun/open/haohan/fun_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.116382 huhk-1.6.9/service/app_t/fun/points/
+-rw-rw-rw-   0        0        0        0 2023-07-21 09:27:08.000000 huhk-1.6.9/service/app_t/fun/points/__init__.py
+-rw-rw-rw-   0        0        0      845 2023-07-21 09:36:16.000000 huhk-1.6.9/service/app_t/fun/points/fun_points_points.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.117380 huhk-1.6.9/service/app_t/sql/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:20:20.000000 huhk-1.6.9/service/app_t/sql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.120372 huhk-1.6.9/service/app_t/sql/open/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:20:21.000000 huhk-1.6.9/service/app_t/sql/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.127354 huhk-1.6.9/service/app_t/sql/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:20:21.000000 huhk-1.6.9/service/app_t/sql/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      570 2023-07-21 02:20:21.000000 huhk-1.6.9/service/app_t/sql/open/haohan/sql_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      566 2023-07-21 02:20:21.000000 huhk-1.6.9/service/app_t/sql/open/haohan/sql_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.132849 huhk-1.6.9/service/app_t/sql/points/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:20:21.000000 huhk-1.6.9/service/app_t/sql/points/__init__.py
+-rw-rw-rw-   0        0        0     1993 2023-07-21 02:20:21.000000 huhk-1.6.9/service/app_t/sql/points/sql_points_points.py
+-rw-rw-rw-   0        0        0     1528 2023-07-21 02:20:21.000000 huhk-1.6.9/service/app_t/sql/points/sql_points_pointsApp.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.147808 huhk-1.6.9/service/demo/
+-rw-rw-rw-   0        0        0      407 2023-07-14 08:11:52.000000 huhk-1.6.9/service/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.149803 huhk-1.6.9/service/demo/api/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.9/service/demo/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.151800 huhk-1.6.9/service/demo/assert/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.9/service/demo/assert/__init__.py
+-rw-rw-rw-   0        0        0      871 2023-07-18 06:50:22.000000 huhk-1.6.9/service/demo/demo_api.py
+-rw-rw-rw-   0        0        0      828 2023-07-18 06:50:22.000000 huhk-1.6.9/service/demo/demo_api_fun.py
+-rw-rw-rw-   0        0        0      459 2023-07-18 06:50:22.000000 huhk-1.6.9/service/demo/demo_assert.py
+-rw-rw-rw-   0        0        0      721 2023-07-18 06:50:22.000000 huhk-1.6.9/service/demo/demo_fun.py
+-rw-rw-rw-   0        0        0      579 2023-07-18 06:50:22.000000 huhk-1.6.9/service/demo/demo_sql.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.154752 huhk-1.6.9/service/demo/fun/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.9/service/demo/fun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.156741 huhk-1.6.9/service/demo/sql/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.9/service/demo/sql/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-21 09:54:10.207576 huhk-1.6.9/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.158740 huhk-1.6.9/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.9/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.196607 huhk-1.6.9/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.9/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.9/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.9/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.9/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.6.9/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.6.9/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.6.9/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.6.9/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.6.9/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.6.9/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.6.9/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.6.9/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.6.9/testcase/apache/test_to_string.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.203591 huhk-1.6.9/testcase/app_t/
+-rw-rw-rw-   0        0        0        0 2023-07-14 06:51:02.000000 huhk-1.6.9/testcase/app_t/__init__.py
+-rw-rw-rw-   0        0        0     1923 2023-07-18 08:08:29.000000 huhk-1.6.9/testcase/app_t/test_api.py
```

### Comparing `huhk-1.6.8/huhk/__init__.py` & `huhk-1.6.9/huhk/__init__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/case_project/json_coder.py` & `huhk-1.6.9/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/case_project/main.py` & `huhk-1.6.9/huhk/case_project/main.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/case_project/project_base.py` & `huhk-1.6.9/huhk/case_project/project_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,15 @@
                     FunBase.write_file(fun_path.path, file_str)
             else:
                 tmp_list = file_str.split("if __name__ == '__main__':")
                 tmp_list[0] += self.get_api_fun_fun_str(fun_name)
                 file_str = "if __name__ == '__main__':".join(tmp_list)
                 FunBase.write_file(fun_path.path, file_str)
         else:
-            file_str = self.get_api_fun_header_str(fun_path.class_name, assert_path) + self.get_api_fun_fun_str(fun_name)
+            file_str = self.get_api_fun_header_str(fun_name) + self.get_api_fun_fun_str(fun_name)
             FunBase.mkdir_file(fun_path.path)
             FunBase.write_file(fun_path.path, file_str)
 
 
 if __name__ == "__main__":
     a = ProjectBase(name="app_t")
     a.dir = r"D:\projects\python_test\huhk-common"
```

### Comparing `huhk-1.6.8/huhk/case_project/project_init.py` & `huhk-1.6.9/huhk/case_project/project_init.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/case_project/project_string.py` & `huhk-1.6.9/huhk/case_project/project_string.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     def get_fun_value(self):
         """生成项目基础方法"""
         value = "import requests\n\nfrom huhk.unit_fun import FunBase\n"
         value += "from huhk.unit_dict import Dict\n"
         value += f"from huhk import admin_host\n\n\nclass {self.name2.replace('_', '')}Fun(FunBase):\n"
         value += "    def __init__(self):\n        super().__init__()\n        self.res = None\n"
         value += "        self.output_list = Dict()\n        self.input_value = Dict()\n"
-        value += "    def run_mysql(self, sql_str, db_id=1):\n"
+        value += "    @staticmethod\n    def run_mysql( sql_str, db_id=1):\n"
         value += "        # 根据后台数据库配置id查询\n"
         value += '        out = requests.post(admin_host + "/sql/running_sql/", '
         value += 'json={"id": db_id, "sql_str": sql_str}).json()\n'
         value += '        if out.get("code") == "0000":\n'
         value += '            return out.get("data")\n        else:\n'
         value += '            assert False, sql_str + str(out.get("msg"))\n\n\n'
         value += f"if __name__ == '__main__':\n    f = {self.name2.replace('_', '')}Fun()\n"
@@ -206,17 +206,22 @@
                          '        # out = self.sql_%s(**kwargs)\n' % (fun_name, fun_name)
         assert_fun_str += '        # flag = self.compare_json_list(self.res, out, [%s])\n' % \
                           ', '.join(['"%s"' % i for i in self.this_fun_list.api[fun_name].input
                                      if str(i).lower() not in self.page_and_size])
         assert_fun_str += '        assert True, "数据比较不一致"\n\n'
         return assert_fun_str
 
-    def get_api_fun_header_str(self, class_name, assert_path):
-        class_name = ""
-        return class_name
+    def get_api_fun_header_str(self, fun_name):
+        assert_path = self.get_path(fun_name, fun_type='assert')
+        fun_path = self.get_path(fun_name, fun_type='fun')
+        header_str = "import allure\n\n"
+        header_str += "from service.app_t.app_t_assert import App_TAssert\n"
+        header_str += "from service.app_t import app_t_api\n\n\n"
+        header_str += f"class {fun_path.class_name}({assert_path.class_name}):\n"
+        return header_str
 
     def get_api_fun_fun_str(self, fun_name):
         api = self.this_fun_list.api[fun_name]
         data_list_tmp = []
         for n in api.input:
             if n in self.size_names:
                 data_list_tmp.append(n.strip() + '=10')
@@ -259,22 +264,21 @@
                     if re.findall(f'^{n_l[0][0]}{"|".join(self.before)}{n_l[0][2]}$', str(data_list)) \
                             and re.findall(f'^{n_l[0][0]}{"|".join(self.before)}{n_l[0][2]}$', str(data_list)):
                         n2 = n_l[0][0] or n_l[0][2]
                     else:
                         n2 = n
                 else:
                     n2 = n
-                api_fun_fun_str += "        self.output_value.%s = self.get_res_value_list('%s')\n" % (n, n2)
+                api_fun_fun_str += "        self.output_list.%s = self.get_res_value_list('%s')\n" % (n, n2)
 
         for n in data_list:
             api_fun_fun_str += "        self.input_value.%s = %s\n" % (n, n)
 
         api_fun_fun_str += '\n' if data_list else ''
         api_fun_fun_str += "        if _assert is True:\n"
         api_fun_fun_str += "            self.assert_%s(**_kwargs)\n" % fun_name
         api_fun_fun_str += "        elif _assert is not True:\n" \
                            '            assert self.res.rsp.code == _assert or self.res.status_code == _assert, ' \
                            '"校验code=%s不通过" % _assert\n'
         api_fun_fun_str += "        return self.res\n\n"
-
         return api_fun_fun_str
```

### Comparing `huhk-1.6.8/huhk/case_project/setup_set.py` & `huhk-1.6.9/huhk/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/init_project.py` & `huhk-1.6.9/huhk/init_project.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/testcase/apache/beam_class.py` & `huhk-1.6.9/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/testcase/apache/data.py` & `huhk-1.6.9/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/testcase/apache/par_do.py` & `huhk-1.6.9/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.6.9/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/testcase/apache/test_fiter.py` & `huhk-1.6.9/huhk/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/testcase/apache/test_flatmap.py` & `huhk-1.6.9/huhk/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/testcase/apache/test_map.py` & `huhk-1.6.9/huhk/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/testcase/apache/test_par_do.py` & `huhk-1.6.9/huhk/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/testcase/apache/test_regex.py` & `huhk-1.6.9/huhk/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/testcase/apache/test_time.py` & `huhk-1.6.9/huhk/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/unit_apache_beam.py` & `huhk-1.6.9/huhk/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/unit_dict.py` & `huhk-1.6.9/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/unit_encryption.py` & `huhk-1.6.9/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/unit_fun.py` & `huhk-1.6.9/huhk/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/unit_logger.py` & `huhk-1.6.9/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/unit_request.py` & `huhk-1.6.9/huhk/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/unit_tasks.py` & `huhk-1.6.9/huhk/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk/常用命令.py` & `huhk-1.6.9/huhk/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/huhk.egg-info/SOURCES.txt` & `huhk-1.6.9/huhk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/app_t/api/open/haohan/api_open_haohan_relation.py` & `huhk-1.6.9/service/app_t/api/open/haohan/api_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/app_t/api/open/haohan/api_open_haohan_rights.py` & `huhk-1.6.9/service/app_t/api/open/haohan/api_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/app_t/api/points/api_points_points.py` & `huhk-1.6.9/service/app_t/api/points/api_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/app_t/api/points/api_points_pointsApp.py` & `huhk-1.6.9/service/app_t/api/points/api_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/app_t/app_t_api.py` & `huhk-1.6.9/service/app_t/app_t_api.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/app_t/app_t_api_fun.py` & `huhk-1.6.9/service/app_t/app_t_api_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/app_t/app_t_assert.py` & `huhk-1.6.9/service/app_t/app_t_assert.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/app_t/app_t_fun.py` & `huhk-1.6.9/service/app_t/app_t_fun.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 class AppTFun(FunBase):
     def __init__(self):
         super().__init__()
         self.res = None
         self.output_value = Dict()
         self.input_value = Dict()
 
-    def run_mysql(self, sql_str, db_id=1):
+    @staticmethod
+    def run_mysql(sql_str, db_id=1):
         # 根据后台数据库配置id查询
         out = requests.post(admin_host + "/sql/running_sql/", json={"id": db_id, "sql_str": sql_str}).json()
         if out.get("code") == "0000":
             return out.get("data")
         else:
             assert False, sql_str + str(out.get("msg"))
```

### Comparing `huhk-1.6.8/service/app_t/app_t_sql.py` & `huhk-1.6.9/service/app_t/app_t_sql.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/app_t/assert/open/haohan/assert_open_haohan_relation.py` & `huhk-1.6.9/service/app_t/assert/open/haohan/assert_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/app_t/assert/open/haohan/assert_open_haohan_rights.py` & `huhk-1.6.9/service/app_t/assert/open/haohan/assert_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/app_t/assert/points/assert_points_points.py` & `huhk-1.6.9/service/app_t/assert/points/assert_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/app_t/assert/points/assert_points_pointsApp.py` & `huhk-1.6.9/service/app_t/assert/points/assert_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/app_t/fun/open/haohan/fun_open_haohan_relation.py` & `huhk-1.6.9/service/app_t/fun/open/haohan/fun_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/app_t/fun/open/haohan/fun_open_haohan_rights.py` & `huhk-1.6.9/service/app_t/fun/open/haohan/fun_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/app_t/fun/points/fun_points_points.py` & `huhk-1.6.9/service/app_t/fun/points/fun_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/app_t/sql/open/haohan/sql_open_haohan_relation.py` & `huhk-1.6.9/service/app_t/sql/open/haohan/sql_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/app_t/sql/open/haohan/sql_open_haohan_rights.py` & `huhk-1.6.9/service/app_t/sql/open/haohan/sql_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/app_t/sql/points/sql_points_points.py` & `huhk-1.6.9/service/app_t/sql/points/sql_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/app_t/sql/points/sql_points_pointsApp.py` & `huhk-1.6.9/service/app_t/sql/points/sql_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/demo/demo_api.py` & `huhk-1.6.9/service/demo/demo_api.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/demo/demo_api_fun.py` & `huhk-1.6.9/service/demo/demo_api_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/demo/demo_fun.py` & `huhk-1.6.9/service/demo/demo_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/service/demo/demo_sql.py` & `huhk-1.6.9/service/demo/demo_sql.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/testcase/apache/beam_class.py` & `huhk-1.6.9/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/testcase/apache/data.py` & `huhk-1.6.9/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/testcase/apache/par_do.py` & `huhk-1.6.9/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/testcase/apache/test_cogroupbykey.py` & `huhk-1.6.9/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/testcase/apache/test_fiter.py` & `huhk-1.6.9/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/testcase/apache/test_flatmap.py` & `huhk-1.6.9/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/testcase/apache/test_map.py` & `huhk-1.6.9/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/testcase/apache/test_par_do.py` & `huhk-1.6.9/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/testcase/apache/test_regex.py` & `huhk-1.6.9/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/testcase/apache/test_time.py` & `huhk-1.6.9/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.8/testcase/app_t/test_api.py` & `huhk-1.6.9/testcase/app_t/test_api.py`

 * *Files identical despite different names*

