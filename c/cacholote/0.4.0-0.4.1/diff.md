# Comparing `tmp/cacholote-0.4.0.tar.gz` & `tmp/cacholote-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cacholote-0.4.0.tar", last modified: Fri Jul 21 08:03:57 2023, max compression
+gzip compressed data, was "cacholote-0.4.1.tar", last modified: Fri Jul 21 16:16:14 2023, max compression
```

## Comparing `cacholote-0.4.0.tar` & `cacholote-0.4.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.540683 cacholote-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-21 08:03:37.000000 cacholote-0.4.0/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.532683 cacholote-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.536683 cacholote-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-21 08:03:37.000000 cacholote-0.4.0/.github/workflows/on-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-07-21 08:03:37.000000 cacholote-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-21 08:03:37.000000 cacholote-0.4.0/.pre-commit-config-cruft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-21 08:03:37.000000 cacholote-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-21 08:03:37.000000 cacholote-0.4.0/DESIGN.rst
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-21 08:03:37.000000 cacholote-0.4.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-07-21 08:03:37.000000 cacholote-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 08:03:37.000000 cacholote-0.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-21 08:03:37.000000 cacholote-0.4.0/OBJECT-STORAGE-DESIGN.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-07-21 08:03:57.540683 cacholote-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-21 08:03:37.000000 cacholote-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.536683 cacholote-0.4.0/cacholote/
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/extra_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-21 08:03:37.000000 cacholote-0.4.0/cacholote/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-21 08:03:57.000000 cacholote-0.4.0/cacholote/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.536683 cacholote-0.4.0/cacholote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-07-21 08:03:57.000000 cacholote-0.4.0/cacholote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-21 08:03:57.000000 cacholote-0.4.0/cacholote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:03:57.000000 cacholote-0.4.0/cacholote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-21 08:03:57.000000 cacholote-0.4.0/cacholote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 08:03:57.000000 cacholote-0.4.0/cacholote.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.536683 cacholote-0.4.0/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-21 08:03:37.000000 cacholote-0.4.0/ci/environment-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-21 08:03:37.000000 cacholote-0.4.0/ci/environment-integration.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.540683 cacholote-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-21 08:03:37.000000 cacholote-0.4.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.540683 cacholote-0.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:37.000000 cacholote-0.4.0/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.540683 cacholote-0.4.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:37.000000 cacholote-0.4.0/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-21 08:03:37.000000 cacholote-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-21 08:03:37.000000 cacholote-0.4.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-21 08:03:37.000000 cacholote-0.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-21 08:03:37.000000 cacholote-0.4.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-21 08:03:37.000000 cacholote-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 08:03:57.540683 cacholote-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:57.540683 cacholote-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/test_00_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/test_01_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/test_02_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/test_10_decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/test_20_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/test_30_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/test_40_xarray_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/test_50_io_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-07-21 08:03:37.000000 cacholote-0.4.0/tests/test_60_clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:16:14.747928 cacholote-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-21 16:15:52.000000 cacholote-0.4.1/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:16:14.743929 cacholote-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:16:14.743929 cacholote-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-21 16:15:52.000000 cacholote-0.4.1/.github/workflows/on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-07-21 16:15:52.000000 cacholote-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-21 16:15:52.000000 cacholote-0.4.1/.pre-commit-config-cruft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-21 16:15:52.000000 cacholote-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-21 16:15:52.000000 cacholote-0.4.1/DESIGN.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-21 16:15:52.000000 cacholote-0.4.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-07-21 16:15:52.000000 cacholote-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 16:15:52.000000 cacholote-0.4.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-21 16:15:52.000000 cacholote-0.4.1/OBJECT-STORAGE-DESIGN.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-07-21 16:16:14.747928 cacholote-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-21 16:15:52.000000 cacholote-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:16:14.743929 cacholote-0.4.1/cacholote/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-21 16:15:52.000000 cacholote-0.4.1/cacholote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-21 16:15:52.000000 cacholote-0.4.1/cacholote/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10600 2023-07-21 16:15:52.000000 cacholote-0.4.1/cacholote/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-07-21 16:15:52.000000 cacholote-0.4.1/cacholote/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-21 16:15:52.000000 cacholote-0.4.1/cacholote/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-21 16:15:52.000000 cacholote-0.4.1/cacholote/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-21 16:15:52.000000 cacholote-0.4.1/cacholote/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12952 2023-07-21 16:15:52.000000 cacholote-0.4.1/cacholote/extra_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:15:52.000000 cacholote-0.4.1/cacholote/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-21 16:15:52.000000 cacholote-0.4.1/cacholote/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-21 16:16:14.000000 cacholote-0.4.1/cacholote/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:16:14.743929 cacholote-0.4.1/cacholote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-07-21 16:16:14.000000 cacholote-0.4.1/cacholote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-21 16:16:14.000000 cacholote-0.4.1/cacholote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:16:14.000000 cacholote-0.4.1/cacholote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-21 16:16:14.000000 cacholote-0.4.1/cacholote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 16:16:14.000000 cacholote-0.4.1/cacholote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:16:14.743929 cacholote-0.4.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-21 16:15:52.000000 cacholote-0.4.1/ci/environment-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-21 16:15:52.000000 cacholote-0.4.1/ci/environment-integration.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:16:14.747928 cacholote-0.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-21 16:15:52.000000 cacholote-0.4.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:16:14.747928 cacholote-0.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:15:52.000000 cacholote-0.4.1/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:16:14.747928 cacholote-0.4.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:15:52.000000 cacholote-0.4.1/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-21 16:15:52.000000 cacholote-0.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-21 16:15:52.000000 cacholote-0.4.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-21 16:15:52.000000 cacholote-0.4.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-21 16:15:52.000000 cacholote-0.4.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-21 16:15:52.000000 cacholote-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 16:16:14.747928 cacholote-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:16:14.747928 cacholote-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-21 16:15:52.000000 cacholote-0.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-21 16:15:52.000000 cacholote-0.4.1/tests/test_00_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-21 16:15:52.000000 cacholote-0.4.1/tests/test_01_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-21 16:15:52.000000 cacholote-0.4.1/tests/test_02_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-21 16:15:52.000000 cacholote-0.4.1/tests/test_10_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-21 16:15:52.000000 cacholote-0.4.1/tests/test_20_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-21 16:15:52.000000 cacholote-0.4.1/tests/test_30_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-07-21 16:15:52.000000 cacholote-0.4.1/tests/test_40_xarray_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-21 16:15:52.000000 cacholote-0.4.1/tests/test_50_io_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-07-21 16:15:52.000000 cacholote-0.4.1/tests/test_60_clean.py
```

### Comparing `cacholote-0.4.0/.cruft.json` & `cacholote-0.4.1/.cruft.json`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/.github/workflows/on-push.yml` & `cacholote-0.4.1/.github/workflows/on-push.yml`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/.gitignore` & `cacholote-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/.pre-commit-config.yaml` & `cacholote-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/DESIGN.rst` & `cacholote-0.4.1/DESIGN.rst`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/LICENSE` & `cacholote-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/Makefile` & `cacholote-0.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/OBJECT-STORAGE-DESIGN.rst` & `cacholote-0.4.1/OBJECT-STORAGE-DESIGN.rst`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/PKG-INFO` & `cacholote-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacholote
-Version: 0.4.0
+Version: 0.4.1
 Summary: Efficiently cache calls to functions
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cacholote-0.4.0/README.md` & `cacholote-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/cacholote/__init__.py` & `cacholote-0.4.1/cacholote/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 extra_encoders.register_all()
 
 __all__ = [
     "__version__",
     "cacheable",
     "clean_cache_files",
+    "clean_invalid_cache_entries",
     "config",
     "database",
     "delete",
     "dumps",
     "extra_encoders",
     "loads",
     "utils",
```

### Comparing `cacholote-0.4.0/cacholote/cache.py` & `cacholote-0.4.1/cacholote/cache.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/cacholote/clean.py` & `cacholote-0.4.1/cacholote/clean.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import json
 import posixpath
 from typing import Any, Callable, Dict, List, Literal, Optional, Sequence, Set, Union
 
 import sqlalchemy as sa
 import sqlalchemy.orm
 
-from . import config, database, encode, extra_encoders, utils
+from . import config, database, decode, encode, extra_encoders, utils
 
 
 def _delete_cache_file(
     obj: Dict[str, Any],
     session: Optional[sa.orm.Session] = None,
     cache_entry: Optional[database.CacheEntry] = None,
     sizes: Optional[Dict[str, int]] = None,
@@ -271,7 +271,16 @@
 
     cleaner.delete_cache_files(
         maxsize=maxsize,
         method=method,
         tags_to_clean=tags_to_clean,
         tags_to_keep=tags_to_keep,
     )
+
+
+def clean_invalid_cache_entries() -> None:
+    with config.get().sessionmaker() as session:
+        for cache_entry in session.scalars(sa.select(database.CacheEntry)):
+            try:
+                decode.loads(cache_entry._result_as_string)
+            except decode.DecodeError:
+                _delete_cache_entry(session, cache_entry)
```

### Comparing `cacholote-0.4.0/cacholote/config.py` & `cacholote-0.4.1/cacholote/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 import pydantic
 import sqlalchemy as sa
 import sqlalchemy.orm
 import structlog
 
 from . import database
 
-_LOGGER = structlog.get_logger(
-    wrapper_class=structlog.make_filtering_bound_logger(logging.WARNING)
-)
 _SETTINGS: Optional[Settings] = None
 _DEFAULT_CACHE_DIR = pathlib.Path(tempfile.gettempdir()) / "cacholote"
 _DEFAULT_CACHE_DIR.mkdir(exist_ok=True)
+_DEFAULT_LOGGER = structlog.get_logger(
+    wrapper_class=structlog.make_filtering_bound_logger(logging.WARNING)
+)
 
 _CONFIG_NOT_SET_MSG = (
     "Configuration settings have not been set. Run `cacholote.config.reset()`."
 )
 
 
 class Settings(pydantic.BaseSettings):
@@ -55,15 +55,15 @@
     io_delete_original: bool = False
     raise_all_encoding_errors: bool = False
     expiration: Optional[datetime.datetime] = None
     tag: Optional[str] = None
     return_cache_entry: bool = False
     logger: Union[
         structlog.BoundLogger, structlog._config.BoundLoggerLazyProxy
-    ] = _LOGGER
+    ] = _DEFAULT_LOGGER
 
     @pydantic.validator("create_engine_kwargs", allow_reuse=True)
     def validate_create_engine_kwargs(
         cls: pydantic.BaseSettings, create_engine_kwargs: Dict[str, Any]
     ) -> Dict[str, Any]:
         poolclass = create_engine_kwargs.get("poolclass")
         if isinstance(poolclass, str):
```

### Comparing `cacholote-0.4.0/cacholote/database.py` & `cacholote-0.4.1/cacholote/database.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/cacholote/decode.py` & `cacholote-0.4.1/cacholote/decode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/cacholote/encode.py` & `cacholote-0.4.1/cacholote/encode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/cacholote/extra_encoders.py` & `cacholote-0.4.1/cacholote/extra_encoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,18 @@
             expected = file_json["file:checksum"]
             actual = (
                 fs.checksum(urlpath)  # Just for backward compatibility.
                 if isinstance(expected, int)
                 else f"{fs.checksum(urlpath):x}"
             )
             if expected != actual:
-                raise ValueError(f"checksum mismatch: {expected=} {actual=}")
+                raise ValueError(f"checksum mismatch: {urlpath=} {expected=} {actual=}")
+            config.get().logger.info(
+                "retrieve cache file", urlpath=fs.unstrip_protocol(urlpath)
+            )
             return (fs, urlpath)
 
     # Attempt to read from href
     urlpath = file_json["href"]
     fs, *_ = fsspec.get_fs_token_paths(urlpath)
     if fs.exists(urlpath):
         return (fs, urlpath)
@@ -220,15 +223,15 @@
                 with _logging_timer("upload", urlpath=fs.unstrip_protocol(urlpath)):
                     obj.to_zarr(mapper, consolidated=True)
     elif not fs.exists(urlpath):
         # Need a tmp local copy to write on a different filesystem
         with tempfile.TemporaryDirectory() as tmpdirname:
             tmpfilename = str(pathlib.Path(tmpdirname) / pathlib.Path(urlpath).name)
 
-            with _logging_timer("download", urlpath=tmpfilename):
+            with _logging_timer("write tmp file", urlpath=tmpfilename):
                 if filetype == "application/netcdf":
                     obj.to_netcdf(tmpfilename)
                 elif filetype == "application/x-grib":
                     import cfgrib.xarray_to_grib
 
                     cfgrib.xarray_to_grib.to_grib(obj, tmpfilename)
                 else:
```

### Comparing `cacholote-0.4.0/cacholote/utils.py` & `cacholote-0.4.1/cacholote/utils.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/cacholote.egg-info/PKG-INFO` & `cacholote-0.4.1/cacholote.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacholote
-Version: 0.4.0
+Version: 0.4.1
 Summary: Efficiently cache calls to functions
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cacholote-0.4.0/cacholote.egg-info/SOURCES.txt` & `cacholote-0.4.1/cacholote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/docs/Makefile` & `cacholote-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/docs/conf.py` & `cacholote-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/docs/make.bat` & `cacholote-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/pyproject.toml` & `cacholote-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/tests/conftest.py` & `cacholote-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/tests/test_01_settings.py` & `cacholote-0.4.1/tests/test_01_settings.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/tests/test_02_utils.py` & `cacholote-0.4.1/tests/test_02_utils.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/tests/test_10_decode.py` & `cacholote-0.4.1/tests/test_10_decode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/tests/test_20_encode.py` & `cacholote-0.4.1/tests/test_20_encode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/tests/test_30_cache.py` & `cacholote-0.4.1/tests/test_30_cache.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.4.0/tests/test_40_xarray_encoder.py` & `cacholote-0.4.1/tests/test_40_xarray_encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,25 +161,29 @@
 
     # Cache dataset
     cfunc = cache.cacheable(get_grib_ds)
     cached_ds = cfunc()
     captured = iter(capsys.readouterr().out.splitlines())
 
     line = next(captured)
-    assert "start download" in line
+    assert "start write tmp file" in line
     assert "urlpath=" in line
 
     line = next(captured)
-    assert "end download" in line
+    assert "end write tmp file" in line
     assert "urlpath=" in line
-    assert "download_time=" in line
+    assert "write_tmp_file_time=" in line
 
     line = next(captured)
     assert "start upload" in line
     assert f"urlpath=file://{cached_ds.encoding['source']}" in line
     assert "size=22597" in line
 
     line = next(captured)
     assert "end upload" in line
     assert f"urlpath=file://{cached_ds.encoding['source']}" in line
     assert "upload_time=" in line
     assert "size=22597" in line
+
+    line = next(captured)
+    assert "retrieve cache file" in line
+    assert f"urlpath=file://{cached_ds.encoding['source']}" in line
```

### Comparing `cacholote-0.4.0/tests/test_50_io_encoder.py` & `cacholote-0.4.1/tests/test_50_io_encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -208,7 +208,11 @@
     assert "size=0" in line
 
     line = next(captured)
     assert "end remove" in line
     assert f"urlpath=file://{tmpfile}" in line
     assert "remove_time=" in line
     assert "size=0" in line
+
+    line = next(captured)
+    assert "retrieve cache file" in line
+    assert f"urlpath=s3://{cached_file.path}" in line
```

### Comparing `cacholote-0.4.0/tests/test_60_clean.py` & `cacholote-0.4.1/tests/test_60_clean.py`

 * *Files 3% similar despite different names*

```diff
@@ -193,14 +193,35 @@
     assert fs.ls(dirname) == []
 
     # Cache again
     assert open_url(tmpfile).read() == b"new"
     assert len(fs.ls(dirname)) == 1
 
 
+def test_clean_invalid_cache_entries(tmpdir: pathlib.Path) -> None:
+    fs, dirname = utils.get_cache_files_fs_dirname()
+    con = config.get().engine.raw_connection()
+    cur = con.cursor()
+
+    # Create and cache 2 files
+    for i in range(2):
+        filepath = tmpdir / f"{i}.txt"
+        fsspec.filesystem("file").touch(filepath)
+        open_url(filepath)
+
+    # Invalidate one file
+    valid, invalid = fs.ls(dirname)
+    fs.touch(invalid)
+
+    clean.clean_invalid_cache_entries()
+    cur.execute("SELECT * FROM cache_entries", ())
+    assert len(cur.fetchall()) == 1
+    assert fs.ls(dirname) == [valid]
+
+
 def test_cleaner_logging(
     capsys: pytest.CaptureFixture[str], tmpdir: pathlib.Path
 ) -> None:
     # Cache file and create unknown
     tmpfile = tmpdir / "test.txt"
     fsspec.filesystem("file").pipe_file(tmpfile, b"1")
     cached_file = open_url(tmpfile)
```

