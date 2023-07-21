# Comparing `tmp/django-cabinet-0.9.0.tar.gz` & `tmp/django-cabinet-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-cabinet-0.9.0.tar", last modified: Mon Apr 15 09:02:09 2019, max compression
+gzip compressed data, was "dist/django-cabinet-0.9.1.tar", last modified: Wed Jul 24 15:00:09 2019, max compression
```

## Comparing `django-cabinet-0.9.0.tar` & `django-cabinet-0.9.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     6271 2019-04-15 09:01:46.000000 django-cabinet-0.9.0/CHANGELOG.rst
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1548 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/LICENSE
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      131 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/MANIFEST.in
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1768 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      852 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/README.rst
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/cabinet/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      113 2019-04-15 09:01:21.000000 django-cabinet-0.9.0/cabinet/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2206 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/admin.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      191 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/apps.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     9370 2019-04-15 08:42:04.000000 django-cabinet-0.9.0/cabinet/base.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    20198 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/base_admin.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1745 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/ckeditor.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2940 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/fields.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/cabinet/locale/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/cabinet/locale/de/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/cabinet/locale/de/LC_MESSAGES/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4034 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     6228 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/cabinet/migrations/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4442 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/migrations/0001_initial.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      916 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/migrations/0002_auto_20170620_0846.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      676 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/migrations/0003_file__overwrite.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1260 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/migrations/0004_auto_20181212_0252.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      941 2019-04-15 08:43:51.000000 django-cabinet-0.9.0/cabinet/migrations/0005_auto_20190415_0343.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/migrations/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2295 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/models.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/cabinet/static/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/cabinet/static/cabinet/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3029 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/static/cabinet/cabinet.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3060 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/static/cabinet/cabinet.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      319 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/static/cabinet/ckeditor.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      321 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/static/cabinet/inline-upload.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1268 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/static/cabinet/inline-upload.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/cabinet/templates/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/cabinet/templates/admin/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/cabinet/templates/admin/cabinet/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      526 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/templates/admin/cabinet/cabinet_file_raw_id_widget.html
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/cabinet/templates/admin/cabinet/file/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1030 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/templates/admin/cabinet/file/change_form.html
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4486 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/templates/admin/cabinet/file/change_list.html
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/cabinet/templates/admin/cabinet/folder/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      958 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/cabinet/templates/admin/cabinet/folder/change_form.html
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/django_cabinet.egg-info/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1768 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/django_cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1176 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/django_cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/django_cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2019-04-15 08:40:45.000000 django-cabinet-0.9.0/django_cabinet.egg-info/not-zip-safe
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       38 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/django_cabinet.egg-info/requires.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        8 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/django_cabinet.egg-info/top_level.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      251 2019-04-15 09:02:09.000000 django-cabinet-0.9.0/setup.cfg
--rwxrwxr-x   0 matthias  (1000) matthias  (1000)     1200 2019-04-15 08:40:40.000000 django-cabinet-0.9.0/setup.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     6271 2019-04-15 09:01:46.000000 django-cabinet-0.9.1/CHANGELOG.rst
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1548 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/LICENSE
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      131 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/MANIFEST.in
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1768 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/PKG-INFO
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      852 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/README.rst
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/cabinet/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      113 2019-07-24 14:59:34.000000 django-cabinet-0.9.1/cabinet/__init__.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2206 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/admin.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      191 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/apps.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     9370 2019-04-15 08:42:04.000000 django-cabinet-0.9.1/cabinet/base.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    20198 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/base_admin.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1745 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/ckeditor.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2967 2019-07-24 14:57:47.000000 django-cabinet-0.9.1/cabinet/fields.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/cabinet/locale/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/cabinet/locale/de/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/cabinet/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     4034 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     6228 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/cabinet/migrations/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     4442 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/migrations/0001_initial.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      916 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/migrations/0002_auto_20170620_0846.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      676 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/migrations/0003_file__overwrite.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1260 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/migrations/0004_auto_20181212_0252.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      941 2019-04-15 08:43:51.000000 django-cabinet-0.9.1/cabinet/migrations/0005_auto_20190415_0343.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/migrations/__init__.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2295 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/models.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/cabinet/static/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/cabinet/static/cabinet/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     3029 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/static/cabinet/cabinet.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     3060 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/static/cabinet/cabinet.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      319 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/static/cabinet/ckeditor.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      321 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/static/cabinet/inline-upload.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1268 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/static/cabinet/inline-upload.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/cabinet/templates/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/cabinet/templates/admin/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/cabinet/templates/admin/cabinet/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      526 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/templates/admin/cabinet/cabinet_file_raw_id_widget.html
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/cabinet/templates/admin/cabinet/file/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1030 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/templates/admin/cabinet/file/change_form.html
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     4486 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/templates/admin/cabinet/file/change_list.html
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/cabinet/templates/admin/cabinet/folder/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      958 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/cabinet/templates/admin/cabinet/folder/change_form.html
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/django_cabinet.egg-info/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1768 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/django_cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1176 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/django_cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/django_cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2019-04-15 08:40:45.000000 django-cabinet-0.9.1/django_cabinet.egg-info/not-zip-safe
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       38 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/django_cabinet.egg-info/requires.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        8 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/django_cabinet.egg-info/top_level.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      251 2019-07-24 15:00:09.000000 django-cabinet-0.9.1/setup.cfg
+-rwxrwxr-x   0 matthias  (1000) matthias  (1000)     1200 2019-04-15 08:40:40.000000 django-cabinet-0.9.1/setup.py
```

### Comparing `django-cabinet-0.9.0/CHANGELOG.rst` & `django-cabinet-0.9.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/LICENSE` & `django-cabinet-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/PKG-INFO` & `django-cabinet-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-cabinet
-Version: 0.9.0
+Version: 0.9.1
 Summary: Media library for Django
 Home-page: http://github.com/matthiask/django-cabinet/
 Author: Matthias Kestenholz
 Author-email: mk@feinheit.ch
 License: BSD License
 Description: =========================================
         django-cabinet - Media library for Django
```

### Comparing `django-cabinet-0.9.0/README.rst` & `django-cabinet-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/cabinet/admin.py` & `django-cabinet-0.9.1/cabinet/admin.py`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/cabinet/base.py` & `django-cabinet-0.9.1/cabinet/base.py`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/cabinet/base_admin.py` & `django-cabinet-0.9.1/cabinet/base_admin.py`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/cabinet/ckeditor.py` & `django-cabinet-0.9.1/cabinet/ckeditor.py`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/cabinet/fields.py` & `django-cabinet-0.9.1/cabinet/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 class CabinetFileRawIdWidget(ForeignKeyRawIdWidget):
     template_name = "admin/cabinet/cabinet_file_raw_id_widget.html"
 
     class Media:
         css = {"all": ["cabinet/inline-upload.css"]}
-        js = ["cabinet/inline-upload.js"]
+        js = ["admin/js/jquery.init.js", "cabinet/inline-upload.js"]
 
     def get_context(self, name, value, attrs):
         context = super().get_context(name, value, attrs)
         instance = getattr(self, "instance", None)
         context["cabinet"] = {
             "upload_form": UploadForm(
                 prefix="cu-{}".format(id(self)),
```

### Comparing `django-cabinet-0.9.0/cabinet/locale/de/LC_MESSAGES/django.mo` & `django-cabinet-0.9.1/cabinet/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/cabinet/locale/de/LC_MESSAGES/django.po` & `django-cabinet-0.9.1/cabinet/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/cabinet/migrations/0001_initial.py` & `django-cabinet-0.9.1/cabinet/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/cabinet/migrations/0002_auto_20170620_0846.py` & `django-cabinet-0.9.1/cabinet/migrations/0002_auto_20170620_0846.py`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/cabinet/migrations/0003_file__overwrite.py` & `django-cabinet-0.9.1/cabinet/migrations/0003_file__overwrite.py`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/cabinet/migrations/0004_auto_20181212_0252.py` & `django-cabinet-0.9.1/cabinet/migrations/0004_auto_20181212_0252.py`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/cabinet/migrations/0005_auto_20190415_0343.py` & `django-cabinet-0.9.1/cabinet/migrations/0005_auto_20190415_0343.py`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/cabinet/models.py` & `django-cabinet-0.9.1/cabinet/models.py`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/cabinet/static/cabinet/cabinet.css` & `django-cabinet-0.9.1/cabinet/static/cabinet/cabinet.css`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/cabinet/static/cabinet/cabinet.js` & `django-cabinet-0.9.1/cabinet/static/cabinet/cabinet.js`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/cabinet/static/cabinet/inline-upload.js` & `django-cabinet-0.9.1/cabinet/static/cabinet/inline-upload.js`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/cabinet/templates/admin/cabinet/cabinet_file_raw_id_widget.html` & `django-cabinet-0.9.1/cabinet/templates/admin/cabinet/cabinet_file_raw_id_widget.html`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/cabinet/templates/admin/cabinet/file/change_form.html` & `django-cabinet-0.9.1/cabinet/templates/admin/cabinet/file/change_form.html`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/cabinet/templates/admin/cabinet/file/change_list.html` & `django-cabinet-0.9.1/cabinet/templates/admin/cabinet/file/change_list.html`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/cabinet/templates/admin/cabinet/folder/change_form.html` & `django-cabinet-0.9.1/cabinet/templates/admin/cabinet/folder/change_form.html`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/django_cabinet.egg-info/PKG-INFO` & `django-cabinet-0.9.1/django_cabinet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-cabinet
-Version: 0.9.0
+Version: 0.9.1
 Summary: Media library for Django
 Home-page: http://github.com/matthiask/django-cabinet/
 Author: Matthias Kestenholz
 Author-email: mk@feinheit.ch
 License: BSD License
 Description: =========================================
         django-cabinet - Media library for Django
```

### Comparing `django-cabinet-0.9.0/django_cabinet.egg-info/SOURCES.txt` & `django-cabinet-0.9.1/django_cabinet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cabinet-0.9.0/setup.py` & `django-cabinet-0.9.1/setup.py`

 * *Files identical despite different names*

