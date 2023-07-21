# Comparing `tmp/django-open-ai-0.0.5.tar.gz` & `tmp/django-open-ai-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-open-ai-0.0.5.tar", last modified: Fri Jul 21 12:35:57 2023, max compression
+gzip compressed data, was "django-open-ai-0.1.0.tar", last modified: Fri Jul 21 13:11:35 2023, max compression
```

## Comparing `django-open-ai-0.0.5.tar` & `django-open-ai-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:35:57.144065 django-open-ai-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-21 12:35:57.144065 django-open-ai-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:35:57.144065 django-open-ai-0.0.5/django_open_ai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:35:57.144065 django-open-ai-0.0.5/django_open_ai/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:35:57.144065 django-open-ai-0.0.5/django_open_ai/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/django_open_ai/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:35:57.144065 django-open-ai-0.0.5/django_open_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-21 12:35:57.000000 django-open-ai-0.0.5/django_open_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-21 12:35:57.000000 django-open-ai-0.0.5/django_open_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:35:57.000000 django-open-ai-0.0.5/django_open_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-21 12:35:57.000000 django-open-ai-0.0.5/django_open_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 12:35:57.000000 django-open-ai-0.0.5/django_open_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-21 12:35:57.144065 django-open-ai-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-21 12:35:45.000000 django-open-ai-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:11:35.271992 django-open-ai-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-21 13:11:20.000000 django-open-ai-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 13:11:20.000000 django-open-ai-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-21 13:11:35.271992 django-open-ai-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-21 13:11:20.000000 django-open-ai-0.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:11:35.271992 django-open-ai-0.1.0/django_open_ai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:11:20.000000 django-open-ai-0.1.0/django_open_ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 13:11:20.000000 django-open-ai-0.1.0/django_open_ai/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-21 13:11:20.000000 django-open-ai-0.1.0/django_open_ai/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-21 13:11:20.000000 django-open-ai-0.1.0/django_open_ai/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-21 13:11:20.000000 django-open-ai-0.1.0/django_open_ai/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:11:35.271992 django-open-ai-0.1.0/django_open_ai/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:11:20.000000 django-open-ai-0.1.0/django_open_ai/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-21 13:11:20.000000 django-open-ai-0.1.0/django_open_ai/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:11:35.271992 django-open-ai-0.1.0/django_open_ai/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-21 13:11:20.000000 django-open-ai-0.1.0/django_open_ai/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 13:11:20.000000 django-open-ai-0.1.0/django_open_ai/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-21 13:11:20.000000 django-open-ai-0.1.0/django_open_ai/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:11:35.271992 django-open-ai-0.1.0/django_open_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-21 13:11:35.000000 django-open-ai-0.1.0/django_open_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-21 13:11:35.000000 django-open-ai-0.1.0/django_open_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:11:35.000000 django-open-ai-0.1.0/django_open_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-21 13:11:35.000000 django-open-ai-0.1.0/django_open_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 13:11:35.000000 django-open-ai-0.1.0/django_open_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-21 13:11:20.000000 django-open-ai-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-21 13:11:35.271992 django-open-ai-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-21 13:11:20.000000 django-open-ai-0.1.0/setup.py
```

### Comparing `django-open-ai-0.0.5/LICENSE` & `django-open-ai-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-open-ai-0.0.5/django_open_ai/helper.py` & `django-open-ai-0.1.0/django_open_ai/helper.py`

 * *Files identical despite different names*

### Comparing `django-open-ai-0.0.5/django_open_ai/views.py` & `django-open-ai-0.1.0/django_open_ai/views.py`

 * *Files identical despite different names*

### Comparing `django-open-ai-0.0.5/django_open_ai.egg-info/SOURCES.txt` & `django-open-ai-0.1.0/django_open_ai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 django_open_ai/__init__.py
 django_open_ai/admin.py
 django_open_ai/apps.py
 django_open_ai/forms.py
 django_open_ai/helper.py
 django_open_ai/models.py
 django_open_ai/tests.py
-django_open_ai/urls.py
 django_open_ai/views.py
 django_open_ai.egg-info/PKG-INFO
 django_open_ai.egg-info/SOURCES.txt
 django_open_ai.egg-info/dependency_links.txt
 django_open_ai.egg-info/requires.txt
 django_open_ai.egg-info/top_level.txt
 django_open_ai/migrations/__init__.py
```

### Comparing `django-open-ai-0.0.5/setup.cfg` & `django-open-ai-0.1.0/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-open-ai
-version = 0.0.5
+version = 0.1.0
 description = Use the power of OpenAI on your Django database
 long_description = file:README.rst
 url = https://github.com/PMCS64/django-open-ai
 license = MIT
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
```

