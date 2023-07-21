# Comparing `tmp/pydal2sql-0.3.1.tar.gz` & `tmp/pydal2sql-0.4.0.tar.gz`

## Comparing `pydal2sql-0.3.1.tar` & `pydal2sql-0.4.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/coverage.svg
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/.github/workflows/su6.yml
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/examples/examples.sh
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/examples/magic.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/examples/settings_in_code.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/examples/settings_via_cli.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74___about___py.html
--rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74___init___py.html
--rw-r--r--   0        0        0    49364 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html
--rw-r--r--   0        0        0    27150 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_core_py.html
--rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html
--rw-r--r--   0        0        0    45751 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html
--rw-r--r--   0        0        0     7967 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_types_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/style.css
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/src/pydal2sql/__about__.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/src/pydal2sql/__init__.py
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/src/pydal2sql/cli.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/src/pydal2sql/core.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/src/pydal2sql/helpers.py
--rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/src/pydal2sql/magic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/src/pydal2sql/py.typed
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/src/pydal2sql/types.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/tests/test_cli.py
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/tests/test_core.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/tests/test_helpers.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/LICENSE.txt
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/README.md
--rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/coverage.svg
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/.github/workflows/su6.yml
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/examples/examples.sh
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/examples/magic.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/examples/settings_in_code.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/examples/settings_via_cli.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/htmlcov/d_8bc7b9c2c0d01e74___about___py.html
+-rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/htmlcov/d_8bc7b9c2c0d01e74___init___py.html
+-rw-r--r--   0        0        0    66547 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html
+-rw-r--r--   0        0        0    27150 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/htmlcov/d_8bc7b9c2c0d01e74_core_py.html
+-rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html
+-rw-r--r--   0        0        0    49372 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html
+-rw-r--r--   0        0        0     7967 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/htmlcov/d_8bc7b9c2c0d01e74_types_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/htmlcov/style.css
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/src/pydal2sql/__about__.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/src/pydal2sql/__init__.py
+-rw-r--r--   0        0        0     7059 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/src/pydal2sql/cli.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/src/pydal2sql/core.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/src/pydal2sql/helpers.py
+-rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/src/pydal2sql/magic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/src/pydal2sql/py.typed
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/src/pydal2sql/types.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/tests/test_core.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/tests/test_helpers.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/README.md
+-rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5133 2020-02-02 00:00:00.000000 pydal2sql-0.4.0/PKG-INFO
```

### Comparing `pydal2sql-0.3.1/CHANGELOG.md` & `pydal2sql-0.4.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.4.0 (2023-07-21)
+
+### Feature
+
+* **cli:** Use `tool.pydal2sql` in pyproject.toml to set default settings (which can normally be set with cli flags) ([`9c67f34`](https://github.com/robinvandernoord/pydal2sql/commit/9c67f3465a896f95c465ffcbeb51f90c84eb0291))
+
 ## v0.3.1 (2023-07-20)
 
 ### Documentation
 
 * **readme:** Add another video ([`ce4312d`](https://github.com/robinvandernoord/pydal2sql/commit/ce4312deb4e9ef6b9261971214d88afc3c431345))
 
 ## v0.3.0 (2023-07-20)
```

### Comparing `pydal2sql-0.3.1/coverage.svg` & `pydal2sql-0.4.0/coverage.svg`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.1/htmlcov/coverage_html.js` & `pydal2sql-0.4.0/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74___about___py.html` & `pydal2sql-0.4.0/htmlcov/d_8bc7b9c2c0d01e74___about___py.html`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 20:23 +0200
+            created at 2023-07-21 11:06 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -83,23 +83,23 @@
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Stores the version.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="com"># SPDX-FileCopyrightText: 2023-present Robin van der Noord &lt;robinvandernoord@gmail.com></span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.2.4"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.3.1"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 20:23 +0200
+            created at 2023-07-21 11:06 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,22 +7,22 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 1 statements   1 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-20 20:23 +0200
+at 2023-07-21 11:06 +0200
 
 
 1""" 
 2Stores the version. 
 3""" 
 4 
 5# SPDX-FileCopyrightText: 2023-present Robin van der Noord
 <robinvandernoord@gmail.com> 
 6# 
 7# SPDX-License-Identifier: MIT 
-8__version__ = "0.2.4" 
+8__version__ = "0.3.1" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-20 20:23 +0200
+at 2023-07-21 11:06 +0200
```

### Comparing `pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74___init___py.html` & `pydal2sql-0.4.0/htmlcov/d_8bc7b9c2c0d01e74___init___py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html` & `pydal2sql-0.4.0/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/pydal2sql/cli.py: 100%</title>
+    <title>Coverage for src/pydal2sql/magic.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/pydal2sql/cli.py</b>:
+            <span class="text">Coverage for </span><b>src/pydal2sql/magic.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">28 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">28<span class="text"> run</span></button>
+            <span class="text">60 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">60<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
-            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">29<span class="text"> excluded</span></button>
+            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_8bc7b9c2c0d01e74___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_8bc7b9c2c0d01e74_helpers_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74_core_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74_types_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 20:24 +0200
+            created at 2023-07-21 11:14 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -77,202 +77,199 @@
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">CLI tool to generate SQL from PyDAL code.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">This file has methods to guess which variables are unknown and to potentially (monkey-patch) fix this.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">argparse</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">pathlib</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">import</span> <span class="nam">select</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">string</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">import</span> <span class="nam">textwrap</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">IO</span><span class="op">,</span> <span class="nam">Optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">ast</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">builtins</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">import</span> <span class="nam">importlib</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">textwrap</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="nam">BUILTINS</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="nam">builtins</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">import</span> <span class="nam">rich</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">from</span> <span class="nam">rich</span><span class="op">.</span><span class="nam">prompt</span> <span class="key">import</span> <span class="nam">Prompt</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">flatten</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">magic</span> <span class="key">import</span> <span class="nam">find_missing_variables</span><span class="op">,</span> <span class="nam">generate_magic_code</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="key">class</span> <span class="nam">PrettyParser</span><span class="op">(</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">ArgumentParser</span><span class="op">)</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="str">    Add 'rich' to the argparse output.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="key">def</span> <span class="nam">_print_message</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">message</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">file</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">IO</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="nam">message</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">file</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="key">def</span> <span class="nam">has_stdin_data</span><span class="op">(</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="str">    Check if the program starts with cli data (pipe | or redirect >&lt;).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">def</span> <span class="nam">traverse_ast</span><span class="op">(</span><span class="nam">node</span><span class="op">:</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">AST</span><span class="op">,</span> <span class="nam">variable_collector</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Callable</span><span class="op">[</span><span class="op">[</span><span class="nam">ast</span><span class="op">.</span><span class="nam">AST</span><span class="op">]</span><span class="op">,</span> <span class="key">None</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="str">    Calls variable_collector on each node recursively.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="nam">variable_collector</span><span class="op">(</span><span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="key">for</span> <span class="nam">child</span> <span class="key">in</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">iter_child_nodes</span><span class="op">(</span><span class="nam">node</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="nam">traverse_ast</span><span class="op">(</span><span class="nam">child</span><span class="op">,</span> <span class="nam">variable_collector</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="key">def</span> <span class="nam">find_missing_variables</span><span class="op">(</span><span class="nam">code_str</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">set</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">    Look through the source code in code_str and try to detect using ast parsing which variables are undefined.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="com"># Partly made by ChatGPT</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="nam">code_str</span> <span class="op">=</span> <span class="nam">textwrap</span><span class="op">.</span><span class="nam">dedent</span><span class="op">(</span><span class="nam">code_str</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="com"># could raise SyntaxError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="nam">tree</span><span class="op">:</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Module</span> <span class="op">=</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">parse</span><span class="op">(</span><span class="nam">code_str</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="str">    See Also:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t"><span class="str">        https://stackoverflow.com/questions/3762881/how-do-i-check-if-stdin-has-some-data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="key">return</span> <span class="nam">any</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">        <span class="nam">select</span><span class="op">.</span><span class="nam">select</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">            <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">                <span class="nam">sys</span><span class="op">.</span><span class="nam">stdin</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">            <span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">            <span class="op">[</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">            <span class="op">[</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">            <span class="num">0.0</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="op">)</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="nam">used_variables</span><span class="op">:</span> <span class="nam">set</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="nam">defined_variables</span><span class="op">:</span> <span class="nam">set</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="nam">imported_modules</span><span class="op">:</span> <span class="nam">set</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="nam">imported_names</span><span class="op">:</span> <span class="nam">set</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="nam">loop_variables</span><span class="op">:</span> <span class="nam">set</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="key">def</span> <span class="nam">collect_variables</span><span class="op">(</span><span class="nam">node</span><span class="op">:</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">AST</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Name</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">            <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">ctx</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Load</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">                <span class="nam">used_variables</span><span class="op">.</span><span class="nam">add</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">            <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">ctx</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">                <span class="nam">defined_variables</span><span class="op">.</span><span class="nam">add</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">            <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">ctx</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Del</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">                <span class="nam">defined_variables</span><span class="op">.</span><span class="nam">discard</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="key">def</span> <span class="nam">handle_cli</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="nam">code</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="nam">db_type</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">    <span class="nam">tables</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="nam">verbose</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="nam">noop</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="nam">magic</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t"><span class="str">    Handle user input.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">    <span class="nam">to_execute</span> <span class="op">=</span> <span class="nam">string</span><span class="op">.</span><span class="nam">Template</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">        <span class="nam">textwrap</span><span class="op">.</span><span class="nam">dedent</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">            <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t"><span class="str">        from pydal import *</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t"><span class="str">        from pydal.objects import *</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t"><span class="str">        from pydal.validators import *</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="key">def</span> <span class="nam">collect_definitions</span><span class="op">(</span><span class="nam">node</span><span class="op">:</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">AST</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Assign</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">            <span class="nam">node_targets</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">list</span><span class="op">[</span><span class="nam">ast</span><span class="op">.</span><span class="nam">Name</span><span class="op">]</span><span class="op">,</span> <span class="nam">node</span><span class="op">.</span><span class="nam">targets</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">            <span class="nam">defined_variables</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">target</span><span class="op">.</span><span class="nam">id</span> <span class="key">for</span> <span class="nam">target</span> <span class="key">in</span> <span class="nam">node_targets</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="key">def</span> <span class="nam">collect_imports</span><span class="op">(</span><span class="nam">node</span><span class="op">:</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">AST</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Import</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">            <span class="key">for</span> <span class="nam">alias</span> <span class="key">in</span> <span class="nam">node</span><span class="op">.</span><span class="nam">names</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">                <span class="nam">imported_names</span><span class="op">.</span><span class="nam">add</span><span class="op">(</span><span class="nam">alias</span><span class="op">.</span><span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">ImportFrom</span><span class="op">)</span> <span class="key">and</span> <span class="nam">node</span><span class="op">.</span><span class="nam">module</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">            <span class="nam">module_name</span> <span class="op">=</span> <span class="nam">node</span><span class="op">.</span><span class="nam">module</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">            <span class="nam">imported_module</span> <span class="op">=</span> <span class="nam">importlib</span><span class="op">.</span><span class="nam">import_module</span><span class="op">(</span><span class="nam">module_name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">            <span class="key">if</span> <span class="nam">node</span><span class="op">.</span><span class="nam">names</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">.</span><span class="nam">name</span> <span class="op">==</span> <span class="str">"*"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">                <span class="nam">imported_names</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">name</span> <span class="key">for</span> <span class="nam">name</span> <span class="key">in</span> <span class="nam">dir</span><span class="op">(</span><span class="nam">imported_module</span><span class="op">)</span> <span class="key">if</span> <span class="key">not</span> <span class="nam">name</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">                <span class="nam">imported_names</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">alias</span><span class="op">.</span><span class="nam">asname</span> <span class="key">or</span> <span class="nam">alias</span><span class="op">.</span><span class="nam">name</span> <span class="key">for</span> <span class="nam">alias</span> <span class="key">in</span> <span class="nam">node</span><span class="op">.</span><span class="nam">names</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t"><span class="str">        from pydal2sql import generate_sql</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t"><span class="str">        db = database = DAL(None, migrate=False)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t"><span class="str">        tables = $tables</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t"><span class="str">        db_type = '$db_type'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t"><span class="str">        $extra</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">    <span class="key">def</span> <span class="nam">collect_imported_names</span><span class="op">(</span><span class="nam">node</span><span class="op">:</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">AST</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">        <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">ImportFrom</span><span class="op">)</span> <span class="key">and</span> <span class="nam">node</span><span class="op">.</span><span class="nam">module</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">            <span class="key">for</span> <span class="nam">alias</span> <span class="key">in</span> <span class="nam">node</span><span class="op">.</span><span class="nam">names</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">                <span class="nam">imported_names</span><span class="op">.</span><span class="nam">add</span><span class="op">(</span><span class="nam">alias</span><span class="op">.</span><span class="nam">asname</span> <span class="key">or</span> <span class="nam">alias</span><span class="op">.</span><span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">    <span class="key">def</span> <span class="nam">collect_loop_variables</span><span class="op">(</span><span class="nam">node</span><span class="op">:</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">AST</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">For</span><span class="op">)</span> <span class="key">and</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">target</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Name</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">            <span class="nam">loop_variables</span><span class="op">.</span><span class="nam">add</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">target</span><span class="op">.</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t"><span class="str">        $code</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t"><span class="str">        if not tables:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t"><span class="str">            tables = db._tables</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t"><span class="str">        for table in tables:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t"><span class="str">            print(generate_sql(db[table], db_type))</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="nam">generated_code</span> <span class="op">=</span> <span class="nam">to_execute</span><span class="op">.</span><span class="nam">substitute</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">        <span class="op">{</span><span class="str">"tables"</span><span class="op">:</span> <span class="nam">flatten</span><span class="op">(</span><span class="nam">tables</span> <span class="key">or</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">,</span> <span class="str">"db_type"</span><span class="op">:</span> <span class="nam">db_type</span> <span class="key">or</span> <span class="str">""</span><span class="op">,</span> <span class="str">"code"</span><span class="op">:</span> <span class="nam">textwrap</span><span class="op">.</span><span class="nam">dedent</span><span class="op">(</span><span class="nam">code</span><span class="op">)</span><span class="op">,</span> <span class="str">"extra"</span><span class="op">:</span> <span class="str">""</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="key">if</span> <span class="nam">verbose</span> <span class="key">or</span> <span class="nam">noop</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="nam">generated_code</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">noop</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">        <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">            <span class="nam">exec</span><span class="op">(</span><span class="nam">generated_code</span><span class="op">)</span>  <span class="com"># nosec: B102</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="key">except</span> <span class="nam">NameError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">            <span class="com"># something is missing!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">            <span class="nam">missing_vars</span> <span class="op">=</span> <span class="nam">find_missing_variables</span><span class="op">(</span><span class="nam">generated_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">            <span class="key">if</span> <span class="key">not</span> <span class="nam">magic</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">                <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">                    <span class="str">f"Your code is missing some variables: {missing_vars}. Add these or try --magic"</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">                <span class="nam">extra_code</span> <span class="op">=</span> <span class="nam">generate_magic_code</span><span class="op">(</span><span class="nam">missing_vars</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">                <span class="nam">generated_code</span> <span class="op">=</span> <span class="nam">to_execute</span><span class="op">.</span><span class="nam">substitute</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">                    <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">                        <span class="str">"tables"</span><span class="op">:</span> <span class="nam">flatten</span><span class="op">(</span><span class="nam">tables</span> <span class="key">or</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">                        <span class="str">"db_type"</span><span class="op">:</span> <span class="nam">db_type</span> <span class="key">or</span> <span class="str">""</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">                        <span class="str">"extra"</span><span class="op">:</span> <span class="nam">extra_code</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">                        <span class="str">"code"</span><span class="op">:</span> <span class="nam">textwrap</span><span class="op">.</span><span class="nam">dedent</span><span class="op">(</span><span class="nam">code</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">                    <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">                <span class="key">if</span> <span class="nam">verbose</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">                    <span class="nam">print</span><span class="op">(</span><span class="nam">generated_code</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">                <span class="nam">exec</span><span class="op">(</span><span class="nam">generated_code</span><span class="op">)</span>  <span class="com"># nosec: B102</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t"><span class="key">def</span> <span class="nam">app</span><span class="op">(</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t"><span class="str">    Entrypoint for the pydal2sql cli command.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">    <span class="nam">parser</span> <span class="op">=</span> <span class="nam">PrettyParser</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="nam">prog</span><span class="op">=</span><span class="str">"pydal2sql"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">        <span class="nam">formatter_class</span><span class="op">=</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">RawDescriptionHelpFormatter</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="nam">description</span><span class="op">=</span><span class="str">"""[green]CLI tool to generate SQL from PyDAL code.[/green]\n</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t"><span class="str">        Aside from using cli arguments, you can also configure the tool in your code.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t"><span class="str">        You can set the following variables:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t"><span class="str">        db_type: str = 'sqlite' # your desired database type;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t"><span class="str">        tables: list[str] = []  # your desired tables to generate SQL for;"""</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">        <span class="nam">epilog</span><span class="op">=</span><span class="str">"Example: [i]cat models.py | pydal2sql sqlite[/i]"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span><span class="str">"filename"</span><span class="op">,</span> <span class="nam">nargs</span><span class="op">=</span><span class="str">"?"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Which file to load? Can also be done with stdin."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">        <span class="str">"db_type"</span><span class="op">,</span> <span class="nam">nargs</span><span class="op">=</span><span class="str">"?"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Which database dialect to generate ([blue]postgres, sqlite, mysql[/blue])"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">    <span class="key">def</span> <span class="nam">collect_everything</span><span class="op">(</span><span class="nam">node</span><span class="op">:</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">AST</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">        <span class="nam">collect_variables</span><span class="op">(</span><span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="nam">collect_definitions</span><span class="op">(</span><span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">        <span class="nam">collect_imported_names</span><span class="op">(</span><span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">        <span class="nam">collect_imports</span><span class="op">(</span><span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">        <span class="nam">collect_loop_variables</span><span class="op">(</span><span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">    <span class="com"># ChatGPT produced (4.20s for 10k):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="com"># traverse_ast(tree, collect_variables)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">    <span class="com"># traverse_ast(tree, collect_definitions)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">    <span class="com"># traverse_ast(tree, collect_imported_names)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="com"># traverse_ast(tree, collect_imports)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">    <span class="com"># traverse_ast(tree, collect_loop_variables)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="com"># manually rewritten (2.19s for 10k):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">    <span class="nam">traverse_ast</span><span class="op">(</span><span class="nam">tree</span><span class="op">,</span> <span class="nam">collect_everything</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">        <span class="nam">var</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">        <span class="key">for</span> <span class="nam">var</span> <span class="key">in</span> <span class="nam">used_variables</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">        <span class="key">if</span> <span class="nam">var</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">defined_variables</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="key">and</span> <span class="nam">var</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">imported_modules</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">        <span class="key">and</span> <span class="nam">var</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">loop_variables</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">        <span class="key">and</span> <span class="nam">var</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">imported_names</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="key">and</span> <span class="nam">var</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">BUILTINS</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">    <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t"><span class="com"># if __name__ == "__main__":</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t"><span class="com">#     # Example usage:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t"><span class="com">#     code_string = """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t"><span class="com">#     from math import floor</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t"><span class="com">#     import datetime</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="com">#     from pydal import DAL</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t"><span class="com">#     a = 1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t"><span class="com">#     b = 2</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t"><span class="com">#     print(a, b + c)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t"><span class="com">#     d = e + b</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t"><span class="com">#     xyz</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t"><span class="com">#     floor(d)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t"><span class="com">#     ceil(d)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t"><span class="com">#     ceil(e)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t"><span class="com">#     datetime.utcnow()</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t"><span class="com">#     db = DAL()</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t"><span class="com">#     db.define_table('...')</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t"><span class="com">#     for table in []:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t"><span class="com">#         print(table)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t"><span class="com">#     if toble := True:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t"><span class="com">#         print(toble)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t"><span class="com">#     """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t"><span class="com">#     # import timeit</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t"><span class="com">#     #</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t"><span class="com">#     # print(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t"><span class="com">#     #     timeit.timeit(lambda: find_missing_variables(code_string), number=10000)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t"><span class="com">#     #</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t"><span class="com">#     #</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t"><span class="com">#     # )</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t"><span class="com">#     missing_variables = find_missing_variables(code_string)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t"><span class="com">#     assert missing_variables == {"c", "xyz", "ceil", "e"}, missing_variables</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span><span class="str">"--verbose"</span><span class="op">,</span> <span class="str">"-v"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Show more info"</span><span class="op">,</span> <span class="nam">action</span><span class="op">=</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">BooleanOptionalAction</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">False</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">        <span class="str">"--noop"</span><span class="op">,</span> <span class="str">"-n"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Only show code, don't run it."</span><span class="op">,</span> <span class="nam">action</span><span class="op">=</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">BooleanOptionalAction</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">        <span class="str">"--magic"</span><span class="op">,</span> <span class="str">"-m"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Perform magic to fix missing vars."</span><span class="op">,</span> <span class="nam">action</span><span class="op">=</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">BooleanOptionalAction</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">        <span class="str">"-t"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">        <span class="str">"--table"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">        <span class="str">"--tables"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">        <span class="nam">action</span><span class="op">=</span><span class="str">"append"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">        <span class="nam">nargs</span><span class="op">=</span><span class="str">"+"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">        <span class="nam">help</span><span class="op">=</span><span class="str">"One or more tables to generate. By default, all tables in the file will be used."</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">    <span class="nam">args</span> <span class="op">=</span> <span class="nam">parser</span><span class="op">.</span><span class="nam">parse_args</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">    <span class="nam">db_type</span> <span class="op">=</span> <span class="nam">args</span><span class="op">.</span><span class="nam">db_type</span> <span class="key">or</span> <span class="nam">args</span><span class="op">.</span><span class="nam">filename</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t"><span class="key">def</span> <span class="nam">generate_magic_code</span><span class="op">(</span><span class="nam">missing_vars</span><span class="op">:</span> <span class="nam">set</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t"><span class="str">    After finding missing vars, fill them in with an object that does nothing except return itself or an empty string.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t"><span class="str">    This way, it's least likely to crash (when used as default or validator in pydal, don't use this for running code!).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">    <span class="nam">extra_code</span> <span class="op">=</span> <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t"><span class="str">        class Empty:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t"><span class="str">            # class that does absolutely nothing</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t"><span class="str">            # but can be accessed like an object (obj.something.whatever)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t"><span class="str">            # or a dict[with][some][keys]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t"><span class="str">            def __getattribute__(self, _):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t"><span class="str">                return self</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t"><span class="str">            def __getitem__(self, _):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t"><span class="str">                return self</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t"><span class="str">            def __get__(self):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t"><span class="str">                return self</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t"><span class="str">            def __call__(self, *_):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t"><span class="str">                return self</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">    <span class="nam">load_file_mode</span> <span class="op">=</span> <span class="op">(</span><span class="nam">filename</span> <span class="op">:=</span> <span class="nam">args</span><span class="op">.</span><span class="nam">filename</span><span class="op">)</span> <span class="key">and</span> <span class="nam">filename</span><span class="op">.</span><span class="nam">endswith</span><span class="op">(</span><span class="str">".py"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="op">(</span><span class="nam">has_stdin_data</span><span class="op">(</span><span class="op">)</span> <span class="key">or</span> <span class="nam">load_file_mode</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">db_type</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">            <span class="nam">db_type</span> <span class="op">=</span> <span class="nam">Prompt</span><span class="op">.</span><span class="nam">ask</span><span class="op">(</span><span class="str">"Which database type do you want to use?"</span><span class="op">,</span> <span class="nam">choices</span><span class="op">=</span><span class="op">[</span><span class="str">"sqlite"</span><span class="op">,</span> <span class="str">"postgres"</span><span class="op">,</span> <span class="str">"mysql"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t"><span class="str">            def __str__(self):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t"><span class="str">                return ''</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t"><span class="str">            def __repr__(self):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t"><span class="str">                return ''</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">"Please paste your define tables code below and press ctrl-D when finished."</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">    <span class="com"># else: data from stdin</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">    <span class="com"># py code or cli args should define settings.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">    <span class="key">if</span> <span class="nam">load_file_mode</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">        <span class="nam">db_type</span> <span class="op">=</span> <span class="nam">args</span><span class="op">.</span><span class="nam">db_type</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">        <span class="nam">text</span> <span class="op">=</span> <span class="nam">pathlib</span><span class="op">.</span><span class="nam">Path</span><span class="op">(</span><span class="nam">filename</span><span class="op">)</span><span class="op">.</span><span class="nam">read_text</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">        <span class="nam">text</span> <span class="op">=</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">stdin</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">    <span class="key">return</span> <span class="nam">handle_cli</span><span class="op">(</span><span class="nam">text</span><span class="op">,</span> <span class="nam">db_type</span><span class="op">,</span> <span class="nam">args</span><span class="op">.</span><span class="nam">table</span><span class="op">,</span> <span class="nam">verbose</span><span class="op">=</span><span class="nam">args</span><span class="op">.</span><span class="nam">verbose</span><span class="op">,</span> <span class="nam">noop</span><span class="op">=</span><span class="nam">args</span><span class="op">.</span><span class="nam">noop</span><span class="op">,</span> <span class="nam">magic</span><span class="op">=</span><span class="nam">args</span><span class="op">.</span><span class="nam">magic</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t"><span class="str">        # todo: overload more methods</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t"><span class="str">        empty = Empty()</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t"><span class="str">            \n</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">    <span class="key">for</span> <span class="nam">variable</span> <span class="key">in</span> <span class="nam">missing_vars</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">        <span class="nam">extra_code</span> <span class="op">+=</span> <span class="str">f"{variable} = empty; "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">    <span class="key">return</span> <span class="nam">textwrap</span><span class="op">.</span><span class="nam">dedent</span><span class="op">(</span><span class="nam">extra_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_8bc7b9c2c0d01e74___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_8bc7b9c2c0d01e74_helpers_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74_core_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74_types_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 20:24 +0200
+            created at 2023-07-21 11:14 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,214 +1,204 @@
 
-****** Coverage for src/pydal2sql/cli.py: 100% ******
+****** Coverage for src/pydal2sql/magic.py: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 28 statements   28 run 0 missing 29 excluded *****
+***** 60 statements   60 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-20 20:24 +0200
+at 2023-07-21 11:14 +0200
 
 
 1""" 
-2CLI tool to generate SQL from PyDAL code. 
+2This file has methods to guess which variables are unknown and to potentially
+(monkey-patch) fix this. 
 3""" 
 4 
-5import argparse 
-6import pathlib 
-7import select 
-8import string 
-9import sys 
-10import textwrap 
-11from typing import IO, Optional 
+5import ast 
+6import builtins 
+7import importlib 
+8import textwrap 
+9import typing 
+10 
+11BUILTINS = set(builtins.__dict__.keys()) 
 12 
-13import rich 
-14from rich.prompt import Prompt 
-15 
-16from .helpers import flatten 
-17from .magic import find_missing_variables, generate_magic_code 
-18 
-19 
-20class PrettyParser(argparse.ArgumentParser): # pragma: no cover 
-21 """ 
-22 Add 'rich' to the argparse output. 
-23 """ 
-24 
-25 def _print_message(self, message: str, file: Optional[IO[str]] = None) -
-> None: 
-26 rich.print(message, file=file) 
-27 
-28 
-29def has_stdin_data() -> bool: # pragma: no cover 
-30 """ 
-31 Check if the program starts with cli data (pipe | or redirect ><). 
+13 
+14def traverse_ast(node: ast.AST, variable_collector: typing.Callable[
+[ast.AST], None]) -> None: 
+15 """ 
+16 Calls variable_collector on each node recursively. 
+17 """ 
+18 variable_collector(node) 
+19 for child in ast.iter_child_nodes(node): 
+20 traverse_ast(child, variable_collector) 
+21 
+22 
+23def find_missing_variables(code_str: str) -> set[str]: 
+24 """ 
+25 Look through the source code in code_str and try to detect using ast parsing
+which variables are undefined. 
+26 """ 
+27 # Partly made by ChatGPT 
+28 code_str = textwrap.dedent(code_str) 
+29 
+30 # could raise SyntaxError 
+31 tree: ast.Module = ast.parse(code_str) 
 32 
-33 See Also: 
-34 https://stackoverflow.com/questions/3762881/how-do-i-check-if-stdin-has-
-some-data 
-35 """ 
-36 return any( 
-37 select.select( 
-38 [ 
-39 sys.stdin, 
-40 ], 
-41 [], 
-42 [], 
-43 0.0, 
-44 )[0] 
-45 ) 
-46 
+33 used_variables: set[str] = set() 
+34 defined_variables: set[str] = set() 
+35 imported_modules: set[str] = set() 
+36 imported_names: set[str] = set() 
+37 loop_variables: set[str] = set() 
+38 
+39 def collect_variables(node: ast.AST) -> None: 
+40 if isinstance(node, ast.Name): 
+41 if isinstance(node.ctx, ast.Load): 
+42 used_variables.add(node.id) 
+43 elif isinstance(node.ctx, ast.Store): 
+44 defined_variables.add(node.id) 
+45 elif isinstance(node.ctx, ast.Del): 
+46 defined_variables.discard(node.id) 
 47 
-48def handle_cli( 
-49 code: str, 
-50 db_type: str = None, 
-51 tables: list[list[str]] = None, 
-52 verbose: bool = False, 
-53 noop: bool = False, 
-54 magic: bool = False, 
-55) -> None: 
-56 """ 
-57 Handle user input. 
-58 """ 
-59 to_execute = string.Template( 
-60 textwrap.dedent( 
-61 """ 
-62 from pydal import * 
-63 from pydal.objects import * 
-64 from pydal.validators import * 
+48 def collect_definitions(node: ast.AST) -> None: 
+49 if isinstance(node, ast.Assign): 
+50 node_targets = typing.cast(list[ast.Name], node.targets) 
+51 
+52 defined_variables.update(target.id for target in node_targets) 
+53 
+54 def collect_imports(node: ast.AST) -> None: 
+55 if isinstance(node, ast.Import): 
+56 for alias in node.names: 
+57 imported_names.add(alias.name) 
+58 elif isinstance(node, ast.ImportFrom) and node.module: 
+59 module_name = node.module 
+60 imported_module = importlib.import_module(module_name) 
+61 if node.names[0].name == "*": 
+62 imported_names.update(name for name in dir(imported_module) if not
+name.startswith("_")) 
+63 else: 
+64 imported_names.update(alias.asname or alias.name for alias in node.names) 
 65 
-66 from pydal2sql import generate_sql 
-67 
-68 db = database = DAL(None, migrate=False) 
-69 
-70 tables = $tables 
-71 db_type = '$db_type' 
-72 
-73 $extra 
+66 def collect_imported_names(node: ast.AST) -> None: 
+67 if isinstance(node, ast.ImportFrom) and node.module: 
+68 for alias in node.names: 
+69 imported_names.add(alias.asname or alias.name) 
+70 
+71 def collect_loop_variables(node: ast.AST) -> None: 
+72 if isinstance(node, ast.For) and isinstance(node.target, ast.Name): 
+73 loop_variables.add(node.target.id) 
 74 
-75 $code 
-76 
-77 if not tables: 
-78 tables = db._tables 
-79 
-80 for table in tables: 
-81 print(generate_sql(db[table], db_type)) 
-82 """ 
-83 ) 
-84 ) 
-85 
-86 generated_code = to_execute.substitute( 
-87 {"tables": flatten(tables or []), "db_type": db_type or "", "code":
-textwrap.dedent(code), "extra": ""} 
-88 ) 
-89 if verbose or noop: 
-90 rich.print(generated_code, file=sys.stderr) 
-91 
-92 if not noop: 
-93 try: 
-94 exec(generated_code) # nosec: B102 
-95 except NameError: 
-96 # something is missing! 
-97 missing_vars = find_missing_variables(generated_code) 
-98 if not magic: 
-99 rich.print( 
-100 f"Your code is missing some variables: {missing_vars}. Add these or try --
-magic", file=sys.stderr 
-101 ) 
-102 else: 
-103 extra_code = generate_magic_code(missing_vars) 
-104 
-105 generated_code = to_execute.substitute( 
-106 { 
-107 "tables": flatten(tables or []), 
-108 "db_type": db_type or "", 
-109 "extra": extra_code, 
-110 "code": textwrap.dedent(code), 
-111 } 
-112 ) 
-113 
-114 if verbose: 
-115 print(generated_code, file=sys.stderr) 
-116 
-117 exec(generated_code) # nosec: B102 
-118 
-119 
-120def app() -> None: # pragma: no cover 
-121 """ 
-122 Entrypoint for the pydal2sql cli command. 
-123 """ 
-124 parser = PrettyParser( 
-125 prog="pydal2sql", 
-126 formatter_class=argparse.RawDescriptionHelpFormatter, 
-127 description="""[green]CLI tool to generate SQL from PyDAL code.[/green]\n 
-128 Aside from using cli arguments, you can also configure the tool in your
-code. 
-129 You can set the following variables: 
-130 
-131 db_type: str = 'sqlite' # your desired database type; 
-132 tables: list[str] = [] # your desired tables to generate SQL for;""", 
-133 epilog="Example: [i]cat models.py | pydal2sql sqlite[/i]", 
-134 ) 
-135 
-136 parser.add_argument("filename", nargs="?", help="Which file to load? Can
-also be done with stdin.") 
-137 
-138 parser.add_argument( 
-139 "db_type", nargs="?", help="Which database dialect to generate (
-[blue]postgres, sqlite, mysql[/blue])" 
-140 ) 
+75 def collect_everything(node: ast.AST) -> None: 
+76 collect_variables(node) 
+77 collect_definitions(node) 
+78 collect_imported_names(node) 
+79 collect_imports(node) 
+80 collect_loop_variables(node) 
+81 
+82 # ChatGPT produced (4.20s for 10k): 
+83 # traverse_ast(tree, collect_variables) 
+84 # traverse_ast(tree, collect_definitions) 
+85 # traverse_ast(tree, collect_imported_names) 
+86 # traverse_ast(tree, collect_imports) 
+87 # traverse_ast(tree, collect_loop_variables) 
+88 
+89 # manually rewritten (2.19s for 10k): 
+90 traverse_ast(tree, collect_everything) 
+91 return { 
+92 var 
+93 for var in used_variables 
+94 if var not in defined_variables 
+95 and var not in imported_modules 
+96 and var not in loop_variables 
+97 and var not in imported_names 
+98 and var not in BUILTINS 
+99 } 
+100 
+101 
+102# if __name__ == "__main__": 
+103# # Example usage: 
+104# code_string = """ 
+105# from math import floor 
+106# import datetime 
+107# from pydal import DAL 
+108# a = 1 
+109# b = 2 
+110# print(a, b + c) 
+111# d = e + b 
+112# xyz 
+113# floor(d) 
+114# ceil(d) 
+115# ceil(e) 
+116# 
+117# datetime.utcnow() 
+118# 
+119# db = DAL() 
+120# 
+121# db.define_table('...') 
+122# 
+123# for table in []: 
+124# print(table) 
+125# 
+126# if toble := True: 
+127# print(toble) 
+128# """ 
+129# 
+130# # import timeit 
+131# # 
+132# # print( 
+133# # timeit.timeit(lambda: find_missing_variables(code_string),
+number=10000) 
+134# # 
+135# # 
+136# # ) 
+137# 
+138# missing_variables = find_missing_variables(code_string) 
+139# assert missing_variables == {"c", "xyz", "ceil", "e"}, missing_variables 
+140 
 141 
-142 parser.add_argument("--verbose", "-v", help="Show more info",
-action=argparse.BooleanOptionalAction, default=False) 
-143 
-144 parser.add_argument( 
-145 "--noop", "-n", help="Only show code, don't run it.",
-action=argparse.BooleanOptionalAction, default=False 
-146 ) 
-147 
-148 parser.add_argument( 
-149 "--magic", "-m", help="Perform magic to fix missing vars.",
-action=argparse.BooleanOptionalAction, default=False 
-150 ) 
-151 
-152 parser.add_argument( 
-153 "-t", 
-154 "--table", 
-155 "--tables", 
-156 action="append", 
-157 nargs="+", 
-158 help="One or more tables to generate. By default, all tables in the file
-will be used.", 
-159 ) 
-160 
-161 args = parser.parse_args() 
-162 
-163 db_type = args.db_type or args.filename 
+142def generate_magic_code(missing_vars: set[str]) -> str: 
+143 """ 
+144 After finding missing vars, fill them in with an object that does nothing
+except return itself or an empty string. 
+145 
+146 This way, it's least likely to crash (when used as default or validator in
+pydal, don't use this for running code!). 
+147 """ 
+148 extra_code = """ 
+149 class Empty: 
+150 # class that does absolutely nothing 
+151 # but can be accessed like an object (obj.something.whatever) 
+152 # or a dict[with][some][keys] 
+153 def __getattribute__(self, _): 
+154 return self 
+155 
+156 def __getitem__(self, _): 
+157 return self 
+158 
+159 def __get__(self): 
+160 return self 
+161 
+162 def __call__(self, *_): 
+163 return self 
 164 
-165 load_file_mode = (filename := args.filename) and filename.endswith(".py") 
-166 
-167 if not (has_stdin_data() or load_file_mode): 
-168 if not db_type: 
-169 db_type = Prompt.ask("Which database type do you want to use?", choices=
-["sqlite", "postgres", "mysql"]) 
+165 def __str__(self): 
+166 return '' 
+167 
+168 def __repr__(self): 
+169 return '' 
 170 
-171 rich.print("Please paste your define tables code below and press ctrl-
-D when finished.", file=sys.stderr) 
-172 
-173 # else: data from stdin 
-174 # py code or cli args should define settings. 
-175 if load_file_mode: 
-176 db_type = args.db_type 
-177 text = pathlib.Path(filename).read_text() 
-178 else: 
-179 text = sys.stdin.read() 
-180 
-181 return handle_cli(text, db_type, args.table, verbose=args.verbose,
-noop=args.noop, magic=args.magic) 
+171 # todo: overload more methods 
+172 empty = Empty() 
+173 \n 
+174 """ 
+175 for variable in missing_vars: 
+176 extra_code += f"{variable} = empty; " 
+177 
+178 return textwrap.dedent(extra_code) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-20 20:24 +0200
+at 2023-07-21 11:14 +0200
```

### Comparing `pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_core_py.html` & `pydal2sql-0.4.0/htmlcov/d_8bc7b9c2c0d01e74_core_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_8bc7b9c2c0d01e74_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74_helpers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 20:23 +0200
+            created at 2023-07-21 11:14 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -175,13 +175,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_8bc7b9c2c0d01e74_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74_helpers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 20:23 +0200
+            created at 2023-07-21 11:14 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 32 statements   32 run 0 missing 2 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-20 20:23 +0200
+at 2023-07-21 11:14 +0200
 
 
 1""" 
 2Main functionality. 
 3""" 
 4 
 5import typing 
@@ -110,8 +110,8 @@
 86 define_table, 
 87 migrate=True, 
 88 fake_migrate=True, 
 89 ) 
 90 return sql 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-20 20:23 +0200
+at 2023-07-21 11:14 +0200
```

### Comparing `pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html` & `pydal2sql-0.4.0/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -58,18 +58,18 @@
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">29<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_8bc7b9c2c0d01e74_core_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74_types_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74_magic_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 16:57 +0200
+            created at 2023-07-21 11:14 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -173,16 +173,16 @@
     <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">        <span class="key">yield</span> <span class="nam">folder_path</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_8bc7b9c2c0d01e74_core_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74_types_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74_magic_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 16:57 +0200
+            created at 2023-07-21 11:14 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 29 statements   29 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-20 16:57 +0200
+at 2023-07-21 11:14 +0200
 
 
 1""" 
 2Contains helpers for core. 
 3""" 
 4 
 5import tempfile 
@@ -110,8 +110,8 @@
 87 if folder_path is None: 
 88 tmp_dir = tempfile.TemporaryDirectory() 
 89 yield tmp_dir.name 
 90 else: 
 91 yield folder_path 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-20 16:57 +0200
+at 2023-07-21 11:14 +0200
```

### Comparing `pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html` & `pydal2sql-0.4.0/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/pydal2sql/magic.py: 100%</title>
+    <title>Coverage for src/pydal2sql/cli.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/pydal2sql/magic.py</b>:
+            <span class="text">Coverage for </span><b>src/pydal2sql/cli.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">58 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">58<span class="text"> run</span></button>
+            <span class="text">48 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">48<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
-            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
+            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">45<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_8bc7b9c2c0d01e74_helpers_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_8bc7b9c2c0d01e74___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74_types_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74_core_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 20:28 +0200
+            created at 2023-07-21 11:14 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -77,180 +77,256 @@
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">This file has methods to guess which variables are unknown and to potentially (monkey-patch) fix this.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">CLI tool to generate SQL from PyDAL code.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">ast</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">builtins</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">import</span> <span class="nam">importlib</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">textwrap</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="nam">BUILTINS</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="nam">builtins</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">argparse</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">pathlib</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">import</span> <span class="nam">select</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">string</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">import</span> <span class="nam">textwrap</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">IO</span><span class="op">,</span> <span class="nam">Optional</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">def</span> <span class="nam">traverse_ast</span><span class="op">(</span><span class="nam">node</span><span class="op">:</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">AST</span><span class="op">,</span> <span class="nam">variable_collector</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Callable</span><span class="op">[</span><span class="op">[</span><span class="nam">ast</span><span class="op">.</span><span class="nam">AST</span><span class="op">]</span><span class="op">,</span> <span class="key">None</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="str">    Calls variable_collector on each node recursively.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="nam">variable_collector</span><span class="op">(</span><span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="key">for</span> <span class="nam">child</span> <span class="key">in</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">iter_child_nodes</span><span class="op">(</span><span class="nam">node</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="nam">traverse_ast</span><span class="op">(</span><span class="nam">child</span><span class="op">,</span> <span class="nam">variable_collector</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="key">def</span> <span class="nam">find_missing_variables</span><span class="op">(</span><span class="nam">code_str</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">set</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">    Look through the source code in code_str and try to detect using ast parsing which variables are undefined.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="com"># Partly made by ChatGPT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="nam">code_str</span> <span class="op">=</span> <span class="nam">textwrap</span><span class="op">.</span><span class="nam">dedent</span><span class="op">(</span><span class="nam">code_str</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">import</span> <span class="nam">configuraptor</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">import</span> <span class="nam">rich</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">from</span> <span class="nam">configuraptor</span> <span class="key">import</span> <span class="nam">TypedConfig</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">from</span> <span class="nam">rich</span><span class="op">.</span><span class="nam">prompt</span> <span class="key">import</span> <span class="nam">Prompt</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="key">from</span> <span class="nam">rich</span><span class="op">.</span><span class="nam">style</span> <span class="key">import</span> <span class="nam">Style</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">flatten</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">magic</span> <span class="key">import</span> <span class="nam">find_missing_variables</span><span class="op">,</span> <span class="nam">generate_magic_code</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">types</span> <span class="key">import</span> <span class="nam">DATABASE_ALIASES</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="key">class</span> <span class="nam">PrettyParser</span><span class="op">(</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">ArgumentParser</span><span class="op">)</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="str">    Add 'rich' to the argparse output.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="com"># could raise SyntaxError</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="nam">tree</span><span class="op">:</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Module</span> <span class="op">=</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">parse</span><span class="op">(</span><span class="nam">code_str</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="key">def</span> <span class="nam">_print_message</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">message</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">file</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">IO</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="nam">message</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">file</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="nam">used_variables</span><span class="op">:</span> <span class="nam">set</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="nam">defined_variables</span><span class="op">:</span> <span class="nam">set</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="nam">imported_modules</span><span class="op">:</span> <span class="nam">set</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="nam">imported_names</span><span class="op">:</span> <span class="nam">set</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="nam">loop_variables</span><span class="op">:</span> <span class="nam">set</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="key">def</span> <span class="nam">collect_variables</span><span class="op">(</span><span class="nam">node</span><span class="op">:</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">AST</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Name</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">            <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">ctx</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Load</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">                <span class="nam">used_variables</span><span class="op">.</span><span class="nam">add</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">            <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">ctx</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">                <span class="nam">defined_variables</span><span class="op">.</span><span class="nam">add</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">            <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">ctx</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Del</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">                <span class="nam">defined_variables</span><span class="op">.</span><span class="nam">discard</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="key">def</span> <span class="nam">collect_definitions</span><span class="op">(</span><span class="nam">node</span><span class="op">:</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">AST</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Assign</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">            <span class="nam">node_targets</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">list</span><span class="op">[</span><span class="nam">ast</span><span class="op">.</span><span class="nam">Name</span><span class="op">]</span><span class="op">,</span> <span class="nam">node</span><span class="op">.</span><span class="nam">targets</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t"><span class="key">def</span> <span class="nam">has_stdin_data</span><span class="op">(</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t"><span class="str">    Check if the program starts with cli data (pipe | or redirect >&lt;).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="str">    See Also:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="str">        https://stackoverflow.com/questions/3762881/how-do-i-check-if-stdin-has-some-data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="key">return</span> <span class="nam">any</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">        <span class="nam">select</span><span class="op">.</span><span class="nam">select</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">            <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">                <span class="nam">sys</span><span class="op">.</span><span class="nam">stdin</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">            <span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">            <span class="op">[</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">            <span class="op">[</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">            <span class="num">0.0</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="op">)</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">            <span class="nam">defined_variables</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">target</span><span class="op">.</span><span class="nam">id</span> <span class="key">for</span> <span class="nam">target</span> <span class="key">in</span> <span class="nam">node_targets</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="key">def</span> <span class="nam">collect_imports</span><span class="op">(</span><span class="nam">node</span><span class="op">:</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">AST</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Import</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">            <span class="key">for</span> <span class="nam">alias</span> <span class="key">in</span> <span class="nam">node</span><span class="op">.</span><span class="nam">names</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">                <span class="nam">imported_names</span><span class="op">.</span><span class="nam">add</span><span class="op">(</span><span class="nam">alias</span><span class="op">.</span><span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">ImportFrom</span><span class="op">)</span> <span class="key">and</span> <span class="nam">node</span><span class="op">.</span><span class="nam">module</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">            <span class="nam">module_name</span> <span class="op">=</span> <span class="nam">node</span><span class="op">.</span><span class="nam">module</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">            <span class="nam">imported_module</span> <span class="op">=</span> <span class="nam">importlib</span><span class="op">.</span><span class="nam">import_module</span><span class="op">(</span><span class="nam">module_name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">            <span class="key">if</span> <span class="nam">node</span><span class="op">.</span><span class="nam">names</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">.</span><span class="nam">name</span> <span class="op">==</span> <span class="str">"*"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">                <span class="nam">imported_names</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">name</span> <span class="key">for</span> <span class="nam">name</span> <span class="key">in</span> <span class="nam">dir</span><span class="op">(</span><span class="nam">imported_module</span><span class="op">)</span> <span class="key">if</span> <span class="key">not</span> <span class="nam">name</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">                <span class="nam">imported_names</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">alias</span><span class="op">.</span><span class="nam">asname</span> <span class="key">or</span> <span class="nam">alias</span><span class="op">.</span><span class="nam">name</span> <span class="key">for</span> <span class="nam">alias</span> <span class="key">in</span> <span class="nam">node</span><span class="op">.</span><span class="nam">names</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">    <span class="key">def</span> <span class="nam">collect_imported_names</span><span class="op">(</span><span class="nam">node</span><span class="op">:</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">AST</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">        <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">ImportFrom</span><span class="op">)</span> <span class="key">and</span> <span class="nam">node</span><span class="op">.</span><span class="nam">module</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">            <span class="key">for</span> <span class="nam">alias</span> <span class="key">in</span> <span class="nam">node</span><span class="op">.</span><span class="nam">names</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">                <span class="nam">imported_names</span><span class="op">.</span><span class="nam">add</span><span class="op">(</span><span class="nam">alias</span><span class="op">.</span><span class="nam">asname</span> <span class="key">or</span> <span class="nam">alias</span><span class="op">.</span><span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t"><span class="key">def</span> <span class="nam">handle_cli</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="nam">code</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">    <span class="nam">db_type</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="nam">tables</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">|</span> <span class="nam">list</span><span class="op">[</span><span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">    <span class="nam">verbose</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">bool</span><span class="op">]</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="nam">noop</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">bool</span><span class="op">]</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">    <span class="nam">magic</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">bool</span><span class="op">]</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t"><span class="str">    Handle user input.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="nam">to_execute</span> <span class="op">=</span> <span class="nam">string</span><span class="op">.</span><span class="nam">Template</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">        <span class="nam">textwrap</span><span class="op">.</span><span class="nam">dedent</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">            <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t"><span class="str">        from pydal import *</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t"><span class="str">        from pydal.objects import *</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t"><span class="str">        from pydal.validators import *</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">    <span class="key">def</span> <span class="nam">collect_loop_variables</span><span class="op">(</span><span class="nam">node</span><span class="op">:</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">AST</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">For</span><span class="op">)</span> <span class="key">and</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">target</span><span class="op">,</span> <span class="nam">ast</span><span class="op">.</span><span class="nam">Name</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">            <span class="nam">loop_variables</span><span class="op">.</span><span class="nam">add</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">target</span><span class="op">.</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t"><span class="str">        from pydal2sql import generate_sql</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t"><span class="str">        db = database = DAL(None, migrate=False)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">    <span class="nam">traverse_ast</span><span class="op">(</span><span class="nam">tree</span><span class="op">,</span> <span class="nam">collect_variables</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">    <span class="nam">traverse_ast</span><span class="op">(</span><span class="nam">tree</span><span class="op">,</span> <span class="nam">collect_definitions</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">    <span class="nam">traverse_ast</span><span class="op">(</span><span class="nam">tree</span><span class="op">,</span> <span class="nam">collect_imported_names</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">    <span class="nam">traverse_ast</span><span class="op">(</span><span class="nam">tree</span><span class="op">,</span> <span class="nam">collect_imports</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="nam">traverse_ast</span><span class="op">(</span><span class="nam">tree</span><span class="op">,</span> <span class="nam">collect_loop_variables</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">        <span class="nam">var</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="key">for</span> <span class="nam">var</span> <span class="key">in</span> <span class="nam">used_variables</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="key">if</span> <span class="nam">var</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">defined_variables</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">        <span class="key">and</span> <span class="nam">var</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">imported_modules</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">        <span class="key">and</span> <span class="nam">var</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">loop_variables</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">        <span class="key">and</span> <span class="nam">var</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">imported_names</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">        <span class="key">and</span> <span class="nam">var</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">BUILTINS</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t"><span class="str">        tables = $tables</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="str">        db_type = '$db_type'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t"><span class="str">        $extra</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t"><span class="str">        $code</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t"><span class="str">        if not tables:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t"><span class="str">            tables = db._tables</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t"><span class="str">        for table in tables:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t"><span class="str">            print(generate_sql(db[table], db_type))</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t"><span class="com"># if __name__ == "__main__":</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t"><span class="com">#     # Example usage:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t"><span class="com">#     code_string = """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t"><span class="com">#     from math import floor</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t"><span class="com">#     import datetime</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t"><span class="com">#     from pydal import DAL</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t"><span class="com">#     a = 1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t"><span class="com">#     b = 2</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t"><span class="com">#     print(a, b + c)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t"><span class="com">#     d = e + b</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t"><span class="com">#     xyz</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t"><span class="com">#     floor(d)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t"><span class="com">#     ceil(d)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t"><span class="com">#     ceil(e)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="com">#     datetime.utcnow()</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t"><span class="com">#     db = DAL()</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t"><span class="com">#     db.define_table('...')</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t"><span class="com">#     for table in []:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t"><span class="com">#         print(table)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t"><span class="com">#     if toble := True:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t"><span class="com">#         print(toble)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t"><span class="com">#     """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t"><span class="com">#     missing_variables = find_missing_variables(code_string)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t"><span class="com">#     assert missing_variables == {"c", "xyz", "ceil", "e"}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">    <span class="nam">generated_code</span> <span class="op">=</span> <span class="nam">to_execute</span><span class="op">.</span><span class="nam">substitute</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">        <span class="op">{</span><span class="str">"tables"</span><span class="op">:</span> <span class="nam">flatten</span><span class="op">(</span><span class="nam">tables</span> <span class="key">or</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">,</span> <span class="str">"db_type"</span><span class="op">:</span> <span class="nam">db_type</span> <span class="key">or</span> <span class="str">""</span><span class="op">,</span> <span class="str">"code"</span><span class="op">:</span> <span class="nam">textwrap</span><span class="op">.</span><span class="nam">dedent</span><span class="op">(</span><span class="nam">code</span><span class="op">)</span><span class="op">,</span> <span class="str">"extra"</span><span class="op">:</span> <span class="str">""</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">    <span class="key">if</span> <span class="nam">verbose</span> <span class="key">or</span> <span class="nam">noop</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="nam">generated_code</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">noop</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">            <span class="nam">exec</span><span class="op">(</span><span class="nam">generated_code</span><span class="op">)</span>  <span class="com"># nosec: B102</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="key">except</span> <span class="nam">NameError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">            <span class="com"># something is missing!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">            <span class="nam">missing_vars</span> <span class="op">=</span> <span class="nam">find_missing_variables</span><span class="op">(</span><span class="nam">generated_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">            <span class="key">if</span> <span class="key">not</span> <span class="nam">magic</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">                <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">                    <span class="str">f"Your code is missing some variables: {missing_vars}. Add these or try --magic"</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">                <span class="nam">extra_code</span> <span class="op">=</span> <span class="nam">generate_magic_code</span><span class="op">(</span><span class="nam">missing_vars</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">                <span class="nam">generated_code</span> <span class="op">=</span> <span class="nam">to_execute</span><span class="op">.</span><span class="nam">substitute</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">                    <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">                        <span class="str">"tables"</span><span class="op">:</span> <span class="nam">flatten</span><span class="op">(</span><span class="nam">tables</span> <span class="key">or</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">                        <span class="str">"db_type"</span><span class="op">:</span> <span class="nam">db_type</span> <span class="key">or</span> <span class="str">""</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">                        <span class="str">"extra"</span><span class="op">:</span> <span class="nam">extra_code</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">                        <span class="str">"code"</span><span class="op">:</span> <span class="nam">textwrap</span><span class="op">.</span><span class="nam">dedent</span><span class="op">(</span><span class="nam">code</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">                    <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">                <span class="key">if</span> <span class="nam">verbose</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">                    <span class="nam">print</span><span class="op">(</span><span class="nam">generated_code</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t"><span class="key">def</span> <span class="nam">generate_magic_code</span><span class="op">(</span><span class="nam">missing_vars</span><span class="op">:</span> <span class="nam">set</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t"><span class="str">    After finding missing vars, fill them in with an object that does nothing except return itself or an empty string.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t"><span class="str">    This way, it's least likely to crash (when used as default or validator in pydal, don't use this for running code!).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">    <span class="nam">extra_code</span> <span class="op">=</span> <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t"><span class="str">        class Empty:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t"><span class="str">            # class that does absolutely nothing</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t"><span class="str">            # but can be accessed like an object (obj.something.whatever)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t"><span class="str">            # or a dict[with][some][keys]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t"><span class="str">            def __getattribute__(self, _):</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t"><span class="str">                return self</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t"><span class="str">            def __getitem__(self, _):</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t"><span class="str">                return self</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t"><span class="str">            def __get__(self):</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t"><span class="str">                return self</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">                <span class="nam">exec</span><span class="op">(</span><span class="nam">generated_code</span><span class="op">)</span>  <span class="com"># nosec: B102</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t"><span class="key">class</span> <span class="nam">CliConfig</span><span class="op">(</span><span class="nam">TypedConfig</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t"><span class="str">    Configuration from pyproject.toml or cli.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">    <span class="nam">db_type</span><span class="op">:</span> <span class="nam">DATABASE_ALIASES</span> <span class="op">|</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">    <span class="nam">verbose</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">|</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">    <span class="nam">noop</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">|</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">    <span class="nam">magic</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">|</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">    <span class="nam">filename</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">    <span class="nam">tables</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">|</span> <span class="nam">list</span><span class="op">[</span><span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t"><span class="str">        Return as semi-fancy string for Debug.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">        <span class="nam">attrs</span> <span class="op">=</span> <span class="op">[</span><span class="str">f"\t{key}={value},\n"</span> <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">value</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">        <span class="nam">classname</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">__class__</span><span class="op">.</span><span class="nam">__name__</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t"><span class="str">            def __call__(self, *_):</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t"><span class="str">                return self</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t"><span class="str">            def __str__(self):</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t"><span class="str">                return ''</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t"><span class="str">            def __repr__(self):</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t"><span class="str">                return ''</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t"><span class="str">        # todo: overload more methods</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t"><span class="str">        empty = Empty()</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t"><span class="str">            \n</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">    <span class="key">for</span> <span class="nam">variable</span> <span class="key">in</span> <span class="nam">missing_vars</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">        <span class="nam">extra_code</span> <span class="op">+=</span> <span class="str">f"{variable} = empty; "</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">    <span class="key">return</span> <span class="nam">textwrap</span><span class="op">.</span><span class="nam">dedent</span><span class="op">(</span><span class="nam">extra_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">        <span class="key">return</span> <span class="str">f"{classname}(\n{''.join(attrs)})"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">    <span class="key">def</span> <span class="nam">__repr__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t"><span class="str">        Return as fancy string for Debug.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">        <span class="nam">attrs</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">        <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">value</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">            <span class="key">if</span> <span class="nam">key</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">                <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">            <span class="nam">style</span> <span class="op">=</span> <span class="nam">Style</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">            <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">                <span class="nam">style</span> <span class="op">=</span> <span class="nam">Style</span><span class="op">(</span><span class="nam">color</span><span class="op">=</span><span class="str">"green"</span><span class="op">,</span> <span class="nam">italic</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">bold</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">                <span class="nam">value</span> <span class="op">=</span> <span class="str">f"'{value}'"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">            <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">bool</span><span class="op">)</span> <span class="key">or</span> <span class="nam">value</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">                <span class="nam">style</span> <span class="op">=</span> <span class="nam">Style</span><span class="op">(</span><span class="nam">color</span><span class="op">=</span><span class="str">"orange1"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">            <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">int</span> <span class="op">|</span> <span class="nam">float</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">                <span class="nam">style</span> <span class="op">=</span> <span class="nam">Style</span><span class="op">(</span><span class="nam">color</span><span class="op">=</span><span class="str">"blue"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">            <span class="nam">attrs</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="str">f"\t{key}={style.render(value)},\n"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">        <span class="nam">classname</span> <span class="op">=</span> <span class="nam">Style</span><span class="op">(</span><span class="nam">color</span><span class="op">=</span><span class="str">"medium_purple4"</span><span class="op">)</span><span class="op">.</span><span class="nam">render</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">__class__</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">        <span class="key">return</span> <span class="str">f"{classname}(\n{''.join(attrs)})"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t"><span class="key">def</span> <span class="nam">app</span><span class="op">(</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t"><span class="str">    Entrypoint for the pydal2sql cli command.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">    <span class="nam">parser</span> <span class="op">=</span> <span class="nam">PrettyParser</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">        <span class="nam">prog</span><span class="op">=</span><span class="str">"pydal2sql"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">        <span class="nam">formatter_class</span><span class="op">=</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">RawDescriptionHelpFormatter</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">        <span class="nam">description</span><span class="op">=</span><span class="str">"""[green]CLI tool to generate SQL from PyDAL code.[/green]\n</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t"><span class="str">        Aside from using cli arguments, you can also configure the tool in your code.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t"><span class="str">        You can set the following variables:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t"><span class="str">        db_type: str = 'sqlite' # your desired database type;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t"><span class="str">        tables: list[str] = []  # your desired tables to generate SQL for;"""</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">        <span class="nam">epilog</span><span class="op">=</span><span class="str">"Example: [i]cat models.py | pydal2sql sqlite[/i]"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span><span class="str">"filename"</span><span class="op">,</span> <span class="nam">nargs</span><span class="op">=</span><span class="str">"?"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Which file to load? Can also be done with stdin."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">        <span class="str">"db_type"</span><span class="op">,</span> <span class="nam">nargs</span><span class="op">=</span><span class="str">"?"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Which database dialect to generate ([blue]postgres, sqlite, mysql[/blue])"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span><span class="str">"--verbose"</span><span class="op">,</span> <span class="str">"-v"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Show more info"</span><span class="op">,</span> <span class="nam">action</span><span class="op">=</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">BooleanOptionalAction</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">False</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">        <span class="str">"--noop"</span><span class="op">,</span> <span class="str">"-n"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Only show code, don't run it."</span><span class="op">,</span> <span class="nam">action</span><span class="op">=</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">BooleanOptionalAction</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">        <span class="str">"--magic"</span><span class="op">,</span> <span class="str">"-m"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Perform magic to fix missing vars."</span><span class="op">,</span> <span class="nam">action</span><span class="op">=</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">BooleanOptionalAction</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">        <span class="str">"-t"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">        <span class="str">"--tables"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">        <span class="str">"--table"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">        <span class="nam">action</span><span class="op">=</span><span class="str">"append"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">        <span class="nam">nargs</span><span class="op">=</span><span class="str">"+"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">        <span class="nam">help</span><span class="op">=</span><span class="str">"One or more tables to generate. By default, all tables in the file will be used."</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">    <span class="nam">args</span> <span class="op">=</span> <span class="nam">parser</span><span class="op">.</span><span class="nam">parse_args</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">CliConfig</span><span class="op">.</span><span class="nam">load</span><span class="op">(</span><span class="nam">key</span><span class="op">=</span><span class="str">"tool.pydal2sql"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">    <span class="nam">config</span><span class="op">.</span><span class="nam">fill</span><span class="op">(</span><span class="op">**</span><span class="nam">args</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">    <span class="nam">config</span><span class="op">.</span><span class="nam">tables</span> <span class="op">=</span> <span class="nam">args</span><span class="op">.</span><span class="nam">tables</span> <span class="key">or</span> <span class="nam">config</span><span class="op">.</span><span class="nam">tables</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">    <span class="nam">db_type</span> <span class="op">=</span> <span class="nam">args</span><span class="op">.</span><span class="nam">db_type</span> <span class="key">or</span> <span class="nam">args</span><span class="op">.</span><span class="nam">filename</span> <span class="key">or</span> <span class="nam">config</span><span class="op">.</span><span class="nam">db_type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">    <span class="nam">load_file_mode</span> <span class="op">=</span> <span class="op">(</span><span class="nam">filename</span> <span class="op">:=</span> <span class="op">(</span><span class="nam">args</span><span class="op">.</span><span class="nam">filename</span> <span class="key">or</span> <span class="nam">config</span><span class="op">.</span><span class="nam">filename</span><span class="op">)</span><span class="op">)</span> <span class="key">and</span> <span class="nam">filename</span><span class="op">.</span><span class="nam">endswith</span><span class="op">(</span><span class="str">".py"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="op">(</span><span class="nam">has_stdin_data</span><span class="op">(</span><span class="op">)</span> <span class="key">or</span> <span class="nam">load_file_mode</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">db_type</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">            <span class="nam">db_type</span> <span class="op">=</span> <span class="nam">Prompt</span><span class="op">.</span><span class="nam">ask</span><span class="op">(</span><span class="str">"Which database type do you want to use?"</span><span class="op">,</span> <span class="nam">choices</span><span class="op">=</span><span class="op">[</span><span class="str">"sqlite"</span><span class="op">,</span> <span class="str">"postgres"</span><span class="op">,</span> <span class="str">"mysql"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">"Please paste your define tables code below and press ctrl-D when finished."</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">    <span class="com"># else: data from stdin</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">    <span class="com"># py code or cli args should define settings.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">    <span class="key">if</span> <span class="nam">load_file_mode</span> <span class="key">and</span> <span class="nam">filename</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">        <span class="nam">db_type</span> <span class="op">=</span> <span class="nam">args</span><span class="op">.</span><span class="nam">db_type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">        <span class="nam">text</span> <span class="op">=</span> <span class="nam">pathlib</span><span class="op">.</span><span class="nam">Path</span><span class="op">(</span><span class="nam">filename</span><span class="op">)</span><span class="op">.</span><span class="nam">read_text</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">        <span class="nam">text</span> <span class="op">=</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">stdin</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">"---"</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">    <span class="key">return</span> <span class="nam">handle_cli</span><span class="op">(</span><span class="nam">text</span><span class="op">,</span> <span class="nam">db_type</span><span class="op">,</span> <span class="nam">config</span><span class="op">.</span><span class="nam">tables</span><span class="op">,</span> <span class="nam">verbose</span><span class="op">=</span><span class="nam">config</span><span class="op">.</span><span class="nam">verbose</span><span class="op">,</span> <span class="nam">noop</span><span class="op">=</span><span class="nam">config</span><span class="op">.</span><span class="nam">noop</span><span class="op">,</span> <span class="nam">magic</span><span class="op">=</span><span class="nam">config</span><span class="op">.</span><span class="nam">magic</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_8bc7b9c2c0d01e74_helpers_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_8bc7b9c2c0d01e74___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74_types_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74_core_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 20:28 +0200
+            created at 2023-07-21 11:14 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,184 +1,269 @@
 
-****** Coverage for src/pydal2sql/magic.py: 100% ******
+****** Coverage for src/pydal2sql/cli.py: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 58 statements   58 run 0 missing 0 excluded *****
+***** 48 statements   48 run 0 missing 45 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-20 20:28 +0200
+at 2023-07-21 11:14 +0200
 
 
 1""" 
-2This file has methods to guess which variables are unknown and to potentially
-(monkey-patch) fix this. 
+2CLI tool to generate SQL from PyDAL code. 
 3""" 
 4 
-5import ast 
-6import builtins 
-7import importlib 
-8import textwrap 
-9import typing 
-10 
-11BUILTINS = set(builtins.__dict__.keys()) 
-12 
+5import argparse 
+6import pathlib 
+7import select 
+8import string 
+9import sys 
+10import textwrap 
+11import typing 
+12from typing import IO, Optional 
 13 
-14def traverse_ast(node: ast.AST, variable_collector: typing.Callable[
-[ast.AST], None]) -> None: 
-15 """ 
-16 Calls variable_collector on each node recursively. 
-17 """ 
-18 variable_collector(node) 
-19 for child in ast.iter_child_nodes(node): 
-20 traverse_ast(child, variable_collector) 
-21 
-22 
-23def find_missing_variables(code_str: str) -> set[str]: 
-24 """ 
-25 Look through the source code in code_str and try to detect using ast parsing
-which variables are undefined. 
+14import configuraptor 
+15import rich 
+16from configuraptor import TypedConfig 
+17from rich.prompt import Prompt 
+18from rich.style import Style 
+19 
+20from .helpers import flatten 
+21from .magic import find_missing_variables, generate_magic_code 
+22from .types import DATABASE_ALIASES 
+23 
+24 
+25class PrettyParser(argparse.ArgumentParser): # pragma: no cover 
 26 """ 
-27 # Partly made by ChatGPT 
-28 code_str = textwrap.dedent(code_str) 
+27 Add 'rich' to the argparse output. 
+28 """ 
 29 
-30 # could raise SyntaxError 
-31 tree: ast.Module = ast.parse(code_str) 
+30 def _print_message(self, message: str, file: Optional[IO[str]] = None) -
+> None: 
+31 rich.print(message, file=file) 
 32 
-33 used_variables: set[str] = set() 
-34 defined_variables: set[str] = set() 
-35 imported_modules: set[str] = set() 
-36 imported_names: set[str] = set() 
-37 loop_variables: set[str] = set() 
-38 
-39 def collect_variables(node: ast.AST) -> None: 
-40 if isinstance(node, ast.Name): 
-41 if isinstance(node.ctx, ast.Load): 
-42 used_variables.add(node.id) 
-43 elif isinstance(node.ctx, ast.Store): 
-44 defined_variables.add(node.id) 
-45 elif isinstance(node.ctx, ast.Del): 
-46 defined_variables.discard(node.id) 
-47 
-48 def collect_definitions(node: ast.AST) -> None: 
-49 if isinstance(node, ast.Assign): 
-50 node_targets = typing.cast(list[ast.Name], node.targets) 
+33 
+34def has_stdin_data() -> bool: # pragma: no cover 
+35 """ 
+36 Check if the program starts with cli data (pipe | or redirect ><). 
+37 
+38 See Also: 
+39 https://stackoverflow.com/questions/3762881/how-do-i-check-if-stdin-has-
+some-data 
+40 """ 
+41 return any( 
+42 select.select( 
+43 [ 
+44 sys.stdin, 
+45 ], 
+46 [], 
+47 [], 
+48 0.0, 
+49 )[0] 
+50 ) 
 51 
-52 defined_variables.update(target.id for target in node_targets) 
-53 
-54 def collect_imports(node: ast.AST) -> None: 
-55 if isinstance(node, ast.Import): 
-56 for alias in node.names: 
-57 imported_names.add(alias.name) 
-58 elif isinstance(node, ast.ImportFrom) and node.module: 
-59 module_name = node.module 
-60 imported_module = importlib.import_module(module_name) 
-61 if node.names[0].name == "*": 
-62 imported_names.update(name for name in dir(imported_module) if not
-name.startswith("_")) 
-63 else: 
-64 imported_names.update(alias.asname or alias.name for alias in node.names) 
-65 
-66 def collect_imported_names(node: ast.AST) -> None: 
-67 if isinstance(node, ast.ImportFrom) and node.module: 
-68 for alias in node.names: 
-69 imported_names.add(alias.asname or alias.name) 
+52 
+53def handle_cli( 
+54 code: str, 
+55 db_type: typing.Optional[str] = None, 
+56 tables: typing.Optional[list[str] | list[list[str]]] = None, 
+57 verbose: typing.Optional[bool] = False, 
+58 noop: typing.Optional[bool] = False, 
+59 magic: typing.Optional[bool] = False, 
+60) -> None: 
+61 """ 
+62 Handle user input. 
+63 """ 
+64 to_execute = string.Template( 
+65 textwrap.dedent( 
+66 """ 
+67 from pydal import * 
+68 from pydal.objects import * 
+69 from pydal.validators import * 
 70 
-71 def collect_loop_variables(node: ast.AST) -> None: 
-72 if isinstance(node, ast.For) and isinstance(node.target, ast.Name): 
-73 loop_variables.add(node.target.id) 
+71 from pydal2sql import generate_sql 
+72 
+73 db = database = DAL(None, migrate=False) 
 74 
-75 traverse_ast(tree, collect_variables) 
-76 traverse_ast(tree, collect_definitions) 
-77 traverse_ast(tree, collect_imported_names) 
-78 traverse_ast(tree, collect_imports) 
-79 traverse_ast(tree, collect_loop_variables) 
-80 
-81 return { 
-82 var 
-83 for var in used_variables 
-84 if var not in defined_variables 
-85 and var not in imported_modules 
-86 and var not in loop_variables 
-87 and var not in imported_names 
-88 and var not in BUILTINS 
-89 } 
+75 tables = $tables 
+76 db_type = '$db_type' 
+77 
+78 $extra 
+79 
+80 $code 
+81 
+82 if not tables: 
+83 tables = db._tables 
+84 
+85 for table in tables: 
+86 print(generate_sql(db[table], db_type)) 
+87 """ 
+88 ) 
+89 ) 
 90 
-91 
-92# if __name__ == "__main__": 
-93# # Example usage: 
-94# code_string = """ 
-95# from math import floor 
-96# import datetime 
-97# from pydal import DAL 
-98# a = 1 
-99# b = 2 
-100# print(a, b + c) 
-101# d = e + b 
-102# xyz 
-103# floor(d) 
-104# ceil(d) 
-105# ceil(e) 
-106# 
-107# datetime.utcnow() 
-108# 
-109# db = DAL() 
-110# 
-111# db.define_table('...') 
-112# 
-113# for table in []: 
-114# print(table) 
-115# 
-116# if toble := True: 
-117# print(toble) 
-118# """ 
-119# missing_variables = find_missing_variables(code_string) 
-120# assert missing_variables == {"c", "xyz", "ceil", "e"} 
+91 generated_code = to_execute.substitute( 
+92 {"tables": flatten(tables or []), "db_type": db_type or "", "code":
+textwrap.dedent(code), "extra": ""} 
+93 ) 
+94 if verbose or noop: 
+95 rich.print(generated_code, file=sys.stderr) 
+96 
+97 if not noop: 
+98 try: 
+99 exec(generated_code) # nosec: B102 
+100 except NameError: 
+101 # something is missing! 
+102 missing_vars = find_missing_variables(generated_code) 
+103 if not magic: 
+104 rich.print( 
+105 f"Your code is missing some variables: {missing_vars}. Add these or try --
+magic", file=sys.stderr 
+106 ) 
+107 else: 
+108 extra_code = generate_magic_code(missing_vars) 
+109 
+110 generated_code = to_execute.substitute( 
+111 { 
+112 "tables": flatten(tables or []), 
+113 "db_type": db_type or "", 
+114 "extra": extra_code, 
+115 "code": textwrap.dedent(code), 
+116 } 
+117 ) 
+118 
+119 if verbose: 
+120 print(generated_code, file=sys.stderr) 
 121 
-122 
-123def generate_magic_code(missing_vars: set[str]) -> str: 
-124 """ 
-125 After finding missing vars, fill them in with an object that does nothing
-except return itself or an empty string. 
-126 
-127 This way, it's least likely to crash (when used as default or validator in
-pydal, don't use this for running code!). 
-128 """ 
-129 extra_code = """ 
-130 class Empty: 
-131 # class that does absolutely nothing 
-132 # but can be accessed like an object (obj.something.whatever) 
-133 # or a dict[with][some][keys] 
-134 def __getattribute__(self, _): 
-135 return self 
-136 
-137 def __getitem__(self, _): 
-138 return self 
-139 
-140 def __get__(self): 
-141 return self 
+122 exec(generated_code) # nosec: B102 
+123 
+124class CliConfig(TypedConfig): 
+125 """ 
+126 Configuration from pyproject.toml or cli. 
+127 """ 
+128 
+129 db_type: DATABASE_ALIASES | None 
+130 verbose: bool | None 
+131 noop: bool | None 
+132 magic: bool | None 
+133 filename: str | None = None 
+134 tables: typing.Optional[list[str] | list[list[str]]] = None 
+135 
+136 def __str__(self) -> str: 
+137 """ 
+138 Return as semi-fancy string for Debug. 
+139 """ 
+140 attrs = [f"\t{key}={value},\n" for key, value in self.__dict__.items()] 
+141 classname = self.__class__.__name__ 
 142 
-143 def __call__(self, *_): 
-144 return self 
-145 
-146 def __str__(self): 
-147 return '' 
-148 
-149 def __repr__(self): 
-150 return '' 
-151 
-152 # todo: overload more methods 
-153 empty = Empty() 
-154 \n 
-155 """ 
-156 for variable in missing_vars: 
-157 extra_code += f"{variable} = empty; " 
-158 
-159 return textwrap.dedent(extra_code) 
+143 return f"{classname}(\n{''.join(attrs)})" 
+144 
+145 def __repr__(self) -> str: 
+146 """ 
+147 Return as fancy string for Debug. 
+148 """ 
+149 attrs = [] 
+150 for key, value in self.__dict__.items(): # pragma: no cover 
+151 if key.startswith("_"): 
+152 continue 
+153 style = Style() 
+154 if isinstance(value, str): 
+155 style = Style(color="green", italic=True, bold=True) 
+156 value = f"'{value}'" 
+157 elif isinstance(value, bool) or value is None: 
+158 style = Style(color="orange1") 
+159 elif isinstance(value, int | float): 
+160 style = Style(color="blue") 
+161 attrs.append(f"\t{key}={style.render(value)},\n") 
+162 
+163 classname = Style(color="medium_purple4").render(self.__class__.__name__) 
+164 
+165 return f"{classname}(\n{''.join(attrs)})" 
+166 
+167 
+168def app() -> None: # pragma: no cover 
+169 """ 
+170 Entrypoint for the pydal2sql cli command. 
+171 """ 
+172 parser = PrettyParser( 
+173 prog="pydal2sql", 
+174 formatter_class=argparse.RawDescriptionHelpFormatter, 
+175 description="""[green]CLI tool to generate SQL from PyDAL code.[/green]\n 
+176 Aside from using cli arguments, you can also configure the tool in your
+code. 
+177 You can set the following variables: 
+178 
+179 db_type: str = 'sqlite' # your desired database type; 
+180 tables: list[str] = [] # your desired tables to generate SQL for;""", 
+181 epilog="Example: [i]cat models.py | pydal2sql sqlite[/i]", 
+182 ) 
+183 
+184 parser.add_argument("filename", nargs="?", help="Which file to load? Can
+also be done with stdin.") 
+185 
+186 parser.add_argument( 
+187 "db_type", nargs="?", help="Which database dialect to generate (
+[blue]postgres, sqlite, mysql[/blue])" 
+188 ) 
+189 
+190 parser.add_argument("--verbose", "-v", help="Show more info",
+action=argparse.BooleanOptionalAction, default=False) 
+191 
+192 parser.add_argument( 
+193 "--noop", "-n", help="Only show code, don't run it.",
+action=argparse.BooleanOptionalAction, default=False 
+194 ) 
+195 
+196 parser.add_argument( 
+197 "--magic", "-m", help="Perform magic to fix missing vars.",
+action=argparse.BooleanOptionalAction, default=False 
+198 ) 
+199 
+200 parser.add_argument( 
+201 "-t", 
+202 "--tables", 
+203 "--table", 
+204 action="append", 
+205 nargs="+", 
+206 help="One or more tables to generate. By default, all tables in the file
+will be used.", 
+207 ) 
+208 
+209 args = parser.parse_args() 
+210 
+211 config = CliConfig.load(key="tool.pydal2sql") 
+212 
+213 config.fill(**args.__dict__) 
+214 config.tables = args.tables or config.tables 
+215 
+216 db_type = args.db_type or args.filename or config.db_type 
+217 
+218 load_file_mode = (filename := (args.filename or config.filename)) and
+filename.endswith(".py") 
+219 
+220 if not (has_stdin_data() or load_file_mode): 
+221 if not db_type: 
+222 db_type = Prompt.ask("Which database type do you want to use?", choices=
+["sqlite", "postgres", "mysql"]) 
+223 
+224 rich.print("Please paste your define tables code below and press ctrl-
+D when finished.", file=sys.stderr) 
+225 
+226 # else: data from stdin 
+227 # py code or cli args should define settings. 
+228 if load_file_mode and filename: 
+229 db_type = args.db_type 
+230 text = pathlib.Path(filename).read_text() 
+231 else: 
+232 text = sys.stdin.read() 
+233 rich.print("---", file=sys.stderr) 
+234 
+235 return handle_cli(text, db_type, config.tables, verbose=config.verbose,
+noop=config.noop, magic=config.magic) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-20 20:28 +0200
+at 2023-07-21 11:14 +0200
```

### Comparing `pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_types_py.html` & `pydal2sql-0.4.0/htmlcov/d_8bc7b9c2c0d01e74_types_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.1/htmlcov/favicon_32.png` & `pydal2sql-0.4.0/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.1/htmlcov/index.html` & `pydal2sql-0.4.0/htmlcov/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 20:28 +0200
+            created at 2023-07-21 11:14 +0200
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -73,18 +73,18 @@
                 <td>5</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="5 5">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_8bc7b9c2c0d01e74_cli_py.html">src/pydal2sql/cli.py</a></td>
-                <td>28</td>
+                <td>48</td>
                 <td>0</td>
-                <td>29</td>
-                <td class="right" data-ratio="28 28">100%</td>
+                <td>45</td>
+                <td class="right" data-ratio="48 48">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_8bc7b9c2c0d01e74_core_py.html">src/pydal2sql/core.py</a></td>
                 <td>32</td>
                 <td>0</td>
                 <td>2</td>
                 <td class="right" data-ratio="32 32">100%</td>
@@ -94,46 +94,46 @@
                 <td>29</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="29 29">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_8bc7b9c2c0d01e74_magic_py.html">src/pydal2sql/magic.py</a></td>
-                <td>58</td>
+                <td>60</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="58 58">100%</td>
+                <td class="right" data-ratio="60 60">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_8bc7b9c2c0d01e74_types_py.html">src/pydal2sql/types.py</a></td>
                 <td>7</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="7 7">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>160</td>
+                <td>182</td>
                 <td>0</td>
-                <td>31</td>
-                <td class="right" data-ratio="160 160">100%</td>
+                <td>47</td>
+                <td class="right" data-ratio="182 182">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 20:28 +0200
+            created at 2023-07-21 11:14 +0200
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_8bc7b9c2c0d01e74_types_py.html"/>
         <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74___about___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -2,22 +2,22 @@
 ****** Coverage report: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.7, created at 2023-07-20 20:28 +0200
+coverage.py_v7.2.7, created at 2023-07-21 11:14 +0200
 
 Module                     statements missing excluded coverage
 src/pydal2sql/__about__.py 1          0       0        100%
 src/pydal2sql/__init__.py  5          0       0        100%
-src/pydal2sql/cli.py       28         0       29       100%
+src/pydal2sql/cli.py       48         0       45       100%
 src/pydal2sql/core.py      32         0       2        100%
 src/pydal2sql/helpers.py   29         0       0        100%
-src/pydal2sql/magic.py     58         0       0        100%
+src/pydal2sql/magic.py     60         0       0        100%
 src/pydal2sql/types.py     7          0       0        100%
-Total                      160        0       31       100%
+Total                      182        0       47       100%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-07-20 20:28 +0200
+coverage.py_v7.2.7, created at 2023-07-21 11:14 +0200
  ____
```

### Comparing `pydal2sql-0.3.1/htmlcov/keybd_closed.png` & `pydal2sql-0.4.0/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.1/htmlcov/keybd_open.png` & `pydal2sql-0.4.0/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.1/htmlcov/status.json` & `pydal2sql-0.4.0/htmlcov/status.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99307208994709%*

 * *Differences: {"'files'": "{'d_8bc7b9c2c0d01e74___about___py': {'hash': 'a61d65b1f3b9256131f26af32d8655cf'}, "*

 * *            "'d_8bc7b9c2c0d01e74_cli_py': {'hash': '6d22e617e6e6da0ce12fee9b24d7594f', 'index': "*

 * *            "{'nums': {insert: [(2, 48), (3, 45)], delete: [3, 2]}}}, "*

 * *            "'d_8bc7b9c2c0d01e74_magic_py': {'hash': '6897b1ab511d3353af7bbf1a21611bac', 'index': "*

 * *            "{'nums': {insert: [(2, 60)], delete: [2]}}}}"}*

```diff
@@ -1,11 +1,11 @@
 {
     "files": {
         "d_8bc7b9c2c0d01e74___about___py": {
-            "hash": "f8f1e1d653598950fd214fe7148d3ce5",
+            "hash": "a61d65b1f3b9256131f26af32d8655cf",
             "index": {
                 "html_filename": "d_8bc7b9c2c0d01e74___about___py.html",
                 "nums": [
                     0,
                     1,
                     1,
                     0,
@@ -31,22 +31,22 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/pydal2sql/__init__.py"
             }
         },
         "d_8bc7b9c2c0d01e74_cli_py": {
-            "hash": "7773c51a1e8e8c8fd3e312f193802ef2",
+            "hash": "6d22e617e6e6da0ce12fee9b24d7594f",
             "index": {
                 "html_filename": "d_8bc7b9c2c0d01e74_cli_py.html",
                 "nums": [
                     0,
                     1,
-                    28,
-                    29,
+                    48,
+                    45,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/pydal2sql/cli.py"
             }
@@ -82,21 +82,21 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/pydal2sql/helpers.py"
             }
         },
         "d_8bc7b9c2c0d01e74_magic_py": {
-            "hash": "6451df20c0fd7823828282fd793bd339",
+            "hash": "6897b1ab511d3353af7bbf1a21611bac",
             "index": {
                 "html_filename": "d_8bc7b9c2c0d01e74_magic_py.html",
                 "nums": [
                     0,
                     1,
-                    58,
+                    60,
                     0,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/pydal2sql/magic.py"
```

### Comparing `pydal2sql-0.3.1/htmlcov/style.css` & `pydal2sql-0.4.0/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.1/src/pydal2sql/cli.py` & `pydal2sql-0.4.0/src/pydal2sql/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,21 +4,25 @@
 
 import argparse
 import pathlib
 import select
 import string
 import sys
 import textwrap
+import typing
 from typing import IO, Optional
 
 import rich
+from configuraptor import TypedConfig
 from rich.prompt import Prompt
+from rich.style import Style
 
 from .helpers import flatten
 from .magic import find_missing_variables, generate_magic_code
+from .types import DATABASE_ALIASES
 
 
 class PrettyParser(argparse.ArgumentParser):  # pragma: no cover
     """
     Add 'rich' to the argparse output.
     """
 
@@ -43,19 +47,19 @@
             0.0,
         )[0]
     )
 
 
 def handle_cli(
     code: str,
-    db_type: str = None,
-    tables: list[list[str]] = None,
-    verbose: bool = False,
-    noop: bool = False,
-    magic: bool = False,
+    db_type: typing.Optional[str] = None,
+    tables: typing.Optional[list[str] | list[list[str]]] = None,
+    verbose: typing.Optional[bool] = False,
+    noop: typing.Optional[bool] = False,
+    magic: typing.Optional[bool] = False,
 ) -> None:
     """
     Handle user input.
     """
     to_execute = string.Template(
         textwrap.dedent(
             """
@@ -113,14 +117,58 @@
 
                 if verbose:
                     print(generated_code, file=sys.stderr)
 
                 exec(generated_code)  # nosec: B102
 
 
+class CliConfig(TypedConfig):
+    """
+    Configuration from pyproject.toml or cli.
+    """
+
+    db_type: DATABASE_ALIASES | None
+    verbose: bool | None
+    noop: bool | None
+    magic: bool | None
+    filename: str | None = None
+    tables: typing.Optional[list[str] | list[list[str]]] = None
+
+    def __str__(self) -> str:
+        """
+        Return as semi-fancy string for Debug.
+        """
+        attrs = [f"\t{key}={value},\n" for key, value in self.__dict__.items()]
+        classname = self.__class__.__name__
+
+        return f"{classname}(\n{''.join(attrs)})"
+
+    def __repr__(self) -> str:
+        """
+        Return as fancy string for Debug.
+        """
+        attrs = []
+        for key, value in self.__dict__.items():  # pragma: no cover
+            if key.startswith("_"):
+                continue
+            style = Style()
+            if isinstance(value, str):
+                style = Style(color="green", italic=True, bold=True)
+                value = f"'{value}'"
+            elif isinstance(value, bool) or value is None:
+                style = Style(color="orange1")
+            elif isinstance(value, int | float):
+                style = Style(color="blue")
+            attrs.append(f"\t{key}={style.render(value)},\n")
+
+        classname = Style(color="medium_purple4").render(self.__class__.__name__)
+
+        return f"{classname}(\n{''.join(attrs)})"
+
+
 def app() -> None:  # pragma: no cover
     """
     Entrypoint for the pydal2sql cli command.
     """
     parser = PrettyParser(
         prog="pydal2sql",
         formatter_class=argparse.RawDescriptionHelpFormatter,
@@ -147,35 +195,41 @@
 
     parser.add_argument(
         "--magic", "-m", help="Perform magic to fix missing vars.", action=argparse.BooleanOptionalAction, default=False
     )
 
     parser.add_argument(
         "-t",
-        "--table",
         "--tables",
+        "--table",
         action="append",
         nargs="+",
         help="One or more tables to generate. By default, all tables in the file will be used.",
     )
 
     args = parser.parse_args()
 
-    db_type = args.db_type or args.filename
+    config = CliConfig.load(key="tool.pydal2sql")
+
+    config.fill(**args.__dict__)
+    config.tables = args.tables or config.tables
+
+    db_type = args.db_type or args.filename or config.db_type
 
-    load_file_mode = (filename := args.filename) and filename.endswith(".py")
+    load_file_mode = (filename := (args.filename or config.filename)) and filename.endswith(".py")
 
     if not (has_stdin_data() or load_file_mode):
         if not db_type:
             db_type = Prompt.ask("Which database type do you want to use?", choices=["sqlite", "postgres", "mysql"])
 
         rich.print("Please paste your define tables code below and press ctrl-D when finished.", file=sys.stderr)
 
     # else: data from stdin
     # py code or cli args should define settings.
-    if load_file_mode:
+    if load_file_mode and filename:
         db_type = args.db_type
         text = pathlib.Path(filename).read_text()
     else:
         text = sys.stdin.read()
+        rich.print("---", file=sys.stderr)
 
-    return handle_cli(text, db_type, args.table, verbose=args.verbose, noop=args.noop, magic=args.magic)
+    return handle_cli(text, db_type, config.tables, verbose=config.verbose, noop=config.noop, magic=config.magic)
```

### Comparing `pydal2sql-0.3.1/src/pydal2sql/core.py` & `pydal2sql-0.4.0/src/pydal2sql/core.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.1/src/pydal2sql/helpers.py` & `pydal2sql-0.4.0/src/pydal2sql/helpers.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.1/src/pydal2sql/magic.py` & `pydal2sql-0.4.0/src/pydal2sql/magic.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,20 +68,30 @@
             for alias in node.names:
                 imported_names.add(alias.asname or alias.name)
 
     def collect_loop_variables(node: ast.AST) -> None:
         if isinstance(node, ast.For) and isinstance(node.target, ast.Name):
             loop_variables.add(node.target.id)
 
-    traverse_ast(tree, collect_variables)
-    traverse_ast(tree, collect_definitions)
-    traverse_ast(tree, collect_imported_names)
-    traverse_ast(tree, collect_imports)
-    traverse_ast(tree, collect_loop_variables)
+    def collect_everything(node: ast.AST) -> None:
+        collect_variables(node)
+        collect_definitions(node)
+        collect_imported_names(node)
+        collect_imports(node)
+        collect_loop_variables(node)
+
+    # ChatGPT produced (4.20s for 10k):
+    # traverse_ast(tree, collect_variables)
+    # traverse_ast(tree, collect_definitions)
+    # traverse_ast(tree, collect_imported_names)
+    # traverse_ast(tree, collect_imports)
+    # traverse_ast(tree, collect_loop_variables)
 
+    # manually rewritten (2.19s for 10k):
+    traverse_ast(tree, collect_everything)
     return {
         var
         for var in used_variables
         if var not in defined_variables
         and var not in imported_modules
         and var not in loop_variables
         and var not in imported_names
@@ -112,16 +122,25 @@
 #
 #     for table in []:
 #         print(table)
 #
 #     if toble := True:
 #         print(toble)
 #     """
+#
+#     # import timeit
+#     #
+#     # print(
+#     #     timeit.timeit(lambda: find_missing_variables(code_string), number=10000)
+#     #
+#     #
+#     # )
+#
 #     missing_variables = find_missing_variables(code_string)
-#     assert missing_variables == {"c", "xyz", "ceil", "e"}
+#     assert missing_variables == {"c", "xyz", "ceil", "e"}, missing_variables
 
 
 def generate_magic_code(missing_vars: set[str]) -> str:
     """
     After finding missing vars, fill them in with an object that does nothing except return itself or an empty string.
 
     This way, it's least likely to crash (when used as default or validator in pydal, don't use this for running code!).
```

### Comparing `pydal2sql-0.3.1/tests/test_cli.py` & `pydal2sql-0.4.0/tests/test_cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from src.pydal2sql.cli import handle_cli
+from src.pydal2sql.cli import handle_cli, CliConfig
 from src.pydal2sql.magic import find_missing_variables
 
 
 def test_cli(capsys):
     code = """
     db.define_table(
         "person",
@@ -145,7 +145,14 @@
     """
 
     # unfixable so magic = False here
     handle_cli(with_del, magic=False)
     captured = capsys.readouterr()
 
     assert "{'a'}" in captured.err
+
+
+def test_config():
+    config = CliConfig.load()
+
+    assert 'CliConfig' in repr(config)  # version with colors
+    assert 'CliConfig(' in str(config)  # text-only version
```

### Comparing `pydal2sql-0.3.1/tests/test_core.py` & `pydal2sql-0.4.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.1/tests/test_helpers.py` & `pydal2sql-0.4.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.1/LICENSE.txt` & `pydal2sql-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.1/README.md` & `pydal2sql-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -86,14 +86,30 @@
 cat model_fragment.py | pydal2sql # without cli args if settings are set in code, or
 cat model_fragment.py | pydal2sql postgres --table person # with args if settings are not in code
 # both output the CREATE TABLE statements to stdout.
 
 # alternatively, you can simply run `pydal2sql` and you will be prompted for the code, which you can then paste.
 ```
 
+### Config via pyproject.toml
+
+You can also configure settings via project settings instead of cli flags:
+
+```toml
+[tool.pydal2sql]
+db_type = "postgres" # postgres, mysql or sqlite
+filename = "examples/magic.py"  # path to Python file to load
+magic = true # bool
+verbose = true # bool
+noop = false # bool
+tables = ["person"] # list of tables
+```
+
+All keys are optional.
+
 ### Example with pipx
 
 [![asciicast](https://asciinema.org/a/upl4wB4QPDf9qO278ijWyPMby.svg)](https://asciinema.org/a/upl4wB4QPDf9qO278ijWyPMby)
 
 ### ⚠️ Experimental 🪄✨Magic🌟💻
 
 If you're copy-pasting some `define_table` statements which have validators or defaults that are defined elsewhere,
```

### Comparing `pydal2sql-0.3.1/pyproject.toml` & `pydal2sql-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "rich",
     "pydal",
+    "configuraptor >= 1.15",
 ]
 
 [project.optional-dependencies]
 dev = [
     "hatch",
     "su6[all]",
     "python-semantic-release < 8",
@@ -82,14 +83,19 @@
 directory = "src"
 stop-after-first-failure = true
 include = []
 exclude = []
 coverage = 100
 badge = true
 
+[tool.pydal2sql]
+db_type = "postgres"
+magic = true
+tables = ["person"]
+
 [tool.black]
 target-version = ["py310"]
 line-length = 120
 # 'extend-exclude' excludes files or directories in addition to the defaults
 extend-exclude = '''
 # A regex preceded with ^/ will apply only to files and directories
 # in the root of the project.
@@ -145,15 +151,16 @@
     # db.field == None should NOT be fixed to db.field is None
     "E711",
 ]
 
 extend-exclude = ["*.bak/", "venv*/"]
 
 ignore = [
-    "RUF013" # implicit optional
+    "RUF013", # implicit optional
+    "RUF012",  # ClassVar
 ]
 
 [tool.bandit]
 # bandit -c pyproject.toml -r .
 exclude_dirs = [".bak", "venv"]
 skips = [
     "B108"  # hard coded /tmp/... files are fine for me tbh
```

### Comparing `pydal2sql-0.3.1/PKG-INFO` & `pydal2sql-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydal2sql
-Version: 0.3.1
+Version: 0.4.0
 Summary: Convert pydal define_tables to SQL using pydal's CREATE TABLE logic
 Project-URL: Documentation, https://github.com/robinvandernoord/pydal2sql#readme
 Project-URL: Issues, https://github.com/robinvandernoord/pydal2sql/issues
 Project-URL: Source, https://github.com/robinvandernoord/pydal2sql
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
+Requires-Dist: configuraptor>=1.15
 Requires-Dist: pydal
 Requires-Dist: rich
 Provides-Extra: all
 Requires-Dist: psycopg2-binary; extra == 'all'
 Requires-Dist: pymysql; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
@@ -122,14 +123,30 @@
 cat model_fragment.py | pydal2sql # without cli args if settings are set in code, or
 cat model_fragment.py | pydal2sql postgres --table person # with args if settings are not in code
 # both output the CREATE TABLE statements to stdout.
 
 # alternatively, you can simply run `pydal2sql` and you will be prompted for the code, which you can then paste.
 ```
 
+### Config via pyproject.toml
+
+You can also configure settings via project settings instead of cli flags:
+
+```toml
+[tool.pydal2sql]
+db_type = "postgres" # postgres, mysql or sqlite
+filename = "examples/magic.py"  # path to Python file to load
+magic = true # bool
+verbose = true # bool
+noop = false # bool
+tables = ["person"] # list of tables
+```
+
+All keys are optional.
+
 ### Example with pipx
 
 [![asciicast](https://asciinema.org/a/upl4wB4QPDf9qO278ijWyPMby.svg)](https://asciinema.org/a/upl4wB4QPDf9qO278ijWyPMby)
 
 ### ⚠️ Experimental 🪄✨Magic🌟💻
 
 If you're copy-pasting some `define_table` statements which have validators or defaults that are defined elsewhere,
```

