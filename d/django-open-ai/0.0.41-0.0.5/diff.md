# Comparing `tmp/django-open-ai-0.0.41.tar.gz` & `tmp/django-open-ai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-open-ai-0.0.41.tar", last modified: Fri Jul 21 12:29:30 2023, max compression
+gzip compressed data, was "django-open-ai-0.0.5.tar", last modified: Fri Jul 21 12:35:57 2023, max compression
```

## Comparing `django-open-ai-0.0.41.tar` & `django-open-ai-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:30.217195 django-open-ai-0.0.41/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-21 12:29:30.217195 django-open-ai-0.0.41/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:30.217195 django-open-ai-0.0.41/django_open_ai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:30.217195 django-open-ai-0.0.41/django_open_ai/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:30.217195 django-open-ai-0.0.41/django_open_ai/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:30.217195 django-open-ai-0.0.41/django_open_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-21 12:29:30.000000 django-open-ai-0.0.41/django_open_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-21 12:29:30.000000 django-open-ai-0.0.41/django_open_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:29:30.000000 django-open-ai-0.0.41/django_open_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-21 12:29:30.000000 django-open-ai-0.0.41/django_open_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 12:29:30.000000 django-open-ai-0.0.41/django_open_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-21 12:29:30.217195 django-open-ai-0.0.41/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:35:57.144065 django-open-ai-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-21 12:35:57.144065 django-open-ai-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:35:57.144065 django-open-ai-0.0.5/django_open_ai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:35:57.144065 django-open-ai-0.0.5/django_open_ai/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:35:57.144065 django-open-ai-0.0.5/django_open_ai/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:35:57.144065 django-open-ai-0.0.5/django_open_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-21 12:35:57.000000 django-open-ai-0.0.5/django_open_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-21 12:35:57.000000 django-open-ai-0.0.5/django_open_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:35:57.000000 django-open-ai-0.0.5/django_open_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-21 12:35:57.000000 django-open-ai-0.0.5/django_open_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 12:35:57.000000 django-open-ai-0.0.5/django_open_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-21 12:35:57.144065 django-open-ai-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/setup.py
```

### Comparing `django-open-ai-0.0.41/LICENSE` & `django-open-ai-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-open-ai-0.0.41/PKG-INFO` & `django-open-ai-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-open-ai
-Version: 0.0.41
+Version: 0.0.5
 Summary: Use the power of OpenAI on your Django database
 Home-page: https://github.com/PMCS64/django-open-ai
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-open-ai-0.0.41/django_open_ai/helper.py` & `django-open-ai-0.0.5/django_open_ai/helper.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,16 +20,14 @@
         if getter:
             return connections.databases[self.database][getter]
         return connections.databases[self.database]
 
     def engage(self):
         engine = self.cursor("ENGINE")
 
-        print(self.cursor("OPTIONS"))
-
         if engine == "django.db.backends.mysql":
             self.starter = "mysql+pymysql"
             self.query = self.cursor("OPTIONS")
 
         elif engine == "django.db.backends.postgresql":
             self.starter = "postgres"
             self.query = self.cursor("OPTIONS")
@@ -37,19 +35,21 @@
         elif engine == "django.db.backends.oracle":
             self.starter = "oracle+cx_oracle"
             self.query = self.cursor("OPTIONS")
 
         elif engine == "mssql":
             self.starter = "mssql+pyodbc"
             query = self.cursor("OPTIONS")
-            if "extra_params" in self.cursor("OPTIONS").keys():
-                query.pop("extra_params")
-                key_value_pairs = self.cursor("OPTIONS")["extra_params"].strip(";").split(";")
-                query.update({kv.split("=")[0]: kv.split("=")[1] for kv in key_value_pairs})
-            self.query = query
+            new_query = {}
+            if "extra_params" in query.keys():
+                key_value_pairs = query["extra_params"].strip(";").split(";")
+                new_query.update({kv.split("=")[0]: kv.split("=")[1] for kv in key_value_pairs})
+            query.pop("extra_params")
+            new_query.update(query)
+            self.query = new_query
 
         else:
             raise Exception("The database engine {} is not yet supported.".format(engine))
 
     def connection_uri(self):
         return URL.create(
                 self.starter,
```

### Comparing `django-open-ai-0.0.41/django_open_ai/views.py` & `django-open-ai-0.0.5/django_open_ai/views.py`

 * *Files identical despite different names*

### Comparing `django-open-ai-0.0.41/django_open_ai.egg-info/PKG-INFO` & `django-open-ai-0.0.5/django_open_ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-open-ai
-Version: 0.0.41
+Version: 0.0.5
 Summary: Use the power of OpenAI on your Django database
 Home-page: https://github.com/PMCS64/django-open-ai
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-open-ai-0.0.41/django_open_ai.egg-info/SOURCES.txt` & `django-open-ai-0.0.5/django_open_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-open-ai-0.0.41/setup.cfg` & `django-open-ai-0.0.5/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-open-ai
-version = 0.0.41
+version = 0.0.5
 description = Use the power of OpenAI on your Django database
 long_description = file:README.rst
 url = https://github.com/PMCS64/django-open-ai
 license = MIT
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
```

