# Comparing `tmp/rasa_sdk-3.7.0b1.tar.gz` & `tmp/rasa_sdk-3.8.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasa_sdk-3.7.0b1.tar", max compression
+gzip compressed data, was "rasa_sdk-3.8.0a1.tar", max compression
```

## Comparing `rasa_sdk-3.7.0b1.tar` & `rasa_sdk-3.8.0a1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11553 2023-06-28 07:37:37.096332 rasa_sdk-3.7.0b1/LICENSE.txt
--rw-r--r--   0        0        0     5282 2023-06-28 07:37:37.096332 rasa_sdk-3.7.0b1/README.md
--rw-r--r--   0        0        0     3124 2023-06-28 07:37:37.096332 rasa_sdk-3.7.0b1/pyproject.toml
--rw-r--r--   0        0        0      420 2023-06-28 07:37:37.096332 rasa_sdk-3.7.0b1/rasa_sdk/__init__.py
--rw-r--r--   0        0        0      947 2023-06-28 07:37:37.096332 rasa_sdk-3.7.0b1/rasa_sdk/__main__.py
--rw-r--r--   0        0        0        0 2023-06-28 07:37:37.096332 rasa_sdk-3.7.0b1/rasa_sdk/cli/__init__.py
--rw-r--r--   0        0        0     1528 2023-06-28 07:37:37.096332 rasa_sdk-3.7.0b1/rasa_sdk/cli/arguments.py
--rw-r--r--   0        0        0      399 2023-06-28 07:37:37.096332 rasa_sdk-3.7.0b1/rasa_sdk/constants.py
--rw-r--r--   0        0        0     5727 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/endpoint.py
--rw-r--r--   0        0        0     6459 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/events.py
--rw-r--r--   0        0        0     1905 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/exceptions.py
--rw-r--r--   0        0        0    15183 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/executor.py
--rw-r--r--   0        0        0    11265 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/forms.py
--rw-r--r--   0        0        0    12929 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/interfaces.py
--rw-r--r--   0        0        0        0 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/knowledge_base/__init__.py
--rw-r--r--   0        0        0    10413 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/knowledge_base/actions.py
--rw-r--r--   0        0        0     8091 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/knowledge_base/storage.py
--rw-r--r--   0        0        0     7266 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/knowledge_base/utils.py
--rw-r--r--   0        0        0     1039 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/plugin.py
--rw-r--r--   0        0        0     7066 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/slots.py
--rw-r--r--   0        0        0     1683 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/types.py
--rw-r--r--   0        0        0    11308 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/utils.py
--rw-r--r--   0        0        0      118 2023-06-28 07:37:37.100332 rasa_sdk-3.7.0b1/rasa_sdk/version.py
--rw-r--r--   0        0        0     6796 1970-01-01 00:00:00.000000 rasa_sdk-3.7.0b1/PKG-INFO
+-rw-r--r--   0        0        0    11553 2023-07-21 08:05:53.769565 rasa_sdk-3.8.0a1/LICENSE.txt
+-rw-r--r--   0        0        0     5282 2023-07-21 08:05:53.769565 rasa_sdk-3.8.0a1/README.md
+-rw-r--r--   0        0        0     3124 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/pyproject.toml
+-rw-r--r--   0        0        0      420 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/__init__.py
+-rw-r--r--   0        0        0      947 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/cli/__init__.py
+-rw-r--r--   0        0        0     1528 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/cli/arguments.py
+-rw-r--r--   0        0        0      399 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/constants.py
+-rw-r--r--   0        0        0     5727 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/endpoint.py
+-rw-r--r--   0        0        0     6459 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/events.py
+-rw-r--r--   0        0        0     1905 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/exceptions.py
+-rw-r--r--   0        0        0    15183 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/executor.py
+-rw-r--r--   0        0        0    11265 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/forms.py
+-rw-r--r--   0        0        0    12929 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/interfaces.py
+-rw-r--r--   0        0        0        0 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/knowledge_base/__init__.py
+-rw-r--r--   0        0        0    10413 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/knowledge_base/actions.py
+-rw-r--r--   0        0        0     8091 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/knowledge_base/storage.py
+-rw-r--r--   0        0        0     7266 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/knowledge_base/utils.py
+-rw-r--r--   0        0        0     1035 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/plugin.py
+-rw-r--r--   0        0        0     7066 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/slots.py
+-rw-r--r--   0        0        0     1683 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/types.py
+-rw-r--r--   0        0        0    11253 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/utils.py
+-rw-r--r--   0        0        0      118 2023-07-21 08:05:53.773565 rasa_sdk-3.8.0a1/rasa_sdk/version.py
+-rw-r--r--   0        0        0     6796 1970-01-01 00:00:00.000000 rasa_sdk-3.8.0a1/PKG-INFO
```

### Comparing `rasa_sdk-3.7.0b1/LICENSE.txt` & `rasa_sdk-3.8.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.7.0b1/README.md` & `rasa_sdk-3.8.0a1/README.md`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.7.0b1/pyproject.toml` & `rasa_sdk-3.8.0a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.black]
 line-length = 88
 target-version = [ "py37", "py38", "py39", "py310",]
 exclude = "((.eggs | .git | .mypy_cache | .pytest_cache | build | dist))"
 
 [tool.poetry]
 name = "rasa-sdk"
-version = "3.7.0b1"
+version = "3.8.0a1"
 description = "Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants"
 authors = [ "Rasa Technologies GmbH <hi@rasa.com>",]
 maintainers = [ "Tom Bocklisch <tom@rasa.com>",]
 homepage = "https://rasa.com"
 repository = "https://github.com/rasahq/rasa-sdk"
 documentation = "https://rasa.com/docs"
 classifiers = [ "Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "License :: OSI Approved :: Apache Software License", "Topic :: Software Development :: Libraries",]
@@ -77,33 +77,33 @@
 python = ">=3.8,<3.11"
 coloredlogs = ">=10,<16"
 sanic = "^21.12.0"
 typing-extensions = ">=4.1.1,<5.0.0"
 Sanic-Cors = "^2.0.0"
 prompt-toolkit = "^3.0,<3.0.29"
 "ruamel.yaml" = ">=0.16.5,<0.18.0"
-websockets = ">=10.0,<11.0"
+websockets = ">=10.0,<12.0"
 pluggy = "^1.0.0"
 
 [tool.poetry.dev-dependencies]
-pytest-cov = "^4.0.0"
+pytest-cov = "^4.1.0"
 coveralls = "^3.0.1"
-pytest = "^7.3.1"
+pytest = "^7.4.0"
 black = "22.12.0"
 questionary = ">=1.5.1,<1.11.0"
-towncrier = "^22.8.0"
+towncrier = "^23.6.0"
 toml = "^0.10.0"
 pep440-version-utils = "^0.3.0"
 semantic_version = "^2.8.5"
-mypy = "^1.3"
+mypy = "^1.4"
 sanic-testing = "^22.3.0, <22.9.0"
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.pytest.ini_options]
 python_functions = "test_"
 asyncio_mode = "auto"
 
 [tool.poetry.group.dev.dependencies]
-ruff = ">=0.0.256,<0.0.268"
+ruff = ">=0.0.256,<0.0.278"
 pytest-asyncio = "^0.21.0"
```

### Comparing `rasa_sdk-3.7.0b1/rasa_sdk/__main__.py` & `rasa_sdk-3.8.0a1/rasa_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.7.0b1/rasa_sdk/cli/arguments.py` & `rasa_sdk-3.8.0a1/rasa_sdk/cli/arguments.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.7.0b1/rasa_sdk/endpoint.py` & `rasa_sdk-3.8.0a1/rasa_sdk/endpoint.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.7.0b1/rasa_sdk/events.py` & `rasa_sdk-3.8.0a1/rasa_sdk/events.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.7.0b1/rasa_sdk/exceptions.py` & `rasa_sdk-3.8.0a1/rasa_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.7.0b1/rasa_sdk/executor.py` & `rasa_sdk-3.8.0a1/rasa_sdk/executor.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.7.0b1/rasa_sdk/forms.py` & `rasa_sdk-3.8.0a1/rasa_sdk/forms.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.7.0b1/rasa_sdk/interfaces.py` & `rasa_sdk-3.8.0a1/rasa_sdk/interfaces.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.7.0b1/rasa_sdk/knowledge_base/actions.py` & `rasa_sdk-3.8.0a1/rasa_sdk/knowledge_base/actions.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.7.0b1/rasa_sdk/knowledge_base/storage.py` & `rasa_sdk-3.8.0a1/rasa_sdk/knowledge_base/storage.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.7.0b1/rasa_sdk/knowledge_base/utils.py` & `rasa_sdk-3.8.0a1/rasa_sdk/knowledge_base/utils.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.7.0b1/rasa_sdk/plugin.py` & `rasa_sdk-3.8.0a1/rasa_sdk/plugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,14 +23,14 @@
     try:
         # rasa_sdk_plugin is a custom package
         # which extends existing functionality on rasa action server via plugins
         import rasa_sdk_plugins
 
         rasa_sdk_plugins.init_hooks(manager)
     except ModuleNotFoundError as e:
-        logger.info("No plugins found", exc_info=e)
+        logger.debug("No plugins found: %s", e)
         pass
 
 
 @hookspec
 def attach_sanic_app_extensions(app: Sanic) -> None:
     """Hook specification for attaching sanic listeners, routes and middlewares."""
```

### Comparing `rasa_sdk-3.7.0b1/rasa_sdk/slots.py` & `rasa_sdk-3.8.0a1/rasa_sdk/slots.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.7.0b1/rasa_sdk/types.py` & `rasa_sdk-3.8.0a1/rasa_sdk/types.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.7.0b1/rasa_sdk/utils.py` & `rasa_sdk-3.8.0a1/rasa_sdk/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 
 class Button(dict):
     pass
 
 
 def all_subclasses(cls: Any) -> List[Any]:
     """Returns all known (imported) subclasses of a class."""
-
     return cls.__subclasses__() + [
         g for s in cls.__subclasses__() for g in all_subclasses(s)
     ]
 
 
 def add_logging_level_option_arguments(parser):
     """Add options to an argument parser to configure logging levels."""
@@ -229,17 +228,19 @@
 
 def check_version_compatibility(rasa_version: Optional[Text]) -> None:
     """Check if the version of rasa and rasa_sdk are compatible.
 
     The version check relies on the version string being formatted as
     'x.y.z' and compares whether the numbers x and y are the same for both
     rasa and rasa_sdk.
+
     Args:
         rasa_version - A string containing the version of rasa that
         is making the call to the action server.
+
     Raises:
         Warning - The version of rasa version unknown or not compatible with
         this version of rasa_sdk.
     """
     # Check for versions of Rasa that are too old to report their version number
     if rasa_version is None:
         warnings.warn(
@@ -333,16 +334,16 @@
             content.encode("utf-8")
             .decode("raw_unicode_escape")
             .encode("utf-16", "surrogatepass")
             .decode("utf-16")
         )
 
     yaml_parser = yaml.YAML(typ=reader_type)
-    yaml_parser.version = YAML_VERSION  # type: ignore[assignment]
-    yaml_parser.preserve_quotes = True  # type: ignore[assignment]
+    yaml_parser.version = YAML_VERSION
+    yaml_parser.preserve_quotes = True
 
     return yaml_parser.load(content) or {}
 
 
 def _is_ascii(text: Text) -> bool:
     return all(ord(character) < 128 for character in text)
```

### Comparing `rasa_sdk-3.7.0b1/PKG-INFO` & `rasa_sdk-3.8.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasa-sdk
-Version: 3.7.0b1
+Version: 3.8.0a1
 Summary: Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants
 Home-page: https://rasa.com
 License: Apache-2.0
 Keywords: nlp,machine-learning,machine-learning-library,bot,bots,botkit,rasa conversational-agents,conversational-ai,chatbot,chatbot-framework,bot-framework
 Author: Rasa Technologies GmbH
 Author-email: hi@rasa.com
 Maintainer: Tom Bocklisch
@@ -21,15 +21,15 @@
 Requires-Dist: Sanic-Cors (>=2.0.0,<3.0.0)
 Requires-Dist: coloredlogs (>=10,<16)
 Requires-Dist: pluggy (>=1.0.0,<2.0.0)
 Requires-Dist: prompt-toolkit (>=3.0,<3.0.29)
 Requires-Dist: ruamel.yaml (>=0.16.5,<0.18.0)
 Requires-Dist: sanic (>=21.12.0,<22.0.0)
 Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
-Requires-Dist: websockets (>=10.0,<11.0)
+Requires-Dist: websockets (>=10.0,<12.0)
 Project-URL: Documentation, https://rasa.com/docs
 Project-URL: Repository, https://github.com/rasahq/rasa-sdk
 Description-Content-Type: text/markdown
 
 # Rasa Python-SDK
 [![Join the chat on Rasa Community Forum](https://img.shields.io/badge/forum-join%20discussions-brightgreen.svg)](https://forum.rasa.com/?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 [![Build Status](https://github.com/RasaHQ/rasa-sdk/workflows/Continous%20Integration/badge.svg?event=push)](https://github.com/RasaHQ/rasa-sdk/actions/runs/)
```

