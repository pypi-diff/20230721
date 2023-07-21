# Comparing `tmp/django-open-ai-0.0.4.tar.gz` & `tmp/django-open-ai-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-open-ai-0.0.4.tar", last modified: Fri Jul 21 12:15:51 2023, max compression
+gzip compressed data, was "django-open-ai-0.0.41.tar", last modified: Fri Jul 21 12:29:30 2023, max compression
```

## Comparing `django-open-ai-0.0.4.tar` & `django-open-ai-0.0.41.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:15:51.566639 django-open-ai-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-21 12:15:51.566639 django-open-ai-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:15:51.566639 django-open-ai-0.0.4/django_open_ai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:15:51.566639 django-open-ai-0.0.4/django_open_ai/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:15:51.566639 django-open-ai-0.0.4/django_open_ai/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:15:51.566639 django-open-ai-0.0.4/django_open_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-21 12:15:51.000000 django-open-ai-0.0.4/django_open_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-21 12:15:51.000000 django-open-ai-0.0.4/django_open_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:15:51.000000 django-open-ai-0.0.4/django_open_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-21 12:15:51.000000 django-open-ai-0.0.4/django_open_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 12:15:51.000000 django-open-ai-0.0.4/django_open_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-21 12:15:51.570639 django-open-ai-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:30.217195 django-open-ai-0.0.41/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-21 12:29:30.217195 django-open-ai-0.0.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:30.217195 django-open-ai-0.0.41/django_open_ai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:30.217195 django-open-ai-0.0.41/django_open_ai/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:30.217195 django-open-ai-0.0.41/django_open_ai/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/django_open_ai/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:30.217195 django-open-ai-0.0.41/django_open_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-21 12:29:30.000000 django-open-ai-0.0.41/django_open_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-21 12:29:30.000000 django-open-ai-0.0.41/django_open_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:29:30.000000 django-open-ai-0.0.41/django_open_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-21 12:29:30.000000 django-open-ai-0.0.41/django_open_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 12:29:30.000000 django-open-ai-0.0.41/django_open_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-21 12:29:30.217195 django-open-ai-0.0.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-21 12:29:18.000000 django-open-ai-0.0.41/setup.py
```

### Comparing `django-open-ai-0.0.4/LICENSE` & `django-open-ai-0.0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `django-open-ai-0.0.4/PKG-INFO` & `django-open-ai-0.0.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-open-ai
-Version: 0.0.4
+Version: 0.0.41
 Summary: Use the power of OpenAI on your Django database
 Home-page: https://github.com/PMCS64/django-open-ai
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-open-ai-0.0.4/django_open_ai/helper.py` & `django-open-ai-0.0.41/django_open_ai/helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,16 @@
         if getter:
             return connections.databases[self.database][getter]
         return connections.databases[self.database]
 
     def engage(self):
         engine = self.cursor("ENGINE")
 
+        print(self.cursor("OPTIONS"))
+
         if engine == "django.db.backends.mysql":
             self.starter = "mysql+pymysql"
             self.query = self.cursor("OPTIONS")
 
         elif engine == "django.db.backends.postgresql":
             self.starter = "postgres"
             self.query = self.cursor("OPTIONS")
```

### Comparing `django-open-ai-0.0.4/django_open_ai/views.py` & `django-open-ai-0.0.41/django_open_ai/views.py`

 * *Files identical despite different names*

### Comparing `django-open-ai-0.0.4/django_open_ai.egg-info/PKG-INFO` & `django-open-ai-0.0.41/django_open_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-open-ai
-Version: 0.0.4
+Version: 0.0.41
 Summary: Use the power of OpenAI on your Django database
 Home-page: https://github.com/PMCS64/django-open-ai
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-open-ai-0.0.4/django_open_ai.egg-info/SOURCES.txt` & `django-open-ai-0.0.41/django_open_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-open-ai-0.0.4/setup.cfg` & `django-open-ai-0.0.41/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-open-ai
-version = 0.0.4
+version = 0.0.41
 description = Use the power of OpenAI on your Django database
 long_description = file:README.rst
 url = https://github.com/PMCS64/django-open-ai
 license = MIT
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
```

