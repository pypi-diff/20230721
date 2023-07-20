# Comparing `tmp/pollination-dragonfly-annual-energy-use-0.3.3.tar.gz` & `tmp/pollination-dragonfly-annual-energy-use-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-dragonfly-annual-energy-use-0.3.3.tar", last modified: Wed Feb  2 17:47:35 2022, max compression
+gzip compressed data, was "dist/pollination-dragonfly-annual-energy-use-0.3.4.tar", last modified: Thu Jul 20 23:09:03 2023, max compression
```

## Comparing `pollination-dragonfly-annual-energy-use-0.3.3.tar` & `pollination-dragonfly-annual-energy-use-0.3.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 17:47:35.000000 pollination-dragonfly-annual-energy-use-0.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 17:47:35.000000 pollination-dragonfly-annual-energy-use-0.3.3/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-02-02 17:46:34.000000 pollination-dragonfly-annual-energy-use-0.3.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 17:47:35.000000 pollination-dragonfly-annual-energy-use-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3043 2022-02-02 17:46:34.000000 pollination-dragonfly-annual-energy-use-0.3.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-02-02 17:46:34.000000 pollination-dragonfly-annual-energy-use-0.3.3/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-02-02 17:46:34.000000 pollination-dragonfly-annual-energy-use-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-02-02 17:46:34.000000 pollination-dragonfly-annual-energy-use-0.3.3/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (121)     5748 2022-02-02 17:46:34.000000 pollination-dragonfly-annual-energy-use-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-02-02 17:47:35.000000 pollination-dragonfly-annual-energy-use-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-02-02 17:46:34.000000 pollination-dragonfly-annual-energy-use-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-02-02 17:46:34.000000 pollination-dragonfly-annual-energy-use-0.3.3/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-02-02 17:46:34.000000 pollination-dragonfly-annual-energy-use-0.3.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 17:47:35.000000 pollination-dragonfly-annual-energy-use-0.3.3/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 17:47:35.000000 pollination-dragonfly-annual-energy-use-0.3.3/pollination/dragonfly_annual_energy_use/
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-02-02 17:46:34.000000 pollination-dragonfly-annual-energy-use-0.3.3/pollination/dragonfly_annual_energy_use/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6493 2022-02-02 17:46:34.000000 pollination-dragonfly-annual-energy-use-0.3.3/pollination/dragonfly_annual_energy_use/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 17:47:35.000000 pollination-dragonfly-annual-energy-use-0.3.3/pollination_dragonfly_annual_energy_use.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-02-02 17:47:35.000000 pollination-dragonfly-annual-energy-use-0.3.3/pollination_dragonfly_annual_energy_use.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-02-02 17:47:35.000000 pollination-dragonfly-annual-energy-use-0.3.3/pollination_dragonfly_annual_energy_use.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-02 17:47:35.000000 pollination-dragonfly-annual-energy-use-0.3.3/pollination_dragonfly_annual_energy_use.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-02 17:46:54.000000 pollination-dragonfly-annual-energy-use-0.3.3/pollination_dragonfly_annual_energy_use.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-02-02 17:47:35.000000 pollination-dragonfly-annual-energy-use-0.3.3/pollination_dragonfly_annual_energy_use.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-02-02 17:47:35.000000 pollination-dragonfly-annual-energy-use-0.3.3/pollination_dragonfly_annual_energy_use.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-02-02 17:46:34.000000 pollination-dragonfly-annual-energy-use-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-02-02 17:47:35.000000 pollination-dragonfly-annual-energy-use-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-02-02 17:46:34.000000 pollination-dragonfly-annual-energy-use-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 17:47:35.000000 pollination-dragonfly-annual-energy-use-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-02 17:46:34.000000 pollination-dragonfly-annual-energy-use-0.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-02-02 17:46:34.000000 pollination-dragonfly-annual-energy-use-0.3.3/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:09:03.000000 pollination-dragonfly-annual-energy-use-0.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:09:03.000000 pollination-dragonfly-annual-energy-use-0.3.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-20 23:08:02.000000 pollination-dragonfly-annual-energy-use-0.3.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:09:03.000000 pollination-dragonfly-annual-energy-use-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-20 23:08:02.000000 pollination-dragonfly-annual-energy-use-0.3.4/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-20 23:08:02.000000 pollination-dragonfly-annual-energy-use-0.3.4/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-20 23:08:02.000000 pollination-dragonfly-annual-energy-use-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-20 23:08:02.000000 pollination-dragonfly-annual-energy-use-0.3.4/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-20 23:08:02.000000 pollination-dragonfly-annual-energy-use-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-20 23:09:03.000000 pollination-dragonfly-annual-energy-use-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-20 23:08:02.000000 pollination-dragonfly-annual-energy-use-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-20 23:08:02.000000 pollination-dragonfly-annual-energy-use-0.3.4/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 23:08:02.000000 pollination-dragonfly-annual-energy-use-0.3.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:09:03.000000 pollination-dragonfly-annual-energy-use-0.3.4/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:09:03.000000 pollination-dragonfly-annual-energy-use-0.3.4/pollination/dragonfly_annual_energy_use/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-20 23:08:02.000000 pollination-dragonfly-annual-energy-use-0.3.4/pollination/dragonfly_annual_energy_use/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-20 23:08:02.000000 pollination-dragonfly-annual-energy-use-0.3.4/pollination/dragonfly_annual_energy_use/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:09:03.000000 pollination-dragonfly-annual-energy-use-0.3.4/pollination_dragonfly_annual_energy_use.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-20 23:09:03.000000 pollination-dragonfly-annual-energy-use-0.3.4/pollination_dragonfly_annual_energy_use.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-20 23:09:03.000000 pollination-dragonfly-annual-energy-use-0.3.4/pollination_dragonfly_annual_energy_use.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 23:09:03.000000 pollination-dragonfly-annual-energy-use-0.3.4/pollination_dragonfly_annual_energy_use.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 23:08:24.000000 pollination-dragonfly-annual-energy-use-0.3.4/pollination_dragonfly_annual_energy_use.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-20 23:09:03.000000 pollination-dragonfly-annual-energy-use-0.3.4/pollination_dragonfly_annual_energy_use.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 23:09:03.000000 pollination-dragonfly-annual-energy-use-0.3.4/pollination_dragonfly_annual_energy_use.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-20 23:08:02.000000 pollination-dragonfly-annual-energy-use-0.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-20 23:09:03.000000 pollination-dragonfly-annual-energy-use-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-20 23:08:02.000000 pollination-dragonfly-annual-energy-use-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:09:03.000000 pollination-dragonfly-annual-energy-use-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 23:08:02.000000 pollination-dragonfly-annual-energy-use-0.3.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-20 23:08:02.000000 pollination-dragonfly-annual-energy-use-0.3.4/tests/validation_test.py
```

### Comparing `pollination-dragonfly-annual-energy-use-0.3.3/.github/workflows/ci.yaml` & `pollination-dragonfly-annual-energy-use-0.3.4/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-dragonfly-annual-energy-use-0.3.3/.github/workflows/tests.yaml` & `pollination-dragonfly-annual-energy-use-0.3.4/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-dragonfly-annual-energy-use-0.3.3/LICENSE` & `pollination-dragonfly-annual-energy-use-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-dragonfly-annual-energy-use-0.3.3/PKG-INFO` & `pollination-dragonfly-annual-energy-use-0.3.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pollination-dragonfly-annual-energy-use
-Version: 0.3.3
+Version: 0.3.4
 Summary: Run an annual energy simulation for a Dragonfly Model and compute energy use intensity.
 Home-page: https://github.com/pollination/dragonfly-annual-energy-use
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: chris, ladybug-tools
 Maintainer-email: chris@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
 Project-URL: icon, https://raw.githubusercontent.com/ladybug-tools/artwork/master/icons_components/dragonfly/png/dfeui.png
 Project-URL: docker, https://hub.docker.com/r/ladybugtools/dragonfly-energy
-Description: # dragonfly-annual-energy-use
-        
-        Calculate annual energy use intensity (EUI) for a Dragonfly model.
-        
 Keywords: dragonfly,energy,ladybug-tools,energyplus,openstudio,energy,dragonfly-annual-energy-use
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dragonfly-annual-energy-use
+
+Calculate annual energy use intensity (EUI) for a Dragonfly model.
```

### Comparing `pollination-dragonfly-annual-energy-use-0.3.3/pollination/dragonfly_annual_energy_use/entry.py` & `pollination-dragonfly-annual-energy-use-0.3.4/pollination/dragonfly_annual_energy_use/entry.py`

 * *Files identical despite different names*

### Comparing `pollination-dragonfly-annual-energy-use-0.3.3/pollination_dragonfly_annual_energy_use.egg-info/PKG-INFO` & `pollination-dragonfly-annual-energy-use-0.3.4/pollination_dragonfly_annual_energy_use.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pollination-dragonfly-annual-energy-use
-Version: 0.3.3
+Version: 0.3.4
 Summary: Run an annual energy simulation for a Dragonfly Model and compute energy use intensity.
 Home-page: https://github.com/pollination/dragonfly-annual-energy-use
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: chris, ladybug-tools
 Maintainer-email: chris@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
 Project-URL: icon, https://raw.githubusercontent.com/ladybug-tools/artwork/master/icons_components/dragonfly/png/dfeui.png
 Project-URL: docker, https://hub.docker.com/r/ladybugtools/dragonfly-energy
-Description: # dragonfly-annual-energy-use
-        
-        Calculate annual energy use intensity (EUI) for a Dragonfly model.
-        
 Keywords: dragonfly,energy,ladybug-tools,energyplus,openstudio,energy,dragonfly-annual-energy-use
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dragonfly-annual-energy-use
+
+Calculate annual energy use intensity (EUI) for a Dragonfly model.
```

### Comparing `pollination-dragonfly-annual-energy-use-0.3.3/pollination_dragonfly_annual_energy_use.egg-info/SOURCES.txt` & `pollination-dragonfly-annual-energy-use-0.3.4/pollination_dragonfly_annual_energy_use.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-dragonfly-annual-energy-use-0.3.3/setup.py` & `pollination-dragonfly-annual-energy-use-0.3.4/setup.py`

 * *Files identical despite different names*

