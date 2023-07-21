# Comparing `tmp/ricecooker-0.7.2.tar.gz` & `tmp/ricecooker-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ricecooker-0.7.2.tar", last modified: Wed May  3 02:22:10 2023, max compression
+gzip compressed data, was "dist/ricecooker-0.7.3.tar", last modified: Fri Jul 21 21:19:31 2023, max compression
```

## Comparing `ricecooker-0.7.2.tar` & `ricecooker-0.7.3.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-03 02:21:59.000000 ricecooker-0.7.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-03 02:21:59.000000 ricecooker-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-03 02:21:59.000000 ricecooker-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-03 02:22:10.000000 ricecooker-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-03 02:21:59.000000 ricecooker-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/404.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/chefops.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/docs/community/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/community/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/docs/concepts/
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/concepts/content_workflows.md
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/concepts/developer_workflows.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/concepts/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/concepts/introduction.md
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/concepts/reviewing_channels.md
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/concepts/terminology.md
--rw-r--r--   0 runner    (1001) docker     (123)    19873 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/docs/csv_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/csv_metadata/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/csv_metadata/csv_exercises.md
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/csv_metadata/csv_workflow.md
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/csv_metadata/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/developer/corrections.md
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/developer/design_cli.md
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/developer/ids.md
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/developer/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/developer/kolibripreview.md
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/developer/sushops.md
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/developer/uploadprocess.md
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/downloader.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/exercises.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/docs/figures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/docs/figures/HandBrake/
--rw-r--r--   0 runner    (1001) docker     (123)   113089 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/figures/HandBrake/handbrake_steps.png
--rw-r--r--   0 runner    (1001) docker     (123)    48626 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/figures/HandBrake/handbreake_audio_settings.png
--rw-r--r--   0 runner    (1001) docker     (123)    52981 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/figures/HandBrake/handbreake_resizing_settings.png
--rw-r--r--   0 runner    (1001) docker     (123)   242328 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/figures/HandBrake/handbreake_screenshot_video_settings.png
--rw-r--r--   0 runner    (1001) docker     (123)   128604 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/figures/content_pipeline_diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)   144375 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/figures/content_pipeline_diagram_with_highlight.png
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/figures/kolibri_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    39710 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/figures/ricecooker_domain.png
--rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/files.md
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14760 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/htmlapps.md
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/index_api_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/index_utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/languages.md
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    21943 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/nodes.md
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/parsing_html.md
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/pdfutils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/docs/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)    10452 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/tutorial/explanations.md
--rw-r--r--   0 runner    (1001) docker     (123)    13376 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/tutorial/gettingstarted.rst
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/tutorial/jiro.md
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/tutorial/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/tutorial/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)    13551 2023-05-03 02:21:59.000000 ricecooker-0.7.2/docs/video_compression.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/ricecooker/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37099 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/chefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/ricecooker/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52387 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/classes/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/classes/licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)    61722 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/classes/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    25149 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/classes/questions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/ricecooker/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/managers/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/managers/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/ricecooker/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/ricecooker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/caching.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25289 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)    37125 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/html_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/jsontrees.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1240 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/kolibripreview.py
--rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/libstudio.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/linecook.py
--rw-r--r--   0 runner    (1001) docker     (123)    41077 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/metadata_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/thumbscropping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/videos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/web.py
--rw-r--r--   0 runner    (1001) docker     (123)    22252 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/youtube.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-03 02:21:59.000000 ricecooker-0.7.2/ricecooker/utils/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/ricecooker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-03 02:22:09.000000 ricecooker-0.7.2/ricecooker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-03 02:22:10.000000 ricecooker-0.7.2/ricecooker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 02:22:09.000000 ricecooker-0.7.2/ricecooker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-03 02:22:09.000000 ricecooker-0.7.2/ricecooker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 02:22:09.000000 ricecooker-0.7.2/ricecooker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-03 02:22:09.000000 ricecooker-0.7.2/ricecooker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 02:22:09.000000 ricecooker-0.7.2/ricecooker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-03 02:22:10.000000 ricecooker-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-03 02:21:59.000000 ricecooker-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/chefs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/chefs/fake_chef.py
--rw-r--r--   0 runner    (1001) docker     (123)    26802 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/files/
--rw-r--r--   0 runner    (1001) docker     (123)    27648 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/Wilhelm_Scream.mp3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/files/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/files/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/assets/css/empty.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/assets/css/empty2.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/files/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/assets/images/4933759886_098e9acf93_m.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/assets/images/copyright.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/files/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/assets/js/empty.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/files/audio/
--rw-r--r--   0 runner    (1001) docker     (123)   764176 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/audio/file_example_MP3_700KB.mp3
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/file_metadata.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/files/generate_thumbnail/
--rw-r--r--   0 runner    (1001) docker     (123)   318539 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/generate_thumbnail/sample.epub
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/generate_thumbnail/sample.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/generate_thumbnail/sample.zip
--rw-r--r--   0 runner    (1001) docker     (123)  5033338 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/kepub.epub
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/page_with_links.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/files/subtitles/
--rw-r--r--   0 runner    (1001) docker     (123)    22759 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/subtitles/basic.srt
--rw-r--r--   0 runner    (1001) docker     (123)    20575 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/subtitles/basic.vtt
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/subtitles/empty.ttml
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/subtitles/encapsulated.sami
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/subtitles/encapsulated.vtt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/subtitles/not.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/media_utils/files/thumbnails/
--rw-r--r--   0 runner    (1001) docker     (123)   163118 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/thumbnails/BRAlogo1.png
--rw-r--r--   0 runner    (1001) docker     (123)   142272 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/thumbnails/toosquare.png
--rw-r--r--   0 runner    (1001) docker     (123)    63258 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/thumbnails/tootall.png
--rw-r--r--   0 runner    (1001) docker     (123)    49913 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/files/thumbnails/toowide.png
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/test_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/test_subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/test_thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/test_videos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/test_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/media_utils/test_youtube.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_chef_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_csv_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    23745 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_exercises.py
--rw-r--r--   0 runner    (1001) docker     (123)    19221 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_pdfutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    15234 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (123)    19584 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_videos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/test_youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/testchannels/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/Channel.csv
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/Content.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/ExerciseQuestions.csv
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/Exercises.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/
--rw-r--r--   0 runner    (1001) docker     (123)    23858 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/algebra_exercise_thumb.png
--rw-r--r--   0 runner    (1001) docker     (123)    37428 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/channel_thumbnail.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/contentnodes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/contentnodes/audio/
--rw-r--r--   0 runner    (1001) docker     (123)   114608 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/contentnodes/audio/WZ_exercise_thumbnail.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:22:10.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/exercises/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:21:59.000000 ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/exercises/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-21 21:19:18.000000 ricecooker-0.7.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-21 21:19:18.000000 ricecooker-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-21 21:19:18.000000 ricecooker-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-07-21 21:19:31.000000 ricecooker-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-21 21:19:18.000000 ricecooker-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/404.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/chefops.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/docs/community/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/community/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/docs/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/concepts/content_workflows.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/concepts/developer_workflows.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/concepts/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/concepts/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/concepts/reviewing_channels.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/concepts/terminology.md
+-rw-r--r--   0 runner    (1001) docker     (123)    19873 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/docs/csv_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/csv_metadata/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/csv_metadata/csv_exercises.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/csv_metadata/csv_workflow.md
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/csv_metadata/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/developer/corrections.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/developer/design_cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/developer/ids.md
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/developer/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/developer/kolibripreview.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/developer/sushops.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/developer/uploadprocess.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/downloader.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/exercises.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/docs/figures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/docs/figures/HandBrake/
+-rw-r--r--   0 runner    (1001) docker     (123)   113089 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/figures/HandBrake/handbrake_steps.png
+-rw-r--r--   0 runner    (1001) docker     (123)    48626 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/figures/HandBrake/handbreake_audio_settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52981 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/figures/HandBrake/handbreake_resizing_settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)   242328 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/figures/HandBrake/handbreake_screenshot_video_settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)   128604 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/figures/content_pipeline_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)   144375 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/figures/content_pipeline_diagram_with_highlight.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/figures/kolibri_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39710 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/figures/ricecooker_domain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/files.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14760 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/htmlapps.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/index_api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/index_utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/languages.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    21943 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/nodes.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/parsing_html.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/pdfutils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)    10452 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/tutorial/explanations.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13376 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/tutorial/gettingstarted.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/tutorial/jiro.md
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/tutorial/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/tutorial/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13551 2023-07-21 21:19:18.000000 ricecooker-0.7.3/docs/video_compression.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/ricecooker/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37099 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/chefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/ricecooker/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52439 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/classes/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/classes/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64763 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/classes/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25149 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/classes/questions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/ricecooker/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/managers/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/managers/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/ricecooker/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/ricecooker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/caching.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25289 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37125 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/html_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/jsontrees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1240 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/kolibripreview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/libstudio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/linecook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41077 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/metadata_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/thumbscropping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/videos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22252 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/youtube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-21 21:19:18.000000 ricecooker-0.7.3/ricecooker/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/ricecooker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-07-21 21:19:31.000000 ricecooker-0.7.3/ricecooker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-21 21:19:31.000000 ricecooker-0.7.3/ricecooker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 21:19:31.000000 ricecooker-0.7.3/ricecooker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-21 21:19:31.000000 ricecooker-0.7.3/ricecooker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 21:19:31.000000 ricecooker-0.7.3/ricecooker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-21 21:19:31.000000 ricecooker-0.7.3/ricecooker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 21:19:31.000000 ricecooker-0.7.3/ricecooker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-21 21:19:31.000000 ricecooker-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-21 21:19:18.000000 ricecooker-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/tests/chefs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/chefs/fake_chef.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26825 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/tests/media_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/tests/media_utils/files/
+-rw-r--r--   0 runner    (1001) docker     (123)    27648 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/Wilhelm_Scream.mp3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/tests/media_utils/files/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/tests/media_utils/files/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/assets/css/empty.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/assets/css/empty2.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/tests/media_utils/files/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/assets/images/4933759886_098e9acf93_m.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/assets/images/copyright.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/tests/media_utils/files/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/assets/js/empty.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/tests/media_utils/files/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)   764176 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/audio/file_example_MP3_700KB.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/file_metadata.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/tests/media_utils/files/generate_thumbnail/
+-rw-r--r--   0 runner    (1001) docker     (123)   318539 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/generate_thumbnail/sample.epub
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/generate_thumbnail/sample.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/generate_thumbnail/sample.zip
+-rw-r--r--   0 runner    (1001) docker     (123)  5033338 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/kepub.epub
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/page_with_links.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/tests/media_utils/files/subtitles/
+-rw-r--r--   0 runner    (1001) docker     (123)    22759 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/subtitles/basic.srt
+-rw-r--r--   0 runner    (1001) docker     (123)    20575 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/subtitles/basic.vtt
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/subtitles/empty.ttml
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/subtitles/encapsulated.sami
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/subtitles/encapsulated.vtt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/subtitles/not.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/tests/media_utils/files/thumbnails/
+-rw-r--r--   0 runner    (1001) docker     (123)   163118 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/thumbnails/BRAlogo1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   142272 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/thumbnails/toosquare.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63258 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/thumbnails/tootall.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49913 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/files/thumbnails/toowide.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/test_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/test_subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/test_thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/test_videos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/media_utils/test_youtube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/test_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/test_chef_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/test_csv_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23745 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/test_exercises.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19225 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/test_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/test_pdfutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15234 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/test_thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23084 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/test_videos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/test_youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/tests/testchannels/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/tests/testchannels/csv_channel_with_exercises/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/testchannels/csv_channel_with_exercises/Channel.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/testchannels/csv_channel_with_exercises/Content.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/testchannels/csv_channel_with_exercises/ExerciseQuestions.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/testchannels/csv_channel_with_exercises/Exercises.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/tests/testchannels/csv_channel_with_exercises/channeldir/
+-rw-r--r--   0 runner    (1001) docker     (123)    23858 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/testchannels/csv_channel_with_exercises/channeldir/algebra_exercise_thumb.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37428 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/testchannels/csv_channel_with_exercises/channeldir/channel_thumbnail.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/tests/testchannels/csv_channel_with_exercises/channeldir/contentnodes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/tests/testchannels/csv_channel_with_exercises/channeldir/contentnodes/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)   114608 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/testchannels/csv_channel_with_exercises/channeldir/contentnodes/audio/WZ_exercise_thumbnail.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:31.000000 ricecooker-0.7.3/tests/testchannels/csv_channel_with_exercises/channeldir/exercises/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:18.000000 ricecooker-0.7.3/tests/testchannels/csv_channel_with_exercises/channeldir/exercises/.gitkeep
```

### Comparing `ricecooker-0.7.2/LICENSE` & `ricecooker-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/PKG-INFO` & `ricecooker-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ricecooker
-Version: 0.7.2
+Version: 0.7.3
 Summary: API for adding content to the Kolibri content curation server
 Home-page: https://github.com/learningequality/ricecooker
 Author: Learning Equality
 Author-email: dev@learningequality.org
 License: MIT license
 Description: ricecooker
         ==========
```

### Comparing `ricecooker-0.7.2/README.md` & `ricecooker-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/Makefile` & `ricecooker-0.7.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/README.rst` & `ricecooker-0.7.3/docs/README.rst`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/chefops.md` & `ricecooker-0.7.3/docs/chefops.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/concepts/content_workflows.md` & `ricecooker-0.7.3/docs/concepts/content_workflows.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/concepts/developer_workflows.md` & `ricecooker-0.7.3/docs/concepts/developer_workflows.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/concepts/introduction.md` & `ricecooker-0.7.3/docs/concepts/introduction.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/concepts/reviewing_channels.md` & `ricecooker-0.7.3/docs/concepts/reviewing_channels.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/concepts/terminology.md` & `ricecooker-0.7.3/docs/concepts/terminology.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/conf.py` & `ricecooker-0.7.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/csv_metadata/csv_exercises.md` & `ricecooker-0.7.3/docs/csv_metadata/csv_exercises.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/csv_metadata/csv_workflow.md` & `ricecooker-0.7.3/docs/csv_metadata/csv_workflow.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/developer/corrections.md` & `ricecooker-0.7.3/docs/developer/corrections.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/developer/design_cli.md` & `ricecooker-0.7.3/docs/developer/design_cli.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/developer/ids.md` & `ricecooker-0.7.3/docs/developer/ids.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/developer/kolibripreview.md` & `ricecooker-0.7.3/docs/developer/kolibripreview.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/developer/sushops.md` & `ricecooker-0.7.3/docs/developer/sushops.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/developer/uploadprocess.md` & `ricecooker-0.7.3/docs/developer/uploadprocess.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/downloader.md` & `ricecooker-0.7.3/docs/downloader.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/examples/index.rst` & `ricecooker-0.7.3/docs/examples/index.rst`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/exercises.md` & `ricecooker-0.7.3/docs/exercises.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/figures/HandBrake/handbrake_steps.png` & `ricecooker-0.7.3/docs/figures/HandBrake/handbrake_steps.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/figures/HandBrake/handbreake_audio_settings.png` & `ricecooker-0.7.3/docs/figures/HandBrake/handbreake_audio_settings.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/figures/HandBrake/handbreake_resizing_settings.png` & `ricecooker-0.7.3/docs/figures/HandBrake/handbreake_resizing_settings.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/figures/HandBrake/handbreake_screenshot_video_settings.png` & `ricecooker-0.7.3/docs/figures/HandBrake/handbreake_screenshot_video_settings.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/figures/content_pipeline_diagram.png` & `ricecooker-0.7.3/docs/figures/content_pipeline_diagram.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/figures/content_pipeline_diagram_with_highlight.png` & `ricecooker-0.7.3/docs/figures/content_pipeline_diagram_with_highlight.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/figures/kolibri_logo.png` & `ricecooker-0.7.3/docs/figures/kolibri_logo.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/figures/ricecooker_domain.png` & `ricecooker-0.7.3/docs/figures/ricecooker_domain.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/files.md` & `ricecooker-0.7.3/docs/files.md`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
 
 Document files
 --------------
 Use the `DocumentFile` class to add PDF documents:
 
     document_file = DocumentFile(
-        path='dir/subdir/lecture_slides.mp4',
+        path='dir/subdir/lecture_slides.pdf',
         language=getlang('en').code
     )
 
 Use the `EPubFile` class to add ePub documents:
 
     document_file = EPubFile(
         path='dir/subdir/lecture_slides.epub',
```

### Comparing `ricecooker-0.7.2/docs/history.rst` & `ricecooker-0.7.3/docs/history.rst`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/htmlapps.md` & `ricecooker-0.7.3/docs/htmlapps.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/index.rst` & `ricecooker-0.7.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/index_api_reference.rst` & `ricecooker-0.7.3/docs/index_api_reference.rst`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/installation.md` & `ricecooker-0.7.3/docs/installation.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/languages.md` & `ricecooker-0.7.3/docs/languages.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/make.bat` & `ricecooker-0.7.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/nodes.md` & `ricecooker-0.7.3/docs/nodes.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/parsing_html.md` & `ricecooker-0.7.3/docs/parsing_html.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/pdfutils.md` & `ricecooker-0.7.3/docs/pdfutils.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/tutorial/explanations.md` & `ricecooker-0.7.3/docs/tutorial/explanations.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/tutorial/gettingstarted.rst` & `ricecooker-0.7.3/docs/tutorial/gettingstarted.rst`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/tutorial/jiro.md` & `ricecooker-0.7.3/docs/tutorial/jiro.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/tutorial/quickstart.rst` & `ricecooker-0.7.3/docs/tutorial/quickstart.rst`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/tutorial/tutorial.rst` & `ricecooker-0.7.3/docs/tutorial/tutorial.rst`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/usage.md` & `ricecooker-0.7.3/docs/usage.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/docs/video_compression.md` & `ricecooker-0.7.3/docs/video_compression.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/chefs.py` & `ricecooker-0.7.3/ricecooker/chefs.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/classes/files.py` & `ricecooker-0.7.3/ricecooker/classes/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -1387,28 +1387,28 @@
         ) as tempf:
             tempf.close()
             create_tiled_image(images, tempf.name)
             filename = copy_file_to_storage(tempf.name, ext=file_formats.PNG)
             return filename
 
 
-class RemoteFile(File):
+class StudioFile(File):
     """
-    Reuse a file that we already know to exist on the remote (normally Studio).
+    Reuse a file that we already know to exist on the remote (Studio).
     This allows for channels to be updated without having to redownload all files again.
     """
 
     skip_upload = True
 
     def __init__(self, checksum, ext, preset, is_primary=False, **kwargs):
         self.filename = "{}.{}".format(checksum, ext)
         self.is_primary = is_primary
         kwargs["preset"] = preset
         self._validated = False
-        super(RemoteFile, self).__init__(**kwargs)
+        super(StudioFile, self).__init__(**kwargs)
 
     def validate(self):
         if not self._validated:
             file_url = config.get_storage_url(self.filename)
             response = config.DOWNLOAD_SESSION.head(file_url)
             try:
                 response.raise_for_status()
@@ -1418,7 +1418,11 @@
                         self.filename, e
                     )
                 )
             self._validated = True
 
     def __str__(self):
         return self.filename
+
+
+# add alias for back-compatibility
+RemoteFile = StudioFile
```

### Comparing `ricecooker-0.7.2/ricecooker/classes/licenses.py` & `ricecooker-0.7.3/ricecooker/classes/licenses.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/classes/nodes.py` & `ricecooker-0.7.3/ricecooker/classes/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from le_utils.constants.labels import needs
 from le_utils.constants.labels import resource_type
 from le_utils.constants.labels import subjects
 
 from .. import __version__
 from .. import config
 from ..exceptions import InvalidNodeException
+from ..utils.utils import is_valid_uuid_string
 from .licenses import License
 
 MASTERY_MODELS = [id for id, name in exercises.MASTERY_MODELS]
 ROLES = [id for id, name in roles.choices]
 
 
 class Node(object):
@@ -465,14 +466,15 @@
         domain_ns=None,
         grade_levels=None,
         resource_types=None,
         learning_activities=None,
         accessibility_labels=None,
         categories=None,
         learner_needs=None,
+        role=roles.LEARNER,
         **kwargs
     ):
         # Map parameters to model variables
         assert isinstance(source_id, str), "source_id must be a string"
         self.source_id = source_id
         self.author = author or ""
         self.aggregator = aggregator or ""
@@ -486,14 +488,15 @@
 
         self.grade_levels = grade_levels or []
         self.resource_types = resource_types or []
         self.learning_activities = learning_activities or []
         self.accessibility_labels = accessibility_labels or []
         self.categories = categories or []
         self.learner_needs = learner_needs or []
+        self.role = role
 
         super(TreeNode, self).__init__(title, **kwargs)
 
     def get_domain_namespace(self):
         if not self.domain_ns:
             self.domain_ns = self.parent.get_domain_namespace()
         return self.domain_ns
@@ -584,17 +587,18 @@
             "extra_fields": json.dumps(self.extra_fields),
             "grade_levels": self.grade_levels,
             "resource_types": self.resource_types,
             "learning_activities": self.learning_activities,
             "accessibility_labels": self.accessibility_labels,
             "categories": self.categories,
             "learner_needs": self.learner_needs,
+            "role": self.role,
         }
 
-    def validate(self):
+    def validate(self):  # noqa: C901
         """validate: Makes sure content node is valid
         Args: None
         Returns: boolean indicating if content node is valid
         """
         assert isinstance(self.author, str), "Assumption Failed: Author is not a string"
         assert isinstance(
             self.aggregator, str
@@ -611,14 +615,76 @@
         ), "Assumption Failed: Extra fields is not a dict"
         assert isinstance(self.tags, list), "Assumption Failed: Tags is not a list"
         for tag in self.tags:
             assert isinstance(tag, str), "Assumption Failed: Tag is not a string"
             assert len(tag) <= 30, (
                 "ERROR: tag " + tag + " is too long. Tags should be 30 chars or less."
             )
+
+        assert (
+            self.role in ROLES
+        ), "Assumption Failed: Role must be one of the following {}".format(ROLES)
+        if self.grade_levels is not None:
+            for grade in self.grade_levels:
+                assert (
+                    grade in levels.LEVELSLIST
+                ), "Assumption Failed: Grade levels must be one of the following {}".format(
+                    levels.LEVELSLIST
+                )
+
+        if self.resource_types is not None:
+            for res_type in self.resource_types:
+                assert (
+                    res_type in resource_type.RESOURCETYPELIST
+                ), "Assumption Failed: Resource types must be one of the following {}".format(
+                    resource_type.RESOURCETYPELIST
+                )
+
+        if self.learning_activities is not None:
+            assert isinstance(
+                self.learning_activities, list
+            ), "Assumption Failed: Learning activities must be list"
+            for learn_act in self.learning_activities:
+                assert (
+                    learn_act in learning_activities.LEARNINGACTIVITIESLIST
+                ), "Assumption Failed: Learning activities must be one of the following {}".format(
+                    learning_activities.LEARNINGACTIVITIESLIST
+                )
+        if self.accessibility_labels is not None:
+            assert isinstance(
+                self.accessibility_labels, list
+            ), "Assumption Failed: Accessibility label must be list"
+            for access_label in self.accessibility_labels:
+                assert (
+                    access_label in accessibility_categories.ACCESSIBILITYCATEGORIESLIST
+                ), "Assumption Failed: Accessibility label must be one of the following {}".format(
+                    accessibility_categories.ACCESSIBILITYCATEGORIESLIST
+                )
+        if self.categories is not None:
+            assert isinstance(
+                self.categories, list
+            ), "Assumption Failed: Categories must be list"
+            for category in self.categories:
+                assert (
+                    category in subjects.SUBJECTSLIST
+                ), "Assumption Failed: Categories must be one of the following {}".format(
+                    subjects.SUBJECTSLIST
+                )
+
+        if self.learner_needs is not None:
+            assert isinstance(
+                self.learner_needs, list
+            ), "Assumption Failed: Learner needs must be list"
+            for learner_need in self.learner_needs:
+                assert (
+                    learner_need in needs.NEEDSLIST
+                ), "Assumption Failed: Learner needs must be one of the following {}".format(
+                    needs.NEEDSLIST
+                )
+
         return super(TreeNode, self).validate()
 
 
 class TopicNode(TreeNode):
     """Model representing channel topics
 
     Topic nodes are used to add organization to the channel's content
@@ -683,27 +749,18 @@
     required_file_format = None
 
     def __init__(
         self,
         source_id,
         title,
         license,
-        role=roles.LEARNER,
         license_description=None,
         copyright_holder=None,
-        grade_levels=None,
-        resource_types=None,
-        learning_activities=None,
-        accessibility_labels=None,
-        categories=None,
-        learner_needs=None,
         **kwargs
     ):
-        self.role = role
-
         self.set_license(
             license, copyright_holder=copyright_holder, description=license_description
         )
         super(ContentNode, self).__init__(source_id, title, **kwargs)
 
     def __str__(self):
         metadata = "{0} {1}".format(
@@ -724,75 +781,14 @@
         self.license = license
 
     def validate(self):  # noqa F401
         """validate: Makes sure content node is valid
         Args: None
         Returns: boolean indicating if content node is valid
         """
-        assert (
-            self.role in ROLES
-        ), "Assumption Failed: Role must be one of the following {}".format(ROLES)
-        if self.grade_levels is not None:
-            for grade in self.grade_levels:
-                assert (
-                    grade in levels.LEVELSLIST
-                ), "Assumption Failed: Grade levels must be one of the following {}".format(
-                    levels.LEVELSLIST
-                )
-
-        if self.resource_types is not None:
-            for res_type in self.resource_types:
-                assert (
-                    res_type in resource_type.RESOURCETYPELIST
-                ), "Assumption Failed: Resource types must be one of the following {}".format(
-                    resource_type.RESOURCETYPELIST
-                )
-
-        if self.learning_activities is not None:
-            assert isinstance(
-                self.learning_activities, list
-            ), "Assumption Failed: Learning activities must be list"
-            for learn_act in self.learning_activities:
-                assert (
-                    learn_act in learning_activities.LEARNINGACTIVITIESLIST
-                ), "Assumption Failed: Learning activities must be one of the following {}".format(
-                    learning_activities.LEARNINGACTIVITIESLIST
-                )
-        if self.accessibility_labels is not None:
-            assert isinstance(
-                self.accessibility_labels, list
-            ), "Assumption Failed: Accessibility label must be list"
-            for access_label in self.accessibility_labels:
-                assert (
-                    access_label in accessibility_categories.ACCESSIBILITYCATEGORIESLIST
-                ), "Assumption Failed: Accessibility label must be one of the following {}".format(
-                    accessibility_categories.ACCESSIBILITYCATEGORIESLIST
-                )
-        if self.categories is not None:
-            assert isinstance(
-                self.categories, list
-            ), "Assumption Failed: Categories must be list"
-            for category in self.categories:
-                assert (
-                    category in subjects.SUBJECTSLIST
-                ), "Assumption Failed: Categories must be one of the following {}".format(
-                    subjects.SUBJECTSLIST
-                )
-
-        if self.learner_needs is not None:
-            assert isinstance(
-                self.learner_needs, list
-            ), "Assumption Failed: Learner needs must be list"
-            for learner_need in self.learner_needs:
-                assert (
-                    learner_need in needs.NEEDSLIST
-                ), "Assumption Failed: Learner needs must be one of the following {}".format(
-                    needs.NEEDSLIST
-                )
-
         assert isinstance(self.license, str) or isinstance(
             self.license, License
         ), "Assumption Failed: License is not a string or license object"
         self.license.validate()
         # if self.required_file_format:
         #     files_valid = False
         #     #not any(f for f in self.files if isinstance(f, DownloadFile))
@@ -882,15 +878,15 @@
 
     def validate(self):
         """validate: Makes sure video is valid
         Args: None
         Returns: boolean indicating if video is valid
         """
         from .files import (
-            RemoteFile,
+            StudioFile,
             VideoFile,
             WebVideoFile,
             SubtitleFile,
             YouTubeSubtitleFile,
         )
 
         try:
@@ -904,15 +900,15 @@
             # Check if there are any .mp4 files if there are video files (other video types don't have paths)
             assert any(
                 f
                 for f in self.files
                 if isinstance(f, VideoFile)
                 or isinstance(f, WebVideoFile)
                 or (
-                    isinstance(f, RemoteFile)
+                    isinstance(f, StudioFile)
                     and f.preset
                     in (format_presets.VIDEO_HIGH_RES, format_presets.VIDEO_LOW_RES)
                 )
             ), "Assumption Failed: Video node should have at least one video file"
 
             # Ensure that there is only one subtitle file per language code
             new_files = []
@@ -970,15 +966,15 @@
     required_file_format = file_formats.MP3
 
     def validate(self):
         """validate: Makes sure audio is valid
         Args: None
         Returns: boolean indicating if audio is valid
         """
-        from .files import AudioFile, RemoteFile
+        from .files import AudioFile, StudioFile
 
         try:
             assert (
                 self.kind == content_kinds.AUDIO
             ), "Assumption Failed: Node should be audio"
             assert (
                 self.questions == []
@@ -986,15 +982,15 @@
             assert (
                 len(self.files) > 0
             ), "Assumption Failed: Audio should have at least one file"
             assert [
                 f
                 for f in self.files
                 if isinstance(f, AudioFile)
-                or (isinstance(f, RemoteFile) and f.preset == format_presets.AUDIO)
+                or (isinstance(f, StudioFile) and f.preset == format_presets.AUDIO)
             ], "Assumption Failed: Audio should have at least one audio file"
             return super(AudioNode, self).validate()
         except AssertionError as ae:
             raise InvalidNodeException(
                 "Invalid node ({}): {} - {}".format(
                     ae.args[0], self.title, self.__dict__
                 )
@@ -1025,15 +1021,15 @@
     required_file_format = file_formats.PDF  # TODO(ivan) change ro allowed_formats
 
     def validate(self):
         """validate: Makes sure document node contains at least one EPUB or PDF
         Args: None
         Returns: boolean indicating if document is valid
         """
-        from .files import DocumentFile, EPubFile, RemoteFile
+        from .files import DocumentFile, EPubFile, StudioFile
 
         try:
             assert (
                 self.kind == content_kinds.DOCUMENT
             ), "Assumption Failed: Node should be a document"
             assert (
                 self.questions == []
@@ -1043,15 +1039,15 @@
             ), "Assumption Failed: Document should have at least one file"
             assert [
                 f
                 for f in self.files
                 if isinstance(f, DocumentFile)
                 or isinstance(f, EPubFile)
                 or (
-                    isinstance(f, RemoteFile)
+                    isinstance(f, StudioFile)
                     and f.preset in (format_presets.DOCUMENT, format_presets.EPUB)
                 )
             ], "Assumption Failed: Document should have at least one document file"
             return super(DocumentNode, self).validate()
         except AssertionError as ae:
             raise InvalidNodeException(
                 "Invalid node ({}): {} - {}".format(
@@ -1125,28 +1121,28 @@
             return None
 
     def validate(self):
         """validate: Makes sure HTML5 app is valid
         Args: None
         Returns: boolean indicating if HTML5 app is valid
         """
-        from .files import HTMLZipFile, RemoteFile
+        from .files import HTMLZipFile, StudioFile
 
         try:
             assert (
                 self.kind == content_kinds.HTML5
             ), "Assumption Failed: Node should be an HTML5 app"
             assert (
                 self.questions == []
             ), "Assumption Failed: HTML should not have questions"
             assert [
                 f
                 for f in self.files
                 if isinstance(f, HTMLZipFile)
-                or (isinstance(f, RemoteFile) and f.preset == format_presets.HTML5_ZIP)
+                or (isinstance(f, StudioFile) and f.preset == format_presets.HTML5_ZIP)
             ], "Assumption Failed: HTML should have at least one html file"
             return super(HTML5AppNode, self).validate()
         except AssertionError as ae:
             raise InvalidNodeException(
                 "Invalid node ({}): {} - {}".format(
                     ae.args[0], self.title, self.__dict__
                 )
@@ -1176,28 +1172,28 @@
     required_file_format = file_formats.H5P
 
     def validate(self):
         """validate: Makes sure H5P app is valid
         Args: None
         Returns: boolean indicating if H5P app is valid
         """
-        from .files import H5PFile, RemoteFile
+        from .files import H5PFile, StudioFile
 
         try:
             assert (
                 self.kind == content_kinds.H5P
             ), "Assumption Failed: Node should be an H5P app"
             assert (
                 self.questions == []
             ), "Assumption Failed: HTML should not have questions"
             assert [
                 f
                 for f in self.files
                 if isinstance(f, H5PFile)
-                or (isinstance(f, RemoteFile) and f.preset == format_presets.H5P_ZIP)
+                or (isinstance(f, StudioFile) and f.preset == format_presets.H5P_ZIP)
             ], "Assumption Failed: H5PAppNode should have at least one h5p file"
             return super(H5PAppNode, self).validate()
         except AssertionError as ae:
             raise InvalidNodeException(
                 "Invalid node ({}): {} - {}".format(
                     ae.args[0], self.title, self.__dict__
                 )
@@ -1559,7 +1555,95 @@
 
     def __init__(self, *args, **kwargs):
         kwargs["exercise_data"] = kwargs.get("exercise_data", {})
         kwargs["exercise_data"]["options"] = kwargs["exercise_data"].get("options", {})
         # TODO: update le-utils version and use a constant value here
         kwargs["exercise_data"]["options"].update({"modality": "QUIZ"})
         super(PracticeQuizNode, self).__init__(*args, **kwargs)
+
+
+class StudioContentNode(TreeNode):
+    """
+    Node class for creating content nodes in the channel that are imported from
+    existing nodes in another channel on Studio.
+
+    Notes:
+    - Your account must have read permissions for the target node.
+    - You must specify the source_channel_id, and at least one of source_node_id or source_content_id.
+    - If you specify both source_node_id and source_content_id, the source_node_id will be used,
+      and it will fallback to looking up by source_content_id if source_node_id is not found.
+    """
+
+    kind = "remotecontent"
+
+    ALLOWED_OVERRIDES = [
+        "title",
+        "description",
+        "aggregator",
+        "provider",
+        "tags",
+        "grade_levels",
+        "resource_types",
+        "learning_activities",
+        "accessibility_labels",
+        "categories",
+        "learner_needs",
+        "role",
+        "thumbnail",
+        "extra_fields",
+        "suggested_duration",
+    ]
+
+    def __init__(
+        self, source_channel_id, source_node_id=None, source_content_id=None, **kwargs
+    ):
+        self.source_channel_id = (
+            source_channel_id if is_valid_uuid_string(source_channel_id) else None
+        )
+        self.source_node_id = (
+            source_node_id if is_valid_uuid_string(source_node_id) else None
+        )
+        self.source_content_id = (
+            source_content_id if is_valid_uuid_string(source_content_id) else None
+        )
+        self.overrides = kwargs.copy()
+        overriden_title = kwargs.pop("title", "<title from remote>")
+        super(StudioContentNode, self).__init__(
+            source_node_id or source_content_id, overriden_title, **kwargs
+        )
+
+    def validate(self):
+        if not self.source_channel_id:
+            raise InvalidNodeException(
+                "Invalid node: source_channel_id must be specified, and be a valid UUID string."
+            )
+        if not self.source_node_id and not self.source_content_id:
+            raise InvalidNodeException(
+                "Invalid node: at least one of source_node_id or source_content_id must be specified, and be a valid UUID string."
+            )
+        for key in self.overrides:
+            if key not in self.ALLOWED_OVERRIDES:
+                raise InvalidNodeException(
+                    "Invalid node: '{}' cannot be overriden on a StudioContentNode.".format(
+                        key
+                    )
+                )
+        super(StudioContentNode, self).validate()
+
+    def to_dict(self):
+        data = {
+            "node_id": self.get_node_id().hex if self.parent else "",
+            "source_channel_id": self.source_channel_id,
+            "source_node_id": self.source_node_id,
+            "source_content_id": self.source_content_id,
+        }
+        if "thumbnail" in self.overrides:
+            self.overrides["files"] = [
+                f.to_dict() for f in self.files if f and f.filename
+            ]
+            del self.overrides["thumbnail"]
+        data.update(self.overrides)
+        return data
+
+
+# add alias for back-compatibility
+RemoteContentNode = StudioContentNode
```

### Comparing `ricecooker-0.7.2/ricecooker/classes/questions.py` & `ricecooker-0.7.3/ricecooker/classes/questions.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/cli.py` & `ricecooker-0.7.3/ricecooker/cli.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/commands.py` & `ricecooker-0.7.3/ricecooker/commands.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/config.py` & `ricecooker-0.7.3/ricecooker/config.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/exceptions.py` & `ricecooker-0.7.3/ricecooker/exceptions.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/managers/progress.py` & `ricecooker-0.7.3/ricecooker/managers/progress.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/managers/tree.py` & `ricecooker-0.7.3/ricecooker/managers/tree.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/audio.py` & `ricecooker-0.7.3/ricecooker/utils/audio.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/browser.py` & `ricecooker-0.7.3/ricecooker/utils/browser.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/caching.py` & `ricecooker-0.7.3/ricecooker/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/corrections.py` & `ricecooker-0.7.3/ricecooker/utils/corrections.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/downloader.py` & `ricecooker-0.7.3/ricecooker/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/encodings.py` & `ricecooker-0.7.3/ricecooker/utils/encodings.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/html.py` & `ricecooker-0.7.3/ricecooker/utils/html.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/html_writer.py` & `ricecooker-0.7.3/ricecooker/utils/html_writer.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/images.py` & `ricecooker-0.7.3/ricecooker/utils/images.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/jsontrees.py` & `ricecooker-0.7.3/ricecooker/utils/jsontrees.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,15 +363,15 @@
                     caption=f.get("caption", ""),
                     descriptive_text=f.get("descriptive_text", ""),
                 )
             )
 
         elif file_type == REMOTE_FILE:
             node.add_file(
-                files.RemoteFile(
+                files.StudioFile(
                     f["checksum"],
                     f["ext"],
                     preset,
                     is_primary=f.get("is_primary", False),
                     language=f.get("language"),
                     source_url=f.get("source_url"),
                 )
```

### Comparing `ricecooker-0.7.2/ricecooker/utils/kolibripreview.py` & `ricecooker-0.7.3/ricecooker/utils/kolibripreview.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/libstudio.py` & `ricecooker-0.7.3/ricecooker/utils/libstudio.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/linecook.py` & `ricecooker-0.7.3/ricecooker/utils/linecook.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/metadata_provider.py` & `ricecooker-0.7.3/ricecooker/utils/metadata_provider.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/paths.py` & `ricecooker-0.7.3/ricecooker/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/pdf.py` & `ricecooker-0.7.3/ricecooker/utils/pdf.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/proxy.py` & `ricecooker-0.7.3/ricecooker/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/subtitles.py` & `ricecooker-0.7.3/ricecooker/utils/subtitles.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/thumbscropping.py` & `ricecooker-0.7.3/ricecooker/utils/thumbscropping.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/tokens.py` & `ricecooker-0.7.3/ricecooker/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/videos.py` & `ricecooker-0.7.3/ricecooker/utils/videos.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/web.py` & `ricecooker-0.7.3/ricecooker/utils/web.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/youtube.py` & `ricecooker-0.7.3/ricecooker/utils/youtube.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker/utils/zip.py` & `ricecooker-0.7.3/ricecooker/utils/zip.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/ricecooker.egg-info/PKG-INFO` & `ricecooker-0.7.3/ricecooker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ricecooker
-Version: 0.7.2
+Version: 0.7.3
 Summary: API for adding content to the Kolibri content curation server
 Home-page: https://github.com/learningequality/ricecooker
 Author: Learning Equality
 Author-email: dev@learningequality.org
 License: MIT license
 Description: ricecooker
         ==========
```

### Comparing `ricecooker-0.7.2/ricecooker.egg-info/SOURCES.txt` & `ricecooker-0.7.3/ricecooker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/setup.py` & `ricecooker-0.7.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,43 +7,14 @@
 
 
 readme = open("README.md").read()
 
 with open("docs/history.rst") as history_file:
     history = history_file.read()
 
-requirements = [
-    "pytest>=3.0.2",
-    "requests>=2.11.1",
-    "le_utils>=0.1.26",
-    "validators",  # TODO: check if this is necessary
-    "requests_file",
-    "beautifulsoup4>=4.6.3,<4.9.0",  # pinned to match versions in le-pycaption
-    "selenium==3.0.1",
-    "yt-dlp>=2023.3.4",
-    "html5lib",
-    "cachecontrol==0.12.0",
-    "lockfile==0.12.2",  # TODO: check if this is necessary
-    "css-html-js-minify==2.2.2",
-    "mock==2.0.0",
-    "pypdf2==1.26.0",
-    "dictdiffer>=0.8.0",
-    "Pillow==8.4.0",
-    "colorlog>=4.1.0,<4.2",
-    "PyYAML>=5.3.1",
-    "Jinja2>=2.10",
-    "chardet==4.0.0",
-    "ffmpy>=0.2.2",
-    "pdf2image==1.11.0",
-    "le-pycaption>=2.2.0a1",
-    "EbookLib>=0.17.1",
-    "filetype>=1.1.0",
-]
-
-
 setup(
     name="ricecooker",
     version=ricecooker.__version__,
     description="API for adding content to the Kolibri content curation server",
     long_description=readme + "\n\n" + history,
     long_description_content_type="text/markdown",
     author="Learning Equality",
@@ -54,15 +25,39 @@
     entry_points={
         "console_scripts": [
             "corrections = ricecooker.utils.corrections:correctionsmain",
             "jiro = ricecooker.cli:main",
         ]
     },
     include_package_data=True,
-    install_requires=requirements,
+    install_requires=[
+        "requests>=2.11.1",
+        "le_utils>=0.1.26",
+        "requests_file",
+        "beautifulsoup4>=4.6.3,<4.9.0",  # pinned to match versions in le-pycaption
+        "selenium==3.0.1",
+        "yt-dlp==2023.7.6",
+        "html5lib",
+        "cachecontrol==0.12.11",
+        "lockfile==0.12.2",  # This is needed, but not specified as a dependency by cachecontrol
+        "css-html-js-minify==2.2.2",
+        "pypdf2==1.26.0",
+        "dictdiffer>=0.8.0",
+        "Pillow==8.4.0",
+        "colorlog>=4.1.0,<4.2",
+        "PyYAML>=5.3.1",
+        "Jinja2>=2.10",
+        "chardet==4.0.0",
+        "ffmpy>=0.2.2",
+        "pdf2image==1.16.3",
+        "le-pycaption>=2.2.0a1",
+        "EbookLib>=0.17.1",
+        "filetype>=1.1.0",
+        "urllib3==1.26.15",
+    ],
     python_requires=">=3.7, <3.11",
     license="MIT license",
     zip_safe=False,
     keywords="ricecooker",
     classifiers=[
         "Intended Audience :: Developers",
         "Development Status :: 5 - Production/Stable",
```

### Comparing `ricecooker-0.7.2/tests/conftest.py` & `ricecooker-0.7.3/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
 
 
 @pytest.fixture
 def topic_data(base_data, channel_domain_namespace, channel_node_id):
     topic_data = copy.deepcopy(base_data)
     ids_dict = genrate_random_ids(channel_domain_namespace, channel_node_id)
     topic_data.update(ids_dict)
-    topic_data.update({"kind": content_kinds.TOPIC})
+    topic_data.update({"kind": content_kinds.TOPIC, "role": roles.LEARNER})
     return topic_data
 
 
 @pytest.fixture
 def topic(channel, title, topic_data):
     args_data = get_topic_node_args(topic_data)
     topic_kwargs = get_topic_node_kwargs_data(topic_data)
```

### Comparing `ricecooker-0.7.2/tests/media_utils/README.md` & `ricecooker-0.7.3/tests/media_utils/README.md`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/files/Wilhelm_Scream.mp3` & `ricecooker-0.7.3/tests/media_utils/files/Wilhelm_Scream.mp3`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/files/assets/images/4933759886_098e9acf93_m.jpg` & `ricecooker-0.7.3/tests/media_utils/files/assets/images/4933759886_098e9acf93_m.jpg`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/files/audio/file_example_MP3_700KB.mp3` & `ricecooker-0.7.3/tests/media_utils/files/audio/file_example_MP3_700KB.mp3`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/files/generate_thumbnail/sample.epub` & `ricecooker-0.7.3/tests/media_utils/files/generate_thumbnail/sample.epub`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/files/generate_thumbnail/sample.pdf` & `ricecooker-0.7.3/tests/media_utils/files/generate_thumbnail/sample.pdf`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/files/generate_thumbnail/sample.zip` & `ricecooker-0.7.3/tests/media_utils/files/generate_thumbnail/sample.zip`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/files/kepub.epub` & `ricecooker-0.7.3/tests/media_utils/files/kepub.epub`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/files/page_with_links.html` & `ricecooker-0.7.3/tests/media_utils/files/page_with_links.html`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/files/subtitles/basic.srt` & `ricecooker-0.7.3/tests/media_utils/files/subtitles/basic.srt`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/files/subtitles/basic.vtt` & `ricecooker-0.7.3/tests/media_utils/files/subtitles/basic.vtt`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/files/subtitles/empty.ttml` & `ricecooker-0.7.3/tests/media_utils/files/subtitles/empty.ttml`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/files/subtitles/encapsulated.sami` & `ricecooker-0.7.3/tests/media_utils/files/subtitles/encapsulated.sami`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/files/thumbnails/BRAlogo1.png` & `ricecooker-0.7.3/tests/media_utils/files/thumbnails/BRAlogo1.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/files/thumbnails/toosquare.png` & `ricecooker-0.7.3/tests/media_utils/files/thumbnails/toosquare.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/files/thumbnails/tootall.png` & `ricecooker-0.7.3/tests/media_utils/files/thumbnails/tootall.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/files/thumbnails/toowide.png` & `ricecooker-0.7.3/tests/media_utils/files/thumbnails/toowide.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/test_audio.py` & `ricecooker-0.7.3/tests/media_utils/test_audio.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/test_proxy.py` & `ricecooker-0.7.3/tests/media_utils/test_proxy.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/test_subtitles.py` & `ricecooker-0.7.3/tests/media_utils/test_subtitles.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/test_thumbnails.py` & `ricecooker-0.7.3/tests/media_utils/test_thumbnails.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/test_videos.py` & `ricecooker-0.7.3/tests/media_utils/test_videos.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/test_web.py` & `ricecooker-0.7.3/tests/media_utils/test_web.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/media_utils/test_youtube.py` & `ricecooker-0.7.3/tests/media_utils/test_youtube.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/test_argparse.py` & `ricecooker-0.7.3/tests/test_argparse.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/test_chef_integration.py` & `ricecooker-0.7.3/tests/test_chef_integration.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/test_csv_metadata.py` & `ricecooker-0.7.3/tests/test_csv_metadata.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/test_data.py` & `ricecooker-0.7.3/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/test_downloader.py` & `ricecooker-0.7.3/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/test_exercises.py` & `ricecooker-0.7.3/tests/test_exercises.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/test_files.py` & `ricecooker-0.7.3/tests/test_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -542,16 +542,16 @@
     All subs have the appropriate extension so no need to specify `subtitlesformat`.
     """
     for fixture in pressurcooker_test_files:
         localpath = fixture["localpath"]
         assert os.path.exists(localpath), "Error mising local test file " + localpath
         subtitle_file = SubtitleFile(localpath, language=fixture["language"])
         filename = subtitle_file.process_file()
-        assert filename, "conferted filename must exit"
-        assert filename.endswith(".vtt"), "conferted filename must have .vtt extension"
+        assert filename, "converted filename must exist"
+        assert filename.endswith(".vtt"), "converted filename must have .vtt extension"
         storage_path = config.get_storage_path(filename)
         with open(storage_path, encoding="utf-8") as converted_vtt:
             filecontents = converted_vtt.read()
             assert (
                 fixture["check_words"] in filecontents
             ), "missing check_words in converted subs"
 
@@ -571,16 +571,16 @@
             "testsubtitles_ar.ttml",
         )
     )
 
     assert os.path.exists(local_path)
     subtitle_file = SubtitleFile(local_path, language="ar")
     filename = subtitle_file.process_file()
-    assert filename, "conferted filename must exit"
-    assert filename.endswith(".vtt"), "conferted filename must have .vtt extension"
+    assert filename, "converted filename must exist"
+    assert filename.endswith(".vtt"), "converted filename must have .vtt extension"
 
 
 def test_convertible_substitles_noext_subtitlesformat():
     """
     Check that we handle correctly cases when path doesn't contain extenstion.
     """
     # local_path = os.path.join(
@@ -600,16 +600,16 @@
     assert os.path.exists(local_path_no_ext)
     subtitle_file = SubtitleFile(
         local_path_no_ext,
         language="ar",
         subtitlesformat="ttml",  # settting subtitlesformat becaue no ext
     )
     filename = subtitle_file.process_file()
-    assert filename, "conferted filename must exit"
-    assert filename.endswith(".vtt"), "conferted filename must have .vtt extension"
+    assert filename, "converted filename must exist"
+    assert filename.endswith(".vtt"), "converted filename must have .vtt extension"
 
 
 def test_convertible_substitles_weirdext_subtitlesformat():
     """
     Check that we handle cases when ext cannot be guessed from URL or localpath.
     Passing `subtitlesformat` allows chef authors to manually specify subs format.
     """
@@ -619,15 +619,15 @@
     )
     subtitle_file = SubtitleFile(
         subs_url,
         language="es",
         subtitlesformat="srt",  # set subtitlesformat when can't inferr ext form url
     )
     filename = subtitle_file.process_file()
-    assert filename, "conferted filename must exit"
-    assert filename.endswith(".vtt"), "conferted filename must have .vtt extension"
+    assert filename, "converted filename must exist"
+    assert filename.endswith(".vtt"), "converted filename must have .vtt extension"
     storage_path = config.get_storage_path(filename)
     with open(storage_path, encoding="utf-8") as converted_vtt:
         filecontents = converted_vtt.read()
         assert (
             "El total de los protones y neutrones de un átomo" in filecontents
         ), "missing check words in converted subs"
```

### Comparing `ricecooker-0.7.2/tests/test_licenses.py` & `ricecooker-0.7.3/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/test_links.py` & `ricecooker-0.7.3/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/test_pdfutils.py` & `ricecooker-0.7.3/tests/test_pdfutils.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/test_requests.py` & `ricecooker-0.7.3/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/test_settings.py` & `ricecooker-0.7.3/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/test_thumbnails.py` & `ricecooker-0.7.3/tests/test_thumbnails.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/test_tree.py` & `ricecooker-0.7.3/tests/test_tree.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 import uuid
 
 import pytest
 from le_utils.constants import content_kinds
 from le_utils.constants import file_types
 from le_utils.constants import format_presets
 from le_utils.constants import licenses
+from le_utils.constants.labels import levels
 from le_utils.constants.languages import getlang
 
 from ricecooker.classes.files import DocumentFile
 from ricecooker.classes.files import HTMLZipFile
 from ricecooker.classes.files import SlideImageFile
 from ricecooker.classes.files import ThumbnailFile
 from ricecooker.classes.licenses import get_license
 from ricecooker.classes.licenses import License
 from ricecooker.classes.nodes import CustomNavigationChannelNode
 from ricecooker.classes.nodes import CustomNavigationNode
 from ricecooker.classes.nodes import DocumentNode
+from ricecooker.classes.nodes import RemoteContentNode
 from ricecooker.classes.nodes import SlideshowNode
 from ricecooker.classes.nodes import TopicNode
 from ricecooker.exceptions import InvalidNodeException
 from ricecooker.utils.jsontrees import build_tree_from_json
 from ricecooker.utils.zip import create_predictable_zip
 
 """ *********** TOPIC FIXTURES *********** """
@@ -578,7 +580,111 @@
     assert custom_navigation_channel_node.to_dict()
     assert custom_navigation_channel_node.to_dict()["thumbnail"] == thumbimg1.filename
     assert len(custom_navigation_channel_node.to_dict()["files"]) == 1
     assert (
         custom_navigation_channel_node.to_dict()["files"][0]["filename"]
         == zipfile.filename
     )
+
+
+def test_remote_content_node_with_no_overrides():
+    remote_content_node = RemoteContentNode(
+        "a" * 32,
+        source_node_id="b" * 32,
+        source_content_id="c" * 32,
+    )
+    assert remote_content_node
+    assert remote_content_node.kind == "remotecontent"
+    assert len(remote_content_node.files) == 0
+    assert remote_content_node.validate_tree()
+    output = remote_content_node.to_dict()
+    assert output.get("title") is None
+    assert output.get("description") is None
+
+
+def test_remote_content_node_with_basic_overrides():
+    remote_content_node = RemoteContentNode(
+        "a" * 32,
+        source_content_id="c" * 32,
+        title="My Title",
+        description="My Description",
+    )
+    assert remote_content_node
+    assert remote_content_node.kind == "remotecontent"
+    assert len(remote_content_node.files) == 0
+    assert remote_content_node.validate_tree()
+    output = remote_content_node.to_dict()
+    assert output.get("title") == "My Title"
+    assert output.get("description") == "My Description"
+
+
+def test_remote_content_node_with_provider_override():
+    remote_content_node = RemoteContentNode(
+        "a" * 32,
+        source_node_id="b" * 32,
+        provider="Doctor Tibbles",
+    )
+    assert remote_content_node
+    assert remote_content_node.kind == "remotecontent"
+    assert len(remote_content_node.files) == 0
+    assert remote_content_node.validate_tree()
+    output = remote_content_node.to_dict()
+    assert output.get("provider") == "Doctor Tibbles"
+
+
+def test_remote_content_node_with_bad_channel_id():
+    with pytest.raises(InvalidNodeException):
+        node = RemoteContentNode(
+            "a" * 4,
+            source_node_id="b" * 32,
+        )
+        node.validate_tree()
+
+
+def test_remote_content_node_with_bad_source_content_node_ids():
+    with pytest.raises(InvalidNodeException):
+        node = RemoteContentNode(
+            "a" * 32,
+            source_node_id="b" * 4,
+            source_content_id="c" * 4,
+        )
+        node.validate_tree()
+
+
+def test_remote_content_node_with_overridden_thumbnail():
+    thumbimg1 = ThumbnailFile(
+        path="tests/testcontent/samples/thumbnail.jpg", language="en"
+    )
+    remote_content_node = RemoteContentNode(
+        "a" * 32,
+        source_content_id="c" * 32,
+        thumbnail=thumbimg1,
+    )
+    assert len(remote_content_node.files) == 1
+    assert remote_content_node.validate_tree()
+    remote_content_node.process_files()
+    output = remote_content_node.to_dict()
+    assert output.get("files")[0]["filename"] == "d7ab03e4263fc374737d96ac2da156c1.jpg"
+
+
+def test_remote_content_node_with_overridden_grade_levels():
+    grades = [levels.LEVELSLIST[0], levels.LEVELSLIST[1], levels.LEVELSLIST[2]]
+    remote_content_node = RemoteContentNode(
+        "a" * 32,
+        source_content_id="c" * 32,
+        grade_levels=grades,
+    )
+    assert remote_content_node
+    assert remote_content_node.kind == "remotecontent"
+    assert remote_content_node.validate_tree()
+    output = remote_content_node.to_dict()
+    assert output.get("grade_levels") == grades
+
+
+def test_remote_content_node_with_invalid_overridden_field():
+    with pytest.raises(InvalidNodeException):
+        node = RemoteContentNode(
+            "a" * 32,
+            source_content_id="c" * 32,
+            author="Such disallowed. Computer says no.",
+        )
+        node.validate_tree()
```

### Comparing `ricecooker-0.7.2/tests/test_videos.py` & `ricecooker-0.7.3/tests/test_videos.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/test_youtube.py` & `ricecooker-0.7.3/tests/test_youtube.py`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/ExerciseQuestions.csv` & `ricecooker-0.7.3/tests/testchannels/csv_channel_with_exercises/ExerciseQuestions.csv`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/Exercises.csv` & `ricecooker-0.7.3/tests/testchannels/csv_channel_with_exercises/Exercises.csv`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/algebra_exercise_thumb.png` & `ricecooker-0.7.3/tests/testchannels/csv_channel_with_exercises/channeldir/algebra_exercise_thumb.png`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/channel_thumbnail.jpg` & `ricecooker-0.7.3/tests/testchannels/csv_channel_with_exercises/channeldir/channel_thumbnail.jpg`

 * *Files identical despite different names*

### Comparing `ricecooker-0.7.2/tests/testchannels/csv_channel_with_exercises/channeldir/contentnodes/audio/WZ_exercise_thumbnail.png` & `ricecooker-0.7.3/tests/testchannels/csv_channel_with_exercises/channeldir/contentnodes/audio/WZ_exercise_thumbnail.png`

 * *Files identical despite different names*

