# Comparing `tmp/jsm-autodynatrace-1.0.1.tar.gz` & `tmp/jsm-autodynatrace-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsm-autodynatrace-1.0.1.tar", last modified: Tue Jul 18 17:36:33 2023, max compression
+gzip compressed data, was "jsm-autodynatrace-1.1.0.tar", last modified: Fri Jul 21 18:54:00 2023, max compression
```

## Comparing `jsm-autodynatrace-1.0.1.tar` & `jsm-autodynatrace-1.1.0.tar`

### file list

```diff
@@ -1,111 +1,116 @@
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.647400 jsm-autodynatrace-1.0.1/
--rw-r--r--   0 matheusslgd   (502) staff       (20)    12871 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/LICENSE
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1140 2023-07-18 17:36:33.647516 jsm-autodynatrace-1.0.1/PKG-INFO
--rw-r--r--   0 matheusslgd   (502) staff       (20)     3168 2023-07-18 15:18:16.000000 jsm-autodynatrace-1.0.1/README.md
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.631983 jsm-autodynatrace-1.0.1/autodynatrace/
--rw-r--r--   0 matheusslgd   (502) staff       (20)     3938 2023-07-18 15:18:16.000000 jsm-autodynatrace-1.0.1/autodynatrace/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      320 2023-07-17 20:30:37.000000 jsm-autodynatrace-1.0.1/autodynatrace/log.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      523 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/sdk.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.632438 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/
--rw-r--r--   0 matheusslgd   (502) staff       (20)        0 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/__init__.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.633097 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/aiohttp/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/aiohttp/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      935 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/aiohttp/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.633903 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/bottle/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/bottle/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2044 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/bottle/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.634365 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/celery/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/celery/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     4454 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/celery/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.634862 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/concurrent/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/concurrent/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1691 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/concurrent/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.635298 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/confluent_kafka/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/confluent_kafka/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     3550 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/confluent_kafka/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.635605 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/custom/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       45 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/custom/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2473 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/custom/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.635963 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/cx_Oracle/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/cx_Oracle/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     4412 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/cx_Oracle/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.636110 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/dbapi/
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2792 2023-07-18 15:18:16.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/dbapi/__init__.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.637249 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django/
--rw-r--r--   0 matheusslgd   (502) staff       (20)      152 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      265 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django/apps.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1819 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django/db.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      656 2023-07-18 15:18:16.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django/log.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     3388 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django/middlewares.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1735 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django/utils.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      974 2023-07-18 15:18:16.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.638141 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django_stomp/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       31 2023-07-18 15:18:16.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django_stomp/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2095 2023-07-18 15:18:16.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django_stomp/consumer.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1658 2023-07-18 15:18:16.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django_stomp/publisher.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      481 2023-07-18 17:36:06.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django_stomp/utils.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      157 2023-07-18 15:18:16.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django_stomp/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.638577 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/fastapi/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/fastapi/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2387 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/fastapi/middleware.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1326 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/fastapi/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.638852 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/flask/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/flask/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2554 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/flask/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.639124 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/grpc/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/grpc/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2357 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/grpc/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.639396 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/paramiko/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/paramiko/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1041 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/paramiko/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.639695 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/pika/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/pika/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     3353 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/pika/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.639981 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/psycopg2/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/psycopg2/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2193 2023-07-18 15:18:16.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/psycopg2/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.640417 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/pymongo/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/pymongo/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2060 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/pymongo/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.640960 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/pysnmp/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/pysnmp/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     4813 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/pysnmp/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.641976 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/redis/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/redis/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      716 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/redis/utils.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2061 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/redis/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.642508 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/ruxit/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/ruxit/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      462 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/ruxit/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.642879 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/sqlalchemy/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/sqlalchemy/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     4386 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/sqlalchemy/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.643400 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/starlette/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/starlette/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1424 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/starlette/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.643779 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/subprocess/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/subprocess/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1365 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/subprocess/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.644333 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/suds/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/suds/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      697 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/suds/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.644718 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/tornado/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/tornado/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1703 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/tornado/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.645208 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/urllib/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/urllib/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1522 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/urllib/wrapper.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      102 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/autodynatrace/wrappers/utils.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.646635 jsm-autodynatrace-1.0.1/jsm_autodynatrace.egg-info/
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1140 2023-07-18 17:36:33.000000 jsm-autodynatrace-1.0.1/jsm_autodynatrace.egg-info/PKG-INFO
--rw-r--r--   0 matheusslgd   (502) staff       (20)     3079 2023-07-18 17:36:33.000000 jsm-autodynatrace-1.0.1/jsm_autodynatrace.egg-info/SOURCES.txt
--rw-r--r--   0 matheusslgd   (502) staff       (20)        1 2023-07-18 17:36:33.000000 jsm-autodynatrace-1.0.1/jsm_autodynatrace.egg-info/dependency_links.txt
--rw-r--r--   0 matheusslgd   (502) staff       (20)       44 2023-07-18 17:36:33.000000 jsm-autodynatrace-1.0.1/jsm_autodynatrace.egg-info/entry_points.txt
--rw-r--r--   0 matheusslgd   (502) staff       (20)       61 2023-07-18 17:36:33.000000 jsm-autodynatrace-1.0.1/jsm_autodynatrace.egg-info/requires.txt
--rw-r--r--   0 matheusslgd   (502) staff       (20)       20 2023-07-18 17:36:33.000000 jsm-autodynatrace-1.0.1/jsm_autodynatrace.egg-info/top_level.txt
--rw-r--r--   0 matheusslgd   (502) staff       (20)      102 2023-07-18 17:36:33.648210 jsm-autodynatrace-1.0.1/setup.cfg
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1545 2023-07-18 17:36:06.000000 jsm-autodynatrace-1.0.1/setup.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-18 17:36:33.647213 jsm-autodynatrace-1.0.1/tests/
--rw-r--r--   0 matheusslgd   (502) staff       (20)        0 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/tests/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     6759 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/tests/test_custom.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1327 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.0.1/tests/test_django.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.537609 jsm-autodynatrace-1.1.0/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)    12871 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/LICENSE
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1140 2023-07-21 18:54:00.537699 jsm-autodynatrace-1.1.0/PKG-INFO
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     3168 2023-07-18 20:34:31.000000 jsm-autodynatrace-1.1.0/README.md
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.524531 jsm-autodynatrace-1.1.0/autodynatrace/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     3973 2023-07-21 18:53:46.000000 jsm-autodynatrace-1.1.0/autodynatrace/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      320 2023-07-17 20:30:37.000000 jsm-autodynatrace-1.1.0/autodynatrace/log.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      523 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/sdk.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.524883 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)        0 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/__init__.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.525391 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/aiohttp/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/aiohttp/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      935 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/aiohttp/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.526146 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/bottle/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/bottle/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2044 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/bottle/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.526491 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/celery/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/celery/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     4454 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/celery/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.526821 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/concurrent/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/concurrent/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1691 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/concurrent/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.527125 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/confluent_kafka/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/confluent_kafka/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     3550 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/confluent_kafka/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.527430 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/custom/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       45 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/custom/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2473 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/custom/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.527724 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/cx_Oracle/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/cx_Oracle/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     4412 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/cx_Oracle/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.527869 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/dbapi/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2792 2023-07-18 20:34:01.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/dbapi/__init__.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.529185 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      152 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      265 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/apps.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1819 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/db.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      656 2023-07-18 20:34:31.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/log.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     3388 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/middlewares.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1735 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/utils.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      974 2023-07-18 20:34:31.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.530283 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_outbox_pattern/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       31 2023-07-21 18:53:46.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_outbox_pattern/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2085 2023-07-21 18:53:46.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_outbox_pattern/consumer.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1623 2023-07-21 18:53:46.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_outbox_pattern/publisher.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      157 2023-07-21 18:53:46.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_outbox_pattern/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.531340 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_stomp/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       31 2023-07-18 20:34:01.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_stomp/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2095 2023-07-18 20:34:01.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_stomp/consumer.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1658 2023-07-18 20:34:01.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_stomp/publisher.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      481 2023-07-18 20:34:02.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_stomp/utils.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      157 2023-07-18 20:34:01.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_stomp/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.531774 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/fastapi/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/fastapi/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2387 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/fastapi/middleware.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1326 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/fastapi/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.532144 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/flask/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/flask/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2554 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/flask/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.532453 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/grpc/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/grpc/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2357 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/grpc/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.532775 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/paramiko/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/paramiko/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1041 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/paramiko/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.533113 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pika/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pika/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     3353 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pika/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.533395 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/psycopg2/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/psycopg2/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2193 2023-07-18 20:34:02.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/psycopg2/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.533755 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pymongo/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pymongo/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2060 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pymongo/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.534112 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pysnmp/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pysnmp/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     4813 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pysnmp/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.534509 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/redis/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/redis/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      716 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/redis/utils.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2061 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/redis/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.534779 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/ruxit/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/ruxit/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      462 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/ruxit/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.535050 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/sqlalchemy/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/sqlalchemy/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     4386 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/sqlalchemy/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.535322 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/starlette/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/starlette/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1424 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/starlette/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.535585 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/subprocess/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/subprocess/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1365 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/subprocess/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.535853 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/suds/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/suds/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      697 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/suds/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.536126 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/tornado/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/tornado/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1703 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/tornado/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.536381 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/urllib/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/urllib/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1522 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/urllib/wrapper.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      102 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/utils.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.537088 jsm-autodynatrace-1.1.0/jsm_autodynatrace.egg-info/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1140 2023-07-21 18:54:00.000000 jsm-autodynatrace-1.1.0/jsm_autodynatrace.egg-info/PKG-INFO
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     3307 2023-07-21 18:54:00.000000 jsm-autodynatrace-1.1.0/jsm_autodynatrace.egg-info/SOURCES.txt
+-rw-r--r--   0 matheusslgd   (502) staff       (20)        1 2023-07-21 18:54:00.000000 jsm-autodynatrace-1.1.0/jsm_autodynatrace.egg-info/dependency_links.txt
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       44 2023-07-21 18:54:00.000000 jsm-autodynatrace-1.1.0/jsm_autodynatrace.egg-info/entry_points.txt
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       61 2023-07-21 18:54:00.000000 jsm-autodynatrace-1.1.0/jsm_autodynatrace.egg-info/requires.txt
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       20 2023-07-21 18:54:00.000000 jsm-autodynatrace-1.1.0/jsm_autodynatrace.egg-info/top_level.txt
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      102 2023-07-21 18:54:00.537933 jsm-autodynatrace-1.1.0/setup.cfg
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1545 2023-07-21 18:53:46.000000 jsm-autodynatrace-1.1.0/setup.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.537461 jsm-autodynatrace-1.1.0/tests/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)        0 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/tests/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     6759 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/tests/test_custom.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1327 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/tests/test_django.py
```

### Comparing `jsm-autodynatrace-1.0.1/LICENSE` & `jsm-autodynatrace-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/PKG-INFO` & `jsm-autodynatrace-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsm-autodynatrace
-Version: 1.0.1
+Version: 1.1.0
 Summary: Auto instrumentation for the OneAgent SDK
 Home-page: https://github.com/juntossomosmais/OneAgent-SDK-Python-AutoInstrumentation
 Author: Juntos Somos Mais
 Author-email: labs@juntossomosmais.com.br
 Project-URL: Issue Tracker, https://github.com/juntossomosmais/OneAgent-SDK-Python-AutoInstrumentation/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `jsm-autodynatrace-1.0.1/README.md` & `jsm-autodynatrace-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/__init__.py` & `jsm-autodynatrace-1.1.0/autodynatrace/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     "psycopg2": True,
     "tornado": True,
     "fastapi": True,
     "starlette": True,
     "aiohttp": True,
     "bottle": True,
     "django_stomp": True,
+    "django_outbox_pattern": True,
 }
 
 
 def will_instrument(lib_name, default):
     # Check if the user has chose to forcefully instrument (or not instrument) this lib
     lib_environment_variable_name = "AUTODYNATRACE_INSTRUMENT_{}".format(lib_name.upper())
```

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/sdk.py` & `jsm-autodynatrace-1.1.0/autodynatrace/sdk.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/aiohttp/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/aiohttp/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/bottle/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/bottle/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/celery/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/celery/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/concurrent/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/concurrent/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/confluent_kafka/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/confluent_kafka/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/custom/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/custom/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/cx_Oracle/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/cx_Oracle/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/dbapi/__init__.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django/db.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/db.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django/log.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/log.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django/middlewares.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/middlewares.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django/utils.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/utils.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django_stomp/consumer.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_stomp/consumer.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/django_stomp/publisher.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_stomp/publisher.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/fastapi/middleware.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/fastapi/middleware.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/fastapi/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/fastapi/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/flask/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/flask/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/grpc/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/grpc/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/paramiko/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/paramiko/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/pika/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pika/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/psycopg2/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/psycopg2/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/pymongo/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pymongo/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/pysnmp/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pysnmp/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/redis/utils.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/redis/utils.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/redis/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/redis/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/sqlalchemy/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/sqlalchemy/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/starlette/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/starlette/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/subprocess/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/subprocess/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/suds/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/suds/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/tornado/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/tornado/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/autodynatrace/wrappers/urllib/wrapper.py` & `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/urllib/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/jsm_autodynatrace.egg-info/PKG-INFO` & `jsm-autodynatrace-1.1.0/jsm_autodynatrace.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsm-autodynatrace
-Version: 1.0.1
+Version: 1.1.0
 Summary: Auto instrumentation for the OneAgent SDK
 Home-page: https://github.com/juntossomosmais/OneAgent-SDK-Python-AutoInstrumentation
 Author: Juntos Somos Mais
 Author-email: labs@juntossomosmais.com.br
 Project-URL: Issue Tracker, https://github.com/juntossomosmais/OneAgent-SDK-Python-AutoInstrumentation/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `jsm-autodynatrace-1.0.1/jsm_autodynatrace.egg-info/SOURCES.txt` & `jsm-autodynatrace-1.1.0/jsm_autodynatrace.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 autodynatrace/wrappers/django/__init__.py
 autodynatrace/wrappers/django/apps.py
 autodynatrace/wrappers/django/db.py
 autodynatrace/wrappers/django/log.py
 autodynatrace/wrappers/django/middlewares.py
 autodynatrace/wrappers/django/utils.py
 autodynatrace/wrappers/django/wrapper.py
+autodynatrace/wrappers/django_outbox_pattern/__init__.py
+autodynatrace/wrappers/django_outbox_pattern/consumer.py
+autodynatrace/wrappers/django_outbox_pattern/publisher.py
+autodynatrace/wrappers/django_outbox_pattern/wrapper.py
 autodynatrace/wrappers/django_stomp/__init__.py
 autodynatrace/wrappers/django_stomp/consumer.py
 autodynatrace/wrappers/django_stomp/publisher.py
 autodynatrace/wrappers/django_stomp/utils.py
 autodynatrace/wrappers/django_stomp/wrapper.py
 autodynatrace/wrappers/fastapi/__init__.py
 autodynatrace/wrappers/fastapi/middleware.py
```

### Comparing `jsm-autodynatrace-1.0.1/setup.py` & `jsm-autodynatrace-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="jsm-autodynatrace",
-    version="1.0.1",
+    version="1.1.0",
     packages=find_packages(),
     package_data={"autodynatrace": ["wrappers/*"]},
     install_requires=["wrapt>=1.11.2", "oneagent-sdk>=1.3.0", "six>=1.10.0", "autowrapt>=1.0"],
     tests_require=["pytest", "mock", "tox", "django"],
     entry_points={"autodynatrace": ["string = autodynatrace:load"]},
     python_requires=">=3.6",
     author="Juntos Somos Mais",
```

### Comparing `jsm-autodynatrace-1.0.1/tests/test_custom.py` & `jsm-autodynatrace-1.1.0/tests/test_custom.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.0.1/tests/test_django.py` & `jsm-autodynatrace-1.1.0/tests/test_django.py`

 * *Files identical despite different names*

