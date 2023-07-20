# Comparing `tmp/fosslight_yocto-3.1.20.tar.gz` & `tmp/fosslight_yocto-3.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fosslight_yocto-3.1.20.tar", last modified: Tue Jul 11 01:51:26 2023, max compression
+gzip compressed data, was "fosslight_yocto-3.1.21.tar", last modified: Thu Jul 20 23:44:31 2023, max compression
```

## Comparing `fosslight_yocto-3.1.20.tar` & `fosslight_yocto-3.1.21.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:51:26.563582 fosslight_yocto-3.1.20/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 01:51:16.000000 fosslight_yocto-3.1.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 01:51:16.000000 fosslight_yocto-3.1.20/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-11 01:51:26.563582 fosslight_yocto-3.1.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-11 01:51:16.000000 fosslight_yocto-3.1.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:51:26.559582 fosslight_yocto-3.1.20/files_for_preparation/
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-11 01:51:16.000000 fosslight_yocto-3.1.20/files_for_preparation/bom.bbclass
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-11 01:51:16.000000 fosslight_yocto-3.1.20/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 01:51:26.563582 fosslight_yocto-3.1.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-11 01:51:16.000000 fosslight_yocto-3.1.20/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:51:26.555582 fosslight_yocto-3.1.20/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:51:26.559582 fosslight_yocto-3.1.20/src/fosslight_yocto/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:51:16.000000 fosslight_yocto-3.1.20/src/fosslight_yocto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-11 01:51:16.000000 fosslight_yocto-3.1.20/src/fosslight_yocto/_help.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5691 2023-07-11 01:51:16.000000 fosslight_yocto-3.1.20/src/fosslight_yocto/_overwrite_yaml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9496 2023-07-11 01:51:16.000000 fosslight_yocto-3.1.20/src/fosslight_yocto/_package_item.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3601 2023-07-11 01:51:16.000000 fosslight_yocto-3.1.20/src/fosslight_yocto/_write_result_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-11 01:51:16.000000 fosslight_yocto-3.1.20/src/fosslight_yocto/_zip_source_works.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43781 2023-07-11 01:51:16.000000 fosslight_yocto-3.1.20/src/fosslight_yocto/create_oss_report_for_yocto.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8200 2023-07-11 01:51:16.000000 fosslight_yocto-3.1.20/src/fosslight_yocto/parsing_meta_doubleopen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:51:26.563582 fosslight_yocto-3.1.20/src/fosslight_yocto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-11 01:51:26.000000 fosslight_yocto-3.1.20/src/fosslight_yocto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-11 01:51:26.000000 fosslight_yocto-3.1.20/src/fosslight_yocto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 01:51:26.000000 fosslight_yocto-3.1.20/src/fosslight_yocto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-11 01:51:26.000000 fosslight_yocto-3.1.20/src/fosslight_yocto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-11 01:51:26.000000 fosslight_yocto-3.1.20/src/fosslight_yocto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 01:51:26.000000 fosslight_yocto-3.1.20/src/fosslight_yocto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:44:31.200653 fosslight_yocto-3.1.21/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 23:44:21.000000 fosslight_yocto-3.1.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-20 23:44:21.000000 fosslight_yocto-3.1.21/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-20 23:44:31.200653 fosslight_yocto-3.1.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-20 23:44:21.000000 fosslight_yocto-3.1.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:44:31.200653 fosslight_yocto-3.1.21/files_for_preparation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-20 23:44:21.000000 fosslight_yocto-3.1.21/files_for_preparation/bom.bbclass
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-20 23:44:21.000000 fosslight_yocto-3.1.21/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 23:44:31.200653 fosslight_yocto-3.1.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-20 23:44:21.000000 fosslight_yocto-3.1.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:44:31.200653 fosslight_yocto-3.1.21/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:44:31.200653 fosslight_yocto-3.1.21/src/fosslight_yocto/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:44:21.000000 fosslight_yocto-3.1.21/src/fosslight_yocto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-20 23:44:21.000000 fosslight_yocto-3.1.21/src/fosslight_yocto/_help.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5691 2023-07-20 23:44:21.000000 fosslight_yocto-3.1.21/src/fosslight_yocto/_overwrite_yaml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9496 2023-07-20 23:44:21.000000 fosslight_yocto-3.1.21/src/fosslight_yocto/_package_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3601 2023-07-20 23:44:21.000000 fosslight_yocto-3.1.21/src/fosslight_yocto/_write_result_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-20 23:44:21.000000 fosslight_yocto-3.1.21/src/fosslight_yocto/_zip_source_works.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43781 2023-07-20 23:44:21.000000 fosslight_yocto-3.1.21/src/fosslight_yocto/create_oss_report_for_yocto.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8200 2023-07-20 23:44:21.000000 fosslight_yocto-3.1.21/src/fosslight_yocto/parsing_meta_doubleopen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:44:31.200653 fosslight_yocto-3.1.21/src/fosslight_yocto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-20 23:44:31.000000 fosslight_yocto-3.1.21/src/fosslight_yocto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-20 23:44:31.000000 fosslight_yocto-3.1.21/src/fosslight_yocto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 23:44:31.000000 fosslight_yocto-3.1.21/src/fosslight_yocto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-20 23:44:31.000000 fosslight_yocto-3.1.21/src/fosslight_yocto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-20 23:44:31.000000 fosslight_yocto-3.1.21/src/fosslight_yocto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 23:44:31.000000 fosslight_yocto-3.1.21/src/fosslight_yocto.egg-info/top_level.txt
```

### Comparing `fosslight_yocto-3.1.20/LICENSE` & `fosslight_yocto-3.1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.20/PKG-INFO` & `fosslight_yocto-3.1.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight_yocto
-Version: 3.1.20
+Version: 3.1.21
 Summary: FOSSLight Yocto
 Home-page: https://github.com/fosslight/fosslight_yocto_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_yocto_scanner
 Description: <!--
         SPDX-FileCopyrightText: Copyright 2023 LG Electronics Inc.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fosslight_yocto Version: 3.1.20 Summary: FOSSLight
+Metadata-Version: 2.1 Name: fosslight_yocto Version: 3.1.21 Summary: FOSSLight
 Yocto Home-page: https://github.com/fosslight/fosslight_yocto_scanner Author:
 LG Electronics License: Apache-2.0 Download-URL: https://github.com/fosslight/
 fosslight_yocto_scanner Description:
                                                                        [Korean]
 # FOSSLight Yocto Scanner [FOSSLight Yocto Scanner is released under the
 Apache-2.0 License.] [Current python package version.] [https://img.shields.io/
 pypi/pyversions/fosslight_yocto] [![REUSE status](https://api.reuse.software/
```

### Comparing `fosslight_yocto-3.1.20/README.md` & `fosslight_yocto-3.1.21/README.md`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.20/files_for_preparation/bom.bbclass` & `fosslight_yocto-3.1.21/files_for_preparation/bom.bbclass`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,18 @@
                 pkg_lic[pkg] = lic
     jsondata["pkg_lic"] = pkg_lic
     jsondata["pe"] = d.getVar("PE", True)
     jsondata["pv"] = d.getVar("PV", True)
     jsondata["pr"] = d.getVar("PR", True)
     jsondata["extendprauto"] = d.getVar("EXTENDPRAUTO", True)
     jsondata["extendpkgv"] = d.getVar("EXTENDPKGV", True)
-     
+    jsondata["description"] = d.getVar("DESCRIPTION", True)
+    jsondata["summary"] = d.getVar("SUMMARY", True)
+    jsondata["cve_check_whitelist "] = d.getVar("CVE_CHECK_WHITELIST", True)
+
     datafile = os.path.join(d.getVar("TOPDIR", True), "bom.json")
     lock = bb.utils.lockfile(datafile + '.lock')
     with open(datafile, "a") as f:
         json.dump(jsondata, f, sort_keys=True, cls=BomJSONEncoder)
         f.write(',\n')
     bb.utils.unlockfile(lock)
 }
```

### Comparing `fosslight_yocto-3.1.20/setup.py` & `fosslight_yocto-3.1.21/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 if __name__ == "__main__":
     setup(
         name='fosslight_yocto',
-        version='3.1.20',
+        version='3.1.21',
         package_dir={"": "src"},
         packages=find_packages(where='src'),
         description='FOSSLight Yocto',
         long_description=readme,
         long_description_content_type='text/markdown',
         license='Apache-2.0',
         author='LG Electronics',
```

### Comparing `fosslight_yocto-3.1.20/src/fosslight_yocto/_help.py` & `fosslight_yocto-3.1.21/src/fosslight_yocto/_help.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.20/src/fosslight_yocto/_overwrite_yaml.py` & `fosslight_yocto-3.1.21/src/fosslight_yocto/_overwrite_yaml.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.20/src/fosslight_yocto/_package_item.py` & `fosslight_yocto-3.1.21/src/fosslight_yocto/_package_item.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.20/src/fosslight_yocto/_write_result_file.py` & `fosslight_yocto-3.1.21/src/fosslight_yocto/_write_result_file.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.20/src/fosslight_yocto/_zip_source_works.py` & `fosslight_yocto-3.1.21/src/fosslight_yocto/_zip_source_works.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.20/src/fosslight_yocto/create_oss_report_for_yocto.py` & `fosslight_yocto-3.1.21/src/fosslight_yocto/create_oss_report_for_yocto.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.20/src/fosslight_yocto/parsing_meta_doubleopen.py` & `fosslight_yocto-3.1.21/src/fosslight_yocto/parsing_meta_doubleopen.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.20/src/fosslight_yocto.egg-info/PKG-INFO` & `fosslight_yocto-3.1.21/src/fosslight_yocto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight-yocto
-Version: 3.1.20
+Version: 3.1.21
 Summary: FOSSLight Yocto
 Home-page: https://github.com/fosslight/fosslight_yocto_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_yocto_scanner
 Description: <!--
         SPDX-FileCopyrightText: Copyright 2023 LG Electronics Inc.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fosslight-yocto Version: 3.1.20 Summary: FOSSLight
+Metadata-Version: 2.1 Name: fosslight-yocto Version: 3.1.21 Summary: FOSSLight
 Yocto Home-page: https://github.com/fosslight/fosslight_yocto_scanner Author:
 LG Electronics License: Apache-2.0 Download-URL: https://github.com/fosslight/
 fosslight_yocto_scanner Description:
                                                                        [Korean]
 # FOSSLight Yocto Scanner [FOSSLight Yocto Scanner is released under the
 Apache-2.0 License.] [Current python package version.] [https://img.shields.io/
 pypi/pyversions/fosslight_yocto] [![REUSE status](https://api.reuse.software/
```

### Comparing `fosslight_yocto-3.1.20/src/fosslight_yocto.egg-info/SOURCES.txt` & `fosslight_yocto-3.1.21/src/fosslight_yocto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

