# Comparing `tmp/autosubmit-4.0.82.tar.gz` & `tmp/autosubmit-4.0.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosubmit-4.0.82.tar", last modified: Thu Jul 20 07:03:39 2023, max compression
+gzip compressed data, was "autosubmit-4.0.84.tar", last modified: Fri Jul 21 08:56:31 2023, max compression
```

## Comparing `autosubmit-4.0.82.tar` & `autosubmit-4.0.84.tar`

### file list

```diff
@@ -1,407 +1,407 @@
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.035902 autosubmit-4.0.82/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      226 2023-07-13 10:54:33.000000 autosubmit-4.0.82/.gitignore
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1361 2023-07-13 10:54:33.000000 autosubmit-4.0.82/.gitlab-ci.yml
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      937 2023-07-13 10:54:33.000000 autosubmit-4.0.82/.readthedocs.yaml
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.82/CHANGELOG
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      722 2023-07-13 10:54:33.000000 autosubmit-4.0.82/CONTRIBUTING.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    35147 2021-10-05 14:18:20.000000 autosubmit-4.0.82/LICENSE
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      119 2021-10-05 14:18:20.000000 autosubmit-4.0.82/MANIFEST.in
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3347 2023-07-20 07:03:39.035902 autosubmit-4.0.82/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5651 2023-07-13 10:54:33.000000 autosubmit-4.0.82/README.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2287 2023-07-13 10:54:33.000000 autosubmit-4.0.82/README_PIP.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        7 2023-07-20 07:03:37.000000 autosubmit-4.0.82/VERSION
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.007902 autosubmit-4.0.82/autosubmit/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.82/autosubmit/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   324689 2023-07-20 07:03:32.000000 autosubmit-4.0.82/autosubmit/autosubmit.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.007902 autosubmit-4.0.82/autosubmit/database/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.82/autosubmit/database/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.007902 autosubmit-4.0.82/autosubmit/database/data/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      258 2021-10-05 14:18:20.000000 autosubmit-4.0.82/autosubmit/database/data/autosubmit.sql
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19910 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/database/db_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7593 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/database/db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6065 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/database/db_structure.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.007902 autosubmit-4.0.82/autosubmit/experiment/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.82/autosubmit/experiment/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5280 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/experiment/experiment_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8450 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/experiment/statistics.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.007902 autosubmit-4.0.82/autosubmit/git/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.82/autosubmit/git/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13703 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/git/autosubmit_git.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.007902 autosubmit-4.0.82/autosubmit/helpers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.82/autosubmit/helpers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5776 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/helpers/autosubmit_helper.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      194 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/helpers/data_transfer.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3304 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/helpers/parameters.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1428 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/helpers/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.007902 autosubmit-4.0.82/autosubmit/history/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.82/autosubmit/history/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.007902 autosubmit-4.0.82/autosubmit/history/data_classes/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.82/autosubmit/history/data_classes/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2432 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/history/data_classes/experiment_run.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10305 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/history/data_classes/job_data.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.011902 autosubmit-4.0.82/autosubmit/history/database_managers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.82/autosubmit/history/database_managers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5688 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/history/database_managers/database_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2409 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/history/database_managers/database_models.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19251 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/history/database_managers/experiment_history_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6456 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/history/database_managers/experiment_status_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18844 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/history/experiment_history.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2382 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/history/experiment_status.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1952 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/history/internal_logging.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.011902 autosubmit-4.0.82/autosubmit/history/platform_monitor/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.82/autosubmit/history/platform_monitor/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.011902 autosubmit-4.0.82/autosubmit/history/platform_monitor/output_examples/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/history/platform_monitor/output_examples/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2022-11-21 08:34:36.000000 autosubmit-4.0.82/autosubmit/history/platform_monitor/output_examples/pending.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      554 2022-11-21 08:34:36.000000 autosubmit-4.0.82/autosubmit/history/platform_monitor/output_examples/wrapper1.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      549 2022-11-21 08:34:36.000000 autosubmit-4.0.82/autosubmit/history/platform_monitor/output_examples/wrapper2.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6105 2022-11-21 08:34:36.000000 autosubmit-4.0.82/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1025 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/history/platform_monitor/platform_monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2298 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/history/platform_monitor/platform_utils.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2475 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/history/platform_monitor/slurm_monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3454 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/history/platform_monitor/slurm_monitor_item.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10951 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/history/strategies.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2784 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/history/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.011902 autosubmit-4.0.82/autosubmit/job/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.82/autosubmit/job/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    99727 2023-07-20 07:01:43.000000 autosubmit-4.0.82/autosubmit/job/job.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10907 2023-07-20 06:53:28.000000 autosubmit-4.0.82/autosubmit/job/job_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20136 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/job/job_dict.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13797 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/job/job_grouping.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   127858 2023-07-20 06:53:28.000000 autosubmit-4.0.82/autosubmit/job/job_list.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4609 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/job/job_list_persistence.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3565 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/job/job_package_persistence.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    62148 2023-07-20 06:53:28.000000 autosubmit-4.0.82/autosubmit/job/job_packager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    38100 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/job/job_packages.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11580 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/job/job_utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.011902 autosubmit-4.0.82/autosubmit/monitor/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.82/autosubmit/monitor/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10182 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/monitor/diagram.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    26910 2023-07-20 06:53:28.000000 autosubmit-4.0.82/autosubmit/monitor/monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1414 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/monitor/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.011902 autosubmit-4.0.82/autosubmit/notifications/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.82/autosubmit/notifications/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4049 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/notifications/mail_notifier.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1196 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/notifications/notifier.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.011902 autosubmit-4.0.82/autosubmit/platforms/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.82/autosubmit/platforms/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13279 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/ecplatform.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.011902 autosubmit-4.0.82/autosubmit/platforms/headers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.82/autosubmit/platforms/headers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5514 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/headers/ec_cca_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4100 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/headers/ec_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1826 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/headers/local_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7391 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/headers/lsf_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2972 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/headers/pbs10_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3497 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/headers/pbs11_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2963 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/headers/pbs12_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5750 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/headers/pjm_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2214 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/headers/ps_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/headers/sge_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8083 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/headers/slurm_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10469 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/locplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5557 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/lsfplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53819 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/paramiko_platform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11370 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/paramiko_submitter.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5224 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/pbsplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20846 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/pjmplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    27527 2023-07-20 06:53:28.000000 autosubmit-4.0.82/autosubmit/platforms/platform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4184 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/psplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4617 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/sgeplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    32072 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/slurmplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1316 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/submitter.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.015902 autosubmit-4.0.82/autosubmit/platforms/wrappers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.82/autosubmit/platforms/wrappers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    38627 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/wrappers/wrapper_builder.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     9302 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/platforms/wrappers/wrapper_factory.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.015902 autosubmit-4.0.82/autosubmit/statistics/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.82/autosubmit/statistics/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2869 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/statistics/jobs_stat.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6724 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/statistics/statistics.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1818 2023-06-28 10:21:26.000000 autosubmit-4.0.82/autosubmit/statistics/stats_summary.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1830 2023-07-13 10:54:33.000000 autosubmit-4.0.82/autosubmit/statistics/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.007902 autosubmit-4.0.82/autosubmit.egg-info/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3347 2023-07-20 07:03:38.000000 autosubmit-4.0.82/autosubmit.egg-info/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13041 2023-07-20 07:03:38.000000 autosubmit-4.0.82/autosubmit.egg-info/SOURCES.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-07-20 07:03:38.000000 autosubmit-4.0.82/autosubmit.egg-info/dependency_links.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      427 2023-07-20 07:03:38.000000 autosubmit-4.0.82/autosubmit.egg-info/requires.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       20 2023-07-20 07:03:38.000000 autosubmit-4.0.82/autosubmit.egg-info/top_level.txt
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.015902 autosubmit-4.0.82/bin/
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     3086 2023-07-13 10:54:33.000000 autosubmit-4.0.82/bin/autosubmit
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.015902 autosubmit-4.0.82/docs/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7869 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/Makefile
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)  1513786 2021-10-05 14:18:20.000000 autosubmit-4.0.82/docs/autosubmit.pdf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.015902 autosubmit-4.0.82/docs/source/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.015902 autosubmit-4.0.82/docs/source/agui/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.015902 autosubmit-4.0.82/docs/source/agui/experiment/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.015902 autosubmit-4.0.82/docs/source/agui/experiment/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   112356 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/experiment/fig/fig_experiment.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1430 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/agui/experiment/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.015902 autosubmit-4.0.82/docs/source/agui/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25707 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/fig/fig1_gui.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   140255 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/fig/fig2_gui.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   184237 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/fig/fig3_gui.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114416 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/fig/fig4_gui.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    44047 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/fig/fig5_gui.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248267 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/fig/fig_ev_1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248251 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/fig/fig_tree_1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   241752 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/fig/fig_tree_2.png
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.019902 autosubmit-4.0.82/docs/source/agui/graph/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.019902 autosubmit-4.0.82/docs/source/agui/graph/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   122929 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/graph/fig/fig_graph_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   123449 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/graph/fig/fig_graph_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   213843 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/graph/fig/fig_graph_3.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    57438 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/graph/fig/fig_graph_4.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6535 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/agui/graph/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4263 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/agui/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.019902 autosubmit-4.0.82/docs/source/agui/log/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.019902 autosubmit-4.0.82/docs/source/agui/log/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25433 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/log/fig/fig_log_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   117240 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/log/fig/fig_log_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1125 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/log/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.019902 autosubmit-4.0.82/docs/source/agui/performance/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.019902 autosubmit-4.0.82/docs/source/agui/performance/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   174233 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/performance/fig/fig_performance_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      910 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/performance/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.019902 autosubmit-4.0.82/docs/source/agui/statistics/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.019902 autosubmit-4.0.82/docs/source/agui/statistics/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    56486 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/statistics/fig/fig_stat_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   101911 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/statistics/fig/fig_stat_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      988 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/statistics/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.019902 autosubmit-4.0.82/docs/source/agui/tree/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.019902 autosubmit-4.0.82/docs/source/agui/tree/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114354 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/agui/tree/fig/fig_tree_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5756 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/agui/tree/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10217 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/conf.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.019902 autosubmit-4.0.82/docs/source/devguide/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2109 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/devguide/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2145 2023-07-20 07:01:43.000000 autosubmit-4.0.82/docs/source/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.019902 autosubmit-4.0.82/docs/source/installation/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12768 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/installation/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.023902 autosubmit-4.0.82/docs/source/introduction/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   769052 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/introduction/fig1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    93570 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/introduction/fig2.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53843 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/introduction/fig3.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6099 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/introduction/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.023902 autosubmit-4.0.82/docs/source/moduledoc/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      130 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/moduledoc/autosubmit.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      445 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/moduledoc/config.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       99 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/moduledoc/database.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       89 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/moduledoc/git.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      128 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/moduledoc/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/moduledoc/job.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       94 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/moduledoc/monitor.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      547 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/moduledoc/platforms.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.023902 autosubmit-4.0.82/docs/source/qstartguide/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    50473 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/qstartguide/dummy.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     9400 2023-07-20 07:01:43.000000 autosubmit-4.0.82/docs/source/qstartguide/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.023902 autosubmit-4.0.82/docs/source/troubleshooting/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18379 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/troubleshooting/changelog.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    22857 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/troubleshooting/error-codes.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.023902 autosubmit-4.0.82/docs/source/troubleshooting/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    83094 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/troubleshooting/fig/monarch-da.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/troubleshooting/fig/new_dependencies_0.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/troubleshooting/fig/new_dependencies_1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2770 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/troubleshooting/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.023902 autosubmit-4.0.82/docs/source/unused_figs/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    49607 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/unused_figs/group_chunk.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    32622 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/unused_figs/horizontal-vertical.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   106298 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/unused_figs/wrapper.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   251472 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/unused_figs/wrapper_expression.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19009 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/unused_figs/wrapper_hybrid.png
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.023902 autosubmit-4.0.82/docs/source/userguide/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.023902 autosubmit-4.0.82/docs/source/userguide/configure/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    30910 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/userguide/configure/develop_a_project.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20564 2023-07-20 07:01:43.000000 autosubmit-4.0.82/docs/source/userguide/configure/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.023902 autosubmit-4.0.82/docs/source/userguide/create/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6907 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/userguide/create/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1877 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/userguide/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.023902 autosubmit-4.0.82/docs/source/userguide/manage/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    14283 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/userguide/manage/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.023902 autosubmit-4.0.82/docs/source/userguide/run/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    16002 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/userguide/run/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.023902 autosubmit-4.0.82/docs/source/userguide/wrappers/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/docs/source/userguide/wrappers/fig/
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)   198622 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/userguide/wrappers/fig/dasim.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    23826 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/userguide/wrappers/fig/horizontal_remote.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   308786 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/userguide/wrappers/fig/multiple_wrappers.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    17531 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/userguide/wrappers/fig/rerun.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    33805 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/userguide/wrappers/fig/vertical-horizontal.png
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)    33140 2023-06-28 10:21:26.000000 autosubmit-4.0.82/docs/source/userguide/wrappers/fig/vertical-mixed.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11646 2023-07-13 10:54:33.000000 autosubmit-4.0.82/docs/source/userguide/wrappers/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      702 2023-07-13 10:54:33.000000 autosubmit-4.0.82/environment.yml
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/log/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.82/log/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2023-07-13 10:54:33.000000 autosubmit-4.0.82/log/fd_show.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13696 2023-07-13 10:54:33.000000 autosubmit-4.0.82/log/log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      464 2023-07-20 07:01:43.000000 autosubmit-4.0.82/requeriments.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-07-20 07:03:39.035902 autosubmit-4.0.82/setup.cfg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3061 2023-07-13 10:54:33.000000 autosubmit-4.0.82/setup.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/test/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/test/integration/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/integration/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1315 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/integration/test_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2874 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/integration/test_job.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/test/regression/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       33 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/.gitignore
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2429 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/README
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/test/regression/db/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       90 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/db/.gitignore
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/test/regression/default_conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1368 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/default_conf/platforms.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2946 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/local_asparser_test.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.003902 autosubmit-4.0.82/test/regression/test_ecmwf_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/test/regression/test_ecmwf_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2459 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      577 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_ecmwf_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/test/regression/test_ecmwf_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       97 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_ecmwf_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.003902 autosubmit-4.0.82/test/regression/test_large_experiment_on_moore_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/test/regression/test_large_experiment_on_moore_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_large_experiment_on_moore_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_large_experiment_on_moore_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/test/regression/test_large_experiment_on_moore_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_large_experiment_on_moore_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.003902 autosubmit-4.0.82/test/regression/test_mistral_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/test/regression/test_mistral_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/test_mistral_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mistral_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mistral_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/test/regression/test_mistral_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mistral_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.003902 autosubmit-4.0.82/test/regression/test_mn3_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/test/regression/test_mn3_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/test_mn3_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn3_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn3_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/test/regression/test_mn3_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn3_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.003902 autosubmit-4.0.82/test/regression/test_mn3_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/test/regression/test_mn3_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn3_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn3_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/test/regression/test_mn3_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/test_mn3_with_paramiko_python/src/TEST_NOLEAP.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.003902 autosubmit-4.0.82/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.003902 autosubmit-4.0.82/test/regression/test_mn4_horizontal_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      647 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.027902 autosubmit-4.0.82/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.007902 autosubmit-4.0.82/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.031902 autosubmit-4.0.82/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.031902 autosubmit-4.0.82/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.007902 autosubmit-4.0.82/test/regression/test_mn4_vertical_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.031902 autosubmit-4.0.82/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      640 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      208 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.031902 autosubmit-4.0.82/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.007902 autosubmit-4.0.82/test/regression/test_mn4_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.031902 autosubmit-4.0.82/test/regression/test_mn4_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      586 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/test_mn4_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.031902 autosubmit-4.0.82/test/regression/test_mn4_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.007902 autosubmit-4.0.82/test/regression/test_mn4_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.031902 autosubmit-4.0.82/test/regression/test_mn4_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_mn4_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.031902 autosubmit-4.0.82/test/regression/test_mn4_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/test_mn4_with_paramiko_python/src/TEST_NOLEAP.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.007902 autosubmit-4.0.82/test/regression/test_moore_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.031902 autosubmit-4.0.82/test/regression/test_moore_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_moore_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2455 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/test_moore_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      352 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_moore_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_moore_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.031902 autosubmit-4.0.82/test/regression/test_moore_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_moore_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.007902 autosubmit-4.0.82/test/regression/test_moore_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.031902 autosubmit-4.0.82/test/regression/test_moore_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/test_moore_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_moore_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_moore_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.031902 autosubmit-4.0.82/test/regression/test_moore_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/test_moore_with_paramiko_python/src/TEST_NOLEAP.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.007902 autosubmit-4.0.82/test/regression/test_sedema_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.031902 autosubmit-4.0.82/test/regression/test_sedema_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/test_sedema_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_sedema_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_sedema_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.031902 autosubmit-4.0.82/test/regression/test_sedema_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_sedema_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.007902 autosubmit-4.0.82/test/regression/test_sedema_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.031902 autosubmit-4.0.82/test/regression/test_sedema_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2458 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_sedema_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/test_sedema_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.031902 autosubmit-4.0.82/test/regression/test_sedema_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/test_sedema_with_paramiko_python/src/TEST_NOLEAP.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2775 2022-11-21 08:34:36.000000 autosubmit-4.0.82/test/regression/tests.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1135 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/regression/tests_commands.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5968 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/tests_log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5504 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/tests_runner.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/regression/tests_utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-20 07:03:39.035902 autosubmit-4.0.82/test/unit/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2039 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/README_PIP.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-12-20 13:25:07.000000 autosubmit-4.0.82/test/unit/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1104 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_basic_config.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4581 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_catlog.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13253 2021-10-05 14:18:20.000000 autosubmit-4.0.82/test/unit/test_chunk_date_lib.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13319 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_database_managers.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2490 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     9696 2023-07-20 06:53:28.000000 autosubmit-4.0.82/test/unit/test_dependencies.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    22969 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_dic_jobs.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8327 2023-07-20 07:01:43.000000 autosubmit-4.0.82/test/unit/test_expid.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19073 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_history.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    14748 2023-07-20 06:53:28.000000 autosubmit-4.0.82/test/unit/test_job.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1015 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_job_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    47843 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_job_graph.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    59633 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_job_grouping.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12769 2023-07-20 06:53:28.000000 autosubmit-4.0.82/test/unit/test_job_list.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8531 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_job_package.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      815 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3772 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_machinefiles_wrapper.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4878 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_paramiko_platform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5244 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_pjm.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4528 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_platform_monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      393 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_setup.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2887 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_slurm_platform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3130 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_statistics.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6724 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_strategies.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    81739 2023-07-13 10:54:33.000000 autosubmit-4.0.82/test/unit/test_wrappers.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.543668 autosubmit-4.0.84/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      226 2023-07-13 10:54:33.000000 autosubmit-4.0.84/.gitignore
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1361 2023-07-13 10:54:33.000000 autosubmit-4.0.84/.gitlab-ci.yml
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      937 2023-07-13 10:54:33.000000 autosubmit-4.0.84/.readthedocs.yaml
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.84/CHANGELOG
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      722 2023-07-13 10:54:33.000000 autosubmit-4.0.84/CONTRIBUTING.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    35147 2021-10-05 14:18:20.000000 autosubmit-4.0.84/LICENSE
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      119 2021-10-05 14:18:20.000000 autosubmit-4.0.84/MANIFEST.in
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3347 2023-07-21 08:56:31.539668 autosubmit-4.0.84/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5651 2023-07-13 10:54:33.000000 autosubmit-4.0.84/README.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2287 2023-07-13 10:54:33.000000 autosubmit-4.0.84/README_PIP.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        7 2023-07-21 08:56:14.000000 autosubmit-4.0.84/VERSION
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.503669 autosubmit-4.0.84/autosubmit/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   324689 2023-07-20 14:05:47.000000 autosubmit-4.0.84/autosubmit/autosubmit.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.503669 autosubmit-4.0.84/autosubmit/database/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/database/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.503669 autosubmit-4.0.84/autosubmit/database/data/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      258 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/database/data/autosubmit.sql
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19910 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/database/db_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7593 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/database/db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6065 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/database/db_structure.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.503669 autosubmit-4.0.84/autosubmit/experiment/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/experiment/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5280 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/experiment/experiment_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8450 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/experiment/statistics.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.503669 autosubmit-4.0.84/autosubmit/git/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/git/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13703 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/git/autosubmit_git.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.503669 autosubmit-4.0.84/autosubmit/helpers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.84/autosubmit/helpers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5776 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/helpers/autosubmit_helper.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      194 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/helpers/data_transfer.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3304 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/helpers/parameters.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1428 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/helpers/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.507669 autosubmit-4.0.84/autosubmit/history/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.84/autosubmit/history/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.507669 autosubmit-4.0.84/autosubmit/history/data_classes/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.84/autosubmit/history/data_classes/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2432 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/data_classes/experiment_run.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10305 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/data_classes/job_data.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.507669 autosubmit-4.0.84/autosubmit/history/database_managers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.84/autosubmit/history/database_managers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5688 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/database_managers/database_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2409 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/database_managers/database_models.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19251 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/database_managers/experiment_history_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6456 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/database_managers/experiment_status_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18844 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/experiment_history.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2382 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/experiment_status.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1952 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/internal_logging.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.507669 autosubmit-4.0.84/autosubmit/history/platform_monitor/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.507669 autosubmit-4.0.84/autosubmit/history/platform_monitor/output_examples/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/output_examples/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2022-11-21 08:34:36.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/output_examples/pending.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      554 2022-11-21 08:34:36.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/output_examples/wrapper1.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      549 2022-11-21 08:34:36.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/output_examples/wrapper2.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6105 2022-11-21 08:34:36.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1025 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/platform_monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2298 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/platform_utils.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2475 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/slurm_monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3454 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/slurm_monitor_item.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10951 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/strategies.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2784 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.507669 autosubmit-4.0.84/autosubmit/job/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/job/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    99727 2023-07-20 07:01:43.000000 autosubmit-4.0.84/autosubmit/job/job.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10907 2023-07-20 06:53:28.000000 autosubmit-4.0.84/autosubmit/job/job_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20136 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/job/job_dict.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13797 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/job/job_grouping.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   127858 2023-07-20 06:53:28.000000 autosubmit-4.0.84/autosubmit/job/job_list.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4609 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/job/job_list_persistence.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3565 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/job/job_package_persistence.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    62148 2023-07-20 06:53:28.000000 autosubmit-4.0.84/autosubmit/job/job_packager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    38254 2023-07-21 08:35:09.000000 autosubmit-4.0.84/autosubmit/job/job_packages.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11580 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/job/job_utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.507669 autosubmit-4.0.84/autosubmit/monitor/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/monitor/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10182 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/monitor/diagram.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    26910 2023-07-20 06:53:28.000000 autosubmit-4.0.84/autosubmit/monitor/monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1414 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/monitor/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.507669 autosubmit-4.0.84/autosubmit/notifications/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/notifications/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4049 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/notifications/mail_notifier.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1196 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/notifications/notifier.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.511669 autosubmit-4.0.84/autosubmit/platforms/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/platforms/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13279 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/ecplatform.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.511669 autosubmit-4.0.84/autosubmit/platforms/headers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/platforms/headers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5514 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/ec_cca_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4100 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/ec_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1826 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/local_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7391 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/lsf_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2972 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/pbs10_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3497 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/pbs11_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2963 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/pbs12_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5750 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/pjm_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2214 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/ps_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/sge_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8083 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/slurm_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10469 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/locplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5557 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/lsfplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53819 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/paramiko_platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11370 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/paramiko_submitter.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5224 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/pbsplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20846 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/pjmplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    27527 2023-07-20 06:53:28.000000 autosubmit-4.0.84/autosubmit/platforms/platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4184 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/psplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4617 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/sgeplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    32072 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/slurmplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1316 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/submitter.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.511669 autosubmit-4.0.84/autosubmit/platforms/wrappers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/platforms/wrappers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    38702 2023-07-21 08:11:30.000000 autosubmit-4.0.84/autosubmit/platforms/wrappers/wrapper_builder.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     9418 2023-07-21 08:13:50.000000 autosubmit-4.0.84/autosubmit/platforms/wrappers/wrapper_factory.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.511669 autosubmit-4.0.84/autosubmit/statistics/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.84/autosubmit/statistics/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2869 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/statistics/jobs_stat.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6724 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/statistics/statistics.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1818 2023-06-28 10:21:26.000000 autosubmit-4.0.84/autosubmit/statistics/stats_summary.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1830 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/statistics/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.503669 autosubmit-4.0.84/autosubmit.egg-info/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3347 2023-07-21 08:56:31.000000 autosubmit-4.0.84/autosubmit.egg-info/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13041 2023-07-21 08:56:31.000000 autosubmit-4.0.84/autosubmit.egg-info/SOURCES.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-07-21 08:56:31.000000 autosubmit-4.0.84/autosubmit.egg-info/dependency_links.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      427 2023-07-21 08:56:31.000000 autosubmit-4.0.84/autosubmit.egg-info/requires.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       20 2023-07-21 08:56:31.000000 autosubmit-4.0.84/autosubmit.egg-info/top_level.txt
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.511669 autosubmit-4.0.84/bin/
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     3086 2023-07-13 10:54:33.000000 autosubmit-4.0.84/bin/autosubmit
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.511669 autosubmit-4.0.84/docs/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7869 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/Makefile
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)  1513786 2021-10-05 14:18:20.000000 autosubmit-4.0.84/docs/autosubmit.pdf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.515669 autosubmit-4.0.84/docs/source/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.515669 autosubmit-4.0.84/docs/source/agui/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.515669 autosubmit-4.0.84/docs/source/agui/experiment/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.515669 autosubmit-4.0.84/docs/source/agui/experiment/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   112356 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/experiment/fig/fig_experiment.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1430 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/agui/experiment/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.519669 autosubmit-4.0.84/docs/source/agui/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25707 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/fig/fig1_gui.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   140255 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/fig/fig2_gui.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   184237 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/fig/fig3_gui.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114416 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/fig/fig4_gui.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    44047 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/fig/fig5_gui.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248267 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/fig/fig_ev_1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248251 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/fig/fig_tree_1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   241752 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/fig/fig_tree_2.png
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.519669 autosubmit-4.0.84/docs/source/agui/graph/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.519669 autosubmit-4.0.84/docs/source/agui/graph/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   122929 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/graph/fig/fig_graph_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   123449 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/graph/fig/fig_graph_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   213843 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/graph/fig/fig_graph_3.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    57438 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/graph/fig/fig_graph_4.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6535 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/agui/graph/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4263 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/agui/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.519669 autosubmit-4.0.84/docs/source/agui/log/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.519669 autosubmit-4.0.84/docs/source/agui/log/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25433 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/log/fig/fig_log_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   117240 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/log/fig/fig_log_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1125 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/log/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.519669 autosubmit-4.0.84/docs/source/agui/performance/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.519669 autosubmit-4.0.84/docs/source/agui/performance/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   174233 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/performance/fig/fig_performance_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      910 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/performance/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.523669 autosubmit-4.0.84/docs/source/agui/statistics/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.523669 autosubmit-4.0.84/docs/source/agui/statistics/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    56486 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/statistics/fig/fig_stat_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   101911 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/statistics/fig/fig_stat_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      988 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/statistics/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.523669 autosubmit-4.0.84/docs/source/agui/tree/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.523669 autosubmit-4.0.84/docs/source/agui/tree/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114354 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/tree/fig/fig_tree_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5756 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/agui/tree/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10217 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/conf.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.523669 autosubmit-4.0.84/docs/source/devguide/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2109 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/devguide/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2145 2023-07-20 07:01:43.000000 autosubmit-4.0.84/docs/source/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.523669 autosubmit-4.0.84/docs/source/installation/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12768 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/installation/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.523669 autosubmit-4.0.84/docs/source/introduction/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   769052 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/introduction/fig1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    93570 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/introduction/fig2.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53843 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/introduction/fig3.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6099 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/introduction/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.527669 autosubmit-4.0.84/docs/source/moduledoc/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      130 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/moduledoc/autosubmit.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      445 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/moduledoc/config.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       99 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/moduledoc/database.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       89 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/moduledoc/git.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      128 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/moduledoc/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/moduledoc/job.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       94 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/moduledoc/monitor.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      547 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/moduledoc/platforms.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.527669 autosubmit-4.0.84/docs/source/qstartguide/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    50473 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/qstartguide/dummy.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     9400 2023-07-20 07:01:43.000000 autosubmit-4.0.84/docs/source/qstartguide/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.527669 autosubmit-4.0.84/docs/source/troubleshooting/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18379 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/troubleshooting/changelog.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    22857 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/troubleshooting/error-codes.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.527669 autosubmit-4.0.84/docs/source/troubleshooting/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    83094 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/troubleshooting/fig/monarch-da.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/troubleshooting/fig/new_dependencies_0.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/troubleshooting/fig/new_dependencies_1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2770 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/troubleshooting/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.527669 autosubmit-4.0.84/docs/source/unused_figs/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    49607 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/unused_figs/group_chunk.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    32622 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/unused_figs/horizontal-vertical.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   106298 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/unused_figs/wrapper.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   251472 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/unused_figs/wrapper_expression.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19009 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/unused_figs/wrapper_hybrid.png
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/docs/source/userguide/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/docs/source/userguide/configure/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    30910 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/userguide/configure/develop_a_project.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20564 2023-07-20 07:01:43.000000 autosubmit-4.0.84/docs/source/userguide/configure/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/docs/source/userguide/create/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6907 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/userguide/create/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1877 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/userguide/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/docs/source/userguide/manage/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    14283 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/userguide/manage/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/docs/source/userguide/run/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    16002 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/userguide/run/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/docs/source/userguide/wrappers/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/docs/source/userguide/wrappers/fig/
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)   198622 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/userguide/wrappers/fig/dasim.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    23826 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/userguide/wrappers/fig/horizontal_remote.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   308786 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/userguide/wrappers/fig/multiple_wrappers.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    17531 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/userguide/wrappers/fig/rerun.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    33805 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/userguide/wrappers/fig/vertical-horizontal.png
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)    33140 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/userguide/wrappers/fig/vertical-mixed.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11646 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/userguide/wrappers/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      702 2023-07-13 10:54:33.000000 autosubmit-4.0.84/environment.yml
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/log/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.84/log/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2023-07-13 10:54:33.000000 autosubmit-4.0.84/log/fd_show.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13696 2023-07-13 10:54:33.000000 autosubmit-4.0.84/log/log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      464 2023-07-20 07:01:43.000000 autosubmit-4.0.84/requeriments.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-07-21 08:56:31.543668 autosubmit-4.0.84/setup.cfg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3061 2023-07-13 10:54:33.000000 autosubmit-4.0.84/setup.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/test/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/test/integration/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/integration/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1315 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/integration/test_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2874 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/integration/test_job.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       33 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/.gitignore
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2429 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/README
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/db/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       90 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/db/.gitignore
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/default_conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1368 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/default_conf/platforms.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2946 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/local_asparser_test.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2459 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      577 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       97 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/src/TEST_NOLEAP.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      647 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      640 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      208 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      586 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/src/TEST_NOLEAP.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_moore_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_moore_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2455 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      352 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_moore_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/src/TEST_NOLEAP.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2458 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/src/TEST_NOLEAP.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2775 2022-11-21 08:34:36.000000 autosubmit-4.0.84/test/regression/tests.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1135 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/tests_commands.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5968 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/tests_log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5504 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/tests_runner.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/tests_utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/unit/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2039 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/README_PIP.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-12-20 13:25:07.000000 autosubmit-4.0.84/test/unit/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1104 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_basic_config.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4581 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_catlog.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13253 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/unit/test_chunk_date_lib.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13319 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_database_managers.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2490 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     9696 2023-07-20 06:53:28.000000 autosubmit-4.0.84/test/unit/test_dependencies.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    22969 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_dic_jobs.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8327 2023-07-20 07:01:43.000000 autosubmit-4.0.84/test/unit/test_expid.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19073 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_history.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    14748 2023-07-20 06:53:28.000000 autosubmit-4.0.84/test/unit/test_job.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1015 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_job_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    47843 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_job_graph.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    59633 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_job_grouping.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12769 2023-07-20 06:53:28.000000 autosubmit-4.0.84/test/unit/test_job_list.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8531 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_job_package.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      815 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3846 2023-07-21 08:33:26.000000 autosubmit-4.0.84/test/unit/test_machinefiles_wrapper.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4878 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_paramiko_platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5244 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_pjm.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4528 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_platform_monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      393 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_setup.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2887 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_slurm_platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3130 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_statistics.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6724 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_strategies.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    81739 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_wrappers.py
```

### Comparing `autosubmit-4.0.82/.gitlab-ci.yml` & `autosubmit-4.0.84/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/.readthedocs.yaml` & `autosubmit-4.0.84/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/CONTRIBUTING.md` & `autosubmit-4.0.84/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/LICENSE` & `autosubmit-4.0.84/LICENSE`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/PKG-INFO` & `autosubmit-4.0.84/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmit
-Version: 4.0.82
+Version: 4.0.84
 Summary: Autosubmit is a Python-based workflow manager to create, manage and monitor complex tasks involving different substeps, such as scientific computational experiments. These workflows may involve multiple computing systems for their completion, from HPCs to post-processing clusters or workstations. Autosubmit can orchestrate all the tasks integrating the workflow by managing their dependencies, interfacing with all the platforms involved, and handling eventual errors.
 Home-page: http://www.bsc.es/projects/earthscience/autosubmit/
 Download-URL: https://earth.bsc.es/wiki/doku.php?id=tools:autosubmit
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 License: GNU GPL v3
 Keywords: climate,weather,workflow,HPC
```

### Comparing `autosubmit-4.0.82/README.md` & `autosubmit-4.0.84/README.md`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/README_PIP.md` & `autosubmit-4.0.84/README_PIP.md`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/autosubmit.py` & `autosubmit-4.0.84/autosubmit/autosubmit.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/database/db_common.py` & `autosubmit-4.0.84/autosubmit/database/db_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/database/db_manager.py` & `autosubmit-4.0.84/autosubmit/database/db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/database/db_structure.py` & `autosubmit-4.0.84/autosubmit/database/db_structure.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/experiment/experiment_common.py` & `autosubmit-4.0.84/autosubmit/experiment/experiment_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/experiment/statistics.py` & `autosubmit-4.0.84/autosubmit/experiment/statistics.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/git/autosubmit_git.py` & `autosubmit-4.0.84/autosubmit/git/autosubmit_git.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/helpers/autosubmit_helper.py` & `autosubmit-4.0.84/autosubmit/helpers/autosubmit_helper.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/helpers/parameters.py` & `autosubmit-4.0.84/autosubmit/helpers/parameters.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/helpers/utils.py` & `autosubmit-4.0.84/autosubmit/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/history/data_classes/experiment_run.py` & `autosubmit-4.0.84/autosubmit/history/data_classes/experiment_run.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/history/data_classes/job_data.py` & `autosubmit-4.0.84/autosubmit/history/data_classes/job_data.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/history/database_managers/database_manager.py` & `autosubmit-4.0.84/autosubmit/history/database_managers/database_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/history/database_managers/database_models.py` & `autosubmit-4.0.84/autosubmit/history/database_managers/database_models.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/history/database_managers/experiment_history_db_manager.py` & `autosubmit-4.0.84/autosubmit/history/database_managers/experiment_history_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/history/database_managers/experiment_status_db_manager.py` & `autosubmit-4.0.84/autosubmit/history/database_managers/experiment_status_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/history/experiment_history.py` & `autosubmit-4.0.84/autosubmit/history/experiment_history.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/history/experiment_status.py` & `autosubmit-4.0.84/autosubmit/history/experiment_status.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/history/internal_logging.py` & `autosubmit-4.0.84/autosubmit/history/internal_logging.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/history/platform_monitor/output_examples/wrapper1.txt` & `autosubmit-4.0.84/autosubmit/history/platform_monitor/output_examples/wrapper1.txt`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/history/platform_monitor/output_examples/wrapper2.txt` & `autosubmit-4.0.84/autosubmit/history/platform_monitor/output_examples/wrapper2.txt`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt` & `autosubmit-4.0.84/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/history/platform_monitor/platform_monitor.py` & `autosubmit-4.0.84/autosubmit/history/platform_monitor/platform_monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/history/platform_monitor/platform_utils.py` & `autosubmit-4.0.84/autosubmit/history/platform_monitor/platform_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/history/platform_monitor/slurm_monitor.py` & `autosubmit-4.0.84/autosubmit/history/platform_monitor/slurm_monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/history/platform_monitor/slurm_monitor_item.py` & `autosubmit-4.0.84/autosubmit/history/platform_monitor/slurm_monitor_item.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/history/strategies.py` & `autosubmit-4.0.84/autosubmit/history/strategies.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/history/utils.py` & `autosubmit-4.0.84/autosubmit/history/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/job/job.py` & `autosubmit-4.0.84/autosubmit/job/job.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/job/job_common.py` & `autosubmit-4.0.84/autosubmit/job/job_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/job/job_dict.py` & `autosubmit-4.0.84/autosubmit/job/job_dict.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/job/job_grouping.py` & `autosubmit-4.0.84/autosubmit/job/job_grouping.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/job/job_list.py` & `autosubmit-4.0.84/autosubmit/job/job_list.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/job/job_list_persistence.py` & `autosubmit-4.0.84/autosubmit/job/job_list_persistence.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/job/job_package_persistence.py` & `autosubmit-4.0.84/autosubmit/job/job_package_persistence.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/job/job_packager.py` & `autosubmit-4.0.84/autosubmit/job/job_packager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/job/job_packages.py` & `autosubmit-4.0.84/autosubmit/job/job_packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 
 # You should have received a copy of the GNU General Public License
 # along with Autosubmit.  If not, see <http://www.gnu.org/licenses/>.
 
 
 
 import os
+import random
+import time
 from datetime import timedelta
 
-import time
-import random
 from autosubmit.job.job_common import Status
-from log.log import Log,AutosubmitCritical,AutosubmitError
+from log.log import Log, AutosubmitCritical
+
 Log.get_logger("Autosubmit")
 from autosubmit.job.job import Job
 from bscearth.utils.date import sum_str_hours
 from threading import Thread, Lock
 from typing import List
 import multiprocessing
 import tarfile
@@ -721,15 +722,15 @@
             wallclock_by_level = None
 
         return self._wrapper_factory.get_wrapper(self._wrapper_factory.vertical_wrapper, name=self._name,
                                                  queue=self._queue, project=self._project, wallclock=self._wallclock,
                                                  num_processors=self._num_processors, jobs_scripts=self._jobs_scripts,
                                                  dependency=self._job_dependency, jobs_resources=self._jobs_resources,
                                                  expid=self._expid, rootdir=self.platform.root_dir,
-                                                 directives=self._custom_directives,threads=self._threads,method=self.method.lower(),retrials=self.inner_retrials, wallclock_by_level=wallclock_by_level,partition=self.partition,wrapper_data=self._wrapper_data)
+                                                 directives=self._custom_directives,threads=self._threads,method=self.method.lower(),retrials=self.inner_retrials, wallclock_by_level=wallclock_by_level,partition=self.partition,wrapper_data=self._wrapper_data,num_processors_value=self._num_processors)
 
 
 class JobPackageHorizontal(JobPackageThread):
     """
     Class to manage a horizontal thread-based package of jobs to be submitted by autosubmit
     """
 
@@ -751,15 +752,15 @@
 
     def _common_script_content(self):
         return self._wrapper_factory.get_wrapper(self._wrapper_factory.horizontal_wrapper, name=self._name,
                                                  queue=self._queue, project=self._project, wallclock=self._wallclock,
                                                  num_processors=self._num_processors, jobs_scripts=self._jobs_scripts,
                                                  dependency=self._job_dependency, jobs_resources=self._jobs_resources,
                                                  expid=self._expid, rootdir=self.platform.root_dir,
-                                                 directives=self._custom_directives,threads=self._threads,method=self.method.lower(),partition=self.partition,wrapper_data=self._wrapper_data)
+                                                 directives=self._custom_directives,threads=self._threads,method=self.method.lower(),partition=self.partition,wrapper_data=self._wrapper_data,num_processors_value=self._num_processors)
 
 class JobPackageHybrid(JobPackageThread):
     """
         Class to manage a hybrid (horizontal and vertical) thread-based package of jobs to be submitted by autosubmit
         """
 
     def __init__(self, jobs, num_processors, total_wallclock, dependency=None, jobs_resources=dict(),method="ASThread",configuration=None,wrapper_section="WRAPPERS"):
@@ -796,20 +797,20 @@
 
     def _common_script_content(self):
         return self._wrapper_factory.get_wrapper(self._wrapper_factory.hybrid_wrapper_vertical_horizontal,
                                                  name=self._name, queue=self._queue, project=self._project,
                                                  wallclock=self._wallclock, num_processors=self._num_processors,
                                                  jobs_scripts=self._jobs_scripts, dependency=self._job_dependency,
                                                  jobs_resources=self._jobs_resources, expid=self._expid,
-                                                 rootdir=self.platform.root_dir, directives=self._custom_directives,threads=self._threads,method=self.method.lower(),partition=self.partition,wrapper_data=self._wrapper_data)
+                                                 rootdir=self.platform.root_dir, directives=self._custom_directives,threads=self._threads,method=self.method.lower(),partition=self.partition,wrapper_data=self._wrapper_data,num_processors_value=self._num_processors)
 
 
 class JobPackageHorizontalVertical(JobPackageHybrid):
 
     def _common_script_content(self):
         return self._wrapper_factory.get_wrapper(self._wrapper_factory.hybrid_wrapper_horizontal_vertical,
                                                  name=self._name, queue=self._queue, project=self._project,
                                                  wallclock=self._wallclock, num_processors=self._num_processors,
                                                  jobs_scripts=self._jobs_scripts, dependency=self._job_dependency,
                                                  jobs_resources=self._jobs_resources, expid=self._expid,
-                                                 rootdir=self.platform.root_dir, directives=self._custom_directives,threads=self._threads,method=self.method.lower(),partition=self.partition,wrapper_data=self._wrapper_data)
+                                                 rootdir=self.platform.root_dir, directives=self._custom_directives,threads=self._threads,method=self.method.lower(),partition=self.partition,wrapper_data=self._wrapper_data,num_processors_value=self._num_processors)
```

### Comparing `autosubmit-4.0.82/autosubmit/job/job_utils.py` & `autosubmit-4.0.84/autosubmit/job/job_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/monitor/diagram.py` & `autosubmit-4.0.84/autosubmit/monitor/diagram.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/monitor/monitor.py` & `autosubmit-4.0.84/autosubmit/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/monitor/utils.py` & `autosubmit-4.0.84/autosubmit/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/notifications/mail_notifier.py` & `autosubmit-4.0.84/autosubmit/notifications/mail_notifier.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/notifications/notifier.py` & `autosubmit-4.0.84/autosubmit/notifications/notifier.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/ecplatform.py` & `autosubmit-4.0.84/autosubmit/platforms/ecplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/headers/ec_cca_header.py` & `autosubmit-4.0.84/autosubmit/platforms/headers/ec_cca_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/headers/ec_header.py` & `autosubmit-4.0.84/autosubmit/platforms/headers/ec_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/headers/local_header.py` & `autosubmit-4.0.84/autosubmit/platforms/headers/local_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/headers/lsf_header.py` & `autosubmit-4.0.84/autosubmit/platforms/headers/lsf_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/headers/pbs10_header.py` & `autosubmit-4.0.84/autosubmit/platforms/headers/pbs10_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/headers/pbs11_header.py` & `autosubmit-4.0.84/autosubmit/platforms/headers/pbs11_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/headers/pbs12_header.py` & `autosubmit-4.0.84/autosubmit/platforms/headers/pbs12_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/headers/pjm_header.py` & `autosubmit-4.0.84/autosubmit/platforms/headers/pjm_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/headers/ps_header.py` & `autosubmit-4.0.84/autosubmit/platforms/headers/ps_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/headers/sge_header.py` & `autosubmit-4.0.84/autosubmit/platforms/headers/sge_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/headers/slurm_header.py` & `autosubmit-4.0.84/autosubmit/platforms/headers/slurm_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/locplatform.py` & `autosubmit-4.0.84/autosubmit/platforms/locplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/lsfplatform.py` & `autosubmit-4.0.84/autosubmit/platforms/lsfplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/paramiko_platform.py` & `autosubmit-4.0.84/autosubmit/platforms/paramiko_platform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/paramiko_submitter.py` & `autosubmit-4.0.84/autosubmit/platforms/paramiko_submitter.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/pbsplatform.py` & `autosubmit-4.0.84/autosubmit/platforms/pbsplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/pjmplatform.py` & `autosubmit-4.0.84/autosubmit/platforms/pjmplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/platform.py` & `autosubmit-4.0.84/autosubmit/platforms/platform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/psplatform.py` & `autosubmit-4.0.84/autosubmit/platforms/psplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/sgeplatform.py` & `autosubmit-4.0.84/autosubmit/platforms/sgeplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/slurmplatform.py` & `autosubmit-4.0.84/autosubmit/platforms/slurmplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/submitter.py` & `autosubmit-4.0.84/autosubmit/platforms/submitter.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/platforms/wrappers/wrapper_builder.py` & `autosubmit-4.0.84/autosubmit/platforms/wrappers/wrapper_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with Autosubmit.  If not, see <http://www.gnu.org/licenses/>.
 
-import textwrap
 import random
 import string
+import textwrap
+
 
 class WrapperDirector:
     """
     Construct an object using the Builder interface.
     """
     def __init__(self):
         self._builder = None
@@ -46,14 +47,15 @@
     def __init__(self, **kwargs):
         if "retrials" in list(kwargs.keys()):
             self.retrials = kwargs['retrials']
         self.header_directive = kwargs['header_directive']
         self.job_scripts = kwargs['jobs_scripts']
         self.threads = kwargs['threads']
         self.num_procs = kwargs['num_processors']
+        self.num_procs_value = kwargs['num_processors_value']
         self.expid = kwargs['expid']
         self.jobs_resources = kwargs.get('jobs_resources', dict())
         self.allocated_nodes = kwargs.get('allocated_nodes', '')
         self.machinefiles_name = ''
         self.machinefiles_indent = 0
         self.exit_thread = ''
         if "wallclock_by_level" in list(kwargs.keys()):
@@ -198,15 +200,15 @@
         all_cores.append(all_nodes[idx])
     else:
         if idx < len(all_nodes)-1:
             idx += 1
         processors_per_node = int(jobs_resources['PROCESSORS_PER_NODE'])
 processors_per_node = int(jobs_resources['PROCESSORS_PER_NODE'])
 
-        """).format(self.num_procs, str(self.jobs_resources), '\n'.ljust(13))
+        """).format(self.num_procs_value, str(self.jobs_resources), '\n'.ljust(13))
 
     def build_machinefiles(self):
         machinefile_function = self.get_machinefile_function()
         if machinefile_function:
             return self.get_machinefile_function() + self._indent(self.write_machinefiles(), self.machinefiles_indent)
         return ""
 
@@ -716,15 +718,15 @@
         all_cores.append(all_nodes[idx])
     else:
         if idx < len(all_nodes)-1:
             idx += 1
         processors_per_node = int(jobs_resources['PROCESSORS_PER_NODE'])
 
 processors_per_node = int(jobs_resources['PROCESSORS_PER_NODE'])
-        """).format(self.num_procs, str(self.jobs_resources), '\n'.ljust(13))
+        """).format(self.num_procs_value, str(self.jobs_resources), '\n'.ljust(13))
 
     def build_machinefiles(self):
         machinefile_function = self.get_machinefile_function()
         if machinefile_function:
             return self.get_machinefile_function() + self._indent(self.write_machinefiles(), self.machinefiles_indent)
         return ""
```

### Comparing `autosubmit-4.0.82/autosubmit/platforms/wrappers/wrapper_factory.py` & `autosubmit-4.0.84/autosubmit/platforms/wrappers/wrapper_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 # You should have received a copy of the GNU General Public License
 # along with Autosubmit.  If not, see <http://www.gnu.org/licenses/>.
 
 from autosubmit.platforms.wrappers.wrapper_builder import WrapperDirector, PythonVerticalWrapperBuilder, \
     PythonHorizontalWrapperBuilder, PythonHorizontalVerticalWrapperBuilder, PythonVerticalHorizontalWrapperBuilder, \
     BashHorizontalWrapperBuilder, BashVerticalWrapperBuilder, SrunHorizontalWrapperBuilder,SrunVerticalHorizontalWrapperBuilder
-from autosubmitconfigparser.config.configcommon import AutosubmitConfig
 
 
 class WrapperFactory(object):
 
     def __init__(self, platform):
         self.as_conf = None
         self.platform = platform
@@ -39,14 +38,18 @@
         kwargs['partition'] = self.partition(wrapper_data['PARTITION'])
         kwargs["exclusive"] = self.exclusive(wrapper_data['EXCLUSIVE'])
         kwargs["custom_directives"] = self.custom_directives(wrapper_data["CUSTOM_DIRECTIVES"])
         kwargs["executable"] = wrapper_data["EXECUTABLE"]
         kwargs['nodes'] = self.nodes(wrapper_data['NODES'])
         kwargs['tasks'] = self.tasks(wrapper_data['TASKS'])
         kwargs['threads'] = self.threads(kwargs['threads'])
+        if str(kwargs['num_processors']).isdigit():
+            kwargs['num_processors_value'] = int(kwargs['num_processors'])
+        else:
+            kwargs['num_processors_value'] = 1
         if str(wrapper_data['NODES']).isdigit() and int(wrapper_data['NODES']) > 1 and kwargs['num_processors'] == '1':
             kwargs['num_processors'] = "#"
         else:
             kwargs['num_processors'] = self.processors(kwargs['num_processors'])
         kwargs['header_directive'] = self.header_directives(**kwargs)
         builder = wrapper_builder(**kwargs)
         return self.wrapper_director.construct(builder)
```

### Comparing `autosubmit-4.0.82/autosubmit/statistics/jobs_stat.py` & `autosubmit-4.0.84/autosubmit/statistics/jobs_stat.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/statistics/statistics.py` & `autosubmit-4.0.84/autosubmit/statistics/statistics.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/statistics/stats_summary.py` & `autosubmit-4.0.84/autosubmit/statistics/stats_summary.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit/statistics/utils.py` & `autosubmit-4.0.84/autosubmit/statistics/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/autosubmit.egg-info/PKG-INFO` & `autosubmit-4.0.84/autosubmit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmit
-Version: 4.0.82
+Version: 4.0.84
 Summary: Autosubmit is a Python-based workflow manager to create, manage and monitor complex tasks involving different substeps, such as scientific computational experiments. These workflows may involve multiple computing systems for their completion, from HPCs to post-processing clusters or workstations. Autosubmit can orchestrate all the tasks integrating the workflow by managing their dependencies, interfacing with all the platforms involved, and handling eventual errors.
 Home-page: http://www.bsc.es/projects/earthscience/autosubmit/
 Download-URL: https://earth.bsc.es/wiki/doku.php?id=tools:autosubmit
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 License: GNU GPL v3
 Keywords: climate,weather,workflow,HPC
```

### Comparing `autosubmit-4.0.82/autosubmit.egg-info/SOURCES.txt` & `autosubmit-4.0.84/autosubmit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/bin/autosubmit` & `autosubmit-4.0.84/bin/autosubmit`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/Makefile` & `autosubmit-4.0.84/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/autosubmit.pdf` & `autosubmit-4.0.84/docs/autosubmit.pdf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/experiment/fig/fig_experiment.jpg` & `autosubmit-4.0.84/docs/source/agui/experiment/fig/fig_experiment.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/experiment/index.rst` & `autosubmit-4.0.84/docs/source/agui/experiment/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/fig/fig1_gui.png` & `autosubmit-4.0.84/docs/source/agui/fig/fig1_gui.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/fig/fig2_gui.png` & `autosubmit-4.0.84/docs/source/agui/fig/fig2_gui.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/fig/fig3_gui.png` & `autosubmit-4.0.84/docs/source/agui/fig/fig3_gui.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/fig/fig4_gui.jpg` & `autosubmit-4.0.84/docs/source/agui/fig/fig4_gui.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/fig/fig5_gui.jpg` & `autosubmit-4.0.84/docs/source/agui/fig/fig5_gui.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/fig/fig_ev_1.png` & `autosubmit-4.0.84/docs/source/agui/fig/fig_ev_1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/fig/fig_tree_1.png` & `autosubmit-4.0.84/docs/source/agui/fig/fig_tree_1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/fig/fig_tree_2.png` & `autosubmit-4.0.84/docs/source/agui/fig/fig_tree_2.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/graph/fig/fig_graph_1.jpg` & `autosubmit-4.0.84/docs/source/agui/graph/fig/fig_graph_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/graph/fig/fig_graph_2.jpg` & `autosubmit-4.0.84/docs/source/agui/graph/fig/fig_graph_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/graph/fig/fig_graph_3.jpg` & `autosubmit-4.0.84/docs/source/agui/graph/fig/fig_graph_3.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/graph/fig/fig_graph_4.jpg` & `autosubmit-4.0.84/docs/source/agui/graph/fig/fig_graph_4.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/graph/index.rst` & `autosubmit-4.0.84/docs/source/agui/graph/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/index.rst` & `autosubmit-4.0.84/docs/source/agui/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/log/fig/fig_log_1.jpg` & `autosubmit-4.0.84/docs/source/agui/log/fig/fig_log_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/log/fig/fig_log_2.jpg` & `autosubmit-4.0.84/docs/source/agui/log/fig/fig_log_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/log/index.rst` & `autosubmit-4.0.84/docs/source/agui/log/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/performance/fig/fig_performance_1.jpg` & `autosubmit-4.0.84/docs/source/agui/performance/fig/fig_performance_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/performance/index.rst` & `autosubmit-4.0.84/docs/source/agui/performance/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/statistics/fig/fig_stat_1.jpg` & `autosubmit-4.0.84/docs/source/agui/statistics/fig/fig_stat_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/statistics/fig/fig_stat_2.jpg` & `autosubmit-4.0.84/docs/source/agui/statistics/fig/fig_stat_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/statistics/index.rst` & `autosubmit-4.0.84/docs/source/agui/statistics/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/tree/fig/fig_tree_2.jpg` & `autosubmit-4.0.84/docs/source/agui/tree/fig/fig_tree_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/agui/tree/index.rst` & `autosubmit-4.0.84/docs/source/agui/tree/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/conf.py` & `autosubmit-4.0.84/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/devguide/index.rst` & `autosubmit-4.0.84/docs/source/devguide/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/index.rst` & `autosubmit-4.0.84/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/installation/index.rst` & `autosubmit-4.0.84/docs/source/installation/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/introduction/fig1.png` & `autosubmit-4.0.84/docs/source/introduction/fig1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/introduction/fig2.png` & `autosubmit-4.0.84/docs/source/introduction/fig2.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/introduction/fig3.png` & `autosubmit-4.0.84/docs/source/introduction/fig3.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/introduction/index.rst` & `autosubmit-4.0.84/docs/source/introduction/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/moduledoc/platforms.rst` & `autosubmit-4.0.84/docs/source/moduledoc/platforms.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/qstartguide/dummy.png` & `autosubmit-4.0.84/docs/source/qstartguide/dummy.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/qstartguide/index.rst` & `autosubmit-4.0.84/docs/source/qstartguide/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/troubleshooting/changelog.rst` & `autosubmit-4.0.84/docs/source/troubleshooting/changelog.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/troubleshooting/error-codes.rst` & `autosubmit-4.0.84/docs/source/troubleshooting/error-codes.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/troubleshooting/fig/monarch-da.png` & `autosubmit-4.0.84/docs/source/troubleshooting/fig/monarch-da.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/troubleshooting/fig/new_dependencies_0.png` & `autosubmit-4.0.84/docs/source/troubleshooting/fig/new_dependencies_0.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/troubleshooting/fig/new_dependencies_1.png` & `autosubmit-4.0.84/docs/source/troubleshooting/fig/new_dependencies_1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/troubleshooting/index.rst` & `autosubmit-4.0.84/docs/source/troubleshooting/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/unused_figs/group_chunk.png` & `autosubmit-4.0.84/docs/source/unused_figs/group_chunk.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/unused_figs/horizontal-vertical.png` & `autosubmit-4.0.84/docs/source/unused_figs/horizontal-vertical.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/unused_figs/wrapper.png` & `autosubmit-4.0.84/docs/source/unused_figs/wrapper.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/unused_figs/wrapper_expression.png` & `autosubmit-4.0.84/docs/source/unused_figs/wrapper_expression.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/unused_figs/wrapper_hybrid.png` & `autosubmit-4.0.84/docs/source/unused_figs/wrapper_hybrid.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/userguide/configure/develop_a_project.rst` & `autosubmit-4.0.84/docs/source/userguide/configure/develop_a_project.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/userguide/configure/index.rst` & `autosubmit-4.0.84/docs/source/userguide/configure/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/userguide/create/index.rst` & `autosubmit-4.0.84/docs/source/userguide/create/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/userguide/index.rst` & `autosubmit-4.0.84/docs/source/userguide/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/userguide/manage/index.rst` & `autosubmit-4.0.84/docs/source/userguide/manage/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/userguide/run/index.rst` & `autosubmit-4.0.84/docs/source/userguide/run/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/userguide/wrappers/fig/dasim.png` & `autosubmit-4.0.84/docs/source/userguide/wrappers/fig/dasim.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/userguide/wrappers/fig/horizontal_remote.png` & `autosubmit-4.0.84/docs/source/userguide/wrappers/fig/horizontal_remote.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/userguide/wrappers/fig/multiple_wrappers.png` & `autosubmit-4.0.84/docs/source/userguide/wrappers/fig/multiple_wrappers.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/userguide/wrappers/fig/rerun.png` & `autosubmit-4.0.84/docs/source/userguide/wrappers/fig/rerun.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/userguide/wrappers/fig/vertical-horizontal.png` & `autosubmit-4.0.84/docs/source/userguide/wrappers/fig/vertical-horizontal.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/userguide/wrappers/fig/vertical-mixed.png` & `autosubmit-4.0.84/docs/source/userguide/wrappers/fig/vertical-mixed.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/docs/source/userguide/wrappers/index.rst` & `autosubmit-4.0.84/docs/source/userguide/wrappers/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/environment.yml` & `autosubmit-4.0.84/environment.yml`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/log/fd_show.py` & `autosubmit-4.0.84/log/fd_show.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/log/log.py` & `autosubmit-4.0.84/log/log.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/setup.py` & `autosubmit-4.0.84/setup.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/integration/test_db_manager.py` & `autosubmit-4.0.84/test/integration/test_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/integration/test_job.py` & `autosubmit-4.0.84/test/integration/test_job.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/README` & `autosubmit-4.0.84/test/regression/README`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/default_conf/platforms.conf` & `autosubmit-4.0.84/test/regression/default_conf/platforms.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/local_asparser_test.py` & `autosubmit-4.0.84/test/regression/local_asparser_test.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf` & `autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mistral_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mn3_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mn3_with_paramiko/conf/jobs.conf` & `autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/conf/jobs.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mn4_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mn4_with_paramiko/conf/jobs.conf` & `autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/conf/jobs.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_moore_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.84/test/regression/test_moore_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_moore_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.84/test/regression/test_moore_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_moore_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_sedema_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/tests.conf` & `autosubmit-4.0.84/test/regression/tests.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/tests_commands.py` & `autosubmit-4.0.84/test/regression/tests_commands.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/tests_log.py` & `autosubmit-4.0.84/test/regression/tests_log.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/tests_runner.py` & `autosubmit-4.0.84/test/regression/tests_runner.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/regression/tests_utils.py` & `autosubmit-4.0.84/test/regression/tests_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/README_PIP.md` & `autosubmit-4.0.84/test/unit/README_PIP.md`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_basic_config.py` & `autosubmit-4.0.84/test/unit/test_basic_config.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_catlog.py` & `autosubmit-4.0.84/test/unit/test_catlog.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_chunk_date_lib.py` & `autosubmit-4.0.84/test/unit/test_chunk_date_lib.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_database_managers.py` & `autosubmit-4.0.84/test/unit/test_database_managers.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_db_manager.py` & `autosubmit-4.0.84/test/unit/test_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_dependencies.py` & `autosubmit-4.0.84/test/unit/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_dic_jobs.py` & `autosubmit-4.0.84/test/unit/test_dic_jobs.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_expid.py` & `autosubmit-4.0.84/test/unit/test_expid.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_history.py` & `autosubmit-4.0.84/test/unit/test_history.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_job.py` & `autosubmit-4.0.84/test/unit/test_job.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_job_common.py` & `autosubmit-4.0.84/test/unit/test_job_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_job_graph.py` & `autosubmit-4.0.84/test/unit/test_job_graph.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_job_grouping.py` & `autosubmit-4.0.84/test/unit/test_job_grouping.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_job_list.py` & `autosubmit-4.0.84/test/unit/test_job_list.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_job_package.py` & `autosubmit-4.0.84/test/unit/test_job_package.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_log.py` & `autosubmit-4.0.84/test/unit/test_log.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_machinefiles_wrapper.py` & `autosubmit-4.0.84/test/unit/test_machinefiles_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from unittest import TestCase
+
+import collections
+import textwrap
 from math import ceil
+
 from autosubmit.platforms.wrappers.wrapper_builder import PythonWrapperBuilder
-import textwrap
-import collections
 
 
 class TestMachinefiles(TestCase):
 
     def setUp(self):
         self.job_scripts = ['JOB_1', 'JOB_2', 'JOB_3']
 
     def test_job_less_than_48_cores_standard(self):
         num_processors = 60
         jobs_resources = {'MACHINEFILES': 'STANDARD', 'JOB': {'PROCESSORS': '20', 'TASKS': '48'},
                           'PROCESSORS_PER_NODE': '48'}
 
         wrapper_builder = PythonWrapperBuilder(header_directive='', jobs_scripts=self.job_scripts,
                                                num_processors=num_processors, expid='a000',
-                                               jobs_resources=jobs_resources,threads='1',retrials=0,wallclock_by_level=None)
+                                               jobs_resources=jobs_resources,threads='1',retrials=0,wallclock_by_level=None,num_processors_value=num_processors)
 
         nodes = self._create_nodelist(num_processors)
         cores_list = wrapper_builder.build_cores_list()
         machinefiles_code = wrapper_builder.get_machinefile_function().replace("_NEWLINE_", '\\n')
 
         result = dict()
 
@@ -55,15 +57,15 @@
     def test_job_more_than_48_cores_standard(self):
         num_processors = 150
         jobs_resources = {'MACHINEFILES': 'STANDARD', 'JOB': {'PROCESSORS': '50', 'TASKS': '48'},
                           'PROCESSORS_PER_NODE': '48'}
 
         wrapper_builder = PythonWrapperBuilder(header_directive='', jobs_scripts=self.job_scripts,
                                                num_processors=num_processors, expid='a000',
-                                               jobs_resources=jobs_resources,threads='1',retrials=0,wallclock_by_level=None)
+                                               jobs_resources=jobs_resources,threads='1',retrials=0,wallclock_by_level=None,num_processors_value=num_processors)
 
         nodes = self._create_nodelist(num_processors)
         cores_list = wrapper_builder.build_cores_list()
         machinefiles_code = wrapper_builder.get_machinefile_function().replace("_NEWLINE_", '\\n')
 
         result = dict()
```

### Comparing `autosubmit-4.0.82/test/unit/test_paramiko_platform.py` & `autosubmit-4.0.84/test/unit/test_paramiko_platform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_pjm.py` & `autosubmit-4.0.84/test/unit/test_pjm.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_platform_monitor.py` & `autosubmit-4.0.84/test/unit/test_platform_monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_slurm_platform.py` & `autosubmit-4.0.84/test/unit/test_slurm_platform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_statistics.py` & `autosubmit-4.0.84/test/unit/test_statistics.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_strategies.py` & `autosubmit-4.0.84/test/unit/test_strategies.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.82/test/unit/test_wrappers.py` & `autosubmit-4.0.84/test/unit/test_wrappers.py`

 * *Files identical despite different names*

