# Comparing `tmp/dxsp-4.1.0.tar.gz` & `tmp/dxsp-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-4.1.0.tar", max compression
+gzip compressed data, was "dxsp-4.1.1.tar", max compression
```

## Comparing `dxsp-4.1.0.tar` & `dxsp-4.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1064 2023-07-20 14:52:07.399715 dxsp-4.1.0/LICENSE
--rw-r--r--   0        0        0     2857 2023-07-20 14:52:07.399715 dxsp-4.1.0/README.md
--rw-r--r--   0        0        0      158 2023-07-20 14:52:08.227724 dxsp-4.1.0/dxsp/__init__.py
--rw-r--r--   0        0        0      418 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/config.py
--rw-r--r--   0        0        0    12100 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/default_settings.toml
--rw-r--r--   0        0        0     5701 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/main.py
--rw-r--r--   0        0        0      104 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     1864 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0     1037 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0      102 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/utils/__init__.py
--rw-r--r--   0        0        0     4834 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/utils/account_utils.py
--rw-r--r--   0        0        0     6619 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/utils/contract_utils.py
--rw-r--r--   0        0        0     1990 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/utils/explorer_utils.py
--rw-r--r--   0        0        0      363 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/utils/utils.py
--rw-r--r--   0        0        0     4100 2023-07-20 14:52:08.227724 dxsp-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     3706 1970-01-01 00:00:00.000000 dxsp-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-21 17:51:56.437077 dxsp-4.1.1/LICENSE
+-rw-r--r--   0        0        0     2857 2023-07-21 17:51:56.437077 dxsp-4.1.1/README.md
+-rw-r--r--   0        0        0      158 2023-07-21 17:51:56.437077 dxsp-4.1.1/dxsp/__init__.py
+-rw-r--r--   0        0        0      418 2023-07-21 17:51:56.437077 dxsp-4.1.1/dxsp/config.py
+-rw-r--r--   0        0        0    12100 2023-07-21 17:51:56.437077 dxsp-4.1.1/dxsp/default_settings.toml
+-rw-r--r--   0        0        0     5701 2023-07-21 17:51:56.437077 dxsp-4.1.1/dxsp/main.py
+-rw-r--r--   0        0        0      104 2023-07-21 17:51:56.437077 dxsp-4.1.1/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-21 17:51:56.437077 dxsp-4.1.1/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1864 2023-07-21 17:51:56.437077 dxsp-4.1.1/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0     1037 2023-07-21 17:51:56.437077 dxsp-4.1.1/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0      102 2023-07-21 17:51:56.437077 dxsp-4.1.1/dxsp/utils/__init__.py
+-rw-r--r--   0        0        0     4834 2023-07-21 17:51:56.437077 dxsp-4.1.1/dxsp/utils/account_utils.py
+-rw-r--r--   0        0        0     6619 2023-07-21 17:51:56.437077 dxsp-4.1.1/dxsp/utils/contract_utils.py
+-rw-r--r--   0        0        0     1990 2023-07-21 17:51:56.437077 dxsp-4.1.1/dxsp/utils/explorer_utils.py
+-rw-r--r--   0        0        0      363 2023-07-21 17:51:56.437077 dxsp-4.1.1/dxsp/utils/utils.py
+-rw-r--r--   0        0        0     4006 2023-07-21 17:52:00.377044 dxsp-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3706 1970-01-01 00:00:00.000000 dxsp-4.1.1/PKG-INFO
```

### Comparing `dxsp-4.1.0/LICENSE` & `dxsp-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-4.1.0/README.md` & `dxsp-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-4.1.0/dxsp/default_settings.toml` & `dxsp-4.1.1/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-4.1.0/dxsp/main.py` & `dxsp-4.1.1/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.1.0/dxsp/protocols/oneinch.py` & `dxsp-4.1.1/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.1.0/dxsp/protocols/uniswap.py` & `dxsp-4.1.1/dxsp/protocols/uniswap.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.1.0/dxsp/protocols/zerox.py` & `dxsp-4.1.1/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.1.0/dxsp/utils/account_utils.py` & `dxsp-4.1.1/dxsp/utils/account_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.1.0/dxsp/utils/contract_utils.py` & `dxsp-4.1.1/dxsp/utils/contract_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.1.0/dxsp/utils/explorer_utils.py` & `dxsp-4.1.1/dxsp/utils/explorer_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.1.0/pyproject.toml` & `dxsp-4.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dxsp"
-version = "4.1.0"
+version = "4.1.1"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
@@ -41,14 +41,15 @@
   "docs/*",
 ]
 ignore = ["F401"]
 format = "github"
 fixable = ["ALL"]
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.11.1"
 eth_tester = "^0.9.0b2"
 
@@ -63,98 +64,99 @@
 omit = [
     "tests/*",
     "examples/*",
     "docs/*",
     "*/config.py"
 ]
 
+
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.0.0"
 sphinx_bootstrap_theme = "^0.8.1"
 sphinx-autoapi = "^2.1.1"
 sphinx-copybutton= "^0.5.2"
 myst-parser = "^2.0.0"
 sphinx-notfound-page = "^0.8.3"
 sphinxext-remoteliteralinclude = "^0.4.0"
 sphinx-togglebutton = "*"
 
 
+# [tool.semantic_release]
+# version_variable = ["pyproject.toml:version","dxsp/__init__.py:__version__"]
+# branch = "main"
+# upload_to_pypi = true
+# upload_to_release = true
+# build_command = "pip install poetry && poetry build"
+# commit_parser = "semantic_release.history.emoji_parser"
+# use_textual_changelog_sections = true
+# major_emoji = "BREAKING,💥,:boom:"
+# minor_emoji = "feat,🥚,:egg:,🚀,:rocket:,💄,:lipstick:,✨,:sparkles:"
+# patch_emoji = "fix,bump,Update,🎨,:art:,🐛,:bug:,🚑,:ambulance:,⚡,:zap:,🔥,:fire:,🚨,:rotating_light:,♻️,:recycle:,🔧,:wrench:,⬆️,:arrow_up:,🩹,:adhesive_bandage:,👷,:construction_worker:,📝,:memo:,🔒,:lock:,👽,:alien:,💬,:speech_balloon:,🥅,:goal_net:,✅,:white_check_mark:,🐳,:whale:,🙈,:see_no_evil:,⚗️,:alembic:,🧐,:monocle_face:,🔇,:mute:,🔊:volume:"
+
 [tool.semantic_release]
-version_variable = ["pyproject.toml:version","dxsp/__init__.py:__version__"]
-branch = "main"
-upload_to_pypi = true
-upload_to_release = true
+tag_format = "v{version}"
+commit_parser = "emoji"
 build_command = "pip install poetry && poetry build"
-commit_parser = "semantic_release.history.emoji_parser"
-use_textual_changelog_sections = true
-major_emoji = "BREAKING,💥,:boom:"
-minor_emoji = "feat,🥚,:egg:,🚀,:rocket:,💄,:lipstick:,✨,:sparkles:"
-patch_emoji = "fix,bump,Update,🎨,:art:,🐛,:bug:,🚑,:ambulance:,⚡,:zap:,🔥,:fire:,🚨,:rotating_light:,♻️,:recycle:,🔧,:wrench:,⬆️,:arrow_up:,🩹,:adhesive_bandage:,👷,:construction_worker:,📝,:memo:,🔒,:lock:,👽,:alien:,💬,:speech_balloon:,🥅,:goal_net:,✅,:white_check_mark:,🐳,:whale:,🙈,:see_no_evil:,⚗️,:alembic:,🧐,:monocle_face:,🔇,:mute:,🔊:volume:"
+version_variable = [
+    "dxsp/__init__.py:__version__",
+    # "docs/conf.py:version",
+]
+version_toml = [
+   "pyproject.toml:tool.poetry.version",
+]
 
-# [tool.semantic_release]
-# tag_format = "v{version}"
-# commit_parser = "emoji"
-# build_command = "pip install poetry && poetry build"
-# version_variable = [
-#     "dxsp/__init__.py:__version__",
-#     # "docs/conf.py:version",
-# ]
-# version_toml = [
-#    "pyproject.toml:tool.poetry.version",
-# ]
-
-# [tool.semantic_release.commit_parser_options]
-# major_tags = [
-#     "BREAKING",
-#     "💥",
-#     ":boom:",
-#   ]
-# minor_tags = ["feat",
-#     "🥚",":egg:",
-#     "🚀",":rocket:",
-#     "💄",":lipstick:",
-#     "✨",":sparkles:",
-# ]
-
-# patch_tags = ["fix","bump","Update",
-#     "🎨",":art:",
-#     "🐛",":bug:",
-#     "🚑",":ambulance:",
-#     "⚡",":zap:",
-#     "🔥",":fire:",
-#     "🚨",":rotating_light:",
-#     "♻️",":recycle:",
-#     "🔧",":wrench:",
-#     "⬆️",":arrow_up:",
-#     "🩹",":adhesive_bandage:",
-#     "👷",":construction_worker:",
-#     "📝",":memo:",
-#     "🔒",":lock:",
-#     "👽",":alien:",
-#     "💬",":speech_balloon:",
-#     "🥅",":goal_net:",
-#     "✅",":white_check_mark:",
-#     "🐳",":whale:",
-#     "🙈",":see_no_evil:",
-#     "⚗️",":alembic:",
-#     "🧐",":monocle_face:",
-#     "🔇",":mute:",
-#     "🔊",":volume:",
-# ]
-
-# [tool.semantic_release.changelog]
-# # template_dir = "templates"
-# changelog_file = "CHANGELOG.md"
-# exclude_commit_patterns = []
-
-# [tool.semantic_release.branches.main]
-# match = "(main|master)"
-# prerelease_token = "rc"
-# prerelease = false
-
-# [tool.semantic_release.publish]
-# dist_glob_patterns = ["dist/*"]
-# upload_to_vcs_release = true
+[tool.semantic_release.commit_parser_options]
+major_tags = [
+    "BREAKING",
+    "💥",
+    ":boom:",
+  ]
+minor_tags = ["feat",
+    "🥚",":egg:",
+    "🚀",":rocket:",
+    "💄",":lipstick:",
+    "✨",":sparkles:",
+]
+
+patch_tags = ["fix","bump","Update",
+    "🎨",":art:",
+    "🐛",":bug:",
+    "🚑",":ambulance:",
+    "⚡",":zap:",
+    "🔥",":fire:",
+    "🚨",":rotating_light:",
+    "♻️",":recycle:",
+    "🔧",":wrench:",
+    "⬆️",":arrow_up:",
+    "🩹",":adhesive_bandage:",
+    "👷",":construction_worker:",
+    "📝",":memo:",
+    "🔒",":lock:",
+    "👽",":alien:",
+    "💬",":speech_balloon:",
+    "🥅",":goal_net:",
+    "✅",":white_check_mark:",
+    "🐳",":whale:",
+    "🙈",":see_no_evil:",
+    "⚗️",":alembic:",
+    "🧐",":monocle_face:",
+    "🔇",":mute:",
+    "🔊",":volume:",
+]
+
+[tool.semantic_release.changelog]
+# template_dir = "templates"
+changelog_file = "CHANGELOG.md"
+exclude_commit_patterns = []
+
+[tool.semantic_release.branches.main]
+match = "(main|master)"
+prerelease_token = "rc"
+prerelease = false
+
+[tool.semantic_release.publish]
+dist_glob_patterns = ["dist/*"]
+upload_to_vcs_release = true
```

### Comparing `dxsp-4.1.0/PKG-INFO` & `dxsp-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 4.1.0
+Version: 4.1.1
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dxsp Version: 4.1.0 Summary: DXSP (DeX SwaP), A
+Metadata-Version: 2.1 Name: dxsp Version: 4.1.1 Summary: DXSP (DeX SwaP), A
 defi swap helper package. Swap made easy. License: MIT Author: mraniki Author-
 email: 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: pycoingecko (>=3.1.0,<4.0.0) Requires-Dist:
 uniswap-python (>=0.7.0,<0.8.0) Requires-Dist: web3 (>=6.4.0,<7.0.0) Project-
```

