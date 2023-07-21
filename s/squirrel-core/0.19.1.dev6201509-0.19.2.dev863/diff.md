# Comparing `tmp/squirrel_core-0.19.1.dev6201509.tar.gz` & `tmp/squirrel_core-0.19.2.dev863.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squirrel_core-0.19.1.dev6201509.tar", max compression
+gzip compressed data, was "squirrel_core-0.19.2.dev863.tar", max compression
```

## Comparing `squirrel_core-0.19.1.dev6201509.tar` & `squirrel_core-0.19.2.dev863.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    11348 2023-06-22 14:05:15.222763 squirrel_core-0.19.1.dev6201509/LICENSE
--rw-r--r--   0        0        0     5424 2023-06-22 14:05:15.222763 squirrel_core-0.19.1.dev6201509/README.md
--rw-r--r--   0        0        0     2962 2023-06-22 14:14:27.189815 squirrel_core-0.19.1.dev6201509/pyproject.toml
--rw-r--r--   0        0        0       80 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/__init__.py
--rw-r--r--   0        0        0     3253 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/benchmark/quantify_randomness.py
--rw-r--r--   0        0        0      147 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/catalog/__init__.py
--rw-r--r--   0        0        0    14080 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/catalog/catalog.py
--rw-r--r--   0        0        0      937 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/catalog/source.py
--rw-r--r--   0        0        0     2208 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/catalog/yaml.py
--rw-r--r--   0        0        0      581 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/constants.py
--rw-r--r--   0        0        0      887 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/driver/__init__.py
--rw-r--r--   0        0        0     1182 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/driver/csv.py
--rw-r--r--   0        0        0     4511 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/driver/data_frame.py
--rw-r--r--   0        0        0     8479 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/driver/driver.py
--rw-r--r--   0        0        0      977 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/driver/excel.py
--rw-r--r--   0        0        0     1045 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/driver/feather.py
--rw-r--r--   0        0        0     2127 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/driver/file.py
--rw-r--r--   0        0        0     2192 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/driver/jsonl.py
--rw-r--r--   0        0        0     1099 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/driver/msgpack.py
--rw-r--r--   0        0        0     1203 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/driver/parquet.py
--rw-r--r--   0        0        0     5113 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/driver/source_combiner.py
--rw-r--r--   0        0        0     4586 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/driver/store.py
--rw-r--r--   0        0        0     3230 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/driver/zarr.py
--rw-r--r--   0        0        0        0 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/framework/__init__.py
--rw-r--r--   0        0        0      165 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/framework/exceptions.py
--rw-r--r--   0        0        0     2234 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/framework/io.py
--rw-r--r--   0        0        0       30 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/framework/plugins/__init__.py
--rw-r--r--   0        0        0      788 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/framework/plugins/hookimpl.py
--rw-r--r--   0        0        0      644 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/framework/plugins/hookspec.py
--rw-r--r--   0        0        0     1566 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/framework/plugins/plugin_manager.py
--rw-r--r--   0        0        0      410 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/fsspec/__init__.py
--rw-r--r--   0        0        0     1313 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/fsspec/custom_gcsfs.py
--rw-r--r--   0        0        0     2211 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/fsspec/fs.py
--rw-r--r--   0        0        0        0 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/integration_test/__init__.py
--rw-r--r--   0        0        0      466 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/integration_test/conftest.py
--rw-r--r--   0        0        0     1747 2023-06-22 14:05:15.234764 squirrel_core-0.19.1.dev6201509/squirrel/integration_test/helpers.py
--rw-r--r--   0        0        0     3837 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/integration_test/shared_fixtures.py
--rw-r--r--   0        0        0     5841 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py
--rw-r--r--   0        0        0      471 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/iterstream/__init__.py
--rw-r--r--   0        0        0    23744 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/iterstream/base.py
--rw-r--r--   0        0        0     9230 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/iterstream/iterators.py
--rw-r--r--   0        0        0     2289 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/iterstream/metrics.py
--rw-r--r--   0        0        0     5999 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/iterstream/source.py
--rw-r--r--   0        0        0     5202 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/iterstream/torch_composables.py
--rw-r--r--   0        0        0      224 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/py.typed
--rw-r--r--   0        0        0      263 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/serialization/__init__.py
--rw-r--r--   0        0        0     4805 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/serialization/jsonl.py
--rw-r--r--   0        0        0     3471 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/serialization/msgpack.py
--rw-r--r--   0        0        0      750 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/serialization/serializer.py
--rw-r--r--   0        0        0      222 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/store/__init__.py
--rw-r--r--   0        0        0     4588 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/store/filesystem.py
--rw-r--r--   0        0        0     4864 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/store/squirrel_store.py
--rw-r--r--   0        0        0     1880 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/store/store.py
--rw-r--r--   0        0        0      110 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/zarr/__init__.py
--rw-r--r--   0        0        0     6137 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/zarr/group.py
--rw-r--r--   0        0        0     2041 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/zarr/key.py
--rw-r--r--   0        0        0     3794 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/zarr/store.py
--rw-r--r--   0        0        0      832 2023-06-22 14:05:15.238764 squirrel_core-0.19.1.dev6201509/squirrel/zarr/sync.py
--rw-r--r--   0        0        0     8009 1970-01-01 00:00:00.000000 squirrel_core-0.19.1.dev6201509/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-07-21 14:00:48.501347 squirrel_core-0.19.2.dev863/LICENSE
+-rw-r--r--   0        0        0     5424 2023-07-21 14:00:48.501347 squirrel_core-0.19.2.dev863/README.md
+-rw-r--r--   0        0        0     3006 2023-07-21 14:06:11.503828 squirrel_core-0.19.2.dev863/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/__init__.py
+-rw-r--r--   0        0        0     3253 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/benchmark/quantify_randomness.py
+-rw-r--r--   0        0        0      147 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/catalog/__init__.py
+-rw-r--r--   0        0        0    14080 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/catalog/catalog.py
+-rw-r--r--   0        0        0      937 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/catalog/source.py
+-rw-r--r--   0        0        0     2208 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/catalog/yaml.py
+-rw-r--r--   0        0        0      581 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/constants.py
+-rw-r--r--   0        0        0      887 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/__init__.py
+-rw-r--r--   0        0        0     1182 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/csv.py
+-rw-r--r--   0        0        0     4511 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/data_frame.py
+-rw-r--r--   0        0        0     8479 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/driver.py
+-rw-r--r--   0        0        0      977 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/excel.py
+-rw-r--r--   0        0        0     1045 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/feather.py
+-rw-r--r--   0        0        0     2127 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/file.py
+-rw-r--r--   0        0        0     2192 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/jsonl.py
+-rw-r--r--   0        0        0     1099 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/msgpack.py
+-rw-r--r--   0        0        0     1203 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/parquet.py
+-rw-r--r--   0        0        0     5113 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/source_combiner.py
+-rw-r--r--   0        0        0     4586 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/store.py
+-rw-r--r--   0        0        0     3230 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/zarr.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/__init__.py
+-rw-r--r--   0        0        0      165 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/exceptions.py
+-rw-r--r--   0        0        0     2234 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/io.py
+-rw-r--r--   0        0        0       30 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/plugins/__init__.py
+-rw-r--r--   0        0        0      788 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/plugins/hookimpl.py
+-rw-r--r--   0        0        0      644 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/plugins/hookspec.py
+-rw-r--r--   0        0        0     1566 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/plugins/plugin_manager.py
+-rw-r--r--   0        0        0      410 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/fsspec/__init__.py
+-rw-r--r--   0        0        0     1313 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/fsspec/custom_gcsfs.py
+-rw-r--r--   0        0        0     2211 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/fsspec/fs.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/integration_test/__init__.py
+-rw-r--r--   0        0        0      466 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/integration_test/conftest.py
+-rw-r--r--   0        0        0     1747 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/integration_test/helpers.py
+-rw-r--r--   0        0        0     3837 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/integration_test/shared_fixtures.py
+-rw-r--r--   0        0        0     5841 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py
+-rw-r--r--   0        0        0      471 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/iterstream/__init__.py
+-rw-r--r--   0        0        0    23773 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/iterstream/base.py
+-rw-r--r--   0        0        0     9230 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/iterstream/iterators.py
+-rw-r--r--   0        0        0     2289 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/iterstream/metrics.py
+-rw-r--r--   0        0        0     5999 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/iterstream/source.py
+-rw-r--r--   0        0        0     5202 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/iterstream/torch_composables.py
+-rw-r--r--   0        0        0      224 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/py.typed
+-rw-r--r--   0        0        0      263 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/serialization/__init__.py
+-rw-r--r--   0        0        0     4805 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/serialization/jsonl.py
+-rw-r--r--   0        0        0     3471 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/serialization/msgpack.py
+-rw-r--r--   0        0        0      750 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/serialization/serializer.py
+-rw-r--r--   0        0        0      222 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/store/__init__.py
+-rw-r--r--   0        0        0     4588 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/store/filesystem.py
+-rw-r--r--   0        0        0     4864 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/store/squirrel_store.py
+-rw-r--r--   0        0        0     1880 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/store/store.py
+-rw-r--r--   0        0        0      110 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/zarr/__init__.py
+-rw-r--r--   0        0        0     6137 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/zarr/group.py
+-rw-r--r--   0        0        0     2041 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/zarr/key.py
+-rw-r--r--   0        0        0     3794 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/zarr/store.py
+-rw-r--r--   0        0        0      832 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/zarr/sync.py
+-rw-r--r--   0        0        0     8039 1970-01-01 00:00:00.000000 squirrel_core-0.19.2.dev863/PKG-INFO
```

### Comparing `squirrel_core-0.19.1.dev6201509/LICENSE` & `squirrel_core-0.19.2.dev863/LICENSE`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/README.md` & `squirrel_core-0.19.2.dev863/README.md`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/pyproject.toml` & `squirrel_core-0.19.2.dev863/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squirrel-core"
-version = "0.19.1-dev6201509"
+version = "0.19.2-dev863"
 description = "Squirrel is a Python library that enables ML teams to share, load, and transform data in a collaborative, flexible and efficient way."
 authors = ["Merantix Momentum"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "squirrel"}]
 homepage = "https://merantix-momentum.com/technology/squirrel/"
 repository = "https://github.com/merantix-momentum/squirrel-core"
@@ -24,29 +24,29 @@
 fsspec = ">=2021.7.0"
 msgpack = "^1.0.4"
 msgpack-numpy = "^0.4.8"
 more-itertools = "^9.0.0"
 pluggy = "^1.0.0"
 ruamel-yaml = "^0.17.21"
 tqdm = "^4.64.1"
-numba = "^0.56.4"
 numpy = "^1.23.5"
 pyjwt = "^2.4.0"
 mako = "^1.2.2"
 oauthlib = "^3.2.1"
 aiohttp = "^3.7.4"
+numba = {version = "^0.56.4", optional = true}
 adlfs = {version = "<2021.10", optional = true}
 dask = {version = ">=2021.7.0", optional = true, extras = ["dataframe", "distributed"]}
 odfpy = {version = "^1.4.1", optional = true}
 openpyxl = {version = "^3.1.1", optional = true}
 pyxlsb = {version = "^1.0.10", optional = true}
 xlrd = {version = "^2.0.1", optional = true}
 gcsfs = {version = ">=2021.7.0", optional = true}
 s3fs = {version = ">=2021.7.0", optional = true}
-torch = {version = "^1.13.1", optional = true}
+torch = {version = ">=1.13.1", optional = true}
 zarr = {version = "^2.10.3", optional = true}
 pyarrow = {version = "^10.0.1", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.2"
 wheel = "^0.38.4"
 pytest = "^6.2.1"
@@ -77,14 +77,15 @@
 feather = ["pyarrow"]
 gcp = ["gcsfs"]
 parquet = ["pyarrow"]
 s3 = ["s3fs"]
 torch = ["torch"]
 zarr = ["zarr"]
 all = ["adlfs", "dask", "odfpy", "openpyxl", "pyxlsb", "xlrd", "pyarrow", "gcsfs", "s3fs", "torch", "zarr"]
+numba = ["numba"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.autopep8]
 max_line_length = 120
```

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/benchmark/quantify_randomness.py` & `squirrel_core-0.19.2.dev863/squirrel/benchmark/quantify_randomness.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/catalog/catalog.py` & `squirrel_core-0.19.2.dev863/squirrel/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/catalog/source.py` & `squirrel_core-0.19.2.dev863/squirrel/catalog/source.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/catalog/yaml.py` & `squirrel_core-0.19.2.dev863/squirrel/catalog/yaml.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/constants.py` & `squirrel_core-0.19.2.dev863/squirrel/constants.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/driver/__init__.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/driver/csv.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/csv.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/driver/data_frame.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/data_frame.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/driver/driver.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/driver.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/driver/excel.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/excel.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/driver/feather.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/feather.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/driver/file.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/file.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/driver/jsonl.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/jsonl.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/driver/msgpack.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/msgpack.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/driver/parquet.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/parquet.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/driver/source_combiner.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/source_combiner.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/driver/store.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/driver/zarr.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/zarr.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/framework/io.py` & `squirrel_core-0.19.2.dev863/squirrel/framework/io.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/framework/plugins/hookimpl.py` & `squirrel_core-0.19.2.dev863/squirrel/framework/plugins/hookimpl.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/framework/plugins/hookspec.py` & `squirrel_core-0.19.2.dev863/squirrel/framework/plugins/hookspec.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/framework/plugins/plugin_manager.py` & `squirrel_core-0.19.2.dev863/squirrel/framework/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/fsspec/custom_gcsfs.py` & `squirrel_core-0.19.2.dev863/squirrel/fsspec/custom_gcsfs.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/fsspec/fs.py` & `squirrel_core-0.19.2.dev863/squirrel/fsspec/fs.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/integration_test/helpers.py` & `squirrel_core-0.19.2.dev863/squirrel/integration_test/helpers.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/integration_test/shared_fixtures.py` & `squirrel_core-0.19.2.dev863/squirrel/integration_test/shared_fixtures.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py` & `squirrel_core-0.19.2.dev863/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/iterstream/base.py` & `squirrel_core-0.19.2.dev863/squirrel/iterstream/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 import queue
 import typing as t
 from abc import abstractmethod
 from concurrent.futures import Executor, ThreadPoolExecutor
 from copy import deepcopy
 from functools import partial
 
-from numba import jit
-
 from squirrel.constants import MetricsType
 from squirrel.iterstream.iterators import (
     batched_,
     dask_delayed_,
     filter_,
     flatten_,
     map_,
@@ -558,24 +556,26 @@
 class _NumbaMap(Composable):
     def __init__(self, source: t.Iterable, callback: t.Callable):
         super().__init__(source)
         self.callback = callback
 
     def __iter__(self) -> t.Iterator:
         """An iterator"""
-        yield from self._iter_in_jit(self.source, self.callback)
+        from numba import jit
 
-    @jit(forceobj=True)  # need `force object` mode to pass custom types of python objects to numba
-    def _iter_in_jit(self, source: t.Iterable, callback: t.Callable) -> t.Iterator:
-        """
-        Wrap the iterator around numba JIT framework to speed up the iteration, instead of doing asynchronous speed
-        up in a message queue (the default `_AsyncMap` behavior). Only evoked when `executor='numba'` is set.
-        """
-        for item in source:
-            yield callback(item)
+        @jit(forceobj=True)  # need `force object` mode to pass custom types of python objects to numba
+        def _iter_in_jit(source: t.Iterable, callback: t.Callable) -> t.Iterator:
+            """
+            Wrap the iterator around numba JIT framework to speed up the iteration, instead of doing asynchronous speed
+            up in a message queue (the default `_AsyncMap` behavior). Only evoked when `executor='numba'` is set.
+            """
+            for item in source:
+                yield callback(item)
+
+        yield from _iter_in_jit(self.source, self.callback)
 
 
 class _DaskMaterializer(_AsyncMap):
     def __init__(self, source: t.Iterable, buffer: int, max_workers: t.Optional[int] = None):
         """Call the init of the parent class `_AsyncMap` and pass dask.compute as the callback"""
         from dask import compute
```

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/iterstream/iterators.py` & `squirrel_core-0.19.2.dev863/squirrel/iterstream/iterators.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/iterstream/metrics.py` & `squirrel_core-0.19.2.dev863/squirrel/iterstream/metrics.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/iterstream/source.py` & `squirrel_core-0.19.2.dev863/squirrel/iterstream/source.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/iterstream/torch_composables.py` & `squirrel_core-0.19.2.dev863/squirrel/iterstream/torch_composables.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/serialization/jsonl.py` & `squirrel_core-0.19.2.dev863/squirrel/serialization/jsonl.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/serialization/msgpack.py` & `squirrel_core-0.19.2.dev863/squirrel/serialization/msgpack.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/serialization/serializer.py` & `squirrel_core-0.19.2.dev863/squirrel/serialization/serializer.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/store/filesystem.py` & `squirrel_core-0.19.2.dev863/squirrel/store/filesystem.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/store/squirrel_store.py` & `squirrel_core-0.19.2.dev863/squirrel/store/squirrel_store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/store/store.py` & `squirrel_core-0.19.2.dev863/squirrel/store/store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/zarr/group.py` & `squirrel_core-0.19.2.dev863/squirrel/zarr/group.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/zarr/key.py` & `squirrel_core-0.19.2.dev863/squirrel/zarr/key.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/zarr/store.py` & `squirrel_core-0.19.2.dev863/squirrel/zarr/store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/squirrel/zarr/sync.py` & `squirrel_core-0.19.2.dev863/squirrel/zarr/sync.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.1.dev6201509/PKG-INFO` & `squirrel_core-0.19.2.dev863/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squirrel-core
-Version: 0.19.1.dev6201509
+Version: 0.19.2.dev863
 Summary: Squirrel is a Python library that enables ML teams to share, load, and transform data in a collaborative, flexible and efficient way.
 Home-page: https://merantix-momentum.com/technology/squirrel/
 License: Apache 2.0
 Author: Merantix Momentum
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
@@ -17,39 +17,40 @@
 Classifier: Typing :: Typed
 Provides-Extra: all
 Provides-Extra: azure
 Provides-Extra: dask
 Provides-Extra: excel
 Provides-Extra: feather
 Provides-Extra: gcp
+Provides-Extra: numba
 Provides-Extra: parquet
 Provides-Extra: s3
 Provides-Extra: torch
 Provides-Extra: zarr
 Requires-Dist: adlfs (<2021.10) ; extra == "azure" or extra == "all"
 Requires-Dist: aiohttp (>=3.7.4,<4.0.0)
 Requires-Dist: dask[dataframe,distributed] (>=2021.7.0) ; extra == "dask" or extra == "all"
 Requires-Dist: fsspec (>=2021.7.0)
 Requires-Dist: gcsfs (>=2021.7.0) ; extra == "gcp" or extra == "all"
 Requires-Dist: mako (>=1.2.2,<2.0.0)
 Requires-Dist: more-itertools (>=9.0.0,<10.0.0)
 Requires-Dist: msgpack (>=1.0.4,<2.0.0)
 Requires-Dist: msgpack-numpy (>=0.4.8,<0.5.0)
-Requires-Dist: numba (>=0.56.4,<0.57.0)
+Requires-Dist: numba (>=0.56.4,<0.57.0) ; extra == "numba"
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: oauthlib (>=3.2.1,<4.0.0)
 Requires-Dist: odfpy (>=1.4.1,<2.0.0) ; extra == "excel" or extra == "all"
 Requires-Dist: openpyxl (>=3.1.1,<4.0.0) ; extra == "excel" or extra == "all"
 Requires-Dist: pluggy (>=1.0.0,<2.0.0)
 Requires-Dist: pyarrow (>=10.0.1,<11.0.0) ; extra == "feather" or extra == "parquet" or extra == "all"
 Requires-Dist: pyjwt (>=2.4.0,<3.0.0)
 Requires-Dist: pyxlsb (>=1.0.10,<2.0.0) ; extra == "excel" or extra == "all"
 Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
 Requires-Dist: s3fs (>=2021.7.0) ; extra == "s3" or extra == "all"
-Requires-Dist: torch (>=1.13.1,<2.0.0) ; extra == "torch" or extra == "all"
+Requires-Dist: torch (>=1.13.1) ; extra == "torch" or extra == "all"
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: xlrd (>=2.0.1,<3.0.0) ; extra == "excel" or extra == "all"
 Requires-Dist: zarr (>=2.10.3,<3.0.0) ; extra == "zarr" or extra == "all"
 Project-URL: Documentation, https://squirrel-core.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/merantix-momentum/squirrel-core
 Description-Content-Type: text/markdown
```

