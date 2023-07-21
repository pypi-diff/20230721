# Comparing `tmp/gardener-cicd-cli-1.2112.0.tar.gz` & `tmp/gardener-cicd-cli-1.2113.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-cli-1.2112.0.tar", last modified: Thu Jul 20 07:44:25 2023, max compression
+gzip compressed data, was "gardener-cicd-cli-1.2113.0.tar", last modified: Fri Jul 21 11:49:30 2023, max compression
```

## Comparing `gardener-cicd-cli-1.2112.0.tar` & `gardener-cicd-cli-1.2113.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 07:44:25.581850 gardener-cicd-cli-1.2112.0/
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      135 2023-07-20 07:44:25.581850 gardener-cicd-cli-1.2112.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 07:44:25.573850 gardener-cicd-cli-1.2112.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)    11039 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/bin/component-cli
--rwxr-xr-x   0 root         (0) root         (0)      369 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/bin/helm
--rwxr-xr-x   0 root         (0) root         (0)     5611 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/bin/launch-dockerd.sh
--rwxr-xr-x   0 root         (0) root         (0)     3301 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/bin/purge_history
--rwxr-xr-x   0 root         (0) root         (0)      265 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/bin/yaml2json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 07:44:25.577850 gardener-cicd-cli-1.2112.0/gardener_ci/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3901 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/_cfg_mgmt.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/_clamav.py
--rw-r--r--   0 root         (0) root         (0)     6463 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/_concourse.py
--rw-r--r--   0 root         (0) root         (0)     8384 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/_oci.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/_osinfo.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/_release_notes.py
--rw-r--r--   0 root         (0) root         (0)      380 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/_slack.py
--rw-r--r--   0 root         (0) root         (0)    11329 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/bdba.py
--rw-r--r--   0 root         (0) root         (0)     8618 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/cd.py
--rw-r--r--   0 root         (0) root         (0)     1899 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/checkmarx_cli.py
--rwxr-xr-x   0 root         (0) root         (0)     9186 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/cli_gen.py
--rw-r--r--   0 root         (0) root         (0)     8141 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/compliance.py
--rw-r--r--   0 root         (0) root         (0)     3188 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/config.py
--rw-r--r--   0 root         (0) root         (0)      401 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/containerutil.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/docker.py
--rw-r--r--   0 root         (0) root         (0)     2415 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/elastic.py
--rw-r--r--   0 root         (0) root         (0)     3512 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/gh.py
--rw-r--r--   0 root         (0) root         (0)     4935 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/githubutil.py
--rw-r--r--   0 root         (0) root         (0)     3212 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/ocm.py
--rw-r--r--   0 root         (0) root         (0)    12219 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     3037 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/productutil_v2.py
--rwxr-xr-x   0 root         (0) root         (0)      265 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/gardener_ci/yaml2json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 07:44:25.581850 gardener-cicd-cli-1.2112.0/gardener_cicd_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      135 2023-07-20 07:44:25.000000 gardener-cicd-cli-1.2112.0/gardener_cicd_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      967 2023-07-20 07:44:25.000000 gardener-cicd-cli-1.2112.0/gardener_cicd_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 07:44:25.000000 gardener-cicd-cli-1.2112.0/gardener_cicd_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-07-20 07:44:25.000000 gardener-cicd-cli-1.2112.0/gardener_cicd_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-07-20 07:44:25.000000 gardener-cicd-cli-1.2112.0/gardener_cicd_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-20 07:44:25.000000 gardener-cicd-cli-1.2112.0/gardener_cicd_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 07:44:25.581850 gardener-cicd-cli-1.2112.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1514 2023-07-20 06:50:11.000000 gardener-cicd-cli-1.2112.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:49:30.897843 gardener-cicd-cli-1.2113.0/
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      135 2023-07-21 11:49:30.897843 gardener-cicd-cli-1.2113.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:49:30.893843 gardener-cicd-cli-1.2113.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)    11039 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/bin/component-cli
+-rwxr-xr-x   0 root         (0) root         (0)      369 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/bin/helm
+-rwxr-xr-x   0 root         (0) root         (0)     5611 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/bin/launch-dockerd.sh
+-rwxr-xr-x   0 root         (0) root         (0)     3301 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/bin/purge_history
+-rwxr-xr-x   0 root         (0) root         (0)      265 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/bin/yaml2json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:49:30.897843 gardener-cicd-cli-1.2113.0/gardener_ci/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3901 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/_cfg_mgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/_clamav.py
+-rw-r--r--   0 root         (0) root         (0)     6463 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/_concourse.py
+-rw-r--r--   0 root         (0) root         (0)     8384 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/_oci.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/_osinfo.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/_release_notes.py
+-rw-r--r--   0 root         (0) root         (0)      380 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/_slack.py
+-rw-r--r--   0 root         (0) root         (0)    12183 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/bdba.py
+-rw-r--r--   0 root         (0) root         (0)     8618 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/cd.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/checkmarx_cli.py
+-rwxr-xr-x   0 root         (0) root         (0)     9186 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/cli_gen.py
+-rw-r--r--   0 root         (0) root         (0)     8141 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/compliance.py
+-rw-r--r--   0 root         (0) root         (0)     3188 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/config.py
+-rw-r--r--   0 root         (0) root         (0)      401 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/containerutil.py
+-rw-r--r--   0 root         (0) root         (0)      886 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/docker.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/elastic.py
+-rw-r--r--   0 root         (0) root         (0)     3512 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/gh.py
+-rw-r--r--   0 root         (0) root         (0)     4935 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/githubutil.py
+-rw-r--r--   0 root         (0) root         (0)     3212 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/ocm.py
+-rw-r--r--   0 root         (0) root         (0)    12219 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     3037 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/productutil_v2.py
+-rwxr-xr-x   0 root         (0) root         (0)      265 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/gardener_ci/yaml2json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:49:30.897843 gardener-cicd-cli-1.2113.0/gardener_cicd_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-07-21 11:49:30.000000 gardener-cicd-cli-1.2113.0/gardener_cicd_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      967 2023-07-21 11:49:30.000000 gardener-cicd-cli-1.2113.0/gardener_cicd_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 11:49:30.000000 gardener-cicd-cli-1.2113.0/gardener_cicd_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-07-21 11:49:30.000000 gardener-cicd-cli-1.2113.0/gardener_cicd_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-21 11:49:30.000000 gardener-cicd-cli-1.2113.0/gardener_cicd_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-21 11:49:30.000000 gardener-cicd-cli-1.2113.0/gardener_cicd_cli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 11:49:30.897843 gardener-cicd-cli-1.2113.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-07-21 11:07:46.000000 gardener-cicd-cli-1.2113.0/setup.py
```

### Comparing `gardener-cicd-cli-1.2112.0/bin/component-cli` & `gardener-cicd-cli-1.2113.0/bin/component-cli`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/bin/launch-dockerd.sh` & `gardener-cicd-cli-1.2113.0/bin/launch-dockerd.sh`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/bin/purge_history` & `gardener-cicd-cli-1.2113.0/bin/purge_history`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/gardener_ci/_cfg_mgmt.py` & `gardener-cicd-cli-1.2113.0/gardener_ci/_cfg_mgmt.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/gardener_ci/_clamav.py` & `gardener-cicd-cli-1.2113.0/gardener_ci/_clamav.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/gardener_ci/_concourse.py` & `gardener-cicd-cli-1.2113.0/gardener_ci/_concourse.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/gardener_ci/_oci.py` & `gardener-cicd-cli-1.2113.0/gardener_ci/_oci.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/gardener_ci/_osinfo.py` & `gardener-cicd-cli-1.2113.0/gardener_ci/_osinfo.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/gardener_ci/_release_notes.py` & `gardener-cicd-cli-1.2113.0/gardener_ci/_release_notes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/gardener_ci/bdba.py` & `gardener-cicd-cli-1.2113.0/gardener_ci/bdba.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import gci.componentmodel as cm
 
 from protecode.model import CVSSVersion, TriageScope
 from protecode.scanning import upload_grouped_images as _upload_grouped_images
 import ccc.oci
 import ccc.protecode
 import ci.util
+import cnudie.iter
 import cnudie.retrieve as cr
 import concourse.steps.component_descriptor_util as component_descriptor_util
 import concourse.steps.images
 import concourse.steps.scan_container_images
 import ctx
 import dso.cvss
 import dso.labels
@@ -24,25 +25,57 @@
 import protecode.model as pm
 
 
 __cmd_name__ = 'bdba'
 logger = logging.getLogger(__name__)
 
 
+def ls_products(
+    ocm_component: str,
+    bdba_cfg_name='gardener',
+    group_id=407,
+    ocm_repo: str=None,
+):
+    if not ocm_repo:
+        ocm_repo = ctx.cfg.ctx.ocm_repo_base_url
+
+    client = ccc.protecode.client(bdba_cfg_name)
+
+    if not ':' in ocm_component:
+        raise ValueError('ocm_component must have form <name>:<version>')
+
+    ocm_lookup = cr.create_default_component_descriptor_lookup(default_ctx_repo=ocm_repo)
+
+    root_component_descriptor = ocm_lookup(ocm_component)
+
+    for ocm_node in cnudie.iter.iter(
+        component=root_component_descriptor,
+        lookup=ocm_lookup,
+        node_filter=cnudie.iter.Filter.components,
+    ):
+        component = ocm_node.component
+
+        metadata = {
+            'COMPONENT_NAME': component.name,
+            'COMPONENT_VERSION': component.version,
+        }
+
+        for app in client.list_apps(group_id=group_id, custom_attribs=metadata):
+            print(app.product_id())
+
+
 def rescore(
     protecode_cfg_name: str,
     product_id: int,
     rescoring_rules: str,
     ctx_repo: str=None,
     categorisation: str=None,
     assess: bool=False,
 ):
-    cfg_factory = ci.util.ctx().cfg_factory()
-    protecode_cfg = cfg_factory.protecode(protecode_cfg_name)
-    client = ccc.protecode.client(protecode_cfg=protecode_cfg)
+    client = ccc.protecode.client(protecode_cfg_name)
 
     if categorisation and not os.path.isfile(categorisation):
         print(f'{categorisation} must point to an existing file w/ CveCategorisation')
         exit(1)
 
     if not os.path.isfile(rescoring_rules):
         print(f'{rescoring_rules} must point to an existing file w/ RescoringRules')
```

### Comparing `gardener-cicd-cli-1.2112.0/gardener_ci/cd.py` & `gardener-cicd-cli-1.2113.0/gardener_ci/cd.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/gardener_ci/checkmarx_cli.py` & `gardener-cicd-cli-1.2113.0/gardener_ci/checkmarx_cli.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/gardener_ci/cli_gen.py` & `gardener-cicd-cli-1.2113.0/gardener_ci/cli_gen.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/gardener_ci/compliance.py` & `gardener-cicd-cli-1.2113.0/gardener_ci/compliance.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/gardener_ci/config.py` & `gardener-cicd-cli-1.2113.0/gardener_ci/config.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/gardener_ci/docker.py` & `gardener-cicd-cli-1.2113.0/gardener_ci/docker.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/gardener_ci/elastic.py` & `gardener-cicd-cli-1.2113.0/gardener_ci/elastic.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/gardener_ci/gh.py` & `gardener-cicd-cli-1.2113.0/gardener_ci/gh.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/gardener_ci/githubutil.py` & `gardener-cicd-cli-1.2113.0/gardener_ci/githubutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/gardener_ci/ocm.py` & `gardener-cicd-cli-1.2113.0/gardener_ci/ocm.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/gardener_ci/pipeline.py` & `gardener-cicd-cli-1.2113.0/gardener_ci/pipeline.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/gardener_ci/productutil_v2.py` & `gardener-cicd-cli-1.2113.0/gardener_ci/productutil_v2.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/gardener_cicd_cli.egg-info/SOURCES.txt` & `gardener-cicd-cli-1.2113.0/gardener_cicd_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2112.0/setup.py` & `gardener-cicd-cli-1.2113.0/setup.py`

 * *Files identical despite different names*

