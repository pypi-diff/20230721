# Comparing `tmp/marshmallow-3.9.0.tar.gz` & `tmp/marshmallow-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/marshmallow-3.9.0.tar", last modified: Sat Oct 31 18:24:04 2020, max compression
+gzip compressed data, was "dist/marshmallow-3.9.1.tar", last modified: Sun Nov  8 01:16:31 2020, max compression
```

## Comparing `marshmallow-3.9.0.tar` & `marshmallow-3.9.1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-10-31 18:24:04.000000 marshmallow-3.9.0/
--rw-r--r--   0 vsts      (1001) docker     (118)     8641 2020-10-31 18:23:52.000000 marshmallow-3.9.0/AUTHORS.rst
--rw-r--r--   0 vsts      (1001) docker     (118)    73931 2020-10-31 18:23:52.000000 marshmallow-3.9.0/CHANGELOG.rst
--rw-r--r--   0 vsts      (1001) docker     (118)     5326 2020-10-31 18:23:52.000000 marshmallow-3.9.0/CONTRIBUTING.rst
--rw-r--r--   0 vsts      (1001) docker     (118)     1069 2020-10-31 18:23:52.000000 marshmallow-3.9.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (118)      319 2020-10-31 18:23:52.000000 marshmallow-3.9.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (118)     1631 2020-10-31 18:23:52.000000 marshmallow-3.9.0/NOTICE
--rw-r--r--   0 vsts      (1001) docker     (118)     8154 2020-10-31 18:24:04.000000 marshmallow-3.9.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (118)     5506 2020-10-31 18:23:52.000000 marshmallow-3.9.0/README.rst
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-10-31 18:24:04.000000 marshmallow-3.9.0/docs/
--rw-r--r--   0 vsts      (1001) docker     (118)       35 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/.gitignore
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-10-31 18:24:04.000000 marshmallow-3.9.0/docs/_static/
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-10-31 18:24:04.000000 marshmallow-3.9.0/docs/_static/css/
--rw-r--r--   0 vsts      (1001) docker     (118)      693 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/_static/css/versionwarning.css
--rw-r--r--   0 vsts      (1001) docker     (118)    13908 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/_static/marshmallow-logo.png
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-10-31 18:24:04.000000 marshmallow-3.9.0/docs/_templates/
--rw-r--r--   0 vsts      (1001) docker     (118)     1021 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/_templates/donate.html
--rw-r--r--   0 vsts      (1001) docker     (118)      148 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/_templates/useful-links.html
--rw-r--r--   0 vsts      (1001) docker     (118)     1297 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/about.rst.inc
--rw-r--r--   0 vsts      (1001) docker     (118)      421 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/api_reference.rst
--rw-r--r--   0 vsts      (1001) docker     (118)       28 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/authors.rst
--rw-r--r--   0 vsts      (1001) docker     (118)      134 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/changelog.rst
--rw-r--r--   0 vsts      (1001) docker     (118)    10869 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/code_of_conduct.rst
--rw-r--r--   0 vsts      (1001) docker     (118)     3502 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/conf.py
--rw-r--r--   0 vsts      (1001) docker     (118)       33 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/contributing.rst
--rw-r--r--   0 vsts      (1001) docker     (118)     5836 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/custom_fields.rst
--rw-r--r--   0 vsts      (1001) docker     (118)      469 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/dashing.json
--rw-r--r--   0 vsts      (1001) docker     (118)      163 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/ecosystem.rst
--rw-r--r--   0 vsts      (1001) docker     (118)     8039 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/examples.rst
--rw-r--r--   0 vsts      (1001) docker     (118)    16289 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/extending.rst
--rw-r--r--   0 vsts      (1001) docker     (118)      981 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/index.rst
--rw-r--r--   0 vsts      (1001) docker     (118)      704 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/install.rst
--rw-r--r--   0 vsts      (1001) docker     (118)      325 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/kudos.rst
--rw-r--r--   0 vsts      (1001) docker     (118)       48 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/license.rst
--rw-r--r--   0 vsts      (1001) docker     (118)       88 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/marshmallow.class_registry.rst
--rw-r--r--   0 vsts      (1001) docker     (118)       94 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/marshmallow.decorators.rst
--rw-r--r--   0 vsts      (1001) docker     (118)      101 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/marshmallow.error_store.rst
--rw-r--r--   0 vsts      (1001) docker     (118)       76 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/marshmallow.exceptions.rst
--rw-r--r--   0 vsts      (1001) docker     (118)      121 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/marshmallow.fields.rst
--rw-r--r--   0 vsts      (1001) docker     (118)      144 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/marshmallow.schema.rst
--rw-r--r--   0 vsts      (1001) docker     (118)       85 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/marshmallow.utils.rst
--rw-r--r--   0 vsts      (1001) docker     (118)      113 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/marshmallow.validate.rst
--rw-r--r--   0 vsts      (1001) docker     (118)     9035 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/nesting.rst
--rw-r--r--   0 vsts      (1001) docker     (118)    18084 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/quickstart.rst
--rw-r--r--   0 vsts      (1001) docker     (118)    53710 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/upgrading.rst
--rw-r--r--   0 vsts      (1001) docker     (118)      271 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/whos_using.rst
--rw-r--r--   0 vsts      (1001) docker     (118)     5504 2020-10-31 18:23:52.000000 marshmallow-3.9.0/docs/why.rst
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-10-31 18:24:04.000000 marshmallow-3.9.0/examples/
--rw-r--r--   0 vsts      (1001) docker     (118)     4096 2020-10-31 18:23:52.000000 marshmallow-3.9.0/examples/flask_example.py
--rw-r--r--   0 vsts      (1001) docker     (118)      888 2020-10-31 18:23:52.000000 marshmallow-3.9.0/examples/inflection_example.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1463 2020-10-31 18:23:52.000000 marshmallow-3.9.0/examples/package_json_example.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5381 2020-10-31 18:23:52.000000 marshmallow-3.9.0/examples/peewee_example.py
--rw-r--r--   0 vsts      (1001) docker     (118)      823 2020-10-31 18:23:52.000000 marshmallow-3.9.0/examples/textblob_example.py
--rw-r--r--   0 vsts      (1001) docker     (118)       80 2020-10-31 18:23:52.000000 marshmallow-3.9.0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (118)      461 2020-10-31 18:24:04.000000 marshmallow-3.9.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (118)     2832 2020-10-31 18:23:52.000000 marshmallow-3.9.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-10-31 18:24:04.000000 marshmallow-3.9.0/src/
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-10-31 18:24:04.000000 marshmallow-3.9.0/src/marshmallow/
--rw-r--r--   0 vsts      (1001) docker     (118)      716 2020-10-31 18:23:52.000000 marshmallow-3.9.0/src/marshmallow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1320 2020-10-31 18:23:52.000000 marshmallow-3.9.0/src/marshmallow/base.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2836 2020-10-31 18:23:52.000000 marshmallow-3.9.0/src/marshmallow/class_registry.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7500 2020-10-31 18:23:52.000000 marshmallow-3.9.0/src/marshmallow/decorators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2223 2020-10-31 18:23:52.000000 marshmallow-3.9.0/src/marshmallow/error_store.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2192 2020-10-31 18:23:52.000000 marshmallow-3.9.0/src/marshmallow/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (118)    65279 2020-10-31 18:23:52.000000 marshmallow-3.9.0/src/marshmallow/fields.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2940 2020-10-31 18:23:52.000000 marshmallow-3.9.0/src/marshmallow/orderedset.py
--rw-r--r--   0 vsts      (1001) docker     (118)    49619 2020-10-31 18:23:52.000000 marshmallow-3.9.0/src/marshmallow/schema.py
--rw-r--r--   0 vsts      (1001) docker     (118)      269 2020-10-31 18:23:52.000000 marshmallow-3.9.0/src/marshmallow/types.py
--rw-r--r--   0 vsts      (1001) docker     (118)    10153 2020-10-31 18:23:52.000000 marshmallow-3.9.0/src/marshmallow/utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)    20647 2020-10-31 18:23:52.000000 marshmallow-3.9.0/src/marshmallow/validate.py
--rw-r--r--   0 vsts      (1001) docker     (118)       65 2020-10-31 18:23:52.000000 marshmallow-3.9.0/src/marshmallow/warnings.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-10-31 18:24:04.000000 marshmallow-3.9.0/src/marshmallow.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (118)     8154 2020-10-31 18:24:03.000000 marshmallow-3.9.0/src/marshmallow.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (118)     1977 2020-10-31 18:24:03.000000 marshmallow-3.9.0/src/marshmallow.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (118)        1 2020-10-31 18:24:03.000000 marshmallow-3.9.0/src/marshmallow.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (118)        1 2020-10-31 18:24:03.000000 marshmallow-3.9.0/src/marshmallow.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (118)      314 2020-10-31 18:24:03.000000 marshmallow-3.9.0/src/marshmallow.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (118)       12 2020-10-31 18:24:03.000000 marshmallow-3.9.0/src/marshmallow.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-10-31 18:24:04.000000 marshmallow-3.9.0/tests/
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2020-10-31 18:23:52.000000 marshmallow-3.9.0/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8180 2020-10-31 18:23:52.000000 marshmallow-3.9.0/tests/base.py
--rw-r--r--   0 vsts      (1001) docker     (118)      565 2020-10-31 18:23:52.000000 marshmallow-3.9.0/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (118)       97 2020-10-31 18:23:52.000000 marshmallow-3.9.0/tests/foo_serializer.py
--rw-r--r--   0 vsts      (1001) docker     (118)    30937 2020-10-31 18:23:52.000000 marshmallow-3.9.0/tests/test_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (118)    74413 2020-10-31 18:23:52.000000 marshmallow-3.9.0/tests/test_deserialization.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5137 2020-10-31 18:23:52.000000 marshmallow-3.9.0/tests/test_error_store.py
--rw-r--r--   0 vsts      (1001) docker     (118)      887 2020-10-31 18:23:52.000000 marshmallow-3.9.0/tests/test_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (118)    20929 2020-10-31 18:23:52.000000 marshmallow-3.9.0/tests/test_fields.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7586 2020-10-31 18:23:52.000000 marshmallow-3.9.0/tests/test_options.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6909 2020-10-31 18:23:52.000000 marshmallow-3.9.0/tests/test_registry.py
--rw-r--r--   0 vsts      (1001) docker     (118)    91752 2020-10-31 18:23:52.000000 marshmallow-3.9.0/tests/test_schema.py
--rw-r--r--   0 vsts      (1001) docker     (118)    32041 2020-10-31 18:23:52.000000 marshmallow-3.9.0/tests/test_serialization.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7100 2020-10-31 18:23:52.000000 marshmallow-3.9.0/tests/test_utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)    29903 2020-10-31 18:23:52.000000 marshmallow-3.9.0/tests/test_validate.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-11-08 01:16:31.000000 marshmallow-3.9.1/
+-rw-r--r--   0 vsts      (1001) docker     (118)     8641 2020-11-08 01:16:22.000000 marshmallow-3.9.1/AUTHORS.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)    74197 2020-11-08 01:16:22.000000 marshmallow-3.9.1/CHANGELOG.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)     5326 2020-11-08 01:16:22.000000 marshmallow-3.9.1/CONTRIBUTING.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)     1069 2020-11-08 01:16:22.000000 marshmallow-3.9.1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (118)      319 2020-11-08 01:16:22.000000 marshmallow-3.9.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (118)     1631 2020-11-08 01:16:22.000000 marshmallow-3.9.1/NOTICE
+-rw-r--r--   0 vsts      (1001) docker     (118)     8154 2020-11-08 01:16:31.000000 marshmallow-3.9.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (118)     5506 2020-11-08 01:16:22.000000 marshmallow-3.9.1/README.rst
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-11-08 01:16:31.000000 marshmallow-3.9.1/docs/
+-rw-r--r--   0 vsts      (1001) docker     (118)       35 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/.gitignore
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-11-08 01:16:31.000000 marshmallow-3.9.1/docs/_static/
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-11-08 01:16:31.000000 marshmallow-3.9.1/docs/_static/css/
+-rw-r--r--   0 vsts      (1001) docker     (118)      696 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/_static/css/versionwarning.css
+-rw-r--r--   0 vsts      (1001) docker     (118)    13908 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/_static/marshmallow-logo.png
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-11-08 01:16:31.000000 marshmallow-3.9.1/docs/_templates/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1021 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/_templates/donate.html
+-rw-r--r--   0 vsts      (1001) docker     (118)      148 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/_templates/useful-links.html
+-rw-r--r--   0 vsts      (1001) docker     (118)     1297 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/about.rst.inc
+-rw-r--r--   0 vsts      (1001) docker     (118)      421 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/api_reference.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)       28 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/authors.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)      134 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/changelog.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)    10869 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/code_of_conduct.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)     3183 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/conf.py
+-rw-r--r--   0 vsts      (1001) docker     (118)       33 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/contributing.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)     5836 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/custom_fields.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)      469 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/dashing.json
+-rw-r--r--   0 vsts      (1001) docker     (118)      163 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/ecosystem.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)     8039 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/examples.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)    16289 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/extending.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)      981 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)      704 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/install.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)      325 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/kudos.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)       48 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/license.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)       88 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/marshmallow.class_registry.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)       94 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/marshmallow.decorators.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)      101 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/marshmallow.error_store.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)       76 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/marshmallow.exceptions.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)      121 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/marshmallow.fields.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)      144 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/marshmallow.schema.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)       85 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/marshmallow.utils.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)      113 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/marshmallow.validate.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)     9035 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/nesting.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)    18084 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/quickstart.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)    53710 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/upgrading.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)      271 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/whos_using.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)     5504 2020-11-08 01:16:22.000000 marshmallow-3.9.1/docs/why.rst
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-11-08 01:16:31.000000 marshmallow-3.9.1/examples/
+-rw-r--r--   0 vsts      (1001) docker     (118)     4096 2020-11-08 01:16:22.000000 marshmallow-3.9.1/examples/flask_example.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      888 2020-11-08 01:16:22.000000 marshmallow-3.9.1/examples/inflection_example.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1463 2020-11-08 01:16:22.000000 marshmallow-3.9.1/examples/package_json_example.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5381 2020-11-08 01:16:22.000000 marshmallow-3.9.1/examples/peewee_example.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      823 2020-11-08 01:16:22.000000 marshmallow-3.9.1/examples/textblob_example.py
+-rw-r--r--   0 vsts      (1001) docker     (118)       80 2020-11-08 01:16:22.000000 marshmallow-3.9.1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (118)      461 2020-11-08 01:16:31.000000 marshmallow-3.9.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (118)     2832 2020-11-08 01:16:22.000000 marshmallow-3.9.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-11-08 01:16:31.000000 marshmallow-3.9.1/src/
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-11-08 01:16:31.000000 marshmallow-3.9.1/src/marshmallow/
+-rw-r--r--   0 vsts      (1001) docker     (118)      716 2020-11-08 01:16:22.000000 marshmallow-3.9.1/src/marshmallow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1320 2020-11-08 01:16:22.000000 marshmallow-3.9.1/src/marshmallow/base.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2836 2020-11-08 01:16:22.000000 marshmallow-3.9.1/src/marshmallow/class_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7500 2020-11-08 01:16:22.000000 marshmallow-3.9.1/src/marshmallow/decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2223 2020-11-08 01:16:22.000000 marshmallow-3.9.1/src/marshmallow/error_store.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2192 2020-11-08 01:16:22.000000 marshmallow-3.9.1/src/marshmallow/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    65419 2020-11-08 01:16:22.000000 marshmallow-3.9.1/src/marshmallow/fields.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2940 2020-11-08 01:16:22.000000 marshmallow-3.9.1/src/marshmallow/orderedset.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    49619 2020-11-08 01:16:22.000000 marshmallow-3.9.1/src/marshmallow/schema.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      269 2020-11-08 01:16:22.000000 marshmallow-3.9.1/src/marshmallow/types.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    10241 2020-11-08 01:16:22.000000 marshmallow-3.9.1/src/marshmallow/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    20676 2020-11-08 01:16:22.000000 marshmallow-3.9.1/src/marshmallow/validate.py
+-rw-r--r--   0 vsts      (1001) docker     (118)       65 2020-11-08 01:16:22.000000 marshmallow-3.9.1/src/marshmallow/warnings.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-11-08 01:16:31.000000 marshmallow-3.9.1/src/marshmallow.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (118)     8154 2020-11-08 01:16:31.000000 marshmallow-3.9.1/src/marshmallow.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (118)     1977 2020-11-08 01:16:31.000000 marshmallow-3.9.1/src/marshmallow.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)        1 2020-11-08 01:16:31.000000 marshmallow-3.9.1/src/marshmallow.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)        1 2020-11-08 01:16:31.000000 marshmallow-3.9.1/src/marshmallow.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (118)      314 2020-11-08 01:16:31.000000 marshmallow-3.9.1/src/marshmallow.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)       12 2020-11-08 01:16:31.000000 marshmallow-3.9.1/src/marshmallow.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-11-08 01:16:31.000000 marshmallow-3.9.1/tests/
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2020-11-08 01:16:22.000000 marshmallow-3.9.1/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8180 2020-11-08 01:16:22.000000 marshmallow-3.9.1/tests/base.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      565 2020-11-08 01:16:22.000000 marshmallow-3.9.1/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (118)       97 2020-11-08 01:16:22.000000 marshmallow-3.9.1/tests/foo_serializer.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    30937 2020-11-08 01:16:22.000000 marshmallow-3.9.1/tests/test_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    74559 2020-11-08 01:16:22.000000 marshmallow-3.9.1/tests/test_deserialization.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5137 2020-11-08 01:16:22.000000 marshmallow-3.9.1/tests/test_error_store.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      887 2020-11-08 01:16:22.000000 marshmallow-3.9.1/tests/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    20929 2020-11-08 01:16:22.000000 marshmallow-3.9.1/tests/test_fields.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7586 2020-11-08 01:16:22.000000 marshmallow-3.9.1/tests/test_options.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6909 2020-11-08 01:16:22.000000 marshmallow-3.9.1/tests/test_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    91647 2020-11-08 01:16:22.000000 marshmallow-3.9.1/tests/test_schema.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    31938 2020-11-08 01:16:22.000000 marshmallow-3.9.1/tests/test_serialization.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7100 2020-11-08 01:16:22.000000 marshmallow-3.9.1/tests/test_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    29903 2020-11-08 01:16:22.000000 marshmallow-3.9.1/tests/test_validate.py
```

### Comparing `marshmallow-3.9.0/AUTHORS.rst` & `marshmallow-3.9.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/CHANGELOG.rst` & `marshmallow-3.9.1/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 ---------
 
+3.9.1 (2020-11-07)
+******************
+
+Bug fixes:
+
+- Cast to mapping type in ``Mapping.serialize`` and ``Mapping.deserialize``
+  (:pr:`1685`).
+- Fix bug letting ``Dict`` pass invalid dict on deserialization when no key or
+  value ``Field`` is specified (:pr:`1685`).
+
 3.9.0 (2020-10-31)
 ******************
 
 Features:
 
 - Add ``format`` argument to ``fields.Time`` and ``timeformat`` *class Meta* option (:issue:`686`).
   Thanks :user:`BennyAlex` for the suggestion and thanks :user:`infinityxxx` for the PR.
@@ -65,15 +75,15 @@
   add summary tables (:pr:`1587`). Thanks :user:`EpicWink` for the PR.
 
 3.6.0 (2020-05-08)
 ******************
 
 Features:
 
-- Add ``validators.ContainsNoneOf`` (:issue:`1528`).
+- Add ``validate.ContainsNoneOf`` (:issue:`1528`).
   Thanks :user:`Resinderate` for the suggestion and the PR.
 
 
 3.5.2 (2020-04-30)
 ******************
 
 Bug fixes:
```

### Comparing `marshmallow-3.9.0/CONTRIBUTING.rst` & `marshmallow-3.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/LICENSE` & `marshmallow-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/NOTICE` & `marshmallow-3.9.1/NOTICE`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/PKG-INFO` & `marshmallow-3.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marshmallow
-Version: 3.9.0
+Version: 3.9.1
 Summary: A lightweight library for converting complex datatypes to and from native Python datatypes.
 Home-page: https://github.com/marshmallow-code/marshmallow
 Author: Steven Loria
 Author-email: sloria1@gmail.com
 License: MIT
 Project-URL: Changelog, https://marshmallow.readthedocs.io/en/latest/changelog.html
 Project-URL: Issues, https://github.com/marshmallow-code/marshmallow/issues
```

### Comparing `marshmallow-3.9.0/README.rst` & `marshmallow-3.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/docs/_static/css/versionwarning.css` & `marshmallow-3.9.1/docs/_static/css/versionwarning.css`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
   letter-spacing: 1px;
   color: #fff;
   text-shadow: 0 0 2px #000;
   text-align: center;
   font-size: 0.9em;
 
-  background: #000
+  background: #004b6b
     repeating-linear-gradient(
       135deg,
       transparent,
       transparent 20px,
       rgba(255, 255, 255, 0.1) 20px,
       rgba(255, 255, 255, 0.1) 40px
     );
```

### Comparing `marshmallow-3.9.0/docs/_static/marshmallow-logo.png` & `marshmallow-3.9.1/docs/_static/marshmallow-logo.png`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/docs/_templates/donate.html` & `marshmallow-3.9.1/docs/_templates/donate.html`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/docs/about.rst.inc` & `marshmallow-3.9.1/docs/about.rst.inc`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/docs/code_of_conduct.rst` & `marshmallow-3.9.1/docs/code_of_conduct.rst`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/docs/conf.py` & `marshmallow-3.9.1/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,161 +59,141 @@
 000003a0: 7569 6c64 225d 0a0a 2320 5448 454d 450a  uild"]..# THEME.
 000003b0: 0a68 746d 6c5f 7468 656d 655f 7061 7468  .html_theme_path
 000003c0: 203d 205b 616c 6162 6173 7465 722e 6765   = [alabaster.ge
 000003d0: 745f 7061 7468 2829 5d0a 6874 6d6c 5f74  t_path()].html_t
 000003e0: 6865 6d65 203d 2022 616c 6162 6173 7465  heme = "alabaste
 000003f0: 7222 0a68 746d 6c5f 7374 6174 6963 5f70  r".html_static_p
 00000400: 6174 6820 3d20 5b22 5f73 7461 7469 6322  ath = ["_static"
-00000410: 5d0a 7465 6d70 6c61 7465 735f 7061 7468  ].templates_path
-00000420: 203d 205b 225f 7465 6d70 6c61 7465 7322   = ["_templates"
-00000430: 5d0a 6874 6d6c 5f73 686f 775f 736f 7572  ].html_show_sour
-00000440: 6365 6c69 6e6b 203d 2046 616c 7365 0a0a  celink = False..
-00000450: 6874 6d6c 5f74 6865 6d65 5f6f 7074 696f  html_theme_optio
-00000460: 6e73 203d 207b 0a20 2020 2022 6c6f 676f  ns = {.    "logo
-00000470: 223a 2022 6d61 7273 686d 616c 6c6f 772d  ": "marshmallow-
-00000480: 6c6f 676f 2e70 6e67 222c 0a20 2020 2022  logo.png",.    "
-00000490: 6465 7363 7269 7074 696f 6e22 3a20 224f  description": "O
-000004a0: 626a 6563 7420 7365 7269 616c 697a 6174  bject serializat
-000004b0: 696f 6e20 616e 6420 6465 7365 7269 616c  ion and deserial
-000004c0: 697a 6174 696f 6e2c 206c 6967 6874 7765  ization, lightwe
-000004d0: 6967 6874 2061 6e64 2066 6c75 6666 792e  ight and fluffy.
-000004e0: 222c 0a20 2020 2022 6465 7363 7269 7074  ",.    "descript
-000004f0: 696f 6e5f 666f 6e74 5f73 7479 6c65 223a  ion_font_style":
-00000500: 2022 6974 616c 6963 222c 0a20 2020 2022   "italic",.    "
-00000510: 6769 7468 7562 5f75 7365 7222 3a20 226d  github_user": "m
-00000520: 6172 7368 6d61 6c6c 6f77 2d63 6f64 6522  arshmallow-code"
-00000530: 2c0a 2020 2020 2267 6974 6875 625f 7265  ,.    "github_re
-00000540: 706f 223a 2022 6d61 7273 686d 616c 6c6f  po": "marshmallo
-00000550: 7722 2c0a 2020 2020 2267 6974 6875 625f  w",.    "github_
-00000560: 6261 6e6e 6572 223a 2054 7275 652c 0a20  banner": True,. 
-00000570: 2020 2022 6769 7468 7562 5f74 7970 6522     "github_type"
-00000580: 3a20 2273 7461 7222 2c0a 2020 2020 226f  : "star",.    "o
-00000590: 7065 6e63 6f6c 6c65 6374 6976 6522 3a20  pencollective": 
-000005a0: 226d 6172 7368 6d61 6c6c 6f77 222c 0a20  "marshmallow",. 
-000005b0: 2020 2022 7469 6465 6c69 6674 5f75 726c     "tidelift_url
-000005c0: 223a 2028 0a20 2020 2020 2020 2022 6874  ": (.        "ht
-000005d0: 7470 733a 2f2f 7469 6465 6c69 6674 2e63  tps://tidelift.c
-000005e0: 6f6d 2f73 7562 7363 7269 7074 696f 6e2f  om/subscription/
-000005f0: 706b 672f 7079 7069 2d6d 6172 7368 6d61  pkg/pypi-marshma
-00000600: 6c6c 6f77 220a 2020 2020 2020 2020 223f  llow".        "?
-00000610: 7574 6d5f 736f 7572 6365 3d6d 6172 7368  utm_source=marsh
-00000620: 6d61 6c6c 6f77 2675 746d 5f6d 6564 6975  mallow&utm_mediu
-00000630: 6d3d 7265 6665 7272 616c 2675 746d 5f63  m=referral&utm_c
-00000640: 616d 7061 6967 6e3d 646f 6373 220a 2020  ampaign=docs".  
-00000650: 2020 292c 0a20 2020 2022 636f 6465 5f66    ),.    "code_f
-00000660: 6f6e 745f 7369 7a65 223a 2022 302e 3865  ont_size": "0.8e
-00000670: 6d22 2c0a 2020 2020 2277 6172 6e5f 6267  m",.    "warn_bg
-00000680: 223a 2022 2346 4643 222c 0a20 2020 2022  ": "#FFC",.    "
-00000690: 7761 726e 5f62 6f72 6465 7222 3a20 2223  warn_border": "#
-000006a0: 4545 4522 2c0a 2020 2020 2320 5573 6564  EEE",.    # Used
-000006b0: 2074 6f20 706f 7075 6c61 7465 2074 6865   to populate the
-000006c0: 2075 7365 6675 6c2d 6c69 6e6b 732e 6874   useful-links.ht
-000006d0: 6d6c 2074 656d 706c 6174 650a 2020 2020  ml template.    
-000006e0: 2265 7874 7261 5f6e 6176 5f6c 696e 6b73  "extra_nav_links
-000006f0: 223a 204f 7264 6572 6564 4469 6374 280a  ": OrderedDict(.
-00000700: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
-00000710: 2020 2020 2020 2822 6d61 7273 686d 616c        ("marshmal
-00000720: 6c6f 7720 4020 5079 5049 222c 2022 6874  low @ PyPI", "ht
-00000730: 7470 733a 2f2f 7079 7069 2e70 7974 686f  tps://pypi.pytho
-00000740: 6e2e 6f72 672f 7079 7069 2f6d 6172 7368  n.org/pypi/marsh
-00000750: 6d61 6c6c 6f77 2229 2c0a 2020 2020 2020  mallow"),.      
-00000760: 2020 2020 2020 2822 6d61 7273 686d 616c        ("marshmal
-00000770: 6c6f 7720 4020 4769 7448 7562 222c 2022  low @ GitHub", "
-00000780: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000790: 6f6d 2f6d 6172 7368 6d61 6c6c 6f77 2d63  om/marshmallow-c
-000007a0: 6f64 652f 6d61 7273 686d 616c 6c6f 7722  ode/marshmallow"
-000007b0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-000007c0: 2249 7373 7565 2054 7261 636b 6572 222c  "Issue Tracker",
-000007d0: 2022 6874 7470 733a 2f2f 6769 7468 7562   "https://github
-000007e0: 2e63 6f6d 2f6d 6172 7368 6d61 6c6c 6f77  .com/marshmallow
-000007f0: 2d63 6f64 652f 6d61 7273 686d 616c 6c6f  -code/marshmallo
-00000800: 772f 6973 7375 6573 2229 2c0a 2020 2020  w/issues"),.    
-00000810: 2020 2020 2020 2020 280a 2020 2020 2020          (.      
-00000820: 2020 2020 2020 2020 2020 2245 636f 7379            "Ecosy
-00000830: 7374 656d 222c 0a20 2020 2020 2020 2020  stem",.         
-00000840: 2020 2020 2020 2022 6874 7470 733a 2f2f         "https://
-00000850: 6769 7468 7562 2e63 6f6d 2f6d 6172 7368  github.com/marsh
-00000860: 6d61 6c6c 6f77 2d63 6f64 652f 6d61 7273  mallow-code/mars
-00000870: 686d 616c 6c6f 772f 7769 6b69 2f45 636f  hmallow/wiki/Eco
-00000880: 7379 7374 656d 222c 0a20 2020 2020 2020  system",.       
-00000890: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-000008a0: 5d0a 2020 2020 292c 0a7d 0a0a 6874 6d6c  ].    ),.}..html
-000008b0: 5f73 6964 6562 6172 7320 3d20 7b0a 2020  _sidebars = {.  
-000008c0: 2020 2269 6e64 6578 223a 205b 2261 626f    "index": ["abo
-000008d0: 7574 2e68 746d 6c22 2c20 2264 6f6e 6174  ut.html", "donat
-000008e0: 652e 6874 6d6c 222c 2022 7573 6566 756c  e.html", "useful
-000008f0: 2d6c 696e 6b73 2e68 746d 6c22 2c20 2273  -links.html", "s
-00000900: 6561 7263 6862 6f78 2e68 746d 6c22 5d2c  earchbox.html"],
-00000910: 0a20 2020 2022 2a2a 223a 205b 0a20 2020  .    "**": [.   
-00000920: 2020 2020 2022 6162 6f75 742e 6874 6d6c       "about.html
-00000930: 222c 0a20 2020 2020 2020 2022 646f 6e61  ",.        "dona
-00000940: 7465 2e68 746d 6c22 2c0a 2020 2020 2020  te.html",.      
-00000950: 2020 2275 7365 6675 6c2d 6c69 6e6b 732e    "useful-links.
-00000960: 6874 6d6c 222c 0a20 2020 2020 2020 2022  html",.        "
-00000970: 6c6f 6361 6c74 6f63 2e68 746d 6c22 2c0a  localtoc.html",.
-00000980: 2020 2020 2020 2020 2272 656c 6174 696f          "relatio
-00000990: 6e73 2e68 746d 6c22 2c0a 2020 2020 2020  ns.html",.      
-000009a0: 2020 2273 6561 7263 6862 6f78 2e68 746d    "searchbox.htm
-000009b0: 6c22 2c0a 2020 2020 5d2c 0a7d 0a0a 2320  l",.    ],.}..# 
-000009c0: 7370 6869 6e78 2d76 6572 7369 6f6e 2d77  sphinx-version-w
-000009d0: 6172 6e69 6e67 2063 6f6e 6669 670a 7665  arning config.ve
-000009e0: 7273 696f 6e77 6172 6e69 6e67 5f6d 6573  rsionwarning_mes
-000009f0: 7361 6765 7320 3d20 7b0a 2020 2020 226c  sages = {.    "l
-00000a00: 6174 6573 7422 3a20 280a 2020 2020 2020  atest": (.      
-00000a10: 2020 2254 6869 7320 646f 6375 6d65 6e74    "This document
-00000a20: 2069 7320 666f 7220 7468 6520 6465 7665   is for the deve
-00000a30: 6c6f 706d 656e 7420 7665 7273 696f 6e2e  lopment version.
-00000a40: 2022 0a20 2020 2020 2020 2027 466f 7220   ".        'For 
-00000a50: 7468 6520 7374 6162 6c65 2076 6572 7369  the stable versi
-00000a60: 6f6e 2064 6f63 756d 656e 7461 7469 6f6e  on documentation
-00000a70: 2c20 7365 6520 3c61 2068 7265 663d 222f  , see <a href="/
-00000a80: 656e 2f73 7461 626c 652f 223e 6865 7265  en/stable/">here
-00000a90: 3c2f 613e 2e27 0a20 2020 2029 2c0a 2020  </a>.'.    ),.  
-00000aa0: 2020 2273 7461 626c 6522 3a20 280a 2020    "stable": (.  
-00000ab0: 2020 2020 2020 223c 7374 726f 6e67 3e42        "<strong>B
-00000ac0: 6c61 636b 204c 6976 6573 204d 6174 7465  lack Lives Matte
-00000ad0: 722e 3c2f 7374 726f 6e67 3e20 220a 2020  r.</strong> ".  
-00000ae0: 2020 2020 2020 2753 7570 706f 7274 2074        'Support t
-00000af0: 6865 203c 6120 6872 6566 3d22 6874 7470  he <a href="http
-00000b00: 733a 2f2f 656a 692e 6f72 672f 223e 4571  s://eji.org/">Eq
-00000b10: 7561 6c20 4a75 7374 6963 6520 496e 6974  ual Justice Init
-00000b20: 6961 7469 7665 3c2f 613e 2061 6e64 2027  iative</a> and '
-00000b30: 0a20 2020 2020 2020 2027 3c61 2068 7265  .        '<a hre
-00000b40: 663d 2268 7474 7073 3a2f 2f63 6f6c 6f72  f="https://color
-00000b50: 6f66 6368 616e 6765 2e6f 7267 2f22 3e43  ofchange.org/">C
-00000b60: 6f6c 6f72 206f 6620 4368 616e 6765 3c2f  olor of Change</
-00000b70: 613e 2e27 0a20 2020 2029 2c0a 2020 2020  a>.'.    ),.    
-00000b80: 2232 2e78 2d6c 696e 6522 3a20 280a 2020  "2.x-line": (.  
-00000b90: 2020 2020 2020 226d 6172 7368 6d61 6c6c        "marshmall
-00000ba0: 6f77 2032 2069 7320 6e6f 206c 6f6e 6765  ow 2 is no longe
-00000bb0: 7220 7375 7070 6f72 7465 6420 6173 206f  r supported as o
-00000bc0: 6620 3230 3230 2d30 382d 3138 2e20 220a  f 2020-08-18. ".
-00000bd0: 2020 2020 2020 2020 273c 6120 6872 6566          '<a href
-00000be0: 3d22 6874 7470 733a 2f2f 6d61 7273 686d  ="https://marshm
-00000bf0: 616c 6c6f 772e 7265 6164 7468 6564 6f63  allow.readthedoc
-00000c00: 732e 696f 2f65 6e2f 6c61 7465 7374 2f75  s.io/en/latest/u
-00000c10: 7067 7261 6469 6e67 2e68 746d 6c23 7570  pgrading.html#up
-00000c20: 6772 6164 696e 672d 746f 2d33 2d30 223e  grading-to-3-0">
-00000c30: 270a 2020 2020 2020 2020 2255 7064 6174  '.        "Updat
-00000c40: 6520 796f 7572 2063 6f64 6520 746f 2075  e your code to u
-00000c50: 7365 206d 6172 7368 6d61 6c6c 6f77 2033  se marshmallow 3
-00000c60: 3c2f 613e 2e22 0a20 2020 2029 2c0a 7d0a  </a>.".    ),.}.
-00000c70: 2320 5368 6f77 2077 6172 6e69 6e67 2061  # Show warning a
-00000c80: 7420 746f 7020 6f66 2070 6167 650a 7665  t top of page.ve
-00000c90: 7273 696f 6e77 6172 6e69 6e67 5f62 6f64  rsionwarning_bod
-00000ca0: 795f 7365 6c65 6374 6f72 203d 2022 6469  y_selector = "di
-00000cb0: 762e 646f 6375 6d65 6e74 220a 7665 7273  v.document".vers
-00000cc0: 696f 6e77 6172 6e69 6e67 5f62 616e 6e65  ionwarning_banne
-00000cd0: 725f 7469 746c 6520 3d20 2222 0a23 2046  r_title = "".# F
-00000ce0: 6f72 2064 6562 7567 6769 6e67 206c 6f63  or debugging loc
-00000cf0: 616c 6c79 0a23 2076 6572 7369 6f6e 7761  ally.# versionwa
-00000d00: 726e 696e 675f 7072 6f6a 6563 745f 7665  rning_project_ve
-00000d10: 7273 696f 6e20 3d20 2273 7461 626c 6522  rsion = "stable"
-00000d20: 0a0a 0a64 6566 2073 6574 7570 2861 7070  ...def setup(app
-00000d30: 293a 0a20 2020 2023 2068 7474 7073 3a2f  ):.    # https:/
-00000d40: 2f64 6f63 732e 7265 6164 7468 6564 6f63  /docs.readthedoc
-00000d50: 732e 696f 2f65 6e2f 6c61 7465 7374 2f67  s.io/en/latest/g
-00000d60: 7569 6465 732f 6164 6469 6e67 2d63 7573  uides/adding-cus
-00000d70: 746f 6d2d 6373 732e 6874 6d6c 0a20 2020  tom-css.html.   
-00000d80: 2061 7070 2e61 6464 5f73 7479 6c65 7368   app.add_stylesh
-00000d90: 6565 7428 2263 7373 2f76 6572 7369 6f6e  eet("css/version
-00000da0: 7761 726e 696e 672e 6373 7322 290a       warning.css").
+00000410: 5d0a 6874 6d6c 5f63 7373 5f66 696c 6573  ].html_css_files
+00000420: 203d 205b 2263 7373 2f76 6572 7369 6f6e   = ["css/version
+00000430: 7761 726e 696e 672e 6373 7322 5d0a 7465  warning.css"].te
+00000440: 6d70 6c61 7465 735f 7061 7468 203d 205b  mplates_path = [
+00000450: 225f 7465 6d70 6c61 7465 7322 5d0a 6874  "_templates"].ht
+00000460: 6d6c 5f73 686f 775f 736f 7572 6365 6c69  ml_show_sourceli
+00000470: 6e6b 203d 2046 616c 7365 0a0a 6874 6d6c  nk = False..html
+00000480: 5f74 6865 6d65 5f6f 7074 696f 6e73 203d  _theme_options =
+00000490: 207b 0a20 2020 2022 6c6f 676f 223a 2022   {.    "logo": "
+000004a0: 6d61 7273 686d 616c 6c6f 772d 6c6f 676f  marshmallow-logo
+000004b0: 2e70 6e67 222c 0a20 2020 2022 6465 7363  .png",.    "desc
+000004c0: 7269 7074 696f 6e22 3a20 224f 626a 6563  ription": "Objec
+000004d0: 7420 7365 7269 616c 697a 6174 696f 6e20  t serialization 
+000004e0: 616e 6420 6465 7365 7269 616c 697a 6174  and deserializat
+000004f0: 696f 6e2c 206c 6967 6874 7765 6967 6874  ion, lightweight
+00000500: 2061 6e64 2066 6c75 6666 792e 222c 0a20   and fluffy.",. 
+00000510: 2020 2022 6465 7363 7269 7074 696f 6e5f     "description_
+00000520: 666f 6e74 5f73 7479 6c65 223a 2022 6974  font_style": "it
+00000530: 616c 6963 222c 0a20 2020 2022 6769 7468  alic",.    "gith
+00000540: 7562 5f75 7365 7222 3a20 226d 6172 7368  ub_user": "marsh
+00000550: 6d61 6c6c 6f77 2d63 6f64 6522 2c0a 2020  mallow-code",.  
+00000560: 2020 2267 6974 6875 625f 7265 706f 223a    "github_repo":
+00000570: 2022 6d61 7273 686d 616c 6c6f 7722 2c0a   "marshmallow",.
+00000580: 2020 2020 2267 6974 6875 625f 6261 6e6e      "github_bann
+00000590: 6572 223a 2054 7275 652c 0a20 2020 2022  er": True,.    "
+000005a0: 6769 7468 7562 5f74 7970 6522 3a20 2273  github_type": "s
+000005b0: 7461 7222 2c0a 2020 2020 226f 7065 6e63  tar",.    "openc
+000005c0: 6f6c 6c65 6374 6976 6522 3a20 226d 6172  ollective": "mar
+000005d0: 7368 6d61 6c6c 6f77 222c 0a20 2020 2022  shmallow",.    "
+000005e0: 7469 6465 6c69 6674 5f75 726c 223a 2028  tidelift_url": (
+000005f0: 0a20 2020 2020 2020 2022 6874 7470 733a  .        "https:
+00000600: 2f2f 7469 6465 6c69 6674 2e63 6f6d 2f73  //tidelift.com/s
+00000610: 7562 7363 7269 7074 696f 6e2f 706b 672f  ubscription/pkg/
+00000620: 7079 7069 2d6d 6172 7368 6d61 6c6c 6f77  pypi-marshmallow
+00000630: 220a 2020 2020 2020 2020 223f 7574 6d5f  ".        "?utm_
+00000640: 736f 7572 6365 3d6d 6172 7368 6d61 6c6c  source=marshmall
+00000650: 6f77 2675 746d 5f6d 6564 6975 6d3d 7265  ow&utm_medium=re
+00000660: 6665 7272 616c 2675 746d 5f63 616d 7061  ferral&utm_campa
+00000670: 6967 6e3d 646f 6373 220a 2020 2020 292c  ign=docs".    ),
+00000680: 0a20 2020 2022 636f 6465 5f66 6f6e 745f  .    "code_font_
+00000690: 7369 7a65 223a 2022 302e 3865 6d22 2c0a  size": "0.8em",.
+000006a0: 2020 2020 2277 6172 6e5f 6267 223a 2022      "warn_bg": "
+000006b0: 2346 4643 222c 0a20 2020 2022 7761 726e  #FFC",.    "warn
+000006c0: 5f62 6f72 6465 7222 3a20 2223 4545 4522  _border": "#EEE"
+000006d0: 2c0a 2020 2020 2320 5573 6564 2074 6f20  ,.    # Used to 
+000006e0: 706f 7075 6c61 7465 2074 6865 2075 7365  populate the use
+000006f0: 6675 6c2d 6c69 6e6b 732e 6874 6d6c 2074  ful-links.html t
+00000700: 656d 706c 6174 650a 2020 2020 2265 7874  emplate.    "ext
+00000710: 7261 5f6e 6176 5f6c 696e 6b73 223a 204f  ra_nav_links": O
+00000720: 7264 6572 6564 4469 6374 280a 2020 2020  rderedDict(.    
+00000730: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+00000740: 2020 2822 6d61 7273 686d 616c 6c6f 7720    ("marshmallow 
+00000750: 4020 5079 5049 222c 2022 6874 7470 733a  @ PyPI", "https:
+00000760: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
+00000770: 672f 7079 7069 2f6d 6172 7368 6d61 6c6c  g/pypi/marshmall
+00000780: 6f77 2229 2c0a 2020 2020 2020 2020 2020  ow"),.          
+00000790: 2020 2822 6d61 7273 686d 616c 6c6f 7720    ("marshmallow 
+000007a0: 4020 4769 7448 7562 222c 2022 6874 7470  @ GitHub", "http
+000007b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+000007c0: 6172 7368 6d61 6c6c 6f77 2d63 6f64 652f  arshmallow-code/
+000007d0: 6d61 7273 686d 616c 6c6f 7722 292c 0a20  marshmallow"),. 
+000007e0: 2020 2020 2020 2020 2020 2028 2249 7373             ("Iss
+000007f0: 7565 2054 7261 636b 6572 222c 2022 6874  ue Tracker", "ht
+00000800: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000810: 2f6d 6172 7368 6d61 6c6c 6f77 2d63 6f64  /marshmallow-cod
+00000820: 652f 6d61 7273 686d 616c 6c6f 772f 6973  e/marshmallow/is
+00000830: 7375 6573 2229 2c0a 2020 2020 2020 2020  sues"),.        
+00000840: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
+00000850: 2020 2020 2020 2245 636f 7379 7374 656d        "Ecosystem
+00000860: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00000870: 2020 2022 6874 7470 733a 2f2f 6769 7468     "https://gith
+00000880: 7562 2e63 6f6d 2f6d 6172 7368 6d61 6c6c  ub.com/marshmall
+00000890: 6f77 2d63 6f64 652f 6d61 7273 686d 616c  ow-code/marshmal
+000008a0: 6c6f 772f 7769 6b69 2f45 636f 7379 7374  low/wiki/Ecosyst
+000008b0: 656d 222c 0a20 2020 2020 2020 2020 2020  em",.           
+000008c0: 2029 2c0a 2020 2020 2020 2020 5d0a 2020   ),.        ].  
+000008d0: 2020 292c 0a7d 0a0a 6874 6d6c 5f73 6964    ),.}..html_sid
+000008e0: 6562 6172 7320 3d20 7b0a 2020 2020 2269  ebars = {.    "i
+000008f0: 6e64 6578 223a 205b 2261 626f 7574 2e68  ndex": ["about.h
+00000900: 746d 6c22 2c20 2264 6f6e 6174 652e 6874  tml", "donate.ht
+00000910: 6d6c 222c 2022 7573 6566 756c 2d6c 696e  ml", "useful-lin
+00000920: 6b73 2e68 746d 6c22 2c20 2273 6561 7263  ks.html", "searc
+00000930: 6862 6f78 2e68 746d 6c22 5d2c 0a20 2020  hbox.html"],.   
+00000940: 2022 2a2a 223a 205b 0a20 2020 2020 2020   "**": [.       
+00000950: 2022 6162 6f75 742e 6874 6d6c 222c 0a20   "about.html",. 
+00000960: 2020 2020 2020 2022 646f 6e61 7465 2e68         "donate.h
+00000970: 746d 6c22 2c0a 2020 2020 2020 2020 2275  tml",.        "u
+00000980: 7365 6675 6c2d 6c69 6e6b 732e 6874 6d6c  seful-links.html
+00000990: 222c 0a20 2020 2020 2020 2022 6c6f 6361  ",.        "loca
+000009a0: 6c74 6f63 2e68 746d 6c22 2c0a 2020 2020  ltoc.html",.    
+000009b0: 2020 2020 2272 656c 6174 696f 6e73 2e68      "relations.h
+000009c0: 746d 6c22 2c0a 2020 2020 2020 2020 2273  tml",.        "s
+000009d0: 6561 7263 6862 6f78 2e68 746d 6c22 2c0a  earchbox.html",.
+000009e0: 2020 2020 5d2c 0a7d 0a0a 2320 7370 6869      ],.}..# sphi
+000009f0: 6e78 2d76 6572 7369 6f6e 2d77 6172 6e69  nx-version-warni
+00000a00: 6e67 2063 6f6e 6669 670a 7665 7273 696f  ng config.versio
+00000a10: 6e77 6172 6e69 6e67 5f6d 6573 7361 6765  nwarning_message
+00000a20: 7320 3d20 7b0a 2020 2020 226c 6174 6573  s = {.    "lates
+00000a30: 7422 3a20 280a 2020 2020 2020 2020 2254  t": (.        "T
+00000a40: 6869 7320 646f 6375 6d65 6e74 2069 7320  his document is 
+00000a50: 666f 7220 7468 6520 6465 7665 6c6f 706d  for the developm
+00000a60: 656e 7420 7665 7273 696f 6e2e 2022 0a20  ent version. ". 
+00000a70: 2020 2020 2020 2027 466f 7220 7468 6520         'For the 
+00000a80: 7374 6162 6c65 2076 6572 7369 6f6e 2064  stable version d
+00000a90: 6f63 756d 656e 7461 7469 6f6e 2c20 7365  ocumentation, se
+00000aa0: 6520 3c61 2068 7265 663d 222f 656e 2f73  e <a href="/en/s
+00000ab0: 7461 626c 652f 223e 6865 7265 3c2f 613e  table/">here</a>
+00000ac0: 2e27 0a20 2020 2029 2c0a 2020 2020 2232  .'.    ),.    "2
+00000ad0: 2e78 2d6c 696e 6522 3a20 280a 2020 2020  .x-line": (.    
+00000ae0: 2020 2020 226d 6172 7368 6d61 6c6c 6f77      "marshmallow
+00000af0: 2032 2069 7320 6e6f 206c 6f6e 6765 7220   2 is no longer 
+00000b00: 7375 7070 6f72 7465 6420 6173 206f 6620  supported as of 
+00000b10: 3230 3230 2d30 382d 3138 2e20 220a 2020  2020-08-18. ".  
+00000b20: 2020 2020 2020 273c 6120 6872 6566 3d22        '<a href="
+00000b30: 6874 7470 733a 2f2f 6d61 7273 686d 616c  https://marshmal
+00000b40: 6c6f 772e 7265 6164 7468 6564 6f63 732e  low.readthedocs.
+00000b50: 696f 2f65 6e2f 6c61 7465 7374 2f75 7067  io/en/latest/upg
+00000b60: 7261 6469 6e67 2e68 746d 6c23 7570 6772  rading.html#upgr
+00000b70: 6164 696e 672d 746f 2d33 2d30 223e 270a  ading-to-3-0">'.
+00000b80: 2020 2020 2020 2020 2255 7064 6174 6520          "Update 
+00000b90: 796f 7572 2063 6f64 6520 746f 2075 7365  your code to use
+00000ba0: 206d 6172 7368 6d61 6c6c 6f77 2033 3c2f   marshmallow 3</
+00000bb0: 613e 2e22 0a20 2020 2029 2c0a 7d0a 2320  a>.".    ),.}.# 
+00000bc0: 5368 6f77 2077 6172 6e69 6e67 2061 7420  Show warning at 
+00000bd0: 746f 7020 6f66 2070 6167 650a 7665 7273  top of page.vers
+00000be0: 696f 6e77 6172 6e69 6e67 5f62 6f64 795f  ionwarning_body_
+00000bf0: 7365 6c65 6374 6f72 203d 2022 6469 762e  selector = "div.
+00000c00: 646f 6375 6d65 6e74 220a 7665 7273 696f  document".versio
+00000c10: 6e77 6172 6e69 6e67 5f62 616e 6e65 725f  nwarning_banner_
+00000c20: 7469 746c 6520 3d20 2222 0a23 2046 6f72  title = "".# For
+00000c30: 2064 6562 7567 6769 6e67 206c 6f63 616c   debugging local
+00000c40: 6c79 0a23 2076 6572 7369 6f6e 7761 726e  ly.# versionwarn
+00000c50: 696e 675f 7072 6f6a 6563 745f 7665 7273  ing_project_vers
+00000c60: 696f 6e20 3d20 226c 6174 6573 7422 0a    ion = "latest".
```

### Comparing `marshmallow-3.9.0/docs/custom_fields.rst` & `marshmallow-3.9.1/docs/custom_fields.rst`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/docs/examples.rst` & `marshmallow-3.9.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/docs/extending.rst` & `marshmallow-3.9.1/docs/extending.rst`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/docs/index.rst` & `marshmallow-3.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/docs/install.rst` & `marshmallow-3.9.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/docs/nesting.rst` & `marshmallow-3.9.1/docs/nesting.rst`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/docs/quickstart.rst` & `marshmallow-3.9.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/docs/upgrading.rst` & `marshmallow-3.9.1/docs/upgrading.rst`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/docs/why.rst` & `marshmallow-3.9.1/docs/why.rst`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/examples/flask_example.py` & `marshmallow-3.9.1/examples/flask_example.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/examples/inflection_example.py` & `marshmallow-3.9.1/examples/inflection_example.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/examples/package_json_example.py` & `marshmallow-3.9.1/examples/package_json_example.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/examples/peewee_example.py` & `marshmallow-3.9.1/examples/peewee_example.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/examples/textblob_example.py` & `marshmallow-3.9.1/examples/textblob_example.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/setup.py` & `marshmallow-3.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "lint": [
         "mypy==0.790",
         "flake8==3.8.4",
         "flake8-bugbear==20.1.4",
         "pre-commit~=2.4",
     ],
     "docs": [
-        "sphinx==3.2.1",
+        "sphinx==3.3.0",
         "sphinx-issues==1.2.0",
         "alabaster==0.7.12",
         "sphinx-version-warning==1.1.2",
         "autodocsumm==0.2.1",
     ],
 }
 EXTRAS_REQUIRE["dev"] = EXTRAS_REQUIRE["tests"] + EXTRAS_REQUIRE["lint"] + ["tox"]
```

### Comparing `marshmallow-3.9.0/src/marshmallow/__init__.py` & `marshmallow-3.9.1/src/marshmallow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     validates,
     validates_schema,
 )
 from marshmallow.utils import EXCLUDE, INCLUDE, RAISE, pprint, missing
 from marshmallow.exceptions import ValidationError
 from distutils.version import LooseVersion
 
-__version__ = "3.9.0"
+__version__ = "3.9.1"
 __version_info__ = tuple(LooseVersion(__version__).version)
 __all__ = [
     "EXCLUDE",
     "INCLUDE",
     "RAISE",
     "Schema",
     "SchemaOpts",
```

### Comparing `marshmallow-3.9.0/src/marshmallow/base.py` & `marshmallow-3.9.1/src/marshmallow/base.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/src/marshmallow/class_registry.py` & `marshmallow-3.9.1/src/marshmallow/class_registry.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/src/marshmallow/decorators.py` & `marshmallow-3.9.1/src/marshmallow/decorators.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/src/marshmallow/error_store.py` & `marshmallow-3.9.1/src/marshmallow/error_store.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/src/marshmallow/exceptions.py` & `marshmallow-3.9.1/src/marshmallow/exceptions.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/src/marshmallow/fields.py` & `marshmallow-3.9.1/src/marshmallow/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1501,15 +1501,15 @@
             self.key_field = copy.deepcopy(self.key_field)
             self.key_field._bind_to_schema(field_name, self)
 
     def _serialize(self, value, attr, obj, **kwargs):
         if value is None:
             return None
         if not self.value_field and not self.key_field:
-            return value
+            return self.mapping_type(value)
 
         #  Serialize keys
         if self.key_field is None:
             keys = {k: k for k in value.keys()}
         else:
             keys = {
                 k: self.key_field._serialize(k, None, None, **kwargs)
@@ -1528,15 +1528,15 @@
 
         return result
 
     def _deserialize(self, value, attr, data, **kwargs):
         if not isinstance(value, _Mapping):
             raise self.make_error("invalid")
         if not self.value_field and not self.key_field:
-            return value
+            return self.mapping_type(value)
 
         errors = collections.defaultdict(dict)
 
         #  Deserialize keys
         if self.key_field is None:
             keys = {k: k for k in value.keys()}
         else:
@@ -1642,15 +1642,18 @@
         self.validators.insert(0, validator)
 
 
 class IP(Field):
     """A IP address field.
 
     :param bool exploded: If `True`, serialize ipv6 address in long form, ie. with groups
-        consisting entirely of zeros included."""
+        consisting entirely of zeros included.
+
+    .. versionadded:: 3.8.0
+    """
 
     default_error_messages = {"invalid_ip": "Not a valid IP address."}
 
     DESERIALIZATION_CLASS = None  # type: typing.Optional[typing.Type]
 
     def __init__(self, *args, exploded=False, **kwargs):
         super().__init__(*args, **kwargs)
@@ -1673,23 +1676,29 @@
                 utils.ensure_text_type(value)
             )
         except (ValueError, TypeError) as error:
             raise self.make_error("invalid_ip") from error
 
 
 class IPv4(IP):
-    """A IPv4 address field."""
+    """A IPv4 address field.
+
+    .. versionadded:: 3.8.0
+    """
 
     default_error_messages = {"invalid_ip": "Not a valid IPv4 address."}
 
     DESERIALIZATION_CLASS = ipaddress.IPv4Address
 
 
 class IPv6(IP):
-    """A IPv6 address field."""
+    """A IPv6 address field.
+
+    .. versionadded:: 3.8.0
+    """
 
     default_error_messages = {"invalid_ip": "Not a valid IPv6 address."}
 
     DESERIALIZATION_CLASS = ipaddress.IPv6Address
 
 
 class Method(Field):
```

### Comparing `marshmallow-3.9.0/src/marshmallow/orderedset.py` & `marshmallow-3.9.1/src/marshmallow/orderedset.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/src/marshmallow/schema.py` & `marshmallow-3.9.1/src/marshmallow/schema.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/src/marshmallow/utils.py` & `marshmallow-3.9.1/src/marshmallow/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,17 @@
     return isinstance(obj, tuple) and hasattr(obj, "_fields")
 
 
 def pprint(obj, *args, **kwargs) -> None:
     """Pretty-printing function that can pretty-print OrderedDicts
     like regular dictionaries. Useful for printing the output of
     :meth:`marshmallow.Schema.dump`.
+
+    .. deprecated:: 3.7.0
+        marshmallow.pprint will be removed in marshmallow 4.
     """
     warnings.warn(
         "marshmallow's pprint function is deprecated and will be removed in marshmallow 4.",
         RemovedInMarshmallow4Warning,
     )
     if isinstance(obj, collections.OrderedDict):
         print(json.dumps(obj, *args, **kwargs))
```

### Comparing `marshmallow-3.9.0/src/marshmallow/validate.py` & `marshmallow-3.9.1/src/marshmallow/validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -560,14 +560,16 @@
 class ContainsNoneOf(NoneOf):
     """Validator which fails if ``value`` is a sequence and any element
     in the sequence is a member of the sequence passed as ``iterable``. Empty input
     is considered valid.
 
     :param iterable iterable: Same as :class:`NoneOf`.
     :param str error: Same as :class:`NoneOf`.
+
+    .. versionadded:: 3.6.0
     """
 
     default_message = "One or more of the choices you made was in: {values}."
 
     def _format_error(self, value) -> str:
         value_text = ", ".join(str(val) for val in value)
         return super()._format_error(value_text)
```

### Comparing `marshmallow-3.9.0/src/marshmallow.egg-info/PKG-INFO` & `marshmallow-3.9.1/src/marshmallow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marshmallow
-Version: 3.9.0
+Version: 3.9.1
 Summary: A lightweight library for converting complex datatypes to and from native Python datatypes.
 Home-page: https://github.com/marshmallow-code/marshmallow
 Author: Steven Loria
 Author-email: sloria1@gmail.com
 License: MIT
 Project-URL: Changelog, https://marshmallow.readthedocs.io/en/latest/changelog.html
 Project-URL: Issues, https://github.com/marshmallow-code/marshmallow/issues
```

### Comparing `marshmallow-3.9.0/src/marshmallow.egg-info/SOURCES.txt` & `marshmallow-3.9.1/src/marshmallow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/tests/base.py` & `marshmallow-3.9.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/tests/conftest.py` & `marshmallow-3.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/tests/test_decorators.py` & `marshmallow-3.9.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/tests/test_deserialization.py` & `marshmallow-3.9.1/tests/test_deserialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -715,16 +715,21 @@
         field = fields.Date()
         with pytest.raises(ValidationError) as excinfo:
             field.deserialize(in_value)
         msg = "Not a valid date."
         assert excinfo.value.args[0] == msg
 
     def test_dict_field_deserialization(self):
+        data = {"foo": "bar"}
         field = fields.Dict()
-        assert field.deserialize({"foo": "bar"}) == {"foo": "bar"}
+        load = field.deserialize(data)
+        assert load == {"foo": "bar"}
+        # Check load is a distinct object
+        load["foo"] = "baz"
+        assert data["foo"] == "bar"
         with pytest.raises(ValidationError) as excinfo:
             field.deserialize("baddict")
         assert excinfo.value.args[0] == "Not a valid mapping type."
 
     def test_structured_dict_value_deserialization(self):
         field = fields.Dict(values=fields.List(fields.Str))
         assert field.deserialize({"foo": ["bar", "baz"]}) == {"foo": ["bar", "baz"]}
```

### Comparing `marshmallow-3.9.0/tests/test_error_store.py` & `marshmallow-3.9.1/tests/test_error_store.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/tests/test_exceptions.py` & `marshmallow-3.9.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/tests/test_fields.py` & `marshmallow-3.9.1/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/tests/test_options.py` & `marshmallow-3.9.1/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/tests/test_registry.py` & `marshmallow-3.9.1/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/tests/test_schema.py` & `marshmallow-3.9.1/tests/test_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -637,19 +637,14 @@
 
 
 def test_can_serialize_time(user, serialized_user):
     expected = user.time_registered.isoformat()[:15]
     assert serialized_user["time_registered"] == expected
 
 
-def test_invalid_dict_but_okay():
-    u = User("Joe", various_data="baddict")
-    UserSchema().dump(u)
-
-
 def test_json_module_is_deprecated():
     with pytest.deprecated_call():
 
         class UserJSONSchema(Schema):
             name = fields.String()
 
             class Meta:
```

### Comparing `marshmallow-3.9.0/tests/test_serialization.py` & `marshmallow-3.9.1/tests/test_serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,24 +365,22 @@
         assert field.serialize("email", user) is None
 
     def test_dict_field_serialize_none(self, user):
         user.various_data = None
         field = fields.Dict()
         assert field.serialize("various_data", user) is None
 
-    def test_dict_field_invalid_dict_but_okay(self, user):
-        user.various_data = "okaydict"
-        field = fields.Dict()
-        field.serialize("various_data", user)
-        assert field.serialize("various_data", user) == "okaydict"
-
     def test_dict_field_serialize(self, user):
         user.various_data = {"foo": "bar"}
         field = fields.Dict()
-        assert field.serialize("various_data", user) == {"foo": "bar"}
+        dump = field.serialize("various_data", user)
+        assert dump == {"foo": "bar"}
+        # Check dump is a distinct object
+        dump["foo"] = "baz"
+        assert user.various_data["foo"] == "bar"
 
     def test_dict_field_serialize_ordereddict(self, user):
         user.various_data = OrderedDict([("foo", "bar"), ("bar", "baz")])
         field = fields.Dict()
         assert field.serialize("various_data", user) == OrderedDict(
             [("foo", "bar"), ("bar", "baz")]
         )
```

### Comparing `marshmallow-3.9.0/tests/test_utils.py` & `marshmallow-3.9.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `marshmallow-3.9.0/tests/test_validate.py` & `marshmallow-3.9.1/tests/test_validate.py`

 * *Files identical despite different names*

