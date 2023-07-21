# Comparing `tmp/botocore-a-la-carte-wafv2-1.31.5.tar.gz` & `tmp/botocore-a-la-carte-wafv2-1.31.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-wafv2-1.31.5.tar", last modified: Wed Jul 19 02:44:19 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-wafv2-1.31.6.tar", last modified: Thu Jul 20 01:20:47 2023, max compression
```

## Comparing `botocore-a-la-carte-wafv2-1.31.5.tar` & `botocore-a-la-carte-wafv2-1.31.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:19.695570 botocore-a-la-carte-wafv2-1.31.5/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-19 02:44:19.000000 botocore-a-la-carte-wafv2-1.31.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-19 02:44:19.695570 botocore-a-la-carte-wafv2-1.31.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:19.695570 botocore-a-la-carte-wafv2-1.31.5/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:19.695570 botocore-a-la-carte-wafv2-1.31.5/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:19.695570 botocore-a-la-carte-wafv2-1.31.5/botocore/data/wafv2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:19.695570 botocore-a-la-carte-wafv2-1.31.5/botocore/data/wafv2/2019-07-29/
--rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-07-19 02:43:32.000000 botocore-a-la-carte-wafv2-1.31.5/botocore/data/wafv2/2019-07-29/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-19 02:43:32.000000 botocore-a-la-carte-wafv2-1.31.5/botocore/data/wafv2/2019-07-29/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-19 02:43:32.000000 botocore-a-la-carte-wafv2-1.31.5/botocore/data/wafv2/2019-07-29/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   447635 2023-07-19 02:43:32.000000 botocore-a-la-carte-wafv2-1.31.5/botocore/data/wafv2/2019-07-29/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:19.695570 botocore-a-la-carte-wafv2-1.31.5/botocore_a_la_carte_wafv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-19 02:44:19.000000 botocore-a-la-carte-wafv2-1.31.5/botocore_a_la_carte_wafv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-19 02:44:19.000000 botocore-a-la-carte-wafv2-1.31.5/botocore_a_la_carte_wafv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:44:19.000000 botocore-a-la-carte-wafv2-1.31.5/botocore_a_la_carte_wafv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 02:44:19.000000 botocore-a-la-carte-wafv2-1.31.5/botocore_a_la_carte_wafv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 02:44:19.695570 botocore-a-la-carte-wafv2-1.31.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-19 02:44:19.000000 botocore-a-la-carte-wafv2-1.31.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:47.330933 botocore-a-la-carte-wafv2-1.31.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-20 01:20:47.000000 botocore-a-la-carte-wafv2-1.31.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 01:20:47.326933 botocore-a-la-carte-wafv2-1.31.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:47.326933 botocore-a-la-carte-wafv2-1.31.6/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:47.326933 botocore-a-la-carte-wafv2-1.31.6/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:47.326933 botocore-a-la-carte-wafv2-1.31.6/botocore/data/wafv2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:47.326933 botocore-a-la-carte-wafv2-1.31.6/botocore/data/wafv2/2019-07-29/
+-rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-07-20 01:19:55.000000 botocore-a-la-carte-wafv2-1.31.6/botocore/data/wafv2/2019-07-29/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 01:19:55.000000 botocore-a-la-carte-wafv2-1.31.6/botocore/data/wafv2/2019-07-29/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 01:19:55.000000 botocore-a-la-carte-wafv2-1.31.6/botocore/data/wafv2/2019-07-29/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   449041 2023-07-20 01:19:55.000000 botocore-a-la-carte-wafv2-1.31.6/botocore/data/wafv2/2019-07-29/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:47.326933 botocore-a-la-carte-wafv2-1.31.6/botocore_a_la_carte_wafv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 01:20:47.000000 botocore-a-la-carte-wafv2-1.31.6/botocore_a_la_carte_wafv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-20 01:20:47.000000 botocore-a-la-carte-wafv2-1.31.6/botocore_a_la_carte_wafv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 01:20:47.000000 botocore-a-la-carte-wafv2-1.31.6/botocore_a_la_carte_wafv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 01:20:47.000000 botocore-a-la-carte-wafv2-1.31.6/botocore_a_la_carte_wafv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 01:20:47.330933 botocore-a-la-carte-wafv2-1.31.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-20 01:20:47.000000 botocore-a-la-carte-wafv2-1.31.6/setup.py
```

### Comparing `botocore-a-la-carte-wafv2-1.31.5/LICENSE.txt` & `botocore-a-la-carte-wafv2-1.31.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-wafv2-1.31.5/PKG-INFO` & `botocore-a-la-carte-wafv2-1.31.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-wafv2
-Version: 1.31.5
+Version: 1.31.6
 Summary: wafv2 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-wafv2-1.31.5/botocore/data/wafv2/2019-07-29/endpoint-rule-set-1.json` & `botocore-a-la-carte-wafv2-1.31.6/botocore/data/wafv2/2019-07-29/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-wafv2-1.31.5/botocore/data/wafv2/2019-07-29/service-2.json` & `botocore-a-la-carte-wafv2-1.31.6/botocore/data/wafv2/2019-07-29/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997054528031771%*

 * *Differences: {"'shapes'": "{'CookieMatchPattern': {'documentation': '<p>The filter to use to identify the "*

 * *             'subset of cookies to inspect in a web request. </p> <p>You must specify exactly one '*

 * *             'setting: either <code>All</code>, <code>IncludedCookies</code>, or '*

 * *             '<code>ExcludedCookies</code>.</p> <p>Example JSON: <code>"MatchPattern": { '*

 * *             '"IncludedCookies": [ "session-id-time", "session-id" ] }</code> </p>\'}, '*

 * *             "'Cookies': {'members': {'MatchPattern':  […]*

```diff
@@ -2143,15 +2143,15 @@
             "type": "list"
         },
         "ConsumedCapacity": {
             "min": 0,
             "type": "long"
         },
         "CookieMatchPattern": {
-            "documentation": "<p>The filter to use to identify the subset of cookies to inspect in a web request. </p> <p>You must specify exactly one setting: either <code>All</code>, <code>IncludedCookies</code>, or <code>ExcludedCookies</code>.</p> <p>Example JSON: <code>\"MatchPattern\": { \"IncludedCookies\": {\"KeyToInclude1\", \"KeyToInclude2\", \"KeyToInclude3\"} }</code> </p>",
+            "documentation": "<p>The filter to use to identify the subset of cookies to inspect in a web request. </p> <p>You must specify exactly one setting: either <code>All</code>, <code>IncludedCookies</code>, or <code>ExcludedCookies</code>.</p> <p>Example JSON: <code>\"MatchPattern\": { \"IncludedCookies\": [ \"session-id-time\", \"session-id\" ] }</code> </p>",
             "members": {
                 "All": {
                     "documentation": "<p>Inspect all cookies. </p>",
                     "shape": "All"
                 },
                 "ExcludedCookies": {
                     "documentation": "<p>Inspect only the cookies whose keys don't match any of the strings specified here. </p>",
@@ -2172,15 +2172,15 @@
             "min": 1,
             "type": "list"
         },
         "Cookies": {
             "documentation": "<p>Inspect the cookies in the web request. You can specify the parts of the cookies to inspect and you can narrow the set of cookies to inspect by including or excluding specific keys.</p> <p>This is used to indicate the web request component to inspect, in the <a>FieldToMatch</a> specification. </p> <p>Example JSON: <code>\"Cookies\": { \"MatchPattern\": { \"All\": {} }, \"MatchScope\": \"KEY\", \"OversizeHandling\": \"MATCH\" }</code> </p>",
             "members": {
                 "MatchPattern": {
-                    "documentation": "<p>The filter to use to identify the subset of cookies to inspect in a web request. </p> <p>You must specify exactly one setting: either <code>All</code>, <code>IncludedCookies</code>, or <code>ExcludedCookies</code>.</p> <p>Example JSON: <code>\"MatchPattern\": { \"IncludedCookies\": {\"KeyToInclude1\", \"KeyToInclude2\", \"KeyToInclude3\"} }</code> </p>",
+                    "documentation": "<p>The filter to use to identify the subset of cookies to inspect in a web request. </p> <p>You must specify exactly one setting: either <code>All</code>, <code>IncludedCookies</code>, or <code>ExcludedCookies</code>.</p> <p>Example JSON: <code>\"MatchPattern\": { \"IncludedCookies\": [ \"session-id-time\", \"session-id\" ] }</code> </p>",
                     "shape": "CookieMatchPattern"
                 },
                 "MatchScope": {
                     "documentation": "<p>The parts of the cookies to inspect with the rule inspection criteria. If you specify <code>All</code>, WAF inspects both keys and values. </p>",
                     "shape": "MapMatchScope"
                 },
                 "OversizeHandling": {
@@ -3883,15 +3883,15 @@
             },
             "type": "structure"
         },
         "HTTPVersion": {
             "type": "string"
         },
         "HeaderMatchPattern": {
-            "documentation": "<p>The filter to use to identify the subset of headers to inspect in a web request. </p> <p>You must specify exactly one setting: either <code>All</code>, <code>IncludedHeaders</code>, or <code>ExcludedHeaders</code>.</p> <p>Example JSON: <code>\"MatchPattern\": { \"ExcludedHeaders\": {\"KeyToExclude1\", \"KeyToExclude2\"} }</code> </p>",
+            "documentation": "<p>The filter to use to identify the subset of headers to inspect in a web request. </p> <p>You must specify exactly one setting: either <code>All</code>, <code>IncludedHeaders</code>, or <code>ExcludedHeaders</code>.</p> <p>Example JSON: <code>\"MatchPattern\": { \"ExcludedHeaders\": [ \"KeyToExclude1\", \"KeyToExclude2\" ] }</code> </p>",
             "members": {
                 "All": {
                     "documentation": "<p>Inspect all headers. </p>",
                     "shape": "All"
                 },
                 "ExcludedHeaders": {
                     "documentation": "<p>Inspect only the headers whose keys don't match any of the strings specified here. </p>",
@@ -3931,15 +3931,15 @@
         "HeaderValue": {
             "type": "string"
         },
         "Headers": {
             "documentation": "<p>Inspect all headers in the web request. You can specify the parts of the headers to inspect and you can narrow the set of headers to inspect by including or excluding specific keys.</p> <p>This is used to indicate the web request component to inspect, in the <a>FieldToMatch</a> specification. </p> <p>If you want to inspect just the value of a single header, use the <code>SingleHeader</code> <code>FieldToMatch</code> setting instead.</p> <p>Example JSON: <code>\"Headers\": { \"MatchPattern\": { \"All\": {} }, \"MatchScope\": \"KEY\", \"OversizeHandling\": \"MATCH\" }</code> </p>",
             "members": {
                 "MatchPattern": {
-                    "documentation": "<p>The filter to use to identify the subset of headers to inspect in a web request. </p> <p>You must specify exactly one setting: either <code>All</code>, <code>IncludedHeaders</code>, or <code>ExcludedHeaders</code>.</p> <p>Example JSON: <code>\"MatchPattern\": { \"ExcludedHeaders\": {\"KeyToExclude1\", \"KeyToExclude2\"} }</code> </p>",
+                    "documentation": "<p>The filter to use to identify the subset of headers to inspect in a web request. </p> <p>You must specify exactly one setting: either <code>All</code>, <code>IncludedHeaders</code>, or <code>ExcludedHeaders</code>.</p> <p>Example JSON: <code>\"MatchPattern\": { \"ExcludedHeaders\": [ \"KeyToExclude1\", \"KeyToExclude2\" ] }</code> </p>",
                     "shape": "HeaderMatchPattern"
                 },
                 "MatchScope": {
                     "documentation": "<p>The parts of the headers to match with the rule inspection criteria. If you specify <code>All</code>, WAF inspects both keys and values. </p>",
                     "shape": "MapMatchScope"
                 },
                 "OversizeHandling": {
@@ -5472,14 +5472,18 @@
                 "QueryArgument": {
                     "documentation": "<p>Use the specified query argument as an aggregate key. Each distinct value for the named query argument contributes to the aggregation instance. If you use a single query argument as your custom key, then each value fully defines an aggregation instance. </p>",
                     "shape": "RateLimitQueryArgument"
                 },
                 "QueryString": {
                     "documentation": "<p>Use the request's query string as an aggregate key. Each distinct string contributes to the aggregation instance. If you use just the query string as your custom key, then each string fully defines an aggregation instance. </p>",
                     "shape": "RateLimitQueryString"
+                },
+                "UriPath": {
+                    "documentation": "<p>Use the request's URI path as an aggregate key. Each distinct URI path contributes to the aggregation instance. If you use just the URI path as your custom key, then each URI path fully defines an aggregation instance. </p>",
+                    "shape": "RateLimitUriPath"
                 }
             },
             "type": "structure"
         },
         "RateBasedStatementCustomKeys": {
             "max": 5,
             "member": {
@@ -5594,14 +5598,27 @@
             "members": {
                 "TextTransformations": {
                     "documentation": "<p>Text transformations eliminate some of the unusual formatting that attackers use in web requests in an effort to bypass detection. Text transformations are used in rule match statements, to transform the <code>FieldToMatch</code> request component before inspecting it, and they're used in rate-based rule statements, to transform request components before using them as custom aggregation keys. If you specify one or more transformations to apply, WAF performs all transformations on the specified content, starting from the lowest priority setting, and then uses the component contents. </p>",
                     "shape": "TextTransformations"
                 }
             },
             "required": [
+                "TextTransformations"
+            ],
+            "type": "structure"
+        },
+        "RateLimitUriPath": {
+            "documentation": "<p>Specifies the request's URI path as an aggregate key for a rate-based rule. Each distinct URI path contributes to the aggregation instance. If you use just the URI path as your custom key, then each URI path fully defines an aggregation instance. </p>",
+            "members": {
+                "TextTransformations": {
+                    "documentation": "<p>Text transformations eliminate some of the unusual formatting that attackers use in web requests in an effort to bypass detection. Text transformations are used in rule match statements, to transform the <code>FieldToMatch</code> request component before inspecting it, and they're used in rate-based rule statements, to transform request components before using them as custom aggregation keys. If you specify one or more transformations to apply, WAF performs all transformations on the specified content, starting from the lowest priority setting, and then uses the component contents. </p>",
+                    "shape": "TextTransformations"
+                }
+            },
+            "required": [
                 "TextTransformations"
             ],
             "type": "structure"
         },
         "RedactedFields": {
             "max": 100,
             "member": {
```

### Comparing `botocore-a-la-carte-wafv2-1.31.5/botocore_a_la_carte_wafv2.egg-info/PKG-INFO` & `botocore-a-la-carte-wafv2-1.31.6/botocore_a_la_carte_wafv2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-wafv2
-Version: 1.31.5
+Version: 1.31.6
 Summary: wafv2 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-wafv2-1.31.5/setup.py` & `botocore-a-la-carte-wafv2-1.31.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-wafv2',
-    version="1.31.5",
+    version="1.31.6",
     description='wafv2 data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/wafv2/*/*.json'],
```

