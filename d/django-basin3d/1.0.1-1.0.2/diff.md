# Comparing `tmp/django-basin3d-1.0.1.tar.gz` & `tmp/django-basin3d-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-basin3d-1.0.1.tar", last modified: Thu Jul  6 15:27:51 2023, max compression
+gzip compressed data, was "django-basin3d-1.0.2.tar", last modified: Thu Jul 20 23:26:59 2023, max compression
```

## Comparing `django-basin3d-1.0.1.tar` & `django-basin3d-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:27:51.035828 django-basin3d-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-07-06 15:27:51.035828 django-basin3d-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:27:51.031828 django-basin3d-1.0.1/django_basin3d/
--rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    17595 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:27:51.035828 django-basin3d-1.0.1/django_basin3d/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:27:51.035828 django-basin3d-1.0.1/django_basin3d/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18926 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/synthesis/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/synthesis/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:27:51.035828 django-basin3d-1.0.1/django_basin3d/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/templatetags/str_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:27:51.035828 django-basin3d-1.0.1/django_basin3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-07-06 15:27:51.000000 django-basin3d-1.0.1/django_basin3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-06 15:27:51.000000 django-basin3d-1.0.1/django_basin3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 15:27:51.000000 django-basin3d-1.0.1/django_basin3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-06 15:27:51.000000 django-basin3d-1.0.1/django_basin3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 15:27:51.000000 django-basin3d-1.0.1/django_basin3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/doecode.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 15:27:51.035828 django-basin3d-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:26:59.245341 django-basin3d-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-07-20 23:26:59.245341 django-basin3d-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:26:59.241341 django-basin3d-1.0.2/django_basin3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/django_basin3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/django_basin3d/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/django_basin3d/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17595 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/django_basin3d/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:26:59.241341 django-basin3d-1.0.2/django_basin3d/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/django_basin3d/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/django_basin3d/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/django_basin3d/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/django_basin3d/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/django_basin3d/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:26:59.241341 django-basin3d-1.0.2/django_basin3d/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/django_basin3d/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18926 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/django_basin3d/synthesis/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13976 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/django_basin3d/synthesis/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:26:59.241341 django-basin3d-1.0.2/django_basin3d/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/django_basin3d/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/django_basin3d/templatetags/str_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/django_basin3d/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/django_basin3d/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/django_basin3d/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:26:59.241341 django-basin3d-1.0.2/django_basin3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-07-20 23:26:59.000000 django-basin3d-1.0.2/django_basin3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-20 23:26:59.000000 django-basin3d-1.0.2/django_basin3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 23:26:59.000000 django-basin3d-1.0.2/django_basin3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-20 23:26:59.000000 django-basin3d-1.0.2/django_basin3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 23:26:59.000000 django-basin3d-1.0.2/django_basin3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/doecode.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-20 23:26:48.000000 django-basin3d-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 23:26:59.245341 django-basin3d-1.0.2/setup.cfg
```

### Comparing `django-basin3d-1.0.1/LICENSE` & `django-basin3d-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.1/PKG-INFO` & `django-basin3d-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-basin3d
-Version: 1.0.1
+Version: 1.0.2
 Summary: BASIN-3D Django Web Framework
 Author-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>, Charuleka Varadharajan <cvaradharajan@lbl.gov>
 Maintainer-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>
 License: Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets (BASIN-3D) Copyright (c) 2019, The
         Regents of the University of California, through Lawrence Berkeley National
         Laboratory (subject to receipt of any required approvals from the U.S.
         Dept. of Energy).  All rights reserved.
```

### Comparing `django-basin3d-1.0.1/README.md` & `django-basin3d-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.1/django_basin3d/__init__.py` & `django-basin3d-1.0.2/django_basin3d/__init__.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.1/django_basin3d/admin.py` & `django-basin3d-1.0.2/django_basin3d/admin.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.1/django_basin3d/catalog.py` & `django-basin3d-1.0.2/django_basin3d/catalog.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.1/django_basin3d/migrations/0001_initial.py` & `django-basin3d-1.0.2/django_basin3d/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.1/django_basin3d/models.py` & `django-basin3d-1.0.2/django_basin3d/models.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.1/django_basin3d/serializers.py` & `django-basin3d-1.0.2/django_basin3d/serializers.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.1/django_basin3d/settings.py` & `django-basin3d-1.0.2/django_basin3d/settings.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.1/django_basin3d/synthesis/__init__.py` & `django-basin3d-1.0.2/django_basin3d/synthesis/__init__.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.1/django_basin3d/synthesis/serializers.py` & `django-basin3d-1.0.2/django_basin3d/synthesis/serializers.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.1/django_basin3d/synthesis/viewsets.py` & `django-basin3d-1.0.2/django_basin3d/synthesis/viewsets.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,58 +109,49 @@
             items.append(i)
 
         serializer = self.__class__.serializer_class(items, many=True, context={'request': request})
         synthesis_response = itr.synthesis_response.dict(exclude_unset=True)
         synthesis_response['data'] = serializer.data
         return Response(synthesis_response)
 
-    def retrieve(self, pk: str, **kwargs) -> Response:
+    def retrieve(self, **kwargs) -> Response:
         """
-        Retrieve a single synthesized value
+        Retrieve a single object
 
-        :param request: The request object
-        :type request: :class:`rest_framework.request.Request`
         :param pk: The primary key
         :return: The HTTP Response
         :rtype: :class:`rest_framework.request.Response`
         """
 
         request = kwargs['request']
         query = kwargs['query']
+        pk = kwargs['pk']
 
         try:
-            try:
-                itr = super(DataSourcePluginViewSet, self).list(query)
-                item = next(itr)
-            except StopIteration:
-                item = None
-                itr = None
+            item_synthesis_response = super(DataSourcePluginViewSet, self).retrieve(query)
 
-            if not item:
-                return Response({"success": False, "detail": "There is no detail for {}".format(pk)},
+            if not item_synthesis_response or not item_synthesis_response.data:
+                return Response({"success": False, "detail": f"There is no detail for {pk}"},
                                 status=status.HTTP_404_NOT_FOUND)
             else:
 
                 try:
-                    serializer = self.__class__.serializer_class(item, context={'request': request})
-                    synthesis_response = itr.synthesis_response.dict(exclude_unset=True)
+                    serializer = self.__class__.serializer_class(item_synthesis_response.data, context={'request': request})
+                    synthesis_response = item_synthesis_response.dict(exclude_unset=True)
                     synthesis_response['data'] = serializer.data
                     return Response(synthesis_response)
                 except Exception as e:
                     logger.error("Plugin error: {}".format(e))
 
-        except DataSource.DoesNotExist:
-            return Response({'success': False, 'detail': "There is no detail for datasource object {}.".format(pk)},
-                            status=status.HTTP_404_NOT_FOUND, )
         except Exception as e:
             return Response({'success': False, 'detail': str(e)},
                             status=status.HTTP_404_NOT_FOUND, )
 
 
-class MonitoringFeatureViewSet(MonitoringFeatureAccess, DataSourcePluginViewSet):
+class MonitoringFeatureViewSet(DataSourcePluginViewSet, MonitoringFeatureAccess):
     """
     MonitoringFeature: A feature upon which monitoring is made. OGC Timeseries Profile OM_MonitoringFeature.
 
     **Synthesis Response**
     This endpoint returns the following synthesis response object.
 
     ```json
@@ -209,18 +200,18 @@
     @typing.no_type_check
     def retrieve(self, request: Request, pk: str) -> Response:
         if not request:
             return Response({'success': False, 'detail': "Request is missing"},
                             status=status.HTTP_400_BAD_REQUEST, )
 
         feature_type = _get_request_feature_type(request)
-        params = request.query_params.dict()
-        return super().retrieve(request=request, pk=pk, query=QueryMonitoringFeature(monitoring_feature=[pk],
-                                                                                     feature_type=feature_type,
-                                                                                     **params))
+
+        # retrieve method order: MonitoringFeatureViewSet, DataSourceViewSet, MonitoringFeatureAccess
+        # call super force this order based on inherited class ordering
+        return super().retrieve(request=request, query=QueryMonitoringFeature(id=pk, feature_type=feature_type), pk=pk)
 
     @action(detail=True, url_name='regions-detail')
     def regions(self, request, pk=None):
         return self.retrieve(request=request, pk=pk)
 
     @action(detail=True, url_name='subregions-detail')
     def subregions(self, request, pk=None):
@@ -259,16 +250,15 @@
         return self.retrieve(request=request, pk=pk)
 
     @action(detail=True, url_name='points-detail')
     def points(self, request, pk=None):
         return self.retrieve(request=request, pk=pk)
 
 
-class MeasurementTimeseriesTVPObservationViewSet(MeasurementTimeseriesTVPObservationAccess,
-                                                 DataSourcePluginViewSet):
+class MeasurementTimeseriesTVPObservationViewSet(DataSourcePluginViewSet, MeasurementTimeseriesTVPObservationAccess):
     """
     MeasurementTimeseriesTVPObservation: Series of measurement (numerical) observations in
     TVP (time value pair) format grouped by time (i.e., a timeseries).
 
     **Synthesis Response**
     This endpoint returns the following synthesis response object.
```

### Comparing `django-basin3d-1.0.1/django_basin3d/urls.py` & `django-basin3d-1.0.2/django_basin3d/urls.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.1/django_basin3d/views.py` & `django-basin3d-1.0.2/django_basin3d/views.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.1/django_basin3d/viewsets.py` & `django-basin3d-1.0.2/django_basin3d/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.1/django_basin3d.egg-info/PKG-INFO` & `django-basin3d-1.0.2/django_basin3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-basin3d
-Version: 1.0.1
+Version: 1.0.2
 Summary: BASIN-3D Django Web Framework
 Author-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>, Charuleka Varadharajan <cvaradharajan@lbl.gov>
 Maintainer-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>
 License: Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets (BASIN-3D) Copyright (c) 2019, The
         Regents of the University of California, through Lawrence Berkeley National
         Laboratory (subject to receipt of any required approvals from the U.S.
         Dept. of Energy).  All rights reserved.
```

### Comparing `django-basin3d-1.0.1/django_basin3d.egg-info/SOURCES.txt` & `django-basin3d-1.0.2/django_basin3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.1/doecode.yml` & `django-basin3d-1.0.2/doecode.yml`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.1/pyproject.toml` & `django-basin3d-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Topic :: Scientific/Engineering :: Hydrology"
 ]
 description = "BASIN-3D Django Web Framework"
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = '>=3.8,<3.11'
 dependencies = [
-    'basin3d==0.4.1',
+    'basin3d==0.4.2',
     'django>=4.0',
     'djangorestframework',
     'django-filter',
     'markdown',
     'pygments'
 ]
```

