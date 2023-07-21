# Comparing `tmp/exonviz-0.1.0.tar.gz` & `tmp/exonviz-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exonviz-0.1.0.tar", last modified: Tue Jul 11 14:11:04 2023, max compression
+gzip compressed data, was "exonviz-0.1.1.tar", last modified: Fri Jul 21 06:51:47 2023, max compression
```

## Comparing `exonviz-0.1.0.tar` & `exonviz-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-11 14:11:04.329136 exonviz-0.1.0/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)    34523 2023-07-11 13:50:44.000000 exonviz-0.1.0/LICENSE
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3887 2023-07-11 14:11:04.329136 exonviz-0.1.0/PKG-INFO
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2881 2023-07-11 13:50:44.000000 exonviz-0.1.0/README.md
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       38 2023-07-11 14:11:04.329136 exonviz-0.1.0/setup.cfg
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2754 2023-07-11 14:06:15.000000 exonviz-0.1.0/setup.py
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-11 14:11:04.325135 exonviz-0.1.0/src/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        0 2023-07-11 13:50:44.000000 exonviz-0.1.0/src/conftest.py
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-11 14:11:04.325135 exonviz-0.1.0/src/exonviz/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        0 2023-07-11 13:50:44.000000 exonviz-0.1.0/src/exonviz/__init__.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       61 2023-07-11 13:50:44.000000 exonviz-0.1.0/src/exonviz/__main__.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2390 2023-07-11 13:50:44.000000 exonviz-0.1.0/src/exonviz/cli.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     5970 2023-07-11 13:50:44.000000 exonviz-0.1.0/src/exonviz/draw.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3039 2023-07-11 13:50:44.000000 exonviz-0.1.0/src/exonviz/exon.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2056 2023-07-11 13:50:44.000000 exonviz-0.1.0/src/exonviz/mutalyzer.py
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-11 14:11:04.325135 exonviz-0.1.0/src/exonviz.egg-info/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3887 2023-07-11 14:11:04.000000 exonviz-0.1.0/src/exonviz.egg-info/PKG-INFO
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)      505 2023-07-11 14:11:04.000000 exonviz-0.1.0/src/exonviz.egg-info/SOURCES.txt
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        1 2023-07-11 14:11:04.000000 exonviz-0.1.0/src/exonviz.egg-info/dependency_links.txt
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       45 2023-07-11 14:11:04.000000 exonviz-0.1.0/src/exonviz.egg-info/entry_points.txt
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        1 2023-07-11 13:51:11.000000 exonviz-0.1.0/src/exonviz.egg-info/not-zip-safe
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        7 2023-07-11 14:11:04.000000 exonviz-0.1.0/src/exonviz.egg-info/requires.txt
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       17 2023-07-11 14:11:04.000000 exonviz-0.1.0/src/exonviz.egg-info/top_level.txt
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-11 14:11:04.325135 exonviz-0.1.0/tests/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     7408 2023-07-11 13:50:44.000000 exonviz-0.1.0/tests/test_Exon.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1090 2023-07-11 13:50:44.000000 exonviz-0.1.0/tests/test_cli.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1958 2023-07-11 13:50:44.000000 exonviz-0.1.0/tests/test_draw_exon.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1699 2023-07-11 13:50:44.000000 exonviz-0.1.0/tests/test_mutalyzer.py
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 06:51:47.665556 exonviz-0.1.1/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)    34523 2023-07-11 13:50:44.000000 exonviz-0.1.1/LICENSE
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3992 2023-07-21 06:51:47.665556 exonviz-0.1.1/PKG-INFO
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2986 2023-07-11 14:22:54.000000 exonviz-0.1.1/README.md
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       38 2023-07-21 06:51:47.665556 exonviz-0.1.1/setup.cfg
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2812 2023-07-21 06:36:22.000000 exonviz-0.1.1/setup.py
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 06:51:47.661555 exonviz-0.1.1/src/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        0 2023-07-11 13:50:44.000000 exonviz-0.1.1/src/conftest.py
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 06:51:47.661555 exonviz-0.1.1/src/exonviz/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       89 2023-07-21 06:23:07.000000 exonviz-0.1.1/src/exonviz/__init__.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       61 2023-07-11 13:50:44.000000 exonviz-0.1.1/src/exonviz/__main__.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2331 2023-07-21 06:35:48.000000 exonviz-0.1.1/src/exonviz/cli.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     5970 2023-07-11 13:50:44.000000 exonviz-0.1.1/src/exonviz/draw.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3039 2023-07-11 13:50:44.000000 exonviz-0.1.1/src/exonviz/exon.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2056 2023-07-21 06:32:19.000000 exonviz-0.1.1/src/exonviz/mutalyzer.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 06:02:29.000000 exonviz-0.1.1/src/exonviz/py.typed
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 06:51:47.661555 exonviz-0.1.1/src/exonviz.egg-info/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3992 2023-07-21 06:51:47.000000 exonviz-0.1.1/src/exonviz.egg-info/PKG-INFO
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)      526 2023-07-21 06:51:47.000000 exonviz-0.1.1/src/exonviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        1 2023-07-21 06:51:47.000000 exonviz-0.1.1/src/exonviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       45 2023-07-21 06:51:47.000000 exonviz-0.1.1/src/exonviz.egg-info/entry_points.txt
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        1 2023-07-11 13:51:11.000000 exonviz-0.1.1/src/exonviz.egg-info/not-zip-safe
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        7 2023-07-21 06:51:47.000000 exonviz-0.1.1/src/exonviz.egg-info/requires.txt
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       17 2023-07-21 06:51:47.000000 exonviz-0.1.1/src/exonviz.egg-info/top_level.txt
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 06:51:47.665556 exonviz-0.1.1/tests/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     7408 2023-07-11 13:50:44.000000 exonviz-0.1.1/tests/test_Exon.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1090 2023-07-11 13:50:44.000000 exonviz-0.1.1/tests/test_cli.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1958 2023-07-11 13:50:44.000000 exonviz-0.1.1/tests/test_draw_exon.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1699 2023-07-11 13:50:44.000000 exonviz-0.1.1/tests/test_mutalyzer.py
```

### Comparing `exonviz-0.1.0/LICENSE` & `exonviz-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.0/PKG-INFO` & `exonviz-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exonviz
-Version: 0.1.0
+Version: 0.1.1
 Summary: Visualise exons and their reading frames
 Home-page: https://github.com/redmar-van-den-berg/exonviz
 Author: Redmar van den Berg
 Author-email: RedmarvandenBerg@lumc.nl
 License: AGPL-3.0
 Project-URL: Changelog, https://github.com/redmar-van-den-berg/exonviz/blob/main/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/redmar-van-den-berg/exonviz/issues
@@ -26,20 +26,28 @@
 [![Continous integration](https://github.com/Redmar-van-den-Berg/exonviz/actions/workflows/ci.yml/badge.svg)](https://github.com/Redmar-van-den-Berg/exonviz/actions/workflows/ci.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 
 # Exonviz
 Visualise exons
 ------------------------------------------------------------------------
+## Installation
+Exonviz only requires Python, and can be installed using PIP:
+```
+pip install exonviz
+```
+
+
 ## Usage
 Pass either a transcript (with version!), or a valid HGVS description to exonviz to generate a figure.
+
 ### Options
 Since each gene is different, you will probably want to play around with the options to get the perfect figure for your favorite gene.
 
-```bash
+```
 
 usage: exonviz [-h] [--max-width MAX_WIDTH] [--height HEIGHT] [--non-coding]
                [--gap GAP]
                transcript
 
 Description of command.
```

### Comparing `exonviz-0.1.0/README.md` & `exonviz-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 [![Continous integration](https://github.com/Redmar-van-den-Berg/exonviz/actions/workflows/ci.yml/badge.svg)](https://github.com/Redmar-van-den-Berg/exonviz/actions/workflows/ci.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 
 # Exonviz
 Visualise exons
 ------------------------------------------------------------------------
+## Installation
+Exonviz only requires Python, and can be installed using PIP:
+```
+pip install exonviz
+```
+
+
 ## Usage
 Pass either a transcript (with version!), or a valid HGVS description to exonviz to generate a figure.
+
 ### Options
 Since each gene is different, you will probably want to play around with the options to get the perfect figure for your favorite gene.
 
-```bash
+```
 
 usage: exonviz [-h] [--max-width MAX_WIDTH] [--height HEIGHT] [--non-coding]
                [--gap GAP]
                transcript
 
 Description of command.
```

### Comparing `exonviz-0.1.0/setup.py` & `exonviz-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,26 +23,29 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="exonviz",
-    version="0.1.0",
+    version="0.1.1",
     license="AGPL-3.0",
     description="Visualise exons and their reading frames",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Redmar van den Berg",
     author_email="RedmarvandenBerg@lumc.nl",
     url="https://github.com/redmar-van-den-berg/exonviz",
     packages=find_packages("src"),
     package_dir={"": "src"},
     py_modules=[splitext(basename(path))[0] for path in glob("src/*.py")],
     include_package_data=True,
+    package_data={
+        "exonviz": ["py.typed"]
+    },
     zip_safe=False,
     classifiers=[
         # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: Unix",
```

### Comparing `exonviz-0.1.0/src/exonviz/cli.py` & `exonviz-0.1.1/src/exonviz/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 
     return transcript
 
 
 def fetch_exons(transcript: str) -> Tuple[List[Exon], bool]:
     """Make or fetch the requested exons"""
 
+    # Does the transcript format make sense?
+    transcript = check_input(transcript)
+
     payload = mutalyzer(transcript)
     if payload:
         return extract_exons(payload)
     else:
         return list(), False
 
 
@@ -53,27 +56,20 @@
         action="store_true",
         default=False,
         help="Show non coding regions",
     )
     parser.add_argument("--gap", type=int, help="Gap between the exons", default=None)
     args = parser.parse_args()
 
-    # Does the transcript format make sense?
-    try:
-        transcript = check_input(args.transcript)
-    except RuntimeError as e:
-        print(e)
-        exit(1)
-
     # Try to talk to mutalyzer
     try:
-        exons, reverse = fetch_exons(transcript)
+        exons, reverse = fetch_exons(args.transcript)
     except RuntimeError as e:
-        print(e)
-        exit(2)
+        print(e, file=sys.stderr)
+        exit(1)
 
     for exon in exons:
         print(exon, file=sys.stderr)
     plot = draw_exons(
         exons,
         reverse,
         max_width=args.max_width,
```

### Comparing `exonviz-0.1.0/src/exonviz/draw.py` & `exonviz-0.1.1/src/exonviz/draw.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.0/src/exonviz/exon.py` & `exonviz-0.1.1/src/exonviz/exon.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.0/src/exonviz/mutalyzer.py` & `exonviz-0.1.1/src/exonviz/mutalyzer.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.0/src/exonviz.egg-info/PKG-INFO` & `exonviz-0.1.1/src/exonviz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exonviz
-Version: 0.1.0
+Version: 0.1.1
 Summary: Visualise exons and their reading frames
 Home-page: https://github.com/redmar-van-den-berg/exonviz
 Author: Redmar van den Berg
 Author-email: RedmarvandenBerg@lumc.nl
 License: AGPL-3.0
 Project-URL: Changelog, https://github.com/redmar-van-den-berg/exonviz/blob/main/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/redmar-van-den-berg/exonviz/issues
@@ -26,20 +26,28 @@
 [![Continous integration](https://github.com/Redmar-van-den-Berg/exonviz/actions/workflows/ci.yml/badge.svg)](https://github.com/Redmar-van-den-Berg/exonviz/actions/workflows/ci.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 
 # Exonviz
 Visualise exons
 ------------------------------------------------------------------------
+## Installation
+Exonviz only requires Python, and can be installed using PIP:
+```
+pip install exonviz
+```
+
+
 ## Usage
 Pass either a transcript (with version!), or a valid HGVS description to exonviz to generate a figure.
+
 ### Options
 Since each gene is different, you will probably want to play around with the options to get the perfect figure for your favorite gene.
 
-```bash
+```
 
 usage: exonviz [-h] [--max-width MAX_WIDTH] [--height HEIGHT] [--non-coding]
                [--gap GAP]
                transcript
 
 Description of command.
```

### Comparing `exonviz-0.1.0/tests/test_Exon.py` & `exonviz-0.1.1/tests/test_Exon.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.0/tests/test_cli.py` & `exonviz-0.1.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.0/tests/test_draw_exon.py` & `exonviz-0.1.1/tests/test_draw_exon.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.0/tests/test_mutalyzer.py` & `exonviz-0.1.1/tests/test_mutalyzer.py`

 * *Files identical despite different names*

