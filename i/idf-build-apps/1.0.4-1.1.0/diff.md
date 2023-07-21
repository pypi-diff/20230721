# Comparing `tmp/idf_build_apps-1.0.4.tar.gz` & `tmp/idf_build_apps-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idf_build_apps-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "idf_build_apps-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `idf_build_apps-1.0.4.tar` & `idf_build_apps-1.1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      351 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.editorconfig
--rw-r--r--   0        0        0      123 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.git-blame-ignore-revs
--rw-r--r--   0        0        0       25 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.gitattributes
--rw-r--r--   0        0        0      513 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.github/dependabot.yml
--rw-r--r--   0        0        0      253 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.github/workflows/check-pre-commit.yml
--rw-r--r--   0        0        0      675 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.github/workflows/issue_comment.yml
--rw-r--r--   0        0        0      620 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.github/workflows/new_issues.yml
--rw-r--r--   0        0        0      796 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.github/workflows/new_prs.yml
--rw-r--r--   0        0        0      438 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      521 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.github/workflows/test-build-docs.yml
--rw-r--r--   0        0        0     3870 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.github/workflows/test-build-idf-apps.yml
--rw-r--r--   0        0        0     3076 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.gitignore
--rw-r--r--   0        0        0     1077 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      383 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.readthedocs.yml
--rw-r--r--   0        0        0     5702 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/CHANGELOG.md
--rw-r--r--   0        0        0     1882 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/CONTRIBUTING.md
--rw-r--r--   0        0        0    11358 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/LICENSE
--rw-r--r--   0        0        0     3843 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/README.md
--rw-r--r--   0        0        0       33 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/CHANGELOG.md
--rw-r--r--   0        0        0       36 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0      634 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/Makefile
--rw-r--r--   0        0        0     6947 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/_static/espressif-logo.svg
--rw-r--r--   0        0        0      942 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/_static/theme_overrides.css
--rw-r--r--   0        0        0      119 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/_templates/layout.html
--rw-r--r--   0        0        0      490 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/api.rst
--rw-r--r--   0        0        0     1449 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/conf.py
--rw-r--r--   0        0        0     2652 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/config_file.md
--rw-r--r--   0        0        0    10473 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/find_build.md
--rw-r--r--   0        0        0      474 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/index.rst
--rw-r--r--   0        0        0     5894 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/manifest.md
--rw-r--r--   0        0        0      481 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/idf_build_apps/__init__.py
--rw-r--r--   0        0        0      182 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/idf_build_apps/__main__.py
--rw-r--r--   0        0        0    27235 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/idf_build_apps/app.py
--rw-r--r--   0        0        0     2794 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/idf_build_apps/config.py
--rw-r--r--   0        0        0     2182 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/idf_build_apps/constants.py
--rw-r--r--   0        0        0     6328 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/idf_build_apps/finder.py
--rw-r--r--   0        0        0     2220 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/idf_build_apps/log.py
--rw-r--r--   0        0        0    30514 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/idf_build_apps/main.py
--rw-r--r--   0        0        0      133 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/idf_build_apps/manifest/__init__.py
--rw-r--r--   0        0        0     6368 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/idf_build_apps/manifest/if_parser.py
--rw-r--r--   0        0        0     6535 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/idf_build_apps/manifest/manifest.py
--rw-r--r--   0        0        0     3423 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/idf_build_apps/manifest/soc_header.py
--rw-r--r--   0        0        0     7081 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/idf_build_apps/utils.py
--rw-r--r--   0        0        0      101 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/license_header.txt
--rw-r--r--   0        0        0     2060 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1221 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/tests/conftest.py
--rw-r--r--   0        0        0     3347 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/tests/test_build.py
--rw-r--r--   0        0        0    18222 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/tests/test_finder.py
--rw-r--r--   0        0        0     1568 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/tests/test_manifest.py
--rw-r--r--   0        0        0     3710 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/tests/test_utils.py
--rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 idf_build_apps-1.0.4/setup.py
--rw-r--r--   0        0        0     5540 1970-01-01 00:00:00.000000 idf_build_apps-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      351 2023-07-21 08:38:46.199686 idf_build_apps-1.1.0/.editorconfig
+-rw-r--r--   0        0        0      123 2023-07-21 08:38:46.199686 idf_build_apps-1.1.0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0       25 2023-07-21 08:38:46.199686 idf_build_apps-1.1.0/.gitattributes
+-rw-r--r--   0        0        0      513 2023-07-21 08:38:46.199686 idf_build_apps-1.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      253 2023-07-21 08:38:46.199686 idf_build_apps-1.1.0/.github/workflows/check-pre-commit.yml
+-rw-r--r--   0        0        0      675 2023-07-21 08:38:46.199686 idf_build_apps-1.1.0/.github/workflows/issue_comment.yml
+-rw-r--r--   0        0        0      620 2023-07-21 08:38:46.199686 idf_build_apps-1.1.0/.github/workflows/new_issues.yml
+-rw-r--r--   0        0        0      796 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/.github/workflows/new_prs.yml
+-rw-r--r--   0        0        0      438 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      521 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/.github/workflows/test-build-docs.yml
+-rw-r--r--   0        0        0     3870 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/.github/workflows/test-build-idf-apps.yml
+-rw-r--r--   0        0        0     3076 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1077 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      383 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/.readthedocs.yml
+-rw-r--r--   0        0        0     5793 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1882 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11358 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3843 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/README.md
+-rw-r--r--   0        0        0       33 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0       36 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0      634 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/Makefile
+-rw-r--r--   0        0        0     6947 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/_static/espressif-logo.svg
+-rw-r--r--   0        0        0      942 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/_static/theme_overrides.css
+-rw-r--r--   0        0        0      119 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/_templates/layout.html
+-rw-r--r--   0        0        0      490 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/api.rst
+-rw-r--r--   0        0        0     1449 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/conf.py
+-rw-r--r--   0        0        0     2652 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/config_file.md
+-rw-r--r--   0        0        0    10473 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/find_build.md
+-rw-r--r--   0        0        0      474 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/index.rst
+-rw-r--r--   0        0        0     5962 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/manifest.md
+-rw-r--r--   0        0        0      481 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/__init__.py
+-rw-r--r--   0        0        0      182 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/__main__.py
+-rw-r--r--   0        0        0    27235 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/app.py
+-rw-r--r--   0        0        0     2794 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/config.py
+-rw-r--r--   0        0        0     2182 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/constants.py
+-rw-r--r--   0        0        0     6328 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/finder.py
+-rw-r--r--   0        0        0     2220 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/log.py
+-rw-r--r--   0        0        0    30514 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/main.py
+-rw-r--r--   0        0        0      133 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/manifest/__init__.py
+-rw-r--r--   0        0        0     6368 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/manifest/if_parser.py
+-rw-r--r--   0        0        0     6535 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/manifest/manifest.py
+-rw-r--r--   0        0        0     3888 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/manifest/soc_header.py
+-rw-r--r--   0        0        0     7081 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/utils.py
+-rw-r--r--   0        0        0      101 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/license_header.txt
+-rw-r--r--   0        0        0     2060 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1221 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     3347 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/tests/test_build.py
+-rw-r--r--   0        0        0    18222 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/tests/test_finder.py
+-rw-r--r--   0        0        0     1568 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/tests/test_manifest.py
+-rw-r--r--   0        0        0     3710 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 idf_build_apps-1.1.0/setup.py
+-rw-r--r--   0        0        0     5540 1970-01-01 00:00:00.000000 idf_build_apps-1.1.0/PKG-INFO
```

### Comparing `idf_build_apps-1.0.4/.github/dependabot.yml` & `idf_build_apps-1.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/.github/workflows/issue_comment.yml` & `idf_build_apps-1.1.0/.github/workflows/issue_comment.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/.github/workflows/new_issues.yml` & `idf_build_apps-1.1.0/.github/workflows/new_issues.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/.github/workflows/new_prs.yml` & `idf_build_apps-1.1.0/.github/workflows/new_prs.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/.github/workflows/test-build-docs.yml` & `idf_build_apps-1.1.0/.github/workflows/test-build-docs.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/.github/workflows/test-build-idf-apps.yml` & `idf_build_apps-1.1.0/.github/workflows/test-build-idf-apps.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/.gitignore` & `idf_build_apps-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/.pre-commit-config.yaml` & `idf_build_apps-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/CHANGELOG.md` & `idf_build_apps-1.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## v1.1.0 (2023-07-21)
+
+### Feat
+
+- support esp_rom caps as keywords in the manifest file
+
 ## v1.0.4 (2023-07-20)
 
 ### Fix
 
 - stop overriding supported targets with sdkconfig file defined one for disabled app
 
 ## v1.0.3 (2023-07-19)
```

### Comparing `idf_build_apps-1.0.4/CONTRIBUTING.md` & `idf_build_apps-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/LICENSE` & `idf_build_apps-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/README.md` & `idf_build_apps-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/docs/Makefile` & `idf_build_apps-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/docs/_static/espressif-logo.svg` & `idf_build_apps-1.1.0/docs/_static/espressif-logo.svg`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/docs/_static/theme_overrides.css` & `idf_build_apps-1.1.0/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/docs/conf.py` & `idf_build_apps-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/docs/config_file.md` & `idf_build_apps-1.1.0/docs/config_file.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/docs/find_build.md` & `idf_build_apps-1.1.0/docs/find_build.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/docs/manifest.md` & `idf_build_apps-1.1.0/docs/manifest.md`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ```
 
 ## `if` Clauses
 
 ### Operands
 
 - Capitalized Words
-  - Variables start with `SOC_`. The value would be parsed from `IDF_PATH/components/soc/[TARGET]/include/soc/*_caps.h`
+  - Variables defined in `IDF_PATH/components/soc/[TARGET]/include/soc/*_caps.h` or in `IDF_PATH/components/esp_rom/[TARGET]/*_caps.h`. e.g., `SOC_WIFI_SUPPORTED`, `ESP_ROM_HAS_SPI_FLASH`
   - `IDF_TARGET`
   - `IDF_VERSION` (IDF_VERSION_MAJOR.IDF_VERSION_MINOR.IDF_VERSION_PATCH. e.g., 5.2.0. Will convert to Version object to do a version comparison instead of a string comparison)
   - `IDF_VERSION_MAJOR`
   - `IDF_VERSION_MINOR`
   - `IDF_VERSION_PATCH`
   - `INCLUDE_DEFAULT` (The default value of officially supported targets is 1, otherwise is 0)
   - `CONFIG_NAME` (config name defined in [](project:#config-rules))
```

### Comparing `idf_build_apps-1.0.4/idf_build_apps/app.py` & `idf_build_apps-1.1.0/idf_build_apps/app.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/idf_build_apps/config.py` & `idf_build_apps-1.1.0/idf_build_apps/config.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/idf_build_apps/constants.py` & `idf_build_apps-1.1.0/idf_build_apps/constants.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/idf_build_apps/finder.py` & `idf_build_apps-1.1.0/idf_build_apps/finder.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/idf_build_apps/log.py` & `idf_build_apps-1.1.0/idf_build_apps/log.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/idf_build_apps/main.py` & `idf_build_apps-1.1.0/idf_build_apps/main.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/idf_build_apps/manifest/if_parser.py` & `idf_build_apps-1.1.0/idf_build_apps/manifest/if_parser.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/idf_build_apps/manifest/manifest.py` & `idf_build_apps-1.1.0/idf_build_apps/manifest/manifest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/idf_build_apps/manifest/soc_header.py` & `idf_build_apps-1.1.0/idf_build_apps/manifest/soc_header.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     QuotedString,
     Word,
     alphas,
     hexnums,
     nums,
 )
 
+from .. import (
+    LOGGER,
+)
 from ..constants import (
     ALL_TARGETS,
     IDF_PATH,
 )
 
 # Group for parsing literal suffix of a numbers, e.g. 100UL
 _literal_symbol = Group(CaselessLiteral('L') | CaselessLiteral('U'))
@@ -64,50 +67,63 @@
 def parse_define(define_line):  # type: (str) -> ParseResults
     res = _define_expr.parseString(define_line)
 
     return res
 
 
 class SocHeader(dict):
+    CAPS_HEADER_FILEPATTERN = '*_caps.h'
+
     def __init__(self, target):  # type: (str) -> None
         if target != 'linux':
             soc_header_dict = self._parse_soc_header(target)
         else:
             soc_header_dict = {}
 
         super(SocHeader, self).__init__(**soc_header_dict)
 
     @staticmethod
-    def _parse_soc_header(target):  # type: (str) -> dict[str, any]
-        soc_headers_dir_candidates = [
-            # other branches
-            IDF_PATH / 'components' / 'soc' / target / 'include' / 'soc',
-            # release/v4.2
-            IDF_PATH / 'components' / 'soc' / 'soc' / target / 'include' / 'soc',
-        ]
-
-        # get the soc_headers_dir
-        soc_headers_dir = None
-        for d in soc_headers_dir_candidates:
+    def _get_dir_from_candidates(candidates):  # type: (list[Path]) -> Path | None
+        for d in candidates:
             if not d.is_dir():
-                logging.debug('No soc header files folder: %s', d.absolute())
+                logging.debug('folder "%s" not found. Skipping...', d.absolute())
             else:
-                soc_headers_dir = d
-                break
+                return d
+
+        return None
 
-        if not soc_headers_dir:
-            return {}
+    @classmethod
+    def _parse_soc_header(cls, target):  # type: (str) -> dict[str, any]
+        soc_headers_dir = cls._get_dir_from_candidates(
+            [
+                # other branches
+                IDF_PATH / 'components' / 'soc' / target / 'include' / 'soc',
+                # release/v4.2
+                IDF_PATH / 'components' / 'soc' / 'soc' / target / 'include' / 'soc',
+            ]
+        )
+        esp_rom_headers_dir = cls._get_dir_from_candidates(
+            [
+                IDF_PATH / 'components' / 'esp_rom' / target,
+            ]
+        )
+
+        header_files = []
+        if soc_headers_dir:
+            header_files += list(soc_headers_dir.glob(cls.CAPS_HEADER_FILEPATTERN))
+        if esp_rom_headers_dir:
+            header_files += list(esp_rom_headers_dir.glob(cls.CAPS_HEADER_FILEPATTERN))
 
         output_dict = {}
-        for soc_header_file in soc_headers_dir.glob('*_caps.h'):
-            for line in get_defines(soc_header_file):
+        for f in header_files:
+            for line in get_defines(f):
                 try:
                     res = parse_define(line)
                 except ParseException:
-                    logging.debug('Failed to parse: %s', line)
+                    LOGGER.debug('Failed to parse: %s', line)
                     continue
 
                 if 'str_value' in res:
                     output_dict[res.name] = res.str_value
                 elif 'int_value' in res:
                     output_dict[res.name] = int(res.int_value)
                 elif 'hex_value' in res:
```

### Comparing `idf_build_apps-1.0.4/idf_build_apps/utils.py` & `idf_build_apps-1.1.0/idf_build_apps/utils.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/pyproject.toml` & `idf_build_apps-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 changelog = "https://github.com/espressif/idf-build-apps/blob/master/CHANGELOG.md"
 
 [project.scripts]
 idf-build-apps = "idf_build_apps:main.main"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.4"
+version = "1.1.0"
 tag_format = "v$version"
 version_files = [
     "idf_build_apps/__init__.py",
 ]
 
 [tool.pytest.ini_options]
 addopts = "-s --log-cli-level DEBUG"
```

### Comparing `idf_build_apps-1.0.4/tests/conftest.py` & `idf_build_apps-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/tests/test_build.py` & `idf_build_apps-1.1.0/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/tests/test_finder.py` & `idf_build_apps-1.1.0/tests/test_finder.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/tests/test_manifest.py` & `idf_build_apps-1.1.0/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/tests/test_utils.py` & `idf_build_apps-1.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.4/setup.py` & `idf_build_apps-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
          'sphinxcontrib-mermaid'],
  'test': ['pytest', 'pytest-cov']}
 
 entry_points = \
 {'console_scripts': ['idf-build-apps = idf_build_apps:main.main']}
 
 setup(name='idf-build-apps',
-      version='1.0.4',
+      version='1.1.0',
       description='Tools for building ESP-IDF related apps.',
       author=None,
       author_email='Fu Hanxi <fuhanxi@espressif.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `idf_build_apps-1.0.4/PKG-INFO` & `idf_build_apps-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-build-apps
-Version: 1.0.4
+Version: 1.1.0
 Summary: Tools for building ESP-IDF related apps.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
```

