# Comparing `tmp/etc_jupyterlab_notebook_state_provider-2.0.9.tar.gz` & `tmp/etc_jupyterlab_notebook_state_provider-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etc_jupyterlab_notebook_state_provider-2.0.9.tar", last modified: Tue Aug  2 01:46:10 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `etc_jupyterlab_notebook_state_provider-2.0.9.tar` & `etc_jupyterlab_notebook_state_provider-2.1.0.tar`

### file list

```diff
@@ -1,57 +1,38 @@
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-02 01:46:10.725955 etc_jupyterlab_notebook_state_provider-2.0.9/
--rw-rw-r--   0 null      (1000) null      (1000)     1503 2022-06-22 18:48:28.000000 etc_jupyterlab_notebook_state_provider-2.0.9/LICENSE
--rw-rw-r--   0 null      (1000) null      (1000)      509 2022-06-22 18:48:28.000000 etc_jupyterlab_notebook_state_provider-2.0.9/MANIFEST.in
--rw-rw-r--   0 null      (1000) null      (1000)     6001 2022-08-02 01:46:10.724955 etc_jupyterlab_notebook_state_provider-2.0.9/PKG-INFO
--rw-rw-r--   0 null      (1000) null      (1000)     4946 2022-06-22 18:48:28.000000 etc_jupyterlab_notebook_state_provider-2.0.9/README.md
--rw-rw-r--   0 null      (1000) null      (1000)     1922 2022-06-22 18:48:28.000000 etc_jupyterlab_notebook_state_provider-2.0.9/RELEASE.md
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-02 01:46:10.716955 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/
--rw-rw-r--   0 null      (1000) null      (1000)      655 2022-07-01 02:04:39.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/__init__.py
--rw-rw-r--   0 null      (1000) null      (1000)      440 2022-06-22 18:48:28.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/_version.py
--rw-r--r--   0 null      (1000) null      (1000)      680 2022-07-05 17:06:45.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/application.py
--rw-rw-r--   0 null      (1000) null      (1000)     1023 2022-07-05 15:10:13.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/handlers.py
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-02 01:46:10.718955 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/labextension/
--rw-rw-r--   0 null      (1000) null      (1000)    22085 2022-08-02 01:45:42.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/labextension/build_log.json
--rw-rw-r--   0 null      (1000) null      (1000)     3173 2022-08-02 01:45:43.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/labextension/package.json
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-02 01:46:10.709955 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/labextension/schemas/
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-02 01:46:10.709955 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/labextension/schemas/@educational-technology-collective/
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-02 01:46:10.718955 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/labextension/schemas/@educational-technology-collective/etc_jupyterlab_notebook_state_provider/
--rw-rw-r--   0 null      (1000) null      (1000)     3031 2022-08-02 01:45:42.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/labextension/schemas/@educational-technology-collective/etc_jupyterlab_notebook_state_provider/package.json.orig
--rw-rw-r--   0 null      (1000) null      (1000)      298 2022-08-02 01:45:42.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/labextension/schemas/@educational-technology-collective/etc_jupyterlab_notebook_state_provider/plugin.json
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-02 01:46:10.721955 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/labextension/static/
--rw-rw-r--   0 null      (1000) null      (1000)    11098 2022-08-02 01:45:43.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/labextension/static/lib_index_js.a4a3e5d1150e7a5b5586.js
--rw-rw-r--   0 null      (1000) null      (1000)    10167 2022-08-02 01:45:43.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/labextension/static/lib_index_js.a4a3e5d1150e7a5b5586.js.map
--rw-rw-r--   0 null      (1000) null      (1000)    28523 2022-08-02 01:45:43.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/labextension/static/remoteEntry.e2d4f614a13c9a73d829.js
--rw-rw-r--   0 null      (1000) null      (1000)    28215 2022-08-02 01:45:43.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/labextension/static/remoteEntry.e2d4f614a13c9a73d829.js.map
--rw-rw-r--   0 null      (1000) null      (1000)      216 2022-08-02 01:45:42.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/labextension/static/style.js
--rw-rw-r--   0 null      (1000) null      (1000)     4370 2022-08-02 01:45:43.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/labextension/static/style_index_js.f1e41f76c7e386a2a0b8.js
--rw-rw-r--   0 null      (1000) null      (1000)     1591 2022-08-02 01:45:43.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/labextension/static/style_index_js.f1e41f76c7e386a2a0b8.js.map
--rw-rw-r--   0 null      (1000) null      (1000)    12176 2022-08-02 01:45:43.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.0fdbe371458a254e2588.js
--rw-rw-r--   0 null      (1000) null      (1000)    13967 2022-08-02 01:45:43.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.0fdbe371458a254e2588.js.map
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-02 01:46:10.717955 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider.egg-info/
--rw-rw-r--   0 null      (1000) null      (1000)     6001 2022-08-02 01:46:10.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider.egg-info/PKG-INFO
--rw-rw-r--   0 null      (1000) null      (1000)     2386 2022-08-02 01:46:10.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider.egg-info/SOURCES.txt
--rw-rw-r--   0 null      (1000) null      (1000)        1 2022-08-02 01:46:10.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider.egg-info/dependency_links.txt
--rw-rw-r--   0 null      (1000) null      (1000)        1 2022-06-22 19:03:43.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider.egg-info/not-zip-safe
--rw-rw-r--   0 null      (1000) null      (1000)       23 2022-08-02 01:46:10.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider.egg-info/requires.txt
--rw-rw-r--   0 null      (1000) null      (1000)       39 2022-08-02 01:46:10.000000 etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider.egg-info/top_level.txt
--rw-rw-r--   0 null      (1000) null      (1000)      237 2022-06-22 18:48:28.000000 etc_jupyterlab_notebook_state_provider-2.0.9/install.json
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-02 01:46:10.709955 etc_jupyterlab_notebook_state_provider-2.0.9/jupyter-config/
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-02 01:46:10.721955 etc_jupyterlab_notebook_state_provider-2.0.9/jupyter-config/nb-config/
--rw-rw-r--   0 null      (1000) null      (1000)      115 2022-06-22 18:48:28.000000 etc_jupyterlab_notebook_state_provider-2.0.9/jupyter-config/nb-config/etc_jupyterlab_notebook_state_provider.json
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-02 01:46:10.722955 etc_jupyterlab_notebook_state_provider-2.0.9/jupyter-config/server-config/
--rw-rw-r--   0 null      (1000) null      (1000)      113 2022-06-22 18:48:28.000000 etc_jupyterlab_notebook_state_provider-2.0.9/jupyter-config/server-config/etc_jupyterlab_notebook_state_provider.json
--rw-rw-r--   0 null      (1000) null      (1000)     3031 2022-08-02 01:45:35.000000 etc_jupyterlab_notebook_state_provider-2.0.9/package.json
--rw-rw-r--   0 null      (1000) null      (1000)      687 2022-06-22 18:48:28.000000 etc_jupyterlab_notebook_state_provider-2.0.9/pyproject.toml
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-02 01:46:10.722955 etc_jupyterlab_notebook_state_provider-2.0.9/schema/
--rw-rw-r--   0 null      (1000) null      (1000)      298 2022-06-22 18:48:28.000000 etc_jupyterlab_notebook_state_provider-2.0.9/schema/plugin.json
--rw-rw-r--   0 null      (1000) null      (1000)       38 2022-08-02 01:46:10.725955 etc_jupyterlab_notebook_state_provider-2.0.9/setup.cfg
--rw-rw-r--   0 null      (1000) null      (1000)     3203 2022-06-22 18:48:28.000000 etc_jupyterlab_notebook_state_provider-2.0.9/setup.py
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-02 01:46:10.723955 etc_jupyterlab_notebook_state_provider-2.0.9/src/
--rw-rw-r--   0 null      (1000) null      (1000)     1125 2022-06-22 18:48:28.000000 etc_jupyterlab_notebook_state_provider-2.0.9/src/handler.ts
--rw-rw-r--   0 null      (1000) null      (1000)     8104 2022-08-01 20:17:05.000000 etc_jupyterlab_notebook_state_provider-2.0.9/src/index.ts
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-02 01:46:10.724955 etc_jupyterlab_notebook_state_provider-2.0.9/style/
--rw-rw-r--   0 null      (1000) null      (1000)        0 2022-06-22 18:48:28.000000 etc_jupyterlab_notebook_state_provider-2.0.9/style/base.css
--rw-rw-r--   0 null      (1000) null      (1000)       25 2022-06-22 18:48:28.000000 etc_jupyterlab_notebook_state_provider-2.0.9/style/index.css
--rw-rw-r--   0 null      (1000) null      (1000)       21 2022-06-22 18:48:28.000000 etc_jupyterlab_notebook_state_provider-2.0.9/style/index.js
--rw-rw-r--   0 null      (1000) null      (1000)      555 2022-06-24 18:59:59.000000 etc_jupyterlab_notebook_state_provider-2.0.9/tsconfig.json
--rw-rw-r--   0 null      (1000) null      (1000)   277943 2022-07-05 15:34:35.000000 etc_jupyterlab_notebook_state_provider-2.0.9/yarn.lock
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/.copier-answers.yml
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/.eslintignore
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/.eslintrc.js
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/.prettierignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/.prettierrc
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/RELEASE.md
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/install.json
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/setup.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/tsconfig.json
+-rw-r--r--   0        0        0   212366 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/yarn.lock
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/etc_jupyterlab_notebook_state_provider/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/etc_jupyterlab_notebook_state_provider/_version.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/etc_jupyterlab_notebook_state_provider/application.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/etc_jupyterlab_notebook_state_provider/handlers.py
+-rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/etc_jupyterlab_notebook_state_provider/labextension/package.json
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/etc_jupyterlab_notebook_state_provider/labextension/schemas/@educational-technology-collective/etc_jupyterlab_notebook_state_provider/package.json.orig
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/etc_jupyterlab_notebook_state_provider/labextension/schemas/@educational-technology-collective/etc_jupyterlab_notebook_state_provider/plugin.json
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/etc_jupyterlab_notebook_state_provider/labextension/static/747.fbf5d1c729eaf27ebfa6.js
+-rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/etc_jupyterlab_notebook_state_provider/labextension/static/763.542ff0b1b83ea4f89503.js
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/etc_jupyterlab_notebook_state_provider/labextension/static/remoteEntry.ea7dfb4dfe122ee9cd09.js
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/etc_jupyterlab_notebook_state_provider/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/etc_jupyterlab_notebook_state_provider/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/jupyter-config/nb-config/etc_jupyterlab_notebook_state_provider.json
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/jupyter-config/server-config/etc_jupyterlab_notebook_state_provider.json
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/schema/plugin.json
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/src/handler.ts
+-rw-r--r--   0        0        0     7979 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/src/index.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/style/index.js
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/LICENSE
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/README.md
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7898 2020-02-02 00:00:00.000000 etc_jupyterlab_notebook_state_provider-2.1.0/PKG-INFO
```

### Comparing `etc_jupyterlab_notebook_state_provider-2.0.9/LICENSE` & `etc_jupyterlab_notebook_state_provider-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `etc_jupyterlab_notebook_state_provider-2.0.9/PKG-INFO` & `etc_jupyterlab_notebook_state_provider-2.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,59 @@
 Metadata-Version: 2.1
 Name: etc_jupyterlab_notebook_state_provider
-Version: 2.0.9
+Version: 2.1.0
 Summary: A JupyterLab extension.
-Home-page: https://github.com/educational-technology-collective/etc_jupyterlab_notebook_state_provider
+Project-URL: Homepage, https://github.com/educational-technology-collective/etc_jupyterlab_notebook_state_provider
+Project-URL: Bug Tracker, https://github.com/educational-technology-collective/etc_jupyterlab_notebook_state_provider/issues
+Project-URL: Repository, https://github.com/educational-technology-collective/etc_jupyterlab_notebook_state_provider.git
 Author: ETC
-Author-email: 
-License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab,JupyterLab3
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
+License: BSD 3-Clause License
+        
+        Copyright (c) 2021, ETC All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        * Redistributions of source code must retain the above copyright notice, this
+          list of conditions and the following disclaimer.
+        
+        * Redistributions in binary form must reproduce the above copyright notice,
+          this list of conditions and the following disclaimer in the documentation
+          and/or other materials provided with the distribution.
+        
+        * Neither the name of the copyright holder nor the names of its
+          contributors may be used to endorse or promote products derived from
+          this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+License-File: LICENSE
+Classifier: Framework :: Jupyter
+Classifier: Framework :: Jupyter :: JupyterLab
+Classifier: Framework :: Jupyter :: JupyterLab :: 4
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Jupyter
-Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Requires-Dist: jupyter-server<3,>=2.0.1
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # ETC JupyterLab Notebook State Provider
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/educational-technology-collective/etc_jupyterlab_notebook_state_provider/main?urlpath=lab)
 
 
 The ETC JupyterLab Notebook State Provider produces sequential diffs of Notebooks.  Each call to `ETCJupyterLabNotebookStateProvider#getNotebookState` produces a representation of the Notebook where cells that are unchanged since the last call contain just their IDs.  Cells that have not changed since the last call contain their unaltered content.  The diffs can be used in order to reconstruct the Notebook at each point in the sequence.
```

### Comparing `etc_jupyterlab_notebook_state_provider-2.0.9/README.md` & `etc_jupyterlab_notebook_state_provider-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/__init__.py` & `etc_jupyterlab_notebook_state_provider-2.1.0/etc_jupyterlab_notebook_state_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/application.py` & `etc_jupyterlab_notebook_state_provider-2.1.0/etc_jupyterlab_notebook_state_provider/application.py`

 * *Files identical despite different names*

### Comparing `etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/handlers.py` & `etc_jupyterlab_notebook_state_provider-2.1.0/etc_jupyterlab_notebook_state_provider/handlers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tornado
 import json
 from jupyter_server.base.handlers import JupyterHandler
 from jupyter_server.extension.handler import ExtensionHandlerMixin
-from ._version import _fetchVersion
+from ._version import VERSION
 
 class RouteHandler(ExtensionHandlerMixin, JupyterHandler):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     # The following decorator should be present on all verb methods (head, get, post,
@@ -15,15 +15,15 @@
     @tornado.web.authenticated
     def get(self, resource):
 
         try:
             self.set_header('Content-Type', 'application/json')
             
             if resource == 'version':
-                self.finish(json.dumps(_fetchVersion()))
+                self.finish(json.dumps(VERSION))
             elif resource == 'config':
                 self.finish(json.dumps(self.config))
             else:
                 self.set_status(404)
 
         except Exception as e:
             self.set_status(500)
```

### Comparing `etc_jupyterlab_notebook_state_provider-2.0.9/etc_jupyterlab_notebook_state_provider/labextension/package.json` & `etc_jupyterlab_notebook_state_provider-2.1.0/package.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.919404761904762%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.2', '@jupyterlab/coreutils': '^6.0.2', "*

 * *                   "'@jupyterlab/notebook': '^4.0.2', '@jupyterlab/services': '^7.0.2', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.2'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@typescript-eslint/eslint-plugin': "*

 * *                      "'^5.55.0', '@typescript-eslint/parser': '^5.55.0', 'eslint': '^8.36.0', "*

 * *                      "'eslint-config-prettier': '^8.8.0', 'eslint-plugi […]*

```diff
@@ -3,54 +3,60 @@
         "email": "",
         "name": "ETC"
     },
     "bugs": {
         "url": "https://github.com/educational-technology-collective/etc_jupyterlab_notebook_state_provider/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0",
-        "@jupyterlab/coreutils": "^5.1.0",
-        "@jupyterlab/notebook": "^3.0.9",
-        "@jupyterlab/services": "^6.1.0",
-        "@jupyterlab/settingregistry": "^3.1.0"
+        "@jupyterlab/application": "^4.0.2",
+        "@jupyterlab/coreutils": "^6.0.2",
+        "@jupyterlab/notebook": "^4.0.2",
+        "@jupyterlab/services": "^7.0.2",
+        "@jupyterlab/settingregistry": "^4.0.2"
     },
     "description": "A JupyterLab extension.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.1.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.15.0",
-        "eslint-plugin-prettier": "^3.1.4",
+        "@jupyterlab/builder": "^4.0.0",
+        "@types/json-schema": "^7.0.11",
+        "@types/react": "^18.0.26",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-prettier": "^5.0.0",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "typescript": "~4.1.3"
+        "prettier": "^3.0.0",
+        "rimraf": "^4.4.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^15.10.1",
+        "stylelint-config-recommended": "^13.0.0",
+        "stylelint-config-standard": "^34.0.0",
+        "stylelint-prettier": "^4.0.0",
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.40"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
-        "schema/*.json"
+        "schema/*.json",
+        "style/index.js"
     ],
     "homepage": "https://github.com/educational-technology-collective/etc_jupyterlab_notebook_state_provider",
     "jupyter-releaser": {
         "hooks": {
             "before-build-npm": [
                 "python -m pip install jupyterlab~=3.1",
                 "jlpm"
             ]
         }
     },
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.e2d4f614a13c9a73d829.js",
-            "style": "./style"
-        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "etc_jupyterlab_notebook_state_provider"
                 },
                 "managers": [
                     "pip"
@@ -70,32 +76,41 @@
     "main": "lib/index.js",
     "name": "@educational-technology-collective/etc_jupyterlab_notebook_state_provider",
     "repository": {
         "type": "git",
         "url": "https://github.com/educational-technology-collective/etc_jupyterlab_notebook_state_provider.git"
     },
     "scripts": {
-        "build": "jlpm run build:lib && jlpm run build:labextension:dev",
+        "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
-        "build:lib": "tsc",
-        "build:prod": "jlpm run clean && jlpm run build:lib && jlpm run build:labextension",
-        "clean": "jlpm run clean:lib",
-        "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
-        "clean:labextension": "rimraf etc_jupyterlab_notebook_state_provider/labextension",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
+        "clean": "jlpm clean:lib",
+        "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
+        "clean:labextension": "rimraf etc_jupyterlab_notebook_state_provider/labextension etc_jupyterlab_notebook_state_provider/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "eslint": "eslint . --ext .ts,.tsx --fix",
-        "eslint:check": "eslint . --ext .ts,.tsx",
-        "install:extension": "jlpm run build",
+        "clean:lintcache": "rimraf .eslintcache .stylelintcache",
+        "eslint": "jlpm eslint:check --fix",
+        "eslint:check": "eslint . --cache --ext .ts,.tsx",
+        "install:extension": "jlpm build",
+        "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
+        "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
+        "prettier": "jlpm prettier:base --write --list-different",
+        "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
+        "prettier:check": "jlpm prettier:base --check",
+        "stylelint": "jlpm stylelint:check --fix",
+        "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "tsc -w --sourceMap"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.0.9"
+    "version": "2.1.0"
 }
```

### Comparing `etc_jupyterlab_notebook_state_provider-2.0.9/src/handler.ts` & `etc_jupyterlab_notebook_state_provider-2.1.0/src/handler.ts`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'etc-jupyterlab-notebook-state-provider', // API Namespace
     endPoint
   );
 
   let response: Response;
   try {
     response = await ServerConnection.makeRequest(requestUrl, init, settings);
-  } catch (error) {
+  } catch (error: any) {
     throw new ServerConnection.NetworkError(error);
   }
 
   let data: any = await response.text();
 
   if (data.length > 0) {
     try {
```

### Comparing `etc_jupyterlab_notebook_state_provider-2.0.9/src/index.ts` & `etc_jupyterlab_notebook_state_provider-2.1.0/src/index.ts`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,25 @@
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 
 import {
   NotebookPanel,
-  Notebook
+  Notebook,
+  CellList
 } from '@jupyterlab/notebook';
 
 import {
   Cell,
   CodeCell,
   ICellModel
 } from '@jupyterlab/cells';
 
-import {
-  IObservableList,
-  IObservableUndoableList,
-  IObservableString
-} from '@jupyterlab/observables';
+import { IObservableList } from '@jupyterlab/observables';
 
 import { IOutputAreaModel } from '@jupyterlab/outputarea';
 
 import { INotebookContent } from '@jupyterlab/nbformat';
 
 import { UUID, Token } from '@lumino/coreutils';
 
@@ -56,15 +53,15 @@
 
       await notebookPanel.revealed;
 
       this.updateCellState();
       //  The notebook loaded; hence, update the cell state.
 
       notebookPanel.content.model?.cells.changed.connect((
-        sender: IObservableUndoableList<ICellModel>,
+        sender: CellList,
         args: IObservableList.IChangedArgs<ICellModel>
       ) => {
 
           this.updateCellState();
           //  A cell event happened; hence, update the cell state.
       }, this);
     })();
@@ -76,16 +73,16 @@
 
       if (!this._cellState.has(cell)) {
 
         this._cellState.set(cell, { changed: true, output: this.createCellOutput(cell) });
         //  It's a new cell; hence, the changed state is set to true.
 
         ////  This is a new cell; hence, add handlers that check for changes in the inputs and outputs.
-        cell.inputArea.model.value.changed.connect(
-          (sender: IObservableString, args: IObservableString.IChangedArgs) => {
+        cell.inputArea?.model.mimeTypeChanged.connect(
+          () => {
             let state = this._cellState.get(cell);
             if (state !== undefined) {
               state.changed = true;
               //  The input area changed; hence, the changed state is set to true.
             }
           });
```

### Comparing `etc_jupyterlab_notebook_state_provider-2.0.9/tsconfig.json` & `etc_jupyterlab_notebook_state_provider-2.1.0/tsconfig.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993421052631579%*

 * *Differences: {"'compilerOptions'": "{'target': 'ES2018'}"}*

```diff
@@ -13,14 +13,14 @@
         "noUnusedLocals": false,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
         "strictNullChecks": true,
-        "target": "es2017",
+        "target": "ES2018",
         "types": []
     },
     "include": [
         "src/*"
     ]
 }
```

