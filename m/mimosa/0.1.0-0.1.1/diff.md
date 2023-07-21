# Comparing `tmp/mimosa-0.1.0.tar.gz` & `tmp/mimosa-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimosa-0.1.0.tar", last modified: Fri Jul 21 08:18:00 2023, max compression
+gzip compressed data, was "mimosa-0.1.1.tar", last modified: Fri Jul 21 08:54:37 2023, max compression
```

## Comparing `mimosa-0.1.0.tar` & `mimosa-0.1.1.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 08:18:00.387225 mimosa-0.1.0/
--rw-rw-rw-   0        0        0       66 2020-05-27 06:46:03.000000 mimosa-0.1.0/.gitattributes
--rw-rw-rw-   0        0        0     2098 2021-05-12 09:46:36.000000 mimosa-0.1.0/.gitignore
--rw-rw-rw-   0        0        0    35822 2020-05-18 11:44:25.000000 mimosa-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       26 2023-07-21 06:53:35.000000 mimosa-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5763 2023-07-21 08:18:00.387225 mimosa-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5477 2023-07-21 06:53:35.000000 mimosa-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.318894 mimosa-0.1.0/mimosa/
--rw-rw-rw-   0        0        0      108 2023-07-21 07:52:23.000000 mimosa-0.1.0/mimosa/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.362212 mimosa-0.1.0/mimosa/__pycache__/
--rw-rw-rw-   0        0        0      275 2023-07-21 07:54:49.000000 mimosa-0.1.0/mimosa/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     3648 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/__pycache__/abstract_model.cpython-310.pyc
--rw-rw-rw-   0        0        0     6915 2023-07-21 07:41:57.000000 mimosa-0.1.0/mimosa/__pycache__/mimosa.cpython-310.pyc
--rw-rw-rw-   0        0        0     5160 2023-07-21 07:41:41.000000 mimosa-0.1.0/mimosa/abstract_model.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.407675 mimosa-0.1.0/mimosa/common/
--rw-rw-rw-   0        0        0     1206 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.427243 mimosa-0.1.0/mimosa/common/__pycache__/
--rw-rw-rw-   0        0        0     1361 2023-07-21 07:41:57.000000 mimosa-0.1.0/mimosa/common/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1405 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/common/__pycache__/economics.cpython-310.pyc
--rw-rw-rw-   0        0        0     9297 2023-07-21 07:41:59.000000 mimosa-0.1.0/mimosa/common/__pycache__/pyomo_utils.cpython-310.pyc
--rw-rw-rw-   0        0        0     3475 2023-07-21 07:42:42.000000 mimosa-0.1.0/mimosa/common/__pycache__/units.cpython-310.pyc
--rw-rw-rw-   0        0        0     1705 2023-07-21 07:42:41.000000 mimosa-0.1.0/mimosa/common/__pycache__/utils.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.436374 mimosa-0.1.0/mimosa/common/config/
--rw-rw-rw-   0        0        0        0 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/common/config/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.447483 mimosa-0.1.0/mimosa/common/config/__pycache__/
--rw-rw-rw-   0        0        0      191 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/common/config/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2230 2023-07-21 07:54:51.000000 mimosa-0.1.0/mimosa/common/config/__pycache__/parseconfig.cpython-310.pyc
--rw-rw-rw-   0        0        0     2429 2023-07-21 07:54:34.000000 mimosa-0.1.0/mimosa/common/config/parseconfig.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.466181 mimosa-0.1.0/mimosa/common/config/utils/
--rw-rw-rw-   0        0        0      112 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/common/config/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.477457 mimosa-0.1.0/mimosa/common/config/utils/__pycache__/
--rw-rw-rw-   0        0        0      352 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/common/config/utils/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1190 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/common/config/utils/__pycache__/nested_dict.cpython-310.pyc
--rw-rw-rw-   0        0        0     9387 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/common/config/utils/__pycache__/parsers.cpython-310.pyc
--rw-rw-rw-   0        0        0      969 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/common/config/utils/nested_dict.py
--rw-rw-rw-   0        0        0     8454 2023-07-21 07:41:43.000000 mimosa-0.1.0/mimosa/common/config/utils/parsers.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.507567 mimosa-0.1.0/mimosa/common/data/
--rw-rw-rw-   0        0        0       36 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/common/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.525585 mimosa-0.1.0/mimosa/common/data/__pycache__/
--rw-rw-rw-   0        0        0      232 2023-07-21 07:42:44.000000 mimosa-0.1.0/mimosa/common/data/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     6111 2023-07-21 07:42:44.000000 mimosa-0.1.0/mimosa/common/data/__pycache__/datastore.cpython-310.pyc
--rw-rw-rw-   0        0        0     1235 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/common/data/__pycache__/utils.cpython-310.pyc
--rw-rw-rw-   0        0        0     6574 2023-07-21 07:42:30.000000 mimosa-0.1.0/mimosa/common/data/datastore.py
--rw-rw-rw-   0        0        0     1463 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/common/data/utils.py
--rw-rw-rw-   0        0        0     1419 2023-07-21 07:41:43.000000 mimosa-0.1.0/mimosa/common/economics.py
--rw-rw-rw-   0        0        0     8234 2023-07-21 07:41:43.000000 mimosa-0.1.0/mimosa/common/pyomo_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.562103 mimosa-0.1.0/mimosa/common/regional_params/
--rw-rw-rw-   0        0        0       38 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/common/regional_params/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.575614 mimosa-0.1.0/mimosa/common/regional_params/__pycache__/
--rw-rw-rw-   0        0        0      247 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/common/regional_params/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2765 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/common/regional_params/__pycache__/main.cpython-310.pyc
--rw-rw-rw-   0        0        0     2404 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/common/regional_params/__pycache__/region_mappers.cpython-310.pyc
--rw-rw-rw-   0        0        0     1334 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/common/regional_params/__pycache__/regional_param_container.cpython-310.pyc
--rw-rw-rw-   0        0        0     2754 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/common/regional_params/main.py
--rw-rw-rw-   0        0        0     2772 2023-07-21 07:42:30.000000 mimosa-0.1.0/mimosa/common/regional_params/region_mappers.py
--rw-rw-rw-   0        0        0     1340 2023-07-21 07:42:30.000000 mimosa-0.1.0/mimosa/common/regional_params/regional_param_container.py
--rw-rw-rw-   0        0        0     3579 2023-07-21 07:42:29.000000 mimosa-0.1.0/mimosa/common/units.py
--rw-rw-rw-   0        0        0     1220 2023-07-21 07:42:29.000000 mimosa-0.1.0/mimosa/common/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.626552 mimosa-0.1.0/mimosa/components/
--rw-rw-rw-   0        0        0        0 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.637424 mimosa-0.1.0/mimosa/components/__pycache__/
--rw-rw-rw-   0        0        0      188 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     4889 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/__pycache__/abatement.cpython-310.pyc
--rw-rw-rw-   0        0        0     3844 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/__pycache__/burdensharing.cpython-310.pyc
--rw-rw-rw-   0        0        0     3333 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/__pycache__/cobbdouglas.cpython-310.pyc
--rw-rw-rw-   0        0        0     6923 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/__pycache__/emissions.cpython-310.pyc
--rw-rw-rw-   0        0        0     3700 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/__pycache__/sealevelrise.cpython-310.pyc
--rw-rw-rw-   0        0        0     5469 2023-07-21 07:41:44.000000 mimosa-0.1.0/mimosa/components/abatement.py
--rw-rw-rw-   0        0        0     4025 2023-07-21 07:41:44.000000 mimosa-0.1.0/mimosa/components/burdensharing.py
--rw-rw-rw-   0        0        0     3697 2023-07-21 07:41:44.000000 mimosa-0.1.0/mimosa/components/cobbdouglas.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.697498 mimosa-0.1.0/mimosa/components/damages/
--rw-rw-rw-   0        0        0      116 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/components/damages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.720649 mimosa-0.1.0/mimosa/components/damages/__pycache__/
--rw-rw-rw-   0        0        0      364 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/damages/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     4552 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/damages/__pycache__/ad_rice2010.cpython-310.pyc
--rw-rw-rw-   0        0        0     4166 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/damages/__pycache__/ad_rice2012.cpython-310.pyc
--rw-rw-rw-   0        0        0     4299 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/damages/__pycache__/ad_witch.cpython-310.pyc
--rw-rw-rw-   0        0        0     3277 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/damages/__pycache__/coacch.cpython-310.pyc
--rw-rw-rw-   0        0        0     1274 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/damages/__pycache__/nodamage.cpython-310.pyc
--rw-rw-rw-   0        0        0     5331 2023-07-21 07:41:45.000000 mimosa-0.1.0/mimosa/components/damages/ad_rice2010.py
--rw-rw-rw-   0        0        0     4874 2023-07-21 07:41:45.000000 mimosa-0.1.0/mimosa/components/damages/ad_rice2012.py
--rw-rw-rw-   0        0        0     6688 2023-07-21 07:41:46.000000 mimosa-0.1.0/mimosa/components/damages/ad_witch.py
--rw-rw-rw-   0        0        0     4260 2023-07-21 07:41:45.000000 mimosa-0.1.0/mimosa/components/damages/coacch.py
--rw-rw-rw-   0        0        0      971 2023-07-21 07:41:45.000000 mimosa-0.1.0/mimosa/components/damages/nodamage.py
--rw-rw-rw-   0        0        0    10151 2023-07-21 07:41:44.000000 mimosa-0.1.0/mimosa/components/emissions.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.777554 mimosa-0.1.0/mimosa/components/emissiontrade/
--rw-rw-rw-   0        0        0      112 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/components/emissiontrade/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.806265 mimosa-0.1.0/mimosa/components/emissiontrade/__pycache__/
--rw-rw-rw-   0        0        0      348 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/emissiontrade/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     3898 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/emissiontrade/__pycache__/emissiontrade.cpython-310.pyc
--rw-rw-rw-   0        0        0     2968 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/emissiontrade/__pycache__/globalcostpool.cpython-310.pyc
--rw-rw-rw-   0        0        0     1414 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/emissiontrade/__pycache__/notrade.cpython-310.pyc
--rw-rw-rw-   0        0        0     5274 2023-07-21 07:41:45.000000 mimosa-0.1.0/mimosa/components/emissiontrade/emissiontrade.py
--rw-rw-rw-   0        0        0     3276 2023-07-21 07:41:44.000000 mimosa-0.1.0/mimosa/components/emissiontrade/globalcostpool.py
--rw-rw-rw-   0        0        0     1131 2023-07-21 07:41:44.000000 mimosa-0.1.0/mimosa/components/emissiontrade/notrade.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.837295 mimosa-0.1.0/mimosa/components/financialtransfer/
--rw-rw-rw-   0        0        0      105 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/components/financialtransfer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.856808 mimosa-0.1.0/mimosa/components/financialtransfer/__pycache__/
--rw-rw-rw-   0        0        0      336 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/financialtransfer/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2230 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/financialtransfer/__pycache__/globaldamagepool.cpython-310.pyc
--rw-rw-rw-   0        0        0     1093 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/financialtransfer/__pycache__/notransfer.cpython-310.pyc
--rw-rw-rw-   0        0        0     1968 2023-07-21 07:41:44.000000 mimosa-0.1.0/mimosa/components/financialtransfer/globaldamagepool.py
--rw-rw-rw-   0        0        0      939 2023-07-21 07:41:44.000000 mimosa-0.1.0/mimosa/components/financialtransfer/notransfer.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.886306 mimosa-0.1.0/mimosa/components/objective/
--rw-rw-rw-   0        0        0      101 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/components/objective/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.897351 mimosa-0.1.0/mimosa/components/objective/__pycache__/
--rw-rw-rw-   0        0        0      322 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/objective/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2118 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/objective/__pycache__/globalcosts.cpython-310.pyc
--rw-rw-rw-   0        0        0     1736 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/objective/__pycache__/utility.cpython-310.pyc
--rw-rw-rw-   0        0        0     1558 2023-07-21 07:41:44.000000 mimosa-0.1.0/mimosa/components/objective/globalcosts.py
--rw-rw-rw-   0        0        0     1713 2023-07-21 07:41:44.000000 mimosa-0.1.0/mimosa/components/objective/utility.py
--rw-rw-rw-   0        0        0     4213 2023-07-21 07:41:44.000000 mimosa-0.1.0/mimosa/components/sealevelrise.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.937281 mimosa-0.1.0/mimosa/components/welfare/
--rw-rw-rw-   0        0        0      165 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/components/welfare/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.957696 mimosa-0.1.0/mimosa/components/welfare/__pycache__/
--rw-rw-rw-   0        0        0      391 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/welfare/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1882 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/welfare/__pycache__/inequal_aversion_elasmu.cpython-310.pyc
--rw-rw-rw-   0        0        0     2368 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/welfare/__pycache__/inequal_aversion_general.cpython-310.pyc
--rw-rw-rw-   0        0        0     2133 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/components/welfare/__pycache__/inequal_aversion_zero.cpython-310.pyc
--rw-rw-rw-   0        0        0     1456 2023-07-21 07:41:44.000000 mimosa-0.1.0/mimosa/components/welfare/inequal_aversion_elasmu.py
--rw-rw-rw-   0        0        0     2048 2023-07-21 07:41:44.000000 mimosa-0.1.0/mimosa/components/welfare/inequal_aversion_general.py
--rw-rw-rw-   0        0        0     1663 2023-07-21 07:41:44.000000 mimosa-0.1.0/mimosa/components/welfare/inequal_aversion_zero.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.967113 mimosa-0.1.0/mimosa/concrete_model/
--rw-rw-rw-   0        0        0        0 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/concrete_model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.976199 mimosa-0.1.0/mimosa/concrete_model/__pycache__/
--rw-rw-rw-   0        0        0      192 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/concrete_model/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     8590 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/concrete_model/__pycache__/instantiate_params.cpython-310.pyc
--rw-rw-rw-   0        0        0    15078 2023-07-21 07:41:42.000000 mimosa-0.1.0/mimosa/concrete_model/instantiate_params.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:18:00.037240 mimosa-0.1.0/mimosa/concrete_model/simulation_mode/
--rw-rw-rw-   0        0        0       39 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/concrete_model/simulation_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:18:00.061794 mimosa-0.1.0/mimosa/concrete_model/simulation_mode/__pycache__/
--rw-rw-rw-   0        0        0      256 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/concrete_model/simulation_mode/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      677 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/concrete_model/simulation_mode/__pycache__/deactivate_constraints.cpython-310.pyc
--rw-rw-rw-   0        0        0     1046 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/concrete_model/simulation_mode/__pycache__/main.cpython-310.pyc
--rw-rw-rw-   0        0        0     2504 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/concrete_model/simulation_mode/__pycache__/set_constraints.cpython-310.pyc
--rw-rw-rw-   0        0        0     2101 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/concrete_model/simulation_mode/__pycache__/utils.cpython-310.pyc
--rw-rw-rw-   0        0        0      493 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/concrete_model/simulation_mode/deactivate_constraints.py
--rw-rw-rw-   0        0        0      907 2023-07-21 07:41:42.000000 mimosa-0.1.0/mimosa/concrete_model/simulation_mode/main.py
--rw-rw-rw-   0        0        0     3369 2023-07-21 07:41:42.000000 mimosa-0.1.0/mimosa/concrete_model/simulation_mode/set_constraints.py
--rw-rw-rw-   0        0        0     1557 2023-07-21 07:41:42.000000 mimosa-0.1.0/mimosa/concrete_model/simulation_mode/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:18:00.117749 mimosa-0.1.0/mimosa/export/
--rw-rw-rw-   0        0        0      202 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/export/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:18:00.127231 mimosa-0.1.0/mimosa/export/__pycache__/
--rw-rw-rw-   0        0        0      418 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/export/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     3355 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/export/__pycache__/plot.cpython-310.pyc
--rw-rw-rw-   0        0        0     2567 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/export/__pycache__/save.cpython-310.pyc
--rw-rw-rw-   0        0        0     5349 2023-07-21 07:42:48.000000 mimosa-0.1.0/mimosa/export/__pycache__/utils.cpython-310.pyc
--rw-rw-rw-   0        0        0     5262 2023-07-21 07:41:42.000000 mimosa-0.1.0/mimosa/export/plot.py
--rw-rw-rw-   0        0        0     3110 2023-07-21 07:41:42.000000 mimosa-0.1.0/mimosa/export/save.py
--rw-rw-rw-   0        0        0     5783 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/export/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.226533 mimosa-0.1.0/mimosa/inputdata/
-drwxrwxrwx   0        0        0        0 2023-07-21 08:18:00.187471 mimosa-0.1.0/mimosa/inputdata/config/
--rw-rw-rw-   0        0        0       13 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/inputdata/config/config.yaml
--rw-rw-rw-   0        0        0     2296 2023-07-21 07:42:29.000000 mimosa-0.1.0/mimosa/inputdata/config/config_R5.yaml
--rw-rw-rw-   0        0        0    13790 2023-07-21 07:42:30.000000 mimosa-0.1.0/mimosa/inputdata/config/config_default.yaml
--rw-rw-rw-   0        0        0      154 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/inputdata/config/default_units.yaml
--rw-rw-rw-   0        0        0      456 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/inputdata/config/extra_units.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 08:18:00.206547 mimosa-0.1.0/mimosa/inputdata/data/
--rw-rw-rw-   0        0        0    89096 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/inputdata/data/data_IMAGE_SSP.csv
--rw-rw-rw-   0        0        0    89101 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/inputdata/data/data_IMAGE_SSP_harmonised_2020.csv
-drwxrwxrwx   0        0        0        0 2023-07-21 08:18:00.277391 mimosa-0.1.0/mimosa/inputdata/params/
--rw-rw-rw-   0        0        0      491 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/inputdata/params/ADRICE2010.csv
--rw-rw-rw-   0        0        0      593 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/inputdata/params/ADRICE2012.csv
--rw-rw-rw-   0        0        0    34077 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/inputdata/params/COACCH.csv
--rw-rw-rw-   0        0        0      321 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/inputdata/params/economics.csv
--rw-rw-rw-   0        0        0     7044 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/inputdata/params/mac.csv
-drwxrwxrwx   0        0        0        0 2023-07-21 08:18:00.366264 mimosa-0.1.0/mimosa/inputdata/regions/
--rw-rw-rw-   0        0        0      286 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/inputdata/regions/IMAGE26_ADRICE2010.csv
--rw-rw-rw-   0        0        0      280 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/inputdata/regions/IMAGE26_ADRICE2012.csv
--rw-rw-rw-   0        0        0      337 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/inputdata/regions/IMAGE26_COACCH.csv
--rw-rw-rw-   0        0        0   167460 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/inputdata/regions/IMAGE26_regions.json
--rw-rw-rw-   0        0        0   123689 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/inputdata/regions/R5_regions.json
--rw-rw-rw-   0        0        0    21007 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/inputdata/regions/country_ISO_codes.csv
--rw-rw-rw-   0        0        0     8217 2023-07-21 07:41:41.000000 mimosa-0.1.0/mimosa/mimosa.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:18:00.387225 mimosa-0.1.0/mimosa/socialcostofcarbon/
--rw-rw-rw-   0        0        0        0 2023-07-21 06:54:00.000000 mimosa-0.1.0/mimosa/socialcostofcarbon/__init__.py
--rw-rw-rw-   0        0        0     5546 2023-07-21 07:41:42.000000 mimosa-0.1.0/mimosa/socialcostofcarbon/scc.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:17:59.353592 mimosa-0.1.0/mimosa.egg-info/
--rw-rw-rw-   0        0        0     5763 2023-07-21 08:17:59.000000 mimosa-0.1.0/mimosa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6851 2023-07-21 08:17:59.000000 mimosa-0.1.0/mimosa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 08:17:59.000000 mimosa-0.1.0/mimosa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-21 08:17:59.000000 mimosa-0.1.0/mimosa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-21 08:17:59.000000 mimosa-0.1.0/mimosa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-21 08:04:00.000000 mimosa-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       61 2023-07-21 06:53:35.000000 mimosa-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0      217 2023-07-21 07:56:33.000000 mimosa-0.1.0/run.py
--rw-rw-rw-   0        0        0       42 2023-07-21 08:18:00.387225 mimosa-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      612 2023-07-21 08:16:00.000000 mimosa-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:37.118028 mimosa-0.1.1/
+-rw-rw-rw-   0        0        0       66 2020-05-27 06:46:03.000000 mimosa-0.1.1/.gitattributes
+-rw-rw-rw-   0        0        0     2098 2021-05-12 09:46:36.000000 mimosa-0.1.1/.gitignore
+-rw-rw-rw-   0        0        0    35822 2020-05-18 11:44:25.000000 mimosa-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-07-21 06:53:35.000000 mimosa-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5763 2023-07-21 08:54:37.108992 mimosa-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5477 2023-07-21 06:53:35.000000 mimosa-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.710850 mimosa-0.1.1/mimosa/
+-rw-rw-rw-   0        0        0      108 2023-07-21 07:52:23.000000 mimosa-0.1.1/mimosa/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.758875 mimosa-0.1.1/mimosa/__pycache__/
+-rw-rw-rw-   0        0        0      275 2023-07-21 07:54:49.000000 mimosa-0.1.1/mimosa/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3648 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/__pycache__/abstract_model.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6915 2023-07-21 07:41:57.000000 mimosa-0.1.1/mimosa/__pycache__/mimosa.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5160 2023-07-21 07:41:41.000000 mimosa-0.1.1/mimosa/abstract_model.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.771986 mimosa-0.1.1/mimosa/common/
+-rw-rw-rw-   0        0        0     1206 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.787763 mimosa-0.1.1/mimosa/common/__pycache__/
+-rw-rw-rw-   0        0        0     1361 2023-07-21 07:41:57.000000 mimosa-0.1.1/mimosa/common/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1405 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/common/__pycache__/economics.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9297 2023-07-21 07:41:59.000000 mimosa-0.1.1/mimosa/common/__pycache__/pyomo_utils.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3475 2023-07-21 07:42:42.000000 mimosa-0.1.1/mimosa/common/__pycache__/units.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1705 2023-07-21 07:42:41.000000 mimosa-0.1.1/mimosa/common/__pycache__/utils.cpython-310.pyc
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.792758 mimosa-0.1.1/mimosa/common/config/
+-rw-rw-rw-   0        0        0        0 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/common/config/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.797761 mimosa-0.1.1/mimosa/common/config/__pycache__/
+-rw-rw-rw-   0        0        0      191 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/common/config/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2230 2023-07-21 07:54:51.000000 mimosa-0.1.1/mimosa/common/config/__pycache__/parseconfig.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2429 2023-07-21 07:54:34.000000 mimosa-0.1.1/mimosa/common/config/parseconfig.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.807084 mimosa-0.1.1/mimosa/common/config/utils/
+-rw-rw-rw-   0        0        0      112 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/common/config/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.812101 mimosa-0.1.1/mimosa/common/config/utils/__pycache__/
+-rw-rw-rw-   0        0        0      352 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/common/config/utils/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1190 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/common/config/utils/__pycache__/nested_dict.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9387 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/common/config/utils/__pycache__/parsers.cpython-310.pyc
+-rw-rw-rw-   0        0        0      969 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/common/config/utils/nested_dict.py
+-rw-rw-rw-   0        0        0     8454 2023-07-21 07:41:43.000000 mimosa-0.1.1/mimosa/common/config/utils/parsers.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.819232 mimosa-0.1.1/mimosa/common/data/
+-rw-rw-rw-   0        0        0       36 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/common/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.828907 mimosa-0.1.1/mimosa/common/data/__pycache__/
+-rw-rw-rw-   0        0        0      232 2023-07-21 07:42:44.000000 mimosa-0.1.1/mimosa/common/data/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6111 2023-07-21 07:42:44.000000 mimosa-0.1.1/mimosa/common/data/__pycache__/datastore.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1235 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/common/data/__pycache__/utils.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6574 2023-07-21 07:42:30.000000 mimosa-0.1.1/mimosa/common/data/datastore.py
+-rw-rw-rw-   0        0        0     1463 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/common/data/utils.py
+-rw-rw-rw-   0        0        0     1419 2023-07-21 07:41:43.000000 mimosa-0.1.1/mimosa/common/economics.py
+-rw-rw-rw-   0        0        0     8234 2023-07-21 07:41:43.000000 mimosa-0.1.1/mimosa/common/pyomo_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.837989 mimosa-0.1.1/mimosa/common/regional_params/
+-rw-rw-rw-   0        0        0       38 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/common/regional_params/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.849510 mimosa-0.1.1/mimosa/common/regional_params/__pycache__/
+-rw-rw-rw-   0        0        0      247 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/common/regional_params/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2765 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/common/regional_params/__pycache__/main.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2404 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/common/regional_params/__pycache__/region_mappers.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1334 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/common/regional_params/__pycache__/regional_param_container.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2754 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/common/regional_params/main.py
+-rw-rw-rw-   0        0        0     2772 2023-07-21 07:42:30.000000 mimosa-0.1.1/mimosa/common/regional_params/region_mappers.py
+-rw-rw-rw-   0        0        0     1340 2023-07-21 07:42:30.000000 mimosa-0.1.1/mimosa/common/regional_params/regional_param_container.py
+-rw-rw-rw-   0        0        0     3579 2023-07-21 07:42:29.000000 mimosa-0.1.1/mimosa/common/units.py
+-rw-rw-rw-   0        0        0     1220 2023-07-21 07:42:29.000000 mimosa-0.1.1/mimosa/common/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.867980 mimosa-0.1.1/mimosa/components/
+-rw-rw-rw-   0        0        0        0 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.886773 mimosa-0.1.1/mimosa/components/__pycache__/
+-rw-rw-rw-   0        0        0      188 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4889 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/__pycache__/abatement.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3844 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/__pycache__/burdensharing.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3333 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/__pycache__/cobbdouglas.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6923 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/__pycache__/emissions.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3700 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/__pycache__/sealevelrise.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5469 2023-07-21 07:41:44.000000 mimosa-0.1.1/mimosa/components/abatement.py
+-rw-rw-rw-   0        0        0     4025 2023-07-21 07:41:44.000000 mimosa-0.1.1/mimosa/components/burdensharing.py
+-rw-rw-rw-   0        0        0     3697 2023-07-21 07:41:44.000000 mimosa-0.1.1/mimosa/components/cobbdouglas.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.901272 mimosa-0.1.1/mimosa/components/damages/
+-rw-rw-rw-   0        0        0      116 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/components/damages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.917777 mimosa-0.1.1/mimosa/components/damages/__pycache__/
+-rw-rw-rw-   0        0        0      364 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/damages/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4552 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/damages/__pycache__/ad_rice2010.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4166 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/damages/__pycache__/ad_rice2012.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4299 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/damages/__pycache__/ad_witch.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3277 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/damages/__pycache__/coacch.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1274 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/damages/__pycache__/nodamage.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5331 2023-07-21 07:41:45.000000 mimosa-0.1.1/mimosa/components/damages/ad_rice2010.py
+-rw-rw-rw-   0        0        0     4874 2023-07-21 07:41:45.000000 mimosa-0.1.1/mimosa/components/damages/ad_rice2012.py
+-rw-rw-rw-   0        0        0     6688 2023-07-21 07:41:46.000000 mimosa-0.1.1/mimosa/components/damages/ad_witch.py
+-rw-rw-rw-   0        0        0     4260 2023-07-21 07:41:45.000000 mimosa-0.1.1/mimosa/components/damages/coacch.py
+-rw-rw-rw-   0        0        0      971 2023-07-21 07:41:45.000000 mimosa-0.1.1/mimosa/components/damages/nodamage.py
+-rw-rw-rw-   0        0        0    10151 2023-07-21 07:41:44.000000 mimosa-0.1.1/mimosa/components/emissions.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.927768 mimosa-0.1.1/mimosa/components/emissiontrade/
+-rw-rw-rw-   0        0        0      112 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/components/emissiontrade/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.938945 mimosa-0.1.1/mimosa/components/emissiontrade/__pycache__/
+-rw-rw-rw-   0        0        0      348 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/emissiontrade/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3898 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/emissiontrade/__pycache__/emissiontrade.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2968 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/emissiontrade/__pycache__/globalcostpool.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1414 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/emissiontrade/__pycache__/notrade.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5274 2023-07-21 07:41:45.000000 mimosa-0.1.1/mimosa/components/emissiontrade/emissiontrade.py
+-rw-rw-rw-   0        0        0     3276 2023-07-21 07:41:44.000000 mimosa-0.1.1/mimosa/components/emissiontrade/globalcostpool.py
+-rw-rw-rw-   0        0        0     1131 2023-07-21 07:41:44.000000 mimosa-0.1.1/mimosa/components/emissiontrade/notrade.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.948894 mimosa-0.1.1/mimosa/components/financialtransfer/
+-rw-rw-rw-   0        0        0      105 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/components/financialtransfer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.958948 mimosa-0.1.1/mimosa/components/financialtransfer/__pycache__/
+-rw-rw-rw-   0        0        0      336 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/financialtransfer/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2230 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/financialtransfer/__pycache__/globaldamagepool.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1093 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/financialtransfer/__pycache__/notransfer.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1968 2023-07-21 07:41:44.000000 mimosa-0.1.1/mimosa/components/financialtransfer/globaldamagepool.py
+-rw-rw-rw-   0        0        0      939 2023-07-21 07:41:44.000000 mimosa-0.1.1/mimosa/components/financialtransfer/notransfer.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.977043 mimosa-0.1.1/mimosa/components/objective/
+-rw-rw-rw-   0        0        0      101 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/components/objective/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.987745 mimosa-0.1.1/mimosa/components/objective/__pycache__/
+-rw-rw-rw-   0        0        0      322 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/objective/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2118 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/objective/__pycache__/globalcosts.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1736 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/objective/__pycache__/utility.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1558 2023-07-21 07:41:44.000000 mimosa-0.1.1/mimosa/components/objective/globalcosts.py
+-rw-rw-rw-   0        0        0     1713 2023-07-21 07:41:44.000000 mimosa-0.1.1/mimosa/components/objective/utility.py
+-rw-rw-rw-   0        0        0     4213 2023-07-21 07:41:44.000000 mimosa-0.1.1/mimosa/components/sealevelrise.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.997820 mimosa-0.1.1/mimosa/components/welfare/
+-rw-rw-rw-   0        0        0      165 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/components/welfare/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:37.008993 mimosa-0.1.1/mimosa/components/welfare/__pycache__/
+-rw-rw-rw-   0        0        0      391 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/welfare/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1882 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/welfare/__pycache__/inequal_aversion_elasmu.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2368 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/welfare/__pycache__/inequal_aversion_general.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2133 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/components/welfare/__pycache__/inequal_aversion_zero.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1456 2023-07-21 07:41:44.000000 mimosa-0.1.1/mimosa/components/welfare/inequal_aversion_elasmu.py
+-rw-rw-rw-   0        0        0     2048 2023-07-21 07:41:44.000000 mimosa-0.1.1/mimosa/components/welfare/inequal_aversion_general.py
+-rw-rw-rw-   0        0        0     1663 2023-07-21 07:41:44.000000 mimosa-0.1.1/mimosa/components/welfare/inequal_aversion_zero.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:37.008993 mimosa-0.1.1/mimosa/concrete_model/
+-rw-rw-rw-   0        0        0        0 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/concrete_model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:37.019003 mimosa-0.1.1/mimosa/concrete_model/__pycache__/
+-rw-rw-rw-   0        0        0      192 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/concrete_model/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8590 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/concrete_model/__pycache__/instantiate_params.cpython-310.pyc
+-rw-rw-rw-   0        0        0    15078 2023-07-21 07:41:42.000000 mimosa-0.1.1/mimosa/concrete_model/instantiate_params.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:37.028031 mimosa-0.1.1/mimosa/concrete_model/simulation_mode/
+-rw-rw-rw-   0        0        0       39 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/concrete_model/simulation_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:37.049243 mimosa-0.1.1/mimosa/concrete_model/simulation_mode/__pycache__/
+-rw-rw-rw-   0        0        0      256 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/concrete_model/simulation_mode/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      677 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/concrete_model/simulation_mode/__pycache__/deactivate_constraints.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1046 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/concrete_model/simulation_mode/__pycache__/main.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2504 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/concrete_model/simulation_mode/__pycache__/set_constraints.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2101 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/concrete_model/simulation_mode/__pycache__/utils.cpython-310.pyc
+-rw-rw-rw-   0        0        0      493 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/concrete_model/simulation_mode/deactivate_constraints.py
+-rw-rw-rw-   0        0        0      907 2023-07-21 07:41:42.000000 mimosa-0.1.1/mimosa/concrete_model/simulation_mode/main.py
+-rw-rw-rw-   0        0        0     3369 2023-07-21 07:41:42.000000 mimosa-0.1.1/mimosa/concrete_model/simulation_mode/set_constraints.py
+-rw-rw-rw-   0        0        0     1557 2023-07-21 07:41:42.000000 mimosa-0.1.1/mimosa/concrete_model/simulation_mode/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:37.057812 mimosa-0.1.1/mimosa/export/
+-rw-rw-rw-   0        0        0      202 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/export/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:37.068935 mimosa-0.1.1/mimosa/export/__pycache__/
+-rw-rw-rw-   0        0        0      418 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/export/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3355 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/export/__pycache__/plot.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2567 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/export/__pycache__/save.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5349 2023-07-21 07:42:48.000000 mimosa-0.1.1/mimosa/export/__pycache__/utils.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5262 2023-07-21 07:41:42.000000 mimosa-0.1.1/mimosa/export/plot.py
+-rw-rw-rw-   0        0        0     3110 2023-07-21 07:41:42.000000 mimosa-0.1.1/mimosa/export/save.py
+-rw-rw-rw-   0        0        0     5783 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/export/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.684095 mimosa-0.1.1/mimosa/inputdata/
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:37.079032 mimosa-0.1.1/mimosa/inputdata/config/
+-rw-rw-rw-   0        0        0       13 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/inputdata/config/config.yaml
+-rw-rw-rw-   0        0        0     2296 2023-07-21 07:42:29.000000 mimosa-0.1.1/mimosa/inputdata/config/config_R5.yaml
+-rw-rw-rw-   0        0        0    13790 2023-07-21 07:42:30.000000 mimosa-0.1.1/mimosa/inputdata/config/config_default.yaml
+-rw-rw-rw-   0        0        0      154 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/inputdata/config/default_units.yaml
+-rw-rw-rw-   0        0        0      456 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/inputdata/config/extra_units.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:37.079032 mimosa-0.1.1/mimosa/inputdata/data/
+-rw-rw-rw-   0        0        0    89096 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/inputdata/data/data_IMAGE_SSP.csv
+-rw-rw-rw-   0        0        0    89101 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/inputdata/data/data_IMAGE_SSP_harmonised_2020.csv
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:37.097220 mimosa-0.1.1/mimosa/inputdata/params/
+-rw-rw-rw-   0        0        0      491 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/inputdata/params/ADRICE2010.csv
+-rw-rw-rw-   0        0        0      593 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/inputdata/params/ADRICE2012.csv
+-rw-rw-rw-   0        0        0    34077 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/inputdata/params/COACCH.csv
+-rw-rw-rw-   0        0        0      321 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/inputdata/params/economics.csv
+-rw-rw-rw-   0        0        0     7044 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/inputdata/params/mac.csv
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:37.108992 mimosa-0.1.1/mimosa/inputdata/regions/
+-rw-rw-rw-   0        0        0      286 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/inputdata/regions/IMAGE26_ADRICE2010.csv
+-rw-rw-rw-   0        0        0      280 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/inputdata/regions/IMAGE26_ADRICE2012.csv
+-rw-rw-rw-   0        0        0      337 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/inputdata/regions/IMAGE26_COACCH.csv
+-rw-rw-rw-   0        0        0   167460 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/inputdata/regions/IMAGE26_regions.json
+-rw-rw-rw-   0        0        0   123689 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/inputdata/regions/R5_regions.json
+-rw-rw-rw-   0        0        0    21007 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/inputdata/regions/country_ISO_codes.csv
+-rw-rw-rw-   0        0        0     8217 2023-07-21 07:41:41.000000 mimosa-0.1.1/mimosa/mimosa.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:37.108992 mimosa-0.1.1/mimosa/socialcostofcarbon/
+-rw-rw-rw-   0        0        0        0 2023-07-21 06:54:00.000000 mimosa-0.1.1/mimosa/socialcostofcarbon/__init__.py
+-rw-rw-rw-   0        0        0     5546 2023-07-21 07:41:42.000000 mimosa-0.1.1/mimosa/socialcostofcarbon/scc.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:54:36.749379 mimosa-0.1.1/mimosa.egg-info/
+-rw-rw-rw-   0        0        0     5763 2023-07-21 08:54:36.000000 mimosa-0.1.1/mimosa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6851 2023-07-21 08:54:36.000000 mimosa-0.1.1/mimosa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 08:54:36.000000 mimosa-0.1.1/mimosa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-21 08:54:36.000000 mimosa-0.1.1/mimosa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-21 08:54:36.000000 mimosa-0.1.1/mimosa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-21 08:04:00.000000 mimosa-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       61 2023-07-21 06:53:35.000000 mimosa-0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0      217 2023-07-21 07:56:33.000000 mimosa-0.1.1/run.py
+-rw-rw-rw-   0        0        0       42 2023-07-21 08:54:37.118028 mimosa-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      621 2023-07-21 08:54:16.000000 mimosa-0.1.1/setup.py
```

### Comparing `mimosa-0.1.0/.gitignore` & `mimosa-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/LICENSE` & `mimosa-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/PKG-INFO` & `mimosa-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimosa
-Version: 0.1.0
+Version: 0.1.1
 Summary: MIMOSA: Integrated Assessment Model for Cost-Benefit Analysis
 Author: Kaj-Ivar van der Wijst
 Author-email: k.i.vanderwijst@gmail.com
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mimosa-0.1.0/README.md` & `mimosa-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/__pycache__/abstract_model.cpython-310.pyc` & `mimosa-0.1.1/mimosa/__pycache__/abstract_model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/__pycache__/mimosa.cpython-310.pyc` & `mimosa-0.1.1/mimosa/__pycache__/mimosa.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/abstract_model.py` & `mimosa-0.1.1/mimosa/abstract_model.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/__init__.py` & `mimosa-0.1.1/mimosa/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/__pycache__/__init__.cpython-310.pyc` & `mimosa-0.1.1/mimosa/common/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/__pycache__/economics.cpython-310.pyc` & `mimosa-0.1.1/mimosa/common/__pycache__/economics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/__pycache__/pyomo_utils.cpython-310.pyc` & `mimosa-0.1.1/mimosa/common/__pycache__/pyomo_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/__pycache__/units.cpython-310.pyc` & `mimosa-0.1.1/mimosa/common/__pycache__/units.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/__pycache__/utils.cpython-310.pyc` & `mimosa-0.1.1/mimosa/common/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/config/__pycache__/parseconfig.cpython-310.pyc` & `mimosa-0.1.1/mimosa/common/config/__pycache__/parseconfig.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/config/parseconfig.py` & `mimosa-0.1.1/mimosa/common/config/parseconfig.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/config/utils/__pycache__/nested_dict.cpython-310.pyc` & `mimosa-0.1.1/mimosa/common/config/utils/__pycache__/nested_dict.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/config/utils/__pycache__/parsers.cpython-310.pyc` & `mimosa-0.1.1/mimosa/common/config/utils/__pycache__/parsers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/config/utils/nested_dict.py` & `mimosa-0.1.1/mimosa/common/config/utils/nested_dict.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/config/utils/parsers.py` & `mimosa-0.1.1/mimosa/common/config/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/data/__pycache__/datastore.cpython-310.pyc` & `mimosa-0.1.1/mimosa/common/data/__pycache__/datastore.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/data/__pycache__/utils.cpython-310.pyc` & `mimosa-0.1.1/mimosa/common/data/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/data/datastore.py` & `mimosa-0.1.1/mimosa/common/data/datastore.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/data/utils.py` & `mimosa-0.1.1/mimosa/common/data/utils.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/economics.py` & `mimosa-0.1.1/mimosa/common/economics.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/pyomo_utils.py` & `mimosa-0.1.1/mimosa/common/pyomo_utils.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/regional_params/__pycache__/main.cpython-310.pyc` & `mimosa-0.1.1/mimosa/common/regional_params/__pycache__/main.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/regional_params/__pycache__/region_mappers.cpython-310.pyc` & `mimosa-0.1.1/mimosa/common/regional_params/__pycache__/region_mappers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/regional_params/__pycache__/regional_param_container.cpython-310.pyc` & `mimosa-0.1.1/mimosa/common/regional_params/__pycache__/regional_param_container.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/regional_params/main.py` & `mimosa-0.1.1/mimosa/common/regional_params/main.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/regional_params/region_mappers.py` & `mimosa-0.1.1/mimosa/common/regional_params/region_mappers.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/regional_params/regional_param_container.py` & `mimosa-0.1.1/mimosa/common/regional_params/regional_param_container.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/units.py` & `mimosa-0.1.1/mimosa/common/units.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/common/utils.py` & `mimosa-0.1.1/mimosa/common/utils.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/__pycache__/abatement.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/__pycache__/abatement.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/__pycache__/burdensharing.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/__pycache__/burdensharing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/__pycache__/cobbdouglas.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/__pycache__/cobbdouglas.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/__pycache__/emissions.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/__pycache__/emissions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/__pycache__/sealevelrise.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/__pycache__/sealevelrise.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/abatement.py` & `mimosa-0.1.1/mimosa/components/abatement.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/burdensharing.py` & `mimosa-0.1.1/mimosa/components/burdensharing.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/cobbdouglas.py` & `mimosa-0.1.1/mimosa/components/cobbdouglas.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/damages/__pycache__/ad_rice2010.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/damages/__pycache__/ad_rice2010.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/damages/__pycache__/ad_rice2012.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/damages/__pycache__/ad_rice2012.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/damages/__pycache__/ad_witch.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/damages/__pycache__/ad_witch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/damages/__pycache__/coacch.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/damages/__pycache__/coacch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/damages/__pycache__/nodamage.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/damages/__pycache__/nodamage.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/damages/ad_rice2010.py` & `mimosa-0.1.1/mimosa/components/damages/ad_rice2010.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/damages/ad_rice2012.py` & `mimosa-0.1.1/mimosa/components/damages/ad_rice2012.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/damages/ad_witch.py` & `mimosa-0.1.1/mimosa/components/damages/ad_witch.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/damages/coacch.py` & `mimosa-0.1.1/mimosa/components/damages/coacch.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/damages/nodamage.py` & `mimosa-0.1.1/mimosa/components/damages/nodamage.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/emissions.py` & `mimosa-0.1.1/mimosa/components/emissions.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/emissiontrade/__pycache__/emissiontrade.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/emissiontrade/__pycache__/emissiontrade.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/emissiontrade/__pycache__/globalcostpool.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/emissiontrade/__pycache__/globalcostpool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/emissiontrade/__pycache__/notrade.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/emissiontrade/__pycache__/notrade.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/emissiontrade/emissiontrade.py` & `mimosa-0.1.1/mimosa/components/emissiontrade/emissiontrade.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/emissiontrade/globalcostpool.py` & `mimosa-0.1.1/mimosa/components/emissiontrade/globalcostpool.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/emissiontrade/notrade.py` & `mimosa-0.1.1/mimosa/components/emissiontrade/notrade.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/financialtransfer/__pycache__/globaldamagepool.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/financialtransfer/__pycache__/globaldamagepool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/financialtransfer/__pycache__/notransfer.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/financialtransfer/__pycache__/notransfer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/financialtransfer/globaldamagepool.py` & `mimosa-0.1.1/mimosa/components/financialtransfer/globaldamagepool.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/financialtransfer/notransfer.py` & `mimosa-0.1.1/mimosa/components/financialtransfer/notransfer.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/objective/__pycache__/globalcosts.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/objective/__pycache__/globalcosts.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/objective/__pycache__/utility.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/objective/__pycache__/utility.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/objective/globalcosts.py` & `mimosa-0.1.1/mimosa/components/objective/globalcosts.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/objective/utility.py` & `mimosa-0.1.1/mimosa/components/objective/utility.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/sealevelrise.py` & `mimosa-0.1.1/mimosa/components/sealevelrise.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/welfare/__pycache__/inequal_aversion_elasmu.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/welfare/__pycache__/inequal_aversion_elasmu.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/welfare/__pycache__/inequal_aversion_general.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/welfare/__pycache__/inequal_aversion_general.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/welfare/__pycache__/inequal_aversion_zero.cpython-310.pyc` & `mimosa-0.1.1/mimosa/components/welfare/__pycache__/inequal_aversion_zero.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/welfare/inequal_aversion_elasmu.py` & `mimosa-0.1.1/mimosa/components/welfare/inequal_aversion_elasmu.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/welfare/inequal_aversion_general.py` & `mimosa-0.1.1/mimosa/components/welfare/inequal_aversion_general.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/components/welfare/inequal_aversion_zero.py` & `mimosa-0.1.1/mimosa/components/welfare/inequal_aversion_zero.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/concrete_model/__pycache__/instantiate_params.cpython-310.pyc` & `mimosa-0.1.1/mimosa/concrete_model/__pycache__/instantiate_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/concrete_model/instantiate_params.py` & `mimosa-0.1.1/mimosa/concrete_model/instantiate_params.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/concrete_model/simulation_mode/__pycache__/deactivate_constraints.cpython-310.pyc` & `mimosa-0.1.1/mimosa/concrete_model/simulation_mode/__pycache__/deactivate_constraints.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/concrete_model/simulation_mode/__pycache__/main.cpython-310.pyc` & `mimosa-0.1.1/mimosa/concrete_model/simulation_mode/__pycache__/main.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/concrete_model/simulation_mode/__pycache__/set_constraints.cpython-310.pyc` & `mimosa-0.1.1/mimosa/concrete_model/simulation_mode/__pycache__/set_constraints.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/concrete_model/simulation_mode/__pycache__/utils.cpython-310.pyc` & `mimosa-0.1.1/mimosa/concrete_model/simulation_mode/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/concrete_model/simulation_mode/main.py` & `mimosa-0.1.1/mimosa/concrete_model/simulation_mode/main.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/concrete_model/simulation_mode/set_constraints.py` & `mimosa-0.1.1/mimosa/concrete_model/simulation_mode/set_constraints.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/concrete_model/simulation_mode/utils.py` & `mimosa-0.1.1/mimosa/concrete_model/simulation_mode/utils.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/export/__pycache__/plot.cpython-310.pyc` & `mimosa-0.1.1/mimosa/export/__pycache__/plot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/export/__pycache__/save.cpython-310.pyc` & `mimosa-0.1.1/mimosa/export/__pycache__/save.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/export/__pycache__/utils.cpython-310.pyc` & `mimosa-0.1.1/mimosa/export/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/export/plot.py` & `mimosa-0.1.1/mimosa/export/plot.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/export/save.py` & `mimosa-0.1.1/mimosa/export/save.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/export/utils.py` & `mimosa-0.1.1/mimosa/export/utils.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/inputdata/config/config_R5.yaml` & `mimosa-0.1.1/mimosa/inputdata/config/config_R5.yaml`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/inputdata/config/config_default.yaml` & `mimosa-0.1.1/mimosa/inputdata/config/config_default.yaml`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/inputdata/data/data_IMAGE_SSP.csv` & `mimosa-0.1.1/mimosa/inputdata/data/data_IMAGE_SSP.csv`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/inputdata/data/data_IMAGE_SSP_harmonised_2020.csv` & `mimosa-0.1.1/mimosa/inputdata/data/data_IMAGE_SSP_harmonised_2020.csv`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/inputdata/params/ADRICE2012.csv` & `mimosa-0.1.1/mimosa/inputdata/params/ADRICE2012.csv`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/inputdata/params/COACCH.csv` & `mimosa-0.1.1/mimosa/inputdata/params/COACCH.csv`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/inputdata/params/mac.csv` & `mimosa-0.1.1/mimosa/inputdata/params/mac.csv`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/inputdata/regions/IMAGE26_regions.json` & `mimosa-0.1.1/mimosa/inputdata/regions/IMAGE26_regions.json`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/inputdata/regions/R5_regions.json` & `mimosa-0.1.1/mimosa/inputdata/regions/R5_regions.json`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/inputdata/regions/country_ISO_codes.csv` & `mimosa-0.1.1/mimosa/inputdata/regions/country_ISO_codes.csv`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/mimosa.py` & `mimosa-0.1.1/mimosa/mimosa.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa/socialcostofcarbon/scc.py` & `mimosa-0.1.1/mimosa/socialcostofcarbon/scc.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/mimosa.egg-info/PKG-INFO` & `mimosa-0.1.1/mimosa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimosa
-Version: 0.1.0
+Version: 0.1.1
 Summary: MIMOSA: Integrated Assessment Model for Cost-Benefit Analysis
 Author: Kaj-Ivar van der Wijst
 Author-email: k.i.vanderwijst@gmail.com
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mimosa-0.1.0/mimosa.egg-info/SOURCES.txt` & `mimosa-0.1.1/mimosa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.0/setup.py` & `mimosa-0.1.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 with open("README.md") as fh:
     description = fh.read()
 
 setup(
     name="mimosa",
-    version="0.1.0",
+    version="0.1.1",
     author="Kaj-Ivar van der Wijst",
     author_email="k.i.vanderwijst@gmail.com",
     packages=["mimosa"],
     # url="http://pypi.python.org/pypi/PackageName/",
     license="LICENSE.txt",
     description="MIMOSA: Integrated Assessment Model for Cost-Benefit Analysis",
     long_description=description,
     long_description_content_type="text/markdown",
-    install_requires=["numpy", "pandas", "pyomo", "pint", "pyyaml"],
+    install_requires=["numpy", "pandas", "pyomo", "pint", "pyyaml", "scipy"],
     include_package_data=True,
 )
```

