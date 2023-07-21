# Comparing `tmp/django-basin3d-1.0.3.tar.gz` & `tmp/django-basin3d-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-basin3d-1.0.3.tar", last modified: Fri Jul 21 14:20:30 2023, max compression
+gzip compressed data, was "django-basin3d-1.0.4.tar", last modified: Fri Jul 21 19:29:56 2023, max compression
```

## Comparing `django-basin3d-1.0.3.tar` & `django-basin3d-1.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:20:30.894257 django-basin3d-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-07-21 14:20:30.894257 django-basin3d-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:20:30.894257 django-basin3d-1.0.3/django_basin3d/
--rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/django_basin3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/django_basin3d/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/django_basin3d/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    17595 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/django_basin3d/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:20:30.894257 django-basin3d-1.0.3/django_basin3d/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/django_basin3d/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/django_basin3d/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/django_basin3d/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/django_basin3d/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/django_basin3d/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:20:30.894257 django-basin3d-1.0.3/django_basin3d/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/django_basin3d/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18926 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/django_basin3d/synthesis/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14037 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/django_basin3d/synthesis/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:20:30.894257 django-basin3d-1.0.3/django_basin3d/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/django_basin3d/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/django_basin3d/templatetags/str_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/django_basin3d/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/django_basin3d/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/django_basin3d/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:20:30.894257 django-basin3d-1.0.3/django_basin3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-07-21 14:20:30.000000 django-basin3d-1.0.3/django_basin3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-21 14:20:30.000000 django-basin3d-1.0.3/django_basin3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:20:30.000000 django-basin3d-1.0.3/django_basin3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-21 14:20:30.000000 django-basin3d-1.0.3/django_basin3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 14:20:30.000000 django-basin3d-1.0.3/django_basin3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/doecode.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-21 14:20:19.000000 django-basin3d-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 14:20:30.894257 django-basin3d-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:29:56.653145 django-basin3d-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-07-21 19:29:56.649145 django-basin3d-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:29:56.649145 django-basin3d-1.0.4/django_basin3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/django_basin3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/django_basin3d/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/django_basin3d/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17595 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/django_basin3d/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:29:56.649145 django-basin3d-1.0.4/django_basin3d/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/django_basin3d/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/django_basin3d/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/django_basin3d/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/django_basin3d/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/django_basin3d/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:29:56.649145 django-basin3d-1.0.4/django_basin3d/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/django_basin3d/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18926 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/django_basin3d/synthesis/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/django_basin3d/synthesis/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:29:56.649145 django-basin3d-1.0.4/django_basin3d/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/django_basin3d/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/django_basin3d/templatetags/str_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/django_basin3d/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/django_basin3d/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/django_basin3d/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:29:56.649145 django-basin3d-1.0.4/django_basin3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-07-21 19:29:56.000000 django-basin3d-1.0.4/django_basin3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-21 19:29:56.000000 django-basin3d-1.0.4/django_basin3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:29:56.000000 django-basin3d-1.0.4/django_basin3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-21 19:29:56.000000 django-basin3d-1.0.4/django_basin3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 19:29:56.000000 django-basin3d-1.0.4/django_basin3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/doecode.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-21 19:29:43.000000 django-basin3d-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 19:29:56.653145 django-basin3d-1.0.4/setup.cfg
```

### Comparing `django-basin3d-1.0.3/LICENSE` & `django-basin3d-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.3/PKG-INFO` & `django-basin3d-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-basin3d
-Version: 1.0.3
+Version: 1.0.4
 Summary: BASIN-3D Django Web Framework
 Author-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>, Charuleka Varadharajan <cvaradharajan@lbl.gov>
 Maintainer-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>
 License: Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets (BASIN-3D) Copyright (c) 2019, The
         Regents of the University of California, through Lawrence Berkeley National
         Laboratory (subject to receipt of any required approvals from the U.S.
         Dept. of Energy).  All rights reserved.
```

### Comparing `django-basin3d-1.0.3/README.md` & `django-basin3d-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.3/django_basin3d/__init__.py` & `django-basin3d-1.0.4/django_basin3d/__init__.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.3/django_basin3d/admin.py` & `django-basin3d-1.0.4/django_basin3d/admin.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.3/django_basin3d/catalog.py` & `django-basin3d-1.0.4/django_basin3d/catalog.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.3/django_basin3d/migrations/0001_initial.py` & `django-basin3d-1.0.4/django_basin3d/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.3/django_basin3d/models.py` & `django-basin3d-1.0.4/django_basin3d/models.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.3/django_basin3d/serializers.py` & `django-basin3d-1.0.4/django_basin3d/serializers.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.3/django_basin3d/settings.py` & `django-basin3d-1.0.4/django_basin3d/settings.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.3/django_basin3d/synthesis/__init__.py` & `django-basin3d-1.0.4/django_basin3d/synthesis/__init__.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.3/django_basin3d/synthesis/serializers.py` & `django-basin3d-1.0.4/django_basin3d/synthesis/serializers.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.3/django_basin3d/synthesis/viewsets.py` & `django-basin3d-1.0.4/django_basin3d/synthesis/viewsets.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     Return the feature type if exists in the request
     :param request: request
     otherwise return the text version
     :return: the feature_type in the format specified, None if none exists
     """
     for feature_type in FeatureTypeEnum.values():
         urlpath = request.path_info
-        url_feature_type = ''.join(feature_type.lower().split())
+        url_feature_type = ''.join(feature_type.lower().split('_'))
         if f'{url_feature_type}s' in urlpath.split('/'):
             return feature_type
     return None
 
 
 def _convert_str_params_to_list(params: dict, query_class) -> dict:
     """
```

### Comparing `django-basin3d-1.0.3/django_basin3d/urls.py` & `django-basin3d-1.0.4/django_basin3d/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             plugin_views = plugin.get_plugin_access()
             for model_name in plugin_views.keys():
                 viewset_models.append(model_name.__name__)
 
             datasource_feature_types = plugin.get_feature_types()
             for feature_type in datasource_feature_types:
                 if feature_type in supported_feature_types:
-                    ft = ''.join(feature_type.lower().split())
+                    ft = ''.join(feature_type.lower().split('_'))
                     path_route = '^monitoringfeature/{}s'.format(ft)
                     urls.extend([
                         re_path(r'{}/$'.format(path_route),
                                 MonitoringFeatureViewSet.as_view({'get': 'list'}),
                                 name='monitoringfeature-list'),
                         re_path(r'{}\.(?P<format>[a-z0-9]+)/?$'.format(path_route),
                                 MonitoringFeatureViewSet.as_view({'get': 'list'}),
```

### Comparing `django-basin3d-1.0.3/django_basin3d/views.py` & `django-basin3d-1.0.4/django_basin3d/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         for model_name in plugin_views.keys():
             viewset_models.append(model_name.__name__)
 
         datasource_feature_types = plugin.get_feature_types()
         unsupported_feature_types = []
         for feature_type in datasource_feature_types:
             if feature_type in supported_feature_types:
-                ft = ''.join(feature_type.lower().split())
+                ft = ''.join(feature_type.lower().split('_'))
                 if ft not in monitoring_features_list.keys():
                     monitoring_features_list['{}s'.format(ft)] = \
                         '{}://{}/monitoringfeature/{}s/'.format(
                         request.scheme, request.get_host(), ft)
             elif feature_type not in unsupported_feature_types:
                 unsupported_feature_types.append(feature_type)
```

### Comparing `django-basin3d-1.0.3/django_basin3d/viewsets.py` & `django-basin3d-1.0.4/django_basin3d/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.3/django_basin3d.egg-info/PKG-INFO` & `django-basin3d-1.0.4/django_basin3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-basin3d
-Version: 1.0.3
+Version: 1.0.4
 Summary: BASIN-3D Django Web Framework
 Author-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>, Charuleka Varadharajan <cvaradharajan@lbl.gov>
 Maintainer-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>
 License: Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets (BASIN-3D) Copyright (c) 2019, The
         Regents of the University of California, through Lawrence Berkeley National
         Laboratory (subject to receipt of any required approvals from the U.S.
         Dept. of Energy).  All rights reserved.
```

### Comparing `django-basin3d-1.0.3/django_basin3d.egg-info/SOURCES.txt` & `django-basin3d-1.0.4/django_basin3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.3/doecode.yml` & `django-basin3d-1.0.4/doecode.yml`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.3/pyproject.toml` & `django-basin3d-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Topic :: Scientific/Engineering :: Hydrology"
 ]
 description = "BASIN-3D Django Web Framework"
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = '>=3.8,<3.11'
 dependencies = [
-    'basin3d==0.4.2',
+    'basin3d==0.4.3',
     'django>=4.0',
     'djangorestframework',
     'django-filter',
     'markdown',
     'pygments'
 ]
```

