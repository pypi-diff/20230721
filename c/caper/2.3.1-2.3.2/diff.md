# Comparing `tmp/caper-2.3.1.tar.gz` & `tmp/caper-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caper-2.3.1.tar", last modified: Thu May  4 21:26:21 2023, max compression
+gzip compressed data, was "caper-2.3.2.tar", last modified: Fri Jul 21 19:53:30 2023, max compression
```

## Comparing `caper-2.3.1.tar` & `caper-2.3.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-05-04 21:26:21.847903 caper-2.3.1/
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1067 2022-06-10 20:40:20.000000 caper-2.3.1/LICENSE
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      457 2023-05-04 21:26:21.847903 caper-2.3.1/PKG-INFO
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     9015 2023-05-04 21:24:00.000000 caper-2.3.1/README.md
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-05-04 21:26:21.795904 caper-2.3.1/bin/
--rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)      295 2022-06-10 20:40:20.000000 caper-2.3.1/bin/caper
--rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)     2285 2022-06-10 20:40:20.000000 caper-2.3.1/bin/run_mysql_server_docker.sh
--rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)     2563 2022-06-10 20:40:20.000000 caper-2.3.1/bin/run_mysql_server_singularity.sh
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-05-04 21:26:21.823903 caper-2.3.1/caper/
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      180 2023-05-04 21:24:00.000000 caper-2.3.1/caper/__init__.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       61 2022-06-10 20:40:20.000000 caper-2.3.1/caper/__main__.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     5322 2023-05-04 21:24:00.000000 caper-2.3.1/caper/arg_tool.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      528 2022-06-10 20:40:20.000000 caper-2.3.1/caper/backward_compatibility.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    36785 2023-05-04 21:24:00.000000 caper-2.3.1/caper/caper_args.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    15742 2022-07-25 22:46:52.000000 caper-2.3.1/caper/caper_backend_conf.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     7780 2023-05-04 21:24:00.000000 caper-2.3.1/caper/caper_base.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    14581 2022-06-10 20:40:20.000000 caper-2.3.1/caper/caper_client.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     5199 2023-05-04 21:24:00.000000 caper-2.3.1/caper/caper_init.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2180 2022-06-10 20:40:20.000000 caper-2.3.1/caper/caper_labels.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    22800 2023-05-04 21:24:00.000000 caper-2.3.1/caper/caper_runner.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2599 2023-05-04 21:24:00.000000 caper-2.3.1/caper/caper_wdl_parser.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    11869 2022-06-10 20:40:20.000000 caper-2.3.1/caper/caper_workflow_opts.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    25758 2023-05-04 21:24:00.000000 caper-2.3.1/caper/cli.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2660 2023-05-04 21:24:00.000000 caper-2.3.1/caper/cli_hpc.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    17327 2023-05-04 21:24:00.000000 caper-2.3.1/caper/cromwell.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    41912 2023-05-04 21:24:00.000000 caper-2.3.1/caper/cromwell_backend.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    17381 2023-05-04 21:24:00.000000 caper-2.3.1/caper/cromwell_metadata.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    18525 2023-05-04 21:24:00.000000 caper-2.3.1/caper/cromwell_rest_api.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    13873 2023-05-04 21:24:00.000000 caper-2.3.1/caper/cromwell_workflow_monitor.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     8639 2023-05-04 21:24:00.000000 caper-2.3.1/caper/dict_tool.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6705 2023-05-04 21:24:00.000000 caper-2.3.1/caper/hocon_string.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     7534 2023-05-04 21:24:00.000000 caper-2.3.1/caper/hpc.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     9319 2023-05-04 21:24:00.000000 caper-2.3.1/caper/nb_subproc_thread.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    12256 2022-06-10 20:40:20.000000 caper-2.3.1/caper/resource_analysis.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     4407 2022-06-10 20:40:20.000000 caper-2.3.1/caper/server_heartbeat.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2755 2022-06-10 20:40:20.000000 caper-2.3.1/caper/singularity.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     7455 2023-05-04 21:24:00.000000 caper-2.3.1/caper/wdl_parser.py
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-05-04 21:26:21.827903 caper-2.3.1/caper.egg-info/
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      457 2023-05-04 21:26:21.000000 caper-2.3.1/caper.egg-info/PKG-INFO
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1469 2023-05-04 21:26:21.000000 caper-2.3.1/caper.egg-info/SOURCES.txt
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)        1 2023-05-04 21:26:21.000000 caper-2.3.1/caper.egg-info/dependency_links.txt
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      171 2023-05-04 21:26:21.000000 caper-2.3.1/caper.egg-info/requires.txt
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       12 2023-05-04 21:26:21.000000 caper-2.3.1/caper.egg-info/top_level.txt
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-05-04 21:26:21.795904 caper-2.3.1/scripts/
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-05-04 21:26:21.831903 caper-2.3.1/scripts/gcp_caper_server/
--rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)    11437 2022-07-21 17:02:18.000000 caper-2.3.1/scripts/gcp_caper_server/create_instance.sh
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       38 2023-05-04 21:26:21.847903 caper-2.3.1/setup.cfg
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1877 2023-05-04 21:24:00.000000 caper-2.3.1/setup.py
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-05-04 21:26:21.847903 caper-2.3.1/tests/
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)        0 2022-06-10 20:40:20.000000 caper-2.3.1/tests/__init__.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2186 2023-05-04 21:24:00.000000 caper-2.3.1/tests/conftest.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3885 2022-06-10 20:40:20.000000 caper-2.3.1/tests/example_wdl.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6057 2022-06-10 20:40:20.000000 caper-2.3.1/tests/test_arg_tool.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1029 2022-06-10 20:40:20.000000 caper-2.3.1/tests/test_caper_labels.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1107 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_caper_wdl_parser.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     9479 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_caper_workflow_opts.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     7079 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_cli_run.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     4731 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_cli_server_client_gcp.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6251 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_cromwell.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1282 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_cromwell_backend.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3183 2022-06-10 20:40:20.000000 caper-2.3.1/tests/test_cromwell_metadata.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6129 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_cromwell_rest_api.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3857 2022-06-10 20:40:20.000000 caper-2.3.1/tests/test_dict_tool.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     5983 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_hocon_string.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2595 2022-06-10 20:40:20.000000 caper-2.3.1/tests/test_nb_subproc_thread.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3114 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_resource_analysis.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      886 2022-06-10 20:40:20.000000 caper-2.3.1/tests/test_server_heartbeat.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1755 2022-06-10 20:40:20.000000 caper-2.3.1/tests/test_singularity.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1957 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_wdl_parser.py
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-07-21 19:53:30.099841 caper-2.3.2/
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1067 2022-06-10 20:40:20.000000 caper-2.3.2/LICENSE
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      457 2023-07-21 19:53:30.099841 caper-2.3.2/PKG-INFO
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     9015 2023-05-04 21:24:00.000000 caper-2.3.2/README.md
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-07-21 19:53:30.075841 caper-2.3.2/bin/
+-rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)      295 2022-06-10 20:40:20.000000 caper-2.3.2/bin/caper
+-rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)     2285 2022-06-10 20:40:20.000000 caper-2.3.2/bin/run_mysql_server_docker.sh
+-rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)     2563 2022-06-10 20:40:20.000000 caper-2.3.2/bin/run_mysql_server_singularity.sh
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-07-21 19:53:30.087841 caper-2.3.2/caper/
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      180 2023-07-21 18:41:02.000000 caper-2.3.2/caper/__init__.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       61 2022-06-10 20:40:20.000000 caper-2.3.2/caper/__main__.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     5322 2023-05-04 21:24:00.000000 caper-2.3.2/caper/arg_tool.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      528 2022-06-10 20:40:20.000000 caper-2.3.2/caper/backward_compatibility.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    36785 2023-05-04 21:24:00.000000 caper-2.3.2/caper/caper_args.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    15742 2022-07-25 22:46:52.000000 caper-2.3.2/caper/caper_backend_conf.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     7780 2023-05-04 21:24:00.000000 caper-2.3.2/caper/caper_base.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    14581 2022-06-10 20:40:20.000000 caper-2.3.2/caper/caper_client.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     5199 2023-05-04 21:24:00.000000 caper-2.3.2/caper/caper_init.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2180 2022-06-10 20:40:20.000000 caper-2.3.2/caper/caper_labels.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    22800 2023-05-04 21:24:00.000000 caper-2.3.2/caper/caper_runner.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2599 2023-05-04 21:24:00.000000 caper-2.3.2/caper/caper_wdl_parser.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    11869 2022-06-10 20:40:20.000000 caper-2.3.2/caper/caper_workflow_opts.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    25758 2023-05-04 21:24:00.000000 caper-2.3.2/caper/cli.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2660 2023-05-04 21:24:00.000000 caper-2.3.2/caper/cli_hpc.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    17327 2023-05-04 21:24:00.000000 caper-2.3.2/caper/cromwell.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    41912 2023-05-04 21:24:00.000000 caper-2.3.2/caper/cromwell_backend.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    17381 2023-05-04 21:24:00.000000 caper-2.3.2/caper/cromwell_metadata.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    18525 2023-05-04 21:24:00.000000 caper-2.3.2/caper/cromwell_rest_api.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    13873 2023-05-04 21:24:00.000000 caper-2.3.2/caper/cromwell_workflow_monitor.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     8639 2023-05-04 21:24:00.000000 caper-2.3.2/caper/dict_tool.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6705 2023-05-04 21:24:00.000000 caper-2.3.2/caper/hocon_string.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     7534 2023-05-04 21:24:00.000000 caper-2.3.2/caper/hpc.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     9319 2023-05-04 21:24:00.000000 caper-2.3.2/caper/nb_subproc_thread.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    12256 2022-06-10 20:40:20.000000 caper-2.3.2/caper/resource_analysis.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     4407 2022-06-10 20:40:20.000000 caper-2.3.2/caper/server_heartbeat.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2755 2022-06-10 20:40:20.000000 caper-2.3.2/caper/singularity.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     7455 2023-05-04 21:24:00.000000 caper-2.3.2/caper/wdl_parser.py
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-07-21 19:53:30.087841 caper-2.3.2/caper.egg-info/
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      457 2023-07-21 19:53:29.000000 caper-2.3.2/caper.egg-info/PKG-INFO
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1469 2023-07-21 19:53:29.000000 caper-2.3.2/caper.egg-info/SOURCES.txt
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)        1 2023-07-21 19:53:29.000000 caper-2.3.2/caper.egg-info/dependency_links.txt
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      159 2023-07-21 19:53:29.000000 caper-2.3.2/caper.egg-info/requires.txt
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       12 2023-07-21 19:53:29.000000 caper-2.3.2/caper.egg-info/top_level.txt
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-07-21 19:53:30.075841 caper-2.3.2/scripts/
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-07-21 19:53:30.087841 caper-2.3.2/scripts/gcp_caper_server/
+-rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)    11437 2022-07-21 17:02:18.000000 caper-2.3.2/scripts/gcp_caper_server/create_instance.sh
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       38 2023-07-21 19:53:30.099841 caper-2.3.2/setup.cfg
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1854 2023-07-21 18:40:30.000000 caper-2.3.2/setup.py
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-07-21 19:53:30.095841 caper-2.3.2/tests/
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)        0 2022-06-10 20:40:20.000000 caper-2.3.2/tests/__init__.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2186 2023-05-04 21:24:00.000000 caper-2.3.2/tests/conftest.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3885 2022-06-10 20:40:20.000000 caper-2.3.2/tests/example_wdl.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6057 2022-06-10 20:40:20.000000 caper-2.3.2/tests/test_arg_tool.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1029 2022-06-10 20:40:20.000000 caper-2.3.2/tests/test_caper_labels.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1107 2023-05-04 21:24:00.000000 caper-2.3.2/tests/test_caper_wdl_parser.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     9479 2023-05-04 21:24:00.000000 caper-2.3.2/tests/test_caper_workflow_opts.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     7079 2023-05-04 21:24:00.000000 caper-2.3.2/tests/test_cli_run.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     4731 2023-05-04 21:24:00.000000 caper-2.3.2/tests/test_cli_server_client_gcp.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6251 2023-05-04 21:24:00.000000 caper-2.3.2/tests/test_cromwell.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1282 2023-05-04 21:24:00.000000 caper-2.3.2/tests/test_cromwell_backend.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3183 2022-06-10 20:40:20.000000 caper-2.3.2/tests/test_cromwell_metadata.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6129 2023-05-04 21:24:00.000000 caper-2.3.2/tests/test_cromwell_rest_api.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3857 2022-06-10 20:40:20.000000 caper-2.3.2/tests/test_dict_tool.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     5983 2023-05-04 21:24:00.000000 caper-2.3.2/tests/test_hocon_string.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2595 2022-06-10 20:40:20.000000 caper-2.3.2/tests/test_nb_subproc_thread.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3114 2023-05-04 21:24:00.000000 caper-2.3.2/tests/test_resource_analysis.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      886 2022-06-10 20:40:20.000000 caper-2.3.2/tests/test_server_heartbeat.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1755 2022-06-10 20:40:20.000000 caper-2.3.2/tests/test_singularity.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1957 2023-05-04 21:24:00.000000 caper-2.3.2/tests/test_wdl_parser.py
```

### Comparing `caper-2.3.1/LICENSE` & `caper-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/README.md` & `caper-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/bin/run_mysql_server_docker.sh` & `caper-2.3.2/bin/run_mysql_server_docker.sh`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/bin/run_mysql_server_singularity.sh` & `caper-2.3.2/bin/run_mysql_server_singularity.sh`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/arg_tool.py` & `caper-2.3.2/caper/arg_tool.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/backward_compatibility.py` & `caper-2.3.2/caper/backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/caper_args.py` & `caper-2.3.2/caper/caper_args.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/caper_backend_conf.py` & `caper-2.3.2/caper/caper_backend_conf.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/caper_base.py` & `caper-2.3.2/caper/caper_base.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/caper_client.py` & `caper-2.3.2/caper/caper_client.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/caper_init.py` & `caper-2.3.2/caper/caper_init.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/caper_labels.py` & `caper-2.3.2/caper/caper_labels.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/caper_runner.py` & `caper-2.3.2/caper/caper_runner.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/caper_wdl_parser.py` & `caper-2.3.2/caper/caper_wdl_parser.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/caper_workflow_opts.py` & `caper-2.3.2/caper/caper_workflow_opts.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/cli.py` & `caper-2.3.2/caper/cli.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/cli_hpc.py` & `caper-2.3.2/caper/cli_hpc.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/cromwell.py` & `caper-2.3.2/caper/cromwell.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/cromwell_backend.py` & `caper-2.3.2/caper/cromwell_backend.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/cromwell_metadata.py` & `caper-2.3.2/caper/cromwell_metadata.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/cromwell_rest_api.py` & `caper-2.3.2/caper/cromwell_rest_api.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/cromwell_workflow_monitor.py` & `caper-2.3.2/caper/cromwell_workflow_monitor.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/dict_tool.py` & `caper-2.3.2/caper/dict_tool.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/hocon_string.py` & `caper-2.3.2/caper/hocon_string.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/hpc.py` & `caper-2.3.2/caper/hpc.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/nb_subproc_thread.py` & `caper-2.3.2/caper/nb_subproc_thread.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/resource_analysis.py` & `caper-2.3.2/caper/resource_analysis.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/server_heartbeat.py` & `caper-2.3.2/caper/server_heartbeat.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/singularity.py` & `caper-2.3.2/caper/singularity.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper/wdl_parser.py` & `caper-2.3.2/caper/wdl_parser.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/caper.egg-info/SOURCES.txt` & `caper-2.3.2/caper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/scripts/gcp_caper_server/create_instance.sh` & `caper-2.3.2/scripts/gcp_caper_server/create_instance.sh`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/setup.py` & `caper-2.3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,10 +65,9 @@
         'miniwdl>=0.7.0',
         'humanfriendly',
         'numpy>=1.8.2',
         'pandas>=1.0',
         'scikit-learn>=0.19.2',
         'matplotlib>=1.5',
         'six>=1.13.0',
-        'pyyaml<=5.5',
     ],
 )
```

### Comparing `caper-2.3.1/tests/conftest.py` & `caper-2.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/tests/example_wdl.py` & `caper-2.3.2/tests/example_wdl.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/tests/test_arg_tool.py` & `caper-2.3.2/tests/test_arg_tool.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/tests/test_caper_labels.py` & `caper-2.3.2/tests/test_caper_labels.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/tests/test_caper_wdl_parser.py` & `caper-2.3.2/tests/test_caper_wdl_parser.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/tests/test_caper_workflow_opts.py` & `caper-2.3.2/tests/test_caper_workflow_opts.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/tests/test_cli_run.py` & `caper-2.3.2/tests/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/tests/test_cli_server_client_gcp.py` & `caper-2.3.2/tests/test_cli_server_client_gcp.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/tests/test_cromwell.py` & `caper-2.3.2/tests/test_cromwell.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/tests/test_cromwell_backend.py` & `caper-2.3.2/tests/test_cromwell_backend.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/tests/test_cromwell_metadata.py` & `caper-2.3.2/tests/test_cromwell_metadata.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/tests/test_cromwell_rest_api.py` & `caper-2.3.2/tests/test_cromwell_rest_api.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/tests/test_dict_tool.py` & `caper-2.3.2/tests/test_dict_tool.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/tests/test_hocon_string.py` & `caper-2.3.2/tests/test_hocon_string.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/tests/test_nb_subproc_thread.py` & `caper-2.3.2/tests/test_nb_subproc_thread.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/tests/test_resource_analysis.py` & `caper-2.3.2/tests/test_resource_analysis.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/tests/test_server_heartbeat.py` & `caper-2.3.2/tests/test_server_heartbeat.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/tests/test_singularity.py` & `caper-2.3.2/tests/test_singularity.py`

 * *Files identical despite different names*

### Comparing `caper-2.3.1/tests/test_wdl_parser.py` & `caper-2.3.2/tests/test_wdl_parser.py`

 * *Files identical despite different names*

