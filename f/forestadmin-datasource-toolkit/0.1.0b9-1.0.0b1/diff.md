# Comparing `tmp/forestadmin_datasource_toolkit-0.1.0b9.tar.gz` & `tmp/forestadmin_datasource_toolkit-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_datasource_toolkit-0.1.0b9.tar", max compression
+gzip compressed data, was "forestadmin_datasource_toolkit-1.0.0b1.tar", max compression
```

## Comparing `forestadmin_datasource_toolkit-0.1.0b9.tar` & `forestadmin_datasource_toolkit-1.0.0b1.tar`

### file list

```diff
@@ -1,90 +1,113 @@
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/README.md
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/__init__.py
--rw-r--r--   0        0        0     2219 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/collections.py
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/context/__init__.py
--rw-r--r--   0        0        0      716 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/context/agent_context.py
--rw-r--r--   0        0        0      768 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/context/collection_context.py
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/context/relaxed_wrappers/__init__.py
--rw-r--r--   0        0        0     6533 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py
--rw-r--r--   0        0        0     1195 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/datasources.py
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/__init__.py
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/__init__.py
--rw-r--r--   0        0        0     4910 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/collections.py
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/context/__init__.py
--rw-r--r--   0        0        0     1944 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/context/base.py
--rw-r--r--   0        0        0      799 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/context/bulk.py
--rw-r--r--   0        0        0      776 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/context/single.py
--rw-r--r--   0        0        0     1984 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/result_builder.py
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/types/__init__.py
--rw-r--r--   0        0        0     1656 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/types/actions.py
--rw-r--r--   0        0        0    12320 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/types/fields.py
--rw-r--r--   0        0        0     1530 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/collections.py
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/computed/__init__.py
--rw-r--r--   0        0        0     4537 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/computed/collections.py
--rw-r--r--   0        0        0      150 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/computed/exceptions.py
--rw-r--r--   0        0        0     5113 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/computed/helpers.py
--rw-r--r--   0        0        0      535 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/computed/types.py
--rw-r--r--   0        0        0     2814 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/computed/utils.py
--rw-r--r--   0        0        0      595 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/datasource.py
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/operators_replace/__init__.py
--rw-r--r--   0        0        0     3279 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/operators_replace/collections.py
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/proxy/__init__.py
--rw-r--r--   0        0        0     3362 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/proxy/collection.py
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/publication/__init__.py
--rw-r--r--   0        0        0     2689 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/publication/collections.py
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/rename/__init__.py
--rw-r--r--   0        0        0     9765 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/rename/collections.py
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/search/__init__.py
--rw-r--r--   0        0        0     5247 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/search/collections.py
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/segments/__init__.py
--rw-r--r--   0        0        0     2432 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/segments/collections.py
--rw-r--r--   0        0        0       54 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/exceptions.py
--rw-r--r--   0        0        0     6148 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/.DS_Store
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/__init__.py
--rw-r--r--   0        0        0     1881 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/actions.py
--rw-r--r--   0        0        0     1781 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/collections.py
--rw-r--r--   0        0        0     5139 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/fields.py
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/models/__init__.py
--rw-r--r--   0        0        0     1400 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/models/collections.py
--rw-r--r--   0        0        0     6148 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/.DS_Store
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/__init__.py
--rw-r--r--   0        0        0     7811 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/aggregation.py
--rw-r--r--   0        0        0     6148 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/__init__.py
--rw-r--r--   0        0        0     4663 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py
--rw-r--r--   0        0        0     5323 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/__init__.py
--rw-r--r--   0        0        0     2124 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py
--rw-r--r--   0        0        0     4370 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py
--rw-r--r--   0        0        0     9674 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py
--rw-r--r--   0        0        0     1270 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/__init__.py
--rw-r--r--   0        0        0     3937 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py
--rw-r--r--   0        0        0     1579 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py
--rw-r--r--   0        0        0     7661 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/filter/__init__.py
--rw-r--r--   0        0        0     6662 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py
--rw-r--r--   0        0        0     2877 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py
--rw-r--r--   0        0        0     3213 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py
--rw-r--r--   0        0        0      875 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/page.py
--rw-r--r--   0        0        0     4482 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py
--rw-r--r--   0        0        0      901 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py
--rw-r--r--   0        0        0     2619 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py
--rw-r--r--   0        0        0      574 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py
--rw-r--r--   0        0        0      118 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/records.py
--rw-r--r--   0        0        0       73 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/utils/__init__.py
--rw-r--r--   0        0        0     7007 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/utils/collections.py
--rw-r--r--   0        0        0     1165 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/utils/records.py
--rw-r--r--   0        0        0     1658 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/utils/schema.py
--rw-r--r--   0        0        0        0 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/__init__.py
--rw-r--r--   0        0        0     4756 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/condition_tree.py
--rw-r--r--   0        0        0     3577 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/field.py
--rw-r--r--   0        0        0      393 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/projection.py
--rw-r--r--   0        0        0     1542 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/records.py
--rw-r--r--   0        0        0     4536 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/rules.py
--rw-r--r--   0        0        0      469 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/sort.py
--rw-r--r--   0        0        0     4348 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/type_getter.py
--rw-r--r--   0        0        0      372 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/types.py
--rw-r--r--   0        0        0     1622 2022-12-07 16:20:54.420138 forestadmin_datasource_toolkit-0.1.0b9/pyproject.toml
--rw-r--r--   0        0        0     2365 1970-01-01 00:00:00.000000 forestadmin_datasource_toolkit-0.1.0b9/setup.py
--rw-r--r--   0        0        0      908 1970-01-01 00:00:00.000000 forestadmin_datasource_toolkit-0.1.0b9/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/__init__.py
+-rw-r--r--   0        0        0     2276 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/collections.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/context/__init__.py
+-rw-r--r--   0        0        0      678 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/context/agent_context.py
+-rw-r--r--   0        0        0      658 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/context/collection_context.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/context/relaxed_wrappers/__init__.py
+-rw-r--r--   0        0        0     6971 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py
+-rw-r--r--   0        0        0     3350 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/datasource_customizer/collection_customizer.py
+-rw-r--r--   0        0        0     1608 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py
+-rw-r--r--   0        0        0     1536 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/datasources.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/__init__.py
+-rw-r--r--   0        0        0     5188 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/collections.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/context/__init__.py
+-rw-r--r--   0        0        0     2039 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/context/base.py
+-rw-r--r--   0        0        0      664 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/context/bulk.py
+-rw-r--r--   0        0        0      907 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/context/single.py
+-rw-r--r--   0        0        0     2167 2023-07-21 14:35:05.906294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/result_builder.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/types/__init__.py
+-rw-r--r--   0        0        0     1688 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/types/actions.py
+-rw-r--r--   0        0        0    14435 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/types/fields.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/chart/__init__.py
+-rw-r--r--   0        0        0     1941 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py
+-rw-r--r--   0        0        0     2133 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py
+-rw-r--r--   0        0        0     1549 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py
+-rw-r--r--   0        0        0     3484 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/chart/result_builder.py
+-rw-r--r--   0        0        0      557 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/chart/types.py
+-rw-r--r--   0        0        0     5005 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/collection_decorator.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/computed/__init__.py
+-rw-r--r--   0        0        0     4690 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/computed/collections.py
+-rw-r--r--   0        0        0      154 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/computed/exceptions.py
+-rw-r--r--   0        0        0     3886 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/computed/helpers.py
+-rw-r--r--   0        0        0      651 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/computed/types.py
+-rw-r--r--   0        0        0     2812 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/computed/utils.py
+-rw-r--r--   0        0        0      902 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/datasource_decorator.py
+-rw-r--r--   0        0        0     3943 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/decorator_stack.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/empty/__init__.py
+-rw-r--r--   0        0        0     4495 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/empty/collection.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/operators_equivalence/__init__.py
+-rw-r--r--   0        0        0     3855 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/publication_field/__init__.py
+-rw-r--r--   0        0        0     3015 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/publication_field/collections.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/rename_field/__init__.py
+-rw-r--r--   0        0        0     9761 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/rename_field/collections.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/schema/__init__.py
+-rw-r--r--   0        0        0      671 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/schema/collection.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/search/__init__.py
+-rw-r--r--   0        0        0     6200 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/search/collections.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/segments/__init__.py
+-rw-r--r--   0        0        0     2651 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/segments/collections.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/validation/__init__.py
+-rw-r--r--   0        0        0     4142 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/validation/collection.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/create_relations/__init__.py
+-rw-r--r--   0        0        0     5102 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/update_relations/__init__.py
+-rw-r--r--   0        0        0     4845 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py
+-rw-r--r--   0        0        0     1020 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/write_replace/__init__.py
+-rw-r--r--   0        0        0      258 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/write_replace/types.py
+-rw-r--r--   0        0        0     1045 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py
+-rw-r--r--   0        0        0     6327 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py
+-rw-r--r--   0        0        0      281 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/exceptions.py
+-rw-r--r--   0        0        0     6148 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/.DS_Store
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/__init__.py
+-rw-r--r--   0        0        0     1933 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/actions.py
+-rw-r--r--   0        0        0      954 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/chart.py
+-rw-r--r--   0        0        0     2534 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/collections.py
+-rw-r--r--   0        0        0     5323 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/fields.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/models/__init__.py
+-rw-r--r--   0        0        0     1420 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/models/collections.py
+-rw-r--r--   0        0        0     6148 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/.DS_Store
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/__init__.py
+-rw-r--r--   0        0        0     7775 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/aggregation.py
+-rw-r--r--   0        0        0     6148 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/__init__.py
+-rw-r--r--   0        0        0     4665 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py
+-rw-r--r--   0        0        0     5377 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/__init__.py
+-rw-r--r--   0        0        0     2124 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py
+-rw-r--r--   0        0        0     4370 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py
+-rw-r--r--   0        0        0     9674 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py
+-rw-r--r--   0        0        0     1270 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/__init__.py
+-rw-r--r--   0        0        0     3941 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py
+-rw-r--r--   0        0        0     1579 2023-07-21 14:35:05.910294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py
+-rw-r--r--   0        0        0     7660 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/filter/__init__.py
+-rw-r--r--   0        0        0     6832 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py
+-rw-r--r--   0        0        0     2877 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py
+-rw-r--r--   0        0        0     3213 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py
+-rw-r--r--   0        0        0      875 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/page.py
+-rw-r--r--   0        0        0     4511 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py
+-rw-r--r--   0        0        0      902 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py
+-rw-r--r--   0        0        0     2619 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py
+-rw-r--r--   0        0        0      595 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py
+-rw-r--r--   0        0        0      118 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/records.py
+-rw-r--r--   0        0        0       73 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0     7235 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/utils/collections.py
+-rw-r--r--   0        0        0     1169 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/utils/records.py
+-rw-r--r--   0        0        0     1658 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/utils/schema.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/__init__.py
+-rw-r--r--   0        0        0     4777 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/condition_tree.py
+-rw-r--r--   0        0        0     3577 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/field.py
+-rw-r--r--   0        0        0      393 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/projection.py
+-rw-r--r--   0        0        0     1542 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/records.py
+-rw-r--r--   0        0        0     4536 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/rules.py
+-rw-r--r--   0        0        0      469 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/sort.py
+-rw-r--r--   0        0        0     4347 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/type_getter.py
+-rw-r--r--   0        0        0      372 2023-07-21 14:35:05.914294 forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/types.py
+-rw-r--r--   0        0        0     1758 2023-07-21 14:35:33.078530 forestadmin_datasource_toolkit-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 forestadmin_datasource_toolkit-1.0.0b1/PKG-INFO
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/collections.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/collections.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,16 @@
         self._datasource = datasource
         self._name = name
         self._schema: CollectionSchema = {
             "actions": {},
             "fields": {},
             "searchable": False,
             "segments": [],
+            "countable": True,
+            "charts": {},
         }
 
     def __repr__(self) -> str:
         return f"{self.name}: {self.schema}"
 
     @property
     def datasource(self) -> "Datasource[Self]":
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import List, Optional, Union, cast
 
+from forestadmin.agent_toolkit.utils.context import User
 from forestadmin.datasource_toolkit.datasources import DatasourceException
 from forestadmin.datasource_toolkit.interfaces.actions import ActionField, ActionResult
+from forestadmin.datasource_toolkit.interfaces.chart import Chart
 from forestadmin.datasource_toolkit.interfaces.collections import Collection
 from forestadmin.datasource_toolkit.interfaces.models.collections import Datasource
 from forestadmin.datasource_toolkit.interfaces.query.aggregation import (
     AggregateResult,
     Aggregation,
     PlainAggregation,
     is_aggregation,
@@ -39,15 +41,15 @@
         self.datasource = datasource
 
     @property
     def collections(self) -> List["RelaxedCollection"]:
         return [RelaxedCollection(collection) for collection in self.datasource.collections]
 
     def get_collection(self, name: str) -> "RelaxedCollection":
-        collection = super().get_collection(name)
+        collection = self.datasource.get_collection(name)
         return RelaxedCollection(collection)
 
     def add_collection(self, collection: "RelaxedCollection") -> None:
         raise RelaxedDatasourceException("Cannot modify existing datasources")
 
 
 class RelaxedCollection(Collection):
@@ -63,28 +65,16 @@
     def name(self) -> str:
         return self.collection.name
 
     @property
     def schema(self):
         return self.collection.schema
 
-    async def execute(
-        self, name: str, data: RecordsDataAlias, filter: Optional[Union[Filter, PlainFilter]]
-    ) -> ActionResult:
-        filter_instance = self._build_filter(filter)
-        return await self.collection.execute(name, data, filter_instance)
-
-    async def get_form(
-        self, name: str, data: Optional[RecordsDataAlias], filter: Optional[Filter]
-    ) -> List[ActionField]:
-        filter_instance = self._build_filter(filter)
-        return await super().get_form(name, data, filter_instance)
-
-    async def create(self, data: List[RecordsDataAlias]) -> List[RecordsDataAlias]:
-        return await self.collection.create(data)
+    async def create(self, caller: User, data: List[RecordsDataAlias]) -> List[RecordsDataAlias]:
+        return await self.collection.create(caller, data)
 
     def _build_filter(self, filter: Optional[Union[Filter, PlainFilter]]) -> Optional[Filter]:
         if not filter:
             return None
         elif is_filter(filter):
             return filter
         else:
@@ -134,29 +124,44 @@
     def _build_aggregation(self, aggregation: Union[Aggregation, PlainAggregation]) -> Aggregation:
         if is_aggregation(aggregation):
             return aggregation
         aggregation = cast(PlainAggregation, aggregation)
         return Aggregation(aggregation)
 
     async def list(
-        self, filter: Union[PaginatedFilter, PlainPaginatedFilter], projection: Projection
+        self, caller: User, filter: Union[PaginatedFilter, PlainPaginatedFilter], projection: Projection
     ) -> List[RecordsDataAlias]:
         filter_instance = self._build_paginated_filter(filter)
         projection_instance = self._build_projection(projection)
 
-        return await self.collection.list(filter_instance, projection_instance)
+        return await self.collection.list(caller, filter_instance, projection_instance)
 
-    async def update(self, filter: Optional[Union[Filter, PlainFilter]], patch: RecordsDataAlias) -> None:
+    async def update(self, caller: User, filter: Optional[Union[Filter, PlainFilter]], patch: RecordsDataAlias) -> None:
         filter_instance = self._build_filter(filter)
-        return await self.collection.update(filter_instance, patch)
+        return await self.collection.update(caller, filter_instance, patch)
 
-    async def delete(self, filter: Optional[Union[Filter, PlainFilter]]) -> None:
+    async def delete(self, caller: User, filter: Optional[Union[Filter, PlainFilter]]) -> None:
         filter_instance = self._build_filter(filter)
-        return await self.collection.delete(filter_instance)
+        return await self.collection.delete(caller, filter_instance)
 
     async def aggregate(
-        self, filter: Optional[Filter], aggregation: Aggregation, limit: Optional[int] = None
+        self, caller: User, filter: Optional[Filter], aggregation: Aggregation, limit: Optional[int] = None
     ) -> List[AggregateResult]:
         filter_instance = self._build_filter(filter)
         aggregation_instance = self._build_aggregation(aggregation)
 
-        return await self.collection.aggregate(filter_instance, aggregation_instance, limit)
+        return await self.collection.aggregate(caller, filter_instance, aggregation_instance, limit)
+
+    async def execute(
+        self, caller: User, name: str, data: RecordsDataAlias, filter: Optional[Union[Filter, PlainFilter]]
+    ) -> ActionResult:
+        filter_instance = self._build_filter(filter)
+        return await self.collection.execute(caller, name, data, filter_instance)
+
+    async def get_form(
+        self, caller: User, name: str, data: Optional[RecordsDataAlias], filter: Optional[Filter]
+    ) -> List[ActionField]:
+        filter_instance = self._build_filter(filter)
+        return await super().get_form(caller, name, data, filter_instance)
+
+    async def render_chart(self, caller: User, name: str, record_id: List) -> Chart:
+        return await super().render_chart(caller, name, record_id)
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/datasources.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/datasources.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from typing import Dict, List
 
+from forestadmin.agent_toolkit.utils.context import User
 from forestadmin.datasource_toolkit.exceptions import DatasourceToolkitException
+from forestadmin.datasource_toolkit.interfaces.chart import Chart
 from forestadmin.datasource_toolkit.interfaces.models.collections import BoundCollection
 from forestadmin.datasource_toolkit.interfaces.models.collections import Datasource as DatasourceInterface
 
 
 class DatasourceException(DatasourceToolkitException):
     pass
 
 
 class Datasource(DatasourceInterface[BoundCollection]):
     def __init__(self) -> None:
         self._collections: Dict[str, BoundCollection] = {}
 
     @property
+    def schema(self):
+        return {"charts": {}}
+
+    @property
     def collections(self) -> List[BoundCollection]:
         return list(self._collections.values())
 
     def get_collection(self, name: str) -> BoundCollection:
         try:
             collection: BoundCollection = self._collections[name]
         except KeyError:
@@ -25,7 +31,10 @@
         else:
             return collection
 
     def add_collection(self, collection: BoundCollection) -> None:
         if collection.name in self._collections:
             raise DatasourceException(f"Collection '{collection.name}' already defined in datasource")
         self._collections[collection.name] = collection
+
+    async def render_chart(self, caller: User, name: str) -> Chart:
+        raise DatasourceException(f"Chart {name} not exists on this datasource.")
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/collections.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/collections.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,102 +1,103 @@
-from typing import Any, Callable, Dict, List, Optional, Set, Union, cast
+from typing import Any, Awaitable, Dict, List, Optional, Set, Union, cast
 
+from forestadmin.agent_toolkit.utils.context import User
 from forestadmin.datasource_toolkit.collections import Collection
 from forestadmin.datasource_toolkit.decorators.action.context.base import ActionContext
 from forestadmin.datasource_toolkit.decorators.action.context.bulk import ActionContextBulk
 from forestadmin.datasource_toolkit.decorators.action.context.single import ActionContextSingle
 from forestadmin.datasource_toolkit.decorators.action.result_builder import ResultBuilder
 from forestadmin.datasource_toolkit.decorators.action.types.actions import (
     ActionAlias,
     ActionBulk,
     ActionGlobal,
     ActionSingle,
 )
 from forestadmin.datasource_toolkit.decorators.action.types.fields import DynamicField
+from forestadmin.datasource_toolkit.decorators.collection_decorator import CollectionDecorator
 from forestadmin.datasource_toolkit.interfaces.actions import Action, ActionField, ActionResult
 from forestadmin.datasource_toolkit.interfaces.models.collections import CollectionSchema
 from forestadmin.datasource_toolkit.interfaces.query.filter.unpaginated import Filter
 from forestadmin.datasource_toolkit.interfaces.records import RecordsDataAlias
 
 
-class ActionMixin:
-    datasource: property
-    mark_schema_as_dirty: Callable[..., None]
-
+class ActionCollectionDecorator(CollectionDecorator):
     def __init__(self, *args: Any, **kwargs: Any):
-        super(ActionMixin, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self._actions: Dict[str, ActionAlias] = {}
 
     def add_action(self, name: str, action: ActionAlias):
         self._actions[name] = action
         self.mark_schema_as_dirty()
 
     async def execute(
         self,
+        caller: User,
         name: str,
         data: RecordsDataAlias,
-        filter: Optional[Filter],
+        filter_: Optional[Filter] = None,
     ) -> ActionResult:
-        action = self._actions[name]
+        action = self._actions.get(name)
         if not action:
-            return super(ActionMixin, self).execute(name, data, filter)  # type: ignore
+            return await super().execute(caller, name, data, filter_)  # type: ignore
 
-        context = self._get_context(action, data, filter)
+        context = self._get_context(caller, action, data, filter_)
         response_builder = ResultBuilder()
-        result = await action.execute(context, response_builder)  # type: ignore
+        result = action.execute(context, response_builder)  # type: ignore
+        if isinstance(result, Awaitable):
+            result = await result
         return result or {"type": "Success", "invalidated": set(), "format": "text", "message": "Success"}
 
     async def get_form(
-        self, name: str, data: Optional[RecordsDataAlias], filter: Optional[Filter]
+        self, caller: User, name: str, data: Optional[RecordsDataAlias], filter_: Optional[Filter] = None
     ) -> List[ActionField]:
         action = self._actions.get(name)
         if not action:
-            return super(ActionMixin, self).get_form(name, data, filter)  # type: ignore
+            return await super().get_form(caller, name, data, filter_)  # type: ignore
         elif not action.form:
             return []
 
         form_values = data or {}
         used: Set[str] = set()
-        context = self._get_context(action, form_values, filter, used)
+        context = self._get_context(caller, action, form_values, filter_, used)
         form_fields: List[DynamicField[ActionContext]] = cast(
             List[DynamicField[ActionContext]], [field for field in action.form]
         )
 
         form_values = await self._build_form_values(context, form_fields, form_values)
         action_fields = await self._build_fields(context, form_fields, form_values)
         for field in action_fields:
             field["watch_changes"] = field["label"] in context.form_values.used_keys
         return action_fields
 
-    @property
-    def schema(self) -> CollectionSchema:
-        schema: CollectionSchema = super(ActionMixin, self).schema  # type: ignore
+    def _refine_schema(self, sub_schema: CollectionSchema) -> CollectionSchema:
+        actions_schema = {}
         for name, action in self._actions.items():
             dynamics: List[bool] = []
             for field in action.form or []:
                 dynamics.append(field.is_dynamic)
-            schema["actions"][name] = Action(
+            actions_schema[name] = Action(
                 scope=action.SCOPE, generate_file=action.GENERATE_FILE, static_form=not any(dynamics)
             )
-
-        return schema
+        return {**sub_schema, "actions": actions_schema}
 
     def _get_context(
         self,
+        caller: User,
         action: Union[ActionSingle, ActionBulk, ActionGlobal],
         form_values: RecordsDataAlias,
-        filter: Optional[Filter],
+        filter_: Optional[Filter] = None,
         used: Optional[Set[str]] = None,
     ) -> ActionContext:
         return {
             ActionSingle.SCOPE: ActionContextSingle,
             ActionBulk.SCOPE: ActionContextBulk,
             ActionGlobal.SCOPE: ActionContext,
         }[action.SCOPE](
-            cast(Collection, self), form_values, filter, used  # type: ignore
+            cast(Collection, self), caller, form_values, filter_, used  # type: ignore
         )
 
     async def _build_form_values(
         self, context: ActionContext, fields: List[DynamicField[ActionContext]], data: Optional[Dict[str, Any]]
     ):
         if data is None:
             form_values: Dict[str, Any] = {}
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/context/base.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/context/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,50 @@
-from typing import Any, List, Optional, Set
+from typing import Any, Dict, List, Optional, Set
 
+from forestadmin.agent_toolkit.utils.context import User
 from forestadmin.datasource_toolkit.collections import Collection
 from forestadmin.datasource_toolkit.context.collection_context import CollectionCustomizationContext
 from forestadmin.datasource_toolkit.interfaces.query.filter.paginated import PaginatedFilter
 from forestadmin.datasource_toolkit.interfaces.query.filter.unpaginated import Filter
 from forestadmin.datasource_toolkit.interfaces.query.projections import Projection
 from forestadmin.datasource_toolkit.interfaces.records import RecordsDataAlias
 from forestadmin.datasource_toolkit.validations.projection import ProjectionValidator
 
 
-class FormValueObserver(dict[str, Any]):
+class FormValueObserver(Dict[str, Any]):
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self._used: Set[str] = set()
 
-    def get(self, __key: str, default: Any) -> Any:
+    def get(self, __key: str, default: Any = None) -> Any:
         self._used.add(__key)
         return super().get(__key, default)
 
     def __getitem__(self, __key: str) -> Any:
         self._used.add(__key)
         return super().__getitem__(__key)
 
     @property
     def used_keys(self) -> Set[str]:
         return self._used
 
 
 class ActionContext(CollectionCustomizationContext):
-    def __init__(self, collection: Collection, form_value: RecordsDataAlias, filter: Filter, used: Optional[Set[str]]):
-        tz = None
-        if filter:
-            tz = filter.timezone
-        super(ActionContext, self).__init__(collection, tz)
+    def __init__(
+        self,
+        collection: Collection,
+        caller: User,
+        form_value: RecordsDataAlias,
+        filter: Filter,
+        used: Optional[Set[str]] = set(),
+    ):
+        super(ActionContext, self).__init__(collection, caller)
         self.form_values = FormValueObserver(**form_value)
         self.filter = filter
 
     async def get_records(self, fields: Projection) -> List[RecordsDataAlias]:
         ProjectionValidator.validate(self.collection, fields)
         projection = Projection(*fields)
         return await self._run_query(projection)
 
     async def _run_query(self, projection: Projection) -> List[RecordsDataAlias]:
-        return await self.collection.list(PaginatedFilter.from_base_filter(self.filter), projection)
+        return await self.collection.list(self._caller, PaginatedFilter.from_base_filter(self.filter), projection)
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/context/bulk.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/context/bulk.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-from typing import Any, List
+from typing import List
 
 from forestadmin.datasource_toolkit.decorators.action.context.base import ActionContext
 from forestadmin.datasource_toolkit.interfaces.query.projections import Projection
 from forestadmin.datasource_toolkit.interfaces.records import CompositeIdAlias
 from forestadmin.datasource_toolkit.utils.records import RecordUtils
 
 
 class ActionContextBulk(ActionContext):
     async def get_records_ids(self) -> List[CompositeIdAlias]:
         projection = Projection().with_pks(self.collection)
         records = await self.get_records(projection)
-        return [RecordUtils.get_primary_key(self.collection.schema, record) for record in records]
-
-    async def get_records(self, fields: Projection) -> Any:
-        return await super(ActionContextBulk, self).get_records(fields)
+        return [RecordUtils.get_primary_key(self.collection.schema, record)[0] for record in records]
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/result_builder.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/result_builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sys
-from io import BytesIO
+from io import IOBase
 
 if sys.version_info >= (3, 8):
-    from typing import Literal
+    from typing import Literal, TypedDict
 else:
-    from typing_extensions import Literal
+    from typing_extensions import Literal, TypedDict
 
-from typing import Any, Dict, List, Optional, TypedDict, Union
+from typing import Any, Dict, List, Optional, Union
 
 from forestadmin.datasource_toolkit.interfaces.actions import ActionResult
 from forestadmin.datasource_toolkit.interfaces.records import RecordsDataAlias
 from typing_extensions import NotRequired
 
 OptionTypeAlias = Union[Literal["html"], Literal["text"]]
 WebhookMethod = Union[Literal["GET"], Literal["POST"]]
@@ -37,27 +37,33 @@
             "type": cls.SUCCESS,
             "message": message or cls.SUCCESS,
             "format": options.get("type", "text"),
             "invalidated": set(options.get("invalidated", [])),
         }
 
     @classmethod
-    def error(cls, message: Optional[str] = None) -> ActionResult:
-        return {"type": cls.ERROR, "message": message or cls.ERROR}
+    def error(cls, message: Optional[str] = None, options: Optional[OptionAlias] = None) -> ActionResult:
+        if not options:
+            options = {}
+        return {
+            "type": cls.ERROR,
+            "message": message or cls.ERROR,
+            "format": options.get("type", "text"),
+        }
 
     @classmethod
     def webhook(
         cls,
         url: str,
         method: WebhookMethod = "POST",
         headers: Optional[RecordsDataAlias] = None,
         body: Optional[Dict[str, Any]] = None,
     ) -> ActionResult:
         return {"type": cls.WEBHOOK, "url": url, "method": method, "headers": headers or {}, "body": body or {}}
 
     @classmethod
-    def file(cls, file: BytesIO, name: str = "file", mime_type: str = "text/plain") -> ActionResult:
+    def file(cls, file: IOBase, name: str = "file", mime_type: str = "text/plain") -> ActionResult:
         return {"type": cls.FILE, "name": name, "mimeType": mime_type, "stream": file}
 
     @classmethod
     def redirect(cls, path: str) -> ActionResult:
         return {"type": cls.REDIRECT, "path": path}
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/types/actions.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/types/actions.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,25 +8,24 @@
 from forestadmin.datasource_toolkit.decorators.action.types.fields import DynamicField, FieldFactory, PlainDynamicField
 from forestadmin.datasource_toolkit.interfaces.actions import ActionResult, ActionsScope
 
 Context = TypeVar("Context", bound=ActionContext)
 
 
 class BaseAction(Generic[Context]):
-
     SCOPE: ActionsScope
     FORM: Sequence[PlainDynamicField] = []
     GENERATE_FILE: bool = False
 
     def __init__(self):
         self.form = self._build_form(self.FORM)  # type: ignore
 
     @abc.abstractmethod
     async def execute(self, context: Context, result_builder: ResultBuilder) -> Union[None, ActionResult]:
-        pass
+        """The main function of the action"""
 
     def _build_form(self, plain_fields: Sequence[PlainDynamicField]) -> List[DynamicField[Context]]:
         form: List[DynamicField[Context]] = []
         for plain_field in plain_fields:
             form.append(FieldFactory[Context].build(plain_field))
         return form
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/types/fields.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/action/types/fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,31 @@
-from typing import Any, Awaitable, Callable, Generic, List, Optional, TypedDict, TypeVar, Union
+import sys
+
+if sys.version_info >= (3, 8):
+    from typing import TypedDict
+else:
+    from typing_extensions import TypedDict
+
+from typing import Any, Awaitable, Callable, Generic, List, Optional, TypeVar, Union
 
 from forestadmin.datasource_toolkit.decorators.action.context.base import ActionContext
 from forestadmin.datasource_toolkit.exceptions import DatasourceToolkitException
 from forestadmin.datasource_toolkit.interfaces.actions import ActionField, ActionFieldType, File
 from forestadmin.datasource_toolkit.interfaces.records import CompositeIdAlias
-from typing_extensions import NotRequired, Self
+from typing_extensions import NotRequired
 
 Context = TypeVar("Context", bound=ActionContext)
 Result = TypeVar("Result")
 
 ValueOrHandler = Union[Callable[[Context], Awaitable[Result]], Callable[[Context], Result], Result]
 
 
 class PlainBaseDynamicField(TypedDict):
     label: str
-    description: str
+    description: NotRequired[str]
     is_required: NotRequired[bool]
     is_read_only: NotRequired[bool]
 
 
 class PlainField(PlainBaseDynamicField):
     type: ActionFieldType
 
@@ -26,15 +33,15 @@
 class BaseDynamicField(Generic[Context, Result]):
     ATTR_TO_EVALUATE = ("is_required", "is_read_only", "if_", "value", "default_value")
     TYPE: ActionFieldType
 
     def __init__(
         self,
         label: str,
-        description: str,
+        description: Optional[str] = "",
         is_required: Optional[ValueOrHandler[Context, bool]] = False,
         is_read_only: Optional[ValueOrHandler[Context, bool]] = False,
         if_: Optional[ValueOrHandler[Context, Any]] = None,
         value: Optional[ValueOrHandler[Context, Result]] = None,
         default_value: Optional[ValueOrHandler[Context, Result]] = None,
     ):
         self.label = label
@@ -50,25 +57,25 @@
         return [self._is_required, self._is_read_only, self._if_, self._value, self._default_value]
 
     @property
     def is_dynamic(self):
         return any(map(lambda x: isinstance(x, Callable), self.dynamic_fields))
 
     async def to_action_field(self, context: Context, default_value: Result) -> ActionField:
-        return {
-            "type": self.TYPE,
-            "label": self.label,
-            "description": self.description,
-            "is_read_only": await self.is_read_only(context),
-            "is_required": await self.is_required(context),
-            "value": await self.value(context) or default_value,
-            "collection_name": None,
-            "enum_values": None,
-            "watch_changes": False,
-        }
+        return ActionField(
+            type=self.TYPE,
+            label=self.label,
+            description=self.description,
+            is_read_only=await self.is_read_only(context),
+            is_required=await self.is_required(context),
+            value=await self.value(context) or default_value,
+            collection_name=None,
+            enum_values=None,
+            watch_changes=False,
+        )
 
     async def default_value(self, context: Context) -> Result:
         return await self._evaluate(context, self._default_value)
 
     async def is_required(self, context: Context) -> bool:
         return await self._evaluate(context, self._is_required)
 
@@ -83,82 +90,91 @@
 
     async def _evaluate(self, context: Context, attribute: ValueOrHandler[ActionContext, Any]):
         if isinstance(attribute, Callable):
             res = attribute(context)
             if isinstance(res, Awaitable):
                 return await res
             return res
+        # ugly hack for static or classmethod in python<3.10
+        # https://stackoverflow.com/questions/41921255/staticmethod-object-is-not-callable
+        elif hasattr(attribute, "__func__") and isinstance(attribute.__func__, Callable):
+            res = attribute.__func__(context)
+            if isinstance(res, Awaitable):
+                return await res
+            return res
         else:
             return attribute
 
-    @classmethod
-    def from_plain_field(cls, plain_field: PlainBaseDynamicField) -> Self:
-        return cls(**plain_field)
+    # @classmethod
+    # def from_plain_field(cls, plain_field: PlainBaseDynamicField) -> Self:
+    #     return cls(**plain_field)
 
 
 class PlainCollectionDynamicField(PlainField):
     collection_name: ValueOrHandler[ActionContext, str]
     if_: NotRequired[ValueOrHandler[ActionContext, Any]]
     value: NotRequired[ValueOrHandler[ActionContext, CompositeIdAlias]]
     default_value: NotRequired[ValueOrHandler[ActionContext, CompositeIdAlias]]
 
 
+# collection
 class CollectionDynamicField(Generic[Context], BaseDynamicField[Context, CompositeIdAlias]):
     TYPE = ActionFieldType.COLLECTION
 
     def __init__(
         self,
         collection_name: ValueOrHandler[Context, str],
         label: str,
-        description: str,
+        description: Optional[str] = "",
         is_required: Optional[ValueOrHandler[Context, bool]] = False,
         is_read_only: Optional[ValueOrHandler[Context, bool]] = False,
         if_: Optional[Awaitable[Any]] = None,
         value: Optional[ValueOrHandler[Context, CompositeIdAlias]] = None,
         default_value: Optional[ValueOrHandler[Context, CompositeIdAlias]] = None,
     ):
-        super(CollectionDynamicField[Context], self).__init__(
+        super(CollectionDynamicField, self).__init__(
             label, description, is_required, is_read_only, if_, value, default_value
         )
         self._collection_name = collection_name
 
     @property
     def dynamic_fields(self):
-        return [*super(CollectionDynamicField[Context], self).dynamic_fields, self._collection_name]
+        return [*super(CollectionDynamicField, self).dynamic_fields, self._collection_name]
 
     async def collection_name(self, context: Context) -> str:
         return await self._evaluate(context, self._collection_name)
 
     async def to_action_field(self, context: Context, default_value: CompositeIdAlias) -> ActionField:
-        res = await super(CollectionDynamicField[Context], self).to_action_field(context, default_value)
+        res = await super(CollectionDynamicField, self).to_action_field(context, default_value)
         res["collection_name"] = await self.collection_name(context)
         return res
 
-    @classmethod
-    def from_plain_field(  # type: ignore
-        cls, plain_field: PlainCollectionDynamicField
-    ) -> Self:  # type: ignore
-        return cls(**plain_field)  # type: ignore
+    # @classmethod
+    # def from_plain_field(  # type: ignore
+    #     cls, plain_field: PlainCollectionDynamicField
+    # ) -> Self:  # type: ignore
+    #     return cls(**plain_field)  # type: ignore
 
 
+# enum
 class PlainEnumDynamicField(PlainField):
     enum_values: ValueOrHandler[ActionContext, List[str]]
     if_: NotRequired[ValueOrHandler[ActionContext, Any]]
     value: NotRequired[ValueOrHandler[ActionContext, str]]
     default_value: NotRequired[ValueOrHandler[ActionContext, str]]
 
 
 class EnumDynamicField(BaseDynamicField[Context, str], Generic[Context]):
     TYPE = ActionFieldType.ENUM
 
     def __init__(
         self,
         enum_values: ValueOrHandler[Context, List[str]],
         label: str,
-        description: str,
+        description: Optional[str] = "",
         is_required: Optional[ValueOrHandler[Context, bool]] = False,
         is_read_only: Optional[ValueOrHandler[Context, bool]] = False,
         if_: Optional[Awaitable[Any]] = None,
         value: Optional[ValueOrHandler[Context, str]] = None,
         default_value: Optional[ValueOrHandler[Context, str]] = None,
     ):
         super().__init__(label, description, is_required, is_read_only, if_, value, default_value)
@@ -172,155 +188,204 @@
         return await self._evaluate(context, self._enum_values)
 
     async def to_action_field(self, context: Context, default_value: str) -> ActionField:
         res = await super().to_action_field(context, default_value)
         res["enum_values"] = await self.enum_values(context)
         return res
 
-    @classmethod
-    def from_plain_field(cls, plain_field: PlainEnumDynamicField[Context, List[str]]) -> Self:  # type: ignore
-        return cls(**plain_field)  # type: ignore
+    # @classmethod
+    # def from_plain_field(cls, plain_field: PlainEnumDynamicField) -> Self:  # type: ignore
+    #     return cls(**plain_field)  # type: ignore
 
 
+# enum list
 class PlainListEnumDynamicField(PlainField):
     enum_values: ValueOrHandler[ActionContext, List[str]]
     if_: NotRequired[ValueOrHandler[ActionContext, Any]]
     value: NotRequired[ValueOrHandler[ActionContext, List[str]]]
     default_value: NotRequired[ValueOrHandler[ActionContext, List[str]]]
 
 
 class EnumListDynamicField(Generic[Context], BaseDynamicField[Context, List[str]]):
     TYPE = ActionFieldType.ENUM_LIST
 
     def __init__(
         self,
         enum_values: ValueOrHandler[Context, List[str]],
         label: str,
-        description: str,
+        description: Optional[str] = "",
         is_required: Optional[ValueOrHandler[Context, bool]] = False,
         is_read_only: Optional[ValueOrHandler[Context, bool]] = False,
         if_: Optional[Awaitable[Any]] = None,
         value: Optional[ValueOrHandler[Context, List[str]]] = None,
         default_value: Optional[ValueOrHandler[Context, List[str]]] = None,
     ):
-        super(EnumListDynamicField[Context], self).__init__(
+        super(EnumListDynamicField, self).__init__(
             label, description, is_required, is_read_only, if_, value, default_value
         )
         self._enum_values = enum_values
 
     @property
     def dynamic_fields(self):
-        return [*super(EnumListDynamicField[Context], self).dynamic_fields, self._enum_values]
+        return [*super(EnumListDynamicField, self).dynamic_fields, self._enum_values]
 
     async def enum_values(self, context: Context) -> List[str]:
         return await self._evaluate(context, self._enum_values)
 
     async def to_action_field(self, context: Context, default_value: List[str]) -> ActionField:
-        res = await super(EnumListDynamicField[Context], self).to_action_field(context, default_value)
+        res = await super(EnumListDynamicField, self).to_action_field(context, default_value)
         res["enum_values"] = await self.enum_values(context)
+        if res["value"] is None:
+            res["value"] = []
         return res
 
-    @classmethod
-    def from_plain_field(cls, plain_field: PlainListEnumDynamicField[Context, List[str]]) -> Self:  # type: ignore
-        return cls(**plain_field)  # type: ignore
+    # unused ???
+    # @classmethod
+    # def from_plain_field(cls, plain_field: PlainListEnumDynamicField) -> Self:  # type: ignore
+    #     return cls(**plain_field)  # type: ignore
 
 
+# boolean
 class PlainBooleanDynamicField(PlainField):
     if_: NotRequired[ValueOrHandler[ActionContext, Any]]
     value: NotRequired[ValueOrHandler[ActionContext, bool]]
     default_value: NotRequired[ValueOrHandler[ActionContext, bool]]
 
 
 class BooleanDynamicField(Generic[Context], BaseDynamicField[Context, bool]):
     TYPE = ActionFieldType.BOOLEAN
 
 
+# number
 class PlainNumberDynamicField(PlainField):
     if_: NotRequired[ValueOrHandler[ActionContext, Any]]
     value: NotRequired[ValueOrHandler[ActionContext, Union[int, float]]]
     default_value: NotRequired[ValueOrHandler[ActionContext, Union[int, float]]]
 
 
 class NumberDynamicField(Generic[Context], BaseDynamicField[Context, Union[int, float]]):
     TYPE = ActionFieldType.NUMBER
 
 
+# number list
 class PlainListNumberDynamicField(PlainField):
     if_: NotRequired[ValueOrHandler[ActionContext, Any]]
     value: NotRequired[ValueOrHandler[ActionContext, Union[int, float]]]
     default_value: NotRequired[ValueOrHandler[ActionContext, Union[int, float]]]
 
 
 class NumberListDynamicField(Generic[Context], BaseDynamicField[Context, List[Union[int, float]]]):
     TYPE = ActionFieldType.NUMBER_LIST
 
 
+# string
+class PlainStringDynamicField(PlainField):
+    if_: NotRequired[ValueOrHandler[ActionContext, Any]]
+    value: NotRequired[ValueOrHandler[ActionContext, str]]
+    default_value: NotRequired[ValueOrHandler[ActionContext, str]]
+
+
+class StringDynamicField(Generic[Context], BaseDynamicField[Context, str]):
+    TYPE = ActionFieldType.STRING
+
+
+# string list
+class PlainStringListDynamicField(PlainField):
+    if_: NotRequired[ValueOrHandler[ActionContext, Any]]
+    value: NotRequired[ValueOrHandler[ActionContext, str]]
+    default_value: NotRequired[ValueOrHandler[ActionContext, str]]
+
+
+class StringListDynamicField(Generic[Context], BaseDynamicField[Context, str]):
+    TYPE = ActionFieldType.STRING_LIST
+
+
+# json
 class PlainJsonDynamicField(PlainField):
     if_: NotRequired[ValueOrHandler[ActionContext, Any]]
     value: NotRequired[ValueOrHandler[ActionContext, str]]
     default_value: NotRequired[ValueOrHandler[ActionContext, str]]
 
 
 class JsonDynamicField(Generic[Context], BaseDynamicField[Context, str]):
     TYPE = ActionFieldType.JSON
 
 
+# file
 class FileDynamicField(Generic[Context], BaseDynamicField[Context, File]):
     TYPE = ActionFieldType.FILE
 
 
 class PlainFileDynamicField(PlainField):
     if_: NotRequired[ValueOrHandler[ActionContext, Any]]
     value: NotRequired[ValueOrHandler[ActionContext, File]]
     default_value: NotRequired[ValueOrHandler[ActionContext, File]]
 
 
+# file list
+class FileListDynamicField(Generic[Context], BaseDynamicField[Context, File]):
+    TYPE = ActionFieldType.FILE_LIST
+
+
+class PlainFileListDynamicField(PlainField):
+    if_: NotRequired[ValueOrHandler[ActionContext, Any]]
+    value: NotRequired[ValueOrHandler[ActionContext, File]]
+    default_value: NotRequired[ValueOrHandler[ActionContext, File]]
+
+
 DynamicField = Union[
     BooleanDynamicField[Context],
     CollectionDynamicField[Context],
     EnumDynamicField[Context],
     EnumListDynamicField[Context],
     NumberDynamicField[Context],
+    StringDynamicField[Context],
     NumberListDynamicField[Context],
     JsonDynamicField[Context],
     FileDynamicField[Context],
 ]
 
 PlainDynamicField = Union[
     PlainBooleanDynamicField,
     PlainCollectionDynamicField,
     PlainEnumDynamicField,
     PlainListEnumDynamicField,
     PlainNumberDynamicField,
+    PlainStringDynamicField,
     PlainListNumberDynamicField,
     PlainJsonDynamicField,
     PlainFileDynamicField,
 ]
 
 
 class FieldFactoryException(DatasourceToolkitException):
     pass
 
 
 class FieldFactory(Generic[Context]):
-
     FIELD_FOR_TYPE: Any = {
         ActionFieldType.COLLECTION: CollectionDynamicField,
         ActionFieldType.NUMBER: NumberDynamicField,
+        ActionFieldType.NUMBER_LIST: NumberListDynamicField,
+        ActionFieldType.STRING: StringDynamicField,
+        ActionFieldType.STRING_LIST: StringListDynamicField,
         ActionFieldType.BOOLEAN: BooleanDynamicField,
         ActionFieldType.ENUM: EnumDynamicField,
+        ActionFieldType.ENUM_LIST: EnumListDynamicField,
         ActionFieldType.JSON: JsonDynamicField,
         ActionFieldType.FILE: FileDynamicField,
+        ActionFieldType.FILE_LIST: FileListDynamicField,
     }
 
     @classmethod
     def build(cls, plain_field: PlainDynamicField) -> DynamicField[Context]:
         try:
             cls_field = cls.FIELD_FOR_TYPE[plain_field["type"]]
         except KeyError:
             raise FieldFactoryException(f"Unknown field type: '{plain_field['type']}'")
 
-        del plain_field["type"]  # type: ignore
+        _plain_field = {**plain_field}
+        del _plain_field["type"]  # type: ignore
         try:
-            return cls_field(**plain_field)
+            return cls_field(**_plain_field)
         except (TypeError, AttributeError) as e:
             raise FieldFactoryException(f"Unable to build a field. cls: '{cls_field.__name__}', e: '{e}'")
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/computed/collections.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/computed/collections.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,84 @@
-from typing import Any, Callable, Dict, List, Optional, cast
+from typing import Any, Dict, List, Optional, Union, cast
 
+from forestadmin.agent_toolkit.utils.context import User
 from forestadmin.datasource_toolkit.context.collection_context import CollectionCustomizationContext
-from forestadmin.datasource_toolkit.decorators.computed.exceptions import ComputedMixinException
-from forestadmin.datasource_toolkit.decorators.computed.helpers import (  # type: ignore
-    compute_aggregate_from_records,
-    compute_from_records,
-    computed_aggregation_projection,
-    rewrite_fields,
-)
+from forestadmin.datasource_toolkit.decorators.collection_decorator import CollectionDecorator
+from forestadmin.datasource_toolkit.decorators.computed.exceptions import ComputedDecoratorException
+from forestadmin.datasource_toolkit.decorators.computed.helpers import compute_from_records, rewrite_fields
 from forestadmin.datasource_toolkit.decorators.computed.types import ComputedDefinition
 from forestadmin.datasource_toolkit.exceptions import DatasourceToolkitException
 from forestadmin.datasource_toolkit.interfaces.collections import Collection
-from forestadmin.datasource_toolkit.interfaces.fields import FieldAlias, FieldType
+from forestadmin.datasource_toolkit.interfaces.fields import FieldType, RelationAlias
 from forestadmin.datasource_toolkit.interfaces.models.collections import CollectionSchema
 from forestadmin.datasource_toolkit.interfaces.query.aggregation import AggregateResult, Aggregation
 from forestadmin.datasource_toolkit.interfaces.query.filter.paginated import PaginatedFilter
 from forestadmin.datasource_toolkit.interfaces.query.filter.unpaginated import Filter
 from forestadmin.datasource_toolkit.interfaces.query.projections import Projection
 from forestadmin.datasource_toolkit.interfaces.records import RecordsDataAlias
 from forestadmin.datasource_toolkit.validations.field import FieldValidator
 from typing_extensions import Self
 
 
-class ComputedMixin:
-
-    name: str
-    get_field: Callable[[str], FieldAlias]
-    datasource: property
-    mark_schema_as_dirty: Callable[..., None]
-
+class ComputedCollectionDecorator(CollectionDecorator):
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self._computeds: Dict[str, ComputedDefinition] = {}
 
-    def get_computed(self, path: str) -> ComputedDefinition:
+    def get_computed(self, path: str) -> Union[ComputedDefinition, None]:
         if ":" not in path:
             try:
                 return self._computeds[path]
             except KeyError:
-                raise ComputedMixinException(f"{path} is not a computed field")
+                return None
 
-        collection_name, path = path.split(":")
-        foreign_collection: Self = self.datasource.get_collection(collection_name)
+        related_field, path = path.split(":")
+        field = cast(RelationAlias, self.get_field(related_field))
+        foreign_collection: Self = self.datasource.get_collection(field["foreign_collection"])
         return foreign_collection.get_computed(path)
 
     def register_computed(self, name: str, computed: ComputedDefinition):
+        if computed.get("dependencies") is None or len(computed["dependencies"]) == 0:
+            raise ComputedDecoratorException(f"Computed field '{self.name}.{name}' must have at least one dependency")
         for field in computed["dependencies"]:
             try:
-                FieldValidator.validate(self, field)  # type: ignore
+                FieldValidator.validate(self.child_collection, field)  # type: ignore
             except DatasourceToolkitException:
-                raise ComputedMixinException(
+                raise ComputedDecoratorException(
                     f"The dependency {field} of the computed field {name} is unknown in the collection {self.name}"
                 )
         self._computeds[name] = computed
         self.mark_schema_as_dirty()
 
-    async def list(self, filter: PaginatedFilter, projection: Projection) -> List[RecordsDataAlias]:
+    async def list(self, caller: User, _filter: PaginatedFilter, projection: Projection) -> List[RecordsDataAlias]:
         new_projection = projection.replace(lambda path: rewrite_fields(self, path))
-        records: List[Optional[RecordsDataAlias]] = await super().list(filter, new_projection)  # type: ignore
-        context = CollectionCustomizationContext(cast(Collection, self), filter.timezone)
+        records: List[Optional[RecordsDataAlias]] = await super().list(caller, _filter, new_projection)  # type: ignore
+        context = CollectionCustomizationContext(cast(Collection, self), caller)
         return await compute_from_records(context, self, new_projection, projection, records)
 
     async def aggregate(
-        self, filter: Optional[Filter], aggregation: Aggregation, limit: Optional[int] = None
+        self, caller: User, _filter: Optional[Filter], aggregation: Aggregation, limit: Optional[int] = None
     ) -> List[AggregateResult]:
-        is_computed = any([field in self._computeds for field in cast(List[str], aggregation.projection)])
-        if is_computed:
-            aggregation, new_to_old_group = computed_aggregation_projection(self, aggregation)  # type: ignore
-        records: List[AggregateResult] = await super().aggregate(filter, aggregation, limit)  # type: ignore
-        if is_computed:
-            records = compute_aggregate_from_records(records, new_to_old_group)  # type: ignore
-        return records
-
-    @property
-    def schema(self) -> CollectionSchema:
-        schema: CollectionSchema = super(ComputedMixin, self).schema  # type: ignore
+        if not any([self.get_computed(field) for field in aggregation.projection]):
+            return await self.child_collection.aggregate(caller, _filter, aggregation, limit)
+
+        records = await self.list(caller, _filter, aggregation.projection)
+        return aggregation.apply(
+            records,
+            caller.timezone,
+        )
+
+    def _refine_schema(self, sub_schema: CollectionSchema) -> CollectionSchema:
+        computed_fields_schema = {**sub_schema["fields"]}
         for name, computed in self._computeds.items():
-            schema["fields"][name] = {
+            computed_fields_schema[name] = {
                 "column_type": computed["column_type"],
                 "default_value": computed.get("default_value", None),
                 "type": FieldType.COLUMN,
                 "enum_values": computed.get("enum_values", None),
                 "filter_operators": set(),
                 "is_primary_key": False,
                 "is_read_only": True,
                 "is_sortable": False,
                 "validations": None,
             }
-        return schema
+        return {**sub_schema, "fields": computed_fields_schema}
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/computed/helpers.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/computed/helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 import copy
-from typing import Any, Dict, List, Optional, Tuple, cast
+from typing import Any, Awaitable, List, Optional, Tuple, cast
 
 from forestadmin.datasource_toolkit.context.collection_context import CollectionCustomizationContext
-from forestadmin.datasource_toolkit.decorators.computed.exceptions import ComputedMixinException
 from forestadmin.datasource_toolkit.decorators.computed.types import ComputedDefinition
 from forestadmin.datasource_toolkit.decorators.computed.utils import Output, flatten, transform_unique_values, unflatten
-from forestadmin.datasource_toolkit.interfaces.collections import Collection
 from forestadmin.datasource_toolkit.interfaces.fields import RelationAlias
-from forestadmin.datasource_toolkit.interfaces.query.aggregation import (
-    AggregateResult,
-    Aggregation,
-    PlainAggregationGroup,
-)
 from forestadmin.datasource_toolkit.interfaces.query.projections import Projection
 from forestadmin.datasource_toolkit.interfaces.records import RecordsDataAlias
 
 
 def rewrite_fields(collection: Any, path: str) -> Projection:
     if ":" in path:
         prefix = path.split(":")[0]
         schema = cast(RelationAlias, collection.get_field(prefix))
         association = collection.datasource.get_collection(schema["foreign_collection"])
         return Projection(path).unnest().replace(lambda sub_path: rewrite_fields(association, sub_path)).nest(prefix)
-    try:
-        computed = collection.get_computed(path)
-    except ComputedMixinException:
+
+    computed = collection.get_computed(path)
+    if computed is None:
         return Projection(path)
     else:
         return Projection(*computed["dependencies"]).replace(lambda dep_path: rewrite_fields(collection, dep_path))
 
 
 async def compute_field(
     context: CollectionCustomizationContext,
     computed: ComputedDefinition,
     paths: List[str],
     dependency_values: List[List[Any]],
 ) -> List[Output]:
     async def _compute_field_cb(unique_partials: List[RecordsDataAlias]) -> Output:
-        return await computed["get_values"](unique_partials, context)
+        ret = computed["get_values"](unique_partials, context)
+        if isinstance(ret, Awaitable):
+            ret = await ret
+        return ret
 
     return await transform_unique_values(unflatten(dependency_values, Projection(*paths)), _compute_field_cb)
 
 
 async def queue_field(
     ctx: CollectionCustomizationContext,
     collection: Any,
@@ -49,16 +45,17 @@
     paths: List[str],
     flatten_records: List[List[Any]],
 ):
     if new_path not in paths:
         computed = collection.get_computed(new_path)
         dependencies = Projection(*computed["dependencies"])
         if ":" in new_path:
-            dependencies = cast(List[str], dependencies.nest(new_path.split(":")[0])).sort()
-
+            nested_field = new_path.split(":")[0]
+            dependencies = cast(List[str], dependencies.nest(nested_field))
+            dependencies.sort()
         for path in cast(List[str], dependencies):
             await queue_field(ctx, collection, path, paths, flatten_records.copy())
         dependency_values = [flatten_records[paths.index(path)] for path in cast(List[str], dependencies)]
         paths.append(new_path)
 
         return await compute_field(ctx, computed, computed["dependencies"], copy.deepcopy(dependency_values)) or []
 
@@ -92,35 +89,7 @@
     for i in delete_operations:
         del flatten_records[i]
 
     for i, value in add_operations:
         flatten_records.insert(i, value)
 
     return [u for u in unflatten(flatten_records, desired_projections) if u]
-
-
-def computed_aggregation_projection(
-    collection: Collection,
-    aggregation: Aggregation,
-):
-    plain_aggregation = aggregation._to_plain  # type: ignore
-    if plain_aggregation.get("field"):
-        plain_aggregation["field"] = rewrite_fields(collection, plain_aggregation["field"])  # type: ignore
-
-    new_to_old_group: Dict[str, str] = {}
-    groups: List[PlainAggregationGroup] = []
-    for group in plain_aggregation.get("groups", []):
-        new: str = rewrite_fields(collection, group["field"])[0]
-        new_to_old_group[new] = group["field"]  # type: ignore
-        group["field"] = new
-        groups.append(group)
-    plain_aggregation["groups"] = groups
-    return Aggregation(plain_aggregation), new_to_old_group
-
-
-def compute_aggregate_from_records(
-    records: List[AggregateResult], new_to_old_group: Dict[str, str]
-) -> List[AggregateResult]:
-    for record in records:
-        key, value = next(iter(record["group"].items()))
-        record["group"] = {f"{new_to_old_group[key]}": value}
-    return records
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/computed/utils.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/computed/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 
 
 async def transform_unique_values(inputs: Input, callback: Callable[[List[Input]], Awaitable[List[Output]]]):
     indexes: Dict[int, int] = {}
     mapping: List[int] = []
     unique_inputs: List[Input] = []
 
-    for input in inputs:
-        if input is not None:
-            if isinstance(input, dict):
-                hsh = hash(json.dumps(input, default=str))
+    for _input in inputs:
+        if _input is not None:
+            if isinstance(_input, dict):
+                hsh = hash(json.dumps(_input, default=str))
             else:
-                hsh = hash(input)
+                hsh = hash(_input)
             if hsh not in indexes:
                 indexes[hsh] = len(unique_inputs)
-                unique_inputs.append(input)
+                unique_inputs.append(_input)
             mapping.append(indexes[hsh])
         else:
             mapping.append(-1)
 
     unique_outputs = await callback(unique_inputs)
     outputs: List[Output] = []
 
@@ -53,15 +53,15 @@
         num_records = 0
 
     records: List[Dict[str, Any]] = [{} for _ in range(0, num_records)]
 
     for column in projection.columns:
         path_index: int = projection.index(column)  # type: ignore
         for idx, value in enumerate(flats[path_index]):
-            records[idx][column] = value or None
+            records[idx][column] = value
 
     for relation, paths in projection.relations.items():
         sub_flats = [flats[projection.index(f"{relation}:{path}")] for path in paths]  # type: ignore
         sub_records = unflatten(sub_flats, paths)
         for idx in range(len(records)):
             records[idx][relation] = sub_records[idx]
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/datasource.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/context/agent_context.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from typing import Any
+from forestadmin.agent_toolkit.utils.context import User
+from forestadmin.datasource_toolkit.context.relaxed_wrappers.collection import RelaxedDatasource
+from forestadmin.datasource_toolkit.interfaces.collections import Collection
+from forestadmin.datasource_toolkit.interfaces.models.collections import Datasource
 
-from forestadmin.datasource_toolkit.datasources import Datasource
-from forestadmin.datasource_toolkit.decorators.collections import CustomizedCollection
-from forestadmin.datasource_toolkit.interfaces.models.collections import BoundCollection
 
+class AgentCustomizationContext:
+    def __init__(self, datasource: Datasource[Collection], caller: User):
+        self._datasource = datasource
+        self._caller = caller
 
-class CustomizedDatasource(Datasource[CustomizedCollection]):  # type: ignore
-    def __init__(self, child_datasource: Datasource[BoundCollection]):
-        super().__init__()
-        self.child_datasource = child_datasource
+    @property
+    def datasource(self) -> RelaxedDatasource:
+        return RelaxedDatasource(self._datasource)
 
-    def __getattr__(self, __name: str) -> Any:
-        return getattr(self.child_datasource, __name)
+    @property
+    def caller(self) -> User:
+        return self._caller
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/operators_replace/collections.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 from typing import Any, Dict, Optional, Set, Union
 
+from forestadmin.agent_toolkit.utils.context import User
+from forestadmin.datasource_toolkit.decorators.collection_decorator import CollectionDecorator
 from forestadmin.datasource_toolkit.interfaces.fields import FieldAlias, Operator, is_column
 from forestadmin.datasource_toolkit.interfaces.models.collections import CollectionSchema
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.equivalence import ConditionTreeEquivalent
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.base import ConditionTree
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.leaf import ConditionTreeLeaf
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.operators import ALL_OPERATORS
 from forestadmin.datasource_toolkit.interfaces.query.filter.paginated import PaginatedFilter
 from forestadmin.datasource_toolkit.interfaces.query.filter.unpaginated import Filter
 from forestadmin.datasource_toolkit.utils.collections import CollectionUtils
 
 
-class OperatorReplaceMixin:
+class OperatorEquivalenceCollectionDecorator(CollectionDecorator):
     def __init__(self, *args: Any, **kwargs: Any):
-        super(OperatorReplaceMixin, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self._allowed_operator: Dict[str, Set[Operator]] = {}
+        self.mark_schema_as_dirty()
 
-    @property
-    def schema(self) -> CollectionSchema:
-        schema: CollectionSchema = super(OperatorReplaceMixin, self).schema  # type: ignore
+    def _refine_schema(self, sub_schema: CollectionSchema) -> CollectionSchema:
         fields: Dict[str, FieldAlias] = {}
 
-        for name, field_schema in schema["fields"].items():
-            if is_column(field_schema) and name not in self._allowed_operator:
-                self._allowed_operator[name] = field_schema.get("filter_operators") or set()
+        for name, field_schema in sub_schema["fields"].items():
+            if is_column(field_schema):
+                if name not in self._allowed_operator:
+                    self._allowed_operator[name] = field_schema.get("filter_operators") or set()
+
                 new_operators: Set[Operator] = set(
                     filter(
                         lambda operator: ConditionTreeEquivalent.has_equivalent_tree(
                             operator,
                             field_schema.get("filter_operators", []),  # type: ignore
                             field_schema.get("column_type"),  # type: ignore
                         ),
                         ALL_OPERATORS,
                     )
                 )
                 fields[name] = {**field_schema, "filter_operators": new_operators}  # type: ignore
             else:
                 fields[name] = field_schema
-
-        return {**schema, "fields": fields}
+        sub_schema = {**sub_schema, "fields": fields}
+        return sub_schema
 
     async def _refine_filter(
-        self, filter: Union[Optional[PaginatedFilter], Optional[Filter]]
+        self, caller: User, _filter: Union[Optional[PaginatedFilter], Optional[Filter]]
     ) -> Optional[Union[PaginatedFilter, Filter]]:
         def refine_equivalent_tree(tree: ConditionTree) -> ConditionTree:
             if isinstance(tree, ConditionTreeLeaf):
-                field_schema = CollectionUtils.get_field_schema(self, tree.field)  # type: ignore
+                collection = self
+                field = tree.field
+                if ":" in tree.field:
+                    parent_name, field = tree.field.split(":")
+                    parent_field = self.get_field(parent_name)
+                    collection = self.datasource.get_collection(parent_field["foreign_collection"])  # type: ignore
+                field_schema = CollectionUtils.get_field_schema(collection, field)  # type: ignore
                 if is_column(field_schema):
                     res = ConditionTreeEquivalent.get_equivalent_tree(
                         tree,
-                        self._allowed_operator[tree.field],
+                        collection._allowed_operator[field],
                         field_schema["column_type"],
-                        filter.timezone,  # type: ignore
+                        _filter.timezone,  # type: ignore
                     )
                     if res:
                         return res
             return tree
 
-        filter = await super()._refine_filter(filter)  # type: ignore
-        if filter and filter.condition_tree:
-            filter = filter.override({"condition_tree": filter.condition_tree.replace(refine_equivalent_tree)})
-        return filter
+        _filter = await super()._refine_filter(caller, _filter)  # type: ignore
+        if _filter and _filter.condition_tree:
+            _filter = _filter.override({"condition_tree": _filter.condition_tree.replace(refine_equivalent_tree)})
+        return _filter
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/proxy/collection.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/collection_decorator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,112 @@
 from typing import List, Optional, Union, cast
 
-from forestadmin.datasource_toolkit.collections import Collection
-from forestadmin.datasource_toolkit.datasources import Datasource
+from forestadmin.agent_toolkit.utils.context import User
+from forestadmin.datasource_toolkit.collections import CollectionException
 from forestadmin.datasource_toolkit.interfaces.actions import ActionField, ActionResult
-from forestadmin.datasource_toolkit.interfaces.models.collections import BoundCollection, CollectionSchema
+from forestadmin.datasource_toolkit.interfaces.chart import Chart
+from forestadmin.datasource_toolkit.interfaces.collections import Collection
+from forestadmin.datasource_toolkit.interfaces.models.collections import BoundCollection, CollectionSchema, Datasource
 from forestadmin.datasource_toolkit.interfaces.query.aggregation import AggregateResult, Aggregation
 from forestadmin.datasource_toolkit.interfaces.query.filter.paginated import PaginatedFilter
 from forestadmin.datasource_toolkit.interfaces.query.filter.unpaginated import Filter
 from forestadmin.datasource_toolkit.interfaces.query.projections import Projection
 from forestadmin.datasource_toolkit.interfaces.records import RecordsDataAlias
 
 
-class ProxyMixin:
+class CollectionDecorator(Collection):
     def __init__(self, collection: Collection, datasource: Datasource[BoundCollection]):
         self.child_collection = collection
-        self.child_collection._datasource = datasource  # type: ignore
-        self.child_collection._schema = self.schema  # type: ignore
+        self._datasource = datasource
+        self._last_schema = None
 
-    def __getattr__(self, name: str):
-        return getattr(self.child_collection, name)
+        if isinstance(self.child_collection, CollectionDecorator):
+            # ugly hack to mark parent schema as dirty
+            child_mark_schema_as_dirty = self.child_collection.mark_schema_as_dirty
+
+            def patched_mark_schema_as_dirty():
+                child_mark_schema_as_dirty()
+                self.mark_schema_as_dirty()
+
+            self.child_collection.mark_schema_as_dirty = patched_mark_schema_as_dirty
+
+    # def __getattr__(self, name: str):
+    #     return getattr(self.child_collection, name)
+
+    def mark_schema_as_dirty(self):
+        self._last_schema = None
+
+    @property
+    def datasource(self) -> Datasource:
+        return self._datasource
+
+    @property
+    def name(self) -> str:
+        return self.child_collection.name
 
     @property
     def schema(self) -> CollectionSchema:
-        return self.child_collection.schema
+        if self._last_schema is None:
+            self._last_schema = self._refine_schema(self.child_collection.schema)
+        return self._last_schema
+
+    def get_field(self, name: str):
+        try:
+            return self.schema["fields"][name]
+        except KeyError:
+            raise CollectionException(f"No such field {name} in the collection {self.name}")
+
+    def _refine_schema(self, sub_schema: CollectionSchema) -> CollectionSchema:
+        return sub_schema
 
     async def _refine_filter(
-        self, filter: Union[Filter, PaginatedFilter, None]
+        self, caller: User, _filter: Union[Filter, PaginatedFilter, None]
     ) -> Union[Filter, PaginatedFilter, None]:
-        return filter
+        return _filter
 
-    async def list(self, filter: PaginatedFilter, projection: Projection) -> List[RecordsDataAlias]:
+    async def list(self, caller: User, _filter: PaginatedFilter, projection: Projection) -> List[RecordsDataAlias]:
         try:
-            refined_filter = cast(PaginatedFilter, await self._refine_filter(filter))
+            refined_filter = cast(PaginatedFilter, await self._refine_filter(caller, _filter))
         except Exception:
             return []
         else:
-            return await self.child_collection.list(refined_filter, projection)  # type: ignore
+            return await self.child_collection.list(caller, refined_filter, projection)  # type: ignore
+
+    async def create(self, caller: User, data: List[RecordsDataAlias]) -> List[RecordsDataAlias]:
+        return await self.child_collection.create(caller, data)
 
-    async def create(self, data: List[RecordsDataAlias]) -> List[RecordsDataAlias]:
-        return await self.child_collection.create(data)
+    async def update(self, caller: User, _filter: Optional[Filter], patch: RecordsDataAlias) -> None:
+        refined_filter = cast(Optional[Filter], await self._refine_filter(caller, _filter))
+        return await self.child_collection.update(caller, refined_filter, patch)
+
+    async def delete(self, caller: User, _filter: Optional[Filter]) -> None:
+        refined_filter = cast(Optional[Filter], await self._refine_filter(caller, _filter))
+        return await self.child_collection.delete(caller, refined_filter)
+
+    async def aggregate(
+        self, caller: User, _filter: Optional[Filter], aggregation: Aggregation, limit: Optional[int] = None
+    ) -> List[AggregateResult]:
+        refined_filter = cast(Optional[Filter], await self._refine_filter(caller, _filter))
+        return await self.child_collection.aggregate(caller, refined_filter, aggregation, limit)
 
     async def execute(
         self,
+        caller: User,
         name: str,
         data: RecordsDataAlias,
-        filter: Optional[Filter],
+        _filter: Optional[Filter] = None,
     ) -> ActionResult:
-        refined_filter = cast(Filter, await self._refine_filter(filter))
-        return await self.child_collection.execute(name, data, refined_filter)
+        refined_filter = cast(Filter, await self._refine_filter(caller, _filter))
+        return await self.child_collection.execute(caller, name, data, refined_filter)
 
     async def get_form(
         self,
+        caller: User,
         name: str,
         data: Optional[RecordsDataAlias],
-        filter: Optional[Filter],
+        _filter: Optional[Filter] = None,
     ) -> List[ActionField]:
-        refined_filter = cast(Optional[Filter], await self._refine_filter(filter))
-        return await self.child_collection.get_form(name, data, refined_filter)
-
-    async def update(self, filter: Optional[Filter], patch: RecordsDataAlias) -> None:
-        refined_filter = cast(Optional[Filter], await self._refine_filter(filter))
-        return await self.child_collection.update(refined_filter, patch)
-
-    async def delete(self, filter: Optional[Filter]) -> None:
-        refined_filter = cast(Optional[Filter], await self._refine_filter(filter))
-        return await self.child_collection.delete(refined_filter)
+        refined_filter = cast(Optional[Filter], await self._refine_filter(caller, _filter))
+        return await self.child_collection.get_form(caller, name, data, refined_filter)
 
-    async def aggregate(
-        self, filter: Optional[Filter], aggregation: Aggregation, limit: Optional[int] = None
-    ) -> List[AggregateResult]:
-        refined_filter = cast(Optional[Filter], await self._refine_filter(filter))
-        return await self.child_collection.aggregate(refined_filter, aggregation, limit)
+    async def render_chart(self, caller: User, name: str, record_id: List) -> Chart:
+        return await self.child_collection.render_chart(caller, name, record_id)
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/rename/collections.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/rename_field/collections.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from typing import Any, Callable, Dict, List, Optional, Union, cast
+from typing import Any, Dict, List, Optional, Union, cast
 
+from forestadmin.agent_toolkit.utils.context import User
+from forestadmin.datasource_toolkit.decorators.collection_decorator import CollectionDecorator
 from forestadmin.datasource_toolkit.exceptions import DatasourceToolkitException
 from forestadmin.datasource_toolkit.interfaces.fields import (
     is_column,
     is_many_to_many,
     is_many_to_one,
     is_one_to_many,
     is_one_to_one,
@@ -11,146 +13,140 @@
 from forestadmin.datasource_toolkit.interfaces.models.collections import BoundCollection, CollectionSchema, Datasource
 from forestadmin.datasource_toolkit.interfaces.query.aggregation import AggregateResult, Aggregation
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.base import ConditionTree
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.leaf import ConditionTreeLeaf
 from forestadmin.datasource_toolkit.interfaces.query.filter.paginated import PaginatedFilter
 from forestadmin.datasource_toolkit.interfaces.query.filter.unpaginated import Filter
 from forestadmin.datasource_toolkit.interfaces.query.projections import Projection
-from forestadmin.datasource_toolkit.interfaces.query.sort import PlainSortClause
 from forestadmin.datasource_toolkit.interfaces.records import RecordsDataAlias
 
 
 class RenameCollectionException(DatasourceToolkitException):
     pass
 
 
-class RenameMixin:
-
-    datasource: property
-    mark_schema_as_dirty: Callable[..., None]
-
+class RenameFieldCollectionDecorator(CollectionDecorator):
     def __init__(self, *args: Any, **kwargs: Any):
-        super(RenameMixin, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self._to_child_collection: Dict[str, str] = {}
         self._from_child_collection: Dict[str, str] = {}
 
     def rename_field(self, current_name: str, new_name: str):
         schema = self.schema
         if current_name not in schema["fields"]:
-            raise RenameCollectionException(f"No such field {current_name}")
+            raise RenameCollectionException(f"No such field '{current_name}'")
 
         initial_name = current_name
+        # Revert previous renaming (avoids conflicts and need to recurse on this.toSubCollection).
         if current_name in self._to_child_collection:
             child_name = self._to_child_collection[current_name]
             del self._to_child_collection[current_name]
             del self._from_child_collection[child_name]
             initial_name = child_name
 
+        # Do not update arrays if renaming is a no-op (ie: customer is cancelling a previous rename).
         if initial_name != new_name:
             self._from_child_collection[initial_name] = new_name
             self._to_child_collection[new_name] = initial_name
         self.mark_schema_as_dirty()
 
     async def _refine_filter(
-        self, filter: Union[Filter, PaginatedFilter, None]
+        self, caller: User, _filter: Union[Filter, PaginatedFilter, None]
     ) -> Union[Filter, PaginatedFilter, None]:
         def computed_fields(tree: ConditionTree) -> ConditionTree:
             if isinstance(tree, ConditionTreeLeaf):
                 tree.field = self._path_to_child_collection(tree.field)
             return tree
 
-        filter = await super()._refine_filter(filter)  # type: ignore
-        if filter and filter.condition_tree:
-            filter = filter.override({"condition_tree": filter.condition_tree.replace(computed_fields)})  # type: ignore
-        return filter
+        _filter = await super()._refine_filter(caller, _filter)  # type: ignore
+        if _filter and _filter.condition_tree:
+            _filter = _filter.override({"condition_tree": _filter.condition_tree.replace(computed_fields)})
+        if _filter and isinstance(_filter, PaginatedFilter) and _filter.sort:
+            new_sort = _filter.sort.replace_clauses(
+                lambda clause: [
+                    {
+                        "field": self._path_to_child_collection(clause["field"]),
+                        "ascending": clause["ascending"],
+                    }
+                ]
+            )
+            _filter = _filter.override({"sort": new_sort})
 
-    async def list(self, filter: PaginatedFilter, projection: Projection) -> List[RecordsDataAlias]:
+        return _filter
+
+    async def list(self, caller: User, _filter: PaginatedFilter, projection: Projection) -> List[RecordsDataAlias]:
         child_projection = projection.replace(lambda field_name: self._path_to_child_collection(field_name))
-        records: List[RecordsDataAlias] = await super(RenameMixin, self).list(filter, child_projection)  # type: ignore
+        records: List[RecordsDataAlias] = await super().list(caller, _filter, child_projection)  # type: ignore
         return [self._record_from_child_collection(record) for record in records]
 
-    async def create(self, data: List[RecordsDataAlias]) -> List[RecordsDataAlias]:
+    async def create(self, caller: User, data: List[RecordsDataAlias]) -> List[RecordsDataAlias]:
         records: List[RecordsDataAlias] = await super().create(  # type: ignore
-            [self._record_to_child_collection(d) for d in data]
+            caller, [self._record_to_child_collection(d) for d in data]
         )
         return [self._record_from_child_collection(record) for record in records]
 
-    async def update(self, filter: Optional[Filter], patch: RecordsDataAlias) -> None:
+    async def update(self, caller: User, _filter: Optional[Filter], patch: RecordsDataAlias) -> None:
         refined_patch = self._record_to_child_collection(patch)
-        return await super(RenameMixin, self).update(filter, refined_patch)  # type: ignore
+        return await super().update(caller, _filter, refined_patch)  # type: ignore
 
     async def aggregate(
-        self, filter: Optional[Filter], aggregation: Aggregation, limit: Optional[int] = None
+        self, caller: User, _filter: Optional[Filter], aggregation: Aggregation, limit: Optional[int] = None
     ) -> List[AggregateResult]:
         rows: List[AggregateResult] = await super().aggregate(  # type: ignore
-            filter, aggregation.replace_fields(lambda name: self._path_to_child_collection(name)), limit
+            caller, _filter, aggregation.replace_fields(lambda name: self._path_to_child_collection(name)), limit
         )
         return [AggregateResult(value=row["value"], group=self._build_group_aggregate(row)) for row in rows]
 
     def _build_group_aggregate(self, row: AggregateResult) -> Dict[str, Any]:
         group: Dict[str, Any] = {}
         for path, value in row["group"].items():
             group[self._path_from_child_collection(path)] = value
         return group
 
-    @property
-    def schema(self) -> CollectionSchema:
-        schema: CollectionSchema = super(RenameMixin, self).schema  # type: ignore
-
+    def _refine_schema(self, sub_schema: CollectionSchema) -> CollectionSchema:
         new_fields_schema = {}
         datasource = cast(Datasource[BoundCollection], self.datasource)
-        for old_field_name, field_schema in schema["fields"].items():
-            if is_many_to_many(field_schema):
+
+        for old_field_name, field_schema in sub_schema["fields"].items():
+            if is_many_to_one(field_schema):
                 field_schema["foreign_key"] = self._from_child_collection.get(
                     field_schema["foreign_key"], field_schema["foreign_key"]
                 )
             elif is_one_to_many(field_schema) or is_one_to_one(field_schema):
                 relation = datasource.get_collection(field_schema["foreign_collection"])
-                relation = cast("RenameMixin", relation)
                 field_schema["origin_key"] = relation._from_child_collection.get(
                     field_schema["origin_key"], field_schema["origin_key"]
                 )
             elif is_many_to_many(field_schema):
                 through = datasource.get_collection(field_schema["through_collection"])
-                through = cast("RenameMixin", through)
                 field_schema["foreign_key"] = through._from_child_collection.get(
                     field_schema["foreign_key"], field_schema["foreign_key"]
                 )
                 field_schema["origin_key"] = through._from_child_collection.get(
                     field_schema["origin_key"], field_schema["origin_key"]
                 )
 
             new_fields_schema[self._from_child_collection.get(old_field_name, old_field_name)] = field_schema
-        schema["fields"] = new_fields_schema
-        return schema
+        return {**sub_schema, "fields": new_fields_schema}
 
     def _path_from_child_collection(self, child_path: str) -> str:
         datasource = cast(Datasource[BoundCollection], self.datasource)
         field, related_field = child_path, None
         if ":" in child_path:
             field, *related_field = child_path.split(":")
         self_field = self._from_child_collection.get(field, field)
         if related_field:
             schema = self.schema["fields"][self_field]
             if is_many_to_many(schema) or is_one_to_many(schema) or is_one_to_one(schema) or is_many_to_one(schema):
                 relation = datasource.get_collection(schema["foreign_collection"])
-                relation = cast("RenameMixin", relation)
                 return f"{self_field}:{relation._path_from_child_collection(':'.join(related_field))}"
             else:
                 raise RenameCollectionException(f"The field {self_field} is not a relation")
         return self_field
 
-    def _refine_leaf_tree(self, tree: ConditionTree) -> ConditionTree:
-        if isinstance(tree, ConditionTreeLeaf):
-            tree.field = self._path_to_child_collection(tree.field)
-        return tree
-
-    def _refine_sort_clause(self, clause: PlainSortClause):
-        return PlainSortClause(field=self._path_to_child_collection(clause["field"]), ascending=clause["ascending"])
-
     def _record_to_child_collection(self, record: RecordsDataAlias) -> RecordsDataAlias:
         child_record: RecordsDataAlias = {}
         for field_name, value in record.items():
             child_record[self._to_child_collection.get(field_name, field_name)] = value
         return child_record
 
     def _record_from_child_collection(self, record: RecordsDataAlias) -> RecordsDataAlias:
@@ -160,27 +156,25 @@
             new_field_name = self._from_child_collection.get(field_name, field_name)
             new_field_name, *_ = new_field_name.split(":")
             schema = self.schema["fields"][new_field_name]
             if is_column(schema) or value is None:
                 new_record[new_field_name] = value
             elif is_many_to_many(schema) or is_many_to_one(schema) or is_one_to_many(schema) or is_one_to_one(schema):
                 relation = datasource.get_collection(schema["foreign_collection"])
-                relation = cast("RenameMixin", relation)
                 new_record[new_field_name] = relation._record_from_child_collection(value)
         return new_record
 
     def _path_to_child_collection(self, path: str) -> str:
         datasource = cast(Datasource[BoundCollection], self.datasource)
         field_name, related_field = path, None
         if ":" in path:
             field_name, *related_field = path.split(":")
             related_field = ":".join(related_field)
         if related_field:
             schema = self.schema["fields"][field_name]
             if is_many_to_many(schema) or is_one_to_many(schema) or is_one_to_one(schema) or is_many_to_one(schema):
                 relation = datasource.get_collection(schema["foreign_collection"])
-                relation = cast("RenameMixin", relation)
                 child_field = self._to_child_collection.get(field_name, field_name)
                 return f"{child_field}:{relation._path_to_child_collection(related_field)}"
             else:
                 raise RenameCollectionException(f"The field {field_name} is not a relation")
         return self._to_child_collection.get(field_name, field_name)
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/search/collections.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/search/collections.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,122 +1,133 @@
-from typing import Dict, List, Optional, Tuple, Union, cast
+from typing import Any, Awaitable, Callable, List, Optional, Tuple, Union
 
+from forestadmin.agent_toolkit.utils.context import User
+from forestadmin.datasource_toolkit.context.collection_context import CollectionCustomizationContext
+from forestadmin.datasource_toolkit.decorators.collection_decorator import CollectionDecorator
+from forestadmin.datasource_toolkit.interfaces.collections import Collection
 from forestadmin.datasource_toolkit.interfaces.fields import (
     Column,
     ColumnAlias,
-    FieldAlias,
     Operator,
     PrimitiveType,
     is_column,
     is_many_to_one,
     is_one_to_one,
+    is_valid_uuid,
 )
 from forestadmin.datasource_toolkit.interfaces.models.collections import BoundCollection, CollectionSchema, Datasource
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.factory import ConditionTreeFactory
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.base import ConditionTree
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.leaf import ConditionTreeLeaf
 from forestadmin.datasource_toolkit.interfaces.query.filter.paginated import PaginatedFilter
 from forestadmin.datasource_toolkit.interfaces.query.filter.unpaginated import Filter
-from forestadmin.datasource_toolkit.validations.type_getter import TypeGetter
-from typing_extensions import TypeGuard
 
+SearchDefinition = Callable[[Any, bool, CollectionCustomizationContext], ConditionTree]
 
-class SearchMixin:  # type: ignore
 
-    datasource: property
+class SearchCollectionDecorator(CollectionDecorator):
+    def __init__(self, collection: Collection, datasource: Datasource[BoundCollection]):
+        super().__init__(collection, datasource)
+        self._replacer: SearchDefinition = None
 
-    TYPE_TO_OPERATOR: Dict[ColumnAlias, Operator] = {
-        PrimitiveType.STRING: Operator.CONTAINS,
-        PrimitiveType.ENUM: Operator.EQUAL,
-        PrimitiveType.NUMBER: Operator.EQUAL,
-        PrimitiveType.UUID: Operator.EQUAL,
-    }
-
-    @property
-    def schema(self) -> CollectionSchema:
-        schema: CollectionSchema = super(SearchMixin, self).schema  # type: ignore
-        schema["searchable"] = True
-        return schema
+    def replace_search(self, replacer: SearchDefinition):
+        self._replacer = replacer
 
-    async def _refine_filter(
-        self, filter: Union[Optional[PaginatedFilter], Optional[Filter]]
-    ) -> Optional[Union[PaginatedFilter, Filter]]:
-        filter = cast(PaginatedFilter, await super()._refine_filter(filter))  # type: ignore
-        if not filter or not filter.search:
-            return filter
-
-        if self._is_empty_string(filter.search):
-            return filter.override({"search": None})
+    def _refine_schema(self, sub_schema: CollectionSchema) -> CollectionSchema:
+        return {**sub_schema, "searchable": True}
 
-        searchable_fields = self._get_searchable_fields(self.schema, filter.search_extended or False)
+    def _default_replacer(self, search: str, extended: bool) -> ConditionTree:
+        searchable_fields = self._get_searchable_fields(self.child_collection, extended)
+        conditions = [self._build_condition(name, field, search) for (name, field) in searchable_fields]
 
-        conditions: List[ConditionTree] = []
-        for field, schema in searchable_fields:
-            try:
-                condition = self._build_condition(field, schema, filter.search)
-            except ValueError:
-                condition = None
-            if condition:
-                conditions.append(condition)
-        trees: List[ConditionTree] = []
-        if conditions:
-            trees.append(ConditionTreeFactory.union(conditions))
-        if filter.condition_tree:
-            trees.append(filter.condition_tree)
-
-        if trees:
-            return filter.override({"condition_tree": ConditionTreeFactory.intersect(trees), "search": None})
-
-        raise Exception("filter search type not matching any fields's type")
-
-    def _build_condition(self, field: str, schema: Column, search: str) -> Optional[ConditionTree]:
-        condition: Optional[ConditionTree] = None
-        type_ = cast(PrimitiveType, schema["column_type"])
-        enum_values = schema["enum_values"] or []
-        value: Union[int, float, str] = search
+        return ConditionTreeFactory.union(conditions)
 
-        if schema["column_type"] == PrimitiveType.NUMBER:
+    async def _refine_filter(
+        self, caller: User, _filter: Union[Optional[PaginatedFilter], Optional[Filter]]
+    ) -> Optional[Union[PaginatedFilter, Filter]]:
+        # Search string is not significant
+        if _filter.search is None or _filter.search.strip() == "":
+            return _filter.override({"search": None})
+
+        # Implement search ourselves
+        if self._replacer or not self.child_collection.schema["searchable"]:
+            context = CollectionCustomizationContext(self, caller)
+            tree = self._default_replacer(_filter.search, _filter)
+
+            if self._replacer is not None:
+                tree = self._replacer(_filter.search, _filter.search_extended, context)
+                if isinstance(tree, Awaitable):
+                    tree = await tree
+
+                if isinstance(tree, dict):
+                    tree = ConditionTreeFactory.from_plain_object(tree)
+
+            # Note that if no fields are searchable with the provided searchString, the conditions
+            # array might be empty, which will create a condition returning zero records
+            # (this is the desired behavior).
+            return _filter.override(
+                {"condition_tree": ConditionTreeFactory.intersect([_filter.condition_tree, tree]), "search": None}
+            )
+
+        # Let sub collection deal with the search
+        return _filter
+
+    def _build_condition(self, field: str, schema: Column, search: str) -> Union[ConditionTree, None]:
+        if (
+            schema["column_type"] == PrimitiveType.NUMBER
+            and search.isnumeric()
+            and Operator.EQUAL in schema.get("filter_operators", [])
+        ):
             try:
                 value = int(search)
             except ValueError:
                 value = float(search)
+            return ConditionTreeLeaf(field, Operator.EQUAL, value)
 
-        search_type = TypeGetter.get(value, type_)
-
-        if self._is_valid_enum(enum_values, search, type_) or search_type in [PrimitiveType.NUMBER, PrimitiveType.UUID]:
-            condition = ConditionTreeLeaf(field, Operator.EQUAL, value)
-        elif search_type == PrimitiveType.STRING:
-            condition = ConditionTreeLeaf(field, Operator.CONTAINS, value)
-
-        return condition
-
-    def _is_valid_enum(self, enum_values: List[str], search: str, search_type: PrimitiveType) -> bool:
-        values = [enum_value.lower() for enum_value in enum_values]
-        search = search.lower().strip()
-        return search_type == PrimitiveType.ENUM and search in values
-
-    def _get_searchable_fields(self, schema: CollectionSchema, search_extended: bool) -> List[Tuple[str, Column]]:
-        fields = list(schema["fields"].items())
-        if search_extended:
-            fields.extend(self._get_deep_fields(fields))
-        return [(field_name, schema) for field_name, schema in fields if self._is_searchable(schema)]
-
-    def _is_searchable(self, schema: FieldAlias) -> TypeGuard[Column]:
-        filter_operators = schema.get("filter_operators") or set()
-        if is_column(schema):
-            try:
-                return self.TYPE_TO_OPERATOR[schema["column_type"]] in filter_operators
-            except KeyError:
-                return False
-        return False
-
-    def _get_deep_fields(self, fields: List[Tuple[str, FieldAlias]]):
-        deep_fields: List[Tuple[str, FieldAlias]] = []
-        for name, field in fields:
-            if is_many_to_one(field) or is_one_to_one(field):
-                related = cast(Datasource[BoundCollection], self.datasource).get_collection(field["foreign_collection"])
-                for deep_name, deep_schema in related.schema["fields"].items():
-                    deep_fields.append((f"{name}:{deep_name}", deep_schema))
-        return deep_fields
-
-    def _is_empty_string(self, search: str) -> bool:
-        return len(search.strip()) == 0
+        if schema["column_type"] == PrimitiveType.ENUM and Operator.EQUAL in schema.get("filter_operators", []):
+            search_value = self.lenient_find(schema["enum_values"], search)
+            if search_value is not None:
+                return ConditionTreeLeaf(field, Operator.EQUAL, search_value)
+
+        if schema["column_type"] == PrimitiveType.STRING:
+            support_icontains = False  # Operator.ICONTAINS in schema.get("filter_operators",[])
+            support_contains = Operator.CONTAINS in schema.get("filter_operators", [])
+            support_equal = Operator.EQUAL in schema.get("filter_operators", [])
+            if support_icontains and not support_contains:
+                pass  # operator = Operator.ICONTAINS
+            elif support_contains:
+                operator = Operator.CONTAINS
+            elif support_equal:
+                operator = Operator.EQUAL
+            else:
+                operator = None
+
+            if operator:
+                return ConditionTreeLeaf(field, operator, search)
+
+        if (
+            schema["column_type"] == PrimitiveType.UUID
+            and is_valid_uuid(search)
+            and Operator.EQUAL in schema.get("filter_operators", [])
+        ):
+            return ConditionTreeLeaf(field, Operator.EQUAL, search)
+
+    def lenient_find(self, haystack: List[str], needle: str) -> Union[str, None]:
+        for item in haystack:
+            if needle.strip() == item or needle.strip().lower() == item.lower():
+                return item
+        return None
+
+    def _get_searchable_fields(self, collection: Collection, extended: bool) -> List[Tuple[str, ColumnAlias]]:
+        fields: List[Tuple[str, ColumnAlias]] = []
+
+        for name, field in collection.schema["fields"].items():
+            if is_column(field):
+                fields.append((name, field))
+
+            if extended and (is_many_to_one(field) or is_one_to_one(field)):
+                related = collection.datasource.get_collection(field["foreign_collection"])
+
+                for sub_name, sub_field in related.schema["fields"].items():
+                    if is_column(sub_field):
+                        fields.append((f"{name}:{sub_name}", sub_field))
+        return fields
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/segments/collections.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/decorators/segments/collections.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 from typing import Any, Awaitable, Callable, Dict, Optional, Union, cast
 
+from forestadmin.agent_toolkit.utils.context import User
 from forestadmin.datasource_toolkit.context.collection_context import CollectionCustomizationContext
+from forestadmin.datasource_toolkit.decorators.collection_decorator import CollectionDecorator
 from forestadmin.datasource_toolkit.interfaces.collections import Collection
 from forestadmin.datasource_toolkit.interfaces.models.collections import CollectionSchema
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.factory import ConditionTreeFactory
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.base import ConditionTree
 from forestadmin.datasource_toolkit.interfaces.query.filter.paginated import PaginatedFilter
 from forestadmin.datasource_toolkit.interfaces.query.filter.unpaginated import Filter
 
 SegmentAlias = Callable[[CollectionCustomizationContext], Union[ConditionTree, Awaitable[ConditionTree]]]
 
 
-class SegmentMixin:
-    mark_schema_as_dirty: Callable[[], None]
-
+class SegmentCollectionDecorator(CollectionDecorator):
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self._segments: Dict[str, SegmentAlias] = {}
 
     def add_segment(self, name: str, segment: SegmentAlias):
         self._segments[name] = segment
         self.mark_schema_as_dirty()
 
-    @property
-    def schema(self) -> CollectionSchema:
-        schema: CollectionSchema = super(SegmentMixin, self).schema  # type: ignore
-        schema["segments"] = [*schema["segments"], *self._segments.keys()]
-        return schema
+    def _refine_schema(self, sub_schema: CollectionSchema) -> CollectionSchema:
+        return {**sub_schema, "segments": [*self._segments.keys()]}
 
     async def _refine_filter(
-        self, filter: Union[Optional[PaginatedFilter], Optional[Filter]]
+        self, caller: User, _filter: Union[Optional[PaginatedFilter], Optional[Filter]]
     ) -> Optional[Union[PaginatedFilter, Filter]]:
-        filter = cast(SegmentMixin, await super()._refine_filter(filter))  # type: ignore
-        if not filter:
+        _filter = await super()._refine_filter(caller, _filter)  # type: ignore
+        if not _filter:
             return None
 
-        if filter.segment and filter.segment in self._segments:
-            definition = self._segments[filter.segment]
-            context = CollectionCustomizationContext(cast(Collection, self), filter.timezone)
+        if _filter.segment and _filter.segment in self._segments:
+            definition = self._segments[_filter.segment]
+            context = CollectionCustomizationContext(cast(Collection, self), caller)
             condition_tree_segment = definition(context)
             if isinstance(condition_tree_segment, Awaitable):
                 condition_tree_segment = await condition_tree_segment
 
+            if isinstance(condition_tree_segment, dict):
+                condition_tree_segment = ConditionTreeFactory.from_plain_object(condition_tree_segment)
+
             trees = [condition_tree_segment]
-            if filter.condition_tree:
-                trees.append(filter.condition_tree)
+            if _filter.condition_tree:
+                trees.append(_filter.condition_tree)
             condition_tree = ConditionTreeFactory.intersect(trees)
-            filter = filter.override({"condition_tree": condition_tree, "segment": None})
-        return filter
+            _filter = _filter.override({"condition_tree": condition_tree, "segment": None})
+        return _filter
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/.DS_Store` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/actions.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/actions.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     format: Union[Literal["html"], Literal["text"]]
     invalidated: Set[str]
 
 
 class ErrorResult(TypedDict):
     type: Literal["Error"]
     message: str
+    format: Union[Literal["html"], Literal["text"]]
 
 
 class WebHookResult(TypedDict):
     type: Literal["Webhook"]
     url: str
     method: Union[Literal["GET"], Literal["POST"]]
     headers: Dict[str, str]
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/fields.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import enum
 import sys
+from uuid import UUID
 
 if sys.version_info >= (3, 8):
     from typing import Literal, TypedDict
 else:
     from typing_extensions import Literal, TypedDict
 
 from typing import Any, Dict, List, Optional, Set, Union
@@ -21,14 +22,15 @@
     GREATER_THAN = "greater_than"
     IN = "in"
     NOT_IN = "not_in"
     LIKE = "like"
     STARTS_WITH = "starts_with"
     ENDS_WITH = "ends_with"
     CONTAINS = "contains"
+    # ICONTAINS = "icontains"
     NOT_CONTAINS = "not_contains"
     LONGER_THAN = "longer_than"
     SHORTER_THAN = "shorter_than"
     BEFORE = "before"
     AFTER = "after"
     AFTER_X_HOURS_AGO = "after_x_hours_ago"
     BEFORE_X_HOURS_AGO = "before_x_hours_ago"
@@ -187,7 +189,15 @@
 
 def is_many_to_many(field: "FieldAlias") -> TypeGuard[ManyToMany]:
     return field["type"] == FieldType.MANY_TO_MANY
 
 
 def is_relation(field: "FieldAlias") -> TypeGuard[RelationAlias]:
     return is_many_to_one(field) or is_one_to_many(field) or is_one_to_one(field) or is_many_to_many(field)
+
+
+def is_valid_uuid(uuid: str) -> bool:
+    try:
+        UUID(uuid)
+        return True
+    except ValueError:
+        return False
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/models/collections.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/models/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 
 class CollectionSchema(TypedDict):
     actions: Dict[str, Action]
     fields: Dict[str, FieldAlias]
     searchable: bool
     segments: List[str]
+    countable: bool
 
 
 class Collection(abc.ABC):
     @abc.abstractproperty
     def datasource(self) -> "Datasource[Self]":
         raise NotImplementedError
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/.DS_Store` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/aggregation.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/aggregation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import enum
 import json
 import sys
+from numbers import Number
 
 if sys.version_info >= (3, 8):
     from typing import Literal, TypedDict
 else:
     from typing_extensions import Literal, TypedDict
 if sys.version_info >= (3, 9):
     import zoneinfo
@@ -172,22 +173,21 @@
             "Max": None,
         }
 
     def _update_summary_in_place(self, summary: Summary, record: RecordsDataAlias) -> Summary:
         summary["start_count"] += 1  #  count(*)
         if self.field:
             value = RecordUtils.get_field_value(record, self.field)
-            is_number = isinstance(value, int)
             if value is not None:
                 summary["Count"] += 1  #  count(field)
-                if is_number and (summary["Min"] is None or value < summary["Min"]):
+                if summary["Min"] is None or value < summary["Min"]:
                     summary["Min"] = value
-                if is_number and (summary["Max"] is None or value > summary["Max"]):
+                if summary["Max"] is None or value > summary["Max"]:
                     summary["Max"] = value
-            if is_number:
+            if isinstance(value, Number):
                 summary["Sum"] += value
         return summary
 
     def _create_group(self, record: RecordsDataAlias, timezone: str) -> RecordsDataAlias:
         group_record: RecordsDataAlias = {}
         for group in self.groups:
             group_value = RecordUtils.get_field_value(record, group["field"])
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     @classmethod
     def _get_replacer(
         cls,
         operator: Operator,
         allowed_operators: Set[Operator],
         column_type: ColumnAlias,
-        visited: Optional[List[Alternative]] = [],
+        visited: Optional[List[Alternative]] = None,
     ) -> Optional[Replacer]:
         if not visited:
             visited = []
 
         if operator in allowed_operators:
             return lambda leaf, tz: leaf
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,16 @@
             return branch.conditions[0]
         return branch
 
     @staticmethod
     def _group(aggregator: Aggregator, trees: List[ConditionTree]) -> ConditionTree:
         conditions: List[ConditionTree] = []
         for tree in trees:
+            if tree is None:
+                continue
             if isinstance(tree, ConditionTreeBranch) and tree.aggregator == aggregator:
                 conditions.extend(tree.conditions)
             else:
                 conditions.append(tree)
 
         if len(conditions) == 1:
             return conditions[0]
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 def _not_equal_to_not_in(leaf: ConditionTreeLeaf, _: zoneinfo.ZoneInfo) -> ConditionTree:
     return leaf.override({"operator": Operator.NOT_IN, "value": [leaf.value]})
 
 
 def _not_in_to_not_equal(leaf: ConditionTreeLeaf, _: zoneinfo.ZoneInfo) -> ConditionTree:
     values = cast(List[Any], leaf.value)
-    return ConditionTreeFactory.union(
+    return ConditionTreeFactory.intersect(
         [leaf.override({"operator": Operator.NOT_EQUAL, "value": item}) for item in values]
     )
 
 
 def equality_transforms() -> Dict[Operator, List[Alternative]]:
     return {
         Operator.BLANK: [
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,14 @@
             }
         )
 
     return replacer
 
 
 def _build_interval(end: datetime, frequency: str, periods: int, tz: zoneinfo.ZoneInfo) -> Interval:
-
     dates: List[datetime] = []
     end = end.astimezone(zoneinfo.ZoneInfo("UTC"))  # mandatory to avoid the panda issue with zoneinfo
     for dt in pd.date_range(end=end, periods=periods, freq=frequency).to_pydatetime():  # type: ignore
         dt = cast(datetime, dt)
         if frequency != Frequency.HOUR.value:
             dt = _start_of(dt, True).replace(tzinfo=tz)
         else:
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import sys
 
+from forestadmin.agent_toolkit.utils.context import User
+
 if sys.version_info >= (3, 9):
     import zoneinfo
 else:
     from backports import zoneinfo
 
 from typing import List, Union, cast
 
@@ -78,34 +80,36 @@
                 ]
             )
         return base_through_filter.override({"condition_tree": condition_tree})
 
     @classmethod
     async def make_through_filter(
         cls,
+        caller: User,
         collection: Collection,
         id: CompositeIdAlias,
         relation: ManyToMany,
         _base_foreign_key_filter: Union[PaginatedFilter, Filter],
     ) -> PaginatedFilter:
         if is_filter(_base_foreign_key_filter):
             base_foreign_key_filter: PaginatedFilter = PaginatedFilter.from_base_filter(_base_foreign_key_filter)
         else:
             base_foreign_key_filter = cast(PaginatedFilter, _base_foreign_key_filter)
-        origin_value = await CollectionUtils.get_value(collection, id, relation["origin_key_target"])
+        origin_value = await CollectionUtils.get_value(caller, collection, id, relation["origin_key_target"])
         if relation["foreign_relation"] and base_foreign_key_filter.is_nestable:
             return cls._build_for_through_relation(
                 base_foreign_key_filter,
                 relation["origin_key"],
                 relation["foreign_relation"],
                 origin_value,
             )
         target = collection.datasource.get_collection(relation["foreign_collection"])
         records = await target.list(
-            await cls.make_foreign_filter(collection, id, relation, base_foreign_key_filter),
+            caller,
+            await cls.make_foreign_filter(caller, collection, id, relation, base_foreign_key_filter),
             Projection(relation["foreign_key_target"]),
         )
 
         return PaginatedFilter(
             {
                 "condition_tree": ConditionTreeFactory.intersect(
                     [
@@ -118,33 +122,35 @@
                     ]
                 )
             }
         )
 
     @staticmethod
     async def make_foreign_filter(
+        caller: User,
         collection: Collection,
         id: CompositeIdAlias,
         relation: Union[ManyToMany, OneToMany],
         _base_foreign_key_filter: Union[PaginatedFilter, Filter],
     ) -> PaginatedFilter:
         if is_filter(_base_foreign_key_filter):
             base_foreign_key_filter: PaginatedFilter = PaginatedFilter.from_base_filter(_base_foreign_key_filter)
         else:
             base_foreign_key_filter = cast(PaginatedFilter, _base_foreign_key_filter)
-        origin_value = await CollectionUtils.get_value(collection, id, relation["origin_key_target"])
+        origin_value = await CollectionUtils.get_value(caller, collection, id, relation["origin_key_target"])
 
         origin_tree: ConditionTree
 
         if relation["type"] == FieldType.ONE_TO_MANY:
             origin_tree = ConditionTreeLeaf(relation["origin_key"], Operator.EQUAL, origin_value)
         else:
             through = collection.datasource.get_collection(relation["through_collection"])
             through_tree = ConditionTreeLeaf(relation["origin_key"], Operator.EQUAL, origin_value)
             records = await through.list(
+                caller,
                 PaginatedFilter({"condition_tree": through_tree}),
                 Projection(relation["foreign_key"]),
             )
             origin_tree = ConditionTreeLeaf(
                 relation["foreign_key_target"],
                 Operator.IN,
                 [record[relation["foreign_key"]] for record in records],
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/page.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/page.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import Counter
 from functools import reduce
 from typing import Any, Callable, DefaultDict, Dict, List, Optional, Union, cast
 
 from forestadmin.datasource_toolkit.exceptions import DatasourceToolkitException
 from forestadmin.datasource_toolkit.interfaces.fields import RelationAlias
 from forestadmin.datasource_toolkit.interfaces.models.collections import Collection
 from forestadmin.datasource_toolkit.interfaces.records import RecordsDataAlias
@@ -30,28 +31,27 @@
             if len(splited) > 1:
                 relation = splited[1:]
                 relations[field] = Projection(*relations[field], ":".join(relation))
         return relations
 
     def replace(self, handler: Callable[[str], Union["Projection", str, List[str]]]) -> "Projection":
         def reducer(memo: Projection, paths: Union["Projection", str, List[str]]) -> Projection:
-
             if isinstance(paths, str):
                 new_paths = [paths]
             else:
                 new_paths: Union[List[str], "Projection"] = paths
             return memo.union(new_paths)
 
         handled = map(handler, self)
 
         return reduce(reducer, handled, Projection())
 
     def union(self, *projections: Union["Projection", List[str]]) -> "Projection":
         fields: List[str] = reduce(lambda x, y: [*x, *y], [self, *projections], [])  # type: ignore
-        return Projection(*sorted(set(fields)))
+        return Projection(*Counter(fields))
 
     def apply(self, records: List[RecordsDataAlias]) -> List[RecordsDataAlias]:
         results: List[RecordsDataAlias] = []
         for record in records:
             result = self._reproject(record)
             if result:
                 results.append(result)
@@ -74,16 +74,16 @@
 
     def nest(self, prefix: str) -> "Projection":
         if prefix:
             return Projection(*map(lambda path: f"{prefix}:{path}", self))  # type: ignore
         return self
 
     def unnest(self) -> "Projection":
-        splited = self[0].split(":")  # type: ignore
-        prefix = splited[0]  # type: ignore
+        splitted = self[0].split(":")  # type: ignore
+        prefix = splitted[0]  # type: ignore
         if not all([path.startswith(prefix) for path in self]):  # type: ignore
             raise ProjectionException("Cannot unnest projection.")
 
         return Projection(*map(lambda path: path[len(prefix) + 1 :], self))  # type: ignore
 
     def _reproject(self, record: Optional[RecordsDataAlias] = None) -> Optional[RecordsDataAlias]:
         result: Optional[RecordsDataAlias] = None
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
         res: List[str] = []
         for column_name, schema in collection.schema["fields"].items():
             if is_column(schema):
                 res.append(f"{prefix}{column_name}")
             elif allow_nested and (is_one_to_one(schema) or is_many_to_one(schema)):
                 relation = collection.datasource.get_collection(schema["foreign_collection"])
                 res.extend(cls.all(relation, f"{column_name}:", False))
-        return Projection(res)
+        return Projection(*res)
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Union
 
-from forestadmin.datasource_toolkit.decorators.collections import CustomizedCollection
+from forestadmin.datasource_toolkit.datasource_customizer.collection_customizer import CollectionCustomizer
 from forestadmin.datasource_toolkit.interfaces.models.collections import Collection
 from forestadmin.datasource_toolkit.interfaces.query.sort import Sort
 from forestadmin.datasource_toolkit.utils.schema import SchemaUtils
 
 
 class SortFactory:
     @staticmethod
-    def by_primary_keys(collection: Union[CustomizedCollection, Collection]) -> Sort:
+    def by_primary_keys(collection: Union[CollectionCustomizer, Collection]) -> Sort:
         return Sort([{"field": pk, "ascending": True} for pk in SchemaUtils.get_primary_keys(collection.schema)])
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/utils/collections.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/utils/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import List, Optional, Union, cast
 
+from forestadmin.agent_toolkit.utils.context import User
 from forestadmin.datasource_toolkit.collections import Collection
 from forestadmin.datasource_toolkit.exceptions import DatasourceToolkitException
 from forestadmin.datasource_toolkit.interfaces.fields import (
     FieldAlias,
     ManyToMany,
     OneToMany,
     RelationAlias,
@@ -49,52 +50,58 @@
         if not (is_many_to_one(schema) or is_one_to_one(schema)):
             raise CollectionUtilsException(f'Unexpected field type {schema["type"]}: {collection.name}.{field_name}')
 
         schema = cast(RelationAlias, schema)
         return cls.get_field_schema(collection.datasource.get_collection(schema["foreign_collection"]), sub_path)
 
     @staticmethod
-    async def get_value(collection: Collection, id: CompositeIdAlias, field: str) -> Union[int, str]:
+    async def get_value(caller: User, collection: Collection, id: CompositeIdAlias, field: str) -> Union[int, str]:
         try:
             index = SchemaUtils.get_primary_keys(collection.schema).index(field)
         except ValueError:
             records = await collection.list(
+                caller,
                 PaginatedFilter({"condition_tree": ConditionTreeFactory.match_ids(collection.schema, [id])}),
                 Projection(field),
             )
             res = records[0]["field"]
         else:
             res = id[index]
 
         return res
 
     @staticmethod
     async def list_relation(
+        caller: User,
         collection: Collection,
         id: CompositeIdAlias,
         foreign_collection: Collection,
         relation: Union[ManyToMany, OneToMany],
         foreign_filter: PaginatedFilter,
         projection: Projection,
     ) -> List[RecordsDataAlias]:
         from forestadmin.datasource_toolkit.interfaces.query.filter.factory import FilterFactory
 
         if is_many_to_many(relation) and relation["foreign_relation"] and foreign_filter.is_nestable:
             through = collection.datasource.get_collection(relation["through_collection"])
             records = await through.list(
+                caller,
                 await FilterFactory.make_through_filter(collection, id, relation, foreign_filter),
                 projection.nest(relation["foreign_relation"]),
             )
             return [record[relation["foreign_relation"]] for record in records]
         return await foreign_collection.list(
-            await FilterFactory.make_foreign_filter(collection, id, relation, foreign_filter), projection
+            caller,
+            await FilterFactory.make_foreign_filter(caller, collection, id, relation, foreign_filter),
+            projection,
         )
 
     @staticmethod
     async def aggregate_relation(
+        caller: User,
         collection: Collection,
         id: CompositeIdAlias,
         relation_name: str,
         foreign_filter: Filter,
         aggregation: Aggregation,
         limit: Optional[int] = None,
     ):
@@ -104,28 +111,28 @@
         foreign_collection = collection.datasource.get_collection(relation["foreign_collection"])
 
         if is_many_to_many(relation) and relation["foreign_relation"] and foreign_filter.is_nestable:
             through = collection.datasource.get_collection(relation["through_collection"])
             filter = await FilterFactory.make_through_filter(collection, id, relation, foreign_filter)
 
             nested_records = await through.aggregate(
-                filter.to_base_filter(), aggregation.nest(relation["foreign_relation"]), limit
+                caller, filter.to_base_filter(), aggregation.nest(relation["foreign_relation"]), limit
             )
 
             records: List[AggregateResult] = []
             for record in nested_records:
                 group = {}
                 for key, value in record["group"].items():
                     group[key.split(":")[1:]] = value
                 records.append({"value": record["value"], "group": record["group"]})
             return records
 
         relation = cast(OneToMany, relation)
-        filter = await FilterFactory.make_foreign_filter(collection, id, relation, foreign_filter)
-        return await foreign_collection.aggregate(filter.to_base_filter(), aggregation, limit)
+        filter = await FilterFactory.make_foreign_filter(caller, collection, id, relation, foreign_filter)
+        return await foreign_collection.aggregate(caller, filter.to_base_filter(), aggregation, limit)
 
     @staticmethod
     def get_inverse_relation(collection: Collection, relation_name: str) -> Optional[str]:
         relation = cast(RelationAlias, collection.get_field(relation_name))
         foreign_collection = collection.datasource.get_collection(relation["foreign_collection"])
         inverse: Optional[str] = None
         for name, field_schema in foreign_collection.schema["fields"].items():
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/utils/records.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/utils/records.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,9 +24,9 @@
         return results
 
     @staticmethod
     def get_field_value(record: RecordsDataAlias, field: str) -> Any:
         current_record = record
         for path in field.split(":"):
             if current_record:
-                current_record = current_record[path]
+                current_record = current_record.get(path)
         return current_record
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/utils/schema.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/utils/schema.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/condition_tree.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/condition_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Union, cast
 
-from forestadmin.datasource_toolkit.decorators.collections import CustomizedCollection
+from forestadmin.datasource_toolkit.datasource_customizer.collection_customizer import CollectionCustomizer
 from forestadmin.datasource_toolkit.exceptions import DatasourceToolkitException
 from forestadmin.datasource_toolkit.interfaces.fields import Column, PrimitiveType, is_column
 from forestadmin.datasource_toolkit.interfaces.models.collections import Collection
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.base import ConditionTree
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.leaf import ConditionTreeLeaf
 from forestadmin.datasource_toolkit.utils.collections import CollectionUtils
 from forestadmin.datasource_toolkit.validations.field import FieldValidator
@@ -18,30 +18,30 @@
 
 class ConditionTreeValidatorException(DatasourceToolkitException):
     pass
 
 
 class ConditionTreeValidator:
     @classmethod
-    def _validate_leaf_condition(cls, collection: Union[Collection, CustomizedCollection]):
+    def _validate_leaf_condition(cls, collection: Union[Collection, CollectionCustomizer]):
         def validate_condition_tree(condition: ConditionTree):
             condition = cast(ConditionTreeLeaf, condition)
             schema = CollectionUtils.get_field_schema(collection, condition.field)
             if is_column(schema):
                 cls.validate_operator(condition, schema)
                 cls.validate_value_for_operator(condition, schema)
                 cls.validate_operator_for_column_type(condition, schema)
                 cls.validate_value_for_column_type(condition, schema)
             else:
                 raise ConditionTreeValidatorException("Unable to apply condition on relation field")
 
         return validate_condition_tree
 
     @classmethod
-    def validate(cls, condition_tree: ConditionTree, collection: Union[Collection, CustomizedCollection]):
+    def validate(cls, condition_tree: ConditionTree, collection: Union[Collection, CollectionCustomizer]):
         condition_tree.apply(cls._validate_leaf_condition(collection))
 
     @staticmethod
     def validate_operator(condition_tree: ConditionTreeLeaf, column_schema: Column):
         operators = column_schema["filter_operators"]
         error_msg = f"The given operator {condition_tree.operator} is not supported by the column:"
         if not operators:
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/field.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/field.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/records.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/records.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/rules.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/rules.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/type_getter.py` & `forestadmin_datasource_toolkit-1.0.0b1/forestadmin/datasource_toolkit/validations/type_getter.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 class TypeGetterException(DatasourceToolkitException):
     pass
 
 
 class TypeGetter:
     @classmethod
     def get(cls, value: Any, type_context: Optional[PrimitiveType]) -> Union[PrimitiveType, ValidationType]:
-
         if isinstance(value, list):
             value = cast(List[Any], value)
             return cls._get_array_type(value, type_context)
         elif isinstance(value, str):
             return cls._get_type_from_string(value, type_context)
         elif isinstance(value, float) or isinstance(value, int):
             return PrimitiveType.NUMBER
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/pyproject.toml` & `forestadmin_datasource_toolkit-1.0.0b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-datasource-toolkit"
-version = "0.1.0-beta.9"
+version = "1.0.0-beta.1"
 description = ""
 authors = [ "Valentin Monté <valentinm@forestadmin.com>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.semantic_release]
@@ -19,23 +19,23 @@
 build_command = "pip install poetry && poetry build"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 typing-extensions = "~=4.2"
 tzdata = "~=2022.6"
 [[tool.poetry.dependencies.pandas]]
-version = "==1.1.5"
+version = "<=1.1.5"
 python = "<3.7.1"
 
 [[tool.poetry.dependencies.pandas]]
-version = "==1.3.5"
+version = ">=1.3.4,<=1.3.5"
 python = ">=3.7.1,<3.8"
 
 [[tool.poetry.dependencies.pandas]]
-version = "~=1.4.2"
+version = ">=1.4.0"
 python = ">=3.8"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
 version = "~=0.2.1"
 python = "<3.9"
 extras = [ "tzdata",]
 
@@ -52,14 +52,15 @@
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "~=7.1"
 pytest-asyncio = "~=0.18"
 coverage = "~=6.5"
 freezegun = "~=1.2.0"
+pytest-cov = "^4.0.0"
 [[tool.poetry.group.test.dependencies.mock]]
 version = "4.0"
 python = "3.7"
 
 [tool.poetry.group.linter.dependencies]
 [[tool.poetry.group.linter.dependencies.flake8]]
 version = "~=5.0"
@@ -70,7 +71,11 @@
 python = ">=3.8.1"
 
 [tool.poetry.group.formatter.dependencies]
 black = "~=22.10"
 
 [tool.poetry.group.sorter.dependencies]
 isort = "~=3.6"
+
+[tool.poetry.group.test.dependencies.forestadmin-agent-toolkit]
+path = "../agent_toolkit"
+develop = true
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b9/PKG-INFO` & `forestadmin_datasource_toolkit-1.0.0b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: forestadmin-datasource-toolkit
-Version: 0.1.0b9
+Version: 1.0.0b1
 Summary: 
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0); python_version < "3.9"
-Requires-Dist: pandas (==1.1.5); python_full_version < "3.7.1"
-Requires-Dist: pandas (==1.3.5); python_full_version >= "3.7.1" and python_version < "3.8"
-Requires-Dist: pandas (>=1.4.2,<1.5.0); python_version >= "3.8"
+Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
+Requires-Dist: pandas (<=1.1.5) ; python_full_version < "3.7.1"
+Requires-Dist: pandas (>=1.3.4,<=1.3.5) ; python_full_version >= "3.7.1" and python_version < "3.8"
+Requires-Dist: pandas (>=1.4.0) ; python_version >= "3.8"
 Requires-Dist: typing-extensions (>=4.2,<5.0)
 Requires-Dist: tzdata (>=2022.6,<2023.0)
 Description-Content-Type: text/markdown
```

