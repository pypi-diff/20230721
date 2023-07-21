# Comparing `tmp/nsj_rest_lib-1.3.1.tar.gz` & `tmp/nsj_rest_lib-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_rest_lib-1.3.1.tar", last modified: Mon Jul  3 15:32:45 2023, max compression
+gzip compressed data, was "nsj_rest_lib-1.4.0.tar", last modified: Fri Jul 21 15:07:02 2023, max compression
```

## Comparing `nsj_rest_lib-1.3.1.tar` & `nsj_rest_lib-1.4.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-03 15:32:45.933283 nsj_rest_lib-1.3.1/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-07-03 15:32:45.933283 nsj_rest_lib-1.3.1/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      130 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/README.md
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      888 2023-07-03 15:32:45.933283 nsj_rest_lib-1.3.1/setup.cfg
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-03 15:32:45.917283 nsj_rest_lib-1.3.1/src/
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-03 15:32:45.921283 nsj_rest_lib-1.3.1/src/nsj_rest_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/__init__.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-03 15:32:45.929283 nsj_rest_lib-1.3.1/src/nsj_rest_lib/controller/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/controller/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/controller/controller_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3298 2023-06-29 22:11:32.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/controller/delete_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3907 2023-06-29 22:11:52.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/controller/get_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4590 2023-07-01 23:25:08.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/controller/list_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4351 2023-06-29 22:09:50.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/controller/patch_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3931 2023-06-29 22:10:22.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/controller/post_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4341 2023-06-29 22:10:52.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/controller/put_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/controller/route_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-03 15:32:45.929283 nsj_rest_lib-1.3.1/src/nsj_rest_lib/dao/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/dao/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    21249 2023-07-02 00:37:26.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/dao/dao_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1223 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/db_pool_config.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-03 15:32:45.929283 nsj_rest_lib-1.3.1/src/nsj_rest_lib/decorator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/decorator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4737 2023-07-01 22:57:27.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/decorator/dto.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-03 15:32:45.929283 nsj_rest_lib-1.3.1/src/nsj_rest_lib/descriptor/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/descriptor/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      418 2023-07-01 22:04:56.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/descriptor/conjunto_type.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    13010 2023-07-02 00:10:05.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/descriptor/dto_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/descriptor/dto_field_validators.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     5408 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/descriptor/dto_list_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      320 2023-07-02 00:29:03.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/descriptor/filter_operator.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/doc_route_generator.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-03 15:32:45.929283 nsj_rest_lib-1.3.1/src/nsj_rest_lib/dto/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/dto/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7653 2023-07-03 15:27:33.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/dto/dto_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-03 15:32:45.933283 nsj_rest_lib-1.3.1/src/nsj_rest_lib/entity/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/entity/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      710 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/entity/entity_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      322 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/entity/filter.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/exception.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/healthcheck_config.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      825 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/injector_factory_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-03 15:32:45.933283 nsj_rest_lib-1.3.1/src/nsj_rest_lib/service/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/service/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    24073 2023-07-02 00:47:53.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/service/service_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      707 2023-06-29 21:53:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/settings.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-03 15:32:45.933283 nsj_rest_lib-1.3.1/src/nsj_rest_lib/validator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/validator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/validator/cpf_cnpj.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib/validator/validate_data.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-03 15:32:45.925283 nsj_rest_lib-1.3.1/src/nsj_rest_lib.egg-info/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-07-03 15:32:45.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1697 2023-07-03 15:32:45.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-03 15:32:45.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      113 2023-07-03 15:32:45.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2023-07-03 15:32:45.000000 nsj_rest_lib-1.3.1/src/nsj_rest_lib.egg-info/top_level.txt
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:07:02.212877 nsj_rest_lib-1.4.0/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-07-21 15:07:02.212877 nsj_rest_lib-1.4.0/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      130 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/README.md
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      888 2023-07-21 15:07:02.212877 nsj_rest_lib-1.4.0/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:07:02.208877 nsj_rest_lib-1.4.0/src/
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:07:02.208877 nsj_rest_lib-1.4.0/src/nsj_rest_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/__init__.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:07:02.208877 nsj_rest_lib-1.4.0/src/nsj_rest_lib/controller/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/controller/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/controller/controller_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3298 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/controller/delete_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3907 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/controller/get_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4590 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/controller/list_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4351 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/controller/patch_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3931 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/controller/post_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4341 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/controller/put_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/controller/route_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:07:02.208877 nsj_rest_lib-1.4.0/src/nsj_rest_lib/dao/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/dao/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    21249 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/dao/dao_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1223 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/db_pool_config.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:07:02.208877 nsj_rest_lib-1.4.0/src/nsj_rest_lib/decorator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/decorator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4737 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/decorator/dto.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:07:02.208877 nsj_rest_lib-1.4.0/src/nsj_rest_lib/descriptor/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/descriptor/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      418 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/descriptor/conjunto_type.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    13146 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/descriptor/dto_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/descriptor/dto_field_validators.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5408 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/descriptor/dto_list_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      320 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/descriptor/filter_operator.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/doc_route_generator.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:07:02.208877 nsj_rest_lib-1.4.0/src/nsj_rest_lib/dto/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/dto/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7760 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/dto/dto_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:07:02.208877 nsj_rest_lib-1.4.0/src/nsj_rest_lib/entity/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/entity/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      710 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/entity/entity_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      322 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/entity/filter.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/healthcheck_config.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      825 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/injector_factory_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:07:02.212877 nsj_rest_lib-1.4.0/src/nsj_rest_lib/service/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/service/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    24142 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/service/service_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      707 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/settings.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:07:02.212877 nsj_rest_lib-1.4.0/src/nsj_rest_lib/validator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/validator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/validator/cpf_cnpj.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2023-07-21 15:01:40.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib/validator/validate_data.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:07:02.208877 nsj_rest_lib-1.4.0/src/nsj_rest_lib.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-07-21 15:07:02.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1697 2023-07-21 15:07:02.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-21 15:07:02.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      113 2023-07-21 15:07:02.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2023-07-21 15:07:02.000000 nsj_rest_lib-1.4.0/src/nsj_rest_lib.egg-info/top_level.txt
```

### Comparing `nsj_rest_lib-1.3.1/PKG-INFO` & `nsj_rest_lib-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_rest_lib
-Version: 1.3.1
+Version: 1.4.0
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-1.3.1/setup.cfg` & `nsj_rest_lib-1.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_rest_lib
-version = 1.3.1
+version = 1.4.0
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj_rest_lib
 project_urls =
```

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/controller/delete_route.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/controller/delete_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/controller/get_route.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/controller/get_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/controller/list_route.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/controller/list_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/controller/patch_route.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/controller/patch_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/controller/post_route.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/controller/post_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/controller/put_route.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/controller/put_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/controller/route_base.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/controller/route_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/dao/dao_base.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/dao/dao_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/db_pool_config.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/db_pool_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/decorator/dto.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/decorator/dto.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/descriptor/dto_field.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/descriptor/dto_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,21 +89,22 @@
     def __get__(self, instance, owner):
         if instance is None:
             return self
         else:
             return instance.__dict__[self.storage_name]
 
     def __set__(self, instance, value):
-        if self.validator is None:
-            if self.use_default_validator:
-                value = self.validate(self, value)
-        else:
-            if self.use_default_validator:
-                value = self.validate(self, value)
-            value = self.validator(self, value)
+        if not ("escape_validator" in instance.__dict__ and instance.__dict__["escape_validator"] == True):
+            if self.validator is None:
+                if self.use_default_validator:
+                    value = self.validate(self, value)
+            else:
+                if self.use_default_validator:
+                    value = self.validate(self, value)
+                value = self.validator(self, value)
 
         instance.__dict__[self.storage_name] = value
 
     def validate(self, dto_field: "DTOField", value):
         """
         Default validator (ckecking default constraints: not null, type, min, max and enum types).
         """
```

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/descriptor/dto_field_validators.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/descriptor/dto_field_validators.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/descriptor/dto_list_field.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/descriptor/dto_list_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/doc_route_generator.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/doc_route_generator.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/dto/dto_base.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/dto/dto_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,21 @@
     list_fields_map: dict = {}
     field_filters_map: Dict[str, DTOFieldFilter]
     # TODO Refatorar para suportar PK composto
     pk_field: str
     fixed_filters: Dict[str, Any]
     conjunto_type: ConjuntoType
     conjunto_field: str
+    escape_validator: bool
 
-    def __init__(self, entity: Union[EntityBase, dict] = None, **kwargs) -> None:
+    def __init__(self, entity: Union[EntityBase, dict] = None, escape_validator: bool = False, **kwargs) -> None:
         super().__init__()
 
+        self.escape_validator = escape_validator
+
         # Transformando a entity em dict (se houver uma entity)
         if entity is not None:
             kwargs = (
                 copy.deepcopy(entity)
                 if type(entity) is dict
                 else copy.deepcopy(entity.__dict__)
             )
@@ -83,15 +86,15 @@
 
                     related_itens = []
                     for item in kwargs[field]:
                         # Preenchendo os campos de particionanmento, se necessário (normalmente: tenant e grupo_empresarial)
                         for partition_field in self.__class__.partition_fields:
                             if (
                                 (
-                                    not (partition_field in item)
+                                    partition_field not in item
                                     or item[partition_field] is None
                                 )
                                 and partition_field
                                 in dto_list_field.dto_type.partition_fields
                             ):
                                 partition_value = getattr(self, partition_field)
                                 item[partition_field] = partition_value
```

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/entity/entity_base.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/entity/entity_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/healthcheck_config.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/healthcheck_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/injector_factory_base.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/injector_factory_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/service/service_base.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/service/service_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
         entity_filters = self._create_entity_filters(partition_fields)
 
         # Recuperando a entity
         entity = self._dao.get(id, entity_fields, entity_filters)
 
         # Convertendo para DTO
-        dto = self._dto_class(entity)
+        dto = self._dto_class(entity, escape_validator=True)
 
         # Tratando das propriedades de lista
         if len(self._dto_class.list_fields_map) > 0:
             self._retrieve_related_lists([dto], fields)
 
         return dto
 
@@ -212,15 +212,15 @@
             order_fields,
             entity_filters,
             conjunto_type=self._dto_class.conjunto_type,
             conjunto_field=self._dto_class.conjunto_field,
         )
 
         # Convertendo para uma lista de DTOs
-        dto_list = [self._dto_class(entity) for entity in entity_list]
+        dto_list = [self._dto_class(entity, escape_validator=True) for entity in entity_list]
 
         # Retrieving related lists
         if len(self._dto_class.list_fields_map) > 0:
             self._retrieve_related_lists(dto_list, fields)
 
         # Returning
         return dto_list
@@ -389,15 +389,15 @@
                 entity_filters = {**id_filters, **aditional_entity_filters}
 
                 # Executando o update pelo DAO
                 entity = self._dao.update(entity, entity_filters, partial_update)
 
             # Convertendo a entity para o DTO de resposta (se houver um)
             if self._dto_post_response_class is not None:
-                response_dto = self._dto_post_response_class(entity)
+                response_dto = self._dto_post_response_class(entity, escape_validator=True)
             else:
                 # Retorna None, se não se espera um DTO de resposta
                 response_dto = None
 
             # Salvando as lista de DTO detalhe
             if len(self._dto_class.list_fields_map) > 0:
                 self._save_related_lists(
```

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/settings.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/settings.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/validator/cpf_cnpj.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/validator/cpf_cnpj.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib/validator/validate_data.py` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib/validator/validate_data.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib.egg-info/PKG-INFO` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-rest-lib
-Version: 1.3.1
+Version: 1.4.0
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-1.3.1/src/nsj_rest_lib.egg-info/SOURCES.txt` & `nsj_rest_lib-1.4.0/src/nsj_rest_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

