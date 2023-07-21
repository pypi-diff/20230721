# Comparing `tmp/openid_whisperer-0.1.8.tar.gz` & `tmp/openid_whisperer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openid_whisperer-0.1.8.tar", max compression
+gzip compressed data, was "openid_whisperer-0.1.9.tar", max compression
```

## Comparing `openid_whisperer-0.1.8.tar` & `openid_whisperer-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1153 2023-06-25 20:59:05.837711 openid_whisperer-0.1.8/LICENSE
--rw-r--r--   0        0        0     6665 2023-07-21 19:06:13.430139 openid_whisperer-0.1.8/README.md
--rw-r--r--   0        0        0     2144 2023-07-21 19:57:08.470386 openid_whisperer-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-03 22:59:15.739113 openid_whisperer-0.1.8/src/openid_whisperer/__init__.py
--rw-r--r--   0        0        0       83 2023-06-03 22:59:15.739296 openid_whisperer-0.1.8/src/openid_whisperer/__main__.py
--rw-r--r--   0        0        0     8889 2023-07-19 16:17:02.507285 openid_whisperer-0.1.8/src/openid_whisperer/config.py
--rw-r--r--   0        0        0     2539 2023-07-13 16:49:06.224941 openid_whisperer-0.1.8/src/openid_whisperer/demo_certs/ca_cert.pem
--rw-r--r--   0        0        0     2681 2023-07-13 16:49:06.225650 openid_whisperer-0.1.8/src/openid_whisperer/demo_certs/cert.pem
--rw-r--r--   0        0        0     1675 2023-07-13 16:49:06.226302 openid_whisperer-0.1.8/src/openid_whisperer/demo_certs/key.pem
--rw-r--r--   0        0        0     1135 2023-07-20 14:49:18.489462 openid_whisperer-0.1.8/src/openid_whisperer/main.py
--rw-r--r--   0        0        0    22460 2023-07-21 15:38:16.110824 openid_whisperer-0.1.8/src/openid_whisperer/openid_blueprint.py
--rw-r--r--   0        0        0    33492 2023-07-21 18:50:19.320462 openid_whisperer-0.1.8/src/openid_whisperer/openid_interface.py
--rw-r--r--   0        0        0      910 2023-07-14 12:33:04.149317 openid_whisperer-0.1.8/src/openid_whisperer/openid_types.py
--rw-r--r--   0        0        0        0 2023-06-04 10:12:20.232971 openid_whisperer-0.1.8/src/openid_whisperer/py.typed
--rw-r--r--   0        0        0     7774 2023-07-04 18:12:57.431778 openid_whisperer-0.1.8/src/openid_whisperer/static/style.css
--rw-r--r--   0        0        0    29021 2023-07-19 16:34:51.108344 openid_whisperer-0.1.8/src/openid_whisperer/templates/authenticate.html
--rw-r--r--   0        0        0      451 2023-07-19 17:15:03.303758 openid_whisperer-0.1.8/src/openid_whisperer/templates/form_post_response.html
--rw-r--r--   0        0        0        0 2023-07-01 16:06:18.981399 openid_whisperer-0.1.8/src/openid_whisperer/utils/__init__.py
--rw-r--r--   0        0        0     5082 2023-07-14 12:36:54.560754 openid_whisperer-0.1.8/src/openid_whisperer/utils/cert_utils.py
--rw-r--r--   0        0        0     6865 2023-07-21 12:59:14.882179 openid_whisperer-0.1.8/src/openid_whisperer/utils/common.py
--rw-r--r--   0        0        0     6144 2023-07-14 12:22:20.152374 openid_whisperer-0.1.8/src/openid_whisperer/utils/config_utils.py
--rw-r--r--   0        0        0     4812 2023-07-14 14:21:24.986862 openid_whisperer-0.1.8/src/openid_whisperer/utils/credential_store.py
--rw-r--r--   0        0        0     3637 2023-07-20 14:49:18.532645 openid_whisperer-0.1.8/src/openid_whisperer/utils/test_utils.py
--rw-r--r--   0        0        0    21916 2023-07-21 19:56:42.003073 openid_whisperer-0.1.8/src/openid_whisperer/utils/token_store.py
--rw-r--r--   0        0        0     3188 2023-07-14 12:43:25.019940 openid_whisperer-0.1.8/src/openid_whisperer/utils/token_utils.py
--rw-r--r--   0        0        0    10641 2023-07-20 14:49:18.662763 openid_whisperer-0.1.8/src/openid_whisperer/utils/user_info_ext.py
--rw-r--r--   0        0        0     7751 1970-01-01 00:00:00.000000 openid_whisperer-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-06-25 20:59:05.837711 openid_whisperer-0.1.9/LICENSE
+-rw-r--r--   0        0        0     6665 2023-07-21 19:59:36.289840 openid_whisperer-0.1.9/README.md
+-rw-r--r--   0        0        0     2144 2023-07-21 20:06:03.495874 openid_whisperer-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-03 22:59:15.739113 openid_whisperer-0.1.9/src/openid_whisperer/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-03 22:59:15.739296 openid_whisperer-0.1.9/src/openid_whisperer/__main__.py
+-rw-r--r--   0        0        0     8889 2023-07-19 16:17:02.507285 openid_whisperer-0.1.9/src/openid_whisperer/config.py
+-rw-r--r--   0        0        0     2539 2023-07-13 16:49:06.224941 openid_whisperer-0.1.9/src/openid_whisperer/demo_certs/ca_cert.pem
+-rw-r--r--   0        0        0     2681 2023-07-13 16:49:06.225650 openid_whisperer-0.1.9/src/openid_whisperer/demo_certs/cert.pem
+-rw-r--r--   0        0        0     1675 2023-07-13 16:49:06.226302 openid_whisperer-0.1.9/src/openid_whisperer/demo_certs/key.pem
+-rw-r--r--   0        0        0     1178 2023-07-21 21:27:24.916359 openid_whisperer-0.1.9/src/openid_whisperer/main.py
+-rw-r--r--   0        0        0    22497 2023-07-21 21:37:43.819352 openid_whisperer-0.1.9/src/openid_whisperer/openid_blueprint.py
+-rw-r--r--   0        0        0    33492 2023-07-21 18:50:19.320462 openid_whisperer-0.1.9/src/openid_whisperer/openid_interface.py
+-rw-r--r--   0        0        0      910 2023-07-14 12:33:04.149317 openid_whisperer-0.1.9/src/openid_whisperer/openid_types.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:12:20.232971 openid_whisperer-0.1.9/src/openid_whisperer/py.typed
+-rw-r--r--   0        0        0     7774 2023-07-04 18:12:57.431778 openid_whisperer-0.1.9/src/openid_whisperer/static/style.css
+-rw-r--r--   0        0        0    29022 2023-07-21 21:28:06.069132 openid_whisperer-0.1.9/src/openid_whisperer/templates/authenticate.html
+-rw-r--r--   0        0        0      451 2023-07-19 17:15:03.303758 openid_whisperer-0.1.9/src/openid_whisperer/templates/form_post_response.html
+-rw-r--r--   0        0        0        0 2023-07-01 16:06:18.981399 openid_whisperer-0.1.9/src/openid_whisperer/utils/__init__.py
+-rw-r--r--   0        0        0     5082 2023-07-14 12:36:54.560754 openid_whisperer-0.1.9/src/openid_whisperer/utils/cert_utils.py
+-rw-r--r--   0        0        0     6865 2023-07-21 12:59:14.882179 openid_whisperer-0.1.9/src/openid_whisperer/utils/common.py
+-rw-r--r--   0        0        0     6144 2023-07-14 12:22:20.152374 openid_whisperer-0.1.9/src/openid_whisperer/utils/config_utils.py
+-rw-r--r--   0        0        0     4812 2023-07-14 14:21:24.986862 openid_whisperer-0.1.9/src/openid_whisperer/utils/credential_store.py
+-rw-r--r--   0        0        0     3637 2023-07-20 14:49:18.532645 openid_whisperer-0.1.9/src/openid_whisperer/utils/test_utils.py
+-rw-r--r--   0        0        0    21916 2023-07-21 19:56:42.003073 openid_whisperer-0.1.9/src/openid_whisperer/utils/token_store.py
+-rw-r--r--   0        0        0     3188 2023-07-14 12:43:25.019940 openid_whisperer-0.1.9/src/openid_whisperer/utils/token_utils.py
+-rw-r--r--   0        0        0    10641 2023-07-20 14:49:18.662763 openid_whisperer-0.1.9/src/openid_whisperer/utils/user_info_ext.py
+-rw-r--r--   0        0        0     7751 1970-01-01 00:00:00.000000 openid_whisperer-0.1.9/PKG-INFO
```

### Comparing `openid_whisperer-0.1.8/LICENSE` & `openid_whisperer-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.8/README.md` & `openid_whisperer-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -134,10 +134,10 @@
 Run OpenID Whisperer (from project root)
 ```
 poetry run python -m openid_whisperer.main 
 ```
 
 Run within a Docker Container
 ```
-docker build -t opendid-whisperer:0.1.4 .
-docker run --name=openid-whisperer -p5005:5005  -eID_SERVICE_PORT_GW=5005 opendid-whisperer:0.1.4
+docker build -t opendid-whisperer:0.1.8 .
+docker run --name=openid-whisperer -p5005:5005  -eID_SERVICE_PORT_GW=5005 opendid-whisperer:0.1.8
 ```
```

### Comparing `openid_whisperer-0.1.8/pyproject.toml` & `openid_whisperer-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openid-whisperer"
-version = "0.1.8"
+version = "0.1.9"
 description = "OpenID 1.0 Mock Identity Service"
 license = "MIT"
 authors = ["Robert Betts <betts_robert@yahoo.com>"]
 maintainers = ["Robert Betts <betts_robert@yahoo.com>"]
 readme = "README.md"
 homepage = "https://github.com/robertbetts/openid-whisperer"
 repository = "https://github.com/robertbetts/openid-whisperer"
```

### Comparing `openid_whisperer-0.1.8/src/openid_whisperer/config.py` & `openid_whisperer-0.1.9/src/openid_whisperer/config.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.8/src/openid_whisperer/demo_certs/ca_cert.pem` & `openid_whisperer-0.1.9/src/openid_whisperer/demo_certs/ca_cert.pem`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.8/src/openid_whisperer/demo_certs/cert.pem` & `openid_whisperer-0.1.9/src/openid_whisperer/demo_certs/cert.pem`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.8/src/openid_whisperer/demo_certs/key.pem` & `openid_whisperer-0.1.9/src/openid_whisperer/demo_certs/key.pem`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.8/src/openid_whisperer/main.py` & `openid_whisperer-0.1.9/src/openid_whisperer/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 config.init_logging()
 
 
 def app() -> "Flask":
     """returns WSGI compliant Object wrapper for openid_whisperer"""
     from flask import Flask
 
-    flask_app = Flask("openid_whisperer")
+    flask_app = Flask(
+        "openid_whisperer",
+        static_folder=None,
+    )
     flask_app.register_blueprint(openid_blueprint)
     return flask_app
 
 
 def main() -> None:  # pragma: no cover
     """Main entrypoint for a standalone Python running instance"""
     ca_certs = [config.ca_cert] if config.ca_cert else None
```

### Comparing `openid_whisperer-0.1.8/src/openid_whisperer/openid_blueprint.py` & `openid_whisperer-0.1.9/src/openid_whisperer/openid_blueprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 )
 
 openid_blueprint: Blueprint = Blueprint(
     "openid",
     __name__,
     template_folder="templates",
     static_folder="static",
+    static_url_path="/openid/static"
 )
 
 
 def update_redirect_url_query(
     redirect_uri: str, data: Dict[str, Any]
 ) -> ResponseReturnValue:
     if len(data) > 0:
```

### Comparing `openid_whisperer-0.1.8/src/openid_whisperer/openid_interface.py` & `openid_whisperer-0.1.9/src/openid_whisperer/openid_interface.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.8/src/openid_whisperer/openid_types.py` & `openid_whisperer-0.1.9/src/openid_whisperer/openid_types.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.8/src/openid_whisperer/static/style.css` & `openid_whisperer-0.1.9/src/openid_whisperer/static/style.css`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.8/src/openid_whisperer/templates/authenticate.html` & `openid_whisperer-0.1.9/src/openid_whisperer/templates/authenticate.html`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
                     node.placeholder = placeholderText;
                 }
             }
         };
 
         //]]>
     </script>
-    <link rel="stylesheet" type="text/css" href="{{url_for('openid.static', filename='style.css') }}" />
+    <link rel="stylesheet" type="text/css" href="{{ url_for('openid.static', filename='style.css') }}" />
 </head>
 <body dir="ltr" class="body">
 <div id="noScript" style="position:static; width:100%; height:100%; z-index:100">
     <h1>JavaScript is required</h1>
     <p>This web browser does not support JavaScript or JavaScript in this web browser is not enabled.</p>
     <p>To find out if your web browser supports JavaScript or to enable JavaScript, see web browser help.</p>
 </div>
```

### Comparing `openid_whisperer-0.1.8/src/openid_whisperer/utils/cert_utils.py` & `openid_whisperer-0.1.9/src/openid_whisperer/utils/cert_utils.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.8/src/openid_whisperer/utils/common.py` & `openid_whisperer-0.1.9/src/openid_whisperer/utils/common.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.8/src/openid_whisperer/utils/config_utils.py` & `openid_whisperer-0.1.9/src/openid_whisperer/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.8/src/openid_whisperer/utils/credential_store.py` & `openid_whisperer-0.1.9/src/openid_whisperer/utils/credential_store.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.8/src/openid_whisperer/utils/test_utils.py` & `openid_whisperer-0.1.9/src/openid_whisperer/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.8/src/openid_whisperer/utils/token_store.py` & `openid_whisperer-0.1.9/src/openid_whisperer/utils/token_store.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.8/src/openid_whisperer/utils/token_utils.py` & `openid_whisperer-0.1.9/src/openid_whisperer/utils/token_utils.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.8/src/openid_whisperer/utils/user_info_ext.py` & `openid_whisperer-0.1.9/src/openid_whisperer/utils/user_info_ext.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.8/PKG-INFO` & `openid_whisperer-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openid-whisperer
-Version: 0.1.8
+Version: 0.1.9
 Summary: OpenID 1.0 Mock Identity Service
 Home-page: https://github.com/robertbetts/openid-whisperer
 License: MIT
 Keywords: python,mock,api,oauth2,openid
 Author: Robert Betts
 Author-email: betts_robert@yahoo.com
 Maintainer: Robert Betts
@@ -162,10 +162,10 @@
 Run OpenID Whisperer (from project root)
 ```
 poetry run python -m openid_whisperer.main 
 ```
 
 Run within a Docker Container
 ```
-docker build -t opendid-whisperer:0.1.4 .
-docker run --name=openid-whisperer -p5005:5005  -eID_SERVICE_PORT_GW=5005 opendid-whisperer:0.1.4
+docker build -t opendid-whisperer:0.1.8 .
+docker run --name=openid-whisperer -p5005:5005  -eID_SERVICE_PORT_GW=5005 opendid-whisperer:0.1.8
 ```
```

