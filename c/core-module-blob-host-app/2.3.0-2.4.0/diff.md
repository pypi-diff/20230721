# Comparing `tmp/core_module_blob_host_app-2.3.0.tar.gz` & `tmp/core_module_blob_host_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_module_blob_host_app-2.3.0.tar", last modified: Tue May  2 19:44:47 2023, max compression
+gzip compressed data, was "core_module_blob_host_app-2.4.0.tar", last modified: Fri Jul 21 02:14:46 2023, max compression
```

## Comparing `core_module_blob_host_app-2.3.0.tar` & `core_module_blob_host_app-2.4.0.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:47.026694 core_module_blob_host_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2023-05-02 19:44:47.022309 core_module_blob_host_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      573 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:46.817067 core_module_blob_host_app-2.3.0/core_module_blob_host_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      716 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:46.648777 core_module_blob_host_app-2.3.0/core_module_blob_host_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:46.652531 core_module_blob_host_app-2.3.0/core_module_blob_host_app/static/core_module_blob_host_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:46.907011 core_module_blob_host_app-2.3.0/core_module_blob_host_app/static/core_module_blob_host_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      347 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app/static/core_module_blob_host_app/js/blob_host.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:46.662747 core_module_blob_host_app-2.3.0/core_module_blob_host_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:46.931410 core_module_blob_host_app-2.3.0/core_module_blob_host_app/templates/core_module_blob_host_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app/templates/core_module_blob_host_app/blob_host.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      507 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app/templates/core_module_blob_host_app/blob_host_display.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      288 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:46.974514 core_module_blob_host_app-2.3.0/core_module_blob_host_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      152 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app/views/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5661 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app/views/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:46.893554 core_module_blob_host_app-2.3.0/core_module_blob_host_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2023-05-02 19:44:46.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      854 2023-05-02 19:44:46.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:44:46.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       51 2023-05-02 19:44:46.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-05-02 19:44:46.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       44 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:44:47.028282 core_module_blob_host_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1073 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:47.000390 core_module_blob_host_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:46.243037 core_module_blob_host_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2023-07-21 02:14:46.236469 core_module_blob_host_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      573 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:45.989531 core_module_blob_host_app-2.4.0/core_module_blob_host_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/core_module_blob_host_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      621 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/core_module_blob_host_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:45.809508 core_module_blob_host_app-2.4.0/core_module_blob_host_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:45.812112 core_module_blob_host_app-2.4.0/core_module_blob_host_app/static/core_module_blob_host_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:46.070862 core_module_blob_host_app-2.4.0/core_module_blob_host_app/static/core_module_blob_host_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      347 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/core_module_blob_host_app/static/core_module_blob_host_app/js/blob_host.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:45.833474 core_module_blob_host_app-2.4.0/core_module_blob_host_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:46.094143 core_module_blob_host_app-2.4.0/core_module_blob_host_app/templates/core_module_blob_host_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/core_module_blob_host_app/templates/core_module_blob_host_app/blob_host.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      533 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/core_module_blob_host_app/templates/core_module_blob_host_app/blob_host_display.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      288 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/core_module_blob_host_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:46.143989 core_module_blob_host_app-2.4.0/core_module_blob_host_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/core_module_blob_host_app/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      152 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/core_module_blob_host_app/views/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5770 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/core_module_blob_host_app/views/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:46.055410 core_module_blob_host_app-2.4.0/core_module_blob_host_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2023-07-21 02:14:45.000000 core_module_blob_host_app-2.4.0/core_module_blob_host_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      940 2023-07-21 02:14:45.000000 core_module_blob_host_app-2.4.0/core_module_blob_host_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:14:45.000000 core_module_blob_host_app-2.4.0/core_module_blob_host_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       51 2023-07-21 02:14:45.000000 core_module_blob_host_app-2.4.0/core_module_blob_host_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-07-21 02:14:45.000000 core_module_blob_host_app-2.4.0/core_module_blob_host_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       44 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:14:46.245009 core_module_blob_host_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1073 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:46.185785 core_module_blob_host_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1849 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:46.200252 core_module_blob_host_app-2.4.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:46.227152 core_module_blob_host_app-2.4.0/tests/views/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/tests/views/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6574 2023-07-21 02:14:44.000000 core_module_blob_host_app-2.4.0/tests/views/views/tests_unit.py
```

### Comparing `core_module_blob_host_app-2.3.0/LICENSE.md` & `core_module_blob_host_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_module_blob_host_app-2.3.0/PKG-INFO` & `core_module_blob_host_app-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_blob_host_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Blob Host module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_blob_host_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_blob_host_app
         =========================
```

### Comparing `core_module_blob_host_app-2.3.0/README.rst` & `core_module_blob_host_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_blob_host_app-2.3.0/core_module_blob_host_app/views/views.py` & `core_module_blob_host_app-2.4.0/core_module_blob_host_app/views/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 from urllib.parse import urljoin
 
 from django.urls import reverse
 
 from core_main_app.components.blob import api as blob_api
 from core_main_app.components.blob.models import Blob
 from core_main_app.components.blob.utils import get_blob_download_uri
+from core_module_blob_host_app import settings
+from core_module_blob_host_app.views.forms import BLOBHostForm
 from core_parser_app.tools.modules.views.builtin.popup_module import (
     AbstractPopupModule,
 )
 from core_parser_app.tools.modules.views.module import AbstractModule
 from xml_utils.xsd_tree.operations.xml_entities import XmlEntities
-from core_module_blob_host_app import settings as blob_host_settings
-from core_module_blob_host_app.views.forms import BLOBHostForm
 
 logger = logging.getLogger(__name__)
 
 
 class BlobHostModule(AbstractPopupModule):
     """BLOB host module"""
 
+    error = None
+
     def __init__(self):
         """Initialize module"""
         super().__init__(
             button_label="Upload File",
             scripts=[
                 "core_parser_app/js/commons/file_uploader.js",
                 "core_module_blob_host_app/js/blob_host.js",
@@ -80,44 +82,45 @@
             )
             blob.blob = uploaded_file
             blob_api.insert(blob, request.user)
 
             blob_pid = None
 
             # Retrieve Blob PID if the core_linked_records_app is installed
-            if "core_linked_records_app" in blob_host_settings.INSTALLED_APPS:
+            if "core_linked_records_app" in settings.INSTALLED_APPS:
+                from core_linked_records_app import (
+                    settings as linked_records_settings,
+                )
                 from core_linked_records_app.components.pid_settings import (
                     api as pid_settings_api,
                 )
                 from core_linked_records_app.components.blob import (
                     api as linked_records_blob_api,
                 )
 
                 # Create blob PID if `auto_set_pid` is True
                 if pid_settings_api.get().auto_set_pid:
                     blob_pid_url = reverse(
                         "core_linked_records_provider_record",
                         kwargs={
-                            "provider": "local",
+                            "provider": linked_records_settings.ID_PROVIDER_SYSTEM_NAME,
                             "record": linked_records_blob_api.get_pid_for_blob(
                                 str(blob.id)
                             ).record_name,
                         },
                     )
-                    blob_pid = urljoin(
-                        blob_host_settings.SERVER_URI, blob_pid_url
-                    )
+                    blob_pid = urljoin(settings.SERVER_URI, blob_pid_url)
 
             # Retrieve download URI.
             return (
                 blob_pid if blob_pid else get_blob_download_uri(blob, request)
             )
         except Exception as exc:
-            logger.log(str(exc))
-            self.error = "An unexpected error occurred."
+            self.error = "An unexpected error occurred"
+            logger.error(f"{self.error}: {str(exc)}")
             return data
 
     def _retrieve_data(self, request):
         """Retrieve module's data
 
         Args:
             request:
@@ -133,15 +136,15 @@
                 if len(request.GET["data"]) > 0:
                     data = request.GET["data"]
         elif request.method == "POST":
             data = self.retrieve_post_data(request)
 
         return (
             data_xml_entities.escape_xml_entities(data)
-            if blob_host_settings.AUTO_ESCAPE_XML_ENTITIES
+            if settings.AUTO_ESCAPE_XML_ENTITIES
             else data
         )
 
     def _render_data(self, request):
         """Return module's data rendering
 
         Args:
```

### Comparing `core_module_blob_host_app-2.3.0/core_module_blob_host_app.egg-info/PKG-INFO` & `core_module_blob_host_app-2.4.0/core_module_blob_host_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-blob-host-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Blob Host module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_blob_host_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_blob_host_app
         =========================
```

### Comparing `core_module_blob_host_app-2.3.0/setup.py` & `core_module_blob_host_app-2.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_blob_host_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Blob Host module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_blob_host_app",
     packages=find_packages(),
     include_package_data=True,
```

