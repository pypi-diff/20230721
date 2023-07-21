# Comparing `tmp/dagster_cloud_examples-1.4.0.tar.gz` & `tmp/dagster_cloud_examples-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_cloud_examples-1.4.0.tar", last modified: Thu Jul 20 22:04:35 2023, max compression
+gzip compressed data, was "dagster_cloud_examples-1.4.1.tar", last modified: Fri Jul 21 15:39:31 2023, max compression
```

## Comparing `dagster_cloud_examples-1.4.0.tar` & `dagster_cloud_examples-1.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:35.448227 dagster_cloud_examples-1.4.0/
--rw-r--r--   0 root         (0) root         (0)      319 2023-07-20 22:04:35.448227 dagster_cloud_examples-1.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-20 21:53:47.000000 dagster_cloud_examples-1.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:35.444227 dagster_cloud_examples-1.4.0/dagster_cloud_examples/
--rw-r--r--   0 root         (0) root         (0)       60 2023-07-20 21:53:47.000000 dagster_cloud_examples-1.4.0/dagster_cloud_examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:35.444227 dagster_cloud_examples-1.4.0/dagster_cloud_examples/cereals/
--rw-r--r--   0 root         (0) root         (0)       63 2023-07-20 21:53:47.000000 dagster_cloud_examples-1.4.0/dagster_cloud_examples/cereals/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:35.448227 dagster_cloud_examples-1.4.0/dagster_cloud_examples/cereals/jobs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud_examples-1.4.0/dagster_cloud_examples/cereals/jobs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:35.448227 dagster_cloud_examples-1.4.0/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud_examples-1.4.0/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:35.448227 dagster_cloud_examples-1.4.0/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/ops/
--rw-r--r--   0 root         (0) root         (0)      770 2023-07-20 21:53:47.000000 dagster_cloud_examples-1.4.0/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/ops/__init__.py
--rw-r--r--   0 root         (0) root         (0)      374 2023-07-20 21:53:47.000000 dagster_cloud_examples-1.4.0/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/process_cereals.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-07-20 21:53:47.000000 dagster_cloud_examples-1.4.0/dagster_cloud_examples/cereals/repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:35.448227 dagster_cloud_examples-1.4.0/dagster_cloud_examples/cereals/schedules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud_examples-1.4.0/dagster_cloud_examples/cereals/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)      367 2023-07-20 21:53:47.000000 dagster_cloud_examples-1.4.0/dagster_cloud_examples/cereals/schedules/daily_process_cereals.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-20 21:53:47.000000 dagster_cloud_examples-1.4.0/dagster_cloud_examples/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:35.444227 dagster_cloud_examples-1.4.0/dagster_cloud_examples.egg-info/
--rw-r--r--   0 root         (0) root         (0)      319 2023-07-20 22:04:35.000000 dagster_cloud_examples-1.4.0/dagster_cloud_examples.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2023-07-20 22:04:35.000000 dagster_cloud_examples-1.4.0/dagster_cloud_examples.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:04:35.000000 dagster_cloud_examples-1.4.0/dagster_cloud_examples.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-20 22:04:35.000000 dagster_cloud_examples-1.4.0/dagster_cloud_examples.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 22:04:35.000000 dagster_cloud_examples-1.4.0/dagster_cloud_examples.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 22:04:35.448227 dagster_cloud_examples-1.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      956 2023-07-20 21:53:47.000000 dagster_cloud_examples-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:31.510977 dagster_cloud_examples-1.4.1/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-07-21 15:39:31.510977 dagster_cloud_examples-1.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-21 15:29:17.000000 dagster_cloud_examples-1.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:31.498977 dagster_cloud_examples-1.4.1/dagster_cloud_examples/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-21 15:29:17.000000 dagster_cloud_examples-1.4.1/dagster_cloud_examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:31.502977 dagster_cloud_examples-1.4.1/dagster_cloud_examples/cereals/
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-21 15:29:17.000000 dagster_cloud_examples-1.4.1/dagster_cloud_examples/cereals/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:31.502977 dagster_cloud_examples-1.4.1/dagster_cloud_examples/cereals/jobs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 15:29:17.000000 dagster_cloud_examples-1.4.1/dagster_cloud_examples/cereals/jobs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:31.502977 dagster_cloud_examples-1.4.1/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 15:29:17.000000 dagster_cloud_examples-1.4.1/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:31.502977 dagster_cloud_examples-1.4.1/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/ops/
+-rw-r--r--   0 root         (0) root         (0)      770 2023-07-21 15:29:17.000000 dagster_cloud_examples-1.4.1/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/ops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      374 2023-07-21 15:29:17.000000 dagster_cloud_examples-1.4.1/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/process_cereals.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-07-21 15:29:17.000000 dagster_cloud_examples-1.4.1/dagster_cloud_examples/cereals/repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:31.510977 dagster_cloud_examples-1.4.1/dagster_cloud_examples/cereals/schedules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 15:29:17.000000 dagster_cloud_examples-1.4.1/dagster_cloud_examples/cereals/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      367 2023-07-21 15:29:17.000000 dagster_cloud_examples-1.4.1/dagster_cloud_examples/cereals/schedules/daily_process_cereals.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 15:29:17.000000 dagster_cloud_examples-1.4.1/dagster_cloud_examples/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:31.498977 dagster_cloud_examples-1.4.1/dagster_cloud_examples.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-07-21 15:39:31.000000 dagster_cloud_examples-1.4.1/dagster_cloud_examples.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2023-07-21 15:39:31.000000 dagster_cloud_examples-1.4.1/dagster_cloud_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:39:31.000000 dagster_cloud_examples-1.4.1/dagster_cloud_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-21 15:39:31.000000 dagster_cloud_examples-1.4.1/dagster_cloud_examples.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 15:39:31.000000 dagster_cloud_examples-1.4.1/dagster_cloud_examples.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 15:39:31.510977 dagster_cloud_examples-1.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      956 2023-07-21 15:29:17.000000 dagster_cloud_examples-1.4.1/setup.py
```

### Comparing `dagster_cloud_examples-1.4.0/README.md` & `dagster_cloud_examples-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dagster_cloud_examples-1.4.0/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/ops/__init__.py` & `dagster_cloud_examples-1.4.1/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_examples-1.4.0/dagster_cloud_examples.egg-info/SOURCES.txt` & `dagster_cloud_examples-1.4.1/dagster_cloud_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster_cloud_examples-1.4.0/setup.py` & `dagster_cloud_examples-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ver = get_version()
 # dont pin dev installs to avoid pip dep resolver issues
 pin = "" if ver == "1!0+dev" else f"=={ver}"
 setup(
     name="dagster_cloud_examples",
     version=ver,
     packages=find_packages(exclude=["dagster_cloud_examples_tests*"]),
-    install_requires=["dagster_cloud==1.4.0"],
+    install_requires=["dagster_cloud==1.4.1"],
     extras_require={"tests": ["mypy", "pylint", "pytest"]},
     author="Elementl",
     author_email="hello@elementl.com",
     license="Apache-2.0",
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
```

