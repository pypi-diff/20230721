# Comparing `tmp/huhk-1.6.9.tar.gz` & `tmp/huhk-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhk-1.6.9.tar", last modified: Fri Jul 21 09:54:10 2023, max compression
+gzip compressed data, was "huhk-1.7.1.tar", last modified: Fri Jul 21 09:58:52 2023, max compression
```

## Comparing `huhk-1.6.9.tar` & `huhk-1.7.1.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.206579 huhk-1.6.9/
--rw-rw-rw-   0        0        0      223 2023-07-21 09:54:10.205616 huhk-1.6.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:09.961799 huhk-1.6.9/huhk/
--rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.6.9/huhk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:09.988724 huhk-1.6.9/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0      790 2023-07-13 02:39:46.000000 huhk-1.6.9/huhk/case_project/main.py
--rw-rw-rw-   0        0        0    15661 2023-07-21 09:53:53.000000 huhk-1.6.9/huhk/case_project/project_base.py
--rw-rw-rw-   0        0        0     2099 2023-07-21 08:18:22.000000 huhk-1.6.9/huhk/case_project/project_init.py
--rw-rw-rw-   0        0        0    14745 2023-07-21 09:53:53.000000 huhk-1.6.9/huhk/case_project/project_string.py
--rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-21 09:54:09.000000 huhk-1.6.9/huhk/case_project/version.py
--rw-rw-rw-   0        0        0    13077 2023-07-21 08:30:09.000000 huhk-1.6.9/huhk/init_project.py
--rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:09.990718 huhk-1.6.9/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.033605 huhk-1.6.9/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.9/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.6.9/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.6.9/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.6.9/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.6.9/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.6.9/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.6.9/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.6.9/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.6.9/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.6.9/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.6.9/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    26063 2023-07-21 01:52:10.000000 huhk-1.6.9/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9533 2023-07-21 02:12:55.000000 huhk-1.6.9/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2473 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.6.9/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:09.972768 huhk-1.6.9/huhk.egg-info/
--rw-rw-rw-   0        0        0      223 2023-07-21 09:54:09.000000 huhk-1.6.9/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3456 2023-07-21 09:54:09.000000 huhk-1.6.9/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 09:54:09.000000 huhk-1.6.9/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-21 09:54:09.000000 huhk-1.6.9/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-07-21 09:54:09.000000 huhk-1.6.9/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-21 09:54:09.000000 huhk-1.6.9/huhk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.037597 huhk-1.6.9/service/
--rw-rw-rw-   0        0        0        0 2023-07-14 06:51:02.000000 huhk-1.6.9/service/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.052554 huhk-1.6.9/service/app_t/
--rw-rw-rw-   0        0        0      402 2023-07-18 06:58:10.000000 huhk-1.6.9/service/app_t/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.056546 huhk-1.6.9/service/app_t/api/
--rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.6.9/service/app_t/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.059539 huhk-1.6.9/service/app_t/api/open/
--rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.6.9/service/app_t/api/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.069509 huhk-1.6.9/service/app_t/api/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.6.9/service/app_t/api/open/haohan/__init__.py
--rw-rw-rw-   0        0        0     3672 2023-07-21 08:42:38.000000 huhk-1.6.9/service/app_t/api/open/haohan/api_open_haohan_relation.py
--rw-rw-rw-   0        0        0     3837 2023-07-21 08:42:38.000000 huhk-1.6.9/service/app_t/api/open/haohan/api_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.081479 huhk-1.6.9/service/app_t/api/points/
--rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.6.9/service/app_t/api/points/__init__.py
--rw-rw-rw-   0        0        0    18817 2023-07-21 08:42:38.000000 huhk-1.6.9/service/app_t/api/points/api_points_points.py
--rw-rw-rw-   0        0        0    12332 2023-07-21 08:42:38.000000 huhk-1.6.9/service/app_t/api/points/api_points_pointsApp.py
--rw-rw-rw-   0        0        0     6231 2023-07-19 03:10:22.000000 huhk-1.6.9/service/app_t/app_t_api.py
--rw-rw-rw-   0        0        0     7301 2023-07-18 08:08:29.000000 huhk-1.6.9/service/app_t/app_t_api_fun.py
--rw-rw-rw-   0        0        0     3353 2023-07-18 08:08:29.000000 huhk-1.6.9/service/app_t/app_t_assert.py
--rw-rw-rw-   0        0        0      754 2023-07-21 09:47:48.000000 huhk-1.6.9/service/app_t/app_t_fun.py
--rw-rw-rw-   0        0        0     4400 2023-07-21 06:34:11.000000 huhk-1.6.9/service/app_t/app_t_sql.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.083470 huhk-1.6.9/service/app_t/assert/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.6.9/service/app_t/assert/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.086463 huhk-1.6.9/service/app_t/assert/open/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.6.9/service/app_t/assert/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.094444 huhk-1.6.9/service/app_t/assert/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.6.9/service/app_t/assert/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      597 2023-07-21 02:24:25.000000 huhk-1.6.9/service/app_t/assert/open/haohan/assert_open_haohan_relation.py
--rw-rw-rw-   0        0        0      542 2023-07-21 02:21:18.000000 huhk-1.6.9/service/app_t/assert/open/haohan/assert_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.100428 huhk-1.6.9/service/app_t/assert/points/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.6.9/service/app_t/assert/points/__init__.py
--rw-rw-rw-   0        0        0     1561 2023-07-21 02:21:18.000000 huhk-1.6.9/service/app_t/assert/points/assert_points_points.py
--rw-rw-rw-   0        0        0     1224 2023-07-21 02:21:18.000000 huhk-1.6.9/service/app_t/assert/points/assert_points_pointsApp.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.101426 huhk-1.6.9/service/app_t/fun/
--rw-rw-rw-   0        0        0        0 2023-07-18 07:32:47.000000 huhk-1.6.9/service/app_t/fun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.104416 huhk-1.6.9/service/app_t/fun/open/
--rw-rw-rw-   0        0        0        0 2023-07-21 09:26:44.000000 huhk-1.6.9/service/app_t/fun/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.111396 huhk-1.6.9/service/app_t/fun/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-21 09:26:44.000000 huhk-1.6.9/service/app_t/fun/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      819 2023-07-21 09:36:16.000000 huhk-1.6.9/service/app_t/fun/open/haohan/fun_open_haohan_relation.py
--rw-rw-rw-   0        0        0      934 2023-07-21 09:36:16.000000 huhk-1.6.9/service/app_t/fun/open/haohan/fun_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.116382 huhk-1.6.9/service/app_t/fun/points/
--rw-rw-rw-   0        0        0        0 2023-07-21 09:27:08.000000 huhk-1.6.9/service/app_t/fun/points/__init__.py
--rw-rw-rw-   0        0        0      845 2023-07-21 09:36:16.000000 huhk-1.6.9/service/app_t/fun/points/fun_points_points.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.117380 huhk-1.6.9/service/app_t/sql/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:20:20.000000 huhk-1.6.9/service/app_t/sql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.120372 huhk-1.6.9/service/app_t/sql/open/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:20:21.000000 huhk-1.6.9/service/app_t/sql/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.127354 huhk-1.6.9/service/app_t/sql/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:20:21.000000 huhk-1.6.9/service/app_t/sql/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      570 2023-07-21 02:20:21.000000 huhk-1.6.9/service/app_t/sql/open/haohan/sql_open_haohan_relation.py
--rw-rw-rw-   0        0        0      566 2023-07-21 02:20:21.000000 huhk-1.6.9/service/app_t/sql/open/haohan/sql_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.132849 huhk-1.6.9/service/app_t/sql/points/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:20:21.000000 huhk-1.6.9/service/app_t/sql/points/__init__.py
--rw-rw-rw-   0        0        0     1993 2023-07-21 02:20:21.000000 huhk-1.6.9/service/app_t/sql/points/sql_points_points.py
--rw-rw-rw-   0        0        0     1528 2023-07-21 02:20:21.000000 huhk-1.6.9/service/app_t/sql/points/sql_points_pointsApp.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.147808 huhk-1.6.9/service/demo/
--rw-rw-rw-   0        0        0      407 2023-07-14 08:11:52.000000 huhk-1.6.9/service/demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.149803 huhk-1.6.9/service/demo/api/
--rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.9/service/demo/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.151800 huhk-1.6.9/service/demo/assert/
--rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.9/service/demo/assert/__init__.py
--rw-rw-rw-   0        0        0      871 2023-07-18 06:50:22.000000 huhk-1.6.9/service/demo/demo_api.py
--rw-rw-rw-   0        0        0      828 2023-07-18 06:50:22.000000 huhk-1.6.9/service/demo/demo_api_fun.py
--rw-rw-rw-   0        0        0      459 2023-07-18 06:50:22.000000 huhk-1.6.9/service/demo/demo_assert.py
--rw-rw-rw-   0        0        0      721 2023-07-18 06:50:22.000000 huhk-1.6.9/service/demo/demo_fun.py
--rw-rw-rw-   0        0        0      579 2023-07-18 06:50:22.000000 huhk-1.6.9/service/demo/demo_sql.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.154752 huhk-1.6.9/service/demo/fun/
--rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.9/service/demo/fun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.156741 huhk-1.6.9/service/demo/sql/
--rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.9/service/demo/sql/__init__.py
--rw-rw-rw-   0        0        0       42 2023-07-21 09:54:10.207576 huhk-1.6.9/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.6.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.158740 huhk-1.6.9/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.9/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.196607 huhk-1.6.9/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.9/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.9/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.9/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.9/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.6.9/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.6.9/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.6.9/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.6.9/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.6.9/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.6.9/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.6.9/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.6.9/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.6.9/testcase/apache/test_to_string.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:54:10.203591 huhk-1.6.9/testcase/app_t/
--rw-rw-rw-   0        0        0        0 2023-07-14 06:51:02.000000 huhk-1.6.9/testcase/app_t/__init__.py
--rw-rw-rw-   0        0        0     1923 2023-07-18 08:08:29.000000 huhk-1.6.9/testcase/app_t/test_api.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.620431 huhk-1.7.1/
+-rw-rw-rw-   0        0        0      223 2023-07-21 09:58:52.619433 huhk-1.7.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.398334 huhk-1.7.1/huhk/
+-rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.7.1/huhk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.431221 huhk-1.7.1/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.1/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.7.1/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0      790 2023-07-13 02:39:46.000000 huhk-1.7.1/huhk/case_project/main.py
+-rw-rw-rw-   0        0        0    15661 2023-07-21 09:53:53.000000 huhk-1.7.1/huhk/case_project/project_base.py
+-rw-rw-rw-   0        0        0     2099 2023-07-21 08:18:22.000000 huhk-1.7.1/huhk/case_project/project_init.py
+-rw-rw-rw-   0        0        0    14758 2023-07-21 09:58:48.000000 huhk-1.7.1/huhk/case_project/project_string.py
+-rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.7.1/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-21 09:58:52.000000 huhk-1.7.1/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0    13077 2023-07-21 08:30:09.000000 huhk-1.7.1/huhk/init_project.py
+-rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.7.1/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.434224 huhk-1.7.1/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.1/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.478093 huhk-1.7.1/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.1/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.7.1/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.7.1/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.7.1/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.7.1/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.7.1/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.7.1/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.7.1/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.7.1/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.7.1/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.7.1/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.7.1/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.7.1/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.7.1/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.7.1/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.7.1/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    26063 2023-07-21 01:52:10.000000 huhk-1.7.1/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.7.1/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0     9533 2023-07-21 02:12:55.000000 huhk-1.7.1/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2473 2023-07-12 01:13:24.000000 huhk-1.7.1/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.7.1/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.409281 huhk-1.7.1/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-07-21 09:58:52.000000 huhk-1.7.1/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3456 2023-07-21 09:58:52.000000 huhk-1.7.1/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 09:58:52.000000 huhk-1.7.1/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-21 09:58:52.000000 huhk-1.7.1/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-07-21 09:58:52.000000 huhk-1.7.1/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-21 09:58:52.000000 huhk-1.7.1/huhk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.481083 huhk-1.7.1/service/
+-rw-rw-rw-   0        0        0        0 2023-07-14 06:51:02.000000 huhk-1.7.1/service/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.495044 huhk-1.7.1/service/app_t/
+-rw-rw-rw-   0        0        0      402 2023-07-18 06:58:10.000000 huhk-1.7.1/service/app_t/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.496043 huhk-1.7.1/service/app_t/api/
+-rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.7.1/service/app_t/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.499062 huhk-1.7.1/service/app_t/api/open/
+-rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.7.1/service/app_t/api/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.505105 huhk-1.7.1/service/app_t/api/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.7.1/service/app_t/api/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0     3672 2023-07-21 08:42:38.000000 huhk-1.7.1/service/app_t/api/open/haohan/api_open_haohan_relation.py
+-rw-rw-rw-   0        0        0     3837 2023-07-21 08:42:38.000000 huhk-1.7.1/service/app_t/api/open/haohan/api_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.512054 huhk-1.7.1/service/app_t/api/points/
+-rw-rw-rw-   0        0        0        0 2023-07-21 03:30:53.000000 huhk-1.7.1/service/app_t/api/points/__init__.py
+-rw-rw-rw-   0        0        0    18817 2023-07-21 08:42:38.000000 huhk-1.7.1/service/app_t/api/points/api_points_points.py
+-rw-rw-rw-   0        0        0    12332 2023-07-21 08:42:38.000000 huhk-1.7.1/service/app_t/api/points/api_points_pointsApp.py
+-rw-rw-rw-   0        0        0     6231 2023-07-19 03:10:22.000000 huhk-1.7.1/service/app_t/app_t_api.py
+-rw-rw-rw-   0        0        0     7301 2023-07-18 08:08:29.000000 huhk-1.7.1/service/app_t/app_t_api_fun.py
+-rw-rw-rw-   0        0        0     3353 2023-07-18 08:08:29.000000 huhk-1.7.1/service/app_t/app_t_assert.py
+-rw-rw-rw-   0        0        0      754 2023-07-21 09:47:48.000000 huhk-1.7.1/service/app_t/app_t_fun.py
+-rw-rw-rw-   0        0        0     4400 2023-07-21 06:34:11.000000 huhk-1.7.1/service/app_t/app_t_sql.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.513050 huhk-1.7.1/service/app_t/assert/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.7.1/service/app_t/assert/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.516041 huhk-1.7.1/service/app_t/assert/open/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.7.1/service/app_t/assert/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.522168 huhk-1.7.1/service/app_t/assert/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.7.1/service/app_t/assert/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      597 2023-07-21 02:24:25.000000 huhk-1.7.1/service/app_t/assert/open/haohan/assert_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      542 2023-07-21 02:21:18.000000 huhk-1.7.1/service/app_t/assert/open/haohan/assert_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.528144 huhk-1.7.1/service/app_t/assert/points/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:21:18.000000 huhk-1.7.1/service/app_t/assert/points/__init__.py
+-rw-rw-rw-   0        0        0     1561 2023-07-21 02:21:18.000000 huhk-1.7.1/service/app_t/assert/points/assert_points_points.py
+-rw-rw-rw-   0        0        0     1224 2023-07-21 02:21:18.000000 huhk-1.7.1/service/app_t/assert/points/assert_points_pointsApp.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.530146 huhk-1.7.1/service/app_t/fun/
+-rw-rw-rw-   0        0        0        0 2023-07-18 07:32:47.000000 huhk-1.7.1/service/app_t/fun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.533109 huhk-1.7.1/service/app_t/fun/open/
+-rw-rw-rw-   0        0        0        0 2023-07-21 09:26:44.000000 huhk-1.7.1/service/app_t/fun/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.540084 huhk-1.7.1/service/app_t/fun/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-21 09:26:44.000000 huhk-1.7.1/service/app_t/fun/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      819 2023-07-21 09:54:25.000000 huhk-1.7.1/service/app_t/fun/open/haohan/fun_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      934 2023-07-21 09:54:25.000000 huhk-1.7.1/service/app_t/fun/open/haohan/fun_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.544107 huhk-1.7.1/service/app_t/fun/points/
+-rw-rw-rw-   0        0        0        0 2023-07-21 09:27:08.000000 huhk-1.7.1/service/app_t/fun/points/__init__.py
+-rw-rw-rw-   0        0        0     4280 2023-07-21 09:54:25.000000 huhk-1.7.1/service/app_t/fun/points/fun_points_points.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.546101 huhk-1.7.1/service/app_t/sql/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:20:20.000000 huhk-1.7.1/service/app_t/sql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.548097 huhk-1.7.1/service/app_t/sql/open/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:20:21.000000 huhk-1.7.1/service/app_t/sql/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.554079 huhk-1.7.1/service/app_t/sql/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:20:21.000000 huhk-1.7.1/service/app_t/sql/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      570 2023-07-21 02:20:21.000000 huhk-1.7.1/service/app_t/sql/open/haohan/sql_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      566 2023-07-21 02:20:21.000000 huhk-1.7.1/service/app_t/sql/open/haohan/sql_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.560030 huhk-1.7.1/service/app_t/sql/points/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:20:21.000000 huhk-1.7.1/service/app_t/sql/points/__init__.py
+-rw-rw-rw-   0        0        0     1993 2023-07-21 02:20:21.000000 huhk-1.7.1/service/app_t/sql/points/sql_points_points.py
+-rw-rw-rw-   0        0        0     1528 2023-07-21 02:20:21.000000 huhk-1.7.1/service/app_t/sql/points/sql_points_pointsApp.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.571034 huhk-1.7.1/service/demo/
+-rw-rw-rw-   0        0        0      407 2023-07-14 08:11:52.000000 huhk-1.7.1/service/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.571996 huhk-1.7.1/service/demo/api/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.7.1/service/demo/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.574990 huhk-1.7.1/service/demo/assert/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.7.1/service/demo/assert/__init__.py
+-rw-rw-rw-   0        0        0      871 2023-07-18 06:50:22.000000 huhk-1.7.1/service/demo/demo_api.py
+-rw-rw-rw-   0        0        0      828 2023-07-18 06:50:22.000000 huhk-1.7.1/service/demo/demo_api_fun.py
+-rw-rw-rw-   0        0        0      459 2023-07-18 06:50:22.000000 huhk-1.7.1/service/demo/demo_assert.py
+-rw-rw-rw-   0        0        0      721 2023-07-18 06:50:22.000000 huhk-1.7.1/service/demo/demo_fun.py
+-rw-rw-rw-   0        0        0      579 2023-07-18 06:50:22.000000 huhk-1.7.1/service/demo/demo_sql.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.577018 huhk-1.7.1/service/demo/fun/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.7.1/service/demo/fun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.578977 huhk-1.7.1/service/demo/sql/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.7.1/service/demo/sql/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-21 09:58:52.620431 huhk-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.580973 huhk-1.7.1/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.1/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.612453 huhk-1.7.1/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.1/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.7.1/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.7.1/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.7.1/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.7.1/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.7.1/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.7.1/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.7.1/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.7.1/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.7.1/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.7.1/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.7.1/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.7.1/testcase/apache/test_to_string.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:58:52.617474 huhk-1.7.1/testcase/app_t/
+-rw-rw-rw-   0        0        0        0 2023-07-14 06:51:02.000000 huhk-1.7.1/testcase/app_t/__init__.py
+-rw-rw-rw-   0        0        0     1923 2023-07-18 08:08:29.000000 huhk-1.7.1/testcase/app_t/test_api.py
```

### Comparing `huhk-1.6.9/huhk/__init__.py` & `huhk-1.7.1/huhk/__init__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/case_project/json_coder.py` & `huhk-1.7.1/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/case_project/main.py` & `huhk-1.7.1/huhk/case_project/main.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/case_project/project_base.py` & `huhk-1.7.1/huhk/case_project/project_base.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/case_project/project_init.py` & `huhk-1.7.1/huhk/case_project/project_init.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/case_project/project_string.py` & `huhk-1.7.1/huhk/case_project/project_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         assert_fun_str += '        assert True, "数据比较不一致"\n\n'
         return assert_fun_str
 
     def get_api_fun_header_str(self, fun_name):
         assert_path = self.get_path(fun_name, fun_type='assert')
         fun_path = self.get_path(fun_name, fun_type='fun')
         header_str = "import allure\n\n"
-        header_str += "from service.app_t.app_t_assert import App_TAssert\n"
+        header_str += f"from {assert_path.import_path} import {assert_path.class_name}\n"
         header_str += "from service.app_t import app_t_api\n\n\n"
         header_str += f"class {fun_path.class_name}({assert_path.class_name}):\n"
         return header_str
 
     def get_api_fun_fun_str(self, fun_name):
         api = self.this_fun_list.api[fun_name]
         data_list_tmp = []
```

### Comparing `huhk-1.6.9/huhk/case_project/setup_set.py` & `huhk-1.7.1/huhk/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/init_project.py` & `huhk-1.7.1/huhk/init_project.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/testcase/apache/beam_class.py` & `huhk-1.7.1/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/testcase/apache/data.py` & `huhk-1.7.1/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/testcase/apache/par_do.py` & `huhk-1.7.1/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.7.1/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/testcase/apache/test_fiter.py` & `huhk-1.7.1/huhk/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/testcase/apache/test_flatmap.py` & `huhk-1.7.1/huhk/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/testcase/apache/test_map.py` & `huhk-1.7.1/huhk/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/testcase/apache/test_par_do.py` & `huhk-1.7.1/huhk/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/testcase/apache/test_regex.py` & `huhk-1.7.1/huhk/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/testcase/apache/test_time.py` & `huhk-1.7.1/huhk/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/unit_apache_beam.py` & `huhk-1.7.1/huhk/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/unit_dict.py` & `huhk-1.7.1/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/unit_encryption.py` & `huhk-1.7.1/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/unit_fun.py` & `huhk-1.7.1/huhk/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/unit_logger.py` & `huhk-1.7.1/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/unit_request.py` & `huhk-1.7.1/huhk/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/unit_tasks.py` & `huhk-1.7.1/huhk/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk/常用命令.py` & `huhk-1.7.1/huhk/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/huhk.egg-info/SOURCES.txt` & `huhk-1.7.1/huhk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/app_t/api/open/haohan/api_open_haohan_relation.py` & `huhk-1.7.1/service/app_t/api/open/haohan/api_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/app_t/api/open/haohan/api_open_haohan_rights.py` & `huhk-1.7.1/service/app_t/api/open/haohan/api_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/app_t/api/points/api_points_points.py` & `huhk-1.7.1/service/app_t/api/points/api_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/app_t/api/points/api_points_pointsApp.py` & `huhk-1.7.1/service/app_t/api/points/api_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/app_t/app_t_api.py` & `huhk-1.7.1/service/app_t/app_t_api.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/app_t/app_t_api_fun.py` & `huhk-1.7.1/service/app_t/app_t_api_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/app_t/app_t_assert.py` & `huhk-1.7.1/service/app_t/app_t_assert.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/app_t/app_t_fun.py` & `huhk-1.7.1/service/app_t/app_t_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/app_t/app_t_sql.py` & `huhk-1.7.1/service/app_t/app_t_sql.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/app_t/assert/open/haohan/assert_open_haohan_relation.py` & `huhk-1.7.1/service/app_t/assert/open/haohan/assert_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/app_t/assert/open/haohan/assert_open_haohan_rights.py` & `huhk-1.7.1/service/app_t/assert/open/haohan/assert_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/app_t/assert/points/assert_points_points.py` & `huhk-1.7.1/service/app_t/assert/points/assert_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/app_t/assert/points/assert_points_pointsApp.py` & `huhk-1.7.1/service/app_t/assert/points/assert_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/app_t/fun/open/haohan/fun_open_haohan_relation.py` & `huhk-1.7.1/service/app_t/fun/open/haohan/fun_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/app_t/fun/open/haohan/fun_open_haohan_rights.py` & `huhk-1.7.1/service/app_t/fun/open/haohan/fun_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/app_t/fun/points/fun_points_points.py` & `huhk-1.7.1/service/demo/demo_api_fun.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,28 @@
-    @allure.step(title="查看积分明细- - 积分流水分页查询")
-    @allure.step(title="查看积分明细- - 积分流水分页查询")
-    def points_points_flowDetail(self, userId="$None$", _assert=True,  **kwargs):
-        """
-            url=/points/points/flowDetail
-                params: headers : 请求头
-        """
-        userId = self.get_value_choice(userId, list_or_dict=None)
+from service.demo.demo_assert import DemoAssert
+from service.demo import demo_api
+
+import allure
+
+
+class DemoApiFun(DemoAssert):
+    @allure.step(title="发送手机验证码")
+    def demo(self, mobile="$None$", headers="$None$", _assert=True,  **kwargs):
+        """url=/common/common/sendSmsCode
+        params: mobile :  : 用户电话号码"""
+        mobile = self.get_value_choice(mobile, list_or_dict=None)
 
         _kwargs = self.get_kwargs(locals())
-        self.res = app_t_api.points_points_flowDetail(**_kwargs)
+        self.res = demo_api.demo(**_kwargs)
 
-        self.input_value.userId = userId
+        self._v_mobile = mobile
 
         if _assert is True:
-            self.assert_points_points_flowDetail(**_kwargs)
-        elif _assert is not True:
-            assert self.res.rsp.code == _assert or self.res.status_code == _assert, "校验code=%s不通过" % _assert
+            self.assert_demo(**_kwargs)
+        elif _assert is not False:
+            assert self.res.rsp.code == _assert, "校验code=%s不通过" % _assert
         return self.res
 
 
+if __name__ == '__main__':
+    s = DemoApiFun()
+
```

### Comparing `huhk-1.6.9/service/app_t/sql/open/haohan/sql_open_haohan_relation.py` & `huhk-1.7.1/service/app_t/sql/open/haohan/sql_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/app_t/sql/open/haohan/sql_open_haohan_rights.py` & `huhk-1.7.1/service/app_t/sql/open/haohan/sql_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/app_t/sql/points/sql_points_points.py` & `huhk-1.7.1/service/app_t/sql/points/sql_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/app_t/sql/points/sql_points_pointsApp.py` & `huhk-1.7.1/service/app_t/sql/points/sql_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/demo/demo_api.py` & `huhk-1.7.1/service/demo/demo_api.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/demo/demo_fun.py` & `huhk-1.7.1/service/demo/demo_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/service/demo/demo_sql.py` & `huhk-1.7.1/service/demo/demo_sql.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/testcase/apache/beam_class.py` & `huhk-1.7.1/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/testcase/apache/data.py` & `huhk-1.7.1/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/testcase/apache/par_do.py` & `huhk-1.7.1/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/testcase/apache/test_cogroupbykey.py` & `huhk-1.7.1/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/testcase/apache/test_fiter.py` & `huhk-1.7.1/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/testcase/apache/test_flatmap.py` & `huhk-1.7.1/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/testcase/apache/test_map.py` & `huhk-1.7.1/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/testcase/apache/test_par_do.py` & `huhk-1.7.1/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/testcase/apache/test_regex.py` & `huhk-1.7.1/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/testcase/apache/test_time.py` & `huhk-1.7.1/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.9/testcase/app_t/test_api.py` & `huhk-1.7.1/testcase/app_t/test_api.py`

 * *Files identical despite different names*

