# Comparing `tmp/aqueduct-py-0.0.2.tar.gz` & `tmp/aqueduct-py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduct-py-0.0.2.tar", last modified: Fri Jun  9 18:35:07 2023, max compression
+gzip compressed data, was "aqueduct-py-0.0.3.tar", last modified: Thu Jul 20 23:59:38 2023, max compression
```

## Comparing `aqueduct-py-0.0.2.tar` & `aqueduct-py-0.0.3.tar`

### file list

```diff
@@ -1,64 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:35:07.150212 aqueduct-py-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-09 18:35:07.150212 aqueduct-py-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-09 18:35:07.150212 aqueduct-py-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:35:07.142212 aqueduct-py-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:35:07.142212 aqueduct-py-0.0.2/src/aqueduct/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:35:07.142212 aqueduct-py-0.0.2/src/aqueduct/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39484 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/core/aq.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/core/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/core/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/core/recordable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/core/setpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/core/socket_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/core/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:35:07.142212 aqueduct-py-0.0.2/src/aqueduct/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/devices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:35:07.142212 aqueduct-py-0.0.2/src/aqueduct/devices/balance/
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/devices/balance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:35:07.146212 aqueduct-py-0.0.2/src/aqueduct/devices/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/devices/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20137 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/devices/base/obj.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/devices/base/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:35:07.146212 aqueduct-py-0.0.2/src/aqueduct/devices/optical_density/
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/devices/optical_density/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:35:07.146212 aqueduct-py-0.0.2/src/aqueduct/devices/ph/
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/devices/ph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:35:07.146212 aqueduct-py-0.0.2/src/aqueduct/devices/pressure/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/devices/pressure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/devices/pressure/transducer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:35:07.146212 aqueduct-py-0.0.2/src/aqueduct/devices/pump/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/devices/pump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/devices/pump/peristaltic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:35:07.146212 aqueduct-py-0.0.2/src/aqueduct/devices/pump/syringe/
--rw-r--r--   0 runner    (1001) docker     (123)    25869 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/devices/pump/syringe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:35:07.146212 aqueduct-py-0.0.2/src/aqueduct/devices/pump/syringe/types/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/devices/pump/syringe/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/devices/pump/syringe/types/tricontinent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:35:07.146212 aqueduct-py-0.0.2/src/aqueduct/devices/test_device/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/devices/test_device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:35:07.146212 aqueduct-py-0.0.2/src/aqueduct/devices/valve/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/devices/valve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/devices/valve/pinch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:35:07.146212 aqueduct-py-0.0.2/src/aqueduct/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:35:07.146212 aqueduct-py-0.0.2/src/aqueduct/tests/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/tests/devices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:35:07.146212 aqueduct-py-0.0.2/src/aqueduct/tests/devices/pump/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/tests/devices/pump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/tests/devices/pump/test_syringe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 18:34:58.000000 aqueduct-py-0.0.2/src/aqueduct/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:35:07.150212 aqueduct-py-0.0.2/src/aqueduct_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-09 18:35:07.000000 aqueduct-py-0.0.2/src/aqueduct_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-09 18:35:07.000000 aqueduct-py-0.0.2/src/aqueduct_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:35:07.000000 aqueduct-py-0.0.2/src/aqueduct_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 18:35:07.000000 aqueduct-py-0.0.2/src/aqueduct_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 18:35:07.000000 aqueduct-py-0.0.2/src/aqueduct_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:35:06.000000 aqueduct-py-0.0.2/src/aqueduct_py.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.445730 aqueduct-py-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-20 23:59:38.445730 aqueduct-py-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-20 23:59:38.445730 aqueduct-py-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.437730 aqueduct-py-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.441730 aqueduct-py-0.0.3/src/aqueduct/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.441730 aqueduct-py-0.0.3/src/aqueduct/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39568 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/core/aq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/core/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/core/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/core/recordable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/core/setpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/core/socket_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/core/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.441730 aqueduct-py-0.0.3/src/aqueduct/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.441730 aqueduct-py-0.0.3/src/aqueduct/devices/balance/
+-rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/balance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.441730 aqueduct-py-0.0.3/src/aqueduct/devices/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22565 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/base/obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/base/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.441730 aqueduct-py-0.0.3/src/aqueduct/devices/mass_flow/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/mass_flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/mass_flow/meter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.441730 aqueduct-py-0.0.3/src/aqueduct/devices/optical_density/
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/optical_density/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.441730 aqueduct-py-0.0.3/src/aqueduct/devices/ph/
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/ph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.441730 aqueduct-py-0.0.3/src/aqueduct/devices/pressure/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/pressure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/pressure/transducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.441730 aqueduct-py-0.0.3/src/aqueduct/devices/pump/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/pump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/pump/peristaltic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.441730 aqueduct-py-0.0.3/src/aqueduct/devices/pump/syringe/
+-rw-r--r--   0 runner    (1001) docker     (123)    27479 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/pump/syringe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.441730 aqueduct-py-0.0.3/src/aqueduct/devices/pump/syringe/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/pump/syringe/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/pump/syringe/types/tricontinent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.441730 aqueduct-py-0.0.3/src/aqueduct/devices/temperature/
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/temperature/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.441730 aqueduct-py-0.0.3/src/aqueduct/devices/test_device/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/test_device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.441730 aqueduct-py-0.0.3/src/aqueduct/devices/valve/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/valve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/valve/pinch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/devices/valve/solenoid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.441730 aqueduct-py-0.0.3/src/aqueduct/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.441730 aqueduct-py-0.0.3/src/aqueduct/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/tests/core/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/tests/core/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.445730 aqueduct-py-0.0.3/src/aqueduct/tests/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/tests/devices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.445730 aqueduct-py-0.0.3/src/aqueduct/tests/devices/pump/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/tests/devices/pump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/tests/devices/pump/test_syringe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 23:59:30.000000 aqueduct-py-0.0.3/src/aqueduct/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:59:38.445730 aqueduct-py-0.0.3/src/aqueduct_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-20 23:59:38.000000 aqueduct-py-0.0.3/src/aqueduct_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-20 23:59:38.000000 aqueduct-py-0.0.3/src/aqueduct_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 23:59:38.000000 aqueduct-py-0.0.3/src/aqueduct_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 23:59:38.000000 aqueduct-py-0.0.3/src/aqueduct_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 23:59:38.000000 aqueduct-py-0.0.3/src/aqueduct_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 23:59:38.000000 aqueduct-py-0.0.3/src/aqueduct_py.egg-info/zip-safe
```

### Comparing `aqueduct-py-0.0.2/PKG-INFO` & `aqueduct-py-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Aqueduct Core package.
 Home-page: http://packages.python.org/*
 Author: Aqueduct Fluidics, LLC
 Author-email: info@aqueductfluidics.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -16,34 +16,36 @@
 
 <p><img src="https://github.com/aqueductfluidics/.github/blob/main/profile/assets/images/logo_blue.svg" alt="Aqueduct Fluidics" /></p>
 
 # Aqueduct Fluidics Python API
 
 The Aqueduct Fluidics Python API is a Python-based software package designed for laboratory automation and instrumentation. It provides an abstraction layer that allows operators to write Python code to interface with devices such as pumps, valves, and sensors, without having to deal with low-level communication protocols.
 
-## Features
-
--   Abstraction layer for device communication
--   User-friendly interface for device control and data acquisition
--   Supports integration with various laboratory instruments and software platforms
+You can find complete documentation here [here](https://docs.aqueductfluidics.com).
 
 ## Getting Started
 
 To get started with the Aqueduct Fluidics Core Application, simply install it using `pip`:
 
 ```bash
 pip install aqueduct-py
 ```
 
 ## Testing
 
 Install with dev dependencies.
 
 ```text
-python -m pip install -e .[test]
+python -m pip install -e '.[test]'
 ```
 
 To test
 
 ```text
 python -m pytest src
 ```
+
+## Pre-Commit Hooks
+
+```text
+pre-commit run --all-files
+```
```

### Comparing `aqueduct-py-0.0.2/README.md` & `aqueduct-py-0.0.3/src/aqueduct_py.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,51 @@
+Metadata-Version: 2.1
+Name: aqueduct-py
+Version: 0.0.3
+Summary: Aqueduct Core package.
+Home-page: http://packages.python.org/*
+Author: Aqueduct Fluidics, LLC
+Author-email: info@aqueductfluidics.com
+License: BSD
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.7.1
+Description-Content-Type: text/markdown
+Provides-Extra: test
+
 <p><img src="https://github.com/aqueductfluidics/.github/blob/main/profile/assets/images/logo_blue.svg" alt="Aqueduct Fluidics" /></p>
 
 # Aqueduct Fluidics Python API
 
 The Aqueduct Fluidics Python API is a Python-based software package designed for laboratory automation and instrumentation. It provides an abstraction layer that allows operators to write Python code to interface with devices such as pumps, valves, and sensors, without having to deal with low-level communication protocols.
 
-## Features
-
--   Abstraction layer for device communication
--   User-friendly interface for device control and data acquisition
--   Supports integration with various laboratory instruments and software platforms
+You can find complete documentation here [here](https://docs.aqueductfluidics.com).
 
 ## Getting Started
 
 To get started with the Aqueduct Fluidics Core Application, simply install it using `pip`:
 
 ```bash
 pip install aqueduct-py
 ```
 
 ## Testing
 
 Install with dev dependencies.
 
 ```text
-python -m pip install -e .[test]
+python -m pip install -e '.[test]'
 ```
 
 To test
 
 ```text
 python -m pytest src
 ```
+
+## Pre-Commit Hooks
+
+```text
+pre-commit run --all-files
+```
```

### Comparing `aqueduct-py-0.0.2/setup.cfg` & `aqueduct-py-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `aqueduct-py-0.0.2/src/aqueduct/core/aq.py` & `aqueduct-py-0.0.3/src/aqueduct/core/aq.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 from aqueduct.core.setpoint import Setpoint
 from aqueduct.core.socket_constants import Events
 from aqueduct.core.socket_constants import OK
 from aqueduct.core.socket_constants import SOCKET_DELAY_S
 from aqueduct.core.socket_constants import SOCKET_TX_ATTEMPTS
 from aqueduct.core.socket_constants import SocketCommands
 from aqueduct.core.utils import send_and_wait_for_rx
+from aqueduct.core.utils import split_packets
 from aqueduct.core.utils import string_to_bool
 from aqueduct.devices.base.obj import Device
 from aqueduct.devices.base.utils import create_device
 
 
 class InitParams:
     """
@@ -820,17 +821,18 @@
         while i < SOCKET_TX_ATTEMPTS:
             try:
                 with self._socket_lock:
                     self._socket.settimeout(1)
                     self._socket.send(message)
                     time.sleep(SOCKET_DELAY_S)
                     data = self._socket.recv(1024 * 8)
-                commands = json.loads(data.replace(b"][", b","))
-                for cmd, _payload in zip(commands[::2], commands[1::2]):
-                    if cmd == Events.UPDATED_USER_PARAMS.value:
+                packets = split_packets(data)
+                for packet in packets:
+                    command = json.loads(packet)
+                    if command[0] == Events.UPDATED_USER_PARAMS.value:
                         return
             except (json.decoder.JSONDecodeError, socket.timeout) as err:
                 if self.is_debug:
                     print(f"update_setpoint error: {err}")
                 continue
             i += 1
 
@@ -872,18 +874,20 @@
         """
         message = json.dumps(
             [
                 SocketCommands.SocketMessage.value,
                 [Events.CLEAR_USER_RECORDABLES.value, dict(params=[recordable.name])],
             ]
         ).encode()
-        self._socket.settimeout(1)
-        with self._socket_lock:
-            self._socket.send(message)
-            time.sleep(SOCKET_DELAY_S)
+
+        self.send_and_wait_for_rx(
+            message,
+            Events.CLEAR_USER_RECORDABLES.value,
+            SOCKET_TX_ATTEMPTS,
+        )
 
     def handle_updated_setpoint(self, setpoint: dict):
         """
         Handle a new value for a setpoint received from the server.
 
         Args:
             setpoint (dict): a dictionary containing the updated setpoint.
@@ -1007,18 +1011,19 @@
         If an exception is raised while processing the data, the exception is printed
         if debug mode is enabled. The method runs until `_run` is set to False.
         """
         while self._run:
             try:
                 while True:
                     data = self._socket.recv(1024 * 16)
-                    commands = json.loads(data.replace(b"][", b","))
-                    for cmd, payload in zip(commands[::2], commands[1::2]):
-                        if cmd == Events.UPDATED_USER_PARAMS.value:
-                            self.handle_updated_user_params(json.loads(payload))
+                    packets = split_packets(data)
+                    for packet in packets:
+                        command = json.loads(packet)
+                        if command[0] == Events.UPDATED_USER_PARAMS.value:
+                            self.handle_updated_user_params(json.loads(command[1]))
                     time.sleep(self._update_frequency_s)
             except BaseException as err:  # pylint: disable=broad-except
                 if self._aq.is_debug:
                     print(f"AqHelper error: {err}")
 
     def handle_updated_user_params(self, message):
         """Processes updated user parameters and calls `handle_updated_setpoint` with each updated parameter.
@@ -1181,19 +1186,19 @@
         Returns:
             None
         """
         while self._run:
             try:
                 while True:
                     data = self._socket.recv(1024 * 16)
-                    commands = json.loads(data.replace(b"][", b","))
-                    for cmd, payload in zip(commands[::2], commands[1::2]):
-                        if cmd == "recipe_status":
-                            self.handle_recipe_status(json.loads(payload))
-
+                    packets = split_packets(data)
+                    for packet in packets:
+                        command = json.loads(packet)
+                        if command[0] == Events.RECIPE_STATUS.value:
+                            self.handle_recipe_status(json.loads(command[1]))
                     time.sleep(self._update_frequency_s)
 
             except json.JSONDecodeError as err:
                 if self._debug:
                     print(f"AqManager JSON decode error: {err}")
             except ConnectionResetError as err:
                 if self._debug:
```

### Comparing `aqueduct-py-0.0.2/src/aqueduct/core/input.py` & `aqueduct-py-0.0.3/src/aqueduct/core/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,32 +193,34 @@
                     [
                         Events.GET_RECIPE_INPUT_VALUE.value,
                         dict(user_id=self._aq.user_id),
                     ],
                 ]
             ).encode()
 
+            # small delay
+            # time.sleep(0.05)
+
             _, data = send_and_wait_for_rx(
                 message=message,
                 sock=self._aq.socket,
                 lock=self._aq.socket_lock,
                 response=Events.GET_RECIPE_INPUT_VALUE.value,
                 size=4096 * 8,
             )
 
             try:
-                v = json.loads(data)
-                v = v.get("value")
+                v = json.loads(data).get("value")
                 if self.dtype == float.__name__:
                     return float(v)
                 elif self.dtype == int.__name__:
                     return int(v)
                 else:
                     return v
-            except BaseException as _e:
+            except BaseException as _e:  # pylint: disable=broad-except
                 return None
 
     def to_json(self):
         """
         Return a JSON representation of the Input object.
 
         :return: A JSON-encoded string representation of the Input object.
```

### Comparing `aqueduct-py-0.0.2/src/aqueduct/core/logging.py` & `aqueduct-py-0.0.3/src/aqueduct/core/logging.py`

 * *Files identical despite different names*

### Comparing `aqueduct-py-0.0.2/src/aqueduct/core/prompt.py` & `aqueduct-py-0.0.3/src/aqueduct/core/prompt.py`

 * *Files identical despite different names*

### Comparing `aqueduct-py-0.0.2/src/aqueduct/core/recordable.py` & `aqueduct-py-0.0.3/src/aqueduct/core/recordable.py`

 * *Files identical despite different names*

### Comparing `aqueduct-py-0.0.2/src/aqueduct/core/setpoint.py` & `aqueduct-py-0.0.3/src/aqueduct/core/setpoint.py`

 * *Files identical despite different names*

### Comparing `aqueduct-py-0.0.2/src/aqueduct/core/socket_constants.py` & `aqueduct-py-0.0.3/src/aqueduct/core/socket_constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     GET_DEVICE = "get_device"
     GET_DEVICE_LIVE = "get_device_live"
     GET_RECIPE_INPUT = "get_recipe_input"
     GET_RECIPE_INPUT_VALUE = "get_recipe_input_value"
     GET_RECIPE_PROMPT = "get_recipe_prompt"
     GET_SETUP = "get_setup"
     PAUSE_RECIPE = "pause_recipe"
+    RECIPE_STATUS = "recipe_status"
     REGISTER_PROCESS = "register_process"
     SET_RECIPE_INPUT = "set_recipe_input"
     SET_RECIPE_PROMPT = "set_recipe_prompt"
     UPDATE_PROCESS = "update_process"
     UPDATE_USER_PARAMS = "update_user_params"
     UPDATE_USER_RECORDABLES = "update_user_recordables"
     UPDATED_USER_PARAMS = "updated_user_params"
@@ -55,7 +56,8 @@
     Stop = 4
     ChangeSpeed = 5
     SetValvePosition = 6
     Tare = 7
     SetCalibration = 8
     Initialize = 9
     SetPlunger = 10
+    Zero = 11
```

### Comparing `aqueduct-py-0.0.2/src/aqueduct/core/utils.py` & `aqueduct-py-0.0.3/src/aqueduct/core/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -35,14 +35,37 @@
         return True
     elif str(string).lower() in ("false", "0"):
         return False
     else:
         raise TypeError(f"Could not convert {string} to a boolean value.")
 
 
+def split_packets(message: bytes) -> typing.Tuple[bytes]:
+    """
+    Split a byte string message into packets and extract the command and payload pairs.
+
+    :param message: The byte string message to be split.
+    :type message: bytes
+    :return: A tuple of tuples containing the command and payload pairs.
+    :rtype: tuple
+    """
+    if b"][" in message:
+        packets = message.split(b"][")
+
+        for i in range(len(packets)):
+            if i == 0:
+                packets[i] = packets[i] + b"]"
+            elif i == len(packets) - 1:
+                packets[i] = b"[" + packets[i]
+    else:
+        packets = (message,)
+
+    return tuple(packets)
+
+
 # pylint: disable=too-many-arguments
 def send_and_wait_for_rx(
     message: str,
     sock: socket.socket,
     lock: typing.Union["threading.Lock", None],
     response: str,
     attempts: int = SOCKET_TX_ATTEMPTS,
@@ -83,19 +106,21 @@
 
         except socket.timeout:
             # Socket timeout occurred, increment attempt counter and continue the loop.
             i += 1
             continue
 
         try:
-            j = json.loads(data)
-            if j[0] == response:
-                if delay_s is not None:
-                    time.sleep(delay_s)
-                return True, j[1]
+            packets = split_packets(data)
+            for packet in packets:
+                j = json.loads(packet)
+                if j[0] == response:
+                    if delay_s is not None:
+                        time.sleep(delay_s)
+                    return True, j[1]
         except (json.decoder.JSONDecodeError, IndexError):
             # Error occurred while parsing the received data as JSON, continue the loop.
             continue
 
         i += 1
 
     # No successful response within the given attempts, return False and None.
```

### Comparing `aqueduct-py-0.0.2/src/aqueduct/devices/balance/__init__.py` & `aqueduct-py-0.0.3/src/aqueduct/devices/balance/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,17 @@
     # initialize the Aqueduct core application and the balance device
     aq = Aqueduct(user_id, ip_address, port)
     balance = aq.devices.get("balance")
 
     # tare the balance
     balance.tare()
 
+    # zero the balance
+    balance.zero()
+
     # get a weight reading from the balance
     weight = balance.get_value()
 
     # get all weight readings from the balance
     weights = balance.get_all_values()
 
 """
@@ -109,14 +112,27 @@
         """
         commands = self.len * [None]
         commands[index] = 1
 
         payload = self.to_payload(Actions.Tare, {"commands": commands}, record)
         self.send_command(payload)
 
+    def zero(self, index: int = 0, record: Union[bool, None] = None):
+        """
+        Send a zero command to the balance device.
+
+        :param index: number-like value to specify the input of the balance to zero
+        :type index: int
+        """
+        commands = self.len * [None]
+        commands[index] = 1
+
+        payload = self.to_payload(Actions.Zero, {"commands": commands}, record)
+        self.send_command(payload)
+
     def value(self, index: int = 0):
         """
         Get a weight value reading from the balance device.
 
         :param index: input to read from, `0` is first input
         :type index: int
         :return: value, in grams
```

### Comparing `aqueduct-py-0.0.2/src/aqueduct/devices/base/obj.py` & `aqueduct-py-0.0.3/src/aqueduct/devices/base/obj.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,63 @@
 import json
 import socket
 import threading
 import time
 from abc import ABC
 from abc import abstractmethod
 from typing import Callable
-from typing import List
+from typing import Optional
 from typing import TypeVar
 
 from aqueduct.core.socket_constants import Actions
 from aqueduct.core.socket_constants import Events
 from aqueduct.core.socket_constants import SOCKET_DELAY_S
 from aqueduct.core.socket_constants import SOCKET_TX_ATTEMPTS
 from aqueduct.core.socket_constants import SocketCommands
 from aqueduct.core.utils import send_and_wait_for_rx
 
 
 # pylint: disable=invalid-name
+class DeviceKeys(enum.Enum):
+    """The keys to extract data from the Device."""
+
+    Live = "live"
+    Stat = "stat"
+    Config = "config"
+    Base = "base"
+
+
+# pylint: disable=invalid-name
+class DeviceBaseKeys(enum.Enum):
+    """The keys to extract data from the Device Base."""
+
+    DeviceId = "device_id"
+    UserId = "user_id"
+    Type = "type"
+    Name = "name"
+    Interface = "interface"
+
+
+# pylint: disable=invalid-name
+class DeviceConfigKeys(enum.Enum):
+    """The keys to extract data from the Device Config."""
+
+    Type = "type"
+    Config = "config"
+
+
+# pylint: disable=invalid-name
+class DeviceConfigInnerKeys(enum.Enum):
+    """The keys to extract data from the Device Config inner data structure."""
+
+    Data = "data"
+    Protocol = "protocol"
+
+
+# pylint: disable=invalid-name
 class Interface(enum.IntEnum):
     """The interface of the Device."""
 
     Sim = 0
     Can = 1
     Ethernet = 2
     Serial = 3
@@ -199,20 +236,33 @@
     Devices are instantiated in Recipes and contain the attributes necessary
     to control execution between the device worker and the main recipe thread.
     """
 
     def __init__(self, sock: socket.socket, socket_lock: threading.Lock, **kwargs):
         self._socket: socket.socket = sock
         self._socket_lock: threading.Lock = socket_lock
-        self._device_id: int = kwargs.get("base").get("device_id")
-        self._user_id: str = kwargs.get("base").get("user_id")
-        self._type: str = kwargs.get("base").get("type")
-        self._name: str = kwargs.get("base").get("name")
-        self._interface: Interface = kwargs.get("base").get("interface")
-        self._len: int = len(kwargs.get("live"))
+
+        self._device_id: int = kwargs.get(DeviceKeys.Base.value).get(
+            DeviceBaseKeys.DeviceId.value
+        )
+        self._user_id: str = kwargs.get(DeviceKeys.Base.value).get(
+            DeviceBaseKeys.UserId.value
+        )
+        self._type: str = kwargs.get(DeviceKeys.Base.value).get(
+            DeviceBaseKeys.Type.value
+        )
+        self._name: str = kwargs.get(DeviceKeys.Base.value).get(
+            DeviceBaseKeys.Name.value
+        )
+        self._interface: Interface = kwargs.get(DeviceKeys.Base.value).get(
+            DeviceBaseKeys.Interface.value
+        )
+
+        self._len: int = len(kwargs.get(DeviceKeys.Live.value))
+
         self._command_delay: float = 0.0
         self._has_sim_values: bool = False
 
         if self.interface == Interface.Sim:
             self._command_delay = 0.0
         else:
             self._command_delay: float = 0.01
@@ -340,15 +390,15 @@
                     self._socket.settimeout(0.5)
                     self._socket.send(message)
                     time.sleep(SOCKET_DELAY_S)
                     data = self._socket.recv(4096 * 8)
                 j = json.loads(data)
                 if j[0] == Events.GET_DEVICE.value:
                     data = json.loads(j[1]).get("device")
-                    base = data.get("base")
+                    base = data.get(DeviceKeys.Base.value)
                     if self.is_for_me(base):
                         return data
             except (json.decoder.JSONDecodeError, socket.timeout) as _err:
                 continue
             i += 1
 
     def get_live(self):
@@ -368,15 +418,15 @@
                     self._socket.send(message)
                     time.sleep(SOCKET_DELAY_S)
                     data = self._socket.recv(1024 * 8)
                 j = json.loads(data)
                 if j[0] == Events.GET_DEVICE_LIVE.value:
                     data = json.loads(j[1])
                     if self.is_for_me(data):
-                        return data.get("live")
+                        return data.get(DeviceKeys.Live.value)
             except (json.decoder.JSONDecodeError, socket.timeout) as _err:
                 continue
             i += 1
 
     T = TypeVar("T")
 
     def get_live_and_cast(self, cast: Callable) -> tuple:
@@ -400,57 +450,59 @@
         :param cast: The casting function to apply to each stat data entry.
         :type cast: Callable
         :return: The casted stat data as a tuple.
         :rtype: tuple
         """
         stat = []
         v = self.get()
-        for i in v.get("stat"):
+        for i in v.get(DeviceKeys.Stat.value):
             stat.append(cast(**i))
         return tuple(stat)
 
     def get_config_and_cast(self, cast: Callable) -> tuple:
         """
         Get the config data and cast it using the provided casting function.
 
         :param cast: The casting function to apply to each config data entry.
         :type cast: Callable
         :return: The casted config data as a tuple.
         :rtype: tuple
         """
-        config = []
-        v = self.get()
-        for i in v.get("config"):
-            config.append(cast(**i))
-        return tuple(config)
+        val = self.get_config()
+        return cast(val)
 
     def get_config(self) -> Config:
         """
         Get the config data.
 
         :return: The casted config data as a tuple.
         :rtype: tuple
         """
         v = self.get()
-        v = v.get("config")
+        v = v.get(DeviceKeys.Config.value)
         return self.extract_config(v)
 
     def extract_config(self, data):
         """
         Recursively extract the configuration data from a nested dictionary.
 
         Args:
             data (dict): The dictionary to extract the configuration data from.
 
         Returns:
             dict or None: The extracted configuration data if found, or None if not found.
         """
         if isinstance(data, dict):
-            if "config" in data and "type" in data:
-                config_data = self.extract_config_data(data["config"])
+            if (
+                DeviceConfigKeys.Config.value in data
+                and DeviceConfigKeys.Type.value in data
+            ):
+                config_data = self.extract_config_data(
+                    data[DeviceConfigKeys.Config.value]
+                )
                 if config_data is not None:
                     return data
             for value in data.values():
                 config_data = self.extract_config(value)
                 if config_data:
                     return config_data
         return None
@@ -462,15 +514,18 @@
         Args:
             data (dict): The dictionary to extract the configuration data from.
 
         Returns:
             dict or None: The extracted configuration data if found, or None if not found.
         """
         if isinstance(data, dict):
-            if "data" in data and "protocol" in data:
+            if (
+                DeviceConfigInnerKeys.Data.value in data
+                and DeviceConfigInnerKeys.Protocol.value in data
+            ):
                 return data
         return None
 
     def extract_live_as_tuple(
         self, key: str, cast: Callable[[str], T] = None
     ) -> tuple[T]:
         """
@@ -551,47 +606,70 @@
 
     def _set_sim_data(
         self,
         values: list[float | None] | tuple | None,
         roc: list[float | None] | tuple | None,
         noise: list[float | None] | tuple | None,
         scale: float = 1.0,
+        conversion_func: Callable[[float], float] | None = None,
     ):
         """
         Sets the simulated data for the device.
 
         :param values: The simulated values.
         :type values: list[float | None] | tuple | None
         :param roc: The rates of change for the simulated values.
         :type roc: list[float | None] | tuple | None
         :param noise: The noise values for the simulated data.
         :type noise: list[float | None] | tuple | None
+        :param conversion_func: Optional conversion function to apply to the values. Default is None.
+        :type conversion_func: Callable[[float], float], optional
         :param scale: Optional scaling factor for unit conversion. Default is 1.0.
         :type scale: float, optional
         :raises Warning: If the device does not have simulated values.
         """
         if self.has_sim_values:
             v_t = []
             for i in range(0, self.len):
-                v_v = (
-                    values[i] * scale
+                value = (
+                    values[i]
                     if values and i < len(values) and values[i] is not None
                     else None
                 )
-                r_c = (
-                    roc[i] * scale
-                    if roc and i < len(roc) and roc[i] is not None
-                    else None
+                roc_value = (
+                    roc[i] if roc and i < len(roc) and roc[i] is not None else None
                 )
-                n_v = (
-                    noise[i] * scale
+                noise_value = (
+                    noise[i]
                     if noise and i < len(noise) and noise[i] is not None
                     else None
                 )
-                v_t.append((v_v, r_c, n_v))
+
+                if conversion_func is not None:
+                    value = (
+                        conversion_func(value * scale) if value is not None else None
+                    )
+                    roc_value = (
+                        conversion_func(roc_value * scale)
+                        if roc_value is not None
+                        else None
+                    )
+                    noise_value = (
+                        conversion_func(noise_value * scale)
+                        if noise_value is not None
+                        else None
+                    )
+                else:
+                    value = value * scale if value is not None else None
+                    roc_value = roc_value * scale if roc_value is not None else None
+                    noise_value = (
+                        noise_value * scale if noise_value is not None else None
+                    )
+
+                v_t.append((value, roc_value, noise_value))
 
             payload = self.to_payload(Actions.SetSimValues, v_t, None)
             self.send_command(payload)
 
         else:
             raise Warning(f"{self.name} does not have simulated values.")
```

### Comparing `aqueduct-py-0.0.2/src/aqueduct/devices/optical_density/__init__.py` & `aqueduct-py-0.0.3/src/aqueduct/devices/optical_density/__init__.py`

 * *Files identical despite different names*

### Comparing `aqueduct-py-0.0.2/src/aqueduct/devices/ph/__init__.py` & `aqueduct-py-0.0.3/src/aqueduct/devices/ph/__init__.py`

 * *Files identical despite different names*

### Comparing `aqueduct-py-0.0.2/src/aqueduct/devices/pressure/transducer.py` & `aqueduct-py-0.0.3/src/aqueduct/devices/pressure/transducer.py`

 * *Files identical despite different names*

### Comparing `aqueduct-py-0.0.2/src/aqueduct/devices/pump/peristaltic.py` & `aqueduct-py-0.0.3/src/aqueduct/devices/pump/peristaltic.py`

 * *Files identical despite different names*

### Comparing `aqueduct-py-0.0.2/src/aqueduct/devices/pump/syringe/__init__.py` & `aqueduct-py-0.0.3/src/aqueduct/devices/pump/syringe/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,19 +44,23 @@
 from typing import List
 from typing import Tuple
 from typing import Union
 
 from aqueduct.core.socket_constants import Actions
 from aqueduct.devices.base.obj import Command
 from aqueduct.devices.base.obj import Device
+from aqueduct.devices.base.obj import DeviceConfigInnerKeys
+from aqueduct.devices.base.obj import DeviceConfigKeys
 
 from .types import Config
 from .types import tricontinent
 
 # pylint: disable=invalid-name
+
+
 class Mode(enum.IntEnum):
     """Operational Mode of the `SyringePump`. Use this value to set the operation to continuous or finite."""
 
     Continuous = 0
     Finite = 1
 
 
@@ -446,14 +450,46 @@
         Get the stat data of the syringe pump.
 
         Returns:
             Tuple[SyringePumpStat]: The stat data of the syringe pump as a tuple of SyringePumpStat objects.
         """
         return self.get_stat_and_cast(SyringePumpStat.from_stat)
 
+    @property
+    def config(self) -> Union[tuple, None]:
+        """
+        Get the configuration data for the syringe pump device.
+
+        This property retrieves the device configuration and casts it to the appropriate types.
+
+        :return: The device configuration data.
+        :rtype: Union[tuple, None]
+        """
+
+        def cast_config(data):
+            if (
+                data
+                and data.get(DeviceConfigKeys.Type.value) == Config.TriContinent.value
+            ):
+                configs = []
+                for _i, d in enumerate(
+                    data.get(DeviceConfigKeys.Config.value).get(
+                        DeviceConfigInnerKeys.Data.value
+                    )
+                ):
+                    configs.append(tricontinent.TriContinentConfig(**d))
+                data[DeviceConfigKeys.Config.value][
+                    DeviceConfigInnerKeys.Data.value
+                ] = configs
+                return data
+            else:
+                return data
+
+        return self.get_config_and_cast(cast_config)
+
     def start(
         self,
         commands: List[Union[StartCommand, None]],
         record: Union[bool, None] = None,
     ) -> dict:
         """Command to start one or more pump inputs in either finite or continuous mode.
 
@@ -731,20 +767,26 @@
 
         config = self.get_config()
         values = [1000000.0] * self.len
 
         if config is None:
             return values
 
-        if config.get("type") == Config.TriContinent.value:
+        if config.get(DeviceConfigKeys.Type.value) == Config.TriContinent.value:
             live = self.live
             stat = self.stat
 
-            for i, d in enumerate(config.get("config").get("data")):
-                pump_series = d.get("pump_series")
+            for i, d in enumerate(
+                config.get(DeviceConfigKeys.Config.value).get(
+                    DeviceConfigInnerKeys.Data.value
+                )
+            ):
+                pump_series = d.get(
+                    tricontinent.TriContinentConfigKeys.PumpSeries.value
+                )
                 resolution = live[i].plunger_mode
                 syringe_volume_ul = stat[i].syringe_volume_ul
                 value = tricontinent.max_rate_ul_min(
                     pump_series, resolution, syringe_volume_ul
                 )
                 if value is not None:
                     values[i] = value
@@ -761,20 +803,26 @@
 
         config = self.get_config()
         values = [0.0] * self.len
 
         if config is None:
             return values
 
-        if config.get("type") == Config.TriContinent.value:
+        if config.get(DeviceConfigKeys.Type.value) == Config.TriContinent.value:
             live = self.live
             stat = self.stat
 
-            for i, d in enumerate(config.get("config").get("data")):
-                pump_series = d.get("pump_series")
+            for i, d in enumerate(
+                config.get(DeviceConfigKeys.Config.value).get(
+                    DeviceConfigInnerKeys.Data.value
+                )
+            ):
+                pump_series = d.get(
+                    tricontinent.TriContinentConfigKeys.PumpSeries.value
+                )
                 resolution = live[i].plunger_mode
                 syringe_volume_ul = stat[i].syringe_volume_ul
 
                 value = tricontinent.min_rate_ul_min(
                     pump_series, resolution, syringe_volume_ul
                 )
                 if value is not None:
```

### Comparing `aqueduct-py-0.0.2/src/aqueduct/devices/test_device/__init__.py` & `aqueduct-py-0.0.3/src/aqueduct/devices/test_device/__init__.py`

 * *Files identical despite different names*

### Comparing `aqueduct-py-0.0.2/src/aqueduct/devices/valve/pinch.py` & `aqueduct-py-0.0.3/src/aqueduct/devices/valve/pinch.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         """
         if index < len(commands):
             commands[index] = command
         else:
             raise Warning("PinchValve: command index larger than device size!")
 
     @staticmethod
-    def make_set_poisition_command(pct_open: float) -> SetPositionCommand:
+    def make_set_position_command(pct_open: float) -> SetPositionCommand:
         """
         Helper method to create a SetPositionCommand object.
 
         :param pct_open: Percentage open value
 
         :return: SetPositionCommand object
         """
```

### Comparing `aqueduct-py-0.0.2/src/aqueduct/tests/devices/pump/test_syringe.py` & `aqueduct-py-0.0.3/src/aqueduct/tests/devices/pump/test_syringe.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,15 @@
     def test_int_to_status(self) -> None:
         s = Status.Infusing.value
         assert s == 1
         assert Status(s) == Status.Infusing
 
     def test_reverse(self) -> None:
         s = Status.Infusing
-        print(s)
         s = s.reverse()
-        print(s)
         assert s == Status.Withdrawing
         s = s.reverse()
         assert s == Status.Infusing
         s = Status.Stopped
         s = s.reverse()
         assert s == Status.Stopped
         s = Status.Paused
```

### Comparing `aqueduct-py-0.0.2/src/aqueduct/tests/test_imports.py` & `aqueduct-py-0.0.3/src/aqueduct/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `aqueduct-py-0.0.2/src/aqueduct_py.egg-info/SOURCES.txt` & `aqueduct-py-0.0.3/src/aqueduct_py.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,28 +15,35 @@
 src/aqueduct/core/units.py
 src/aqueduct/core/utils.py
 src/aqueduct/devices/__init__.py
 src/aqueduct/devices/balance/__init__.py
 src/aqueduct/devices/base/__init__.py
 src/aqueduct/devices/base/obj.py
 src/aqueduct/devices/base/utils.py
+src/aqueduct/devices/mass_flow/__init__.py
+src/aqueduct/devices/mass_flow/meter.py
 src/aqueduct/devices/optical_density/__init__.py
 src/aqueduct/devices/ph/__init__.py
 src/aqueduct/devices/pressure/__init__.py
 src/aqueduct/devices/pressure/transducer.py
 src/aqueduct/devices/pump/__init__.py
 src/aqueduct/devices/pump/peristaltic.py
 src/aqueduct/devices/pump/syringe/__init__.py
 src/aqueduct/devices/pump/syringe/types/__init__.py
 src/aqueduct/devices/pump/syringe/types/tricontinent.py
+src/aqueduct/devices/temperature/__init__.py
 src/aqueduct/devices/test_device/__init__.py
 src/aqueduct/devices/valve/__init__.py
 src/aqueduct/devices/valve/pinch.py
+src/aqueduct/devices/valve/solenoid.py
 src/aqueduct/tests/__init__.py
 src/aqueduct/tests/test_imports.py
+src/aqueduct/tests/core/__init__.py
+src/aqueduct/tests/core/test_units.py
+src/aqueduct/tests/core/test_utils.py
 src/aqueduct/tests/devices/__init__.py
 src/aqueduct/tests/devices/pump/__init__.py
 src/aqueduct/tests/devices/pump/test_syringe.py
 src/aqueduct_py.egg-info/PKG-INFO
 src/aqueduct_py.egg-info/SOURCES.txt
 src/aqueduct_py.egg-info/dependency_links.txt
 src/aqueduct_py.egg-info/requires.txt
```

