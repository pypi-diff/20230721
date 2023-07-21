# Comparing `tmp/cylc-flow-8.1.4.tar.gz` & `tmp/cylc-flow-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cylc-flow-8.1.4.tar", last modified: Thu May  4 12:38:02 2023, max compression
+gzip compressed data, was "cylc-flow-8.2.0.tar", last modified: Fri Jul 21 09:36:02 2023, max compression
```

## Comparing `cylc-flow-8.1.4.tar` & `cylc-flow-8.2.0.tar`

### file list

```diff
@@ -1,315 +1,318 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.254397 cylc-flow-8.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-05-04 12:38:02.254397 cylc-flow-8.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.202397 cylc-flow-8.1.4/cylc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.222397 cylc-flow-8.1.4/cylc/flow/
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/async_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17180 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/broadcast_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/broadcast_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/c3mro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.222397 cylc-flow-8.1.4/cylc/flow/cfgspec/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cfgspec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cfgspec/glbl_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)    71511 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cfgspec/globalcfg.py
--rw-r--r--   0 runner    (1001) docker     (123)    83023 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cfgspec/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/command_polling.py
--rw-r--r--   0 runner    (1001) docker     (123)    97151 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/context_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.222397 cylc-flow-8.1.4/cylc/flow/cycling/
--rw-r--r--   0 runner    (1001) docker     (123)    14593 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cycling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23211 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cycling/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)    34957 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cycling/iso8601.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cycling/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cycling/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/cylc_subproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/daemonize.py
--rw-r--r--   0 runner    (1001) docker     (123)    22194 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/data_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    89336 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/data_store_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/dbstatecheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.226397 cylc-flow-8.1.4/cylc/flow/etc/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     7934 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/cylc
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/cylc-completion.bash
--rw-r--r--   0 runner    (1001) docker     (123)    14460 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/job.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.226397 cylc-flow-8.1.4/cylc/flow/etc/syntax/
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/syntax/cylc-mode.el
--rw-r--r--   0 runner    (1001) docker     (123)    25186 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/syntax/cylc.lang
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/syntax/cylc.vim
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/syntax/cylc.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.226397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/api-keys
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.226397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/
--rwxr-xr-x   0 runner    (1001) docker     (123)      802 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/.validate
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.226397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.226397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.206397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.226397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.226397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.226397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1139 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.206397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/forecast-script/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/forecast-script/forecast
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/forecast-script/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/inheritance-tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/map-template/
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/map-template/map-template.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.206397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/message-trigger-tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/random.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/retries-tutorial/
--rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/retries-tutorial/.validate
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/retries-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-introduction/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-introduction/.validate
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-introduction/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      459 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-introduction/bin/get-observations
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-introduction/etc/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-introduction/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.230397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.234397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.234397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.206397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.234397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.234397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/runtime
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.234397 cylc-flow-8.1.4/cylc/flow/etc/tutorial/test-data/
--rw-r--r--   0 runner    (1001) docker     (123)    33085 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/test-data/rainfall.csv
--rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv
--rw-r--r--   0 runner    (1001) docker     (123)    38004 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/flow_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    35572 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/graph_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/graphnode.py
--rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/host_select.py
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/hostuserutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    24245 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/id.py
--rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/id_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/id_match.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.234397 cylc-flow-8.1.4/cylc/flow/install_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/install_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/install_plugins/log_vc_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.206397 cylc-flow-8.1.4/cylc/flow/jinja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.234397 cylc-flow-8.1.4/cylc/flow/jinja/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/jinja/filters/duration_as.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/jinja/filters/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/jinja/filters/strftime.py
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.238397 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/at.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/background.py
--rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/loadleveler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/moab.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/pbs_multi_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/sge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_handlers/slurm_packjob.py
--rw-r--r--   0 runner    (1001) docker     (123)    33912 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/job_runner_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/listify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/log_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (123)    15363 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/loggingutil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.238397 cylc-flow-8.1.4/cylc/flow/main_loop/
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/main_loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/main_loop/auto_restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/main_loop/health_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/main_loop/log_data_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/main_loop/log_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/main_loop/log_main_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/main_loop/log_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/main_loop/reset_bad_hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.242397 cylc-flow-8.1.4/cylc/flow/network/
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/authorisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11918 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/replier.py
--rw-r--r--   0 runner    (1001) docker     (123)    30538 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    74542 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/ssh_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/network/subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)    28587 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/option_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/param_expand.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.242397 cylc-flow-8.1.4/cylc/flow/parsec/
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/OrderedDict.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/empysupport.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/fileparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/include.py
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/jinja2support.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    40452 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/parsec/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/pathutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    25192 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/platforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/prerequisite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/print_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    39289 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/rundb.py
--rw-r--r--   0 runner    (1001) docker     (123)    80364 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20200 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scheduler_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.250397 cylc-flow-8.1.4/cylc/flow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15346 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/broadcast.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20637 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/cat_log.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5028 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/check_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/clean.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2617 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20478 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/completion_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6429 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8931 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/cycle_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    21083 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/cylc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6042 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/diff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8083 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4425 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/ext_trigger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1491 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/function_run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2514 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/get_resources.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1871 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/get_workflow_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2311 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/get_workflow_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14884 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4378 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/hold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10639 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/install.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1722 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/jobs_kill.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1697 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/jobs_poll.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/jobs_submit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2483 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/kill.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24919 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/lint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6228 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6419 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/pause.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3955 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/play.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2548 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/psutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    12227 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/reinstall.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3711 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/release.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3254 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/reload.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2108 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/remote_init.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1533 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/remote_tidy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2225 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/remove.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13206 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/report_timings.py
--rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/scan.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3504 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/set_outputs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2536 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/set_verbosity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12679 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/show.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8360 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/stop.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3658 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/subscribe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5272 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/tui.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6321 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/validate_install_play.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/validate_reinstall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/view.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10001 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/scripts/workflow_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/subprocctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    23404 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/subprocpool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_action_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    63362 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_events_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_job_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55110 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_job_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    80010 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    18451 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.250397 cylc-flow-8.1.4/cylc/flow/task_queues/
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_queues/independent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_remote_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    25375 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_remote_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    18423 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_state_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/task_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/taskdef.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/templatevars.py
--rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/time_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.254397 cylc-flow-8.1.4/cylc/flow/tui/
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18584 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/tui/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/tui/overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/tui/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/unicode_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/wallclock.py
--rw-r--r--   0 runner    (1001) docker     (123)    33592 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/workflow_db_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/workflow_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    69723 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/workflow_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/workflow_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/xtrigger_mgr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.254397 cylc-flow-8.1.4/cylc/flow/xtriggers/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/xtriggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/xtriggers/echo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/xtriggers/wall_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/xtriggers/workflow_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/cylc/flow/xtriggers/xrandom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:38:02.254397 cylc-flow-8.1.4/cylc_flow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-05-04 12:38:01.000000 cylc-flow-8.1.4/cylc_flow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-05-04 12:38:01.000000 cylc-flow-8.1.4/cylc_flow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:38:01.000000 cylc-flow-8.1.4/cylc_flow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-04 12:38:01.000000 cylc-flow-8.1.4/cylc_flow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-04 12:38:01.000000 cylc-flow-8.1.4/cylc_flow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 12:38:01.000000 cylc-flow-8.1.4/cylc_flow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-05-04 12:38:02.254397 cylc-flow-8.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-04 12:37:56.000000 cylc-flow-8.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.189521 cylc-flow-8.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-21 09:36:02.189521 cylc-flow-8.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.157521 cylc-flow-8.2.0/cylc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.169521 cylc-flow-8.2.0/cylc/flow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/async_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17061 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/broadcast_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/broadcast_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/c3mro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.169521 cylc-flow-8.2.0/cylc/flow/cfgspec/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/cfgspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/cfgspec/glbl_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72543 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/cfgspec/globalcfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84962 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/cfgspec/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16942 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/command_polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99371 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/context_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.169521 cylc-flow-8.2.0/cylc/flow/cycling/
+-rw-r--r--   0 runner    (1001) docker     (123)    14593 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/cycling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23211 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/cycling/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35019 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/cycling/iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/cycling/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/cycling/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/cylc_subproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/daemonize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22632 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/data_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88708 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/data_store_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/dbstatecheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.169521 cylc-flow-8.2.0/cylc/flow/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7934 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/cylc
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/cylc-completion.bash
+-rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/job.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.169521 cylc-flow-8.2.0/cylc/flow/etc/syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/syntax/cylc-mode.el
+-rw-r--r--   0 runner    (1001) docker     (123)    25186 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/syntax/cylc.lang
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/syntax/cylc.vim
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/syntax/cylc.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.169521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/api-keys
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.173521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      802 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/.validate
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.173521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.173521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.157521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.173521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.173521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.173521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1139 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.173521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.173521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.157521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.173521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.173521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.173521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/forecast-script/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/forecast-script/forecast
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/forecast-script/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.173521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/inheritance-tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.173521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/map-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/map-template/map-template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.157521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/message-trigger-tutorial/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.173521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/random.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.173521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/retries-tutorial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/retries-tutorial/.validate
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/retries-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.173521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-introduction/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-introduction/.validate
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.173521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-introduction/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      459 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-introduction/bin/get-observations
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.173521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-introduction/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-introduction/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.173521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.177521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.177521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.157521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.177521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.177521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/runtime
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.177521 cylc-flow-8.2.0/cylc/flow/etc/tutorial/test-data/
+-rw-r--r--   0 runner    (1001) docker     (123)    33085 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/test-data/rainfall.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38004 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/flow_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35424 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/graph_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/graphnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/host_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/hostuserutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24799 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/id_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/id_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21546 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/install.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.177521 cylc-flow-8.2.0/cylc/flow/install_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/install_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/install_plugins/log_vc_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.157521 cylc-flow-8.2.0/cylc/flow/jinja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.177521 cylc-flow-8.2.0/cylc/flow/jinja/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/jinja/filters/duration_as.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/jinja/filters/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/jinja/filters/strftime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15445 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/job_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.177521 cylc-flow-8.2.0/cylc/flow/job_runner_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/job_runner_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/job_runner_handlers/at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/job_runner_handlers/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/job_runner_handlers/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/job_runner_handlers/loadleveler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/job_runner_handlers/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/job_runner_handlers/moab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/job_runner_handlers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/job_runner_handlers/pbs_multi_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/job_runner_handlers/sge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/job_runner_handlers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/job_runner_handlers/slurm_packjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33926 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/job_runner_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/listify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/log_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/loggingutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.181521 cylc-flow-8.2.0/cylc/flow/main_loop/
+-rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/main_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/main_loop/auto_restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/main_loop/health_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/main_loop/log_data_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/main_loop/log_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/main_loop/log_main_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/main_loop/log_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/main_loop/reset_bad_hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.181521 cylc-flow-8.2.0/cylc/flow/network/
+-rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/network/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/network/authorisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/network/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/network/client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/network/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/network/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/network/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/network/replier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30538 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/network/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16241 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/network/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79817 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/network/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/network/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/network/ssh_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/network/subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29250 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/option_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17877 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/param_expand.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.181521 cylc-flow-8.2.0/cylc/flow/parsec/
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/parsec/OrderedDict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/parsec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/parsec/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/parsec/empysupport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/parsec/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21611 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/parsec/fileparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/parsec/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/parsec/jinja2support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/parsec/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/parsec/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42818 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/parsec/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/pathutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24924 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/prerequisite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/print_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39531 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/rundb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87673 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20741 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scheduler_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.189521 cylc-flow-8.2.0/cylc/flow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15346 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/broadcast.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20655 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/cat_log.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4986 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/check_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/clean.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2617 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20478 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/completion_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6429 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8931 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/cycle_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/cylc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5986 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8083 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4425 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/ext_trigger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1491 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/function_run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2513 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/get_resources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1871 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/get_workflow_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2311 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/get_workflow_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14884 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4378 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/hold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10942 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/install.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1722 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/jobs_kill.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1697 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/jobs_poll.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/jobs_submit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2483 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/kill.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38644 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/lint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6228 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/list.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6417 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/pause.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3955 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/play.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2548 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/psutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/reinstall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3711 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/release.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3254 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/reload.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2106 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/remote_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1533 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/remote_tidy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2225 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/remove.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13206 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/report_timings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16114 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/scan.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3504 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/set_outputs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2536 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/set_verbosity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12153 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/show.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8360 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/stop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3658 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/subscribe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5272 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/tui.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6436 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/validate_install_play.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/validate_reinstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/view.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10001 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/scripts/workflow_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/subprocctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23404 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/subprocpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/task_action_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63549 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/task_events_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/task_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/task_job_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55051 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/task_job_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/task_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/task_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80460 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/task_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/task_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/task_qualifiers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.189521 cylc-flow-8.2.0/cylc/flow/task_queues/
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/task_queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/task_queues/independent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/task_remote_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25398 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/task_remote_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18225 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/task_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/task_state_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/task_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14419 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/taskdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/templatevars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/time_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.189521 cylc-flow-8.2.0/cylc/flow/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18799 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/tui/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/tui/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/tui/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/unicode_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/wallclock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32498 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/workflow_db_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/workflow_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34081 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/workflow_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/workflow_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/xtrigger_mgr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.189521 cylc-flow-8.2.0/cylc/flow/xtriggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/xtriggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/xtriggers/echo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/xtriggers/wall_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/xtriggers/workflow_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/cylc/flow/xtriggers/xrandom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:36:02.189521 cylc-flow-8.2.0/cylc_flow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-21 09:36:01.000000 cylc-flow-8.2.0/cylc_flow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-07-21 09:36:01.000000 cylc-flow-8.2.0/cylc_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:36:01.000000 cylc-flow-8.2.0/cylc_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-21 09:36:01.000000 cylc-flow-8.2.0/cylc_flow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-21 09:36:01.000000 cylc-flow-8.2.0/cylc_flow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 09:36:01.000000 cylc-flow-8.2.0/cylc_flow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-21 09:36:02.193522 cylc-flow-8.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-21 09:35:56.000000 cylc-flow-8.2.0/setup.py
```

### Comparing `cylc-flow-8.1.4/COPYING` & `cylc-flow-8.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/PKG-INFO` & `cylc-flow-8.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-flow
-Version: 8.1.4
+Version: 8.2.0
 Summary: A workflow engine for cycling systems
 Home-page: https://cylc.org/
 Author: Hilary Oliver
 License: GPL
 Project-URL: Documentation, https://cylc.github.io/cylc-doc/stable/html/index.html
 Project-URL: Source, https://github.com/cylc/cylc-flow
 Project-URL: Tracker, https://github.com/cylc/cylc-flow/issues
@@ -18,14 +18,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: empy
 Provides-Extra: graph
@@ -90,14 +91,20 @@
 cylc install example
 cylc play example
 
 # watch it run
 cylc tui example
 ```
 
+### The Cylc Ecosystem
+
+- [cylc-flow](https://github.com/cylc/cylc-flow) - The core Cylc Scheduler for defining and running workflows.
+- [cylc-uiserver](https://github.com/cylc/cylc-uiserver) - The web-based Cylc graphical user interface for monitoring and controlling workflows.
+- [cylc-rose](https://github.com/cylc/cylc-rose) - Provides integration with [Rose](http://metomi.github.io/rose/).
+
 ### Migrating From Cylc 7
 
 [Migration Guide](https://cylc.github.io/cylc-doc/stable/html/7-to-8/index.html)
 | [Migration Support](https://cylc.discourse.group/c/cylc/7-to-8/13)
 
 Cylc 8 can run most Cylc 7 workflows in compatibility mode with little to no
 changes, go through the
@@ -154,9 +161,7 @@
 * Read the [contributing](CONTRIBUTING.md) page.
 * Development setup instructions are in the
   [developer docs](https://cylc.github.io/cylc-admin/#cylc-8-developer-docs).
 * Involved change proposals can be found in the
   [admin pages](https://cylc.github.io/cylc-admin/#change-proposals).
 * Touch base in the
   [developers chat](https://matrix.to/#/#cylc-general:matrix.org).
-
-
```

### Comparing `cylc-flow-8.1.4/README.md` & `cylc-flow-8.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,20 @@
 cylc install example
 cylc play example
 
 # watch it run
 cylc tui example
 ```
 
+### The Cylc Ecosystem
+
+- [cylc-flow](https://github.com/cylc/cylc-flow) - The core Cylc Scheduler for defining and running workflows.
+- [cylc-uiserver](https://github.com/cylc/cylc-uiserver) - The web-based Cylc graphical user interface for monitoring and controlling workflows.
+- [cylc-rose](https://github.com/cylc/cylc-rose) - Provides integration with [Rose](http://metomi.github.io/rose/).
+
 ### Migrating From Cylc 7
 
 [Migration Guide](https://cylc.github.io/cylc-doc/stable/html/7-to-8/index.html)
 | [Migration Support](https://cylc.discourse.group/c/cylc/7-to-8/13)
 
 Cylc 8 can run most Cylc 7 workflows in compatibility mode with little to no
 changes, go through the
```

### Comparing `cylc-flow-8.1.4/cylc/flow/__init__.py` & `cylc-flow-8.2.0/cylc/flow/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,26 +31,33 @@
     "NORMAL": logging.INFO,
     "WARNING": logging.WARNING,
     "ERROR": logging.ERROR,
     "CRITICAL": logging.CRITICAL,
 }
 
 
+class LoggerAdaptor(logging.LoggerAdapter):
+    """Adds a prefix to log messages."""
+    def process(self, msg, kwargs):
+        ret = f"[{self.extra['prefix']}] {msg}" if self.extra else msg
+        return ret, kwargs
+
+
 def environ_init():
     """Initialise cylc environment."""
     # Python output buffering delays appearance of stdout and stderr
     # when output is not directed to a terminal (this occurred when
     # running pre-5.0 cylc via the posix nohup command; is it still the
     # case in post-5.0 daemon-mode cylc?)
     os.environ['PYTHONUNBUFFERED'] = 'true'
 
 
 environ_init()
 
-__version__ = '8.1.4'
+__version__ = '8.2.0'
 
 
 def iter_entry_points(entry_point_name):
     """Iterate over Cylc entry points."""
     import pkg_resources
     yield from (
         entry_point
```

### Comparing `cylc-flow-8.1.4/cylc/flow/async_util.py` & `cylc-flow-8.2.0/cylc/flow/async_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,20 +12,19 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Utilities for use with asynchronous code."""
 
 import asyncio
+from functools import partial, wraps
 import os
 from pathlib import Path
 from typing import List, Union
 
-from aiofiles.os import wrap  # type: ignore[attr-defined]
-
 from cylc.flow import LOG
 
 
 class _AsyncPipe:
     """Implement the @pipe interface.
 
     Represents and implements an asynchronous pipe.
@@ -56,20 +55,20 @@
             The previous item in the pipe or None.
         _right (_AsyncPipe):
             The next item in the pipe or None.
 
     """
 
     def __init__(
-            self,
-            func,
-            args=None,
-            kwargs=None,
-            filter_stop=True,
-            preserve_order=True
+        self,
+        func,
+        args=None,
+        kwargs=None,
+        filter_stop=True,
+        preserve_order=True
     ):
         self.func = func
         self.args = args or ()
         self.kwargs = kwargs or {}
         self.filter_stop = filter_stop
         self.preserve_order = preserve_order
         self._left = None
@@ -389,17 +388,14 @@
     else:
         # @pipe()
         def _pipe(func):
             return _PipeFunction(func)
         return _pipe
 
 
-async_listdir = wrap(os.listdir)
-
-
 async def scandir(path: Union[Path, str]) -> List[Path]:
     """Asynchronous directory listing (performs os.listdir in an executor)."""
     return [
         Path(path, sub_path)
         for sub_path in await async_listdir(path)
     ]
 
@@ -445,7 +441,27 @@
     while pending:
         done, pending = await asyncio.wait(
             pending,
             return_when=asyncio.FIRST_COMPLETED
         )
         for task in done:
             yield task._args, task.result()
+
+
+def make_async(fcn):
+    """Make a synchronous function async by running it in an executor.
+
+    The default asyncio executor is the ThreadPoolExecutor so this essentially
+    syntactic sugar for running the wrapped function in a thread.
+    """
+    @wraps(fcn)
+    async def _fcn(*args, executor=None, **kwargs):
+        nonlocal fcn
+        return await asyncio.get_event_loop().run_in_executor(
+            executor,
+            partial(fcn, *args, **kwargs),
+        )
+
+    return _fcn
+
+
+async_listdir = make_async(os.listdir)
```

### Comparing `cylc-flow-8.1.4/cylc/flow/broadcast_mgr.py` & `cylc-flow-8.2.0/cylc/flow/broadcast_mgr.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,33 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Manage broadcast (and external trigger broadcast)."""
 
 import re
 from copy import deepcopy
 from threading import RLock
+from typing import Optional, TYPE_CHECKING
 
 from cylc.flow import LOG
 from cylc.flow.broadcast_report import (
     CHANGE_FMT,
     CHANGE_PREFIX_SET,
     get_broadcast_change_report,
     get_broadcast_bad_options_report,
 )
 from cylc.flow.cfgspec.workflow import SPEC
-from cylc.flow.id import Tokens
 from cylc.flow.cycling.loader import get_point, standardise_point_string
 from cylc.flow.exceptions import PointParsingError
 from cylc.flow.parsec.util import listjoin
 from cylc.flow.parsec.validate import BroadcastConfigValidator
 
+if TYPE_CHECKING:
+    from cylc.flow.id import Tokens
+
+
 ALL_CYCLE_POINTS_STRS = ["*", "all-cycle-points", "all-cycles"]
 
 
 def addict(target, source):
     """Recursively add source dict to target dict."""
     for key, val in source.items():
         if isinstance(val, dict):
@@ -152,36 +156,29 @@
                         point_string not in ALL_CYCLE_POINTS_STRS and
                         get_point(point_string) < cutoff_point):
                     point_strings.append(point_string)
         if not point_strings:
             return (None, {"expire": [cutoff]})
         return self.clear_broadcast(point_strings=point_strings, **kwargs)
 
-    def get_broadcast(self, task_id=None):
+    def get_broadcast(self, tokens: 'Optional[Tokens]' = None) -> dict:
         """Retrieve all broadcast variables that target a given task ID."""
-        if task_id == "None":
-            task_id = None
-        if not task_id:
+        if tokens is None or tokens == 'None':
             # all broadcasts requested
             return self.broadcasts
-        try:
-            tokens = Tokens(task_id, relative=True)
-            name = tokens['task']
-            point_string = tokens['cycle']
-        except ValueError:
-            raise Exception("Can't split task_id %s" % task_id)
-
-        ret = {}
+        ret: dict = {}
         # The order is:
         #    all:root -> all:FAM -> ... -> all:task
         # -> tag:root -> tag:FAM -> ... -> tag:task
-        for cycle in ALL_CYCLE_POINTS_STRS + [point_string]:
+        for cycle in ALL_CYCLE_POINTS_STRS + [tokens['cycle']]:
             if cycle not in self.broadcasts:
                 continue
-            for namespace in reversed(self.linearized_ancestors[name]):
+            for namespace in reversed(
+                    self.linearized_ancestors[tokens['task']]
+            ):
                 if namespace in self.broadcasts[cycle]:
                     addict(ret, self.broadcasts[cycle][namespace])
         return ret
 
     def load_db_broadcast_states(self, row_idx, row):
         """Load broadcast variables from runtime DB broadcast states row."""
         if row_idx == 0:
```

### Comparing `cylc-flow-8.1.4/cylc/flow/broadcast_report.py` & `cylc-flow-8.2.0/cylc/flow/broadcast_report.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/c3mro.py` & `cylc-flow-8.2.0/cylc/flow/c3mro.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/cfgspec/__init__.py` & `cylc-flow-8.2.0/cylc/flow/cfgspec/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/cfgspec/glbl_cfg.py` & `cylc-flow-8.2.0/cylc/flow/cfgspec/glbl_cfg.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/cfgspec/globalcfg.py` & `cylc-flow-8.2.0/cylc/flow/cfgspec/globalcfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,14 +259,21 @@
     'abort on inactivity timeout': f'''
         Whether the scheduler should shut down immediately with error status if
         the inactivity timer times out.
 
         .. versionchanged:: 8.0.0
 
            {REPLACES}``abort on inactivity``.
+    ''',
+    'restart timeout': '''
+        How long to wait for intervention on restarting a completed workflow.
+        The timer stops if any task is triggered.
+
+        .. versionadded:: 8.2.0
+
     '''
 }
 
 MAIL_DESCR = '''
 Settings for the scheduler to send event emails.
 
 These settings are used for both workflow and task events.
@@ -835,14 +842,16 @@
                 elif item.startswith("abort on"):
                     vdr_type = VDR.V_BOOLEAN
                     default = (item == "abort on stall timeout")
                 elif item.endswith("timeout"):
                     vdr_type = VDR.V_INTERVAL
                     if item == "stall timeout":
                         default = DurationFloat(3600)
+                    elif item == "restart timeout":
+                        default = DurationFloat(120)
                     else:
                         default = None
                 Conf(item, vdr_type, default, desc=desc)
 
         with Conf('mail', desc=(
             default_for(MAIL_DESCR, "[scheduler][mail]", section=True)
         )):
@@ -1020,70 +1029,70 @@
             with Conf('<install target>', desc="""
                 :ref:`Host <Install targets>` on which to create the symlinks.
             """):
                 Conf('run', VDR.V_STRING, None, desc="""
                     Alternative location for the run dir.
 
                     If specified, the workflow run directory will
-                    be created in ``<this-path>/cylc-run/<workflow-name>``
+                    be created in ``<this-path>/cylc-run/<workflow-id>``
                     and a symbolic link will be created from
-                    ``$HOME/cylc-run/<workflow-name>``.
+                    ``$HOME/cylc-run/<workflow-id>``.
                     If not specified the workflow run directory will be created
-                    in ``$HOME/cylc-run/<workflow-name>``.
+                    in ``$HOME/cylc-run/<workflow-id>``.
                     All the workflow files and the ``.service`` directory get
                     installed into this directory.
 
                     .. versionadded:: 8.0.0
                 """)
                 Conf('log', VDR.V_STRING, None, desc="""
                     Alternative location for the log dir.
 
                     If specified the workflow log directory will be created in
-                    ``<this-path>/cylc-run/<workflow-name>/log`` and a
+                    ``<this-path>/cylc-run/<workflow-id>/log`` and a
                     symbolic link will be created from
-                    ``$HOME/cylc-run/<workflow-name>/log``. If not specified
+                    ``$HOME/cylc-run/<workflow-id>/log``. If not specified
                     the workflow log directory will be created in
-                    ``$HOME/cylc-run/<workflow-name>/log``.
+                    ``$HOME/cylc-run/<workflow-id>/log``.
 
                     .. versionadded:: 8.0.0
                 """)
                 Conf('share', VDR.V_STRING, None, desc="""
                     Alternative location for the share dir.
 
                     If specified the workflow share directory will be
-                    created in ``<this-path>/cylc-run/<workflow-name>/share``
+                    created in ``<this-path>/cylc-run/<workflow-id>/share``
                     and a symbolic link will be created from
-                    ``<$HOME/cylc-run/<workflow-name>/share``. If not specified
+                    ``<$HOME/cylc-run/<workflow-id>/share``. If not specified
                     the workflow share directory will be created in
-                    ``$HOME/cylc-run/<workflow-name>/share``.
+                    ``$HOME/cylc-run/<workflow-id>/share``.
 
                     .. versionadded:: 8.0.0
                 """)
                 Conf('share/cycle', VDR.V_STRING, None, desc="""
                     Alternative directory for the share/cycle dir.
 
                     If specified the workflow share/cycle directory
                     will be created in
-                    ``<this-path>/cylc-run/<workflow-name>/share/cycle``
+                    ``<this-path>/cylc-run/<workflow-id>/share/cycle``
                     and a symbolic link will be created from
-                    ``$HOME/cylc-run/<workflow-name>/share/cycle``. If not
+                    ``$HOME/cylc-run/<workflow-id>/share/cycle``. If not
                     specified the workflow share/cycle directory will be
-                    created in ``$HOME/cylc-run/<workflow-name>/share/cycle``.
+                    created in ``$HOME/cylc-run/<workflow-id>/share/cycle``.
 
                     .. versionadded:: 8.0.0
                 """)
                 Conf('work', VDR.V_STRING, None, desc="""
                     Alternative directory for the work dir.
 
                     If specified the workflow work directory will be created in
-                    ``<this-path>/cylc-run/<workflow-name>/work`` and a
+                    ``<this-path>/cylc-run/<workflow-id>/work`` and a
                     symbolic link will be created from
-                    ``$HOME/cylc-run/<workflow-name>/work``. If not specified
+                    ``$HOME/cylc-run/<workflow-id>/work``. If not specified
                     the workflow work directory will be created in
-                    ``$HOME/cylc-run/<workflow-name>/work``.
+                    ``$HOME/cylc-run/<workflow-id>/work``.
 
                     .. versionadded:: 8.0.0
                 """)
     with Conf('platforms', desc='''
         Platforms allow you to define compute resources available at your
         site.
 
@@ -1395,14 +1404,25 @@
                    {REPLACES}``global.rc[hosts][<host>]retrieve job logs``.
                    {PLATFORM_REPLACES.format("[remote]retrieve job logs")}
             ''')
             Conf('retrieve job logs command', VDR.V_STRING, 'rsync -a',
                  desc=f'''
                 {LOG_RETR_SETTINGS['retrieve job logs command']}
 
+                .. note::
+                   The default command (``rsync -a``) means that the retrieved
+                   files (and the directories above including ``job/log``) get
+                   the same permissions as on the remote host. This can cause
+                   problems if the remote host uses different permissions to
+                   the scheduler host (e.g. no world read access). To avoid
+                   this problem you can set the command to
+                   ``rsync -a --no-p --no-g --chmod=ugo=rwX`` which means the
+                   retrieved files get the default permissions used on the
+                   scheduler host.
+
                 .. versionchanged:: 8.0.0
 
                    {REPLACES}``global.rc[hosts][<host>]retrieve job logs
                    command``.
             ''')
             Conf('retrieve job logs max size', VDR.V_STRING, desc=f'''
                 {LOG_RETR_SETTINGS['retrieve job logs max size']}
@@ -1422,20 +1442,23 @@
 
                    {REPLACES}``global.rc[hosts][<host>]retrieve job logs
                    retry delays``.
                    {PLATFORM_REPLACES.format(
                        "[remote]retrieve job logs retry delays")}
             ''')
             Conf('tail command template',
-                 VDR.V_STRING, 'tail -n +1 --follow=name -F %(filename)s',
+                 VDR.V_STRING, 'tail -n +1 --follow=name %(filename)s',
                  desc=f'''
                 A command template (with ``%(filename)s`` substitution) to
                 tail-follow job logs this platform, by ``cylc cat-log``.
 
-                You are are unlikely to need to override this.
+                .. warning::
+
+                   You are are unlikely to need to override this. Doing so may
+                   adversely affect the UI log view.
 
                 .. versionchanged:: 8.0.0
 
                    {REPLACES}``global.rc[hosts][<host>]tail command template``.
             ''')
             Conf('err tailer', VDR.V_STRING, desc=f'''
                 A command template (with ``%(job_id)s`` substitution) that can
```

### Comparing `cylc-flow-8.1.4/cylc/flow/cfgspec/workflow.py` & `cylc-flow-8.2.0/cylc/flow/cfgspec/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -716,18 +716,19 @@
             listing all member tasks.
         '''):
             Conf('clock-trigger', VDR.V_STRING_LIST, desc='''
             Legacy clock trigger definitions.
 
             .. deprecated:: 8.0.0
 
-               Please read :ref:`Section External Triggers` before
-               using the older clock triggers described in this section.
+               These are now auto-upgraded to the newer wall_clock xtriggers
+               (see :ref:`Section External Triggers`). The old way defining
+               clock-triggers will be removed in an upcoming Cylc version.
 
-            Clock-trigger tasks (see :ref:`ClockTriggerTasks`) wait on a wall
+            Clock-triggered tasks (see :ref:`ClockTriggerTasks`) wait on a wall
             clock time specified as an offset from their own cycle point.
 
             Example:
 
             ``foo(PT1H30M), bar(PT1.5H), baz``
             ''')
             Conf('external-trigger', VDR.V_STRING_LIST, desc='''
@@ -1525,15 +1526,15 @@
 
             with Conf('workflow state polling', desc=f'''
                 Configure automatic workflow polling tasks as described in
                 :ref:`WorkflowStatePolling`.
 
                 The items in this section reflect
                 options and defaults of the ``cylc workflow-state`` command,
-                except that the target workflow name and the
+                except that the target workflow ID and the
                 ``--task``, ``--cycle``, and ``--status`` options are
                 taken from the graph notation.
 
                 .. versionchanged:: 8.0.0
 
                    {REPLACES}``[runtime][<namespace>]suite state polling``.
             '''):
@@ -1589,15 +1590,15 @@
                 .. seealso::
 
                    :ref:`TaskExecutionEnvironment`.
 
                 You can also specify job environment templates here for
                 :ref:`parameterized tasks <User Guide Param>`.
             '''):
-                Conf('<variable>', VDR.V_STRING, desc='''
+                Conf('<variable>', VDR.V_STRING, desc=r'''
                     A custom user defined variable for a task execution
                     environment.
 
                     The order of definition is preserved that each variable can
                     refer to previously defined
                     variables. Values are passed through to the job
                     script without evaluation or manipulation by Cylc
@@ -1630,14 +1631,40 @@
 
                     Examples::
 
                        MYNUM = %(i)d
                        MYITEM = %(item)s
                        MYFILE = /path/to/%(i)03d/%(item)s
 
+                    .. note::
+
+                       As with other Cylc configurations, leading or trailing
+                       whitespace will be stripped, so the following two
+                       examples are equivalent:
+
+                       .. list-table::
+                          :class: grid-table
+
+                          * - .. code-block:: cylc
+
+                                 [environment]
+                                     FOO = " a "
+                                     BAR = """
+                                       $(foo bar baz)
+                                   """
+                            - .. code-block:: cylc
+
+                                 [environment]
+                                     FOO = "a"
+                                     BAR = "$(foo bar baz)"
+
+                       If leading or trailing whitespace is required, consider
+                       using the ``\0`` escape character, or set the variable
+                       in :cylc:conf:`[..][..]env-script`.
+
                     .. versionchanged:: 7.8.7/7.9.2
 
                        Parameter environment templates (previously in
                        ``[runtime][X][parameter environment templates]``) have
                        moved here.
                 ''')
 
@@ -1650,30 +1677,48 @@
                 Conf('<directive>', VDR.V_STRING, desc=DIRECTIVES_ITEM_DESCR)
 
             with Conf('outputs', desc='''
                 Register custom task outputs for use in message triggering in
                 this section (:ref:`MessageTriggers`)
             '''):
                 Conf('<output>', VDR.V_STRING, desc='''
-                    Task output messages (:ref:`MessageTriggers`).
+                    Define custom task outputs (aka :ref:`MessageTriggers`).
+
+                    :term:`Custom outputs <custom output>` allow you to extend
+                    the built-in task outputs e.g. ``succeeded`` and ``failed``
+                    in order to provide more detailed information about task
+                    state. Custom outputs can be used to express dependencies
+                    in the graph as with built-in outputs.
 
-                    The item name is used to select the custom output
-                    message in graph trigger notation.
+                    Custom outputs are defined in the form:
+
+                    .. code-block:: cylc
+
+                       output = message
+
+                    Where ``output`` is the name of the output as it is used in
+                    the graph, and ``message`` is the task message sent by
+                    the ``cylc message`` command which tells Cylc that this
+                    output has been completed. See :ref:`MessageTriggers` for
+                    more details.
 
                     Examples:
 
                     .. code-block:: cylc
 
                        out1 = "sea state products ready"
                        out2 = "NWP restart files completed"
 
-                    Task outputs are validated by
-                    :py:class:`cylc.flow.unicode_rules.TaskOutputValidator`.
+                    Custom outputs must satisfy these rules:
 
                     .. autoclass:: cylc.flow.unicode_rules.TaskOutputValidator
+
+                    Task messages must satisfy these rules:
+
+                    .. autoclass:: cylc.flow.unicode_rules.TaskMessageValidator
                 ''')
 
             with Conf('parameter environment templates', desc='''
                 .. deprecated:: 7.8.7/7.9.2
 
                    Parameter environment templates have moved to
                    :cylc:conf:`flow.cylc[runtime][<namespace>][environment]`.
```

### Comparing `cylc-flow-8.1.4/cylc/flow/command_polling.py` & `cylc-flow-8.2.0/cylc/flow/command_polling.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/config.py` & `cylc-flow-8.2.0/cylc/flow/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,35 +55,33 @@
     INTEGER_CYCLING_TYPE, ISO8601_CYCLING_TYPE
 )
 from cylc.flow.id import Tokens
 from cylc.flow.cycling.integer import IntegerInterval
 from cylc.flow.cycling.iso8601 import ingest_time, ISO8601Interval
 from cylc.flow.exceptions import (
     CylcError,
-    WorkflowConfigError,
+    InputError,
     IntervalParsingError,
-    TaskDefError,
     ParamExpandError,
-    InputError
+    TaskDefError,
+    WorkflowConfigError,
 )
 import cylc.flow.flags
 from cylc.flow.graph_parser import GraphParser
 from cylc.flow.listify import listify
 from cylc.flow.option_parsers import verbosity_to_env
 from cylc.flow.graphnode import GraphNodeParser
 from cylc.flow.param_expand import NameExpander
 from cylc.flow.parsec.exceptions import ItemNotFoundError
 from cylc.flow.parsec.OrderedDict import OrderedDictWithDefaults
 from cylc.flow.parsec.util import replicate
 from cylc.flow.pathutil import (
-    get_workflow_run_dir,
-    get_workflow_run_scheduler_log_dir,
-    get_workflow_run_share_dir,
-    get_workflow_run_work_dir,
-    get_workflow_name_from_id
+    get_workflow_name_from_id,
+    get_cylc_run_dir,
+    is_relative_to,
 )
 from cylc.flow.platforms import FORBIDDEN_WITH_PLATFORM
 from cylc.flow.print_tree import print_tree
 from cylc.flow.subprocctx import SubFuncContext
 from cylc.flow.task_events_mgr import (
     EventData,
     get_event_handler_data
@@ -94,14 +92,15 @@
     TaskOutputs
 )
 from cylc.flow.task_trigger import TaskTrigger, Dependency
 from cylc.flow.taskdef import TaskDef
 from cylc.flow.unicode_rules import (
     TaskNameValidator,
     TaskOutputValidator,
+    TaskMessageValidator,
     XtriggerNameValidator,
 )
 from cylc.flow.wallclock import (
     get_current_time_string, set_utc_mode, get_utc_mode)
 from cylc.flow.workflow_files import (
     NO_TITLE,
     WorkflowFiles,
@@ -109,26 +108,26 @@
 )
 from cylc.flow.xtrigger_mgr import XtriggerManager
 
 if TYPE_CHECKING:
     from optparse import Values
     from cylc.flow.cycling import IntervalBase, PointBase, SequenceBase
 
-
 RE_CLOCK_OFFSET = re.compile(
     rf'''
         ^
         \s*
         ({TaskID.NAME_RE})   # task name
         (?:\(\s*(.+)\s*\))?  # optional (arguments, ...)
         \s*
         $
     ''',
     re.X,
 )
+
 RE_EXT_TRIGGER = re.compile(
     r'''
         ^
         \s*
         (.*)            # task name
         \s*
         \(\s*(.+)\s*\)  # required (arguments, ...)
@@ -206,14 +205,16 @@
         'foo'
         >>> dequote("'foo'")
         'foo'
         >>> dequote('foo')
         'foo'
         >>> dequote('"f')
         '"f'
+        >>> dequote('f')
+        'f'
 
     """
     if len(string) < 2:
         return string
     if (string[0] == string[-1]) and string.startswith(("'", '"')):
         return string[1:-1]
     return string
@@ -236,35 +237,41 @@
         xtrigger_mgr: Optional[XtriggerManager] = None,
         mem_log_func: Optional[Callable[[str], None]] = None,
         run_dir: Optional[str] = None,
         log_dir: Optional[str] = None,
         work_dir: Optional[str] = None,
         share_dir: Optional[str] = None
     ) -> None:
+        """
+        Initialize the workflow config object.
+
+        Args:
+            workflow: workflow ID
+            fpath: workflow config file path
+            options: CLI options
+        """
         check_deprecation(Path(fpath))
         self.mem_log = mem_log_func
         if self.mem_log is None:
             self.mem_log = lambda x: None
         self.mem_log("config.py:config.py: start init config")
-        self.workflow = workflow  # workflow id
+        self.workflow = workflow
         self.workflow_name = get_workflow_name_from_id(self.workflow)
-        self.fpath = str(fpath)  # workflow definition
-        self.fdir = os.path.dirname(fpath)
-        self.run_dir = run_dir or get_workflow_run_dir(self.workflow)
-        self.log_dir = (log_dir or
-                        get_workflow_run_scheduler_log_dir(self.workflow))
-        self.share_dir = share_dir or get_workflow_run_share_dir(self.workflow)
-        self.work_dir = work_dir or get_workflow_run_work_dir(self.workflow)
+        self.fpath: Path = Path(fpath)
+        self.fdir = str(self.fpath.parent)
+        self.run_dir = run_dir
+        self.log_dir = log_dir
+        self.share_dir = share_dir
+        self.work_dir = work_dir
         self.options = options
         self.implicit_tasks: Set[str] = set()
         self.edges: Dict[
             'SequenceBase', Set[Tuple[str, str, bool, bool]]
         ] = {}
         self.taskdefs: Dict[str, TaskDef] = {}
-        self.clock_offsets = {}
         self.expiration_offsets = {}
         self.ext_triggers = {}  # Old external triggers (client/server)
         self.xtrigger_mgr = xtrigger_mgr
         self.workflow_polling_tasks = {}  # type: ignore # TODO figure out type
 
         self.initial_point: 'PointBase'
         self.start_point: 'PointBase'
@@ -490,22 +497,18 @@
                 if name in self.runtime['descendants']:
                     result.remove(item)
                     for member in self.runtime['descendants'][name]:
                         if member in self.runtime['descendants']:
                             # (sub-family)
                             continue
                         result.append(member + extn)
-                        if s_type == 'clock-trigger':
-                            self.clock_offsets[member] = offset_interval
                         if s_type == 'clock-expire':
                             self.expiration_offsets[member] = offset_interval
                         if s_type == 'external-trigger':
                             self.ext_triggers[member] = ext_trigger_msg
-                elif s_type == 'clock-trigger':
-                    self.clock_offsets[name] = offset_interval
                 elif s_type == 'clock-expire':
                     self.expiration_offsets[name] = offset_interval
                 elif s_type == 'external-trigger':
                     self.ext_triggers[name] = dequote(ext_trigger_msg)
 
             self.cfg['scheduling']['special tasks'][s_type] = result
 
@@ -544,14 +547,16 @@
                 else:
                     LOG.error(
                         "External trigger '%s'\n  used in tasks %s and %s." % (
                             msg, name, seen[msg]))
                     raise WorkflowConfigError(
                         "external triggers must be used only once.")
 
+        self.upgrade_clock_triggers()
+
         self.leaves = self.get_task_name_list()
         for ancestors in self.runtime['first-parent ancestors'].values():
             try:
                 foot = ancestors[-2]  # one back from 'root'
             except IndexError:
                 pass
             else:
@@ -889,15 +894,15 @@
         if not cylc.flow.flags.cylc7_back_compat:
             msg += (
                 "\nTo allow implicit tasks, use "
                 f"'{WorkflowFiles.FLOW_FILE}[scheduler]allow implicit tasks'"
             )
         # Allow implicit tasks in back-compat mode unless rose-suite.conf
         # present (to maintain compat with Rose 2019)
-        elif not Path(self.run_dir, 'rose-suite.conf').is_file():
+        elif not (self.fpath.parent / "rose-suite.conf").is_file():
             LOG.debug(msg)
             return
 
         raise WorkflowConfigError(msg)
 
     def _check_circular(self):
         """Check for circular dependence in graph."""
@@ -1490,27 +1495,49 @@
                     if tmp > maxlen:
                         maxlen = tmp
             padding = maxlen * ' '
 
         print_tree(tree, padding=padding, use_unicode=pretty)
 
     def process_workflow_env(self):
-        """Workflow context is exported to the local environment."""
+        """Export Workflow context to the local environment.
+
+        A source workflow has only a name.
+        Once installed it also has an ID and a run directory.
+        And at scheduler start-up it has work, share, and log sub-dirs too.
+        """
         for key, value in {
             **verbosity_to_env(cylc.flow.flags.verbosity),
-            'CYLC_WORKFLOW_ID': self.workflow,
             'CYLC_WORKFLOW_NAME': self.workflow_name,
             'CYLC_WORKFLOW_NAME_BASE': str(Path(self.workflow_name).name),
-            'CYLC_WORKFLOW_RUN_DIR': self.run_dir,
-            'CYLC_WORKFLOW_LOG_DIR': self.log_dir,
-            'CYLC_WORKFLOW_WORK_DIR': self.work_dir,
-            'CYLC_WORKFLOW_SHARE_DIR': self.share_dir,
         }.items():
             os.environ[key] = value
 
+        if is_relative_to(self.fdir, get_cylc_run_dir()):
+            # This is an installed workflow.
+            #  - self.run_dir is only defined by the scheduler
+            #  - but the run dir exists, created at installation
+            #  - run sub-dirs may exist, if this installation was run already
+            #    but if the scheduler is not running they shouldn't be used.
+            for key, value in {
+                'CYLC_WORKFLOW_ID': self.workflow,
+                'CYLC_WORKFLOW_RUN_DIR': str(self.fdir),
+            }.items():
+                os.environ[key] = value
+
+        if self.run_dir is not None:
+            # Run directory is only defined if the scheduler is running; in
+            # which case the following run sub-directories must exist.
+            for key, value in {
+                'CYLC_WORKFLOW_LOG_DIR': str(self.log_dir),
+                'CYLC_WORKFLOW_WORK_DIR': str(self.work_dir),
+                'CYLC_WORKFLOW_SHARE_DIR': str(self.share_dir),
+            }.items():
+                os.environ[key] = value
+
     def process_config_env(self):
         """Set local config derived environment."""
         os.environ['CYLC_UTC'] = str(get_utc_mode())
         os.environ['CYLC_WORKFLOW_INITIAL_CYCLE_POINT'] = str(
             self.initial_point
         )
         os.environ['CYLC_WORKFLOW_FINAL_CYCLE_POINT'] = str(self.final_point)
@@ -1735,15 +1762,14 @@
             valid, msg = validator(label)
             if not valid:
                 raise WorkflowConfigError(
                     f'Invalid xtrigger name "{label}" - {msg}'
                 )
 
         for label in xtrig_labels:
-
             try:
                 xtrig = self.cfg['scheduling']['xtriggers'][label]
             except KeyError:
                 if label != 'wall_clock':
                     raise WorkflowConfigError(f"xtrigger not defined: {label}")
                 else:
                     # Allow "@wall_clock" in the graph as an undeclared
@@ -2244,18 +2270,25 @@
                     LOG.error(orig_expr)
                 raise WorkflowConfigError(str(exc))
             else:
                 # Record custom message outputs from [runtime].
                 for output, message in (
                     self.cfg['runtime'][name]['outputs'].items()
                 ):
-                    valid, msg = TaskOutputValidator.validate(message)
+                    valid, msg = TaskOutputValidator.validate(output)
                     if not valid:
                         raise WorkflowConfigError(
-                            f'Invalid message trigger "'
+                            f'Invalid task output "'
+                            f'[runtime][{name}][outputs]'
+                            f'{output} = {message}" - {msg}'
+                        )
+                    valid, msg = TaskMessageValidator.validate(message)
+                    if not valid:
+                        raise WorkflowConfigError(
+                            f'Invalid task message "'
                             f'[runtime][{name}][outputs]'
                             f'{output} = {message}" - {msg}'
                         )
                     self.taskdefs[name].add_output(output, message)
 
         return self.taskdefs[name]
 
@@ -2273,16 +2306,14 @@
         # Get the taskdef object for generating the task proxy class
         taskd = TaskDef(
             name, rtcfg, self.run_mode(), self.start_point,
             self.initial_point)
 
         # TODO - put all taskd.foo items in a single config dict
 
-        if name in self.clock_offsets:
-            taskd.clocktrigger_offset = self.clock_offsets[name]
         if name in self.expiration_offsets:
             taskd.expiration_offset = self.expiration_offsets[name]
         if name in self.ext_triggers:
             taskd.external_triggers.append(self.ext_triggers[name])
 
         taskd.sequential = (
             name in self.cfg['scheduling']['special tasks']['sequential'])
@@ -2425,7 +2456,38 @@
                 '\nsee https://cylc.github.io/cylc-doc/stable/'
                 'html/7-to-8/major-changes/remote-owner.html'
                 f'\nFirst {min(len(owners), 5)} tasks:'
             )
             for task, _ in list(owners.items())[:5]:
                 msg += f'\n  * {task}"'
             raise WorkflowConfigError(msg)
+
+    def upgrade_clock_triggers(self):
+        """Convert old-style clock triggers to clock xtriggers.
+
+        [[special tasks]]
+           clock-trigger = foo(PT1D)
+
+        becomes:
+
+        [[xtriggers]]
+           _cylc_wall_clock_foo = wallclock(PT1D)
+
+        Not done by parsec upgrade because the graph has to be parsed first.
+        """
+        for item in self.cfg['scheduling']['special tasks']['clock-trigger']:
+            match = RE_CLOCK_OFFSET.match(item)
+            # (Already validated during "special tasks" parsing above.)
+            task_name, offset = match.groups()
+            # Derive an xtrigger label.
+            label = '_'.join(('_cylc', 'wall_clock', task_name))
+            # Define the xtrigger function.
+            xtrig = SubFuncContext(label, 'wall_clock', [], {})
+            xtrig.func_kwargs["offset"] = offset
+            if self.xtrigger_mgr is None:
+                XtriggerManager.validate_xtrigger(label, xtrig, self.fdir)
+            else:
+                self.xtrigger_mgr.add_trig(label, xtrig, self.fdir)
+            # Add it to the task, for each sequence that the task appears in.
+            taskdef = self.get_taskdef(task_name)
+            for seq in taskdef.sequences:
+                taskdef.add_xtrig_label(label, seq)
```

### Comparing `cylc-flow-8.1.4/cylc/flow/context_node.py` & `cylc-flow-8.2.0/cylc/flow/context_node.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/cycling/__init__.py` & `cylc-flow-8.2.0/cylc/flow/cycling/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/cycling/integer.py` & `cylc-flow-8.2.0/cylc/flow/cycling/integer.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/cycling/iso8601.py` & `cylc-flow-8.2.0/cylc/flow/cycling/iso8601.py`

 * *Files 1% similar despite different names*

```diff
@@ -540,15 +540,18 @@
                     point, result
                 )
         # Check it is in the exclusions list now
         if result and result in self.exclusions:
             return self.get_next_point_on_sequence(result)
         return result
 
-    def get_first_point(self, point):
+    def get_first_point(
+        self,
+        point: ISO8601Point
+    ) -> Optional[ISO8601Point]:
         """Return the first point >= to point, or None if out of bounds."""
         with contextlib.suppress(KeyError):
             return ISO8601Point(self._cached_first_point_values[point.value])
         p_iso_point = point_parse(point.value)
         for recurrence_iso_point in self.recurrence:
             if recurrence_iso_point >= p_iso_point:
                 first_point_value = str(recurrence_iso_point)
```

### Comparing `cylc-flow-8.1.4/cylc/flow/cycling/loader.py` & `cylc-flow-8.2.0/cylc/flow/cycling/loader.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/cycling/util.py` & `cylc-flow-8.2.0/cylc/flow/cycling/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/cylc_subproc.py` & `cylc-flow-8.2.0/cylc/flow/cylc_subproc.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/daemonize.py` & `cylc-flow-8.2.0/cylc/flow/daemonize.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/data_messages_pb2.py` & `cylc-flow-8.2.0/cylc/flow/data_messages_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # type: ignore
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: data_messages.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x64\x61ta_messages.proto\"\x96\x01\n\x06PbMeta\x12\x12\n\x05title\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x10\n\x03URL\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x19\n\x0cuser_defined\x18\x04 \x01(\tH\x03\x88\x01\x01\x42\x08\n\x06_titleB\x0e\n\x0c_descriptionB\x06\n\x04_URLB\x0f\n\r_user_defined\"\xaa\x01\n\nPbTimeZone\x12\x12\n\x05hours\x18\x01 \x01(\x05H\x00\x88\x01\x01\x12\x14\n\x07minutes\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x19\n\x0cstring_basic\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x1c\n\x0fstring_extended\x18\x04 \x01(\tH\x03\x88\x01\x01\x42\x08\n\x06_hoursB\n\n\x08_minutesB\x0f\n\r_string_basicB\x12\n\x10_string_extended\"\'\n\x0fPbTaskProxyRefs\x12\x14\n\x0ctask_proxies\x18\x01 \x03(\t\"\xf2\x0b\n\nPbWorkflow\x12\x12\n\x05stamp\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x02id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x11\n\x04name\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x13\n\x06status\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x11\n\x04host\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x11\n\x04port\x18\x06 \x01(\x05H\x05\x88\x01\x01\x12\x12\n\x05owner\x18\x07 \x01(\tH\x06\x88\x01\x01\x12\r\n\x05tasks\x18\x08 \x03(\t\x12\x10\n\x08\x66\x61milies\x18\t \x03(\t\x12\x1c\n\x05\x65\x64ges\x18\n \x01(\x0b\x32\x08.PbEdgesH\x07\x88\x01\x01\x12\x18\n\x0b\x61pi_version\x18\x0b \x01(\x05H\x08\x88\x01\x01\x12\x19\n\x0c\x63ylc_version\x18\x0c \x01(\tH\t\x88\x01\x01\x12\x19\n\x0clast_updated\x18\r \x01(\x01H\n\x88\x01\x01\x12\x1a\n\x04meta\x18\x0e \x01(\x0b\x32\x07.PbMetaH\x0b\x88\x01\x01\x12&\n\x19newest_active_cycle_point\x18\x10 \x01(\tH\x0c\x88\x01\x01\x12&\n\x19oldest_active_cycle_point\x18\x11 \x01(\tH\r\x88\x01\x01\x12\x15\n\x08reloaded\x18\x12 \x01(\x08H\x0e\x88\x01\x01\x12\x15\n\x08run_mode\x18\x13 \x01(\tH\x0f\x88\x01\x01\x12\x19\n\x0c\x63ycling_mode\x18\x14 \x01(\tH\x10\x88\x01\x01\x12\x32\n\x0cstate_totals\x18\x15 \x03(\x0b\x32\x1c.PbWorkflow.StateTotalsEntry\x12\x1d\n\x10workflow_log_dir\x18\x16 \x01(\tH\x11\x88\x01\x01\x12(\n\x0etime_zone_info\x18\x17 \x01(\x0b\x32\x0b.PbTimeZoneH\x12\x88\x01\x01\x12\x17\n\ntree_depth\x18\x18 \x01(\x05H\x13\x88\x01\x01\x12\x15\n\rjob_log_names\x18\x19 \x03(\t\x12\x14\n\x0cns_def_order\x18\x1a \x03(\t\x12\x0e\n\x06states\x18\x1b \x03(\t\x12\x14\n\x0ctask_proxies\x18\x1c \x03(\t\x12\x16\n\x0e\x66\x61mily_proxies\x18\x1d \x03(\t\x12\x17\n\nstatus_msg\x18\x1e \x01(\tH\x14\x88\x01\x01\x12\x1a\n\ris_held_total\x18\x1f \x01(\x05H\x15\x88\x01\x01\x12\x0c\n\x04jobs\x18  \x03(\t\x12\x15\n\x08pub_port\x18! \x01(\x05H\x16\x88\x01\x01\x12\x17\n\nbroadcasts\x18\" \x01(\tH\x17\x88\x01\x01\x12\x1c\n\x0fis_queued_total\x18# \x01(\x05H\x18\x88\x01\x01\x12=\n\x12latest_state_tasks\x18$ \x03(\x0b\x32!.PbWorkflow.LatestStateTasksEntry\x12\x13\n\x06pruned\x18% \x01(\x08H\x19\x88\x01\x01\x12\x1e\n\x11is_runahead_total\x18& \x01(\x05H\x1a\x88\x01\x01\x1a\x32\n\x10StateTotalsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\x1aI\n\x15LatestStateTasksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1f\n\x05value\x18\x02 \x01(\x0b\x32\x10.PbTaskProxyRefs:\x02\x38\x01\x42\x08\n\x06_stampB\x05\n\x03_idB\x07\n\x05_nameB\t\n\x07_statusB\x07\n\x05_hostB\x07\n\x05_portB\x08\n\x06_ownerB\x08\n\x06_edgesB\x0e\n\x0c_api_versionB\x0f\n\r_cylc_versionB\x0f\n\r_last_updatedB\x07\n\x05_metaB\x1c\n\x1a_newest_active_cycle_pointB\x1c\n\x1a_oldest_active_cycle_pointB\x0b\n\t_reloadedB\x0b\n\t_run_modeB\x0f\n\r_cycling_modeB\x13\n\x11_workflow_log_dirB\x11\n\x0f_time_zone_infoB\r\n\x0b_tree_depthB\r\n\x0b_status_msgB\x10\n\x0e_is_held_totalB\x0b\n\t_pub_portB\r\n\x0b_broadcastsB\x12\n\x10_is_queued_totalB\t\n\x07_prunedB\x14\n\x12_is_runahead_total\"\xb9\x06\n\tPbRuntime\x12\x15\n\x08platform\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x13\n\x06script\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x18\n\x0binit_script\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x17\n\nenv_script\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x17\n\nerr_script\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x18\n\x0b\x65xit_script\x18\x06 \x01(\tH\x05\x88\x01\x01\x12\x17\n\npre_script\x18\x07 \x01(\tH\x06\x88\x01\x01\x12\x18\n\x0bpost_script\x18\x08 \x01(\tH\x07\x88\x01\x01\x12\x19\n\x0cwork_sub_dir\x18\t \x01(\tH\x08\x88\x01\x01\x12(\n\x1b\x65xecution_polling_intervals\x18\n \x01(\tH\t\x88\x01\x01\x12#\n\x16\x65xecution_retry_delays\x18\x0b \x01(\tH\n\x88\x01\x01\x12!\n\x14\x65xecution_time_limit\x18\x0c \x01(\tH\x0b\x88\x01\x01\x12)\n\x1csubmission_polling_intervals\x18\r \x01(\tH\x0c\x88\x01\x01\x12$\n\x17submission_retry_delays\x18\x0e \x01(\tH\r\x88\x01\x01\x12\x17\n\ndirectives\x18\x0f \x01(\tH\x0e\x88\x01\x01\x12\x18\n\x0b\x65nvironment\x18\x10 \x01(\tH\x0f\x88\x01\x01\x12\x14\n\x07outputs\x18\x11 \x01(\tH\x10\x88\x01\x01\x42\x0b\n\t_platformB\t\n\x07_scriptB\x0e\n\x0c_init_scriptB\r\n\x0b_env_scriptB\r\n\x0b_err_scriptB\x0e\n\x0c_exit_scriptB\r\n\x0b_pre_scriptB\x0e\n\x0c_post_scriptB\x0f\n\r_work_sub_dirB\x1e\n\x1c_execution_polling_intervalsB\x19\n\x17_execution_retry_delaysB\x17\n\x15_execution_time_limitB\x1f\n\x1d_submission_polling_intervalsB\x1a\n\x18_submission_retry_delaysB\r\n\x0b_directivesB\x0e\n\x0c_environmentB\n\n\x08_outputs\"\xab\x05\n\x05PbJob\x12\x12\n\x05stamp\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x02id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x17\n\nsubmit_num\x18\x03 \x01(\x05H\x02\x88\x01\x01\x12\x12\n\x05state\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x17\n\ntask_proxy\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x1b\n\x0esubmitted_time\x18\x06 \x01(\tH\x05\x88\x01\x01\x12\x19\n\x0cstarted_time\x18\x07 \x01(\tH\x06\x88\x01\x01\x12\x1a\n\rfinished_time\x18\x08 \x01(\tH\x07\x88\x01\x01\x12\x13\n\x06job_id\x18\t \x01(\tH\x08\x88\x01\x01\x12\x1c\n\x0fjob_runner_name\x18\n \x01(\tH\t\x88\x01\x01\x12!\n\x14\x65xecution_time_limit\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x15\n\x08platform\x18\x0f \x01(\tH\x0b\x88\x01\x01\x12\x18\n\x0bjob_log_dir\x18\x11 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\nextra_logs\x18\x1d \x03(\t\x12\x11\n\x04name\x18\x1e \x01(\tH\r\x88\x01\x01\x12\x18\n\x0b\x63ycle_point\x18\x1f \x01(\tH\x0e\x88\x01\x01\x12\x10\n\x08messages\x18  \x03(\t\x12 \n\x07runtime\x18! \x01(\x0b\x32\n.PbRuntimeH\x0f\x88\x01\x01\x42\x08\n\x06_stampB\x05\n\x03_idB\r\n\x0b_submit_numB\x08\n\x06_stateB\r\n\x0b_task_proxyB\x11\n\x0f_submitted_timeB\x0f\n\r_started_timeB\x10\n\x0e_finished_timeB\t\n\x07_job_idB\x12\n\x10_job_runner_nameB\x17\n\x15_execution_time_limitB\x0b\n\t_platformB\x0e\n\x0c_job_log_dirB\x07\n\x05_nameB\x0e\n\x0c_cycle_pointB\n\n\x08_runtime\"\xe2\x02\n\x06PbTask\x12\x12\n\x05stamp\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x02id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x11\n\x04name\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x1a\n\x04meta\x18\x04 \x01(\x0b\x32\x07.PbMetaH\x03\x88\x01\x01\x12\x1e\n\x11mean_elapsed_time\x18\x05 \x01(\x02H\x04\x88\x01\x01\x12\x12\n\x05\x64\x65pth\x18\x06 \x01(\x05H\x05\x88\x01\x01\x12\x0f\n\x07proxies\x18\x07 \x03(\t\x12\x11\n\tnamespace\x18\x08 \x03(\t\x12\x0f\n\x07parents\x18\t \x03(\t\x12\x19\n\x0c\x66irst_parent\x18\n \x01(\tH\x06\x88\x01\x01\x12 \n\x07runtime\x18\x0b \x01(\x0b\x32\n.PbRuntimeH\x07\x88\x01\x01\x42\x08\n\x06_stampB\x05\n\x03_idB\x07\n\x05_nameB\x07\n\x05_metaB\x14\n\x12_mean_elapsed_timeB\x08\n\x06_depthB\x0f\n\r_first_parentB\n\n\x08_runtime\"\xd8\x01\n\nPbPollTask\x12\x18\n\x0blocal_proxy\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x15\n\x08workflow\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x19\n\x0cremote_proxy\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x16\n\treq_state\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x19\n\x0cgraph_string\x18\x05 \x01(\tH\x04\x88\x01\x01\x42\x0e\n\x0c_local_proxyB\x0b\n\t_workflowB\x0f\n\r_remote_proxyB\x0c\n\n_req_stateB\x0f\n\r_graph_string\"\xcb\x01\n\x0bPbCondition\x12\x17\n\ntask_proxy\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x17\n\nexpr_alias\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x16\n\treq_state\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x16\n\tsatisfied\x18\x04 \x01(\x08H\x03\x88\x01\x01\x12\x14\n\x07message\x18\x05 \x01(\tH\x04\x88\x01\x01\x42\r\n\x0b_task_proxyB\r\n\x0b_expr_aliasB\x0c\n\n_req_stateB\x0c\n\n_satisfiedB\n\n\x08_message\"\x96\x01\n\x0ePbPrerequisite\x12\x17\n\nexpression\x18\x01 \x01(\tH\x00\x88\x01\x01\x12 \n\nconditions\x18\x02 \x03(\x0b\x32\x0c.PbCondition\x12\x14\n\x0c\x63ycle_points\x18\x03 \x03(\t\x12\x16\n\tsatisfied\x18\x04 \x01(\x08H\x01\x88\x01\x01\x42\r\n\x0b_expressionB\x0c\n\n_satisfied\"\x8c\x01\n\x08PbOutput\x12\x12\n\x05label\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x14\n\x07message\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x16\n\tsatisfied\x18\x03 \x01(\x08H\x02\x88\x01\x01\x12\x11\n\x04time\x18\x04 \x01(\x01H\x03\x88\x01\x01\x42\x08\n\x06_labelB\n\n\x08_messageB\x0c\n\n_satisfiedB\x07\n\x05_time\"|\n\x0ePbClockTrigger\x12\x11\n\x04time\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x18\n\x0btime_string\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x16\n\tsatisfied\x18\x03 \x01(\x08H\x02\x88\x01\x01\x42\x07\n\x05_timeB\x0e\n\x0c_time_stringB\x0c\n\n_satisfied\"\xa5\x01\n\tPbTrigger\x12\x0f\n\x02id\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x12\n\x05label\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x14\n\x07message\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x16\n\tsatisfied\x18\x04 \x01(\x08H\x03\x88\x01\x01\x12\x11\n\x04time\x18\x05 \x01(\x01H\x04\x88\x01\x01\x42\x05\n\x03_idB\x08\n\x06_labelB\n\n\x08_messageB\x0c\n\n_satisfiedB\x07\n\x05_time\"\xa6\x08\n\x0bPbTaskProxy\x12\x12\n\x05stamp\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x02id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x11\n\x04task\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x12\n\x05state\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x18\n\x0b\x63ycle_point\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x12\n\x05\x64\x65pth\x18\x06 \x01(\x05H\x05\x88\x01\x01\x12\x18\n\x0bjob_submits\x18\x07 \x01(\x05H\x06\x88\x01\x01\x12*\n\x07outputs\x18\t \x03(\x0b\x32\x19.PbTaskProxy.OutputsEntry\x12\x11\n\tnamespace\x18\x0b \x03(\t\x12&\n\rprerequisites\x18\x0c \x03(\x0b\x32\x0f.PbPrerequisite\x12\x0c\n\x04jobs\x18\r \x03(\t\x12\x19\n\x0c\x66irst_parent\x18\x0f \x01(\tH\x07\x88\x01\x01\x12\x11\n\x04name\x18\x10 \x01(\tH\x08\x88\x01\x01\x12\x14\n\x07is_held\x18\x11 \x01(\x08H\t\x88\x01\x01\x12\r\n\x05\x65\x64ges\x18\x12 \x03(\t\x12\x11\n\tancestors\x18\x13 \x03(\t\x12\x16\n\tflow_nums\x18\x14 \x01(\tH\n\x88\x01\x01\x12+\n\rclock_trigger\x18\x16 \x01(\x0b\x32\x0f.PbClockTriggerH\x0b\x88\x01\x01\x12=\n\x11\x65xternal_triggers\x18\x17 \x03(\x0b\x32\".PbTaskProxy.ExternalTriggersEntry\x12.\n\txtriggers\x18\x18 \x03(\x0b\x32\x1b.PbTaskProxy.XtriggersEntry\x12\x16\n\tis_queued\x18\x19 \x01(\x08H\x0c\x88\x01\x01\x12\x18\n\x0bis_runahead\x18\x1a \x01(\x08H\r\x88\x01\x01\x12\x16\n\tflow_wait\x18\x1b \x01(\x08H\x0e\x88\x01\x01\x12 \n\x07runtime\x18\x1c \x01(\x0b\x32\n.PbRuntimeH\x0f\x88\x01\x01\x1a\x39\n\x0cOutputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.PbOutput:\x02\x38\x01\x1a\x43\n\x15\x45xternalTriggersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x19\n\x05value\x18\x02 \x01(\x0b\x32\n.PbTrigger:\x02\x38\x01\x1a<\n\x0eXtriggersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x19\n\x05value\x18\x02 \x01(\x0b\x32\n.PbTrigger:\x02\x38\x01\x42\x08\n\x06_stampB\x05\n\x03_idB\x07\n\x05_taskB\x08\n\x06_stateB\x0e\n\x0c_cycle_pointB\x08\n\x06_depthB\x0e\n\x0c_job_submitsB\x0f\n\r_first_parentB\x07\n\x05_nameB\n\n\x08_is_heldB\x0c\n\n_flow_numsB\x10\n\x0e_clock_triggerB\x0c\n\n_is_queuedB\x0e\n\x0c_is_runaheadB\x0c\n\n_flow_waitB\n\n\x08_runtime\"\xc8\x02\n\x08PbFamily\x12\x12\n\x05stamp\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x02id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x11\n\x04name\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x1a\n\x04meta\x18\x04 \x01(\x0b\x32\x07.PbMetaH\x03\x88\x01\x01\x12\x12\n\x05\x64\x65pth\x18\x05 \x01(\x05H\x04\x88\x01\x01\x12\x0f\n\x07proxies\x18\x06 \x03(\t\x12\x0f\n\x07parents\x18\x07 \x03(\t\x12\x13\n\x0b\x63hild_tasks\x18\x08 \x03(\t\x12\x16\n\x0e\x63hild_families\x18\t \x03(\t\x12\x19\n\x0c\x66irst_parent\x18\n \x01(\tH\x05\x88\x01\x01\x12 \n\x07runtime\x18\x0b \x01(\x0b\x32\n.PbRuntimeH\x06\x88\x01\x01\x42\x08\n\x06_stampB\x05\n\x03_idB\x07\n\x05_nameB\x07\n\x05_metaB\x08\n\x06_depthB\x0f\n\r_first_parentB\n\n\x08_runtime\"\x84\x06\n\rPbFamilyProxy\x12\x12\n\x05stamp\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x02id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x18\n\x0b\x63ycle_point\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x11\n\x04name\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x13\n\x06\x66\x61mily\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x12\n\x05state\x18\x06 \x01(\tH\x05\x88\x01\x01\x12\x12\n\x05\x64\x65pth\x18\x07 \x01(\x05H\x06\x88\x01\x01\x12\x19\n\x0c\x66irst_parent\x18\x08 \x01(\tH\x07\x88\x01\x01\x12\x13\n\x0b\x63hild_tasks\x18\n \x03(\t\x12\x16\n\x0e\x63hild_families\x18\x0b \x03(\t\x12\x14\n\x07is_held\x18\x0c \x01(\x08H\x08\x88\x01\x01\x12\x11\n\tancestors\x18\r \x03(\t\x12\x0e\n\x06states\x18\x0e \x03(\t\x12\x35\n\x0cstate_totals\x18\x0f \x03(\x0b\x32\x1f.PbFamilyProxy.StateTotalsEntry\x12\x1a\n\ris_held_total\x18\x10 \x01(\x05H\t\x88\x01\x01\x12\x16\n\tis_queued\x18\x11 \x01(\x08H\n\x88\x01\x01\x12\x1c\n\x0fis_queued_total\x18\x12 \x01(\x05H\x0b\x88\x01\x01\x12\x18\n\x0bis_runahead\x18\x13 \x01(\x08H\x0c\x88\x01\x01\x12\x1e\n\x11is_runahead_total\x18\x14 \x01(\x05H\r\x88\x01\x01\x12 \n\x07runtime\x18\x15 \x01(\x0b\x32\n.PbRuntimeH\x0e\x88\x01\x01\x1a\x32\n\x10StateTotalsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\x42\x08\n\x06_stampB\x05\n\x03_idB\x0e\n\x0c_cycle_pointB\x07\n\x05_nameB\t\n\x07_familyB\x08\n\x06_stateB\x08\n\x06_depthB\x0f\n\r_first_parentB\n\n\x08_is_heldB\x10\n\x0e_is_held_totalB\x0c\n\n_is_queuedB\x12\n\x10_is_queued_totalB\x0e\n\x0c_is_runaheadB\x14\n\x12_is_runahead_totalB\n\n\x08_runtime\"\xbc\x01\n\x06PbEdge\x12\x12\n\x05stamp\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x02id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x13\n\x06source\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x13\n\x06target\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x14\n\x07suicide\x18\x05 \x01(\x08H\x04\x88\x01\x01\x12\x11\n\x04\x63ond\x18\x06 \x01(\x08H\x05\x88\x01\x01\x42\x08\n\x06_stampB\x05\n\x03_idB\t\n\x07_sourceB\t\n\x07_targetB\n\n\x08_suicideB\x07\n\x05_cond\"{\n\x07PbEdges\x12\x0f\n\x02id\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\r\n\x05\x65\x64ges\x18\x02 \x03(\t\x12+\n\x16workflow_polling_tasks\x18\x03 \x03(\x0b\x32\x0b.PbPollTask\x12\x0e\n\x06leaves\x18\x04 \x03(\t\x12\x0c\n\x04\x66\x65\x65t\x18\x05 \x03(\tB\x05\n\x03_id\"\xf2\x01\n\x10PbEntireWorkflow\x12\"\n\x08workflow\x18\x01 \x01(\x0b\x32\x0b.PbWorkflowH\x00\x88\x01\x01\x12\x16\n\x05tasks\x18\x02 \x03(\x0b\x32\x07.PbTask\x12\"\n\x0ctask_proxies\x18\x03 \x03(\x0b\x32\x0c.PbTaskProxy\x12\x14\n\x04jobs\x18\x04 \x03(\x0b\x32\x06.PbJob\x12\x1b\n\x08\x66\x61milies\x18\x05 \x03(\x0b\x32\t.PbFamily\x12&\n\x0e\x66\x61mily_proxies\x18\x06 \x03(\x0b\x32\x0e.PbFamilyProxy\x12\x16\n\x05\x65\x64ges\x18\x07 \x03(\x0b\x32\x07.PbEdgeB\x0b\n\t_workflow\"\xaf\x01\n\x07\x45\x44\x65ltas\x12\x11\n\x04time\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x63hecksum\x18\x02 \x01(\x03H\x01\x88\x01\x01\x12\x16\n\x05\x61\x64\x64\x65\x64\x18\x03 \x03(\x0b\x32\x07.PbEdge\x12\x18\n\x07updated\x18\x04 \x03(\x0b\x32\x07.PbEdge\x12\x0e\n\x06pruned\x18\x05 \x03(\t\x12\x15\n\x08reloaded\x18\x06 \x01(\x08H\x02\x88\x01\x01\x42\x07\n\x05_timeB\x0b\n\t_checksumB\x0b\n\t_reloaded\"\xb3\x01\n\x07\x46\x44\x65ltas\x12\x11\n\x04time\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x63hecksum\x18\x02 \x01(\x03H\x01\x88\x01\x01\x12\x18\n\x05\x61\x64\x64\x65\x64\x18\x03 \x03(\x0b\x32\t.PbFamily\x12\x1a\n\x07updated\x18\x04 \x03(\x0b\x32\t.PbFamily\x12\x0e\n\x06pruned\x18\x05 \x03(\t\x12\x15\n\x08reloaded\x18\x06 \x01(\x08H\x02\x88\x01\x01\x42\x07\n\x05_timeB\x0b\n\t_checksumB\x0b\n\t_reloaded\"\xbe\x01\n\x08\x46PDeltas\x12\x11\n\x04time\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x63hecksum\x18\x02 \x01(\x03H\x01\x88\x01\x01\x12\x1d\n\x05\x61\x64\x64\x65\x64\x18\x03 \x03(\x0b\x32\x0e.PbFamilyProxy\x12\x1f\n\x07updated\x18\x04 \x03(\x0b\x32\x0e.PbFamilyProxy\x12\x0e\n\x06pruned\x18\x05 \x03(\t\x12\x15\n\x08reloaded\x18\x06 \x01(\x08H\x02\x88\x01\x01\x42\x07\n\x05_timeB\x0b\n\t_checksumB\x0b\n\t_reloaded\"\xad\x01\n\x07JDeltas\x12\x11\n\x04time\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x63hecksum\x18\x02 \x01(\x03H\x01\x88\x01\x01\x12\x15\n\x05\x61\x64\x64\x65\x64\x18\x03 \x03(\x0b\x32\x06.PbJob\x12\x17\n\x07updated\x18\x04 \x03(\x0b\x32\x06.PbJob\x12\x0e\n\x06pruned\x18\x05 \x03(\t\x12\x15\n\x08reloaded\x18\x06 \x01(\x08H\x02\x88\x01\x01\x42\x07\n\x05_timeB\x0b\n\t_checksumB\x0b\n\t_reloaded\"\xaf\x01\n\x07TDeltas\x12\x11\n\x04time\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x63hecksum\x18\x02 \x01(\x03H\x01\x88\x01\x01\x12\x16\n\x05\x61\x64\x64\x65\x64\x18\x03 \x03(\x0b\x32\x07.PbTask\x12\x18\n\x07updated\x18\x04 \x03(\x0b\x32\x07.PbTask\x12\x0e\n\x06pruned\x18\x05 \x03(\t\x12\x15\n\x08reloaded\x18\x06 \x01(\x08H\x02\x88\x01\x01\x42\x07\n\x05_timeB\x0b\n\t_checksumB\x0b\n\t_reloaded\"\xba\x01\n\x08TPDeltas\x12\x11\n\x04time\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x63hecksum\x18\x02 \x01(\x03H\x01\x88\x01\x01\x12\x1b\n\x05\x61\x64\x64\x65\x64\x18\x03 \x03(\x0b\x32\x0c.PbTaskProxy\x12\x1d\n\x07updated\x18\x04 \x03(\x0b\x32\x0c.PbTaskProxy\x12\x0e\n\x06pruned\x18\x05 \x03(\t\x12\x15\n\x08reloaded\x18\x06 \x01(\x08H\x02\x88\x01\x01\x42\x07\n\x05_timeB\x0b\n\t_checksumB\x0b\n\t_reloaded\"\xc3\x01\n\x07WDeltas\x12\x11\n\x04time\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x1f\n\x05\x61\x64\x64\x65\x64\x18\x02 \x01(\x0b\x32\x0b.PbWorkflowH\x01\x88\x01\x01\x12!\n\x07updated\x18\x03 \x01(\x0b\x32\x0b.PbWorkflowH\x02\x88\x01\x01\x12\x15\n\x08reloaded\x18\x04 \x01(\x08H\x03\x88\x01\x01\x12\x13\n\x06pruned\x18\x05 \x01(\tH\x04\x88\x01\x01\x42\x07\n\x05_timeB\x08\n\x06_addedB\n\n\x08_updatedB\x0b\n\t_reloadedB\t\n\x07_pruned\"\xd1\x01\n\tAllDeltas\x12\x1a\n\x08\x66\x61milies\x18\x01 \x01(\x0b\x32\x08.FDeltas\x12!\n\x0e\x66\x61mily_proxies\x18\x02 \x01(\x0b\x32\t.FPDeltas\x12\x16\n\x04jobs\x18\x03 \x01(\x0b\x32\x08.JDeltas\x12\x17\n\x05tasks\x18\x04 \x01(\x0b\x32\x08.TDeltas\x12\x1f\n\x0ctask_proxies\x18\x05 \x01(\x0b\x32\t.TPDeltas\x12\x17\n\x05\x65\x64ges\x18\x06 \x01(\x0b\x32\x08.EDeltas\x12\x1a\n\x08workflow\x18\x07 \x01(\x0b\x32\x08.WDeltasb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x64\x61ta_messages.proto\"\x96\x01\n\x06PbMeta\x12\x12\n\x05title\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x10\n\x03URL\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x19\n\x0cuser_defined\x18\x04 \x01(\tH\x03\x88\x01\x01\x42\x08\n\x06_titleB\x0e\n\x0c_descriptionB\x06\n\x04_URLB\x0f\n\r_user_defined\"\xaa\x01\n\nPbTimeZone\x12\x12\n\x05hours\x18\x01 \x01(\x05H\x00\x88\x01\x01\x12\x14\n\x07minutes\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x19\n\x0cstring_basic\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x1c\n\x0fstring_extended\x18\x04 \x01(\tH\x03\x88\x01\x01\x42\x08\n\x06_hoursB\n\n\x08_minutesB\x0f\n\r_string_basicB\x12\n\x10_string_extended\"\'\n\x0fPbTaskProxyRefs\x12\x14\n\x0ctask_proxies\x18\x01 \x03(\t\"\xa2\x0c\n\nPbWorkflow\x12\x12\n\x05stamp\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x02id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x11\n\x04name\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x13\n\x06status\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x11\n\x04host\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x11\n\x04port\x18\x06 \x01(\x05H\x05\x88\x01\x01\x12\x12\n\x05owner\x18\x07 \x01(\tH\x06\x88\x01\x01\x12\r\n\x05tasks\x18\x08 \x03(\t\x12\x10\n\x08\x66\x61milies\x18\t \x03(\t\x12\x1c\n\x05\x65\x64ges\x18\n \x01(\x0b\x32\x08.PbEdgesH\x07\x88\x01\x01\x12\x18\n\x0b\x61pi_version\x18\x0b \x01(\x05H\x08\x88\x01\x01\x12\x19\n\x0c\x63ylc_version\x18\x0c \x01(\tH\t\x88\x01\x01\x12\x19\n\x0clast_updated\x18\r \x01(\x01H\n\x88\x01\x01\x12\x1a\n\x04meta\x18\x0e \x01(\x0b\x32\x07.PbMetaH\x0b\x88\x01\x01\x12&\n\x19newest_active_cycle_point\x18\x10 \x01(\tH\x0c\x88\x01\x01\x12&\n\x19oldest_active_cycle_point\x18\x11 \x01(\tH\r\x88\x01\x01\x12\x15\n\x08reloaded\x18\x12 \x01(\x08H\x0e\x88\x01\x01\x12\x15\n\x08run_mode\x18\x13 \x01(\tH\x0f\x88\x01\x01\x12\x19\n\x0c\x63ycling_mode\x18\x14 \x01(\tH\x10\x88\x01\x01\x12\x32\n\x0cstate_totals\x18\x15 \x03(\x0b\x32\x1c.PbWorkflow.StateTotalsEntry\x12\x1d\n\x10workflow_log_dir\x18\x16 \x01(\tH\x11\x88\x01\x01\x12(\n\x0etime_zone_info\x18\x17 \x01(\x0b\x32\x0b.PbTimeZoneH\x12\x88\x01\x01\x12\x17\n\ntree_depth\x18\x18 \x01(\x05H\x13\x88\x01\x01\x12\x15\n\rjob_log_names\x18\x19 \x03(\t\x12\x14\n\x0cns_def_order\x18\x1a \x03(\t\x12\x0e\n\x06states\x18\x1b \x03(\t\x12\x14\n\x0ctask_proxies\x18\x1c \x03(\t\x12\x16\n\x0e\x66\x61mily_proxies\x18\x1d \x03(\t\x12\x17\n\nstatus_msg\x18\x1e \x01(\tH\x14\x88\x01\x01\x12\x1a\n\ris_held_total\x18\x1f \x01(\x05H\x15\x88\x01\x01\x12\x0c\n\x04jobs\x18  \x03(\t\x12\x15\n\x08pub_port\x18! \x01(\x05H\x16\x88\x01\x01\x12\x17\n\nbroadcasts\x18\" \x01(\tH\x17\x88\x01\x01\x12\x1c\n\x0fis_queued_total\x18# \x01(\x05H\x18\x88\x01\x01\x12=\n\x12latest_state_tasks\x18$ \x03(\x0b\x32!.PbWorkflow.LatestStateTasksEntry\x12\x13\n\x06pruned\x18% \x01(\x08H\x19\x88\x01\x01\x12\x1e\n\x11is_runahead_total\x18& \x01(\x05H\x1a\x88\x01\x01\x12\x1b\n\x0estates_updated\x18\' \x01(\x08H\x1b\x88\x01\x01\x1a\x32\n\x10StateTotalsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\x1aI\n\x15LatestStateTasksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1f\n\x05value\x18\x02 \x01(\x0b\x32\x10.PbTaskProxyRefs:\x02\x38\x01\x42\x08\n\x06_stampB\x05\n\x03_idB\x07\n\x05_nameB\t\n\x07_statusB\x07\n\x05_hostB\x07\n\x05_portB\x08\n\x06_ownerB\x08\n\x06_edgesB\x0e\n\x0c_api_versionB\x0f\n\r_cylc_versionB\x0f\n\r_last_updatedB\x07\n\x05_metaB\x1c\n\x1a_newest_active_cycle_pointB\x1c\n\x1a_oldest_active_cycle_pointB\x0b\n\t_reloadedB\x0b\n\t_run_modeB\x0f\n\r_cycling_modeB\x13\n\x11_workflow_log_dirB\x11\n\x0f_time_zone_infoB\r\n\x0b_tree_depthB\r\n\x0b_status_msgB\x10\n\x0e_is_held_totalB\x0b\n\t_pub_portB\r\n\x0b_broadcastsB\x12\n\x10_is_queued_totalB\t\n\x07_prunedB\x14\n\x12_is_runahead_totalB\x11\n\x0f_states_updated\"\xb9\x06\n\tPbRuntime\x12\x15\n\x08platform\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x13\n\x06script\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x18\n\x0binit_script\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x17\n\nenv_script\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x17\n\nerr_script\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x18\n\x0b\x65xit_script\x18\x06 \x01(\tH\x05\x88\x01\x01\x12\x17\n\npre_script\x18\x07 \x01(\tH\x06\x88\x01\x01\x12\x18\n\x0bpost_script\x18\x08 \x01(\tH\x07\x88\x01\x01\x12\x19\n\x0cwork_sub_dir\x18\t \x01(\tH\x08\x88\x01\x01\x12(\n\x1b\x65xecution_polling_intervals\x18\n \x01(\tH\t\x88\x01\x01\x12#\n\x16\x65xecution_retry_delays\x18\x0b \x01(\tH\n\x88\x01\x01\x12!\n\x14\x65xecution_time_limit\x18\x0c \x01(\tH\x0b\x88\x01\x01\x12)\n\x1csubmission_polling_intervals\x18\r \x01(\tH\x0c\x88\x01\x01\x12$\n\x17submission_retry_delays\x18\x0e \x01(\tH\r\x88\x01\x01\x12\x17\n\ndirectives\x18\x0f \x01(\tH\x0e\x88\x01\x01\x12\x18\n\x0b\x65nvironment\x18\x10 \x01(\tH\x0f\x88\x01\x01\x12\x14\n\x07outputs\x18\x11 \x01(\tH\x10\x88\x01\x01\x42\x0b\n\t_platformB\t\n\x07_scriptB\x0e\n\x0c_init_scriptB\r\n\x0b_env_scriptB\r\n\x0b_err_scriptB\x0e\n\x0c_exit_scriptB\r\n\x0b_pre_scriptB\x0e\n\x0c_post_scriptB\x0f\n\r_work_sub_dirB\x1e\n\x1c_execution_polling_intervalsB\x19\n\x17_execution_retry_delaysB\x17\n\x15_execution_time_limitB\x1f\n\x1d_submission_polling_intervalsB\x1a\n\x18_submission_retry_delaysB\r\n\x0b_directivesB\x0e\n\x0c_environmentB\n\n\x08_outputs\"\xab\x05\n\x05PbJob\x12\x12\n\x05stamp\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x02id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x17\n\nsubmit_num\x18\x03 \x01(\x05H\x02\x88\x01\x01\x12\x12\n\x05state\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x17\n\ntask_proxy\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x1b\n\x0esubmitted_time\x18\x06 \x01(\tH\x05\x88\x01\x01\x12\x19\n\x0cstarted_time\x18\x07 \x01(\tH\x06\x88\x01\x01\x12\x1a\n\rfinished_time\x18\x08 \x01(\tH\x07\x88\x01\x01\x12\x13\n\x06job_id\x18\t \x01(\tH\x08\x88\x01\x01\x12\x1c\n\x0fjob_runner_name\x18\n \x01(\tH\t\x88\x01\x01\x12!\n\x14\x65xecution_time_limit\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x15\n\x08platform\x18\x0f \x01(\tH\x0b\x88\x01\x01\x12\x18\n\x0bjob_log_dir\x18\x11 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\nextra_logs\x18\x1d \x03(\t\x12\x11\n\x04name\x18\x1e \x01(\tH\r\x88\x01\x01\x12\x18\n\x0b\x63ycle_point\x18\x1f \x01(\tH\x0e\x88\x01\x01\x12\x10\n\x08messages\x18  \x03(\t\x12 \n\x07runtime\x18! \x01(\x0b\x32\n.PbRuntimeH\x0f\x88\x01\x01\x42\x08\n\x06_stampB\x05\n\x03_idB\r\n\x0b_submit_numB\x08\n\x06_stateB\r\n\x0b_task_proxyB\x11\n\x0f_submitted_timeB\x0f\n\r_started_timeB\x10\n\x0e_finished_timeB\t\n\x07_job_idB\x12\n\x10_job_runner_nameB\x17\n\x15_execution_time_limitB\x0b\n\t_platformB\x0e\n\x0c_job_log_dirB\x07\n\x05_nameB\x0e\n\x0c_cycle_pointB\n\n\x08_runtime\"\xe2\x02\n\x06PbTask\x12\x12\n\x05stamp\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x02id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x11\n\x04name\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x1a\n\x04meta\x18\x04 \x01(\x0b\x32\x07.PbMetaH\x03\x88\x01\x01\x12\x1e\n\x11mean_elapsed_time\x18\x05 \x01(\x02H\x04\x88\x01\x01\x12\x12\n\x05\x64\x65pth\x18\x06 \x01(\x05H\x05\x88\x01\x01\x12\x0f\n\x07proxies\x18\x07 \x03(\t\x12\x11\n\tnamespace\x18\x08 \x03(\t\x12\x0f\n\x07parents\x18\t \x03(\t\x12\x19\n\x0c\x66irst_parent\x18\n \x01(\tH\x06\x88\x01\x01\x12 \n\x07runtime\x18\x0b \x01(\x0b\x32\n.PbRuntimeH\x07\x88\x01\x01\x42\x08\n\x06_stampB\x05\n\x03_idB\x07\n\x05_nameB\x07\n\x05_metaB\x14\n\x12_mean_elapsed_timeB\x08\n\x06_depthB\x0f\n\r_first_parentB\n\n\x08_runtime\"\xd8\x01\n\nPbPollTask\x12\x18\n\x0blocal_proxy\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x15\n\x08workflow\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x19\n\x0cremote_proxy\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x16\n\treq_state\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x19\n\x0cgraph_string\x18\x05 \x01(\tH\x04\x88\x01\x01\x42\x0e\n\x0c_local_proxyB\x0b\n\t_workflowB\x0f\n\r_remote_proxyB\x0c\n\n_req_stateB\x0f\n\r_graph_string\"\xcb\x01\n\x0bPbCondition\x12\x17\n\ntask_proxy\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x17\n\nexpr_alias\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x16\n\treq_state\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x16\n\tsatisfied\x18\x04 \x01(\x08H\x03\x88\x01\x01\x12\x14\n\x07message\x18\x05 \x01(\tH\x04\x88\x01\x01\x42\r\n\x0b_task_proxyB\r\n\x0b_expr_aliasB\x0c\n\n_req_stateB\x0c\n\n_satisfiedB\n\n\x08_message\"\x96\x01\n\x0ePbPrerequisite\x12\x17\n\nexpression\x18\x01 \x01(\tH\x00\x88\x01\x01\x12 \n\nconditions\x18\x02 \x03(\x0b\x32\x0c.PbCondition\x12\x14\n\x0c\x63ycle_points\x18\x03 \x03(\t\x12\x16\n\tsatisfied\x18\x04 \x01(\x08H\x01\x88\x01\x01\x42\r\n\x0b_expressionB\x0c\n\n_satisfied\"\x8c\x01\n\x08PbOutput\x12\x12\n\x05label\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x14\n\x07message\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x16\n\tsatisfied\x18\x03 \x01(\x08H\x02\x88\x01\x01\x12\x11\n\x04time\x18\x04 \x01(\x01H\x03\x88\x01\x01\x42\x08\n\x06_labelB\n\n\x08_messageB\x0c\n\n_satisfiedB\x07\n\x05_time\"\xa5\x01\n\tPbTrigger\x12\x0f\n\x02id\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x12\n\x05label\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x14\n\x07message\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x16\n\tsatisfied\x18\x04 \x01(\x08H\x03\x88\x01\x01\x12\x11\n\x04time\x18\x05 \x01(\x01H\x04\x88\x01\x01\x42\x05\n\x03_idB\x08\n\x06_labelB\n\n\x08_messageB\x0c\n\n_satisfiedB\x07\n\x05_time\"\xe7\x07\n\x0bPbTaskProxy\x12\x12\n\x05stamp\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x02id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x11\n\x04task\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x12\n\x05state\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x18\n\x0b\x63ycle_point\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x12\n\x05\x64\x65pth\x18\x06 \x01(\x05H\x05\x88\x01\x01\x12\x18\n\x0bjob_submits\x18\x07 \x01(\x05H\x06\x88\x01\x01\x12*\n\x07outputs\x18\t \x03(\x0b\x32\x19.PbTaskProxy.OutputsEntry\x12\x11\n\tnamespace\x18\x0b \x03(\t\x12&\n\rprerequisites\x18\x0c \x03(\x0b\x32\x0f.PbPrerequisite\x12\x0c\n\x04jobs\x18\r \x03(\t\x12\x19\n\x0c\x66irst_parent\x18\x0f \x01(\tH\x07\x88\x01\x01\x12\x11\n\x04name\x18\x10 \x01(\tH\x08\x88\x01\x01\x12\x14\n\x07is_held\x18\x11 \x01(\x08H\t\x88\x01\x01\x12\r\n\x05\x65\x64ges\x18\x12 \x03(\t\x12\x11\n\tancestors\x18\x13 \x03(\t\x12\x16\n\tflow_nums\x18\x14 \x01(\tH\n\x88\x01\x01\x12=\n\x11\x65xternal_triggers\x18\x17 \x03(\x0b\x32\".PbTaskProxy.ExternalTriggersEntry\x12.\n\txtriggers\x18\x18 \x03(\x0b\x32\x1b.PbTaskProxy.XtriggersEntry\x12\x16\n\tis_queued\x18\x19 \x01(\x08H\x0b\x88\x01\x01\x12\x18\n\x0bis_runahead\x18\x1a \x01(\x08H\x0c\x88\x01\x01\x12\x16\n\tflow_wait\x18\x1b \x01(\x08H\r\x88\x01\x01\x12 \n\x07runtime\x18\x1c \x01(\x0b\x32\n.PbRuntimeH\x0e\x88\x01\x01\x1a\x39\n\x0cOutputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.PbOutput:\x02\x38\x01\x1a\x43\n\x15\x45xternalTriggersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x19\n\x05value\x18\x02 \x01(\x0b\x32\n.PbTrigger:\x02\x38\x01\x1a<\n\x0eXtriggersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x19\n\x05value\x18\x02 \x01(\x0b\x32\n.PbTrigger:\x02\x38\x01\x42\x08\n\x06_stampB\x05\n\x03_idB\x07\n\x05_taskB\x08\n\x06_stateB\x0e\n\x0c_cycle_pointB\x08\n\x06_depthB\x0e\n\x0c_job_submitsB\x0f\n\r_first_parentB\x07\n\x05_nameB\n\n\x08_is_heldB\x0c\n\n_flow_numsB\x0c\n\n_is_queuedB\x0e\n\x0c_is_runaheadB\x0c\n\n_flow_waitB\n\n\x08_runtime\"\xc8\x02\n\x08PbFamily\x12\x12\n\x05stamp\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x02id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x11\n\x04name\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x1a\n\x04meta\x18\x04 \x01(\x0b\x32\x07.PbMetaH\x03\x88\x01\x01\x12\x12\n\x05\x64\x65pth\x18\x05 \x01(\x05H\x04\x88\x01\x01\x12\x0f\n\x07proxies\x18\x06 \x03(\t\x12\x0f\n\x07parents\x18\x07 \x03(\t\x12\x13\n\x0b\x63hild_tasks\x18\x08 \x03(\t\x12\x16\n\x0e\x63hild_families\x18\t \x03(\t\x12\x19\n\x0c\x66irst_parent\x18\n \x01(\tH\x05\x88\x01\x01\x12 \n\x07runtime\x18\x0b \x01(\x0b\x32\n.PbRuntimeH\x06\x88\x01\x01\x42\x08\n\x06_stampB\x05\n\x03_idB\x07\n\x05_nameB\x07\n\x05_metaB\x08\n\x06_depthB\x0f\n\r_first_parentB\n\n\x08_runtime\"\x84\x06\n\rPbFamilyProxy\x12\x12\n\x05stamp\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x02id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x18\n\x0b\x63ycle_point\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x11\n\x04name\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x13\n\x06\x66\x61mily\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x12\n\x05state\x18\x06 \x01(\tH\x05\x88\x01\x01\x12\x12\n\x05\x64\x65pth\x18\x07 \x01(\x05H\x06\x88\x01\x01\x12\x19\n\x0c\x66irst_parent\x18\x08 \x01(\tH\x07\x88\x01\x01\x12\x13\n\x0b\x63hild_tasks\x18\n \x03(\t\x12\x16\n\x0e\x63hild_families\x18\x0b \x03(\t\x12\x14\n\x07is_held\x18\x0c \x01(\x08H\x08\x88\x01\x01\x12\x11\n\tancestors\x18\r \x03(\t\x12\x0e\n\x06states\x18\x0e \x03(\t\x12\x35\n\x0cstate_totals\x18\x0f \x03(\x0b\x32\x1f.PbFamilyProxy.StateTotalsEntry\x12\x1a\n\ris_held_total\x18\x10 \x01(\x05H\t\x88\x01\x01\x12\x16\n\tis_queued\x18\x11 \x01(\x08H\n\x88\x01\x01\x12\x1c\n\x0fis_queued_total\x18\x12 \x01(\x05H\x0b\x88\x01\x01\x12\x18\n\x0bis_runahead\x18\x13 \x01(\x08H\x0c\x88\x01\x01\x12\x1e\n\x11is_runahead_total\x18\x14 \x01(\x05H\r\x88\x01\x01\x12 \n\x07runtime\x18\x15 \x01(\x0b\x32\n.PbRuntimeH\x0e\x88\x01\x01\x1a\x32\n\x10StateTotalsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\x42\x08\n\x06_stampB\x05\n\x03_idB\x0e\n\x0c_cycle_pointB\x07\n\x05_nameB\t\n\x07_familyB\x08\n\x06_stateB\x08\n\x06_depthB\x0f\n\r_first_parentB\n\n\x08_is_heldB\x10\n\x0e_is_held_totalB\x0c\n\n_is_queuedB\x12\n\x10_is_queued_totalB\x0e\n\x0c_is_runaheadB\x14\n\x12_is_runahead_totalB\n\n\x08_runtime\"\xbc\x01\n\x06PbEdge\x12\x12\n\x05stamp\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x02id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x13\n\x06source\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x13\n\x06target\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x14\n\x07suicide\x18\x05 \x01(\x08H\x04\x88\x01\x01\x12\x11\n\x04\x63ond\x18\x06 \x01(\x08H\x05\x88\x01\x01\x42\x08\n\x06_stampB\x05\n\x03_idB\t\n\x07_sourceB\t\n\x07_targetB\n\n\x08_suicideB\x07\n\x05_cond\"{\n\x07PbEdges\x12\x0f\n\x02id\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\r\n\x05\x65\x64ges\x18\x02 \x03(\t\x12+\n\x16workflow_polling_tasks\x18\x03 \x03(\x0b\x32\x0b.PbPollTask\x12\x0e\n\x06leaves\x18\x04 \x03(\t\x12\x0c\n\x04\x66\x65\x65t\x18\x05 \x03(\tB\x05\n\x03_id\"\xf2\x01\n\x10PbEntireWorkflow\x12\"\n\x08workflow\x18\x01 \x01(\x0b\x32\x0b.PbWorkflowH\x00\x88\x01\x01\x12\x16\n\x05tasks\x18\x02 \x03(\x0b\x32\x07.PbTask\x12\"\n\x0ctask_proxies\x18\x03 \x03(\x0b\x32\x0c.PbTaskProxy\x12\x14\n\x04jobs\x18\x04 \x03(\x0b\x32\x06.PbJob\x12\x1b\n\x08\x66\x61milies\x18\x05 \x03(\x0b\x32\t.PbFamily\x12&\n\x0e\x66\x61mily_proxies\x18\x06 \x03(\x0b\x32\x0e.PbFamilyProxy\x12\x16\n\x05\x65\x64ges\x18\x07 \x03(\x0b\x32\x07.PbEdgeB\x0b\n\t_workflow\"\xaf\x01\n\x07\x45\x44\x65ltas\x12\x11\n\x04time\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x63hecksum\x18\x02 \x01(\x03H\x01\x88\x01\x01\x12\x16\n\x05\x61\x64\x64\x65\x64\x18\x03 \x03(\x0b\x32\x07.PbEdge\x12\x18\n\x07updated\x18\x04 \x03(\x0b\x32\x07.PbEdge\x12\x0e\n\x06pruned\x18\x05 \x03(\t\x12\x15\n\x08reloaded\x18\x06 \x01(\x08H\x02\x88\x01\x01\x42\x07\n\x05_timeB\x0b\n\t_checksumB\x0b\n\t_reloaded\"\xb3\x01\n\x07\x46\x44\x65ltas\x12\x11\n\x04time\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x63hecksum\x18\x02 \x01(\x03H\x01\x88\x01\x01\x12\x18\n\x05\x61\x64\x64\x65\x64\x18\x03 \x03(\x0b\x32\t.PbFamily\x12\x1a\n\x07updated\x18\x04 \x03(\x0b\x32\t.PbFamily\x12\x0e\n\x06pruned\x18\x05 \x03(\t\x12\x15\n\x08reloaded\x18\x06 \x01(\x08H\x02\x88\x01\x01\x42\x07\n\x05_timeB\x0b\n\t_checksumB\x0b\n\t_reloaded\"\xbe\x01\n\x08\x46PDeltas\x12\x11\n\x04time\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x63hecksum\x18\x02 \x01(\x03H\x01\x88\x01\x01\x12\x1d\n\x05\x61\x64\x64\x65\x64\x18\x03 \x03(\x0b\x32\x0e.PbFamilyProxy\x12\x1f\n\x07updated\x18\x04 \x03(\x0b\x32\x0e.PbFamilyProxy\x12\x0e\n\x06pruned\x18\x05 \x03(\t\x12\x15\n\x08reloaded\x18\x06 \x01(\x08H\x02\x88\x01\x01\x42\x07\n\x05_timeB\x0b\n\t_checksumB\x0b\n\t_reloaded\"\xad\x01\n\x07JDeltas\x12\x11\n\x04time\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x63hecksum\x18\x02 \x01(\x03H\x01\x88\x01\x01\x12\x15\n\x05\x61\x64\x64\x65\x64\x18\x03 \x03(\x0b\x32\x06.PbJob\x12\x17\n\x07updated\x18\x04 \x03(\x0b\x32\x06.PbJob\x12\x0e\n\x06pruned\x18\x05 \x03(\t\x12\x15\n\x08reloaded\x18\x06 \x01(\x08H\x02\x88\x01\x01\x42\x07\n\x05_timeB\x0b\n\t_checksumB\x0b\n\t_reloaded\"\xaf\x01\n\x07TDeltas\x12\x11\n\x04time\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x63hecksum\x18\x02 \x01(\x03H\x01\x88\x01\x01\x12\x16\n\x05\x61\x64\x64\x65\x64\x18\x03 \x03(\x0b\x32\x07.PbTask\x12\x18\n\x07updated\x18\x04 \x03(\x0b\x32\x07.PbTask\x12\x0e\n\x06pruned\x18\x05 \x03(\t\x12\x15\n\x08reloaded\x18\x06 \x01(\x08H\x02\x88\x01\x01\x42\x07\n\x05_timeB\x0b\n\t_checksumB\x0b\n\t_reloaded\"\xba\x01\n\x08TPDeltas\x12\x11\n\x04time\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x63hecksum\x18\x02 \x01(\x03H\x01\x88\x01\x01\x12\x1b\n\x05\x61\x64\x64\x65\x64\x18\x03 \x03(\x0b\x32\x0c.PbTaskProxy\x12\x1d\n\x07updated\x18\x04 \x03(\x0b\x32\x0c.PbTaskProxy\x12\x0e\n\x06pruned\x18\x05 \x03(\t\x12\x15\n\x08reloaded\x18\x06 \x01(\x08H\x02\x88\x01\x01\x42\x07\n\x05_timeB\x0b\n\t_checksumB\x0b\n\t_reloaded\"\xc3\x01\n\x07WDeltas\x12\x11\n\x04time\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x1f\n\x05\x61\x64\x64\x65\x64\x18\x02 \x01(\x0b\x32\x0b.PbWorkflowH\x01\x88\x01\x01\x12!\n\x07updated\x18\x03 \x01(\x0b\x32\x0b.PbWorkflowH\x02\x88\x01\x01\x12\x15\n\x08reloaded\x18\x04 \x01(\x08H\x03\x88\x01\x01\x12\x13\n\x06pruned\x18\x05 \x01(\tH\x04\x88\x01\x01\x42\x07\n\x05_timeB\x08\n\x06_addedB\n\n\x08_updatedB\x0b\n\t_reloadedB\t\n\x07_pruned\"\xd1\x01\n\tAllDeltas\x12\x1a\n\x08\x66\x61milies\x18\x01 \x01(\x0b\x32\x08.FDeltas\x12!\n\x0e\x66\x61mily_proxies\x18\x02 \x01(\x0b\x32\t.FPDeltas\x12\x16\n\x04jobs\x18\x03 \x01(\x0b\x32\x08.JDeltas\x12\x17\n\x05tasks\x18\x04 \x01(\x0b\x32\x08.TDeltas\x12\x1f\n\x0ctask_proxies\x18\x05 \x01(\x0b\x32\t.TPDeltas\x12\x17\n\x05\x65\x64ges\x18\x06 \x01(\x0b\x32\x08.EDeltas\x12\x1a\n\x08workflow\x18\x07 \x01(\x0b\x32\x08.WDeltasb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'data_messages_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'data_messages_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _PBWORKFLOW_STATETOTALSENTRY._options = None
   _PBWORKFLOW_STATETOTALSENTRY._serialized_options = b'8\001'
   _PBWORKFLOW_LATESTSTATETASKSENTRY._options = None
   _PBWORKFLOW_LATESTSTATETASKSENTRY._serialized_options = b'8\001'
@@ -29,74 +30,72 @@
   _PBTASKPROXY_OUTPUTSENTRY._serialized_options = b'8\001'
   _PBTASKPROXY_EXTERNALTRIGGERSENTRY._options = None
   _PBTASKPROXY_EXTERNALTRIGGERSENTRY._serialized_options = b'8\001'
   _PBTASKPROXY_XTRIGGERSENTRY._options = None
   _PBTASKPROXY_XTRIGGERSENTRY._serialized_options = b'8\001'
   _PBFAMILYPROXY_STATETOTALSENTRY._options = None
   _PBFAMILYPROXY_STATETOTALSENTRY._serialized_options = b'8\001'
-  _PBMETA._serialized_start=24
-  _PBMETA._serialized_end=174
-  _PBTIMEZONE._serialized_start=177
-  _PBTIMEZONE._serialized_end=347
-  _PBTASKPROXYREFS._serialized_start=349
-  _PBTASKPROXYREFS._serialized_end=388
-  _PBWORKFLOW._serialized_start=391
-  _PBWORKFLOW._serialized_end=1913
-  _PBWORKFLOW_STATETOTALSENTRY._serialized_start=1382
-  _PBWORKFLOW_STATETOTALSENTRY._serialized_end=1432
-  _PBWORKFLOW_LATESTSTATETASKSENTRY._serialized_start=1434
-  _PBWORKFLOW_LATESTSTATETASKSENTRY._serialized_end=1507
-  _PBRUNTIME._serialized_start=1916
-  _PBRUNTIME._serialized_end=2741
-  _PBJOB._serialized_start=2744
-  _PBJOB._serialized_end=3427
-  _PBTASK._serialized_start=3430
-  _PBTASK._serialized_end=3784
-  _PBPOLLTASK._serialized_start=3787
-  _PBPOLLTASK._serialized_end=4003
-  _PBCONDITION._serialized_start=4006
-  _PBCONDITION._serialized_end=4209
-  _PBPREREQUISITE._serialized_start=4212
-  _PBPREREQUISITE._serialized_end=4362
-  _PBOUTPUT._serialized_start=4365
-  _PBOUTPUT._serialized_end=4505
-  _PBCLOCKTRIGGER._serialized_start=4507
-  _PBCLOCKTRIGGER._serialized_end=4631
-  _PBTRIGGER._serialized_start=4634
-  _PBTRIGGER._serialized_end=4799
-  _PBTASKPROXY._serialized_start=4802
-  _PBTASKPROXY._serialized_end=5864
-  _PBTASKPROXY_OUTPUTSENTRY._serialized_start=5472
-  _PBTASKPROXY_OUTPUTSENTRY._serialized_end=5529
-  _PBTASKPROXY_EXTERNALTRIGGERSENTRY._serialized_start=5531
-  _PBTASKPROXY_EXTERNALTRIGGERSENTRY._serialized_end=5598
-  _PBTASKPROXY_XTRIGGERSENTRY._serialized_start=5600
-  _PBTASKPROXY_XTRIGGERSENTRY._serialized_end=5660
-  _PBFAMILY._serialized_start=5867
-  _PBFAMILY._serialized_end=6195
-  _PBFAMILYPROXY._serialized_start=6198
-  _PBFAMILYPROXY._serialized_end=6970
-  _PBFAMILYPROXY_STATETOTALSENTRY._serialized_start=1382
-  _PBFAMILYPROXY_STATETOTALSENTRY._serialized_end=1432
-  _PBEDGE._serialized_start=6973
-  _PBEDGE._serialized_end=7161
-  _PBEDGES._serialized_start=7163
-  _PBEDGES._serialized_end=7286
-  _PBENTIREWORKFLOW._serialized_start=7289
-  _PBENTIREWORKFLOW._serialized_end=7531
-  _EDELTAS._serialized_start=7534
-  _EDELTAS._serialized_end=7709
-  _FDELTAS._serialized_start=7712
-  _FDELTAS._serialized_end=7891
-  _FPDELTAS._serialized_start=7894
-  _FPDELTAS._serialized_end=8084
-  _JDELTAS._serialized_start=8087
-  _JDELTAS._serialized_end=8260
-  _TDELTAS._serialized_start=8263
-  _TDELTAS._serialized_end=8438
-  _TPDELTAS._serialized_start=8441
-  _TPDELTAS._serialized_end=8627
-  _WDELTAS._serialized_start=8630
-  _WDELTAS._serialized_end=8825
-  _ALLDELTAS._serialized_start=8828
-  _ALLDELTAS._serialized_end=9037
+  _globals['_PBMETA']._serialized_start=24
+  _globals['_PBMETA']._serialized_end=174
+  _globals['_PBTIMEZONE']._serialized_start=177
+  _globals['_PBTIMEZONE']._serialized_end=347
+  _globals['_PBTASKPROXYREFS']._serialized_start=349
+  _globals['_PBTASKPROXYREFS']._serialized_end=388
+  _globals['_PBWORKFLOW']._serialized_start=391
+  _globals['_PBWORKFLOW']._serialized_end=1961
+  _globals['_PBWORKFLOW_STATETOTALSENTRY']._serialized_start=1411
+  _globals['_PBWORKFLOW_STATETOTALSENTRY']._serialized_end=1461
+  _globals['_PBWORKFLOW_LATESTSTATETASKSENTRY']._serialized_start=1463
+  _globals['_PBWORKFLOW_LATESTSTATETASKSENTRY']._serialized_end=1536
+  _globals['_PBRUNTIME']._serialized_start=1964
+  _globals['_PBRUNTIME']._serialized_end=2789
+  _globals['_PBJOB']._serialized_start=2792
+  _globals['_PBJOB']._serialized_end=3475
+  _globals['_PBTASK']._serialized_start=3478
+  _globals['_PBTASK']._serialized_end=3832
+  _globals['_PBPOLLTASK']._serialized_start=3835
+  _globals['_PBPOLLTASK']._serialized_end=4051
+  _globals['_PBCONDITION']._serialized_start=4054
+  _globals['_PBCONDITION']._serialized_end=4257
+  _globals['_PBPREREQUISITE']._serialized_start=4260
+  _globals['_PBPREREQUISITE']._serialized_end=4410
+  _globals['_PBOUTPUT']._serialized_start=4413
+  _globals['_PBOUTPUT']._serialized_end=4553
+  _globals['_PBTRIGGER']._serialized_start=4556
+  _globals['_PBTRIGGER']._serialized_end=4721
+  _globals['_PBTASKPROXY']._serialized_start=4724
+  _globals['_PBTASKPROXY']._serialized_end=5723
+  _globals['_PBTASKPROXY_OUTPUTSENTRY']._serialized_start=5349
+  _globals['_PBTASKPROXY_OUTPUTSENTRY']._serialized_end=5406
+  _globals['_PBTASKPROXY_EXTERNALTRIGGERSENTRY']._serialized_start=5408
+  _globals['_PBTASKPROXY_EXTERNALTRIGGERSENTRY']._serialized_end=5475
+  _globals['_PBTASKPROXY_XTRIGGERSENTRY']._serialized_start=5477
+  _globals['_PBTASKPROXY_XTRIGGERSENTRY']._serialized_end=5537
+  _globals['_PBFAMILY']._serialized_start=5726
+  _globals['_PBFAMILY']._serialized_end=6054
+  _globals['_PBFAMILYPROXY']._serialized_start=6057
+  _globals['_PBFAMILYPROXY']._serialized_end=6829
+  _globals['_PBFAMILYPROXY_STATETOTALSENTRY']._serialized_start=1411
+  _globals['_PBFAMILYPROXY_STATETOTALSENTRY']._serialized_end=1461
+  _globals['_PBEDGE']._serialized_start=6832
+  _globals['_PBEDGE']._serialized_end=7020
+  _globals['_PBEDGES']._serialized_start=7022
+  _globals['_PBEDGES']._serialized_end=7145
+  _globals['_PBENTIREWORKFLOW']._serialized_start=7148
+  _globals['_PBENTIREWORKFLOW']._serialized_end=7390
+  _globals['_EDELTAS']._serialized_start=7393
+  _globals['_EDELTAS']._serialized_end=7568
+  _globals['_FDELTAS']._serialized_start=7571
+  _globals['_FDELTAS']._serialized_end=7750
+  _globals['_FPDELTAS']._serialized_start=7753
+  _globals['_FPDELTAS']._serialized_end=7943
+  _globals['_JDELTAS']._serialized_start=7946
+  _globals['_JDELTAS']._serialized_end=8119
+  _globals['_TDELTAS']._serialized_start=8122
+  _globals['_TDELTAS']._serialized_end=8297
+  _globals['_TPDELTAS']._serialized_start=8300
+  _globals['_TPDELTAS']._serialized_end=8486
+  _globals['_WDELTAS']._serialized_start=8489
+  _globals['_WDELTAS']._serialized_end=8684
+  _globals['_ALLDELTAS']._serialized_start=8687
+  _globals['_ALLDELTAS']._serialized_end=8896
 # @@protoc_insertion_point(module_scope)
```

### Comparing `cylc-flow-8.1.4/cylc/flow/data_store_mgr.py` & `cylc-flow-8.2.0/cylc/flow/data_store_mgr.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,21 @@
 """
 
 from contextlib import suppress
 from collections import Counter, deque
 from copy import deepcopy
 import json
 from time import time
-from typing import Union, Tuple, TYPE_CHECKING
+from typing import (
+    Any,
+    Optional,
+    TYPE_CHECKING,
+    Tuple,
+    Union,
+)
 import zlib
 
 from cylc.flow import __version__ as CYLC_VERSION, LOG
 from cylc.flow.data_messages_pb2 import (  # type: ignore
     PbEdge, PbEntireWorkflow, PbFamily, PbFamilyProxy, PbJob, PbTask,
     PbTaskProxy, PbWorkflow, PbRuntime, AllDeltas, EDeltas, FDeltas,
     FPDeltas, JDeltas, TDeltas, TPDeltas, WDeltas)
@@ -95,16 +101,15 @@
 from cylc.flow.util import (
     serialise,
     deserialise
 )
 from cylc.flow.wallclock import (
     TIME_ZONE_LOCAL_INFO,
     TIME_ZONE_UTC_INFO,
-    get_utc_mode,
-    get_time_string_from_unix_time as time2str
+    get_utc_mode
 )
 
 if TYPE_CHECKING:
     from cylc.flow.cycling import PointBase
 
 
 EDGES = 'edges'
@@ -291,15 +296,15 @@
             data[key].CopyFrom(delta.added)
     # Merge in updated fields
     if getattr(delta, 'updated', False):
         if key == WORKFLOW:
             # Clear fields that require overwrite with delta
             field_set = {f.name for f, _ in delta.updated.ListFields()}
             for field in CLEAR_FIELD_MAP[key]:
-                if field in field_set:
+                if field in field_set or delta.updated.states_updated:
                     data[key].ClearField(field)
             data[key].MergeFrom(delta.updated)
         else:
             for element in delta.updated:
                 try:
                     data_element = data[key][element.id]
                     # Clear fields that require overwrite with delta
@@ -494,14 +499,15 @@
         self.n_window_nodes = {}
         self.n_window_edges = {}
         self.n_window_boundary_nodes = {}
         self.db_load_task_proxies = {}
         self.family_pruned_ids = set()
         self.prune_trigger_nodes = {}
         self.prune_flagged_nodes = set()
+        self.pruned_task_proxies = set()
         self.updates_pending = False
         self.publish_pending = False
 
     def initiate_data_model(self, reloaded=False):
         """Initiate or Update data model on start/restart/reload.
 
         Args:
@@ -682,25 +688,25 @@
         workflow.families.extend(list(families))
 
         self.ancestors = ancestors
         self.descendants = descendants
         self.parents = parents
 
     def increment_graph_window(
-            self,
-            source_tokens,
-            point,
-            flow_nums,
-            edge_distance=0,
-            active_id=None,
-            descendant=False,
-            is_parent=False,
-            is_manual_submit=False,
-            itask=None
-    ):
+        self,
+        source_tokens: Tokens,
+        point,
+        flow_nums,
+        edge_distance=0,
+        active_id: Optional[str] = None,
+        descendant=False,
+        is_parent=False,
+        is_manual_submit=False,
+        itask=None
+    ) -> None:
         """Generate graph window about active task proxy to n-edge-distance.
 
         A recursive function, that creates a node then moves to children and
         parents repeating this process out to one edge beyond the max window
         size (in edges). Going out one edge further, we can trigger
         pruning as new active tasks appear beyond this boundary.
 
@@ -717,15 +723,14 @@
                 Is the current node a direct descendent of the active/origin.
             is_parent (bool)
             is_manual_submit (bool)
             itask (cylc.flow.task_proxy.TaskProxy):
                 Active/Other task proxy, passed in with pool invocation.
 
         Returns:
-
             None
 
         """
         is_active = not (descendant or is_parent)
         # ID passed through recursion as reference to original/active node.
         if active_id is None:
             source_tokens = self.id_.duplicate(source_tokens)
@@ -767,14 +772,16 @@
         )
 
         self.n_window_nodes[active_id].add(source_tokens.id)
 
         edge_distance += 1
 
         # Don't expand window about orphan task.
+        child_tokens: Tokens
+        parent_tokens: Tokens
         if not is_orphan:
             tdef = self.schd.config.taskdefs[source_tokens['task']]
             # TODO: xtrigger is workflow_state edges too
             # Reference set for workflow relations
             final_point = self.schd.config.final_point
             if descendant or is_active:
                 if graph_children is None:
@@ -860,15 +867,20 @@
                 self.prune_trigger_nodes.setdefault(
                     tp_id, set()).add(active_id)
             del self.n_window_boundary_nodes[active_id]
             if self.n_window_edges[active_id]:
                 getattr(self.updated[WORKFLOW], EDGES).edges.extend(
                     self.n_window_edges[active_id])
 
-    def generate_edge(self, parent_tokens, child_tokens, active_id):
+    def generate_edge(
+        self,
+        parent_tokens: Tokens,
+        child_tokens: Tokens,
+        active_id: str,
+    ) -> None:
         """Construct edge of child and parent task proxy node."""
         # Initiate edge element.
         e_id = self.edge_id(parent_tokens, child_tokens)
         if e_id in self.n_window_edges[active_id]:
             return
         if (
             e_id not in self.data[self.workflow_id][EDGES]
@@ -918,34 +930,33 @@
             cycle=str(point),
             task=name,
         ).id
         self.all_task_pool.add(tp_id)
 
     def generate_ghost_task(
         self,
-        tokens,
+        tokens: Tokens,
         point,
         flow_nums,
         is_parent=False,
         itask=None
-    ):
+    ) -> Tuple[bool, Optional[dict]]:
         """Create task-point element populated with static data.
 
         Args:
             source_tokens (cylc.flow.id.Tokens)
             point (PointBase)
             flow_nums (set)
             is_parent (bool):
                 Used to determine whether to load DB state.
             itask (cylc.flow.task_proxy.TaskProxy):
                 Update task-node from corresponding task proxy object.
 
         Returns:
-
-            (True/False, Dict/None)
+            (is_orphan, graph_children)
 
         Orphan tasks with no children return (True, None) respectively.
 
         """
         name = tokens['task']
         point_string = tokens['cycle']
         t_id = self.definition_id(name)
@@ -961,14 +972,15 @@
         if tp_id in task_proxies or tp_id in self.added[TASK_PROXIES]:
             if itask is None:
                 return is_orphan, None
             return is_orphan, itask.graph_children
 
         if itask is None:
             itask = TaskProxy(
+                self.id_,
                 self.schd.config.get_taskdef(name),
                 point,
                 flow_nums,
                 submit_num=0,
                 data_mode=True
             )
 
@@ -1140,15 +1152,15 @@
             ]
             if fp_delta.ancestors:
                 fp_delta.first_parent = fp_delta.ancestors[0]
 
             fp_delta.runtime.CopyFrom(
                 runtime_from_config(
                     self._apply_broadcasts_to_runtime(
-                        tokens.relative_id,
+                        tokens,
                         self.schd.config.cfg['runtime'][fam.name]
                     )
                 )
             )
 
             self.added[FAMILY_PROXIES][fp_id] = fp_delta
             fp_parent = fp_delta
@@ -1182,15 +1194,16 @@
         for (
                 cycle, name, flow_nums_str, status, submit_num, outputs_str
         ) in flow_db.select_tasks_for_datastore(task_ids):
             tokens = self.id_.duplicate(
                 cycle=cycle,
                 task=name,
             )
-            itask, is_parent = self.db_load_task_proxies[tokens.relative_id]
+            relative_id = tokens.relative_id
+            itask, is_parent = self.db_load_task_proxies[relative_id]
             itask.submit_num = submit_num
             flow_nums = deserialise(flow_nums_str)
             # Do not set states and outputs for future tasks in flow.
             if (
                     itask.flow_nums and
                     flow_nums != itask.flow_nums and
                     not is_parent
@@ -1207,15 +1220,15 @@
                         TASK_STATUS_FAILED,
                         TASK_STATUS_SUCCEEDED
                     )
             ):
                 for message in json.loads(outputs_str):
                     itask.state.outputs.set_completion(message, True)
             # Gather tasks with flow id.
-            prereq_ids.add(f'{tokens.relative_id}/{flow_nums_str}')
+            prereq_ids.add(f'{relative_id}/{flow_nums_str}')
 
         # Batch load prerequisites of tasks according to flow.
         prereqs_map = {}
         for (
                 cycle, name, prereq_name,
                 prereq_cycle, prereq_output, satisfied
         ) in flow_db.select_prereqs_for_datastore(prereq_ids):
@@ -1274,20 +1287,14 @@
         for label, message, satisfied in itask.state.outputs.get_all():
             output = tproxy.outputs[label]
             output.label = label
             output.message = message
             output.satisfied = satisfied
             output.time = update_time
 
-        if itask.tdef.clocktrigger_offset is not None:
-            tproxy.clock_trigger.satisfied = itask.is_waiting_clock_done()
-            tproxy.clock_trigger.time = itask.clock_trigger_time
-            tproxy.clock_trigger.time_string = time2str(
-                itask.clock_trigger_time)
-
         for trig, satisfied in itask.state.external_triggers.items():
             ext_trig = tproxy.external_triggers[trig]
             ext_trig.id = trig
             ext_trig.satisfied = satisfied
 
         for label, satisfied in itask.state.xtriggers.items():
             sig = self.schd.xtrigger_mgr.get_xtrig_ctx(
@@ -1295,65 +1302,64 @@
             xtrig = tproxy.xtriggers[sig]
             xtrig.id = sig
             xtrig.label = label
             xtrig.satisfied = satisfied
             self.xtrigger_tasks.setdefault(sig, set()).add(tproxy.id)
 
         if tproxy.state in self.latest_state_tasks:
-            tp_ref = Tokens(tproxy.id).relative_id
+            tp_ref = itask.identity
             tp_queue = self.latest_state_tasks[tproxy.state]
             if tp_ref in tp_queue:
                 tp_queue.remove(tp_ref)
             self.latest_state_tasks[tproxy.state].appendleft(tp_ref)
 
         tproxy.runtime.CopyFrom(
             runtime_from_config(
                 self._apply_broadcasts_to_runtime(
-                    itask.identity,
+                    itask.tokens,
                     itask.tdef.rtconfig
                 )
             )
         )
 
-    def _apply_broadcasts_to_runtime(self, relative_id, rtconfig):
+    def _apply_broadcasts_to_runtime(self, tokens, rtconfig):
         # Handle broadcasts
-        overrides = self.schd.broadcast_mgr.get_broadcast(relative_id)
+        overrides = self.schd.broadcast_mgr.get_broadcast(tokens)
         if overrides:
             rtconfig = pdeepcopy(rtconfig)
             poverride(rtconfig, overrides, prepend=True)
         return rtconfig
 
-    def insert_job(self, name, point_string, status, job_conf):
+    def insert_job(self, name, cycle_point, status, job_conf):
         """Insert job into data-store.
 
         Args:
             name (str): Corresponding task name.
-            point_string (str): Cycle point string
+            cycle_point (str|PointBase): Cycle point string
             job_conf (dic):
                 Dictionary of job configuration used to generate
                 the job script.
                 (see TaskJobManager._prep_submit_task_job_impl)
 
         Returns:
 
             None
 
         """
         sub_num = job_conf['submit_num']
-        tp_id, tproxy = self.store_node_fetcher(name, point_string)
+        tp_tokens = self.id_.duplicate(
+            cycle=str(cycle_point),
+            task=name,
+        )
+        tp_id, tproxy = self.store_node_fetcher(tp_tokens)
         if not tproxy:
             return
         update_time = time()
-        tp_tokens = Tokens(tp_id)
         j_tokens = tp_tokens.duplicate(job=str(sub_num))
-        j_id, job = self.store_node_fetcher(
-            j_tokens['task'],
-            j_tokens['cycle'],
-            j_tokens['job'],
-        )
+        j_id, job = self.store_node_fetcher(j_tokens)
         if job:
             # Job already exists (i.e. post-submission submit failure)
             return
 
         if status not in JOB_STATUS_SET:
             return
 
@@ -1368,15 +1374,15 @@
             execution_time_limit=job_conf.get('execution_time_limit'),
             platform=job_conf.get('platform')['name'],
             job_runner_name=job_conf.get('job_runner_name'),
         )
         # Not all fields are populated with some submit-failures,
         # so use task cfg as base.
         j_cfg = pdeepcopy(self._apply_broadcasts_to_runtime(
-            tp_tokens.relative_id,
+            tp_tokens,
             self.schd.config.cfg['runtime'][tproxy.name]
         ))
         for key, val in job_conf.items():
             j_cfg[key] = val
         j_buf.runtime.CopyFrom(runtime_from_config(j_cfg))
 
         # Add in log files.
@@ -1410,19 +1416,21 @@
             time_run,
             time_run_exit,
             run_status,
             job_runner_name,
             job_id,
             platform_name
         ) = row
-
-        tp_id, tproxy = self.store_node_fetcher(name, point_string)
+        tp_tokens = self.id_.duplicate(
+            cycle=point_string,
+            task=name,
+        )
+        tp_id, tproxy = self.store_node_fetcher(tp_tokens)
         if not tproxy:
             return
-        tp_tokens = Tokens(tp_id)
         j_tokens = tp_tokens.duplicate(job=str(submit_num))
         j_id = j_tokens.id
 
         if run_status is not None:
             if run_status == 0:
                 status = TASK_STATUS_SUCCEEDED
             else:
@@ -1489,32 +1497,38 @@
             self.n_edge_distance = self.next_n_edge_distance
             self.next_n_edge_distance = None
 
         self.prune_data_store()
         if self.state_update_families:
             self.update_family_proxies()
 
+        next_update_pending = False
         if self.updates_pending:
             # Update workflow statuses and totals if needed
             self.update_workflow()
 
+            # Don't process updated deltas of pruned nodes
+            if self.pruned_task_proxies:
+                next_update_pending = True
+            self.prune_pruned_updated_nodes()
+
             # Apply current deltas
             self.batch_deltas()
             self.apply_delta_batch()
 
         if reloaded:
             self.clear_delta_batch()
             self.batch_deltas(reloaded=True)
 
         if self.updates_pending or reloaded:
             self.apply_delta_checksum()
             # Gather this batch of deltas for publish
             self.publish_deltas = self.get_publish_deltas()
 
-        self.updates_pending = False
+        self.updates_pending = next_update_pending
 
         # Clear deltas
         self.clear_delta_batch()
         self.clear_delta_store()
 
     def prune_data_store(self):
         """Remove flagged nodes and edges not in the set of active paths."""
@@ -1542,16 +1556,14 @@
         node_ids = out_paths_nodes.difference(in_paths_nodes)
         # Absolute triggers may be present in task pool, so recheck.
         # Clear the rest.
         self.prune_flagged_nodes.intersection_update(self.all_task_pool)
 
         tp_data = self.data[self.workflow_id][TASK_PROXIES]
         tp_added = self.added[TASK_PROXIES]
-        tp_updated = self.updated[TASK_PROXIES]
-        j_updated = self.updated[JOBS]
         parent_ids = set()
         for tp_id in list(node_ids):
             if tp_id in self.n_window_nodes:
                 del self.n_window_nodes[tp_id]
             if tp_id in self.n_window_edges:
                 del self.n_window_edges[tp_id]
             if tp_id in tp_data:
@@ -1562,34 +1574,28 @@
                 node_ids.remove(tp_id)
                 continue
             for sig in node.xtriggers:
                 self.xtrigger_tasks[sig].remove(tp_id)
                 if not self.xtrigger_tasks[sig]:
                     del self.xtrigger_tasks[sig]
 
-            # Don't process updated deltas of pruned node
-            if tp_id in tp_updated:
-                for j_id in list(node.jobs) + list(tp_updated[tp_id].jobs):
-                    if j_id in j_updated:
-                        del j_updated[j_id]
-                del tp_updated[tp_id]
-
             self.deltas[TASK_PROXIES].pruned.append(tp_id)
             self.deltas[JOBS].pruned.extend(node.jobs)
             self.deltas[EDGES].pruned.extend(node.edges)
             parent_ids.add(node.first_parent)
 
         checked_ids = set()
         while parent_ids:
             self._family_ascent_point_prune(
                 next(iter(parent_ids)),
                 node_ids, parent_ids, checked_ids, self.family_pruned_ids)
         if self.family_pruned_ids:
             self.deltas[FAMILY_PROXIES].pruned.extend(self.family_pruned_ids)
         if node_ids:
+            self.pruned_task_proxies.update(node_ids)
             self.updates_pending = True
 
     def _family_ascent_point_prune(
             self, fp_id, node_ids, parent_ids, checked_ids, prune_ids):
         """Find and prune family recursively checking child families.
 
         Recursively map out child families to the bottom from the origin
@@ -1631,14 +1637,40 @@
                 if fp_id in fp_updated:
                     del fp_updated[fp_id]
                 prune_ids.add(fp_id)
         checked_ids.add(fp_id)
         if fp_id in parent_ids:
             parent_ids.remove(fp_id)
 
+    def prune_pruned_updated_nodes(self):
+        """Remove updated nodes that will also be pruned this batch.
+
+        This will avoid processing and sending deltas that will immediately
+        be pruned. Kept separate from other pruning to allow for update
+        information to be included in summaries.
+
+        """
+        tp_data = self.data[self.workflow_id][TASK_PROXIES]
+        tp_added = self.added[TASK_PROXIES]
+        tp_updated = self.updated[TASK_PROXIES]
+        j_updated = self.updated[JOBS]
+        for tp_id in self.pruned_task_proxies:
+            if tp_id in tp_updated:
+                if tp_id in tp_data:
+                    node = tp_data[tp_id]
+                elif tp_id in tp_added:
+                    node = tp_added[tp_id]
+                else:
+                    continue
+                for j_id in list(node.jobs) + list(tp_updated[tp_id].jobs):
+                    if j_id in j_updated:
+                        del j_updated[j_id]
+                del tp_updated[tp_id]
+        self.pruned_task_proxies.clear()
+
     def update_family_proxies(self):
         """Update state & summary of flagged families and ancestors.
 
         Tasks whose state are updated flag their first parent, as a family
         to be updated, by adding their ID to a set.
         This set is iterated over here until empty, with each members child
         families checked/updated and first parent added to the set (flagged).
@@ -1802,14 +1834,15 @@
                     is_queued_total += root_node.is_queued_total
                     is_runahead_total += root_node.is_runahead_total
                     state_counter += Counter(dict(root_node.state_totals))
             w_delta.states[:] = state_counter.keys()
             for state, state_cnt in state_counter.items():
                 w_delta.state_totals[state] = state_cnt
 
+            w_delta.states_updated = True
             w_delta.is_held_total = is_held_total
             w_delta.is_queued_total = is_queued_total
             w_delta.is_runahead_total = is_runahead_total
             delta_set = True
 
             for state, tp_queue in self.latest_state_tasks.items():
                 w_delta.latest_state_tasks[state].task_proxies[:] = tp_queue
@@ -1878,15 +1911,15 @@
 
     def _generate_broadcast_node_deltas(self, node_data, node_type):
         cfg = self.schd.config.cfg
         for node_id, node in node_data.items():
             tokens = Tokens(node_id)
             new_runtime = runtime_from_config(
                 self._apply_broadcasts_to_runtime(
-                    tokens.relative_id,
+                    tokens,
                     cfg['runtime'][node.name]
                 )
             )
             new_sruntime = new_runtime.SerializeToString(
                 deterministic=True
             )
             old_sruntime = node.runtime.SerializeToString(
@@ -1905,27 +1938,27 @@
 
         Args:
             itask (cylc.flow.task_proxy.TaskProxy):
                 Update task-node from corresponding task proxy
                 objects from the workflow task pool.
 
         """
-        tp_id, tproxy = self.store_node_fetcher(itask.tdef.name, itask.point)
+        tp_id, tproxy = self.store_node_fetcher(itask.tokens)
         if not tproxy:
             return
         update_time = time()
 
         # update task instance
         tp_delta = self.updated[TASK_PROXIES].setdefault(
             tp_id, PbTaskProxy(id=tp_id))
         tp_delta.stamp = f'{tp_id}@{update_time}'
         tp_delta.state = itask.state.status
         self.state_update_families.add(tproxy.first_parent)
         if tp_delta.state in self.latest_state_tasks:
-            tp_ref = Tokens(tproxy.id).relative_id
+            tp_ref = itask.identity
             tp_queue = self.latest_state_tasks[tp_delta.state]
             if tp_ref in tp_queue:
                 tp_queue.remove(tp_ref)
             self.latest_state_tasks[tp_delta.state].appendleft(tp_ref)
         # if state is final work out new task mean.
         if tp_delta.state in TASK_STATUSES_FINAL:
             elapsed_time = task_mean_elapsed_time(itask.tdef)
@@ -1939,88 +1972,95 @@
                     t_id,
                     PbTask(id=t_id)).MergeFrom(t_delta)
         self.updates_pending = True
 
     def delta_task_held(
         self,
         itask: Union[TaskProxy, Tuple[str, 'PointBase', bool]]
-    ):
+    ) -> None:
         """Create delta for change in task proxy held state.
 
         Args:
             itask:
                 The TaskProxy to hold/release OR a tuple of the form
                 (name, cycle, is_held).
 
         """
         if isinstance(itask, TaskProxy):
-            name = itask.tdef.name
-            cycle = itask.point
+            tokens = itask.tokens
             is_held = itask.state.is_held
         else:
             name, cycle, is_held = itask
+            tokens = self.id_.duplicate(
+                task=name,
+                cycle=str(cycle),
+            )
 
-        tp_id, tproxy = self.store_node_fetcher(name, cycle)
+        tp_id, tproxy = self.store_node_fetcher(tokens)
         if not tproxy:
             return
         tp_delta = self.updated[TASK_PROXIES].setdefault(
             tp_id, PbTaskProxy(id=tp_id))
         tp_delta.stamp = f'{tp_id}@{time()}'
         tp_delta.is_held = is_held
         self.state_update_families.add(tproxy.first_parent)
         self.updates_pending = True
 
-    def delta_task_queued(self, itask):
+    def delta_task_queued(self, itask: TaskProxy) -> None:
         """Create delta for change in task proxy queued state.
 
         Args:
             itask (cylc.flow.task_proxy.TaskProxy):
                 Update task-node from corresponding task proxy
                 objects from the workflow task pool.
 
         """
-        tp_id, tproxy = self.store_node_fetcher(itask.tdef.name, itask.point)
+        tp_id, tproxy = self.store_node_fetcher(itask.tokens)
         if not tproxy:
             return
         tp_delta = self.updated[TASK_PROXIES].setdefault(
             tp_id, PbTaskProxy(id=tp_id))
         tp_delta.stamp = f'{tp_id}@{time()}'
         tp_delta.is_queued = itask.state.is_queued
         self.state_update_families.add(tproxy.first_parent)
         self.updates_pending = True
 
-    def delta_task_runahead(self, itask):
+    def delta_task_runahead(self, itask: TaskProxy) -> None:
         """Create delta for change in task proxy runahead state.
 
         Args:
             itask (cylc.flow.task_proxy.TaskProxy):
                 Update task-node from corresponding task proxy
                 objects from the workflow task pool.
 
         """
-        tp_id, tproxy = self.store_node_fetcher(itask.tdef.name, itask.point)
+        tp_id, tproxy = self.store_node_fetcher(itask.tokens)
         if not tproxy:
             return
         tp_delta = self.updated[TASK_PROXIES].setdefault(
             tp_id, PbTaskProxy(id=tp_id))
         tp_delta.stamp = f'{tp_id}@{time()}'
         tp_delta.is_runahead = itask.state.is_runahead
         self.state_update_families.add(tproxy.first_parent)
         self.updates_pending = True
 
-    def delta_task_output(self, itask, message):
+    def delta_task_output(
+        self,
+        itask: TaskProxy,
+        message: str,
+    ) -> None:
         """Create delta for change in task proxy output.
 
         Args:
             itask (cylc.flow.task_proxy.TaskProxy):
                 Update task-node from corresponding task proxy
                 objects from the workflow task pool.
 
         """
-        tp_id, tproxy = self.store_node_fetcher(itask.tdef.name, itask.point)
+        tp_id, tproxy = self.store_node_fetcher(itask.tokens)
         if not tproxy:
             return
         item = itask.state.outputs.get_item(message)
         if item is None:
             return
         label, _, satisfied = item
         # update task instance
@@ -2031,48 +2071,48 @@
         output = tp_delta.outputs[label]
         output.label = label
         output.message = message
         output.satisfied = satisfied
         output.time = update_time
         self.updates_pending = True
 
-    def delta_task_outputs(self, itask):
+    def delta_task_outputs(self, itask: TaskProxy) -> None:
         """Create delta for change in all task proxy outputs.
 
         Args:
             itask (cylc.flow.task_proxy.TaskProxy):
                 Update task-node from corresponding task proxy
                 objects from the workflow task pool.
 
         """
-        tp_id, tproxy = self.store_node_fetcher(itask.tdef.name, itask.point)
+        tp_id, tproxy = self.store_node_fetcher(itask.tokens)
         if not tproxy:
             return
         update_time = time()
         tp_delta = self.updated[TASK_PROXIES].setdefault(
             tp_id, PbTaskProxy(id=tp_id))
         tp_delta.stamp = f'{tp_id}@{update_time}'
         for label, _, satisfied in itask.state.outputs.get_all():
             output = tp_delta.outputs[label]
             output.label = label
             output.satisfied = satisfied
             output.time = update_time
 
         self.updates_pending = True
 
-    def delta_task_prerequisite(self, itask):
+    def delta_task_prerequisite(self, itask: TaskProxy) -> None:
         """Create delta for change in task proxy prerequisite.
 
         Args:
             itask (cylc.flow.task_proxy.TaskProxy):
                 Update task-node from corresponding task proxy
                 objects from the workflow task pool.
 
         """
-        tp_id, tproxy = self.store_node_fetcher(itask.tdef.name, itask.point)
+        tp_id, tproxy = self.store_node_fetcher(itask.tokens)
         if not tproxy:
             return
         update_time = time()
 
         tp_delta = self.updated[TASK_PROXIES].setdefault(
             tp_id, PbTaskProxy(id=tp_id))
         tp_delta.stamp = f'{tp_id}@{update_time}'
@@ -2082,56 +2122,32 @@
             prereq_obj = prereq.api_dump()
             if prereq_obj:
                 prereq_list.append(prereq_obj)
         del tp_delta.prerequisites[:]
         tp_delta.prerequisites.extend(prereq_list)
         self.updates_pending = True
 
-    def delta_task_clock_trigger(self, itask, check_items):
-        """Create delta for change in task proxy prereqs.
-
-        Args:
-            itask (cylc.flow.task_proxy.TaskProxy):
-                Update task-node from corresponding task proxy
-                objects from the workflow task pool.
-            check_items (tuple):
-                Collection of prerequisites checked to determine if
-                task is ready to run.
-
-        """
-        tp_id, tproxy = self.store_node_fetcher(itask.tdef.name, itask.point)
-        if not tproxy:
-            return
-        if len(check_items) == 1:
-            return
-        _, clock, _ = check_items
-        # update task instance
-        if (
-                tproxy.HasField('clock_trigger')
-                and tproxy.clock_trigger.satisfied is not clock
-        ):
-            update_time = time()
-            tp_delta = self.updated[TASK_PROXIES].setdefault(
-                tp_id, PbTaskProxy(id=tp_id))
-            tp_delta.stamp = f'{tp_id}@{update_time}'
-            tp_delta.clock_trigger.satisfied = clock
-            self.updates_pending = True
-
-    def delta_task_ext_trigger(self, itask, trig, message, satisfied):
+    def delta_task_ext_trigger(
+        self,
+        itask: TaskProxy,
+        trig: str,
+        message: str,
+        satisfied: bool,
+    ) -> None:
         """Create delta for change in task proxy external_trigger.
 
         Args:
             itask (cylc.flow.task_proxy.TaskProxy):
                 Update task-node from corresponding task proxy
                 objects from the workflow task pool.
             trig (str): Trigger ID.
             message (str): Trigger message.
 
         """
-        tp_id, tproxy = self.store_node_fetcher(itask.tdef.name, itask.point)
+        tp_id, tproxy = self.store_node_fetcher(itask.tokens)
         if not tproxy:
             return
         # update task instance
         update_time = time()
         tp_delta = self.updated[TASK_PROXIES].setdefault(
             tp_id, PbTaskProxy(id=tp_id))
         tp_delta.stamp = f'{tp_id}@{update_time}'
@@ -2162,22 +2178,17 @@
             xtrigger.satisfied = satisfied
             xtrigger.time = update_time
             self.updates_pending = True
 
     # -----------
     # Job Deltas
     # -----------
-    def delta_job_msg(self, job_d, msg):
+    def delta_job_msg(self, tokens: Tokens, msg: str) -> None:
         """Add message to job."""
-        tokens = Tokens(job_d, relative=True)
-        j_id, job = self.store_node_fetcher(
-            tokens['task'],
-            tokens['cycle'],
-            tokens['job'],
-        )
+        j_id, job = self.store_node_fetcher(tokens)
         if not job:
             return
         j_delta = self.updated[JOBS].setdefault(
             j_id,
             PbJob(id=j_id)
         )
         j_delta.stamp = f'{j_id}@{time()}'
@@ -2185,92 +2196,80 @@
         if j_delta.messages:
             j_delta.messages.append(msg)
         else:
             j_delta.messages[:] = job.messages
             j_delta.messages.append(msg)
         self.updates_pending = True
 
-    def delta_job_attr(self, job_d, attr_key, attr_val):
+    def delta_job_attr(
+        self,
+        tokens: Tokens,
+        attr_key: str,
+        attr_val: Any,
+    ) -> None:
         """Set job attribute."""
-        tokens = Tokens(job_d, relative=True)
-        j_id, job = self.store_node_fetcher(
-            tokens['task'],
-            tokens['cycle'],
-            tokens['job'],
-        )
+        j_id, job = self.store_node_fetcher(tokens)
         if not job:
             return
         j_delta = PbJob(stamp=f'{j_id}@{time()}')
         setbuff(j_delta, attr_key, attr_val)
         self.updated[JOBS].setdefault(
             j_id,
             PbJob(id=j_id)
         ).MergeFrom(j_delta)
         self.updates_pending = True
 
-    def delta_job_state(self, job_d, status):
+    def delta_job_state(
+        self,
+        tokens: Tokens,
+        status: str,
+    ) -> None:
         """Set job state."""
-        tokens = Tokens(job_d, relative=True)
-        j_id, job = self.store_node_fetcher(
-            tokens['task'],
-            tokens['cycle'],
-            tokens['job'],
-        )
+        j_id, job = self.store_node_fetcher(tokens)
         if not job or status not in JOB_STATUS_SET:
             return
         j_delta = PbJob(
             stamp=f'{j_id}@{time()}',
             state=status
         )
         self.updated[JOBS].setdefault(
             j_id,
             PbJob(id=j_id)
         ).MergeFrom(j_delta)
         self.updates_pending = True
 
-    def delta_job_time(self, job_d, event_key, time_str=None):
+    def delta_job_time(
+        self,
+        tokens: Tokens,
+        event_key: str,
+        time_str: Optional[str] = None,
+    ) -> None:
         """Set an event time in job pool object.
 
         Set values of both event_key + '_time' and event_key + '_time_string'.
         """
-        tokens = Tokens(job_d, relative=True)
-        j_id, job = self.store_node_fetcher(
-            tokens['task'],
-            tokens['cycle'],
-            tokens['job'],
-        )
+        j_id, job = self.store_node_fetcher(tokens)
         if not job:
             return
         j_delta = PbJob(stamp=f'{j_id}@{time()}')
         time_attr = f'{event_key}_time'
         setbuff(j_delta, time_attr, time_str)
         self.updated[JOBS].setdefault(
             j_id,
             PbJob(id=j_id)
         ).MergeFrom(j_delta)
         self.updates_pending = True
 
-    def store_node_fetcher(
-            self, name, point=None, sub_num=None, node_type=TASK_PROXIES):
+    def store_node_fetcher(self, tokens: Tokens) -> Tuple[str, Any]:
         """Check that task proxy is in or being added to the store"""
-        if point is None:
-            node_id = self.definition_id(name)
-            node_type = TASKS
-        elif sub_num is None:
-            node_id = self.id_.duplicate(
-                cycle=str(point),
-                task=name,
-            ).id
-        else:
-            node_id = self.id_.duplicate(
-                cycle=str(point),
-                task=name,
-                job=str(sub_num),
-            ).id
-            node_type = JOBS
+        node_type = {
+            'task': TASK_PROXIES,
+            'job': JOBS,
+        }[tokens.lowest_token]
+        node_id = tokens.id
         if node_id in self.added[node_type]:
             return (node_id, self.added[node_type][node_id])
         elif node_id in self.data[self.workflow_id][node_type]:
             return (node_id, self.data[self.workflow_id][node_type][node_id])
         return (node_id, False)
 
     def batch_deltas(self, reloaded=False):
```

### Comparing `cylc-flow-8.1.4/cylc/flow/dbstatecheck.py` & `cylc-flow-8.2.0/cylc/flow/dbstatecheck.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/cylc` & `cylc-flow-8.2.0/cylc/flow/etc/cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/cylc-completion.bash` & `cylc-flow-8.2.0/cylc/flow/etc/cylc-completion.bash`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/job.sh` & `cylc-flow-8.2.0/cylc/flow/etc/job.sh`

 * *Files 1% similar despite different names*

```diff
@@ -127,16 +127,16 @@
     export CYLC_TASK_WORK_PATH="${CYLC_TASK_WORK_DIR}"
 
     # Send task started message
     cylc message -- "${CYLC_WORKFLOW_ID}" "${CYLC_TASK_JOB}" 'started' &
     CYLC_TASK_MESSAGE_STARTED_PID=$!
     # System paths:
     # * workflow directory (installed run-dir first).
-    export PATH="${CYLC_WORKFLOW_RUN_DIR}/bin:${PATH}"
-    export PYTHONPATH="${CYLC_WORKFLOW_RUN_DIR}/lib/python:${PYTHONPATH:-}"
+    export PATH="${CYLC_WORKFLOW_RUN_DIR}/share/bin:${CYLC_WORKFLOW_RUN_DIR}/bin:${PATH}"
+    export PYTHONPATH="${CYLC_WORKFLOW_RUN_DIR}/share/lib/python:${CYLC_WORKFLOW_RUN_DIR}/lib/python:${PYTHONPATH:-}"
     # Create share and work directories
     mkdir -p "${CYLC_WORKFLOW_SHARE_DIR}" || true
     mkdir -p "$(dirname "${CYLC_TASK_WORK_DIR}")" || true
     mkdir -p "${CYLC_TASK_WORK_DIR}"
     cd "${CYLC_TASK_WORK_DIR}"
     # Env-Script, User Environment, Pre-Script, Script and Post-Script
     # Run user scripts in subshell to protect cylc job script from interference.
```

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/syntax/cylc-mode.el` & `cylc-flow-8.2.0/cylc/flow/etc/syntax/cylc-mode.el`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/syntax/cylc.lang` & `cylc-flow-8.2.0/cylc/flow/etc/syntax/cylc.lang`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/syntax/cylc.vim` & `cylc-flow-8.2.0/cylc/flow/etc/syntax/cylc.vim`

 * *Files 18% similar despite different names*

```diff
@@ -40,66 +40,76 @@
 syn region myFold start='\_^ *\[\(\w\| \)' end='\_^ *\ze\[\(\w\| \)' transparent fold
 
 " note contained items are only recognized inside containing items
 syn match lineCon "\\$"
 syn match badLineCon "\\ \+$"
 syn match trailingWS " \+\(\n\)\@="
 
-syn region jinja2 start='{%' end='%}'
-syn region jinja2 start='{{' end='}}'
-syn region jinja2 start='{#' end='#}'
+syn region jinja2Block start='{%' end='%}'
+syn region jinja2Print start='{{' end='}}'
+syn region jinja2Comment start='{#' end='#}'
 
 syn region empy start='@\[' end=']'
 syn region empy start='@{' end='}'
 syn region empy start='@(' end=')'
 
-syn region cylcSection start='\[' end='\]' contains=trailingWS,lineCon,badLineCon,jinja2,empy
-syn region cylcSection start='\[\[' end='\]\]' contains=trailingWS,lineCon,badLineCon,jinja2,empy
-syn region cylcSection start='\[\[\[' end='\]\]\]' contains=trailingWS,lineCon,badLineCon,jinja2,empy
+syn region cylcSection start='\[' end='\]' contains=trailingWS,lineCon,badLineCon,jinja2Block,jinja2Print,jinja2Comment,empy
+syn region cylcSection start='\[\[' end='\]\]' contains=trailingWS,lineCon,badLineCon,jinja2Block,jinja2Print,jinja2Comment,empy
+syn region cylcSection start='\[\[\[' end='\]\]\]' contains=trailingWS,lineCon,badLineCon,jinja2Block,jinja2Print,jinja2Comment,empy
 
-syn match cylcItem ' *\zs\(\w\| \|\-\)*\> *=\@='
+syn match cylcItem ' *\zs\(\w\|+\|\/\| \|\-\)*\> *=\@='
 syn match cylcEquals '='
 
 syn match trigger /=>/ contained
-syn match output /:[a-zA-Z0-9-]*\>/ contained
+syn match xtrigger /@[a-zA-Z0-9_-]*/ contained
+syn match parameter /<[^>]*>/ contained
+syn match output /:[a-zA-Z0-9_-]*\>/ contained
 syn match suicide /\!\w\+/ contained
 syn match offset /\[.\{-}\]/ contained
+syn match optional /?/ contained
 
 "file inclusion:
-syn match cylcInclude '%include *\(\w\|\-\|\/\|\.\)*'
+syn match cylcInclude '%include *\(\w\|"\| \|\-\|\/\|\.\)*'
 "inlined file markers:
 syn match cylcInclude '\_^!\{1,}'
 syn match cylcInclude '.*\(START INLINED\|END INLINED\).*'
 
 syn match cylcToDo /[Tt][Oo][Dd][Oo]/
+syn match cylcToDo /[Ff][Ii][Xx][Mm][Ee]/
 
 syn match empyVariable /@[a-zA-Z0-9]\+/
 syn match empyComment /@#.*/ contains=trailingWS,cylcToDo,lineCon,badLineCon
-syn match cylcComment /#.*/ contains=trailingWS,cylcToDo,lineCon,badLineCon,jinja2,empy
+syn match cylcComment /#.*/ contains=trailingWS,cylcToDo,lineCon,badLineCon,jinja2Block,jinja2Print,jinja2Comment,empy
 
-syn region cylcString start=+'+ skip=+\\'+ end=+'+ contains=trailingWS,lineCon,badLineCon,jinja2,empy,cylcToDo
-syn region cylcString start=+"+ skip=+\\"+ end=+"+ contains=trailingWS,lineCon,badLineCon,jinja2,empy,cylcToDo
-syn region cylcString start=+=\@<= *"""+ end=+"""+ contains=trailingWS,lineCon,badLineCon,jinja2,empy,empyComment,cylcComment,trigger,output,suicide,offset,cylcToDo
-syn region cylcString start=+=\@<= *'''+ end=+'''+ contains=trailingWS,lineCon,badLineCon,jinja2,empy,empyComment,cylcComment,trigger,output,suicide,offset,cylcToDo
+syn region cylcString start=+'+ skip=+\\'+ end=+'+ contains=trailingWS,lineCon,badLineCon,jinja2Block,jinja2Print,jinja2Comment,empy,cylcToDo
+syn region cylcString start=+"+ skip=+\\"+ end=+"+ contains=trailingWS,lineCon,badLineCon,jinja2Block,jinja2Print,jinja2Comment,empy,cylcToDo
+syn region cylcString start=+=\@<= *"""+ end=+"""+ contains=trailingWS,lineCon,badLineCon,jinja2Block,jinja2Print,jinja2Comment,empy,empyComment,cylcComment,optional,trigger,output,suicide,offset,cylcToDo,xtrigger,parameter
+syn region cylcString start=+=\@<= *'''+ end=+'''+ contains=trailingWS,lineCon,badLineCon,jinja2Block,jinja2Print,jinja2Comment,empy,empyComment,cylcComment,optional,trigger,output,suicide,offset,cylcToDo,xtrigger,parameter
 
 "de-emphasize strings as quoting is irrelevant in cylc
 hi def link cylcString Normal
 
 hi def link cylcSection Statement
 hi def link cylcItem Type
 hi def link cylcComment Comment
 
 hi def link lineCon Constant
 hi def link badLineCon Error
 hi def link trailingWS Underlined
 
 hi def link cylcToDo Todo
-hi def link cylcInclude MatchParen
-hi def link jinja2 CursorColumn
-hi def link empy CursorColumn
+hi def link cylcInclude Include
+hi def link jinja2Block PreProc
+hi def link jinja2Print PreProc
+hi def link jinja2Comment Comment
+hi def link empy PreProc
 hi def link empyComment CursorColumn
-hi def link empyVariable CursorColumn
+hi def link empyVariable PreProc
 hi def link cylcEquals LineNr
-hi def link output Special
+hi def link output Identifier
 hi def link suicide Special
 hi def link offset Special
 hi def link trigger Constant
+hi def link optional Type
+
+hi def link xtrigger Function
+hi def link parameter Function
```

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/syntax/cylc.xml` & `cylc-flow-8.2.0/cylc/flow/etc/syntax/cylc.xml`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/.validate` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/forecast-script/forecast` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/forecast-script/forecast`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/forecast-script/util.py` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/forecast-script/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/map-template/map-template.html` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/map-template/map-template.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/retries-tutorial/.validate` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/retries-tutorial/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-introduction/.validate` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-introduction/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/runtime-tutorial/runtime` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/runtime-tutorial/runtime`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/test-data/rainfall.csv` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/test-data/rainfall.csv`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv` & `cylc-flow-8.2.0/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/exceptions.py` & `cylc-flow-8.2.0/cylc/flow/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,14 +131,18 @@
 
 
 class WorkflowFilesError(CylcError):
     """Exception for errors related to workflow files/directories."""
     bullet = "\n    -"
 
 
+class ContactFileExists(CylcError):
+    """Workflow contact file exists."""
+
+
 def handle_rmtree_err(
     function: Callable,
     path: str,
     excinfo: Tuple[Type[Exception], Exception, object]
 ) -> NoReturn:
     """Error handler for shutil.rmtree."""
     exc = excinfo[1]
```

### Comparing `cylc-flow-8.1.4/cylc/flow/flags.py` & `cylc-flow-8.2.0/cylc/flow/flags.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/flow_mgr.py` & `cylc-flow-8.2.0/cylc/flow/flow_mgr.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,18 @@
         """
         self.counter = self.db_mgr.pri_dao.select_workflow_flows_max_flow_num()
         self.flows = self.db_mgr.pri_dao.select_workflow_flows(flow_nums)
         self._log()
 
     def _log(self) -> None:
         """Write current flow info to log."""
+        if not self.flows:
+            LOG.info("Flows: (none)")
+            return
+
         LOG.info(
             "Flows:\n" + "\n".join(
                 (
                     f"flow: {f} "
                     f"({self.flows[f]['description']}) "
                     f"{self.flows[f]['start_time']}"
                 )
```

### Comparing `cylc-flow-8.1.4/cylc/flow/graph_parser.py` & `cylc-flow-8.2.0/cylc/flow/graph_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,28 @@
     TASK_OUTPUT_SUCCEEDED,
     TASK_OUTPUT_STARTED,
     TASK_OUTPUT_FAILED,
     TASK_OUTPUT_FINISHED,
     TASK_OUTPUT_SUBMITTED,
     TASK_OUTPUT_SUBMIT_FAILED
 )
+from cylc.flow.task_qualifiers import (
+    QUAL_FAM_SUCCEED_ALL,
+    QUAL_FAM_SUCCEED_ANY,
+    QUAL_FAM_FAIL_ALL,
+    QUAL_FAM_FAIL_ANY,
+    QUAL_FAM_FINISH_ALL,
+    QUAL_FAM_FINISH_ANY,
+    QUAL_FAM_START_ALL,
+    QUAL_FAM_START_ANY,
+    QUAL_FAM_SUBMIT_ALL,
+    QUAL_FAM_SUBMIT_ANY,
+    QUAL_FAM_SUBMIT_FAIL_ALL,
+    QUAL_FAM_SUBMIT_FAIL_ANY,
+)
 
 
 class Replacement:
     """A class to remember match group information in re.sub() calls"""
     def __init__(self, replacement):
         self.replacement = replacement
         self.substitutions = []
@@ -98,27 +112,14 @@
     OPTIONAL = '?'
     QUALIFIER = ':'
     ARROW = '=>'
     XTRIG = '@'
     CONTINUATION_STRS = (ARROW, OP_AND, OP_OR)
     BAD_STRS = (OP_AND_ERR, OP_OR_ERR)
 
-    QUAL_FAM_SUCCEED_ALL = "succeed-all"
-    QUAL_FAM_SUCCEED_ANY = "succeed-any"
-    QUAL_FAM_FAIL_ALL = "fail-all"
-    QUAL_FAM_FAIL_ANY = "fail-any"
-    QUAL_FAM_FINISH_ALL = "finish-all"
-    QUAL_FAM_FINISH_ANY = "finish-any"
-    QUAL_FAM_START_ALL = "start-all"
-    QUAL_FAM_START_ANY = "start-any"
-    QUAL_FAM_SUBMIT_ALL = "submit-all"
-    QUAL_FAM_SUBMIT_ANY = "submit-any"
-    QUAL_FAM_SUBMIT_FAIL_ALL = "submit-fail-all"
-    QUAL_FAM_SUBMIT_FAIL_ANY = "submit-fail-any"
-
     # Map family trigger type to (member-trigger, any/all), for use in
     # expanding family trigger expressions to member trigger expressions.
     # - "FAM:succeed-all => g" means "f1:succeed & f2:succeed => g"
     # - "FAM:fail-any => g" means "f1:fail | f2:fail => g".
     # E.g. QUAL_FAM_START_ALL: (TASK_OUTPUT_STARTED, True) simply maps
     #   "FAM:start-all" to "MEMBER:started" and "-all" (all members).
     fam_to_mem_trigger_map: Dict[str, Tuple[str, bool]] = {
@@ -856,15 +857,15 @@
 
             if name in self.family_map:
                 fam = True
                 mems = self.family_map[name]
                 if not output:
                     # (Plain family name on RHS).
                     # Make implicit success explicit.
-                    output = self.__class__.QUAL_FAM_SUCCEED_ALL
+                    output = QUAL_FAM_SUCCEED_ALL
                 elif output.startswith("finish"):
                     if optional:
                         raise GraphParseError(
                             f"Family pseudo-output {name}:{output} can't be"
                             " optional")
                     # But implicit optional for the real succeed/fail outputs.
                     optional = True
```

### Comparing `cylc-flow-8.1.4/cylc/flow/graphnode.py` & `cylc-flow-8.2.0/cylc/flow/graphnode.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/host_select.py` & `cylc-flow-8.2.0/cylc/flow/host_select.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/hostuserutil.py` & `cylc-flow-8.2.0/cylc/flow/hostuserutil.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/id.py` & `cylc-flow-8.2.0/cylc/flow/id.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,20 +148,24 @@
         if self.is_null:
             id_ = ''
         else:
             id_ = self.id
         return f'<id: {id_}>'
 
     def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
         return all(
             self[key] == other[key]
             for key in self._KEYS
         )
 
     def __ne__(self, other):
+        if not isinstance(other, self.__class__):
+            return True
         return any(
             self[key] != other[key]
             for key in self._KEYS
         )
 
     @property # noqa A003 (not shadowing id built-in)
     def id(self) -> str:  # noqa A003 (not shadowing id built-in)
@@ -537,14 +541,29 @@
         )?
         $
     ''',
     re.X
 )
 
 
+def quick_relative_detokenise(cycle, task):
+    """Generate a relative ID for a task.
+
+    This is a more efficient solution to `Tokens` for cases where
+    you only want the ID string and don't have any use for a Tokens object.
+
+    Example:
+        >>> q = quick_relative_detokenise
+        >>> q('1', 'a') == Tokens(cycle='1', task='a').relative_id
+        True
+
+    """
+    return f'{cycle}/{task}'
+
+
 def _dict_strip(dictionary):
     """Run str.strip against dictionary values.
 
     Examples:
         >>> _dict_strip({'a': ' x ', 'b': 'x', 'c': None})
         {'a': 'x', 'b': 'x', 'c': None}
```

### Comparing `cylc-flow-8.1.4/cylc/flow/id_cli.py` & `cylc-flow-8.2.0/cylc/flow/id_cli.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/id_match.py` & `cylc-flow-8.2.0/cylc/flow/id_match.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/install_plugins/__init__.py` & `cylc-flow-8.2.0/cylc/flow/install_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/install_plugins/log_vc_info.py` & `cylc-flow-8.2.0/cylc/flow/install_plugins/log_vc_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,21 +62,24 @@
 import json
 from pathlib import Path
 from subprocess import Popen, DEVNULL, PIPE
 from typing import (
     Any, Dict, Iterable, List, Optional, TYPE_CHECKING, TextIO, Union, overload
 )
 
-from cylc.flow import LOG
+from cylc.flow import LOG as _LOG, LoggerAdaptor
 from cylc.flow.exceptions import CylcError
+import cylc.flow.flags
 from cylc.flow.workflow_files import WorkflowFiles
 
 if TYPE_CHECKING:
     from optparse import Values
 
+LOG = LoggerAdaptor(_LOG, {'prefix': __name__})
+
 
 SVN = 'svn'
 GIT = 'git'
 
 INFO_COMMANDS: Dict[str, List[str]] = {
     SVN: ['info', '--non-interactive'],
     GIT: ['describe', '--always', '--dirty']
@@ -158,22 +161,22 @@
         except VCSNotInstalledError as exc:
             LOG.debug(exc)
             continue
         except VCSMissingBaseError as exc:
             missing_base = True
             LOG.debug(exc)
         except OSError as exc:
-            if not any(
+            if any(
                 exc.strerror.lower().startswith(err)
                 for err in NOT_REPO_ERRS[vcs]
             ):
-                raise exc
-            else:
                 LOG.debug(f"Source dir {path} is not a {vcs} repository")
-                continue
+            elif cylc.flow.flags.verbosity > -1:
+                LOG.warning(f"$ {vcs} {' '.join(args)}\n{exc}")
+            continue
 
         info['version control system'] = vcs
         if vcs == SVN:
             info.update(_parse_svn_info(out))
         elif vcs == GIT:
             if not missing_base:
                 info['repository version'] = out.splitlines()[0]
```

### Comparing `cylc-flow-8.1.4/cylc/flow/jinja/filters/duration_as.py` & `cylc-flow-8.2.0/cylc/flow/jinja/filters/duration_as.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/jinja/filters/pad.py` & `cylc-flow-8.2.0/cylc/flow/jinja/filters/pad.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/jinja/filters/strftime.py` & `cylc-flow-8.2.0/cylc/flow/jinja/filters/strftime.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/job_file.py` & `cylc-flow-8.2.0/cylc/flow/job_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,21 @@
 
 from cylc.flow import __version__ as CYLC_VERSION
 from cylc.flow.job_runner_mgr import JobRunnerManager
 import cylc.flow.flags
 from cylc.flow.option_parsers import verbosity_to_env
 from cylc.flow.config import interpolate_template, ParamExpandError
 
+# the maximum number of task dependencies which Cylc will list before
+# omitting the CYLC_TASK_DEPENDENCIES environment variable
+# see: https://github.com/cylc/cylc-flow/issues/5551
+# NOTE: please update `src/reference/job-script-vars/var-list.txt`
+#       in cylc-doc if changing this value
+MAX_CYLC_TASK_DEPENDENCIES_LEN = 50
+
 
 class JobFileWriter:
 
     """Write job files."""
 
     def __init__(self):
         self.workflow_env = {}
@@ -216,17 +223,26 @@
 
         handle.write("\n\n    # CYLC TASK ENVIRONMENT:")
         handle.write(f"\n    export CYLC_TASK_COMMS_METHOD={comm_meth}")
         handle.write('\n    export CYLC_TASK_JOB="%s"' % job_conf['job_d'])
         handle.write(
             '\n    export CYLC_TASK_NAMESPACE_HIERARCHY="%s"' %
             ' '.join(job_conf['namespace_hierarchy']))
-        handle.write(
-            '\n    export CYLC_TASK_DEPENDENCIES="%s"' %
-            ' '.join(job_conf['dependencies']))
+        if len(job_conf['dependencies']) <= MAX_CYLC_TASK_DEPENDENCIES_LEN:
+            handle.write(
+                '\n    export CYLC_TASK_DEPENDENCIES="%s"' %
+                ' '.join(job_conf['dependencies']))
+        else:
+            # redact the CYLC_TASK_DEPENDENCIES variable but leave a note
+            # explaining why
+            # see: https://github.com/cylc/cylc-flow/issues/5551
+            handle.write(
+                '\n    # CYLC_TASK_DEPENDENCIES=disabled'
+                f' (more than {MAX_CYLC_TASK_DEPENDENCIES_LEN} dependencies)'
+            )
         handle.write(
             '\n    export CYLC_TASK_TRY_NUMBER=%s' % job_conf['try_num'])
         handle.write(
             "\n    export CYLC_TASK_FLOW_NUMBERS="
             f"{','.join(str(f) for f in job_conf['flow_nums'])}"
         )
         # Standard parameter environment variables
```

### Comparing `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/__init__.py` & `cylc-flow-8.2.0/cylc/flow/job_runner_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/at.py` & `cylc-flow-8.2.0/cylc/flow/job_runner_handlers/at.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/background.py` & `cylc-flow-8.2.0/cylc/flow/job_runner_handlers/background.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/documentation.py` & `cylc-flow-8.2.0/cylc/flow/job_runner_handlers/documentation.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/loadleveler.py` & `cylc-flow-8.2.0/cylc/flow/job_runner_handlers/loadleveler.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/lsf.py` & `cylc-flow-8.2.0/cylc/flow/job_runner_handlers/lsf.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/moab.py` & `cylc-flow-8.2.0/cylc/flow/job_runner_handlers/moab.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/pbs.py` & `cylc-flow-8.2.0/cylc/flow/job_runner_handlers/pbs.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     #         job name length maximum = 15
     JOB_NAME_LEN_MAX = 236
     KILL_CMD_TMPL = "qdel '%(job_id)s'"
     # N.B. The "qstat JOB_ID" command returns 1 if JOB_ID is no longer in the
     # system, so there is no need to filter its output.
     POLL_CMD = "qstat"
     POLL_CANT_CONNECT_ERR = "Connection refused"
-    REC_ID_FROM_SUBMIT_OUT = re.compile(r"""\A\s*(?P<id>\S+)\s*\Z""")
+    REC_ID_FROM_SUBMIT_OUT = re.compile(r"^\s*(?P<id>\d+)", re.M)
     SUBMIT_CMD_TMPL = "qsub '%(job)s'"
 
     def format_directives(self, job_conf):
         """Format the job directives for a job file."""
         job_file_path = job_conf['job_file_path']
         directives = job_conf["directives"].__class__()  # an ordereddict
         # Change task/runM to task-runM in the job name
@@ -119,9 +119,14 @@
                 # E.g. -q queue_name
                 lines.append("%s%s %s" % (self.DIRECTIVE_PREFIX, key, value))
             else:
                 # E.g. -V
                 lines.append(self.DIRECTIVE_PREFIX + key)
         return lines
 
+    @classmethod
+    def filter_poll_many_output(cls, out):
+        """Strip trailing stuff from the job ID."""
+        return cls.REC_ID_FROM_SUBMIT_OUT.findall(out)
+
 
 JOB_RUNNER_HANDLER = PBSHandler()
```

### Comparing `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/pbs_multi_cluster.py` & `cylc-flow-8.2.0/cylc/flow/job_runner_handlers/pbs_multi_cluster.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/sge.py` & `cylc-flow-8.2.0/cylc/flow/job_runner_handlers/sge.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/slurm.py` & `cylc-flow-8.2.0/cylc/flow/job_runner_handlers/slurm.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/job_runner_handlers/slurm_packjob.py` & `cylc-flow-8.2.0/cylc/flow/job_runner_handlers/slurm_packjob.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/job_runner_mgr.py` & `cylc-flow-8.2.0/cylc/flow/job_runner_mgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,15 +399,16 @@
         if source == "01":
             for name in os.listdir(task_log_dir):
                 if name != source and name.isdigit():
                     # Ignore errors, not disastrous if rmtree fails
                     rmtree(
                         os.path.join(task_log_dir, name), ignore_errors=True)
 
-    def _filter_submit_output(self, st_file_path, job_runner, out, err):
+    @classmethod
+    def _filter_submit_output(cls, st_file_path, job_runner, out, err):
         """Filter submit command output, if relevant."""
         job_id = None
         if hasattr(job_runner, "REC_ID_FROM_SUBMIT_ERR"):
             text = err
             rec_id = job_runner.REC_ID_FROM_SUBMIT_ERR
         elif hasattr(job_runner, "REC_ID_FROM_SUBMIT_OUT"):
             text = out
@@ -417,17 +418,17 @@
                 match = rec_id.match(line)
                 if match:
                     job_id = match.group("id")
                     if hasattr(job_runner, "manip_job_id"):
                         job_id = job_runner.manip_job_id(job_id)
                     with open(st_file_path, "a") as job_status_file:
                         job_status_file.write("{0}={1}\n".format(
-                            self.CYLC_JOB_ID, job_id))
+                            cls.CYLC_JOB_ID, job_id))
                         job_status_file.write("{0}={1}\n".format(
-                            self.CYLC_JOB_RUNNER_SUBMIT_TIME,
+                            cls.CYLC_JOB_RUNNER_SUBMIT_TIME,
                             get_current_time_string()))
                     break
         if hasattr(job_runner, "filter_submit_output"):
             out, err = job_runner.filter_submit_output(out, err)
         return out, err, job_id
 
     def _jobs_poll_status_files(self, job_log_root, job_log_dir):
```

### Comparing `cylc-flow-8.1.4/cylc/flow/listify.py` & `cylc-flow-8.2.0/cylc/flow/listify.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/log_diagnosis.py` & `cylc-flow-8.2.0/cylc/flow/log_diagnosis.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/loggingutil.py` & `cylc-flow-8.2.0/cylc/flow/loggingutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,19 +329,19 @@
 def re_formatter(log_string):
     """Read in an uncoloured log_string file and apply colour formatting."""
     for sub, repl in LOG_LEVEL_REGEXES:
         log_string = sub.sub(repl, log_string)
     return log_string
 
 
-def disable_timestamps(logger: logging.Logger) -> None:
-    """For readability omit timestamps from logging."""
+def set_timestamps(logger: logging.Logger, enable: bool) -> None:
+    """Enable or disable logging timestamps."""
     for handler in logger.handlers:
         if isinstance(handler.formatter, CylcLogFormatter):
-            handler.formatter.configure(timestamp=False)
+            handler.formatter.configure(timestamp=enable)
 
 
 def setup_segregated_log_streams(
     logger: logging.Logger, stderr_handler: logging.StreamHandler
 ) -> None:
     """Set up a logger so that info and debug messages get printed to stdout,
     while warnings and above get printed to stderr.
```

### Comparing `cylc-flow-8.1.4/cylc/flow/main_loop/__init__.py` & `cylc-flow-8.2.0/cylc/flow/main_loop/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,21 +123,20 @@
 For examples see the built-in plugins in the :py:mod:`cylc.flow.main_loop`
 module which are registered in the Cylc Flow ``setup.cfg`` file.
 
 Coroutines
 ^^^^^^^^^^
 
 .. _coroutines: https://docs.python.org/3/library/asyncio-task.html#coroutines
-.. _aiofiles: https://github.com/Tinche/aiofiles
 
 Plugins provide asynchronous functions (`coroutines`_) which Cylc will
 then run inside the scheduler.
 
 Coroutines should be fast running (read as gentle on the scheduler)
-and perform IO asynchronously e.g. by using `aiofiles`_.
+and perform IO asynchronously.
 
 Coroutines shouldn't meddle with the state of the scheduler and should be
 parallel-safe with other plugins.
 
 Event Types
 ^^^^^^^^^^^
```

### Comparing `cylc-flow-8.1.4/cylc/flow/main_loop/auto_restart.py` & `cylc-flow-8.2.0/cylc/flow/main_loop/auto_restart.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/main_loop/health_check.py` & `cylc-flow-8.2.0/cylc/flow/main_loop/health_check.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/main_loop/log_data_store.py` & `cylc-flow-8.2.0/cylc/flow/main_loop/log_data_store.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/main_loop/log_db.py` & `cylc-flow-8.2.0/cylc/flow/main_loop/log_db.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/main_loop/log_main_loop.py` & `cylc-flow-8.2.0/cylc/flow/main_loop/log_main_loop.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/main_loop/log_memory.py` & `cylc-flow-8.2.0/cylc/flow/main_loop/log_memory.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/main_loop/reset_bad_hosts.py` & `cylc-flow-8.2.0/cylc/flow/main_loop/reset_bad_hosts.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/network/__init__.py` & `cylc-flow-8.2.0/cylc/flow/network/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import asyncio
 import getpass
 import json
 from typing import Optional, Tuple
 
 import zmq
 import zmq.asyncio
+import zmq.auth
 
 from cylc.flow import LOG
 from cylc.flow.exceptions import (
     ClientError,
     CylcError,
     CylcVersionError,
     ServiceFileError,
@@ -62,15 +63,15 @@
 
 def get_location(workflow: str) -> Tuple[str, int, int]:
     """Extract host and port from a workflow's contact file.
 
     NB: if it fails to load the workflow contact file, it will exit.
 
     Args:
-        workflow: workflow name
+        workflow: workflow ID
     Returns:
         Tuple (host name, port number, publish port number)
     Raises:
         WorkflowStopped: if the workflow is not running.
         CylcVersionError: if target is a Cylc 7 (or earlier) workflow.
     """
     try:
```

### Comparing `cylc-flow-8.1.4/cylc/flow/network/authentication.py` & `cylc-flow-8.2.0/cylc/flow/network/authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,20 +20,20 @@
     KeyOwner,
     KeyType,
     create_server_keys,
     get_workflow_srv_dir,
     remove_keys_on_server)
 
 
-def key_housekeeping(reg, platform=None, create=True):
+def key_housekeeping(id_, platform=None, create=True):
 
     """Clean any existing authentication keys and create new ones.
         If create is set to false, keys will only be cleaned from
         server."""
-    workflow_srv_dir = get_workflow_srv_dir(reg)
+    workflow_srv_dir = get_workflow_srv_dir(id_)
     keys = {
         "client_public_key": KeyInfo(
             KeyType.PUBLIC,
             KeyOwner.CLIENT,
             workflow_srv_dir=workflow_srv_dir, install_target=platform),
         "client_private_key": KeyInfo(
             KeyType.PRIVATE,
```

### Comparing `cylc-flow-8.1.4/cylc/flow/network/authorisation.py` & `cylc-flow-8.2.0/cylc/flow/network/authorisation.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/network/client.py` & `cylc-flow-8.2.0/cylc/flow/network/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 import zmq
 import zmq.asyncio
 
 from cylc.flow import LOG
 from cylc.flow.exceptions import (
     ClientError,
     ClientTimeout,
+    ContactFileExists,
     CylcError,
-    ServiceFileError,
     WorkflowStopped,
 )
 from cylc.flow.hostuserutil import get_fqdn_by_host
 from cylc.flow.network import (
     encode_,
     decode_,
     get_location,
@@ -143,15 +143,15 @@
                 f'It has moved to {contact_host}:{contact_port}'
             )
 
         # Cannot connect, perhaps workflow is no longer running and is leaving
         # behind a contact file?
         try:
             detect_old_contact_file(self.workflow)
-        except (AssertionError, ServiceFileError):
+        except ContactFileExists:
             # old contact file exists and the workflow process still alive
             return
         else:
             # the workflow has stopped
             raise WorkflowStopped(self.workflow)
 
 
@@ -301,27 +301,29 @@
                 ' This could be due to network or server issues.'
                 ' Check the workflow log.'
             )
 
         if msg['command'] in PB_METHOD_MAP:
             response = {'data': res}
         else:
-            response = decode_(res.decode())
+            response = decode_(
+                res.decode() if isinstance(res, bytes) else res
+            )
         LOG.debug('zmq:recv %s', response)
 
         try:
             return response['data']
         except KeyError:
             error = response.get(
                 'error',
                 {'message': f'Received invalid response: {response}'},
             )
             raise ClientError(
-                error.get('message'),
-                error.get('traceback'),
+                error.get('message'),  # type: ignore
+                error.get('traceback'),  # type: ignore
             )
 
     def get_header(self) -> dict:
         """Return "header" data to attach to each request for traceability.
 
         Returns:
             dict: dictionary with the header information, such as
```

### Comparing `cylc-flow-8.1.4/cylc/flow/network/client_factory.py` & `cylc-flow-8.2.0/cylc/flow/network/client_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     workflow: str,
     timeout: Union[float, str, None] = None
 ) -> 'WorkflowRuntimeClientBase':
     """Return client for the provided communication method.
 
         Args:
             comm_method: communication method
-            workflow: workflow name
+            workflow: workflow ID
     """
     if comms_method == CommsMeth.SSH:
         from cylc.flow.network.ssh_client import WorkflowRuntimeClient
     else:
         from cylc.flow.network.client import (  # type: ignore[assignment]
             WorkflowRuntimeClient
         )
```

### Comparing `cylc-flow-8.1.4/cylc/flow/network/graphql.py` & `cylc-flow-8.2.0/cylc/flow/network/graphql.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/network/multi.py` & `cylc-flow-8.2.0/cylc/flow/network/multi.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/network/publisher.py` & `cylc-flow-8.2.0/cylc/flow/network/publisher.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/network/replier.py` & `cylc-flow-8.2.0/cylc/flow/network/replier.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/network/resolvers.py` & `cylc-flow-8.2.0/cylc/flow/network/resolvers.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/network/scan.py` & `cylc-flow-8.2.0/cylc/flow/network/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -532,25 +532,17 @@
 @pipe
 async def workflow_params(flow):
     """Extract workflow parameter entries from the workflow database.
 
     Requires:
         * is_active(True)
     """
-    params = {}
-
-    def _callback(_, entry):
-        nonlocal params
-        key, value = entry
-        params[key] = value
-
     # NOTE: use the public DB for reading
     # (only the scheduler process/thread should access the private database)
     db_file = Path(get_workflow_run_dir(
         flow['name'], WorkflowFiles.LogDir.DIRNAME, WorkflowFiles.LogDir.DB
     ))
     if db_file.exists():
         with CylcWorkflowDAO(db_file, is_public=True) as dao:
-            dao.select_workflow_params(_callback)
-            flow['workflow_params'] = params
+            flow['workflow_params'] = dict(dao.select_workflow_params())
 
     return flow
```

### Comparing `cylc-flow-8.1.4/cylc/flow/network/schema.py` & `cylc-flow-8.2.0/cylc/flow/network/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -602,109 +602,193 @@
     string_extended = String()
 
 
 class Workflow(ObjectType):
     class Meta:
         description = """Global workflow info."""
     id = ID()  # noqa: A003 (required for definition)
-    name = String()
-    status = String()
-    status_msg = String()
-    host = String()
-    port = Int()
-    pub_port = Int()
-    owner = String()
+    name = String(
+        description='The workflow ID with the ~user/ prefix removed.',
+    )
+    status = String(
+        description='The workflow status e.g. `running`.',
+    )
+    status_msg = String(
+        description='A description of the workflow status.',
+    )
+    host = String(
+        description='The host where the scheduler process is running.',
+    )
+    port = Int(
+        description='The port for sending ZMQ requests to the scheduler.',
+    )
+    pub_port = Int(
+        description=sstrip('''
+            The port for subscribing to ZMQ updates from the scheduler.
+        '''),
+    )
+    owner = String(
+        description='The user account that the workflow is running under.',
+    )
     tasks = graphene.List(
         lambda: Task,
-        description="""Task definitions.""",
+        description="Task definitions.",
         args=DEF_ARGS,
         strip_null=STRIP_NULL_DEFAULT,
         delta_store=DELTA_STORE_DEFAULT,
         delta_type=DELTA_TYPE_DEFAULT,
-        resolver=get_nodes_by_ids)
+        resolver=get_nodes_by_ids,
+    )
     families = graphene.List(
         lambda: Family,
-        description="""Family definitions.""",
+        description="Family definitions.",
         args=DEF_ARGS,
         strip_null=STRIP_NULL_DEFAULT,
         delta_store=DELTA_STORE_DEFAULT,
         delta_type=DELTA_TYPE_DEFAULT,
-        resolver=get_nodes_by_ids)
+        resolver=get_nodes_by_ids,
+    )
     task_proxies = graphene.List(
         lambda: TaskProxy,
-        description="""Task cycle instances.""",
+        description="Task instances.",
         args=PROXY_ARGS,
         strip_null=STRIP_NULL_DEFAULT,
         delta_store=DELTA_STORE_DEFAULT,
         delta_type=DELTA_TYPE_DEFAULT,
-        resolver=get_nodes_by_ids)
+        resolver=get_nodes_by_ids,
+    )
     family_proxies = graphene.List(
         lambda: FamilyProxy,
-        description="""Family cycle instances.""",
+        description="Family instances.",
         args=PROXY_ARGS,
         strip_null=STRIP_NULL_DEFAULT,
         delta_store=DELTA_STORE_DEFAULT,
         delta_type=DELTA_TYPE_DEFAULT,
-        resolver=get_nodes_by_ids)
+        resolver=get_nodes_by_ids,
+    )
     jobs = graphene.List(
         lambda: Job,
-        description="""Jobs.""",
+        description="Jobs.",
         args=JOB_ARGS,
         strip_null=STRIP_NULL_DEFAULT,
         delta_store=DELTA_STORE_DEFAULT,
         delta_type=DELTA_TYPE_DEFAULT,
-        resolver=get_nodes_by_ids)
+        resolver=get_nodes_by_ids,
+    )
     edges = Field(
         lambda: Edges,
         args=EDGE_ARGS,
         strip_null=STRIP_NULL_DEFAULT,
         delta_store=DELTA_STORE_DEFAULT,
         delta_type=DELTA_TYPE_DEFAULT,
-        description="""Graph edges""")
+        description="Graph edges.",
+    )
     nodes_edges = Field(
         lambda: NodesEdges,
         args=NODES_EDGES_ARGS,
         strip_null=STRIP_NULL_DEFAULT,
         delta_store=DELTA_STORE_DEFAULT,
         delta_type=DELTA_TYPE_DEFAULT,
-        resolver=get_nodes_edges)
-    api_version = Int()
-    cylc_version = String()
-    last_updated = Float()
-    meta = Field(NodeMeta)
-    newest_active_cycle_point = String()
-    oldest_active_cycle_point = String()
-    reloaded = Boolean()
-    run_mode = String()
-    is_held_total = Int()
-    is_queued_total = Int()
-    is_runahead_total = Int()
-    state_totals = GenericScalar(resolver=resolve_state_totals)
+        resolver=get_nodes_edges,
+        description='Graph nodes and edges.'
+    )
+    api_version = Int(
+        description='The Cylc scheduler communication protocol version number.'
+    )
+    cylc_version = String(
+        description='The Cylc version this workflow is running under.',
+    )
+    last_updated = Float(
+        description='The time of the most recent state change in the workflow.'
+    )
+    meta = Field(
+        NodeMeta,
+        description="The workflow's `[meta]` section.",
+    )
+    newest_active_cycle_point = String(
+        description='The newest cycle point which has active tasks.'
+    )
+    oldest_active_cycle_point = String(
+        description='The oldest cycle point which has active tasks.'
+    )
+    reloaded = Boolean(
+        description=sstrip('''
+            When subscribing to workflow updates, this field is `True` if the
+            update relates to a workflow reload.
+        '''),
+    )
+    run_mode = String(
+        description="The scheduler's run-mode e.g. `live`.",
+    )
+    is_held_total = Int(
+        description='The number of "held" tasks.',
+    )
+    is_queued_total = Int(
+        description='The number of queued tasks.',
+    )
+    is_runahead_total = Int(
+        description=sstrip('''
+            The number of tasks which are held back by the runahead limit.
+        ''')
+    )
+    state_totals = GenericScalar(
+        resolver=resolve_state_totals,
+        description='The number of tasks in each state as a JSON object.',
+    )
     latest_state_tasks = GenericScalar(
         states=graphene.List(
             String,
             description="List of task states to show",
             default_value=TASK_STATUSES_ORDERED),
-        resolver=resolve_state_tasks)
-    workflow_log_dir = String()
-    time_zone_info = Field(TimeZone)
-    tree_depth = Int()
-    ns_def_order = graphene.List(String)
-    job_log_names = graphene.List(String)
-    states = graphene.List(String)
+        resolver=resolve_state_tasks,
+        description='The latest tasks to have entered each task state.',
+    )
+    workflow_log_dir = String(
+        description="The path to the workflow's run directory.",
+    )
+    time_zone_info = Field(
+        TimeZone,
+        description='The scheduler time zone.',
+    )
+    tree_depth = Int()  # TODO: what is this? write description
+    ns_def_order = graphene.List(
+        String,
+        description=sstrip('''
+            Namespace definition order.
+
+            The order in which tasks were defined in the workflow
+            configuration.
+        '''),
+    )
+    job_log_names = graphene.List(
+        # TODO: remove, see https://github.com/cylc/cylc-flow/issues/5610
+        String,
+        description='Deprecated, do not use this.',
+    )
+    states = graphene.List(
+        String,
+        description=sstrip('''
+            The task states present in the workflow.
+
+            Similar to stateTotals.
+        '''),
+    )
     broadcasts = GenericScalar(
         ids=graphene.List(
             ID,
             description=sstrip('''
                 Node IDs, cycle point and/or-just family/task namespace:
                     ["1234/foo", "1234/FAM", "*/FAM"]
             '''),
-            default_value=[]),
-        resolver=resolve_broadcasts)
-    pruned = Boolean()
+            default_value=[]
+        ),
+        resolver=resolve_broadcasts,
+        description='Any active workflow broadcasts.'
+    )
+    pruned = Boolean()  # TODO: what is this? write description
 
 
 class RuntimeSetting(ObjectType):
     """Key = value setting for a `[runtime][<namespace>]` configuration."""
     key = String(default_value=None)
     value = String(default_value=None)
 
@@ -753,70 +837,125 @@
     'work_sub_dir': 'work sub-directory',
 }
 """Map GQL Runtime fields' names to workflow config setting names."""
 
 
 class Job(ObjectType):
     class Meta:
-        description = """Jobs."""
+        description = "Jobs."
+
     id = ID()  # noqa: A003 (required for definition)
-    submit_num = Int()
-    state = String()
-    # name and cycle_point for filtering/sorting
-    name = String()
-    cycle_point = String()
+    submit_num = Int(
+        description='The submission number for this job, starts at 1.',
+    )
+    state = String(
+        description='The job state e.g. `running` or `succeeded`.',
+    )
+    name = String(
+        description='The name of the task which submitted this job.',
+    )
+    cycle_point = String(
+        description='The cycle of the task which submitted this job.',
+    )
     task_proxy = Field(
         lambda: TaskProxy,
-        description="""Associated Task Proxy""",
+        description="The TaskProxy of the task which submitted this job",
         strip_null=STRIP_NULL_DEFAULT,
         delta_store=DELTA_STORE_DEFAULT,
         delta_type=DELTA_TYPE_DEFAULT,
         resolver=get_node_by_id)
-    submitted_time = String()
-    started_time = String()
-    finished_time = String()
-    job_id = ID()
-    job_runner_name = String()
-    execution_time_limit = Float()
-    platform = String()
-    job_log_dir = String()
-    extra_logs = graphene.List(String)
-    messages = graphene.List(String)
-    runtime = Field(Runtime)
+    submitted_time = String(
+        description='The time this job was submitted to the job runner.',
+    )
+    started_time = String(
+        description='The time this job started running (if it has yet).',
+    )
+    finished_time = String(
+        description='The time this job finished running (if it has yet).',
+    )
+    job_id = ID(
+        description='The ID of this job in the job runner it was submitted to.'
+    )
+    job_runner_name = String(
+        description='The job runner this job was submitted to.',
+    )
+    execution_time_limit = Float(
+        description='The time limit for this job if configured.',
+    )
+    platform = String(
+        description='The Cylc platform this job was submitted to.',
+    )
+    job_log_dir = String(
+        description="The path to the job's log directory.",
+    )
+    extra_logs = graphene.List(
+        # TODO: remove. see https://github.com/cylc/cylc-flow/issues/5610
+        String,
+        description='Obsolete, do not use.',
+    )
+    messages = graphene.List(
+        String,
+        description='The list of task messages generated by this job.',
+    )
+    runtime = Field(
+        Runtime,
+        description=sstrip('''
+            The `[runtime]` configuration of the task which submitted this job.
+        '''),
+    )
 
 
 class Task(ObjectType):
     class Meta:
-        description = """Task definition, static fields"""
+        description = sstrip("""
+            Task definitions.
+
+            These are the task "definitions" as they appear in the
+            configuration as opposed to task "instances" which you will find
+            in the `TaskProxies` field.
+        """)
+
     id = ID()  # noqa: A003 (required for definition)
-    name = String()
-    meta = Field(NodeMeta)
-    runtime = Field(Runtime)
-    mean_elapsed_time = Float()
-    depth = Int()
+    name = String(
+        description='The task name.'
+    )
+    meta = Field(
+        NodeMeta,
+        description="The task's `[meta]` section.",
+    )
+    runtime = Field(
+        Runtime,
+        description="The task's `[runtime`] section.",
+    )
+    mean_elapsed_time = Float(
+        description="The task's average runtime."
+    )
+    depth = Int(
+        description='The family inheritance depth.'
+    )
     proxies = graphene.List(
         lambda: TaskProxy,
-        description="""Associated cycle point proxies""",
+        description="Associated cycle point proxies",
         args=PROXY_ARGS,
         strip_null=STRIP_NULL_DEFAULT,
         delta_store=DELTA_STORE_DEFAULT,
         delta_type=DELTA_TYPE_DEFAULT,
         resolver=get_nodes_by_ids)
     parents = graphene.List(
         lambda: Family,
-        description="""Family definition parent.""",
+        description="Family definition parent.",
         args=DEF_ARGS,
         strip_null=STRIP_NULL_DEFAULT,
         delta_store=DELTA_STORE_DEFAULT,
         delta_type=DELTA_TYPE_DEFAULT,
         resolver=get_nodes_by_ids)
     namespace = graphene.List(String)
     first_parent = Field(
         lambda: Family,
-        description="""Task first parent.""",
+        description="Task first parent.",
         strip_null=STRIP_NULL_DEFAULT,
         delta_store=DELTA_STORE_DEFAULT,
         delta_type=DELTA_TYPE_DEFAULT,
         resolver=get_node_by_id)
 
 
 class PollTask(ObjectType):
@@ -865,22 +1004,14 @@
         description = """Task output"""
     label = String()
     message = String()
     satisfied = Boolean()
     time = Float()
 
 
-class ClockTrigger(ObjectType):
-    class Meta:
-        description = """Task clock-trigger"""
-    time = Float()
-    time_string = String()
-    satisfied = Boolean()
-
-
 class XTrigger(ObjectType):
     class Meta:
         description = """Task trigger"""
     id = String()  # noqa: A003 (required for definition)
     label = String()
     message = String()
     satisfied = Boolean()
@@ -889,94 +1020,136 @@
 
 class TaskProxy(ObjectType):
     class Meta:
         description = """Task cycle instance."""
     id = ID()  # noqa: A003 (required for schema definition)
     task = Field(
         Task,
-        description="""Task definition""",
+        description="The task definition relating to this task instance.",
         strip_null=STRIP_NULL_DEFAULT,
         delta_store=DELTA_STORE_DEFAULT,
         delta_type=DELTA_TYPE_DEFAULT,
         resolver=get_node_by_id)
-    runtime = Field(Runtime)
-    state = String()
-    cycle_point = String()
-    is_held = Boolean()
-    is_queued = Boolean()
-    is_runahead = Boolean()
-    flow_nums = String()
-    flow_wait = Boolean()
-    depth = Int()
-    job_submits = Int()
+    runtime = Field(
+        Runtime,
+        description="This task's `[runtime]` section.",
+    )
+    state = String(
+        description='The task state e.g. `running`.',
+    )
+    name = String(
+        description="The task's name.",
+    )
+    cycle_point = String(
+        description="The task's cycle point.",
+    )
+    namespace = graphene.List(
+        String,
+        description='The inheritance order for this task.',
+    )
+    is_held = Boolean(
+        description='True if this task is "held".',
+    )
+    is_queued = Boolean(
+        description=sstrip('''
+            True if this task is "queued".
+
+            This relates to Cylc's internal task queues, not a job runner
+            queue.
+        '''),
+    )
+    is_runahead = Boolean(
+        description='True if this task is held back by the "runahead limit".',
+    )
+    flow_nums = String(
+        description='The flows this task instance belongs to.',
+    )
+    flow_wait = Boolean(
+        description=sstrip('''
+            True if this task will wait for an approaching flow before spawning
+            outputs downstream.
+        '''),
+    )
+    depth = Int(
+        description='The family inheritance depth',
+    )
+    job_submits = Int(
+        description='The number of job submissions for this task instance.',
+    )
     outputs = graphene.List(
         Output,
-        description="""Task outputs.""",
+        description="Outputs this task instance has generated.",
         sort=SortArgs(default_value=None),
         sort_order=graphene.List(
             String,
             default_value=list(SORT_ORDERS)
         ),
         limit=Int(default_value=0),
         satisfied=Boolean(),
         resolver=resolve_mapping_to_list)
-    clock_trigger = Field(ClockTrigger)
     external_triggers = graphene.List(
         XTrigger,
-        description="""Task external trigger prerequisites.""",
+        description="Task external trigger prerequisites.",
         sort=SortArgs(default_value=None),
         sort_order=graphene.List(String),
         limit=Int(default_value=0),
         satisfied=Boolean(),
         resolver=resolve_mapping_to_list)
     xtriggers = graphene.List(
         XTrigger,
-        description="""Task xtrigger prerequisites.""",
+        description="Task xtrigger prerequisites.",
         sort=SortArgs(default_value=None),
         sort_order=graphene.List(String),
         limit=Int(default_value=0),
         satisfied=Boolean(),
         resolver=resolve_mapping_to_list)
-    extras = GenericScalar(resolver=resolve_json_dump)
-    # name & namespace for filtering/sorting
-    name = String()
-    namespace = graphene.List(String)
-    prerequisites = graphene.List(Prerequisite)
+    extras = GenericScalar(
+        # TODO: what is this? write description
+        resolver=resolve_json_dump,
+    )
+    prerequisites = graphene.List(
+        Prerequisite,
+        description='The prerequisites of this task.',
+    )
     jobs = graphene.List(
         Job,
-        description="""Jobs.""",
+        description="Jobs.",
         args=JOB_ARGS,
         strip_null=STRIP_NULL_DEFAULT,
         delta_store=DELTA_STORE_DEFAULT,
         delta_type=DELTA_TYPE_DEFAULT,
-        resolver=get_nodes_by_ids)
+        resolver=get_nodes_by_ids,
+    )
     parents = graphene.List(
         lambda: FamilyProxy,
-        description="""Task parents.""",
+        description="Task parents (i.e. families).",
         args=PROXY_ARGS,
         strip_null=STRIP_NULL_DEFAULT,
         delta_store=DELTA_STORE_DEFAULT,
         delta_type=DELTA_TYPE_DEFAULT,
-        resolver=get_nodes_by_ids)
+        resolver=get_nodes_by_ids,
+    )
     first_parent = Field(
         lambda: FamilyProxy,
-        description="""Task first parent.""",
+        description="The task's first parent (i.e. its containing family).",
         args=PROXY_ARGS,
         strip_null=STRIP_NULL_DEFAULT,
         delta_store=DELTA_STORE_DEFAULT,
         delta_type=DELTA_TYPE_DEFAULT,
-        resolver=get_node_by_id)
+        resolver=get_node_by_id,
+    )
     ancestors = graphene.List(
         lambda: FamilyProxy,
-        description="""First parent ancestors.""",
+        description="First parent ancestors (i.e. inheritance hierarchy).",
         args=PROXY_ARGS,
         strip_null=STRIP_NULL_DEFAULT,
         delta_store=DELTA_STORE_DEFAULT,
         delta_type=DELTA_TYPE_DEFAULT,
-        resolver=get_nodes_by_ids)
+        resolver=get_nodes_by_ids,
+    )
 
 
 class Family(ObjectType):
     class Meta:
         description = """Task definition, static fields"""
     id = ID()  # noqa: A003 (required for schema definition)
     name = String()
@@ -1593,15 +1766,15 @@
             - The scheduler, if communication is possible.
 
             Jobs use this to record and report status such
             as success and failure. Applications run by jobs can use
             this command to report messages and to report registered task
             outputs.
 
-            Valid for: paused, running workflows.
+            Valid for: paused, running, stopping workflows.
         ''')
         resolver = partial(mutator, command='put_messages')
 
     class Arguments:
         workflows = graphene.List(WorkflowID, required=True)
         task_job = String(required=True)
         event_time = String(default_value=None)
@@ -1724,15 +1897,15 @@
 
             Tasks that become ready after the shutdown is ordered will be
             submitted immediately if the workflow is restarted.
             Remaining task event handlers, job poll and kill commands, will
             be executed prior to shutdown, unless
             the stop mode is `{WorkflowStopMode.Now.name}`.
 
-            Valid for: paused, running workflows.
+            Valid for: paused, running, stopping workflows.
         ''')
         resolver = mutator
 
     class Arguments:
         workflows = graphene.List(WorkflowID, required=True)
         mode = WorkflowStopMode(
             default_value=WorkflowStopMode.Clean.name
@@ -1877,15 +2050,15 @@
 
 class Kill(Mutation, TaskMutation):
     # TODO: This should be a job mutation?
     class Meta:
         description = sstrip('''
             Kill running or submitted jobs.
 
-            Valid for: paused, running workflows.
+            Valid for: paused, running, stopping workflows.
         ''')
         resolver = partial(mutator, command='kill_tasks')
 
 
 class Poll(Mutation, TaskMutation):
     class Meta:
         description = sstrip('''
@@ -1894,15 +2067,15 @@
             This checks the job status file and queries the
             job runner on the job platform.
 
             Pollable tasks are those in the n=0 window with
             an associated job ID, including incomplete finished
             tasks.
 
-            Valid for: paused, running workflows.
+            Valid for: paused, running, stopping workflows.
         ''')
         resolver = partial(mutator, command='poll_tasks')
 
     class Arguments(TaskMutation.Arguments):
         ...
```

### Comparing `cylc-flow-8.1.4/cylc/flow/network/server.py` & `cylc-flow-8.2.0/cylc/flow/network/server.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/network/ssh_client.py` & `cylc-flow-8.2.0/cylc/flow/network/ssh_client.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/network/subscriber.py` & `cylc-flow-8.2.0/cylc/flow/network/subscriber.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/option_parsers.py` & `cylc-flow-8.2.0/cylc/flow/option_parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from contextlib import suppress
 import logging
 from itertools import product
 from optparse import (
     OptionParser,
     Values,
     Option,
-    IndentedHelpFormatter
+    IndentedHelpFormatter,
 )
 import os
 import re
 from ansimarkup import (
     parse as cparse,
     strip as cstrip
 )
@@ -359,14 +359,23 @@
 
                 <dim># Match the workflows foo-1, foo-2</dim>
                 'foo-[12]'
 
             See `cylc help id` for more details.
     '''))
 
+    CAN_BE_USED_MULTIPLE = (
+        " This option can be used multiple times on the command line.")
+
+    NOTE_PERSIST_ACROSS_RESTARTS = (
+        " NOTE: these settings persist across workflow restarts,"
+        " but can be set again on the \"cylc play\""
+        " command line if they need to be overridden."
+    )
+
     STD_OPTIONS = [
         OptionSettings(
             ['-q', '--quiet'], help='Decrease verbosity.',
             action='decrement', dest='verbosity', useif='all'),
         OptionSettings(
             ['-v', '--verbose'], help='Increase Verbosity',
             dest='verbosity', action='count',
@@ -399,32 +408,44 @@
             ['-s', '--set'], metavar='NAME=VALUE',
             help=(
                 "Set the value of a Jinja2 template variable in the"
                 " workflow definition."
                 " Values should be valid Python literals so strings"
                 " must be quoted"
                 " e.g. 'STR=\"string\"', INT=43, BOOL=True."
-                " This option can be used multiple "
-                " times on the command line."
-                " NOTE: these settings persist across workflow restarts,"
-                " but can be set again on the \"cylc play\""
-                " command line if they need to be overridden."
+                + CAN_BE_USED_MULTIPLE
+                + NOTE_PERSIST_ACROSS_RESTARTS
             ),
-            action='append', default=[], dest='templatevars', useif='jset'),
+            action='append', default=[], dest='templatevars', useif='jset'
+        ),
+        OptionSettings(
+            ['-z', '--set-list', '--template-list'],
+            metavar='NAME=VALUE1,VALUE2,...',
+            help=(
+                'Set the value of a Jinja2 template variable in the'
+                ' workflow definition as a comma separated'
+                ' list of Python strings.'
+                ' Values containing commas must be quoted.'
+                " e.g. '+s STR=a,b,c' => ['a', 'b', 'c']"
+                " or '+ s STR=a,\"b,c\"' => ['a', 'b,c']"
+                + CAN_BE_USED_MULTIPLE
+                + NOTE_PERSIST_ACROSS_RESTARTS
+            ),
+            action='append', default=[], dest='templatevars_lists',
+            useif='jset'
+        ),
         OptionSettings(
             ['--set-file'], metavar='FILE',
             help=(
                 "Set the value of Jinja2 template variables in the"
                 " workflow definition from a file containing NAME=VALUE"
                 " pairs (one per line)."
                 " As with --set values should be valid Python literals "
                 " so strings must be quoted e.g. STR='string'."
-                " NOTE: these settings persist across workflow restarts,"
-                " but can be set again on the \"cylc play\""
-                " command line if they need to be overridden."
+                + NOTE_PERSIST_ACROSS_RESTARTS
             ),
             action='store', default=None, dest='templatevars_file',
             useif='jset'
         )
     ]
 
     def __init__(
```

### Comparing `cylc-flow-8.1.4/cylc/flow/param_expand.py` & `cylc-flow-8.2.0/cylc/flow/param_expand.py`

 * *Files 15% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 foo_m1=>bar_m1_n1
 foo_m1=>bar_m1_n2
 #------------------------------------------------------------------------------
 """
 
 from contextlib import suppress
 import re
+from typing import List, Tuple
 
 from cylc.flow.exceptions import ParamExpandError
 from cylc.flow.task_id import TaskID
 from cylc.flow.parsec.OrderedDict import OrderedDictWithDefaults
 
 # To split runtime heading name lists.
 REC_NAMES = re.compile(r'(?:[^,<]|<[^>]*>)+')
@@ -197,32 +198,95 @@
                 raise ParamExpandError('parameter %s is not '
                                        'defined.' % str(exc.args[0]))
         else:
             for param_val in params[0][1]:
                 spec_vals[params[0][0]] = param_val
                 self._expand_name(results, tmpl, params[1:], spec_vals)
 
+    @staticmethod
+    def _parse_task_name_string(task_str: str) -> Tuple[List[str], str]:
+        """Takes a parent string and returns a list of parameters and a
+        template string.
+
+        Examples:
+            >>> this = NameExpander._parse_task_name_string
+
+            # Parent doesn't contain a parameter:
+            >>> this('foo')
+            ([], 'foo')
+
+            # Parent contains a simple single parameter:
+            >>> this('<foo>')
+            (['foo'], '{foo}')
+
+            # Parent contains 2 parameters in 1 <>:
+            >>> this('something<foo, bar>other')
+            (['foo', 'bar'], 'something{foo}{bar}other')
+
+            # Parent contains 2 parameters in 2 <>:
+            >>> this('something<foo>middlebit<bar>other')
+            (['foo', 'bar'], 'something{foo}middlebit{bar}other')
+
+            # Parent contains 2 parameters, once with an = sign in it.
+            >>> this('something<foo=42>middlebit<bar>other')
+            (['foo=42', 'bar'], 'something{foo}middlebit{bar}other')
+
+            # Parent contains 2 parameters in 2 <>:
+            >>> this('something<foo,bar=99>other')
+            (['foo', 'bar=99'], 'something{foo}{bar}other')
+
+            # Parent contains spaces around = sign:
+            >>> this('FAM<i = cat ,j=3>')
+            (['i = cat', 'j=3'], 'FAM{i}{j}')
+        """
+        param_list = []
+
+        for match in REC_P_GROUP.finditer(task_str):
+            param = match.group(1)
+            if ',' in param:
+                # parameter syntax `<foo, bar>`
+                replacement = ''
+                for sub_param in param.split(','):
+                    sub_param = sub_param.strip()
+                    param_list.append(sub_param)
+                    if '=' in sub_param:
+                        sub_param = sub_param.split('=')[0].strip()
+                    replacement += '{' + sub_param + '}'
+            else:
+                # parameter syntax: `<foo><bar>`
+                param_list.append(param)
+                if '=' in param:
+                    replacement = '{' + param.split('=')[0] + '}'
+                else:
+                    replacement = '{' + param + '}'
+
+            task_str = task_str.replace(match.group(0), replacement, 1)
+
+        return param_list, task_str
+
     def expand_parent_params(self, parent, param_values, origin):
         """Replace parameters with specific values in inherited parent names.
 
         If a value is NOT specified, e.g.:
             inherit = parent<m>
         then it must be given in param_values (as defined by expansion of the
         enclosing namespace name).
 
         If a value IS specified, e.g.:
             inherit = parent<m=3>
         then it must be a legal value for that parameter.
 
         """
-        head, p_list_str, tail = REC_P_ALL.match(parent).groups()
-        if not p_list_str:
-            return (None, head)
+        p_list, tmpl = self._parse_task_name_string(parent)
+
+        if not p_list:
+            return (None, parent)
+
         used = {}
-        for item in (i.strip() for i in p_list_str.split(',')):
+        for item in p_list:
             if '-' in item or '+' in item:
                 raise ParamExpandError(
                     "parameter offsets illegal here: '%s'" % origin)
             elif '=' in item:
                 # Specific value given.
                 pname, pval = [val.strip() for val in item.split('=', 1)]
                 with suppress(ValueError):
@@ -240,22 +304,18 @@
                 # Non-specific; value must be supplied in param_values.
                 try:
                     used[item] = param_values[item]
                 except KeyError:
                     raise ParamExpandError(
                         "parameter '%s' undefined in '%s'" % (
                             item, origin))
-        if head:
-            tmpl = head
-        else:
-            tmpl = ''
-        for pname in used:
-            tmpl += self.param_tmpl_cfg[pname]
-        if tail:
-            tmpl += tail
+
+        # For each parameter substitute the param_tmpl_cfg.
+        tmpl = tmpl.format(**self.param_tmpl_cfg)
+        # Insert parameter values into template.
         return (used, tmpl % used)
 
 
 class GraphExpander:
     """Handle parameter expansion of graph string lines."""
 
     _REMOVE = -32768
```

### Comparing `cylc-flow-8.1.4/cylc/flow/parsec/OrderedDict.py` & `cylc-flow-8.2.0/cylc/flow/parsec/OrderedDict.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/parsec/__init__.py` & `cylc-flow-8.2.0/cylc/flow/parsec/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/parsec/config.py` & `cylc-flow-8.2.0/cylc/flow/parsec/config.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/parsec/empysupport.py` & `cylc-flow-8.2.0/cylc/flow/parsec/empysupport.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/parsec/exceptions.py` & `cylc-flow-8.2.0/cylc/flow/parsec/exceptions.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/parsec/fileparse.py` & `cylc-flow-8.2.0/cylc/flow/parsec/fileparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -397,14 +397,20 @@
     used to generate continuation lines.
     """
     template_vars = template_vars if template_vars is not None else {}
     template_vars = _prepend_old_templatevars(fpath, template_vars)
     fpath = _get_fpath_for_source(fpath, opts)
     fdir = os.path.dirname(fpath)
 
+    odir = os.getcwd()
+
+    # Move to the file location to give the template processor easy access to
+    # other files in the workflow directory (whether source or installed).
+    os.chdir(fdir)
+
     # Allow Python modules in lib/python/ (e.g. for use by Jinja2 filters).
     workflow_lib_python = os.path.join(fdir, "lib", "python")
     if (
         os.path.isdir(workflow_lib_python)
         and workflow_lib_python not in sys.path
     ):
         sys.path.append(workflow_lib_python)
@@ -490,14 +496,16 @@
                 fpath, flines, fdir, template_vars
             )
 
     # concatenate continuation lines
     if do_contin:
         flines = _concatenate(flines)
 
+    os.chdir(odir)
+
     # return rstripped lines
     return [fl.rstrip() for fl in flines]
 
 
 def hashbang_and_plugin_templating_clash(
     templating: str, flines: t.List[str]
 ) -> t.Optional[str]:
```

### Comparing `cylc-flow-8.1.4/cylc/flow/parsec/include.py` & `cylc-flow-8.2.0/cylc/flow/parsec/include.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/parsec/jinja2support.py` & `cylc-flow-8.2.0/cylc/flow/parsec/jinja2support.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/parsec/upgrade.py` & `cylc-flow-8.2.0/cylc/flow/parsec/upgrade.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/parsec/util.py` & `cylc-flow-8.2.0/cylc/flow/parsec/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/parsec/validate.py` & `cylc-flow-8.2.0/cylc/flow/parsec/validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 Also provides default values from the spec as a nested dict.
 """
 
 import re
 import shlex
 from collections import deque
 from textwrap import dedent
+from typing import List, Dict, Any, Tuple
 
 from metomi.isodatetime.data import Duration, TimePoint
 from metomi.isodatetime.dumpers import TimePointDumper
 from metomi.isodatetime.parsers import TimePointParser, DurationParser
 from metomi.isodatetime.exceptions import IsodatetimeError, ISO8601SyntaxError
 
 from cylc.flow.parsec.exceptions import (
@@ -990,49 +991,121 @@
                 raise IllegalValueError(
                     'parameter', keys, value, '%s: bad value' % item)
         try:
             return [int(item) for item in items]
         except ValueError:
             return items
 
+    @staticmethod
+    def parse_xtrig_arglist(value: str) -> Tuple[List[Any], Dict[str, Any]]:
+        """Parse Pythonic-like arg/kwarg signatures.
+
+        A stateful parser treats all args/kwargs as strings with
+        implicit quoting.
+
+        Examples:
+            >>> parse = CylcConfigValidator.parse_xtrig_arglist
+
+            # Parse pythonic syntax
+            >>> parse('a, b, c, d=1, e=2,')
+            (['a', 'b', 'c'], {'d': '1', 'e': '2'})
+            >>> parse('a, "1,2,3", b=",=",')
+            (['a', '"1,2,3"'], {'b': '",="'})
+            >>> parse('a, "b c", '"'d=e '")
+            (['a', '"b c"', "'d=e '"], {})
+
+            # Parse implicit (i.e. unquoted) strings
+            >>> parse('%(cycle)s, %(task)s, output=succeeded')
+            (['%(cycle)s', '%(task)s'], {'output': 'succeeded'})
+
+        """
+        # results
+        args = []
+        kwargs = {}
+        # state
+        in_str = False  # are we inside a quoted string
+        in_kwarg = False  # are we after the = sign of a kwarg
+        buffer = ''  # the current argument being parsed
+        kwarg_buffer = ''  # the key of a kwarg if in_kwarg == True
+        # parser
+        for char in value:
+            if char in {'"', "'"}:
+                in_str = not in_str
+                buffer += char
+            elif not in_str and char == ',':
+                if in_kwarg:
+                    kwargs[kwarg_buffer.strip()] = buffer.strip()
+                    in_kwarg = False
+                    kwarg_buffer = ''
+                else:
+                    args.append(buffer.strip())
+                buffer = ''
+            elif char == '=' and not in_str and not in_kwarg:
+                in_kwarg = True
+                kwarg_buffer = buffer
+                buffer = ''
+            else:
+                buffer += char
+
+        # reached the end of the string
+        if buffer:
+            if in_kwarg:
+                kwargs[kwarg_buffer.strip()] = buffer.strip()
+            else:
+                args.append(buffer.strip())
+
+        return args, kwargs
+
     @classmethod
     def coerce_xtrigger(cls, value, keys):
         """Coerce a string into an xtrigger function context object.
 
         func_name(*func_args, **func_kwargs)
         Checks for legal string templates in arg values too.
 
         Examples:
-            >>> CylcConfigValidator.coerce_xtrigger('a(b, c):PT1M', [None])
-            a(b, c):60.0
+            >>> xtrig = CylcConfigValidator.coerce_xtrigger
 
-        """
+            >>> ctx = xtrig('a(b, c):PT1M', [None])
+            >>> ctx.get_signature()
+            'a(b, c)'
+            >>> ctx.intvl
+            60.0
+
+            # cast types
+            >>> x = xtrig('a(1, 1.1, True, abc, x=True, y=1.1)', [None])
+            >>> x.func_args
+            [1, 1.1, True, 'abc']
+            >>> x.func_kwargs
+            {'x': True, 'y': 1.1}
 
+        """
         label = keys[-1]
         value = cls.strip_and_unquote(keys, value)
         if not value:
             raise IllegalValueError("xtrigger", keys, value)
-        args = []
-        kwargs = {}
         match = cls._REC_TRIG_FUNC.match(value)
         if match is None:
             raise IllegalValueError("xtrigger", keys, value)
         fname, fargs, intvl = match.groups()
         if intvl:
             intvl = cls.coerce_interval(intvl, keys)
 
-        if fargs:
-            # Extract function args and kwargs.
-            for farg in fargs.split(r','):
-                try:
-                    key, val = farg.strip().split(r'=', 1)
-                except ValueError:
-                    args.append(cls._coerce_type(farg.strip()))
-                else:
-                    kwargs[key.strip()] = cls._coerce_type(val.strip())
+        # parse args
+        args, kwargs = CylcConfigValidator.parse_xtrig_arglist(fargs or '')
+
+        # cast types
+        args = [
+            CylcConfigValidator._coerce_type(arg)
+            for arg in args
+        ]
+        kwargs = {
+            key: CylcConfigValidator._coerce_type(value)
+            for key, value in kwargs.items()
+        }
 
         return SubFuncContext(label, fname, args, kwargs, intvl)
 
     @classmethod
     def _coerce_type(cls, value):
         """Convert value to int, float, or bool, if possible.
```

### Comparing `cylc-flow-8.1.4/cylc/flow/pathutil.py` & `cylc-flow-8.2.0/cylc/flow/pathutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,43 +52,43 @@
     extra args."""
     return os.path.normpath(os.path.expanduser(os.path.expandvars(
         os.path.join(*args)
     )))
 
 
 def get_remote_workflow_run_dir(
-    workflow_name: Union[Path, str], *args: Union[Path, str]
+    workflow_id: Union[Path, str], *args: Union[Path, str]
 ) -> str:
     """Return remote workflow run directory, joining any extra args,
     NOT expanding vars or user."""
-    return os.path.join(_CYLC_RUN_DIR, workflow_name, *args)
+    return os.path.join(_CYLC_RUN_DIR, workflow_id, *args)
 
 
 def get_remote_workflow_run_job_dir(
-    workflow_name: Union[Path, str], *args: Union[Path, str]
+    workflow_id: Union[Path, str], *args: Union[Path, str]
 ) -> str:
     """Return remote workflow job log directory, joining any extra args,
     NOT expanding vars or user."""
-    return get_remote_workflow_run_dir(workflow_name, 'log', 'job', *args)
+    return get_remote_workflow_run_dir(workflow_id, 'log', 'job', *args)
 
 
 def get_cylc_run_dir() -> str:
     """Return the cylc-run dir path with vars/user expanded."""
     return expand_path(_CYLC_RUN_DIR)
 
 
 def get_workflow_run_dir(
-    workflow_name: Union[Path, str], *args: Union[Path, str]
+    workflow_id: Union[Path, str], *args: Union[Path, str]
 ) -> str:
     """Return local workflow run directory, joining any extra args, and
     expanding vars and user.
 
     Does not check that the directory exists.
     """
-    return expand_path(_CYLC_RUN_DIR, workflow_name, *args)
+    return expand_path(_CYLC_RUN_DIR, workflow_id, *args)
 
 
 def get_workflow_run_job_dir(workflow, *args):
     """Return workflow run job (log) directory, join any extra args."""
     return get_workflow_run_dir(workflow, 'log', 'job', *args)
 
 
@@ -191,24 +191,24 @@
         if symlink_success:
             symlinks_created[target] = symlink_path
     return symlinks_created
 
 
 def get_dirs_to_symlink(
     install_target: str,
-    workflow_name: str,
+    workflow_id: str,
     symlink_conf: Optional[Dict[str, Dict[str, Any]]] = None
 ) -> Dict[str, str]:
     """Returns dictionary of directories to symlink.
 
     Note the paths should remain unexpanded, to be expanded on the remote.
 
     Args:
         install_target: Symlinks to be created on this install target
-        flow_name: full name of the run, e.g. myflow/run1
+        workflow_id: full id of the run, e.g. myflow/run1
         symlink_conf: Symlink dirs, if sent on the cli.
             Defaults to None, in which case global config symlink dirs will
             be applied.
 
     Returns:
         dirs_to_symlink: [directory: symlink_path]
     """
@@ -216,21 +216,21 @@
     if symlink_conf is None:
         symlink_conf = glbl_cfg().get(['install', 'symlink dirs'])
     if install_target not in symlink_conf.keys():
         return dirs_to_symlink
     base_dir = symlink_conf[install_target]['run']
     if base_dir:
         dirs_to_symlink['run'] = os.path.join(
-            base_dir, 'cylc-run', workflow_name)
+            base_dir, 'cylc-run', workflow_id)
     for dir_ in ['log', 'share', 'share/cycle', 'work']:
         link = symlink_conf[install_target].get(dir_, None)
         if (not link) or link == base_dir:
             continue
         dirs_to_symlink[dir_] = os.path.join(
-            link, 'cylc-run', workflow_name, dir_)
+            link, 'cylc-run', workflow_id, dir_)
     return dirs_to_symlink
 
 
 def make_symlink_dir(path: Union[Path, str], target: Union[Path, str]) -> bool:
     """Makes symlinks for directories.
 
     Args:
```

### Comparing `cylc-flow-8.1.4/cylc/flow/platforms.py` & `cylc-flow-8.2.0/cylc/flow/platforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,15 @@
             # Need to calculate platform
             # NOTE: Do NOT use .get() on OrderedDictWithDefaults - see above
             task_job_section = task_conf['job'] if 'job' in task_conf else {}
             task_remote_section = (
                 task_conf['remote'] if 'remote' in task_conf else {})
             return platform_from_name(
                 platform_name_from_job_info(
-                    glbl_cfg(cached=False).get(['platforms']),
+                    glbl_cfg().get(['platforms']),
                     task_job_section,
                     task_remote_section
                 ),
                 bad_hosts=bad_hosts
             )
 
 
@@ -215,15 +215,15 @@
         if re.fullmatch(platform_name_re, platform_name):
             platform_name = get_platform_from_group(
                 platform_groups[platform_name_re], group_name=platform_name,
                 bad_hosts=bad_hosts
             )
             break
 
-    for platform_name_re in list(platforms):
+    for platform_name_re in platforms:
         if (
             # If the platform_name_re contains special regex chars
             re.escape(platform_name_re) != platform_name_re
             and re.match(platform_name_re, 'localhost')
         ):
             raise PlatformLookupError(
                 'The "localhost" platform cannot be defined using a '
@@ -233,35 +233,35 @@
 
     # The list is reversed to allow user-set platforms (which are appended to
     # than site set platforms) to be matched first and override site defined
     # platforms.
     for platform_name_re in reversed(list(platforms)):
         # We substitute commas with or without spaces to
         # allow lists of platforms
-        if (
-            re.fullmatch(
-                re.sub(
-                    r'\s*(?!{[\s\d]*),(?![\s\d]*})\s*',
-                    '|',
-                    platform_name_re
-                ),
-                platform_name
-            )
+        if re.fullmatch(
+            re.sub(
+                r'\s*(?!{[\s\d]*),(?![\s\d]*})\s*',
+                '|',
+                platform_name_re
+            ),
+            platform_name
         ):
             # Deepcopy prevents contaminating platforms with data
             # from other platforms matching platform_name_re
             platform_data = deepcopy(platforms[platform_name_re])
 
             # If hosts are not filled in make remote
             # hosts the platform name.
             # Example: `[platforms][workplace_vm_123]<nothing>`
             #   should create a platform where
-            #   `remote_hosts = ['workplace_vm_123']`
+            #   `hosts = ['workplace_vm_123']`
+            # NOTE: Probably don't use .get() due to OrderedDictWithDefaults -
+            # see https://github.com/cylc/cylc-flow/pull/4975
             if (
-                'hosts' not in platform_data.keys() or
+                'hosts' not in platform_data or
                 not platform_data['hosts']
             ):
                 platform_data['hosts'] = [platform_name]
             # Fill in the "private" name field.
             platform_data['name'] = platform_name
             return platform_data
 
@@ -288,23 +288,21 @@
     Raises:
         NoPlatformsError: If there are no platforms with any usable
         hosts in the platform group.
 
     TODO: Uses host_selection methods; should also allow custom select methods.
     """
     if bad_hosts:
-        good_platforms = []
-        for platform in group['platforms']:
+        platform_names = [
+            platform for platform in group['platforms']
             if any(
                 host not in bad_hosts
                 for host in platform_from_name(platform)['hosts']
-            ):
-                good_platforms.append(platform)
-
-        platform_names = list(good_platforms)
+            )
+        ]
     else:
         platform_names = group['platforms']
 
     # Return False if there are no platforms available to be selected.
     if not platform_names:
         raise NoPlatformsError(group_name)
 
@@ -635,41 +633,29 @@
     quiet: bool = False
 ) -> Dict[str, List[Dict[str, Any]]]:
     """Get a dictionary of unique install targets and the platforms which use
     them.
 
     Args:
         platform_names: List of platform names to look up in the global config.
-        quiet: Supress PlatformNotFound Errors
+        quiet: Supress PlatformLookupErrors
 
     Return {install_target_1: [platform_1_dict, platform_2_dict, ...], ...}
     """
-    platform_names = set(platform_names)
-    platforms: List[Dict[str, Any]] = []
-    for p_name in platform_names:
+    ret: Dict[str, List[Dict[str, Any]]] = {}
+    for p_name in set(platform_names):
         try:
             platform = platform_from_name(p_name)
         except PlatformLookupError as exc:
             if not quiet:
                 raise exc
         else:
-            platforms.append(platform)
-
-    install_targets = {
-        get_install_target_from_platform(platform)
-        for platform in platforms
-    }
-    return {
-        target: [
-            platform
-            for platform in platforms
-            if get_install_target_from_platform(platform) == target
-        ]
-        for target in install_targets
-    }
+            install_target = get_install_target_from_platform(platform)
+            ret.setdefault(install_target, []).append(platform)
+    return ret
 
 
 def is_platform_with_target_in_list(
         install_target: str,
         distinct_platforms_list: Iterable[Dict[str, Any]]
 ) -> bool:
     """Determines whether install target is in the list of platforms"""
```

### Comparing `cylc-flow-8.1.4/cylc/flow/prerequisite.py` & `cylc-flow-8.2.0/cylc/flow/prerequisite.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from cylc.flow.cycling.loader import get_point
 from cylc.flow.exceptions import TriggerExpressionError
 from cylc.flow.data_messages_pb2 import (  # type: ignore
     PbPrerequisite,
     PbCondition,
 )
-from cylc.flow.id import Tokens
+from cylc.flow.id import quick_relative_detokenise
 
 
 class Prerequisite:
     """The concrete result of an abstract logical trigger expression.
 
     A single TaskProxy can have multiple Prerequisites, all of which require
     satisfying. This corresponds to multiple tasks being dependencies of a task
@@ -37,34 +37,34 @@
     also have multiple 'messages' (basically, subcomponents of a Prerequisite)
     corresponding to parenthesised expressions in Cylc graphs (e.g.
     `(a & b) => c` or `(a | b) => c`). For the OR operator (`|`), only one
     message has to be satisfied for the Prerequisite to be satisfied.
     """
 
     # Memory optimization - constrain possible attributes to this list.
-    __slots__ = ["satisfied", "_all_satisfied",
-                 "target_point_strings",
-                 "conditional_expression", "point"]
+    __slots__ = (
+        "satisfied",
+        "_all_satisfied",
+        "conditional_expression",
+        "point",
+    )
 
     # Extracts T from "foo.T succeeded" etc.
     SATISFIED_TEMPLATE = 'bool(self.satisfied[("%s", "%s", "%s")])'
     MESSAGE_TEMPLATE = r'%s/%s %s'
 
     DEP_STATE_SATISFIED = 'satisfied naturally'
     DEP_STATE_OVERRIDDEN = 'force satisfied'
     DEP_STATE_UNSATISFIED = False
 
     def __init__(self, point):
         # The cycle point to which this prerequisite belongs.
         # cylc.flow.cycling.PointBase
         self.point = point
 
-        # List of cycle point strings that this prerequisite depends on.
-        self.target_point_strings = []
-
         # Dictionary of messages pertaining to this prerequisite.
         # {('point string', 'task name', 'output'): DEP_STATE_X, ...}
         self.satisfied = {}
 
         # Expression present only when conditions are used.
         # '1/foo failed & 1/bar succeeded'
         self.conditional_expression = None
@@ -102,16 +102,14 @@
         # Add a new prerequisite as satisfied if pre-initial, else unsatisfied.
         if pre_initial:
             self.satisfied[message] = self.DEP_STATE_SATISFIED
         else:
             self.satisfied[message] = self.DEP_STATE_UNSATISFIED
         if self._all_satisfied is not None:
             self._all_satisfied = False
-        if point and str(point) not in self.target_point_strings:
-            self.target_point_strings.append(str(point))
 
     def get_raw_conditional_expression(self):
         """Return a representation of this prereq as a string.
 
         Returns None if this prerequisite is not a conditional one.
 
         """
@@ -212,47 +210,49 @@
         return relevant_messages
 
     def api_dump(self):
         """Return list of populated Protobuf data objects."""
         if not self.satisfied:
             return None
         if self.conditional_expression:
-            temp = self.get_raw_conditional_expression()
-            temp = temp.replace('|', ' | ')
-            temp = temp.replace('&', ' & ')
+            expr = (
+                self.get_raw_conditional_expression()
+            ).replace('|', ' | ').replace('&', ' & ')
         else:
-            for s_msg in self.satisfied:
-                temp = self.MESSAGE_TEMPLATE % s_msg
+            expr = ' & '.join(
+                self.MESSAGE_TEMPLATE % s_msg
+                for s_msg in self.satisfied
+            )
         conds = []
         num_length = math.ceil(len(self.satisfied) / 10)
         for ind, message_tuple in enumerate(sorted(self.satisfied)):
             point, name = message_tuple[0:2]
-            t_id = Tokens(cycle=str(point), task=name).relative_id
+            t_id = quick_relative_detokenise(point, name)
             char = 'c%.{0}d'.format(num_length) % ind
             c_msg = self.MESSAGE_TEMPLATE % message_tuple
             c_val = self.satisfied[message_tuple]
             c_bool = bool(c_val)
             if c_bool is False:
                 c_val = "unsatisfied"
-            cond = PbCondition(
-                task_proxy=t_id,
-                expr_alias=char,
-                req_state=message_tuple[2],
-                satisfied=c_bool,
-                message=c_val,
+            conds.append(
+                PbCondition(
+                    task_proxy=t_id,
+                    expr_alias=char,
+                    req_state=message_tuple[2],
+                    satisfied=c_bool,
+                    message=c_val,
+                )
             )
-            conds.append(cond)
-            temp = temp.replace(c_msg, char)
-        prereq_buf = PbPrerequisite(
-            expression=temp,
+            expr = expr.replace(c_msg, char)
+        return PbPrerequisite(
+            expression=expr,
             satisfied=self.is_satisfied(),
+            conditions=conds,
+            cycle_points=sorted(self.iter_target_point_strings()),
         )
-        prereq_buf.conditions.extend(conds)
-        prereq_buf.cycle_points.extend(self.target_point_strings)
-        return prereq_buf
 
     def set_satisfied(self):
         """Force this prerequisite into the satisfied state.
 
         State can be overridden by calling `self.satisfy_me`.
 
         """
@@ -260,33 +260,26 @@
             if not self.satisfied[message]:
                 self.satisfied[message] = self.DEP_STATE_OVERRIDDEN
         if self.conditional_expression is None:
             self._all_satisfied = True
         else:
             self._all_satisfied = self._conditional_is_satisfied()
 
-    def set_not_satisfied(self):
-        """Force this prerequisite into the un-satisfied state.
-
-        State can be overridden by calling `self.satisfy_me`.
-
-        """
-        for message in self.satisfied:
-            self.satisfied[message] = self.DEP_STATE_UNSATISFIED
-        if not self.satisfied:
-            self._all_satisfied = True
-        elif self.conditional_expression is None:
-            self._all_satisfied = False
-        else:
-            self._all_satisfied = self._conditional_is_satisfied()
+    def iter_target_point_strings(self):
+        yield from {
+            message[0]
+            for message in self.satisfied
+        }
 
     def get_target_points(self):
         """Return a list of cycle points target by each prerequisite,
         including each component of conditionals."""
-        return [get_point(p) for p in self.target_point_strings]
+        return [
+            get_point(p) for p in self.iter_target_point_strings()
+        ]
 
     def get_resolved_dependencies(self):
         """Return a list of satisfied dependencies.
 
         E.G: ['1/foo', '2/bar']
 
         """
```

### Comparing `cylc-flow-8.1.4/cylc/flow/print_tree.py` & `cylc-flow-8.2.0/cylc/flow/print_tree.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/profiler.py` & `cylc-flow-8.2.0/cylc/flow/profiler.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/remote.py` & `cylc-flow-8.2.0/cylc/flow/remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     stdin=None,
     stdin_str=None,
     capture_process=False,
     capture_status=False,
     manage=False,
     text=True,
 ):
-    """Run a given cylc command on another account and/or host.
+    """Run a given cylc command on another host.
 
     Arguments:
         command (list):
             command inclusive of all opts and args required to run via ssh.
         stdin (file):
             If specified, it should be a readable file object.
             If None, DEVNULL is set if output is to be captured.
@@ -103,14 +103,17 @@
 
     Return:
         * If capture_process=True, the Popen[str] object if created
           successfully.
         * Else True if the remote command is executed successfully, or
           if unsuccessful and capture_status=True the remote command exit code.
         * Otherwise exit with an error message.
+
+    Exits with code 1 in the event of certain command errors.
+
     """
     # CODACY ISSUE:
     #   subprocess call - check for execution of untrusted input.
     # REASON IGNORED:
     #   The command is read from the site/user global config file, but we check
     #   above that it ends in 'cylc', and in any case the user could execute
     #   any such command directly via ssh.
@@ -381,14 +384,16 @@
     Uses the provided platform configuration to construct the command.
 
     For arguments and returns see construct_ssh_cmd and run_cmd.
 
     Raises:
         NoHostsError: If the platform is not contactable.
 
+    Exits with code 1 in the event of certain command errors.
+
     """
     if not host:
         # no host selected => perform host selection from platform config
         host = get_host_from_platform(platform, bad_hosts=bad_hosts)
 
     return run_cmd(
         construct_ssh_cmd(
@@ -422,14 +427,16 @@
     with the localhost platform.
 
     For arguments and returns see construct_ssh_cmd and run_cmd.
 
     Raises:
         NoHostsError: If the platform is not contactable.
 
+    Exits with code 1 in the event of certain command errors.
+
     """
     return remote_cylc_cmd(
         cmd,
         get_platform(),  # use localhost settings
         host=host,
         **kwargs,
     )
```

### Comparing `cylc-flow-8.1.4/cylc/flow/resources.py` & `cylc-flow-8.2.0/cylc/flow/resources.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/rundb.py` & `cylc-flow-8.2.0/cylc/flow/rundb.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from contextlib import suppress
 from dataclasses import dataclass
 from os.path import expandvars
 from pprint import pformat
 import sqlite3
 import traceback
-from typing import TYPE_CHECKING, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Iterable, List, Optional, Tuple, Union
 
 from cylc.flow import LOG
 from cylc.flow.exceptions import PlatformLookupError
 from cylc.flow.util import deserialise
 import cylc.flow.flags
 
 if TYPE_CHECKING:
@@ -541,30 +541,26 @@
         Invoke callback(row_idx, row) on each row, where each row contains:
             [point, namespace, key, value]
         """
         stmt = self.pre_select_broadcast_states(order=sort)
         for row_idx, row in enumerate(self.connect().execute(stmt)):
             callback(row_idx, list(row))
 
-    def select_workflow_params(self, callback):
-        """Select from workflow_params.
+    def select_workflow_params(self) -> Iterable[Tuple[str, Optional[str]]]:
+        """Select all from workflow_params.
 
-        Invoke callback(row_idx, row) on each row, where each row contains:
-            [key, value]
-
-        E.g. a row might be ['UTC mode', '1']
+        E.g. a row might be ('UTC mode', '1')
         """
         stmt = rf'''
             SELECT
                 key, value
             FROM
                 {self.TABLE_WORKFLOW_PARAMS}
         '''  # nosec (table name is code constant)
-        for row_idx, row in enumerate(self.connect().execute(stmt)):
-            callback(row_idx, list(row))
+        return self.connect().execute(stmt)
 
     def select_workflow_flows(self, flow_nums):
         """Return flow data for selected flows."""
         stmt = rf'''
             SELECT
                 flow_num, start_time, description
             FROM
@@ -779,14 +775,22 @@
         ) % {"name": self.TABLE_TASK_STATES}
         ret = {}
         for flow_nums_str, submit_num, flow_wait in self.connect().execute(
                 stmt, (name, point,)):
             ret[submit_num] = (flow_wait == 1, deserialise(flow_nums_str))
         return ret
 
+    def select_latest_flow_nums(self):
+        """Return a list of the most recent previous flow numbers."""
+        stmt = rf'''
+            SELECT flow_nums, MAX(time_created) FROM {self.TABLE_TASK_STATES}
+        '''  # nosec (table name is code constant)
+        flow_nums_str = list(self.connect().execute(stmt))[0][0]
+        return deserialise(flow_nums_str)
+
     def select_task_outputs(self, name, point):
         """Select task outputs for each flow.
 
         Return: {outputs_list: flow_nums_set}
 
         """
         stmt = rf'''
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scheduler.py` & `cylc-flow-8.2.0/cylc/flow/scheduler.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,35 +14,36 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Cylc scheduler server."""
 
 import asyncio
 from contextlib import suppress
 from collections import deque
-from dataclasses import dataclass
 from optparse import Values
 import os
+import inspect
 from pathlib import Path
 from queue import Empty, Queue
 from shlex import quote
 from socket import gaierror
 from subprocess import Popen, PIPE, DEVNULL
 import sys
 from threading import Barrier, Thread
 from time import sleep, time
 import traceback
 from typing import (
     TYPE_CHECKING,
+    Any,
     Callable,
+    Dict,
     Iterable,
+    List,
     NoReturn,
     Optional,
-    List,
     Set,
-    Dict,
     Tuple,
     Union,
 )
 from uuid import uuid4
 
 import psutil
 
@@ -137,45 +138,48 @@
     TASK_STATUSES_ACTIVE,
     TASK_STATUSES_NEVER_ACTIVE,
     TASK_STATUS_PREPARING,
     TASK_STATUS_SUBMITTED,
     TASK_STATUS_RUNNING,
     TASK_STATUS_WAITING,
     TASK_STATUS_FAILED)
-from cylc.flow.templatevars import load_template_vars
+from cylc.flow.templatevars import get_template_vars
 from cylc.flow.util import cli_format
 from cylc.flow.wallclock import (
     get_current_time_string,
     get_time_string_from_unix_time as time2str,
     get_utc_mode)
 from cylc.flow.xtrigger_mgr import XtriggerManager
 
 if TYPE_CHECKING:
-    from cylc.flow.task_proxy import TaskProxy
+    # BACK COMPAT: typing_extensions.Literal
+    # FROM: Python 3.7
+    # TO: Python 3.8
+    from typing_extensions import Literal
 
 
 class SchedulerStop(CylcError):
     """Scheduler normal stop."""
 
 
 class SchedulerError(CylcError):
     """Scheduler expected error stop."""
 
 
-@dataclass
 class Scheduler:
     """Cylc scheduler server."""
 
     EVENT_STARTUP = WorkflowEventHandler.EVENT_STARTUP
     EVENT_SHUTDOWN = WorkflowEventHandler.EVENT_SHUTDOWN
     EVENT_ABORTED = WorkflowEventHandler.EVENT_ABORTED
     EVENT_WORKFLOW_TIMEOUT = WorkflowEventHandler.EVENT_WORKFLOW_TIMEOUT
+    EVENT_STALL = WorkflowEventHandler.EVENT_STALL
     EVENT_STALL_TIMEOUT = WorkflowEventHandler.EVENT_STALL_TIMEOUT
+    EVENT_RESTART_TIMEOUT = WorkflowEventHandler.EVENT_RESTART_TIMEOUT
     EVENT_INACTIVITY_TIMEOUT = WorkflowEventHandler.EVENT_INACTIVITY_TIMEOUT
-    EVENT_STALL = WorkflowEventHandler.EVENT_STALL
 
     # Intervals in seconds
     INTERVAL_MAIN_LOOP = 1.0
     INTERVAL_MAIN_LOOP_QUICK = 0.5
     INTERVAL_STOP_KILL = 10.0
     INTERVAL_STOP_PROCESS_POOL_EMPTY = 0.5
     INTERVAL_AUTO_RESTART_ERROR = 5
@@ -192,14 +196,15 @@
     # flow information
     workflow: str
     owner: str
     host: str
     id: str  # noqa: A003 (instance attr not local)
     uuid_str: str
     is_restart: bool
+    bad_hosts: Set[str]
 
     # directories
     workflow_log_dir: str
     workflow_run_dir: str
     workflow_share_dir: str
     workflow_work_dir: str
 
@@ -221,40 +226,39 @@
     message_queue: 'Queue[TaskMsg]'
     ext_trigger_queue: Queue
 
     # configuration
     config: WorkflowConfig  # flow config
     options: Values
     cylc_config: DictTree  # [scheduler] config
+    template_vars: Dict[str, Any]
 
     # tcp / zmq
     server: WorkflowRuntimeServer
 
     # Note: attributes without a default must come before those with defaults
 
     # flow information
     contact_data: Optional[dict] = None
-    bad_hosts: Optional[Set[str]] = None
 
     # configuration
     flow_file: Optional[str] = None
     flow_file_update_time: Optional[float] = None
 
-    # run options
-    template_vars: Optional[dict] = None
-
     # workflow params
     stop_mode: Optional[StopMode] = None
     stop_task: Optional[str] = None
     stop_clock_time: Optional[int] = None
+    reload_pending: 'Union[Literal[False], str]' = False
 
     # task event loop
     is_paused = False
     is_updated = False
     is_stalled = False
+    is_restart_timeout_wait = False
     is_reloaded = False
 
     # main loop
     main_loop_intervals: deque = deque(maxlen=10)
     main_loop_plugins: Optional[dict] = None
     auto_restart_mode: Optional[AutoRestartMode] = None
     auto_restart_time: Optional[float] = None
@@ -263,37 +267,35 @@
     _profile_amounts: Optional[dict] = None
     _profile_update_times: Optional[dict] = None
     previous_profile_point: float = 0
     count: int = 0
 
     time_next_kill: Optional[float] = None
 
-    def __init__(self, reg: str, options: Values) -> None:
+    def __init__(self, id_: str, options: Values) -> None:
         # flow information
-        self.workflow = reg
+        self.workflow = id_
         self.workflow_name = get_workflow_name_from_id(self.workflow)
         self.owner = get_user()
         self.host = get_host()
-        self.id = Tokens(
+        self.tokens = Tokens(
             user=self.owner,
             workflow=self.workflow,
-        ).id
+        )
+        self.id = self.tokens.id
         self.uuid_str = str(uuid4())
         self.options = options
-        self.template_vars = load_template_vars(
-            self.options.templatevars,
-            self.options.templatevars_file
-        )
+        self.template_vars = get_template_vars(self.options)
 
         # mutable defaults
         self._profile_amounts = {}
         self._profile_update_times = {}
         self.bad_hosts: Set[str] = set()
 
-        self.restored_stop_task_id = None
+        self.restored_stop_task_id: Optional[str] = None
 
         self.timers: Dict[str, Timer] = {}
 
         self.workflow_run_dir = get_workflow_run_dir(self.workflow)
         self.workflow_work_dir = get_workflow_run_work_dir(self.workflow)
         self.workflow_share_dir = get_workflow_run_share_dir(self.workflow)
         self.workflow_log_dir = get_workflow_run_scheduler_log_dir(
@@ -424,15 +426,16 @@
         self._check_startup_opts()
 
         if self.is_restart:
             self.load_workflow_params_and_tmpl_vars()
 
         self.profiler.log_memory("scheduler.py: before load_flow_file")
         try:
-            self.load_flow_file()
+            cfg = self.load_flow_file()
+            self.apply_new_config(cfg, is_reload=False)
         except ParsecError as exc:
             # Mark this exc as expected (see docstring for .schd_expected):
             exc.schd_expected = True
             raise exc
         self.profiler.log_memory("scheduler.py: after load_flow_file")
 
         self.workflow_db_mgr.on_workflow_start(self.is_restart)
@@ -458,14 +461,15 @@
             LOG.addHandler(ReferenceLogFileHandler(
                 self.config.get_ref_log_name()))
         elif self.options.reftest:
             LOG.addHandler(ReferenceLogFileHandler(
                 get_workflow_test_log_path(self.workflow)))
 
         self.pool = TaskPool(
+            self.tokens,
             self.config,
             self.workflow_db_mgr,
             self.task_events_mgr,
             self.data_store_mgr,
             self.flow_mgr
         )
 
@@ -493,23 +497,35 @@
             if not self.config.cfg['scheduler']['events'][event]:
                 self.config.cfg['scheduler']['events'][event] = DurationFloat(
                     180
                 )
         for event, start_now, log_reset_func in [
             (self.EVENT_INACTIVITY_TIMEOUT, True, LOG.debug),
             (self.EVENT_WORKFLOW_TIMEOUT, True, None),
-            (self.EVENT_STALL_TIMEOUT, False, None)
+            (self.EVENT_STALL_TIMEOUT, False, None),
+            (self.EVENT_RESTART_TIMEOUT, False, None)
         ]:
             interval = self._get_events_conf(event)
             if interval is not None:
                 timer = Timer(event, interval, log_reset_func)
                 if start_now:
                     timer.reset()
                 self.timers[event] = timer
 
+        if self.is_restart and not self.pool.get_all_tasks():
+            # This workflow completed before restart; wait for intervention.
+            with suppress(KeyError):
+                self.timers[self.EVENT_RESTART_TIMEOUT].reset()
+                self.is_restart_timeout_wait = True
+                LOG.warning(
+                    "This workflow already ran to completion."
+                    "\nTo make it continue, trigger new tasks"
+                    " before the restart timeout."
+                )
+
         # Main loop plugins
         self.main_loop_plugins = main_loop.load(
             self.cylc_config.get('main loop', {}),
             self.options.main_loop
         )
 
         holdcp = None
@@ -517,16 +533,15 @@
             holdcp = self.options.holdcp
         elif self.config.cfg['scheduling']['hold after cycle point']:
             holdcp = self.config.cfg['scheduling']['hold after cycle point']
         if holdcp is not None:
             self.command_set_hold_point(holdcp)
 
         if self.options.paused_start:
-            LOG.info("Paused on start up")
-            self.pause_workflow()
+            self.pause_workflow('Paused on start up')
 
         self.profiler.log_memory("scheduler.py: begin run while loop")
         self.is_updated = True
         if self.options.profile_mode:
             self.previous_profile_point = 0
             self.count = 0
 
@@ -535,15 +550,15 @@
         self.profiler.log_memory("scheduler.py: end configure")
 
     def load_workflow_params_and_tmpl_vars(self) -> None:
         """Load workflow params and template variables"""
         with self.workflow_db_mgr.get_pri_dao() as pri_dao:
             # This logic handles lack of initial cycle point in flow.cylc and
             # things that can't change on workflow restart/reload.
-            pri_dao.select_workflow_params(self._load_workflow_params)
+            self._load_workflow_params(pri_dao.select_workflow_params())
             pri_dao.select_workflow_template_vars(self._load_template_vars)
             pri_dao.execute_queued_items()
 
     def log_start(self) -> None:
         """Log headers, that also get logged on each rollover.
 
         Note: daemonize polls for 2 of these headers before detaching.
@@ -611,16 +626,18 @@
     async def run_scheduler(self) -> None:
         """Start the scheduler main loop."""
         try:
             if self.is_restart:
                 self.task_job_mgr.task_remote_mgr.is_restart = True
                 self.task_job_mgr.task_remote_mgr.rsync_includes = (
                     self.config.get_validated_rsync_includes())
-                self.restart_remote_init()
-                self.command_poll_tasks(['*/*'])
+                if self.pool.get_all_tasks():
+                    # (If we're not restarting a finished workflow)
+                    self.restart_remote_init()
+                    self.command_poll_tasks(['*/*'])
 
             self.run_event_handlers(self.EVENT_STARTUP, 'workflow starting')
             await asyncio.gather(
                 *main_loop.get_runners(
                     self.main_loop_plugins,
                     main_loop.CoroTypes.StartUp,
                     self
@@ -649,16 +666,31 @@
                 )
             except Exception as exc:
                 # Need to log traceback manually because otherwise this
                 # exception gets swallowed
                 LOG.exception(exc)
                 raise
 
-        except (KeyboardInterrupt, asyncio.CancelledError, Exception) as exc:
-            # Includes SchedulerError
+        except (KeyboardInterrupt, asyncio.CancelledError) as exc:
+            await self.handle_exception(exc)
+
+        except CylcError as exc:  # Includes SchedulerError
+            # catch "expected" errors
+            await self.handle_exception(exc)
+
+        except Exception as exc:
+            # catch "unexpected" errors
+            with suppress(Exception):
+                LOG.critical(
+                    'An uncaught error caused Cylc to shut down.'
+                    '\nIf you think this was an issue in Cylc,'
+                    ' please report the following traceback to the developers.'
+                    '\nhttps://github.com/cylc/cylc-flow/issues/new'
+                    '?assignees=&labels=bug&template=bug.md&title=;'
+                )
             await self.handle_exception(exc)
 
         else:
             # main loop ends (not used?)
             await self.shutdown(SchedulerStop(StopMode.AUTO.value))
 
         finally:
@@ -680,16 +712,16 @@
                 target=self.server.start,
                 args=(barrier,),
                 daemon=False
             )
             self.server.thread.start()
             barrier.wait()
 
-            await self.configure()
             self._configure_contact()
+            await self.configure()
         except (KeyboardInterrupt, asyncio.CancelledError, Exception) as exc:
             await self.handle_exception(exc)
 
     async def run(self):
         """Run the startup sequence and set the main loop running.
 
         Lightweight wrapper for testing convenience.
@@ -862,15 +894,15 @@
 
     def queue_command(self, command: str, kwargs: dict) -> None:
         self.command_queue.put((
             command,
             tuple(kwargs.values()), {}
         ))
 
-    def process_command_queue(self) -> None:
+    async def process_command_queue(self) -> None:
         """Process queued commands."""
         qsize = self.command_queue.qsize()
         if qsize <= 0:
             return
         LOG.debug(f"Processing {qsize} queued command(s)")
         while True:
             try:
@@ -881,31 +913,36 @@
             args_string = ', '.join(str(a) for a in args)
             kwargs_string = ', '.join(
                 f"{key}={value}" for key, value in kwargs.items()
             )
             sep = ', ' if kwargs_string and args_string else ''
             cmdstr = f"{name}({args_string}{sep}{kwargs_string})"
             try:
-                n_warnings: Optional[int] = self.get_command_method(name)(
-                    *args, **kwargs)
+                fcn = self.get_command_method(name)
+                n_warnings: Optional[int]
+                if inspect.iscoroutinefunction(fcn):
+                    n_warnings = await fcn(*args, **kwargs)
+                else:
+                    n_warnings = fcn(*args, **kwargs)
             except Exception as exc:
                 # Don't let a bad command bring the workflow down.
                 if (
                     cylc.flow.flags.verbosity > 1 or
                     not isinstance(exc, CommandFailedError)
                 ):
                     LOG.error(traceback.format_exc())
                 LOG.error(f"Command failed: {cmdstr}\n{exc}")
             else:
                 if n_warnings:
                     LOG.info(
-                        'Command succeeded with %s warning(s): %s' %
-                        (n_warnings, cmdstr))
+                        f"Command actioned with {n_warnings} warning(s): "
+                        f"{cmdstr}"
+                    )
                 else:
-                    LOG.info(f"Command succeeded: {cmdstr}")
+                    LOG.info(f"Command actioned: {cmdstr}")
                 self.is_updated = True
             self.command_queue.task_done()
 
     def info_get_graph_raw(self, cto, ctn, grouping=None):
         """Return raw graph."""
         return (
             self.config.get_graph_raw(cto, ctn, grouping),
@@ -1026,45 +1063,121 @@
             raise CommandFailedError(exc)
         cylc.flow.flags.verbosity = log_level_to_verbosity(lvl)
 
     def command_remove_tasks(self, items) -> int:
         """Remove tasks."""
         return self.pool.remove_tasks(items)
 
-    def command_reload_workflow(self) -> None:
+    async def command_reload_workflow(self) -> None:
         """Reload workflow configuration."""
-        LOG.info("Reloading the workflow definition.")
-        old_tasks = set(self.config.get_task_name_list())
-        # Things that can't change on workflow reload:
-        self.workflow_db_mgr.pri_dao.select_workflow_params(
-            self._load_workflow_params
-        )
+        # pause the workflow if not already
+        was_paused_before_reload = self.is_paused
+        if not was_paused_before_reload:
+            self.pause_workflow('Reloading workflow')
+            self.process_workflow_db_queue()  # see #5593
+
+        # flush out preparing tasks before attempting reload
+        self.reload_pending = 'waiting for pending tasks to submit'
+        while self.release_queued_tasks():
+            # Run the subset of main-loop functionality required to push
+            # preparing through the submission pipeline and keep the workflow
+            # responsive (e.g. to the `cylc stop` command).
+
+            # NOTE: this reload method was called by process_command_queue
+            # which is called synchronously in the main loop so this call is
+            # blocking to other main loop functions
+
+            # subproc pool - for issueing/tracking remote-init commands
+            self.proc_pool.process()
+            # task messages - for tracking task status changes
+            self.process_queued_task_messages()
+            # command queue - keeps the scheduler responsive
+            await self.process_command_queue()
+            # allows the scheduler to shutdown --now
+            await self.workflow_shutdown()
+            # keep the data store up to date with what's going on
+            await self.update_data_structure()
+            self.update_data_store()
+            # give commands time to complete
+            sleep(1)  # give any remove-init's time to complete
 
+        # reload the workflow definition
+        self.reload_pending = 'loading the workflow definition'
+        self.update_data_store()  # update workflow status msg
+        self._update_workflow_state()
+        LOG.info("Reloading the workflow definition.")
         try:
-            self.load_flow_file(is_reload=True)
+            config = self.load_flow_file(is_reload=True)
         except (ParsecError, CylcConfigError) as exc:
-            raise CommandFailedError(exc)
-        self.broadcast_mgr.linearized_ancestors = (
-            self.config.get_linearized_ancestors())
-        self.pool.set_do_reload(self.config)
-        self.task_events_mgr.mail_interval = self.cylc_config['mail'][
-            'task event batch interval']
-        self.task_events_mgr.mail_smtp = self._get_events_conf("smtp")
-        self.task_events_mgr.mail_footer = self._get_events_conf("footer")
-
-        # Log tasks that have been added by the reload, removed tasks are
-        # logged by the TaskPool.
-        add = set(self.config.get_task_name_list()) - old_tasks
-        for task in add:
-            LOG.warning(f"Added task: '{task}'")
-        self.workflow_db_mgr.put_workflow_template_vars(self.template_vars)
-        self.workflow_db_mgr.put_runtime_inheritance(self.config)
-        self.workflow_db_mgr.put_workflow_params(self)
-        self.is_updated = True
-        self.is_reloaded = True
+            if cylc.flow.flags.verbosity > 1:
+                # log full traceback in debug mode
+                LOG.exception(exc)
+            LOG.critical(
+                f'Reload failed - {exc.__class__.__name__}: {exc}'
+                '\nThis is probably due to an issue with the new'
+                ' configuration.'
+                '\nTo continue with the pre-reload config, un-pause the'
+                ' workflow.'
+                '\nOtherwise, fix the configuration and attempt to reload'
+                ' again.'
+            )
+        else:
+            self.reload_pending = 'applying the new config'
+            old_tasks = set(self.config.get_task_name_list())
+            # Things that can't change on workflow reload:
+            self._load_workflow_params(
+                self.workflow_db_mgr.pri_dao.select_workflow_params()
+            )
+            self.apply_new_config(config, is_reload=True)
+            self.broadcast_mgr.linearized_ancestors = (
+                self.config.get_linearized_ancestors())
+
+            self.task_events_mgr.mail_interval = self.cylc_config['mail'][
+                'task event batch interval']
+            self.task_events_mgr.mail_smtp = self._get_events_conf("smtp")
+            self.task_events_mgr.mail_footer = self._get_events_conf("footer")
+
+            # Log tasks that have been added by the reload, removed tasks are
+            # logged by the TaskPool.
+            add = set(self.config.get_task_name_list()) - old_tasks
+            for task in add:
+                LOG.warning(f"Added task: '{task}'")
+            self.workflow_db_mgr.put_workflow_template_vars(self.template_vars)
+            self.workflow_db_mgr.put_runtime_inheritance(self.config)
+            self.workflow_db_mgr.put_workflow_params(self)
+            self.process_workflow_db_queue()  # see #5593
+            self.is_updated = True
+            self.is_reloaded = True
+            self._update_workflow_state()
+
+            # Re-initialise data model on reload
+            self.data_store_mgr.initiate_data_model(reloaded=True)
+
+            # Reset the remote init map to trigger fresh file installation
+            self.task_job_mgr.task_remote_mgr.remote_init_map.clear()
+            self.task_job_mgr.task_remote_mgr.is_reload = True
+            self.pool.reload_taskdefs(config)
+            # Load jobs from DB
+            self.workflow_db_mgr.pri_dao.select_jobs_for_restart(
+                self.data_store_mgr.insert_db_job
+            )
+            if self.pool.compute_runahead(force=True):
+                self.pool.release_runahead_tasks()
+            self.is_reloaded = True
+            self.is_updated = True
+
+            LOG.info("Reload completed.")
+
+        # resume the workflow if previously paused
+        self.reload_pending = False
+        self.update_data_store()  # update workflow status msg
+        self._update_workflow_state()
+        if not was_paused_before_reload:
+            self.resume_workflow()
+            self.process_workflow_db_queue()  # see #5593
 
     def get_restart_num(self) -> int:
         """Return the number of the restart, else 0 if not a restart.
 
         Performs DB restart-check the first time this is called.
         """
         if not self.is_restart:
@@ -1087,22 +1200,22 @@
             fields.HOST:
                 self.host,
             fields.NAME:
                 self.workflow,
             fields.OWNER:
                 self.owner,
             fields.PORT:
-                str(self.server.port),  # type: ignore
+                str(self.server.port),
             fields.PID:
                 str(proc.pid),
             fields.COMMAND:
                 cli_format(proc.cmdline()),
             fields.PUBLISH_PORT:
-                str(self.server.pub_port),  # type: ignore
-            fields.WORKFLOW_RUN_DIR_ON_WORKFLOW_HOST:  # type: ignore
+                str(self.server.pub_port),
+            fields.WORKFLOW_RUN_DIR_ON_WORKFLOW_HOST:
                 self.workflow_run_dir,
             fields.UUID:
                 self.uuid_str,
             fields.VERSION:
                 CYLC_VERSION,
             fields.SCHEDULER_SSH_COMMAND:
                 str(get_platform()['ssh command']),
@@ -1113,29 +1226,29 @@
         }
         # fmt: on
 
     def _configure_contact(self) -> None:
         """Create contact file."""
         # Make sure another workflow of the same name hasn't started while this
         # one is starting
-        # NOTE: raises ServiceFileError if workflow is running
+        # NOTE: raises ContactFileExists if workflow is running
         workflow_files.detect_old_contact_file(self.workflow)
 
         # Extract contact data.
         contact_data = self.get_contact_data()
 
         # Write workflow contact file.
         # Preserve contact data in memory, for regular health check.
         workflow_files.dump_contact_file(self.workflow, contact_data)
         self.contact_data = contact_data
 
     def load_flow_file(self, is_reload=False):
         """Load, and log the workflow definition."""
         # Local workflow environment set therein.
-        self.config = WorkflowConfig(
+        return WorkflowConfig(
             self.workflow,
             self.flow_file,
             self.options,
             self.template_vars,
             xtrigger_mgr=self.xtrigger_mgr,
             mem_log_func=self.profiler.log_memory,
             output_fname=os.path.join(
@@ -1143,19 +1256,21 @@
                 workflow_files.WorkflowFiles.FLOW_FILE_PROCESSED
             ),
             run_dir=self.workflow_run_dir,
             log_dir=self.workflow_log_dir,
             work_dir=self.workflow_work_dir,
             share_dir=self.workflow_share_dir,
         )
+
+    def apply_new_config(self, config, is_reload=False):
+        self.config = config
         self.cylc_config = DictTree(
             self.config.cfg['scheduler'],
             glbl_cfg().get(['scheduler'])
         )
-
         self.flow_file_update_time = time()
         # Dump the loaded flow.cylc file for future reference.
         config_dir = get_workflow_run_config_log_dir(
             self.workflow)
         config_logs = get_sorted_logs_by_time(config_dir, "*[0-9].cylc")
         log_num = get_next_log_number(config_logs[-1]) if config_logs else 1
         if is_reload:
@@ -1186,81 +1301,87 @@
             ),
             'CYLC_WORKFLOW_INITIAL_CYCLE_POINT': str(
                 self.config.initial_point
             ),
             'CYLC_WORKFLOW_FINAL_CYCLE_POINT': str(self.config.final_point),
         })
 
-    def _load_workflow_params(self, row_idx, row):
+    def _load_workflow_params(
+        self, params: Iterable[Tuple[str, Optional[str]]]
+    ) -> None:
         """Load a row in the "workflow_params" table in a restart/reload.
 
         This currently includes:
         * Initial/Final cycle points.
         * Start/Stop Cycle points.
         * Stop task.
         * Workflow UUID.
         * A flag to indicate if the workflow should be paused or not.
         * Original workflow run time zone.
         """
-        if row_idx == 0:
-            LOG.info('LOADING workflow parameters')
-        key, value = row
-        if key in self.workflow_db_mgr.KEY_INITIAL_CYCLE_POINT_COMPATS:
-            self.options.icp = value
-            LOG.info(f"+ initial point = {value}")
-        elif key in self.workflow_db_mgr.KEY_START_CYCLE_POINT_COMPATS:
-            self.options.startcp = value
-            LOG.info(f"+ start point = {value}")
-        elif key in self.workflow_db_mgr.KEY_FINAL_CYCLE_POINT_COMPATS:
-            if self.is_restart and self.options.fcp == 'reload':
-                LOG.debug(f"- final point = {value} (ignored)")
-            elif self.options.fcp is None:
-                self.options.fcp = value
-                LOG.info(f"+ final point = {value}")
-        elif key == self.workflow_db_mgr.KEY_STOP_CYCLE_POINT:
-            if self.is_restart and self.options.stopcp == 'reload':
-                LOG.debug(f"- stop point = {value} (ignored)")
-            elif self.options.stopcp is None:
-                self.options.stopcp = value
-                LOG.info(f"+ stop point = {value}")
-        elif key == self.workflow_db_mgr.KEY_RUN_MODE:
-            if self.options.run_mode is None:
+        LOG.info('LOADING workflow parameters')
+        for key, value in params:
+            if value is None:
+                continue
+            if key in self.workflow_db_mgr.KEY_INITIAL_CYCLE_POINT_COMPATS:
+                self.options.icp = value
+                LOG.info(f"+ initial point = {value}")
+            elif key in self.workflow_db_mgr.KEY_START_CYCLE_POINT_COMPATS:
+                self.options.startcp = value
+                LOG.info(f"+ start point = {value}")
+            elif key in self.workflow_db_mgr.KEY_FINAL_CYCLE_POINT_COMPATS:
+                if self.is_restart and self.options.fcp == 'reload':
+                    LOG.debug(f"- final point = {value} (ignored)")
+                elif self.options.fcp is None:
+                    self.options.fcp = value
+                    LOG.info(f"+ final point = {value}")
+            elif key == self.workflow_db_mgr.KEY_STOP_CYCLE_POINT:
+                if self.is_restart and self.options.stopcp == 'reload':
+                    LOG.debug(f"- stop point = {value} (ignored)")
+                elif self.options.stopcp is None:
+                    self.options.stopcp = value
+                    LOG.info(f"+ stop point = {value}")
+            elif (
+                key == self.workflow_db_mgr.KEY_RUN_MODE
+                and self.options.run_mode is None
+            ):
                 self.options.run_mode = value
                 LOG.info(f"+ run mode = {value}")
-        elif key == self.workflow_db_mgr.KEY_UUID_STR:
-            self.uuid_str = value
-            LOG.info('+ workflow UUID = %s', value)
-        elif key == self.workflow_db_mgr.KEY_PAUSED:
-            if self.options.paused_start is None:
-                self.options.paused_start = bool(value)
-                LOG.info(f'+ paused = {bool(value)}')
-        elif key == self.workflow_db_mgr.KEY_HOLD_CYCLE_POINT:
-            if self.options.holdcp is None:
+            elif key == self.workflow_db_mgr.KEY_UUID_STR:
+                self.uuid_str = value
+                LOG.info(f"+ workflow UUID = {value}")
+            elif key == self.workflow_db_mgr.KEY_PAUSED:
+                bool_val = bool(int(value))
+                if bool_val and not self.options.paused_start:
+                    self.options.paused_start = bool_val
+                    LOG.info(f"+ paused = {bool_val}")
+            elif (
+                key == self.workflow_db_mgr.KEY_HOLD_CYCLE_POINT
+                and self.options.holdcp is None
+            ):
                 self.options.holdcp = value
-                LOG.info('+ hold point = %s', value)
-        elif key == self.workflow_db_mgr.KEY_STOP_CLOCK_TIME:
-            value = int(value)
-            if time() <= value:
-                self.stop_clock_time = value
-                LOG.info('+ stop clock time = %d (%s)', value, time2str(value))
-            else:
-                LOG.debug(
-                    '- stop clock time = %d (%s) (ignored)',
-                    value,
-                    time2str(value))
-        elif key == self.workflow_db_mgr.KEY_STOP_TASK:
-            self.restored_stop_task_id = value
-            LOG.info('+ stop task = %s', value)
-        elif key == self.workflow_db_mgr.KEY_UTC_MODE:
-            value = bool(int(value))
-            self.options.utc_mode = value
-            LOG.info(f"+ UTC mode = {value}")
-        elif key == self.workflow_db_mgr.KEY_CYCLE_POINT_TIME_ZONE:
-            self.options.cycle_point_tz = value
-            LOG.info(f"+ cycle point time zone = {value}")
+                LOG.info(f"+ hold point = {value}")
+            elif key == self.workflow_db_mgr.KEY_STOP_CLOCK_TIME:
+                int_val = int(value)
+                msg = f"stop clock time = {int_val} ({time2str(int_val)})"
+                if time() <= int_val:
+                    self.stop_clock_time = int_val
+                    LOG.info(f"+ {msg}")
+                else:
+                    LOG.debug(f"- {msg} (ignored)")
+            elif key == self.workflow_db_mgr.KEY_STOP_TASK:
+                self.restored_stop_task_id = value
+                LOG.info(f"+ stop task = {value}")
+            elif key == self.workflow_db_mgr.KEY_UTC_MODE:
+                bool_val = bool(int(value))
+                self.options.utc_mode = bool_val
+                LOG.info(f"+ UTC mode = {bool_val}")
+            elif key == self.workflow_db_mgr.KEY_CYCLE_POINT_TIME_ZONE:
+                self.options.cycle_point_tz = value
+                LOG.info(f"+ cycle point time zone = {value}")
 
     def _load_template_vars(self, _, row):
         """Load workflow start up template variables."""
         key, value = row
         # Command line argument takes precedence
         if key not in self.template_vars:
             self.template_vars[key] = eval_var(value)
@@ -1274,15 +1395,15 @@
         with suppress(KeyError):
             if (
                 conf.run_mode('simulation', 'dummy')
             ):
                 return
         self.workflow_event_handler.handle(self, event, str(reason))
 
-    def release_queued_tasks(self) -> None:
+    def release_queued_tasks(self) -> bool:
         """Release queued tasks, and submit jobs.
 
         The task queue manages references to task proxies in the task pool.
 
         Tasks which have entered the submission pipeline but not yet finished
         (pre_prep_tasks) are passed to job submission multiple times until they
         have passed through a series of asynchronous operations (host select,
@@ -1292,37 +1413,50 @@
             We do not maintain a list of "pre_prep_tasks" between iterations
             of this method as this creates an intermediate task staging pool
             which has nasty consequences:
 
             * https://github.com/cylc/cylc-flow/pull/4620
             * https://github.com/cylc/cylc-flow/issues/4974
 
+        Returns:
+            True if tasks were passed through the submit-pipeline
+            (i.e. new waiting tasks have entered the preparing state OR
+            preparing tasks have been passed back through for
+            submission).
+
         """
         if (
             not self.is_paused
             and self.stop_mode is None
             and self.auto_restart_time is None
+            and self.reload_pending is False
         ):
             pre_prep_tasks = self.pool.release_queued_tasks()
 
         elif (
-            self.should_auto_restart_now()
-            and self.auto_restart_mode == AutoRestartMode.RESTART_NORMAL
+            (
+                # Need to get preparing tasks to submit before auto restart
+                self.should_auto_restart_now()
+                and self.auto_restart_mode == AutoRestartMode.RESTART_NORMAL
+            ) or (
+                # Need to get preparing tasks to submit before reload
+                self.reload_pending
+            )
         ):
-            # Need to get preparing tasks to submit before auto restart
+            # don't release queued tasks, finish processing preparing tasks
             pre_prep_tasks = [
                 itask for itask in self.pool.get_tasks()
                 if itask.state(TASK_STATUS_PREPARING)
             ]
 
         # Return, if no tasks to submit.
         else:
-            return
+            return False
         if not pre_prep_tasks:
-            return
+            return False
 
         # Start the job submission process.
         self.is_updated = True
         self.reset_inactivity_timer()
 
         self.task_job_mgr.task_remote_mgr.rsync_includes = (
             self.config.get_validated_rsync_includes())
@@ -1342,14 +1476,17 @@
             else:
                 flow = FLOW_NONE
             log(
                 f"{itask.identity} -triggered off "
                 f"{itask.state.get_resolved_dependencies()} in flow {flow}"
             )
 
+        # one or more tasks were passed through the submission pipeline
+        return True
+
     def process_workflow_db_queue(self):
         """Update workflow DB."""
         self.workflow_db_mgr.process_queued_ops()
 
     def database_health_check(self):
         """If public database is stuck, blast it away by copying the content
         of the private database into it."""
@@ -1397,29 +1534,29 @@
             self.pool.stop_task_done() or
             self.check_auto_shutdown()
         ):
             self._set_stop(StopMode.AUTO)
 
         # Is the workflow ready to shut down now?
         if self.pool.can_stop(self.stop_mode):
-            await self.update_data_structure()
+            await self.update_data_structure(self.is_reloaded)
             self.proc_pool.close()
             if self.stop_mode != StopMode.REQUEST_NOW_NOW:
                 # Wait for process pool to complete,
                 # unless --now --now is requested
                 stop_process_pool_empty_msg = (
                     "Waiting for the command process pool to empty" +
                     " for shutdown")
                 while self.proc_pool.is_not_done():
                     sleep(self.INTERVAL_STOP_PROCESS_POOL_EMPTY)
                     if stop_process_pool_empty_msg:
                         LOG.info(stop_process_pool_empty_msg)
                         stop_process_pool_empty_msg = None
                     self.proc_pool.process()
-                    self.process_command_queue()
+                    await self.process_command_queue()
             if self.options.profile_mode:
                 self.profiler.log_memory(
                     "scheduler.py: end main loop (total loops %d): %s" %
                     (self.count, get_current_time_string()))
             if self.stop_mode == StopMode.AUTO_ON_TASK_FAILURE:
                 raise SchedulerError(self.stop_mode.value)
             else:
@@ -1538,31 +1675,16 @@
         while True:  # MAIN LOOP
             tinit = time()
 
             # Useful for debugging core scheduler issues:
             # self.pool.log_task_pool(logging.CRITICAL)
             if self.incomplete_ri_map:
                 self.manage_remote_init()
-            if self.pool.do_reload:
-                # Re-initialise data model on reload
-                self.data_store_mgr.initiate_data_model(reloaded=True)
-                # Reset the remote init map to trigger fresh file installation
-                self.task_job_mgr.task_remote_mgr.remote_init_map.clear()
-                self.task_job_mgr.task_remote_mgr.is_reload = True
-                self.pool.reload_taskdefs()
-                # Load jobs from DB
-                self.workflow_db_mgr.pri_dao.select_jobs_for_restart(
-                    self.data_store_mgr.insert_db_job)
-                LOG.info("Reload completed.")
-                if self.pool.compute_runahead(force=True):
-                    self.pool.release_runahead_tasks()
-                self.is_reloaded = True
-                self.is_updated = True
 
-            self.process_command_queue()
+            await self.process_command_queue()
             self.proc_pool.process()
 
             # Tasks in the main pool that are waiting but not queued must be
             # waiting on external dependencies, i.e. xtriggers or ext_triggers.
             # For these tasks, call any unsatisfied xtrigger functions, and
             # queue tasks that have become ready. (Tasks do not appear in the
             # main pool at all until all other-task deps are satisfied, and are
@@ -1597,21 +1719,14 @@
                     and not itask.state.external_triggers_all_satisfied()
                     and self.broadcast_mgr.check_ext_triggers(
                         itask, self.ext_trigger_queue)
                     and all(itask.is_ready_to_run())
                 ):
                     self.pool.queue_task(itask)
 
-                # Old-style clock-trigger tasks:
-                if (
-                    itask.tdef.clocktrigger_offset is not None
-                    and all(itask.is_ready_to_run())
-                ):
-                    self.pool.queue_task(itask)
-
             if housekeep_xtriggers:
                 # (Could do this periodically?)
                 self.xtrigger_mgr.housekeep(self.pool.get_tasks())
 
             self.pool.set_expired_tasks()
             self.release_queued_tasks()
 
@@ -1619,24 +1734,49 @@
                 # A simulated task state change occurred.
                 self.reset_inactivity_timer()
 
             self.broadcast_mgr.expire_broadcast(self.pool.get_min_point())
             self.late_tasks_check()
 
             self.process_queued_task_messages()
-            self.process_command_queue()
+            await self.process_command_queue()
             self.task_events_mgr.process_events(self)
 
             # Update state summary, database, and uifeed
             self.workflow_db_mgr.put_task_event_timers(self.task_events_mgr)
-            has_updated = await self.update_data_structure()
-            if has_updated and not self.is_stalled:
-                # Stop the stalled timer.
+
+            # List of task whose states have changed.
+            updated_task_list = [
+                t for t in self.pool.get_tasks() if t.state.is_updated]
+            has_updated = updated_task_list or self.is_updated
+
+            if updated_task_list and self.is_restart_timeout_wait:
+                # Stop restart timeout if action has been triggered.
                 with suppress(KeyError):
-                    self.timers[self.EVENT_STALL_TIMEOUT].stop()
+                    self.timers[self.EVENT_RESTART_TIMEOUT].stop()
+                    self.is_restart_timeout_wait = False
+
+            if has_updated:
+                # Update the datastore.
+                await self.update_data_structure(self.is_reloaded)
+
+                if not self.is_reloaded:
+                    # (A reload cannot un-stall workflow by itself)
+                    self.is_stalled = False
+                self.is_reloaded = False
+
+                # Reset workflow and task updated flags.
+                self.is_updated = False
+                for itask in updated_task_list:
+                    itask.state.is_updated = False
+
+                if not self.is_stalled:
+                    # Stop the stalled timer.
+                    with suppress(KeyError):
+                        self.timers[self.EVENT_STALL_TIMEOUT].stop()
 
             self.process_workflow_db_queue()
 
             # If public database is stuck, blast it away by copying the content
             # of the private database into it.
             self.database_health_check()
 
@@ -1677,56 +1817,69 @@
             else:
                 duration = self.INTERVAL_MAIN_LOOP - elapsed
             await asyncio.sleep(duration)
             # Record latest main loop interval
             self.main_loop_intervals.append(time() - tinit)
             # END MAIN LOOP
 
-    async def update_data_structure(self) -> Union[bool, List['TaskProxy']]:
+    def _update_workflow_state(self):
+        """Update workflow state in the data store and push out any deltas.
+
+        A cut-down version of update_data_structure which only considers
+        workflow state changes e.g. status, status message, state totals, etc.
+        """
+        # update the workflow state in the data store
+        self.data_store_mgr.update_workflow()
+
+        # push out update deltas
+        self.data_store_mgr.batch_deltas()
+        self.data_store_mgr.apply_delta_batch()
+        self.data_store_mgr.apply_delta_checksum()
+        self.data_store_mgr.publish_deltas = (
+            self.data_store_mgr.get_publish_deltas()
+        )
+        self.server.publish_queue.put(
+            self.data_store_mgr.publish_deltas)
+
+        # Non-async sleep - yield to other threads rather
+        # than event loop
+        sleep(0)
+
+    async def update_data_structure(self, reloaded: bool = False):
         """Update DB, UIS, Summary data elements"""
-        updated_tasks = [
-            t for t in self.pool.get_tasks() if t.state.is_updated]
-        has_updated = self.is_updated or updated_tasks
-        reloaded = self.is_reloaded
-        # Add tasks that have moved moved from runahead to live pool.
-        if has_updated or self.data_store_mgr.updates_pending:
+        # Add tasks that have moved from runahead to live pool.
+        if self.data_store_mgr.updates_pending:
             # Collect/apply data store updates/deltas
             self.data_store_mgr.update_data_structure(reloaded=reloaded)
-            self.is_reloaded = False
             # Publish updates:
             if self.data_store_mgr.publish_pending:
                 self.data_store_mgr.publish_pending = False
                 self.server.publish_queue.put(
                     self.data_store_mgr.publish_deltas)
                 # Non-async sleep - yield to other threads rather
                 # than event loop
                 sleep(0)
-        if has_updated:
-            # Database update
-            self.workflow_db_mgr.put_task_pool(self.pool)
-            # Reset workflow and task updated flags.
-            self.is_updated = False
-            if not reloaded:  # (A reload cannot unstall workflow by itself)
-                self.is_stalled = False
-            for itask in updated_tasks:
-                itask.state.is_updated = False
-            self.update_data_store()
-        return has_updated
+        # Database update
+        self.workflow_db_mgr.put_task_pool(self.pool)
+        self.update_data_store()
 
     def check_workflow_timers(self):
         """Check timers, and abort or run event handlers as configured."""
         for event, timer in self.timers.items():
             if not timer.timed_out():
                 continue
             abort_conf = f"abort on {event}"
             if self._get_events_conf(abort_conf):
                 # "cylc play" needs to exit with error status here.
                 raise SchedulerError(f'"{abort_conf}" is set')
             if self._get_events_conf(f"{event} handlers") is not None:
                 self.run_event_handlers(event)
+            if event == self.EVENT_RESTART_TIMEOUT:
+                # Unset wait flag to allow normal shutdown.
+                self.is_restart_timeout_wait = False
 
     def check_workflow_stalled(self) -> bool:
         """Check if workflow is stalled or not."""
         if self.is_stalled:  # already reported
             return True
         if self.is_paused:  # cannot be stalled it's not even running
             return False
@@ -1794,23 +1947,30 @@
         if self.server:
             await self.server.stop(reason)
 
         # Flush errors and info before removing workflow contact file
         sys.stdout.flush()
         sys.stderr.flush()
 
+        if (
+            self.workflow_db_mgr.pri_path
+            and Path(self.workflow_db_mgr.pri_path).exists()
+        ):
+            # only attempt remote tidy if the workflow has been started
+            self.task_job_mgr.task_remote_mgr.remote_tidy()
+
         try:
             # Remove ZMQ keys from scheduler
             LOG.debug("Removing authentication keys from scheduler")
             key_housekeeping(self.workflow, create=False)
         except Exception as ex:
             LOG.exception(ex)
         # disconnect from workflow-db, stop db queue
         try:
-            self.workflow_db_mgr.process_queued_ops()
+            self.process_workflow_db_queue()
             self.workflow_db_mgr.on_workflow_shutdown()
         except Exception as exc:
             LOG.exception(exc)
 
         # NOTE: Removing the contact file should happen last of all (apart
         # from running event handlers), because the existence of the file is
         # used to determine if the workflow is running
@@ -1821,16 +1981,14 @@
             except OSError as exc:
                 LOG.warning(f"failed to remove workflow contact file: {fname}")
                 LOG.exception(exc)
             else:
                 # Useful to identify that this Scheduler has shut down
                 # properly (e.g. in tests):
                 self.contact_data = None
-            if self.task_job_mgr:
-                self.task_job_mgr.task_remote_mgr.remote_tidy()
 
         # The getattr() calls and if tests below are used in case the
         # workflow is not fully configured before the shutdown is called.
         if getattr(self, "config", None) is not None:
             # run shutdown handlers
             if isinstance(reason, CylcError):
                 self.run_event_handlers(self.EVENT_SHUTDOWN, reason.args[0])
@@ -1879,76 +2037,90 @@
         if self.stop_clock_time is None:
             return
         now = time()
         if now > self.stop_clock_time:
             LOG.info("Wall clock stop time reached: %s", time2str(
                 self.stop_clock_time))
             self.stop_clock_time = None
-            self.workflow_db_mgr.delete_workflow_stop_clock_time()
+            self.workflow_db_mgr.put_workflow_stop_clock_time(None)
             self.update_data_store()
             return True
         LOG.debug("stop time=%d; current time=%d", self.stop_clock_time, now)
         return False
 
     def check_auto_shutdown(self):
         """Check if we should shut down now."""
-        if self.is_paused:
-            # Don't if paused.
-            return False
-
-        if self.check_workflow_stalled():
-            return False
-
-        if any(
-            itask for itask in self.pool.get_tasks()
-            if itask.state(
-                TASK_STATUS_PREPARING,
-                TASK_STATUS_SUBMITTED,
-                TASK_STATUS_RUNNING
-            )
-            or (
-                itask.state(TASK_STATUS_WAITING)
-                and not itask.state.is_runahead
+        if (
+            self.is_paused or
+            self.is_restart_timeout_wait or
+            self.check_workflow_stalled() or
+            # if more tasks to run (if waiting and not
+            # runahead, then held, queued, or xtriggered).
+            any(
+                itask for itask in self.pool.get_tasks()
+                if itask.state(
+                    TASK_STATUS_PREPARING,
+                    TASK_STATUS_SUBMITTED,
+                    TASK_STATUS_RUNNING
+                )
+                or (
+                    itask.state(TASK_STATUS_WAITING)
+                    and not itask.state.is_runahead
+                )
             )
         ):
-            # Don't if there are more tasks to run (if waiting and not
-            # runahead, then held, queued, or xtriggered).
             return False
 
         # Can shut down.
         if self.pool.stop_point:
             # Forget early stop point in case of a restart.
-            self.workflow_db_mgr.delete_workflow_stop_cycle_point()
+            self.workflow_db_mgr.put_workflow_stop_cycle_point(None)
 
         return True
 
-    def pause_workflow(self) -> None:
-        """Pause the workflow."""
+    def pause_workflow(self, msg: Optional[str] = None) -> None:
+        """Pause the workflow.
+
+        Args:
+            msg:
+                A user-facing string explaining why the workflow was paused if
+                helpful.
+
+        """
         if self.is_paused:
             LOG.info("Workflow is already paused")
             return
-        LOG.info("PAUSING the workflow now")
+        _msg = "PAUSING the workflow now"
+        if msg:
+            _msg += f': {msg}'
+        LOG.info(_msg)
         self.is_paused = True
-        self.workflow_db_mgr.put_workflow_paused()
+        self.workflow_db_mgr.put_workflow_paused(True)
         self.update_data_store()
 
     def resume_workflow(self, quiet: bool = False) -> None:
         """Resume the workflow.
 
         Args:
-            quiet: whether to log anything.
+            quiet:
+                Whether to log anything in the event the workflow is not
+                paused.
+
         """
+        if self.reload_pending:
+            LOG.warning('Cannot resume - workflow is reloading')
+            return
         if not self.is_paused:
             if not quiet:
-                LOG.warning("Cannot resume - workflow is not paused")
+                LOG.warning("No need to resume - workflow is not paused")
             return
         if not quiet:
             LOG.info("RESUMING the workflow now")
         self.is_paused = False
-        self.workflow_db_mgr.delete_workflow_paused()
+        self.workflow_db_mgr.put_workflow_paused(False)
         self.update_data_store()
 
     def command_force_trigger_tasks(self, items, flow, flow_wait, flow_descr):
         """Manual task trigger."""
         return self.pool.force_trigger_tasks(
             items, flow, flow_wait, flow_descr)
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scheduler_cli.py` & `cylc-flow-8.2.0/cylc/flow/scheduler_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,19 @@
 from shlex import quote
 import sys
 from typing import TYPE_CHECKING
 
 from pkg_resources import parse_version
 
 from cylc.flow import LOG, __version__
-from cylc.flow.exceptions import ServiceFileError
+from cylc.flow.exceptions import (
+    ContactFileExists,
+    CylcError,
+    ServiceFileError,
+)
 import cylc.flow.flags
 from cylc.flow.id import upgrade_legacy_ids
 from cylc.flow.host_select import select_workflow_host
 from cylc.flow.hostuserutil import is_remote_host
 from cylc.flow.id_cli import parse_ids
 from cylc.flow.loggingutil import (
     close_log,
@@ -130,15 +134,15 @@
 )
 
 PLAY_RUN_MODE = deepcopy(RUN_MODE)
 PLAY_RUN_MODE.sources = {'play'}
 
 PLAY_OPTIONS = [
     OptionSettings(
-        ["-n", "--no-detach", "--non-daemon"],
+        ["-N", "--no-detach", "--non-daemon"],
         help="Do not daemonize the scheduler (infers --format=plain)",
         action='store_true', dest="no_detach", sources={'play'}),
     OptionSettings(
         ["--profile"],
         help="Output profiling (performance) information",
         action='store_true',
         default=False,
@@ -195,14 +199,15 @@
         dest="starttask",
         sources={'play'},
     ),
     OptionSettings(
         ["--pause"],
         help="Pause the workflow immediately on start up.",
         action='store_true',
+        default=False,
         dest="paused_start",
         sources={'play'},
     ),
     OptionSettings(
         ["--hold-after", "--hold-cycle-point", "--holdcp"],
         help="Hold all tasks after this cycle point.",
         metavar="CYCLE_POINT",
@@ -382,15 +387,15 @@
     ):
         sys.exit(1)
 
     # upgrade the workflow DB (after user has confirmed upgrade)
     _upgrade_database(db_file)
 
     # re-execute on another host if required
-    _distribute(options.host, workflow_id_raw, workflow_id)
+    _distribute(options.host, workflow_id_raw, workflow_id, options.color)
 
     # print the start message
     _print_startup_message(options)
 
     # setup the scheduler
     # NOTE: asyncio.run opens an event loop, runs your coro,
     #       then shutdown async generators and closes the event loop
@@ -427,29 +432,29 @@
     sys.exit(ret)
 
 
 def _resume(workflow_id, options):
     """Resume the workflow if it is already running."""
     try:
         detect_old_contact_file(workflow_id)
-    except ServiceFileError as exc:
+    except ContactFileExists as exc:
         print(f"Resuming already-running workflow\n\n{exc}")
         pclient = WorkflowRuntimeClient(
             workflow_id,
             timeout=options.comms_timeout,
         )
         mutation_kwargs = {
             'request_string': RESUME_MUTATION,
             'variables': {
                 'wFlows': [workflow_id]
             }
         }
         pclient('graphql', mutation_kwargs)
         sys.exit(0)
-    except Exception as exc:
+    except CylcError as exc:
         LOG.error(exc)
         LOG.critical(
             'Cannot tell if the workflow is running'
             '\nNote, Cylc 8 cannot restart Cylc 7 workflows.'
         )
         sys.exit(1)
 
@@ -519,14 +524,15 @@
                         f' <yellow>{last_run_version}</yellow>'
                         f' to <green>{__version__}</green>?'
                     ),
                     {'y': True, 'n': False},
                     process=str.lower,
                 )
             # we are in non-interactive mode, abort abort abort
+            print('Use "--upgrade" to upgrade the workflow.', file=sys.stderr)
             return False
         elif itt > 2 and this > that:
             # restart would INCREASE the Cylc version in a little way
             return True
     return True
 
 
@@ -553,15 +559,15 @@
             )
         )
 
     if cylc.flow.flags.cylc7_back_compat:
         LOG.warning(SUITERC_DEPR_MSG)
 
 
-def _distribute(host, workflow_id_raw, workflow_id):
+def _distribute(host, workflow_id_raw, workflow_id, color):
     """Re-invoke this command on a different host if requested.
 
     Args:
         host:
             The remote host to re-invoke on.
         workflow_id_raw:
             The workflow ID as it appears in the CLI arguments.
@@ -585,14 +591,23 @@
             for ind, item in enumerate(cmd):
                 if item == workflow_id_raw:
                     cmd[ind] = workflow_id
 
         # Prevent recursive host selection
         cmd.append("--host=localhost")
 
+        # Preserve CLI colour
+        if is_terminal() and color != 'never':
+            # the detached process doesn't pass the is_terminal test
+            # so we have to explicitly tell Cylc to use color
+            cmd.append('--color=always')
+        else:
+            # otherwise set --color=never to make testing easier
+            cmd.append('--color=never')
+
         # Re-invoke the command
         # NOTE: has the potential to raise NoHostsError, however, this will
         # most likely have been raised during host-selection
         cylc_server_cmd(cmd, host=host)
         sys.exit(0)
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/__init__.py` & `cylc-flow-8.2.0/cylc/flow/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/broadcast.py` & `cylc-flow-8.2.0/cylc/flow/scripts/broadcast.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/cat_log.py` & `cylc-flow-8.2.0/cylc/flow/scripts/cat_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
         # * batchview command is user configurable
         colorise_cat_log(proc1, color=color)
         return 0
     if mode == 'tail':
         if batchview_cmd is not None:
             cmd = batchview_cmd
         else:
-            cmd = tailer_tmpl % {"filename": logpath}
+            cmd = tailer_tmpl % {"filename": shlex.quote(str(logpath))}
         proc = Popen(shlex.split(cmd), stdin=DEVNULL)  # nosec
         # * batchview command is user configurable
         with suppress(KeyboardInterrupt):
             watch_and_kill(proc)
         return proc.wait()
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/check_versions.py` & `cylc-flow-8.2.0/cylc/flow/scripts/check_versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from cylc.flow.cylc_subproc import procopen, PIPE, DEVNULL
 from cylc.flow import __version__ as CYLC_VERSION
 from cylc.flow.config import WorkflowConfig
 from cylc.flow.exceptions import NoHostsError
 from cylc.flow.id_cli import parse_id
 from cylc.flow.platforms import get_platform, get_host_from_platform
 from cylc.flow.remote import construct_ssh_cmd
-from cylc.flow.templatevars import load_template_vars
+from cylc.flow.templatevars import get_template_vars
 from cylc.flow.terminal import cli_function
 
 if TYPE_CHECKING:
     from optparse import Values
 
 
 def get_option_parser():
@@ -83,15 +83,15 @@
     )
 
     # extract task host platforms from the workflow_id
     config = WorkflowConfig(
         workflow_id,
         flow_file,
         options,
-        load_template_vars(options.templatevars, options.templatevars_file))
+        get_template_vars(options))
 
     platforms = {
         config.get_config(['runtime', name, 'platform'])
         for name in config.get_namespace_list('all tasks')
     } - {None, 'localhost'}
 
     # When "workflow run hosts" are formalised as "flow platforms"
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/clean.py` & `cylc-flow-8.2.0/cylc/flow/scripts/clean.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 NOTE: this command is intended for workflows installed with `cylc install`. If
 this is run for a workflow that was instead written directly in ~/cylc-run and
 not backed up elsewhere, it will be lost.
 
 It will also remove any symlink directory targets.
 
-Workflow names can be hierarchical, corresponding to the path under ~/cylc-run.
+Workflow IDs can be hierarchical, corresponding to the path under ~/cylc-run.
 
 Examples:
   # Remove the workflow at ~/cylc-run/foo/bar
   $ cylc clean foo/bar
 
   # Remove multiple workflows
   $ cylc clean one two three
@@ -60,25 +60,25 @@
 """
 
 import asyncio
 import sys
 from typing import TYPE_CHECKING, Iterable, List, Tuple
 
 from cylc.flow import LOG
+from cylc.flow.clean import init_clean, get_contained_workflows
 from cylc.flow.exceptions import CylcError, InputError
 import cylc.flow.flags
 from cylc.flow.id_cli import parse_ids_async
-from cylc.flow.loggingutil import disable_timestamps
+from cylc.flow.loggingutil import set_timestamps
 from cylc.flow.option_parsers import (
     WORKFLOW_ID_MULTI_ARG_DOC,
     CylcOptionParser as COP,
     Options,
 )
 from cylc.flow.terminal import cli_function, is_terminal
-from cylc.flow.workflow_files import init_clean, get_contained_workflows
 
 if TYPE_CHECKING:
     from optparse import Values
 
 
 def get_option_parser():
     parser = COP(
@@ -205,15 +205,15 @@
             msg += f"\nWorkflow: {workflow}\nError: {exc_message}"
         raise CylcError(msg)
 
 
 @cli_function(get_option_parser)
 def main(_, opts: 'Values', *ids: str):
     if cylc.flow.flags.verbosity < 2:
-        disable_timestamps(LOG)
+        set_timestamps(LOG, False)
 
     if opts.local_only and opts.remote_only:
         raise InputError(
             "--local and --remote options are mutually exclusive"
         )
 
     asyncio.run(run(*ids, opts=opts))
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/client.py` & `cylc-flow-8.2.0/cylc/flow/scripts/client.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/common.py` & `cylc-flow-8.2.0/cylc/flow/scripts/common.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/completion_server.py` & `cylc-flow-8.2.0/cylc/flow/scripts/completion_server.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/config.py` & `cylc-flow-8.2.0/cylc/flow/scripts/config.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/cycle_point.py` & `cylc-flow-8.2.0/cylc/flow/scripts/cycle_point.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/cylc.py` & `cylc-flow-8.2.0/cylc/flow/scripts/cylc.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,19 @@
     print(ID_HELP)
 
 
 def print_license() -> None:
     try:
         from importlib.metadata import files
     except ImportError:
-        from importlib_metadata import files
+        # BACK COMPAT: importlib_metadata
+        #   importlib.metadata was added in Python 3.8
+        # FROM: Python 3.7
+        # TO: Python: 3.8
+        from importlib_metadata import files  # type: ignore[no-redef]
     license_file = next(filter(
         lambda f: f.name == 'COPYING', files('cylc-flow')
     ))
     print(license_file.read_text())
 
 
 def print_command_list(commands=None, indent=0):
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/diff.py` & `cylc-flow-8.2.0/cylc/flow/scripts/diff.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from cylc.flow.id_cli import parse_id
 from cylc.flow.option_parsers import (
     WORKFLOW_ID_OR_PATH_ARG_DOC,
     CylcOptionParser as COP,
     icp_option,
 )
 from cylc.flow.config import WorkflowConfig
-from cylc.flow.templatevars import load_template_vars
+from cylc.flow.templatevars import get_template_vars
 from cylc.flow.terminal import cli_function
 
 if TYPE_CHECKING:
     from optparse import Values
 
 
 n_oone = 0
@@ -151,17 +151,15 @@
         workflow_id2,
         src=True,
         constraint='workflows',
     )
     if workflow_file_1_ == workflow_file_2_:
         parser.error("You can't diff a single workflow.")
     print(f"Parsing {workflow_id_1} ({workflow_file_1_})")
-    template_vars = load_template_vars(
-        options.templatevars, options.templatevars_file
-    )
+    template_vars = get_template_vars(options)
     config1 = WorkflowConfig(
         workflow_id_1, workflow_file_1_, options, template_vars
     ).cfg
     print(f"Parsing {workflow_id_2} ({workflow_file_2_})")
     config2 = WorkflowConfig(
         workflow_id_2, workflow_file_2_, options, template_vars
     ).cfg
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/dump.py` & `cylc-flow-8.2.0/cylc/flow/scripts/dump.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/ext_trigger.py` & `cylc-flow-8.2.0/cylc/flow/scripts/ext_trigger.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/function_run.py` & `cylc-flow-8.2.0/cylc/flow/scripts/function_run.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/get_resources.py` & `cylc-flow-8.2.0/cylc/flow/scripts/get_resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     $ cylc get-resources tutorial
 """
 
 import sys
 
 from cylc.flow import LOG
 import cylc.flow.flags
-from cylc.flow.loggingutil import disable_timestamps
+from cylc.flow.loggingutil import set_timestamps
 from cylc.flow.option_parsers import CylcOptionParser as COP
 from cylc.flow.resources import get_resources, list_resources
 from cylc.flow.terminal import cli_function
 
 
 def get_option_parser():
     parser = COP(
@@ -71,12 +71,12 @@
 
     return parser
 
 
 @cli_function(get_option_parser)
 def main(parser, opts, resource=None, tgt_dir=None):
     if cylc.flow.flags.verbosity < 2:
-        disable_timestamps(LOG)
+        set_timestamps(LOG, False)
     if not resource or opts.list:
         list_resources()
         sys.exit(0)
     get_resources(resource, tgt_dir)
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/get_workflow_contact.py` & `cylc-flow-8.2.0/cylc/flow/scripts/get_workflow_contact.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/get_workflow_version.py` & `cylc-flow-8.2.0/cylc/flow/scripts/get_workflow_version.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/graph.py` & `cylc-flow-8.2.0/cylc/flow/scripts/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
             edges.add((task, namespace))
             nodes.add(task)
 
     return sorted(nodes), sorted(edges)
 
 
 def get_config(workflow_id: str, opts: 'Values', flow_file) -> WorkflowConfig:
-    """Return a WorkflowConfig object for the provided reg / path."""
+    """Return a WorkflowConfig object for the provided id_ / path."""
     template_vars = get_template_vars(opts)
     return WorkflowConfig(
         workflow_id, flow_file, opts, template_vars=template_vars
     )
 
 
 def format_graphviz(
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/hold.py` & `cylc-flow-8.2.0/cylc/flow/scripts/hold.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/install.py` & `cylc-flow-8.2.0/cylc/flow/scripts/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 The workflow can then be started, stopped, and targeted by name.
 
 Normal installation creates a numbered run directory
 "~/cylc-run/<workflow-name>/run<number>".
 
 If a SOURCE_NAME is supplied, Cylc will search for the workflow source in the
 list of directories given by "global.cylc[install]source dirs", and install
-the first match. The installed workflow name will be the same as SOURCE_NAME,
+the first match. The installed workflow ID will start with SOURCE_NAME,
 unless --workflow-name is used.
 
 If a PATH is supplied, Cylc will install the workflow from the source directory
 given by the path. Relative paths must start with "./" to avoid ambiguity with
 SOURCE_NAME (i.e. "foo/bar" will be interpreted as a source name, whereas
-"./foo/bar" will be interpreted as a path). The installed workflow name will
-be the basename of the path, unless --workflow-name is used.
+"./foo/bar" will be interpreted as a path). The installed workflow ID will
+start with the basename of the path, unless --workflow-name is used.
 
 If no argument is supplied, Cylc will install the workflow from the source
 in the current working directory.
 
 A "_cylc-install/source" symlink to the source directory will be created in
 "~/cylc-run/<workflow-name>". Any files or directories (excluding .git, .svn)
 from the source directory are copied to the new run directory. A ".service"
@@ -88,31 +88,32 @@
 
 from cylc.flow.scripts.scan import (
     get_pipe,
     _format_plain,
     FLOW_STATE_SYMBOLS,
     FLOW_STATE_CMAP
 )
-from cylc.flow import iter_entry_points
+from cylc.flow import LOG, iter_entry_points
 from cylc.flow.exceptions import PluginError, InputError
-from cylc.flow.loggingutil import CylcLogFormatter
+from cylc.flow.loggingutil import CylcLogFormatter, set_timestamps
 from cylc.flow.option_parsers import (
     CylcOptionParser as COP,
     OptionSettings,
     Options
 )
 from cylc.flow.pathutil import (
     EXPLICIT_RELATIVE_PATH_REGEX,
     expand_path,
     get_workflow_run_dir
 )
-from cylc.flow.workflow_files import (
+from cylc.flow.install import (
     install_workflow,
     parse_cli_sym_dirs,
-    search_install_source_dirs
+    search_install_source_dirs,
+    check_deprecation,
 )
 from cylc.flow.terminal import cli_function
 
 
 INSTALL_OPTIONS = [
     OptionSettings(
         ["--workflow-name", "-n"],
@@ -133,15 +134,15 @@
             " share/cycle directories. Enter"
             " an empty list '' to skip making localhost symlink dirs."),
         action="store",
         dest="symlink_dirs",
         sources={'install'},
     ),
     OptionSettings(
-        ["--run-name"],
+        ["--run-name", "-r"],
         help=(
             "Give the run a custom name instead of automatically"
             " numbering it."),
         action="store",
         metavar="RUN_NAME",
         default=None,
         dest="run_name",
@@ -260,40 +261,46 @@
 InstallOptions = Options(get_option_parser())
 
 
 @cli_function(get_option_parser)
 def main(
     _parser: COP,
     opts: 'Values',
-    reg: Optional[str] = None
+    id_: Optional[str] = None
 ) -> None:
     """CLI wrapper."""
-    install_cli(opts, reg)
+    install_cli(opts, id_)
 
 
 def install_cli(
     opts: 'Values',
-    reg: Optional[str] = None
+    id_: Optional[str] = None
 ) -> Tuple[str, str]:
     """Install workflow and scan for already-running instances."""
-    wf_name, wf_id = install(opts, reg)
+    wf_name, wf_id = install(opts, id_)
     asyncio.run(
         scan(wf_name, not opts.no_ping)
     )
     return wf_name, wf_id
 
 
 def install(
-    opts: 'Values', reg: Optional[str] = None
+    opts: 'Values', id_: Optional[str] = None
 ) -> Tuple[str, str]:
+    set_timestamps(LOG, opts.log_timestamp and opts.verbosity > 1)
     if opts.no_run_name and opts.run_name:
         raise InputError(
             "options --no-run-name and --run-name are mutually exclusive."
         )
-    source = get_source_location(reg)
+    source = get_source_location(id_)
+
+    # Check deprecation to allow plugins to have access to correct flags
+    # for compatibility mode:
+    check_deprecation(source)
+
     for entry_point in iter_entry_points(
         'cylc.pre_configure'
     ):
         try:
             entry_point.resolve()(srcdir=source, opts=opts)
         except Exception as exc:
             # NOTE: except Exception (purposefully vague)
@@ -332,8 +339,10 @@
             # this is to separate plugin from core Cylc errors
             raise PluginError(
                 'cylc.post_install',
                 entry_point.name,
                 exc
             ) from None
 
+    print(f'INSTALLED {workflow_id} from {source_dir}')
+
     return workflow_name, workflow_id
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/jobs_kill.py` & `cylc-flow-8.2.0/cylc/flow/scripts/jobs_kill.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/jobs_poll.py` & `cylc-flow-8.2.0/cylc/flow/scripts/jobs_poll.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/jobs_submit.py` & `cylc-flow-8.2.0/cylc/flow/scripts/jobs_submit.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/kill.py` & `cylc-flow-8.2.0/cylc/flow/scripts/kill.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/lint.py` & `cylc-flow-8.2.0/cylc/flow/scripts/lint.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,35 +27,207 @@
 Check .cylc and .rc files for code style, deprecated syntax and other issues.
 
 By default, suggestions are written to stdout.
 
 In-place mode ("-i, --inplace") writes suggestions into the file as comments.
 Commit to version control before using this, in case you want to back out.
 
+A non-zero return code will be returned if any issues are identified.
+This can be overridden by providing the "--exit-zero" flag.
+
 Configurations for Cylc lint can also be set in a pyproject.toml file.
 
 """
 from colorama import Fore
+import functools
 from optparse import Values
 from pathlib import Path
 import re
-import tomli
-from typing import Generator, Union
+import sys
+import shutil
+try:
+    # BACK COMPAT: tomli
+    #   Support for Python versions before tomllib was added to the
+    #   standard library.
+    # FROM: Python 3.7
+    # TO: Python: 3.10
+    from tomli import (
+        loads as toml_loads,
+        TOMLDecodeError,
+    )
+except ImportError:
+    from tomllib import (  # type: ignore[no-redef]
+        loads as toml_loads,
+        TOMLDecodeError,
+    )
+from typing import Callable, Dict, Iterator, List, Union
 
 from cylc.flow import LOG
 from cylc.flow.exceptions import CylcError
 from cylc.flow.option_parsers import (
     CylcOptionParser as COP,
     WORKFLOW_ID_OR_PATH_ARG_DOC
 )
 from cylc.flow.cfgspec.workflow import upg, SPEC
 from cylc.flow.id_cli import parse_id
 from cylc.flow.parsec.config import ParsecConfig
+from cylc.flow.scripts.cylc import DEAD_ENDS
 from cylc.flow.terminal import cli_function
 
+DEPRECATED_ENV_VARS = {
+    'CYLC_SUITE_HOST': 'CYLC_WORKFLOW_HOST',
+    'CYLC_SUITE_OWNER': 'CYLC_WORKFLOW_OWNER',
+    'CYLC_SUITE_SHARE_DIR': 'CYLC_WORKFLOW_SHARE_DIR',
+    'CYLC_SUITE_SHARE_PATH': 'CYLC_WORKFLOW_SHARE_PATH',
+    'CYLC_SUITE_NAME': 'CYLC_WORKFLOW_ID',
+    'CYLC_SUITE_LOG_DIR': 'CYLC_WORKFLOW_LOG_DIR',
+    'CYLC_SUITE_INITIAL_CYCLE_POINT': 'CYLC_WORKFLOW_INITIAL_CYCLE_POINT',
+    'CYLC_SUITE_INITIAL_CYCLE_TIME': 'CYLC_WORKFLOW_INITIAL_CYCLE_TIME',
+    'CYLC_SUITE_FINAL_CYCLE_POINT': 'CYLC_WORKFLOW_FINAL_CYCLE_POINT',
+    'CYLC_SUITE_FINAL_CYCLE_TIME': 'CYLC_WORKFLOW_FINAL_CYCLE_TIME',
+    'CYLC_SUITE_WORK_DIR': 'CYLC_WORKFLOW_WORK_DIR',
+    'CYLC_SUITE_UUID': 'CYLC_WORKFLOW_UUID',
+    'CYLC_SUITE_RUN_DIR': 'CYLC_WORKFLOW_RUN_DIR',
+}
+
+OBSOLETE_ENV_VARS = {
+    'CYLC_SUITE_DEF_PATH',
+    'CYLC_SUITE_DEF_PATH_ON_SUITE_HOST'
+}
+
+
+def check_jinja2_no_shebang(
+    line: str,
+    file: Path,
+    function: Callable,
+    jinja_shebang: bool = False,
+    **kwargs
+):
+    """Check ONLY top level workflow files for jinja without shebangs.
+
+    Examples:
+        >>> func = re.compile(r'{{').findall
+
+        >>> check_jinja2_no_shebang(
+        ... '{{FOO}}',
+        ... function=func, jinja_shebang=True, file=Path('foo.cylc'))
+        False
+
+        >>> check_jinja2_no_shebang(
+        ... '{{FOO}}',
+        ... function=func, jinja_shebang=False, file=Path('suite.rc'))
+        ['{{']
+    """
+    if (
+        jinja_shebang
+        or file.name not in {'flow.cylc', 'suite.rc'}
+    ):
+        return False
+    return function(line)
+
+
+def check_if_jinja2(
+    line: str,
+    jinja_shebang: bool,
+    function: Callable,
+    **kwargs
+):
+    """Run function if Jinja2 switched on.
+
+    Examples:
+        >>> func = re.compile('foo').findall
+
+        >>> check_if_jinja2('barfoo', jinja_shebang=False, function=func)
+        False
+
+        >>> check_if_jinja2('foofoo', jinja_shebang=True, function=func)
+        ['foo', 'foo']
+
+    """
+    if jinja_shebang:
+        return function(line)
+    return False
+
+
+def check_dead_ends(line: str) -> bool:
+    """Check for dead end cylc scripts as defined in cylc.flow.scripts.cylc
+
+    Examples:
+        # Context:
+        # [runtime]
+        #   [[task]]
+        #     script = \"\"\"
+
+        >>> check_dead_ends('        cylc check-software')
+        True
+
+        >>> check_dead_ends('        cylc log')
+        False
+    """
+    return any(
+        f'cylc {dead_end}' in line for dead_end in DEAD_ENDS
+    )
+
+
+def check_for_suicide_triggers(
+    line: str,
+    file: Path,
+    function: Callable,
+    **kwargs
+):
+    """Check for suicide triggers, if file is a .cylc file.
+
+    Examples:
+        >>> func = lambda line: line
+
+        # Suicide trigger in a *.cylc file:
+        >>> check_for_suicide_triggers(
+        ... 'x:fail => !y', function=func, file=Path('foo.cylc'))
+        'x:fail => !y'
+
+        # Suicide trigger in a suite.rc file:
+        >>> check_for_suicide_triggers(
+        ... 'x:fail => !y', function=func, file=Path('suite.rc'))
+        False
+    """
+    if file.name.endswith('.cylc'):
+        return function(line)
+    return False
+
+
+def check_for_deprecated_environment_variables(
+    line: str
+) -> Union[bool, dict]:
+    """Warn that environment variables with SUITE in are deprecated"""
+    vars_found = [
+        f'{k}: {v}' for k, v in DEPRECATED_ENV_VARS.items()
+        if k in line
+    ]
+
+    if len(vars_found) == 1:
+        return {'vars': vars_found}
+    elif vars_found:
+        return {'vars': '\n * ' + '\n * '.join(vars_found)}
+    return False
+
+
+def check_for_obsolete_environment_variables(line: str) -> List[str]:
+    """Warn that environment variables are obsolete.
+
+    Examples:
+
+        >>> this = check_for_obsolete_environment_variables
+        >>> this('CYLC_SUITE_DEF_PATH')
+        ['CYLC_SUITE_DEF_PATH']
+    """
+    return [i for i in OBSOLETE_ENV_VARS if i in line]
+
+
+FUNCTION = 'function'
+
 STYLE_GUIDE = (
     'https://cylc.github.io/cylc-doc/stable/html/workflow-design-guide/'
     'style-guide.html#'
 )
 URL_STUB = "https://cylc.github.io/cylc-doc/stable/html/7-to-8/"
 SECTION2 = r'\[\[\s*{}\s*\]\]'
 SECTION3 = r'\[\[\[\s*{}\s*\]\]\]'
@@ -80,138 +252,283 @@
     'rst': (
         'settings in ``[runtime][<namespace>][{}]`` have been moved to '
         '``[runtime][<namespace>]`` and ``global.cylc[platforms]'
         '[<platforms name>]``'
     )
 }
 JINJA2_FOUND_WITHOUT_SHEBANG = 'jinja2 found: no shebang (#!jinja2)'
-CHECKS_DESC = {'U': '7 to 8 upgrades', 'S': 'Style'}
+CHECKS_DESC = {
+    'U': '7 to 8 upgrades',
+    'A': 'Auto Generated 7 to 8 upgrades',
+    'S': 'Style'
+}
+LINE_LEN_NO = 'S012'
+# Checks Dictionary fields:
+# TODO: Consider making the checks an object.
+# Key: A unique reference number.
+# - short: A short description of the issue.
+# - url: A link to a fuller description.
+# - function: A function to use to run the check.
+# - fallback: A second function(The first function might want to call this?)
+# - kwargs: We want to pass a set of common kwargs to the check function.
+# - evaluate commented lines: Run this check on commented lines.
+# - rst: An rst description, for use in the Cylc docs.
 STYLE_CHECKS = {
-    re.compile(r'^\t'): {
+    "S001": {
         'short': 'Use multiple spaces, not tabs',
         'url': STYLE_GUIDE + 'tab-characters',
-        'index': 1
+        FUNCTION: re.compile(r'^\t').findall
     },
-    # Not a full test, but if a non section is not indented...
-    re.compile(r'^[^\{\[|\s]'): {
+    "S002": {
         'short': 'Item not indented.',
+        # Non-indented items should be sections:
         'url': STYLE_GUIDE + 'indentation',
-        'index': 2
+        FUNCTION: re.compile(r'^[^\{\[|\s]').findall
     },
-    #            [section]
-    re.compile(r'^\s+\[[^\[.]*\]'): {
+    "S003": {
         'short': 'Top level sections should not be indented.',
         'url': STYLE_GUIDE + 'indentation',
-        'index': 3
+        FUNCTION: re.compile(r'^\s+\[[^\[.]*\]').findall
     },
-    # 2 or 4 space indentation both seem reasonable:
-    re.compile(r'^(|\s|\s{2,3}|\s{5,})\[\[[^\[.]*\]\]'): {
+    "S004": {
         'short': (
             'Second level sections should be indented exactly '
             '4 spaces.'
         ),
         'url': STYLE_GUIDE + 'indentation',
-        'index': 4
+        FUNCTION: re.compile(r'^(|\s|\s{2,3}|\s{5,})\[\[[^\[.]*\]\]').findall
     },
-    re.compile(r'^(|\s{1,7}|\s{9,})\[\[\[[^\[.]*\]\]\]'): {
+    "S005": {
         'short': (
             'Third level sections should be indented exactly '
             '8 spaces.'
         ),
         'url': STYLE_GUIDE + 'indentation',
-        'index': 5
+        FUNCTION: re.compile(r'^(|\s{1,7}|\s{9,})\[\[\[[^\[.]*\]\]\]').findall
     },
-    re.compile(r'\s$'): {
+    "S006": {
         'short': 'trailing whitespace.',
         'url': STYLE_GUIDE + 'trailing-whitespace',
-        'index': 6
+        FUNCTION: re.compile(r'[ \t]$').findall
     },
-    # Look for families both from inherit=FAMILY and FAMILY:trigger-all/any
-    re.compile(r'(inherit\s*=\s*.*[a-z].*)|(\w[a-z]\w:\w+?-a(ll|ny))'): {
+    # Look for families both from inherit=FAMILY and FAMILY:trigger-all/any.
+    # Do not match inherit lines with `None` at the start.
+    "S007": {
         'short': 'Family name contains lowercase characters.',
         'url': STYLE_GUIDE + 'task-naming-conventions',
-        'index': 7
+        FUNCTION: re.compile(
+            r'''
+            # match all inherit statements
+            ^\s*inherit\s*=
+            # filtering out those which match only valid family names
+            (?!
+                \s*
+                # none, None and root are valid family names
+                # and `inherit =` or `inherit = # x` are valid too
+                (['"]?(none|None|root|\#.*|$)['"]?|
+                (
+                    # as are families named with capital letters
+                    [A-Z0-9_-]+
+                    # and optional quotes
+                    | [\'\"]
+                    # which may include Cylc parameters
+                    | (<[^>]+>)
+                    # or Jinja2
+                    | ({[{%].*[%}]})
+                    # or EmPy
+                    | (@[\[{\(]).*([\]\}\)])
+                )+
+                )
+                # this can be a comma separated list
+                (
+                \s*,\s*
+                # none, None and root are valid family names
+                (['"]?(none|None|root)['"]?|
+                    (
+                    # as are families named with capital letters
+                    [A-Z0-9_-]+
+                    # and optional quotes
+                    | [\'\"]
+                    # which may include Cylc parameters
+                    | (<[^>]+>)
+                    # or Jinja2
+                    | ({[{%].*[%}]})
+                    # or EmPy
+                    | (@[\[{\(]).*([\]\}\)])
+                    )+
+                )
+                )*
+                # allow trailing commas and whitespace
+                \s*,?\s*
+                # allow trailing comments
+                (\#.*)?
+                $
+            )
+            ''',
+            re.X
+        ).findall,
     },
-    re.compile(r'{[{%]'): {
+    "S008": {
         'short': JINJA2_FOUND_WITHOUT_SHEBANG,
         'url': '',
-        'index': 8
+        'kwargs': True,
+        FUNCTION: functools.partial(
+            check_jinja2_no_shebang,
+            function=re.compile(r'{[{%]').findall
+        )
     },
-    re.compile(r'platform\s*=\s*\$\(.*?\)'): {
+    "S009": {
         'short': 'Host Selection Script may be redundant with platform',
         'url': (
             'https://cylc.github.io/cylc-doc/stable/html/7-to-8/'
             'major-changes/platforms.html'
         ),
-        'index': 9
+        FUNCTION: re.compile(r'platform\s*=\s*\$\(.*?\)').findall,
     },
-    re.compile(r'platform\s*=\s*(`.*?`)'): {
+    "S010": {
         'short': 'Using backticks to invoke subshell is deprecated',
         'url': 'https://github.com/cylc/cylc-flow/issues/3825',
-        'index': 10
+        FUNCTION: re.compile(r'platform\s*=\s*(`.*?`)').findall,
     },
-    re.compile(r'#.*?{[{%]'): {
+    "S011": {
         'short': 'Cylc will process commented Jinja2!',
         'url': '',
-        'index': 11
+        'kwargs': True,
+        'evaluate commented lines': True,
+        FUNCTION: functools.partial(
+            check_if_jinja2,
+            function=re.compile(r'(?<!{)#.*?{[{%]').findall
+        )
     }
-    # re.compile(r'^.{{maxlen},}'): {
-    #     'short': 'line > {maxlen} characters.',
-    #     'url': STYLE_GUIDE + 'line-length-and-continuation',
-    #     'index': 8
-    # },
 }
 # Subset of deprecations which are tricky (impossible?) to scrape from the
 # upgrader.
 MANUAL_DEPRECATIONS = {
-    re.compile(SECTION2.format('dependencies')): {
+    "U001": {
         'short': DEPENDENCY_SECTION_MSG['text'],
         'url': '',
-        'rst': DEPENDENCY_SECTION_MSG['rst']
+        'rst': DEPENDENCY_SECTION_MSG['rst'],
+        FUNCTION: re.compile(SECTION2.format('dependencies')).findall,
     },
-    re.compile(r'graph\s*=\s*'): {
+    "U002": {
         'short': DEPENDENCY_SECTION_MSG['text'],
         'url': '',
-        'rst': DEPENDENCY_SECTION_MSG['rst']
+        'rst': DEPENDENCY_SECTION_MSG['rst'],
+        FUNCTION: re.compile(r'graph\s*=\s*').findall,
     },
-    re.compile(SECTION3.format('remote')): {
+    "U003": {
         'short': JOBANDREMOTE_SECTION_MSG['text'].format('remote'),
         'url': '',
-        'rst': JOBANDREMOTE_SECTION_MSG['rst'].format('remote')
+        'rst': JOBANDREMOTE_SECTION_MSG['rst'].format('remote'),
+        FUNCTION: re.compile(SECTION3.format('remote')).findall
     },
-    re.compile(SECTION3.format('job')): {
+    "U004": {
         'short': JOBANDREMOTE_SECTION_MSG['text'].format('job'),
         'url': '',
-        'rst': JOBANDREMOTE_SECTION_MSG['rst'].format('job')
+        'rst': JOBANDREMOTE_SECTION_MSG['rst'].format('job'),
+        FUNCTION: re.compile(SECTION3.format('job')).findall,
     },
-    re.compile(r'batch system\s*=\s*'): {
+    "U005": {
         'short': (
             'flow.cylc[runtime][<namespace>][job]batch system -> '
             'global.cylc[platforms][<platform name>]job runner'
         ),
         'url': '',
         'rst': (
             '``flow.cylc[runtime][<namespace>][job]batch system`` -> '
             '``global.cylc[platforms][<platform name>]job runner``'
-        )
+        ),
+        FUNCTION: re.compile(r'batch system\s*=\s*').findall,
     },
-    re.compile(r'host\s*=\s*(`.*?`)'): {
+    "U006": {
         'short': 'Using backticks to invoke subshell will fail at Cylc 8.',
-        'url': 'https://github.com/cylc/cylc-flow/issues/3825'
+        'url': 'https://github.com/cylc/cylc-flow/issues/3825',
+        FUNCTION: re.compile(r'host\s*=\s*(`.*?`)').findall,
+    },
+    'U007': {
+        'short': (
+            'Use built in platform selection instead of rose host-select.'),
+        'url': (
+            'https://cylc.github.io/cylc-doc/stable/html/7-to-8/'
+            'major-changes/platforms.html'),
+        FUNCTION: re.compile(r'platform\s*=\s*\$\(\s*rose host-select').findall
+    },
+    'U008': {
+        'short': 'Suicide triggers are not required at Cylc 8.',
+        'url': '',
+        'kwargs': True,
+        FUNCTION: functools.partial(
+            check_for_suicide_triggers,
+            function=re.compile(r'=>\s*\!.*').findall
+        ),
+    },
+    'U009': {
+        'short': 'This line contains an obsolete Cylc CLI command.',
+        'url': '',
+        FUNCTION: check_dead_ends
+    },
+    'U010': {
+        'short': 'rose suite-hook is deprecated at Rose 2,',
+        'url': (
+            'https://cylc.github.io/cylc-doc/stable/html/7-to-8'
+            '/major-changes/suicide-triggers.html'),
+        FUNCTION: lambda line: 'rose suite-hook' in line,
+    },
+    'U011': {
+        'short': 'Leading zeros are no longer valid for Jinja2 integers.',
+        'url': (
+            'https://cylc.github.io/cylc-doc/stable/html/7-to-8/major-changes'
+            '/python-2-3.html#jinja2-integers-with-leading-zeros'),
+        'kwargs': True,
+        FUNCTION: functools.partial(
+            check_if_jinja2,
+            function=re.compile(r'\{%\s*set\s*.+?\s*=\s*0\d+\s*%\}').findall
+        )
+    },
+    'U012': {
+        'short': (
+            'Deprecated environment variables: {vars}'),
+        'rst': (
+            'The following environment variables are deprecated:\n\n'
+            '.. list-table::'
+            '\n   :header-rows: 1'
+            '\n\n   * - Deprecated Variable'
+            '\n     - New Variable'
+        ) + ''.join(
+            [
+                f'\n   * - ``{old}``\n     - ``{new}``'
+                for old, new in DEPRECATED_ENV_VARS.items()
+            ]
+        ),
+        'url': (
+            'https://cylc.github.io/cylc-doc/stable/html/reference/'
+            'job-script-vars/index.html'
+        ),
+        FUNCTION: check_for_deprecated_environment_variables,
+    },
+    'U013': {
+        'short': (
+            'Obsolete environment variables: {vars}'),
+        'rst': (
+            'The following environment variables are obsolete:\n\n'
+            + ''.join([f'\n * ``{old}``' for old in OBSOLETE_ENV_VARS])
+        ),
+        'url': (
+            'https://cylc.github.io/cylc-doc/stable/html/reference/'
+            'job-script-vars/index.html'
+        ),
+        FUNCTION: check_for_obsolete_environment_variables,
     }
 }
 RULESETS = ['728', 'style', 'all']
 EXTRA_TOML_VALIDATION = {
     'ignore': {
         lambda x: re.match(r'[A-Z]\d\d\d', x):
             '{item} not valid: Ignore codes should be in the form X001',
-        lambda x: x in [
-            f'{i["purpose"]}{i["index"]:03d}'
-            for i in parse_checks(['728', 'style']).values()
-        ]:
+        lambda x: x in parse_checks(['728', 'style']):
             '{item} is a not a known linter code.'
     },
     'rulesets': {
         lambda item: item in RULESETS:
             '{item} not valid: Rulesets can be '
             '\'728\', \'style\' or \'all\'.'
     },
@@ -264,16 +581,16 @@
     """if a pyproject.toml file is present open it and return settings.
     """
     keys = ['rulesets', 'ignore', 'exclude', 'max-line-length']
     tomlfile = Path(dir_ / 'pyproject.toml')
     tomldata = {}
     if tomlfile.is_file():
         try:
-            loadeddata = tomli.loads(tomlfile.read_text())
-        except tomli.TOMLDecodeError as exc:
+            loadeddata = toml_loads(tomlfile.read_text())
+        except TOMLDecodeError as exc:
             raise CylcError(f'pyproject.toml did not load: {exc}')
 
         if any(
             i in loadeddata for i in ['cylc-lint', 'cylclint', 'cylc_lint']
         ):
             for key in keys:
                 tomldata[key] = loadeddata.get('cylc-lint').get(key, [])
@@ -367,60 +684,63 @@
 
 def get_upgrader_info():
     """Extract info about obseletions and deprecations from Parsec Objects."""
     conf = ParsecConfig(SPEC, upg)
     upgrades = conf.upgrader(conf.dense, '').upgrades
     deprecations = {}
 
-    for _, upgrades_for_version in upgrades.items():
-        for upgrade in upgrades_for_version:
+    for upgrades_for_version in upgrades.values():
+        for index, upgrade in enumerate(upgrades_for_version):
             # Set a flag indicating that a variable has been moved.
+            is_dep, is_obs = False, False
             if upgrade['new'] is None:
                 section_name = list_to_config(
                     upgrade["old"], upgrade["is_section"])
                 short = f'{section_name} - not available at Cylc 8'
                 rst = f'``{section_name}`` is not available at Cylc 8'
+                is_obs = True
             elif upgrade["old"][-1] == upgrade['new'][-1]:
                 # Where an item with the same name has been moved
                 # a 1 line regex isn't going to work.
                 continue
             else:
                 old = list_to_config(
                     upgrade["old"], upgrade["is_section"])
                 new = list_to_config(
                     upgrade["new"], upgrade["is_section"])
                 short = f'{old} -> {new}'
                 rst = f'``{old}`` is now ``{new}``'
+                is_dep = True
 
             # Check whether upgrade is section:
             if upgrade['is_section'] is True:
                 section_depth = len(upgrade['old'])
                 start = r'\[' * section_depth
                 end = r'\]' * section_depth
                 name = upgrade["old"][-1]
-                regex = re.compile(fr'{start}\s*{name}\s*{end}\s*$')
+                expr = fr'{start}\s*{name}\s*{end}\s*$'
             else:
                 name = upgrade["old"][-1]
                 expr = rf'^\s*{name}\s*=\s*.*'
-                regex = re.compile(expr)
 
-            deprecations[regex] = {
+            deprecations[f'A{index:03d}'] = {
                 'short': short,
                 'url': '',
                 'rst': rst,
+                FUNCTION: re.compile(expr).findall,
+                'is_obs': is_obs,
+                'is_dep': is_dep,
             }
-    # Some deprecations are not specified in a straightforward to scrape
-    # way and these are specified in MANUAL_DEPRECATIONS:
-    deprecations.update(MANUAL_DEPRECATIONS)
+
     return deprecations
 
 
 PURPOSE_FILTER_MAP = {
     'style': 'S',
-    '728': 'U',
+    '728': 'UA',
 }
 
 
 def parse_checks(check_args, ignores=None, max_line_len=None, reference=False):
     """Prepare dictionary of checks.
 
     Args:
@@ -431,108 +751,197 @@
             this. (If None, rule not enforced)
         reference: Function is being used to get a reference. If true
             max-line-length will have a generic message, rather than
             using any specific value.
     """
     ignores = ignores or []
     parsedchecks = {}
-    purpose_filters = [PURPOSE_FILTER_MAP[i] for i in check_args]
-
-    checks = {'U': get_upgrader_info(), 'S': STYLE_CHECKS}
-
+    purpose_filters = [
+        purpose
+        for arg in check_args
+        for purpose in PURPOSE_FILTER_MAP[arg]
+    ]
+
+    checks = {
+        'S': STYLE_CHECKS,
+        'U': MANUAL_DEPRECATIONS,
+        'A': get_upgrader_info(),
+    }
     for purpose, ruleset in checks.items():
         if purpose in purpose_filters:
             # Run through the rest of the config items.
-            for index, (pattern, meta) in enumerate(ruleset.items(), start=1):
+            for index, meta in ruleset.items():
                 meta.update({'purpose': purpose})
-                if 'index' not in meta:
-                    meta.update({'index': index})
-                if f'{purpose}{index:03d}' not in ignores:
-                    parsedchecks.update({pattern: meta})
-            if 'S' in purpose and "S008" not in ignores:
+                if f'{index}' not in ignores:
+                    parsedchecks.update({index: meta})
+            if 'S' in purpose and LINE_LEN_NO not in ignores:
+                # Special handling for max line length:
                 if not max_line_len:
                     max_line_len = 130
                 regex = r"^.{" + str(max_line_len) + r"}"
                 if reference:
                     msg = (
                         'line > ``<max_line_len>`` characters. Max line '
                         ' length set in pyproject.toml (default 130)'
                     )
                 else:
                     msg = f'line > {max_line_len} characters.'
-                parsedchecks[re.compile(regex)] = {
+                parsedchecks[LINE_LEN_NO] = {
                     'short': msg,
                     'url': STYLE_GUIDE + 'line-length-and-continuation',
-                    'index': 8,
+                    FUNCTION: re.compile(regex).findall,
                     'purpose': 'S'
                 }
     return parsedchecks
 
 
+def get_index_str(meta: dict, index: str) -> str:
+    """Printable purpose string - mask useless numbers for auto-generated
+    upgrades."""
+    if meta.get('is_dep', None):
+        return 'U998'
+    elif meta.get('is_obs', None):
+        return 'U999'
+    else:
+        return f'{index}'
+
+
 def check_cylc_file(
-    dir_, file_, checks,
-    modify=False,
+    file: Path,
+    file_rel: Path,
+    checks: Dict[str, dict],
+    counter: Dict[str, int],
+    modify: bool = False,
 ):
     """Check A Cylc File for Cylc 7 Config"""
-    file_rel = file_.relative_to(dir_)
-    # Set mode as read-write or read only.
-    outlines = []
-
-    # Open file, and read it's line to memory.
-    lines = file_.read_text().split('\n')
-    jinja_shebang = lines[0].strip().lower() == JINJA2_SHEBANG
-    count = 0
-    for line_no, line in enumerate(lines, start=1):
-        for check, message in checks.items():
-            # Tests with for presence of Jinja2 if no shebang line is
-            # present.
+    with open(file, 'r') as cylc_file:
+        # generator which reads and lints one line at a time
+        linter = lint(
+            file_rel,
+            cylc_file,
+            checks,
+            counter,
+            modify,
+        )
+
+        if modify:
+            # write modifications into a ".temp" file
+            modify_file_path = file.parent / f'{file.name}.temp'
+            with open(modify_file_path, 'w+') as modify_file:
+                for line in linter:
+                    modify_file.write(line)
+            # replace the original with the ".temp" file
+            shutil.move(str(modify_file_path), file)
+        else:
+            for _line in linter:
+                pass
+
+
+def lint(
+    file_rel: Path,
+    lines: Iterator[str],
+    checks: Dict[str, dict],
+    counter: Dict[str, int],
+    modify: bool = False,
+    write: Callable = print
+) -> Iterator[str]:
+    """Lint text, one line at a time.
+
+    Arguments:
+        file_rel:
+            The filepath relative to the workflow configuration directory
+            (used in messages).
+        lines:
+            Iterator which produces one line of text at a time
+            e.g. open(file) or iter(['foo\n', 'bar\n', 'baz\n'].
+        counter:
+            Dictionary for counting lint hits per category.
+        modify:
+            If True, this generator will yield the file one line at a time
+            with comments inserted to help users fix their lint.
+        write:
+            A function for reporting lint messages.
+
+    Yields:
+        The original file with added comments when `modify is True`.
+
+    """
+    # get the first line
+    line_no = 1
+    line = next(lines)
+    # check if it is a jinja2 shebang
+    jinja_shebang = line.strip().lower() == JINJA2_SHEBANG
+
+    while True:
+        # run lint checks against the current line
+        for index, check_meta in checks.items():
+            # Skip commented line unless check says not to.
             if (
-                jinja_shebang
-                and message['short'].startswith(
-                    JINJA2_FOUND_WITHOUT_SHEBANG)
+                line.strip().startswith('#')
+                and not check_meta.get('evaluate commented lines', False)
             ):
                 continue
 
-            if (
-                check.findall(line)
-                and (
-                    not line.strip().startswith('#')
-                    or (
-                        'commented Jinja2!' in message['short']
-                        and check.findall(line)
-                    )
+            if check_meta.get('kwargs', False):
+                # Use a more complex function with keywords:
+                check_function = functools.partial(
+                    check_meta['function'],
+                    check_meta=check_meta,
+                    file=file_rel,
+                    jinja_shebang=jinja_shebang,
                 )
-            ):
-                count += 1
+            else:
+                # Just going to pass the line to the check function:
+                check_function = check_meta['function']
+
+            # Run the check:
+            check = check_function(line)
+
+            if check:
+                # we have lint!
+                if isinstance(check, dict):
+                    msg = check_meta['short'].format(**check)
+                else:
+                    msg = check_meta['short']
+                counter.setdefault(check_meta['purpose'], 0)
+                counter[check_meta['purpose']] += 1
                 if modify:
-                    if message['url'].startswith('http'):
-                        url = message['url']
+                    # insert a command to help the user
+                    if check_meta['url'].startswith('http'):
+                        url = check_meta['url']
                     else:
-                        url = URL_STUB + message['url']
-                    outlines.append(
-                        f'# [{message["purpose"]}{message["index"]:03d}]: '
-                        f'{message["short"]}\n'
-                        f'# - see {url}'
+                        url = URL_STUB + check_meta['url']
+
+                    yield (
+                        f'# [{get_index_str(check_meta, index)}]: '
+                        f'{msg}\n'
+                        f'# - see {url}\n'
                     )
                 else:
-                    print(
+                    # write a message to inform the user
+                    write(
                         Fore.YELLOW +
-                        f'[{message["purpose"]}{message["index"]:03d}]'
-                        f' {file_rel}:{line_no}: {message["short"]}'
+                        f'[{get_index_str(check_meta, index)}]'
+                        f' {file_rel}:{line_no}: {msg}'
                     )
         if modify:
-            outlines.append(line)
-    if modify:
-        file_.write_text('\n'.join(outlines))
-    return count
+            yield line
+
+        try:
+            # get the next line
+            line = next(lines)
+        except StopIteration:
+            # end of interator
+            return
+        line_no += 1
 
 
 def get_cylc_files(
     base: Path, exclusions: Union[list, None] = None
-) -> Generator[Path, None, None]:
+) -> Iterator[Path]:
     """Given a directory yield paths to check."""
     exclusions = [] if exclusions is None else exclusions
     except_these_files = [
         file for exclusion in exclusions for file in base.rglob(exclusion)]
     for rglob in FILEGLOBS:
         for path in base.rglob(rglob):
             # Exclude log directory:
@@ -547,87 +956,103 @@
     """Print a reference for checks to be carried out.
 
     Returns:
         RST compatible text.
     """
     output = ''
     current_checkset = ''
-    for check, meta in checks.items():
+    for index, meta in checks.items():
         # Check if the purpose has changed - if so create a new
         # section title:
         if meta['purpose'] != current_checkset:
             current_checkset = meta['purpose']
             title = CHECKS_DESC[meta["purpose"]]
             output += f'\n{title}\n{"-" * len(title)}\n\n'
 
-        # Fill a template with info about the issue.
-        template = (
-            '{checkset}{index:003d}\n^^^^\n{summary}\n\n'
-        )
-        if meta['url'].startswith('http'):
-            url = meta['url']
+            if current_checkset == 'A':
+                output += (
+                    '\n.. note::\n'
+                    '\n   U998 and U999 represent automatically generated '
+                    'sets of deprecations and upgrades.\n\n'
+                )
+
+        if current_checkset == 'A':
+            summary = meta.get("rst", meta['short'])
+            output += '\n- ' + summary
         else:
-            url = URL_STUB + meta['url']
-        summary = meta.get("rst", meta['short'])
-        msg = template.format(
-            title=check.pattern.replace('\\', ''),
-            checkset=meta['purpose'],
-            summary=summary,
-            url=url,
-            index=meta['index'],
-        )
-        output += msg
+            # Fill a template with info about the issue.
+            template = (
+                '{check}\n^^^^\n{summary}\n\n'
+            )
+            if meta['url'].startswith('http'):
+                url = meta['url']
+            else:
+                url = URL_STUB + meta['url']
+            summary = meta.get("rst", meta['short'])
+            msg = template.format(
+                check=get_index_str(meta, index),
+                summary=summary,
+                url=url,
+            )
+            output += msg
     output += '\n'
     return output
 
 
 def get_reference_text(checks):
     """Print a reference for checks to be carried out.
 
     Returns:
         RST compatible text.
     """
     output = ''
     current_checkset = ''
-    for check, meta in checks.items():
+    for index, meta in checks.items():
         # Check if the purpose has changed - if so create a new
         # section title:
         if meta['purpose'] != current_checkset:
             current_checkset = meta['purpose']
             title = CHECKS_DESC[meta["purpose"]]
             output += f'\n{title}\n{"-" * len(title)}\n\n'
 
+            if current_checkset == 'A':
+                output += (
+                    'U998 and U999 represent automatically generated'
+                    ' sets of deprecations and upgrades.'
+                )
         # Fill a template with info about the issue.
-        template = (
-            '{checkset}{index:003d}:\n    {summary}\n\n'
-        )
-        if meta['url'].startswith('http'):
-            url = meta['url']
+        if current_checkset == 'A':
+            summary = meta.get("rst", meta['short']).replace('``', '')
+            output += '\n* ' + summary
         else:
-            url = URL_STUB + meta['url']
-        msg = template.format(
-            title=check.pattern.replace('\\', ''),
-            checkset=meta['purpose'],
-            summary=meta['short'],
-            url=url,
-            index=meta['index'],
-        )
-        output += msg
+            template = (
+                '{check}:\n    {summary}\n\n'
+            )
+            if meta['url'].startswith('http'):
+                url = meta['url']
+            else:
+                url = URL_STUB + meta['url']
+            msg = template.format(
+                title=index,
+                check=get_index_str(meta, index),
+                summary=meta['short'],
+                url=url,
+            )
+            output += msg
     output += '\n'
     return output
 
 
 def get_option_parser() -> COP:
     parser = COP(
         COP_DOC,
         argdoc=[
             COP.optional(WORKFLOW_ID_OR_PATH_ARG_DOC)
         ],
     )
-
     parser.add_option(
         '--inplace', '-i',
         help=(
             'Modify files in place, adding comments to files. '
             'If not set, the script will work as a linter'
         ),
         action='store_true',
@@ -657,44 +1082,50 @@
         help=(
             'Ignore this check number.'
         ),
         action='append',
         default=[],
         dest='ignores',
         metavar="CODE",
-        choices=tuple([f'S{i["index"]:03d}' for i in STYLE_CHECKS.values()])
+        choices=tuple(STYLE_CHECKS)
+    )
+    parser.add_option(
+        '--exit-zero',
+        help='Exit with status code "0" even if there are issues.',
+        action='store_true',
+        default=False,
+        dest='exit_zero'
     )
 
     return parser
 
 
 @cli_function(get_option_parser)
 def main(parser: COP, options: 'Values', target=None) -> None:
     if options.ref_mode:
         if options.linter in {'all', ''}:
             rulesets = ['728', 'style']
         else:
             rulesets = [options.linter]
         print(get_reference_text(parse_checks(rulesets, reference=True)))
-        exit(0)
+        sys.exit(0)
 
     # If target not given assume we are looking at PWD
     if target is None:
         target = str(Path.cwd())
 
     # make sure the target is a src/run directories
     _, _, target = parse_id(
         target,
         src=True,
         constraint='workflows',
     )
 
     # Get a list of checks bas ed on the checking options:
     # Allow us to check any number of folders at once
-    count = 0
     target = target.parent
     ruleset_default = False
     if options.linter == 'all':
         options.linter = ['728', 'style']
     elif options.linter == '':
         options.linter = ['728', 'style']
         ruleset_default = True
@@ -717,49 +1148,60 @@
     cylc8 = (target / 'flow.cylc').exists()
     if not cylc8 and mergedopts['rulesets'] == ['728']:
         LOG.error(
             f'{target} not a Cylc 8 workflow: '
             'Lint after renaming '
             '"suite.rc" to "flow.cylc"'
         )
-        exit(0)
+        # Exit with an error code if --exit-zero was not set.
+        # Return codes: sys.exit(True) == 1, sys.exit(False) == 0
+        sys.exit(not options.exit_zero)
     elif not cylc8 and '728' in mergedopts['rulesets']:
         check_names = mergedopts['rulesets']
         check_names.remove('728')
     else:
         check_names = mergedopts['rulesets']
 
     # Check each file:
     checks = parse_checks(
         check_names,
         ignores=mergedopts['ignore'],
         max_line_len=mergedopts['max-line-length']
     )
-    for file_ in get_cylc_files(target, mergedopts['exclude']):
-        LOG.debug(f'Checking {file_}')
-        count += check_cylc_file(
-            target,
-            file_,
+
+    counter: Dict[str, int] = {}
+    for file in get_cylc_files(target, mergedopts['exclude']):
+        LOG.debug(f'Checking {file}')
+        check_cylc_file(
+            file,
+            file.relative_to(target),
             checks,
+            counter,
             options.inplace,
         )
 
-    if count > 0:
+    if counter:
+        total_lint_hits = sum(counter.values())
         msg = (
             f'\n{Fore.YELLOW}'
             f'Checked {target} against {check_names} '
-            f'rules and found {count} issue'
-            f'{"s" if count > 1 else ""}.'
+            f'rules and found {total_lint_hits} issue'
+            f'{"s" if total_lint_hits > 1 else ""}.'
         )
     else:
         msg = (
             f'{Fore.GREEN}'
             f'Checked {target} against {check_names} rules and '
             'found no issues.'
         )
 
     print(msg)
 
+    # Exit with an error code if there were warnings and
+    # if --exit-zero was not set.
+    # Return codes: sys.exit(True) == 1, sys.exit(False) == 0
+    sys.exit(bool(counter) and not options.exit_zero)
+
 
 # NOTE: use += so that this works with __import__
 # (docstring needed for `cylc help all` output)
 __doc__ += get_reference_rst(parse_checks(['728', 'style'], reference=True))
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/list.py` & `cylc-flow-8.2.0/cylc/flow/scripts/list.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/message.py` & `cylc-flow-8.2.0/cylc/flow/scripts/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 Note:
   To abort a job script with a custom error message, use cylc__job_abort:
     cylc__job_abort 'message...'
   (For technical reasons this is a shell function, not a cylc sub-command).
 
 For backward compatibility, if number of arguments is less than or equal to 2,
 the command assumes the classic interface, where all arguments are messages.
-Otherwise, the first 2 arguments are assumed to be workflow name and job
+Otherwise, the first 2 arguments are assumed to be workflow ID and job
 identifier.
 """
 
 
 from logging import getLevelName, INFO
 import os
 import sys
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/pause.py` & `cylc-flow-8.2.0/cylc/flow/scripts/pause.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/ping.py` & `cylc-flow-8.2.0/cylc/flow/scripts/ping.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/play.py` & `cylc-flow-8.2.0/cylc/flow/scripts/play.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/poll.py` & `cylc-flow-8.2.0/cylc/flow/scripts/poll.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/psutil.py` & `cylc-flow-8.2.0/cylc/flow/scripts/psutil.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/reinstall.py` & `cylc-flow-8.2.0/cylc/flow/scripts/reinstall.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,26 +76,27 @@
 
 from cylc.flow import iter_entry_points
 from cylc.flow.exceptions import (
     PluginError,
     ServiceFileError,
     WorkflowFilesError,
 )
+from cylc.flow.install import (
+    reinstall_workflow,
+)
 from cylc.flow.id_cli import parse_id
 from cylc.flow.option_parsers import (
     CylcOptionParser as COP,
     OptionSettings,
-    Options,
     WORKFLOW_ID_ARG_DOC,
 )
 from cylc.flow.pathutil import get_workflow_run_dir
 from cylc.flow.workflow_files import (
     get_workflow_source_dir,
     load_contact_file,
-    reinstall_workflow,
 )
 from cylc.flow.terminal import cli_function, DIM, is_terminal
 
 if TYPE_CHECKING:
     from optparse import Values
 
 _input = input  # to enable testing
@@ -108,33 +109,44 @@
         action='store_true',
         default=False,
         dest="clear_rose_install_opts",
         sources={'reinstall'}
     )
 ]
 
+REINSTALL_OPTIONS = [
+    OptionSettings(
+        ["--yes"],
+        help='Skip interactive prompts.',
+        action="store_true",
+        default=False,
+        dest="skip_interactive",
+        sources={'reinstall'}
+    ),
+]
+
 
 def get_option_parser() -> COP:
     parser = COP(
         __doc__, comms=True, argdoc=[WORKFLOW_ID_ARG_DOC]
     )
 
-    parser.add_cylc_rose_options()
     try:
         # If cylc-rose plugin is available
         __import__('cylc.rose')
     except ImportError:
-        pass
+        options = REINSTALL_OPTIONS
     else:
-        for option in REINSTALL_CYLC_ROSE_OPTIONS:
-            parser.add_option(*option.args, **option.kwargs)
-    return parser
+        parser.add_cylc_rose_options()
+        options = REINSTALL_CYLC_ROSE_OPTIONS + REINSTALL_OPTIONS
 
+    for option in options:
+        parser.add_option(*option.args, **option.kwargs)
 
-ReInstallOptions = Options(get_option_parser())
+    return parser
 
 
 @cli_function(get_option_parser)
 def main(
     _parser: COP,
     opts: 'Values',
     args: Optional[str] = None
@@ -142,14 +154,15 @@
     """CLI wrapper."""
     reinstall_cli(opts, args)
 
 
 def reinstall_cli(
     opts: 'Values',
     args: Optional[str] = None,
+    print_reload_tip: bool = True,
 ) -> bool:
     """Implement cylc reinstall.
 
     This is the bit which contains all the CLI logic.
     """
     run_dir: Optional[Path]
     workflow_id: str
@@ -171,15 +184,16 @@
             f'Workflow source dir is not accessible: "{source}".\n'
             f'Restore the source or modify the "{source_symlink}"'
             ' symlink to continue.'
         )
 
     usr: str = ''
     try:
-        if is_terminal():  # interactive mode - perform dry-run and prompt
+        if is_terminal() and not opts.skip_interactive:
+            # interactive mode - perform dry-run and prompt
             # dry-mode reinstall
             if not reinstall(
                 opts,
                 workflow_id,
                 source,
                 run_dir,
                 dry_run=True,
@@ -208,15 +222,16 @@
         usr = 'n'  # cancel the reinstall
         print()    # clear the traceback line
 
     if usr == 'y':
         # reinstall for real
         reinstall(opts, workflow_id, source, run_dir, dry_run=False)
         print(cparse('<green>Successfully reinstalled.</green>'))
-        display_cylc_reload_tip(workflow_id)
+        if print_reload_tip:
+            display_cylc_reload_tip(workflow_id)
         return True
 
     else:
         # no reinstall
         print(
             cparse('<magenta>Reinstall canceled, no changes made.</magenta>')
         )
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/release.py` & `cylc-flow-8.2.0/cylc/flow/scripts/release.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/reload.py` & `cylc-flow-8.2.0/cylc/flow/scripts/reload.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/remote_init.py` & `cylc-flow-8.2.0/cylc/flow/scripts/remote_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """cylc remote-init [OPTIONS] ARGS
 
 (This command is for internal use.)
 
 Initialise an install target.
 
 Initialisation creates a workflow run directory on the install target,
-"$HOME/cylc-run/<WORKFLOW_NAME>/". The .service directory is also created and
+"$HOME/cylc-run/<WORKFLOW_ID>/". The .service directory is also created and
 populated with the install target authentication files and the contact file.
 
 Symlinks are created for run, work, share, share/cycle, log directories,
 configured in the global.flow.
 
 Return:
     0:
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/remote_tidy.py` & `cylc-flow-8.2.0/cylc/flow/scripts/remote_tidy.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/remove.py` & `cylc-flow-8.2.0/cylc/flow/scripts/remove.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/report_timings.py` & `cylc-flow-8.2.0/cylc/flow/scripts/report_timings.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/scan.py` & `cylc-flow-8.2.0/cylc/flow/scripts/scan.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,43 +13,48 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """cylc scan [OPTIONS]
 
-List Cylc workflows.
+List your source, and/or installed, and/or running workflows.
 
-By default this shows only running or paused workflows.
+By default, running workflows are listed as indicated by the presence of
+scheduler contact files, ~/cylc-run/<Workflow-ID>/.service/contact.
+
+With "--ping" or "-t rich", attempt to contact the schedulers. If any are not
+found to be running, their contact files will be removed (these files may left
+behind if the scheduler did not shut down cleanly).
 
 Examples:
-  # list all "active" workflows (i.e. running or paused)
+  # list all active workflows (i.e. running or paused)
   $ cylc scan
 
-  # show more information about these workflows
+  # show more information about active workflows
   $ cylc scan -t rich
 
   # don't rely on colour for job state totals
   $ cylc scan -t rich --colour-blind
 
-  # list all "inactive" workflows (i.e. registered or stopped)
+  # list workflows that are installed but stopped or not run yet
   $ cylc scan --state stopped
 
   # list all workflows (active or inactive)
   $ cylc scan --state=running,paused,stopped
   $ cylc scan --state=all  # or using the shorthand
 
   # filter workflows by name
   $ cylc scan --name '^f.*'  # show only flows starting with "f"
 
-  # list source workflows in a tree
+  # list source workflows in tree format
   # (looks in the dirs configured by "global.cylc[install]source dirs")
   $ cylc scan --source -t tree
 
-  # get results in JSON format
+  # print contact file data in JSON format
   $ cylc scan -t json
 """
 
 import asyncio
 import json
 from pathlib import Path
 from typing import Callable, Optional, TYPE_CHECKING
@@ -200,20 +205,20 @@
         default=False,
         action='store_true'
     )
 
     parser.add_option(
         '--format', '-t',
         help=(
-            'Set the output format.'
-            ' (rich: multi-line, human readable)'
-            ' (plain: single-line)'
-            ' (json: machine readable)'
-            ' (tree: display registration hierarchy as a tree)'
-            ' (name: just show flow names, machine readable)'
+            'Output data and format (default "plain").'
+            ' ("name": list the workflow IDs only)'
+            ' ("plain": name,host:port,PID on one line)'
+            ' ("tree": name,host:port,PID in tree format)'
+            ' ("json": full contact data in JSON format)'
+            ' ("rich": include task state summary data)'
         ),
         choices=('rich', 'plain', 'json', 'tree', 'name'),
         default='plain'
     )
 
     parser.add_option(
         '--sort',
@@ -221,27 +226,25 @@
         action='store_true'
     )
 
     parser.add_option(
         '--colour-blind', '--color-blind',
         help=(
             "Don't depend on colour to convey information. "
-            ' Use this rather than --color=never so you still get bold text.'
+            'Use this rather than --color=never so you still get bold text.'
         ),
         action='store_true'
     )
 
     parser.add_option(
         '--ping',
         help=(
-            'Test the connection to the flow. Scan normally just reads flow'
-            ' contact files, but --ping forces a connection to the scheduler'
-            ' and removes the contact file if it is not found to be running'
-            " (this can happen if the scheduler gets killed and can't clean"
-            ' up after itself).'
+            "Connect to schedulers and remove contact files if they are not "
+            "found to be running. Contact files can be left behind when "
+            "schedulers get killed."
         ),
         action='store_true'
     )
 
     return parser
 
 
@@ -293,15 +296,19 @@
     )
 
 
 def _format_plain(flow, _):
     """A single line format of the form: <name> [<host>:<port>]"""
     if flow.get('contact'):
         try:
-            return f"<b>{flow['name']}</b> {flow[Cont.HOST]}:{flow[Cont.PORT]}"
+            return (
+                f"<b>{flow['name']}</b> "
+                f"{flow[Cont.HOST]}:{flow[Cont.PORT]} "
+                f"{flow[Cont.PID]}"
+            )
         except KeyError:
             LOG.warning(BAD_CONTACT_FILE_MSG.format(flow_name=flow['name']))
             return None
     else:
         return f'<{DIM}><b>{flow["name"]}</b></{DIM}>'
 
 
@@ -336,15 +343,16 @@
                 )
             },
             **{
                 name: flow[key]
                 for name, key in (
                     ('version', 'cylcVersion'),
                     ('host', Cont.HOST),
-                    ('port', Cont.PORT)
+                    ('port', Cont.PORT),
+                    ('PID', Cont.PID)
                 )
             }
         }
         maxlen = max(len(key) for key in display)
         for key, value in display.items():
             # format multiline strings by whitespace padding the lines
             value = ('\n' + (' ' * (maxlen + 7))).join(value.splitlines())
@@ -403,15 +411,16 @@
         ret.append(flow)
 
     tree = {}
     _construct_tree(ret, tree, formatter, opts, write)
 
     # print tree
     ret = get_tree(tree, '', sort=False, use_unicode=True)
-    write('\n'.join(ret))
+    if ret:
+        write('\n'.join(ret))
 
 
 def _construct_tree(flows, tree, formatter, opts, write):
     """Construct the tree, for given flows and formatter."""
     for flow in sorted(flows, key=lambda f: f['name']):
         parts = Path(flow['name']).parts
         pointer = tree
@@ -551,17 +560,16 @@
         not opts.states
         or not all(
             state in FLOW_STATES
             for state in opts.states
         )
     ):
         raise InputError(
-            '--states must be set to a comma separated list of workflow'
-            ' states. \nSee `cylc scan --help` for a list of supported'
-            ' states.'
+            '--states must be a comma separated list of workflow states.'
+            '\nSee `cylc scan --help` for supported states.'
         )
 
     if not color:
         # we cannot support colour or have been requested not to use it
         opts.colour_blind = True
 
     # print state totals key as needed
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/set_outputs.py` & `cylc-flow-8.2.0/cylc/flow/scripts/set_outputs.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/set_verbosity.py` & `cylc-flow-8.2.0/cylc/flow/scripts/set_verbosity.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/show.py` & `cylc-flow-8.2.0/cylc/flow/scripts/show.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,18 +113,14 @@
       satisfied
     }
     outputs {
       label
       message
       satisfied
     }
-    clockTrigger {
-      timeString
-      satisfied
-    }
     externalTriggers {
       id
       label
       message
       satisfied
     }
     xtriggers {
@@ -323,27 +319,19 @@
                     " ('<red>-</red>': not completed)")
                 if not t_proxy['outputs']:  # (Not possible - standard outputs)
                     print('  (None)')
                 for output in t_proxy['outputs']:
                     info = f'{task_id} {output["label"]}'
                     print_msg_state(info, output['satisfied'])
                 if (
-                        t_proxy['clockTrigger']['timeString']
-                        or t_proxy['externalTriggers']
+                        t_proxy['externalTriggers']
                         or t_proxy['xtriggers']
                 ):
                     ansiprint(
                         "<bold>other:</bold> ('<red>-</red>': not satisfied)")
-                    if t_proxy['clockTrigger']['timeString']:
-                        state = t_proxy['clockTrigger']['satisfied']
-                        time_str = t_proxy['clockTrigger']['timeString']
-                        print_msg_state(
-                            'Clock trigger time reached',
-                            state)
-                        print(f'  o Triggers at ... {time_str}')
                     for ext_trig in t_proxy['externalTriggers']:
                         state = ext_trig['satisfied']
                         print_msg_state(
                             f'{ext_trig["label"]} ... {state}',
                             state)
                     for xtrig in t_proxy['xtriggers']:
                         state = xtrig['satisfied']
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/stop.py` & `cylc-flow-8.2.0/cylc/flow/scripts/stop.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/subscribe.py` & `cylc-flow-8.2.0/cylc/flow/scripts/subscribe.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/trigger.py` & `cylc-flow-8.2.0/cylc/flow/scripts/trigger.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/tui.py` & `cylc-flow-8.2.0/cylc/flow/scripts/tui.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/validate.py` & `cylc-flow-8.2.0/cylc/flow/scripts/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,17 @@
 from cylc.flow.config import WorkflowConfig
 from cylc.flow.exceptions import (
     WorkflowConfigError,
     TaskProxySequenceBoundsError,
     TriggerExpressionError
 )
 import cylc.flow.flags
+from cylc.flow.id import Tokens
 from cylc.flow.id_cli import parse_id_async
-from cylc.flow.loggingutil import disable_timestamps
+from cylc.flow.loggingutil import set_timestamps
 from cylc.flow.option_parsers import (
     AGAINST_SOURCE_OPTION,
     WORKFLOW_ID_OR_PATH_ARG_DOC,
     CylcOptionParser as COP,
     OptionSettings,
     Options,
     ICP_OPTION,
@@ -140,15 +141,15 @@
     parser: COP, options: 'Values', workflow_id: str
 ) -> None:
     """cylc validate CLI."""
     profiler = Profiler(None, options.profile_mode)
     profiler.start()
 
     if cylc.flow.flags.verbosity < 2:
-        disable_timestamps(LOG)
+        set_timestamps(LOG, False)
 
     workflow_id, _, flow_file = await parse_id_async(
         workflow_id,
         src=True,
         constraint='workflows',
     )
     cfg = WorkflowConfig(
@@ -163,15 +164,19 @@
     # Instantiate tasks and force evaluation of trigger expressions.
     # (Taken from config.py to avoid circular import problems.)
     # TODO - This is not exhaustive, it only uses the initial cycle point.
     if cylc.flow.flags.verbosity > 0:
         print('Instantiating tasks to check trigger expressions')
     for name, taskdef in cfg.taskdefs.items():
         try:
-            itask = TaskProxy(taskdef, cfg.start_point)
+            itask = TaskProxy(
+                Tokens(workflow_id),
+                taskdef,
+                cfg.start_point,
+            )
         except TaskProxySequenceBoundsError:
             # Should already failed above
             mesg = 'Task out of bounds for %s: %s\n' % (cfg.start_point, name)
             if cylc.flow.flags.verbosity > 0:
                 sys.stderr.write(' + %s\n' % mesg)
             continue
         except Exception as exc:
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/validate_install_play.py` & `cylc-flow-8.2.0/cylc/flow/scripts/validate_install_play.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,22 +24,26 @@
 
     $ cylc validate /path/to/myworkflow
     $ cylc install /path/to/myworkflow
     $ cylc play myworkflow
 
 """
 
+import sys
+
 from cylc.flow.scripts.validate import (
     VALIDATE_OPTIONS,
     _main as validate_main
 )
 from cylc.flow.scripts.install import (
     INSTALL_OPTIONS, install_cli as cylc_install, get_source_location
 )
+from cylc.flow import LOG
 from cylc.flow.scheduler_cli import PLAY_OPTIONS
+from cylc.flow.loggingutil import set_timestamps
 from cylc.flow.option_parsers import (
     CylcOptionParser as COP,
     combine_options,
     cleanup_sysargv,
     log_subcommand,
 )
 from cylc.flow.scheduler_cli import _play
@@ -75,26 +79,25 @@
         ]
     )
     for option in VIP_OPTIONS:
         # Make a special exception for option against_source which makes
         # no sense in a VIP context.
         if option.kwargs.get('dest') != 'against_source':
             parser.add_option(*option.args, **option.kwargs)
+
     return parser
 
 
 @cli_function(get_option_parser)
 def main(parser: COP, options: 'Values', workflow_id: Optional[str] = None):
     """Run Cylc validate - install - play in sequence."""
     if not workflow_id:
         workflow_id = '.'
-
     orig_source = workflow_id
     source = get_source_location(workflow_id)
-
     log_subcommand('validate', source)
     validate_main(parser, options, str(source))
 
     log_subcommand('install', source)
     _, workflow_id = cylc_install(options, workflow_id)
 
     cleanup_sysargv(
@@ -105,9 +108,10 @@
         script_opts=(
             PLAY_OPTIONS + CYLC_ROSE_OPTIONS
             + parser.get_std_options()
         ),
         source=orig_source,
     )
 
-    log_subcommand('play', workflow_id)
+    set_timestamps(LOG, options.log_timestamp)
+    log_subcommand(*sys.argv[1:])
     _play(parser, options, workflow_id)
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/validate_reinstall.py` & `cylc-flow-8.2.0/cylc/flow/scripts/validate_reinstall.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,41 +42,48 @@
 import sys
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from optparse import Values
 
 from cylc.flow import LOG
-from cylc.flow.exceptions import ServiceFileError
+from cylc.flow.exceptions import (
+    ContactFileExists,
+    CylcError,
+)
 from cylc.flow.id_cli import parse_id
+from cylc.flow.loggingutil import set_timestamps
 from cylc.flow.option_parsers import (
     WORKFLOW_ID_ARG_DOC,
     CylcOptionParser as COP,
     combine_options,
     log_subcommand,
     cleanup_sysargv
 )
 from cylc.flow.scheduler_cli import PLAY_OPTIONS, scheduler_cli
 from cylc.flow.scripts.validate import (
     VALIDATE_OPTIONS,
     _main as cylc_validate
 )
 from cylc.flow.scripts.reinstall import (
-    REINSTALL_CYLC_ROSE_OPTIONS, reinstall_cli as cylc_reinstall
+    REINSTALL_CYLC_ROSE_OPTIONS,
+    REINSTALL_OPTIONS,
+    reinstall_cli as cylc_reinstall,
 )
 from cylc.flow.scripts.reload import (
     reload_cli as cylc_reload
 )
 from cylc.flow.terminal import cli_function
 from cylc.flow.workflow_files import detect_old_contact_file
 
 
 CYLC_ROSE_OPTIONS = COP.get_cylc_rose_options()
 VR_OPTIONS = combine_options(
     VALIDATE_OPTIONS,
+    REINSTALL_OPTIONS,
     REINSTALL_CYLC_ROSE_OPTIONS,
     PLAY_OPTIONS,
     CYLC_ROSE_OPTIONS,
     modify={'cylc-rose': 'validate, install'}
 )
 
 
@@ -131,18 +138,18 @@
         constraint='workflows',
     )
 
     # Use this interface instead of scan, because it can have an ambiguous
     # outcome which we want to capture before we install.
     try:
         detect_old_contact_file(workflow_id)
-    except ServiceFileError:
+    except ContactFileExists:
         # Workflow is definitely running:
         workflow_running = True
-    except Exception as exc:
+    except CylcError as exc:
         LOG.error(exc)
         LOG.critical(
             'Cannot tell if the workflow is running'
             '\nNote, Cylc 8 cannot restart Cylc 7 workflows.'
         )
         raise
     else:
@@ -158,29 +165,30 @@
 
     # Force on the against_source option:
     options.against_source = True   # Make validate check against source.
     log_subcommand('validate --against-source', workflow_id)
     cylc_validate(parser, options, workflow_id)
 
     log_subcommand('reinstall', workflow_id)
-    reinstall_ok = cylc_reinstall(options, workflow_id)
+    reinstall_ok = cylc_reinstall(options, workflow_id, print_reload_tip=False)
     if not reinstall_ok:
         LOG.warning(
             'No changes to source: No reinstall or'
             f' {"reload" if workflow_running else "play"} required.'
         )
         return 1
 
     # Run reload if workflow is running or paused:
     if workflow_running:
         log_subcommand('reload', workflow_id)
         cylc_reload(options, workflow_id)
 
     # run play anyway, to play a stopped workflow:
     else:
+        set_timestamps(LOG, options.log_timestamp)
         cleanup_sysargv(
             'play',
             unparsed_wid,
             options,
             compound_script_opts=VR_OPTIONS,
             script_opts=(
                 PLAY_OPTIONS + CYLC_ROSE_OPTIONS
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/view.py` & `cylc-flow-8.2.0/cylc/flow/scripts/view.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from cylc.flow.id_cli import parse_id_async
 from cylc.flow.option_parsers import (
     AGAINST_SOURCE_OPTION,
     WORKFLOW_ID_OR_PATH_ARG_DOC,
     CylcOptionParser as COP,
 )
 from cylc.flow.parsec.fileparse import read_and_proc
-from cylc.flow.templatevars import load_template_vars
+from cylc.flow.templatevars import get_template_vars
 from cylc.flow.terminal import cli_function
 
 if TYPE_CHECKING:
     from optparse import Values
 
 
 def get_option_parser():
@@ -110,26 +110,25 @@
 
 async def _main(options: 'Values', workflow_id: str) -> None:
     workflow_id, _, flow_file = await parse_id_async(
         workflow_id,
         src=True,
         constraint='workflows',
     )
-
     # read in the flow.cylc file
     viewcfg = {
         'mark': options.mark,
         'single': options.single,
         'label': options.label,
         'empy': options.empy or options.process,
         'jinja2': options.jinja2 or options.process,
         'contin': options.cat or options.process,
         'inline': (options.inline or options.jinja2 or options.empy
                    or options.process),
     }
     for line in read_and_proc(
         flow_file,
-        load_template_vars(options.templatevars, options.templatevars_file),
+        get_template_vars(options),
         viewcfg=viewcfg,
         opts=options,
     ):
         print(line)
```

### Comparing `cylc-flow-8.1.4/cylc/flow/scripts/workflow_state.py` & `cylc-flow-8.2.0/cylc/flow/scripts/workflow_state.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/subprocctx.py` & `cylc-flow-8.2.0/cylc/flow/subprocctx.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,16 +154,7 @@
 
     def get_signature(self):
         """Return the function call signature (as a string)."""
         skeys = sorted(self.func_kwargs.keys())
         args = self.func_args + [
             "%s=%s" % (i, self.func_kwargs[i]) for i in skeys]
         return "%s(%s)" % (self.func_name, ", ".join([str(a) for a in args]))
-
-    def __str__(self):
-        return (
-            f'{self.func_name}('
-            f'{", ".join(self.func_args + list(self.func_kwargs))}'
-            f'):{self.intvl}'
-        )
-
-    __repr__ = __str__
```

### Comparing `cylc-flow-8.1.4/cylc/flow/subprocpool.py` & `cylc-flow-8.2.0/cylc/flow/subprocpool.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/task_action_timer.py` & `cylc-flow-8.2.0/cylc/flow/task_action_timer.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/task_events_mgr.py` & `cylc-flow-8.2.0/cylc/flow/task_events_mgr.py`

 * *Files 2% similar despite different names*

```diff
@@ -429,27 +429,27 @@
             self.setup_event_handlers(itask, event, msg)
             return True
         else:
             return can_poll
 
     def _get_remote_conf(self, itask, key):
         """Get deprecated "[remote]" items that default to platforms."""
-        overrides = self.broadcast_mgr.get_broadcast(itask.identity)
+        overrides = self.broadcast_mgr.get_broadcast(itask.tokens)
         SKEY = 'remote'
         if SKEY not in overrides:
             overrides[SKEY] = {}
         return (
             overrides[SKEY].get(key) or
             itask.tdef.rtconfig[SKEY][key] or
             itask.platform[key]
         )
 
     def _get_workflow_platforms_conf(self, itask, key):
         """Return top level [runtime] items that default to platforms."""
-        overrides = self.broadcast_mgr.get_broadcast(itask.identity)
+        overrides = self.broadcast_mgr.get_broadcast(itask.tokens)
         return (
             overrides.get(key) or
             itask.tdef.rtconfig[key] or
             itask.platform[key]
         )
 
     def process_events(self, schd: 'Scheduler') -> None:
@@ -593,15 +593,15 @@
 
         # always update the workflow state summary for latest message
         if flag == self.FLAG_POLLED:
             new_msg = f'{message} {self.FLAG_POLLED}'
         else:
             new_msg = message
         self.data_store_mgr.delta_job_msg(
-            itask.tokens.duplicate(job=str(submit_num)).relative_id,
+            itask.tokens.duplicate(job=str(submit_num)),
             new_msg
         )
 
         # Satisfy my output, if possible, and spawn children.
         # (first remove signal: failed/EXIT -> failed)
 
         msg0 = message.split('/')[0]
@@ -674,19 +674,19 @@
                 # (sim mode does not have the job prep state)
                 self._process_message_submitted(itask, event_time)
                 self.spawn_func(itask, TASK_OUTPUT_SUBMITTED)
 
             # ... but either way update the job ID in the job proxy (it only
             # comes in via the submission message).
             if itask.tdef.run_mode != 'simulation':
-                job_d = itask.tokens.duplicate(
+                job_tokens = itask.tokens.duplicate(
                     job=str(itask.submit_num)
-                ).relative_id
+                )
                 self.data_store_mgr.delta_job_attr(
-                    job_d, 'job_id', itask.summary['submit_method_id'])
+                    job_tokens, 'job_id', itask.summary['submit_method_id'])
 
         elif message.startswith(FAIL_MESSAGE_PREFIX):
             # Task received signal.
             if (
                     flag == self.FLAG_RECEIVED
                     and itask.state.is_gt(TASK_STATUS_FAILED)
             ):
@@ -922,15 +922,15 @@
                     self.unset_waiting_event_timer(id_key)
             except KeyError as exc:
                 LOG.exception(exc)
 
     def _get_events_conf(self, itask, key, default=None):
         """Return an events setting from workflow then global configuration."""
         for getter in [
-                self.broadcast_mgr.get_broadcast(itask.identity).get("events"),
+                self.broadcast_mgr.get_broadcast(itask.tokens).get("events"),
                 itask.tdef.rtconfig["mail"],
                 itask.tdef.rtconfig["events"],
                 glbl_cfg().get(["scheduler", "mail"]),
                 glbl_cfg().get()["task events"],
         ]:
             try:
                 value = getter.get(key)
@@ -1107,17 +1107,17 @@
 
         Return True if no retries (hence go to the failed state).
         """
         no_retries = False
         if event_time is None:
             event_time = get_current_time_string()
         itask.set_summary_time('finished', event_time)
-        job_d = itask.tokens.duplicate(job=str(itask.submit_num)).relative_id
-        self.data_store_mgr.delta_job_time(job_d, 'finished', event_time)
-        self.data_store_mgr.delta_job_state(job_d, TASK_STATUS_FAILED)
+        job_tokens = itask.tokens.duplicate(job=str(itask.submit_num))
+        self.data_store_mgr.delta_job_time(job_tokens, 'finished', event_time)
+        self.data_store_mgr.delta_job_state(job_tokens, TASK_STATUS_FAILED)
         self.workflow_db_mgr.put_update_task_jobs(itask, {
             "run_status": 1,
             "time_run_exit": event_time,
         })
         if (
                 TimerFlags.EXECUTION_RETRY not in itask.try_timers
                 or itask.try_timers[TimerFlags.EXECUTION_RETRY].next() is None
@@ -1139,17 +1139,17 @@
         return no_retries
 
     def _process_message_started(self, itask, event_time):
         """Helper for process_message, handle a started message."""
         if itask.job_vacated:
             itask.job_vacated = False
             LOG.warning(f"[{itask}] Vacated job restarted")
-        job_d = itask.tokens.duplicate(job=str(itask.submit_num)).relative_id
-        self.data_store_mgr.delta_job_time(job_d, 'started', event_time)
-        self.data_store_mgr.delta_job_state(job_d, TASK_STATUS_RUNNING)
+        job_tokens = itask.tokens.duplicate(job=str(itask.submit_num))
+        self.data_store_mgr.delta_job_time(job_tokens, 'started', event_time)
+        self.data_store_mgr.delta_job_state(job_tokens, TASK_STATUS_RUNNING)
         itask.set_summary_time('started', event_time)
         self.workflow_db_mgr.put_update_task_jobs(itask, {
             "time_run": itask.summary['started_time_string']})
         if itask.state_reset(TASK_STATUS_RUNNING):
             self.setup_event_handlers(
                 itask, self.EVENT_STARTED, f'job {self.EVENT_STARTED}')
             self.data_store_mgr.delta_task_state(itask)
@@ -1157,17 +1157,18 @@
 
         # submission was successful so reset submission try number
         if TimerFlags.SUBMISSION_RETRY in itask.try_timers:
             itask.try_timers[TimerFlags.SUBMISSION_RETRY].num = 0
 
     def _process_message_succeeded(self, itask, event_time):
         """Helper for process_message, handle a succeeded message."""
-        job_d = itask.tokens.duplicate(job=str(itask.submit_num)).relative_id
-        self.data_store_mgr.delta_job_time(job_d, 'finished', event_time)
-        self.data_store_mgr.delta_job_state(job_d, TASK_STATUS_SUCCEEDED)
+
+        job_tokens = itask.tokens.duplicate(job=str(itask.submit_num))
+        self.data_store_mgr.delta_job_time(job_tokens, 'finished', event_time)
+        self.data_store_mgr.delta_job_state(job_tokens, TASK_STATUS_SUCCEEDED)
         itask.set_summary_time('finished', event_time)
         self.workflow_db_mgr.put_update_task_jobs(itask, {
             "run_status": 0,
             "time_run_exit": event_time,
         })
         # Update mean elapsed time only on task succeeded.
         if itask.summary['started_time'] is not None:
@@ -1212,17 +1213,20 @@
             self._retry_task(itask, timer.timeout, submit_retry=True)
             delay_msg = f"retrying in {timer.delay_timeout_as_str()}"
             LOG.warning(f"[{itask}] {delay_msg}")
             msg = f"job {self.EVENT_SUBMIT_FAILED}, {delay_msg}"
             self.setup_event_handlers(itask, self.EVENT_SUBMIT_RETRY, msg)
 
         # Register newly submit-failed job with the database and datastore.
-        job_d = itask.tokens.duplicate(job=str(itask.submit_num)).relative_id
+        job_tokens = itask.tokens.duplicate(job=str(itask.submit_num))
         self._insert_task_job(itask, event_time, self.JOB_SUBMIT_FAIL_FLAG)
-        self.data_store_mgr.delta_job_state(job_d, TASK_STATUS_SUBMIT_FAILED)
+        self.data_store_mgr.delta_job_state(
+            job_tokens,
+            TASK_STATUS_SUBMIT_FAILED
+        )
 
         self._reset_job_timers(itask)
 
         return no_retries
 
     def _process_message_submitted(
         self, itask: 'TaskProxy', event_time: str
@@ -1263,21 +1267,32 @@
                     self.data_store_mgr.delta_task_state(itask)
                     self.data_store_mgr.delta_task_queued(itask)
                 self._reset_job_timers(itask)
 
         # Register the newly submitted job with the database and datastore.
         # Do after itask has changed state
         self._insert_task_job(itask, event_time, self.JOB_SUBMIT_SUCCESS_FLAG)
-        job_d = itask.tokens.duplicate(job=str(itask.submit_num)).relative_id
-        self.data_store_mgr.delta_job_time(job_d, 'submitted', event_time)
+        job_tokens = itask.tokens.duplicate(job=str(itask.submit_num))
+        self.data_store_mgr.delta_job_time(
+            job_tokens,
+            'submitted',
+            event_time,
+        )
         if itask.tdef.run_mode == 'simulation':
             # Simulate job started as well.
-            self.data_store_mgr.delta_job_time(job_d, 'started', event_time)
+            self.data_store_mgr.delta_job_time(
+                job_tokens,
+                'started',
+                event_time,
+            )
         else:
-            self.data_store_mgr.delta_job_state(job_d, TASK_STATUS_SUBMITTED)
+            self.data_store_mgr.delta_job_state(
+                job_tokens,
+                TASK_STATUS_SUBMITTED,
+            )
 
     def _insert_task_job(
         self,
         itask: 'TaskProxy',
         event_time: str,
         submit_status: int
     ):
```

### Comparing `cylc-flow-8.1.4/cylc/flow/task_id.py` & `cylc-flow-8.2.0/cylc/flow/task_id.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/task_job_logs.py` & `cylc-flow-8.2.0/cylc/flow/task_job_logs.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/task_job_mgr.py` & `cylc-flow-8.2.0/cylc/flow/task_job_mgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,15 +364,15 @@
                     # Remote init not in progress for target, so start it.
                     self.task_remote_mgr.remote_init(
                         platform, curve_auth, client_pub_key_dir)
                     for itask in itasks:
                         self.data_store_mgr.delta_job_msg(
                             itask.tokens.duplicate(
                                 job=str(itask.submit_num)
-                            ).relative_id,
+                            ),
                             self.REMOTE_INIT_MSG,
                         )
                     continue
 
                 elif ri_map[install_target] == REMOTE_INIT_DONE:
                     # Already done remote init so move on to file install
                     self.task_remote_mgr.file_install(platform)
@@ -393,15 +393,15 @@
                     del ri_map[install_target]
                     self.task_remote_mgr.remote_init(
                         platform, curve_auth, client_pub_key_dir)
                     for itask in itasks:
                         self.data_store_mgr.delta_job_msg(
                             itask.tokens.duplicate(
                                 job=str(itask.submit_num)
-                            ).relative_id,
+                            ),
                             self.REMOTE_INIT_MSG
                         )
                     continue
 
             # Ensure that localhost background/at jobs are recorded as running
             # on the host name of the current workflow host, rather than just
             # "localhost". On restart on a different workflow host, this
@@ -417,15 +417,15 @@
                 del ri_map[install_target]
                 self.task_remote_mgr.remote_init(
                     platform, curve_auth, client_pub_key_dir)
                 for itask in itasks:
                     self.data_store_mgr.delta_job_msg(
                         itask.tokens.duplicate(
                             job=str(itask.submit_num)
-                        ).relative_id,
+                        ),
                         self.REMOTE_INIT_MSG,
                     )
                 continue
 
             if (
                 self.job_runner_mgr.is_job_local_to_host(
                     itask.summary['job_runner_name']
@@ -451,15 +451,15 @@
             if ri_map[install_target] == REMOTE_FILE_INSTALL_255:
                 del ri_map[install_target]
                 self.task_remote_mgr.file_install(platform)
                 for itask in itasks:
                     self.data_store_mgr.delta_job_msg(
                         itask.tokens.duplicate(
                             job=str(itask.submit_num)
-                        ).relative_id,
+                        ),
                         REMOTE_FILE_INSTALL_IN_PROGRESS
                     )
                 continue
 
             if ri_map[install_target] in {
                 REMOTE_INIT_FAILED, REMOTE_FILE_INSTALL_FAILED
             }:
@@ -701,15 +701,15 @@
             log_lvl = DEBUG
             log_msg = (
                 'ignoring job kill result, unexpected task state: %s' %
                 itask.state.status)
         self.data_store_mgr.delta_job_msg(
             itask.tokens.duplicate(
                 job=str(itask.submit_num)
-            ).relative_id,
+            ),
             log_msg
         )
         LOG.log(log_lvl, f"[{itask}] {log_msg}")
 
     def _manip_task_jobs_callback(
             self, ctx, workflow, itasks, summary_callback,
             more_callbacks=None):
@@ -806,25 +806,25 @@
 
     def _poll_task_job_callback(self, workflow, itask, cmd_ctx, line):
         """Helper for _poll_task_jobs_callback, on one task job."""
         ctx = SubProcContext(self.JOBS_POLL, None)
         ctx.out = line
         ctx.ret_code = 0
         # See cylc.flow.job_runner_mgr.JobPollContext
-        job_d = itask.tokens.duplicate(job=str(itask.submit_num)).relative_id
+        job_tokens = itask.tokens.duplicate(job=str(itask.submit_num))
         try:
             job_log_dir, context = line.split('|')[1:3]
             items = json.loads(context)
             jp_ctx = JobPollContext(job_log_dir, **items)
         except TypeError:
-            self.data_store_mgr.delta_job_msg(job_d, self.POLL_FAIL)
+            self.data_store_mgr.delta_job_msg(job_tokens, self.POLL_FAIL)
             ctx.cmd = cmd_ctx.cmd  # print original command on failure
             return
         except ValueError:
-            self.data_store_mgr.delta_job_msg(job_d, self.POLL_FAIL)
+            self.data_store_mgr.delta_job_msg(job_tokens, self.POLL_FAIL)
             ctx.cmd = cmd_ctx.cmd  # print original command on failure
             return
         finally:
             log_task_job_activity(ctx, workflow, itask.point, itask.tdef.name)
 
         flag = self.task_events_mgr.FLAG_POLLED
         # Only log at INFO level if manually polling
@@ -1091,15 +1091,15 @@
 
         """
         if itask.local_job_file_path:
             return itask
 
         # Handle broadcasts
         overrides = self.task_events_mgr.broadcast_mgr.get_broadcast(
-            itask.identity
+            itask.tokens
         )
         if overrides:
             rtconfig = pdeepcopy(itask.tdef.rtconfig)
             poverride(rtconfig, overrides, prepend=True)
         else:
             rtconfig = itask.tdef.rtconfig
```

### Comparing `cylc-flow-8.1.4/cylc/flow/task_message.py` & `cylc-flow-8.2.0/cylc/flow/task_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     """Record task job messages.
 
     Print the messages according to their severity.
     Write the messages in the job status file.
     Send the messages to the workflow, if possible.
 
     Arguments:
-        workflow: Workflow name.
+        workflow: Workflow ID.
         job_id: Job identifier "CYCLE/TASK_NAME/SUBMIT_NUM".
         messages: List of messages "[[severity, message], ...]".
     """
     # Record the event time, in case the message is delayed in some way.
     event_time = get_current_time_string(
         override_use_utc=(os.getenv('CYLC_UTC') == 'True'))
     write_messages(workflow, job_id, messages, event_time)
```

### Comparing `cylc-flow-8.1.4/cylc/flow/task_outputs.py` & `cylc-flow-8.2.0/cylc/flow/task_outputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,24 @@
     TASK_OUTPUT_EXPIRED,
     TASK_OUTPUT_SUBMITTED,
     TASK_OUTPUT_SUBMIT_FAILED,
     TASK_OUTPUT_STARTED,
     TASK_OUTPUT_SUCCEEDED,
     TASK_OUTPUT_FAILED)
 
+TASK_OUTPUTS = (
+    TASK_OUTPUT_EXPIRED,
+    TASK_OUTPUT_SUBMITTED,
+    TASK_OUTPUT_SUBMIT_FAILED,
+    TASK_OUTPUT_STARTED,
+    TASK_OUTPUT_SUCCEEDED,
+    TASK_OUTPUT_FAILED,
+    TASK_OUTPUT_FINISHED,
+)
+
 _TRIGGER = 0
 _MESSAGE = 1
 _IS_COMPLETED = 2
 
 
 class TaskOutputs:
     """Task output message manager.
```

### Comparing `cylc-flow-8.1.4/cylc/flow/task_pool.py` & `cylc-flow-8.2.0/cylc/flow/task_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,52 +90,52 @@
 
     ERR_TMPL_NO_TASKID_MATCH = "No matching tasks found: {0}"
     ERR_PREFIX_TASK_NOT_ON_SEQUENCE = "Invalid cycle point for task: {0}, {1}"
     SUICIDE_MSG = "suicide"
 
     def __init__(
         self,
+        tokens: 'Tokens',
         config: 'WorkflowConfig',
         workflow_db_mgr: 'WorkflowDatabaseManager',
         task_events_mgr: 'TaskEventsManager',
         data_store_mgr: 'DataStoreMgr',
         flow_mgr: 'FlowMgr'
     ) -> None:
-
+        self.tokens = tokens
         self.config: 'WorkflowConfig' = config
         self.stop_point = config.stop_point or config.final_point
         self.workflow_db_mgr: 'WorkflowDatabaseManager' = workflow_db_mgr
         self.task_events_mgr: 'TaskEventsManager' = task_events_mgr
         # TODO this is ugly:
         self.task_events_mgr.spawn_func = self.spawn_on_output
         self.data_store_mgr: 'DataStoreMgr' = data_store_mgr
         self.flow_mgr: 'FlowMgr' = flow_mgr
 
-        self.do_reload = False
         self.max_future_offset: Optional['IntervalBase'] = None
         self._prev_runahead_base_point: Optional['PointBase'] = None
         self._prev_runahead_sequence_points: Optional[Set['PointBase']] = None
         self.runahead_limit_point: Optional['PointBase'] = None
 
         self.main_pool: Pool = {}
         self.hidden_pool: Pool = {}
         self._main_pool_list: List[TaskProxy] = []
         self._hidden_pool_list: List[TaskProxy] = []
         self.main_pool_changed = False
         self.hidden_pool_changed = False
+        self.tasks_removed = False
 
         self.hold_point: Optional['PointBase'] = None
         self.abs_outputs_done: Set[Tuple[str, str, str]] = set()
 
         self.stop_task_id: Optional[str] = None
         self.stop_task_finished = False
         self.abort_task_failed = False
         self.expected_failed_tasks = self.config.get_expected_failed_tasks()
 
-        self.orphans: List[str] = []
         self.task_name_list = self.config.get_task_name_list()
         self.task_queue_mgr = IndepQueueManager(
             self.config.cfg['scheduling']['queues'],
             self.task_name_list,
             self.config.runtime['descendants']
         )
         self.tasks_to_hold: Set[Tuple[str, 'PointBase']] = set()
@@ -155,18 +155,17 @@
 
     def stop_task_done(self):
         """Return True if stop task has succeeded."""
         if self.stop_task_id is not None and self.stop_task_finished:
             LOG.info("Stop task %s finished" % self.stop_task_id)
             self.stop_task_id = None
             self.stop_task_finished = False
-            self.workflow_db_mgr.delete_workflow_stop_task()
+            self.workflow_db_mgr.put_workflow_stop_task(None)
             return True
-        else:
-            return False
+        return False
 
     def _swap_out(self, itask):
         """Swap old task for new, during reload."""
         if itask.identity in self.hidden_pool.get(itask.point, set()):
             self.hidden_pool[itask.point][itask.identity] = itask
             self.hidden_pool_changed = True
         elif itask.identity in self.main_pool.get(itask.point, set()):
@@ -307,20 +306,25 @@
         The limit itself is limited by workflow stop point, if there is one,
         and adjusted upward on the fly if tasks with future offsets appear.
 
         With force=True we recompute the limit even if the base point has not
         changed (needed if max_future_offset changed, or on reload).
         """
         points: List['PointBase'] = []
+        sequence_points: Set['PointBase']
         if not self.main_pool:
             # Start at first point in each sequence, after the initial point.
-            points = list({
-                seq.get_first_point(self.config.start_point)
-                for seq in self.config.sequences
-            })
+            points = [
+                point
+                for point in {
+                    seq.get_first_point(self.config.start_point)
+                    for seq in self.config.sequences
+                }
+                if point is not None
+            ]
         else:
             # Find the earliest point with unfinished tasks.
             for point, itasks in sorted(self.get_tasks_by_point().items()):
                 if (
                     points  # got the limit already so this point too
                     or any(
                         not itask.state(
@@ -467,14 +471,15 @@
             LOG.info("LOADING task proxies")
         # Create a task proxy corresponding to this DB entry.
         (cycle, name, flow_nums, flow_wait, is_manual_submit, is_late, status,
          is_held, submit_num, _, platform_name, time_submit, time_run, timeout,
          outputs_str) = row
         try:
             itask = TaskProxy(
+                self.tokens,
                 self.config.get_taskdef(name),
                 get_point(cycle),
                 deserialise(flow_nums),
                 status=status,
                 is_held=is_held,
                 submit_num=submit_num,
                 is_late=bool(is_late),
@@ -725,41 +730,43 @@
                 point, tdef.name, flow_nums
             )
             if ntask is not None:
                 self.add_to_pool(ntask)
 
     def remove(self, itask, reason=""):
         """Remove a task from the pool (e.g. after a reload)."""
+        self.tasks_removed = True
         msg = "task proxy removed"
         if reason:
             msg += f" ({reason})"
 
         try:
             del self.hidden_pool[itask.point][itask.identity]
         except KeyError:
             pass
         else:
             # e.g. for suicide of partially satisfied task
             self.hidden_pool_changed = True
             if not self.hidden_pool[itask.point]:
                 del self.hidden_pool[itask.point]
             LOG.debug(f"[{itask}] {msg}")
+            self.task_queue_mgr.remove_task(itask)
             return
 
         try:
             del self.main_pool[itask.point][itask.identity]
         except KeyError:
             pass
         else:
             self.main_pool_changed = True
             if not self.main_pool[itask.point]:
                 del self.main_pool[itask.point]
-                self.task_queue_mgr.remove_task(itask)
-                if itask.tdef.max_future_prereq_offset is not None:
-                    self.set_max_future_offset()
+            self.task_queue_mgr.remove_task(itask)
+            if itask.tdef.max_future_prereq_offset is not None:
+                self.set_max_future_offset()
 
             # Notify the data-store manager of their removal
             # (the manager uses window boundary tracking for pruning).
             self.data_store_mgr.remove_pool_node(itask.tdef.name, itask.point)
             # Event-driven final update of task_states table.
             # TODO: same for datastore (still updated by scheduler loop)
             self.workflow_db_mgr.put_update_task_state(itask)
@@ -787,15 +794,15 @@
         if self.hidden_pool_changed:
             self.hidden_pool_changed = False
             self._hidden_pool_list = []
             for itask_id_maps in self.hidden_pool.values():
                 self._hidden_pool_list.extend(list(itask_id_maps.values()))
         return self._hidden_pool_list
 
-    def get_tasks_by_point(self):
+    def get_tasks_by_point(self) -> 'Dict[PointBase, List[TaskProxy]]':
         """Return a map of task proxies by cycle point."""
         point_itasks = {}
         for point, itask_id_map in self.main_pool.items():
             point_itasks[point] = list(itask_id_map.values())
         for point, itask_id_map in self.hidden_pool.items():
             if point not in point_itasks:
                 point_itasks[point] = list(itask_id_map.values())
@@ -907,68 +914,69 @@
                 )
             ):
                 max_offset = itask.tdef.max_future_prereq_offset
         self.max_future_offset = max_offset
         if max_offset != orig and self.compute_runahead(force=True):
             self.release_runahead_tasks()
 
-    def set_do_reload(self, config: 'WorkflowConfig') -> None:
-        """Set the task pool to reload mode."""
-        self.config = config
-        self.stop_point = config.stop_point or config.final_point
-        self.do_reload = True
-
-        # find any old tasks that have been removed from the workflow
-        old_task_name_list = self.task_name_list
-        self.task_name_list = self.config.get_task_name_list()
-        for name in old_task_name_list:
-            if name not in self.task_name_list:
-                self.orphans.append(name)
-        for name in self.task_name_list:
-            if name in self.orphans:
-                self.orphans.remove(name)
-        # adjust the new workflow config to handle the orphans
-        self.config.adopt_orphans(self.orphans)
-
-    def reload_taskdefs(self) -> None:
+    def reload_taskdefs(self, config: 'WorkflowConfig') -> None:
         """Reload the definitions of task proxies in the pool.
 
         Orphaned tasks (whose definitions were removed from the workflow):
         - remove if not active yet
         - if active, leave them but prevent them from spawning children on
           subsequent outputs
         Otherwise: replace task definitions but copy over existing outputs etc.
 
         """
+        self.config = config
+        self.stop_point = config.stop_point or config.final_point
+
+        # find any old tasks that have been removed from the workflow
+        old_task_name_list = self.task_name_list
+        self.task_name_list = self.config.get_task_name_list()
+        orphans = [
+            task
+            for task in old_task_name_list
+            if task not in self.task_name_list
+        ]
+
+        # adjust the new workflow config to handle the orphans
+        self.config.adopt_orphans(orphans)
+
         LOG.info("Reloading task definitions.")
         tasks = self.get_all_tasks()
         # Log tasks orphaned by a reload but not currently in the task pool.
-        for name in self.orphans:
+        for name in orphans:
             if name not in (itask.tdef.name for itask in tasks):
                 LOG.warning("Removed task: '%s'", name)
         for itask in tasks:
-            if itask.tdef.name in self.orphans:
+            if itask.tdef.name in orphans:
                 if (
-                        itask.state(TASK_STATUS_WAITING)
-                        or itask.state.is_held
-                        or itask.state.is_queued
+                    itask.state(TASK_STATUS_WAITING)
+                    or itask.state.is_held
+                    or itask.state.is_queued
                 ):
                     # Remove orphaned task if it hasn't started running yet.
                     self.remove(itask, 'task definition removed')
                 else:
                     # Keep active orphaned task, but stop it from spawning.
                     itask.graph_children = {}
                     LOG.warning(
                         f"[{itask}] will not spawn children "
                         "- task definition removed"
                     )
             else:
                 new_task = TaskProxy(
+                    self.tokens,
                     self.config.get_taskdef(itask.tdef.name),
-                    itask.point, itask.flow_nums, itask.state.status)
+                    itask.point,
+                    itask.flow_nums,
+                    itask.state.status,
+                )
                 itask.copy_to_reload_successor(
                     new_task,
                     self.check_task_output,
                 )
                 self._swap_out(new_task)
                 self.data_store_mgr.delta_task_prerequisite(new_task)
                 LOG.info(f"[{itask}] reloaded task definition")
@@ -994,24 +1002,17 @@
         for itask in self.get_tasks():
             # Recreate data store elements from main pool.
             self.create_data_store_elements(itask)
             if itask.state.is_queued:
                 # Already queued
                 continue
             ready_check_items = itask.is_ready_to_run()
-            # Use this periodic checking point for data-store delta
-            # creation, some items aren't event driven (i.e. clock).
-            if itask.tdef.clocktrigger_offset is not None:
-                self.data_store_mgr.delta_task_clock_trigger(
-                    itask, ready_check_items)
             if all(ready_check_items) and not itask.state.is_runahead:
                 self.queue_task(itask)
 
-        self.do_reload = False
-
     def set_stop_point(self, stop_point: 'PointBase') -> bool:
         """Set the workflow stop cycle point.
 
         And reset the runahead limit if less than the stop point.
         """
         if self.stop_point == stop_point:
             LOG.info(f"Stop point unchanged: {stop_point}")
@@ -1229,15 +1230,15 @@
     def release_hold_point(self) -> None:
         """Unset the workflow hold point and release all held active tasks."""
         self.hold_point = None
         for itask in self.get_all_tasks():
             self.release_held_active_task(itask)
         self.tasks_to_hold.clear()
         self.workflow_db_mgr.put_tasks_to_hold(self.tasks_to_hold)
-        self.workflow_db_mgr.delete_workflow_hold_cycle_point()
+        self.workflow_db_mgr.put_workflow_hold_cycle_point(None)
 
     def check_abort_on_task_fails(self):
         """Check whether workflow should abort on task failure.
 
         Return True if a task failed and `--abort-if-any-task-fails` was given.
         """
         return self.abort_task_failed
@@ -1265,19 +1266,19 @@
         self.workflow_db_mgr.put_update_task_outputs(itask)
         if (
             output == TASK_OUTPUT_FAILED
             and self.expected_failed_tasks is not None
             and itask.identity not in self.expected_failed_tasks
         ):
             self.abort_task_failed = True
-        try:
-            children = itask.graph_children[output]
-        except KeyError:
-            # No children depend on this output
-            children = []
+
+        children = []
+        if itask.flow_nums or forced:
+            with suppress(KeyError):
+                children = itask.graph_children[output]
 
         suicide = []
         for c_name, c_point, is_abs in children:
             if is_abs:
                 self.abs_outputs_done.add(
                     (str(itask.point), itask.tdef.name, output))
                 self.workflow_db_mgr.put_insert_abs_output(
@@ -1399,14 +1400,16 @@
 
         If completed_only is True:
            Used to retroactively spawn on already-completed outputs when a flow
            merges into a force-triggered no-flow task. In this case, do set the
            associated prerequisites of spawned children to satisifed.
 
         """
+        if not itask.flow_nums:
+            return
         if completed_only:
             outputs = itask.state.outputs.get_completed()
         else:
             outputs = itask.state.outputs._by_message
 
         for output in outputs:
             try:
@@ -1514,20 +1517,21 @@
                 self.ERR_PREFIX_TASK_NOT_ON_SEQUENCE.format(
                     taskdef.name, point
                 )
             )
             return None
 
         itask = TaskProxy(
+            self.tokens,
             taskdef,
             point,
             flow_nums,
             submit_num=submit_num,
             is_manual_submit=is_manual_submit,
-            flow_wait=flow_wait
+            flow_wait=flow_wait,
         )
         if (name, point) in self.tasks_to_hold:
             LOG.info(f"[{itask}] holding (as requested earlier)")
             self.hold_active_task(itask)
         elif self.hold_point and itask.point > self.hold_point:
             # Hold if beyond the workflow hold point
             LOG.info(
@@ -1595,25 +1599,38 @@
             flow_nums = None
         else:
             flow_nums = {flow_num}
 
         n_warnings, task_items = self.match_taskdefs(items)
         for (_, point), taskdef in sorted(task_items.items()):
             # This the parent task:
-            itask = TaskProxy(taskdef, point, flow_nums=flow_nums)
+            itask = TaskProxy(
+                self.tokens,
+                taskdef,
+                point,
+                flow_nums=flow_nums,
+            )
             # Spawn children of selected outputs.
             for trig, out, _ in itask.state.outputs.get_all():
                 if trig in outputs:
                     LOG.info(f"[{itask}] Forced spawning on {out}")
                     self.spawn_on_output(itask, out, forced=True)
 
-    def _get_active_flow_nums(self):
+    def _get_active_flow_nums(self) -> Set[int]:
+        """Return all active, or most recent previous, flow numbers.
+
+        If there are any active flows, return all active flow numbers.
+        Otherwise (e.g. on restarting a completed workflow) return
+        the flow numbers of the most recent previous active task.
+        """
         fnums = set()
         for itask in self.get_all_tasks():
             fnums.update(itask.flow_nums)
+        if not fnums:
+            fnums = self.workflow_db_mgr.pri_dao.select_latest_flow_nums()
         return fnums
 
     def remove_tasks(self, items):
         """Remove tasks from the pool."""
         itasks, _, bad_items = self.filter_task_proxies(items)
         for itask in itasks:
             self.remove(itask, 'request')
@@ -1720,17 +1737,20 @@
                 itask.summary['started_time'] = now
             timeout = (itask.summary['started_time'] +
                        itask.tdef.rtconfig['job']['simulated run length'])
             if now > timeout:
                 conf = itask.tdef.rtconfig['simulation']
                 job_d = itask.tokens.duplicate(job=str(itask.submit_num))
                 now_str = get_current_time_string()
-                if (itask.point in conf['fail cycle points'] and
-                        (itask.get_try_num() == 1 or
-                         not conf['fail try 1 only'])):
+                if (
+                    conf['fail cycle points'] is None  # i.e. "all"
+                    or itask.point in conf['fail cycle points']
+                ) and (
+                    itask.get_try_num() == 1 or not conf['fail try 1 only']
+                ):
                     message_queue.put(
                         TaskMsg(job_d, now_str, 'CRITICAL', TASK_STATUS_FAILED)
                     )
                 else:
                     # Simulate message outputs.
                     for msg in itask.tdef.rtconfig['outputs'].values():
                         message_queue.put(
```

### Comparing `cylc-flow-8.1.4/cylc/flow/task_proxy.py` & `cylc-flow-8.2.0/cylc/flow/task_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Provide a class to represent a task proxy in a running workflow."""
 
 from collections import Counter
 from copy import copy
 from fnmatch import fnmatchcase
-from time import time
 from typing import (
     Any, Callable, Dict, List, Set, Tuple, Optional, TYPE_CHECKING
 )
 
 from metomi.isodatetime.timezone import get_local_time_zone
 
 from cylc.flow import LOG
@@ -47,15 +46,15 @@
 
 class TaskProxy:
     """Represent an instance of a cycling task in a running workflow.
 
     Attributes:
         .clock_trigger_time:
             Clock trigger time in seconds since epoch.
-            (Used for both old-style clock triggers and wall_clock xtrigger).
+            (Used for wall_clock xtrigger).
         .expire_time:
             Time in seconds since epoch when this task is considered expired.
         .identity:
             Task ID in POINT/NAME syntax.
         .tokens:
             Task ID tokens.
         .is_late:
@@ -181,14 +180,15 @@
         'tokens',
         'try_timers',
         'waiting_on_job_prep',
     ]
 
     def __init__(
         self,
+        scheduler_tokens: 'Tokens',
         tdef: 'TaskDef',
         start_point: 'PointBase',
         flow_nums: Optional[Set[int]] = None,
         status: str = TASK_STATUS_WAITING,
         is_held: bool = False,
         submit_num: int = 0,
         is_late: bool = False,
@@ -205,16 +205,15 @@
         if flow_nums is None:
             self.flow_nums = set()
         else:
             # (don't share flow_nums ref with parent task)
             self.flow_nums = copy(flow_nums)
         self.flow_wait = flow_wait
         self.point = start_point
-        self.tokens = Tokens(
-            # TODO: make these absolute?
+        self.tokens = scheduler_tokens.duplicate(
             cycle=str(self.point),
             task=self.tdef.name,
         )
         self.identity = self.tokens.relative_id
         self.reload_successor: Optional['TaskProxy'] = None
         self.point_as_seconds: Optional[int] = None
 
@@ -387,55 +386,42 @@
         """Return the next cycle point."""
         return self.tdef.next_point(self.point)
 
     def is_ready_to_run(self) -> Tuple[bool, ...]:
         """Is this task ready to run?
 
         Takes account of all dependence: on other tasks, xtriggers, and
-        old-style ext- and clock-triggers. Or, manual triggering.
+        old-style ext-triggers. Or, manual triggering.
 
         """
         if self.is_manual_submit:
             # Manually triggered, ignore unsatisfied prerequisites.
             return (True,)
         if self.state.is_held:
             # A held task is not ready to run.
             return (False,)
         if self.state.status in self.try_timers:
             # A try timer is still active.
             return (self.try_timers[self.state.status].is_delay_done(),)
         return (
             self.state(TASK_STATUS_WAITING),
-            self.is_waiting_clock_done(),
             self.is_waiting_prereqs_done()
         )
 
     def set_summary_time(self, event_key, time_str=None):
         """Set an event time in self.summary
 
         Set values of both event_key + "_time" and event_key + "_time_string".
         """
         if time_str is None:
             self.summary[event_key + '_time'] = None
         else:
             self.summary[event_key + '_time'] = float(str2time(time_str))
         self.summary[event_key + '_time_string'] = time_str
 
-    def is_waiting_clock_done(self):
-        """Is this task done waiting for its old-style clock trigger time?
-
-        Return True if there is no clock trigger or when clock trigger is done.
-        """
-        if self.tdef.clocktrigger_offset is None:
-            return True
-        return (
-            time() >
-            self.get_clock_trigger_time(str(self.tdef.clocktrigger_offset))
-        )
-
     def is_task_prereqs_not_done(self):
         """Are some task prerequisites not satisfied?"""
         return (not all(pre.is_satisfied()
                 for pre in self.state.prerequisites))
 
     def is_waiting_prereqs_done(self):
         """Are ALL prerequisites satisfied?"""
```

### Comparing `cylc-flow-8.1.4/cylc/flow/task_queues/__init__.py` & `cylc-flow-8.2.0/cylc/flow/task_queues/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/task_queues/independent.py` & `cylc-flow-8.2.0/cylc/flow/task_queues/independent.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/task_remote_cmd.py` & `cylc-flow-8.2.0/cylc/flow/task_remote_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             KeyType.PUBLIC, KeyOwner.SERVER, workflow_srv_dir=srvd)})
     for k in keys.values():
         if os.path.exists(k.full_key_path):
             os.remove(k.full_key_path)
 
 
 def create_client_keys(srvd, install_target):
-    """Create or renew authentication keys for workflow 'reg' in the .service
+    """Create or renew authentication keys for workflow 'id_' in the .service
      directory.
      Generate a pair of ZMQ authentication keys"""
 
     cli_pub_key = KeyInfo(
         KeyType.PUBLIC,
         KeyOwner.CLIENT,
         workflow_srv_dir=srvd,
```

### Comparing `cylc-flow-8.1.4/cylc/flow/task_remote_mgr.py` & `cylc-flow-8.2.0/cylc/flow/task_remote_mgr.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,16 +342,17 @@
         """Remove workflow contact files and keys from initialised remotes.
 
         Call "cylc remote-tidy".
         This method is called on workflow shutdown, so we want nothing to hang.
         Timeout any incomplete commands after 10 seconds.
         """
         # Get a list of all platforms used from workflow database:
-        platforms_used = (
-            self.db_mgr.get_pri_dao().select_task_job_platforms())
+        with self.db_mgr.get_pri_dao() as pri_dao:
+            platforms_used = pri_dao.select_task_job_platforms()
+
         # For each install target compile a list of platforms:
         install_targets = {
             target for target, msg
             in self.remote_init_map.items()
             if msg == REMOTE_FILE_INSTALL_DONE
         }
         install_targets_map = self._get_remote_tidy_targets(
```

### Comparing `cylc-flow-8.1.4/cylc/flow/task_state.py` & `cylc-flow-8.2.0/cylc/flow/task_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,20 +360,14 @@
 
     def set_prerequisites_all_satisfied(self):
         """Set prerequisites to all satisfied."""
         for prereq in self.prerequisites:
             prereq.set_satisfied()
         self._is_satisfied = None
 
-    def set_prerequisites_not_satisfied(self):
-        """Reset prerequisites."""
-        for prereq in self.prerequisites:
-            prereq.set_not_satisfied()
-        self._is_satisfied = None
-
     def get_resolved_dependencies(self):
         """Return a list of dependencies which have been met for this task.
 
         E.G: ['1/foo', '2/bar']
 
         The returned list is sorted to allow comparison with reference run
         task with lots of near-simultaneous triggers.
```

### Comparing `cylc-flow-8.1.4/cylc/flow/task_state_prop.py` & `cylc-flow-8.2.0/cylc/flow/task_state_prop.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/task_trigger.py` & `cylc-flow-8.2.0/cylc/flow/task_trigger.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,31 +13,18 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from cylc.flow.cycling.loader import (
     get_point, get_point_relative, get_interval)
 from cylc.flow.prerequisite import Prerequisite
-from cylc.flow.task_outputs import (
-    TASK_OUTPUT_EXPIRED, TASK_OUTPUT_SUBMITTED, TASK_OUTPUT_SUBMIT_FAILED,
-    TASK_OUTPUT_STARTED, TASK_OUTPUT_SUCCEEDED, TASK_OUTPUT_FAILED,
-    TASK_OUTPUT_FINISHED
-)
+from cylc.flow.task_qualifiers import ALT_QUALIFIERS
 
 # Task trigger names (e.g. foo:fail => bar).
 # Can use "foo:fail => bar" or "foo:failed => bar", etc.
-_ALT_TRIGGER_NAMES = {
-    TASK_OUTPUT_EXPIRED: ["expire"],
-    TASK_OUTPUT_SUBMITTED: ["submit"],
-    TASK_OUTPUT_SUBMIT_FAILED: ["submit-fail"],
-    TASK_OUTPUT_STARTED: ["start"],
-    TASK_OUTPUT_SUCCEEDED: ["succeed"],
-    TASK_OUTPUT_FAILED: ["fail"],
-    TASK_OUTPUT_FINISHED: ["finish"],
-}
 
 
 class TaskTrigger:
     """Class representing an upstream dependency.
 
     Args:
         task_name (str): The name of the upstream task.
@@ -153,19 +140,25 @@
 
     @staticmethod
     def standardise_name(name):
         """Replace trigger name aliases with standard names.
 
         Arg name should be a valid standard name or alias, otherwise assumed
         to be a custom trigger and return as-is.
+
+        Examples:
+            >>> TaskTrigger.standardise_name('foo')
+            'foo'
+            >>> TaskTrigger.standardise_name('succeed')
+            'succeeded'
+            >>> TaskTrigger.standardise_name('succeeded')
+            'succeeded'
+
         """
-        for standard_name, alt_names in _ALT_TRIGGER_NAMES.items():
-            if name == standard_name or name in alt_names:
-                return standard_name
-        return name
+        return ALT_QUALIFIERS.get(name, name)
 
 
 class Dependency:
     """A graph dependency in its abstract form.
 
     Used to generate cylc.flow.prerequisite.Prerequisite objects.
```

### Comparing `cylc-flow-8.1.4/cylc/flow/taskdef.py` & `cylc-flow-8.2.0/cylc/flow/taskdef.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     """Task definition."""
 
     # Memory optimization - constrain possible attributes to this list.
     __slots__ = [
         "run_mode", "rtconfig", "start_point", "initial_point", "sequences",
         "used_in_offset_trigger", "max_future_prereq_offset",
         "sequential", "is_coldstart",
-        "workflow_polling_cfg", "clocktrigger_offset", "expiration_offset",
+        "workflow_polling_cfg", "expiration_offset",
         "namespace_hierarchy", "dependencies", "outputs", "param_var",
         "graph_children", "graph_parents", "has_abs_triggers",
         "external_triggers", "xtrig_labels", "name", "elapsed_times"]
 
     # Store the elapsed times for a maximum of 10 cycles
     MAX_LEN_ELAPSED_TIMES = 10
 
@@ -154,15 +154,14 @@
         self.used_in_offset_trigger = False
 
         # some defaults
         self.max_future_prereq_offset = None
         self.sequential = False
         self.workflow_polling_cfg = {}
 
-        self.clocktrigger_offset = None
         self.expiration_offset = None
         self.namespace_hierarchy = []
         self.dependencies = {}
         self.outputs = {}  # {output: (message, is_required)}
         self.graph_children = {}
         self.graph_parents = {}
         self.param_var = {}
```

### Comparing `cylc-flow-8.1.4/cylc/flow/terminal.py` & `cylc-flow-8.2.0/cylc/flow/terminal.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/time_parser.py` & `cylc-flow-8.2.0/cylc/flow/time_parser.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/timer.py` & `cylc-flow-8.2.0/cylc/flow/timer.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/tui/__init__.py` & `cylc-flow-8.2.0/cylc/flow/tui/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/tui/app.py` & `cylc-flow-8.2.0/cylc/flow/tui/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,15 +197,15 @@
 
     This is a single workflow view component (purposefully).
 
     Multi-workflow functionality can be achieved via a GScan-esque
     tab/selection panel.
 
     Arguments:
-        reg (str):
+        id_ (str):
             Workflow registration
 
     """
 
     UPDATE_INTERVAL = 1
     CLIENT_TIMEOUT = 1
 
@@ -223,16 +223,16 @@
         (f'overlay_job_{status}', colour, 'light gray')
         for status, colour in JOB_COLOURS.items()
     ] + [  # workflow state colours
         (f'workflow_{status}',) + spec
         for status, spec in WORKFLOW_COLOURS.items()
     ]
 
-    def __init__(self, reg, screen=None):
-        self.reg = reg
+    def __init__(self, id_, screen=None):
+        self.id_ = id_
         self.client = None
         self.loop = None
         self.screen = None
         self.stack = 0
         self.tree_walker = None
 
         # create the template
@@ -293,15 +293,15 @@
 
         Returns:
             dict if successful, else False
 
         """
         try:
             if not self.client:
-                self.client = get_client(self.reg, timeout=self.CLIENT_TIMEOUT)
+                self.client = get_client(self.id_, timeout=self.CLIENT_TIMEOUT)
             data = self.client(
                 'graphql',
                 {
                     'request_string': QUERY,
                     'variables': {
                         # list of task states we want to see
                         'taskStates': [
@@ -311,29 +311,29 @@
                         ]
                     }
                 }
             )
         except WorkflowStopped:
             # Distinguish stopped flow from non-existent flow.
             self.client = None
-            full_path = Path(get_workflow_run_dir(self.reg))
+            full_path = Path(get_workflow_run_dir(self.id_))
             if (
                 (full_path / WorkflowFiles.SUITE_RC).is_file()
                 or (full_path / WorkflowFiles.FLOW_FILE).is_file()
             ):
                 message = "stopped"
             else:
                 message = (
                     f"No {WorkflowFiles.SUITE_RC} or {WorkflowFiles.FLOW_FILE}"
-                    f"found in {self.reg}."
+                    f"found in {self.id_}."
                 )
 
             return dummy_flow({
-                'name': self.reg,
-                'id': self.reg,
+                'name': self.id_,
+                'id': self.id_,
                 'status': message,
                 'stateTotals': {}
             })
         except (ClientError, ClientTimeout) as exc:
             # catch network / client errors
             self.set_header([('workflow_error', str(exc))])
             return False
@@ -477,14 +477,15 @@
                 constructor.
 
                 You will likely need to set `width` and `height` here.
 
                 See `urwid` docs for details.
 
         """
+        # create the overlay
         kwargs = {'width': 'pack', 'height': 'pack', **kwargs}
         overlay = urwid.Overlay(
             urwid.LineBox(
                 urwid.AttrMap(
                     urwid.Frame(
                         urwid.Padding(
                             widget,
@@ -499,17 +500,23 @@
             self.loop.widget,
             align='center',
             valign='middle',
             left=self.stack * 5,
             top=self.stack * 5,
             **kwargs,
         )
+
+        # add it into the overlay stack
         self.loop.widget = overlay
         self.stack += 1
 
+        # force urwid to render the overlay now rather than waiting until the
+        # event loop becomes idle
+        self.loop.draw_screen()
+
     def close_topmost(self):
         """Remove the topmost frame or uit the app if none present."""
         if self.stack <= 0:
             raise urwid.ExitMainLoop()
         self.loop.widget = self.loop.widget[0]
         self.stack -= 1
```

### Comparing `cylc-flow-8.1.4/cylc/flow/tui/data.py` & `cylc-flow-8.2.0/cylc/flow/tui/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from functools import partial
 from subprocess import Popen, PIPE
 import sys
 
 from cylc.flow.exceptions import ClientError
 from cylc.flow.tui.util import (
     extract_context
 )
@@ -80,15 +81,14 @@
     }
   }
 '''
 
 MUTATIONS = {
     'workflow': [
         'pause',
-        'resume',
         'reload',
         'stop',
     ],
     'cycle': [
         'hold',
         'release',
         'kill',
@@ -126,14 +126,54 @@
             result
           }
         }
     '''
 }
 
 
+def cli_cmd(*cmd):
+    """Issue a CLI command.
+
+    Args:
+        cmd:
+            The command without the 'cylc' prefix'.
+
+    Rasies:
+        ClientError:
+            In the event of mishap for consistency with the network
+            client alternative.
+
+    """
+    proc = Popen(  # nosec (command constructed internally, no untrusted input)
+        ['cylc', *cmd],
+        stderr=PIPE,
+        stdout=PIPE,
+        text=True,
+    )
+    out, err = proc.communicate()
+    if proc.returncode != 0:
+        raise ClientError(f'Error in command {" ".join(cmd)}\n{err}')
+
+
+def _clean(workflow):
+    # for now we will exit tui when the workflow is cleaned
+    # this will change when tui supports multiple workflows
+    cli_cmd('clean', workflow)
+    sys.exit(0)
+
+
+OFFLINE_MUTATIONS = {
+    'workflow': {
+        'play': partial(cli_cmd, 'play'),
+        'clean': _clean,
+        'reinstall-reload': partial(cli_cmd, 'vr', '--yes'),
+    }
+}
+
+
 def generate_mutation(mutation, arguments):
     graphql_args = ', '.join([
         f'${argument}: {ARGUMENT_TYPES[argument]}'
         for argument in arguments
     ])
     mutation_args = ', '.join([
         f'{argument}s: ${argument}'
@@ -145,18 +185,24 @@
             {mutation} ({mutation_args}) {{
                 result
             }}
         }}
     '''
 
 
-def list_mutations(selection):
+def list_mutations(client, selection):
     context = extract_context(selection)
     selection_type = list(context)[-1]
-    return MUTATIONS.get(selection_type, [])
+    ret = []
+    if client:
+        # add the online mutations
+        ret.extend(MUTATIONS.get(selection_type, []))
+    # add the offline mutations
+    ret.extend(OFFLINE_MUTATIONS.get(selection_type, []))
+    return sorted(ret)
 
 
 def context_to_variables(context):
     """Derive multiple selection out of single selection.
 
     Examples:
         >>> context_to_variables(extract_context(['~a/b//c/d']))
@@ -177,14 +223,26 @@
         ]
     elif 'cycle' in context:
         variables['task'] = [f'{context["cycle"][0]}/*']
     return variables
 
 
 def mutate(client, mutation, selection):
+    if mutation in OFFLINE_MUTATIONS['workflow']:
+        offline_mutate(mutation, selection)
+    elif client:
+        online_mutate(client, mutation, selection)
+    else:
+        raise Exception(
+            f'Cannot peform command {mutation} on a stopped workflow'
+            ' or invalid command.'
+        )
+
+
+def online_mutate(client, mutation, selection):
     """Issue a mutation over a network interface."""
     context = extract_context(selection)
     variables = context_to_variables(context)
     request_string = generate_mutation(mutation, variables)
     client(
         'graphql',
         {
@@ -195,43 +253,9 @@
 
 
 def offline_mutate(mutation, selection):
     """Issue a mutation over the CLI or other offline interface."""
     context = extract_context(selection)
     variables = context_to_variables(context)
     for workflow in variables['workflow']:
-        if mutation == 'play':
-            cli_cmd('play', workflow)
-        elif mutation == 'clean':  # noqa: SIM106
-            cli_cmd('clean', workflow)
-            # tui only supports single-workflow display ATM so
-            # clean should shut down the program
-            sys.exit()
-        elif mutation in list_mutations(selection):  # noqa: SIM106
-            # this is an "online" mutation -> ignore
-            pass
-        else:
-            raise Exception(f'Invalid mutation: {mutation}')
-
-
-def cli_cmd(*cmd):
-    """Issue a CLI command.
-
-    Args:
-        cmd:
-            The command without the 'cylc' prefix'.
-
-    Rasies:
-        ClientError:
-            In the event of mishap for consistency with the network
-            client alternative.
-
-    """
-    proc = Popen(  # nosec (command constructed internally, no untrusted input)
-        ['cylc', *cmd],
-        stderr=PIPE,
-        stdout=PIPE,
-        text=True,
-    )
-    out, err = proc.communicate()
-    if proc.returncode != 0:
-        raise ClientError(err)
+        # NOTE: this currently only supports workflow mutations
+        OFFLINE_MUTATIONS['workflow'][mutation](workflow)
```

### Comparing `cylc-flow-8.1.4/cylc/flow/tui/overlay.py` & `cylc-flow-8.2.0/cylc/flow/tui/overlay.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     JOB_COLOURS,
     JOB_ICON,
     TUI
 )
 from cylc.flow.tui.data import (
     list_mutations,
     mutate,
-    offline_mutate,
 )
 from cylc.flow.tui.util import (
     get_task_icon
 )
 
 
 def filter_task_state(app):
@@ -214,24 +213,22 @@
 def context(app):
     """An overlay for context menus."""
     value = app.tree_walker.get_focus()[0].get_node().get_value()
     selection = [value['id_']]  # single selection ATM
 
     def _mutate(mutation, _):
         nonlocal app
+        app.open_overlay(partial(progress, text='Running Command'))
         try:
-            if app.client:
-                mutate(app.client, mutation, selection)
-            else:
-                offline_mutate(mutation, selection)
+            mutate(app.client, mutation, selection)
         except ClientError as exc:
-            # app.set_header([('workflow_error', str(exc))])
             app.open_overlay(partial(error, text=str(exc)))
         else:
             app.close_topmost()
+            app.close_topmost()
 
     widget = urwid.ListBox(
         urwid.SimpleFocusListWalker(
             [
                 urwid.Text(f'id: {value["id_"]}'),
                 urwid.Divider(),
                 urwid.Text('Action'),
@@ -241,32 +238,38 @@
                 ),
                 urwid.Divider()
             ] + [
                 urwid.Button(
                     mutation,
                     on_press=partial(_mutate, mutation)
                 )
-                for mutation in (
-                    list_mutations(selection)
-                    if app.client
-                    else ['play', 'clean']
-                )
+                for mutation in list_mutations(app.client, selection)
             ]
         )
     )
 
     return (
         widget,
-        {'width': 30, 'height': 15}
+        {'width': 30, 'height': 20}
     )
 
 
 def error(app, text=''):
     """An overlay for unexpected errors."""
     return (
         urwid.ListBox([
             urwid.Text('Error'),
             urwid.Divider(),
             urwid.Text(text),
         ]),
         {'width': 50, 'height': 40}
     )
+
+
+def progress(app, text='Working'):
+    """An overlay for presenting a running action."""
+    return (
+        urwid.ListBox([
+            urwid.Text(text),
+        ]),
+        {'width': 30, 'height': 10}
+    )
```

### Comparing `cylc-flow-8.1.4/cylc/flow/tui/tree.py` & `cylc-flow-8.2.0/cylc/flow/tui/tree.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/tui/util.py` & `cylc-flow-8.2.0/cylc/flow/tui/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/unicode_rules.py` & `cylc-flow-8.2.0/cylc/flow/unicode_rules.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import re
 
 from cylc.flow.task_id import (
     _TASK_NAME_CHARACTERS,
     _TASK_NAME_PREFIX,
 )
+from cylc.flow.task_qualifiers import TASK_QUALIFIERS
 
 ENGLISH_REGEX_MAP = {
     r'\w': 'alphanumeric',
     r'a-zA-Z0-9': 'latin letters and numbers',
     r'\d': 'numbers',
     r'\-': '``-``',
     r'\.': '``.``',
@@ -171,38 +172,79 @@
     """
     return (
         re.compile(rf'^(?!{re.escape(string)})'),
         f'cannot start with: ``{string}``'
     )
 
 
-def not_equals(string):
-    """Restrict entire string.
+def _human_format_list(lst):
+    """Write a list in plain text.
+
+    Examples:
+        >>> _human_format_list(['a'])
+        'a'
+        >>> _human_format_list(['a', 'b'])
+        'a or b'
+        >>> _human_format_list(['a', 'b', 'c'])
+        'a, b or c'
+
+    """
+    if len(lst) > 1:
+        return ', '.join(lst[:-1]) + f' or {lst[-1]}'
+    return lst[0]
+
+
+def _re_format_list(lst):
+    """Write a list in regex format.
+
+    Examples:
+        >>> _re_format_list('a')
+        '(a)'
+        >>> _re_format_list(['a', 'b'])
+        '(a|b)'
+        >>> _re_format_list(['a', 'b', 'c'])
+        '(a|b|c)'
+
+    """
+    return f"({'|'.join(map(re.escape, lst))})"
+
+
+def not_equals(*strings):
+    r"""Restrict entire string.
 
     Example:
         Regular usage:
         >>> regex, message = not_equals('foo')
         >>> message
         'cannot be: ``foo``'
-        >>> bool(regex.match('foot'))
+        >>> bool(regex.match('foot'))  # "foot" shouldn't match
+        True
+        >>> bool(regex.match('a\nb'))  # newlines should be tolerated
         True
-        >>> bool(regex.match('foo'))
+        >>> bool(regex.match('foo'))   # "foo" should match
         False
 
+        Regular use (multi):
+        >>> regex, message = not_equals('foo', 'bar', 'baz')
+        >>> regex.pattern
+        '^(?!^(foo|bar|baz)$).*$'
+        >>> message
+        'cannot be: ``foo``, ``bar`` or ``baz``'
+
         Note regex chars are escaped automatically:
         >>> regex, message = not_equals('...')
         >>> bool(regex.match('...'))
         False
         >>> bool(regex.match('aaa'))
         True
 
     """
     return (
-        re.compile(rf'^(?!{re.escape(string)}$).*$'),
-        f'cannot be: ``{string}``'
+        re.compile(rf'^(?!^{_re_format_list(strings)}$).*$', re.M),
+        'cannot be: ' + _human_format_list([f'``{s}``' for s in strings])
     )
 
 
 def disallow_char_if_not_at_end_of_first_word(char):
     """Prevent use of a (non-alphanumeric) character unless it occurs directly
     after first word (in which case there is no limit on subsequent
     occurances).
@@ -284,23 +326,36 @@
     ]
 
 
 class TaskMessageValidator(UnicodeRuleChecker):
     """The rules for valid task messages:"""
 
     RULES = [
-        disallow_char_if_not_at_end_of_first_word(':')
+        # <severity>:<message> e.g. "WARN: something went wrong
+        disallow_char_if_not_at_end_of_first_word(':'),
+        # blacklist built-in qualifiers
+        # (technically we need only blacklist task messages, however, to avoid
+        # confusion it's best to blacklist qualifiers too)
+        not_equals(*TASK_QUALIFIERS),
+        not_starts_with('_cylc'),
     ]
 
 
 class TaskOutputValidator(UnicodeRuleChecker):
     """The rules for valid task outputs/message triggers:"""
 
     RULES = [
-        disallowed_characters(':')
+        # restrict outputs to sensible characters
+        allowed_characters(r'\w', r'\d', r'\-', r'\.'),
+        # blacklist the _cylc prefix
+        not_starts_with('_cylc'),
+        # blacklist keywords
+        not_equals('required', 'optional', 'all'),
+        # blacklist built-in task qualifiers
+        not_equals(*TASK_QUALIFIERS),
     ]
 
 
 class TaskNameValidator(UnicodeRuleChecker):
     """The rules for valid task and family names:"""
 
     RULES = [
```

### Comparing `cylc-flow-8.1.4/cylc/flow/util.py` & `cylc-flow-8.2.0/cylc/flow/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/wallclock.py` & `cylc-flow-8.2.0/cylc/flow/wallclock.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/workflow_db_mgr.py` & `cylc-flow-8.2.0/cylc/flow/workflow_db_mgr.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import json
 import os
 from pkg_resources import parse_version
 from shutil import copy, rmtree
 from sqlite3 import OperationalError
 from tempfile import mkstemp
 from typing import (
-    Any, AnyStr, Dict, List, Set, TYPE_CHECKING, Tuple, Union
+    Any, AnyStr, Dict, List, Optional, Set, TYPE_CHECKING, Tuple, Union
 )
 
 from cylc.flow import LOG
 from cylc.flow.broadcast_report import get_broadcast_change_iter
 from cylc.flow.rundb import CylcWorkflowDAO
 from cylc.flow import __version__ as CYLC_VERSION
 from cylc.flow.wallclock import get_current_time_string, get_utc_mode
@@ -165,41 +165,14 @@
             os.rename(temp_pub_db_file_name, self.pub_dao.db_file_name)
             os.chmod(self.pub_dao.db_file_name, st_mode)
         except OSError:
             if os.path.exists(temp_pub_db_file_name):
                 os.remove(temp_pub_db_file_name)
             raise
 
-    def delete_workflow_params(self, *keys):
-        """Schedule deletion of rows from workflow_params table by keys."""
-        for key in keys:
-            self.db_deletes_map[self.TABLE_WORKFLOW_PARAMS].append(
-                {'key': key}
-            )
-
-    def delete_workflow_paused(self):
-        """Delete paused status."""
-        self.delete_workflow_params(self.KEY_PAUSED)
-
-    def delete_workflow_hold_cycle_point(self):
-        """Delete workflow hold cycle point."""
-        self.delete_workflow_params(self.KEY_HOLD_CYCLE_POINT)
-
-    def delete_workflow_stop_clock_time(self):
-        """Delete workflow stop clock time from workflow_params table."""
-        self.delete_workflow_params(self.KEY_STOP_CLOCK_TIME)
-
-    def delete_workflow_stop_cycle_point(self):
-        """Delete workflow stop cycle point from workflow_params table."""
-        self.delete_workflow_params(self.KEY_STOP_CYCLE_POINT)
-
-    def delete_workflow_stop_task(self):
-        """Delete workflow stop task from workflow_params table."""
-        self.delete_workflow_params(self.KEY_STOP_TASK)
-
     def get_pri_dao(self) -> CylcWorkflowDAO:
         """Return the primary DAO.
 
         NOTE: the DAO should be closed after use. You can use this function as
         a context manager, which handles this for you.
         """
         return CylcWorkflowDAO(self.pri_path, create_tables=True)
@@ -341,82 +314,79 @@
         """
         self.db_deletes_map[self.TABLE_WORKFLOW_PARAMS].append({})
         self.db_inserts_map[self.TABLE_WORKFLOW_PARAMS].extend([
             {"key": self.KEY_UUID_STR, "value": schd.uuid_str},
             {"key": self.KEY_CYLC_VERSION, "value": CYLC_VERSION},
             {"key": self.KEY_UTC_MODE, "value": get_utc_mode()},
             {"key": self.KEY_RESTART_COUNT, "value": self.n_restart},
+            {"key": self.KEY_CYCLE_POINT_FORMAT,
+             "value": schd.config.cycle_point_dump_format},
+            {"key": self.KEY_PAUSED, "value": int(schd.is_paused)},
+            {"key": self.KEY_STOP_CLOCK_TIME, "value": schd.stop_clock_time},
+            {"key": self.KEY_STOP_TASK, "value": schd.stop_task},
         ])
-        if schd.config.cycle_point_dump_format is not None:
-            self.put_workflow_params_1(
-                self.KEY_CYCLE_POINT_FORMAT,
-                schd.config.cycle_point_dump_format
-            )
-        if schd.is_paused:
-            self.put_workflow_params_1(self.KEY_PAUSED, 1)
         for key in (
             self.KEY_INITIAL_CYCLE_POINT,
             self.KEY_FINAL_CYCLE_POINT,
             self.KEY_START_CYCLE_POINT,
             self.KEY_STOP_CYCLE_POINT
         ):
             value = getattr(schd.options, key, None)
-            if value is not None and value != 'reload':
-                self.put_workflow_params_1(key, value)
+            value = None if value == 'reload' else value
+            self.put_workflow_params_1(key, value)
         for key in (
             self.KEY_RUN_MODE,
             self.KEY_CYCLE_POINT_TIME_ZONE
         ):
-            value = getattr(schd.options, key, None)
-            if value is not None:
-                self.put_workflow_params_1(key, value)
-        for key in (
-            self.KEY_STOP_CLOCK_TIME,
-            self.KEY_STOP_TASK
-        ):
-            value = getattr(schd, key, None)
-            if value is not None:
-                self.put_workflow_params_1(key, value)
+            self.put_workflow_params_1(key, getattr(schd.options, key, None))
 
     def put_workflow_params_1(
-        self, key: str, value: Union[AnyStr, float]
+        self, key: str, value: Union[AnyStr, float, None]
     ) -> None:
         """Queue insertion of 1 key=value pair to the workflow_params table."""
         self.db_inserts_map[self.TABLE_WORKFLOW_PARAMS].append(
             {"key": key, "value": value}
         )
 
-    def put_workflow_paused(self):
+    def put_workflow_paused(self, value: bool) -> None:
         """Put workflow paused flag to workflow_params table."""
-        self.put_workflow_params_1(self.KEY_PAUSED, 1)
+        self.put_workflow_params_1(self.KEY_PAUSED, int(value))
 
-    def put_workflow_hold_cycle_point(self, value):
+    def put_workflow_hold_cycle_point(
+        self, value: Optional['PointBase']
+    ) -> None:
         """Put workflow hold cycle point to workflow_params table."""
-        self.put_workflow_params_1(self.KEY_HOLD_CYCLE_POINT, str(value))
+        self.put_workflow_params_1(
+            self.KEY_HOLD_CYCLE_POINT,
+            str(value) if value is not None else None
+        )
 
-    def put_workflow_stop_clock_time(self, value):
+    def put_workflow_stop_clock_time(self, value: Optional[str]) -> None:
         """Put workflow stop clock time to workflow_params table."""
         self.put_workflow_params_1(self.KEY_STOP_CLOCK_TIME, value)
 
-    def put_workflow_stop_cycle_point(self, value):
+    def put_workflow_stop_cycle_point(self, value: Optional[str]) -> None:
         """Put workflow stop cycle point to workflow_params table."""
         self.put_workflow_params_1(self.KEY_STOP_CYCLE_POINT, value)
 
-    def put_workflow_stop_task(self, value):
+    def put_workflow_stop_task(self, value: Optional[str]) -> None:
         """Put workflow stop task to workflow_params table."""
         self.put_workflow_params_1(self.KEY_STOP_TASK, value)
 
-    def put_workflow_template_vars(self, template_vars):
+    def put_workflow_template_vars(
+        self, template_vars: Dict[str, Any]
+    ) -> None:
         """Put template_vars in runtime database.
 
         This method queues the relevant insert statements.
         """
-        for key, value in template_vars.items():
-            self.db_inserts_map[self.TABLE_WORKFLOW_TEMPLATE_VARS].append(
-                {"key": key, "value": repr(value)})
+        self.db_inserts_map[self.TABLE_WORKFLOW_TEMPLATE_VARS].extend(
+            {"key": key, "value": repr(value)}
+            for key, value in template_vars.items()
+        )
 
     def put_task_event_timers(self, task_events_mgr):
         """Put statements to update the task_action_timers table."""
         if task_events_mgr.event_timers_updated:
             self.db_deletes_map[self.TABLE_TASK_ACTION_TIMERS].append({})
             for key, timer in task_events_mgr._event_timers.items():
                 key1, point, name, submit_num = key
```

### Comparing `cylc-flow-8.1.4/cylc/flow/workflow_events.py` & `cylc-flow-8.2.0/cylc/flow/workflow_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,15 @@
     EVENT_STARTUP = 'startup'
     EVENT_SHUTDOWN = 'shutdown'
     EVENT_ABORTED = 'abort'
     EVENT_WORKFLOW_TIMEOUT = 'workflow timeout'
     EVENT_INACTIVITY_TIMEOUT = 'inactivity timeout'
     EVENT_STALL = 'stall'
     EVENT_STALL_TIMEOUT = 'stall timeout'
+    EVENT_RESTART_TIMEOUT = 'restart timeout'
 
     WORKFLOW_EVENT_HANDLER = 'workflow-event-handler'
     WORKFLOW_EVENT_MAIL = 'workflow-event-mail'
 
     def __init__(self, proc_pool):
         self.proc_pool = proc_pool
```

### Comparing `cylc-flow-8.1.4/cylc/flow/workflow_status.py` & `cylc-flow-8.2.0/cylc/flow/workflow_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,17 @@
     """
     status = WorkflowStatus.RUNNING
     status_msg = ''
 
     if schd.stop_mode is not None:
         status = WorkflowStatus.STOPPING
         status_msg = f'stopping: {schd.stop_mode.explain()}'
+    elif schd.reload_pending:
+        status = WorkflowStatus.PAUSED
+        status_msg = f'reloading: {schd.reload_pending}'
     elif schd.is_stalled:
         status_msg = 'stalled'
     elif schd.is_paused:
         status = WorkflowStatus.PAUSED
         status_msg = 'paused'
     elif schd.pool.hold_point:
         status_msg = (
```

### Comparing `cylc-flow-8.1.4/cylc/flow/xtrigger_mgr.py` & `cylc-flow-8.2.0/cylc/flow/xtrigger_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/xtriggers/__init__.py` & `cylc-flow-8.2.0/cylc/flow/xtriggers/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/xtriggers/echo.py` & `cylc-flow-8.2.0/cylc/flow/xtriggers/echo.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/xtriggers/wall_clock.py` & `cylc-flow-8.2.0/cylc/flow/xtriggers/wall_clock.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/xtriggers/workflow_state.py` & `cylc-flow-8.2.0/cylc/flow/xtriggers/workflow_state.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc/flow/xtriggers/xrandom.py` & `cylc-flow-8.2.0/cylc/flow/xtriggers/xrandom.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.4/cylc_flow.egg-info/PKG-INFO` & `cylc-flow-8.2.0/cylc_flow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-flow
-Version: 8.1.4
+Version: 8.2.0
 Summary: A workflow engine for cycling systems
 Home-page: https://cylc.org/
 Author: Hilary Oliver
 License: GPL
 Project-URL: Documentation, https://cylc.github.io/cylc-doc/stable/html/index.html
 Project-URL: Source, https://github.com/cylc/cylc-flow
 Project-URL: Tracker, https://github.com/cylc/cylc-flow/issues
@@ -18,14 +18,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: empy
 Provides-Extra: graph
@@ -90,14 +91,20 @@
 cylc install example
 cylc play example
 
 # watch it run
 cylc tui example
 ```
 
+### The Cylc Ecosystem
+
+- [cylc-flow](https://github.com/cylc/cylc-flow) - The core Cylc Scheduler for defining and running workflows.
+- [cylc-uiserver](https://github.com/cylc/cylc-uiserver) - The web-based Cylc graphical user interface for monitoring and controlling workflows.
+- [cylc-rose](https://github.com/cylc/cylc-rose) - Provides integration with [Rose](http://metomi.github.io/rose/).
+
 ### Migrating From Cylc 7
 
 [Migration Guide](https://cylc.github.io/cylc-doc/stable/html/7-to-8/index.html)
 | [Migration Support](https://cylc.discourse.group/c/cylc/7-to-8/13)
 
 Cylc 8 can run most Cylc 7 workflows in compatibility mode with little to no
 changes, go through the
@@ -154,9 +161,7 @@
 * Read the [contributing](CONTRIBUTING.md) page.
 * Development setup instructions are in the
   [developer docs](https://cylc.github.io/cylc-admin/#cylc-8-developer-docs).
 * Involved change proposals can be found in the
   [admin pages](https://cylc.github.io/cylc-admin/#change-proposals).
 * Touch base in the
   [developers chat](https://matrix.to/#/#cylc-general:matrix.org).
-
-
```

### Comparing `cylc-flow-8.1.4/cylc_flow.egg-info/SOURCES.txt` & `cylc-flow-8.2.0/cylc_flow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.cfg
 setup.py
 cylc/flow/__init__.py
 cylc/flow/async_util.py
 cylc/flow/broadcast_mgr.py
 cylc/flow/broadcast_report.py
 cylc/flow/c3mro.py
+cylc/flow/clean.py
 cylc/flow/command_polling.py
 cylc/flow/config.py
 cylc/flow/context_node.py
 cylc/flow/cylc_subproc.py
 cylc/flow/daemonize.py
 cylc/flow/data_messages_pb2.py
 cylc/flow/data_store_mgr.py
@@ -22,14 +23,15 @@
 cylc/flow/graph_parser.py
 cylc/flow/graphnode.py
 cylc/flow/host_select.py
 cylc/flow/hostuserutil.py
 cylc/flow/id.py
 cylc/flow/id_cli.py
 cylc/flow/id_match.py
+cylc/flow/install.py
 cylc/flow/job_file.py
 cylc/flow/job_runner_mgr.py
 cylc/flow/listify.py
 cylc/flow/log_diagnosis.py
 cylc/flow/loggingutil.py
 cylc/flow/option_parsers.py
 cylc/flow/param_expand.py
@@ -51,14 +53,15 @@
 cylc/flow/task_id.py
 cylc/flow/task_job_logs.py
 cylc/flow/task_job_mgr.py
 cylc/flow/task_message.py
 cylc/flow/task_outputs.py
 cylc/flow/task_pool.py
 cylc/flow/task_proxy.py
+cylc/flow/task_qualifiers.py
 cylc/flow/task_remote_cmd.py
 cylc/flow/task_remote_mgr.py
 cylc/flow/task_state.py
 cylc/flow/task_state_prop.py
 cylc/flow/task_trigger.py
 cylc/flow/taskdef.py
 cylc/flow/templatevars.py
```

### Comparing `cylc-flow-8.1.4/cylc_flow.egg-info/entry_points.txt` & `cylc-flow-8.2.0/cylc_flow.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -61,11 +61,7 @@
 log_db = cylc.flow.main_loop.log_db [main_loop-log_db]
 log_main_loop = cylc.flow.main_loop.log_main_loop [main_loop-log_main_loop]
 log_memory = cylc.flow.main_loop.log_memory [main_loop-log_memory]
 reset_bad_hosts = cylc.flow.main_loop.reset_bad_hosts
 
 [cylc.post_install]
 log_vc_info = cylc.flow.install_plugins.log_vc_info:main
-
-[cylc.pre_configure]
-
-
```

### Comparing `cylc-flow-8.1.4/cylc_flow.egg-info/requires.txt` & `cylc-flow-8.2.0/cylc_flow.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-aiofiles==0.7.*
 ansimarkup>=1.0.0
 async-timeout>=3.0.0
 colorama<=1,>=0.4
 graphene<3,>=2.1
 jinja2==3.0.*
 metomi-isodatetime==1!3.0.*
 protobuf<4.22.0,>=4.21.2
 psutil>=5.6.0
-pyzmq==22.*
-setuptools<67,>=49
+pyzmq>=22
+setuptools!=67.*,>=49
 urwid==2.*
 rx
 promise
 
 [:python_version < "3.11"]
 tomli>=2
 
@@ -21,19 +20,15 @@
 
 [all]
 EmPy==3.3.*
 pillow
 pympler
 matplotlib
 sqlparse
-matplotlib
-pympler
-matplotlib
 pandas==1.*
-matplotlib
 async_generator
 bandit>=1.7.0
 coverage>=5.0.0
 flake8-broken-line>=0.3.0
 flake8-bugbear>=21.0.0
 flake8-builtins>=1.5.0
 flake8-comprehensions>=3.5.0
@@ -45,22 +40,19 @@
 pytest-asyncio>=0.17
 pytest-cov>=2.8.0
 pytest-xdist>=2
 pytest-env>=0.6.2
 pytest-mock>=3.6.1
 pytest>=6
 testfixtures>=6.11.0
-types-aiofiles>=0.7.0
 types-Jinja2>=0.1.3
-types-aiofiles>=0.1.3
 types-pkg_resources>=0.1.2
 types-protobuf>=0.1.10
 types-six>=0.1.6
 typing-extensions>=4
-pillow
 requests
 
 [empy]
 EmPy==3.3.*
 
 [graph]
 pillow
@@ -99,17 +91,15 @@
 pytest-asyncio>=0.17
 pytest-cov>=2.8.0
 pytest-xdist>=2
 pytest-env>=0.6.2
 pytest-mock>=3.6.1
 pytest>=6
 testfixtures>=6.11.0
-types-aiofiles>=0.7.0
 types-Jinja2>=0.1.3
-types-aiofiles>=0.1.3
 types-pkg_resources>=0.1.2
 types-protobuf>=0.1.10
 types-six>=0.1.6
 typing-extensions>=4
 
 [tutorials]
 pillow
```

### Comparing `cylc-flow-8.1.4/setup.cfg` & `cylc-flow-8.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -31,34 +31,34 @@
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Scientific/Engineering :: Atmospheric Science
 
 [options]
 packages = find_namespace:
 include_package_data = True
 python_requires = >=3.7
 install_requires = 
-	aiofiles==0.7.*
 	ansimarkup>=1.0.0
 	async-timeout>=3.0.0
 	colorama>=0.4,<=1
 	graphene>=2.1,<3
 	jinja2==3.0.*
 	metomi-isodatetime==1!3.0.*
 	protobuf>=4.21.2,<4.22.0
 	psutil>=5.6.0
-	pyzmq==22.*
-	setuptools>=49, <67
+	pyzmq>=22
+	setuptools>=49,!=67.*
 	importlib_metadata; python_version < "3.8"
 	urwid==2.*
 	rx
 	promise
 	tomli>=2; python_version < "3.11"
 
 [options.packages.find]
@@ -98,17 +98,15 @@
 	pytest-asyncio>=0.17
 	pytest-cov>=2.8.0
 	pytest-xdist>=2
 	pytest-env>=0.6.2
 	pytest-mock>=3.6.1
 	pytest>=6
 	testfixtures>=6.11.0
-	types-aiofiles>=0.7.0
 	types-Jinja2>=0.1.3
-	types-aiofiles>=0.1.3
 	types-pkg_resources>=0.1.2
 	types-protobuf>=0.1.10
 	types-six>=0.1.6
 	typing-extensions>=4
 tutorials = 
 	pillow
 	requests
```

### Comparing `cylc-flow-8.1.4/setup.py` & `cylc-flow-8.2.0/setup.py`

 * *Files identical despite different names*

