# Comparing `tmp/letsbuilda-pypi-5.0.0b2.tar.gz` & `tmp/letsbuilda-pypi-5.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letsbuilda-pypi-5.0.0b2.tar", last modified: Fri Jul 14 23:49:04 2023, max compression
+gzip compressed data, was "letsbuilda-pypi-5.0.0b3.tar", last modified: Fri Jul 21 20:30:24 2023, max compression
```

## Comparing `letsbuilda-pypi-5.0.0b2.tar` & `letsbuilda-pypi-5.0.0b3.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-14 23:49:04.437579 letsbuilda-pypi-5.0.0b2/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1074 2023-07-12 21:27:21.000000 letsbuilda-pypi-5.0.0b2/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1145 2023-07-14 23:49:04.437579 letsbuilda-pypi-5.0.0b2/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      644 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b2/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1264 2023-07-14 23:46:47.000000 letsbuilda-pypi-5.0.0b2/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-07-14 23:49:04.437579 letsbuilda-pypi-5.0.0b2/setup.cfg
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-14 23:49:04.417579 letsbuilda-pypi-5.0.0b2/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-14 23:49:04.417579 letsbuilda-pypi-5.0.0b2/src/letsbuilda/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-14 23:49:04.437579 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      232 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2444 2023-07-14 23:45:41.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/async_client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      511 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/exceptions.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      880 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/files.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-14 23:49:04.437579 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/models/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      212 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/models/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3572 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/models/models_json.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1383 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/models/models_package.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1200 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/models/models_rss.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2121 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/sync_client.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-14 23:49:04.437579 letsbuilda-pypi-5.0.0b2/src/letsbuilda_pypi.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1145 2023-07-14 23:49:04.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda_pypi.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-07-14 23:49:04.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda_pypi.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-14 23:49:04.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda_pypi.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      146 2023-07-14 23:49:04.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda_pypi.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       11 2023-07-14 23:49:04.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda_pypi.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-14 23:49:04.437579 letsbuilda-pypi-5.0.0b2/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1250 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b2/tests/test_rss_feed_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:30:24.985936 letsbuilda-pypi-5.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-21 20:30:13.000000 letsbuilda-pypi-5.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-21 20:30:24.985936 letsbuilda-pypi-5.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-21 20:30:13.000000 letsbuilda-pypi-5.0.0b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-21 20:30:13.000000 letsbuilda-pypi-5.0.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 20:30:24.985936 letsbuilda-pypi-5.0.0b3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:30:24.981935 letsbuilda-pypi-5.0.0b3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:30:24.981935 letsbuilda-pypi-5.0.0b3/src/letsbuilda/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:30:24.981935 letsbuilda-pypi-5.0.0b3/src/letsbuilda/pypi/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-21 20:30:13.000000 letsbuilda-pypi-5.0.0b3/src/letsbuilda/pypi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-21 20:30:13.000000 letsbuilda-pypi-5.0.0b3/src/letsbuilda/pypi/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-21 20:30:13.000000 letsbuilda-pypi-5.0.0b3/src/letsbuilda/pypi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:30:24.981935 letsbuilda-pypi-5.0.0b3/src/letsbuilda/pypi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-21 20:30:13.000000 letsbuilda-pypi-5.0.0b3/src/letsbuilda/pypi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-21 20:30:13.000000 letsbuilda-pypi-5.0.0b3/src/letsbuilda/pypi/models/models_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-21 20:30:13.000000 letsbuilda-pypi-5.0.0b3/src/letsbuilda/pypi/models/models_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-21 20:30:13.000000 letsbuilda-pypi-5.0.0b3/src/letsbuilda/pypi/models/models_rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-21 20:30:13.000000 letsbuilda-pypi-5.0.0b3/src/letsbuilda/pypi/sync_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:30:24.985936 letsbuilda-pypi-5.0.0b3/src/letsbuilda_pypi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-21 20:30:24.000000 letsbuilda-pypi-5.0.0b3/src/letsbuilda_pypi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-21 20:30:24.000000 letsbuilda-pypi-5.0.0b3/src/letsbuilda_pypi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:30:24.000000 letsbuilda-pypi-5.0.0b3/src/letsbuilda_pypi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-21 20:30:24.000000 letsbuilda-pypi-5.0.0b3/src/letsbuilda_pypi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 20:30:24.000000 letsbuilda-pypi-5.0.0b3/src/letsbuilda_pypi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:30:24.985936 letsbuilda-pypi-5.0.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-21 20:30:13.000000 letsbuilda-pypi-5.0.0b3/tests/test_rss_feed_parsing.py
```

### Comparing `letsbuilda-pypi-5.0.0b2/LICENSE` & `letsbuilda-pypi-5.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-5.0.0b2/PKG-INFO` & `letsbuilda-pypi-5.0.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: letsbuilda-pypi
-Version: 5.0.0b2
+Version: 5.0.0b3
 Summary: A wrapper for PyPI's API and RSS feed
 Author-email: Bradley Reynolds <bradley.reynolds@darbia.dev>
 License: MIT
 Project-URL: repository, https://github.com/letsbuilda/letsbuilda-pypi/
 Project-URL: documentation, https://docs.letsbuilda.dev/letsbuilda-pypi/
-Requires-Python: >=3.11.4
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: async
 Provides-Extra: dev
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `letsbuilda-pypi-5.0.0b2/README.md` & `letsbuilda-pypi-5.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-5.0.0b2/pyproject.toml` & `letsbuilda-pypi-5.0.0b3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "letsbuilda-pypi"
-version = "5.0.0b2"
+version = "5.0.0b3"
 description = "A wrapper for PyPI's API and RSS feed"
 authors = [
     { name = "Bradley Reynolds", email = "bradley.reynolds@darbia.dev" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
-requires-python = ">=3.11.4"
+requires-python = ">=3.11"
 dependencies = [
     "requests",
     "xmltodict",
 ]
 
 [project.urls]
 repository = "https://github.com/letsbuilda/letsbuilda-pypi/"
```

### Comparing `letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/async_client.py` & `letsbuilda-pypi-5.0.0b3/src/letsbuilda/pypi/async_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """The async client."""
 
 from http import HTTPStatus
-from io import BytesIO
 from typing import Final, Self
 
 import xmltodict
 
 try:
     from aiohttp import ClientSession
 except ImportError as error:
@@ -50,18 +49,7 @@
     async def get_package_metadata(
         self: Self,
         package_title: str,
         package_version: str | None = None,
     ) -> Package:
         """Get metadata for a package."""
         return Package.from_json_api_data(await self.get_package_json_metadata(package_title, package_version))
-
-    async def fetch_bytes(
-        self: Self,
-        url: str,
-    ) -> BytesIO:
-        """Fetch bytes from a URL."""
-        buffer = BytesIO()
-        async with self.http_session.get(url) as response:
-            buffer.write(await response.content.read())
-        buffer.seek(0)
-        return buffer
```

### Comparing `letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/models/models_json.py` & `letsbuilda-pypi-5.0.0b3/src/letsbuilda/pypi/models/models_json.py`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/models/models_package.py` & `letsbuilda-pypi-5.0.0b3/src/letsbuilda/pypi/models/models_package.py`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/models/models_rss.py` & `letsbuilda-pypi-5.0.0b3/src/letsbuilda/pypi/models/models_rss.py`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/sync_client.py` & `letsbuilda-pypi-5.0.0b3/src/letsbuilda/pypi/sync_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """The sync client."""
 
 from http import HTTPStatus
-from io import BytesIO
 from typing import Final, Self
 
 import xmltodict
 from requests import Session
 
 from .exceptions import PackageNotFoundError
 from .models import JSONPackageMetadata, Package, RSSPackageMetadata
@@ -44,17 +43,7 @@
     def get_package_metadata(
         self: Self,
         package_title: str,
         package_version: str | None = None,
     ) -> Package:
         """Get metadata for a package."""
         return Package.from_json_api_data(self.get_package_json_metadata(package_title, package_version))
-
-    def fetch_bytes(
-        self: Self,
-        url: str,
-    ) -> BytesIO:
-        """Fetch bytes from a URL."""
-        response = self.http_session.get(url)
-        buffer = BytesIO(response.content)
-        buffer.seek(0)
-        return buffer
```

### Comparing `letsbuilda-pypi-5.0.0b2/src/letsbuilda_pypi.egg-info/PKG-INFO` & `letsbuilda-pypi-5.0.0b3/src/letsbuilda_pypi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: letsbuilda-pypi
-Version: 5.0.0b2
+Version: 5.0.0b3
 Summary: A wrapper for PyPI's API and RSS feed
 Author-email: Bradley Reynolds <bradley.reynolds@darbia.dev>
 License: MIT
 Project-URL: repository, https://github.com/letsbuilda/letsbuilda-pypi/
 Project-URL: documentation, https://docs.letsbuilda.dev/letsbuilda-pypi/
-Requires-Python: >=3.11.4
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: async
 Provides-Extra: dev
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `letsbuilda-pypi-5.0.0b2/src/letsbuilda_pypi.egg-info/SOURCES.txt` & `letsbuilda-pypi-5.0.0b3/src/letsbuilda_pypi.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 src/letsbuilda/pypi/__init__.py
 src/letsbuilda/pypi/async_client.py
 src/letsbuilda/pypi/exceptions.py
-src/letsbuilda/pypi/files.py
 src/letsbuilda/pypi/sync_client.py
 src/letsbuilda/pypi/models/__init__.py
 src/letsbuilda/pypi/models/models_json.py
 src/letsbuilda/pypi/models/models_package.py
 src/letsbuilda/pypi/models/models_rss.py
 src/letsbuilda_pypi.egg-info/PKG-INFO
 src/letsbuilda_pypi.egg-info/SOURCES.txt
```

### Comparing `letsbuilda-pypi-5.0.0b2/tests/test_rss_feed_parsing.py` & `letsbuilda-pypi-5.0.0b3/tests/test_rss_feed_parsing.py`

 * *Files identical despite different names*

