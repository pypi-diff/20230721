# Comparing `tmp/pretext-1.7.2.tar.gz` & `tmp/pretext-1.7.2.dev20230721.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.7.2.tar", max compression
+gzip compressed data, was "pretext-1.7.2.dev20230721.tar", max compression
```

## Comparing `pretext-1.7.2.tar` & `pretext-1.7.2.dev20230721.tar`

### file list

```diff
@@ -1,32 +1,28 @@
--rw-r--r--   0        0        0    35148 2023-07-21 15:14:18.663323 pretext-1.7.2/LICENSE
--rw-r--r--   0        0        0     9757 2023-07-21 15:14:18.663323 pretext-1.7.2/README.md
--rw-r--r--   0        0        0     1500 2023-07-21 15:14:18.667322 pretext-1.7.2/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-07-21 15:14:18.667322 pretext-1.7.2/pretext/__main__.py
--rw-r--r--   0        0        0    11608 2023-07-21 15:14:18.667322 pretext-1.7.2/pretext/build.py
--rw-r--r--   0        0        0    26150 2023-07-21 15:14:18.667322 pretext-1.7.2/pretext/cli.py
--rw-r--r--   0        0        0     6086 2023-07-21 15:14:18.667322 pretext-1.7.2/pretext/codechat.py
--rw-r--r--   0        0        0     5943 2023-07-21 15:14:18.667322 pretext-1.7.2/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      675 2023-07-21 15:14:18.667322 pretext-1.7.2/pretext/constants.py
--rw-r--r--   0        0        0      350 2023-07-21 15:14:18.667322 pretext-1.7.2/pretext/core/__init__.py
--rw-r--r--   0        0        0   172498 2023-07-21 15:14:54.991710 pretext-1.7.2/pretext/core/pretext.py
--rw-r--r--   0        0        0     1484 2023-07-21 15:14:18.667322 pretext-1.7.2/pretext/core/resources.py
--rw-r--r--   0        0        0  1045100 2023-07-21 15:14:54.991710 pretext-1.7.2/pretext/core/resources.zip
--rw-r--r--   0        0        0    16741 2023-07-21 15:14:18.667322 pretext-1.7.2/pretext/generate.py
--rw-r--r--   0        0        0    29656 2023-07-21 15:14:18.667322 pretext-1.7.2/pretext/project/__init__.py
--rw-r--r--   0        0        0    28919 2023-07-21 15:14:18.667322 pretext-1.7.2/pretext/project/refactor.py
--rw-r--r--   0        0        0     2360 2023-07-21 15:14:18.667322 pretext-1.7.2/pretext/project/xml.py
--rw-r--r--   0        0        0      739 2023-07-21 15:14:18.667322 pretext-1.7.2/pretext/templates/__init__.py
--rw-r--r--   0        0        0     2480 2023-07-21 15:14:55.063711 pretext-1.7.2/pretext/templates/resources/.devcontainer.json
--rw-r--r--   0        0        0     1676 2023-07-21 15:14:55.063711 pretext-1.7.2/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-07-21 15:14:55.063711 pretext-1.7.2/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   158841 2023-07-21 15:14:55.059711 pretext-1.7.2/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     6347 2023-07-21 15:14:55.047711 pretext-1.7.2/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   172170 2023-07-21 15:14:55.043711 pretext-1.7.2/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     3388 2023-07-21 15:14:55.063711 pretext-1.7.2/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-07-21 15:14:55.063711 pretext-1.7.2/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-07-21 15:14:55.063711 pretext-1.7.2/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     7123 2023-07-21 15:14:55.051710 pretext-1.7.2/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0      109 2023-07-21 15:14:18.667322 pretext-1.7.2/pretext/types.py
--rw-r--r--   0        0        0    25401 2023-07-21 15:14:18.667322 pretext-1.7.2/pretext/utils.py
--rw-r--r--   0        0        0     3341 2023-07-21 15:14:18.667322 pretext-1.7.2/pyproject.toml
--rw-r--r--   0        0        0    10879 1970-01-01 00:00:00.000000 pretext-1.7.2/PKG-INFO
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

### Comparing `pretext-1.7.2/LICENSE` & `pretext-1.7.2.dev20230721/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.7.2/README.md` & `pretext-1.7.2.dev20230721/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.7.2/pretext/__init__.py` & `pretext-1.7.2.dev20230721/pretext/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,15 +17,40 @@
 from pathlib import Path
 from single_version import get_version
 
 log = logging.getLogger("ptxlogger")
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
-CORE_COMMIT = "9bce7e55911fb14e3e6e362bfa78bd6431c38597"
+CORE_COMMIT = '9bce7e55911fb14e3e6e362bfa78bd6431c38597'
+
+# List of templates, build formats, and assets that are supported by the CLI.
+NEW_TEMPLATES = ["book", "article", "demo", "hello", "slideshow"]
+BUILD_FORMATS = [
+    "html",
+    "pdf",
+    "latex",
+    "epub",
+    "kindle",
+    "braille",
+    "html-zip",
+    "webwork-sets",
+    "webwork-sets-zipped",
+]
+ASSETS = [
+    "ALL",
+    "webwork",
+    "latex-image",
+    "sageplot",
+    "asymptote",
+    "interactive",
+    "youtube",
+    "codelens",
+    "datafile",
+]
 
 
 def activate() -> None:
     """
     This function was provided by the original `pretext` package
     deployed to PyPI by Alex Willmer. Thanks to their generosity,
     we were allowed to adopt this namespace as of 1.0, so we raise an error here
```

### Comparing `pretext-1.7.2/pretext/build.py` & `pretext-1.7.2.dev20230721/pretext/build.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,124 +1,27 @@
 import logging
 import os
 from pathlib import Path
 import sys
 from typing import Dict, Optional
 
 from . import utils, core, codechat
-from .project.xml import Executables
 
 # Get access to logger
 log = logging.getLogger("ptxlogger")
 
 
-def build(
-    format: str,
-    ptxfile: Path,
-    pub_file: Path,
-    output: Path,
-    stringparams: Dict[str, str],
-    custom_xsl: Optional[Path],
-    xmlid: Optional[str],
-    zipped: bool = False,
-    project_path: Optional[Path] = None,
-    latex_engine: str = "xelatex",
-    executables: Dict[str, str] = Executables().dict(),
-    braille_mode: str = "emboss",
-) -> None:
-    core.set_executables(executables)
-    try:
-        if format == "html":
-            html(
-                ptxfile=ptxfile,
-                pub_file=pub_file,
-                output=output,
-                stringparams=stringparams,
-                custom_xsl=custom_xsl,
-                xmlid_root=xmlid,
-                zipped=zipped,
-                project_path=project_path,
-            )
-        elif format == "latex":
-            latex(
-                ptxfile=ptxfile,
-                pub_file=pub_file,
-                output=output,
-                stringparams=stringparams,
-                custom_xsl=custom_xsl,
-            )
-        elif format == "pdf":
-            pdf(
-                ptxfile=ptxfile,
-                pub_file=pub_file,
-                output=output,
-                stringparams=stringparams,
-                custom_xsl=custom_xsl,
-                pdf_method=latex_engine,
-            )
-        elif format == "custom":
-            if output.is_file():
-                output_filename = output.name
-                output = output.parent
-            else:
-                output_filename = None
-            assert custom_xsl is not None
-            custom(
-                ptxfile=ptxfile,
-                pub_file=pub_file,
-                output=output,
-                stringparams=stringparams,
-                custom_xsl=custom_xsl,
-                output_filename=output_filename,
-            )
-        elif format == "epub":
-            epub(
-                ptxfile=ptxfile,
-                pub_file=pub_file,
-                output=output,
-                stringparams=stringparams,
-            )
-        elif format == "kindle":
-            kindle(
-                ptxfile=ptxfile,
-                pub_file=pub_file,
-                output=output,
-                stringparams=stringparams,
-            )
-        elif format == "braille":
-            braille(
-                ptxfile=ptxfile,
-                pub_file=pub_file,
-                output=output,
-                stringparams=stringparams,
-                page_format=braille_mode,
-            )
-        elif format == "webwork":
-            webwork_sets(
-                ptxfile=ptxfile,
-                pub_file=pub_file,
-                output=output,
-                stringparams=stringparams,
-                zipped=zipped,
-            )
-        else:
-            raise NotImplementedError(f"{format} is not supported")
-    finally:
-        core.release_temporary_directories()
-
-
 def html(
     ptxfile: Path,
     pub_file: Path,
     output: Path,
     stringparams: Dict[str, str],
     custom_xsl: Optional[Path],
     xmlid_root: Optional[str],
     zipped: bool = False,
-    project_path: Optional[Path] = None,
 ) -> None:
     os.makedirs(output, exist_ok=True)
     log.info(f"\nNow building HTML into {output}\n")
     if xmlid_root is not None:
         log.info(f"Only building @xml:id `{xmlid_root}`\n")
     if zipped:
         file_format = "zip"
@@ -133,18 +36,17 @@
                 stringparams,
                 xmlid_root,
                 file_format,
                 custom_xsl and custom_xsl.as_posix(),  # pass None or posix string
                 None,
                 output.as_posix(),
             )
-            if project_path is None:
-                project_path = utils.project_path(ptxfile)
-            assert project_path is not None, f"Invalid project path to {ptxfile}."
-            codechat.map_path_to_xml_id(ptxfile, project_path, output.as_posix())
+            pp = utils.project_path(ptxfile)
+            assert pp is not None, f"Invalid project path to {ptxfile}."
+            codechat.map_path_to_xml_id(ptxfile, pp, output.as_posix())
         except Exception as e:
             log.critical(e)
             log.debug("Exception info:\n##################\n", exc_info=True)
             log.info("##################")
             sys.exit("Failed to build html.  Exiting...")
 
 
@@ -208,15 +110,14 @@
     ptxfile: Path,
     pub_file: Path,
     output: Path,
     stringparams: Dict[str, str],
     custom_xsl: Path,
     output_filename: Optional[str] = None,
 ) -> None:
-    stringparams["publisher"] = pub_file.as_posix()
     os.makedirs(output, exist_ok=True)
     if output_filename is not None:
         output_filepath = output / output_filename
         output_dir = None
         log.info(f"\nNow building with custom {custom_xsl} into {output_filepath}\n")
     else:
         output_filepath = None
```

### Comparing `pretext-1.7.2/pretext/cli.py` & `pretext-1.7.2.dev20230721/pretext/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 from typing import List, Optional, Tuple
 from .config import xml_overlay
 
 from . import (
     utils,
     templates,
     core,
-    constants,
     VERSION,
     CORE_COMMIT,
+    NEW_TEMPLATES,
+    ASSETS,
 )
 from .project import Project
 
 
 log = logging.getLogger("ptxlogger")
 click_log.basic_config(log)
 click_log_format = click_log.ColorFormatter()
@@ -173,15 +174,15 @@
 @main.command(
     short_help="Generates the necessary files for a new PreTeXt project.",
     context_settings=CONTEXT_SETTINGS,
 )
 @click.argument(
     "template",
     default="book",
-    type=click.Choice(constants.NEW_TEMPLATES, case_sensitive=False),
+    type=click.Choice(NEW_TEMPLATES, case_sensitive=False),
 )
 @click.option(
     "-d",
     "--directory",
     type=click.Path(),
     default="new-pretext-project",
     help="Directory to create/use for the project.",
@@ -320,15 +321,15 @@
 )
 @click.option(
     "-g",
     "--generate",
     is_flag=False,
     flag_value="ALL",
     default=None,
-    type=click.Choice(constants.ASSETS, case_sensitive=False),
+    type=click.Choice(ASSETS, case_sensitive=False),
     help="Generates assets for target.  -g [asset] will generate the specific assets given.",
 )
 @click.option(
     "-q",
     "--no-generate",
     is_flag=True,
     default=False,
@@ -450,15 +451,15 @@
 
 # pretext generate
 @main.command(
     short_help="Generate specified assets for specified target",
     context_settings=CONTEXT_SETTINGS,
 )
 @click.argument(
-    "assets", default="ALL", type=click.Choice(constants.ASSETS, case_sensitive=False)
+    "assets", default="ALL", type=click.Choice(ASSETS, case_sensitive=False)
 )
 @click.option(
     "-t",
     "--target",
     "target_name",
     type=click.STRING,
     help="Name of target to generate assets for (if not specified, first target from manifest is used).",
@@ -606,15 +607,15 @@
 )
 @click.option(
     "-g",
     "--generate",
     is_flag=False,
     flag_value="ALL",
     default=None,
-    type=click.Choice(constants.ASSETS, case_sensitive=False),
+    type=click.Choice(ASSETS, case_sensitive=False),
     help="Generate all or specific assets before viewing",
 )
 @click.option(
     "--no-launch",
     is_flag=True,
     help="By default, pretext view tries to launch the default application to view the specified target.  Setting this suppresses this behavior.",
 )
```

### Comparing `pretext-1.7.2/pretext/codechat.py` & `pretext-1.7.2.dev20230721/pretext/codechat.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,21 +68,18 @@
     )
 
     # lxml turns ``xml:id`` into the string below.
     xml_ns = "{http://www.w3.org/XML/1998/namespace}"
     xml_base_attrib = f"{xml_ns}base"
     xml_id_attrib = f"{xml_ns}id"
 
-    # Define a loader which sets the ``xml:base`` of an xincluded element. While lxml `evidently used to do this in 2013 <https://stackoverflow.com/a/18158472/16038919>`_, a change eliminated this ability per some `discussion <https://mail.gnome.org/archives/xml/2014-April/msg00015.html>`_, which included a rejected patch fixing this problem. `Current source <https://github.com/GNOME/libxml2/blob/master/xinclude.c#L1689>`_ lacks this patch.
+    # Define a loader which sets the ``xml:base`` of an xincluded element. While lxml `evidently used to do this in 2013 <https://stackoverflow.com/a/18158472/16038919>`_, a change eliminated this ability per some `dicussion <https://mail.gnome.org/archives/xml/2014-April/msg00015.html>`_, which included a rejected patch fixing this problem. `Current source <https://github.com/GNOME/libxml2/blob/master/xinclude.c#L1689>`_ lacks this patch.
     #
     # Since there's few docs on this function, ignore the lack of types.
-    def my_loader(href: str, parse: str, encoding: str = None, parser=None):  # type: ignore
-        # Decode the URL-encoded filename for non-xml, on-disk data. See `lxml.ElementInclude._lxml_default_loader`.
-        if parse != "xml" and "://" not in href:
-            href = urllib.parse.unquote(href)
+    def my_loader(href, parse, encoding=None, parser=None):  # type: ignore
         ret = lxml.ElementInclude._lxml_default_loader(href, parse, encoding, parser)
         # The return value may not be an element.
         if isinstance(ret, ET._Element):
             ret.attrib[xml_base_attrib] = href
         return ret
 
     # Load the XML, performing xincludes using this loader.
```

### Comparing `pretext-1.7.2/pretext/config/xml_overlay.py` & `pretext-1.7.2.dev20230721/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.2/pretext/core/pretext.py` & `pretext-1.7.2.dev20230721/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.2/pretext/core/resources.py` & `pretext-1.7.2.dev20230721/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.2/pretext/core/resources.zip` & `pretext-1.7.2.dev20230721/pretext/core/resources.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,144 +1,144 @@
 Zip file size: 1045100 bytes, number of entries: 142
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 xsl/
--rw-r--r--  2.0 unx    30908 b- defN 23-Jul-21 15:14 pretext/pretext
--rw-r--r--  2.0 unx     1955 b- defN 23-Jul-21 15:14 pretext/module-test.py
--rw-r--r--  2.0 unx     2566 b- defN 23-Jul-21 15:14 pretext/pretext.cfg
--rw-r--r--  2.0 unx   172498 b- defN 23-Jul-21 15:14 pretext/pretext.py
--rw-r--r--  2.0 unx     1367 b- defN 23-Jul-21 15:14 pretext/README.md
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 15:14 pretext/__init__.py
--rw-r--r--  2.0 unx    36045 b- defN 23-Jul-21 15:14 pretext/braille_format.py
--rw-r--r--  2.0 unx   125135 b- defN 23-Jul-21 15:14 schema/pretext.xsd
--rw-r--r--  2.0 unx      326 b- defN 23-Jul-21 15:14 schema/xml.xsd
--rw-r--r--  2.0 unx    58086 b- defN 23-Jul-21 15:14 schema/pretext.rnc
--rw-r--r--  2.0 unx    17587 b- defN 23-Jul-21 15:14 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx    25870 b- defN 23-Jul-21 15:14 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx    18421 b- defN 23-Jul-21 15:14 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx     1180 b- defN 23-Jul-21 15:14 schema/README.md
--rw-r--r--  2.0 unx   134043 b- defN 23-Jul-21 15:14 schema/pretext.xml
--rw-r--r--  2.0 unx     3135 b- defN 23-Jul-21 15:14 schema/build.sh
--rw-r--r--  2.0 unx    34210 b- defN 23-Jul-21 15:14 schema/pretext-dev.rng
--rw-r--r--  2.0 unx   101829 b- defN 23-Jul-21 15:14 schema/pretext.rng
--rw-r--r--  2.0 unx     1276 b- defN 23-Jul-21 15:14 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx     2608 b- defN 23-Jul-21 15:14 css/colors_default.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-21 15:14 css/colors_blue_red.css
--rw-r--r--  2.0 unx    12567 b- defN 23-Jul-21 15:14 css/style_oscarlevin.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-21 15:14 css/colors_green_plum.css
--rw-r--r--  2.0 unx     3473 b- defN 23-Jul-21 15:14 css/style_soundwriting.css
--rw-r--r--  2.0 unx     1338 b- defN 23-Jul-21 15:14 css/colors_red_blue.css
--rw-r--r--  2.0 unx     7761 b- defN 23-Jul-21 15:14 css/style_default.css
--rw-r--r--  2.0 unx     2438 b- defN 23-Jul-21 15:14 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jul-21 15:14 css/colors_martiansands.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jul-21 15:14 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-21 15:14 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     1280 b- defN 23-Jul-21 15:14 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-21 15:14 css/colors_orange_navy.css
--rw-r--r--  2.0 unx    14069 b- defN 23-Jul-21 15:14 css/setcolors.css
--rw-r--r--  2.0 unx     4021 b- defN 23-Jul-21 15:14 css/update_css
--rw-r--r--  2.0 unx     1865 b- defN 23-Jul-21 15:14 css/README.md
--rw-r--r--  2.0 unx     4308 b- defN 23-Jul-21 15:14 css/colors_blue_green.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-21 15:14 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx    22438 b- defN 23-Jul-21 15:14 css/pretext.css
--rw-r--r--  2.0 unx   146685 b- defN 23-Jul-21 15:14 css/mathbook-content.css
--rw-r--r--  2.0 unx   435680 b- defN 23-Jul-21 15:14 css/mathbook-3.css
--rw-r--r--  2.0 unx     1362 b- defN 23-Jul-21 15:14 css/epub.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-21 15:14 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx      691 b- defN 23-Jul-21 15:14 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-21 15:14 css/colors_green_blue.css
--rw-r--r--  2.0 unx    71198 b- defN 23-Jul-21 15:14 css/pretext_add_on.css
--rw-r--r--  2.0 unx    63664 b- defN 23-Jul-21 15:14 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     2441 b- defN 23-Jul-21 15:14 css/kindle.css
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 xsl/utilities/
--rw-r--r--  2.0 unx     2248 b- defN 23-Jul-21 15:14 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-Jul-21 15:14 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-Jul-21 15:14 xsl/entities.ent
--rw-r--r--  2.0 unx    17293 b- defN 23-Jul-21 15:14 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-Jul-21 15:14 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-Jul-21 15:14 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-Jul-21 15:14 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-Jul-21 15:14 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx   231265 b- defN 23-Jul-21 15:14 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx   611284 b- defN 23-Jul-21 15:14 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-Jul-21 15:14 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-Jul-21 15:14 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-Jul-21 15:14 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-Jul-21 15:14 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-Jul-21 15:14 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx    94587 b- defN 23-Jul-21 15:14 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-Jul-21 15:14 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-Jul-21 15:14 xsl/README.md
--rw-r--r--  2.0 unx    10708 b- defN 23-Jul-21 15:14 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-Jul-21 15:14 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-Jul-21 15:14 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-Jul-21 15:14 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-Jul-21 15:14 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-Jul-21 15:14 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx   544154 b- defN 23-Jul-21 15:14 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx   139486 b- defN 23-Jul-21 15:14 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx   548615 b- defN 23-Jul-21 15:14 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-Jul-21 15:14 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-Jul-21 15:14 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx   116581 b- defN 23-Jul-21 15:14 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-Jul-21 15:14 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-Jul-21 15:14 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-Jul-21 15:14 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-Jul-21 15:14 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-Jul-21 15:14 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-Jul-21 15:14 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-Jul-21 15:14 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx   110949 b- defN 23-Jul-21 15:14 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx    12084 b- defN 23-Jul-21 15:14 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx    14482 b- defN 23-Jul-21 15:14 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-Jul-21 15:14 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-Jul-21 15:14 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-Jul-21 15:14 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-Jul-21 15:14 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx      787 b- defN 23-Jul-21 15:14 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx    30257 b- defN 23-Jul-21 15:14 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-Jul-21 15:14 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx      513 b- defN 23-Jul-21 15:14 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4299 b- defN 23-Jul-21 15:14 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx     1810 b- defN 23-Jul-21 15:14 xsl/utilities/README.md
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 xsl/support/play-button/
--rw-r--r--  2.0 unx      486 b- defN 23-Jul-21 15:14 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5879 b- defN 23-Jul-21 15:14 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx      504 b- defN 23-Jul-21 15:14 xsl/support/README.md
--rw-r--r--  2.0 unx     5065 b- defN 23-Jul-21 15:14 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx    10306 b- defN 23-Jul-21 15:14 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-Jul-21 15:14 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx     5800 b- defN 23-Jul-21 15:14 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx     6621 b- defN 23-Jul-21 15:14 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx      722 b- defN 23-Jul-21 15:14 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     2657 b- defN 23-Jul-21 15:14 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx    16534 b- defN 23-Jul-21 15:14 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    16349 b- defN 23-Jul-21 15:14 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    15866 b- defN 23-Jul-21 15:14 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16312 b- defN 23-Jul-21 15:14 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx    15582 b- defN 23-Jul-21 15:14 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    17056 b- defN 23-Jul-21 15:14 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    16085 b- defN 23-Jul-21 15:14 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    19185 b- defN 23-Jul-21 15:14 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    17081 b- defN 23-Jul-21 15:14 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx     2286 b- defN 23-Jul-21 15:14 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx     4760 b- defN 23-Jul-21 15:14 xsl/localizations/README.md
--rw-r--r--  2.0 unx    19326 b- defN 23-Jul-21 15:14 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    17231 b- defN 23-Jul-21 15:14 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16500 b- defN 23-Jul-21 15:14 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17301 b- defN 23-Jul-21 15:14 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    20481 b- defN 23-Jul-21 15:14 xsl/localizations/ku-CKB.xml
--rw-r--r--  2.0 unx    16252 b- defN 23-Jul-21 15:14 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    16837 b- defN 23-Jul-21 15:14 xsl/localizations/af-ZA.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-Jul-21 15:14 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-Jul-21 15:14 script/mbx
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 15:14 script/mjsre/update-sre
--rw-r--r--  2.0 unx      116 b- defN 23-Jul-21 15:14 script/mjsre/package.json
--rw-r--r--  2.0 unx      481 b- defN 23-Jul-21 15:14 script/mjsre/README.md
--rw-r--r--  2.0 unx     9251 b- defN 23-Jul-21 15:14 script/mjsre/mj-sre-page.js
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

### Comparing `pretext-1.7.2/pretext/generate.py` & `pretext-1.7.2.dev20230721/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.2/pretext/project/__init__.py` & `pretext-1.7.2.dev20230721/pretext/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pickle
 from lxml import etree as ET
 from lxml.etree import _Element
 import os
 import shutil
 import logging
 import tempfile
-from .. import utils, generate, core
-from .. import build as builder
-from .. import constants
+from . import utils, generate, core
+from . import build as builder
+from . import ASSETS
 from pathlib import Path
 import sys
-from ..config.xml_overlay import ShadowXmlDocument
-from typing import Dict, List, Literal, Optional, Tuple
+from .config.xml_overlay import ShadowXmlDocument
+from typing import Dict, List, Optional, Tuple
 import hashlib
 import subprocess
 
 log = logging.getLogger("ptxlogger")
 
 asset_table_type = Dict[Tuple[str, str], bytes]
 
@@ -176,15 +176,15 @@
         if ele is None:
             return None
         else:
             return self.require_str_value(ele.text, "xmlid-root").strip()
 
     def asset_hash(self) -> asset_table_type:
         asset_hash_dict = {}
-        for asset in constants.ASSETS:
+        for asset in ASSETS:
             if asset == "webwork":
                 ww = self.source_xml().xpath(".//webwork[@*|*]")
                 assert isinstance(ww, List)
                 # WeBWorK must be regenerated every time *any* of the ww exercises change.
                 if len(ww) == 0:
                     # Only generate a hash if there are actually ww exercises in the source
                     continue
@@ -306,15 +306,15 @@
         else:
             log.error("Unable to find target.")
             return None
 
     def view(
         self,
         target_name: str,
-        access: Literal["public", "private"],
+        access: str,
         port: int,
         watch: bool = False,
         no_launch: bool = False,
     ) -> None:
         target = self.target(target_name)
         if target is None:
             log.error("Unable to find target.")
```

### Comparing `pretext-1.7.2/pretext/templates/__init__.py` & `pretext-1.7.2.dev20230721/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.2/pretext/templates/resources/.devcontainer.json` & `pretext-1.7.2.dev20230721/pretext/templates/resources/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.7.2/pretext/templates/resources/.gitignore` & `pretext-1.7.2.dev20230721/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.7.2/pretext/templates/resources/article.zip` & `pretext-1.7.2.dev20230721/pretext/templates/resources/article.zip`

 * *Files 3% similar despite different names*

#### zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 158841 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-21 15:14 .gitignore
--rw-r--r--  2.0 unx       86 b- defN 23-Jul-21 15:14 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-21 15:14 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-21 15:14 codechat_config.yaml
--rw-r--r--  2.0 unx      242 b- defN 23-Jul-21 15:14 publication/publication.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-Jul-21 15:14 source/section-2.ptx
--rw-r--r--  2.0 unx      449 b- defN 23-Jul-21 15:14 source/section-1.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-Jul-21 15:14 source/main.ptx
--rw-r--r--  2.0 unx   154806 b- defN 23-Jul-21 15:14 assets/frog.jpg
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

### Comparing `pretext-1.7.2/pretext/templates/resources/book.zip` & `pretext-1.7.2.dev20230721/pretext/templates/resources/book.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 6347 bytes, number of entries: 8
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-21 15:14 .gitignore
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-21 15:14 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-21 15:14 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-21 15:14 codechat_config.yaml
--rw-r--r--  2.0 unx     6114 b- defN 23-Jul-21 15:14 publication/publication.ptx
--rw-r--r--  2.0 unx     1767 b- defN 23-Jul-21 15:14 source/main.ptx
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

### Comparing `pretext-1.7.2/pretext/templates/resources/demo.zip` & `pretext-1.7.2.dev20230721/pretext/templates/resources/demo.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,35 +1,34 @@
-Zip file size: 172170 bytes, number of entries: 33
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-21 15:14 .gitignore
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-21 15:14 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-21 15:14 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-21 15:14 codechat_config.yaml
--rw-r--r--  2.0 unx     6092 b- defN 23-Jul-21 15:14 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 source/images/
--rw-r--r--  2.0 unx     1515 b- defN 23-Jul-21 15:14 source/ex-first.ptx
--rw-r--r--  2.0 unx     2295 b- defN 23-Jul-21 15:14 source/ch-generate.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-Jul-21 15:14 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-Jul-21 15:14 source/sec-features.ptx
--rw-r--r--  2.0 unx      777 b- defN 23-Jul-21 15:14 source/ww.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-Jul-21 15:14 source/ch-empty.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-Jul-21 15:14 source/frontmatter.ptx
--rw-r--r--  2.0 unx     2428 b- defN 23-Jul-21 15:14 source/main.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-Jul-21 15:14 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-Jul-21 15:14 source/backmatter.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-Jul-21 15:14 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-Jul-21 15:14 source/ch-features.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-Jul-21 15:14 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-Jul-21 15:14 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-Jul-21 15:14 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-Jul-21 15:14 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-Jul-21 15:14 source/docinfo.ptx
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-21 15:14 source/images/sageplot2d.sage
--rw-r--r--  2.0 unx      835 b- defN 23-Jul-21 15:14 source/images/cflag.asy
--rw-r--r--  2.0 unx       93 b- defN 23-Jul-21 15:14 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx      357 b- defN 23-Jul-21 15:14 source/images/tikz.tex
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-Jul-21 15:14 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-Jul-21 15:14 assets/jsxgraph/infinity.js
-33 files, 187859 bytes uncompressed, 168354 bytes compressed:  10.4%
+Zip file size: 172040 bytes, number of entries: 32
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
+32 files, 187912 bytes uncompressed, 168326 bytes compressed:  10.4%
```

#### zipnote {}

```diff
@@ -33,17 +33,14 @@
 
 Filename: source/ch-first with spaces.ptx
 Comment: 
 
 Filename: source/sec-features.ptx
 Comment: 
 
-Filename: source/ww.ptx
-Comment: 
-
 Filename: source/ch-empty.ptx
 Comment: 
 
 Filename: source/frontmatter.ptx
 Comment: 
 
 Filename: source/main.ptx
```

#### source/ch-generate.ptx

##### source/ch-generate.ptx

```diff
@@ -1,30 +1,86 @@
 <?xml version="1.0" encoding="utf-8"?>
 <chapter xmlns:xi="http://www.w3.org/2001/XInclude" xml:id="ch-generate">
   <title>
     <pretext/>
     features that require generation
   </title>
   <introduction>
-    <p>Here we demonstrate various kinds of assets.</p>
+    <p>
+      In
+      <c>main.ptx</c>
+      , uncomment this chapter to try building various
+      types of assets.
+    </p>
   </introduction>
   <section>
     <title>Image Examples</title>
     <xi:include href="./fig-tikz.ptx"/>
     <xi:include href="./fig-sage2d.ptx"/>
     <xi:include href="./fig-sage3d.ptx"/>
     <xi:include href="./fig-asymptote.ptx"/>
   </section>
   <section xml:id="webwork">
     <title>
       <webwork/>
       Example
     </title>
     <exercise>
-      <xi:include href="./ww.ptx"/>
+      <webwork>
+        <pg-code>$a = Compute(random(1, 9, 1));
+          $b = Compute(random(1, 9, 1));
+          $c = $a + $b;</pg-code>
+        <statement>
+          <p>
+            Compute the sum of
+            <m>
+              <var name="$a"/>
+            </m>
+            and
+            <m>
+              <var name="$b"/>
+            </m>
+            :
+          </p>
+          <p>
+            <m>
+              <var name="$a"/>
+              +
+              <var name="$b"/>
+              =
+            </m>
+            <var name="$c" width="5"/>
+          </p>
+        </statement>
+        <hint>
+          <p>
+            Add
+            <m>
+              <var name="$a"/>
+            </m>
+            and
+            <m>
+              <var name="$b"/>
+            </m>
+            together.
+          </p>
+        </hint>
+        <solution>
+          <p>
+            <m>
+              <var name="$a"/>
+              +
+              <var name="$b"/>
+              =
+              <var name="$c"/>
+            </m>
+            .
+          </p>
+        </solution>
+      </webwork>
     </exercise>
   </section>
   <section xml:id="youtube">
     <title>YouTube Example</title>
     <video youtube="dQw4w9WgXcQ"/>
   </section>
   <section>
```

#### source/main.ptx

##### source/main.ptx

```diff
@@ -28,13 +28,14 @@
     <!-- illustrate what pretext can do, plus links to more help.  -->
     <!-- We recommend keeping this handy, and commenting it out    -->
     <!-- when you show off your own work.                          -->
     <xi:include href="./ch-features.ptx"/>
     <!-- This chapter includes several features that require pregeneration   -->
     <!-- of assets with `pretext generate` or similar. Some features require -->
     <!-- internet access; others require local installs not automatically    -->
-    <!-- provided by the CLI.                                                -->
-    <xi:include href="./ch-generate.ptx"/>
+    <!-- provided by the CLI. Uncomment to view this chapter, and comment    -->
+    <!-- features you don't wish to generate.                                -->
+    <!-- <xi:include href="./ch-generate.ptx" /> -->
     <!-- Finaly we place the backmatter in its own file and inlcude-->
     <xi:include href="./backmatter.ptx"/>
   </book>
 </pretext>
```

### Comparing `pretext-1.7.2/pretext/templates/resources/hello.zip` & `pretext-1.7.2.dev20230721/pretext/templates/resources/hello.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 3388 bytes, number of entries: 8
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-21 15:14 .gitignore
--rw-r--r--  2.0 unx       69 b- defN 23-Jul-21 15:14 README.md
--rw-r--r--  2.0 unx     1217 b- defN 23-Jul-21 15:14 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-21 15:14 codechat_config.yaml
--rw-r--r--  2.0 unx      242 b- defN 23-Jul-21 15:14 publication/publication.ptx
--rw-r--r--  2.0 unx      156 b- defN 23-Jul-21 15:14 source/main.ptx
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

### Comparing `pretext-1.7.2/pretext/templates/resources/project.ptx` & `pretext-1.7.2.dev20230721/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.7.2/pretext/templates/resources/slideshow.zip` & `pretext-1.7.2.dev20230721/pretext/templates/resources/slideshow.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 7123 bytes, number of entries: 9
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 15:14 xsl/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-21 15:14 .gitignore
--rw-r--r--  2.0 unx      784 b- defN 23-Jul-21 15:14 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-21 15:14 codechat_config.yaml
--rw-r--r--  2.0 unx     2097 b- defN 23-Jul-21 15:14 publication/publication.ptx
--rw-r--r--  2.0 unx    11200 b- defN 23-Jul-21 15:14 source/main.ptx
--rw-r--r--  2.0 unx      190 b- defN 23-Jul-21 15:14 xsl/slides.xsl
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

### Comparing `pretext-1.7.2/pretext/utils.py` & `pretext-1.7.2.dev20230721/pretext/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,26 +9,25 @@
 import platform
 import re
 import socketserver
 import socket
 import subprocess
 import logging
 import logging.handlers
-import multiprocessing
 import threading
 import watchdog.events
 import watchdog.observers
 import time
 import webbrowser
 import typing as t
 from lxml import etree as ET
 from lxml.etree import _ElementTree, _Element
 from typing import Any, cast, Callable, List, Optional
 
-from . import core, templates, constants
+from . import core, templates, BUILD_FORMATS
 
 # Get access to logger
 log = logging.getLogger("ptxlogger")
 
 
 @contextmanager
 def working_directory(path: Path) -> Generator:
@@ -124,23 +123,25 @@
             f"No targets with alias {alias} found in project manifest file project.ptx."
         )
         return None
     return matches[0]
 
 
 # check xml syntax
-def xml_syntax_is_valid(xmlfile: Path, root_tag: str = "pretext") -> bool:
+def xml_syntax_is_valid(xmlfile: Path) -> bool:
     # parse xml
     try:
         source_xml = ET.parse(xmlfile)
-        source_xml.xinclude()
+        # we need to call xinclude once for each level of nesting (just to check for errors).  25 levels should be more than sufficient
+        for i in range(25):
+            source_xml.xinclude()
         log.debug("XML syntax appears well formed.")
-        if source_xml.getroot().tag != root_tag:
+        if source_xml.getroot().tag != "pretext":
             log.error(
-                f'The file {xmlfile} does not have "<{root_tag}>" as its root element.  Did you use a subfile as your source?  Check the project manifest (project.ptx).'
+                f'The file {xmlfile} does not have "<pretext>" as its root element.  Did you use a subfile as your source?  Check the project manifest (project.ptx).'
             )
             return False
     # check for file IO error
     except IOError:
         log.error(f"The file {xmlfile} does not exist")
         return False
     # check for XML syntax errors
@@ -160,15 +161,14 @@
     schemarngfile = core.resources.path("schema", "pretext.rng")
 
     # Open schemafile for validation:
     relaxng = ET.RelaxNG(file=schemarngfile)
 
     # Parse xml file:
     source_xml = ET.parse(xmlfile)
-    source_xml.xinclude()
 
     # just for testing
     # ----------------
     # relaxng.validate(source_xml)
     # log = relaxng.error_log
     # print(log)
 
@@ -212,35 +212,30 @@
                 handler.callback()
 
         threading.Thread(target=timeout_callback, args=(self,)).start()
 
 
 # boilerplate to prevent overzealous caching by preview server, and
 # avoid port issues
-def binding_for_access(access: t.Literal["public", "private"] = "private") -> str:
+def binding_for_access(access: str = "private") -> str:
     if access == "private":
         return "localhost"
     else:
         return "0.0.0.0"
 
 
-def url_for_access(
-    access: t.Literal["public", "private"] = "private", port: int = 8000
-) -> str:
+def url_for_access(access: str = "private", port: int = 8000) -> str:
     if access == "public":
         return f"http://{socket.gethostbyname(socket.gethostname())}:{port}"
     else:
         return f"http://localhost:{port}"
 
 
 def serve_forever(
-    directory: Path,
-    access: t.Literal["public", "private"] = "private",
-    port: int = 8000,
-    no_launch: bool = False,
+    directory: Path, access: str = "private", port: int = 8000, no_launch: bool = False
 ) -> None:
     log.info(f"Now preparing local server to preview directory `{directory}`.")
     log.info(
         "  (Reminder: use `pretext deploy` to deploy your built project to a public"
     )
     log.info(
         "  GitHub Pages site that can be shared with readers who cannot access your"
@@ -286,15 +281,15 @@
             log.warning(f"Port {port} could not be used.")
             port = random.randint(49152, 65535)
             log.warning(f"Trying port {port} instead.\n")
 
 
 def run_server(
     directory: Path,
-    access: t.Literal["public", "private"],
+    access: str,
     port: int,
     watch_directory: t.Optional[Path] = None,
     watch_callback: Callable[[], None] = lambda: None,
     no_launch: bool = False,
 ) -> None:
     threading.Thread(
         target=lambda: serve_forever(directory, access, port, no_launch), daemon=True
@@ -312,25 +307,14 @@
         log.info("\nClosing server...")
         if watch_directory is not None:
             observer.stop()
     if watch_directory is not None:
         observer.join()
 
 
-def server_process(
-    directory: Path,
-    access: t.Literal["public", "private"],
-    port: int,
-    launch: bool = True,
-) -> multiprocessing.Process:
-    return multiprocessing.Process(
-        target=serve_forever, args=[directory, access, port, not launch]
-    )
-
-
 # Info on namespaces: http://lxml.de/tutorial.html#namespaces
 NSMAP = {
     "xi": "http://www.w3.org/2001/XInclude",
     "xml": "http://www.w3.org/XML/1998/namespace",
 }
 
 
@@ -447,15 +431,15 @@
     # just in case this was called in the wrong place:
     if project.target(name=target_format) is not None:
         return
     # Otherwise continue with hints:
     log.critical(
         f'There is not a target named "{target_format}" for this project.ptx manifest.'
     )
-    if target_format in constants.BUILD_FORMATS:
+    if target_format in BUILD_FORMATS:
         target_names = project.target_names(target_format)
         if len(target_names) == 1:
             log.info(
                 f'However, the target named "{target_names[0]}" has "{target_format}" as its format.  Try to {task} that instead or edit your project.ptx manifest.'
             )
         elif len(target_names) > 1:
             log.info(
```

### Comparing `pretext-1.7.2/pyproject.toml` & `pretext-1.7.2.dev20230721/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # See https://python-poetry.org/docs/dependency-specification/ to get an understanding of
 # how poetry specifies dependencies.
 #
 # Project metadata
 # ----------------
 [tool.poetry]
 name = "pretext"
-version = "1.7.2"
+version = "1.7.2.dev20230721"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
@@ -35,15 +35,14 @@
 click = "^8"
 pdfCropMargins = "~1.0.9"
 PyPDF2 = "~2.5"
 click-log = "^0.4"
 ghp-import = "^2"
 single-version = "^1"
 playwright = "^1"
-pydantic-xml = "^1"
 qrcode = "^7"
 
 # Development dependencies
 # ------------------------
 [tool.poetry.group.dev.dependencies]
 black = "^23"
 codechat-server = "^0"
```

### Comparing `pretext-1.7.2/PKG-INFO` & `pretext-1.7.2.dev20230721/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.7.2
+Version: 1.7.2.dev20230721
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -16,15 +16,14 @@
 Requires-Dist: PyPDF2 (>=2.5,<2.6)
 Requires-Dist: click (>=8,<9)
 Requires-Dist: click-log (>=0.4,<0.5)
 Requires-Dist: ghp-import (>=2,<3)
 Requires-Dist: lxml (>=4.8,<5.0)
 Requires-Dist: pdfCropMargins (>=1.0.9,<1.1.0)
 Requires-Dist: playwright (>=1,<2)
-Requires-Dist: pydantic-xml (>=1,<2)
 Requires-Dist: qrcode (>=7,<8)
 Requires-Dist: requests (>=2,<3)
 Requires-Dist: single-version (>=1,<2)
 Requires-Dist: watchdog (>=2,<3)
 Project-URL: Repository, https://github.com/PreTeXtBook/pretext-cli
 Description-Content-Type: text/markdown
```

