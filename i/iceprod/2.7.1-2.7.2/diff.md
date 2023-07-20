# Comparing `tmp/iceprod-2.7.1.tar.gz` & `tmp/iceprod-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iceprod-2.7.1.tar", last modified: Mon Jul 17 21:10:48 2023, max compression
+gzip compressed data, was "iceprod-2.7.2.tar", last modified: Thu Jul 20 23:21:11 2023, max compression
```

## Comparing `iceprod-2.7.1.tar` & `iceprod-2.7.2.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.290387 iceprod-2.7.1/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-07-17 21:10:44.000000 iceprod-2.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2634 2023-07-17 21:10:48.290387 iceprod-2.7.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1774 2023-07-17 21:10:44.000000 iceprod-2.7.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.258387 iceprod-2.7.1/bin/
--rwxr-xr-x   0 root         (0) root         (0)    10083 2023-07-17 21:10:44.000000 iceprod-2.7.1/bin/basic_submit.py
--rwxr-xr-x   0 root         (0) root         (0)     1331 2023-07-17 21:10:44.000000 iceprod-2.7.1/bin/iceprod_add_site_to_master.py
--rwxr-xr-x   0 root         (0) root         (0)     1408 2023-07-17 21:10:44.000000 iceprod-2.7.1/bin/iceprod_debugger.py
--rwxr-xr-x   0 root         (0) root         (0)     1095 2023-07-17 21:10:44.000000 iceprod-2.7.1/bin/iceprod_gridftp_proxy.py
--rwxr-xr-x   0 root         (0) root         (0)     1330 2023-07-17 21:10:44.000000 iceprod-2.7.1/bin/iceprod_join_pool.py
--rwxr-xr-x   0 root         (0) root         (0)     3330 2023-07-17 21:10:44.000000 iceprod-2.7.1/bin/iceprod_rest.py
--rwxr-xr-x   0 root         (0) root         (0)     4606 2023-07-17 21:10:44.000000 iceprod-2.7.1/bin/iceprod_server.py
--rwxr-xr-x   0 root         (0) root         (0)     7147 2023-07-17 21:10:44.000000 iceprod-2.7.1/bin/iceprodsh
--rwxr-xr-x   0 root         (0) root         (0)     3697 2023-07-17 21:10:44.000000 iceprod-2.7.1/bin/loader.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.262387 iceprod-2.7.1/iceprod/
--rw-r--r--   0 root         (0) root         (0)      625 2023-07-17 21:10:45.000000 iceprod-2.7.1/iceprod/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/client_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.266387 iceprod-2.7.1/iceprod/core/
--rw-r--r--   0 root         (0) root         (0)     2295 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5339 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/data_transfer.py
--rw-r--r--   0 root         (0) root         (0)    33372 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/dataclasses.py
--rw-r--r--   0 root         (0) root         (0)      591 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/defaults.py
--rw-r--r--   0 root         (0) root         (0)    45616 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/exe.py
--rw-r--r--   0 root         (0) root         (0)     4147 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/exe_helper.py
--rw-r--r--   0 root         (0) root         (0)    18581 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/exe_json.py
--rw-r--r--   0 root         (0) root         (0)     4927 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/file_catalog.py
--rw-r--r--   0 root         (0) root         (0)    15935 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/functions.py
--rw-r--r--   0 root         (0) root         (0)    16121 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/gridftp.py
--rw-r--r--   0 root         (0) root         (0)    21592 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/i3exec.py
--rw-r--r--   0 root         (0) root         (0)     6108 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/jsonUtil.py
--rw-r--r--   0 root         (0) root         (0)     4035 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/logger.py
--rw-r--r--   0 root         (0) root         (0)    20137 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/parser.py
--rw-r--r--   0 root         (0) root         (0)    25463 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/pilot.py
--rw-r--r--   0 root         (0) root         (0)    30084 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/resources.py
--rw-r--r--   0 root         (0) root         (0)     1949 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/serialization.py
--rw-r--r--   0 root         (0) root         (0)      556 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.270387 iceprod-2.7.1/iceprod/credentials/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/credentials/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1059 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/credentials/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2985 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/credentials/client.py
--rw-r--r--   0 root         (0) root         (0)    19558 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/credentials/server.py
--rw-r--r--   0 root         (0) root         (0)     6689 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/credentials/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.270387 iceprod-2.7.1/iceprod/materialization/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/materialization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1059 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/materialization/__main__.py
--rw-r--r--   0 root         (0) root         (0)    13731 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/materialization/materialize.py
--rw-r--r--   0 root         (0) root         (0)    14142 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/materialization/server.py
--rw-r--r--   0 root         (0) root         (0)     3247 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/materialization/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.270387 iceprod-2.7.1/iceprod/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.270387 iceprod-2.7.1/iceprod/rest/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1059 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/__main__.py
--rw-r--r--   0 root         (0) root         (0)     4892 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/auth.py
--rw-r--r--   0 root         (0) root         (0)     1829 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/base_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.274387 iceprod-2.7.1/iceprod/rest/handlers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6059 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/auth.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/config.py
--rw-r--r--   0 root         (0) root         (0)    12602 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/datasets.py
--rw-r--r--   0 root         (0) root         (0)     3804 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/grids.py
--rw-r--r--   0 root         (0) root         (0)    10884 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/jobs.py
--rw-r--r--   0 root         (0) root         (0)    11679 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/logs.py
--rw-r--r--   0 root         (0) root         (0)     5706 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/pilots.py
--rw-r--r--   0 root         (0) root         (0)     7201 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/task_stats.py
--rw-r--r--   0 root         (0) root         (0)    39857 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/tasks.py
--rw-r--r--   0 root         (0) root         (0)     5278 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/server.py
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/roles_groups.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.278387 iceprod-2.7.1/iceprod/server/
--rw-r--r--   0 root         (0) root         (0)     7572 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8125 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/config.py
--rw-r--r--   0 root         (0) root         (0)     6025 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.254387 iceprod-2.7.1/iceprod/server/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.278387 iceprod-2.7.1/iceprod/server/data/etc/
--rw-r--r--   0 root         (0) root         (0)     1272 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/etc/config_defaults.json
--rw-r--r--   0 root         (0) root         (0)     1820 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/etc/iceprod_schema.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.282387 iceprod-2.7.1/iceprod/server/data/www/
--rw-r--r--   0 root         (0) root         (0)     8624 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/base.css
--rw-r--r--   0 root         (0) root         (0)    13205 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/chart.stackedarea.js
--rw-r--r--   0 root         (0) root         (0)      646 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/chosen-sprite.png
--rw-r--r--   0 root         (0) root         (0)      872 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/chosen-sprite@2x.png
--rw-r--r--   0 root         (0) root         (0)    26966 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/chosen.jquery.min.js
--rw-r--r--   0 root         (0) root         (0)    10751 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/chosen.min.css
--rw-r--r--   0 root         (0) root         (0)      643 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/documentation.css
--rw-r--r--   0 root         (0) root         (0)     1591 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/documentation.js
--rw-r--r--   0 root         (0) root         (0)     1150 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/favicon.ico
--rw-r--r--   0 root         (0) root         (0)      211 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/favicon.png
--rw-r--r--   0 root         (0) root         (0)    13277 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/fetch.js
--rw-r--r--   0 root         (0) root         (0)     1493 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/json-rpc.js
--rw-r--r--   0 root         (0) root         (0)     8775 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/jsonlint.js
--rw-r--r--   0 root         (0) root         (0)    46933 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/jsviews.min.js
--rw-r--r--   0 root         (0) root         (0)     3842 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/logo_155x60.png
--rw-r--r--   0 root         (0) root         (0)    10659 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/rest.js
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/robots.txt
--rw-r--r--   0 root         (0) root         (0)     5218 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/submit.css
--rw-r--r--   0 root         (0) root         (0)    29484 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/submit.js
--rw-r--r--   0 root         (0) root         (0)     7716 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/util.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.286387 iceprod-2.7.1/iceprod/server/data/www_templates/
--rw-r--r--   0 root         (0) root         (0)      315 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/404.html
--rw-r--r--   0 root         (0) root         (0)     3124 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/base.html
--rw-r--r--   0 root         (0) root         (0)     1417 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/dataset_browse.html
--rw-r--r--   0 root         (0) root         (0)     4467 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/dataset_detail.html
--rw-r--r--   0 root         (0) root         (0)     2659 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/groups.html
--rw-r--r--   0 root         (0) root         (0)     2285 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/job_browse.html
--rw-r--r--   0 root         (0) root         (0)     2255 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/job_detail.html
--rw-r--r--   0 root         (0) root         (0)      611 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/login.html
--rw-r--r--   0 root         (0) root         (0)      183 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/logout.html
--rw-r--r--   0 root         (0) root         (0)      352 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/main.html
--rw-r--r--   0 root         (0) root         (0)     6133 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/profile.html
--rw-r--r--   0 root         (0) root         (0)     2121 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/site.html
--rw-r--r--   0 root         (0) root         (0)     6626 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/submit.html
--rw-r--r--   0 root         (0) root         (0)     1790 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/task_browse.html
--rw-r--r--   0 root         (0) root         (0)     4893 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/task_detail.html
--rw-r--r--   0 root         (0) root         (0)      360 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/tasks.html
--rw-r--r--   0 root         (0) root         (0)     4547 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/dataset_prio.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/documentation.py
--rw-r--r--   0 root         (0) root         (0)     3501 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/globus.py
--rw-r--r--   0 root         (0) root         (0)    30710 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/grid.py
--rw-r--r--   0 root         (0) root         (0)     6785 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.286387 iceprod-2.7.1/iceprod/server/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8067 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/modules/queue.py
--rw-r--r--   0 root         (0) root         (0)     1148 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/modules/schedule.py
--rw-r--r--   0 root         (0) root         (0)    30111 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/modules/website.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.286387 iceprod-2.7.1/iceprod/server/plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11131 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/plugins/condor.py
--rw-r--r--   0 root         (0) root         (0)    47259 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/plugins/condor_direct.py
--rw-r--r--   0 root         (0) root         (0)     2463 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/plugins/condor_file_transfer.py
--rw-r--r--   0 root         (0) root         (0)    33448 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/plugins/sc_demo.py
--rw-r--r--   0 root         (0) root         (0)    10523 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/plugins/supercomp_cedar.py
--rw-r--r--   0 root         (0) root         (0)    22909 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/plugins/supercomp_graham.py
--rw-r--r--   0 root         (0) root         (0)    10177 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/priority.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.290387 iceprod-2.7.1/iceprod/server/scheduled_tasks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2927 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/buffer_jobs_tasks.py
--rw-r--r--   0 root         (0) root         (0)     3846 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/dataset_cleanup.py
--rw-r--r--   0 root         (0) root         (0)     3492 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/dataset_completion.py
--rw-r--r--   0 root         (0) root         (0)     5660 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/dataset_monitor.py
--rw-r--r--   0 root         (0) root         (0)     3444 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/job_completion.py
--rw-r--r--   0 root         (0) root         (0)     4904 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/job_temp_cleaning.py
--rw-r--r--   0 root         (0) root         (0)     2088 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/log_cleanup.py
--rw-r--r--   0 root         (0) root         (0)     5274 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/non_active_tasks.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/pilot_cleanup.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/pilot_monitor.py
--rw-r--r--   0 root         (0) root         (0)     5355 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/queue_tasks.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/removed_tasks.py
--rw-r--r--   0 root         (0) root         (0)     3500 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/reset_tasks.py
--rw-r--r--   0 root         (0) root         (0)     3896 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/update_task_priority.py
--rw-r--r--   0 root         (0) root         (0)     3638 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/server.py
--rw-r--r--   0 root         (0) root         (0)     8715 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/ssl_cert.py
--rw-r--r--   0 root         (0) root         (0)     1344 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/task_queue.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.262387 iceprod-2.7.1/iceprod.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2634 2023-07-17 21:10:48.000000 iceprod-2.7.1/iceprod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4828 2023-07-17 21:10:48.000000 iceprod-2.7.1/iceprod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 21:10:48.000000 iceprod-2.7.1/iceprod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      368 2023-07-17 21:10:48.000000 iceprod-2.7.1/iceprod.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-17 21:10:48.000000 iceprod-2.7.1/iceprod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2090 2023-07-17 21:10:48.294387 iceprod-2.7.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      224 2023-07-17 21:10:44.000000 iceprod-2.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:21:11.700996 iceprod-2.7.2/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-07-20 23:21:08.000000 iceprod-2.7.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2634 2023-07-20 23:21:11.700996 iceprod-2.7.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1774 2023-07-20 23:21:08.000000 iceprod-2.7.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:21:11.688995 iceprod-2.7.2/bin/
+-rwxr-xr-x   0 root         (0) root         (0)    10083 2023-07-20 23:21:08.000000 iceprod-2.7.2/bin/basic_submit.py
+-rwxr-xr-x   0 root         (0) root         (0)     1331 2023-07-20 23:21:08.000000 iceprod-2.7.2/bin/iceprod_add_site_to_master.py
+-rwxr-xr-x   0 root         (0) root         (0)     1408 2023-07-20 23:21:08.000000 iceprod-2.7.2/bin/iceprod_debugger.py
+-rwxr-xr-x   0 root         (0) root         (0)     1095 2023-07-20 23:21:08.000000 iceprod-2.7.2/bin/iceprod_gridftp_proxy.py
+-rwxr-xr-x   0 root         (0) root         (0)     1330 2023-07-20 23:21:08.000000 iceprod-2.7.2/bin/iceprod_join_pool.py
+-rwxr-xr-x   0 root         (0) root         (0)     3330 2023-07-20 23:21:08.000000 iceprod-2.7.2/bin/iceprod_rest.py
+-rwxr-xr-x   0 root         (0) root         (0)     4606 2023-07-20 23:21:08.000000 iceprod-2.7.2/bin/iceprod_server.py
+-rwxr-xr-x   0 root         (0) root         (0)     7147 2023-07-20 23:21:08.000000 iceprod-2.7.2/bin/iceprodsh
+-rwxr-xr-x   0 root         (0) root         (0)     3697 2023-07-20 23:21:08.000000 iceprod-2.7.2/bin/loader.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:21:11.688995 iceprod-2.7.2/iceprod/
+-rw-r--r--   0 root         (0) root         (0)      625 2023-07-20 23:21:09.000000 iceprod-2.7.2/iceprod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/client_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:21:11.688995 iceprod-2.7.2/iceprod/core/
+-rw-r--r--   0 root         (0) root         (0)     2295 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5339 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/core/data_transfer.py
+-rw-r--r--   0 root         (0) root         (0)    33372 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/core/dataclasses.py
+-rw-r--r--   0 root         (0) root         (0)      591 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/core/defaults.py
+-rw-r--r--   0 root         (0) root         (0)    45616 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/core/exe.py
+-rw-r--r--   0 root         (0) root         (0)     4147 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/core/exe_helper.py
+-rw-r--r--   0 root         (0) root         (0)    18581 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/core/exe_json.py
+-rw-r--r--   0 root         (0) root         (0)     4927 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/core/file_catalog.py
+-rw-r--r--   0 root         (0) root         (0)    15935 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/core/functions.py
+-rw-r--r--   0 root         (0) root         (0)    16121 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/core/gridftp.py
+-rw-r--r--   0 root         (0) root         (0)    21592 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/core/i3exec.py
+-rw-r--r--   0 root         (0) root         (0)     6108 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/core/jsonUtil.py
+-rw-r--r--   0 root         (0) root         (0)     4035 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/core/logger.py
+-rw-r--r--   0 root         (0) root         (0)    20137 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/core/parser.py
+-rw-r--r--   0 root         (0) root         (0)    25463 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/core/pilot.py
+-rw-r--r--   0 root         (0) root         (0)    30084 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/core/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1949 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/core/serialization.py
+-rw-r--r--   0 root         (0) root         (0)      556 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/core/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:21:11.692995 iceprod-2.7.2/iceprod/credentials/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/credentials/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/credentials/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/credentials/client.py
+-rw-r--r--   0 root         (0) root         (0)    19558 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/credentials/server.py
+-rw-r--r--   0 root         (0) root         (0)     6689 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/credentials/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:21:11.692995 iceprod-2.7.2/iceprod/materialization/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/materialization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/materialization/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    13731 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/materialization/materialize.py
+-rw-r--r--   0 root         (0) root         (0)    14142 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/materialization/server.py
+-rw-r--r--   0 root         (0) root         (0)     3247 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/materialization/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:21:11.692995 iceprod-2.7.2/iceprod/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:21:11.692995 iceprod-2.7.2/iceprod/rest/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/rest/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     4892 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/rest/auth.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/rest/base_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:21:11.692995 iceprod-2.7.2/iceprod/rest/handlers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/rest/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6059 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/rest/handlers/auth.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/rest/handlers/config.py
+-rw-r--r--   0 root         (0) root         (0)    12602 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/rest/handlers/datasets.py
+-rw-r--r--   0 root         (0) root         (0)     3804 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/rest/handlers/grids.py
+-rw-r--r--   0 root         (0) root         (0)    10884 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/rest/handlers/jobs.py
+-rw-r--r--   0 root         (0) root         (0)    11679 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/rest/handlers/logs.py
+-rw-r--r--   0 root         (0) root         (0)     5706 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/rest/handlers/pilots.py
+-rw-r--r--   0 root         (0) root         (0)     7201 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/rest/handlers/task_stats.py
+-rw-r--r--   0 root         (0) root         (0)    39857 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/rest/handlers/tasks.py
+-rw-r--r--   0 root         (0) root         (0)     5286 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/rest/server.py
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/roles_groups.py
+-rw-r--r--   0 root         (0) root         (0)     5267 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:21:11.696995 iceprod-2.7.2/iceprod/server/
+-rw-r--r--   0 root         (0) root         (0)     7572 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8125 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/config.py
+-rw-r--r--   0 root         (0) root         (0)     6025 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:21:11.684996 iceprod-2.7.2/iceprod/server/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:21:11.696995 iceprod-2.7.2/iceprod/server/data/etc/
+-rw-r--r--   0 root         (0) root         (0)     1272 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/etc/config_defaults.json
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/etc/iceprod_schema.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:21:11.696995 iceprod-2.7.2/iceprod/server/data/www/
+-rw-r--r--   0 root         (0) root         (0)     8624 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/base.css
+-rw-r--r--   0 root         (0) root         (0)    13205 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/chart.stackedarea.js
+-rw-r--r--   0 root         (0) root         (0)      646 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/chosen-sprite.png
+-rw-r--r--   0 root         (0) root         (0)      872 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/chosen-sprite@2x.png
+-rw-r--r--   0 root         (0) root         (0)    26966 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/chosen.jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)    10751 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/chosen.min.css
+-rw-r--r--   0 root         (0) root         (0)      643 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/documentation.css
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/documentation.js
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)      211 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/favicon.png
+-rw-r--r--   0 root         (0) root         (0)    13277 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/fetch.js
+-rw-r--r--   0 root         (0) root         (0)     1493 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/json-rpc.js
+-rw-r--r--   0 root         (0) root         (0)     8775 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/jsonlint.js
+-rw-r--r--   0 root         (0) root         (0)    46933 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/jsviews.min.js
+-rw-r--r--   0 root         (0) root         (0)     3842 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/logo_155x60.png
+-rw-r--r--   0 root         (0) root         (0)    10659 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/rest.js
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/robots.txt
+-rw-r--r--   0 root         (0) root         (0)     5218 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/submit.css
+-rw-r--r--   0 root         (0) root         (0)    29484 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/submit.js
+-rw-r--r--   0 root         (0) root         (0)     7716 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www/util.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:21:11.700996 iceprod-2.7.2/iceprod/server/data/www_templates/
+-rw-r--r--   0 root         (0) root         (0)      315 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www_templates/404.html
+-rw-r--r--   0 root         (0) root         (0)     3124 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www_templates/base.html
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www_templates/dataset_browse.html
+-rw-r--r--   0 root         (0) root         (0)     4467 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www_templates/dataset_detail.html
+-rw-r--r--   0 root         (0) root         (0)     2659 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www_templates/groups.html
+-rw-r--r--   0 root         (0) root         (0)     2285 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www_templates/job_browse.html
+-rw-r--r--   0 root         (0) root         (0)     2255 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www_templates/job_detail.html
+-rw-r--r--   0 root         (0) root         (0)      611 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www_templates/login.html
+-rw-r--r--   0 root         (0) root         (0)      183 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www_templates/logout.html
+-rw-r--r--   0 root         (0) root         (0)      352 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www_templates/main.html
+-rw-r--r--   0 root         (0) root         (0)     6133 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www_templates/profile.html
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www_templates/site.html
+-rw-r--r--   0 root         (0) root         (0)     6626 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www_templates/submit.html
+-rw-r--r--   0 root         (0) root         (0)     1790 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www_templates/task_browse.html
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www_templates/task_detail.html
+-rw-r--r--   0 root         (0) root         (0)      360 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/data/www_templates/tasks.html
+-rw-r--r--   0 root         (0) root         (0)     4547 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/dataset_prio.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/documentation.py
+-rw-r--r--   0 root         (0) root         (0)     3501 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/globus.py
+-rw-r--r--   0 root         (0) root         (0)    30710 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/grid.py
+-rw-r--r--   0 root         (0) root         (0)     6785 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:21:11.700996 iceprod-2.7.2/iceprod/server/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8067 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/modules/queue.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/modules/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    30111 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/modules/website.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:21:11.700996 iceprod-2.7.2/iceprod/server/plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11131 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/plugins/condor.py
+-rw-r--r--   0 root         (0) root         (0)    47259 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/plugins/condor_direct.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/plugins/condor_file_transfer.py
+-rw-r--r--   0 root         (0) root         (0)    33448 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/plugins/sc_demo.py
+-rw-r--r--   0 root         (0) root         (0)    10523 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/plugins/supercomp_cedar.py
+-rw-r--r--   0 root         (0) root         (0)    22909 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/plugins/supercomp_graham.py
+-rw-r--r--   0 root         (0) root         (0)    10177 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/priority.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:21:11.700996 iceprod-2.7.2/iceprod/server/scheduled_tasks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/scheduled_tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2927 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/scheduled_tasks/buffer_jobs_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     3846 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/scheduled_tasks/dataset_cleanup.py
+-rw-r--r--   0 root         (0) root         (0)     3492 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/scheduled_tasks/dataset_completion.py
+-rw-r--r--   0 root         (0) root         (0)     5660 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/scheduled_tasks/dataset_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     3444 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/scheduled_tasks/job_completion.py
+-rw-r--r--   0 root         (0) root         (0)     7329 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/scheduled_tasks/job_temp_cleaning.py
+-rw-r--r--   0 root         (0) root         (0)     2088 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/scheduled_tasks/log_cleanup.py
+-rw-r--r--   0 root         (0) root         (0)     5274 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/scheduled_tasks/non_active_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/scheduled_tasks/pilot_cleanup.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/scheduled_tasks/pilot_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     5355 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/scheduled_tasks/queue_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/scheduled_tasks/removed_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/scheduled_tasks/reset_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     3896 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/scheduled_tasks/update_task_priority.py
+-rw-r--r--   0 root         (0) root         (0)     3638 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     8715 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/ssl_cert.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/task_queue.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-07-20 23:21:08.000000 iceprod-2.7.2/iceprod/server/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:21:11.688995 iceprod-2.7.2/iceprod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2634 2023-07-20 23:21:11.000000 iceprod-2.7.2/iceprod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4828 2023-07-20 23:21:11.000000 iceprod-2.7.2/iceprod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 23:21:11.000000 iceprod-2.7.2/iceprod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      368 2023-07-20 23:21:11.000000 iceprod-2.7.2/iceprod.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-20 23:21:11.000000 iceprod-2.7.2/iceprod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2090 2023-07-20 23:21:11.704995 iceprod-2.7.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      224 2023-07-20 23:21:08.000000 iceprod-2.7.2/setup.py
```

### Comparing `iceprod-2.7.1/LICENSE` & `iceprod-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/PKG-INFO` & `iceprod-2.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceprod
-Version: 2.7.1
+Version: 2.7.2
 Summary: IceCube dataset management system
 Home-page: https://github.com/WIPACrepo/iceprod
 Download-URL: https://pypi.org/project/iceprod/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/iceprod/issues
```

### Comparing `iceprod-2.7.1/README.rst` & `iceprod-2.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/bin/basic_submit.py` & `iceprod-2.7.2/bin/basic_submit.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/bin/iceprod_add_site_to_master.py` & `iceprod-2.7.2/bin/iceprod_add_site_to_master.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/bin/iceprod_debugger.py` & `iceprod-2.7.2/bin/iceprod_debugger.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/bin/iceprod_gridftp_proxy.py` & `iceprod-2.7.2/bin/iceprod_gridftp_proxy.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/bin/iceprod_join_pool.py` & `iceprod-2.7.2/bin/iceprod_join_pool.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/bin/iceprod_rest.py` & `iceprod-2.7.2/bin/iceprod_rest.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/bin/iceprod_server.py` & `iceprod-2.7.2/bin/iceprod_server.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/bin/iceprodsh` & `iceprod-2.7.2/bin/iceprodsh`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/bin/loader.sh` & `iceprod-2.7.2/bin/loader.sh`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/__init__.py` & `iceprod-2.7.2/iceprod/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "2.7.1"
+__version__ = "2.7.2"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `iceprod-2.7.1/iceprod/client_auth.py` & `iceprod-2.7.2/iceprod/client_auth.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/core/__init__.py` & `iceprod-2.7.2/iceprod/core/__init__.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/core/data_transfer.py` & `iceprod-2.7.2/iceprod/core/data_transfer.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/core/dataclasses.py` & `iceprod-2.7.2/iceprod/core/dataclasses.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/core/defaults.py` & `iceprod-2.7.2/iceprod/core/defaults.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/core/exe.py` & `iceprod-2.7.2/iceprod/core/exe.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/core/exe_helper.py` & `iceprod-2.7.2/iceprod/core/exe_helper.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/core/exe_json.py` & `iceprod-2.7.2/iceprod/core/exe_json.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/core/file_catalog.py` & `iceprod-2.7.2/iceprod/core/file_catalog.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/core/functions.py` & `iceprod-2.7.2/iceprod/core/functions.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/core/gridftp.py` & `iceprod-2.7.2/iceprod/core/gridftp.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/core/i3exec.py` & `iceprod-2.7.2/iceprod/core/i3exec.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/core/jsonUtil.py` & `iceprod-2.7.2/iceprod/core/jsonUtil.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/core/logger.py` & `iceprod-2.7.2/iceprod/core/logger.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/core/parser.py` & `iceprod-2.7.2/iceprod/core/parser.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/core/pilot.py` & `iceprod-2.7.2/iceprod/core/pilot.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/core/resources.py` & `iceprod-2.7.2/iceprod/core/resources.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/core/serialization.py` & `iceprod-2.7.2/iceprod/core/serialization.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/core/util.py` & `iceprod-2.7.2/iceprod/core/util.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/credentials/__main__.py` & `iceprod-2.7.2/iceprod/credentials/__main__.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/credentials/client.py` & `iceprod-2.7.2/iceprod/credentials/client.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/credentials/server.py` & `iceprod-2.7.2/iceprod/credentials/server.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/credentials/service.py` & `iceprod-2.7.2/iceprod/credentials/service.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/materialization/__main__.py` & `iceprod-2.7.2/iceprod/materialization/__main__.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/materialization/materialize.py` & `iceprod-2.7.2/iceprod/materialization/materialize.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/materialization/server.py` & `iceprod-2.7.2/iceprod/materialization/server.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/materialization/service.py` & `iceprod-2.7.2/iceprod/materialization/service.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/rest/__main__.py` & `iceprod-2.7.2/iceprod/rest/__main__.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/rest/auth.py` & `iceprod-2.7.2/iceprod/rest/auth.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/rest/base_handler.py` & `iceprod-2.7.2/iceprod/rest/base_handler.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/rest/handlers/auth.py` & `iceprod-2.7.2/iceprod/rest/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/rest/handlers/config.py` & `iceprod-2.7.2/iceprod/rest/handlers/config.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/rest/handlers/datasets.py` & `iceprod-2.7.2/iceprod/rest/handlers/datasets.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/rest/handlers/grids.py` & `iceprod-2.7.2/iceprod/rest/handlers/grids.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/rest/handlers/jobs.py` & `iceprod-2.7.2/iceprod/rest/handlers/jobs.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/rest/handlers/logs.py` & `iceprod-2.7.2/iceprod/rest/handlers/logs.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/rest/handlers/pilots.py` & `iceprod-2.7.2/iceprod/rest/handlers/pilots.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/rest/handlers/task_stats.py` & `iceprod-2.7.2/iceprod/rest/handlers/task_stats.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/rest/handlers/tasks.py` & `iceprod-2.7.2/iceprod/rest/handlers/tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/rest/server.py` & `iceprod-2.7.2/iceprod/rest/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import pkgutil
 
 import motor.motor_asyncio
 from rest_tools.server import RestServer
 from tornado.web import RequestHandler, HTTPError
 from wipac_dev_tools import from_environment
 
-from ..s3 import boto3, S3, FakeS3
+from ..s3 import boto3, S3
 from ..server.module import FakeStatsClient, StatsClientIgnoreErrors
 from .base_handler import IceProdRestConfig
 
 logger = logging.getLogger('rest-server')
 
 
 class Error(RequestHandler):
@@ -88,15 +88,15 @@
                 statsd = StatsClientIgnoreErrors(addr, port=port, prefix=config['STATSD_PREFIX'])
             except Exception:
                 logger.warning('failed to connect to statsd: %r', config['STATSD_ADDRESS'], exc_info=True)
 
         s3conn = None
         if s3_override:
             logging.warning('S3 in testing mode')
-            s3conn = FakeS3(s3_override)
+            s3conn = S3('', '', '', mock_s3=s3_override)
         elif boto3 and config['S3_ACCESS_KEY'] and config['S3_SECRET_KEY']:
             s3conn = S3(config['S3_ADDRESS'], config['S3_ACCESS_KEY'], config['S3_SECRET_KEY'])
         else:
             logger.warning('S3 is not available!')
 
         logging_url = config["DB_URL"].split('@')[-1] if '@' in config["DB_URL"] else config["DB_URL"]
         logging.info(f'DB: {logging_url}')
```

### Comparing `iceprod-2.7.1/iceprod/server/__init__.py` & `iceprod-2.7.2/iceprod/server/__init__.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/config.py` & `iceprod-2.7.2/iceprod/server/config.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/daemon.py` & `iceprod-2.7.2/iceprod/server/daemon.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/etc/config_defaults.json` & `iceprod-2.7.2/iceprod/server/data/etc/config_defaults.json`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/etc/iceprod_schema.json` & `iceprod-2.7.2/iceprod/server/data/etc/iceprod_schema.json`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www/base.css` & `iceprod-2.7.2/iceprod/server/data/www/base.css`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www/chart.stackedarea.js` & `iceprod-2.7.2/iceprod/server/data/www/chart.stackedarea.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www/chosen-sprite.png` & `iceprod-2.7.2/iceprod/server/data/www/chosen-sprite.png`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www/chosen-sprite@2x.png` & `iceprod-2.7.2/iceprod/server/data/www/chosen-sprite@2x.png`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www/chosen.jquery.min.js` & `iceprod-2.7.2/iceprod/server/data/www/chosen.jquery.min.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www/chosen.min.css` & `iceprod-2.7.2/iceprod/server/data/www/chosen.min.css`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www/documentation.css` & `iceprod-2.7.2/iceprod/server/data/www/documentation.css`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www/documentation.js` & `iceprod-2.7.2/iceprod/server/data/www/documentation.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www/favicon.ico` & `iceprod-2.7.2/iceprod/server/data/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www/fetch.js` & `iceprod-2.7.2/iceprod/server/data/www/fetch.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www/json-rpc.js` & `iceprod-2.7.2/iceprod/server/data/www/json-rpc.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www/jsonlint.js` & `iceprod-2.7.2/iceprod/server/data/www/jsonlint.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www/jsviews.min.js` & `iceprod-2.7.2/iceprod/server/data/www/jsviews.min.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www/logo_155x60.png` & `iceprod-2.7.2/iceprod/server/data/www/logo_155x60.png`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www/rest.js` & `iceprod-2.7.2/iceprod/server/data/www/rest.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www/submit.css` & `iceprod-2.7.2/iceprod/server/data/www/submit.css`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www/submit.js` & `iceprod-2.7.2/iceprod/server/data/www/submit.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www/util.js` & `iceprod-2.7.2/iceprod/server/data/www/util.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www_templates/base.html` & `iceprod-2.7.2/iceprod/server/data/www_templates/base.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www_templates/dataset_browse.html` & `iceprod-2.7.2/iceprod/server/data/www_templates/dataset_browse.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www_templates/dataset_detail.html` & `iceprod-2.7.2/iceprod/server/data/www_templates/dataset_detail.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www_templates/groups.html` & `iceprod-2.7.2/iceprod/server/data/www_templates/groups.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www_templates/job_browse.html` & `iceprod-2.7.2/iceprod/server/data/www_templates/job_browse.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www_templates/job_detail.html` & `iceprod-2.7.2/iceprod/server/data/www_templates/job_detail.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www_templates/login.html` & `iceprod-2.7.2/iceprod/server/data/www_templates/login.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www_templates/profile.html` & `iceprod-2.7.2/iceprod/server/data/www_templates/profile.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www_templates/site.html` & `iceprod-2.7.2/iceprod/server/data/www_templates/site.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www_templates/submit.html` & `iceprod-2.7.2/iceprod/server/data/www_templates/submit.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www_templates/task_browse.html` & `iceprod-2.7.2/iceprod/server/data/www_templates/task_browse.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/data/www_templates/task_detail.html` & `iceprod-2.7.2/iceprod/server/data/www_templates/task_detail.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/dataset_prio.py` & `iceprod-2.7.2/iceprod/server/dataset_prio.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/documentation.py` & `iceprod-2.7.2/iceprod/server/documentation.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/globus.py` & `iceprod-2.7.2/iceprod/server/globus.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/grid.py` & `iceprod-2.7.2/iceprod/server/grid.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/module.py` & `iceprod-2.7.2/iceprod/server/module.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/modules/queue.py` & `iceprod-2.7.2/iceprod/server/modules/queue.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/modules/schedule.py` & `iceprod-2.7.2/iceprod/server/modules/schedule.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/modules/website.py` & `iceprod-2.7.2/iceprod/server/modules/website.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/plugins/condor.py` & `iceprod-2.7.2/iceprod/server/plugins/condor.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/plugins/condor_direct.py` & `iceprod-2.7.2/iceprod/server/plugins/condor_direct.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/plugins/condor_file_transfer.py` & `iceprod-2.7.2/iceprod/server/plugins/condor_file_transfer.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/plugins/sc_demo.py` & `iceprod-2.7.2/iceprod/server/plugins/sc_demo.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/plugins/supercomp_cedar.py` & `iceprod-2.7.2/iceprod/server/plugins/supercomp_cedar.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/plugins/supercomp_graham.py` & `iceprod-2.7.2/iceprod/server/plugins/supercomp_graham.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/priority.py` & `iceprod-2.7.2/iceprod/server/priority.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/scheduled_tasks/buffer_jobs_tasks.py` & `iceprod-2.7.2/iceprod/server/scheduled_tasks/buffer_jobs_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/scheduled_tasks/dataset_cleanup.py` & `iceprod-2.7.2/iceprod/server/scheduled_tasks/dataset_cleanup.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/scheduled_tasks/dataset_completion.py` & `iceprod-2.7.2/iceprod/server/scheduled_tasks/dataset_completion.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/scheduled_tasks/dataset_monitor.py` & `iceprod-2.7.2/iceprod/server/scheduled_tasks/dataset_monitor.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/scheduled_tasks/job_completion.py` & `iceprod-2.7.2/iceprod/server/scheduled_tasks/job_completion.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/scheduled_tasks/log_cleanup.py` & `iceprod-2.7.2/iceprod/server/scheduled_tasks/log_cleanup.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/scheduled_tasks/non_active_tasks.py` & `iceprod-2.7.2/iceprod/server/scheduled_tasks/non_active_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/scheduled_tasks/pilot_cleanup.py` & `iceprod-2.7.2/iceprod/server/scheduled_tasks/pilot_cleanup.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/scheduled_tasks/pilot_monitor.py` & `iceprod-2.7.2/iceprod/server/scheduled_tasks/pilot_monitor.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/scheduled_tasks/queue_tasks.py` & `iceprod-2.7.2/iceprod/server/scheduled_tasks/queue_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/scheduled_tasks/removed_tasks.py` & `iceprod-2.7.2/iceprod/server/scheduled_tasks/removed_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/scheduled_tasks/reset_tasks.py` & `iceprod-2.7.2/iceprod/server/scheduled_tasks/reset_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/scheduled_tasks/update_task_priority.py` & `iceprod-2.7.2/iceprod/server/scheduled_tasks/update_task_priority.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/server.py` & `iceprod-2.7.2/iceprod/server/server.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/ssl_cert.py` & `iceprod-2.7.2/iceprod/server/ssl_cert.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/task_queue.py` & `iceprod-2.7.2/iceprod/server/task_queue.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod/server/util.py` & `iceprod-2.7.2/iceprod/server/util.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/iceprod.egg-info/PKG-INFO` & `iceprod-2.7.2/iceprod.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceprod
-Version: 2.7.1
+Version: 2.7.2
 Summary: IceCube dataset management system
 Home-page: https://github.com/WIPACrepo/iceprod
 Download-URL: https://pypi.org/project/iceprod/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/iceprod/issues
```

### Comparing `iceprod-2.7.1/iceprod.egg-info/SOURCES.txt` & `iceprod-2.7.2/iceprod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.1/setup.cfg` & `iceprod-2.7.2/setup.cfg`

 * *Files identical despite different names*

