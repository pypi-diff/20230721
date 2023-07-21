# Comparing `tmp/django-open-ai-0.0.3.tar.gz` & `tmp/django-open-ai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-open-ai-0.0.3.tar", last modified: Fri Jul 21 11:38:01 2023, max compression
+gzip compressed data, was "django-open-ai-0.0.4.tar", last modified: Fri Jul 21 12:15:51 2023, max compression
```

## Comparing `django-open-ai-0.0.3.tar` & `django-open-ai-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:38:01.156454 django-open-ai-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-21 11:37:44.000000 django-open-ai-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-21 11:38:01.156454 django-open-ai-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-21 11:37:44.000000 django-open-ai-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:38:01.156454 django-open-ai-0.0.3/django_open_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-21 11:38:01.000000 django-open-ai-0.0.3/django_open_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-21 11:38:01.000000 django-open-ai-0.0.3/django_open_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:38:01.000000 django-open-ai-0.0.3/django_open_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 11:38:01.000000 django-open-ai-0.0.3/django_open_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:38:01.000000 django-open-ai-0.0.3/django_open_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-21 11:38:01.160455 django-open-ai-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-21 11:37:44.000000 django-open-ai-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:15:51.566639 django-open-ai-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-21 12:15:51.566639 django-open-ai-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:15:51.566639 django-open-ai-0.0.4/django_open_ai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:15:51.566639 django-open-ai-0.0.4/django_open_ai/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:15:51.566639 django-open-ai-0.0.4/django_open_ai/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/django_open_ai/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:15:51.566639 django-open-ai-0.0.4/django_open_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-21 12:15:51.000000 django-open-ai-0.0.4/django_open_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-21 12:15:51.000000 django-open-ai-0.0.4/django_open_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:15:51.000000 django-open-ai-0.0.4/django_open_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-21 12:15:51.000000 django-open-ai-0.0.4/django_open_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 12:15:51.000000 django-open-ai-0.0.4/django_open_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-21 12:15:51.570639 django-open-ai-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-21 12:15:37.000000 django-open-ai-0.0.4/setup.py
```

### Comparing `django-open-ai-0.0.3/LICENSE` & `django-open-ai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-open-ai-0.0.3/setup.cfg` & `django-open-ai-0.0.4/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = django-open-ai
-version = 0.0.3
+version = 0.0.4
 description = Use the power of OpenAI on your Django database
-long_description = file:README.md
+long_description = file:README.rst
 url = https://github.com/PMCS64/django-open-ai
 license = MIT
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
@@ -16,13 +16,17 @@
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Software Development :: Libraries :: Application Frameworks
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 include_package_data = true
 python_requires = >=3.10
-install_requires = Django>=4.2
+install_requires = 
+	Django>=4.2
+	sqlalchemy>=2.0.19
+	openai>=0.27.8
+	langchain>=0.0.238
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

