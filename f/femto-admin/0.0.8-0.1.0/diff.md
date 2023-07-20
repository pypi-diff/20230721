# Comparing `tmp/femto-admin-0.0.8.tar.gz` & `tmp/femto-admin-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femto-admin-0.0.8.tar", last modified: Thu Jul 20 19:04:20 2023, max compression
+gzip compressed data, was "femto-admin-0.1.0.tar", last modified: Thu Jul 20 23:53:22 2023, max compression
```

## Comparing `femto-admin-0.0.8.tar` & `femto-admin-0.1.0.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 19:04:20.137082 femto-admin-0.0.8/
--rw-r--r--   0 sol        (501) staff       (20)       17 2023-07-20 14:49:50.000000 femto-admin-0.0.8/MANIFEST.in
--rw-r--r--   0 sol        (501) staff       (20)      256 2023-07-20 19:04:20.136813 femto-admin-0.0.8/PKG-INFO
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 19:04:20.114498 femto-admin-0.0.8/femto_admin/
--rw-r--r--   0 sol        (501) staff       (20)       36 2023-07-20 11:43:08.000000 femto-admin-0.0.8/femto_admin/__init__.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 19:04:20.117583 femto-admin-0.0.8/femto_admin/__pycache__/
--rw-r--r--   0 sol        (501) staff       (20)      220 2023-07-20 14:50:39.000000 femto-admin-0.0.8/femto_admin/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 sol        (501) staff       (20)     4981 2023-07-20 15:03:22.000000 femto-admin-0.0.8/femto_admin/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0 sol        (501) staff       (20)     1314 2023-07-13 11:06:49.000000 femto-admin-0.0.8/femto_admin/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 sol        (501) staff       (20)     2716 2023-07-20 15:18:42.000000 femto-admin-0.0.8/femto_admin/admin.py
--rw-r--r--   0 sol        (501) staff       (20)      193 2023-07-19 16:49:12.000000 femto-admin-0.0.8/femto_admin/consts.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 19:04:20.111229 femto-admin-0.0.8/femto_admin/statics/
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 19:04:20.118127 femto-admin-0.0.8/femto_admin/statics/placeholders/
--rw-r--r--   0 sol        (501) staff       (20)    16958 2023-06-23 13:05:44.000000 femto-admin-0.0.8/femto_admin/statics/placeholders/favicon.ico
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 19:04:20.118564 femto-admin-0.0.8/femto_admin/statics/placeholders/logo/
--rw-r--r--   0 sol        (501) staff       (20)      418 2023-06-23 17:08:58.000000 femto-admin-0.0.8/femto_admin/statics/placeholders/logo/logo-white.svg
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 19:04:20.119083 femto-admin-0.0.8/femto_admin/statics/placeholders/users/
--rw-r--r--   0 sol        (501) staff       (20)     2094 2023-05-04 14:33:48.000000 femto-admin-0.0.8/femto_admin/statics/placeholders/users/admin.jpg
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 19:04:20.111705 femto-admin-0.0.8/femto_admin/statics/vendor/
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 19:04:20.111506 femto-admin-0.0.8/femto_admin/statics/vendor/DataTables/
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 19:04:20.120188 femto-admin-0.0.8/femto_admin/statics/vendor/DataTables/css/
--rw-r--r--   0 sol        (501) staff       (20)    13550 2023-07-04 13:18:30.000000 femto-admin-0.0.8/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.css
--rw-r--r--   0 sol        (501) staff       (20)    11981 2023-07-04 13:18:30.000000 femto-admin-0.0.8/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.min.css
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 19:04:20.123630 femto-admin-0.0.8/femto_admin/statics/vendor/DataTables/js/
--rw-r--r--   0 sol        (501) staff       (20)     5265 2023-07-04 13:18:32.000000 femto-admin-0.0.8/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.js
--rw-r--r--   0 sol        (501) staff       (20)     2353 2023-07-04 13:18:32.000000 femto-admin-0.0.8/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.min.js
--rw-r--r--   0 sol        (501) staff       (20)   457166 2023-07-04 13:18:32.000000 femto-admin-0.0.8/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.js
--rw-r--r--   0 sol        (501) staff       (20)    87093 2023-07-04 13:18:32.000000 femto-admin-0.0.8/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.min.js
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 19:04:20.125966 femto-admin-0.0.8/femto_admin/statics/vendor/jQuery/
--rw-r--r--   0 sol        (501) staff       (20)   284996 2023-07-04 13:23:04.000000 femto-admin-0.0.8/femto_admin/statics/vendor/jQuery/jquery.js
--rw-r--r--   0 sol        (501) staff       (20)    87462 2023-07-04 13:23:04.000000 femto-admin-0.0.8/femto_admin/statics/vendor/jQuery/jquery.min.js
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 19:04:20.111858 femto-admin-0.0.8/femto_admin/statics/vendor/tabler/
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 19:04:20.128979 femto-admin-0.0.8/femto_admin/statics/vendor/tabler/css/
--rw-r--r--   0 sol        (501) staff       (20)   642443 2023-05-16 21:47:00.000000 femto-admin-0.0.8/femto_admin/statics/vendor/tabler/css/tabler.css
--rw-r--r--   0 sol        (501) staff       (20)   542559 2023-05-16 21:47:00.000000 femto-admin-0.0.8/femto_admin/statics/vendor/tabler/css/tabler.min.css
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 19:04:20.133706 femto-admin-0.0.8/femto_admin/statics/vendor/tabler/js/
--rw-r--r--   0 sol        (501) staff       (20)     1053 2023-07-19 10:42:04.000000 femto-admin-0.0.8/femto_admin/statics/vendor/tabler/js/dark-theme.js
--rw-r--r--   0 sol        (501) staff       (20)      679 2023-05-16 21:47:00.000000 femto-admin-0.0.8/femto_admin/statics/vendor/tabler/js/dark-theme.min.js
--rw-r--r--   0 sol        (501) staff       (20)   265501 2023-05-16 21:47:00.000000 femto-admin-0.0.8/femto_admin/statics/vendor/tabler/js/tabler.js
--rw-r--r--   0 sol        (501) staff       (20)   136567 2023-05-16 21:47:00.000000 femto-admin-0.0.8/femto_admin/statics/vendor/tabler/js/tabler.min.js
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 19:04:20.136201 femto-admin-0.0.8/femto_admin/templates/
--rw-r--r--   0 sol        (501) staff       (20)       27 2023-07-20 15:06:51.000000 femto-admin-0.0.8/femto_admin/templates/dashboard.html
--rw-r--r--   0 sol        (501) staff       (20)    26017 2023-07-20 14:57:19.000000 femto-admin-0.0.8/femto_admin/templates/layout.html
--rw-r--r--   0 sol        (501) staff       (20)        0 2023-07-18 09:39:11.000000 femto-admin-0.0.8/femto_admin/templates/modal.html
--rw-r--r--   0 sol        (501) staff       (20)      786 2023-07-20 14:58:28.000000 femto-admin-0.0.8/femto_admin/templates/table.html
--rw-r--r--   0 sol        (501) staff       (20)     2213 2023-07-19 23:37:52.000000 femto-admin-0.0.8/femto_admin/utils.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 19:04:20.115969 femto-admin-0.0.8/femto_admin.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)      256 2023-07-20 19:04:20.000000 femto-admin-0.0.8/femto_admin.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)     1515 2023-07-20 19:04:20.000000 femto-admin-0.0.8/femto_admin.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-20 19:04:20.000000 femto-admin-0.0.8/femto_admin.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       27 2023-07-20 19:04:20.000000 femto-admin-0.0.8/femto_admin.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       12 2023-07-20 19:04:20.000000 femto-admin-0.0.8/femto_admin.egg-info/top_level.txt
--rw-r--r--   0 sol        (501) staff       (20)      381 2023-07-20 19:03:13.000000 femto-admin-0.0.8/pyproject.toml
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-20 19:04:20.137147 femto-admin-0.0.8/setup.cfg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.167400 femto-admin-0.1.0/
+-rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 femto-admin-0.1.0/LICENSE
+-rw-r--r--   0 sol        (501) staff       (20)       17 2023-07-20 14:49:50.000000 femto-admin-0.1.0/MANIFEST.in
+-rw-r--r--   0 sol        (501) staff       (20)     2062 2023-07-20 23:53:22.167163 femto-admin-0.1.0/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)     1499 2023-07-20 23:49:02.000000 femto-admin-0.1.0/README.md
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.139828 femto-admin-0.1.0/femto_admin/
+-rw-r--r--   0 sol        (501) staff       (20)       36 2023-07-20 11:43:08.000000 femto-admin-0.1.0/femto_admin/__init__.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.142997 femto-admin-0.1.0/femto_admin/__pycache__/
+-rw-r--r--   0 sol        (501) staff       (20)      220 2023-07-20 14:50:39.000000 femto-admin-0.1.0/femto_admin/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 sol        (501) staff       (20)     7092 2023-07-20 23:07:29.000000 femto-admin-0.1.0/femto_admin/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0 sol        (501) staff       (20)     1314 2023-07-13 11:06:49.000000 femto-admin-0.1.0/femto_admin/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 sol        (501) staff       (20)     3335 2023-07-20 23:06:46.000000 femto-admin-0.1.0/femto_admin/admin.py
+-rw-r--r--   0 sol        (501) staff       (20)      193 2023-07-19 16:49:12.000000 femto-admin-0.1.0/femto_admin/consts.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.135776 femto-admin-0.1.0/femto_admin/statics/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.143571 femto-admin-0.1.0/femto_admin/statics/placeholders/
+-rw-r--r--   0 sol        (501) staff       (20)    16958 2023-06-23 13:05:44.000000 femto-admin-0.1.0/femto_admin/statics/placeholders/favicon.ico
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.144709 femto-admin-0.1.0/femto_admin/statics/placeholders/logo/
+-rw-r--r--   0 sol        (501) staff       (20)      418 2023-06-23 17:08:58.000000 femto-admin-0.1.0/femto_admin/statics/placeholders/logo/logo-white.svg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.145305 femto-admin-0.1.0/femto_admin/statics/placeholders/users/
+-rw-r--r--   0 sol        (501) staff       (20)     2094 2023-05-04 14:33:48.000000 femto-admin-0.1.0/femto_admin/statics/placeholders/users/admin.jpg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.136268 femto-admin-0.1.0/femto_admin/statics/vendor/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.136045 femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.146448 femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/css/
+-rw-r--r--   0 sol        (501) staff       (20)    13550 2023-07-04 13:18:30.000000 femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.css
+-rw-r--r--   0 sol        (501) staff       (20)    11981 2023-07-04 13:18:30.000000 femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.min.css
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.150565 femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/js/
+-rw-r--r--   0 sol        (501) staff       (20)     5265 2023-07-04 13:18:32.000000 femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.js
+-rw-r--r--   0 sol        (501) staff       (20)     2353 2023-07-04 13:18:32.000000 femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.min.js
+-rw-r--r--   0 sol        (501) staff       (20)   457166 2023-07-04 13:18:32.000000 femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.js
+-rw-r--r--   0 sol        (501) staff       (20)    87093 2023-07-04 13:18:32.000000 femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.min.js
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.154156 femto-admin-0.1.0/femto_admin/statics/vendor/jQuery/
+-rw-r--r--   0 sol        (501) staff       (20)   284996 2023-07-04 13:23:04.000000 femto-admin-0.1.0/femto_admin/statics/vendor/jQuery/jquery.js
+-rw-r--r--   0 sol        (501) staff       (20)    87462 2023-07-04 13:23:04.000000 femto-admin-0.1.0/femto_admin/statics/vendor/jQuery/jquery.min.js
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.136463 femto-admin-0.1.0/femto_admin/statics/vendor/tabler/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.158036 femto-admin-0.1.0/femto_admin/statics/vendor/tabler/css/
+-rw-r--r--   0 sol        (501) staff       (20)   642443 2023-05-16 21:47:00.000000 femto-admin-0.1.0/femto_admin/statics/vendor/tabler/css/tabler.css
+-rw-r--r--   0 sol        (501) staff       (20)   542559 2023-05-16 21:47:00.000000 femto-admin-0.1.0/femto_admin/statics/vendor/tabler/css/tabler.min.css
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.163921 femto-admin-0.1.0/femto_admin/statics/vendor/tabler/js/
+-rw-r--r--   0 sol        (501) staff       (20)     1053 2023-07-19 10:42:04.000000 femto-admin-0.1.0/femto_admin/statics/vendor/tabler/js/dark-theme.js
+-rw-r--r--   0 sol        (501) staff       (20)      679 2023-05-16 21:47:00.000000 femto-admin-0.1.0/femto_admin/statics/vendor/tabler/js/dark-theme.min.js
+-rw-r--r--   0 sol        (501) staff       (20)   265501 2023-05-16 21:47:00.000000 femto-admin-0.1.0/femto_admin/statics/vendor/tabler/js/tabler.js
+-rw-r--r--   0 sol        (501) staff       (20)   136567 2023-05-16 21:47:00.000000 femto-admin-0.1.0/femto_admin/statics/vendor/tabler/js/tabler.min.js
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.166876 femto-admin-0.1.0/femto_admin/templates/
+-rw-r--r--   0 sol        (501) staff       (20)       27 2023-07-20 15:06:51.000000 femto-admin-0.1.0/femto_admin/templates/dashboard.html
+-rw-r--r--   0 sol        (501) staff       (20)    26017 2023-07-20 14:57:19.000000 femto-admin-0.1.0/femto_admin/templates/layout.html
+-rw-r--r--   0 sol        (501) staff       (20)        0 2023-07-18 09:39:11.000000 femto-admin-0.1.0/femto_admin/templates/modal.html
+-rw-r--r--   0 sol        (501) staff       (20)      816 2023-07-20 20:27:40.000000 femto-admin-0.1.0/femto_admin/templates/table.html
+-rw-r--r--   0 sol        (501) staff       (20)     2183 2023-07-20 21:10:39.000000 femto-admin-0.1.0/femto_admin/utils.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.140989 femto-admin-0.1.0/femto_admin.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)     2062 2023-07-20 23:53:22.000000 femto-admin-0.1.0/femto_admin.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)     1533 2023-07-20 23:53:22.000000 femto-admin-0.1.0/femto_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-20 23:53:22.000000 femto-admin-0.1.0/femto_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       27 2023-07-20 23:53:22.000000 femto-admin-0.1.0/femto_admin.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       12 2023-07-20 23:53:22.000000 femto-admin-0.1.0/femto_admin.egg-info/top_level.txt
+-rw-r--r--   0 sol        (501) staff       (20)      691 2023-07-20 23:40:54.000000 femto-admin-0.1.0/pyproject.toml
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-20 23:53:22.167472 femto-admin-0.1.0/setup.cfg
```

### Comparing `femto-admin-0.0.8/femto_admin/__pycache__/utils.cpython-311.pyc` & `femto-admin-0.1.0/femto_admin/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `femto-admin-0.0.8/femto_admin/admin.py` & `femto-admin-0.1.0/femto_admin/admin.py`

 * *Files 20% similar despite different names*

```diff
@@ -54,15 +54,27 @@
 
     async def index(self, request: Request):
         model: Model = self._get_model(request)
         return self.templates.TemplateResponse("table.html", {
             'title': model.__name__,
             'subtitle': model._meta.table_description,
             'request': request,
-            'fields': model._meta.fields_map
+            'fields': {k: v for k, v in model._meta.fields_map.items() if not k.endswith('_id')}
         })
 
     async def dt(self, request: Request):
+        def render(dct: dict):
+            def rel(val: dict):
+                return f'<a class="m-1 py-1 px-2 badge bg-blue-lt lead" href="/{val["type"]}/{val["id"]}">{val["repr"]}</a>'
+            def check(val):
+                if isinstance(val, dict) and 'repr' in val.keys():
+                    return rel(val)
+                elif isinstance(val, list) and val and isinstance(val[0], dict) and 'repr' in val[0].keys():
+                    return ' '.join(rel(v) for v in val)
+                return val
+
+            return [check(val) for key, val in dct.items()]
+
         model: Model = self._get_model(request)
         objects: [Model] = await model.all().prefetch_related(*model._meta.fetch_fields)
-        data = [list(jsonify(obj).values()) for obj in objects]
+        data = [render(jsonify(obj)) for obj in objects]
         return JSONResponse({'data': data})
```

### Comparing `femto-admin-0.0.8/femto_admin/statics/placeholders/favicon.ico` & `femto-admin-0.1.0/femto_admin/statics/placeholders/favicon.ico`

 * *Files identical despite different names*

### Comparing `femto-admin-0.0.8/femto_admin/statics/placeholders/users/admin.jpg` & `femto-admin-0.1.0/femto_admin/statics/placeholders/users/admin.jpg`

 * *Files identical despite different names*

### Comparing `femto-admin-0.0.8/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.css` & `femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `femto-admin-0.0.8/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.min.css` & `femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.min.css`

 * *Files identical despite different names*

### Comparing `femto-admin-0.0.8/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.js` & `femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.0.8/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.min.js` & `femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.0.8/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.js` & `femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.0.8/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.min.js` & `femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.0.8/femto_admin/statics/vendor/jQuery/jquery.js` & `femto-admin-0.1.0/femto_admin/statics/vendor/jQuery/jquery.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.0.8/femto_admin/statics/vendor/jQuery/jquery.min.js` & `femto-admin-0.1.0/femto_admin/statics/vendor/jQuery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.0.8/femto_admin/statics/vendor/tabler/css/tabler.css` & `femto-admin-0.1.0/femto_admin/statics/vendor/tabler/css/tabler.css`

 * *Files identical despite different names*

### Comparing `femto-admin-0.0.8/femto_admin/statics/vendor/tabler/css/tabler.min.css` & `femto-admin-0.1.0/femto_admin/statics/vendor/tabler/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `femto-admin-0.0.8/femto_admin/statics/vendor/tabler/js/dark-theme.js` & `femto-admin-0.1.0/femto_admin/statics/vendor/tabler/js/dark-theme.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.0.8/femto_admin/statics/vendor/tabler/js/dark-theme.min.js` & `femto-admin-0.1.0/femto_admin/statics/vendor/tabler/js/dark-theme.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.0.8/femto_admin/statics/vendor/tabler/js/tabler.js` & `femto-admin-0.1.0/femto_admin/statics/vendor/tabler/js/tabler.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.0.8/femto_admin/statics/vendor/tabler/js/tabler.min.js` & `femto-admin-0.1.0/femto_admin/statics/vendor/tabler/js/tabler.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.0.8/femto_admin/templates/layout.html` & `femto-admin-0.1.0/femto_admin/templates/layout.html`

 * *Files identical despite different names*

### Comparing `femto-admin-0.0.8/femto_admin/templates/table.html` & `femto-admin-0.1.0/femto_admin/templates/table.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% extends "layout.html" %}
 
 {% block styles %}
-    <link href="{{ url_for('public', path='vendor/DataTables/css/dataTables.bootstrap5.css') }}" rel="stylesheet"/>
+    <link href="{{ url_for('public', path='vendor/DataTables/css/dataTables.bootstrap5.'+minify+'css') }}" rel="stylesheet"/>
 {% endblock %}
 
 {% block body %}
     <table id="dt" class="table table-striped" style="width:100%">
         <thead>
         <tr>
             {% for field in fields %}
@@ -13,11 +13,11 @@
             {% endfor %}
         </tr>
         </thead>
     </table>
 {% endblock %}
 
 {% block scripts %}
-    <script src="{{ url_for('public', path='vendor/DataTables/js/jquery.dataTables.js') }}"></script>
-    <script src="{{ url_for('public', path='vendor/DataTables/js/dataTables.bootstrap5.js') }}"></script>
+    <script src="{{ url_for('public', path='vendor/DataTables/js/jquery.dataTables.'+minify+'js') }}"></script>
+    <script src="{{ url_for('public', path='vendor/DataTables/js/dataTables.bootstrap5.'+minify+'js') }}"></script>
     <script>new DataTable('#dt', {ajax: 'dt/{{ request.path_params["model"] }}'})</script>
 {% endblock %}
```

### Comparing `femto-admin-0.0.8/femto_admin/utils.py` & `femto-admin-0.1.0/femto_admin/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from datetime import datetime
 from tortoise import Model
 from tortoise.fields.data import IntEnumFieldInstance, CharEnumField
 from tortoise.fields.relational import BackwardFKRelation, ForeignKeyFieldInstance, ManyToManyFieldInstance
 from tortoise.fields import Field, CharField, IntField, SmallIntField, BigIntField, DecimalField as DecField, \
     FloatField as FlotField, TextField, BooleanField as BoolField, DatetimeField, DateField as DatField, \
     TimeField as TimField, JSONField as JsonField, OneToOneField, ForeignKeyRelation, OneToOneRelation, \
     ManyToManyRelation, ForeignKeyNullableRelation, OneToOneNullableRelation
```

### Comparing `femto-admin-0.0.8/femto_admin.egg-info/SOURCES.txt` & `femto-admin-0.1.0/femto_admin.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+LICENSE
 MANIFEST.in
+README.md
 pyproject.toml
 femto_admin/__init__.py
 femto_admin/admin.py
 femto_admin/consts.py
 femto_admin/utils.py
 femto_admin.egg-info/PKG-INFO
 femto_admin.egg-info/SOURCES.txt
```

