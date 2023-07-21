# Comparing `tmp/sintef-pyshop-1.4.3.tar.gz` & `tmp/sintef-pyshop-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sintef-pyshop-1.4.3.tar", last modified: Tue Jul 11 08:08:51 2023, max compression
+gzip compressed data, was "sintef-pyshop-1.4.4.tar", last modified: Fri Jul 21 08:03:27 2023, max compression
```

## Comparing `sintef-pyshop-1.4.3.tar` & `sintef-pyshop-1.4.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:08:51.608825 sintef-pyshop-1.4.3/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6128 2023-07-11 08:08:51.607825 sintef-pyshop-1.4.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5070 2023-07-04 11:41:21.000000 sintef-pyshop-1.4.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:08:51.576824 sintef-pyshop-1.4.3/pyshop/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.3/pyshop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:08:51.582824 sintef-pyshop-1.4.3/pyshop/helpers/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.3/pyshop/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.3/pyshop/helpers/commands.py
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.3/pyshop/helpers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     5040 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/helpers/timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/helpers/typing_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:08:51.596825 sintef-pyshop-1.4.3/pyshop/lp_model/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/lp_model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2195 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/lp_model/index.py
--rw-rw-rw-   0 root         (0) root         (0)     2555 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/lp_model/lp_model.py
--rw-rw-rw-   0 root         (0) root         (0)    10661 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/lp_model/row.py
--rw-rw-rw-   0 root         (0) root         (0)     9366 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/lp_model/var.py
--rw-rw-rw-   0 root         (0) root         (0)    13751 2023-06-08 08:57:15.000000 sintef-pyshop-1.4.3/pyshop/shop_runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:08:51.602825 sintef-pyshop-1.4.3/pyshop/shopcore/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/shopcore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2330 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/shopcore/command_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    24862 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/shopcore/model_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    13037 2023-07-11 08:08:40.000000 sintef-pyshop-1.4.3/pyshop/shopcore/script_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    15169 2023-07-11 08:08:40.000000 sintef-pyshop-1.4.3/pyshop/shopcore/shop_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1611 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/shopcore/shop_rest.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 08:08:51.608825 sintef-pyshop-1.4.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1882 2023-06-07 13:27:40.000000 sintef-pyshop-1.4.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:08:51.604825 sintef-pyshop-1.4.3/sintef_pyshop.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6128 2023-07-11 08:08:51.000000 sintef-pyshop-1.4.3/sintef_pyshop.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      790 2023-07-11 08:08:51.000000 sintef-pyshop-1.4.3/sintef_pyshop.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 08:08:51.000000 sintef-pyshop-1.4.3/sintef_pyshop.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-07-11 08:08:51.000000 sintef-pyshop-1.4.3/sintef_pyshop.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-11 08:08:51.000000 sintef-pyshop-1.4.3/sintef_pyshop.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:08:51.606825 sintef-pyshop-1.4.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)      724 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/tests/test_helpers_command.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/tests/test_helpers_time.py
--rw-rw-rw-   0 root         (0) root         (0)     8163 2023-07-05 14:05:21.000000 sintef-pyshop-1.4.3/tests/test_shop_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 08:03:27.533469 sintef-pyshop-1.4.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6128 2023-07-21 08:03:27.533469 sintef-pyshop-1.4.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5070 2023-07-05 14:04:50.000000 sintef-pyshop-1.4.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 08:03:27.527469 sintef-pyshop-1.4.4/pyshop/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.4/pyshop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 08:03:27.528469 sintef-pyshop-1.4.4/pyshop/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.4/pyshop/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.4/pyshop/helpers/commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.4/pyshop/helpers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     5040 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.4/pyshop/helpers/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.4/pyshop/helpers/typing_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 08:03:27.529469 sintef-pyshop-1.4.4/pyshop/lp_model/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.4/pyshop/lp_model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.4/pyshop/lp_model/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     2555 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.4/pyshop/lp_model/lp_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    10661 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.4/pyshop/lp_model/row.py
+-rw-rw-rw-   0 root         (0) root         (0)     9366 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.4/pyshop/lp_model/var.py
+-rw-rw-rw-   0 root         (0) root         (0)    13751 2023-06-08 08:59:06.000000 sintef-pyshop-1.4.4/pyshop/shop_runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 08:03:27.531469 sintef-pyshop-1.4.4/pyshop/shopcore/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.4/pyshop/shopcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2330 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.4/pyshop/shopcore/command_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    24862 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.4/pyshop/shopcore/model_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    13037 2023-07-11 08:08:19.000000 sintef-pyshop-1.4.4/pyshop/shopcore/script_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    15331 2023-07-21 08:02:14.000000 sintef-pyshop-1.4.4/pyshop/shopcore/shop_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1611 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.4/pyshop/shopcore/shop_rest.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 08:03:27.533469 sintef-pyshop-1.4.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1882 2023-06-07 13:14:22.000000 sintef-pyshop-1.4.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 08:03:27.532469 sintef-pyshop-1.4.4/sintef_pyshop.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6128 2023-07-21 08:03:27.000000 sintef-pyshop-1.4.4/sintef_pyshop.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      790 2023-07-21 08:03:27.000000 sintef-pyshop-1.4.4/sintef_pyshop.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 08:03:27.000000 sintef-pyshop-1.4.4/sintef_pyshop.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-21 08:03:27.000000 sintef-pyshop-1.4.4/sintef_pyshop.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-21 08:03:27.000000 sintef-pyshop-1.4.4/sintef_pyshop.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 08:03:27.532469 sintef-pyshop-1.4.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      724 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.4/tests/test_helpers_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.4/tests/test_helpers_time.py
+-rw-rw-rw-   0 root         (0) root         (0)     8163 2023-07-05 14:04:50.000000 sintef-pyshop-1.4.4/tests/test_shop_api.py
```

### Comparing `sintef-pyshop-1.4.3/LICENSE` & `sintef-pyshop-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.3/PKG-INFO` & `sintef-pyshop-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sintef-pyshop
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python interface to SHOP
 Home-page: http://www.sintef.no/programvare/SHOP
 Author: SINTEF Energy Research
 Author-email: support.energy@sintef.no
 License: MIT
 Project-URL: Documentation, https://shop.sintef.energy/documentation/tutorials/pyshop/
 Project-URL: Source, https://gitlab.sintef.no/energy/shop/pyshop
```

### Comparing `sintef-pyshop-1.4.3/README.md` & `sintef-pyshop-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.3/pyshop/helpers/commands.py` & `sintef-pyshop-1.4.4/pyshop/helpers/commands.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.3/pyshop/helpers/time.py` & `sintef-pyshop-1.4.4/pyshop/helpers/time.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.3/pyshop/helpers/timeseries.py` & `sintef-pyshop-1.4.4/pyshop/helpers/timeseries.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.3/pyshop/helpers/typing_annotations.py` & `sintef-pyshop-1.4.4/pyshop/helpers/typing_annotations.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.3/pyshop/lp_model/index.py` & `sintef-pyshop-1.4.4/pyshop/lp_model/index.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.3/pyshop/lp_model/lp_model.py` & `sintef-pyshop-1.4.4/pyshop/lp_model/lp_model.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.3/pyshop/lp_model/row.py` & `sintef-pyshop-1.4.4/pyshop/lp_model/row.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.3/pyshop/lp_model/var.py` & `sintef-pyshop-1.4.4/pyshop/lp_model/var.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.3/pyshop/shop_runner.py` & `sintef-pyshop-1.4.4/pyshop/shop_runner.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.3/pyshop/shopcore/command_builder.py` & `sintef-pyshop-1.4.4/pyshop/shopcore/command_builder.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.3/pyshop/shopcore/model_builder.py` & `sintef-pyshop-1.4.4/pyshop/shopcore/model_builder.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.3/pyshop/shopcore/script_generator.py` & `sintef-pyshop-1.4.4/pyshop/shopcore/script_generator.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.3/pyshop/shopcore/shop_api.py` & `sintef-pyshop-1.4.4/pyshop/shopcore/shop_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,21 +179,29 @@
             shop_api.SetXyCurve(object_type, object_name, attribute_name, ref, value.index.values,
                                 value.values)
         else:
             x = [x[0] for x in value['xy']]
             y = [x[1] for x in value['xy']]
             shop_api.SetXyCurve(object_type, object_name, attribute_name, value['ref'], x, y)
     elif datatype == 'sy':
+        strings = []
+        y = np.array([])
         if isinstance(value, pd.Series):
-            shop_api.SetSyCurve(object_type, object_name, attribute_name, value.index.to_list(),
-                                value.values)
+            strings = []
+            for s in value.index:
+                if isinstance(s, pd.Timestamp):
+                    s = get_shop_timestring(s)            
+                strings.append(s)
+
+            y = value.values
         else:
-            s = [s[0] for s in value['sy']]
-            y = [x[1] for x in value['sy']]
-            shop_api.SetSyCurve(object_type, object_name, attribute_name, list(s), y)
+            strings = [point[0] for point in value['sy']]
+            y = np.array([point[1] for point in value['sy']])
+
+        shop_api.SetSyCurve(object_type, object_name, attribute_name, strings, y)
     elif datatype == 'xy_array':
         if len(value) == 0:
             return
         ref = np.array([])
         x = np.array([])
         y = np.array([])
         n = np.array([])
```

### Comparing `sintef-pyshop-1.4.3/pyshop/shopcore/shop_rest.py` & `sintef-pyshop-1.4.4/pyshop/shopcore/shop_rest.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.3/setup.py` & `sintef-pyshop-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.3/sintef_pyshop.egg-info/PKG-INFO` & `sintef-pyshop-1.4.4/sintef_pyshop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sintef-pyshop
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python interface to SHOP
 Home-page: http://www.sintef.no/programvare/SHOP
 Author: SINTEF Energy Research
 Author-email: support.energy@sintef.no
 License: MIT
 Project-URL: Documentation, https://shop.sintef.energy/documentation/tutorials/pyshop/
 Project-URL: Source, https://gitlab.sintef.no/energy/shop/pyshop
```

### Comparing `sintef-pyshop-1.4.3/sintef_pyshop.egg-info/SOURCES.txt` & `sintef-pyshop-1.4.4/sintef_pyshop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.3/tests/test_helpers_command.py` & `sintef-pyshop-1.4.4/tests/test_helpers_command.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.3/tests/test_helpers_time.py` & `sintef-pyshop-1.4.4/tests/test_helpers_time.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.3/tests/test_shop_api.py` & `sintef-pyshop-1.4.4/tests/test_shop_api.py`

 * *Files identical despite different names*

