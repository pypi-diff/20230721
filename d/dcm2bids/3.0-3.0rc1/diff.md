# Comparing `tmp/dcm2bids-3.0.tar.gz` & `tmp/dcm2bids-3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcm2bids-3.0.tar", last modified: Fri Jul 21 19:48:17 2023, max compression
+gzip compressed data, was "dcm2bids-3.0rc1.tar", last modified: Mon Jul 17 17:54:31 2023, max compression
```

## Comparing `dcm2bids-3.0.tar` & `dcm2bids-3.0rc1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:48:17.641231 dcm2bids-3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35235 2023-07-21 19:48:09.000000 dcm2bids-3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 19:48:09.000000 dcm2bids-3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-07-21 19:48:17.641231 dcm2bids-3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-21 19:48:09.000000 dcm2bids-3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:48:17.641231 dcm2bids-3.0/dcm2bids/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:48:09.000000 dcm2bids-3.0/dcm2bids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-07-21 19:48:09.000000 dcm2bids-3.0/dcm2bids/acquisition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:48:17.641231 dcm2bids-3.0/dcm2bids/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:48:09.000000 dcm2bids-3.0/dcm2bids/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-21 19:48:09.000000 dcm2bids-3.0/dcm2bids/cli/dcm2bids.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-21 19:48:09.000000 dcm2bids-3.0/dcm2bids/cli/dcm2bids_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-21 19:48:09.000000 dcm2bids-3.0/dcm2bids/cli/dcm2bids_scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-07-21 19:48:09.000000 dcm2bids-3.0/dcm2bids/dcm2bids_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-21 19:48:09.000000 dcm2bids-3.0/dcm2bids/dcm2niix_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-21 19:48:09.000000 dcm2bids-3.0/dcm2bids/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    20267 2023-07-21 19:48:09.000000 dcm2bids-3.0/dcm2bids/sidecar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:48:17.641231 dcm2bids-3.0/dcm2bids/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:48:09.000000 dcm2bids-3.0/dcm2bids/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-21 19:48:09.000000 dcm2bids-3.0/dcm2bids/utils/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-21 19:48:09.000000 dcm2bids-3.0/dcm2bids/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-21 19:48:09.000000 dcm2bids-3.0/dcm2bids/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-21 19:48:09.000000 dcm2bids-3.0/dcm2bids/utils/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-21 19:48:09.000000 dcm2bids-3.0/dcm2bids/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-07-21 19:48:09.000000 dcm2bids-3.0/dcm2bids/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-21 19:48:09.000000 dcm2bids-3.0/dcm2bids/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:48:17.641231 dcm2bids-3.0/dcm2bids.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-07-21 19:48:17.000000 dcm2bids-3.0/dcm2bids.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-21 19:48:17.000000 dcm2bids-3.0/dcm2bids.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:48:17.000000 dcm2bids-3.0/dcm2bids.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-21 19:48:17.000000 dcm2bids-3.0/dcm2bids.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 19:48:17.000000 dcm2bids-3.0/dcm2bids.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 19:48:17.000000 dcm2bids-3.0/dcm2bids.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:48:09.000000 dcm2bids-3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 19:48:17.641231 dcm2bids-3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1078 2023-07-21 19:48:09.000000 dcm2bids-3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:54:31.735131 dcm2bids-3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35235 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-17 17:54:31.735131 dcm2bids-3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:54:31.731131 dcm2bids-3.0rc1/dcm2bids/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/acquisition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:54:31.731131 dcm2bids-3.0rc1/dcm2bids/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/cli/dcm2bids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/cli/dcm2bids_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/cli/dcm2bids_scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/dcm2bids_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/dcm2niix_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20267 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/sidecar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:54:31.735131 dcm2bids-3.0rc1/dcm2bids/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/utils/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/utils/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:54:31.731131 dcm2bids-3.0rc1/dcm2bids.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-17 17:54:31.000000 dcm2bids-3.0rc1/dcm2bids.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-17 17:54:31.000000 dcm2bids-3.0rc1/dcm2bids.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:54:31.000000 dcm2bids-3.0rc1/dcm2bids.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-17 17:54:31.000000 dcm2bids-3.0rc1/dcm2bids.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 17:54:31.000000 dcm2bids-3.0rc1/dcm2bids.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 17:54:31.000000 dcm2bids-3.0rc1/dcm2bids.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 17:54:31.735131 dcm2bids-3.0rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1078 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/setup.py
```

### Comparing `dcm2bids-3.0/LICENSE.txt` & `dcm2bids-3.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcm2bids-3.0/PKG-INFO` & `dcm2bids-3.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcm2bids
-Version: 3.0
+Version: 3.0rc1
 Summary: Reorganising NIfTI files from dcm2niix into the Brain Imaging Data Structure
 Maintainer: Arnaud Boré
 Maintainer-email: arnaud.bore@gmail.com
 License: GPLv3+
 Project-URL: Documentation, https://unfmontreal.github.io/Dcm2Bids
 Project-URL: Source Code, https://github.com/unfmontreal/Dcm2Bids
 Platform: OS Independent
@@ -91,14 +91,14 @@
 [bids]: http://bids.neuroimaging.io/
 [bids-examples]: https://github.com/bids-standard/bids-examples
 [bids-spec]: https://bids-specification.readthedocs.io/en/stable/
 [dcm2bids-doc]: https://unfmontreal.github.io/Dcm2Bids
 [dcm2bids-install]: https://unfmontreal.github.io/Dcm2Bids/latest/get-started/install/
 [dcm2bids-tutorial]: https://unfmontreal.github.io/Dcm2Bids/latest/tutorial/first-steps/#tutorial-first-steps
 [dcm2bids-advanced]: https://unfmontreal.github.io/Dcm2Bids/latest/advanced/
-[dcm2bids-upgrade]: https://unfmontreal.github.io/Dcm2Bids/dev/upgrade/
+[dcm2bids-upgrade]: https://unfmontreal.github.io/Dcm2Bids/latest/upgrade/
 [dcm2bids-issues]: https://github.com/UNFmontreal/Dcm2Bids/issues
 [dcm2niix-install]: https://github.com/rordenlab/dcm2niix#install
 [dcm2niix-github]: https://github.com/rordenlab/dcm2niix
 [neurostars]: https://neurostars.org/
 [neurostars-dcm2bids]: https://neurostars.org/tag/dcm2bids
 [dcm2bids-contributing]:  https://unfmontreal.github.io/Dcm2Bids/latest/how-to/contributing/
```

### Comparing `dcm2bids-3.0/README.md` & `dcm2bids-3.0rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,14 @@
 [bids]: http://bids.neuroimaging.io/
 [bids-examples]: https://github.com/bids-standard/bids-examples
 [bids-spec]: https://bids-specification.readthedocs.io/en/stable/
 [dcm2bids-doc]: https://unfmontreal.github.io/Dcm2Bids
 [dcm2bids-install]: https://unfmontreal.github.io/Dcm2Bids/latest/get-started/install/
 [dcm2bids-tutorial]: https://unfmontreal.github.io/Dcm2Bids/latest/tutorial/first-steps/#tutorial-first-steps
 [dcm2bids-advanced]: https://unfmontreal.github.io/Dcm2Bids/latest/advanced/
-[dcm2bids-upgrade]: https://unfmontreal.github.io/Dcm2Bids/dev/upgrade/
+[dcm2bids-upgrade]: https://unfmontreal.github.io/Dcm2Bids/latest/upgrade/
 [dcm2bids-issues]: https://github.com/UNFmontreal/Dcm2Bids/issues
 [dcm2niix-install]: https://github.com/rordenlab/dcm2niix#install
 [dcm2niix-github]: https://github.com/rordenlab/dcm2niix
 [neurostars]: https://neurostars.org/
 [neurostars-dcm2bids]: https://neurostars.org/tag/dcm2bids
 [dcm2bids-contributing]:  https://unfmontreal.github.io/Dcm2Bids/latest/how-to/contributing/
```

### Comparing `dcm2bids-3.0/dcm2bids/acquisition.py` & `dcm2bids-3.0rc1/dcm2bids/acquisition.py`

 * *Files 6% similar despite different names*

```diff
@@ -208,41 +208,35 @@
         for key, value in self.sidecar_changes.items():
             values = []
 
             if not isinstance(value, list):
                 value = [value]
 
             for val in value:
-                if isinstance(val, str) or isinstance(val, bool):
+                if isinstance(val, str):
                     if val not in idList and key in DEFAULT.keyWithPathsidecar_changes:
                         logging.warning(f"No id found for '{key}' value '{val}'.")
                         logging.warning(f"No sidecar changes for field '{key}' "
                                         f"will be made "
                                         f"for json file '{self.dstFile}.json' "
                                         "with this id.")
                     else:
                         values.append(idList.get(val, val))
-                        if values[-1] != val:
-                            if isinstance(values[-1], list):
-                                values[-1] = "bids::" + values[-1][0]
-                            else:
-                                 values[-1] = "bids::" + values[-1]
 
             # handle if nested list vs str
             flat_value_list = []
             for item in values:
                 if isinstance(item, list):
                     flat_value_list += item
                 else:
                     flat_value_list.append(item)
-            
             if len(flat_value_list) == 1:
-                data[key] = flat_value_list[0]
-            else:
-                data[key] = flat_value_list
+                flat_value_list = flat_value_list[0]
+
+            data[key] = flat_value_list
 
         return data
 
     @staticmethod
     def prepend(value, char="_"):
         """ Prepend `char` to `value` if necessary
```

### Comparing `dcm2bids-3.0/dcm2bids/cli/dcm2bids.py` & `dcm2bids-3.0rc1/dcm2bids/cli/dcm2bids.py`

 * *Files identical despite different names*

### Comparing `dcm2bids-3.0/dcm2bids/cli/dcm2bids_helper.py` & `dcm2bids-3.0rc1/dcm2bids/cli/dcm2bids_helper.py`

 * *Files identical despite different names*

### Comparing `dcm2bids-3.0/dcm2bids/cli/dcm2bids_scaffold.py` & `dcm2bids-3.0rc1/dcm2bids/cli/dcm2bids_scaffold.py`

 * *Files identical despite different names*

### Comparing `dcm2bids-3.0/dcm2bids/dcm2bids_gen.py` & `dcm2bids-3.0rc1/dcm2bids/dcm2bids_gen.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,19 +151,17 @@
                 else:
                     self.logger.info("Use --clobber option to overwrite")
                     continue
 
             # Populate idList
             if '.nii' in ext:
                 if acquisition.id in idList:
-                    idList[acquisition.id].append(os.path.join(acquisition.participant.name,
-                                                               acquisition.dstId + "".join(ext)))
+                    idList[acquisition.id].append(acquisition.dstId + "".join(ext))
                 else:
-                    idList[acquisition.id] = [os.path.join(acquisition.participant.name,
-                                                           acquisition.dstId + "".join(ext))]
+                    idList[acquisition.id] = [acquisition.dstId + "".join(ext)]
 
                 for curr_post_op in post_op:
                     if acquisition.datatype in curr_post_op['datatype'] or 'any' in curr_post_op['datatype']:
                         if acquisition.suffix in curr_post_op['suffix'] or '_any' in curr_post_op['suffix']:
                             cmd = curr_post_op['cmd'].replace('src_file', str(srcFile))
                             cmd = cmd.replace('dst_file', str(dstFile))
                             run_shell_command(cmd.split())
```

### Comparing `dcm2bids-3.0/dcm2bids/dcm2niix_gen.py` & `dcm2bids-3.0rc1/dcm2bids/dcm2niix_gen.py`

 * *Files identical despite different names*

### Comparing `dcm2bids-3.0/dcm2bids/participant.py` & `dcm2bids-3.0rc1/dcm2bids/participant.py`

 * *Files identical despite different names*

### Comparing `dcm2bids-3.0/dcm2bids/sidecar.py` & `dcm2bids-3.0rc1/dcm2bids/sidecar.py`

 * *Files identical despite different names*

### Comparing `dcm2bids-3.0/dcm2bids/utils/args.py` & `dcm2bids-3.0rc1/dcm2bids/utils/args.py`

 * *Files identical despite different names*

### Comparing `dcm2bids-3.0/dcm2bids/utils/io.py` & `dcm2bids-3.0rc1/dcm2bids/utils/io.py`

 * *Files identical despite different names*

### Comparing `dcm2bids-3.0/dcm2bids/utils/logger.py` & `dcm2bids-3.0rc1/dcm2bids/utils/logger.py`

 * *Files identical despite different names*

### Comparing `dcm2bids-3.0/dcm2bids/utils/scaffold.py` & `dcm2bids-3.0rc1/dcm2bids/utils/scaffold.py`

 * *Files identical despite different names*

### Comparing `dcm2bids-3.0/dcm2bids/utils/tools.py` & `dcm2bids-3.0rc1/dcm2bids/utils/tools.py`

 * *Files identical despite different names*

### Comparing `dcm2bids-3.0/dcm2bids/utils/utils.py` & `dcm2bids-3.0rc1/dcm2bids/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dcm2bids-3.0/dcm2bids/version.py` & `dcm2bids-3.0rc1/dcm2bids/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 # Format expected by setup.py and doc/source/conf.py: string of form "X.Y.Z"
 _version_major = 3
 _version_minor = 0
 _version_micro = 0
-_version_extra = ''
+_version_extra = 'rc1'
 
 # Construct full version string from these.
 _ver = [_version_major, _version_minor]
 if _version_micro:
     _ver.append(_version_micro)
 if _version_extra:
     _ver.append(_version_extra)
```

### Comparing `dcm2bids-3.0/dcm2bids.egg-info/PKG-INFO` & `dcm2bids-3.0rc1/dcm2bids.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcm2bids
-Version: 3.0
+Version: 3.0rc1
 Summary: Reorganising NIfTI files from dcm2niix into the Brain Imaging Data Structure
 Maintainer: Arnaud Boré
 Maintainer-email: arnaud.bore@gmail.com
 License: GPLv3+
 Project-URL: Documentation, https://unfmontreal.github.io/Dcm2Bids
 Project-URL: Source Code, https://github.com/unfmontreal/Dcm2Bids
 Platform: OS Independent
@@ -91,14 +91,14 @@
 [bids]: http://bids.neuroimaging.io/
 [bids-examples]: https://github.com/bids-standard/bids-examples
 [bids-spec]: https://bids-specification.readthedocs.io/en/stable/
 [dcm2bids-doc]: https://unfmontreal.github.io/Dcm2Bids
 [dcm2bids-install]: https://unfmontreal.github.io/Dcm2Bids/latest/get-started/install/
 [dcm2bids-tutorial]: https://unfmontreal.github.io/Dcm2Bids/latest/tutorial/first-steps/#tutorial-first-steps
 [dcm2bids-advanced]: https://unfmontreal.github.io/Dcm2Bids/latest/advanced/
-[dcm2bids-upgrade]: https://unfmontreal.github.io/Dcm2Bids/dev/upgrade/
+[dcm2bids-upgrade]: https://unfmontreal.github.io/Dcm2Bids/latest/upgrade/
 [dcm2bids-issues]: https://github.com/UNFmontreal/Dcm2Bids/issues
 [dcm2niix-install]: https://github.com/rordenlab/dcm2niix#install
 [dcm2niix-github]: https://github.com/rordenlab/dcm2niix
 [neurostars]: https://neurostars.org/
 [neurostars-dcm2bids]: https://neurostars.org/tag/dcm2bids
 [dcm2bids-contributing]:  https://unfmontreal.github.io/Dcm2Bids/latest/how-to/contributing/
```

### Comparing `dcm2bids-3.0/dcm2bids.egg-info/SOURCES.txt` & `dcm2bids-3.0rc1/dcm2bids.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcm2bids-3.0/setup.py` & `dcm2bids-3.0rc1/setup.py`

 * *Files identical despite different names*

