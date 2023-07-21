# Comparing `tmp/appengine-python-standard-1.1.2.tar.gz` & `tmp/appengine-python-standard-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appengine-python-standard-1.1.2.tar", last modified: Wed May 31 17:45:09 2023, max compression
+gzip compressed data, was "appengine-python-standard-1.1.3.tar", last modified: Fri Jul 21 20:07:02 2023, max compression
```

## Comparing `appengine-python-standard-1.1.2.tar` & `appengine-python-standard-1.1.3.tar`

### file list

```diff
@@ -1,245 +1,245 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.468728 appengine-python-standard-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-31 17:45:09.468728 appengine-python-standard-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 17:45:09.468728 appengine-python-standard-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.408723 appengine-python-standard-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.420724 appengine-python-standard-1.1.2/src/appengine_python_standard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-31 17:45:09.000000 appengine-python-standard-1.1.2/src/appengine_python_standard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-05-31 17:45:09.000000 appengine-python-standard-1.1.2/src/appengine_python_standard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:45:09.000000 appengine-python-standard-1.1.2/src/appengine_python_standard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 17:45:09.000000 appengine-python-standard-1.1.2/src/appengine_python_standard.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-31 17:45:09.000000 appengine-python-standard-1.1.2/src/appengine_python_standard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 17:45:09.000000 appengine-python-standard-1.1.2/src/appengine_python_standard.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.420724 appengine-python-standard-1.1.2/src/google/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.420724 appengine-python-standard-1.1.2/src/google/appengine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.420724 appengine-python-standard-1.1.2/src/google/appengine/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.424725 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4766 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4565 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/dfa.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5416 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/dottreegen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10171 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1004 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/extras.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6616 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    40831 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/recognizers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34633 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/streams.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9197 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/tokens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    55086 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/tree.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15019 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/treewizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.432725 appengine-python-standard-1.1.2/src/google/appengine/api/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2648 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4326 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/api_base_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6637 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/api_testutil.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7038 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/apiproxy_rpc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5483 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/apiproxy_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23020 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/apiproxy_stub_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.436726 appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1184 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2487 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/_metadata_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13352 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8066 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_defaultcredentialsbased_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8537 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_keybased_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9244 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2728 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8305 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_stub_base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    92389 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/appinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5506 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/appinfo_errors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5858 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/backendinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.436726 appengine-python-standard-1.1.2/src/google/appengine/api/background_thread/
--rwxr-xr-x   0 runner    (1001) docker     (123)      705 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/background_thread/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4207 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/background_thread/background_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.436726 appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/
--rwxr-xr-x   0 runner    (1001) docker     (123)      686 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1722 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blob_storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17082 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blobstore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8934 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blobstore_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15313 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blobstore_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2975 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blobstore_stub_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1815 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/dict_blob_storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4402 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/file_blob_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.436726 appengine-python-standard-1.1.2/src/google/appengine/api/capabilities/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6171 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/capabilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3227 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/capabilities/capability_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5127 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/capabilities/capability_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3816 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/cmp_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6304 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/croninfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    94133 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/datastore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2641 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/datastore_admin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12012 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/datastore_entities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4349 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/datastore_errors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23483 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/datastore_file_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    65487 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/datastore_types.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6643 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/dispatchinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3566 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/full_app_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.440726 appengine-python-standard-1.1.2/src/google/appengine/api/images/
--rwxr-xr-x   0 runner    (1001) docker     (123)    76512 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/images/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2607 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/images/image_comparison.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2210 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/images/images_blob_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15751 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/images/images_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25149 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/images/images_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12487 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/lib_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    56706 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/mail.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1718 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/mail_errors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4303 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/mail_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16788 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/mail_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4871 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/mail_stub_service_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.440726 appengine-python-standard-1.1.2/src/google/appengine/api/memcache/
--rwxr-xr-x   0 runner    (1001) docker     (123)    54575 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/memcache/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17524 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/memcache/memcache_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18037 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/memcache/memcache_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4122 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/memcache/memcache_stub_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5450 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/module_testutil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.440726 appengine-python-standard-1.1.2/src/google/appengine/api/modules/
--rwxr-xr-x   0 runner    (1001) docker     (123)      678 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/modules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15352 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/modules/modules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10494 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/modules/modules_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5951 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/modules/modules_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.440726 appengine-python-standard-1.1.2/src/google/appengine/api/namespace_manager/
--rwxr-xr-x   0 runner    (1001) docker     (123)      711 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/namespace_manager/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2828 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/namespace_manager/namespace_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.440726 appengine-python-standard-1.1.2/src/google/appengine/api/oauth/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1061 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/oauth/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8589 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/oauth/oauth_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10946 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/queueinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24147 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/request_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.440726 appengine-python-standard-1.1.2/src/google/appengine/api/runtime/
--rwxr-xr-x   0 runner    (1001) docker     (123)      709 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/runtime/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3314 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/runtime/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.444726 appengine-python-standard-1.1.2/src/google/appengine/api/search/
--rwxr-xr-x   0 runner    (1001) docker     (123)    39873 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/ExpressionLexer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    55393 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/ExpressionParser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28531 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/QueryLexer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    82233 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/QueryParser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5199 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/expression_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2000 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/geo_util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8248 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/query_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   139421 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17321 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/search_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5749 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/search_util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    40299 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/simple_search_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.448727 appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/
--rwxr-xr-x   0 runner    (1001) docker     (123)      601 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18579 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/document_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20569 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/expression_evaluator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13705 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/simple_facet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5815 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/simple_tokenizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3229 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/tokens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2237 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/search/unicode_util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1765 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/stublib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.448727 appengine-python-standard-1.1.2/src/google/appengine/api/system/
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/system/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5013 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/system/system_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3545 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/system/system_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.448727 appengine-python-standard-1.1.2/src/google/appengine/api/taskqueue/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1854 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/taskqueue/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    96230 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/taskqueue/taskqueue.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    39984 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/taskqueue/taskqueue_service_bytes_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   103352 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/taskqueue/taskqueue_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4393 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/titanoboa_request_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17484 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/urlfetch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2624 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/urlfetch_errors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5949 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/urlfetch_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18940 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/urlfetch_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6192 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/user_service_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7422 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/user_service_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9540 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/users.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47815 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/validation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13341 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/yaml_builder.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2955 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/yaml_errors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8120 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/yaml_listener.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9368 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/yaml_object.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5539 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/api/yaml_test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.448727 appengine-python-standard-1.1.2/src/google/appengine/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/base/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3147 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/base/capabilities_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.456727 appengine-python-standard-1.1.2/src/google/appengine/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2996 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/action_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1835 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/cloud_datastore_v1_remote_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20288 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/cloud_datastore_v1_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    38410 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/cloud_datastore_validator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31628 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_index.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6350 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_index_xml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1582 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_pb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    57902 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_pbs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   110009 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_query.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    97472 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_rpc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17779 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_stub_index.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   173811 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_stub_util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36343 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_v3_bytes_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25116 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_v4_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14281 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_v4_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    39296 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_v4_validator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6730 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/document_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19017 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/entity_bytes_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5968 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/entity_v4_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1990 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/snapshot_pb2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17703 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/datastore/sortable_pb_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.456727 appengine-python-standard-1.1.2/src/google/appengine/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.456727 appengine-python-standard-1.1.2/src/google/appengine/ext/blobstore/
--rwxr-xr-x   0 runner    (1001) docker     (123)      686 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/blobstore/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50088 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/blobstore/blobstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.456727 appengine-python-standard-1.1.2/src/google/appengine/ext/db/
--rwxr-xr-x   0 runner    (1001) docker     (123)   126163 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/db/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9980 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/db/metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12855 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/db/polymodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13730 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/db/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4993 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/db/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.460728 appengine-python-standard-1.1.2/src/google/appengine/ext/deferred/
--rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/deferred/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14355 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/deferred/deferred.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.460728 appengine-python-standard-1.1.2/src/google/appengine/ext/gql/
--rwxr-xr-x   0 runner    (1001) docker     (123)    44600 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/gql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.460728 appengine-python-standard-1.1.2/src/google/appengine/ext/key_range/
--rwxr-xr-x   0 runner    (1001) docker     (123)    27878 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/key_range/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.464728 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15403 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/blobstore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43446 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/context.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1995 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/django_middleware.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9344 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/eventloop.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30714 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/key.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21525 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/key_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9859 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   130896 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8545 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/polymodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    66131 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/query.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14590 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37881 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/tasklets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6591 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/test_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5606 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.464728 appengine-python-standard-1.1.2/src/google/appengine/ext/remote_api/
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/remote_api/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6866 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/remote_api/remote_api_bytes_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.464728 appengine-python-standard-1.1.2/src/google/appengine/ext/testbed/
--rwxr-xr-x   0 runner    (1001) docker     (123)    32956 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/ext/testbed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.464728 appengine-python-standard-1.1.2/src/google/appengine/runtime/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1607 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      798 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/apiproxy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3096 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/apiproxy_errors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6655 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/background.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1480 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.468728 appengine-python-standard-1.1.2/src/google/appengine/runtime/context/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1582 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/context/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6143 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/context/ctx_test_util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1875 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/context/gae_headers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1723 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/context/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10909 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/default_api_stub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5666 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/initialize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10837 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/middlewares.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4553 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/request_environment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4117 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/runtime/thread_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:45:09.468728 appengine-python-standard-1.1.2/src/google/appengine/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      904 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/tools/app_engine_config_exception.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1411 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/tools/os_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8563 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/tools/queue_xml_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1774 2023-05-31 17:44:56.000000 appengine-python-standard-1.1.2/src/google/appengine/tools/xml_parser_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.458986 appengine-python-standard-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-21 20:07:02.454986 appengine-python-standard-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 20:07:02.458986 appengine-python-standard-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.426986 appengine-python-standard-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.426986 appengine-python-standard-1.1.3/src/appengine_python_standard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-21 20:07:02.000000 appengine-python-standard-1.1.3/src/appengine_python_standard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-21 20:07:02.000000 appengine-python-standard-1.1.3/src/appengine_python_standard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:07:02.000000 appengine-python-standard-1.1.3/src/appengine_python_standard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 20:07:02.000000 appengine-python-standard-1.1.3/src/appengine_python_standard.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-21 20:07:02.000000 appengine-python-standard-1.1.3/src/appengine_python_standard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 20:07:02.000000 appengine-python-standard-1.1.3/src/appengine_python_standard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.430986 appengine-python-standard-1.1.3/src/google/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.430986 appengine-python-standard-1.1.3/src/google/appengine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.430986 appengine-python-standard-1.1.3/src/google/appengine/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/_internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.430986 appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4766 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4565 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/dfa.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5416 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/dottreegen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10171 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1004 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/extras.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6616 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40831 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/recognizers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34633 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/streams.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9197 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/tokens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55086 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/tree.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15019 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/treewizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.438986 appengine-python-standard-1.1.3/src/google/appengine/api/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2648 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4326 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/api_base_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6637 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/api_testutil.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7038 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/apiproxy_rpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5483 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/apiproxy_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23020 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/apiproxy_stub_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.438986 appengine-python-standard-1.1.3/src/google/appengine/api/app_identity/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1184 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/app_identity/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2487 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/app_identity/_metadata_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13352 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/app_identity/app_identity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8066 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/app_identity/app_identity_defaultcredentialsbased_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8537 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/app_identity/app_identity_keybased_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9244 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/app_identity/app_identity_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2728 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/app_identity/app_identity_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8305 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/app_identity/app_identity_stub_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    92389 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/appinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5506 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/appinfo_errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5858 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/backendinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.438986 appengine-python-standard-1.1.3/src/google/appengine/api/background_thread/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      705 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/background_thread/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4207 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/background_thread/background_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.438986 appengine-python-standard-1.1.3/src/google/appengine/api/blobstore/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      686 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/blobstore/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1722 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/blobstore/blob_storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17082 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/blobstore/blobstore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8934 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/blobstore/blobstore_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15313 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/blobstore/blobstore_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2975 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/blobstore/blobstore_stub_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1815 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/blobstore/dict_blob_storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4402 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/blobstore/file_blob_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.438986 appengine-python-standard-1.1.3/src/google/appengine/api/capabilities/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6171 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/capabilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3227 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/capabilities/capability_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5127 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/capabilities/capability_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3816 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/cmp_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6304 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/croninfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    94133 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/datastore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2641 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/datastore_admin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12012 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/datastore_entities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4349 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/datastore_errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23483 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/datastore_file_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    65487 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/datastore_types.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6643 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/dispatchinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3566 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/full_app_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.438986 appengine-python-standard-1.1.3/src/google/appengine/api/images/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    76512 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/images/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2607 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/images/image_comparison.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2210 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/images/images_blob_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15751 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/images/images_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25149 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/images/images_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12487 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/lib_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    56706 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/mail.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1718 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/mail_errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4303 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/mail_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16788 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/mail_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4871 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/mail_stub_service_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.442986 appengine-python-standard-1.1.3/src/google/appengine/api/memcache/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54575 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/memcache/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17524 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/memcache/memcache_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18037 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/memcache/memcache_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4122 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/memcache/memcache_stub_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5450 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/module_testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.442986 appengine-python-standard-1.1.3/src/google/appengine/api/modules/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      678 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/modules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15352 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/modules/modules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10494 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/modules/modules_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5951 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/modules/modules_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.442986 appengine-python-standard-1.1.3/src/google/appengine/api/namespace_manager/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      711 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/namespace_manager/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2828 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/namespace_manager/namespace_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.442986 appengine-python-standard-1.1.3/src/google/appengine/api/oauth/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1061 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/oauth/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8589 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/oauth/oauth_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10946 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/queueinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24147 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/request_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.442986 appengine-python-standard-1.1.3/src/google/appengine/api/runtime/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      709 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/runtime/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3314 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/runtime/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.442986 appengine-python-standard-1.1.3/src/google/appengine/api/search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39873 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/search/ExpressionLexer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55393 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/search/ExpressionParser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28531 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/search/QueryLexer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    82233 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/search/QueryParser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5199 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/search/expression_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2000 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/search/geo_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8248 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/search/query_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   140625 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/search/search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17366 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/search/search_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5749 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/search/search_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40851 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/search/simple_search_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.442986 appengine-python-standard-1.1.3/src/google/appengine/api/search/stub/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      601 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/search/stub/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18579 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/search/stub/document_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20569 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/search/stub/expression_evaluator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13705 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/search/stub/simple_facet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5815 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/search/stub/simple_tokenizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3229 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/search/stub/tokens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2237 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/search/unicode_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1765 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/stublib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.446986 appengine-python-standard-1.1.3/src/google/appengine/api/system/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/system/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5013 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/system/system_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3545 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/system/system_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.446986 appengine-python-standard-1.1.3/src/google/appengine/api/taskqueue/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1854 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/taskqueue/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    96230 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/taskqueue/taskqueue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39984 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/taskqueue/taskqueue_service_bytes_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   103352 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/taskqueue/taskqueue_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4393 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/titanoboa_request_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17484 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/urlfetch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2624 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/urlfetch_errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5949 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/urlfetch_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18940 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/urlfetch_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6192 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/user_service_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7422 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/user_service_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9540 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/users.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47815 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/validation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13341 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/yaml_builder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2955 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/yaml_errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8120 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/yaml_listener.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9368 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/yaml_object.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5539 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/api/yaml_test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.446986 appengine-python-standard-1.1.3/src/google/appengine/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/base/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3147 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/base/capabilities_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.450986 appengine-python-standard-1.1.3/src/google/appengine/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2996 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/action_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1835 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/cloud_datastore_v1_remote_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20288 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/cloud_datastore_v1_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38410 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/cloud_datastore_validator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31628 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_index.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6350 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_index_xml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1582 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_pb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57902 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_pbs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   110009 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_query.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    97472 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_rpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17901 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_stub_index.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   173811 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_stub_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36343 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_v3_bytes_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25116 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_v4_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14281 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_v4_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39296 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_v4_validator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6730 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/document_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19017 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/entity_bytes_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5968 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/entity_v4_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1990 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/snapshot_pb2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17703 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/datastore/sortable_pb_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.450986 appengine-python-standard-1.1.3/src/google/appengine/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.450986 appengine-python-standard-1.1.3/src/google/appengine/ext/blobstore/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      686 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/blobstore/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50088 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/blobstore/blobstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.450986 appengine-python-standard-1.1.3/src/google/appengine/ext/db/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   126163 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/db/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9980 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/db/metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12855 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/db/polymodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13730 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/db/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4993 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/db/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.450986 appengine-python-standard-1.1.3/src/google/appengine/ext/deferred/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/deferred/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14355 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/deferred/deferred.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.450986 appengine-python-standard-1.1.3/src/google/appengine/ext/gql/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44600 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/gql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.450986 appengine-python-standard-1.1.3/src/google/appengine/ext/key_range/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27878 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/key_range/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.454986 appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15403 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/blobstore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43446 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/context.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1995 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/django_middleware.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9344 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/eventloop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30714 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/key.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21525 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/key_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9859 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   130896 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8545 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/polymodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    66131 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/query.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14590 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37881 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/tasklets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6591 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/test_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5606 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.454986 appengine-python-standard-1.1.3/src/google/appengine/ext/remote_api/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/remote_api/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6866 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/remote_api/remote_api_bytes_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.454986 appengine-python-standard-1.1.3/src/google/appengine/ext/testbed/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33561 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/ext/testbed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.454986 appengine-python-standard-1.1.3/src/google/appengine/runtime/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1607 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/runtime/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      798 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/runtime/apiproxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3096 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/runtime/apiproxy_errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6655 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/runtime/background.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1480 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/runtime/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.454986 appengine-python-standard-1.1.3/src/google/appengine/runtime/context/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1582 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/runtime/context/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6143 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/runtime/context/ctx_test_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1875 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/runtime/context/gae_headers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1723 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/runtime/context/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10909 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/runtime/default_api_stub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5666 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/runtime/initialize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10837 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/runtime/middlewares.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4553 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/runtime/request_environment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4117 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/runtime/thread_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:07:02.454986 appengine-python-standard-1.1.3/src/google/appengine/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      904 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/tools/app_engine_config_exception.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1411 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/tools/os_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8563 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/tools/queue_xml_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1774 2023-07-21 20:06:47.000000 appengine-python-standard-1.1.3/src/google/appengine/tools/xml_parser_utils.py
```

### Comparing `appengine-python-standard-1.1.2/LICENSE` & `appengine-python-standard-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/PKG-INFO` & `appengine-python-standard-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appengine-python-standard
-Version: 1.1.2
+Version: 1.1.3
 Summary: Google App Engine services SDK for Python 3
 Home-page: https://github.com/GoogleCloudPlatform/appengine-python-standard
 Author: Google LLC
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <4
```

### Comparing `appengine-python-standard-1.1.2/README.md` & `appengine-python-standard-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/setup.py` & `appengine-python-standard-1.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="appengine-python-standard",
-    version="1.1.2",
+    version="1.1.3",
     author="Google LLC",
     description="Google App Engine services SDK for Python 3",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/GoogleCloudPlatform/appengine-python-standard",
     packages=setuptools.find_packages(where="src"),
     namespace_packages=["google"],
```

### Comparing `appengine-python-standard-1.1.2/src/appengine_python_standard.egg-info/PKG-INFO` & `appengine-python-standard-1.1.3/src/appengine_python_standard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appengine-python-standard
-Version: 1.1.2
+Version: 1.1.3
 Summary: Google App Engine services SDK for Python 3
 Home-page: https://github.com/GoogleCloudPlatform/appengine-python-standard
 Author: Google LLC
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <4
```

### Comparing `appengine-python-standard-1.1.2/src/appengine_python_standard.egg-info/SOURCES.txt` & `appengine-python-standard-1.1.3/src/appengine_python_standard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/__init__.py` & `appengine-python-standard-1.1.3/src/google/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/compat.py` & `appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/compat.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/constants.py` & `appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/constants.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/dfa.py` & `appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/dfa.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/dottreegen.py` & `appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/dottreegen.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/exceptions.py` & `appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/exceptions.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/extras.py` & `appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/extras.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/main.py` & `appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/main.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/recognizers.py` & `appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/recognizers.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/streams.py` & `appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/streams.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/tokens.py` & `appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/tokens.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/tree.py` & `appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/tree.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/_internal/antlr3/treewizard.py` & `appengine-python-standard-1.1.3/src/google/appengine/_internal/antlr3/treewizard.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/api_base_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/api_base_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/api_testutil.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/api_testutil.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/apiproxy_rpc.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/apiproxy_rpc.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/apiproxy_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/apiproxy_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/apiproxy_stub_map.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/apiproxy_stub_map.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/app_identity/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/_metadata_server.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/app_identity/_metadata_server.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/app_identity/app_identity.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_defaultcredentialsbased_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/app_identity/app_identity_defaultcredentialsbased_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_keybased_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/app_identity/app_identity_keybased_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_service_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/app_identity/app_identity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/app_identity/app_identity_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/app_identity/app_identity_stub_base.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/app_identity/app_identity_stub_base.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/appinfo.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/appinfo.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/appinfo_errors.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/appinfo_errors.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/backendinfo.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/backendinfo.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/background_thread/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/background_thread/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/background_thread/background_thread.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/background_thread/background_thread.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/blobstore/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blob_storage.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/blobstore/blob_storage.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blobstore.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/blobstore/blobstore.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blobstore_service_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/blobstore/blobstore_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blobstore_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/blobstore/blobstore_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/blobstore_stub_service_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/blobstore/blobstore_stub_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/dict_blob_storage.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/blobstore/dict_blob_storage.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/blobstore/file_blob_storage.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/blobstore/file_blob_storage.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/capabilities/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/capabilities/capability_service_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/capabilities/capability_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/capabilities/capability_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/capabilities/capability_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/cmp_compat.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/cmp_compat.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/croninfo.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/croninfo.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/datastore.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/datastore.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/datastore_admin.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/datastore_admin.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/datastore_entities.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/datastore_entities.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/datastore_errors.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/datastore_errors.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/datastore_file_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/datastore_file_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/datastore_types.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/datastore_types.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/dispatchinfo.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/dispatchinfo.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/full_app_id.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/full_app_id.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/images/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/images/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/images/image_comparison.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/images/image_comparison.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/images/images_blob_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/images/images_blob_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/images/images_service_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/images/images_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/images/images_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/images/images_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/lib_config.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/lib_config.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/mail.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/mail.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/mail_errors.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/mail_errors.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/mail_service_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/mail_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/mail_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/mail_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/mail_stub_service_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/mail_stub_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/memcache/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/memcache/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/memcache/memcache_service_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/memcache/memcache_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/memcache/memcache_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/memcache/memcache_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/memcache/memcache_stub_service_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/memcache/memcache_stub_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/module_testutil.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/module_testutil.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/modules/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/modules/modules.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/modules/modules.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/modules/modules_service_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/modules/modules_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/modules/modules_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/modules/modules_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/namespace_manager/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/namespace_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/namespace_manager/namespace_manager.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/namespace_manager/namespace_manager.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/oauth/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/oauth/oauth_api.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/oauth/oauth_api.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/queueinfo.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/queueinfo.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/request_info.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/request_info.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/runtime/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/runtime/runtime.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/search/ExpressionLexer.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/search/ExpressionLexer.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/search/ExpressionParser.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/search/ExpressionParser.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/search/QueryLexer.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/search/QueryLexer.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/search/QueryParser.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/search/QueryParser.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/search/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/search/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/search/expression_parser.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/search/expression_parser.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/search/geo_util.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/search/geo_util.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/search/query_parser.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/search/query_parser.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/search/search.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/search/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -879,54 +879,78 @@
   ])
 
 
 @datastore_rpc._positional(7)
 def get_indexes(namespace='', offset=None, limit=20,
                 start_index_name=None, include_start_index=True,
                 index_name_prefix=None, fetch_schema=False, deadline=None,
-                **kwargs):
+                all_namespaces=None, **kwargs):
   """Returns a list of available indexes.
 
   Args:
     namespace: The namespace of indexes to be returned. If not set
       then the current namespace is used.
     offset: The offset of the first returned index.
     limit: The number of indexes to return.
     start_index_name: The name of the first index to be returned.
     include_start_index: Whether or not to return the start index.
     index_name_prefix: The prefix used to select returned indexes.
     fetch_schema: Whether to retrieve Schema for each Index or not.
-
-  Kwargs:
-    deadline: Deadline for RPC call in seconds; if None use the default.
+    deadline: Deadline for RPC calls in seconds; if None use the default.
+    all_namespaces: Whether to return indexes from all namespaces.
+    **kwargs: Additional kwargs.
 
   Returns:
     The GetResponse containing a list of available indexes.
 
   Raises:
     InternalError: If the request fails on internal servers.
     TypeError: If any of the parameters have invalid types, or an unknown
       attribute is passed.
     ValueError: If any of the parameters have invalid values (e.g., a
       negative deadline).
   """
   return get_indexes_async(
       namespace, offset, limit, start_index_name, include_start_index,
-      index_name_prefix, fetch_schema, deadline=deadline, **kwargs).get_result()
+      index_name_prefix, fetch_schema, deadline=deadline,
+      all_namespaces=all_namespaces, **kwargs).get_result()
 
 
 @datastore_rpc._positional(7)
 def get_indexes_async(namespace='', offset=None, limit=20,
                       start_index_name=None, include_start_index=True,
                       index_name_prefix=None, fetch_schema=False, deadline=None,
-                      **kwargs):
+                      all_namespaces=None, **kwargs):
   """Asynchronously returns a list of available indexes.
 
-  Identical to get_indexes() except that it returns a future. Call
-  get_result() on the return value to block on the call and get its result.
+  Identical to get_indexes() except that it returns a future.
+
+  Args:
+    namespace: The namespace of indexes to be returned. If not set
+      then the current namespace is used.
+    offset: The offset of the first returned index.
+    limit: The number of indexes to return.
+    start_index_name: The name of the first index to be returned.
+    include_start_index: Whether or not to return the start index.
+    index_name_prefix: The prefix used to select returned indexes.
+    fetch_schema: Whether to retrieve Schema for each Index or not.
+    deadline: Deadline for RPC calls in seconds; if None use the default.
+    all_namespaces: Whether to return indexes from all namespaces.
+    **kwargs: Additional kwargs.
+
+  Returns:
+    A future. Call get_result() on the return value to block on the call and get
+    its result.
+
+  Raises:
+    InternalError: If the request fails on internal servers.
+    TypeError: If any of the parameters have invalid types, or an unknown
+      attribute is passed.
+    ValueError: If any of the parameters have invalid values (e.g., a
+      negative deadline).
   """
 
   app_id = kwargs.pop('app_id', None)
   if kwargs:
     raise TypeError('Invalid arguments: %s' % ', '.join(kwargs))
 
   request = search_service_pb2.ListIndexesRequest()
@@ -956,14 +980,16 @@
     params.include_start_index = bool(include_start_index)
   if index_name_prefix is not None:
     params.index_name_prefix = _ValidateString(
         index_name_prefix,
         'index_name_prefix',
         MAXIMUM_INDEX_NAME_LENGTH,
         empty_ok=False)
+  if all_namespaces is not None:
+    params.all_namespaces = bool(all_namespaces)
   params.fetch_schema = fetch_schema
 
   response = search_service_pb2.ListIndexesResponse()
   if app_id:
     request.app_id = app_id
 
   def hook():
```

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/search/search_service_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/search/search_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,21 +26,20 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.appengine.datastore import document_pb2 as google_dot_appengine_dot_datastore_dot_document__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0google/appengine/api/search/search_service.proto\x12\x10google.appengine\x1a)google/appengine/datastore/document.proto\"\xa8\x01\n\x12SearchServiceError\"\x91\x01\n\tErrorCode\x12\x06\n\x02OK\x10\x00\x12\x13\n\x0fINVALID_REQUEST\x10\x01\x12\x13\n\x0fTRANSIENT_ERROR\x10\x02\x12\x12\n\x0eINTERNAL_ERROR\x10\x03\x12\x15\n\x11PERMISSION_DENIED\x10\x04\x12\x0b\n\x07TIMEOUT\x10\x05\x12\x1a\n\x16\x43ONCURRENT_TRANSACTION\x10\x06\"{\n\rRequestStatus\x12<\n\x04\x63ode\x18\x01 \x01(\x0e\x32..google.appengine.SearchServiceError.ErrorCode\x12\x14\n\x0c\x65rror_detail\x18\x02 \x01(\t\x12\x16\n\x0e\x63\x61nonical_code\x18\x03 \x01(\x05\"\x8a\x03\n\tIndexSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12J\n\x0b\x63onsistency\x18\x02 \x01(\x0e\x32\'.google.appengine.IndexSpec.Consistency:\x0cPER_DOCUMENT\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\x05\x12:\n\x06source\x18\x05 \x01(\x0e\x32\".google.appengine.IndexSpec.Source:\x06SEARCH\x12\x38\n\x04mode\x18\x06 \x01(\x0e\x32 .google.appengine.IndexSpec.Mode:\x08PRIORITY\"+\n\x0b\x43onsistency\x12\n\n\x06GLOBAL\x10\x00\x12\x10\n\x0cPER_DOCUMENT\x10\x01\"6\n\x06Source\x12\n\n\x06SEARCH\x10\x00\x12\r\n\tDATASTORE\x10\x01\x12\x11\n\rCLOUD_STORAGE\x10\x02\"$\n\x04Mode\x12\x0c\n\x08PRIORITY\x10\x00\x12\x0e\n\nBACKGROUND\x10\x01\"\x8d\x03\n\rIndexMetadata\x12/\n\nindex_spec\x18\x01 \x01(\x0b\x32\x1b.google.appengine.IndexSpec\x12.\n\x05\x66ield\x18\x02 \x03(\x0b\x32\x1f.storage_onestore_v3.FieldTypes\x12\x38\n\x07storage\x18\x03 \x01(\x0b\x32\'.google.appengine.IndexMetadata.Storage\x12G\n\x0bindex_state\x18\x04 \x01(\x0e\x32*.google.appengine.IndexMetadata.IndexState:\x06\x41\x43TIVE\x12\x19\n\x11index_delete_time\x18\x05 \x01(\x03\x12\x15\n\nnum_shards\x18\x06 \x01(\x05:\x01\x31\x1a-\n\x07Storage\x12\x13\n\x0b\x61mount_used\x18\x01 \x01(\x03\x12\r\n\x05limit\x18\x02 \x01(\x03\"7\n\nIndexState\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\x10\n\x0cSOFT_DELETED\x10\x01\x12\x0b\n\x07PURGING\x10\x02\"\x83\x02\n\x13IndexDocumentParams\x12/\n\x08\x64ocument\x18\x01 \x03(\x0b\x32\x1d.storage_onestore_v3.Document\x12U\n\tfreshness\x18\x02 \x01(\x0e\x32/.google.appengine.IndexDocumentParams.Freshness:\rSYNCHRONOUSLYB\x02\x18\x01\x12/\n\nindex_spec\x18\x03 \x01(\x0b\x32\x1b.google.appengine.IndexSpec\"3\n\tFreshness\x12\x11\n\rSYNCHRONOUSLY\x10\x00\x12\x13\n\x0fWHEN_CONVENIENT\x10\x01\"]\n\x14IndexDocumentRequest\x12\x35\n\x06params\x18\x01 \x01(\x0b\x32%.google.appengine.IndexDocumentParams\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\x0c\"`\n\x15IndexDocumentResponse\x12/\n\x06status\x18\x01 \x03(\x0b\x32\x1f.google.appengine.RequestStatus\x12\x0e\n\x06\x64oc_id\x18\x02 \x03(\t*\x06\x08\xe8\x07\x10\x90N\"W\n\x14\x44\x65leteDocumentParams\x12\x0e\n\x06\x64oc_id\x18\x01 \x03(\t\x12/\n\nindex_spec\x18\x02 \x01(\x0b\x32\x1b.google.appengine.IndexSpec\"_\n\x15\x44\x65leteDocumentRequest\x12\x36\n\x06params\x18\x01 \x01(\x0b\x32&.google.appengine.DeleteDocumentParams\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\x0c\"I\n\x16\x44\x65leteDocumentResponse\x12/\n\x06status\x18\x01 \x03(\x0b\x32\x1f.google.appengine.RequestStatus\"\xa4\x01\n\x13ListDocumentsParams\x12/\n\nindex_spec\x18\x01 \x01(\x0b\x32\x1b.google.appengine.IndexSpec\x12\x14\n\x0cstart_doc_id\x18\x02 \x01(\t\x12\x1f\n\x11include_start_doc\x18\x03 \x01(\x08:\x04true\x12\x12\n\x05limit\x18\x04 \x01(\x05:\x03\x31\x30\x30\x12\x11\n\tkeys_only\x18\x05 \x01(\x08\"]\n\x14ListDocumentsRequest\x12\x35\n\x06params\x18\x01 \x01(\x0b\x32%.google.appengine.ListDocumentsParams\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\x0c\"y\n\x15ListDocumentsResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.google.appengine.RequestStatus\x12/\n\x08\x64ocument\x18\x02 \x03(\x0b\x32\x1d.storage_onestore_v3.Document\"D\n\x11\x44\x65leteIndexParams\x12/\n\nindex_spec\x18\x01 \x01(\x0b\x32\x1b.google.appengine.IndexSpec\"Y\n\x12\x44\x65leteIndexRequest\x12\x33\n\x06params\x18\x01 \x01(\x0b\x32#.google.appengine.DeleteIndexParams\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\x0c\"F\n\x13\x44\x65leteIndexResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.google.appengine.RequestStatus\"J\n\x17\x43\x61ncelDeleteIndexParams\x12/\n\nindex_spec\x18\x01 \x01(\x0b\x32\x1b.google.appengine.IndexSpec\"e\n\x18\x43\x61ncelDeleteIndexRequest\x12\x39\n\x06params\x18\x01 \x01(\x0b\x32).google.appengine.CancelDeleteIndexParams\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\x0c\"L\n\x19\x43\x61ncelDeleteIndexResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.google.appengine.RequestStatus\"\xf3\x01\n\x11ListIndexesParams\x12\x14\n\x0c\x66\x65tch_schema\x18\x01 \x01(\x08\x12\x11\n\x05limit\x18\x02 \x01(\x05:\x02\x32\x30\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x18\n\x10start_index_name\x18\x04 \x01(\t\x12!\n\x13include_start_index\x18\x05 \x01(\x08:\x04true\x12\x19\n\x11index_name_prefix\x18\x06 \x01(\t\x12\x0e\n\x06offset\x18\x07 \x01(\x05\x12:\n\x06source\x18\x08 \x01(\x0e\x32\".google.appengine.IndexSpec.Source:\x06SEARCH\"Y\n\x12ListIndexesRequest\x12\x33\n\x06params\x18\x01 \x01(\x0b\x32#.google.appengine.ListIndexesParams\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\x0c\"\x7f\n\x13ListIndexesResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.google.appengine.RequestStatus\x12\x37\n\x0eindex_metadata\x18\x02 \x03(\x0b\x32\x1f.google.appengine.IndexMetadata\"\x9e\x01\n\x12\x44\x65leteSchemaParams\x12:\n\x06source\x18\x01 \x01(\x0e\x32\".google.appengine.IndexSpec.Source:\x06SEARCH\x12/\n\nindex_spec\x18\x02 \x03(\x0b\x32\x1b.google.appengine.IndexSpec\x12\x1b\n\x13require_empty_index\x18\x03 \x01(\x08\"[\n\x13\x44\x65leteSchemaRequest\x12\x34\n\x06params\x18\x01 \x01(\x0b\x32$.google.appengine.DeleteSchemaParams\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\x0c\"G\n\x14\x44\x65leteSchemaResponse\x12/\n\x06status\x18\x01 \x03(\x0b\x32\x1f.google.appengine.RequestStatus\"}\n\x08SortSpec\x12\x17\n\x0fsort_expression\x18\x01 \x01(\t\x12\x1d\n\x0fsort_descending\x18\x02 \x01(\x08:\x04true\x12\x1a\n\x12\x64\x65\x66\x61ult_value_text\x18\x04 \x01(\t\x12\x1d\n\x15\x64\x65\x66\x61ult_value_numeric\x18\x05 \x01(\x01\"\xbd\x01\n\nScorerSpec\x12\x41\n\x06scorer\x18\x01 \x01(\x0e\x32#.google.appengine.ScorerSpec.Scorer:\x0cMATCH_SCORER\x12\x13\n\x05limit\x18\x02 \x01(\x05:\x04\x31\x30\x30\x30\x12\x1f\n\x17match_scorer_parameters\x18\t \x01(\t\"6\n\x06Scorer\x12\x1a\n\x16RESCORING_MATCH_SCORER\x10\x00\x12\x10\n\x0cMATCH_SCORER\x10\x02\"\x85\x01\n\tFieldSpec\x12\x0c\n\x04name\x18\x01 \x03(\t\x12:\n\nexpression\x18\x02 \x03(\n2&.google.appengine.FieldSpec.Expression\x1a.\n\nExpression\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\nexpression\x18\x04 \x01(\t\"6\n\nFacetRange\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\t\x12\x0b\n\x03\x65nd\x18\x03 \x01(\t\"o\n\x11\x46\x61\x63\x65tRequestParam\x12\x13\n\x0bvalue_limit\x18\x01 \x01(\x05\x12+\n\x05range\x18\x02 \x03(\x0b\x32\x1c.google.appengine.FacetRange\x12\x18\n\x10value_constraint\x18\x03 \x03(\t\"/\n\x14\x46\x61\x63\x65tAutoDetectParam\x12\x17\n\x0bvalue_limit\x18\x01 \x01(\x05:\x02\x31\x30\"Q\n\x0c\x46\x61\x63\x65tRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x33\n\x06params\x18\x02 \x01(\x0b\x32#.google.appengine.FacetRequestParam\"\x8b\x01\n\x0f\x46\x61\x63\x65tRefinement\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x36\n\x05range\x18\x03 \x01(\x0b\x32\'.google.appengine.FacetRefinement.Range\x1a#\n\x05Range\x12\r\n\x05start\x18\x01 \x01(\t\x12\x0b\n\x03\x65nd\x18\x02 \x01(\t\"\xd6\x06\n\x0cSearchParams\x12/\n\nindex_spec\x18\x01 \x01(\x0b\x32\x1b.google.appengine.IndexSpec\x12\r\n\x05query\x18\x02 \x01(\t\x12\x0e\n\x06\x63ursor\x18\x04 \x01(\t\x12\x0e\n\x06offset\x18\x0b \x01(\x05\x12\x44\n\x0b\x63ursor_type\x18\x05 \x01(\x0e\x32).google.appengine.SearchParams.CursorType:\x04NONE\x12\x11\n\x05limit\x18\x06 \x01(\x05:\x02\x32\x30\x12\x1e\n\x16matched_count_accuracy\x18\x07 \x01(\x05\x12-\n\tsort_spec\x18\x08 \x03(\x0b\x32\x1a.google.appengine.SortSpec\x12\x31\n\x0bscorer_spec\x18\t \x01(\x0b\x32\x1c.google.appengine.ScorerSpec\x12/\n\nfield_spec\x18\n \x01(\x0b\x32\x1b.google.appengine.FieldSpec\x12\x11\n\tkeys_only\x18\x0c \x01(\x08\x12H\n\x0cparsing_mode\x18\r \x01(\x0e\x32*.google.appengine.SearchParams.ParsingMode:\x06STRICT\x12$\n\x19\x61uto_discover_facet_count\x18\x0f \x01(\x05:\x01\x30\x12\x35\n\rinclude_facet\x18\x10 \x03(\x0b\x32\x1e.google.appengine.FacetRequest\x12;\n\x10\x66\x61\x63\x65t_refinement\x18\x11 \x03(\x0b\x32!.google.appengine.FacetRefinement\x12G\n\x17\x66\x61\x63\x65t_auto_detect_param\x18\x12 \x01(\x0b\x32&.google.appengine.FacetAutoDetectParam\x12\x19\n\x0b\x66\x61\x63\x65t_depth\x18\x13 \x01(\x05:\x04\x31\x30\x30\x30\x12#\n\x14\x65nable_query_rewrite\x18\x14 \x01(\x08:\x05\x66\x61lse\"2\n\nCursorType\x12\x08\n\x04NONE\x10\x00\x12\n\n\x06SINGLE\x10\x01\x12\x0e\n\nPER_RESULT\x10\x02\"&\n\x0bParsingMode\x12\n\n\x06STRICT\x10\x00\x12\x0b\n\x07RELAXED\x10\x01\"O\n\rSearchRequest\x12.\n\x06params\x18\x01 \x01(\x0b\x32\x1e.google.appengine.SearchParams\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\x0c\"f\n\x10\x46\x61\x63\x65tResultValue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\x05\x12\x35\n\nrefinement\x18\x03 \x01(\x0b\x32!.google.appengine.FacetRefinement\"N\n\x0b\x46\x61\x63\x65tResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x31\n\x05value\x18\x02 \x03(\x0b\x32\".google.appengine.FacetResultValue\"\x8e\x01\n\x0cSearchResult\x12/\n\x08\x64ocument\x18\x01 \x01(\x0b\x32\x1d.storage_onestore_v3.Document\x12.\n\nexpression\x18\x04 \x03(\x0b\x32\x1a.storage_onestore_v3.Field\x12\r\n\x05score\x18\x02 \x03(\x01\x12\x0e\n\x06\x63ursor\x18\x03 \x01(\t\"\xea\x01\n\x0eSearchResponse\x12.\n\x06result\x18\x01 \x03(\x0b\x32\x1e.google.appengine.SearchResult\x12\x15\n\rmatched_count\x18\x02 \x01(\x03\x12/\n\x06status\x18\x03 \x01(\x0b\x32\x1f.google.appengine.RequestStatus\x12\x0e\n\x06\x63ursor\x18\x04 \x01(\t\x12\x33\n\x0c\x66\x61\x63\x65t_result\x18\x05 \x03(\x0b\x32\x1d.google.appengine.FacetResult\x12\x13\n\x0b\x64ocs_scored\x18\x06 \x01(\x05*\x06\x08\xe8\x07\x10\x90NB8\n%com.google.appengine.api.search.protoB\x0fSearchServicePb')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0google/appengine/api/search/search_service.proto\x12\x10google.appengine\x1a)google/appengine/datastore/document.proto\"\xa8\x01\n\x12SearchServiceError\"\x91\x01\n\tErrorCode\x12\x06\n\x02OK\x10\x00\x12\x13\n\x0fINVALID_REQUEST\x10\x01\x12\x13\n\x0fTRANSIENT_ERROR\x10\x02\x12\x12\n\x0eINTERNAL_ERROR\x10\x03\x12\x15\n\x11PERMISSION_DENIED\x10\x04\x12\x0b\n\x07TIMEOUT\x10\x05\x12\x1a\n\x16\x43ONCURRENT_TRANSACTION\x10\x06\"{\n\rRequestStatus\x12<\n\x04\x63ode\x18\x01 \x01(\x0e\x32..google.appengine.SearchServiceError.ErrorCode\x12\x14\n\x0c\x65rror_detail\x18\x02 \x01(\t\x12\x16\n\x0e\x63\x61nonical_code\x18\x03 \x01(\x05\"\x8a\x03\n\tIndexSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12J\n\x0b\x63onsistency\x18\x02 \x01(\x0e\x32\'.google.appengine.IndexSpec.Consistency:\x0cPER_DOCUMENT\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\x05\x12:\n\x06source\x18\x05 \x01(\x0e\x32\".google.appengine.IndexSpec.Source:\x06SEARCH\x12\x38\n\x04mode\x18\x06 \x01(\x0e\x32 .google.appengine.IndexSpec.Mode:\x08PRIORITY\"+\n\x0b\x43onsistency\x12\n\n\x06GLOBAL\x10\x00\x12\x10\n\x0cPER_DOCUMENT\x10\x01\"6\n\x06Source\x12\n\n\x06SEARCH\x10\x00\x12\r\n\tDATASTORE\x10\x01\x12\x11\n\rCLOUD_STORAGE\x10\x02\"$\n\x04Mode\x12\x0c\n\x08PRIORITY\x10\x00\x12\x0e\n\nBACKGROUND\x10\x01\"\x8d\x03\n\rIndexMetadata\x12/\n\nindex_spec\x18\x01 \x01(\x0b\x32\x1b.google.appengine.IndexSpec\x12.\n\x05\x66ield\x18\x02 \x03(\x0b\x32\x1f.storage_onestore_v3.FieldTypes\x12\x38\n\x07storage\x18\x03 \x01(\x0b\x32\'.google.appengine.IndexMetadata.Storage\x12G\n\x0bindex_state\x18\x04 \x01(\x0e\x32*.google.appengine.IndexMetadata.IndexState:\x06\x41\x43TIVE\x12\x19\n\x11index_delete_time\x18\x05 \x01(\x03\x12\x15\n\nnum_shards\x18\x06 \x01(\x05:\x01\x31\x1a-\n\x07Storage\x12\x13\n\x0b\x61mount_used\x18\x01 \x01(\x03\x12\r\n\x05limit\x18\x02 \x01(\x03\"7\n\nIndexState\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\x10\n\x0cSOFT_DELETED\x10\x01\x12\x0b\n\x07PURGING\x10\x02\"\x83\x02\n\x13IndexDocumentParams\x12/\n\x08\x64ocument\x18\x01 \x03(\x0b\x32\x1d.storage_onestore_v3.Document\x12U\n\tfreshness\x18\x02 \x01(\x0e\x32/.google.appengine.IndexDocumentParams.Freshness:\rSYNCHRONOUSLYB\x02\x18\x01\x12/\n\nindex_spec\x18\x03 \x01(\x0b\x32\x1b.google.appengine.IndexSpec\"3\n\tFreshness\x12\x11\n\rSYNCHRONOUSLY\x10\x00\x12\x13\n\x0fWHEN_CONVENIENT\x10\x01\"]\n\x14IndexDocumentRequest\x12\x35\n\x06params\x18\x01 \x01(\x0b\x32%.google.appengine.IndexDocumentParams\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\x0c\"`\n\x15IndexDocumentResponse\x12/\n\x06status\x18\x01 \x03(\x0b\x32\x1f.google.appengine.RequestStatus\x12\x0e\n\x06\x64oc_id\x18\x02 \x03(\t*\x06\x08\xe8\x07\x10\x90N\"W\n\x14\x44\x65leteDocumentParams\x12\x0e\n\x06\x64oc_id\x18\x01 \x03(\t\x12/\n\nindex_spec\x18\x02 \x01(\x0b\x32\x1b.google.appengine.IndexSpec\"_\n\x15\x44\x65leteDocumentRequest\x12\x36\n\x06params\x18\x01 \x01(\x0b\x32&.google.appengine.DeleteDocumentParams\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\x0c\"I\n\x16\x44\x65leteDocumentResponse\x12/\n\x06status\x18\x01 \x03(\x0b\x32\x1f.google.appengine.RequestStatus\"\xa4\x01\n\x13ListDocumentsParams\x12/\n\nindex_spec\x18\x01 \x01(\x0b\x32\x1b.google.appengine.IndexSpec\x12\x14\n\x0cstart_doc_id\x18\x02 \x01(\t\x12\x1f\n\x11include_start_doc\x18\x03 \x01(\x08:\x04true\x12\x12\n\x05limit\x18\x04 \x01(\x05:\x03\x31\x30\x30\x12\x11\n\tkeys_only\x18\x05 \x01(\x08\"]\n\x14ListDocumentsRequest\x12\x35\n\x06params\x18\x01 \x01(\x0b\x32%.google.appengine.ListDocumentsParams\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\x0c\"y\n\x15ListDocumentsResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.google.appengine.RequestStatus\x12/\n\x08\x64ocument\x18\x02 \x03(\x0b\x32\x1d.storage_onestore_v3.Document\"D\n\x11\x44\x65leteIndexParams\x12/\n\nindex_spec\x18\x01 \x01(\x0b\x32\x1b.google.appengine.IndexSpec\"Y\n\x12\x44\x65leteIndexRequest\x12\x33\n\x06params\x18\x01 \x01(\x0b\x32#.google.appengine.DeleteIndexParams\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\x0c\"F\n\x13\x44\x65leteIndexResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.google.appengine.RequestStatus\"J\n\x17\x43\x61ncelDeleteIndexParams\x12/\n\nindex_spec\x18\x01 \x01(\x0b\x32\x1b.google.appengine.IndexSpec\"e\n\x18\x43\x61ncelDeleteIndexRequest\x12\x39\n\x06params\x18\x01 \x01(\x0b\x32).google.appengine.CancelDeleteIndexParams\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\x0c\"L\n\x19\x43\x61ncelDeleteIndexResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.google.appengine.RequestStatus\"\x8b\x02\n\x11ListIndexesParams\x12\x14\n\x0c\x66\x65tch_schema\x18\x01 \x01(\x08\x12\x11\n\x05limit\x18\x02 \x01(\x05:\x02\x32\x30\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x18\n\x10start_index_name\x18\x04 \x01(\t\x12!\n\x13include_start_index\x18\x05 \x01(\x08:\x04true\x12\x19\n\x11index_name_prefix\x18\x06 \x01(\t\x12\x0e\n\x06offset\x18\x07 \x01(\x05\x12:\n\x06source\x18\x08 \x01(\x0e\x32\".google.appengine.IndexSpec.Source:\x06SEARCH\x12\x16\n\x0e\x61ll_namespaces\x18\t \x01(\x08\"Y\n\x12ListIndexesRequest\x12\x33\n\x06params\x18\x01 \x01(\x0b\x32#.google.appengine.ListIndexesParams\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\x0c\"\x7f\n\x13ListIndexesResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.google.appengine.RequestStatus\x12\x37\n\x0eindex_metadata\x18\x02 \x03(\x0b\x32\x1f.google.appengine.IndexMetadata\"\x9e\x01\n\x12\x44\x65leteSchemaParams\x12:\n\x06source\x18\x01 \x01(\x0e\x32\".google.appengine.IndexSpec.Source:\x06SEARCH\x12/\n\nindex_spec\x18\x02 \x03(\x0b\x32\x1b.google.appengine.IndexSpec\x12\x1b\n\x13require_empty_index\x18\x03 \x01(\x08\"[\n\x13\x44\x65leteSchemaRequest\x12\x34\n\x06params\x18\x01 \x01(\x0b\x32$.google.appengine.DeleteSchemaParams\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\x0c\"G\n\x14\x44\x65leteSchemaResponse\x12/\n\x06status\x18\x01 \x03(\x0b\x32\x1f.google.appengine.RequestStatus\"}\n\x08SortSpec\x12\x17\n\x0fsort_expression\x18\x01 \x01(\t\x12\x1d\n\x0fsort_descending\x18\x02 \x01(\x08:\x04true\x12\x1a\n\x12\x64\x65\x66\x61ult_value_text\x18\x04 \x01(\t\x12\x1d\n\x15\x64\x65\x66\x61ult_value_numeric\x18\x05 \x01(\x01\"\xbd\x01\n\nScorerSpec\x12\x41\n\x06scorer\x18\x01 \x01(\x0e\x32#.google.appengine.ScorerSpec.Scorer:\x0cMATCH_SCORER\x12\x13\n\x05limit\x18\x02 \x01(\x05:\x04\x31\x30\x30\x30\x12\x1f\n\x17match_scorer_parameters\x18\t \x01(\t\"6\n\x06Scorer\x12\x1a\n\x16RESCORING_MATCH_SCORER\x10\x00\x12\x10\n\x0cMATCH_SCORER\x10\x02\"\x85\x01\n\tFieldSpec\x12\x0c\n\x04name\x18\x01 \x03(\t\x12:\n\nexpression\x18\x02 \x03(\n2&.google.appengine.FieldSpec.Expression\x1a.\n\nExpression\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\nexpression\x18\x04 \x01(\t\"6\n\nFacetRange\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\t\x12\x0b\n\x03\x65nd\x18\x03 \x01(\t\"o\n\x11\x46\x61\x63\x65tRequestParam\x12\x13\n\x0bvalue_limit\x18\x01 \x01(\x05\x12+\n\x05range\x18\x02 \x03(\x0b\x32\x1c.google.appengine.FacetRange\x12\x18\n\x10value_constraint\x18\x03 \x03(\t\"/\n\x14\x46\x61\x63\x65tAutoDetectParam\x12\x17\n\x0bvalue_limit\x18\x01 \x01(\x05:\x02\x31\x30\"Q\n\x0c\x46\x61\x63\x65tRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x33\n\x06params\x18\x02 \x01(\x0b\x32#.google.appengine.FacetRequestParam\"\x8b\x01\n\x0f\x46\x61\x63\x65tRefinement\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x36\n\x05range\x18\x03 \x01(\x0b\x32\'.google.appengine.FacetRefinement.Range\x1a#\n\x05Range\x12\r\n\x05start\x18\x01 \x01(\t\x12\x0b\n\x03\x65nd\x18\x02 \x01(\t\"\xd6\x06\n\x0cSearchParams\x12/\n\nindex_spec\x18\x01 \x01(\x0b\x32\x1b.google.appengine.IndexSpec\x12\r\n\x05query\x18\x02 \x01(\t\x12\x0e\n\x06\x63ursor\x18\x04 \x01(\t\x12\x0e\n\x06offset\x18\x0b \x01(\x05\x12\x44\n\x0b\x63ursor_type\x18\x05 \x01(\x0e\x32).google.appengine.SearchParams.CursorType:\x04NONE\x12\x11\n\x05limit\x18\x06 \x01(\x05:\x02\x32\x30\x12\x1e\n\x16matched_count_accuracy\x18\x07 \x01(\x05\x12-\n\tsort_spec\x18\x08 \x03(\x0b\x32\x1a.google.appengine.SortSpec\x12\x31\n\x0bscorer_spec\x18\t \x01(\x0b\x32\x1c.google.appengine.ScorerSpec\x12/\n\nfield_spec\x18\n \x01(\x0b\x32\x1b.google.appengine.FieldSpec\x12\x11\n\tkeys_only\x18\x0c \x01(\x08\x12H\n\x0cparsing_mode\x18\r \x01(\x0e\x32*.google.appengine.SearchParams.ParsingMode:\x06STRICT\x12$\n\x19\x61uto_discover_facet_count\x18\x0f \x01(\x05:\x01\x30\x12\x35\n\rinclude_facet\x18\x10 \x03(\x0b\x32\x1e.google.appengine.FacetRequest\x12;\n\x10\x66\x61\x63\x65t_refinement\x18\x11 \x03(\x0b\x32!.google.appengine.FacetRefinement\x12G\n\x17\x66\x61\x63\x65t_auto_detect_param\x18\x12 \x01(\x0b\x32&.google.appengine.FacetAutoDetectParam\x12\x19\n\x0b\x66\x61\x63\x65t_depth\x18\x13 \x01(\x05:\x04\x31\x30\x30\x30\x12#\n\x14\x65nable_query_rewrite\x18\x14 \x01(\x08:\x05\x66\x61lse\"2\n\nCursorType\x12\x08\n\x04NONE\x10\x00\x12\n\n\x06SINGLE\x10\x01\x12\x0e\n\nPER_RESULT\x10\x02\"&\n\x0bParsingMode\x12\n\n\x06STRICT\x10\x00\x12\x0b\n\x07RELAXED\x10\x01\"O\n\rSearchRequest\x12.\n\x06params\x18\x01 \x01(\x0b\x32\x1e.google.appengine.SearchParams\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\x0c\"f\n\x10\x46\x61\x63\x65tResultValue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\x05\x12\x35\n\nrefinement\x18\x03 \x01(\x0b\x32!.google.appengine.FacetRefinement\"N\n\x0b\x46\x61\x63\x65tResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x31\n\x05value\x18\x02 \x03(\x0b\x32\".google.appengine.FacetResultValue\"\x8e\x01\n\x0cSearchResult\x12/\n\x08\x64ocument\x18\x01 \x01(\x0b\x32\x1d.storage_onestore_v3.Document\x12.\n\nexpression\x18\x04 \x03(\x0b\x32\x1a.storage_onestore_v3.Field\x12\r\n\x05score\x18\x02 \x03(\x01\x12\x0e\n\x06\x63ursor\x18\x03 \x01(\t\"\xea\x01\n\x0eSearchResponse\x12.\n\x06result\x18\x01 \x03(\x0b\x32\x1e.google.appengine.SearchResult\x12\x15\n\rmatched_count\x18\x02 \x01(\x03\x12/\n\x06status\x18\x03 \x01(\x0b\x32\x1f.google.appengine.RequestStatus\x12\x0e\n\x06\x63ursor\x18\x04 \x01(\t\x12\x33\n\x0c\x66\x61\x63\x65t_result\x18\x05 \x03(\x0b\x32\x1d.google.appengine.FacetResult\x12\x13\n\x0b\x64ocs_scored\x18\x06 \x01(\x05*\x06\x08\xe8\x07\x10\x90NB8\n%com.google.appengine.api.search.protoB\x0fSearchServicePb')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.appengine.api.search.search_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n%com.google.appengine.api.search.protoB\017SearchServicePb'
   _INDEXDOCUMENTPARAMS.fields_by_name['freshness']._options = None
   _INDEXDOCUMENTPARAMS.fields_by_name['freshness']._serialized_options = b'\030\001'
   _globals['_SEARCHSERVICEERROR']._serialized_start=114
   _globals['_SEARCHSERVICEERROR']._serialized_end=282
   _globals['_SEARCHSERVICEERROR_ERRORCODE']._serialized_start=137
@@ -90,57 +89,56 @@
   _globals['_CANCELDELETEINDEXPARAMS']._serialized_start=2540
   _globals['_CANCELDELETEINDEXPARAMS']._serialized_end=2614
   _globals['_CANCELDELETEINDEXREQUEST']._serialized_start=2616
   _globals['_CANCELDELETEINDEXREQUEST']._serialized_end=2717
   _globals['_CANCELDELETEINDEXRESPONSE']._serialized_start=2719
   _globals['_CANCELDELETEINDEXRESPONSE']._serialized_end=2795
   _globals['_LISTINDEXESPARAMS']._serialized_start=2798
-  _globals['_LISTINDEXESPARAMS']._serialized_end=3041
-  _globals['_LISTINDEXESREQUEST']._serialized_start=3043
-  _globals['_LISTINDEXESREQUEST']._serialized_end=3132
-  _globals['_LISTINDEXESRESPONSE']._serialized_start=3134
-  _globals['_LISTINDEXESRESPONSE']._serialized_end=3261
-  _globals['_DELETESCHEMAPARAMS']._serialized_start=3264
-  _globals['_DELETESCHEMAPARAMS']._serialized_end=3422
-  _globals['_DELETESCHEMAREQUEST']._serialized_start=3424
-  _globals['_DELETESCHEMAREQUEST']._serialized_end=3515
-  _globals['_DELETESCHEMARESPONSE']._serialized_start=3517
-  _globals['_DELETESCHEMARESPONSE']._serialized_end=3588
-  _globals['_SORTSPEC']._serialized_start=3590
-  _globals['_SORTSPEC']._serialized_end=3715
-  _globals['_SCORERSPEC']._serialized_start=3718
-  _globals['_SCORERSPEC']._serialized_end=3907
-  _globals['_SCORERSPEC_SCORER']._serialized_start=3853
-  _globals['_SCORERSPEC_SCORER']._serialized_end=3907
-  _globals['_FIELDSPEC']._serialized_start=3910
-  _globals['_FIELDSPEC']._serialized_end=4043
-  _globals['_FIELDSPEC_EXPRESSION']._serialized_start=3997
-  _globals['_FIELDSPEC_EXPRESSION']._serialized_end=4043
-  _globals['_FACETRANGE']._serialized_start=4045
-  _globals['_FACETRANGE']._serialized_end=4099
-  _globals['_FACETREQUESTPARAM']._serialized_start=4101
-  _globals['_FACETREQUESTPARAM']._serialized_end=4212
-  _globals['_FACETAUTODETECTPARAM']._serialized_start=4214
-  _globals['_FACETAUTODETECTPARAM']._serialized_end=4261
-  _globals['_FACETREQUEST']._serialized_start=4263
-  _globals['_FACETREQUEST']._serialized_end=4344
-  _globals['_FACETREFINEMENT']._serialized_start=4347
-  _globals['_FACETREFINEMENT']._serialized_end=4486
-  _globals['_FACETREFINEMENT_RANGE']._serialized_start=4451
-  _globals['_FACETREFINEMENT_RANGE']._serialized_end=4486
-  _globals['_SEARCHPARAMS']._serialized_start=4489
-  _globals['_SEARCHPARAMS']._serialized_end=5343
-  _globals['_SEARCHPARAMS_CURSORTYPE']._serialized_start=5253
-  _globals['_SEARCHPARAMS_CURSORTYPE']._serialized_end=5303
-  _globals['_SEARCHPARAMS_PARSINGMODE']._serialized_start=5305
-  _globals['_SEARCHPARAMS_PARSINGMODE']._serialized_end=5343
-  _globals['_SEARCHREQUEST']._serialized_start=5345
-  _globals['_SEARCHREQUEST']._serialized_end=5424
-  _globals['_FACETRESULTVALUE']._serialized_start=5426
-  _globals['_FACETRESULTVALUE']._serialized_end=5528
-  _globals['_FACETRESULT']._serialized_start=5530
-  _globals['_FACETRESULT']._serialized_end=5608
-  _globals['_SEARCHRESULT']._serialized_start=5611
-  _globals['_SEARCHRESULT']._serialized_end=5753
-  _globals['_SEARCHRESPONSE']._serialized_start=5756
-  _globals['_SEARCHRESPONSE']._serialized_end=5990
-
+  _globals['_LISTINDEXESPARAMS']._serialized_end=3065
+  _globals['_LISTINDEXESREQUEST']._serialized_start=3067
+  _globals['_LISTINDEXESREQUEST']._serialized_end=3156
+  _globals['_LISTINDEXESRESPONSE']._serialized_start=3158
+  _globals['_LISTINDEXESRESPONSE']._serialized_end=3285
+  _globals['_DELETESCHEMAPARAMS']._serialized_start=3288
+  _globals['_DELETESCHEMAPARAMS']._serialized_end=3446
+  _globals['_DELETESCHEMAREQUEST']._serialized_start=3448
+  _globals['_DELETESCHEMAREQUEST']._serialized_end=3539
+  _globals['_DELETESCHEMARESPONSE']._serialized_start=3541
+  _globals['_DELETESCHEMARESPONSE']._serialized_end=3612
+  _globals['_SORTSPEC']._serialized_start=3614
+  _globals['_SORTSPEC']._serialized_end=3739
+  _globals['_SCORERSPEC']._serialized_start=3742
+  _globals['_SCORERSPEC']._serialized_end=3931
+  _globals['_SCORERSPEC_SCORER']._serialized_start=3877
+  _globals['_SCORERSPEC_SCORER']._serialized_end=3931
+  _globals['_FIELDSPEC']._serialized_start=3934
+  _globals['_FIELDSPEC']._serialized_end=4067
+  _globals['_FIELDSPEC_EXPRESSION']._serialized_start=4021
+  _globals['_FIELDSPEC_EXPRESSION']._serialized_end=4067
+  _globals['_FACETRANGE']._serialized_start=4069
+  _globals['_FACETRANGE']._serialized_end=4123
+  _globals['_FACETREQUESTPARAM']._serialized_start=4125
+  _globals['_FACETREQUESTPARAM']._serialized_end=4236
+  _globals['_FACETAUTODETECTPARAM']._serialized_start=4238
+  _globals['_FACETAUTODETECTPARAM']._serialized_end=4285
+  _globals['_FACETREQUEST']._serialized_start=4287
+  _globals['_FACETREQUEST']._serialized_end=4368
+  _globals['_FACETREFINEMENT']._serialized_start=4371
+  _globals['_FACETREFINEMENT']._serialized_end=4510
+  _globals['_FACETREFINEMENT_RANGE']._serialized_start=4475
+  _globals['_FACETREFINEMENT_RANGE']._serialized_end=4510
+  _globals['_SEARCHPARAMS']._serialized_start=4513
+  _globals['_SEARCHPARAMS']._serialized_end=5367
+  _globals['_SEARCHPARAMS_CURSORTYPE']._serialized_start=5277
+  _globals['_SEARCHPARAMS_CURSORTYPE']._serialized_end=5327
+  _globals['_SEARCHPARAMS_PARSINGMODE']._serialized_start=5329
+  _globals['_SEARCHPARAMS_PARSINGMODE']._serialized_end=5367
+  _globals['_SEARCHREQUEST']._serialized_start=5369
+  _globals['_SEARCHREQUEST']._serialized_end=5448
+  _globals['_FACETRESULTVALUE']._serialized_start=5450
+  _globals['_FACETRESULTVALUE']._serialized_end=5552
+  _globals['_FACETRESULT']._serialized_start=5554
+  _globals['_FACETRESULT']._serialized_end=5632
+  _globals['_SEARCHRESULT']._serialized_start=5635
+  _globals['_SEARCHRESULT']._serialized_end=5777
+  _globals['_SEARCHRESPONSE']._serialized_start=5780
+  _globals['_SEARCHRESPONSE']._serialized_end=6014
```

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/search/search_util.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/search/search_util.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/search/simple_search_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/search/simple_search_stub.py`

 * *Files 2% similar despite different names*

```diff
@@ -792,30 +792,42 @@
           [search_service_pb2.SearchServiceError.OK] * 10 +
           [search_service_pb2.SearchServiceError.TRANSIENT_ERROR] +
           [search_service_pb2.SearchServiceError.INTERNAL_ERROR])
       return
 
     response.status.code = search_service_pb2.SearchServiceError.OK
 
-    namespace = self._GetNamespace(request.params.namespace)
-    if namespace not in self.__indexes or not self.__indexes[namespace]:
-      return
+    params = request.params
+    namespace = self._GetNamespace(params.namespace)
+
+    indexes_by_namespace_and_name = {}
+    if params.all_namespaces:
+      for namespace, indexes_by_name in six.iteritems(self.__indexes):
+        for index_name, index in six.iteritems(indexes_by_name):
+          indexes_by_namespace_and_name[(namespace, index_name)] = index
+    else:
+      if namespace not in self.__indexes or not self.__indexes[namespace]:
+        return
+      for index_name, index in six.iteritems(self.__indexes[namespace]):
+        indexes_by_namespace_and_name[(namespace, index_name)] = index
 
     keys, indexes = list(
         six.moves.zip(*sorted(
-            six.iteritems(self.__indexes[namespace]), key=lambda v: v[0])))
+            six.iteritems(indexes_by_namespace_and_name),
+            key=lambda v: v[0])))
     position = 0
-    params = request.params
     if params.HasField('start_index_name'):
-      position = bisect.bisect_left(keys, params.start_index_name)
+      position = bisect.bisect_left(keys,
+                                    (params.namespace, params.start_index_name))
       if (not params.include_start_index and position < len(keys) and
-          keys[position] == params.start_index_name):
+          keys[position] == (params.namespace, params.start_index_name)):
         position += 1
     elif params.HasField('index_name_prefix'):
-      position = bisect.bisect_left(keys, params.index_name_prefix)
+      position = bisect.bisect_left(
+          keys, (params.namespace, params.index_name_prefix))
     if params.HasField('offset'):
       position += params.offset
     end_position = position + params.limit
     prefix = params.index_name_prefix
     for index in indexes[min(position, len(keys)):min(end_position, len(keys))]:
       index_spec = index.index_spec
       if prefix and not index_spec.name.startswith(prefix):
```

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/search/stub/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/document_matcher.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/search/stub/document_matcher.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/expression_evaluator.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/search/stub/expression_evaluator.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/simple_facet.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/search/stub/simple_facet.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/simple_tokenizer.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/search/stub/simple_tokenizer.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/search/stub/tokens.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/search/stub/tokens.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/search/unicode_util.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/search/unicode_util.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/stublib.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/stublib.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/system/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/system/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/system/system_service_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/system/system_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/system/system_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/system/system_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/taskqueue/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/taskqueue/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/taskqueue/taskqueue.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/taskqueue/taskqueue.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/taskqueue/taskqueue_service_bytes_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/taskqueue/taskqueue_service_bytes_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/taskqueue/taskqueue_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/taskqueue/taskqueue_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/titanoboa_request_info.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/titanoboa_request_info.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/urlfetch.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/urlfetch.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/urlfetch_errors.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/urlfetch_errors.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/urlfetch_service_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/urlfetch_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/urlfetch_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/urlfetch_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/user_service_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/user_service_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/user_service_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/users.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/users.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/validation.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/validation.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/yaml_builder.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/yaml_builder.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/yaml_errors.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/yaml_errors.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/yaml_listener.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/yaml_listener.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/yaml_object.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/yaml_object.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/api/yaml_test_util.py` & `appengine-python-standard-1.1.3/src/google/appengine/api/yaml_test_util.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/base/capabilities_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/base/capabilities_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/action_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/action_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/cloud_datastore_v1_remote_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/cloud_datastore_v1_remote_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/cloud_datastore_v1_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/cloud_datastore_v1_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/cloud_datastore_validator.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/cloud_datastore_validator.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_index.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_index.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_index_xml.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_index_xml.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_pb.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_pb.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_pbs.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_pbs.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_query.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_query.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_rpc.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_rpc.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_stub_index.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_stub_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,15 +305,17 @@
     if index_yaml_mtime is None:
       index_yaml_data = None
     else:
       try:
 
 
 
-        fh = openfile(index_yaml_file, 'rU')
+        # The 'U' option is deprecated in py3, as universal newlines
+        # are the default option
+        fh = openfile(index_yaml_file, 'r' if six.PY3 else 'rU')
       except IOError:
         index_yaml_data = None
       else:
         try:
           index_yaml_data = fh.read()
           if not index_yaml_data:
             raise EmptyIndexFileError(
```

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_stub_util.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_stub_util.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_v3_bytes_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_v3_bytes_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_v4_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_v4_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_v4_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_v4_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/datastore_v4_validator.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/datastore_v4_validator.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/document_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/document_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/entity_bytes_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/entity_bytes_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/entity_v4_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/entity_v4_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/snapshot_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/datastore/sortable_pb_encoder.py` & `appengine-python-standard-1.1.3/src/google/appengine/datastore/sortable_pb_encoder.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/blobstore/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/blobstore/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/blobstore/blobstore.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/blobstore/blobstore.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/db/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/db/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/db/metadata.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/db/metadata.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/db/polymodel.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/db/polymodel.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/db/stats.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/db/stats.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/db/sync.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/db/sync.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/deferred/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/deferred/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/deferred/deferred.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/deferred/deferred.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/gql/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/gql/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/key_range/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/key_range/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/blobstore.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/blobstore.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/context.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/context.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/django_middleware.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/django_middleware.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/eventloop.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/eventloop.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/key.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/key.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/key_test.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/key_test.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/metadata.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/metadata.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/model.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/model.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/polymodel.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/polymodel.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/query.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/query.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/stats.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/stats.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/tasklets.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/tasklets.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/test_utils.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/test_utils.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/ndb/utils.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/ndb/utils.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/remote_api/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/remote_api/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/remote_api/remote_api_bytes_pb2.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/remote_api/remote_api_bytes_pb2.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/ext/testbed/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/ext/testbed/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,15 @@
 from google.appengine.api.blobstore import dict_blob_storage
 from google.appengine.api.capabilities import capability_stub
 from google.appengine.api.images import images_stub
 from google.appengine.api.memcache import memcache_stub
 from google.appengine.api.modules import modules_stub
 from google.appengine.api.namespace_manager import namespace_manager
 from google.appengine.api.oauth import oauth_api
+from google.appengine.api.search import simple_search_stub
 from google.appengine.api.taskqueue import taskqueue_stub
 from google.appengine.datastore import cloud_datastore_v1_stub
 from google.appengine.datastore import datastore_pbs
 from google.appengine.datastore import datastore_stub_util
 from google.appengine.datastore import datastore_v4_stub
 from google.appengine.runtime import context
 import six
@@ -208,14 +209,15 @@
 CAPABILITY_SERVICE_NAME = 'capability_service'
 CHANNEL_SERVICE_NAME = 'channel'
 DATASTORE_SERVICE_NAME = 'datastore_v3'
 FILES_SERVICE_NAME = 'file'
 IMAGES_SERVICE_NAME = 'images'
 MAIL_SERVICE_NAME = 'mail'
 MEMCACHE_SERVICE_NAME = 'memcache'
+SEARCH_SERVICE_NAME = 'search'
 TASKQUEUE_SERVICE_NAME = 'taskqueue'
 URLFETCH_SERVICE_NAME = 'urlfetch'
 USER_SERVICE_NAME = 'user'
 XMPP_SERVICE_NAME = 'xmpp'
 MODULES_SERVICE_NAME = 'modules'
 
 
@@ -929,14 +931,29 @@
           real service should be disabled.
 
     Raises:
       StubNotSupportedError: If called.
     """
     raise StubNotSupportedError('The xmpp stub is not supported in Titanoboa.')
 
+  def init_search_stub(self, enable=True, **stub_kw_args):
+    """Enables the search stub.
+
+    Args:
+      enable: `True` if the fake service should be enabled, or `False` if the
+          real service should be disabled.
+      **stub_kw_args: Keyword arguments that are passed on to the service
+          stub.
+    """
+    if not enable:
+      self._disable_stub(SEARCH_SERVICE_NAME)
+      return
+    stub = simple_search_stub.SearchServiceStub(**stub_kw_args)
+    self._register_stub(SEARCH_SERVICE_NAME, stub)
+
   def init_modules_stub(self, enable=True):
     """Enables the modules stub.
 
     Args:
       enable: `True` if the fake service should be enabled, or `False` if the
           real service should be disabled.
     """
```

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/runtime/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/runtime/apiproxy.py` & `appengine-python-standard-1.1.3/src/google/appengine/runtime/apiproxy.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/runtime/apiproxy_errors.py` & `appengine-python-standard-1.1.3/src/google/appengine/runtime/apiproxy_errors.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/runtime/background.py` & `appengine-python-standard-1.1.3/src/google/appengine/runtime/background.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/runtime/callback.py` & `appengine-python-standard-1.1.3/src/google/appengine/runtime/callback.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/runtime/context/__init__.py` & `appengine-python-standard-1.1.3/src/google/appengine/runtime/context/__init__.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/runtime/context/ctx_test_util.py` & `appengine-python-standard-1.1.3/src/google/appengine/runtime/context/ctx_test_util.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/runtime/context/gae_headers.py` & `appengine-python-standard-1.1.3/src/google/appengine/runtime/context/gae_headers.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/runtime/context/wsgi.py` & `appengine-python-standard-1.1.3/src/google/appengine/runtime/context/wsgi.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/runtime/default_api_stub.py` & `appengine-python-standard-1.1.3/src/google/appengine/runtime/default_api_stub.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/runtime/initialize.py` & `appengine-python-standard-1.1.3/src/google/appengine/runtime/initialize.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/runtime/middlewares.py` & `appengine-python-standard-1.1.3/src/google/appengine/runtime/middlewares.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/runtime/request_environment.py` & `appengine-python-standard-1.1.3/src/google/appengine/runtime/request_environment.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/runtime/thread_hooks.py` & `appengine-python-standard-1.1.3/src/google/appengine/runtime/thread_hooks.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/tools/app_engine_config_exception.py` & `appengine-python-standard-1.1.3/src/google/appengine/tools/app_engine_config_exception.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/tools/os_compat.py` & `appengine-python-standard-1.1.3/src/google/appengine/tools/os_compat.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/tools/queue_xml_parser.py` & `appengine-python-standard-1.1.3/src/google/appengine/tools/queue_xml_parser.py`

 * *Files identical despite different names*

### Comparing `appengine-python-standard-1.1.2/src/google/appengine/tools/xml_parser_utils.py` & `appengine-python-standard-1.1.3/src/google/appengine/tools/xml_parser_utils.py`

 * *Files identical despite different names*

