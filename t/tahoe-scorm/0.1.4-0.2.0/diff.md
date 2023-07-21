# Comparing `tmp/tahoe-scorm-0.1.4.tar.gz` & `tmp/tahoe-scorm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahoe-scorm-0.1.4.tar", last modified: Thu Jul 21 12:26:30 2022, max compression
+gzip compressed data, was "tahoe-scorm-0.2.0.tar", last modified: Fri Jul 21 21:06:49 2023, max compression
```

## Comparing `tahoe-scorm-0.1.4.tar` & `tahoe-scorm-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 12:26:30.802120 tahoe-scorm-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-07-21 12:26:17.000000 tahoe-scorm-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-07-21 12:26:30.802120 tahoe-scorm-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-07-21 12:26:17.000000 tahoe-scorm-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-21 12:26:30.802120 tahoe-scorm-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-07-21 12:26:17.000000 tahoe-scorm-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 12:26:30.802120 tahoe-scorm-0.1.4/tahoe_scorm/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 12:26:17.000000 tahoe-scorm-0.1.4/tahoe_scorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-07-21 12:26:17.000000 tahoe-scorm-0.1.4/tahoe_scorm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2221 2022-07-21 12:26:17.000000 tahoe-scorm-0.1.4/tahoe_scorm/storages.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 12:26:30.802120 tahoe-scorm-0.1.4/tahoe_scorm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-07-21 12:26:30.000000 tahoe-scorm-0.1.4/tahoe_scorm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-07-21 12:26:30.000000 tahoe-scorm-0.1.4/tahoe_scorm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 12:26:30.000000 tahoe-scorm-0.1.4/tahoe_scorm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-21 12:26:30.000000 tahoe-scorm-0.1.4/tahoe_scorm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:06:49.636787 tahoe-scorm-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-21 21:06:38.000000 tahoe-scorm-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-21 21:06:49.636787 tahoe-scorm-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-21 21:06:38.000000 tahoe-scorm-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 21:06:49.636787 tahoe-scorm-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-21 21:06:38.000000 tahoe-scorm-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:06:49.632787 tahoe-scorm-0.2.0/tahoe_scorm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:06:38.000000 tahoe-scorm-0.2.0/tahoe_scorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-21 21:06:38.000000 tahoe-scorm-0.2.0/tahoe_scorm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-21 21:06:38.000000 tahoe-scorm-0.2.0/tahoe_scorm/storages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:06:49.636787 tahoe-scorm-0.2.0/tahoe_scorm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-21 21:06:49.000000 tahoe-scorm-0.2.0/tahoe_scorm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-21 21:06:49.000000 tahoe-scorm-0.2.0/tahoe_scorm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 21:06:49.000000 tahoe-scorm-0.2.0/tahoe_scorm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 21:06:49.000000 tahoe-scorm-0.2.0/tahoe_scorm.egg-info/top_level.txt
```

### Comparing `tahoe-scorm-0.1.4/LICENSE` & `tahoe-scorm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tahoe-scorm-0.1.4/tahoe_scorm/storages.py` & `tahoe-scorm-0.2.0/tahoe_scorm/storages.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,49 +3,54 @@
 from .exceptions import ScormException
 
 
 def tahoe_scorm_storage(xblock):
     """
     Multi-tenant SCORM storage backend for overhangio/openedx-scorm-xblock. The
     following function returns a custom Django storages backend in which the
-    location is determined based on a combination of a settings and the
-    course_org_filter site settings.
+    location is determined based on a combination of a settings and,
+    by default, the course_org_filter site settings.
     The Tahoe default file storage backend is S3Boto3Storage, so is the one this
     function will return.
     """
     from django.conf import settings
     from django.core.files.storage import get_storage_class
     from openedx.core.djangoapps.appsembler.api.sites import get_site_for_course
 
-    # retrieve the site based on the course site id, it will work in the LMS and Studio as well.
-    current_site = get_site_for_course(xblock.course_id)
+    # in Tahoe we use 'storages.backends.s3boto3.S3Boto3Storage'
+    storage_class = get_storage_class(settings.DEFAULT_FILE_STORAGE)
 
     # the root dir inside the S3 bucket, configurable in global settings
     scorm_sub_folder = getattr(settings, "TAHOE_SCORM_XBLOCK_ROOT_DIR", None)
+
     if not scorm_sub_folder:
         raise ScormException(
             'TAHOE_SCORM_XBLOCK_ROOT_DIR is not defined in Django settings. '
             'Please fix it so tahoe_scorm_storage works.'
         )
 
-    # we use course organization id filter as customer SCORM folder
-    site_scorm_folder = str(xblock.course_id.org)
-
-    # in Tahoe we use 'storages.backends.s3boto3.S3Boto3Storage'
-    storage_class = get_storage_class(settings.DEFAULT_FILE_STORAGE)
-    storage_location = os.path.join(scorm_sub_folder, site_scorm_folder)
     # in order to allow CORS restrictions in the browser we need to use a custom
     # domain for the storage. Then in Nginx we have a proxy for the location,
     # but again, in order to allow CORS issues, if we browsing the content in
     # the LMS, the file must come from the LMS, and in Studio from Studio.
     # We cannot simply rely on settings for LMS and Studio URLs, because we need
     # to keep custom domains inside the ecuation.
-    if settings.SERVICE_VARIANT == "lms":
-        s3_custom_domain = current_site.domain
+    s3_custom_domain = settings.SITE_NAME
+
+    if getattr(settings, "TAHOE_SCORM_USE_COURSE_ORG_FOR_DOMAIN", True):
+        # retrieve the site based on the course site id, it will work in the LMS and Studio as well.
+        current_site = get_site_for_course(xblock.course_id)
+
+        # we use course organization id filter as customer SCORM folder
+        site_scorm_folder = str(xblock.course_id.org)
+        storage_location = os.path.join(scorm_sub_folder, site_scorm_folder)
+
+        if settings.SERVICE_VARIANT == "lms":
+            s3_custom_domain = current_site.domain
     else:
-        s3_custom_domain = settings.SITE_NAME
+        storage_location = scorm_sub_folder
 
     return storage_class(
         location=storage_location,
         default_acl='public-read',
         custom_domain=s3_custom_domain
     )
```

