# Comparing `tmp/claudia-0.1.1.tar.gz` & `tmp/claudia-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claudia-0.1.1.tar", last modified: Thu Jul 20 03:44:26 2023, max compression
+gzip compressed data, was "claudia-0.1.2.tar", last modified: Fri Jul 21 01:53:22 2023, max compression
```

## Comparing `claudia-0.1.1.tar` & `claudia-0.1.2.tar`

### file list

```diff
@@ -1,92 +1,90 @@
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.744444 claudia-0.1.1/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1074 2023-05-25 22:01:40.000000 claudia-0.1.1/LICENSE
--rw-r--r--   0 ksaxena    (502) staff       (20)    11120 2023-07-20 03:44:26.744176 claudia-0.1.1/PKG-INFO
--rw-r--r--   0 ksaxena    (502) staff       (20)      402 2023-06-22 00:52:56.000000 claudia-0.1.1/README.md
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.723141 claudia-0.1.1/claudia.egg-info/
--rw-r--r--   0 ksaxena    (502) staff       (20)    11120 2023-07-20 03:44:26.000000 claudia-0.1.1/claudia.egg-info/PKG-INFO
--rw-r--r--   0 ksaxena    (502) staff       (20)     2825 2023-07-20 03:44:26.000000 claudia-0.1.1/claudia.egg-info/SOURCES.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)        1 2023-07-20 03:44:26.000000 claudia-0.1.1/claudia.egg-info/dependency_links.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-07-20 03:44:26.000000 claudia-0.1.1/claudia.egg-info/entry_points.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)      109 2023-07-20 03:44:26.000000 claudia-0.1.1/claudia.egg-info/requires.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)        8 2023-07-20 03:44:26.000000 claudia-0.1.1/claudia.egg-info/top_level.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       38 2023-07-20 03:44:26.744507 claudia-0.1.1/setup.cfg
--rw-r--r--   0 ksaxena    (502) staff       (20)     1478 2023-07-20 03:43:11.000000 claudia-0.1.1/setup.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.717372 claudia-0.1.1/src/
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.724646 claudia-0.1.1/src/claudia/
--rw-r--r--   0 ksaxena    (502) staff       (20)    10771 2023-06-22 00:52:56.000000 claudia-0.1.1/src/claudia/README.md
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-30 20:36:34.000000 claudia-0.1.1/src/claudia/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    40220 2023-07-20 03:37:15.000000 claudia-0.1.1/src/claudia/claudia.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.725682 claudia-0.1.1/src/claudia/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)    14321 2023-05-30 20:36:34.000000 claudia-0.1.1/src/claudia/features/nft_burn_mint.feature
--rw-r--r--   0 ksaxena    (502) staff       (20)     5371 2023-07-12 21:19:51.000000 claudia-0.1.1/src/claudia/features/payments.feature
--rw-r--r--   0 ksaxena    (502) staff       (20)    11071 2023-05-30 20:36:34.000000 claudia-0.1.1/src/claudia/features/trustline.feature
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.728789 claudia-0.1.1/src/claudia/javascript/
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      118 2023-05-30 20:36:34.000000 claudia-0.1.1/src/claudia/javascript/cleanup
--rw-r--r--   0 ksaxena    (502) staff       (20)      145 2023-05-30 20:36:34.000000 claudia-0.1.1/src/claudia/javascript/cucumber.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.729156 claudia-0.1.1/src/claudia/javascript/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1227 2023-05-30 20:36:34.000000 claudia-0.1.1/src/claudia/javascript/features/context.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.729432 claudia-0.1.1/src/claudia/javascript/features/lib/
--rw-r--r--   0 ksaxena    (502) staff       (20)     2107 2023-05-30 20:36:34.000000 claudia-0.1.1/src/claudia/javascript/features/lib/ObjFactory.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.731582 claudia-0.1.1/src/claudia/javascript/features/steps/
--rw-r--r--   0 ksaxena    (502) staff       (20)    38910 2023-06-22 00:52:56.000000 claudia-0.1.1/src/claudia/javascript/features/steps/common.js
--rw-r--r--   0 ksaxena    (502) staff       (20)      303 2023-06-05 20:21:20.000000 claudia-0.1.1/src/claudia/javascript/features/steps/constants.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    71153 2023-05-30 20:36:34.000000 claudia-0.1.1/src/claudia/javascript/features/steps/nft_mint_burn.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    19024 2023-05-30 20:36:34.000000 claudia-0.1.1/src/claudia/javascript/features/steps/payments.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    59478 2023-05-30 20:36:34.000000 claudia-0.1.1/src/claudia/javascript/features/steps/trustline.js
--rw-r--r--   0 ksaxena    (502) staff       (20)   129466 2023-06-14 21:08:34.000000 claudia-0.1.1/src/claudia/javascript/package-lock.json
--rw-r--r--   0 ksaxena    (502) staff       (20)      221 2023-05-30 20:36:34.000000 claudia-0.1.1/src/claudia/javascript/package.json
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      870 2023-05-30 20:36:34.000000 claudia-0.1.1/src/claudia/javascript/runSetup
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     5028 2023-06-22 00:52:56.000000 claudia-0.1.1/src/claudia/javascript/runTest
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.732606 claudia-0.1.1/src/claudia/network_setup/
--rw-r--r--   0 ksaxena    (502) staff       (20)      251 2023-06-22 00:52:56.000000 claudia-0.1.1/src/claudia/network_setup/Dockerfile.rippled_build
--rw-r--r--   0 ksaxena    (502) staff       (20)      714 2023-06-22 00:52:56.000000 claudia-0.1.1/src/claudia/network_setup/Dockerfile.rippled_install
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.719593 claudia-0.1.1/src/claudia/network_setup/configs/
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.719465 claudia-0.1.1/src/claudia/network_setup/configs/rippled/
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.733331 claudia-0.1.1/src/claudia/network_setup/configs/rippled/rippled_1/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1796 2023-06-22 00:52:56.000000 claudia-0.1.1/src/claudia/network_setup/configs/rippled/rippled_1/rippled.cfg
--rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-22 00:52:56.000000 claudia-0.1.1/src/claudia/network_setup/configs/rippled/rippled_1/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.734067 claudia-0.1.1/src/claudia/network_setup/configs/rippled/rippled_2/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1838 2023-06-22 00:52:56.000000 claudia-0.1.1/src/claudia/network_setup/configs/rippled/rippled_2/rippled.cfg
--rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-22 00:52:56.000000 claudia-0.1.1/src/claudia/network_setup/configs/rippled/rippled_2/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.734576 claudia-0.1.1/src/claudia/network_setup/configs/rippled/rippled_3/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1838 2023-06-22 00:52:56.000000 claudia-0.1.1/src/claudia/network_setup/configs/rippled/rippled_3/rippled.cfg
--rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-22 00:52:56.000000 claudia-0.1.1/src/claudia/network_setup/configs/rippled/rippled_3/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.735020 claudia-0.1.1/src/claudia/network_setup/configs/rippled/rippled_4/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1837 2023-06-22 00:52:56.000000 claudia-0.1.1/src/claudia/network_setup/configs/rippled/rippled_4/rippled.cfg
--rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-22 00:52:56.000000 claudia-0.1.1/src/claudia/network_setup/configs/rippled/rippled_4/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.735241 claudia-0.1.1/src/claudia/network_setup/configs/sidechain/
--rw-r--r--   0 ksaxena    (502) staff       (20)     2150 2023-06-22 00:52:56.000000 claudia-0.1.1/src/claudia/network_setup/configs/sidechain/bridge_bootstrap.json
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.737499 claudia-0.1.1/src/claudia/network_setup/lib/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1775 2023-06-22 00:52:56.000000 claudia-0.1.1/src/claudia/network_setup/lib/build.sh
--rw-r--r--   0 ksaxena    (502) staff       (20)     1268 2023-06-22 00:52:56.000000 claudia-0.1.1/src/claudia/network_setup/lib/rippled_network.yml
--rw-r--r--   0 ksaxena    (502) staff       (20)    27352 2023-07-20 03:37:15.000000 claudia-0.1.1/src/claudia/network_setup/lib/setup_helper.sh
--rw-r--r--   0 ksaxena    (502) staff       (20)     1268 2023-06-22 00:52:56.000000 claudia-0.1.1/src/claudia/network_setup/lib/sidechain_network.yml
--rw-r--r--   0 ksaxena    (502) staff       (20)     5442 2023-06-22 00:52:56.000000 claudia-0.1.1/src/claudia/network_setup/lib/validate_network.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     4013 2023-07-19 20:08:15.000000 claudia-0.1.1/src/claudia/network_setup/lib/witness_action.sh
--rw-r--r--   0 ksaxena    (502) staff       (20)    16916 2023-07-19 20:08:15.000000 claudia-0.1.1/src/claudia/network_setup/lib/xchain_bridge_create.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     7323 2023-07-20 03:37:15.000000 claudia-0.1.1/src/claudia/network_setup/setup.sh
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.739347 claudia-0.1.1/src/claudia/python/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-30 20:36:34.000000 claudia-0.1.1/src/claudia/python/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)      107 2023-05-30 20:36:34.000000 claudia-0.1.1/src/claudia/python/behave.ini
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      123 2023-05-30 20:36:34.000000 claudia-0.1.1/src/claudia/python/cleanup
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.739891 claudia-0.1.1/src/claudia/python/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-30 20:36:34.000000 claudia-0.1.1/src/claudia/python/features/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     3217 2023-07-19 20:08:15.000000 claudia-0.1.1/src/claudia/python/features/environment.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.741137 claudia-0.1.1/src/claudia/python/features/steps/
--rw-r--r--   0 ksaxena    (502) staff       (20)    65912 2023-07-19 20:08:15.000000 claudia-0.1.1/src/claudia/python/features/steps/nft_mint_burn.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    21832 2023-07-19 20:08:15.000000 claudia-0.1.1/src/claudia/python/features/steps/payments.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    54630 2023-07-19 20:08:15.000000 claudia-0.1.1/src/claudia/python/features/steps/trustline.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.741610 claudia-0.1.1/src/claudia/python/lib/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-07-19 20:08:15.000000 claudia-0.1.1/src/claudia/python/lib/__init__.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.742076 claudia-0.1.1/src/claudia/python/lib/exceptions/
--rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-07-19 20:08:15.000000 claudia-0.1.1/src/claudia/python/lib/exceptions/InvalidInputException.py
--rw-r--r--   0 ksaxena    (502) staff       (20)       60 2023-07-19 20:08:15.000000 claudia-0.1.1/src/claudia/python/lib/exceptions/UnconfiguredEnvironmentException.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-20 03:44:26.743764 claudia-0.1.1/src/claudia/python/lib/framework/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-07-19 20:08:15.000000 claudia-0.1.1/src/claudia/python/lib/framework/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    26245 2023-07-19 20:08:15.000000 claudia-0.1.1/src/claudia/python/lib/framework/common.py
--rw-r--r--   0 ksaxena    (502) staff       (20)      252 2023-07-19 20:08:15.000000 claudia-0.1.1/src/claudia/python/lib/framework/constants.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     9149 2023-07-19 20:08:15.000000 claudia-0.1.1/src/claudia/python/lib/framework/object_factory.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    22326 2023-07-19 20:08:15.000000 claudia-0.1.1/src/claudia/python/lib/framework/workflow_helper.py
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     1382 2023-05-30 20:36:34.000000 claudia-0.1.1/src/claudia/python/runSetup
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     6158 2023-07-12 21:19:51.000000 claudia-0.1.1/src/claudia/python/runTest
--rw-r--r--   0 ksaxena    (502) staff       (20)      109 2023-06-22 00:52:56.000000 claudia-0.1.1/src/claudia/requirements.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.919436 claudia-0.1.2/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1074 2023-05-25 22:01:40.000000 claudia-0.1.2/LICENSE
+-rw-r--r--   0 ksaxena    (502) staff       (20)    11120 2023-07-21 01:53:22.918224 claudia-0.1.2/PKG-INFO
+-rw-r--r--   0 ksaxena    (502) staff       (20)      402 2023-06-22 00:52:56.000000 claudia-0.1.2/README.md
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.879432 claudia-0.1.2/claudia.egg-info/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    11120 2023-07-21 01:53:22.000000 claudia-0.1.2/claudia.egg-info/PKG-INFO
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2759 2023-07-21 01:53:22.000000 claudia-0.1.2/claudia.egg-info/SOURCES.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)        1 2023-07-21 01:53:22.000000 claudia-0.1.2/claudia.egg-info/dependency_links.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-07-21 01:53:22.000000 claudia-0.1.2/claudia.egg-info/entry_points.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)      109 2023-07-21 01:53:22.000000 claudia-0.1.2/claudia.egg-info/requires.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)        8 2023-07-21 01:53:22.000000 claudia-0.1.2/claudia.egg-info/top_level.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       38 2023-07-21 01:53:22.919555 claudia-0.1.2/setup.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1478 2023-07-20 20:52:54.000000 claudia-0.1.2/setup.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.870006 claudia-0.1.2/src/
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.881323 claudia-0.1.2/src/claudia/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    10771 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/README.md
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    40220 2023-07-20 20:52:46.000000 claudia-0.1.2/src/claudia/claudia.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.883072 claudia-0.1.2/src/claudia/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    14321 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/features/nft_burn_mint.feature
+-rw-r--r--   0 ksaxena    (502) staff       (20)     5371 2023-07-12 21:19:51.000000 claudia-0.1.2/src/claudia/features/payments.feature
+-rw-r--r--   0 ksaxena    (502) staff       (20)    11071 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/features/trustline.feature
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.887083 claudia-0.1.2/src/claudia/javascript/
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      118 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/javascript/cleanup
+-rw-r--r--   0 ksaxena    (502) staff       (20)      145 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/javascript/cucumber.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.887728 claudia-0.1.2/src/claudia/javascript/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1227 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/javascript/features/context.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.888195 claudia-0.1.2/src/claudia/javascript/features/lib/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2107 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/javascript/features/lib/ObjFactory.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.891077 claudia-0.1.2/src/claudia/javascript/features/steps/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    38941 2023-07-21 01:52:20.000000 claudia-0.1.2/src/claudia/javascript/features/steps/common.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)      303 2023-06-05 20:21:20.000000 claudia-0.1.2/src/claudia/javascript/features/steps/constants.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    71153 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/javascript/features/steps/nft_mint_burn.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    19024 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/javascript/features/steps/payments.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    59478 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/javascript/features/steps/trustline.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)   130175 2023-07-21 01:52:20.000000 claudia-0.1.2/src/claudia/javascript/package-lock.json
+-rw-r--r--   0 ksaxena    (502) staff       (20)      221 2023-07-21 01:52:20.000000 claudia-0.1.2/src/claudia/javascript/package.json
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      870 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/javascript/runSetup
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     5028 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/javascript/runTest
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.892833 claudia-0.1.2/src/claudia/network_setup/
+-rw-r--r--   0 ksaxena    (502) staff       (20)      251 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/network_setup/Dockerfile.rippled_build
+-rw-r--r--   0 ksaxena    (502) staff       (20)      714 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/network_setup/Dockerfile.rippled_install
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.872612 claudia-0.1.2/src/claudia/network_setup/configs/
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.873464 claudia-0.1.2/src/claudia/network_setup/configs/rippled/
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.893956 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_1/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1809 2023-07-20 20:52:54.000000 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_1/rippled.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_1/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.894953 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_2/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1851 2023-07-20 20:52:54.000000 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_2/rippled.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_2/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.895897 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_3/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1851 2023-07-20 20:52:54.000000 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_3/rippled.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_3/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.896779 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_4/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1850 2023-07-20 20:52:54.000000 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_4/rippled.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_4/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.900560 claudia-0.1.2/src/claudia/network_setup/lib/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1775 2023-07-21 01:52:09.000000 claudia-0.1.2/src/claudia/network_setup/lib/build.sh
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1268 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/network_setup/lib/rippled_network.yml
+-rw-r--r--   0 ksaxena    (502) staff       (20)    27463 2023-07-21 01:52:09.000000 claudia-0.1.2/src/claudia/network_setup/lib/setup_helper.sh
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1268 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/network_setup/lib/sidechain_network.yml
+-rw-r--r--   0 ksaxena    (502) staff       (20)     5442 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/network_setup/lib/validate_network.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     4013 2023-07-19 20:08:15.000000 claudia-0.1.2/src/claudia/network_setup/lib/witness_action.sh
+-rw-r--r--   0 ksaxena    (502) staff       (20)    16916 2023-07-19 20:08:15.000000 claudia-0.1.2/src/claudia/network_setup/lib/xchain_bridge_create.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     7323 2023-07-20 20:52:46.000000 claudia-0.1.2/src/claudia/network_setup/setup.sh
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.903987 claudia-0.1.2/src/claudia/python/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/python/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)      107 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/python/behave.ini
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      123 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/python/cleanup
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.905575 claudia-0.1.2/src/claudia/python/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/python/features/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     3217 2023-07-19 20:08:15.000000 claudia-0.1.2/src/claudia/python/features/environment.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.911637 claudia-0.1.2/src/claudia/python/features/steps/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    65962 2023-07-20 20:52:54.000000 claudia-0.1.2/src/claudia/python/features/steps/nft_mint_burn.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    21692 2023-07-20 20:52:54.000000 claudia-0.1.2/src/claudia/python/features/steps/payments.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    54433 2023-07-20 20:52:54.000000 claudia-0.1.2/src/claudia/python/features/steps/trustline.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.912630 claudia-0.1.2/src/claudia/python/lib/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-07-19 20:08:15.000000 claudia-0.1.2/src/claudia/python/lib/__init__.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.914209 claudia-0.1.2/src/claudia/python/lib/exceptions/
+-rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-07-19 20:08:15.000000 claudia-0.1.2/src/claudia/python/lib/exceptions/InvalidInputException.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)       60 2023-07-19 20:08:15.000000 claudia-0.1.2/src/claudia/python/lib/exceptions/UnconfiguredEnvironmentException.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.917277 claudia-0.1.2/src/claudia/python/lib/framework/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-07-19 20:08:15.000000 claudia-0.1.2/src/claudia/python/lib/framework/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    26242 2023-07-20 20:52:54.000000 claudia-0.1.2/src/claudia/python/lib/framework/common.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)      252 2023-07-19 20:08:15.000000 claudia-0.1.2/src/claudia/python/lib/framework/constants.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     9148 2023-07-20 20:52:54.000000 claudia-0.1.2/src/claudia/python/lib/framework/object_factory.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    22326 2023-07-19 20:08:15.000000 claudia-0.1.2/src/claudia/python/lib/framework/workflow_helper.py
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     1382 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/python/runSetup
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     6158 2023-07-12 21:19:51.000000 claudia-0.1.2/src/claudia/python/runTest
+-rw-r--r--   0 ksaxena    (502) staff       (20)      109 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/requirements.txt
```

### Comparing `claudia-0.1.1/LICENSE` & `claudia-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/PKG-INFO` & `claudia-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claudia
-Version: 0.1.1
+Version: 0.1.2
 Summary: Run XRPL Automated Tests
 Home-page: https://xrpl.org/
 Download-URL: https://gitlab.ops.ripple.com/xrpledger/xrpl-nocode-automation
 Author: Kausty Saxena
 Author-email: ksaxena@ripple.com
 Keywords: ripple xrpl python javascript
 Description-Content-Type: text/markdown
```

### Comparing `claudia-0.1.1/claudia.egg-info/PKG-INFO` & `claudia-0.1.2/claudia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claudia
-Version: 0.1.1
+Version: 0.1.2
 Summary: Run XRPL Automated Tests
 Home-page: https://xrpl.org/
 Download-URL: https://gitlab.ops.ripple.com/xrpledger/xrpl-nocode-automation
 Author: Kausty Saxena
 Author-email: ksaxena@ripple.com
 Keywords: ripple xrpl python javascript
 Description-Content-Type: text/markdown
```

### Comparing `claudia-0.1.1/claudia.egg-info/SOURCES.txt` & `claudia-0.1.2/claudia.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 src/claudia/network_setup/configs/rippled/rippled_1/validators.txt
 src/claudia/network_setup/configs/rippled/rippled_2/rippled.cfg
 src/claudia/network_setup/configs/rippled/rippled_2/validators.txt
 src/claudia/network_setup/configs/rippled/rippled_3/rippled.cfg
 src/claudia/network_setup/configs/rippled/rippled_3/validators.txt
 src/claudia/network_setup/configs/rippled/rippled_4/rippled.cfg
 src/claudia/network_setup/configs/rippled/rippled_4/validators.txt
-src/claudia/network_setup/configs/sidechain/bridge_bootstrap.json
 src/claudia/network_setup/lib/build.sh
 src/claudia/network_setup/lib/rippled_network.yml
 src/claudia/network_setup/lib/setup_helper.sh
 src/claudia/network_setup/lib/sidechain_network.yml
 src/claudia/network_setup/lib/validate_network.py
 src/claudia/network_setup/lib/witness_action.sh
 src/claudia/network_setup/lib/xchain_bridge_create.py
```

### Comparing `claudia-0.1.1/setup.py` & `claudia-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         requirements = content.split('\n')
 
     return requirements
 
 
 setup(
     name='claudia',
-    version='0.1.1',
+    version='0.1.2',
     description='Run XRPL Automated Tests',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     author="Kausty Saxena",
     author_email="ksaxena@ripple.com",
     keywords="ripple xrpl python javascript",
     url='https://xrpl.org/',
```

### Comparing `claudia-0.1.1/src/claudia/README.md` & `claudia-0.1.2/src/claudia/README.md`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/claudia.py` & `claudia-0.1.2/src/claudia/claudia.py`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/features/nft_burn_mint.feature` & `claudia-0.1.2/src/claudia/features/nft_burn_mint.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/features/payments.feature` & `claudia-0.1.2/src/claudia/features/payments.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/features/trustline.feature` & `claudia-0.1.2/src/claudia/features/trustline.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/javascript/features/context.js` & `claudia-0.1.2/src/claudia/javascript/features/context.js`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/javascript/features/lib/ObjFactory.js` & `claudia-0.1.2/src/claudia/javascript/features/lib/ObjFactory.js`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/javascript/features/steps/common.js` & `claudia-0.1.2/src/claudia/javascript/features/steps/common.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -178,14 +178,15 @@
     if (context.connectionType == "websocket") {
         try {
             client = new xrpl.Client(context.url, {
                 feeCushion: 1
             });
             await client.connect()
         } catch (error) {
+            console.log(error)
             throw new Error("\nERROR: Cannot connect to " + context.url + ". Make sure the network is accessible.")
         }
     } else {
         throw "Unsupported CONNECTION_TYPE = '" + context.connectionType + "'";
     }
     return client;
 }
```

### Comparing `claudia-0.1.1/src/claudia/javascript/features/steps/nft_mint_burn.js` & `claudia-0.1.2/src/claudia/javascript/features/steps/nft_mint_burn.js`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/javascript/features/steps/payments.js` & `claudia-0.1.2/src/claudia/javascript/features/steps/payments.js`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/javascript/features/steps/trustline.js` & `claudia-0.1.2/src/claudia/javascript/features/steps/trustline.js`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/javascript/package-lock.json` & `claudia-0.1.2/src/claudia/javascript/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971730174538701%*

 * *Differences: {"'dependencies'": "{'buffer': {'version': '6.0.3', 'resolved': "*

 * *                   "'https://registry.npmjs.org/buffer/-/buffer-6.0.3.tgz', 'integrity': "*

 * *                   "'sha512-FTiCpNxtwiZZHEZbcbTIcZjERVICn9yq/pDFkTl95/AxzD1naBctN7YO68riM/gLSDY7sdrMby8hofADYuuqOA==', "*

 * *                   "'requires': {'base64-js': '^1.3.1', 'ieee754': '^1.2.1'}}, 'get-intrinsic': "*

 * *                   "{'version': '1.2.1', 'resolved': "*

 * *                   "'https://registry.npmjs.org/get-intrinsic/-/get-intrinsic-1.2 […]*

```diff
@@ -376,21 +376,21 @@
                 "create-hash": "^1.1.0",
                 "safe-buffer": "^5.1.2"
             },
             "resolved": "https://registry.npmjs.org/bs58check/-/bs58check-2.1.2.tgz",
             "version": "2.1.2"
         },
         "buffer": {
-            "integrity": "sha512-/gDYp/UtU0eA1ys8bOs9J6a+E/KWIY+DZ+Q2WESNUA0jFRsJOc0SNUO6xJ5SGA1xueg3NL65W6s+NY5l9cunuw==",
+            "integrity": "sha512-FTiCpNxtwiZZHEZbcbTIcZjERVICn9yq/pDFkTl95/AxzD1naBctN7YO68riM/gLSDY7sdrMby8hofADYuuqOA==",
             "requires": {
-                "base64-js": "^1.0.2",
-                "ieee754": "^1.1.4"
+                "base64-js": "^1.3.1",
+                "ieee754": "^1.2.1"
             },
-            "resolved": "https://registry.npmjs.org/buffer/-/buffer-5.6.0.tgz",
-            "version": "5.6.0"
+            "resolved": "https://registry.npmjs.org/buffer/-/buffer-6.0.3.tgz",
+            "version": "6.0.3"
         },
         "buffer-from": {
             "integrity": "sha512-E+XQCRwSbaaiChtv6k6Dwgc+bx+Bs6vuKJHHl5kox/BaKbhiXzqQOwK4cO22yElGp2OCmjwVhT3HmxgyPGnJfQ==",
             "resolved": "https://registry.npmjs.org/buffer-from/-/buffer-from-1.1.2.tgz",
             "version": "1.1.2"
         },
         "call-bind": {
@@ -611,22 +611,23 @@
         },
         "function-bind": {
             "integrity": "sha512-yIovAzMX49sF8Yl58fSCWJ5svSLuaibPxXQJFLmBObTuCr0Mf1KiPopGM9NiFjiYBCbfaa2Fh6breQ6ANVTI0A==",
             "resolved": "https://registry.npmjs.org/function-bind/-/function-bind-1.1.1.tgz",
             "version": "1.1.1"
         },
         "get-intrinsic": {
-            "integrity": "sha512-L049y6nFOuom5wGyRc3/gdTLO94dySVKRACj1RmJZBQXlbTMhtNIgkWkUHq+jYmZvKf14EW1EoJnnjbmoHij0Q==",
+            "integrity": "sha512-2DcsyfABl+gVHEfCOaTrWgyt+tb6MSEGmKq+kI5HwLbIYgjgmMcV8KQ41uaKz1xxUcn9tJtgFbQUEVcEbd0FYw==",
             "requires": {
                 "function-bind": "^1.1.1",
                 "has": "^1.0.3",
+                "has-proto": "^1.0.1",
                 "has-symbols": "^1.0.3"
             },
-            "resolved": "https://registry.npmjs.org/get-intrinsic/-/get-intrinsic-1.2.0.tgz",
-            "version": "1.2.0"
+            "resolved": "https://registry.npmjs.org/get-intrinsic/-/get-intrinsic-1.2.1.tgz",
+            "version": "1.2.1"
         },
         "glob": {
             "integrity": "sha512-nFR0zLpU2YCaRxwoCJvL6UvCH2JFyFVIvwTLsIf21AuHlMskA1hhTdk+LlYJtOlYt9v6dvszD2BGRqBL+iQK9Q==",
             "requires": {
                 "fs.realpath": "^1.0.0",
                 "inflight": "^1.0.4",
                 "inherits": "2",
@@ -678,14 +679,19 @@
             "integrity": "sha512-62DVLZGoiEBDHQyqG4w9xCuZ7eJEwNmJRWw2VY84Oedb7WFcA27fiEVe8oUQx9hAUJ4ekurquucTGwsyO1XGdQ==",
             "requires": {
                 "get-intrinsic": "^1.1.1"
             },
             "resolved": "https://registry.npmjs.org/has-property-descriptors/-/has-property-descriptors-1.0.0.tgz",
             "version": "1.0.0"
         },
+        "has-proto": {
+            "integrity": "sha512-7qE+iP+O+bgF9clE5+UoBFzE65mlBiVj3tKCrlNQ0Ogwm0BjpT/gK4SlLYDMybDh5I3TCTKnPPa0oMG7JDYrhg==",
+            "resolved": "https://registry.npmjs.org/has-proto/-/has-proto-1.0.1.tgz",
+            "version": "1.0.1"
+        },
         "has-symbols": {
             "integrity": "sha512-l3LCuF6MgDNwTDKkdYGEihYjt5pRPbEg46rtlmnSPlUbgmB8LOIrKJbYYFBSbnPaJexMKtiPO8hmeRjRz2Td+A==",
             "resolved": "https://registry.npmjs.org/has-symbols/-/has-symbols-1.0.3.tgz",
             "version": "1.0.3"
         },
         "has-tostringtag": {
             "integrity": "sha512-kFjcSNhnlGV1kyoGk7OXKSawH5JOb/LzUc5w9B02hOTO0dfFRjbHQKvg1d6cf3HbeUmtU9VbbV3qzZ2Teh97WQ==",
@@ -814,24 +820,20 @@
         },
         "is-stream": {
             "integrity": "sha512-hFoiJiTl63nn+kstHGBtewWSKnQLpyb155KHheA1l39uvtO9nWIop1p3udqPcUd/xbF1VLMO4n7OI6p7RbngDg==",
             "resolved": "https://registry.npmjs.org/is-stream/-/is-stream-2.0.1.tgz",
             "version": "2.0.1"
         },
         "is-typed-array": {
-            "integrity": "sha512-PJqgEHiWZvMpaFZ3uTc8kHPM4+4ADTlDniuQL7cU/UDA0Ql7F70yGfHph3cLNe+c9toaigv+DFzTJKhc2CtO6A==",
+            "integrity": "sha512-Z14TF2JNG8Lss5/HMqt0//T9JeHXttXy5pH/DBU4vi98ozO2btxzq9MwYDZYnKwU8nRsz/+GVFVRDq3DkVuSPg==",
             "requires": {
-                "available-typed-arrays": "^1.0.5",
-                "call-bind": "^1.0.2",
-                "for-each": "^0.3.3",
-                "gopd": "^1.0.1",
-                "has-tostringtag": "^1.0.0"
+                "which-typed-array": "^1.1.11"
             },
-            "resolved": "https://registry.npmjs.org/is-typed-array/-/is-typed-array-1.1.10.tgz",
-            "version": "1.1.10"
+            "resolved": "https://registry.npmjs.org/is-typed-array/-/is-typed-array-1.1.12.tgz",
+            "version": "1.1.12"
         },
         "knuth-shuffle-seeded": {
             "integrity": "sha512-9pFH0SplrfyKyojCLxZfMcvkhf5hH0d+UwR9nTVJ/DDQJGuzcXjTwB7TP7sDfehSudlGGaOLblmEWqv04ERVWg==",
             "requires": {
                 "seed-random": "~2.2.0"
             },
             "resolved": "https://registry.npmjs.org/knuth-shuffle-seeded/-/knuth-shuffle-seeded-1.0.6.tgz",
@@ -1080,46 +1082,46 @@
                 "hash-base": "^3.0.0",
                 "inherits": "^2.0.1"
             },
             "resolved": "https://registry.npmjs.org/ripemd160/-/ripemd160-2.0.2.tgz",
             "version": "2.0.2"
         },
         "ripple-address-codec": {
-            "integrity": "sha512-SZ96zZH+0REeyEcYVFl0vqcsGRXiFXS2RUgHupHhtVkOEk6men53vngVjJwBrSnY+oa6Cri15q1zSni3DEoxNw==",
+            "integrity": "sha512-Tvd81i7hpDmNqHvkj6iYlj8Tv3I1Romw5gfjni9eacewJvGV2xe+p2y0FAw39z72qfciRMhQyHvpnviBcWVBNw==",
             "requires": {
                 "base-x": "^3.0.9",
                 "create-hash": "^1.1.2"
             },
-            "resolved": "https://registry.npmjs.org/ripple-address-codec/-/ripple-address-codec-4.2.5.tgz",
-            "version": "4.2.5"
+            "resolved": "https://registry.npmjs.org/ripple-address-codec/-/ripple-address-codec-4.3.0.tgz",
+            "version": "4.3.0"
         },
         "ripple-binary-codec": {
-            "integrity": "sha512-P4ALjAJWBJpRApTQO+dJCrHE6mZxm7ypZot9OS0a3RCKOWTReNw0pDWfdhCGh1qXh71TeQnAk4CHdMLwR/76oQ==",
+            "integrity": "sha512-DuVCZFSOXXPj4Njaj4+8XbYYXQBB+rrnhKd3ON+TtlmtwJUXryc59jKLMGUItqkdf8TAc89pb9+iU3WKlQrhtw==",
             "requires": {
                 "assert": "^2.0.0",
                 "big-integer": "^1.6.48",
-                "buffer": "5.6.0",
+                "buffer": "6.0.3",
                 "create-hash": "^1.2.0",
                 "decimal.js": "^10.2.0",
-                "ripple-address-codec": "^4.2.5"
+                "ripple-address-codec": "^4.3.0"
             },
-            "resolved": "https://registry.npmjs.org/ripple-binary-codec/-/ripple-binary-codec-1.4.3.tgz",
-            "version": "1.4.3"
+            "resolved": "https://registry.npmjs.org/ripple-binary-codec/-/ripple-binary-codec-1.7.1.tgz",
+            "version": "1.7.1"
         },
         "ripple-keypairs": {
-            "integrity": "sha512-wLJXIBsMVazn2Yp/7oP4PvgA4Gd1HtuZLftdEJFNOLgraf82phqa2AnNK3t9f3XeQnApW1jAe/FcFFOY6QUn5w==",
+            "integrity": "sha512-LzM3Up9Pwz3dYqnczzNptimN3AxtjeGbDGeiOzREzbkslKiZcJ615b/ghBN4H23SC6W1GAL95juEzzimDi4THw==",
             "requires": {
                 "bn.js": "^5.1.1",
                 "brorand": "^1.0.5",
                 "elliptic": "^6.5.4",
                 "hash.js": "^1.0.3",
-                "ripple-address-codec": "^4.2.5"
+                "ripple-address-codec": "^4.3.0"
             },
-            "resolved": "https://registry.npmjs.org/ripple-keypairs/-/ripple-keypairs-1.1.5.tgz",
-            "version": "1.1.5"
+            "resolved": "https://registry.npmjs.org/ripple-keypairs/-/ripple-keypairs-1.3.0.tgz",
+            "version": "1.3.0"
         },
         "safe-buffer": {
             "integrity": "sha512-rp3So07KcdmmKbGvgaNxQSJr7bGVSVk5S9Eq1F+ppbRo70+YeaDxkw5Dd8NPN+GD6bjnYm2VuPuCXmpuYvmCXQ==",
             "resolved": "https://registry.npmjs.org/safe-buffer/-/safe-buffer-5.2.1.tgz",
             "version": "5.2.1"
         },
         "seed-random": {
@@ -1314,25 +1316,24 @@
                 "core-util-is": "1.0.2",
                 "extsprintf": "^1.2.0"
             },
             "resolved": "https://registry.npmjs.org/verror/-/verror-1.10.1.tgz",
             "version": "1.10.1"
         },
         "which-typed-array": {
-            "integrity": "sha512-w9c4xkx6mPidwp7180ckYWfMmvxpjlZuIudNtDf4N/tTAUB8VJbX25qZoAsrtGuYNnGw3pa0AXgbGKRB8/EceA==",
+            "integrity": "sha512-qe9UWWpkeG5yzZ0tNYxDmd7vo58HDBc39mZ0xWWpolAGADdFOzkfamWLDxkOWcvHQKVmdTyQdLD4NOfjLWTKew==",
             "requires": {
                 "available-typed-arrays": "^1.0.5",
                 "call-bind": "^1.0.2",
                 "for-each": "^0.3.3",
                 "gopd": "^1.0.1",
-                "has-tostringtag": "^1.0.0",
-                "is-typed-array": "^1.1.10"
+                "has-tostringtag": "^1.0.0"
             },
-            "resolved": "https://registry.npmjs.org/which-typed-array/-/which-typed-array-1.1.9.tgz",
-            "version": "1.1.9"
+            "resolved": "https://registry.npmjs.org/which-typed-array/-/which-typed-array-1.1.11.tgz",
+            "version": "1.1.11"
         },
         "wif": {
             "integrity": "sha512-HIanZn1zmduSF+BQhkE+YXIbEiH0xPr1012QbFEGB0xsKqJii0/SqJjyn8dFv6y36kOznMgMB+LGcbZTJ1xACQ==",
             "requires": {
                 "bs58check": "<3.0.0"
             },
             "resolved": "https://registry.npmjs.org/wif/-/wif-2.0.6.tgz",
@@ -1351,28 +1352,28 @@
         },
         "xmlbuilder": {
             "integrity": "sha512-yMqGBqtXyeN1e3TGYvgNgDVZ3j84W4cwkOXQswghol6APgZWaff9lnbvN7MHYJOiXsvGPXtjTYJEiC9J2wv9Eg==",
             "resolved": "https://registry.npmjs.org/xmlbuilder/-/xmlbuilder-15.1.1.tgz",
             "version": "15.1.1"
         },
         "xrpl": {
-            "integrity": "sha512-P4M/Myxn2U7wl1avAG2Y/JuJMlKw2boLNx0f9woYQJLrS68sICmAfGOYKqPSzwRPc9P7kmydNrk+737nmFW5Vw==",
+            "integrity": "sha512-4zWxsIRzL7E3XGwR8PpMijUgiRrynwFmNv4H9r/eVO6NDw7TtMQz2Yes+6UNsMtn5mm6MAjjQl4hG0X06h9bqw==",
             "requires": {
                 "bignumber.js": "^9.0.0",
                 "bip32": "^2.0.6",
                 "bip39": "^3.0.4",
                 "https-proxy-agent": "^5.0.0",
                 "lodash": "^4.17.4",
-                "ripple-address-codec": "^4.2.5",
-                "ripple-binary-codec": "^1.4.3",
-                "ripple-keypairs": "^1.1.5",
+                "ripple-address-codec": "^4.3.0",
+                "ripple-binary-codec": "^1.7.1",
+                "ripple-keypairs": "^1.3.0",
                 "ws": "^8.2.2"
             },
-            "resolved": "https://registry.npmjs.org/xrpl/-/xrpl-2.7.0.tgz",
-            "version": "2.7.0"
+            "resolved": "https://registry.npmjs.org/xrpl/-/xrpl-2.9.1.tgz",
+            "version": "2.9.1"
         },
         "yallist": {
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
         "yaml": {
@@ -1398,15 +1399,15 @@
     "lockfileVersion": 2,
     "name": "javascript",
     "packages": {
         "": {
             "dependencies": {
                 "@cucumber/cucumber": "^9.1.2",
                 "@cucumber/pretty-formatter": "^1.0.0",
-                "xrpl": "^2.7.0"
+                "xrpl": "^2.9.1"
             }
         },
         "node_modules/@babel/runtime": {
             "dependencies": {
                 "regenerator-runtime": "^0.13.11"
             },
             "engines": {
@@ -1860,20 +1861,34 @@
             },
             "integrity": "sha512-0TS1jicxdU09dwJMNZtVAfzPi6Q6QeN0pM1Fkzrjn+XYHvzMKPU3pHVpva+769iNVSfIYWf7LJ6WR+BuuMf8cA==",
             "resolved": "https://registry.npmjs.org/bs58check/-/bs58check-2.1.2.tgz",
             "version": "2.1.2"
         },
         "node_modules/buffer": {
             "dependencies": {
-                "base64-js": "^1.0.2",
-                "ieee754": "^1.1.4"
+                "base64-js": "^1.3.1",
+                "ieee754": "^1.2.1"
             },
-            "integrity": "sha512-/gDYp/UtU0eA1ys8bOs9J6a+E/KWIY+DZ+Q2WESNUA0jFRsJOc0SNUO6xJ5SGA1xueg3NL65W6s+NY5l9cunuw==",
-            "resolved": "https://registry.npmjs.org/buffer/-/buffer-5.6.0.tgz",
-            "version": "5.6.0"
+            "funding": [
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/feross"
+                },
+                {
+                    "type": "patreon",
+                    "url": "https://www.patreon.com/feross"
+                },
+                {
+                    "type": "consulting",
+                    "url": "https://feross.org/support"
+                }
+            ],
+            "integrity": "sha512-FTiCpNxtwiZZHEZbcbTIcZjERVICn9yq/pDFkTl95/AxzD1naBctN7YO68riM/gLSDY7sdrMby8hofADYuuqOA==",
+            "resolved": "https://registry.npmjs.org/buffer/-/buffer-6.0.3.tgz",
+            "version": "6.0.3"
         },
         "node_modules/buffer-from": {
             "integrity": "sha512-E+XQCRwSbaaiChtv6k6Dwgc+bx+Bs6vuKJHHl5kox/BaKbhiXzqQOwK4cO22yElGp2OCmjwVhT3HmxgyPGnJfQ==",
             "resolved": "https://registry.npmjs.org/buffer-from/-/buffer-from-1.1.2.tgz",
             "version": "1.1.2"
         },
         "node_modules/call-bind": {
@@ -2145,22 +2160,23 @@
             "resolved": "https://registry.npmjs.org/function-bind/-/function-bind-1.1.1.tgz",
             "version": "1.1.1"
         },
         "node_modules/get-intrinsic": {
             "dependencies": {
                 "function-bind": "^1.1.1",
                 "has": "^1.0.3",
+                "has-proto": "^1.0.1",
                 "has-symbols": "^1.0.3"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
-            "integrity": "sha512-L049y6nFOuom5wGyRc3/gdTLO94dySVKRACj1RmJZBQXlbTMhtNIgkWkUHq+jYmZvKf14EW1EoJnnjbmoHij0Q==",
-            "resolved": "https://registry.npmjs.org/get-intrinsic/-/get-intrinsic-1.2.0.tgz",
-            "version": "1.2.0"
+            "integrity": "sha512-2DcsyfABl+gVHEfCOaTrWgyt+tb6MSEGmKq+kI5HwLbIYgjgmMcV8KQ41uaKz1xxUcn9tJtgFbQUEVcEbd0FYw==",
+            "resolved": "https://registry.npmjs.org/get-intrinsic/-/get-intrinsic-1.2.1.tgz",
+            "version": "1.2.1"
         },
         "node_modules/glob": {
             "dependencies": {
                 "fs.realpath": "^1.0.0",
                 "inflight": "^1.0.4",
                 "inherits": "2",
                 "minimatch": "^3.1.1",
@@ -2239,14 +2255,25 @@
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
             "integrity": "sha512-62DVLZGoiEBDHQyqG4w9xCuZ7eJEwNmJRWw2VY84Oedb7WFcA27fiEVe8oUQx9hAUJ4ekurquucTGwsyO1XGdQ==",
             "resolved": "https://registry.npmjs.org/has-property-descriptors/-/has-property-descriptors-1.0.0.tgz",
             "version": "1.0.0"
         },
+        "node_modules/has-proto": {
+            "engines": {
+                "node": ">= 0.4"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/ljharb"
+            },
+            "integrity": "sha512-7qE+iP+O+bgF9clE5+UoBFzE65mlBiVj3tKCrlNQ0Ogwm0BjpT/gK4SlLYDMybDh5I3TCTKnPPa0oMG7JDYrhg==",
+            "resolved": "https://registry.npmjs.org/has-proto/-/has-proto-1.0.1.tgz",
+            "version": "1.0.1"
+        },
         "node_modules/has-symbols": {
             "engines": {
                 "node": ">= 0.4"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
@@ -2456,29 +2483,25 @@
             },
             "integrity": "sha512-hFoiJiTl63nn+kstHGBtewWSKnQLpyb155KHheA1l39uvtO9nWIop1p3udqPcUd/xbF1VLMO4n7OI6p7RbngDg==",
             "resolved": "https://registry.npmjs.org/is-stream/-/is-stream-2.0.1.tgz",
             "version": "2.0.1"
         },
         "node_modules/is-typed-array": {
             "dependencies": {
-                "available-typed-arrays": "^1.0.5",
-                "call-bind": "^1.0.2",
-                "for-each": "^0.3.3",
-                "gopd": "^1.0.1",
-                "has-tostringtag": "^1.0.0"
+                "which-typed-array": "^1.1.11"
             },
             "engines": {
                 "node": ">= 0.4"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
-            "integrity": "sha512-PJqgEHiWZvMpaFZ3uTc8kHPM4+4ADTlDniuQL7cU/UDA0Ql7F70yGfHph3cLNe+c9toaigv+DFzTJKhc2CtO6A==",
-            "resolved": "https://registry.npmjs.org/is-typed-array/-/is-typed-array-1.1.10.tgz",
-            "version": "1.1.10"
+            "integrity": "sha512-Z14TF2JNG8Lss5/HMqt0//T9JeHXttXy5pH/DBU4vi98ozO2btxzq9MwYDZYnKwU8nRsz/+GVFVRDq3DkVuSPg==",
+            "resolved": "https://registry.npmjs.org/is-typed-array/-/is-typed-array-1.1.12.tgz",
+            "version": "1.1.12"
         },
         "node_modules/knuth-shuffle-seeded": {
             "dependencies": {
                 "seed-random": "~2.2.0"
             },
             "integrity": "sha512-9pFH0SplrfyKyojCLxZfMcvkhf5hH0d+UwR9nTVJ/DDQJGuzcXjTwB7TP7sDfehSudlGGaOLblmEWqv04ERVWg==",
             "resolved": "https://registry.npmjs.org/knuth-shuffle-seeded/-/knuth-shuffle-seeded-1.0.6.tgz",
@@ -2797,48 +2820,48 @@
             "dependencies": {
                 "base-x": "^3.0.9",
                 "create-hash": "^1.1.2"
             },
             "engines": {
                 "node": ">= 10"
             },
-            "integrity": "sha512-SZ96zZH+0REeyEcYVFl0vqcsGRXiFXS2RUgHupHhtVkOEk6men53vngVjJwBrSnY+oa6Cri15q1zSni3DEoxNw==",
-            "resolved": "https://registry.npmjs.org/ripple-address-codec/-/ripple-address-codec-4.2.5.tgz",
-            "version": "4.2.5"
+            "integrity": "sha512-Tvd81i7hpDmNqHvkj6iYlj8Tv3I1Romw5gfjni9eacewJvGV2xe+p2y0FAw39z72qfciRMhQyHvpnviBcWVBNw==",
+            "resolved": "https://registry.npmjs.org/ripple-address-codec/-/ripple-address-codec-4.3.0.tgz",
+            "version": "4.3.0"
         },
         "node_modules/ripple-binary-codec": {
             "dependencies": {
                 "assert": "^2.0.0",
                 "big-integer": "^1.6.48",
-                "buffer": "5.6.0",
+                "buffer": "6.0.3",
                 "create-hash": "^1.2.0",
                 "decimal.js": "^10.2.0",
-                "ripple-address-codec": "^4.2.5"
+                "ripple-address-codec": "^4.3.0"
             },
             "engines": {
                 "node": ">= 10"
             },
-            "integrity": "sha512-P4ALjAJWBJpRApTQO+dJCrHE6mZxm7ypZot9OS0a3RCKOWTReNw0pDWfdhCGh1qXh71TeQnAk4CHdMLwR/76oQ==",
-            "resolved": "https://registry.npmjs.org/ripple-binary-codec/-/ripple-binary-codec-1.4.3.tgz",
-            "version": "1.4.3"
+            "integrity": "sha512-DuVCZFSOXXPj4Njaj4+8XbYYXQBB+rrnhKd3ON+TtlmtwJUXryc59jKLMGUItqkdf8TAc89pb9+iU3WKlQrhtw==",
+            "resolved": "https://registry.npmjs.org/ripple-binary-codec/-/ripple-binary-codec-1.7.1.tgz",
+            "version": "1.7.1"
         },
         "node_modules/ripple-keypairs": {
             "dependencies": {
                 "bn.js": "^5.1.1",
                 "brorand": "^1.0.5",
                 "elliptic": "^6.5.4",
                 "hash.js": "^1.0.3",
-                "ripple-address-codec": "^4.2.5"
+                "ripple-address-codec": "^4.3.0"
             },
             "engines": {
                 "node": ">= 10"
             },
-            "integrity": "sha512-wLJXIBsMVazn2Yp/7oP4PvgA4Gd1HtuZLftdEJFNOLgraf82phqa2AnNK3t9f3XeQnApW1jAe/FcFFOY6QUn5w==",
-            "resolved": "https://registry.npmjs.org/ripple-keypairs/-/ripple-keypairs-1.1.5.tgz",
-            "version": "1.1.5"
+            "integrity": "sha512-LzM3Up9Pwz3dYqnczzNptimN3AxtjeGbDGeiOzREzbkslKiZcJ615b/ghBN4H23SC6W1GAL95juEzzimDi4THw==",
+            "resolved": "https://registry.npmjs.org/ripple-keypairs/-/ripple-keypairs-1.3.0.tgz",
+            "version": "1.3.0"
         },
         "node_modules/safe-buffer": {
             "funding": [
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/feross"
                 },
@@ -3097,26 +3120,25 @@
         },
         "node_modules/which-typed-array": {
             "dependencies": {
                 "available-typed-arrays": "^1.0.5",
                 "call-bind": "^1.0.2",
                 "for-each": "^0.3.3",
                 "gopd": "^1.0.1",
-                "has-tostringtag": "^1.0.0",
-                "is-typed-array": "^1.1.10"
+                "has-tostringtag": "^1.0.0"
             },
             "engines": {
                 "node": ">= 0.4"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
-            "integrity": "sha512-w9c4xkx6mPidwp7180ckYWfMmvxpjlZuIudNtDf4N/tTAUB8VJbX25qZoAsrtGuYNnGw3pa0AXgbGKRB8/EceA==",
-            "resolved": "https://registry.npmjs.org/which-typed-array/-/which-typed-array-1.1.9.tgz",
-            "version": "1.1.9"
+            "integrity": "sha512-qe9UWWpkeG5yzZ0tNYxDmd7vo58HDBc39mZ0xWWpolAGADdFOzkfamWLDxkOWcvHQKVmdTyQdLD4NOfjLWTKew==",
+            "resolved": "https://registry.npmjs.org/which-typed-array/-/which-typed-array-1.1.11.tgz",
+            "version": "1.1.11"
         },
         "node_modules/wif": {
             "dependencies": {
                 "bs58check": "<3.0.0"
             },
             "integrity": "sha512-HIanZn1zmduSF+BQhkE+YXIbEiH0xPr1012QbFEGB0xsKqJii0/SqJjyn8dFv6y36kOznMgMB+LGcbZTJ1xACQ==",
             "resolved": "https://registry.npmjs.org/wif/-/wif-2.0.6.tgz",
@@ -3158,25 +3180,25 @@
         "node_modules/xrpl": {
             "dependencies": {
                 "bignumber.js": "^9.0.0",
                 "bip32": "^2.0.6",
                 "bip39": "^3.0.4",
                 "https-proxy-agent": "^5.0.0",
                 "lodash": "^4.17.4",
-                "ripple-address-codec": "^4.2.5",
-                "ripple-binary-codec": "^1.4.3",
-                "ripple-keypairs": "^1.1.5",
+                "ripple-address-codec": "^4.3.0",
+                "ripple-binary-codec": "^1.7.1",
+                "ripple-keypairs": "^1.3.0",
                 "ws": "^8.2.2"
             },
             "engines": {
                 "node": ">=10.13.0"
             },
-            "integrity": "sha512-P4M/Myxn2U7wl1avAG2Y/JuJMlKw2boLNx0f9woYQJLrS68sICmAfGOYKqPSzwRPc9P7kmydNrk+737nmFW5Vw==",
-            "resolved": "https://registry.npmjs.org/xrpl/-/xrpl-2.7.0.tgz",
-            "version": "2.7.0"
+            "integrity": "sha512-4zWxsIRzL7E3XGwR8PpMijUgiRrynwFmNv4H9r/eVO6NDw7TtMQz2Yes+6UNsMtn5mm6MAjjQl4hG0X06h9bqw==",
+            "resolved": "https://registry.npmjs.org/xrpl/-/xrpl-2.9.1.tgz",
+            "version": "2.9.1"
         },
         "node_modules/yallist": {
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/yaml": {
```

### Comparing `claudia-0.1.1/src/claudia/javascript/runSetup` & `claudia-0.1.2/src/claudia/javascript/runSetup`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/javascript/runTest` & `claudia-0.1.2/src/claudia/javascript/runTest`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/network_setup/Dockerfile.rippled_install` & `claudia-0.1.2/src/claudia/network_setup/Dockerfile.rippled_install`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/network_setup/configs/rippled/rippled_1/rippled.cfg` & `claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_1/rippled.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -109,7 +109,8 @@
 TicketBatch
 FlowSortStrands
 fixSTAmountCanonicalize
 fixRmSmallIncreasedQOffers
 CheckCashMakesTrustLine
 NonFungibleTokensV1
 NonFungibleTokensV1_1
+XChainBridge
```

### Comparing `claudia-0.1.1/src/claudia/network_setup/configs/rippled/rippled_2/rippled.cfg` & `claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_2/rippled.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -113,7 +113,8 @@
 TicketBatch
 FlowSortStrands
 fixSTAmountCanonicalize
 fixRmSmallIncreasedQOffers
 CheckCashMakesTrustLine
 NonFungibleTokensV1
 NonFungibleTokensV1_1
+XChainBridge
```

### Comparing `claudia-0.1.1/src/claudia/network_setup/configs/rippled/rippled_3/rippled.cfg` & `claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_4/rippled.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 time.windows.com
 time.apple.com
 time.nist.gov
 pool.ntp.org
 
 # [ips]
 # r.altnet.rippletest.net 51235
-
 [validators_file]
 validators.txt
 
 # Turn down default logging to save disk space in the long run.
 # Valid values here are trace, debug, info, warning, error, and fatal
 [rpc_startup]
 { "command": "log_level", "severity": "warning" }
@@ -66,15 +65,15 @@
 
 
 [ips_fixed]
 rippled_3 2459
 rippled_4 2459
 
 [validation_seed]
-snaAU7bmrkMNwYm1pHFApyTDz6nA1
+snjm2cyL7iLfHkJJZvKKBBGNdaq6e
 
 [amendment_majority_time]
 30 minutes
 
 [features]
 PayChan  
 Flow
@@ -113,7 +112,8 @@
 TicketBatch
 FlowSortStrands
 fixSTAmountCanonicalize
 fixRmSmallIncreasedQOffers
 CheckCashMakesTrustLine
 NonFungibleTokensV1
 NonFungibleTokensV1_1
+XChainBridge
```

### Comparing `claudia-0.1.1/src/claudia/network_setup/configs/rippled/rippled_4/rippled.cfg` & `claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_3/rippled.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 time.windows.com
 time.apple.com
 time.nist.gov
 pool.ntp.org
 
 # [ips]
 # r.altnet.rippletest.net 51235
+
 [validators_file]
 validators.txt
 
 # Turn down default logging to save disk space in the long run.
 # Valid values here are trace, debug, info, warning, error, and fatal
 [rpc_startup]
 { "command": "log_level", "severity": "warning" }
@@ -65,15 +66,15 @@
 
 
 [ips_fixed]
 rippled_3 2459
 rippled_4 2459
 
 [validation_seed]
-snjm2cyL7iLfHkJJZvKKBBGNdaq6e
+snaAU7bmrkMNwYm1pHFApyTDz6nA1
 
 [amendment_majority_time]
 30 minutes
 
 [features]
 PayChan  
 Flow
@@ -112,7 +113,8 @@
 TicketBatch
 FlowSortStrands
 fixSTAmountCanonicalize
 fixRmSmallIncreasedQOffers
 CheckCashMakesTrustLine
 NonFungibleTokensV1
 NonFungibleTokensV1_1
+XChainBridge
```

### Comparing `claudia-0.1.1/src/claudia/network_setup/lib/build.sh` & `claudia-0.1.2/src/claudia/network_setup/lib/build.sh`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/network_setup/lib/rippled_network.yml` & `claudia-0.1.2/src/claudia/network_setup/lib/rippled_network.yml`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/network_setup/lib/setup_helper.sh` & `claudia-0.1.2/src/claudia/network_setup/lib/setup_helper.sh`

 * *Files 0% similar despite different names*

```diff
@@ -426,14 +426,15 @@
       rippled_build_path=$(dirname "${rippled_exec_loc_saved_in_container}")
       rippled_home=$(dirname "${rippled_build_path}")
       echo "- Start ${network} network (with built rippled)"
       echo "  rippled repo: ${rippled_home}"
 
       docker build --quiet -t ${RIPPLED_NODE_CONTAINER_NAME} -f "${RIPPLED_NODE_DOCKER_FILE_BUILD_MODE}" . > /dev/null 2>&1
     else
+      disable_feature true XChainBridge  # TODO: Temporary workaround until sidechain is released/packaged
       echo "- Start ${network} network (with installed rippled)"
       rippled_build_path=""
     fi
     set_rippled_node_env "${rippled_build_path}"
     docker-compose -f "${network_config}" down > /dev/null 2>&1
     docker-compose -f "${network_config}" up -d > /dev/null 2>&1
 
@@ -690,15 +691,15 @@
           feature_enabled=true
         fi
       done
 
       if [ "${feature_enabled}" = "true" ]; then
         echo "- Feature '${feature}' enabled"
         stop_all_networks
-        echo "Please restart required networks"
+        echo "  Please restart required networks"
       else
         echo "- Feature '${feature}' already enabled"
       fi
     else
       echo "Missing parameter <feature name>"
       exit 1
     fi
@@ -721,15 +722,15 @@
           feature_disabled=true
         fi
       done
 
       if [ "${feature_disabled}" = "true" ]; then
         echo "- Feature '${feature}' disabled"
         stop_all_networks
-        echo "Please restart required networks"
+        echo "  Please restart required networks"
       else
         echo "- Feature '${feature}' already disabled"
       fi
     else
       echo "Missing parameter <feature name>. Check help"
       exit 1
     fi
```

### Comparing `claudia-0.1.1/src/claudia/network_setup/lib/sidechain_network.yml` & `claudia-0.1.2/src/claudia/network_setup/lib/sidechain_network.yml`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/network_setup/lib/validate_network.py` & `claudia-0.1.2/src/claudia/network_setup/lib/validate_network.py`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/network_setup/lib/witness_action.sh` & `claudia-0.1.2/src/claudia/network_setup/lib/witness_action.sh`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/network_setup/lib/xchain_bridge_create.py` & `claudia-0.1.2/src/claudia/network_setup/lib/xchain_bridge_create.py`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/network_setup/setup.sh` & `claudia-0.1.2/src/claudia/network_setup/setup.sh`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/python/features/environment.py` & `claudia-0.1.2/src/claudia/python/features/environment.py`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/python/features/steps/nft_mint_burn.py` & `claudia-0.1.2/src/claudia/python/features/steps/nft_mint_burn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import random
 import string
 
 from behave import *
 from hamcrest import assert_that, equal_to, contains_string
 from xrpl.account import get_balance
 from xrpl.models import AccountSet, AccountSetFlag, Tx
-from lib import constants
-from lib.common import *
+from claudia.python.lib.framework import constants
+from claudia.python.lib.framework.common import *
 from claudia.python.lib.framework.object_factory import ObjFactory, ObjType
 
 
 @when('we mint NFT using same token taxon')
 def step_impl(context):
     try:
         payload = ObjFactory.getObj(
```

### Comparing `claudia-0.1.1/src/claudia/python/features/steps/payments.py` & `claudia-0.1.2/src/claudia/python/features/steps/payments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from behave import *
 from xrpl.account import get_balance
 from xrpl.models import IssuedCurrencyAmount, DepositPreauth, AccountSet, AccountSetFlag
 from xrpl.models.requests import Tx
 from xrpl.transaction import (
     safe_sign_and_autofill_transaction,
     send_reliable_submission, submit_transaction, )
-
-from lib.common import get_account_sequence, verify_payment_account_objects, verify_account_balance, \
-    get_account_balance, verify_test_status, verify_test_error_message, ResponseCode
-
+from claudia.python.lib.framework.common import *
 from claudia.python.lib.framework.object_factory import ObjFactory, ObjType
 
 
 @when('we send a payment of "{transfer_amount}" XRP from Alice to Bob')
 def step_impl(context, transfer_amount):
     try:
         context.transferAmount = float(transfer_amount) if '.' in transfer_amount else int(transfer_amount)
```

### Comparing `claudia-0.1.1/src/claudia/python/features/steps/trustline.py` & `claudia-0.1.2/src/claudia/python/features/steps/trustline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from behave import *
 from hamcrest import assert_that, equal_to, contains_string
 from xrpl.account import get_balance
 from xrpl.models import AccountSet, AccountSetFlag
-
-from lib.common import generate_issued_currency_amount, sign_autofill_and_submit, \
-    verify_trustline_account_objects, verify_payment_account_objects, ResponseCode, \
-    generate_path_step, verify_offer_create_account_objects, sanitize_args
-
+from claudia.python.lib.framework.common import *
 from claudia.python.lib.framework.object_factory import ObjFactory, ObjType
 
 
 @when('we send a trustline payment using one currency from Alice to Bob')
 def step_impl(context):
     try:
         context.transferAmount = "10000"
```

### Comparing `claudia-0.1.1/src/claudia/python/lib/framework/common.py` & `claudia-0.1.2/src/claudia/python/lib/framework/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,18 @@
 from xrpl.account import get_balance, get_account_info
 from xrpl.asyncio.transaction import XRPLReliableSubmissionException
 from xrpl.models import IssuedCurrencyAmount, PathStep
 from xrpl.transaction import (
     safe_sign_and_autofill_transaction,
     send_reliable_submission, safe_sign_transaction)
 from xrpl.wallet import Wallet
-
 from claudia.python.lib.exceptions.InvalidInputException import InvalidInputException
-from claudia.python.lib.framework import constants
-
 from claudia.python.lib.exceptions.UnconfiguredEnvironmentException import UnconfiguredEnvironmentException
-
 from claudia.python.lib.framework.object_factory import ObjFactory, ObjType
+from claudia.python.lib.framework import constants
 
 
 class ResponseCode(str, Enum):
     success = "tesSUCCESS"
     path_dry = "tecPATH_DRY"
     no_destination = "tecNO_DST"
     no_line_redundant = "tecNO_LINE_REDUNDANT"
```

### Comparing `claudia-0.1.1/src/claudia/python/lib/framework/object_factory.py` & `claudia-0.1.2/src/claudia/python/lib/framework/object_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from enum import Enum
 
 from xrpl.models import Payment, TrustSet, AccountLines, AccountObjects, OfferCreate, NFTokenMint, NFTokenBurn, \
     TicketCreate, AccountDelete, AccountNFTs, Tx, Memo, LedgerCurrent, NFTokenCreateOffer, NFTokenAcceptOffer
-
 from claudia.python.lib.exceptions.InvalidInputException import InvalidInputException
 
 
 class ObjFactory(object):
     @staticmethod
     def getObj(obj_type, **kwargs):
         payload = {}
```

### Comparing `claudia-0.1.1/src/claudia/python/lib/framework/workflow_helper.py` & `claudia-0.1.2/src/claudia/python/lib/framework/workflow_helper.py`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/python/runSetup` & `claudia-0.1.2/src/claudia/python/runSetup`

 * *Files identical despite different names*

### Comparing `claudia-0.1.1/src/claudia/python/runTest` & `claudia-0.1.2/src/claudia/python/runTest`

 * *Files identical despite different names*

