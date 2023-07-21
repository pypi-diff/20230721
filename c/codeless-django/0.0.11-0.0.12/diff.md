# Comparing `tmp/codeless_django-0.0.11.tar.gz` & `tmp/codeless-django-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "codeless-django-0.0.12.tar", last modified: Fri Jul 21 13:46:20 2023, max compression
```

## Comparing `codeless_django-0.0.11.tar` & `codeless-django-0.0.12.tar`

### file list

```diff
@@ -1,42 +1,54 @@
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 codeless_django-0.0.11/MANIFEST.in
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 codeless_django-0.0.11/setup.cfg
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 codeless_django-0.0.11/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/apps.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/data_manager.py
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/fields.json
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/tests.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/urls.py
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/views.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/additional_files/.gitignore
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/additional_files/root_urls.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/templates/codeless_django/base.html
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/templates/codeless_django/demo.html
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/templates/codeless_django/fields.html
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/templates/codeless_django/home.html
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/templates/codeless_django/forms/all_field_types.html
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/templates/codeless_django/forms/app_form.html
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/templates/codeless_django/forms/choice_option.html
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/templates/codeless_django/forms/common_option_form.html
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/templates/codeless_django/forms/dropdown_option.html
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/templates/codeless_django/forms/field_form.html
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/templates/codeless_django/forms/field_option.html
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/templates/codeless_django/forms/model_form.html
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/templates/codeless_django/forms/model_meta_form.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/templates/codeless_django/forms/option_form.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/templatetags/__init__.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/templatetags/codeless_django_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/writers/__init__.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/writers/apis.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/writers/apps.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/writers/base.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/writers/documentation.py
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/writers/files.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/writers/models.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/writers/serializers.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 codeless_django-0.0.11/codeless_django/writers/views.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 codeless_django-0.0.11/.gitignore
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 codeless_django-0.0.11/LICENSE
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 codeless_django-0.0.11/README.md
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 codeless_django-0.0.11/pyproject.toml
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 codeless_django-0.0.11/PKG-INFO
+drwxrwxr-x   0 omar      (1000) omar      (1000)        0 2023-07-21 13:46:20.107052 codeless-django-0.0.12/
+-rw-rw-r--   0 omar      (1000) omar      (1000)     1450 2023-04-11 02:03:29.000000 codeless-django-0.0.12/LICENSE
+-rw-rw-r--   0 omar      (1000) omar      (1000)      228 2023-04-11 14:21:10.000000 codeless-django-0.0.12/MANIFEST.in
+-rw-rw-r--   0 omar      (1000) omar      (1000)     1375 2023-07-21 13:46:20.107052 codeless-django-0.0.12/PKG-INFO
+-rw-rw-r--   0 omar      (1000) omar      (1000)      828 2023-04-11 03:07:49.000000 codeless-django-0.0.12/README.md
+drwxrwxr-x   0 omar      (1000) omar      (1000)        0 2023-07-21 13:46:20.099052 codeless-django-0.0.12/codeless_django/
+-rw-rw-r--   0 omar      (1000) omar      (1000)        0 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/__init__.py
+drwxrwxr-x   0 omar      (1000) omar      (1000)        0 2023-07-21 13:46:20.103052 codeless-django-0.0.12/codeless_django/additional_files/
+-rw-rw-r--   0 omar      (1000) omar      (1000)     1823 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/additional_files/.gitignore
+-rw-rw-r--   0 omar      (1000) omar      (1000)     1623 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/additional_files/root_urls.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)      154 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/apps.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)     3218 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/data_manager.py
+drwxrwxr-x   0 omar      (1000) omar      (1000)        0 2023-07-21 13:46:20.099052 codeless-django-0.0.12/codeless_django/templates/
+drwxrwxr-x   0 omar      (1000) omar      (1000)        0 2023-07-21 13:46:20.103052 codeless-django-0.0.12/codeless_django/templates/codeless_django/
+-rw-rw-r--   0 omar      (1000) omar      (1000)     2183 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/templates/codeless_django/base.html
+-rw-rw-r--   0 omar      (1000) omar      (1000)     2925 2023-04-11 14:28:30.000000 codeless-django-0.0.12/codeless_django/templates/codeless_django/demo.html
+-rw-rw-r--   0 omar      (1000) omar      (1000)      369 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/templates/codeless_django/fields.html
+drwxrwxr-x   0 omar      (1000) omar      (1000)        0 2023-07-21 13:46:20.103052 codeless-django-0.0.12/codeless_django/templates/codeless_django/forms/
+-rw-rw-r--   0 omar      (1000) omar      (1000)      121 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/templates/codeless_django/forms/all_field_types.html
+-rw-rw-r--   0 omar      (1000) omar      (1000)      480 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/templates/codeless_django/forms/app_form.html
+-rw-rw-r--   0 omar      (1000) omar      (1000)      198 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/templates/codeless_django/forms/choice_option.html
+-rw-rw-r--   0 omar      (1000) omar      (1000)      257 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/templates/codeless_django/forms/common_option_form.html
+-rw-rw-r--   0 omar      (1000) omar      (1000)      288 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/templates/codeless_django/forms/dropdown_option.html
+-rw-rw-r--   0 omar      (1000) omar      (1000)      986 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/templates/codeless_django/forms/field_form.html
+-rw-rw-r--   0 omar      (1000) omar      (1000)      761 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/templates/codeless_django/forms/field_option.html
+-rw-rw-r--   0 omar      (1000) omar      (1000)      159 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/templates/codeless_django/forms/model_form.html
+-rw-rw-r--   0 omar      (1000) omar      (1000)     1122 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/templates/codeless_django/forms/model_meta_form.html
+-rw-rw-r--   0 omar      (1000) omar      (1000)        0 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/templates/codeless_django/forms/option_form.html
+-rw-rw-r--   0 omar      (1000) omar      (1000)     3437 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/templates/codeless_django/home.html
+drwxrwxr-x   0 omar      (1000) omar      (1000)        0 2023-07-21 13:46:20.103052 codeless-django-0.0.12/codeless_django/templatetags/
+-rw-rw-r--   0 omar      (1000) omar      (1000)        0 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/templatetags/__init__.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)      716 2023-04-11 15:32:15.000000 codeless-django-0.0.12/codeless_django/templatetags/codeless_django_tags.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)       60 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/tests.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)     1065 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/urls.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)     3719 2023-04-23 15:48:20.000000 codeless-django-0.0.12/codeless_django/views.py
+drwxrwxr-x   0 omar      (1000) omar      (1000)        0 2023-07-21 13:46:20.107052 codeless-django-0.0.12/codeless_django/writers/
+-rw-rw-r--   0 omar      (1000) omar      (1000)        0 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/writers/__init__.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)     1871 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/writers/apis.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)     4645 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/writers/apps.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)     1389 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/writers/base.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)      447 2023-04-11 15:15:42.000000 codeless-django-0.0.12/codeless_django/writers/documentation.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)     2590 2023-04-11 15:25:44.000000 codeless-django-0.0.12/codeless_django/writers/files.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)     1342 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/writers/models.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)      689 2023-04-11 15:17:07.000000 codeless-django-0.0.12/codeless_django/writers/serializers.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)     1965 2023-04-11 01:56:03.000000 codeless-django-0.0.12/codeless_django/writers/views.py
+drwxrwxr-x   0 omar      (1000) omar      (1000)        0 2023-07-21 13:46:20.099052 codeless-django-0.0.12/codeless_django.egg-info/
+-rw-rw-r--   0 omar      (1000) omar      (1000)     1375 2023-07-21 13:46:20.000000 codeless-django-0.0.12/codeless_django.egg-info/PKG-INFO
+-rw-rw-r--   0 omar      (1000) omar      (1000)     1788 2023-07-21 13:46:20.000000 codeless-django-0.0.12/codeless_django.egg-info/SOURCES.txt
+-rw-rw-r--   0 omar      (1000) omar      (1000)        1 2023-07-21 13:46:20.000000 codeless-django-0.0.12/codeless_django.egg-info/dependency_links.txt
+-rw-rw-r--   0 omar      (1000) omar      (1000)       12 2023-07-21 13:46:20.000000 codeless-django-0.0.12/codeless_django.egg-info/requires.txt
+-rw-rw-r--   0 omar      (1000) omar      (1000)       16 2023-07-21 13:46:20.000000 codeless-django-0.0.12/codeless_django.egg-info/top_level.txt
+-rw-rw-r--   0 omar      (1000) omar      (1000)      528 2023-07-21 13:42:12.000000 codeless-django-0.0.12/pyproject.toml
+-rw-rw-r--   0 omar      (1000) omar      (1000)      938 2023-07-21 13:46:20.107052 codeless-django-0.0.12/setup.cfg
+-rw-rw-r--   0 omar      (1000) omar      (1000)       37 2023-04-07 17:41:04.000000 codeless-django-0.0.12/setup.py
```

### Comparing `codeless_django-0.0.11/codeless_django/data_manager.py` & `codeless-django-0.0.12/codeless_django/data_manager.py`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/codeless_django/urls.py` & `codeless-django-0.0.12/codeless_django/urls.py`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/codeless_django/views.py` & `codeless-django-0.0.12/codeless_django/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,7 +99,8 @@
     write_template_views=bool(request.POST.get("template_views"))
     write_api_views=bool(request.POST.get("api_views"))
     data=data_manager._load_data()
     app_writer = WriteApps(data["apps"],write_template_views,write_api_views)
     app_writer.write()
     os.system("rm data.json")
     return redirect('/swagger/')
+
```

### Comparing `codeless_django-0.0.11/codeless_django/additional_files/.gitignore` & `codeless-django-0.0.12/codeless_django/additional_files/.gitignore`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/codeless_django/additional_files/root_urls.py` & `codeless-django-0.0.12/codeless_django/additional_files/root_urls.py`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/codeless_django/templates/codeless_django/base.html` & `codeless-django-0.0.12/codeless_django/templates/codeless_django/base.html`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/codeless_django/templates/codeless_django/demo.html` & `codeless-django-0.0.12/codeless_django/templates/codeless_django/demo.html`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/codeless_django/templates/codeless_django/home.html` & `codeless-django-0.0.12/codeless_django/templates/codeless_django/home.html`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/codeless_django/templates/codeless_django/forms/field_form.html` & `codeless-django-0.0.12/codeless_django/templates/codeless_django/forms/field_form.html`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/codeless_django/templates/codeless_django/forms/field_option.html` & `codeless-django-0.0.12/codeless_django/templates/codeless_django/forms/field_option.html`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/codeless_django/templates/codeless_django/forms/model_meta_form.html` & `codeless-django-0.0.12/codeless_django/templates/codeless_django/forms/model_meta_form.html`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/codeless_django/templatetags/codeless_django_tags.py` & `codeless-django-0.0.12/codeless_django/templatetags/codeless_django_tags.py`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/codeless_django/writers/apis.py` & `codeless-django-0.0.12/codeless_django/writers/apis.py`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/codeless_django/writers/apps.py` & `codeless-django-0.0.12/codeless_django/writers/apps.py`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/codeless_django/writers/base.py` & `codeless-django-0.0.12/codeless_django/writers/base.py`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/codeless_django/writers/files.py` & `codeless-django-0.0.12/codeless_django/writers/files.py`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/codeless_django/writers/models.py` & `codeless-django-0.0.12/codeless_django/writers/models.py`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/codeless_django/writers/serializers.py` & `codeless-django-0.0.12/codeless_django/writers/serializers.py`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/codeless_django/writers/views.py` & `codeless-django-0.0.12/codeless_django/writers/views.py`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/LICENSE` & `codeless-django-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/README.md` & `codeless-django-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `codeless_django-0.0.11/pyproject.toml` & `codeless-django-0.0.12/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "codeless-django"
-version = "0.0.11"
+version = "0.0.12"
 authors = [
   { name="Omar Faruk", email="omar.iut.09@gmail.com" },
 ]
 description = "A Django app to create django apps, models, urls, views , api-views, documentation in a single click"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `codeless_django-0.0.11/PKG-INFO` & `codeless-django-0.0.12/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: codeless-django
-Version: 0.0.11
+Version: 0.0.12
 Summary: A Django app to create django apps, models, urls, views , api-views, documentation in a single click
+Home-page: https://www.example.com/
+Author: Omar Faruk
 Author-email: Omar Faruk <omar.iut.09@gmail.com>
-License-File: LICENSE
+License: BSD-3-Clause  # Example license
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # CodeLess-Django
 
 CodeLess-Django is a Django app to develop django apps without writing code. Developers can create apps and models from a web page where all the models field types and options are placed in front of developers eyes . CodeLess-Django will take care of adding apps to settings file, creating generic views and api views etc.
 Detailed documentation is in the "docs" directory.
 
 ## Quick start
```

