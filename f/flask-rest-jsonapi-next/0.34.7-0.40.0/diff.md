# Comparing `tmp/flask-rest-jsonapi-next-0.34.7.tar.gz` & `tmp/flask-rest-jsonapi-next-0.40.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-rest-jsonapi-next-0.34.7.tar", last modified: Wed Jun 28 13:56:10 2023, max compression
+gzip compressed data, was "flask-rest-jsonapi-next-0.40.0.tar", last modified: Fri Jul 21 17:53:07 2023, max compression
```

## Comparing `flask-rest-jsonapi-next-0.34.7.tar` & `flask-rest-jsonapi-next-0.40.0.tar`

### file list

```diff
@@ -1,81 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:56:10.527414 flask-rest-jsonapi-next-0.34.7/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-06-28 13:56:10.527414 flask-rest-jsonapi-next-0.34.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:56:10.519414 flask-rest-jsonapi-next-0.34.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/data_layer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/features.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/filtering.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/flask-rest-jsonapi-next.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:56:10.519414 flask-rest-jsonapi-next-0.34.7/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    60801 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/img/schema.png
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/include_related_objects.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/logical_data_abstraction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/oauth.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/pagination.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/permission.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25491 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/resource_manager.rst
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/routing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/sorting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/docs/sparse_fieldsets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:56:10.519414 flask-rest-jsonapi-next-0.34.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/examples/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/examples/api_nested.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:56:10.523414 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:56:10.523414 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/data_layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/data_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32059 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/data_layers/alchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/data_layers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:56:10.523414 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/data_layers/filtering/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/data_layers/filtering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/data_layers/filtering/alchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:56:10.523414 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/error_responses/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/error_responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/error_responses/error_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/error_responses/errors_as_json_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:56:10.523414 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/error_responses/exception_converters/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/error_responses/exception_converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/error_responses/exception_converters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/error_responses/exception_converters/flask_rest_jsonapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/error_responses/exception_converters/marshamallow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/error_responses/exception_converters/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/error_responses/exception_converters/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/error_responses/exception_converters/werkzeug.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/error_responses/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/querystring.py
--rw-r--r--   0 runner    (1001) docker     (123)    21925 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:56:10.523414 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-06-28 13:56:10.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-28 13:56:10.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 13:56:10.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 13:56:10.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-28 13:56:10.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-28 13:56:10.000000 flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 13:56:10.527414 flask-rest-jsonapi-next-0.34.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:56:10.527414 flask-rest-jsonapi-next-0.34.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    69985 2023-06-28 13:56:00.000000 flask-rest-jsonapi-next-0.34.7/tests/test_sqlalchemy_data_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.873710 flask-rest-jsonapi-next-0.40.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-21 17:53:07.873710 flask-rest-jsonapi-next-0.40.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.865710 flask-rest-jsonapi-next-0.40.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/data_layer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/filtering.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/flask-rest-jsonapi-next.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.865710 flask-rest-jsonapi-next-0.40.0/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    60801 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/img/schema.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/include_related_objects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/logical_data_abstraction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/oauth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/pagination.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/permission.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25464 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/resource_manager.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/routing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/sorting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/sparse_fieldsets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/sqlalchemy_2x_support.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.865710 flask-rest-jsonapi-next-0.40.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/examples/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/examples/api_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 17:53:07.873710 flask-rest-jsonapi-next-0.40.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.861710 flask-rest-jsonapi-next-0.40.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.869710 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.869710 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37548 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/alchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13929 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.869710 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/filtering/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/filtering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/filtering/alchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.869710 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/error_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/errors_as_json_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.869710 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/flask_rest_jsonapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/marshamallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/werkzeug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/querystring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22299 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.869710 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-21 17:53:07.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-21 17:53:07.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 17:53:07.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 17:53:07.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-21 17:53:07.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 17:53:07.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.869710 flask-rest-jsonapi-next-0.40.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/content_type_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.869710 flask-rest-jsonapi-next-0.40.0/tests/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/flask_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.873710 flask-rest-jsonapi-next-0.40.0/tests/factories/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/models/computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/models/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/models/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/models/person_single_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/models/person_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/models/string_json_attribute_person.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.873710 flask-rest-jsonapi-next-0.40.0/tests/factories/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/resources/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/resources/computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/resources/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/resources/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/resources/string_json_attribute_person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/querystring_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/resource_detail_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/resource_list_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/resource_relationship_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/resource_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/sqlalchemy_data_layer_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/sqlalchemy_filtering_spec.py
```

### Comparing `flask-rest-jsonapi-next-0.34.7/CHANGELOG.md` & `flask-rest-jsonapi-next-0.40.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # CHANGELOG
 
+## 0.40.0 (2023-07-21)
+
+- removed restriction on SQLAlchemy version, library now works with SQLAlchemy 2.x
+  - working with SQLAlchemy 2.x layer requires some changes in client code, otherwise
+    there might be performance penalties
+  - added docs section on SQLAlchemy 2.x usage
+- tested with psycopg 3
+
 ## 0.34.7 (fork-0.34.7) (2023-06-28)
 
 - fix: missing import
 
 ## 0.34.6 (fork-0.34.6) (2023-06-27)
 
 - fix: filtering operator `between` was not correctly implemented for SQLAlchemy
```

### Comparing `flask-rest-jsonapi-next-0.34.7/LICENSE` & `flask-rest-jsonapi-next-0.40.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/PKG-INFO` & `flask-rest-jsonapi-next-0.40.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rest-jsonapi-next
-Version: 0.34.7
+Version: 0.40.0
 Summary: Flask extension to create REST web api according to JSONAPI 1.0 specification with Flask, Marshmallow and data provider of your choice (SQLAlchemy, MongoDB, ...)
 Author: original miLibris/flask-rest-jsonapi contributors
 Maintainer-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-rest-jsonapi-next
 Project-URL: Documentation, https://flask-rest-jsonapi-next.readthedocs.io/en/latest/
 Keywords: web,api,rest,jsonapi,flask,sqlalchemy,marshmallow
@@ -45,16 +45,14 @@
 ```sh
 pip install flask-rest-jsonapi-next
 ```
 
 ## A minimal API
 
 ```py
-# -*- coding: utf-8 -*-
-
 from flask import Flask
 from flask_rest_jsonapi_next import Api, ResourceDetail, ResourceList
 from flask_sqlalchemy import SQLAlchemy
 from marshmallow_jsonapi.flask import Schema
 from marshmallow_jsonapi import fields
 
 # Create the Flask application and the Flask-SQLAlchemy object.
```

### Comparing `flask-rest-jsonapi-next-0.34.7/README.md` & `flask-rest-jsonapi-next-0.40.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 ```sh
 pip install flask-rest-jsonapi-next
 ```
 
 ## A minimal API
 
 ```py
-# -*- coding: utf-8 -*-
-
 from flask import Flask
 from flask_rest_jsonapi_next import Api, ResourceDetail, ResourceList
 from flask_sqlalchemy import SQLAlchemy
 from marshmallow_jsonapi.flask import Schema
 from marshmallow_jsonapi import fields
 
 # Create the Flask application and the Flask-SQLAlchemy object.
```

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/Makefile` & `flask-rest-jsonapi-next-0.40.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/conf.py` & `flask-rest-jsonapi-next-0.40.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "flask-rest-jsonapi-next"
 copyright = "2016-2021 miLibris; 2021-... miLibris, tadams42"
 author = "tadams42"
-release = "0.34.7"
+release = "0.40.0"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
```

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/data_layer.rst` & `flask-rest-jsonapi-next-0.40.0/docs/data_layer.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/errors.rst` & `flask-rest-jsonapi-next-0.40.0/docs/errors.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/features.rst` & `flask-rest-jsonapi-next-0.40.0/docs/features.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/filtering.rst` & `flask-rest-jsonapi-next-0.40.0/docs/filtering.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/flask-rest-jsonapi-next.rst` & `flask-rest-jsonapi-next-0.40.0/docs/flask-rest-jsonapi-next.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/img/schema.png` & `flask-rest-jsonapi-next-0.40.0/docs/img/schema.png`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/include_related_objects.rst` & `flask-rest-jsonapi-next-0.40.0/docs/include_related_objects.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/index.rst` & `flask-rest-jsonapi-next-0.40.0/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
    pagination
    sorting
    errors
    api
    permission
    oauth
    configuration
+   sqlalchemy_2x_support
 
 API Reference
 -------------
 
 If you are looking for information on a specific function, class or
 method, this part of the documentation is for you.
```

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/installation.rst` & `flask-rest-jsonapi-next-0.40.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/logical_data_abstraction.rst` & `flask-rest-jsonapi-next-0.40.0/docs/logical_data_abstraction.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/make.bat` & `flask-rest-jsonapi-next-0.40.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/oauth.rst` & `flask-rest-jsonapi-next-0.40.0/docs/oauth.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/pagination.rst` & `flask-rest-jsonapi-next-0.40.0/docs/pagination.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/permission.rst` & `flask-rest-jsonapi-next-0.40.0/docs/permission.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/quickstart.rst` & `flask-rest-jsonapi-next-0.40.0/docs/quickstart.rst`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 First example
 -------------
 
 An example of flask-rest-jsonapi-next API looks like this:
 
 .. code-block:: python
 
-    # -*- coding: utf-8 -*-
+
 
     from flask import Flask
     from flask_rest_jsonapi_next import Api, ResourceDetail, ResourceList, ResourceRelationship
     from flask_rest_jsonapi_next.exceptions import ObjectNotFound
     from flask_sqlalchemy import SQLAlchemy
     from sqlalchemy.orm.exc import NoResultFound
     from marshmallow_jsonapi.flask import Schema, Relationship
```

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/resource_manager.rst` & `flask-rest-jsonapi-next-0.40.0/docs/resource_manager.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/routing.rst` & `flask-rest-jsonapi-next-0.40.0/docs/routing.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/sorting.rst` & `flask-rest-jsonapi-next-0.40.0/docs/sorting.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/docs/sparse_fieldsets.rst` & `flask-rest-jsonapi-next-0.40.0/docs/sparse_fieldsets.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/examples/api.py` & `flask-rest-jsonapi-next-0.40.0/examples/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-# -*- coding: utf-8 -*-
-
 from flask import Flask
-from flask_rest_jsonapi_next import Api, ResourceDetail, ResourceList, ResourceRelationship
+from flask_rest_jsonapi_next import (
+    Api,
+    ResourceDetail,
+    ResourceList,
+    ResourceRelationship,
+)
 from flask_rest_jsonapi_next.exceptions import ObjectNotFound
 from flask_sqlalchemy import SQLAlchemy
 from sqlalchemy.orm.exc import NoResultFound
 from marshmallow_jsonapi.flask import Schema, Relationship
 from marshmallow_jsonapi import fields
 
 # Create the Flask application
 app = Flask(__name__)
-app.config['DEBUG'] = True
-app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
+app.config["DEBUG"] = True
+app.config["SQLALCHEMY_TRACK_MODIFICATIONS"] = False
 
 
 # Initialize SQLAlchemy
-app.config['SQLALCHEMY_DATABASE_URI'] = 'sqlite:////tmp/test.db'
+app.config["SQLALCHEMY_DATABASE_URI"] = "sqlite:////tmp/test.db"
 db = SQLAlchemy(app)
 
 
 # Create data storage
 class Person(db.Model):
     id = db.Column(db.Integer, primary_key=True)
     name = db.Column(db.String)
@@ -27,133 +30,157 @@
     birth_date = db.Column(db.Date)
     password = db.Column(db.String)
 
 
 class Computer(db.Model):
     id = db.Column(db.Integer, primary_key=True)
     serial = db.Column(db.String)
-    person_id = db.Column(db.Integer, db.ForeignKey('person.id'))
-    person = db.relationship('Person', backref=db.backref('computers'))
+    person_id = db.Column(db.Integer, db.ForeignKey("person.id"))
+    person = db.relationship("Person", backref=db.backref("computers"))
+
 
 db.create_all()
 
 
 # Create logical data abstraction (same as data storage for this first example)
 class PersonSchema(Schema):
     class Meta:
-        type_ = 'person'
-        self_view = 'person_detail'
-        self_view_kwargs = {'id': '<id>'}
-        self_view_many = 'person_list'
+        type_ = "person"
+        self_view = "person_detail"
+        self_view_kwargs = {"id": "<id>"}
+        self_view_many = "person_list"
 
     id = fields.Integer(as_string=True, dump_only=True)
     name = fields.Str(required=True, load_only=True)
     email = fields.Email(load_only=True)
     birth_date = fields.Date()
-    display_name = fields.Function(lambda obj: "{} <{}>".format(obj.name.upper(), obj.email))
-    computers = Relationship(self_view='person_computers',
-                             self_view_kwargs={'id': '<id>'},
-                             related_view='computer_list',
-                             related_view_kwargs={'id': '<id>'},
-                             many=True,
-                             schema='ComputerSchema',
-                             type_='computer')
+    display_name = fields.Function(
+        lambda obj: "{} <{}>".format(obj.name.upper(), obj.email)
+    )
+    computers = Relationship(
+        self_view="person_computers",
+        self_view_kwargs={"id": "<id>"},
+        related_view="computer_list",
+        related_view_kwargs={"id": "<id>"},
+        many=True,
+        schema="ComputerSchema",
+        type_="computer",
+    )
 
 
 class ComputerSchema(Schema):
     class Meta:
-        type_ = 'computer'
-        self_view = 'computer_detail'
-        self_view_kwargs = {'id': '<id>'}
+        type_ = "computer"
+        self_view = "computer_detail"
+        self_view_kwargs = {"id": "<id>"}
 
     id = fields.Integer(as_string=True, dump_only=True)
     serial = fields.Str(required=True)
-    owner = Relationship(attribute='person',
-                         self_view='computer_person',
-                         self_view_kwargs={'id': '<id>'},
-                         related_view='person_detail',
-                         related_view_kwargs={'computer_id': '<id>'},
-                         schema='PersonSchema',
-                         type_='person')
+    owner = Relationship(
+        attribute="person",
+        self_view="computer_person",
+        self_view_kwargs={"id": "<id>"},
+        related_view="person_detail",
+        related_view_kwargs={"computer_id": "<id>"},
+        schema="PersonSchema",
+        type_="person",
+    )
 
 
 # Create resource managers
 class PersonList(ResourceList):
     schema = PersonSchema
-    data_layer = {'session': db.session,
-                  'model': Person}
+    data_layer = {"session": db.session, "model": Person}
 
 
 class PersonDetail(ResourceDetail):
     def before_get_object(self, view_kwargs):
-        if view_kwargs.get('computer_id') is not None:
+        if view_kwargs.get("computer_id") is not None:
             try:
-                computer = self.session.query(Computer).filter_by(id=view_kwargs['computer_id']).one()
+                computer = (
+                    self.session.query(Computer)
+                    .filter_by(id=view_kwargs["computer_id"])
+                    .one()
+                )
             except NoResultFound:
-                raise ObjectNotFound({'parameter': 'computer_id'},
-                                     "Computer: {} not found".format(view_kwargs['computer_id']))
+                raise ObjectNotFound(
+                    {"parameter": "computer_id"},
+                    "Computer: {} not found".format(view_kwargs["computer_id"]),
+                )
             else:
                 if computer.person is not None:
-                    view_kwargs['id'] = computer.person.id
+                    view_kwargs["id"] = computer.person.id
                 else:
-                    view_kwargs['id'] = None
+                    view_kwargs["id"] = None
 
     schema = PersonSchema
-    data_layer = {'session': db.session,
-                  'model': Person,
-                  'methods': {'before_get_object': before_get_object}}
+    data_layer = {
+        "session": db.session,
+        "model": Person,
+        "methods": {"before_get_object": before_get_object},
+    }
 
 
 class PersonRelationship(ResourceRelationship):
     schema = PersonSchema
-    data_layer = {'session': db.session,
-                  'model': Person}
+    data_layer = {"session": db.session, "model": Person}
 
 
 class ComputerList(ResourceList):
     def query(self, view_kwargs):
         query_ = self.session.query(Computer)
-        if view_kwargs.get('id') is not None:
+        if view_kwargs.get("id") is not None:
             try:
-                self.session.query(Person).filter_by(id=view_kwargs['id']).one()
+                self.session.query(Person).filter_by(id=view_kwargs["id"]).one()
             except NoResultFound:
-                raise ObjectNotFound({'parameter': 'id'}, "Person: {} not found".format(view_kwargs['id']))
+                raise ObjectNotFound(
+                    {"parameter": "id"},
+                    "Person: {} not found".format(view_kwargs["id"]),
+                )
             else:
-                query_ = query_.join(Person).filter(Person.id == view_kwargs['id'])
+                query_ = query_.join(Person).filter(Person.id == view_kwargs["id"])
         return query_
 
     def before_create_object(self, data, view_kwargs):
-        if view_kwargs.get('id') is not None:
-            person = self.session.query(Person).filter_by(id=view_kwargs['id']).one()
-            data['person_id'] = person.id
+        if view_kwargs.get("id") is not None:
+            person = self.session.query(Person).filter_by(id=view_kwargs["id"]).one()
+            data["person_id"] = person.id
 
     schema = ComputerSchema
-    data_layer = {'session': db.session,
-                  'model': Computer,
-                  'methods': {'query': query,
-                              'before_create_object': before_create_object}}
+    data_layer = {
+        "session": db.session,
+        "model": Computer,
+        "methods": {"query": query, "before_create_object": before_create_object},
+    }
 
 
 class ComputerDetail(ResourceDetail):
     schema = ComputerSchema
-    data_layer = {'session': db.session,
-                  'model': Computer}
+    data_layer = {"session": db.session, "model": Computer}
 
 
 class ComputerRelationship(ResourceRelationship):
     schema = ComputerSchema
-    data_layer = {'session': db.session,
-                  'model': Computer}
+    data_layer = {"session": db.session, "model": Computer}
 
 
 # Create endpoints
 api = Api(app)
-api.route(PersonList, 'person_list', '/persons')
-api.route(PersonDetail, 'person_detail', '/persons/<int:id>', '/computers/<int:computer_id>/owner')
-api.route(PersonRelationship, 'person_computers', '/persons/<int:id>/relationships/computers')
-api.route(ComputerList, 'computer_list', '/computers', '/persons/<int:id>/computers')
-api.route(ComputerDetail, 'computer_detail', '/computers/<int:id>')
-api.route(ComputerRelationship, 'computer_person', '/computers/<int:id>/relationships/owner')
+api.route(PersonList, "person_list", "/persons")
+api.route(
+    PersonDetail,
+    "person_detail",
+    "/persons/<int:id>",
+    "/computers/<int:computer_id>/owner",
+)
+api.route(
+    PersonRelationship, "person_computers", "/persons/<int:id>/relationships/computers"
+)
+api.route(ComputerList, "computer_list", "/computers", "/persons/<int:id>/computers")
+api.route(ComputerDetail, "computer_detail", "/computers/<int:id>")
+api.route(
+    ComputerRelationship, "computer_person", "/computers/<int:id>/relationships/owner"
+)
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     # Start application
     app.run(debug=True)
```

### Comparing `flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/api.py` & `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-# -*- coding: utf-8 -*-
-# isort: skip_file
-# fmt: off
-
 """This module contains the main class of the Api to initialize the Api, plug default decorators for each resources
-methods, speficy which blueprint to use, define the Api routes and plug additional oauth manager and permission manager
+methods, specify which blueprint to use, define the Api routes and plug additional oauth manager and permission manager
 """
 
 import inspect
 from functools import wraps
 from pathlib import Path
 
-from flask import request, abort
+from flask import abort, request
 
-from .resource import ResourceList, ResourceRelationship
 from .error_responses import ErrorsAsJsonApi
+from .resource import ResourceList, ResourceRelationship
 
 
 class Api(object):
     """The main class of the Api"""
 
     def __init__(self, app=None, blueprint=None, decorators=None, register_at="/"):
         """Initialize an instance of the Api
@@ -46,96 +42,111 @@
         if app is not None:
             self.app = app
 
         if blueprint is not None:
             self.blueprint = blueprint
 
         for resource in self.resources:
-            self.route(resource['resource'],
-                       resource['view'],
-                       *resource['urls'],
-                       url_rule_options=resource['url_rule_options'])
+            self.route(
+                resource["resource"],
+                resource["view"],
+                *resource["urls"],
+                url_rule_options=resource["url_rule_options"],
+            )
 
         root_url_prefix = Path(self.register_at or "/")
 
         if self.blueprint is not None:
             self.app.register_blueprint(
                 self.blueprint,
-                url_prefix=str(root_url_prefix / f"./{self.blueprint.url_prefix or ''}"),
+                url_prefix=str(
+                    root_url_prefix / f"./{self.blueprint.url_prefix or ''}"
+                ),
             )
 
         if additional_blueprints is not None:
             for blueprint in additional_blueprints:
                 self.app.register_blueprint(
                     blueprint,
                     url_prefix=str(root_url_prefix / f"./{blueprint.url_prefix or ''}"),
                 )
 
-        self.app.config.setdefault('PAGE_SIZE', 30)
+        self.app.config.setdefault("PAGE_SIZE", 30)
 
         ErrorsAsJsonApi(app)
 
     def route(self, resource, view, *urls, **kwargs):
         """Create an api view.
 
         :param Resource resource: a resource class inherited from Resource
         :param str view: the view name
         :param list urls: the urls of the view
         :param dict kwargs: additional options of the route
         """
         resource.view = view
-        url_rule_options = kwargs.get('url_rule_options') or dict()
+        url_rule_options = kwargs.get("url_rule_options") or dict()
 
         # Allow the customization of the resource class instance
-        resource_args = kwargs.get('resource_args', [])
-        resource_kwargs = kwargs.get('resource_kwargs', {})
+        resource_args = kwargs.get("resource_args", [])
+        resource_kwargs = kwargs.get("resource_kwargs", {})
 
         view_func = resource.as_view(view, *resource_args, **resource_kwargs)
 
-        if 'blueprint' in kwargs:
-            resource.view = '.'.join([kwargs['blueprint'].name, resource.view])
+        if "blueprint" in kwargs:
+            resource.view = ".".join([kwargs["blueprint"].name, resource.view])
             for url in urls:
-                kwargs['blueprint'].add_url_rule(url, view_func=view_func, **url_rule_options)
+                kwargs["blueprint"].add_url_rule(
+                    url, view_func=view_func, **url_rule_options
+                )
         elif self.blueprint is not None:
-            resource.view = '.'.join([self.blueprint.name, resource.view])
+            resource.view = ".".join([self.blueprint.name, resource.view])
             for url in urls:
-                self.blueprint.add_url_rule(url, view_func=view_func, **url_rule_options)
+                self.blueprint.add_url_rule(
+                    url, view_func=view_func, **url_rule_options
+                )
         elif self.app is not None:
             for url in urls:
                 self.app.add_url_rule(url, view_func=view_func, **url_rule_options)
         else:
-            self.resources.append({'resource': resource,
-                                   'view': view,
-                                   'urls': urls,
-                                   'url_rule_options': url_rule_options})
+            self.resources.append(
+                {
+                    "resource": resource,
+                    "view": view,
+                    "urls": urls,
+                    "url_rule_options": url_rule_options,
+                }
+            )
 
         self.resource_registry.append(resource)
 
     def oauth_manager(self, oauth_manager):
         """Use the oauth manager to enable oauth for API
 
         :param oauth_manager: the oauth manager
         """
+
         @self.app.before_request
         def before_request():
             endpoint = request.endpoint
             resource = None
             if endpoint:
-                resource = getattr(self.app.view_functions[endpoint], 'view_class', None)
+                resource = getattr(
+                    self.app.view_functions[endpoint], "view_class", None
+                )
 
-            if resource and not getattr(resource, 'disable_oauth', None):
-                scopes = request.args.get('scopes')
+            if resource and not getattr(resource, "disable_oauth", None):
+                scopes = request.args.get("scopes")
 
-                if getattr(resource, 'schema'):
+                if getattr(resource, "schema"):
                     scopes = [self.build_scope(resource, request.method)]
                 elif scopes:
-                    scopes = scopes.split(',')
+                    scopes = scopes.split(",")
 
                     if scopes:
-                        scopes = scopes.split(',')
+                        scopes = scopes.split(",")
 
                 valid, req = oauth_manager.verify_request(scopes)
 
                 for func in oauth_manager._after_request_funcs:
                     valid, req = func(valid, req)
 
                 if not valid:
@@ -149,63 +160,70 @@
     def build_scope(resource, method):
         """Compute the name of the scope for oauth
 
         :param Resource resource: the resource manager
         :param str method: an http method
         :return str: the name of the scope
         """
-        if ResourceList in inspect.getmro(resource) and method == 'GET':
-            prefix = 'list'
+        if ResourceList in inspect.getmro(resource) and method == "GET":
+            prefix = "list"
         else:
-            method_to_prefix = {'GET': 'get',
-                                'POST': 'create',
-                                'PATCH': 'update',
-                                'DELETE': 'delete'}
+            method_to_prefix = {
+                "GET": "get",
+                "POST": "create",
+                "PATCH": "update",
+                "DELETE": "delete",
+            }
             prefix = method_to_prefix[method]
 
             if ResourceRelationship in inspect.getmro(resource):
-                prefix = '_'.join([prefix, 'relationship'])
+                prefix = "_".join([prefix, "relationship"])
 
-        return '_'.join([prefix, resource.schema.opts.type_])
+        return "_".join([prefix, resource.schema.opts.type_])
 
     def permission_manager(self, permission_manager, with_decorators=True):
         """Use permission manager to enable permission for API
 
         :param callable permission_manager: the permission manager
         """
         self.check_permissions = permission_manager
 
         if with_decorators:
             for resource in self.resource_registry:
-                if getattr(resource, 'disable_permission', None) is not True:
-                    for method in getattr(resource, 'methods', ('GET', 'POST', 'PATCH', 'DELETE')):
-                        setattr(resource,
-                                method.lower(),
-                                self.has_permission()(getattr(resource, method.lower())))
+                if getattr(resource, "disable_permission", None) is not True:
+                    for method in getattr(
+                        resource, "methods", ("GET", "POST", "PATCH", "DELETE")
+                    ):
+                        setattr(
+                            resource,
+                            method.lower(),
+                            self.has_permission()(getattr(resource, method.lower())),
+                        )
 
     def has_permission(self, *args, **kwargs):
         """Decorator used to check permissions before to call resource manager method"""
+
         def wrapper(view):
-            if getattr(view, '_has_permissions_decorator', False) is True:
+            if getattr(view, "_has_permissions_decorator", False) is True:
                 return view
 
             @wraps(view)
             def decorated(*view_args, **view_kwargs):
                 self.check_permissions(view, view_args, view_kwargs, *args, **kwargs)
                 return view(*view_args, **view_kwargs)
+
             decorated._has_permissions_decorator = True
             return decorated
+
         return wrapper
 
     @staticmethod
     def check_permissions(view, view_args, view_kwargs, *args, **kwargs):
         """The function use to check permissions
 
         :param callable view: the view
         :param list view_args: view args
         :param dict view_kwargs: view kwargs
         :param list args: decorator args
         :param dict kwargs: decorator kwargs
         """
         raise NotImplementedError
-
-# fmt: on
```

### Comparing `flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/data_layers/alchemy.py` & `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/alchemy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,71 @@
-# -*- coding: utf-8 -*-
-# isort: skip_file
-# fmt: off
-
 """This module is a CRUD interface between resource managers and the sqlalchemy ORM"""
+import warnings
 
-from sqlalchemy.orm.exc import NoResultFound
-from sqlalchemy.orm.collections import InstrumentedList
-from sqlalchemy.inspection import inspect
-from sqlalchemy.orm.attributes import QueryableAttribute
-from sqlalchemy.orm import joinedload, ColumnProperty, RelationshipProperty
+import marshmallow
+import sqlalchemy
+from flask import current_app
 from marshmallow import class_registry
 from marshmallow.base import SchemaABC
+from packaging.version import Version
+from sqlalchemy import orm
+from sqlalchemy.inspection import inspect
+from sqlalchemy.orm import ColumnProperty, RelationshipProperty
+from sqlalchemy.orm.attributes import QueryableAttribute
+from sqlalchemy.orm.collections import InstrumentedList
+from sqlalchemy.orm.exc import NoResultFound
 
-from flask import current_app
+from ..exceptions import (
+    InvalidInclude,
+    InvalidSort,
+    InvalidType,
+    JsonApiException,
+    ObjectNotFound,
+    RelatedObjectNotFound,
+    RelationNotFound,
+)
+from ..schema import (
+    get_model_field,
+    get_nested_fields,
+    get_related_schema,
+    get_relationships,
+    get_schema_field,
+)
 from .base import BaseDataLayer
-from ..exceptions import RelationNotFound, RelatedObjectNotFound, JsonApiException,\
-    InvalidSort, ObjectNotFound, InvalidInclude, InvalidType
 from .filtering.alchemy import create_filters
-from ..schema import get_model_field, get_related_schema, get_relationships, get_nested_fields, get_schema_field
 
-import marshmallow
+_IS_SQLALCHEMY_1x = Version(sqlalchemy.__version__) < Version("2.0.0")
+
+
+class FlaskRestJsonApiNextWarning(UserWarning):
+    pass
 
 
 class SqlalchemyDataLayer(BaseDataLayer):
     """Sqlalchemy data layer"""
 
     def __init__(self, kwargs):
         """Initialize an instance of SqlalchemyDataLayer
 
         :param dict kwargs: initialization parameters of an SqlalchemyDataLayer instance
         """
         super(SqlalchemyDataLayer, self).__init__(kwargs)
 
-        if not hasattr(self, 'session'):
-            raise Exception("You must provide a session in data_layer_kwargs to use sqlalchemy data layer in {}"
-                            .format(self.resource.__name__))
-        if not hasattr(self, 'model'):
-            raise Exception("You must provide a model in data_layer_kwargs to use sqlalchemy data layer in {}"
-                            .format(self.resource.__name__))
+        if not hasattr(self, "session"):
+            raise Exception(
+                "You must provide a session in data_layer_kwargs to use sqlalchemy data layer in {}".format(
+                    self.resource.__name__
+                )
+            )
+        if not hasattr(self, "model"):
+            raise Exception(
+                "You must provide a model in data_layer_kwargs to use sqlalchemy data layer in {}".format(
+                    self.resource.__name__
+                )
+            )
 
     def rollback(self):
         self.session.rollback()
 
     def create_object(self, data, view_kwargs):
         """Create an object through sqlalchemy
 
@@ -52,16 +76,17 @@
         self.before_create_object(data, view_kwargs)
 
         relationship_fields = get_relationships(self.resource.schema, model_field=True)
         nested_fields = get_nested_fields(self.resource.schema, model_field=True)
 
         join_fields = relationship_fields + nested_fields
 
-        obj = self.model(**{key: value
-                            for (key, value) in data.items() if key not in join_fields})
+        obj = self.model(
+            **{key: value for (key, value) in data.items() if key not in join_fields}
+        )
         self.apply_relationships(data, obj)
         self.apply_nested_fields(data, obj)
 
         self.before_commit(obj)
 
         self.session.add(obj)
         try:
@@ -78,26 +103,28 @@
         """Retrieve an object through sqlalchemy
 
         :params dict view_kwargs: kwargs from the resource view
         :return DeclarativeMeta: an object from sqlalchemy
         """
         self.before_get_object(view_kwargs)
 
-        id_field = getattr(self, 'id_field', inspect(self.model).primary_key[0].key)
+        id_field = getattr(self, "id_field", inspect(self.model).primary_key[0].key)
         try:
             filter_field = getattr(self.model, id_field)
         except Exception:
-            raise Exception("{} has no attribute {}".format(self.model.__name__, id_field))
+            raise Exception(
+                "{} has no attribute {}".format(self.model.__name__, id_field)
+            )
 
-        url_field = getattr(self, 'url_field', 'id')
+        url_field = getattr(self, "url_field", "id")
         filter_value = view_kwargs[url_field]
 
         query = self.retrieve_object_query(view_kwargs, filter_field, filter_value)
 
-        if qs is not None and getattr(self, 'eagerload_includes', True):
+        if qs is not None and getattr(self, "eagerload_includes", True):
             query = self.eagerload_includes(query, qs)
 
         obj = query.one()
 
         self.after_get_object(obj, view_kwargs)
 
         return obj
@@ -124,15 +151,15 @@
             query = self.filter_query(query, qs.filters, self.model)
 
         if qs.sorting:
             query = self.sort_query(query, qs.sorting)
 
         object_count = query.count()
 
-        if getattr(self, 'eagerload_includes', True):
+        if getattr(self, "eagerload_includes", True):
             query = self.eagerload_includes(query, qs)
 
         query = self.paginate_query(query, qs.pagination)
 
         if as_query:
             collection = query
         else:
@@ -147,18 +174,20 @@
 
         :param DeclarativeMeta obj: an object from sqlalchemy
         :param dict data: the data validated by marshmallow
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if object have changed else False
         """
         if obj is None:
-            url_field = getattr(self, 'url_field', 'id')
+            url_field = getattr(self, "url_field", "id")
             filter_value = view_kwargs[url_field]
-            raise ObjectNotFound('{}: {} not found'.format(self.model.__name__, filter_value),
-                                 source={'parameter': url_field})
+            raise ObjectNotFound(
+                "{}: {} not found".format(self.model.__name__, filter_value),
+                source={"parameter": url_field},
+            )
 
         self.before_update_object(obj, data, view_kwargs)
 
         relationship_fields = get_relationships(self.resource.schema, model_field=True)
         nested_fields = get_nested_fields(self.resource.schema, model_field=True)
 
         join_fields = relationship_fields + nested_fields
@@ -183,316 +212,422 @@
     def delete_object(self, obj, view_kwargs):
         """Delete an object through sqlalchemy
 
         :param DeclarativeMeta item: an item from sqlalchemy
         :param dict view_kwargs: kwargs from the resource view
         """
         if obj is None:
-            url_field = getattr(self, 'url_field', 'id')
+            url_field = getattr(self, "url_field", "id")
             filter_value = view_kwargs[url_field]
-            raise ObjectNotFound('{}: {} not found'.format(self.model.__name__, filter_value),
-                                 source={'parameter': url_field})
+            raise ObjectNotFound(
+                "{}: {} not found".format(self.model.__name__, filter_value),
+                source={"parameter": url_field},
+            )
 
         self.before_delete_object(obj, view_kwargs)
 
         self.session.delete(obj)
         try:
             self.session.commit()
         except:
             self.session.rollback()
             raise
 
         self.after_delete_object(obj, view_kwargs)
 
-    def create_relationship(self, json_data, relationship_field, related_id_field, view_kwargs):
+    def create_relationship(
+        self, json_data, relationship_field, related_id_field, view_kwargs
+    ):
         """Create a relationship
 
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if relationship have changed else False
         """
-        self.before_create_relationship(json_data, relationship_field, related_id_field, view_kwargs)
+        self.before_create_relationship(
+            json_data, relationship_field, related_id_field, view_kwargs
+        )
 
         obj = self.get_object(view_kwargs)
 
         if obj is None:
-            url_field = getattr(self, 'url_field', 'id')
+            url_field = getattr(self, "url_field", "id")
             filter_value = view_kwargs[url_field]
-            raise ObjectNotFound('{}: {} not found'.format(self.model.__name__, filter_value),
-                                 source={'parameter': url_field})
+            raise ObjectNotFound(
+                "{}: {} not found".format(self.model.__name__, filter_value),
+                source={"parameter": url_field},
+            )
 
         if not hasattr(obj, relationship_field):
-            raise RelationNotFound("{} has no attribute {}".format(obj.__class__.__name__, relationship_field))
-
-        related_model = getattr(obj.__class__, relationship_field).property.mapper.class_
+            raise RelationNotFound(
+                "{} has no attribute {}".format(
+                    obj.__class__.__name__, relationship_field
+                )
+            )
+
+        related_model = getattr(
+            obj.__class__, relationship_field
+        ).property.mapper.class_
 
         updated = False
 
-        if isinstance(json_data['data'], list):
-            obj_ids = {str(getattr(obj__, related_id_field)) for obj__ in getattr(obj, relationship_field)}
-
-            for obj_ in json_data['data']:
-                if obj_['id'] not in obj_ids:
-                    getattr(obj,
-                            relationship_field).append(self.get_related_object(related_model, related_id_field, obj_))
+        if isinstance(json_data["data"], list):
+            obj_ids = {
+                str(getattr(obj__, related_id_field))
+                for obj__ in getattr(obj, relationship_field)
+            }
+
+            for obj_ in json_data["data"]:
+                if obj_["id"] not in obj_ids:
+                    getattr(obj, relationship_field).append(
+                        self.get_related_object(related_model, related_id_field, obj_)
+                    )
                     updated = True
         else:
             related_object = None
 
-            if json_data['data'] is not None:
-                related_object = self.get_related_object(related_model, related_id_field, json_data['data'])
+            if json_data["data"] is not None:
+                related_object = self.get_related_object(
+                    related_model, related_id_field, json_data["data"]
+                )
 
             obj_id = getattr(getattr(obj, relationship_field), related_id_field, None)
             new_obj_id = getattr(related_object, related_id_field, None)
             if obj_id != new_obj_id:
                 setattr(obj, relationship_field, related_object)
                 updated = True
 
         try:
             self.session.commit()
         except:
             self.session.rollback()
             raise
 
-        self.after_create_relationship(obj, updated, json_data, relationship_field, related_id_field, view_kwargs)
+        self.after_create_relationship(
+            obj, updated, json_data, relationship_field, related_id_field, view_kwargs
+        )
 
         return obj, updated
 
-    def get_relationship(self, relationship_field, related_type_, related_id_field, view_kwargs):
+    def get_relationship(
+        self, relationship_field, related_type_, related_id_field, view_kwargs
+    ):
         """Get a relationship
 
         :param str relationship_field: the model attribute used for relationship
         :param str related_type_: the related resource type
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return tuple: the object and related object(s)
         """
-        self.before_get_relationship(relationship_field, related_type_, related_id_field, view_kwargs)
+        self.before_get_relationship(
+            relationship_field, related_type_, related_id_field, view_kwargs
+        )
 
         obj = self.get_object(view_kwargs)
 
         if obj is None:
-            url_field = getattr(self, 'url_field', 'id')
+            url_field = getattr(self, "url_field", "id")
             filter_value = view_kwargs[url_field]
-            raise ObjectNotFound('{}: {} not found'.format(self.model.__name__, filter_value),
-                                 source={'parameter': url_field})
+            raise ObjectNotFound(
+                "{}: {} not found".format(self.model.__name__, filter_value),
+                source={"parameter": url_field},
+            )
 
         if not hasattr(obj, relationship_field):
-            raise RelationNotFound("{} has no attribute {}".format(obj.__class__.__name__, relationship_field))
+            raise RelationNotFound(
+                "{} has no attribute {}".format(
+                    obj.__class__.__name__, relationship_field
+                )
+            )
 
         related_objects = getattr(obj, relationship_field)
 
         if related_objects is None:
             return obj, related_objects
 
-        self.after_get_relationship(obj, related_objects, relationship_field, related_type_, related_id_field,
-                                    view_kwargs)
+        self.after_get_relationship(
+            obj,
+            related_objects,
+            relationship_field,
+            related_type_,
+            related_id_field,
+            view_kwargs,
+        )
 
         if isinstance(related_objects, InstrumentedList):
-            return obj,\
-                [{'type': related_type_, 'id': getattr(obj_, related_id_field)} for obj_ in related_objects]
+            return obj, [
+                {"type": related_type_, "id": getattr(obj_, related_id_field)}
+                for obj_ in related_objects
+            ]
         else:
-            return obj, {'type': related_type_, 'id': getattr(related_objects, related_id_field)}
-
-    def update_relationship(self, json_data, relationship_field, related_id_field, view_kwargs):
+            return obj, {
+                "type": related_type_,
+                "id": getattr(related_objects, related_id_field),
+            }
+
+    def update_relationship(
+        self, json_data, relationship_field, related_id_field, view_kwargs
+    ):
         """Update a relationship
 
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if relationship have changed else False
         """
-        self.before_update_relationship(json_data, relationship_field, related_id_field, view_kwargs)
+        self.before_update_relationship(
+            json_data, relationship_field, related_id_field, view_kwargs
+        )
 
         obj = self.get_object(view_kwargs)
 
         if obj is None:
-            url_field = getattr(self, 'url_field', 'id')
+            url_field = getattr(self, "url_field", "id")
             filter_value = view_kwargs[url_field]
-            raise ObjectNotFound('{}: {} not found'.format(self.model.__name__, filter_value),
-                                 source={'parameter': url_field})
+            raise ObjectNotFound(
+                "{}: {} not found".format(self.model.__name__, filter_value),
+                source={"parameter": url_field},
+            )
 
         if not hasattr(obj, relationship_field):
-            raise RelationNotFound("{} has no attribute {}".format(obj.__class__.__name__, relationship_field))
-
-        related_model = getattr(obj.__class__, relationship_field).property.mapper.class_
+            raise RelationNotFound(
+                "{} has no attribute {}".format(
+                    obj.__class__.__name__, relationship_field
+                )
+            )
+
+        related_model = getattr(
+            obj.__class__, relationship_field
+        ).property.mapper.class_
 
         updated = False
 
-        if isinstance(json_data['data'], list):
+        if isinstance(json_data["data"], list):
             related_objects = []
 
-            for obj_ in json_data['data']:
-                related_objects.append(self.get_related_object(related_model, related_id_field, obj_))
-
-            obj_ids = {getattr(obj__, related_id_field) for obj__ in getattr(obj, relationship_field)}
-            new_obj_ids = {getattr(related_object, related_id_field) for related_object in related_objects}
+            for obj_ in json_data["data"]:
+                related_objects.append(
+                    self.get_related_object(related_model, related_id_field, obj_)
+                )
+
+            obj_ids = {
+                getattr(obj__, related_id_field)
+                for obj__ in getattr(obj, relationship_field)
+            }
+            new_obj_ids = {
+                getattr(related_object, related_id_field)
+                for related_object in related_objects
+            }
             if obj_ids != new_obj_ids:
                 setattr(obj, relationship_field, related_objects)
                 updated = True
 
         else:
             related_object = None
 
-            if json_data['data'] is not None:
-                related_object = self.get_related_object(related_model, related_id_field, json_data['data'])
+            if json_data["data"] is not None:
+                related_object = self.get_related_object(
+                    related_model, related_id_field, json_data["data"]
+                )
 
             obj_id = getattr(getattr(obj, relationship_field), related_id_field, None)
             new_obj_id = getattr(related_object, related_id_field, None)
             if obj_id != new_obj_id:
                 setattr(obj, relationship_field, related_object)
                 updated = True
 
         try:
             self.session.commit()
         except Exception:
             self.session.rollback()
             raise
 
-        self.after_update_relationship(obj, updated, json_data, relationship_field, related_id_field, view_kwargs)
+        self.after_update_relationship(
+            obj, updated, json_data, relationship_field, related_id_field, view_kwargs
+        )
 
         return obj, updated
 
-    def delete_relationship(self, json_data, relationship_field, related_id_field, view_kwargs):
+    def delete_relationship(
+        self, json_data, relationship_field, related_id_field, view_kwargs
+    ):
         """Delete a relationship
 
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         """
-        self.before_delete_relationship(json_data, relationship_field, related_id_field, view_kwargs)
+        self.before_delete_relationship(
+            json_data, relationship_field, related_id_field, view_kwargs
+        )
 
         obj = self.get_object(view_kwargs)
 
         if obj is None:
-            url_field = getattr(self, 'url_field', 'id')
+            url_field = getattr(self, "url_field", "id")
             filter_value = view_kwargs[url_field]
-            raise ObjectNotFound('{}: {} not found'.format(self.model.__name__, filter_value),
-                                 source={'parameter': url_field})
+            raise ObjectNotFound(
+                "{}: {} not found".format(self.model.__name__, filter_value),
+                source={"parameter": url_field},
+            )
 
         if not hasattr(obj, relationship_field):
-            raise RelationNotFound("{} has no attribute {}".format(obj.__class__.__name__, relationship_field))
-
-        related_model = getattr(obj.__class__, relationship_field).property.mapper.class_
+            raise RelationNotFound(
+                "{} has no attribute {}".format(
+                    obj.__class__.__name__, relationship_field
+                )
+            )
+
+        related_model = getattr(
+            obj.__class__, relationship_field
+        ).property.mapper.class_
 
         updated = False
 
-        if isinstance(json_data['data'], list):
-            obj_ids = {str(getattr(obj__, related_id_field)) for obj__ in getattr(obj, relationship_field)}
-
-            for obj_ in json_data['data']:
-                if obj_['id'] in obj_ids:
-                    getattr(obj,
-                            relationship_field).remove(self.get_related_object(related_model, related_id_field, obj_))
+        if isinstance(json_data["data"], list):
+            obj_ids = {
+                str(getattr(obj__, related_id_field))
+                for obj__ in getattr(obj, relationship_field)
+            }
+
+            for obj_ in json_data["data"]:
+                if obj_["id"] in obj_ids:
+                    getattr(obj, relationship_field).remove(
+                        self.get_related_object(related_model, related_id_field, obj_)
+                    )
                     updated = True
         else:
             setattr(obj, relationship_field, None)
             updated = True
 
         try:
             self.session.commit()
         except JsonApiException as e:
             self.session.rollback()
             raise e
         except Exception as e:
             self.session.rollback()
             raise JsonApiException("Delete relationship error: " + str(e))
 
-        self.after_delete_relationship(obj, updated, json_data, relationship_field, related_id_field, view_kwargs)
+        self.after_delete_relationship(
+            obj, updated, json_data, relationship_field, related_id_field, view_kwargs
+        )
 
         return obj, updated
 
     def get_related_object(self, related_model, related_id_field, obj):
         """Get a related object
 
         :param Model related_model: an sqlalchemy model
         :param str related_id_field: the identifier field of the related model
         :param DeclarativeMeta obj: the sqlalchemy object to retrieve related objects from
         :return DeclarativeMeta: a related object
         """
         try:
-            related_object = self.session.query(related_model)\
-                                         .filter(getattr(related_model, related_id_field) == obj['id'])\
-                                         .one()
+            related_object = (
+                self.session.query(related_model)
+                .filter(getattr(related_model, related_id_field) == obj["id"])
+                .one()
+            )
         except NoResultFound:
-            raise RelatedObjectNotFound("{}.{}: {} not found".format(related_model.__name__,
-                                                                     related_id_field,
-                                                                     obj['id']))
+            raise RelatedObjectNotFound(
+                "{}.{}: {} not found".format(
+                    related_model.__name__, related_id_field, obj["id"]
+                )
+            )
 
         return related_object
 
-
     def apply_relationships(self, data, obj):
         """Apply relationship provided by data to obj
 
         :param dict data: data provided by the client
         :param DeclarativeMeta obj: the sqlalchemy object to plug relationships to
         :return boolean: True if relationship have changed else False
         """
         relationships_to_apply = []
         relationship_fields = get_relationships(self.resource.schema, model_field=True)
         for key, value in data.items():
             if key in relationship_fields:
                 related_model = getattr(obj.__class__, key).property.mapper.class_
                 schema_field = get_schema_field(self.resource.schema, key)
-                related_id_field = self.resource.schema._declared_fields[schema_field].id_field
+                related_id_field = self.resource.schema._declared_fields[
+                    schema_field
+                ].id_field
 
                 if isinstance(value, list):
                     related_objects = []
 
                     for identifier in value:
-                        related_object = self.get_related_object(related_model, related_id_field, {'id': identifier})
+                        related_object = self.get_related_object(
+                            related_model, related_id_field, {"id": identifier}
+                        )
                         related_objects.append(related_object)
 
-                    relationships_to_apply.append({'field': key, 'value': related_objects})
+                    relationships_to_apply.append(
+                        {"field": key, "value": related_objects}
+                    )
                 else:
                     related_object = None
 
                     if value is not None:
-                        related_object = self.get_related_object(related_model, related_id_field, {'id': value})
-
-                    relationships_to_apply.append({'field': key, 'value': related_object})
+                        related_object = self.get_related_object(
+                            related_model, related_id_field, {"id": value}
+                        )
+
+                    relationships_to_apply.append(
+                        {"field": key, "value": related_object}
+                    )
 
         for relationship in relationships_to_apply:
-            setattr(obj, relationship['field'], relationship['value'])
+            setattr(obj, relationship["field"], relationship["value"])
 
     def apply_nested_fields(self, data, obj):
         nested_fields_to_apply = []
         nested_fields = get_nested_fields(self.resource.schema, model_field=True)
         for key, value in data.items():
             if key in nested_fields:
                 nested_field_inspection = inspect(getattr(obj.__class__, key))
 
                 if not isinstance(nested_field_inspection, QueryableAttribute):
-                    raise InvalidType("Unrecognized nested field type: not a queryable attribute.")
+                    raise InvalidType(
+                        "Unrecognized nested field type: not a queryable attribute."
+                    )
 
                 if isinstance(nested_field_inspection.property, RelationshipProperty):
                     nested_model = getattr(obj.__class__, key).property.mapper.class_
 
                     if isinstance(value, list):
                         nested_objects = []
 
                         for identifier in value:
                             nested_object = nested_model(**identifier)
                             nested_objects.append(nested_object)
 
-                        nested_fields_to_apply.append({'field': key, 'value': nested_objects})
+                        nested_fields_to_apply.append(
+                            {"field": key, "value": nested_objects}
+                        )
                     else:
-                        nested_fields_to_apply.append({'field': key, 'value': nested_model(**value)})
+                        nested_fields_to_apply.append(
+                            {"field": key, "value": nested_model(**value)}
+                        )
                 elif isinstance(nested_field_inspection.property, ColumnProperty):
-                    nested_fields_to_apply.append({'field': key, 'value': value})
+                    nested_fields_to_apply.append({"field": key, "value": value})
                 else:
-                    raise InvalidType("Unrecognized nested field type: not a RelationshipProperty or ColumnProperty.")
+                    raise InvalidType(
+                        "Unrecognized nested field type: not a RelationshipProperty or ColumnProperty."
+                    )
 
         for nested_field in nested_fields_to_apply:
-            setattr(obj, nested_field['field'], nested_field['value'])
+            setattr(obj, nested_field["field"], nested_field["value"])
 
     def filter_query(self, query, filter_info, model):
         """Filter query according to jsonapi 1.0
 
         :param Query query: sqlalchemy query to sort
         :param filter_info: filter information
         :type filter_info: dict or None
@@ -509,75 +644,165 @@
         """Sort query according to jsonapi 1.0
 
         :param Query query: sqlalchemy query to sort
         :param list sort_info: sort information
         :return Query: the sorted query
         """
         for sort_opt in sort_info:
-            field = sort_opt['field']
+            field = sort_opt["field"]
             if not hasattr(self.model, field):
-                raise InvalidSort("{} has no attribute {}".format(self.model.__name__, field))
-            query = query.order_by(getattr(getattr(self.model, field), sort_opt['order'])())
+                raise InvalidSort(
+                    "{} has no attribute {}".format(self.model.__name__, field)
+                )
+            query = query.order_by(
+                getattr(getattr(self.model, field), sort_opt["order"])()
+            )
         return query
 
     def paginate_query(self, query, paginate_info):
         """Paginate query according to jsonapi 1.0
 
         :param Query query: sqlalchemy queryset
         :param dict paginate_info: pagination information
         :return Query: the paginated query
         """
-        if int(paginate_info.get('size', 1)) == 0:
+        if int(paginate_info.get("size", 1)) == 0:
             return query
 
-        page_size = int(paginate_info.get('size', 0)) or current_app.config['PAGE_SIZE']
+        page_size = int(paginate_info.get("size", 0)) or current_app.config["PAGE_SIZE"]
         query = query.limit(page_size)
-        if paginate_info.get('number'):
-            query = query.offset((int(paginate_info['number']) - 1) * page_size)
+        if paginate_info.get("number"):
+            query = query.offset((int(paginate_info["number"]) - 1) * page_size)
 
         return query
 
     def eagerload_includes(self, query, qs):
         """Use eagerload feature of sqlalchemy to optimize data retrieval for include querystring parameter
 
         :param Query query: sqlalchemy queryset
         :param QueryStringManager qs: a querystring manager to retrieve information from url
         :return Query: the query with includes eagerloaded
         """
+        if _IS_SQLALCHEMY_1x:
+            return self._legacy_eagerload_includes(query, qs)
+
+        for include in qs.include:
+            joinload_object = None
+
+            if "." in include:
+                current_schema = self.resource.schema
+                for field_name in include.split("."):
+                    joinload_object = self._field_eager_loader(
+                        current_schema, field_name, joinload_object
+                    )
+
+                    related_schema_cls = get_related_schema(current_schema, field_name)
+                    if isinstance(related_schema_cls, SchemaABC):
+                        related_schema_cls = related_schema_cls.__class__
+                    else:
+                        related_schema_cls = class_registry.get_class(
+                            related_schema_cls
+                        )
+                    current_schema = related_schema_cls
+            else:
+                joinload_object = self._field_eager_loader(
+                    self.resource.schema, include, None
+                )
+
+            if joinload_object:
+                query = query.options(joinload_object)
+
+        return query
+
+    def _field_eager_loader(self, schema, field_name, previous_loader=None):
+        try:
+            model_attribute_name = get_model_field(schema, field_name)
+        except Exception as e:
+            raise InvalidInclude(field_name)
+
+        loader = previous_loader
+        schema_meta = getattr(schema, "Meta", None)
+        model = getattr(schema_meta, "model", None)
+        model_attribute = None
+        if model:
+            try:
+                model_attribute = getattr(model, model_attribute_name)
+            except Exception as e:
+                raise InvalidInclude(model_attribute_name)
+        else:
+            warnings.warn(
+                FlaskRestJsonApiNextWarning(
+                    "When using SQLAlchemy 2.x, resource schema classes must have "
+                    "'SchemaClass.Meta.model' attribute. Without this, eager loading "
+                    "of included objects can't work and is disabled. Without eager "
+                    "loading, app may run into N + 1 query problem which will affect "
+                    f"performance. Warning for: {schema}.{field_name}."
+                )
+            )
+            return previous_loader
+
+        # schema_field = schema().fields[field_name]
+        # if hasattr(schema_field, "eager_loader_for"):
+        #     return schema_field.eager_loader_for(previous_loader)
+        # elif model_attribute:
+
+        if model_attribute:
+            if previous_loader is None:
+                loader = orm.joinedload(model_attribute)
+            else:
+                loader = previous_loader.joinedload(model_attribute)
+
+        return loader
+
+    def _legacy_eagerload_includes(self, query, qs):
+        # Broken on SQLAlchemy 2.x
+        # https://docs.sqlalchemy.org/en/20/changelog/changelog_20.html#change-c4886b74af98b72892877aefa7d6a6a4
+        #
+        # > Loader options no longer accept strings for attribute names. The
+        # > long-documented approach of using Class.attrname for loader option targets is
+        # > now standard.
         for include in qs.include:
             joinload_object = None
 
-            if '.' in include:
+            if "." in include:
                 current_schema = self.resource.schema
-                for obj in include.split('.'):
+                for obj in include.split("."):
                     try:
                         field = get_model_field(current_schema, obj)
                     except Exception as e:
                         raise InvalidInclude(str(e))
 
-                    if joinload_object is None:
-                        joinload_object = joinedload(field)
-                    else:
-                        joinload_object = joinload_object.joinedload(field)
+                    try:
+                        if joinload_object is None:
+                            joinload_object = orm.joinedload(field)
+                        else:
+                            joinload_object = joinload_object.joinedload(field)
+                    except sqlalchemy.exc.ArgumentError as e:
+                        raise InvalidInclude(str(e))
 
                     related_schema_cls = get_related_schema(current_schema, obj)
 
                     if isinstance(related_schema_cls, SchemaABC):
                         related_schema_cls = related_schema_cls.__class__
                     else:
-                        related_schema_cls = class_registry.get_class(related_schema_cls)
+                        related_schema_cls = class_registry.get_class(
+                            related_schema_cls
+                        )
 
                     current_schema = related_schema_cls
             else:
                 try:
                     field = get_model_field(self.resource.schema, include)
                 except Exception as e:
                     raise InvalidInclude(str(e))
 
-                joinload_object = joinedload(field)
+                try:
+                    joinload_object = orm.joinedload(field)
+                except sqlalchemy.exc.ArgumentError as e:
+                    raise InvalidInclude(str(e))
 
             query = query.options(joinload_object)
 
         return query
 
     def retrieve_object_query(self, view_kwargs, filter_field, filter_value):
         """Build query to retrieve object
@@ -688,103 +913,122 @@
         """Make work after delete object
 
         :param obj: an object from data layer
         :param dict view_kwargs: kwargs from the resource view
         """
         pass
 
-    def before_create_relationship(self, json_data, relationship_field, related_id_field, view_kwargs):
+    def before_create_relationship(
+        self, json_data, relationship_field, related_id_field, view_kwargs
+    ):
         """Make work before to create a relationship
 
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if relationship have changed else False
         """
         pass
 
-    def after_create_relationship(self, obj, updated, json_data, relationship_field, related_id_field, view_kwargs):
+    def after_create_relationship(
+        self, obj, updated, json_data, relationship_field, related_id_field, view_kwargs
+    ):
         """Make work after to create a relationship
 
         :param obj: an object from data layer
         :param bool updated: True if object was updated else False
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if relationship have changed else False
         """
         pass
 
-    def before_get_relationship(self, relationship_field, related_type_, related_id_field, view_kwargs):
+    def before_get_relationship(
+        self, relationship_field, related_type_, related_id_field, view_kwargs
+    ):
         """Make work before to get information about a relationship
 
         :param str relationship_field: the model attribute used for relationship
         :param str related_type_: the related resource type
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return tuple: the object and related object(s)
         """
         pass
 
-    def after_get_relationship(self, obj, related_objects, relationship_field, related_type_, related_id_field,
-                               view_kwargs):
+    def after_get_relationship(
+        self,
+        obj,
+        related_objects,
+        relationship_field,
+        related_type_,
+        related_id_field,
+        view_kwargs,
+    ):
         """Make work after to get information about a relationship
 
         :param obj: an object from data layer
         :param iterable related_objects: related objects of the object
         :param str relationship_field: the model attribute used for relationship
         :param str related_type_: the related resource type
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return tuple: the object and related object(s)
         """
         pass
 
-    def before_update_relationship(self, json_data, relationship_field, related_id_field, view_kwargs):
+    def before_update_relationship(
+        self, json_data, relationship_field, related_id_field, view_kwargs
+    ):
         """Make work before to update a relationship
 
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if relationship have changed else False
         """
         pass
 
-    def after_update_relationship(self, obj, updated, json_data, relationship_field, related_id_field, view_kwargs):
+    def after_update_relationship(
+        self, obj, updated, json_data, relationship_field, related_id_field, view_kwargs
+    ):
         """Make work after to update a relationship
 
         :param obj: an object from data layer
         :param bool updated: True if object was updated else False
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if relationship have changed else False
         """
         pass
 
-    def before_delete_relationship(self, json_data, relationship_field, related_id_field, view_kwargs):
+    def before_delete_relationship(
+        self, json_data, relationship_field, related_id_field, view_kwargs
+    ):
         """Make work before to delete a relationship
 
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         """
         pass
 
-    def after_delete_relationship(self, obj, updated, json_data, relationship_field, related_id_field, view_kwargs):
+    def after_delete_relationship(
+        self, obj, updated, json_data, relationship_field, related_id_field, view_kwargs
+    ):
         """Make work after to delete a relationship
 
         :param obj: an object from data layer
         :param bool updated: True if object was updated else False
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         """
         pass
-
-# fmt: on
```

### Comparing `flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/data_layers/base.py` & `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,48 @@
-# -*- coding: utf-8 -*-
-# isort: skip_file
-# fmt: off
-
 """The base class of a data layer. If you want to create your own data layer you must inherite from this base class"""
 
 import types
 
 
 class BaseDataLayer(object):
     """Base class of a data layer"""
 
-    REWRITABLE_METHODS = ('query',
-                          'before_create_object',
-                          'after_create_object',
-                          'before_get_object',
-                          'after_get_object',
-                          'before_get_collection',
-                          'after_get_collection',
-                          'before_update_object',
-                          'after_update_object',
-                          'before_delete_object',
-                          'after_delete_object',
-                          'before_create_relationship',
-                          'after_create_relationship',
-                          'before_get_relationship',
-                          'after_get_relationship',
-                          'before_update_relationship',
-                          'after_update_relationship',
-                          'before_delete_relationship',
-                          'after_delete_relationship',
-                          'retrieve_object_query')
+    REWRITABLE_METHODS = (
+        "query",
+        "before_create_object",
+        "after_create_object",
+        "before_get_object",
+        "after_get_object",
+        "before_get_collection",
+        "after_get_collection",
+        "before_update_object",
+        "after_update_object",
+        "before_delete_object",
+        "after_delete_object",
+        "before_create_relationship",
+        "after_create_relationship",
+        "before_get_relationship",
+        "after_get_relationship",
+        "before_update_relationship",
+        "after_update_relationship",
+        "before_delete_relationship",
+        "after_delete_relationship",
+        "retrieve_object_query",
+    )
 
     def __init__(self, kwargs):
         """Intialize an data layer instance with kwargs
 
         :param dict kwargs: information about data layer instance
         """
-        if kwargs.get('methods') is not None:
-            self.bound_rewritable_methods(kwargs['methods'])
-            kwargs.pop('methods')
+        if kwargs.get("methods") is not None:
+            self.bound_rewritable_methods(kwargs["methods"])
+            kwargs.pop("methods")
 
-        kwargs.pop('class', None)
+        kwargs.pop("class", None)
 
         for key, value in kwargs.items():
             setattr(self, key, value)
 
     def create_object(self, data, view_kwargs):
         """Create an object
 
@@ -89,48 +87,56 @@
         """Delete an item through the data layer
 
         :param DeclarativeMeta obj: an object
         :param dict view_kwargs: kwargs from the resource view
         """
         raise NotImplementedError
 
-    def create_relationship(self, json_data, relationship_field, related_id_field, view_kwargs):
+    def create_relationship(
+        self, json_data, relationship_field, related_id_field, view_kwargs
+    ):
         """Create a relationship
 
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if relationship have changed else False
         """
         raise NotImplementedError
 
-    def get_relationship(self, relationship_field, related_type_, related_id_field, view_kwargs):
+    def get_relationship(
+        self, relationship_field, related_type_, related_id_field, view_kwargs
+    ):
         """Get information about a relationship
 
         :param str relationship_field: the model attribute used for relationship
         :param str related_type_: the related resource type
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return tuple: the object and related object(s)
         """
         raise NotImplementedError
 
-    def update_relationship(self, json_data, relationship_field, related_id_field, view_kwargs):
+    def update_relationship(
+        self, json_data, relationship_field, related_id_field, view_kwargs
+    ):
         """Update a relationship
 
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if relationship have changed else False
         """
         raise NotImplementedError
 
-    def delete_relationship(self, json_data, relationship_field, related_id_field, view_kwargs):
+    def delete_relationship(
+        self, json_data, relationship_field, related_id_field, view_kwargs
+    ):
         """Delete a relationship
 
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         """
@@ -222,98 +228,119 @@
         """Make work after delete object
 
         :param obj: an object from data layer
         :param dict view_kwargs: kwargs from the resource view
         """
         raise NotImplementedError
 
-    def before_create_relationship(self, json_data, relationship_field, related_id_field, view_kwargs):
+    def before_create_relationship(
+        self, json_data, relationship_field, related_id_field, view_kwargs
+    ):
         """Make work before to create a relationship
 
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if relationship have changed else False
         """
         raise NotImplementedError
 
-    def after_create_relationship(self, obj, updated, json_data, relationship_field, related_id_field, view_kwargs):
+    def after_create_relationship(
+        self, obj, updated, json_data, relationship_field, related_id_field, view_kwargs
+    ):
         """Make work after to create a relationship
 
         :param obj: an object from data layer
         :param bool updated: True if object was updated else False
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if relationship have changed else False
         """
         raise NotImplementedError
 
-    def before_get_relationship(self, relationship_field, related_type_, related_id_field, view_kwargs):
+    def before_get_relationship(
+        self, relationship_field, related_type_, related_id_field, view_kwargs
+    ):
         """Make work before to get information about a relationship
 
         :param str relationship_field: the model attribute used for relationship
         :param str related_type_: the related resource type
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return tuple: the object and related object(s)
         """
         raise NotImplementedError
 
-    def after_get_relationship(self, obj, related_objects, relationship_field, related_type_, related_id_field,
-                               view_kwargs):
+    def after_get_relationship(
+        self,
+        obj,
+        related_objects,
+        relationship_field,
+        related_type_,
+        related_id_field,
+        view_kwargs,
+    ):
         """Make work after to get information about a relationship
 
         :param obj: an object from data layer
         :param iterable related_objects: related objects of the object
         :param str relationship_field: the model attribute used for relationship
         :param str related_type_: the related resource type
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return tuple: the object and related object(s)
         """
         raise NotImplementedError
 
-    def before_update_relationship(self, json_data, relationship_field, related_id_field, view_kwargs):
+    def before_update_relationship(
+        self, json_data, relationship_field, related_id_field, view_kwargs
+    ):
         """Make work before to update a relationship
 
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if relationship have changed else False
         """
         raise NotImplementedError
 
-    def after_update_relationship(self, obj, updated, json_data, relationship_field, related_id_field, view_kwargs):
+    def after_update_relationship(
+        self, obj, updated, json_data, relationship_field, related_id_field, view_kwargs
+    ):
         """Make work after to update a relationship
 
         :param obj: an object from data layer
         :param bool updated: True if object was updated else False
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if relationship have changed else False
         """
         raise NotImplementedError
 
-    def before_delete_relationship(self, json_data, relationship_field, related_id_field, view_kwargs):
+    def before_delete_relationship(
+        self, json_data, relationship_field, related_id_field, view_kwargs
+    ):
         """Make work before to delete a relationship
 
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         """
         raise NotImplementedError
 
-    def after_delete_relationship(self, obj, updated, json_data, relationship_field, related_id_field, view_kwargs):
+    def after_delete_relationship(
+        self, obj, updated, json_data, relationship_field, related_id_field, view_kwargs
+    ):
         """Make work after to delete a relationship
 
         :param obj: an object from data layer
         :param bool updated: True if object was updated else False
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
@@ -331,9 +358,7 @@
         """Bound additional methods to current instance
 
         :param class meta: information from Meta class used to configure the data layer instance
         """
         for key, value in methods.items():
             if key in self.REWRITABLE_METHODS:
                 setattr(self, key, types.MethodType(value, self))
-
-# fmt: on
```

### Comparing `flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/data_layers/filtering/alchemy.py` & `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/filtering/alchemy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-# -*- coding: utf-8 -*-
-# isort: skip_file
-# fmt: off
-
 """Helper to create sqlalchemy filters according to filter querystring parameter"""
 
-from sqlalchemy import and_, or_, not_
+from sqlalchemy import and_, not_, or_
 
 from ...exceptions import InvalidFilters
-from ...schema import get_relationships, get_nested_fields, get_model_field
+from ...schema import get_model_field, get_nested_fields, get_relationships
 
 
 def create_filters(model, filter_info, resource):
     """Apply filters from filters information to base query
 
     :param DeclarativeMeta model: the model of the node
     :param dict filter_info: current node filter information
@@ -38,65 +34,83 @@
         self.model = model
         self.filter_ = filter_
         self.resource = resource
         self.schema = schema
 
     def resolve(self):
         """Create filter for a particular node of the filter tree"""
-        if 'or' not in self.filter_ and 'and' not in self.filter_ and 'not' not in self.filter_:
+        if (
+            "or" not in self.filter_
+            and "and" not in self.filter_
+            and "not" not in self.filter_
+        ):
             value = self.value
 
             if self.operator == "between":
                 return self.column.between(*value)
 
             if isinstance(value, dict):
-                value = Node(self.related_model, value, self.resource, self.related_schema).resolve()
+                value = Node(
+                    self.related_model, value, self.resource, self.related_schema
+                ).resolve()
 
-            if '__' in self.filter_.get('name', ''):
-                value = {self.filter_['name'].split('__')[1]: value}
+            if "__" in self.filter_.get("name", ""):
+                value = {self.filter_["name"].split("__")[1]: value}
 
             if isinstance(value, dict):
                 return getattr(self.column, self.operator)(**value)
             else:
                 return getattr(self.column, self.operator)(value)
 
-        if 'or' in self.filter_:
-            return or_(Node(self.model, filt, self.resource, self.schema).resolve() for filt in self.filter_['or'])
-        if 'and' in self.filter_:
-            return and_(Node(self.model, filt, self.resource, self.schema).resolve() for filt in self.filter_['and'])
-        if 'not' in self.filter_:
-            return not_(Node(self.model, self.filter_['not'], self.resource, self.schema).resolve())
+        if "or" in self.filter_:
+            return or_(
+                Node(self.model, filt, self.resource, self.schema).resolve()
+                for filt in self.filter_["or"]
+            )
+        if "and" in self.filter_:
+            return and_(
+                Node(self.model, filt, self.resource, self.schema).resolve()
+                for filt in self.filter_["and"]
+            )
+        if "not" in self.filter_:
+            return not_(
+                Node(
+                    self.model, self.filter_["not"], self.resource, self.schema
+                ).resolve()
+            )
 
     @property
     def name(self):
         """Return the name of the node or raise a BadRequest exception
 
         :return str: the name of the field to filter on
         """
-        name = self.filter_.get('name')
+        name = self.filter_.get("name")
 
         if name is None:
             raise InvalidFilters("Can't find name of a filter")
 
-        if '__' in name:
-            name = name.split('__')[0]
+        if "__" in name:
+            name = name.split("__")[0]
 
         if name not in self.schema._declared_fields:
-            raise InvalidFilters("{} has no attribute {}".format(self.schema.__name__, name))
+            raise InvalidFilters(
+                "{} has no attribute {}".format(self.schema.__name__, name)
+            )
 
         return name
 
     @property
     def op(self):
         """Return the operator of the node
 
         :return str: the operator to use in the filter
         """
         try:
-            return self.filter_['op']
+            return self.filter_["op"]
         except KeyError:
             raise InvalidFilters("Can't find op of a filter")
 
     @property
     def column(self):
         """Get the column object
 
@@ -107,70 +121,84 @@
         field = self.name
 
         model_field = get_model_field(self.schema, field)
 
         try:
             return getattr(self.model, model_field)
         except AttributeError:
-            raise InvalidFilters("{} has no attribute {}".format(self.model.__name__, model_field))
+            raise InvalidFilters(
+                "{} has no attribute {}".format(self.model.__name__, model_field)
+            )
 
     @property
     def operator(self):
         """Get the function operator from his name
 
         :return callable: a callable to make operation on a column
         """
-        operators = (self.op, self.op + '_', '__' + self.op + '__')
+        operators = (self.op, self.op + "_", "__" + self.op + "__")
 
         for op in operators:
             if hasattr(self.column, op):
                 return op
 
         raise InvalidFilters("{} has no operator {}".format(self.column.key, self.op))
 
     @property
     def value(self):
         """Get the value to filter on
 
         :return: the value to filter on
         """
-        if self.filter_.get('field') is not None:
+        if self.filter_.get("field") is not None:
             try:
-                result = getattr(self.model, self.filter_['field'])
+                result = getattr(self.model, self.filter_["field"])
             except AttributeError:
-                raise InvalidFilters("{} has no attribute {}".format(self.model.__name__, self.filter_['field']))
+                raise InvalidFilters(
+                    "{} has no attribute {}".format(
+                        self.model.__name__, self.filter_["field"]
+                    )
+                )
             else:
                 return result
         else:
-            if 'val' not in self.filter_:
+            if "val" not in self.filter_:
                 raise InvalidFilters("Can't find value or field in a filter")
 
-            return self.filter_['val']
+            return self.filter_["val"]
 
     @property
     def related_model(self):
         """Get the related model of a related (relationship or nested) field
 
         :return DeclarativeMeta: the related model
         """
         related_field_name = self.name
 
         related_fields = get_relationships(self.schema) + get_nested_fields(self.schema)
         if related_field_name not in related_fields:
-            raise InvalidFilters("{} has no relationship or nested attribute {}".format(self.schema.__name__, related_field_name))
-
-        return getattr(self.model, get_model_field(self.schema, related_field_name)).property.mapper.class_
+            raise InvalidFilters(
+                "{} has no relationship or nested attribute {}".format(
+                    self.schema.__name__, related_field_name
+                )
+            )
+
+        return getattr(
+            self.model, get_model_field(self.schema, related_field_name)
+        ).property.mapper.class_
 
     @property
     def related_schema(self):
         """Get the related schema of a related (relationship or nested) field
 
         :return Schema: the related schema
         """
         related_field_name = self.name
         related_fields = get_relationships(self.schema) + get_nested_fields(self.schema)
         if related_field_name not in related_fields:
-            raise InvalidFilters("{} has no relationship or nested attribute {}".format(self.schema.__name__, related_field_name))
+            raise InvalidFilters(
+                "{} has no relationship or nested attribute {}".format(
+                    self.schema.__name__, related_field_name
+                )
+            )
 
         return self.schema._declared_fields[related_field_name].schema.__class__
-
-# fmt: on
```

### Comparing `flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/decorators.py` & `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/decorators.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,78 +1,76 @@
-# -*- coding: utf-8 -*-
-# isort: skip_file
-# fmt: off
-
 """Decorators to check headers and method requirements for each Api calls"""
 
-import json
 from functools import wraps
 
-from flask import request, make_response, jsonify, current_app
+from flask import current_app, request
 
-from .errors import jsonapi_errors
 from .exceptions import JsonApiException
 
 
 def check_headers(func):
     """Check headers according to jsonapi reference
 
     :param callable func: the function to decorate
     :return callable: the wrapped function
     """
+
     @wraps(func)
     def wrapper(*args, **kwargs):
-        if request.method in ('POST', 'PATCH'):
-            if (
-                'Content-Type' not in request.headers
-                or (
-                    request.mimetype != 'application/vnd.api+json'
-                    and request.mimetype != 'application/json'
-                    and request.mimetype != 'multipart/form-data'
-                )
+        if request.method in ("POST", "PATCH"):
+            if "Content-Type" not in request.headers or (
+                request.mimetype != "application/vnd.api+json"
+                and request.mimetype != "application/json"
+                and request.mimetype != "multipart/form-data"
             ):
                 raise JsonApiException(
                     detail="Content-Type header must be application/vnd.api+json or application/json or multipart/form-data",
                     title="Invalid request header",
                     status=415,
                 )
 
-        if 'Accept' in request.headers:
+        if "Accept" in request.headers:
             flag = False
-            for accept in request.headers['Accept'].split(','):
-                if accept.strip() == 'application/vnd.api+json':
+            for accept in request.headers["Accept"].split(","):
+                if accept.strip() == "application/vnd.api+json":
                     flag = False
                     break
-                if 'application/vnd.api+json' in accept and accept.strip() != 'application/vnd.api+json':
+                if (
+                    "application/vnd.api+json" in accept
+                    and accept.strip() != "application/vnd.api+json"
+                ):
                     flag = True
             if flag is True:
                 raise JsonApiException(
                     detail="Accept header must be application/vnd.api+json without media type parameters",
                     title="Invalid request header",
                     status=406,
                 )
 
         return func(*args, **kwargs)
+
     return wrapper
 
 
 def check_method_requirements(func):
     """Check methods requirements
 
     :param callable func: the function to decorate
     :return callable: the wrapped function
     """
+
     @wraps(func)
     def wrapper(*args, **kwargs):
         error_message = "You must provide {error_field} in {cls} to get access to the default {method} method"
-        error_data = {'cls': args[0].__class__.__name__,
-                      'method': request.method.lower()}
-
-        if request.method != 'DELETE':
-            if not hasattr(args[0], 'schema'):
-                error_data.update({'error_field': 'a schema class'})
+        error_data = {
+            "cls": args[0].__class__.__name__,
+            "method": request.method.lower(),
+        }
+
+        if request.method != "DELETE":
+            if not hasattr(args[0], "schema"):
+                error_data.update({"error_field": "a schema class"})
                 raise Exception(error_message.format(**error_data))
 
         return func(*args, **kwargs)
-    return wrapper
 
-# fmt: on
+    return wrapper
```

### Comparing `flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/error_responses/error_formatters.py` & `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/error_formatters.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/error_responses/errors_as_json_api.py` & `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/errors_as_json_api.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/error_responses/exception_converters/marshamallow.py` & `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/marshamallow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import marshmallow
 import marshmallow_jsonapi
 import requests
 
 from .base import ExceptionConverter
 
 
-class MarshmallowValidationErrorConverter(ExceptionConverter):
+class _MarshmallowValidationErrorConverter(ExceptionConverter):
     @classmethod
     def convert(cls, exc):
         if not isinstance(exc, marshmallow.ValidationError):
             raise ValueError()
 
         retv = []
         messages = exc.normalized_messages()
@@ -29,15 +29,15 @@
         for _ in retv:
             _["title"] = _.get("title", "ValidationError")
             _["http_status"] = requests.codes["unprocessable"]
 
         return retv
 
 
-class MarshmallowJsonapiIncorrectTypeErrorConverter(ExceptionConverter):
+class _MarshmallowJsonapiIncorrectTypeErrorConverter(ExceptionConverter):
     @classmethod
     def convert(cls, exc):
         if not isinstance(exc, marshmallow_jsonapi.exceptions.IncorrectTypeError):
             raise ValueError()
 
         return dict(
             title="IncorrectTypeError",
```

### Comparing `flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/error_responses/exceptions.py` & `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exceptions.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/exceptions.py` & `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-# -*- coding: utf-8 -*-
-# isort: skip_file
-# fmt: off
-
 """Collection of useful http error for the Api"""
 
 
 class JsonApiException(Exception):
     """Base exception class for unknown errors"""
 
-    title = 'Unknown error'
-    status = '500'
+    title = "Unknown error"
+    status = "500"
     source = None
 
-    def __init__(self, detail="", source=None, title=None, status=None, code=None, id_=None, links=None, meta=None):
+    def __init__(
+        self,
+        detail="",
+        source=None,
+        title=None,
+        status=None,
+        code=None,
+        id_=None,
+        links=None,
+        meta=None,
+    ):
         """Initialize a jsonapi exception
 
         :param dict source: the source of the error
         :param str detail: the detail of the error
         """
         self.detail = detail
         if source is not None:
@@ -29,84 +35,91 @@
             self.title = title
         if status is not None:
             self.status = status
 
     def to_dict(self):
         """Return values of each fields of an jsonapi error"""
         error_dict = {}
-        for field in ('status', 'source', 'title', 'detail', 'id', 'code', 'links', 'meta'):
+        for field in (
+            "status",
+            "source",
+            "title",
+            "detail",
+            "id",
+            "code",
+            "links",
+            "meta",
+        ):
             if getattr(self, field, None):
                 error_dict.update({field: getattr(self, field)})
 
         return error_dict
 
 
 class BadRequest(JsonApiException):
     """BadRequest error"""
 
-    title = 'Bad request'
-    status = '400'
+    title = "Bad request"
+    status = "400"
 
 
 class InvalidField(BadRequest):
     """Error to warn that a field specified in fields querystring is not in the requested resource schema"""
 
     title = "Invalid fields querystring parameter."
-    source = {'parameter': 'fields'}
+    source = {"parameter": "fields"}
 
 
 class InvalidInclude(BadRequest):
     """Error to warn that a field specified in include querystring parameter is not a relationship of the requested
     resource schema
     """
 
-    title = 'Invalid include querystring parameter.'
-    source = {'parameter': 'include'}
+    title = "Invalid include querystring parameter."
+    source = {"parameter": "include"}
 
 
 class InvalidFilters(BadRequest):
     """Error to warn that a specified filters in querystring parameter contains errors"""
 
-    title = 'Invalid filters querystring parameter.'
-    source = {'parameter': 'filter'}
+    title = "Invalid filters querystring parameter."
+    source = {"parameter": "filter"}
 
 
 class InvalidSort(BadRequest):
     """Error to warn that a field specified in sort querystring parameter is not in the requested resource schema"""
 
-    title = 'Invalid sort querystring parameter.'
-    source = {'parameter': 'sort'}
+    title = "Invalid sort querystring parameter."
+    source = {"parameter": "sort"}
 
 
 class ObjectNotFound(JsonApiException):
     """Error to warn that an object is not found in a database"""
 
-    title = 'Object not found'
-    status = '404'
+    title = "Object not found"
+    status = "404"
 
 
 class RelatedObjectNotFound(ObjectNotFound):
     """Error to warn that a related object is not found"""
 
-    title = 'Related object not found'
+    title = "Related object not found"
 
 
 class RelationNotFound(JsonApiException):
     """Error to warn that a relationship is not found on a model"""
 
-    title = 'Relation not found'
+    title = "Relation not found"
 
 
 class InvalidType(JsonApiException):
     """Error to warn that there is a conflit between resource types"""
 
-    title = 'Invalid type'
-    status = '409'
+    title = "Invalid type"
+    status = "409"
 
 
 class AccessDenied(JsonApiException):
     """Throw this error when requested resource owner doesn't match the user of the ticket"""
 
-    title = 'Access denied'
-    status = '403'
-
-# fmt: on
+    title = "Access denied"
+    status = "403"
```

### Comparing `flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/pagination.py` & `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/pagination.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-# -*- coding: utf-8 -*-
-# isort: skip_file
-# fmt: off
-
 """Helper to create pagination links according to jsonapi specification"""
 
 from __future__ import division
-from six.moves.urllib.parse import urlencode
-from math import ceil
+
 from copy import copy
+from math import ceil
+from urllib.parse import urlencode
 
 from flask import current_app
 
 
 def add_pagination_links(data, object_count, querystring, base_url):
     """Add pagination links to result
 
@@ -19,42 +16,43 @@
     :param int object_count: number of objects in result
     :param QueryStringManager querystring: the managed querystring fields and values
     :param str base_url: the base url for pagination
     """
     links = {}
     all_qs_args = copy(querystring.querystring)
 
-    links['self'] = base_url
+    links["self"] = base_url
 
     # compute self link
     if all_qs_args:
-        links['self'] += '?' + urlencode(all_qs_args)
+        links["self"] += "?" + urlencode(all_qs_args)
 
-    if querystring.pagination.get('size') != '0' and object_count > 1:
+    if querystring.pagination.get("size") != "0" and object_count > 1:
         # compute last link
-        page_size = int(querystring.pagination.get('size', 0)) or current_app.config['PAGE_SIZE']
+        page_size = (
+            int(querystring.pagination.get("size", 0))
+            or current_app.config["PAGE_SIZE"]
+        )
         last_page = int(ceil(object_count / page_size))
 
         if last_page > 1:
-            links['first'] = links['last'] = base_url
+            links["first"] = links["last"] = base_url
 
-            all_qs_args.pop('page[number]', None)
+            all_qs_args.pop("page[number]", None)
 
             # compute first link
             if all_qs_args:
-                links['first'] += '?' + urlencode(all_qs_args)
+                links["first"] += "?" + urlencode(all_qs_args)
 
-            all_qs_args.update({'page[number]': last_page})
-            links['last'] += '?' + urlencode(all_qs_args)
+            all_qs_args.update({"page[number]": last_page})
+            links["last"] += "?" + urlencode(all_qs_args)
 
             # compute previous and next link
-            current_page = int(querystring.pagination.get('number', 0)) or 1
+            current_page = int(querystring.pagination.get("number", 0)) or 1
             if current_page > 1:
-                all_qs_args.update({'page[number]': current_page - 1})
-                links['prev'] = '?'.join((base_url, urlencode(all_qs_args)))
+                all_qs_args.update({"page[number]": current_page - 1})
+                links["prev"] = "?".join((base_url, urlencode(all_qs_args)))
             if current_page < last_page:
-                all_qs_args.update({'page[number]': current_page + 1})
-                links['next'] = '?'.join((base_url, urlencode(all_qs_args)))
-
-    data['links'] = links
+                all_qs_args.update({"page[number]": current_page + 1})
+                links["next"] = "?".join((base_url, urlencode(all_qs_args)))
 
-# fmt: on
+    data["links"] = links
```

### Comparing `flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/querystring.py` & `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/querystring.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-# -*- coding: utf-8 -*-
-# isort: skip_file
-# fmt: off
-
 """Helper to deal with querystring parameters according to jsonapi specification"""
 
 import json
 
 from flask import current_app
 
-from .exceptions import BadRequest, InvalidFilters, InvalidSort, InvalidField, InvalidInclude
+from .exceptions import (
+    BadRequest,
+    InvalidField,
+    InvalidFilters,
+    InvalidInclude,
+    InvalidSort,
+)
 from .schema import get_model_field, get_relationships, get_schema_from_type
 
 
 class QueryStringManager(object):
     """Querystring parser according to jsonapi reference"""
 
-    MANAGED_KEYS = (
-        'filter',
-        'page',
-        'fields',
-        'sort',
-        'include',
-        'q'
-    )
+    MANAGED_KEYS = ("filter", "page", "fields", "sort", "include", "q")
 
-    def __init__(self, querystring, schema, allow_disable_pagination=None, max_page_size=None):
+    def __init__(
+        self, querystring, schema, allow_disable_pagination=None, max_page_size=None
+    ):
         """Initialization instance
 
         :param dict querystring: query string dict from request.args
         """
         if not isinstance(querystring, dict):
-            raise ValueError('QueryStringManager require a dict-like object querystring parameter')
+            raise ValueError(
+                "QueryStringManager require a dict-like object querystring parameter"
+            )
 
         self.qs = querystring
         self.schema = schema
 
         self.allow_disable_pagination = allow_disable_pagination
         self.max_page_size = max_page_size
 
@@ -47,65 +46,68 @@
         results = {}
 
         for key, value in self.qs.items():
             try:
                 if not key.startswith(name):
                     continue
 
-                key_start = key.index('[') + 1
-                key_end = key.index(']')
+                key_start = key.index("[") + 1
+                key_end = key.index("]")
                 item_key = key[key_start:key_end]
 
-                if ',' in value:
-                    item_value = value.split(',')
+                if "," in value:
+                    item_value = value.split(",")
                 else:
                     item_value = value
                 results.update({item_key: item_value})
             except Exception:
-                raise BadRequest("Parse error", source={'parameter': key})
+                raise BadRequest("Parse error", source={"parameter": key})
 
         return results
 
     def _simple_filters(self, dict_):
         """Return filter list
 
         :return list: list of dict for filter parameters. Includes support for 'in' for list values
         """
         filter_list = []
-        for (key, value) in dict_.items():
-            operator = 'eq'
+        for key, value in dict_.items():
+            operator = "eq"
             if isinstance(value, list):
-                operator = 'in'
+                operator = "in"
             filter_list.append({"name": key, "op": operator, "val": value})
         return filter_list
 
     @property
     def querystring(self):
         """Return original querystring but containing only managed keys
 
         :return dict: dict of managed querystring parameter
         """
-        return {key: value for (key, value) in self.qs.items()
-                if key.startswith(self.MANAGED_KEYS) or self._get_key_values('filter[')}
+        return {
+            key: value
+            for (key, value) in self.qs.items()
+            if key.startswith(self.MANAGED_KEYS) or self._get_key_values("filter[")
+        }
 
     @property
     def filters(self):
         """Return filters from query string.
 
         :return list: filter information
         """
         results = []
-        filters = self.qs.get('filter')
+        filters = self.qs.get("filter")
         if filters is not None:
             try:
                 results.extend(json.loads(filters))
             except (ValueError, TypeError):
                 raise InvalidFilters("Parse error")
-        if self._get_key_values('filter['):
-            results.extend(self._simple_filters(self._get_key_values('filter[')))
+        if self._get_key_values("filter["):
+            results.extend(self._simple_filters(self._get_key_values("filter[")))
         return results
 
     @property
     def pagination(self):
         """Return all page parameters as a dict.
 
         :return dict: a dict of pagination information
@@ -120,38 +122,48 @@
         Example with number strategy::
 
             >>> query_string = {'page[number]': '25', 'page[size]': '10'}
             >>> parsed_query.pagination
             {'number': '25', 'size': '10'}
         """
         # check values type
-        result = self._get_key_values('page')
+        result = self._get_key_values("page")
         for key, value in result.items():
-            if key not in ('number', 'size'):
-                raise BadRequest("{} is not a valid parameter of pagination".format(key), source={'parameter': 'page'})
+            if key not in ("number", "size"):
+                raise BadRequest(
+                    "{} is not a valid parameter of pagination".format(key),
+                    source={"parameter": "page"},
+                )
             try:
                 int(value)
             except ValueError:
-                raise BadRequest("Parse error", source={'parameter': 'page[{}]'.format(key)})
+                raise BadRequest(
+                    "Parse error", source={"parameter": "page[{}]".format(key)}
+                )
 
         if self.allow_disable_pagination is None:
             self.allow_disable_pagination = current_app.config.get(
-                'ALLOW_DISABLE_PAGINATION', True
+                "ALLOW_DISABLE_PAGINATION", True
             )
 
         if self.max_page_size is None:
-            self.max_page_size = current_app.config.get('MAX_PAGE_SIZE', None)
+            self.max_page_size = current_app.config.get("MAX_PAGE_SIZE", None)
 
-        if not self.allow_disable_pagination and int(result.get('size', 1)) == 0:
-            raise BadRequest("You are not allowed to disable pagination", source={'parameter': 'page[size]'})
+        if not self.allow_disable_pagination and int(result.get("size", 1)) == 0:
+            raise BadRequest(
+                "You are not allowed to disable pagination",
+                source={"parameter": "page[size]"},
+            )
 
-        if self.max_page_size is not None and 'size' in result:
-            if int(result['size']) > self.max_page_size:
-                raise BadRequest(f"Maximum page size is {self.max_page_size}",
-                                 source={'parameter': 'page[size]'})
+        if self.max_page_size is not None and "size" in result:
+            if int(result["size"]) > self.max_page_size:
+                raise BadRequest(
+                    f"Maximum page size is {self.max_page_size}",
+                    source={"parameter": "page[size]"},
+                )
 
         return result
 
     @property
     def fields(self):
         """Return fields wanted by client.
 
@@ -160,24 +172,26 @@
         Return value will be a dict containing all fields by resource, for example::
 
             {
                 "user": ['name', 'email'],
             }
 
         """
-        result = self._get_key_values('fields')
+        result = self._get_key_values("fields")
         for key, value in result.items():
             if not isinstance(value, list):
                 result[key] = [value]
 
         for key, value in result.items():
             schema = get_schema_from_type(key)
             for obj in value:
                 if obj not in schema._declared_fields:
-                    raise InvalidField("{} has no attribute {}".format(schema.__name__, obj))
+                    raise InvalidField(
+                        "{} has no attribute {}".format(schema.__name__, obj)
+                    )
 
         return result
 
     @property
     def sorting(self):
         """Return fields to sort by including sort name for SQLAlchemy and row
         sort parameter for other ORMs
@@ -187,39 +201,49 @@
         Example of return value::
 
             [
                 {'field': 'created_at', 'order': 'desc'},
             ]
 
         """
-        if self.qs.get('sort'):
+        if self.qs.get("sort"):
             sorting_results = []
-            for sort_field in self.qs['sort'].split(','):
-                field = sort_field.replace('-', '')
+            for sort_field in self.qs["sort"].split(","):
+                field = sort_field.replace("-", "")
                 if field not in self.schema._declared_fields:
-                    raise InvalidSort("{} has no attribute {}".format(self.schema.__name__, field))
+                    raise InvalidSort(
+                        "{} has no attribute {}".format(self.schema.__name__, field)
+                    )
                 if field in get_relationships(self.schema):
-                    raise InvalidSort("You can't sort on {} because it is a relationship field".format(field))
+                    raise InvalidSort(
+                        "You can't sort on {} because it is a relationship field".format(
+                            field
+                        )
+                    )
                 field = get_model_field(self.schema, field)
-                order = 'desc' if sort_field.startswith('-') else 'asc'
-                sorting_results.append({'field': field, 'order': order})
+                order = "desc" if sort_field.startswith("-") else "asc"
+                sorting_results.append({"field": field, "order": order})
             return sorting_results
 
         return []
 
     @property
     def include(self):
         """Return fields to include
 
         :return list: a list of include information
         """
-        include_param = self.qs.get('include', [])
+        include_param = self.qs.get("include", [])
 
-        if current_app.config.get('MAX_INCLUDE_DEPTH') is not None:
+        if current_app.config.get("MAX_INCLUDE_DEPTH") is not None:
             for include_path in include_param:
-                if len(include_path.split('.')) > current_app.config['MAX_INCLUDE_DEPTH']:
-                    raise InvalidInclude("You can't use include through more than {} relationships"
-                                         .format(current_app.config['MAX_INCLUDE_DEPTH']))
-
-        return include_param.split(',') if include_param else []
+                if (
+                    len(include_path.split("."))
+                    > current_app.config["MAX_INCLUDE_DEPTH"]
+                ):
+                    raise InvalidInclude(
+                        "You can't use include through more than {} relationships".format(
+                            current_app.config["MAX_INCLUDE_DEPTH"]
+                        )
+                    )
 
-# fmt: on
+        return include_param.split(",") if include_param else []
```

### Comparing `flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/resource.py` & `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/resource.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,52 @@
-# -*- coding: utf-8 -*-
-# isort: skip_file
-# fmt: off
-
 """This module contains the logic of resource management"""
 
 import inspect
 import re
 
-from werkzeug.wrappers import Response
 import flask
-from flask import request, url_for, make_response
-from flask.wrappers import Response as FlaskResponse
+from flask import make_response, request, url_for
 from flask.views import MethodView
-from marshmallow_jsonapi.exceptions import IncorrectTypeError
-from marshmallow import ValidationError
-
-from .querystring import QueryStringManager as QSManager
-from .pagination import add_pagination_links
-from .exceptions import InvalidType, BadRequest, RelationNotFound
-from .decorators import check_headers, check_method_requirements
-from .schema import compute_schema, get_relationships, get_model_field
-from .data_layers.base import BaseDataLayer
-from .data_layers.alchemy import SqlalchemyDataLayer
+from flask.wrappers import Response as FlaskResponse
 from marshmallow_jsonapi.fields import BaseRelationship
 from werkzeug.datastructures import ImmutableMultiDict
+from werkzeug.wrappers import Response
+
+from .data_layers.alchemy import SqlalchemyDataLayer
+from .data_layers.base import BaseDataLayer
+from .decorators import check_headers, check_method_requirements
+from .exceptions import BadRequest, InvalidType, RelationNotFound
+from .pagination import add_pagination_links
+from .querystring import QueryStringManager as QSManager
+from .schema import compute_schema, get_model_field, get_relationships
 
 
 class Resource(MethodView):
     """Base resource class"""
 
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
 
         if "data_layer" in cls.__dict__:
             if not isinstance(cls.__dict__["data_layer"], dict):
                 raise RuntimeError(f"{cls.__name__}.data_layer must be dict!")
 
-            if (
-                cls.__dict__['data_layer'].get('class') is not None
-                and BaseDataLayer not in inspect.getmro(
-                    cls.__dict__['data_layer']['class']
-                )
+            if cls.__dict__["data_layer"].get(
+                "class"
+            ) is not None and BaseDataLayer not in inspect.getmro(
+                cls.__dict__["data_layer"]["class"]
             ):
                 raise RuntimeError(
                     f"{cls.__name__}.data_layer['class'] must be inherited from BaseDataLayer!"
                 )
 
-            data_layer_cls = cls.__dict__['data_layer'].get('class', SqlalchemyDataLayer)
-            data_layer_kwargs = cls.__dict__['data_layer']
+            data_layer_cls = cls.__dict__["data_layer"].get(
+                "class", SqlalchemyDataLayer
+            )
+            data_layer_kwargs = cls.__dict__["data_layer"]
             cls._data_layer = data_layer_cls(data_layer_kwargs)
             cls._data_layer.resource = cls
 
         decorators = [check_headers]
 
         for base_cls in cls.mro():
             for dcrtr in getattr(base_cls, "decorators", []) or []:
@@ -59,62 +54,61 @@
                     decorators.append(dcrtr)
 
         if "decorators" in cls.__dict__:
             decorators.extend(cls.decorators)
 
         cls.decorators = tuple(decorators)
 
-
     def dispatch_request(self, *args, **kwargs):
         """Logic of how to handle a request"""
         method = getattr(self, request.method.lower(), None)
-        if method is None and request.method == 'HEAD':
-            method = getattr(self, 'get', None)
-        assert method is not None, 'Unimplemented method {}'.format(request.method)
+        if method is None and request.method == "HEAD":
+            method = getattr(self, "get", None)
+        assert method is not None, "Unimplemented method {}".format(request.method)
 
-        headers = {'Content-Type': 'application/vnd.api+json'}
+        headers = {"Content-Type": "application/vnd.api+json"}
 
         response = method(*args, **kwargs)
 
         if isinstance(response, Response):
             if "Content-Type" not in response.headers:
-                response.headers.add('Content-Type', 'application/vnd.api+json')
+                response.headers.add("Content-Type", "application/vnd.api+json")
             return response
 
         if not isinstance(response, tuple):
             if isinstance(response, dict):
-                response.update({'jsonapi': {'version': '1.0'}})
+                response.update({"jsonapi": {"version": "1.0"}})
             return make_response(flask.json.dumps(response), 200, headers)
 
         try:
             data, status_code, headers = response
             if "Content-Type" not in headers:
-                headers.update({'Content-Type': 'application/vnd.api+json'})
+                headers.update({"Content-Type": "application/vnd.api+json"})
         except ValueError:
             pass
 
         try:
             data, status_code = response
         except ValueError:
             pass
 
         if isinstance(data, dict):
-            data.update({'jsonapi': {'version': '1.0'}})
+            data.update({"jsonapi": {"version": "1.0"}})
 
         if isinstance(data, FlaskResponse):
             if "Content-Type" not in data.headers:
-                data.headers.add('Content-Type', 'application/vnd.api+json')
+                data.headers.add("Content-Type", "application/vnd.api+json")
             data.status_code = status_code
             return data
         elif isinstance(data, str):
-            json_reponse = data
+            json_response = data
         else:
-            json_reponse = flask.json.dumps(data)
+            json_response = flask.json.dumps(data)
 
-        return make_response(json_reponse, status_code, headers)
+        return make_response(json_response, status_code, headers)
 
 
 class ResourceList(Resource):
     """Base class of a resource list manager"""
 
     @check_method_requirements
     def get(self, *args, **kwargs):
@@ -122,82 +116,84 @@
         self.before_get(args, kwargs)
 
         qs = QSManager(request.args, self.schema)
 
         parent_filter = self._get_parent_filter(request.url, kwargs)
         objects_count, objects = self.get_collection(qs, kwargs, filters=parent_filter)
 
-        schema_kwargs = getattr(self, 'get_schema_kwargs', dict())
-        schema_kwargs.update({'many': True})
+        schema_kwargs = getattr(self, "get_schema_kwargs", dict())
+        schema_kwargs.update({"many": True})
 
         self.before_marshmallow(args, kwargs)
 
-        schema = compute_schema(self.schema,
-                                schema_kwargs,
-                                qs,
-                                qs.include)
+        schema = compute_schema(self.schema, schema_kwargs, qs, qs.include)
 
         result = schema.dump(objects)
 
-        view_kwargs = request.view_args if getattr(self, 'view_kwargs', None) is True else dict()
-        add_pagination_links(result,
-                             objects_count,
-                             qs,
-                             url_for(self.view, _external=True, **view_kwargs))
+        view_kwargs = (
+            request.view_args if getattr(self, "view_kwargs", None) is True else dict()
+        )
+        add_pagination_links(
+            result, objects_count, qs, url_for(self.view, _external=True, **view_kwargs)
+        )
 
-        result.update({'meta': {'count': objects_count}})
+        result.update({"meta": {"count": objects_count}})
 
         final_result = self.after_get(result)
 
         return final_result
 
     @check_method_requirements
     def post(self, *args, **kwargs):
         """Create an object"""
         json_data = request.get_json() or {}
 
         qs = QSManager(request.args, self.schema)
 
         self.before_marshmallow(args, kwargs)
 
-        schema = compute_schema(getattr(self, 'post_schema', self.schema),
-                                getattr(self, 'post_schema_kwargs', dict()),
-                                qs,
-                                qs.include)
+        schema = compute_schema(
+            getattr(self, "post_schema", self.schema),
+            getattr(self, "post_schema_kwargs", dict()),
+            qs,
+            qs.include,
+        )
 
         data = schema.load(json_data)
 
         self.before_post(args, kwargs, data=data)
 
         try:
             obj = self.create_object(data, kwargs)
         except Exception:
             # Subclass can override self.create_object, but doesn't have to do it
             # correctly. Let's protect from that.
             self._data_layer.rollback()
             raise
 
-        result = getattr(self, 'post_response_schema', self.schema)(many=False).dump(obj)
+        result = getattr(self, "post_response_schema", self.schema)(many=False).dump(
+            obj
+        )
 
-        if result['data'].get('links', {}).get('self'):
-            final_result = (result, 201, {'Location': result['data']['links']['self']})
+        if result["data"].get("links", {}).get("self"):
+            final_result = (result, 201, {"Location": result["data"]["links"]["self"]})
         else:
             final_result = (result, 201)
 
         result = self.after_post(final_result)
 
         return result
 
     def _get_parent_filter(self, url, kwargs):
         """
         Returns a dictionary of filters that should be applied to ensure only resources
         belonging to the parent resource are returned
         """
 
-        url_segments = url.split('/')
+        url_segments = url.split("/")
         parent_segment = url_segments[-3]
         parent_id = url_segments[-2]
 
         for key, value in self.schema._declared_fields.items():
             if isinstance(value, BaseRelationship):
                 if value.type_ == parent_segment:
                     return {value.id_field: parent_id}
@@ -246,23 +242,25 @@
     _RE_IS_LIST_VALUE = re.compile(r"^\[(.+)\]$")
 
     def _transform_simple_filter(self, k, v):
         key_match = self._RE_IS_SIMPLE_FILTER.match(k)
         value_match = self._RE_IS_LIST_VALUE.match(v)
 
         if key_match and value_match:
-            k = 'filter'
+            k = "filter"
 
             try:
-                values = [int(_) for _ in value_match.groups()[0].split(',')]
+                values = [int(_) for _ in value_match.groups()[0].split(",")]
 
             except ValueError:
-                values = value_match.groups()[0].split(',')
+                values = value_match.groups()[0].split(",")
 
-            v = flask.json.dumps([{'name': key_match.groups()[0], 'op': 'in', 'val': values}])
+            v = flask.json.dumps(
+                [{"name": key_match.groups()[0], "op": "in", "val": values}]
+            )
 
         return k, v
 
     def create_object(self, data, kwargs):
         return self._data_layer.create_object(data, kwargs)
 
 
@@ -276,71 +274,76 @@
 
         qs = QSManager(request.args, self.schema)
 
         obj = self.get_object(kwargs, qs)
 
         self.before_marshmallow(args, kwargs)
 
-        schema = compute_schema(self.schema,
-                                getattr(self, 'get_schema_kwargs', dict()),
-                                qs,
-                                qs.include)
+        schema = compute_schema(
+            self.schema, getattr(self, "get_schema_kwargs", dict()), qs, qs.include
+        )
 
         result = schema.dump(obj) if obj else None
 
         final_result = self.after_get(result)
 
         return final_result
 
     @check_method_requirements
     def patch(self, *args, **kwargs):
         """Update an object"""
         json_data = request.get_json() or {}
 
         qs = QSManager(request.args, self.schema)
-        schema_kwargs = getattr(self, 'patch_schema_kwargs', dict())
+        schema_kwargs = getattr(self, "patch_schema_kwargs", dict())
 
         self.before_marshmallow(args, kwargs)
 
-        schema = compute_schema(getattr(self, 'patch_schema', self.schema),
-                                schema_kwargs,
-                                qs,
-                                qs.include)
+        schema = compute_schema(
+            getattr(self, "patch_schema", self.schema), schema_kwargs, qs, qs.include
+        )
 
         data = schema.load(json_data)
 
-        if 'id' not in json_data['data']:
-            raise BadRequest('Missing id in "data" node',
-                             source={'pointer': '/data/id'})
-        if (str(json_data['data']['id']) != str(kwargs[getattr(self._data_layer, 'url_field', 'id')])):
-            raise BadRequest('Value of id does not match the resource identifier in url',
-                             source={'pointer': '/data/id'})
+        if "id" not in json_data["data"]:
+            raise BadRequest(
+                'Missing id in "data" node', source={"pointer": "/data/id"}
+            )
+        if str(json_data["data"]["id"]) != str(
+            kwargs[getattr(self._data_layer, "url_field", "id")]
+        ):
+            raise BadRequest(
+                "Value of id does not match the resource identifier in url",
+                source={"pointer": "/data/id"},
+            )
 
         self.before_patch(args, kwargs, data=data)
 
         try:
             obj = self.update_object(data, qs, kwargs)
         except Exception:
             self._data_layer.rollback()
             raise
 
-        result = getattr(self, 'patch_response_schema', self.schema)(many=False).dump(obj)
+        result = getattr(self, "patch_response_schema", self.schema)(many=False).dump(
+            obj
+        )
 
         final_result = self.after_patch(result)
 
         return final_result
 
     @check_method_requirements
     def delete(self, *args, **kwargs):
         """Delete an object"""
         self.before_delete(args, kwargs)
 
         self.delete_object(kwargs)
 
-        result = {'meta': {'message': 'Object successfully deleted'}}
+        result = {"meta": {"message": "Object successfully deleted"}}
 
         final_result = self.after_delete(result)
 
         return final_result
 
     def before_get(self, args, kwargs):
         """Hook to make custom work before get method"""
@@ -387,180 +390,259 @@
     """Base class of a resource relationship manager"""
 
     @check_method_requirements
     def get(self, *args, **kwargs):
         """Get a relationship details"""
         self.before_get(args, kwargs)
 
-        relationship_field, model_relationship_field, related_type_, related_id_field = self._get_relationship_data()
+        (
+            relationship_field,
+            model_relationship_field,
+            related_type_,
+            related_id_field,
+        ) = self._get_relationship_data()
 
-        obj, data = self._data_layer.get_relationship(model_relationship_field,
-                                                      related_type_,
-                                                      related_id_field,
-                                                      kwargs)
-
-        result = {'links': {'self': request.path,
-                            'related': self.schema._declared_fields[relationship_field].get_related_url(obj)},
-                  'data': data}
+        obj, data = self._data_layer.get_relationship(
+            model_relationship_field, related_type_, related_id_field, kwargs
+        )
+
+        result = {
+            "links": {
+                "self": request.path,
+                "related": self.schema._declared_fields[
+                    relationship_field
+                ].get_related_url(obj),
+            },
+            "data": data,
+        }
 
         qs = QSManager(request.args, self.schema)
         if qs.include:
             schema = compute_schema(self.schema, dict(), qs, qs.include)
 
             serialized_obj = schema.dump(obj)
-            result['included'] = serialized_obj.get('included', dict())
+            result["included"] = serialized_obj.get("included", dict())
 
         final_result = self.after_get(result)
 
         return final_result
 
     @check_method_requirements
     def post(self, *args, **kwargs):
         """Add / create relationship(s)"""
         json_data = request.get_json() or {}
 
-        relationship_field, model_relationship_field, related_type_, related_id_field = self._get_relationship_data()
-
-        if 'data' not in json_data:
-            raise BadRequest('You must provide data with a "data" route node', source={'pointer': '/data'})
-        if isinstance(json_data['data'], dict):
-            if 'type' not in json_data['data']:
-                raise BadRequest('Missing type in "data" node', source={'pointer': '/data/type'})
-            if 'id' not in json_data['data']:
-                raise BadRequest('Missing id in "data" node', source={'pointer': '/data/id'})
-            if json_data['data']['type'] != related_type_:
-                raise InvalidType('The type field does not match the resource type', source={'pointer': '/data/type'})
-        if isinstance(json_data['data'], list):
-            for obj in json_data['data']:
-                if 'type' not in obj:
-                    raise BadRequest('Missing type in "data" node', source={'pointer': '/data/type'})
-                if 'id' not in obj:
-                    raise BadRequest('Missing id in "data" node', source={'pointer': '/data/id'})
-                if obj['type'] != related_type_:
-                    raise InvalidType('The type provided does not match the resource type',
-                                      source={'pointer': '/data/type'})
+        (
+            relationship_field,
+            model_relationship_field,
+            related_type_,
+            related_id_field,
+        ) = self._get_relationship_data()
+
+        if "data" not in json_data:
+            raise BadRequest(
+                'You must provide data with a "data" route node',
+                source={"pointer": "/data"},
+            )
+        if isinstance(json_data["data"], dict):
+            if "type" not in json_data["data"]:
+                raise BadRequest(
+                    'Missing type in "data" node', source={"pointer": "/data/type"}
+                )
+            if "id" not in json_data["data"]:
+                raise BadRequest(
+                    'Missing id in "data" node', source={"pointer": "/data/id"}
+                )
+            if json_data["data"]["type"] != related_type_:
+                raise InvalidType(
+                    "The type field does not match the resource type",
+                    source={"pointer": "/data/type"},
+                )
+        if isinstance(json_data["data"], list):
+            for obj in json_data["data"]:
+                if "type" not in obj:
+                    raise BadRequest(
+                        'Missing type in "data" node', source={"pointer": "/data/type"}
+                    )
+                if "id" not in obj:
+                    raise BadRequest(
+                        'Missing id in "data" node', source={"pointer": "/data/id"}
+                    )
+                if obj["type"] != related_type_:
+                    raise InvalidType(
+                        "The type provided does not match the resource type",
+                        source={"pointer": "/data/type"},
+                    )
 
         self.before_post(args, kwargs, json_data=json_data)
 
-        obj_, updated = self._data_layer.create_relationship(json_data,
-                                                             model_relationship_field,
-                                                             related_id_field,
-                                                             kwargs)
+        obj_, updated = self._data_layer.create_relationship(
+            json_data, model_relationship_field, related_id_field, kwargs
+        )
 
         status_code = 200
-        result = {'meta': {'message': 'Relationship successfully created'}}
+        result = {"meta": {"message": "Relationship successfully created"}}
 
         if updated is False:
-            result = ''
+            result = ""
             status_code = 204
 
         final_result = self.after_post(result, status_code)
 
         return final_result
 
     @check_method_requirements
     def patch(self, *args, **kwargs):
         """Update a relationship"""
         json_data = request.get_json() or {}
 
-        relationship_field, model_relationship_field, related_type_, related_id_field = self._get_relationship_data()
-
-        if 'data' not in json_data:
-            raise BadRequest('You must provide data with a "data" route node', source={'pointer': '/data'})
-        if isinstance(json_data['data'], dict):
-            if 'type' not in json_data['data']:
-                raise BadRequest('Missing type in "data" node', source={'pointer': '/data/type'})
-            if 'id' not in json_data['data']:
-                raise BadRequest('Missing id in "data" node', source={'pointer': '/data/id'})
-            if json_data['data']['type'] != related_type_:
-                raise InvalidType('The type field does not match the resource type', source={'pointer': '/data/type'})
-        if isinstance(json_data['data'], list):
-            for obj in json_data['data']:
-                if 'type' not in obj:
-                    raise BadRequest('Missing type in "data" node', source={'pointer': '/data/type'})
-                if 'id' not in obj:
-                    raise BadRequest('Missing id in "data" node', source={'pointer': '/data/id'})
-                if obj['type'] != related_type_:
-                    raise InvalidType('The type provided does not match the resource type',
-                                      source={'pointer': '/data/type'})
+        (
+            relationship_field,
+            model_relationship_field,
+            related_type_,
+            related_id_field,
+        ) = self._get_relationship_data()
+
+        if "data" not in json_data:
+            raise BadRequest(
+                'You must provide data with a "data" route node',
+                source={"pointer": "/data"},
+            )
+        if isinstance(json_data["data"], dict):
+            if "type" not in json_data["data"]:
+                raise BadRequest(
+                    'Missing type in "data" node', source={"pointer": "/data/type"}
+                )
+            if "id" not in json_data["data"]:
+                raise BadRequest(
+                    'Missing id in "data" node', source={"pointer": "/data/id"}
+                )
+            if json_data["data"]["type"] != related_type_:
+                raise InvalidType(
+                    "The type field does not match the resource type",
+                    source={"pointer": "/data/type"},
+                )
+        if isinstance(json_data["data"], list):
+            for obj in json_data["data"]:
+                if "type" not in obj:
+                    raise BadRequest(
+                        'Missing type in "data" node', source={"pointer": "/data/type"}
+                    )
+                if "id" not in obj:
+                    raise BadRequest(
+                        'Missing id in "data" node', source={"pointer": "/data/id"}
+                    )
+                if obj["type"] != related_type_:
+                    raise InvalidType(
+                        "The type provided does not match the resource type",
+                        source={"pointer": "/data/type"},
+                    )
 
         self.before_patch(args, kwargs, json_data=json_data)
 
-        obj_, updated = self._data_layer.update_relationship(json_data,
-                                                             model_relationship_field,
-                                                             related_id_field,
-                                                             kwargs)
+        obj_, updated = self._data_layer.update_relationship(
+            json_data, model_relationship_field, related_id_field, kwargs
+        )
 
         status_code = 200
-        result = {'meta': {'message': 'Relationship successfully updated'}}
+        result = {"meta": {"message": "Relationship successfully updated"}}
 
         if updated is False:
-            result = ''
+            result = ""
             status_code = 204
 
         final_result = self.after_patch(result, status_code)
 
         return final_result
 
     @check_method_requirements
     def delete(self, *args, **kwargs):
         """Delete relationship(s)"""
         json_data = request.get_json() or {}
 
-        relationship_field, model_relationship_field, related_type_, related_id_field = self._get_relationship_data()
-
-        if 'data' not in json_data:
-            raise BadRequest('You must provide data with a "data" route node', source={'pointer': '/data'})
-        if isinstance(json_data['data'], dict):
-            if 'type' not in json_data['data']:
-                raise BadRequest('Missing type in "data" node', source={'pointer': '/data/type'})
-            if 'id' not in json_data['data']:
-                raise BadRequest('Missing id in "data" node', source={'pointer': '/data/id'})
-            if json_data['data']['type'] != related_type_:
-                raise InvalidType('The type field does not match the resource type', source={'pointer': '/data/type'})
-        if isinstance(json_data['data'], list):
-            for obj in json_data['data']:
-                if 'type' not in obj:
-                    raise BadRequest('Missing type in "data" node', source={'pointer': '/data/type'})
-                if 'id' not in obj:
-                    raise BadRequest('Missing id in "data" node', source={'pointer': '/data/id'})
-                if obj['type'] != related_type_:
-                    raise InvalidType('The type provided does not match the resource type',
-                                      source={'pointer': '/data/type'})
+        (
+            relationship_field,
+            model_relationship_field,
+            related_type_,
+            related_id_field,
+        ) = self._get_relationship_data()
+
+        if "data" not in json_data:
+            raise BadRequest(
+                'You must provide data with a "data" route node',
+                source={"pointer": "/data"},
+            )
+        if isinstance(json_data["data"], dict):
+            if "type" not in json_data["data"]:
+                raise BadRequest(
+                    'Missing type in "data" node', source={"pointer": "/data/type"}
+                )
+            if "id" not in json_data["data"]:
+                raise BadRequest(
+                    'Missing id in "data" node', source={"pointer": "/data/id"}
+                )
+            if json_data["data"]["type"] != related_type_:
+                raise InvalidType(
+                    "The type field does not match the resource type",
+                    source={"pointer": "/data/type"},
+                )
+        if isinstance(json_data["data"], list):
+            for obj in json_data["data"]:
+                if "type" not in obj:
+                    raise BadRequest(
+                        'Missing type in "data" node', source={"pointer": "/data/type"}
+                    )
+                if "id" not in obj:
+                    raise BadRequest(
+                        'Missing id in "data" node', source={"pointer": "/data/id"}
+                    )
+                if obj["type"] != related_type_:
+                    raise InvalidType(
+                        "The type provided does not match the resource type",
+                        source={"pointer": "/data/type"},
+                    )
 
         self.before_delete(args, kwargs, json_data=json_data)
 
-        obj_, updated = self._data_layer.delete_relationship(json_data,
-                                                             model_relationship_field,
-                                                             related_id_field,
-                                                             kwargs)
+        obj_, updated = self._data_layer.delete_relationship(
+            json_data, model_relationship_field, related_id_field, kwargs
+        )
 
         status_code = 200
-        result = {'meta': {'message': 'Relationship successfully updated'}}
+        result = {"meta": {"message": "Relationship successfully updated"}}
 
         if updated is False:
-            result = ''
+            result = ""
             status_code = 204
 
         final_result = self.after_delete(result, status_code)
 
         return final_result
 
     def _get_relationship_data(self):
         """Get useful data for relationship management"""
-        relationship_field = request.path.split('/')[-1].replace('-', '_')
+        relationship_field = request.path.split("/")[-1].replace("-", "_")
 
         if relationship_field not in get_relationships(self.schema):
-            raise RelationNotFound("{} has no attribute {}".format(self.schema.__name__, relationship_field))
+            raise RelationNotFound(
+                "{} has no attribute {}".format(
+                    self.schema.__name__, relationship_field
+                )
+            )
 
         related_type_ = self.schema._declared_fields[relationship_field].type_
         related_id_field = self.schema._declared_fields[relationship_field].id_field
         model_relationship_field = get_model_field(self.schema, relationship_field)
 
-        return relationship_field, model_relationship_field, related_type_, related_id_field
+        return (
+            relationship_field,
+            model_relationship_field,
+            related_type_,
+            related_id_field,
+        )
 
     def before_get(self, args, kwargs):
         """Hook to make custom work before get method"""
         pass
 
     def after_get(self, result):
         """Hook to make custom work after get method"""
@@ -585,9 +667,7 @@
     def before_delete(self, args, kwargs, json_data=None):
         """Hook to make custom work before delete method"""
         pass
 
     def after_delete(self, result, status_code):
         """Hook to make custom work after delete method"""
         return result, status_code
-
-# fmt: on
```

### Comparing `flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next/schema.py` & `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,14 @@
-# -*- coding: utf-8 -*-
-# isort: skip_file
-# fmt: off
-
 """Helpers to deal with marshmallow schemas"""
 
-import copy
-from typing import Optional, Tuple, Set
+from typing import Optional, Tuple
 
 from marshmallow import class_registry
 from marshmallow.base import SchemaABC
-from marshmallow_jsonapi.fields import Relationship, List, Nested
+from marshmallow_jsonapi.fields import List, Nested, Relationship
 
 from .exceptions import InvalidInclude
 
 
 def compute_schema(schema_cls, default_kwargs, qs, include):
     """Compute a schema around compound documents and sparse fieldsets
 
@@ -22,60 +17,70 @@
     :param QueryStringManager qs: qs
     :param list include: the relation field to include data from
 
     :return Schema schema: the schema computed
     """
     # manage include_data parameter of the schema
     schema_kwargs = default_kwargs
-    schema_kwargs['include_data'] = tuple()
+    schema_kwargs["include_data"] = tuple()
 
     # collect sub-related_includes
     related_includes = {}
 
     if include:
         for include_path in include:
-            field = include_path.split('.')[0]
+            field = include_path.split(".")[0]
 
             if field not in schema_cls._declared_fields:
-                raise InvalidInclude("{} has no attribute {}".format(schema_cls.__name__, field))
+                raise InvalidInclude(
+                    "{} has no attribute {}".format(schema_cls.__name__, field)
+                )
             elif not isinstance(schema_cls._declared_fields[field], Relationship):
-                raise InvalidInclude("{} is not a relationship attribute of {}".format(field, schema_cls.__name__))
+                raise InvalidInclude(
+                    "{} is not a relationship attribute of {}".format(
+                        field, schema_cls.__name__
+                    )
+                )
 
-            schema_kwargs['include_data'] += (field, )
+            schema_kwargs["include_data"] += (field,)
             if field not in related_includes:
                 related_includes[field] = []
-            if '.' in include_path:
-                related_includes[field] += ['.'.join(include_path.split('.')[1:])]
+            if "." in include_path:
+                related_includes[field] += [".".join(include_path.split(".")[1:])]
 
     only = _compute_sparse(schema_cls, default_kwargs, qs, include)
     if only is not None:
         schema_kwargs["only"] = only
 
     # create base schema instance
     schema = schema_cls(**schema_kwargs)
 
     # manage compound documents
     if include:
         for include_path in include:
-            field = include_path.split('.')[0]
+            field = include_path.split(".")[0]
             relation_field = schema.declared_fields[field]
-            related_schema_cls = schema.declared_fields[field].__dict__['_Relationship__schema']
+            related_schema_cls = schema.declared_fields[field].__dict__[
+                "_Relationship__schema"
+            ]
             related_schema_kwargs = {}
-            if 'context' in default_kwargs:
-                related_schema_kwargs['context'] = default_kwargs['context']
+            if "context" in default_kwargs:
+                related_schema_kwargs["context"] = default_kwargs["context"]
             if isinstance(related_schema_cls, SchemaABC):
-                related_schema_kwargs['many'] = related_schema_cls.many
+                related_schema_kwargs["many"] = related_schema_cls.many
                 related_schema_cls = related_schema_cls.__class__
             if isinstance(related_schema_cls, str):
                 related_schema_cls = class_registry.get_class(related_schema_cls)
-            related_schema = compute_schema(related_schema_cls,
-                                            related_schema_kwargs,
-                                            qs,
-                                            related_includes[field] or None)
-            relation_field.__dict__['_Relationship__schema'] = related_schema
+            related_schema = compute_schema(
+                related_schema_cls,
+                related_schema_kwargs,
+                qs,
+                related_includes[field] or None,
+            )
+            relation_field.__dict__["_Relationship__schema"] = related_schema
 
     return schema
 
 
 def get_model_field(schema, field):
     """Get the model field of a schema field
 
@@ -86,56 +91,62 @@
     if schema._declared_fields.get(field) is None:
         raise Exception("{} has no attribute {}".format(schema.__name__, field))
 
     if schema._declared_fields[field].attribute is not None:
         return schema._declared_fields[field].attribute
     return field
 
+
 def get_nested_fields(schema, model_field=False):
     """Return nested fields of a schema to support a join
 
     :param Schema schema: a marshmallow schema
     :param boolean model_field: whether to extract the model field for the nested fields
     :return list: list of nested fields of the schema
     """
 
     nested_fields = []
-    for (key, value) in schema._declared_fields.items():
+    for key, value in schema._declared_fields.items():
         if isinstance(value, List):
             nested_fields.append(key)
         elif isinstance(value, Nested):
             nested_fields.append(key)
 
     if model_field is True:
         nested_fields = [get_model_field(schema, key) for key in nested_fields]
 
     return nested_fields
 
+
 def get_relationships(schema, model_field=False):
     """Return relationship fields of a schema
 
     :param Schema schema: a marshmallow schema
     :param list: list of relationship fields of a schema
     """
-    relationships = [key for (key, value) in schema._declared_fields.items() if isinstance(value, Relationship)]
+    relationships = [
+        key
+        for (key, value) in schema._declared_fields.items()
+        if isinstance(value, Relationship)
+    ]
 
     if model_field is True:
         relationships = [get_model_field(schema, key) for key in relationships]
 
     return relationships
 
 
 def get_related_schema(schema, field):
     """Retrieve the related schema of a relationship field
 
     :param Schema schema: the schema to retrieve le relationship field from
     :param field: the relationship field
     :return Schema: the related schema
     """
-    return schema._declared_fields[field].__dict__['_Relationship__schema']
+    return schema._declared_fields[field].__dict__["_Relationship__schema"]
 
 
 def get_schema_from_type(resource_type):
     """Retrieve a schema from the registry by his type
 
     :param str type_: the type of the resource
     :return Schema: the schema class
@@ -153,36 +164,37 @@
 def get_schema_field(schema, field):
     """Get the schema field of a model field
 
     :param Schema schema: a marshmallow schema
     :param str field: the name of the model field
     :return str: the name of the field in the schema
     """
-    schema_fields_to_model = {key: get_model_field(schema, key) for (key, value) in schema._declared_fields.items()}
+    schema_fields_to_model = {
+        key: get_model_field(schema, key)
+        for (key, value) in schema._declared_fields.items()
+    }
     for key, value in schema_fields_to_model.items():
         if value == field:
             return key
 
     raise ValueError("Couldn't find schema field from {}".format(field))
 
-# fmt: on
-
 
 def _compute_sparse(
     schema_cls, default_kwargs, qs, include
 ) -> Optional[Tuple[str, ...]]:
     """
     Compute "only" keyword argument for marshmallow.Schema.
 
     We need this because following has no effect:
 
         schema = FooSchema()
         schema.only = ("field1", "field2", ...)
 
-    marsmallow.Schema.only should really, really, really be private attribute or
+    marshmallow.Schema.only should really, really, really be private attribute or
     read-only property: setting it's value after instance had been __init__-ialized
     has no effect.
     """
     # manage include_data parameter of the schema
     schema_kwargs = {k: v for k, v in (default_kwargs or dict()).items()}
 
     only = schema_kwargs.get("only")
```

### Comparing `flask-rest-jsonapi-next-0.34.7/flask_rest_jsonapi_next.egg-info/PKG-INFO` & `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rest-jsonapi-next
-Version: 0.34.7
+Version: 0.40.0
 Summary: Flask extension to create REST web api according to JSONAPI 1.0 specification with Flask, Marshmallow and data provider of your choice (SQLAlchemy, MongoDB, ...)
 Author: original miLibris/flask-rest-jsonapi contributors
 Maintainer-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-rest-jsonapi-next
 Project-URL: Documentation, https://flask-rest-jsonapi-next.readthedocs.io/en/latest/
 Keywords: web,api,rest,jsonapi,flask,sqlalchemy,marshmallow
@@ -45,16 +45,14 @@
 ```sh
 pip install flask-rest-jsonapi-next
 ```
 
 ## A minimal API
 
 ```py
-# -*- coding: utf-8 -*-
-
 from flask import Flask
 from flask_rest_jsonapi_next import Api, ResourceDetail, ResourceList
 from flask_sqlalchemy import SQLAlchemy
 from marshmallow_jsonapi.flask import Schema
 from marshmallow_jsonapi import fields
 
 # Create the Flask application and the Flask-SQLAlchemy object.
```

### Comparing `flask-rest-jsonapi-next-0.34.7/pyproject.toml` & `flask-rest-jsonapi-next-0.40.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 [build-system]
 # setuptools v64 was first to support `pip install -e` for packages defined using
 # pyproject.toml (older versions support this, but only for setup.py projects)
 requires = ["setuptools>=64", "wheel"]
-build-backend = "setuptools.build_meta"
 
 [project]
 name = "flask-rest-jsonapi-next"
-version = "0.34.7"
+version = "0.40.0"
 description = "Flask extension to create REST web api according to JSONAPI 1.0 specification with Flask, Marshmallow and data provider of your choice (SQLAlchemy, MongoDB, ...)"
 readme = "README.md"
 classifiers = [
 	"Framework :: Flask",
 	"Programming Language :: Python :: 3",
 	"Programming Language :: Python :: 3.7",
 	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3 :: Only",
 	"License :: OSI Approved :: MIT License",
 ]
 dependencies = [
-	"six",
 	"Flask >= 2.2.0",
 	"marshmallow >= 3",
-	"marshmallow_jsonapi",
-	"sqlalchemy < 2.0.0",
+	"marshmallow-jsonapi",
+	"sqlalchemy",
 	"requests",
+	"packaging",
 ]
 keywords = [
 	"web",
 	"api",
 	"rest",
 	"jsonapi",
 	"flask",
@@ -47,43 +46,52 @@
 Source = "https://github.com/tadams42/flask-rest-jsonapi-next"
 Documentation = "https://flask-rest-jsonapi-next.readthedocs.io/en/latest/"
 
 [project.optional-dependencies]
 dev = [
 	"black",
 	"bump2version",
-	"check-manifest",
-	"furo",
 	"ipython",
 	"isort",
-	"myst-parser",
-	"pytest",
-	"sphinx-copybutton",
-	"sphinx",
-	"psycopg2-binary",
+	"psycopg[binary]",
+	"rich",
+	"pre-commit",
 ]
 docs = ["furo", "myst-parser", "sphinx", "sphinx-copybutton"]
 tests = ["check-manifest", "pytest", "coverage"]
 
 
 [tool.setuptools]
 zip-safe = false
 platforms = ["any"]
 include-package-data = true
 
+
 [tool.setuptools.packages.find]
+where = ["src"]
 exclude = ["tests"]
 
+
 [tool.isort]
 profile = "black"
 skip_gitignore = true
 
-[tool.coverage.paths]
-source = ["flask_rest_jsonapi_next"]
 
 [tool.coverage.run]
 branch = true
-source = ["flask_rest_jsonapi_next"]
+source = ["src"]
+
 
 [tool.coverage.report]
 show_missing = true
 precision = 2
+
+[tool.pytest.ini_options]
+minversion = "7.0"
+testpaths = ["tests"]
+
+python_classes = ["Describe*", "When*", "describe_*", "when_*"]
+python_functions = ["it_*", "test_*", "then_*", "when_*"]
+python_files = ["test_*", "*_spec.py", "*_test.py"]
+
+[tool.pytest-watcher]
+delay = 0.5
```

