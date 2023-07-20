# Comparing `tmp/grafana-wtf-0.8.1.tar.gz` & `tmp/grafana-wtf-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grafana-wtf-0.8.1.tar", last modified: Wed May  8 18:26:13 2019, max compression
+gzip compressed data, was "dist/grafana-wtf-0.9.0.tar", last modified: Wed Nov  6 01:46:33 2019, max compression
```

## Comparing `grafana-wtf-0.8.1.tar` & `grafana-wtf-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 amo        (502) staff       (20)        0 2019-05-08 18:26:13.000000 grafana-wtf-0.8.1/
--rw-r--r--   0 amo        (502) staff       (20)     1717 2019-05-08 18:13:24.000000 grafana-wtf-0.8.1/CHANGES.rst
--rw-r--r--   0 amo        (502) staff       (20)    34520 2018-12-07 12:53:22.000000 grafana-wtf-0.8.1/LICENSE
--rw-r--r--   0 amo        (502) staff       (20)      136 2019-01-22 19:55:49.000000 grafana-wtf-0.8.1/MANIFEST.in
--rw-r--r--   0 amo        (502) staff       (20)     4749 2019-05-08 18:26:13.000000 grafana-wtf-0.8.1/PKG-INFO
--rw-r--r--   0 amo        (502) staff       (20)     2295 2019-05-07 21:39:28.000000 grafana-wtf-0.8.1/README.rst
-drwxr-xr-x   0 amo        (502) staff       (20)        0 2019-05-08 18:26:13.000000 grafana-wtf-0.8.1/grafana_wtf/
--rw-r--r--   0 amo        (502) staff       (20)      103 2019-05-08 18:26:04.000000 grafana-wtf-0.8.1/grafana_wtf/__init__.py
--rw-r--r--   0 amo        (502) staff       (20)     6482 2019-05-08 18:11:16.000000 grafana-wtf-0.8.1/grafana_wtf/commands.py
--rw-r--r--   0 amo        (502) staff       (20)     9274 2019-05-08 18:10:50.000000 grafana-wtf-0.8.1/grafana_wtf/core.py
--rw-r--r--   0 amo        (502) staff       (20)      472 2019-02-25 22:15:09.000000 grafana-wtf-0.8.1/grafana_wtf/replacements.py
--rw-r--r--   0 amo        (502) staff       (20)     4341 2019-05-08 00:22:14.000000 grafana-wtf-0.8.1/grafana_wtf/report.py
--rw-r--r--   0 amo        (502) staff       (20)     2943 2019-05-08 05:49:08.000000 grafana-wtf-0.8.1/grafana_wtf/util.py
-drwxr-xr-x   0 amo        (502) staff       (20)        0 2019-05-08 18:26:13.000000 grafana-wtf-0.8.1/grafana_wtf.egg-info/
--rw-r--r--   0 amo        (502) staff       (20)     4749 2019-05-08 18:26:13.000000 grafana-wtf-0.8.1/grafana_wtf.egg-info/PKG-INFO
--rw-r--r--   0 amo        (502) staff       (20)      435 2019-05-08 18:26:13.000000 grafana-wtf-0.8.1/grafana_wtf.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (502) staff       (20)        1 2019-05-08 18:26:13.000000 grafana-wtf-0.8.1/grafana_wtf.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (502) staff       (20)       58 2019-05-08 18:26:13.000000 grafana-wtf-0.8.1/grafana_wtf.egg-info/entry_points.txt
--rw-r--r--   0 amo        (502) staff       (20)        1 2019-01-22 19:59:46.000000 grafana-wtf-0.8.1/grafana_wtf.egg-info/not-zip-safe
--rw-r--r--   0 amo        (502) staff       (20)      185 2019-05-08 18:26:13.000000 grafana-wtf-0.8.1/grafana_wtf.egg-info/requires.txt
--rw-r--r--   0 amo        (502) staff       (20)       12 2019-05-08 18:26:13.000000 grafana-wtf-0.8.1/grafana_wtf.egg-info/top_level.txt
--rw-r--r--   0 amo        (502) staff       (20)       38 2019-05-08 18:26:13.000000 grafana-wtf-0.8.1/setup.cfg
--rw-r--r--   0 amo        (502) staff       (20)     2592 2019-05-08 18:26:04.000000 grafana-wtf-0.8.1/setup.py
+drwxr-xr-x   0 amo        (502) staff       (20)        0 2019-11-06 01:46:33.000000 grafana-wtf-0.9.0/
+-rw-r--r--   0 amo        (502) staff       (20)     1935 2019-11-06 01:45:34.000000 grafana-wtf-0.9.0/CHANGES.rst
+-rw-r--r--   0 amo        (502) staff       (20)    34520 2018-12-07 12:53:22.000000 grafana-wtf-0.9.0/LICENSE
+-rw-r--r--   0 amo        (502) staff       (20)      136 2019-01-22 19:55:49.000000 grafana-wtf-0.9.0/MANIFEST.in
+-rw-r--r--   0 amo        (502) staff       (20)     4749 2019-11-06 01:46:33.000000 grafana-wtf-0.9.0/PKG-INFO
+-rw-r--r--   0 amo        (502) staff       (20)     2295 2019-05-07 21:39:28.000000 grafana-wtf-0.9.0/README.rst
+drwxr-xr-x   0 amo        (502) staff       (20)        0 2019-11-06 01:46:33.000000 grafana-wtf-0.9.0/grafana_wtf/
+-rw-r--r--   0 amo        (502) staff       (20)      103 2019-11-06 01:46:25.000000 grafana-wtf-0.9.0/grafana_wtf/__init__.py
+-rw-r--r--   0 amo        (502) staff       (20)     7453 2019-11-06 01:44:32.000000 grafana-wtf-0.9.0/grafana_wtf/commands.py
+-rw-r--r--   0 amo        (502) staff       (20)    10587 2019-11-06 01:45:00.000000 grafana-wtf-0.9.0/grafana_wtf/core.py
+-rw-r--r--   0 amo        (502) staff       (20)      472 2019-02-25 22:15:09.000000 grafana-wtf-0.9.0/grafana_wtf/replacements.py
+-rw-r--r--   0 amo        (502) staff       (20)     4341 2019-05-08 00:22:14.000000 grafana-wtf-0.9.0/grafana_wtf/report.py
+-rw-r--r--   0 amo        (502) staff       (20)     3172 2019-11-06 00:01:06.000000 grafana-wtf-0.9.0/grafana_wtf/util.py
+drwxr-xr-x   0 amo        (502) staff       (20)        0 2019-11-06 01:46:33.000000 grafana-wtf-0.9.0/grafana_wtf.egg-info/
+-rw-r--r--   0 amo        (502) staff       (20)     4749 2019-11-06 01:46:33.000000 grafana-wtf-0.9.0/grafana_wtf.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (502) staff       (20)      435 2019-11-06 01:46:33.000000 grafana-wtf-0.9.0/grafana_wtf.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (502) staff       (20)        1 2019-11-06 01:46:33.000000 grafana-wtf-0.9.0/grafana_wtf.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (502) staff       (20)       58 2019-11-06 01:46:33.000000 grafana-wtf-0.9.0/grafana_wtf.egg-info/entry_points.txt
+-rw-r--r--   0 amo        (502) staff       (20)        1 2019-01-22 19:59:46.000000 grafana-wtf-0.9.0/grafana_wtf.egg-info/not-zip-safe
+-rw-r--r--   0 amo        (502) staff       (20)      184 2019-11-06 01:46:33.000000 grafana-wtf-0.9.0/grafana_wtf.egg-info/requires.txt
+-rw-r--r--   0 amo        (502) staff       (20)       12 2019-11-06 01:46:33.000000 grafana-wtf-0.9.0/grafana_wtf.egg-info/top_level.txt
+-rw-r--r--   0 amo        (502) staff       (20)       38 2019-11-06 01:46:33.000000 grafana-wtf-0.9.0/setup.cfg
+-rw-r--r--   0 amo        (502) staff       (20)     2591 2019-11-06 01:46:25.000000 grafana-wtf-0.9.0/setup.py
```

### Comparing `grafana-wtf-0.8.1/CHANGES.rst` & `grafana-wtf-0.9.0/CHANGES.rst`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 grafana-wtf changelog
 #####################
 
 
 in progress
 ===========
 
+2019-11-06 0.9.0
+================
+- Add option ``--select-dashboard`` to scan specific dashboards by list of uids
+- Bump dependent modules to their most recent versions
+- Add option to replace string within dashboard
+
 2019-05-08 0.8.1
 ================
 - Compensate for leading slash in API URL inserted by ``grafana_api``. Thanks, `@jangaraj`_.
 
 2019-05-08 0.8.0
 ================
 - Add "--http-logging" option
```

### Comparing `grafana-wtf-0.8.1/LICENSE` & `grafana-wtf-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grafana-wtf-0.8.1/PKG-INFO` & `grafana-wtf-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana-wtf
-Version: 0.8.1
+Version: 0.9.0
 Summary: Grep through all Grafana entities in the spirit of git-wtf
 Home-page: https://github.com/daq-tools/grafana-wtf
 Author: Andreas Motl
 Author-email: andreas@hiveeyes.org
 License: AGPL 3, EUPL 1.2
 Description: .. image:: https://img.shields.io/badge/Python-3.6-green.svg
             :target: https://pypi.org/project/grafana-wtf/
```

### Comparing `grafana-wtf-0.8.1/README.rst` & `grafana-wtf-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `grafana-wtf-0.8.1/grafana_wtf/commands.py` & `grafana-wtf-0.9.0/grafana_wtf/commands.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,30 +8,33 @@
 from operator import itemgetter
 from collections import OrderedDict
 from docopt import docopt, DocoptExit
 
 from grafana_wtf import __appname__, __version__
 from grafana_wtf.core import GrafanaSearch
 from grafana_wtf.report import WtfReport
-from grafana_wtf.util import normalize_options, setup_logging, configure_http_logging
+from grafana_wtf.util import normalize_options, setup_logging, configure_http_logging, read_list
 
 log = logging.getLogger(__name__)
 
 
 def run():
     """
     Usage:
-      grafana-wtf [options] find [<expression>]
+      grafana-wtf [options] find [<search-expression>]
+      grafana-wtf [options] replace <search-expression> <replacement>
       grafana-wtf [options] log [<dashboard_uid>] [--number=<count>]
       grafana-wtf --version
       grafana-wtf (-h | --help)
 
     Options:
       --grafana-url=<grafana-url>       URL to Grafana instance
       --grafana-token=<grafana-token>   Grafana API Key token
+      --select-dashboard=<uuid>         Restrict operation to dashboard by UID.
+                                        Can be a list of comma-separated dashboard UIDs.
       --format=<format>                 Output format. [default: json]
       --cache-ttl=<cache-ttl>           Time-to-live for the request cache in seconds. [default: 300]
       --drop-cache                      Drop cache before requesting resources
       --concurrency=<concurrency>       Run multiple requests in parallel. [default: 5]
       --verbose                         Enable verbose mode
       --version                         Show version information
       --debug                           Enable debug messages
@@ -58,14 +61,22 @@
 
       # Use infinite cache expiration time, essentially caching forever.
       grafana-wtf find '#299c46' --cache-ttl=inf
 
       # Set cache expiration time to zero, essentially disabling the cache.
       grafana-wtf find geohash --cache-ttl=0
 
+      # Search keyword within list of specific dashboards.
+      grafana-wtf --select-dashboard=_JJ22OZZk,5iGTqNWZk find grafana-worldmap
+
+    Replace examples:
+
+      # Replace string within specific dashboard.
+      grafana-wtf --select-dashboard=_JJ22OZZk replace grafana-worldmap-panel grafana-map-panel
+
     History examples:
 
       # Display 50 most recent changes across all dashboards.
       grafana-wtf log --number=50
 
       # Display 5 most recent changes for specific dashboard.
       grafana-wtf log NP0wTOtmk --number=5
@@ -111,22 +122,35 @@
         raise DocoptExit('No Grafana URL given. Please use "--grafana-url" option or environment variable "GRAFANA_URL".')
 
     engine = GrafanaSearch(grafana_url, grafana_token)
     engine.enable_cache(expire_after=cache_ttl, drop_cache=options['drop-cache'])
     engine.enable_concurrency(int(options['concurrency']))
     engine.setup()
 
-    if options.find:
-        result = engine.search(options.expression)
+    if options.find or options.replace:
+
+        if options.select_dashboard:
+            # Restrict scan to list of dashboards.
+            dashboard_uids = read_list(options.select_dashboard)
+            engine.scan_dashboards(dashboard_uids)
+
+        else:
+            # Scan everything.
+            engine.scan()
+
+        result = engine.search(options.search_expression)
         #print(json.dumps(result, indent=4))
 
         report = WtfReport(grafana_url, verbose=options.verbose)
-        report.display(options.expression, result)
+        report.display(options.search_expression, result)
+
+    if options.replace:
+        engine.replace(options.search_expression, options.replacement)
 
-    elif options.log:
+    if options.log:
         engine.scan_dashboards()
         #print(options.dashboard_uid)
         entries = engine.log(dashboard_uid=options.dashboard_uid)
         entries = sorted(entries, key=itemgetter('datetime'), reverse=True)
 
         if options.number is not None:
             count = int(options.number)
```

### Comparing `grafana-wtf-0.8.1/grafana_wtf/core.py` & `grafana-wtf-0.9.0/grafana_wtf/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # (c) 2019 Andreas Motl <andreas@hiveeyes.org>
 # License: GNU Affero General Public License, Version 3
+import json
 import colored
 import logging
 import asyncio
 import requests
 import requests_cache
 from tqdm import tqdm
 from munch import Munch, munchify
@@ -80,28 +81,39 @@
 
     def start_progressbar(self, total):
         if self.progressbar:
             self.taqadum = tqdm(total=total)
 
     def search(self, expression):
         log.info('Searching Grafana at "{}" for expression "{}"'.format(self.grafana_url, expression))
-        self.scan()
 
         results = Munch(datasources=[], dashboard_list=[], dashboards=[])
 
         # Check datasources
         log.info('Searching data sources')
         self.search_items(expression, self.data.datasources, results.datasources)
 
         # Check dashboards
         log.info('Searching dashboards')
         self.search_items(expression, self.data.dashboards, results.dashboards)
 
         return results
 
+    def replace(self, expression, replacement):
+        log.info(f'Replacing "{expression}" by "{replacement}" within Grafana at "{self.grafana_url}"')
+        for dashboard in self.data.dashboards:
+            payload_before = json.dumps(dashboard)
+            payload_after = payload_before.replace(expression, replacement)
+            if payload_before == payload_after:
+                log.info(f'No replacements for dashboard with uid "{dashboard.dashboard.uid}"')
+                continue
+            dashboard_new = json.loads(payload_after)
+            dashboard_new['message'] = f'grafana-wtf: Replaced "{expression}" by "{replacement}"'
+            self.grafana.dashboard.update_dashboard(dashboard=dashboard_new)
+
     def log(self, dashboard_uid=None):
         if dashboard_uid:
             what = 'Grafana dashboard "{}"'.format(dashboard_uid)
         else:
             what = 'multiple Grafana dashboards'
         log.info('Aggregating edit history for {what} at {url}'.format(what=what, url=self.grafana_url))
 
@@ -148,58 +160,71 @@
 
         self.scan_datasources()
         self.scan_dashboards()
 
     def scan_datasources(self):
         log.info('Scanning datasources')
         try:
-            self.data.datasources = self.grafana.datasource.list_datasources()
+            self.data.datasources = munchify(self.grafana.datasource.list_datasources())
             log.info('Found {} data sources'.format(len(self.data.datasources)))
         except GrafanaClientError as ex:
             message = '{name}: {ex}'.format(name=ex.__class__.__name__, ex=ex)
             log.error(self.get_red_message(message))
             if isinstance(ex, GrafanaUnauthorizedError):
                 log.error(self.get_red_message('Please use --grafana-token or GRAFANA_TOKEN '
                                                'for authenticating with Grafana'))
 
     @staticmethod
     def get_red_message(message):
         return colored.stylize(message, colored.fg("red") + colored.attr("bold"))
 
-    def scan_dashboards(self):
+    def scan_dashboards(self, dashboard_uids=None):
 
         log.info('Scanning dashboards')
         try:
-            self.data.dashboard_list = self.grafana.search.search_dashboards(limit=5000)
+            if dashboard_uids is not None:
+                for uid in dashboard_uids:
+                    log.info(f'Fetching dashboard by uid {uid}')
+                    try:
+                        dashboard = self.grafana.dashboard.get_dashboard(uid)
+                        self.data.dashboard_list.append(dashboard['dashboard'])
+                    except GrafanaClientError as ex:
+                        self.handle_grafana_error(ex)
+                        continue
+            else:
+                self.data.dashboard_list = self.grafana.search.search_dashboards(limit=5000)
             log.info('Found {} dashboards'.format(len(self.data.dashboard_list)))
 
         except GrafanaClientError as ex:
-            message = '{name}: {ex}'.format(name=ex.__class__.__name__, ex=ex)
-            message = colored.stylize(message, colored.fg("red") + colored.attr("bold"))
-            log.error(self.get_red_message(message))
-            if isinstance(ex, GrafanaUnauthorizedError):
-                log.error(self.get_red_message('Please use --grafana-token or GRAFANA_TOKEN '
-                                               'for authenticating with Grafana'))
+            self.handle_grafana_error(ex)
             return
 
         if self.progressbar:
             self.start_progressbar(len(self.data.dashboard_list))
 
         if self.concurrency is None or self.concurrency <= 1:
             self.fetch_dashboards()
         else:
             self.fetch_dashboards_parallel()
 
         if self.progressbar:
             self.taqadum.close()
 
+    def handle_grafana_error(self, ex):
+        message = '{name}: {ex}'.format(name=ex.__class__.__name__, ex=ex)
+        message = colored.stylize(message, colored.fg("red") + colored.attr("bold"))
+        log.error(self.get_red_message(message))
+        if isinstance(ex, GrafanaUnauthorizedError):
+            log.error(self.get_red_message('Please use --grafana-token or GRAFANA_TOKEN '
+                                           'for authenticating with Grafana'))
+
     def fetch_dashboard(self, dashboard_info):
         log.debug(f'Fetching dashboard "{dashboard_info["title"]}" ({dashboard_info["uid"]})')
         dashboard = self.grafana.dashboard.get_dashboard(dashboard_info['uid'])
-        self.data.dashboards.append(dashboard)
+        self.data.dashboards.append(munchify(dashboard))
         if self.taqadum is not None:
             self.taqadum.update(1)
 
     def fetch_dashboards(self):
         log.info('Fetching dashboards one by one')
         results = self.data.dashboard_list
         for dashboard_info in results:
```

### Comparing `grafana-wtf-0.8.1/grafana_wtf/report.py` & `grafana-wtf-0.9.0/grafana_wtf/report.py`

 * *Files identical despite different names*

### Comparing `grafana-wtf-0.8.1/grafana_wtf/util.py` & `grafana-wtf-0.9.0/grafana_wtf/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,21 +40,30 @@
     normalized = {}
     for key, value in options.items():
 
         # Add primary variant.
         key = key.strip('--<>')
         normalized[key] = value
 
-        # Add second variant.
+        # Add secondary variant.
         key = key.replace('-', '_')
         normalized[key] = value
 
     return munchify(normalized)
 
 
+def read_list(data, separator=u','):
+    if data is None:
+        return []
+    result = list(map(lambda x: x.strip(), data.split(separator)))
+    if len(result) == 1 and not result[0]:
+        result = []
+    return result
+
+
 class JsonPathFinder:
 
     def __init__(self):
         self.jsonpath_expr = parse('$..*')
         self.non_leaf_nodes = ('rows', 'panels', 'targets', 'tags', 'groupBy', 'list', 'links')
         self.scalars = (str, int, float, list)
```

### Comparing `grafana-wtf-0.8.1/grafana_wtf.egg-info/PKG-INFO` & `grafana-wtf-0.9.0/grafana_wtf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana-wtf
-Version: 0.8.1
+Version: 0.9.0
 Summary: Grep through all Grafana entities in the spirit of git-wtf
 Home-page: https://github.com/daq-tools/grafana-wtf
 Author: Andreas Motl
 Author-email: andreas@hiveeyes.org
 License: AGPL 3, EUPL 1.2
 Description: .. image:: https://img.shields.io/badge/Python-3.6-green.svg
             :target: https://pypi.org/project/grafana-wtf/
```

### Comparing `grafana-wtf-0.8.1/setup.py` & `grafana-wtf-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 README = open(os.path.join(here, 'README.rst')).read()
 
 requires = [
 
     # Core
-    'six==1.12.0',
+    'six==1.13.0',
     'docopt==0.6.2',
-    'munch==2.3.2',
-    'tqdm==4.31.1',
+    'munch==2.5.0',
+    'tqdm==4.37.0',
 
     # Grafana
-    'requests==2.21.0',
-    'grafana-api==0.7.3',
+    'requests==2.22.0',
+    'grafana-api==0.9.1',
     'jsonpath-rw==1.4.0',
 
     # Caching
-    'requests-cache==0.5.0',
+    'requests-cache==0.5.2',
 
     # Output
-    'tabulate==0.8.3',
-    'colored==1.3.93',
-    'Pygments==2.3.1',
+    'tabulate==0.8.5',
+    'colored==1.4.0',
+    'Pygments==2.4.2',
 
 ]
 
 extras = {'test': []}
 
 setup(name='grafana-wtf',
-      version='0.8.1',
+      version='0.9.0',
       description='Grep through all Grafana entities in the spirit of git-wtf',
       long_description=README,
       license="AGPL 3, EUPL 1.2",
       classifiers=[
         "Programming Language :: Python",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)",
```

