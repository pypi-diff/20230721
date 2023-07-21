# Comparing `tmp/sqlmath-2023.6.26.tar.gz` & `tmp/sqlmath-2023.7.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmath-2023.6.26.tar", last modified: Mon Jun 26 18:19:42 2023, max compression
+gzip compressed data, was "sqlmath-2023.7.21.tar", last modified: Fri Jul 21 19:11:47 2023, max compression
```

## Comparing `sqlmath-2023.6.26.tar` & `sqlmath-2023.7.21.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 18:19:42.369035 sqlmath-2023.6.26/
--rw-rw-rw-   0        0        0    14419 2023-05-19 17:59:37.000000 sqlmath-2023.6.26/.ci.sh
--rw-rw-rw-   0        0        0      649 2023-06-26 18:06:40.000000 sqlmath-2023.6.26/.gitconfig
-drwxrwxrwx   0        0        0        0 2023-06-26 18:19:42.320034 sqlmath-2023.6.26/.github/
-drwxrwxrwx   0        0        0        0 2023-06-26 18:19:42.363037 sqlmath-2023.6.26/.github/workflows/
--rw-rw-rw-   0        0        0     2678 2023-06-26 18:06:40.000000 sqlmath-2023.6.26/.github/workflows/ci.yml
--rw-rw-rw-   0        0        0     1979 2023-06-26 18:06:41.000000 sqlmath-2023.6.26/.github/workflows/publish.yml
--rw-rw-rw-   0        0        0      350 2023-06-26 18:06:41.000000 sqlmath-2023.6.26/.gitignore
--rw-rw-rw-   0        0        0      121 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/.npmignore
--rw-rw-rw-   0        0        0    22602 2023-06-26 17:28:16.000000 sqlmath-2023.6.26/CHANGELOG.md
--rw-rw-rw-   0        0        0     1051 2023-04-27 14:22:07.000000 sqlmath-2023.6.26/LICENSE
--rw-rw-rw-   0        0        0      941 2023-06-26 17:31:00.000000 sqlmath-2023.6.26/MANIFEST.in
--rw-rw-rw-   0        0        0     7336 2023-06-26 18:19:42.369035 sqlmath-2023.6.26/PKG-INFO
--rw-rw-rw-   0        0        0     4924 2023-06-26 17:31:03.000000 sqlmath-2023.6.26/README.md
--rw-rw-rw-   0        0        0      564 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/asset_image_folder_open_solid.svg
--rw-rw-rw-   0        0        0     1536 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/asset_image_github_brands.svg
--rw-rw-rw-   0        0        0     1060 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/asset_image_logo_512.html
--rw-rw-rw-   0        0        0     7087 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/asset_image_logo_512.png
--rw-rw-rw-   0        0        0     2823 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/asset_image_logo_512.svg
--rw-rw-rw-   0        0        0   472927 2023-06-26 17:31:58.000000 sqlmath-2023.6.26/asset_sqlmath_external_rollup.js
--rw-rw-rw-   0        0        0   262193 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/cpplint.py
--rw-rw-rw-   0        0        0   385557 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/csslint.js
--rwxrwxrwx   0        0        0    72704 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/indent.exe
--rw-rw-rw-   0        0        0    23525 2023-06-26 17:31:59.000000 sqlmath-2023.6.26/index.html
--rw-rw-rw-   0        0        0   337350 2023-05-24 18:34:34.000000 sqlmath-2023.6.26/jslint.mjs
--rw-rw-rw-   0        0        0   100564 2023-05-25 18:03:44.000000 sqlmath-2023.6.26/jslint_ci.sh
--rw-rw-rw-   0        0        0  1008128 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/libiconv2.dll
--rw-rw-rw-   0        0        0   103424 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/libintl3.dll
--rw-rw-rw-   0        0        0      920 2023-06-26 17:30:54.000000 sqlmath-2023.6.26/package.json
--rw-rw-rw-   0        0        0     1497 2023-05-25 19:02:01.000000 sqlmath-2023.6.26/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-26 18:19:42.369035 sqlmath-2023.6.26/setup.cfg
--rw-rw-rw-   0        0        0    12790 2023-05-26 16:26:03.000000 sqlmath-2023.6.26/setup.py
--rw-rw-rw-   0        0        0 11372418 2023-06-26 17:32:05.000000 sqlmath-2023.6.26/sqlite_rollup.c
-drwxrwxrwx   0        0        0        0 2023-06-26 18:19:42.365039 sqlmath-2023.6.26/sqlmath/
--rw-rw-rw-   0        0        0      855 2023-06-26 17:31:03.000000 sqlmath-2023.6.26/sqlmath/__init__.py
--rw-rw-rw-   0        0        0   148110 2023-06-26 17:32:07.000000 sqlmath-2023.6.26/sqlmath/sqlmath_dbapi2.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:19:42.368035 sqlmath-2023.6.26/sqlmath.egg-info/
--rw-rw-rw-   0        0        0     7336 2023-06-26 18:19:42.000000 sqlmath-2023.6.26/sqlmath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      760 2023-06-26 18:19:42.000000 sqlmath-2023.6.26/sqlmath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 18:19:42.000000 sqlmath-2023.6.26/sqlmath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-26 18:19:42.000000 sqlmath-2023.6.26/sqlmath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    37595 2023-06-26 17:30:54.000000 sqlmath-2023.6.26/sqlmath.mjs
--rw-rw-rw-   0        0        0    92524 2023-06-20 14:29:28.000000 sqlmath-2023.6.26/sqlmath_base.c
--rw-rw-rw-   0        0        0   142223 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/sqlmath_browser.mjs
--rw-rw-rw-   0        0        0     1522 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/sqlmath_custom.c
--rw-rw-rw-   0        0        0      150 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/sqlmath_custom.mjs
--rw-rw-rw-   0        0        0    32647 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/sqlmath_jenks.c
--rw-rw-rw-   0        0        0     7931 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/sqlmath_wrapper_wasm.js
--rw-rw-rw-   0        0        0    73312 2023-06-20 14:29:28.000000 sqlmath-2023.6.26/test.mjs
+drwxrwxrwx   0        0        0        0 2023-07-21 19:11:47.880912 sqlmath-2023.7.21/
+-rw-rw-rw-   0        0        0    14419 2023-05-19 17:59:37.000000 sqlmath-2023.7.21/.ci.sh
+-rw-rw-rw-   0        0        0      649 2023-07-21 18:35:39.000000 sqlmath-2023.7.21/.gitconfig
+drwxrwxrwx   0        0        0        0 2023-07-21 19:11:47.834036 sqlmath-2023.7.21/.github/
+drwxrwxrwx   0        0        0        0 2023-07-21 19:11:47.880912 sqlmath-2023.7.21/.github/workflows/
+-rw-rw-rw-   0        0        0     2678 2023-07-21 18:35:39.000000 sqlmath-2023.7.21/.github/workflows/ci.yml
+-rw-rw-rw-   0        0        0     1979 2023-07-21 18:35:40.000000 sqlmath-2023.7.21/.github/workflows/publish.yml
+-rw-rw-rw-   0        0        0      350 2023-07-21 18:35:40.000000 sqlmath-2023.7.21/.gitignore
+-rw-rw-rw-   0        0        0      121 2023-05-16 16:00:43.000000 sqlmath-2023.7.21/.npmignore
+-rw-rw-rw-   0        0        0    22764 2023-07-21 18:13:11.000000 sqlmath-2023.7.21/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1051 2023-04-27 14:22:07.000000 sqlmath-2023.7.21/LICENSE
+-rw-rw-rw-   0        0        0      941 2023-07-21 18:15:39.000000 sqlmath-2023.7.21/MANIFEST.in
+-rw-rw-rw-   0        0        0     7336 2023-07-21 19:11:47.880912 sqlmath-2023.7.21/PKG-INFO
+-rw-rw-rw-   0        0        0     4924 2023-07-21 18:15:40.000000 sqlmath-2023.7.21/README.md
+-rw-rw-rw-   0        0        0      564 2023-05-16 16:00:43.000000 sqlmath-2023.7.21/asset_image_folder_open_solid.svg
+-rw-rw-rw-   0        0        0     1536 2023-05-16 16:00:43.000000 sqlmath-2023.7.21/asset_image_github_brands.svg
+-rw-rw-rw-   0        0        0     1060 2023-05-16 16:00:43.000000 sqlmath-2023.7.21/asset_image_logo_512.html
+-rw-rw-rw-   0        0        0     7087 2023-05-16 16:00:43.000000 sqlmath-2023.7.21/asset_image_logo_512.png
+-rw-rw-rw-   0        0        0     2823 2023-05-16 16:00:43.000000 sqlmath-2023.7.21/asset_image_logo_512.svg
+-rw-rw-rw-   0        0        0   472927 2023-07-21 18:32:16.000000 sqlmath-2023.7.21/asset_sqlmath_external_rollup.js
+-rw-rw-rw-   0        0        0   262193 2023-05-16 16:00:43.000000 sqlmath-2023.7.21/cpplint.py
+-rw-rw-rw-   0        0        0   385557 2023-05-16 16:00:43.000000 sqlmath-2023.7.21/csslint.js
+-rwxrwxrwx   0        0        0    72704 2023-05-16 16:00:43.000000 sqlmath-2023.7.21/indent.exe
+-rw-rw-rw-   0        0        0    23525 2023-07-21 18:32:18.000000 sqlmath-2023.7.21/index.html
+-rw-rw-rw-   0        0        0   337346 2023-07-21 17:36:43.000000 sqlmath-2023.7.21/jslint.mjs
+-rw-rw-rw-   0        0        0   100490 2023-07-21 14:06:22.000000 sqlmath-2023.7.21/jslint_ci.sh
+-rw-rw-rw-   0        0        0  1008128 2023-05-16 16:00:43.000000 sqlmath-2023.7.21/libiconv2.dll
+-rw-rw-rw-   0        0        0   103424 2023-05-16 16:00:43.000000 sqlmath-2023.7.21/libintl3.dll
+-rw-rw-rw-   0        0        0      920 2023-07-21 18:15:30.000000 sqlmath-2023.7.21/package.json
+-rw-rw-rw-   0        0        0     1497 2023-05-25 19:02:01.000000 sqlmath-2023.7.21/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-21 19:11:47.880912 sqlmath-2023.7.21/setup.cfg
+-rw-rw-rw-   0        0        0    12820 2023-07-03 20:57:05.000000 sqlmath-2023.7.21/setup.py
+-rw-rw-rw-   0        0        0 11372418 2023-07-21 18:32:22.000000 sqlmath-2023.7.21/sqlite_rollup.c
+drwxrwxrwx   0        0        0        0 2023-07-21 19:11:47.880912 sqlmath-2023.7.21/sqlmath/
+-rw-rw-rw-   0        0        0      855 2023-07-21 18:15:40.000000 sqlmath-2023.7.21/sqlmath/__init__.py
+-rw-rw-rw-   0        0        0   148110 2023-07-21 18:32:23.000000 sqlmath-2023.7.21/sqlmath/sqlmath_dbapi2.py
+drwxrwxrwx   0        0        0        0 2023-07-21 19:11:47.880912 sqlmath-2023.7.21/sqlmath.egg-info/
+-rw-rw-rw-   0        0        0     7336 2023-07-21 19:11:47.000000 sqlmath-2023.7.21/sqlmath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      760 2023-07-21 19:11:47.000000 sqlmath-2023.7.21/sqlmath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 19:11:47.000000 sqlmath-2023.7.21/sqlmath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-21 19:11:47.000000 sqlmath-2023.7.21/sqlmath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    37660 2023-07-21 18:15:30.000000 sqlmath-2023.7.21/sqlmath.mjs
+-rw-rw-rw-   0        0        0    93021 2023-07-13 18:56:04.000000 sqlmath-2023.7.21/sqlmath_base.c
+-rw-rw-rw-   0        0        0   142230 2023-07-21 18:14:02.000000 sqlmath-2023.7.21/sqlmath_browser.mjs
+-rw-rw-rw-   0        0        0     1522 2023-05-16 16:00:43.000000 sqlmath-2023.7.21/sqlmath_custom.c
+-rw-rw-rw-   0        0        0      150 2023-05-16 16:00:43.000000 sqlmath-2023.7.21/sqlmath_custom.mjs
+-rw-rw-rw-   0        0        0    32647 2023-05-16 16:00:43.000000 sqlmath-2023.7.21/sqlmath_jenks.c
+-rw-rw-rw-   0        0        0     7931 2023-05-16 16:00:43.000000 sqlmath-2023.7.21/sqlmath_wrapper_wasm.js
+-rw-rw-rw-   0        0        0    76531 2023-07-17 14:05:15.000000 sqlmath-2023.7.21/test.mjs
```

### Comparing `sqlmath-2023.6.26/.ci.sh` & `sqlmath-2023.7.21/.ci.sh`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/.gitconfig` & `sqlmath-2023.7.21/.gitconfig`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/.github/workflows/ci.yml` & `sqlmath-2023.7.21/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/.github/workflows/publish.yml` & `sqlmath-2023.7.21/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/CHANGELOG.md` & `sqlmath-2023.7.21/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Changelog
 
 # Todo
 - none
 
+# v2023.7.21
+- sqlmath - Update sql-function win_slr2() to additionally return predicted y-value and rmse.
+- betadog - Migrate market-indicator from spy to spx.
+
 # v2023.6.26
 - sqlmath - fix broken interpolation in sql-function quantile().
 - sqlmath - Add sql-function win_quantile1(), win_quantile2().
 - sqlmath - Update sql-function win_slr2() to be vectorized.
 - sqlmath - Add sql-function win_ema2().
 - betadog - Add feature xema_xxx into ml model.
 - sqlmath - Add sql-function win_slr().
```

### Comparing `sqlmath-2023.6.26/LICENSE` & `sqlmath-2023.7.21/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/MANIFEST.in` & `sqlmath-2023.7.21/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/PKG-INFO` & `sqlmath-2023.7.21/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmath
-Version: 2023.6.26
+Version: 2023.7.21
 Summary: sqlite for datascience
 Author: Kai Zhu
 License: Copyright (c) 2021 Kai Zhu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -44,15 +44,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sqlmath - sqlite for data-science
 
 
 # Status
-| Branch | [master<br>(v2023.6.26)](https://github.com/sqlmath/sqlmath/tree/master) | [beta<br>(Web Demo)](https://github.com/sqlmath/sqlmath/tree/beta) | [alpha<br>(Development)](https://github.com/sqlmath/sqlmath/tree/alpha) |
+| Branch | [master<br>(v2023.7.21)](https://github.com/sqlmath/sqlmath/tree/master) | [beta<br>(Web Demo)](https://github.com/sqlmath/sqlmath/tree/beta) | [alpha<br>(Development)](https://github.com/sqlmath/sqlmath/tree/alpha) |
 |--:|:--:|:--:|:--:|
 | CI | [![ci](https://github.com/sqlmath/sqlmath/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/sqlmath/sqlmath/actions?query=branch%3Amaster) | [![ci](https://github.com/sqlmath/sqlmath/actions/workflows/ci.yml/badge.svg?branch=beta)](https://github.com/sqlmath/sqlmath/actions?query=branch%3Abeta) | [![ci](https://github.com/sqlmath/sqlmath/actions/workflows/ci.yml/badge.svg?branch=alpha)](https://github.com/sqlmath/sqlmath/actions?query=branch%3Aalpha) |
 | Coverage | [![coverage](https://sqlmath.github.io/sqlmath/branch-master/.artifact/coverage/coverage_badge.svg)](https://sqlmath.github.io/sqlmath/branch-master/.artifact/coverage/index.html) | [![coverage](https://sqlmath.github.io/sqlmath/branch-beta/.artifact/coverage/coverage_badge.svg)](https://sqlmath.github.io/sqlmath/branch-beta/.artifact/coverage/index.html) | [![coverage](https://sqlmath.github.io/sqlmath/branch-alpha/.artifact/coverage/coverage_badge.svg)](https://sqlmath.github.io/sqlmath/branch-alpha/.artifact/coverage/index.html) |
 | Demo | [<img src="asset_image_github_brands.svg" height="32">](https://sqlmath.github.io/sqlmath/branch-master/index.html) | [<img src="asset_image_github_brands.svg" height="32">](https://sqlmath.github.io/sqlmath/branch-beta/index.html) | [<img src="asset_image_github_brands.svg" height="32">](https://sqlmath.github.io/sqlmath/branch-alpha/index.html) |
 | Artifacts | [<img src="asset_image_folder_open_solid.svg" height="30">](https://github.com/sqlmath/sqlmath/tree/gh-pages/branch-master/.artifact) | [<img src="asset_image_folder_open_solid.svg" height="30">](https://github.com/sqlmath/sqlmath/tree/gh-pages/branch-beta/.artifact) | [<img src="asset_image_folder_open_solid.svg" height="30">](https://github.com/sqlmath/sqlmath/tree/gh-pages/branch-alpha/.artifact) |
 
 
@@ -162,13 +162,13 @@
 
 
 <br><br>
 ### python pypi publish
 ```shell
 python -m build
 #
-twine upload --repository testpypi dist/sqlmath-2023.6.26*
-py -m pip install --index-url https://test.pypi.org/simple/ sqlmath==2023.6.26
+twine upload --repository testpypi dist/sqlmath-2023.7.21*
+py -m pip install --index-url https://test.pypi.org/simple/ sqlmath==2023.7.21
 #
-twine upload dist/sqlmath-2023.6.26*
-pip install sqlmath==2023.6.26
+twine upload dist/sqlmath-2023.7.21*
+pip install sqlmath==2023.7.21
 ```
```

### Comparing `sqlmath-2023.6.26/README.md` & `sqlmath-2023.7.21/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # sqlmath - sqlite for data-science
 
 
 # Status
-| Branch | [master<br>(v2023.6.26)](https://github.com/sqlmath/sqlmath/tree/master) | [beta<br>(Web Demo)](https://github.com/sqlmath/sqlmath/tree/beta) | [alpha<br>(Development)](https://github.com/sqlmath/sqlmath/tree/alpha) |
+| Branch | [master<br>(v2023.7.21)](https://github.com/sqlmath/sqlmath/tree/master) | [beta<br>(Web Demo)](https://github.com/sqlmath/sqlmath/tree/beta) | [alpha<br>(Development)](https://github.com/sqlmath/sqlmath/tree/alpha) |
 |--:|:--:|:--:|:--:|
 | CI | [![ci](https://github.com/sqlmath/sqlmath/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/sqlmath/sqlmath/actions?query=branch%3Amaster) | [![ci](https://github.com/sqlmath/sqlmath/actions/workflows/ci.yml/badge.svg?branch=beta)](https://github.com/sqlmath/sqlmath/actions?query=branch%3Abeta) | [![ci](https://github.com/sqlmath/sqlmath/actions/workflows/ci.yml/badge.svg?branch=alpha)](https://github.com/sqlmath/sqlmath/actions?query=branch%3Aalpha) |
 | Coverage | [![coverage](https://sqlmath.github.io/sqlmath/branch-master/.artifact/coverage/coverage_badge.svg)](https://sqlmath.github.io/sqlmath/branch-master/.artifact/coverage/index.html) | [![coverage](https://sqlmath.github.io/sqlmath/branch-beta/.artifact/coverage/coverage_badge.svg)](https://sqlmath.github.io/sqlmath/branch-beta/.artifact/coverage/index.html) | [![coverage](https://sqlmath.github.io/sqlmath/branch-alpha/.artifact/coverage/coverage_badge.svg)](https://sqlmath.github.io/sqlmath/branch-alpha/.artifact/coverage/index.html) |
 | Demo | [<img src="asset_image_github_brands.svg" height="32">](https://sqlmath.github.io/sqlmath/branch-master/index.html) | [<img src="asset_image_github_brands.svg" height="32">](https://sqlmath.github.io/sqlmath/branch-beta/index.html) | [<img src="asset_image_github_brands.svg" height="32">](https://sqlmath.github.io/sqlmath/branch-alpha/index.html) |
 | Artifacts | [<img src="asset_image_folder_open_solid.svg" height="30">](https://github.com/sqlmath/sqlmath/tree/gh-pages/branch-master/.artifact) | [<img src="asset_image_folder_open_solid.svg" height="30">](https://github.com/sqlmath/sqlmath/tree/gh-pages/branch-beta/.artifact) | [<img src="asset_image_folder_open_solid.svg" height="30">](https://github.com/sqlmath/sqlmath/tree/gh-pages/branch-alpha/.artifact) |
 
 
@@ -116,13 +116,13 @@
 
 
 <br><br>
 ### python pypi publish
 ```shell
 python -m build
 #
-twine upload --repository testpypi dist/sqlmath-2023.6.26*
-py -m pip install --index-url https://test.pypi.org/simple/ sqlmath==2023.6.26
+twine upload --repository testpypi dist/sqlmath-2023.7.21*
+py -m pip install --index-url https://test.pypi.org/simple/ sqlmath==2023.7.21
 #
-twine upload dist/sqlmath-2023.6.26*
-pip install sqlmath==2023.6.26
+twine upload dist/sqlmath-2023.7.21*
+pip install sqlmath==2023.7.21
 ```
```

### Comparing `sqlmath-2023.6.26/asset_image_folder_open_solid.svg` & `sqlmath-2023.7.21/asset_image_folder_open_solid.svg`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/asset_image_github_brands.svg` & `sqlmath-2023.7.21/asset_image_github_brands.svg`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/asset_image_logo_512.html` & `sqlmath-2023.7.21/asset_image_logo_512.html`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/asset_image_logo_512.png` & `sqlmath-2023.7.21/asset_image_logo_512.png`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/asset_image_logo_512.svg` & `sqlmath-2023.7.21/asset_image_logo_512.svg`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/asset_sqlmath_external_rollup.js` & `sqlmath-2023.7.21/asset_sqlmath_external_rollup.js`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/cpplint.py` & `sqlmath-2023.7.21/cpplint.py`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/csslint.js` & `sqlmath-2023.7.21/csslint.js`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/indent.exe` & `sqlmath-2023.7.21/indent.exe`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/index.html` & `sqlmath-2023.7.21/index.html`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/jslint.mjs` & `sqlmath-2023.7.21/jslint.mjs`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
     + "\b\t\n\u000b\f\r\u000e\u000f"
     + "\u0010\u0011\u0012\u0013\u0014\u0015\u0016\u0017"
     + "\u0018\u0019\u001a\u001b\u001c\u001d\u001e\u001f"
     + " !\"#$%&'()*+,-./0123456789:;<=>?"
     + "@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\\]^_"
     + "`abcdefghijklmnopqrstuvwxyz{|}~\u007f"
 );
-let jslint_edition = "v2023.6.1-beta";
+let jslint_edition = "v2023.6.21";
 let jslint_export;                      // The jslint object to be exported.
 let jslint_fudge = 1;                   // Fudge starting line and starting
                                         // ... column to 1.
 let jslint_import_meta_url = "";        // import.meta.url used by cli.
 let jslint_rgx_cap = (
     /^[A-Z]/
 );
```

### Comparing `sqlmath-2023.6.26/jslint_ci.sh` & `sqlmath-2023.7.21/jslint_ci.sh`

 * *Files 0% similar despite different names*

```diff
@@ -661,24 +661,25 @@
     export GITHUB_GITHUB_IO="$(
         printf "$GITHUB_REPOSITORY" | sed -e "s|/|.github.io/|"
     )"
     node --input-type=module --eval '
 import moduleAssert from "assert";
 import moduleFs from "fs";
 import moduleHttps from "https";
-import moduleUrl from "url";
 (async function () {
     let {
         GITHUB_BRANCH0,
         GITHUB_GITHUB_IO,
         GITHUB_REPOSITORY,
         UPSTREAM_GITHUB_IO,
         UPSTREAM_REPOSITORY
     } = process.env;
-    let dict = {};
+    let dict = {
+        "https://unlicense.org/": true
+    };
     Array.from(
         await moduleFs.promises.readdir(".")
     ).forEach(async function (file) {
         let data;
         if (file === "CHANGELOG.md" || !(
             /.\.html$|.\.md$/m
         ).test(file)) {
@@ -714,17 +715,15 @@
                 `shDirHttplinkValidate - ${file} - insecure link - ${url}`
             );
             // ignore duplicate-link
             if (dict.hasOwnProperty(url)) {
                 return "";
             }
             dict[url] = true;
-            req = moduleHttps.request(moduleUrl.parse(
-                url
-            ), function (res) {
+            req = moduleHttps.request(url, function (res) {
                 console.error(
                     "shDirHttplinkValidate " + res.statusCode + " " + url
                 );
                 moduleAssert.ok(
                     res.statusCode < 400,
                     `shDirHttplinkValidate - ${file} - unreachable url ${url}`
                 );
@@ -1011,16 +1010,15 @@
         "https://github.com/$GITHUB_REPOSITORY" __tmp1 \
         --branch="$GITHUB_REF_NAME" --depth=1 --single-branch
     mv __tmp1/.git .
     cp __tmp1/.gitconfig .git/config
     rm -rf __tmp1
     git reset "origin/$GITHUB_REF_NAME" --hard
     # fetch jslint_ci.sh from trusted source
-    git branch -D __tmp1 &>/dev/null || true
-    shGitCmdWithGithubToken fetch origin alpha:__tmp1 --depth=1
+    shGitCmdWithGithubToken fetch origin alpha:__tmp1 --depth=1 -f
     for FILE in .ci.sh .ci2.sh jslint_ci.sh myci2.sh
     do
         if [ -f "$FILE" ]
         then
             git checkout __tmp1 "$FILE"
         fi
     done
```

### Comparing `sqlmath-2023.6.26/libiconv2.dll` & `sqlmath-2023.7.21/libiconv2.dll`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/libintl3.dll` & `sqlmath-2023.7.21/libintl3.dll`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/package.json` & `sqlmath-2023.7.21/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'version'": "'2023.7.21'"}*

```diff
@@ -34,9 +34,9 @@
     "scripts": {
         "build": "sh jslint_ci.sh shCiBuildNodejs",
         "test": "sh jslint_ci.sh shCiTestNodejs",
         "test2": "sh jslint_ci.sh shCiBase"
     },
     "shCiArtifactUpload": 1,
     "shCiNpmPublish": 1,
-    "version": "2023.6.26"
+    "version": "2023.7.21"
 }
```

### Comparing `sqlmath-2023.6.26/pyproject.toml` & `sqlmath-2023.7.21/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/setup.py` & `sqlmath-2023.7.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,15 @@
             key.lower(): val
             for key, _, val in
             (line.partition("=") for line in env.splitlines())
             if key and val
         }
         await_list = []
         for exe in ["cl.exe", "link.exe"]:
-            await_list.append(
+            await_list.append( # noqa=PERF401
                 (
                     await asyncio.create_subprocess_exec(
                         *["where", exe],
                         env=env,
                         stdout=asyncio.subprocess.PIPE,
                     )
                 ).stdout.readline(),
@@ -274,15 +274,15 @@
             exe.splitlines()[0] for exe in await asyncio.gather(*await_list)
         ]
     #
     # build_ext - virtualenv
     for arr in [path_include, path_library]:
         for path in arr:
             if path_prefix_base != path_prefix:
-                arr.append(path.replace(path_prefix, path_prefix_base))
+                arr.append(path.replace(path_prefix, path_prefix_base)) # noqa=PERF401
     #
     # build_ext - compile .obj file
     await asyncio.gather(*[
         build_ext_obj(cdefine)
         for cdefine in [
             "SRC_ZLIB_BASE",
             "SRC_ZLIB_TEST_EXAMPLE",
```

### Comparing `sqlmath-2023.6.26/sqlite_rollup.c` & `sqlmath-2023.7.21/sqlite_rollup.c`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/sqlmath/__init__.py` & `sqlmath-2023.7.21/sqlmath/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """sqlmath.py."""
 
-__version__ = "2023.6.26"
-__version_info__ = ("2023", "6", "26")
+__version__ = "2023.7.21"
+__version_info__ = ("2023", "7", "21")
 
 import sys
 
 from .sqlmath_dbapi2 import *  # noqa=F403
 
 
 def debugInline(*argv): # noqa=N802
```

### Comparing `sqlmath-2023.6.26/sqlmath/sqlmath_dbapi2.py` & `sqlmath-2023.7.21/sqlmath/sqlmath_dbapi2.py`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/sqlmath.egg-info/PKG-INFO` & `sqlmath-2023.7.21/sqlmath.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmath
-Version: 2023.6.26
+Version: 2023.7.21
 Summary: sqlite for datascience
 Author: Kai Zhu
 License: Copyright (c) 2021 Kai Zhu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -44,15 +44,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sqlmath - sqlite for data-science
 
 
 # Status
-| Branch | [master<br>(v2023.6.26)](https://github.com/sqlmath/sqlmath/tree/master) | [beta<br>(Web Demo)](https://github.com/sqlmath/sqlmath/tree/beta) | [alpha<br>(Development)](https://github.com/sqlmath/sqlmath/tree/alpha) |
+| Branch | [master<br>(v2023.7.21)](https://github.com/sqlmath/sqlmath/tree/master) | [beta<br>(Web Demo)](https://github.com/sqlmath/sqlmath/tree/beta) | [alpha<br>(Development)](https://github.com/sqlmath/sqlmath/tree/alpha) |
 |--:|:--:|:--:|:--:|
 | CI | [![ci](https://github.com/sqlmath/sqlmath/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/sqlmath/sqlmath/actions?query=branch%3Amaster) | [![ci](https://github.com/sqlmath/sqlmath/actions/workflows/ci.yml/badge.svg?branch=beta)](https://github.com/sqlmath/sqlmath/actions?query=branch%3Abeta) | [![ci](https://github.com/sqlmath/sqlmath/actions/workflows/ci.yml/badge.svg?branch=alpha)](https://github.com/sqlmath/sqlmath/actions?query=branch%3Aalpha) |
 | Coverage | [![coverage](https://sqlmath.github.io/sqlmath/branch-master/.artifact/coverage/coverage_badge.svg)](https://sqlmath.github.io/sqlmath/branch-master/.artifact/coverage/index.html) | [![coverage](https://sqlmath.github.io/sqlmath/branch-beta/.artifact/coverage/coverage_badge.svg)](https://sqlmath.github.io/sqlmath/branch-beta/.artifact/coverage/index.html) | [![coverage](https://sqlmath.github.io/sqlmath/branch-alpha/.artifact/coverage/coverage_badge.svg)](https://sqlmath.github.io/sqlmath/branch-alpha/.artifact/coverage/index.html) |
 | Demo | [<img src="asset_image_github_brands.svg" height="32">](https://sqlmath.github.io/sqlmath/branch-master/index.html) | [<img src="asset_image_github_brands.svg" height="32">](https://sqlmath.github.io/sqlmath/branch-beta/index.html) | [<img src="asset_image_github_brands.svg" height="32">](https://sqlmath.github.io/sqlmath/branch-alpha/index.html) |
 | Artifacts | [<img src="asset_image_folder_open_solid.svg" height="30">](https://github.com/sqlmath/sqlmath/tree/gh-pages/branch-master/.artifact) | [<img src="asset_image_folder_open_solid.svg" height="30">](https://github.com/sqlmath/sqlmath/tree/gh-pages/branch-beta/.artifact) | [<img src="asset_image_folder_open_solid.svg" height="30">](https://github.com/sqlmath/sqlmath/tree/gh-pages/branch-alpha/.artifact) |
 
 
@@ -162,13 +162,13 @@
 
 
 <br><br>
 ### python pypi publish
 ```shell
 python -m build
 #
-twine upload --repository testpypi dist/sqlmath-2023.6.26*
-py -m pip install --index-url https://test.pypi.org/simple/ sqlmath==2023.6.26
+twine upload --repository testpypi dist/sqlmath-2023.7.21*
+py -m pip install --index-url https://test.pypi.org/simple/ sqlmath==2023.7.21
 #
-twine upload dist/sqlmath-2023.6.26*
-pip install sqlmath==2023.6.26
+twine upload dist/sqlmath-2023.7.21*
+pip install sqlmath==2023.7.21
 ```
```

### Comparing `sqlmath-2023.6.26/sqlmath.egg-info/SOURCES.txt` & `sqlmath-2023.7.21/sqlmath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/sqlmath.mjs` & `sqlmath-2023.7.21/sqlmath.mjs`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 let SQLITE_OPEN_SUBJOURNAL = 0x00002000;    /* VFS only */
 let SQLITE_OPEN_SUPER_JOURNAL = 0x00004000; /* VFS only */
 let SQLITE_OPEN_TEMP_DB = 0x00000200;       /* VFS only */
 let SQLITE_OPEN_TEMP_JOURNAL = 0x00001000;  /* VFS only */
 let SQLITE_OPEN_TRANSIENT_DB = 0x00000400;  /* VFS only */
 let SQLITE_OPEN_URI = 0x00000040;           /* Ok for sqlite3_open_v2() */
 let SQLITE_OPEN_WAL = 0x00080000;           /* VFS only */
+let SQLITE_WIN_SLR_ELEM_SIZE = 10;
 let cModule;
 let cModulePath;
 let consoleError = console.error;
 let dbDict = new WeakMap(); // private-dict of sqlite-database-connections
 let dbFinalizationRegistry;
 // init debugInline
 let debugInline = (function () {
@@ -93,15 +94,15 @@
     npm_config_mode_debug,
     npm_config_mode_setup,
     npm_config_mode_test
 } = typeof process === "object" && process?.env;
 let sqlMessageDict = {}; // dict of web-worker-callbacks
 let sqlMessageId = 0;
 let sqlWorker;
-let version = "v2023.6.26";
+let version = "v2023.7.21";
 
 function assertJsonEqual(aa, bb, message) {
 
 // This function will assert JSON.stringify(<aa>) === JSON.stringify(<bb>).
 
     aa = JSON.stringify(objectDeepCopyWithKeysSorted(aa), undefined, 1);
     bb = JSON.stringify(objectDeepCopyWithKeysSorted(bb), undefined, 1);
@@ -1352,14 +1353,15 @@
     SQLITE_OPEN_SUBJOURNAL,
     SQLITE_OPEN_SUPER_JOURNAL,
     SQLITE_OPEN_TEMP_DB,
     SQLITE_OPEN_TEMP_JOURNAL,
     SQLITE_OPEN_TRANSIENT_DB,
     SQLITE_OPEN_URI,
     SQLITE_OPEN_WAL,
+    SQLITE_WIN_SLR_ELEM_SIZE,
     assertJsonEqual,
     assertNumericalEqual,
     assertOrThrow,
     childProcessSpawn2,
     ciBuildExt,
     dbCloseAsync,
     dbExecAndReturnLastBlobAsync,
```

### Comparing `sqlmath-2023.6.26/sqlmath_base.c` & `sqlmath-2023.7.21/sqlmath_base.c`

 * *Files 0% similar despite different names*

```diff
@@ -2429,26 +2429,29 @@
     double mxx;                 // average xx
     double myy;                 // average yy
     double exx;                 // stdev.s xx
     double eyy;                 // stdev.s yy
     double crr;                 // pearson xy
     double cbb;                 // linest slope
     double caa;                 // linest intercept
+    double cyy;                 // linest y-estimate
+    double cee;                 // linest y-error
 } WinSlrResult;
 static const int WinSlrResultN = sizeof(WinSlrResult) / sizeof(double);
 
 typedef struct WinSlrStep {
-    double invp;                // 1.0 / nnn
-    double invs;                // 1.0 / (nnn - 1)
+    double inv0;                // 1.0 / nnn
+    double inv1;                // 1.0 / (nnn - 1)
+    double inv2;                // 1.0 / (nnn - 2)
     double mxx;                 // average xx
     double myy;                 // average yy
     double nnn;                 // number of elements
-    double sxx;                 // variance.p xx
-    double sxy;                 // covariance.p xy
-    double syy;                 // variance.p yy
+    double vxx;                 // variance.p xx
+    double vxy;                 // covariance.p xy
+    double vyy;                 // variance.p yy
     double xx0;                 // previous xx
     double yy0;                 // previous yy
 } WinSlrStep;
 static const int WinSlrStepN = sizeof(WinSlrStep) / sizeof(double);
 
 SQLMATH_FUNC static void sql3_win_slr2_value(
     sqlite3_context * context
@@ -2459,29 +2462,35 @@
     // declare var
     const WinSlrStep *slr = (WinSlrStep *) vec99_head;
     const int ncol = vec99->ncol;
     double *result = vec99_head + ncol * WinSlrStepN;
     int errcode = 0;
     // calculate slr
     for (int ii = 0; ii < ncol; ii += 1) {
+        const double inv1 = slr->inv1;
+        const double inv2 = slr->inv2;
         const double mxx = slr->mxx;
         const double myy = slr->myy;
-        const double exx = sqrt(slr->sxx * slr->invs);
-        const double eyy = sqrt(slr->syy * slr->invs);
-        const double crr = slr->sxy / sqrt(slr->sxx * slr->syy);
-        const double cbb = slr->sxy / slr->sxx;
+        const double vxx = slr->vxx;
+        const double vxy = slr->vxy;
+        const double vyy = slr->vyy;
+        //
+        const double crr = vxy / sqrt(vxx * vyy);
+        const double cbb = vxy / vxx;
         const double caa = myy - cbb * mxx;
         result[0] = slr->nnn;
-        result[1] = mxx;
-        result[2] = myy;
-        result[3] = exx;
-        result[4] = eyy;
-        result[5] = crr;
-        result[6] = cbb;
-        result[7] = caa;
+        result[1] = mxx;        // mxx
+        result[2] = myy;        // myy
+        result[3] = sqrt(vxx * inv1);   // exx
+        result[4] = sqrt(vyy * inv1);   // eyy
+        result[5] = crr;        // crr
+        result[6] = cbb;        // cbb
+        result[7] = caa;        // caa
+        result[8] = caa + cbb * slr->xx0;       // cyy
+        result[9] = sqrt(vyy * (1 - crr * crr) * inv2); // cee
         result += WinSlrResultN;
         slr += 1;
     }
     // str99 - result
     SQLITE3_RESULT_JSONFLOAT64ARRAY(str99, result - ncol * WinSlrResultN,
         ncol * WinSlrResultN);
   catch_error:
@@ -2545,61 +2554,62 @@
         // fprintf(stderr, "ii=%d argv0=%f, xx0=%f mxx=%f pp=%p\n",        //
         //     ii, sqlite3_value_double_or_nan(argv[0]), slr->xx0, slr->mxx,
         //     slr);
         const double xx = sqlite3_value_double_or_prev(argv[0], &slr->xx0);
         const double yy = sqlite3_value_double_or_prev(argv[1], &slr->yy0);
         double mxx = slr->mxx;
         double myy = slr->myy;
-        double sxx = slr->sxx;
-        double sxy = slr->sxy;
-        double syy = slr->syy;
+        double vxx = slr->vxx;
+        double vxy = slr->vxy;
+        double vyy = slr->vyy;
         // vec99 - calculate slr
         if (vec99->wnn) {
             // calculate running slr - window
-            const double invp = slr->invp;
+            const double inv0 = slr->inv0;
             const double xx0 = xxyy0[0];
             const double yy0 = xxyy0[1];
             const double dx = xx - xx0;
             const double dy = yy - yy0;
-            sxx += (xx * xx - xx0 * xx0) - invp * dx * dx - 2 * dx * mxx;
-            sxy +=
-                (xx * yy - xx0 * yy0) - invp * dx * dy - mxx * dy - dx * myy;
-            syy += (yy * yy - yy0 * yy0) - invp * dy * dy - 2 * dy * myy;
-            mxx += dx * invp;
-            myy += dy * invp;
+            vxx += (xx * xx - xx0 * xx0) - inv0 * dx * dx - 2 * dx * mxx;
+            vxy +=
+                (xx * yy - xx0 * yy0) - inv0 * dx * dy - mxx * dy - dx * myy;
+            vyy += (yy * yy - yy0 * yy0) - inv0 * dy * dy - 2 * dy * myy;
+            mxx += dx * inv0;
+            myy += dy * inv0;
             // debug
             // fprintf(stderr,     //
             //     "win_slr2 - wnn=%.0f wii=%.0f xx,yy=%f,%f xx0,yy0=%f,%f\n",
             //     vec99->wnn, vec99->wii, xx, yy, xx0, yy0);
         } else {
             // calculate running slr - welford
             double dd;
-            slr->invp = 1.0 / (slr->nnn + 1);
-            slr->invs = 1.0 / (slr->nnn + 0);
+            slr->inv0 = 1.0 / (slr->nnn + 1);
+            slr->inv1 = 1.0 / (slr->nnn + 0);
+            slr->inv2 = 1.0 / (slr->nnn - 1);
             slr->nnn += 1;
-            // welford - increment syy
+            // welford - increment vyy
             dd = yy - myy;
-            myy += dd * slr->invp;
-            syy += dd * (yy - myy);
-            // welford - increment sxx
+            myy += dd * slr->inv0;
+            vyy += dd * (yy - myy);
+            // welford - increment vxx
             dd = xx - mxx;
-            mxx += dd * slr->invp;
-            sxx += dd * (xx - mxx);
-            // welford - increment sxy
-            sxy += dd * (yy - myy);
+            mxx += dd * slr->inv0;
+            vxx += dd * (xx - mxx);
+            // welford - increment vxy
+            vxy += dd * (yy - myy);
             // debug
             // fprintf(stderr,     //
             //     "win_slr2 - nbody=%.0f xx,yy=%f,%f\n",  //
             //     vec99->nbody, xx, yy);
         }
         slr->mxx = mxx;
         slr->myy = myy;
-        slr->sxx = sxx;
-        slr->sxy = sxy;
-        slr->syy = syy;
+        slr->vxx = vxx;
+        slr->vxy = vxy;
+        slr->vyy = vyy;
         // debug
         // fprintf(stderr, "ii=%d argv0=%f, xx0=%f mxx=%f pp=%p\n",        //
         //     ii, sqlite3_value_double_or_nan(argv[0]), slr->xx0, slr->mxx,
         //     slr);
         // increment counter
         argv += 2;
         slr += 1;
```

### Comparing `sqlmath-2023.6.26/sqlmath_browser.mjs` & `sqlmath-2023.7.21/sqlmath_browser.mjs`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,15 @@
     JOIN (SELECT MIN(ydate) AS __ydate FROM tradebot_intraday_day)
     JOIN (
         SELECT
             MAX(ydate) AS ydate
         FROM tradebot_historical
         JOIN tradebot_state
         WHERE
-            sym = 'spy'
+            sym = '.spx'
             AND ydate < datemkt0
     ) USING (ydate);
 
 -- table - tradebot_intraday_week - insert
 DROP TABLE IF EXISTS tradebot_intraday_week;
 CREATE TABLE tradebot_intraday_week AS
     SELECT
@@ -535,31 +535,31 @@
     --
     SELECT '2e_sqq_lms', ydate, sqq_lms FROM tradebot_intraday_lmt
     --
     UNION ALL
     --
     SELECT '2f_sqq_pnl', ydate, sqq_pnl FROM tradebot_intraday_lmt;
 
--- table - tradebot_technical_week - insert - spy
+-- table - tradebot_technical_week - insert - .spx
 INSERT INTO tradebot_technical_week
     SELECT
-        '1a_spy' AS tname,
+        '1a_spx' AS tname,
         ydate AS tt,
         price
     FROM tradebot_intraday_day
     WHERE
-        sym = 'spy';
+        sym = '.spx';
 INSERT OR IGNORE INTO tradebot_technical_week
     SELECT
-        '1a_spy' AS tname,
+        '1a_spx' AS tname,
         ydate AS tt,
         price
     FROM tradebot_intraday_week
     WHERE
-        sym = 'spy';
+        sym = '.spx';
 
 -- table - tradebot_technical_day - insert
 DROP TABLE IF EXISTS tradebot_technical_day;
 CREATE table tradebot_technical_day AS
     SELECT
         tradebot_technical_week.*
     FROM tradebot_state
@@ -643,26 +643,26 @@
         'options' AS datatype,
         '${JSON.stringify(optionDict)}' AS options;
 INSERT INTO ${tableChart} (datatype, options, series_index, series_label)
     SELECT
         'series_label' AS datatype,
         JSON_OBJECT(
             'isDummy', is_dummy,
-            'isHidden', sym NOT in ('11_mybot', 'spy', 'dia', 'qqq')
+            'isHidden', sym NOT in ('11_mybot', '.spx', 'dia', 'qqq')
         ) AS options,
         rownum AS series_index,
         sym AS series_label
     FROM (
         SELECT
             sym LIKE '-%' AS is_dummy,
             ROW_NUMBER() OVER (
                 ORDER BY
                     sym = '11_mybot' DESC,
                     sym = '----' DESC,
-                    sym = 'spy' DESC,
+                    sym = '.spx' DESC,
                     sym = 'dia' DESC,
                     sym = 'qqq' DESC,
                     sym = '---- ' DESC,
                     sym
             ) AS rownum,
             sym
         FROM (
@@ -1199,50 +1199,50 @@
                 yvalueSuffix: " %"
             };
             return (`
 -- table - ${tableData} - normalize
 UPDATE ${tableData}
     SET
         tval = (CASE
-            WHEN (tname = '1a_spy') THEN
-                (lmt_eee * 1.0 / spy_eee) * (tval - spy_avg) + lmt_avg
+            WHEN (tname = '1a_spx') THEN
+                (lmt_eee * 1.0 / spx_eee) * (tval - spx_avg) + lmt_avg
             WHEN (tname = '1f_stk_pnl') THEN
                 (lmt_eee * 1.0 / pnl_eee) * (tval - pnl_avg) + lmt_avg
         END)
     FROM (SELECT
     -- __join1
         lmt_avg,
         lmt_eee,
         pnl_avg,
         pnl_eee,
-        spy_avg,
-        spy_eee
+        spx_avg,
+        spx_eee
     FROM (SELECT 0)
     JOIN (SELECT
         MEDIAN(tval) AS lmt_avg,
         STDEV(tval) AS lmt_eee
         FROM ${tableData}
         WHERE tname = '1b_stk_lmt'
     )
     JOIN (SELECT
         MEDIAN(tval) AS pnl_avg,
         STDEV(tval) AS pnl_eee
         FROM ${tableData}
         WHERE tname = '1f_stk_pnl'
     )
     JOIN (SELECT
-        MEDIAN(tval) AS spy_avg,
-        STDEV(tval) AS spy_eee
+        MEDIAN(tval) AS spx_avg,
+        STDEV(tval) AS spx_eee
         FROM ${tableData}
-        WHERE tname = '1a_spy'
+        WHERE tname = '1a_spx'
     )
     --
     ) AS __join1
     WHERE
-        tname IN ('1a_spy', '1f_stk_pnl');
+        tname IN ('1a_spx', '1f_stk_pnl');
 UPDATE ${tableData}
     SET
         tt = UNIXEPOCH(tt),
         tval = ROUNDORZERO(100 * tval, 4);
 
 -- chart - ${tableChart} - create
 DROP TABLE IF EXISTS ${tableChart};
@@ -1260,15 +1260,15 @@
         'options' AS datatype,
         '${JSON.stringify(optionDict)}' AS options;
 
 INSERT INTO ${tableChart} (datatype, options, series_index, series_label)
     SELECT
         'series_label' AS datatype,
         JSON_OBJECT(
-            'isHidden', tname NOT IN ('1a_spy', '1b_stk_lmt', '1c_stk_pct'),
+            'isHidden', tname NOT IN ('1a_spx', '1b_stk_lmt', '1c_stk_pct'),
             'seriesColor', (CASE
             WHEN (tname LIKE '%_lmb' OR tname LIKE '%_lms') THEN
                 '#999'
             ELSE
                 NULL
                 -- (
                 --     '#'
@@ -1329,15 +1329,15 @@
         )
     )
     LEFT JOIN ${tableData} ON tname = series_label AND tt = xx_label;
 DELETE FROM ${tableChart} WHERE datatype = 'xx_label';
 UPDATE ${tableChart}
     SET
         series_label = (CASE
-            WHEN (series_label = '1a_spy') THEN '1a spy change'
+            WHEN (series_label = '1a_spx') THEN '1a .spx change'
             WHEN (series_label = '1b_stk_lmt') THEN '1b stk holding ideal'
             WHEN (series_label = '1c_stk_pct') THEN '1c stk holding actual'
             WHEN (series_label = '1d_stk_lmb') THEN '1d stk holding bracket min'
             WHEN (series_label = '1e_stk_lms') THEN '1e stk holding bracket max'
             WHEN (series_label = '1f_stk_pnl') THEN '1f stk gain'
             WHEN (series_label = '2b_sqq_lmt') THEN '2b sqq holding ideal'
             WHEN (series_label = '2c_sqq_pct') THEN '2c sqq holding actual'
```

### Comparing `sqlmath-2023.6.26/sqlmath_custom.c` & `sqlmath-2023.7.21/sqlmath_custom.c`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/sqlmath_jenks.c` & `sqlmath-2023.7.21/sqlmath_jenks.c`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/sqlmath_wrapper_wasm.js` & `sqlmath-2023.7.21/sqlmath_wrapper_wasm.js`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.6.26/test.mjs` & `sqlmath-2023.7.21/test.mjs`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 // OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 // SOFTWARE.
 
 
 /*jslint beta, node*/
 import jslint from "./jslint.mjs";
 import {
+    SQLITE_WIN_SLR_ELEM_SIZE,
     assertJsonEqual,
     assertNumericalEqual,
     assertOrThrow,
     childProcessSpawn2,
     ciBuildExt,
     dbCloseAsync,
     dbExecAndReturnLastBlobAsync,
@@ -2063,54 +2064,68 @@
                     valIn: JSON.stringify(valIn)
                 },
                 db,
                 sql: (`
 SELECT
         id,
         --
-        ROUND(slr->>(0 + 0), 8) AS nnn1,
-        ROUND(slr->>(0 + 1), 8) AS mxx1,
-        ROUND(slr->>(0 + 2), 8) AS myy1,
-        ROUND(slr->>(0 + 3), 8) AS exx1,
-        ROUND(slr->>(0 + 4), 8) AS eyy1,
-        ROUND(slr->>(0 + 5), 8) AS crr1,
-        ROUND(slr->>(0 + 6), 8) AS cbb1,
-        ROUND(slr->>(0 + 7), 8) AS caa1,
+        ROUND(slr->>(0 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 0), 8) AS nnn1,
+        ROUND(slr->>(0 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 1), 8) AS mxx1,
+        ROUND(slr->>(0 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 2), 8) AS myy1,
+        ROUND(slr->>(0 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 3), 8) AS exx1,
+        ROUND(slr->>(0 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 4), 8) AS eyy1,
+        ROUND(slr->>(0 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 5), 8) AS crr1,
+        ROUND(slr->>(0 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 6), 8) AS cbb1,
+        ROUND(slr->>(0 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 7), 8) AS caa1,
+        ROUND(slr->>(0 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 8), 8) AS cyy1,
+        ROUND(slr->>(0 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 9), 8) AS cee1,
         --
-        ROUND(slr->>(8 + 0), 8) AS nnn2,
-        ROUND(slr->>(8 + 1), 8) AS mxx2,
-        ROUND(slr->>(8 + 2), 8) AS myy2,
-        ROUND(slr->>(8 + 3), 8) AS exx2,
-        ROUND(slr->>(8 + 4), 8) AS eyy2,
-        ROUND(slr->>(8 + 5), 8) AS crr2,
-        ROUND(slr->>(8 + 6), 8) AS cbb2,
-        ROUND(slr->>(8 + 7), 8) AS caa2
+        ROUND(slr->>(9 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 0), 8) AS nnn2,
+        ROUND(slr->>(9 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 1), 8) AS mxx2,
+        ROUND(slr->>(9 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 2), 8) AS myy2,
+        ROUND(slr->>(9 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 3), 8) AS exx2,
+        ROUND(slr->>(9 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 4), 8) AS eyy2,
+        ROUND(slr->>(9 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 5), 8) AS crr2,
+        ROUND(slr->>(9 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 6), 8) AS cbb2,
+        ROUND(slr->>(9 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 7), 8) AS caa2,
+        ROUND(slr->>(9 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 8), 8) AS cyy2,
+        ROUND(slr->>(9 * ${SQLITE_WIN_SLR_ELEM_SIZE} + 9), 8) AS cee2
     FROM (
         SELECT
             id,
             win_slr2(
-                value->>0,
-                value->>1,
-                value->>0,
-                IIF(id = 28, -1, value->>1)
+                value->>0, value->>1,
+                value->>0, value->>1,
+                value->>0, value->>1,
+                value->>0, value->>1,
+                value->>0, value->>1,
+                value->>0, value->>1,
+                value->>0, value->>1,
+                value->>0, value->>1,
+                value->>0, value->>1,
+                value->>0, IIF(id = 28, -1, value->>1)
             ) OVER (
                 ORDER BY NULL ASC
                 ${sqlBetween}
             ) AS slr
         FROM JSON_EAcH($valIn)
     );
                 `)
             });
             valActual = valActual[0].map(function ({
                 caa1,
                 caa2,
                 cbb1,
                 cbb2,
+                cee1,
+                cee2,
                 crr1,
                 crr2,
+                cyy1,
+                cyy2,
                 exx1,
                 exx2,
                 eyy1,
                 eyy2,
                 mxx1,
                 mxx2,
                 myy1,
@@ -2119,25 +2134,29 @@
                 nnn2
             }, ii, list) {
                 let obj1;
                 let obj2;
                 obj1 = {
                     caa: caa1,
                     cbb: cbb1,
+                    cee: cee1,
                     crr: crr1,
+                    cyy: cyy1,
                     exx: exx1,
                     eyy: eyy1,
                     mxx: mxx1,
                     myy: myy1,
                     nnn: nnn1
                 };
                 obj2 = {
                     caa: caa2,
                     cbb: cbb2,
+                    cee: cee2,
                     crr: crr2,
+                    cyy: cyy2,
                     exx: exx2,
                     eyy: eyy2,
                     mxx: mxx2,
                     myy: myy2,
                     nnn: nnn2
                 };
                 if (ii + (bb || 0) + 1 >= list.length) {
@@ -2150,105 +2169,125 @@
             assertJsonEqual(valActual, valExpected);
         }
         noop(test_win_slr2_aggregate);
         valExpected = [
             {
                 "caa": null,
                 "cbb": null,
+                "cee": null,
                 "crr": null,
+                "cyy": null,
                 "exx": null,
                 "eyy": null,
                 "mxx": 2,
                 "myy": 0,
                 "nnn": 1
             },
             {
                 "caa": null,
                 "cbb": null,
+                "cee": null,
                 "crr": null,
+                "cyy": null,
                 "exx": 0,
                 "eyy": 0.70710678,
                 "mxx": 2,
                 "myy": 0.5,
                 "nnn": 2
             },
             {
                 "caa": -4.5,
                 "cbb": 2.5,
+                "cee": 0.70710678,
                 "crr": 0.94491118,
+                "cyy": 3,
                 "exx": 0.57735027,
                 "eyy": 1.52752523,
                 "mxx": 2.33333333,
                 "myy": 1.33333333,
                 "nnn": 3
             },
             {
                 "caa": -3,
                 "cbb": 1.81818182,
+                "cee": 0.67419986,
                 "crr": 0.95346259,
+                "cyy": 4.27272727,
                 "exx": 0.95742711,
                 "eyy": 1.82574186,
                 "mxx": 2.75,
                 "myy": 2,
                 "nnn": 4
             },
             {
                 "caa": -2.29411765,
                 "cbb": 1.52941176,
+                "cee": 0.65678958,
                 "crr": 0.96164474,
+                "cyy": 5.35294118,
                 "exx": 1.30384048,
                 "eyy": 2.07364414,
                 "mxx": 3.2,
                 "myy": 2.6,
                 "nnn": 5
             },
             {
                 "caa": -2.54385965,
                 "cbb": 1.63157895,
+                "cee": 0.62126074,
                 "crr": 0.97080629,
+                "cyy": 5.61403509,
                 "exx": 1.37840488,
                 "eyy": 2.31660671,
                 "mxx": 3.5,
                 "myy": 3.16666667,
                 "nnn": 6
             },
             {
                 "caa": -2.65,
                 "cbb": 1.675,
+                "cee": 0.57445626,
                 "crr": 0.9752227,
+                "cyy": 5.725,
                 "exx": 1.38013112,
                 "eyy": 2.37045304,
                 "mxx": 3.71428571,
                 "myy": 3.57142857,
                 "nnn": 7
             },
             {
                 "caa": -2.5,
                 "cbb": 1.625,
+                "cee": 0.54006172,
                 "crr": 0.97991187,
+                "cyy": 7.25,
                 "exx": 1.51185789,
                 "eyy": 2.50713268,
                 "mxx": 4,
                 "myy": 4,
                 "nnn": 8
             },
             {
                 "caa": 0.75,
                 "cbb": 0.85,
+                "cee": 1.08781126,
                 "crr": 0.89597867,
+                "cyy": 9.25,
                 "exx": 2.39045722,
                 "eyy": 2.26778684,
                 "mxx": 5,
                 "myy": 5,
                 "nnn": 8
             },
             {
                 "caa": 2.75,
                 "cbb": 0.55,
+                "cee": 0.99163165,
                 "crr": 0.81989159,
+                "cyy": 3.85,
                 "exx": 2.39045722,
                 "eyy": 1.60356745,
                 "mxx": 5,
                 "myy": 5.5,
                 "nnn": 8
             }
         ];
@@ -2310,35 +2349,82 @@
                         10, // nnn
                         4.4, // mxx
                         4.5, // myy
                         2.45854519, // exx
                         2.54950976, // eyy
                         0.81541829, // crr
                         0.84558824, // cbb
-                        0.77941176 // caa
+                        0.77941176, // caa
+                        2.47058824, // cyy
+                        1.56536502 // cee
                     ]
                 );
             }()),
             // test win_slr2-aggregate-window handling-behavior
             test_win_slr2_aggregate({
                 aa: 8,
                 bb: 0,
                 valExpected,
                 valExpected2: {
                     caa: -0.25,
                     cbb: 1,
+                    cee: 1.60727513,
                     crr: 0.84895272,
+                    cyy: 1.75,
                     exx: 2.39045722,
                     eyy: 2.81577191,
                     mxx: 5,
                     myy: 4.75,
                     nnn: 8
                 }
             })
         ]);
+        valActual = {
+            "caa": -0.820256776034237,
+            "cbb": 0.146219686162625,
+            "cee": 2.74202903932406,
+            "crr": 0.865664999629448,
+            "cyy": 6.63694721825963,
+            "exx": 29.003448070876,
+            "eyy": 4.89897948556636,
+            "mxx": 74,
+            "myy": 10,
+            "nnn": 6
+        };
+        valExpected = noop(
+            await dbExecAsync({
+                db,
+                sql: (`
+SELECT
+        __slr->>0 AS nnn,
+        __slr->>1 AS mxx,
+        __slr->>2 AS myy,
+        __slr->>3 AS exx,
+        __slr->>4 AS eyy,
+        __slr->>5 AS crr,
+        __slr->>6 AS cbb,
+        __slr->>7 AS caa,
+        __slr->>8 AS cyy,
+        __slr->>9 AS cee
+    FROM (
+        SELECT
+            win_slr2(xx, yy) AS __slr
+        FROM (
+            SELECT 34 AS xx, 5 AS yy
+            UNION ALL SELECT 108, 17
+            UNION ALL SELECT 64, 11
+            UNION ALL SELECT 88, 8
+            UNION ALL SELECT 99, 14
+            UNION ALL SELECT 51, 5
+        )
+    )
+                `)
+            })
+        )[0][0];
+        assertJsonEqual(valActual, valExpected);
     });
 });
 
 jstestDescribe((
     "test_sqlmathWebworkerInit"
 ), function test_sqlmathWebworkerInit() {
     jstestIt((
```

