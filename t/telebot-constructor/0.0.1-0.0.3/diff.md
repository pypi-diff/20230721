# Comparing `tmp/telebot_constructor-0.0.1.tar.gz` & `tmp/telebot_constructor-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telebot_constructor-0.0.1.tar", max compression
+gzip compressed data, was "telebot_constructor-0.0.3.tar", max compression
```

## Comparing `telebot_constructor-0.0.1.tar` & `telebot_constructor-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0      836 2023-07-21 09:13:07.747436 telebot_constructor-0.0.1/README.md
--rw-r--r--   0        0        0     1109 2023-07-21 09:23:48.474984 telebot_constructor-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 09:08:36.263070 telebot_constructor-0.0.1/telebot_constructor/__init__.py
--rw-r--r--   0        0        0     7101 2023-07-21 09:08:36.263974 telebot_constructor-0.0.1/telebot_constructor/app.py
--rw-r--r--   0        0        0      564 2023-07-21 09:08:36.264100 telebot_constructor-0.0.1/telebot_constructor/construct.py
--rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 telebot_constructor-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      836 2023-07-21 13:20:16.273652 telebot_constructor-0.0.3/README.md
+-rw-r--r--   0        0        0     1330 2023-07-21 13:20:36.745796 telebot_constructor-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 13:20:16.273652 telebot_constructor-0.0.3/telebot_constructor/__init__.py
+-rw-r--r--   0        0        0    11831 2023-07-21 13:20:16.273652 telebot_constructor-0.0.3/telebot_constructor/app.py
+-rw-r--r--   0        0        0       94 2023-07-21 13:20:16.273652 telebot_constructor-0.0.3/telebot_constructor/bot_config.py
+-rw-r--r--   0        0        0      643 2023-07-21 13:20:16.273652 telebot_constructor-0.0.3/telebot_constructor/construct.py
+-rw-r--r--   0        0        0     2718 2023-07-21 13:20:16.273652 telebot_constructor-0.0.3/telebot_constructor/runners.py
+-rw-r--r--   0        0        0     3226 2023-07-21 13:20:35.369787 telebot_constructor-0.0.3/telebot_constructor/static/index.html
+-rw-r--r--   0        0        0     1477 1970-01-01 00:00:00.000000 telebot_constructor-0.0.3/PKG-INFO
```

### Comparing `telebot_constructor-0.0.1/README.md` & `telebot_constructor-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `telebot_constructor-0.0.1/pyproject.toml` & `telebot_constructor-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 [tool.poetry]
 name = "telebot-constructor"
-version = "0.0.1"
-description = "WIP"
+version = "0.0.3"
+description = "No-code Telegram bot constructor"
 authors = ["Igor Vaiman <gosha.vaiman@gmail.com>"]
 license = "GPL-3"
 readme = "README.md"
 packages = [{include = "telebot_constructor"}]
+include = ["telebot_constructor/static/*"]
+
+[tool.poetry.group.dev.dependencies]
+pyproject-flake8 = "^6.0.0.post1"
 
 [tool.poetry-dynamic-versioning]
-enable = true
+enable = false
 vcs = "git"
 dirty = true
 style="semver"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-telebot-components = "^0.8.12"
-
+telebot-components = "^0.8.13"
+pydantic = "^2.0.3"
+aiohttp-swagger = "^1.0.16"
+telebot-against-war = "^0.6.9"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-aiohttp = "1.0.4"
 pytest-asyncio = "^0.18.3"
 python-dotenv = "^0.20.0"
 aioresponses = "0.7.3"
 black = "^22.3.0"
 isort = "^5.10.1"
 pre-commit = "^2.19.0"
 mypy = "^1.4.1"
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-
 [tool.black]
 line-length = 120
 
 [tool.isort]
 profile = 'black'
 
 [tool.pytest.ini_options]
```

### Comparing `telebot_constructor-0.0.1/PKG-INFO` & `telebot_constructor-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: telebot-constructor
-Version: 0.0.1
-Summary: WIP
+Version: 0.0.3
+Summary: No-code Telegram bot constructor
 License: GPL-3
 Author: Igor Vaiman
 Author-email: gosha.vaiman@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: telebot-components (>=0.8.12,<0.9.0)
+Requires-Dist: aiohttp-swagger (>=1.0.16,<2.0.0)
+Requires-Dist: pydantic (>=2.0.3,<3.0.0)
+Requires-Dist: telebot-against-war (>=0.6.9,<0.7.0)
+Requires-Dist: telebot-components (>=0.8.13,<0.9.0)
 Description-Content-Type: text/markdown
 
 # telebot-constructor
 
 Free & open-source Telegram bot constructor with no-code web UI, using as backend [telebot-components](https://github.com/bots-against-war/telebot-components).
 
 ## Development
```

