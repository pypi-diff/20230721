# Comparing `tmp/mtrain-superclient-0.2.0.tar.gz` & `tmp/mtrain-superclient-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtrain-superclient-0.2.0.tar", max compression
+gzip compressed data, was "mtrain-superclient-0.3.0.tar", max compression
```

## Comparing `mtrain-superclient-0.2.0.tar` & `mtrain-superclient-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0     1077 2023-03-15 21:57:55.572106 mtrain-superclient-0.2.0/LICENSE
--rw-r--r--   0        0        0     2578 2023-03-15 21:57:55.572372 mtrain-superclient-0.2.0/README.md
--rw-r--r--   0        0        0     1939 2023-06-28 20:35:44.312676 mtrain-superclient-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       63 2023-03-15 21:57:55.578126 mtrain-superclient-0.2.0/src/mtrain_superclient/__init__.py
--rw-r--r--   0        0        0      226 2023-03-15 21:57:55.578252 mtrain-superclient-0.2.0/src/mtrain_superclient/__main__.py
--rw-r--r--   0        0        0    10321 2023-06-28 19:40:18.563802 mtrain-superclient-0.2.0/src/mtrain_superclient/client.py
--rw-r--r--   0        0        0      209 2023-03-15 21:57:55.579228 mtrain-superclient-0.2.0/src/mtrain_superclient/exceptions.py
--rw-r--r--   0        0        0     1089 2023-06-28 19:40:18.564364 mtrain-superclient-0.2.0/src/mtrain_superclient/mtrain_lims.py
--rwxr-xr-x   0        0        0      325 2023-06-28 19:40:18.565151 mtrain-superclient-0.2.0/src/mtrain_superclient/mtrain_lims_upload.sh
--rw-r--r--   0        0        0        0 2023-03-15 21:57:55.579335 mtrain-superclient-0.2.0/src/mtrain_superclient/py.typed
--rw-r--r--   0        0        0     4701 2023-03-26 13:56:29.198507 mtrain-superclient-0.2.0/src/mtrain_superclient/utils.py
--rw-r--r--   0        0        0     3564 2023-06-28 20:36:03.006708 mtrain-superclient-0.2.0/setup.py
--rw-r--r--   0        0        0     3554 2023-06-28 20:36:03.007259 mtrain-superclient-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-03-15 21:57:55.572106 mtrain-superclient-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2578 2023-03-15 21:57:55.572372 mtrain-superclient-0.3.0/README.md
+-rw-r--r--   0        0        0     2059 2023-07-21 21:46:12.966356 mtrain-superclient-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-07-19 21:36:09.530106 mtrain-superclient-0.3.0/src/mtrain_superclient/__init__.py
+-rw-r--r--   0        0        0     6539 2023-07-21 21:43:34.518350 mtrain-superclient-0.3.0/src/mtrain_superclient/__main__.py
+-rw-r--r--   0        0        0      712 2023-07-19 21:24:21.644285 mtrain-superclient-0.3.0/src/mtrain_superclient/autoconfig.py
+-rw-r--r--   0        0        0    12302 2023-07-11 19:34:52.086842 mtrain-superclient-0.3.0/src/mtrain_superclient/client.py
+-rw-r--r--   0        0        0      209 2023-03-15 21:57:55.579228 mtrain-superclient-0.3.0/src/mtrain_superclient/exceptions.py
+-rw-r--r--   0        0        0     4985 2023-07-21 17:52:51.991685 mtrain-superclient-0.3.0/src/mtrain_superclient/github_regimens.py
+-rw-r--r--   0        0        0     3561 2023-07-21 20:14:32.385644 mtrain-superclient-0.3.0/src/mtrain_superclient/models.py
+-rw-r--r--   0        0        0     1089 2023-06-28 19:40:18.564364 mtrain-superclient-0.3.0/src/mtrain_superclient/mtrain_lims.py
+-rwxr-xr-x   0        0        0      325 2023-06-28 19:40:18.565151 mtrain-superclient-0.3.0/src/mtrain_superclient/mtrain_lims_upload.sh
+-rw-r--r--   0        0        0        0 2023-03-15 21:57:55.579335 mtrain-superclient-0.3.0/src/mtrain_superclient/py.typed
+-rw-r--r--   0        0        0     6916 2023-07-21 08:20:55.644089 mtrain-superclient-0.3.0/src/mtrain_superclient/utils.py
+-rw-r--r--   0        0        0     3716 2023-07-21 21:50:30.262038 mtrain-superclient-0.3.0/setup.py
+-rw-r--r--   0        0        0     3774 2023-07-21 21:50:30.263770 mtrain-superclient-0.3.0/PKG-INFO
```

### Comparing `mtrain-superclient-0.2.0/LICENSE` & `mtrain-superclient-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mtrain-superclient-0.2.0/README.md` & `mtrain-superclient-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mtrain-superclient-0.2.0/pyproject.toml` & `mtrain-superclient-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mtrain-superclient"
-version = "0.2.0"
+version = "0.3.0"
 description = "Mtrain Superclient"
 authors = ["Christopher Mochizuki <chrism@alleninstitute.org>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/mochic/mtrain-superclient"
 repository = "https://github.com/mochic/mtrain-superclient"
 documentation = "https://mtrain-superclient.readthedocs.io"
@@ -16,14 +16,19 @@
 Changelog = "https://github.com/mochic/mtrain-superclient/releases"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 click = ">=8.0.1"
 pytest = "^7.2.1"
 requests = "^2.31.0"
+pydantic = "^2.0"
+PyGithub = "^1.59.0"
+"ruamel.yaml" = "^0.17.32"
+"ruamel.yaml.string" = "^0.1.1"
+np-config = "^0.4.25"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
```

### Comparing `mtrain-superclient-0.2.0/src/mtrain_superclient/client.py` & `mtrain-superclient-0.3.0/src/mtrain_superclient/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 import sys
 import functools
 import subprocess
 import yaml
 from copy import deepcopy
 
-from . import exceptions, utils, mtrain_lims
+from . import exceptions, utils, mtrain_lims, models
 
 logger = logging.getLogger(__name__)
 
 
 def logged_in_guard(method):
     """Decorator to protect methods that require the client to be logged in.
 
@@ -30,15 +30,15 @@
     return wrapper
 
 
 class Client:
 
     SERIALIZE_PARAM_NAMES = ("q", )
     ENTITIES = ("regimens", "states", "subjects",
-                "stages", "behavior_sessions", )
+                "stages", "behavior_sessions", "transitions", )
 
     def __init__(self, api_base: str, username: str, password: str, login=True):
         self._logged_in = False
         self.__logged_in = False
         self.__api_base = api_base
         self.__username = username
         self.__password = password
@@ -111,14 +111,61 @@
         logger.debug("Response JSON: %s" % response_json)
         objects = response_json["objects"]
         if not len(objects) > 0:
             raise exceptions.NotFoundError("No objects returned from query.")
 
         return objects[0]
 
+    def get_full_regimen(self, regimen_name: str) -> models.Regimen:
+        """Gets a full regimen, including stages and states
+        """
+        regimen_record = self.get(
+            entity_name="regimens",
+            filter_property_name="name",
+            filter_property_value=regimen_name
+        )
+        logger.debug("Fetched regimen: %s" % regimen_record)
+        logger.info("Fetched regimen_id: %s" % regimen_record["id"])
+        transitions = []
+        for state in regimen_record["states"]:
+            try:
+                transition_record = self.get(
+                    entity_name="transitions",
+                    filter_property_name="source_state_id",
+                    filter_property_value=state["id"],
+                )
+                transitions.append(models.Transition(
+                    trigger=transition_record.get("trigger"),
+                    source=utils.resolve_stage_name(
+                        regimen_record,
+                        transition_record["source_state_id"],
+                    ),
+                    dest=utils.resolve_stage_name(
+                        regimen_record,
+                        transition_record["target_state_id"],
+                    ),
+                    conditions=transition_record.get("conditions"),
+                    unless=transition_record.get("unless"),
+                ))
+            except exceptions.NotFoundError:
+                logger.debug("No transition source for state. id=%s" % state["id"])
+
+        return models.Regimen(
+            name=regimen_record["name"],
+            stages={
+                stage_record["name"]: models.Stage(
+                    script=stage_record["script"],
+                    script_md5=stage_record["script_md5"],
+                    parameters=stage_record["parameters"],
+                )
+                for stage_record in regimen_record["stages"]
+            },
+            transitions=transitions,
+        )
+
     def get_state(self, regimen_name: str, stage_name: str):
         """Mainly a convenience function because this is repeated sometimes
         """
         regimen = self.get(
             entity_name="regimens",
             filter_property_name="name",
             filter_property_value=regimen_name
```

### Comparing `mtrain-superclient-0.2.0/src/mtrain_superclient/mtrain_lims.py` & `mtrain-superclient-0.3.0/src/mtrain_superclient/mtrain_lims.py`

 * *Files identical despite different names*

### Comparing `mtrain-superclient-0.2.0/setup.py` & `mtrain-superclient-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,29 @@
 packages = \
 ['mtrain_superclient']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['click>=8.0.1', 'pytest>=7.2.1,<8.0.0', 'requests>=2.31.0,<3.0.0']
+['PyGithub>=1.59.0,<2.0.0',
+ 'click>=8.0.1',
+ 'np-config>=0.4.25,<0.5.0',
+ 'pydantic>=2.0,<3.0',
+ 'pytest>=7.2.1,<8.0.0',
+ 'requests>=2.31.0,<3.0.0',
+ 'ruamel.yaml.string>=0.1.1,<0.2.0',
+ 'ruamel.yaml>=0.17.32,<0.18.0']
 
 entry_points = \
 {'console_scripts': ['mtrain-superclient = mtrain_superclient.__main__:main']}
 
 setup_kwargs = {
     'name': 'mtrain-superclient',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Mtrain Superclient',
     'long_description': "# Mtrain Superclient\n\n[![PyPI](https://img.shields.io/pypi/v/mtrain-superclient.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/mtrain-superclient.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/mtrain-superclient)][python version]\n[![License](https://img.shields.io/pypi/l/mtrain-superclient)][license]\n\n[![Read the documentation at https://mtrain-superclient.readthedocs.io/](https://img.shields.io/readthedocs/mtrain-superclient/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/mochic/mtrain-superclient/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/mochic/mtrain-superclient/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/mtrain-superclient/\n[status]: https://pypi.org/project/mtrain-superclient/\n[python version]: https://pypi.org/project/mtrain-superclient\n[read the docs]: https://mtrain-superclient.readthedocs.io/\n[tests]: https://github.com/mochic/mtrain-superclient/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/mochic/mtrain-superclient\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n- TODO\n\n## Requirements\n\n- TODO\n\n## Installation\n\nYou can install _Mtrain Superclient_ via [pip] from [PyPI]:\n\n```console\n$ pip install mtrain-superclient\n```\n\n## Usage\n\nPlease see the [Command-line Reference] for details.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Mtrain Superclient_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/mochic/mtrain-superclient/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/mochic/mtrain-superclient/blob/main/LICENSE\n[contributor guide]: https://github.com/mochic/mtrain-superclient/blob/main/CONTRIBUTING.md\n[command-line reference]: https://mtrain-superclient.readthedocs.io/en/latest/usage.html\n",
     'author': 'Christopher Mochizuki',
     'author_email': 'chrism@alleninstitute.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/mochic/mtrain-superclient',
```

### Comparing `mtrain-superclient-0.2.0/PKG-INFO` & `mtrain-superclient-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: mtrain-superclient
-Version: 0.2.0
+Version: 0.3.0
 Summary: Mtrain Superclient
 Home-page: https://github.com/mochic/mtrain-superclient
 License: MIT
 Author: Christopher Mochizuki
 Author-email: chrism@alleninstitute.org
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: PyGithub (>=1.59.0,<2.0.0)
 Requires-Dist: click (>=8.0.1)
+Requires-Dist: np-config (>=0.4.25,<0.5.0)
+Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: pytest (>=7.2.1,<8.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: ruamel.yaml (>=0.17.32,<0.18.0)
+Requires-Dist: ruamel.yaml.string (>=0.1.1,<0.2.0)
 Project-URL: Changelog, https://github.com/mochic/mtrain-superclient/releases
 Project-URL: Documentation, https://mtrain-superclient.readthedocs.io
 Project-URL: Repository, https://github.com/mochic/mtrain-superclient
 Description-Content-Type: text/markdown
 
 # Mtrain Superclient
```

