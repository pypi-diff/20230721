# Comparing `tmp/smile_id_core-2.0.1.tar.gz` & `tmp/smile_id_core-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smile_id_core-2.0.1.tar", max compression
+gzip compressed data, was "smile_id_core-2.1.0.tar", max compression
```

## Comparing `smile_id_core-2.0.1.tar` & `smile_id_core-2.1.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0     1071 2023-02-22 20:32:22.654704 smile_id_core-2.0.1/LICENSE.txt
--rw-r--r--   0        0        0    21382 2023-02-22 20:32:22.654704 smile_id_core-2.0.1/README.md
--rw-r--r--   0        0        0     1880 2023-02-22 20:32:22.654704 smile_id_core-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2726 2023-02-22 20:32:22.654704 smile_id_core-2.0.1/smile_id_core/IdApi.py
--rw-r--r--   0        0        0      127 2023-02-22 20:32:22.654704 smile_id_core-2.0.1/smile_id_core/ServerError.py
--rw-r--r--   0        0        0     1093 2023-02-22 20:32:22.654704 smile_id_core-2.0.1/smile_id_core/Signature.py
--rw-r--r--   0        0        0     8962 2023-02-22 20:32:22.654704 smile_id_core-2.0.1/smile_id_core/Utilities.py
--rw-r--r--   0        0        0     8852 2023-02-22 20:32:22.654704 smile_id_core-2.0.1/smile_id_core/WebApi.py
--rw-r--r--   0        0        0      333 2023-02-22 20:32:22.654704 smile_id_core-2.0.1/smile_id_core/__init__.py
--rw-r--r--   0        0        0     4260 2023-02-22 20:32:22.654704 smile_id_core-2.0.1/smile_id_core/image_upload.py
--rw-r--r--   0        0        0    22259 1970-01-01 00:00:00.000000 smile_id_core-2.0.1/setup.py
--rw-r--r--   0        0        0    22054 1970-01-01 00:00:00.000000 smile_id_core-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3967 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/README.md
+-rw-r--r--   0        0        0     2136 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3137 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/BusinessVerification.py
+-rw-r--r--   0        0        0     3657 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/IdApi.py
+-rw-r--r--   0        0        0      223 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/ServerError.py
+-rw-r--r--   0        0        0     2369 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/Signature.py
+-rw-r--r--   0        0        0    14727 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/Utilities.py
+-rw-r--r--   0        0        0    12058 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/WebApi.py
+-rw-r--r--   0        0        0      662 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/__init__.py
+-rw-r--r--   0        0        0     1019 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/base.py
+-rw-r--r--   0        0        0     2125 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/constants.py
+-rw-r--r--   0        0        0     8523 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/image_upload.py
+-rw-r--r--   0        0        0      811 2023-07-21 11:16:48.445598 smile_id_core-2.1.0/smile_id_core/types.py
+-rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 smile_id_core-2.1.0/PKG-INFO
```

### Comparing `smile_id_core-2.0.1/LICENSE.txt` & `smile_id_core-2.1.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Smile Identity
+Copyright (c) 2023 Smile Identity
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `smile_id_core-2.0.1/pyproject.toml` & `smile_id_core-2.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [tool.poetry]
 name = "smile-id-core"
-version = "2.0.1"
+version = "2.1.0"
 description = "The official Smile Identity package exposes four classes namely; the WebApi class, the IDApi class, the Signature class and the Utilities class."
 license = "MIT"
 authors = ["Smile Identity <support@smileidentity.com>"]
 readme = "README.md"
 homepage = "https://github.com/smileidentity/smile-identity-core-python-3"
 classifiers = [
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
@@ -22,53 +21,66 @@
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 pycryptodome = "^3.15.0"
-python = "^3.6.2"
+python = "^3.7"
 requests = "^2.27.1"
+typing-extensions = "4.7.1"
+types-requests = "^2.28.11.5"
 
 [tool.poetry.group.dev]
 optional = true
-
 [tool.poetry.group.dev.dependencies]
-black = "^22.8.0"
+black = ">=22.8,<24.0"
+coverage = "7.2.7"
 isort = "^5.10.1"
+mock = ">=4.0.3,<6.0.0"
+mypy = "1.4.1"
+pylint = "2.13.9"
 pytest = "^7.0.1"
 pytest-cov = "^4.0.0"
+pydocstyle = "^6.3.0"
 pytest-xdist = "^3.0.2"
-responses = "^0.17.0"
+responses = ">=0.17,<0.24"
+types-mock = ">=4.0.15.2,<6.0.0.0"
 
 [tool.poetry.group.github-actions]
 optional = true
-
 [tool.poetry.group.github-actions.dependencies]
-pytest-github-actions-annotate-failures = "^0.1.7"
+pytest-github-actions-annotate-failures = ">=0.1.7,<0.3.0"
 
-[tool.poetry.group.typing]
-optional = true
-
-[tool.poetry.group.typing.dependencies]
-mypy = "^0.971"
-types-requests = "^2.28.11.4"
+[tool.black]
+line-length = 80
+target-version = ['py39']
+
+[tool.coverage.run]
+omit = [
+  "tests/*",
+]
 
 [tool.isort]
 profile = "black"
+line_length = 80
 
 [tool.mypy]
+allow_untyped_decorators = true
+disallow_untyped_defs = false
 files = "smile_id_core,tests"
+no_implicit_reexport = false
 pretty = true
 show_error_codes = true
+strict = true
 strict_equality = true
 warn_no_return = true
 warn_redundant_casts = true
-warn_unreachable = true
-warn_unused_configs = true
-warn_unused_ignores = true
+warn_unreachable = false
+warn_unused_configs = false
+warn_unused_ignores = false
 
 [tool.pytest.ini_options]
 addopts = "-n auto"
 testpaths = [
     "tests"
 ]
```

