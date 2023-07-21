# Comparing `tmp/pyprocessors_generative_augmenter-0.5.17.tar.gz` & `tmp/pyprocessors-generative_augmenter-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprocessors_generative_augmenter-0.5.17.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyprocessors-generative_augmenter-0.5.9.tar", last modified: Thu Apr 27 11:12:50 2023, max compression
```

## Comparing `pyprocessors_generative_augmenter-0.5.17.tar` & `pyprocessors-generative_augmenter-0.5.9.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0       97 2023-07-21 07:14:22.947893 pyprocessors_generative_augmenter-0.5.17/.dockerignore
--rw-r--r--   0        0        0      167 2023-07-21 07:14:22.947893 pyprocessors_generative_augmenter-0.5.17/.gitignore
--rw-r--r--   0        0        0      448 2023-07-21 07:14:22.947893 pyprocessors_generative_augmenter-0.5.17/Dockerfile
--rw-r--r--   0        0        0    10240 2023-07-21 07:14:22.948893 pyprocessors_generative_augmenter-0.5.17/Jenkinsfile
--rw-r--r--   0        0        0      380 2023-07-21 07:14:22.948893 pyprocessors_generative_augmenter-0.5.17/README.md
--rw-r--r--   0        0        0     1559 2023-07-21 07:14:22.949893 pyprocessors_generative_augmenter-0.5.17/bumpversion.py
--rw-r--r--   0        0        0       55 2023-07-21 07:16:41.444816 pyprocessors_generative_augmenter-0.5.17/pyprocessors_generative_augmenter/__init__.py
--rw-r--r--   0        0        0     5927 2023-07-21 07:14:22.950893 pyprocessors_generative_augmenter-0.5.17/pyprocessors_generative_augmenter/generative_augmenter.py
--rw-r--r--   0        0        0     2600 2023-07-21 07:14:22.950893 pyprocessors_generative_augmenter-0.5.17/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 07:14:22.950893 pyprocessors_generative_augmenter-0.5.17/tests/__init__.py
--rw-r--r--   0        0        0     9161 2023-07-21 07:14:22.951893 pyprocessors_generative_augmenter-0.5.17/tests/data/jinjadocs.json
--rw-r--r--   0        0        0     3031 2023-07-21 07:14:22.952893 pyprocessors_generative_augmenter-0.5.17/tests/data/jinjadocs_en.json
--rw-r--r--   0        0        0    13529 2023-07-21 07:14:22.953893 pyprocessors_generative_augmenter-0.5.17/tests/data/jinjadocs_preserve_entities.json
--rw-r--r--   0        0        0    17884 2023-07-21 07:16:38.492732 pyprocessors_generative_augmenter-0.5.17/tests/data/jinjadocs_preserve_entities_augmented.json
--rw-r--r--   0        0        0    14427 2023-07-21 07:14:22.955893 pyprocessors_generative_augmenter-0.5.17/tests/data/jinjadocs_substitute_entities.json
--rw-r--r--   0        0        0    19309 2023-07-21 07:16:38.497732 pyprocessors_generative_augmenter-0.5.17/tests/data/jinjadocs_substitute_entities_augmented.json
--rw-r--r--   0        0        0     2384 2023-07-21 07:14:22.956894 pyprocessors_generative_augmenter-0.5.17/tests/test_generative_augmenter.py
--rw-r--r--   0        0        0      951 2023-07-21 07:14:22.957893 pyprocessors_generative_augmenter-0.5.17/tox.ini
--rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 pyprocessors_generative_augmenter-0.5.17/setup.py
--rw-r--r--   0        0        0     2498 1970-01-01 00:00:00.000000 pyprocessors_generative_augmenter-0.5.17/PKG-INFO
+-rw-r--r--   0        0        0       97 2023-04-27 10:51:51.452409 pyprocessors-generative_augmenter-0.5.9/.dockerignore
+-rw-r--r--   0        0        0      167 2023-04-27 11:04:50.634861 pyprocessors-generative_augmenter-0.5.9/.gitignore
+-rw-r--r--   0        0        0      448 2023-04-27 10:51:51.452409 pyprocessors-generative_augmenter-0.5.9/Dockerfile
+-rw-r--r--   0        0        0    10240 2023-04-27 10:51:51.452409 pyprocessors-generative_augmenter-0.5.9/Jenkinsfile
+-rw-r--r--   0        0        0      380 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.9/README.md
+-rw-r--r--   0        0        0     1559 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.9/bumpversion.py
+-rw-r--r--   0        0        0       54 2023-04-27 11:12:49.262433 pyprocessors-generative_augmenter-0.5.9/pyprocessors_generative_augmenter/__init__.py
+-rw-r--r--   0        0        0     5857 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.9/pyprocessors_generative_augmenter/generative_augmenter.py
+-rw-r--r--   0        0        0     2593 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.9/tests/__init__.py
+-rw-r--r--   0        0        0     9161 2023-04-27 10:51:51.454409 pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs.json
+-rw-r--r--   0        0        0     6757 2023-04-27 10:51:51.454409 pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs_preserve_entities.json
+-rw-r--r--   0        0        0     7931 2023-04-27 11:12:46.257354 pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs_preserve_entities_augmented.json
+-rw-r--r--   0        0        0     6713 2023-04-27 10:51:51.454409 pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs_substitute_entities.json
+-rw-r--r--   0        0        0     8111 2023-04-27 11:12:46.260354 pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs_substitute_entities_augmented.json
+-rw-r--r--   0        0        0     1379 2023-04-27 10:51:51.455409 pyprocessors-generative_augmenter-0.5.9/tests/test_generative_augmenter.py
+-rw-r--r--   0        0        0      951 2023-04-27 10:51:51.455409 pyprocessors-generative_augmenter-0.5.9/tox.ini
+-rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 pyprocessors-generative_augmenter-0.5.9/setup.py
+-rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 pyprocessors-generative_augmenter-0.5.9/PKG-INFO
```

### Comparing `pyprocessors_generative_augmenter-0.5.17/Jenkinsfile` & `pyprocessors-generative_augmenter-0.5.9/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `pyprocessors_generative_augmenter-0.5.17/bumpversion.py` & `pyprocessors-generative_augmenter-0.5.9/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_generative_augmenter-0.5.17/pyprocessors_generative_augmenter/generative_augmenter.py` & `pyprocessors-generative_augmenter-0.5.9/pyprocessors_generative_augmenter/generative_augmenter.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         "variants",
         description="""The alternative text where are stored the variants generated by another component.""",
     )
     variant_separator_regex: Optional[str] = Field(
         None, description="Regex used to split variants", extra="advanced"
     )
     annotation_regex: Optional[str] = Field(
-        "\\[(?P<label>[^:\\]]+):(?P<text>[^]]+)\\]", description="Regex used to extract entities with labels",
+        "\\[(?P<label>[^:]+):(?P<text>[^]]+)\\]", description="Regex used to extract entities with labels",
         extra="advanced"
     )
 
 
 class GenerativeAugmenterProcessor(ProcessorBase):
     __doc__ = """Replace text of the input document by the variants and replace the existing annotations in text."""
 
@@ -49,15 +49,15 @@
             for document in documents:
                 altTexts = document.altTexts or []
                 variant_altText = next(alt for alt in altTexts if
                                        alt.name == params.variant_altText)
                 sentences = []
                 annotations = []
                 dtext = ""
-                if variant_altText:
+                if params.variant_separator_regex is not None and variant_altText:
                     variant_text = variant_altText.text
                     for stext, sannots in segment_augmented_text(document, variant_text, params):
                         sentences.append(Sentence(start=len(dtext), end=len(dtext) + len(stext)))
                         for a in sannots:
                             a.start += len(dtext)
                             a.end += len(dtext)
                             annotations.append(a)
@@ -124,19 +124,17 @@
                 rtext += atext
                 sstart = match.end()
             if sstart < len(stext):
                 rtext += stext[sstart:]
             return rtext, annotations
 
     sstart = -1
-    if params.variant_separator_regex:
-        matches = re.finditer(params.variant_separator_regex, variant_text, re.MULTILINE)
-        for matchNum, match in enumerate(matches, start=1):
-            send = match.start()
-            if sstart >= 0:
-                stext = variant_text[sstart:send]
-                yield extract_annotations(stext)
-            sstart = match.end()
+    matches = re.finditer(params.variant_separator_regex, variant_text, re.MULTILINE)
+    for matchNum, match in enumerate(matches, start=1):
+        send = match.start()
+        if sstart >= 0:
+            stext = variant_text[sstart:send]
+            yield extract_annotations(stext)
+        sstart = match.end()
     if sstart < len(variant_text):
-        sstart = 0 if sstart == -1 else sstart
         stext = variant_text[sstart:]
         yield extract_annotations(stext)
```

### Comparing `pyprocessors_generative_augmenter-0.5.17/pyproject.toml` & `pyprocessors-generative_augmenter-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 [tool.flit.entrypoints."pyprocessors.plugins"]
 generative_augmenter = "pyprocessors_generative_augmenter.generative_augmenter:GenerativeAugmenterProcessor"
 
 
 [tool.flit.metadata.requires-extra]
 test = [
-    "pytest>=7.0.0",
+    "pytest",
     "pytest-cov",
     "pytest-flake8",
     "pytest-black",
 #    "hypothesis",
     "flake8==3.9.2",
     "tox",
     "dirty-equals",
```

### Comparing `pyprocessors_generative_augmenter-0.5.17/tests/data/jinjadocs.json` & `pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_generative_augmenter-0.5.17/tox.ini` & `pyprocessors-generative_augmenter-0.5.9/tox.ini`

 * *Files identical despite different names*

### Comparing `pyprocessors_generative_augmenter-0.5.17/setup.py` & `pyprocessors-generative_augmenter-0.5.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,30 +15,30 @@
 extras_require = \
 {'dev': ['flit', 'pre-commit', 'bump2version'],
  'docs': ['sphinx',
           'sphinx-rtd-theme',
           'm2r2',
           'sphinxcontrib.apidoc',
           'jupyter_sphinx'],
- 'test': ['pytest>=7.0.0',
+ 'test': ['pytest',
           'pytest-cov',
           'pytest-flake8',
           'pytest-black',
           'flake8==3.9.2',
           'tox',
           'dirty-equals',
           'werkzeug==2.0.0',
           'flask==2.1.3']}
 
 entry_points = \
 {'pyprocessors.plugins': ['generative_augmenter = '
                           'pyprocessors_generative_augmenter.generative_augmenter:GenerativeAugmenterProcessor']}
 
 setup(name='pyprocessors-generative_augmenter',
-      version='0.5.17',
+      version='0.5.9',
       description='GenerativeazA$$ processor',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://kairntech.com/',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `pyprocessors_generative_augmenter-0.5.17/PKG-INFO` & `pyprocessors-generative_augmenter-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprocessors-generative_augmenter
-Version: 0.5.17
+Version: 0.5.9
 Summary: GenerativeazA$$ processor
 Home-page: https://kairntech.com/
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
@@ -32,15 +32,15 @@
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: bump2version ; extra == "dev"
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme ; extra == "docs"
 Requires-Dist: m2r2 ; extra == "docs"
 Requires-Dist: sphinxcontrib.apidoc ; extra == "docs"
 Requires-Dist: jupyter_sphinx ; extra == "docs"
-Requires-Dist: pytest>=7.0.0 ; extra == "test"
+Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-flake8 ; extra == "test"
 Requires-Dist: pytest-black ; extra == "test"
 Requires-Dist: flake8==3.9.2 ; extra == "test"
 Requires-Dist: tox ; extra == "test"
 Requires-Dist: dirty-equals ; extra == "test"
 Requires-Dist: werkzeug==2.0.0 ; extra == "test"
```

