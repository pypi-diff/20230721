# Comparing `tmp/django-admin-commands2-1.1.2.tar.gz` & `tmp/django-admin-commands2-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-commands2-1.1.2.tar", last modified: Tue Jul 18 09:18:46 2023, max compression
+gzip compressed data, was "django-admin-commands2-1.1.3.tar", last modified: Fri Jul 21 12:17:33 2023, max compression
```

## Comparing `django-admin-commands2-1.1.2.tar` & `django-admin-commands2-1.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-18 09:18:46.257682 django-admin-commands2-1.1.2/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1510 2023-02-15 10:45:20.000000 django-admin-commands2-1.1.2/LICENSE
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      193 2023-02-15 05:55:10.000000 django-admin-commands2-1.1.2/MANIFEST.in
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     5217 2023-07-18 09:18:46.257682 django-admin-commands2-1.1.2/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     3705 2023-02-15 06:11:17.000000 django-admin-commands2-1.1.2/README.rst
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-18 09:18:46.257682 django-admin-commands2-1.1.2/admin_commands/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2023-07-18 09:18:43.000000 django-admin-commands2-1.1.2/admin_commands/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     5414 2023-07-18 09:17:59.000000 django-admin-commands2-1.1.2/admin_commands/admin.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      464 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.2/admin_commands/app_settings.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      552 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.2/admin_commands/apps.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      313 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.2/admin_commands/forms.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-18 09:18:46.257682 django-admin-commands2-1.1.2/admin_commands/migrations/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2121 2023-02-10 19:33:30.000000 django-admin-commands2-1.1.2/admin_commands/migrations/0001_initial.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-02-09 09:31:02.000000 django-admin-commands2-1.1.2/admin_commands/migrations/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2538 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.2/admin_commands/models.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-18 09:18:46.253682 django-admin-commands2-1.1.2/admin_commands/templates/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-18 09:18:46.257682 django-admin-commands2-1.1.2/admin_commands/templates/admin_commands/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1729 2023-02-15 05:55:10.000000 django-admin-commands2-1.1.2/admin_commands/templates/admin_commands/execute_command.html
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4851 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.2/admin_commands/tests.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1276 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.2/admin_commands/utils.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       63 2023-02-09 09:31:02.000000 django-admin-commands2-1.1.2/admin_commands/views.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-18 09:18:46.257682 django-admin-commands2-1.1.2/django_admin_commands2.egg-info/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     5217 2023-07-18 09:18:46.000000 django-admin-commands2-1.1.2/django_admin_commands2.egg-info/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      645 2023-07-18 09:18:46.000000 django-admin-commands2-1.1.2/django_admin_commands2.egg-info/SOURCES.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-07-18 09:18:46.000000 django-admin-commands2-1.1.2/django_admin_commands2.egg-info/dependency_links.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       12 2023-07-18 09:18:46.000000 django-admin-commands2-1.1.2/django_admin_commands2.egg-info/requires.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       21 2023-07-18 09:18:46.000000 django-admin-commands2-1.1.2/django_admin_commands2.egg-info/top_level.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1458 2023-07-18 09:18:46.257682 django-admin-commands2-1.1.2/setup.cfg
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       37 2019-12-25 18:25:30.000000 django-admin-commands2-1.1.2/setup.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-21 12:17:33.527306 django-admin-commands2-1.1.3/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1510 2023-07-21 12:16:06.000000 django-admin-commands2-1.1.3/LICENSE
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      193 2023-02-15 05:55:10.000000 django-admin-commands2-1.1.3/MANIFEST.in
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     5217 2023-07-21 12:17:33.531308 django-admin-commands2-1.1.3/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     3705 2023-07-21 12:16:06.000000 django-admin-commands2-1.1.3/README.rst
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-21 12:17:33.527306 django-admin-commands2-1.1.3/admin_commands/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2023-07-21 12:16:06.000000 django-admin-commands2-1.1.3/admin_commands/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     5432 2023-07-21 12:16:06.000000 django-admin-commands2-1.1.3/admin_commands/admin.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      464 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.3/admin_commands/app_settings.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      552 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.3/admin_commands/apps.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      313 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.3/admin_commands/forms.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-21 12:17:33.527306 django-admin-commands2-1.1.3/admin_commands/migrations/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2121 2023-02-10 19:33:30.000000 django-admin-commands2-1.1.3/admin_commands/migrations/0001_initial.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-02-09 09:31:02.000000 django-admin-commands2-1.1.3/admin_commands/migrations/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2538 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.3/admin_commands/models.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-21 12:17:33.519303 django-admin-commands2-1.1.3/admin_commands/templates/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-21 12:17:33.527306 django-admin-commands2-1.1.3/admin_commands/templates/admin_commands/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1729 2023-02-15 05:55:10.000000 django-admin-commands2-1.1.3/admin_commands/templates/admin_commands/execute_command.html
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4851 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.3/admin_commands/tests.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1276 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.3/admin_commands/utils.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       63 2023-02-09 09:31:02.000000 django-admin-commands2-1.1.3/admin_commands/views.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-21 12:17:33.527306 django-admin-commands2-1.1.3/django_admin_commands2.egg-info/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     5217 2023-07-21 12:17:33.000000 django-admin-commands2-1.1.3/django_admin_commands2.egg-info/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      645 2023-07-21 12:17:33.000000 django-admin-commands2-1.1.3/django_admin_commands2.egg-info/SOURCES.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-07-21 12:17:33.000000 django-admin-commands2-1.1.3/django_admin_commands2.egg-info/dependency_links.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       12 2023-07-21 12:17:33.000000 django-admin-commands2-1.1.3/django_admin_commands2.egg-info/requires.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       21 2023-07-21 12:17:33.000000 django-admin-commands2-1.1.3/django_admin_commands2.egg-info/top_level.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1458 2023-07-21 12:17:33.531308 django-admin-commands2-1.1.3/setup.cfg
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       37 2019-12-25 18:25:30.000000 django-admin-commands2-1.1.3/setup.py
```

### Comparing `django-admin-commands2-1.1.2/LICENSE` & `django-admin-commands2-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-commands2-1.1.2/PKG-INFO` & `django-admin-commands2-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-commands2
-Version: 1.1.2
+Version: 1.1.3
 Summary: Execute management commands via admin with ease and control.
 Home-page: https://github.com/KUWAITNET/django-admin-commands
 Author: Ramez Ashraf
 Author-email: ramez@kuwaitnet.com
 Project-URL: Source, https://github.com/KUWAITNET/django-admin-commands
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-admin-commands2-1.1.2/README.rst` & `django-admin-commands2-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-admin-commands2-1.1.2/admin_commands/admin.py` & `django-admin-commands2-1.1.3/admin_commands/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,16 +63,17 @@
 
     def execute_command_and_return_response(self, request, command, args):
 
         if ADMIN_COMMANDS_CONFIG['use_django_rq']:
             from django_rq import get_queue
             queue = get_queue('default')
             queue.enqueue(command.execute, request.user, args)
+        else:
+            command.execute(request.user, args)
 
-        command.execute(request.user, args)
         self.message_user(request, _('Command executed'))
         return self.response_post_save_add(request, command)
 
     def execute_command_view(self, request, object_id):
         command = self.get_object(request, object_id)
         if self.has_change_permission(request, command) is False:
             raise PermissionDenied
```

### Comparing `django-admin-commands2-1.1.2/admin_commands/apps.py` & `django-admin-commands2-1.1.3/admin_commands/apps.py`

 * *Files identical despite different names*

### Comparing `django-admin-commands2-1.1.2/admin_commands/migrations/0001_initial.py` & `django-admin-commands2-1.1.3/admin_commands/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-admin-commands2-1.1.2/admin_commands/models.py` & `django-admin-commands2-1.1.3/admin_commands/models.py`

 * *Files identical despite different names*

### Comparing `django-admin-commands2-1.1.2/admin_commands/templates/admin_commands/execute_command.html` & `django-admin-commands2-1.1.3/admin_commands/templates/admin_commands/execute_command.html`

 * *Files identical despite different names*

### Comparing `django-admin-commands2-1.1.2/admin_commands/tests.py` & `django-admin-commands2-1.1.3/admin_commands/tests.py`

 * *Files identical despite different names*

### Comparing `django-admin-commands2-1.1.2/admin_commands/utils.py` & `django-admin-commands2-1.1.3/admin_commands/utils.py`

 * *Files identical despite different names*

### Comparing `django-admin-commands2-1.1.2/django_admin_commands2.egg-info/PKG-INFO` & `django-admin-commands2-1.1.3/django_admin_commands2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-commands2
-Version: 1.1.2
+Version: 1.1.3
 Summary: Execute management commands via admin with ease and control.
 Home-page: https://github.com/KUWAITNET/django-admin-commands
 Author: Ramez Ashraf
 Author-email: ramez@kuwaitnet.com
 Project-URL: Source, https://github.com/KUWAITNET/django-admin-commands
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-admin-commands2-1.1.2/django_admin_commands2.egg-info/SOURCES.txt` & `django-admin-commands2-1.1.3/django_admin_commands2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-commands2-1.1.2/setup.cfg` & `django-admin-commands2-1.1.3/setup.cfg`

 * *Files identical despite different names*

