# Comparing `tmp/nomenklatura-3.3.3.tar.gz` & `tmp/nomenklatura-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenklatura-3.3.3.tar", last modified: Wed Jul 19 14:12:12 2023, max compression
+gzip compressed data, was "nomenklatura-3.3.4.tar", last modified: Fri Jul 21 07:12:29 2023, max compression
```

## Comparing `nomenklatura-3.3.3.tar` & `nomenklatura-3.3.4.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:12:12.102342 nomenklatura-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-19 14:12:12.102342 nomenklatura-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:12:12.094342 nomenklatura-3.3.3/nomenklatura/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:12:12.094342 nomenklatura-3.3.3/nomenklatura/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/data/regression-v1.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/data/regression-v2.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:12:12.094342 nomenklatura-3.3.3/nomenklatura/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/dataset/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/dataset/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/dataset/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/dataset/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/dataset/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:12:12.094342 nomenklatura-3.3.3/nomenklatura/enrich/
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/enrich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/enrich/aleph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/enrich/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/enrich/nominatim.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/enrich/opencorporates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:12:12.098342 nomenklatura-3.3.3/nomenklatura/enrich/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/enrich/wikidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/enrich/wikidata/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/enrich/wikidata/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/enrich/wikidata/props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/enrich/wikidata/qualified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/enrich/wikidata/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/enrich/yente.py
--rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:12:12.098342 nomenklatura-3.3.3/nomenklatura/index/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/index/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/index/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/judgement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:12:12.098342 nomenklatura-3.3.3/nomenklatura/matching/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:12:12.098342 nomenklatura-3.3.3/nomenklatura/matching/heuristic/
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/heuristic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/heuristic/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:12:12.098342 nomenklatura-3.3.3/nomenklatura/matching/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/v1/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/v1/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/v1/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/v1/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/v1/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/v1/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:12:12.098342 nomenklatura-3.3.3/nomenklatura/matching/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/v2/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/v2/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/v2/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/v2/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/v2/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/matching/v2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:12:12.098342 nomenklatura-3.3.3/nomenklatura/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/publish/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/publish/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/publish/names.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:12:12.098342 nomenklatura-3.3.3/nomenklatura/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/resolver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/resolver/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/resolver/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/senzing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:12:12.098342 nomenklatura-3.3.3/nomenklatura/statement/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/statement/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/statement/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:12:12.098342 nomenklatura-3.3.3/nomenklatura/store/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/store/level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/store/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/store/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:12:12.102342 nomenklatura-3.3.3/nomenklatura/tui/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/tui/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/nomenklatura/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:12:12.094342 nomenklatura-3.3.3/nomenklatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-19 14:12:12.000000 nomenklatura-3.3.3/nomenklatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-19 14:12:12.000000 nomenklatura-3.3.3/nomenklatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 14:12:12.000000 nomenklatura-3.3.3/nomenklatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-19 14:12:12.000000 nomenklatura-3.3.3/nomenklatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 14:12:12.000000 nomenklatura-3.3.3/nomenklatura.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 14:11:13.000000 nomenklatura-3.3.3/nomenklatura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-19 14:12:12.000000 nomenklatura-3.3.3/nomenklatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-19 14:12:12.000000 nomenklatura-3.3.3/nomenklatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 14:12:12.102342 nomenklatura-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-19 14:09:37.000000 nomenklatura-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.874382 nomenklatura-3.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-21 07:12:29.874382 nomenklatura-3.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.866381 nomenklatura-3.3.4/nomenklatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.870382 nomenklatura-3.3.4/nomenklatura/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/data/regression-v1.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/data/regression-v2.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.870382 nomenklatura-3.3.4/nomenklatura/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/dataset/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/dataset/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/dataset/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/dataset/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/dataset/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.870382 nomenklatura-3.3.4/nomenklatura/enrich/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/nominatim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/opencorporates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.870382 nomenklatura-3.3.4/nomenklatura/enrich/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/wikidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/wikidata/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/wikidata/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/wikidata/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/wikidata/qualified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/wikidata/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/enrich/yente.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.870382 nomenklatura-3.3.4/nomenklatura/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/index/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/index/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/judgement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.870382 nomenklatura-3.3.4/nomenklatura/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.870382 nomenklatura-3.3.4/nomenklatura/matching/heuristic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/heuristic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/heuristic/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.870382 nomenklatura-3.3.4/nomenklatura/matching/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v1/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v1/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v1/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v1/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v1/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v1/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.874382 nomenklatura-3.3.4/nomenklatura/matching/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v2/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v2/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v2/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v2/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/matching/v2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.874382 nomenklatura-3.3.4/nomenklatura/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/publish/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/publish/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/publish/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.874382 nomenklatura-3.3.4/nomenklatura/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/resolver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/resolver/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/resolver/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/senzing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.874382 nomenklatura-3.3.4/nomenklatura/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/statement/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/statement/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/statement/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.874382 nomenklatura-3.3.4/nomenklatura/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/store/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/store/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/store/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.874382 nomenklatura-3.3.4/nomenklatura/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/tui/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/nomenklatura/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:12:29.866381 nomenklatura-3.3.4/nomenklatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-21 07:12:29.000000 nomenklatura-3.3.4/nomenklatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-21 07:12:29.000000 nomenklatura-3.3.4/nomenklatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:12:29.000000 nomenklatura-3.3.4/nomenklatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-21 07:12:29.000000 nomenklatura-3.3.4/nomenklatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:12:29.000000 nomenklatura-3.3.4/nomenklatura.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:11:32.000000 nomenklatura-3.3.4/nomenklatura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-21 07:12:29.000000 nomenklatura-3.3.4/nomenklatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 07:12:29.000000 nomenklatura-3.3.4/nomenklatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 07:12:29.874382 nomenklatura-3.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-21 07:09:55.000000 nomenklatura-3.3.4/setup.py
```

### Comparing `nomenklatura-3.3.3/LICENSE` & `nomenklatura-3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/PKG-INFO` & `nomenklatura-3.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.3.3
+Version: 3.3.4
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: leveldb
 License-File: LICENSE
 
 # nomenklatura
 
@@ -91,7 +92,9 @@
 ## Contact, contributions etc.
 
 This codebase is licensed under the terms of an MIT license (see LICENSE).
 
 We're keen for any contributions, bug fixes and feature suggestions, please use the GitHub issue tracker for this repository. 
 
 Nomenklatura is currently developed thanks to a Prototypefund grant for [OpenSanctions](https://opensanctions.org). Previous iterations of the package were developed with support from [Knight-Mozilla OpenNews](http://opennews.org) and the [Open Knowledge Foundation Labs](http://okfnlabs.org).
+
+
```

### Comparing `nomenklatura-3.3.3/README.md` & `nomenklatura-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/cache.py` & `nomenklatura-3.3.4/nomenklatura/cache.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/cli.py` & `nomenklatura-3.3.4/nomenklatura/cli.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/data/regression-v1.pkl` & `nomenklatura-3.3.4/nomenklatura/data/regression-v1.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/data/regression-v2.pkl` & `nomenklatura-3.3.4/nomenklatura/data/regression-v2.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/dataset/catalog.py` & `nomenklatura-3.3.4/nomenklatura/dataset/catalog.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/dataset/coverage.py` & `nomenklatura-3.3.4/nomenklatura/dataset/coverage.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/dataset/dataset.py` & `nomenklatura-3.3.4/nomenklatura/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/dataset/publisher.py` & `nomenklatura-3.3.4/nomenklatura/dataset/publisher.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/dataset/resource.py` & `nomenklatura-3.3.4/nomenklatura/dataset/resource.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/dataset/util.py` & `nomenklatura-3.3.4/nomenklatura/dataset/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/db.py` & `nomenklatura-3.3.4/nomenklatura/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/enrich/__init__.py` & `nomenklatura-3.3.4/nomenklatura/enrich/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/enrich/aleph.py` & `nomenklatura-3.3.4/nomenklatura/enrich/aleph.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/enrich/common.py` & `nomenklatura-3.3.4/nomenklatura/enrich/common.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/enrich/nominatim.py` & `nomenklatura-3.3.4/nomenklatura/enrich/nominatim.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/enrich/opencorporates.py` & `nomenklatura-3.3.4/nomenklatura/enrich/opencorporates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/enrich/wikidata/__init__.py` & `nomenklatura-3.3.4/nomenklatura/enrich/wikidata/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/enrich/wikidata/lang.py` & `nomenklatura-3.3.4/nomenklatura/enrich/wikidata/lang.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/enrich/wikidata/model.py` & `nomenklatura-3.3.4/nomenklatura/enrich/wikidata/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/enrich/wikidata/props.py` & `nomenklatura-3.3.4/nomenklatura/enrich/wikidata/props.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/enrich/wikidata/qualified.py` & `nomenklatura-3.3.4/nomenklatura/enrich/wikidata/qualified.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/enrich/wikidata/value.py` & `nomenklatura-3.3.4/nomenklatura/enrich/wikidata/value.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/enrich/yente.py` & `nomenklatura-3.3.4/nomenklatura/enrich/yente.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
         api_key: Optional[str] = os.path.expandvars(config.pop("api_key", "")).strip()
         if api_key is None or not len(api_key):
             api_key = os.environ.get("YENTE_API_KEY")
         self._api_key: Optional[str] = api_key
         if self._api_key is not None:
             self.session.headers["Authorization"] = f"ApiKey {self._api_key}"
 
-        match_url = urljoin(self._api, f"match/{self._dataset}")
-        self.cache.preload(f"{match_url}%")
+        # match_url = urljoin(self._api, f"match/{self._dataset}")
+        # self.cache.preload(f"{match_url}%")
 
     def make_url(self, entity: CE) -> str:
         return urljoin(self._api, f"entities/{entity.id}")
 
     def match(self, entity: CE) -> Generator[CE, None, None]:
         if not entity.schema.matchable:
             return
```

### Comparing `nomenklatura-3.3.3/nomenklatura/entity.py` & `nomenklatura-3.3.4/nomenklatura/entity.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/index/entry.py` & `nomenklatura-3.3.4/nomenklatura/index/entry.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/index/index.py` & `nomenklatura-3.3.4/nomenklatura/index/index.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/index/tokenizer.py` & `nomenklatura-3.3.4/nomenklatura/index/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/judgement.py` & `nomenklatura-3.3.4/nomenklatura/judgement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/matching/__init__.py` & `nomenklatura-3.3.4/nomenklatura/matching/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/matching/heuristic/__init__.py` & `nomenklatura-3.3.4/nomenklatura/matching/heuristic/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/matching/heuristic/logic.py` & `nomenklatura-3.3.4/nomenklatura/matching/heuristic/logic.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/matching/pairs.py` & `nomenklatura-3.3.4/nomenklatura/matching/pairs.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/matching/types.py` & `nomenklatura-3.3.4/nomenklatura/matching/types.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/matching/util.py` & `nomenklatura-3.3.4/nomenklatura/matching/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/matching/v1/dates.py` & `nomenklatura-3.3.4/nomenklatura/matching/v1/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/matching/v1/misc.py` & `nomenklatura-3.3.4/nomenklatura/matching/v1/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/matching/v1/model.py` & `nomenklatura-3.3.4/nomenklatura/matching/v1/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/matching/v1/names.py` & `nomenklatura-3.3.4/nomenklatura/matching/v1/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/matching/v1/train.py` & `nomenklatura-3.3.4/nomenklatura/matching/v1/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/matching/v1/util.py` & `nomenklatura-3.3.4/nomenklatura/matching/v1/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/matching/v2/dates.py` & `nomenklatura-3.3.4/nomenklatura/matching/v2/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/matching/v2/misc.py` & `nomenklatura-3.3.4/nomenklatura/matching/v2/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/matching/v2/model.py` & `nomenklatura-3.3.4/nomenklatura/matching/v2/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/matching/v2/names.py` & `nomenklatura-3.3.4/nomenklatura/matching/v2/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/matching/v2/train.py` & `nomenklatura-3.3.4/nomenklatura/matching/v2/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/matching/v2/util.py` & `nomenklatura-3.3.4/nomenklatura/matching/v2/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/publish/dates.py` & `nomenklatura-3.3.4/nomenklatura/publish/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/publish/edges.py` & `nomenklatura-3.3.4/nomenklatura/publish/edges.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/publish/names.py` & `nomenklatura-3.3.4/nomenklatura/publish/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/resolver/edge.py` & `nomenklatura-3.3.4/nomenklatura/resolver/edge.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/resolver/identifier.py` & `nomenklatura-3.3.4/nomenklatura/resolver/identifier.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/resolver/resolver.py` & `nomenklatura-3.3.4/nomenklatura/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/senzing.py` & `nomenklatura-3.3.4/nomenklatura/senzing.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/statement/serialize.py` & `nomenklatura-3.3.4/nomenklatura/statement/serialize.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/statement/statement.py` & `nomenklatura-3.3.4/nomenklatura/statement/statement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/store/__init__.py` & `nomenklatura-3.3.4/nomenklatura/store/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/store/base.py` & `nomenklatura-3.3.4/nomenklatura/store/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,17 @@
         canonical_id = self.resolver.get_canonical(id)
         with self.writer() as writer:
             for referent in self.resolver.get_referents(canonical_id):
                 for stmt in writer.pop(referent):
                     stmt.canonical_id = canonical_id
                     writer.add_statement(stmt)
 
+    def close(self) -> None:
+        pass
+
     def __repr__(self) -> str:
         return f"<{type(self).__name__}({self.dataset.name!r})>"
 
 
 class Writer(Generic[DS, CE]):
     """Bulk writing operations."""
```

### Comparing `nomenklatura-3.3.3/nomenklatura/store/level.py` & `nomenklatura-3.3.4/nomenklatura/store/level.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 
     def writer(self) -> Writer[DS, CE]:
         return LevelDBWriter(self)
 
     def view(self, scope: DS, external: bool = False) -> View[DS, CE]:
         return LevelDBView(self, scope, external=external)
 
+    def close(self) -> None:
+        self.db.close()
+
 
 class LevelDBWriter(Writer[DS, CE]):
     BATCH_STATEMENTS = 50000
 
     def __init__(self, store: LevelDBStore[DS, CE]):
         self.store: LevelDBStore[DS, CE] = store
         self.batch: Optional[Any] = None
```

### Comparing `nomenklatura-3.3.3/nomenklatura/store/memory.py` & `nomenklatura-3.3.4/nomenklatura/store/memory.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/store/util.py` & `nomenklatura-3.3.4/nomenklatura/store/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/tui/app.py` & `nomenklatura-3.3.4/nomenklatura/tui/app.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/tui/comparison.py` & `nomenklatura-3.3.4/nomenklatura/tui/comparison.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/tui/util.py` & `nomenklatura-3.3.4/nomenklatura/tui/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura/util.py` & `nomenklatura-3.3.4/nomenklatura/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from functools import lru_cache, cache
 from normality.constants import WS
 from followthemoney import model
 from collections.abc import Mapping, Sequence
 from fingerprints.fingerprint import fingerprint
 from fingerprints.cleanup import clean_strict
 from followthemoney.util import sanitize_text
-from typing import cast, Any, Mapping, Union, Iterable, Tuple, Optional, List, Set
+from typing import cast, Any, Union, Iterable, Tuple, Optional, List, Set
 from urllib.parse import urlparse, urlunparse, parse_qsl, urlencode
 
 DATA_PATH = Path(os.path.join(os.path.dirname(__file__), "data")).resolve()
 QID = re.compile(r"^Q(\d+)$")
 BASE_ID = "id"
 PathLike = Union[str, os.PathLike[str]]
 ParamsType = Union[None, Iterable[Tuple[str, Any]], Mapping[str, Any]]
```

### Comparing `nomenklatura-3.3.3/nomenklatura/xref.py` & `nomenklatura-3.3.4/nomenklatura/xref.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.3/nomenklatura.egg-info/PKG-INFO` & `nomenklatura-3.3.4/nomenklatura.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.3.3
+Version: 3.3.4
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: leveldb
 License-File: LICENSE
 
 # nomenklatura
 
@@ -91,7 +92,9 @@
 ## Contact, contributions etc.
 
 This codebase is licensed under the terms of an MIT license (see LICENSE).
 
 We're keen for any contributions, bug fixes and feature suggestions, please use the GitHub issue tracker for this repository. 
 
 Nomenklatura is currently developed thanks to a Prototypefund grant for [OpenSanctions](https://opensanctions.org). Previous iterations of the package were developed with support from [Knight-Mozilla OpenNews](http://opennews.org) and the [Open Knowledge Foundation Labs](http://okfnlabs.org).
+
+
```

### Comparing `nomenklatura-3.3.3/nomenklatura.egg-info/SOURCES.txt` & `nomenklatura-3.3.4/nomenklatura.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 nomenklatura/publish/names.py
 nomenklatura/resolver/__init__.py
 nomenklatura/resolver/common.py
 nomenklatura/resolver/edge.py
 nomenklatura/resolver/identifier.py
 nomenklatura/resolver/resolver.py
 nomenklatura/statement/__init__.py
+nomenklatura/statement/db.py
 nomenklatura/statement/serialize.py
 nomenklatura/statement/statement.py
 nomenklatura/store/__init__.py
 nomenklatura/store/base.py
 nomenklatura/store/level.py
 nomenklatura/store/memory.py
 nomenklatura/store/util.py
```

### Comparing `nomenklatura-3.3.3/setup.py` & `nomenklatura-3.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="nomenklatura",
-    version="3.3.3",
+    version="3.3.4",
     description="Make record linkages in followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney linkage record",
     author="Friedrich Lindenberg",
     author_email="friedrich@pudo.org",
     url="https://github.com/opensanctions/nomenklatura",
```

