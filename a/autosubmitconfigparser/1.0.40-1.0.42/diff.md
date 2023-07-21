# Comparing `tmp/autosubmitconfigparser-1.0.40.tar.gz` & `tmp/autosubmitconfigparser-1.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosubmitconfigparser-1.0.40.tar", last modified: Fri Jul 14 13:52:50 2023, max compression
+gzip compressed data, was "autosubmitconfigparser-1.0.42.tar", last modified: Fri Jul 21 08:55:23 2023, max compression
```

## Comparing `autosubmitconfigparser-1.0.40.tar` & `autosubmitconfigparser-1.0.42.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-14 13:52:50.922066 autosubmitconfigparser-1.0.40/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       41 2023-03-03 13:49:23.000000 autosubmitconfigparser-1.0.40/MANIFEST.in
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2123 2023-07-14 13:52:50.922066 autosubmitconfigparser-1.0.40/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1493 2022-12-05 09:31:33.000000 autosubmitconfigparser-1.0.40/README.md
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-14 13:52:50.922066 autosubmitconfigparser-1.0.40/autosubmitconfigparser/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 13:48:23.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-14 13:52:50.922066 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 13:49:24.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/__init__.py
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     7990 2023-04-25 12:49:03.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/basicconfig.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   107450 2023-07-14 13:47:59.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/configcommon.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-14 13:52:50.922066 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/autosubmit-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/autosubmit.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      562 2023-02-14 09:24:09.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/expdef-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      557 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/expdef.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      401 2023-03-03 11:06:17.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/git-minimal.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/jobs-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/jobs.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      321 2023-03-03 12:26:14.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/local-minimal.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/platforms-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/platforms.yml
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      275 2023-06-07 12:06:41.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/yamlparser.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-14 13:52:50.922066 autosubmitconfigparser-1.0.40/autosubmitconfigparser.egg-info/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2123 2023-07-14 13:52:50.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser.egg-info/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1029 2023-07-14 13:52:50.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser.egg-info/SOURCES.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-07-14 13:52:50.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser.egg-info/dependency_links.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      321 2023-07-14 13:52:50.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser.egg-info/requires.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2023-07-14 13:52:50.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser.egg-info/top_level.txt
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-14 13:52:50.922066 autosubmitconfigparser-1.0.40/log/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.40/log/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.40/log/fd_show.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13106 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.40/log/log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-07-14 13:52:50.922066 autosubmitconfigparser-1.0.40/setup.cfg
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1461 2023-07-14 13:50:19.000000 autosubmitconfigparser-1.0.40/setup.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:55:23.084870 autosubmitconfigparser-1.0.42/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       41 2023-03-03 13:49:23.000000 autosubmitconfigparser-1.0.42/MANIFEST.in
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-07-21 08:55:23.084870 autosubmitconfigparser-1.0.42/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1493 2022-12-05 09:31:33.000000 autosubmitconfigparser-1.0.42/README.md
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:55:23.080870 autosubmitconfigparser-1.0.42/autosubmitconfigparser/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 13:48:23.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:55:23.084870 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 13:49:24.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/__init__.py
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     7990 2023-04-25 12:49:03.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/basicconfig.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   107552 2023-07-21 08:27:49.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/configcommon.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:55:23.084870 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/autosubmit-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/autosubmit.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      562 2023-02-14 09:24:09.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/expdef-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      557 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/expdef.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      401 2023-03-03 11:06:17.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/git-minimal.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/jobs-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/jobs.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      321 2023-03-03 12:26:14.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/local-minimal.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/platforms-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/platforms.yml
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      275 2023-06-07 12:06:41.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/yamlparser.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:55:23.084870 autosubmitconfigparser-1.0.42/autosubmitconfigparser.egg-info/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-07-21 08:55:23.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser.egg-info/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1029 2023-07-21 08:55:23.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser.egg-info/SOURCES.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-07-21 08:55:23.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser.egg-info/dependency_links.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      321 2023-07-21 08:55:23.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser.egg-info/requires.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2023-07-21 08:55:23.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser.egg-info/top_level.txt
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:55:23.084870 autosubmitconfigparser-1.0.42/log/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.42/log/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.42/log/fd_show.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13106 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.42/log/log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-07-21 08:55:23.084870 autosubmitconfigparser-1.0.42/setup.cfg
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1461 2023-07-21 08:52:24.000000 autosubmitconfigparser-1.0.42/setup.py
```

### Comparing `autosubmitconfigparser-1.0.40/PKG-INFO` & `autosubmitconfigparser-1.0.42/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: autosubmitconfigparser
-Version: 1.0.40
+Version: 1.0.42
 Summary: An utility library that allows to read an Autosubmit 4 experiment configuration.
 Home-page: https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
-License: UNKNOWN
 Keywords: climate,weather,workflow,HPC
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 
 Simple library that allows to read the data of an Autosubmit experiment.
@@ -58,9 +56,7 @@
 # This is a sample text with a placeholder expid
 
 # delete samples
 os.remove("as_sample.txt")
 os.remove("as_sample_parsed.txt")
 ```
 
-
-
```

### Comparing `autosubmitconfigparser-1.0.40/README.md` & `autosubmitconfigparser-1.0.42/README.md`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/basicconfig.py` & `autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/basicconfig.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/configcommon.py` & `autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/configcommon.py`

 * *Files 1% similar despite different names*

```diff
@@ -589,19 +589,19 @@
         Get all yaml files in a folder and return a list with the filenames
         :param yaml_folder: folder to search for yaml files
         :param ignore_minimal: ignore minimal files
         :return: list of filenames
         """
         filenames_to_load = []
         if ignore_minimal:
-            for yaml_file in [p.resolve() for p in Path(yaml_folder).glob("*") if
-                              p.suffix in {".yml", ".yaml"} and not p.name.endswith(("minimal.yml", "minimal.yaml"))]:
+            for yaml_file in sorted([p.resolve() for p in Path(yaml_folder).glob("*") if
+                              p.suffix in {".yml", ".yaml"} and not p.name.endswith(("minimal.yml", "minimal.yaml"))]):
                 filenames_to_load.append(str(yaml_file))
         else:
-            for yaml_file in [p.resolve() for p in Path(yaml_folder).glob("*") if p.suffix in {".yml", ".yaml"}]:
+            for yaml_file in sorted([p.resolve() for p in Path(yaml_folder).glob("*") if p.suffix in {".yml", ".yaml"}]):
                 filenames_to_load.append(str(yaml_file))
         return filenames_to_load
 
 
     def load_config_folder(self,current_data,yaml_folder,ignore_minimal=False):
         """
         Load a config folder and return pre and post config
@@ -645,20 +645,20 @@
             if file_to_load in self.current_loaded_files:
                 if file_to_load in self.current_loaded_files:
                     f_list = filenames_to_load["POST"]
                     f_list.remove(file_to_load)
         return filenames_to_load
 
     def unify_conf(self,current_data,new_data):
-        '''
+        """
         Unifies all configuration files into a single dictionary.
         :param current_data: dict with current configuration
         :param new_data: dict with new configuration
         :return: dict with new configuration taking priority over current configuration
-        '''
+        """
         # Basic data
         current_data = self.deep_update(current_data, new_data)
         # Parser loops in custom config
         current_data = self.deep_read_loops(current_data)
         self.dynamic_variables = list(set(self.dynamic_variables))
         self.special_dynamic_variables = list(set(self.special_dynamic_variables))
         current_data = self.deep_normalize(current_data)
@@ -773,20 +773,21 @@
             start_long = 2
         if parameters is None:
             parameters = self.deep_parameters_export(self.experiment_data)
         # Check if the parameters key provided are long(%DEFAULT.EXPID%) or short(DEFAULT[EXPID]) if it is not specified.
         if dict_keys_type is None:
             dict_keys_type = self.check_dict_keys_type(parameters)
 
-        backup_variables = dynamic_variables_
+        backup_variables = copy.deepcopy(dynamic_variables_)
         max_deep = max_deep + len(dynamic_variables_)
 
         while len(dynamic_variables_) > 0 and max_deep > 0:
             dynamic_variables = []
             for dynamic_var in dynamic_variables_:
+                value = None
                 #get value of placeholder with  name without %%
                 if dict_keys_type == "long":
                     keys = parameters.get(str(dynamic_var[0][start_long:-1]),None)
                     if keys is None:
                         keys = parameters.get(str(dynamic_var[0]), None)
                 else:
                     keys = dynamic_var[1]
@@ -815,35 +816,33 @@
                         value = None
                 else:
                     value = None
                 if value is not None:
                     if dict_keys_type == "long":
                         dict_key = parameters.get(str(dynamic_var[0]), {})
                         if len(dict_key) > 0:
-                            substituted = True
                             parameters[str(dynamic_var[0])] = value
                             if match is not (re.search(pattern, dynamic_var[1], flags=re.IGNORECASE)):
                                 dynamic_variables.append((dynamic_var[0], value))
-                        else:
-                            substituted = False
                     else:
                         parameters = self.dict_replace_value(parameters, dynamic_var[1], value)
-                        substituted = False
-                else:
-                    # This may be True instead of False
-                    substituted = False
-                if not substituted:
-                    if value is not None:
-                        dynamic_variables.append((dynamic_var[0],value))
-                    else:
-                        dynamic_variables.append(dynamic_var)
-            if in_the_end:
-                self.special_dynamic_variables = dynamic_variables
-            else:
-                self.dynamic_variables = dynamic_variables
+                if value is None:
+                    dynamic_variables.append(dynamic_var)
+                elif "%" in value:
+                    dynamic_variables.append((dynamic_var[0], value))
+            # checksum of each element
+            if len(dynamic_variables) == len(dynamic_variables_):
+                same_as_previous_step = True
+                for index,ele in enumerate(dynamic_variables):
+                    if ele[1] != dynamic_variables_[index][1]:
+                        same_as_previous_step = False
+                        break
+                if same_as_previous_step:
+                    max_deep = 0
+            dynamic_variables_ = dynamic_variables
             max_deep = max_deep - 1
         if in_the_end:
             self.special_dynamic_variables = backup_variables
             self.clean_dynamic_variables(pattern,in_the_end)
         else:
             self.dynamic_variables = backup_variables
             self.clean_dynamic_variables(pattern)
@@ -887,15 +886,15 @@
                 self.special_dynamic_variables.append((long_key+key, val))
             if key == "FOR":
                 # special case: check dynamic variables in the for loop
                 for for_sections,for_values in data[key].items():
                     if re.search(dynamic_var_pattern, str(for_values), flags=re.IGNORECASE) is not None:
                         self.dynamic_variables.append((long_key+key, str(for_values)))
                 self.data_loops.append(for_keys)
-            if isinstance(val, collections.abc.Mapping ):
+            elif isinstance(val, collections.abc.Mapping ):
                 self.deep_read_loops(data.get(key, {}),for_keys+[key],long_key=long_key+key+".")
         return data
 
 
 
 
 
@@ -1819,14 +1818,16 @@
         """
         date_list = list()
         date_value = str(self.get_section(['EXPERIMENT', 'DATELIST'],"20220401"))
         # Allows to use the old format for define a list.
         if type(date_value) is not list:
             if not date_value.startswith("["):
                 string = '[{0}]'.format(date_value)
+            else:
+                string = date_value
             split_string = nestedExpr('[', ']').parseString(string).asList()
             string_date = None
             for split in split_string[0]:
                 if type(split) is list:
                     for split_in in split:
                         if split_in.find("-") != -1:
                             numbers = split_in.split("-")
```

### Comparing `autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/expdef-dummy.yml` & `autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/expdef-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/expdef.yml` & `autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/expdef.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/jobs-dummy.yml` & `autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/jobs-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/jobs.yml` & `autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/jobs.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/platforms-dummy.yml` & `autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/platforms-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/platforms.yml` & `autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/platforms.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.40/autosubmitconfigparser.egg-info/PKG-INFO` & `autosubmitconfigparser-1.0.42/autosubmitconfigparser.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: autosubmitconfigparser
-Version: 1.0.40
+Version: 1.0.42
 Summary: An utility library that allows to read an Autosubmit 4 experiment configuration.
 Home-page: https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
-License: UNKNOWN
 Keywords: climate,weather,workflow,HPC
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 
 Simple library that allows to read the data of an Autosubmit experiment.
@@ -58,9 +56,7 @@
 # This is a sample text with a placeholder expid
 
 # delete samples
 os.remove("as_sample.txt")
 os.remove("as_sample_parsed.txt")
 ```
 
-
-
```

### Comparing `autosubmitconfigparser-1.0.40/autosubmitconfigparser.egg-info/SOURCES.txt` & `autosubmitconfigparser-1.0.42/autosubmitconfigparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.40/log/fd_show.py` & `autosubmitconfigparser-1.0.42/log/fd_show.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.40/log/log.py` & `autosubmitconfigparser-1.0.42/log/log.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.40/setup.py` & `autosubmitconfigparser-1.0.42/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autosubmitconfigparser",
-    version="1.0.40",
+    version="1.0.42",
     author="Daniel Beltran Mora",
     author_email="daniel.beltran@bsc.es",
     description="An utility library that allows to read an Autosubmit 4 experiment configuration.",
     keywords=['climate', 'weather', 'workflow', 'HPC'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git",
```

