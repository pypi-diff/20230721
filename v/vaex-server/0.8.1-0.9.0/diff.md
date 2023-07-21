# Comparing `tmp/vaex-server-0.8.1.tar.gz` & `tmp/vaex-server-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vaex-server-0.8.1.tar", last modified: Mon Feb  7 14:36:41 2022, max compression
+gzip compressed data, was "dist/vaex-server-0.9.0.tar", last modified: Fri Jul 21 10:38:31 2023, max compression
```

## Comparing `vaex-server-0.8.1.tar` & `vaex-server-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-07 14:36:41.000000 vaex-server-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1087 2022-02-07 14:36:29.000000 vaex-server-0.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)       20 2022-02-07 14:36:29.000000 vaex-server-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      290 2022-02-07 14:36:41.000000 vaex-server-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-02-07 14:36:41.000000 vaex-server-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      926 2022-02-07 14:36:29.000000 vaex-server-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-07 14:36:41.000000 vaex-server-0.8.1/vaex/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-07 14:36:41.000000 vaex-server-0.8.1/vaex/server/
--rw-r--r--   0 runner    (1001) docker     (116)      204 2022-02-07 14:36:29.000000 vaex-server-0.8.1/vaex/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       64 2022-02-07 14:36:29.000000 vaex-server-0.8.1/vaex/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)       52 2022-02-07 14:36:29.000000 vaex-server-0.8.1/vaex/server/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     4169 2022-02-07 14:36:29.000000 vaex-server-0.8.1/vaex/server/client.py
--rw-r--r--   0 runner    (1001) docker     (116)     6587 2022-02-07 14:36:29.000000 vaex-server-0.8.1/vaex/server/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (116)     2487 2022-02-07 14:36:29.000000 vaex-server-0.8.1/vaex/server/dummy.py
--rw-r--r--   0 runner    (1001) docker     (116)     1753 2022-02-07 14:36:29.000000 vaex-server-0.8.1/vaex/server/executor.py
--rw-r--r--   0 runner    (1001) docker     (116)    16124 2022-02-07 14:36:29.000000 vaex-server-0.8.1/vaex/server/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (116)     5999 2022-02-07 14:36:29.000000 vaex-server-0.8.1/vaex/server/index.html
--rw-r--r--   0 runner    (1001) docker     (116)       26 2022-02-07 14:36:29.000000 vaex-server-0.8.1/vaex/server/server.py
--rw-r--r--   0 runner    (1001) docker     (116)     3349 2022-02-07 14:36:29.000000 vaex-server-0.8.1/vaex/server/service.py
--rw-r--r--   0 runner    (1001) docker     (116)      650 2022-02-07 14:36:29.000000 vaex-server-0.8.1/vaex/server/settings.py
--rw-r--r--   0 runner    (1001) docker     (116)     5000 2022-02-07 14:36:29.000000 vaex-server-0.8.1/vaex/server/tornado_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     9913 2022-02-07 14:36:29.000000 vaex-server-0.8.1/vaex/server/tornado_server.py
--rw-r--r--   0 runner    (1001) docker     (116)      691 2022-02-07 14:36:29.000000 vaex-server-0.8.1/vaex/server/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     6582 2022-02-07 14:36:29.000000 vaex-server-0.8.1/vaex/server/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-07 14:36:41.000000 vaex-server-0.8.1/vaex_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      290 2022-02-07 14:36:41.000000 vaex-server-0.8.1/vaex_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      625 2022-02-07 14:36:41.000000 vaex-server-0.8.1/vaex_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-07 14:36:41.000000 vaex-server-0.8.1/vaex_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-07 14:36:41.000000 vaex-server-0.8.1/vaex_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       69 2022-02-07 14:36:41.000000 vaex-server-0.8.1/vaex_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        5 2022-02-07 14:36:41.000000 vaex-server-0.8.1/vaex_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:38:31.000000 vaex-server-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-07-21 10:38:16.000000 vaex-server-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-21 10:38:16.000000 vaex-server-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      290 2023-07-21 10:38:31.000000 vaex-server-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-21 10:38:31.000000 vaex-server-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      926 2023-07-21 10:38:16.000000 vaex-server-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:38:31.000000 vaex-server-0.9.0/vaex/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:38:31.000000 vaex-server-0.9.0/vaex/server/
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-07-21 10:38:16.000000 vaex-server-0.9.0/vaex/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-21 10:38:16.000000 vaex-server-0.9.0/vaex/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-07-21 10:38:16.000000 vaex-server-0.9.0/vaex/server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4169 2023-07-21 10:38:16.000000 vaex-server-0.9.0/vaex/server/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6587 2023-07-21 10:38:16.000000 vaex-server-0.9.0/vaex/server/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2487 2023-07-21 10:38:16.000000 vaex-server-0.9.0/vaex/server/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-07-21 10:38:16.000000 vaex-server-0.9.0/vaex/server/executor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16318 2023-07-21 10:38:16.000000 vaex-server-0.9.0/vaex/server/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5999 2023-07-21 10:38:16.000000 vaex-server-0.9.0/vaex/server/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-21 10:38:16.000000 vaex-server-0.9.0/vaex/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3349 2023-07-21 10:38:16.000000 vaex-server-0.9.0/vaex/server/service.py
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-07-21 10:38:16.000000 vaex-server-0.9.0/vaex/server/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5000 2023-07-21 10:38:16.000000 vaex-server-0.9.0/vaex/server/tornado_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9913 2023-07-21 10:38:16.000000 vaex-server-0.9.0/vaex/server/tornado_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-07-21 10:38:16.000000 vaex-server-0.9.0/vaex/server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6582 2023-07-21 10:38:16.000000 vaex-server-0.9.0/vaex/server/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:38:31.000000 vaex-server-0.9.0/vaex_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      290 2023-07-21 10:38:31.000000 vaex-server-0.9.0/vaex_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-07-21 10:38:31.000000 vaex-server-0.9.0/vaex_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 10:38:31.000000 vaex-server-0.9.0/vaex_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 10:38:31.000000 vaex-server-0.9.0/vaex_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-21 10:38:31.000000 vaex-server-0.9.0/vaex_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-21 10:38:31.000000 vaex-server-0.9.0/vaex_server.egg-info/top_level.txt
```

### Comparing `vaex-server-0.8.1/LICENSE.txt` & `vaex-server-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vaex-server-0.8.1/setup.py` & `vaex-server-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `vaex-server-0.8.1/vaex/server/client.py` & `vaex-server-0.9.0/vaex/server/client.py`

 * *Files identical despite different names*

### Comparing `vaex-server-0.8.1/vaex/server/dataframe.py` & `vaex-server-0.9.0/vaex/server/dataframe.py`

 * *Files identical despite different names*

### Comparing `vaex-server-0.8.1/vaex/server/dummy.py` & `vaex-server-0.9.0/vaex/server/dummy.py`

 * *Files identical despite different names*

### Comparing `vaex-server-0.8.1/vaex/server/executor.py` & `vaex-server-0.9.0/vaex/server/executor.py`

 * *Files identical despite different names*

### Comparing `vaex-server-0.8.1/vaex/server/fastapi.py` & `vaex-server-0.9.0/vaex/server/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from fastapi.security import OAuth2PasswordBearer
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import Response
 from fastapi.openapi.docs import get_swagger_ui_html
 import requests
 
 
-from pydantic import BaseModel, BaseSettings
+from pydantic import BaseModel
 from starlette.responses import HTMLResponse, PlainTextResponse
 
 
 import vaex
 import vaex.server
 import vaex.settings
 import vaex.server.websocket
@@ -40,16 +40,16 @@
 
 class HistogramInput(BaseModel):
     dataset_id: str
     expression: str
     shape: int = 128
     min: Optional[Union[float, int, str]] = None
     max: Optional[Union[float, int, str]] = None
-    filter: str = None
-    virtual_columns: Dict[str, str] = None
+    filter: Optional[str] = None
+    virtual_columns: Optional[Dict[str, str]] = None
 
 
 class HistogramOutput(BaseModel):
     dataset_id: str
     # expression: str
     # what: str
     # bins: List[int]
@@ -64,16 +64,16 @@
     expression_y: str
     shape_x: int = 128
     shape_y: int = 128
     min_x: Optional[Union[float, int, str]] = None
     max_x: Optional[Union[float, int, str]] = None
     min_y: Optional[Union[float, int, str]] = None
     max_y: Optional[Union[float, int, str]] = None
-    filter: str = None
-    virtual_columns: Dict[str, str] = None
+    filter: Optional[str] = None
+    virtual_columns: Optional[Dict[str, str]] = None
 
 
 class HeatmapOutput(BaseModel):
     dataset_id: str
     expression_x: str
     expression_y: str
     # expression: str
@@ -135,17 +135,25 @@
 @contextlib.contextmanager
 def get_df(name):
     if name not in datasets:
         raise HTTPException(status_code=404, detail=f"dataset {name!r} not found")
     yield vaex.from_dataset(datasets[name])
 
 
+def _number(v):
+    if v is None:
+        return v
+    try:
+        return float(v)
+    except:
+        return v
+
 async def _compute_histogram(input: HistogramInput) -> HistogramOutput:
     with get_df(input.dataset_id) as df:
-        limits = [input.min, input.max]
+        limits = [_number(input.min), _number(input.max)]
         limits = df.limits(input.expression, limits, delay=True)
         await df.execute_async()
         limits = await limits
 
         counts = df.count(binby=input.expression, limits=limits, shape=input.shape, delay=True, selection=input.filter)
         await df.execute_async()
         counts = await counts
@@ -181,16 +189,16 @@
         fig.canvas.print_png(f)
         plt.close(fig)
         return ImageResponse(content=f.getvalue())
 
 
 async def _compute_heatmap(input: HeatmapInput) -> HeatmapOutput:
     with get_df(input.dataset_id) as df:
-        limits_x = [input.min_x, input.max_x]
-        limits_y = [input.min_y, input.max_y]
+        limits_x = [_number(input.min_x), _number(input.max_x)]
+        limits_y = [_number(input.min_y), _number(input.max_y)]
         limits_x = df.limits(input.expression_x, limits_x, delay=True)
         limits_y = df.limits(input.expression_y, limits_y, delay=True)
         await df.execute_async()
         limits_x = await limits_x
         limits_y = await limits_y
 
         limits = [limits_x, limits_y]
```

### Comparing `vaex-server-0.8.1/vaex/server/index.html` & `vaex-server-0.9.0/vaex/server/index.html`

 * *Files identical despite different names*

### Comparing `vaex-server-0.8.1/vaex/server/service.py` & `vaex-server-0.9.0/vaex/server/service.py`

 * *Files identical despite different names*

### Comparing `vaex-server-0.8.1/vaex/server/settings.py` & `vaex-server-0.9.0/vaex/server/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 
 from typing import Dict
-from pydantic import BaseSettings, Field
+from pydantic import Field
+import pydantic
 import vaex.config
+from ..minisettings import BaseSettings, Field
+
 
 class Settings(BaseSettings):
     '''Configuration options for the FastAPI server'''
     # vaex_config_file: str = "vaex-server.json"
     add_example: bool = Field(True, title="Add example dataset")
     # vaex_config: dict = None
     graphql: bool = Field(False, title="Add graphql endpoint")
-    files: Dict[str, str] = Field(default_factory=list, title="Mapping of name to path")
+    files: Dict[str, str] = Field(default_factory=dict, title="Mapping of name to path")
     class Config(vaex.config.ConfigDefault):
         env_file = '.env'
         env_file_encoding = 'utf-8'
         env_prefix = 'vaex_server_'
         # secrets_dir = '/run/secrets'
```

### Comparing `vaex-server-0.8.1/vaex/server/tornado_client.py` & `vaex-server-0.9.0/vaex/server/tornado_client.py`

 * *Files identical despite different names*

### Comparing `vaex-server-0.8.1/vaex/server/tornado_server.py` & `vaex-server-0.9.0/vaex/server/tornado_server.py`

 * *Files identical despite different names*

### Comparing `vaex-server-0.8.1/vaex/server/utils.py` & `vaex-server-0.9.0/vaex/server/utils.py`

 * *Files identical despite different names*

### Comparing `vaex-server-0.8.1/vaex/server/websocket.py` & `vaex-server-0.9.0/vaex/server/websocket.py`

 * *Files identical despite different names*

### Comparing `vaex-server-0.8.1/vaex_server.egg-info/SOURCES.txt` & `vaex-server-0.9.0/vaex_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

