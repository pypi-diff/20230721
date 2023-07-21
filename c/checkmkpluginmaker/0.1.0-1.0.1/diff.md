# Comparing `tmp/checkmkpluginmaker-0.1.0.tar.gz` & `tmp/checkmkpluginmaker-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkmkpluginmaker-0.1.0.tar", max compression
+gzip compressed data, was "checkmkpluginmaker-1.0.1.tar", max compression
```

## Comparing `checkmkpluginmaker-0.1.0.tar` & `checkmkpluginmaker-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      319 2023-07-21 16:57:38.744578 checkmkpluginmaker-0.1.0/README.md
--rw-r--r--   0        0        0      556 2023-07-21 16:33:52.794578 checkmkpluginmaker-0.1.0/pluginmaker/__init__.py
--rw-r--r--   0        0        0       24 2023-07-21 09:12:45.534578 checkmkpluginmaker-0.1.0/pluginmaker/cookiecutter_templates/__init__.py
--rw-r--r--   0        0        0      806 2023-07-21 16:51:32.184578 checkmkpluginmaker-0.1.0/pluginmaker/cookiecutter_templates/cmk_plugin/cookiecutter.json
--rw-r--r--   0        0        0     1472 2023-07-21 16:52:27.424578 checkmkpluginmaker-0.1.0/pluginmaker/cookiecutter_templates/cmk_plugin/hooks/pre_gen_project.py
--rw-r--r--   0        0        0      327 2023-07-21 09:13:57.824578 checkmkpluginmaker-0.1.0/pluginmaker/cookiecutter_templates/cmk_plugin/setup.py
--rw-r--r--   0        0        0     1811 2023-07-21 16:14:14.124578 checkmkpluginmaker-0.1.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0        0        0     1175 2023-07-21 15:39:03.984578 checkmkpluginmaker-0.1.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_invoker/agent_{{cookiecutter.agent_id}}
--rw-r--r--   0        0        0     4063 2023-07-21 15:35:37.274578 checkmkpluginmaker-0.1.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_special/agent_{{cookiecutter.agent_id}}
--rw-r--r--   0        0        0     1058 2023-07-21 16:10:45.904578 checkmkpluginmaker-0.1.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/mkp/config
--rw-r--r--   0        0        0      848 2023-07-21 15:47:57.314578 checkmkpluginmaker-0.1.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/plugin/service_{{cookiecutter.agent_id}}.py
--rw-r--r--   0        0        0     1888 2023-07-21 15:43:49.764578 checkmkpluginmaker-0.1.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/wato/{{cookiecutter.agent_id}}_register.py
--rw-r--r--   0        0        0     1128 2023-07-21 09:11:22.454578 checkmkpluginmaker-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 checkmkpluginmaker-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      335 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/README.md
+-rw-r--r--   0        0        0      556 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/__init__.py
+-rw-r--r--   0        0        0      806 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/cookiecutter.json
+-rw-r--r--   0        0        0     1472 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      327 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/setup.py
+-rw-r--r--   0        0        0     1811 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0        0        0     1175 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_invoker/agent_{{cookiecutter.agent_id}}
+-rw-r--r--   0        0        0     4063 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_special/agent_{{cookiecutter.agent_id}}
+-rw-r--r--   0        0        0     1058 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/mkp/config
+-rw-r--r--   0        0        0      848 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/plugin/service_{{cookiecutter.agent_id}}.py
+-rw-r--r--   0        0        0     1888 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/wato/{{cookiecutter.agent_id}}_register.py
+-rw-r--r--   0        0        0     1128 2023-07-21 17:11:43.856893 checkmkpluginmaker-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 checkmkpluginmaker-1.0.1/PKG-INFO
```

### Comparing `checkmkpluginmaker-0.1.0/pluginmaker/__init__.py` & `checkmkpluginmaker-1.0.1/pluginmaker/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """Entry point of my coca tools
 """
 import os
 import sys
 from cookiecutter.main import cookiecutter
 
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 BASE_PATH = os.path.dirname(os.path.abspath(__file__))
 TEMPLATE_PATH = os.path.join(BASE_PATH, 'cookiecutter_templates')
 
 
 def welcome():
     """Say welcome to users"""
     print('I am , welcome to CheckMK Plugin Maker')
```

### Comparing `checkmkpluginmaker-0.1.0/pluginmaker/cookiecutter_templates/cmk_plugin/cookiecutter.json` & `checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `checkmkpluginmaker-0.1.0/pluginmaker/cookiecutter_templates/cmk_plugin/hooks/pre_gen_project.py` & `checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/hooks/pre_gen_project.py`

 * *Files identical despite different names*

### Comparing `checkmkpluginmaker-0.1.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/Makefile` & `checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `checkmkpluginmaker-0.1.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_invoker/agent_{{cookiecutter.agent_id}}` & `checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_invoker/agent_{{cookiecutter.agent_id}}`

 * *Files identical despite different names*

### Comparing `checkmkpluginmaker-0.1.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_special/agent_{{cookiecutter.agent_id}}` & `checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_special/agent_{{cookiecutter.agent_id}}`

 * *Files identical despite different names*

### Comparing `checkmkpluginmaker-0.1.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/mkp/config` & `checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/mkp/config`

 * *Files identical despite different names*

### Comparing `checkmkpluginmaker-0.1.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/plugin/service_{{cookiecutter.agent_id}}.py` & `checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/plugin/service_{{cookiecutter.agent_id}}.py`

 * *Files identical despite different names*

### Comparing `checkmkpluginmaker-0.1.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/wato/{{cookiecutter.agent_id}}_register.py` & `checkmkpluginmaker-1.0.1/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/wato/{{cookiecutter.agent_id}}_register.py`

 * *Files identical despite different names*

### Comparing `checkmkpluginmaker-0.1.0/pyproject.toml` & `checkmkpluginmaker-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkmkpluginmaker"
-version = "0.1.0"
+version = "1.0.1"
 description = ""
 authors = ["NhanDD3 <nhandd3@fpt.com>"]
 readme = "README.md"
 packages = [{include = "pluginmaker"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `checkmkpluginmaker-0.1.0/PKG-INFO` & `checkmkpluginmaker-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkmkpluginmaker
-Version: 0.1.0
+Version: 1.0.1
 Summary: 
 Author: NhanDD3
 Author-email: nhandd3@fpt.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bump2version (>=1.0.1,<2.0.0)
@@ -22,19 +22,19 @@
 Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
 Description-Content-Type: text/markdown
 
 # Installation
 - Require python >= 3.11
 - using pip
     ```
-    $ pip install coca-tools
+    $ pip install checkmkpluginmaker
     ```
 - using poetry
     ```
-    $ poetry add coca-tools
+    $ poetry add checkmkpluginmaker
     ```
 
 
 # Guide
 - Require: using in global environment
 - create new checkmk plugin template with command then fill the questions
     ```
```

