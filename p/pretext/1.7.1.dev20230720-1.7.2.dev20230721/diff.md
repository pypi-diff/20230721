# Comparing `tmp/pretext-1.7.1.dev20230720.tar.gz` & `tmp/pretext-1.7.2.dev20230721.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.7.1.dev20230720.tar", max compression
+gzip compressed data, was "pretext-1.7.2.dev20230721.tar", max compression
```

## Comparing `pretext-1.7.1.dev20230720.tar` & `pretext-1.7.2.dev20230721.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35148 2023-07-20 06:13:00.089528 pretext-1.7.1.dev20230720/LICENSE
--rw-r--r--   0        0        0     9757 2023-07-20 06:13:00.089528 pretext-1.7.1.dev20230720/README.md
--rw-r--r--   0        0        0     1962 2023-07-20 06:13:32.521266 pretext-1.7.1.dev20230720/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-07-20 06:13:00.093528 pretext-1.7.1.dev20230720/pretext/__main__.py
--rw-r--r--   0        0        0     8531 2023-07-20 06:13:00.093528 pretext-1.7.1.dev20230720/pretext/build.py
--rw-r--r--   0        0        0    25724 2023-07-20 06:13:00.093528 pretext-1.7.1.dev20230720/pretext/cli.py
--rw-r--r--   0        0        0     5856 2023-07-20 06:13:00.093528 pretext-1.7.1.dev20230720/pretext/codechat.py
--rw-r--r--   0        0        0     5943 2023-07-20 06:13:00.093528 pretext-1.7.1.dev20230720/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-07-20 06:13:00.093528 pretext-1.7.1.dev20230720/pretext/core/__init__.py
--rw-r--r--   0        0        0   172498 2023-07-20 06:13:37.389224 pretext-1.7.1.dev20230720/pretext/core/pretext.py
--rw-r--r--   0        0        0     1484 2023-07-20 06:13:00.093528 pretext-1.7.1.dev20230720/pretext/core/resources.py
--rw-r--r--   0        0        0  1045100 2023-07-20 06:13:37.389224 pretext-1.7.1.dev20230720/pretext/core/resources.zip
--rw-r--r--   0        0        0    16741 2023-07-20 06:13:00.093528 pretext-1.7.1.dev20230720/pretext/generate.py
--rw-r--r--   0        0        0    29108 2023-07-20 06:13:00.093528 pretext-1.7.1.dev20230720/pretext/project.py
--rw-r--r--   0        0        0      739 2023-07-20 06:13:00.093528 pretext-1.7.1.dev20230720/pretext/templates/__init__.py
--rw-r--r--   0        0        0     2480 2023-07-20 06:13:37.457223 pretext-1.7.1.dev20230720/pretext/templates/resources/.devcontainer.json
--rw-r--r--   0        0        0     1676 2023-07-20 06:13:37.457223 pretext-1.7.1.dev20230720/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-07-20 06:13:37.457223 pretext-1.7.1.dev20230720/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   158841 2023-07-20 06:13:37.457223 pretext-1.7.1.dev20230720/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     6347 2023-07-20 06:13:37.445223 pretext-1.7.1.dev20230720/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   172040 2023-07-20 06:13:37.441223 pretext-1.7.1.dev20230720/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     3388 2023-07-20 06:13:37.457223 pretext-1.7.1.dev20230720/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-07-20 06:13:37.457223 pretext-1.7.1.dev20230720/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-07-20 06:13:37.457223 pretext-1.7.1.dev20230720/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     7123 2023-07-20 06:13:37.445223 pretext-1.7.1.dev20230720/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    25086 2023-07-20 06:13:00.093528 pretext-1.7.1.dev20230720/pretext/utils.py
--rw-r--r--   0        0        0     3333 2023-07-20 06:13:32.521266 pretext-1.7.1.dev20230720/pyproject.toml
--rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.7.1.dev20230720/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-07-21 06:13:04.985951 pretext-1.7.2.dev20230721/LICENSE
+-rw-r--r--   0        0        0     9757 2023-07-21 06:13:04.985951 pretext-1.7.2.dev20230721/README.md
+-rw-r--r--   0        0        0     1962 2023-07-21 06:13:33.674528 pretext-1.7.2.dev20230721/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-07-21 06:13:04.985951 pretext-1.7.2.dev20230721/pretext/__main__.py
+-rw-r--r--   0        0        0     8531 2023-07-21 06:13:04.985951 pretext-1.7.2.dev20230721/pretext/build.py
+-rw-r--r--   0        0        0    26126 2023-07-21 06:13:04.985951 pretext-1.7.2.dev20230721/pretext/cli.py
+-rw-r--r--   0        0        0     5856 2023-07-21 06:13:04.985951 pretext-1.7.2.dev20230721/pretext/codechat.py
+-rw-r--r--   0        0        0     5943 2023-07-21 06:13:04.985951 pretext-1.7.2.dev20230721/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-07-21 06:13:04.985951 pretext-1.7.2.dev20230721/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172498 2023-07-21 06:13:38.622630 pretext-1.7.2.dev20230721/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1484 2023-07-21 06:13:04.985951 pretext-1.7.2.dev20230721/pretext/core/resources.py
+-rw-r--r--   0        0        0  1045100 2023-07-21 06:13:38.622630 pretext-1.7.2.dev20230721/pretext/core/resources.zip
+-rw-r--r--   0        0        0    16741 2023-07-21 06:13:04.985951 pretext-1.7.2.dev20230721/pretext/generate.py
+-rw-r--r--   0        0        0    29605 2023-07-21 06:13:04.985951 pretext-1.7.2.dev20230721/pretext/project.py
+-rw-r--r--   0        0        0      739 2023-07-21 06:13:04.985951 pretext-1.7.2.dev20230721/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     2480 2023-07-21 06:13:38.690632 pretext-1.7.2.dev20230721/pretext/templates/resources/.devcontainer.json
+-rw-r--r--   0        0        0     1676 2023-07-21 06:13:38.690632 pretext-1.7.2.dev20230721/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-07-21 06:13:38.690632 pretext-1.7.2.dev20230721/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   158841 2023-07-21 06:13:38.686632 pretext-1.7.2.dev20230721/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     6347 2023-07-21 06:13:38.678632 pretext-1.7.2.dev20230721/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   172040 2023-07-21 06:13:38.674632 pretext-1.7.2.dev20230721/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     3388 2023-07-21 06:13:38.690632 pretext-1.7.2.dev20230721/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-07-21 06:13:38.690632 pretext-1.7.2.dev20230721/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-07-21 06:13:38.690632 pretext-1.7.2.dev20230721/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     7123 2023-07-21 06:13:38.678632 pretext-1.7.2.dev20230721/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    25086 2023-07-21 06:13:04.989951 pretext-1.7.2.dev20230721/pretext/utils.py
+-rw-r--r--   0        0        0     3333 2023-07-21 06:13:33.678528 pretext-1.7.2.dev20230721/pyproject.toml
+-rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.7.2.dev20230721/PKG-INFO
```

### Comparing `pretext-1.7.1.dev20230720/LICENSE` & `pretext-1.7.2.dev20230721/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.7.1.dev20230720/README.md` & `pretext-1.7.2.dev20230721/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.7.1.dev20230720/pretext/__init__.py` & `pretext-1.7.2.dev20230721/pretext/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.1.dev20230720/pretext/build.py` & `pretext-1.7.2.dev20230721/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.1.dev20230720/pretext/cli.py` & `pretext-1.7.2.dev20230721/pretext/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -384,30 +384,37 @@
             f"Since no build target was supplied, the first target of the project.ptx manifest ({target.name()}) will be built.\n"
         )
         target_name = target.name()
     if target is None:
         utils.show_target_hints(target_name, project, task="build")
         log.critical("Exiting without completing build.")
         return
+    # First, make sure a webwork-representations file exists if needed:
+    if target.needs_ww_reps() and not target.has_ww_reps():
+        log.info(
+            "This target needs a webwork-representations.xml file, but it wasn't found (possibly manually deleted?).  Generating it now."
+        )
+        project.generate_webwork(target.name(), xmlid=xmlid)
     # Automatically generate any assets that have changed.
     if not no_generate:
         asset_table = target.load_asset_table()
         asset_hash_dict = target.asset_hash()
         if asset_table == asset_hash_dict:
             log.info(
                 "No change in assets requiring generating detected.  To force regeneration of assets, use `-g` flag.\n"
             )
         else:
-            for asset in set(asset[0] for asset in asset_hash_dict.keys()):
-                if asset in ["webwork"]:
-                    if (asset, "") not in asset_table or asset_hash_dict[
-                        (asset, "")
-                    ] != asset_table[(asset, "")]:
-                        project.generate(target.name(), asset_list=[asset])
-                elif (asset, "") not in asset_table or asset_hash_dict[
+            if ("webwork", "") not in asset_table or asset_hash_dict[
+                ("webwork", "")
+            ] != asset_table[("webwork", "")]:
+                project.generate_webwork(target.name(), xmlid=xmlid)
+            assets = set(asset[0] for asset in asset_hash_dict.keys())
+            assets.discard("webwork")
+            for asset in assets:
+                if (asset, "") not in asset_table or asset_hash_dict[
                     (asset, "")
                 ] != asset_table[(asset, "")]:
                     project.generate(target.name(), asset_list=[asset])
                 else:
                     for id in set(
                         key[1] for key in asset_hash_dict.keys() if key[0] == asset
                     ):
@@ -424,26 +431,25 @@
     else:
         log.info("Skipping asset generation as requested.")
     if generate == "ALL":
         log.info("Generating all assets in default formats as requested.")
         log.info(
             "Note: PreTeXt will automatically generate assets that have been changed since your last build, so this option is no longer necessary unless something isn't happening as expected."
         )
-        project.generate(target.name())
+        project.generate_webwork(target.name(), xmlid=xmlid)
+        project.generate(target.name(), xmlid=xmlid)
     elif generate is not None:
         log.info(f"Generating {generate} assets as requested.")
         log.info(
             "Note: PreTeXt will automatically generate assets that have been changed since your last build, so this option is no longer necessary unless something isn't happening as expected."
         )
-        project.generate(target.name(), asset_list=[generate])
-    if target.needs_ww_reps() and not target.has_ww_reps():
-        log.info(
-            "This target needs a webwork-representations.xml file, but it wasn't found (possibly manually deleted?).  Generating it now."
-        )
-        project.generate(target.name(), asset_list=["webwork"])
+        if "webwork" in generate:
+            project.generate_webwork(target.name(), xmlid=xmlid)
+        project.generate(target.name(), asset_list=[generate], xmlid=xmlid)
+    # Now finally build the target
     project.build(target.name(), clean)
 
 
 # pretext generate
 @main.command(
     short_help="Generate specified assets for specified target",
     context_settings=CONTEXT_SETTINGS,
@@ -508,14 +514,16 @@
         utils.show_target_hints(target_name, project, task="generating assets for")
         log.critical("Exiting without generating any assets.")
         return
     if target_name is None:
         log.info(
             f"Since no target was specified with the -t flag, we will generate assets for the first target in the manifest ({target.name()})."
         )
+    if "webwork" in assets or assets == "ALL":
+        project.generate_webwork(target.name(), xmlid=xmlid)
     if all_formats and assets == "ALL":
         log.info(
             f'Generating all assets in all asset formats for the target "{target.name()}".'
         )
         project.generate(target.name(), all_formats=True, xmlid=xmlid)
     elif all_formats:
         log.info(
```

### Comparing `pretext-1.7.1.dev20230720/pretext/codechat.py` & `pretext-1.7.2.dev20230721/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.1.dev20230720/pretext/config/xml_overlay.py` & `pretext-1.7.2.dev20230721/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.1.dev20230720/pretext/core/pretext.py` & `pretext-1.7.2.dev20230721/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.1.dev20230720/pretext/core/resources.py` & `pretext-1.7.2.dev20230721/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.1.dev20230720/pretext/core/resources.zip` & `pretext-1.7.2.dev20230721/pretext/core/resources.zip`

 * *Files 5% similar despite different names*

#### zipinfo {}

```diff
@@ -1,144 +1,144 @@
 Zip file size: 1045100 bytes, number of entries: 142
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 xsl/
--rw-r--r--  2.0 unx    30908 b- defN 23-Jul-20 06:13 pretext/pretext
--rw-r--r--  2.0 unx     1955 b- defN 23-Jul-20 06:13 pretext/module-test.py
--rw-r--r--  2.0 unx     2566 b- defN 23-Jul-20 06:13 pretext/pretext.cfg
--rw-r--r--  2.0 unx   172498 b- defN 23-Jul-20 06:13 pretext/pretext.py
--rw-r--r--  2.0 unx     1367 b- defN 23-Jul-20 06:13 pretext/README.md
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-20 06:13 pretext/__init__.py
--rw-r--r--  2.0 unx    36045 b- defN 23-Jul-20 06:13 pretext/braille_format.py
--rw-r--r--  2.0 unx   125135 b- defN 23-Jul-20 06:13 schema/pretext.xsd
--rw-r--r--  2.0 unx      326 b- defN 23-Jul-20 06:13 schema/xml.xsd
--rw-r--r--  2.0 unx    58086 b- defN 23-Jul-20 06:13 schema/pretext.rnc
--rw-r--r--  2.0 unx    17587 b- defN 23-Jul-20 06:13 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx    25870 b- defN 23-Jul-20 06:13 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx    18421 b- defN 23-Jul-20 06:13 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx     1180 b- defN 23-Jul-20 06:13 schema/README.md
--rw-r--r--  2.0 unx   134043 b- defN 23-Jul-20 06:13 schema/pretext.xml
--rw-r--r--  2.0 unx     3135 b- defN 23-Jul-20 06:13 schema/build.sh
--rw-r--r--  2.0 unx    34210 b- defN 23-Jul-20 06:13 schema/pretext-dev.rng
--rw-r--r--  2.0 unx   101829 b- defN 23-Jul-20 06:13 schema/pretext.rng
--rw-r--r--  2.0 unx     1276 b- defN 23-Jul-20 06:13 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx     2608 b- defN 23-Jul-20 06:13 css/colors_default.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-20 06:13 css/colors_blue_red.css
--rw-r--r--  2.0 unx    12567 b- defN 23-Jul-20 06:13 css/style_oscarlevin.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-20 06:13 css/colors_green_plum.css
--rw-r--r--  2.0 unx     3473 b- defN 23-Jul-20 06:13 css/style_soundwriting.css
--rw-r--r--  2.0 unx     1338 b- defN 23-Jul-20 06:13 css/colors_red_blue.css
--rw-r--r--  2.0 unx     7761 b- defN 23-Jul-20 06:13 css/style_default.css
--rw-r--r--  2.0 unx     2438 b- defN 23-Jul-20 06:13 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jul-20 06:13 css/colors_martiansands.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jul-20 06:13 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-20 06:13 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     1280 b- defN 23-Jul-20 06:13 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-20 06:13 css/colors_orange_navy.css
--rw-r--r--  2.0 unx    14069 b- defN 23-Jul-20 06:13 css/setcolors.css
--rw-r--r--  2.0 unx     4021 b- defN 23-Jul-20 06:13 css/update_css
--rw-r--r--  2.0 unx     1865 b- defN 23-Jul-20 06:13 css/README.md
--rw-r--r--  2.0 unx     4308 b- defN 23-Jul-20 06:13 css/colors_blue_green.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-20 06:13 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx    22438 b- defN 23-Jul-20 06:13 css/pretext.css
--rw-r--r--  2.0 unx   146685 b- defN 23-Jul-20 06:13 css/mathbook-content.css
--rw-r--r--  2.0 unx   435680 b- defN 23-Jul-20 06:13 css/mathbook-3.css
--rw-r--r--  2.0 unx     1362 b- defN 23-Jul-20 06:13 css/epub.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-20 06:13 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx      691 b- defN 23-Jul-20 06:13 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-20 06:13 css/colors_green_blue.css
--rw-r--r--  2.0 unx    71198 b- defN 23-Jul-20 06:13 css/pretext_add_on.css
--rw-r--r--  2.0 unx    63664 b- defN 23-Jul-20 06:13 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     2441 b- defN 23-Jul-20 06:13 css/kindle.css
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 xsl/utilities/
--rw-r--r--  2.0 unx     2248 b- defN 23-Jul-20 06:13 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-Jul-20 06:13 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-Jul-20 06:13 xsl/entities.ent
--rw-r--r--  2.0 unx    17293 b- defN 23-Jul-20 06:13 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-Jul-20 06:13 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-Jul-20 06:13 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-Jul-20 06:13 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-Jul-20 06:13 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx   231265 b- defN 23-Jul-20 06:13 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx   611284 b- defN 23-Jul-20 06:13 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-Jul-20 06:13 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-Jul-20 06:13 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-Jul-20 06:13 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-Jul-20 06:13 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-Jul-20 06:13 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx    94587 b- defN 23-Jul-20 06:13 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-Jul-20 06:13 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-Jul-20 06:13 xsl/README.md
--rw-r--r--  2.0 unx    10708 b- defN 23-Jul-20 06:13 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-Jul-20 06:13 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-Jul-20 06:13 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-Jul-20 06:13 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-Jul-20 06:13 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-Jul-20 06:13 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx   544154 b- defN 23-Jul-20 06:13 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx   139486 b- defN 23-Jul-20 06:13 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx   548615 b- defN 23-Jul-20 06:13 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-Jul-20 06:13 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-Jul-20 06:13 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx   116581 b- defN 23-Jul-20 06:13 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-Jul-20 06:13 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-Jul-20 06:13 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-Jul-20 06:13 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-Jul-20 06:13 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-Jul-20 06:13 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-Jul-20 06:13 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-Jul-20 06:13 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx   110949 b- defN 23-Jul-20 06:13 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx    12084 b- defN 23-Jul-20 06:13 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx    14482 b- defN 23-Jul-20 06:13 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-Jul-20 06:13 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-Jul-20 06:13 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-Jul-20 06:13 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-Jul-20 06:13 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx      787 b- defN 23-Jul-20 06:13 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx    30257 b- defN 23-Jul-20 06:13 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-Jul-20 06:13 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx      513 b- defN 23-Jul-20 06:13 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4299 b- defN 23-Jul-20 06:13 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx     1810 b- defN 23-Jul-20 06:13 xsl/utilities/README.md
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 xsl/support/play-button/
--rw-r--r--  2.0 unx      486 b- defN 23-Jul-20 06:13 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5879 b- defN 23-Jul-20 06:13 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx      504 b- defN 23-Jul-20 06:13 xsl/support/README.md
--rw-r--r--  2.0 unx     5065 b- defN 23-Jul-20 06:13 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx    10306 b- defN 23-Jul-20 06:13 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-Jul-20 06:13 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx     5800 b- defN 23-Jul-20 06:13 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx     6621 b- defN 23-Jul-20 06:13 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx      722 b- defN 23-Jul-20 06:13 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     2657 b- defN 23-Jul-20 06:13 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx    16534 b- defN 23-Jul-20 06:13 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    16349 b- defN 23-Jul-20 06:13 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    15866 b- defN 23-Jul-20 06:13 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16312 b- defN 23-Jul-20 06:13 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx    15582 b- defN 23-Jul-20 06:13 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    17056 b- defN 23-Jul-20 06:13 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    16085 b- defN 23-Jul-20 06:13 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    19185 b- defN 23-Jul-20 06:13 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    17081 b- defN 23-Jul-20 06:13 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx     2286 b- defN 23-Jul-20 06:13 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx     4760 b- defN 23-Jul-20 06:13 xsl/localizations/README.md
--rw-r--r--  2.0 unx    19326 b- defN 23-Jul-20 06:13 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    17231 b- defN 23-Jul-20 06:13 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16500 b- defN 23-Jul-20 06:13 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17301 b- defN 23-Jul-20 06:13 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    20481 b- defN 23-Jul-20 06:13 xsl/localizations/ku-CKB.xml
--rw-r--r--  2.0 unx    16252 b- defN 23-Jul-20 06:13 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    16837 b- defN 23-Jul-20 06:13 xsl/localizations/af-ZA.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-Jul-20 06:13 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-Jul-20 06:13 script/mbx
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 06:13 script/mjsre/update-sre
--rw-r--r--  2.0 unx      116 b- defN 23-Jul-20 06:13 script/mjsre/package.json
--rw-r--r--  2.0 unx      481 b- defN 23-Jul-20 06:13 script/mjsre/README.md
--rw-r--r--  2.0 unx     9251 b- defN 23-Jul-20 06:13 script/mjsre/mj-sre-page.js
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 xsl/
+-rw-r--r--  2.0 unx    30908 b- defN 23-Jul-21 06:13 pretext/pretext
+-rw-r--r--  2.0 unx     1955 b- defN 23-Jul-21 06:13 pretext/module-test.py
+-rw-r--r--  2.0 unx     2566 b- defN 23-Jul-21 06:13 pretext/pretext.cfg
+-rw-r--r--  2.0 unx   172498 b- defN 23-Jul-21 06:13 pretext/pretext.py
+-rw-r--r--  2.0 unx     1367 b- defN 23-Jul-21 06:13 pretext/README.md
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 06:13 pretext/__init__.py
+-rw-r--r--  2.0 unx    36045 b- defN 23-Jul-21 06:13 pretext/braille_format.py
+-rw-r--r--  2.0 unx   125135 b- defN 23-Jul-21 06:13 schema/pretext.xsd
+-rw-r--r--  2.0 unx      326 b- defN 23-Jul-21 06:13 schema/xml.xsd
+-rw-r--r--  2.0 unx    58086 b- defN 23-Jul-21 06:13 schema/pretext.rnc
+-rw-r--r--  2.0 unx    17587 b- defN 23-Jul-21 06:13 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx    25870 b- defN 23-Jul-21 06:13 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx    18421 b- defN 23-Jul-21 06:13 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx     1180 b- defN 23-Jul-21 06:13 schema/README.md
+-rw-r--r--  2.0 unx   134043 b- defN 23-Jul-21 06:13 schema/pretext.xml
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jul-21 06:13 schema/build.sh
+-rw-r--r--  2.0 unx    34210 b- defN 23-Jul-21 06:13 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx   101829 b- defN 23-Jul-21 06:13 schema/pretext.rng
+-rw-r--r--  2.0 unx     1276 b- defN 23-Jul-21 06:13 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-Jul-21 06:13 css/colors_default.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-21 06:13 css/colors_blue_red.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-Jul-21 06:13 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-21 06:13 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-Jul-21 06:13 css/style_soundwriting.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-Jul-21 06:13 css/colors_red_blue.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-Jul-21 06:13 css/style_default.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-Jul-21 06:13 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jul-21 06:13 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jul-21 06:13 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-21 06:13 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-Jul-21 06:13 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-21 06:13 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-Jul-21 06:13 css/setcolors.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-Jul-21 06:13 css/update_css
+-rw-r--r--  2.0 unx     1865 b- defN 23-Jul-21 06:13 css/README.md
+-rw-r--r--  2.0 unx     4308 b- defN 23-Jul-21 06:13 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-21 06:13 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-Jul-21 06:13 css/pretext.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-Jul-21 06:13 css/mathbook-content.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-Jul-21 06:13 css/mathbook-3.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-Jul-21 06:13 css/epub.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-21 06:13 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx      691 b- defN 23-Jul-21 06:13 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-21 06:13 css/colors_green_blue.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-Jul-21 06:13 css/pretext_add_on.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-Jul-21 06:13 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-Jul-21 06:13 css/kindle.css
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 xsl/utilities/
+-rw-r--r--  2.0 unx     2248 b- defN 23-Jul-21 06:13 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-Jul-21 06:13 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-Jul-21 06:13 xsl/entities.ent
+-rw-r--r--  2.0 unx    17293 b- defN 23-Jul-21 06:13 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-Jul-21 06:13 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-Jul-21 06:13 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-Jul-21 06:13 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx    39918 b- defN 23-Jul-21 06:13 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx   231265 b- defN 23-Jul-21 06:13 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx   611284 b- defN 23-Jul-21 06:13 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-Jul-21 06:13 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-Jul-21 06:13 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 23-Jul-21 06:13 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-Jul-21 06:13 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-Jul-21 06:13 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx    94587 b- defN 23-Jul-21 06:13 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-Jul-21 06:13 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-Jul-21 06:13 xsl/README.md
+-rw-r--r--  2.0 unx    10708 b- defN 23-Jul-21 06:13 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-Jul-21 06:13 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-Jul-21 06:13 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-Jul-21 06:13 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-Jul-21 06:13 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-Jul-21 06:13 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx   544154 b- defN 23-Jul-21 06:13 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx   139486 b- defN 23-Jul-21 06:13 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx   548615 b- defN 23-Jul-21 06:13 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-Jul-21 06:13 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-Jul-21 06:13 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx   116581 b- defN 23-Jul-21 06:13 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-Jul-21 06:13 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-Jul-21 06:13 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-Jul-21 06:13 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-Jul-21 06:13 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-Jul-21 06:13 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-Jul-21 06:13 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-Jul-21 06:13 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx   110949 b- defN 23-Jul-21 06:13 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx    12084 b- defN 23-Jul-21 06:13 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx    14482 b- defN 23-Jul-21 06:13 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-Jul-21 06:13 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-Jul-21 06:13 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-Jul-21 06:13 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-Jul-21 06:13 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx      787 b- defN 23-Jul-21 06:13 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx    30257 b- defN 23-Jul-21 06:13 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 23-Jul-21 06:13 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx      513 b- defN 23-Jul-21 06:13 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4299 b- defN 23-Jul-21 06:13 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx     1810 b- defN 23-Jul-21 06:13 xsl/utilities/README.md
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 xsl/support/play-button/
+-rw-r--r--  2.0 unx      486 b- defN 23-Jul-21 06:13 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5879 b- defN 23-Jul-21 06:13 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx      504 b- defN 23-Jul-21 06:13 xsl/support/README.md
+-rw-r--r--  2.0 unx     5065 b- defN 23-Jul-21 06:13 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx    10306 b- defN 23-Jul-21 06:13 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-Jul-21 06:13 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx     5800 b- defN 23-Jul-21 06:13 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx     6621 b- defN 23-Jul-21 06:13 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx      722 b- defN 23-Jul-21 06:13 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     2657 b- defN 23-Jul-21 06:13 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx    16534 b- defN 23-Jul-21 06:13 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    16349 b- defN 23-Jul-21 06:13 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    15866 b- defN 23-Jul-21 06:13 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16312 b- defN 23-Jul-21 06:13 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx    15582 b- defN 23-Jul-21 06:13 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    17056 b- defN 23-Jul-21 06:13 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    16085 b- defN 23-Jul-21 06:13 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    19185 b- defN 23-Jul-21 06:13 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    17081 b- defN 23-Jul-21 06:13 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx     2286 b- defN 23-Jul-21 06:13 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx     4760 b- defN 23-Jul-21 06:13 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    19326 b- defN 23-Jul-21 06:13 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    17231 b- defN 23-Jul-21 06:13 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16500 b- defN 23-Jul-21 06:13 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17301 b- defN 23-Jul-21 06:13 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    20481 b- defN 23-Jul-21 06:13 xsl/localizations/ku-CKB.xml
+-rw-r--r--  2.0 unx    16252 b- defN 23-Jul-21 06:13 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    16837 b- defN 23-Jul-21 06:13 xsl/localizations/af-ZA.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-Jul-21 06:13 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-Jul-21 06:13 script/mbx
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 06:13 script/mjsre/update-sre
+-rw-r--r--  2.0 unx      116 b- defN 23-Jul-21 06:13 script/mjsre/package.json
+-rw-r--r--  2.0 unx      481 b- defN 23-Jul-21 06:13 script/mjsre/README.md
+-rw-r--r--  2.0 unx     9251 b- defN 23-Jul-21 06:13 script/mjsre/mj-sre-page.js
 142 files, 4848159 bytes uncompressed, 1027526 bytes compressed:  78.8%
```

### Comparing `pretext-1.7.1.dev20230720/pretext/generate.py` & `pretext-1.7.2.dev20230721/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.1.dev20230720/pretext/project.py` & `pretext-1.7.2.dev20230721/pretext/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -491,14 +491,33 @@
             core.release_temporary_directories()
         # build was successful
         log.info(f"\nSuccess! Run `pretext view {target.name()}` to see the results.\n")
         if custom_xsl is not None:
             # errors may occur in Windows so we do the best we can
             shutil.rmtree(custom_xsl.parent, ignore_errors=True)
 
+    # Webwork is special since its generation is required for all builds and generates when webwork is in source, so we use a dedicated method for it.
+    def generate_webwork(self, target_name: str, xmlid: Optional[str] = None) -> None:
+        target = self.target(target_name)
+        if target is None:
+            log.error(f"Target `{target_name}` not found.")
+            return
+        xmlid = xmlid or target.xmlid_root()
+        webwork_output = target.generated_dir_found() / "webwork"
+        generate.webwork(
+            target.source(),
+            target.publication(),
+            webwork_output,
+            target.stringparams(),
+            xmlid,
+        )
+        # Delete temporary directories left behind by core:
+        core.release_temporary_directories()
+
+    # Generate all non-webwork targets
     def generate(
         self,
         target_name: str,
         asset_list: Optional[List[str]] = None,
         all_formats: bool = False,
         xmlid: Optional[str] = None,
     ) -> None:
@@ -509,23 +528,14 @@
             gen_all = False
         target = self.target(target_name)
         if target is None:
             log.error(f"Target `{target_name}` not found.")
             return
         xmlid = xmlid or target.xmlid_root()
         # build targets:
-        if gen_all or "webwork" in asset_list:
-            webwork_output = target.generated_dir_found() / "webwork"
-            generate.webwork(
-                target.source(),
-                target.publication(),
-                webwork_output,
-                target.stringparams(),
-                xmlid,
-            )
         if gen_all or "latex-image" in asset_list:
             generate.latex_image(
                 target.source(),
                 target.publication(),
                 target.generated_dir_found(),
                 target.stringparams(),
                 target.format(),
```

### Comparing `pretext-1.7.1.dev20230720/pretext/templates/__init__.py` & `pretext-1.7.2.dev20230721/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.1.dev20230720/pretext/templates/resources/.devcontainer.json` & `pretext-1.7.2.dev20230721/pretext/templates/resources/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.7.1.dev20230720/pretext/templates/resources/.gitignore` & `pretext-1.7.2.dev20230721/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.7.1.dev20230720/pretext/templates/resources/article.zip` & `pretext-1.7.2.dev20230721/pretext/templates/resources/article.zip`

 * *Files 1% similar despite different names*

#### zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 158841 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-20 06:13 .gitignore
--rw-r--r--  2.0 unx       86 b- defN 23-Jul-20 06:13 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-20 06:13 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-20 06:13 codechat_config.yaml
--rw-r--r--  2.0 unx      242 b- defN 23-Jul-20 06:13 publication/publication.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-Jul-20 06:13 source/section-2.ptx
--rw-r--r--  2.0 unx      449 b- defN 23-Jul-20 06:13 source/section-1.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-Jul-20 06:13 source/main.ptx
--rw-r--r--  2.0 unx   154806 b- defN 23-Jul-20 06:13 assets/frog.jpg
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-21 06:13 .gitignore
+-rw-r--r--  2.0 unx       86 b- defN 23-Jul-21 06:13 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jul-21 06:13 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-21 06:13 codechat_config.yaml
+-rw-r--r--  2.0 unx      242 b- defN 23-Jul-21 06:13 publication/publication.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-Jul-21 06:13 source/section-2.ptx
+-rw-r--r--  2.0 unx      449 b- defN 23-Jul-21 06:13 source/section-1.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-Jul-21 06:13 source/main.ptx
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jul-21 06:13 assets/frog.jpg
 12 files, 162649 bytes uncompressed, 157561 bytes compressed:  3.1%
```

### Comparing `pretext-1.7.1.dev20230720/pretext/templates/resources/book.zip` & `pretext-1.7.2.dev20230721/pretext/templates/resources/book.zip`

 * *Files 6% similar despite different names*

#### zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 6347 bytes, number of entries: 8
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-20 06:13 .gitignore
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-20 06:13 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-20 06:13 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-20 06:13 codechat_config.yaml
--rw-r--r--  2.0 unx     6114 b- defN 23-Jul-20 06:13 publication/publication.ptx
--rw-r--r--  2.0 unx     1767 b- defN 23-Jul-20 06:13 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-21 06:13 .gitignore
+-rw-r--r--  2.0 unx       82 b- defN 23-Jul-21 06:13 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jul-21 06:13 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-21 06:13 codechat_config.yaml
+-rw-r--r--  2.0 unx     6114 b- defN 23-Jul-21 06:13 publication/publication.ptx
+-rw-r--r--  2.0 unx     1767 b- defN 23-Jul-21 06:13 source/main.ptx
 8 files, 13617 bytes uncompressed, 5495 bytes compressed:  59.6%
```

### Comparing `pretext-1.7.1.dev20230720/pretext/templates/resources/demo.zip` & `pretext-1.7.2.dev20230721/pretext/templates/resources/demo.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,34 +1,34 @@
 Zip file size: 172040 bytes, number of entries: 32
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-20 06:13 .gitignore
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-20 06:13 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-20 06:13 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-20 06:13 codechat_config.yaml
--rw-r--r--  2.0 unx     6092 b- defN 23-Jul-20 06:13 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 source/images/
--rw-r--r--  2.0 unx     1515 b- defN 23-Jul-20 06:13 source/ex-first.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-Jul-20 06:13 source/ch-generate.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-Jul-20 06:13 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-Jul-20 06:13 source/sec-features.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-Jul-20 06:13 source/ch-empty.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-Jul-20 06:13 source/frontmatter.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-Jul-20 06:13 source/main.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-Jul-20 06:13 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-Jul-20 06:13 source/backmatter.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-Jul-20 06:13 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-Jul-20 06:13 source/ch-features.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-Jul-20 06:13 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-Jul-20 06:13 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-Jul-20 06:13 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-Jul-20 06:13 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-Jul-20 06:13 source/docinfo.ptx
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-20 06:13 source/images/sageplot2d.sage
--rw-r--r--  2.0 unx      835 b- defN 23-Jul-20 06:13 source/images/cflag.asy
--rw-r--r--  2.0 unx       93 b- defN 23-Jul-20 06:13 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx      357 b- defN 23-Jul-20 06:13 source/images/tikz.tex
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-Jul-20 06:13 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-Jul-20 06:13 assets/jsxgraph/infinity.js
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-21 06:13 .gitignore
+-rw-r--r--  2.0 unx       82 b- defN 23-Jul-21 06:13 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jul-21 06:13 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-21 06:13 codechat_config.yaml
+-rw-r--r--  2.0 unx     6092 b- defN 23-Jul-21 06:13 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 source/images/
+-rw-r--r--  2.0 unx     1515 b- defN 23-Jul-21 06:13 source/ex-first.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jul-21 06:13 source/ch-generate.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-Jul-21 06:13 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-Jul-21 06:13 source/sec-features.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-Jul-21 06:13 source/ch-empty.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-Jul-21 06:13 source/frontmatter.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jul-21 06:13 source/main.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-Jul-21 06:13 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-Jul-21 06:13 source/backmatter.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-Jul-21 06:13 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-Jul-21 06:13 source/ch-features.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-Jul-21 06:13 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-Jul-21 06:13 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-Jul-21 06:13 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-Jul-21 06:13 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-Jul-21 06:13 source/docinfo.ptx
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-21 06:13 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx      835 b- defN 23-Jul-21 06:13 source/images/cflag.asy
+-rw-r--r--  2.0 unx       93 b- defN 23-Jul-21 06:13 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx      357 b- defN 23-Jul-21 06:13 source/images/tikz.tex
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jul-21 06:13 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-Jul-21 06:13 assets/jsxgraph/infinity.js
 32 files, 187912 bytes uncompressed, 168326 bytes compressed:  10.4%
```

### Comparing `pretext-1.7.1.dev20230720/pretext/templates/resources/hello.zip` & `pretext-1.7.2.dev20230721/pretext/templates/resources/hello.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 3388 bytes, number of entries: 8
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-20 06:13 .gitignore
--rw-r--r--  2.0 unx       69 b- defN 23-Jul-20 06:13 README.md
--rw-r--r--  2.0 unx     1217 b- defN 23-Jul-20 06:13 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-20 06:13 codechat_config.yaml
--rw-r--r--  2.0 unx      242 b- defN 23-Jul-20 06:13 publication/publication.ptx
--rw-r--r--  2.0 unx      156 b- defN 23-Jul-20 06:13 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-21 06:13 .gitignore
+-rw-r--r--  2.0 unx       69 b- defN 23-Jul-21 06:13 README.md
+-rw-r--r--  2.0 unx     1217 b- defN 23-Jul-21 06:13 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-21 06:13 codechat_config.yaml
+-rw-r--r--  2.0 unx      242 b- defN 23-Jul-21 06:13 publication/publication.ptx
+-rw-r--r--  2.0 unx      156 b- defN 23-Jul-21 06:13 source/main.ptx
 8 files, 5628 bytes uncompressed, 2536 bytes compressed:  54.9%
```

### Comparing `pretext-1.7.1.dev20230720/pretext/templates/resources/project.ptx` & `pretext-1.7.2.dev20230721/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.7.1.dev20230720/pretext/templates/resources/slideshow.zip` & `pretext-1.7.2.dev20230721/pretext/templates/resources/slideshow.zip`

 * *Files 7% similar despite different names*

#### zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 7123 bytes, number of entries: 9
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 06:13 xsl/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-20 06:13 .gitignore
--rw-r--r--  2.0 unx      784 b- defN 23-Jul-20 06:13 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-20 06:13 codechat_config.yaml
--rw-r--r--  2.0 unx     2097 b- defN 23-Jul-20 06:13 publication/publication.ptx
--rw-r--r--  2.0 unx    11200 b- defN 23-Jul-20 06:13 source/main.ptx
--rw-r--r--  2.0 unx      190 b- defN 23-Jul-20 06:13 xsl/slides.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 06:13 xsl/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-21 06:13 .gitignore
+-rw-r--r--  2.0 unx      784 b- defN 23-Jul-21 06:13 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-21 06:13 codechat_config.yaml
+-rw-r--r--  2.0 unx     2097 b- defN 23-Jul-21 06:13 publication/publication.ptx
+-rw-r--r--  2.0 unx    11200 b- defN 23-Jul-21 06:13 source/main.ptx
+-rw-r--r--  2.0 unx      190 b- defN 23-Jul-21 06:13 xsl/slides.xsl
 9 files, 18215 bytes uncompressed, 6177 bytes compressed:  66.1%
```

### Comparing `pretext-1.7.1.dev20230720/pretext/utils.py` & `pretext-1.7.2.dev20230721/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.1.dev20230720/pyproject.toml` & `pretext-1.7.2.dev20230721/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # See https://python-poetry.org/docs/dependency-specification/ to get an understanding of
 # how poetry specifies dependencies.
 #
 # Project metadata
 # ----------------
 [tool.poetry]
 name = "pretext"
-version = "1.7.1.dev20230720"
+version = "1.7.2.dev20230721"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.7.1.dev20230720/PKG-INFO` & `pretext-1.7.2.dev20230721/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.7.1.dev20230720
+Version: 1.7.2.dev20230721
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

