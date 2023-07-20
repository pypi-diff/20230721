# Comparing `tmp/pollination-dragonfly-energy-0.2.7.tar.gz` & `tmp/pollination-dragonfly-energy-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-dragonfly-energy-0.2.7.tar", last modified: Wed Feb  2 16:20:09 2022, max compression
+gzip compressed data, was "dist/pollination-dragonfly-energy-0.2.8.tar", last modified: Thu Jul 20 22:52:15 2023, max compression
```

## Comparing `pollination-dragonfly-energy-0.2.7.tar` & `pollination-dragonfly-energy-0.2.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 16:20:09.000000 pollination-dragonfly-energy-0.2.7/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 16:20:09.000000 pollination-dragonfly-energy-0.2.7/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-02-02 16:19:08.000000 pollination-dragonfly-energy-0.2.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 16:20:09.000000 pollination-dragonfly-energy-0.2.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3352 2022-02-02 16:19:08.000000 pollination-dragonfly-energy-0.2.7/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1018 2022-02-02 16:19:08.000000 pollination-dragonfly-energy-0.2.7/.github/workflows/dependency-release.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-02-02 16:19:08.000000 pollination-dragonfly-energy-0.2.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-02-02 16:19:08.000000 pollination-dragonfly-energy-0.2.7/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (121)     5748 2022-02-02 16:19:08.000000 pollination-dragonfly-energy-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-02-02 16:20:09.000000 pollination-dragonfly-energy-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-02-02 16:19:08.000000 pollination-dragonfly-energy-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-02-02 16:19:08.000000 pollination-dragonfly-energy-0.2.7/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-02-02 16:19:08.000000 pollination-dragonfly-energy-0.2.7/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 16:20:09.000000 pollination-dragonfly-energy-0.2.7/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 16:20:09.000000 pollination-dragonfly-energy-0.2.7/pollination/dragonfly_energy/
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-02-02 16:19:08.000000 pollination-dragonfly-energy-0.2.7/pollination/dragonfly_energy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-02-02 16:19:08.000000 pollination-dragonfly-energy-0.2.7/pollination/dragonfly_energy/edit.py
--rw-r--r--   0 runner    (1001) docker     (121)     5282 2022-02-02 16:19:08.000000 pollination-dragonfly-energy-0.2.7/pollination/dragonfly_energy/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 16:20:09.000000 pollination-dragonfly-energy-0.2.7/pollination_dragonfly_energy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-02-02 16:20:09.000000 pollination-dragonfly-energy-0.2.7/pollination_dragonfly_energy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-02-02 16:20:09.000000 pollination-dragonfly-energy-0.2.7/pollination_dragonfly_energy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-02 16:20:09.000000 pollination-dragonfly-energy-0.2.7/pollination_dragonfly_energy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-02 16:19:31.000000 pollination-dragonfly-energy-0.2.7/pollination_dragonfly_energy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-02-02 16:20:09.000000 pollination-dragonfly-energy-0.2.7/pollination_dragonfly_energy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-02-02 16:20:09.000000 pollination-dragonfly-energy-0.2.7/pollination_dragonfly_energy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-02-02 16:19:08.000000 pollination-dragonfly-energy-0.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-02-02 16:20:09.000000 pollination-dragonfly-energy-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-02-02 16:19:08.000000 pollination-dragonfly-energy-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 16:20:09.000000 pollination-dragonfly-energy-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-02 16:19:08.000000 pollination-dragonfly-energy-0.2.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-02-02 16:19:08.000000 pollination-dragonfly-energy-0.2.7/tests/edit_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-02-02 16:19:08.000000 pollination-dragonfly-energy-0.2.7/tests/translate_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:52:15.000000 pollination-dragonfly-energy-0.2.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:52:15.000000 pollination-dragonfly-energy-0.2.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-20 22:51:19.000000 pollination-dragonfly-energy-0.2.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:52:15.000000 pollination-dragonfly-energy-0.2.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-20 22:51:19.000000 pollination-dragonfly-energy-0.2.8/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-20 22:51:19.000000 pollination-dragonfly-energy-0.2.8/.github/workflows/dependency-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-20 22:51:19.000000 pollination-dragonfly-energy-0.2.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-20 22:51:19.000000 pollination-dragonfly-energy-0.2.8/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-20 22:51:19.000000 pollination-dragonfly-energy-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-20 22:52:15.000000 pollination-dragonfly-energy-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-20 22:51:19.000000 pollination-dragonfly-energy-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-20 22:51:19.000000 pollination-dragonfly-energy-0.2.8/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 22:51:19.000000 pollination-dragonfly-energy-0.2.8/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:52:15.000000 pollination-dragonfly-energy-0.2.8/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:52:15.000000 pollination-dragonfly-energy-0.2.8/pollination/dragonfly_energy/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-20 22:51:19.000000 pollination-dragonfly-energy-0.2.8/pollination/dragonfly_energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-20 22:51:19.000000 pollination-dragonfly-energy-0.2.8/pollination/dragonfly_energy/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-20 22:51:19.000000 pollination-dragonfly-energy-0.2.8/pollination/dragonfly_energy/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:52:15.000000 pollination-dragonfly-energy-0.2.8/pollination_dragonfly_energy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-20 22:52:15.000000 pollination-dragonfly-energy-0.2.8/pollination_dragonfly_energy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-20 22:52:15.000000 pollination-dragonfly-energy-0.2.8/pollination_dragonfly_energy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 22:52:15.000000 pollination-dragonfly-energy-0.2.8/pollination_dragonfly_energy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 22:51:39.000000 pollination-dragonfly-energy-0.2.8/pollination_dragonfly_energy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-20 22:52:15.000000 pollination-dragonfly-energy-0.2.8/pollination_dragonfly_energy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 22:52:15.000000 pollination-dragonfly-energy-0.2.8/pollination_dragonfly_energy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-20 22:51:19.000000 pollination-dragonfly-energy-0.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-20 22:52:15.000000 pollination-dragonfly-energy-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-20 22:51:19.000000 pollination-dragonfly-energy-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:52:15.000000 pollination-dragonfly-energy-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:51:19.000000 pollination-dragonfly-energy-0.2.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-20 22:51:19.000000 pollination-dragonfly-energy-0.2.8/tests/edit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-20 22:51:19.000000 pollination-dragonfly-energy-0.2.8/tests/translate_test.py
```

### Comparing `pollination-dragonfly-energy-0.2.7/.github/workflows/ci.yaml` & `pollination-dragonfly-energy-0.2.8/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-dragonfly-energy-0.2.7/.github/workflows/dependency-release.yaml` & `pollination-dragonfly-energy-0.2.8/.github/workflows/dependency-release.yaml`

 * *Files identical despite different names*

### Comparing `pollination-dragonfly-energy-0.2.7/LICENSE` & `pollination-dragonfly-energy-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-dragonfly-energy-0.2.7/PKG-INFO` & `pollination-dragonfly-energy-0.2.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pollination-dragonfly-energy
-Version: 0.2.7
+Version: 0.2.8
 Summary: Dragonfly energy plugin for Pollination.
 Home-page: https://github.com/pollination/dragonfly-energy
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: chris, ladybug-tools
 Maintainer-email: chris@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
 Project-URL: icon, https://raw.githubusercontent.com/ladybug-tools/artwork/master/icons_bugs/grasshopper_tabs/Dragonfly.png
 Project-URL: docker, https://hub.docker.com/r/ladybugtools/dragonfly-energy
-Description: # Pollination Dragonfly Energy
-        
-        A plugin that adds large-scale energy simulation functions to Pollination, including
-        scales from large buildings to entire urban districts.
-        
-        ## Sources
-        
-        - `dragonfly-energy` Python package. [PyPI](https://pypi.org/project/dragonfly-energy/), [source](https://github.com/ladybug-tools/dragonfly-energy)
-        
 Keywords: dragonfly,energy,ladybug-tools,energyplus,openstudio
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Pollination Dragonfly Energy
+
+A plugin that adds large-scale energy simulation functions to Pollination, including
+scales from large buildings to entire urban districts.
+
+## Sources
+
+- `dragonfly-energy` Python package. [PyPI](https://pypi.org/project/dragonfly-energy/), [source](https://github.com/ladybug-tools/dragonfly-energy)
```

### Comparing `pollination-dragonfly-energy-0.2.7/pollination/dragonfly_energy/edit.py` & `pollination-dragonfly-energy-0.2.8/pollination/dragonfly_energy/edit.py`

 * *Files identical despite different names*

### Comparing `pollination-dragonfly-energy-0.2.7/pollination/dragonfly_energy/translate.py` & `pollination-dragonfly-energy-0.2.8/pollination/dragonfly_energy/translate.py`

 * *Files identical despite different names*

### Comparing `pollination-dragonfly-energy-0.2.7/pollination_dragonfly_energy.egg-info/PKG-INFO` & `pollination-dragonfly-energy-0.2.8/pollination_dragonfly_energy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pollination-dragonfly-energy
-Version: 0.2.7
+Version: 0.2.8
 Summary: Dragonfly energy plugin for Pollination.
 Home-page: https://github.com/pollination/dragonfly-energy
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: chris, ladybug-tools
 Maintainer-email: chris@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
 Project-URL: icon, https://raw.githubusercontent.com/ladybug-tools/artwork/master/icons_bugs/grasshopper_tabs/Dragonfly.png
 Project-URL: docker, https://hub.docker.com/r/ladybugtools/dragonfly-energy
-Description: # Pollination Dragonfly Energy
-        
-        A plugin that adds large-scale energy simulation functions to Pollination, including
-        scales from large buildings to entire urban districts.
-        
-        ## Sources
-        
-        - `dragonfly-energy` Python package. [PyPI](https://pypi.org/project/dragonfly-energy/), [source](https://github.com/ladybug-tools/dragonfly-energy)
-        
 Keywords: dragonfly,energy,ladybug-tools,energyplus,openstudio
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Pollination Dragonfly Energy
+
+A plugin that adds large-scale energy simulation functions to Pollination, including
+scales from large buildings to entire urban districts.
+
+## Sources
+
+- `dragonfly-energy` Python package. [PyPI](https://pypi.org/project/dragonfly-energy/), [source](https://github.com/ladybug-tools/dragonfly-energy)
```

### Comparing `pollination-dragonfly-energy-0.2.7/pollination_dragonfly_energy.egg-info/SOURCES.txt` & `pollination-dragonfly-energy-0.2.8/pollination_dragonfly_energy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-dragonfly-energy-0.2.7/setup.py` & `pollination-dragonfly-energy-0.2.8/setup.py`

 * *Files identical despite different names*

