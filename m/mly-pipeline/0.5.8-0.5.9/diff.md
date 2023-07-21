# Comparing `tmp/mly_pipeline-0.5.8.tar.gz` & `tmp/mly_pipeline-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mly_pipeline-0.5.8.tar", last modified: Tue Jul 18 15:43:00 2023, max compression
+gzip compressed data, was "mly_pipeline-0.5.9.tar", last modified: Fri Jul 21 10:16:23 2023, max compression
```

## Comparing `mly_pipeline-0.5.8.tar` & `mly_pipeline-0.5.9.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:43:00.517521 mly_pipeline-0.5.8/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      123 2023-06-27 09:51:40.000000 mly_pipeline-0.5.8/.gitignore
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1691 2023-05-16 13:29:19.000000 mly_pipeline-0.5.8/.gitlab-ci.yml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-16 13:28:31.000000 mly_pipeline-0.5.8/LICENSE
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-18 15:43:00.517521 mly_pipeline-0.5.8/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6313 2022-03-23 16:00:11.000000 mly_pipeline-0.5.8/README.md
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:43:00.353520 mly_pipeline-0.5.8/docs/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2022-09-29 13:06:48.000000 mly_pipeline-0.5.8/docs/Makefile
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:43:00.230518 mly_pipeline-0.5.8/docs/build/
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:43:00.367520 mly_pipeline-0.5.8/docs/build/doctrees/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29429 2022-09-29 13:06:48.000000 mly_pipeline-0.5.8/docs/build/doctrees/HowToUse.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10289 2022-09-29 13:06:48.000000 mly_pipeline-0.5.8/docs/build/doctrees/Installation.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  2500354 2023-07-17 10:27:02.000000 mly_pipeline-0.5.8/docs/build/doctrees/environment.pickle
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    62765 2023-02-20 18:02:10.000000 mly_pipeline-0.5.8/docs/build/doctrees/gettingstarted.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    42039 2023-02-20 18:02:10.000000 mly_pipeline-0.5.8/docs/build/doctrees/howtouse.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6427 2023-07-17 10:27:02.000000 mly_pipeline-0.5.8/docs/build/doctrees/index.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9090 2023-07-17 10:27:02.000000 mly_pipeline-0.5.8/docs/build/doctrees/installation.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9551 2023-07-17 10:27:02.000000 mly_pipeline-0.5.8/docs/build/doctrees/runningasearch.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    69042 2023-07-17 10:27:02.000000 mly_pipeline-0.5.8/docs/build/doctrees/settingupasearch.doctree
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:43:00.385520 mly_pipeline-0.5.8/docs/build/html/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9207 2023-02-20 18:02:10.000000 mly_pipeline-0.5.8/docs/build/html/Getting Started.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9206 2023-02-20 18:02:10.000000 mly_pipeline-0.5.8/docs/build/html/GettingStarted.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4601 2022-09-29 13:06:49.000000 mly_pipeline-0.5.8/docs/build/html/How to use.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17205 2023-02-20 18:02:10.000000 mly_pipeline-0.5.8/docs/build/html/HowToUse.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8839 2023-02-20 18:02:10.000000 mly_pipeline-0.5.8/docs/build/html/Installation.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:43:00.415520 mly_pipeline-0.5.8/docs/build/html/_modules/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3285 2023-04-26 10:02:39.000000 mly_pipeline-0.5.8/docs/build/html/_modules/index.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13865 2022-09-29 13:06:49.000000 mly_pipeline-0.5.8/docs/build/html/_modules/io.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:43:00.421520 mly_pipeline-0.5.8/docs/build/html/_sources/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      979 2022-09-29 13:06:49.000000 mly_pipeline-0.5.8/docs/build/html/_sources/How to use.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5555 2023-02-20 18:02:10.000000 mly_pipeline-0.5.8/docs/build/html/_sources/HowToUse.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2490 2022-09-29 13:06:49.000000 mly_pipeline-0.5.8/docs/build/html/_sources/Installation.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      924 2023-07-13 11:06:23.000000 mly_pipeline-0.5.8/docs/build/html/_sources/index.rst.txt
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:43:00.489521 mly_pipeline-0.5.8/docs/build/html/_static/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      673 2022-09-29 13:06:49.000000 mly_pipeline-0.5.8/docs/build/html/_static/ajax-loader.gif
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    11185 2022-09-29 13:06:49.000000 mly_pipeline-0.5.8/docs/build/html/_static/alabaster.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14813 2023-07-17 10:27:02.000000 mly_pipeline-0.5.8/docs/build/html/_static/basic.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9827 2023-07-17 10:27:02.000000 mly_pipeline-0.5.8/docs/build/html/_static/bizstyle.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1142 2023-07-17 10:27:02.000000 mly_pipeline-0.5.8/docs/build/html/_static/bizstyle.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14940 2022-09-29 13:06:49.000000 mly_pipeline-0.5.8/docs/build/html/_static/css3-mediaqueries.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28634 2023-02-20 18:02:10.000000 mly_pipeline-0.5.8/docs/build/html/_static/css3-mediaqueries_src.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       42 2022-09-29 13:06:49.000000 mly_pipeline-0.5.8/docs/build/html/_static/custom.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4472 2023-05-12 22:36:26.000000 mly_pipeline-0.5.8/docs/build/html/_static/doctools.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      420 2023-07-17 10:27:02.000000 mly_pipeline-0.5.8/docs/build/html/_static/documentation_options.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   268039 2022-09-29 13:06:49.000000 mly_pipeline-0.5.8/docs/build/html/_static/jquery-3.2.1.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    89501 2023-02-20 18:02:10.000000 mly_pipeline-0.5.8/docs/build/html/_static/jquery.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4758 2023-07-17 10:27:02.000000 mly_pipeline-0.5.8/docs/build/html/_static/language_data.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4846 2023-07-17 10:27:02.000000 mly_pipeline-0.5.8/docs/build/html/_static/pygments.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    18215 2023-05-12 22:36:26.000000 mly_pipeline-0.5.8/docs/build/html/_static/searchtools.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35168 2022-09-29 13:06:50.000000 mly_pipeline-0.5.8/docs/build/html/_static/underscore-1.3.1.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19530 2023-02-20 18:02:10.000000 mly_pipeline-0.5.8/docs/build/html/_static/underscore.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25355 2022-09-29 13:06:50.000000 mly_pipeline-0.5.8/docs/build/html/_static/websupport.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3014 2023-07-17 10:27:02.000000 mly_pipeline-0.5.8/docs/build/html/genindex.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22800 2023-02-20 18:02:10.000000 mly_pipeline-0.5.8/docs/build/html/gettingstarted.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17606 2023-02-20 18:02:10.000000 mly_pipeline-0.5.8/docs/build/html/howtouse.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9144 2023-07-17 10:27:02.000000 mly_pipeline-0.5.8/docs/build/html/index.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8510 2023-07-17 10:27:02.000000 mly_pipeline-0.5.8/docs/build/html/installation.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1716 2023-07-17 10:27:02.000000 mly_pipeline-0.5.8/docs/build/html/objects.inv
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3898 2022-09-29 13:06:50.000000 mly_pipeline-0.5.8/docs/build/html/py-modindex.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7979 2023-07-17 10:27:02.000000 mly_pipeline-0.5.8/docs/build/html/runningasearch.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3317 2023-07-17 10:27:02.000000 mly_pipeline-0.5.8/docs/build/html/search.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    26439 2023-07-17 10:27:02.000000 mly_pipeline-0.5.8/docs/build/html/searchindex.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27117 2023-07-17 10:27:02.000000 mly_pipeline-0.5.8/docs/build/html/settingupasearch.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:43:00.497521 mly_pipeline-0.5.8/docs/source/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5974 2023-07-17 10:26:32.000000 mly_pipeline-0.5.8/docs/source/conf.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      924 2023-07-13 11:06:23.000000 mly_pipeline-0.5.8/docs/source/index.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2134 2023-06-13 10:58:33.000000 mly_pipeline-0.5.8/docs/source/installation.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1763 2023-07-13 11:09:19.000000 mly_pipeline-0.5.8/docs/source/runningasearch.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2017 2023-07-13 10:41:45.000000 mly_pipeline-0.5.8/docs/source/runningasearchoffline.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13127 2023-07-13 10:22:53.000000 mly_pipeline-0.5.8/docs/source/runningasearchonline.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14239 2023-07-11 11:08:34.000000 mly_pipeline-0.5.8/docs/source/settingupasearch.rst
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:43:00.508521 mly_pipeline-0.5.8/mly_pipeline/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      726 2023-05-12 12:55:33.000000 mly_pipeline-0.5.8/mly_pipeline/__init__.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    27971 2023-07-11 10:01:40.000000 mly_pipeline-0.5.8/mly_pipeline/continuous_FAR.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17355 2023-06-27 11:02:28.000000 mly_pipeline-0.5.8/mly_pipeline/continuous_FAR_test.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    30927 2023-07-12 09:32:36.000000 mly_pipeline-0.5.8/mly_pipeline/initialization.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    13344 2023-05-16 13:28:31.000000 mly_pipeline-0.5.8/mly_pipeline/make_eff_estimation.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    33579 2023-07-11 13:15:40.000000 mly_pipeline-0.5.8/mly_pipeline/manager.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5596 2023-07-10 10:12:27.000000 mly_pipeline-0.5.8/mly_pipeline/mly_to_grace.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    19130 2023-07-12 09:55:13.000000 mly_pipeline-0.5.8/mly_pipeline/offline_search.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17405 2023-07-18 15:42:00.000000 mly_pipeline-0.5.8/mly_pipeline/search.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    49627 2023-07-17 13:33:09.000000 mly_pipeline-0.5.8/mly_pipeline/search_functions.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:43:00.515521 mly_pipeline-0.5.8/mly_pipeline/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-0.5.8/mly_pipeline/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-07-04 13:10:16.000000 mly_pipeline-0.5.8/mly_pipeline/tests/test_skymap_generation.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:43:00.513521 mly_pipeline-0.5.8/mly_pipeline.egg-info/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-18 15:43:00.000000 mly_pipeline-0.5.8/mly_pipeline.egg-info/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2705 2023-07-18 15:43:00.000000 mly_pipeline-0.5.8/mly_pipeline.egg-info/SOURCES.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-07-18 15:43:00.000000 mly_pipeline-0.5.8/mly_pipeline.egg-info/dependency_links.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      194 2023-07-18 15:43:00.000000 mly_pipeline-0.5.8/mly_pipeline.egg-info/entry_points.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-07-18 15:43:00.000000 mly_pipeline-0.5.8/mly_pipeline.egg-info/requires.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2023-07-18 15:43:00.000000 mly_pipeline-0.5.8/mly_pipeline.egg-info/top_level.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      762 2023-07-18 15:41:25.000000 mly_pipeline-0.5.8/pyproject.toml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2023-07-18 15:43:00.517521 mly_pipeline-0.5.8/setup.cfg
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.616546 mly_pipeline-0.5.9/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      123 2023-06-27 09:51:40.000000 mly_pipeline-0.5.9/.gitignore
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1691 2023-05-16 13:29:19.000000 mly_pipeline-0.5.9/.gitlab-ci.yml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-16 13:28:31.000000 mly_pipeline-0.5.9/LICENSE
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-21 10:16:23.615546 mly_pipeline-0.5.9/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6313 2022-03-23 16:00:11.000000 mly_pipeline-0.5.9/README.md
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.447545 mly_pipeline-0.5.9/docs/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2022-09-29 13:06:48.000000 mly_pipeline-0.5.9/docs/Makefile
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.405544 mly_pipeline-0.5.9/docs/build/
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.503545 mly_pipeline-0.5.9/docs/build/doctrees/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29429 2022-09-29 13:06:48.000000 mly_pipeline-0.5.9/docs/build/doctrees/HowToUse.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10289 2022-09-29 13:06:48.000000 mly_pipeline-0.5.9/docs/build/doctrees/Installation.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  2500354 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/doctrees/environment.pickle
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    62765 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/doctrees/gettingstarted.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    42039 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/doctrees/howtouse.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6427 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/doctrees/index.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9090 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/doctrees/installation.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9551 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/doctrees/runningasearch.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    69042 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/doctrees/settingupasearch.doctree
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.521546 mly_pipeline-0.5.9/docs/build/html/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9207 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/Getting Started.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9206 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/GettingStarted.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4601 2022-09-29 13:06:49.000000 mly_pipeline-0.5.9/docs/build/html/How to use.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17205 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/HowToUse.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8839 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/Installation.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.536546 mly_pipeline-0.5.9/docs/build/html/_modules/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3285 2023-04-26 10:02:39.000000 mly_pipeline-0.5.9/docs/build/html/_modules/index.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13865 2022-09-29 13:06:49.000000 mly_pipeline-0.5.9/docs/build/html/_modules/io.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.540546 mly_pipeline-0.5.9/docs/build/html/_sources/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      979 2022-09-29 13:06:49.000000 mly_pipeline-0.5.9/docs/build/html/_sources/How to use.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5555 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/_sources/HowToUse.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2490 2022-09-29 13:06:49.000000 mly_pipeline-0.5.9/docs/build/html/_sources/Installation.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      924 2023-07-13 11:06:23.000000 mly_pipeline-0.5.9/docs/build/html/_sources/index.rst.txt
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.590546 mly_pipeline-0.5.9/docs/build/html/_static/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      673 2022-09-29 13:06:49.000000 mly_pipeline-0.5.9/docs/build/html/_static/ajax-loader.gif
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    11185 2022-09-29 13:06:49.000000 mly_pipeline-0.5.9/docs/build/html/_static/alabaster.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14813 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/_static/basic.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9827 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/_static/bizstyle.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1142 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/_static/bizstyle.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14940 2022-09-29 13:06:49.000000 mly_pipeline-0.5.9/docs/build/html/_static/css3-mediaqueries.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28634 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/_static/css3-mediaqueries_src.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       42 2022-09-29 13:06:49.000000 mly_pipeline-0.5.9/docs/build/html/_static/custom.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4472 2023-05-12 22:36:26.000000 mly_pipeline-0.5.9/docs/build/html/_static/doctools.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      420 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/_static/documentation_options.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   268039 2022-09-29 13:06:49.000000 mly_pipeline-0.5.9/docs/build/html/_static/jquery-3.2.1.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    89501 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/_static/jquery.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4758 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/_static/language_data.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4846 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/_static/pygments.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    18215 2023-05-12 22:36:26.000000 mly_pipeline-0.5.9/docs/build/html/_static/searchtools.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35168 2022-09-29 13:06:50.000000 mly_pipeline-0.5.9/docs/build/html/_static/underscore-1.3.1.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19530 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/_static/underscore.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25355 2022-09-29 13:06:50.000000 mly_pipeline-0.5.9/docs/build/html/_static/websupport.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3014 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/genindex.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22800 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/gettingstarted.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17606 2023-02-20 18:02:10.000000 mly_pipeline-0.5.9/docs/build/html/howtouse.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9144 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/index.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8510 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/installation.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1716 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/objects.inv
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3898 2022-09-29 13:06:50.000000 mly_pipeline-0.5.9/docs/build/html/py-modindex.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7979 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/runningasearch.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3317 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/search.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    26439 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/searchindex.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27117 2023-07-17 10:27:02.000000 mly_pipeline-0.5.9/docs/build/html/settingupasearch.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.598546 mly_pipeline-0.5.9/docs/source/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5974 2023-07-17 10:26:32.000000 mly_pipeline-0.5.9/docs/source/conf.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      924 2023-07-13 11:06:23.000000 mly_pipeline-0.5.9/docs/source/index.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2134 2023-06-13 10:58:33.000000 mly_pipeline-0.5.9/docs/source/installation.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1763 2023-07-13 11:09:19.000000 mly_pipeline-0.5.9/docs/source/runningasearch.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2017 2023-07-13 10:41:45.000000 mly_pipeline-0.5.9/docs/source/runningasearchoffline.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13127 2023-07-13 10:22:53.000000 mly_pipeline-0.5.9/docs/source/runningasearchonline.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14239 2023-07-11 11:08:34.000000 mly_pipeline-0.5.9/docs/source/settingupasearch.rst
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.608546 mly_pipeline-0.5.9/mly_pipeline/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      726 2023-05-12 12:55:33.000000 mly_pipeline-0.5.9/mly_pipeline/__init__.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    27971 2023-07-11 10:01:40.000000 mly_pipeline-0.5.9/mly_pipeline/continuous_FAR.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17355 2023-06-27 11:02:28.000000 mly_pipeline-0.5.9/mly_pipeline/continuous_FAR_test.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    30927 2023-07-12 09:32:36.000000 mly_pipeline-0.5.9/mly_pipeline/initialization.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    13202 2023-07-20 15:14:03.000000 mly_pipeline-0.5.9/mly_pipeline/make_eff_estimation.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    33609 2023-07-19 15:01:03.000000 mly_pipeline-0.5.9/mly_pipeline/manager.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5596 2023-07-10 10:12:27.000000 mly_pipeline-0.5.9/mly_pipeline/mly_to_grace.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    19085 2023-07-20 13:01:50.000000 mly_pipeline-0.5.9/mly_pipeline/offline_search.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17405 2023-07-18 15:42:00.000000 mly_pipeline-0.5.9/mly_pipeline/search.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    49627 2023-07-17 13:33:09.000000 mly_pipeline-0.5.9/mly_pipeline/search_functions.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.614546 mly_pipeline-0.5.9/mly_pipeline/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-0.5.9/mly_pipeline/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-07-04 13:10:16.000000 mly_pipeline-0.5.9/mly_pipeline/tests/test_skymap_generation.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:16:23.613546 mly_pipeline-0.5.9/mly_pipeline.egg-info/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-21 10:16:23.000000 mly_pipeline-0.5.9/mly_pipeline.egg-info/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2705 2023-07-21 10:16:23.000000 mly_pipeline-0.5.9/mly_pipeline.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-07-21 10:16:23.000000 mly_pipeline-0.5.9/mly_pipeline.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      194 2023-07-21 10:16:23.000000 mly_pipeline-0.5.9/mly_pipeline.egg-info/entry_points.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-07-21 10:16:23.000000 mly_pipeline-0.5.9/mly_pipeline.egg-info/requires.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2023-07-21 10:16:23.000000 mly_pipeline-0.5.9/mly_pipeline.egg-info/top_level.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      762 2023-07-21 09:26:47.000000 mly_pipeline-0.5.9/pyproject.toml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2023-07-21 10:16:23.616546 mly_pipeline-0.5.9/setup.cfg
```

### Comparing `mly_pipeline-0.5.8/.gitlab-ci.yml` & `mly_pipeline-0.5.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/LICENSE` & `mly_pipeline-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/PKG-INFO` & `mly_pipeline-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly_pipeline
-Version: 0.5.8
+Version: 0.5.9
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-0.5.8/README.md` & `mly_pipeline-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/Makefile` & `mly_pipeline-0.5.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/doctrees/HowToUse.doctree` & `mly_pipeline-0.5.9/docs/build/doctrees/HowToUse.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/doctrees/Installation.doctree` & `mly_pipeline-0.5.9/docs/build/doctrees/Installation.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/doctrees/environment.pickle` & `mly_pipeline-0.5.9/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/doctrees/gettingstarted.doctree` & `mly_pipeline-0.5.9/docs/build/doctrees/gettingstarted.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/doctrees/howtouse.doctree` & `mly_pipeline-0.5.9/docs/build/doctrees/howtouse.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/doctrees/index.doctree` & `mly_pipeline-0.5.9/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/doctrees/installation.doctree` & `mly_pipeline-0.5.9/docs/build/doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/doctrees/runningasearch.doctree` & `mly_pipeline-0.5.9/docs/build/doctrees/runningasearch.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/doctrees/settingupasearch.doctree` & `mly_pipeline-0.5.9/docs/build/doctrees/settingupasearch.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/Getting Started.html` & `mly_pipeline-0.5.9/docs/build/html/Getting Started.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/GettingStarted.html` & `mly_pipeline-0.5.9/docs/build/html/GettingStarted.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/How to use.html` & `mly_pipeline-0.5.9/docs/build/html/How to use.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/HowToUse.html` & `mly_pipeline-0.5.9/docs/build/html/HowToUse.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/Installation.html` & `mly_pipeline-0.5.9/docs/build/html/Installation.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_modules/index.html` & `mly_pipeline-0.5.9/docs/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_modules/io.html` & `mly_pipeline-0.5.9/docs/build/html/_modules/io.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_sources/How to use.rst.txt` & `mly_pipeline-0.5.9/docs/build/html/_sources/How to use.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_sources/HowToUse.rst.txt` & `mly_pipeline-0.5.9/docs/build/html/_sources/HowToUse.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_sources/Installation.rst.txt` & `mly_pipeline-0.5.9/docs/build/html/_sources/Installation.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_sources/index.rst.txt` & `mly_pipeline-0.5.9/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_static/ajax-loader.gif` & `mly_pipeline-0.5.9/docs/build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_static/alabaster.css` & `mly_pipeline-0.5.9/docs/build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_static/basic.css` & `mly_pipeline-0.5.9/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_static/bizstyle.css` & `mly_pipeline-0.5.9/docs/build/html/_static/bizstyle.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_static/bizstyle.js` & `mly_pipeline-0.5.9/docs/build/html/_static/bizstyle.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_static/css3-mediaqueries.js` & `mly_pipeline-0.5.9/docs/build/html/_static/css3-mediaqueries.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_static/css3-mediaqueries_src.js` & `mly_pipeline-0.5.9/docs/build/html/_static/css3-mediaqueries_src.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_static/doctools.js` & `mly_pipeline-0.5.9/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_static/jquery-3.2.1.js` & `mly_pipeline-0.5.9/docs/build/html/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_static/jquery.js` & `mly_pipeline-0.5.9/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_static/language_data.js` & `mly_pipeline-0.5.9/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_static/pygments.css` & `mly_pipeline-0.5.9/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_static/searchtools.js` & `mly_pipeline-0.5.9/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_static/underscore-1.3.1.js` & `mly_pipeline-0.5.9/docs/build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_static/underscore.js` & `mly_pipeline-0.5.9/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/_static/websupport.js` & `mly_pipeline-0.5.9/docs/build/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/genindex.html` & `mly_pipeline-0.5.9/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/gettingstarted.html` & `mly_pipeline-0.5.9/docs/build/html/gettingstarted.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/howtouse.html` & `mly_pipeline-0.5.9/docs/build/html/howtouse.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/index.html` & `mly_pipeline-0.5.9/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/installation.html` & `mly_pipeline-0.5.9/docs/build/html/installation.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/objects.inv` & `mly_pipeline-0.5.9/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/py-modindex.html` & `mly_pipeline-0.5.9/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/runningasearch.html` & `mly_pipeline-0.5.9/docs/build/html/runningasearch.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/search.html` & `mly_pipeline-0.5.9/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/searchindex.js` & `mly_pipeline-0.5.9/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/build/html/settingupasearch.html` & `mly_pipeline-0.5.9/docs/build/html/settingupasearch.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/source/conf.py` & `mly_pipeline-0.5.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/source/index.rst` & `mly_pipeline-0.5.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/source/installation.rst` & `mly_pipeline-0.5.9/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/source/runningasearch.rst` & `mly_pipeline-0.5.9/docs/source/runningasearch.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/source/runningasearchoffline.rst` & `mly_pipeline-0.5.9/docs/source/runningasearchoffline.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/source/runningasearchonline.rst` & `mly_pipeline-0.5.9/docs/source/runningasearchonline.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/docs/source/settingupasearch.rst` & `mly_pipeline-0.5.9/docs/source/settingupasearch.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/mly_pipeline/__init__.py` & `mly_pipeline-0.5.9/mly_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/mly_pipeline/continuous_FAR.py` & `mly_pipeline-0.5.9/mly_pipeline/continuous_FAR.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/mly_pipeline/continuous_FAR_test.py` & `mly_pipeline-0.5.9/mly_pipeline/continuous_FAR_test.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/mly_pipeline/initialization.py` & `mly_pipeline-0.5.9/mly_pipeline/initialization.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/mly_pipeline/make_eff_estimation.py` & `mly_pipeline-0.5.9/mly_pipeline/make_eff_estimation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 #!/usr/bin/env python
-import sys
-# Sourcing the submodule of mly in a very unpythonic way 
-sys.path.append("/".join(sys.argv[0].split("/")[:-1])+"/mly/")
-
 
 import os
-import time ,json, argparse
+import time ,json, argparse, subprocess
+
+import numpy as np
+import pickle
+import matplotlib.pyplot as plt
+
 from pycondor import Job, Dagman
 from mly.datatools import DataSet
 from mly.validators import Validator
 from mly.tools import *
-from functools import partial
-from typing import Callable
-from lal import gpstime
-import numpy as np
-import pickle
-import matplotlib.pyplot as plt
-from search_functions import far, stackVirgo
+
+
+from .search_functions import far, stackVirgo
 
 with open('config.json') as json_file:
     config = json.load(json_file)
 
 config = stackVirgo(config)
 
 os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
 
+which_python = str(subprocess.check_output(['which','python']))[2:-3]
+print(which_python)
 
 # # # Managing arguments
 # 
 # List of arguments to pass:
 arguments = ['mode','injectionPath','injectionSNR','injectionHRSS']
 
 #Construct argument parser:
@@ -96,15 +95,15 @@
                   ,[["strain"], ["strain", "correlation"]]]
 
         # print(models)
         # print(injectionSNR)
         # print(injectionHRSS)
         print('injection_path: ',injection_path)
         t0=time.time()
-        print("savefile",efficiencyDirectory+f"_{injection_path.split('/')[-1]}_{gps_time_start}-{gps_time_end}")
+        print("savefile",efficiencyDirectory+f"{injection_path.split('/')[-1]}_{gps_time_start}-{gps_time_end}")
 
         if 'V' not in config['detectors']:
             efficiencies = Validator.accuracy(models=models, 
                                         duration=1, 
                                         size=size,
                                         fs=1024,
                                         detectors=config['detectors'], 
@@ -271,31 +270,31 @@
         dagman = Dagman(name='efficiencyTestDagman',submit=submit)
 
 
         injection_paths_HRSS =  config["eff_config"]["injectionsWithHRSS"]
         
         injection_paths_SNR = config["eff_config"]["injectionsWithSNR"]
 
-        os.system('chmod 777 '+config["mlyPipelineSource"]+'/make_eff_estimation.py')
         
         job_list=[]
 
         for injection_path in injection_paths_HRSS:
             print(injSourceDir+injection_path)
 
             jobname = injection_path.split('/')[-1]
             print(injSourceDir+injection_path)
-            thearguments = ("--mode=test" 
+            thearguments = ( "-m mly_pipeline.make_eff_estimation"
+                             +" --mode=test" 
                              +" --injectionPath="+injSourceDir+injection_path
                              +" --injectionHRSS="+config['eff_config']['injectionHRSS'])
 
 
 
             job = Job(name = jobname
-                       ,executable = config["mlyPipelineSource"]+"/make_eff_estimation.py"
+                       ,executable = which_python
                        ,arguments = thearguments
                        ,submit=submit
                        ,error=error
                        ,output=output
                        ,log=log
                        ,getenv=True
                        ,dag=dagman
@@ -309,24 +308,25 @@
             
             
             
         for injection_path in injection_paths_SNR:
 
             jobname = injection_path.split('/')[-1]
             print(injSourceDir+injection_path)
-            thearguments = ( "--mode=test"
+            thearguments = ( "-m mly_pipeline.make_eff_estimation"
+                             +" --mode=test" 
                              +" --injectionPath="+injSourceDir+injection_path
                              +" --injectionSNR="+config['eff_config']['injectionSNR'])
 
 
 
 
 
             job = Job(name = jobname
-                       ,executable = config["mlyPipelineSource"]+"/make_eff_estimation.py"
+                       ,executable = which_python
                        ,arguments = thearguments
                        ,submit=submit
                        ,error=error
                        ,output=output
                        ,log=log
                        ,getenv=True
                        ,dag=dagman
@@ -334,16 +334,16 @@
                                     ,"accounting_group="+accounting_group
                                     ,"request_disk            = 64M"])
 
             job_list.append(job)
 
 
         plot_job = Job(name = 'plotJob'
-                   ,executable = config["mlyPipelineSource"]+"/make_eff_estimation.py"
-                   ,arguments = ("--mode=plot")
+                   ,executable = which_python
+                   ,arguments = ("-m mly_pipeline.make_eff_estimation --mode=plot")
                    ,submit=submit
                    ,error=error
                    ,output=output
                    ,log=log
                    ,getenv=True
                    ,dag=dagman
                    ,extra_lines=["accounting_group_user="+accounting_group_user
```

### Comparing `mly_pipeline-0.5.8/mly_pipeline/manager.py` & `mly_pipeline-0.5.9/mly_pipeline/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,16 @@
                 # Removing all the ones we used after we made sure the set is saved.   
                 for each_pod in pod_list[:efficiencyTestBuffer]:
 
                     os.system("rm "+config['bufferDirectory']+"/temp/"+each_pod)
                     
                 # Running the efficiencies script only if the previous has finished.
                 if len(dirlist(config['efficiencies'])) <= 2:
-                    os.system("nohup python "+config["mlyPipelineSource"]+"/make_eff_estimation.py --mode condor > efficiencyTest.out &")
+                    print("RUN EFFICIENCY? YES")
+                    os.system("nohup python -m mly_pipeline.make_eff_estimation --mode condor > efficiencyTest.out &")
                     logger.info(f"Efficiency test initiated")
 
 
         logger.debug(f"PROCESSES before fartest management: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
 
         # # # FAR test management 
         #
```

### Comparing `mly_pipeline-0.5.8/mly_pipeline/mly_to_grace.py` & `mly_pipeline-0.5.9/mly_pipeline/mly_to_grace.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/mly_pipeline/offline_search.py` & `mly_pipeline-0.5.9/mly_pipeline/offline_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,30 +21,28 @@
 import pandas as pd
 
 import gwdatafind
 
 from mly.datatools import DataPod
 from mly.validators import Validator
 from mly.createFileSystem import createFileSysem
-from mly.null_energy_map import *
 from .search_functions import *
 
-from mly.null_energy_map import *
 from ligo.skymap.io import fits
 
 import matplotlib.pyplot as plt
 
 from pycondor import Job, Dagman
 
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'
 os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
 
 
 
-
+which_python = str(subprocess.check_output(['which','python']))[2:-3]
 
 def main(**kwargs):
     """ Main functionality of the search script. Given the arguments
     provided it conducts a real time search on gravitational wave data. It
     uses a predefined given model for iference.
 
     Parameters
@@ -166,15 +164,15 @@
                 continue
 
 
     
             thearguments = ("-m mly_pipeline.offline_search --mode job "+"--i "+str(i))
 
             job = Job(name = jobname
-                    ,executable = "/home/vasileios.skliris/.conda/envs/hermesEnv/bin/python"
+                    ,executable = which_python
                     ,arguments = thearguments
                     ,submit=submit
                     ,error=error
                     ,output=output
                     ,log=log
                     ,getenv=True
                     ,dag=dagman
```

### Comparing `mly_pipeline-0.5.8/mly_pipeline/search.py` & `mly_pipeline-0.5.9/mly_pipeline/search.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/mly_pipeline/search_functions.py` & `mly_pipeline-0.5.9/mly_pipeline/search_functions.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/mly_pipeline/tests/__init__.py` & `mly_pipeline-0.5.9/mly_pipeline/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/mly_pipeline/tests/test_skymap_generation.py` & `mly_pipeline-0.5.9/mly_pipeline/tests/test_skymap_generation.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/mly_pipeline.egg-info/PKG-INFO` & `mly_pipeline-0.5.9/mly_pipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly-pipeline
-Version: 0.5.8
+Version: 0.5.9
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-0.5.8/mly_pipeline.egg-info/SOURCES.txt` & `mly_pipeline-0.5.9/mly_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.8/pyproject.toml` & `mly_pipeline-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>61", "setuptools-scm>=3.4.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mly_pipeline"
-version = "0.5.8"
+version = "0.5.9"
 authors = [
     {name = "Vasileios SKliris", email = "sklirisv@cardiff.ac.uk"},
 ]
 description = "Search pipeline to run online and offline GW searches with mly package."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["ml", "gravitational waves", "bursts"]
```

