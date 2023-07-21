# Comparing `tmp/remoulade-1.2.4.tar.gz` & `tmp/remoulade-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remoulade-1.2.4.tar", last modified: Wed Jul  5 09:58:07 2023, max compression
+gzip compressed data, was "remoulade-2.0.0.tar", last modified: Fri Jul 21 14:53:58 2023, max compression
```

## Comparing `remoulade-1.2.4.tar` & `remoulade-2.0.0.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:58:07.536289 remoulade-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-05 09:57:51.000000 remoulade-1.2.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-07-05 09:57:51.000000 remoulade-1.2.4/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-05 09:57:51.000000 remoulade-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-05 09:58:07.536289 remoulade-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-05 09:57:51.000000 remoulade-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:58:07.512289 remoulade-1.2.4/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      275 2023-07-05 09:57:51.000000 remoulade-1.2.4/bin/remoulade-gevent
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-05 09:57:51.000000 remoulade-1.2.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:58:07.516289 remoulade-1.2.4/remoulade/
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/actor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:58:07.520289 remoulade-1.2.4/remoulade/api/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/api/apispec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/api/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/api/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    17143 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:58:07.520289 remoulade-1.2.4/remoulade/brokers/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/brokers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/brokers/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    21648 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/brokers/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/brokers/stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:58:07.524289 remoulade-1.2.4/remoulade/cancel/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/cancel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/cancel/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:58:07.524289 remoulade-1.2.4/remoulade/cancel/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/cancel/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/cancel/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/cancel/backends/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/cancel/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/cancel/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:58:07.524289 remoulade-1.2.4/remoulade/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/cli/remoulade_ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/cli/remoulade_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/cli/remoulade_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/collection_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:58:07.524289 remoulade-1.2.4/remoulade/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/helpers/actor_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/helpers/backoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/helpers/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/helpers/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:58:07.532289 remoulade-1.2.4/remoulade/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/middleware/age_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/middleware/catch_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/middleware/current_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/middleware/logging_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/middleware/max_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/middleware/max_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/middleware/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/middleware/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/middleware/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/middleware/retries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/middleware/shutdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/middleware/threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/middleware/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:58:07.532289 remoulade-1.2.4/remoulade/rate_limits/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/rate_limits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/rate_limits/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:58:07.532289 remoulade-1.2.4/remoulade/rate_limits/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/rate_limits/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/rate_limits/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/rate_limits/backends/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/rate_limits/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/rate_limits/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/rate_limits/rate_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/rate_limits/window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:58:07.532289 remoulade-1.2.4/remoulade/results/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/results/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:58:07.536289 remoulade-1.2.4/remoulade/results/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/results/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/results/backends/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/results/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/results/backends/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/results/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/results/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:58:07.536289 remoulade-1.2.4/remoulade/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:58:07.536289 remoulade-1.2.4/remoulade/state/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/state/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:58:07.536289 remoulade-1.2.4/remoulade/state/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/state/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/state/backends/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/state/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/state/backends/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/state/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/state/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20405 2023-07-05 09:57:51.000000 remoulade-1.2.4/remoulade/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:58:07.520289 remoulade-1.2.4/remoulade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-05 09:58:07.000000 remoulade-1.2.4/remoulade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-05 09:58:07.000000 remoulade-1.2.4/remoulade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:58:07.000000 remoulade-1.2.4/remoulade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-05 09:58:07.000000 remoulade-1.2.4/remoulade.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-05 09:58:07.000000 remoulade-1.2.4/remoulade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 09:58:07.000000 remoulade-1.2.4/remoulade.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-05 09:58:07.536289 remoulade-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-05 09:57:51.000000 remoulade-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:58.098007 remoulade-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-21 14:53:46.000000 remoulade-2.0.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-07-21 14:53:46.000000 remoulade-2.0.0/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 14:53:46.000000 remoulade-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-21 14:53:58.098007 remoulade-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-21 14:53:46.000000 remoulade-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:58.090010 remoulade-2.0.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      275 2023-07-21 14:53:46.000000 remoulade-2.0.0/bin/remoulade-gevent
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-21 14:53:46.000000 remoulade-2.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:58.094009 remoulade-2.0.0/remoulade/
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/actor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:58.094009 remoulade-2.0.0/remoulade/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/api/apispec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/api/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/api/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17143 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:58.094009 remoulade-2.0.0/remoulade/brokers/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/brokers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/brokers/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21648 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/brokers/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/brokers/stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:58.094009 remoulade-2.0.0/remoulade/cancel/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/cancel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/cancel/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:58.094009 remoulade-2.0.0/remoulade/cancel/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/cancel/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/cancel/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/cancel/backends/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/cancel/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/cancel/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:58.094009 remoulade-2.0.0/remoulade/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/cli/remoulade_ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/cli/remoulade_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/cli/remoulade_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/collection_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:58.098007 remoulade-2.0.0/remoulade/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/helpers/actor_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/helpers/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/helpers/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/helpers/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:58.098007 remoulade-2.0.0/remoulade/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/middleware/age_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/middleware/catch_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/middleware/current_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/middleware/logging_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/middleware/max_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/middleware/max_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/middleware/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/middleware/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/middleware/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/middleware/retries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/middleware/shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/middleware/threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/middleware/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:58.098007 remoulade-2.0.0/remoulade/rate_limits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/rate_limits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/rate_limits/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:58.098007 remoulade-2.0.0/remoulade/rate_limits/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/rate_limits/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/rate_limits/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/rate_limits/backends/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/rate_limits/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/rate_limits/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/rate_limits/rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/rate_limits/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:58.098007 remoulade-2.0.0/remoulade/results/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/results/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:58.098007 remoulade-2.0.0/remoulade/results/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/results/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/results/backends/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/results/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/results/backends/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/results/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/results/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:58.098007 remoulade-2.0.0/remoulade/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:58.098007 remoulade-2.0.0/remoulade/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/state/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:58.098007 remoulade-2.0.0/remoulade/state/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/state/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/state/backends/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/state/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/state/backends/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/state/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/state/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20405 2023-07-21 14:53:46.000000 remoulade-2.0.0/remoulade/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:53:58.094009 remoulade-2.0.0/remoulade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-21 14:53:58.000000 remoulade-2.0.0/remoulade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-21 14:53:58.000000 remoulade-2.0.0/remoulade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:53:58.000000 remoulade-2.0.0/remoulade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-21 14:53:58.000000 remoulade-2.0.0/remoulade.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-21 14:53:58.000000 remoulade-2.0.0/remoulade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 14:53:58.000000 remoulade-2.0.0/remoulade.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-21 14:53:58.102006 remoulade-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-21 14:53:46.000000 remoulade-2.0.0/setup.py
```

### Comparing `remoulade-1.2.4/COPYING` & `remoulade-2.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/COPYING.LESSER` & `remoulade-2.0.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/PKG-INFO` & `remoulade-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remoulade
-Version: 1.2.4
+Version: 2.0.0
 Summary: Background Processing for Python 3.
 Author: Wiremind
 Author-email: dev@wiremind.io
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `remoulade-1.2.4/README.md` & `remoulade-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/__init__.py` & `remoulade-2.0.0/remoulade/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,8 +86,8 @@
     # Workers
     "Worker",
     # Scheduler
     "get_scheduler",
     "set_scheduler",
 ]
 
-__version__ = "1.2.4"
+__version__ = "2.0.0"
```

### Comparing `remoulade-1.2.4/remoulade/__main__.py` & `remoulade-2.0.0/remoulade/__main__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/actor.py` & `remoulade-2.0.0/remoulade/actor.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/api/apispec.py` & `remoulade-2.0.0/remoulade/api/apispec.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/api/main.py` & `remoulade-2.0.0/remoulade/api/main.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/api/scheduler.py` & `remoulade-2.0.0/remoulade/api/scheduler.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/api/state.py` & `remoulade-2.0.0/remoulade/api/state.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/broker.py` & `remoulade-2.0.0/remoulade/broker.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/brokers/__init__.py` & `remoulade-2.0.0/remoulade/brokers/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/brokers/local.py` & `remoulade-2.0.0/remoulade/brokers/local.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/brokers/rabbitmq.py` & `remoulade-2.0.0/remoulade/brokers/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/brokers/stub.py` & `remoulade-2.0.0/remoulade/brokers/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/cancel/__init__.py` & `remoulade-2.0.0/remoulade/cancel/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/cancel/backend.py` & `remoulade-2.0.0/remoulade/cancel/backend.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/cancel/backends/__init__.py` & `remoulade-2.0.0/remoulade/cancel/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/cancel/backends/redis.py` & `remoulade-2.0.0/remoulade/cancel/backends/redis.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/cancel/backends/stub.py` & `remoulade-2.0.0/remoulade/cancel/backends/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/cancel/errors.py` & `remoulade-2.0.0/remoulade/cancel/errors.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/cancel/middleware.py` & `remoulade-2.0.0/remoulade/cancel/middleware.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/cli/remoulade_ls.py` & `remoulade-2.0.0/remoulade/cli/remoulade_ls.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/cli/remoulade_run.py` & `remoulade-2.0.0/remoulade/cli/remoulade_run.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/cli/remoulade_scheduler.py` & `remoulade-2.0.0/remoulade/cli/remoulade_scheduler.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/collection_results.py` & `remoulade-2.0.0/remoulade/collection_results.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/common.py` & `remoulade-2.0.0/remoulade/common.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/composition.py` & `remoulade-2.0.0/remoulade/composition.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/encoder.py` & `remoulade-2.0.0/remoulade/encoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 
 import abc
 import json
 import pickle
 import warnings
 from typing import Any, Dict, Optional, get_type_hints
 
+from typing_extensions import Annotated
+
 try:
-    from pydantic import BaseConfig, BaseModel, ValidationError, create_model
-    from pydantic.error_wrappers import ErrorWrapper
-    from pydantic.fields import ModelField
+    from pydantic import BaseConfig, BaseModel, TypeAdapter, ValidationError, WithJsonSchema, create_model
     from simplejson.decoder import JSONDecoder
     from simplejson.encoder import JSONEncoder as _JSONEncoder
 except ImportError:  # pragma: no cover
     warnings.warn(
         "Pydantic and simplejson are not available.  Run `pip install remoulade[pydantic]`",
         ImportWarning,
     )
@@ -97,15 +97,15 @@
         self.json_encoder = _JSONEncoder(default=self.default)
         self.json_decoder = JSONDecoder()
 
     @staticmethod
     def default(o):
         if isinstance(o, BaseModel):
             # keep dict otherwise it will be serialized as a string (see Pydantic .json())
-            return json.loads(o.json())
+            return json.loads(o.model_dump_json())
         raise TypeError("Object of type %s is not JSON serializable" % o.__class__.__name__)
 
     def encode(self, data: MessageData) -> bytes:
         try:
             return self.json_encoder.encode(data).encode("utf-8")
         except Exception as e:
             if self.fallback_encoder is not None:
@@ -120,52 +120,42 @@
             raw_message = self.json_decoder.decode(data.decode("utf-8"))  # type: ignore
             actor_name = raw_message["actor_name"]
             actor_fn = get_broker().get_actor(actor_name).fn
 
             # Retrieve the Pydantic schemas from typing
             schemas_by_param_name = {}
             for param_name, type_hint in get_type_hints(actor_fn).items():
-                schemas_by_param_name[param_name] = ModelField(
-                    type_=type_hint,
-                    name=f"{param_name}_schema",
-                    class_validators=None,
-                    model_config=BaseConfig,
+                schemas_by_param_name[param_name] = TypeAdapter(
+                    Annotated[
+                        type_hint,
+                        WithJsonSchema(
+                            {"type": type_hint, "description": f"{param_name}_schema"}, mode="serialization"
+                        ),
+                    ]
                 )
 
             # Override message_data with Pydantic schema when it matches
             parsed_message: Dict[str, Any] = {}
             for key, values in raw_message.items():
                 if key == "kwargs":
                     assert isinstance(values, dict)
                     parsed_message[key] = {
-                        param_name: self.get_parsed_value(raw_value, schemas_by_param_name[param_name])
+                        param_name: schemas_by_param_name[param_name].validate_python(raw_value)
                         for param_name, raw_value in values.items()
                     }
                 elif key == "args":
                     assert isinstance(values, list)
                     schemas = list(schemas_by_param_name.values())
                     parsed_message[key] = [
-                        self.get_parsed_value(raw_value, schemas[order]) for order, raw_value in enumerate(values)
+                        schemas[order].validate_python(raw_value) for order, raw_value in enumerate(values)
                     ]
                 elif key == "result":
-                    parsed_message[key] = self.get_parsed_value(values, schemas_by_param_name["return"])
+                    parsed_message[key] = schemas_by_param_name["return"].validate_python(values)
                 else:
                     parsed_message[key] = values
 
             return parsed_message
         except Exception as e:
             if self.fallback_encoder is not None:
                 return self.fallback_encoder.decode(data)
             else:
                 raise e
-
-    @staticmethod
-    def get_parsed_value(raw_value: Any, schema: "ModelField"):
-        errors = []
-        parsed_value, errors_ = schema.validate(raw_value, {}, loc=())
-        if isinstance(errors_, ErrorWrapper):
-            errors.append(errors_)
-        elif isinstance(errors_, list):
-            errors.extend(errors_)
-        if errors:
-            raise ValidationError(errors, create_model("RemouladeEncoder"))
-        return parsed_value
```

### Comparing `remoulade-1.2.4/remoulade/errors.py` & `remoulade-2.0.0/remoulade/errors.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/generic.py` & `remoulade-2.0.0/remoulade/generic.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/helpers/__init__.py` & `remoulade-2.0.0/remoulade/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/helpers/actor_arguments.py` & `remoulade-2.0.0/remoulade/helpers/actor_arguments.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/helpers/backoff.py` & `remoulade-2.0.0/remoulade/helpers/backoff.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/helpers/queues.py` & `remoulade-2.0.0/remoulade/helpers/queues.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/helpers/reduce.py` & `remoulade-2.0.0/remoulade/helpers/reduce.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/logging.py` & `remoulade-2.0.0/remoulade/logging.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/message.py` & `remoulade-2.0.0/remoulade/message.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/middleware/__init__.py` & `remoulade-2.0.0/remoulade/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/middleware/age_limit.py` & `remoulade-2.0.0/remoulade/middleware/age_limit.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/middleware/catch_error.py` & `remoulade-2.0.0/remoulade/middleware/catch_error.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/middleware/current_message.py` & `remoulade-2.0.0/remoulade/middleware/current_message.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/middleware/logging_metadata.py` & `remoulade-2.0.0/remoulade/middleware/logging_metadata.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/middleware/max_memory.py` & `remoulade-2.0.0/remoulade/middleware/max_memory.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/middleware/max_tasks.py` & `remoulade-2.0.0/remoulade/middleware/max_tasks.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/middleware/middleware.py` & `remoulade-2.0.0/remoulade/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/middleware/pipelines.py` & `remoulade-2.0.0/remoulade/middleware/pipelines.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/middleware/prometheus.py` & `remoulade-2.0.0/remoulade/middleware/prometheus.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/middleware/retries.py` & `remoulade-2.0.0/remoulade/middleware/retries.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/middleware/shutdown.py` & `remoulade-2.0.0/remoulade/middleware/shutdown.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/middleware/threading.py` & `remoulade-2.0.0/remoulade/middleware/threading.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/middleware/time_limit.py` & `remoulade-2.0.0/remoulade/middleware/time_limit.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/rate_limits/__init__.py` & `remoulade-2.0.0/remoulade/rate_limits/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/rate_limits/backend.py` & `remoulade-2.0.0/remoulade/rate_limits/backend.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/rate_limits/backends/__init__.py` & `remoulade-2.0.0/remoulade/rate_limits/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/rate_limits/backends/redis.py` & `remoulade-2.0.0/remoulade/rate_limits/backends/redis.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/rate_limits/backends/stub.py` & `remoulade-2.0.0/remoulade/rate_limits/backends/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/rate_limits/bucket.py` & `remoulade-2.0.0/remoulade/rate_limits/bucket.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/rate_limits/concurrent.py` & `remoulade-2.0.0/remoulade/rate_limits/concurrent.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/rate_limits/rate_limiter.py` & `remoulade-2.0.0/remoulade/rate_limits/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/rate_limits/window.py` & `remoulade-2.0.0/remoulade/rate_limits/window.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/result.py` & `remoulade-2.0.0/remoulade/result.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/results/__init__.py` & `remoulade-2.0.0/remoulade/results/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/results/backend.py` & `remoulade-2.0.0/remoulade/results/backend.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/results/backends/__init__.py` & `remoulade-2.0.0/remoulade/results/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/results/backends/local.py` & `remoulade-2.0.0/remoulade/results/backends/local.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/results/backends/redis.py` & `remoulade-2.0.0/remoulade/results/backends/redis.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/results/backends/stub.py` & `remoulade-2.0.0/remoulade/results/backends/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/results/errors.py` & `remoulade-2.0.0/remoulade/results/errors.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/results/middleware.py` & `remoulade-2.0.0/remoulade/results/middleware.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/scheduler/__init__.py` & `remoulade-2.0.0/remoulade/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/scheduler/scheduler.py` & `remoulade-2.0.0/remoulade/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/state/backend.py` & `remoulade-2.0.0/remoulade/state/backend.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/state/backends/__init__.py` & `remoulade-2.0.0/remoulade/state/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/state/backends/postgres.py` & `remoulade-2.0.0/remoulade/state/backends/postgres.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/state/backends/redis.py` & `remoulade-2.0.0/remoulade/state/backends/redis.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/state/backends/stub.py` & `remoulade-2.0.0/remoulade/state/backends/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/state/middleware.py` & `remoulade-2.0.0/remoulade/state/middleware.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/utils.py` & `remoulade-2.0.0/remoulade/utils.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade/worker.py` & `remoulade-2.0.0/remoulade/worker.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade.egg-info/PKG-INFO` & `remoulade-2.0.0/remoulade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remoulade
-Version: 1.2.4
+Version: 2.0.0
 Summary: Background Processing for Python 3.
 Author: Wiremind
 Author-email: dev@wiremind.io
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `remoulade-1.2.4/remoulade.egg-info/SOURCES.txt` & `remoulade-2.0.0/remoulade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/remoulade.egg-info/requires.txt` & `remoulade-2.0.0/remoulade.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 prometheus-client>=0.2
 pytz
 python-dateutil>=2.8.0
 typing-extensions>=3.7
 
 [all]
-simplejson
+sqlalchemy<2,>=1.4.29
 flask<2.2,>=1.1
 amqpstorm<3,>=2.6
-psycopg2==2.9.5
-marshmallow>=3
-pydantic<2
 flask-apispec
-sqlalchemy<2,>=1.4.29
+pydantic>=2.0
 redis~=4.5
+psycopg2==2.9.5
+simplejson
+marshmallow>=3
 
 [dev]
-simplejson
+sqlalchemy<2,>=1.4.29
 flask<2.2,>=1.1
 amqpstorm<3,>=2.6
-psycopg2==2.9.5
-marshmallow>=3
-pydantic<2
 flask-apispec
-sqlalchemy<2,>=1.4.29
+pydantic>=2.0
 redis~=4.5
+psycopg2==2.9.5
+simplejson
+marshmallow>=3
 alabaster
 sphinx==4.1.1
 sphinxcontrib-napoleon
 sphinxcontrib-versioning
 sphinx-copybutton
 flake8
 flake8-bugbear
@@ -50,15 +50,15 @@
 freezegun
 
 [postgres]
 sqlalchemy<2,>=1.4.29
 psycopg2==2.9.5
 
 [pydantic]
-pydantic<2
+pydantic>=2.0
 simplejson
 
 [rabbitmq]
 amqpstorm<3,>=2.6
 
 [redis]
 redis~=4.5
```

### Comparing `remoulade-1.2.4/setup.cfg` & `remoulade-2.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.4/setup.py` & `remoulade-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 dependencies = ["prometheus-client>=0.2", "pytz", "python-dateutil>=2.8.0", "typing-extensions>=3.7"]
 
 extra_dependencies = {
     "rabbitmq": ["amqpstorm>=2.6,<3"],
     "redis": ["redis~=4.5"],
     "server": ["flask>=1.1,<2.2", "marshmallow>=3", "flask-apispec"],
     "postgres": ["sqlalchemy>=1.4.29,<2", "psycopg2==2.9.5"],
-    "pydantic": ["pydantic<2", "simplejson"]
+    "pydantic": ["pydantic>=2.0", "simplejson"],
 }
 
 extra_dependencies["all"] = list(set(sum(extra_dependencies.values(), [])))
 extra_dependencies["dev"] = extra_dependencies["all"] + [
     # Docs
     "alabaster",
     "sphinx==4.1.1",
```

