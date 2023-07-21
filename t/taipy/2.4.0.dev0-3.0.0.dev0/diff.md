# Comparing `tmp/taipy-2.4.0.dev0.tar.gz` & `tmp/taipy-3.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-2.4.0.dev0.tar", last modified: Fri Jul 21 12:56:58 2023, max compression
+gzip compressed data, was "taipy-3.0.0.dev0.tar", last modified: Fri Jun 23 10:47:19 2023, max compression
```

## Comparing `taipy-2.4.0.dev0.tar` & `taipy-3.0.0.dev0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:56:58.622823 taipy-2.4.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-21 12:55:26.000000 taipy-2.4.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-21 12:55:26.000000 taipy-2.4.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-07-21 12:56:58.622823 taipy-2.4.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-21 12:55:26.000000 taipy-2.4.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 12:55:26.000000 taipy-2.4.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 12:56:58.622823 taipy-2.4.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-21 12:55:57.000000 taipy-2.4.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:56:58.618823 taipy-2.4.0.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:56:58.622823 taipy-2.4.0.dev0/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-21 12:55:27.000000 taipy-2.4.0.dev0/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:56:58.622823 taipy-2.4.0.dev0/src/taipy/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 12:55:27.000000 taipy-2.4.0.dev0/src/taipy/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-21 12:55:27.000000 taipy-2.4.0.dev0/src/taipy/_cli/_help_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-21 12:55:27.000000 taipy-2.4.0.dev0/src/taipy/_cli/_scaffold_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-21 12:55:27.000000 taipy-2.4.0.dev0/src/taipy/_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-21 12:55:27.000000 taipy-2.4.0.dev0/src/taipy/_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:56:58.622823 taipy-2.4.0.dev0/src/taipy/gui_core/
--rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-07-21 12:55:27.000000 taipy-2.4.0.dev0/src/taipy/gui_core/GuiCoreLib.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-21 12:55:27.000000 taipy-2.4.0.dev0/src/taipy/gui_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-21 12:55:27.000000 taipy-2.4.0.dev0/src/taipy/gui_core/_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:56:58.622823 taipy-2.4.0.dev0/src/taipy/gui_core/lib/
--rw-r--r--   0 runner    (1001) docker     (123)   657993 2023-07-21 12:56:51.000000 taipy-2.4.0.dev0/src/taipy/gui_core/lib/taipy-gui-core.js
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-21 12:55:27.000000 taipy-2.4.0.dev0/src/taipy/version.json
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-21 12:55:27.000000 taipy-2.4.0.dev0/src/taipy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:56:58.622823 taipy-2.4.0.dev0/src/taipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-07-21 12:56:58.000000 taipy-2.4.0.dev0/src/taipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-21 12:56:58.000000 taipy-2.4.0.dev0/src/taipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:56:58.000000 taipy-2.4.0.dev0/src/taipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 12:56:58.000000 taipy-2.4.0.dev0/src/taipy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:56:52.000000 taipy-2.4.0.dev0/src/taipy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-21 12:56:58.000000 taipy-2.4.0.dev0/src/taipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 12:56:58.000000 taipy-2.4.0.dev0/src/taipy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:56:58.622823 taipy-2.4.0.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-21 12:55:27.000000 taipy-2.4.0.dev0/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.938102 taipy-3.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-23 10:47:19.938102 taipy-3.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:47:19.938102 taipy-3.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-23 10:46:09.000000 taipy-3.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.926101 taipy-3.0.0.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.930101 taipy-3.0.0.dev0/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.934102 taipy-3.0.0.dev0/src/taipy/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/_cli/_help_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/_cli/_scaffold_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.938102 taipy-3.0.0.dev0/src/taipy/gui_core/
+-rw-r--r--   0 runner    (1001) docker     (123)    22398 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/gui_core/GuiCoreLib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/gui_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/gui_core/_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.938102 taipy-3.0.0.dev0/src/taipy/gui_core/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)   658126 2023-06-23 10:47:12.000000 taipy-3.0.0.dev0/src/taipy/gui_core/lib/taipy-gui-core.js
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.934102 taipy-3.0.0.dev0/src/taipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-23 10:47:19.000000 taipy-3.0.0.dev0/src/taipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-23 10:47:19.000000 taipy-3.0.0.dev0/src/taipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:47:19.000000 taipy-3.0.0.dev0/src/taipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-23 10:47:19.000000 taipy-3.0.0.dev0/src/taipy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:47:12.000000 taipy-3.0.0.dev0/src/taipy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-23 10:47:19.000000 taipy-3.0.0.dev0/src/taipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 10:47:19.000000 taipy-3.0.0.dev0/src/taipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.938102 taipy-3.0.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/tests/test_run.py
```

### Comparing `taipy-2.4.0.dev0/LICENSE` & `taipy-3.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-2.4.0.dev0/PKG-INFO` & `taipy-3.0.0.dev0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy
-Version: 2.4.0.dev0
+Version: 3.0.0.dev0
 Summary: A 360° open-source platform from Python pilots to production-ready web apps.
 Home-page: https://github.com/avaiga/taipy
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy
 Classifier: Intended Audience :: Developers
@@ -25,53 +25,55 @@
 License-File: LICENSE
 
 <br>
 <br>
 
 <img align="left" src="readme_img/readme_logo.png" alt="Taipy Logo" width="20%" ></img>
 <br>
-#  Welcome to Taipy
+#  Welcome to Taipy 
 <p align="left">
     <a href="https://pypi.python.org/pypi/taipy/" alt="Taipy version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/taipy.svg?label=pip&logo=PyPI&color=ff462b&labelColor=283282"></a>
     <a href="https://pypi.org/project/taipy" alt="Python version">
         <img alt="PyPI" src="https://img.shields.io/pypi/pyversions/taipy?color=ff462b&labelColor=283282"></a>
     <a href="https://www.youtube.com/@taipy8009" alt="YouTube">
         <img src="https://img.shields.io/badge/youtube-click_to_watch_videos-red.svg?color=ff462b&labelColor=283282&logo=youtube" /></a>
      <a href="https://twitter.com/Taipy_io" alt="Twitter">
         <img src="https://img.shields.io/badge/twitter-click_for_tweets-red.svg?color=ff462b&labelColor=283282&logo=twitter" /></a>
+    <a href="https://github.com/Avaiga/taipy/actions/workflows/tests.yml" alt="tests">
+        <img alt="PyPI" src="https://github.com/Avaiga/taipy/actions/workflows/tests.yml/badge.svg"></a>
 
 
 <br>
 
-###  <div align="left">Turns Data and AI algorithms into full web applications in no time.
-###  How? Taipy GUI with Taipy Core pops out as a 360° platform to build production-ready web applications</div>
-
+###  <div align="left">Turns Data and AI algorithms into full web applications in no time. 
+###  How? Taipy GUI with Taipy Core pops out as a 360° platform to build production-ready web applications</div>  
 
+ 
 
 <br>
 <br>
 
 ###  <div align="left">*Open Source, 100% Python*</div>
 
 
 <br>
 <br>
 <br>
 
-#  <div align="center"> 📊 We make both ends meet ⚙️ </div>
+#  <div align="center"> 📊 We make both ends meet ⚙️ </div>  
 <br>
  <div align="center">
-
+    
 | TAIPY GUI - the frond-end  | TAIPY Core - the back-end |
 | --------  | -------- |
 |<img src="readme_img/readme_gui_intro.gif" alt="Taipy GUI Animation"  width="100%"/> | <img src="readme_img/readme_core_intro.gif" alt="Taipy Core Animation"  width="100%"/>
 
-
-</div>
+    
+</div> 
 
 <br>
 <br>
 
 ## Installation
 
 Open a terminal and run:
@@ -100,66 +102,66 @@
 
 My excitement level: <|{excitement}|text|>
 """
 excitement = 100
 
 Gui(page=excitement_page).run()
 ```
-*RUN*🏃🏽‍♀️
-<div align="center">🎊 TA-DA! 🎊</div>
+*RUN*🏃🏽‍♀️  
+<div align="center">🎊 TA-DA! 🎊</div>  
 <br>
-<div align="center"><img src="readme_img/readme_gui_app.gif" width="60%" alt="GUI demo"></img></div>
+<div align="center"><img src="readme_img/readme_gui_app.gif" width="60%" alt="GUI demo"></img></div>  
 
 <br>
 <br>
 
 ### <div align="center">*Find out more*</div>
 *<div align="center">Check out our [Getting Started](https://docs.taipy.io/en/latest/getting_started/getting-started-gui/) and [Documentation](https://docs.taipy.io/en/latest/manuals/gui/)</div>*
 
 <br>
 <br>
 
 ## EN-CORE?
 
-#### <div align="center">Let's create a back-end execution, also called *scenario* using Taipy Core. Our scenario will filter movie data based on the genre you choose. This scenario will be submitted (i.e., executed) each time the genre selection changes and output the seven most popular movies of that genre. </div>
+#### <div align="center">Let's create a back-end execution, also called *scenario* using Taipy Core. Our scenario will filter movie data based on the genre you choose. This scenario will be submitted (i.e., executed) each time the genre selection changes and output the seven most popular movies of that genre. </div>  
 <br>
 
 *Here is our filter function: a standard Python function that is used by the unique task in the scenario*
 ```python
 def filter_genre(initial_dataset: pd.DataFrame, selected_genre):
     filtered_dataset = initial_dataset[initial_dataset['genres'].str.contains(selected_genre)]
     filtered_data = filtered_dataset.nlargest(7, 'Popularity %')
     return filtered_data
 ```
 
 *This is the execution graph of the scenario we are implementing*
 
-<div align="center"><img src="readme_img/readme_exec_g.png" alt="Taipy Core Graph"  width="60%"/></div>
+<div align="center"><img src="readme_img/readme_exec_g.png" alt="Taipy Core Graph"  width="60%"/></div> 
 
 
 ### Taipy Studio - The easy peasy way
-*You can use the Taipy Studio extension in VSCode to configure your pipeline with no code*
+*You can use the Taipy Studio extension in VSCode to configure your pipeline with no code* 
 
-<div align="center"><img src="readme_img/readme_studio.gif" width="80%" alt="GUI demo"></img></div>
+<div align="center"><img src="readme_img/readme_studio.gif" width="80%" alt="GUI demo"></img></div> 
 
-*Your configuration is automatically saved as a TOML file*
+*Your configuration is automatically saved as a TOML file* 
 
 <br>
 <br>
 
 ### <div align="center">*Find out more*</div>
 *<div align="center">Check out our [Getting Started](https://docs.taipy.io/en/latest/getting_started/getting-started-core/) and [Documentation](https://docs.taipy.io/en/latest/manuals/studio/) </div>*
 
 <br>
 <br>
 <br>
 <br>
 
 ### Taipy Core - a walk on the code side
-<div align="left">For more advanced use cases or if you prefer coding your configurations instead of using Taipy Studio, Taipy has your back! </div>
+<div align="left">For more advanced use cases or if you prefer coding your configurations instead of using Taipy Studio, Taipy has your back! </div>   
 
 *<div align="left">Check out the movie genre demo scenario creation with this [Demo](https://www.taipy.io/project/movie-genre-selector/) </div>*
 
 <br>
 <br>
 <br>
 
@@ -200,15 +202,15 @@
 # TAIPY GUI
 # Let's add Taipy GUI to our Taipy Core for a full application
 
 # Callback definition - submits scenario with genre selection
 def on_genre_selected(state):
     scenario.selected_genre_node.write(state.selected_genre)
     tp.submit(scenario)
-    state.df = scenario.filtered_data.read()
+    state.df = scenario.filtered_data.read()  
 
 # Get list of genres
 genres = [
     'Action', 'Adventure', 'Animation', 'Children', 'Comedy', 'Fantasy', 'IMAX'
     'Romance','Sci-FI', 'Western', 'Crime', 'Mystery', 'Drama', 'Horror', 'Thriller', 'Film-Noir','War', 'Musical', 'Documentary'
     ]
 
@@ -226,21 +228,21 @@
 ## Here are the top seven picks by popularity
 <|{df}|chart|x=Title|y=Popularity %|type=bar|title=Film Popularity|>
 """
 
 Gui(page=my_page).run()
 
 ```
-*RUN*🏃🏽‍♀️
+*RUN*🏃🏽‍♀️ 
 
 <br>
 
-<div align="center">🎊TA-DA!🎊</div>
+<div align="center">🎊TA-DA!🎊</div>  
 <br>
-<div align="center"><img src="readme_img/readme_app.gif" width="80%" alt="GUI demo"></img></div>
+<div align="center"><img src="readme_img/readme_app.gif" width="80%" alt="GUI demo"></img></div> 
 
 <br>
 
 <br>
 
 <br>
 <br>
```

### Comparing `taipy-2.4.0.dev0/README.md` & `taipy-3.0.0.dev0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 <br>
 <br>
 
 <img align="left" src="readme_img/readme_logo.png" alt="Taipy Logo" width="20%" ></img>
 <br>
-#  Welcome to Taipy
+#  Welcome to Taipy 
 <p align="left">
     <a href="https://pypi.python.org/pypi/taipy/" alt="Taipy version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/taipy.svg?label=pip&logo=PyPI&color=ff462b&labelColor=283282"></a>
     <a href="https://pypi.org/project/taipy" alt="Python version">
         <img alt="PyPI" src="https://img.shields.io/pypi/pyversions/taipy?color=ff462b&labelColor=283282"></a>
     <a href="https://www.youtube.com/@taipy8009" alt="YouTube">
         <img src="https://img.shields.io/badge/youtube-click_to_watch_videos-red.svg?color=ff462b&labelColor=283282&logo=youtube" /></a>
      <a href="https://twitter.com/Taipy_io" alt="Twitter">
         <img src="https://img.shields.io/badge/twitter-click_for_tweets-red.svg?color=ff462b&labelColor=283282&logo=twitter" /></a>
+    <a href="https://github.com/Avaiga/taipy/actions/workflows/tests.yml" alt="tests">
+        <img alt="PyPI" src="https://github.com/Avaiga/taipy/actions/workflows/tests.yml/badge.svg"></a>
 
 
 <br>
 
-###  <div align="left">Turns Data and AI algorithms into full web applications in no time.
-###  How? Taipy GUI with Taipy Core pops out as a 360° platform to build production-ready web applications</div>
-
+###  <div align="left">Turns Data and AI algorithms into full web applications in no time. 
+###  How? Taipy GUI with Taipy Core pops out as a 360° platform to build production-ready web applications</div>  
 
+ 
 
 <br>
 <br>
 
 ###  <div align="left">*Open Source, 100% Python*</div>
 
 
 <br>
 <br>
 <br>
 
-#  <div align="center"> 📊 We make both ends meet ⚙️ </div>
+#  <div align="center"> 📊 We make both ends meet ⚙️ </div>  
 <br>
  <div align="center">
-
+    
 | TAIPY GUI - the frond-end  | TAIPY Core - the back-end |
 | --------  | -------- |
 |<img src="readme_img/readme_gui_intro.gif" alt="Taipy GUI Animation"  width="100%"/> | <img src="readme_img/readme_core_intro.gif" alt="Taipy Core Animation"  width="100%"/>
 
-
-</div>
+    
+</div> 
 
 <br>
 <br>
 
 ## Installation
 
 Open a terminal and run:
@@ -74,66 +76,66 @@
 
 My excitement level: <|{excitement}|text|>
 """
 excitement = 100
 
 Gui(page=excitement_page).run()
 ```
-*RUN*🏃🏽‍♀️
-<div align="center">🎊 TA-DA! 🎊</div>
+*RUN*🏃🏽‍♀️  
+<div align="center">🎊 TA-DA! 🎊</div>  
 <br>
-<div align="center"><img src="readme_img/readme_gui_app.gif" width="60%" alt="GUI demo"></img></div>
+<div align="center"><img src="readme_img/readme_gui_app.gif" width="60%" alt="GUI demo"></img></div>  
 
 <br>
 <br>
 
 ### <div align="center">*Find out more*</div>
 *<div align="center">Check out our [Getting Started](https://docs.taipy.io/en/latest/getting_started/getting-started-gui/) and [Documentation](https://docs.taipy.io/en/latest/manuals/gui/)</div>*
 
 <br>
 <br>
 
 ## EN-CORE?
 
-#### <div align="center">Let's create a back-end execution, also called *scenario* using Taipy Core. Our scenario will filter movie data based on the genre you choose. This scenario will be submitted (i.e., executed) each time the genre selection changes and output the seven most popular movies of that genre. </div>
+#### <div align="center">Let's create a back-end execution, also called *scenario* using Taipy Core. Our scenario will filter movie data based on the genre you choose. This scenario will be submitted (i.e., executed) each time the genre selection changes and output the seven most popular movies of that genre. </div>  
 <br>
 
 *Here is our filter function: a standard Python function that is used by the unique task in the scenario*
 ```python
 def filter_genre(initial_dataset: pd.DataFrame, selected_genre):
     filtered_dataset = initial_dataset[initial_dataset['genres'].str.contains(selected_genre)]
     filtered_data = filtered_dataset.nlargest(7, 'Popularity %')
     return filtered_data
 ```
 
 *This is the execution graph of the scenario we are implementing*
 
-<div align="center"><img src="readme_img/readme_exec_g.png" alt="Taipy Core Graph"  width="60%"/></div>
+<div align="center"><img src="readme_img/readme_exec_g.png" alt="Taipy Core Graph"  width="60%"/></div> 
 
 
 ### Taipy Studio - The easy peasy way
-*You can use the Taipy Studio extension in VSCode to configure your pipeline with no code*
+*You can use the Taipy Studio extension in VSCode to configure your pipeline with no code* 
 
-<div align="center"><img src="readme_img/readme_studio.gif" width="80%" alt="GUI demo"></img></div>
+<div align="center"><img src="readme_img/readme_studio.gif" width="80%" alt="GUI demo"></img></div> 
 
-*Your configuration is automatically saved as a TOML file*
+*Your configuration is automatically saved as a TOML file* 
 
 <br>
 <br>
 
 ### <div align="center">*Find out more*</div>
 *<div align="center">Check out our [Getting Started](https://docs.taipy.io/en/latest/getting_started/getting-started-core/) and [Documentation](https://docs.taipy.io/en/latest/manuals/studio/) </div>*
 
 <br>
 <br>
 <br>
 <br>
 
 ### Taipy Core - a walk on the code side
-<div align="left">For more advanced use cases or if you prefer coding your configurations instead of using Taipy Studio, Taipy has your back! </div>
+<div align="left">For more advanced use cases or if you prefer coding your configurations instead of using Taipy Studio, Taipy has your back! </div>   
 
 *<div align="left">Check out the movie genre demo scenario creation with this [Demo](https://www.taipy.io/project/movie-genre-selector/) </div>*
 
 <br>
 <br>
 <br>
 
@@ -174,15 +176,15 @@
 # TAIPY GUI
 # Let's add Taipy GUI to our Taipy Core for a full application
 
 # Callback definition - submits scenario with genre selection
 def on_genre_selected(state):
     scenario.selected_genre_node.write(state.selected_genre)
     tp.submit(scenario)
-    state.df = scenario.filtered_data.read()
+    state.df = scenario.filtered_data.read()  
 
 # Get list of genres
 genres = [
     'Action', 'Adventure', 'Animation', 'Children', 'Comedy', 'Fantasy', 'IMAX'
     'Romance','Sci-FI', 'Western', 'Crime', 'Mystery', 'Drama', 'Horror', 'Thriller', 'Film-Noir','War', 'Musical', 'Documentary'
     ]
 
@@ -200,21 +202,21 @@
 ## Here are the top seven picks by popularity
 <|{df}|chart|x=Title|y=Popularity %|type=bar|title=Film Popularity|>
 """
 
 Gui(page=my_page).run()
 
 ```
-*RUN*🏃🏽‍♀️
+*RUN*🏃🏽‍♀️ 
 
 <br>
 
-<div align="center">🎊TA-DA!🎊</div>
+<div align="center">🎊TA-DA!🎊</div>  
 <br>
-<div align="center"><img src="readme_img/readme_app.gif" width="80%" alt="GUI demo"></img></div>
+<div align="center"><img src="readme_img/readme_app.gif" width="80%" alt="GUI demo"></img></div> 
 
 <br>
 
 <br>
 
 <br>
 <br>
```

### Comparing `taipy-2.4.0.dev0/setup.py` & `taipy-3.0.0.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
     version = json.load(version_file)
     version_string = f'{version.get("major", 0)}.{version.get("minor", 0)}.{version.get("patch", 0)}'
     if vext := version.get("ext"):
         version_string = f"{version_string}.{vext}"
 
 requirements = [
     "cookiecutter>=2.1.1,<2.2",
-    "taipy-rest==2.4.0.dev0",
-    "taipy-gui==2.4.0.dev0",
-    "taipy-templates==2.4.0.dev0",
+    "taipy-gui==3.0.0.dev0",
+    "taipy-rest==3.0.0.dev0",
+    "taipy-templates==3.0.0.dev0",
 ]
 
 test_requirements = ["pytest>=3.8"]
 
 extras_require = {
     "ngrok": ["pyngrok>=5.1,<6.0"],
     "image": [
```

### Comparing `taipy-2.4.0.dev0/src/taipy/__init__.py` & `taipy-3.0.0.dev0/src/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-2.4.0.dev0/src/taipy/_cli/__init__.py` & `taipy-3.0.0.dev0/src/taipy/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-2.4.0.dev0/src/taipy/_cli/_help_cli.py` & `taipy-3.0.0.dev0/src/taipy/_cli/_help_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-2.4.0.dev0/src/taipy/_cli/_scaffold_cli.py` & `taipy-3.0.0.dev0/src/taipy/_cli/_scaffold_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-2.4.0.dev0/src/taipy/_entrypoint.py` & `taipy-3.0.0.dev0/src/taipy/_entrypoint.py`

 * *Files identical despite different names*

### Comparing `taipy-2.4.0.dev0/src/taipy/_run.py` & `taipy-3.0.0.dev0/src/taipy/_run.py`

 * *Files identical despite different names*

### Comparing `taipy-2.4.0.dev0/src/taipy/gui_core/GuiCoreLib.py` & `taipy-3.0.0.dev0/src/taipy/gui_core/GuiCoreLib.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,20 +68,20 @@
         if isinstance(data, Scenario):
             scenario = core_get(data.id)
             if scenario:
                 return [
                     scenario.id,
                     scenario.is_primary,
                     scenario.config_id,
-                    scenario.cycle.get_simple_label() if scenario.cycle else "",
+                    scenario.creation_date,
                     scenario.get_simple_label(),
-                    list(scenario.tags) if scenario.tags else [],
-                    [(k, v) for k, v in scenario.properties.items() if k not in _GuiCoreScenarioAdapter.__INNER_PROPS] if scenario.properties else [],
-                    [(p.id, p.get_simple_label(), is_submittable(p)) for p in scenario.pipelines.values()] if scenario.pipelines else [],
-                    list(scenario.properties.get("authorized_tags", [])) if scenario.properties else [],
+                    list(scenario.tags),
+                    [(k, v) for k, v in scenario.properties.items() if k not in _GuiCoreScenarioAdapter.__INNER_PROPS],
+                    [(p.id, p.get_simple_label(), is_submittable(p)) for p in scenario.pipelines.values()],
+                    list(scenario.properties.get("authorized_tags", set())),
                     is_deletable(scenario),  # deletable
                     is_promotable(scenario),
                     is_submittable(scenario),
                 ]
         return None
 
     @staticmethod
@@ -153,16 +153,15 @@
         reg_id, reg_queue = Notifier.register()
         self.lock = Lock()
         super().__init__(reg_id, reg_queue)
         self.start()
 
     def process_event(self, event: Event):
         if event.entity_type == EventEntityType.SCENARIO:
-            with self.lock:
-                self.scenarios_base_level = None
+            self.scenarios_base_level = None
             scenario = core_get(event.entity_id) if event.operation.value != 3 else None
             self.gui.broadcast(
                 _GuiCoreContext._CORE_CHANGED_NAME,
                 {"scenario": event.entity_id if scenario else True},
             )
             self.data_nodes_base_level = None
         elif event.entity_type == EventEntityType.PIPELINE and event.entity_id:  # TODO import EventOperation
@@ -407,20 +406,20 @@
         "scenario": Element(
             "scenario",
             {
                 "id": ElementProperty(PropertyType.string),
                 "scenario": ElementProperty(_GuiCoreScenarioAdapter),
                 "active": ElementProperty(PropertyType.dynamic_boolean, True),
                 "expandable": ElementProperty(PropertyType.boolean, True),
-                "expanded": ElementProperty(PropertyType.boolean, True),
+                "expanded": ElementProperty(PropertyType.dynamic_boolean, False),
                 "show_submit": ElementProperty(PropertyType.boolean, True),
                 "show_delete": ElementProperty(PropertyType.boolean, True),
                 "show_config": ElementProperty(PropertyType.boolean, False),
                 "show_cycle": ElementProperty(PropertyType.boolean, False),
-                "show_tags": ElementProperty(PropertyType.boolean, True),
+                "show_tags": ElementProperty(PropertyType.boolean, False),
                 "show_properties": ElementProperty(PropertyType.boolean, True),
                 "show_pipelines": ElementProperty(PropertyType.boolean, True),
                 "show_submit_pipelines": ElementProperty(PropertyType.boolean, True),
                 "class_name": ElementProperty(PropertyType.dynamic_string),
             },
             inner_properties={
                 "on_edit": ElementProperty(PropertyType.function, f"{{{__CTX_VAR_NAME}.edit_entity}}"),
@@ -470,25 +469,17 @@
     def get_elements(self) -> t.Dict[str, Element]:
         return _GuiCore.__elts
 
     def get_scripts(self) -> t.List[str]:
         return ["lib/taipy-gui-core.js"]
 
     def on_init(self, gui: Gui) -> t.Optional[t.Tuple[str, t.Any]]:
-        gui._get_default_locals_bind().update(
-            {
-                _GuiCoreContext._SCENARIO_SELECTOR_ERROR_VAR: "",
-                _GuiCoreContext._SCENARIO_SELECTOR_ID_VAR: "",
-                _GuiCoreContext._SCENARIO_VIZ_ERROR_VAR: "",
-            }
-        )
-        ctx = _GuiCoreContext(gui)
-        gui._add_adapter_for_type(_GuiCore.__SCENARIO_ADAPTER, ctx.scenario_adapter)
-        gui._add_adapter_for_type(_GuiCore.__DATANODE_ADAPTER, ctx.data_node_adapter)
-        return _GuiCore.__CTX_VAR_NAME, ctx
+        gui._add_adapter_for_type(_GuiCore.__SCENARIO_ADAPTER, _GuiCoreContext.scenario_adapter)
+        gui._add_adapter_for_type(_GuiCore.__DATANODE_ADAPTER, _GuiCoreContext.data_node_adapter)
+        return _GuiCore.__CTX_VAR_NAME, _GuiCoreContext(gui)
 
     def on_user_init(self, state: State):
         for var in [
             _GuiCoreContext._SCENARIO_SELECTOR_ERROR_VAR,
             _GuiCoreContext._SCENARIO_SELECTOR_ID_VAR,
             _GuiCoreContext._SCENARIO_VIZ_ERROR_VAR,
         ]:
```

### Comparing `taipy-2.4.0.dev0/src/taipy/gui_core/__init__.py` & `taipy-3.0.0.dev0/src/taipy/gui_core/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-2.4.0.dev0/src/taipy/gui_core/_init.py` & `taipy-3.0.0.dev0/src/taipy/gui_core/_init.py`

 * *Files identical despite different names*

### Comparing `taipy-2.4.0.dev0/src/taipy/gui_core/lib/taipy-gui-core.js` & `taipy-3.0.0.dev0/src/taipy/gui_core/lib/taipy-gui-core.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -24768,15 +24768,15 @@
                         onConfirm: y
                     })]
                 })
             },
             jg = n => {
                 const {
                     id: r = "",
-                    scenarios: o,
+                    scenarios: o = [],
                     propagate: i = !0,
                     defaultValue: a = "",
                     value: s
                 } = n, [l, u] = (0, t.useState)(!1), [c, d] = (0, t.useState)(!1), [p, f] = (0, t.useState)(""), h = vg(n.libClassName, n.dynamicClassName, n.className), g = (0, Qh.useDispatch)(), v = (0, Qh.useModule)();
                 (0, Qh.useDispatchRequestUpdateOnFirstRender)(g, r, v, n.updateVars);
                 const m = (0, Qh.useDynamicProperty)(n.showAddButton, n.defaultShowAddButton, !0),
                     y = (0, Qh.useDynamicProperty)(n.displayCycles, n.defaultDisplayCycles, !0),
@@ -24822,15 +24822,15 @@
                     else if (a) try {
                         const e = JSON.parse(a);
                         Array.isArray(e) ? e.length && f(e[0]) : f(e)
                     } catch (e) {
                         f(a)
                     } else null === s && f("")
                 }), [a, s]), (0, t.useEffect)((() => {
-                    o && !o.length && E()
+                    o.length || E()
                 }), [o, E]);
                 const O = (0, t.useMemo)((() => Object.assign(Object.assign({}, hg), {
                     maxHeight: n.height || "50vh"
                 })), [n.height]);
                 return (0, e.jsxs)(e.Fragment, {
                     children: [(0, e.jsxs)(Ft, {
                         sx: fg,
@@ -28459,190 +28459,189 @@
                 })
             },
             xy = e => e.length == ug && "string" == typeof e[lg.id] ? e : 1 == e.length ? e[0] : void 0,
             wy = n => {
                 const {
                     id: r = "",
                     expandable: o = !0,
-                    expanded: i = !0,
-                    showConfig: a = !1,
-                    showCycle: s = !1,
-                    showDelete: l = !0,
-                    showProperties: u = !0,
-                    showPipelines: c = !0,
-                    showSubmit: d = !0,
-                    showSubmitPipelines: p = !0,
-                    showTags: f = !0
-                } = n, h = (0, Qh.useDispatch)(), g = (0, Qh.useModule)(), [v, m, y, b, x, w, k, S, E, C, O, _, T] = (0, t.useMemo)((() => {
+                    showConfig: i = !1,
+                    showCycle: a = !1,
+                    showDelete: s = !0,
+                    showProperties: l = !0,
+                    showPipelines: u = !0,
+                    showSubmit: c = !0,
+                    showSubmitPipelines: d = !0,
+                    showTags: p = !1
+                } = n, f = (0, Qh.useDispatch)(), h = (0, Qh.useModule)(), [g, v, m, y, b, x, w, k, S, E, C, O, _] = (0, t.useMemo)((() => {
                     let e;
                     if (Array.isArray(n.scenario)) e = xy(n.scenario);
                     else if (n.defaultScenario) try {
                         e = xy(JSON.parse(n.defaultScenario))
                     } catch (e) {}
                     return e ? [...e, !0] : ["", !1, "", "", "", [],
                         [],
                         [],
                         [], !1, !1, !1, !1
                     ]
-                }), [n.scenario, n.defaultScenario]), P = (0, Qh.useDynamicProperty)(n.active, n.defaultActive, !0), M = vg(n.libClassName, n.dynamicClassName, n.className), [j, A] = (0, t.useState)(!1), R = (0, t.useCallback)((() => A(!0)), []), I = (0, t.useCallback)((() => A(!1)), []), N = (0, t.useCallback)((() => {
-                    A(!1), T && h((0, Qh.createSendActionNameAction)(r, g, n.onDelete, !0, !0, {
-                        id: v
+                }), [n.scenario, n.defaultScenario]), T = (0, Qh.useDynamicProperty)(n.active, n.defaultActive, !0), P = (0, Qh.useDynamicProperty)(n.expanded, n.defaultExpanded, !1), M = vg(n.libClassName, n.dynamicClassName, n.className), [j, A] = (0, t.useState)(!1), R = (0, t.useCallback)((() => A(!0)), []), I = (0, t.useCallback)((() => A(!1)), []), N = (0, t.useCallback)((() => {
+                    A(!1), _ && f((0, Qh.createSendActionNameAction)(r, h, n.onDelete, !0, !0, {
+                        id: g
                     }))
-                }), [T, n.onDelete, v, r, h, g]), [L, D] = (0, t.useState)(!1), F = (0, t.useCallback)((() => D(!0)), []), $ = (0, t.useCallback)((() => D(!1)), []), z = (0, t.useCallback)((() => {
-                    D(!1), T && h((0, Qh.createSendActionNameAction)(r, g, n.onEdit, {
-                        id: v,
+                }), [_, n.onDelete, g, r, f, h]), [L, D] = (0, t.useState)(!1), F = (0, t.useCallback)((() => D(!0)), []), $ = (0, t.useCallback)((() => D(!1)), []), z = (0, t.useCallback)((() => {
+                    D(!1), _ && f((0, Qh.createSendActionNameAction)(r, h, n.onEdit, {
+                        id: g,
                         primary: !0
                     }))
-                }), [T, n.onEdit, v, r, h, g]), [W, B] = (0, t.useState)([]), [U, Y] = (0, t.useState)({
+                }), [_, n.onEdit, g, r, f, h]), [W, B] = (0, t.useState)([]), [U, Y] = (0, t.useState)({
                     id: "",
                     key: "",
                     value: ""
-                }), [H, V] = (0, t.useState)(T && i), G = (0, t.useCallback)(((e, t) => o && V(t)), [o]), q = (0, t.useCallback)((e => {
-                    h((0, Qh.createSendActionNameAction)(r, g, n.onSubmit, {
+                }), [H, V] = (0, t.useState)(!1), G = (0, t.useCallback)(((e, t) => V(t)), []), q = (0, t.useCallback)((e => {
+                    f((0, Qh.createSendActionNameAction)(r, h, n.onSubmit, {
                         id: e
                     }))
-                }), [n.onSubmit, r, h, g]), X = (0, t.useCallback)((e => {
-                    e.stopPropagation(), T && h((0, Qh.createSendActionNameAction)(r, g, n.onSubmit, {
-                        id: v
+                }), [n.onSubmit, r, f, h]), X = (0, t.useCallback)((e => {
+                    e.stopPropagation(), _ && f((0, Qh.createSendActionNameAction)(r, h, n.onSubmit, {
+                        id: g
                     }))
-                }), [T, n.onSubmit, r, v, h, g]), [K, Z] = (0, t.useState)(""), Q = (0, t.useCallback)((e => {
+                }), [_, n.onSubmit, r, g, f, h]), [K, Z] = (0, t.useState)(""), Q = (0, t.useCallback)((e => {
                     e.stopPropagation(), Z(e.currentTarget.dataset.focus || "")
                 }), []), [J, ee] = (0, t.useState)(), te = (0, t.useCallback)((e => {
-                    e.stopPropagation(), T && (h((0, Qh.createSendActionNameAction)(r, g, n.onEdit, {
-                        id: v,
+                    e.stopPropagation(), _ && (f((0, Qh.createSendActionNameAction)(r, h, n.onEdit, {
+                        id: g,
                         name: J
                     })), Z(""))
-                }), [T, n.onEdit, v, J, r, h, g]), ne = (0, t.useCallback)((e => {
-                    e.stopPropagation(), ee(x), Z("")
-                }), [x, ee, Z]), re = (0, t.useCallback)((e => ee(e.target.value)), []), [oe, ie] = (0, t.useState)([]), ae = (0, t.useCallback)((e => {
-                    e.stopPropagation(), T && (h((0, Qh.createSendActionNameAction)(r, g, n.onEdit, {
-                        id: v,
+                }), [_, n.onEdit, g, J, r, f, h]), ne = (0, t.useCallback)((e => {
+                    e.stopPropagation(), ee(b), Z("")
+                }), [b, ee, Z]), re = (0, t.useCallback)((e => ee(e.target.value)), []), [oe, ie] = (0, t.useState)([]), ae = (0, t.useCallback)((e => {
+                    e.stopPropagation(), _ && (f((0, Qh.createSendActionNameAction)(r, h, n.onEdit, {
+                        id: g,
                         tags: oe
                     })), Z(""))
-                }), [T, n.onEdit, v, oe, r, h, g]), se = (0, t.useCallback)((e => {
-                    e.stopPropagation(), ie(w), Z("")
-                }), [w]), le = (0, t.useCallback)(((e, t) => ie(t)), []), ue = (0, t.useCallback)((e => {
+                }), [_, n.onEdit, g, oe, r, f, h]), se = (0, t.useCallback)((e => {
+                    e.stopPropagation(), ie(x), Z("")
+                }), [x]), le = (0, t.useCallback)(((e, t) => ie(t)), []), ue = (0, t.useCallback)((e => {
                     var t, n;
                     const {
                         id: r = "",
                         name: o = ""
                     } = (null === (n = null === (t = e.currentTarget.parentElement) || void 0 === t ? void 0 : t.parentElement) || void 0 === n ? void 0 : n.dataset) || {};
                     o && (r ? B((t => t.map((t => r === t.id ? Object.assign(Object.assign({}, t), {
                         [o]: e.target.value
                     }) : t)))) : Y((t => Object.assign(Object.assign({}, t), {
                         [o]: e.target.value
                     }))))
                 }), []), ce = (0, t.useCallback)((e => {
-                    if (e.stopPropagation(), T) {
+                    if (e.stopPropagation(), _) {
                         const {
                             id: t = ""
                         } = e.currentTarget.dataset || {}, o = t ? W.find((e => e.id === t)) : U;
                         if (o) {
                             const e = o.id,
                                 t = {
-                                    id: v,
+                                    id: g,
                                     properties: [o]
                                 };
                             e && e != o.key && (t.deleted_properties = [{
                                 key: e
-                            }]), h((0, Qh.createSendActionNameAction)(r, g, n.onEdit, t))
+                            }]), f((0, Qh.createSendActionNameAction)(r, h, n.onEdit, t))
                         }
                         Y((e => Object.assign(Object.assign({}, e), {
                             key: "",
                             value: ""
                         }))), Z("")
                     }
-                }), [T, n.onEdit, v, W, U, r, h, g]), de = (0, t.useCallback)((e => {
-                    if (e.stopPropagation(), T) {
+                }), [_, n.onEdit, g, W, U, r, f, h]), de = (0, t.useCallback)((e => {
+                    if (e.stopPropagation(), _) {
                         const {
                             id: t = ""
-                        } = e.currentTarget.dataset || {}, n = k.find((([e]) => e === t));
+                        } = e.currentTarget.dataset || {}, n = w.find((([e]) => e === t));
                         n && B((e => e.map((e => e.id === n[0] ? Object.assign(Object.assign({}, e), {
                             key: n[0],
                             value: n[1]
                         }) : e)))), Z("")
                     }
-                }), [T, k]), pe = (0, t.useCallback)((e => {
+                }), [_, w]), pe = (0, t.useCallback)((e => {
                     e.stopPropagation();
                     const {
                         id: t = ""
                     } = e.currentTarget.dataset;
                     B((e => e.filter((e => e.id !== t))));
                     const o = W.find((e => e.id === t));
-                    o && h((0, Qh.createSendActionNameAction)(r, g, n.onEdit, {
-                        id: v,
+                    o && f((0, Qh.createSendActionNameAction)(r, h, n.onEdit, {
+                        id: g,
                         deleted_properties: [o]
                     })), Z("")
-                }), [n.onEdit, v, r, h, g, W]), fe = (0, t.useCallback)(((e, t) => {
-                    T && (h((0, Qh.createSendActionNameAction)(e, g, n.onEdit, {
+                }), [n.onEdit, g, r, f, h, W]), fe = (0, t.useCallback)(((e, t) => {
+                    _ && (f((0, Qh.createSendActionNameAction)(e, h, n.onEdit, {
                         id: e,
                         name: t
                     })), Z(""))
-                }), [T, n.onEdit, h, g]);
+                }), [_, n.onEdit, f, h]);
                 return (0, t.useEffect)((() => {
-                    f && ie(w), u && B(k.map((([e, t]) => ({
+                    p && ie(x), l && B(w.map((([e, t]) => ({
                         id: e,
                         key: e,
                         value: t
-                    })))), ee(x), V(i && T)
-                }), [w, k, x, T, f, u, i]), (0, t.useEffect)((() => {
+                    })))), ee(b), _ || V(!1)
+                }), [x, w, b, _, p, l]), (0, t.useEffect)((() => {
                     var e;
                     const t = null === (e = n.coreChanged) || void 0 === e ? void 0 : e.scenario;
-                    ("string" == typeof t ? t === v : Array.isArray(t) ? t.includes(v) : t) && n.updateVarName && h((0, Qh.createRequestUpdateAction)(r, g, [n.updateVarName], !0))
-                }), [n.coreChanged, n.updateVarName, r, g, h, v]), (0, e.jsxs)(e.Fragment, {
+                    ("string" == typeof t ? t === g : Array.isArray(t) ? t.includes(g) : t) && n.updateVarName && f((0, Qh.createRequestUpdateAction)(r, h, [n.updateVarName], !0))
+                }), [n.coreChanged, n.updateVarName, r, h, f, g]), (0, e.jsxs)(e.Fragment, {
                     children: [(0, e.jsxs)(Ft, {
                         sx: uy,
                         id: r,
                         onClick: Q,
                         className: M,
                         children: [(0, e.jsxs)(Dg, {
-                            defaultExpanded: i,
+                            defaultExpanded: o && P,
                             expanded: H,
                             onChange: G,
-                            disabled: !T,
+                            disabled: !_,
                             children: [(0, e.jsx)(qg, {
-                                expandIcon: o ? (0, e.jsx)(Rs.ArrowForwardIosSharp, {
+                                expandIcon: (0, e.jsx)(Rs.ArrowForwardIosSharp, {
                                     sx: dy
-                                }) : null,
+                                }),
                                 sx: my,
                                 children: (0, e.jsxs)(Nr, {
                                     container: !0,
                                     alignItems: "center",
                                     direction: "row",
                                     flexWrap: "nowrap",
                                     justifyContent: "space-between",
                                     spacing: 1,
                                     children: [(0, e.jsxs)(Nr, {
                                         item: !0,
-                                        children: [x, m ? (0, e.jsx)(jm, {
+                                        children: [b, v && (0, e.jsx)(jm, {
                                             color: "primary",
                                             label: (0, e.jsx)(Rs.FlagOutlined, {
                                                 sx: cg
                                             }),
                                             size: "small",
                                             sx: py
-                                        }) : null]
+                                        })]
                                     }), (0, e.jsx)(Nr, {
                                         item: !0,
-                                        children: d ? (0, e.jsx)(zr, {
+                                        children: c ? (0, e.jsx)(zr, {
                                             sx: fy,
                                             onClick: X,
-                                            disabled: !T || !P || !_,
+                                            disabled: !_ || !T || !O,
                                             children: (0, e.jsx)(Rs.Send, {
                                                 fontSize: "medium",
-                                                color: yy("info", !T || !P || !_)
+                                                color: yy("info", !_ || !T || !O)
                                             })
                                         }) : null
                                     })]
                                 })
                             }), (0, e.jsx)(Wg, {
                                 children: (0, e.jsxs)(Nr, {
                                     container: !0,
                                     rowSpacing: 2,
-                                    children: [a ? (0, e.jsxs)(Nr, {
+                                    children: [i ? (0, e.jsxs)(Nr, {
                                         item: !0,
                                         xs: 12,
                                         container: !0,
                                         justifyContent: "space-between",
                                         children: [(0, e.jsx)(Nr, {
                                             item: !0,
                                             xs: 4,
@@ -28652,18 +28651,18 @@
                                                 children: "Config ID"
                                             })
                                         }), (0, e.jsx)(Nr, {
                                             item: !0,
                                             xs: 8,
                                             children: (0, e.jsx)(Qn, {
                                                 variant: "subtitle2",
-                                                children: y
+                                                children: m
                                             })
                                         })]
-                                    }) : null, s ? (0, e.jsxs)(Nr, {
+                                    }) : null, a ? (0, e.jsxs)(Nr, {
                                         item: !0,
                                         xs: 12,
                                         container: !0,
                                         justifyContent: "space-between",
                                         children: [(0, e.jsx)(Nr, {
                                             item: !0,
                                             xs: 4,
@@ -28672,15 +28671,15 @@
                                                 children: "Cycle / Frequency"
                                             })
                                         }), (0, e.jsx)(Nr, {
                                             item: !0,
                                             xs: 8,
                                             children: (0, e.jsx)(Qn, {
                                                 variant: "subtitle2",
-                                                children: b
+                                                children: y
                                             })
                                         })]
                                     }) : null, (0, e.jsxs)(Nr, {
                                         item: !0,
                                         xs: 12,
                                         container: !0,
                                         justifyContent: "space-between",
@@ -28689,15 +28688,15 @@
                                             item: !0,
                                             xs: 12,
                                             container: !0,
                                             justifyContent: "space-between",
                                             "data-focus": "label",
                                             onClick: Q,
                                             sx: vy,
-                                            children: [P && "label" === K ? (0, e.jsx)(As, {
+                                            children: [T && "label" === K ? (0, e.jsx)(As, {
                                                 label: "Label",
                                                 variant: "outlined",
                                                 fullWidth: !0,
                                                 sx: cy,
                                                 value: J || "",
                                                 onChange: re,
                                                 InputProps: {
@@ -28714,44 +28713,44 @@
                                                             onClick: ne,
                                                             children: (0, e.jsx)(Rs.Cancel, {
                                                                 color: "inherit"
                                                             })
                                                         })]
                                                     })
                                                 },
-                                                disabled: !T
+                                                disabled: !_
                                             }) : (0, e.jsxs)(e.Fragment, {
                                                 children: [(0, e.jsx)(Nr, {
                                                     item: !0,
                                                     xs: 4,
                                                     children: (0, e.jsx)(Qn, {
                                                         variant: "subtitle2",
                                                         children: "Label"
                                                     })
                                                 }), (0, e.jsx)(Nr, {
                                                     item: !0,
                                                     xs: 8,
                                                     children: (0, e.jsx)(Qn, {
                                                         variant: "subtitle2",
-                                                        children: x
+                                                        children: b
                                                     })
                                                 })]
                                             }), " "]
-                                        }), f ? (0, e.jsx)(Nr, {
+                                        }), p ? (0, e.jsx)(Nr, {
                                             item: !0,
                                             xs: 12,
                                             container: !0,
                                             justifyContent: "space-between",
                                             "data-focus": "tags",
                                             onClick: Q,
                                             sx: vy,
-                                            children: P && "tags" === K ? (0, e.jsx)(Zm, {
+                                            children: T && "tags" === K ? (0, e.jsx)(Zm, {
                                                 multiple: !0,
-                                                options: E,
-                                                freeSolo: !E.length,
+                                                options: S,
+                                                freeSolo: !S.length,
                                                 renderTags: (t, n) => t.map(((t, r) => (0, e.jsx)(jm, Object.assign({
                                                     variant: "outlined",
                                                     label: t,
                                                     sx: fy
                                                 }, n({
                                                     index: r
                                                 }))))),
@@ -28777,15 +28776,15 @@
                                                                 children: (0, e.jsx)(Rs.Cancel, {
                                                                     color: "inherit"
                                                                 })
                                                             })]
                                                         })
                                                     })
                                                 })),
-                                                disabled: !T
+                                                disabled: !_
                                             }) : (0, e.jsxs)(e.Fragment, {
                                                 children: [(0, e.jsx)(Nr, {
                                                     item: !0,
                                                     xs: 4,
                                                     children: (0, e.jsx)(Qn, {
                                                         variant: "subtitle2",
                                                         children: "Tags"
@@ -28800,16 +28799,24 @@
                                                 })]
                                             })
                                         }) : null]
                                     }), (0, e.jsx)(Nr, {
                                         item: !0,
                                         xs: 12,
                                         children: (0, e.jsx)(ny, {})
-                                    }), u ? (0, e.jsxs)(e.Fragment, {
-                                        children: [(0, e.jsxs)(Nr, {
+                                    }), l ? (0, e.jsxs)(e.Fragment, {
+                                        children: [(0, e.jsx)(Nr, {
+                                            item: !0,
+                                            xs: 12,
+                                            container: !0,
+                                            children: (0, e.jsx)(Qn, {
+                                                variant: "h6",
+                                                children: "Custom Properties"
+                                            })
+                                        }), (0, e.jsxs)(Nr, {
                                             item: !0,
                                             xs: 12,
                                             container: !0,
                                             rowSpacing: 2,
                                             children: [W ? W.map((t => {
                                                 const n = `property-${t.id}`;
                                                 return (0, e.jsx)(Nr, {
@@ -28817,44 +28824,44 @@
                                                     xs: 12,
                                                     spacing: 1,
                                                     container: !0,
                                                     justifyContent: "space-between",
                                                     "data-focus": n,
                                                     onClick: Q,
                                                     sx: vy,
-                                                    children: P && K === n ? (0, e.jsxs)(e.Fragment, {
+                                                    children: T && K === n ? (0, e.jsxs)(e.Fragment, {
                                                         children: [(0, e.jsx)(Nr, {
                                                             item: !0,
                                                             xs: 4,
                                                             children: (0, e.jsx)(As, {
                                                                 label: "Key",
                                                                 variant: "outlined",
                                                                 value: t.key,
                                                                 sx: cy,
-                                                                disabled: !T,
+                                                                disabled: !_,
                                                                 "data-name": "key",
                                                                 "data-id": t.id,
                                                                 onChange: ue
                                                             })
                                                         }), (0, e.jsx)(Nr, {
                                                             item: !0,
-                                                            xs: 5,
+                                                            xs: 6,
                                                             children: (0, e.jsx)(As, {
                                                                 label: "Value",
                                                                 variant: "outlined",
                                                                 value: t.value,
                                                                 sx: cy,
-                                                                disabled: !T,
+                                                                disabled: !_,
                                                                 "data-name": "value",
                                                                 "data-id": t.id,
                                                                 onChange: ue
                                                             })
                                                         }), (0, e.jsxs)(Nr, {
                                                             item: !0,
-                                                            xs: 2,
+                                                            xs: 1,
                                                             container: !0,
                                                             alignContent: "center",
                                                             alignItems: "center",
                                                             justifyContent: "center",
                                                             children: [(0, e.jsx)(zr, {
                                                                 sx: fy,
                                                                 "data-id": t.id,
@@ -28877,79 +28884,79 @@
                                                             alignContent: "center",
                                                             alignItems: "center",
                                                             justifyContent: "center",
                                                             children: (0, e.jsx)(zr, {
                                                                 sx: hy,
                                                                 "data-id": t.id,
                                                                 onClick: pe,
-                                                                disabled: !T,
+                                                                disabled: !_,
                                                                 children: (0, e.jsx)(Rs.DeleteOutline, {
                                                                     fontSize: "small",
-                                                                    color: yy("primary", !T)
+                                                                    color: yy("primary", !_)
                                                                 })
                                                             })
                                                         })]
                                                     }) : (0, e.jsxs)(e.Fragment, {
                                                         children: [(0, e.jsx)(Nr, {
                                                             item: !0,
                                                             xs: 4,
                                                             children: (0, e.jsx)(Qn, {
                                                                 variant: "subtitle2",
                                                                 children: t.key
                                                             })
                                                         }), (0, e.jsx)(Nr, {
                                                             item: !0,
-                                                            xs: 5,
+                                                            xs: 6,
                                                             children: (0, e.jsx)(Qn, {
                                                                 variant: "subtitle2",
                                                                 children: t.value
                                                             })
                                                         }), " ", (0, e.jsx)(Nr, {
                                                             item: !0,
-                                                            xs: 3
+                                                            xs: 2
                                                         })]
                                                     })
                                                 }, t.id)
                                             })) : null, (0, e.jsx)(Nr, {
                                                 item: !0,
                                                 xs: 12,
                                                 spacing: 1,
                                                 container: !0,
                                                 justifyContent: "space-between",
                                                 "data-focus": "new-property",
                                                 onClick: Q,
                                                 sx: vy,
-                                                children: P && "new-property" == K ? (0, e.jsxs)(e.Fragment, {
+                                                children: T && "new-property" == K ? (0, e.jsxs)(e.Fragment, {
                                                     children: [(0, e.jsx)(Nr, {
                                                         item: !0,
                                                         xs: 4,
                                                         children: (0, e.jsx)(As, {
                                                             value: U.key,
                                                             "data-name": "key",
                                                             onChange: ue,
                                                             label: "Key",
                                                             variant: "outlined",
                                                             sx: cy,
-                                                            disabled: !T
+                                                            disabled: !_
                                                         })
                                                     }), (0, e.jsx)(Nr, {
                                                         item: !0,
-                                                        xs: 5,
+                                                        xs: 6,
                                                         children: (0, e.jsx)(As, {
                                                             value: U.value,
                                                             "data-name": "value",
                                                             onChange: ue,
                                                             label: "Value",
                                                             variant: "outlined",
                                                             sx: cy,
-                                                            disabled: !T
+                                                            disabled: !_
                                                         })
                                                     }), (0, e.jsxs)(Nr, {
                                                         item: !0,
-                                                        xs: 2,
+                                                        xs: 1,
                                                         container: !0,
                                                         alignContent: "center",
                                                         alignItems: "center",
                                                         justifyContent: "center",
                                                         children: [(0, e.jsx)(zr, {
                                                             sx: fy,
                                                             onClick: ce,
@@ -28973,50 +28980,50 @@
                                                         xs: 4,
                                                         children: (0, e.jsx)(Qn, {
                                                             variant: "subtitle2",
                                                             children: "New Property Key"
                                                         })
                                                     }), (0, e.jsx)(Nr, {
                                                         item: !0,
-                                                        xs: 5,
+                                                        xs: 6,
                                                         children: (0, e.jsx)(Qn, {
                                                             variant: "subtitle2",
                                                             children: "Value"
                                                         })
                                                     }), (0, e.jsx)(Nr, {
                                                         item: !0,
-                                                        xs: 3
+                                                        xs: 2
                                                     })]
                                                 })
                                             })]
                                         }), (0, e.jsx)(Nr, {
                                             item: !0,
                                             xs: 12,
                                             children: (0, e.jsx)(ny, {})
                                         })]
-                                    }) : null, c ? (0, e.jsxs)(e.Fragment, {
+                                    }) : null, u ? (0, e.jsxs)(e.Fragment, {
                                         children: [(0, e.jsx)(Nr, {
                                             item: !0,
                                             xs: 12,
                                             container: !0,
                                             justifyContent: "space-between",
                                             children: (0, e.jsx)(Qn, {
                                                 variant: "h6",
                                                 children: "Pipelines"
                                             })
-                                        }), S && S.map(((t, n) => {
+                                        }), k && k.map(((t, n) => {
                                             const [r, o, i] = t;
                                             return (0, e.jsx)(by, {
-                                                active: P,
+                                                active: T,
                                                 number: n,
                                                 id: r,
                                                 label: o,
                                                 submitEntity: q,
-                                                enableScenarioFields: T,
-                                                submit: p,
+                                                enableScenarioFields: _,
+                                                submit: d,
                                                 editLabel: fe,
                                                 onFocus: Q,
                                                 focusName: K,
                                                 setFocusName: Z,
                                                 submittable: i
                                             }, r)
                                         })), (0, e.jsx)(Nr, {
@@ -29025,24 +29032,24 @@
                                             children: (0, e.jsx)(ny, {})
                                         })]
                                     }) : null, (0, e.jsxs)(Nr, {
                                         item: !0,
                                         xs: 12,
                                         container: !0,
                                         justifyContent: "space-between",
-                                        children: [l ? (0, e.jsx)(Ln, {
+                                        children: [s ? (0, e.jsx)(Ln, {
                                             variant: "outlined",
                                             color: "primary",
-                                            disabled: !P || !T || !C,
+                                            disabled: !T || !_ || !E,
                                             onClick: R,
                                             children: "DELETE"
                                         }) : null, (0, e.jsx)(Ln, {
                                             variant: "outlined",
                                             color: "primary",
-                                            disabled: !P || !T || m || !O,
+                                            disabled: !T || !_ || v || !C,
                                             onClick: F,
                                             children: "PROMOTE TO PRIMARY"
                                         })]
                                     })]
                                 })
                             })]
                         }), (0, e.jsx)(Ft, {
@@ -33138,15 +33145,15 @@
                         showPrimaryFlag: t.showPrimaryFlag
                     }, n[0])))
                 })
             },
             Ew = n => {
                 const {
                     id: r = "",
-                    datanodes: o,
+                    datanodes: o = [],
                     propagate: i = !0
                 } = n, [a, s] = (0, t.useState)(""), l = vg(n.libClassName, n.dynamicClassName, n.className), u = (0, Qh.useDispatch)(), c = (0, Qh.useModule)();
                 (0, Qh.useDispatchRequestUpdateOnFirstRender)(u, r, c, n.updateVars);
                 const d = (0, Qh.useDynamicProperty)(n.displayCycles, n.defaultDisplayCycles, !0),
                     p = (0, Qh.useDynamicProperty)(n.showPrimaryFlag, n.defaultShowPrimaryFlag, !0),
                     f = (0, t.useCallback)(((e, t) => {
                         var r;
@@ -33160,15 +33167,15 @@
                             const e = (0, Qh.getUpdateVar)(n.updateVars, "datanodes");
                             u((0, Qh.createSendUpdateAction)(n.updateVarName, void 0, c, n.onChange, i, e)), s("")
                         }
                     }), [n.updateVarName, n.updateVars, n.onChange, i, u, c, a]);
                 (0, t.useEffect)((() => {
                     void 0 !== n.value ? s(n.value) : n.defaultValue && s(n.defaultValue)
                 }), [n.defaultValue, n.value]), (0, t.useEffect)((() => {
-                    o && !o.length && h()
+                    o.length || h()
                 }), [o, h]), (0, t.useEffect)((() => {
                     var e;
                     if (null === (e = n.coreChanged) || void 0 === e ? void 0 : e.scenario) {
                         const e = (0, Qh.getUpdateVar)(n.updateVars, "datanodes");
                         e && u((0, Qh.createRequestUpdateAction)(r, c, [e], !0))
                     }
                 }), [n.coreChanged, n.updateVars, c, u, r]);
@@ -33181,19 +33188,19 @@
                     className: l,
                     children: [(0, e.jsx)(cl, {
                         defaultCollapseIcon: (0, e.jsx)(Rs.ExpandMore, {}),
                         defaultExpandIcon: (0, e.jsx)(Rs.ChevronRight, {}),
                         sx: g,
                         onNodeSelect: f,
                         selected: a,
-                        children: o ? o.map((t => (0, e.jsx)(Sw, {
+                        children: o.map((t => (0, e.jsx)(Sw, {
                             item: t,
                             displayCycles: d,
                             showPrimaryFlag: p
-                        }, t[0]))) : null
+                        }, t[0])))
                     }), (0, e.jsx)(Ft, {
                         children: n.error
                     })]
                 })
             }
     })(), a
 })()));
```

### Comparing `taipy-2.4.0.dev0/src/taipy/version.py` & `taipy-3.0.0.dev0/src/taipy/version.py`

 * *Files identical despite different names*

### Comparing `taipy-2.4.0.dev0/src/taipy.egg-info/PKG-INFO` & `taipy-3.0.0.dev0/src/taipy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy
-Version: 2.4.0.dev0
+Version: 3.0.0.dev0
 Summary: A 360° open-source platform from Python pilots to production-ready web apps.
 Home-page: https://github.com/avaiga/taipy
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy
 Classifier: Intended Audience :: Developers
@@ -25,53 +25,55 @@
 License-File: LICENSE
 
 <br>
 <br>
 
 <img align="left" src="readme_img/readme_logo.png" alt="Taipy Logo" width="20%" ></img>
 <br>
-#  Welcome to Taipy
+#  Welcome to Taipy 
 <p align="left">
     <a href="https://pypi.python.org/pypi/taipy/" alt="Taipy version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/taipy.svg?label=pip&logo=PyPI&color=ff462b&labelColor=283282"></a>
     <a href="https://pypi.org/project/taipy" alt="Python version">
         <img alt="PyPI" src="https://img.shields.io/pypi/pyversions/taipy?color=ff462b&labelColor=283282"></a>
     <a href="https://www.youtube.com/@taipy8009" alt="YouTube">
         <img src="https://img.shields.io/badge/youtube-click_to_watch_videos-red.svg?color=ff462b&labelColor=283282&logo=youtube" /></a>
      <a href="https://twitter.com/Taipy_io" alt="Twitter">
         <img src="https://img.shields.io/badge/twitter-click_for_tweets-red.svg?color=ff462b&labelColor=283282&logo=twitter" /></a>
+    <a href="https://github.com/Avaiga/taipy/actions/workflows/tests.yml" alt="tests">
+        <img alt="PyPI" src="https://github.com/Avaiga/taipy/actions/workflows/tests.yml/badge.svg"></a>
 
 
 <br>
 
-###  <div align="left">Turns Data and AI algorithms into full web applications in no time.
-###  How? Taipy GUI with Taipy Core pops out as a 360° platform to build production-ready web applications</div>
-
+###  <div align="left">Turns Data and AI algorithms into full web applications in no time. 
+###  How? Taipy GUI with Taipy Core pops out as a 360° platform to build production-ready web applications</div>  
 
+ 
 
 <br>
 <br>
 
 ###  <div align="left">*Open Source, 100% Python*</div>
 
 
 <br>
 <br>
 <br>
 
-#  <div align="center"> 📊 We make both ends meet ⚙️ </div>
+#  <div align="center"> 📊 We make both ends meet ⚙️ </div>  
 <br>
  <div align="center">
-
+    
 | TAIPY GUI - the frond-end  | TAIPY Core - the back-end |
 | --------  | -------- |
 |<img src="readme_img/readme_gui_intro.gif" alt="Taipy GUI Animation"  width="100%"/> | <img src="readme_img/readme_core_intro.gif" alt="Taipy Core Animation"  width="100%"/>
 
-
-</div>
+    
+</div> 
 
 <br>
 <br>
 
 ## Installation
 
 Open a terminal and run:
@@ -100,66 +102,66 @@
 
 My excitement level: <|{excitement}|text|>
 """
 excitement = 100
 
 Gui(page=excitement_page).run()
 ```
-*RUN*🏃🏽‍♀️
-<div align="center">🎊 TA-DA! 🎊</div>
+*RUN*🏃🏽‍♀️  
+<div align="center">🎊 TA-DA! 🎊</div>  
 <br>
-<div align="center"><img src="readme_img/readme_gui_app.gif" width="60%" alt="GUI demo"></img></div>
+<div align="center"><img src="readme_img/readme_gui_app.gif" width="60%" alt="GUI demo"></img></div>  
 
 <br>
 <br>
 
 ### <div align="center">*Find out more*</div>
 *<div align="center">Check out our [Getting Started](https://docs.taipy.io/en/latest/getting_started/getting-started-gui/) and [Documentation](https://docs.taipy.io/en/latest/manuals/gui/)</div>*
 
 <br>
 <br>
 
 ## EN-CORE?
 
-#### <div align="center">Let's create a back-end execution, also called *scenario* using Taipy Core. Our scenario will filter movie data based on the genre you choose. This scenario will be submitted (i.e., executed) each time the genre selection changes and output the seven most popular movies of that genre. </div>
+#### <div align="center">Let's create a back-end execution, also called *scenario* using Taipy Core. Our scenario will filter movie data based on the genre you choose. This scenario will be submitted (i.e., executed) each time the genre selection changes and output the seven most popular movies of that genre. </div>  
 <br>
 
 *Here is our filter function: a standard Python function that is used by the unique task in the scenario*
 ```python
 def filter_genre(initial_dataset: pd.DataFrame, selected_genre):
     filtered_dataset = initial_dataset[initial_dataset['genres'].str.contains(selected_genre)]
     filtered_data = filtered_dataset.nlargest(7, 'Popularity %')
     return filtered_data
 ```
 
 *This is the execution graph of the scenario we are implementing*
 
-<div align="center"><img src="readme_img/readme_exec_g.png" alt="Taipy Core Graph"  width="60%"/></div>
+<div align="center"><img src="readme_img/readme_exec_g.png" alt="Taipy Core Graph"  width="60%"/></div> 
 
 
 ### Taipy Studio - The easy peasy way
-*You can use the Taipy Studio extension in VSCode to configure your pipeline with no code*
+*You can use the Taipy Studio extension in VSCode to configure your pipeline with no code* 
 
-<div align="center"><img src="readme_img/readme_studio.gif" width="80%" alt="GUI demo"></img></div>
+<div align="center"><img src="readme_img/readme_studio.gif" width="80%" alt="GUI demo"></img></div> 
 
-*Your configuration is automatically saved as a TOML file*
+*Your configuration is automatically saved as a TOML file* 
 
 <br>
 <br>
 
 ### <div align="center">*Find out more*</div>
 *<div align="center">Check out our [Getting Started](https://docs.taipy.io/en/latest/getting_started/getting-started-core/) and [Documentation](https://docs.taipy.io/en/latest/manuals/studio/) </div>*
 
 <br>
 <br>
 <br>
 <br>
 
 ### Taipy Core - a walk on the code side
-<div align="left">For more advanced use cases or if you prefer coding your configurations instead of using Taipy Studio, Taipy has your back! </div>
+<div align="left">For more advanced use cases or if you prefer coding your configurations instead of using Taipy Studio, Taipy has your back! </div>   
 
 *<div align="left">Check out the movie genre demo scenario creation with this [Demo](https://www.taipy.io/project/movie-genre-selector/) </div>*
 
 <br>
 <br>
 <br>
 
@@ -200,15 +202,15 @@
 # TAIPY GUI
 # Let's add Taipy GUI to our Taipy Core for a full application
 
 # Callback definition - submits scenario with genre selection
 def on_genre_selected(state):
     scenario.selected_genre_node.write(state.selected_genre)
     tp.submit(scenario)
-    state.df = scenario.filtered_data.read()
+    state.df = scenario.filtered_data.read()  
 
 # Get list of genres
 genres = [
     'Action', 'Adventure', 'Animation', 'Children', 'Comedy', 'Fantasy', 'IMAX'
     'Romance','Sci-FI', 'Western', 'Crime', 'Mystery', 'Drama', 'Horror', 'Thriller', 'Film-Noir','War', 'Musical', 'Documentary'
     ]
 
@@ -226,21 +228,21 @@
 ## Here are the top seven picks by popularity
 <|{df}|chart|x=Title|y=Popularity %|type=bar|title=Film Popularity|>
 """
 
 Gui(page=my_page).run()
 
 ```
-*RUN*🏃🏽‍♀️
+*RUN*🏃🏽‍♀️ 
 
 <br>
 
-<div align="center">🎊TA-DA!🎊</div>
+<div align="center">🎊TA-DA!🎊</div>  
 <br>
-<div align="center"><img src="readme_img/readme_app.gif" width="80%" alt="GUI demo"></img></div>
+<div align="center"><img src="readme_img/readme_app.gif" width="80%" alt="GUI demo"></img></div> 
 
 <br>
 
 <br>
 
 <br>
 <br>
```

### Comparing `taipy-2.4.0.dev0/src/taipy.egg-info/SOURCES.txt` & `taipy-3.0.0.dev0/src/taipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taipy-2.4.0.dev0/tests/test_run.py` & `taipy-3.0.0.dev0/tests/test_run.py`

 * *Files identical despite different names*

