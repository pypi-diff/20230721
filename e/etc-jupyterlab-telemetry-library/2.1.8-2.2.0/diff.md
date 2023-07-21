# Comparing `tmp/etc_jupyterlab_telemetry_library-2.1.8.tar.gz` & `tmp/etc_jupyterlab_telemetry_library-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etc_jupyterlab_telemetry_library-2.1.8.tar", last modified: Tue Aug 23 14:46:02 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `etc_jupyterlab_telemetry_library-2.1.8.tar` & `etc_jupyterlab_telemetry_library-2.2.0.tar`

### file list

```diff
@@ -1,59 +1,43 @@
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-23 14:46:02.427557 etc_jupyterlab_telemetry_library-2.1.8/
--rw-rw-r--   0 null      (1000) null      (1000)     1503 2022-06-27 14:50:13.000000 etc_jupyterlab_telemetry_library-2.1.8/LICENSE
--rw-rw-r--   0 null      (1000) null      (1000)      503 2022-06-27 14:50:13.000000 etc_jupyterlab_telemetry_library-2.1.8/MANIFEST.in
--rw-rw-r--   0 null      (1000) null      (1000)    14041 2022-08-23 14:46:02.427557 etc_jupyterlab_telemetry_library-2.1.8/PKG-INFO
--rw-rw-r--   0 null      (1000) null      (1000)    12998 2022-08-01 20:01:03.000000 etc_jupyterlab_telemetry_library-2.1.8/README.md
--rw-rw-r--   0 null      (1000) null      (1000)     1916 2022-06-27 14:50:13.000000 etc_jupyterlab_telemetry_library-2.1.8/RELEASE.md
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-23 14:46:02.407557 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/
--rw-rw-r--   0 null      (1000) null      (1000)      634 2022-06-27 14:50:13.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/__init__.py
--rw-rw-r--   0 null      (1000) null      (1000)      440 2022-06-27 14:50:13.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/_version.py
--rw-rw-r--   0 null      (1000) null      (1000)     1335 2022-07-05 16:54:25.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/application.py
--rw-rw-r--   0 null      (1000) null      (1000)     1163 2022-07-05 15:23:16.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/handlers.py
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-23 14:46:02.411557 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/
--rw-rw-r--   0 null      (1000) null      (1000)    22141 2022-08-23 14:45:43.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/build_log.json
--rw-rw-r--   0 null      (1000) null      (1000)     3624 2022-08-23 14:45:43.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/package.json
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-23 14:46:02.402557 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/schemas/
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-23 14:46:02.402557 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/schemas/@educational-technology-collective/
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-23 14:46:02.413557 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/schemas/@educational-technology-collective/etc_jupyterlab_telemetry_library/
--rw-rw-r--   0 null      (1000) null      (1000)     3482 2022-08-23 14:45:43.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/schemas/@educational-technology-collective/etc_jupyterlab_telemetry_library/package.json.orig
--rw-rw-r--   0 null      (1000) null      (1000)      286 2022-08-23 14:45:43.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/schemas/@educational-technology-collective/etc_jupyterlab_telemetry_library/plugin.json
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-23 14:46:02.422557 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/static/
--rw-rw-r--   0 null      (1000) null      (1000)    33228 2022-08-23 14:45:43.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/static/lib_index_js.969da09a6a07272b33b5.js
--rw-rw-r--   0 null      (1000) null      (1000)    32095 2022-08-23 14:45:43.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/static/lib_index_js.969da09a6a07272b33b5.js.map
--rw-rw-r--   0 null      (1000) null      (1000)    29280 2022-08-23 14:45:43.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/static/remoteEntry.87528f3d41d835f4fc03.js
--rw-rw-r--   0 null      (1000) null      (1000)    28879 2022-08-23 14:45:43.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/static/remoteEntry.87528f3d41d835f4fc03.js.map
--rw-rw-r--   0 null      (1000) null      (1000)      210 2022-08-23 14:45:43.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/static/style.js
--rw-rw-r--   0 null      (1000) null      (1000)     4358 2022-08-23 14:45:43.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/static/style_index_js.a404980115044a488230.js
--rw-rw-r--   0 null      (1000) null      (1000)     1573 2022-08-23 14:45:43.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/static/style_index_js.a404980115044a488230.js.map
--rw-rw-r--   0 null      (1000) null      (1000)    12164 2022-08-23 14:45:43.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8b0e18ea8b0e5765847a.js
--rw-rw-r--   0 null      (1000) null      (1000)    13949 2022-08-23 14:45:43.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8b0e18ea8b0e5765847a.js.map
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-23 14:46:02.408557 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library.egg-info/
--rw-rw-r--   0 null      (1000) null      (1000)    14041 2022-08-23 14:46:02.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library.egg-info/PKG-INFO
--rw-rw-r--   0 null      (1000) null      (1000)     2252 2022-08-23 14:46:02.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library.egg-info/SOURCES.txt
--rw-rw-r--   0 null      (1000) null      (1000)        1 2022-08-23 14:46:02.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library.egg-info/dependency_links.txt
--rw-rw-r--   0 null      (1000) null      (1000)        1 2022-06-27 15:38:18.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library.egg-info/not-zip-safe
--rw-rw-r--   0 null      (1000) null      (1000)       72 2022-08-23 14:46:02.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library.egg-info/requires.txt
--rw-rw-r--   0 null      (1000) null      (1000)       33 2022-08-23 14:46:02.000000 etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library.egg-info/top_level.txt
--rw-rw-r--   0 null      (1000) null      (1000)      225 2022-06-27 14:50:13.000000 etc_jupyterlab_telemetry_library-2.1.8/install.json
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-23 14:46:02.403557 etc_jupyterlab_telemetry_library-2.1.8/jupyter-config/
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-23 14:46:02.423557 etc_jupyterlab_telemetry_library-2.1.8/jupyter-config/nb-config/
--rw-rw-r--   0 null      (1000) null      (1000)      109 2022-06-27 14:50:13.000000 etc_jupyterlab_telemetry_library-2.1.8/jupyter-config/nb-config/etc_jupyterlab_telemetry_library.json
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-23 14:46:02.423557 etc_jupyterlab_telemetry_library-2.1.8/jupyter-config/server-config/
--rw-rw-r--   0 null      (1000) null      (1000)      107 2022-06-27 14:50:13.000000 etc_jupyterlab_telemetry_library-2.1.8/jupyter-config/server-config/etc_jupyterlab_telemetry_library.json
--rw-rw-r--   0 null      (1000) null      (1000)     3482 2022-08-23 14:45:36.000000 etc_jupyterlab_telemetry_library-2.1.8/package.json
--rw-rw-r--   0 null      (1000) null      (1000)      663 2022-06-27 14:50:13.000000 etc_jupyterlab_telemetry_library-2.1.8/pyproject.toml
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-23 14:46:02.424557 etc_jupyterlab_telemetry_library-2.1.8/schema/
--rw-rw-r--   0 null      (1000) null      (1000)      286 2022-06-27 14:50:13.000000 etc_jupyterlab_telemetry_library-2.1.8/schema/plugin.json
--rw-rw-r--   0 null      (1000) null      (1000)       38 2022-08-23 14:46:02.427557 etc_jupyterlab_telemetry_library-2.1.8/setup.cfg
--rw-rw-r--   0 null      (1000) null      (1000)     3234 2022-06-27 14:50:13.000000 etc_jupyterlab_telemetry_library-2.1.8/setup.py
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-23 14:46:02.425557 etc_jupyterlab_telemetry_library-2.1.8/src/
--rw-rw-r--   0 null      (1000) null      (1000)     1119 2022-06-27 14:50:13.000000 etc_jupyterlab_telemetry_library-2.1.8/src/handler.ts
--rw-rw-r--   0 null      (1000) null      (1000)     4500 2022-08-05 16:46:39.000000 etc_jupyterlab_telemetry_library-2.1.8/src/index.ts
--rw-rw-r--   0 null      (1000) null      (1000)    25570 2022-08-02 01:07:36.000000 etc_jupyterlab_telemetry_library-2.1.8/src/library.ts
--rw-rw-r--   0 null      (1000) null      (1000)      948 2022-08-23 14:39:15.000000 etc_jupyterlab_telemetry_library-2.1.8/src/types.ts
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-08-23 14:46:02.426557 etc_jupyterlab_telemetry_library-2.1.8/style/
--rw-rw-r--   0 null      (1000) null      (1000)        0 2022-06-27 14:50:13.000000 etc_jupyterlab_telemetry_library-2.1.8/style/base.css
--rw-rw-r--   0 null      (1000) null      (1000)       25 2022-06-27 14:50:13.000000 etc_jupyterlab_telemetry_library-2.1.8/style/index.css
--rw-rw-r--   0 null      (1000) null      (1000)       21 2022-06-27 14:50:13.000000 etc_jupyterlab_telemetry_library-2.1.8/style/index.js
--rw-rw-r--   0 null      (1000) null      (1000)      555 2022-06-27 14:50:13.000000 etc_jupyterlab_telemetry_library-2.1.8/tsconfig.json
--rw-rw-r--   0 null      (1000) null      (1000)   278864 2022-07-05 17:13:16.000000 etc_jupyterlab_telemetry_library-2.1.8/yarn.lock
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/.copier-answers.yml
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/.eslintignore
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/.eslintrc.js
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/.prettierignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/.prettierrc
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/RELEASE.md
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/etc_jupyterlab_telemetry_library.json
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/install.json
+-rw-r--r--   0        0        0   670109 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/package-lock.json
+-rw-r--r--   0        0        0     4610 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/tsconfig.json
+-rw-r--r--   0        0        0   218600 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/yarn.lock
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/configuration_example/jupyter_etc_jupyterlab_telemetry_library_config.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/etc_jupyterlab_telemetry_library/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/etc_jupyterlab_telemetry_library/_version.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/etc_jupyterlab_telemetry_library/application.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/etc_jupyterlab_telemetry_library/handlers.py
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/etc_jupyterlab_telemetry_library/labextension/package.json
+-rw-r--r--   0        0        0     4610 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/etc_jupyterlab_telemetry_library/labextension/schemas/@educational-technology-collective/etc_jupyterlab_telemetry_library/package.json.orig
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/etc_jupyterlab_telemetry_library/labextension/schemas/@educational-technology-collective/etc_jupyterlab_telemetry_library/plugin.json
+-rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/etc_jupyterlab_telemetry_library/labextension/static/747.d3c939ccdb588e1b8370.js
+-rw-r--r--   0        0        0    12491 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/etc_jupyterlab_telemetry_library/labextension/static/799.d0740fa6889ffa3ac8ca.js
+-rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/etc_jupyterlab_telemetry_library/labextension/static/remoteEntry.fb26a52f062bfbd4034e.js
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/etc_jupyterlab_telemetry_library/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/etc_jupyterlab_telemetry_library/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/jupyter-config/nb-config/etc_jupyterlab_telemetry_library.json
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/jupyter-config/server-config/etc_jupyterlab_telemetry_library.json
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/schema/plugin.json
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/src/handler.ts
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/src/index.ts
+-rw-r--r--   0        0        0    25426 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/src/library.ts
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/src/types.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/style/index.js
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/.gitignore
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/LICENSE
+-rw-r--r--   0        0        0    13143 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/README.md
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0    16071 2020-02-02 00:00:00.000000 etc_jupyterlab_telemetry_library-2.2.0/PKG-INFO
```

### Comparing `etc_jupyterlab_telemetry_library-2.1.8/LICENSE` & `etc_jupyterlab_telemetry_library-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `etc_jupyterlab_telemetry_library-2.1.8/PKG-INFO` & `etc_jupyterlab_telemetry_library-2.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,19 @@
-Metadata-Version: 2.1
-Name: etc_jupyterlab_telemetry_library
-Version: 2.1.8
-Summary: A JupyterLab extension.
-Home-page: https://github.com/educational-technology-collective/etc_jupyterlab_telemetry_library
-Author: ETC
-Author-email: 
-License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab,JupyterLab3
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Jupyter
-Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# Introduction
 
-# ETC JupyterLab Telemetry Library
+This extension provides a factory that produces an object that implements an interface that consists of grouped Lumino [Signals](#signals) that can be used in order to capture telemetry events.
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/educational-technology-collective/etc_jupyterlab_telemetry_library/main?urlpath=lab)
+This extension is not intended to operate on its own.  This extension should be consumed by a [Consumer](https://jupyterlab.readthedocs.io/en/stable/extension/extension_dev.html?highlight=consumer#tokens) extension that filters, modifies, and records the messages produced by this extension as required for the given application. Please see the [ETC JupyterLab Telemetry Coursera](https://github.com/educational-technology-collective/etc_jupyterlab_telemetry_coursera) extension for an example of how to consume this extension and log the messages produced by it.
 
-This extension provides a JupyterLab service, identified by the `IETCJupyterLabTelemetryLibraryFactory` token, that can be used to construct a `ETCJupyterLabTelemetryLibrary` instance that exposes Signals associated with user actions in the Notebook.
+# Signals
 
-The `IETCJupyterLabTelemetryLibraryFactory` Token represents a **service** that can be consumed by a JupyterLab plugin similar to how core services are consumed by plugins: [Core Tokens](https://jupyterlab.readthedocs.io/en/stable/extension/extension_points.html#core-tokens). See the [Usage](#usage) section for instructions on how to consume the service.
-
-The ETCJupyterLabTelemetryLibrary service contains Signals grouped according to their functionality. For example in order to `console.log` the `notebook_open` event, you would connect to the Signal like this:
+This extension consists of "Signal Groups" and their respective Signals.  A Signal Group is a means of grouping Signals that are either related or that have shared dependencies.  Accessing a Signal is done through its respective group; for example, once you have instantiated a `ETCJupyterLabTelemetryLibrary` instance you can access the `notebookVisible` Signal through the `notebookVisibilityEvent` Signal Group. For example:
 
 ```js
-etcJupyterLabTelemetryLibrary.notebookOpenEvent.notebookOpened.connect(
-  console.log
-);
+etcJupyterLabTelemetryLibrary.notebookVisibilityEvent.notebookVisible.connect(messageAdapter.log)
 ```
 
 The following table provides the Signal Groups and their respective Signal(s).
 
 | Signal Group            | Signal(s)                                                              |
 | ----------------------- | ---------------------------------------------------------------------- |
 | notebookClipboardEvent  | notebookClipboardCopied, notebookClipboardCut, notebookClipboardPasted |
@@ -56,29 +26,25 @@
 | cellAddEvent            | cellAdded                                                              |
 | cellRemoveEvent         | cellRemoved                                                            |
 | cellExecutionEvent      | cellExecuted                                                           |
 | cellErrorEvent          | cellErrored                                                            |
 
 A plugin that consumes this plugin can attach a handler to the Signal(s) of each Signal Group in order to log the event message.
 
-## Events
+## Event Messages
 
 Each event message (i.e., the message emitted by the Signal) contains a list of cells relevant to that event. See the [Relevant Cells](#relevant-cells) section for details.
 
-## Event Message Schema
+### Event Message Schema
 
 Each event message will contain the name of the event, a list of cells that are relevant to the event, and a reference to the NotebookPanel that emitted the event.
 
-Each event message conforms to the following JSON schema.
-
-### TO DO
-
-## Relevant Cells
+### Relevant Cells
 
-For each event message, in addition to reference to the complete NotebookPanel, which contains the full contents of each cell, the top level `cells` property in the message will contain the cells relevant to the event.
+For each event message, in addition to a reference to the complete NotebookPanel, which contains the full contents of each cell, the top level `cells` property in the message will contain the cells relevant to the event.
 
 
 | Signal(s)                                                              | Relevant Cells |
 | ---------------------------------------------------------------------- | ---------------|
 | notebookClipboardCopied, notebookClipboardCut, notebookClipboardPasted | The cell list contains the ID of the active cell. |
 | notebookVisible, notebookHidden                                        | The cell list contains the IDs of the cells that are visible to the user. |
 | notebookClosed                                                         | The cell list contains the IDs of all the cells in the notebook. |
@@ -87,23 +53,25 @@
 | notebookScrolled                                                       | The cell list contains the IDs of the cells that are visible to the user. |
 | activeCellChanged                                                      | The cell list contains the ID of the active cell. |
 | cellAdded                                                              | The cell list contains the IDs of the added cells. |
 | cellRemoved                                                            | The cell list contains the IDs of the removed cells. |
 | cellExecuted                                                           | The cell list contains the ID of the executed cell. |
 | cellErrored                                                            | The cell list contains the ID of the cell that produced the error. |
 
-## Usage
+# Usage
 
-Install the extension according to the installation instructions.
+This extension provides a factory service, identified by the `IETCJupyterLabTelemetryLibraryFactory` token, that can be used to construct a `ETCJupyterLabTelemetryLibrary` instance that exposes Signals associated with user actions in the Notebook.
 
-Once the extension is installed a plugin can consume the service by including it in its `requires` list. See the below code for an example.
+The `IETCJupyterLabTelemetryLibraryFactory` Token represents a **service** that can be consumed by a JupyterLab plugin similar to how core services are consumed by plugins: [Core Tokens](https://jupyterlab.readthedocs.io/en/stable/extension/extension_points.html#core-tokens). See the [Usage](#usage) section for instructions on how to consume the service.
+
+Install the extension according to the [installation](#install) instructions.  Once the extension is installed a plugin can consume the service by including it in its `requires` list. See the below code for an example.
 
-The extension provides a service identified by the `IETCJupyterLabTelemetryLibraryFactory` token. In the following example, the `consumer` plugin consumes the Token provided by the `etc_jupyterlab_telemetry_library` extension. The `ETCJupyterLabTelemetryLibraryFactory` is used in order to instantiate a `ETCJupyterLabTelemetryLibrary` for each NotebookPanel. Each `ETCJupyterLabTelemetryLibrary` instance contains grouped Signals that are connected to the `console.log` method, which will log the events to the console.
+In the example below, the extension provides a service identified by the `IETCJupyterLabTelemetryLibraryFactory` token. The `consumer` plugin consumes the Token provided by the `etc_jupyterlab_telemetry_library` extension. The `ETCJupyterLabTelemetryLibraryFactory` is used in order to instantiate a `ETCJupyterLabTelemetryLibrary` for each NotebookPanel. Each `ETCJupyterLabTelemetryLibrary` instance contains grouped Signals that are connected to the `console.log` method, which will log the events to the console.
 
-The Signals can be connected to any handler that you choose. The content of the messages can be filtered according to your needs.
+The Signals can be connected to the handler of your choice. The content of the messages can be filtered according to your needs.
 
 ```js
 const plugin: JupyterFrontEndPlugin<void> = {
   id: PLUGIN_ID,
   autoStart: true,
   requires: [INotebookTracker, IETCJupyterLabTelemetryLibraryFactory],
   activate: (
@@ -177,15 +145,15 @@
         console.error(e);
       }
     })();
   }
 };
 ```
 
-## Configuration
+# Configuration
 
 The extension requires a configuration file that specifies which Signal _groups_ will emit events.
 
 The configuration file may be placed in any of the Jupyter Server configuration directories e.g., `/etc/jupyter`. Execute `jupyter --paths` in order to get a list of valid configuration directories. The configuration file must be named `jupyter_etc_jupyterlab_telemetry_coursera_config.py`.
 
 This is an example of a valid configuration file:
 
@@ -199,55 +167,17 @@
 c.ETCJupyterLabTelemetryLibraryApp.notebook_cell_add_event = True
 c.ETCJupyterLabTelemetryLibraryApp.notebook_cell_execution_event = True
 c.ETCJupyterLabTelemetryLibraryApp.notebook_scroll_event = True
 c.ETCJupyterLabTelemetryLibraryApp.notebook_active_cell_change_event = True
 c.ETCJupyterLabTelemetryLibraryApp.notebook_cell_error_event = True
 ```
 
-An Signal group can be enable or disabled by setting the respective property to `True` or `False`. This setting will enable or disable all of the Signals in the respective group.  The change will take effect each time JupyterLab is started.
-
-## Requirements
-
-- JupyterLab >= 3.0
-
-## Install
-
-To install the extension, execute:
-
-```bash
-pip install etc_jupyterlab_telemetry_library
-```
-
-## Uninstall
-
-To remove the extension, execute:
-
-```bash
-pip uninstall etc_jupyterlab_telemetry_library
-```
-
-## Troubleshoot
-
-If you are seeing the frontend extension, but it is not working, check
-that the server extension is enabled:
-
-```bash
-jupyter server extension list
-```
-
-If the server extension is installed and enabled, but you are not seeing
-the frontend extension, check the frontend extension is installed:
-
-```bash
-jupyter labextension list
-```
-
-## Contributing
+A Signal group can be enabled or disabled by setting the respective property to `True` or `False`. This setting will enable or disable all of the Signals in the respective group.  The change will take effect each time the Jupyter Server is started.
 
-### Development install
+# Development Install
 
 Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
@@ -277,22 +207,22 @@
 
 By default, the `jlpm run build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
 
 ```bash
 jupyter lab build --minimize=False
 ```
 
-### Development uninstall
+## Development Uninstall
 
 ```bash
 # Server extension must be manually disabled in develop mode
 jupyter server extension disable etc_jupyterlab_telemetry_library
 pip uninstall etc_jupyterlab_telemetry_library
 ```
 
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `@educational-technology-collective/etc_jupyterlab_telemetry_library` within that folder.
 
-### Packaging the extension
+## Packaging the Extension
 
 See [RELEASE](RELEASE.md)
```

### Comparing `etc_jupyterlab_telemetry_library-2.1.8/README.md` & `etc_jupyterlab_telemetry_library-2.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,72 @@
-# ETC JupyterLab Telemetry Library
+Metadata-Version: 2.1
+Name: etc_jupyterlab_telemetry_library
+Version: 2.2.0
+Summary: A JupyterLab extension.
+Project-URL: Homepage, https://github.com/educational-technology-collective/etc_jupyterlab_telemetry_library
+Project-URL: Bug Tracker, https://github.com/educational-technology-collective/etc_jupyterlab_telemetry_library/issues
+Project-URL: Repository, https://github.com/educational-technology-collective/etc_jupyterlab_telemetry_library.git
+Author: ETC
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
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Requires-Dist: jupyter-server<3,>=2.0.1
+Description-Content-Type: text/markdown
+
+# Introduction
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/educational-technology-collective/etc_jupyterlab_telemetry_library/main?urlpath=lab)
+This extension provides a factory that produces an object that implements an interface that consists of grouped Lumino [Signals](#signals) that can be used in order to capture telemetry events.
 
-This extension provides a JupyterLab service, identified by the `IETCJupyterLabTelemetryLibraryFactory` token, that can be used to construct a `ETCJupyterLabTelemetryLibrary` instance that exposes Signals associated with user actions in the Notebook.
+This extension is not intended to operate on its own.  This extension should be consumed by a [Consumer](https://jupyterlab.readthedocs.io/en/stable/extension/extension_dev.html?highlight=consumer#tokens) extension that filters, modifies, and records the messages produced by this extension as required for the given application. Please see the [ETC JupyterLab Telemetry Coursera](https://github.com/educational-technology-collective/etc_jupyterlab_telemetry_coursera) extension for an example of how to consume this extension and log the messages produced by it.
 
-The `IETCJupyterLabTelemetryLibraryFactory` Token represents a **service** that can be consumed by a JupyterLab plugin similar to how core services are consumed by plugins: [Core Tokens](https://jupyterlab.readthedocs.io/en/stable/extension/extension_points.html#core-tokens). See the [Usage](#usage) section for instructions on how to consume the service.
+# Signals
 
-The ETCJupyterLabTelemetryLibrary service contains Signals grouped according to their functionality. For example in order to `console.log` the `notebook_open` event, you would connect to the Signal like this:
+This extension consists of "Signal Groups" and their respective Signals.  A Signal Group is a means of grouping Signals that are either related or that have shared dependencies.  Accessing a Signal is done through its respective group; for example, once you have instantiated a `ETCJupyterLabTelemetryLibrary` instance you can access the `notebookVisible` Signal through the `notebookVisibilityEvent` Signal Group. For example:
 
 ```js
-etcJupyterLabTelemetryLibrary.notebookOpenEvent.notebookOpened.connect(
-  console.log
-);
+etcJupyterLabTelemetryLibrary.notebookVisibilityEvent.notebookVisible.connect(messageAdapter.log)
 ```
 
 The following table provides the Signal Groups and their respective Signal(s).
 
 | Signal Group            | Signal(s)                                                              |
 | ----------------------- | ---------------------------------------------------------------------- |
 | notebookClipboardEvent  | notebookClipboardCopied, notebookClipboardCut, notebookClipboardPasted |
@@ -28,29 +79,25 @@
 | cellAddEvent            | cellAdded                                                              |
 | cellRemoveEvent         | cellRemoved                                                            |
 | cellExecutionEvent      | cellExecuted                                                           |
 | cellErrorEvent          | cellErrored                                                            |
 
 A plugin that consumes this plugin can attach a handler to the Signal(s) of each Signal Group in order to log the event message.
 
-## Events
+## Event Messages
 
 Each event message (i.e., the message emitted by the Signal) contains a list of cells relevant to that event. See the [Relevant Cells](#relevant-cells) section for details.
 
-## Event Message Schema
+### Event Message Schema
 
 Each event message will contain the name of the event, a list of cells that are relevant to the event, and a reference to the NotebookPanel that emitted the event.
 
-Each event message conforms to the following JSON schema.
-
-### TO DO
+### Relevant Cells
 
-## Relevant Cells
-
-For each event message, in addition to reference to the complete NotebookPanel, which contains the full contents of each cell, the top level `cells` property in the message will contain the cells relevant to the event.
+For each event message, in addition to a reference to the complete NotebookPanel, which contains the full contents of each cell, the top level `cells` property in the message will contain the cells relevant to the event.
 
 
 | Signal(s)                                                              | Relevant Cells |
 | ---------------------------------------------------------------------- | ---------------|
 | notebookClipboardCopied, notebookClipboardCut, notebookClipboardPasted | The cell list contains the ID of the active cell. |
 | notebookVisible, notebookHidden                                        | The cell list contains the IDs of the cells that are visible to the user. |
 | notebookClosed                                                         | The cell list contains the IDs of all the cells in the notebook. |
@@ -59,23 +106,25 @@
 | notebookScrolled                                                       | The cell list contains the IDs of the cells that are visible to the user. |
 | activeCellChanged                                                      | The cell list contains the ID of the active cell. |
 | cellAdded                                                              | The cell list contains the IDs of the added cells. |
 | cellRemoved                                                            | The cell list contains the IDs of the removed cells. |
 | cellExecuted                                                           | The cell list contains the ID of the executed cell. |
 | cellErrored                                                            | The cell list contains the ID of the cell that produced the error. |
 
-## Usage
+# Usage
 
-Install the extension according to the installation instructions.
+This extension provides a factory service, identified by the `IETCJupyterLabTelemetryLibraryFactory` token, that can be used to construct a `ETCJupyterLabTelemetryLibrary` instance that exposes Signals associated with user actions in the Notebook.
 
-Once the extension is installed a plugin can consume the service by including it in its `requires` list. See the below code for an example.
+The `IETCJupyterLabTelemetryLibraryFactory` Token represents a **service** that can be consumed by a JupyterLab plugin similar to how core services are consumed by plugins: [Core Tokens](https://jupyterlab.readthedocs.io/en/stable/extension/extension_points.html#core-tokens). See the [Usage](#usage) section for instructions on how to consume the service.
 
-The extension provides a service identified by the `IETCJupyterLabTelemetryLibraryFactory` token. In the following example, the `consumer` plugin consumes the Token provided by the `etc_jupyterlab_telemetry_library` extension. The `ETCJupyterLabTelemetryLibraryFactory` is used in order to instantiate a `ETCJupyterLabTelemetryLibrary` for each NotebookPanel. Each `ETCJupyterLabTelemetryLibrary` instance contains grouped Signals that are connected to the `console.log` method, which will log the events to the console.
+Install the extension according to the [installation](#install) instructions.  Once the extension is installed a plugin can consume the service by including it in its `requires` list. See the below code for an example.
 
-The Signals can be connected to any handler that you choose. The content of the messages can be filtered according to your needs.
+In the example below, the extension provides a service identified by the `IETCJupyterLabTelemetryLibraryFactory` token. The `consumer` plugin consumes the Token provided by the `etc_jupyterlab_telemetry_library` extension. The `ETCJupyterLabTelemetryLibraryFactory` is used in order to instantiate a `ETCJupyterLabTelemetryLibrary` for each NotebookPanel. Each `ETCJupyterLabTelemetryLibrary` instance contains grouped Signals that are connected to the `console.log` method, which will log the events to the console.
+
+The Signals can be connected to the handler of your choice. The content of the messages can be filtered according to your needs.
 
 ```js
 const plugin: JupyterFrontEndPlugin<void> = {
   id: PLUGIN_ID,
   autoStart: true,
   requires: [INotebookTracker, IETCJupyterLabTelemetryLibraryFactory],
   activate: (
@@ -149,15 +198,15 @@
         console.error(e);
       }
     })();
   }
 };
 ```
 
-## Configuration
+# Configuration
 
 The extension requires a configuration file that specifies which Signal _groups_ will emit events.
 
 The configuration file may be placed in any of the Jupyter Server configuration directories e.g., `/etc/jupyter`. Execute `jupyter --paths` in order to get a list of valid configuration directories. The configuration file must be named `jupyter_etc_jupyterlab_telemetry_coursera_config.py`.
 
 This is an example of a valid configuration file:
 
@@ -171,55 +220,17 @@
 c.ETCJupyterLabTelemetryLibraryApp.notebook_cell_add_event = True
 c.ETCJupyterLabTelemetryLibraryApp.notebook_cell_execution_event = True
 c.ETCJupyterLabTelemetryLibraryApp.notebook_scroll_event = True
 c.ETCJupyterLabTelemetryLibraryApp.notebook_active_cell_change_event = True
 c.ETCJupyterLabTelemetryLibraryApp.notebook_cell_error_event = True
 ```
 
-An Signal group can be enable or disabled by setting the respective property to `True` or `False`. This setting will enable or disable all of the Signals in the respective group.  The change will take effect each time JupyterLab is started.
-
-## Requirements
-
-- JupyterLab >= 3.0
-
-## Install
-
-To install the extension, execute:
-
-```bash
-pip install etc_jupyterlab_telemetry_library
-```
-
-## Uninstall
-
-To remove the extension, execute:
-
-```bash
-pip uninstall etc_jupyterlab_telemetry_library
-```
-
-## Troubleshoot
-
-If you are seeing the frontend extension, but it is not working, check
-that the server extension is enabled:
-
-```bash
-jupyter server extension list
-```
-
-If the server extension is installed and enabled, but you are not seeing
-the frontend extension, check the frontend extension is installed:
-
-```bash
-jupyter labextension list
-```
-
-## Contributing
+A Signal group can be enabled or disabled by setting the respective property to `True` or `False`. This setting will enable or disable all of the Signals in the respective group.  The change will take effect each time the Jupyter Server is started.
 
-### Development install
+# Development Install
 
 Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
@@ -249,22 +260,22 @@
 
 By default, the `jlpm run build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
 
 ```bash
 jupyter lab build --minimize=False
 ```
 
-### Development uninstall
+## Development Uninstall
 
 ```bash
 # Server extension must be manually disabled in develop mode
 jupyter server extension disable etc_jupyterlab_telemetry_library
 pip uninstall etc_jupyterlab_telemetry_library
 ```
 
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `@educational-technology-collective/etc_jupyterlab_telemetry_library` within that folder.
 
-### Packaging the extension
+## Packaging the Extension
 
 See [RELEASE](RELEASE.md)
```

### Comparing `etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/__init__.py` & `etc_jupyterlab_telemetry_library-2.2.0/etc_jupyterlab_telemetry_library/__init__.py`

 * *Files identical despite different names*

### Comparing `etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/application.py` & `etc_jupyterlab_telemetry_library-2.2.0/etc_jupyterlab_telemetry_library/application.py`

 * *Files identical despite different names*

### Comparing `etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/handlers.py` & `etc_jupyterlab_telemetry_library-2.2.0/etc_jupyterlab_telemetry_library/handlers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import tornado
 import json
 from jupyter_server.base.handlers import JupyterHandler
 from jupyter_server.extension.handler import ExtensionHandlerMixin
 import pprint
-from ._version import _fetchVersion
+from ._version import VERSION
 
 class RouteHandler(ExtensionHandlerMixin, JupyterHandler):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     # The following decorator should be present on all verb methods (head, get, post,
@@ -17,15 +17,15 @@
     @tornado.web.authenticated
     def get(self, resource):
 
         try:
             self.set_header('Content-Type', 'application/json')
             
             if resource == 'version':
-                self.finish(json.dumps(_fetchVersion()))
+                self.finish(json.dumps(VERSION))
             elif resource == 'config':
                 self.finish(json.dumps(self.config))
             elif resource == 'environ':
                 self.finish(json.dumps({k:v for k, v in os.environ.items()}))
             else:
                 self.set_status(404)
```

### Comparing `etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/package.json` & `etc_jupyterlab_telemetry_library-2.2.0/package.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9149350649350649%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.2', '@jupyterlab/coreutils': '^6.0.2', "*

 * *                   "'@jupyterlab/docregistry': '^4.0.2', '@jupyterlab/nbformat': '^4.0.2', "*

 * *                   "'@jupyterlab/notebook': '^4.0.2', '@jupyterlab/observables': '^5.0.2', "*

 * *                   "'@jupyterlab/outputarea': '^4.0.2', '@jupyterlab/services': '^7.0.2', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.2', '@lumino/signaling': '^2.0.0', "*

 * *                   'delete: '*

 * *                […]*

```diff
@@ -3,112 +3,119 @@
         "email": "",
         "name": "ETC"
     },
     "bugs": {
         "url": "https://github.com/educational-technology-collective/etc_jupyterlab_telemetry_library/issues"
     },
     "dependencies": {
-        "@educational-technology-collective/etc_jupyterlab_notebook_state_provider": "^2.0.0",
-        "@jupyterlab/application": "^3.0.9",
-        "@jupyterlab/coreutils": "^5.0.5",
-        "@jupyterlab/docregistry": "^3.0.9",
-        "@jupyterlab/nbformat": "^3.0.5",
-        "@jupyterlab/notebook": "^3.0.9",
-        "@jupyterlab/observables": "^4.0.5",
-        "@jupyterlab/outputarea": "^3.0.8",
-        "@jupyterlab/services": "^6.0.7",
-        "@jupyterlab/settingregistry": "^3.0.5",
-        "@lumino/signaling": "^1.4.3"
+        "@jupyterlab/application": "^4.0.2",
+        "@jupyterlab/coreutils": "^6.0.2",
+        "@jupyterlab/docregistry": "^4.0.2",
+        "@jupyterlab/nbformat": "^4.0.2",
+        "@jupyterlab/notebook": "^4.0.2",
+        "@jupyterlab/observables": "^5.0.2",
+        "@jupyterlab/outputarea": "^4.0.2",
+        "@jupyterlab/services": "^7.0.2",
+        "@jupyterlab/settingregistry": "^4.0.2",
+        "@lumino/signaling": "^2.0.0"
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
     "homepage": "https://github.com/educational-technology-collective/etc_jupyterlab_telemetry_library",
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
-            "load": "static/remoteEntry.87528f3d41d835f4fc03.js",
-            "style": "./style"
-        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "etc_jupyterlab_telemetry_library"
                 },
                 "managers": [
                     "pip"
                 ]
             }
         },
         "extension": true,
         "outputDir": "etc_jupyterlab_telemetry_library/labextension",
-        "schemaDir": "schema",
-        "sharedPackages": {
-            "@educational-technology-collective/etc_jupyterlab_notebook_state_provider": {
-                "bundled": false,
-                "singleton": true,
-                "strictVersion": true
-            }
-        }
+        "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "@educational-technology-collective/etc_jupyterlab_telemetry_library",
     "repository": {
         "type": "git",
         "url": "https://github.com/educational-technology-collective/etc_jupyterlab_telemetry_library.git"
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
-        "clean:labextension": "rimraf etc_jupyterlab_telemetry_library/labextension",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
+        "clean": "jlpm clean:lib",
+        "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
+        "clean:labextension": "rimraf etc_jupyterlab_telemetry_library/labextension etc_jupyterlab_telemetry_library/_version.py",
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
-    "version": "2.1.8"
+    "version": "2.2.0"
 }
```

### Comparing `etc_jupyterlab_telemetry_library-2.1.8/etc_jupyterlab_telemetry_library/labextension/schemas/@educational-technology-collective/etc_jupyterlab_telemetry_library/package.json.orig` & `etc_jupyterlab_telemetry_library-2.2.0/etc_jupyterlab_telemetry_library/labextension/schemas/@educational-technology-collective/etc_jupyterlab_telemetry_library/package.json.orig`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9182683982683983%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.2', '@jupyterlab/coreutils': '^6.0.2', "*

 * *                   "'@jupyterlab/docregistry': '^4.0.2', '@jupyterlab/nbformat': '^4.0.2', "*

 * *                   "'@jupyterlab/notebook': '^4.0.2', '@jupyterlab/observables': '^5.0.2', "*

 * *                   "'@jupyterlab/outputarea': '^4.0.2', '@jupyterlab/services': '^7.0.2', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.2', '@lumino/signaling': '^2.0.0', "*

 * *                   'delete: '*

 * *                […]*

```diff
@@ -3,44 +3,54 @@
         "email": "",
         "name": "ETC"
     },
     "bugs": {
         "url": "https://github.com/educational-technology-collective/etc_jupyterlab_telemetry_library/issues"
     },
     "dependencies": {
-        "@educational-technology-collective/etc_jupyterlab_notebook_state_provider": "^2.0.0",
-        "@jupyterlab/application": "^3.0.9",
-        "@jupyterlab/coreutils": "^5.0.5",
-        "@jupyterlab/docregistry": "^3.0.9",
-        "@jupyterlab/nbformat": "^3.0.5",
-        "@jupyterlab/notebook": "^3.0.9",
-        "@jupyterlab/observables": "^4.0.5",
-        "@jupyterlab/outputarea": "^3.0.8",
-        "@jupyterlab/services": "^6.0.7",
-        "@jupyterlab/settingregistry": "^3.0.5",
-        "@lumino/signaling": "^1.4.3"
+        "@jupyterlab/application": "^4.0.2",
+        "@jupyterlab/coreutils": "^6.0.2",
+        "@jupyterlab/docregistry": "^4.0.2",
+        "@jupyterlab/nbformat": "^4.0.2",
+        "@jupyterlab/notebook": "^4.0.2",
+        "@jupyterlab/observables": "^5.0.2",
+        "@jupyterlab/outputarea": "^4.0.2",
+        "@jupyterlab/services": "^7.0.2",
+        "@jupyterlab/settingregistry": "^4.0.2",
+        "@lumino/signaling": "^2.0.0"
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
     "homepage": "https://github.com/educational-technology-collective/etc_jupyterlab_telemetry_library",
     "jupyter-releaser": {
         "hooks": {
             "before-build-npm": [
                 "python -m pip install jupyterlab~=3.1",
                 "jlpm"
@@ -56,54 +66,56 @@
                 "managers": [
                     "pip"
                 ]
             }
         },
         "extension": true,
         "outputDir": "etc_jupyterlab_telemetry_library/labextension",
-        "schemaDir": "schema",
-        "sharedPackages": {
-            "@educational-technology-collective/etc_jupyterlab_notebook_state_provider": {
-                "bundled": false,
-                "singleton": true,
-                "strictVersion": true
-            }
-        }
+        "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "@educational-technology-collective/etc_jupyterlab_telemetry_library",
     "repository": {
         "type": "git",
         "url": "https://github.com/educational-technology-collective/etc_jupyterlab_telemetry_library.git"
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
-        "clean:labextension": "rimraf etc_jupyterlab_telemetry_library/labextension",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
+        "clean": "jlpm clean:lib",
+        "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
+        "clean:labextension": "rimraf etc_jupyterlab_telemetry_library/labextension etc_jupyterlab_telemetry_library/_version.py",
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
-    "version": "2.1.8"
+    "version": "2.2.0"
 }
```

### Comparing `etc_jupyterlab_telemetry_library-2.1.8/package.json` & `etc_jupyterlab_telemetry_library-2.2.0/etc_jupyterlab_telemetry_library/labextension/package.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9149350649350649%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.2', '@jupyterlab/coreutils': '^6.0.2', "*

 * *                   "'@jupyterlab/docregistry': '^4.0.2', '@jupyterlab/nbformat': '^4.0.2', "*

 * *                   "'@jupyterlab/notebook': '^4.0.2', '@jupyterlab/observables': '^5.0.2', "*

 * *                   "'@jupyterlab/outputarea': '^4.0.2', '@jupyterlab/services': '^7.0.2', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.2', '@lumino/signaling': '^2.0.0', "*

 * *                   'delete: '*

 * *                […]*

```diff
@@ -3,107 +3,124 @@
         "email": "",
         "name": "ETC"
     },
     "bugs": {
         "url": "https://github.com/educational-technology-collective/etc_jupyterlab_telemetry_library/issues"
     },
     "dependencies": {
-        "@educational-technology-collective/etc_jupyterlab_notebook_state_provider": "^2.0.0",
-        "@jupyterlab/application": "^3.0.9",
-        "@jupyterlab/coreutils": "^5.0.5",
-        "@jupyterlab/docregistry": "^3.0.9",
-        "@jupyterlab/nbformat": "^3.0.5",
-        "@jupyterlab/notebook": "^3.0.9",
-        "@jupyterlab/observables": "^4.0.5",
-        "@jupyterlab/outputarea": "^3.0.8",
-        "@jupyterlab/services": "^6.0.7",
-        "@jupyterlab/settingregistry": "^3.0.5",
-        "@lumino/signaling": "^1.4.3"
+        "@jupyterlab/application": "^4.0.2",
+        "@jupyterlab/coreutils": "^6.0.2",
+        "@jupyterlab/docregistry": "^4.0.2",
+        "@jupyterlab/nbformat": "^4.0.2",
+        "@jupyterlab/notebook": "^4.0.2",
+        "@jupyterlab/observables": "^5.0.2",
+        "@jupyterlab/outputarea": "^4.0.2",
+        "@jupyterlab/services": "^7.0.2",
+        "@jupyterlab/settingregistry": "^4.0.2",
+        "@lumino/signaling": "^2.0.0"
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
     "homepage": "https://github.com/educational-technology-collective/etc_jupyterlab_telemetry_library",
     "jupyter-releaser": {
         "hooks": {
             "before-build-npm": [
                 "python -m pip install jupyterlab~=3.1",
                 "jlpm"
             ]
         }
     },
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.fb26a52f062bfbd4034e.js",
+            "style": "./style"
+        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "etc_jupyterlab_telemetry_library"
                 },
                 "managers": [
                     "pip"
                 ]
             }
         },
         "extension": true,
         "outputDir": "etc_jupyterlab_telemetry_library/labextension",
-        "schemaDir": "schema",
-        "sharedPackages": {
-            "@educational-technology-collective/etc_jupyterlab_notebook_state_provider": {
-                "bundled": false,
-                "singleton": true,
-                "strictVersion": true
-            }
-        }
+        "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "@educational-technology-collective/etc_jupyterlab_telemetry_library",
     "repository": {
         "type": "git",
         "url": "https://github.com/educational-technology-collective/etc_jupyterlab_telemetry_library.git"
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
-        "clean:labextension": "rimraf etc_jupyterlab_telemetry_library/labextension",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
+        "clean": "jlpm clean:lib",
+        "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
+        "clean:labextension": "rimraf etc_jupyterlab_telemetry_library/labextension etc_jupyterlab_telemetry_library/_version.py",
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
-    "version": "2.1.8"
+    "version": "2.2.0"
 }
```

### Comparing `etc_jupyterlab_telemetry_library-2.1.8/src/handler.ts` & `etc_jupyterlab_telemetry_library-2.2.0/src/handler.ts`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'etc-jupyterlab-telemetry-library', // API Namespace
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

### Comparing `etc_jupyterlab_telemetry_library-2.1.8/src/library.ts` & `etc_jupyterlab_telemetry_library-2.2.0/src/library.ts`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import {
     NotebookPanel,
     INotebookModel,
     Notebook,
     NotebookActions,
-    KernelError
+    KernelError,
+    CellList
 } from '@jupyterlab/notebook';
 
 import {
     ISignal,
     Signal
 } from '@lumino/signaling';
 
 import {
     Cell,
     ICellModel
 } from '@jupyterlab/cells';
 
 import {
-    IObservableList,
-    IObservableUndoableList
+    IObservableList
 } from '@jupyterlab/observables';
 
 import {
     DocumentRegistry
 } from '@jupyterlab/docregistry';
 
-import { IMessage, MessageType } from '@jupyterlab/services/lib/kernel/messages';
-
 import { ICellMeta, IConfig, INotebookEventMessage, INotebookEventOptions } from './types';
 
 import { requestAPI } from './handler';
 
 export class ETCJupyterLabTelemetryLibrary {
 
     public notebookClipboardEvent: NotebookClipboardEvent;
@@ -649,22 +647,22 @@
         }
     }
 
     private onDisposed() {
         Signal.disconnectAll(this);
     }
 
-    private onActiveCellChanged(send: Notebook, args: Cell<ICellModel>): void {
+    private onActiveCellChanged(send: Notebook, args: Cell<ICellModel> | null): void {
 
         if (this._notebook.widgets.length > 1) {
             //  More than 1 cell is needed in order for this event to happen; hence, check the number of cells.
 
             let cells = [
                 {
-                    id: args.model.id,
+                    id: args?.model.id,
                     index: this._notebook.widgets.findIndex((value: Cell<ICellModel>) => value == args)
                 }
             ];
 
             this._activeCellChanged.emit({
                 eventName: 'active_cell_changed',
                 cells: cells,
@@ -765,15 +763,15 @@
 
     private onDisposed() {
 
         Signal.disconnectAll(this);
     }
 
     private onCellsChanged(
-        sender: IObservableUndoableList<ICellModel>,
+        sender: CellList,
         args: IObservableList.IChangedArgs<ICellModel>) {
 
         if (args.type == 'add') {
 
             let cells = [{ id: args.newValues[0].id, index: args.newIndex }];
 
             this._cellAdded.emit({
@@ -817,15 +815,15 @@
 
     private onDisposed() {
 
         Signal.disconnectAll(this);
     }
 
     private onCellsChanged(
-        sender: IObservableUndoableList<ICellModel>,
+        sender: CellList,
         args: IObservableList.IChangedArgs<ICellModel>) {
 
         if (args.type == 'remove') {
 
             let cells = [{ id: args.oldValues[0].id, index: args.oldIndex }];
 
             this._cellRemoved.emit({
```

### Comparing `etc_jupyterlab_telemetry_library-2.1.8/src/types.ts` & `etc_jupyterlab_telemetry_library-2.2.0/src/types.ts`

 * *Files identical despite different names*

### Comparing `etc_jupyterlab_telemetry_library-2.1.8/tsconfig.json` & `etc_jupyterlab_telemetry_library-2.2.0/tsconfig.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9868421052631579%*

 * *Differences: {"'compilerOptions'": "{'noUnusedLocals': True, 'target': 'ES2018'}"}*

```diff
@@ -6,21 +6,21 @@
         "esModuleInterop": true,
         "incremental": true,
         "jsx": "react",
         "module": "esnext",
         "moduleResolution": "node",
         "noEmitOnError": true,
         "noImplicitAny": true,
-        "noUnusedLocals": false,
+        "noUnusedLocals": true,
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

