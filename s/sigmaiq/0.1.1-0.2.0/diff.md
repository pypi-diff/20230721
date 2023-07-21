# Comparing `tmp/sigmaiq-0.1.1.tar.gz` & `tmp/sigmaiq-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmaiq-0.1.1.tar", max compression
+gzip compressed data, was "sigmaiq-0.2.0.tar", max compression
```

## Comparing `sigmaiq-0.1.1.tar` & `sigmaiq-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
--rw-r--r--   0        0        0    26526 2023-06-20 15:33:58.531341 sigmaiq-0.1.1/LICENSE
--rw-r--r--   0        0        0    23477 2023-06-20 15:33:58.531341 sigmaiq-0.1.1/README.md
--rw-r--r--   0        0        0     1365 2023-06-20 15:33:58.531341 sigmaiq-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2964 2023-06-20 15:33:58.531341 sigmaiq-0.1.1/sigmaiq/.gitignore
--rw-r--r--   0        0        0      131 2023-06-20 15:33:58.531341 sigmaiq-0.1.1/sigmaiq/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 15:33:58.531341 sigmaiq-0.1.1/sigmaiq/backends/__init__.py
--rw-r--r--   0        0        0       51 2023-06-20 15:33:58.531341 sigmaiq-0.1.1/sigmaiq/backends/carbonblack/__init__.py
--rw-r--r--   0        0        0      802 2023-06-20 15:33:58.531341 sigmaiq-0.1.1/sigmaiq/backends/carbonblack/carbonblack.py
--rw-r--r--   0        0        0       57 2023-06-20 15:33:58.531341 sigmaiq-0.1.1/sigmaiq/backends/crowdstrike/__init__.py
--rw-r--r--   0        0        0      394 2023-06-20 15:33:58.531341 sigmaiq-0.1.1/sigmaiq/backends/crowdstrike/crowdstrike.py
--rw-r--r--   0        0        0       55 2023-06-20 15:33:58.531341 sigmaiq-0.1.1/sigmaiq/backends/elasticsearch/__init__.py
--rw-r--r--   0        0        0      520 2023-06-20 15:33:58.531341 sigmaiq-0.1.1/sigmaiq/backends/elasticsearch/elasticsearch.py
--rw-r--r--   0        0        0       48 2023-06-20 15:33:58.531341 sigmaiq-0.1.1/sigmaiq/backends/insightidr/__init__.py
--rw-r--r--   0        0        0      336 2023-06-20 15:33:58.531341 sigmaiq-0.1.1/sigmaiq/backends/insightidr/insightidr.py
--rw-r--r--   0        0        0       36 2023-06-20 15:33:58.531341 sigmaiq-0.1.1/sigmaiq/backends/loki/__init__.py
--rw-r--r--   0        0        0      437 2023-06-20 15:33:58.531341 sigmaiq-0.1.1/sigmaiq/backends/loki/loki.py
--rw-r--r--   0        0        0       69 2023-06-20 15:33:58.531341 sigmaiq-0.1.1/sigmaiq/backends/microsoft365defender/__init__.py
--rw-r--r--   0        0        0      397 2023-06-20 15:33:58.531341 sigmaiq-0.1.1/sigmaiq/backends/microsoft365defender/microsoft365defender.py
--rw-r--r--   0        0        0       48 2023-06-20 15:33:58.531341 sigmaiq-0.1.1/sigmaiq/backends/opensearch/__init__.py
--rw-r--r--   0        0        0      601 2023-06-20 15:33:58.535341 sigmaiq-0.1.1/sigmaiq/backends/opensearch/opensearch.py
--rw-r--r--   0        0        0       41 2023-06-20 15:33:58.535341 sigmaiq-0.1.1/sigmaiq/backends/qradar/__init__.py
--rw-r--r--   0        0        0      490 2023-06-20 15:33:58.535341 sigmaiq-0.1.1/sigmaiq/backends/qradar/qradar.py
--rw-r--r--   0        0        0       51 2023-06-20 15:33:58.535341 sigmaiq-0.1.1/sigmaiq/backends/sentinelone/__init__.py
--rw-r--r--   0        0        0      787 2023-06-20 15:33:58.535341 sigmaiq-0.1.1/sigmaiq/backends/sentinelone/sentinelone.py
--rw-r--r--   0        0        0       39 2023-06-20 15:33:58.535341 sigmaiq-0.1.1/sigmaiq/backends/sigma/__init__.py
--rw-r--r--   0        0        0     3505 2023-06-20 15:33:58.535341 sigmaiq-0.1.1/sigmaiq/backends/sigma/sigma.py
--rw-r--r--   0        0        0    11764 2023-06-20 15:33:58.535341 sigmaiq-0.1.1/sigmaiq/backends/sigmaiq_abstract_backend.py
--rw-r--r--   0        0        0       40 2023-06-20 15:33:58.535341 sigmaiq-0.1.1/sigmaiq/backends/splunk/__init__.py
--rw-r--r--   0        0        0     1557 2023-06-20 15:33:58.535341 sigmaiq-0.1.1/sigmaiq/backends/splunk/savedsearches_template.txt
--rw-r--r--   0        0        0     3067 2023-06-20 15:33:58.535341 sigmaiq-0.1.1/sigmaiq/backends/splunk/splunk.py
--rw-r--r--   0        0        0       37 2023-06-20 15:33:58.535341 sigmaiq-0.1.1/sigmaiq/backends/stix/__init__.py
--rw-r--r--   0        0        0      432 2023-06-20 15:33:58.535341 sigmaiq-0.1.1/sigmaiq/backends/stix/stix.py
--rw-r--r--   0        0        0     1327 2023-06-20 15:33:58.535341 sigmaiq-0.1.1/sigmaiq/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-20 15:33:58.535341 sigmaiq-0.1.1/sigmaiq/pipelines/__init__.py
--rw-r--r--   0        0        0      133 2023-06-20 15:33:58.535341 sigmaiq-0.1.1/sigmaiq/pipelines/splunk_windows_audit/__init__.py
--rw-r--r--   0        0        0      793 2023-06-20 15:33:58.535341 sigmaiq-0.1.1/sigmaiq/pipelines/splunk_windows_audit/splunk_wineventlog.py
--rw-r--r--   0        0        0    11008 2023-06-20 15:33:58.535341 sigmaiq-0.1.1/sigmaiq/sigmaiq_backend_factory.py
--rw-r--r--   0        0        0    17697 2023-06-20 15:33:58.535341 sigmaiq-0.1.1/sigmaiq/sigmaiq_pipeline_factory.py
--rw-r--r--   0        0        0    24970 1970-01-01 00:00:00.000000 sigmaiq-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/LICENSE
+-rw-r--r--   0        0        0    23477 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/README.md
+-rw-r--r--   0        0        0     1434 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2964 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/.gitignore
+-rw-r--r--   0        0        0      131 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/__init__.py
+-rw-r--r--   0        0        0       51 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/carbonblack/__init__.py
+-rw-r--r--   0        0        0      802 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/carbonblack/carbonblack.py
+-rw-r--r--   0        0        0       47 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/cortexxdr/__init__.py
+-rw-r--r--   0        0        0      732 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/cortexxdr/cortexxdr.py
+-rw-r--r--   0        0        0       57 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/crowdstrike/__init__.py
+-rw-r--r--   0        0        0      394 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/crowdstrike/crowdstrike.py
+-rw-r--r--   0        0        0       55 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/elasticsearch/__init__.py
+-rw-r--r--   0        0        0      520 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/elasticsearch/elasticsearch.py
+-rw-r--r--   0        0        0       48 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/insightidr/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/insightidr/insightidr.py
+-rw-r--r--   0        0        0       36 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/loki/__init__.py
+-rw-r--r--   0        0        0      437 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/loki/loki.py
+-rw-r--r--   0        0        0       69 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/microsoft365defender/__init__.py
+-rw-r--r--   0        0        0      397 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/microsoft365defender/microsoft365defender.py
+-rw-r--r--   0        0        0       48 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/opensearch/__init__.py
+-rw-r--r--   0        0        0      601 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/opensearch/opensearch.py
+-rw-r--r--   0        0        0       41 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/qradar/__init__.py
+-rw-r--r--   0        0        0      490 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/qradar/qradar.py
+-rw-r--r--   0        0        0       51 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/sentinelone/__init__.py
+-rw-r--r--   0        0        0      787 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/sentinelone/sentinelone.py
+-rw-r--r--   0        0        0       39 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/sigma/__init__.py
+-rw-r--r--   0        0        0     3505 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/sigma/sigma.py
+-rw-r--r--   0        0        0    11764 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/sigmaiq_abstract_backend.py
+-rw-r--r--   0        0        0       40 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/splunk/__init__.py
+-rw-r--r--   0        0        0     1557 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/splunk/savedsearches_template.txt
+-rw-r--r--   0        0        0     3154 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/splunk/splunk.py
+-rw-r--r--   0        0        0       37 2023-07-21 17:34:19.024881 sigmaiq-0.2.0/sigmaiq/backends/stix/__init__.py
+-rw-r--r--   0        0        0      432 2023-07-21 17:34:19.028881 sigmaiq-0.2.0/sigmaiq/backends/stix/stix.py
+-rw-r--r--   0        0        0     1327 2023-07-21 17:34:19.028881 sigmaiq-0.2.0/sigmaiq/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-21 17:34:19.028881 sigmaiq-0.2.0/sigmaiq/pipelines/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-21 17:34:19.028881 sigmaiq-0.2.0/sigmaiq/pipelines/splunk_windows_audit/__init__.py
+-rw-r--r--   0        0        0      793 2023-07-21 17:34:19.028881 sigmaiq-0.2.0/sigmaiq/pipelines/splunk_windows_audit/splunk_wineventlog.py
+-rw-r--r--   0        0        0    11241 2023-07-21 17:34:19.028881 sigmaiq-0.2.0/sigmaiq/sigmaiq_backend_factory.py
+-rw-r--r--   0        0        0    17980 2023-07-21 17:34:19.028881 sigmaiq-0.2.0/sigmaiq/sigmaiq_pipeline_factory.py
+-rw-r--r--   0        0        0    25081 1970-01-01 00:00:00.000000 sigmaiq-0.2.0/PKG-INFO
```

### Comparing `sigmaiq-0.1.1/LICENSE` & `sigmaiq-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.1.1/README.md` & `sigmaiq-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.1.1/pyproject.toml` & `sigmaiq-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SigmAIQ"
-version = "0.1.1"
+version = "0.2.0"
 description = "Wrapper and tools for pySigma and Sigma rules"
 authors = ["Stephen Lincoln <stephen.lincoln@attackiq.com>", "AttackIQ <support@attackiq.com>"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)",
@@ -18,30 +18,32 @@
 packages = [
     { include = "sigmaiq" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pysigma = "0.9.11"
-pysigma-backend-carbonblack = "^0.1.2"
-pysigma-backend-elasticsearch = "^1.0.3"
+pysigma-backend-carbonblack = "^0.1.4"
+pysigma-backend-elasticsearch = "^1.0.5"
 pysigma-backend-insightidr = "^0.2.1"
 pysigma-backend-loki = "^0.9.1"
 pysigma-backend-microsoft365defender = "^0.2.0"
 pysigma-backend-opensearch = "^1.0.0"
-pysigma-backend-qradar-aql = "^0.1.3"
-pysigma-backend-sentinelone = "^0.1.1"
+pysigma-backend-qradar-aql = "^0.1.4"
+pysigma-backend-sentinelone = "^0.1.2"
 pysigma-backend-splunk = "^1.0.2"
 pysigma-backend-stix = "^0.1.8"
 pysigma-pipeline-crowdstrike = "^1.0.0"
 pysigma-pipeline-sysmon = "^1.0.2"
 pysigma-pipeline-windows = "^1.1.0"
+importlib-resources = "^5.13.0"
+pysigma-backend-cortexxdr = "^0.1.0"
 
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.3.2"
+pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sigmaiq-0.1.1/sigmaiq/.gitignore` & `sigmaiq-0.2.0/sigmaiq/.gitignore`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.1.1/sigmaiq/backends/carbonblack/carbonblack.py` & `sigmaiq-0.2.0/sigmaiq/backends/carbonblack/carbonblack.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.1.1/sigmaiq/backends/elasticsearch/elasticsearch.py` & `sigmaiq-0.2.0/sigmaiq/backends/elasticsearch/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.1.1/sigmaiq/backends/opensearch/opensearch.py` & `sigmaiq-0.2.0/sigmaiq/backends/opensearch/opensearch.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.1.1/sigmaiq/backends/sentinelone/sentinelone.py` & `sigmaiq-0.2.0/sigmaiq/backends/sentinelone/sentinelone.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.1.1/sigmaiq/backends/sigma/sigma.py` & `sigmaiq-0.2.0/sigmaiq/backends/sigma/sigma.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.1.1/sigmaiq/backends/sigmaiq_abstract_backend.py` & `sigmaiq-0.2.0/sigmaiq/backends/sigmaiq_abstract_backend.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.1.1/sigmaiq/backends/splunk/savedsearches_template.txt` & `sigmaiq-0.2.0/sigmaiq/backends/splunk/savedsearches_template.txt`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.1.1/sigmaiq/backends/splunk/splunk.py` & `sigmaiq-0.2.0/sigmaiq/backends/splunk/splunk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from sigma.backends.splunk import SplunkBackend
 from sigma.rule import SigmaRule
 from sigma.collection import SigmaCollection
 from sigmaiq.backends.sigmaiq_abstract_backend import AbstractGenericSigmAIQBackendClass
-from copy import copy
+from copy import copy, deepcopy
 import re
+from importlib_resources import files
+
+SAVEDSEARCHES_TEMPLATE = files('sigmaiq.backends.splunk').joinpath('savedsearches_template.txt').read_text()
 
 
 class SigmAIQSplunkBackend(AbstractGenericSigmAIQBackendClass, SplunkBackend):
     """SigmAIQ backend interface for the pySigma Splunk Backend library to translate a SigmaRule object
     to a Splunk search query"""
 
     custom_formats = {'stanza': 'Enterprise Security savedsearches.conf stanza'}
@@ -44,16 +47,15 @@
             replacements = {'%TITLE_PLACEHOLDER%': title,
                             '%MITRE_ATTACK_PLACEHOLDER%': f'{tags}',
                             '%NOTABLE_TITLE_PLACEHOLDER%': title,
                             '%DRILLDOWN_TITLE_PLACEHOLDER%': title,
                             '%DRILLDOWN_SEARCH_PLACEHOLDER%': search,
                             '%SEARCH_PLACEHOLDER%': search}
 
-            with open('./sigmaiq/backends/splunk/savedsearches_template.txt', 'r') as fh:
-                stanza = fh.read()
+            stanza = deepcopy(SAVEDSEARCHES_TEMPLATE)
             for k, v in replacements.items():
                 stanza = stanza.replace(k, v)
             stanzas.append(stanza)
         return stanzas
 
     @staticmethod
     def _extract_mitre_tags(tags):
```

### Comparing `sigmaiq-0.1.1/sigmaiq/exceptions.py` & `sigmaiq-0.2.0/sigmaiq/exceptions.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.1.1/sigmaiq/pipelines/splunk_windows_audit/splunk_wineventlog.py` & `sigmaiq-0.2.0/sigmaiq/pipelines/splunk_windows_audit/splunk_wineventlog.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.1.1/sigmaiq/sigmaiq_backend_factory.py` & `sigmaiq-0.2.0/sigmaiq/sigmaiq_backend_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from sigmaiq.exceptions import InvalidSigmAIQBackend
 from sigmaiq.sigmaiq_pipeline_factory import SigmAIQPipelineResolver, SigmAIQPipeline
 
 # Backends
 from sigmaiq.backends.carbonblack import SigmAIQCarbonBlackBackend
 from sigmaiq.backends.crowdstrike import SigmAIQCrowdstrikeSplunkBackend
+from sigmaiq.backends.cortexxdr import SigmAIQCortexXDRBackend
 from sigmaiq.backends.elasticsearch import SigmAIQElasticsearchBackend
 from sigmaiq.backends.insightidr import SigmAIQInsightIDRBackend
 from sigmaiq.backends.loki import SigmAIQLokiBackend
 from sigmaiq.backends.microsoft365defender import SigmAIQMicrosoft365DefenderBackend
 from sigmaiq.backends.opensearch import SigmAIQOpensearchBackend
 from sigmaiq.backends.qradar import SigmAIQQRadarBackend
 from sigmaiq.backends.sentinelone import SigmAIQSentinelOneBackend
@@ -25,14 +26,15 @@
 
 ## Abstract
 from sigmaiq.backends.sigmaiq_abstract_backend import AbstractGenericSigmAIQBackendClass
 
 
 AVAILABLE_BACKENDS = {
         'carbonblack': 'Carbon Black EDR',
+        'cortexxdr': 'Palo Alto Cortex XDR',
         'crowdstrike_splunk': 'Crowdstrike Splunk Query',
         'elasticsearch': 'Elastic Elasticsearch SIEM',
         'insightidr': 'Rapid7 InsightIDR SIEM',
         'loki': 'Grafana Loki LogQL SIEM',
         'microsoft365defender': 'Microsoft 365 Defender Advanced Hunting Query (KQL)',
         'opensearch': 'OpenSearch Lucene',
         'qradar': 'IBM QRadar',
@@ -81,14 +83,17 @@
         """
         kwargs = {'processing_pipeline': self.processing_pipeline,
                   'output_format': self.output_format}
 
         # Carbon Black EDR (standard & enterprise)
         if self.backend == 'carbonblack':
             return SigmAIQCarbonBlackBackend(**kwargs)
+        # Cortex XDR, Palo Alto
+        if self.backend == "cortexxdr":
+            return SigmAIQCortexXDRBackend(**kwargs)
         # Crowdstrike Splunk Query
         if self.backend == "crowdstrike_splunk":
             pipelines = ["crowdstrike", kwargs['processing_pipeline']]
             kwargs['processing_pipeline'] = SigmAIQPipelineResolver(pipelines).process_pipelines()
             return SigmAIQCrowdstrikeSplunkBackend(**kwargs)
         # Elasticsearch
         if self.backend == 'elasticsearch':
```

### Comparing `sigmaiq-0.1.1/sigmaiq/sigmaiq_pipeline_factory.py` & `sigmaiq-0.2.0/sigmaiq/sigmaiq_pipeline_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
 ## AIQ
 from sigmaiq.pipelines.splunk_windows_audit import splunk_wineventlog_pipeline
 
 ## Carbon Black
 from sigma.pipelines.carbonblack import CarbonBlack_pipeline, CarbonBlackResponse_pipeline
 
+## Cortex XDR
+from sigma.pipelines.cortexxdr import CortexXDR_pipeline
+
 ## Crowdstrike
 from sigma.pipelines.crowdstrike import crowdstrike_fdr_pipeline
 
 ## Elasticsearch
 from sigma.pipelines.elasticsearch import (ecs_windows,
                                            ecs_windows_old,
                                            ecs_zeek_beats,
@@ -69,14 +72,20 @@
     },
     # CarbonBlack
     'carbonblack': {
         'description': 'Uses Carbon Black EDR field mappings',
         'pipeline': CarbonBlackResponse_pipeline(),
         'display_name': 'CB'
     },
+    # Cortex XDR, Palo Alto
+    'cortexxdr': {
+        'description': 'Uses Palo Alto Cortex XDR field mappings',
+        'pipeline': CortexXDR_pipeline(),
+        'display_name': 'Palo Alto Cortex XDR',
+    },
     'carbonblack_enterprise': {
         'description': 'Uses Carbon Black Enterprise EDR field mappings',
         'pipeline': CarbonBlack_pipeline(),
         'display_name': 'CB'
     },
     # Crowdstrike
     'crowdstrike': {
```

### Comparing `sigmaiq-0.1.1/PKG-INFO` & `sigmaiq-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: sigmaiq
-Version: 0.1.1
+Version: 0.2.0
 Summary: Wrapper and tools for pySigma and Sigma rules
 Author: Stephen Lincoln
 Author-email: stephen.lincoln@attackiq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
+Requires-Dist: importlib-resources (>=5.13.0,<6.0.0)
 Requires-Dist: pysigma (==0.9.11)
-Requires-Dist: pysigma-backend-carbonblack (>=0.1.2,<0.2.0)
-Requires-Dist: pysigma-backend-elasticsearch (>=1.0.3,<2.0.0)
+Requires-Dist: pysigma-backend-carbonblack (>=0.1.4,<0.2.0)
+Requires-Dist: pysigma-backend-cortexxdr (>=0.1.0,<0.2.0)
+Requires-Dist: pysigma-backend-elasticsearch (>=1.0.5,<2.0.0)
 Requires-Dist: pysigma-backend-insightidr (>=0.2.1,<0.3.0)
 Requires-Dist: pysigma-backend-loki (>=0.9.1,<0.10.0)
 Requires-Dist: pysigma-backend-microsoft365defender (>=0.2.0,<0.3.0)
 Requires-Dist: pysigma-backend-opensearch (>=1.0.0,<2.0.0)
-Requires-Dist: pysigma-backend-qradar-aql (>=0.1.3,<0.2.0)
-Requires-Dist: pysigma-backend-sentinelone (>=0.1.1,<0.2.0)
+Requires-Dist: pysigma-backend-qradar-aql (>=0.1.4,<0.2.0)
+Requires-Dist: pysigma-backend-sentinelone (>=0.1.2,<0.2.0)
 Requires-Dist: pysigma-backend-splunk (>=1.0.2,<2.0.0)
 Requires-Dist: pysigma-backend-stix (>=0.1.8,<0.2.0)
 Requires-Dist: pysigma-pipeline-crowdstrike (>=1.0.0,<2.0.0)
 Requires-Dist: pysigma-pipeline-sysmon (>=1.0.2,<2.0.0)
 Requires-Dist: pysigma-pipeline-windows (>=1.1.0,<2.0.0)
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,27 +1,29 @@
-Metadata-Version: 2.1 Name: sigmaiq Version: 0.1.1 Summary: Wrapper and tools
+Metadata-Version: 2.1 Name: sigmaiq Version: 0.2.0 Summary: Wrapper and tools
 for pySigma and Sigma rules Author: Stephen Lincoln Author-email:
 stephen.lincoln@attackiq.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2
 (LGPLv2) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Security Requires-
-Dist: pysigma (==0.9.11) Requires-Dist: pysigma-backend-carbonblack
-(>=0.1.2,<0.2.0) Requires-Dist: pysigma-backend-elasticsearch (>=1.0.3,<2.0.0)
-Requires-Dist: pysigma-backend-insightidr (>=0.2.1,<0.3.0) Requires-Dist:
-pysigma-backend-loki (>=0.9.1,<0.10.0) Requires-Dist: pysigma-backend-
-microsoft365defender (>=0.2.0,<0.3.0) Requires-Dist: pysigma-backend-opensearch
-(>=1.0.0,<2.0.0) Requires-Dist: pysigma-backend-qradar-aql (>=0.1.3,<0.2.0)
-Requires-Dist: pysigma-backend-sentinelone (>=0.1.1,<0.2.0) Requires-Dist:
-pysigma-backend-splunk (>=1.0.2,<2.0.0) Requires-Dist: pysigma-backend-stix
-(>=0.1.8,<0.2.0) Requires-Dist: pysigma-pipeline-crowdstrike (>=1.0.0,<2.0.0)
-Requires-Dist: pysigma-pipeline-sysmon (>=1.0.2,<2.0.0) Requires-Dist: pysigma-
-pipeline-windows (>=1.1.0,<2.0.0) Description-Content-Type: text/markdown
+Dist: importlib-resources (>=5.13.0,<6.0.0) Requires-Dist: pysigma (==0.9.11)
+Requires-Dist: pysigma-backend-carbonblack (>=0.1.4,<0.2.0) Requires-Dist:
+pysigma-backend-cortexxdr (>=0.1.0,<0.2.0) Requires-Dist: pysigma-backend-
+elasticsearch (>=1.0.5,<2.0.0) Requires-Dist: pysigma-backend-insightidr
+(>=0.2.1,<0.3.0) Requires-Dist: pysigma-backend-loki (>=0.9.1,<0.10.0)
+Requires-Dist: pysigma-backend-microsoft365defender (>=0.2.0,<0.3.0) Requires-
+Dist: pysigma-backend-opensearch (>=1.0.0,<2.0.0) Requires-Dist: pysigma-
+backend-qradar-aql (>=0.1.4,<0.2.0) Requires-Dist: pysigma-backend-sentinelone
+(>=0.1.2,<0.2.0) Requires-Dist: pysigma-backend-splunk (>=1.0.2,<2.0.0)
+Requires-Dist: pysigma-backend-stix (>=0.1.8,<0.2.0) Requires-Dist: pysigma-
+pipeline-crowdstrike (>=1.0.0,<2.0.0) Requires-Dist: pysigma-pipeline-sysmon
+(>=1.0.2,<2.0.0) Requires-Dist: pysigma-pipeline-windows (>=1.1.0,<2.0.0)
+Description-Content-Type: text/markdown
                                   [AttackIQ]
                 ****** SigmAIQ: pySigma Wrapper & Utils ******
 ![Tests](https://github.com/AttackIQ/SigmAIQ/actions/workflows/test.yml/
 badge.svg) ![Coverage Badge](https://img.shields.io/endpoint?url=https://
 gist.githubusercontent.com/slincoln-aiq/f6d72f7ec2b300546a114fd80d371f7e/raw/
 slincoln-aiq-SigmAIQ.json) ![Status](https://img.shields.io/badge/Status-pre--
 release-orange) SigmAIQ is a wrapper for [pySigma](https://github.com/SigmaHQ/
```

